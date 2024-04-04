# Comparing `tmp/vector_vault-4.3.2.tar.gz` & `tmp/vector_vault-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.3.2.tar", last modified: Thu Apr  4 06:08:05 2024, max compression
+gzip compressed data, was "vector_vault-4.3.3.tar", last modified: Thu Apr  4 06:19:26 2024, max compression
```

## Comparing `vector_vault-4.3.2.tar` & `vector_vault-4.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:08:05.022287 vector_vault-4.3.2/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.2/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 06:08:05.022135 vector_vault-4.3.2/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.2/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-04 06:08:05.022321 vector_vault-4.3.2/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-04 06:07:49.000000 vector_vault-4.3.2/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:08:05.018777 vector_vault-4.3.2/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 06:08:04.000000 vector_vault-4.3.2/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-04 06:08:04.000000 vector_vault-4.3.2/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-04 06:08:04.000000 vector_vault-4.3.2/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-04 06:08:04.000000 vector_vault-4.3.2/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-04 06:08:04.000000 vector_vault-4.3.2/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:08:05.021809 vector_vault-4.3.2/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.2/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.3.2/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.2/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5982 2024-04-04 06:07:20.000000 vector_vault-4.3.2/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.2/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.2/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-04 06:07:40.000000 vector_vault-4.3.2/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-04 06:07:37.000000 vector_vault-4.3.2/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62538 2024-04-04 06:07:35.000000 vector_vault-4.3.2/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.2/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.2/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:19:26.273832 vector_vault-4.3.3/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.3.3/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 06:19:26.273684 vector_vault-4.3.3/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.3.3/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-04 06:19:26.273868 vector_vault-4.3.3/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1111 2024-04-04 06:19:18.000000 vector_vault-4.3.3/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:19:26.270388 vector_vault-4.3.3/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23345 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-04 06:19:26.000000 vector_vault-4.3.3/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-04 06:19:26.273310 vector_vault-4.3.3/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.3.3/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-03-26 17:36:03.000000 vector_vault-4.3.3/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.3.3/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5982 2024-04-04 06:07:20.000000 vector_vault-4.3.3/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2023-12-30 00:40:36.000000 vector_vault-4.3.3/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.3.3/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-04 06:07:40.000000 vector_vault-4.3.3/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    20814 2024-04-04 06:07:37.000000 vector_vault-4.3.3/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62521 2024-04-04 06:19:13.000000 vector_vault-4.3.3/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.3.3/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.3.3/vectorvault/wrap.py
```

### Comparing `vector_vault-4.3.2/LICENSE` & `vector_vault-4.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/PKG-INFO` & `vector_vault-4.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.3.2
+Version: 4.3.3
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.3.2/README.md` & `vector_vault-4.3.3/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/setup.py` & `vector_vault-4.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.3.2",
+    version="4.3.3",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.3.2/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.3.3/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.3.2
+Version: 4.3.3
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.3.2/vectorvault/ai.py` & `vector_vault-4.3.3/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/vectorvault/cloud_api.py` & `vector_vault-4.3.3/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/vectorvault/cloudmanager.py` & `vector_vault-4.3.3/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/vectorvault/creds.py` & `vector_vault-4.3.3/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/vectorvault/download.py` & `vector_vault-4.3.3/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/vectorvault/itemize.py` & `vector_vault-4.3.3/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/vectorvault/tools_gpt.py` & `vector_vault-4.3.3/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.3.2/vectorvault/vault.py` & `vector_vault-4.3.3/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.verbose = verbose
         self.embeddings_model = embeddings_model if embeddings_model else 'text-embedding-3-small'
         self.dims = 1536 if embeddings_model != 'text-embedding-3-large' else 3072
         if openai_key:
             self.openai_key = openai_key
             openai.api_key = self.openai_key
         try:
-            self.cloud_manager = CloudManager(self.user, self.api, self.vault, self.openai_key)
+            self.cloud_manager = CloudManager(self.user, self.api, self.vault)
             print(f'Connected vault: {self.vault}') if self.verbose else 0 
         except Exception as e:
             print('API KEY NOT FOUND or no internet connection!', e)
             # user can still use the get_chat() function without an api key
             self.cloud_manager = None
 
         T(target=self.init_vecs)
```

### Comparing `vector_vault-4.3.2/vectorvault/vecreq.py` & `vector_vault-4.3.3/vectorvault/vecreq.py`

 * *Files identical despite different names*

