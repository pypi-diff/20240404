# Comparing `tmp/graphene_django_query_optimizer-0.5.0.tar.gz` & `tmp/graphene_django_query_optimizer-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.5.0.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.5.1.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.5.0.tar` & `graphene_django_query_optimizer-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/LICENSE
--rw-r--r--   0        0        0     3151 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/README.md
--rw-r--r--   0        0        0     6905 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      496 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11596 2024-04-03 16:39:48.753631 graphene_django_query_optimizer-0.5.0/query_optimizer/ast.py
--rw-r--r--   0        0        0     8039 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/errors.py
--rw-r--r--   0        0        0    15513 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/filter.py
--rw-r--r--   0        0        0     5238 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    11297 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/py.typed
--rw-r--r--   0        0        0     2627 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/settings.py
--rw-r--r--   0        0        0     2996 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/types.py
--rw-r--r--   0        0        0     3639 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/typing.py
--rw-r--r--   0        0        0     6141 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/utils.py
--rw-r--r--   0        0        0     3840 2024-04-03 16:39:48.757631 graphene_django_query_optimizer-0.5.0/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3151 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/README.md
+-rw-r--r--   0        0        0     6905 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11596 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8683 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/errors.py
+-rw-r--r--   0        0        0    15513 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5238 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    10870 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/py.typed
+-rw-r--r--   0        0        0     2627 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/settings.py
+-rw-r--r--   0        0        0     2996 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/types.py
+-rw-r--r--   0        0        0     3639 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6141 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3840 2024-04-04 08:55:00.909151 graphene_django_query_optimizer-0.5.1/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.5.1/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.5.0/LICENSE` & `graphene_django_query_optimizer-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/README.md` & `graphene_django_query_optimizer-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/pyproject.toml` & `graphene_django_query_optimizer-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.5.0"
+version = "0.5.1"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
```

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/compiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import contextlib
 from typing import TYPE_CHECKING, Optional, Union
 
+from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
 from django.db.models import ForeignKey, Manager, ManyToOneRel, Model, QuerySet
 from graphene.utils.str_converters import to_snake_case
 from graphene_django.utils import maybe_queryset
 
 from .ast import GraphQLASTWalker
 from .errors import OptimizerError
 from .optimizer import QueryOptimizer
@@ -130,37 +131,51 @@
         field_type: GrapheneObjectType,
         field_node: FieldNode,
         related_field: ToOneField,
         related_model: type[Model],
     ) -> None:
         name = related_field.get_cache_name() or related_field.name
         optimizer = QueryOptimizer(model=related_model, info=self.info, name=name)
-        self.optimizer.select_related[name] = optimizer
+
+        if isinstance(related_field, GenericForeignKey):
+            self.optimizer.prefetch_related[name] = optimizer
+        else:
+            self.optimizer.select_related[name] = optimizer
+
         if isinstance(related_field, ForeignKey):
             self.optimizer.related_fields.append(related_field.attname)
 
+        if isinstance(related_field, GenericForeignKey):
+            self.optimizer.related_fields.append(related_field.ct_field)
+            self.optimizer.related_fields.append(related_field.fk_field)
+
         with self.use_optimizer(optimizer):
-            super().handle_to_many_field(field_type, field_node, related_field, related_model)
+            super().handle_to_one_field(field_type, field_node, related_field, related_model)
 
     def handle_to_many_field(
         self,
         field_type: GrapheneObjectType,
         field_node: FieldNode,
         related_field: ToManyField,
         related_model: type[Model],
     ) -> None:
         name = related_field.get_cache_name() or related_field.name
         key = self.to_attr if self.to_attr is not None else name
         self.to_attr = None
 
         optimizer = QueryOptimizer(model=related_model, info=self.info, name=name)
         self.optimizer.prefetch_related[key] = optimizer
+
         if isinstance(related_field, ManyToOneRel):
             optimizer.related_fields.append(related_field.field.attname)
 
+        if isinstance(related_field, GenericRelation):
+            optimizer.related_fields.append(related_field.object_id_field_name)
+            optimizer.related_fields.append(related_field.content_type_field_name)
+
         with self.use_optimizer(optimizer):
             super().handle_to_many_field(field_type, field_node, related_field, related_model)
 
     def handle_total_count(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
         self.optimizer.total_count = True
 
     def handle_custom_field(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
```

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/fields.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/filter_info.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,37 +36,29 @@
 ]
 
 
 @dataclasses.dataclass
 class CompilationResults:
     only_fields: list[str] = dataclasses.field(default_factory=list)
     select_related: list[str] = dataclasses.field(default_factory=list)
-    prefetch_related: list[Prefetch] = dataclasses.field(default_factory=list)
-
-    @property
-    def cache_key(self) -> str:
-        only = ",".join(self.only_fields)
-        select = ",".join(self.select_related)
-        prefetch = ",".join(item.prefetch_to for item in self.prefetch_related)
-        return f"{only=}|{select=}|{prefetch=}"
+    prefetch_related: list[Prefetch | str] = dataclasses.field(default_factory=list)
 
 
 class QueryOptimizer:
     """Creates optimized queryset based on the optimization data found by the OptimizationCompiler."""
 
-    def __init__(self, model: type[Model], info: GQLInfo, name: Optional[str] = None) -> None:
+    def __init__(self, model: type[Model] | None, info: GQLInfo, name: Optional[str] = None) -> None:
         self.model = model
         self.info = info
         self.only_fields: list[str] = []
         self.related_fields: list[str] = []
         self.aliases: dict[str, ExpressionKind] = {}
         self.annotations: dict[str, ExpressionKind] = {}
         self.select_related: dict[str, QueryOptimizer] = {}
         self.prefetch_related: dict[str, QueryOptimizer] = {}
-        self._cache_key: Optional[str] = None  # generated during the optimization process
         self.total_count: bool = False
         self.name = name
 
     def optimize_queryset(
         self,
         queryset: QuerySet[TModel],
         *,
@@ -119,39 +111,43 @@
                 self.compile_prefetch(name, optimizer, results, filter_info)
             else:
                 self.compile_select(name, optimizer, results, filter_info)
 
         for attr, optimizer in self.prefetch_related.items():
             self.compile_prefetch(attr, optimizer, results, filter_info)
 
-        self._cache_key = results.cache_key
         return results
 
     def compile_select(
         self,
         name: str,
         optimizer: QueryOptimizer,
         results: CompilationResults,
         filter_info: GraphQLFilterInfo,
     ) -> None:
         results.select_related.append(name)
         nested_results = optimizer.compile(filter_info=filter_info)
         results.only_fields.extend(f"{name}{LOOKUP_SEP}{only}" for only in nested_results.only_fields)
         results.select_related.extend(f"{name}{LOOKUP_SEP}{select}" for select in nested_results.select_related)
         for prefetch in nested_results.prefetch_related:
-            prefetch.add_prefix(name)
-            results.prefetch_related.append(prefetch)
+            if isinstance(prefetch, Prefetch):
+                prefetch.add_prefix(name)
+                results.prefetch_related.append(prefetch)
 
     def compile_prefetch(
         self,
         attr: str,
         optimizer: QueryOptimizer,
         results: CompilationResults,
         filter_info: GraphQLFilterInfo,
     ) -> None:
+        if optimizer.model is None:  # generic foreign keys
+            results.prefetch_related.append(optimizer.name)
+            return
+
         filter_info = filter_info.get("children", {}).get(optimizer.name, {})
         queryset = optimizer.model._default_manager.all()
         queryset = optimizer.optimize_queryset(queryset, filter_info=filter_info)
         queryset = optimizer.paginate_prefetch_queryset(self.model, queryset, optimizer.name, filter_info=filter_info)
         to_attr = attr if attr != optimizer.name else None
         results.prefetch_related.append(Prefetch(optimizer.name, queryset, to_attr=to_attr))
 
@@ -254,16 +250,7 @@
             return object_type.filter_queryset(queryset, self.info)  # type: ignore[union-attr]
         return queryset  # pragma: no cover
 
     def process_filters(self, input_data: dict[str, Any]) -> dict[str, Any]:
         from graphene_django.filter.fields import convert_enum
 
         return {key: convert_enum(value) for key, value in input_data.items()}
-
-    @property
-    def cache_key(self) -> str:
-        if self._cache_key is None:
-            self.compile(filter_info={})
-        return self._cache_key
-
-    def __str__(self) -> str:  # pragma: no cover
-        return self.cache_key
```

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/types.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/typing.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.5.1/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.5.0/PKG-INFO` & `graphene_django_query_optimizer-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

