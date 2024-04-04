# Comparing `tmp/inoopa_utils-2.7.0.tar.gz` & `tmp/inoopa_utils-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inoopa_utils-2.7.0.tar", max compression
+gzip compressed data, was "inoopa_utils-2.8.0.tar", max compression
```

## Comparing `inoopa_utils-2.7.0.tar` & `inoopa_utils-2.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      953 2024-03-11 12:17:35.204315 inoopa_utils-2.7.0/README.md
--rw-r--r--   0        0        0        0 2023-11-06 09:05:33.934711 inoopa_utils-2.7.0/inoopa_utils/__init__.py
--rw-r--r--   0        0        0     1781 2024-03-08 11:42:35.645264 inoopa_utils-2.7.0/inoopa_utils/address_parser.py
--rw-r--r--   0        0        0     6238 2024-03-08 11:42:34.540729 inoopa_utils-2.7.0/inoopa_utils/batch_processing.py
--rw-r--r--   0        0        0        0 2024-03-08 11:43:03.997156 inoopa_utils-2.7.0/inoopa_utils/custom_types/__init__.py
--rw-r--r--   0        0        0     9136 2024-03-08 11:43:05.631896 inoopa_utils-2.7.0/inoopa_utils/custom_types/companies.py
--rw-r--r--   0        0        0      801 2024-03-08 11:43:06.928124 inoopa_utils-2.7.0/inoopa_utils/custom_types/decision_makers.py
--rw-r--r--   0        0        0      117 2024-03-08 11:43:11.918631 inoopa_utils-2.7.0/inoopa_utils/custom_types/exceptions.py
--rw-r--r--   0        0        0     1940 2024-04-04 10:56:25.695895 inoopa_utils-2.7.0/inoopa_utils/custom_types/typesense_schemas.py
--rw-r--r--   0        0        0      358 2024-03-08 11:43:09.416778 inoopa_utils-2.7.0/inoopa_utils/custom_types/websites.py
--rw-r--r--   0        0        0     1720 2024-03-08 11:42:33.437130 inoopa_utils-2.7.0/inoopa_utils/inoopa_logging.py
--rw-r--r--   0        0        0    16195 2024-03-08 11:42:26.507548 inoopa_utils-2.7.0/inoopa_utils/mongodb_helpers.py
--rw-r--r--   0        0        0     3207 2024-03-27 14:28:43.391739 inoopa_utils-2.7.0/inoopa_utils/openai_helpers.py
--rw-r--r--   0        0        0     4243 2024-03-08 11:42:32.029627 inoopa_utils-2.7.0/inoopa_utils/rabbitmq_helpers.py
--rw-r--r--   0        0        0     4871 2024-03-08 11:42:30.821464 inoopa_utils-2.7.0/inoopa_utils/sql_helpers.py
--rw-r--r--   0        0        0      427 2023-11-06 09:54:38.711474 inoopa_utils-2.7.0/inoopa_utils/tests/test_logging.py
--rw-r--r--   0        0        0      627 2023-11-06 12:56:31.343962 inoopa_utils-2.7.0/inoopa_utils/tests/test_rabbitmq.py
--rw-r--r--   0        0        0    11883 2024-04-04 11:00:18.240136 inoopa_utils-2.7.0/inoopa_utils/typesense_helpers.py
--rw-r--r--   0        0        0        0 2023-11-06 00:28:42.240779 inoopa_utils-2.7.0/inoopa_utils/utils/__init__.py
--rw-r--r--   0        0        0      368 2024-03-08 11:43:44.438533 inoopa_utils-2.7.0/inoopa_utils/utils/env_variables_helper.py
--rw-r--r--   0        0        0      144 2024-03-08 11:43:22.052184 inoopa_utils-2.7.0/inoopa_utils/utils/exceptions.py
--rw-r--r--   0        0        0      662 2024-04-04 11:00:40.963230 inoopa_utils-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 inoopa_utils-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0      953 2024-03-11 12:17:35.204315 inoopa_utils-2.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-11-06 09:05:33.934711 inoopa_utils-2.8.0/inoopa_utils/__init__.py
+-rw-r--r--   0        0        0     1781 2024-03-08 11:42:35.645264 inoopa_utils-2.8.0/inoopa_utils/address_parser.py
+-rw-r--r--   0        0        0     6238 2024-03-08 11:42:34.540729 inoopa_utils-2.8.0/inoopa_utils/batch_processing.py
+-rw-r--r--   0        0        0        0 2024-03-08 11:43:03.997156 inoopa_utils-2.8.0/inoopa_utils/custom_types/__init__.py
+-rw-r--r--   0        0        0     9136 2024-03-08 11:43:05.631896 inoopa_utils-2.8.0/inoopa_utils/custom_types/companies.py
+-rw-r--r--   0        0        0      801 2024-03-08 11:43:06.928124 inoopa_utils-2.8.0/inoopa_utils/custom_types/decision_makers.py
+-rw-r--r--   0        0        0      117 2024-03-08 11:43:11.918631 inoopa_utils-2.8.0/inoopa_utils/custom_types/exceptions.py
+-rw-r--r--   0        0        0     1953 2024-04-04 11:07:46.026938 inoopa_utils-2.8.0/inoopa_utils/custom_types/typesense_schemas.py
+-rw-r--r--   0        0        0      358 2024-03-08 11:43:09.416778 inoopa_utils-2.8.0/inoopa_utils/custom_types/websites.py
+-rw-r--r--   0        0        0     1720 2024-03-08 11:42:33.437130 inoopa_utils-2.8.0/inoopa_utils/inoopa_logging.py
+-rw-r--r--   0        0        0    16195 2024-03-08 11:42:26.507548 inoopa_utils-2.8.0/inoopa_utils/mongodb_helpers.py
+-rw-r--r--   0        0        0     3207 2024-03-27 14:28:43.391739 inoopa_utils-2.8.0/inoopa_utils/openai_helpers.py
+-rw-r--r--   0        0        0     4243 2024-03-08 11:42:32.029627 inoopa_utils-2.8.0/inoopa_utils/rabbitmq_helpers.py
+-rw-r--r--   0        0        0     4871 2024-03-08 11:42:30.821464 inoopa_utils-2.8.0/inoopa_utils/sql_helpers.py
+-rw-r--r--   0        0        0      427 2023-11-06 09:54:38.711474 inoopa_utils-2.8.0/inoopa_utils/tests/test_logging.py
+-rw-r--r--   0        0        0      627 2023-11-06 12:56:31.343962 inoopa_utils-2.8.0/inoopa_utils/tests/test_rabbitmq.py
+-rw-r--r--   0        0        0    11883 2024-04-04 11:00:18.240136 inoopa_utils-2.8.0/inoopa_utils/typesense_helpers.py
+-rw-r--r--   0        0        0        0 2023-11-06 00:28:42.240779 inoopa_utils-2.8.0/inoopa_utils/utils/__init__.py
+-rw-r--r--   0        0        0      368 2024-03-08 11:43:44.438533 inoopa_utils-2.8.0/inoopa_utils/utils/env_variables_helper.py
+-rw-r--r--   0        0        0      144 2024-03-08 11:43:22.052184 inoopa_utils-2.8.0/inoopa_utils/utils/exceptions.py
+-rw-r--r--   0        0        0      662 2024-04-04 11:08:01.166103 inoopa_utils-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 inoopa_utils-2.8.0/PKG-INFO
```

### Comparing `inoopa_utils-2.7.0/README.md` & `inoopa_utils-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/address_parser.py` & `inoopa_utils-2.8.0/inoopa_utils/address_parser.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/batch_processing.py` & `inoopa_utils-2.8.0/inoopa_utils/batch_processing.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/custom_types/companies.py` & `inoopa_utils-2.8.0/inoopa_utils/custom_types/companies.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/custom_types/decision_makers.py` & `inoopa_utils-2.8.0/inoopa_utils/custom_types/decision_makers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/custom_types/typesense_schemas.py` & `inoopa_utils-2.8.0/inoopa_utils/custom_types/typesense_schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     name_nl_embedding: list[float] | None = None
     name_de: str | None = None
     name_de_embedding: list[float] | None = None
 
 
 @dataclass(EntityName, slots=True)
 class CompanyNameTypesense:
+    _id: str
     establishments_names: list[EntityName] | None = None
 
 
 @dataclass(slots=True)
 class OnlineContentTypesense:
     companies_id: list[str] | None = None
     facebook_page_url: str | None = None
```

### Comparing `inoopa_utils-2.7.0/inoopa_utils/inoopa_logging.py` & `inoopa_utils-2.8.0/inoopa_utils/inoopa_logging.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/mongodb_helpers.py` & `inoopa_utils-2.8.0/inoopa_utils/mongodb_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/openai_helpers.py` & `inoopa_utils-2.8.0/inoopa_utils/openai_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/rabbitmq_helpers.py` & `inoopa_utils-2.8.0/inoopa_utils/rabbitmq_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/sql_helpers.py` & `inoopa_utils-2.8.0/inoopa_utils/sql_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/tests/test_rabbitmq.py` & `inoopa_utils-2.8.0/inoopa_utils/tests/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/inoopa_utils/typesense_helpers.py` & `inoopa_utils-2.8.0/inoopa_utils/typesense_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.7.0/pyproject.toml` & `inoopa_utils-2.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "inoopa_utils"
 description = "Collection of utils used at Inoopa."
-version = "2.7.0"
+version = "2.8.0"
 authors = ["Dev Inoopa <dev@inoopa.com>"]
 packages = [{ include = "inoopa_utils" }]
 repository = "https://bitbucket.org/inoopa/inoopa_utils/"
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `inoopa_utils-2.7.0/PKG-INFO` & `inoopa_utils-2.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inoopa_utils
-Version: 2.7.0
+Version: 2.8.0
 Summary: Collection of utils used at Inoopa.
 Home-page: https://bitbucket.org/inoopa/inoopa_utils/
 Author: Dev Inoopa
 Author-email: dev@inoopa.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

