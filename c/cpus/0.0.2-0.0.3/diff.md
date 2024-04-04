# Comparing `tmp/cpus-0.0.2.tar.gz` & `tmp/cpus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpus-0.0.2.tar", last modified: Tue Dec 19 15:08:49 2023, max compression
+gzip compressed data, was "cpus-0.0.3.tar", last modified: Thu Apr  4 12:31:11 2024, max compression
```

## Comparing `cpus-0.0.2.tar` & `cpus-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-19 15:08:49.440288 cpus-0.0.2/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-12-19 13:56:38.000000 cpus-0.0.2/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-12-19 13:56:38.000000 cpus-0.0.2/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2038 2023-12-19 15:08:49.440157 cpus-0.0.2/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1431 2023-12-19 14:21:08.000000 cpus-0.0.2/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-19 15:08:49.439050 cpus-0.0.2/cpus/
--rw-r--r--   0 solst      (501) staff       (20)      323 2023-12-19 15:08:47.000000 cpus-0.0.2/cpus/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)      836 2023-12-19 15:08:47.000000 cpus-0.0.2/cpus/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1852 2023-12-19 15:08:47.000000 cpus-0.0.2/cpus/core.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-19 15:08:49.439997 cpus-0.0.2/cpus.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2038 2023-12-19 15:08:49.000000 cpus-0.0.2/cpus.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      294 2023-12-19 15:08:49.000000 cpus-0.0.2/cpus.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-12-19 15:08:49.000000 cpus-0.0.2/cpus.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-12-19 15:08:49.000000 cpus-0.0.2/cpus.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-12-19 14:21:39.000000 cpus-0.0.2/cpus.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       21 2023-12-19 15:08:49.000000 cpus-0.0.2/cpus.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-12-19 15:08:49.000000 cpus-0.0.2/cpus.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      816 2023-12-19 15:08:06.000000 cpus-0.0.2/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-12-19 15:08:49.440325 cpus-0.0.2/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2023-12-19 13:56:38.000000 cpus-0.0.2/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:31:11.673821 cpus-0.0.3/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-12-19 13:56:38.000000 cpus-0.0.3/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-12-19 13:56:38.000000 cpus-0.0.3/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2038 2024-04-04 12:31:11.673683 cpus-0.0.3/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1431 2023-12-19 14:21:08.000000 cpus-0.0.3/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:31:11.672381 cpus-0.0.3/cpus/
+-rw-r--r--   0 solst      (501) staff       (20)      323 2024-04-04 12:31:08.000000 cpus-0.0.3/cpus/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     1712 2024-04-04 12:31:08.000000 cpus-0.0.3/cpus/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     7757 2024-04-04 12:31:08.000000 cpus-0.0.3/cpus/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:31:11.673516 cpus-0.0.3/cpus.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2038 2024-04-04 12:31:11.000000 cpus-0.0.3/cpus.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      294 2024-04-04 12:31:11.000000 cpus-0.0.3/cpus.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-04 12:31:11.000000 cpus-0.0.3/cpus.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-04 12:31:11.000000 cpus-0.0.3/cpus.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-12-19 14:21:39.000000 cpus-0.0.3/cpus.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       21 2024-04-04 12:31:11.000000 cpus-0.0.3/cpus.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-04 12:31:11.000000 cpus-0.0.3/cpus.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      816 2023-12-19 15:10:03.000000 cpus-0.0.3/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-04 12:31:11.673873 cpus-0.0.3/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2023-12-19 13:56:38.000000 cpus-0.0.3/setup.py
```

### Comparing `cpus-0.0.2/LICENSE` & `cpus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpus-0.0.2/PKG-INFO` & `cpus-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpus
-Version: 0.0.2
+Version: 0.0.3
 Summary: cpus
 Home-page: https://github.com/dsm-72/cpus
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: cpus is question bool type guard typeguard check cpus
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cpus-0.0.2/README.md` & `cpus-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cpus-0.0.2/cpus.egg-info/PKG-INFO` & `cpus-0.0.3/cpus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpus
-Version: 0.0.2
+Version: 0.0.3
 Summary: cpus
 Home-page: https://github.com/dsm-72/cpus
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: cpus is question bool type guard typeguard check cpus
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cpus-0.0.2/settings.ini` & `cpus-0.0.3/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = cpus
 lib_name = cpus
-version = 0.0.2
+version = 0.0.3
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = cpus
 nbs_path = nbs
 recursive = True
```

### Comparing `cpus-0.0.2/setup.py` & `cpus-0.0.3/setup.py`

 * *Files identical despite different names*

