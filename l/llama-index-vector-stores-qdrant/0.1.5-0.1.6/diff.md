# Comparing `tmp/llama_index_vector_stores_qdrant-0.1.5.tar.gz` & `tmp/llama_index_vector_stores_qdrant-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_qdrant-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_qdrant-0.1.6.tar", max compression
```

## Comparing `llama_index_vector_stores_qdrant-0.1.5.tar` & `llama_index_vector_stores_qdrant-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       47 2024-03-28 16:08:26.968369 llama_index_vector_stores_qdrant-0.1.5/README.md
--rw-r--r--   0        0        0      101 2024-03-28 16:08:26.968369 llama_index_vector_stores_qdrant-0.1.5/llama_index/vector_stores/qdrant/__init__.py
--rw-r--r--   0        0        0    31296 2024-03-28 16:08:26.968369 llama_index_vector_stores_qdrant-0.1.5/llama_index/vector_stores/qdrant/base.py
--rw-r--r--   0        0        0     6897 2024-03-28 16:08:26.968369 llama_index_vector_stores_qdrant-0.1.5/llama_index/vector_stores/qdrant/utils.py
--rw-r--r--   0        0        0     1600 2024-03-28 16:08:26.968369 llama_index_vector_stores_qdrant-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/README.md
+-rw-r--r--   0        0        0      101 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/__init__.py
+-rw-r--r--   0        0        0    31682 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/base.py
+-rw-r--r--   0        0        0     6897 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/utils.py
+-rw-r--r--   0        0        0     1600 2024-04-04 01:40:11.428289 llama_index_vector_stores_qdrant-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 llama_index_vector_stores_qdrant-0.1.6/PKG-INFO
```

### Comparing `llama_index_vector_stores_qdrant-0.1.5/llama_index/vector_stores/qdrant/base.py` & `llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,24 @@
             enable_hybrid=enable_hybrid,
         )
 
     @classmethod
     def class_name(cls) -> str:
         return "QdrantVectorStore"
 
+    def set_query_functions(
+        self,
+        sparse_doc_fn: Optional[SparseEncoderCallable] = None,
+        sparse_query_fn: Optional[SparseEncoderCallable] = None,
+        hybrid_fusion_fn: Optional[HybridFusionCallable] = None,
+    ):
+        self._sparse_doc_fn = sparse_doc_fn
+        self._sparse_query_fn = sparse_query_fn
+        self._hybrid_fusion_fn = hybrid_fusion_fn
+
     def _build_points(self, nodes: List[BaseNode]) -> Tuple[List[Any], List[str]]:
         ids = []
         points = []
         for node_batch in iter_batch(nodes, self.batch_size):
             node_ids = []
             vectors: List[Any] = []
             sparse_vectors: List[List[float]] = []
```

### Comparing `llama_index_vector_stores_qdrant-0.1.5/llama_index/vector_stores/qdrant/utils.py` & `llama_index_vector_stores_qdrant-0.1.6/llama_index/vector_stores/qdrant/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_qdrant-0.1.5/pyproject.toml` & `llama_index_vector_stores_qdrant-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores qdrant integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-qdrant"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 llama-index-core = "^0.10.1"
 qdrant-client = "^1.7.1"
 grpcio = "^1.60.0"
```

### Comparing `llama_index_vector_stores_qdrant-0.1.5/PKG-INFO` & `llama_index_vector_stores_qdrant-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-qdrant
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index vector_stores qdrant integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

