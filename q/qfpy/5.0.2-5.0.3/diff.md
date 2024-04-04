# Comparing `tmp/qfpy-5.0.2.tar.gz` & `tmp/qfpy-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-5.0.2.tar", last modified: Thu Apr  4 18:45:56 2024, max compression
+gzip compressed data, was "qfpy-5.0.3.tar", last modified: Thu Apr  4 19:00:29 2024, max compression
```

## Comparing `qfpy-5.0.2.tar` & `qfpy-5.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 18:45:56.566470 qfpy-5.0.2/
--rw-rw-rw-   0        0        0      159 2024-04-04 18:45:56.564528 qfpy-5.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-04 18:45:40.000000 qfpy-5.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 18:45:56.566470 qfpy-5.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 18:45:56.544986 qfpy-5.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 18:45:56.555739 qfpy-5.0.2/src/qfpy/
--rw-rw-rw-   0        0        0       29 2024-03-06 16:44:46.000000 qfpy-5.0.2/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0     1393 2024-03-27 09:56:39.000000 qfpy-5.0.2/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     3083 2024-03-23 10:22:51.000000 qfpy-5.0.2/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      495 2024-04-04 18:45:31.000000 qfpy-5.0.2/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      845 2024-03-23 10:23:45.000000 qfpy-5.0.2/src/qfpy/func.py
--rw-rw-rw-   0        0        0      804 2024-03-23 10:20:43.000000 qfpy-5.0.2/src/qfpy/process.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:45:56.562567 qfpy-5.0.2/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      159 2024-04-04 18:45:56.000000 qfpy-5.0.2/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-04 18:45:56.000000 qfpy-5.0.2/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 18:45:56.000000 qfpy-5.0.2/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-04 18:45:56.000000 qfpy-5.0.2/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 19:00:29.479059 qfpy-5.0.3/
+-rw-rw-rw-   0        0        0      159 2024-04-04 19:00:29.478055 qfpy-5.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-04 19:00:22.000000 qfpy-5.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:00:29.479059 qfpy-5.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 19:00:29.460054 qfpy-5.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 19:00:29.470057 qfpy-5.0.3/src/qfpy/
+-rw-rw-rw-   0        0        0       29 2024-03-06 16:44:46.000000 qfpy-5.0.3/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0     1393 2024-03-27 09:56:39.000000 qfpy-5.0.3/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     3083 2024-03-23 10:22:51.000000 qfpy-5.0.3/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      611 2024-04-04 18:59:51.000000 qfpy-5.0.3/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      845 2024-03-23 10:23:45.000000 qfpy-5.0.3/src/qfpy/func.py
+-rw-rw-rw-   0        0        0      804 2024-03-23 10:20:43.000000 qfpy-5.0.3/src/qfpy/process.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:00:29.477060 qfpy-5.0.3/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-04-04 19:00:29.000000 qfpy-5.0.3/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-04 19:00:29.000000 qfpy-5.0.3/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:00:29.000000 qfpy-5.0.3/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-04 19:00:29.000000 qfpy-5.0.3/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-5.0.2/src/qfpy/exif.py` & `qfpy-5.0.3/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-5.0.2/src/qfpy/ffmpeg.py` & `qfpy-5.0.3/src/qfpy/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `qfpy-5.0.2/src/qfpy/func.py` & `qfpy-5.0.3/src/qfpy/func.py`

 * *Files identical despite different names*

### Comparing `qfpy-5.0.2/src/qfpy/process.py` & `qfpy-5.0.3/src/qfpy/process.py`

 * *Files identical despite different names*

