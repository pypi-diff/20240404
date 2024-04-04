# Comparing `tmp/skdir-0.1.3.tar.gz` & `tmp/skdir-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skdir-0.1.3.tar", last modified: Thu Apr  4 02:59:59 2024, max compression
+gzip compressed data, was "skdir-0.1.4.tar", last modified: Thu Apr  4 03:05:57 2024, max compression
```

## Comparing `skdir-0.1.3.tar` & `skdir-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 02:59:59.467301 skdir-0.1.3/
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.1.3/LICENSE
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 02:59:59.467120 skdir-0.1.3/PKG-INFO
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.1.3/README.md
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 02:59:59.465758 skdir-0.1.3/lab/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      680 2024-04-04 02:52:48.000000 skdir-0.1.3/lab/__init__.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.1.3/lab/p1.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.1.3/lab/p2.py
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.1.3/lab/p3.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.1.3/lab/p4.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.1.3/lab/p5.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.1.3/lab/p6.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.1.3/lab/p7.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.1.3/lab/p8.py
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-04 02:59:59.467380 skdir-0.1.3/setup.cfg
--rw-rw-r--   0 sharathchandrak   (501) staff       (20)      925 2024-04-04 02:59:55.000000 skdir-0.1.3/setup.py
-drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 02:59:59.466831 skdir-0.1.3/skdir.egg-info/
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/PKG-INFO
--rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/SOURCES.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/dependency_links.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/requires.txt
--rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-04 02:59:59.000000 skdir-0.1.3/skdir.egg-info/top_level.txt
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:05:57.010275 skdir-0.1.4/
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     1064 2021-07-27 04:28:46.000000 skdir-0.1.4/LICENSE
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 03:05:57.010064 skdir-0.1.4/PKG-INFO
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      981 2021-07-27 04:28:46.000000 skdir-0.1.4/README.md
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:05:57.008728 skdir-0.1.4/lab/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      561 2024-04-04 03:05:16.000000 skdir-0.1.4/lab/__init__.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     2873 2024-04-03 16:35:15.000000 skdir-0.1.4/lab/p1.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      985 2024-04-03 16:35:24.000000 skdir-0.1.4/lab/p2.py
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)     4208 2024-04-03 16:35:34.000000 skdir-0.1.4/lab/p3.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1701 2024-04-03 16:36:03.000000 skdir-0.1.4/lab/p4.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1808 2024-04-03 16:36:40.000000 skdir-0.1.4/lab/p5.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1798 2024-04-03 16:36:57.000000 skdir-0.1.4/lab/p6.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1869 2024-04-03 16:37:20.000000 skdir-0.1.4/lab/p7.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)     1111 2024-04-03 16:38:04.000000 skdir-0.1.4/lab/p8.py
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       38 2024-04-04 03:05:57.010351 skdir-0.1.4/setup.cfg
+-rw-rw-r--   0 sharathchandrak   (501) staff       (20)      925 2024-04-04 03:05:52.000000 skdir-0.1.4/setup.py
+drwxr-xr-x   0 sharathchandrak   (501) staff       (20)        0 2024-04-04 03:05:57.009773 skdir-0.1.4/skdir.egg-info/
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      615 2024-04-04 03:05:56.000000 skdir-0.1.4/skdir.egg-info/PKG-INFO
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)      266 2024-04-04 03:05:57.000000 skdir-0.1.4/skdir.egg-info/SOURCES.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        1 2024-04-04 03:05:56.000000 skdir-0.1.4/skdir.egg-info/dependency_links.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)       53 2024-04-04 03:05:57.000000 skdir-0.1.4/skdir.egg-info/requires.txt
+-rw-r--r--   0 sharathchandrak   (501) staff       (20)        4 2024-04-04 03:05:57.000000 skdir-0.1.4/skdir.egg-info/top_level.txt
```

### Comparing `skdir-0.1.3/LICENSE` & `skdir-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/PKG-INFO` & `skdir-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.1.3
+Version: 0.1.4
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
```

### Comparing `skdir-0.1.3/README.md` & `skdir-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/lab/__init__.py` & `skdir-0.1.4/lab/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-# __init__.py
-
-# Import any modules or symbols needed for printing the AIML code files
 import os
 
 # Define the directory path where the AIML code files are located
 AIML_CODE_DIR = '/Users/sharathchandrak/Desktop/avi_package-main/lab'
 
-# Function to print the contents of AIML code files
-def print_aiml_code_file(filename):
-    file_path = os.path.join(AIML_CODE_DIR, filename)
-    if os.path.exists(file_path):
-        with open(file_path, 'r') as file:
-            print(f"Contents of {filename}:")
-            print(file.read())
-    else:
-        print(f"File {filename} does not exist.")
-def Print(filename):
-    print_aiml_code_file(filename)
+# Function to print the contents of all AIML code files
+def print_all_aiml_code_files():
+    for filename in os.listdir(AIML_CODE_DIR):
+        if filename.endswith(".py"):
+            file_path = os.path.join(AIML_CODE_DIR, filename)
+            with open(file_path, 'r') as file:
+                print(f"Contents of {filename}:")
+                print(file.read())
+
 # Example usage:
-Print('p1.py') 
+print_all_aiml_code_files()
```

### Comparing `skdir-0.1.3/lab/p1.py` & `skdir-0.1.4/lab/p1.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/lab/p2.py` & `skdir-0.1.4/lab/p2.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/lab/p3.py` & `skdir-0.1.4/lab/p3.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/lab/p4.py` & `skdir-0.1.4/lab/p4.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/lab/p5.py` & `skdir-0.1.4/lab/p5.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/lab/p6.py` & `skdir-0.1.4/lab/p6.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/lab/p7.py` & `skdir-0.1.4/lab/p7.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/lab/p8.py` & `skdir-0.1.4/lab/p8.py`

 * *Files identical despite different names*

### Comparing `skdir-0.1.3/setup.py` & `skdir-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 DESCRIPTION = 'skdir'
 LONG_DESCRIPTION = 'A package to perform 5th sem AIML lab'
 
 # Setting up
 setup(
     name="skdir",
     version=VERSION,
```

### Comparing `skdir-0.1.3/skdir.egg-info/PKG-INFO` & `skdir-0.1.4/skdir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skdir
-Version: 0.1.3
+Version: 0.1.4
 Summary: skdir
 Home-page: UNKNOWN
 Author: Sk
 Author-email: karnamsharath3@gmail.com
 License: UNKNOWN
 Keywords: arithmetic,math,mathematics,python tutorial,avi upadhyay
 Platform: UNKNOWN
```

