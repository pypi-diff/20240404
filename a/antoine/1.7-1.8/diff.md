# Comparing `tmp/antoine-1.7.tar.gz` & `tmp/antoine-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antoine-1.7.tar", last modified: Thu Apr  4 13:24:03 2024, max compression
+gzip compressed data, was "antoine-1.8.tar", last modified: Thu Apr  4 13:36:38 2024, max compression
```

## Comparing `antoine-1.7.tar` & `antoine-1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:24:03.105708 antoine-1.7/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 13:24:03.105512 antoine-1.7/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      321 2024-04-04 13:18:28.000000 antoine-1.7/README.md
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:24:03.104651 antoine-1.7/antoine/
--rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-1.7/antoine/__init__.py
--rw-r--r--   0 antoinebertin   (501) staff       (20)     1443 2024-04-04 13:08:46.000000 antoine-1.7/antoine/app.py
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:24:03.105307 antoine-1.7/antoine.egg-info/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 13:24:03.000000 antoine-1.7/antoine.egg-info/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-04 13:24:03.000000 antoine-1.7/antoine.egg-info/SOURCES.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-04 13:24:03.000000 antoine-1.7/antoine.egg-info/dependency_links.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       52 2024-04-04 13:24:03.000000 antoine-1.7/antoine.egg-info/entry_points.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-04 13:24:03.000000 antoine-1.7/antoine.egg-info/top_level.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-04 13:24:03.105741 antoine-1.7/setup.cfg
--rw-r--r--   0 antoinebertin   (501) staff       (20)      727 2024-04-04 13:23:26.000000 antoine-1.7/setup.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:36:38.258667 antoine-1.8/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 13:36:38.258442 antoine-1.8/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      263 2024-04-04 13:29:29.000000 antoine-1.8/README.md
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:36:38.257667 antoine-1.8/antoine/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-1.8/antoine/__init__.py
+-rw-r--r--   0 antoinebertin   (501) staff       (20)     1443 2024-04-04 13:08:46.000000 antoine-1.8/antoine/app.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:36:38.258229 antoine-1.8/antoine.egg-info/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/SOURCES.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/dependency_links.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       52 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/entry_points.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/top_level.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-04 13:36:38.258704 antoine-1.8/setup.cfg
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      727 2024-04-04 13:36:22.000000 antoine-1.8/setup.py
```

### Comparing `antoine-1.7/antoine/app.py` & `antoine-1.8/antoine/app.py`

 * *Files identical despite different names*

### Comparing `antoine-1.7/setup.py` & `antoine-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 # Print a message before installation
 print("Installing Antoine...")
 
 setup(
     name='antoine',
-    version='1.7',
+    version='1.8',
     packages=['antoine'],  # 'antoine' is the name of the package
     author='Antoine Bertin',
     author_email='monolok35@gmail.com',
     description='Hiring Antoine is so much fun!',
     url='https://github.com/monolok/antoine/',
     license='MIT',
     entry_points={
```

