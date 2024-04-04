# Comparing `tmp/signapse-1.0.7.tar.gz` & `tmp/signapse-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.7.tar", last modified: Thu Apr  4 13:54:25 2024, max compression
+gzip compressed data, was "signapse-1.0.8.tar", last modified: Thu Apr  4 14:03:05 2024, max compression
```

## Comparing `signapse-1.0.7.tar` & `signapse-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 13:54:25.008584 signapse-1.0.7/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.7/LICENSE.txt
--rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 13:54:25.008584 signapse-1.0.7/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3071 2024-04-04 12:54:19.000000 signapse-1.0.7/README.md
--rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 13:54:25.008584 signapse-1.0.7/setup.cfg
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1407 2024-04-04 13:53:43.000000 signapse-1.0.7/setup.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 13:54:25.008584 signapse-1.0.7/signapse/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.7/signapse/__init__.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.7/signapse/build_opt.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.7/signapse/compute.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.7/signapse/constants.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.7/signapse/create.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.7/signapse/create_model.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.7/signapse/heatmaps.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.7/signapse/lang_sam.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.7/signapse/lang_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.7/signapse/models_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.7/signapse/mp_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.7/signapse/poses.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.7/signapse/preprocessing.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.7/signapse/utils.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 13:54:25.008584 signapse-1.0.7/signapse.egg-info/
--rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/SOURCES.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/dependency_links.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      312 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/requires.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/top_level.txt
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:03:05.102008 signapse-1.0.8/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.8/LICENSE.txt
+-rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 14:03:05.102008 signapse-1.0.8/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3071 2024-04-04 12:54:19.000000 signapse-1.0.8/README.md
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 14:03:05.102008 signapse-1.0.8/setup.cfg
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1407 2024-04-04 14:02:33.000000 signapse-1.0.8/setup.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:03:05.102008 signapse-1.0.8/signapse/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.8/signapse/__init__.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.8/signapse/build_opt.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.8/signapse/compute.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.8/signapse/constants.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.8/signapse/create.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.8/signapse/create_model.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.8/signapse/heatmaps.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.8/signapse/lang_sam.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.8/signapse/lang_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.8/signapse/models_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.8/signapse/mp_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.8/signapse/poses.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.8/signapse/preprocessing.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.8/signapse/utils.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:03:05.102008 signapse-1.0.8/signapse.egg-info/
+-rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/SOURCES.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/dependency_links.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      312 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/requires.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.7/LICENSE.txt` & `signapse-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/PKG-INFO` & `signapse-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.7
+Version: 1.0.8
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,17 +23,17 @@
 Requires-Dist: pandas==2.1.1
 Requires-Dist: pickle5==0.0.11
 Requires-Dist: protobuf==3.20.*
 Requires-Dist: boto3==1.24.47
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: scipy==1.8
 Requires-Dist: pycpd==2.0.0
-Requires-Dist: torch==1.11.3+cu116
-Requires-Dist: torchvision==0.11.3+cu116
-Requires-Dist: torchaudio==0.11.3
+Requires-Dist: torch==1.11.0+cu113
+Requires-Dist: torchvision==0.12.0+cu113
+Requires-Dist: torchaudio==0.11.0
 Requires-Dist: Pillow==9.3.0
 Requires-Dist: imageio
 Requires-Dist: PyYAML
 
 # Signapse synthetic signer
 ![Signapse](https://static.wixstatic.com/media/45e73d_8ab2ecfdee064f20860fe2a1e3f8ddb2~mv2.png/v1/fill/w_132,h_35,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/Blank%202000%20x%202000%20-%202022-04-03T185113_234.png)
```

### Comparing `signapse-1.0.7/README.md` & `signapse-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/setup.py` & `signapse-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as ofile:
     long_description_file = ofile.read()
     
 setup(
     name='signapse',
-    version='1.0.7',
+    version='1.0.8',
     description='Signapse_synthetic_signer',
     long_description=long_description_file,
     long_description_content_type="text/markdown",
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
@@ -32,15 +32,15 @@
         'pandas==2.1.1',
         'pickle5==0.0.11',
         'protobuf==3.20.*',
         'boto3 == 1.24.47',
         'ffmpeg-python == 0.2.0',
         'scipy == 1.8,',
         'pycpd==2.0.0',
-        'torch==1.11.3+cu116',
-        'torchvision==0.11.3+cu116',
-        'torchaudio==0.11.3',
+        'torch==1.11.0+cu113',
+        'torchvision==0.12.0+cu113',
+        'torchaudio==0.11.0',
         'Pillow==9.3.0',
         'imageio',
         'PyYAML',
     ]
 )
```

### Comparing `signapse-1.0.7/signapse/build_opt.py` & `signapse-1.0.8/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/compute.py` & `signapse-1.0.8/signapse/compute.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/constants.py` & `signapse-1.0.8/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/create.py` & `signapse-1.0.8/signapse/create.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/create_model.py` & `signapse-1.0.8/signapse/create_model.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/heatmaps.py` & `signapse-1.0.8/signapse/heatmaps.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/lang_sam.py` & `signapse-1.0.8/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/lang_utils.py` & `signapse-1.0.8/signapse/lang_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/models_utils.py` & `signapse-1.0.8/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/mp_utils.py` & `signapse-1.0.8/signapse/mp_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/poses.py` & `signapse-1.0.8/signapse/poses.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/preprocessing.py` & `signapse-1.0.8/signapse/preprocessing.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse/utils.py` & `signapse-1.0.8/signapse/utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.7/signapse.egg-info/PKG-INFO` & `signapse-1.0.8/signapse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.7
+Version: 1.0.8
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,17 +23,17 @@
 Requires-Dist: pandas==2.1.1
 Requires-Dist: pickle5==0.0.11
 Requires-Dist: protobuf==3.20.*
 Requires-Dist: boto3==1.24.47
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: scipy==1.8
 Requires-Dist: pycpd==2.0.0
-Requires-Dist: torch==1.11.3+cu116
-Requires-Dist: torchvision==0.11.3+cu116
-Requires-Dist: torchaudio==0.11.3
+Requires-Dist: torch==1.11.0+cu113
+Requires-Dist: torchvision==0.12.0+cu113
+Requires-Dist: torchaudio==0.11.0
 Requires-Dist: Pillow==9.3.0
 Requires-Dist: imageio
 Requires-Dist: PyYAML
 
 # Signapse synthetic signer
 ![Signapse](https://static.wixstatic.com/media/45e73d_8ab2ecfdee064f20860fe2a1e3f8ddb2~mv2.png/v1/fill/w_132,h_35,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/Blank%202000%20x%202000%20-%202022-04-03T185113_234.png)
```

