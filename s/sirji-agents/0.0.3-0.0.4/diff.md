# Comparing `tmp/sirji-agents-0.0.3.tar.gz` & `tmp/sirji-agents-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-agents-0.0.3.tar", last modified: Thu Apr  4 05:58:43 2024, max compression
+gzip compressed data, was "sirji-agents-0.0.4.tar", last modified: Thu Apr  4 13:12:11 2024, max compression
```

## Comparing `sirji-agents-0.0.3.tar` & `sirji-agents-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.310216 sirji-agents-0.0.3/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3284 2024-04-04 05:58:43.306249 sirji-agents-0.0.3/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2921 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 05:58:43.311028 sirji-agents-0.0.3/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      665 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.163338 sirji-agents-0.0.3/sirji_agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/sirji_agents/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.219792 sirji-agents-0.0.3/sirji_agents/llm/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/sirji_agents/llm/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2447 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/sirji_agents/llm/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-04 05:57:46.000000 sirji-agents-0.0.3/sirji_agents/llm/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/llm/planner.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.234182 sirji-agents-0.0.3/sirji_agents/researcher/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.255030 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5581 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/embeddings/openai_assistant.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.288550 sirji-agents-0.0.3/sirji_agents/researcher/inferer/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/inferer/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/inferer/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/inferer/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/inferer/openai_assistant.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4442 2024-04-04 05:57:47.000000 sirji-agents-0.0.3/sirji_agents/researcher/researcher.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 05:58:43.291691 sirji-agents-0.0.3/sirji_agents.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3284 2024-04-04 05:58:41.000000 sirji-agents-0.0.3/sirji_agents.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-04 05:58:42.000000 sirji-agents-0.0.3/sirji_agents.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 05:58:41.000000 sirji-agents-0.0.3/sirji_agents.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-04 05:58:41.000000 sirji-agents-0.0.3/sirji_agents.egg-info/requires.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-04 05:58:41.000000 sirji-agents-0.0.3/sirji_agents.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.476536 sirji-agents-0.0.4/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-04 13:12:11.475705 sirji-agents-0.0.4/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3060 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 13:12:11.476765 sirji-agents-0.0.4/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      684 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.464194 sirji-agents-0.0.4/sirji_agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      188 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.468335 sirji-agents-0.0.4/sirji_agents/llm/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/llm/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2447 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/llm/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      228 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/llm/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      232 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/llm/planner.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.469345 sirji-agents-0.0.4/sirji_agents/researcher/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       67 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.471513 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      385 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      342 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     5581 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/embeddings/openai_assistant.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.473950 sirji-agents-0.0.4/sirji_agents/researcher/inferer/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/inferer/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1075 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/inferer/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      324 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/inferer/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4364 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/inferer/openai_assistant.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4442 2024-04-04 13:11:54.000000 sirji-agents-0.0.4/sirji_agents/researcher/researcher.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:12:11.474868 sirji-agents-0.0.4/sirji_agents.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3436 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      794 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       56 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/requires.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       13 2024-04-04 13:12:11.000000 sirji-agents-0.0.4/sirji_agents.egg-info/top_level.txt
```

### Comparing `sirji-agents-0.0.3/LICENSE` & `sirji-agents-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.3/PKG-INFO` & `sirji-agents-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 Metadata-Version: 2.1
 Name: sirji-agents
-Version: 0.0.3
+Version: 0.0.4
 Summary: Research, Coding and Planning agents used by Sirji.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
+License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sirji-messages==0.0.3
-Requires-Dist: sirji-tools==0.0.3
+Requires-Dist: sirji-messages==0.0.4
+Requires-Dist: sirji-tools==0.0.4
 Requires-Dist: openai==1.14.1
 
 # sirji-agents
 
-`sirji-agents` is a Python package designed to handle messages for Coding Agent, Planning Agent and Research Agent.
+`sirji-agents` is a PyPI package that implements three key agents for Sirji:
 
-## Installation
+- Coding Agent
+- Planning Agent
+- Research Agent
 
-Install `sirji-agents` quickly with pip:
+It Utilizes:
 
-```
+- OpenAI Chat Completions API
+- OpenAI Assistants API
+
+This package communicates with models and RAG assistants.
+
+## Installation
+
+```zsh
 pip install sirji-agents
 ```
 
+Run the following to enable playwright:
+
+```zsh
+playwright install
+```
+
 ## Usages
 
 ### Research Agent
 
 ### Initialization
 
 ```python
@@ -113,8 +129,8 @@
 
 # call the Planner and update the history variable
 response_message, planner_history = planner.message(message_str, planner_history)
 ```
 
 ## License
 
-`sirji-agents` is made available under the MIT License. See the included LICENSE file for more details.
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `sirji-agents-0.0.3/README.md` & `sirji-agents-0.0.4/sirji_agents.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,48 @@
+Metadata-Version: 2.1
+Name: sirji-agents
+Version: 0.0.4
+Summary: Research, Coding and Planning agents used by Sirji.
+Home-page: https://github.com/sirji-ai/sirji
+Author: Sirji
+License: MIT
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sirji-messages==0.0.4
+Requires-Dist: sirji-tools==0.0.4
+Requires-Dist: openai==1.14.1
+
 # sirji-agents
 
-`sirji-agents` is a Python package designed to handle messages for Coding Agent, Planning Agent and Research Agent.
+`sirji-agents` is a PyPI package that implements three key agents for Sirji:
 
-## Installation
+- Coding Agent
+- Planning Agent
+- Research Agent
 
-Install `sirji-agents` quickly with pip:
+It Utilizes:
 
-```
+- OpenAI Chat Completions API
+- OpenAI Assistants API
+
+This package communicates with models and RAG assistants.
+
+## Installation
+
+```zsh
 pip install sirji-agents
 ```
 
+Run the following to enable playwright:
+
+```zsh
+playwright install
+```
+
 ## Usages
 
 ### Research Agent
 
 ### Initialization
 
 ```python
@@ -100,8 +129,8 @@
 
 # call the Planner and update the history variable
 response_message, planner_history = planner.message(message_str, planner_history)
 ```
 
 ## License
 
-`sirji-agents` is made available under the MIT License. See the included LICENSE file for more details.
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `sirji-agents-0.0.3/setup.py` & `sirji-agents-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-agents',
-    version='0.0.3',
+    version='0.0.4',
     author='Sirji',
     description='Research, Coding and Planning agents used by Sirji.',
+    license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
     include_package_data=True,  # This includes non-code files specified in MANIFEST.in
     install_requires=[
         x for x in open("./requirements.txt", "r+").readlines() if x.strip()
```

### Comparing `sirji-agents-0.0.3/sirji_agents/llm/base.py` & `sirji-agents-0.0.4/sirji_agents/llm/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.3/sirji_agents/researcher/embeddings/openai_assistant.py` & `sirji-agents-0.0.4/sirji_agents/researcher/embeddings/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.3/sirji_agents/researcher/inferer/base.py` & `sirji-agents-0.0.4/sirji_agents/researcher/inferer/base.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.3/sirji_agents/researcher/inferer/openai_assistant.py` & `sirji-agents-0.0.4/sirji_agents/researcher/inferer/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.3/sirji_agents/researcher/researcher.py` & `sirji-agents-0.0.4/sirji_agents/researcher/researcher.py`

 * *Files identical despite different names*

### Comparing `sirji-agents-0.0.3/sirji_agents.egg-info/SOURCES.txt` & `sirji-agents-0.0.4/sirji_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

