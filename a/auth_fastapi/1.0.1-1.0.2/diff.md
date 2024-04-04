# Comparing `tmp/auth_fastapi-1.0.1.tar.gz` & `tmp/auth_fastapi-1.0.2.tar.gz`

## Comparing `auth_fastapi-1.0.1.tar` & `auth_fastapi-1.0.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    92675 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/logo.png
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/.github/workflows/workflow.yml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/__main__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/consts.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/exceptions.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/fastapi_auth.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/hasher.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/jwt.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/permissions.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/authenticators/__init__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/authenticators/base.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/backends/__init__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/backends/backend.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/backends/base.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/filters/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/filters/base.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/filters/ordering_filter.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/filters/search_filter.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/managers/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/managers/base.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/managers/manager.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/models/__init__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/models/model.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/models/token.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/models/user.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/base.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/limit_pagination.py
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/page.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/page_pagination.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/repositories/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/repositories/base.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/schemas/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/schemas/default_schemas.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/base.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/sqlalchemy/serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/tortoise/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/tortoise/serializers.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/signals/__init__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/signals/signal.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/sqlalchemy_models/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/strategies/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/strategies/base.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/strategies/db.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/strategies/jwt.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/tortoise_models/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/utils/__init__.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/utils/command_utils.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/utils/utils.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/.gitignore
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/README.md
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    92675 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/logo.png
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/__main__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/consts.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/exceptions.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/fastapi_auth.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/hasher.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/jwt.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/permissions.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/authenticators/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/authenticators/base.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/backends/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/backends/backend.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/backends/base.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/filters/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/filters/base.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/filters/ordering_filter.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/filters/search_filter.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/managers/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/managers/base.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/managers/manager.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/models/__init__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/models/model.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/models/token.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/models/user.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/pagination/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/pagination/base.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/pagination/limit_pagination.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/pagination/page.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/pagination/page_pagination.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/repositories/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/repositories/base.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/schemas/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/schemas/default_schemas.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/serializers/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/serializers/base.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/serializers/serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/serializers/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/serializers/sqlalchemy/serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/serializers/tortoise/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/serializers/tortoise/serializers.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/signals/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/signals/signal.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/sqlalchemy_models/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/strategies/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/strategies/base.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/strategies/db.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/strategies/jwt.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/tortoise_models/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/utils/__init__.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/utils/command_utils.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/fastapi_auth/utils/utils.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/.gitignore
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/README.md
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 auth_fastapi-1.0.2/PKG-INFO
```

### Comparing `auth_fastapi-1.0.1/logo.png` & `auth_fastapi-1.0.2/logo.png`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/.github/workflows/workflow.yml` & `auth_fastapi-1.0.2/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/hasher.py` & `auth_fastapi-1.0.2/fastapi_auth/hasher.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/jwt.py` & `auth_fastapi-1.0.2/fastapi_auth/jwt.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/permissions.py` & `auth_fastapi-1.0.2/fastapi_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/authenticators/base.py` & `auth_fastapi-1.0.2/fastapi_auth/authenticators/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/backends/base.py` & `auth_fastapi-1.0.2/fastapi_auth/backends/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/filters/base.py` & `auth_fastapi-1.0.2/fastapi_auth/filters/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/filters/ordering_filter.py` & `auth_fastapi-1.0.2/fastapi_auth/filters/ordering_filter.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/filters/search_filter.py` & `auth_fastapi-1.0.2/fastapi_auth/filters/search_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 self._check_item(item, search_field1, queryset, param, sub_item)
             else:
                 self._check_item(item, search_field, queryset, param)
 
     def _check_item(self, item: object, search_field: str, queryset: Set, param: str, sub_item: object = None):
         obj = sub_item if sub_item is not None else item
         if hasattr(obj, search_field):
-            if param in str(getattr(obj, search_field, "")).lower().strip():
+            if param.lower() in str(getattr(obj, search_field, "")).lower().strip():
                 queryset.add(item)
         else:
             raise AttributeError(f"{obj} has no attribute {search_field}")
 
     @classmethod
     def request_schema(cls) -> Type[BaseModel]:
         request_schema = {
```

### Comparing `auth_fastapi-1.0.1/fastapi_auth/managers/base.py` & `auth_fastapi-1.0.2/fastapi_auth/managers/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/models/model.py` & `auth_fastapi-1.0.2/fastapi_auth/models/model.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/models/token.py` & `auth_fastapi-1.0.2/fastapi_auth/models/token.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/models/user.py` & `auth_fastapi-1.0.2/fastapi_auth/models/user.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/pagination/base.py` & `auth_fastapi-1.0.2/fastapi_auth/pagination/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/pagination/limit_pagination.py` & `auth_fastapi-1.0.2/fastapi_auth/pagination/limit_pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.count = self.get_count(instances)
         self.limit = self._get_limit()
         self.offset = self._get_offset()
         if self.count == 0 or self.offset > self.count:
             return []
         return instances[self.offset:self.offset + self.limit]
 
-    async def get_paginated_response(self, instances) -> OrderedDict:
+    async def get_paginated_response(self, instances: Sequence[object]) -> OrderedDict:
         data = self._paginate_queryset(instances)
         return OrderedDict([
             ('count', self.count),
             ('next', self.get_next_link()),
             ('previous', self.get_previous_link()),
             ('results', await self._serializer(data, many=True).data)
         ])
```

### Comparing `auth_fastapi-1.0.1/fastapi_auth/pagination/page.py` & `auth_fastapi-1.0.2/fastapi_auth/pagination/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections
 import inspect
 import warnings
 from functools import cached_property
 from math import ceil
-from typing import Optional
+from typing import Optional, Sequence
 from fastapi_auth.utils import method_has_no_args
 
 
 class InvalidPage(Exception):
     pass
 
 
@@ -27,15 +27,15 @@
         "invalid_page": "That page number is not an integer",
         "min_page": "That page number is less than 1",
         "no_results": "That page contains no results",
     }
 
     def __init__(
             self,
-            object_list: list,
+            object_list: Sequence,
             per_page,
             orphans=0,
             allow_empty_first_page: bool = True,
             error_messages: Optional[dict] = None,
     ):
         self.object_list = object_list
         self._check_object_list_is_ordered()
```

### Comparing `auth_fastapi-1.0.1/fastapi_auth/pagination/page_pagination.py` & `auth_fastapi-1.0.2/fastapi_auth/pagination/page_pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import OrderedDict
-from typing import Type, Optional
+from typing import Type, Optional, Sequence
 from pydantic import BaseModel, Field, create_model, ConfigDict
 from fastapi_auth.pagination.base import BasePagination
 from fastapi_auth.serializers.base import BaseSerializer
 from fastapi import Request, HTTPException
 from fastapi_auth.pagination.page import Paginator, InvalidPage
 
 from fastapi_auth.utils import replace_query_param, remove_query_param
@@ -16,15 +16,15 @@
     invalid_page_message = 'Invalid page.'
 
     def __init__(self, request: Request, serializer: Type[BaseSerializer]):
         self._request = request
         self._serializer = serializer
         self.page = None
 
-    def _paginate_queryset(self, instances: list[object]) -> list[object]:
+    def _paginate_queryset(self, instances: Sequence[object]) -> list[object]:
         page_number = self.get_page_number()
         page_size = self.get_page_size()
         paginator = Paginator(instances, page_size, allow_empty_first_page=True)
         try:
             self.page = paginator.page(page_number)
         except InvalidPage as exc:
             msg = self.invalid_page_message.format(
```

### Comparing `auth_fastapi-1.0.1/fastapi_auth/repositories/base.py` & `auth_fastapi-1.0.2/fastapi_auth/repositories/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/serializers/base.py` & `auth_fastapi-1.0.2/fastapi_auth/serializers/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/serializers/serializers.py` & `auth_fastapi-1.0.2/fastapi_auth/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/serializers/sqlalchemy/serializers.py` & `auth_fastapi-1.0.2/fastapi_auth/serializers/sqlalchemy/serializers.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/serializers/tortoise/serializers.py` & `auth_fastapi-1.0.2/fastapi_auth/serializers/tortoise/serializers.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/signals/signal.py` & `auth_fastapi-1.0.2/fastapi_auth/signals/signal.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/sqlalchemy_models/__init__.py` & `auth_fastapi-1.0.2/fastapi_auth/sqlalchemy_models/__init__.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/strategies/base.py` & `auth_fastapi-1.0.2/fastapi_auth/strategies/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/strategies/db.py` & `auth_fastapi-1.0.2/fastapi_auth/strategies/db.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/strategies/jwt.py` & `auth_fastapi-1.0.2/fastapi_auth/strategies/jwt.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/utils/command_utils.py` & `auth_fastapi-1.0.2/fastapi_auth/utils/command_utils.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/fastapi_auth/utils/utils.py` & `auth_fastapi-1.0.2/fastapi_auth/utils/utils.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/README.md` & `auth_fastapi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/pyproject.toml` & `auth_fastapi-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.1/PKG-INFO` & `auth_fastapi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: auth_fastapi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Authentication library for FastAPI for fast migration from Django/DRF. Serializers, signals, permissions, pagination and filters included.
 Project-URL: Source, https://github.com/zayycev22/fastapi-auth
 Author: zayycev22
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: auth_fastapi Version: 1.0.1 Summary: Authentication
+Metadata-Version: 2.3 Name: auth_fastapi Version: 1.0.2 Summary: Authentication
 library for FastAPI for fast migration from Django/DRF. Serializers, signals,
 permissions, pagination and filters included. Project-URL: Source, https://
 github.com/zayycev22/fastapi-auth Author: zayycev22 Classifier: Framework ::
 FastAPI Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

