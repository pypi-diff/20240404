# Comparing `tmp/multion-0.4.3.tar.gz` & `tmp/multion-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multion-0.4.3.tar", max compression
+gzip compressed data, was "multion-0.4.4.tar", max compression
```

## Comparing `multion-0.4.3.tar` & `multion-0.4.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     3846 2024-04-04 08:18:10.851647 multion-0.4.3/README.md
--rw-r--r--   0        0        0      592 2024-04-04 08:18:10.851647 multion-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      990 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/__init__.py
--rw-r--r--   0        0        0    14297 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/client.py
--rw-r--r--   0        0        0      853 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/api_error.py
--rw-r--r--   0        0        0     1490 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/core/request_options.py
--rw-r--r--   0        0        0      162 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/environment.py
--rw-r--r--   0        0        0      170 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/py.typed
--rw-r--r--   0        0        0      247 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/__init__.py
--rw-r--r--   0        0        0    25066 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/client.py
--rw-r--r--   0        0        0      341 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/types/__init__.py
--rw-r--r--   0        0        0     1048 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/types/sessions_close_response.py
--rw-r--r--   0        0        0      953 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/types/sessions_list_response.py
--rw-r--r--   0        0        0      967 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/sessions/types/sessions_screenshot_response.py
--rw-r--r--   0        0        0      812 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/browse_output.py
--rw-r--r--   0        0        0      953 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/http_validation_error.py
--rw-r--r--   0        0        0      850 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/remote_value.py
--rw-r--r--   0        0        0     1312 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/retrieve_output.py
--rw-r--r--   0        0        0     1361 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/session_created.py
--rw-r--r--   0        0        0     1650 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/session_input.py
--rw-r--r--   0        0        0     1016 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/session_input_browser_params.py
--rw-r--r--   0        0        0     1365 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/session_step_success.py
--rw-r--r--   0        0        0      972 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/types/validation_error_loc_item.py
--rw-r--r--   0        0        0       75 2024-04-04 08:18:10.855647 multion-0.4.3/src/multion/version.py
--rw-r--r--   0        0        0     4336 1970-01-01 00:00:00.000000 multion-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     3937 2024-04-04 18:35:22.843058 multion-0.4.4/README.md
+-rw-r--r--   0        0        0      592 2024-04-04 18:35:22.843058 multion-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      990 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/__init__.py
+-rw-r--r--   0        0        0    14283 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/client.py
+-rw-r--r--   0        0        0      853 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/api_error.py
+-rw-r--r--   0        0        0     1490 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/file.py
+-rw-r--r--   0        0        0     5059 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/core/request_options.py
+-rw-r--r--   0        0        0      162 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/environment.py
+-rw-r--r--   0        0        0      170 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/py.typed
+-rw-r--r--   0        0        0      247 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/sessions/__init__.py
+-rw-r--r--   0        0        0    24876 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/sessions/client.py
+-rw-r--r--   0        0        0      341 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/sessions/types/__init__.py
+-rw-r--r--   0        0        0     1048 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/sessions/types/sessions_close_response.py
+-rw-r--r--   0        0        0      953 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/sessions/types/sessions_list_response.py
+-rw-r--r--   0        0        0      967 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/sessions/types/sessions_screenshot_response.py
+-rw-r--r--   0        0        0      812 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/browse_output.py
+-rw-r--r--   0        0        0      953 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/http_validation_error.py
+-rw-r--r--   0        0        0      850 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/remote_value.py
+-rw-r--r--   0        0        0     1312 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/retrieve_output.py
+-rw-r--r--   0        0        0     1361 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/session_created.py
+-rw-r--r--   0        0        0     1650 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/session_input.py
+-rw-r--r--   0        0        0     1016 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/session_input_browser_params.py
+-rw-r--r--   0        0        0     1365 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/session_step_success.py
+-rw-r--r--   0        0        0      972 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       75 2024-04-04 18:35:22.843058 multion-0.4.4/src/multion/version.py
+-rw-r--r--   0        0        0     4427 1970-01-01 00:00:00.000000 multion-0.4.4/PKG-INFO
```

### Comparing `multion-0.4.3/README.md` & `multion-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # MultiOn Python Library
 
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
+[![pypi](https://img.shields.io/pypi/v/multion.svg)](https://pypi.python.org/pypi/multion)
 
 The MultiOn Python Library provides convenient access to the MultiOn API from applications written in Python.
 
 ## Documentation
 
 API reference documentation is available [here](https://multion.docs.buildwithfern.com/).
```

### Comparing `multion-0.4.3/pyproject.toml` & `multion-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "multion"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "multion", from = "src"}
 ]
```

### Comparing `multion-0.4.3/src/multion/__init__.py` & `multion-0.4.4/src/multion/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/client.py` & `multion-0.4.4/src/multion/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
             _request["max_steps"] = max_steps
         if stream is not OMIT:
             _request["stream"] = stream
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/web/browse"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "browse"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
@@ -272,15 +272,15 @@
             _request["max_steps"] = max_steps
         if stream is not OMIT:
             _request["stream"] = stream
         if include_screenshot is not OMIT:
             _request["include_screenshot"] = include_screenshot
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/web/browse"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "browse"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
```

### Comparing `multion-0.4.3/src/multion/core/__init__.py` & `multion-0.4.4/src/multion/core/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/core/client_wrapper.py` & `multion-0.4.4/src/multion/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "multion",
-            "X-Fern-SDK-Version": "0.4.3",
+            "X-Fern-SDK-Version": "0.4.4",
         }
         headers["X_MULTION_API_KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `multion-0.4.3/src/multion/core/datetime_utils.py` & `multion-0.4.4/src/multion/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/core/file.py` & `multion-0.4.4/src/multion/core/file.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/core/http_client.py` & `multion-0.4.4/src/multion/core/http_client.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/core/jsonable_encoder.py` & `multion-0.4.4/src/multion/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/core/request_options.py` & `multion-0.4.4/src/multion/core/request_options.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/sessions/client.py` & `multion-0.4.4/src/multion/sessions/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         )
         client.sessions.create(
             request=SessionInput(),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/web/session"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "session"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -106,17 +106,15 @@
         client.sessions.step(
             session_id="session_id",
             request=SessionInput(),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/web/session/{jsonable_encoder(session_id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -164,17 +162,15 @@
         )
         client.sessions.close(
             session_id="session_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/web/session/{jsonable_encoder(session_id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -219,15 +215,15 @@
         client.sessions.screenshot(
             session_id="session_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/web/screenshot/{jsonable_encoder(session_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"screenshot/{jsonable_encoder(session_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
@@ -267,15 +263,15 @@
         client = MultiOn(
             api_key="YOUR_API_KEY",
         )
         client.sessions.list()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/web/sessions"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -321,15 +317,15 @@
         )
         await client.sessions.create(
             request=SessionInput(),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/web/session"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "session"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -381,17 +377,15 @@
         await client.sessions.step(
             session_id="session_id",
             request=SessionInput(),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/web/session/{jsonable_encoder(session_id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
@@ -439,17 +433,15 @@
         )
         await client.sessions.close(
             session_id="session_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "DELETE",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/web/session/{jsonable_encoder(session_id)}"
-            ),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"session/{jsonable_encoder(session_id)}"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
@@ -494,15 +486,15 @@
         await client.sessions.screenshot(
             session_id="session_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/web/screenshot/{jsonable_encoder(session_id)}"
+                f"{self._client_wrapper.get_base_url()}/", f"screenshot/{jsonable_encoder(session_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
@@ -542,15 +534,15 @@
         client = AsyncMultiOn(
             api_key="YOUR_API_KEY",
         )
         await client.sessions.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/web/sessions"),
+            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
```

### Comparing `multion-0.4.3/src/multion/sessions/types/sessions_close_response.py` & `multion-0.4.4/src/multion/sessions/types/sessions_close_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/sessions/types/sessions_list_response.py` & `multion-0.4.4/src/multion/sessions/types/sessions_list_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/sessions/types/sessions_screenshot_response.py` & `multion-0.4.4/src/multion/sessions/types/sessions_screenshot_response.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/__init__.py` & `multion-0.4.4/src/multion/types/__init__.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/browse_output.py` & `multion-0.4.4/src/multion/types/browse_output.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/http_validation_error.py` & `multion-0.4.4/src/multion/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/remote_value.py` & `multion-0.4.4/src/multion/types/remote_value.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/retrieve_output.py` & `multion-0.4.4/src/multion/types/retrieve_output.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/session_created.py` & `multion-0.4.4/src/multion/types/session_created.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/session_input.py` & `multion-0.4.4/src/multion/types/session_input.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/session_input_browser_params.py` & `multion-0.4.4/src/multion/types/session_input_browser_params.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/session_step_success.py` & `multion-0.4.4/src/multion/types/session_step_success.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/src/multion/types/validation_error.py` & `multion-0.4.4/src/multion/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `multion-0.4.3/PKG-INFO` & `multion-0.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multion
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,14 +12,15 @@
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # MultiOn Python Library
 
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
+[![pypi](https://img.shields.io/pypi/v/multion.svg)](https://pypi.python.org/pypi/multion)
 
 The MultiOn Python Library provides convenient access to the MultiOn API from applications written in Python.
 
 ## Documentation
 
 API reference documentation is available [here](https://multion.docs.buildwithfern.com/).
```

