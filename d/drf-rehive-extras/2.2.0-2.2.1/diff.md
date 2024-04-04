# Comparing `tmp/drf-rehive-extras-2.2.0.tar.gz` & `tmp/drf-rehive-extras-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-2.2.0.tar", last modified: Mon Nov  6 13:19:23 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-2.2.1.tar", last modified: Thu Apr  4 13:57:26 2024, max compression
```

## Comparing `drf-rehive-extras-2.2.0.tar` & `drf-rehive-extras-2.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      132 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      487 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6467 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)     5360 2023-11-06 13:07:48.000000 drf-rehive-extras-2.2.0/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      367 2023-07-27 16:27:26.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7163 2023-11-06 13:06:45.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)    15330 2023-07-27 16:27:26.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/schema.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2749 2023-11-06 13:08:18.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6873 2023-07-27 16:27:26.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-27 13:20:51.000000 drf-rehive-extras-2.2.0/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1776 2023-11-06 13:09:00.000000 drf-rehive-extras-2.2.0/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.2.0/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.2.0/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6467 2023-11-06 13:19:23.000000 drf-rehive-extras-2.2.0/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      132 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      487 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6467 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     5360 2023-11-06 13:07:48.000000 drf-rehive-extras-2.2.1/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      367 2023-07-27 16:27:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7163 2023-11-06 13:06:45.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)    15197 2024-04-04 13:53:30.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/schema.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2749 2023-11-06 13:08:18.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6873 2023-07-27 16:27:26.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2684 2023-07-27 13:20:51.000000 drf-rehive-extras-2.2.1/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1776 2024-04-04 13:51:55.000000 drf-rehive-extras-2.2.1/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.2.1/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.2.1/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6467 2024-04-04 13:57:26.000000 drf-rehive-extras-2.2.1/PKG-INFO
```

### Comparing `drf-rehive-extras-2.2.0/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-2.2.1/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.2.0
+Version: 2.2.1
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.2.0.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.2.1.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-2.2.0/README.md` & `drf-rehive-extras-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.2.0/drf_rehive_extras/mixins.py` & `drf-rehive-extras-2.2.1/drf_rehive_extras/mixins.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.2.0/drf_rehive_extras/schema.py` & `drf-rehive-extras-2.2.1/drf_rehive_extras/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,23 +101,16 @@
                     if not all_docs:
                         all_docs = {}
                     all_docs.update(docs)
 
         return all_docs
 
 
-@lru_cache(maxsize=None)
-def get_additional_documentation():
-    """
-    Method to get additional documentation.
-
-    Cache the result so it does not have to call it repeatedly.
-    """
-
-    return Documentation()
+# Create a module level singleton instance.
+additional_documentation = Documentation()
 
 
 # Extensions
 
 class OneOfOpenApiSerializerExtensionMixin():
     """
     Mixin for SerializerExtensions that must offer a oneOf interface.
@@ -162,15 +155,15 @@
         """
         Helper to get additional docs for a view.
 
         A `Documentation` instance must be found in settings.ADDITIONAL_DOCS.
         """
 
         try:
-            docs = get_additional_documentation().docs
+            docs = additional_documentation.docs
         except (NameError, AttributeError):
             return None
 
         # Create a key for the specific view and check if it exists.
         key = "{}.{}".format(self.view.__module__, self.view.__class__.__name__)
         try:
             return docs[key][self.method]
```

### Comparing `drf-rehive-extras-2.2.0/drf_rehive_extras/pagination.py` & `drf-rehive-extras-2.2.1/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.2.0/drf_rehive_extras/generics.py` & `drf-rehive-extras-2.2.1/drf_rehive_extras/generics.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.2.0/drf_rehive_extras/fields.py` & `drf-rehive-extras-2.2.1/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.2.0/setup.py` & `drf-rehive-extras-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '2.2.0'
+VERSION = '2.2.1'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-2.2.0/LICENSE` & `drf-rehive-extras-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-2.2.0/PKG-INFO` & `drf-rehive-extras-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 2.2.0
+Version: 2.2.1
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.2.0.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.2.1.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

