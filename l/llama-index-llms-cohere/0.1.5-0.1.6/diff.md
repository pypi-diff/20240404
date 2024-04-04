# Comparing `tmp/llama_index_llms_cohere-0.1.5.tar.gz` & `tmp/llama_index_llms_cohere-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_cohere-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_llms_cohere-0.1.6.tar", max compression
```

## Comparing `llama_index_llms_cohere-0.1.5.tar` & `llama_index_llms_cohere-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       38 2024-03-29 16:11:38.705421 llama_index_llms_cohere-0.1.5/README.md
--rw-r--r--   0        0        0       70 2024-03-29 16:11:38.705421 llama_index_llms_cohere-0.1.5/llama_index/llms/cohere/__init__.py
--rw-r--r--   0        0        0    11689 2024-03-29 16:11:38.705421 llama_index_llms_cohere-0.1.5/llama_index/llms/cohere/base.py
--rw-r--r--   0        0        0     3955 2024-03-29 16:11:38.705421 llama_index_llms_cohere-0.1.5/llama_index/llms/cohere/utils.py
--rw-r--r--   0        0        0     1439 2024-03-29 16:11:38.705421 llama_index_llms_cohere-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 llama_index_llms_cohere-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/README.md
+-rw-r--r--   0        0        0       70 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/__init__.py
+-rw-r--r--   0        0        0    11689 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/base.py
+-rw-r--r--   0        0        0     3985 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/utils.py
+-rw-r--r--   0        0        0     1439 2024-04-04 14:59:01.166962 llama_index_llms_cohere-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 llama_index_llms_cohere-0.1.6/PKG-INFO
```

### Comparing `llama_index_llms_cohere-0.1.5/llama_index/llms/cohere/base.py` & `llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_cohere-0.1.5/llama_index/llms/cohere/utils.py` & `llama_index_llms_cohere-0.1.6/llama_index/llms/cohere/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
 COMMAND_MODELS = {
     "command-r": 128000,
+    "command-r-plus": 128000,
     "command": 4096,
     "command-nightly": 4096,
     "command-light": 4096,
     "command-light-nightly": 4096,
 }
 
 GENERATION_MODELS = {"base": 2048, "base-light": 2048}
```

### Comparing `llama_index_llms_cohere-0.1.5/pyproject.toml` & `llama_index_llms_cohere-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms cohere integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-cohere"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-cohere = "^5.1.1"
+cohere = "^5.1.2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_llms_cohere-0.1.5/PKG-INFO` & `llama_index_llms_cohere-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-cohere
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index llms cohere integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cohere (>=5.1.1,<6.0.0)
+Requires-Dist: cohere (>=5.1.2,<6.0.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Cohere
```

