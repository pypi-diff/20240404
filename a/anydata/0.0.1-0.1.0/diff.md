# Comparing `tmp/anydata-0.0.1.tar.gz` & `tmp/anydata-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydata-0.0.1.tar", max compression
+gzip compressed data, was "anydata-0.1.0.tar", max compression
```

## Comparing `anydata-0.0.1.tar` & `anydata-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-04-01 21:27:17.734610 anydata-0.0.1/LICENSE
--rw-r--r--   0        0        0        9 2024-04-01 21:27:17.734734 anydata-0.0.1/README.md
--rw-r--r--   0        0        0       69 2024-04-01 23:18:17.446624 anydata-0.0.1/anydata/__init__.py
--rw-r--r--   0        0        0     9927 2024-04-01 22:46:56.105109 anydata-0.0.1/anydata/core/dataapi.py
--rw-r--r--   0        0        0     6934 2024-04-02 00:16:17.762794 anydata-0.0.1/anydata/core/endpoint.py
--rw-r--r--   0        0        0     6668 2024-04-01 22:48:33.648618 anydata-0.0.1/anydata/engine/functions.py
--rw-r--r--   0        0        0      343 2024-04-01 21:29:01.793515 anydata-0.0.1/anydata/engine/models.py
--rw-r--r--   0        0        0     1303 2024-04-01 21:29:01.800618 anydata-0.0.1/anydata/engine/prompts/system_prompts.py
--rw-r--r--   0        0        0     1156 2024-04-01 21:29:01.800928 anydata-0.0.1/anydata/engine/prompts/user_prompts.py
--rw-r--r--   0        0        0     6148 2024-04-01 21:29:15.125940 anydata-0.0.1/anydata/parsers/.DS_Store
--rw-r--r--   0        0        0     8550 2024-04-01 22:48:49.129458 anydata-0.0.1/anydata/parsers/openapi.py
--rw-r--r--   0        0        0     2039 2024-04-01 23:09:38.254952 anydata-0.0.1/anydata/parsers/response_parser.py
--rw-r--r--   0        0        0     4502 2024-04-01 21:29:26.598358 anydata-0.0.1/anydata/schemas/core.py
--rw-r--r--   0        0        0     2595 2024-04-01 21:29:26.598807 anydata-0.0.1/anydata/schemas/openapi.py
--rw-r--r--   0        0        0      553 2024-04-01 23:13:46.546543 anydata-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 anydata-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-01 21:27:17.734610 anydata-0.1.0/LICENSE
+-rw-r--r--   0        0        0        9 2024-04-01 21:27:17.734734 anydata-0.1.0/README.md
+-rw-r--r--   0        0        0       69 2024-04-01 23:18:17.446624 anydata-0.1.0/anydata/__init__.py
+-rw-r--r--   0        0        0    10014 2024-04-03 04:10:20.922198 anydata-0.1.0/anydata/core/dataapi.py
+-rw-r--r--   0        0        0     7797 2024-04-03 03:04:12.951439 anydata-0.1.0/anydata/core/endpoint.py
+-rw-r--r--   0        0        0     6680 2024-04-04 02:31:10.427039 anydata-0.1.0/anydata/engine/functions.py
+-rw-r--r--   0        0        0      343 2024-04-01 21:29:01.793515 anydata-0.1.0/anydata/engine/models.py
+-rw-r--r--   0        0        0     1303 2024-04-01 21:29:01.800618 anydata-0.1.0/anydata/engine/prompts/system_prompts.py
+-rw-r--r--   0        0        0     1156 2024-04-01 21:29:01.800928 anydata-0.1.0/anydata/engine/prompts/user_prompts.py
+-rw-r--r--   0        0        0     6148 2024-04-01 21:29:15.125940 anydata-0.1.0/anydata/parsers/.DS_Store
+-rw-r--r--   0        0        0     8550 2024-04-01 22:48:49.129458 anydata-0.1.0/anydata/parsers/openapi.py
+-rw-r--r--   0        0        0     2039 2024-04-01 23:09:38.254952 anydata-0.1.0/anydata/parsers/response_parser.py
+-rw-r--r--   0        0        0     4529 2024-04-03 00:04:13.649448 anydata-0.1.0/anydata/schemas/core.py
+-rw-r--r--   0        0        0     2595 2024-04-01 21:29:26.598807 anydata-0.1.0/anydata/schemas/openapi.py
+-rw-r--r--   0        0        0      553 2024-04-04 04:54:42.425818 anydata-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 anydata-0.1.0/PKG-INFO
```

### Comparing `anydata-0.0.1/LICENSE` & `anydata-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anydata-0.0.1/anydata/core/dataapi.py` & `anydata-0.1.0/anydata/core/dataapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import json
+import copy
 import inspect
 from typing import Optional, Union, List, Tuple
 from dataclasses import dataclass
 from guidance.models import Model
 from ..schemas.core import ABCDataAPI
 from ..core.endpoint import Endpoint
 from ..engine.functions import dataapi_from_prompt, evaluate_unsuccessful_response
@@ -67,26 +68,26 @@
         Update the shared parameters for the DataAPI.
         This method overwrites the 'shared_params' parameter defined at DataAPI instantiation
         and propagate to all attached endpoints, if 'propagate' is True.
         '''
         self.shared_params = params
         if propagate:
             for endpoint in self.endpoints():
-                self[endpoint[0]].merge_params(params)
+                self[endpoint[0]].merge_params(copy.deepcopy(params))
     
     def set_shared_headers(self, headers: dict, propagate: bool=True) -> None:
         '''
         Update the shared headers for the DataAPI.
         This method overwrites the 'shared_headers' parameter defined at DataAPI instantiation
         and propagate to all attached endpoints, if 'propagate' is True.
         '''
         self.shared_headers = headers
         if propagate:
             for endpoint in self.endpoints():
-                self[endpoint[0]].merge_headers(headers)
+                self[endpoint[0]].merge_headers(copy.deepcopy(headers))
 
     def endpoints(self) -> List[Tuple[str, Endpoint]]:
         return inspect.getmembers(self, lambda a: isinstance(a, Endpoint))
 
     def add_endpoint(
             self,
             endpoint: str,
@@ -119,18 +120,18 @@
             stream=self.stream if stream is None else stream,
             verify=self.verify if verify is None else verify,
             cert=cert or self.cert,
             **kwargs
         )
         # Merge explicit parameters with shared parameters
         if params and self.shared_params:
-            endpoint_object.merge_params(self.shared_params)
+            endpoint_object.merge_params(copy.deepcopy(self.shared_params))
         # Merge explicit headers with shared headers
         if headers and self.shared_headers:
-            endpoint_object.merge_headers(self.shared_headers)
+            endpoint_object.merge_headers(copy.deepcopy(self.shared_headers))
         # Attach endpoint to DataAPI
         if alias:
             super().__setitem__(alias, endpoint_object)
         else:
             super().__setitem__(endpoint, endpoint_object)
 
     def smart_add_endpoint(
@@ -159,15 +160,15 @@
                 endpoint=stateless_lm['endpoint'],
                 method=stateless_lm['method'],
                 params=json.loads(stateless_lm['parameters']),
                 headers=self.shared_headers,
                 raise_unsuccessful=False
             )
             if self.shared_params:
-                test_endpoint.merge_params(self.shared_params)
+                test_endpoint.merge_params(copy.deepcopy(self.shared_params))
             test_response = test_endpoint.request()
             print(f"Test request to the endpoint '{stateless_lm['endpoint']}' returned status code {test_response.status_code}.")
             if test_response.status_code != 200:
                 stateless_lm += evaluate_unsuccessful_response(prompt=prompt, response=test_response)
             else:
                 self.add_endpoint(
                     endpoint=stateless_lm['endpoint'],
```

### Comparing `anydata-0.0.1/anydata/core/endpoint.py` & `anydata-0.1.0/anydata/core/endpoint.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,20 +16,21 @@
         print(resp.text)
         raise ValueError(f"Unsuccessful request with status code {resp.status_code}.")
 
 def _merge_setting(new_setting: dict, base_setting: Optional[dict]=None) -> dict:
     assert isinstance(new_setting, Mapping), f"New setting to be merged must be a valid mapping. 'new_setting' provided is of type {type(new_setting)}."
     if base_setting:
         assert isinstance(base_setting, Mapping), f"Base setting to be merged must be a valid mapping. 'base_setting' provided is of type {type(base_setting)}."
-        new_setting = copy.deepcopy(new_setting)
+        merged_setting = copy.deepcopy(new_setting)
         try:
             for key, value in base_setting.items():
-                new_setting.setdefault(key, value)
+                merged_setting.setdefault(key, value)
         except AttributeError:
             pass
+        return merged_setting
     return new_setting
 
 class Endpoint(EndpointSession):
     def __init__(
             self,
             base_url: str,
             endpoint: str,
@@ -82,79 +83,97 @@
             f'{stream_str}'
             f'{cert_str}'
             f')'
         ).replace(", )", ")")
 
     def _set_path_params(self) -> dict:
         '''
-        Sets path parameters from the endpoint URL as a dictionary with parameter names as values.
-        If self.params is defined, attempts to assign path parameters values from self.params, deleting them from self.params.
-        If self.params is not defined, returns None for each path parameter found in the endpoint relative URL.
-        Will match any string between curly braces {} at the endpoint relative URL.
-        '''
-        path_params = re.findall(r'\{([^{}]+)\}', self.endpoint)
+        Extract path parameters from the endpoint and store them in self.path_params.
+        To obtain path parameters values this method takes self.params as the first precedence, and self.path_params as the second.
+        It will also remove path parameters from self.params if they are found in the endpoint.
+        Example:
+            endpoint = "/users/{user_id}/posts/{post_id}"
+            endpoint.params = {"user_id": 2, "post_id": None, "format": "json"}
+            endpoint.path_params = {"user_id": 1, "post_id": 1}
+            endpoint._set_path_params()
+        Will result in:
+            endpoint.params = {"format": "json"}
+            endpoint.path_params = {"user_id": 2, "post_id": 1}
+        '''
+        # List all path parameters in the endpoint
+        path_params_list = re.findall(r'\{([^{}]+)\}', self.endpoint)
+        # Initialize path parameters dictionary
+        path_params = {param: None for param in path_params_list}
+        # Merge with current self.path_params, if any
+        if hasattr(self, 'path_params'):
+            path_params = _merge_setting(self.path_params, path_params)
+        # Merge with current self.params, if any
+        if self.params:
+            path_params = _merge_setting(self.params, path_params)
+        # Trim to only path parameters
+        path_params = {param: path_params[param] for param in path_params_list}
+        # Remove path parameters from self.params, if any
         if self.params:
-            path_params_dict = {}
-            for parameter in path_params:
+            for param in path_params:
                 try:
-                    path_params_dict[parameter] = self.params[parameter]
-                    self.params.pop(parameter)
+                    self.params.pop(param)
                 except KeyError:
-                    path_params_dict[parameter] = None
-        else:
-            path_params_dict = {param: None for param in path_params}
-        if hasattr(self, 'path_params'):
-            self.path_params = _merge_setting(path_params_dict, self.path_params)
-        else:
-            self.path_params = path_params_dict
+                    pass
+        self.path_params = path_params
 
-    def set_params(self, params: dict, reset_path_params: bool=True) -> None:
+    def set_params(self, params: dict) -> None:
         '''
         Replace Endpoint 'params' with new parameters.
         This method overwrites default parameters defined at Endpoint instantiation,
         '''
         self.params = params
-        if reset_path_params:
-            self._set_path_params()
+        self._set_path_params()
     
     def set_body(self, body: dict) -> None:
         '''
         Update the body for the Endpoint.
         '''
         self.body = body
     
-    def merge_params(self, params: dict, reset_path_params: bool=True) -> None:
+    def merge_params(self, params: dict) -> None:
         '''
         Merge Endpoint 'params' with new parameters.
         This method replaces existing parameter values with new ones, and preserves the rest.
         '''
         self.params = _merge_setting(params, self.params)
-        if reset_path_params:
-            self._set_path_params()
+        self._set_path_params()
 
     def merge_headers(self, headers: dict) -> None:
         '''
         Merge Endpoint 'headers' with new headers.
         This method replaces existing header values with new ones, and preserves the rest.
         It is preferred over manual assignment to avoid losing default headers.
         '''
         self.headers = _merge_setting(headers, self.headers)
 
     def request(
             self,
             params: Optional[dict] = None,
-            path_params: Optional[dict] = None,
             body: Optional[dict] = None,
             headers: Optional[dict] = None,
             files: Optional[dict] = None,
             timeout: Optional[int] = None,
             stream: Optional[bool] = None
     ) -> Response:
-        path_params = path_params or {}
-        path_params = _merge_setting(path_params, self.path_params)
+        if params:
+            # Retrieve path parameters passed explicitly in the request
+            path_params = {param: value for param, value in params.items() if param in self.path_params}
+            # And remove them from explicitly passed parameters
+            for param in path_params:
+                params.pop(param)
+            # Merge with default path parameters, if any
+            path_params = _merge_setting(path_params, self.path_params)
+        else:
+            path_params = self.path_params
+        # Format endpoint
         endpoint = self.endpoint.format(**path_params)
         resp = super().request(
             endpoint=endpoint,
             params=params,
             body=body,
             headers=headers,
             files=files,
```

### Comparing `anydata-0.0.1/anydata/engine/functions.py` & `anydata-0.1.0/anydata/engine/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                                     openapi: OpenAPI,
                                     endpoint: Optional[str]=None
                                     ) -> guidance.models.Model:
     '''
     Returns a guidance lm model carrying a REST API operation for the endpoint at the 'method' variable.
     '''
     if not endpoint:
-        assert lm['endpoint'], "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
+        assert 'endpoint' in lm, "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
         endpoint = lm['endpoint']
     # endpoint_summary = yaml.dump(openapi.paths_summary()[endpoint])
     endpoint_summary = openapi.paths_summary()[endpoint]
     endpoint_methods = dict(openapi.endpoint_methods)[endpoint]
     with system():
         lm += REST_API_OPERATION_FETCHER
     with user():
@@ -93,18 +93,18 @@
                                      method: Optional[str]=None,
                                      temperature: Optional[float]=0.0
                                      ) -> guidance.models.Model:
     '''
     Returns a guidance lm model carrying a JSON object with key value pairs for the parameters needed to call the endpoint.
     '''
     if not endpoint:
-        assert lm['endpoint'], "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
+        assert 'endpoint' in lm, "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
         endpoint = lm['endpoint']
     if not method:
-        assert lm['method'], "If 'method' is not provided, it must be captured at the 'method' variable in the lm model."
+        assert 'method' in lm, "If 'method' is not provided, it must be captured at the 'method' variable in the lm model."
         method = lm['method']
     # method_openapi = yaml.dump(openapi.paths_summary(resolve_parameter_references=True)[endpoint][method])
     method_openapi = openapi.paths_summary(resolve_parameter_references=True)[endpoint][method]
     with system():
         lm += REST_API_PARAMETERS_FETCHER
     with user():
         lm += rest_api_parameters_user_prompt(prompt, endpoint, method_openapi)
@@ -120,21 +120,21 @@
                                    method: Optional[str]=None,
                                    parameters: Optional[dict]=None
                                    ) -> guidance.models.Model:
     '''
     Evaluates the response from a REST API call and raises an error if the response is unsuccessful.
     '''
     if not endpoint:
-        assert lm['endpoint'], "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
+        assert 'endpoint' in lm, "If 'endpoint' is not provided, it must be captured at the 'endpoint' variable in the lm model."
         endpoint = lm['endpoint']
     if not method:
-        assert lm['method'], "If 'method' is not provided, it must be captured at the 'method' variable in the lm model."
+        assert 'method' in lm, "If 'method' is not provided, it must be captured at the 'method' variable in the lm model."
         method = lm['method']
     if not parameters:
-        assert lm['parameters'], "If 'parameters' is not provided, it must be captured at the 'parameters' variable in the lm model."
+        assert 'parameters' in lm, "If 'parameters' is not provided, it must be captured at the 'parameters' variable in the lm model."
         parameters = lm['parameters']
     with system():
         lm += '''
 You only reply with a number corresponding to one of the following options:
     1. The parameters provided are incorrect.
     2. The REST API operation is incorrect.
     3. The endpoint is incorrect.
```

### Comparing `anydata-0.0.1/anydata/engine/prompts/system_prompts.py` & `anydata-0.1.0/anydata/engine/prompts/system_prompts.py`

 * *Files identical despite different names*

### Comparing `anydata-0.0.1/anydata/engine/prompts/user_prompts.py` & `anydata-0.1.0/anydata/engine/prompts/user_prompts.py`

 * *Files identical despite different names*

### Comparing `anydata-0.0.1/anydata/parsers/.DS_Store` & `anydata-0.1.0/anydata/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `anydata-0.0.1/anydata/parsers/openapi.py` & `anydata-0.1.0/anydata/parsers/openapi.py`

 * *Files identical despite different names*

### Comparing `anydata-0.0.1/anydata/parsers/response_parser.py` & `anydata-0.1.0/anydata/parsers/response_parser.py`

 * *Files identical despite different names*

### Comparing `anydata-0.0.1/anydata/schemas/core.py` & `anydata-0.1.0/anydata/schemas/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 from typing import Optional
 from requests.sessions import Session
 from collections.abc import MutableMapping
 from requests.sessions import Session, merge_setting
 
 class ABCDataAPI(MutableMapping):
     '''
@@ -66,15 +67,15 @@
         # Session.__init__() sets default headers, default hooks,
         # max_redirects, and initialize an empty cookie jar
         # It also initialize and mount adapters
         super().__init__()
         # Override defaults from Session.__init__()
         # Update default headers with user defined headers
         self.headers = merge_setting(headers, self.headers)
-        self.params = params
+        self.params = copy.deepcopy(params)
         self.auth = auth
         self.stream = stream
         self.verify = verify
         self.cert = cert
 
     def request(
             self,
```

### Comparing `anydata-0.0.1/anydata/schemas/openapi.py` & `anydata-0.1.0/anydata/schemas/openapi.py`

 * *Files identical despite different names*

### Comparing `anydata-0.0.1/pyproject.toml` & `anydata-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydata"
-version = "0.0.1"
+version = "0.1.0"
 description = "Smart framework to interact with and fetch data from REST APIs."
 authors = ["Erich Silva <erich@esilva.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `anydata-0.0.1/PKG-INFO` & `anydata-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydata
-Version: 0.0.1
+Version: 0.1.0
 Summary: Smart framework to interact with and fetch data from REST APIs.
 License: Apache 2.0
 Author: Erich Silva
 Author-email: erich@esilva.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

