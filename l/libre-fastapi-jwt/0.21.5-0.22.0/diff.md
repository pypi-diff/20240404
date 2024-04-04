# Comparing `tmp/libre_fastapi_jwt-0.21.5.tar.gz` & `tmp/libre_fastapi_jwt-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libre_fastapi_jwt-0.21.5.tar", max compression
+gzip compressed data, was "libre_fastapi_jwt-0.22.0.tar", max compression
```

## Comparing `libre_fastapi_jwt-0.21.5.tar` & `libre_fastapi_jwt-0.22.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-04 05:38:12.436142 libre_fastapi_jwt-0.21.5/LICENSE
--rw-r--r--   0        0        0     2079 2024-04-04 05:38:12.436142 libre_fastapi_jwt-0.21.5/README.md
--rw-r--r--   0        0        0      148 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/__init__.py
--rw-r--r--   0        0        0     5413 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/auth_config.py
--rw-r--r--   0        0        0    44689 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/auth_jwt.py
--rw-r--r--   0        0        0     5124 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/config.py
--rw-r--r--   0        0        0     3059 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/exceptions.py
--rw-r--r--   0        0        0     1083 2024-04-04 05:38:12.444142 libre_fastapi_jwt-0.21.5/pyproject.toml
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.21.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-04 06:13:46.403351 libre_fastapi_jwt-0.22.0/LICENSE
+-rw-r--r--   0        0        0     2079 2024-04-04 06:13:46.403351 libre_fastapi_jwt-0.22.0/README.md
+-rw-r--r--   0        0        0      148 2024-04-04 06:13:46.403351 libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/__init__.py
+-rw-r--r--   0        0        0     5413 2024-04-04 06:13:46.403351 libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/auth_config.py
+-rw-r--r--   0        0        0    45316 2024-04-04 06:13:46.407351 libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/auth_jwt.py
+-rw-r--r--   0        0        0     5124 2024-04-04 06:13:46.407351 libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/config.py
+-rw-r--r--   0        0        0     3059 2024-04-04 06:13:46.407351 libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/exceptions.py
+-rw-r--r--   0        0        0     1083 2024-04-04 06:13:46.407351 libre_fastapi_jwt-0.22.0/pyproject.toml
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.22.0/PKG-INFO
```

### Comparing `libre_fastapi_jwt-0.21.5/LICENSE` & `libre_fastapi_jwt-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.5/README.md` & `libre_fastapi_jwt-0.22.0/README.md`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/auth_config.py` & `libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/auth_config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/auth_jwt.py` & `libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/auth_jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-import jwt, re, hmac
+import hmac
+import re
 from uuid import uuid4
 from datetime import datetime, timedelta, timezone
 from typing import Dict, Optional, Sequence, Union
-from fastapi import Request, Response, WebSocket, Header, Security
-from fastapi.security import APIKeyCookie
+
+import jwt
+from fastapi import Request, Response, WebSocket, Header
+from fastapi.openapi.models import HTTPBearer as HTTPBearerModel
+from fastapi.security.http import HTTPBase
+
 from jwt.algorithms import has_crypto, requires_cryptography
 from jwt.exceptions import ExpiredSignatureError
 
 from libre_fastapi_jwt.auth_config import AuthConfig
 from libre_fastapi_jwt.exceptions import (
     AccessTokenRequired,
     ClaimsRequired,
@@ -1121,7 +1126,23 @@
 
         :param encoded_token: The encoded JWT to get the Header from
         :return: JWT header parameters as a dictionary
         """
         encoded_token = encoded_token or self._token
 
         return jwt.get_unverified_header(encoded_token)
+
+class AuthJWTBearer(HTTPBase):
+    def __init__(
+        self,
+        *,
+        bearerFormat: Optional[str] = None,
+        scheme_name: Optional[str] = None,
+        description: Optional[str] = None,
+        auto_error: bool = True,
+    ):
+        self.model = HTTPBearerModel(bearerFormat=bearerFormat, description=description)
+        self.scheme_name = scheme_name or self.__class__.__name__
+        self.auto_error = auto_error
+
+    def __call__(self, req: Request = None, res: Response = None) -> AuthJWT:
+        return AuthJWT(req=req, res=res)
```

### Comparing `libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/config.py` & `libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/exceptions.py` & `libre_fastapi_jwt-0.22.0/libre_fastapi_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.5/pyproject.toml` & `libre_fastapi_jwt-0.22.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "libre-fastapi-jwt"
-version = "0.21.5"
+version = "0.22.0"
 description = "Yet another fork of fast-jwt-auth"
 authors = ["Libre NZ <github-support@libre.nz>"]
 license = "MIT"
 repository = "https://github.com/LibreNZ/libre-fastapi-jwt"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
```

### Comparing `libre_fastapi_jwt-0.21.5/PKG-INFO` & `libre_fastapi_jwt-0.22.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libre-fastapi-jwt
-Version: 0.21.5
+Version: 0.22.0
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
-Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.21.5 Summary: Yet
+Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.22.0 Summary: Yet
 another fork of fast-jwt-auth Home-page: https://github.com/LibreNZ/libre-
 fastapi-jwt License: MIT Author: Libre NZ Author-email: github-support@libre.nz
 Requires-Python: >=3.9,<4.0 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

