# Comparing `tmp/llama_index_llms_anthropic-0.1.7.tar.gz` & `tmp/llama_index_llms_anthropic-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_anthropic-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_llms_anthropic-0.1.8.tar", max compression
```

## Comparing `llama_index_llms_anthropic-0.1.7.tar` & `llama_index_llms_anthropic-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       41 2024-03-19 15:27:11.985205 llama_index_llms_anthropic-0.1.7/README.md
--rw-r--r--   0        0        0       79 2024-03-19 15:27:11.985205 llama_index_llms_anthropic-0.1.7/llama_index/llms/anthropic/__init__.py
--rw-r--r--   0        0        0     9244 2024-03-19 15:27:11.985205 llama_index_llms_anthropic-0.1.7/llama_index/llms/anthropic/base.py
--rw-r--r--   0        0        0     3394 2024-03-19 15:27:11.985205 llama_index_llms_anthropic-0.1.7/llama_index/llms/anthropic/utils.py
--rw-r--r--   0        0        0     1455 2024-03-19 15:27:11.985205 llama_index_llms_anthropic-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 llama_index_llms_anthropic-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/README.md
+-rw-r--r--   0        0        0       79 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/__init__.py
+-rw-r--r--   0        0        0     9812 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/base.py
+-rw-r--r--   0        0        0     3394 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/utils.py
+-rw-r--r--   0        0        0     1455 2024-04-04 01:49:31.042679 llama_index_llms_anthropic-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 llama_index_llms_anthropic-0.1.8/PKG-INFO
```

### Comparing `llama_index_llms_anthropic-0.1.7/llama_index/llms/anthropic/base.py` & `llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,29 @@
 import anthropic
 
 DEFAULT_ANTHROPIC_MODEL = "claude-2.1"
 DEFAULT_ANTHROPIC_MAX_TOKENS = 512
 
 
 class Anthropic(LLM):
+    """Anthropic LLM.
+
+    Examples:
+        `pip install llama-index-llms-anthropic`
+
+        ```python
+        from llama_index.llms.anthropic import Anthropic
+
+        llm = Anthropic(model="claude-instant-1")
+        resp = llm.stream_complete("Paul Graham is ")
+        for r in resp:
+            print(r.delta, end="")
+        ```
+    """
+
     model: str = Field(
         default=DEFAULT_ANTHROPIC_MODEL, description="The anthropic model to use."
     )
     temperature: float = Field(
         default=DEFAULT_TEMPERATURE,
         description="The temperature to use for sampling.",
         gte=0.0,
@@ -75,28 +90,37 @@
         max_tokens: int = DEFAULT_ANTHROPIC_MAX_TOKENS,
         base_url: Optional[str] = None,
         timeout: Optional[float] = None,
         max_retries: int = 10,
         api_key: Optional[str] = None,
         additional_kwargs: Optional[Dict[str, Any]] = None,
         callback_manager: Optional[CallbackManager] = None,
+        default_headers: Optional[Dict[str, str]] = None,
         system_prompt: Optional[str] = None,
         messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
         completion_to_prompt: Optional[Callable[[str], str]] = None,
         pydantic_program_mode: PydanticProgramMode = PydanticProgramMode.DEFAULT,
         output_parser: Optional[BaseOutputParser] = None,
     ) -> None:
         additional_kwargs = additional_kwargs or {}
         callback_manager = callback_manager or CallbackManager([])
 
         self._client = anthropic.Anthropic(
-            api_key=api_key, base_url=base_url, timeout=timeout, max_retries=max_retries
+            api_key=api_key,
+            base_url=base_url,
+            timeout=timeout,
+            max_retries=max_retries,
+            default_headers=default_headers,
         )
         self._aclient = anthropic.AsyncAnthropic(
-            api_key=api_key, base_url=base_url, timeout=timeout, max_retries=max_retries
+            api_key=api_key,
+            base_url=base_url,
+            timeout=timeout,
+            max_retries=max_retries,
+            default_headers=default_headers,
         )
 
         super().__init__(
             temperature=temperature,
             max_tokens=max_tokens,
             additional_kwargs=additional_kwargs,
             base_url=base_url,
```

### Comparing `llama_index_llms_anthropic-0.1.7/llama_index/llms/anthropic/utils.py` & `llama_index_llms_anthropic-0.1.8/llama_index/llms/anthropic/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_anthropic-0.1.7/pyproject.toml` & `llama_index_llms_anthropic-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms anthropic integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-anthropic"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 anthropic = "^0.20.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_llms_anthropic-0.1.7/PKG-INFO` & `llama_index_llms_anthropic-0.1.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-anthropic
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index llms anthropic integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

