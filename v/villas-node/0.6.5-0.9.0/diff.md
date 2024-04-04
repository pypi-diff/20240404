# Comparing `tmp/villas-node-0.6.5.tar.gz` & `tmp/villas-node-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/villas-node-0.6.5.tar", last modified: Tue Sep  3 19:01:14 2019, max compression
+gzip compressed data, was "dist/villas-node-0.9.0.tar", last modified: Tue Nov 12 22:18:39 2019, max compression
```

## Comparing `villas-node-0.6.5.tar` & `villas-node-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 stv0g      (501) staff       (20)        0 2019-09-03 19:01:14.000000 villas-node-0.6.5/
--rw-r--r--   0 stv0g      (501) staff       (20)     3454 2019-09-03 19:01:14.000000 villas-node-0.6.5/PKG-INFO
--rw-r--r--   0 stv0g      (501) staff       (20)     2271 2019-09-03 18:59:02.000000 villas-node-0.6.5/README.md
-drwxr-xr-x   0 stv0g      (501) staff       (20)        0 2019-09-03 19:01:14.000000 villas-node-0.6.5/bin/
--rwxr-xr-x   0 stv0g      (501) staff       (20)     1436 2019-09-03 18:59:02.000000 villas-node-0.6.5/bin/villas-cumulative-dist
--rwxr-xr-x   0 stv0g      (501) staff       (20)      370 2019-09-03 18:59:02.000000 villas-node-0.6.5/bin/villas-extract-rtt
--rwxr-xr-x   0 stv0g      (501) staff       (20)      316 2019-09-03 18:59:02.000000 villas-node-0.6.5/bin/villas-file-filter
--rwxr-xr-x   0 stv0g      (501) staff       (20)      510 2019-09-03 18:59:02.000000 villas-node-0.6.5/bin/villas-file-merge
--rw-r--r--   0 stv0g      (501) staff       (20)       38 2019-09-03 19:01:14.000000 villas-node-0.6.5/setup.cfg
--rw-r--r--   0 stv0g      (501) staff       (20)     1139 2019-09-03 19:00:45.000000 villas-node-0.6.5/setup.py
-drwxr-xr-x   0 stv0g      (501) staff       (20)        0 2019-09-03 19:01:14.000000 villas-node-0.6.5/villas/
-drwxr-xr-x   0 stv0g      (501) staff       (20)        0 2019-09-03 19:01:14.000000 villas-node-0.6.5/villas/node/
--rw-r--r--   0 stv0g      (501) staff       (20)        0 2019-09-03 18:59:02.000000 villas-node-0.6.5/villas/node/__init__.py
--rw-r--r--   0 stv0g      (501) staff       (20)     2742 2019-09-03 18:59:02.000000 villas-node-0.6.5/villas/node/node.py
--rw-r--r--   0 stv0g      (501) staff       (20)     1897 2019-09-03 18:59:02.000000 villas-node-0.6.5/villas/node/sample.py
-drwxr-xr-x   0 stv0g      (501) staff       (20)        0 2019-09-03 19:01:14.000000 villas-node-0.6.5/villas_node.egg-info/
--rw-r--r--   0 stv0g      (501) staff       (20)     3454 2019-09-03 19:01:14.000000 villas-node-0.6.5/villas_node.egg-info/PKG-INFO
--rw-r--r--   0 stv0g      (501) staff       (20)      353 2019-09-03 19:01:14.000000 villas-node-0.6.5/villas_node.egg-info/SOURCES.txt
--rw-r--r--   0 stv0g      (501) staff       (20)        1 2019-09-03 19:01:14.000000 villas-node-0.6.5/villas_node.egg-info/dependency_links.txt
--rw-r--r--   0 stv0g      (501) staff       (20)        9 2019-09-03 19:01:14.000000 villas-node-0.6.5/villas_node.egg-info/requires.txt
--rw-r--r--   0 stv0g      (501) staff       (20)        7 2019-09-03 19:01:14.000000 villas-node-0.6.5/villas_node.egg-info/top_level.txt
+drwxr-xr-x   0 stv0g_local   (501) staff       (20)        0 2019-11-12 22:18:39.000000 villas-node-0.9.0/
+-rw-r--r--   0 stv0g_local   (501) staff       (20)     3454 2019-11-12 22:18:39.000000 villas-node-0.9.0/PKG-INFO
+-rw-r--r--   0 stv0g_local   (501) staff       (20)     2271 2019-06-18 09:48:05.000000 villas-node-0.9.0/README.md
+drwxr-xr-x   0 stv0g_local   (501) staff       (20)        0 2019-11-12 22:18:39.000000 villas-node-0.9.0/bin/
+-rwxr-xr-x   0 stv0g_local   (501) staff       (20)     1436 2019-06-18 09:48:05.000000 villas-node-0.9.0/bin/villas-cumulative-dist
+-rwxr-xr-x   0 stv0g_local   (501) staff       (20)      370 2019-06-18 09:48:05.000000 villas-node-0.9.0/bin/villas-extract-rtt
+-rwxr-xr-x   0 stv0g_local   (501) staff       (20)      316 2019-06-18 09:48:05.000000 villas-node-0.9.0/bin/villas-file-filter
+-rwxr-xr-x   0 stv0g_local   (501) staff       (20)      510 2019-06-18 09:48:05.000000 villas-node-0.9.0/bin/villas-file-merge
+-rw-r--r--   0 stv0g_local   (501) staff       (20)       38 2019-11-12 22:18:39.000000 villas-node-0.9.0/setup.cfg
+-rw-r--r--   0 stv0g_local   (501) staff       (20)     1192 2019-11-12 22:18:06.000000 villas-node-0.9.0/setup.py
+drwxr-xr-x   0 stv0g_local   (501) staff       (20)        0 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas/
+drwxr-xr-x   0 stv0g_local   (501) staff       (20)        0 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas/human/
+-rw-r--r--   0 stv0g_local   (501) staff       (20)       60 2019-06-18 09:48:05.000000 villas-node-0.9.0/villas/human/__init__.py
+-rw-r--r--   0 stv0g_local   (501) staff       (20)      523 2019-06-18 09:48:05.000000 villas-node-0.9.0/villas/human/message.py
+-rw-r--r--   0 stv0g_local   (501) staff       (20)     1198 2019-06-18 09:48:05.000000 villas-node-0.9.0/villas/human/timestamp.py
+drwxr-xr-x   0 stv0g_local   (501) staff       (20)        0 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas/node/
+-rw-r--r--   0 stv0g_local   (501) staff       (20)        0 2019-10-27 19:24:41.000000 villas-node-0.9.0/villas/node/__init__.py
+-rw-r--r--   0 stv0g_local   (501) staff       (20)     2742 2019-06-18 09:48:05.000000 villas-node-0.9.0/villas/node/node.py
+-rw-r--r--   0 stv0g_local   (501) staff       (20)     1897 2019-06-18 09:48:05.000000 villas-node-0.9.0/villas/node/sample.py
+drwxr-xr-x   0 stv0g_local   (501) staff       (20)        0 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas_node.egg-info/
+-rw-r--r--   0 stv0g_local   (501) staff       (20)     3454 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas_node.egg-info/PKG-INFO
+-rw-r--r--   0 stv0g_local   (501) staff       (20)      428 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas_node.egg-info/SOURCES.txt
+-rw-r--r--   0 stv0g_local   (501) staff       (20)        1 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas_node.egg-info/dependency_links.txt
+-rw-r--r--   0 stv0g_local   (501) staff       (20)        9 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas_node.egg-info/requires.txt
+-rw-r--r--   0 stv0g_local   (501) staff       (20)        7 2019-11-12 22:18:39.000000 villas-node-0.9.0/villas_node.egg-info/top_level.txt
```

### Comparing `villas-node-0.6.5/PKG-INFO` & `villas-node-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villas-node
-Version: 0.6.5
+Version: 0.9.0
 Summary: Python-support for VILLASnode simulation-data gateway
 Home-page: https://git.rwth-aachen.de/acs/public/villas/VILLASnode
 Author: Steffen Vogel
 Author-email: acs-software@eonerc.rwth-aachen.de
 License: GPL-3.0
 Description: # VILLASnode Python Support
```

### Comparing `villas-node-0.6.5/README.md` & `villas-node-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `villas-node-0.6.5/bin/villas-cumulative-dist` & `villas-node-0.9.0/bin/villas-cumulative-dist`

 * *Files identical despite different names*

### Comparing `villas-node-0.6.5/setup.py` & `villas-node-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
-from setuptools import setup
+from setuptools import setup, find_namespace_packages
 from glob import glob
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name = 'villas-node',
-    version = '0.6.5',
+    version = '0.9.0',
     author = 'Steffen Vogel',
     author_email = 'acs-software@eonerc.rwth-aachen.de',
     description = 'Python-support for VILLASnode simulation-data gateway',
     license = 'GPL-3.0',
     keywords = 'simulation power system real-time villas',
     url = 'https://git.rwth-aachen.de/acs/public/villas/VILLASnode',
-    packages = [ 'villas.node' ],
+    packages = find_namespace_packages(include=['villas.*']),
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     classifiers = [
         'Development Status :: 4 - Beta',
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: MacOS :: MacOS X',
```

### Comparing `villas-node-0.6.5/villas/node/node.py` & `villas-node-0.9.0/villas/node/node.py`

 * *Files identical despite different names*

### Comparing `villas-node-0.6.5/villas/node/sample.py` & `villas-node-0.9.0/villas/node/sample.py`

 * *Files identical despite different names*

### Comparing `villas-node-0.6.5/villas_node.egg-info/PKG-INFO` & `villas-node-0.9.0/villas_node.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villas-node
-Version: 0.6.5
+Version: 0.9.0
 Summary: Python-support for VILLASnode simulation-data gateway
 Home-page: https://git.rwth-aachen.de/acs/public/villas/VILLASnode
 Author: Steffen Vogel
 Author-email: acs-software@eonerc.rwth-aachen.de
 License: GPL-3.0
 Description: # VILLASnode Python Support
```

