# Comparing `tmp/skdir-0.1.4.tar.gz` & `tmp/skdir-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skdir-0.1.4.tar", last modified: Thu Apr  4 03:05:57 2024, max compression
+gzip compressed data, was "skdir-0.1.5.tar", last modified: Thu Apr  4 03:14:45 2024, max compression
```

## Comparing `skdir-0.1.4.tar` & `skdir-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:05:57.010275 skdir-0.1.4/
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.1.4/LICENSE
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 03:05:57.010064 skdir-0.1.4/PKG-INFO
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.1.4/README.md
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:05:57.008728 skdir-0.1.4/lab/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      561 2024-04-04 03:05:16.000000 skdir-0.1.4/lab/__init__.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.1.4/lab/p1.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.1.4/lab/p2.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.1.4/lab/p3.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.1.4/lab/p4.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.1.4/lab/p5.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.1.4/lab/p6.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.1.4/lab/p7.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.1.4/lab/p8.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-04 03:05:57.010351 skdir-0.1.4/setup.cfg
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      925 2024-04-04 03:05:52.000000 skdir-0.1.4/setup.py
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:05:57.009773 skdir-0.1.4/skdir.egg-info/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 03:05:56.000000 skdir-0.1.4/skdir.egg-info/PKG-INFO
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-04 03:05:57.000000 skdir-0.1.4/skdir.egg-info/SOURCES.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-04 03:05:56.000000 skdir-0.1.4/skdir.egg-info/dependency_links.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-04 03:05:57.000000 skdir-0.1.4/skdir.egg-info/requires.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-04 03:05:57.000000 skdir-0.1.4/skdir.egg-info/top_level.txt
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:14:45.428423 skdir-0.1.5/
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.1.5/LICENSE
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 03:14:45.428186 skdir-0.1.5/PKG-INFO
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.1.5/README.md
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:14:45.426262 skdir-0.1.5/lab/
+-rwxr-xrwx   0 sharathchandrak   (501) staff       (20)      561 2024-04-04 03:05:16.000000 skdir-0.1.5/lab/__init__.py
+-rwxrwxrwx   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.1.5/lab/p1.py
+-rwxrwxrwx   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.1.5/lab/p2.py
+-rwxrwxrwx   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.1.5/lab/p3.py
+-rwxr-xrwx   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.1.5/lab/p4.py
+-rwxr-xrwx   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.1.5/lab/p5.py
+-rwxr-xrwx   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.1.5/lab/p6.py
+-rwxr-xrwx   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.1.5/lab/p7.py
+-rwxr-xrwx   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.1.5/lab/p8.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-04 03:14:45.428518 skdir-0.1.5/setup.cfg
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      925 2024-04-04 03:14:41.000000 skdir-0.1.5/setup.py
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:14:45.427794 skdir-0.1.5/skdir.egg-info/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 03:14:45.000000 skdir-0.1.5/skdir.egg-info/PKG-INFO
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-04 03:14:45.000000 skdir-0.1.5/skdir.egg-info/SOURCES.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-04 03:14:45.000000 skdir-0.1.5/skdir.egg-info/dependency_links.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-04 03:14:45.000000 skdir-0.1.5/skdir.egg-info/requires.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-04 03:14:45.000000 skdir-0.1.5/skdir.egg-info/top_level.txt
```

### Comparing `skdir-0.1.4/LICENSE` & `skdir-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/PKG-INFO` & `skdir-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.1.4
+Version: 0.1.5
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
```

### Comparing `skdir-0.1.4/README.md` & `skdir-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/__init__.py` & `skdir-0.1.5/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/p1.py` & `skdir-0.1.5/lab/p1.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/p2.py` & `skdir-0.1.5/lab/p2.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/p3.py` & `skdir-0.1.5/lab/p3.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/p4.py` & `skdir-0.1.5/lab/p4.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/p5.py` & `skdir-0.1.5/lab/p5.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/p6.py` & `skdir-0.1.5/lab/p6.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/p7.py` & `skdir-0.1.5/lab/p7.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/lab/p8.py` & `skdir-0.1.5/lab/p8.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.4/setup.py` & `skdir-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'skdir'
 LONG_DESCRIPTION = 'A package to perform 5th sem AIML lab'
 
 # Setting up
 setup(
     name="skdir",
     version=VERSION,
```

### Comparing `skdir-0.1.4/skdir.egg-info/PKG-INFO` & `skdir-0.1.5/skdir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.1.4
+Version: 0.1.5
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
```

