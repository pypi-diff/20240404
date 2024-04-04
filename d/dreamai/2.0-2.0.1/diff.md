# Comparing `tmp/dreamai-2.0.tar.gz` & `tmp/dreamai-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai-2.0.tar", max compression
+gzip compressed data, was "dreamai-2.0.1.tar", max compression
```

## Comparing `dreamai-2.0.tar` & `dreamai-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0/dreamai/__init__.py
--rw-r--r--   0        0        0     3040 2024-04-03 18:36:32.193450 dreamai-2.0/dreamai/ai.py
--rw-r--r--   0        0        0     4959 2024-04-04 15:15:49.821233 dreamai-2.0/dreamai/chroma.py
--rw-r--r--   0        0        0     1902 2024-04-03 19:08:30.427986 dreamai-2.0/dreamai/pdf.py
--rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0/dreamai/templates.py
--rw-r--r--   0        0        0     5693 2024-04-03 18:34:42.550727 dreamai-2.0/dreamai/utils.py
--rw-r--r--   0        0        0      676 2024-04-04 15:03:56.280560 dreamai-2.0/pyproject.toml
--rw-r--r--   0        0        0     1092 1970-01-01 00:00:00.000000 dreamai-2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 18:01:24.734686 dreamai-2.0.1/dreamai/__init__.py
+-rw-r--r--   0        0        0     3040 2024-04-03 18:36:32.193450 dreamai-2.0.1/dreamai/ai.py
+-rw-r--r--   0        0        0     4958 2024-04-04 18:12:01.063564 dreamai-2.0.1/dreamai/chroma.py
+-rw-r--r--   0        0        0     1881 2024-04-04 18:10:25.180688 dreamai-2.0.1/dreamai/pdf.py
+-rw-r--r--   0        0        0     1242 2024-04-03 18:50:22.543583 dreamai-2.0.1/dreamai/templates.py
+-rw-r--r--   0        0        0     5693 2024-04-03 18:34:42.550727 dreamai-2.0.1/dreamai/utils.py
+-rw-r--r--   0        0        0      678 2024-04-04 18:13:16.578683 dreamai-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 dreamai-2.0.1/PKG-INFO
```

### Comparing `dreamai-2.0/dreamai/ai.py` & `dreamai-2.0.1/dreamai/ai.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0/dreamai/chroma.py` & `dreamai-2.0.1/dreamai/chroma.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,37 +117,37 @@
     return ids
 
 
 def query_collection(
     query_text: str,
     collection: ChromaCollection,
     n_results: int = 10,
-    n_traversal_steps: int = 2,
+    n_prev_links: int = 2,
+    n_next_links: int = 2,
     include: list[str] = ["metadatas", "documents"],
 ) -> list[dict]:
     query_res = collection.query(
         query_texts=query_text, n_results=n_results, include=include
     )
-    if n_traversal_steps == 0:
-        return [
-            {k: [v[0][i]] for k, v in query_res.items() if v is not None}
-            for i in range(n_results)
-        ]
+    # if n_traversal_steps == 0:
+    #     return [
+    #         {k: [v[0][i]] for k, v in query_res.items() if v is not None}
+    #         for i in range(n_results)
+    #     ]
     results = []
     for i, metadata in enumerate(query_res["metadatas"][0]):
         curr_id = query_res["ids"][0][i]
         prev_ids = traverse_id_tree(
             metadata=metadata,
             collection=collection,
             direction="prev",
-            n_steps=n_traversal_steps,
+            n_steps=n_prev_links,
         )
         next_ids = traverse_id_tree(
             metadata=metadata,
             collection=collection,
             direction="next",
-            n_steps=n_traversal_steps,
+            n_steps=n_next_links,
         )
         res_ids = prev_ids[::-1] + [curr_id] + next_ids
-        print(res_ids)
         results.append(collection.get(ids=res_ids, include=include))
     return results
```

### Comparing `dreamai-2.0/dreamai/pdf.py` & `dreamai-2.0.1/dreamai/pdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,24 +41,24 @@
     chunk_overlap: int = CHUNK_OVERLAP,
     separators: list[str] = SEPARATORS,
     collection_name: str = CHROMA_COLLECTION_NAME,
     persistent_dir: str = CHROMA_DIR,
     delete_existing: bool = CHROMA_DELETE_EXISTING,
     embedding_model: str = CHROMA_EMBEDDING_MODEL,
     device: str = CHROMA_DEVICE,
+    add_links: bool = True,
 ) -> ChromaCollection:
     pdf_docs = pdf_to_docs(
         pdf_file=pdf_file,
         chunk_size=chunk_size,
         chunk_overlap=chunk_overlap,
         separators=separators,
     )
     collection = chroma_collection(
         name=collection_name,
         persistent_dir=persistent_dir,
         delete_existing=delete_existing,
         embedding_model=embedding_model,
         device=device,
     )
-    ids, docs, metadatas = lc_docs_to_chroma_docs(pdf_docs)
-    collection.add(ids=ids, documents=docs, metadatas=metadatas)
+    collection.add(**lc_docs_to_chroma_docs(pdf_docs, add_links=add_links))
     return collection
```

### Comparing `dreamai-2.0/dreamai/templates.py` & `dreamai-2.0.1/dreamai/templates.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0/dreamai/utils.py` & `dreamai-2.0.1/dreamai/utils.py`

 * *Files identical despite different names*

### Comparing `dreamai-2.0/pyproject.toml` & `dreamai-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dreamai"
-version = "2.0"
+version = "2.0.1"
 description = "🔂"
 authors = ["Hamza Farhan <thehamza96@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 notebook = "^7.1.2"
```

### Comparing `dreamai-2.0/PKG-INFO` & `dreamai-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai
-Version: 2.0
+Version: 2.0.1
 Summary: 🔂
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
```

