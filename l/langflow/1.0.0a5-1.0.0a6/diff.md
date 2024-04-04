# Comparing `tmp/langflow-1.0.0a5.tar.gz` & `tmp/langflow-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-1.0.0a5.tar", max compression
+gzip compressed data, was "langflow-1.0.0a6.tar", max compression
```

## Comparing `langflow-1.0.0a5.tar` & `langflow-1.0.0a6.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0     1065 2024-04-04 05:47:11.670544 langflow-1.0.0a5/LICENSE
--rw-r--r--   0        0        0     6934 2024-04-04 05:47:11.671417 langflow-1.0.0a5/README.md
--rw-r--r--   0        0        0     3669 2024-04-04 06:24:20.522524 langflow-1.0.0a5/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-04 05:47:12.068790 langflow-1.0.0a5/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      244 2024-04-04 05:52:19.875396 langflow-1.0.0a5/src/backend/langflow/version/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      449 2024-04-04 05:52:19.880207 langflow-1.0.0a5/src/backend/langflow/version/__pycache__/version.cpython-311.pyc
--rw-r--r--   0        0        0      156 2024-04-04 05:47:12.068865 langflow-1.0.0a5/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0    10097 1970-01-01 00:00:00.000000 langflow-1.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-04 06:39:26.766430 langflow-1.0.0a6/LICENSE
+-rw-r--r--   0        0        0     6934 2024-04-04 06:39:26.766430 langflow-1.0.0a6/README.md
+-rw-r--r--   0        0        0     3669 2024-04-04 06:39:55.522399 langflow-1.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-04 06:39:27.226429 langflow-1.0.0a6/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-04 06:39:27.226429 langflow-1.0.0a6/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0    10097 1970-01-01 00:00:00.000000 langflow-1.0.0a6/PKG-INFO
```

### Comparing `langflow-1.0.0a5/LICENSE` & `langflow-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a5/README.md` & `langflow-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a5/pyproject.toml` & `langflow-1.0.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "1.0.0a5"
+version = "1.0.0a6"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Igor Carvalho <igorr.ackerman@gmail.com>",
@@ -22,15 +22,15 @@
 
 [tool.poetry.scripts]
 langflow = "langflow.__main__:main"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-langflow-base = "^0.0.18"
+langflow-base = "^0.0.19"
 beautifulsoup4 = "^4.12.2"
 google-search-results = "^2.4.1"
 google-api-python-client = "^2.118.0"
 huggingface-hub = { version = "^0.20.0", extras = ["inference"] }
 llama-cpp-python = { version = "~0.2.0", optional = true }
 networkx = "^3.1"
 pysrt = "^1.1.2"
```

### Comparing `langflow-1.0.0a5/PKG-INFO` & `langflow-1.0.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
@@ -33,15 +33,15 @@
 Requires-Dist: flower (>=2.0.0,<3.0.0) ; extra == "deploy"
 Requires-Dist: google-api-python-client (>=2.118.0,<3.0.0)
 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: huggingface-hub[inference] (>=0.20.0,<0.21.0)
 Requires-Dist: langchain-cohere (>=0.1.0rc1,<0.2.0)
 Requires-Dist: langchain-google-genai (>=1.0.1,<2.0.0)
-Requires-Dist: langflow-base (>=0.0.18,<0.0.19)
+Requires-Dist: langflow-base (>=0.0.19,<0.0.20)
 Requires-Dist: langfuse (>=2.9.0,<3.0.0)
 Requires-Dist: litellm (>=1.34.22,<2.0.0)
 Requires-Dist: llama-cpp-python (>=0.2.0,<0.3.0) ; extra == "local"
 Requires-Dist: llama-index (>=0.10.13,<0.11.0)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
 Requires-Dist: metal-sdk (>=2.5.0,<3.0.0)
 Requires-Dist: metaphor-python (>=0.1.11,<0.2.0)
```

