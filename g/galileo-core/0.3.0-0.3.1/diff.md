# Comparing `tmp/galileo_core-0.3.0.tar.gz` & `tmp/galileo_core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_core-0.3.0.tar", max compression
+gzip compressed data, was "galileo_core-0.3.1.tar", max compression
```

## Comparing `galileo_core-0.3.0.tar` & `galileo_core-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10946 2024-04-03 23:51:05.020440 galileo_core-0.3.0/LICENSE
--rw-r--r--   0        0        0       80 2024-04-03 23:51:05.020440 galileo_core-0.3.0/README.md
--rw-r--r--   0        0        0     2270 2024-04-03 23:51:06.044449 galileo_core-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-03 23:51:06.044449 galileo_core-0.3.0/src/galileo_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/constants/__init__.py
--rw-r--r--   0        0        0      573 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/constants/http_headers.py
--rw-r--r--   0        0        0      362 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/helpers/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/helpers/api_client.py
--rw-r--r--   0        0        0     5322 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/helpers/config.py
--rw-r--r--   0        0        0       60 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/helpers/logger.py
--rw-r--r--   0        0        0        0 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/__init__.py
--rw-r--r--   0        0        0      849 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/action.py
--rw-r--r--   0        0        0      557 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/rule.py
--rw-r--r--   0        0        0     1034 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/ruleset.py
--rw-r--r--   0        0        0     1124 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/stage.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-04 00:03:19.783371 galileo_core-0.3.1/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-04 00:03:19.783371 galileo_core-0.3.1/README.md
+-rw-r--r--   0        0        0     2323 2024-04-04 00:03:20.843375 galileo_core-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-04 00:03:20.843375 galileo_core-0.3.1/src/galileo_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/constants/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/constants/http_headers.py
+-rw-r--r--   0        0        0      362 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/helpers/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/helpers/api_client.py
+-rw-r--r--   0        0        0     5322 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/helpers/config.py
+-rw-r--r--   0        0        0       60 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/helpers/logger.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/schemas/protect/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/schemas/protect/action.py
+-rw-r--r--   0        0        0      557 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/schemas/protect/rule.py
+-rw-r--r--   0        0        0     1034 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/schemas/protect/ruleset.py
+-rw-r--r--   0        0        0     1124 2024-04-04 00:03:19.783371 galileo_core-0.3.1/src/galileo_core/schemas/protect/stage.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.3.1/PKG-INFO
```

### Comparing `galileo_core-0.3.0/LICENSE` & `galileo_core-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_core-0.3.0/pyproject.toml` & `galileo_core-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "galileo-core"
-version = "0.3.0"
+version = "0.3.1"
 description = "Shared schemas and configuration for Galileo's Python packages."
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_core", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
-pydantic = "^2.6.4"
+pydantic = "^2.6.0"
 pydantic-settings = "^2.2.1"
 requests = "^2.31.0"
 pyjwt = "^2.8.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
@@ -25,14 +25,15 @@
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 pre-commit = "^3.5.0"
 invoke = "^2.2.0"
 types-requests = "^2.31.0.20240311"
 types-jwt = "^0.1.3"
+pydantic = { extras = ["mypy"], version = "^2.6.0" }
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `galileo_core-0.3.0/src/galileo_core/constants/http_headers.py` & `galileo_core-0.3.1/src/galileo_core/constants/http_headers.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.3.0/src/galileo_core/helpers/api_client.py` & `galileo_core-0.3.1/src/galileo_core/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.3.0/src/galileo_core/helpers/config.py` & `galileo_core-0.3.1/src/galileo_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.3.0/src/galileo_core/schemas/protect/action.py` & `galileo_core-0.3.1/src/galileo_core/schemas/protect/action.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.3.0/src/galileo_core/schemas/protect/rule.py` & `galileo_core-0.3.1/src/galileo_core/schemas/protect/rule.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.3.0/src/galileo_core/schemas/protect/ruleset.py` & `galileo_core-0.3.1/src/galileo_core/schemas/protect/ruleset.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.3.0/src/galileo_core/schemas/protect/stage.py` & `galileo_core-0.3.1/src/galileo_core/schemas/protect/stage.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.3.0/PKG-INFO` & `galileo_core-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: galileo-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: Shared schemas and configuration for Galileo's Python packages.
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # galileo-core
```

