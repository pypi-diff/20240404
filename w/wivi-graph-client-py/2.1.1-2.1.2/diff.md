# Comparing `tmp/wivi_graph_client_py-2.1.1.tar.gz` & `tmp/wivi_graph_client_py-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wivi_graph_client_py-2.1.1.tar", last modified: Thu Apr  4 09:53:19 2024, max compression
+gzip compressed data, was "wivi_graph_client_py-2.1.2.tar", last modified: Thu Apr  4 11:32:26 2024, max compression
```

## Comparing `wivi_graph_client_py-2.1.1.tar` & `wivi_graph_client_py-2.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/
--rw-r--r--   0 root         (0) root         (0)      363 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      449 2024-04-04 09:53:06.000000 wivi_graph_client_py-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/wivi_graph_client_py/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8590 2023-11-23 13:49:45.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/client.py
--rw-rw-r--   0 root         (0) root         (0)     1239 2024-02-12 19:32:52.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     1283 2024-02-12 19:33:53.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_connection.py
--rw-rw-r--   0 root         (0) root         (0)      886 2023-11-23 09:54:12.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_info.py
--rw-rw-r--   0 root         (0) root         (0)     1060 2024-02-12 21:21:44.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_status.py
--rw-rw-r--   0 root         (0) root         (0)      838 2024-02-12 21:21:41.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_version.py
--rw-rw-r--   0 root         (0) root         (0)     1323 2024-02-12 21:24:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/dtc.py
--rw-rw-r--   0 root         (0) root         (0)      217 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/ecu.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2024-02-12 21:24:43.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/fail_processing.py
--rw-rw-r--   0 root         (0) root         (0)     1226 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/formula.py
--rw-rw-r--   0 root         (0) root         (0)      864 2024-02-12 21:25:59.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/gps.py
--rw-rw-r--   0 root         (0) root         (0)      549 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/main.py
--rw-rw-r--   0 root         (0) root         (0)      647 2024-02-12 21:26:32.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/message.py
--rw-rw-r--   0 root         (0) root         (0)      213 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/network.py
--rw-rw-r--   0 root         (0) root         (0)     1000 2024-04-04 09:46:03.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/network_stats.py
--rw-rw-r--   0 root         (0) root         (0)     1345 2024-02-12 21:31:53.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/signal.py
--rw-rw-r--   0 root         (0) root         (0)     2701 2024-02-18 20:16:53.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_configuration.py
--rw-rw-r--   0 root         (0) root         (0)     2659 2024-02-19 09:44:20.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_device_connection.py
--rw-rw-r--   0 root         (0) root         (0)     1437 2024-02-19 08:55:57.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_device_version.py
--rw-rw-r--   0 root         (0) root         (0)     3459 2024-02-18 16:27:42.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_dtc.py
--rw-rw-r--   0 root         (0) root         (0)     2575 2024-02-18 22:28:53.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_fail_processing.py
--rw-rw-r--   0 root         (0) root         (0)     2066 2024-02-18 16:26:36.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_gps.py
--rw-rw-r--   0 root         (0) root         (0)     1972 2024-02-18 20:50:16.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_message.py
--rw-rw-r--   0 root         (0) root         (0)     2441 2024-04-04 09:45:48.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_network_stats.py
--rw-rw-r--   0 root         (0) root         (0)     8811 2024-02-18 16:52:58.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_signal.py
--rw-rw-r--   0 root         (0) root         (0)      771 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)      363 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1195 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:32:26.618934 wivi_graph_client_py-2.1.2/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-04-04 11:32:26.618934 wivi_graph_client_py-2.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 11:32:26.618934 wivi_graph_client_py-2.1.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      449 2024-04-04 11:31:44.000000 wivi_graph_client_py-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:32:26.618934 wivi_graph_client_py-2.1.2/wivi_graph_client_py/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8590 2023-11-23 13:49:45.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/client.py
+-rw-rw-r--   0 root         (0) root         (0)     1249 2024-04-04 11:30:05.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     1283 2024-02-12 19:33:53.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/device_connection.py
+-rw-rw-r--   0 root         (0) root         (0)      886 2023-11-23 09:54:12.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/device_info.py
+-rw-rw-r--   0 root         (0) root         (0)     1060 2024-02-12 21:21:44.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/device_status.py
+-rw-rw-r--   0 root         (0) root         (0)      838 2024-02-12 21:21:41.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/device_version.py
+-rw-rw-r--   0 root         (0) root         (0)     1323 2024-02-12 21:24:05.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/dtc.py
+-rw-rw-r--   0 root         (0) root         (0)      217 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/ecu.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2024-02-12 21:24:43.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/fail_processing.py
+-rw-rw-r--   0 root         (0) root         (0)     1226 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/formula.py
+-rw-rw-r--   0 root         (0) root         (0)      864 2024-02-12 21:25:59.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/gps.py
+-rw-rw-r--   0 root         (0) root         (0)      549 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/main.py
+-rw-rw-r--   0 root         (0) root         (0)      647 2024-02-12 21:26:32.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/message.py
+-rw-rw-r--   0 root         (0) root         (0)      213 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/network.py
+-rw-rw-r--   0 root         (0) root         (0)     1000 2024-04-04 09:46:03.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/network_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     1345 2024-02-12 21:31:53.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/signal.py
+-rw-rw-r--   0 root         (0) root         (0)     2701 2024-02-18 20:16:53.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     2659 2024-02-19 09:44:20.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_device_connection.py
+-rw-rw-r--   0 root         (0) root         (0)     1437 2024-02-19 08:55:57.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_device_version.py
+-rw-rw-r--   0 root         (0) root         (0)     3459 2024-02-18 16:27:42.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_dtc.py
+-rw-rw-r--   0 root         (0) root         (0)     2575 2024-02-18 22:28:53.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_fail_processing.py
+-rw-rw-r--   0 root         (0) root         (0)     2066 2024-02-18 16:26:36.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_gps.py
+-rw-rw-r--   0 root         (0) root         (0)     1972 2024-02-18 20:50:16.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_message.py
+-rw-rw-r--   0 root         (0) root         (0)     2441 2024-04-04 09:45:48.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_network_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     8811 2024-02-18 16:52:58.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_signal.py
+-rw-rw-r--   0 root         (0) root         (0)      771 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 11:32:26.618934 wivi_graph_client_py-2.1.2/wivi_graph_client_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-04-04 11:32:26.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-04-04 11:32:26.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 11:32:26.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 11:32:26.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-04 11:32:26.000000 wivi_graph_client_py-2.1.2/wivi_graph_client_py.egg-info/top_level.txt
```

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/client.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/client.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/configuration.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,9 @@
             createConfiguration(input: $input) {
                 id
                 deviceId
                 vehicleId
                 organizationId
                 fleetId
             }
+        }
     """
```

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_connection.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/device_connection.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_info.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/device_info.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_status.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/device_status.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_version.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/device_version.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/dtc.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/dtc.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/fail_processing.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/fail_processing.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/formula.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/formula.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/gps.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/gps.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/main.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/main.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/message.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/message.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/network_stats.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/network_stats.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/signal.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/signal.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_configuration.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_configuration.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_device_connection.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_device_connection.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_device_version.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_device_version.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_dtc.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_dtc.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_fail_processing.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_fail_processing.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_gps.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_gps.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_message.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_message.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_network_stats.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_network_stats.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_signal.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/test_signal.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py/version.py` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py/version.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/SOURCES.txt` & `wivi_graph_client_py-2.1.2/wivi_graph_client_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

