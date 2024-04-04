# Comparing `tmp/inoopa_utils-2.5.0.tar.gz` & `tmp/inoopa_utils-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inoopa_utils-2.5.0.tar", max compression
+gzip compressed data, was "inoopa_utils-2.6.0.tar", max compression
```

## Comparing `inoopa_utils-2.5.0.tar` & `inoopa_utils-2.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      953 2024-03-11 12:17:35.204315 inoopa_utils-2.5.0/README.md
--rw-r--r--   0        0        0        0 2023-11-06 09:05:33.934711 inoopa_utils-2.5.0/inoopa_utils/__init__.py
--rw-r--r--   0        0        0     1781 2024-03-08 11:42:35.645264 inoopa_utils-2.5.0/inoopa_utils/address_parser.py
--rw-r--r--   0        0        0     6238 2024-03-08 11:42:34.540729 inoopa_utils-2.5.0/inoopa_utils/batch_processing.py
--rw-r--r--   0        0        0        0 2024-03-08 11:43:03.997156 inoopa_utils-2.5.0/inoopa_utils/custom_types/__init__.py
--rw-r--r--   0        0        0     9136 2024-03-08 11:43:05.631896 inoopa_utils-2.5.0/inoopa_utils/custom_types/companies.py
--rw-r--r--   0        0        0      801 2024-03-08 11:43:06.928124 inoopa_utils-2.5.0/inoopa_utils/custom_types/decision_makers.py
--rw-r--r--   0        0        0      117 2024-03-08 11:43:11.918631 inoopa_utils-2.5.0/inoopa_utils/custom_types/exceptions.py
--rw-r--r--   0        0        0     2297 2024-03-27 12:13:56.455959 inoopa_utils-2.5.0/inoopa_utils/custom_types/typesense_schemas.py
--rw-r--r--   0        0        0      358 2024-03-08 11:43:09.416778 inoopa_utils-2.5.0/inoopa_utils/custom_types/websites.py
--rw-r--r--   0        0        0     1720 2024-03-08 11:42:33.437130 inoopa_utils-2.5.0/inoopa_utils/inoopa_logging.py
--rw-r--r--   0        0        0    16195 2024-03-08 11:42:26.507548 inoopa_utils-2.5.0/inoopa_utils/mongodb_helpers.py
--rw-r--r--   0        0        0     3207 2024-03-27 14:28:43.391739 inoopa_utils-2.5.0/inoopa_utils/openai_helpers.py
--rw-r--r--   0        0        0     4243 2024-03-08 11:42:32.029627 inoopa_utils-2.5.0/inoopa_utils/rabbitmq_helpers.py
--rw-r--r--   0        0        0     4871 2024-03-08 11:42:30.821464 inoopa_utils-2.5.0/inoopa_utils/sql_helpers.py
--rw-r--r--   0        0        0      427 2023-11-06 09:54:38.711474 inoopa_utils-2.5.0/inoopa_utils/tests/test_logging.py
--rw-r--r--   0        0        0      627 2023-11-06 12:56:31.343962 inoopa_utils-2.5.0/inoopa_utils/tests/test_rabbitmq.py
--rw-r--r--   0        0        0    10729 2024-03-27 13:56:59.695059 inoopa_utils-2.5.0/inoopa_utils/typesense_helpers.py
--rw-r--r--   0        0        0        0 2023-11-06 00:28:42.240779 inoopa_utils-2.5.0/inoopa_utils/utils/__init__.py
--rw-r--r--   0        0        0      368 2024-03-08 11:43:44.438533 inoopa_utils-2.5.0/inoopa_utils/utils/env_variables_helper.py
--rw-r--r--   0        0        0      144 2024-03-08 11:43:22.052184 inoopa_utils-2.5.0/inoopa_utils/utils/exceptions.py
--rw-r--r--   0        0        0      662 2024-03-27 14:28:54.938875 inoopa_utils-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 inoopa_utils-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0      953 2024-03-11 12:17:35.204315 inoopa_utils-2.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-11-06 09:05:33.934711 inoopa_utils-2.6.0/inoopa_utils/__init__.py
+-rw-r--r--   0        0        0     1781 2024-03-08 11:42:35.645264 inoopa_utils-2.6.0/inoopa_utils/address_parser.py
+-rw-r--r--   0        0        0     6238 2024-03-08 11:42:34.540729 inoopa_utils-2.6.0/inoopa_utils/batch_processing.py
+-rw-r--r--   0        0        0        0 2024-03-08 11:43:03.997156 inoopa_utils-2.6.0/inoopa_utils/custom_types/__init__.py
+-rw-r--r--   0        0        0     9136 2024-03-08 11:43:05.631896 inoopa_utils-2.6.0/inoopa_utils/custom_types/companies.py
+-rw-r--r--   0        0        0      801 2024-03-08 11:43:06.928124 inoopa_utils-2.6.0/inoopa_utils/custom_types/decision_makers.py
+-rw-r--r--   0        0        0      117 2024-03-08 11:43:11.918631 inoopa_utils-2.6.0/inoopa_utils/custom_types/exceptions.py
+-rw-r--r--   0        0        0     1940 2024-04-04 10:56:25.695895 inoopa_utils-2.6.0/inoopa_utils/custom_types/typesense_schemas.py
+-rw-r--r--   0        0        0      358 2024-03-08 11:43:09.416778 inoopa_utils-2.6.0/inoopa_utils/custom_types/websites.py
+-rw-r--r--   0        0        0     1720 2024-03-08 11:42:33.437130 inoopa_utils-2.6.0/inoopa_utils/inoopa_logging.py
+-rw-r--r--   0        0        0    16195 2024-03-08 11:42:26.507548 inoopa_utils-2.6.0/inoopa_utils/mongodb_helpers.py
+-rw-r--r--   0        0        0     3207 2024-03-27 14:28:43.391739 inoopa_utils-2.6.0/inoopa_utils/openai_helpers.py
+-rw-r--r--   0        0        0     4243 2024-03-08 11:42:32.029627 inoopa_utils-2.6.0/inoopa_utils/rabbitmq_helpers.py
+-rw-r--r--   0        0        0     4871 2024-03-08 11:42:30.821464 inoopa_utils-2.6.0/inoopa_utils/sql_helpers.py
+-rw-r--r--   0        0        0      427 2023-11-06 09:54:38.711474 inoopa_utils-2.6.0/inoopa_utils/tests/test_logging.py
+-rw-r--r--   0        0        0      627 2023-11-06 12:56:31.343962 inoopa_utils-2.6.0/inoopa_utils/tests/test_rabbitmq.py
+-rw-r--r--   0        0        0    11819 2024-04-04 10:56:04.473918 inoopa_utils-2.6.0/inoopa_utils/typesense_helpers.py
+-rw-r--r--   0        0        0        0 2023-11-06 00:28:42.240779 inoopa_utils-2.6.0/inoopa_utils/utils/__init__.py
+-rw-r--r--   0        0        0      368 2024-03-08 11:43:44.438533 inoopa_utils-2.6.0/inoopa_utils/utils/env_variables_helper.py
+-rw-r--r--   0        0        0      144 2024-03-08 11:43:22.052184 inoopa_utils-2.6.0/inoopa_utils/utils/exceptions.py
+-rw-r--r--   0        0        0      662 2024-04-04 10:56:51.853763 inoopa_utils-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 inoopa_utils-2.6.0/PKG-INFO
```

### Comparing `inoopa_utils-2.5.0/README.md` & `inoopa_utils-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/address_parser.py` & `inoopa_utils-2.6.0/inoopa_utils/address_parser.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/batch_processing.py` & `inoopa_utils-2.6.0/inoopa_utils/batch_processing.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/custom_types/companies.py` & `inoopa_utils-2.6.0/inoopa_utils/custom_types/companies.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/custom_types/decision_makers.py` & `inoopa_utils-2.6.0/inoopa_utils/custom_types/decision_makers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/custom_types/typesense_schemas.py` & `inoopa_utils-2.6.0/inoopa_utils/custom_types/typesense_schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,38 +12,30 @@
     label_en_embedding: list[float] | None = None
     label_fr: str | None = None
     label_fr_embedding: list[float] | None = None
     label_nl: str | None = None
     label_nl_embedding: list[float] | None = None
 
 
-@dataclass(slots=True)
-class EstablishmentNameTypesense:
-    name: str
-    name_embedding: list[float] | None = None
-    name_fr: str | None = None
-    name_fr_embedding: list[float] | None = None
-    name_nl: str | None = None
-    name_nl_embedding: list[float] | None = None
-    establishments: list[str] | None = None
-    establishments_fr: list[str] | None = None
-    establishments_nl: list[str] | None = None
-
 
 @dataclass(slots=True)
-class CompanyNameTypesense:
-    name: str
+class EntityName:
+    name: str | None = None
     name_embedding: list[float] | None = None
     name_fr: str | None = None
     name_fr_embedding: list[float] | None = None
     name_nl: str | None = None
     name_nl_embedding: list[float] | None = None
     name_de: str | None = None
     name_de_embedding: list[float] | None = None
-    establishments: list[EstablishmentNameTypesense] | None = None
+
+
+@dataclass(EntityName, slots=True)
+class CompanyNameTypesense:
+    establishments_names: list[EntityName] | None = None
 
 
 @dataclass(slots=True)
 class OnlineContentTypesense:
     companies_id: list[str] | None = None
     facebook_page_url: str | None = None
     facebook_page_text: str | None = None
```

### Comparing `inoopa_utils-2.5.0/inoopa_utils/inoopa_logging.py` & `inoopa_utils-2.6.0/inoopa_utils/inoopa_logging.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/mongodb_helpers.py` & `inoopa_utils-2.6.0/inoopa_utils/mongodb_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/openai_helpers.py` & `inoopa_utils-2.6.0/inoopa_utils/openai_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/rabbitmq_helpers.py` & `inoopa_utils-2.6.0/inoopa_utils/rabbitmq_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/sql_helpers.py` & `inoopa_utils-2.6.0/inoopa_utils/sql_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/tests/test_rabbitmq.py` & `inoopa_utils-2.6.0/inoopa_utils/tests/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.5.0/inoopa_utils/typesense_helpers.py` & `inoopa_utils-2.6.0/inoopa_utils/typesense_helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,52 +6,57 @@
 import typesense
 from typesense import exceptions
 from typesense.collection import Collection
 
 from inoopa_utils.inoopa_logging import create_logger
 
 
-EMBEDDING_MODEL = 'text-embedding-3-small'
+EMBEDDING_MODEL = "text-embedding-3-small"
 EMBEDDING_CONTEXT_MAX_LENGTH = 8191
-EMBEDDING_ENCODING = 'cl100k_base'
+EMBEDDING_ENCODING = "cl100k_base"
 # For the model name to typesense's namming convention
 EMBEDDING_MODEL_TYPESENSE_NAME = f"openai/{EMBEDDING_MODEL}"
+OPENAI_API_KEY = os.environ["OPENAI_API_KEY"]
 
 
 class TypesenseManager:
     """
     This class is a client to interact with the Typesense search engine server (deployed in InfraV2).
     You can then is the client outside of the class to interact with the Typesense server.
 
     It also take care of creating the collections if they don't exist.
     ! Please maintain the schemas in the same file as the TypesenseManager class. !
 
     :attribute typesense_url: The typesense server URL.
     :attribute client: The typesense client object to interact with the typesense server.
+    :attribute collection_nace_codes: The nace_codes collection object.
+    :attribute collection_companies_names: The companies_names collection object.
+    :attribute collection_online_content: The online_content collection object.
     """
     def __init__(
         self,
         host: str = os.environ["TYPESENSE_HOST"],
-        port: str = os.environ["TYPESENSE_PORT"],
+        port: str = os.getenv("TYPESENSE_PORT", 443), # Default port is 443 for HTTPS
         api_key: str = os.environ["TYPESENSE_API_KEY"],
+        protocol: str = "https",
     ):
         """
         :param host: Typesense's server host
         :param port: Typesense's server port
         :param api_key: Typesense's API key
         :param mongo_db_collection_name : define which MongoDB collection will be used
         """
         self._logger = create_logger("INOOPA.TYPESENSE.CLIENT")
         self.typesense_url = f"https://{host}"
         self.client: typesense.Client = typesense.Client({
             'api_key': api_key,
             'nodes': [{
                 'host': host,
                 'port': port,
-                'protocol': 'https'
+                'protocol': protocol,
             }],
             'connection_timeout_seconds': 10
         })
 
         # 1. Check the API's health
         self._check_server_heatlh()
         # 2. Create collections if they don't exist
@@ -124,15 +129,15 @@
             "type": "float[]",
             "embed": {
                 "from": [
                     "label_en"
                 ],
                 "model_config": {
                     "model_name": EMBEDDING_MODEL_TYPESENSE_NAME,
-                    "api_key": os.getenv("OPENAI_API_KEY")
+                    "api_key": OPENAI_API_KEY
                 }
             }
         },
         {
             "optional": True,
             "name": "label_fr",
             "type": "string"
@@ -143,15 +148,15 @@
             "type": "float[]",
             "embed": {
                 "from": [
                     "label_fr"
                 ],
                 "model_config": {
                     "model_name": EMBEDDING_MODEL_TYPESENSE_NAME,
-                    "api_key": os.getenv("OPENAI_API_KEY")
+                    "api_key": OPENAI_API_KEY
                 }
             }
         },
         {
             "optional": True,
             "name": "label_nl",
             "type": "string"
@@ -162,32 +167,49 @@
             "type": "float[]",
             "embed": {
                 "from": [
                     "label_nl"
                 ],
                 "model_config": {
                     "model_name": EMBEDDING_MODEL_TYPESENSE_NAME,
-                    "api_key": os.getenv("OPENAI_API_KEY")
+                    "api_key": OPENAI_API_KEY
                 }
             }
         },
     ]
 }
 
 # Contains all the companies and establishment names for name matching puprose
 companies_names_collection_schema = {
     "name": "companies_names",
     "enable_nested_fields": True,
     "fields": [
         {"optional" : True, "name": "name", "type": "string"},
+        {"optional" : True, "name": "name_embeddings", "type": "float[]"},
+
         {"optional" : True, "name": "name_fr", "type": "string" },
+        {"optional" : True, "name": "name_fr_embeddings", "type": "float[]" },
+
         {"optional" : True, "name": "name_nl", "type": "string"},
+        {"optional" : True, "name": "name_nl_embeddings", "type": "float[]"},
+
+        {"optional" : True, "name": "name_de", "type": "string"},
+        {"optional" : True, "name": "name_de_embeddings", "type": "float[]"},
+
         {"optional" : True, "name": "establishments.name", "type": "string[]"},
+        {"optional" : True, "name": "establishments.name_embeddings", "type": "float[][]"},
+
         {"optional" : True, "name": "establishments.name_fr", "type": "string[]"},
+        {"optional" : True, "name": "establishments.name_fr_embeddings", "type": "float[][]"},
+
         {"optional" : True, "name": "establishments.name_nl", "type": "string[]"},
+        {"optional" : True, "name": "establishments.name_nl_embeddings", "type": "float[][]"},
+
+        {"optional" : True, "name": "establishments.name_de", "type": "string[]"},
+        {"optional" : True, "name": "establishments.name_de_embeddings", "type": "float[][]"},
     ],
 }
 
 # Contain an online content. Ex: website, social network,... Used for search
 online_content_collection_schema = {
     "name": "online_content",
     "enable_nested_fields": True,
@@ -214,15 +236,15 @@
             "name": "facebook_page_embedding",
             "optional": True,
             "type": "float[]",
             "embed": {
                 "from": ["facebook_page_text"],
                 "model_config": {
                     "model_name": EMBEDDING_MODEL_TYPESENSE_NAME,
-                    "api_key": os.getenv("OPENAI_API_KEY")
+                    "api_key": OPENAI_API_KEY
                 }
             }
         },
 
         # ---- Google's content ----
         {
             "name": "google_my_business_url",
@@ -238,15 +260,15 @@
             "name": "google_my_business_embedding",
             "optional": True,
             "type": "float[]",
             "embed": {
                 "from": ["google_my_business_text"],
                 "model_config": {
                     "model_name": EMBEDDING_MODEL_TYPESENSE_NAME,
-                    "api_key": os.getenv("OPENAI_API_KEY")
+                    "api_key": OPENAI_API_KEY
                 }
             }
         },
 
         # ---- Websites' content ----
         {
             "name": "website_base_url",
@@ -273,15 +295,15 @@
             "optional": True,
             "name": "website_home_page_embedding",
             "type": "float[]",
             "embed": {
                 "from": ["website_home_page_text"],
                 "model_config": {
                     "model_name": EMBEDDING_MODEL_TYPESENSE_NAME,
-                    "api_key": os.getenv("OPENAI_API_KEY")
+                    "api_key": OPENAI_API_KEY
                 }
             }
         },
         # - About page -
         {
             "optional": True,
             "name": "website_about_page_url",
@@ -301,15 +323,15 @@
             "optional": True,
             "name": "website_about_page_embedding",
             "type": "float[]",
             "embed": {
                 "from": ["website_about_page_text"],
                 "model_config": {
                     "model_name": EMBEDDING_MODEL_TYPESENSE_NAME,
-                    "api_key": os.getenv("OPENAI_API_KEY")
+                    "api_key": OPENAI_API_KEY
                 }
             }
         },
         # - Contact page -
         {
             "optional": True,
             "name": "website_contact_page_url",
@@ -329,15 +351,15 @@
             "optional": True,
             "name": "website_contact_page_embedding",
             "type": "float[]",
             "embed": {
                 "from": ["website_contact_page_text"],
                 "model_config": {
                     "model_name": EMBEDDING_MODEL_TYPESENSE_NAME,
-                    "api_key": os.getenv("OPENAI_API_KEY")
+                    "api_key": OPENAI_API_KEY
                 }
             }
         }
     ]
 }
```

### Comparing `inoopa_utils-2.5.0/pyproject.toml` & `inoopa_utils-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "inoopa_utils"
 description = "Collection of utils used at Inoopa."
-version = "2.5.0"
+version = "2.6.0"
 authors = ["Dev Inoopa <dev@inoopa.com>"]
 packages = [{ include = "inoopa_utils" }]
 repository = "https://bitbucket.org/inoopa/inoopa_utils/"
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `inoopa_utils-2.5.0/PKG-INFO` & `inoopa_utils-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inoopa_utils
-Version: 2.5.0
+Version: 2.6.0
 Summary: Collection of utils used at Inoopa.
 Home-page: https://bitbucket.org/inoopa/inoopa_utils/
 Author: Dev Inoopa
 Author-email: dev@inoopa.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

