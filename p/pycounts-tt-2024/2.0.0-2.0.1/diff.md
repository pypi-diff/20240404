# Comparing `tmp/pycounts_tt_2024-2.0.0.tar.gz` & `tmp/pycounts_tt_2024-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycounts_tt_2024-2.0.0.tar", max compression
+gzip compressed data, was "pycounts_tt_2024-2.0.1.tar", max compression
```

## Comparing `pycounts_tt_2024-2.0.0.tar` & `pycounts_tt_2024-2.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1074 2024-01-30 16:45:57.163092 pycounts_tt_2024-2.0.0/LICENSE
--rw-r--r--   0        0        0     1192 2024-01-30 16:45:57.163092 pycounts_tt_2024-2.0.0/README.md
--rw-r--r--   0        0        0      927 2024-01-30 16:46:07.591112 pycounts_tt_2024-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      118 2024-01-30 16:45:57.167092 pycounts_tt_2024-2.0.0/src/pycounts_tt_2024/__init__.py
--rw-r--r--   0        0        0      816 2024-01-30 16:45:57.167092 pycounts_tt_2024-2.0.0/src/pycounts_tt_2024/plotting_tt_2024.py
--rw-r--r--   0        0        0     1419 2024-01-30 16:45:57.167092 pycounts_tt_2024-2.0.0/src/pycounts_tt_2024/pycounts_tt_2024.py
--rw-r--r--   0        0        0     1739 1970-01-01 00:00:00.000000 pycounts_tt_2024-2.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-04-04 15:46:07.461280 pycounts_tt_2024-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1195 2024-04-04 15:46:07.461280 pycounts_tt_2024-2.0.1/README.md
+-rw-r--r--   0        0        0      927 2024-04-04 15:46:19.033305 pycounts_tt_2024-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-04-04 15:46:07.465280 pycounts_tt_2024-2.0.1/src/pycounts_tt_2024/__init__.py
+-rw-r--r--   0        0        0      816 2024-04-04 15:46:07.465280 pycounts_tt_2024-2.0.1/src/pycounts_tt_2024/plotting_tt_2024.py
+-rw-r--r--   0        0        0     1419 2024-04-04 15:46:07.465280 pycounts_tt_2024-2.0.1/src/pycounts_tt_2024/pycounts_tt_2024.py
+-rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 pycounts_tt_2024-2.0.1/PKG-INFO
```

### Comparing `pycounts_tt_2024-2.0.0/LICENSE` & `pycounts_tt_2024-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycounts_tt_2024-2.0.0/README.md` & `pycounts_tt_2024-2.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pycounts_tt_2024
 
 [![Documentation Status](https://readthedocs.org/projects/pycounts-tt-2024/badge/?version=latest)](https://pycounts-tt-2024.readthedocs.io/en/latest/?badge=latest)
 
-Author: Tiffany Timbers
+Author: Tiffany A. Timbers
 
 Calculate word counts in a text file!!!
 
 ## Installation
 
 ```bash
 $ pip install pycounts_tt_2024
```

### Comparing `pycounts_tt_2024-2.0.0/pyproject.toml` & `pycounts_tt_2024-2.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycounts_tt_2024"
-version = "2.0.0"
+version = "2.0.1"
 description = "Calculate word counts in a text file!"
 authors = ["Tiffany Timbers"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `pycounts_tt_2024-2.0.0/src/pycounts_tt_2024/plotting_tt_2024.py` & `pycounts_tt_2024-2.0.1/src/pycounts_tt_2024/plotting_tt_2024.py`

 * *Files identical despite different names*

### Comparing `pycounts_tt_2024-2.0.0/src/pycounts_tt_2024/pycounts_tt_2024.py` & `pycounts_tt_2024-2.0.1/src/pycounts_tt_2024/pycounts_tt_2024.py`

 * *Files identical despite different names*

### Comparing `pycounts_tt_2024-2.0.0/PKG-INFO` & `pycounts_tt_2024-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycounts_tt_2024
-Version: 2.0.0
+Version: 2.0.1
 Summary: Calculate word counts in a text file!
 License: MIT
 Author: Tiffany Timbers
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,15 +14,15 @@
 Requires-Dist: matplotlib (>=3.8.2)
 Description-Content-Type: text/markdown
 
 # pycounts_tt_2024
 
 [![Documentation Status](https://readthedocs.org/projects/pycounts-tt-2024/badge/?version=latest)](https://pycounts-tt-2024.readthedocs.io/en/latest/?badge=latest)
 
-Author: Tiffany Timbers
+Author: Tiffany A. Timbers
 
 Calculate word counts in a text file!!!
 
 ## Installation
 
 ```bash
 $ pip install pycounts_tt_2024
```

