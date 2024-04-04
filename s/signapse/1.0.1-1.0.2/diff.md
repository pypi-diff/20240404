# Comparing `tmp/signapse-1.0.1.tar.gz` & `tmp/signapse-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.1.tar", last modified: Thu Apr  4 11:00:51 2024, max compression
+gzip compressed data, was "signapse-1.0.2.tar", last modified: Thu Apr  4 11:25:42 2024, max compression
```

## Comparing `signapse-1.0.1.tar` & `signapse-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:00:51.863678 signapse-1.0.1/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.1/LICENSE.txt
--rw-r--r--   0 basheer   (1000) basheer   (1000)     1097 2024-04-04 11:00:51.863678 signapse-1.0.1/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      240 2024-04-04 09:58:36.000000 signapse-1.0.1/README.md
--rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 11:00:51.863678 signapse-1.0.1/setup.cfg
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1176 2024-04-04 11:00:40.000000 signapse-1.0.1/setup.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:00:51.863678 signapse-1.0.1/signapse/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      418 2024-04-04 10:54:16.000000 signapse-1.0.1/signapse/__init__.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.1/signapse/build_opt.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9168 2024-04-04 10:51:00.000000 signapse-1.0.1/signapse/compute.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.1/signapse/constants.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     7257 2024-04-04 10:51:26.000000 signapse-1.0.1/signapse/create.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1216 2024-04-04 10:51:42.000000 signapse-1.0.1/signapse/create_model.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.1/signapse/heatmaps.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.1/signapse/lang_sam.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4413 2024-04-04 10:52:44.000000 signapse-1.0.1/signapse/lang_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.1/signapse/models_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.1/signapse/mp_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     7987 2024-04-04 10:50:14.000000 signapse-1.0.1/signapse/poses.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.1/signapse/preprocessing.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.1/signapse/utils.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:00:51.863678 signapse-1.0.1/signapse.egg-info/
--rw-r--r--   0 basheer   (1000) basheer   (1000)     1097 2024-04-04 11:00:51.000000 signapse-1.0.1/signapse.egg-info/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 11:00:51.000000 signapse-1.0.1/signapse.egg-info/SOURCES.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 11:00:51.000000 signapse-1.0.1/signapse.egg-info/dependency_links.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      223 2024-04-04 11:00:51.000000 signapse-1.0.1/signapse.egg-info/requires.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 11:00:51.000000 signapse-1.0.1/signapse.egg-info/top_level.txt
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:25:42.047058 signapse-1.0.2/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.2/LICENSE.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      619 2024-04-04 11:25:42.047058 signapse-1.0.2/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      240 2024-04-04 09:58:36.000000 signapse-1.0.2/README.md
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 11:25:42.047058 signapse-1.0.2/setup.cfg
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1176 2024-04-04 11:24:45.000000 signapse-1.0.2/setup.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:25:42.047058 signapse-1.0.2/signapse/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.2/signapse/__init__.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.2/signapse/build_opt.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.2/signapse/compute.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.2/signapse/constants.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.2/signapse/create.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.2/signapse/create_model.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.2/signapse/heatmaps.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.2/signapse/lang_sam.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.2/signapse/lang_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.2/signapse/models_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.2/signapse/mp_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.2/signapse/poses.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.2/signapse/preprocessing.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.2/signapse/utils.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 11:25:42.047058 signapse-1.0.2/signapse.egg-info/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      619 2024-04-04 11:25:41.000000 signapse-1.0.2/signapse.egg-info/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 11:25:42.000000 signapse-1.0.2/signapse.egg-info/SOURCES.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 11:25:41.000000 signapse-1.0.2/signapse.egg-info/dependency_links.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      223 2024-04-04 11:25:41.000000 signapse-1.0.2/signapse.egg-info/requires.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 11:25:41.000000 signapse-1.0.2/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.1/LICENSE.txt` & `signapse-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `signapse-1.0.1/setup.py` & `signapse-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='signapse',
-    version='1.0.1',
+    version='1.0.2',
     description='Signapse_synthetic_signer',
     long_description='Signapse_synthetic_signer package',
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
     classifiers=[
```

### Comparing `signapse-1.0.1/signapse/build_opt.py` & `signapse-1.0.2/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.1/signapse/compute.py` & `signapse-1.0.2/signapse/compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cv2, math, torch,multiprocessing,imageio
 import mediapipe as mp
-from mp_utils import IMAGE_PROCESSING 
+from signapse.mp_utils import IMAGE_PROCESSING 
 
 mp_holistic = mp.solutions.holistic
 mp_face_mesh = mp.solutions.face_mesh
 
 # Given a MediaPipe tensor, find the shoulder centre
 def find_shoulder_centre_MP_small_tensor(MP_results_find):
     left_shoulder = MP_results_find[0]
```

### Comparing `signapse-1.0.1/signapse/constants.py` & `signapse-1.0.2/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.1/signapse/create.py` & `signapse-1.0.2/signapse/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging, torch, imageio, cv2, copy, os
 import numpy as np
 from pathlib import Path
-from heatmaps import HEATMAPS
+from signapse.heatmaps import HEATMAPS
 
 
 class GENERATOR():
     def __init__(self, args):
         super(GENERATOR,self).__init__()
         self.args=args
```

### Comparing `signapse-1.0.1/signapse/create_model.py` & `signapse-1.0.2/signapse/create_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from models_utils import create_model
+from signapse.models_utils import create_model
 import pickle5 as pickle
 import gzip
 
 class CROP_GAN():
     def __init__(self, args):
         super(CROP_GAN,self).__init__()
         self.args=args
```

### Comparing `signapse-1.0.1/signapse/heatmaps.py` & `signapse-1.0.2/signapse/heatmaps.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.1/signapse/lang_sam.py` & `signapse-1.0.2/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.1/signapse/lang_utils.py` & `signapse-1.0.2/signapse/lang_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import  torch,logging,imageio 
 import mediapipe as mp
 import numpy as np
 from PIL import Image, ImageEnhance
 logging.basicConfig(level=logging.INFO)
 
-from lang_sam import LangSAM
+from signapse.lang_sam import LangSAM
 import signapse.constants as C
-from create import GENERATOR
-from utils import INTERPLATION, IMAGE_PROCESSING
+from signapse.create import GENERATOR
+from signapse.mp_utils import INTERPLATION, IMAGE_PROCESSING
 
 mp_face_mesh = mp.solutions.face_mesh
 face_mesh =  mp_face_mesh.FaceMesh(max_num_faces=1,
                                     static_image_mode=True,
                                     refine_landmarks=True,
                                     min_detection_confidence=0.8,
                                     min_tracking_confidence=0.8)
```

### Comparing `signapse-1.0.1/signapse/models_utils.py` & `signapse-1.0.2/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.1/signapse/mp_utils.py` & `signapse-1.0.2/signapse/mp_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.1/signapse/poses.py` & `signapse-1.0.2/signapse/poses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch,logging
-from compute import parallel_computing, serial_computing
-from mp_utils import INTERPLATION, IMAGE_PROCESSING
+from signapse.compute import parallel_computing, serial_computing
+from signapse.mp_utils import INTERPLATION, IMAGE_PROCESSING
 import numpy as np
-import constants as C
+import signapse.constants as C
 
 class POSE():
     def __init__(self, args):
         super(POSE,self).__init__()
         self.args=args   
         
     def face_mesh_landmarks_to_small_tensor(self,face_mesh_landmarks):
```

### Comparing `signapse-1.0.1/signapse/preprocessing.py` & `signapse-1.0.2/signapse/preprocessing.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.1/signapse/utils.py` & `signapse-1.0.2/signapse/utils.py`

 * *Files identical despite different names*

