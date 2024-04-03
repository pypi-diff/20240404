# Comparing `tmp/mattsollamatools-0.0.8.tar.gz` & `tmp/mattsollamatools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattsollamatools-0.0.8.tar", last modified: Tue Oct 17 22:37:35 2023, max compression
+gzip compressed data, was "mattsollamatools-0.0.9.tar", last modified: Tue Oct 17 22:47:38 2023, max compression
```

## Comparing `mattsollamatools-0.0.8.tar` & `mattsollamatools-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-10-17 22:37:35.378883 mattsollamatools-0.0.8/
--rw-r--r--   0 matt       (501) staff       (20)      326 2023-10-17 22:37:35.378826 mattsollamatools-0.0.8/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)       21 2023-10-17 21:51:25.000000 mattsollamatools-0.0.8/README.md
--rw-r--r--   0 matt       (501) staff       (20)       93 2023-10-17 22:23:50.000000 mattsollamatools-0.0.8/pyproject.toml
--rw-r--r--   0 matt       (501) staff       (20)      470 2023-10-17 22:37:35.379085 mattsollamatools-0.0.8/setup.cfg
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-10-17 22:37:35.377616 mattsollamatools-0.0.8/src/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-10-17 22:37:35.378178 mattsollamatools-0.0.8/src/mattsollamatools/
--rw-r--r--   0 matt       (501) staff       (20)       26 2023-10-17 22:37:20.000000 mattsollamatools-0.0.8/src/mattsollamatools/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)      945 2023-10-17 22:03:32.000000 mattsollamatools-0.0.8/src/mattsollamatools/tools.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-10-17 22:37:35.378651 mattsollamatools-0.0.8/src/mattsollamatools.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)      326 2023-10-17 22:37:35.000000 mattsollamatools-0.0.8/src/mattsollamatools.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      273 2023-10-17 22:37:35.000000 mattsollamatools-0.0.8/src/mattsollamatools.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2023-10-17 22:37:35.000000 mattsollamatools-0.0.8/src/mattsollamatools.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)       17 2023-10-17 22:37:35.000000 mattsollamatools-0.0.8/src/mattsollamatools.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-10-17 22:47:38.479926 mattsollamatools-0.0.9/
+-rw-r--r--   0 matt       (501) staff       (20)      326 2023-10-17 22:47:38.479860 mattsollamatools-0.0.9/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      723 2023-10-17 22:47:19.000000 mattsollamatools-0.0.9/README.md
+-rw-r--r--   0 matt       (501) staff       (20)       93 2023-10-17 22:23:50.000000 mattsollamatools-0.0.9/pyproject.toml
+-rw-r--r--   0 matt       (501) staff       (20)      470 2023-10-17 22:47:38.480172 mattsollamatools-0.0.9/setup.cfg
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-10-17 22:47:38.478651 mattsollamatools-0.0.9/src/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-10-17 22:47:38.479192 mattsollamatools-0.0.9/src/mattsollamatools/
+-rw-r--r--   0 matt       (501) staff       (20)       26 2023-10-17 22:37:20.000000 mattsollamatools-0.0.9/src/mattsollamatools/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)      945 2023-10-17 22:03:32.000000 mattsollamatools-0.0.9/src/mattsollamatools/tools.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-10-17 22:47:38.479621 mattsollamatools-0.0.9/src/mattsollamatools.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)      326 2023-10-17 22:47:38.000000 mattsollamatools-0.0.9/src/mattsollamatools.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      273 2023-10-17 22:47:38.000000 mattsollamatools-0.0.9/src/mattsollamatools.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-10-17 22:47:38.000000 mattsollamatools-0.0.9/src/mattsollamatools.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)       17 2023-10-17 22:47:38.000000 mattsollamatools-0.0.9/src/mattsollamatools.egg-info/top_level.txt
```

### Comparing `mattsollamatools-0.0.8/src/mattsollamatools/tools.py` & `mattsollamatools-0.0.9/src/mattsollamatools/tools.py`

 * *Files identical despite different names*

