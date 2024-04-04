# Comparing `tmp/pygqlc-3.1.4.tar.gz` & `tmp/pygqlc-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygqlc-3.1.4.tar", max compression
+gzip compressed data, was "pygqlc-3.2.0.tar", max compression
```

## Comparing `pygqlc-3.1.4.tar` & `pygqlc-3.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     5367 2023-08-16 22:16:59.121902 pygqlc-3.1.4/README.md
--rw-r--r--   0        0        0    25872 2023-04-21 18:46:19.761900 pygqlc-3.1.4/pygqlc/GraphQLClient.py
--rw-r--r--   0        0        0     4941 2021-12-22 16:29:04.043942 pygqlc-3.1.4/pygqlc/MutationBatch.py
--rw-r--r--   0        0        0     2795 2021-12-22 16:29:04.044073 pygqlc-3.1.4/pygqlc/MutationParser.py
--rw-r--r--   0        0        0        0 2021-12-22 16:29:04.044124 pygqlc-3.1.4/pygqlc/QueryBatch.py
--rw-r--r--   0        0        0      761 2021-12-22 16:29:04.044246 pygqlc-3.1.4/pygqlc/QueryParser.py
--rw-r--r--   0        0        0      124 2021-12-22 16:29:04.044355 pygqlc-3.1.4/pygqlc/SubscriptionParser.py
--rw-r--r--   0        0        0      293 2023-08-16 22:16:59.124384 pygqlc-3.1.4/pygqlc/__init__.py
--rw-r--r--   0        0        0      338 2021-12-22 16:29:04.044601 pygqlc-3.1.4/pygqlc/__main__.py
--rw-r--r--   0        0        0       21 2023-08-16 22:28:54.638529 pygqlc-3.1.4/pygqlc/__version__.py
--rw-r--r--   0        0        0      362 2021-12-22 16:29:04.044775 pygqlc-3.1.4/pygqlc/helper_modules/Singleton.py
--rw-r--r--   0        0        0        0 2021-12-22 16:29:04.044829 pygqlc-3.1.4/pygqlc/helper_modules/__init__.py
--rw-r--r--   0        0        0      836 2023-08-16 22:28:54.631668 pygqlc-3.1.4/pyproject.toml
--rw-r--r--   0        0        0     5990 1970-01-01 00:00:00.000000 pygqlc-3.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5367 2023-08-16 22:16:59.121902 pygqlc-3.2.0/README.md
+-rw-r--r--   0        0        0    25872 2023-04-21 18:46:19.761900 pygqlc-3.2.0/pygqlc/GraphQLClient.py
+-rw-r--r--   0        0        0     4941 2021-12-22 16:29:04.043942 pygqlc-3.2.0/pygqlc/MutationBatch.py
+-rw-r--r--   0        0        0     2795 2021-12-22 16:29:04.044073 pygqlc-3.2.0/pygqlc/MutationParser.py
+-rw-r--r--   0        0        0        0 2021-12-22 16:29:04.044124 pygqlc-3.2.0/pygqlc/QueryBatch.py
+-rw-r--r--   0        0        0      761 2021-12-22 16:29:04.044246 pygqlc-3.2.0/pygqlc/QueryParser.py
+-rw-r--r--   0        0        0      124 2021-12-22 16:29:04.044355 pygqlc-3.2.0/pygqlc/SubscriptionParser.py
+-rw-r--r--   0        0        0      293 2023-08-16 22:16:59.124384 pygqlc-3.2.0/pygqlc/__init__.py
+-rw-r--r--   0        0        0      338 2021-12-22 16:29:04.044601 pygqlc-3.2.0/pygqlc/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-04 15:24:13.727825 pygqlc-3.2.0/pygqlc/__version__.py
+-rw-r--r--   0        0        0      362 2021-12-22 16:29:04.044775 pygqlc-3.2.0/pygqlc/helper_modules/Singleton.py
+-rw-r--r--   0        0        0        0 2021-12-22 16:29:04.044829 pygqlc-3.2.0/pygqlc/helper_modules/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-04 15:24:13.728102 pygqlc-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5982 1970-01-01 00:00:00.000000 pygqlc-3.2.0/PKG-INFO
```

### Comparing `pygqlc-3.1.4/README.md` & `pygqlc-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pygqlc-3.1.4/pygqlc/GraphQLClient.py` & `pygqlc-3.2.0/pygqlc/GraphQLClient.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.1.4/pygqlc/MutationBatch.py` & `pygqlc-3.2.0/pygqlc/MutationBatch.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.1.4/pygqlc/MutationParser.py` & `pygqlc-3.2.0/pygqlc/MutationParser.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.1.4/pygqlc/QueryParser.py` & `pygqlc-3.2.0/pygqlc/QueryParser.py`

 * *Files identical despite different names*

### Comparing `pygqlc-3.1.4/pyproject.toml` & `pygqlc-3.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 [tool.poetry]
 name = "pygqlc"
-version = "3.1.4"
+version = "3.2.0"
 description = "Python client for graphql APIs"
 authors = ["Baruc Almaguer <baruc.almaguer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "~=2.26"
-pydash = "~=5.0"
-tenacity = "~=6.3"
-websocket-client = "==0.54.0"
-certifi = "^2023.07.22"
+pydash = "~=7.0"
+tenacity = "~=8.0"
+websocket-client = "^1.0"
+certifi = "^2024"
 
 
 [tool.poetry.group.dev.dependencies]
-pipenv-poetry-migrate = "^0.3.2"
 pytest = "*"
 pylint = "*"
 autopep8 = "*"
 setuptools = "*"
 wheel = "*"
 twine = "*"
 pytest-cov = "*"
 sphinx = "3.1"
 sphinx-rtd-theme = "==0.5.0"
 
-
-[[tool.poetry.source]]
-name = "valiot"
-url = "https://pypi.valiot.io/"
-priority = "primary"
-
-
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pygqlc-3.1.4/PKG-INFO` & `pygqlc-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pygqlc
-Version: 3.1.4
+Version: 3.2.0
 Summary: Python client for graphql APIs
 Author: Baruc Almaguer
 Author-email: baruc.almaguer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: certifi (>=2023.07.22,<2024.0.0)
-Requires-Dist: pydash (>=5.0,<6.0)
+Requires-Dist: certifi (>=2024,<2025)
+Requires-Dist: pydash (>=7.0,<8.0)
 Requires-Dist: requests (>=2.26,<3.0)
-Requires-Dist: tenacity (>=6.3,<7.0)
-Requires-Dist: websocket-client (==0.54.0)
+Requires-Dist: tenacity (>=8.0,<9.0)
+Requires-Dist: websocket-client (>=1.0,<2.0)
 Description-Content-Type: text/markdown
 
 # pygqlc
 
 Python client for graphql APIs
 
 ### Scope
```

