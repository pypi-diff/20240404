# Comparing `tmp/tableland-0.0.1rc1.tar.gz` & `tmp/tableland-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableland-0.0.1rc1.tar", max compression
+gzip compressed data, was "tableland-0.0.1rc2.tar", max compression
```

## Comparing `tableland-0.0.1rc1.tar` & `tableland-0.0.1rc2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1092 2024-04-04 07:02:19.547519 tableland-0.0.1rc1/LICENSE
--rw-r--r--   0        0        0     9723 2024-03-28 22:25:56.228374 tableland-0.0.1rc1/LICENSE-APACHE
--rw-r--r--   0        0        0     5810 2024-04-04 07:02:26.258854 tableland-0.0.1rc1/README.md
--rw-r--r--   0        0        0     1497 2024-04-04 07:01:42.570760 tableland-0.0.1rc1/pyproject.toml
--rw-r--r--   0        0        0     1120 2024-04-04 04:50:22.113829 tableland-0.0.1rc1/tableland/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 19:33:35.553404 tableland-0.0.1rc1/tableland/__main__.py
--rw-r--r--   0        0        0    22663 2024-04-02 02:05:50.567072 tableland-0.0.1rc1/tableland/abi.json
--rw-r--r--   0        0        0     8339 2024-04-04 06:58:40.742608 tableland-0.0.1rc1/tableland/database.py
--rw-r--r--   0        0        0     6478 2024-04-04 07:02:56.358179 tableland-0.0.1rc1/tableland/helpers.py
--rw-r--r--   0        0        0     3268 2024-04-03 23:42:44.792540 tableland-0.0.1rc1/tableland/types.py
--rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 tableland-0.0.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-04 07:02:19.547519 tableland-0.0.1rc2/LICENSE
+-rw-r--r--   0        0        0     9723 2024-03-28 22:25:56.228374 tableland-0.0.1rc2/LICENSE-APACHE
+-rw-r--r--   0        0        0     5810 2024-04-04 07:02:26.258854 tableland-0.0.1rc2/README.md
+-rw-r--r--   0        0        0     1530 2024-04-04 07:18:45.609749 tableland-0.0.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     1120 2024-04-04 04:50:22.113829 tableland-0.0.1rc2/tableland/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 19:33:35.553404 tableland-0.0.1rc2/tableland/__main__.py
+-rw-r--r--   0        0        0     8339 2024-04-04 06:58:40.742608 tableland-0.0.1rc2/tableland/database.py
+-rw-r--r--   0        0        0     6478 2024-04-04 07:02:56.358179 tableland-0.0.1rc2/tableland/helpers.py
+-rw-r--r--   0        0        0     3268 2024-04-03 23:42:44.792540 tableland-0.0.1rc2/tableland/types.py
+-rw-r--r--   0        0        0     6433 1970-01-01 00:00:00.000000 tableland-0.0.1rc2/PKG-INFO
```

### Comparing `tableland-0.0.1rc1/LICENSE` & `tableland-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc1/LICENSE-APACHE` & `tableland-0.0.1rc2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc1/README.md` & `tableland-0.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc1/pyproject.toml` & `tableland-0.0.1rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "tableland"
-version = "0.0.1-pre.1"
+version = "0.0.1-pre.2"
 description = "A minimal Tableland Python SDK for creating, writing, and reading onchain tables"
 authors = ["Dan Buchholz <dbuchholz30@gmail.com>"]
 license = "MIT AND Apache-2.0"
 readme = "README.md"
+include = ["tableland/abi.json"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 web3 = "^6.16.0"
 requests = "^2.31.0"
 sqlglot = "^23.6.3"
```

### Comparing `tableland-0.0.1rc1/tableland/__init__.py` & `tableland-0.0.1rc2/tableland/__init__.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc1/tableland/database.py` & `tableland-0.0.1rc2/tableland/database.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc1/tableland/helpers.py` & `tableland-0.0.1rc2/tableland/helpers.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc1/tableland/types.py` & `tableland-0.0.1rc2/tableland/types.py`

 * *Files identical despite different names*

### Comparing `tableland-0.0.1rc1/PKG-INFO` & `tableland-0.0.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableland
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A minimal Tableland Python SDK for creating, writing, and reading onchain tables
 License: MIT AND Apache-2.0
 Author: Dan Buchholz
 Author-email: dbuchholz30@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

