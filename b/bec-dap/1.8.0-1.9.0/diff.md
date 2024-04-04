# Comparing `tmp/bec_dap-1.8.0.tar.gz` & `tmp/bec_dap-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_dap-1.8.0.tar", last modified: Tue Feb 20 20:19:28 2024, max compression
+gzip compressed data, was "bec_dap-1.9.0.tar", last modified: Thu Feb 22 19:50:22 2024, max compression
```

## Comparing `bec_dap-1.8.0.tar` & `bec_dap-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.697555 bec_dap-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      460 2024-02-20 20:19:28.697555 bec_dap-1.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.697555 bec_dap-1.8.0/bec_dap.egg-info/
--rw-r--r--   0 root         (0) root         (0)      460 2024-02-20 20:19:28.000000 bec_dap-1.8.0/bec_dap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      445 2024-02-20 20:19:28.000000 bec_dap-1.8.0/bec_dap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 20:19:28.000000 bec_dap-1.8.0/bec_dap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-02-20 20:19:28.000000 bec_dap-1.8.0/bec_dap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-02-20 20:19:28.000000 bec_dap-1.8.0/bec_dap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-02-20 20:19:28.000000 bec_dap-1.8.0/bec_dap.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.695555 bec_dap-1.8.0/data_processing/
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-02-20 11:03:23.000000 bec_dap-1.8.0/data_processing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.695555 bec_dap-1.8.0/data_processing/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-20 20:19:15.000000 bec_dap-1.8.0/data_processing/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1046 2024-02-20 17:20:48.000000 bec_dap-1.8.0/data_processing/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)     1347 2024-02-20 17:20:48.000000 bec_dap-1.8.0/data_processing/dap_server.py
--rw-rw-rw-   0 root         (0) root         (0)     4890 2024-02-20 17:20:48.000000 bec_dap-1.8.0/data_processing/dap_service.py
--rw-rw-rw-   0 root         (0) root         (0)     9890 2024-02-20 17:20:48.000000 bec_dap-1.8.0/data_processing/dap_service_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    12162 2024-02-20 17:20:48.000000 bec_dap-1.8.0/data_processing/lmfit1d_service.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-02-20 20:19:28.698556 bec_dap-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1752 2024-02-20 20:19:24.000000 bec_dap-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.418050 bec_dap-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      460 2024-02-22 19:50:22.418050 bec_dap-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.418050 bec_dap-1.9.0/bec_dap.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      460 2024-02-22 19:50:22.000000 bec_dap-1.9.0/bec_dap.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      445 2024-02-22 19:50:22.000000 bec_dap-1.9.0/bec_dap.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:22.000000 bec_dap-1.9.0/bec_dap.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-02-22 19:50:22.000000 bec_dap-1.9.0/bec_dap.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-02-22 19:50:22.000000 bec_dap-1.9.0/bec_dap.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-02-22 19:50:22.000000 bec_dap-1.9.0/bec_dap.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.417050 bec_dap-1.9.0/data_processing/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-02-22 18:57:01.000000 bec_dap-1.9.0/data_processing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.417050 bec_dap-1.9.0/data_processing/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_dap-1.9.0/data_processing/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2024-02-22 18:57:01.000000 bec_dap-1.9.0/data_processing/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-02-22 18:57:01.000000 bec_dap-1.9.0/data_processing/dap_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     4890 2024-02-22 18:57:01.000000 bec_dap-1.9.0/data_processing/dap_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     9890 2024-02-22 19:40:05.000000 bec_dap-1.9.0/data_processing/dap_service_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    12162 2024-02-22 19:40:05.000000 bec_dap-1.9.0/data_processing/lmfit1d_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-02-22 19:50:22.430051 bec_dap-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2024-02-22 19:50:16.000000 bec_dap-1.9.0/setup.py
```

### Comparing `bec_dap-1.8.0/data_processing/cli/launch.py` & `bec_dap-1.9.0/data_processing/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_dap-1.8.0/data_processing/dap_server.py` & `bec_dap-1.9.0/data_processing/dap_server.py`

 * *Files identical despite different names*

### Comparing `bec_dap-1.8.0/data_processing/dap_service.py` & `bec_dap-1.9.0/data_processing/dap_service.py`

 * *Files identical despite different names*

### Comparing `bec_dap-1.8.0/data_processing/dap_service_manager.py` & `bec_dap-1.9.0/data_processing/dap_service_manager.py`

 * *Files identical despite different names*

### Comparing `bec_dap-1.8.0/data_processing/lmfit1d_service.py` & `bec_dap-1.9.0/data_processing/lmfit1d_service.py`

 * *Files identical despite different names*

### Comparing `bec_dap-1.8.0/setup.cfg` & `bec_dap-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_dap-1.8.0/setup.py` & `bec_dap-1.9.0/setup.py`

 * *Files 1% similar despite different names*

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

