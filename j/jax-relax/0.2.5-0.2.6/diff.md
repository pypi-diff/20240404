# Comparing `tmp/jax-relax-0.2.5.tar.gz` & `tmp/jax-relax-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-relax-0.2.5.tar", last modified: Tue Feb 20 21:03:02 2024, max compression
+gzip compressed data, was "jax-relax-0.2.6.tar", last modified: Thu Apr  4 15:25:57 2024, max compression
```

## Comparing `jax-relax-0.2.5.tar` & `jax-relax-0.2.6.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-02-20 21:03:02.595894 jax-relax-0.2.5/
--rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-09-10 14:18:49.000000 jax-relax-0.2.5/CONTRIBUTING.md
--rw-r--r--   0 birk      (1000) birk      (1000)    11538 2023-09-10 14:18:49.000000 jax-relax-0.2.5/LICENSE
--rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-09-10 14:18:49.000000 jax-relax-0.2.5/MANIFEST.in
--rw-r--r--   0 birk      (1000) birk      (1000)     8880 2024-02-20 21:03:02.595894 jax-relax-0.2.5/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)     8099 2024-01-16 16:50:43.000000 jax-relax-0.2.5/README.md
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-02-20 21:03:02.585894 jax-relax-0.2.5/jax_relax.egg-info/
--rw-r--r--   0 birk      (1000) birk      (1000)     8880 2024-02-20 21:03:02.000000 jax-relax-0.2.5/jax_relax.egg-info/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)      956 2024-02-20 21:03:02.000000 jax-relax-0.2.5/jax_relax.egg-info/SOURCES.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2024-02-20 21:03:02.000000 jax-relax-0.2.5/jax_relax.egg-info/dependency_links.txt
--rw-r--r--   0 birk      (1000) birk      (1000)       32 2024-02-20 21:03:02.000000 jax-relax-0.2.5/jax_relax.egg-info/entry_points.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-09-10 15:15:42.000000 jax-relax-0.2.5/jax_relax.egg-info/not-zip-safe
--rw-r--r--   0 birk      (1000) birk      (1000)      206 2024-02-20 21:03:02.000000 jax-relax-0.2.5/jax_relax.egg-info/requires.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        6 2024-02-20 21:03:02.000000 jax-relax-0.2.5/jax_relax.egg-info/top_level.txt
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-02-20 21:03:02.595894 jax-relax-0.2.5/relax/
--rw-r--r--   0 birk      (1000) birk      (1000)      300 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)   103101 2024-02-20 21:01:42.000000 jax-relax-0.2.5/relax/_modidx.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2110 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/base.py
--rw-r--r--   0 birk      (1000) birk      (1000)    19570 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/data_module.py
--rw-r--r--   0 birk      (1000) birk      (1000)    23205 2024-02-20 21:01:42.000000 jax-relax-0.2.5/relax/data_utils.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7257 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/docs.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9513 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/evaluate.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9500 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/explain.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1435 2023-11-28 15:29:08.000000 jax-relax-0.2.5/relax/import_essentials.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-02-20 21:03:02.595894 jax-relax-0.2.5/relax/legacy/
--rw-r--r--   0 birk      (1000) birk      (1000)        0 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/legacy/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3895 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/legacy/ckpt_manager.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1425 2023-11-28 15:29:08.000000 jax-relax-0.2.5/relax/legacy/import_essentials.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2121 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/legacy/logger.py
--rw-r--r--   0 birk      (1000) birk      (1000)     8054 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/legacy/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     5358 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/legacy/trainer.py
--rw-r--r--   0 birk      (1000) birk      (1000)     5883 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/legacy/utils.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-02-20 21:03:02.595894 jax-relax-0.2.5/relax/methods/
--rw-r--r--   0 birk      (1000) birk      (1000)      435 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     2640 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/base.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9283 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/cchvae.py
--rw-r--r--   0 birk      (1000) birk      (1000)    10667 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/clue.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12317 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/counternet.py
--rw-r--r--   0 birk      (1000) birk      (1000)     5585 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/dice.py
--rw-r--r--   0 birk      (1000) birk      (1000)    15559 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/l2c.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7013 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/proto.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12201 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/sphere.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9542 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/vaecf.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4096 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/methods/vanilla.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7822 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/ml_model.py
--rw-r--r--   0 birk      (1000) birk      (1000)     8089 2024-02-20 20:56:01.000000 jax-relax-0.2.5/relax/strategy.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6782 2024-02-20 21:01:42.000000 jax-relax-0.2.5/relax/utils.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1131 2024-01-21 15:37:48.000000 jax-relax-0.2.5/settings.ini
--rw-r--r--   0 birk      (1000) birk      (1000)       38 2024-02-20 21:03:02.595894 jax-relax-0.2.5/setup.cfg
--rw-r--r--   0 birk      (1000) birk      (1000)     2658 2023-11-26 18:26:06.000000 jax-relax-0.2.5/setup.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/
+-rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-09-10 14:18:49.000000 jax-relax-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0 birk      (1000) birk      (1000)    11538 2023-09-10 14:18:49.000000 jax-relax-0.2.6/LICENSE
+-rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-09-10 14:18:49.000000 jax-relax-0.2.6/MANIFEST.in
+-rw-r--r--   0 birk      (1000) birk      (1000)     8880 2024-04-04 15:25:57.171337 jax-relax-0.2.6/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)     8099 2024-01-16 16:50:43.000000 jax-relax-0.2.6/README.md
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/jax_relax.egg-info/
+-rw-r--r--   0 birk      (1000) birk      (1000)     8880 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)     1059 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/SOURCES.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/dependency_links.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)       32 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/entry_points.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-09-10 15:15:42.000000 jax-relax-0.2.6/jax_relax.egg-info/not-zip-safe
+-rw-r--r--   0 birk      (1000) birk      (1000)      199 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/requires.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        6 2024-04-04 15:25:57.000000 jax-relax-0.2.6/jax_relax.egg-info/top_level.txt
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/relax/
+-rw-r--r--   0 birk      (1000) birk      (1000)      301 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)   115942 2024-04-04 15:15:48.000000 jax-relax-0.2.6/relax/_modidx.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     2110 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/base.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    19574 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_module.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/relax/data_utils/
+-rw-r--r--   0 birk      (1000) birk      (1000)       82 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_utils/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    12617 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_utils/features.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     5140 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_utils/preprocessing.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6755 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/data_utils/transforms.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7257 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/docs.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9513 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/evaluate.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9500 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/explain.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1435 2023-11-28 15:29:08.000000 jax-relax-0.2.6/relax/import_essentials.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/relax/legacy/
+-rw-r--r--   0 birk      (1000) birk      (1000)        0 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3895 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/ckpt_manager.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1425 2023-11-28 15:29:08.000000 jax-relax-0.2.6/relax/legacy/import_essentials.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     2121 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/logger.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     8054 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     5358 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/trainer.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     5883 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/legacy/utils.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2024-04-04 15:25:57.171337 jax-relax-0.2.6/relax/methods/
+-rw-r--r--   0 birk      (1000) birk      (1000)      435 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     2640 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/base.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9283 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/cchvae.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    10667 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/clue.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    12317 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/counternet.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     5585 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/dice.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    15559 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/l2c.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7013 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/proto.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    12201 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/sphere.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9542 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/vaecf.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4096 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/methods/vanilla.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7822 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/ml_model.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     8089 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/strategy.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6600 2024-04-04 15:15:35.000000 jax-relax-0.2.6/relax/utils.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1162 2024-04-03 13:49:44.000000 jax-relax-0.2.6/settings.ini
+-rw-r--r--   0 birk      (1000) birk      (1000)       38 2024-04-04 15:25:57.171337 jax-relax-0.2.6/setup.cfg
+-rw-r--r--   0 birk      (1000) birk      (1000)     2658 2023-11-26 18:26:06.000000 jax-relax-0.2.6/setup.py
```

### Comparing `jax-relax-0.2.5/CONTRIBUTING.md` & `jax-relax-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/LICENSE` & `jax-relax-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/PKG-INFO` & `jax-relax-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.2.5
+Version: 0.2.6
 Summary: JAX-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/jax-relax
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: JAX,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jax-relax-0.2.5/README.md` & `jax-relax-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/jax_relax.egg-info/PKG-INFO` & `jax-relax-0.2.6/jax_relax.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.2.5
+Version: 0.2.6
 Summary: JAX-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/jax-relax
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: JAX,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jax-relax-0.2.5/jax_relax.egg-info/SOURCES.txt` & `jax-relax-0.2.6/jax_relax.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 jax_relax.egg-info/not-zip-safe
 jax_relax.egg-info/requires.txt
 jax_relax.egg-info/top_level.txt
 relax/__init__.py
 relax/_modidx.py
 relax/base.py
 relax/data_module.py
-relax/data_utils.py
 relax/docs.py
 relax/evaluate.py
 relax/explain.py
 relax/import_essentials.py
 relax/ml_model.py
 relax/strategy.py
 relax/utils.py
+relax/data_utils/__init__.py
+relax/data_utils/features.py
+relax/data_utils/preprocessing.py
+relax/data_utils/transforms.py
 relax/legacy/__init__.py
 relax/legacy/ckpt_manager.py
 relax/legacy/import_essentials.py
 relax/legacy/logger.py
 relax/legacy/module.py
 relax/legacy/trainer.py
 relax/legacy/utils.py
```

### Comparing `jax-relax-0.2.5/relax/_modidx.py` & `jax-relax-0.2.6/relax/_modidx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,823 +1,876 @@
-# Autogenerated by nbdev
-
-d = { 'settings': { 'branch': 'master',
-                'doc_baseurl': '/jax-relax',
-                'doc_host': 'https://birkhoffg.github.io',
-                'git_url': 'https://github.com/birkhoffg/jax-relax',
-                'lib_path': 'relax'},
-  'syms': { 'relax.base': { 'relax.base.BaseConfig': ('base.html#baseconfig', 'relax/base.py'),
-                            'relax.base.BaseConfig.load_from_json': ('base.html#baseconfig.load_from_json', 'relax/base.py'),
-                            'relax.base.BaseConfig.save': ('base.html#baseconfig.save', 'relax/base.py'),
-                            'relax.base.BaseModule': ('base.html#basemodule', 'relax/base.py'),
-                            'relax.base.BaseModule.__init__': ('base.html#basemodule.__init__', 'relax/base.py'),
-                            'relax.base.BaseModule.load_from_path': ('base.html#basemodule.load_from_path', 'relax/base.py'),
-                            'relax.base.BaseModule.name': ('base.html#basemodule.name', 'relax/base.py'),
-                            'relax.base.BaseModule.save': ('base.html#basemodule.save', 'relax/base.py'),
-                            'relax.base.PredFnMixedin': ('base.html#predfnmixedin', 'relax/base.py'),
-                            'relax.base.PredFnMixedin.pred_fn': ('base.html#predfnmixedin.pred_fn', 'relax/base.py'),
-                            'relax.base.TrainableMixedin': ('base.html#trainablemixedin', 'relax/base.py'),
-                            'relax.base.TrainableMixedin.is_trained': ('base.html#trainablemixedin.is_trained', 'relax/base.py'),
-                            'relax.base.TrainableMixedin.train': ('base.html#trainablemixedin.train', 'relax/base.py')},
-            'relax.data_module': { 'relax.data_module.BaseDataModule': ('data.html#basedatamodule', 'relax/data_module.py'),
-                                   'relax.data_module.BaseDataModule._prepare': ( 'data.html#basedatamodule._prepare',
-                                                                                  'relax/data_module.py'),
-                                   'relax.data_module.BaseDataModule.apply_constraints': ( 'data.html#basedatamodule.apply_constraints',
-                                                                                           'relax/data_module.py'),
-                                   'relax.data_module.BaseDataModule.compute_reg_loss': ( 'data.html#basedatamodule.compute_reg_loss',
-                                                                                          'relax/data_module.py'),
-                                   'relax.data_module.DataModule': ('data.html#datamodule', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule.__getitem__': ('data.html#datamodule.__getitem__', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule.__init__': ('data.html#datamodule.__init__', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule._get_data': ('data.html#datamodule._get_data', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule._prepare': ('data.html#datamodule._prepare', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule.apply_constraints': ( 'data.html#datamodule.apply_constraints',
-                                                                                       'relax/data_module.py'),
-                                   'relax.data_module.DataModule.compute_reg_loss': ( 'data.html#datamodule.compute_reg_loss',
-                                                                                      'relax/data_module.py'),
-                                   'relax.data_module.DataModule.from_config': ('data.html#datamodule.from_config', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule.from_features': ( 'data.html#datamodule.from_features',
-                                                                                   'relax/data_module.py'),
-                                   'relax.data_module.DataModule.from_numpy': ('data.html#datamodule.from_numpy', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule.from_path': ('data.html#datamodule.from_path', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule.inverse_transform': ( 'data.html#datamodule.inverse_transform',
-                                                                                       'relax/data_module.py'),
-                                   'relax.data_module.DataModule.load_from_path': ( 'data.html#datamodule.load_from_path',
-                                                                                    'relax/data_module.py'),
-                                   'relax.data_module.DataModule.sample': ('data.html#datamodule.sample', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule.save': ('data.html#datamodule.save', 'relax/data_module.py'),
-                                   'relax.data_module.DataModule.set_transformations': ( 'data.html#datamodule.set_transformations',
-                                                                                         'relax/data_module.py'),
-                                   'relax.data_module.DataModule.transform': ('data.html#datamodule.transform', 'relax/data_module.py'),
-                                   'relax.data_module.DataModuleConfig': ('data.html#datamoduleconfig', 'relax/data_module.py'),
-                                   'relax.data_module.DataModuleConfig.shuffle': ( 'data.html#datamoduleconfig.shuffle',
-                                                                                   'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin': ('data.html#datamoduleinfomixin', 'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin.data': ( 'data.html#datamoduleinfomixin.data',
-                                                                                   'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin.dataset': ( 'data.html#datamoduleinfomixin.dataset',
-                                                                                      'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin.features': ( 'data.html#datamoduleinfomixin.features',
-                                                                                       'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin.label': ( 'data.html#datamoduleinfomixin.label',
-                                                                                    'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin.test_indices': ( 'data.html#datamoduleinfomixin.test_indices',
-                                                                                           'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin.train_indices': ( 'data.html#datamoduleinfomixin.train_indices',
-                                                                                            'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin.xs': ('data.html#datamoduleinfomixin.xs', 'relax/data_module.py'),
-                                   'relax.data_module.DataModuleInfoMixin.ys': ('data.html#datamoduleinfomixin.ys', 'relax/data_module.py'),
-                                   'relax.data_module.TabularDataModule': ('data.html#tabulardatamodule', 'relax/data_module.py'),
-                                   'relax.data_module.TabularDataModule.__init__': ( 'data.html#tabulardatamodule.__init__',
-                                                                                     'relax/data_module.py'),
-                                   'relax.data_module.TabularDataModuleConfigs': ( 'data.html#tabulardatamoduleconfigs',
-                                                                                   'relax/data_module.py'),
-                                   'relax.data_module.TabularDataModuleConfigs.__ini__': ( 'data.html#tabulardatamoduleconfigs.__ini__',
-                                                                                           'relax/data_module.py'),
-                                   'relax.data_module._validate_dataname': ('data.html#_validate_dataname', 'relax/data_module.py'),
-                                   'relax.data_module.dataframe2features': ('data.html#dataframe2features', 'relax/data_module.py'),
-                                   'relax.data_module.dataframe2labels': ('data.html#dataframe2labels', 'relax/data_module.py'),
-                                   'relax.data_module.dm_equals': ('data.html#dm_equals', 'relax/data_module.py'),
-                                   'relax.data_module.download_data_module_files': ( 'data.html#download_data_module_files',
-                                                                                     'relax/data_module.py'),
-                                   'relax.data_module.features2config': ('data.html#features2config', 'relax/data_module.py'),
-                                   'relax.data_module.features2pandas': ('data.html#features2pandas', 'relax/data_module.py'),
-                                   'relax.data_module.load_data': ('data.html#load_data', 'relax/data_module.py'),
-                                   'relax.data_module.to_feature': ('data.html#to_feature', 'relax/data_module.py')},
-            'relax.data_utils': { 'relax.data_utils.DataPreprocessor': ('data.utils.html#datapreprocessor', 'relax/data_utils.py'),
-                                  'relax.data_utils.DataPreprocessor.__init__': ( 'data.utils.html#datapreprocessor.__init__',
-                                                                                  'relax/data_utils.py'),
-                                  'relax.data_utils.DataPreprocessor.fit': ('data.utils.html#datapreprocessor.fit', 'relax/data_utils.py'),
-                                  'relax.data_utils.DataPreprocessor.fit_transform': ( 'data.utils.html#datapreprocessor.fit_transform',
-                                                                                       'relax/data_utils.py'),
-                                  'relax.data_utils.DataPreprocessor.from_dict': ( 'data.utils.html#datapreprocessor.from_dict',
-                                                                                   'relax/data_utils.py'),
-                                  'relax.data_utils.DataPreprocessor.inverse_transform': ( 'data.utils.html#datapreprocessor.inverse_transform',
-                                                                                           'relax/data_utils.py'),
-                                  'relax.data_utils.DataPreprocessor.to_dict': ( 'data.utils.html#datapreprocessor.to_dict',
-                                                                                 'relax/data_utils.py'),
-                                  'relax.data_utils.DataPreprocessor.transform': ( 'data.utils.html#datapreprocessor.transform',
-                                                                                   'relax/data_utils.py'),
-                                  'relax.data_utils.EncoderPreprocessor': ('data.utils.html#encoderpreprocessor', 'relax/data_utils.py'),
-                                  'relax.data_utils.EncoderPreprocessor._fit': ( 'data.utils.html#encoderpreprocessor._fit',
-                                                                                 'relax/data_utils.py'),
-                                  'relax.data_utils.EncoderPreprocessor._inverse_transform': ( 'data.utils.html#encoderpreprocessor._inverse_transform',
-                                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.EncoderPreprocessor._transform': ( 'data.utils.html#encoderpreprocessor._transform',
-                                                                                       'relax/data_utils.py'),
-                                  'relax.data_utils.EncoderPreprocessor.from_dict': ( 'data.utils.html#encoderpreprocessor.from_dict',
-                                                                                      'relax/data_utils.py'),
-                                  'relax.data_utils.EncoderPreprocessor.to_dict': ( 'data.utils.html#encoderpreprocessor.to_dict',
-                                                                                    'relax/data_utils.py'),
-                                  'relax.data_utils.Feature': ('data.utils.html#feature', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.__get_item__': ('data.utils.html#feature.__get_item__', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.__init__': ('data.utils.html#feature.__init__', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.__repr__': ('data.utils.html#feature.__repr__', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature._dispatch_transformation': ( 'data.utils.html#feature._dispatch_transformation',
-                                                                                         'relax/data_utils.py'),
-                                  'relax.data_utils.Feature._init_is_categorical': ( 'data.utils.html#feature._init_is_categorical',
-                                                                                     'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.apply_constraints': ( 'data.utils.html#feature.apply_constraints',
-                                                                                  'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.compute_reg_loss': ( 'data.utils.html#feature.compute_reg_loss',
-                                                                                 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.data': ('data.utils.html#feature.data', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.fit': ('data.utils.html#feature.fit', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.fit_transform': ( 'data.utils.html#feature.fit_transform',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.from_dict': ('data.utils.html#feature.from_dict', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.inverse_transform': ( 'data.utils.html#feature.inverse_transform',
-                                                                                  'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.is_categorical': ( 'data.utils.html#feature.is_categorical',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.is_immutable': ('data.utils.html#feature.is_immutable', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.set_transformation': ( 'data.utils.html#feature.set_transformation',
-                                                                                   'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.to_dict': ('data.utils.html#feature.to_dict', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.transform': ('data.utils.html#feature.transform', 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.transformation': ( 'data.utils.html#feature.transformation',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.transformed_data': ( 'data.utils.html#feature.transformed_data',
-                                                                                 'relax/data_utils.py'),
-                                  'relax.data_utils.Feature.with_transformed_data': ( 'data.utils.html#feature.with_transformed_data',
-                                                                                      'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList': ('data.utils.html#featureslist', 'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.__getitem__': ( 'data.utils.html#featureslist.__getitem__',
-                                                                                 'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.__init__': ( 'data.utils.html#featureslist.__init__',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.__iter__': ( 'data.utils.html#featureslist.__iter__',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.__len__': ('data.utils.html#featureslist.__len__', 'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.__next__': ( 'data.utils.html#featureslist.__next__',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList._transform_data': ( 'data.utils.html#featureslist._transform_data',
-                                                                                     'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.apply_constraints': ( 'data.utils.html#featureslist.apply_constraints',
-                                                                                       'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.compute_reg_loss': ( 'data.utils.html#featureslist.compute_reg_loss',
-                                                                                      'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.feature_indices': ( 'data.utils.html#featureslist.feature_indices',
-                                                                                     'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.feature_name_indices': ( 'data.utils.html#featureslist.feature_name_indices',
-                                                                                          'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.features': ( 'data.utils.html#featureslist.features',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.features_and_indices': ( 'data.utils.html#featureslist.features_and_indices',
-                                                                                          'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.from_dict': ( 'data.utils.html#featureslist.from_dict',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.inverse_transform': ( 'data.utils.html#featureslist.inverse_transform',
-                                                                                       'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.load_from_path': ( 'data.utils.html#featureslist.load_from_path',
-                                                                                    'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.save': ('data.utils.html#featureslist.save', 'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.set_transformations': ( 'data.utils.html#featureslist.set_transformations',
-                                                                                         'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.to_dict': ('data.utils.html#featureslist.to_dict', 'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.to_pandas': ( 'data.utils.html#featureslist.to_pandas',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.transform': ( 'data.utils.html#featureslist.transform',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.transformed_data': ( 'data.utils.html#featureslist.transformed_data',
-                                                                                      'relax/data_utils.py'),
-                                  'relax.data_utils.FeaturesList.with_transformed_data': ( 'data.utils.html#featureslist.with_transformed_data',
-                                                                                           'relax/data_utils.py'),
-                                  'relax.data_utils.GumbelSoftmaxTransformation': ( 'data.utils.html#gumbelsoftmaxtransformation',
-                                                                                    'relax/data_utils.py'),
-                                  'relax.data_utils.GumbelSoftmaxTransformation.__init__': ( 'data.utils.html#gumbelsoftmaxtransformation.__init__',
-                                                                                             'relax/data_utils.py'),
-                                  'relax.data_utils.GumbelSoftmaxTransformation.apply_constraints': ( 'data.utils.html#gumbelsoftmaxtransformation.apply_constraints',
-                                                                                                      'relax/data_utils.py'),
-                                  'relax.data_utils.GumbelSoftmaxTransformation.soft_constraints': ( 'data.utils.html#gumbelsoftmaxtransformation.soft_constraints',
-                                                                                                     'relax/data_utils.py'),
-                                  'relax.data_utils.IdentityTransformation': ( 'data.utils.html#identitytransformation',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.IdentityTransformation.__init__': ( 'data.utils.html#identitytransformation.__init__',
-                                                                                        'relax/data_utils.py'),
-                                  'relax.data_utils.IdentityTransformation.apply_constraints': ( 'data.utils.html#identitytransformation.apply_constraints',
-                                                                                                 'relax/data_utils.py'),
-                                  'relax.data_utils.IdentityTransformation.fit': ( 'data.utils.html#identitytransformation.fit',
-                                                                                   'relax/data_utils.py'),
-                                  'relax.data_utils.IdentityTransformation.fit_transform': ( 'data.utils.html#identitytransformation.fit_transform',
-                                                                                             'relax/data_utils.py'),
-                                  'relax.data_utils.IdentityTransformation.from_dict': ( 'data.utils.html#identitytransformation.from_dict',
-                                                                                         'relax/data_utils.py'),
-                                  'relax.data_utils.IdentityTransformation.to_dict': ( 'data.utils.html#identitytransformation.to_dict',
-                                                                                       'relax/data_utils.py'),
-                                  'relax.data_utils.IdentityTransformation.transform': ( 'data.utils.html#identitytransformation.transform',
-                                                                                         'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxScaler': ('data.utils.html#minmaxscaler', 'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxScaler.__init__': ( 'data.utils.html#minmaxscaler.__init__',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxScaler.fit': ('data.utils.html#minmaxscaler.fit', 'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxScaler.from_dict': ( 'data.utils.html#minmaxscaler.from_dict',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxScaler.inverse_transform': ( 'data.utils.html#minmaxscaler.inverse_transform',
-                                                                                       'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxScaler.to_dict': ('data.utils.html#minmaxscaler.to_dict', 'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxScaler.transform': ( 'data.utils.html#minmaxscaler.transform',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxTransformation': ('data.utils.html#minmaxtransformation', 'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxTransformation.__init__': ( 'data.utils.html#minmaxtransformation.__init__',
-                                                                                      'relax/data_utils.py'),
-                                  'relax.data_utils.MinMaxTransformation.apply_constraints': ( 'data.utils.html#minmaxtransformation.apply_constraints',
-                                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.OneHotEncoder': ('data.utils.html#onehotencoder', 'relax/data_utils.py'),
-                                  'relax.data_utils.OneHotEncoder.fit': ('data.utils.html#onehotencoder.fit', 'relax/data_utils.py'),
-                                  'relax.data_utils.OneHotEncoder.inverse_transform': ( 'data.utils.html#onehotencoder.inverse_transform',
-                                                                                        'relax/data_utils.py'),
-                                  'relax.data_utils.OneHotEncoder.transform': ( 'data.utils.html#onehotencoder.transform',
-                                                                                'relax/data_utils.py'),
-                                  'relax.data_utils.OneHotTransformation': ('data.utils.html#onehottransformation', 'relax/data_utils.py'),
-                                  'relax.data_utils.OrdinalPreprocessor': ('data.utils.html#ordinalpreprocessor', 'relax/data_utils.py'),
-                                  'relax.data_utils.OrdinalPreprocessor.fit': ( 'data.utils.html#ordinalpreprocessor.fit',
-                                                                                'relax/data_utils.py'),
-                                  'relax.data_utils.OrdinalPreprocessor.inverse_transform': ( 'data.utils.html#ordinalpreprocessor.inverse_transform',
-                                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.OrdinalPreprocessor.transform': ( 'data.utils.html#ordinalpreprocessor.transform',
-                                                                                      'relax/data_utils.py'),
-                                  'relax.data_utils.OrdinalTransformation': ( 'data.utils.html#ordinaltransformation',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.OrdinalTransformation.__init__': ( 'data.utils.html#ordinaltransformation.__init__',
-                                                                                       'relax/data_utils.py'),
-                                  'relax.data_utils.OrdinalTransformation.num_categories': ( 'data.utils.html#ordinaltransformation.num_categories',
-                                                                                             'relax/data_utils.py'),
-                                  'relax.data_utils.SoftmaxTransformation': ( 'data.utils.html#softmaxtransformation',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils.SoftmaxTransformation.soft_constraints': ( 'data.utils.html#softmaxtransformation.soft_constraints',
-                                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation': ('data.utils.html#transformation', 'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.__init__': ( 'data.utils.html#transformation.__init__',
-                                                                                'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.apply_constraints': ( 'data.utils.html#transformation.apply_constraints',
-                                                                                         'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.compute_reg_loss': ( 'data.utils.html#transformation.compute_reg_loss',
-                                                                                        'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.fit': ('data.utils.html#transformation.fit', 'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.fit_transform': ( 'data.utils.html#transformation.fit_transform',
-                                                                                     'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.from_dict': ( 'data.utils.html#transformation.from_dict',
-                                                                                 'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.inverse_transform': ( 'data.utils.html#transformation.inverse_transform',
-                                                                                         'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.is_categorical': ( 'data.utils.html#transformation.is_categorical',
-                                                                                      'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.to_dict': ( 'data.utils.html#transformation.to_dict',
-                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils.Transformation.transform': ( 'data.utils.html#transformation.transform',
-                                                                                 'relax/data_utils.py'),
-                                  'relax.data_utils._OneHotTransformation': ( 'data.utils.html#_onehottransformation',
-                                                                              'relax/data_utils.py'),
-                                  'relax.data_utils._OneHotTransformation.__init__': ( 'data.utils.html#_onehottransformation.__init__',
-                                                                                       'relax/data_utils.py'),
-                                  'relax.data_utils._OneHotTransformation.apply_constraints': ( 'data.utils.html#_onehottransformation.apply_constraints',
-                                                                                                'relax/data_utils.py'),
-                                  'relax.data_utils._OneHotTransformation.compute_reg_loss': ( 'data.utils.html#_onehottransformation.compute_reg_loss',
-                                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils._OneHotTransformation.hard_constraints': ( 'data.utils.html#_onehottransformation.hard_constraints',
-                                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils._OneHotTransformation.num_categories': ( 'data.utils.html#_onehottransformation.num_categories',
-                                                                                             'relax/data_utils.py'),
-                                  'relax.data_utils._OneHotTransformation.soft_constraints': ( 'data.utils.html#_onehottransformation.soft_constraints',
-                                                                                               'relax/data_utils.py'),
-                                  'relax.data_utils._check_xs': ('data.utils.html#_check_xs', 'relax/data_utils.py'),
-                                  'relax.data_utils._unique': ('data.utils.html#_unique', 'relax/data_utils.py')},
-            'relax.docs': { 'relax.docs.CustomizedMarkdownRenderer': ('docs.html#customizedmarkdownrenderer', 'relax/docs.py'),
-                            'relax.docs.CustomizedMarkdownRenderer.__init__': ( 'docs.html#customizedmarkdownrenderer.__init__',
-                                                                                'relax/docs.py'),
-                            'relax.docs.CustomizedMarkdownRenderer._check_sym': ( 'docs.html#customizedmarkdownrenderer._check_sym',
-                                                                                  'relax/docs.py'),
-                            'relax.docs.CustomizedMarkdownRenderer._repr_markdown_': ( 'docs.html#customizedmarkdownrenderer._repr_markdown_',
-                                                                                       'relax/docs.py'),
-                            'relax.docs.CustomizedMarkdownRenderer.hook_methods': ( 'docs.html#customizedmarkdownrenderer.hook_methods',
-                                                                                    'relax/docs.py'),
-                            'relax.docs.ListDocment': ('docs.html#listdocment', 'relax/docs.py'),
-                            'relax.docs.ListDocment.__init__': ('docs.html#listdocment.__init__', 'relax/docs.py'),
-                            'relax.docs.ListDocment._repre_mardown': ('docs.html#listdocment._repre_mardown', 'relax/docs.py'),
-                            'relax.docs.ParserMarkdownRenderer': ('docs.html#parsermarkdownrenderer', 'relax/docs.py'),
-                            'relax.docs.ParserMarkdownRenderer.__init__': ('docs.html#parsermarkdownrenderer.__init__', 'relax/docs.py'),
-                            'relax.docs._bold': ('docs.html#_bold', 'relax/docs.py'),
-                            'relax.docs._docment_parser': ('docs.html#_docment_parser', 'relax/docs.py'),
-                            'relax.docs._fmt_sig': ('docs.html#_fmt_sig', 'relax/docs.py'),
-                            'relax.docs._inner_list2mdlist': ('docs.html#_inner_list2mdlist', 'relax/docs.py'),
-                            'relax.docs._italic': ('docs.html#_italic', 'relax/docs.py'),
-                            'relax.docs._params_mdlist': ('docs.html#_params_mdlist', 'relax/docs.py'),
-                            'relax.docs._repr_markdown': ('docs.html#_repr_markdown', 'relax/docs.py'),
-                            'relax.docs._return_mdlist': ('docs.html#_return_mdlist', 'relax/docs.py'),
-                            'relax.docs._show_param': ('docs.html#_show_param', 'relax/docs.py'),
-                            'relax.docs._show_params_return': ('docs.html#_show_params_return', 'relax/docs.py')},
-            'relax.evaluate': { 'relax.evaluate.BaseEvalMetrics': ('evaluate.html#baseevalmetrics', 'relax/evaluate.py'),
-                                'relax.evaluate.BaseEvalMetrics.__call__': ('evaluate.html#baseevalmetrics.__call__', 'relax/evaluate.py'),
-                                'relax.evaluate.BaseEvalMetrics.__init__': ('evaluate.html#baseevalmetrics.__init__', 'relax/evaluate.py'),
-                                'relax.evaluate.BaseEvalMetrics.__str__': ('evaluate.html#baseevalmetrics.__str__', 'relax/evaluate.py'),
-                                'relax.evaluate.ManifoldDist': ('evaluate.html#manifolddist', 'relax/evaluate.py'),
-                                'relax.evaluate.ManifoldDist.__call__': ('evaluate.html#manifolddist.__call__', 'relax/evaluate.py'),
-                                'relax.evaluate.ManifoldDist.__init__': ('evaluate.html#manifolddist.__init__', 'relax/evaluate.py'),
-                                'relax.evaluate.PredictiveAccuracy': ('evaluate.html#predictiveaccuracy', 'relax/evaluate.py'),
-                                'relax.evaluate.PredictiveAccuracy.__call__': ( 'evaluate.html#predictiveaccuracy.__call__',
-                                                                                'relax/evaluate.py'),
-                                'relax.evaluate.PredictiveAccuracy.__init__': ( 'evaluate.html#predictiveaccuracy.__init__',
-                                                                                'relax/evaluate.py'),
-                                'relax.evaluate.Proximity': ('evaluate.html#proximity', 'relax/evaluate.py'),
-                                'relax.evaluate.Proximity.__call__': ('evaluate.html#proximity.__call__', 'relax/evaluate.py'),
-                                'relax.evaluate.Proximity.__init__': ('evaluate.html#proximity.__init__', 'relax/evaluate.py'),
-                                'relax.evaluate.Runtime': ('evaluate.html#runtime', 'relax/evaluate.py'),
-                                'relax.evaluate.Runtime.__call__': ('evaluate.html#runtime.__call__', 'relax/evaluate.py'),
-                                'relax.evaluate.Runtime.__init__': ('evaluate.html#runtime.__init__', 'relax/evaluate.py'),
-                                'relax.evaluate.Sparsity': ('evaluate.html#sparsity', 'relax/evaluate.py'),
-                                'relax.evaluate.Sparsity.__call__': ('evaluate.html#sparsity.__call__', 'relax/evaluate.py'),
-                                'relax.evaluate.Sparsity.__init__': ('evaluate.html#sparsity.__init__', 'relax/evaluate.py'),
-                                'relax.evaluate.Validity': ('evaluate.html#validity', 'relax/evaluate.py'),
-                                'relax.evaluate.Validity.__call__': ('evaluate.html#validity.__call__', 'relax/evaluate.py'),
-                                'relax.evaluate.Validity.__init__': ('evaluate.html#validity.__init__', 'relax/evaluate.py'),
-                                'relax.evaluate._get_metric': ('evaluate.html#_get_metric', 'relax/evaluate.py'),
-                                'relax.evaluate.benchmark_cfs': ('evaluate.html#benchmark_cfs', 'relax/evaluate.py'),
-                                'relax.evaluate.compute_proximity': ('evaluate.html#compute_proximity', 'relax/evaluate.py'),
-                                'relax.evaluate.compute_single_proximity': ('evaluate.html#compute_single_proximity', 'relax/evaluate.py'),
-                                'relax.evaluate.compute_single_sparsity': ('evaluate.html#compute_single_sparsity', 'relax/evaluate.py'),
-                                'relax.evaluate.compute_single_validity': ('evaluate.html#compute_single_validity', 'relax/evaluate.py'),
-                                'relax.evaluate.compute_sparsity': ('evaluate.html#compute_sparsity', 'relax/evaluate.py'),
-                                'relax.evaluate.compute_validity': ('evaluate.html#compute_validity', 'relax/evaluate.py'),
-                                'relax.evaluate.evaluate_cfs': ('evaluate.html#evaluate_cfs', 'relax/evaluate.py'),
-                                'relax.evaluate.l2_ann': ('evaluate.html#l2_ann', 'relax/evaluate.py'),
-                                'relax.evaluate.pairwise_distances': ('evaluate.html#pairwise_distances', 'relax/evaluate.py')},
-            'relax.explain': { 'relax.explain.Explanation': ('explain.html#explanation', 'relax/explain.py'),
-                               'relax.explain.Explanation.__getitem__': ('explain.html#explanation.__getitem__', 'relax/explain.py'),
-                               'relax.explain.Explanation.__init__': ('explain.html#explanation.__init__', 'relax/explain.py'),
-                               'relax.explain.Explanation.__repr__': ('explain.html#explanation.__repr__', 'relax/explain.py'),
-                               'relax.explain.Explanation.cfs': ('explain.html#explanation.cfs', 'relax/explain.py'),
-                               'relax.explain.Explanation.copy': ('explain.html#explanation.copy', 'relax/explain.py'),
-                               'relax.explain.Explanation.data_name': ('explain.html#explanation.data_name', 'relax/explain.py'),
-                               'relax.explain.Explanation.feature_indices': ( 'explain.html#explanation.feature_indices',
-                                                                              'relax/explain.py'),
-                               'relax.explain.Explanation.features_and_indices': ( 'explain.html#explanation.features_and_indices',
-                                                                                   'relax/explain.py'),
-                               'relax.explain.Explanation.load_from_path': ('explain.html#explanation.load_from_path', 'relax/explain.py'),
-                               'relax.explain.Explanation.save': ('explain.html#explanation.save', 'relax/explain.py'),
-                               'relax.explain.fake_explanation': ('explain.html#fake_explanation', 'relax/explain.py'),
-                               'relax.explain.generate_cf_explanations': ('explain.html#generate_cf_explanations', 'relax/explain.py'),
-                               'relax.explain.prepare_cf_module': ('explain.html#prepare_cf_module', 'relax/explain.py'),
-                               'relax.explain.prepare_pred_fn': ('explain.html#prepare_pred_fn', 'relax/explain.py'),
-                               'relax.explain.prepare_rng_keys': ('explain.html#prepare_rng_keys', 'relax/explain.py')},
-            'relax.import_essentials': {},
-            'relax.legacy.ckpt_manager': { 'relax.legacy.ckpt_manager.CheckpointManager': ( 'legacy/ckpt_manager.html#checkpointmanager',
-                                                                                            'relax/legacy/ckpt_manager.py'),
-                                           'relax.legacy.ckpt_manager.CheckpointManager.__init__': ( 'legacy/ckpt_manager.html#checkpointmanager.__init__',
-                                                                                                     'relax/legacy/ckpt_manager.py'),
-                                           'relax.legacy.ckpt_manager.CheckpointManager.delete_net_opt': ( 'legacy/ckpt_manager.html#checkpointmanager.delete_net_opt',
-                                                                                                           'relax/legacy/ckpt_manager.py'),
-                                           'relax.legacy.ckpt_manager.CheckpointManager.save_net_opt': ( 'legacy/ckpt_manager.html#checkpointmanager.save_net_opt',
-                                                                                                         'relax/legacy/ckpt_manager.py'),
-                                           'relax.legacy.ckpt_manager.CheckpointManager.update_checkpoints': ( 'legacy/ckpt_manager.html#checkpointmanager.update_checkpoints',
-                                                                                                               'relax/legacy/ckpt_manager.py'),
-                                           'relax.legacy.ckpt_manager.load_checkpoint': ( 'legacy/ckpt_manager.html#load_checkpoint',
-                                                                                          'relax/legacy/ckpt_manager.py'),
-                                           'relax.legacy.ckpt_manager.save_checkpoint': ( 'legacy/ckpt_manager.html#save_checkpoint',
-                                                                                          'relax/legacy/ckpt_manager.py')},
-            'relax.legacy.import_essentials': {},
-            'relax.legacy.logger': { 'relax.legacy.logger.Logger': ('legacy/logger.html#logger', 'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.__init__': ( 'legacy/logger.html#logger.__init__',
-                                                                              'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.close': ('legacy/logger.html#logger.close', 'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.get_last_logs': ( 'legacy/logger.html#logger.get_last_logs',
-                                                                                   'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.log': ('legacy/logger.html#logger.log', 'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.log_dict': ( 'legacy/logger.html#logger.log_dict',
-                                                                              'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.log_dir': ('legacy/logger.html#logger.log_dir', 'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.on_epoch_finished': ( 'legacy/logger.html#logger.on_epoch_finished',
-                                                                                       'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.on_epoch_started': ( 'legacy/logger.html#logger.on_epoch_started',
-                                                                                      'relax/legacy/logger.py'),
-                                     'relax.legacy.logger.Logger.save_hyperparams': ( 'legacy/logger.html#logger.save_hyperparams',
-                                                                                      'relax/legacy/logger.py')},
-            'relax.legacy.module': { 'relax.legacy.module.BaseNetwork': ('legacy/module.html#basenetwork', 'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseNetwork.__call__': ( 'legacy/module.html#basenetwork.__call__',
-                                                                                   'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseTrainingModule': ( 'legacy/module.html#basetrainingmodule',
-                                                                                 'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseTrainingModule.init_logger': ( 'legacy/module.html#basetrainingmodule.init_logger',
-                                                                                             'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseTrainingModule.init_net_opt': ( 'legacy/module.html#basetrainingmodule.init_net_opt',
-                                                                                              'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseTrainingModule.log': ( 'legacy/module.html#basetrainingmodule.log',
-                                                                                     'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseTrainingModule.log_dict': ( 'legacy/module.html#basetrainingmodule.log_dict',
-                                                                                          'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseTrainingModule.save_hyperparameters': ( 'legacy/module.html#basetrainingmodule.save_hyperparameters',
-                                                                                                      'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseTrainingModule.training_step': ( 'legacy/module.html#basetrainingmodule.training_step',
-                                                                                               'relax/legacy/module.py'),
-                                     'relax.legacy.module.BaseTrainingModule.validation_step': ( 'legacy/module.html#basetrainingmodule.validation_step',
-                                                                                                 'relax/legacy/module.py'),
-                                     'relax.legacy.module.DenseBlock': ('legacy/module.html#denseblock', 'relax/legacy/module.py'),
-                                     'relax.legacy.module.DenseBlock.__call__': ( 'legacy/module.html#denseblock.__call__',
-                                                                                  'relax/legacy/module.py'),
-                                     'relax.legacy.module.DenseBlock.__init__': ( 'legacy/module.html#denseblock.__init__',
-                                                                                  'relax/legacy/module.py'),
-                                     'relax.legacy.module.MLP': ('legacy/module.html#mlp', 'relax/legacy/module.py'),
-                                     'relax.legacy.module.MLP.__call__': ('legacy/module.html#mlp.__call__', 'relax/legacy/module.py'),
-                                     'relax.legacy.module.MLP.__init__': ('legacy/module.html#mlp.__init__', 'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveModel': ( 'legacy/module.html#predictivemodel',
-                                                                              'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveModel.__call__': ( 'legacy/module.html#predictivemodel.__call__',
-                                                                                       'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveModel.__init__': ( 'legacy/module.html#predictivemodel.__init__',
-                                                                                       'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveModelConfigs': ( 'legacy/module.html#predictivemodelconfigs',
-                                                                                     'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule': ( 'legacy/module.html#predictivetrainingmodule',
-                                                                                       'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule.__init__': ( 'legacy/module.html#predictivetrainingmodule.__init__',
-                                                                                                'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule._training_step': ( 'legacy/module.html#predictivetrainingmodule._training_step',
-                                                                                                      'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule.forward': ( 'legacy/module.html#predictivetrainingmodule.forward',
-                                                                                               'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule.init_net_opt': ( 'legacy/module.html#predictivetrainingmodule.init_net_opt',
-                                                                                                    'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule.loss_fn': ( 'legacy/module.html#predictivetrainingmodule.loss_fn',
-                                                                                               'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule.pred_fn': ( 'legacy/module.html#predictivetrainingmodule.pred_fn',
-                                                                                               'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule.training_step': ( 'legacy/module.html#predictivetrainingmodule.training_step',
-                                                                                                     'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModule.validation_step': ( 'legacy/module.html#predictivetrainingmodule.validation_step',
-                                                                                                       'relax/legacy/module.py'),
-                                     'relax.legacy.module.PredictiveTrainingModuleConfigs': ( 'legacy/module.html#predictivetrainingmoduleconfigs',
-                                                                                              'relax/legacy/module.py')},
-            'relax.legacy.trainer': { 'relax.legacy.trainer.TrainingConfigs': ( 'legacy/trainer.html#trainingconfigs',
-                                                                                'relax/legacy/trainer.py'),
-                                      'relax.legacy.trainer.TrainingConfigs.PRNGSequence': ( 'legacy/trainer.html#trainingconfigs.prngsequence',
-                                                                                             'relax/legacy/trainer.py'),
-                                      'relax.legacy.trainer.train_model': ('legacy/trainer.html#train_model', 'relax/legacy/trainer.py'),
-                                      'relax.legacy.trainer.train_model_with_states': ( 'legacy/trainer.html#train_model_with_states',
-                                                                                        'relax/legacy/trainer.py')},
-            'relax.legacy.utils': { 'relax.legacy.utils.Config': ('legacy/utils.html#config', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.Config.default': ('legacy/utils.html#config.default', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.accuracy': ('legacy/utils.html#accuracy', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.binary_cross_entropy': ( 'legacy/utils.html#binary_cross_entropy',
-                                                                                 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.cat_normalize': ('legacy/utils.html#cat_normalize', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.check_cat_info': ('legacy/utils.html#check_cat_info', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.dist': ('legacy/utils.html#dist', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.get_config': ('legacy/utils.html#get_config', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.grad_update': ('legacy/utils.html#grad_update', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.init_net_opt': ('legacy/utils.html#init_net_opt', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.load_json': ('legacy/utils.html#load_json', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.make_hk_module': ('legacy/utils.html#make_hk_module', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.make_model': ('legacy/utils.html#make_model', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.proximity': ('legacy/utils.html#proximity', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.sigmoid': ('legacy/utils.html#sigmoid', 'relax/legacy/utils.py'),
-                                    'relax.legacy.utils.validate_configs': ('legacy/utils.html#validate_configs', 'relax/legacy/utils.py')},
-            'relax.methods.base': { 'relax.methods.base.CFModule': ('methods/base.html#cfmodule', 'relax/methods/base.py'),
-                                    'relax.methods.base.CFModule.__init__': ( 'methods/base.html#cfmodule.__init__',
-                                                                              'relax/methods/base.py'),
-                                    'relax.methods.base.CFModule.apply_constraints': ( 'methods/base.html#cfmodule.apply_constraints',
-                                                                                       'relax/methods/base.py'),
-                                    'relax.methods.base.CFModule.before_generate_cf': ( 'methods/base.html#cfmodule.before_generate_cf',
-                                                                                        'relax/methods/base.py'),
-                                    'relax.methods.base.CFModule.compute_reg_loss': ( 'methods/base.html#cfmodule.compute_reg_loss',
-                                                                                      'relax/methods/base.py'),
-                                    'relax.methods.base.CFModule.generate_cf': ( 'methods/base.html#cfmodule.generate_cf',
-                                                                                 'relax/methods/base.py'),
-                                    'relax.methods.base.CFModule.set_apply_constraints_fn': ( 'methods/base.html#cfmodule.set_apply_constraints_fn',
-                                                                                              'relax/methods/base.py'),
-                                    'relax.methods.base.CFModule.set_compute_reg_loss_fn': ( 'methods/base.html#cfmodule.set_compute_reg_loss_fn',
-                                                                                             'relax/methods/base.py'),
-                                    'relax.methods.base.CFModule.set_data_module': ( 'methods/base.html#cfmodule.set_data_module',
-                                                                                     'relax/methods/base.py'),
-                                    'relax.methods.base.ParametricCFModule': ( 'methods/base.html#parametriccfmodule',
-                                                                               'relax/methods/base.py'),
-                                    'relax.methods.base.ParametricCFModule.train': ( 'methods/base.html#parametriccfmodule.train',
-                                                                                     'relax/methods/base.py'),
-                                    'relax.methods.base.default_apply_constraints_fn': ( 'methods/base.html#default_apply_constraints_fn',
-                                                                                         'relax/methods/base.py'),
-                                    'relax.methods.base.default_compute_reg_loss_fn': ( 'methods/base.html#default_compute_reg_loss_fn',
-                                                                                        'relax/methods/base.py')},
-            'relax.methods.cchvae': { 'relax.methods.cchvae.CCHVAE': ('methods/cchvae.html#cchvae', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CCHVAE.__init__': ( 'methods/cchvae.html#cchvae.__init__',
-                                                                                'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CCHVAE._init_model': ( 'methods/cchvae.html#cchvae._init_model',
-                                                                                   'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CCHVAE.generate_cf': ( 'methods/cchvae.html#cchvae.generate_cf',
-                                                                                   'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CCHVAE.train': ('methods/cchvae.html#cchvae.train', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CCHVAEConfig': ('methods/cchvae.html#cchvaeconfig', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE': ('methods/cchvae.html#chvae', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.__init__': ( 'methods/cchvae.html#chvae.__init__',
-                                                                               'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.build': ('methods/cchvae.html#chvae.build', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.call': ('methods/cchvae.html#chvae.call', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.compute_kl_loss': ( 'methods/cchvae.html#chvae.compute_kl_loss',
-                                                                                      'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.decode': ('methods/cchvae.html#chvae.decode', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.encode': ('methods/cchvae.html#chvae.encode', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.forward': ( 'methods/cchvae.html#chvae.forward',
-                                                                              'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.regenerate': ( 'methods/cchvae.html#chvae.regenerate',
-                                                                                 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.reparameterize': ( 'methods/cchvae.html#chvae.reparameterize',
-                                                                                     'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae.CHVAE.set_apply_constraints_fn': ( 'methods/cchvae.html#chvae.set_apply_constraints_fn',
-                                                                                               'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae._cchvae': ('methods/cchvae.html#_cchvae', 'relax/methods/cchvae.py'),
-                                      'relax.methods.cchvae._hyper_sphere_coordindates': ( 'methods/cchvae.html#_hyper_sphere_coordindates',
-                                                                                           'relax/methods/cchvae.py')},
-            'relax.methods.clue': { 'relax.methods.clue.CLUE': ('methods/clue.html#clue', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.CLUE.__init__': ('methods/clue.html#clue.__init__', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.CLUE._init_model': ('methods/clue.html#clue._init_model', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.CLUE.generate_cf': ('methods/clue.html#clue.generate_cf', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.CLUE.train': ('methods/clue.html#clue.train', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.CLUEConfig': ('methods/clue.html#clueconfig', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.Decoder': ('methods/clue.html#decoder', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.Decoder.__call__': ('methods/clue.html#decoder.__call__', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.Decoder.__init__': ('methods/clue.html#decoder.__init__', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.Encoder': ('methods/clue.html#encoder', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.Encoder.__init__': ('methods/clue.html#encoder.__init__', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.Encoder.call': ('methods/clue.html#encoder.call', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat': ('methods/clue.html#vaegausscat', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.__init__': ( 'methods/clue.html#vaegausscat.__init__',
-                                                                                 'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.build': ( 'methods/clue.html#vaegausscat.build',
-                                                                              'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.call': ('methods/clue.html#vaegausscat.call', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.compute_vae_loss': ( 'methods/clue.html#vaegausscat.compute_vae_loss',
-                                                                                         'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.decode': ( 'methods/clue.html#vaegausscat.decode',
-                                                                               'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.encode': ( 'methods/clue.html#vaegausscat.encode',
-                                                                               'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.sample': ( 'methods/clue.html#vaegausscat.sample',
-                                                                               'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.sample_latent': ( 'methods/clue.html#vaegausscat.sample_latent',
-                                                                                      'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.sample_step': ( 'methods/clue.html#vaegausscat.sample_step',
-                                                                                    'relax/methods/clue.py'),
-                                    'relax.methods.clue.VAEGaussCat.set_reconstruction_loss': ( 'methods/clue.html#vaegausscat.set_reconstruction_loss',
-                                                                                                'relax/methods/clue.py'),
-                                    'relax.methods.clue._clue_generate': ('methods/clue.html#_clue_generate', 'relax/methods/clue.py'),
-                                    'relax.methods.clue.get_reconstruction_loss_fn': ( 'methods/clue.html#get_reconstruction_loss_fn',
-                                                                                       'relax/methods/clue.py'),
-                                    'relax.methods.clue.kl_divergence': ('methods/clue.html#kl_divergence', 'relax/methods/clue.py')},
-            'relax.methods.counternet': { 'relax.methods.counternet.CounterNet': ( 'methods/counternet.html#counternet',
-                                                                                   'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.__init__': ( 'methods/counternet.html#counternet.__init__',
-                                                                                            'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet._init_model': ( 'methods/counternet.html#counternet._init_model',
-                                                                                               'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.generate_cf': ( 'methods/counternet.html#counternet.generate_cf',
-                                                                                               'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.is_trained': ( 'methods/counternet.html#counternet.is_trained',
-                                                                                              'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.pred_fn': ( 'methods/counternet.html#counternet.pred_fn',
-                                                                                           'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNet.train': ( 'methods/counternet.html#counternet.train',
-                                                                                         'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetConfig': ( 'methods/counternet.html#counternetconfig',
-                                                                                         'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetModel': ( 'methods/counternet.html#counternetmodel',
-                                                                                        'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetModel.__call__': ( 'methods/counternet.html#counternetmodel.__call__',
-                                                                                                 'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetModel.__init__': ( 'methods/counternet.html#counternetmodel.__init__',
-                                                                                                 'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule': ( 'methods/counternet.html#counternettrainingmodule',
-                                                                                                 'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.__init__': ( 'methods/counternet.html#counternettrainingmodule.__init__',
-                                                                                                          'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule._explainer_step': ( 'methods/counternet.html#counternettrainingmodule._explainer_step',
-                                                                                                                 'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule._predictor_step': ( 'methods/counternet.html#counternettrainingmodule._predictor_step',
-                                                                                                                 'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule._training_step': ( 'methods/counternet.html#counternettrainingmodule._training_step',
-                                                                                                                'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule._training_step_logs': ( 'methods/counternet.html#counternettrainingmodule._training_step_logs',
-                                                                                                                     'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.exp_loss_fn': ( 'methods/counternet.html#counternettrainingmodule.exp_loss_fn',
-                                                                                                             'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.forward': ( 'methods/counternet.html#counternettrainingmodule.forward',
-                                                                                                         'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.generate_cf': ( 'methods/counternet.html#counternettrainingmodule.generate_cf',
-                                                                                                             'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.init_net_opt': ( 'methods/counternet.html#counternettrainingmodule.init_net_opt',
-                                                                                                              'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_1': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_1',
-                                                                                                           'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_2': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_2',
-                                                                                                           'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_3': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_3',
-                                                                                                           'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.pred_fn': ( 'methods/counternet.html#counternettrainingmodule.pred_fn',
-                                                                                                         'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.pred_loss_fn': ( 'methods/counternet.html#counternettrainingmodule.pred_loss_fn',
-                                                                                                              'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.training_step': ( 'methods/counternet.html#counternettrainingmodule.training_step',
-                                                                                                               'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.CounterNetTrainingModule.validation_step': ( 'methods/counternet.html#counternettrainingmodule.validation_step',
-                                                                                                                 'relax/methods/counternet.py'),
-                                          'relax.methods.counternet.partition_trainable_params': ( 'methods/counternet.html#partition_trainable_params',
-                                                                                                   'relax/methods/counternet.py')},
-            'relax.methods.dice': { 'relax.methods.dice.DiverseCF': ('methods/dice.html#diversecf', 'relax/methods/dice.py'),
-                                    'relax.methods.dice.DiverseCF.__init__': ( 'methods/dice.html#diversecf.__init__',
-                                                                               'relax/methods/dice.py'),
-                                    'relax.methods.dice.DiverseCF.generate_cf': ( 'methods/dice.html#diversecf.generate_cf',
-                                                                                  'relax/methods/dice.py'),
-                                    'relax.methods.dice.DiverseCF.load_from_path': ( 'methods/dice.html#diversecf.load_from_path',
-                                                                                     'relax/methods/dice.py'),
-                                    'relax.methods.dice.DiverseCF.save': ('methods/dice.html#diversecf.save', 'relax/methods/dice.py'),
-                                    'relax.methods.dice.DiverseCFConfig': ('methods/dice.html#diversecfconfig', 'relax/methods/dice.py'),
-                                    'relax.methods.dice._diverse_cf': ('methods/dice.html#_diverse_cf', 'relax/methods/dice.py'),
-                                    'relax.methods.dice.dpp_style_vmap': ('methods/dice.html#dpp_style_vmap', 'relax/methods/dice.py')},
-            'relax.methods.l2c': { 'relax.methods.l2c.Discretizer': ('methods/l2c.html#discretizer', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.__init__': ( 'methods/l2c.html#discretizer.__init__',
-                                                                               'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.fit': ('methods/l2c.html#discretizer.fit', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.fit_transform': ( 'methods/l2c.html#discretizer.fit_transform',
-                                                                                    'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.get_pred_fn': ( 'methods/l2c.html#discretizer.get_pred_fn',
-                                                                                  'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.inverse_transform': ( 'methods/l2c.html#discretizer.inverse_transform',
-                                                                                        'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.inverse_transform_indices': ( 'methods/l2c.html#discretizer.inverse_transform_indices',
-                                                                                                'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.inversed_transform_pytree': ( 'methods/l2c.html#discretizer.inversed_transform_pytree',
-                                                                                                'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.transform': ( 'methods/l2c.html#discretizer.transform',
-                                                                                'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.Discretizer.transform_indices': ( 'methods/l2c.html#discretizer.transform_indices',
-                                                                                        'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2C': ('methods/l2c.html#l2c', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2C.__init__': ('methods/l2c.html#l2c.__init__', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2C.generate_cf': ('methods/l2c.html#l2c.generate_cf', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2C.train': ('methods/l2c.html#l2c.train', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CConfig': ('methods/l2c.html#l2cconfig', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel': ('methods/l2c.html#l2cmodel', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.__init__': ('methods/l2c.html#l2cmodel.__init__', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.build': ('methods/l2c.html#l2cmodel.build', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.call': ('methods/l2c.html#l2cmodel.call', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.compute_l2c_loss': ( 'methods/l2c.html#l2cmodel.compute_l2c_loss',
-                                                                                    'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.forward': ('methods/l2c.html#l2cmodel.forward', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.set_features_info': ( 'methods/l2c.html#l2cmodel.set_features_info',
-                                                                                     'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.set_immutable_mask': ( 'methods/l2c.html#l2cmodel.set_immutable_mask',
-                                                                                      'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.set_pred_fn': ( 'methods/l2c.html#l2cmodel.set_pred_fn',
-                                                                               'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.L2CModel.start_end_indices': ( 'methods/l2c.html#l2cmodel.start_end_indices',
-                                                                                     'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.cut_quantiles': ('methods/l2c.html#cut_quantiles', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.discretize_xs': ('methods/l2c.html#discretize_xs', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.gumbel_softmax': ('methods/l2c.html#gumbel_softmax', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.qcut': ('methods/l2c.html#qcut', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.qcut_inverse': ('methods/l2c.html#qcut_inverse', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.sample_bernouli': ('methods/l2c.html#sample_bernouli', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.sample_categorical': ('methods/l2c.html#sample_categorical', 'relax/methods/l2c.py'),
-                                   'relax.methods.l2c.split_fn': ('methods/l2c.html#split_fn', 'relax/methods/l2c.py')},
-            'relax.methods.proto': { 'relax.methods.proto.ProtoCF': ('methods/proto.html#protocf', 'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF.__init__': ( 'methods/proto.html#protocf.__init__',
-                                                                               'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF._init_model': ( 'methods/proto.html#protocf._init_model',
-                                                                                  'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF.generate_cf': ( 'methods/proto.html#protocf.generate_cf',
-                                                                                  'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCF.train': ('methods/proto.html#protocf.train', 'relax/methods/proto.py'),
-                                     'relax.methods.proto.ProtoCFConfig': ('methods/proto.html#protocfconfig', 'relax/methods/proto.py'),
-                                     'relax.methods.proto._proto_cf': ('methods/proto.html#_proto_cf', 'relax/methods/proto.py')},
-            'relax.methods.sphere': { 'relax.methods.sphere.GSConfig': ('methods/sphere.html#gsconfig', 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere': ( 'methods/sphere.html#growingsphere',
-                                                                              'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.__init__': ( 'methods/sphere.html#growingsphere.__init__',
-                                                                                       'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.before_generate_cf': ( 'methods/sphere.html#growingsphere.before_generate_cf',
-                                                                                                 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.generate_cf': ( 'methods/sphere.html#growingsphere.generate_cf',
-                                                                                          'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.has_data_module': ( 'methods/sphere.html#growingsphere.has_data_module',
-                                                                                              'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.load_from_path': ( 'methods/sphere.html#growingsphere.load_from_path',
-                                                                                             'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.GrowingSphere.save': ( 'methods/sphere.html#growingsphere.save',
-                                                                                   'relax/methods/sphere.py'),
-                                      'relax.methods.sphere._growing_spheres': ( 'methods/sphere.html#_growing_spheres',
-                                                                                 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.cat_perturb_fn': ( 'methods/sphere.html#cat_perturb_fn',
-                                                                               'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.default_perturb_function': ( 'methods/sphere.html#default_perturb_function',
-                                                                                         'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.features_to_infos_and_perturb_fn': ( 'methods/sphere.html#features_to_infos_and_perturb_fn',
-                                                                                                 'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.hyper_sphere_coordindates': ( 'methods/sphere.html#hyper_sphere_coordindates',
-                                                                                          'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.perturb_function_with_features': ( 'methods/sphere.html#perturb_function_with_features',
-                                                                                               'relax/methods/sphere.py'),
-                                      'relax.methods.sphere.sample_categorical': ( 'methods/sphere.html#sample_categorical',
-                                                                                   'relax/methods/sphere.py')},
-            'relax.methods.vaecf': { 'relax.methods.vaecf.VAE': ('methods/vaecf.html#vae', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.__init__': ('methods/vaecf.html#vae.__init__', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE._compile': ('methods/vaecf.html#vae._compile', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.build': ('methods/vaecf.html#vae.build', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.call': ('methods/vaecf.html#vae.call', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.compute_vae_loss': ( 'methods/vaecf.html#vae.compute_vae_loss',
-                                                                                   'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.decode': ('methods/vaecf.html#vae.decode', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.encode': ('methods/vaecf.html#vae.encode', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.sample': ('methods/vaecf.html#vae.sample', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.set_compute_regularization_fn': ( 'methods/vaecf.html#vae.set_compute_regularization_fn',
-                                                                                                'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAE.set_pred_fn': ( 'methods/vaecf.html#vae.set_pred_fn',
-                                                                              'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAECF': ('methods/vaecf.html#vaecf', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAECF.__init__': ('methods/vaecf.html#vaecf.__init__', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAECF._init_model': ( 'methods/vaecf.html#vaecf._init_model',
-                                                                                'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAECF.generate_cf': ( 'methods/vaecf.html#vaecf.generate_cf',
-                                                                                'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAECF.train': ('methods/vaecf.html#vaecf.train', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.VAECFConfig': ('methods/vaecf.html#vaecfconfig', 'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.hindge_embedding_loss': ( 'methods/vaecf.html#hindge_embedding_loss',
-                                                                                    'relax/methods/vaecf.py'),
-                                     'relax.methods.vaecf.sample_latent': ('methods/vaecf.html#sample_latent', 'relax/methods/vaecf.py')},
-            'relax.methods.vanilla': { 'relax.methods.vanilla.VanillaCF': ('methods/vanilla.html#vanillacf', 'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCF.__init__': ( 'methods/vanilla.html#vanillacf.__init__',
-                                                                                     'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCF.generate_cf': ( 'methods/vanilla.html#vanillacf.generate_cf',
-                                                                                        'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCF.load_from_path': ( 'methods/vanilla.html#vanillacf.load_from_path',
-                                                                                           'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCF.save': ( 'methods/vanilla.html#vanillacf.save',
-                                                                                 'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla.VanillaCFConfig': ( 'methods/vanilla.html#vanillacfconfig',
-                                                                                  'relax/methods/vanilla.py'),
-                                       'relax.methods.vanilla._vanilla_cf': ( 'methods/vanilla.html#_vanilla_cf',
-                                                                              'relax/methods/vanilla.py')},
-            'relax.ml_model': { 'relax.ml_model.AutoEncoder': ('ml_model.html#autoencoder', 'relax/ml_model.py'),
-                                'relax.ml_model.AutoEncoder.__init__': ('ml_model.html#autoencoder.__init__', 'relax/ml_model.py'),
-                                'relax.ml_model.AutoEncoder.call': ('ml_model.html#autoencoder.call', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModule': ('ml_model.html#mlmodule', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModule.__init__': ('ml_model.html#mlmodule.__init__', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModule._init_model': ('ml_model.html#mlmodule._init_model', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModule.is_trained': ('ml_model.html#mlmodule.is_trained', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModule.load_from_path': ('ml_model.html#mlmodule.load_from_path', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModule.pred_fn': ('ml_model.html#mlmodule.pred_fn', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModule.save': ('ml_model.html#mlmodule.save', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModule.train': ('ml_model.html#mlmodule.train', 'relax/ml_model.py'),
-                                'relax.ml_model.MLModuleConfig': ('ml_model.html#mlmoduleconfig', 'relax/ml_model.py'),
-                                'relax.ml_model.MLP': ('ml_model.html#mlp', 'relax/ml_model.py'),
-                                'relax.ml_model.MLP.__init__': ('ml_model.html#mlp.__init__', 'relax/ml_model.py'),
-                                'relax.ml_model.MLP.call': ('ml_model.html#mlp.call', 'relax/ml_model.py'),
-                                'relax.ml_model.MLP.get_config': ('ml_model.html#mlp.get_config', 'relax/ml_model.py'),
-                                'relax.ml_model.MLPBlock': ('ml_model.html#mlpblock', 'relax/ml_model.py'),
-                                'relax.ml_model.MLPBlock.__init__': ('ml_model.html#mlpblock.__init__', 'relax/ml_model.py'),
-                                'relax.ml_model.MLPBlock.build': ('ml_model.html#mlpblock.build', 'relax/ml_model.py'),
-                                'relax.ml_model.MLPBlock.call': ('ml_model.html#mlpblock.call', 'relax/ml_model.py'),
-                                'relax.ml_model.download_ml_module': ('ml_model.html#download_ml_module', 'relax/ml_model.py'),
-                                'relax.ml_model.load_ml_module': ('ml_model.html#load_ml_module', 'relax/ml_model.py')},
-            'relax.strategy': { 'relax.strategy.BaseStrategy': ('explain.strategy.html#basestrategy', 'relax/strategy.py'),
-                                'relax.strategy.BaseStrategy.__call__': ( 'explain.strategy.html#basestrategy.__call__',
-                                                                          'relax/strategy.py'),
-                                'relax.strategy.BatchedPmapStrategy': ('explain.strategy.html#batchedpmapstrategy', 'relax/strategy.py'),
-                                'relax.strategy.BatchedPmapStrategy.__call__': ( 'explain.strategy.html#batchedpmapstrategy.__call__',
-                                                                                 'relax/strategy.py'),
-                                'relax.strategy.BatchedPmapStrategy.__init__': ( 'explain.strategy.html#batchedpmapstrategy.__init__',
-                                                                                 'relax/strategy.py'),
-                                'relax.strategy.BatchedVmapStrategy': ('explain.strategy.html#batchedvmapstrategy', 'relax/strategy.py'),
-                                'relax.strategy.BatchedVmapStrategy.__call__': ( 'explain.strategy.html#batchedvmapstrategy.__call__',
-                                                                                 'relax/strategy.py'),
-                                'relax.strategy.BatchedVmapStrategy.__init__': ( 'explain.strategy.html#batchedvmapstrategy.__init__',
-                                                                                 'relax/strategy.py'),
-                                'relax.strategy.IterativeStrategy': ('explain.strategy.html#iterativestrategy', 'relax/strategy.py'),
-                                'relax.strategy.IterativeStrategy.__call__': ( 'explain.strategy.html#iterativestrategy.__call__',
-                                                                               'relax/strategy.py'),
-                                'relax.strategy.PmapStrategy': ('explain.strategy.html#pmapstrategy', 'relax/strategy.py'),
-                                'relax.strategy.PmapStrategy.__call__': ( 'explain.strategy.html#pmapstrategy.__call__',
-                                                                          'relax/strategy.py'),
-                                'relax.strategy.PmapStrategy.__init__': ( 'explain.strategy.html#pmapstrategy.__init__',
-                                                                          'relax/strategy.py'),
-                                'relax.strategy.StrategyFactory': ('explain.strategy.html#strategyfactory', 'relax/strategy.py'),
-                                'relax.strategy.StrategyFactory.__init__': ( 'explain.strategy.html#strategyfactory.__init__',
-                                                                             'relax/strategy.py'),
-                                'relax.strategy.StrategyFactory.get_default_strategy': ( 'explain.strategy.html#strategyfactory.get_default_strategy',
-                                                                                         'relax/strategy.py'),
-                                'relax.strategy.StrategyFactory.get_strategy': ( 'explain.strategy.html#strategyfactory.get_strategy',
-                                                                                 'relax/strategy.py'),
-                                'relax.strategy.VmapStrategy': ('explain.strategy.html#vmapstrategy', 'relax/strategy.py'),
-                                'relax.strategy.VmapStrategy.__call__': ( 'explain.strategy.html#vmapstrategy.__call__',
-                                                                          'relax/strategy.py'),
-                                'relax.strategy._batched_generation': ('explain.strategy.html#_batched_generation', 'relax/strategy.py'),
-                                'relax.strategy._pad_divisible_X': ('explain.strategy.html#_pad_divisible_x', 'relax/strategy.py'),
-                                'relax.strategy._pad_xs': ('explain.strategy.html#_pad_xs', 'relax/strategy.py')},
-            'relax.utils': { 'relax.utils.Config': ('utils.html#config', 'relax/utils.py'),
-                             'relax.utils.Config.default': ('utils.html#config.default', 'relax/utils.py'),
-                             'relax.utils._is_array': ('utils.html#_is_array', 'relax/utils.py'),
-                             'relax.utils._reshape_x': ('utils.html#_reshape_x', 'relax/utils.py'),
-                             'relax.utils.auto_reshaping': ('utils.html#auto_reshaping', 'relax/utils.py'),
-                             'relax.utils.get_config': ('utils.html#get_config', 'relax/utils.py'),
-                             'relax.utils.grad_update': ('utils.html#grad_update', 'relax/utils.py'),
-                             'relax.utils.gumbel_softmax': ('utils.html#gumbel_softmax', 'relax/utils.py'),
-                             'relax.utils.load_json': ('utils.html#load_json', 'relax/utils.py'),
-                             'relax.utils.load_pytree': ('utils.html#load_pytree', 'relax/utils.py'),
-                             'relax.utils.save_pytree': ('utils.html#save_pytree', 'relax/utils.py'),
-                             'relax.utils.set_config': ('utils.html#set_config', 'relax/utils.py'),
-                             'relax.utils.validate_configs': ('utils.html#validate_configs', 'relax/utils.py')}}}
+# Autogenerated by nbdev
+
+d = { 'settings': { 'branch': 'master',
+                'doc_baseurl': '/jax-relax',
+                'doc_host': 'https://birkhoffg.github.io',
+                'git_url': 'https://github.com/birkhoffg/jax-relax',
+                'lib_path': 'relax'},
+  'syms': { 'relax.base': { 'relax.base.BaseConfig': ('base.html#baseconfig', 'relax/base.py'),
+                            'relax.base.BaseConfig.load_from_json': ('base.html#baseconfig.load_from_json', 'relax/base.py'),
+                            'relax.base.BaseConfig.save': ('base.html#baseconfig.save', 'relax/base.py'),
+                            'relax.base.BaseModule': ('base.html#basemodule', 'relax/base.py'),
+                            'relax.base.BaseModule.__init__': ('base.html#basemodule.__init__', 'relax/base.py'),
+                            'relax.base.BaseModule.load_from_path': ('base.html#basemodule.load_from_path', 'relax/base.py'),
+                            'relax.base.BaseModule.name': ('base.html#basemodule.name', 'relax/base.py'),
+                            'relax.base.BaseModule.save': ('base.html#basemodule.save', 'relax/base.py'),
+                            'relax.base.PredFnMixedin': ('base.html#predfnmixedin', 'relax/base.py'),
+                            'relax.base.PredFnMixedin.pred_fn': ('base.html#predfnmixedin.pred_fn', 'relax/base.py'),
+                            'relax.base.TrainableMixedin': ('base.html#trainablemixedin', 'relax/base.py'),
+                            'relax.base.TrainableMixedin.is_trained': ('base.html#trainablemixedin.is_trained', 'relax/base.py'),
+                            'relax.base.TrainableMixedin.train': ('base.html#trainablemixedin.train', 'relax/base.py')},
+            'relax.data_module': { 'relax.data_module.BaseDataModule': ('data.html#basedatamodule', 'relax/data_module.py'),
+                                   'relax.data_module.BaseDataModule._prepare': ( 'data.html#basedatamodule._prepare',
+                                                                                  'relax/data_module.py'),
+                                   'relax.data_module.BaseDataModule.apply_constraints': ( 'data.html#basedatamodule.apply_constraints',
+                                                                                           'relax/data_module.py'),
+                                   'relax.data_module.BaseDataModule.compute_reg_loss': ( 'data.html#basedatamodule.compute_reg_loss',
+                                                                                          'relax/data_module.py'),
+                                   'relax.data_module.DataModule': ('data.html#datamodule', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule.__getitem__': ('data.html#datamodule.__getitem__', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule.__init__': ('data.html#datamodule.__init__', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule._get_data': ('data.html#datamodule._get_data', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule._prepare': ('data.html#datamodule._prepare', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule.apply_constraints': ( 'data.html#datamodule.apply_constraints',
+                                                                                       'relax/data_module.py'),
+                                   'relax.data_module.DataModule.compute_reg_loss': ( 'data.html#datamodule.compute_reg_loss',
+                                                                                      'relax/data_module.py'),
+                                   'relax.data_module.DataModule.from_config': ('data.html#datamodule.from_config', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule.from_features': ( 'data.html#datamodule.from_features',
+                                                                                   'relax/data_module.py'),
+                                   'relax.data_module.DataModule.from_numpy': ('data.html#datamodule.from_numpy', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule.from_path': ('data.html#datamodule.from_path', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule.inverse_transform': ( 'data.html#datamodule.inverse_transform',
+                                                                                       'relax/data_module.py'),
+                                   'relax.data_module.DataModule.load_from_path': ( 'data.html#datamodule.load_from_path',
+                                                                                    'relax/data_module.py'),
+                                   'relax.data_module.DataModule.sample': ('data.html#datamodule.sample', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule.save': ('data.html#datamodule.save', 'relax/data_module.py'),
+                                   'relax.data_module.DataModule.set_transformations': ( 'data.html#datamodule.set_transformations',
+                                                                                         'relax/data_module.py'),
+                                   'relax.data_module.DataModule.transform': ('data.html#datamodule.transform', 'relax/data_module.py'),
+                                   'relax.data_module.DataModuleConfig': ('data.html#datamoduleconfig', 'relax/data_module.py'),
+                                   'relax.data_module.DataModuleConfig.shuffle': ( 'data.html#datamoduleconfig.shuffle',
+                                                                                   'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin': ('data.html#datamoduleinfomixin', 'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin.data': ( 'data.html#datamoduleinfomixin.data',
+                                                                                   'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin.dataset': ( 'data.html#datamoduleinfomixin.dataset',
+                                                                                      'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin.features': ( 'data.html#datamoduleinfomixin.features',
+                                                                                       'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin.label': ( 'data.html#datamoduleinfomixin.label',
+                                                                                    'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin.test_indices': ( 'data.html#datamoduleinfomixin.test_indices',
+                                                                                           'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin.train_indices': ( 'data.html#datamoduleinfomixin.train_indices',
+                                                                                            'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin.xs': ('data.html#datamoduleinfomixin.xs', 'relax/data_module.py'),
+                                   'relax.data_module.DataModuleInfoMixin.ys': ('data.html#datamoduleinfomixin.ys', 'relax/data_module.py'),
+                                   'relax.data_module.TabularDataModule': ('data.html#tabulardatamodule', 'relax/data_module.py'),
+                                   'relax.data_module.TabularDataModule.__init__': ( 'data.html#tabulardatamodule.__init__',
+                                                                                     'relax/data_module.py'),
+                                   'relax.data_module.TabularDataModuleConfigs': ( 'data.html#tabulardatamoduleconfigs',
+                                                                                   'relax/data_module.py'),
+                                   'relax.data_module.TabularDataModuleConfigs.__ini__': ( 'data.html#tabulardatamoduleconfigs.__ini__',
+                                                                                           'relax/data_module.py'),
+                                   'relax.data_module._validate_dataname': ('data.html#_validate_dataname', 'relax/data_module.py'),
+                                   'relax.data_module.dataframe2features': ('data.html#dataframe2features', 'relax/data_module.py'),
+                                   'relax.data_module.dataframe2labels': ('data.html#dataframe2labels', 'relax/data_module.py'),
+                                   'relax.data_module.dm_equals': ('data.html#dm_equals', 'relax/data_module.py'),
+                                   'relax.data_module.download_data_module_files': ( 'data.html#download_data_module_files',
+                                                                                     'relax/data_module.py'),
+                                   'relax.data_module.features2config': ('data.html#features2config', 'relax/data_module.py'),
+                                   'relax.data_module.features2pandas': ('data.html#features2pandas', 'relax/data_module.py'),
+                                   'relax.data_module.load_data': ('data.html#load_data', 'relax/data_module.py'),
+                                   'relax.data_module.to_feature': ('data.html#to_feature', 'relax/data_module.py')},
+            'relax.data_utils.features': { 'relax.data_utils.features.Feature': ( 'data_utils/features.html#feature',
+                                                                                  'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.__get_item__': ( 'data_utils/features.html#feature.__get_item__',
+                                                                                               'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.__init__': ( 'data_utils/features.html#feature.__init__',
+                                                                                           'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.__repr__': ( 'data_utils/features.html#feature.__repr__',
+                                                                                           'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature._dispatch_transformation': ( 'data_utils/features.html#feature._dispatch_transformation',
+                                                                                                           'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature._init_is_categorical': ( 'data_utils/features.html#feature._init_is_categorical',
+                                                                                                       'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.apply_constraints': ( 'data_utils/features.html#feature.apply_constraints',
+                                                                                                    'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.compute_reg_loss': ( 'data_utils/features.html#feature.compute_reg_loss',
+                                                                                                   'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.data': ( 'data_utils/features.html#feature.data',
+                                                                                       'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.fit': ( 'data_utils/features.html#feature.fit',
+                                                                                      'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.fit_transform': ( 'data_utils/features.html#feature.fit_transform',
+                                                                                                'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.from_dict': ( 'data_utils/features.html#feature.from_dict',
+                                                                                            'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.inverse_transform': ( 'data_utils/features.html#feature.inverse_transform',
+                                                                                                    'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.is_categorical': ( 'data_utils/features.html#feature.is_categorical',
+                                                                                                 'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.is_immutable': ( 'data_utils/features.html#feature.is_immutable',
+                                                                                               'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.set_transformation': ( 'data_utils/features.html#feature.set_transformation',
+                                                                                                     'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.to_dict': ( 'data_utils/features.html#feature.to_dict',
+                                                                                          'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.transform': ( 'data_utils/features.html#feature.transform',
+                                                                                            'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.transformation': ( 'data_utils/features.html#feature.transformation',
+                                                                                                 'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.transformed_data': ( 'data_utils/features.html#feature.transformed_data',
+                                                                                                   'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.Feature.with_transformed_data': ( 'data_utils/features.html#feature.with_transformed_data',
+                                                                                                        'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList': ( 'data_utils/features.html#featureslist',
+                                                                                       'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.__getitem__': ( 'data_utils/features.html#featureslist.__getitem__',
+                                                                                                   'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.__init__': ( 'data_utils/features.html#featureslist.__init__',
+                                                                                                'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.__iter__': ( 'data_utils/features.html#featureslist.__iter__',
+                                                                                                'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.__len__': ( 'data_utils/features.html#featureslist.__len__',
+                                                                                               'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.__next__': ( 'data_utils/features.html#featureslist.__next__',
+                                                                                                'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList._transform_data': ( 'data_utils/features.html#featureslist._transform_data',
+                                                                                                       'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.apply_constraints': ( 'data_utils/features.html#featureslist.apply_constraints',
+                                                                                                         'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.compute_reg_loss': ( 'data_utils/features.html#featureslist.compute_reg_loss',
+                                                                                                        'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.feature_indices': ( 'data_utils/features.html#featureslist.feature_indices',
+                                                                                                       'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.feature_name_indices': ( 'data_utils/features.html#featureslist.feature_name_indices',
+                                                                                                            'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.features': ( 'data_utils/features.html#featureslist.features',
+                                                                                                'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.features_and_indices': ( 'data_utils/features.html#featureslist.features_and_indices',
+                                                                                                            'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.from_dict': ( 'data_utils/features.html#featureslist.from_dict',
+                                                                                                 'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.inverse_transform': ( 'data_utils/features.html#featureslist.inverse_transform',
+                                                                                                         'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.load_from_path': ( 'data_utils/features.html#featureslist.load_from_path',
+                                                                                                      'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.save': ( 'data_utils/features.html#featureslist.save',
+                                                                                            'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.set_transformations': ( 'data_utils/features.html#featureslist.set_transformations',
+                                                                                                           'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.to_dict': ( 'data_utils/features.html#featureslist.to_dict',
+                                                                                               'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.to_pandas': ( 'data_utils/features.html#featureslist.to_pandas',
+                                                                                                 'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.transform': ( 'data_utils/features.html#featureslist.transform',
+                                                                                                 'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.transformed_data': ( 'data_utils/features.html#featureslist.transformed_data',
+                                                                                                        'relax/data_utils/features.py'),
+                                           'relax.data_utils.features.FeaturesList.with_transformed_data': ( 'data_utils/features.html#featureslist.with_transformed_data',
+                                                                                                             'relax/data_utils/features.py')},
+            'relax.data_utils.preprocessing': { 'relax.data_utils.preprocessing.DataPreprocessor': ( 'data_utils/preprocessing.html#datapreprocessor',
+                                                                                                     'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.DataPreprocessor.__init__': ( 'data_utils/preprocessing.html#datapreprocessor.__init__',
+                                                                                                              'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.DataPreprocessor.fit': ( 'data_utils/preprocessing.html#datapreprocessor.fit',
+                                                                                                         'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.DataPreprocessor.fit_transform': ( 'data_utils/preprocessing.html#datapreprocessor.fit_transform',
+                                                                                                                   'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.DataPreprocessor.from_dict': ( 'data_utils/preprocessing.html#datapreprocessor.from_dict',
+                                                                                                               'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.DataPreprocessor.inverse_transform': ( 'data_utils/preprocessing.html#datapreprocessor.inverse_transform',
+                                                                                                                       'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.DataPreprocessor.to_dict': ( 'data_utils/preprocessing.html#datapreprocessor.to_dict',
+                                                                                                             'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.DataPreprocessor.transform': ( 'data_utils/preprocessing.html#datapreprocessor.transform',
+                                                                                                               'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.EncoderPreprocessor': ( 'data_utils/preprocessing.html#encoderpreprocessor',
+                                                                                                        'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.EncoderPreprocessor._fit': ( 'data_utils/preprocessing.html#encoderpreprocessor._fit',
+                                                                                                             'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.EncoderPreprocessor._inverse_transform': ( 'data_utils/preprocessing.html#encoderpreprocessor._inverse_transform',
+                                                                                                                           'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.EncoderPreprocessor._transform': ( 'data_utils/preprocessing.html#encoderpreprocessor._transform',
+                                                                                                                   'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.EncoderPreprocessor.from_dict': ( 'data_utils/preprocessing.html#encoderpreprocessor.from_dict',
+                                                                                                                  'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.EncoderPreprocessor.to_dict': ( 'data_utils/preprocessing.html#encoderpreprocessor.to_dict',
+                                                                                                                'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.MinMaxScaler': ( 'data_utils/preprocessing.html#minmaxscaler',
+                                                                                                 'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.MinMaxScaler.__init__': ( 'data_utils/preprocessing.html#minmaxscaler.__init__',
+                                                                                                          'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.MinMaxScaler.fit': ( 'data_utils/preprocessing.html#minmaxscaler.fit',
+                                                                                                     'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.MinMaxScaler.from_dict': ( 'data_utils/preprocessing.html#minmaxscaler.from_dict',
+                                                                                                           'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.MinMaxScaler.inverse_transform': ( 'data_utils/preprocessing.html#minmaxscaler.inverse_transform',
+                                                                                                                   'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.MinMaxScaler.to_dict': ( 'data_utils/preprocessing.html#minmaxscaler.to_dict',
+                                                                                                         'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.MinMaxScaler.transform': ( 'data_utils/preprocessing.html#minmaxscaler.transform',
+                                                                                                           'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.OneHotEncoder': ( 'data_utils/preprocessing.html#onehotencoder',
+                                                                                                  'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.OneHotEncoder.fit': ( 'data_utils/preprocessing.html#onehotencoder.fit',
+                                                                                                      'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.OneHotEncoder.inverse_transform': ( 'data_utils/preprocessing.html#onehotencoder.inverse_transform',
+                                                                                                                    'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.OneHotEncoder.transform': ( 'data_utils/preprocessing.html#onehotencoder.transform',
+                                                                                                            'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.OrdinalPreprocessor': ( 'data_utils/preprocessing.html#ordinalpreprocessor',
+                                                                                                        'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.OrdinalPreprocessor.fit': ( 'data_utils/preprocessing.html#ordinalpreprocessor.fit',
+                                                                                                            'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.OrdinalPreprocessor.inverse_transform': ( 'data_utils/preprocessing.html#ordinalpreprocessor.inverse_transform',
+                                                                                                                          'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing.OrdinalPreprocessor.transform': ( 'data_utils/preprocessing.html#ordinalpreprocessor.transform',
+                                                                                                                  'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing._check_xs': ( 'data_utils/preprocessing.html#_check_xs',
+                                                                                              'relax/data_utils/preprocessing.py'),
+                                                'relax.data_utils.preprocessing._unique': ( 'data_utils/preprocessing.html#_unique',
+                                                                                            'relax/data_utils/preprocessing.py')},
+            'relax.data_utils.transforms': { 'relax.data_utils.transforms.BaseTransformation': ( 'data_utils/transform.html#basetransformation',
+                                                                                                 'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.__init__': ( 'data_utils/transform.html#basetransformation.__init__',
+                                                                                                          'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.apply_constraints': ( 'data_utils/transform.html#basetransformation.apply_constraints',
+                                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.compute_reg_loss': ( 'data_utils/transform.html#basetransformation.compute_reg_loss',
+                                                                                                                  'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.fit': ( 'data_utils/transform.html#basetransformation.fit',
+                                                                                                     'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.fit_transform': ( 'data_utils/transform.html#basetransformation.fit_transform',
+                                                                                                               'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.from_dict': ( 'data_utils/transform.html#basetransformation.from_dict',
+                                                                                                           'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.inverse_transform': ( 'data_utils/transform.html#basetransformation.inverse_transform',
+                                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.is_categorical': ( 'data_utils/transform.html#basetransformation.is_categorical',
+                                                                                                                'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.to_dict': ( 'data_utils/transform.html#basetransformation.to_dict',
+                                                                                                         'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.BaseTransformation.transform': ( 'data_utils/transform.html#basetransformation.transform',
+                                                                                                           'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.GumbelSoftmaxTransformation': ( 'data_utils/transform.html#gumbelsoftmaxtransformation',
+                                                                                                          'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.GumbelSoftmaxTransformation.__init__': ( 'data_utils/transform.html#gumbelsoftmaxtransformation.__init__',
+                                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.GumbelSoftmaxTransformation.apply_constraints': ( 'data_utils/transform.html#gumbelsoftmaxtransformation.apply_constraints',
+                                                                                                                            'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.GumbelSoftmaxTransformation.soft_constraints': ( 'data_utils/transform.html#gumbelsoftmaxtransformation.soft_constraints',
+                                                                                                                           'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.GumbelSoftmaxTransformation.to_dict': ( 'data_utils/transform.html#gumbelsoftmaxtransformation.to_dict',
+                                                                                                                  'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.IdentityTransformation': ( 'data_utils/transform.html#identitytransformation',
+                                                                                                     'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.IdentityTransformation.__init__': ( 'data_utils/transform.html#identitytransformation.__init__',
+                                                                                                              'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.IdentityTransformation.apply_constraints': ( 'data_utils/transform.html#identitytransformation.apply_constraints',
+                                                                                                                       'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.IdentityTransformation.fit': ( 'data_utils/transform.html#identitytransformation.fit',
+                                                                                                         'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.IdentityTransformation.fit_transform': ( 'data_utils/transform.html#identitytransformation.fit_transform',
+                                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.IdentityTransformation.from_dict': ( 'data_utils/transform.html#identitytransformation.from_dict',
+                                                                                                               'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.IdentityTransformation.to_dict': ( 'data_utils/transform.html#identitytransformation.to_dict',
+                                                                                                             'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.IdentityTransformation.transform': ( 'data_utils/transform.html#identitytransformation.transform',
+                                                                                                               'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.MinMaxTransformation': ( 'data_utils/transform.html#minmaxtransformation',
+                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.MinMaxTransformation.__init__': ( 'data_utils/transform.html#minmaxtransformation.__init__',
+                                                                                                            'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.MinMaxTransformation.apply_constraints': ( 'data_utils/transform.html#minmaxtransformation.apply_constraints',
+                                                                                                                     'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.OneHotTransformation': ( 'data_utils/transform.html#onehottransformation',
+                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.OrdinalTransformation': ( 'data_utils/transform.html#ordinaltransformation',
+                                                                                                    'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.OrdinalTransformation.__init__': ( 'data_utils/transform.html#ordinaltransformation.__init__',
+                                                                                                             'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.OrdinalTransformation.num_categories': ( 'data_utils/transform.html#ordinaltransformation.num_categories',
+                                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.SoftmaxTransformation': ( 'data_utils/transform.html#softmaxtransformation',
+                                                                                                    'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.SoftmaxTransformation.__init__': ( 'data_utils/transform.html#softmaxtransformation.__init__',
+                                                                                                             'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms.SoftmaxTransformation.soft_constraints': ( 'data_utils/transform.html#softmaxtransformation.soft_constraints',
+                                                                                                                     'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation': ( 'data_utils/transform.html#_defaulttransformation',
+                                                                                                     'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.apply_constraints': ( 'data_utils/transform.html#_defaulttransformation.apply_constraints',
+                                                                                                                       'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.compute_reg_loss': ( 'data_utils/transform.html#_defaulttransformation.compute_reg_loss',
+                                                                                                                      'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.fit': ( 'data_utils/transform.html#_defaulttransformation.fit',
+                                                                                                         'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.fit_transform': ( 'data_utils/transform.html#_defaulttransformation.fit_transform',
+                                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.from_dict': ( 'data_utils/transform.html#_defaulttransformation.from_dict',
+                                                                                                               'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.inverse_transform': ( 'data_utils/transform.html#_defaulttransformation.inverse_transform',
+                                                                                                                       'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.is_categorical': ( 'data_utils/transform.html#_defaulttransformation.is_categorical',
+                                                                                                                    'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.to_dict': ( 'data_utils/transform.html#_defaulttransformation.to_dict',
+                                                                                                             'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._DefaultTransformation.transform': ( 'data_utils/transform.html#_defaulttransformation.transform',
+                                                                                                               'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._OneHotTransformation': ( 'data_utils/transform.html#_onehottransformation',
+                                                                                                    'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._OneHotTransformation.__init__': ( 'data_utils/transform.html#_onehottransformation.__init__',
+                                                                                                             'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._OneHotTransformation.apply_constraints': ( 'data_utils/transform.html#_onehottransformation.apply_constraints',
+                                                                                                                      'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._OneHotTransformation.compute_reg_loss': ( 'data_utils/transform.html#_onehottransformation.compute_reg_loss',
+                                                                                                                     'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._OneHotTransformation.hard_constraints': ( 'data_utils/transform.html#_onehottransformation.hard_constraints',
+                                                                                                                     'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._OneHotTransformation.num_categories': ( 'data_utils/transform.html#_onehottransformation.num_categories',
+                                                                                                                   'relax/data_utils/transforms.py'),
+                                             'relax.data_utils.transforms._OneHotTransformation.soft_constraints': ( 'data_utils/transform.html#_onehottransformation.soft_constraints',
+                                                                                                                     'relax/data_utils/transforms.py')},
+            'relax.docs': { 'relax.docs.CustomizedMarkdownRenderer': ('docs.html#customizedmarkdownrenderer', 'relax/docs.py'),
+                            'relax.docs.CustomizedMarkdownRenderer.__init__': ( 'docs.html#customizedmarkdownrenderer.__init__',
+                                                                                'relax/docs.py'),
+                            'relax.docs.CustomizedMarkdownRenderer._check_sym': ( 'docs.html#customizedmarkdownrenderer._check_sym',
+                                                                                  'relax/docs.py'),
+                            'relax.docs.CustomizedMarkdownRenderer._repr_markdown_': ( 'docs.html#customizedmarkdownrenderer._repr_markdown_',
+                                                                                       'relax/docs.py'),
+                            'relax.docs.CustomizedMarkdownRenderer.hook_methods': ( 'docs.html#customizedmarkdownrenderer.hook_methods',
+                                                                                    'relax/docs.py'),
+                            'relax.docs.ListDocment': ('docs.html#listdocment', 'relax/docs.py'),
+                            'relax.docs.ListDocment.__init__': ('docs.html#listdocment.__init__', 'relax/docs.py'),
+                            'relax.docs.ListDocment._repre_mardown': ('docs.html#listdocment._repre_mardown', 'relax/docs.py'),
+                            'relax.docs.ParserMarkdownRenderer': ('docs.html#parsermarkdownrenderer', 'relax/docs.py'),
+                            'relax.docs.ParserMarkdownRenderer.__init__': ('docs.html#parsermarkdownrenderer.__init__', 'relax/docs.py'),
+                            'relax.docs._bold': ('docs.html#_bold', 'relax/docs.py'),
+                            'relax.docs._docment_parser': ('docs.html#_docment_parser', 'relax/docs.py'),
+                            'relax.docs._fmt_sig': ('docs.html#_fmt_sig', 'relax/docs.py'),
+                            'relax.docs._inner_list2mdlist': ('docs.html#_inner_list2mdlist', 'relax/docs.py'),
+                            'relax.docs._italic': ('docs.html#_italic', 'relax/docs.py'),
+                            'relax.docs._params_mdlist': ('docs.html#_params_mdlist', 'relax/docs.py'),
+                            'relax.docs._repr_markdown': ('docs.html#_repr_markdown', 'relax/docs.py'),
+                            'relax.docs._return_mdlist': ('docs.html#_return_mdlist', 'relax/docs.py'),
+                            'relax.docs._show_param': ('docs.html#_show_param', 'relax/docs.py'),
+                            'relax.docs._show_params_return': ('docs.html#_show_params_return', 'relax/docs.py')},
+            'relax.evaluate': { 'relax.evaluate.BaseEvalMetrics': ('evaluate.html#baseevalmetrics', 'relax/evaluate.py'),
+                                'relax.evaluate.BaseEvalMetrics.__call__': ('evaluate.html#baseevalmetrics.__call__', 'relax/evaluate.py'),
+                                'relax.evaluate.BaseEvalMetrics.__init__': ('evaluate.html#baseevalmetrics.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.BaseEvalMetrics.__str__': ('evaluate.html#baseevalmetrics.__str__', 'relax/evaluate.py'),
+                                'relax.evaluate.ManifoldDist': ('evaluate.html#manifolddist', 'relax/evaluate.py'),
+                                'relax.evaluate.ManifoldDist.__call__': ('evaluate.html#manifolddist.__call__', 'relax/evaluate.py'),
+                                'relax.evaluate.ManifoldDist.__init__': ('evaluate.html#manifolddist.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.PredictiveAccuracy': ('evaluate.html#predictiveaccuracy', 'relax/evaluate.py'),
+                                'relax.evaluate.PredictiveAccuracy.__call__': ( 'evaluate.html#predictiveaccuracy.__call__',
+                                                                                'relax/evaluate.py'),
+                                'relax.evaluate.PredictiveAccuracy.__init__': ( 'evaluate.html#predictiveaccuracy.__init__',
+                                                                                'relax/evaluate.py'),
+                                'relax.evaluate.Proximity': ('evaluate.html#proximity', 'relax/evaluate.py'),
+                                'relax.evaluate.Proximity.__call__': ('evaluate.html#proximity.__call__', 'relax/evaluate.py'),
+                                'relax.evaluate.Proximity.__init__': ('evaluate.html#proximity.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.Runtime': ('evaluate.html#runtime', 'relax/evaluate.py'),
+                                'relax.evaluate.Runtime.__call__': ('evaluate.html#runtime.__call__', 'relax/evaluate.py'),
+                                'relax.evaluate.Runtime.__init__': ('evaluate.html#runtime.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.Sparsity': ('evaluate.html#sparsity', 'relax/evaluate.py'),
+                                'relax.evaluate.Sparsity.__call__': ('evaluate.html#sparsity.__call__', 'relax/evaluate.py'),
+                                'relax.evaluate.Sparsity.__init__': ('evaluate.html#sparsity.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.Validity': ('evaluate.html#validity', 'relax/evaluate.py'),
+                                'relax.evaluate.Validity.__call__': ('evaluate.html#validity.__call__', 'relax/evaluate.py'),
+                                'relax.evaluate.Validity.__init__': ('evaluate.html#validity.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate._get_metric': ('evaluate.html#_get_metric', 'relax/evaluate.py'),
+                                'relax.evaluate.benchmark_cfs': ('evaluate.html#benchmark_cfs', 'relax/evaluate.py'),
+                                'relax.evaluate.compute_proximity': ('evaluate.html#compute_proximity', 'relax/evaluate.py'),
+                                'relax.evaluate.compute_single_proximity': ('evaluate.html#compute_single_proximity', 'relax/evaluate.py'),
+                                'relax.evaluate.compute_single_sparsity': ('evaluate.html#compute_single_sparsity', 'relax/evaluate.py'),
+                                'relax.evaluate.compute_single_validity': ('evaluate.html#compute_single_validity', 'relax/evaluate.py'),
+                                'relax.evaluate.compute_sparsity': ('evaluate.html#compute_sparsity', 'relax/evaluate.py'),
+                                'relax.evaluate.compute_validity': ('evaluate.html#compute_validity', 'relax/evaluate.py'),
+                                'relax.evaluate.evaluate_cfs': ('evaluate.html#evaluate_cfs', 'relax/evaluate.py'),
+                                'relax.evaluate.l2_ann': ('evaluate.html#l2_ann', 'relax/evaluate.py'),
+                                'relax.evaluate.pairwise_distances': ('evaluate.html#pairwise_distances', 'relax/evaluate.py')},
+            'relax.explain': { 'relax.explain.Explanation': ('explain.html#explanation', 'relax/explain.py'),
+                               'relax.explain.Explanation.__getitem__': ('explain.html#explanation.__getitem__', 'relax/explain.py'),
+                               'relax.explain.Explanation.__init__': ('explain.html#explanation.__init__', 'relax/explain.py'),
+                               'relax.explain.Explanation.__repr__': ('explain.html#explanation.__repr__', 'relax/explain.py'),
+                               'relax.explain.Explanation.cfs': ('explain.html#explanation.cfs', 'relax/explain.py'),
+                               'relax.explain.Explanation.copy': ('explain.html#explanation.copy', 'relax/explain.py'),
+                               'relax.explain.Explanation.data_name': ('explain.html#explanation.data_name', 'relax/explain.py'),
+                               'relax.explain.Explanation.feature_indices': ( 'explain.html#explanation.feature_indices',
+                                                                              'relax/explain.py'),
+                               'relax.explain.Explanation.features_and_indices': ( 'explain.html#explanation.features_and_indices',
+                                                                                   'relax/explain.py'),
+                               'relax.explain.Explanation.load_from_path': ('explain.html#explanation.load_from_path', 'relax/explain.py'),
+                               'relax.explain.Explanation.save': ('explain.html#explanation.save', 'relax/explain.py'),
+                               'relax.explain.fake_explanation': ('explain.html#fake_explanation', 'relax/explain.py'),
+                               'relax.explain.generate_cf_explanations': ('explain.html#generate_cf_explanations', 'relax/explain.py'),
+                               'relax.explain.prepare_cf_module': ('explain.html#prepare_cf_module', 'relax/explain.py'),
+                               'relax.explain.prepare_pred_fn': ('explain.html#prepare_pred_fn', 'relax/explain.py'),
+                               'relax.explain.prepare_rng_keys': ('explain.html#prepare_rng_keys', 'relax/explain.py')},
+            'relax.import_essentials': {},
+            'relax.legacy.ckpt_manager': { 'relax.legacy.ckpt_manager.CheckpointManager': ( 'legacy/ckpt_manager.html#checkpointmanager',
+                                                                                            'relax/legacy/ckpt_manager.py'),
+                                           'relax.legacy.ckpt_manager.CheckpointManager.__init__': ( 'legacy/ckpt_manager.html#checkpointmanager.__init__',
+                                                                                                     'relax/legacy/ckpt_manager.py'),
+                                           'relax.legacy.ckpt_manager.CheckpointManager.delete_net_opt': ( 'legacy/ckpt_manager.html#checkpointmanager.delete_net_opt',
+                                                                                                           'relax/legacy/ckpt_manager.py'),
+                                           'relax.legacy.ckpt_manager.CheckpointManager.save_net_opt': ( 'legacy/ckpt_manager.html#checkpointmanager.save_net_opt',
+                                                                                                         'relax/legacy/ckpt_manager.py'),
+                                           'relax.legacy.ckpt_manager.CheckpointManager.update_checkpoints': ( 'legacy/ckpt_manager.html#checkpointmanager.update_checkpoints',
+                                                                                                               'relax/legacy/ckpt_manager.py'),
+                                           'relax.legacy.ckpt_manager.load_checkpoint': ( 'legacy/ckpt_manager.html#load_checkpoint',
+                                                                                          'relax/legacy/ckpt_manager.py'),
+                                           'relax.legacy.ckpt_manager.save_checkpoint': ( 'legacy/ckpt_manager.html#save_checkpoint',
+                                                                                          'relax/legacy/ckpt_manager.py')},
+            'relax.legacy.import_essentials': {},
+            'relax.legacy.logger': { 'relax.legacy.logger.Logger': ('legacy/logger.html#logger', 'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.__init__': ( 'legacy/logger.html#logger.__init__',
+                                                                              'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.close': ('legacy/logger.html#logger.close', 'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.get_last_logs': ( 'legacy/logger.html#logger.get_last_logs',
+                                                                                   'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.log': ('legacy/logger.html#logger.log', 'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.log_dict': ( 'legacy/logger.html#logger.log_dict',
+                                                                              'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.log_dir': ('legacy/logger.html#logger.log_dir', 'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.on_epoch_finished': ( 'legacy/logger.html#logger.on_epoch_finished',
+                                                                                       'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.on_epoch_started': ( 'legacy/logger.html#logger.on_epoch_started',
+                                                                                      'relax/legacy/logger.py'),
+                                     'relax.legacy.logger.Logger.save_hyperparams': ( 'legacy/logger.html#logger.save_hyperparams',
+                                                                                      'relax/legacy/logger.py')},
+            'relax.legacy.module': { 'relax.legacy.module.BaseNetwork': ('legacy/module.html#basenetwork', 'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseNetwork.__call__': ( 'legacy/module.html#basenetwork.__call__',
+                                                                                   'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseTrainingModule': ( 'legacy/module.html#basetrainingmodule',
+                                                                                 'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseTrainingModule.init_logger': ( 'legacy/module.html#basetrainingmodule.init_logger',
+                                                                                             'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseTrainingModule.init_net_opt': ( 'legacy/module.html#basetrainingmodule.init_net_opt',
+                                                                                              'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseTrainingModule.log': ( 'legacy/module.html#basetrainingmodule.log',
+                                                                                     'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseTrainingModule.log_dict': ( 'legacy/module.html#basetrainingmodule.log_dict',
+                                                                                          'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseTrainingModule.save_hyperparameters': ( 'legacy/module.html#basetrainingmodule.save_hyperparameters',
+                                                                                                      'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseTrainingModule.training_step': ( 'legacy/module.html#basetrainingmodule.training_step',
+                                                                                               'relax/legacy/module.py'),
+                                     'relax.legacy.module.BaseTrainingModule.validation_step': ( 'legacy/module.html#basetrainingmodule.validation_step',
+                                                                                                 'relax/legacy/module.py'),
+                                     'relax.legacy.module.DenseBlock': ('legacy/module.html#denseblock', 'relax/legacy/module.py'),
+                                     'relax.legacy.module.DenseBlock.__call__': ( 'legacy/module.html#denseblock.__call__',
+                                                                                  'relax/legacy/module.py'),
+                                     'relax.legacy.module.DenseBlock.__init__': ( 'legacy/module.html#denseblock.__init__',
+                                                                                  'relax/legacy/module.py'),
+                                     'relax.legacy.module.MLP': ('legacy/module.html#mlp', 'relax/legacy/module.py'),
+                                     'relax.legacy.module.MLP.__call__': ('legacy/module.html#mlp.__call__', 'relax/legacy/module.py'),
+                                     'relax.legacy.module.MLP.__init__': ('legacy/module.html#mlp.__init__', 'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveModel': ( 'legacy/module.html#predictivemodel',
+                                                                              'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveModel.__call__': ( 'legacy/module.html#predictivemodel.__call__',
+                                                                                       'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveModel.__init__': ( 'legacy/module.html#predictivemodel.__init__',
+                                                                                       'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveModelConfigs': ( 'legacy/module.html#predictivemodelconfigs',
+                                                                                     'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule': ( 'legacy/module.html#predictivetrainingmodule',
+                                                                                       'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule.__init__': ( 'legacy/module.html#predictivetrainingmodule.__init__',
+                                                                                                'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule._training_step': ( 'legacy/module.html#predictivetrainingmodule._training_step',
+                                                                                                      'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule.forward': ( 'legacy/module.html#predictivetrainingmodule.forward',
+                                                                                               'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule.init_net_opt': ( 'legacy/module.html#predictivetrainingmodule.init_net_opt',
+                                                                                                    'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule.loss_fn': ( 'legacy/module.html#predictivetrainingmodule.loss_fn',
+                                                                                               'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule.pred_fn': ( 'legacy/module.html#predictivetrainingmodule.pred_fn',
+                                                                                               'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule.training_step': ( 'legacy/module.html#predictivetrainingmodule.training_step',
+                                                                                                     'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModule.validation_step': ( 'legacy/module.html#predictivetrainingmodule.validation_step',
+                                                                                                       'relax/legacy/module.py'),
+                                     'relax.legacy.module.PredictiveTrainingModuleConfigs': ( 'legacy/module.html#predictivetrainingmoduleconfigs',
+                                                                                              'relax/legacy/module.py')},
+            'relax.legacy.trainer': { 'relax.legacy.trainer.TrainingConfigs': ( 'legacy/trainer.html#trainingconfigs',
+                                                                                'relax/legacy/trainer.py'),
+                                      'relax.legacy.trainer.TrainingConfigs.PRNGSequence': ( 'legacy/trainer.html#trainingconfigs.prngsequence',
+                                                                                             'relax/legacy/trainer.py'),
+                                      'relax.legacy.trainer.train_model': ('legacy/trainer.html#train_model', 'relax/legacy/trainer.py'),
+                                      'relax.legacy.trainer.train_model_with_states': ( 'legacy/trainer.html#train_model_with_states',
+                                                                                        'relax/legacy/trainer.py')},
+            'relax.legacy.utils': { 'relax.legacy.utils.Config': ('legacy/utils.html#config', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.Config.default': ('legacy/utils.html#config.default', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.accuracy': ('legacy/utils.html#accuracy', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.binary_cross_entropy': ( 'legacy/utils.html#binary_cross_entropy',
+                                                                                 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.cat_normalize': ('legacy/utils.html#cat_normalize', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.check_cat_info': ('legacy/utils.html#check_cat_info', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.dist': ('legacy/utils.html#dist', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.get_config': ('legacy/utils.html#get_config', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.grad_update': ('legacy/utils.html#grad_update', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.init_net_opt': ('legacy/utils.html#init_net_opt', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.load_json': ('legacy/utils.html#load_json', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.make_hk_module': ('legacy/utils.html#make_hk_module', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.make_model': ('legacy/utils.html#make_model', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.proximity': ('legacy/utils.html#proximity', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.sigmoid': ('legacy/utils.html#sigmoid', 'relax/legacy/utils.py'),
+                                    'relax.legacy.utils.validate_configs': ('legacy/utils.html#validate_configs', 'relax/legacy/utils.py')},
+            'relax.methods.base': { 'relax.methods.base.CFModule': ('methods/base.html#cfmodule', 'relax/methods/base.py'),
+                                    'relax.methods.base.CFModule.__init__': ( 'methods/base.html#cfmodule.__init__',
+                                                                              'relax/methods/base.py'),
+                                    'relax.methods.base.CFModule.apply_constraints': ( 'methods/base.html#cfmodule.apply_constraints',
+                                                                                       'relax/methods/base.py'),
+                                    'relax.methods.base.CFModule.before_generate_cf': ( 'methods/base.html#cfmodule.before_generate_cf',
+                                                                                        'relax/methods/base.py'),
+                                    'relax.methods.base.CFModule.compute_reg_loss': ( 'methods/base.html#cfmodule.compute_reg_loss',
+                                                                                      'relax/methods/base.py'),
+                                    'relax.methods.base.CFModule.generate_cf': ( 'methods/base.html#cfmodule.generate_cf',
+                                                                                 'relax/methods/base.py'),
+                                    'relax.methods.base.CFModule.set_apply_constraints_fn': ( 'methods/base.html#cfmodule.set_apply_constraints_fn',
+                                                                                              'relax/methods/base.py'),
+                                    'relax.methods.base.CFModule.set_compute_reg_loss_fn': ( 'methods/base.html#cfmodule.set_compute_reg_loss_fn',
+                                                                                             'relax/methods/base.py'),
+                                    'relax.methods.base.CFModule.set_data_module': ( 'methods/base.html#cfmodule.set_data_module',
+                                                                                     'relax/methods/base.py'),
+                                    'relax.methods.base.ParametricCFModule': ( 'methods/base.html#parametriccfmodule',
+                                                                               'relax/methods/base.py'),
+                                    'relax.methods.base.ParametricCFModule.train': ( 'methods/base.html#parametriccfmodule.train',
+                                                                                     'relax/methods/base.py'),
+                                    'relax.methods.base.default_apply_constraints_fn': ( 'methods/base.html#default_apply_constraints_fn',
+                                                                                         'relax/methods/base.py'),
+                                    'relax.methods.base.default_compute_reg_loss_fn': ( 'methods/base.html#default_compute_reg_loss_fn',
+                                                                                        'relax/methods/base.py')},
+            'relax.methods.cchvae': { 'relax.methods.cchvae.CCHVAE': ('methods/cchvae.html#cchvae', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE.__init__': ( 'methods/cchvae.html#cchvae.__init__',
+                                                                                'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE._init_model': ( 'methods/cchvae.html#cchvae._init_model',
+                                                                                   'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE.generate_cf': ( 'methods/cchvae.html#cchvae.generate_cf',
+                                                                                   'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE.train': ('methods/cchvae.html#cchvae.train', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAEConfig': ('methods/cchvae.html#cchvaeconfig', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE': ('methods/cchvae.html#chvae', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.__init__': ( 'methods/cchvae.html#chvae.__init__',
+                                                                               'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.build': ('methods/cchvae.html#chvae.build', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.call': ('methods/cchvae.html#chvae.call', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.compute_kl_loss': ( 'methods/cchvae.html#chvae.compute_kl_loss',
+                                                                                      'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.decode': ('methods/cchvae.html#chvae.decode', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.encode': ('methods/cchvae.html#chvae.encode', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.forward': ( 'methods/cchvae.html#chvae.forward',
+                                                                              'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.regenerate': ( 'methods/cchvae.html#chvae.regenerate',
+                                                                                 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.reparameterize': ( 'methods/cchvae.html#chvae.reparameterize',
+                                                                                     'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CHVAE.set_apply_constraints_fn': ( 'methods/cchvae.html#chvae.set_apply_constraints_fn',
+                                                                                               'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae._cchvae': ('methods/cchvae.html#_cchvae', 'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae._hyper_sphere_coordindates': ( 'methods/cchvae.html#_hyper_sphere_coordindates',
+                                                                                           'relax/methods/cchvae.py')},
+            'relax.methods.clue': { 'relax.methods.clue.CLUE': ('methods/clue.html#clue', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE.__init__': ('methods/clue.html#clue.__init__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE._init_model': ('methods/clue.html#clue._init_model', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE.generate_cf': ('methods/clue.html#clue.generate_cf', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUE.train': ('methods/clue.html#clue.train', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.CLUEConfig': ('methods/clue.html#clueconfig', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Decoder': ('methods/clue.html#decoder', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Decoder.__call__': ('methods/clue.html#decoder.__call__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Decoder.__init__': ('methods/clue.html#decoder.__init__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Encoder': ('methods/clue.html#encoder', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Encoder.__init__': ('methods/clue.html#encoder.__init__', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.Encoder.call': ('methods/clue.html#encoder.call', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat': ('methods/clue.html#vaegausscat', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.__init__': ( 'methods/clue.html#vaegausscat.__init__',
+                                                                                 'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.build': ( 'methods/clue.html#vaegausscat.build',
+                                                                              'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.call': ('methods/clue.html#vaegausscat.call', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.compute_vae_loss': ( 'methods/clue.html#vaegausscat.compute_vae_loss',
+                                                                                         'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.decode': ( 'methods/clue.html#vaegausscat.decode',
+                                                                               'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.encode': ( 'methods/clue.html#vaegausscat.encode',
+                                                                               'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.sample': ( 'methods/clue.html#vaegausscat.sample',
+                                                                               'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.sample_latent': ( 'methods/clue.html#vaegausscat.sample_latent',
+                                                                                      'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.sample_step': ( 'methods/clue.html#vaegausscat.sample_step',
+                                                                                    'relax/methods/clue.py'),
+                                    'relax.methods.clue.VAEGaussCat.set_reconstruction_loss': ( 'methods/clue.html#vaegausscat.set_reconstruction_loss',
+                                                                                                'relax/methods/clue.py'),
+                                    'relax.methods.clue._clue_generate': ('methods/clue.html#_clue_generate', 'relax/methods/clue.py'),
+                                    'relax.methods.clue.get_reconstruction_loss_fn': ( 'methods/clue.html#get_reconstruction_loss_fn',
+                                                                                       'relax/methods/clue.py'),
+                                    'relax.methods.clue.kl_divergence': ('methods/clue.html#kl_divergence', 'relax/methods/clue.py')},
+            'relax.methods.counternet': { 'relax.methods.counternet.CounterNet': ( 'methods/counternet.html#counternet',
+                                                                                   'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNet.__init__': ( 'methods/counternet.html#counternet.__init__',
+                                                                                            'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNet._init_model': ( 'methods/counternet.html#counternet._init_model',
+                                                                                               'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNet.generate_cf': ( 'methods/counternet.html#counternet.generate_cf',
+                                                                                               'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNet.is_trained': ( 'methods/counternet.html#counternet.is_trained',
+                                                                                              'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNet.pred_fn': ( 'methods/counternet.html#counternet.pred_fn',
+                                                                                           'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNet.train': ( 'methods/counternet.html#counternet.train',
+                                                                                         'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetConfig': ( 'methods/counternet.html#counternetconfig',
+                                                                                         'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetModel': ( 'methods/counternet.html#counternetmodel',
+                                                                                        'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetModel.__call__': ( 'methods/counternet.html#counternetmodel.__call__',
+                                                                                                 'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetModel.__init__': ( 'methods/counternet.html#counternetmodel.__init__',
+                                                                                                 'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule': ( 'methods/counternet.html#counternettrainingmodule',
+                                                                                                 'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.__init__': ( 'methods/counternet.html#counternettrainingmodule.__init__',
+                                                                                                          'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule._explainer_step': ( 'methods/counternet.html#counternettrainingmodule._explainer_step',
+                                                                                                                 'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule._predictor_step': ( 'methods/counternet.html#counternettrainingmodule._predictor_step',
+                                                                                                                 'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule._training_step': ( 'methods/counternet.html#counternettrainingmodule._training_step',
+                                                                                                                'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule._training_step_logs': ( 'methods/counternet.html#counternettrainingmodule._training_step_logs',
+                                                                                                                     'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.exp_loss_fn': ( 'methods/counternet.html#counternettrainingmodule.exp_loss_fn',
+                                                                                                             'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.forward': ( 'methods/counternet.html#counternettrainingmodule.forward',
+                                                                                                         'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.generate_cf': ( 'methods/counternet.html#counternettrainingmodule.generate_cf',
+                                                                                                             'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.init_net_opt': ( 'methods/counternet.html#counternettrainingmodule.init_net_opt',
+                                                                                                              'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_1': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_1',
+                                                                                                           'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_2': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_2',
+                                                                                                           'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.loss_fn_3': ( 'methods/counternet.html#counternettrainingmodule.loss_fn_3',
+                                                                                                           'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.pred_fn': ( 'methods/counternet.html#counternettrainingmodule.pred_fn',
+                                                                                                         'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.pred_loss_fn': ( 'methods/counternet.html#counternettrainingmodule.pred_loss_fn',
+                                                                                                              'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.training_step': ( 'methods/counternet.html#counternettrainingmodule.training_step',
+                                                                                                               'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNetTrainingModule.validation_step': ( 'methods/counternet.html#counternettrainingmodule.validation_step',
+                                                                                                                 'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.partition_trainable_params': ( 'methods/counternet.html#partition_trainable_params',
+                                                                                                   'relax/methods/counternet.py')},
+            'relax.methods.dice': { 'relax.methods.dice.DiverseCF': ('methods/dice.html#diversecf', 'relax/methods/dice.py'),
+                                    'relax.methods.dice.DiverseCF.__init__': ( 'methods/dice.html#diversecf.__init__',
+                                                                               'relax/methods/dice.py'),
+                                    'relax.methods.dice.DiverseCF.generate_cf': ( 'methods/dice.html#diversecf.generate_cf',
+                                                                                  'relax/methods/dice.py'),
+                                    'relax.methods.dice.DiverseCF.load_from_path': ( 'methods/dice.html#diversecf.load_from_path',
+                                                                                     'relax/methods/dice.py'),
+                                    'relax.methods.dice.DiverseCF.save': ('methods/dice.html#diversecf.save', 'relax/methods/dice.py'),
+                                    'relax.methods.dice.DiverseCFConfig': ('methods/dice.html#diversecfconfig', 'relax/methods/dice.py'),
+                                    'relax.methods.dice._diverse_cf': ('methods/dice.html#_diverse_cf', 'relax/methods/dice.py'),
+                                    'relax.methods.dice.dpp_style_vmap': ('methods/dice.html#dpp_style_vmap', 'relax/methods/dice.py')},
+            'relax.methods.l2c': { 'relax.methods.l2c.Discretizer': ('methods/l2c.html#discretizer', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.__init__': ( 'methods/l2c.html#discretizer.__init__',
+                                                                               'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.fit': ('methods/l2c.html#discretizer.fit', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.fit_transform': ( 'methods/l2c.html#discretizer.fit_transform',
+                                                                                    'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.get_pred_fn': ( 'methods/l2c.html#discretizer.get_pred_fn',
+                                                                                  'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.inverse_transform': ( 'methods/l2c.html#discretizer.inverse_transform',
+                                                                                        'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.inverse_transform_indices': ( 'methods/l2c.html#discretizer.inverse_transform_indices',
+                                                                                                'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.inversed_transform_pytree': ( 'methods/l2c.html#discretizer.inversed_transform_pytree',
+                                                                                                'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.transform': ( 'methods/l2c.html#discretizer.transform',
+                                                                                'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.Discretizer.transform_indices': ( 'methods/l2c.html#discretizer.transform_indices',
+                                                                                        'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2C': ('methods/l2c.html#l2c', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2C.__init__': ('methods/l2c.html#l2c.__init__', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2C.generate_cf': ('methods/l2c.html#l2c.generate_cf', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2C.train': ('methods/l2c.html#l2c.train', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CConfig': ('methods/l2c.html#l2cconfig', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel': ('methods/l2c.html#l2cmodel', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.__init__': ('methods/l2c.html#l2cmodel.__init__', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.build': ('methods/l2c.html#l2cmodel.build', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.call': ('methods/l2c.html#l2cmodel.call', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.compute_l2c_loss': ( 'methods/l2c.html#l2cmodel.compute_l2c_loss',
+                                                                                    'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.forward': ('methods/l2c.html#l2cmodel.forward', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.set_features_info': ( 'methods/l2c.html#l2cmodel.set_features_info',
+                                                                                     'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.set_immutable_mask': ( 'methods/l2c.html#l2cmodel.set_immutable_mask',
+                                                                                      'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.set_pred_fn': ( 'methods/l2c.html#l2cmodel.set_pred_fn',
+                                                                               'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.L2CModel.start_end_indices': ( 'methods/l2c.html#l2cmodel.start_end_indices',
+                                                                                     'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.cut_quantiles': ('methods/l2c.html#cut_quantiles', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.discretize_xs': ('methods/l2c.html#discretize_xs', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.gumbel_softmax': ('methods/l2c.html#gumbel_softmax', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.qcut': ('methods/l2c.html#qcut', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.qcut_inverse': ('methods/l2c.html#qcut_inverse', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.sample_bernouli': ('methods/l2c.html#sample_bernouli', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.sample_categorical': ('methods/l2c.html#sample_categorical', 'relax/methods/l2c.py'),
+                                   'relax.methods.l2c.split_fn': ('methods/l2c.html#split_fn', 'relax/methods/l2c.py')},
+            'relax.methods.proto': { 'relax.methods.proto.ProtoCF': ('methods/proto.html#protocf', 'relax/methods/proto.py'),
+                                     'relax.methods.proto.ProtoCF.__init__': ( 'methods/proto.html#protocf.__init__',
+                                                                               'relax/methods/proto.py'),
+                                     'relax.methods.proto.ProtoCF._init_model': ( 'methods/proto.html#protocf._init_model',
+                                                                                  'relax/methods/proto.py'),
+                                     'relax.methods.proto.ProtoCF.generate_cf': ( 'methods/proto.html#protocf.generate_cf',
+                                                                                  'relax/methods/proto.py'),
+                                     'relax.methods.proto.ProtoCF.train': ('methods/proto.html#protocf.train', 'relax/methods/proto.py'),
+                                     'relax.methods.proto.ProtoCFConfig': ('methods/proto.html#protocfconfig', 'relax/methods/proto.py'),
+                                     'relax.methods.proto._proto_cf': ('methods/proto.html#_proto_cf', 'relax/methods/proto.py')},
+            'relax.methods.sphere': { 'relax.methods.sphere.GSConfig': ('methods/sphere.html#gsconfig', 'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere': ( 'methods/sphere.html#growingsphere',
+                                                                              'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere.__init__': ( 'methods/sphere.html#growingsphere.__init__',
+                                                                                       'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere.before_generate_cf': ( 'methods/sphere.html#growingsphere.before_generate_cf',
+                                                                                                 'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere.generate_cf': ( 'methods/sphere.html#growingsphere.generate_cf',
+                                                                                          'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere.has_data_module': ( 'methods/sphere.html#growingsphere.has_data_module',
+                                                                                              'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere.load_from_path': ( 'methods/sphere.html#growingsphere.load_from_path',
+                                                                                             'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.GrowingSphere.save': ( 'methods/sphere.html#growingsphere.save',
+                                                                                   'relax/methods/sphere.py'),
+                                      'relax.methods.sphere._growing_spheres': ( 'methods/sphere.html#_growing_spheres',
+                                                                                 'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.cat_perturb_fn': ( 'methods/sphere.html#cat_perturb_fn',
+                                                                               'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.default_perturb_function': ( 'methods/sphere.html#default_perturb_function',
+                                                                                         'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.features_to_infos_and_perturb_fn': ( 'methods/sphere.html#features_to_infos_and_perturb_fn',
+                                                                                                 'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.hyper_sphere_coordindates': ( 'methods/sphere.html#hyper_sphere_coordindates',
+                                                                                          'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.perturb_function_with_features': ( 'methods/sphere.html#perturb_function_with_features',
+                                                                                               'relax/methods/sphere.py'),
+                                      'relax.methods.sphere.sample_categorical': ( 'methods/sphere.html#sample_categorical',
+                                                                                   'relax/methods/sphere.py')},
+            'relax.methods.vaecf': { 'relax.methods.vaecf.VAE': ('methods/vaecf.html#vae', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.__init__': ('methods/vaecf.html#vae.__init__', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE._compile': ('methods/vaecf.html#vae._compile', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.build': ('methods/vaecf.html#vae.build', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.call': ('methods/vaecf.html#vae.call', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.compute_vae_loss': ( 'methods/vaecf.html#vae.compute_vae_loss',
+                                                                                   'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.decode': ('methods/vaecf.html#vae.decode', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.encode': ('methods/vaecf.html#vae.encode', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.sample': ('methods/vaecf.html#vae.sample', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.set_compute_regularization_fn': ( 'methods/vaecf.html#vae.set_compute_regularization_fn',
+                                                                                                'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAE.set_pred_fn': ( 'methods/vaecf.html#vae.set_pred_fn',
+                                                                              'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF': ('methods/vaecf.html#vaecf', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF.__init__': ('methods/vaecf.html#vaecf.__init__', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF._init_model': ( 'methods/vaecf.html#vaecf._init_model',
+                                                                                'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF.generate_cf': ( 'methods/vaecf.html#vaecf.generate_cf',
+                                                                                'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF.train': ('methods/vaecf.html#vaecf.train', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECFConfig': ('methods/vaecf.html#vaecfconfig', 'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.hindge_embedding_loss': ( 'methods/vaecf.html#hindge_embedding_loss',
+                                                                                    'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.sample_latent': ('methods/vaecf.html#sample_latent', 'relax/methods/vaecf.py')},
+            'relax.methods.vanilla': { 'relax.methods.vanilla.VanillaCF': ('methods/vanilla.html#vanillacf', 'relax/methods/vanilla.py'),
+                                       'relax.methods.vanilla.VanillaCF.__init__': ( 'methods/vanilla.html#vanillacf.__init__',
+                                                                                     'relax/methods/vanilla.py'),
+                                       'relax.methods.vanilla.VanillaCF.generate_cf': ( 'methods/vanilla.html#vanillacf.generate_cf',
+                                                                                        'relax/methods/vanilla.py'),
+                                       'relax.methods.vanilla.VanillaCF.load_from_path': ( 'methods/vanilla.html#vanillacf.load_from_path',
+                                                                                           'relax/methods/vanilla.py'),
+                                       'relax.methods.vanilla.VanillaCF.save': ( 'methods/vanilla.html#vanillacf.save',
+                                                                                 'relax/methods/vanilla.py'),
+                                       'relax.methods.vanilla.VanillaCFConfig': ( 'methods/vanilla.html#vanillacfconfig',
+                                                                                  'relax/methods/vanilla.py'),
+                                       'relax.methods.vanilla._vanilla_cf': ( 'methods/vanilla.html#_vanilla_cf',
+                                                                              'relax/methods/vanilla.py')},
+            'relax.ml_model': { 'relax.ml_model.AutoEncoder': ('ml_model.html#autoencoder', 'relax/ml_model.py'),
+                                'relax.ml_model.AutoEncoder.__init__': ('ml_model.html#autoencoder.__init__', 'relax/ml_model.py'),
+                                'relax.ml_model.AutoEncoder.call': ('ml_model.html#autoencoder.call', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModule': ('ml_model.html#mlmodule', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModule.__init__': ('ml_model.html#mlmodule.__init__', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModule._init_model': ('ml_model.html#mlmodule._init_model', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModule.is_trained': ('ml_model.html#mlmodule.is_trained', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModule.load_from_path': ('ml_model.html#mlmodule.load_from_path', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModule.pred_fn': ('ml_model.html#mlmodule.pred_fn', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModule.save': ('ml_model.html#mlmodule.save', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModule.train': ('ml_model.html#mlmodule.train', 'relax/ml_model.py'),
+                                'relax.ml_model.MLModuleConfig': ('ml_model.html#mlmoduleconfig', 'relax/ml_model.py'),
+                                'relax.ml_model.MLP': ('ml_model.html#mlp', 'relax/ml_model.py'),
+                                'relax.ml_model.MLP.__init__': ('ml_model.html#mlp.__init__', 'relax/ml_model.py'),
+                                'relax.ml_model.MLP.call': ('ml_model.html#mlp.call', 'relax/ml_model.py'),
+                                'relax.ml_model.MLP.get_config': ('ml_model.html#mlp.get_config', 'relax/ml_model.py'),
+                                'relax.ml_model.MLPBlock': ('ml_model.html#mlpblock', 'relax/ml_model.py'),
+                                'relax.ml_model.MLPBlock.__init__': ('ml_model.html#mlpblock.__init__', 'relax/ml_model.py'),
+                                'relax.ml_model.MLPBlock.build': ('ml_model.html#mlpblock.build', 'relax/ml_model.py'),
+                                'relax.ml_model.MLPBlock.call': ('ml_model.html#mlpblock.call', 'relax/ml_model.py'),
+                                'relax.ml_model.download_ml_module': ('ml_model.html#download_ml_module', 'relax/ml_model.py'),
+                                'relax.ml_model.load_ml_module': ('ml_model.html#load_ml_module', 'relax/ml_model.py')},
+            'relax.strategy': { 'relax.strategy.BaseStrategy': ('explain.strategy.html#basestrategy', 'relax/strategy.py'),
+                                'relax.strategy.BaseStrategy.__call__': ( 'explain.strategy.html#basestrategy.__call__',
+                                                                          'relax/strategy.py'),
+                                'relax.strategy.BatchedPmapStrategy': ('explain.strategy.html#batchedpmapstrategy', 'relax/strategy.py'),
+                                'relax.strategy.BatchedPmapStrategy.__call__': ( 'explain.strategy.html#batchedpmapstrategy.__call__',
+                                                                                 'relax/strategy.py'),
+                                'relax.strategy.BatchedPmapStrategy.__init__': ( 'explain.strategy.html#batchedpmapstrategy.__init__',
+                                                                                 'relax/strategy.py'),
+                                'relax.strategy.BatchedVmapStrategy': ('explain.strategy.html#batchedvmapstrategy', 'relax/strategy.py'),
+                                'relax.strategy.BatchedVmapStrategy.__call__': ( 'explain.strategy.html#batchedvmapstrategy.__call__',
+                                                                                 'relax/strategy.py'),
+                                'relax.strategy.BatchedVmapStrategy.__init__': ( 'explain.strategy.html#batchedvmapstrategy.__init__',
+                                                                                 'relax/strategy.py'),
+                                'relax.strategy.IterativeStrategy': ('explain.strategy.html#iterativestrategy', 'relax/strategy.py'),
+                                'relax.strategy.IterativeStrategy.__call__': ( 'explain.strategy.html#iterativestrategy.__call__',
+                                                                               'relax/strategy.py'),
+                                'relax.strategy.PmapStrategy': ('explain.strategy.html#pmapstrategy', 'relax/strategy.py'),
+                                'relax.strategy.PmapStrategy.__call__': ( 'explain.strategy.html#pmapstrategy.__call__',
+                                                                          'relax/strategy.py'),
+                                'relax.strategy.PmapStrategy.__init__': ( 'explain.strategy.html#pmapstrategy.__init__',
+                                                                          'relax/strategy.py'),
+                                'relax.strategy.StrategyFactory': ('explain.strategy.html#strategyfactory', 'relax/strategy.py'),
+                                'relax.strategy.StrategyFactory.__init__': ( 'explain.strategy.html#strategyfactory.__init__',
+                                                                             'relax/strategy.py'),
+                                'relax.strategy.StrategyFactory.get_default_strategy': ( 'explain.strategy.html#strategyfactory.get_default_strategy',
+                                                                                         'relax/strategy.py'),
+                                'relax.strategy.StrategyFactory.get_strategy': ( 'explain.strategy.html#strategyfactory.get_strategy',
+                                                                                 'relax/strategy.py'),
+                                'relax.strategy.VmapStrategy': ('explain.strategy.html#vmapstrategy', 'relax/strategy.py'),
+                                'relax.strategy.VmapStrategy.__call__': ( 'explain.strategy.html#vmapstrategy.__call__',
+                                                                          'relax/strategy.py'),
+                                'relax.strategy._batched_generation': ('explain.strategy.html#_batched_generation', 'relax/strategy.py'),
+                                'relax.strategy._pad_divisible_X': ('explain.strategy.html#_pad_divisible_x', 'relax/strategy.py'),
+                                'relax.strategy._pad_xs': ('explain.strategy.html#_pad_xs', 'relax/strategy.py')},
+            'relax.utils': { 'relax.utils.Config': ('utils.html#config', 'relax/utils.py'),
+                             'relax.utils.Config.default': ('utils.html#config.default', 'relax/utils.py'),
+                             'relax.utils._is_array': ('utils.html#_is_array', 'relax/utils.py'),
+                             'relax.utils._reshape_x': ('utils.html#_reshape_x', 'relax/utils.py'),
+                             'relax.utils.auto_reshaping': ('utils.html#auto_reshaping', 'relax/utils.py'),
+                             'relax.utils.get_config': ('utils.html#get_config', 'relax/utils.py'),
+                             'relax.utils.grad_update': ('utils.html#grad_update', 'relax/utils.py'),
+                             'relax.utils.gumbel_softmax': ('utils.html#gumbel_softmax', 'relax/utils.py'),
+                             'relax.utils.load_json': ('utils.html#load_json', 'relax/utils.py'),
+                             'relax.utils.load_pytree': ('utils.html#load_pytree', 'relax/utils.py'),
+                             'relax.utils.save_pytree': ('utils.html#save_pytree', 'relax/utils.py'),
+                             'relax.utils.set_config': ('utils.html#set_config', 'relax/utils.py'),
+                             'relax.utils.validate_configs': ('utils.html#validate_configs', 'relax/utils.py')}}}
```

### Comparing `jax-relax-0.2.5/relax/base.py` & `jax-relax-0.2.6/relax/base.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/data_module.py` & `jax-relax-0.2.6/relax/data_module.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         elif name in ['valid', 'test']:
             return self._get_data(self.config.test_indices)
         else:
             raise ValueError(f"Unknown data name: {name}. Should be one of ['train', 'valid', 'test']")
     
     def set_transformations(
         self, 
-        feature_names_to_transformation: Dict[str, Union[str, Dict, Transformation]], # Dict[feature_name, Transformation]
+        feature_names_to_transformation: Dict[str, Union[str, Dict, BaseTransformation]], # Dict[feature_name, Transformation]
     ) -> DataModule:
         """Reset transformations for features."""
 
         self._features = self._features.set_transformations(feature_names_to_transformation)
         return self
     
     def sample(
```

### Comparing `jax-relax-0.2.5/relax/docs.py` & `jax-relax-0.2.6/relax/docs.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/evaluate.py` & `jax-relax-0.2.6/relax/evaluate.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/explain.py` & `jax-relax-0.2.6/relax/explain.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/import_essentials.py` & `jax-relax-0.2.6/relax/import_essentials.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/legacy/ckpt_manager.py` & `jax-relax-0.2.6/relax/legacy/ckpt_manager.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/legacy/import_essentials.py` & `jax-relax-0.2.6/relax/legacy/import_essentials.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/legacy/logger.py` & `jax-relax-0.2.6/relax/legacy/logger.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/legacy/module.py` & `jax-relax-0.2.6/relax/legacy/module.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/legacy/trainer.py` & `jax-relax-0.2.6/relax/legacy/trainer.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/legacy/utils.py` & `jax-relax-0.2.6/relax/legacy/utils.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/base.py` & `jax-relax-0.2.6/relax/methods/base.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/cchvae.py` & `jax-relax-0.2.6/relax/methods/cchvae.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/clue.py` & `jax-relax-0.2.6/relax/methods/clue.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/counternet.py` & `jax-relax-0.2.6/relax/methods/counternet.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/dice.py` & `jax-relax-0.2.6/relax/methods/dice.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/l2c.py` & `jax-relax-0.2.6/relax/methods/l2c.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/proto.py` & `jax-relax-0.2.6/relax/methods/proto.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/sphere.py` & `jax-relax-0.2.6/relax/methods/sphere.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/vaecf.py` & `jax-relax-0.2.6/relax/methods/vaecf.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/methods/vanilla.py` & `jax-relax-0.2.6/relax/methods/vanilla.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/ml_model.py` & `jax-relax-0.2.6/relax/ml_model.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/strategy.py` & `jax-relax-0.2.6/relax/strategy.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.2.5/relax/utils.py` & `jax-relax-0.2.6/relax/utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_utils.ipynb.
-
-# %% ../nbs/00_utils.ipynb 3
-from __future__ import annotations
-from .import_essentials import *
-import nbdev
-from fastcore.basics import AttrDict
-from nbdev.showdoc import BasicMarkdownRenderer
-from inspect import isclass
-from fastcore.test import *
-from jax.core import InconclusiveDimensionOperation
-
-# %% auto 0
-__all__ = ['validate_configs', 'save_pytree', 'load_pytree', 'auto_reshaping', 'grad_update', 'gumbel_softmax', 'load_json',
-           'get_config', 'set_config']
-
-# %% ../nbs/00_utils.ipynb 5
-def validate_configs(
-    configs: dict | BaseParser,  # A configuration of the model/dataset.
-    config_cls: BaseParser,  # The desired configuration class.
-) -> BaseParser:
-    """return a valid configuration object."""
-
-    assert isclass(config_cls), f"`config_cls` should be a class."
-    assert issubclass(config_cls, BaseParser), \
-        f"{config_cls} should be a subclass of `BaseParser`."
-    
-    if isinstance(configs, dict):
-        configs = config_cls(**configs)
-    if not isinstance(configs, config_cls):
-        raise TypeError(
-            f"configs should be either a `dict` or an instance of {config_cls.__name__}.")
-    return configs
-
-# %% ../nbs/00_utils.ipynb 15
-def _is_array(x):
-    return isinstance(x, np.ndarray) or isinstance(x, jnp.ndarray) or isinstance(x, list)
-
-def save_pytree(pytree, saved_dir):
-    """Save a pytree to a directory."""
-    with open(os.path.join(saved_dir, "data.npy"), "wb") as f:
-        for x in jax.tree_util.tree_leaves(pytree):
-            np.save(f, x)
-
-    tree_struct = jax.tree_util.tree_map(lambda t: _is_array(t), pytree)
-    with open(os.path.join(saved_dir, "treedef.json"), "w") as f:
-        json.dump(tree_struct, f)
-
-# %% ../nbs/00_utils.ipynb 20
-def load_pytree(saved_dir):
-    """Load a pytree from a saved directory."""
-    with open(os.path.join(saved_dir, "treedef.json"), "r") as f:
-        tree_struct = json.load(f)
-
-    leaves, treedef = jax.tree_util.tree_flatten(tree_struct)
-    with open(os.path.join(saved_dir, "data.npy"), "rb") as f:
-        flat_state = [
-            np.load(f, allow_pickle=True) if is_arr else np.load(f, allow_pickle=True).item()
-            for is_arr in leaves
-        ]
-    return jax.tree_util.tree_unflatten(treedef, flat_state)
-
-# %% ../nbs/00_utils.ipynb 24
-def _reshape_x(x: Array):
-    x_size = x.shape
-    if len(x_size) > 1 and x_size[0] != 1:
-        raise ValueError(
-            f"""Invalid Input Shape: Require `x.shape` = (1, k) or (k, ),
-but got `x.shape` = {x.shape}. This method expects a single input instance."""
-        )
-    if len(x_size) == 1:
-        x = x.reshape(1, -1)
-    return x, x_size
-
-# %% ../nbs/00_utils.ipynb 25
-def auto_reshaping(
-    reshape_argname: str, # The name of the argument to be reshaped.
-    reshape_output: bool = True, # Whether to reshape the output. Useful to set `False` when returning multiple cfs.
-):
-    """
-    Decorator to automatically reshape function's input into (1, k), 
-    and out to input's shape.
-    """
-    def decorator(func):
-        def wrapper(*args, **kwargs):
-            kwargs = inspect.getcallargs(func, *args, **kwargs)
-            if reshape_argname in kwargs:
-                reshaped_x, x_shape = _reshape_x(kwargs[reshape_argname])
-                kwargs[reshape_argname] = reshaped_x
-            else:
-                raise ValueError(
-                    f"Invalid argument name: `{reshape_argname}` is not a valid argument name.")
-            # Call the function.
-            cf = func(**kwargs)
-            if not isinstance(cf, Array): 
-                raise ValueError(
-                    f"Invalid return type: must be a `jax.Array`, but got `{type(cf).__name__}`.")
-            if reshape_output:
-                try: 
-                    cf = cf.reshape(x_shape)
-                except (InconclusiveDimensionOperation, TypeError) as e:
-                    raise ValueError(
-                        f"Invalid return shape: Require `cf.shape` = {cf.shape} "
-                        f"is not compatible with `x.shape` = {x_shape}.")
-            return cf
-
-        return wrapper
-    return decorator
-
-# %% ../nbs/00_utils.ipynb 30
-def grad_update(
-    grads, # A pytree of gradients.
-    params, # A pytree of parameters.
-    opt_state: optax.OptState,
-    opt: optax.GradientTransformation,
-): # Return (upt_params, upt_opt_state)
-    updates, opt_state = opt.update(grads, opt_state, params)
-    upt_params = optax.apply_updates(params, updates)
-    return upt_params, opt_state
-
-# %% ../nbs/00_utils.ipynb 32
-def gumbel_softmax(
-    key: jrand.PRNGKey, # Random key
-    logits: Array, # Logits for each class. Shape (batch_size, num_classes)
-    tau: float, # Temperature for the Gumbel softmax
-    axis: int | tuple[int, ...] = -1, # The axis or axes along which the gumbel softmax should be computed
-):
-    """The Gumbel softmax function."""
-
-    gumbel_noise = jrand.gumbel(key, shape=logits.shape)
-    y = logits + gumbel_noise
-    return jax.nn.softmax(y / tau, axis=axis)
-
-# %% ../nbs/00_utils.ipynb 34
-def load_json(f_name: str) -> Dict[str, Any]:  # file name
-    with open(f_name) as f:
-        return json.load(f)
-
-
-# %% ../nbs/00_utils.ipynb 36
-@dataclass
-class Config:
-    rng_reserve_size: int
-    global_seed: int
-
-    @classmethod
-    def default(cls) -> Config:
-        return cls(rng_reserve_size=1, global_seed=42)
-
-main_config = Config.default()
-
-# %% ../nbs/00_utils.ipynb 37
-def get_config() -> Config: 
-    return main_config
-
-# %% ../nbs/00_utils.ipynb 38
-def set_config(
-    *,
-    rng_reserve_size: int = None, # The number of random number generators to reserve.
-    global_seed: int = None, # The global seed for random number generators.
-    **kwargs
-) -> None:
-    """Sets the global configurations."""
-
-    def set_val(
-        arg_name: str, # The name of the argument.
-        arg_value: int, # The value of the argument.
-        arg_min: int # The minimum value of the argument.
-    ) -> None:
-        """Checks the validity of the argument and sets the value."""
-        
-        if arg_value is None or not hasattr(main_config, arg_name):
-            return
-        
-        if not isinstance(arg_value, int):
-            raise TypeError(f"`{arg_name}` must be an integer, but got {type(arg_value).__name__}.")
-        if arg_value < arg_min:
-            raise ValueError(f"`{arg_name}` must be non-negative, but got {arg_value}.")
-        setattr(main_config, arg_name, arg_value)
-
-    set_val('rng_reserve_size', rng_reserve_size, 1)
-    set_val('global_seed', global_seed, 0)
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_utils.ipynb.
+
+# %% ../nbs/00_utils.ipynb 3
+from __future__ import annotations
+from .import_essentials import *
+import nbdev
+from fastcore.basics import AttrDict
+from nbdev.showdoc import BasicMarkdownRenderer
+from inspect import isclass
+from fastcore.test import *
+from jax.core import InconclusiveDimensionOperation
+
+# %% auto 0
+__all__ = ['validate_configs', 'save_pytree', 'load_pytree', 'auto_reshaping', 'grad_update', 'gumbel_softmax', 'load_json',
+           'get_config', 'set_config']
+
+# %% ../nbs/00_utils.ipynb 5
+def validate_configs(
+    configs: dict | BaseParser,  # A configuration of the model/dataset.
+    config_cls: BaseParser,  # The desired configuration class.
+) -> BaseParser:
+    """return a valid configuration object."""
+
+    assert isclass(config_cls), f"`config_cls` should be a class."
+    assert issubclass(config_cls, BaseParser), \
+        f"{config_cls} should be a subclass of `BaseParser`."
+    
+    if isinstance(configs, dict):
+        configs = config_cls(**configs)
+    if not isinstance(configs, config_cls):
+        raise TypeError(
+            f"configs should be either a `dict` or an instance of {config_cls.__name__}.")
+    return configs
+
+# %% ../nbs/00_utils.ipynb 15
+def _is_array(x):
+    return isinstance(x, np.ndarray) or isinstance(x, jnp.ndarray) or isinstance(x, list)
+
+def save_pytree(pytree, saved_dir):
+    """Save a pytree to a directory."""
+    with open(os.path.join(saved_dir, "data.npy"), "wb") as f:
+        for x in jax.tree_util.tree_leaves(pytree):
+            np.save(f, x)
+
+    tree_struct = jax.tree_util.tree_map(lambda t: _is_array(t), pytree)
+    with open(os.path.join(saved_dir, "treedef.json"), "w") as f:
+        json.dump(tree_struct, f)
+
+# %% ../nbs/00_utils.ipynb 20
+def load_pytree(saved_dir):
+    """Load a pytree from a saved directory."""
+    with open(os.path.join(saved_dir, "treedef.json"), "r") as f:
+        tree_struct = json.load(f)
+
+    leaves, treedef = jax.tree_util.tree_flatten(tree_struct)
+    with open(os.path.join(saved_dir, "data.npy"), "rb") as f:
+        flat_state = [
+            np.load(f, allow_pickle=True) if is_arr else np.load(f, allow_pickle=True).item()
+            for is_arr in leaves
+        ]
+    return jax.tree_util.tree_unflatten(treedef, flat_state)
+
+# %% ../nbs/00_utils.ipynb 24
+def _reshape_x(x: Array):
+    x_size = x.shape
+    if len(x_size) > 1 and x_size[0] != 1:
+        raise ValueError(
+            f"""Invalid Input Shape: Require `x.shape` = (1, k) or (k, ),
+but got `x.shape` = {x.shape}. This method expects a single input instance."""
+        )
+    if len(x_size) == 1:
+        x = x.reshape(1, -1)
+    return x, x_size
+
+# %% ../nbs/00_utils.ipynb 25
+def auto_reshaping(
+    reshape_argname: str, # The name of the argument to be reshaped.
+    reshape_output: bool = True, # Whether to reshape the output. Useful to set `False` when returning multiple cfs.
+):
+    """
+    Decorator to automatically reshape function's input into (1, k), 
+    and out to input's shape.
+    """
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            kwargs = inspect.getcallargs(func, *args, **kwargs)
+            if reshape_argname in kwargs:
+                reshaped_x, x_shape = _reshape_x(kwargs[reshape_argname])
+                kwargs[reshape_argname] = reshaped_x
+            else:
+                raise ValueError(
+                    f"Invalid argument name: `{reshape_argname}` is not a valid argument name.")
+            # Call the function.
+            cf = func(**kwargs)
+            if not isinstance(cf, Array): 
+                raise ValueError(
+                    f"Invalid return type: must be a `jax.Array`, but got `{type(cf).__name__}`.")
+            if reshape_output:
+                try: 
+                    cf = cf.reshape(x_shape)
+                except (InconclusiveDimensionOperation, TypeError) as e:
+                    raise ValueError(
+                        f"Invalid return shape: Require `cf.shape` = {cf.shape} "
+                        f"is not compatible with `x.shape` = {x_shape}.")
+            return cf
+
+        return wrapper
+    return decorator
+
+# %% ../nbs/00_utils.ipynb 30
+def grad_update(
+    grads, # A pytree of gradients.
+    params, # A pytree of parameters.
+    opt_state: optax.OptState,
+    opt: optax.GradientTransformation,
+): # Return (upt_params, upt_opt_state)
+    updates, opt_state = opt.update(grads, opt_state, params)
+    upt_params = optax.apply_updates(params, updates)
+    return upt_params, opt_state
+
+# %% ../nbs/00_utils.ipynb 32
+def gumbel_softmax(
+    key: jrand.PRNGKey, # Random key
+    logits: Array, # Logits for each class. Shape (batch_size, num_classes)
+    tau: float, # Temperature for the Gumbel softmax
+    axis: int | tuple[int, ...] = -1, # The axis or axes along which the gumbel softmax should be computed
+):
+    """The Gumbel softmax function."""
+
+    gumbel_noise = jrand.gumbel(key, shape=logits.shape)
+    y = logits + gumbel_noise
+    return jax.nn.softmax(y / tau, axis=axis)
+
+# %% ../nbs/00_utils.ipynb 34
+def load_json(f_name: str) -> Dict[str, Any]:  # file name
+    with open(f_name) as f:
+        return json.load(f)
+
+
+# %% ../nbs/00_utils.ipynb 36
+@dataclass
+class Config:
+    rng_reserve_size: int
+    global_seed: int
+
+    @classmethod
+    def default(cls) -> Config:
+        return cls(rng_reserve_size=1, global_seed=42)
+
+main_config = Config.default()
+
+# %% ../nbs/00_utils.ipynb 37
+def get_config() -> Config: 
+    return main_config
+
+# %% ../nbs/00_utils.ipynb 38
+def set_config(
+    *,
+    rng_reserve_size: int = None, # The number of random number generators to reserve.
+    global_seed: int = None, # The global seed for random number generators.
+    **kwargs
+) -> None:
+    """Sets the global configurations."""
+
+    def set_val(
+        arg_name: str, # The name of the argument.
+        arg_value: int, # The value of the argument.
+        arg_min: int # The minimum value of the argument.
+    ) -> None:
+        """Checks the validity of the argument and sets the value."""
+        
+        if arg_value is None or not hasattr(main_config, arg_name):
+            return
+        
+        if not isinstance(arg_value, int):
+            raise TypeError(f"`{arg_name}` must be an integer, but got {type(arg_value).__name__}.")
+        if arg_value < arg_min:
+            raise ValueError(f"`{arg_name}` must be non-negative, but got {arg_value}.")
+        setattr(main_config, arg_name, arg_value)
+
+    set_val('rng_reserve_size', rng_reserve_size, 1)
+    set_val('global_seed', global_seed, 0)
```

### Comparing `jax-relax-0.2.5/settings.ini` & `jax-relax-0.2.6/settings.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-[DEFAULT]
-repo = jax-relax
-lib_name = jax-relax
-version = 0.2.5
-min_python = 3.9
-license = apache2
-black_formatting = False
-doc_path = _docs
-lib_path = relax
-nbs_path = nbs
-recursive = True
-tst_flags = slow
-put_version_in_init = True
-branch = master
-custom_sidebar = True
-doc_host = https://birkhoffg.github.io
-doc_baseurl = /jax-relax
-git_url = https://github.com/birkhoffg/jax-relax
-title = jax-relax
-renderer = relax.docs.CustomizedMarkdownRenderer
-audience = Developers
-author = BirkhoffG
-author_email = 26811230+BirkhoffG@users.noreply.github.com
-copyright = 2022 onwards, BirkhoffG
-description = JAX-based Recourse Explanation Library
-keywords = JAX, Recourse, Explanation, Interpretability, Machine Learning
-language = English
-status = 3
-user = birkhoffg
-requirements = scikit-learn>=1.0.2,<1.4.0 pandas jax[cpu] tqdm optax pydantic>=1.9.0,<2 jax-tqdm einops keras>=3.0.3 matplotlib seaborn dm-haiku
-dev_requirements = torch>=1.7.0 causalgraphicalmodels pre-commit datasets nbdev jupyter
-readme_nb = index.ipynb
-allowed_metadata_keys = 
-allowed_cell_metadata_keys = 
-jupyter_hooks = True
-clean_ids = True
-clear_all = False
-
+[DEFAULT]
+repo = jax-relax
+lib_name = jax-relax
+version = 0.2.6
+min_python = 3.9
+license = apache2
+black_formatting = False
+doc_path = _docs
+lib_path = relax
+nbs_path = nbs
+recursive = True
+tst_flags = slow
+put_version_in_init = True
+branch = master
+custom_sidebar = True
+doc_host = https://birkhoffg.github.io
+doc_baseurl = /jax-relax
+git_url = https://github.com/birkhoffg/jax-relax
+title = jax-relax
+renderer = relax.docs.CustomizedMarkdownRenderer
+audience = Developers
+author = BirkhoffG
+author_email = 26811230+BirkhoffG@users.noreply.github.com
+copyright = 2022 onwards, BirkhoffG
+description = JAX-based Recourse Explanation Library
+keywords = JAX, Recourse, Explanation, Interpretability, Machine Learning
+language = English
+status = 3
+user = birkhoffg
+requirements = scikit-learn>=1.0.2 pandas jax[cpu] tqdm optax pydantic>=1.9.0,<2 jax-tqdm einops keras>=3.0.3 matplotlib seaborn dm-haiku
+dev_requirements = torch>=1.7.0 causalgraphicalmodels pre-commit datasets nbdev jupyter
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
+
```

### Comparing `jax-relax-0.2.5/setup.py` & `jax-relax-0.2.6/setup.py`

 * *Files identical despite different names*

