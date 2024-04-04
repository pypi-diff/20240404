# Comparing `tmp/bec_file_writer-1.8.0.tar.gz` & `tmp/bec_file_writer-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_file_writer-1.8.0.tar", last modified: Tue Feb 20 20:19:28 2024, max compression
+gzip compressed data, was "bec_file_writer-1.9.0.tar", last modified: Thu Feb 22 19:50:22 2024, max compression
```

## Comparing `bec_file_writer-1.8.0.tar` & `bec_file_writer-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.399526 bec_file_writer-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      475 2024-02-20 20:19:28.399526 bec_file_writer-1.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.399526 bec_file_writer-1.8.0/bec_file_writer.egg-info/
--rw-r--r--   0 root         (0) root         (0)      475 2024-02-20 20:19:28.000000 bec_file_writer-1.8.0/bec_file_writer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      539 2024-02-20 20:19:28.000000 bec_file_writer-1.8.0/bec_file_writer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 20:19:28.000000 bec_file_writer-1.8.0/bec_file_writer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-02-20 20:19:28.000000 bec_file_writer-1.8.0/bec_file_writer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-02-20 20:19:28.000000 bec_file_writer-1.8.0/bec_file_writer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-20 20:19:28.000000 bec_file_writer-1.8.0/bec_file_writer.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.398527 bec_file_writer-1.8.0/file_writer/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-02-20 11:03:23.000000 bec_file_writer-1.8.0/file_writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.398527 bec_file_writer-1.8.0/file_writer/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-20 20:19:15.000000 bec_file_writer-1.8.0/file_writer/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-20 11:03:23.000000 bec_file_writer-1.8.0/file_writer/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)    11711 2024-02-20 17:20:48.000000 bec_file_writer-1.8.0/file_writer/file_writer.py
--rw-r--r--   0 root         (0) root         (0)    11615 2024-02-20 20:19:16.000000 bec_file_writer-1.8.0/file_writer/file_writer_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2024-02-20 11:03:23.000000 bec_file_writer-1.8.0/file_writer/merged_dicts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.398527 bec_file_writer-1.8.0/file_writer_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-02-20 11:03:23.000000 bec_file_writer-1.8.0/file_writer_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22335 2024-02-20 11:03:23.000000 bec_file_writer-1.8.0/file_writer_plugins/cSAXS.py
--rw-rw-rw-   0 root         (0) root         (0)     3018 2024-02-20 11:03:23.000000 bec_file_writer-1.8.0/file_writer_plugins/default_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-02-20 20:19:28.401527 bec_file_writer-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1773 2024-02-20 20:19:24.000000 bec_file_writer-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.103020 bec_file_writer-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      475 2024-02-22 19:50:22.103020 bec_file_writer-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.103020 bec_file_writer-1.9.0/bec_file_writer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      475 2024-02-22 19:50:22.000000 bec_file_writer-1.9.0/bec_file_writer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      539 2024-02-22 19:50:22.000000 bec_file_writer-1.9.0/bec_file_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:22.000000 bec_file_writer-1.9.0/bec_file_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-02-22 19:50:22.000000 bec_file_writer-1.9.0/bec_file_writer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-02-22 19:50:22.000000 bec_file_writer-1.9.0/bec_file_writer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-02-22 19:50:22.000000 bec_file_writer-1.9.0/bec_file_writer.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.102019 bec_file_writer-1.9.0/file_writer/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-02-22 18:57:01.000000 bec_file_writer-1.9.0/file_writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.102019 bec_file_writer-1.9.0/file_writer/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_file_writer-1.9.0/file_writer/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-02-22 18:57:01.000000 bec_file_writer-1.9.0/file_writer/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)    11711 2024-02-22 18:57:01.000000 bec_file_writer-1.9.0/file_writer/file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)    11615 2024-02-22 19:40:05.000000 bec_file_writer-1.9.0/file_writer/file_writer_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2024-02-22 18:57:01.000000 bec_file_writer-1.9.0/file_writer/merged_dicts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.102019 bec_file_writer-1.9.0/file_writer_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-02-22 18:57:01.000000 bec_file_writer-1.9.0/file_writer_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22335 2024-02-22 18:57:01.000000 bec_file_writer-1.9.0/file_writer_plugins/cSAXS.py
+-rw-rw-rw-   0 root         (0) root         (0)     3018 2024-02-22 18:57:01.000000 bec_file_writer-1.9.0/file_writer_plugins/default_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-02-22 19:50:22.105020 bec_file_writer-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2024-02-22 19:50:16.000000 bec_file_writer-1.9.0/setup.py
```

### Comparing `bec_file_writer-1.8.0/bec_file_writer.egg-info/SOURCES.txt` & `bec_file_writer-1.9.0/bec_file_writer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_file_writer-1.8.0/file_writer/cli/launch.py` & `bec_file_writer-1.9.0/file_writer/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-1.8.0/file_writer/file_writer.py` & `bec_file_writer-1.9.0/file_writer/file_writer.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-1.8.0/file_writer/file_writer_manager.py` & `bec_file_writer-1.9.0/file_writer/file_writer_manager.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-1.8.0/file_writer/merged_dicts.py` & `bec_file_writer-1.9.0/file_writer/merged_dicts.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-1.8.0/file_writer_plugins/cSAXS.py` & `bec_file_writer-1.9.0/file_writer_plugins/cSAXS.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-1.8.0/file_writer_plugins/default_writer.py` & `bec_file_writer-1.9.0/file_writer_plugins/default_writer.py`

 * *Files identical despite different names*

### Comparing `bec_file_writer-1.8.0/setup.cfg` & `bec_file_writer-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_file_writer-1.8.0/setup.py` & `bec_file_writer-1.9.0/setup.py`

 * *Files 4% similar despite different names*

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

