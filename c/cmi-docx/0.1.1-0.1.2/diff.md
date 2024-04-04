# Comparing `tmp/cmi_docx-0.1.1.tar.gz` & `tmp/cmi_docx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmi_docx-0.1.1.tar", max compression
+gzip compressed data, was "cmi_docx-0.1.2.tar", max compression
```

## Comparing `cmi_docx-0.1.1.tar` & `cmi_docx-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    26526 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/LICENSE
--rw-r--r--   0        0        0     2762 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/README.md
--rw-r--r--   0        0        0     1557 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      295 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/__init__.py
--rw-r--r--   0        0        0     4801 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/document.py
--rw-r--r--   0        0        0     4925 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/paragraph.py
--rw-r--r--   0        0        0     4253 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/run.py
--rw-r--r--   0        0        0     2347 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/table.py
--rw-r--r--   0        0        0      440 2024-04-03 15:40:59.468700 cmi_docx-0.1.1/src/cmi_docx/utils.py
--rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 cmi_docx-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2762 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/README.md
+-rw-r--r--   0        0        0     1557 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      295 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/__init__.py
+-rw-r--r--   0        0        0     4921 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/document.py
+-rw-r--r--   0        0        0     4925 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/paragraph.py
+-rw-r--r--   0        0        0     4253 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/run.py
+-rw-r--r--   0        0        0     2684 2024-04-04 17:49:39.103690 cmi_docx-0.1.2/src/cmi_docx/table.py
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 cmi_docx-0.1.2/PKG-INFO
```

### Comparing `cmi_docx-0.1.1/LICENSE` & `cmi_docx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.1/README.md` & `cmi_docx-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.1/pyproject.toml` & `cmi_docx-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmi_docx"
-version = "0.1.1"
+version = "0.1.2"
 description = ".docx utilities"
 authors = ["Reinder Vos de Wael <reinder.vosdewael@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "cmi_docx", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cmi_docx-0.1.1/src/cmi_docx/document.py` & `cmi_docx-0.1.2/src/cmi_docx/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,16 @@
             index: The index to insert the paragraph at.
             text: The text to insert.
             style: The style to apply to the text.
 
         Returns:
             The new paragraph.
         """
-        new_paragraph = self._insert_empty_paragraph(index)
-        new_paragraph.add_run(text, style=style)
+        new_paragraph = self._insert_empty_paragraph(index, style)
+        new_paragraph.add_run(text)
         return new_paragraph
 
     def insert_paragraph_by_object(
         self,
         index: int,
         paragraph: docx_paragraph.Paragraph,
     ) -> docx_paragraph.Paragraph:
@@ -93,15 +93,15 @@
             paragraph: The paragraph to insert.
 
         Returns:
             The new paragraph.
         """
         new_paragraph = self._insert_empty_paragraph(index)
         for paragraph_run in paragraph.runs:
-            new_paragraph.add_run(paragraph_run.text, paragraph_run.style)
+            new_paragraph.add_run(paragraph_run.text)
         return new_paragraph
 
     def insert_image(
         self,
         index: int,
         image_path: str | pathlib.Path,
         width: int | None = None,
@@ -127,28 +127,32 @@
 
         for section in self.document.sections:
             all_paragraphs.extend(
                 (*section.footer.paragraphs, *section.header.paragraphs)
             )
         return all_paragraphs
 
-    def _insert_empty_paragraph(self, index: int) -> docx_paragraph.Paragraph:
+    def _insert_empty_paragraph(
+        self, index: int, style: str | None = None
+    ) -> docx_paragraph.Paragraph:
         """Inserts an empty paragraph at a given index.
 
         Args:
             index: The index to insert the paragraph at.
+            style: The style to apply to the paragraph.
 
         Returns:
             The new paragraph.
         """
         n_paragraphs = len(self.document.paragraphs)
         if index > n_paragraphs:
             raise ValueError(f"Index {index} is out of range.")
 
         if index == n_paragraphs:
-            new_paragraph = self.document.add_paragraph()
+            new_paragraph = self.document.add_paragraph(style=style)
         else:
             new_paragraph = new_paragraph = self.document.paragraphs[
                 index
             ]._insert_paragraph_before()
+            new_paragraph.style = style
 
         return new_paragraph
```

### Comparing `cmi_docx-0.1.1/src/cmi_docx/paragraph.py` & `cmi_docx-0.1.2/src/cmi_docx/paragraph.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.1/src/cmi_docx/run.py` & `cmi_docx-0.1.2/src/cmi_docx/run.py`

 * *Files identical despite different names*

### Comparing `cmi_docx-0.1.1/PKG-INFO` & `cmi_docx-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmi_docx
-Version: 0.1.1
+Version: 0.1.2
 Summary: .docx utilities
 License: LGPL-2.1
 Author: Reinder Vos de Wael
 Author-email: reinder.vosdewael@childmind.org
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

