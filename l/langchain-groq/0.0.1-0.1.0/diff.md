# Comparing `tmp/langchain_groq-0.0.1.tar.gz` & `tmp/langchain_groq-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_groq-0.0.1.tar", max compression
+gzip compressed data, was "langchain_groq-0.1.0.tar", max compression
```

## Comparing `langchain_groq-0.0.1.tar` & `langchain_groq-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-02-22 15:52:13.572358 langchain_groq-0.0.1/LICENSE
--rw-r--r--   0        0        0     1986 2024-02-22 15:52:13.572946 langchain_groq-0.0.1/README.md
--rw-r--r--   0        0        0       72 2024-02-22 15:52:13.573134 langchain_groq-0.0.1/langchain_groq/__init__.py
--rw-r--r--   0        0        0    19099 2024-02-22 15:52:13.573417 langchain_groq-0.0.1/langchain_groq/chat_models.py
--rw-r--r--   0        0        0        0 2024-02-22 15:52:13.573698 langchain_groq-0.0.1/langchain_groq/py.typed
--rw-r--r--   0        0        0     2456 2024-02-22 15:52:13.574343 langchain_groq-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2788 1970-01-01 00:00:00.000000 langchain_groq-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1986 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/README.md
+-rw-r--r--   0        0        0       72 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/langchain_groq/__init__.py
+-rw-r--r--   0        0        0    38440 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/langchain_groq/chat_models.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:23:27.635170 langchain_groq-0.1.0/langchain_groq/py.typed
+-rw-r--r--   0        0        0     2544 2024-04-03 22:23:27.639171 langchain_groq-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2793 1970-01-01 00:00:00.000000 langchain_groq-0.1.0/PKG-INFO
```

### Comparing `langchain_groq-0.0.1/LICENSE` & `langchain_groq-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.0.1/README.md` & `langchain_groq-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_groq-0.0.1/pyproject.toml` & `langchain_groq-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "langchain-groq"
-version = "0.0.1"
+version = "0.1.0"
 description = "An integration package connecting Groq and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/groq"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1"
+langchain-core = "^0.1.40"
 groq = ">=0.4.1,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
-pytest-mock  = "^3.10.0"
+pytest-mock = "^3.10.0"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -35,43 +35,41 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 
 [tool.ruff]
 select = [
-  "E",  # pycodestyle
-  "F",  # pyflakes
-  "I",  # isort
-  "W",  # Warnings
+  "E", # pycodestyle
+  "F", # pyflakes
+  "I", # isort
+  "W", # Warnings
 ]
 
 [tool.mypy]
 disallow_untyped_defs = "True"
 
 [tool.coverage.run]
-omit = [
-    "tests/*",
-]
+omit = ["tests/*"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 # --strict-markers will raise errors on unknown marks.
@@ -85,11 +83,13 @@
 # https://docs.pytest.org/en/7.1.x/example/markers.html#registering-markers
 markers = [
   "compile: mark placeholder test used to compile integration tests without running them",
   "scheduled: mark tests to run in scheduled testing",
 ]
 filterwarnings = [
   "error",
+  'ignore::ResourceWarning:',
+  'ignore:The function `with_structured_output` is in beta',
   # Maintain support for pydantic 1.X
-  'default:The `dict` method is deprecated; use `model_dump` instead.*:DeprecationWarning',
+  'default:The `dict` method is deprecated; use `model_dump` instead:DeprecationWarning',
 ]
 asyncio_mode = "auto"
```

### Comparing `langchain_groq-0.0.1/PKG-INFO` & `langchain_groq-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-groq
-Version: 0.0.1
+Version: 0.1.0
 Summary: An integration package connecting Groq and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: groq (>=0.4.1,<1)
-Requires-Dist: langchain-core (>=0.1,<0.2)
+Requires-Dist: langchain-core (>=0.1.40,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/groq
 Description-Content-Type: text/markdown
 
 # langchain-groq
 
 ## Welcome to Groq! 🚀
```

