# Comparing `tmp/wivi_graph_client_py-1.0.0.tar.gz` & `tmp/wivi_graph_client_py-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wivi_graph_client_py-1.0.0.tar", last modified: Tue Jan 16 08:57:46 2024, max compression
+gzip compressed data, was "wivi_graph_client_py-2.1.1.tar", last modified: Thu Apr  4 09:53:19 2024, max compression
```

## Comparing `wivi_graph_client_py-1.0.0.tar` & `wivi_graph_client_py-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 08:57:46.054310 wivi_graph_client_py-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-16 08:57:46.054310 wivi_graph_client_py-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-16 08:57:46.054310 wivi_graph_client_py-1.0.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      449 2024-01-16 08:47:52.000000 wivi_graph_client_py-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 08:57:46.054310 wivi_graph_client_py-1.0.0/wivi_graph_client_py/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8590 2023-11-23 13:49:45.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/client.py
--rw-rw-r--   0 root         (0) root         (0)      954 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     1521 2023-11-23 15:14:56.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/device_connection.py
--rw-rw-r--   0 root         (0) root         (0)      886 2023-11-23 09:54:12.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/device_info.py
--rw-rw-r--   0 root         (0) root         (0)      920 2023-11-23 10:41:03.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/device_status.py
--rw-rw-r--   0 root         (0) root         (0)      921 2023-11-23 10:48:43.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/device_version.py
--rw-rw-r--   0 root         (0) root         (0)      913 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/dtc.py
--rw-rw-r--   0 root         (0) root         (0)      217 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/ecu.py
--rw-rw-r--   0 root         (0) root         (0)     1252 2023-11-14 13:44:52.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/fail_processing.py
--rw-rw-r--   0 root         (0) root         (0)     1226 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/formula.py
--rw-rw-r--   0 root         (0) root         (0)      867 2023-11-29 15:21:16.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/gps.py
--rw-rw-r--   0 root         (0) root         (0)      549 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/main.py
--rw-rw-r--   0 root         (0) root         (0)      643 2023-12-05 09:09:21.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/message.py
--rw-rw-r--   0 root         (0) root         (0)      213 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/network.py
--rw-rw-r--   0 root         (0) root         (0)     1055 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/network_stats.py
--rw-rw-r--   0 root         (0) root         (0)     1494 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/signal.py
--rw-rw-r--   0 root         (0) root         (0)     1669 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/test.py
--rw-rw-r--   0 root         (0) root         (0)      771 2023-10-02 08:31:05.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 08:57:46.054310 wivi_graph_client_py-1.0.0/wivi_graph_client_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-16 08:57:45.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      863 2024-01-16 08:57:46.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 08:57:45.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-01-16 08:57:45.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-16 08:57:45.000000 wivi_graph_client_py-1.0.0/wivi_graph_client_py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      449 2024-04-04 09:53:06.000000 wivi_graph_client_py-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/wivi_graph_client_py/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8590 2023-11-23 13:49:45.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/client.py
+-rw-rw-r--   0 root         (0) root         (0)     1239 2024-02-12 19:32:52.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     1283 2024-02-12 19:33:53.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_connection.py
+-rw-rw-r--   0 root         (0) root         (0)      886 2023-11-23 09:54:12.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_info.py
+-rw-rw-r--   0 root         (0) root         (0)     1060 2024-02-12 21:21:44.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_status.py
+-rw-rw-r--   0 root         (0) root         (0)      838 2024-02-12 21:21:41.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_version.py
+-rw-rw-r--   0 root         (0) root         (0)     1323 2024-02-12 21:24:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/dtc.py
+-rw-rw-r--   0 root         (0) root         (0)      217 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/ecu.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2024-02-12 21:24:43.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/fail_processing.py
+-rw-rw-r--   0 root         (0) root         (0)     1226 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/formula.py
+-rw-rw-r--   0 root         (0) root         (0)      864 2024-02-12 21:25:59.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/gps.py
+-rw-rw-r--   0 root         (0) root         (0)      549 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/main.py
+-rw-rw-r--   0 root         (0) root         (0)      647 2024-02-12 21:26:32.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/message.py
+-rw-rw-r--   0 root         (0) root         (0)      213 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/network.py
+-rw-rw-r--   0 root         (0) root         (0)     1000 2024-04-04 09:46:03.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/network_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     1345 2024-02-12 21:31:53.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/signal.py
+-rw-rw-r--   0 root         (0) root         (0)     2701 2024-02-18 20:16:53.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     2659 2024-02-19 09:44:20.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_device_connection.py
+-rw-rw-r--   0 root         (0) root         (0)     1437 2024-02-19 08:55:57.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_device_version.py
+-rw-rw-r--   0 root         (0) root         (0)     3459 2024-02-18 16:27:42.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_dtc.py
+-rw-rw-r--   0 root         (0) root         (0)     2575 2024-02-18 22:28:53.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_fail_processing.py
+-rw-rw-r--   0 root         (0) root         (0)     2066 2024-02-18 16:26:36.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_gps.py
+-rw-rw-r--   0 root         (0) root         (0)     1972 2024-02-18 20:50:16.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_message.py
+-rw-rw-r--   0 root         (0) root         (0)     2441 2024-04-04 09:45:48.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_network_stats.py
+-rw-rw-r--   0 root         (0) root         (0)     8811 2024-02-18 16:52:58.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/test_signal.py
+-rw-rw-r--   0 root         (0) root         (0)      771 2023-10-02 08:31:05.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 09:53:19.491735 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1195 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-04 09:53:19.000000 wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/top_level.txt
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/client.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/client.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/configuration.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 class Configuration_Query:
     get_configuration_query = """
-        query GetConfigurations($input: ConfigurationFilterInput) {
+        query configurations($input: ConfigurationFilterInput) {
+            configuration(input: $input) {
+                id
+                deviceId
+                fleetId
+                organizationId
+                vehicleId
+            }
+        }
+    """
+    configurationsMetaQuery = """
+        query configurations($input: ConfigurationFilterInput) {
             configuration(input: $input) {
                 id
                 deviceId
                 fleetId
                 organizationId
                 vehicleId
                 signals {
@@ -18,21 +29,18 @@
                 }
                 network {
                     name
                 }
             }
         }
     """
-
-
 class Configuration_Mutation:
     create_configuration_mutation = """
-        mutation CreateConfiguration($input: CreateConfigurationInput) {
+        mutation createConfiguration($input: CreateConfigurationInput!) {
             createConfiguration(input: $input) {
                 id
                 deviceId
-                fleetId
-                organizationId
                 vehicleId
+                organizationId
+                fleetId
             }
-        }
     """
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/device_connection.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_connection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 class Device_Connections_Query:
     get_device_connection_query = """
-        query GetDeviceConnection($input: DeviceConnectionFilterInput) {
+        query deviceConnection($input: DeviceConnectionFilterInput) {
             deviceConnection(input: $input) {
-                configuration:{
+                configuration {
+                    deviceId
                     vehicleId
-                    fleetId
                     organizationId
-                    deviceId
+                    fleetId
                 }
-                bytesReceived
-                bytesSent
-                networkProvider
-                network
-                networkType
-                version
-                startTime
-                endTime
-                time
             }
         }
     """
 
 
 class Device_Connections_Mutation:
 
     upsert_device_connection_mutation = '''
-        mutation UpsertDeviceConnection($input: CreateDeviceConnectionInput) {
+        mutation createDeviceConnection($input: CreateDeviceConnectionInput) {
             createDeviceConnection(input: $input) {
                 configuration {
                     vehicleId
                     fleetId
                     organizationId
                     deviceId
                 }
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/device_info.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_info.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/device_status.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 class Device_Status_Query:
     get_device_status_query = """
         query GetDeviceStatus($input: DeviceStatusFilterInput) {
-            deviceStatus(input: $input) {
+            DeviceStatus(input: $input) {
                 vehicleId
-                deviceStatusData {
+                DeviceStatusData {
                     name
                     data {
                         time
                         svalue
                         value
                     }
                 }
             }
         }
     """
 
 class Device_Status_Mutation:
     create_device_status_mutation = '''
-        mutation CreateDeviceStatus($input: CreateDeviceStatusInput) {
+        mutation createDeviceStatus($input: CreateDeviceStatusInput) {
             createDeviceStatus(input: $input) {
-                configurationId
+                configuration {
+                    deviceId
+                    vehicleId
+                    organizationId
+                    fleetId
+                }
             }
         }
     '''
 
     delete_device_status_mutation = '''
         mutation DeleteDeviceStatus($input: DeleteDeviceStatusInput) {
             deleteDeviceStatus(input: $input) {
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/device_version.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/device_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 class Device_Version_Query:
     get_device_version_query = """
-        query GetDeviceInfo($input: DeviceInfoFilterInput) {
-            deviceInfo(input: $input) {
+        query deviceVersion($input: DeviceVersionFilterInput) {
+            deviceVersion(input: $input) {
                 vehicleId
-                deviceInfoData {
+                deviceVersion {
                     name
-                    data {
-                        time
-                        svalue
-                        value
-                    }
+                    time
+                    value
                 }
             }
         }
     """
 class Device_Version_Mutation:
     upsert_device_version_mutation = '''
         mutation UpsertDeviceVersion($input: UpsertDeviceVersionInput) {
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/dtc.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/dtc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 class Dtc_Query:
     get_dtc_query = """
-        query GetDtcData($input: DtcDataFilterArgs) {
+        query dtcData($input: DtcDataFilterInput) {
             dtcData(input: $input) {
                 vehicleId
                 dtcs {
+                    messageName
+                    description
+                    uploadId
+                    domain
                     code
                     status
-                    message {
-                        id
-                        name
-                    }
-                    failure
-                    time
+                    dtcId
+                    value
                     count
+                    failure
+                    occurances {
+                        time
+                        state
+                        snapshots {
+                            time
+                            bytes
+                        }
+                        extensions {
+                            time
+                            bytes
+                        }
+                    }
                 }
             }
         }
     """
 
 class Dtc_Mutation:
     upsert_dtc_mutation = """
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/fail_processing.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/fail_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 class FailProcessingQuery:
     get_failed_processing_query = """
-        query GetFailedProcessing($input: FailedProcessingFilterInput) {
+        query failedProcessing($input: FailedProcessingFilterInput) {
             failedProcessing(input: $input) {
                 configuration {
-                    vehicleId
+                    id
+                    deviceId
                     fleetId
                     organizationId
                     vehicleId
                 }
-                uploadId
                 dbExists
-                xmlExists
                 pipelineStatus
+                uploadId
+                xmlExists
             }
         }
     """
 
 class FailProcessingMutation:
     upsert_failed_processing_mutation = '''
-        mutation UpsertFailedProcessing($input: UpsertFailedProcessingInput) {
+        mutation upsertFailedProcessing($input: UpsertFailedProcessingInput) {
             upsertFailedProcessing(input: $input) {
                 configuration {
+                    id
                     vehicleId
                     fleetId
                     organizationId
                     vehicleId
                 }
                 uploadId
                 dbExists
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/formula.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/formula.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/gps.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/gps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 class GPS_Query:
     get_gps_query = """
-        query GetGPSData($input: GPSDataFilterArgs) {
+        query gpsData($input: GpsDataFilterArgs) {
             gpsData(input: $input) {
                 vehicleId
                 gpsData {
+                    time
                     latitude
                     longitude
                     accuracy
                     altitude
-                    time
                 }
             }
         }
 """
 
 class GPS_Mutation:
     upsert_gps_mutation = """
-        mutation UpsertGPSData($input: UpsertGpsDataInput) {
+        mutation UpsertGpsData($input: UpsertGpsDataInput) {
             upsertGpsData(input: $input) {
                 deviceId
                 fleetId
                 vehicleId
                 id
                 organizationId
             }
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/main.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/main.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/message.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/message.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 class Message_Query:
     get_message_query = """
-        query GetMessages($input: MessageFilterArgs) {
+        query messages($input: MessageFilterArgs) {
             message(input: $input) {
-                id
                 arbId
                 name
                 networkId
+                networkName
                 ecuId
                 uploadId
             }
         }
     """
 
 class Message_Mutation:
     create_message_mutation = """
-        mutation CreateNewMessage($input: CreateMessageInput) {
+        mutation createMessage($input: CreateMessageInput!) {
             createMessage(input: $input) {
                 id
                 arbId
                 name
                 networkName
                 ecuId
                 uploadId
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/network_stats.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/network_stats.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 class Network_Stats_Query:
     get_network_stats_query = """
-        query GetNetworkStats($input: NetworkStatsFilter) {
+        query networkStatusQuery($input: NetworkStatsFilter) {
             networkStats(input: $input) {
-                id
-                name
-                vehicleId
-                uploadId
-                totalMessages
-                matchedMessages
-                unmatchedMessages
                 errorMessages
                 longMessageParts
-                minTime
+                matchedMessages
                 maxTime
-                rate
+                minTime
+                name
+                uploadId
+                vehicleId
+                unmatchedMessages
+                totalMessages
             }
         }
     """
 
 class Network_Stats_Mutation:
     create_network_stats_mutation = """
-        mutation CreateNetworkStats($input: CreateNetworkStatsInput) {
+        mutation createNetworkStats($input: CreateNetworkStatsInput!) {
             createNetworkStats(input: $input) {
-                id
                 name
                 vehicleId
                 uploadId
                 totalMessages
                 matchedMessages
                 unmatchedMessages
                 errorMessages
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/signal.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/signal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 class Signals_Query:
     get_signals_query = """
-        query GetSignals($input: SignalFilterArgs) {
+        query signals($input: SignalFilterArgs) {
             signal(input: $input) {
-                id
                 name
                 unit
                 paramType
+                paramId
+                messageName
                 configurationId
                 messageId
+                networkName
             }
         }
     """
 
     get_signals_data_query = """
-        query GetSignalData($input: SignalDataFilterArgs) {
+        query signalData($input: SignalDataFilterArgs) {
             signalData(input: $input) {
                 vehicleId
                 data {
                     value
                     signalType
                     time
                     signalId
@@ -28,28 +30,20 @@
         }
     """
 
 class Signals_Mutation:
     upsert_signal_data_mutation = """
         mutation UpsertSignalData($input: UpsertSignalDataArgs) {
             upsertSignalData(input: $input) {
-                id
-                name
-                unit
-                paramType
                 configurationId
                 messageId
-                signalData {
-                    value
-                    signalType
-                    time
-                    signalId
-                    stateId
-                    svalue
-                }
+                messageName
+                name
+                paramType
+                unit
             }
         }
     """
 
     delete_signal_data_mutation = """
         mutation DeleteSignalData($input: DeleteSignalDataInput) {
             deleteSignalData(input: $input) {
```

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py/version.py` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py/version.py`

 * *Files identical despite different names*

### Comparing `wivi_graph_client_py-1.0.0/wivi_graph_client_py.egg-info/SOURCES.txt` & `wivi_graph_client_py-2.1.1/wivi_graph_client_py.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 wivi_graph_client_py/formula.py
 wivi_graph_client_py/gps.py
 wivi_graph_client_py/main.py
 wivi_graph_client_py/message.py
 wivi_graph_client_py/network.py
 wivi_graph_client_py/network_stats.py
 wivi_graph_client_py/signal.py
-wivi_graph_client_py/test.py
+wivi_graph_client_py/test_configuration.py
+wivi_graph_client_py/test_device_connection.py
+wivi_graph_client_py/test_device_version.py
+wivi_graph_client_py/test_dtc.py
+wivi_graph_client_py/test_fail_processing.py
+wivi_graph_client_py/test_gps.py
+wivi_graph_client_py/test_message.py
+wivi_graph_client_py/test_network_stats.py
+wivi_graph_client_py/test_signal.py
 wivi_graph_client_py/version.py
 wivi_graph_client_py.egg-info/PKG-INFO
 wivi_graph_client_py.egg-info/SOURCES.txt
 wivi_graph_client_py.egg-info/dependency_links.txt
 wivi_graph_client_py.egg-info/requires.txt
 wivi_graph_client_py.egg-info/top_level.txt
```

