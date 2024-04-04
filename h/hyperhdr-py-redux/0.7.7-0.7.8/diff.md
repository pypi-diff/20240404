# Comparing `tmp/hyperhdr_py_redux-0.7.7.tar.gz` & `tmp/hyperhdr_py_redux-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperhdr_py_redux-0.7.7.tar", max compression
+gzip compressed data, was "hyperhdr_py_redux-0.7.8.tar", max compression
```

## Comparing `hyperhdr_py_redux-0.7.7.tar` & `hyperhdr_py_redux-0.7.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/LICENSE
--rw-r--r--   0        0        0    19564 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/README.md
--rw-r--r--   0        0        0       31 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/hyperion/__init__.py
--rw-r--r--   0        0        0    64491 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/hyperion/client.py
--rwxr-xr-x   0        0        0     3663 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/hyperion/const.py
--rw-r--r--   0        0        0        0 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.7/hyperion/py.typed
--rw-r--r--   0        0        0     1582 2024-04-04 09:18:39.940957 hyperhdr_py_redux-0.7.7/pyproject.toml
--rw-r--r--   0        0        0    20442 1970-01-01 00:00:00.000000 hyperhdr_py_redux-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.8/LICENSE
+-rw-r--r--   0        0        0    19564 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.8/README.md
+-rw-r--r--   0        0        0       31 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.8/hyperion/__init__.py
+-rw-r--r--   0        0        0    64491 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.8/hyperion/client.py
+-rwxr-xr-x   0        0        0     3736 2024-04-04 10:04:08.145722 hyperhdr_py_redux-0.7.8/hyperion/const.py
+-rw-r--r--   0        0        0        0 2024-04-04 09:18:39.939957 hyperhdr_py_redux-0.7.8/hyperion/py.typed
+-rw-r--r--   0        0        0     1582 2024-04-04 10:04:08.145722 hyperhdr_py_redux-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0    20442 1970-01-01 00:00:00.000000 hyperhdr_py_redux-0.7.8/PKG-INFO
```

### Comparing `hyperhdr_py_redux-0.7.7/LICENSE` & `hyperhdr_py_redux-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperhdr_py_redux-0.7.7/README.md` & `hyperhdr_py_redux-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `hyperhdr_py_redux-0.7.7/hyperion/client.py` & `hyperhdr_py_redux-0.7.8/hyperion/client.py`

 * *Files identical despite different names*

### Comparing `hyperhdr_py_redux-0.7.7/hyperion/const.py` & `hyperhdr_py_redux-0.7.8/hyperion/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 KEY_COMPONENTID_SMOOTHING = "SMOOTHING"
 KEY_COMPONENTID_BLACKBORDER = "BLACKBORDER"
 KEY_COMPONENTID_FORWARDER = "FORWARDER"
 KEY_COMPONENTID_BOBLIGHTSERVER = "BOBLIGHTSERVER"
 KEY_COMPONENTID_SYSTEMGRABBER = "SYSTEMGRABBER"
 KEY_COMPONENTID_LEDDEVICE = "LEDDEVICE"
 KEY_COMPONENTID_VIDEOGRABBER = "VIDEOGRABBER"
+KEY_COMPONENTID_HDR = "HDR"
 
 KEY_COMPONENTID_EXTERNAL_SOURCES = [
     KEY_COMPONENTID_BOBLIGHTSERVER,
     KEY_COMPONENTID_SYSTEMGRABBER,
     KEY_COMPONENTID_VIDEOGRABBER,
 ]
 
@@ -104,14 +105,15 @@
     KEY_COMPONENTID_SMOOTHING: "Smoothing",
     KEY_COMPONENTID_BLACKBORDER: "Blackbar Detection",
     KEY_COMPONENTID_FORWARDER: "Forwarder",
     KEY_COMPONENTID_BOBLIGHTSERVER: "Boblight Server",
     KEY_COMPONENTID_SYSTEMGRABBER: "Platform Capture",
     KEY_COMPONENTID_LEDDEVICE: "LED Device",
     KEY_COMPONENTID_VIDEOGRABBER: "USB Capture",
+    KEY_COMPONENTID_HDR: "HDR Tone Mapping",
 }
 KEY_COMPONENTID_FROM_NAME = {
     name: component for component, name in KEY_COMPONENTID_TO_NAME.items()
 }
 
 DEFAULT_INSTANCE = 0
 DEFAULT_CONNECTION_RETRY_DELAY_SECS = 30
```

### Comparing `hyperhdr_py_redux-0.7.7/pyproject.toml` & `hyperhdr_py_redux-0.7.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperhdr-py-redux"
-version = "0.7.7"
+version = "0.7.8"
 description = "Hyperion Ambient Lighting Python Package"
 authors = ["Andrew Kennedy <andrewk36@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hyperhdr_py_redux-0.7.7/PKG-INFO` & `hyperhdr_py_redux-0.7.8/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperhdr-py-redux
-Version: 0.7.7
+Version: 0.7.8
 Summary: Hyperion Ambient Lighting Python Package
 Home-page: https://github.com/andrew-kennedy/hyperion-py
 License: MIT
 Keywords: hyperion
 Author: Andrew Kennedy
 Author-email: andrewk36@gmail.com
 Requires-Python: >=3.8,<4.0
```

