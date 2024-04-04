# Comparing `tmp/vonage-utils-1.0.0.tar.gz` & `tmp/vonage-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-utils-1.0.0.tar", last modified: Thu Feb 22 04:12:53 2024, max compression
+gzip compressed data, was "vonage-utils-1.0.1.tar", last modified: Thu Apr  4 05:14:01 2024, max compression
```

## Comparing `vonage-utils-1.0.0.tar` & `vonage-utils-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-02-22 04:12:53.385923 vonage-utils-1.0.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     1677 2024-02-22 04:12:53.384755 vonage-utils-1.0.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      974 2024-02-22 04:12:52.000000 vonage-utils-1.0.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-02-22 04:12:52.000000 vonage-utils-1.0.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      771 2024-02-22 04:12:52.000000 vonage-utils-1.0.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-02-22 04:12:53.385985 vonage-utils-1.0.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-02-22 04:12:53.376738 vonage-utils-1.0.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-02-22 04:12:53.380164 vonage-utils-1.0.0/src/vonage_utils/
--rw-r--r--   0 mkahan     (503) staff       (20)      163 2024-02-22 04:12:52.000000 vonage-utils-1.0.0/src/vonage_utils/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      325 2024-02-22 04:12:52.000000 vonage-utils-1.0.0/src/vonage_utils/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-02-22 04:12:52.000000 vonage-utils-1.0.0/src/vonage_utils/utils.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-02-22 04:12:53.384000 vonage-utils-1.0.0/src/vonage_utils.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     1677 2024-02-22 04:12:53.000000 vonage-utils-1.0.0/src/vonage_utils.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      282 2024-02-22 04:12:53.000000 vonage-utils-1.0.0/src/vonage_utils.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-02-22 04:12:53.000000 vonage-utils-1.0.0/src/vonage_utils.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-02-22 04:12:53.000000 vonage-utils-1.0.0/src/vonage_utils.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.670259 vonage-utils-1.0.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1708 2024-04-04 05:14:01.668280 vonage-utils-1.0.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      974 2024-04-04 05:14:00.000000 vonage-utils-1.0.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-04 05:14:00.000000 vonage-utils-1.0.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      806 2024-04-04 05:14:00.000000 vonage-utils-1.0.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-04 05:14:01.670347 vonage-utils-1.0.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.633454 vonage-utils-1.0.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.646075 vonage-utils-1.0.1/src/vonage_utils/
+-rw-r--r--   0 mkahan     (503) staff       (20)      221 2024-04-04 05:14:00.000000 vonage-utils-1.0.1/src/vonage_utils/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      325 2024-04-04 05:14:00.000000 vonage-utils-1.0.1/src/vonage_utils/errors.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.660478 vonage-utils-1.0.1/src/vonage_utils/types/
+-rw-r--r--   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:00.000000 vonage-utils-1.0.1/src/vonage_utils/types/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      132 2024-04-04 05:14:00.000000 vonage-utils-1.0.1/src/vonage_utils/types/phone_number.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-04 05:14:00.000000 vonage-utils-1.0.1/src/vonage_utils/utils.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.665501 vonage-utils-1.0.1/src/vonage_utils.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1708 2024-04-04 05:14:01.000000 vonage-utils-1.0.1/src/vonage_utils.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      395 2024-04-04 05:14:01.000000 vonage-utils-1.0.1/src/vonage_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-04 05:14:01.000000 vonage-utils-1.0.1/src/vonage_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       16 2024-04-04 05:14:01.000000 vonage-utils-1.0.1/src/vonage_utils.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-04 05:14:01.000000 vonage-utils-1.0.1/src/vonage_utils.egg-info/top_level.txt
```

### Comparing `vonage-utils-1.0.0/PKG-INFO` & `vonage-utils-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: vonage-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utils package containing objects for use with Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
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
+Requires-Dist: pydantic>=2.6.1
 
 # Vonage Utils Package
 
 This package contains utility code that is used by the Vonage Python SDK and other related packages.
 
 The utils module provides two utility functions: `format_phone_number` and `remove_none_values`. It also exposes the `VonageError` type that other exceptions related to Vonage SDK inherit from. This can also be accessed via the main SDK module with `vonage.VonageError`.
```

### Comparing `vonage-utils-1.0.0/README.md` & `vonage-utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vonage-utils-1.0.0/backend_shim.py` & `vonage-utils-1.0.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-utils-1.0.0/pyproject.toml` & `vonage-utils-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name = 'vonage-utils'
-version = '1.0.0'
+version = '1.0.1'
 description = 'Utils package containing objects for use with Vonage APIs'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
+dependencies = ["pydantic>=2.6.1"]
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `vonage-utils-1.0.0/src/vonage_utils/utils.py` & `vonage-utils-1.0.1/src/vonage_utils/utils.py`

 * *Files identical despite different names*

### Comparing `vonage-utils-1.0.0/src/vonage_utils.egg-info/PKG-INFO` & `vonage-utils-1.0.1/src/vonage_utils.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: vonage-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utils package containing objects for use with Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
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
+Requires-Dist: pydantic>=2.6.1
 
 # Vonage Utils Package
 
 This package contains utility code that is used by the Vonage Python SDK and other related packages.
 
 The utils module provides two utility functions: `format_phone_number` and `remove_none_values`. It also exposes the `VonageError` type that other exceptions related to Vonage SDK inherit from. This can also be accessed via the main SDK module with `vonage.VonageError`.
```

