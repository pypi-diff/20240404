# Comparing `tmp/dyapi-0.9.2.tar.gz` & `tmp/dyapi-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyapi-0.9.2.tar", max compression
+gzip compressed data, was "dyapi-0.9.3.tar", max compression
```

## Comparing `dyapi-0.9.2.tar` & `dyapi-0.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3693 2024-03-31 19:41:39.711292 dyapi-0.9.2/README.md
--rw-r--r--   0        0        0      463 2024-04-02 10:45:19.035467 dyapi-0.9.2/dyapi/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 11:00:17.031695 dyapi-0.9.2/dyapi/entities/__init__.py
--rw-r--r--   0        0        0      556 2024-03-29 16:33:17.090998 dyapi-0.9.2/dyapi/entities/config.py
--rw-r--r--   0        0        0      308 2024-03-31 17:47:11.932909 dyapi-0.9.2/dyapi/entities/endpoint_settings.py
--rw-r--r--   0        0        0      235 2024-03-29 17:06:44.747416 dyapi-0.9.2/dyapi/entities/model_settings.py
--rw-r--r--   0        0        0      331 2024-03-29 11:50:46.579490 dyapi-0.9.2/dyapi/entities/pagination.py
--rw-r--r--   0        0        0        0 2024-03-29 08:54:12.822771 dyapi-0.9.2/dyapi/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 09:10:39.710706 dyapi-0.9.2/dyapi/implementations/builders/__init__.py
--rw-r--r--   0        0        0     2063 2024-03-31 19:30:12.023845 dyapi-0.9.2/dyapi/implementations/builders/api.py
--rw-r--r--   0        0        0     3643 2024-04-02 11:09:55.856179 dyapi-0.9.2/dyapi/implementations/builders/crud.py
--rw-r--r--   0        0        0     8080 2024-04-02 11:09:55.741953 dyapi-0.9.2/dyapi/implementations/builders/endpoint.py
--rw-r--r--   0        0        0     3141 2024-04-03 09:47:26.457626 dyapi-0.9.2/dyapi/implementations/builders/model.py
--rw-r--r--   0        0        0        0 2024-03-29 11:51:32.889326 dyapi-0.9.2/dyapi/implementations/storages/__init__.py
--rw-r--r--   0        0        0      141 2024-03-29 11:50:46.360544 dyapi-0.9.2/dyapi/implementations/storages/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-29 11:52:43.740255 dyapi-0.9.2/dyapi/implementations/storages/postgres/__init__.py
--rw-r--r--   0        0        0     6517 2024-04-02 12:58:49.115195 dyapi-0.9.2/dyapi/implementations/storages/postgres/base.py
--rw-r--r--   0        0        0     2311 2024-04-02 10:56:42.827026 dyapi-0.9.2/dyapi/implementations/storages/postgres/manager.py
--rw-r--r--   0        0        0        0 2024-03-29 09:09:32.173661 dyapi-0.9.2/dyapi/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2024-03-29 08:49:20.167380 dyapi-0.9.2/dyapi/interfaces/builders/__init__.py
--rw-r--r--   0        0        0      775 2024-03-31 17:47:11.947727 dyapi-0.9.2/dyapi/interfaces/builders/api.py
--rw-r--r--   0        0        0      909 2024-03-31 17:47:11.948512 dyapi-0.9.2/dyapi/interfaces/builders/crud.py
--rw-r--r--   0        0        0     1319 2024-03-31 16:53:23.735626 dyapi-0.9.2/dyapi/interfaces/builders/endpoint.py
--rw-r--r--   0        0        0     1027 2024-03-31 17:47:11.949901 dyapi-0.9.2/dyapi/interfaces/builders/model.py
--rw-r--r--   0        0        0      118 2024-03-29 16:30:09.491190 dyapi-0.9.2/dyapi/interfaces/storages/__init__.py
--rw-r--r--   0        0        0      846 2024-03-31 20:27:44.610243 dyapi-0.9.2/dyapi/interfaces/storages/base.py
--rw-r--r--   0        0        0      235 2024-03-31 17:47:12.079538 dyapi-0.9.2/dyapi/interfaces/storages/manager.py
--rw-r--r--   0        0        0     2154 2024-04-03 09:47:34.019649 dyapi-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 dyapi-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     3693 2024-03-31 19:41:39.711292 dyapi-0.9.3/README.md
+-rw-r--r--   0        0        0      463 2024-04-02 10:45:19.035467 dyapi-0.9.3/dyapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 11:00:17.031695 dyapi-0.9.3/dyapi/entities/__init__.py
+-rw-r--r--   0        0        0      556 2024-03-29 16:33:17.090998 dyapi-0.9.3/dyapi/entities/config.py
+-rw-r--r--   0        0        0      308 2024-03-31 17:47:11.932909 dyapi-0.9.3/dyapi/entities/endpoint_settings.py
+-rw-r--r--   0        0        0      235 2024-03-29 17:06:44.747416 dyapi-0.9.3/dyapi/entities/model_settings.py
+-rw-r--r--   0        0        0      331 2024-03-29 11:50:46.579490 dyapi-0.9.3/dyapi/entities/pagination.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:54:12.822771 dyapi-0.9.3/dyapi/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 09:10:39.710706 dyapi-0.9.3/dyapi/implementations/builders/__init__.py
+-rw-r--r--   0        0        0     2063 2024-03-31 19:30:12.023845 dyapi-0.9.3/dyapi/implementations/builders/api.py
+-rw-r--r--   0        0        0     3756 2024-04-04 09:06:39.864204 dyapi-0.9.3/dyapi/implementations/builders/crud.py
+-rw-r--r--   0        0        0     8547 2024-04-04 09:07:44.328849 dyapi-0.9.3/dyapi/implementations/builders/endpoint.py
+-rw-r--r--   0        0        0     3268 2024-04-04 08:36:23.342013 dyapi-0.9.3/dyapi/implementations/builders/model.py
+-rw-r--r--   0        0        0        0 2024-03-29 11:51:32.889326 dyapi-0.9.3/dyapi/implementations/storages/__init__.py
+-rw-r--r--   0        0        0      141 2024-03-29 11:50:46.360544 dyapi-0.9.3/dyapi/implementations/storages/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-29 11:52:43.740255 dyapi-0.9.3/dyapi/implementations/storages/postgres/__init__.py
+-rw-r--r--   0        0        0     7482 2024-04-04 09:07:28.274489 dyapi-0.9.3/dyapi/implementations/storages/postgres/base.py
+-rw-r--r--   0        0        0     2311 2024-04-02 10:56:42.827026 dyapi-0.9.3/dyapi/implementations/storages/postgres/manager.py
+-rw-r--r--   0        0        0        0 2024-03-29 09:09:32.173661 dyapi-0.9.3/dyapi/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-29 08:49:20.167380 dyapi-0.9.3/dyapi/interfaces/builders/__init__.py
+-rw-r--r--   0        0        0      775 2024-03-31 17:47:11.947727 dyapi-0.9.3/dyapi/interfaces/builders/api.py
+-rw-r--r--   0        0        0      909 2024-03-31 17:47:11.948512 dyapi-0.9.3/dyapi/interfaces/builders/crud.py
+-rw-r--r--   0        0        0     1319 2024-03-31 16:53:23.735626 dyapi-0.9.3/dyapi/interfaces/builders/endpoint.py
+-rw-r--r--   0        0        0     1027 2024-03-31 17:47:11.949901 dyapi-0.9.3/dyapi/interfaces/builders/model.py
+-rw-r--r--   0        0        0      118 2024-03-29 16:30:09.491190 dyapi-0.9.3/dyapi/interfaces/storages/__init__.py
+-rw-r--r--   0        0        0      846 2024-03-31 20:27:44.610243 dyapi-0.9.3/dyapi/interfaces/storages/base.py
+-rw-r--r--   0        0        0      235 2024-03-31 17:47:12.079538 dyapi-0.9.3/dyapi/interfaces/storages/manager.py
+-rw-r--r--   0        0        0     2154 2024-04-04 09:06:35.602370 dyapi-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4214 1970-01-01 00:00:00.000000 dyapi-0.9.3/PKG-INFO
```

### Comparing `dyapi-0.9.2/README.md` & `dyapi-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/dyapi/entities/config.py` & `dyapi-0.9.3/dyapi/entities/config.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/dyapi/implementations/builders/api.py` & `dyapi-0.9.3/dyapi/implementations/builders/api.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/dyapi/implementations/builders/crud.py` & `dyapi-0.9.3/dyapi/implementations/builders/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,18 @@
                 "{" + field + "}"
                 for field in self.endpoint.path_schema.model_fields.keys()
             ]
         )
 
         router.add_api_route("/", self.endpoint.create, methods=["POST"])
 
+        router.add_api_route(
+            "/upsert_many", self.endpoint.upsert_many, methods=["POST"]
+        )
+
         router.add_api_route("/", self.endpoint.list, methods=["GET"])
 
         router.add_api_route(f"/{path}", self.endpoint.get, methods=["GET"])
 
         router.add_api_route(f"/{path}", self.endpoint.update, methods=["PUT"])
 
         router.add_api_route(f"/{path}", self.endpoint.delete, methods=["DELETE"])
```

### Comparing `dyapi-0.9.2/dyapi/implementations/builders/endpoint.py` & `dyapi-0.9.3/dyapi/implementations/builders/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,28 @@
                 raise AlreadyExistsException(message="Entity already exists")
 
             return schema(**model.__dict__)
 
         return endpoint
 
     @cached_property
+    def upsert_many(self) -> Callable[[Any], Any]:
+        schema = self.schema
+
+        async def endpoint(
+            entities: list[schema] = Body(...),  # type: ignore
+            session: AsyncSession = Depends(self.db_session),
+        ) -> list[schema]:  # type: ignore
+            return await self.storage.upsert_many(
+                session=session, model_type=self.db_model, entities=entities
+            )
+
+        return endpoint
+
+    @cached_property
     def get(self) -> Callable[[Any], Any]:
         schema = self.schema
 
         async def endpoint(
             path: schema = Depends(self.path_schema),  # type: ignore
             session: AsyncSession = Depends(self.db_session),
         ) -> schema:  # type: ignore
```

### Comparing `dyapi-0.9.2/dyapi/implementations/builders/model.py` & `dyapi-0.9.3/dyapi/implementations/builders/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from functools import cached_property
 from typing import Type
 
-from pydantic import BaseModel, create_model
-from sqlalchemy.orm import DeclarativeBase
-
 from dyapi.entities.config import Config, ConfigField
 from dyapi.interfaces.builders.model import IModelBuilder
+from pydantic import BaseModel, create_model
+from sqlalchemy.orm import DeclarativeBase
 
 
 class ModelBuilder(IModelBuilder):
     def __init__(self, config: Config):
         self.config = config
 
     @staticmethod
@@ -59,27 +58,33 @@
         self.model = model
 
     @cached_property
     def base(self) -> Type[BaseModel]:
         return create_model(  # type: ignore
             self.model.__name__ + "Schema",
             **{
-                key: (value.type.python_type | None, None)
-                if value.nullable else (value.type.python_type, ...)
+                key: (
+                    (value.type.python_type | None, None)
+                    if value.nullable
+                    else (value.type.python_type, ...)
+                )
                 for key, value in self.model.__table__.columns.items()
             },
         )
 
     @cached_property
     def path(self) -> Type[BaseModel]:
         return create_model(  # type: ignore
             self.model.__name__ + "SchemaIdentifier",
             **{
-                key: (value.type.python_type | None, None)
-                if value.nullable else (value.type.python_type, ...)
+                key: (
+                    (value.type.python_type | None, None)
+                    if value.nullable
+                    else (value.type.python_type, ...)
+                )
                 for key, value in self.model.__table__.columns.items()
                 if value.primary_key
             },
         )
 
     @cached_property
     def filter(self) -> Type[BaseModel]:
```

### Comparing `dyapi-0.9.2/dyapi/implementations/storages/postgres/base.py` & `dyapi-0.9.3/dyapi/implementations/storages/postgres/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from asyncpg import UniqueViolationError
 from dyapi.entities.pagination import PaginationEntity
 from dyapi.implementations.storages.exceptions import AlreadyExistsError, NotFoundError
 from dyapi.interfaces.storages import IStorage
 from pydantic import BaseModel
 from sqlalchemy import Table, func, select
+from sqlalchemy.dialects.postgresql import insert
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
 from sqlalchemy.orm import DeclarativeBase
 
 __all__ = ["PostgresEngineStorage"]
 
 
@@ -133,14 +134,39 @@
         except IntegrityError as exc:
             await session.rollback()
             if exc.orig.sqlstate == UniqueViolationError.sqlstate:
                 raise AlreadyExistsError from exc
         return model
 
     @staticmethod
+    async def upsert_many(
+        entities: list[BaseModel],
+        model_type: Type[DeclarativeBase],
+        session: AsyncSession,
+    ) -> list[BaseModel]:
+        stmt = insert(model_type.__table__).values([e.model_dump() for e in entities])
+        pk_fields: list[str] = [
+            field_name
+            for field_name, field_value in model_type.__table__.columns.items()
+            if field_value.primary_key
+        ]
+        regular_fields: list[str] = [
+            field_name
+            for field_name, field_value in model_type.__table__.columns.items()
+            if not field_value.primary_key
+        ]
+        query = stmt.on_conflict_do_update(
+            index_elements=pk_fields,
+            set_={field: getattr(stmt.excluded, field) for field in regular_fields},
+        )
+        await session.execute(query)
+        await session.flush()
+        return entities
+
+    @staticmethod
     async def get(
         model_type: Type[DeclarativeBase],
         session: AsyncSession,
         filter_: BaseModel,
     ) -> DeclarativeBase:
         query = select(model_type).filter_by(**filter_.model_dump())
         model = (await session.execute(query)).fetchone()
```

### Comparing `dyapi-0.9.2/dyapi/implementations/storages/postgres/manager.py` & `dyapi-0.9.3/dyapi/implementations/storages/postgres/manager.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/dyapi/interfaces/builders/api.py` & `dyapi-0.9.3/dyapi/interfaces/builders/api.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/dyapi/interfaces/builders/crud.py` & `dyapi-0.9.3/dyapi/interfaces/builders/crud.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/dyapi/interfaces/builders/endpoint.py` & `dyapi-0.9.3/dyapi/interfaces/builders/endpoint.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/dyapi/interfaces/builders/model.py` & `dyapi-0.9.3/dyapi/interfaces/builders/model.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/dyapi/interfaces/storages/base.py` & `dyapi-0.9.3/dyapi/interfaces/storages/base.py`

 * *Files identical despite different names*

### Comparing `dyapi-0.9.2/pyproject.toml` & `dyapi-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dyapi"
-version = "0.9.2"
+version = "0.9.3"
 description = ""
 authors = ["Artem Bogdanov <abogdaov@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "dyapi", from = "." }]
 
 
 [tool.poetry.dependencies]
```

### Comparing `dyapi-0.9.2/PKG-INFO` & `dyapi-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyapi
-Version: 0.9.2
+Version: 0.9.3
 Summary: 
 Author: Artem Bogdanov
 Author-email: abogdaov@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

