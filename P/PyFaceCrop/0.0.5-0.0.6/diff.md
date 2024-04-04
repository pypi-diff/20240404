# Comparing `tmp/PyFaceCrop-0.0.5.tar.gz` & `tmp/PyFaceCrop-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFaceCrop-0.0.5.tar", last modified: Thu Apr  4 10:34:44 2024, max compression
+gzip compressed data, was "PyFaceCrop-0.0.6.tar", last modified: Thu Apr  4 10:39:17 2024, max compression
```

## Comparing `PyFaceCrop-0.0.5.tar` & `PyFaceCrop-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:34:44.004275 PyFaceCrop-0.0.5/
--rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.5/LICENSE
--rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:34:44.003979 PyFaceCrop-0.0.5/PKG-INFO
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:34:44.002398 PyFaceCrop-0.0.5/PyFaceCrop/
--rw-r--r--   0 cdp        (501) staff       (20)     2704 2024-04-04 10:02:57.000000 PyFaceCrop-0.0.5/PyFaceCrop/FaceCrop.py
--rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.5/PyFaceCrop/__init__.py
--rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.5/PyFaceCrop/main.py
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:34:44.003568 PyFaceCrop-0.0.5/PyFaceCrop/screenshots/
--rw-r--r--   0 cdp        (501) staff       (20)        0 2024-04-04 10:32:12.000000 PyFaceCrop-0.0.5/PyFaceCrop/screenshots/__init__.py
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:34:44.003344 PyFaceCrop-0.0.5/PyFaceCrop.egg-info/
--rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:34:43.000000 PyFaceCrop-0.0.5/PyFaceCrop.egg-info/PKG-INFO
--rw-r--r--   0 cdp        (501) staff       (20)      295 2024-04-04 10:34:43.000000 PyFaceCrop-0.0.5/PyFaceCrop.egg-info/SOURCES.txt
--rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-04 10:34:43.000000 PyFaceCrop-0.0.5/PyFaceCrop.egg-info/dependency_links.txt
--rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-04 10:34:43.000000 PyFaceCrop-0.0.5/PyFaceCrop.egg-info/requires.txt
--rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-04 10:34:43.000000 PyFaceCrop-0.0.5/PyFaceCrop.egg-info/top_level.txt
--rw-r--r--   0 cdp        (501) staff       (20)     1504 2024-04-04 09:46:16.000000 PyFaceCrop-0.0.5/README.md
--rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-04 10:34:44.004342 PyFaceCrop-0.0.5/setup.cfg
--rw-r--r--   0 cdp        (501) staff       (20)      314 2024-04-04 10:32:20.000000 PyFaceCrop-0.0.5/setup.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:39:17.538385 PyFaceCrop-0.0.6/
+-rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.6/LICENSE
+-rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:39:17.537952 PyFaceCrop-0.0.6/PKG-INFO
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:39:17.536389 PyFaceCrop-0.0.6/PyFaceCrop/
+-rw-r--r--   0 cdp        (501) staff       (20)     2704 2024-04-04 10:02:57.000000 PyFaceCrop-0.0.6/PyFaceCrop/FaceCrop.py
+-rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.6/PyFaceCrop/__init__.py
+-rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.6/PyFaceCrop/main.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:39:17.537609 PyFaceCrop-0.0.6/PyFaceCrop/screenshots/
+-rw-r--r--   0 cdp        (501) staff       (20)        0 2024-04-04 10:32:12.000000 PyFaceCrop-0.0.6/PyFaceCrop/screenshots/__init__.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:39:17.537403 PyFaceCrop-0.0.6/PyFaceCrop.egg-info/
+-rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:39:17.000000 PyFaceCrop-0.0.6/PyFaceCrop.egg-info/PKG-INFO
+-rw-r--r--   0 cdp        (501) staff       (20)      295 2024-04-04 10:39:17.000000 PyFaceCrop-0.0.6/PyFaceCrop.egg-info/SOURCES.txt
+-rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-04 10:39:17.000000 PyFaceCrop-0.0.6/PyFaceCrop.egg-info/dependency_links.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-04 10:39:17.000000 PyFaceCrop-0.0.6/PyFaceCrop.egg-info/requires.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-04 10:39:17.000000 PyFaceCrop-0.0.6/PyFaceCrop.egg-info/top_level.txt
+-rw-r--r--   0 cdp        (501) staff       (20)     1504 2024-04-04 09:46:16.000000 PyFaceCrop-0.0.6/README.md
+-rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-04 10:39:17.538601 PyFaceCrop-0.0.6/setup.cfg
+-rw-r--r--   0 cdp        (501) staff       (20)      314 2024-04-04 10:39:12.000000 PyFaceCrop-0.0.6/setup.py
```

### Comparing `PyFaceCrop-0.0.5/LICENSE` & `PyFaceCrop-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFaceCrop-0.0.5/PKG-INFO` & `PyFaceCrop-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFaceCrop
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 
 ## PyFaceCrop
 A PyFaceCrop library has been developed to streamline the process of cropping faces from videos while disregarding irrelevant frames. This library offers a convenient solution for extracting facial features from video data efficiently. By leveraging advanced computer vision techniques, it identifies and isolates faces within the video frames, providing a cropped output focused solely on facial content. This tool significantly simplifies the task of processing video data for applications such as facial recognition, emotion detection, and content analysis. With its user-friendly interface and robust functionality, the Python library for face cropping enhances productivity and accuracy in various domains reliant on video analysis.
```

### Comparing `PyFaceCrop-0.0.5/PyFaceCrop/FaceCrop.py` & `PyFaceCrop-0.0.6/PyFaceCrop/FaceCrop.py`

 * *Files identical despite different names*

### Comparing `PyFaceCrop-0.0.5/PyFaceCrop.egg-info/PKG-INFO` & `PyFaceCrop-0.0.6/PyFaceCrop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFaceCrop
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 
 ## PyFaceCrop
 A PyFaceCrop library has been developed to streamline the process of cropping faces from videos while disregarding irrelevant frames. This library offers a convenient solution for extracting facial features from video data efficiently. By leveraging advanced computer vision techniques, it identifies and isolates faces within the video frames, providing a cropped output focused solely on facial content. This tool significantly simplifies the task of processing video data for applications such as facial recognition, emotion detection, and content analysis. With its user-friendly interface and robust functionality, the Python library for face cropping enhances productivity and accuracy in various domains reliant on video analysis.
```

### Comparing `PyFaceCrop-0.0.5/README.md` & `PyFaceCrop-0.0.6/README.md`

 * *Files identical despite different names*

