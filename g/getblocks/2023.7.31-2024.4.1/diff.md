# Comparing `tmp/getblocks-2023.7.31.tar.gz` & `tmp/getblocks-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-2023.7.31.tar", last modified: Tue Aug  1 00:59:58 2023, max compression
+gzip compressed data, was "getblocks-2024.4.1.tar", last modified: Wed Apr  3 23:45:56 2024, max compression
```

## Comparing `getblocks-2023.7.31.tar` & `getblocks-2024.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:59:58.726213 getblocks-2023.7.31/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 00:59:48.000000 getblocks-2023.7.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-01 00:59:58.726213 getblocks-2023.7.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-01 00:59:48.000000 getblocks-2023.7.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:59:58.722213 getblocks-2023.7.31/getblocks/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 00:59:48.000000 getblocks-2023.7.31/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-01 00:59:48.000000 getblocks-2023.7.31/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-08-01 00:59:48.000000 getblocks-2023.7.31/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 00:59:58.726213 getblocks-2023.7.31/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 00:59:58.000000 getblocks-2023.7.31/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 00:59:58.726213 getblocks-2023.7.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-01 00:59:48.000000 getblocks-2023.7.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:45:56.589134 getblocks-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 23:45:52.000000 getblocks-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 23:45:56.589134 getblocks-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 23:45:52.000000 getblocks-2024.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:45:56.589134 getblocks-2024.4.1/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 23:45:52.000000 getblocks-2024.4.1/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 23:45:52.000000 getblocks-2024.4.1/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-03 23:45:52.000000 getblocks-2024.4.1/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:45:56.589134 getblocks-2024.4.1/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:45:56.589134 getblocks-2024.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 23:45:52.000000 getblocks-2024.4.1/setup.py
```

### Comparing `getblocks-2023.7.31/LICENSE` & `getblocks-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-2023.7.31/PKG-INFO` & `getblocks-2024.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2023.7.31
+Version: 2024.4.1
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/jblukach/getblocks
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: blake3
+Requires-Dist: requests==2.29.0
 
 # getblocks
 
 ### NORMALIZATION
 
 Clean data is mission-critical for collecting operating system artifacts, especially with user home directories.
```

### Comparing `getblocks-2023.7.31/README.md` & `getblocks-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `getblocks-2023.7.31/getblocks/cli.py` & `getblocks-2024.4.1/getblocks/cli.py`

 * *Files identical despite different names*

### Comparing `getblocks-2023.7.31/getblocks.egg-info/PKG-INFO` & `getblocks-2024.4.1/getblocks.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2023.7.31
+Version: 2024.4.1
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/jblukach/getblocks
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: blake3
+Requires-Dist: requests==2.29.0
 
 # getblocks
 
 ### NORMALIZATION
 
 Clean data is mission-critical for collecting operating system artifacts, especially with user home directories.
```

### Comparing `getblocks-2023.7.31/setup.py` & `getblocks-2024.4.1/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     zip_safe = False,
     entry_points = {
         "console_scripts": [
             "getblocks=getblocks.cli:main"
         ],
     },
     python_requires = ">=3.7",
-)
+)
```

