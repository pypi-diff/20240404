# Comparing `tmp/fastapi_cruddy_framework-1.4.2.tar.gz` & `tmp/fastapi_cruddy_framework-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-1.4.2.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-1.4.3.tar", max compression
```

## Comparing `fastapi_cruddy_framework-1.4.2.tar` & `fastapi_cruddy_framework-1.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.2/LICENSE
--rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.2/README.md
--rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    41158 2024-03-20 18:15:08.576318 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0    15489 2024-03-20 18:15:08.576677 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/graphql.py
--rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/pubsub.py
--rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    28384 2024-04-03 17:54:33.618921 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/test_helpers.py
--rw-r--r--   0        0        0     6287 2024-03-20 18:15:08.577324 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/websocket_manager.py
--rw-r--r--   0        0        0     2252 2024-04-03 18:22:26.256931 fastapi_cruddy_framework-1.4.2/pyproject.toml
--rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.3/LICENSE
+-rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.3/README.md
+-rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    41190 2024-04-03 20:42:10.151471 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/graphql.py
+-rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/pubsub.py
+-rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    30303 2024-04-04 00:54:23.409075 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/test_helpers.py
+-rw-r--r--   0        0        0     7939 2024-04-04 00:54:23.318752 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/websocket_manager.py
+-rw-r--r--   0        0        0     2252 2024-04-04 00:58:30.705453 fastapi_cruddy_framework-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.3/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-1.4.2/LICENSE` & `fastapi_cruddy_framework-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/README.md` & `fastapi_cruddy_framework-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/adapters.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -753,15 +753,15 @@
 ):
     far_col: ColumnElement = next(iter(config.orm_relationship.remote_side))
     col: ColumnElement = next(iter(config.orm_relationship.local_columns))
     far_col_name = far_col.name
     near_col_name = col.name
     resource_model_name = f"{repository.model.__name__}".lower()
     foreign_model_name = pluralizer.plural(
-        f"{config.foreign_resource.repository.model.__name__}".lower()
+        f"{config.foreign_resource.repository.model.__name__}".lower()  # type: ignore
     )
 
     # Merge three policy sets onto this endpoint:
     # 1. Universal policies
     # 2. Primary resource policies
     # 3. Related resource policies
     @controller.get(
@@ -853,15 +853,15 @@
     policies_universal: list = [],
     policies_get_one: list = [],
     default_limit: int = 10,
 ):
     far_model: Type[CruddyModel] = config.foreign_resource.repository.model
     resource_model_name = f"{repository.model.__name__}".lower()
     foreign_model_name = pluralizer.plural(
-        f"{config.foreign_resource.repository.model.__name__}".lower()
+        f"{config.foreign_resource.repository.model.__name__}".lower()  # type: ignore
     )
 
     # Merge three policy sets onto this endpoint:
     # 1. Universal policies
     # 2. Primary resource policies
     # 3. Related resource policies
     @controller.get(
```

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/graphql.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/graphql.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,19 +168,19 @@
     def _format_context(
         self,
         type_name: str,
         route_generator: Callable | None = None,
         valid_selectors: dict[str, Callable] | None = None,
         graphql_resolver_name_override: str | None = None,
     ):
-        plural_type_name = pluralizer.plural(type_name)
+        plural_type_name = pluralizer.plural(type_name)  # type: ignore
         graphql_resolver_type = (
             plural_type_name
             if graphql_resolver_name_override is None
-            else pluralizer.plural(graphql_resolver_name_override)
+            else pluralizer.plural(graphql_resolver_name_override)  # type: ignore
         )
         if route_generator is None:
 
             def default_route(_):
                 return plural_type_name
 
             route_generator = default_route
```

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/pubsub.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/pubsub.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,20 @@
     Example,
     UUID,
     uuid7,
 )
 from .controller import Actions, CruddyController, ControllerConfigurator
 from .repository import AbstractRepository
 from .adapters import BaseAdapter, SqliteAdapter, MysqlAdapter, PostgresqlAdapter
-from .util import possible_id_types, possible_id_values, lifecycle_types
+from .util import (
+    possible_id_types,
+    possible_id_values,
+    lifecycle_types,
+    estimate_simple_example,
+)
 
 
 class SchemaDict(TypedDict):
     single: Type[CruddyGenericModel]
     many: Type[CruddyGenericModel]
     create: Type[CruddyGenericModel]
     create_relations: Type[CruddyModel]
@@ -133,15 +138,15 @@
         lifecycle_before_controller_get_one: lifecycle_types = None,
         lifecycle_after_controller_get_one: lifecycle_types = None,
         lifecycle_before_controller_get_all: lifecycle_types = None,
         lifecycle_after_controller_get_all: lifecycle_types = None,
         controller_extension: Type[CruddyController] | None = None,
     ):
         possible_tag = f"{resource_model.__name__}".lower()
-        possible_path = f"/{pluralizer.plural(possible_tag)}"
+        possible_path = f"/{pluralizer.plural(possible_tag)}"  # type: ignore
         self._on_resolution = None
         self._link_prefix = link_prefix
         self._resource_path = possible_path if path == None else path
         self._tags = [possible_tag] if tags == None else tags
         self._response_schema = response_schema
         self._update_schema = resource_update_model
         self._create_schema = resource_create_model
@@ -242,20 +247,20 @@
     # Converting this section a plugin pattern will allow
     # other response formats, like JSON API.
     # Alterations will also require ControllerConfigurator
     # to be modified somehow...
 
     def generate_internal_schemas(self):
         local_resource = self
-        response_schema = self._response_schema
+        response_schema: CruddyModel = self._response_schema
         create_schema = self._create_schema
         update_schema = self._update_schema
         response_meta_schema = self._meta_schema
         resource_model_name = f"{self.repository.model.__name__}".lower()
-        resource_model_plural = pluralizer.plural(resource_model_name)
+        resource_model_plural = pluralizer.plural(resource_model_name)  # type: ignore
         resource_response_name = response_schema.__name__
         resource_create_name = create_schema.__name__
         resource_update_name = update_schema.__name__
 
         self._model_name_single = resource_model_name
         self._model_name_plural = resource_model_plural
 
@@ -271,66 +276,83 @@
                 "example": (
                     int(str(example_id))
                     if self.repository.id_type == int
                     else str(example_id)
                 )
             }
             if possible_id.json_schema_extra is not None:
+                possible_id_examples = possible_id.json_schema_extra.get(
+                    "examples", None
+                )
+                if not isinstance(possible_id_examples, list):
+                    possible_id_examples = []
                 possible_id_example = possible_id.json_schema_extra.get("example", None)
+                if possible_id_example is None and len(possible_id_examples) > 0:
+                    possible_id_example = possible_id_examples[0]
                 if possible_id_example is not None:
                     example_id = possible_id_example
+                elif possible_id.default is not None:
+                    example_id = possible_id.default
+                elif possible_id.default_factory is not None:
+                    example_id = possible_id.default_factory()
                 possible_id.json_schema_extra.update(example_dict)
             else:
                 possible_id.json_schema_extra = example_dict  # type: ignore
 
         # Create shared link model
         link_object = {}
         false_create_attrs = {}
         false_update_attrs = {}
+        view_example_dict = {}
         create_protected_relationships = (
             self._protected_relationships + self._protected_create_relationships
         )
         update_protected_relationships = (
             self._protected_relationships + self._protected_update_relationships
         )
+
+        for k, v in response_schema.model_fields.items():
+            default_example = None
+            if v.json_schema_extra is not None:
+                possible_examples = v.json_schema_extra.get("examples", None)
+                possible_example = v.json_schema_extra.get("example", None)
+                if isinstance(possible_examples, list) and len(possible_examples) > 0:
+                    default_example = possible_examples[0]
+                elif possible_example is not None:
+                    default_example = possible_example
+            elif v.default is not None:
+                default_example = v.default
+            elif v.default_factory is not None:
+                default_example = v.default_factory()
+            if default_example is None:
+                default_example = estimate_simple_example(v.annotation)
+            view_example_dict[k] = default_example
+        view_example_dict["links"] = {}
         for k, v in self._relations.items():
+            ex_link = self._single_link(id=str(example_id), relationship=k)
             link_object[k] = (
                 str,
-                Field(
-                    schema_extra={
-                        "json_schema_extra": {
-                            "example": self._single_link(
-                                id=str(example_id), relationship=k
-                            )
-                        }
-                    }
-                ),
+                Field(schema_extra={"json_schema_extra": {"example": ex_link}}),
             )
+            view_example_dict["links"][k] = ex_link
             rel_def = self._derive_shadow_relationship(
                 v.orm_relationship.direction, v.foreign_resource._id_type
             )
             if k not in create_protected_relationships:
                 false_create_attrs[k] = rel_def
             if k not in update_protected_relationships:
                 false_update_attrs[k] = rel_def
         for item in self._artificial_relationship_paths:
+            ex_link = self._single_link(id=str(example_id), relationship=item)
             link_object[item] = (
                 str,
-                Field(
-                    schema_extra={
-                        "json_schema_extra": {
-                            "example": self._single_link(
-                                id=str(example_id), relationship=item
-                            )
-                        }
-                    }
-                ),
+                Field(schema_extra={"json_schema_extra": {"example": ex_link}}),
             )
+            view_example_dict["links"][item] = ex_link
         link_object["__base__"] = CruddyModel
-
         LinkModel = create_model(f"{resource_model_name}Links", **link_object)
         # End shared link model
 
         SingleCreateSchema = create_model(
             f"{resource_create_name}Proxy", __base__=create_schema, **false_create_attrs
         )
 
@@ -358,24 +380,31 @@
         )
         # End update record envelope schema
 
         # Single record schema with embedded links
         SingleSchemaLinked = create_model(
             f"{resource_response_name}Linked",
             links=(LinkModel, None),
-            __base__=response_schema,
+            __base__=response_schema,  # type: ignore
         )
         # End single record schema with embedded links
 
         # Single record return payload (for get/{id})
         SingleSchemaEnvelope = create_model(
             f"{resource_response_name}Envelope",
             __base__=CruddyGenericModel,
             **{
-                resource_model_name: (SingleSchemaLinked, ...),
+                resource_model_name: (
+                    SingleSchemaLinked,
+                    Field(
+                        schema_extra={
+                            "json_schema_extra": {"example": view_example_dict}
+                        }
+                    ),
+                ),
                 "meta": (dict[str, Any] | None, None),
             },  # type: ignore
         )
 
         handle_data_or_none = self._create_schema_arg_handler(
             single_schema_linked=SingleSchemaLinked,
             resource_model_name=resource_model_name,
@@ -393,15 +422,22 @@
         # End single record return payload
 
         # Many records return payload (for get/ and queries with "where")
         ManySchemaEnvelope = create_model(
             f"{resource_response_name}List",
             __base__=CruddyGenericModel,
             **{
-                resource_model_plural: (list[SingleSchemaLinked], ...),
+                resource_model_plural: (
+                    list[SingleSchemaLinked],
+                    Field(
+                        schema_extra={
+                            "json_schema_extra": {"example": [view_example_dict]}
+                        }
+                    ),
+                ),
             },  # type: ignore
             meta=(response_meta_schema, ...),
         )
 
         old_many_init = ManySchemaEnvelope.__init__
 
         def new_many_init(self, *args, **kwargs):
```

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/test_helpers.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/util.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import inspect
-from typing import Type, Coroutine, Any, Callable
+from typing import Type, Coroutine, Any, Callable, Union
+from typing_extensions import get_args, get_origin
+from datetime import date, datetime, timezone
 from json import dumps, loads
-from uuid import UUID
 from datetime import date, datetime, timezone, timedelta
 from re import compile, Match
 from fastapi import Request, WebSocket, Depends
+from fastapi.types import UnionType
 from pydantic.errors import PydanticErrorMixin
 from sqlalchemy.orm import class_mapper, object_mapper
+from .schemas import UUID, uuid7
 
 
 possible_id_types = Type[UUID] | Type[int] | Type[str]
 possible_id_values = UUID | int | str
 lifecycle_types = Callable[..., Coroutine[Any, Any, Any]] | None
 EPOCH = datetime(1970, 1, 1)
 # if greater than this, the number is in ms, if less than or equal it's in seconds
@@ -210,7 +213,48 @@
     default: Any | None = None,
 ) -> Any:
     return getattr(connection.state, key, default)
 
 
 def set_state(connection: Request | WebSocket, key: str, value: Any) -> None:
     setattr(connection.state, key, value)
+
+
+def estimate_example_for_type(type_annotation: type[Any] | None):
+    if type_annotation is None or not inspect.isclass(type_annotation):
+        return None
+    if issubclass(type_annotation, UUID):
+        return f"{uuid7()}"
+    if issubclass(type_annotation, bool):
+        return True
+    if issubclass(type_annotation, str):
+        return "string"
+    if issubclass(type_annotation, int):
+        return 1
+    if issubclass(type_annotation, float):
+        return 1.0
+    if issubclass(type_annotation, dict):
+        return {}
+    if issubclass(type_annotation, list):
+        return []
+    if issubclass(type_annotation, tuple):
+        return []
+    if issubclass(type_annotation, datetime):
+        return datetime.now(tz=timezone.utc).isoformat()
+    if issubclass(type_annotation, date):
+        return date.today().isoformat()
+    return None
+
+
+def estimate_simple_example(annotation: Any | None) -> Any | None:
+    origin = get_origin(annotation)
+    if origin is Union or origin is UnionType:
+        for arg in get_args(annotation):
+            possible_example = estimate_example_for_type(arg)
+            if possible_example is not None:
+                return possible_example
+            possible_example = estimate_simple_example(arg)
+            if possible_example is not None:
+                return possible_example
+    if (possible_example := estimate_example_for_type(annotation)) is not None:
+        return possible_example
+    return estimate_example_for_type(origin)
```

### Comparing `fastapi_cruddy_framework-1.4.2/fastapi_cruddy_framework/websocket_manager.py` & `fastapi_cruddy_framework-1.4.3/fastapi_cruddy_framework/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.2/pyproject.toml` & `fastapi_cruddy_framework-1.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "1.4.2"
+version = "1.4.3"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-1.4.2/PKG-INFO` & `fastapi_cruddy_framework-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 1.4.2
+Version: 1.4.3
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.2 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.3 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

