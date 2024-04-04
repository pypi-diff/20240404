# Comparing `tmp/antoine-1.8.tar.gz` & `tmp/antoine-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antoine-1.8.tar", last modified: Thu Apr  4 13:36:38 2024, max compression
+gzip compressed data, was "antoine-1.9.tar", last modified: Thu Apr  4 13:56:36 2024, max compression
```

## Comparing `antoine-1.8.tar` & `antoine-1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:36:38.258667 antoine-1.8/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 13:36:38.258442 antoine-1.8/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      263 2024-04-04 13:29:29.000000 antoine-1.8/README.md
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:36:38.257667 antoine-1.8/antoine/
--rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-1.8/antoine/__init__.py
--rw-r--r--   0 antoinebertin   (501) staff       (20)     1443 2024-04-04 13:08:46.000000 antoine-1.8/antoine/app.py
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:36:38.258229 antoine-1.8/antoine.egg-info/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/SOURCES.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/dependency_links.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       52 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/entry_points.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-04 13:36:38.000000 antoine-1.8/antoine.egg-info/top_level.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-04 13:36:38.258704 antoine-1.8/setup.cfg
--rw-r--r--   0 antoinebertin   (501) staff       (20)      727 2024-04-04 13:36:22.000000 antoine-1.8/setup.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:56:36.701254 antoine-1.9/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 13:56:36.701056 antoine-1.9/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      263 2024-04-04 13:29:29.000000 antoine-1.9/README.md
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:56:36.700093 antoine-1.9/antoine/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-1.9/antoine/__init__.py
+-rw-r--r--   0 antoinebertin   (501) staff       (20)     1443 2024-04-04 13:08:46.000000 antoine-1.9/antoine/app.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-04 13:56:36.700783 antoine-1.9/antoine.egg-info/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-04 13:56:36.000000 antoine-1.9/antoine.egg-info/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-04 13:56:36.000000 antoine-1.9/antoine.egg-info/SOURCES.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-04 13:56:36.000000 antoine-1.9/antoine.egg-info/dependency_links.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       54 2024-04-04 13:56:36.000000 antoine-1.9/antoine.egg-info/entry_points.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-04 13:56:36.000000 antoine-1.9/antoine.egg-info/top_level.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-04 13:56:36.701295 antoine-1.9/setup.cfg
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      938 2024-04-04 13:55:38.000000 antoine-1.9/setup.py
```

### Comparing `antoine-1.8/antoine/app.py` & `antoine-1.9/antoine/app.py`

 * *Files identical despite different names*

