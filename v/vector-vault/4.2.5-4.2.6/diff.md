# Comparing `tmp/vector_vault-4.2.5.tar.gz` & `tmp/vector_vault-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.2.5.tar", last modified: Wed Apr  3 01:10:10 2024, max compression
+gzip compressed data, was "vector_vault-4.2.6.tar", last modified: Thu Apr  4 04:46:02 2024, max compression
```

## Comparing `vector_vault-4.2.5.tar` & `vector_vault-4.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-03 01:10:10.142808 vector_vault-4.2.5/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.5/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-03 01:10:10.142535 vector_vault-4.2.5/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.5/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-03 01:10:10.142886 vector_vault-4.2.5/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-03 01:09:08.000000 vector_vault-4.2.5/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-03 01:10:10.140926 vector_vault-4.2.5/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-03 01:10:10.000000 vector_vault-4.2.5/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-03 01:10:10.142381 vector_vault-4.2.5/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.5/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.5/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.5/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6326 2024-03-13 21:53:47.000000 vector_vault-4.2.5/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.5/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.5/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2984 2024-03-08 18:43:23.000000 vector_vault-4.2.5/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-01 23:51:29.000000 vector_vault-4.2.5/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    57181 2024-04-03 01:08:55.000000 vector_vault-4.2.5/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     4525 2024-01-03 00:13:43.000000 vector_vault-4.2.5/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.5/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 04:46:02.261484 vector_vault-4.2.6/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.6/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 04:46:02.261290 vector_vault-4.2.6/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.6/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-04 04:46:02.261526 vector_vault-4.2.6/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-04 04:45:01.000000 vector_vault-4.2.6/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 04:46:02.257935 vector_vault-4.2.6/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 04:46:02.000000 vector_vault-4.2.6/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-04 04:46:02.000000 vector_vault-4.2.6/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-04 04:46:02.000000 vector_vault-4.2.6/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-04 04:46:02.000000 vector_vault-4.2.6/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-04 04:46:02.000000 vector_vault-4.2.6/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 04:46:02.260946 vector_vault-4.2.6/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.6/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.6/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.6/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6003 2024-04-04 04:44:48.000000 vector_vault-4.2.6/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.6/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.6/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-04 04:44:31.000000 vector_vault-4.2.6/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20813 2024-04-03 19:52:04.000000 vector_vault-4.2.6/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62683 2024-04-04 04:44:24.000000 vector_vault-4.2.6/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.2.6/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.6/vectorvault/wrap.py
```

### Comparing `vector_vault-4.2.5/LICENSE` & `vector_vault-4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.5/PKG-INFO` & `vector_vault-4.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.2.5
+Version: 4.2.6
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.5/README.md` & `vector_vault-4.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.5/setup.py` & `vector_vault-4.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.2.5",
+    version="4.2.6",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.2.5/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.2.6/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.2.5
+Version: 4.2.6
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.5/vectorvault/ai.py` & `vector_vault-4.2.6/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.5/vectorvault/cloud_api.py` & `vector_vault-4.2.6/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.5/vectorvault/cloudmanager.py` & `vector_vault-4.2.6/vectorvault/cloudmanager.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault. See license for consent.
 
 from google.cloud import storage
 from .creds import CustomCredentials
 from .vecreq import call_proj, call_update
 from .itemize import cloud_name
-from .vault import ThreadPoolExecutor, as_completed, T as t, time, json, os, tempfile
+from .vault import ThreadPoolExecutor, as_completed, time, json, os, tempfile, time
 
 class CloudManager:
-    def __init__(self, user: str, api_key: str, vault: str):
+    def __init__(self, user: str, api_key: str, vault: str, ai_api: str = None):
         self.user = user
         self.api = api_key
         self.vault = vault
+        self.ai_api = ai_api
         # Create credentials
         self.credentials = CustomCredentials(user, self.api)
         # Instantiate the client 
         self.storage_client = storage.Client(project=call_proj(), credentials=self.credentials)
         self.username = self.username(self.user)
         self.cloud = self.storage_client.bucket(self.username)
         self.cloud_name = cloud_name
@@ -80,40 +81,30 @@
             blob = self.cloud.blob(vault_name)
             blob.download_to_filename(temp_file_path)
         finally:
             # Close the file descriptor
             os.close(temp_file_descriptor)
         return temp_file_path
     
-    def upload(self, item, text, meta):
-        self.upload_to_cloud(self.cloud_name(self.vault, item, self.user, self.api, item=True), text)
-        self.upload_to_cloud(self.cloud_name(self.vault, item, self.user, self.api, meta=True), json.dumps(meta))
-    
-    def upload_personality_message(self, personality_message):
-        self.upload_to_cloud(f'{self.vault}/personality_message', personality_message)
-    
-    def upload_custom_prompt(self, prompt):
-        self.upload_to_cloud(f'{self.vault}/prompt', prompt)
-
-    def upload_no_context_prompt(self, prompt):
-        self.upload_to_cloud(f'{self.vault}/no_context_prompt', prompt)
-     
+    def upload(self, item, text, meta, vault = None):
+        self.upload_to_cloud(self.cloud_name(vault if vault else self.vault, item, self.user, self.api, item=True), text)
+        self.upload_to_cloud(self.cloud_name(vault if vault else self.vault, item, self.user, self.api, meta=True), json.dumps(meta))
+        
     def username(self, input_string):
         return input_string.replace("@", "_at_").replace(".", "_dot_") + '_vvclient'
 
     def get_mapping(self):
         temp_file_path = self.download_to_temp_file(f'{self.username}.json')
         with open(temp_file_path, 'r') as json_file:
             _map = json.load(json_file)
         os.remove(temp_file_path)
         return _map
     
     def update(self):
-        th = t(target=call_update, args=(self.user, self.vault, self.api))
-        th.start()
+        call_update(self.user, self.vault, self.api)
     
     def build_update(self):
         _map = self.get_mapping()
         for i in range(len(_map)):
             if _map[i]['vault'] == self.vault:
                 _map[i]['last_use'] = time.time()
                 try:
```

### Comparing `vector_vault-4.2.5/vectorvault/creds.py` & `vector_vault-4.2.6/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.5/vectorvault/download.py` & `vector_vault-4.2.6/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.5/vectorvault/itemize.py` & `vector_vault-4.2.6/vectorvault/itemize.py`

 * *Files 20% similar despite different names*

```diff
@@ -87,8 +87,32 @@
         }
     else:
         result = {
             "data": item_data,
             "metadata": meta,
             "distance": distance
         }
-    return result
+    return result
+
+def get_time_statement(now, message_time):
+    diff = now - message_time
+    days, seconds = diff.days, diff.seconds
+    human_readable_time = ""
+
+    if days >= 365:
+        years = days // 365
+        human_readable_time = f"{years} {'year' if years == 1 else 'years'} ago: "
+    elif days >= 30:
+        months = days // 30
+        human_readable_time = f"{months} {'month' if months == 1 else 'months'} ago: "
+    elif days >= 1:
+        human_readable_time = f"{days} {'day' if days == 1 else 'days'} ago: "
+    elif seconds >= 3600:
+        hours = seconds // 3600
+        human_readable_time = f"{hours} {'hour' if hours == 1 else 'hours'} ago: "
+    elif seconds >= 60:
+        minutes = seconds // 60
+        human_readable_time = f"{minutes} {'minute' if minutes == 1 else 'minutes'} ago: "
+    else:
+        human_readable_time = "just now: "
+
+    return human_readable_time
```

### Comparing `vector_vault-4.2.5/vectorvault/tools_gpt.py` & `vector_vault-4.2.6/vectorvault/tools_gpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .ai import AI
+from ai import AI
 import time
 import ast
 
 '''
     ToolsGPT is a set of tools special to large language models. 
     Every tool turns unstructured data into structured data.
```

### Comparing `vector_vault-4.2.5/vectorvault/vault.py` & `vector_vault-4.2.6/vectorvault/vault.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,27 +19,27 @@
 import os
 import time
 import uuid
 import re
 import json
 import traceback
 import random
-from datetime import datetime
 from typing import List
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from ai import AI, openai
 from threading import Thread as T
+from datetime import datetime, timedelta
+from .concurrent.futures import ThreadPoolExecutor, as_completed
 from .cloudmanager import CloudManager
-from .ai import AI, openai
-from .itemize import itemize, name_vecs, get_item, get_vectors, build_return, cloud_name, name_map
-from .vecreq import call_get_similar
+from .itemize import itemize, name_vecs, get_item, get_vectors, build_return, cloud_name, name_map, get_time_statement
+from .vecreq import call_get_similar, call_cloud_save
 from .tools_gpt import ToolsGPT
 
 
 class Vault:
-    def __init__(self, user: str = None, api_key: str = None, vault: str = None, openai_key: str = None, embeddings_model: str = None, verbose: bool = False):
+    def __init__(self, user: str = None, api_key: str = None, openai_key: str = None, vault: str = None, embeddings_model: str = None, verbose: bool = False, conversation_user_id: str = None):
         ''' 
         ### Create a vector database instance like this:
         ```
         vault = Vault(user='YOUR_EMAIL',
               api_key='VECTOR_VAULT_API_KEY',
               openai_key='OPENAI_API_KEY',
               vault='VAULT_NAME',
@@ -71,39 +71,40 @@
               personality_message='Answer like you are Snoop Dogg',
               verbose=False)
         ```
         '''
         self.user = user.lower()
         self.vault = vault.strip() if vault else 'home'
         self.api = api_key
-        t = T(target=self.connect_to_cloud)
-        t.start()
         if openai_key:
             self.openai_key = openai_key
             openai.api_key = self.openai_key
+        t = T(target=self.connect_to_cloud)
+        t.start()
         self.embeddings_model = embeddings_model if embeddings_model else 'text-embedding-3-small'
         self.dims = 1536 if embeddings_model != 'text-embedding-3-large' else 3072
         self.vectors = get_vectors(self.dims)
         self.verbose = verbose
         self.x = 0
         self.x_checked = False
         self.vecs_loaded = False
         self.map = {}
         self.items = []
         self.last_time = None
         self.saved_already = False
         self.ai_loaded = False
         self.tools = ToolsGPT(verbose=verbose)
         self.rate_limiter = RateLimiter(max_attempts=30)
+        self.cuid = conversation_user_id
         t.join()
 
 
     def connect_to_cloud(self):
         try:
-            self.cloud_manager = CloudManager(self.user, self.api, self.vault)
+            self.cloud_manager = CloudManager(self.user, self.api, self.vault, self.openai_key)
             print(f'Connected vault: {self.vault}') if self.verbose else 0 
                 
         except Exception as e:
             print('API KEY NOT FOUND or no internet connection!', e)
             # user can still use the get_chat() function without an api key
             self.cloud_manager = None
 
@@ -216,15 +217,15 @@
             else: # only when called externally in some situations
                 self.load_ai()
                 prompt = self.ai.main_prompt_with_context if context else self.ai.prompt
             
         return prompt
 
 
-    def save(self, trees: int = 10):
+    def save(self, trees: int = 10, vault = None):
         '''
             Saves all the data added locally to the Cloud. All Vault references are Cloud references.
             To add data to your Vault and access it later, you must first call add(), then get_vectors(), and finally save().
         '''
         if self.saved_already:
             self.clear_cache()
             print("The last save was aborted before the build process finished. Clearing cache to start again...")
@@ -233,18 +234,18 @@
         self.vectors.build(trees)
 
         total_saved_items = 0
 
         with ThreadPoolExecutor() as executor:
             for item in self.items:
                 item_text, item_id, item_meta = get_item(item)
-                executor.submit(self.cloud_manager.upload, self.map.get(str(item_id)), item_text, item_meta)
+                executor.submit(self.cloud_manager.upload, self.map.get(str(item_id)), item_text, item_meta, vault = vault if vault else self.vault)
                 total_saved_items += 1
 
-        self.upload_vectors()
+        self.upload_vectors(vault if vault else self.vault)
         print(f"upload time --- {(time.time() - start_time)} seconds --- {total_saved_items} items saved") if self.verbose else 0
             
 
     def clear_cache(self):
         '''
             Clears the cache for all the loaded items 
         '''
@@ -387,44 +388,48 @@
         self.cloud_manager.upload_to_cloud(cloud_name(self.vault, self.map[str(item_id)], self.user, self.api, meta=True), json.dumps(metadata))
         print(f'Item {item_id} metadata saved') if self.verbose else 0
 
 
     def check_index(self):
         if not self.x_checked:
             start_time = time.time()
+            while self.cloud_manager is None:
+                time.sleep(.01)
             if self.cloud_manager.vault_exists(name_vecs(self.vault, self.user, self.api)):
                 if not self.vecs_loaded:
                     self.load_vectors()
                 self.reload_vectors()
             
             self.x_checked = True
             print("initialize index --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
                 
 
-    def load_mapping(self):
+    def load_mapping(self, vault = None):
         '''Internal function only'''
+        vault = vault if vault else self.vault 
         try: # try to get the map
-            temp_file_path = self.cloud_manager.download_to_temp_file(name_map(self.vault, self.user, self.api))
+            temp_file_path = self.cloud_manager.download_to_temp_file(name_map(vault, self.user, self.api))
             with open(temp_file_path, 'r') as json_file:
                 self.map = json.load(json_file)
             os.remove(temp_file_path)
         except: # it doesn't exist
-            if self.cloud_manager.vault_exists(name_vecs(self.vault, self.user, self.api)): # but if the vault does
+            if self.cloud_manager.vault_exists(name_vecs(vault, self.user, self.api)): # but if the vault does
                 self.map = {str(i): str(i) for i in range(self.vectors.get_n_items())}
 
     def add_to_map(self):
         self.map[str(self.x)] = str(uuid.uuid4())
         self.x +=1
     
 
-    def load_vectors(self):
+    def load_vectors(self, vault = None):
         start_time = time.time()
+        vault = vault if vault else self.vault 
         t = T(target=self.load_mapping())
         t.start()
-        temp_file_path = self.cloud_manager.download_to_temp_file(name_vecs(self.vault, self.user, self.api))
+        temp_file_path = self.cloud_manager.download_to_temp_file(name_vecs(vault, self.user, self.api))
         self.vectors.load(temp_file_path)
         os.remove(temp_file_path)
         t.join()
         self.vecs_loaded = True
         print("get load vectors --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
 
 
@@ -533,27 +538,28 @@
             count += 1
             vector = self.vectors.get_item_vector(i)
             new_index.add_item(i, vector)
         self.x = count + 1
         self.vectors = new_index
 
 
-    def upload_vectors(self):
+    def upload_vectors(self, vault = None):
+        vault = vault if vault else self.vault
         with tempfile.NamedTemporaryFile(delete=False) as temp_file:
             vector_temp_file_path = temp_file.name
             self.vectors.save(vector_temp_file_path)
             byte = os.path.getsize(vector_temp_file_path)
-            self.cloud_manager.upload_temp_file(vector_temp_file_path, name_vecs(self.vault, self.user, self.api, byte))
+            self.cloud_manager.upload_temp_file(vector_temp_file_path, name_vecs(vault, self.user, self.api, byte))
         
         map_temp_file_path = None
         with tempfile.NamedTemporaryFile(mode='w', delete=False) as temp_file:
             map_temp_file_path = temp_file.name
             json.dump(self.map, temp_file, indent=2)
         
-        self.cloud_manager.upload_temp_file(map_temp_file_path, name_map(self.vault, self.user, self.api, byte))
+        self.cloud_manager.upload_temp_file(map_temp_file_path, name_map(vault, self.user, self.api, byte))
         if os.path.exists(map_temp_file_path):
             os.remove(map_temp_file_path)
             
         self.items.clear()
         self.vectors = get_vectors(self.dims)
         self.x_checked = False
         self.vecs_loaded = False
@@ -660,29 +666,30 @@
                 results[index] = result  # Insert each result at its corresponding index
             
         print(f"Retrieved {len(ids)} items --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
         
         return results
 
 
-    def get_items_by_vector(self, vector: list, n: int = 4, include_distances: bool = False):
+    def get_items_by_vector(self, vector: list, n: int = 4, include_distances: bool = False, vault = None) -> list:
         '''
             Internal function that returns vector similar items. Requires input vector, returns similar items
         '''
         try:
-            self.load_vectors()
+            vault = vault if vault else self.vault 
+            self.load_vectors(vault)
             start_time = time.time()
             if not include_distances:
                 vecs = self.vectors.get_nns_by_vector(vector, n)
                 results = [None] * len(vecs)  # Pre-fill the results list with placeholders
 
                 def fetch_item(index, vec):
                     # Function to fetch a single item, to be run in parallel
-                    item_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, self.map[str(vec)], self.user, self.api, item=True))
-                    meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, self.map[str(vec)], self.user, self.api, meta=True))
+                    item_data = self.cloud_manager.download_text_from_cloud(cloud_name(vault, self.map[str(vec)], self.user, self.api, item=True))
+                    meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(vault, self.map[str(vec)], self.user, self.api, meta=True))
                     meta = json.loads(meta_data)
                     return index, build_return(item_data, meta)
                 
                 with ThreadPoolExecutor() as executor:
                     futures = [executor.submit(fetch_item, i, vec) for i, vec in enumerate(vecs)]
                     for future in as_completed(futures):
                         index, result = future.result()
@@ -693,16 +700,16 @@
                 return results
             else:
                 vecs, distances = self.vectors.get_nns_by_vector(vector, n, include_distances=include_distances)
                 results = [None] * len(vecs)  # Pre-fill the results list with placeholders
 
                 def fetch_item(index, vec, distance):
                     # Function to fetch a single item, to be run in parallel
-                    item_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, self.map[str(vec)], self.user, self.api, item=True))
-                    meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(self.vault, self.map[str(vec)], self.user, self.api, meta=True))
+                    item_data = self.cloud_manager.download_text_from_cloud(cloud_name(vault, self.map[str(vec)], self.user, self.api, item=True))
+                    meta_data = self.cloud_manager.download_text_from_cloud(cloud_name(vault, self.map[str(vec)], self.user, self.api, meta=True))
                     meta = json.loads(meta_data)
                     return index, build_return(item_data, meta, distance)
 
                 with ThreadPoolExecutor() as executor:
                     futures = [executor.submit(fetch_item, i, vec, distances[i]) for i, vec in enumerate(vecs)]
                     for future in as_completed(futures):
                         index, result = future.result()
@@ -711,72 +718,73 @@
                 print(f"get {n} items back --- %s seconds ---" % (time.time() - start_time))if self.verbose else 0
                    
                 return results
         except:
             return [{'data': 'No data has been added', 'metadata': {'no meta': 'No metadata has been added'}}]
 
 
-    def get_similar_local(self, text: str, n: int = 4, include_distances: bool = False):
+    def get_similar_local(self, text: str, n: int = 4, include_distances: bool = False, vault = None):
         '''
             Returns similar items from the Vault as the one you entered, but locally
             (saves a few milliseconds and is sometimes used on production builds)
         '''
         self.cloud_manager.update()
         vector = self.process_batch([text], never_stop=False, loop_timeout=180)[0]
-        return self.get_items_by_vector(vector, n, include_distances=include_distances)
+        return self.get_items_by_vector(vector, n, include_distances = include_distances, vault = vault if vault else self.vault)
     
 
-    def get_similar(self, text: str, n: int = 4, include_distances: bool = False):
+    def get_similar(self, text: str, n: int = 4, include_distances: bool = False, vault = None):
         '''
             Returns similar items from the Vault as the text you enter.
 
             Param `include_distances = True` adds the "distance" field to the return.
             The distance can be useful for assessing similarity differences in the items returned. 
             Each item has its' own distance number, and this changes the structure of the output.
         '''
-        return call_get_similar(self.user, self.vault, self.api, self.openai_key, text, n, include_distances=include_distances, verbose=self.verbose)
+        return call_get_similar(self.user, vault if vault else self.vault, self.api, self.openai_key, text, n, include_distances=include_distances, verbose=self.verbose)
 
 
-    def add_item(self, text: str, meta: dict = None, name: str = None):
+    def add_item(self, text: str, meta: dict = None, name: str = None, vault = None):
         """
             If your text length is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
         self.check_index()
-        new_item = itemize(self.vault, self.x, meta, text, name)
+        new_item = itemize(vault if vault else self.vault, self.x, meta, text, name)
         self.items.append(new_item)
         self.add_to_map()
 
 
-    def add(self, text: str, meta: dict = None, name: str = None, split: bool = False, split_size: int = 1000, max_threshold: int = 16000):
+    def add(self, text: str, meta: dict = None, name: str = None, split: bool = False, split_size: int = 1000, max_threshold: int = 16000, vault = None):
         """
             If your text length is greater than 4000 tokens, Vault.split_text(your_text)  
             will automatically be added
         """
         self.check_index()
 
         if len(text) > 15000 or split:
             print('Using the built-in "split_text()" function to get a list of texts') if self.verbose else 0 
                 
             texts = self.split_text(text, min_threshold=split_size, max_threshold=max_threshold) # returns list of text segments
         else:
             texts = [text]
         for text in texts:
-            self.add_item(text, meta, name)
+            self.add_item(text, meta, name, vault if vault else self.vault)
 
 
-    def add_n_save(self, text: str, meta: dict = None, name: str = None, split: bool = False, split_size: int = 1000, max_threshold: int = 16000):
+    def add_n_save(self, text: str, meta: dict = None, name: str = None, split: bool = False, split_size: int = 1000, max_threshold: int = 16000, vault = None):
         """
             Adds data, gets vectors, then saves the data to the cloud in one call
             If your text length is greater than 4000 tokens, your text will automatically be split by
             Vault.split_text(your_text).
         """
-        self.add(text=text, meta=meta, name=name, split=split, split_size=split_size, max_threshold=max_threshold)
+        self.add(text=text, meta=meta, name=name, split=split, split_size=split_size, max_threshold=max_threshold, vault=vault if vault else self.vault)
         self.get_vectors()
-        self.save()
+        self.save(vault = vault if vault else self.vault)
+        T(target=self.clear_cache).start()
 
 
     def add_item_with_vector(self, text: str, vector: list, meta: dict = None, name: str = None):
         """
             If your text length is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
@@ -849,15 +857,15 @@
                 self.vectors.add_item(item_index, embedding)
                 current_item_index += 1
 
         self.last_time = time.time()
         print("get vectors time --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
             
 
-    def get_chat(self, text: str = None, history: str = None, summary: bool = False, get_context: bool = False, 
+    def get_chat(self, text: str = None, history: str = '', summary: bool = False, get_context: bool = False, 
                  n_context: int = 4, return_context: bool = False, history_search: bool = False, smart_history_search: bool = False, 
                  model: str = 'gpt-3.5-turbo', include_context_meta: bool = False, custom_prompt: bool = False, 
                  local: bool =False, temperature: int = 0, timeout: int = 300):
         '''
             Chat get response from OpenAI's ChatGPT. 
             Models: ChatGPT = "gpt-3.5-turbo" • GPT4 = "gpt-4" 
             Large Context Models: ChatGPT 16k = "gpt-3.5-turbo-16k" • GPT4 32k = "gpt-4-32k"
@@ -934,18 +942,19 @@
             ```
 
         '''
         if not self.ai_loaded:
             self.load_ai()
         model = model.lower()
         start_time = time.time()
-
-        if not history:
-            history = ''
-
+    
+        history_time = time.time() if self.cuid else None
+        history = self.get_conversation_history(self.cuid, text) if self.cuid else history
+        print('history retrieval took:', history_time - time.time()) if self.cuid and self.verbose else None
+        
         if text: 
             inputs = [text]
         else:
             if not custom_prompt:
                 raise ValueError("No input text provided. Please enter text to proceed.")
             else:
                 inputs = [0]
@@ -1002,20 +1011,21 @@
                     print(traceback.format_exc())
                     print(f"API Error: {e}. Backing off for {self.rate_limiter.current_delay} seconds.")
                     self.rate_limiter.on_failure()
                     if attempts >= self.rate_limiter.max_attempts:
                         print(f"API Failed too many times, exiting loop: {e}.")
                         break
 
+        self.update_conversation_history(self.cuid, response) if self.cuid else None
         print("get chat time --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
             
         return {'response': response, 'context': context} if return_context else response
         
 
-    def get_chat_stream(self, text: str = None, history: str = None, summary: bool = False, get_context: bool = False,
+    def get_chat_stream(self, text: str = None, history: str = '', summary: bool = False, get_context: bool = False,
                         n_context: int = 4, return_context: bool = False, history_search: bool = False, smart_history_search: bool = False, 
                         model: str ='gpt-3.5-turbo', include_context_meta: bool = False, metatag: bool = False,
                         metatag_prefixes: bool = False, metatag_suffixes: bool = False, custom_prompt: bool = False, 
                         local: bool = False, temperature: int = 0, timeout: int = 300):
         '''
             Always use this get_chat_stream() wrapped by either print_stream(), or cloud_stream().
             cloud_stream() is for cloud functions, like a flask app serving a front end elsewhere.
@@ -1080,31 +1090,32 @@
             response = vault.print_stream(vault.get_chat_stream(text, chat_history, get_context = True, custom_prompt=my_prompt))
             ```
         '''
         if not self.ai_loaded:
             self.load_ai()
         model = model.lower()
         start_time = time.time()
-
-        if not history:
-            history = ''
+    
+        history_time = time.time()
+        history = self.get_conversation_history(self.cuid, text) if self.cuid else history
+        print('history retrieval took:', history_time - time.time()) if self.cuid and self.verbose else None
 
         if text:
             inputs = [text]
         else:
             if not custom_prompt:
                 raise ValueError("No input text provided. Please enter text to proceed.")
             else:
                 inputs = []
                 
         counter = 0
         for segment in inputs:
             start_time = time.time()
             exceptions = 0
-
+            full_response = ''
             while True:
                 try:
                     if summary and not get_context:
                         try:
                             token_limit = self.ai.model_token_limits.get(model, 4000)
                             total_tokens = self.ai.get_tokens(segment)
 
@@ -1112,21 +1123,23 @@
                                 # Calculate start and end indices for the current chunk
                                 start_index = i * token_limit
                                 end_index = min((i + 1) * token_limit, total_tokens)
                                 # Extract the current chunk from the segment
                                 current_chunk = segment[start_index:end_index]
                                 # Process the current chunk and concatenate the response
                                 for word in self.ai.summarize_stream(current_chunk, model=model, custom_prompt=custom_prompt, temperature=temperature):
+                                    full_response += word
                                     yield word
                                 yield ' '
 
                             self.rate_limiter.on_success()
                         except Exception as e:
                             raise e
                         if counter == len(inputs):
+                            self.update_conversation_history(self.cuid, full_response) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
                     
                     elif text and get_context and not summary:
                         if smart_history_search:
                             custom_entry = f"Using the current message, with the message history, what is the user is focused on. \nCurrent message: {text}. \n\nPrevious messages: {history}."
                             search_input = self.ai.llm(custom_prompt=custom_entry, model=model, temperature=temperature, timeout=timeout)
@@ -1136,14 +1149,15 @@
                         context = self.get_similar(search_input, n=n_context) if not local else self.get_similar_local(search_input, n=n_context)
                         input_ = str(context) if include_context_meta else ''
                         for text in context:
                             input_ += text['data']
 
                         try:
                             for word in self.ai.llm_w_context_stream(segment, input_, history, model=model, custom_prompt=custom_prompt, temperature=temperature):
+                                full_response += word
                                 yield word
                             self.rate_limiter.on_success()
                         except Exception as e:
                             raise e
 
                         if return_context:
                             for item in context:
@@ -1155,28 +1169,33 @@
                                         if metatag_suffixes:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
                                         else:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
                                 yield item['data']
+                            self.update_conversation_history(self.cuid, full_response) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
                         else:
+                            self.update_conversation_history(self.cuid, full_response) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
 
                     else:
                         try:
                             for word in self.ai.llm_stream(segment, history, model=model, custom_prompt=custom_prompt, temperature=temperature):
+                                full_response += word
                                 yield word
                             self.rate_limiter.on_success()
                         except Exception as e:
                             raise e
+                        self.update_conversation_history(self.cuid, full_response) if self.cuid else None
                         yield '!END'
+
                     self.rate_limiter.on_success()
                     break
                 except Exception as e:
                     exceptions += 1
                     print(f"API Error: {e}. Applying backoff.")
                     self.rate_limiter.on_failure()
                     if exceptions >= self.rate_limiter.max_attempts:
@@ -1248,14 +1267,91 @@
         '''
             For cloud application yielding the chat stream, like a flask app
         '''
         for word in function:
             yield f"data: {json.dumps({'data': word})} \n\n"
 
 
+    def update_conversation_history(self, conversation_id, message, metadata_list = None, user = True):
+        message = f'User: {message}' if user else f'AI: {message}'
+        try:
+            metadata_list = metadata_list if metadata_list else json.loads(self.cloud_manager.download_text_from_cloud(f'user_history/{conversation_id}/metadata'))
+        except:
+            metadata_list = []
+        message_id = f"{time.time():.0f}"  # Current time
+        metadata_list.append({ 'M': message_id, 'L': len(message) })
+        t1 = T(target=self.cloud_manager.upload_to_cloud, args=(f'user_history/{conversation_id}/{message_id}', message))
+        t2 = T(target=self.cloud_manager.upload_to_cloud, args=(f'user_history/{conversation_id}/metadata', json.dumps(metadata_list)))
+        t1.start()
+        t2.start()
+        call_cloud_save(self.user, self.api, self.openai_key, f'user_history/{conversation_id}/vectors', self.embeddings_model, message, name=message_id, split_size=3000)
+        t1.join()
+        t2.join()
+
+    def get_conversation_history(self, conversation_id, message):
+        def download_conversation_metadata():
+            try:
+                return json.loads(self.cloud_manager.download_text_from_cloud(f'user_history/{conversation_id}/metadata'))
+            except:
+                return []
+
+        def download_conversation_message(msg_id):
+            try:
+                return self.cloud_manager.download_text_from_cloud(f'user_history/{conversation_id}/{msg_id}')
+            except:
+                return []
+
+        def golden_retriever(metadata_list): 
+            one_hour_ago = datetime.now() - timedelta(hours=1)
+            return [metadata['M'] for metadata in reversed(metadata_list) if datetime.fromtimestamp(float(metadata['M'])) >= one_hour_ago]
+
+        def vector_search_conversation_history(message):
+            return self.get_similar_local(message, vault=f'user_history/{conversation_id}/vectors')
+
+        history = ''
+
+        try:
+            meta = download_conversation_metadata()
+        except:
+            meta = None
+
+        message_ids = golden_retriever(meta) if meta != None else []
+
+        update = T(target=self.update_conversation_history, args=(conversation_id, message, meta if meta else None))
+        update.start()
+
+        print('message_ids:', message_ids) if self.verbose else None
+
+        if message_ids != []:
+            history_lines = []
+            with ThreadPoolExecutor(max_workers=10) as executor:
+                future_to_message_id = {executor.submit(download_conversation_message, message_id): message_id for message_id in message_ids}
+
+                # Iterate over the futures as they complete (preserves order)
+                for future in as_completed(future_to_message_id):
+                    message_content = future.result()
+                    history_lines.append(message_content)
+
+            history = '\n'.join(history_lines)
+            history = "Recent conversation history:" + history
+
+            vector_similar_results = vector_search_conversation_history(message)
+            vector_history = []
+            now = datetime.now()
+            for i in vector_similar_results:
+                message_time = datetime.fromtimestamp(float(i['name']))
+                data = i['data']
+                vector_history.append(f'{get_time_statement(now, message_time)} {data}')                
+
+            history = history + "Vector search conversation history:" + '\n'.join(vector_history)
+
+        update.join()
+        return history
+
+
 class RateLimiter:
     def __init__(self, max_attempts=30):
         self.base_delay = 1  # Base delay of 1 second
         self.max_delay = 60  # Maximum delay of 60 seconds
         self.backoff_factor = 2
         self.current_delay = self.base_delay
         self.max_attempts = max_attempts
@@ -1263,8 +1359,8 @@
     def on_success(self):
         # Reset delay after a successful call
         self.current_delay = self.base_delay
 
     def on_failure(self):
         # Apply exponential backoff with a random jitter
         self.current_delay = min(self.max_delay, random.uniform(self.base_delay, self.current_delay * self.backoff_factor))
-        time.sleep(self.current_delay)
+        time.sleep(self.current_delay)
```

### Comparing `vector_vault-4.2.5/vectorvault/vecreq.py` & `vector_vault-4.2.6/vectorvault/vecreq.py`

 * *Files 13% similar despite different names*

```diff
@@ -109,14 +109,42 @@
     if response.status_code == 200:
         # Parse the response JSON
         data = response.json()
         return data
     else:
         raise Exception(f"Request failed with status {response.status_code}")
 
+def call_cloud_save(user, api_key, openai_key, vault, embeddings_model, text, meta = None, name = None, split = None, split_size = None):
+    url = "https://api.vectorvault.io/add_cloud"
+
+    # Define the data payload
+    data = {
+        'user': user,
+        'vault': vault,
+        'api_key': api_key,
+        'openai_key': openai_key,
+        "text": text,
+        "embeddings_model": embeddings_model,
+        "meta": meta,
+        "name": name,
+        "split": split,
+        "split_size": split_size,
+    }
+
+    # Make the POST request
+    response = requests.post(url, json=data)
+
+    # Check the request was successful
+    if response.status_code == 200:
+        # Parse the response JSON
+        data = response.json()
+        return data
+    else:
+        raise Exception(f"Request failed with status {response.status_code}")
+
 
 def call_get_chat(user, vault, api_key, openai_key, text, history=None, summary=False, get_context=False, n_context=4, return_context=False, expansion=False, history_search=False, model='gpt-3.5-turbo', include_context_meta=False):
     url = "https://api.vectorvault.io/get_chat"
 
     # Define the data payload
     data = {
         'user': user,
```

