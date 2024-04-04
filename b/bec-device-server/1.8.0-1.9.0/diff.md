# Comparing `tmp/bec_device_server-1.8.0.tar.gz` & `tmp/bec_device_server-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_device_server-1.8.0.tar", last modified: Tue Feb 20 20:19:27 2024, max compression
+gzip compressed data, was "bec_device_server-1.9.0.tar", last modified: Thu Feb 22 19:50:21 2024, max compression
```

## Comparing `bec_device_server-1.8.0.tar` & `bec_device_server-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.814470 bec_device_server-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      515 2024-02-20 20:19:27.814470 bec_device_server-1.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.814470 bec_device_server-1.8.0/bec_device_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      515 2024-02-20 20:19:27.000000 bec_device_server-1.8.0/bec_device_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      589 2024-02-20 20:19:27.000000 bec_device_server-1.8.0/bec_device_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 20:19:27.000000 bec_device_server-1.8.0/bec_device_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-02-20 20:19:27.000000 bec_device_server-1.8.0/bec_device_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      105 2024-02-20 20:19:27.000000 bec_device_server-1.8.0/bec_device_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-02-20 20:19:27.000000 bec_device_server-1.8.0/bec_device_server.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.813470 bec_device_server-1.8.0/device_server/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-02-20 11:03:23.000000 bec_device_server-1.8.0/device_server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.813470 bec_device_server-1.8.0/device_server/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-20 20:19:15.000000 bec_device_server-1.8.0/device_server/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1169 2024-02-20 11:03:23.000000 bec_device_server-1.8.0/device_server/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)    19157 2024-02-20 17:20:48.000000 bec_device_server-1.8.0/device_server/device_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:27.813470 bec_device_server-1.8.0/device_server/devices/
--rw-rw-rw-   0 root         (0) root         (0)      154 2024-02-20 11:03:23.000000 bec_device_server-1.8.0/device_server/devices/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4216 2024-02-20 17:20:48.000000 bec_device_server-1.8.0/device_server/devices/config_update_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3422 2024-02-20 11:03:23.000000 bec_device_server-1.8.0/device_server/devices/device_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)    17889 2024-02-20 17:20:48.000000 bec_device_server-1.8.0/device_server/devices/devicemanager.py
--rw-rw-rw-   0 root         (0) root         (0)     7694 2024-02-20 17:20:48.000000 bec_device_server-1.8.0/device_server/rpc_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-02-20 20:19:27.829471 bec_device_server-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1908 2024-02-20 20:19:24.000000 bec_device_server-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.464958 bec_device_server-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      515 2024-02-22 19:50:21.465958 bec_device_server-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.464958 bec_device_server-1.9.0/bec_device_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      515 2024-02-22 19:50:21.000000 bec_device_server-1.9.0/bec_device_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      589 2024-02-22 19:50:21.000000 bec_device_server-1.9.0/bec_device_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:21.000000 bec_device_server-1.9.0/bec_device_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2024-02-22 19:50:21.000000 bec_device_server-1.9.0/bec_device_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2024-02-22 19:50:21.000000 bec_device_server-1.9.0/bec_device_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-02-22 19:50:21.000000 bec_device_server-1.9.0/bec_device_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.463958 bec_device_server-1.9.0/device_server/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-02-22 18:57:01.000000 bec_device_server-1.9.0/device_server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.463958 bec_device_server-1.9.0/device_server/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_device_server-1.9.0/device_server/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1169 2024-02-22 18:57:01.000000 bec_device_server-1.9.0/device_server/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)    19157 2024-02-22 19:40:05.000000 bec_device_server-1.9.0/device_server/device_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:21.464958 bec_device_server-1.9.0/device_server/devices/
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-02-22 18:57:01.000000 bec_device_server-1.9.0/device_server/devices/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4216 2024-02-22 18:57:01.000000 bec_device_server-1.9.0/device_server/devices/config_update_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2024-02-22 19:40:05.000000 bec_device_server-1.9.0/device_server/devices/device_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)    17889 2024-02-22 19:40:05.000000 bec_device_server-1.9.0/device_server/devices/devicemanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7694 2024-02-22 19:40:05.000000 bec_device_server-1.9.0/device_server/rpc_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-02-22 19:50:21.466958 bec_device_server-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2024-02-22 19:50:16.000000 bec_device_server-1.9.0/setup.py
```

### Comparing `bec_device_server-1.8.0/PKG-INFO` & `bec_device_server-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec_device_server
-Version: 1.8.0
+Version: 1.9.0
 Summary: BEC service for connecting, controlling and monitoring devices through ophyd
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_device_server-1.8.0/bec_device_server.egg-info/PKG-INFO` & `bec_device_server-1.9.0/bec_device_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bec-device-server
-Version: 1.8.0
+Version: 1.9.0
 Summary: BEC service for connecting, controlling and monitoring devices through ophyd
 Home-page: https://gitlab.psi.ch/bec/bec
 License: UNKNOWN
 Project-URL: Bug Tracker, https://gitlab.psi.ch/bec/bec/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bec_device_server-1.8.0/bec_device_server.egg-info/SOURCES.txt` & `bec_device_server-1.9.0/bec_device_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_device_server-1.8.0/device_server/cli/launch.py` & `bec_device_server-1.9.0/device_server/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-1.8.0/device_server/device_server.py` & `bec_device_server-1.9.0/device_server/device_server.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-1.8.0/device_server/devices/config_update_handler.py` & `bec_device_server-1.9.0/device_server/devices/config_update_handler.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-1.8.0/device_server/devices/device_serializer.py` & `bec_device_server-1.9.0/device_server/devices/device_serializer.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-1.8.0/device_server/devices/devicemanager.py` & `bec_device_server-1.9.0/device_server/devices/devicemanager.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-1.8.0/device_server/rpc_mixin.py` & `bec_device_server-1.9.0/device_server/rpc_mixin.py`

 * *Files identical despite different names*

### Comparing `bec_device_server-1.8.0/setup.cfg` & `bec_device_server-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_device_server-1.8.0/setup.py` & `bec_device_server-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
 bec_lib = f"{current_path}/../bec_lib/"
 
 ophyd_devices = os.getenv("OPHYD_DEVICES_PATH", f"{current_path}/../../ophyd_devices/")
 
-__version__ = "1.8.0"
+__version__ = "1.9.0"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```

