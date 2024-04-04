# Comparing `tmp/hyperon_das-0.7.2.tar.gz` & `tmp/hyperon_das-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das-0.7.2.tar", max compression
+gzip compressed data, was "hyperon_das-0.7.3.tar", max compression
```

## Comparing `hyperon_das-0.7.2.tar` & `hyperon_das-0.7.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2024-03-28 22:47:41.085997 hyperon_das-0.7.2/LICENCE
--rw-r--r--   0        0        0    12442 2024-03-28 22:47:41.085997 hyperon_das-0.7.2/README.md
--rw-r--r--   0        0        0      108 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/__init__.py
--rw-r--r--   0        0        0    20544 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/cache.py
--rw-r--r--   0        0        0     6621 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/client.py
--rw-r--r--   0        0        0      127 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/constants.py
--rw-r--r--   0        0        0    25387 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/das.py
--rw-r--r--   0        0        0     1830 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/decorators.py
--rw-r--r--   0        0        0     1012 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/exceptions.py
--rw-r--r--   0        0        0     1072 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/logger.py
--rw-r--r--   0        0        0       39 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/pattern_matcher/__init__.py
--rw-r--r--   0        0        0      274 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/pattern_matcher/constants.py
--rw-r--r--   0        0        0    31913 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/pattern_matcher/pattern_matcher.py
--rw-r--r--   0        0        0    21024 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/query_engines.py
--rw-r--r--   0        0        0     1685 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/traverse_engines.py
--rw-r--r--   0        0        0     5992 2024-03-28 22:47:41.129997 hyperon_das-0.7.2/hyperon_das/utils.py
--rw-r--r--   0        0        0     1315 2024-03-28 22:47:53.490058 hyperon_das-0.7.2/pyproject.toml
--rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-04 18:35:49.338260 hyperon_das-0.7.3/LICENCE
+-rw-r--r--   0        0        0    12442 2024-04-04 18:35:49.338260 hyperon_das-0.7.3/README.md
+-rw-r--r--   0        0        0      108 2024-04-04 18:35:49.378260 hyperon_das-0.7.3/hyperon_das/__init__.py
+-rw-r--r--   0        0        0    20544 2024-04-04 18:35:49.378260 hyperon_das-0.7.3/hyperon_das/cache.py
+-rw-r--r--   0        0        0     6621 2024-04-04 18:35:49.378260 hyperon_das-0.7.3/hyperon_das/client.py
+-rw-r--r--   0        0        0      127 2024-04-04 18:35:49.378260 hyperon_das-0.7.3/hyperon_das/constants.py
+-rw-r--r--   0        0        0    25387 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/das.py
+-rw-r--r--   0        0        0     1830 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/decorators.py
+-rw-r--r--   0        0        0     1012 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/exceptions.py
+-rw-r--r--   0        0        0     1072 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/logger.py
+-rw-r--r--   0        0        0       39 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/pattern_matcher/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/pattern_matcher/constants.py
+-rw-r--r--   0        0        0    31913 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/pattern_matcher/pattern_matcher.py
+-rw-r--r--   0        0        0    21024 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/query_engines.py
+-rw-r--r--   0        0        0     1685 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/traverse_engines.py
+-rw-r--r--   0        0        0     5992 2024-04-04 18:35:49.382260 hyperon_das-0.7.3/hyperon_das/utils.py
+-rw-r--r--   0        0        0     1315 2024-04-04 18:36:00.362313 hyperon_das-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0    13311 1970-01-01 00:00:00.000000 hyperon_das-0.7.3/PKG-INFO
```

### Comparing `hyperon_das-0.7.2/LICENCE` & `hyperon_das-0.7.3/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/README.md` & `hyperon_das-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/cache.py` & `hyperon_das-0.7.3/hyperon_das/cache.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/client.py` & `hyperon_das-0.7.3/hyperon_das/client.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/das.py` & `hyperon_das-0.7.3/hyperon_das/das.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/decorators.py` & `hyperon_das-0.7.3/hyperon_das/decorators.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/exceptions.py` & `hyperon_das-0.7.3/hyperon_das/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/logger.py` & `hyperon_das-0.7.3/hyperon_das/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/pattern_matcher/pattern_matcher.py` & `hyperon_das-0.7.3/hyperon_das/pattern_matcher/pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/query_engines.py` & `hyperon_das-0.7.3/hyperon_das/query_engines.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/traverse_engines.py` & `hyperon_das-0.7.3/hyperon_das/traverse_engines.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/hyperon_das/utils.py` & `hyperon_das-0.7.3/hyperon_das/utils.py`

 * *Files identical despite different names*

### Comparing `hyperon_das-0.7.2/pyproject.toml` & `hyperon_das-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyperon-das"
-version = "0.7.2"
+version = "0.7.3"
 description = "Query Engine API for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das"}]
 
 [tool.poetry.urls]
 "Documentation" = "https://singnet.github.io/das-query-engine"
 "Code" = "https://github.com/singnet/das-query-engine"
 "Bug Tracker" = "https://github.com/singnet/das-query-engine/issues"
 "Releases" = "https://github.com/singnet/das-query-engine/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8.5"
-hyperon-das-atomdb = "0.6.1"
+hyperon-das-atomdb = "0.6.2"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 black = "^23.9.1"
 pytest = "^7.4.2"
```

### Comparing `hyperon_das-0.7.2/PKG-INFO` & `hyperon_das-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: hyperon-das
-Version: 0.7.2
+Version: 0.7.3
 Summary: Query Engine API for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: hyperon-das-atomdb (==0.6.1)
+Requires-Dist: hyperon-das-atomdb (==0.6.2)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/singnet/das-query-engine/issues
 Project-URL: Code, https://github.com/singnet/das-query-engine
 Project-URL: Documentation, https://singnet.github.io/das-query-engine
 Project-URL: Releases, https://github.com/singnet/das-query-engine/releases
 Description-Content-Type: text/markdown
```

