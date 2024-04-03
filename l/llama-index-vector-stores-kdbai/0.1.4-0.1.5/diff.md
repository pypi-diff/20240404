# Comparing `tmp/llama_index_vector_stores_kdbai-0.1.4.tar.gz` & `tmp/llama_index_vector_stores_kdbai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_kdbai-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_kdbai-0.1.5.tar", max compression
```

## Comparing `llama_index_vector_stores_kdbai-0.1.4.tar` & `llama_index_vector_stores_kdbai-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       47 2024-03-29 16:56:50.151683 llama_index_vector_stores_kdbai-0.1.4/README.md
--rw-r--r--   0        0        0       99 2024-03-29 16:56:50.152008 llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/__init__.py
--rw-r--r--   0        0        0     6875 2024-03-31 21:32:29.669989 llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/base.py
--rw-r--r--   0        0        0      735 2024-03-29 16:56:50.152279 llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/utils.py
--rw-r--r--   0        0        0     1700 2024-04-01 15:49:44.031952 llama_index_vector_stores_kdbai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 llama_index_vector_stores_kdbai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-03 22:41:02.101293 llama_index_vector_stores_kdbai-0.1.5/README.md
+-rw-r--r--   0        0        0       99 2024-04-03 22:41:02.101293 llama_index_vector_stores_kdbai-0.1.5/llama_index/vector_stores/kdbai/__init__.py
+-rw-r--r--   0        0        0     6878 2024-04-03 22:41:02.101293 llama_index_vector_stores_kdbai-0.1.5/llama_index/vector_stores/kdbai/base.py
+-rw-r--r--   0        0        0      735 2024-04-03 22:41:02.101293 llama_index_vector_stores_kdbai-0.1.5/llama_index/vector_stores/kdbai/utils.py
+-rw-r--r--   0        0        0     1700 2024-04-03 22:41:02.101293 llama_index_vector_stores_kdbai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 llama_index_vector_stores_kdbai-0.1.5/PKG-INFO
```

### Comparing `llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/base.py` & `llama_index_vector_stores_kdbai-0.1.5/llama_index/vector_stores/kdbai/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
                     self._table.insert(batch, warn=False)
                     logger.info(f"inserted batch {i}")
                 except Exception as e:
                     logger.exception(
                         f"Failed to insert batch {i} of documents into the datastore: {e}"
                     )
 
-            return List(df["document_id"])
+            return df["document_id"].tolist()
 
         except Exception as e:
             logger.error(f"Error preparing data for KDB.AI: {e}.")
 
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
         if query.filters is None:
             filter = []
```

### Comparing `llama_index_vector_stores_kdbai-0.1.4/llama_index/vector_stores/kdbai/utils.py` & `llama_index_vector_stores_kdbai-0.1.5/llama_index/vector_stores/kdbai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_vector_stores_kdbai-0.1.4/pyproject.toml` & `llama_index_vector_stores_kdbai-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores kdbai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-kdbai"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 pykx = "^2.1.1"
 kdbai-client = "^0.1.2"
```

### Comparing `llama_index_vector_stores_kdbai-0.1.4/PKG-INFO` & `llama_index_vector_stores_kdbai-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-kdbai
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index vector_stores kdbai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

