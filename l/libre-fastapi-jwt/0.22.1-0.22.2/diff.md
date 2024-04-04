# Comparing `tmp/libre_fastapi_jwt-0.22.1.tar.gz` & `tmp/libre_fastapi_jwt-0.22.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libre_fastapi_jwt-0.22.1.tar", max compression
+gzip compressed data, was "libre_fastapi_jwt-0.22.2.tar", max compression
```

## Comparing `libre_fastapi_jwt-0.22.1.tar` & `libre_fastapi_jwt-0.22.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-04 06:18:08.402983 libre_fastapi_jwt-0.22.1/LICENSE
--rw-r--r--   0        0        0     2079 2024-04-04 06:18:08.406983 libre_fastapi_jwt-0.22.1/README.md
--rw-r--r--   0        0        0      148 2024-04-04 06:18:08.410983 libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/__init__.py
--rw-r--r--   0        0        0     5413 2024-04-04 06:18:08.410983 libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/auth_config.py
--rw-r--r--   0        0        0    45258 2024-04-04 06:18:08.410983 libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/auth_jwt.py
--rw-r--r--   0        0        0     5124 2024-04-04 06:18:08.410983 libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/config.py
--rw-r--r--   0        0        0     3059 2024-04-04 06:18:08.410983 libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/exceptions.py
--rw-r--r--   0        0        0     1083 2024-04-04 06:18:08.410983 libre_fastapi_jwt-0.22.1/pyproject.toml
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.22.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-04 08:09:29.402369 libre_fastapi_jwt-0.22.2/LICENSE
+-rw-r--r--   0        0        0     2079 2024-04-04 08:09:29.402369 libre_fastapi_jwt-0.22.2/README.md
+-rw-r--r--   0        0        0      163 2024-04-04 08:09:29.406369 libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/__init__.py
+-rw-r--r--   0        0        0     5413 2024-04-04 08:09:29.406369 libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/auth_config.py
+-rw-r--r--   0        0        0    45258 2024-04-04 08:09:29.406369 libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/auth_jwt.py
+-rw-r--r--   0        0        0     5124 2024-04-04 08:09:29.406369 libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/config.py
+-rw-r--r--   0        0        0     3059 2024-04-04 08:09:29.406369 libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/exceptions.py
+-rw-r--r--   0        0        0     1083 2024-04-04 08:09:29.406369 libre_fastapi_jwt-0.22.2/pyproject.toml
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.22.2/PKG-INFO
```

### Comparing `libre_fastapi_jwt-0.22.1/LICENSE` & `libre_fastapi_jwt-0.22.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.22.1/README.md` & `libre_fastapi_jwt-0.22.2/README.md`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/auth_config.py` & `libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/auth_config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/auth_jwt.py` & `libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/config.py` & `libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.22.1/libre_fastapi_jwt/exceptions.py` & `libre_fastapi_jwt-0.22.2/libre_fastapi_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.22.1/pyproject.toml` & `libre_fastapi_jwt-0.22.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "libre-fastapi-jwt"
-version = "0.22.1"
+version = "0.22.2"
 description = "Yet another fork of fast-jwt-auth"
 authors = ["Libre NZ <github-support@libre.nz>"]
 license = "MIT"
 repository = "https://github.com/LibreNZ/libre-fastapi-jwt"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
```

### Comparing `libre_fastapi_jwt-0.22.1/PKG-INFO` & `libre_fastapi_jwt-0.22.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libre-fastapi-jwt
-Version: 0.22.1
+Version: 0.22.2
 Summary: Yet another fork of fast-jwt-auth
 Home-page: https://github.com/LibreNZ/libre-fastapi-jwt
 License: MIT
 Author: Libre NZ
 Author-email: github-support@libre.nz
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.22.1 Summary: Yet
+Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.22.2 Summary: Yet
 another fork of fast-jwt-auth Home-page: https://github.com/LibreNZ/libre-
 fastapi-jwt License: MIT Author: Libre NZ Author-email: github-support@libre.nz
 Requires-Python: >=3.9,<4.0 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

