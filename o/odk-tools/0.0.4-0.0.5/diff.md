# Comparing `tmp/odk_tools-0.0.4.tar.gz` & `tmp/odk_tools-0.0.5.tar.gz`

## Comparing `odk_tools-0.0.4.tar` & `odk_tools-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.0.4/src/odk_tools/__init__.py
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 odk_tools-0.0.4/src/odk_tools/classes.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 odk_tools-0.0.4/src/odk_tools/functions.py
--rw-r--r--   0        0        0    20194 2020-02-02 00:00:00.000000 odk_tools-0.0.4/src/odk_tools/odk.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.0.4/LICENSE
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 odk_tools-0.0.4/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 odk_tools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 odk_tools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 odk_tools-0.0.5/src/odk_tools/__init__.py
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 odk_tools-0.0.5/src/odk_tools/classes.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 odk_tools-0.0.5/src/odk_tools/functions.py
+-rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 odk_tools-0.0.5/src/odk_tools/odk.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 odk_tools-0.0.5/LICENSE
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 odk_tools-0.0.5/README.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 odk_tools-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 odk_tools-0.0.5/PKG-INFO
```

### Comparing `odk_tools-0.0.4/src/odk_tools/classes.py` & `odk_tools-0.0.5/src/odk_tools/classes.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.4/src/odk_tools/functions.py` & `odk_tools-0.0.5/src/odk_tools/functions.py`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.4/src/odk_tools/odk.py` & `odk_tools-0.0.5/src/odk_tools/odk.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import copy
 import datetime as dt
 import zipfile as zip
 import xlsxwriter
 import xml.etree.ElementTree as ET
 import uuid
 from types import FunctionType
-from classes import Form
+from .classes import Form
 
 def save_to_excel(data, filename="output.xlsx", column_width=25, include_index=False, row_colours={0: "#D8E4BC", 1: "#C5D9F1"}, row_bold=[0], row_wrap=[1], autofilter=True, freeze_panes=True):
 
     workbook = xlsxwriter.Workbook(filename)
     worksheet = workbook.add_worksheet()
 
     for i in range(len(data.columns)):
```

### Comparing `odk_tools-0.0.4/LICENSE` & `odk_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `odk_tools-0.0.4/pyproject.toml` & `odk_tools-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "odk_tools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for interacting with an ODK server and uploading/downloading submissions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `odk_tools-0.0.4/PKG-INFO` & `odk_tools-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: odk_tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of tools for interacting with an ODK server and uploading/downloading submissions
 Project-URL: Homepage, https://github.com/federlorenz/odk_tools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

