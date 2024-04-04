# Comparing `tmp/PyFaceCrop-0.0.2.tar.gz` & `tmp/PyFaceCrop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFaceCrop-0.0.2.tar", last modified: Wed Apr  3 10:21:03 2024, max compression
+gzip compressed data, was "PyFaceCrop-0.0.3.tar", last modified: Thu Apr  4 10:12:42 2024, max compression
```

## Comparing `PyFaceCrop-0.0.2.tar` & `PyFaceCrop-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 10:21:03.155194 PyFaceCrop-0.0.2/
--rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.2/LICENSE
--rw-r--r--   0 cdp        (501) staff       (20)      179 2024-04-03 10:21:03.154905 PyFaceCrop-0.0.2/PKG-INFO
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 10:21:03.153497 PyFaceCrop-0.0.2/PyFaceCrop/
--rw-r--r--   0 cdp        (501) staff       (20)     4414 2024-04-03 06:52:33.000000 PyFaceCrop-0.0.2/PyFaceCrop/FaceCrop.py
--rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.2/PyFaceCrop/__init__.py
--rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.2/PyFaceCrop/main.py
-drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-03 10:21:03.154498 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/
--rw-r--r--   0 cdp        (501) staff       (20)      179 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/PKG-INFO
--rw-r--r--   0 cdp        (501) staff       (20)      260 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/SOURCES.txt
--rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/dependency_links.txt
--rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/requires.txt
--rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-03 10:21:03.000000 PyFaceCrop-0.0.2/PyFaceCrop.egg-info/top_level.txt
--rw-r--r--   0 cdp        (501) staff       (20)       33 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.2/README.md
--rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-03 10:21:03.155257 PyFaceCrop-0.0.2/setup.cfg
--rw-r--r--   0 cdp        (501) staff       (20)      320 2024-04-03 10:19:54.000000 PyFaceCrop-0.0.2/setup.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:12:42.355910 PyFaceCrop-0.0.3/
+-rw-r--r--   0 cdp        (501) staff       (20)     1065 2024-04-03 06:26:46.000000 PyFaceCrop-0.0.3/LICENSE
+-rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:12:42.355623 PyFaceCrop-0.0.3/PKG-INFO
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:12:42.353973 PyFaceCrop-0.0.3/PyFaceCrop/
+-rw-r--r--   0 cdp        (501) staff       (20)     2704 2024-04-04 10:02:57.000000 PyFaceCrop-0.0.3/PyFaceCrop/FaceCrop.py
+-rw-r--r--   0 cdp        (501) staff       (20)       24 2024-04-03 06:29:52.000000 PyFaceCrop-0.0.3/PyFaceCrop/__init__.py
+-rw-r--r--   0 cdp        (501) staff       (20)      112 2024-04-03 07:19:43.000000 PyFaceCrop-0.0.3/PyFaceCrop/main.py
+drwxr-xr-x   0 cdp        (501) staff       (20)        0 2024-04-04 10:12:42.355140 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/
+-rw-r--r--   0 cdp        (501) staff       (20)     1650 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/PKG-INFO
+-rw-r--r--   0 cdp        (501) staff       (20)      260 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/SOURCES.txt
+-rw-r--r--   0 cdp        (501) staff       (20)        1 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/dependency_links.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       14 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/requires.txt
+-rw-r--r--   0 cdp        (501) staff       (20)       11 2024-04-04 10:12:42.000000 PyFaceCrop-0.0.3/PyFaceCrop.egg-info/top_level.txt
+-rw-r--r--   0 cdp        (501) staff       (20)     1504 2024-04-04 09:46:16.000000 PyFaceCrop-0.0.3/README.md
+-rw-r--r--   0 cdp        (501) staff       (20)       38 2024-04-04 10:12:42.355974 PyFaceCrop-0.0.3/setup.cfg
+-rw-r--r--   0 cdp        (501) staff       (20)      320 2024-04-04 09:58:23.000000 PyFaceCrop-0.0.3/setup.py
```

### Comparing `PyFaceCrop-0.0.2/LICENSE` & `PyFaceCrop-0.0.3/LICENSE`

 * *Files identical despite different names*

