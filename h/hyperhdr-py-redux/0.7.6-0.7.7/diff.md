# Comparing `tmp/hyperhdr_py_redux-0.7.6.tar.gz` & `tmp/hyperhdr_py_redux-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperhdr_py_redux-0.7.6.tar", max compression
+gzip compressed data, was "hyperhdr_py_redux-0.7.7.tar", max compression
```

## Comparing `hyperhdr_py_redux-0.7.6.tar` & `hyperhdr_py_redux-0.7.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-04-04 03:37:51.660652 hyperhdr_py_redux-0.7.6/LICENSE
--rw-r--r--   0        0        0    19564 2024-04-04 03:37:51.660652 hyperhdr_py_redux-0.7.6/README.md
--rw-r--r--   0        0        0       31 2024-04-04 03:37:51.660652 hyperhdr_py_redux-0.7.6/hyperion/__init__.py
--rw-r--r--   0        0        0    64491 2024-04-04 03:37:51.661652 hyperhdr_py_redux-0.7.6/hyperion/client.py
--rwxr-xr-x   0        0        0     3682 2024-04-04 03:37:51.661652 hyperhdr_py_redux-0.7.6/hyperion/const.py
--rw-r--r--   0        0        0        0 2024-04-04 03:37:51.661652 hyperhdr_py_redux-0.7.6/hyperion/py.typed
--rw-r--r--   0        0        0     1582 2024-04-04 08:40:39.701153 hyperhdr_py_redux-0.7.6/pyproject.toml
--rw-r--r--   0        0        0    20442 1970-01-01 00:00:00.000000 hyperhdr_py_redux-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/LICENSE
+-rw-r--r--   0        0        0    19564 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/README.md
+-rw-r--r--   0        0        0       31 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/hyperion/__init__.py
+-rw-r--r--   0        0        0    64491 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/hyperion/client.py
+-rwxr-xr-x   0        0        0     3663 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/hyperion/const.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/hyperion/py.typed
+-rw-r--r--   0        0        0     1582 2024-04-04 09:18:39.940957 hyperhdr_py_redux-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0    20442 1970-01-01 00:00:00.000000 hyperhdr_py_redux-0.7.7/PKG-INFO
```

### Comparing `hyperhdr_py_redux-0.7.6/LICENSE` & `hyperhdr_py_redux-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperhdr_py_redux-0.7.6/README.md` & `hyperhdr_py_redux-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `hyperhdr_py_redux-0.7.6/hyperion/client.py` & `hyperhdr_py_redux-0.7.7/hyperion/client.py`

 * *Files identical despite different names*

### Comparing `hyperhdr_py_redux-0.7.6/hyperion/const.py` & `hyperhdr_py_redux-0.7.7/hyperion/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 KEY_COMPONENTID_SMOOTHING = "SMOOTHING"
 KEY_COMPONENTID_BLACKBORDER = "BLACKBORDER"
 KEY_COMPONENTID_FORWARDER = "FORWARDER"
 KEY_COMPONENTID_BOBLIGHTSERVER = "BOBLIGHTSERVER"
 KEY_COMPONENTID_SYSTEMGRABBER = "SYSTEMGRABBER"
 KEY_COMPONENTID_LEDDEVICE = "LEDDEVICE"
 KEY_COMPONENTID_VIDEOGRABBER = "VIDEOGRABBER"
-KEY_COMPONENTID_V4L = "V4L"
 
 KEY_COMPONENTID_EXTERNAL_SOURCES = [
     KEY_COMPONENTID_BOBLIGHTSERVER,
     KEY_COMPONENTID_SYSTEMGRABBER,
     KEY_COMPONENTID_VIDEOGRABBER,
 ]
 
@@ -104,15 +103,15 @@
     KEY_COMPONENTID_ALL: "All",
     KEY_COMPONENTID_SMOOTHING: "Smoothing",
     KEY_COMPONENTID_BLACKBORDER: "Blackbar Detection",
     KEY_COMPONENTID_FORWARDER: "Forwarder",
     KEY_COMPONENTID_BOBLIGHTSERVER: "Boblight Server",
     KEY_COMPONENTID_SYSTEMGRABBER: "Platform Capture",
     KEY_COMPONENTID_LEDDEVICE: "LED Device",
-    KEY_COMPONENTID_V4L: "USB Capture",
+    KEY_COMPONENTID_VIDEOGRABBER: "USB Capture",
 }
 KEY_COMPONENTID_FROM_NAME = {
     name: component for component, name in KEY_COMPONENTID_TO_NAME.items()
 }
 
 DEFAULT_INSTANCE = 0
 DEFAULT_CONNECTION_RETRY_DELAY_SECS = 30
```

### Comparing `hyperhdr_py_redux-0.7.6/pyproject.toml` & `hyperhdr_py_redux-0.7.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperhdr-py-redux"
-version = "0.7.6"
+version = "0.7.7"
 description = "Hyperion Ambient Lighting Python Package"
 authors = ["Andrew Kennedy <andrewk36@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hyperhdr_py_redux-0.7.6/PKG-INFO` & `hyperhdr_py_redux-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperhdr-py-redux
-Version: 0.7.6
+Version: 0.7.7
 Summary: Hyperion Ambient Lighting Python Package
 Home-page: https://github.com/andrew-kennedy/hyperion-py
 License: MIT
 Keywords: hyperion
 Author: Andrew Kennedy
 Author-email: andrewk36@gmail.com
 Requires-Python: >=3.8,<4.0
```

