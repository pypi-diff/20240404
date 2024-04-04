# Comparing `tmp/PyFaceCrop-0.0.8.tar.gz` & `tmp/PyFaceCrop-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFaceCrop-0.0.8.tar", last modified: Thu Apr  4 10:51:39 2024, max compression
+gzip compressed data, last modified: Thu Apr  4 11:03:47 2024, from Unix
```

## Comparing `PyFaceCrop-0.0.8.tar` & `PyFaceCrop-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:51:39.350797 PyFaceCrop-0.0.8/
--rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.8/LICENSE
--rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:51:39.350357 PyFaceCrop-0.0.8/PKG-INFO
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:51:39.348269 PyFaceCrop-0.0.8/PyFaceCrop/
--rw-r--r--   0 cdp        (501) staff       (20)     2704 2024-04-04 10:02:57.000000 PyFaceCrop-0.0.8/PyFaceCrop/FaceCrop.py
--rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.8/PyFaceCrop/__init__.py
--rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.8/PyFaceCrop/main.py
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:51:39.349946 PyFaceCrop-0.0.8/PyFaceCrop/screenshots/
--rw-r--r--   0 cdp        (501) staff       (20)        0 2024-04-04 10:32:12.000000 PyFaceCrop-0.0.8/PyFaceCrop/screenshots/__init__.py
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:51:39.349661 PyFaceCrop-0.0.8/PyFaceCrop.egg-info/
--rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:51:39.000000 PyFaceCrop-0.0.8/PyFaceCrop.egg-info/PKG-INFO
--rw-r--r--   0 cdp        (501) staff       (20)      295 2024-04-04 10:51:39.000000 PyFaceCrop-0.0.8/PyFaceCrop.egg-info/SOURCES.txt
--rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-04 10:51:39.000000 PyFaceCrop-0.0.8/PyFaceCrop.egg-info/dependency_links.txt
--rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-04 10:51:39.000000 PyFaceCrop-0.0.8/PyFaceCrop.egg-info/requires.txt
--rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-04 10:51:39.000000 PyFaceCrop-0.0.8/PyFaceCrop.egg-info/top_level.txt
--rw-r--r--   0 cdp        (501) staff       (20)     1504 2024-04-04 09:46:16.000000 PyFaceCrop-0.0.8/README.md
--rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-04 10:51:39.351032 PyFaceCrop-0.0.8/setup.cfg
--rw-r--r--   0 cdp        (501) staff       (20)      314 2024-04-04 10:51:35.000000 PyFaceCrop-0.0.8/setup.py
+-rwxr-xr-x   0 cdp        (501) staff       (20)      220 2024-04-04 10:59:18.000000 ._PyFaceCrop-0.0.9
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:59:18.483282 PyFaceCrop-0.0.9/
+-rw-r--r--   0 cdp        (501) staff       (20)     1881 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PKG-INFO
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PyFaceCrop/
+-rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.9/LICENSE
+-rw-r--r--   0 cdp        (501) staff       (20)      163 2024-04-04 11:00:10.000000 PyFaceCrop-0.0.9/._README.md
+-rw-r--r--   0 cdp        (501) staff       (20)     1735 2024-04-04 11:00:10.625540 PyFaceCrop-0.0.9/README.md
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PyFaceCrop.egg-info/
+-rw-r--r--   0 cdp        (501) staff       (20)      319 2024-04-04 10:54:51.000000 PyFaceCrop-0.0.9/setup.py
+-rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/setup.cfg
+-rw-r--r--   0 cdp        (501) staff       (20)     1881 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PyFaceCrop.egg-info/PKG-INFO
+-rw-r--r--   0 cdp        (501) staff       (20)      295 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PyFaceCrop.egg-info/SOURCES.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PyFaceCrop.egg-info/requires.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PyFaceCrop.egg-info/top_level.txt
+-rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PyFaceCrop.egg-info/dependency_links.txt
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:59:18.000000 PyFaceCrop-0.0.9/PyFaceCrop/screenshots/
+-rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.9/PyFaceCrop/__init__.py
+-rw-r--r--   0 cdp        (501) staff       (20)     2704 2024-04-04 10:02:57.000000 PyFaceCrop-0.0.9/PyFaceCrop/FaceCrop.py
+-rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.9/PyFaceCrop/main.py
+-rw-r--r--   0 cdp        (501) staff       (20)        0 2024-04-04 10:32:12.000000 PyFaceCrop-0.0.9/PyFaceCrop/screenshots/__init__.py
```

### Comparing `PyFaceCrop-0.0.8/LICENSE` & `PyFaceCrop-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFaceCrop-0.0.8/PKG-INFO` & `PyFaceCrop-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFaceCrop
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 
 ## PyFaceCrop
 A PyFaceCrop library has been developed to streamline the process of cropping faces from videos while disregarding irrelevant frames. This library offers a convenient solution for extracting facial features from video data efficiently. By leveraging advanced computer vision techniques, it identifies and isolates faces within the video frames, providing a cropped output focused solely on facial content. This tool significantly simplifies the task of processing video data for applications such as facial recognition, emotion detection, and content analysis. With its user-friendly interface and robust functionality, the Python library for face cropping enhances productivity and accuracy in various domains reliant on video analysis.
 
@@ -16,20 +16,24 @@
 
 ## Code implementation
 ```
 from PyFaceCrop import FaceCrop
 capture = FaceCrop.FaceCrop("../Samples/test","identified_faces")
 capture.generate()
 ```
-![screenshot](./screenshots/Screenshot_Input.png)
+![screenshot](https://github.com/udayatom/PyFaceCrop/raw/main/PyFaceCrop/screenshots/Screenshot_Input.png)
 
 generate() croping the faces from the present frame, if the face is above to recognize.
 
 ## Points to remember
 
 PyFaceCrop generated crop frame faces into destination folder along with the respective folder with the name of the input the video file. So better to avoid multiple faces in the same video file to get a better dataset.
 
-![screenshot](./screenshots/Screenshot_Sajja.png)   
-![screenshot](./screenshots/Screenshot_Yogesh.png) 
-![screenshot](./screenshots/Screenshot_User23.png) 
+![screenshot](https://github.com/udayatom/PyFaceCrop/raw/main/PyFaceCrop/screenshots/Screenshot_Sajja.png)  
+
+
+![screenshot](https://github.com/udayatom/PyFaceCrop/raw/main/PyFaceCrop/screenshots/Screenshot_Yogesh.png) 
+
+
+![screenshot](https://github.com/udayatom/PyFaceCrop/raw/main/PyFaceCrop/screenshots/Screenshot_User23.png)
```

### Comparing `PyFaceCrop-0.0.8/PyFaceCrop/FaceCrop.py` & `PyFaceCrop-0.0.9/PyFaceCrop/FaceCrop.py`

 * *Files identical despite different names*

### Comparing `PyFaceCrop-0.0.8/PyFaceCrop.egg-info/PKG-INFO` & `PyFaceCrop-0.0.9/PyFaceCrop.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFaceCrop
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 
 ## PyFaceCrop
 A PyFaceCrop library has been developed to streamline the process of cropping faces from videos while disregarding irrelevant frames. This library offers a convenient solution for extracting facial features from video data efficiently. By leveraging advanced computer vision techniques, it identifies and isolates faces within the video frames, providing a cropped output focused solely on facial content. This tool significantly simplifies the task of processing video data for applications such as facial recognition, emotion detection, and content analysis. With its user-friendly interface and robust functionality, the Python library for face cropping enhances productivity and accuracy in various domains reliant on video analysis.
 
@@ -16,20 +16,24 @@
 
 ## Code implementation
 ```
 from PyFaceCrop import FaceCrop
 capture = FaceCrop.FaceCrop("../Samples/test","identified_faces")
 capture.generate()
 ```
-![screenshot](./screenshots/Screenshot_Input.png)
+![screenshot](https://github.com/udayatom/PyFaceCrop/raw/main/PyFaceCrop/screenshots/Screenshot_Input.png)
 
 generate() croping the faces from the present frame, if the face is above to recognize.
 
 ## Points to remember
 
 PyFaceCrop generated crop frame faces into destination folder along with the respective folder with the name of the input the video file. So better to avoid multiple faces in the same video file to get a better dataset.
 
-![screenshot](./screenshots/Screenshot_Sajja.png)   
-![screenshot](./screenshots/Screenshot_Yogesh.png) 
-![screenshot](./screenshots/Screenshot_User23.png) 
+![screenshot](https://github.com/udayatom/PyFaceCrop/raw/main/PyFaceCrop/screenshots/Screenshot_Sajja.png)  
+
+
+![screenshot](https://github.com/udayatom/PyFaceCrop/raw/main/PyFaceCrop/screenshots/Screenshot_Yogesh.png) 
+
+
+![screenshot](https://github.com/udayatom/PyFaceCrop/raw/main/PyFaceCrop/screenshots/Screenshot_User23.png)
```

