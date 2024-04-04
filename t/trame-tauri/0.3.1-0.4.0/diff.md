# Comparing `tmp/trame-tauri-0.3.1.tar.gz` & `tmp/trame-tauri-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-tauri-0.3.1.tar", last modified: Fri Mar 22 22:19:57 2024, max compression
+gzip compressed data, was "trame-tauri-0.4.0.tar", last modified: Thu Apr  4 20:06:07 2024, max compression
```

## Comparing `trame-tauri-0.3.1.tar` & `trame-tauri-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/
--rw-r--r--   0 root         (0) root         (0)      583 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2518 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1736 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      925 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame/modules/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame/widgets/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/trame_tauri/
--rw-r--r--   0 root         (0) root         (0)       93 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame_tauri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/trame_tauri/module/
--rw-r--r--   0 root         (0) root         (0)      199 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame_tauri/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/trame_tauri/module/serve/
--rw-r--r--   0 root         (0) root         (0)     5914 2024-03-22 22:19:53.000000 trame-tauri-0.3.1/trame_tauri/module/serve/trame-tauri.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/trame_tauri/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame_tauri/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4411 2024-03-22 22:19:34.000000 trame-tauri-0.3.1/trame_tauri/widgets/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 22:19:57.184317 trame-tauri-0.3.1/trame_tauri.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2518 2024-03-22 22:19:57.000000 trame-tauri-0.3.1/trame_tauri.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-03-22 22:19:57.000000 trame-tauri-0.3.1/trame_tauri.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 22:19:57.000000 trame-tauri-0.3.1/trame_tauri.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-03-22 22:19:57.000000 trame-tauri-0.3.1/trame_tauri.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-22 22:19:57.000000 trame-tauri-0.3.1/trame_tauri.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      925 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/modules/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/widgets/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri/
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame_tauri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri/module/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame_tauri/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri/module/serve/
+-rw-r--r--   0 root         (0) root         (0)    32933 2024-04-04 20:06:02.000000 trame-tauri-0.4.0/trame_tauri/module/serve/trame-tauri.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame_tauri/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame_tauri/widgets/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/top_level.txt
```

### Comparing `trame-tauri-0.3.1/LICENSE` & `trame-tauri-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.3.1/PKG-INFO` & `trame-tauri-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-tauri
-Version: 0.3.1
+Version: 0.4.0
 Summary: Helper widget to provide simpler integration with Tauri
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-tauri-0.3.1/README.rst` & `trame-tauri-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.3.1/setup.cfg` & `trame-tauri-0.4.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-tauri
-version = 0.3.1
+version = 0.4.0
 description = Helper widget to provide simpler integration with Tauri
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-tauri-0.3.1/trame_tauri/widgets/tauri.py` & `trame-tauri-0.4.0/trame_tauri/widgets/tauri.py`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.3.1/trame_tauri.egg-info/PKG-INFO` & `trame-tauri-0.4.0/trame_tauri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-tauri
-Version: 0.3.1
+Version: 0.4.0
 Summary: Helper widget to provide simpler integration with Tauri
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

