# Comparing `tmp/sirji-agents-0.0.2.tar.gz` & `tmp/sirji-agents-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-agents-0.0.2.tar", last modified: Wed Apr  3 15:14:21 2024, max compression
+gzip compressed data, was "sirji-agents-0.0.3.tar", last modified: Thu Apr  4 05:58:43 2024, max compression
```

## Comparing `sirji-agents-0.0.2.tar` & `sirji-agents-0.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.488916 sirji-agents-0.0.2/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3284 2024-04-03 15:14:21.488402 sirji-agents-0.0.2/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2921 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-03 15:14:21.489035 sirji-agents-0.0.2/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      665 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.479757 sirji-agents-0.0.2/sirji_agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.483112 sirji-agents-0.0.2/sirji_agents/llm/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/llm/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2447 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/llm/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/llm/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/llm/planner.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.483869 sirji-agents-0.0.2/sirji_agents/researcher/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.485626 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5284 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/embeddings/openai_assistant.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.487201 sirji-agents-0.0.2/sirji_agents/researcher/inferer/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/inferer/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/inferer/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/inferer/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/inferer/openai_assistant.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4140 2024-04-03 15:13:58.000000 sirji-agents-0.0.2/sirji_agents/researcher/researcher.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:14:21.487782 sirji-agents-0.0.2/sirji_agents.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3284 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-03 15:14:21.000000 sirji-agents-0.0.2/sirji_agents.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.310216 sirji-agents-0.0.3/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3284 2024-04-04 05:58:43.306249 sirji-agents-0.0.3/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2921 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 05:58:43.311028 sirji-agents-0.0.3/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      665 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.163338 sirji-agents-0.0.3/sirji_agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/sirji_agents/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.219792 sirji-agents-0.0.3/sirji_agents/llm/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/sirji_agents/llm/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2447 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/sirji_agents/llm/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/sirji_agents/llm/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/llm/planner.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.234182 sirji-agents-0.0.3/sirji_agents/researcher/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.255030 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5581 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/openai_assistant.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.288550 sirji-agents-0.0.3/sirji_agents/researcher/inferer/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/inferer/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/inferer/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/inferer/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/inferer/openai_assistant.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4442 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/researcher.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.291691 sirji-agents-0.0.3/sirji_agents.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3284 2024-04-04 05:58:41.000000 sirji-agents-0.0.3/sirji_agents.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-04 05:58:42.000000 sirji-agents-0.0.3/sirji_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 05:58:41.000000 sirji-agents-0.0.3/sirji_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-04 05:58:41.000000 sirji-agents-0.0.3/sirji_agents.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-04 05:58:41.000000 sirji-agents-0.0.3/sirji_agents.egg-info/top_level.txt
```

### Comparing `sirji-agents-0.0.2/LICENSE` & `sirji-agents-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.2/PKG-INFO` & `sirji-agents-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.2
+Version: 0.0.3
 Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sirji-messages==0.0.3
-Requires-Dist: sirji-tools==0.0.2
+Requires-Dist: sirji-tools==0.0.3
 Requires-Dist: openai==1.14.1
 
 # sirji-agents
 
 `sirji-agents` is a Python package designed to handle messages for Coding Agent, Planning Agent and Research Agent.
 
 ## Installation
```

### Comparing `sirji-agents-0.0.2/README.md` & `sirji-agents-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.2/setup.py` & `sirji-agents-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-agents',
-    version='0.0.2',
+    version='0.0.3',
     author='Sirji',
     description='Research, Coding and Planning agents used by Sirji.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
     include_package_data=True,  # This includes non-code files specified in MANIFEST.in
```

### Comparing `sirji-agents-0.0.2/sirji_agents/llm/base.py` & `sirji-agents-0.0.3/sirji_agents/llm/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.2/sirji_agents/researcher/embeddings/openai_assistant.py` & `sirji-agents-0.0.3/sirji_agents/researcher/embeddings/openai_assistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             self.assistant_id = self._create_assistant()
             # Update payload
             self.init_payload['assistant_id'] = self.assistant_id
 
             # Provide a way to output this updated init_payload
             logger.info(f"New assistant created with ID: {self.assistant_id}")
 
-        self.index_file_path = 'workspace/researcher/file_index.json'
+        self.index_file_path = os.path.join(self._get_workspace_folder(), '.sirji', 'researcher', 'file_index.json')
 
         # Load or initialize the index file
         self.index_data = self._load_or_initialize_index_file()
 
         logger.info("Completed initializing OpenAI Assistant Embeddings")
 
     def index(self, folder_path):
@@ -78,14 +78,21 @@
         """
         Retrieve context using embeddings match for a problem statement.
         For OpenAI Assistants API, this step is not needed.
         To re-use the assistant_id, pass it in the retrieved context.
         """
         return ""
 
+    def _get_workspace_folder(self):
+        workspace = os.environ.get("SIRJI_WORKSPACE")
+        if workspace is None:
+            raise ValueError(
+                "SIRJI_WORKSPACE is not set as an environment variable")
+        return workspace
+
     def _create_assistant(self):
         logger.info("Creating a new assistant instance")
         """
         Create a new assistant
         """
         assistant = self.client.beta.assistants.create(
             name="Research Assistant",
```

### Comparing `sirji-agents-0.0.2/sirji_agents/researcher/inferer/base.py` & `sirji-agents-0.0.3/sirji_agents/researcher/inferer/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.2/sirji_agents/researcher/inferer/openai_assistant.py` & `sirji-agents-0.0.3/sirji_agents/researcher/inferer/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.2/sirji_agents/researcher/researcher.py` & `sirji-agents-0.0.3/sirji_agents/researcher/researcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,29 +19,36 @@
             embeddings_type, init_payload)
 
         self.init_payload = self._embeddings_manager.init_payload
 
         self._inferer = InfererFactory.get_instance(
             inferer_type, self.init_payload)
 
-        self._research_folder = 'workspace/researcher'
+        self._research_folder = os.path.join(self._get_workspace_folder(), '.sirji', "researcher")
 
         logger.info("Completed initializing researcher")
 
     def message(self, input_message):
         """Public method to process input messages and dispatch actions."""
         parsed_message = message_parse(input_message)
         action = parsed_message.get("ACTION")
 
         if action == ActionEnum.TRAIN_USING_SEARCH_TERM.name:
             return self._handle_train_using_search_term(parsed_message)
         elif action == ActionEnum.TRAIN_USING_URL.name:
             return self._handle_train_using_url(parsed_message)
         elif action == ActionEnum.INFER.name:
             return self._handle_infer(parsed_message)
+        
+    def _get_workspace_folder(self):
+        workspace = os.environ.get("SIRJI_WORKSPACE")
+        if workspace is None:
+            raise ValueError(
+                "SIRJI_WORKSPACE is not set as an environment variable")
+        return workspace
 
     def _handle_train_using_search_term(self, parsed_message):
         """Private method to handle training using a search term."""
         logger.info(
             f"Training using search term: {parsed_message.get('TERM')}")
         self._search_and_index(parsed_message.get('TERM'))
```

### Comparing `sirji-agents-0.0.2/sirji_agents.egg-info/PKG-INFO` & `sirji-agents-0.0.3/sirji_agents.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.2
+Version: 0.0.3
 Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sirji-messages==0.0.3
-Requires-Dist: sirji-tools==0.0.2
+Requires-Dist: sirji-tools==0.0.3
 Requires-Dist: openai==1.14.1
 
 # sirji-agents
 
 `sirji-agents` is a Python package designed to handle messages for Coding Agent, Planning Agent and Research Agent.
 
 ## Installation
```

### Comparing `sirji-agents-0.0.2/sirji_agents.egg-info/SOURCES.txt` & `sirji-agents-0.0.3/sirji_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

