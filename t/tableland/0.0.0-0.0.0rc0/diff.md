# Comparing `tmp/tableland-0.0.0.tar.gz` & `tmp/tableland-0.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableland-0.0.0.tar", max compression
+gzip compressed data, was "tableland-0.0.0rc0.tar", max compression
```

## Comparing `tableland-0.0.0.tar` & `tableland-0.0.0rc0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1092 2024-03-28 22:26:33.294056 tableland-0.0.0/LICENSE
--rw-r--r--   0        0        0     9723 2024-03-28 22:25:56.228374 tableland-0.0.0/LICENSE-APACHE
--rw-r--r--   0        0        0     5666 2024-04-04 04:53:25.879251 tableland-0.0.0/README.md
--rw-r--r--   0        0        0     1491 2024-04-04 05:19:45.246731 tableland-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1120 2024-04-04 04:50:22.113829 tableland-0.0.0/tableland/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 19:33:35.553404 tableland-0.0.0/tableland/__main__.py
--rw-r--r--   0        0        0     8346 2024-04-04 04:50:22.118833 tableland-0.0.0/tableland/database.py
--rw-r--r--   0        0        0     6478 2024-04-04 04:50:22.116536 tableland-0.0.0/tableland/helpers.py
--rw-r--r--   0        0        0     3268 2024-04-03 23:42:44.792540 tableland-0.0.0/tableland/types.py
--rw-r--r--   0        0        0     6286 1970-01-01 00:00:00.000000 tableland-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-04 06:06:28.522639 tableland-0.0.0rc0/LICENSE
+-rw-r--r--   0        0        0     9723 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/LICENSE-APACHE
+-rw-r--r--   0        0        0     5760 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/README.md
+-rw-r--r--   0        0        0     1497 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1120 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/__main__.py
+-rw-r--r--   0        0        0     8346 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/database.py
+-rw-r--r--   0        0        0     6478 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/helpers.py
+-rw-r--r--   0        0        0     3268 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/types.py
+-rw-r--r--   0        0        0     6383 1970-01-01 00:00:00.000000 tableland-0.0.0rc0/PKG-INFO
```

### Comparing `tableland-0.0.0/LICENSE` & `tableland-0.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0/LICENSE-APACHE` & `tableland-0.0.0rc0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0/README.md` & `tableland-0.0.0rc0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # tableland.py
 
 [![License: MIT AND Apache-2.0](https://img.shields.io/badge/License-MIT%20AND%20Apache--2.0-blue.svg)](./LICENSE)
 [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
+[![PyPI version](https://badge.fury.io/py/tableland.svg)](https://badge.fury.io/py/tableland)
 
 > A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 
 ## Background
 
 This package is a simple Tableland SDK for Python. It is designed to work with the [Tableland](https://tableland.xyz) network and uses the [web3.py](https://web3py.readthedocs.io/en/stable/) library for blockchain interacts.
```

### Comparing `tableland-0.0.0/pyproject.toml` & `tableland-0.0.0rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tableland"
-version = "0.0.0"
+version = "0.0.0-pre.0"
 description = "A minimal Tableland Python SDK for creating, writing, and reading onchain tables"
 authors = ["Dan Buchholz <dbuchholz30@gmail.com>"]
 license = "MIT AND Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tableland-0.0.0/tableland/__init__.py` & `tableland-0.0.0rc0/tableland/__init__.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0/tableland/database.py` & `tableland-0.0.0rc0/tableland/database.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0/tableland/helpers.py` & `tableland-0.0.0rc0/tableland/helpers.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0/tableland/types.py` & `tableland-0.0.0rc0/tableland/types.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0/PKG-INFO` & `tableland-0.0.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableland
-Version: 0.0.0
+Version: 0.0.0rc0
 Summary: A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 License: MIT AND Apache-2.0
 Author: Dan Buchholz
 Author-email: dbuchholz30@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Requires-Dist: web3 (>=6.16.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # tableland.py
 
 [![License: MIT AND Apache-2.0](https://img.shields.io/badge/License-MIT%20AND%20Apache--2.0-blue.svg)](./LICENSE)
 [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
+[![PyPI version](https://badge.fury.io/py/tableland.svg)](https://badge.fury.io/py/tableland)
 
 > A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 
 ## Background
 
 This package is a simple Tableland SDK for Python. It is designed to work with the [Tableland](https://tableland.xyz) network and uses the [web3.py](https://web3py.readthedocs.io/en/stable/) library for blockchain interacts.
```

