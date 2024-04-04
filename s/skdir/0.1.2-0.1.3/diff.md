# Comparing `tmp/skdir-0.1.2.tar.gz` & `tmp/skdir-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skdir-0.1.2.tar", last modified: Wed Apr  3 19:28:22 2024, max compression
+gzip compressed data, was "skdir-0.1.3.tar", last modified: Thu Apr  4 02:59:59 2024, max compression
```

## Comparing `skdir-0.1.2.tar` & `skdir-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:28:22.583394 skdir-0.1.2/
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.1.2/LICENSE
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 19:28:22.583179 skdir-0.1.2/PKG-INFO
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.1.2/README.md
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:28:22.581829 skdir-0.1.2/lab/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      680 2024-04-03 19:27:29.000000 skdir-0.1.2/lab/__init__.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.1.2/lab/p1.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.1.2/lab/p2.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.1.2/lab/p3.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.1.2/lab/p4.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.1.2/lab/p5.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.1.2/lab/p6.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.1.2/lab/p7.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.1.2/lab/p8.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-03 19:28:22.583471 skdir-0.1.2/setup.cfg
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      930 2024-04-03 19:27:54.000000 skdir-0.1.2/setup.py
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-03 19:28:22.582847 skdir-0.1.2/skdir.egg-info/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      620 2024-04-03 19:28:22.000000 skdir-0.1.2/skdir.egg-info/PKG-INFO
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-03 19:28:22.000000 skdir-0.1.2/skdir.egg-info/SOURCES.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-03 19:28:22.000000 skdir-0.1.2/skdir.egg-info/dependency_links.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-03 19:28:22.000000 skdir-0.1.2/skdir.egg-info/requires.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-03 19:28:22.000000 skdir-0.1.2/skdir.egg-info/top_level.txt
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 02:59:59.467301 skdir-0.1.3/
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.1.3/LICENSE
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 02:59:59.467120 skdir-0.1.3/PKG-INFO
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.1.3/README.md
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 02:59:59.465758 skdir-0.1.3/lab/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      680 2024-04-04 02:52:48.000000 skdir-0.1.3/lab/__init__.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.1.3/lab/p1.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.1.3/lab/p2.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.1.3/lab/p3.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.1.3/lab/p4.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.1.3/lab/p5.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.1.3/lab/p6.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.1.3/lab/p7.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.1.3/lab/p8.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-04 02:59:59.467380 skdir-0.1.3/setup.cfg
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      925 2024-04-04 02:59:55.000000 skdir-0.1.3/setup.py
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 02:59:59.466831 skdir-0.1.3/skdir.egg-info/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/PKG-INFO
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/SOURCES.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/dependency_links.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/requires.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/top_level.txt
```

### Comparing `skdir-0.1.2/LICENSE` & `skdir-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/PKG-INFO` & `skdir-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.1.2
+Version: 0.1.3
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
@@ -13,9 +13,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package to perform arithmetic operations
+A package to perform 5th sem AIML lab
```

### Comparing `skdir-0.1.2/README.md` & `skdir-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/__init__.py` & `skdir-0.1.3/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/p1.py` & `skdir-0.1.3/lab/p1.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/p2.py` & `skdir-0.1.3/lab/p2.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/p3.py` & `skdir-0.1.3/lab/p3.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/p4.py` & `skdir-0.1.3/lab/p4.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/p5.py` & `skdir-0.1.3/lab/p5.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/p6.py` & `skdir-0.1.3/lab/p6.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/p7.py` & `skdir-0.1.3/lab/p7.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/lab/p8.py` & `skdir-0.1.3/lab/p8.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.2/setup.py` & `skdir-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'skdir'
-LONG_DESCRIPTION = 'A package to perform arithmetic operations'
+LONG_DESCRIPTION = 'A package to perform 5th sem AIML lab'
 
 # Setting up
 setup(
     name="skdir",
     version=VERSION,
     author="Sk",
     author_email="karnamsharath3@gmail.com",
```

### Comparing `skdir-0.1.2/skdir.egg-info/PKG-INFO` & `skdir-0.1.3/skdir.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.1.2
+Version: 0.1.3
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
@@ -13,9 +13,9 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package to perform arithmetic operations
+A package to perform 5th sem AIML lab
```

