# Comparing `tmp/amilib-0.0.1a3.tar.gz` & `tmp/amilib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amilib-0.0.1a3.tar", last modified: Mon Apr  1 17:08:54 2024, max compression
+gzip compressed data, was "dist/amilib-0.0.2.tar", last modified: Thu Apr  4 14:52:03 2024, max compression
```

## Comparing `amilib-0.0.1a3.tar` & `amilib-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 17:08:54.411780 amilib-0.0.1a3/
--rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-03-27 16:20:01.000000 amilib-0.0.1a3/LICENSE
--rw-r--r--   0 pm286      (503) staff       (20)      818 2024-04-01 17:08:54.411651 amilib-0.0.1a3/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)       76 2024-03-27 16:22:55.000000 amilib-0.0.1a3/README.md
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 17:08:54.409358 amilib-0.0.1a3/amilib/
--rw-r--r--   0 pm286      (503) staff       (20)        0 2024-03-27 18:27:17.000000 amilib-0.0.1a3/amilib/__init__.py
--rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/ami_bib.py
--rw-r--r--   0 pm286      (503) staff       (20)      285 2024-04-01 09:12:21.000000 amilib-0.0.1a3/amilib/ami_csv.py
--rw-r--r--   0 pm286      (503) staff       (20)   168207 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/ami_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    16712 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/ami_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)     8293 2024-03-31 19:36:35.000000 amilib-0.0.1a3/amilib/ami_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    27357 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/ami_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)    82090 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/ami_pdf_libs.py
--rw-r--r--   0 pm286      (503) staff       (20)     4978 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/ami_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-03-31 14:07:47.000000 amilib-0.0.1a3/amilib/ami_util.py
--rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-03-31 17:50:56.000000 amilib-0.0.1a3/amilib/amidriver.py
--rw-r--r--   0 pm286      (503) staff       (20)    50146 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/amix.py
--rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/bbox.py
--rw-r--r--   0 pm286      (503) staff       (20)    14093 2024-03-28 20:25:22.000000 amilib-0.0.1a3/amilib/file_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)    16712 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/html_generator.py
--rw-r--r--   0 pm286      (503) staff       (20)    48233 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/html_marker.py
--rw-r--r--   0 pm286      (503) staff       (20)    36840 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/util.py
--rw-r--r--   0 pm286      (503) staff       (20)    35077 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/wikimedia.py
--rw-r--r--   0 pm286      (503) staff       (20)    54688 2024-04-01 09:44:34.000000 amilib-0.0.1a3/amilib/xml_lib.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 17:08:54.410307 amilib-0.0.1a3/amilib.egg-info/
--rw-r--r--   0 pm286      (503) staff       (20)      818 2024-04-01 17:08:53.000000 amilib-0.0.1a3/amilib.egg-info/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)      783 2024-04-01 17:08:54.000000 amilib-0.0.1a3/amilib.egg-info/SOURCES.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-01 17:08:54.000000 amilib-0.0.1a3/amilib.egg-info/dependency_links.txt
--rw-r--r--   0 pm286      (503) staff       (20)       44 2024-04-01 17:08:54.000000 amilib-0.0.1a3/amilib.egg-info/entry_points.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-01 17:07:33.000000 amilib-0.0.1a3/amilib.egg-info/not-zip-safe
--rw-r--r--   0 pm286      (503) staff       (20)      111 2024-04-01 17:08:54.000000 amilib-0.0.1a3/amilib.egg-info/requires.txt
--rw-r--r--   0 pm286      (503) staff       (20)        7 2024-04-01 17:08:54.000000 amilib-0.0.1a3/amilib.egg-info/top_level.txt
--rw-r--r--   0 pm286      (503) staff       (20)       38 2024-04-01 17:08:54.411824 amilib-0.0.1a3/setup.cfg
--rw-r--r--   0 pm286      (503) staff       (20)     1630 2024-04-01 17:08:49.000000 amilib-0.0.1a3/setup.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-01 17:08:54.411498 amilib-0.0.1a3/test/
--rw-r--r--   0 pm286      (503) staff       (20)     7614 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_all.py
--rw-r--r--   0 pm286      (503) staff       (20)     5098 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_file.py
--rw-r--r--   0 pm286      (503) staff       (20)    38379 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_headless.py
--rw-r--r--   0 pm286      (503) staff       (20)   121224 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_html.py
--rw-r--r--   0 pm286      (503) staff       (20)     1133 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    80006 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10141 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    35925 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_wikidata.py
--rw-r--r--   0 pm286      (503) staff       (20)     1973 2024-04-01 09:44:34.000000 amilib-0.0.1a3/test/test_xml.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-04 14:52:03.749619 amilib-0.0.2/
+-rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-03-27 16:20:01.000000 amilib-0.0.2/LICENSE
+-rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-04 14:52:03.749414 amilib-0.0.2/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)       76 2024-03-27 16:22:55.000000 amilib-0.0.2/README.md
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-04 14:52:03.743245 amilib-0.0.2/amilib/
+-rw-r--r--   0 pm286      (503) staff       (20)        0 2024-03-27 18:27:17.000000 amilib-0.0.2/amilib/__init__.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/ami_bib.py
+-rw-r--r--   0 pm286      (503) staff       (20)      285 2024-04-01 09:12:21.000000 amilib-0.0.2/amilib/ami_csv.py
+-rw-r--r--   0 pm286      (503) staff       (20)   168207 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/ami_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16712 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/ami_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8293 2024-03-31 19:36:35.000000 amilib-0.0.2/amilib/ami_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    27357 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/ami_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)    82090 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/ami_pdf_libs.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4978 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/ami_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-03-31 14:07:47.000000 amilib-0.0.2/amilib/ami_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-03-31 17:50:56.000000 amilib-0.0.2/amilib/amidriver.py
+-rw-r--r--   0 pm286      (503) staff       (20)    49418 2024-04-04 14:51:17.000000 amilib-0.0.2/amilib/amix.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/bbox.py
+-rw-r--r--   0 pm286      (503) staff       (20)    14093 2024-03-28 20:25:22.000000 amilib-0.0.2/amilib/file_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16712 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/html_generator.py
+-rw-r--r--   0 pm286      (503) staff       (20)    48233 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/html_marker.py
+-rw-r--r--   0 pm286      (503) staff       (20)    36840 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    35077 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/wikimedia.py
+-rw-r--r--   0 pm286      (503) staff       (20)    54688 2024-04-01 09:44:34.000000 amilib-0.0.2/amilib/xml_lib.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-04 14:52:03.744607 amilib-0.0.2/amilib.egg-info/
+-rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-04 14:52:03.000000 amilib-0.0.2/amilib.egg-info/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)      783 2024-04-04 14:52:03.000000 amilib-0.0.2/amilib.egg-info/SOURCES.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-04 14:52:03.000000 amilib-0.0.2/amilib.egg-info/dependency_links.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       44 2024-04-04 14:52:03.000000 amilib-0.0.2/amilib.egg-info/entry_points.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-02 16:57:37.000000 amilib-0.0.2/amilib.egg-info/not-zip-safe
+-rw-r--r--   0 pm286      (503) staff       (20)      125 2024-04-04 14:52:03.000000 amilib-0.0.2/amilib.egg-info/requires.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        7 2024-04-04 14:52:03.000000 amilib-0.0.2/amilib.egg-info/top_level.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       38 2024-04-04 14:52:03.749683 amilib-0.0.2/setup.cfg
+-rw-r--r--   0 pm286      (503) staff       (20)     1651 2024-04-04 14:51:17.000000 amilib-0.0.2/setup.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-04 14:52:03.748959 amilib-0.0.2/test/
+-rw-r--r--   0 pm286      (503) staff       (20)     7614 2024-04-01 09:44:34.000000 amilib-0.0.2/test/test_all.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5098 2024-04-01 09:44:34.000000 amilib-0.0.2/test/test_file.py
+-rw-r--r--   0 pm286      (503) staff       (20)    38235 2024-04-03 14:46:19.000000 amilib-0.0.2/test/test_headless.py
+-rw-r--r--   0 pm286      (503) staff       (20)   121224 2024-04-01 09:44:34.000000 amilib-0.0.2/test/test_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1349 2024-04-03 14:27:01.000000 amilib-0.0.2/test/test_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    80006 2024-04-01 09:44:34.000000 amilib-0.0.2/test/test_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-01 09:44:34.000000 amilib-0.0.2/test/test_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10324 2024-04-02 21:34:31.000000 amilib-0.0.2/test/test_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    35925 2024-04-01 09:44:34.000000 amilib-0.0.2/test/test_wikidata.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1973 2024-04-01 09:44:34.000000 amilib-0.0.2/test/test_xml.py
```

### Comparing `amilib-0.0.1a3/LICENSE` & `amilib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/PKG-INFO` & `amilib-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.0.1a3
+Version: 0.0.2
 Summary: document download, cleaning, managemenr
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.0.1a3/amilib/ami_bib.py` & `amilib-0.0.2/amilib/ami_bib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/ami_html.py` & `amilib-0.0.2/amilib/ami_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/ami_integrate.py` & `amilib-0.0.2/amilib/ami_integrate.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/ami_nlp.py` & `amilib-0.0.2/amilib/ami_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/ami_pdf.py` & `amilib-0.0.2/amilib/ami_pdf.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/ami_pdf_libs.py` & `amilib-0.0.2/amilib/ami_pdf_libs.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/ami_svg.py` & `amilib-0.0.2/amilib/ami_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/ami_util.py` & `amilib-0.0.2/amilib/ami_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/amidriver.py` & `amilib-0.0.2/amilib/amidriver.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/amix.py` & `amilib-0.0.2/amilib/amix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1153,45 +1153,22 @@
     def version(self):
         """
         reads setup.py and extracts line of form version='0.0.29'
         This is still a mess. We need to set the version once somewhere.
         """
 
         version = '0.0.1a1'  # 2024-03-27
+        version = '0.0.1a3'  # 2024-03-27
+        version = '0.0.1'  # 2024-04-03
+        version = '0.0.2'  # 2024-04-04
 
         # logging.warn(f"VERSION {version}")
         return version
 
 
-# class ContentStore:
-#     """holds path-related content
-#
-#     replaces earlier pyamihtmlx.file_dict
-#     uses a dict
-#     at presemt the key is the path(name) and the value is either the content or None
-#     """
-#
-#     def __init__(self, pyami):
-#         self.pyami = pyami
-#         self.file_dict = {}
-#
-#     def add_files(self, files, add_contents=False):
-#         for file in files:
-#             self.add_file(file, add_contents)
-#
-#     def add_file(self, file, add_contents=False):
-#         self.file_dict[file] = self.get_contents(file) if add_contents else None
-#
-#     def keys(self):
-#         return self.file_dict.keys() if self.file_dict is not None else None
-#
-#     def get_file_contents(self, file):
-#         """return dictionary or None"""
-#         return self.file_dict.get(file)
-#
 
 class AmiLibArgs(AbstractArgs):
     """Parse args to analyze, edit and annotate HTML"""
 
     def __init__(self):
         """arg_dict is set to default"""
         super().__init__()
@@ -1308,28 +1285,28 @@
 
 
 def main():
     # make_cmd()
     """ main entry point for cmdline
 
     """
-    # print(f"PYAMI")
-    run_dsl = False
+    print(f"PYAMI")
     run_tests = False  # needs re-implementing
 
     run_commands = True
     #    run_commands = False
+
     #    run_tests = True
 
-    # AmiLib.logger.debug(
-    #     f"\n============== running pyami main ===============\n{sys.argv[1:]}")
-    # amix = AmiLib()
-    # print(f"***** PYAMI VERSION {amix.version()} *****")
-    # # this needs commandline
-    # if run_commands:
-    #     amix.run_command(sys.argv[1:])
+    AmiLib.logger.debug(
+        f"\n============== running pyami main ===============\n{sys.argv[1:]}")
+    amix = AmiLib()
+    print(f"***** PYAMI VERSION {amix.version()} *****")
+    # this needs commandline
+    if run_commands:
+        amix.run_command(sys.argv[1:])
 
 
 if __name__ == "__main__":
 
     main()
```

### Comparing `amilib-0.0.1a3/amilib/bbox.py` & `amilib-0.0.2/amilib/bbox.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/file_lib.py` & `amilib-0.0.2/amilib/file_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/html_generator.py` & `amilib-0.0.2/amilib/html_generator.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/html_marker.py` & `amilib-0.0.2/amilib/html_marker.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/util.py` & `amilib-0.0.2/amilib/util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/wikimedia.py` & `amilib-0.0.2/amilib/wikimedia.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib/xml_lib.py` & `amilib-0.0.2/amilib/xml_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/amilib.egg-info/PKG-INFO` & `amilib-0.0.2/amilib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.0.1a3
+Version: 0.0.2
 Summary: document download, cleaning, managemenr
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.0.1a3/amilib.egg-info/SOURCES.txt` & `amilib-0.0.2/amilib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/setup.py` & `amilib-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,36 +6,38 @@
 # with open('requirements.txt') as f:
 #    required = f.read().splitlines()
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 long_desc = """
-amilib is a library for dowloading, cleaning, annotating, documents fo various sorts (HTML, PDF, XML)"""
+amilib is a library for downloading, cleaning, annotating, documents fo various sorts (HTML, PDF, XML)"""
 
 requirements = [
  'lxml',
  'nltk',
  'pdfminer3',
  'Pillow',
  'setuptools',
  'pdfplumber',
  'requests',
  'numpy',
  'pandas',
+ 'pyvis',
  'selenium',
+ 'tinycss',
  'webdriver-manager',
  'scikit-learn',
 
 ]
 
 setup(
     name='amilib',
     url='https://github.com/petermr/amilib',
-    version='0.0.1a3',
+    version='0.0.2',
     description='document download, cleaning, managemenr',
     long_description_content_type='text/markdown',
     long_description=readme,
     author="Peter Murray-Rust",
     author_email='petermurrayrust@googlemail.com',
     license='Apache2',
     install_requires=requirements,
```

### Comparing `amilib-0.0.1a3/test/test_all.py` & `amilib-0.0.2/test/test_all.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/test/test_file.py` & `amilib-0.0.2/test/test_file.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/test/test_headless.py` & `amilib-0.0.2/test/test_headless.py`

 * *Files 0% similar despite different names*

```diff
@@ -880,39 +880,34 @@
                 term = entry.text
                 print(f"entry: {i}; term {term}")
                 wikidata_lookup = WikidataLookup()
                 qitem0, desc, wikidata_hits = wikidata_lookup.lookup_wikidata(term)
                 print(f"qitem {qitem0, desc}")
                 wikiwriter.writerow([term, qitem0, desc, wikidata_hits])
 
+    @unittest.skip("no idea what this does - I only wrote it!")
     def test_abbreviations_wikimedia_WIKI(self):
         """
         reads an acronym file as CSV and looks up entries in Wikidata and Wikipedia
         TODO move elsewhere
         """
         abbrev_file = Path(TOTAL_GLOSS_DIR, "glossaries", "total", "acronyms.csv")
         print(f"looking up acronym file {abbrev_file} in Wikidata")
         offset = 1000
         count = 0
         MAXCOUNT = 3
-        for start in range(0, 1700, offset):
-            count += 1
-            if count > MAXCOUNT:
-                break
-            end = start + offset
+        for start in range(0, 3):
             lookup = WikidataLookup()
             output_file = Path(TOTAL_GLOSS_DIR, "glossaries", "total", f"acronyms_wiki_{start}_{end}.csv")
             with open(output_file, "w") as fout:
                 csvwriter = csv.writer(fout)
                 csvwriter.writerow(['abb', 'term', 'qid', 'desc', 'hits'])
                 with open(abbrev_file, newline='') as input:
                     csvreader = csv.reader(input)
                     for i, row in enumerate(csvreader):
-                        if i < start or i > end:
-                            continue
                         abb = row[0]
                         term = row[1]
                         qitem0, desc, hits = lookup.lookup_wikidata(term)
                         if qitem0 is None:
                             print(f"failed on text: {row}")
                             # qitem0, desc, hits = lookup.lookup_wikidata(abb)
                             if qitem0 is None:
```

### Comparing `amilib-0.0.1a3/test/test_html.py` & `amilib-0.0.2/test/test_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/test/test_pdf.py` & `amilib-0.0.2/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/test/test_svg.py` & `amilib-0.0.2/test/test_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/test/test_util.py` & `amilib-0.0.2/test/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,27 +99,31 @@
         try:
             _, v = Util.create_name_value(arg, delim=" ")
             raise ValueError(f"failed to trap {arg}")
         except ValueError as ve:
             assert str(ve) == f"arg [{arg}] may not contain whitespace"
 
     def test_read_csv(self):
-        """use Python csv to select column values"""
+        """
+        use Python csv to select column values
+        Reads compound_enzyme.csv into CSV DictReader and checks values in first 3 rows
+        with column names "NAME" and "TYPE"
+        """
         csv_file = Path(Resources.TEST_RESOURCES_DIR, "eoCompound", "compound_enzyme.csv")
         assert csv_file.exists(), f"{csv_file} should exist"
+        expected_row_values = [["isopentenyl diphosphate", "COMPOUND"],
+                               ["dimethylallyl diphosphate", "COMPOUND"],
+                               ["hemiterpene", "COMPOUND"]]
         with open(str(csv_file), newline='') as csvfile:
-            row_values = [["isopentenyl diphosphate", "COMPOUND"],
-                          ["dimethylallyl diphosphate", "COMPOUND"],
-                          ["hemiterpene", "COMPOUND"]]
             reader = csv.DictReader(csvfile)
 
             for i, row in enumerate(reader):
                 if i < 3:
-                    assert row['NAME'] == row_values[i][0]
-                    assert row['TYPE'] == row_values[i][1]
+                    assert row['NAME'] == expected_row_values[i][0]
+                    assert row['TYPE'] == expected_row_values[i][1]
 
     def test_select_csv_field_by_type(self):
         """select value in column of csv file by value of defining column
         """
         csv_file = Path(Resources.TEST_RESOURCES_DIR, "eoCompound", "compound_enzyme.csv")
         assert csv_file.exists(), f"{csv_file} should exist"
         selector_column = "TYPE"
```

### Comparing `amilib-0.0.1a3/test/test_wikidata.py` & `amilib-0.0.2/test/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.1a3/test/test_xml.py` & `amilib-0.0.2/test/test_xml.py`

 * *Files identical despite different names*

