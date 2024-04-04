# Comparing `tmp/rs_metrics-0.5.0.tar.gz` & `tmp/rs_metrics-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rs_metrics-0.5.0.tar", last modified: Sat May 22 11:16:46 2021, max compression
+gzip compressed data, was "dist/rs_metrics-0.5.1.tar", last modified: Thu Apr  4 13:31:54 2024, max compression
```

## Comparing `rs_metrics-0.5.0.tar` & `rs_metrics-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 ym.tamm    (501) staff       (20)        0 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/
--rw-r--r--   0 ym.tamm    (501) staff       (20)      823 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/PKG-INFO
--rw-r--r--   0 ym.tamm    (501) staff       (20)      272 2020-12-20 11:59:16.000000 rs_metrics-0.5.0/README.md
-drwxr-xr-x   0 ym.tamm    (501) staff       (20)        0 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/rs_metrics/
--rw-r--r--   0 ym.tamm    (501) staff       (20)      206 2021-05-22 11:06:53.000000 rs_metrics-0.5.0/rs_metrics/__init__.py
--rw-r--r--   0 ym.tamm    (501) staff       (20)      585 2020-12-20 11:00:29.000000 rs_metrics-0.5.0/rs_metrics/helpers.py
--rw-r--r--   0 ym.tamm    (501) staff       (20)     4838 2021-05-22 11:14:20.000000 rs_metrics-0.5.0/rs_metrics/metrics.py
--rw-r--r--   0 ym.tamm    (501) staff       (20)     1084 2021-01-13 12:27:02.000000 rs_metrics-0.5.0/rs_metrics/parallel.py
--rw-r--r--   0 ym.tamm    (501) staff       (20)      178 2020-06-30 22:21:08.000000 rs_metrics-0.5.0/rs_metrics/statistics.py
-drwxr-xr-x   0 ym.tamm    (501) staff       (20)        0 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/rs_metrics.egg-info/
--rw-r--r--   0 ym.tamm    (501) staff       (20)      823 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/rs_metrics.egg-info/PKG-INFO
--rw-r--r--   0 ym.tamm    (501) staff       (20)      302 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/rs_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 ym.tamm    (501) staff       (20)        1 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/rs_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 ym.tamm    (501) staff       (20)       13 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/rs_metrics.egg-info/requires.txt
--rw-r--r--   0 ym.tamm    (501) staff       (20)       11 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/rs_metrics.egg-info/top_level.txt
--rw-r--r--   0 ym.tamm    (501) staff       (20)       38 2021-05-22 11:16:46.000000 rs_metrics-0.5.0/setup.cfg
--rw-r--r--   0 ym.tamm    (501) staff       (20)      710 2021-05-22 11:14:20.000000 rs_metrics-0.5.0/setup.py
+drwxr-xr-x   0 ym.tamm    (501) staff       (20)        0 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/
+-rw-r--r--   0 ym.tamm    (501) staff       (20)      680 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/PKG-INFO
+-rw-r--r--   0 ym.tamm    (501) staff       (20)      272 2020-12-20 11:59:16.000000 rs_metrics-0.5.1/README.md
+drwxr-xr-x   0 ym.tamm    (501) staff       (20)        0 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/rs_metrics/
+-rw-r--r--   0 ym.tamm    (501) staff       (20)      206 2021-05-22 11:06:53.000000 rs_metrics-0.5.1/rs_metrics/__init__.py
+-rw-r--r--   0 ym.tamm    (501) staff       (20)      614 2024-04-04 13:14:04.000000 rs_metrics-0.5.1/rs_metrics/helpers.py
+-rw-r--r--   0 ym.tamm    (501) staff       (20)     5329 2024-04-03 19:00:08.000000 rs_metrics-0.5.1/rs_metrics/metrics.py
+-rw-r--r--   0 ym.tamm    (501) staff       (20)     1057 2024-04-03 18:54:52.000000 rs_metrics-0.5.1/rs_metrics/parallel.py
+-rw-r--r--   0 ym.tamm    (501) staff       (20)      178 2020-06-30 22:21:08.000000 rs_metrics-0.5.1/rs_metrics/statistics.py
+drwxr-xr-x   0 ym.tamm    (501) staff       (20)        0 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/rs_metrics.egg-info/
+-rw-r--r--   0 ym.tamm    (501) staff       (20)      680 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/rs_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 ym.tamm    (501) staff       (20)      324 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/rs_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 ym.tamm    (501) staff       (20)        1 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/rs_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 ym.tamm    (501) staff       (20)       13 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/rs_metrics.egg-info/requires.txt
+-rw-r--r--   0 ym.tamm    (501) staff       (20)       11 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/rs_metrics.egg-info/top_level.txt
+-rw-r--r--   0 ym.tamm    (501) staff       (20)       38 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/setup.cfg
+-rw-r--r--   0 ym.tamm    (501) staff       (20)      710 2024-04-04 13:16:59.000000 rs_metrics-0.5.1/setup.py
+drwxr-xr-x   0 ym.tamm    (501) staff       (20)        0 2024-04-04 13:31:54.000000 rs_metrics-0.5.1/tests/
+-rw-r--r--   0 ym.tamm    (501) staff       (20)     3038 2024-04-04 13:10:57.000000 rs_metrics-0.5.1/tests/test_metrics.py
```

### Comparing `rs_metrics-0.5.0/rs_metrics/helpers.py` & `rs_metrics-0.5.1/rs_metrics/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 
 def flatten_list(arr):
     return [item for sublist in arr for item in sublist]
 
 
 def convert_pandas(metric):
-    def wrap(true, pred, k=10, user_col='user_id', item_col='item_id'):
+    def wrap(true, pred, k=10, apply_mean=True, user_col='user_id', item_col='item_id'):
         if type(true) is pd.DataFrame:
             true = pandas_to_dict(true, user_col, item_col)
 
         if type(pred) is pd.DataFrame:
             pred = pandas_to_dict(pred, user_col, item_col)
 
-        return metric(true, pred, k)
+        return metric(true, pred, k, apply_mean)
     return wrap
```

### Comparing `rs_metrics-0.5.0/rs_metrics/metrics.py` & `rs_metrics-0.5.1/rs_metrics/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from functools import lru_cache
 
 import numpy as np
 import pandas as pd
 
 from rs_metrics.helpers import flatten_list, pandas_to_dict, convert_pandas
-from rs_metrics.parallel import user_mean, top_k, user_apply, user_mean_sub
+from rs_metrics.parallel import user_parallel, top_k, user_apply, user_mean_sub
 from rs_metrics.statistics import item_pop
 
 
 @convert_pandas
-def ndcg(true, pred, k=10):
+def ndcg(true, pred, k=10, apply_mean=True):
     """Measures ranking quality"""
-    return user_mean(_ndcg_score, true, pred, k)
+    res = user_parallel(_ndcg_score, true, pred, k)
+    res = np.mean(res) if apply_mean else res
+    return res
 
 def _ndcg_score(true, pred, k):
     true = set(true)
     gain = [item in true for item in pred]
     dcg = np.sum(gain / _discounts(len(gain)))
     return dcg / _idcg(min(len(true), k))
 
@@ -24,60 +26,71 @@
     return np.log2(np.arange(k) + 2)
 
 @lru_cache(maxsize=128)
 def _idcg(k):
     return np.sum(np.ones(k) / np.log2(np.arange(k) + 2))
 
 @convert_pandas
-def hitrate(true, pred, k=10):
+def hitrate(true, pred, k=10, apply_mean=True):
     """Shows what percentage of users has at least one relevant recommendation in their list."""
-    return user_mean(_hitrate, true, pred, k)
+    res = user_parallel(_hitrate, true, pred, k)
+    res = np.mean(res) if apply_mean else res
+    return res
 
 
 def _hitrate(true, pred, k):
     return int(np.isin(pred, true).any())
 
 
 @convert_pandas
-def precision(true, pred, k=10):
+def precision(true, pred, k=10, apply_mean=True):
     """Shows what percentage of items in recommendations are relevant, on average."""
-    return user_mean(_precision, true, pred, k)
+    res = user_parallel(_precision, true, pred, k)
+    res = np.mean(res) if apply_mean else res
+    return res
+
 
 
 def _precision(true, pred, k):
     return np.isin(pred, true).mean()
 
 
 @convert_pandas
-def recall(true, pred, k=10):
+def recall(true, pred, k=10, apply_mean=True):
     """Shows what percentage of relevant items appeared in recommendations, on average."""
-    return user_mean(_recall, true, pred, k)
+    res = user_parallel(_recall, true, pred, k)
+    res = np.mean(res) if apply_mean else res
+    return res
 
 
 def _recall(true, pred, k):
     return np.isin(true, pred).mean()
 
 
 @convert_pandas
-def mrr(true, pred, k=10):
+def mrr(true, pred, k=10, apply_mean=True):
     """Shows inverted position of the first relevant item, on average."""
-    return user_mean(_mrr, true, pred, k)
+    res = user_parallel(_mrr, true, pred, k)
+    res = np.mean(res) if apply_mean else res
+    return res
 
 
 def _mrr(true, pred, k):
     entries = np.isin(pred, true)
     if entries.any():
         return 1 / (entries.argmax() + 1)
     else:
         return 0
 
 
 @convert_pandas
-def mapr(true, pred, k=10):
-    return user_mean(_map, true, pred, k)
+def mapr(true, pred, k=10, apply_mean=True):
+    res = user_parallel(_map, true, pred, k)
+    res = np.mean(res) if apply_mean else res
+    return res
 
 
 def _map(true, pred, k):
     rel = np.isin(pred, true)
     if len(true) > 0:
         return (rel.cumsum() / np.arange(1, len(pred) + 1) * rel).sum() / len(true)
     else:
```

### Comparing `rs_metrics-0.5.0/rs_metrics/parallel.py` & `rs_metrics-0.5.1/rs_metrics/parallel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from multiprocessing import Pool, cpu_count
 import numpy as np
 
 
-def user_mean(func, true, pred, k):
+def user_parallel(func, true, pred, k):
     with Pool(cpu_count()) as p:
-        return np.mean(
-            p.starmap(func, [(true[user], pred.get(user, list())[:k], k) for user in true])
-        )
+        return p.starmap(func, [(true[user], pred.get(user, list())[:k], k) for user in true])
 
 
 
 def user_mean_sub(func, true, pred, subprofiles, k, aplha):
     pred = top_k(pred, k)
     with Pool(cpu_count()) as p:
         return np.mean(
```

### Comparing `rs_metrics-0.5.0/rs_metrics.egg-info/PKG-INFO` & `rs_metrics-0.5.1/rs_metrics.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: rs-metrics
-Version: 0.5.0
+Version: 0.5.1
 Summary: Metrics for recommender systems
 Home-page: https://github.com/darel13712/rs_metrics
 Author: Darel
 Author-email: darel142857@gmail.com
-License: UNKNOWN
-Description: ![PyPI](https://img.shields.io/pypi/v/rs_metrics?color=%2300ccff)
-        
-        This package implements metrics common in recommendation systems.
-        
-        ## Installation
-        
-        ```bash
-        pip install rs_metrics
-        ```
-        
-        ## Documentation
-        
-        Docs are available [here](https://darel13712.github.io/rs_metrics/)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+![PyPI](https://img.shields.io/pypi/v/rs_metrics?color=%2300ccff)
+
+This package implements metrics common in recommendation systems.
+
+## Installation
+
+```bash
+pip install rs_metrics
+```
+
+## Documentation
+
+Docs are available [here](https://darel13712.github.io/rs_metrics/)
```

### Comparing `rs_metrics-0.5.0/setup.py` & `rs_metrics-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rs_metrics",
-    version="0.5.0",
+    version="0.5.1",
     author="Darel",
     author_email="darel142857@gmail.com",
     description="Metrics for recommender systems",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/darel13712/rs_metrics",
     packages=setuptools.find_packages(),
```

