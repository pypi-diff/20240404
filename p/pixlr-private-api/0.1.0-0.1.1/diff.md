# Comparing `tmp/pixlr_private_api-0.1.0.tar.gz` & `tmp/pixlr_private_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixlr_private_api-0.1.0.tar", last modified: Mon Apr  1 08:55:40 2024, max compression
+gzip compressed data, was "pixlr_private_api-0.1.1.tar", last modified: Thu Apr  4 03:03:52 2024, max compression
```

## Comparing `pixlr_private_api-0.1.0.tar` & `pixlr_private_api-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-01 08:55:40.382591 pixlr_private_api-0.1.0/
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     1069 2024-04-01 06:31:04.000000 pixlr_private_api-0.1.0/LICENCE.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     4954 2024-04-01 08:55:40.382591 pixlr_private_api-0.1.0/PKG-INFO
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     3921 2024-04-01 08:53:23.000000 pixlr_private_api-0.1.0/README.md
-drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-01 08:55:40.380591 pixlr_private_api-0.1.0/pixlr_private_api/
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-01 06:31:04.000000 pixlr_private_api-0.1.0/pixlr_private_api/__init__.py
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)    18763 2024-04-01 08:50:37.000000 pixlr_private_api-0.1.0/pixlr_private_api/main.py
-drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-01 08:55:40.381591 pixlr_private_api-0.1.0/pixlr_private_api.egg-info/
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     4954 2024-04-01 08:55:40.000000 pixlr_private_api-0.1.0/pixlr_private_api.egg-info/PKG-INFO
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)      290 2024-04-01 08:55:40.000000 pixlr_private_api-0.1.0/pixlr_private_api.egg-info/SOURCES.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)        1 2024-04-01 08:55:40.000000 pixlr_private_api-0.1.0/pixlr_private_api.egg-info/dependency_links.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       27 2024-04-01 08:55:40.000000 pixlr_private_api-0.1.0/pixlr_private_api.egg-info/requires.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       18 2024-04-01 08:55:40.000000 pixlr_private_api-0.1.0/pixlr_private_api.egg-info/top_level.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       38 2024-04-01 08:55:40.382591 pixlr_private_api-0.1.0/setup.cfg
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     1239 2024-04-01 08:55:34.000000 pixlr_private_api-0.1.0/setup.py
+drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:03:52.405807 pixlr_private_api-0.1.1/
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     1069 2024-04-01 06:31:04.000000 pixlr_private_api-0.1.1/LICENCE.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     4954 2024-04-04 03:03:52.405807 pixlr_private_api-0.1.1/PKG-INFO
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     3921 2024-04-01 08:53:23.000000 pixlr_private_api-0.1.1/README.md
+drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:03:52.403807 pixlr_private_api-0.1.1/pixlr_private_api/
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-01 06:31:04.000000 pixlr_private_api-0.1.1/pixlr_private_api/__init__.py
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)    18763 2024-04-01 08:50:37.000000 pixlr_private_api-0.1.1/pixlr_private_api/main.py
+drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:03:52.405807 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     4954 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/PKG-INFO
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)      290 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/SOURCES.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)        1 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/dependency_links.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       27 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/requires.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       18 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/top_level.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       38 2024-04-04 03:03:52.405807 pixlr_private_api-0.1.1/setup.cfg
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     1184 2024-04-04 03:03:31.000000 pixlr_private_api-0.1.1/setup.py
```

### Comparing `pixlr_private_api-0.1.0/LICENCE.txt` & `pixlr_private_api-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pixlr_private_api-0.1.0/PKG-INFO` & `pixlr_private_api-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixlr_private_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Package to Generate Images with http://pixlr.com programmatically.
 Home-page: https://github.com/Automa-Automations/pixlr-private-api
 Author: Simon Ferns
 Author-email: business@simonferns.com
 License: MIT
 Keywords: temp-email automation email
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pixlr_private_api-0.1.0/README.md` & `pixlr_private_api-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pixlr_private_api-0.1.0/pixlr_private_api/main.py` & `pixlr_private_api-0.1.1/pixlr_private_api/main.py`

 * *Files identical despite different names*

### Comparing `pixlr_private_api-0.1.0/pixlr_private_api.egg-info/PKG-INFO` & `pixlr_private_api-0.1.1/pixlr_private_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixlr_private_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Package to Generate Images with http://pixlr.com programmatically.
 Home-page: https://github.com/Automa-Automations/pixlr-private-api
 Author: Simon Ferns
 Author-email: business@simonferns.com
 License: MIT
 Keywords: temp-email automation email
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pixlr_private_api-0.1.0/setup.py` & `pixlr_private_api-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pixlr_private_api",
-    version=".".join([i.strip() for i in open("version.txt").readlines()]),
+    version="0.1.1",
     description="A Python Package to Generate Images with http://pixlr.com programmatically.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Automa-Automations/pixlr-private-api",
     author="Simon Ferns",
     author_email="business@simonferns.com",
     license="MIT",
```

