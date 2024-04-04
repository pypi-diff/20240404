# Comparing `tmp/dddesign-0.0.4.tar.gz` & `tmp/dddesign-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dddesign-0.0.4.tar", max compression
+gzip compressed data, was "dddesign-0.0.5.tar", max compression
```

## Comparing `dddesign-0.0.4.tar` & `dddesign-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1070 2024-04-04 20:54:56.863445 dddesign-0.0.4/LICENSE
--rw-r--r--   0        0        0       10 2024-04-04 20:54:56.863445 dddesign-0.0.4/README.md
--rw-r--r--   0        0        0       54 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/__init__.py
--rw-r--r--   0        0        0       68 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/__init__.py
--rw-r--r--   0        0        0      118 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/applications/__init__.py
--rw-r--r--   0        0        0      151 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/applications/application.py
--rw-r--r--   0        0        0    10184 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/applications/application_factory.py
--rw-r--r--   0        0        0       84 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/__init__.py
--rw-r--r--   0        0        0       90 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/aggregates/__init__.py
--rw-r--r--   0        0        0      153 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/aggregates/aggregate.py
--rw-r--r--   0        0        0     7850 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/aggregates/aggregate_list_factory.py
--rw-r--r--   0        0        0       32 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/constants/__init__.py
--rw-r--r--   0        0        0      204 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/constants/base_enum.py
--rw-r--r--   0        0        0       36 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/dto/__init__.py
--rw-r--r--   0        0        0      158 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/dto/dto.py
--rw-r--r--   0        0        0       27 2024-04-04 20:54:56.863445 dddesign-0.0.4/dddesign/structure/domains/entities/__init__.py
--rw-r--r--   0        0        0      433 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/domains/entities/entity.py
--rw-r--r--   0        0        0       80 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/domains/errors/__init__.py
--rw-r--r--   0        0        0     1407 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/domains/errors/base_error.py
--rw-r--r--   0        0        0      765 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/domains/errors/collection_error.py
--rw-r--r--   0        0        0       32 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/domains/types/__init__.py
--rw-r--r--   0        0        0      267 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/domains/types/base_type.py
--rw-r--r--   0        0        0       38 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/domains/value_objects/__init__.py
--rw-r--r--   0        0        0      151 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/domains/value_objects/value_object.py
--rw-r--r--   0        0        0       39 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/infrastructure/__init__.py
--rw-r--r--   0        0        0       35 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/infrastructure/adapters/__init__.py
--rw-r--r--   0        0        0       46 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/infrastructure/adapters/external/__init__.py
--rw-r--r--   0        0        0      155 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/infrastructure/adapters/external/external_adapter.py
--rw-r--r--   0        0        0       46 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/infrastructure/adapters/internal/__init__.py
--rw-r--r--   0        0        0      155 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/infrastructure/adapters/internal/internal_adapter.py
--rw-r--r--   0        0        0       35 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      150 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/infrastructure/repositories/repository.py
--rw-r--r--   0        0        0       29 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/services/__init__.py
--rw-r--r--   0        0        0      262 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/structure/services/service.py
--rw-r--r--   0        0        0       68 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/types/__init__.py
--rw-r--r--   0        0        0      381 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/types/email_str.py
--rw-r--r--   0        0        0     1431 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/types/string_uuid.py
--rw-r--r--   0        0        0       26 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/unittest/__init__.py
--rw-r--r--   0        0        0      659 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/unittest/magic_mock.py
--rw-r--r--   0        0        0      125 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/__init__.py
--rw-r--r--   0        0        0      152 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/base_model/__init__.py
--rw-r--r--   0        0        0     1458 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/base_model/changes_tracker.py
--rw-r--r--   0        0        0      506 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/base_model/error_instance_factory.py
--rw-r--r--   0        0        0      926 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/base_model/error_wrapper.py
--rw-r--r--   0        0        0      156 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/convertors.py
--rw-r--r--   0        0        0     2890 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/function_exceptions_extractor.py
--rw-r--r--   0        0        0      636 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/module_getter.py
--rw-r--r--   0        0        0     1365 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/safe_decorators.py
--rw-r--r--   0        0        0      174 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/sequence_helpers.py
--rw-r--r--   0        0        0     2292 2024-04-04 20:54:56.867445 dddesign-0.0.4/dddesign/utils/type_helpers.py
--rw-r--r--   0        0        0      648 2024-04-04 20:54:56.867445 dddesign-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 dddesign-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-04 21:04:24.552297 dddesign-0.0.5/LICENSE
+-rw-r--r--   0        0        0       10 2024-04-04 21:04:24.552297 dddesign-0.0.5/README.md
+-rw-r--r--   0        0        0       54 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/__init__.py
+-rw-r--r--   0        0        0      118 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/applications/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/applications/application.py
+-rw-r--r--   0        0        0    10184 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/applications/application_factory.py
+-rw-r--r--   0        0        0       84 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/aggregates/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/aggregates/aggregate.py
+-rw-r--r--   0        0        0     7850 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/aggregates/aggregate_list_factory.py
+-rw-r--r--   0        0        0       32 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/constants/__init__.py
+-rw-r--r--   0        0        0      204 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/constants/base_enum.py
+-rw-r--r--   0        0        0       36 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/dto/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/dto/dto.py
+-rw-r--r--   0        0        0       27 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/entities/__init__.py
+-rw-r--r--   0        0        0      433 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/entities/entity.py
+-rw-r--r--   0        0        0       80 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/errors/__init__.py
+-rw-r--r--   0        0        0     1407 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/errors/base_error.py
+-rw-r--r--   0        0        0      765 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/errors/collection_error.py
+-rw-r--r--   0        0        0       32 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/types/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/types/base_type.py
+-rw-r--r--   0        0        0       38 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/value_objects/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/domains/value_objects/value_object.py
+-rw-r--r--   0        0        0       39 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/infrastructure/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/infrastructure/adapters/__init__.py
+-rw-r--r--   0        0        0       46 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/infrastructure/adapters/external/__init__.py
+-rw-r--r--   0        0        0      155 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/infrastructure/adapters/external/external_adapter.py
+-rw-r--r--   0        0        0       46 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/infrastructure/adapters/internal/__init__.py
+-rw-r--r--   0        0        0      155 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/infrastructure/adapters/internal/internal_adapter.py
+-rw-r--r--   0        0        0       35 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/infrastructure/repositories/repository.py
+-rw-r--r--   0        0        0       29 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/services/__init__.py
+-rw-r--r--   0        0        0      262 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/structure/services/service.py
+-rw-r--r--   0        0        0       68 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/types/__init__.py
+-rw-r--r--   0        0        0      381 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/types/email_str.py
+-rw-r--r--   0        0        0     1431 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/types/string_uuid.py
+-rw-r--r--   0        0        0       26 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/unittest/__init__.py
+-rw-r--r--   0        0        0      659 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/unittest/magic_mock.py
+-rw-r--r--   0        0        0      125 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/base_model/__init__.py
+-rw-r--r--   0        0        0     1458 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/base_model/changes_tracker.py
+-rw-r--r--   0        0        0      506 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/base_model/error_instance_factory.py
+-rw-r--r--   0        0        0      926 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/base_model/error_wrapper.py
+-rw-r--r--   0        0        0      156 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/convertors.py
+-rw-r--r--   0        0        0     2890 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/function_exceptions_extractor.py
+-rw-r--r--   0        0        0      636 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/module_getter.py
+-rw-r--r--   0        0        0     1365 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/safe_decorators.py
+-rw-r--r--   0        0        0      174 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/sequence_helpers.py
+-rw-r--r--   0        0        0     2292 2024-04-04 21:04:24.552297 dddesign-0.0.5/dddesign/utils/type_helpers.py
+-rw-r--r--   0        0        0      680 2024-04-04 21:04:24.552297 dddesign-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      753 1970-01-01 00:00:00.000000 dddesign-0.0.5/PKG-INFO
```

### Comparing `dddesign-0.0.4/LICENSE` & `dddesign-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/structure/applications/application_factory.py` & `dddesign-0.0.5/dddesign/structure/applications/application_factory.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/structure/domains/aggregates/aggregate_list_factory.py` & `dddesign-0.0.5/dddesign/structure/domains/aggregates/aggregate_list_factory.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/structure/domains/errors/base_error.py` & `dddesign-0.0.5/dddesign/structure/domains/errors/base_error.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/structure/domains/errors/collection_error.py` & `dddesign-0.0.5/dddesign/structure/domains/errors/collection_error.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/types/string_uuid.py` & `dddesign-0.0.5/dddesign/types/string_uuid.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/unittest/magic_mock.py` & `dddesign-0.0.5/dddesign/unittest/magic_mock.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/utils/base_model/changes_tracker.py` & `dddesign-0.0.5/dddesign/utils/base_model/changes_tracker.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/utils/base_model/error_wrapper.py` & `dddesign-0.0.5/dddesign/utils/base_model/error_wrapper.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/utils/function_exceptions_extractor.py` & `dddesign-0.0.5/dddesign/utils/function_exceptions_extractor.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/utils/module_getter.py` & `dddesign-0.0.5/dddesign/utils/module_getter.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/utils/safe_decorators.py` & `dddesign-0.0.5/dddesign/utils/safe_decorators.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/dddesign/utils/type_helpers.py` & `dddesign-0.0.5/dddesign/utils/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dddesign-0.0.4/pyproject.toml` & `dddesign-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "dddesign"
 description = "Domain Driven Design Library"
-version = "0.0.4"
+version = "0.0.5"
 authors = ["davyddd"]
 license = "MIT"
 repository = "https://github.com/davyddd/dddesign"
 readme = "README.md"
 keywords = ["python", "ddd", "domain driven design", "ddd architecture", "ddd structure", "architecture", "structure", "dddesign"]
 packages = [{include = "dddesign"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-pydantic = "^1.10"
+pydantic = {version = "^1.10", extras = ["email"]}
 
 [tool.poetry.group.dev.dependencies]
 mypy = "1.1.1"
 ruff = "0.1.7"
 ipdb = "0.13.9"
 ipython = "8.12.3"
 pytest = "8.1.1"
```

### Comparing `dddesign-0.0.4/PKG-INFO` & `dddesign-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: dddesign
-Version: 0.0.4
+Version: 0.0.5
 Summary: Domain Driven Design Library
 Home-page: https://github.com/davyddd/dddesign
 License: MIT
 Keywords: python,ddd,domain driven design,ddd architecture,ddd structure,architecture,structure,dddesign
 Author: davyddd
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.10,<2.0)
+Requires-Dist: pydantic[email] (>=1.10,<2.0)
 Project-URL: Repository, https://github.com/davyddd/dddesign
 Description-Content-Type: text/markdown
 
 # dddesign
```
