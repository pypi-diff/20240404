# Comparing `tmp/libWiiPy-0.1.0.tar.gz` & `tmp/libWiiPy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libWiiPy-0.1.0.tar", last modified: Thu Feb 29 04:58:58 2024, max compression
+gzip compressed data, was "libWiiPy-0.2.0.tar", last modified: Wed Apr  3 22:16:31 2024, max compression
```

## Comparing `libWiiPy-0.1.0.tar` & `libWiiPy-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-02-29 04:58:58.439246 libWiiPy-0.1.0/
--rw-r--r--   0 campbell  (1000) campbell  (1000)     1056 2024-02-06 23:30:14.000000 libWiiPy-0.1.0/LICENSE
--rw-r--r--   0 campbell  (1000) campbell  (1000)     3060 2024-02-29 04:58:58.439246 libWiiPy-0.1.0/PKG-INFO
--rw-r--r--   0 campbell  (1000) campbell  (1000)     2480 2024-02-27 01:27:07.000000 libWiiPy-0.1.0/README.md
--rw-r--r--   0 campbell  (1000) campbell  (1000)      673 2024-02-29 04:54:33.000000 libWiiPy-0.1.0/pyproject.toml
--rw-r--r--   0 campbell  (1000) campbell  (1000)       38 2024-02-29 04:58:58.439246 libWiiPy-0.1.0/setup.cfg
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-02-29 04:58:58.435912 libWiiPy-0.1.0/src/
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-02-29 04:58:58.439246 libWiiPy-0.1.0/src/libWiiPy/
--rw-r--r--   0 campbell  (1000) campbell  (1000)        0 2024-02-06 23:23:02.000000 libWiiPy-0.1.0/src/libWiiPy/__init__.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)      614 2024-02-29 04:54:33.000000 libWiiPy-0.1.0/src/libWiiPy/commonkeys.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)      215 2024-02-07 02:00:49.000000 libWiiPy-0.1.0/src/libWiiPy/shared.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     6801 2024-02-29 04:54:33.000000 libWiiPy-0.1.0/src/libWiiPy/tmd.py
--rw-r--r--   0 campbell  (1000) campbell  (1000)     5860 2024-02-29 04:54:33.000000 libWiiPy-0.1.0/src/libWiiPy/wad.py
-drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-02-29 04:58:58.439246 libWiiPy-0.1.0/src/libWiiPy.egg-info/
--rw-r--r--   0 campbell  (1000) campbell  (1000)     3060 2024-02-29 04:58:58.000000 libWiiPy-0.1.0/src/libWiiPy.egg-info/PKG-INFO
--rw-r--r--   0 campbell  (1000) campbell  (1000)      291 2024-02-29 04:58:58.000000 libWiiPy-0.1.0/src/libWiiPy.egg-info/SOURCES.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)        1 2024-02-29 04:58:58.000000 libWiiPy-0.1.0/src/libWiiPy.egg-info/dependency_links.txt
--rw-r--r--   0 campbell  (1000) campbell  (1000)        9 2024-02-29 04:58:58.000000 libWiiPy-0.1.0/src/libWiiPy.egg-info/top_level.txt
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1056 2024-02-06 23:30:14.000000 libWiiPy-0.2.0/LICENSE
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4537 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/PKG-INFO
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     3903 2024-04-03 22:05:00.000000 libWiiPy-0.2.0/README.md
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      738 2024-03-08 05:11:53.000000 libWiiPy-0.2.0/pyproject.toml
+-rw-r--r--   0 campbell  (1000) campbell  (1000)       38 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/setup.cfg
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/src/
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/src/libWiiPy/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      331 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/__init__.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1086 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/commonkeys.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    16468 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/content.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4301 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/crypto.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1181 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/shared.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    11921 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/ticket.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     9062 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/title.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    13738 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/tmd.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     1938 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/types.py
+-rw-r--r--   0 campbell  (1000) campbell  (1000)    12583 2024-04-03 22:05:07.000000 libWiiPy-0.2.0/src/libWiiPy/wad.py
+drwxr-xr-x   0 campbell  (1000) campbell  (1000)        0 2024-04-03 22:16:31.515271 libWiiPy-0.2.0/src/libWiiPy.egg-info/
+-rw-r--r--   0 campbell  (1000) campbell  (1000)     4537 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/PKG-INFO
+-rw-r--r--   0 campbell  (1000) campbell  (1000)      440 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/SOURCES.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)        1 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/dependency_links.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)       13 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/requires.txt
+-rw-r--r--   0 campbell  (1000) campbell  (1000)        9 2024-04-03 22:16:31.000000 libWiiPy-0.2.0/src/libWiiPy.egg-info/top_level.txt
```

### Comparing `libWiiPy-0.1.0/LICENSE` & `libWiiPy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libWiiPy-0.1.0/pyproject.toml` & `libWiiPy-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [project]
 name = "libWiiPy"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name="NinjaCheetah", email="ninjacheetah@ncxprogramming.com" },
     { name="Lillian Skinner", email="lillian@randommeaninglesscharacters.com" }
 ]
-description = "A Wii-related library for Python"
+description = "A modern Python library for handling files used by the Wii"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "pycryptodome",
+]
 
 [project.urls]
 Homepage = "https://github.com/NinjaCheetah/libWiiPy"
 Issues = "https://github.com/NinjaCheetah/libWiipy/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
```

