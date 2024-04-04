# Comparing `tmp/salure_helpers_leapsome-1.0.0.tar.gz` & `tmp/salure_helpers_leapsome-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_leapsome-1.0.0.tar", last modified: Mon Dec 18 17:40:39 2023, max compression
+gzip compressed data, was "dist/salure_helpers_leapsome-1.2.0.tar", last modified: Thu Apr  4 09:59:33 2024, max compression
```

## Comparing `salure_helpers_leapsome-1.0.0.tar` & `salure_helpers_leapsome-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      268 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers/leapsome/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-12-18 17:40:26.000000 salure_helpers_leapsome-1.0.0/salure_helpers/leapsome/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3869 2023-12-18 17:40:26.000000 salure_helpers_leapsome-1.0.0/salure_helpers/leapsome/sftp_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers_leapsome.egg-info/
--rw-r--r--   0 root         (0) root         (0)      268 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers_leapsome.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      366 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers_leapsome.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers_leapsome.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers_leapsome.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       89 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers_leapsome.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/salure_helpers_leapsome.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-18 17:40:39.000000 salure_helpers_leapsome-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      534 2023-12-18 17:40:26.000000 salure_helpers_leapsome-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-04 09:59:16.000000 salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4576 2024-04-04 09:59:16.000000 salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/api_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     3869 2024-04-04 09:59:16.000000 salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/sftp_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       89 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/salure_helpers_leapsome.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 09:59:33.000000 salure_helpers_leapsome-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      534 2024-04-04 09:59:16.000000 salure_helpers_leapsome-1.2.0/setup.py
```

### Comparing `salure_helpers_leapsome-1.0.0/salure_helpers/leapsome/sftp_interface.py` & `salure_helpers_leapsome-1.2.0/salure_helpers/leapsome/sftp_interface.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_leapsome-1.0.0/setup.py` & `salure_helpers_leapsome-1.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='salure_helpers_leapsome',
-    version='1.0.0',
+    version='1.2.0',
     description='Leapsome wrapper from Salure',
     long_description='Leapsome wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.leapsome"],
     license='Salure License',
     install_requires=[
```

