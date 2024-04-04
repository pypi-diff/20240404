# Comparing `tmp/pyhelper_utils-0.0.3.tar.gz` & `tmp/pyhelper_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelper_utils-0.0.3.tar", max compression
+gzip compressed data, was "pyhelper_utils-0.0.4.tar", max compression
```

## Comparing `pyhelper_utils-0.0.3.tar` & `pyhelper_utils-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-03 15:36:29.586323 pyhelper_utils-0.0.3/LICENSE
--rw-r--r--   0        0        0      680 2024-04-03 15:36:29.587323 pyhelper_utils-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-04-03 15:36:29.590323 pyhelper_utils-0.0.3/pyhelper_utils/__init__.py
--rw-r--r--   0        0        0     1798 2024-04-03 15:36:29.590323 pyhelper_utils-0.0.3/pyhelper_utils/general.py
--rw-r--r--   0        0        0     2286 2024-04-03 15:36:29.590323 pyhelper_utils-0.0.3/pyhelper_utils/shell.py
--rw-r--r--   0        0        0     1511 2024-04-03 15:36:36.436267 pyhelper_utils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1616 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-04 10:58:45.508589 pyhelper_utils-0.0.4/LICENSE
+-rw-r--r--   0        0        0      680 2024-04-04 10:58:45.508589 pyhelper_utils-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-04 10:58:45.508589 pyhelper_utils-0.0.4/pyhelper_utils/__init__.py
+-rw-r--r--   0        0        0     1798 2024-04-04 10:58:45.509589 pyhelper_utils-0.0.4/pyhelper_utils/general.py
+-rw-r--r--   0        0        0     1215 2024-04-04 10:58:45.509589 pyhelper_utils-0.0.4/pyhelper_utils/notifications.py
+-rw-r--r--   0        0        0     2286 2024-04-04 10:58:45.509589 pyhelper_utils-0.0.4/pyhelper_utils/shell.py
+-rw-r--r--   0        0        0     1532 2024-04-04 10:58:49.221558 pyhelper_utils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1658 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.4/PKG-INFO
```

### Comparing `pyhelper_utils-0.0.3/LICENSE` & `pyhelper_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.3/README.md` & `pyhelper_utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.3/pyhelper_utils/general.py` & `pyhelper_utils-0.0.4/pyhelper_utils/general.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.3/pyhelper_utils/shell.py` & `pyhelper_utils-0.0.4/pyhelper_utils/shell.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.3/pyproject.toml` & `pyhelper_utils-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "pyhelper-utils"
-version = "0.0.3"
+version = "0.0.4"
 description = "Collective utility functions for python projects"
 readme = "README.md"
 repository = "https://github.com/RedHatQE/pyhelper-utils"
 authors = [
   "Meni Yakove <myakove@gmail.com>",
   "Ruth Netser <rnetser@gmail.com>",
   "Debarati Basu-Nag <dbasunag@redhat.com>",
@@ -36,14 +36,15 @@
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-simple-logger = "^1.0.19"
+requests = "^2.31.0"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.14.0"
```

### Comparing `pyhelper_utils-0.0.3/PKG-INFO` & `pyhelper_utils-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelper-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Collective utility functions for python projects
 Home-page: https://github.com/RedHatQE/pyhelper-utils
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: python-simple-logger (>=1.0.19,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://github.com/RedHatQE/pyhelper-utils/blob/main/README.md
 Project-URL: Repository, https://github.com/RedHatQE/pyhelper-utils
 Description-Content-Type: text/markdown
 
 # pyhelper-utils
 Repository for various python utilities
 ## Installation
```

