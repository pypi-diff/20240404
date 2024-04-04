# Comparing `tmp/tcia_utils-2.1.0.tar.gz` & `tmp/tcia_utils-2.1.1.tar.gz`

## Comparing `tcia_utils-2.1.0.tar` & `tcia_utils-2.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/__init__.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/datacite.py
--rw-r--r--   0        0        0    87232 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/nbia.py
--rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/pathdb.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/utils.py
--rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/src/tcia_utils/wordpress.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/LICENSE
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 tcia_utils-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/__init__.py
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/datacite.py
+-rw-r--r--   0        0        0    87232 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/nbia.py
+-rw-r--r--   0        0        0    10726 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/pathdb.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/utils.py
+-rw-r--r--   0        0        0    13674 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/src/tcia_utils/wordpress.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/LICENSE
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 tcia_utils-2.1.1/PKG-INFO
```

### Comparing `tcia_utils-2.1.0/src/tcia_utils/datacite.py` & `tcia_utils-2.1.1/src/tcia_utils/datacite.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.0/src/tcia_utils/nbia.py` & `tcia_utils-2.1.1/src/tcia_utils/nbia.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.0/src/tcia_utils/pathdb.py` & `tcia_utils-2.1.1/src/tcia_utils/pathdb.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.0/src/tcia_utils/utils.py` & `tcia_utils-2.1.1/src/tcia_utils/utils.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.0/src/tcia_utils/wordpress.py` & `tcia_utils-2.1.1/src/tcia_utils/wordpress.py`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.0/.gitignore` & `tcia_utils-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.0/LICENSE` & `tcia_utils-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.0/README.md` & `tcia_utils-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tcia_utils-2.1.0/pyproject.toml` & `tcia_utils-2.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcia_utils"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
   { name="Justin Kirby", email="justin.kirby@nih.gov" },
 ]
 description = "A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tcia_utils-2.1.0/PKG-INFO` & `tcia_utils-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tcia_utils
-Version: 2.1.0
+Version: 2.1.1
 Summary: A package to simplify common tasks one might perform when interacting with The Cancer Imaging Archive (TCIA) via Jupyter/Python.
 Project-URL: Homepage, https://github.com/kirbyju/tcia_utils
 Project-URL: Bug Tracker, https://github.com/kirbyju/tcia_utils/issues
 Author-email: Justin Kirby <justin.kirby@nih.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

