# Comparing `tmp/bec_scan_bundler-1.8.0.tar.gz` & `tmp/bec_scan_bundler-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scan_bundler-1.8.0.tar", last modified: Tue Feb 20 20:19:28 2024, max compression
+gzip compressed data, was "bec_scan_bundler-1.9.0.tar", last modified: Thu Feb 22 19:50:21 2024, max compression
```

## Comparing `bec_scan_bundler-1.8.0.tar` & `bec_scan_bundler-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.105498 bec_scan_bundler-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      490 2024-02-20 20:19:28.105498 bec_scan_bundler-1.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.105498 bec_scan_bundler-1.8.0/bec_scan_bundler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      490 2024-02-20 20:19:28.000000 bec_scan_bundler-1.8.0/bec_scan_bundler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-02-20 20:19:28.000000 bec_scan_bundler-1.8.0/bec_scan_bundler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 20:19:28.000000 bec_scan_bundler-1.8.0/bec_scan_bundler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-02-20 20:19:28.000000 bec_scan_bundler-1.8.0/bec_scan_bundler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       85 2024-02-20 20:19:28.000000 bec_scan_bundler-1.8.0/bec_scan_bundler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-02-20 20:19:28.000000 bec_scan_bundler-1.8.0/bec_scan_bundler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.105498 bec_scan_bundler-1.8.0/scan_bundler/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-02-20 11:03:23.000000 bec_scan_bundler-1.8.0/scan_bundler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2024-02-20 17:20:48.000000 bec_scan_bundler-1.8.0/scan_bundler/bec_emitter.py
--rw-rw-rw-   0 root         (0) root         (0)     5002 2024-02-20 17:20:48.000000 bec_scan_bundler-1.8.0/scan_bundler/bluesky_emitter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.105498 bec_scan_bundler-1.8.0/scan_bundler/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-20 20:19:15.000000 bec_scan_bundler-1.8.0/scan_bundler/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2024-02-20 11:03:23.000000 bec_scan_bundler-1.8.0/scan_bundler/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     1848 2024-02-20 17:20:48.000000 bec_scan_bundler-1.8.0/scan_bundler/emitter.py
--rw-rw-rw-   0 root         (0) root         (0)    15800 2024-02-20 17:20:48.000000 bec_scan_bundler-1.8.0/scan_bundler/scan_bundler.py
--rw-rw-rw-   0 root         (0) root         (0)      551 2024-02-20 20:19:28.124500 bec_scan_bundler-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1749 2024-02-20 20:19:24.000000 bec_scan_bundler-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.784989 bec_scan_bundler-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      490 2024-02-22 19:50:21.784989 bec_scan_bundler-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.784989 bec_scan_bundler-1.9.0/bec_scan_bundler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      490 2024-02-22 19:50:21.000000 bec_scan_bundler-1.9.0/bec_scan_bundler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-02-22 19:50:21.000000 bec_scan_bundler-1.9.0/bec_scan_bundler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:21.000000 bec_scan_bundler-1.9.0/bec_scan_bundler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-02-22 19:50:21.000000 bec_scan_bundler-1.9.0/bec_scan_bundler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-02-22 19:50:21.000000 bec_scan_bundler-1.9.0/bec_scan_bundler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-02-22 19:50:21.000000 bec_scan_bundler-1.9.0/bec_scan_bundler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.783989 bec_scan_bundler-1.9.0/scan_bundler/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-02-22 18:57:01.000000 bec_scan_bundler-1.9.0/scan_bundler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-02-22 19:40:05.000000 bec_scan_bundler-1.9.0/scan_bundler/bec_emitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5002 2024-02-22 19:40:05.000000 bec_scan_bundler-1.9.0/scan_bundler/bluesky_emitter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.783989 bec_scan_bundler-1.9.0/scan_bundler/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_scan_bundler-1.9.0/scan_bundler/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-02-22 18:57:01.000000 bec_scan_bundler-1.9.0/scan_bundler/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2024-02-22 18:57:01.000000 bec_scan_bundler-1.9.0/scan_bundler/emitter.py
+-rw-rw-rw-   0 root         (0) root         (0)    15800 2024-02-22 18:57:01.000000 bec_scan_bundler-1.9.0/scan_bundler/scan_bundler.py
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-02-22 19:50:21.786989 bec_scan_bundler-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2024-02-22 19:50:16.000000 bec_scan_bundler-1.9.0/setup.py
```

### Comparing `bec_scan_bundler-1.8.0/scan_bundler/bec_emitter.py` & `bec_scan_bundler-1.9.0/scan_bundler/bec_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-1.8.0/scan_bundler/bluesky_emitter.py` & `bec_scan_bundler-1.9.0/scan_bundler/bluesky_emitter.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-1.8.0/scan_bundler/cli/launch.py` & `bec_scan_bundler-1.9.0/scan_bundler/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-1.8.0/scan_bundler/emitter.py` & `bec_scan_bundler-1.9.0/scan_bundler/emitter.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-1.8.0/scan_bundler/scan_bundler.py` & `bec_scan_bundler-1.9.0/scan_bundler/scan_bundler.py`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-1.8.0/setup.cfg` & `bec_scan_bundler-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scan_bundler-1.8.0/setup.py` & `bec_scan_bundler-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

