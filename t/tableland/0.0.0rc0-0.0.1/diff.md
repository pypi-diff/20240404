# Comparing `tmp/tableland-0.0.0rc0.tar.gz` & `tmp/tableland-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableland-0.0.0rc0.tar", max compression
+gzip compressed data, was "tableland-0.0.1.tar", max compression
```

## Comparing `tableland-0.0.0rc0.tar` & `tableland-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1092 2024-04-04 06:06:28.522639 tableland-0.0.0rc0/LICENSE
--rw-r--r--   0        0        0     9723 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/LICENSE-APACHE
--rw-r--r--   0        0        0     5760 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/README.md
--rw-r--r--   0        0        0     1497 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1120 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/__main__.py
--rw-r--r--   0        0        0     8346 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/database.py
--rw-r--r--   0        0        0     6478 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/helpers.py
--rw-r--r--   0        0        0     3268 2024-04-04 06:06:28.526639 tableland-0.0.0rc0/tableland/types.py
--rw-r--r--   0        0        0     6383 1970-01-01 00:00:00.000000 tableland-0.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-04 06:12:33.926030 tableland-0.0.1/LICENSE
+-rw-r--r--   0        0        0     9723 2024-04-04 06:12:33.926030 tableland-0.0.1/LICENSE-APACHE
+-rw-r--r--   0        0        0     5800 2024-04-04 06:12:33.926030 tableland-0.0.1/README.md
+-rw-r--r--   0        0        0     1491 2024-04-04 06:12:33.926030 tableland-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1120 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/__main__.py
+-rw-r--r--   0        0        0     8346 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/database.py
+-rw-r--r--   0        0        0     6478 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/helpers.py
+-rw-r--r--   0        0        0     3268 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/types.py
+-rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 tableland-0.0.1/PKG-INFO
```

### Comparing `tableland-0.0.0rc0/LICENSE` & `tableland-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0rc0/LICENSE-APACHE` & `tableland-0.0.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0rc0/README.md` & `tableland-0.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
 [![PyPI version](https://badge.fury.io/py/tableland.svg)](https://badge.fury.io/py/tableland)
 
 > A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 
 ## Background
 
-This package is a simple Tableland SDK for Python. It is designed to work with the [Tableland](https://tableland.xyz) network and uses the [web3.py](https://web3py.readthedocs.io/en/stable/) library for blockchain interacts.
+This package is a simple Python SDK for the [Tableland](https://tableland.xyz) network. It's built around the [web3.py](https://web3py.readthedocs.io/en/stable/) library for onchain interactions and lets developers create, read, and write data to Tableland tables.
 
 ## Install
 
 You can install with `pip`:
 
 ```sh
 pip install tableland
```

### Comparing `tableland-0.0.0rc0/pyproject.toml` & `tableland-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tableland"
-version = "0.0.0-pre.0"
+version = "0.0.1"
 description = "A minimal Tableland Python SDK for creating, writing, and reading onchain tables"
 authors = ["Dan Buchholz <dbuchholz30@gmail.com>"]
 license = "MIT AND Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `tableland-0.0.0rc0/tableland/__init__.py` & `tableland-0.0.1/tableland/__init__.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0rc0/tableland/database.py` & `tableland-0.0.1/tableland/database.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0rc0/tableland/helpers.py` & `tableland-0.0.1/tableland/helpers.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0rc0/tableland/types.py` & `tableland-0.0.1/tableland/types.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.0rc0/PKG-INFO` & `tableland-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableland
-Version: 0.0.0rc0
+Version: 0.0.1
 Summary: A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 License: MIT AND Apache-2.0
 Author: Dan Buchholz
 Author-email: dbuchholz30@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -21,15 +21,15 @@
 [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
 [![PyPI version](https://badge.fury.io/py/tableland.svg)](https://badge.fury.io/py/tableland)
 
 > A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 
 ## Background
 
-This package is a simple Tableland SDK for Python. It is designed to work with the [Tableland](https://tableland.xyz) network and uses the [web3.py](https://web3py.readthedocs.io/en/stable/) library for blockchain interacts.
+This package is a simple Python SDK for the [Tableland](https://tableland.xyz) network. It's built around the [web3.py](https://web3py.readthedocs.io/en/stable/) library for onchain interactions and lets developers create, read, and write data to Tableland tables.
 
 ## Install
 
 You can install with `pip`:
 
 ```sh
 pip install tableland
```

