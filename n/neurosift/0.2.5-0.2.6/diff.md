# Comparing `tmp/neurosift-0.2.5.tar.gz` & `tmp/neurosift-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurosift-0.2.5.tar", last modified: Wed Mar  6 14:55:42 2024, max compression
+gzip compressed data, was "neurosift-0.2.6.tar", last modified: Thu Apr  4 11:43:37 2024, max compression
```

## Comparing `neurosift-0.2.5.tar` & `neurosift-0.2.6.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-06 14:55:42.026709 neurosift-0.2.5/
--rw-rw-r--   0 magland   (1000) magland   (1000)      103 2024-02-25 01:27:01.000000 neurosift-0.2.5/MANIFEST.in
--rw-r--r--   0 magland   (1000) magland   (1000)     1014 2024-03-06 14:55:42.026709 neurosift-0.2.5/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      471 2024-02-25 01:27:01.000000 neurosift-0.2.5/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-06 14:55:42.022709 neurosift-0.2.5/neurosift/
--rw-rw-r--   0 magland   (1000) magland   (1000)     1446 2023-12-22 21:08:36.000000 neurosift-0.2.5/neurosift/TemporaryDirectory.py
--rw-rw-r--   0 magland   (1000) magland   (1000)        0 2024-02-01 21:59:30.000000 neurosift-0.2.5/neurosift/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     3050 2024-03-05 14:15:17.000000 neurosift-0.2.5/neurosift/cli.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-06 14:55:42.026709 neurosift-0.2.5/neurosift/local-file-access-js/
--rw-rw-r--   0 magland   (1000) magland   (1000)      318 2024-02-25 01:27:01.000000 neurosift-0.2.5/neurosift/local-file-access-js/package.json
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-06 14:55:42.026709 neurosift-0.2.5/neurosift/local-file-access-js/src/
--rw-rw-r--   0 magland   (1000) magland   (1000)     2189 2024-03-05 14:13:19.000000 neurosift-0.2.5/neurosift/local-file-access-js/src/index.js
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-03-06 14:55:42.026709 neurosift-0.2.5/neurosift.egg-info/
--rw-r--r--   0 magland   (1000) magland   (1000)     1014 2024-03-06 14:55:41.000000 neurosift-0.2.5/neurosift.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      399 2024-03-06 14:55:42.000000 neurosift-0.2.5/neurosift.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2024-03-06 14:55:41.000000 neurosift-0.2.5/neurosift.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       54 2024-03-06 14:55:41.000000 neurosift-0.2.5/neurosift.egg-info/entry_points.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        6 2024-03-06 14:55:41.000000 neurosift-0.2.5/neurosift.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       10 2024-03-06 14:55:41.000000 neurosift-0.2.5/neurosift.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      528 2024-03-06 14:55:42.026709 neurosift-0.2.5/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      509 2024-02-25 01:27:01.000000 neurosift-0.2.5/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-04 11:43:37.990944 neurosift-0.2.6/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      103 2024-02-25 01:27:01.000000 neurosift-0.2.6/MANIFEST.in
+-rw-r--r--   0 magland   (1000) magland   (1000)     1014 2024-04-04 11:43:37.990944 neurosift-0.2.6/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)      471 2024-02-25 01:27:01.000000 neurosift-0.2.6/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-04 11:43:37.990944 neurosift-0.2.6/neurosift/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1446 2023-12-22 21:08:36.000000 neurosift-0.2.6/neurosift/TemporaryDirectory.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)        0 2024-02-01 21:59:30.000000 neurosift-0.2.6/neurosift/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3050 2024-03-05 14:15:17.000000 neurosift-0.2.6/neurosift/cli.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-04 11:43:37.990944 neurosift-0.2.6/neurosift/codecs/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2986 2024-04-04 11:21:59.000000 neurosift-0.2.6/neurosift/codecs/MP4AVCCodec.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)       51 2024-04-04 10:50:34.000000 neurosift-0.2.6/neurosift/codecs/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-04 11:43:37.990944 neurosift-0.2.6/neurosift/local-file-access-js/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      318 2024-02-25 01:27:01.000000 neurosift-0.2.6/neurosift/local-file-access-js/package.json
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-04 11:43:37.990944 neurosift-0.2.6/neurosift/local-file-access-js/src/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2189 2024-03-05 14:13:19.000000 neurosift-0.2.6/neurosift/local-file-access-js/src/index.js
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2024-04-04 11:43:37.990944 neurosift-0.2.6/neurosift.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)     1014 2024-04-04 11:43:37.000000 neurosift-0.2.6/neurosift.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)      460 2024-04-04 11:43:37.000000 neurosift-0.2.6/neurosift.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2024-04-04 11:43:37.000000 neurosift-0.2.6/neurosift.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       54 2024-04-04 11:43:37.000000 neurosift-0.2.6/neurosift.egg-info/entry_points.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        6 2024-04-04 11:43:37.000000 neurosift-0.2.6/neurosift.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       10 2024-04-04 11:43:37.000000 neurosift-0.2.6/neurosift.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      528 2024-04-04 11:43:37.990944 neurosift-0.2.6/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      509 2024-02-25 01:27:01.000000 neurosift-0.2.6/setup.py
```

### Comparing `neurosift-0.2.5/PKG-INFO` & `neurosift-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurosift
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple utility to view local NWB files using Neurosift
 Home-page: https://github.com/flatironinstitute/neurosift
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/flatironinstitute/neurosift/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neurosift-0.2.5/neurosift/TemporaryDirectory.py` & `neurosift-0.2.6/neurosift/TemporaryDirectory.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.5/neurosift/cli.py` & `neurosift-0.2.6/neurosift/cli.py`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.5/neurosift/local-file-access-js/src/index.js` & `neurosift-0.2.6/neurosift/local-file-access-js/src/index.js`

 * *Files identical despite different names*

### Comparing `neurosift-0.2.5/neurosift.egg-info/PKG-INFO` & `neurosift-0.2.6/neurosift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurosift
-Version: 0.2.5
+Version: 0.2.6
 Summary: Simple utility to view local NWB files using Neurosift
 Home-page: https://github.com/flatironinstitute/neurosift
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/flatironinstitute/neurosift/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `neurosift-0.2.5/setup.cfg` & `neurosift-0.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = neurosift
-version = 0.2.5
+version = 0.2.6
 author = Jeremy Magland
 author_email = jmagland@flatironinstitute.org
 description = Simple utility to view local NWB files using Neurosift
 url = https://github.com/flatironinstitute/neurosift
 include_package_data = True
 project_urls = 
 	Bug Tracker = https://github.com/flatironinstitute/neurosift/issues
```

