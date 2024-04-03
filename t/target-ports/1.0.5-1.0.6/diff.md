# Comparing `tmp/target-ports-1.0.5.tar.gz` & `tmp/target-ports-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-1.0.5.tar", last modified: Wed Apr  3 22:09:09 2024, max compression
+gzip compressed data, was "target-ports-1.0.6.tar", last modified: Wed Apr  3 22:53:29 2024, max compression
```

## Comparing `target-ports-1.0.5.tar` & `target-ports-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:09:09.618787 target-ports-1.0.5/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.5/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 22:09:09.618206 target-ports-1.0.5/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 21:12:11.000000 target-ports-1.0.5/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 22:07:50.000000 target-ports-1.0.5/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 22:09:09.618861 target-ports-1.0.5/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:09:09.601154 target-ports-1.0.5/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:09:09.604374 target-ports-1.0.5/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.5/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     6217 2024-04-03 22:08:51.000000 target-ports-1.0.5/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:09:09.617600 target-ports-1.0.5/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 22:09:09.000000 target-ports-1.0.5/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 22:09:09.000000 target-ports-1.0.5/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 22:09:09.000000 target-ports-1.0.5/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 22:09:09.000000 target-ports-1.0.5/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 22:09:09.000000 target-ports-1.0.5/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 22:09:09.000000 target-ports-1.0.5/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:53:29.046998 target-ports-1.0.6/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.6/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 22:53:29.046643 target-ports-1.0.6/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 22:52:42.000000 target-ports-1.0.6/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 22:52:33.000000 target-ports-1.0.6/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 22:53:29.047048 target-ports-1.0.6/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:53:29.033334 target-ports-1.0.6/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:53:29.035888 target-ports-1.0.6/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.6/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     6219 2024-04-03 22:52:30.000000 target-ports-1.0.6/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:53:29.046228 target-ports-1.0.6/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 22:53:29.000000 target-ports-1.0.6/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 22:53:29.000000 target-ports-1.0.6/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 22:53:29.000000 target-ports-1.0.6/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 22:53:29.000000 target-ports-1.0.6/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 22:53:29.000000 target-ports-1.0.6/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 22:53:29.000000 target-ports-1.0.6/src/target_ports.egg-info/top_level.txt
```

### Comparing `target-ports-1.0.5/LICENSE` & `target-ports-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.5/PKG-INFO` & `target-ports-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.5
+Version: 1.0.6
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -46,15 +46,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
 Requires-Dist: optioner>=1.4.5
 
 ![PyPI - Version](https://img.shields.io/pypi/v/target-ports)
 ![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/target-ports)
-![Static Badge](https://img.shields.io/badge/Dependencies-optioner%3E%3D1.4.4%2C%20termcolor-purple?style=plastic&logo=python&logoColor=pink&link=https%3A%2F%2Fgithub.com%2Fd33pster%2Foptioner)
+![Static Badge](https://img.shields.io/badge/Dependencies-optioner%3E%3D1.4.5%2C%20termcolor-purple?style=plastic&logo=python&logoColor=pink&link=https%3A%2F%2Fgithub.com%2Fd33pster%2Foptioner)
 
 
 # Overview
 
 target-ports is a basic port scanner written in python and makes use of socket programming to identify open ports.
 
 ## Installation
```

### Comparing `target-ports-1.0.5/README.md` & `target-ports-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![PyPI - Version](https://img.shields.io/pypi/v/target-ports)
 ![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/target-ports)
-![Static Badge](https://img.shields.io/badge/Dependencies-optioner%3E%3D1.4.4%2C%20termcolor-purple?style=plastic&logo=python&logoColor=pink&link=https%3A%2F%2Fgithub.com%2Fd33pster%2Foptioner)
+![Static Badge](https://img.shields.io/badge/Dependencies-optioner%3E%3D1.4.5%2C%20termcolor-purple?style=plastic&logo=python&logoColor=pink&link=https%3A%2F%2Fgithub.com%2Fd33pster%2Foptioner)
 
 
 # Overview
 
 target-ports is a basic port scanner written in python and makes use of socket programming to identify open ports.
 
 ## Installation
```

### Comparing `target-ports-1.0.5/pyproject.toml` & `target-ports-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "1.0.5"
+version = "1.0.6"
 description = "Scan ports of a target"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
```

### Comparing `target-ports-1.0.5/src/target_ports/target_ports.py` & `target-ports-1.0.6/src/target_ports/target_ports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-__version__ = '0.1'
+__version__ = '1.0.6'
 
 from socket import socket, AF_INET, SOCK_STREAM, gaierror, error
 from optioner import options
 from sys import argv
 from re import match
 import termcolor
```

### Comparing `target-ports-1.0.5/src/target_ports.egg-info/PKG-INFO` & `target-ports-1.0.6/src/target_ports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.5
+Version: 1.0.6
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -46,15 +46,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: termcolor
 Requires-Dist: optioner>=1.4.5
 
 ![PyPI - Version](https://img.shields.io/pypi/v/target-ports)
 ![GitHub last commit](https://img.shields.io/github/last-commit/d33pster/target-ports)
-![Static Badge](https://img.shields.io/badge/Dependencies-optioner%3E%3D1.4.4%2C%20termcolor-purple?style=plastic&logo=python&logoColor=pink&link=https%3A%2F%2Fgithub.com%2Fd33pster%2Foptioner)
+![Static Badge](https://img.shields.io/badge/Dependencies-optioner%3E%3D1.4.5%2C%20termcolor-purple?style=plastic&logo=python&logoColor=pink&link=https%3A%2F%2Fgithub.com%2Fd33pster%2Foptioner)
 
 
 # Overview
 
 target-ports is a basic port scanner written in python and makes use of socket programming to identify open ports.
 
 ## Installation
```

