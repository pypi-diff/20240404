# Comparing `tmp/bec_scan_server-1.8.0.tar.gz` & `tmp/bec_scan_server-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scan_server-1.8.0.tar", last modified: Tue Feb 20 20:19:27 2024, max compression
+gzip compressed data, was "bec_scan_server-1.9.0.tar", last modified: Thu Feb 22 19:50:21 2024, max compression
```

## Comparing `bec_scan_server-1.8.0.tar` & `bec_scan_server-1.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.514441 bec_scan_server-1.8.0/
--rw-r--r--   0 root         (0) root         (0)     2560 2024-02-20 20:19:27.514441 bec_scan_server-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-02-20 11:03:23.000000 bec_scan_server-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.514441 bec_scan_server-1.8.0/bec_scan_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2560 2024-02-20 20:19:27.000000 bec_scan_server-1.8.0/bec_scan_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      815 2024-02-20 20:19:27.000000 bec_scan_server-1.8.0/bec_scan_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 20:19:27.000000 bec_scan_server-1.8.0/bec_scan_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-02-20 20:19:27.000000 bec_scan_server-1.8.0/bec_scan_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       98 2024-02-20 20:19:27.000000 bec_scan_server-1.8.0/bec_scan_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-20 20:19:27.000000 bec_scan_server-1.8.0/bec_scan_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.512441 bec_scan_server-1.8.0/scan_plugins/
--rw-rw-rw-   0 root         (0) root         (0)    21430 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_plugins/LamNIFermatScan.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-02-20 11:03:23.000000 bec_scan_server-1.8.0/scan_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6325 2024-02-20 11:03:23.000000 bec_scan_server-1.8.0/scan_plugins/otf_scan.py
--rw-rw-rw-   0 root         (0) root         (0)    13214 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_plugins/owis_grid.py
--rw-rw-rw-   0 root         (0) root         (0)     9165 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_plugins/sgalil_grid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.513441 bec_scan_server-1.8.0/scan_server/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-02-20 11:03:23.000000 bec_scan_server-1.8.0/scan_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.514441 bec_scan_server-1.8.0/scan_server/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-20 20:19:15.000000 bec_scan_server-1.8.0/scan_server/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-02-20 11:03:23.000000 bec_scan_server-1.8.0/scan_server/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     6553 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_server/device_validation.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-20 11:03:23.000000 bec_scan_server-1.8.0/scan_server/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2024-02-20 11:03:23.000000 bec_scan_server-1.8.0/scan_server/path_optimization.py
--rw-rw-rw-   0 root         (0) root         (0)     2075 2024-02-20 11:03:23.000000 bec_scan_server-1.8.0/scan_server/scan_assembler.py
--rw-rw-rw-   0 root         (0) root         (0)     6743 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_server/scan_guard.py
--rw-rw-rw-   0 root         (0) root         (0)     4075 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_server/scan_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    32191 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_server/scan_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     3317 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_server/scan_server.py
--rw-rw-rw-   0 root         (0) root         (0)    13251 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_server/scan_stubs.py
--rw-rw-rw-   0 root         (0) root         (0)    34124 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_server/scan_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    50510 2024-02-20 17:20:48.000000 bec_scan_server-1.8.0/scan_server/scans.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-02-20 20:19:27.515441 bec_scan_server-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1782 2024-02-20 20:19:24.000000 bec_scan_server-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.112923 bec_scan_server-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)     2560 2024-02-22 19:50:21.112923 bec_scan_server-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.112923 bec_scan_server-1.9.0/bec_scan_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2560 2024-02-22 19:50:21.000000 bec_scan_server-1.9.0/bec_scan_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      815 2024-02-22 19:50:21.000000 bec_scan_server-1.9.0/bec_scan_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:21.000000 bec_scan_server-1.9.0/bec_scan_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2024-02-22 19:50:21.000000 bec_scan_server-1.9.0/bec_scan_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2024-02-22 19:50:21.000000 bec_scan_server-1.9.0/bec_scan_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-02-22 19:50:21.000000 bec_scan_server-1.9.0/bec_scan_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.110923 bec_scan_server-1.9.0/scan_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)    21430 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_plugins/LamNIFermatScan.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6325 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_plugins/otf_scan.py
+-rw-rw-rw-   0 root         (0) root         (0)    13214 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_plugins/owis_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     9165 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_plugins/sgalil_grid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.111923 bec_scan_server-1.9.0/scan_server/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.111923 bec_scan_server-1.9.0/scan_server/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_scan_server-1.9.0/scan_server/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6553 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/device_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/path_optimization.py
+-rw-rw-rw-   0 root         (0) root         (0)     2075 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/scan_assembler.py
+-rw-rw-rw-   0 root         (0) root         (0)     6743 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/scan_guard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4075 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/scan_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    32191 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/scan_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3317 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/scan_server.py
+-rw-rw-rw-   0 root         (0) root         (0)    13251 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/scan_stubs.py
+-rw-rw-rw-   0 root         (0) root         (0)    34124 2024-02-22 19:40:05.000000 bec_scan_server-1.9.0/scan_server/scan_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    50510 2024-02-22 18:57:01.000000 bec_scan_server-1.9.0/scan_server/scans.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-02-22 19:50:21.113924 bec_scan_server-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2024-02-22 19:50:16.000000 bec_scan_server-1.9.0/setup.py
```

### Comparing `bec_scan_server-1.8.0/PKG-INFO` & `bec_scan_server-1.9.0/bec_scan_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bec_scan_server
-Version: 1.8.0
+Name: bec-scan-server
+Version: 1.9.0
 Summary: BEC scan server
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_scan_server-1.8.0/README.md` & `bec_scan_server-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/bec_scan_server.egg-info/PKG-INFO` & `bec_scan_server-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bec-scan-server
-Version: 1.8.0
+Name: bec_scan_server
+Version: 1.9.0
 Summary: BEC scan server
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_scan_server-1.8.0/bec_scan_server.egg-info/SOURCES.txt` & `bec_scan_server-1.9.0/bec_scan_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_plugins/LamNIFermatScan.py` & `bec_scan_server-1.9.0/scan_plugins/LamNIFermatScan.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_plugins/otf_scan.py` & `bec_scan_server-1.9.0/scan_plugins/otf_scan.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_plugins/owis_grid.py` & `bec_scan_server-1.9.0/scan_plugins/owis_grid.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_plugins/sgalil_grid.py` & `bec_scan_server-1.9.0/scan_plugins/sgalil_grid.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/cli/launch.py` & `bec_scan_server-1.9.0/scan_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/device_validation.py` & `bec_scan_server-1.9.0/scan_server/device_validation.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/path_optimization.py` & `bec_scan_server-1.9.0/scan_server/path_optimization.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/scan_assembler.py` & `bec_scan_server-1.9.0/scan_server/scan_assembler.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/scan_guard.py` & `bec_scan_server-1.9.0/scan_server/scan_guard.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/scan_manager.py` & `bec_scan_server-1.9.0/scan_server/scan_manager.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/scan_queue.py` & `bec_scan_server-1.9.0/scan_server/scan_queue.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/scan_server.py` & `bec_scan_server-1.9.0/scan_server/scan_server.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/scan_stubs.py` & `bec_scan_server-1.9.0/scan_server/scan_stubs.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/scan_worker.py` & `bec_scan_server-1.9.0/scan_server/scan_worker.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/scan_server/scans.py` & `bec_scan_server-1.9.0/scan_server/scans.py`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/setup.cfg` & `bec_scan_server-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scan_server-1.8.0/setup.py` & `bec_scan_server-1.9.0/setup.py`

 * *Files 0% similar despite different names*

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

