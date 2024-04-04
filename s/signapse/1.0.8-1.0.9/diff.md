# Comparing `tmp/signapse-1.0.8.tar.gz` & `tmp/signapse-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.8.tar", last modified: Thu Apr  4 14:03:05 2024, max compression
+gzip compressed data, was "signapse-1.0.9.tar", last modified: Thu Apr  4 14:26:51 2024, max compression
```

## Comparing `signapse-1.0.8.tar` & `signapse-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:03:05.102008 signapse-1.0.8/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.8/LICENSE.txt
--rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 14:03:05.102008 signapse-1.0.8/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3071 2024-04-04 12:54:19.000000 signapse-1.0.8/README.md
--rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 14:03:05.102008 signapse-1.0.8/setup.cfg
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1407 2024-04-04 14:02:33.000000 signapse-1.0.8/setup.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:03:05.102008 signapse-1.0.8/signapse/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.8/signapse/__init__.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.8/signapse/build_opt.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.8/signapse/compute.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.8/signapse/constants.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.8/signapse/create.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.8/signapse/create_model.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.8/signapse/heatmaps.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.8/signapse/lang_sam.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.8/signapse/lang_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.8/signapse/models_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.8/signapse/mp_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.8/signapse/poses.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.8/signapse/preprocessing.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.8/signapse/utils.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:03:05.102008 signapse-1.0.8/signapse.egg-info/
--rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/SOURCES.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/dependency_links.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      312 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/requires.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 14:03:05.000000 signapse-1.0.8/signapse.egg-info/top_level.txt
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:26:51.801535 signapse-1.0.9/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.9/LICENSE.txt
+-rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 14:26:51.797536 signapse-1.0.9/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3071 2024-04-04 12:54:19.000000 signapse-1.0.9/README.md
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 14:26:51.801535 signapse-1.0.9/setup.cfg
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1407 2024-04-04 14:26:25.000000 signapse-1.0.9/setup.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:26:51.797536 signapse-1.0.9/signapse/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.9/signapse/__init__.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.9/signapse/build_opt.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.9/signapse/compute.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.9/signapse/constants.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.9/signapse/create.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.9/signapse/create_model.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    21720 2024-04-04 14:21:52.000000 signapse-1.0.9/signapse/heatmaps.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.9/signapse/lang_sam.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.9/signapse/lang_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.9/signapse/models_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3888 2024-04-04 14:23:34.000000 signapse-1.0.9/signapse/mp_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.9/signapse/poses.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3401 2024-04-04 14:22:51.000000 signapse-1.0.9/signapse/preprocessing.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.9/signapse/utils.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 14:26:51.797536 signapse-1.0.9/signapse.egg-info/
+-rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 14:26:51.000000 signapse-1.0.9/signapse.egg-info/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 14:26:51.000000 signapse-1.0.9/signapse.egg-info/SOURCES.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 14:26:51.000000 signapse-1.0.9/signapse.egg-info/dependency_links.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      312 2024-04-04 14:26:51.000000 signapse-1.0.9/signapse.egg-info/requires.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 14:26:51.000000 signapse-1.0.9/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.8/LICENSE.txt` & `signapse-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/PKG-INFO` & `signapse-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `signapse-1.0.8/README.md` & `signapse-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/setup.py` & `signapse-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as ofile:
     long_description_file = ofile.read()
     
 setup(
     name='signapse',
-    version='1.0.8',
+    version='1.0.9',
     description='Signapse_synthetic_signer',
     long_description=long_description_file,
     long_description_content_type="text/markdown",
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
```

### Comparing `signapse-1.0.8/signapse/build_opt.py` & `signapse-1.0.9/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/compute.py` & `signapse-1.0.9/signapse/compute.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/constants.py` & `signapse-1.0.9/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/create.py` & `signapse-1.0.9/signapse/create.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/create_model.py` & `signapse-1.0.9/signapse/create_model.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/heatmaps.py` & `signapse-1.0.9/signapse/heatmaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch, copy, cv2, math
 import numpy as np
-import constants as C
+import signapse.constants as C
 from torchvision import transforms 
 from torch.autograd import Variable
 import mediapipe as mp
 mp_face_mesh = mp.solutions.face_mesh
 
 
 # Draw a line between two points using OpenCV, if they are positive points
```

### Comparing `signapse-1.0.8/signapse/lang_sam.py` & `signapse-1.0.9/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/lang_utils.py` & `signapse-1.0.9/signapse/lang_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/models_utils.py` & `signapse-1.0.9/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/mp_utils.py` & `signapse-1.0.9/signapse/mp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import gzip, cv2, torch
 import pickle5 as pickle
 import numpy as np
 from pandas import Series
 from scipy.ndimage import gaussian_filter1d
-import constants as C
+import signapse.constants as C
 
 
 class INTERPLATION():
     def __init__(self):
         super(INTERPLATION,self).__init__() 
     
         # Interpolate over a numpy array
```

### Comparing `signapse-1.0.8/signapse/poses.py` & `signapse-1.0.9/signapse/poses.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse/preprocessing.py` & `signapse-1.0.9/signapse/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import imageio, torch
 import mediapipe as mp
-import constants as c
+import signapse.constants as C
 
 class Model():
     def __init__(self):
         super(Model, self).__init__()
         self.mp_holistic = mp.solutions.holistic
               
     def model(self):
```

### Comparing `signapse-1.0.8/signapse/utils.py` & `signapse-1.0.9/signapse/utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.8/signapse.egg-info/PKG-INFO` & `signapse-1.0.9/signapse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

