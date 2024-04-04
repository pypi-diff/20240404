# Comparing `tmp/yamlscript-0.1.5.tar.gz` & `tmp/yamlscript-0.1.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlscript-0.1.5.tar", last modified: Tue Jan  2 17:27:29 2024, max compression
+gzip compressed data, was "yamlscript-0.1.50.tar", last modified: Thu Apr  4 15:18:37 2024, max compression
```

## Comparing `yamlscript-0.1.5.tar` & `yamlscript-0.1.50.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-01-02 17:27:29.660160 yamlscript-0.1.5/
--rw-r--r--   0 ingy      (1000) ingy      (1000)        0 2024-01-02 17:26:17.000000 yamlscript-0.1.5/.long_description.md
--rw-r--r--   0 ingy      (1000) ingy      (1000)       47 2024-01-02 17:26:17.000000 yamlscript-0.1.5/MANIFEST.in
--rw-r--r--   0 ingy      (1000) ingy      (1000)      756 2024-01-02 17:27:29.660160 yamlscript-0.1.5/PKG-INFO
--rw-r--r--   0 ingy      (1000) ingy      (1000)     1638 2023-12-29 15:51:05.000000 yamlscript-0.1.5/ReadMe.md
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-01-02 17:27:29.660160 yamlscript-0.1.5/lib/
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-01-02 17:27:29.660160 yamlscript-0.1.5/lib/yamlscript/
--rw-r--r--   0 ingy      (1000) ingy      (1000)     4057 2024-01-02 17:10:23.000000 yamlscript-0.1.5/lib/yamlscript/__init__.py
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-01-02 17:27:29.660160 yamlscript-0.1.5/lib/yamlscript.egg-info/
--rw-r--r--   0 ingy      (1000) ingy      (1000)      756 2024-01-02 17:27:29.000000 yamlscript-0.1.5/lib/yamlscript.egg-info/PKG-INFO
--rw-r--r--   0 ingy      (1000) ingy      (1000)      290 2024-01-02 17:27:29.000000 yamlscript-0.1.5/lib/yamlscript.egg-info/SOURCES.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)        1 2024-01-02 17:27:29.000000 yamlscript-0.1.5/lib/yamlscript.egg-info/dependency_links.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)        7 2024-01-02 17:27:29.000000 yamlscript-0.1.5/lib/yamlscript.egg-info/requires.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)       11 2024-01-02 17:27:29.000000 yamlscript-0.1.5/lib/yamlscript.egg-info/top_level.txt
--rw-r--r--   0 ingy      (1000) ingy      (1000)       79 2024-01-02 17:27:29.664160 yamlscript-0.1.5/setup.cfg
--rw-r--r--   0 ingy      (1000) ingy      (1000)     1145 2024-01-02 17:23:23.000000 yamlscript-0.1.5/setup.py
-drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-01-02 17:27:29.660160 yamlscript-0.1.5/test/
--rw-r--r--   0 ingy      (1000) ingy      (1000)      144 2023-12-29 15:51:05.000000 yamlscript-0.1.5/test/test.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-04 15:18:37.573656 yamlscript-0.1.50/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        0 2024-04-04 15:18:37.000000 yamlscript-0.1.50/.long_description.md
+-rw-r--r--   0 ingy      (1000) ingy      (1000)       47 2024-04-04 15:18:37.000000 yamlscript-0.1.50/MANIFEST.in
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-04 15:18:37.573656 yamlscript-0.1.50/PKG-INFO
+-rw-rw-r--   0 ingy      (1000) ingy      (1000)     3079 2024-03-28 18:44:00.000000 yamlscript-0.1.50/ReadMe.md
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-04 15:18:37.573656 yamlscript-0.1.50/lib/
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-04 15:18:37.573656 yamlscript-0.1.50/lib/yamlscript/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)     4362 2024-04-04 15:12:21.000000 yamlscript-0.1.50/lib/yamlscript/__init__.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-04 15:18:37.573656 yamlscript-0.1.50/lib/yamlscript.egg-info/
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      757 2024-04-04 15:18:37.000000 yamlscript-0.1.50/lib/yamlscript.egg-info/PKG-INFO
+-rw-r--r--   0 ingy      (1000) ingy      (1000)      290 2024-04-04 15:18:37.000000 yamlscript-0.1.50/lib/yamlscript.egg-info/SOURCES.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        1 2024-04-04 15:18:37.000000 yamlscript-0.1.50/lib/yamlscript.egg-info/dependency_links.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)        7 2024-04-04 15:18:37.000000 yamlscript-0.1.50/lib/yamlscript.egg-info/requires.txt
+-rw-r--r--   0 ingy      (1000) ingy      (1000)       11 2024-04-04 15:18:37.000000 yamlscript-0.1.50/lib/yamlscript.egg-info/top_level.txt
+-rw-rw-r--   0 ingy      (1000) ingy      (1000)       79 2024-04-04 15:18:37.573656 yamlscript-0.1.50/setup.cfg
+-rw-r--r--   0 ingy      (1000) ingy      (1000)     1146 2024-04-04 15:12:21.000000 yamlscript-0.1.50/setup.py
+drwxr-xr-x   0 ingy      (1000) ingy      (1000)        0 2024-04-04 15:18:37.573656 yamlscript-0.1.50/test/
+-rw-rw-r--   0 ingy      (1000) ingy      (1000)      144 2024-03-28 18:44:00.000000 yamlscript-0.1.50/test/test.py
```

### Comparing `yamlscript-0.1.5/PKG-INFO` & `yamlscript-0.1.50/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlscript
-Version: 0.1.5
+Version: 0.1.50
 Summary: Program in YAML
 Home-page: https://github.com/ingydotnet/yamlscript
 Author: Ingy döt Net
 Author-email: ingy@ingy.net
 License: MIT
 Keywords: yaml,language
 Platform: UNKNOWN
```

### Comparing `yamlscript-0.1.5/lib/yamlscript/__init__.py` & `yamlscript-0.1.50/lib/yamlscript/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 The load() method takes a YAMLScript string as input and returns the Python
 object that the YAMLScript code evaluates to.
 """
 
 # This value is automatically updated by 'make bump'.
 # The version number is used to find the correct shared library file.
 # We currently only support binding to an exact version of libyamlscript.
-yamlscript_version = '0.1.34'
+yamlscript_version = '0.1.50'
 
 import os, sys
 import ctypes
 import json
 
 # Require Python 3.6 or greater:
 assert sys.version_info >= (3, 6), \
@@ -45,25 +45,30 @@
     "libyamlscript.%s.%s" % (so, yamlscript_version)
 
   # Use LD_LIBRARY_PATH to find libyamlscript shared library, or default to
   # '/usr/local/lib' (where it is installed by default):
   ld_library_path = os.environ.get('LD_LIBRARY_PATH')
   ld_library_paths = ld_library_path.split(':') if ld_library_path else []
   ld_library_paths.append('/usr/local/lib')
+  ld_library_paths.append(os.environ.get('HOME') + '/.local/lib')
 
   libyamlscript_path = None
   for path in ld_library_paths:
     path = path + '/' + libyamlscript_name
     if os.path.isfile(path):
       libyamlscript_path = path
       break
 
   if not libyamlscript_path:
     raise Exception(
-      "Shared library file '%s' not found." % libyamlscript_name)
+      """\
+Shared library file '%s' not found
+Try: curl -sSL yamlscript.org/install | VERSION=%s LIB=1 bash
+See: https://github.com/yaml/yamlscript/wiki/Installing-YAMLScript
+""" % (libyamlscript_name, yamlscript_version))
 
   return libyamlscript_path
 
 # Load libyamlscript shared library:
 libyamlscript = ctypes.CDLL(find_libyamlscript_path())
 
 # Create binding to 'load_ys_to_json' function:
@@ -74,57 +79,62 @@
 # The YAMLScript class is the main user facing API for this module.
 class YAMLScript():
   """
   Interface with the libyamlscript shared library.
 
   Usage:
     import yamlscript
-    ys = YAMLScript()
+    ys = yamlscript.YAMLScript()
     data = ys.load(open('file.ys').read())
   """
 
   # YAMLScript instance constructor:
   def __init__(self, config={}):
     # config not used yet
-    self.config = config
-    # Create a new GraalVM isolate for life of the YAMLScript instance:
-    self.isolate = ctypes.c_void_p()
+    # self.config = config
+
+    # Create a new GraalVM isolatethread for life of the YAMLScript instance:
+    self.isolatethread = ctypes.c_void_p()
+
+    # Create a new GraalVM isolate:
+    rc = libyamlscript.graal_create_isolate(
+      None,
+      None,
+      ctypes.byref(self.isolatethread),
+    )
+
+    if rc != 0:
+      raise Exception("Failed to create isolate")
 
   # Compile and eval a YAMLScript string and return the result:
   def load(self, input):
     # Reset any previous error:
     self.error = None
 
-    # Create a new GraalVM isolate thread for each call to load():
-    isolatethread = ctypes.c_void_p()
-    libyamlscript.graal_create_isolate(
-      None,
-      ctypes.byref(self.isolate),
-      ctypes.byref(isolatethread),
-    )
-
     # Call 'load_ys_to_json' function in libyamlscript shared library:
     data_json = load_ys_to_json(
-      isolatethread,
+      self.isolatethread,
       ctypes.c_char_p(bytes(input, "utf8")),
     ).decode()
 
     # Decode the JSON response:
     resp = json.loads(data_json)
 
-    # Tear down the isolate thread to free resources:
-    ret = libyamlscript.graal_tear_down_isolate(isolatethread)
-    if ret != 0:
-      raise Exception("Failed to tear down isolate.")
-
     # Check for libyamlscript error in JSON response:
     self.error = resp.get('error')
     if self.error:
       raise Exception(self.error['cause'])
 
     # Get the response object from evaluating the YAMLScript string:
-    data = resp.get('data')
-    if data is None:
+    if not 'data' in resp:
       raise Exception("Unexpected response from 'libyamlscript'")
+    data = resp.get('data')
 
     # Return the response object:
     return data
+
+  # YAMLScript instance destructor:
+  def __del__(self):
+    # Tear down the isolate thread to free resources:
+    rc = libyamlscript.graal_tear_down_isolate(self.isolatethread)
+    if rc != 0:
+      raise Exception("Failed to tear down isolate")
```

### Comparing `yamlscript-0.1.5/lib/yamlscript.egg-info/PKG-INFO` & `yamlscript-0.1.50/lib/yamlscript.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlscript
-Version: 0.1.5
+Version: 0.1.50
 Summary: Program in YAML
 Home-page: https://github.com/ingydotnet/yamlscript
 Author: Ingy döt Net
 Author-email: ingy@ingy.net
 License: MIT
 Keywords: yaml,language
 Platform: UNKNOWN
```

### Comparing `yamlscript-0.1.5/setup.py` & `yamlscript-0.1.50/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = '0.1.5'
+version = '0.1.50'
 
 from setuptools import setup
 import pathlib
 
 root = pathlib.Path(__file__).parent.resolve()
 
 long_description = \
```

