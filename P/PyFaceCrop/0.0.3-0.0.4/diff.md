# Comparing `tmp/PyFaceCrop-0.0.3.tar.gz` & `tmp/PyFaceCrop-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFaceCrop-0.0.3.tar", last modified: Thu Apr  4 10:12:42 2024, max compression
+gzip compressed data, was "PyFaceCrop-0.0.4.tar", last modified: Thu Apr  4 10:19:08 2024, max compression
```

## Comparing `PyFaceCrop-0.0.3.tar` & `PyFaceCrop-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:12:42.355910 PyFaceCrop-0.0.3/
--rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.3/LICENSE
--rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:12:42.355623 PyFaceCrop-0.0.3/PKG-INFO
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:12:42.353973 PyFaceCrop-0.0.3/PyFaceCrop/
--rw-r--r--   0 cdp        (501) staff       (20)     2704 2024-04-04 10:02:57.000000 PyFaceCrop-0.0.3/PyFaceCrop/FaceCrop.py
--rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.3/PyFaceCrop/__init__.py
--rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.3/PyFaceCrop/main.py
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:12:42.355140 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/
--rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/PKG-INFO
--rw-r--r--   0 cdp        (501) staff       (20)      260 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/SOURCES.txt
--rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/dependency_links.txt
--rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/requires.txt
--rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/top_level.txt
--rw-r--r--   0 cdp        (501) staff       (20)     1504 2024-04-04 09:46:16.000000 PyFaceCrop-0.0.3/README.md
--rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-04 10:12:42.355974 PyFaceCrop-0.0.3/setup.cfg
--rw-r--r--   0 cdp        (501) staff       (20)      320 2024-04-04 09:58:23.000000 PyFaceCrop-0.0.3/setup.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:19:08.818348 PyFaceCrop-0.0.4/
+-rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.4/LICENSE
+-rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:19:08.818036 PyFaceCrop-0.0.4/PKG-INFO
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:19:08.816432 PyFaceCrop-0.0.4/PyFaceCrop/
+-rw-r--r--   0 cdp        (501) staff       (20)     2704 2024-04-04 10:02:57.000000 PyFaceCrop-0.0.4/PyFaceCrop/FaceCrop.py
+-rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.4/PyFaceCrop/__init__.py
+-rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.4/PyFaceCrop/main.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:19:08.817607 PyFaceCrop-0.0.4/PyFaceCrop.egg-info/
+-rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:19:08.000000 PyFaceCrop-0.0.4/PyFaceCrop.egg-info/PKG-INFO
+-rw-r--r--   0 cdp        (501) staff       (20)      260 2024-04-04 10:19:08.000000 PyFaceCrop-0.0.4/PyFaceCrop.egg-info/SOURCES.txt
+-rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-04 10:19:08.000000 PyFaceCrop-0.0.4/PyFaceCrop.egg-info/dependency_links.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-04 10:19:08.000000 PyFaceCrop-0.0.4/PyFaceCrop.egg-info/requires.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-04 10:19:08.000000 PyFaceCrop-0.0.4/PyFaceCrop.egg-info/top_level.txt
+-rw-r--r--   0 cdp        (501) staff       (20)     1504 2024-04-04 09:46:16.000000 PyFaceCrop-0.0.4/README.md
+-rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-04 10:19:08.818420 PyFaceCrop-0.0.4/setup.cfg
+-rw-r--r--   0 cdp        (501) staff       (20)      320 2024-04-04 10:19:01.000000 PyFaceCrop-0.0.4/setup.py
```

### Comparing `PyFaceCrop-0.0.3/LICENSE` & `PyFaceCrop-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyFaceCrop-0.0.3/PKG-INFO` & `PyFaceCrop-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFaceCrop
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 
 ## PyFaceCrop
 A PyFaceCrop library has been developed to streamline the process of cropping faces from videos while disregarding irrelevant frames. This library offers a convenient solution for extracting facial features from video data efficiently. By leveraging advanced computer vision techniques, it identifies and isolates faces within the video frames, providing a cropped output focused solely on facial content. This tool significantly simplifies the task of processing video data for applications such as facial recognition, emotion detection, and content analysis. With its user-friendly interface and robust functionality, the Python library for face cropping enhances productivity and accuracy in various domains reliant on video analysis.
```

### Comparing `PyFaceCrop-0.0.3/PyFaceCrop/FaceCrop.py` & `PyFaceCrop-0.0.4/PyFaceCrop/FaceCrop.py`

 * *Files identical despite different names*

### Comparing `PyFaceCrop-0.0.3/PyFaceCrop.egg-info/PKG-INFO` & `PyFaceCrop-0.0.4/PyFaceCrop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFaceCrop
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python
 
 ## PyFaceCrop
 A PyFaceCrop library has been developed to streamline the process of cropping faces from videos while disregarding irrelevant frames. This library offers a convenient solution for extracting facial features from video data efficiently. By leveraging advanced computer vision techniques, it identifies and isolates faces within the video frames, providing a cropped output focused solely on facial content. This tool significantly simplifies the task of processing video data for applications such as facial recognition, emotion detection, and content analysis. With its user-friendly interface and robust functionality, the Python library for face cropping enhances productivity and accuracy in various domains reliant on video analysis.
```

### Comparing `PyFaceCrop-0.0.3/README.md` & `PyFaceCrop-0.0.4/README.md`

 * *Files identical despite different names*
