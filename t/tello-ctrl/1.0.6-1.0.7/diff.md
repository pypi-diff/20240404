# Comparing `tmp/tello-ctrl-1.0.6.tar.gz` & `tmp/tello-ctrl-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tello-ctrl-1.0.6.tar", last modified: Wed Apr  3 22:14:29 2024, max compression
+gzip compressed data, was "tello-ctrl-1.0.7.tar", last modified: Thu Apr  4 00:57:19 2024, max compression
```

## Comparing `tello-ctrl-1.0.6.tar` & `tello-ctrl-1.0.7.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 22:14:29.293339 tello-ctrl-1.0.6/
--rw-rw-rw-   0        0        0    11556 2024-04-03 19:20:58.000000 tello-ctrl-1.0.6/License.txt
--rw-rw-rw-   0        0        0     2421 2024-04-03 22:14:29.292286 tello-ctrl-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1774 2024-04-03 22:08:30.000000 tello-ctrl-1.0.6/README.md
--rw-rw-rw-   0        0        0      773 2024-04-03 21:03:20.000000 tello-ctrl-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 22:14:29.293339 tello-ctrl-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 22:14:29.276898 tello-ctrl-1.0.6/tello_ctrl/
-drwxrwxrwx   0        0        0        0 2024-04-03 22:14:29.289066 tello-ctrl-1.0.6/tello_ctrl/common/
--rw-rw-rw-   0        0        0        0 2024-04-03 11:28:24.000000 tello-ctrl-1.0.6/tello_ctrl/common/__init__.py
--rw-rw-rw-   0        0        0     4117 2018-11-24 02:38:19.000000 tello-ctrl-1.0.6/tello_ctrl/common/crc.py
--rw-rw-rw-   0        0        0     3287 2024-03-17 13:23:42.000000 tello-ctrl-1.0.6/tello_ctrl/common/dispatcher.py
--rw-rw-rw-   0        0        0      374 2018-11-24 02:38:19.000000 tello-ctrl-1.0.6/tello_ctrl/common/event.py
--rw-rw-rw-   0        0        0    18291 2024-03-29 10:29:38.000000 tello-ctrl-1.0.6/tello_ctrl/common/protocol.py
--rw-rw-rw-   0        0        0      382 2018-11-24 02:38:19.000000 tello-ctrl-1.0.6/tello_ctrl/common/state.py
--rw-rw-rw-   0        0        0     1201 2024-03-21 16:49:47.000000 tello-ctrl-1.0.6/tello_ctrl/common/utils.py
--rw-rw-rw-   0        0        0     2749 2024-03-21 12:29:31.000000 tello-ctrl-1.0.6/tello_ctrl/common/video_stream.py
-drwxrwxrwx   0        0        0        0 2024-04-03 22:14:29.292286 tello-ctrl-1.0.6/tello_ctrl/tello_ctrl.egg-info/
--rw-rw-rw-   0        0        0     2421 2024-04-03 22:14:29.000000 tello-ctrl-1.0.6/tello_ctrl/tello_ctrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2024-04-03 22:14:29.000000 tello-ctrl-1.0.6/tello_ctrl/tello_ctrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 22:14:29.000000 tello-ctrl-1.0.6/tello_ctrl/tello_ctrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-03 22:14:29.000000 tello-ctrl-1.0.6/tello_ctrl/tello_ctrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 22:14:29.000000 tello-ctrl-1.0.6/tello_ctrl/tello_ctrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 00:57:19.383605 tello-ctrl-1.0.7/
+-rw-rw-rw-   0        0        0    11556 2024-04-03 19:20:58.000000 tello-ctrl-1.0.7/License.txt
+-rw-rw-rw-   0        0        0     2398 2024-04-04 00:57:19.382635 tello-ctrl-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1774 2024-04-03 22:08:30.000000 tello-ctrl-1.0.7/README.md
+-rw-rw-rw-   0        0        0      713 2024-04-04 00:57:14.000000 tello-ctrl-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 00:57:19.383605 tello-ctrl-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 00:57:19.374674 tello-ctrl-1.0.7/tello_ctrl/
+-rw-rw-rw-   0        0        0       56 2024-04-03 20:04:00.000000 tello-ctrl-1.0.7/tello_ctrl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:57:19.379636 tello-ctrl-1.0.7/tello_ctrl/common/
+-rw-rw-rw-   0        0        0        0 2024-04-03 11:28:24.000000 tello-ctrl-1.0.7/tello_ctrl/common/__init__.py
+-rw-rw-rw-   0        0        0     4117 2018-11-24 02:38:19.000000 tello-ctrl-1.0.7/tello_ctrl/common/crc.py
+-rw-rw-rw-   0        0        0     3287 2024-03-17 13:23:42.000000 tello-ctrl-1.0.7/tello_ctrl/common/dispatcher.py
+-rw-rw-rw-   0        0        0      374 2018-11-24 02:38:19.000000 tello-ctrl-1.0.7/tello_ctrl/common/event.py
+-rw-rw-rw-   0        0        0    18291 2024-03-29 10:29:38.000000 tello-ctrl-1.0.7/tello_ctrl/common/protocol.py
+-rw-rw-rw-   0        0        0      382 2018-11-24 02:38:19.000000 tello-ctrl-1.0.7/tello_ctrl/common/state.py
+-rw-rw-rw-   0        0        0     1201 2024-03-21 16:49:47.000000 tello-ctrl-1.0.7/tello_ctrl/common/utils.py
+-rw-rw-rw-   0        0        0     2749 2024-03-21 12:29:31.000000 tello-ctrl-1.0.7/tello_ctrl/common/video_stream.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:57:19.382635 tello-ctrl-1.0.7/tello_ctrl/tello_ctrl.egg-info/
+-rw-rw-rw-   0        0        0     2398 2024-04-04 00:57:19.000000 tello-ctrl-1.0.7/tello_ctrl/tello_ctrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2024-04-04 00:57:19.000000 tello-ctrl-1.0.7/tello_ctrl/tello_ctrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 00:57:19.000000 tello-ctrl-1.0.7/tello_ctrl/tello_ctrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 00:57:19.000000 tello-ctrl-1.0.7/tello_ctrl/tello_ctrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-04-04 00:57:19.000000 tello-ctrl-1.0.7/tello_ctrl/tello_ctrl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    85865 2024-04-03 20:42:11.000000 tello-ctrl-1.0.7/tello_ctrl/tello_ctrl.py
```

### Comparing `tello-ctrl-1.0.6/License.txt` & `tello-ctrl-1.0.7/License.txt`

 * *Files identical despite different names*

### Comparing `tello-ctrl-1.0.6/PKG-INFO` & `tello-ctrl-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: tello-ctrl
-Version: 1.0.6
+Version: 1.0.7
 Project-URL: Issues, https://github.com/sebdelp/tello-control/issues
 Project-URL: Repository, https://github.com/sebdelp/tello-control
 Keywords: tello,drone,Control,low level protocol,dji
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: License.txt
 Requires-Dist: av
-Requires-Dist: pillow
 Requires-Dist: opencv-python
 
 # tello-ctrl a python package to control your Tello drone
 
 This is a package to control your Tello Drone. A significant part of the code is from the TelloPy package 
 from Hanyazou and the original GOBOT project (https://gobot.io/blog/2018/04/20/hello-tello-hacking-drones-with-go)
```

### Comparing `tello-ctrl-1.0.6/README.md` & `tello-ctrl-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tello-ctrl-1.0.6/pyproject.toml` & `tello-ctrl-1.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tello-ctrl"
-version = "1.0.6"
+version = "1.0.7"
 readme = "README.md"
 
 keywords = ["tello", "drone","Control","low level protocol","dji"]
 classifiers = [
     "Programming Language :: Python :: 3",
 	'Intended Audience :: Developers',
 	'Operating System :: Microsoft :: Windows',
 	'Development Status :: 3 - Alpha',
 	'License :: OSI Approved :: Apache Software License',
 ]
 dependencies = [
     "av",
-    "pillow",
-	"opencv-python"
+    "opencv-python"
 ]
 
-[tool.setuptools.packages.find]
-where = ["tello_ctrl"]
-namespaces = false
-exclude = ['_pycache_']
+[tool.setuptools]
+package-dir = {""="tello_ctrl"}
+
 
 [project.urls]
 Issues = "https://github.com/sebdelp/tello-control/issues"
 Repository = "https://github.com/sebdelp/tello-control"
```

### Comparing `tello-ctrl-1.0.6/tello_ctrl/common/crc.py` & `tello-ctrl-1.0.7/tello_ctrl/common/crc.py`

 * *Files identical despite different names*

### Comparing `tello-ctrl-1.0.6/tello_ctrl/common/dispatcher.py` & `tello-ctrl-1.0.7/tello_ctrl/common/dispatcher.py`

 * *Files identical despite different names*

### Comparing `tello-ctrl-1.0.6/tello_ctrl/common/protocol.py` & `tello-ctrl-1.0.7/tello_ctrl/common/protocol.py`

 * *Files identical despite different names*

### Comparing `tello-ctrl-1.0.6/tello_ctrl/common/utils.py` & `tello-ctrl-1.0.7/tello_ctrl/common/utils.py`

 * *Files identical despite different names*

### Comparing `tello-ctrl-1.0.6/tello_ctrl/common/video_stream.py` & `tello-ctrl-1.0.7/tello_ctrl/common/video_stream.py`

 * *Files identical despite different names*

### Comparing `tello-ctrl-1.0.6/tello_ctrl/tello_ctrl.egg-info/PKG-INFO` & `tello-ctrl-1.0.7/tello_ctrl/tello_ctrl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: tello-ctrl
-Version: 1.0.6
+Version: 1.0.7
 Project-URL: Issues, https://github.com/sebdelp/tello-control/issues
 Project-URL: Repository, https://github.com/sebdelp/tello-control
 Keywords: tello,drone,Control,low level protocol,dji
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: License.txt
 Requires-Dist: av
-Requires-Dist: pillow
 Requires-Dist: opencv-python
 
 # tello-ctrl a python package to control your Tello drone
 
 This is a package to control your Tello Drone. A significant part of the code is from the TelloPy package 
 from Hanyazou and the original GOBOT project (https://gobot.io/blog/2018/04/20/hello-tello-hacking-drones-with-go)
```

