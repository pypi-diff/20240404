# Comparing `tmp/vonage-http-client-1.1.1.tar.gz` & `tmp/vonage-http-client-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-http-client-1.1.1.tar", last modified: Thu Mar 28 03:16:58 2024, max compression
+gzip compressed data, was "vonage-http-client-1.2.0.tar", last modified: Thu Apr  4 05:14:01 2024, max compression
```

## Comparing `vonage-http-client-1.1.1.tar` & `vonage-http-client-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:58.181553 vonage-http-client-1.1.1/
--rw-r--r--   0 mkahan     (503) staff       (20)     3264 2024-03-28 03:16:58.181038 vonage-http-client-1.1.1/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     2391 2024-03-28 03:16:57.000000 vonage-http-client-1.1.1/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-03-28 03:16:57.000000 vonage-http-client-1.1.1/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      910 2024-03-28 03:16:57.000000 vonage-http-client-1.1.1/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-03-28 03:16:58.181617 vonage-http-client-1.1.1/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:58.167457 vonage-http-client-1.1.1/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:58.174245 vonage-http-client-1.1.1/src/vonage_http_client/
--rw-r--r--   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:57.000000 vonage-http-client-1.1.1/src/vonage_http_client/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     5060 2024-03-28 03:16:57.000000 vonage-http-client-1.1.1/src/vonage_http_client/auth.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4194 2024-03-28 03:16:57.000000 vonage-http-client-1.1.1/src/vonage_http_client/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     8216 2024-03-28 03:16:57.000000 vonage-http-client-1.1.1/src/vonage_http_client/http_client.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-03-28 03:16:58.180507 vonage-http-client-1.1.1/src/vonage_http_client.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     3264 2024-03-28 03:16:58.000000 vonage-http-client-1.1.1/src/vonage_http_client.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      406 2024-03-28 03:16:58.000000 vonage-http-client-1.1.1/src/vonage_http_client.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-03-28 03:16:58.000000 vonage-http-client-1.1.1/src/vonage_http_client.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       96 2024-03-28 03:16:58.000000 vonage-http-client-1.1.1/src/vonage_http_client.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       19 2024-03-28 03:16:58.000000 vonage-http-client-1.1.1/src/vonage_http_client.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.639546 vonage-http-client-1.2.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3640 2024-04-04 05:14:01.637722 vonage-http-client-1.2.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     2767 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      910 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-04 05:14:01.639777 vonage-http-client-1.2.0/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.612169 vonage-http-client-1.2.0/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.624034 vonage-http-client-1.2.0/src/vonage_http_client/
+-rw-r--r--   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/src/vonage_http_client/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     5021 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/src/vonage_http_client/auth.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     4824 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/src/vonage_http_client/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     9284 2024-04-04 05:14:00.000000 vonage-http-client-1.2.0/src/vonage_http_client/http_client.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-04 05:14:01.634907 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3640 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      406 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       96 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       19 2024-04-04 05:14:01.000000 vonage-http-client-1.2.0/src/vonage_http_client.egg-info/top_level.txt
```

### Comparing `vonage-http-client-1.1.1/PKG-INFO` & `vonage-http-client-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vonage-http-client
-Version: 1.1.1
+Version: 1.2.0
 Summary: An HTTP client for making requests to Vonage APIs.
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-utils>=1.0.0
+Requires-Dist: vonage-utils>=1.0.1
 Requires-Dist: vonage-jwt>=1.1.0
 Requires-Dist: requests>=2.27.0
 Requires-Dist: pydantic>=2.6.1
 Requires-Dist: typing_extensions>=4.9.0
 
 # Vonage HTTP Client Package
 
@@ -60,17 +60,29 @@
 # Make a GET request
 response = client.get(host='api.nexmo.com', request_path='/v1/messages')
 
 # Make a POST request
 response = client.post(host='api.nexmo.com', request_path='/v1/messages', params={'key': 'value'})
 ```
 
+## Get the Last Request and Last Response from the HTTP Client
+
+The `HttpClient` class exposes two properties, `last_request` and `last_response` that cache the last sent request and response.
+
+```python
+# Get last request, has type requests.PreparedRequest
+request = client.last_request
+
+# Get last response, has type requests.Response
+response = client.last_response
+```
+
 ### Appending to the User-Agent Header
 
-The HttpClient class also supports appending additional information to the User-Agent header via the append_to_user_agent method:
+The `HttpClient` class also supports appending additional information to the User-Agent header via the append_to_user_agent method:
 
 ```python
 client.append_to_user_agent('additional_info')
 ```
 
 ### Changing the Authentication Method Used
```

### Comparing `vonage-http-client-1.1.1/README.md` & `vonage-http-client-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,29 @@
 # Make a GET request
 response = client.get(host='api.nexmo.com', request_path='/v1/messages')
 
 # Make a POST request
 response = client.post(host='api.nexmo.com', request_path='/v1/messages', params={'key': 'value'})
 ```
 
+## Get the Last Request and Last Response from the HTTP Client
+
+The `HttpClient` class exposes two properties, `last_request` and `last_response` that cache the last sent request and response.
+
+```python
+# Get last request, has type requests.PreparedRequest
+request = client.last_request
+
+# Get last response, has type requests.Response
+response = client.last_response
+```
+
 ### Appending to the User-Agent Header
 
-The HttpClient class also supports appending additional information to the User-Agent header via the append_to_user_agent method:
+The `HttpClient` class also supports appending additional information to the User-Agent header via the append_to_user_agent method:
 
 ```python
 client.append_to_user_agent('additional_info')
 ```
 
 ### Changing the Authentication Method Used
```

### Comparing `vonage-http-client-1.1.1/backend_shim.py` & `vonage-http-client-1.2.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-http-client-1.1.1/pyproject.toml` & `vonage-http-client-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "vonage-http-client"
-version = "1.1.1"
+version = "1.2.0"
 description = "An HTTP client for making requests to Vonage APIs."
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-utils>=1.0.0",
+  "vonage-utils>=1.0.1",
   "vonage-jwt>=1.1.0",
   "requests>=2.27.0",
   "pydantic>=2.6.1",
   "typing_extensions>=4.9.0",
 ]
 classifiers = [
   "Programming Language :: Python",
```

### Comparing `vonage-http-client-1.1.1/src/vonage_http_client/auth.py` & `vonage-http-client-1.2.0/src/vonage_http_client/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         hasher = hmac.new(
             self._signature_secret.encode(),
             digestmod=self._signature_method,
         )
 
         if not params.get('timestamp'):
             params['timestamp'] = int(time())
-            print(params['timestamp'])
 
         for key in sorted(params):
             value = params[key]
 
             if isinstance(value, str):
                 value = value.replace('&', '_').replace('=', '_')
```

### Comparing `vonage-http-client-1.1.1/src/vonage_http_client/errors.py` & `vonage-http-client-1.2.0/src/vonage_http_client/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,14 +63,32 @@
         message (str): The returned error message.
     """
 
     def __init__(self, response: Response, content_type: str):
         super().__init__(response, content_type)
 
 
+class ForbiddenError(HttpRequestError):
+    """Exception indicating a forbidden request in a Vonage SDK request.
+
+    This error is raised when the HTTP response status code is 403 (Forbidden).
+
+    Args:
+        response (requests.Response): The HTTP response object.
+        content_type (str): The response content type.
+
+    Attributes (inherited from HttpRequestError parent exception):
+        response (requests.Response): The HTTP response object.
+        message (str): The returned error message.
+    """
+
+    def __init__(self, response: Response, content_type: str):
+        super().__init__(response, content_type)
+
+
 class NotFoundError(HttpRequestError):
     """Exception indicating a resource was not found in a Vonage SDK request.
 
     This error is raised when the HTTP response status code is 404 (Not Found).
 
     Args:
         response (requests.Response): The HTTP response object.
```

### Comparing `vonage-http-client-1.1.1/src/vonage_http_client/http_client.py` & `vonage-http-client-1.2.0/src/vonage_http_client/http_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from json import JSONDecodeError
 from logging import getLogger
 from platform import python_version
 from typing import Literal, Optional, Union
 
 from pydantic import BaseModel, Field, ValidationError, validate_call
-from requests import Response
+from requests import PreparedRequest, Response
 from requests.adapters import HTTPAdapter
 from requests.sessions import Session
 from typing_extensions import Annotated
 from vonage_http_client.auth import Auth
 from vonage_http_client.errors import (
     AuthenticationError,
+    ForbiddenError,
     HttpRequestError,
     InvalidHttpClientOptionsError,
     NotFoundError,
     RateLimitedError,
     ServerError,
 )
 
@@ -77,14 +78,17 @@
             max_retries=self._http_client_options.max_retries,
         )
         self._session.mount('https://', self._adapter)
 
         self._user_agent = f'vonage-python-sdk/{sdk_version} python/{python_version()}'
         self._headers = {'User-Agent': self._user_agent, 'Accept': 'application/json'}
 
+        self._last_request = None
+        self._last_response = None
+
     @property
     def auth(self):
         return self._auth
 
     @property
     def http_client_options(self):
         return self._http_client_options
@@ -97,80 +101,103 @@
     def rest_host(self):
         return self._rest_host
 
     @property
     def user_agent(self):
         return self._user_agent
 
+    @property
+    def last_request(self) -> Optional[PreparedRequest]:
+        """The last request sent to the server.
+
+        Returns:
+            Optional[PreparedRequest]: The exact bytes of the request sent to the server,
+                or None if no request has been sent.
+        """
+        return self._last_response.request
+
+    @property
+    def last_response(self) -> Optional[Response]:
+        """The last response received from the server.
+
+        Returns:
+            Optional[Response]: The response object received from the server,
+                or None if no response has been received.
+        """
+        return self._last_response
+
     def post(
         self,
         host: str,
         request_path: str = '',
         params: dict = None,
-        auth_type: Literal['jwt', 'basic', 'signature'] = 'jwt',
+        auth_type: Literal['jwt', 'basic', 'body', 'signature'] = 'jwt',
         sent_data_type: Literal['json', 'data'] = 'json',
     ) -> Union[dict, None]:
         return self.make_request(
             'POST', host, request_path, params, auth_type, sent_data_type
         )
 
     def get(
         self,
         host: str,
         request_path: str = '',
         params: dict = None,
-        auth_type: Literal['jwt', 'basic', 'signature'] = 'jwt',
-        sent_data_type: Literal['json', 'form', 'query_params'] = 'json',
+        auth_type: Literal['jwt', 'basic', 'body', 'signature'] = 'jwt',
+        sent_data_type: Literal['json', 'form', 'query_params'] = 'query_params',
     ) -> Union[dict, None]:
         return self.make_request(
             'GET', host, request_path, params, auth_type, sent_data_type
         )
 
     def patch(
         self,
         host: str,
         request_path: str = '',
         params: dict = None,
-        auth_type: Literal['jwt', 'basic', 'signature'] = 'jwt',
+        auth_type: Literal['jwt', 'basic', 'body', 'signature'] = 'jwt',
         sent_data_type: Literal['json', 'form', 'query_params'] = 'json',
     ) -> Union[dict, None]:
         return self.make_request(
             'PATCH', host, request_path, params, auth_type, sent_data_type
         )
 
     def delete(
         self,
         host: str,
         request_path: str = '',
         params: dict = None,
-        auth_type: Literal['jwt', 'basic', 'signature'] = 'jwt',
+        auth_type: Literal['jwt', 'basic', 'body', 'signature'] = 'jwt',
         sent_data_type: Literal['json', 'form', 'query_params'] = 'json',
     ) -> Union[dict, None]:
         return self.make_request(
             'DELETE', host, request_path, params, auth_type, sent_data_type
         )
 
     @validate_call
     def make_request(
         self,
         request_type: Literal['GET', 'POST', 'PATCH', 'DELETE'],
         host: str,
         request_path: str = '',
         params: Optional[dict] = None,
-        auth_type: Literal['jwt', 'basic', 'signature'] = 'jwt',
+        auth_type: Literal['jwt', 'basic', 'body', 'signature'] = 'jwt',
         sent_data_type: Literal['json', 'form', 'query_params'] = 'json',
     ):
         url = f'https://{host}{request_path}'
         logger.debug(
             f'{request_type} request to {url}, with data: {params}; headers: {self._headers}'
         )
         if auth_type == 'jwt':
             self._headers['Authorization'] = self._auth.create_jwt_auth_string()
         elif auth_type == 'basic':
             self._headers['Authorization'] = self._auth.create_basic_auth_string()
+        elif auth_type == 'body':
+            params['api_key'] = self._auth.api_key
+            params['api_secret'] = self._auth.api_secret
         elif auth_type == 'signature':
             params['api_key'] = self._auth.api_key
             params['sig'] = self._auth.sign_params(params)
 
         request_params = {
             'method': request_type,
             'url': url,
@@ -192,28 +219,31 @@
     def append_to_user_agent(self, string: str):
         self._user_agent += f' {string}'
 
     def _parse_response(self, response: Response) -> Union[dict, None]:
         logger.debug(
             f'Response received from {response.url} with status code: {response.status_code}; headers: {response.headers}'
         )
+        self._last_response = response
         content_type = response.headers['Content-Type'].split(';', 1)[0]
         if 200 <= response.status_code < 300:
             if response.status_code == 204:
                 return None
             try:
                 return response.json()
             except JSONDecodeError:
                 return None
         if response.status_code >= 400:
             logger.warning(
                 f'Http Response Error! Status code: {response.status_code}; content: {repr(response.text)}; from url: {response.url}'
             )
-            if response.status_code == 401 or response.status_code == 403:
+            if response.status_code == 401:
                 raise AuthenticationError(response, content_type)
+            if response.status_code == 403:
+                raise ForbiddenError(response, content_type)
             elif response.status_code == 404:
                 raise NotFoundError(response, content_type)
             elif response.status_code == 429:
                 raise RateLimitedError(response, content_type)
             elif response.status_code == 500:
                 raise ServerError(response, content_type)
         raise HttpRequestError(response, content_type)
```

### Comparing `vonage-http-client-1.1.1/src/vonage_http_client.egg-info/PKG-INFO` & `vonage-http-client-1.2.0/src/vonage_http_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vonage-http-client
-Version: 1.1.1
+Version: 1.2.0
 Summary: An HTTP client for making requests to Vonage APIs.
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-utils>=1.0.0
+Requires-Dist: vonage-utils>=1.0.1
 Requires-Dist: vonage-jwt>=1.1.0
 Requires-Dist: requests>=2.27.0
 Requires-Dist: pydantic>=2.6.1
 Requires-Dist: typing_extensions>=4.9.0
 
 # Vonage HTTP Client Package
 
@@ -60,17 +60,29 @@
 # Make a GET request
 response = client.get(host='api.nexmo.com', request_path='/v1/messages')
 
 # Make a POST request
 response = client.post(host='api.nexmo.com', request_path='/v1/messages', params={'key': 'value'})
 ```
 
+## Get the Last Request and Last Response from the HTTP Client
+
+The `HttpClient` class exposes two properties, `last_request` and `last_response` that cache the last sent request and response.
+
+```python
+# Get last request, has type requests.PreparedRequest
+request = client.last_request
+
+# Get last response, has type requests.Response
+response = client.last_response
+```
+
 ### Appending to the User-Agent Header
 
-The HttpClient class also supports appending additional information to the User-Agent header via the append_to_user_agent method:
+The `HttpClient` class also supports appending additional information to the User-Agent header via the append_to_user_agent method:
 
 ```python
 client.append_to_user_agent('additional_info')
 ```
 
 ### Changing the Authentication Method Used
```

