# Comparing `tmp/energyml_utils-0.0.1.dev2.tar.gz` & `tmp/energyml_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyml_utils-0.0.1.dev2.tar", max compression
+gzip compressed data, was "energyml_utils-1.0.0.tar", max compression
```

## Comparing `energyml_utils-0.0.1.dev2.tar` & `energyml_utils-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11338 2024-04-04 02:20:27.625834 energyml_utils-0.0.1.dev2/LICENSE
--rw-r--r--   0        0        0      855 2024-04-04 02:20:27.625834 energyml_utils-0.0.1.dev2/README.md
--rw-r--r--   0        0        0     3076 2024-04-04 02:20:27.685834 energyml_utils-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0       74 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/__init__.py
--rw-r--r--   0        0        0      514 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/__init__.py
--rw-r--r--   0        0        0      281 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/data/__init__.py
--rw-r--r--   0        0        0     5895 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/data/hdf.py
--rw-r--r--   0        0        0    17632 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/data/helper.py
--rw-r--r--   0        0        0    19741 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/data/mesh.py
--rw-r--r--   0        0        0    22114 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/epc.py
--rw-r--r--   0        0        0    30269 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/introspection.py
--rw-r--r--   0        0        0     7655 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/manager.py
--rw-r--r--   0        0        0     2998 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/serialization.py
--rw-r--r--   0        0        0    13604 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/validation.py
--rw-r--r--   0        0        0     6411 2024-04-04 02:20:27.693834 energyml_utils-0.0.1.dev2/src/energyml/utils/xml.py
--rw-r--r--   0        0        0     2486 1970-01-01 00:00:00.000000 energyml_utils-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-04-04 14:33:10.568410 energyml_utils-1.0.0/LICENSE
+-rw-r--r--   0        0        0      855 2024-04-04 14:33:10.568410 energyml_utils-1.0.0/README.md
+-rw-r--r--   0        0        0     3073 2024-04-04 14:33:41.101194 energyml_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/__init__.py
+-rw-r--r--   0        0        0      281 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/data/__init__.py
+-rw-r--r--   0        0        0     5895 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/data/hdf.py
+-rw-r--r--   0        0        0    17632 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/data/helper.py
+-rw-r--r--   0        0        0    19741 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/data/mesh.py
+-rw-r--r--   0        0        0    22114 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/epc.py
+-rw-r--r--   0        0        0    30269 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/introspection.py
+-rw-r--r--   0        0        0     7655 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/manager.py
+-rw-r--r--   0        0        0     2998 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/serialization.py
+-rw-r--r--   0        0        0    13604 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/validation.py
+-rw-r--r--   0        0        0     6411 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/xml.py
+-rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 energyml_utils-1.0.0/PKG-INFO
```

### Comparing `energyml_utils-0.0.1.dev2/LICENSE` & `energyml_utils-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/README.md` & `energyml_utils-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/pyproject.toml` & `energyml_utils-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
-#requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
-#build-backend = "poetry_dynamic_versioning.backend"
-requires = ["setuptools"]
-build-backend = "setuptools.build_meta"
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
+# requires = ["setuptools"]
+# build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "energyml-utils"
-version = "0.0.1.dev2" # Set at build time
+version = "1.0.0" # Set at build time
 description = "Energyml helper"
 authors = [
     "Valentin Gauthier <valentin.gauthier@geosiris.com>"
 ]
 maintainers = [
     "Valentin Gauthier <valentin.gauthier@geosiris.com>"
 ]
```

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/__init__.py` & `energyml_utils-1.0.0/src/energyml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/data/hdf.py` & `energyml_utils-1.0.0/src/energyml/utils/data/hdf.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/data/helper.py` & `energyml_utils-1.0.0/src/energyml/utils/data/helper.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/data/mesh.py` & `energyml_utils-1.0.0/src/energyml/utils/data/mesh.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/epc.py` & `energyml_utils-1.0.0/src/energyml/utils/epc.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/introspection.py` & `energyml_utils-1.0.0/src/energyml/utils/introspection.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/manager.py` & `energyml_utils-1.0.0/src/energyml/utils/manager.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/serialization.py` & `energyml_utils-1.0.0/src/energyml/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/validation.py` & `energyml_utils-1.0.0/src/energyml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/src/energyml/utils/xml.py` & `energyml_utils-1.0.0/src/energyml/utils/xml.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-0.0.1.dev2/PKG-INFO` & `energyml_utils-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyml-utils
-Version: 0.0.1.dev2
+Version: 1.0.0
 Summary: Energyml helper
 Home-page: http://www.geosiris.com
 License: Apache-2.0
 Keywords: energyml,resqml,witsml,prodml
 Author: Valentin Gauthier
 Author-email: valentin.gauthier@geosiris.com
 Maintainer: Valentin Gauthier
```

