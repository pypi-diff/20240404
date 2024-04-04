# Comparing `tmp/signapse-1.0.5.tar.gz` & `tmp/signapse-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.5.tar", last modified: Thu Apr  4 12:44:19 2024, max compression
+gzip compressed data, was "signapse-1.0.6.tar", last modified: Thu Apr  4 12:52:32 2024, max compression
```

## Comparing `signapse-1.0.5.tar` & `signapse-1.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:44:19.625991 signapse-1.0.5/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.5/LICENSE.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9479 2024-04-04 12:44:19.621991 signapse-1.0.5/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     8854 2024-04-04 12:42:27.000000 signapse-1.0.5/README.md
--rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 12:44:19.625991 signapse-1.0.5/setup.cfg
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1296 2024-04-04 12:43:51.000000 signapse-1.0.5/setup.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:44:19.621991 signapse-1.0.5/signapse/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.5/signapse/__init__.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.5/signapse/build_opt.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.5/signapse/compute.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.5/signapse/constants.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.5/signapse/create.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.5/signapse/create_model.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.5/signapse/heatmaps.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.5/signapse/lang_sam.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.5/signapse/lang_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.5/signapse/models_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.5/signapse/mp_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.5/signapse/poses.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.5/signapse/preprocessing.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.5/signapse/utils.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:44:19.621991 signapse-1.0.5/signapse.egg-info/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9479 2024-04-04 12:44:19.000000 signapse-1.0.5/signapse.egg-info/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 12:44:19.000000 signapse-1.0.5/signapse.egg-info/SOURCES.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 12:44:19.000000 signapse-1.0.5/signapse.egg-info/dependency_links.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      223 2024-04-04 12:44:19.000000 signapse-1.0.5/signapse.egg-info/requires.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 12:44:19.000000 signapse-1.0.5/signapse.egg-info/top_level.txt
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:52:32.496654 signapse-1.0.6/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.6/LICENSE.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3824 2024-04-04 12:52:32.496654 signapse-1.0.6/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3199 2024-04-04 12:51:00.000000 signapse-1.0.6/README.md
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 12:52:32.496654 signapse-1.0.6/setup.cfg
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1296 2024-04-04 12:52:28.000000 signapse-1.0.6/setup.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:52:32.496654 signapse-1.0.6/signapse/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.6/signapse/__init__.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.6/signapse/build_opt.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.6/signapse/compute.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.6/signapse/constants.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.6/signapse/create.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.6/signapse/create_model.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.6/signapse/heatmaps.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.6/signapse/lang_sam.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.6/signapse/lang_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.6/signapse/models_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.6/signapse/mp_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.6/signapse/poses.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.6/signapse/preprocessing.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.6/signapse/utils.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:52:32.496654 signapse-1.0.6/signapse.egg-info/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3824 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/SOURCES.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/dependency_links.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      223 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/requires.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.5/LICENSE.txt` & `signapse-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/setup.py` & `signapse-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as ofile:
     long_description_file = ofile.read()
     
 setup(
     name='signapse',
-    version='1.0.5',
+    version='1.0.6',
     description='Signapse_synthetic_signer',
     long_description=long_description_file,
     long_description_content_type="text/markdown",
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
```

### Comparing `signapse-1.0.5/signapse/build_opt.py` & `signapse-1.0.6/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/compute.py` & `signapse-1.0.6/signapse/compute.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/constants.py` & `signapse-1.0.6/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/create.py` & `signapse-1.0.6/signapse/create.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/create_model.py` & `signapse-1.0.6/signapse/create_model.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/heatmaps.py` & `signapse-1.0.6/signapse/heatmaps.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/lang_sam.py` & `signapse-1.0.6/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/lang_utils.py` & `signapse-1.0.6/signapse/lang_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/models_utils.py` & `signapse-1.0.6/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/mp_utils.py` & `signapse-1.0.6/signapse/mp_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/poses.py` & `signapse-1.0.6/signapse/poses.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/preprocessing.py` & `signapse-1.0.6/signapse/preprocessing.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.5/signapse/utils.py` & `signapse-1.0.6/signapse/utils.py`

 * *Files identical despite different names*

