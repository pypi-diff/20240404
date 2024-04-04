# Comparing `tmp/qfpy-4.0.3.tar.gz` & `tmp/qfpy-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-4.0.3.tar", last modified: Wed Mar 27 09:58:16 2024, max compression
+gzip compressed data, was "qfpy-5.0.0.tar", last modified: Thu Apr  4 17:54:09 2024, max compression
```

## Comparing `qfpy-4.0.3.tar` & `qfpy-5.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 09:58:16.330511 qfpy-4.0.3/
--rw-rw-rw-   0        0        0      159 2024-03-27 09:58:16.329513 qfpy-4.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-03-27 09:58:06.000000 qfpy-4.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 09:58:16.330511 qfpy-4.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-27 09:58:16.311514 qfpy-4.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-27 09:58:16.319514 qfpy-4.0.3/src/qfpy/
--rw-rw-rw-   0        0        0       29 2024-03-06 16:44:46.000000 qfpy-4.0.3/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0     1393 2024-03-27 09:56:39.000000 qfpy-4.0.3/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     3083 2024-03-23 10:22:51.000000 qfpy-4.0.3/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      845 2024-03-23 10:23:45.000000 qfpy-4.0.3/src/qfpy/func.py
--rw-rw-rw-   0        0        0      804 2024-03-23 10:20:43.000000 qfpy-4.0.3/src/qfpy/process.py
-drwxrwxrwx   0        0        0        0 2024-03-27 09:58:16.327554 qfpy-4.0.3/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      159 2024-03-27 09:58:16.000000 qfpy-4.0.3/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-03-27 09:58:16.000000 qfpy-4.0.3/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 09:58:16.000000 qfpy-4.0.3/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-27 09:58:16.000000 qfpy-4.0.3/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 17:54:09.527212 qfpy-5.0.0/
+-rw-rw-rw-   0        0        0      159 2024-04-04 17:54:09.525278 qfpy-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-04 17:53:58.000000 qfpy-5.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 17:54:09.527212 qfpy-5.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 17:54:09.496366 qfpy-5.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 17:54:09.512562 qfpy-5.0.0/src/qfpy/
+-rw-rw-rw-   0        0        0       29 2024-03-06 16:44:46.000000 qfpy-5.0.0/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0     1393 2024-03-27 09:56:39.000000 qfpy-5.0.0/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     3083 2024-03-23 10:22:51.000000 qfpy-5.0.0/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      427 2024-04-04 17:53:45.000000 qfpy-5.0.0/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      845 2024-03-23 10:23:45.000000 qfpy-5.0.0/src/qfpy/func.py
+-rw-rw-rw-   0        0        0      804 2024-03-23 10:20:43.000000 qfpy-5.0.0/src/qfpy/process.py
+drwxrwxrwx   0        0        0        0 2024-04-04 17:54:09.523304 qfpy-5.0.0/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-04-04 17:54:09.000000 qfpy-5.0.0/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-04 17:54:09.000000 qfpy-5.0.0/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 17:54:09.000000 qfpy-5.0.0/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-04 17:54:09.000000 qfpy-5.0.0/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-4.0.3/src/qfpy/exif.py` & `qfpy-5.0.0/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-4.0.3/src/qfpy/ffmpeg.py` & `qfpy-5.0.0/src/qfpy/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `qfpy-4.0.3/src/qfpy/func.py` & `qfpy-5.0.0/src/qfpy/func.py`

 * *Files identical despite different names*

### Comparing `qfpy-4.0.3/src/qfpy/process.py` & `qfpy-5.0.0/src/qfpy/process.py`

 * *Files identical despite different names*

