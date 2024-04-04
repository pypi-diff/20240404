# Comparing `tmp/whylogs_container_types-0.4.13.tar.gz` & `tmp/whylogs_container_types-0.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs_container_types-0.4.13.tar", max compression
+gzip compressed data, was "whylogs_container_types-0.4.14.tar", max compression
```

## Comparing `whylogs_container_types-0.4.13.tar` & `whylogs_container_types-0.4.14.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      104 2023-11-29 03:51:56.422148 whylogs_container_types-0.4.13/README.md
--rw-r--r--   0        0        0     1232 2024-03-26 22:37:38.642643 whylogs_container_types-0.4.13/pyproject.toml
--rw-r--r--   0        0        0     1287 2024-02-06 21:14:40.603869 whylogs_container_types-0.4.13/whylogs_container_types/__init__.py
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 whylogs_container_types-0.4.13/PKG-INFO
+-rw-r--r--   0        0        0      104 2023-11-29 03:51:56.422148 whylogs_container_types-0.4.14/README.md
+-rw-r--r--   0        0        0     1186 2024-04-04 17:16:34.302192 whylogs_container_types-0.4.14/pyproject.toml
+-rw-r--r--   0        0        0     1287 2024-04-04 17:16:23.730230 whylogs_container_types-0.4.14/whylogs_container_types/__init__.py
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 whylogs_container_types-0.4.14/PKG-INFO
```

### Comparing `whylogs_container_types-0.4.13/pyproject.toml` & `whylogs_container_types-0.4.14/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "whylogs-container-types"
-version = "0.4.13"
+version = "0.4.14"
 description = ""
 authors = ["Anthony Naddeo <anthony@whylabs.ai>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "whylogs_container_types/**/*.py" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 whylogs = "*"
-langkit = {version= "0.0.28.dev0", extras = ["all"], optional = true}
+langkit = "0.0.28.dev0"
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.337"
 ruff = "^0.1.13"
 
 [tool.poetry.extras]
```

### Comparing `whylogs_container_types-0.4.13/whylogs_container_types/__init__.py` & `whylogs_container_types-0.4.14/whylogs_container_types/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_types-0.4.13/PKG-INFO` & `whylogs_container_types-0.4.14/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: whylogs-container-types
-Version: 0.4.13
+Version: 0.4.14
 Summary: 
 License: MIT
 Author: Anthony Naddeo
 Author-email: anthony@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: llm
-Requires-Dist: langkit[all] (==0.0.28.dev0) ; extra == "llm"
+Requires-Dist: langkit (==0.0.28.dev0) ; extra == "llm"
 Requires-Dist: whylogs
 Description-Content-Type: text/markdown
 
 
 This packages contains various types that are used for customizing the whylogs python container. 
 
 TBD
```

