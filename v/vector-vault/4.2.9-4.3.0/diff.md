# Comparing `tmp/vector_vault-4.2.9.tar.gz` & `tmp/vector_vault-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.2.9.tar", last modified: Thu Apr  4 05:25:08 2024, max compression
+gzip compressed data, was "vector_vault-4.3.0.tar", last modified: Thu Apr  4 05:44:12 2024, max compression
```

## Comparing `vector_vault-4.2.9.tar` & `vector_vault-4.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:25:08.258731 vector_vault-4.2.9/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.9/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 05:25:08.258584 vector_vault-4.2.9/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.9/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-04 05:25:08.258768 vector_vault-4.2.9/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-04 05:24:21.000000 vector_vault-4.2.9/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:25:08.256669 vector_vault-4.2.9/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:25:08.258391 vector_vault-4.2.9/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.9/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.9/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.9/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6003 2024-04-04 04:44:48.000000 vector_vault-4.2.9/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.9/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.9/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-04 04:44:31.000000 vector_vault-4.2.9/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-04 05:06:14.000000 vector_vault-4.2.9/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62710 2024-04-04 05:24:12.000000 vector_vault-4.2.9/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.2.9/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.9/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:44:12.432390 vector_vault-4.3.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 05:44:12.432245 vector_vault-4.3.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-04 05:44:12.432427 vector_vault-4.3.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-04 05:43:29.000000 vector_vault-4.3.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:44:12.428995 vector_vault-4.3.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 05:44:12.000000 vector_vault-4.3.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-04 05:44:12.000000 vector_vault-4.3.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-04 05:44:12.000000 vector_vault-4.3.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-04 05:44:12.000000 vector_vault-4.3.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-04 05:44:12.000000 vector_vault-4.3.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:44:12.431963 vector_vault-4.3.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.3.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.0/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6031 2024-04-04 05:44:05.000000 vector_vault-4.3.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-04 05:43:54.000000 vector_vault-4.3.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-04 05:43:50.000000 vector_vault-4.3.0/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62467 2024-04-04 05:43:46.000000 vector_vault-4.3.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.0/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.0/vectorvault/wrap.py
```

### Comparing `vector_vault-4.2.9/LICENSE` & `vector_vault-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.9/PKG-INFO` & `vector_vault-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.2.9
+Version: 4.3.0
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.9/README.md` & `vector_vault-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.9/setup.py` & `vector_vault-4.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.2.9",
+    version="4.3.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.2.9/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.3.0/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.2.9
+Version: 4.3.0
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.9/vectorvault/ai.py` & `vector_vault-4.3.0/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.9/vectorvault/cloud_api.py` & `vector_vault-4.3.0/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.9/vectorvault/cloudmanager.py` & `vector_vault-4.3.0/vectorvault/cloudmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # is strictly forbidden unless prior written permission is obtained
 # from Vector Vault. See license for consent.
 
 from google.cloud import storage
 from .creds import CustomCredentials
 from .vecreq import call_proj, call_update
 from .itemize import cloud_name
-from .vault import ThreadPoolExecutor, as_completed, time, json, os, tempfile, time
+from .vault import ThreadPoolExecutor, T, as_completed, time, json, os, tempfile, time
 
 class CloudManager:
     def __init__(self, user: str, api_key: str, vault: str, ai_api: str = None):
         self.user = user
         self.api = api_key
         self.vault = vault
         self.ai_api = ai_api
@@ -96,15 +96,15 @@
         temp_file_path = self.download_to_temp_file(f'{self.username}.json')
         with open(temp_file_path, 'r') as json_file:
             _map = json.load(json_file)
         os.remove(temp_file_path)
         return _map
     
     def update(self):
-        call_update(self.user, self.vault, self.api)
+        T(target=call_update, args=(self.user, self.vault, self.api)).start()
     
     def build_update(self):
         _map = self.get_mapping()
         for i in range(len(_map)):
             if _map[i]['vault'] == self.vault:
                 _map[i]['last_use'] = time.time()
                 try:
```

### Comparing `vector_vault-4.2.9/vectorvault/creds.py` & `vector_vault-4.3.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.9/vectorvault/download.py` & `vector_vault-4.3.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.9/vectorvault/itemize.py` & `vector_vault-4.3.0/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.9/vectorvault/tools_gpt.py` & `vector_vault-4.3.0/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.9/vectorvault/vault.py` & `vector_vault-4.3.0/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,22 @@
         '''
         self.user = user.lower()
         self.vault = vault.strip() if vault else 'home'
         self.api = api_key
         if openai_key:
             self.openai_key = openai_key
             openai.api_key = self.openai_key
-        t = T(target=self.connect_to_cloud)
-        t.start()
+        try:
+            self.cloud_manager = CloudManager(self.user, self.api, self.vault, self.openai_key)
+            print(f'Connected vault: {self.vault}') if self.verbose else 0 
+        except Exception as e:
+            print('API KEY NOT FOUND or no internet connection!', e)
+            # user can still use the get_chat() function without an api key
+            self.cloud_manager = None
+
         self.embeddings_model = embeddings_model if embeddings_model else 'text-embedding-3-small'
         self.dims = 1536 if embeddings_model != 'text-embedding-3-large' else 3072
         self.vectors = get_vectors(self.dims)
         self.verbose = verbose
         self.x = 0
         self.x_checked = False
         self.vecs_loaded = False
@@ -91,27 +97,14 @@
         self.items = []
         self.last_time = None
         self.saved_already = False
         self.ai_loaded = False
         self.tools = ToolsGPT(verbose=verbose)
         self.rate_limiter = RateLimiter(max_attempts=30)
         self.cuid = conversation_user_id
-        t.join()
-
-
-    def connect_to_cloud(self):
-        try:
-            self.cloud_manager = CloudManager(self.user, self.api, self.vault, self.openai_key)
-            print(f'Connected vault: {self.vault}') if self.verbose else 0 
-                
-        except Exception as e:
-            print('API KEY NOT FOUND or no internet connection!', e)
-            # user can still use the get_chat() function without an api key
-            self.cloud_manager = None
-
 
     def get_vaults(self, vault: str = None):
         '''
             Returns a list of vaults within the current vault directory 
         '''
         vault = self.vault if vault is None else vault
         if self.cloud_manager is None:
@@ -388,16 +381,14 @@
         self.cloud_manager.upload_to_cloud(cloud_name(self.vault, self.map[str(item_id)], self.user, self.api, meta=True), json.dumps(metadata))
         print(f'Item {item_id} metadata saved') if self.verbose else 0
 
 
     def check_index(self):
         if not self.x_checked:
             start_time = time.time()
-            while self.cloud_manager is None:
-                time.sleep(.01)
             if self.cloud_manager.vault_exists(name_vecs(self.vault, self.user, self.api)):
                 if not self.vecs_loaded:
                     self.load_vectors()
                 self.reload_vectors()
             
             self.x_checked = True
             print("initialize index --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
@@ -1011,15 +1002,15 @@
                     print(traceback.format_exc())
                     print(f"API Error: {e}. Backing off for {self.rate_limiter.current_delay} seconds.")
                     self.rate_limiter.on_failure()
                     if attempts >= self.rate_limiter.max_attempts:
                         print(f"API Failed too many times, exiting loop: {e}.")
                         break
 
-        self.update_conversation_history(self.cuid, response) if self.cuid else None
+        self.update_conversation_history(self.cuid, response, user=False) if self.cuid else None
         print("get chat time --- %s seconds ---" % (time.time() - start_time)) if self.verbose else 0
             
         return {'response': response, 'context': context} if return_context else response
         
 
     def get_chat_stream(self, text: str = None, history: str = '', summary: bool = False, get_context: bool = False,
                         n_context: int = 4, return_context: bool = False, history_search: bool = False, smart_history_search: bool = False, 
@@ -1131,15 +1122,15 @@
                                     yield word
                                 yield ' '
 
                             self.rate_limiter.on_success()
                         except Exception as e:
                             raise e
                         if counter == len(inputs):
-                            self.update_conversation_history(self.cuid, full_response) if self.cuid else None
+                            self.update_conversation_history(self.cuid, full_response, user=False) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
                     
                     elif text and get_context and not summary:
                         if smart_history_search:
                             custom_entry = f"Using the current message, with the message history, what is the user is focused on. \nCurrent message: {text}. \n\nPrevious messages: {history}."
                             search_input = self.ai.llm(custom_prompt=custom_entry, model=model, temperature=temperature, timeout=timeout)
@@ -1169,31 +1160,31 @@
                                         if metatag_suffixes:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}']) + str(metatag_suffixes[i])
                                         else:
                                             for i in range(len(metatag)):
                                                 yield str(metatag_prefixes[i]) + str(item['metadata'][f'{metatag[i]}'])
                                 yield item['data']
-                            self.update_conversation_history(self.cuid, full_response) if self.cuid else None
+                            self.update_conversation_history(self.cuid, full_response, user=False) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
                         else:
-                            self.update_conversation_history(self.cuid, full_response) if self.cuid else None
+                            self.update_conversation_history(self.cuid, full_response, user=False) if self.cuid else None
                             yield '!END'
                             self.rate_limiter.on_success()
 
                     else:
                         try:
                             for word in self.ai.llm_stream(segment, history, model=model, custom_prompt=custom_prompt, temperature=temperature):
                                 full_response += word
                                 yield word
                             self.rate_limiter.on_success()
                         except Exception as e:
                             raise e
-                        self.update_conversation_history(self.cuid, full_response) if self.cuid else None
+                        self.update_conversation_history(self.cuid, full_response, user=False) if self.cuid else None
                         yield '!END'
 
                     self.rate_limiter.on_success()
                     break
                 except Exception as e:
                     exceptions += 1
                     print(f"API Error: {e}. Applying backoff.")
@@ -1279,15 +1270,15 @@
             metadata_list = []
         message_id = f"{time.time():.0f}"  # Current time
         metadata_list.append({ 'M': message_id, 'L': len(message) })
         t1 = T(target=self.cloud_manager.upload_to_cloud, args=(f'user_history/{conversation_id}/{message_id}', message))
         t2 = T(target=self.cloud_manager.upload_to_cloud, args=(f'user_history/{conversation_id}/metadata', json.dumps(metadata_list)))
         t1.start()
         t2.start()
-        T(target=call_cloud_save, args=(self.user, self.api, self.openai_key, f'user_history/{conversation_id}/vectors', self.embeddings_model, message, None, message_id, None, None, 3000)).start()
+        self.add_n_save(message, vault = f'user_history/{conversation_id}/vectors', name = message_id)
         t1.join()
         t2.join()
 
     def get_conversation_history(self, conversation_id, message):
         def download_conversation_metadata():
             try:
                 return json.loads(self.cloud_manager.download_text_from_cloud(f'user_history/{conversation_id}/metadata'))
```

### Comparing `vector_vault-4.2.9/vectorvault/vecreq.py` & `vector_vault-4.3.0/vectorvault/vecreq.py`

 * *Files identical despite different names*

