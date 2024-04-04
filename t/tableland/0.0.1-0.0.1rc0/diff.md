# Comparing `tmp/tableland-0.0.1.tar.gz` & `tmp/tableland-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableland-0.0.1.tar", max compression
+gzip compressed data, was "tableland-0.0.1rc0.tar", max compression
```

## Comparing `tableland-0.0.1.tar` & `tableland-0.0.1rc0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1092 2024-04-04 06:12:33.926030 tableland-0.0.1/LICENSE
--rw-r--r--   0        0        0     9723 2024-04-04 06:12:33.926030 tableland-0.0.1/LICENSE-APACHE
--rw-r--r--   0        0        0     5800 2024-04-04 06:12:33.926030 tableland-0.0.1/README.md
--rw-r--r--   0        0        0     1491 2024-04-04 06:12:33.926030 tableland-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1120 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/__main__.py
--rw-r--r--   0        0        0     8346 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/database.py
--rw-r--r--   0        0        0     6478 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/helpers.py
--rw-r--r--   0        0        0     3268 2024-04-04 06:12:33.926030 tableland-0.0.1/tableland/types.py
--rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 tableland-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-04 06:47:42.486679 tableland-0.0.1rc0/LICENSE
+-rw-r--r--   0        0        0     9723 2024-04-04 06:47:42.486679 tableland-0.0.1rc0/LICENSE-APACHE
+-rw-r--r--   0        0        0     5800 2024-04-04 06:47:42.486679 tableland-0.0.1rc0/README.md
+-rw-r--r--   0        0        0    22663 2024-04-04 06:47:42.486679 tableland-0.0.1rc0/abi.json
+-rw-r--r--   0        0        0     1573 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/pyproject.toml
+-rw-r--r--   0        0        0     1120 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/__main__.py
+-rw-r--r--   0        0        0     8346 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/database.py
+-rw-r--r--   0        0        0     6478 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/helpers.py
+-rw-r--r--   0        0        0     3268 2024-04-04 06:47:42.490679 tableland-0.0.1rc0/tableland/types.py
+-rw-r--r--   0        0        0     6423 1970-01-01 00:00:00.000000 tableland-0.0.1rc0/PKG-INFO
```

### Comparing `tableland-0.0.1/LICENSE` & `tableland-0.0.1rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1/LICENSE-APACHE` & `tableland-0.0.1rc0/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1/README.md` & `tableland-0.0.1rc0/README.md`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1/pyproject.toml` & `tableland-0.0.1rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [tool.poetry]
 name = "tableland"
-version = "0.0.1"
+version = "0.0.1-pre.0"
 description = "A minimal Tableland Python SDK for creating, writing, and reading onchain tables"
 authors = ["Dan Buchholz <dbuchholz30@gmail.com>"]
 license = "MIT AND Apache-2.0"
 readme = "README.md"
+packages = [
+    { include = "abi.json" },
+    { include = "tableland" },
+]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 web3 = "^6.16.0"
 requests = "^2.31.0"
 sqlglot = "^23.6.3"
```

### Comparing `tableland-0.0.1/tableland/__init__.py` & `tableland-0.0.1rc0/tableland/__init__.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1/tableland/database.py` & `tableland-0.0.1rc0/tableland/database.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1/tableland/helpers.py` & `tableland-0.0.1rc0/tableland/helpers.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1/tableland/types.py` & `tableland-0.0.1rc0/tableland/types.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1/PKG-INFO` & `tableland-0.0.1rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableland
-Version: 0.0.1
+Version: 0.0.1rc0
 Summary: A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 License: MIT AND Apache-2.0
 Author: Dan Buchholz
 Author-email: dbuchholz30@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

