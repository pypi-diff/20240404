# Comparing `tmp/cg_pytest_reporter-2024.1.16.1248.tar.gz` & `tmp/cg_pytest_reporter-2024.2.26.1340.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cg_pytest_reporter-2024.1.16.1248.tar", max compression
+gzip compressed data, was "cg_pytest_reporter-2024.2.26.1340.tar", max compression
```

## Comparing `cg_pytest_reporter-2024.1.16.1248.tar` & `cg_pytest_reporter-2024.2.26.1340.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6290 2024-01-16 12:47:47.126261 cg_pytest_reporter-2024.1.16.1248/README.md
--rw-r--r--   0        0        0      605 2024-01-16 12:47:47.126261 cg_pytest_reporter-2024.1.16.1248/cg_pytest_reporter/__init__.py
--rw-r--r--   0        0        0    15521 2024-01-16 12:47:47.126261 cg_pytest_reporter-2024.1.16.1248/cg_pytest_reporter/plugin.py
--rw-r--r--   0        0        0     1859 2024-01-16 12:48:08.762079 cg_pytest_reporter-2024.1.16.1248/pyproject.toml
--rw-r--r--   0        0        0     6889 1970-01-01 00:00:00.000000 cg_pytest_reporter-2024.1.16.1248/PKG-INFO
+-rw-r--r--   0        0        0     6290 2024-02-26 13:40:04.654529 cg_pytest_reporter-2024.2.26.1340/README.md
+-rw-r--r--   0        0        0      605 2024-02-26 13:40:04.654529 cg_pytest_reporter-2024.2.26.1340/cg_pytest_reporter/__init__.py
+-rw-r--r--   0        0        0    15521 2024-02-26 13:40:04.658530 cg_pytest_reporter-2024.2.26.1340/cg_pytest_reporter/plugin.py
+-rw-r--r--   0        0        0     1859 2024-02-26 13:40:21.862798 cg_pytest_reporter-2024.2.26.1340/pyproject.toml
+-rw-r--r--   0        0        0     6889 1970-01-01 00:00:00.000000 cg_pytest_reporter-2024.2.26.1340/PKG-INFO
```

### Comparing `cg_pytest_reporter-2024.1.16.1248/README.md` & `cg_pytest_reporter-2024.2.26.1340/README.md`

 * *Files identical despite different names*

### Comparing `cg_pytest_reporter-2024.1.16.1248/cg_pytest_reporter/__init__.py` & `cg_pytest_reporter-2024.2.26.1340/cg_pytest_reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `cg_pytest_reporter-2024.1.16.1248/cg_pytest_reporter/plugin.py` & `cg_pytest_reporter-2024.2.26.1340/cg_pytest_reporter/plugin.py`

 * *Files identical despite different names*

### Comparing `cg_pytest_reporter-2024.1.16.1248/pyproject.toml` & `cg_pytest_reporter-2024.2.26.1340/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cg-pytest-reporter"
-version = "2024.01.16.1248"
+version = "2024.02.26.1340"
 description = ""
 authors = ["CodeGrade <info@codegrade.com>"]
 readme = "README.md"
 packages = [{ include = "cg_pytest_reporter" }]
 license = "MIT"
 
 [tool.poetry.plugins.pytest11]
@@ -13,15 +13,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pytest = ">=7.0.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 pylint = "^2.17.4"
-yapf = "^0.33.0"
+yapf = "^0.40.0"
 isort = "^5.12.0"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cg_pytest_reporter-2024.1.16.1248/PKG-INFO` & `cg_pytest_reporter-2024.2.26.1340/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cg-pytest-reporter
-Version: 2024.1.16.1248
+Version: 2024.2.26.1340
 Summary: 
 License: MIT
 Author: CodeGrade
 Author-email: info@codegrade.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

