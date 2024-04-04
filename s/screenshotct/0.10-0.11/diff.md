# Comparing `tmp/screenshotct-0.10.tar.gz` & `tmp/screenshotct-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenshotct-0.10.tar", last modified: Thu Apr  4 02:02:42 2024, max compression
+gzip compressed data, was "screenshotct-0.11.tar", last modified: Thu Apr  4 02:04:43 2024, max compression
```

## Comparing `screenshotct-0.10.tar` & `screenshotct-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 02:02:42.052976 screenshotct-0.10/
--rw-rw-rw-   0        0        0     1148 2024-04-04 02:02:32.000000 screenshotct-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      107 2024-04-04 02:02:32.000000 screenshotct-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     1833 2024-04-04 02:02:42.052225 screenshotct-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-04-04 01:49:10.000000 screenshotct-0.10/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 02:02:42.046224 screenshotct-0.10/screenshotct/
--rw-rw-rw-   0        0        0     1122 2024-04-04 01:49:10.000000 screenshotct-0.10/screenshotct/README.MD
--rw-rw-rw-   0        0        0    10095 2024-04-04 02:01:13.000000 screenshotct-0.10/screenshotct/__init__.py
--rw-rw-rw-   0        0        0       27 2024-04-04 02:02:40.000000 screenshotct-0.10/screenshotct/requirements.txt
--rw-rw-rw-   0        0        0    50366 2024-04-04 02:02:40.000000 screenshotct-0.10/screenshotct/thirdparty.json
-drwxrwxrwx   0        0        0        0 2024-04-04 02:02:42.051474 screenshotct-0.10/screenshotct.egg-info/
--rw-rw-rw-   0        0        0     1833 2024-04-04 02:02:41.000000 screenshotct-0.10/screenshotct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-04-04 02:02:41.000000 screenshotct-0.10/screenshotct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 02:02:41.000000 screenshotct-0.10/screenshotct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-04 02:02:41.000000 screenshotct-0.10/screenshotct.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 02:02:41.000000 screenshotct-0.10/screenshotct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-04 02:02:42.053727 screenshotct-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1289 2024-04-04 02:02:40.000000 screenshotct-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 02:04:43.944186 screenshotct-0.11/
+-rw-rw-rw-   0        0        0     1148 2024-04-04 02:04:35.000000 screenshotct-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      107 2024-04-04 02:04:35.000000 screenshotct-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     1832 2024-04-04 02:04:43.944186 screenshotct-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1121 2024-04-04 02:04:17.000000 screenshotct-0.11/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 02:04:43.937434 screenshotct-0.11/screenshotct/
+-rw-rw-rw-   0        0        0     1121 2024-04-04 02:04:17.000000 screenshotct-0.11/screenshotct/README.MD
+-rw-rw-rw-   0        0        0    10095 2024-04-04 02:01:13.000000 screenshotct-0.11/screenshotct/__init__.py
+-rw-rw-rw-   0        0        0       27 2024-04-04 02:04:42.000000 screenshotct-0.11/screenshotct/requirements.txt
+-rw-rw-rw-   0        0        0    50366 2024-04-04 02:04:42.000000 screenshotct-0.11/screenshotct/thirdparty.json
+drwxrwxrwx   0        0        0        0 2024-04-04 02:04:43.943446 screenshotct-0.11/screenshotct.egg-info/
+-rw-rw-rw-   0        0        0     1832 2024-04-04 02:04:43.000000 screenshotct-0.11/screenshotct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2024-04-04 02:04:43.000000 screenshotct-0.11/screenshotct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 02:04:43.000000 screenshotct-0.11/screenshotct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-04 02:04:43.000000 screenshotct-0.11/screenshotct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 02:04:43.000000 screenshotct-0.11/screenshotct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-04 02:04:43.945732 screenshotct-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1289 2024-04-04 02:04:42.000000 screenshotct-0.11/setup.py
```

### Comparing `screenshotct-0.10/LICENSE.rst` & `screenshotct-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `screenshotct-0.10/PKG-INFO` & `screenshotct-0.11/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenshotct
-Version: 0.10
+Version: 0.11
 Summary: Screenshots - ctypes
 Home-page: https://github.com/hansalemaos/screenshotct
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: screenshots
 Classifier: Development Status :: 4 - Beta
@@ -18,15 +18,15 @@
 Requires-Dist: numpy
 
 
 # Screenshot with ctypes
 
 ## Tested against Windows 10 / Python 3.11 / Anaconda
 
-### pip install getpublicipv4
+### pip install screenshotct
 
 ```PY
 import cv2
 from screenshotct import take_screenshot
 import time
 from ctypes_window_info import get_window_infos
```

### Comparing `screenshotct-0.10/README.md` & `screenshotct-0.11/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Screenshot with ctypes
 
 ## Tested against Windows 10 / Python 3.11 / Anaconda
 
-### pip install getpublicipv4
+### pip install screenshotct
 
 ```PY
 import cv2
 from screenshotct import take_screenshot
 import time
 from ctypes_window_info import get_window_infos
```

### Comparing `screenshotct-0.10/screenshotct/README.MD` & `screenshotct-0.11/screenshotct/README.MD`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Screenshot with ctypes
 
 ## Tested against Windows 10 / Python 3.11 / Anaconda
 
-### pip install getpublicipv4
+### pip install screenshotct
 
 ```PY
 import cv2
 from screenshotct import take_screenshot
 import time
 from ctypes_window_info import get_window_infos
```

### Comparing `screenshotct-0.10/screenshotct/__init__.py` & `screenshotct-0.11/screenshotct/__init__.py`

 * *Files identical despite different names*

### Comparing `screenshotct-0.10/screenshotct/thirdparty.json` & `screenshotct-0.11/screenshotct/thirdparty.json`

 * *Files identical despite different names*

### Comparing `screenshotct-0.10/screenshotct.egg-info/PKG-INFO` & `screenshotct-0.11/screenshotct.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenshotct
-Version: 0.10
+Version: 0.11
 Summary: Screenshots - ctypes
 Home-page: https://github.com/hansalemaos/screenshotct
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: screenshots
 Classifier: Development Status :: 4 - Beta
@@ -18,15 +18,15 @@
 Requires-Dist: numpy
 
 
 # Screenshot with ctypes
 
 ## Tested against Windows 10 / Python 3.11 / Anaconda
 
-### pip install getpublicipv4
+### pip install screenshotct
 
 ```PY
 import cv2
 from screenshotct import take_screenshot
 import time
 from ctypes_window_info import get_window_infos
```

### Comparing `screenshotct-0.10/setup.py` & `screenshotct-0.11/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Screenshots - ctypes'''
 
 # Setting up
 setup(
     name="screenshotct",
     version=VERSION,
     license='MIT',
```

