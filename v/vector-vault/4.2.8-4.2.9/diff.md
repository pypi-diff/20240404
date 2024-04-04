# Comparing `tmp/vector_vault-4.2.8.tar.gz` & `tmp/vector_vault-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.2.8.tar", last modified: Thu Apr  4 05:06:33 2024, max compression
+gzip compressed data, was "vector_vault-4.2.9.tar", last modified: Thu Apr  4 05:25:08 2024, max compression
```

## Comparing `vector_vault-4.2.8.tar` & `vector_vault-4.2.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:06:33.691971 vector_vault-4.2.8/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.8/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 05:06:33.691812 vector_vault-4.2.8/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.8/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-04 05:06:33.692008 vector_vault-4.2.8/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-04 05:06:22.000000 vector_vault-4.2.8/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:06:33.688017 vector_vault-4.2.8/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 05:06:33.000000 vector_vault-4.2.8/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-04 05:06:33.000000 vector_vault-4.2.8/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-04 05:06:33.000000 vector_vault-4.2.8/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-04 05:06:33.000000 vector_vault-4.2.8/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-04 05:06:33.000000 vector_vault-4.2.8/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:06:33.691447 vector_vault-4.2.8/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.8/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.8/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.8/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6003 2024-04-04 04:44:48.000000 vector_vault-4.2.8/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.8/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.8/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-04 04:44:31.000000 vector_vault-4.2.8/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-04 05:06:14.000000 vector_vault-4.2.8/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62683 2024-04-04 05:04:15.000000 vector_vault-4.2.8/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.2.8/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.8/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:25:08.258731 vector_vault-4.2.9/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.2.9/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 05:25:08.258584 vector_vault-4.2.9/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.2.9/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-04 05:25:08.258768 vector_vault-4.2.9/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-04 05:24:21.000000 vector_vault-4.2.9/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:25:08.256669 vector_vault-4.2.9/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-04 05:25:08.000000 vector_vault-4.2.9/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 05:25:08.258391 vector_vault-4.2.9/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.2.9/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.2.9/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.2.9/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6003 2024-04-04 04:44:48.000000 vector_vault-4.2.9/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.2.9/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.2.9/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-04 04:44:31.000000 vector_vault-4.2.9/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-04 05:06:14.000000 vector_vault-4.2.9/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62710 2024-04-04 05:24:12.000000 vector_vault-4.2.9/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.2.9/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.2.9/vectorvault/wrap.py
```

### Comparing `vector_vault-4.2.8/LICENSE` & `vector_vault-4.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/PKG-INFO` & `vector_vault-4.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.2.8
+Version: 4.2.9
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.8/README.md` & `vector_vault-4.2.9/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/setup.py` & `vector_vault-4.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.2.8",
+    version="4.2.9",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.2.8/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.2.9/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.2.8
+Version: 4.2.9
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.2.8/vectorvault/ai.py` & `vector_vault-4.2.9/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/vectorvault/cloud_api.py` & `vector_vault-4.2.9/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/vectorvault/cloudmanager.py` & `vector_vault-4.2.9/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/vectorvault/creds.py` & `vector_vault-4.2.9/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/vectorvault/download.py` & `vector_vault-4.2.9/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/vectorvault/itemize.py` & `vector_vault-4.2.9/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/vectorvault/tools_gpt.py` & `vector_vault-4.2.9/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.2.8/vectorvault/vault.py` & `vector_vault-4.2.9/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -1279,15 +1279,15 @@
             metadata_list = []
         message_id = f"{time.time():.0f}"  # Current time
         metadata_list.append({ 'M': message_id, 'L': len(message) })
         t1 = T(target=self.cloud_manager.upload_to_cloud, args=(f'user_history/{conversation_id}/{message_id}', message))
         t2 = T(target=self.cloud_manager.upload_to_cloud, args=(f'user_history/{conversation_id}/metadata', json.dumps(metadata_list)))
         t1.start()
         t2.start()
-        call_cloud_save(self.user, self.api, self.openai_key, f'user_history/{conversation_id}/vectors', self.embeddings_model, message, name=message_id, split_size=3000)
+        T(target=call_cloud_save, args=(self.user, self.api, self.openai_key, f'user_history/{conversation_id}/vectors', self.embeddings_model, message, None, message_id, None, None, 3000)).start()
         t1.join()
         t2.join()
 
     def get_conversation_history(self, conversation_id, message):
         def download_conversation_metadata():
             try:
                 return json.loads(self.cloud_manager.download_text_from_cloud(f'user_history/{conversation_id}/metadata'))
```

### Comparing `vector_vault-4.2.8/vectorvault/vecreq.py` & `vector_vault-4.2.9/vectorvault/vecreq.py`

 * *Files identical despite different names*

