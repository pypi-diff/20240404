# Comparing `tmp/signapse-1.0.2.tar.gz` & `tmp/signapse-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.2.tar", last modified: Thu Apr  4 11:25:42 2024, max compression
+gzip compressed data, was "signapse-1.0.3.tar", last modified: Thu Apr  4 12:29:00 2024, max compression
```

## Comparing `signapse-1.0.2.tar` & `signapse-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:25:42.047058 signapse-1.0.2/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.2/LICENSE.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      619 2024-04-04 11:25:42.047058 signapse-1.0.2/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      240 2024-04-04 09:58:36.000000 signapse-1.0.2/README.md
--rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 11:25:42.047058 signapse-1.0.2/setup.cfg
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1176 2024-04-04 11:24:45.000000 signapse-1.0.2/setup.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:25:42.047058 signapse-1.0.2/signapse/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.2/signapse/__init__.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.2/signapse/build_opt.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.2/signapse/compute.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.2/signapse/constants.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.2/signapse/create.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.2/signapse/create_model.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.2/signapse/heatmaps.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.2/signapse/lang_sam.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.2/signapse/lang_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.2/signapse/models_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.2/signapse/mp_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.2/signapse/poses.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.2/signapse/preprocessing.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.2/signapse/utils.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:25:42.047058 signapse-1.0.2/signapse.egg-info/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      619 2024-04-04 11:25:41.000000 signapse-1.0.2/signapse.egg-info/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 11:25:42.000000 signapse-1.0.2/signapse.egg-info/SOURCES.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 11:25:41.000000 signapse-1.0.2/signapse.egg-info/dependency_links.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      223 2024-04-04 11:25:41.000000 signapse-1.0.2/signapse.egg-info/requires.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 11:25:41.000000 signapse-1.0.2/signapse.egg-info/top_level.txt
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:29:00.676382 signapse-1.0.3/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.3/LICENSE.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      865 2024-04-04 12:29:00.676382 signapse-1.0.3/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      240 2024-04-04 09:58:36.000000 signapse-1.0.3/README.md
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 12:29:00.676382 signapse-1.0.3/setup.cfg
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1296 2024-04-04 12:28:45.000000 signapse-1.0.3/setup.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:29:00.676382 signapse-1.0.3/signapse/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.3/signapse/__init__.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.3/signapse/build_opt.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.3/signapse/compute.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.3/signapse/constants.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.3/signapse/create.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.3/signapse/create_model.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.3/signapse/heatmaps.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.3/signapse/lang_sam.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.3/signapse/lang_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.3/signapse/models_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.3/signapse/mp_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.3/signapse/poses.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.3/signapse/preprocessing.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.3/signapse/utils.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:29:00.676382 signapse-1.0.3/signapse.egg-info/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      865 2024-04-04 12:29:00.000000 signapse-1.0.3/signapse.egg-info/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 12:29:00.000000 signapse-1.0.3/signapse.egg-info/SOURCES.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 12:29:00.000000 signapse-1.0.3/signapse.egg-info/dependency_links.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      223 2024-04-04 12:29:00.000000 signapse-1.0.3/signapse.egg-info/requires.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 12:29:00.000000 signapse-1.0.3/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.2/LICENSE.txt` & `signapse-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/setup.py` & `signapse-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from setuptools import setup, find_packages
 
+with open("README.md","r") as ofile:
+    long_description_file = ofile.read()
+    
 setup(
     name='signapse',
-    version='1.0.2',
+    version='1.0.3',
     description='Signapse_synthetic_signer',
-    long_description='Signapse_synthetic_signer package',
+    long_description=long_description_file,
+    long_description_content_type="text/markdown",
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Developers',
```

### Comparing `signapse-1.0.2/signapse/build_opt.py` & `signapse-1.0.3/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/compute.py` & `signapse-1.0.3/signapse/compute.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/constants.py` & `signapse-1.0.3/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/create.py` & `signapse-1.0.3/signapse/create.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/create_model.py` & `signapse-1.0.3/signapse/create_model.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/heatmaps.py` & `signapse-1.0.3/signapse/heatmaps.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/lang_sam.py` & `signapse-1.0.3/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/lang_utils.py` & `signapse-1.0.3/signapse/lang_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/models_utils.py` & `signapse-1.0.3/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/mp_utils.py` & `signapse-1.0.3/signapse/mp_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/poses.py` & `signapse-1.0.3/signapse/poses.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/preprocessing.py` & `signapse-1.0.3/signapse/preprocessing.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.2/signapse/utils.py` & `signapse-1.0.3/signapse/utils.py`

 * *Files identical despite different names*

