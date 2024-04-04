# Comparing `tmp/vonage-3.99.0a3.tar.gz` & `tmp/vonage-3.99.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-3.99.0a3.tar", last modified: Thu Mar 28 03:44:58 2024, max compression
+gzip compressed data, was "vonage-3.99.0a4.tar", last modified: Thu Apr  4 05:14:01 2024, max compression
```

## Comparing `vonage-3.99.0a3.tar` & `vonage-3.99.0a4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:44:58.312339 vonage-3.99.0a3/
--rw-r--r--   0 mkahan     (503) staff       (20)     2302 2024-03-28 03:44:58.311707 vonage-3.99.0a3/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     1429 2024-03-28 03:44:57.000000 vonage-3.99.0a3/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-03-28 03:44:57.000000 vonage-3.99.0a3/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      989 2024-03-28 03:44:57.000000 vonage-3.99.0a3/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-03-28 03:44:58.312384 vonage-3.99.0a3/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:44:58.305770 vonage-3.99.0a3/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:44:58.308339 vonage-3.99.0a3/src/vonage/
--rw-r--r--   0 mkahan     (503) staff       (20)      251 2024-03-28 03:44:57.000000 vonage-3.99.0a3/src/vonage/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-03-28 03:44:57.000000 vonage-3.99.0a3/src/vonage/_version.py
--rw-r--r--   0 mkahan     (503) staff       (20)      987 2024-03-28 03:44:57.000000 vonage-3.99.0a3/src/vonage/vonage.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:44:58.311149 vonage-3.99.0a3/src/vonage.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2302 2024-03-28 03:44:58.000000 vonage-3.99.0a3/src/vonage.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      276 2024-03-28 03:44:58.000000 vonage-3.99.0a3/src/vonage.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-03-28 03:44:58.000000 vonage-3.99.0a3/src/vonage.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      116 2024-03-28 03:44:58.000000 vonage-3.99.0a3/src/vonage.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        7 2024-03-28 03:44:58.000000 vonage-3.99.0a3/src/vonage.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.769268 vonage-3.99.0a4/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2338 2024-04-04 05:14:01.767833 vonage-3.99.0a4/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     1429 2024-04-04 05:14:00.000000 vonage-3.99.0a4/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-04 05:14:00.000000 vonage-3.99.0a4/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1015 2024-04-04 05:14:00.000000 vonage-3.99.0a4/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-04 05:14:01.769490 vonage-3.99.0a4/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.743387 vonage-3.99.0a4/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.756206 vonage-3.99.0a4/src/vonage/
+-rw-r--r--   0 mkahan     (503) staff       (20)      273 2024-04-04 05:14:00.000000 vonage-3.99.0a4/src/vonage/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-04-04 05:14:00.000000 vonage-3.99.0a4/src/vonage/_version.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1359 2024-04-04 05:14:00.000000 vonage-3.99.0a4/src/vonage/vonage.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.766298 vonage-3.99.0a4/src/vonage.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2338 2024-04-04 05:14:01.000000 vonage-3.99.0a4/src/vonage.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      276 2024-04-04 05:14:01.000000 vonage-3.99.0a4/src/vonage.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-04 05:14:01.000000 vonage-3.99.0a4/src/vonage.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      137 2024-04-04 05:14:01.000000 vonage-3.99.0a4/src/vonage.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        7 2024-04-04 05:14:01.000000 vonage-3.99.0a4/src/vonage.egg-info/top_level.txt
```

### Comparing `vonage-3.99.0a3/PKG-INFO` & `vonage-3.99.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: vonage
-Version: 3.99.0a3
+Version: 3.99.0a4
 Summary: Python Server SDK for using Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-utils>=1.0.0
-Requires-Dist: vonage-http-client>=1.1.1
+Requires-Dist: vonage-utils>=1.0.1
+Requires-Dist: vonage-http-client>=1.2.0
 Requires-Dist: vonage-number-insight-v2>=0.1.0
 Requires-Dist: vonage-sms>=1.0.2
-Requires-Dist: vonage-users>=1.0.0
+Requires-Dist: vonage-users>=1.0.1
+Requires-Dist: vonage-verify>=1.0.0
 
 # Vonage Python SDK
 
 The Vonage Python SDK Package `vonage` provides a streamlined interface for using Vonage APIs in Python projects. This package includes the `Vonage` class, which simplifies API interactions.
 
 The Vonage class in this package serves as the main entry point for using Vonage APIs. It abstracts away complexities with authentication, HTTP requests and more.
```

### Comparing `vonage-3.99.0a3/README.md` & `vonage-3.99.0a4/README.md`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a3/backend_shim.py` & `vonage-3.99.0a4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a3/pyproject.toml` & `vonage-3.99.0a4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 name = "vonage"
 dynamic = ["version"]
 description = "Python Server SDK for using Vonage APIs"
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-utils>=1.0.0",
-  "vonage-http-client>=1.1.1",
+  "vonage-utils>=1.0.1",
+  "vonage-http-client>=1.2.0",
   "vonage-number-insight-v2>=0.1.0",
   "vonage-sms>=1.0.2",
-  "vonage-users>=1.0.0",
+  "vonage-users>=1.0.1",
+  "vonage-verify>=1.0.0",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `vonage-3.99.0a3/src/vonage.egg-info/PKG-INFO` & `vonage-3.99.0a4/src/vonage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: vonage
-Version: 3.99.0a3
+Version: 3.99.0a4
 Summary: Python Server SDK for using Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-utils>=1.0.0
-Requires-Dist: vonage-http-client>=1.1.1
+Requires-Dist: vonage-utils>=1.0.1
+Requires-Dist: vonage-http-client>=1.2.0
 Requires-Dist: vonage-number-insight-v2>=0.1.0
 Requires-Dist: vonage-sms>=1.0.2
-Requires-Dist: vonage-users>=1.0.0
+Requires-Dist: vonage-users>=1.0.1
+Requires-Dist: vonage-verify>=1.0.0
 
 # Vonage Python SDK
 
 The Vonage Python SDK Package `vonage` provides a streamlined interface for using Vonage APIs in Python projects. This package includes the `Vonage` class, which simplifies API interactions.
 
 The Vonage class in this package serves as the main entry point for using Vonage APIs. It abstracts away complexities with authentication, HTTP requests and more.
```

