# Comparing `tmp/auth_fastapi-1.0.0.tar.gz` & `tmp/auth_fastapi-1.0.1.tar.gz`

## Comparing `auth_fastapi-1.0.0.tar` & `auth_fastapi-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    92675 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/logo.png
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/.github/workflows/workflow.yml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/__main__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/consts.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/exceptions.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/fastapi_auth.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/hasher.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/jwt.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/permissions.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/authenticators/__init__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/authenticators/base.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/backends/__init__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/backends/backend.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/backends/base.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/filters/__init__.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/filters/base.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/filters/ordering_filter.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/filters/search_filter.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/managers/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/managers/base.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/managers/manager.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/models/__init__.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/models/model.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/models/token.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/models/user.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/pagination/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/pagination/base.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/pagination/limit_pagination.py
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/pagination/page.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/pagination/page_pagination.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/repositories/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/repositories/base.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/schemas/__init__.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/schemas/default_schemas.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/serializers/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/serializers/base.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/serializers/serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/serializers/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/serializers/sqlalchemy/serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/serializers/tortoise/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/serializers/tortoise/serializers.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/signals/__init__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/signals/signal.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/sqlalchemy_models/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/strategies/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/strategies/base.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/strategies/db.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/strategies/jwt.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/tortoise_models/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/utils/__init__.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/utils/command_utils.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/fastapi_auth/utils/utils.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/.gitignore
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/README.md
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 auth_fastapi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    92675 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/logo.png
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/__main__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/consts.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/exceptions.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/fastapi_auth.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/hasher.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/jwt.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/permissions.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/authenticators/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/authenticators/base.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/backends/__init__.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/backends/backend.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/backends/base.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/filters/__init__.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/filters/base.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/filters/ordering_filter.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/filters/search_filter.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/managers/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/managers/base.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/managers/manager.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/models/__init__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/models/model.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/models/token.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/models/user.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/base.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/limit_pagination.py
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/page.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/pagination/page_pagination.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/repositories/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/repositories/base.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/schemas/__init__.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/schemas/default_schemas.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/base.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/sqlalchemy/serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/tortoise/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/serializers/tortoise/serializers.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/signals/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/signals/signal.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/sqlalchemy_models/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/strategies/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/strategies/base.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/strategies/db.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/strategies/jwt.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/tortoise_models/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/utils/__init__.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/utils/command_utils.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/fastapi_auth/utils/utils.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/.gitignore
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/README.md
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 auth_fastapi-1.0.1/PKG-INFO
```

### Comparing `auth_fastapi-1.0.0/logo.png` & `auth_fastapi-1.0.1/logo.png`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/.github/workflows/workflow.yml` & `auth_fastapi-1.0.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/hasher.py` & `auth_fastapi-1.0.1/fastapi_auth/hasher.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/jwt.py` & `auth_fastapi-1.0.1/fastapi_auth/jwt.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/permissions.py` & `auth_fastapi-1.0.1/fastapi_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/authenticators/base.py` & `auth_fastapi-1.0.1/fastapi_auth/authenticators/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/backends/base.py` & `auth_fastapi-1.0.1/fastapi_auth/backends/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/filters/base.py` & `auth_fastapi-1.0.1/fastapi_auth/filters/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/filters/ordering_filter.py` & `auth_fastapi-1.0.1/fastapi_auth/filters/ordering_filter.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/filters/search_filter.py` & `auth_fastapi-1.0.1/fastapi_auth/filters/search_filter.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/managers/base.py` & `auth_fastapi-1.0.1/fastapi_auth/managers/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/models/model.py` & `auth_fastapi-1.0.1/fastapi_auth/models/model.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/models/token.py` & `auth_fastapi-1.0.1/fastapi_auth/models/token.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/models/user.py` & `auth_fastapi-1.0.1/fastapi_auth/models/user.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/pagination/base.py` & `auth_fastapi-1.0.1/fastapi_auth/pagination/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/pagination/limit_pagination.py` & `auth_fastapi-1.0.1/fastapi_auth/pagination/limit_pagination.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/pagination/page.py` & `auth_fastapi-1.0.1/fastapi_auth/pagination/page.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/pagination/page_pagination.py` & `auth_fastapi-1.0.1/fastapi_auth/pagination/page_pagination.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/repositories/base.py` & `auth_fastapi-1.0.1/fastapi_auth/repositories/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/serializers/base.py` & `auth_fastapi-1.0.1/fastapi_auth/serializers/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/serializers/serializers.py` & `auth_fastapi-1.0.1/fastapi_auth/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/serializers/sqlalchemy/serializers.py` & `auth_fastapi-1.0.1/fastapi_auth/serializers/sqlalchemy/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,22 +32,23 @@
 
         fields = cls.Meta.fields
         mapper = class_mapper(cls.Meta.model)
         annotations = cls.__annotations__
         for prop in mapper.iterate_properties:
             if prop.key not in annotations:
                 if not isinstance(prop, Relationship):
-                    if fields != "__all__" and prop.key in fields:
-                        try:
-                            if prop.columns[0].expression.nullable:
-                                annotations[prop.columns[0].description] = Optional[prop.columns[0].type.python_type]
-                            else:
-                                annotations[prop.columns[0].description] = prop.columns[0].type.python_type
-                        except NotImplementedError:
-                            raise TypeError(f"Unknown type {prop.key}")
+                    if fields != "__all__":
+                        if prop.key in fields:
+                            try:
+                                if prop.columns[0].expression.nullable:
+                                    annotations[prop.columns[0].description] = Optional[prop.columns[0].type.python_type]
+                                else:
+                                    annotations[prop.columns[0].description] = prop.columns[0].type.python_type
+                            except NotImplementedError:
+                                raise TypeError(f"Unknown type {prop.key}")
                     else:
                         try:
                             if prop.columns[0].expression.nullable:
                                 annotations[prop.columns[0].description] = Optional[prop.columns[0].type.python_type]
                             else:
                                 annotations[prop.columns[0].description] = prop.columns[0].type.python_type
                         except NotImplementedError:
```

### Comparing `auth_fastapi-1.0.0/fastapi_auth/serializers/tortoise/serializers.py` & `auth_fastapi-1.0.1/fastapi_auth/serializers/tortoise/serializers.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/signals/signal.py` & `auth_fastapi-1.0.1/fastapi_auth/signals/signal.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/sqlalchemy_models/__init__.py` & `auth_fastapi-1.0.1/fastapi_auth/sqlalchemy_models/__init__.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/strategies/base.py` & `auth_fastapi-1.0.1/fastapi_auth/strategies/base.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/strategies/db.py` & `auth_fastapi-1.0.1/fastapi_auth/strategies/db.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/strategies/jwt.py` & `auth_fastapi-1.0.1/fastapi_auth/strategies/jwt.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/utils/command_utils.py` & `auth_fastapi-1.0.1/fastapi_auth/utils/command_utils.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/fastapi_auth/utils/utils.py` & `auth_fastapi-1.0.1/fastapi_auth/utils/utils.py`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/README.md` & `auth_fastapi-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/pyproject.toml` & `auth_fastapi-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `auth_fastapi-1.0.0/PKG-INFO` & `auth_fastapi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: auth_fastapi
-Version: 1.0.0
+Version: 1.0.1
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
-Metadata-Version: 2.3 Name: auth_fastapi Version: 1.0.0 Summary: Authentication
+Metadata-Version: 2.3 Name: auth_fastapi Version: 1.0.1 Summary: Authentication
 library for FastAPI for fast migration from Django/DRF. Serializers, signals,
 permissions, pagination and filters included. Project-URL: Source, https://
 github.com/zayycev22/fastapi-auth Author: zayycev22 Classifier: Framework ::
 FastAPI Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

