# Comparing `tmp/nowpy-0.1.2.tar.gz` & `tmp/nowpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nowpy-0.1.2.tar", max compression
+gzip compressed data, was "nowpy-0.1.3.tar", max compression
```

## Comparing `nowpy-0.1.2.tar` & `nowpy-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1909 2024-02-18 20:48:15.306827 nowpy-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-02-18 20:48:15.303889 nowpy-0.1.2/nowpy/__init__.py
--rw-r--r--   0        0        0     6836 2024-03-06 22:52:15.512326 nowpy-0.1.2/nowpy/main.py
--rw-r--r--   0        0        0      530 2024-03-06 22:52:33.220319 nowpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 nowpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-06 22:55:47.533625 nowpy-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1909 2024-02-18 20:48:15.306827 nowpy-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-02-18 20:48:15.303889 nowpy-0.1.3/nowpy/__init__.py
+-rw-r--r--   0        0        0     6819 2024-04-04 20:00:26.198563 nowpy-0.1.3/nowpy/main.py
+-rw-r--r--   0        0        0      509 2024-04-04 20:01:34.406608 nowpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 nowpy-0.1.3/PKG-INFO
```

### Comparing `nowpy-0.1.2/README.md` & `nowpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nowpy-0.1.2/nowpy/main.py` & `nowpy-0.1.3/nowpy/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import pythonads
 import typer
 import sys
 import os
 import subprocess
 from pathlib import Path
 import ast
 import toml
```

### Comparing `nowpy-0.1.2/PKG-INFO` & `nowpy-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: nowpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Run any Python file instantly, with just one command
 Home-page: https://github.com/WillDenby/nowpy
 License: MIT
 Author: WillDenby
 Author-email: 119456795+WillDenby@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pythonads (>=0.1.0,<0.2.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: virtualenv (>=20.25.0,<21.0.0)
 Project-URL: Repository, https://github.com/WillDenby/nowpy
 Description-Content-Type: text/markdown
 
 # nowpy - Run Any Python File Instantly
```

