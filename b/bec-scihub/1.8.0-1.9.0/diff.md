# Comparing `tmp/bec_scihub-1.8.0.tar.gz` & `tmp/bec_scihub-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_scihub-1.8.0.tar", last modified: Tue Feb 20 20:19:28 2024, max compression
+gzip compressed data, was "bec_scihub-1.9.0.tar", last modified: Thu Feb 22 19:50:22 2024, max compression
```

## Comparing `bec_scihub-1.8.0.tar` & `bec_scihub-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.970582 bec_scihub-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      477 2024-02-20 20:19:28.970582 bec_scihub-1.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.970582 bec_scihub-1.8.0/bec_scihub.egg-info/
--rw-r--r--   0 root         (0) root         (0)      477 2024-02-20 20:19:28.000000 bec_scihub-1.8.0/bec_scihub.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      534 2024-02-20 20:19:28.000000 bec_scihub-1.8.0/bec_scihub.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 20:19:28.000000 bec_scihub-1.8.0/bec_scihub.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-20 20:19:28.000000 bec_scihub-1.8.0/bec_scihub.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-02-20 20:19:28.000000 bec_scihub-1.8.0/bec_scihub.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-20 20:19:28.000000 bec_scihub-1.8.0/bec_scihub.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.969582 bec_scihub-1.8.0/scihub/
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-02-20 11:03:23.000000 bec_scihub-1.8.0/scihub/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.969582 bec_scihub-1.8.0/scihub/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-20 20:19:15.000000 bec_scihub-1.8.0/scihub/cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-02-20 11:03:23.000000 bec_scihub-1.8.0/scihub/cli/launch.py
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-02-20 11:03:23.000000 bec_scihub-1.8.0/scihub/repeated_timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.969582 bec_scihub-1.8.0/scihub/scibec/
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-20 11:03:23.000000 bec_scihub-1.8.0/scihub/scibec/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7644 2024-02-20 17:20:48.000000 bec_scihub-1.8.0/scihub/scibec/config_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7705 2024-02-20 17:20:48.000000 bec_scihub-1.8.0/scihub/scibec/scibec_connector.py
--rw-rw-rw-   0 root         (0) root         (0)     6480 2024-02-20 17:20:48.000000 bec_scihub-1.8.0/scihub/scibec/scibec_metadata_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-02-20 17:20:48.000000 bec_scihub-1.8.0/scihub/scihub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 20:19:28.969582 bec_scihub-1.8.0/scihub/scilog/
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-02-20 11:03:23.000000 bec_scihub-1.8.0/scihub/scilog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2024-02-20 17:20:48.000000 bec_scihub-1.8.0/scihub/scilog/scilog.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-02-20 20:19:28.971582 bec_scihub-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-02-20 20:19:24.000000 bec_scihub-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.730080 bec_scihub-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      477 2024-02-22 19:50:22.730080 bec_scihub-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.730080 bec_scihub-1.9.0/bec_scihub.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      477 2024-02-22 19:50:22.000000 bec_scihub-1.9.0/bec_scihub.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      534 2024-02-22 19:50:22.000000 bec_scihub-1.9.0/bec_scihub.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 19:50:22.000000 bec_scihub-1.9.0/bec_scihub.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-02-22 19:50:22.000000 bec_scihub-1.9.0/bec_scihub.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-02-22 19:50:22.000000 bec_scihub-1.9.0/bec_scihub.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-02-22 19:50:22.000000 bec_scihub-1.9.0/bec_scihub.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.729080 bec_scihub-1.9.0/scihub/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-02-22 18:57:01.000000 bec_scihub-1.9.0/scihub/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.729080 bec_scihub-1.9.0/scihub/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-22 19:50:05.000000 bec_scihub-1.9.0/scihub/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-02-22 18:57:01.000000 bec_scihub-1.9.0/scihub/cli/launch.py
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-02-22 18:57:01.000000 bec_scihub-1.9.0/scihub/repeated_timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.729080 bec_scihub-1.9.0/scihub/scibec/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-02-22 18:57:01.000000 bec_scihub-1.9.0/scihub/scibec/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2024-02-22 18:57:01.000000 bec_scihub-1.9.0/scihub/scibec/config_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7663 2024-02-22 19:40:05.000000 bec_scihub-1.9.0/scihub/scibec/scibec_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)     6702 2024-02-22 19:40:05.000000 bec_scihub-1.9.0/scihub/scibec/scibec_metadata_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-02-22 18:57:01.000000 bec_scihub-1.9.0/scihub/scihub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 19:50:22.729080 bec_scihub-1.9.0/scihub/scilog/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-02-22 18:57:01.000000 bec_scihub-1.9.0/scihub/scilog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2024-02-22 18:57:01.000000 bec_scihub-1.9.0/scihub/scilog/scilog.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-02-22 19:50:22.731081 bec_scihub-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-02-22 19:50:16.000000 bec_scihub-1.9.0/setup.py
```

### Comparing `bec_scihub-1.8.0/bec_scihub.egg-info/SOURCES.txt` & `bec_scihub-1.9.0/bec_scihub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bec_scihub-1.8.0/scihub/cli/launch.py` & `bec_scihub-1.9.0/scihub/cli/launch.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-1.8.0/scihub/repeated_timer.py` & `bec_scihub-1.9.0/scihub/repeated_timer.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-1.8.0/scihub/scibec/config_handler.py` & `bec_scihub-1.9.0/scihub/scibec/config_handler.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-1.8.0/scihub/scibec/scibec_connector.py` & `bec_scihub-1.9.0/scihub/scibec/scibec_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
             logger.warning("No environment file found. Cannot connect to SciBec.")
             return
         try:
             self._update_scibec_instance()
             self._update_experiment_info()
             self._update_eaccount_in_redis()
 
-        except (ApiException, SciBecConnectorError, MaxRetryError) as exc:
+        except Exception as exc:
             self.scibec = None
             logger.warning(f"Could not connect to SciBec: {exc}")
 
     def _update_scibec_instance(self):
         logger.info(f"Connecting to SciBec on {self.host}")
         self.scibec = SciBecCore(host=self.host)
         self.scibec.login(username=self.ingestor, password=self.ingestor_secret)
```

### Comparing `bec_scihub-1.8.0/scihub/scibec/scibec_metadata_handler.py` & `bec_scihub-1.9.0/scihub/scibec/scibec_metadata_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
+import time
 from typing import TYPE_CHECKING
 
 from bec_lib import MessageEndpoints, bec_logger, messages
+from bec_lib.serialization import json_ext
 
 logger = bec_logger.logger
 
 if TYPE_CHECKING:
     from scihub.scibec import SciBecConnector
 
 
@@ -143,27 +145,31 @@
         if not scan:
             logger.warning(
                 f"Could not find scan with scanID {data['metadata']['scanID']}. Cannot write scan"
                 " data to SciBec."
             )
             return
         scan = scan[0]
+        data_bec = {key: json_ext.dumps(value) for key, value in data.items()}
+        start = time.time()
         scibec.scan_data.scan_data_controller_create_many(
             body=scibec.models.ScanData(
                 **{
                     "readACL": scan["readACL"],
                     "writeACL": scan["readACL"],
                     "owner": scan["owner"],
                     "scanId": scan["id"],
                     "filePath": file_path,
-                    "data": data,
+                    "data": data_bec,
                 }
             )
         )
-        logger.info(f"Wrote scan data to SciBec for scanID {data['metadata']['scanID']}")
+        logger.info(
+            f"Wrote scan data to SciBec for scanID {data['metadata']['scanID']} in {time.time() - start} seconds."
+        )
 
     def shutdown(self):
         """
         Shutdown the metadata handler
         """
         if self._scan_status_consumer:
             self._scan_status_consumer.shutdown()
```

### Comparing `bec_scihub-1.8.0/scihub/scihub.py` & `bec_scihub-1.9.0/scihub/scihub.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-1.8.0/scihub/scilog/scilog.py` & `bec_scihub-1.9.0/scihub/scilog/scilog.py`

 * *Files identical despite different names*

### Comparing `bec_scihub-1.8.0/setup.cfg` & `bec_scihub-1.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bec_scihub-1.8.0/setup.py` & `bec_scihub-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
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

