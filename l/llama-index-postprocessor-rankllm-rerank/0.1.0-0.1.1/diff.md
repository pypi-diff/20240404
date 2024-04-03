# Comparing `tmp/llama_index_postprocessor_rankllm_rerank-0.1.0.tar.gz` & `tmp/llama_index_postprocessor_rankllm_rerank-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_rankllm_rerank-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_rankllm_rerank-0.1.1.tar", max compression
```

## Comparing `llama_index_postprocessor_rankllm_rerank-0.1.0.tar` & `llama_index_postprocessor_rankllm_rerank-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      479 2024-03-28 17:03:38.481370 llama_index_postprocessor_rankllm_rerank-0.1.0/README.md
--rw-r--r--   0        0        0      102 2024-03-28 17:03:38.483053 llama_index_postprocessor_rankllm_rerank-0.1.0/llama_index/postprocessor/rankllm_rerank/__init__.py
--rw-r--r--   0        0        0     3505 2024-03-28 17:03:38.483800 llama_index_postprocessor_rankllm_rerank-0.1.0/llama_index/postprocessor/rankllm_rerank/base.py
--rw-r--r--   0        0        0     1618 2024-03-28 17:04:17.184326 llama_index_postprocessor_rankllm_rerank-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 llama_index_postprocessor_rankllm_rerank-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1637 2024-03-29 21:18:24.328183 llama_index_postprocessor_rankllm_rerank-0.1.1/README.md
+-rw-r--r--   0        0        0      102 2024-03-29 21:18:24.328183 llama_index_postprocessor_rankllm_rerank-0.1.1/llama_index/postprocessor/rankllm_rerank/__init__.py
+-rw-r--r--   0        0        0     3505 2024-03-29 21:18:24.328183 llama_index_postprocessor_rankllm_rerank-0.1.1/llama_index/postprocessor/rankllm_rerank/base.py
+-rw-r--r--   0        0        0     1618 2024-03-29 21:18:24.328183 llama_index_postprocessor_rankllm_rerank-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 llama_index_postprocessor_rankllm_rerank-0.1.1/PKG-INFO
```

### Comparing `llama_index_postprocessor_rankllm_rerank-0.1.0/llama_index/postprocessor/rankllm_rerank/base.py` & `llama_index_postprocessor_rankllm_rerank-0.1.1/llama_index/postprocessor/rankllm_rerank/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_postprocessor_rankllm_rerank-0.1.0/pyproject.toml` & `llama_index_postprocessor_rankllm_rerank-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor rankllm-rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-rankllm-rerank"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
```

