# Comparing `tmp/langflow-1.0.0a6.tar.gz` & `tmp/langflow-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-1.0.0a6.tar", max compression
+gzip compressed data, was "langflow-1.0.0a7.tar", max compression
```

## Comparing `langflow-1.0.0a6.tar` & `langflow-1.0.0a7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2024-04-04 06:39:26.766430 langflow-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     6934 2024-04-04 06:39:26.766430 langflow-1.0.0a6/README.md
--rw-r--r--   0        0        0     3669 2024-04-04 06:39:55.522399 langflow-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-04 06:39:27.226429 langflow-1.0.0a6/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      156 2024-04-04 06:39:27.226429 langflow-1.0.0a6/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0    10097 1970-01-01 00:00:00.000000 langflow-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-04 14:14:04.746055 langflow-1.0.0a7/LICENSE
+-rw-r--r--   0        0        0     6934 2024-04-04 14:14:04.746055 langflow-1.0.0a7/README.md
+-rw-r--r--   0        0        0     3669 2024-04-04 14:14:31.541925 langflow-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-04 14:14:05.210055 langflow-1.0.0a7/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-04 14:14:05.210055 langflow-1.0.0a7/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0    10097 1970-01-01 00:00:00.000000 langflow-1.0.0a7/PKG-INFO
```

### Comparing `langflow-1.0.0a6/LICENSE` & `langflow-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a6/README.md` & `langflow-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a6/pyproject.toml` & `langflow-1.0.0a7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "1.0.0a6"
+version = "1.0.0a7"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Igor Carvalho <igorr.ackerman@gmail.com>",
```

### Comparing `langflow-1.0.0a6/PKG-INFO` & `langflow-1.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
```

