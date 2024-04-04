# Comparing `tmp/draupnir-0.0.29.tar.gz` & `tmp/draupnir-0.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draupnir-0.0.29.tar", last modified: Tue Apr  2 22:02:55 2024, max compression
+gzip compressed data, was "draupnir-0.0.30.tar", last modified: Thu Apr  4 14:39:56 2024, max compression
```

## Comparing `draupnir-0.0.29.tar` & `draupnir-0.0.30.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-02 22:02:55.505727 draupnir-0.0.29/
--rw-r--r--   0 lys       (1000) lys       (1000)     1071 2022-02-03 12:22:28.000000 draupnir-0.0.29/LICENSE
--rw-r--r--   0 lys       (1000) lys       (1000)       15 2022-02-04 14:46:10.000000 draupnir-0.0.29/MANIFEST.in
--rw-r--r--   0 lys       (1000) lys       (1000)    11167 2024-04-02 22:02:55.505727 draupnir-0.0.29/PKG-INFO
--rw-r--r--   0 lys       (1000) lys       (1000)     9945 2024-02-23 18:22:33.000000 draupnir-0.0.29/README.md
--rw-r--r--   0 lys       (1000) lys       (1000)      103 2022-02-03 12:19:06.000000 draupnir-0.0.29/pyproject.toml
--rw-r--r--   0 lys       (1000) lys       (1000)      748 2024-04-02 22:02:55.505727 draupnir-0.0.29/setup.cfg
--rw-r--r--   0 lys       (1000) lys       (1000)     3138 2024-04-02 21:58:37.000000 draupnir-0.0.29/setup.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-02 22:02:55.481727 draupnir-0.0.29/src/
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-02 22:02:55.485727 draupnir-0.0.29/src/draupnir/
--rw-r--r--   0 lys       (1000) lys       (1000)    15019 2022-03-01 17:48:39.000000 draupnir-0.0.29/src/draupnir/3D.py
--rw-r--r--   0 lys       (1000) lys       (1000)      496 2022-03-30 13:01:42.000000 draupnir-0.0.29/src/draupnir/__init__.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-02 22:02:55.485727 draupnir-0.0.29/src/draupnir/data/
--rw-r--r--   0 lys       (1000) lys       (1000)     1578 2021-07-28 14:11:37.000000 draupnir-0.0.29/src/draupnir/data/AA_properties.txt
--rw-r--r--   0 lys       (1000) lys       (1000) 32494553 2021-07-28 14:11:52.000000 draupnir-0.0.29/src/draupnir/data/PfamPdbMap.txt
--rw-r--r--   0 lys       (1000) lys       (1000)    37249 2024-04-01 21:31:59.000000 draupnir-0.0.29/src/draupnir/datasets.py
--rw-r--r--   0 lys       (1000) lys       (1000)     9362 2022-03-22 15:01:49.000000 draupnir-0.0.29/src/draupnir/draw_tree.py
--rw-r--r--   0 lys       (1000) lys       (1000)    11193 2024-04-02 21:27:05.000000 draupnir-0.0.29/src/draupnir/guides.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-02 22:02:55.505727 draupnir-0.0.29/src/draupnir/infer_angles/
--rw-r--r--   0 lys       (1000) lys       (1000)      330 2022-02-15 14:19:01.000000 draupnir-0.0.29/src/draupnir/infer_angles/__init__.py
--rw-r--r--   0 lys       (1000) lys       (1000)     5319 2021-08-19 13:41:22.000000 draupnir-0.0.29/src/draupnir/infer_angles/calculate_coords.py
--rw-r--r--   0 lys       (1000) lys       (1000)     1362 2021-08-13 17:18:45.000000 draupnir-0.0.29/src/draupnir/infer_angles/nerf.py
--rw-r--r--   0 lys       (1000) lys       (1000)     9437 2021-08-13 17:41:01.000000 draupnir-0.0.29/src/draupnir/infer_angles/pnerf.py
--rw-r--r--   0 lys       (1000) lys       (1000)    19190 2022-02-13 16:56:12.000000 draupnir-0.0.29/src/draupnir/infer_angles/superposition.py
--rw-r--r--   0 lys       (1000) lys       (1000)    60195 2024-04-02 17:24:44.000000 draupnir-0.0.29/src/draupnir/load_utils.py
--rw-r--r--   0 lys       (1000) lys       (1000)   182199 2024-04-02 21:09:37.000000 draupnir-0.0.29/src/draupnir/main.py
--rw-r--r--   0 lys       (1000) lys       (1000)    68853 2024-04-02 21:55:50.000000 draupnir-0.0.29/src/draupnir/models.py
--rw-r--r--   0 lys       (1000) lys       (1000)    23103 2024-04-02 21:16:58.000000 draupnir-0.0.29/src/draupnir/models_utils.py
--rw-r--r--   0 lys       (1000) lys       (1000)    17819 2023-05-10 11:36:14.000000 draupnir-0.0.29/src/draupnir/mutual_information.py
--rw-r--r--   0 lys       (1000) lys       (1000)    81724 2024-02-23 21:46:00.000000 draupnir-0.0.29/src/draupnir/plots.py
--rw-r--r--   0 lys       (1000) lys       (1000)     6840 2024-04-02 21:24:45.000000 draupnir-0.0.29/src/draupnir/train.py
--rw-r--r--   0 lys       (1000) lys       (1000)   109487 2024-04-02 21:36:45.000000 draupnir-0.0.29/src/draupnir/utils.py
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-02 22:02:55.505727 draupnir-0.0.29/src/draupnir.egg-info/
--rw-r--r--   0 lys       (1000) lys       (1000)    11167 2024-04-02 22:02:55.000000 draupnir-0.0.29/src/draupnir.egg-info/PKG-INFO
--rw-r--r--   0 lys       (1000) lys       (1000)      951 2024-04-02 22:02:55.000000 draupnir-0.0.29/src/draupnir.egg-info/SOURCES.txt
--rw-r--r--   0 lys       (1000) lys       (1000)        1 2024-04-02 22:02:55.000000 draupnir-0.0.29/src/draupnir.egg-info/dependency_links.txt
--rw-r--r--   0 lys       (1000) lys       (1000)        1 2022-03-02 13:52:18.000000 draupnir-0.0.29/src/draupnir.egg-info/not-zip-safe
--rw-r--r--   0 lys       (1000) lys       (1000)      229 2024-04-02 22:02:55.000000 draupnir-0.0.29/src/draupnir.egg-info/requires.txt
--rw-r--r--   0 lys       (1000) lys       (1000)      120 2024-04-02 22:02:55.000000 draupnir-0.0.29/src/draupnir.egg-info/top_level.txt
-drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-02 22:02:55.505727 draupnir-0.0.29/tests/
--rw-r--r--   0 lys       (1000) lys       (1000)     6414 2022-03-30 15:40:03.000000 draupnir-0.0.29/tests/test_accuracy.py
--rw-r--r--   0 lys       (1000) lys       (1000)     2173 2022-03-30 16:33:30.000000 draupnir-0.0.29/tests/test_examples.py
--rw-r--r--   0 lys       (1000) lys       (1000)     3793 2022-03-30 13:55:34.000000 draupnir-0.0.29/tests/test_load.py
--rw-r--r--   0 lys       (1000) lys       (1000)     4483 2022-03-29 19:20:16.000000 draupnir-0.0.29/tests/test_norworking.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-04 14:39:56.777207 draupnir-0.0.30/
+-rw-r--r--   0 lys       (1000) lys       (1000)     1071 2022-02-03 12:22:28.000000 draupnir-0.0.30/LICENSE
+-rw-r--r--   0 lys       (1000) lys       (1000)       15 2022-02-04 14:46:10.000000 draupnir-0.0.30/MANIFEST.in
+-rw-r--r--   0 lys       (1000) lys       (1000)    11262 2024-04-04 14:39:56.777207 draupnir-0.0.30/PKG-INFO
+-rw-r--r--   0 lys       (1000) lys       (1000)    10040 2024-04-04 14:37:58.000000 draupnir-0.0.30/README.md
+-rw-r--r--   0 lys       (1000) lys       (1000)      103 2022-02-03 12:19:06.000000 draupnir-0.0.30/pyproject.toml
+-rw-r--r--   0 lys       (1000) lys       (1000)      748 2024-04-04 14:39:56.777207 draupnir-0.0.30/setup.cfg
+-rw-r--r--   0 lys       (1000) lys       (1000)     3138 2024-04-04 14:37:58.000000 draupnir-0.0.30/setup.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-04 14:39:56.757207 draupnir-0.0.30/src/
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-04 14:39:56.757207 draupnir-0.0.30/src/draupnir/
+-rw-r--r--   0 lys       (1000) lys       (1000)    15019 2022-03-01 17:48:39.000000 draupnir-0.0.30/src/draupnir/3D.py
+-rw-r--r--   0 lys       (1000) lys       (1000)      496 2022-03-30 13:01:42.000000 draupnir-0.0.30/src/draupnir/__init__.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-04 14:39:56.757207 draupnir-0.0.30/src/draupnir/data/
+-rw-r--r--   0 lys       (1000) lys       (1000)     1578 2021-07-28 14:11:37.000000 draupnir-0.0.30/src/draupnir/data/AA_properties.txt
+-rw-r--r--   0 lys       (1000) lys       (1000) 32494553 2021-07-28 14:11:52.000000 draupnir-0.0.30/src/draupnir/data/PfamPdbMap.txt
+-rw-r--r--   0 lys       (1000) lys       (1000)    37249 2024-04-01 21:31:59.000000 draupnir-0.0.30/src/draupnir/datasets.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     9362 2022-03-22 15:01:49.000000 draupnir-0.0.30/src/draupnir/draw_tree.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    11193 2024-04-02 21:27:05.000000 draupnir-0.0.30/src/draupnir/guides.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-04 14:39:56.777207 draupnir-0.0.30/src/draupnir/infer_angles/
+-rw-r--r--   0 lys       (1000) lys       (1000)      330 2022-02-15 14:19:01.000000 draupnir-0.0.30/src/draupnir/infer_angles/__init__.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     5319 2021-08-19 13:41:22.000000 draupnir-0.0.30/src/draupnir/infer_angles/calculate_coords.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     1362 2021-08-13 17:18:45.000000 draupnir-0.0.30/src/draupnir/infer_angles/nerf.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     9437 2021-08-13 17:41:01.000000 draupnir-0.0.30/src/draupnir/infer_angles/pnerf.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    19190 2022-02-13 16:56:12.000000 draupnir-0.0.30/src/draupnir/infer_angles/superposition.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    60195 2024-04-02 17:24:44.000000 draupnir-0.0.30/src/draupnir/load_utils.py
+-rw-r--r--   0 lys       (1000) lys       (1000)   182199 2024-04-02 21:09:37.000000 draupnir-0.0.30/src/draupnir/main.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    86384 2024-04-04 14:36:15.000000 draupnir-0.0.30/src/draupnir/models.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    23103 2024-04-02 21:16:58.000000 draupnir-0.0.30/src/draupnir/models_utils.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    17819 2023-05-10 11:36:14.000000 draupnir-0.0.30/src/draupnir/mutual_information.py
+-rw-r--r--   0 lys       (1000) lys       (1000)    81724 2024-02-23 21:46:00.000000 draupnir-0.0.30/src/draupnir/plots.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     6840 2024-04-02 21:24:45.000000 draupnir-0.0.30/src/draupnir/train.py
+-rw-r--r--   0 lys       (1000) lys       (1000)   109487 2024-04-02 21:36:45.000000 draupnir-0.0.30/src/draupnir/utils.py
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-04 14:39:56.777207 draupnir-0.0.30/src/draupnir.egg-info/
+-rw-r--r--   0 lys       (1000) lys       (1000)    11262 2024-04-04 14:39:56.000000 draupnir-0.0.30/src/draupnir.egg-info/PKG-INFO
+-rw-r--r--   0 lys       (1000) lys       (1000)      951 2024-04-04 14:39:56.000000 draupnir-0.0.30/src/draupnir.egg-info/SOURCES.txt
+-rw-r--r--   0 lys       (1000) lys       (1000)        1 2024-04-04 14:39:56.000000 draupnir-0.0.30/src/draupnir.egg-info/dependency_links.txt
+-rw-r--r--   0 lys       (1000) lys       (1000)        1 2022-03-02 13:52:18.000000 draupnir-0.0.30/src/draupnir.egg-info/not-zip-safe
+-rw-r--r--   0 lys       (1000) lys       (1000)      229 2024-04-04 14:39:56.000000 draupnir-0.0.30/src/draupnir.egg-info/requires.txt
+-rw-r--r--   0 lys       (1000) lys       (1000)      120 2024-04-04 14:39:56.000000 draupnir-0.0.30/src/draupnir.egg-info/top_level.txt
+drwxrwxr-x   0 lys       (1000) lys       (1000)        0 2024-04-04 14:39:56.777207 draupnir-0.0.30/tests/
+-rw-r--r--   0 lys       (1000) lys       (1000)     6414 2022-03-30 15:40:03.000000 draupnir-0.0.30/tests/test_accuracy.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     2173 2022-03-30 16:33:30.000000 draupnir-0.0.30/tests/test_examples.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     3793 2022-03-30 13:55:34.000000 draupnir-0.0.30/tests/test_load.py
+-rw-r--r--   0 lys       (1000) lys       (1000)     4483 2022-03-29 19:20:16.000000 draupnir-0.0.30/tests/test_norworking.py
```

### Comparing `draupnir-0.0.29/LICENSE` & `draupnir-0.0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/PKG-INFO` & `draupnir-0.0.30/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draupnir
-Version: 0.0.29
+Version: 0.0.30
 Summary: Ancestral sequence reconstruction using a tree structured Ornstein Uhlenbeck variational autoencoder
 Home-page: https://github.com/LysSanzMoreta/DRAUPNIR_ASR
 Author: Lys Sanz Moreta
 Author-email: lys.sanz.moreta@outlook.com
 Project-URL: Changelog, https://github.com/LysSanzMoreta/DRAUPNIR_ASR/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/LysSanzMoreta/DRAUPNIR_ASR/issues
 Classifier: Development Status :: 4 - Beta
@@ -187,14 +187,16 @@
   year={2021}
 }
 ```
 
 
 **Do not hesitate to give input on how to improve the documentation of this library**
 
+**Leave like and subscribe ... wait that was somewhere else ... well, a star will do it ;) **
+
```

### Comparing `draupnir-0.0.29/README.md` & `draupnir-0.0.30/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,16 @@
   year={2021}
 }
 ```
 
 
 **Do not hesitate to give input on how to improve the documentation of this library**
 
+**Leave like and subscribe ... wait that was somewhere else ... well, a star will do it ;) **
+
```

### Comparing `draupnir-0.0.29/setup.cfg` & `draupnir-0.0.30/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = draupnir-artistworking43
-version = 0.0.29
+version = 0.0.30
 author = Lys Sanz Moreta
 author_email = lys.sanz.moreta@outlook.com
 description = Draupnir: Ancestral protein sequence reconstruction using a tree-structured Ornstein-Uhlenbeck variational autoencoder
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/LysSanzMoreta/DRAUPNIR_ASR
 project_urls =
```

### Comparing `draupnir-0.0.29/setup.py` & `draupnir-0.0.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 setup(name='draupnir',
-      version='0.0.29',
+      version='0.0.30',
       # list folders, not files
       packages=find_packages('src'),
       package_dir={'': 'src'},
       py_modules=[splitext(basename(path))[0] for path in glob('src/draupnir/*.py')],
       #scripts=['bin/script1.py'],
       package_data={'draupnir': ['data/*']},
       description= 'Ancestral sequence reconstruction using a tree structured Ornstein Uhlenbeck variational autoencoder',
```

### Comparing `draupnir-0.0.29/src/draupnir/3D.py` & `draupnir-0.0.30/src/draupnir/3D.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/data/AA_properties.txt` & `draupnir-0.0.30/src/draupnir/data/AA_properties.txt`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/data/PfamPdbMap.txt` & `draupnir-0.0.30/src/draupnir/data/PfamPdbMap.txt`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/datasets.py` & `draupnir-0.0.30/src/draupnir/datasets.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/draw_tree.py` & `draupnir-0.0.30/src/draupnir/draw_tree.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/guides.py` & `draupnir-0.0.30/src/draupnir/guides.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/infer_angles/calculate_coords.py` & `draupnir-0.0.30/src/draupnir/infer_angles/calculate_coords.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/infer_angles/nerf.py` & `draupnir-0.0.30/src/draupnir/infer_angles/nerf.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/infer_angles/pnerf.py` & `draupnir-0.0.30/src/draupnir/infer_angles/pnerf.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/infer_angles/superposition.py` & `draupnir-0.0.30/src/draupnir/infer_angles/superposition.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/load_utils.py` & `draupnir-0.0.30/src/draupnir/load_utils.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/main.py` & `draupnir-0.0.30/src/draupnir/main.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/models.py` & `draupnir-0.0.30/src/draupnir/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 import torch
 import draupnir.utils as DraupnirUtils
 from draupnir.models_utils import *
 import pyro
 import pyro.distributions as dist
 
 SamplingOutput = namedtuple("SamplingOutput",["aa_sequences","latent_space","logits","phis","psis","mean_phi","mean_psi","kappa_phi","kappa_psi"])
+
 class DRAUPNIRModelClass(nn.Module):
     def __init__(self, ModelLoad):
         super(DRAUPNIRModelClass, self).__init__()
+        self.args = ModelLoad.args
         self.num_epochs = ModelLoad.args.num_epochs
         self.gru_hidden_dim = ModelLoad.gru_hidden_dim
         self.embedding_dim = ModelLoad.args.embedding_dim #blosum embedding dim
         self.position_embedding_dim= ModelLoad.args.position_embedding_dim
         self.pretrained_params = ModelLoad.pretrained_params
         self.z_dim = ModelLoad.z_dim
         self.leaves_nodes = ModelLoad.leaves_nodes
@@ -280,25 +282,26 @@
             latent_space = dist.MultivariateNormal(OU_mean.squeeze(-1), torch.linalg.inv(Inverse_internal)).to_event(1).sample()
             #latent_space = dist.MultivariateNormal(OU_mean.squeeze(-1), torch.cholesky_inverse(Inverse_internal) + 1e-6).to_event(1).sample()
 
             latent_space = latent_space.T
             assert latent_space.shape == (self.n_internal_batch, self.z_dim)
             return latent_space
 
-class DRAUPNIRModel_classic_test(DRAUPNIRModelClass):
+class DRAUPNIRModel_classic(DRAUPNIRModelClass):
     """Implements the ordinary version of Draupnir as described in the paper. It receives as an input the entire leaves dataset,
      uses a GRU as the mapping function and blosum embeddings"""
     def __init__(self,ModelLoad):
         DRAUPNIRModelClass.__init__(self,ModelLoad)
         self.rnn_input_size = self.z_dim + self.aa_probs
         self.num_layers = 1
         self.decoder = RNNDecoder_Tiling_new(self.align_seq_len, self.aa_probs, self.gru_hidden_dim, self.z_dim,
                                          self.rnn_input_size,self.kappa_addition,self.num_layers,self.pretrained_params)
         self.embed = EmbedComplex(self.aa_probs,self.embedding_dim, self.pretrained_params)
-    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
+
+    def model_variational(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
         aminoacid_sequences = family_data[:, 2:, 0]
         #batch_nodes = family_data[:, 0, 1]
         #batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
         # Highlight: Register GRU module
         pyro.module("embeddings",self.embed)
         pyro.module("decoder", self.decoder)
 
@@ -311,20 +314,54 @@
             blosum = self.embed(blosum)
             latent_space = torch.cat((latent_space,blosum),dim=2) #[n_nodes,align_seq_len,z_dim + 21]
             decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],
                                                        self.gru_hidden_dim).contiguous()  # bidirectional
 
             # if guide_map_estimates is not None:
             #     decoder_hidden = guide_map_estimates["rnn_final_bidirectional"]
-            with pyro.plate("plate_len", dim=-2):#with pyro.plate("plate_len", dim=-2, device=self.device):
+            with pyro.plate("plate_len", dim=-2):
                     logits = self.decoder.forward(
                         input=latent_space,
                         hidden=decoder_hidden)
                     pyro.sample("aa_sequences", dist.Categorical(logits=logits),obs=aminoacid_sequences)  # aa_seq = [n_nodes,align_seq_len]
 
+
+    def model_delta_map(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
+        aminoacid_sequences = family_data[:, 2:, 0]
+        #batch_nodes = family_data[:, 0, 1]
+        #batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
+        # Highlight: Register GRU module
+        pyro.module("embeddings",self.embed)
+        pyro.module("decoder", self.decoder)
+
+        # Highlight: GP prior over the latent space
+        latent_space = self.gp_prior(patristic_matrix_sorted)
+        # Highlight: MAP the latent space to logits using the Decoder from a Seq2seq model with/without attention
+        latent_space = latent_space.repeat(1,self.align_seq_len).reshape(latent_space.shape[0],self.align_seq_len,self.z_dim) #[n_nodes,max_seq,z_dim] #This can maybe be done with new axis solely
+        blosum = self.blosum_weighted.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.align_seq_len,self.aa_probs) #[n_nodes,max_seq,21]
+        blosum = self.embed(blosum)
+        latent_space = torch.cat((latent_space,blosum),dim=2) #[n_nodes,align_seq_len,z_dim + 21]
+        decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],
+                                                   self.gru_hidden_dim).contiguous()  # bidirectional
+
+        # if guide_map_estimates is not None:
+        #     decoder_hidden = guide_map_estimates["rnn_final_bidirectional"]
+        with pyro.plate("plate_len", aminoacid_sequences.shape[1], dim=-1), pyro.plate("plate_seq",aminoacid_sequences.shape[0],dim=-2):
+                logits = self.decoder.forward(
+                    input=latent_space,
+                    hidden=decoder_hidden)
+                pyro.sample("aa_sequences", dist.Categorical(logits=logits),obs=aminoacid_sequences)  # aa_seq = [n_nodes,align_seq_len]
+
+
+    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates):
+        if self.args.select_guide == "delta_map":
+            self.model_delta_map(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+        else:
+            self.model_variational(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+
     def sample(self, map_estimates, n_samples, family_data_test, patristic_matrix,cladistic_matrix,use_argmax=False,use_test=True,use_test2=False):
         if use_test2: #MAP estimate
             assert patristic_matrix[1:,1:].shape == (self.n_all,self.n_all)
             latent_space = self.conditional_samplingMAP(map_estimates,patristic_matrix)
             n_nodes = self.n_internal #I had to split it up because of some weird data cases (coral), otherwise family_data_test.shape[0] would have sufficed
         elif use_test:# Marginal posterior
             assert patristic_matrix[1:,1:].shape == (self.n_all,self.n_all)
@@ -337,23 +374,23 @@
 
         decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],self.gru_hidden_dim).contiguous()  # Not bidirectional
         latent_space_ = latent_space.repeat(1, self.align_seq_len).reshape(n_nodes,self.align_seq_len, self.z_dim)
         blosum = self.blosum_weighted.repeat(latent_space_.shape[0], 1).reshape(latent_space_.shape[0], self.align_seq_len,self.aa_probs)  # [n_nodes,max_seq,21]
         blosum = self.embed(blosum)
         latent_space_ = torch.cat((latent_space_, blosum), dim=2)  # [n_nodes,align_seq_len,z_dim + 21]
 
-        with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2,subsample_size=n_nodes):
-            logits = self.decoder.forward(
-                input=latent_space_,
-                hidden=decoder_hidden)
-            if use_argmax:
-                #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
-                aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
-            else:
-                aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
+        #with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2,subsample_size=n_nodes):
+        logits = self.decoder.forward(
+            input=latent_space_,
+            hidden=decoder_hidden)
+        if use_argmax:
+            #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
+            aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
+        else:
+            aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
 
         sampling_out = SamplingOutput(aa_sequences=aa_sequences.detach(),
                                       latent_space=latent_space.detach(),
                                       logits=logits.detach(),
                                       phis=None,
                                       psis=None,
                                       mean_phi=None,
@@ -366,15 +403,15 @@
 class DRAUPNIRModel_classic_no_blosum(DRAUPNIRModelClass):
     """Implements the ordinary version of Draupnir without blosum embeddings.
     It receives as an input the entire leaf dataset, uses a GRU as the mapping function WITHOUT blosum embeddings"""
     def __init__(self,ModelLoad):
         DRAUPNIRModelClass.__init__(self,ModelLoad)
         self.rnn_input_size = self.z_dim
         self.decoder = RNNDecoder_Tiling(self.align_seq_len, self.aa_probs, self.gru_hidden_dim, self.z_dim, self.rnn_input_size,self.kappa_addition,self.num_layers,self.pretrained_params)
-    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum = None,guide_map_estimates=None):
+    def model_variational(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum = None,guide_map_estimates=None):
         aminoacid_sequences = family_data[:, 2:, 0]
         batch_nodes = family_data[:, 0, 1]
         # Highlight: Register GRU module
         pyro.module("decoder", self.decoder)
         with pyro.plate("plate_batch", dim=-1, device=self.device):
             # Highlight: GP prior over the latent space
             latent_space = self.gp_prior(patristic_matrix_sorted)
@@ -385,36 +422,59 @@
 
             with pyro.plate("plate_len", aminoacid_sequences.shape[1], dim=-2):
                     logits = self.decoder.forward(
                         input=latent_space,
                         hidden=decoder_hidden)
                     pyro.sample("aa_sequences", dist.Categorical(logits=logits),obs=aminoacid_sequences)  # aa_seq = [n_nodes,align_seq_len]
 
+    def model_delta_map(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum = None,guide_map_estimates=None):
+        aminoacid_sequences = family_data[:, 2:, 0]
+        batch_nodes = family_data[:, 0, 1]
+        # Highlight: Register GRU module
+        pyro.module("decoder", self.decoder)
+        # Highlight: GP prior over the latent space
+        latent_space = self.gp_prior(patristic_matrix_sorted)
+        # Highlight: MAP the latent space to logits using the Decoder from a Seq2seq model with/without attention
+        latent_space = latent_space.repeat(1,self.align_seq_len).reshape(latent_space.shape[0],self.align_seq_len,self.z_dim) #[n_nodes,max_seq,z_dim]
+        decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],
+                                               self.gru_hidden_dim).contiguous()  # bidirectional
+
+        with pyro.plate("plate_len", aminoacid_sequences.shape[1], dim=-1), pyro.plate("plate_seq",aminoacid_sequences.shape[0], dim=-2):
+                logits = self.decoder.forward(
+                    input=latent_space,
+                    hidden=decoder_hidden)
+                pyro.sample("aa_sequences", dist.Categorical(logits=logits),obs=aminoacid_sequences)  # aa_seq = [n_nodes,align_seq_len]
+
+    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates):
+        if self.args.select_guide == "delta_map":
+            self.model_delta_map(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+        else:
+            self.model_variational(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
     def sample(self, map_estimates, n_samples, family_data_test, patristic_matrix,cladistic_matrix,use_argmax=False,use_test=True,use_test2=False):
         if use_test or use_test2:
             assert patristic_matrix[1:,1:].shape == (self.n_all,self.n_all)
             latent_space = self.conditional_sampling(map_estimates,patristic_matrix)
             n_nodes = self.n_internal #I had to split it up because of some weird data cases (coral), otherwise family_data_test.shape[0] would have sufficed
         else:
             latent_space = map_estimates["latent_z"].T
             assert latent_space.shape == (self.n_leaves, self.z_dim)
             n_nodes = self.n_leaves
 
         decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],self.gru_hidden_dim).contiguous()  # Not bidirectional
         latent_space_ = latent_space.repeat(1, self.align_seq_len).reshape(n_nodes,self.align_seq_len, self.z_dim)
 
-        with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2,subsample_size=n_nodes):
-            logits = self.decoder.forward(
-                input=latent_space_,
-                hidden=decoder_hidden)
-            if use_argmax:
-                #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
-                aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
-            else:
-                aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
+        #with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2,subsample_size=n_nodes):
+        logits = self.decoder.forward(
+            input=latent_space_,
+            hidden=decoder_hidden)
+        if use_argmax:
+            #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
+            aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
+        else:
+            aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
         #return aa_sequences,latent_space, logits, None, None
         sampling_out = SamplingOutput(aa_sequences=aa_sequences.detach(),
                                       latent_space=latent_space.detach(),
                                       logits=logits.detach(),
                                       phis=None,
                                       psis=None,
                                       mean_phi=None,
@@ -437,40 +497,66 @@
         self.decoder = RNNDecoder_Tiling(self.align_seq_len, self.aa_probs, self.gru_hidden_dim, self.z_dim, self.rnn_input_size,self.kappa_addition,self.num_layers,self.pretrained_params)
         self.embed = EmbedComplex(self.aa_probs,self.embedding_dim, self.pretrained_params)
         self.splitted_leaves_indexes = list(torch.tensor_split(torch.arange(self.n_leaves), int(self.n_leaves / self.plate_size)) * self.num_epochs)
         if self.plate_unordered:
             self.model = self.model_unordered
         else:
             self.model = self.model_ordered
-    def model_ordered(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum = None,guide_map_estimates=None):
+    def model_delta_map_ordered(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum = None,guide_map_estimates=None):
         aminoacid_sequences = family_data[:, 2:, 0]
         batch_nodes = family_data[:, 0, 1]
         #batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
         # Highlight: Register GRU module
         pyro.module("embeddings",self.embed)
         pyro.module("decoder", self.decoder)
         # Highlight: GP prior over the latent space
         latent_space = self.gp_prior(patristic_matrix_sorted)
         # Highlight: MAP the latent space to logits using the Decoder from a Seq2seq model with/without attention
         latent_space = latent_space.repeat(1,self.align_seq_len).reshape(latent_space.shape[0],self.align_seq_len,self.z_dim) #[n_nodes,max_seq,z_dim]
         blosum = self.blosum_weighted.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.align_seq_len,self.aa_probs) #[n_nodes,max_seq,21]
-        blosum = self.embed(blosum) #TODO: Introduce a noise variable to be able to deal with more random mutations?
+        blosum = self.embed(blosum)
         latent_space = torch.cat((latent_space,blosum),dim=2) #[n_nodes,align_seq_len,z_dim + 21]
 
         decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],
                                                self.gru_hidden_dim).contiguous()
 
         with pyro.plate("plate_len", aminoacid_sequences.shape[1], dim=-1):
             with pyro.plate("plate_seq", aminoacid_sequences.shape[0], dim=-2, subsample=self.splitted_leaves_indexes.pop(0)) as indx:  # Highlight: Ordered subsampling
                 logits = self.decoder.forward(
                     input=latent_space[indx],
                     hidden=decoder_hidden[:,indx])
                 pyro.sample("aa_sequences", dist.Categorical(logits=logits),obs=aminoacid_sequences[indx])  # aa_seq = [n_nodes,align_seq_len]
 
-    def model_unordered(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum = None,guide_map_estimates=None):
+    def model_variational_ordered(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum = None,guide_map_estimates=None):
+        aminoacid_sequences = family_data[:, 2:, 0]
+        batch_nodes = family_data[:, 0, 1]
+        #batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
+        # Highlight: Register GRU module
+        pyro.module("embeddings",self.embed)
+        pyro.module("decoder", self.decoder)
+        with pyro.plate("plate_batch", dim=-1, device=self.device):
+            # Highlight: GP prior over the latent space
+            latent_space = self.gp_prior(patristic_matrix_sorted)
+            # Highlight: MAP the latent space to logits using the Decoder from a Seq2seq model with/without attention
+            latent_space = latent_space.repeat(1,self.align_seq_len).reshape(latent_space.shape[0],self.align_seq_len,self.z_dim) #[n_nodes,max_seq,z_dim]
+            blosum = self.blosum_weighted.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.align_seq_len,self.aa_probs) #[n_nodes,max_seq,21]
+            blosum = self.embed(blosum)
+            latent_space = torch.cat((latent_space,blosum),dim=2) #[n_nodes,align_seq_len,z_dim + 21]
+
+            decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],
+                                                   self.gru_hidden_dim).contiguous()
+
+            with pyro.plate("plate_len", aminoacid_sequences.shape[1], dim=-1):
+                with pyro.plate("plate_seq", aminoacid_sequences.shape[0], dim=-2, subsample=self.splitted_leaves_indexes.pop(0)) as indx:  # Highlight: Ordered subsampling
+                    logits = self.decoder.forward(
+                        input=latent_space[indx],
+                        hidden=decoder_hidden[:,indx])
+                    pyro.sample("aa_sequences", dist.Categorical(logits=logits),obs=aminoacid_sequences[indx])  # aa_seq = [n_nodes,align_seq_len]
+
+    def model_delta_map_unordered(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum = None,guide_map_estimates=None):
         aminoacid_sequences = family_data[:, 2:, 0]
         batch_nodes = family_data[:, 0, 1]
         #batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
         # Highlight: Register GRU module
         pyro.module("embeddings",self.embed)
         pyro.module("decoder", self.decoder)
         # Highlight: GP prior over the latent space
@@ -488,14 +574,32 @@
             with pyro.plate("plate_seq",aminoacid_sequences.shape[0],dim=-2,subsample_size=self.plate_size) as indx:#Highlight: Random subsampling
             #with pyro.plate("plate_seq", aminoacid_sequences.shape[0], dim=-2,subsample=self.splitted_leaves_indexes.pop(0)) as indx:  # Highlight: Ordered subsampling
                 logits = self.decoder.forward(
                     input=latent_space[indx],
                     hidden=decoder_hidden[:,indx])
                 pyro.sample("aa_sequences", dist.Categorical(logits=logits),obs=aminoacid_sequences[indx])  # aa_seq = [n_nodes,align_seq_len]
 
+    def model(self, family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum, batch_blosum,
+              guide_map_estimates):
+        if self.args.select_guide == "delta_map":
+            if self.args.plate_unordered:
+                self.model_delta_map_unordered(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,
+                                     batch_blosum, guide_map_estimates)
+            else:
+                self.model_delta_map_ordered(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,
+                                     batch_blosum, guide_map_estimates)
+        else:
+            raise ValueError("Under construction")
+            if self.args.plate_unordered:
+                self.model_variationl_unordered(sfamily_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,
+                                     batch_blosum, guide_map_estimates)
+            else:
+                self.model_variational_ordered(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,
+                                       batch_blosum, guide_map_estimates)
+
     def sample(self, map_estimates, n_samples, family_data_test, patristic_matrix,cladistic_matrix,use_argmax=False,use_test=True,use_test2=False):
         if use_test or use_test2:
             assert patristic_matrix[1:,1:].shape == (self.n_all,self.n_all)
             latent_space = self.conditional_sampling(map_estimates,patristic_matrix)
             n_nodes = self.n_internal #I had to split it up because of some weird data cases (coral), otherwise family_data_test.shape[0] would have sufficed
         else:
             latent_space = map_estimates["latent_z"].T
@@ -537,15 +641,15 @@
     def __init__(self,ModelLoad):
         DRAUPNIRModelClass.__init__(self,ModelLoad)
         self.rnn_input_size = self.z_dim + self.aa_probs
         self.decoder = RNNDecoder_Tiling(self.align_seq_len, self.aa_probs, self.gru_hidden_dim, self.z_dim, self.rnn_input_size,self.kappa_addition,self.num_layers,self.pretrained_params)
         self.embed = EmbedComplex(self.aa_probs,self.embedding_dim, self.pretrained_params)
         self.internal_nodes_batch = None
         self.n_leaves_internal_batch = None
-    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates=None):
+    def model_delta_map(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates=None):
         aminoacid_sequences = family_data[:, 2:, 0]
         batch_nodes = family_data[:, 0, 1]
         batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
         # Highlight: Register GRU module
         pyro.module("embeddings",self.embed)
         pyro.module("decoder", self.decoder)
         # Highlight: GP prior over the latent space
@@ -559,14 +663,41 @@
         decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],
                                                self.gru_hidden_dim).contiguous()  # bidirectional
         with pyro.plate("plate_len", aminoacid_sequences.shape[1], dim=-1), pyro.plate("plate_seq",aminoacid_sequences.shape[0],dim=-2):
             logits = self.decoder.forward(
                     input=latent_space,
                     hidden=decoder_hidden)
             pyro.sample("aa_sequences", dist.Categorical(logits=logits), obs=aminoacid_sequences) #aa_seq = [n_nodes,max_seq_len]
+    def model_variational(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates=None):
+        aminoacid_sequences = family_data[:, 2:, 0]
+        batch_nodes = family_data[:, 0, 1]
+        batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
+        # Highlight: Register GRU module
+        pyro.module("embeddings",self.embed)
+        pyro.module("decoder", self.decoder)
+        # Highlight: GP prior over the latent space
+        latent_space = self.gp_prior_batched(patristic_matrix_sorted)
+        # Highlight: MAP the latent space to logits using the Decoder from a Seq2seq model with/without attention
+        latent_space = latent_space.repeat(1,self.align_seq_len).reshape(latent_space.shape[0],self.align_seq_len,self.z_dim) #[n_nodes,max_seq,z_dim]
+        blosum = self.blosum_weighted.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.align_seq_len,self.aa_probs) #[n_nodes,max_seq,21] #Highlight: it workedwith the entire blosum weighted matrix
+        #blosum = batch_blosum.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.max_seq_len,self.aa_prob) #[n_nodes,max_seq,21] #only use the weighted average of the batch sequences
+        blosum = self.embed(blosum)
+        latent_space = torch.cat((latent_space,blosum),dim=2) #[n_nodes,max_seq_len,z_dim + 21]
+        decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],
+                                               self.gru_hidden_dim).contiguous()  # bidirectional
+        with pyro.plate("plate_len", aminoacid_sequences.shape[1], dim=-1), pyro.plate("plate_seq",aminoacid_sequences.shape[0],dim=-2):
+            logits = self.decoder.forward(
+                    input=latent_space,
+                    hidden=decoder_hidden)
+            pyro.sample("aa_sequences", dist.Categorical(logits=logits), obs=aminoacid_sequences) #aa_seq = [n_nodes,max_seq_len]
+    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates):
+        if self.args.select_guide == "delta_map":
+            self.model_delta_map(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+        else:
+            self.model_variational(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
 
     def sample(self, map_estimates, n_samples, family_data_test, patristic_matrix,cladistic_matrix,use_argmax=False,use_test=True,use_test2=False):
         """Samples using all sequences, which is not computationally feasible if there is a high number of sequences"""
         if use_test2: #MAP estimate
             assert patristic_matrix[1:,1:].shape == (self.n_all,self.n_all)
             latent_space = self.conditional_samplingMAP(map_estimates,patristic_matrix)
             n_nodes = self.n_internal #I had to split it up because of some weird data cases (coral), otherwise family_data_test.shape[0] would have sufficed
@@ -581,23 +712,23 @@
 
         decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],self.gru_hidden_dim).contiguous()  # Not bidirectional
         latent_space_ = latent_space.repeat(1, self.max_seq_len).reshape(n_nodes,self.align_seq_len, self.z_dim)
         blosum = self.blosum_weighted.repeat(latent_space_.shape[0], 1).reshape(latent_space_.shape[0], self.align_seq_len,self.aa_probs)  # [n_nodes,max_seq,21]
         blosum = self.embed(blosum)
         latent_space_ = torch.cat((latent_space_, blosum), dim=2)  # [n_nodes,max_seq_len,z_dim + 21]
 
-        with pyro.plate("plate_len",self.max_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2):
-            logits = self.decoder.forward(
-                input=latent_space_,
-                hidden=decoder_hidden)
-            if use_argmax:
-                #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
-                aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
-            else:
-                aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
+        #with pyro.plate("plate_len",self.max_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2):
+        logits = self.decoder.forward(
+            input=latent_space_,
+            hidden=decoder_hidden)
+        if use_argmax:
+            #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
+            aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
+        else:
+            aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
         #return aa_sequences,latent_space, logits, None, None
         sampling_out = SamplingOutput(aa_sequences=aa_sequences.detach(),
                                       latent_space=latent_space.detach(),
                                       logits=logits.detach(),
                                       phis=None,
                                       psis=None,
                                       mean_phi=None,
@@ -664,15 +795,15 @@
     Clade batch training and sampling."""
     def __init__(self,ModelLoad):
         DRAUPNIRModelClass.__init__(self,ModelLoad)
         self.rnn_input_size = self.z_dim + self.aa_probs
         #self.decoder_attention = RNNAttentionDecoder(self.n_leaves, self.max_seq_len, self.aa_prob, self.gru_hidden_dim,self.rnn_input_size,self.embedding_dim, self.z_dim, self.kappa_addition)
         self.decoder = RNNDecoder_Tiling(self.align_seq_len, self.aa_probs, self.gru_hidden_dim, self.z_dim, self.rnn_input_size,self.kappa_addition,self.num_layers,self.pretrained_params)
         self.embed = EmbedComplex(self.aa_probs,self.embedding_dim, self.pretrained_params)
-    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates=None):
+    def model_delta_map(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates=None):
         aminoacid_sequences = family_data[:, 2:, 0]
         #batch_nodes = family_data[:, 0, 1]
         #batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
         # Highlight: Register GRU module
         pyro.module("embeddings",self.embed)
         pyro.module("decoder", self.decoder)
         self.n_leaves_batch = family_data.shape[0]
@@ -690,14 +821,47 @@
                                                self.gru_hidden_dim).contiguous()  # bidirectional
         with pyro.plate("plate_len", aminoacid_sequences.shape[1], dim=-1), pyro.plate("plate_seq",aminoacid_sequences.shape[0],dim=-2):
             logits = self.decoder.forward(
                     input=batch_latent_space,
                     hidden=decoder_hidden)
             pyro.sample("aa_sequences", dist.Categorical(logits=logits), obs=aminoacid_sequences) #aa_seq = [n_nodes,max_seq_len]
 
+    def model_variational(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates=None):
+        aminoacid_sequences = family_data[:, 2:, 0]
+        #batch_nodes = family_data[:, 0, 1]
+        #batch_indexes = (patristic_matrix_sorted[1:, 0][..., None] == batch_nodes).any(-1)
+        # Highlight: Register GRU module
+        pyro.module("embeddings",self.embed)
+        pyro.module("decoder", self.decoder)
+        self.n_leaves_batch = family_data.shape[0]
+        with pyro.plate("plate_batch", dim=-1, device=self.device):
+            # Highlight: GP prior over the latent space of all the leaves
+            latent_space = self.gp_prior_batched(patristic_matrix_sorted) #TODO: make a function model and one model_batched?
+            # Highlight: MAP the latent space to logits using the Decoder from a Seq2seq model with/without attention
+            latent_space = latent_space.repeat(1,self.align_seq_len).reshape(latent_space.shape[0],self.align_seq_len,self.z_dim) #[n_nodes,max_seq,z_dim]
+            #blosum = batch_blosum.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.max_seq_len,self.aa_prob) #[n_nodes,max_seq,21]
+            blosum = self.blosum_weighted.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.align_seq_len,self.aa_probs) #[n_nodes,max_seq,21]
+            blosum = self.embed(blosum)
+            batch_latent_space = torch.cat((latent_space,blosum),dim=2) #[n_nodes,max_seq_len,z_dim + 21]
+            #batch_latent_space = latent_space[batch_indexes] #Highlight: For plating; In order to reduce the load on the GRU memory we split the latent space of the leaves by clades/batch
+            decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2,
+                                                   batch_latent_space.shape[0],
+                                                   self.gru_hidden_dim).contiguous()  # bidirectional
+            with pyro.plate("plate_len", dim=-2):
+                logits = self.decoder.forward(
+                        input=batch_latent_space,
+                        hidden=decoder_hidden)
+                pyro.sample("aa_sequences", dist.Categorical(logits=logits), obs=aminoacid_sequences) #aa_seq = [n_nodes,max_seq_len]
+
+    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates):
+        if self.args.select_guide == "delta_map":
+            self.model_delta_map(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+        else:
+            self.model_variational(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+
     def sample(self, map_estimates, n_samples, family_data_test, patristic_matrix,cladistic_matrix,use_argmax=False,use_test=True,use_test2=False):
         """Full latent space inference, plating sequences by clade"""
         if use_test:
             assert patristic_matrix[1:,1:].shape == (self.n_all,self.n_all)
             latent_space = self.conditional_sampling(map_estimates,patristic_matrix)
             n_nodes = self.n_internal #DO NOT REMOVE: I had to write this line because of some weird data cases (coral dataset), otherwise family_data_test.shape[0] would have sufficed
         elif use_test2:
@@ -711,22 +875,22 @@
 
         decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],self.gru_hidden_dim).contiguous()  # Not bidirectional
         latent_space_extended = latent_space.repeat(1, self.align_seq_len).reshape(n_nodes,self.align_seq_len, self.z_dim)
         blosum = self.blosum_weighted.repeat(latent_space_extended.shape[0], 1).reshape(latent_space_extended.shape[0], self.align_seq_len,self.aa_probs)  # [n_nodes,max_seq,21]
         blosum = self.embed(blosum)
         latent_space_extended = torch.cat((latent_space_extended, blosum), dim=2)  # [n_nodes,max_seq_len,z_dim + 21]
 
-        with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2):
-            logits = self.decoder.forward(
-                    input=latent_space_extended,
-                    hidden=decoder_hidden)
-            if use_argmax: #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
-                aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
-            else:
-                aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
+        #with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2):
+        logits = self.decoder.forward(
+                input=latent_space_extended,
+                hidden=decoder_hidden)
+        if use_argmax: #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
+            aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
+        else:
+            aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
         sampling_out = SamplingOutput(aa_sequences=aa_sequences.detach(),
                                       latent_space=latent_space.detach(),
                                       logits=logits.detach(),
                                       phis=None,
                                       psis=None,
                                       mean_phi=None,
                                       mean_psi=None,
@@ -791,15 +955,15 @@
     """Leaves training and testing. Train on full leave latent space (train + test), only observe the pre-selected train leaves"""
     def __init__(self,ModelLoad):
         DRAUPNIRModelClass.__init__(self,ModelLoad)
         self.rnn_input_size = self.z_dim + self.aa_probs
         #self.decoder_attention = RNNAttentionDecoder(self.n_leaves, self.align_seq_len, self.aa_probs, self.gru_hidden_dim,self.rnn_input_size,self.embedding_dim, self.z_dim, self.kappa_addition)
         self.decoder = RNNDecoder_Tiling(self.align_seq_len, self.aa_probs, self.gru_hidden_dim, self.z_dim, self.rnn_input_size,self.kappa_addition,self.num_layers,self.pretrained_params)
         self.embed = EmbedComplex(self.aa_probs,self.embedding_dim, self.pretrained_params)
-    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
+    def model_delta_map(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
         aminoacid_sequences = family_data[:, 2:, 0]
         #angles = family_data[:, 2:, 1:3]
         train_nodes = family_data[:, 0, 1]
         train_indexes = (patristic_matrix_sorted[1:, 0][..., None] == train_nodes).any(-1)
         # Highlight: Register GRU module
         pyro.module("embeddings",self.embed)
         pyro.module("decoder", self.decoder)
@@ -818,14 +982,47 @@
             logits = self.decoder.forward(
                     input=latent_space,
                     hidden=decoder_hidden)
             #Highlight: Observe only some of the leaves
             logits = logits[train_indexes]
             pyro.sample("aa_sequences", dist.Categorical(logits=logits), obs=aminoacid_sequences) #aa_seq = [n_nodes,align_seq_len]
 
+    def model_variational(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
+        aminoacid_sequences = family_data[:, 2:, 0]
+        #angles = family_data[:, 2:, 1:3]
+        train_nodes = family_data[:, 0, 1]
+        train_indexes = (patristic_matrix_sorted[1:, 0][..., None] == train_nodes).any(-1)
+        # Highlight: Register GRU module
+        pyro.module("embeddings",self.embed)
+        pyro.module("decoder", self.decoder)
+        with pyro.plate("plate_batch", dim=-1, device=self.device):
+            # Highlight: GP prior over the latent space of all the leaves
+            latent_space = self.gp_prior(patristic_matrix_sorted)
+            # Highlight: MAP the latent space to logits using the Decoder from a Seq2seq model with/without attention
+            latent_space = latent_space.repeat(1,self.align_seq_len).reshape(latent_space.shape[0],self.align_seq_len,self.z_dim) #[n_nodes,max_seq,z_dim]
+            blosum = self.blosum_weighted.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.align_seq_len,self.aa_probs) #[n_nodes,max_seq,21]
+            blosum = self.embed(blosum)
+            latent_space = torch.cat((latent_space,blosum),dim=2) #[n_nodes,align_seq_len,z_dim + 21]
+            decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2,
+                                                   latent_space.shape[0],
+                                                   self.gru_hidden_dim).contiguous()  # bidirectional
+            with pyro.plate("plate_len", dim=-2):
+                logits = self.decoder.forward(
+                        input=latent_space,
+                        hidden=decoder_hidden)
+                #Highlight: Observe only some of the leaves
+                logits = logits[train_indexes]
+                pyro.sample("aa_sequences", dist.Categorical(logits=logits), obs=aminoacid_sequences) #aa_seq = [n_nodes,align_seq_len]
+
+    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates):
+        if self.args.select_guide == "delta_map":
+            self.model_delta_map(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+        else:
+            self.model_variational(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+
     def sample(self, map_estimates, n_samples, family_data_test, patristic_matrix,cladistic_matrix,use_argmax=False,use_test=True,use_test2=False):
         if use_test2:
             assert patristic_matrix[1:,1:].shape == (self.n_all,self.n_all)
             latent_space = self.conditional_sampling(map_estimates,patristic_matrix)
             n_nodes = self.n_internal #DO NOT REMOVE: I had to write this line because of some weird data cases (coral dataset), otherwise family_data_test.shape[0] would have sufficed
         elif use_test:
             #latent_space = self.conditional_sampling_descendants(map_estimates,patristic_matrix)
@@ -841,26 +1038,26 @@
 
         decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2, latent_space.shape[0],self.gru_hidden_dim).contiguous()  # Not bidirectional
         latent_space_extended = latent_space.repeat(1, self.align_seq_len).reshape(n_nodes,self.align_seq_len, self.z_dim)
         blosum = self.blosum_weighted.repeat(latent_space_extended.shape[0], 1).reshape(latent_space_extended.shape[0], self.align_seq_len,self.aa_probs)  # [n_nodes,max_seq,21]
         blosum = self.embed(blosum)
         latent_space_extended = torch.cat((latent_space_extended, blosum), dim=2)  # [n_nodes,align_seq_len,z_dim + 21]
 
-        with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2):
-            logits = self.decoder.forward(
-                    input=latent_space_extended,
-                    hidden=decoder_hidden)
+        #with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2):
+        logits = self.decoder.forward(
+                input=latent_space_extended,
+                hidden=decoder_hidden)
 
-            # batch_nodes = family_data_test[:, 0, 1]
-            # batch_indexes = (patristic_matrix[1:, 0][..., None] == batch_nodes).any(-1)
-            # batch_logits = logits[batch_indexes]
-            if use_argmax: #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
-                aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
-            else:
-                aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
+        # batch_nodes = family_data_test[:, 0, 1]
+        # batch_indexes = (patristic_matrix[1:, 0][..., None] == batch_nodes).any(-1)
+        # batch_logits = logits[batch_indexes]
+        if use_argmax: #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
+            aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
+        else:
+            aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
         #return aa_sequences,latent_space, logits, None, None
         sampling_out = SamplingOutput(aa_sequences=aa_sequences.detach(),
                                       latent_space=latent_space.detach(),
                                       logits=logits.detach(),
                                       phis=None,
                                       psis=None,
                                       mean_phi=None,
@@ -874,15 +1071,15 @@
     """Leaves training and testing.Predicting both ANGLES and AA sequences. Working on full or partial leaves space depending on the
     leaves_testing argument stated in datasets.py"""
     def __init__(self,ModelLoad):
         DRAUPNIRModelClass.__init__(self,ModelLoad)
         self.rnn_input_size = self.z_dim + self.aa_probs
         self.decoder = RNNDecoder_Tiling_Angles(self.align_seq_len, self.aa_probs, self.gru_hidden_dim, self.z_dim, self.rnn_input_size,self.kappa_addition,self.num_layers,self.pretrained_params)
         self.embed = EmbedComplex(self.aa_probs,self.embedding_dim, self.pretrained_params)
-    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
+    def model_delta_map(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
         aminoacid_sequences = family_data[:, 2:, 0]
         angles = family_data[:, 2:, 1:3]
         angles_mask = torch.where(angles == 0., angles, 1.).type(angles.dtype) #keep as 0 the gaps and set to 1 where there is an observation
         train_nodes = family_data[:, 0, 1]
         train_indexes = (patristic_matrix_sorted[1:, 0][..., None] == train_nodes).any(-1)
         # Highlight: Register GRU module
         pyro.module("embeddings",self.embed)
@@ -907,14 +1104,53 @@
             logits = logits[train_indexes]
             means = means[train_indexes]
             kappas = kappas[train_indexes]
             pyro.sample("aa_sequences", dist.Categorical(logits=logits), obs=aminoacid_sequences) #aa_seq = [n_nodes,align_seq_len]
             pyro.sample("phi",dist.VonMises(loc = means[:,:,0],concentration = kappas[:,:,0]).mask(angles_mask), obs=angles[:,:,0])
             pyro.sample("psi",dist.VonMises(loc = means[:,:,1],concentration = kappas[:,:,1]).mask(angles_mask), obs=angles[:,:,1])
 
+    def model_variational(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum=None,guide_map_estimates=None):
+        aminoacid_sequences = family_data[:, 2:, 0]
+        angles = family_data[:, 2:, 1:3]
+        angles_mask = torch.where(angles == 0., angles, 1.).type(angles.dtype) #keep as 0 the gaps and set to 1 where there is an observation
+        train_nodes = family_data[:, 0, 1]
+        train_indexes = (patristic_matrix_sorted[1:, 0][..., None] == train_nodes).any(-1)
+        # Highlight: Register GRU module
+        pyro.module("embeddings",self.embed)
+        pyro.module("decoder", self.decoder)
+        with pyro.plate("plate_batch", dim=-1, device=self.device):
+            # Highlight: GP prior over the latent space of all the leaves
+            latent_space = self.gp_prior(patristic_matrix_sorted)
+            # Highlight: MAP the latent space to logits using the Decoder from a Seq2seq model with/without attention
+
+            latent_space = latent_space.repeat(1,self.align_seq_len).reshape(latent_space.shape[0],self.align_seq_len,self.z_dim) #[n_nodes,max_seq,z_dim]
+
+            blosum = self.blosum_weighted.repeat(latent_space.shape[0],1).reshape(latent_space.shape[0],self.align_seq_len,self.aa_probs) #[n_nodes,max_seq,21]
+            blosum = self.embed(blosum)
+            latent_space = torch.cat((latent_space,blosum),dim=2) #[n_nodes,align_seq_len,z_dim + 21]
+            decoder_hidden = self.h_0_MODEL.expand(self.decoder.num_layers * 2,
+                                                   latent_space.shape[0],
+                                                   self.gru_hidden_dim).contiguous()  # bidirectional
+            with pyro.plate("plate_len", dim=-2):
+                logits,means,kappas = self.decoder.forward(
+                    input=latent_space,
+                    hidden=decoder_hidden)
+                logits = logits[train_indexes]
+                means = means[train_indexes]
+                kappas = kappas[train_indexes]
+                pyro.sample("aa_sequences", dist.Categorical(logits=logits), obs=aminoacid_sequences) #aa_seq = [n_nodes,align_seq_len]
+                pyro.sample("phi",dist.VonMises(loc = means[:,:,0],concentration = kappas[:,:,0]).mask(angles_mask), obs=angles[:,:,0])
+                pyro.sample("psi",dist.VonMises(loc = means[:,:,1],concentration = kappas[:,:,1]).mask(angles_mask), obs=angles[:,:,1])
+
+    def model(self, family_data, patristic_matrix_sorted,cladistic_matrix,data_blosum,batch_blosum,guide_map_estimates):
+        if self.args.select_guide == "delta_map":
+            self.model_delta_map(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+        else:
+            self.model_variational(family_data, patristic_matrix_sorted, cladistic_matrix, data_blosum,batch_blosum, guide_map_estimates)
+
     def sample(self, map_estimates, n_samples, family_data_test, patristic_matrix,cladistic_matrix,use_argmax=False,use_test=True,use_test2=False):
         if use_test:
             #latent_space = self.conditional_sampling_descendants(map_estimates,patristic_matrix)
             latent_space = self.map_sampling(map_estimates,patristic_matrix)
             n_nodes = self.n_internal
         elif use_test2:
             assert patristic_matrix[1:,1:].shape == (self.n_all,self.n_all)
@@ -934,26 +1170,26 @@
                                                self.gru_hidden_dim).contiguous()  # Contains 2 hidden states in 1, to be processed by different GRU/SRUs
 
         latent_space_extended = latent_space.repeat(1, self.align_seq_len).reshape(n_nodes,self.align_seq_len, self.z_dim)
         blosum = self.blosum_weighted.repeat(latent_space_extended.shape[0], 1).reshape(latent_space_extended.shape[0], self.align_seq_len,self.aa_probs)  # [n_nodes,max_seq,21]
         blosum = self.embed(blosum)
         latent_space_extended = torch.cat((latent_space_extended, blosum), dim=2)  # [n_nodes,align_seq_len,z_dim + 21]
 
-        with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2):
+        #with pyro.plate("plate_len",self.align_seq_len, dim=-1), pyro.plate("plate_seq",n_nodes,dim=-2):
 
-            logits,means,kappas = self.decoder.forward(
-                input=latent_space_extended,
-                hidden=decoder_hidden)
+        logits,means,kappas = self.decoder.forward(
+            input=latent_space_extended,
+            hidden=decoder_hidden)
 
-            if use_argmax: #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
-                aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
-            else:
-                aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
-            phis = dist.VonMises(loc=means[:,:,0],concentration = kappas[:,:,0]).sample([n_samples])
-            psis = dist.VonMises(loc=means[:,:,1],concentration = kappas[:,:,1]).sample([n_samples])
+        if use_argmax: #Pick the sequence with the highest likelihood, now n_samples, n_samples = 1
+            aa_sequences = torch.argmax(logits,dim=2).unsqueeze(0) #I add one dimension at the beginning to resemble 1 sample and not have to change all the plotting code
+        else:
+            aa_sequences = dist.Categorical(logits=logits).sample([n_samples])
+        phis = dist.VonMises(loc=means[:,:,0],concentration = kappas[:,:,0]).sample([n_samples])
+        psis = dist.VonMises(loc=means[:,:,1],concentration = kappas[:,:,1]).sample([n_samples])
 
         sampling_out = SamplingOutput(aa_sequences=aa_sequences.detach(),
                                       latent_space=latent_space.detach(),
                                       logits=logits.detach(),
                                       phis=phis.detach(),
                                       psis=psis.detach(),
                                       mean_phi = means[:,:,0].detach(),
```

### Comparing `draupnir-0.0.29/src/draupnir/models_utils.py` & `draupnir-0.0.30/src/draupnir/models_utils.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/mutual_information.py` & `draupnir-0.0.30/src/draupnir/mutual_information.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/plots.py` & `draupnir-0.0.30/src/draupnir/plots.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/train.py` & `draupnir-0.0.30/src/draupnir/train.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir/utils.py` & `draupnir-0.0.30/src/draupnir/utils.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/src/draupnir.egg-info/PKG-INFO` & `draupnir-0.0.30/src/draupnir.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: draupnir
-Version: 0.0.29
+Version: 0.0.30
 Summary: Ancestral sequence reconstruction using a tree structured Ornstein Uhlenbeck variational autoencoder
 Home-page: https://github.com/LysSanzMoreta/DRAUPNIR_ASR
 Author: Lys Sanz Moreta
 Author-email: lys.sanz.moreta@outlook.com
 Project-URL: Changelog, https://github.com/LysSanzMoreta/DRAUPNIR_ASR/blob/master/CHANGELOG.rst
 Project-URL: Issue Tracker, https://github.com/LysSanzMoreta/DRAUPNIR_ASR/issues
 Classifier: Development Status :: 4 - Beta
@@ -187,14 +187,16 @@
   year={2021}
 }
 ```
 
 
 **Do not hesitate to give input on how to improve the documentation of this library**
 
+**Leave like and subscribe ... wait that was somewhere else ... well, a star will do it ;) **
+
```

### Comparing `draupnir-0.0.29/src/draupnir.egg-info/SOURCES.txt` & `draupnir-0.0.30/src/draupnir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/tests/test_accuracy.py` & `draupnir-0.0.30/tests/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/tests/test_examples.py` & `draupnir-0.0.30/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/tests/test_load.py` & `draupnir-0.0.30/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `draupnir-0.0.29/tests/test_norworking.py` & `draupnir-0.0.30/tests/test_norworking.py`

 * *Files identical despite different names*

