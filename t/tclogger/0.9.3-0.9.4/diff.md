# Comparing `tmp/tclogger-0.9.3.tar.gz` & `tmp/tclogger-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tclogger-0.9.3.tar", last modified: Mon Mar 11 09:42:38 2024, max compression
+gzip compressed data, was "tclogger-0.9.4.tar", last modified: Thu Apr  4 18:31:33 2024, max compression
```

## Comparing `tclogger-0.9.3.tar` & `tclogger-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:42:38.178104 tclogger-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-11 09:42:15.000000 tclogger-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-11 09:42:38.178104 tclogger-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-11 09:42:15.000000 tclogger-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-11 09:42:15.000000 tclogger-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 09:42:38.178104 tclogger-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:42:38.174104 tclogger-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:42:38.178104 tclogger-0.9.3/src/tclogger/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-11 09:42:15.000000 tclogger-0.9.3/src/tclogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-03-11 09:42:15.000000 tclogger-0.9.3/src/tclogger/tclogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 09:42:38.178104 tclogger-0.9.3/src/tclogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-11 09:42:38.000000 tclogger-0.9.3/src/tclogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-11 09:42:38.000000 tclogger-0.9.3/src/tclogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 09:42:38.000000 tclogger-0.9.3/src/tclogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-11 09:42:38.000000 tclogger-0.9.3/src/tclogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 09:42:38.000000 tclogger-0.9.3/src/tclogger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:31:33.781635 tclogger-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-04 18:31:22.000000 tclogger-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 18:31:33.781635 tclogger-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-04 18:31:22.000000 tclogger-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-04 18:31:22.000000 tclogger-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:31:33.781635 tclogger-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:31:33.777635 tclogger-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:31:33.777635 tclogger-0.9.4/src/tclogger/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 18:31:22.000000 tclogger-0.9.4/src/tclogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-04-04 18:31:22.000000 tclogger-0.9.4/src/tclogger/tclogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:31:33.781635 tclogger-0.9.4/src/tclogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 18:31:33.000000 tclogger-0.9.4/src/tclogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 18:31:33.000000 tclogger-0.9.4/src/tclogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:31:33.000000 tclogger-0.9.4/src/tclogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 18:31:33.000000 tclogger-0.9.4/src/tclogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 18:31:33.000000 tclogger-0.9.4/src/tclogger.egg-info/top_level.txt
```

### Comparing `tclogger-0.9.3/LICENSE` & `tclogger-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tclogger-0.9.3/PKG-INFO` & `tclogger-0.9.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclogger
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python terminal colored logger
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/tclogger
 Project-URL: Issues, https://github.com/Hansimov/tclogger/issues
 Project-URL: Changelog, https://github.com/Hansimov/tclogger/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,17 +14,23 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: termcolor
 
 # tclogger
 Python terminal colored logger
 
+![](https://img.shields.io/pypi/v/tclogger?label=tclogger&color=blue&cacheSeconds=60)
+
 ## Install
 ```sh
 pip install tclogger
 ```
 
 ## Usage
 ```py
-from tclogger import logger
-logger.note("hello world")
+from tclogger import logger, count_digits, Runtimer
+with Runtimer():
+    logger.note("hello world")
+    logger.mesg(count_digits(1234567890))
+
+shell_cmd("ls -l")
 ```
```

### Comparing `tclogger-0.9.3/pyproject.toml` & `tclogger-0.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tclogger"
-version = "0.9.3"
+version = "0.9.4"
 authors = [
     { name="Hansimov" },
 ]
 description = "Python terminal colored logger"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `tclogger-0.9.3/src/tclogger/tclogger.py` & `tclogger-0.9.4/src/tclogger/tclogger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import functools
 import inspect
 import json
 import logging
+import math
 import os
 import shutil
 import subprocess
 
 from pathlib import Path
 from requests.structures import CaseInsensitiveDict
 from termcolor import colored
@@ -33,14 +34,21 @@
     else:
         raise ValueError("Invalid fill_side")
 
     filled_str = f"{leading_fill_str}{text}{trailing_fill_str}"
     return filled_str
 
 
+# calculate digits of integer
+def count_digits(num, base: int = 10):
+    if num == 0:
+        return 0
+    return int(math.log(num, base) + 1)
+
+
 class TCLogger(logging.Logger):
     LOG_METHODS = {
         "err": ("error", "red"),
         "warn": ("warning", "light_red"),
         "note": ("info", "light_magenta"),
         "mesg": ("info", "light_cyan"),
         "file": ("info", "light_blue"),
```

### Comparing `tclogger-0.9.3/src/tclogger.egg-info/PKG-INFO` & `tclogger-0.9.4/src/tclogger.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tclogger
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python terminal colored logger
 Author: Hansimov
 Project-URL: Homepage, https://github.com/Hansimov/tclogger
 Project-URL: Issues, https://github.com/Hansimov/tclogger/issues
 Project-URL: Changelog, https://github.com/Hansimov/tclogger/blob/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,17 +14,23 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: termcolor
 
 # tclogger
 Python terminal colored logger
 
+![](https://img.shields.io/pypi/v/tclogger?label=tclogger&color=blue&cacheSeconds=60)
+
 ## Install
 ```sh
 pip install tclogger
 ```
 
 ## Usage
 ```py
-from tclogger import logger
-logger.note("hello world")
+from tclogger import logger, count_digits, Runtimer
+with Runtimer():
+    logger.note("hello world")
+    logger.mesg(count_digits(1234567890))
+
+shell_cmd("ls -l")
 ```
```

