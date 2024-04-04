# Comparing `tmp/pyigor-0.1.6.tar.gz` & `tmp/pyigor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyigor-0.1.6.tar", last modified: Tue Oct 31 01:21:40 2023, max compression
+gzip compressed data, was "pyigor-0.2.0.tar", last modified: Thu Apr  4 13:20:19 2024, max compression
```

## Comparing `pyigor-0.1.6.tar` & `pyigor-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-10-31 01:21:40.274043 pyigor-0.1.6/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 pyigor-0.1.6/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       26 2023-01-22 05:57:41.000000 pyigor-0.1.6/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     2393 2023-10-31 01:21:40.273982 pyigor-0.1.6/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     1388 2023-01-24 02:29:07.000000 pyigor-0.1.6/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 pyigor-0.1.6/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)     1053 2023-10-31 01:21:40.274300 pyigor-0.1.6/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 pyigor-0.1.6/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-10-31 01:21:40.271623 pyigor-0.1.6/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-10-31 01:21:40.273024 pyigor-0.1.6/src/pyigor/
--rw-r--r--   0 shuntaro   (501) staff       (20)       36 2023-01-22 05:51:31.000000 pyigor-0.1.6/src/pyigor/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)      276 2023-10-31 01:21:18.000000 pyigor-0.1.6/src/pyigor/__main__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     6236 2023-10-31 01:18:51.000000 pyigor-0.1.6/src/pyigor/pyigor.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2023-10-31 01:21:40.273746 pyigor-0.1.6/src/pyigor.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     2393 2023-10-31 01:21:40.000000 pyigor-0.1.6/src/pyigor.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      303 2023-10-31 01:21:40.000000 pyigor-0.1.6/src/pyigor.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2023-10-31 01:21:40.000000 pyigor-0.1.6/src/pyigor.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       21 2023-10-31 01:21:40.000000 pyigor-0.1.6/src/pyigor.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        7 2023-10-31 01:21:40.000000 pyigor-0.1.6/src/pyigor.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-04 13:20:19.484627 pyigor-0.2.0/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 pyigor-0.2.0/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       26 2023-01-22 05:57:41.000000 pyigor-0.2.0/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2360 2024-04-04 13:20:19.484569 pyigor-0.2.0/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1553 2024-04-04 10:54:26.000000 pyigor-0.2.0/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 pyigor-0.2.0/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      899 2024-04-04 13:20:19.484875 pyigor-0.2.0/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 pyigor-0.2.0/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-04 13:20:19.481792 pyigor-0.2.0/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-04 13:20:19.483451 pyigor-0.2.0/src/pyigor/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       36 2023-01-22 05:51:31.000000 pyigor-0.2.0/src/pyigor/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)      276 2023-10-31 01:21:18.000000 pyigor-0.2.0/src/pyigor/__main__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     7148 2024-04-04 11:01:30.000000 pyigor-0.2.0/src/pyigor/pyigor.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-04 13:20:19.484365 pyigor-0.2.0/src/pyigor.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2360 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      303 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       21 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        7 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/top_level.txt
```

### Comparing `pyigor-0.1.6/LICENSE.txt` & `pyigor-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyigor-0.1.6/PKG-INFO` & `pyigor-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: pyigor
-Version: 0.1.6
+Version: 0.2.0
 Summary: Bridging between Python and Igor Pro
 Home-page: https://github.com/chocolate-icecream/pyigor
 Author: chocolate-icecream
 Project-URL: Bug Tracker, https://github.com/chocolate-icecream/pyigor/issues
 Keywords: Igor
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: flask>=2.1
@@ -78,7 +74,15 @@
 By using Connection(security_hole=True), you can call any Python code. Meanwhile, this option makes it possible to execute any Python code by HTTP requests: http://localhost/code -> `eval(code)`. Do not use unless you are sure of it.
 
 ###### Calling registered functions from Igor Pro
 
 ```
 print PyIgorCall("myfunc(10)")
 ```
+
+
+
+## Contributors
+
+A special thanks to the people who have contributed to this project:
+\- [@nlyamada](https://github.com/nlyamada) - Made compatible with Windows
+
```

### Comparing `pyigor-0.1.6/README.md` & `pyigor-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -52,7 +52,15 @@
 By using Connection(security_hole=True), you can call any Python code. Meanwhile, this option makes it possible to execute any Python code by HTTP requests: http://localhost/code -> `eval(code)`. Do not use unless you are sure of it.
 
 ###### Calling registered functions from Igor Pro
 
 ```
 print PyIgorCall("myfunc(10)")
 ```
+
+
+
+## Contributors
+
+A special thanks to the people who have contributed to this project:
+\- [@nlyamada](https://github.com/nlyamada) - Made compatible with Windows
+
```

### Comparing `pyigor-0.1.6/src/pyigor/pyigor.py` & `pyigor-0.2.0/src/pyigor/pyigor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 import os
 import logging
 import threading
 import queue
 import uuid
 import subprocess
-import re, ast, json, glob
+import re, ast, json, glob, platform
 
 import flask
 from flask import Flask
 import h5py
 
+my_platform = "mac" if platform.platform(terse=True).startswith("macOS") else ("windows" if platform.platform(terse=True).startswith("Windows") else None)
+
+def alphanumeric_sort(l):
+    convert = lambda text: int(text) if text.isdigit() else text.lower()
+    alphanum_key = lambda key: [convert(c) for c in re.split('([0-9]+)', key)]
+    return sorted(l, key=alphanum_key, reverse=True)
+
 ##### OS dependent codes #####
 def find_executable_path():
-    exe_path = None
-    path_candidates = glob.glob("/Applications/Igor Pro*/Igor64.app/Contents/MacOS/Igor64")
+    exe_path_dict = {   "mac": "/Applications/Igor Pro * Folder/Igor64.app/Contents/MacOS/Igor64",
+                        "windows": "C:\Program Files\WaveMetrics\Igor Pro * Folder\IgorBinaries_x64\Igor64.exe"}
+
+    path_candidates = glob.glob(exe_path_dict[my_platform])
     assert len(path_candidates) > 0, "Cannot find Igor Pro"
-    exe_path = path_candidates[0]
+
+    exe_path = alphanumeric_sort(path_candidates)[0] # get the newest version
     return exe_path
 
+def execute_command_on_my_platform(command, executable_path):
+    if my_platform == "mac":
+        subprocess.run([executable_path, "-Q", "-X", command])
+    if my_platform == "windows":
+        temp = subprocess.list2cmdline([executable_path, "-Q", "-X"])
+        subprocess.run(f"{temp} {command}")
+
 def convert_to_igor_path(path):
     return path.replace(os.path.sep, ":")
 ##### OS dependent codes #####
 
 
 class Connection:
     TIMEOUT = 3
@@ -149,15 +166,15 @@
         path = os.path.join(self._basepath, f"temp_pyigor_{self._port}.h5")
         if for_igor:
             path = convert_to_igor_path(path)
         return path
 
     
     def execute_command(self, command):
-        subprocess.run([self._executable_path, "-Q", "-X", command])
+        execute_command_on_my_platform(command, self._executable_path)
 
     def wait_done(self):
         try:
             while True:
                if input("Input q to finish:") == "q":
                    break
         except KeyboardInterrupt:
@@ -169,17 +186,17 @@
             return f(*args, **kwargs)
         self._registered_functions[f.__name__] == f
         return wrapper
 
 class Wave:
     def __init__(self, array):
         self.array = array
-        self.offsets = 0
-        self.deltas = 1
-        self.units = None
+        self.offset = [0]
+        self.delta = [1]
+        self.units = [None]
     
     @classmethod
     def from_dict(cls, d):
         wave = Wave(d["array"])
         return wave
     
     def __str__(self):
```

### Comparing `pyigor-0.1.6/src/pyigor.egg-info/PKG-INFO` & `pyigor-0.2.0/src/pyigor.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: pyigor
-Version: 0.1.6
+Version: 0.2.0
 Summary: Bridging between Python and Igor Pro
 Home-page: https://github.com/chocolate-icecream/pyigor
 Author: chocolate-icecream
 Project-URL: Bug Tracker, https://github.com/chocolate-icecream/pyigor/issues
 Keywords: Igor
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: flask>=2.1
@@ -78,7 +74,15 @@
 By using Connection(security_hole=True), you can call any Python code. Meanwhile, this option makes it possible to execute any Python code by HTTP requests: http://localhost/code -> `eval(code)`. Do not use unless you are sure of it.
 
 ###### Calling registered functions from Igor Pro
 
 ```
 print PyIgorCall("myfunc(10)")
 ```
+
+
+
+## Contributors
+
+A special thanks to the people who have contributed to this project:
+\- [@nlyamada](https://github.com/nlyamada) - Made compatible with Windows
+
```

