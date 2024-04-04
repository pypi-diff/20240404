# Comparing `tmp/MLstatkit-0.1.3.tar.gz` & `tmp/MLstatkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLstatkit-0.1.3.tar", last modified: Tue Apr  2 04:39:42 2024, max compression
+gzip compressed data, was "MLstatkit-0.1.4.tar", last modified: Thu Apr  4 08:06:07 2024, max compression
```

## Comparing `MLstatkit-0.1.3.tar` & `MLstatkit-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-02 04:39:42.596489 MLstatkit-0.1.3/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1072 2024-04-01 20:44:17.000000 MLstatkit-0.1.3/LICENSE
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-02 04:39:42.595671 MLstatkit-0.1.3/MLstatkit/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:44:17.000000 MLstatkit-0.1.3/MLstatkit/__init__.py
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     6446 2024-04-01 21:39:19.000000 MLstatkit-0.1.3/MLstatkit/stats.py
-drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-02 04:39:42.596199 MLstatkit-0.1.3/MLstatkit.egg-info/
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     7779 2024-04-02 04:39:42.000000 MLstatkit-0.1.3/MLstatkit.egg-info/PKG-INFO
--rw-r--r--   0 brritanyhuang   (501) staff       (20)      231 2024-04-02 04:39:42.000000 MLstatkit-0.1.3/MLstatkit.egg-info/SOURCES.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)        1 2024-04-02 04:39:42.000000 MLstatkit-0.1.3/MLstatkit.egg-info/dependency_links.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       37 2024-04-02 04:39:42.000000 MLstatkit-0.1.3/MLstatkit.egg-info/requires.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       10 2024-04-02 04:39:42.000000 MLstatkit-0.1.3/MLstatkit.egg-info/top_level.txt
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     7779 2024-04-02 04:39:42.596362 MLstatkit-0.1.3/PKG-INFO
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     6732 2024-04-02 04:38:12.000000 MLstatkit-0.1.3/README.md
--rw-r--r--   0 brritanyhuang   (501) staff       (20)       38 2024-04-02 04:39:42.596532 MLstatkit-0.1.3/setup.cfg
--rw-r--r--   0 brritanyhuang   (501) staff       (20)     1398 2024-04-02 04:39:08.000000 MLstatkit-0.1.3/setup.py
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-04 08:06:07.686036 MLstatkit-0.1.4/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1072 2024-04-01 20:44:17.000000 MLstatkit-0.1.4/LICENSE
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-04 08:06:07.685031 MLstatkit-0.1.4/MLstatkit/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        0 2024-04-01 20:44:17.000000 MLstatkit-0.1.4/MLstatkit/__init__.py
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)    10084 2024-04-04 08:05:59.000000 MLstatkit-0.1.4/MLstatkit/stats.py
+drwxr-xr-x   0 brritanyhuang   (501) staff       (20)        0 2024-04-04 08:06:07.685579 MLstatkit-0.1.4/MLstatkit.egg-info/
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)    11840 2024-04-04 08:06:07.000000 MLstatkit-0.1.4/MLstatkit.egg-info/PKG-INFO
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)      231 2024-04-04 08:06:07.000000 MLstatkit-0.1.4/MLstatkit.egg-info/SOURCES.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)        1 2024-04-04 08:06:07.000000 MLstatkit-0.1.4/MLstatkit.egg-info/dependency_links.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       37 2024-04-04 08:06:07.000000 MLstatkit-0.1.4/MLstatkit.egg-info/requires.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       10 2024-04-04 08:06:07.000000 MLstatkit-0.1.4/MLstatkit.egg-info/top_level.txt
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)    11840 2024-04-04 08:06:07.685781 MLstatkit-0.1.4/PKG-INFO
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)    10793 2024-04-04 08:04:35.000000 MLstatkit-0.1.4/README.md
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)       38 2024-04-04 08:06:07.686085 MLstatkit-0.1.4/setup.cfg
+-rw-r--r--   0 brritanyhuang   (501) staff       (20)     1398 2024-04-04 08:04:56.000000 MLstatkit-0.1.4/setup.py
```

### Comparing `MLstatkit-0.1.3/LICENSE` & `MLstatkit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MLstatkit-0.1.3/setup.py` & `MLstatkit-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MLstatkit",
-    version="0.1.3",
+    version="0.1.4",
     description="MLstatkit is a comprehensive Python library designed to seamlessly integrate established statistical methods into machine learning projects.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Brritany/MLstatkit',
     project_urls={
         'Tracker': 'https://github.com/Brritany/MLstatkit/issues',
     },
```

