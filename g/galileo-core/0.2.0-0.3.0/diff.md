# Comparing `tmp/galileo_core-0.2.0.tar.gz` & `tmp/galileo_core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_core-0.2.0.tar", max compression
+gzip compressed data, was "galileo_core-0.3.0.tar", max compression
```

## Comparing `galileo_core-0.2.0.tar` & `galileo_core-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    10946 2024-03-28 18:27:37.711179 galileo_core-0.2.0/LICENSE
--rw-r--r--   0        0        0       80 2024-03-28 18:27:37.711179 galileo_core-0.2.0/README.md
--rw-r--r--   0        0        0     2270 2024-03-28 18:27:38.707181 galileo_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-28 18:27:38.707181 galileo_core-0.2.0/src/galileo_core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/constants/__init__.py
--rw-r--r--   0        0        0      573 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/constants/http_headers.py
--rw-r--r--   0        0        0      362 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/constants/routes.py
--rw-r--r--   0        0        0        0 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/helpers/__init__.py
--rw-r--r--   0        0        0     1543 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/helpers/api_client.py
--rw-r--r--   0        0        0     5271 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/helpers/config.py
--rw-r--r--   0        0        0       60 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/helpers/logger.py
--rw-r--r--   0        0        0        0 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/schemas/protect/__init__.py
--rw-r--r--   0        0        0      849 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/schemas/protect/action.py
--rw-r--r--   0        0        0      557 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/schemas/protect/rule.py
--rw-r--r--   0        0        0     1034 2024-03-28 18:27:37.715179 galileo_core-0.2.0/src/galileo_core/schemas/protect/ruleset.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-03 23:51:05.020440 galileo_core-0.3.0/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-03 23:51:05.020440 galileo_core-0.3.0/README.md
+-rw-r--r--   0        0        0     2270 2024-04-03 23:51:06.044449 galileo_core-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-03 23:51:06.044449 galileo_core-0.3.0/src/galileo_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/constants/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/constants/http_headers.py
+-rw-r--r--   0        0        0      362 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/helpers/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/helpers/api_client.py
+-rw-r--r--   0        0        0     5322 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/helpers/config.py
+-rw-r--r--   0        0        0       60 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/helpers/logger.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/action.py
+-rw-r--r--   0        0        0      557 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/rule.py
+-rw-r--r--   0        0        0     1034 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/ruleset.py
+-rw-r--r--   0        0        0     1124 2024-04-03 23:51:05.020440 galileo_core-0.3.0/src/galileo_core/schemas/protect/stage.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.3.0/PKG-INFO
```

### Comparing `galileo_core-0.2.0/LICENSE` & `galileo_core-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_core-0.2.0/pyproject.toml` & `galileo_core-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-core"
-version = "0.2.0"
+version = "0.3.0"
 description = "Shared schemas and configuration for Galileo's Python packages."
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_core", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
```

### Comparing `galileo_core-0.2.0/src/galileo_core/constants/http_headers.py` & `galileo_core-0.3.0/src/galileo_core/constants/http_headers.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.2.0/src/galileo_core/helpers/api_client.py` & `galileo_core-0.3.0/src/galileo_core/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.2.0/src/galileo_core/helpers/config.py` & `galileo_core-0.3.0/src/galileo_core/helpers/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,16 +130,19 @@
     @property
     def api_client(self) -> ApiClient:
         self.refresh_jwt_token()
         if not self.jwt_token:
             raise ValueError("No token set. Please log in.")
         return ApiClient(host=self.api_url, jwt_token=self.jwt_token)
 
-    def logout(self) -> None:
+    def reset(self) -> None:
         # Reset credentials.
         self.username = None
         self.password = None
         self.api_key = None
         self.jwt_token = None
         self.current_user = None
+
+    def logout(self) -> None:
+        self.reset()
         self.write()
         print(f"👋 You have logged out of 🔭 Galileo ({self.console_url}).")
```

### Comparing `galileo_core-0.2.0/src/galileo_core/schemas/protect/action.py` & `galileo_core-0.3.0/src/galileo_core/schemas/protect/action.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.2.0/src/galileo_core/schemas/protect/rule.py` & `galileo_core-0.3.0/src/galileo_core/schemas/protect/rule.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.2.0/src/galileo_core/schemas/protect/ruleset.py` & `galileo_core-0.3.0/src/galileo_core/schemas/protect/ruleset.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.2.0/PKG-INFO` & `galileo_core-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galileo-core
-Version: 0.2.0
+Version: 0.3.0
 Summary: Shared schemas and configuration for Galileo's Python packages.
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

