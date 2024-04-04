# Comparing `tmp/libre_fastapi_jwt-0.21.4.tar.gz` & `tmp/libre_fastapi_jwt-0.21.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libre_fastapi_jwt-0.21.4.tar", max compression
+gzip compressed data, was "libre_fastapi_jwt-0.21.5.tar", max compression
```

## Comparing `libre_fastapi_jwt-0.21.4.tar` & `libre_fastapi_jwt-0.21.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-01 08:53:59.420708 libre_fastapi_jwt-0.21.4/LICENSE
--rw-r--r--   0        0        0     2079 2024-04-01 08:53:59.420708 libre_fastapi_jwt-0.21.4/README.md
--rw-r--r--   0        0        0      148 2024-04-01 08:53:59.424708 libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/__init__.py
--rw-r--r--   0        0        0     5472 2024-04-01 08:53:59.424708 libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/auth_config.py
--rw-r--r--   0        0        0    44626 2024-04-01 08:53:59.424708 libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/auth_jwt.py
--rw-r--r--   0        0        0     5124 2024-04-01 08:53:59.424708 libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/config.py
--rw-r--r--   0        0        0     3059 2024-04-01 08:53:59.424708 libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/exceptions.py
--rw-r--r--   0        0        0     1083 2024-04-01 08:53:59.424708 libre_fastapi_jwt-0.21.4/pyproject.toml
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.21.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-04 05:38:12.436142 libre_fastapi_jwt-0.21.5/LICENSE
+-rw-r--r--   0        0        0     2079 2024-04-04 05:38:12.436142 libre_fastapi_jwt-0.21.5/README.md
+-rw-r--r--   0        0        0      148 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/__init__.py
+-rw-r--r--   0        0        0     5413 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/auth_config.py
+-rw-r--r--   0        0        0    44689 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/auth_jwt.py
+-rw-r--r--   0        0        0     5124 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/config.py
+-rw-r--r--   0        0        0     3059 2024-04-04 05:38:12.440142 libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/exceptions.py
+-rw-r--r--   0        0        0     1083 2024-04-04 05:38:12.444142 libre_fastapi_jwt-0.21.5/pyproject.toml
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 libre_fastapi_jwt-0.21.5/PKG-INFO
```

### Comparing `libre_fastapi_jwt-0.21.4/LICENSE` & `libre_fastapi_jwt-0.21.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.4/README.md` & `libre_fastapi_jwt-0.21.5/README.md`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/auth_config.py` & `libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/auth_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from libre_fastapi_jwt.config import LoadConfig
 from pydantic import ValidationError
 from typing import Callable, List
 from datetime import timedelta
-from fastapi.security.base import SecurityBase
 
 
-class AuthConfig(SecurityBase):
+class AuthConfig():
     _token = None
     _token_location = {"headers"}
 
     _secret_key = None
     _public_key = None
     _private_key = None
     _algorithm = "HS256"
```

### Comparing `libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/auth_jwt.py` & `libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/auth_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import jwt, re, hmac
 from uuid import uuid4
 from datetime import datetime, timedelta, timezone
 from typing import Dict, Optional, Sequence, Union
-from fastapi import Request, Response, WebSocket, Header
+from fastapi import Request, Response, WebSocket, Header, Security
+from fastapi.security import APIKeyCookie
 from jwt.algorithms import has_crypto, requires_cryptography
 from jwt.exceptions import ExpiredSignatureError
 
 from libre_fastapi_jwt.auth_config import AuthConfig
 from libre_fastapi_jwt.exceptions import (
     AccessTokenRequired,
     ClaimsRequired,
@@ -41,18 +42,18 @@
             auth = (b"authorization", bytes("Bearer {}".format(token), "UTF-8"))
             req.headers._list.append(auth)
 
         if res and self.jwt_in_cookies:
             self._response = res
 
         if req:
-            # get request object when cookies in token location
+            # get request object when 'cookies' in authjwt_token_location
             if self.jwt_in_cookies:
                 self._request = req
-            # get jwt in headers when headers in token location
+            # get jwt in headers when 'headers' in authjwt_token_location
             if self.jwt_in_headers:
                 auth = req.headers.get(self._header_name.lower())
                 if auth:
                     self._get_jwt_from_headers(auth)
 
     def _get_jwt_from_headers(self, auth: str) -> "AuthJWT":
         """
@@ -911,29 +912,27 @@
             for claim in self._required_claims:
                 if claim not in raw_token or raw_token[claim] is None:
                     raise ClaimsRequired(status_code=422, message="Missing claim: team")
 
     def jwt_required(
         self,
         auth_from: str = "request",
-        token: Optional[str] = None,
+        token: Optional[str] = Security(APIKeyCookie(name="Authorization", auto_error=False)),
         websocket: Optional[WebSocket] = None,
         csrf_token: Optional[str] = None,
         roles: list = [],
         claims: list = [],
     ) -> None:
         """
         Only access token can access this function
 
         :param auth_from: for identity get token from HTTP or WebSocket
-        :param token: the encoded JWT, it's required if the protected endpoint use WebSocket to
-                      authorization and get token from Query Url or Path
+        :param token: the encoded JWT, it's required if the protected endpoint use WebSocket to authorize and get token from Query Url or Path
         :param websocket: an instance of WebSocket, it's required if protected endpoint use a cookie to authorization
-        :param csrf_token: the CSRF double submit token. since WebSocket cannot add specifying additional headers
-                           its must be passing csrf_token manually and can achieve by Query Url or Path
+        :param csrf_token: the CSRF double submit token. Since WebSocket cannot add specific additional headers, it must pass csrf_token manually to achieve a Query Url or Path
         """
         self._required_claims = claims
         self._required_roles = roles
 
         if auth_from == "websocket":
             if websocket:
                 self._verify_and_get_jwt_in_cookies("access", websocket, csrf_token)
```

### Comparing `libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/config.py` & `libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/config.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.4/libre_fastapi_jwt/exceptions.py` & `libre_fastapi_jwt-0.21.5/libre_fastapi_jwt/exceptions.py`

 * *Files identical despite different names*

### Comparing `libre_fastapi_jwt-0.21.4/pyproject.toml` & `libre_fastapi_jwt-0.21.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "libre-fastapi-jwt"
-version = "0.21.4"
+version = "0.21.5"
 description = "Yet another fork of fast-jwt-auth"
 authors = ["Libre NZ <github-support@libre.nz>"]
 license = "MIT"
 repository = "https://github.com/LibreNZ/libre-fastapi-jwt"
 readme = "README.md"
 classifiers = [
   "Environment :: Web Environment",
```

### Comparing `libre_fastapi_jwt-0.21.4/PKG-INFO` & `libre_fastapi_jwt-0.21.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libre-fastapi-jwt
-Version: 0.21.4
+Version: 0.21.5
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
-Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.21.4 Summary: Yet
+Metadata-Version: 2.1 Name: libre-fastapi-jwt Version: 0.21.5 Summary: Yet
 another fork of fast-jwt-auth Home-page: https://github.com/LibreNZ/libre-
 fastapi-jwt License: MIT Author: Libre NZ Author-email: github-support@libre.nz
 Requires-Python: >=3.9,<4.0 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

