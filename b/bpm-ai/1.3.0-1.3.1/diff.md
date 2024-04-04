# Comparing `tmp/bpm_ai-1.3.0.tar.gz` & `tmp/bpm_ai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpm_ai-1.3.0.tar", max compression
+gzip compressed data, was "bpm_ai-1.3.1.tar", max compression
```

## Comparing `bpm_ai-1.3.0.tar` & `bpm_ai-1.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      932 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/common/__init__.py
--rw-r--r--   0        0        0      143 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/common/errors.py
--rw-r--r--   0        0        0     1034 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/common/multimodal.py
--rw-r--r--   0        0        0        0 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/__init__.py
--rw-r--r--   0        0        0     1509 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/compose.anthropic.prompt
--rw-r--r--   0        0        0     1369 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/compose.openai.prompt
--rw-r--r--   0        0        0     3575 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/compose.py
--rw-r--r--   0        0        0      738 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/compose/util.py
--rw-r--r--   0        0        0        0 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/__init__.py
--rw-r--r--   0        0        0     3316 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/decide.anthropic.prompt
--rw-r--r--   0        0        0     3385 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/decide.openai.prompt
--rw-r--r--   0        0        0     4082 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/decide.py
--rw-r--r--   0        0        0     1986 2024-04-03 11:23:36.689689 bpm_ai-1.3.0/bpm_ai/decide/schema.py
--rw-r--r--   0        0        0        0 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/extract/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/extract/extract.anthropic.prompt
--rw-r--r--   0        0        0     1286 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/extract/extract.openai.prompt
--rw-r--r--   0        0        0     7210 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/extract/extract.py
--rw-r--r--   0        0        0        0 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/generic/__init__.py
--rw-r--r--   0        0        0      616 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/generic/generic.anthropic.prompt
--rw-r--r--   0        0        0      544 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/generic/generic.openai.prompt
--rw-r--r--   0        0        0     1486 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/generic/generic.py
--rw-r--r--   0        0        0        0 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/__init__.py
--rw-r--r--   0        0        0      160 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/schema.py
--rw-r--r--   0        0        0      576 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/translate.anthropic.prompt
--rw-r--r--   0        0        0      611 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/translate.openai.prompt
--rw-r--r--   0        0        0     3004 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/bpm_ai/translate/translate.py
--rw-r--r--   0        0        0     1355 2024-04-03 11:23:36.693689 bpm_ai-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 bpm_ai-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      932 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/common/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/common/errors.py
+-rw-r--r--   0        0        0     1034 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/common/multimodal.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/__init__.py
+-rw-r--r--   0        0        0     1509 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/compose.anthropic.prompt
+-rw-r--r--   0        0        0     1369 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/compose.openai.prompt
+-rw-r--r--   0        0        0     3575 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/compose.py
+-rw-r--r--   0        0        0      738 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/compose/util.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/__init__.py
+-rw-r--r--   0        0        0     3316 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/decide.anthropic.prompt
+-rw-r--r--   0        0        0     3385 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/decide.openai.prompt
+-rw-r--r--   0        0        0     4082 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/decide.py
+-rw-r--r--   0        0        0     1986 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/decide/schema.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/extract/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/extract/extract.anthropic.prompt
+-rw-r--r--   0        0        0     1286 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/extract/extract.openai.prompt
+-rw-r--r--   0        0        0     7210 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/extract/extract.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/generic/__init__.py
+-rw-r--r--   0        0        0      616 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/generic/generic.anthropic.prompt
+-rw-r--r--   0        0        0      544 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/generic/generic.openai.prompt
+-rw-r--r--   0        0        0     1486 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/generic/generic.py
+-rw-r--r--   0        0        0        0 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/__init__.py
+-rw-r--r--   0        0        0      160 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/schema.py
+-rw-r--r--   0        0        0      576 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/translate.anthropic.prompt
+-rw-r--r--   0        0        0      611 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/translate.openai.prompt
+-rw-r--r--   0        0        0     3004 2024-04-04 10:58:06.142568 bpm_ai-1.3.1/bpm_ai/translate/translate.py
+-rw-r--r--   0        0        0     1407 2024-04-04 10:58:06.146568 bpm_ai-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 bpm_ai-1.3.1/PKG-INFO
```

### Comparing `bpm_ai-1.3.0/README.md` & `bpm_ai-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/common/multimodal.py` & `bpm_ai-1.3.1/bpm_ai/common/multimodal.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/compose/compose.anthropic.prompt` & `bpm_ai-1.3.1/bpm_ai/compose/compose.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/compose/compose.openai.prompt` & `bpm_ai-1.3.1/bpm_ai/compose/compose.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/compose/compose.py` & `bpm_ai-1.3.1/bpm_ai/compose/compose.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/compose/util.py` & `bpm_ai-1.3.1/bpm_ai/compose/util.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/decide/decide.anthropic.prompt` & `bpm_ai-1.3.1/bpm_ai/decide/decide.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/decide/decide.openai.prompt` & `bpm_ai-1.3.1/bpm_ai/decide/decide.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/decide/decide.py` & `bpm_ai-1.3.1/bpm_ai/decide/decide.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/decide/schema.py` & `bpm_ai-1.3.1/bpm_ai/decide/schema.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/extract/extract.anthropic.prompt` & `bpm_ai-1.3.1/bpm_ai/extract/extract.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/extract/extract.openai.prompt` & `bpm_ai-1.3.1/bpm_ai/extract/extract.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/extract/extract.py` & `bpm_ai-1.3.1/bpm_ai/extract/extract.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/generic/generic.anthropic.prompt` & `bpm_ai-1.3.1/bpm_ai/generic/generic.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/generic/generic.openai.prompt` & `bpm_ai-1.3.1/bpm_ai/generic/generic.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/generic/generic.py` & `bpm_ai-1.3.1/bpm_ai/generic/generic.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/translate/translate.anthropic.prompt` & `bpm_ai-1.3.1/bpm_ai/translate/translate.anthropic.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/translate/translate.openai.prompt` & `bpm_ai-1.3.1/bpm_ai/translate/translate.openai.prompt`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/bpm_ai/translate/translate.py` & `bpm_ai-1.3.1/bpm_ai/translate/translate.py`

 * *Files identical despite different names*

### Comparing `bpm_ai-1.3.0/pyproject.toml` & `bpm_ai-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "bpm-ai"
-version = "1.3.0"
+version = "1.3.1"
 description = "AI task automation for BPM engines."
 authors = ["Bennet Krause <bennet.krause@holisticon.de>"]
 repository = "https://github.com/holunda-io/bpm-ai"
 homepage = "https://www.holisticon.de/"
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 bpm-ai-core = "2.2.0"
 openai = "^1.11.0"
-anthropic = "^0.20.0"
+anthropic = "^0.21.3"
 langfuse = "^2.13.3"
 amazon-textract-prettyprinter = "^0.1.9"
 aiobotocore = "^2.12.1"
 azure-storage-blob = "^12.19.1"
 azure-ai-translation-text = "^1.0.0b1"
 azure-ai-documentintelligence = "^1.0.0b2"
-
+langcodes = { version = "^3.3.0", extras = ["data"]}
 
 [tool.poetry.group.dev.dependencies]
 bpm-ai-inference = "0.2.2"
 torch = [
     { version = "=2.2.2", source="pypi", markers = "sys_platform == 'darwin'" },
     { version = "=2.2.2+cpu", source = "torch-cpu", markers = "sys_platform != 'darwin'" },
 ]
```

### Comparing `bpm_ai-1.3.0/PKG-INFO` & `bpm_ai-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: bpm-ai
-Version: 1.3.0
+Version: 1.3.1
 Summary: AI task automation for BPM engines.
 Home-page: https://www.holisticon.de/
 License: Apache-2.0
 Author: Bennet Krause
 Author-email: bennet.krause@holisticon.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiobotocore (>=2.12.1,<3.0.0)
 Requires-Dist: amazon-textract-prettyprinter (>=0.1.9,<0.2.0)
-Requires-Dist: anthropic (>=0.20.0,<0.21.0)
+Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: azure-ai-documentintelligence (>=1.0.0b2,<2.0.0)
 Requires-Dist: azure-ai-translation-text (>=1.0.0b1,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
 Requires-Dist: bpm-ai-core (==2.2.0)
+Requires-Dist: langcodes[data] (>=3.3.0,<4.0.0)
 Requires-Dist: langfuse (>=2.13.3,<3.0.0)
 Requires-Dist: openai (>=1.11.0,<2.0.0)
 Project-URL: Repository, https://github.com/holunda-io/bpm-ai
 Description-Content-Type: text/markdown
 
 # bpm-ai
 _AI task automation for BPM engines._
```

