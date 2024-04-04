# Comparing `tmp/chatbees_python_client-0.9.5.tar.gz` & `tmp/chatbees_python_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatbees_python_client-0.9.5.tar", max compression
+gzip compressed data, was "chatbees_python_client-1.0.0.tar", max compression
```

## Comparing `chatbees_python_client-0.9.5.tar` & `chatbees_python_client-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0    11342 2024-02-03 05:19:30.172255 chatbees_python_client-0.9.5/LICENSE
--rw-r--r--   0        0        0     6073 2024-02-11 21:33:26.595699 chatbees_python_client-0.9.5/README.md
--rw-r--r--   0        0        0      271 2024-03-02 06:55:50.362492 chatbees_python_client-0.9.5/chatbees/__init__.py
--rw-r--r--   0        0        0        0 2024-02-03 05:19:30.172668 chatbees_python_client-0.9.5/chatbees/client/__init__.py
--rw-r--r--   0        0        0     1460 2024-02-11 21:33:26.596005 chatbees_python_client-0.9.5/chatbees/client/admin_management.py
--rw-r--r--   0        0        0     2739 2024-02-07 18:36:45.796000 chatbees_python_client-0.9.5/chatbees/client/collection_management.py
--rw-r--r--   0        0        0        0 2024-02-03 05:19:30.173002 chatbees_python_client-0.9.5/chatbees/client_models/__init__.py
--rw-r--r--   0        0        0      974 2024-03-02 06:48:17.127868 chatbees_python_client-0.9.5/chatbees/client_models/chat.py
--rw-r--r--   0        0        0    12173 2024-03-04 22:07:02.125192 chatbees_python_client-0.9.5/chatbees/client_models/collection.py
--rw-r--r--   0        0        0        0 2024-02-03 05:19:30.173430 chatbees_python_client-0.9.5/chatbees/server_models/__init__.py
--rw-r--r--   0        0        0      138 2024-02-11 21:33:17.343641 chatbees_python_client-0.9.5/chatbees/server_models/admin_api.py
--rw-r--r--   0        0        0      684 2024-02-06 18:41:34.330037 chatbees_python_client-0.9.5/chatbees/server_models/chat.py
--rw-r--r--   0        0        0      812 2024-03-02 06:52:45.710414 chatbees_python_client-0.9.5/chatbees/server_models/collection_api.py
--rw-r--r--   0        0        0     2329 2024-03-04 18:14:25.037767 chatbees_python_client-0.9.5/chatbees/server_models/doc_api.py
--rw-r--r--   0        0        0      640 2024-03-04 22:18:48.317703 chatbees_python_client-0.9.5/chatbees/server_models/ingestion_api.py
--rw-r--r--   0        0        0      460 2024-03-04 05:35:32.118837 chatbees_python_client-0.9.5/chatbees/server_models/ingestion_type.py
--rw-r--r--   0        0        0      358 2024-03-02 06:52:45.706561 chatbees_python_client-0.9.5/chatbees/server_models/search_api.py
--rw-r--r--   0        0        0    11482 2024-03-04 05:38:54.678077 chatbees_python_client-0.9.5/chatbees/tests/api_surface_test.py
--rw-r--r--   0        0        0       39 2024-02-03 05:19:30.174160 chatbees_python_client-0.9.5/chatbees/tests/data/española.txt
--rw-r--r--   0        0        0       32 2024-02-03 05:19:30.174268 chatbees_python_client-0.9.5/chatbees/tests/data/française.txt
--rw-r--r--   0        0        0      463 2024-02-03 05:19:30.174378 chatbees_python_client-0.9.5/chatbees/tests/data/text_file.txt
--rw-r--r--   0        0        0       30 2024-02-03 05:19:30.174477 chatbees_python_client-0.9.5/chatbees/tests/data/中文.txt
--rw-r--r--   0        0        0     8156 2024-03-04 05:36:31.980841 chatbees_python_client-0.9.5/chatbees/tests/smoke_test.py
--rw-r--r--   0        0        0        0 2024-02-03 05:19:30.174691 chatbees_python_client-0.9.5/chatbees/utils/__init__.py
--rw-r--r--   0        0        0     1022 2024-02-06 18:39:33.176649 chatbees_python_client-0.9.5/chatbees/utils/ask.py
--rw-r--r--   0        0        0     1638 2024-03-02 06:40:30.984218 chatbees_python_client-0.9.5/chatbees/utils/config.py
--rw-r--r--   0        0        0     1709 2024-02-03 05:19:30.174998 chatbees_python_client-0.9.5/chatbees/utils/exceptions.py
--rw-r--r--   0        0        0      729 2024-02-03 05:19:30.175089 chatbees_python_client-0.9.5/chatbees/utils/file_upload.py
--rw-r--r--   0        0        0      477 2024-03-05 18:07:01.986725 chatbees_python_client-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 chatbees_python_client-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-02-03 05:19:30.172255 chatbees_python_client-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6073 2024-02-11 21:33:26.595699 chatbees_python_client-1.0.0/README.md
+-rw-r--r--   0        0        0     6148 2024-03-20 20:25:04.619495 chatbees_python_client-1.0.0/chatbees/.DS_Store
+-rw-r--r--   0        0        0      271 2024-04-04 16:21:08.597061 chatbees_python_client-1.0.0/chatbees/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-03 05:19:30.172668 chatbees_python_client-1.0.0/chatbees/client/__init__.py
+-rw-r--r--   0        0        0     1460 2024-02-11 21:33:26.596005 chatbees_python_client-1.0.0/chatbees/client/admin_management.py
+-rw-r--r--   0        0        0     3536 2024-04-04 16:21:08.597882 chatbees_python_client-1.0.0/chatbees/client/collection_management.py
+-rw-r--r--   0        0        0        0 2024-02-03 05:19:30.173002 chatbees_python_client-1.0.0/chatbees/client_models/__init__.py
+-rw-r--r--   0        0        0      974 2024-04-04 16:21:08.598133 chatbees_python_client-1.0.0/chatbees/client_models/chat.py
+-rw-r--r--   0        0        0    12283 2024-04-04 16:21:08.598329 chatbees_python_client-1.0.0/chatbees/client_models/collection.py
+-rw-r--r--   0        0        0        0 2024-02-03 05:19:30.173430 chatbees_python_client-1.0.0/chatbees/server_models/__init__.py
+-rw-r--r--   0        0        0      138 2024-02-11 21:33:17.343641 chatbees_python_client-1.0.0/chatbees/server_models/admin_api.py
+-rw-r--r--   0        0        0      684 2024-02-06 18:41:34.330037 chatbees_python_client-1.0.0/chatbees/server_models/chat.py
+-rw-r--r--   0        0        0      998 2024-04-04 16:21:08.598469 chatbees_python_client-1.0.0/chatbees/server_models/collection_api.py
+-rw-r--r--   0        0        0     2329 2024-04-04 16:21:08.598600 chatbees_python_client-1.0.0/chatbees/server_models/doc_api.py
+-rw-r--r--   0        0        0      640 2024-04-04 16:21:08.598825 chatbees_python_client-1.0.0/chatbees/server_models/ingestion_api.py
+-rw-r--r--   0        0        0      841 2024-04-04 16:21:08.598928 chatbees_python_client-1.0.0/chatbees/server_models/ingestion_type.py
+-rw-r--r--   0        0        0      358 2024-04-04 16:21:08.599119 chatbees_python_client-1.0.0/chatbees/server_models/search_api.py
+-rw-r--r--   0        0        0    11482 2024-04-04 16:21:08.599399 chatbees_python_client-1.0.0/chatbees/tests/api_surface_test.py
+-rw-r--r--   0        0        0       39 2024-02-03 05:19:30.174160 chatbees_python_client-1.0.0/chatbees/tests/data/española.txt
+-rw-r--r--   0        0        0       32 2024-02-03 05:19:30.174268 chatbees_python_client-1.0.0/chatbees/tests/data/française.txt
+-rw-r--r--   0        0        0      463 2024-02-03 05:19:30.174378 chatbees_python_client-1.0.0/chatbees/tests/data/text_file.txt
+-rw-r--r--   0        0        0       30 2024-02-03 05:19:30.174477 chatbees_python_client-1.0.0/chatbees/tests/data/中文.txt
+-rw-r--r--   0        0        0     8527 2024-04-04 16:21:08.599719 chatbees_python_client-1.0.0/chatbees/tests/smoke_test.py
+-rw-r--r--   0        0        0        0 2024-02-03 05:19:30.174691 chatbees_python_client-1.0.0/chatbees/utils/__init__.py
+-rw-r--r--   0        0        0     1022 2024-02-06 18:39:33.176649 chatbees_python_client-1.0.0/chatbees/utils/ask.py
+-rw-r--r--   0        0        0     1638 2024-03-11 18:24:32.039859 chatbees_python_client-1.0.0/chatbees/utils/config.py
+-rw-r--r--   0        0        0     1709 2024-02-03 05:19:30.174998 chatbees_python_client-1.0.0/chatbees/utils/exceptions.py
+-rw-r--r--   0        0        0      729 2024-04-04 16:20:59.474400 chatbees_python_client-1.0.0/chatbees/utils/file_upload.py
+-rw-r--r--   0        0        0      477 2024-04-04 16:21:45.575686 chatbees_python_client-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 chatbees_python_client-1.0.0/PKG-INFO
```

### Comparing `chatbees_python_client-0.9.5/LICENSE` & `chatbees_python_client-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/README.md` & `chatbees_python_client-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/client/admin_management.py` & `chatbees_python_client-1.0.0/chatbees/client/admin_management.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/client/collection_management.py` & `chatbees_python_client-1.0.0/chatbees/client/collection_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,26 @@
     Collection,
     describe_response_to_collection,
 )
 from chatbees.utils.config import Config
 
 from chatbees.server_models.collection_api import (
     CreateCollectionRequest,
+    ConfigureCollectionRequest,
     ListCollectionsRequest,
     ListCollectionsResponse,
     DeleteCollectionRequest,
     DescribeCollectionRequest,
     DescribeCollectionResponse,
 )
 
 __all__ = [
     "create_collection",
     "collection",
+    "configure_collection",
     "list_collections",
     "delete_collection",
     "describe_collection",
 ]
 
 
 def create_collection(col: Collection) -> Collection:
@@ -53,14 +55,35 @@
 
     Returns:
         Collection: The collection object.
     """
     return Collection(name=collection_name)
 
 
+def configure_collection(
+    collection_name: str, public_read: bool = None, description: str = None):
+    """
+    Configure a collection.
+
+    Args:
+        collection_name (str): The name of the collection.
+        public_read (bool): Enable/disable public_read for the collection.
+        description (str): Update the description for the collection.
+    """
+    req = ConfigureCollectionRequest(
+        namespace_name=Config.namespace,
+        collection_name=collection_name)
+    if public_read is not None:
+        req.public_read = public_read
+    if description is not None:
+        req.description = description
+    url = f'{Config.get_base_url()}/collections/configure'
+    Config.post(url=url, data=req.model_dump_json())
+
+
 def list_collections() -> List[str]:
     """
     List all collections in ChatBees.
 
     Returns:
         List[Collection]: A list of collection objects.
     """
```

### Comparing `chatbees_python_client-0.9.5/chatbees/client_models/chat.py` & `chatbees_python_client-1.0.0/chatbees/client_models/chat.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/client_models/collection.py` & `chatbees_python_client-1.0.0/chatbees/client_models/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 from typing import List, Dict, Tuple, Any, Union
 from urllib import request
 
 from pydantic import BaseModel
 
 from chatbees.client_models.chat import Chat
 from chatbees.server_models.doc_api import (
+    CrawlStatus,
     IngestionStatus,
     AnswerReference,
-    SearchReference, CrawlStatus,
+    SearchReference,
 )
 from chatbees.server_models.chat import ConfigureChatRequest, ChatAttributes
 from chatbees.server_models.ingestion_type import (
     IngestionType,
     ConfluenceSpec,
+    GDriveSpec,
+    NotionSpec,
 )
 from chatbees.server_models.doc_api import (
     AddDocRequest,
     DeleteDocRequest,
     ListDocsRequest,
     ListDocsResponse,
     SummaryRequest,
@@ -217,22 +220,24 @@
         resp = Config.post(url=url, data=req.model_dump_json())
         crawl_resp = CreateCrawlResponse.model_validate(resp.json())
         return crawl_resp.crawl_id
 
     def create_ingestion(
         self,
         ingestion_type: IngestionType,
-        ingestion_spec: Union[ConfluenceSpec]
+        ingestion_spec: Union[ConfluenceSpec, GDriveSpec, NotionSpec]
     ) -> str:
         """
         Create an Ingestion task
 
         :param ingestion_type: the ingestion type
         :param ingestion_spec: the spec for the ingestion. Currently, supports
             - ConfluenceSpec
+            - GDriveSpec
+            - NotionSpec
         :return: the id of the ingestion
         """
         url = f'{Config.get_base_url()}/docs/create_ingestion'
         req = CreateIngestionRequest(
             namespace_name=Config.namespace,
             collection_name=self.name,
             type=ingestion_type,
```

### Comparing `chatbees_python_client-0.9.5/chatbees/server_models/chat.py` & `chatbees_python_client-1.0.0/chatbees/server_models/chat.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/server_models/collection_api.py` & `chatbees_python_client-1.0.0/chatbees/server_models/collection_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 class CreateCollectionRequest(CollectionBaseRequest):
     description: Optional[str] = None
 
     # If true, create a collection that can be read without an API key
     public_read: Optional[bool] = None
 
 
+class ConfigureCollectionRequest(CollectionBaseRequest):
+    description: Optional[str] = None
+    # whether the collection is publicly readable
+    public_read: Optional[bool] = None
+
+
 class DeleteCollectionRequest(CollectionBaseRequest):
     pass
 
 
 class ListCollectionsRequest(BaseModel):
     namespace_name: str
```

### Comparing `chatbees_python_client-0.9.5/chatbees/server_models/doc_api.py` & `chatbees_python_client-1.0.0/chatbees/server_models/doc_api.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/server_models/ingestion_api.py` & `chatbees_python_client-1.0.0/chatbees/server_models/ingestion_api.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/tests/api_surface_test.py` & `chatbees_python_client-1.0.0/chatbees/tests/api_surface_test.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/tests/smoke_test.py` & `chatbees_python_client-1.0.0/chatbees/tests/smoke_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,24 @@
         col = self.create_collection(public_read=True)
         col.upload_document(f'{os.path.dirname(os.path.abspath(__file__))}/data/text_file.txt')
 
         # Clear API key and ask questions again
         cdb.init(api_key=None)
         col.ask('should not fail')
 
+        cdb.init(owner)
+        cdb.configure_collection(collection_name=col.name, public_read=False)
+        cdb.init(api_key=None)
+        self.assertRaises(cdb.UnAuthorized, col.ask, 'should fail')
+
+        cdb.init(owner)
+        cdb.configure_collection(collection_name=col.name, public_read=True)
+        cdb.init(api_key=None)
+        col.ask('should not fail')
+
     def test_doc_apis(self):
         owner = self.apikey1
         cdb.init(owner)
         col = self.create_collection()
 
         files = [
             f'{os.path.dirname(os.path.abspath(__file__))}/data/text_file.txt',
@@ -223,8 +233,8 @@
                 col, IngestionType.SLACK, SlackSpec(token=slack_token))
             self._synchronous_ingest(
                 col, IngestionType.NOTION, NotionSpec(token=notion_token))
 
         finally:
             cdb.delete_collection(col.name)
 
-    """
+    """
```

### Comparing `chatbees_python_client-0.9.5/chatbees/utils/ask.py` & `chatbees_python_client-1.0.0/chatbees/utils/ask.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/utils/config.py` & `chatbees_python_client-1.0.0/chatbees/utils/config.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/utils/exceptions.py` & `chatbees_python_client-1.0.0/chatbees/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/chatbees/utils/file_upload.py` & `chatbees_python_client-1.0.0/chatbees/utils/file_upload.py`

 * *Files identical despite different names*

### Comparing `chatbees_python_client-0.9.5/PKG-INFO` & `chatbees_python_client-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatbees-python-client
-Version: 0.9.5
+Version: 1.0.0
 Summary: Python client for ChatBees
 Author: ChatBees
 Author-email: build@chatbees.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

