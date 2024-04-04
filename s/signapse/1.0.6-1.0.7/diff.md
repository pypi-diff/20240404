# Comparing `tmp/signapse-1.0.6.tar.gz` & `tmp/signapse-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signapse-1.0.6.tar", last modified: Thu Apr  4 12:52:32 2024, max compression
+gzip compressed data, was "signapse-1.0.7.tar", last modified: Thu Apr  4 13:54:25 2024, max compression
```

## Comparing `signapse-1.0.6.tar` & `signapse-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:52:32.496654 signapse-1.0.6/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.6/LICENSE.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3824 2024-04-04 12:52:32.496654 signapse-1.0.6/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3199 2024-04-04 12:51:00.000000 signapse-1.0.6/README.md
--rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 12:52:32.496654 signapse-1.0.6/setup.cfg
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1296 2024-04-04 12:52:28.000000 signapse-1.0.6/setup.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:52:32.496654 signapse-1.0.6/signapse/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.6/signapse/__init__.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.6/signapse/build_opt.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.6/signapse/compute.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.6/signapse/constants.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.6/signapse/create.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.6/signapse/create_model.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.6/signapse/heatmaps.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.6/signapse/lang_sam.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.6/signapse/lang_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.6/signapse/models_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.6/signapse/mp_utils.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.6/signapse/poses.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.6/signapse/preprocessing.py
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.6/signapse/utils.py
-drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 12:52:32.496654 signapse-1.0.6/signapse.egg-info/
--rw-rw-r--   0 basheer   (1000) basheer   (1000)     3824 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/PKG-INFO
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/SOURCES.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/dependency_links.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)      223 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/requires.txt
--rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 12:52:32.000000 signapse-1.0.6/signapse.egg-info/top_level.txt
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 13:54:25.008584 signapse-1.0.7/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1065 2024-04-04 10:20:56.000000 signapse-1.0.7/LICENSE.txt
+-rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 13:54:25.008584 signapse-1.0.7/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3071 2024-04-04 12:54:19.000000 signapse-1.0.7/README.md
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)       38 2024-04-04 13:54:25.008584 signapse-1.0.7/setup.cfg
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1407 2024-04-04 13:53:43.000000 signapse-1.0.7/setup.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 13:54:25.008584 signapse-1.0.7/signapse/
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      463 2024-04-04 11:18:15.000000 signapse-1.0.7/signapse/__init__.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     5835 2024-03-23 21:03:41.000000 signapse-1.0.7/signapse/build_opt.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     9177 2024-04-04 11:09:13.000000 signapse-1.0.7/signapse/compute.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2662 2024-04-04 10:51:14.000000 signapse-1.0.7/signapse/constants.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     7266 2024-04-04 11:07:47.000000 signapse-1.0.7/signapse/create.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     1225 2024-04-04 11:11:01.000000 signapse-1.0.7/signapse/create_model.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    21711 2024-04-04 10:51:53.000000 signapse-1.0.7/signapse/heatmaps.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4652 2023-12-03 23:04:06.000000 signapse-1.0.7/signapse/lang_sam.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     4443 2024-04-04 11:20:45.000000 signapse-1.0.7/signapse/lang_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)    17696 2023-12-03 23:04:06.000000 signapse-1.0.7/signapse/models_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3879 2024-04-04 10:53:01.000000 signapse-1.0.7/signapse/mp_utils.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     8014 2024-04-04 11:08:36.000000 signapse-1.0.7/signapse/poses.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     3392 2024-04-04 10:53:14.000000 signapse-1.0.7/signapse/preprocessing.py
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)     2610 2023-12-03 23:04:06.000000 signapse-1.0.7/signapse/utils.py
+drwxrwxr-x   0 basheer   (1000) basheer   (1000)        0 2024-04-04 13:54:25.008584 signapse-1.0.7/signapse.egg-info/
+-rw-r--r--   0 basheer   (1000) basheer   (1000)     4293 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/PKG-INFO
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      491 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/SOURCES.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        1 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/dependency_links.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)      312 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/requires.txt
+-rw-rw-r--   0 basheer   (1000) basheer   (1000)        9 2024-04-04 13:54:25.000000 signapse-1.0.7/signapse.egg-info/top_level.txt
```

### Comparing `signapse-1.0.6/LICENSE.txt` & `signapse-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/PKG-INFO` & `signapse-1.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.6
+Version: 1.0.7
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: essentials
+Requires-Dist: setuptools
+Requires-Dist: wheel==0.38.4
+Requires-Dist: mediapipe==0.10.3
+Requires-Dist: opencv-python==4.7.0.72
+Requires-Dist: opencv-python-headless==4.7.0.72
+Requires-Dist: pandas==2.1.1
+Requires-Dist: pickle5==0.0.11
+Requires-Dist: protobuf==3.20.*
+Requires-Dist: boto3==1.24.47
+Requires-Dist: ffmpeg-python==0.2.0
+Requires-Dist: scipy==1.8
+Requires-Dist: pycpd==2.0.0
+Requires-Dist: torch==1.11.3+cu116
+Requires-Dist: torchvision==0.11.3+cu116
+Requires-Dist: torchaudio==0.11.3
+Requires-Dist: Pillow==9.3.0
+Requires-Dist: imageio
+Requires-Dist: PyYAML
 
-## Signapse synthetic signer
+# Signapse synthetic signer
 ![Signapse](https://static.wixstatic.com/media/45e73d_8ab2ecfdee064f20860fe2a1e3f8ddb2~mv2.png/v1/fill/w_132,h_35,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/Blank%202000%20x%202000%20-%202022-04-03T185113_234.png)
 
-
-# Synthetic Signer
 Requires python=3.7.0
 
 ### Example command 
 
 ```python inference.py "{\"GPU\":\"cpu\",\"input_video_path\":\"path/to/video.mp4\",\"input_type\":\"video\",\"start\":0,\"stop\":-1,\"num_workers\":1,\"GAN_folder\":\"GAN\",\"signer\":\"Barbara\",\"stereo\":\"False\",\"pro\":\"True\",\"detailed_video\":\"False\",\"organisation_id\":\"0\",\"sign_request_id\":\"0\",\"sign_result_queue_url\":\"0\",\"synthetic_sign_results_bucket\":\"0\"}" ```
 
 
@@ -98,10 +115,8 @@
 
 ## To run with Stereo data (--stereo True and --input_video_path refers to the pickle file) 
 
 Pass the respective *--stereo True* argument.
 
 ```python ./inference.py --organisation_id 0  --sign_result_queue_url 0 --synthetic_sign_results_bucket 0 --input_video_path /home/basheer/Signapse/Stereo/video_1/H020_smile2.flircorder.H020_data_m6.H020.07042022.142814_recording_data.pkl  --stop 1000 --num_workers 8 --GPU cuda --sign_request_id NoFaB_100 --GAN_folder GAN --stereo True```
 
-=======
-Pass the respective `--input_type numpy` argument.
->>>>>>> 66c02cb886bab2dfb428e57ab477c5bf8ab59209
+
```

### Comparing `signapse-1.0.6/README.md` & `signapse-1.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-## Signapse synthetic signer
+# Signapse synthetic signer
 ![Signapse](https://static.wixstatic.com/media/45e73d_8ab2ecfdee064f20860fe2a1e3f8ddb2~mv2.png/v1/fill/w_132,h_35,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/Blank%202000%20x%202000%20-%202022-04-03T185113_234.png)
 
-
-# Synthetic Signer
 Requires python=3.7.0
 
 ### Example command 
 
 ```python inference.py "{\"GPU\":\"cpu\",\"input_video_path\":\"path/to/video.mp4\",\"input_type\":\"video\",\"start\":0,\"stop\":-1,\"num_workers\":1,\"GAN_folder\":\"GAN\",\"signer\":\"Barbara\",\"stereo\":\"False\",\"pro\":\"True\",\"detailed_video\":\"False\",\"organisation_id\":\"0\",\"sign_request_id\":\"0\",\"sign_result_queue_url\":\"0\",\"synthetic_sign_results_bucket\":\"0\"}" ```
 
 
@@ -81,10 +79,8 @@
 
 ## To run with Stereo data (--stereo True and --input_video_path refers to the pickle file) 
 
 Pass the respective *--stereo True* argument.
 
 ```python ./inference.py --organisation_id 0  --sign_result_queue_url 0 --synthetic_sign_results_bucket 0 --input_video_path /home/basheer/Signapse/Stereo/video_1/H020_smile2.flircorder.H020_data_m6.H020.07042022.142814_recording_data.pkl  --stop 1000 --num_workers 8 --GPU cuda --sign_request_id NoFaB_100 --GAN_folder GAN --stereo True```
 
-=======
-Pass the respective `--input_type numpy` argument.
->>>>>>> 66c02cb886bab2dfb428e57ab477c5bf8ab59209
+
```

### Comparing `signapse-1.0.6/setup.py` & `signapse-1.0.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r") as ofile:
     long_description_file = ofile.read()
     
 setup(
     name='signapse',
-    version='1.0.6',
+    version='1.0.7',
     description='Signapse_synthetic_signer',
     long_description=long_description_file,
     long_description_content_type="text/markdown",
     author='Basheer Alwaely',
     author_email='basheer@signapse.ai',
     url='https://github.com/signapse/signapse',
     packages=find_packages(),
@@ -21,24 +21,26 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     install_requires=[
         'essentials',
         'setuptools',
-        'wheel',
-        'mediapipe==0.8.11',
-        'opencv-python==4.6.0.66',
-        'opencv-python-headless==4.5.5.62',
-        'pandas',
-        'pickle5',
+        'wheel==0.38.4',
+        'mediapipe==0.10.3',
+        'opencv-python==4.7.0.72',
+        'opencv-python-headless==4.7.0.72',
+        'pandas==2.1.1',
+        'pickle5==0.0.11',
         'protobuf==3.20.*',
         'boto3 == 1.24.47',
         'ffmpeg-python == 0.2.0',
-        'scipy == 1.7.3,',
-        'pycpd',
-        'torch',
-        'torchvision',
+        'scipy == 1.8,',
+        'pycpd==2.0.0',
+        'torch==1.11.3+cu116',
+        'torchvision==0.11.3+cu116',
+        'torchaudio==0.11.3',
+        'Pillow==9.3.0',
         'imageio',
         'PyYAML',
     ]
 )
```

### Comparing `signapse-1.0.6/signapse/build_opt.py` & `signapse-1.0.7/signapse/build_opt.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/compute.py` & `signapse-1.0.7/signapse/compute.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/constants.py` & `signapse-1.0.7/signapse/constants.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/create.py` & `signapse-1.0.7/signapse/create.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/create_model.py` & `signapse-1.0.7/signapse/create_model.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/heatmaps.py` & `signapse-1.0.7/signapse/heatmaps.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/lang_sam.py` & `signapse-1.0.7/signapse/lang_sam.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/lang_utils.py` & `signapse-1.0.7/signapse/lang_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/models_utils.py` & `signapse-1.0.7/signapse/models_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/mp_utils.py` & `signapse-1.0.7/signapse/mp_utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/poses.py` & `signapse-1.0.7/signapse/poses.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/preprocessing.py` & `signapse-1.0.7/signapse/preprocessing.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse/utils.py` & `signapse-1.0.7/signapse/utils.py`

 * *Files identical despite different names*

### Comparing `signapse-1.0.6/signapse.egg-info/PKG-INFO` & `signapse-1.0.7/signapse.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 Metadata-Version: 2.1
 Name: signapse
-Version: 1.0.6
+Version: 1.0.7
 Summary: Signapse_synthetic_signer
 Home-page: https://github.com/signapse/signapse
 Author: Basheer Alwaely
 Author-email: basheer@signapse.ai
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: essentials
+Requires-Dist: setuptools
+Requires-Dist: wheel==0.38.4
+Requires-Dist: mediapipe==0.10.3
+Requires-Dist: opencv-python==4.7.0.72
+Requires-Dist: opencv-python-headless==4.7.0.72
+Requires-Dist: pandas==2.1.1
+Requires-Dist: pickle5==0.0.11
+Requires-Dist: protobuf==3.20.*
+Requires-Dist: boto3==1.24.47
+Requires-Dist: ffmpeg-python==0.2.0
+Requires-Dist: scipy==1.8
+Requires-Dist: pycpd==2.0.0
+Requires-Dist: torch==1.11.3+cu116
+Requires-Dist: torchvision==0.11.3+cu116
+Requires-Dist: torchaudio==0.11.3
+Requires-Dist: Pillow==9.3.0
+Requires-Dist: imageio
+Requires-Dist: PyYAML
 
-## Signapse synthetic signer
+# Signapse synthetic signer
 ![Signapse](https://static.wixstatic.com/media/45e73d_8ab2ecfdee064f20860fe2a1e3f8ddb2~mv2.png/v1/fill/w_132,h_35,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/Blank%202000%20x%202000%20-%202022-04-03T185113_234.png)
 
-
-# Synthetic Signer
 Requires python=3.7.0
 
 ### Example command 
 
 ```python inference.py "{\"GPU\":\"cpu\",\"input_video_path\":\"path/to/video.mp4\",\"input_type\":\"video\",\"start\":0,\"stop\":-1,\"num_workers\":1,\"GAN_folder\":\"GAN\",\"signer\":\"Barbara\",\"stereo\":\"False\",\"pro\":\"True\",\"detailed_video\":\"False\",\"organisation_id\":\"0\",\"sign_request_id\":\"0\",\"sign_result_queue_url\":\"0\",\"synthetic_sign_results_bucket\":\"0\"}" ```
 
 
@@ -98,10 +115,8 @@
 
 ## To run with Stereo data (--stereo True and --input_video_path refers to the pickle file) 
 
 Pass the respective *--stereo True* argument.
 
 ```python ./inference.py --organisation_id 0  --sign_result_queue_url 0 --synthetic_sign_results_bucket 0 --input_video_path /home/basheer/Signapse/Stereo/video_1/H020_smile2.flircorder.H020_data_m6.H020.07042022.142814_recording_data.pkl  --stop 1000 --num_workers 8 --GPU cuda --sign_request_id NoFaB_100 --GAN_folder GAN --stereo True```
 
-=======
-Pass the respective `--input_type numpy` argument.
->>>>>>> 66c02cb886bab2dfb428e57ab477c5bf8ab59209
+
```

