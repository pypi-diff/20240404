# Comparing `tmp/django_contract_tester-1.3.0.tar.gz` & `tmp/django_contract_tester-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_contract_tester-1.3.0.tar", max compression
+gzip compressed data, was "django_contract_tester-1.3.1.tar", max compression
```

## Comparing `django_contract_tester-1.3.0.tar` & `django_contract_tester-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      598 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1500 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/LICENSE
--rw-r--r--   0        0        0     8081 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/README.md
--rw-r--r--   0        0        0      558 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/__init__.py
--rw-r--r--   0        0        0     1135 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/case_testers.py
--rw-r--r--   0        0        0     1363 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/clients.py
--rw-r--r--   0        0        0      428 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/config.py
--rw-r--r--   0        0        0     2780 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/constants.py
--rw-r--r--   0        0        0      742 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/exceptions.py
--rw-r--r--   0        0        0    10894 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/loaders.py
--rw-r--r--   0        0        0        0 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/py.typed
--rw-r--r--   0        0        0     1934 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/response_handler.py
--rw-r--r--   0        0        0      845 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/response_handler_factory.py
--rw-r--r--   0        0        0    23192 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/schema_tester.py
--rw-r--r--   0        0        0     2151 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/utils.py
--rw-r--r--   0        0        0     7938 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/openapi_tester/validators.py
--rw-r--r--   0        0        0     3552 2024-03-14 17:02:50.904580 django_contract_tester-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    10654 1970-01-01 00:00:00.000000 django_contract_tester-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      598 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1500 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/LICENSE
+-rw-r--r--   0        0        0     8081 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/README.md
+-rw-r--r--   0        0        0      577 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/case_testers.py
+-rw-r--r--   0        0        0     4032 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/clients.py
+-rw-r--r--   0        0        0      426 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/config.py
+-rw-r--r--   0        0        0     2923 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/constants.py
+-rw-r--r--   0        0        0      762 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/exceptions.py
+-rw-r--r--   0        0        0    11261 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/py.typed
+-rw-r--r--   0        0        0     1918 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/response_handler.py
+-rw-r--r--   0        0        0      856 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/response_handler_factory.py
+-rw-r--r--   0        0        0    26740 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/schema_tester.py
+-rw-r--r--   0        0        0     2197 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/utils.py
+-rw-r--r--   0        0        0     8559 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/openapi_tester/validators.py
+-rw-r--r--   0        0        0     4045 2024-04-04 16:27:27.397993 django_contract_tester-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    10900 1970-01-01 00:00:00.000000 django_contract_tester-1.3.1/PKG-INFO
```

### Comparing `django_contract_tester-1.3.0/CHANGELOG.md` & `django_contract_tester-1.3.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.0/LICENSE` & `django_contract_tester-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.0/README.md` & `django_contract_tester-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_contract_tester-1.3.0/openapi_tester/__init__.py` & `django_contract_tester-1.3.1/openapi_tester/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-""" Django OpenAPI Schema Tester """
+"""Django OpenAPI Schema Tester"""
 
 from .case_testers import is_camel_case, is_kebab_case, is_pascal_case, is_snake_case
 from .clients import OpenAPIClient
-from .loaders import BaseSchemaLoader, DrfSpectacularSchemaLoader, DrfYasgSchemaLoader, StaticSchemaLoader
+from .loaders import (
+    BaseSchemaLoader,
+    DrfSpectacularSchemaLoader,
+    DrfYasgSchemaLoader,
+    StaticSchemaLoader,
+)
 from .schema_tester import SchemaTester
 
 __all__ = [
     "BaseSchemaLoader",
     "DrfSpectacularSchemaLoader",
     "DrfYasgSchemaLoader",
     "SchemaTester",
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/case_testers.py` & `django_contract_tester-1.3.1/openapi_tester/case_testers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Case testers - this module includes helper functions to test key casing """
+"""Case testers - this module includes helper functions to test key casing"""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from inflection import camelize, dasherize, underscore
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/constants.py` & `django_contract_tester-1.3.1/openapi_tester/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-""" Constants module """
+"""Constants module"""
 
 OPENAPI_PYTHON_MAPPING = {
     "boolean": bool.__name__,
     "string": str.__name__,
     "file": str.__name__,
     "array": list.__name__,
     "object": dict.__name__,
     "integer": int.__name__,
     "number": f"{int.__name__} or {float.__name__}",
 }
 
 # Validation errors
-VALIDATE_FORMAT_ERROR = 'Expected: {article} "{format}" formatted value\n\nReceived: {received}'
-VALIDATE_PATTERN_ERROR = 'The string "{data}" does not match the specified pattern: {pattern}'
+VALIDATE_FORMAT_ERROR = (
+    'Expected: {article} "{format}" formatted value\n\nReceived: {received}'
+)
+VALIDATE_PATTERN_ERROR = (
+    'The string "{data}" does not match the specified pattern: {pattern}'
+)
 INVALID_PATTERN_ERROR = "String pattern is not valid regex: {pattern}"
 VALIDATE_ENUM_ERROR = "Expected: a member of the enum {enum}\n\nReceived: {received}"
 VALIDATE_TYPE_ERROR = 'Expected: {article} "{type}" type value\n\nReceived: {received}'
 VALIDATE_MULTIPLE_OF_ERROR = "The value {data} should be a multiple of {multiple}"
-VALIDATE_MINIMUM_ERROR = "The value {data} is lower than the specified minimum of {minimum}"
-VALIDATE_MAXIMUM_ERROR = "The value {data} exceeds the maximum allowed value of {maximum}"
-VALIDATE_MIN_LENGTH_ERROR = 'The length of "{data}" is shorter than the specified minimum length of {min_length}'
-VALIDATE_MAX_LENGTH_ERROR = 'The length of "{data}" exceeds the specified maximum length of {max_length}'
-VALIDATE_MIN_ARRAY_LENGTH_ERROR = (
-    "The length of the array {data} is shorter than the specified minimum length of {min_length}"
+VALIDATE_MINIMUM_ERROR = (
+    "The value {data} is lower than the specified minimum of {minimum}"
 )
-VALIDATE_MAX_ARRAY_LENGTH_ERROR = "The length of the array {data} exceeds the specified maximum length of {max_length}"
-VALIDATE_MINIMUM_NUMBER_OF_PROPERTIES_ERROR = (
-    "The number of properties in {data} is fewer than the specified minimum number of properties of {min_length}"
+VALIDATE_MAXIMUM_ERROR = (
+    "The value {data} exceeds the maximum allowed value of {maximum}"
 )
-VALIDATE_MAXIMUM_NUMBER_OF_PROPERTIES_ERROR = (
-    "The number of properties in {data} exceeds the specified maximum number of properties of {max_length}"
+VALIDATE_MIN_LENGTH_ERROR = 'The length of "{data}" is shorter than the specified minimum length of {min_length}'
+VALIDATE_MAX_LENGTH_ERROR = (
+    'The length of "{data}" exceeds the specified maximum length of {max_length}'
 )
+VALIDATE_MIN_ARRAY_LENGTH_ERROR = "The length of the array {data} is shorter than the specified minimum length of {min_length}"
+VALIDATE_MAX_ARRAY_LENGTH_ERROR = "The length of the array {data} exceeds the specified maximum length of {max_length}"
+VALIDATE_MINIMUM_NUMBER_OF_PROPERTIES_ERROR = "The number of properties in {data} is fewer than the specified minimum number of properties of {min_length}"
+VALIDATE_MAXIMUM_NUMBER_OF_PROPERTIES_ERROR = "The number of properties in {data} exceeds the specified maximum number of properties of {max_length}"
 VALIDATE_UNIQUE_ITEMS_ERROR = "The array {data} must contain unique items only"
-VALIDATE_NONE_ERROR = "Received a null value for a non-nullable schema object"
-VALIDATE_MISSING_KEY_ERROR = 'The following property is missing in the {http_message} data: "{missing_key}"'
-VALIDATE_EXCESS_KEY_ERROR = (
-    'The following property was found in the {http_message}, but is missing from the schema definition: "{excess_key}"'
+VALIDATE_NONE_ERROR = "A property received a null value in the {http_message} data, but is a non-nullable object in the schema definition"
+VALIDATE_MISSING_KEY_ERROR = (
+    "The following property was found in the schema definition, "
+    'but is missing from the {http_message} data: "{missing_key}"'
 )
-VALIDATE_WRITE_ONLY_RESPONSE_KEY_ERROR = (
-    'The following property was found in the response, but is documented as being "writeOnly": "{write_only_key}"'
+VALIDATE_EXCESS_KEY_ERROR = (
+    "The following property was found in the {http_message} data, "
+    'but is missing from the schema definition: "{excess_key}"'
 )
+VALIDATE_WRITE_ONLY_RESPONSE_KEY_ERROR = 'The following property was found in the response, but is documented as being "writeOnly": "{write_only_key}"'
 VALIDATE_ONE_OF_ERROR = "Expected data to match one and only one of the oneOf schema types; found {matches} matches"
 VALIDATE_ANY_OF_ERROR = "Expected data to match one or more of the documented anyOf schema types, but found no matches"
-UNDOCUMENTED_SCHEMA_SECTION_ERROR = "Error: Unsuccessfully tried to index the OpenAPI schema by `{key}`. {error_addon}"
+UNDOCUMENTED_SCHEMA_SECTION_ERROR = (
+    "Error: Unsuccessfully tried to index the OpenAPI schema by `{key}`. {error_addon}"
+)
 INIT_ERROR = "Unable to configure loader"
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/exceptions.py` & `django_contract_tester-1.3.1/openapi_tester/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Exceptions Module """
+"""Exceptions Module"""
 
 
 class DocumentationError(AssertionError):
     """
     Custom exception raised when package tests fail.
     """
 
@@ -11,15 +11,17 @@
 
 class CaseError(DocumentationError):
     """
     Custom exception raised when items are not cased correctly.
     """
 
     def __init__(self, key: str, case: str, expected: str) -> None:
-        super().__init__(f"The response key `{key}` is not properly {case}. Expected value: {expected}")
+        super().__init__(
+            f"The response key `{key}` is not properly {case}. Expected value: {expected}"
+        )
 
 
 class OpenAPISchemaError(Exception):
     """
     Custom exception raised for invalid schema specifications.
     """
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/loaders.py` & `django_contract_tester-1.3.1/openapi_tester/loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Loaders Module """
+"""Loaders Module"""
 
 from __future__ import annotations
 
 import difflib
 import json
 import pathlib
 import re
@@ -10,15 +10,19 @@
 from typing import TYPE_CHECKING, cast
 from urllib.parse import urlparse
 
 import requests
 import yaml
 from django.urls import Resolver404, resolve
 from django.utils.functional import cached_property
-from openapi_spec_validator import OpenAPIV2SpecValidator, OpenAPIV30SpecValidator, OpenAPIV31SpecValidator
+from openapi_spec_validator import (
+    OpenAPIV2SpecValidator,
+    OpenAPIV30SpecValidator,
+    OpenAPIV31SpecValidator,
+)
 from prance.util.resolver import RefResolver
 from rest_framework.schemas.generators import BaseSchemaGenerator, EndpointEnumerator
 from rest_framework.settings import api_settings
 
 from openapi_tester.constants import UNDOCUMENTED_SCHEMA_SECTION_ERROR
 from openapi_tester.exceptions import UndocumentedSchemaSectionError
 
@@ -91,15 +95,17 @@
         resolver.resolve_references()
         return resolver.specs
 
     def normalize_schema_paths(self, schema: dict) -> dict[str, dict]:
         normalized_paths: dict[str, dict] = {}
         for key, value in schema["paths"].items():
             try:
-                parameterized_path, _ = self.resolve_path(endpoint_path=key, method=list(value.keys())[0])
+                parameterized_path, _ = self.resolve_path(
+                    endpoint_path=key, method=list(value.keys())[0]
+                )
                 normalized_paths[parameterized_path] = value
             except ValueError:
                 normalized_paths[key] = value
         return {**schema, "paths": normalized_paths}
 
     @staticmethod
     def validate_schema(schema: dict):
@@ -111,19 +117,22 @@
                 if (major, minor) == ("3", "0"):
                     validator = OpenAPIV30SpecValidator(schema=schema)
                 elif (major, minor) == ("3", "1"):
                     validator = OpenAPIV31SpecValidator(schema=schema)
                 else:
                     raise UndocumentedSchemaSectionError(
                         UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(
-                            key=schema["openapi"], error_addon="Support might need to be added."
+                            key=schema["openapi"],
+                            error_addon="Support might need to be added.",
                         )
                     )
             else:
-                raise UndocumentedSchemaSectionError(UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(key=schema["openapi"]))
+                raise UndocumentedSchemaSectionError(
+                    UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(key=schema["openapi"])
+                )
         else:
             validator = OpenAPIV2SpecValidator(schema=schema)
         validator.validate()
 
     def set_schema(self, schema: dict) -> None:
         """
         Sets self.schema and self.original_schema.
@@ -134,17 +143,21 @@
         self.schema = self.normalize_schema_paths(de_referenced_schema)
 
     @cached_property
     def endpoints(self) -> list[str]:
         """
         Returns a list of endpoint paths.
         """
-        return list({endpoint[0] for endpoint in EndpointEnumerator().get_api_endpoints()})
+        return list(
+            {endpoint[0] for endpoint in EndpointEnumerator().get_api_endpoints()}
+        )
 
-    def resolve_path(self, endpoint_path: str, method: str) -> tuple[str, ResolverMatch]:
+    def resolve_path(
+        self, endpoint_path: str, method: str
+    ) -> tuple[str, ResolverMatch]:
         """
         Resolves a Django path.
         """
         url_object = urlparse(endpoint_path)
         parsed_path = url_object.path
         if not parsed_path.startswith("/"):
             parsed_path = "/" + parsed_path
@@ -164,27 +177,33 @@
                     path, resolved_route = self.handle_pk_parameter(
                         resolved_route=resolved_route, path=path, method=method
                     )
                 return path, resolved_route
         message = f"Could not resolve path `{endpoint_path}`."
         close_matches = difflib.get_close_matches(endpoint_path, self.endpoints)
         if close_matches:
-            message += "\n\nDid you mean one of these?\n\n- " + "\n- ".join(close_matches)
+            message += "\n\nDid you mean one of these?\n\n- " + "\n- ".join(
+                close_matches
+            )
         raise ValueError(message)
 
     @staticmethod
-    def handle_pk_parameter(resolved_route: ResolverMatch, path: str, method: str) -> tuple[str, ResolverMatch]:
+    def handle_pk_parameter(
+        resolved_route: ResolverMatch, path: str, method: str
+    ) -> tuple[str, ResolverMatch]:
         """
         Handle the DRF conversion of params called {pk} into a named parameter based on Model field
         """
         coerced_path = BaseSchemaGenerator().coerce_path(
             path=path, method=method, view=cast("APIView", resolved_route.func)
         )
         pk_field_name = "".join(
-            entry.replace("+ ", "") for entry in difflib.Differ().compare(path, coerced_path) if "+ " in entry
+            entry.replace("+ ", "")
+            for entry in difflib.Differ().compare(path, coerced_path)
+            if "+ " in entry
         )
         resolved_route.kwargs[pk_field_name] = resolved_route.kwargs["pk"]
         del resolved_route.kwargs["pk"]
         return coerced_path, resolved_route
 
 
 class DrfYasgSchemaLoader(BaseSchemaLoader):
@@ -193,25 +212,31 @@
     """
 
     def __init__(self, field_key_map: dict[str, str] | None = None) -> None:
         super().__init__(field_key_map=field_key_map)
         from drf_yasg.generators import OpenAPISchemaGenerator
         from drf_yasg.openapi import Info
 
-        self.schema_generator = OpenAPISchemaGenerator(info=Info(title="", default_version=""))
+        self.schema_generator = OpenAPISchemaGenerator(
+            info=Info(title="", default_version="")
+        )
 
     def load_schema(self) -> dict:
         """
         Loads generated schema from drf-yasg and returns it as a dict.
         """
         odict_schema = self.schema_generator.get_schema(None, True)
         return cast("dict", loads(dumps(odict_schema.as_odict())))
 
-    def resolve_path(self, endpoint_path: str, method: str) -> tuple[str, ResolverMatch]:
-        de_parameterized_path, resolved_path = super().resolve_path(endpoint_path=endpoint_path, method=method)
+    def resolve_path(
+        self, endpoint_path: str, method: str
+    ) -> tuple[str, ResolverMatch]:
+        de_parameterized_path, resolved_path = super().resolve_path(
+            endpoint_path=endpoint_path, method=method
+        )
         path_prefix = self.schema_generator.determine_path_prefix(self.endpoints)
         trim_length = len(path_prefix) if path_prefix != "/" else 0
         return de_parameterized_path[trim_length:], resolved_path
 
 
 class DrfSpectacularSchemaLoader(BaseSchemaLoader):
     """
@@ -226,18 +251,22 @@
 
     def load_schema(self) -> dict:
         """
         Loads generated schema from drf_spectacular and returns it as a dict.
         """
         return cast("dict", loads(dumps(self.schema_generator.get_schema(public=True))))
 
-    def resolve_path(self, endpoint_path: str, method: str) -> tuple[str, ResolverMatch]:
+    def resolve_path(
+        self, endpoint_path: str, method: str
+    ) -> tuple[str, ResolverMatch]:
         from drf_spectacular.settings import spectacular_settings
 
-        de_parameterized_path, resolved_path = super().resolve_path(endpoint_path=endpoint_path, method=method)
+        de_parameterized_path, resolved_path = super().resolve_path(
+            endpoint_path=endpoint_path, method=method
+        )
         return (
             de_parameterized_path[len(spectacular_settings.SCHEMA_PATH_PREFIX or "") :],
             resolved_path,
         )
 
 
 class StaticSchemaLoader(BaseSchemaLoader):
@@ -256,15 +285,18 @@
 
         :return: Schema contents as a dict
         :raises: ImproperlyConfigured
         """
         with open(self.path, encoding="utf-8") as file:
             content = file.read()
             return cast(
-                "dict", json.loads(content) if ".json" in self.path else yaml.load(content, Loader=yaml.FullLoader)
+                "dict",
+                json.loads(content)
+                if ".json" in self.path
+                else yaml.load(content, Loader=yaml.FullLoader),
             )
 
 
 class UrlStaticSchemaLoader(BaseSchemaLoader):
     """
     Loads OpenAPI schema from an url static file.
     """
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/response_handler.py` & `django_contract_tester-1.3.1/openapi_tester/response_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,18 @@
         self._response = response
 
     @property
     def response(self) -> Union["Response", "HttpResponse"]:
         return self._response
 
     @property
-    def data(self) -> Optional[dict]:
-        ...
+    def data(self) -> Optional[dict]: ...
 
     @property
-    def request_data(self) -> Optional[dict]:
-        ...
+    def request_data(self) -> Optional[dict]: ...
 
 
 class DRFResponseHandler(ResponseHandler):
     """
     Handles the response and request data from DRF responses.
     """
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/response_handler_factory.py` & `django_contract_tester-1.3.1/openapi_tester/response_handler_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # pylint: disable=R0903
 """
-  Module that contains the factory to create response handlers.
+Module that contains the factory to create response handlers.
 """
 
 from typing import TYPE_CHECKING, Union
 
 from rest_framework.response import Response
 
-from openapi_tester.response_handler import DjangoNinjaResponseHandler, DRFResponseHandler
+from openapi_tester.response_handler import (
+    DjangoNinjaResponseHandler,
+    DRFResponseHandler,
+)
 
 if TYPE_CHECKING:
     from django.http.response import HttpResponse
 
     from openapi_tester.response_handler import ResponseHandler
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/schema_tester.py` & `django_contract_tester-1.3.1/openapi_tester/schema_tester.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-""" Schema Tester """
+"""Schema Tester"""
 
 from __future__ import annotations
 
+import json
 import re
+from copy import copy
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Callable, cast
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.core.validators import URLValidator
 
@@ -17,15 +19,19 @@
     VALIDATE_ANY_OF_ERROR,
     VALIDATE_EXCESS_KEY_ERROR,
     VALIDATE_MISSING_KEY_ERROR,
     VALIDATE_NONE_ERROR,
     VALIDATE_ONE_OF_ERROR,
     VALIDATE_WRITE_ONLY_RESPONSE_KEY_ERROR,
 )
-from openapi_tester.exceptions import DocumentationError, OpenAPISchemaError, UndocumentedSchemaSectionError
+from openapi_tester.exceptions import (
+    DocumentationError,
+    OpenAPISchemaError,
+    UndocumentedSchemaSectionError,
+)
 from openapi_tester.loaders import (
     DrfSpectacularSchemaLoader,
     DrfYasgSchemaLoader,
     StaticSchemaLoader,
     UrlStaticSchemaLoader,
 )
 from openapi_tester.response_handler_factory import ResponseHandlerFactory
@@ -55,15 +61,20 @@
 
     from openapi_tester.response_handler import ResponseHandler
 
 
 class SchemaTester:
     """Schema Tester: this is the base class of the library."""
 
-    loader: StaticSchemaLoader | DrfSpectacularSchemaLoader | DrfYasgSchemaLoader | UrlStaticSchemaLoader
+    loader: (
+        StaticSchemaLoader
+        | DrfSpectacularSchemaLoader
+        | DrfYasgSchemaLoader
+        | UrlStaticSchemaLoader
+    )
     validators: list[Callable[[dict, Any], str | None]]
 
     def __init__(
         self,
         case_tester: Callable[[str], None] | None = None,
         ignore_case: list[str] | None = None,
         schema_file_path: str | None = None,
@@ -84,198 +95,251 @@
         self._path_prefix = path_prefix
         self.ignore_case = ignore_case or []
         self.validators = validators or []
 
         if schema_file_path is not None:
             try:
                 URLValidator()(schema_file_path)
-                self.loader = UrlStaticSchemaLoader(schema_file_path, field_key_map=field_key_map)
+                self.loader = UrlStaticSchemaLoader(
+                    schema_file_path, field_key_map=field_key_map
+                )
             except ValidationError:
-                self.loader = StaticSchemaLoader(schema_file_path, field_key_map=field_key_map)
+                self.loader = StaticSchemaLoader(
+                    schema_file_path, field_key_map=field_key_map
+                )
         elif "drf_spectacular" in settings.INSTALLED_APPS:
             self.loader = DrfSpectacularSchemaLoader(field_key_map=field_key_map)
         elif "drf_yasg" in settings.INSTALLED_APPS:
             self.loader = DrfYasgSchemaLoader(field_key_map=field_key_map)
         else:
             raise ImproperlyConfigured(INIT_ERROR)
 
     @staticmethod
-    def get_key_value(schema: dict[str, dict], key: str, error_addon: str = "", use_regex=False) -> dict:
+    def get_key_value(
+        schema: dict[str, dict], key: str, error_addon: str = "", use_regex=False
+    ) -> dict:
         """
         Returns the value of a given key
         """
         try:
             if use_regex:
                 compiled_pattern = re.compile(key)
                 for key_ in schema.keys():
                     if compiled_pattern.match(key_):
                         return schema[key_]
             return schema[key]
         except KeyError as e:
             raise UndocumentedSchemaSectionError(
-                UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(key=key, error_addon=error_addon)
+                UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(
+                    key=key, error_addon=error_addon
+                )
             ) from e
 
     @staticmethod
-    def get_status_code(schema: dict[str | int, dict], status_code: str | int, error_addon: str = "") -> dict:
+    def get_status_code(
+        schema: dict[str | int, dict], status_code: str | int, error_addon: str = ""
+    ) -> dict:
         """
         Returns the status code section of a schema, handles both str and int status codes
         """
         if str(status_code) in schema:
             return schema[str(status_code)]
         if int(status_code) in schema:
             return schema[int(status_code)]
         raise UndocumentedSchemaSectionError(
-            UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(key=status_code, error_addon=error_addon)
+            UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(
+                key=status_code, error_addon=error_addon
+            )
         )
 
     @staticmethod
     def get_schema_type(schema: dict[str, str]) -> str | None:
         if "type" in schema:
             return schema["type"]
         if "properties" in schema or "additionalProperties" in schema:
             return "object"
         return None
 
     def get_paths_object(self) -> dict[str, Any]:
         schema = self.loader.get_schema()
         paths_object = self.get_key_value(schema, "paths")
         if self._path_prefix:
-            paths_object = {f"{self._path_prefix}{key}": value for key, value in paths_object.items()}
+            paths_object = {
+                f"{self._path_prefix}{key}": value
+                for key, value in paths_object.items()
+            }
 
         return paths_object
 
-    def get_response_schema_section(self, response_handler: ResponseHandler) -> dict[str, Any]:
+    def get_response_schema_section(
+        self, response_handler: ResponseHandler, test_config: OpenAPITestConfig
+    ) -> dict[str, Any]:
         """
         Fetches the response section of a schema, wrt. the route, method, status code, and schema version.
 
         :param response: DRF Response Instance
         :return dict
         """
         response = response_handler.response
         schema = self.loader.get_schema()
 
         response_method = response.request["REQUEST_METHOD"].lower()  # type: ignore
         parameterized_path, _ = self.loader.resolve_path(
-            response.request["PATH_INFO"], method=response_method  # type: ignore
+            response.request["PATH_INFO"],  # type: ignore
+            method=response_method,
         )
         paths_object = self.get_paths_object()
 
         route_object = self.get_key_value(
             paths_object,
             parameterized_path,
-            f"\n\nUndocumented route {parameterized_path}.\n\nDocumented routes: " + "\n\t• ".join(paths_object.keys()),
+            (
+                f"\n\n{test_config.reference}\n\nUndocumented route {parameterized_path}.\n\nDocumented routes: "
+                + "\n\t• ".join(paths_object.keys())
+            ),
         )
 
         method_object = self.get_key_value(
             route_object,
             response_method,
             (
-                f"\n\nUndocumented method: {response_method}.\n\nDocumented methods: "
+                f"\n\n{test_config.reference}"
+                f"\n\nUndocumented method: {response_method}."
+                "\n\nDocumented methods: "
                 f"{[method.lower() for method in route_object.keys() if method.lower() != 'parameters']}."
             ),
         )
 
         responses_object = self.get_key_value(method_object, "responses")
         status_code_object = self.get_status_code(
             responses_object,
             response.status_code,
             (
-                f"\n\nUndocumented status code: {response.status_code}.\n\n"
-                f"Documented status codes: {list(responses_object.keys())}. "
+                f"\n\n{test_config.reference}"
+                f"\n\nUndocumented status code: {response.status_code}."
+                f"\n\nDocumented status codes: {list(responses_object.keys())}. "
             ),
         )
 
         if "openapi" not in schema:
             # openapi 2.0, i.e. "swagger" has a different structure than openapi 3.0 status sub-schemas
             return self.get_key_value(status_code_object, "schema")
 
         if status_code_object.get("content"):
             content_object = self.get_key_value(
                 status_code_object,
                 "content",
-                f"\n\nNo content documented for method: {response_method}, path: {parameterized_path}",
+                (
+                    f"\n\n{test_config.reference}"
+                    f"\n\nNo content documented for method: {response_method}, path: {parameterized_path}"
+                ),
             )
             json_object = self.get_key_value(
                 content_object,
                 r"^application\/.*json$",
                 (
+                    f"\n\n{test_config.reference}"
                     "\n\nNo `application/json` responses documented for method: "
                     f"{response_method}, path: {parameterized_path}"
                 ),
                 use_regex=True,
             )
             return self.get_key_value(json_object, "schema")
 
         if response_handler.data:
             raise UndocumentedSchemaSectionError(
                 UNDOCUMENTED_SCHEMA_SECTION_ERROR.format(
                     key="content",
                     error_addon=(
+                        f"\n\n{test_config.reference}"
                         f"\n\nNo `content` defined for this response: {response_method}, path: {parameterized_path}"
                     ),
                 )
             )
         return {}
 
-    def get_request_body_schema_section(self, request: dict[str, Any]) -> dict[str, Any]:
+    def get_request_body_schema_section(
+        self, request: dict[str, Any], test_config: OpenAPITestConfig
+    ) -> dict[str, Any]:
         """
         Fetches the request section of a schema.
 
         :param response: DRF Request Instance
         :return dict
         """
         request_method = request["REQUEST_METHOD"].lower()
 
-        parameterized_path, _ = self.loader.resolve_path(request["PATH_INFO"], method=request_method)
+        parameterized_path, _ = self.loader.resolve_path(
+            request["PATH_INFO"], method=request_method
+        )
         paths_object = self.get_paths_object()
 
         route_object = self.get_key_value(
             paths_object,
             parameterized_path,
-            f"\n\nUndocumented route {parameterized_path}.\n\nDocumented routes: " + "\n\t• ".join(paths_object.keys()),
+            (
+                f"\n\n{test_config.reference}\n\nUndocumented route {parameterized_path}.\n\nDocumented routes: "
+                + "\n\t• ".join(paths_object.keys())
+            ),
         )
 
         method_object = self.get_key_value(
             route_object,
             request_method,
             (
-                f"\n\nUndocumented method: {request_method}.\n\nDocumented methods: "
+                f"\n\n{test_config.reference}"
+                f"\n\nUndocumented method: {request_method}."
+                "\n\nDocumented methods: "
                 f"{[method.lower() for method in route_object.keys() if method.lower() != 'parameters']}."
             ),
         )
 
-        if all(key in request for key in ["CONTENT_LENGTH", "CONTENT_TYPE", "wsgi.input"]):
+        if all(
+            key in request for key in ["CONTENT_LENGTH", "CONTENT_TYPE", "wsgi.input"]
+        ):
             if request["CONTENT_TYPE"] != "application/json":
                 return {}
 
             request_body_object = self.get_key_value(
                 method_object,
                 "requestBody",
-                f"\n\nNo request body documented for method: {request_method}, path: {parameterized_path}",
+                (
+                    f"\n\n{test_config.reference}"
+                    f"\n\nNo request body documented for method: {request_method}, path: {parameterized_path}"
+                ),
             )
             content_object = self.get_key_value(
                 request_body_object,
                 "content",
-                f"\n\nNo content documented for method: {request_method}, path: {parameterized_path}",
+                (
+                    f"\n\n{test_config.reference}"
+                    f"\n\nNo content documented for method: {request_method}, path: {parameterized_path}"
+                ),
             )
             json_object = self.get_key_value(
                 content_object,
                 r"^application\/.*json$",
                 (
+                    f"\n\n{test_config.reference}"
                     "\n\nNo `application/json` requests documented for method: "
                     f"{request_method}, path: {parameterized_path}"
                 ),
                 use_regex=True,
             )
             return self.get_key_value(json_object, "schema")
 
         return {}
 
-    def handle_one_of(self, schema_section: dict, data: Any, reference: str, test_config: OpenAPITestConfig) -> None:
+    def handle_one_of(
+        self,
+        schema_section: dict,
+        data: Any,
+        reference: str,
+        test_config: OpenAPITestConfig,
+    ) -> None:
         matches = 0
         passed_schema_section_formats = set()
         for option in schema_section["oneOf"]:
             try:
                 test_config.reference = f"{test_config.reference}.oneOf"
                 self.test_schema_section(
                     schema_section=option,
@@ -288,30 +352,40 @@
                 continue
         if matches == 2 and passed_schema_section_formats == {"date", "date-time"}:
             # With Django v4, the datetime validator now parses normal
             # date formats successfully, so a oneOf: date // datetime section
             # will succeed twice where it used to succeed once.
             return
         if matches != 1:
-            raise DocumentationError(f"{VALIDATE_ONE_OF_ERROR.format(matches=matches)}\n\nReference: {reference}.oneOf")
+            raise DocumentationError(
+                f"{VALIDATE_ONE_OF_ERROR.format(matches=matches)}\n\nReference: {reference}.oneOf"
+            )
 
-    def handle_any_of(self, schema_section: dict, data: Any, reference: str, test_config: OpenAPITestConfig) -> None:
+    def handle_any_of(
+        self,
+        schema_section: dict,
+        data: Any,
+        reference: str,
+        test_config: OpenAPITestConfig,
+    ) -> None:
         any_of: list[dict[str, Any]] = schema_section.get("anyOf", [])
         for schema in chain(any_of, lazy_combinations(any_of)):
             test_config.reference = f"{test_config.reference}.anyOf"
             try:
                 self.test_schema_section(
                     schema_section=schema,
                     data=data,
                     test_config=test_config,
                 )
                 return
             except DocumentationError:
                 continue
-        raise DocumentationError(f"{VALIDATE_ANY_OF_ERROR}\n\nReference: {reference}.anyOf")
+        raise DocumentationError(
+            f"{VALIDATE_ANY_OF_ERROR}\n\nReference: {reference}.anyOf"
+        )
 
     def is_openapi_schema(self) -> bool:
         return self.loader.get_schema().get("openapi") is not None
 
     @staticmethod
     def test_is_nullable(schema_item: dict) -> bool:
         """
@@ -321,28 +395,33 @@
         OpenApi 2 ref: https://help.apiary.io/api_101/swagger-extensions/
 
         :param schema_item: schema item
         :return: whether or not the item can be None
         """
         openapi_schema_3_nullable = "nullable"
         swagger_2_nullable = "x-nullable"
+        openapi_schema_3_1_type_nullable = "null"
         if "oneOf" in schema_item:
             one_of: list[dict[str, Any]] = schema_item.get("oneOf", [])
             return any(
                 nullable_key in schema and schema[nullable_key]
                 for schema in one_of
                 for nullable_key in [openapi_schema_3_nullable, swagger_2_nullable]
             )
         if "anyOf" in schema_item:
             any_of: list[dict[str, Any]] = schema_item.get("anyOf", [])
             return any(
                 nullable_key in schema and schema[nullable_key]
                 for schema in any_of
                 for nullable_key in [openapi_schema_3_nullable, swagger_2_nullable]
             )
+        if "type" in schema_item and isinstance(schema_item["type"], list):
+            types: list[str] = schema_item["type"]
+            return openapi_schema_3_1_type_nullable in types
+
         return any(
             nullable_key in schema_item and schema_item[nullable_key]
             for nullable_key in [openapi_schema_3_nullable, swagger_2_nullable]
         )
 
     def test_key_casing(
         self,
@@ -366,27 +445,35 @@
         """
         test_config = test_config or OpenAPITestConfig()
         if data is None:
             if self.test_is_nullable(schema_section) or not schema_section:
                 # If data is None and nullable, we return early
                 return
             raise DocumentationError(
-                f"{VALIDATE_NONE_ERROR}\n\n"
-                f"Reference: {test_config.reference}\n\n"
-                "Hint: Return a valid type, or document the value as nullable"
+                f"{VALIDATE_NONE_ERROR.format(http_message=test_config.http_message)}"
+                "\n\nReference:"
+                f"\n\n{test_config.reference}"
+                f"\n\nSchema description:\n  {json.dumps(schema_section, indent=4)}"
+                "\n\nHint: Return a valid type, or document the value as nullable"
             )
         schema_section = normalize_schema_section(schema_section)
         if "oneOf" in schema_section:
             self.handle_one_of(
-                schema_section=schema_section, data=data, reference=test_config.reference, test_config=test_config
+                schema_section=schema_section,
+                data=data,
+                reference=test_config.reference,
+                test_config=test_config,
             )
             return
         if "anyOf" in schema_section:
             self.handle_any_of(
-                schema_section=schema_section, data=data, reference=test_config.reference, test_config=test_config
+                schema_section=schema_section,
+                data=data,
+                reference=test_config.reference,
+                test_config=test_config,
             )
             return
 
         schema_section_type = self.get_schema_type(schema_section)
         if not schema_section_type:
             return
         combined_validators = cast(
@@ -409,90 +496,123 @@
                 *self.validators,
                 *(test_config.validators or []),
             ],
         )
         for validator in combined_validators:
             error = validator(schema_section, data)
             if error:
-                raise DocumentationError(f"\n\n{error}\n\nReference: {test_config.reference}")
+                raise DocumentationError(
+                    f"\n\n{error}"
+                    "\n\nReference: "
+                    f"\n\n{test_config.reference}"
+                    f"\n\n {test_config.http_message.capitalize()} value:\n  {data}"
+                    f"\n Schema description:\n  {schema_section}"
+                )
 
         if schema_section_type == "object":
-            self.test_openapi_object(schema_section=schema_section, data=data, test_config=test_config)
+            self.test_openapi_object(
+                schema_section=schema_section, data=data, test_config=test_config
+            )
         elif schema_section_type == "array":
-            self.test_openapi_array(schema_section=schema_section, data=data, test_config=test_config)
+            self.test_openapi_array(
+                schema_section=schema_section, data=data, test_config=test_config
+            )
 
     def test_openapi_object(
         self,
         schema_section: dict,
         data: dict,
         test_config: OpenAPITestConfig,
     ) -> None:
         """
         1. Validate that casing is correct for both request/response and schema
         2. Check if any required key is missing from the request/response
         3. Check if any request/response key is not in the schema
         4. Validate sub-schema/nested data
         """
         properties = schema_section.get("properties", {})
-        write_only_properties = [key for key in properties.keys() if properties[key].get("writeOnly")]
-        required_keys = [key for key in schema_section.get("required", []) if key not in write_only_properties]
+        write_only_properties = [
+            key for key in properties.keys() if properties[key].get("writeOnly")
+        ]
+        required_keys = [
+            key
+            for key in schema_section.get("required", [])
+            if key not in write_only_properties
+        ]
         request_response_keys = data.keys()
-        additional_properties: bool | dict | None = schema_section.get("additionalProperties")
+        additional_properties: bool | dict | None = schema_section.get(
+            "additionalProperties"
+        )
         additional_properties_allowed = additional_properties is not None
-        if additional_properties_allowed and not isinstance(additional_properties, (bool, dict)):
+        if additional_properties_allowed and not isinstance(
+            additional_properties, (bool, dict)
+        ):
             raise OpenAPISchemaError("Invalid additionalProperties type")
         for key in properties.keys():
             self.test_key_casing(key, test_config.case_tester, test_config.ignore_case)
             if key in required_keys and key not in request_response_keys:
                 raise DocumentationError(
                     f"{VALIDATE_MISSING_KEY_ERROR.format(missing_key=key, http_message=test_config.http_message)}"
                     "\n\nReference:"
-                    f" {test_config.reference}.object:key:{key}\n\nHint: Remove the key from your OpenAPI docs, or"
+                    f"\n\n{test_config.reference} > {key}"
+                    f"\n\n{test_config.http_message.capitalize()} body:\n  {json.dumps(data, indent=4)}"
+                    f"\nSchema section:\n  {json.dumps(properties, indent=4)}"
+                    "\n\nHint: Remove the key from your OpenAPI docs, or"
                     f" include it in your API {test_config.http_message}"
                 )
         for key in request_response_keys:
             self.test_key_casing(key, test_config.case_tester, test_config.ignore_case)
             if key not in properties and not additional_properties_allowed:
                 raise DocumentationError(
                     f"{VALIDATE_EXCESS_KEY_ERROR.format(excess_key=key, http_message=test_config.http_message)}"
                     "\n\nReference:"
-                    f" {test_config.reference}.object:key:{key}\n\nHint: Remove the key from your API"
+                    f"\n\n{test_config.reference} > {key}"
+                    f"\n\n{test_config.http_message.capitalize()} body:\n  {json.dumps(data, indent=4)}"
+                    f"\n\nSchema section:\n  {json.dumps(properties, indent=4)}"
+                    "\n\nHint: Remove the key from your API"
                     f" {test_config.http_message}, or include it in your OpenAPI docs"
                 )
             if key in write_only_properties:
                 raise DocumentationError(
                     f"{VALIDATE_WRITE_ONLY_RESPONSE_KEY_ERROR.format(write_only_key=key)}\n\nReference:"
-                    f" {test_config.reference}.object:key:{key}\n\nHint:"
-                    f" Remove the key from your API {test_config.http_message}, or"
+                    f"\n\n{test_config.reference} > {key}"
+                    f"\n\n{test_config.http_message.capitalize()} body:\n  {json.dumps(data, indent=4)}"
+                    f"\nSchema section:\n  {json.dumps(properties, indent=4)}"
+                    f"\n\nHint: Remove the key from your API {test_config.http_message}, or"
                     ' remove the "WriteOnly" restriction'
                 )
         for key, value in data.items():
             if key in properties:
-                test_config.reference = f"{test_config.reference}.object:key:{key}"
+                drill_down_test_config = copy(test_config)
+                drill_down_test_config.reference = f"{test_config.reference} > {key}"
                 self.test_schema_section(
                     schema_section=properties[key],
                     data=value,
-                    test_config=test_config,
+                    test_config=drill_down_test_config,
                 )
             elif isinstance(additional_properties, dict):
-                test_config.reference = f"{test_config.reference}.object:key:{key}"
+                drill_down_test_config = copy(test_config)
+                drill_down_test_config.reference = f"{test_config.reference} > {key}"
                 self.test_schema_section(
                     schema_section=additional_properties,
                     data=value,
-                    test_config=test_config,
+                    test_config=drill_down_test_config,
                 )
 
-    def test_openapi_array(self, schema_section: dict[str, Any], data: dict, test_config: OpenAPITestConfig) -> None:
-        for datum in data:
-            test_config.reference = f"{test_config.reference}.array.item"
+    def test_openapi_array(
+        self, schema_section: dict[str, Any], data: dict, test_config: OpenAPITestConfig
+    ) -> None:
+        for array_item in data:
+            array_item_test_config = copy(test_config)
+            array_item_test_config.reference = f"{test_config.reference}"
             self.test_schema_section(
                 # the items keyword is required in arrays
                 schema_section=schema_section["items"],
-                data=datum,
-                test_config=test_config,
+                data=array_item,
+                test_config=array_item_test_config,
             )
 
     def validate_request(
         self,
         response: Response | HttpResponse,
         test_config: OpenAPITestConfig | None = None,
     ) -> None:
@@ -506,19 +626,25 @@
         :param **kwargs: Request keyword arguments
         :raises: ``openapi_tester.exceptions.DocumentationError`` for inconsistencies in the API response and schema.
                  ``openapi_tester.exceptions.CaseError`` for case errors.
         """
         response_handler = ResponseHandlerFactory.create(response)
         if self.is_openapi_schema():
             # TODO: Implement for other schema types
+            request = response.request  # type: ignore
             if test_config:
                 test_config.http_message = "request"
             else:
-                test_config = OpenAPITestConfig(http_message="request")
-            request_body_schema = self.get_request_body_schema_section(response.request)  # type: ignore
+                test_config = OpenAPITestConfig(
+                    http_message="request",
+                    reference=f"{request['REQUEST_METHOD']} {request['PATH_INFO']} > request",
+                )
+            request_body_schema = self.get_request_body_schema_section(
+                request, test_config=test_config
+            )
 
             if request_body_schema:
                 self.test_schema_section(
                     schema_section=request_body_schema,
                     data=response_handler.request_data,
                     test_config=test_config,
                 )
@@ -539,14 +665,20 @@
                  ``openapi_tester.exceptions.CaseError`` for case errors.
         """
         response_handler = ResponseHandlerFactory.create(response)
 
         if test_config:
             test_config.http_message = "response"
         else:
-            test_config = OpenAPITestConfig(http_message="response")
-        response_schema = self.get_response_schema_section(response_handler)
+            request = response.request  # type: ignore
+            test_config = OpenAPITestConfig(
+                http_message="response",
+                reference=f"{request['REQUEST_METHOD']} {request['PATH_INFO']} > response > {response.status_code}",
+            )
+        response_schema = self.get_response_schema_section(
+            response_handler, test_config=test_config
+        )
         self.test_schema_section(
             schema_section=response_schema,
             data=response_handler.data,
             test_config=test_config,
         )
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/utils.py` & `django_contract_tester-1.3.1/openapi_tester/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,18 @@
         # handle the way drf-spectacular is doing enums
         one_of = output.pop("oneOf")
         output = {**output, **merge_objects(one_of)}
     for key, value in output.items():
         if isinstance(value, dict):
             output[key] = normalize_schema_section(value)
         elif isinstance(value, list):
-            output[key] = [normalize_schema_section(entry) if isinstance(entry, dict) else entry for entry in value]
+            output[key] = [
+                normalize_schema_section(entry) if isinstance(entry, dict) else entry
+                for entry in value
+            ]
     return output
 
 
 def lazy_combinations(options_list: Sequence[dict[str, Any]]) -> Iterator[dict]:
     """
     Lazily evaluate possible combinations.
     """
```

### Comparing `django_contract_tester-1.3.0/openapi_tester/validators.py` & `django_contract_tester-1.3.1/openapi_tester/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-""" Schema Validators """
+"""Schema Validators"""
 
 from __future__ import annotations
 
 import base64
 import json
 import re
 from typing import TYPE_CHECKING
 from uuid import UUID
 
 from django.core.exceptions import ValidationError
-from django.core.validators import EmailValidator, URLValidator, validate_ipv4_address, validate_ipv6_address
+from django.core.validators import (
+    EmailValidator,
+    URLValidator,
+    validate_ipv4_address,
+    validate_ipv6_address,
+)
 from django.utils.dateparse import parse_date, parse_datetime, parse_time
 
 from openapi_tester.constants import (
     INVALID_PATTERN_ERROR,
     VALIDATE_ENUM_ERROR,
     VALIDATE_FORMAT_ERROR,
     VALIDATE_MAX_ARRAY_LENGTH_ERROR,
@@ -31,37 +36,45 @@
 )
 from openapi_tester.exceptions import OpenAPISchemaError
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
 
-def create_validator(validation_fn: Callable, wrap_as_validator: bool = False) -> Callable[[Any], bool]:
+def create_validator(
+    validation_fn: Callable, wrap_as_validator: bool = False
+) -> Callable[[Any], bool]:
     def wrapped(value: Any) -> bool:
         try:
             return bool(validation_fn(value)) or not wrap_as_validator
         except (ValueError, ValidationError):
             return False
 
     return wrapped
 
 
 number_format_validator = create_validator(
     lambda x: isinstance(x, float) if x != 0 else isinstance(x, (int, float)), True
 )
 
-base64_format_validator = create_validator(lambda x: base64.b64encode(base64.b64decode(x, validate=True)) == x)
+base64_format_validator = create_validator(
+    lambda x: base64.b64encode(base64.b64decode(x, validate=True)) == x
+)
 
 VALIDATOR_MAP: dict[str, Callable] = {
     # by type
     "string": create_validator(lambda x: isinstance(x, str), True),
     "file": create_validator(lambda x: isinstance(x, str), True),
     "boolean": create_validator(lambda x: isinstance(x, bool), True),
-    "integer": create_validator(lambda x: isinstance(x, int) and not isinstance(x, bool), True),
-    "number": create_validator(lambda x: isinstance(x, (float, int)) and not isinstance(x, bool), True),
+    "integer": create_validator(
+        lambda x: isinstance(x, int) and not isinstance(x, bool), True
+    ),
+    "number": create_validator(
+        lambda x: isinstance(x, (float, int)) and not isinstance(x, bool), True
+    ),
     "object": create_validator(lambda x: isinstance(x, dict), True),
     "array": create_validator(lambda x: isinstance(x, list), True),
     # by format
     "byte": base64_format_validator,
     "base64": base64_format_validator,
     "date": create_validator(parse_date, True),
     "date-time": create_validator(parse_datetime, True),
@@ -74,20 +87,31 @@
     "uri": create_validator(URLValidator()),
     "url": create_validator(URLValidator()),
     "uuid": create_validator(UUID),
 }
 
 
 def validate_type(schema_section: dict[str, Any], data: Any) -> str | None:
-    schema_type: str = schema_section.get("type", "object")
-    if not VALIDATOR_MAP[schema_type](data):
-        an_articles = ["integer", "object", "array"]
+    an_articles = ["integer", "object", "array"]
+    schema_types: str = schema_section.get("type", "object")
+    if isinstance(schema_types, list):
+        has_type = False
+        for schema_type in schema_types:
+            if VALIDATOR_MAP[schema_type](data):
+                return None
+        if not has_type:
+            return VALIDATE_TYPE_ERROR.format(
+                article="a" if schema_types not in an_articles else "an",
+                type=schema_types,
+                received=f'"{data}"' if isinstance(data, str) else data,
+            )
+    if not VALIDATOR_MAP[schema_types](data):
         return VALIDATE_TYPE_ERROR.format(
-            article="a" if schema_type not in an_articles else "an",
-            type=schema_type,
+            article="a" if schema_types not in an_articles else "an",
+            type=schema_types,
             received=f'"{data}"' if isinstance(data, str) else data,
         )
     return None
 
 
 def validate_format(schema_section: dict[str, Any], data: Any) -> str | None:
     schema_format: str = schema_section.get("format", "")
@@ -99,15 +123,17 @@
         )
     return None
 
 
 def validate_enum(schema_section: dict[str, Any], data: Any) -> str | None:
     enum = schema_section.get("enum")
     if enum and data not in enum:
-        return VALIDATE_ENUM_ERROR.format(enum=schema_section["enum"], received=f'"{data}"')
+        return VALIDATE_ENUM_ERROR.format(
+            enum=schema_section["enum"], received=f'"{data}"'
+        )
     return None
 
 
 def validate_pattern(schema_section: dict[str, Any], data: str) -> str | None:
     pattern = schema_section.get("pattern")
     if not pattern:
         return None
@@ -116,15 +142,17 @@
     except re.error as e:
         raise OpenAPISchemaError(INVALID_PATTERN_ERROR.format(pattern=pattern)) from e
     if not compiled_pattern.match(str(data)):
         return VALIDATE_PATTERN_ERROR.format(data=data, pattern=pattern)
     return None
 
 
-def validate_multiple_of(schema_section: dict[str, Any], data: int | float) -> str | None:
+def validate_multiple_of(
+    schema_section: dict[str, Any], data: int | float
+) -> str | None:
     multiple = schema_section.get("multipleOf")
     if multiple and data % multiple != 0:
         return VALIDATE_MULTIPLE_OF_ERROR.format(data=data, multiple=multiple)
     return None
 
 
 def validate_maximum(schema_section: dict[str, Any], data: int | float) -> str | None:
@@ -143,18 +171,23 @@
     if minimum and exclusive_minimum and data <= minimum:
         return VALIDATE_MINIMUM_ERROR.format(data=data, minimum=minimum + 1)
     if minimum and not exclusive_minimum and data < minimum:
         return VALIDATE_MINIMUM_ERROR.format(data=data, minimum=minimum)
     return None
 
 
-def validate_unique_items(schema_section: dict[str, Any], data: list[Any]) -> str | None:
+def validate_unique_items(
+    schema_section: dict[str, Any], data: list[Any]
+) -> str | None:
     unique_items = schema_section.get("uniqueItems")
     if unique_items:
-        comparison_data = (json.dumps(item, sort_keys=True) if isinstance(item, dict) else item for item in data)
+        comparison_data = (
+            json.dumps(item, sort_keys=True) if isinstance(item, dict) else item
+            for item in data
+        )
         if len(set(comparison_data)) != len(data):
             return VALIDATE_UNIQUE_ITEMS_ERROR.format(data=data)
     return None
 
 
 def validate_min_length(schema_section: dict[str, Any], data: str) -> str | None:
     min_length: int | None = schema_section.get("minLength")
@@ -183,16 +216,20 @@
         return VALIDATE_MAX_ARRAY_LENGTH_ERROR.format(data=data, max_length=max_length)
     return None
 
 
 def validate_min_properties(schema_section: dict[str, Any], data: dict) -> str | None:
     min_properties: int | None = schema_section.get("minProperties")
     if min_properties and len(data.keys()) < int(min_properties):
-        return VALIDATE_MINIMUM_NUMBER_OF_PROPERTIES_ERROR.format(data=data, min_length=min_properties)
+        return VALIDATE_MINIMUM_NUMBER_OF_PROPERTIES_ERROR.format(
+            data=data, min_length=min_properties
+        )
     return None
 
 
 def validate_max_properties(schema_section: dict[str, Any], data: dict) -> str | None:
     max_properties: int | None = schema_section.get("maxProperties")
     if max_properties and len(data.keys()) > int(max_properties):
-        return VALIDATE_MAXIMUM_NUMBER_OF_PROPERTIES_ERROR.format(data=data, max_length=max_properties)
+        return VALIDATE_MAXIMUM_NUMBER_OF_PROPERTIES_ERROR.format(
+            data=data, max_length=max_properties
+        )
     return None
```

### Comparing `django_contract_tester-1.3.0/pyproject.toml` & `django_contract_tester-1.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-contract-tester"
-version = "1.3.0"
+version = "1.3.1"
 description = "Test utility for validating OpenAPI response documentation"
 authors =["Matías Cárdenas <cardenasmatias.1990@gmail.com>", "Sondre Lillebø Gundersen <sondrelg@live.no>", "Na'aman Hirschfeld <nhirschfeld@gmail.com>"]
 license = "BSD-4-Clause"
 readme = "README.md"
 homepage = "https://github.com/maticardenas/django-contract-tester"
 repository = "https://github.com/maticardenas/django-contract-tester"
 documentation = "https://github.com/maticardenas/django-contract-tester"
@@ -24,14 +24,16 @@
     "Programming Language :: Python :: 3.11",
     "Framework :: Django",
     'Framework :: Django :: 3.0',
     'Framework :: Django :: 3.1',
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
+    'Framework :: Django :: 4.2',
+    'Framework :: Django :: 5.0',
     "Framework :: Pytest",
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Documentation",
     "Topic :: Software Development :: Testing",
@@ -43,16 +45,18 @@
 packages = [
     { include = "openapi_tester" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = [
-    { version = '^3', python = '<=3.8' },
-    { version = '^3 || ^4', python = '>=3.8' },
+    { version = '^4.2 || ^5', python = '>=3.11' },
+    { version = '^4.1 || ^5', python = '>=3.10, <3.11' },
+    { version = '^3 || ^4', python = '>=3.8, <3.10' },
+    { version = '^3', python = '<3.8' },
 ]
 djangorestframework = "*"
 inflection = "*"
 openapi-spec-validator = "^0.7.1"
 prance = "*"
 pyYAML = "*"
 drf-spectacular = { version = "*", optional = true }
@@ -68,28 +72,21 @@
 coverage = { extras = ["toml"], version = "^6" }
 Faker = "*"
 pre-commit = "*"
 pylint = "*"
 pytest = "*"
 pytest-django = "*"
 
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.3.5"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
-[tool.black]
-line-length = 120
-preview = true
-quiet = true
-include = '\.pyi?$'
-
-[tool.isort]
-profile = "black"
-line_length = 120
-
 [tool.pylint.FORMAT]
 max-line-length = 120
 
 [tool.pylint.MESSAGE_CONTROL]
 disable = """
     unsubscriptable-object,
     unnecessary-pass,
@@ -106,14 +103,30 @@
 max-returns = 21
 max-branches = 20
 max-locals = 20
 
 [tool.pylint.BASIC]
 good-names = "_,e,i"
 
+[tool.ruff]
+lint.select = [
+    "B",    # flake8-bugbear
+    "C",    # flake8-comprehensions
+    "E",    # pycodestyle errors
+    "F",    # pyflakes
+    "I",    # isort
+    "UP",   # pyupgrade
+    "W",    # pycodestyle warnings
+]
+lint.ignore = [
+    "E501", # line too long, handled by black
+    "B008", # do not perform function calls in argument defaults
+    "C901", # too complex
+]
+
 [tool.coverage.run]
 source = [
     "openapi_tester",
 ]
 omit = [
     "manage.py",
     "test_project/*",
```

### Comparing `django_contract_tester-1.3.0/PKG-INFO` & `django_contract_tester-1.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-contract-tester
-Version: 1.3.0
+Version: 1.3.1
 Summary: Test utility for validating OpenAPI response documentation
 Home-page: https://github.com/maticardenas/django-contract-tester
 License: BSD-4-Clause
 Keywords: openapi,swagger,api,testing,schema,django,drf
 Author: Matías Cárdenas
 Author-email: cardenasmatias.1990@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,14 +12,16 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -38,16 +40,18 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: django-ninja
 Provides-Extra: drf-spectacular
 Provides-Extra: drf-yasg
-Requires-Dist: django (>=3,<4) ; python_full_version <= "3.8.0"
-Requires-Dist: django (>=3,<5) ; python_version >= "3.8"
+Requires-Dist: django (>=3,<4) ; python_version < "3.8"
+Requires-Dist: django (>=3,<5) ; python_version >= "3.8" and python_version < "3.10"
+Requires-Dist: django (>=4.1,<6) ; python_version >= "3.10" and python_version < "3.11"
+Requires-Dist: django (>=4.2,<6) ; python_version >= "3.11"
 Requires-Dist: django-ninja (>=1.1.0,<2.0.0) ; extra == "django-ninja"
 Requires-Dist: djangorestframework
 Requires-Dist: drf-spectacular ; extra == "drf-spectacular"
 Requires-Dist: drf-yasg ; extra == "drf-yasg"
 Requires-Dist: inflection
 Requires-Dist: openapi-spec-validator (>=0.7.1,<0.8.0)
 Requires-Dist: prance
```

