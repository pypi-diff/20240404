# Comparing `tmp/pyquocca-0.0.8.tar.gz` & `tmp/pyquocca-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquocca-0.0.8.tar", max compression
+gzip compressed data, was "pyquocca-0.0.9.tar", max compression
```

## Comparing `pyquocca-0.0.8.tar` & `pyquocca-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      170 2024-04-04 09:49:58.865306 pyquocca-0.0.8/README.md
--rw-r--r--   0        0        0      538 2024-04-04 10:19:29.173944 pyquocca-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      185 2024-04-04 09:24:01.403598 pyquocca-0.0.8/src/pyquocca/__init__.py
--rw-r--r--   0        0        0     1406 2024-04-04 09:16:57.462393 pyquocca-0.0.8/src/pyquocca/flags.py
--rw-r--r--   0        0        0     1944 2024-04-04 09:26:15.720158 pyquocca-0.0.8/src/pyquocca/gunicorn.py
--rw-r--r--   0        0        0     2470 2024-04-04 09:22:51.096293 pyquocca-0.0.8/src/pyquocca/header_utils.py
--rw-r--r--   0        0        0     2738 2024-04-04 09:43:36.455874 pyquocca-0.0.8/src/pyquocca/xssbot.py
--rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 pyquocca-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      170 2024-04-04 09:49:58.865306 pyquocca-0.0.9/README.md
+-rw-r--r--   0        0        0      538 2024-04-04 10:26:19.106818 pyquocca-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-04 09:24:01.403598 pyquocca-0.0.9/src/pyquocca/__init__.py
+-rw-r--r--   0        0        0     1406 2024-04-04 09:16:57.462393 pyquocca-0.0.9/src/pyquocca/flags.py
+-rw-r--r--   0        0        0     1944 2024-04-04 09:26:15.720158 pyquocca-0.0.9/src/pyquocca/gunicorn.py
+-rw-r--r--   0        0        0     2470 2024-04-04 09:22:51.096293 pyquocca-0.0.9/src/pyquocca/header_utils.py
+-rw-r--r--   0        0        0     2738 2024-04-04 09:43:36.455874 pyquocca-0.0.9/src/pyquocca/xssbot.py
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 pyquocca-0.0.9/PKG-INFO
```

### Comparing `pyquocca-0.0.8/pyproject.toml` & `pyquocca-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "pyquocca"
-version = "0.0.8"
+version = "0.0.9"
 description = "Challenge utilities for SecEDU CTFs (primarily UNSW's COMP6[48]43)."
 authors = ["HamishWHC <20359560+HamishWHC@users.noreply.github.com>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-flask = ">= 2.1.2, < 4"
+flask = ">= 2.0.3, < 4"
 requests = "^2.31.0"
 gunicorn = "^21.2.0"
 python-json-logger = "^2.0.7"
 typing-extensions = "^4.10.0"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `pyquocca-0.0.8/src/pyquocca/flags.py` & `pyquocca-0.0.9/src/pyquocca/flags.py`

 * *Files identical despite different names*

### Comparing `pyquocca-0.0.8/src/pyquocca/gunicorn.py` & `pyquocca-0.0.9/src/pyquocca/gunicorn.py`

 * *Files identical despite different names*

### Comparing `pyquocca-0.0.8/src/pyquocca/header_utils.py` & `pyquocca-0.0.9/src/pyquocca/header_utils.py`

 * *Files identical despite different names*

### Comparing `pyquocca-0.0.8/src/pyquocca/xssbot.py` & `pyquocca-0.0.9/src/pyquocca/xssbot.py`

 * *Files identical despite different names*

### Comparing `pyquocca-0.0.8/PKG-INFO` & `pyquocca-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pyquocca
-Version: 0.0.8
+Version: 0.0.9
 Summary: Challenge utilities for SecEDU CTFs (primarily UNSW's COMP6[48]43).
 Author: HamishWHC
 Author-email: 20359560+HamishWHC@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: flask (>=2.1.2,<4)
+Requires-Dist: flask (>=2.0.3,<4)
 Requires-Dist: gunicorn (>=21.2.0,<22.0.0)
 Requires-Dist: python-json-logger (>=2.0.7,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # QuoccaBank Standard Library
```

