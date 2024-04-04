# Comparing `tmp/piholesdk-0.1.0.tar.gz` & `tmp/piholesdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piholesdk-0.1.0.tar", last modified: Thu Apr  4 14:58:04 2024, max compression
+gzip compressed data, was "piholesdk-0.1.1.tar", last modified: Thu Apr  4 18:32:39 2024, max compression
```

## Comparing `piholesdk-0.1.0.tar` & `piholesdk-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:58:04.921254 piholesdk-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 14:58:04.921254 piholesdk-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 14:57:58.000000 piholesdk-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:58:04.921254 piholesdk-0.1.0/piholesdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:57:58.000000 piholesdk-0.1.0/piholesdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:57:58.000000 piholesdk-0.1.0/piholesdk/piholesdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:58:04.921254 piholesdk-0.1.0/piholesdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 14:58:04.000000 piholesdk-0.1.0/piholesdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 14:58:04.000000 piholesdk-0.1.0/piholesdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:58:04.000000 piholesdk-0.1.0/piholesdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 14:58:04.000000 piholesdk-0.1.0/piholesdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 14:58:04.000000 piholesdk-0.1.0/piholesdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:58:04.921254 piholesdk-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-04 14:57:58.000000 piholesdk-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:58:04.921254 piholesdk-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:57:58.000000 piholesdk-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:57:58.000000 piholesdk-0.1.0/tests/test_piholesdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:39.708562 piholesdk-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 18:32:39.708562 piholesdk-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 18:32:35.000000 piholesdk-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:39.708562 piholesdk-0.1.1/piholesdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 18:32:35.000000 piholesdk-0.1.1/piholesdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 18:32:35.000000 piholesdk-0.1.1/piholesdk/piholesdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:39.708562 piholesdk-0.1.1/piholesdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:32:39.708562 piholesdk-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-04 18:32:35.000000 piholesdk-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:39.708562 piholesdk-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:35.000000 piholesdk-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:35.000000 piholesdk-0.1.1/tests/test_piholesdk.py
```

### Comparing `piholesdk-0.1.0/setup.py` & `piholesdk-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="piholesdk",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     author="Melih Teke",
     author_email="me@mteke.com",
     description="A Python client for managing DNS records on a Pi-hole server via SSH.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/melihteke/piholesdk.git",
@@ -15,8 +15,8 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         'paramiko',
     ],
-)
+)
```

