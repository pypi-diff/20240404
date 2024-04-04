# Comparing `tmp/sentence_store-0.3.0.tar.gz` & `tmp/sentence_store-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentence_store-0.3.0.tar", last modified: Sun Mar 31 02:23:43 2024, max compression
+gzip compressed data, was "sentence_store-0.4.0.tar", last modified: Thu Apr  4 03:06:56 2024, max compression
```

## Comparing `sentence_store-0.3.0.tar` & `sentence_store-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-31 02:23:43.645073 sentence_store-0.3.0/
--rw-r--r--   0 tarau      (503) staff       (20)     1067 2024-03-22 00:56:36.000000 sentence_store-0.3.0/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)      929 2024-03-31 02:23:43.644841 sentence_store-0.3.0/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)      597 2024-03-22 02:11:02.000000 sentence_store-0.3.0/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-31 02:23:43.642747 sentence_store-0.3.0/sentence_store/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2024-03-31 02:22:12.000000 sentence_store-0.3.0/sentence_store/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     6034 2024-03-31 02:02:44.000000 sentence_store-0.3.0/sentence_store/main.py
--rw-r--r--   0 tarau      (503) staff       (20)       45 2024-03-22 21:22:17.000000 sentence_store-0.3.0/sentence_store/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      985 2024-03-22 02:08:50.000000 sentence_store-0.3.0/sentence_store/tools.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-03-31 02:23:43.644493 sentence_store-0.3.0/sentence_store.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)      929 2024-03-31 02:23:43.000000 sentence_store-0.3.0/sentence_store.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)      358 2024-03-31 02:23:43.000000 sentence_store-0.3.0/sentence_store.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-03-31 02:23:43.000000 sentence_store-0.3.0/sentence_store.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-03-31 02:23:43.000000 sentence_store-0.3.0/sentence_store.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       45 2024-03-31 02:23:43.000000 sentence_store-0.3.0/sentence_store.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)       15 2024-03-31 02:23:43.000000 sentence_store-0.3.0/sentence_store.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2024-03-31 02:23:43.645159 sentence_store-0.3.0/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      938 2024-03-22 02:06:24.000000 sentence_store-0.3.0/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:06:56.786668 sentence_store-0.4.0/
+-rw-r--r--   0 tarau      (503) staff       (20)     1067 2024-03-22 00:56:36.000000 sentence_store-0.4.0/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)      929 2024-04-04 03:06:56.786413 sentence_store-0.4.0/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)      597 2024-03-22 02:11:02.000000 sentence_store-0.4.0/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:06:56.784336 sentence_store-0.4.0/sentence_store/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-04 03:06:51.000000 sentence_store-0.4.0/sentence_store/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6661 2024-04-04 02:45:15.000000 sentence_store-0.4.0/sentence_store/main.py
+-rw-r--r--   0 tarau      (503) staff       (20)       45 2024-03-22 21:22:17.000000 sentence_store-0.4.0/sentence_store/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1009 2024-04-04 02:08:24.000000 sentence_store-0.4.0/sentence_store/tools.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:06:56.786015 sentence_store-0.4.0/sentence_store.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)      929 2024-04-04 03:06:56.000000 sentence_store-0.4.0/sentence_store.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)      358 2024-04-04 03:06:56.000000 sentence_store-0.4.0/sentence_store.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:06:56.000000 sentence_store-0.4.0/sentence_store.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:06:56.000000 sentence_store-0.4.0/sentence_store.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       45 2024-04-04 03:06:56.000000 sentence_store-0.4.0/sentence_store.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       15 2024-04-04 03:06:56.000000 sentence_store-0.4.0/sentence_store.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-04 03:06:56.786770 sentence_store-0.4.0/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      938 2024-03-22 02:06:24.000000 sentence_store-0.4.0/setup.py
```

### Comparing `sentence_store-0.3.0/LICENSE` & `sentence_store-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentence_store-0.3.0/PKG-INFO` & `sentence_store-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentence_store
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tool to extract and store sentence embeddings to a fast and scalable vector db
 Home-page: https://github.com/ptarau/sentence_store.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sentence_store-0.3.0/README.md` & `sentence_store-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sentence_store-0.3.0/sentence_store/main.py` & `sentence_store-0.4.0/sentence_store/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from sentence_store.tools import (
     to_json, from_json, exists_file, remove_file
 )
 import torch
 from sentence_transformers import SentenceTransformer
 from vecstore.vecstore import VecStore
+from sentify.main import sentify, Segmenter, sent_cleaner
 
 
 # SBERT API
 
 def seq_sbert_embed(sents, emebedding_model="all-MiniLM-L6-v2"):
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     model = SentenceTransformer(emebedding_model, device=device)
@@ -23,25 +24,26 @@
     device = 'cuda' if torch.cuda.is_available() else 'cpu'
     model = SentenceTransformer(emebedding_model, device=device)
     if device == 'cuda':
         return seq_sbert_embed(sents, emebedding_model=emebedding_model)
     num_cores = max(1, os.cpu_count() // 2 - 2)
     devices = ['cpu'] * num_cores
     pool = model.start_multi_process_pool(target_devices=devices)
-    embeddings = model.encode_multi_process(sents,pool)
+    embeddings = model.encode_multi_process(sents, pool)
     SentenceTransformer.stop_multi_process_pool(pool)
     return embeddings
 
 
-def sbert_embed(sents, emebedding_model="all-MiniLM-L6-v2",multi_cpu=False):
+def sbert_embed(sents, emebedding_model="all-MiniLM-L6-v2", multi_cpu=False):
     if multi_cpu:
         return par_cpu_sbert_embed(sents, emebedding_model=emebedding_model)
     else:
         return seq_sbert_embed(sents, emebedding_model=emebedding_model)
 
+
 class Embedder:
     """
     embeds a set of sentences using an LLM
     and store them into a vector store
     """
 
     def __init__(self, cache_name):
@@ -52,47 +54,59 @@
         self.emebedding_model = None
         self.vstore = None
         self.times = Counter()
 
     def cache(self, ending):
         return self.CACHES + self.cache_name + ending
 
-    def embed(self, sents,multi_cpu=False):
+    def embed(self, sents, multi_cpu=False):
         t1 = time()
-        embeddings = sbert_embed(sents,multi_cpu=multi_cpu)
+        embeddings = sbert_embed(sents, multi_cpu=multi_cpu)
         t2 = time()
         self.times['embed'] += t2 - t1
         return embeddings
 
     def clear(self):
         fj = self.cache('.json')
         fb = self.cache('.bin')
         remove_file(fj)
         remove_file(fb)
 
-    def store(self, sents):
+    def store(self, sents,multi_cpu=False):
         """
         embeds and caches the sentences and their embeddings
         unleass this is already done or force=True
         """
         fj = self.cache('.json')
         fb = self.cache('.bin')
         if exists_file(fj) and exists_file(fb):
             self.load()
             return
 
-        embeddings = self.embed(sents,multi_cpu=True)
+        embeddings = self.embed(sents, multi_cpu=multi_cpu)
         dim = embeddings.shape[1]
         if self.vstore is None:
             self.vstore = VecStore(fb, dim=dim)
         self.vstore.add(embeddings)
 
         to_json((dim, sents), fj)
         self.vstore.save()
 
+    def store_doc(self, doc_type, doc_name, clean=True, return_timings=False,multi_cpu=False):
+        store=self.cache('_sents.txt')
+        sents = sentify(doc_type, doc_name, clean=clean, store=None, return_timings=return_timings)
+        self.store(sents,multi_cpu=multi_cpu)
+
+    def store_text(self, text, clean=True, multi_cpu=False):
+        seg = Segmenter()
+        sents = seg.text2sents(text)
+        if clean:
+            sents = sent_cleaner(sents)
+        self.store(sents,multi_cpu=multi_cpu)
+
     def load(self):
         """
         fetches the store
         """
         fj = self.cache('.json')
         fb = self.cache(ending='.bin')
         dim, sents = from_json(fj)
@@ -102,15 +116,15 @@
 
     def knn_query(self, query_sent, top_k):
         """
         gets knns and answers matching the query
         """
         t1 = time()
         sents = self.load()
-        query_embeddings = self.embed([query_sent],multi_cpu=False)
+        query_embeddings = self.embed([query_sent], multi_cpu=False)
         t2 = time()
         self.times['query'] += t2 - t1
         knn_pairs = self.vstore.query_one(query_embeddings[0], k=top_k)
         answers = [(sents[i], r) for (i, r) in knn_pairs]
         return knn_pairs, answers
 
     def query(self, query_sent, top_k):
@@ -146,15 +160,15 @@
         "The dog barks to the moon",
         "The cat sits on the mat",
         "The phone rings",
         "The rocket explodes",
         "The cat and the dog sleep",
         "The cellphone is on the table"
     ]
-    e.store(sents)
+    e.store(sents,multi_cpu=True)
     q = 'Who sleeps on the mat?'
     rs = e(q, 2)
     for r in rs: print(r)
 
     print("\nCOMPUTING KNNS for k=3:")
 
     as_weights = False
@@ -182,23 +196,23 @@
         text = f.read().decode('utf-8')
         print('TEXT:', text[0:50], '...')
         sents = text.split('\n')
         sents = [s.strip() for s in sents if s.strip()]
         e = Embedder(cache_name='big_test')
         print('SENTS:', len(sents))
         print('COMPUTING AND STORING EMBEDDINGS')
-        e.store(sents)
+        e.store(sents,multi_cpu=True)
         print('DIMS:', e.vstore)
         print("COMPUTING KNNS for k=3:")
         print('DONE:', len(e.knns(3, as_weights=True)))
         print('QUERY WITH 3 ANSWERS:')
         rs = e('What did Napoleon say when he arrived to Moscow?', 3)
         print('RETRIEVED:\n')
         for r in rs: print(*r)
         print('\nTIMES:\n')
         for x in e.get_times().items(): print(x)
         return True
 
 
 if __name__ == "__main__":
     assert test_big()
-    #assert test_main()
+    # assert test_main()
```

### Comparing `sentence_store-0.3.0/sentence_store/tools.py` & `sentence_store-0.4.0/sentence_store/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 def exists_file(fname):
     """tests  if it exists as file or dir """
     return os.path.exists(fname)
 
 
 def remove_file(fname):
-    return os.remove(fname)
+    if exists_file(fname):
+        os.remove(fname)
 
 
 def remove_dir(dname):
     if exists_file(dname):
         shutil.rmtree(dname)
```

### Comparing `sentence_store-0.3.0/sentence_store.egg-info/PKG-INFO` & `sentence_store-0.4.0/sentence_store.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentence-store
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tool to extract and store sentence embeddings to a fast and scalable vector db
 Home-page: https://github.com/ptarau/sentence_store.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sentence_store-0.3.0/setup.py` & `sentence_store-0.4.0/setup.py`

 * *Files identical despite different names*

