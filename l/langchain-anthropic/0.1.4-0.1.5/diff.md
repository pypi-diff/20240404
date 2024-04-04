# Comparing `tmp/langchain_anthropic-0.1.4.tar.gz` & `tmp/langchain_anthropic-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_anthropic-0.1.4.tar", max compression
+gzip compressed data, was "langchain_anthropic-0.1.5.tar", max compression
```

## Comparing `langchain_anthropic-0.1.4.tar` & `langchain_anthropic-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-03-08 21:49:03.914383 langchain_anthropic-0.1.4/LICENSE
--rw-r--r--   0        0        0     1215 2024-03-08 21:49:03.914383 langchain_anthropic-0.1.4/README.md
--rw-r--r--   0        0        0      225 2024-03-08 21:49:03.914383 langchain_anthropic-0.1.4/langchain_anthropic/__init__.py
--rw-r--r--   0        0        0    10450 2024-03-08 21:49:03.914383 langchain_anthropic-0.1.4/langchain_anthropic/chat_models.py
--rw-r--r--   0        0        0    10569 2024-03-08 21:49:03.914383 langchain_anthropic-0.1.4/langchain_anthropic/experimental.py
--rw-r--r--   0        0        0    12362 2024-03-08 21:49:03.914383 langchain_anthropic-0.1.4/langchain_anthropic/llms.py
--rw-r--r--   0        0        0        0 2024-03-08 21:49:03.914383 langchain_anthropic-0.1.4/langchain_anthropic/py.typed
--rw-r--r--   0        0        0     2674 2024-03-08 21:49:03.914383 langchain_anthropic-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2089 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-04 20:38:16.678844 langchain_anthropic-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1215 2024-04-04 20:38:16.678844 langchain_anthropic-0.1.5/README.md
+-rw-r--r--   0        0        0      225 2024-04-04 20:38:16.678844 langchain_anthropic-0.1.5/langchain_anthropic/__init__.py
+-rw-r--r--   0        0        0    17208 2024-04-04 20:38:16.678844 langchain_anthropic-0.1.5/langchain_anthropic/chat_models.py
+-rw-r--r--   0        0        0     4908 2024-04-04 20:38:16.678844 langchain_anthropic-0.1.5/langchain_anthropic/experimental.py
+-rw-r--r--   0        0        0    11687 2024-04-04 20:38:16.678844 langchain_anthropic-0.1.5/langchain_anthropic/llms.py
+-rw-r--r--   0        0        0     2194 2024-04-04 20:38:16.678844 langchain_anthropic-0.1.5/langchain_anthropic/output_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-04 20:38:16.678844 langchain_anthropic-0.1.5/langchain_anthropic/py.typed
+-rw-r--r--   0        0        0     2677 2024-04-04 20:38:16.682844 langchain_anthropic-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2094 1970-01-01 00:00:00.000000 langchain_anthropic-0.1.5/PKG-INFO
```

### Comparing `langchain_anthropic-0.1.4/LICENSE` & `langchain_anthropic-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.4/README.md` & `langchain_anthropic-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_anthropic-0.1.4/langchain_anthropic/llms.py` & `langchain_anthropic-0.1.5/langchain_anthropic/llms.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,51 +135,39 @@
         # Never want model to invent new turns of Human / Assistant dialog.
         stop.extend([self.HUMAN_PROMPT])
 
         return stop
 
 
 class AnthropicLLM(LLM, _AnthropicCommon):
-    """Anthropic large language models.
+    """Anthropic large language model.
 
-    To use, you should have the ``anthropic`` python package installed, and the
-    environment variable ``ANTHROPIC_API_KEY`` set with your API key, or pass
-    it as a named parameter to the constructor.
+    To use, you should have the environment variable ``ANTHROPIC_API_KEY``
+    set with your API key, or pass it as a named parameter to the constructor.
 
     Example:
         .. code-block:: python
 
-            import anthropic
-            from langchain_community.llms import Anthropic
+            from langchain_anthropic import AnthropicLLM
 
-            model = Anthropic(model="<model_name>", anthropic_api_key="my-api-key")
-
-            # Simplest invocation, automatically wrapped with HUMAN_PROMPT
-            # and AI_PROMPT.
-            response = model("What are the biggest risks facing humanity?")
-
-            # Or if you want to use the chat mode, build a few-shot-prompt, or
-            # put words in the Assistant's mouth, use HUMAN_PROMPT and AI_PROMPT:
-            raw_prompt = "What are the biggest risks facing humanity?"
-            prompt = f"{anthropic.HUMAN_PROMPT} {prompt}{anthropic.AI_PROMPT}"
-            response = model(prompt)
+            model = AnthropicLLM()
     """
 
     class Config:
         """Configuration for this pydantic object."""
 
         allow_population_by_field_name = True
         arbitrary_types_allowed = True
 
     @root_validator()
     def raise_warning(cls, values: Dict) -> Dict:
         """Raise warning that this class is deprecated."""
         warnings.warn(
             "This Anthropic LLM is deprecated. "
-            "Please use `from langchain_community.chat_models import ChatAnthropic` "
+            "Please use `from langchain_anthropic import ChatAnthropic` "
             "instead"
         )
         return values
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
```

### Comparing `langchain_anthropic-0.1.4/pyproject.toml` & `langchain_anthropic-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-anthropic"
-version = "0.1.4"
+version = "0.1.5"
 description = "An integration package connecting AnthropicMessages and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1"
+langchain-core = "^0.1.33"
 anthropic = ">=0.17.0,<1"
 defusedxml = { version = "^0.7.1", optional = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_anthropic-0.1.4/PKG-INFO` & `langchain_anthropic-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-anthropic
-Version: 0.1.4
+Version: 0.1.5
 Summary: An integration package connecting AnthropicMessages and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anthropic (>=0.17.0,<1)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: langchain-core (>=0.1,<0.2)
+Requires-Dist: langchain-core (>=0.1.33,<0.2.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/anthropic
 Description-Content-Type: text/markdown
 
 # langchain-anthropic
 
 This package contains the LangChain integration for Anthropic's generative models.
```

