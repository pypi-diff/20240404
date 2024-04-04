# Comparing `tmp/sartorial-0.6.1.tar.gz` & `tmp/sartorial-0.7.0.tar.gz`

## Comparing `sartorial-0.6.1.tar` & `sartorial-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sartorial-0.6.1/sartorial/__init__.py
--rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 sartorial-0.6.1/sartorial/schema.py
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 sartorial-0.6.1/sartorial/serialization.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 sartorial-0.6.1/sartorial/types.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sartorial-0.6.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sartorial-0.6.1/LICENSE
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 sartorial-0.6.1/README.md
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sartorial-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 sartorial-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 sartorial-0.7.0/sartorial/__init__.py
+-rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 sartorial-0.7.0/sartorial/schema.py
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 sartorial-0.7.0/sartorial/serialization.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 sartorial-0.7.0/sartorial/types.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 sartorial-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 sartorial-0.7.0/LICENSE
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 sartorial-0.7.0/README.md
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 sartorial-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 sartorial-0.7.0/PKG-INFO
```

### Comparing `sartorial-0.6.1/sartorial/schema.py` & `sartorial-0.7.0/sartorial/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     Sequence,
     Type,
     get_args,
     get_origin,
     get_type_hints,
 )
 
-from foundational.casing import to_camel_case
-from foundational.collections import is_mapping
-from foundational.enum import StringEnum
-from foundational.nesting import nested_get, nested_set
-from foundational.nulls import Omitted
+from communal.casing import to_camel_case
+from communal.collections import is_mapping
+from communal.enum import StringEnum
+from communal.nesting import nested_get, nested_set
+from communal.nulls import Omitted
 from pydantic import BaseModel, ConfigDict, create_model
 
 from sartorial.types import JSON_SCHEMA_DEFAULT_TYPES, JSONSchemaFormatted
 
 
 def json_schema_extra(schema: Dict[str, AnyType], model: Type["Schema"]) -> None:
     model.json_schema_extra(schema, model)
```

### Comparing `sartorial-0.6.1/sartorial/serialization.py` & `sartorial-0.7.0/sartorial/serialization.py`

 * *Files identical despite different names*

### Comparing `sartorial-0.6.1/sartorial/types.py` & `sartorial-0.7.0/sartorial/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     IPv6Network,
 )
 from pathlib import Path
 from typing import Any as AnyType
 from typing import ClassVar, Type
 from uuid import UUID
 
-from foundational.nulls import DoesNotExist, Omitted
+from communal.nulls import DoesNotExist, Omitted
 from pydantic import GetCoreSchemaHandler
 from pydantic.json_schema import GetJsonSchemaHandler, JsonSchemaValue
 from pydantic_core import CoreSchema, SchemaSerializer, core_schema
 
 JSON_SCHEMA_DEFAULT_TYPES = {
     "string": str,
     "number": float,
@@ -73,14 +73,19 @@
     @classmethod
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         if "python_type" not in cls.__dict__:
             cls.python_type = cls
         if not cls.schema_format:
             raise ValueError("schema_format is required")
+        if "schema_format" not in cls.__dict__ and (
+            not hasattr(".__pydantic_generic_metadata__")
+            or not cls.__pydantic_generic_metadata__.get("origin")
+        ):
+            raise ValueError("schema_format is required for generic base classes")
         cls.register(cls.python_type, cls.schema_type, cls.schema_format)
 
     @classmethod
     def get_type(
         cls, schema_type: str, schema_format: str, default: AnyType = DoesNotExist
     ) -> Type:
         return cls.__string_type_formats__.get(schema_type, {}).get(
```

### Comparing `sartorial-0.6.1/.gitignore` & `sartorial-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sartorial-0.6.1/LICENSE` & `sartorial-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sartorial-0.6.1/pyproject.toml` & `sartorial-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [bumpver]
-current_version = "0.6.1"
+current_version = "0.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
@@ -44,15 +44,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "foundational",
+    "communal",
     "pydantic>2"
 ]
 
 [project.urls]
 Homepage = "https://github.com/goodcleanfun/sartorial"
 Repository = "https://github.com/goodcleanfun/sartorial"
```

### Comparing `sartorial-0.6.1/PKG-INFO` & `sartorial-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sartorial
-Version: 0.6.1
+Version: 0.7.0
 Summary: Pydantic model base classes and custom type handling, JSON schema generation, etc. covering a variety of common scenarios without much config
 Project-URL: Homepage, https://github.com/goodcleanfun/sartorial
 Project-URL: Repository, https://github.com/goodcleanfun/sartorial
 Author: Al Barrentine
 License-Expression: MIT
 License-File: LICENSE
 Keywords: json-schema,model,pydantic,sartorial,schema
@@ -13,13 +13,13 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
-Requires-Dist: foundational
+Requires-Dist: communal
 Requires-Dist: pydantic>2
 Description-Content-Type: text/markdown
 
 # sartorial
 Tailoring custom types to fit Pydantic models, including JSON schema generation and on-the-fly model generation with custom types using JSON Schema's "format" key, allowing lossless serialization/deserialiation of arbitrary models. Contains simple JSON encoding/decoding for most types and the ability to specify them for new types with an interface mixin.
```

