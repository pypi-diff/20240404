# Comparing `tmp/jara_utils-1.2.0.tar.gz` & `tmp/jara_utils-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jara_utils-1.2.0.tar", max compression
+gzip compressed data, was "jara_utils-1.2.1.tar", max compression
```

## Comparing `jara_utils-1.2.0.tar` & `jara_utils-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1544 2024-02-20 15:54:40.171715 jara_utils-1.2.0/README_pypi.rst
--rw-r--r--   0        0        0        0 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/__init__.py
--rw-r--r--   0        0        0     1945 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/cli_output.py
--rw-r--r--   0        0        0      293 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/constants.py
--rw-r--r--   0        0        0     1367 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/decorators.py
--rw-r--r--   0        0        0      707 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/dotenv_configs.py
--rw-r--r--   0        0        0     1337 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/environment.py
--rw-r--r--   0        0        0      531 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/exceptions.py
--rw-r--r--   0        0        0      498 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/normalization/__init__.py
--rw-r--r--   0        0        0     1302 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/normalization/boolean.py
--rw-r--r--   0        0        0      671 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/normalization/datetime.py
--rw-r--r--   0        0        0      444 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/normalization/integer.py
--rw-r--r--   0        0        0      786 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/normalization/iterable.py
--rw-r--r--   0        0        0      613 2024-02-20 15:54:40.171715 jara_utils-1.2.0/jara_utils/normalization/string.py
--rw-r--r--   0        0        0     2555 2024-02-20 15:54:40.171715 jara_utils-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 jara_utils-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1544 2024-04-04 15:33:25.923939 jara_utils-1.2.1/README_pypi.rst
+-rw-r--r--   0        0        0        0 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/__init__.py
+-rw-r--r--   0        0        0     1945 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/cli_output.py
+-rw-r--r--   0        0        0      293 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/constants.py
+-rw-r--r--   0        0        0     1367 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/decorators.py
+-rw-r--r--   0        0        0      707 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/dotenv_configs.py
+-rw-r--r--   0        0        0     1337 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/environment.py
+-rw-r--r--   0        0        0      531 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/exceptions.py
+-rw-r--r--   0        0        0      498 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/normalization/__init__.py
+-rw-r--r--   0        0        0     1302 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/normalization/boolean.py
+-rw-r--r--   0        0        0      671 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/normalization/datetime.py
+-rw-r--r--   0        0        0      444 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/normalization/integer.py
+-rw-r--r--   0        0        0      786 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/normalization/iterable.py
+-rw-r--r--   0        0        0      613 2024-04-04 15:33:25.923939 jara_utils-1.2.1/jara_utils/normalization/string.py
+-rw-r--r--   0        0        0     2608 2024-04-04 15:33:25.927939 jara_utils-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 jara_utils-1.2.1/PKG-INFO
```

### Comparing `jara_utils-1.2.0/README_pypi.rst` & `jara_utils-1.2.1/README_pypi.rst`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/cli_output.py` & `jara_utils-1.2.1/jara_utils/cli_output.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/decorators.py` & `jara_utils-1.2.1/jara_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/dotenv_configs.py` & `jara_utils-1.2.1/jara_utils/dotenv_configs.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/environment.py` & `jara_utils-1.2.1/jara_utils/environment.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/exceptions.py` & `jara_utils-1.2.1/jara_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/normalization/boolean.py` & `jara_utils-1.2.1/jara_utils/normalization/boolean.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/normalization/datetime.py` & `jara_utils-1.2.1/jara_utils/normalization/datetime.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/normalization/iterable.py` & `jara_utils-1.2.1/jara_utils/normalization/iterable.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/jara_utils/normalization/string.py` & `jara_utils-1.2.1/jara_utils/normalization/string.py`

 * *Files identical despite different names*

### Comparing `jara_utils-1.2.0/pyproject.toml` & `jara_utils-1.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jara-utils"
-version = "1.2.0"
+version = "1.2.1"
 description = "A package with basic stuff."
 authors = ["Serban Senciuc <senciuc.serban@gmail.com>"]
 readme = "README_pypi.rst"
 repository = "https://github.com/senciucserban/jara-utils"
 classifiers = [
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -22,59 +22,61 @@
 
 [tool.poetry.extras]
 dotenv = ["python-dotenv"]
 all = ["python-dotenv"]
 
 
 [tool.poetry.group.test.dependencies]
-faker = ">=16.4,<24.0"
+faker = ">=16.4,<25.0"
 pytest = ">=7.2.1,<9.0.0"
 pytest-cov = "^4.0.0"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = ">=0.20.3,<0.24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest-sugar = ">=0.9.6,<1.1.0"
 pytest-deadfixtures = "^2.2.1"
 ipython = "^8.8.0"
 ipdb = "^0.13.11"
 
 [tool.poetry.group.lint.dependencies]
-mypy = ">=0.991,<1.9"
+mypy = ">=0.991,<1.10"
 bandit = "^1.7.4"
-ruff = "^0.0.284"
+ruff = ">=0.0.284,<0.3.5"
 black = ">=23.7,<25.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # -------------------- ruff --------------------
 [tool.ruff]
 src = ["src", "test"]
-format = "grouped"
+output-format = "grouped"
+line-length = 120
+target-version = "py311"
+
+[tool.ruff.lint]
 select = ["ALL"]
 ignore = ["D", "S", "DTZ", "FBT", "ANN101", "ANN102", "ANN401", "ANN002", "ANN003"]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 per-file-ignores = {}
-line-length = 120
-target-version = "py311"
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 inline-quotes = "single"
 multiline-quotes = "single"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 combine-as-imports = true
 known-first-party = ["src"]
 
 # -------------------- black --------------------
 [tool.black]
 line-length = 120
 skip-string-normalization = true
```

### Comparing `jara_utils-1.2.0/PKG-INFO` & `jara_utils-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jara-utils
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package with basic stuff.
 Home-page: https://github.com/senciucserban/jara-utils
 Author: Serban Senciuc
 Author-email: senciuc.serban@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

