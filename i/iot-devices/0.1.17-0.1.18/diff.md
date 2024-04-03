# Comparing `tmp/iot_devices-0.1.17.tar.gz` & `tmp/iot_devices-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iot_devices-0.1.17.tar", last modified: Wed Feb 21 04:44:42 2024, max compression
+gzip compressed data, was "iot_devices-0.1.18.tar", last modified: Wed Apr  3 23:29:24 2024, max compression
```

## Comparing `iot_devices-0.1.17.tar` & `iot_devices-0.1.18.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.048868 iot_devices-0.1.17/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2022-02-10 22:14:24.000000 iot_devices-0.1.17/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     4177 2024-02-21 04:44:42.044868 iot_devices-0.1.17/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     3888 2024-01-17 11:22:56.000000 iot_devices-0.1.17/README.md
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2022-01-03 09:54:14.000000 iot_devices-0.1.17/iot_devices/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    32142 2024-02-03 02:38:18.000000 iot_devices-0.1.17/iot_devices/device.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/ESPHomePlugin/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    10116 2023-12-25 04:28:15.000000 iot_devices-0.1.17/iot_devices/devices/ESPHomePlugin/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/RTL433/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    11157 2023-11-21 01:00:18.000000 iot_devices-0.1.17/iot_devices/devices/RTL433/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/RokuRemoteApp/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    16072 2022-12-26 22:53:44.000000 iot_devices-0.1.17/iot_devices/devices/RokuRemoteApp/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/WeatherPlugin/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3227 2023-08-30 00:32:34.000000 iot_devices-0.1.17/iot_devices/devices/WeatherPlugin/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/Yeelight/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     9537 2023-11-21 00:39:42.000000 iot_devices-0.1.17/iot_devices/devices/Yeelight/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/YoLink/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    16934 2023-11-21 00:36:22.000000 iot_devices-0.1.17/iot_devices/devices/YoLink/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/Zigbee2MQTTPlugin/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    13322 2024-01-17 11:17:21.000000 iot_devices-0.1.17/iot_devices/devices/Zigbee2MQTTPlugin/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        2 2022-01-03 09:54:14.000000 iot_devices-0.1.17/iot_devices/devices/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/alarm/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      908 2023-11-20 03:14:46.000000 iot_devices-0.1.17/iot_devices/devices/alarm/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/demo/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1813 2023-10-25 01:16:55.000000 iot_devices-0.1.17/iot_devices/devices/demo/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/rfc_ser_server/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1813 2023-10-21 01:06:28.000000 iot_devices-0.1.17/iot_devices/devices/rfc_ser_server/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices/devices/servermonitor/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4099 2024-02-03 03:27:42.000000 iot_devices-0.1.17/iot_devices/devices/servermonitor/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2126 2024-01-16 04:14:09.000000 iot_devices-0.1.17/iot_devices/devices_manifest.json
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4928 2023-12-14 00:41:54.000000 iot_devices-0.1.17/iot_devices/host.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    11308 2024-01-17 11:23:49.000000 iot_devices-0.1.17/iot_devices/tui_dash.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-02-21 04:44:42.044868 iot_devices-0.1.17/iot_devices.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     4177 2024-02-21 04:44:41.000000 iot_devices-0.1.17/iot_devices.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      869 2024-02-21 04:44:42.000000 iot_devices-0.1.17/iot_devices.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-02-21 04:44:41.000000 iot_devices-0.1.17/iot_devices.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       56 2024-02-21 04:44:41.000000 iot_devices-0.1.17/iot_devices.egg-info/entry_points.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       44 2024-02-21 04:44:41.000000 iot_devices-0.1.17/iot_devices.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2024-02-21 04:44:41.000000 iot_devices-0.1.17/iot_devices.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-02-21 04:44:42.048868 iot_devices-0.1.17/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      659 2024-02-21 04:43:28.000000 iot_devices-0.1.17/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.289176 iot_devices-0.1.18/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2022-02-10 22:14:24.000000 iot_devices-0.1.18/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4964 2024-04-03 23:29:24.285176 iot_devices-0.1.18/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     4675 2024-04-03 23:18:12.000000 iot_devices-0.1.18/README.md
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       15 2022-01-03 09:54:14.000000 iot_devices-0.1.18/iot_devices/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    33278 2024-04-02 04:50:43.000000 iot_devices-0.1.18/iot_devices/device.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/ESPHomePlugin/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    10116 2023-12-25 04:28:15.000000 iot_devices-0.1.18/iot_devices/devices/ESPHomePlugin/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/GPIODevice/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     6475 2024-04-02 04:53:29.000000 iot_devices-0.1.18/iot_devices/devices/GPIODevice/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/RTL433/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    11105 2024-04-02 00:09:26.000000 iot_devices-0.1.18/iot_devices/devices/RTL433/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/RokuRemoteApp/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    16033 2024-04-02 05:41:11.000000 iot_devices-0.1.18/iot_devices/devices/RokuRemoteApp/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/WeatherPlugin/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3227 2023-08-30 00:32:34.000000 iot_devices-0.1.18/iot_devices/devices/WeatherPlugin/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/Yeelight/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     9397 2024-04-02 00:09:21.000000 iot_devices-0.1.18/iot_devices/devices/Yeelight/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/YoLink/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    17311 2024-02-21 05:13:55.000000 iot_devices-0.1.18/iot_devices/devices/YoLink/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/Zigbee2MQTTPlugin/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13274 2024-04-02 04:54:35.000000 iot_devices-0.1.18/iot_devices/devices/Zigbee2MQTTPlugin/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        2 2022-01-03 09:54:14.000000 iot_devices-0.1.18/iot_devices/devices/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/alarm/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      908 2023-11-20 03:14:46.000000 iot_devices-0.1.18/iot_devices/devices/alarm/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/demo/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1841 2024-04-02 19:04:20.000000 iot_devices-0.1.18/iot_devices/devices/demo/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/rfc_ser_server/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1813 2023-10-21 01:06:28.000000 iot_devices-0.1.18/iot_devices/devices/rfc_ser_server/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices/devices/servermonitor/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4115 2024-04-02 05:41:59.000000 iot_devices-0.1.18/iot_devices/devices/servermonitor/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2511 2024-04-03 23:11:09.000000 iot_devices-0.1.18/iot_devices/devices_manifest.json
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5286 2024-04-02 05:37:37.000000 iot_devices-0.1.18/iot_devices/host.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     3882 2024-04-02 05:38:37.000000 iot_devices-0.1.18/iot_devices/iot_devices_scan.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     8025 2024-04-02 04:19:51.000000 iot_devices-0.1.18/iot_devices/tui_dash.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-03 23:29:24.285176 iot_devices-0.1.18/iot_devices.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     4964 2024-04-03 23:29:24.000000 iot_devices-0.1.18/iot_devices.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      944 2024-04-03 23:29:24.000000 iot_devices-0.1.18/iot_devices.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2024-04-03 23:29:24.000000 iot_devices-0.1.18/iot_devices.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       56 2024-04-03 23:29:24.000000 iot_devices-0.1.18/iot_devices.egg-info/entry_points.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       53 2024-04-03 23:29:24.000000 iot_devices-0.1.18/iot_devices.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2024-04-03 23:29:24.000000 iot_devices-0.1.18/iot_devices.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2024-04-03 23:29:24.289176 iot_devices-0.1.18/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      679 2024-04-03 23:29:10.000000 iot_devices-0.1.18/setup.py
```

### Comparing `iot_devices-0.1.17/LICENSE` & `iot_devices-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `iot_devices-0.1.17/PKG-INFO` & `iot_devices-0.1.18/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: iot_devices
-Version: 0.1.17
-Summary: UNKNOWN
-Home-page: https://github.com/EternityForest/iot_devices
-Author: Daniel Dunn
-Author-email: dannydunn@eternityforest.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # iot_devices
 
 Very early draft of a platform independent abstraction of the idea of a "device".
 
 The intent is that you can make plugins for automation frameworks that can also be trivially used as a standalone library.
 
 The API is basically: Get a class based on a data dict, and make it.
@@ -110,44 +98,67 @@
 
 Note: We never have to import the module ourselves. It is imported on demand based on the data!  We automatically search sys.path.
 
 
 [Full host API docs](https://eternityforest.github.io/iot_devices/docs/iot_devices/host.html)
 
 ``` python
-from iot_devices.host import get_class
+from iot_devices.host import get_class, create_device
 
 data = {
-    "type": "RandomDevice"
+    "type": "DemoDevice"
 }
 
 
 # Get the class that would be able to construct a matching device given the data
 c = get_class(data)
 
-# Make an instance of that device
-device = c("Random Device", data)
+# Make an instance of that device.
+# Create device is very simple, it just calls cls(name, data),
+# But you can override it to add hooks whenever a device is created.
+device = create_device(c ,"Random Device", data)
 
 #One of the values this class exposes.
 # Note that values here can be "None" if there is no data yet.
 print(device.datapoints['random'])
 
 # This is an on-demand getter.  
 # This explicitly calls the getter we set.
 # It also sets the key in device.datapoints
 print(device.request_data_point('dyn_random'))
 
 # clean up
-c.close()
+device.close()
 ```
 
 ### Using subdevices
 
 See host_demo.py
 
 
 
 ### Docs for the included devices
 
-See devicedocs.md.  Note these are generated with tui-dash inspect-deep, an experimental
-command that actually creates an instance of every device.
+See devicedocs.md for a code example of each one.  Note these are generated with iot_devices_scan.py.  This script searches all of the python paths for any folder that contains devices,  creates
+an instance of each one, and inspects the object to generate report, including a usable code example.
+
+For example, here's an auto-generated example of using a GPIO input, powered by the GPIOZero library.
+
+```python
+from iot_devices.host import create_device
+from iot_devices.devices.GPIODevice import GPIOInput
+
+dev = create_device(GPIOInput, "name", {
+    'device.active_high': 'true',
+    'device.pull_up': 'false',
+    'device.pull_down': 'false',
+    'device.pin': 'MOCK1',
+    'device.debounce_time_ms': '0'
+})
+
+
+
+# boolean
+print(dev.datapoints['value'])
+# >>> 0
 
+```
```

### Comparing `iot_devices-0.1.17/README.md` & `iot_devices-0.1.18/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: iot_devices
+Version: 0.1.18
+Summary: UNKNOWN
+Home-page: https://github.com/EternityForest/iot_devices
+Author: Daniel Dunn
+Author-email: dannydunn@eternityforest.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # iot_devices
 
 Very early draft of a platform independent abstraction of the idea of a "device".
 
 The intent is that you can make plugins for automation frameworks that can also be trivially used as a standalone library.
 
 The API is basically: Get a class based on a data dict, and make it.
@@ -98,43 +110,68 @@
 
 Note: We never have to import the module ourselves. It is imported on demand based on the data!  We automatically search sys.path.
 
 
 [Full host API docs](https://eternityforest.github.io/iot_devices/docs/iot_devices/host.html)
 
 ``` python
-from iot_devices.host import get_class
+from iot_devices.host import get_class, create_device
 
 data = {
-    "type": "RandomDevice"
+    "type": "DemoDevice"
 }
 
 
 # Get the class that would be able to construct a matching device given the data
 c = get_class(data)
 
-# Make an instance of that device
-device = c("Random Device", data)
+# Make an instance of that device.
+# Create device is very simple, it just calls cls(name, data),
+# But you can override it to add hooks whenever a device is created.
+device = create_device(c ,"Random Device", data)
 
 #One of the values this class exposes.
 # Note that values here can be "None" if there is no data yet.
 print(device.datapoints['random'])
 
 # This is an on-demand getter.  
 # This explicitly calls the getter we set.
 # It also sets the key in device.datapoints
 print(device.request_data_point('dyn_random'))
 
 # clean up
-c.close()
+device.close()
 ```
 
 ### Using subdevices
 
 See host_demo.py
 
 
 
 ### Docs for the included devices
 
-See devicedocs.md.  Note these are generated with tui-dash inspect-deep, an experimental
-command that actually creates an instance of every device.
+See devicedocs.md for a code example of each one.  Note these are generated with iot_devices_scan.py.  This script searches all of the python paths for any folder that contains devices,  creates
+an instance of each one, and inspects the object to generate report, including a usable code example.
+
+For example, here's an auto-generated example of using a GPIO input, powered by the GPIOZero library.
+
+```python
+from iot_devices.host import create_device
+from iot_devices.devices.GPIODevice import GPIOInput
+
+dev = create_device(GPIOInput, "name", {
+    'device.active_high': 'true',
+    'device.pull_up': 'false',
+    'device.pull_down': 'false',
+    'device.pin': 'MOCK1',
+    'device.debounce_time_ms': '0'
+})
+
+
+
+# boolean
+print(dev.datapoints['value'])
+# >>> 0
+
+```
+
```

### Comparing `iot_devices-0.1.17/iot_devices/device.py` & `iot_devices-0.1.18/iot_devices/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,17 @@
     made by the driver.
     """
 
     # this name must be the same as the name of the device itself
     device_type: str = "Device"
     default_config = {}
 
-    # Iterable of config keys that should be considered secret, and hidden behind asterisks and such.
-    config_secrets = {}
-
     # This represents either a long text readme or an absolute path beginning with / to such
     readme: str = ''
 
-    # Used to store properties about config keys
-    config_properties: Dict[str, Dict[str, Any]] = {}
-
     def __init__(self, name: str, config: Dict[str, str], subdevice_config=None, **kw):
         """ 
 
         The base class __init__ does nothing if 
         called a second time, to simplify the complex
         inheritance.
 
@@ -111,15 +105,15 @@
                 Taken from config['title'] if possible, otherwise it is the name.
 
             config:
                 The current configuration of the device
 
             config_properties:
 
-                Class level property. For each key in config, there MAY be a
+                For each key in config, there MAY be a
                 key in this dict, that can contain any of these optional keys.
 
                 secret:
                     Denotes that the key must be protected from shoulder surfing
 
                 description:
                     Free text
@@ -152,14 +146,18 @@
 
 
                 All your device-specific options should begin with device.
 
                 Subdevice configuration must have is_subdevice: True in save files so the host does not try to create it by itself.
         """
 
+        if not hasattr(self, "config_properties"):
+            # Used to store properties about config keys
+            self.config_properties: Dict[str, Dict[str, Any]] = {}
+
         # Due to complex inheritance patterns, this could be called more than once
         if not hasattr(self, "__initial_setup"):
 
             config = copy.deepcopy(config)
 
             if config.get("type", self.device_type) != self.device_type:
                 raise ValueError(
@@ -185,14 +183,17 @@
             self.config: Dict[str, str] = config
 
             self.title: str = self.config.get('title', '').strip() or name
 
             self.__datapointhandlers: Dict[str, Callable] = {}
             self.datapoints = {}
 
+            # Used mostly to determine if the data is still the default.
+            self.__datapoint_timestamps = {}
+
             # Functions that can be called to explicitly request a data point
             # That return the new value
             self.__datapoint_getters: Dict[str, Callable] = {}
 
             for i in self.default_config:
                 if i not in self.config:
                     self.set_config_option(i, self.default_config[i])
@@ -397,14 +398,15 @@
 
     def numeric_data_point(self,
                            name: str,
                            min: Optional[float] = None,
                            max: Optional[float] = None,
                            hi: Optional[float] = None,
                            lo: Optional[float] = None,
+                           default: Optional[float] = None,
                            description: str = "",
                            unit: str = '',
                            handler: Optional[Callable[[
                                float, float, Any], Any]] = None,
                            interval: float = 0,
                            subtype: str = '',
                            writable=True,
@@ -426,15 +428,17 @@
             hi: A value the point can take on that would be considered excessive
             lo: A value the point can take on that would be considered excessively low
 
             description: Free text
 
             unit: A unit of measure, such as "degC" or "MPH"
 
-            handler: A function taking the value,timestamp, and annotation on changes
+            default: If unset default value is None, or may be framework defined. Default does not trigger handler.
+
+            handler: A function taking the value,timestamp, and annotation on changes.
 
             interval :annotates the default data rate the point will produce, for use in setting default poll
                 rates by the host, if the host wants to poll.  It does not mean the host SHOULD poll this, 
                 it only suggest a rate to poll at if the host has an interest in this data.
 
             writable:  is purely for a host that might subclass this, to determine if it should allow writing to the point.
 
@@ -448,15 +452,15 @@
             minval = min
 
         if max is None:
             maxval: float = 10**24
         else:
             maxval = max
 
-        self.datapoints[name] = None
+        self.datapoints[name] = default
 
         def on_change_attempt(v1: Optional[float], t, a):
             if v1 is None:
                 return
             if callable(v1):
                 v1 = v1()
 
@@ -469,15 +473,18 @@
 
             v = minimum(maxval, v)
             v = maximum(minval, v)
 
             t = t or time.monotonic()
 
             if self.datapoints[name] == v:
-                return
+                # It's still considered a change if the previous value
+                # was the default.
+                if self.__datapoint_timestamps.get(name, 0):
+                    return
 
             self.datapoints[name] = v
 
             # Handler used by the device
             if handler:
                 handler(v, t, a)
 
@@ -487,14 +494,15 @@
 
     def string_data_point(self,
                           name: str,
                           description: str = "",
                           unit: str = '',
                           handler: Optional[Callable[[
                               str, float, Any], Any]] = None,
+                          default: Optional[str] = None,
                           interval: float = 0,
                           writable=True,
                           subtype: str = '',
                           **kwargs):
         """Register a new string data point with the given properties. 
 
         Handler will be called when it changes.
@@ -505,40 +513,46 @@
 
         Most fields are just extra annotations to the host.
 
 
         Args:
             description: Free text
 
-            handler: A function taking the value,timestamp, and annotation on changes
+            default: If unset default value is None, or may be framework defined. Default does not trigger handler.
+
+            handler: A function taking the value,timestamp, and annotation on changes.
 
             interval: annotates the default data rate the point will produce, for use in setting default poll
                 rates by the host if the host wants to poll.  
 
                 It does not mean the host SHOULD poll this, 
                 it only suggest a rate to poll at if the host has an interest in this data.
 
             writable:  is purely for a host that might subclass this, to determine if it should allow writing to the point.
 
             subtype: A string further describing the data type of this value, as a hint to UI generation.
 
         """
 
-        self.datapoints[name] = None
+        self.datapoints[name] = default
 
         def onChangeAttempt(v: Optional[str], t, a):
+            "This function handles the change detection by itself"
             if v is None:
                 return
             if callable(v):
                 v = v()
             v = str(v)
             t = t or time.monotonic()
 
             if self.datapoints[name] == v:
-                return
+                # It's still considered a change if the previous value
+                # was the default.
+                if self.__datapoint_timestamps.get(name, 0):
+                    return
 
             self.datapoints[name] = v
 
             # Handler used by the device
             if handler:
                 handler(v, t, a)
 
@@ -599,15 +613,18 @@
 
             # Mutability trouble
             v = copy.deepcopy(v)
 
             t = t or time.monotonic()
 
             if self.datapoints[name] == v:
-                return
+                # It's still considered a change if the previous value
+                # was the default.
+                if self.__datapoint_timestamps.get(name, 0):
+                    return
 
             self.datapoints[name] = v
 
             # Handler used by the device
             if handler:
                 handler(v, t, a)
 
@@ -680,14 +697,15 @@
         This must be thread safe, but the change detection could glitch out and discard if you go from A to B and back to A again.
 
         When there is multiple writers you will want to aither do your own lock or ensure that you use unique values, 
         like with an event counter.
 
         """
 
+        self.__datapoint_timestamps[name] = timestamp
         self.__datapointhandlers[name](value, timestamp, annotation)
 
     def set_data_point_getter(self, name: str, getter: Callable):
         """Set the Getter of a datapoint, making it into an on-request point.
         The callable may return either the new value, or None if it has no new data.
         """
         self.__datapoint_getters[name] = getter
@@ -701,17 +719,20 @@
 
         Meant to be called by external host code.
 
         """
         if name in self.__datapoint_getters:
             x = self.__datapoint_getters[name]()
             if x is not None:
+                timestamp = time.monotonic()
                 # there has been a change! Maybe!  call a handler
                 self.__datapointhandlers[name](
-                    x, time.monotonic(), "From getter")
+                    x, timestamp, "From getter")
+
+                self.__datapoint_timestamps[name] = timestamp
                 self.datapoints[name] = x
                 return x
 
         return self.datapoints[name]
 
     def set_alarm(self, name: str, datapoint: str,
                   expression: str, priority: str = "info",
```

### Comparing `iot_devices-0.1.17/iot_devices/devices/ESPHomePlugin/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/ESPHomePlugin/__init__.py`

 * *Files identical despite different names*

### Comparing `iot_devices-0.1.17/iot_devices/devices/RTL433/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/RTL433/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,10 +295,7 @@
             all_devs[self.name] = self
         except Exception:
             self.handle_exception()
 
     def close(self):
         return super().close()
         self.connection.unsubscribe(self.noGarbage[0])
-
-    def getManagementForm(self):
-        return ""
```

### Comparing `iot_devices-0.1.17/iot_devices/devices/RokuRemoteApp/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/RokuRemoteApp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+import os.path
+import os
+import asyncio
+from contextlib import closing
+import socket
+import time
 from re import L
 import uuid
 from iot_devices import device
 import threading
 import logging
 
 
@@ -60,26 +66,22 @@
         <SCPDURL>ecp_SCPD.xml</SCPDURL>
     </service>
     </serviceList>
 </device>
 </root>"""
 
 
-def ssdpxml(name,uuid):
-    return x.replace("FN", name).replace('XXXX',uuid.replace('-','').upper())
+def ssdpxml(name, uuid):
+    return x.replace("FN", name).replace('XXXX', uuid.replace('-', '').upper())
 
 
 logger = logging.Logger("plugins.pyremote")
 
-import time
-import socket
 
 # Attr: https://stackoverflow.com/questions/1365265/on-localhost-how-do-i-pick-a-free-port-number
-import socket
-from contextlib import closing
 
 
 def find_free_port():
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
         s.bind(('0.0.0.0', 0))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         return s.getsockname()[1]
@@ -173,15 +175,15 @@
                 s = {}
                 s.update(self.services[i])
                 s.update(reply)
                 s['ST'] = s.get('ST', i)
 
                 s['Location'] = s['Location'].replace(
                     'localhost', getLocalIPForRemoteClient(a))
-                
+
                 s['LOCATION'] = s['LOCATION'].replace(
                     'localhost', getLocalIPForRemoteClient(a))
                 if not 'USN' in s:
                     s['USN'] = 'uuid:' + getUID() + "::" + s['ST']
                 s = make_httpu(s)
                 self.sock.sendto(s, a)
 
@@ -223,22 +225,14 @@
     for l in lines:
         tokens = l.split(':', 1)
         if len(tokens) > 1:
             d[tokens[0]] = tokens[1].strip()
     return d
 
 
-import logging
-import asyncio
-
-
-import os
-import os.path
-
-
 def tzget():
     tzname = os.environ.get('TZ')
     if tzname:
         return tzname
     elif os.path.exists('/etc/timezone'):
         with open('/etc/timezone') as f:
             return f.read().strip()
@@ -308,18 +302,14 @@
     <grandcentral-version>5.5.62</grandcentral-version>
     <trc-version>3.0</trc-version>
     <trc-channel-version>4.2.3</trc-channel-version>
     <davinci-version>2.8.20</davinci-version>
     </device-info>"""
 
 
-import logging
-import asyncio
-
-
 class RokuRemoteApp(device.Device):
     device_type = 'RokuRemoteApp'
     readme = """
 Implements an extended version of the (https://developer.roku.com/docs/developer-program/debugging/external-control-api.md)[Roku ECP protocol].  Does not currently work with most real Roku apps,
 intended mostly for use with DIY handheld remotes.
 
 We condense everything down to a single "Command" tag.  "Launch" commands are mapped to a string like "launch:78797".
@@ -348,21 +338,22 @@
         device.Device.__init__(self, name, data)
         self.closed = False
         self.httpd = None
 
         self.object_data_point("command", subtype='event')
         self.set_data_point('command', [None, time.monotonic(), None])
 
-        self.numeric_data_point("battery", min=0, max=100, unit="%")
+        self.numeric_data_point(
+            "battery", min=0, max=100, unit="%", writable=False)
         self.set_alarm('LowBattery', datapoint='battery', expression='value < 20',
                        priority='warning', release_condition='value > 35')
 
         try:
             self.set_config_default("device.serial", "P0A070000007")
-            self.set_config_default("device.uuid",str(uuid.uuid4()))
+            self.set_config_default("device.uuid", str(uuid.uuid4()))
             self.set_config_default(
                 "device.bind", "0.0.0.0:" + str(find_free_port()))
 
             if not self.config['device.bind'].strip():
                 raise RuntimeError("No address selected")
 
             p = self.config['device.bind'].split(":")[1]
@@ -370,37 +361,38 @@
 
             self.bind = self.config['device.bind']
             if not check_port(p):
                 self.bind = "0.0.0.0:" + str(find_free_port())
 
             self.ssdp = HTTPUServer()
             self.ssdp.services = {'roku:ecp': {'Location': "http://" + self.bind.replace('0.0.0.0', 'localhost'),
-                                                'LOCATION': "http://" + self.bind.replace('0.0.0.0', 'localhost'),
-                                               'USN': 'uuid:roku:ecp:'+self.config['device.uuid'].replace('-','').upper(),
+                                               'LOCATION': "http://" + self.bind.replace('0.0.0.0', 'localhost'),
+                                               'USN': 'uuid:roku:ecp:'+self.config['device.uuid'].replace('-', '').upper(),
                                                'Cache-Control': 'max-age=3600'
                                                }}
 
             class S(BaseHTTPRequestHandler):
                 def _set_headers(s):
                     s.send_response(200)
                     s.send_header("Content-type", "text/xml")
                     s.end_headers()
 
                 def do_GET(s):
-                    if not s.path.endswith('.png'):                               
+                    if not s.path.endswith('.png'):
                         s.send_response(200)
-                        s.send_header('Content-Type', 'text/xml; charset=utf-8')
+                        s.send_header('Content-Type',
+                                      'text/xml; charset=utf-8')
                         s.end_headers()
-                    else:                        
+                    else:
                         s.send_response(200)
                         s.send_header("Content-type", "image/png")
                         s.end_headers()
-        
-                    if s.path=='/query/apps':
-                        x="""<apps>
+
+                    if s.path == '/query/apps':
+                        x = """<apps>
                         <app id="11">Roku Channel Store</app>
                         <app id="12">Netflix</app>
                         <app id="13">Amazon Video on Demand</app>
                         <app id="837">YouTube</app>
                         <app id="2016">Crackle</app>
                         <app id="3423">Rdio</app>
                         <app id="21952">Blockbuster</app>
@@ -411,21 +403,22 @@
                         </apps>""".encode()
                         x.wfile.write(x.encode())
 
                     if s.path == '/query/device-info':
                         s.wfile.write(fakeroku(self.name).encode())
 
                     elif s.path == "/":
-                        s.wfile.write(ssdpxml(self.name, self.config['device.uuid']).encode())
+                        s.wfile.write(
+                            ssdpxml(self.name, self.config['device.uuid']).encode())
 
                     elif s.path == '/unixtime':
                         s.wfile.write(str(time.time()).encode())
 
                     elif s.path == '/device-image.png':
-                        with open(os.path.join(os.path.dirname(__file__), "placeholder.png"),'rb') as f:
+                        with open(os.path.join(os.path.dirname(__file__), "placeholder.png"), 'rb') as f:
                             s.wfile.write(f.read())
 
                 def do_HEAD(s):
                     s._set_headers()
 
                 def do_POST(s):
                     s._set_headers()
```

### Comparing `iot_devices-0.1.17/iot_devices/devices/WeatherPlugin/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/WeatherPlugin/__init__.py`

 * *Files identical despite different names*

### Comparing `iot_devices-0.1.17/iot_devices/devices/Yeelight/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/Yeelight/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,11 +298,7 @@
                 }
             )
 
             l[lookup[i]['capabilities'].get(
                 "name", '') or lookup[i]['ip']] = config2
 
         return l
-
-    def getManagementForm(self):
-        return templateGetter.get_template("bulbpage.html").render(
-            data=self.data, obj=self)
```

### Comparing `iot_devices-0.1.17/iot_devices/devices/YoLink/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/YoLink/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,17 +76,24 @@
         self.topic2 = "yl-home/" + homeid + "/+/response"
 
         self.mqtt_url = mqtt_url
         self.mqtt_port = int(mqtt_port)
         self.key = key
         self.parent = parent
 
-        self.client = mqtt.Client(client_id=str(__name__ + str(client_id)),
-                                  clean_session=True, userdata=None,
-                                  protocol=mqtt.MQTTv311, transport="tcp")
+        try:
+            self.client = mqtt.Client(client_id=str(__name__ + str(client_id)),
+                                      clean_session=True, userdata=None,
+                                      protocol=mqtt.MQTTv311, transport="tcp")
+        except TypeError:
+            self.client = mqtt.Client(callback_api_version=mqtt.CallbackAPIVersion.VERSION1,
+                                      client_id=str(__name__ + str(client_id)),
+                                      clean_session=True, userdata=None,
+                                      protocol=mqtt.MQTTv311, transport="tcp")
+
         self.client.reconnect_delay_set(60, 30*60)
         self.client.on_connect = self.on_connect
         self.client.on_message = self.on_message
 
     def close(self):
         self.client.disconnect()
         self.client.loop_stop()
```

### Comparing `iot_devices-0.1.17/iot_devices/devices/Zigbee2MQTTPlugin/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/Zigbee2MQTTPlugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,15 @@
         self.set_config_default("device.friendly_name", '__all__')
 
         try:
             from kaithem.src.scullery import mqtt
 
             # Ensure a new real connection.  This makes sure we get any retained messages.
             self.connection = mqtt.getConnection(
-                self.config['device.mqtt_server'],
-                connection_id=str(time.time()))
+                self.config['device.mqtt_server'])
 
             self.connection.subscribe('zigbee2mqtt/bridge/devices',
                                       self.onDevices)
         except Exception:
             self.handle_exception()
 
     def on_data_point_change(self, tn, v, t, a):
```

### Comparing `iot_devices-0.1.17/iot_devices/devices/alarm/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/alarm/__init__.py`

 * *Files identical despite different names*

### Comparing `iot_devices-0.1.17/iot_devices/devices/demo/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/rfc_ser_server/__init__.py`

 * *Files identical despite different names*

### Comparing `iot_devices-0.1.17/iot_devices/devices/rfc_ser_server/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/demo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from iot_devices import device
 
 import random
 import time
 import os
 
+
 class DemoDevice(device.Device):
     device_type = "DemoDevice"
-    def __init__(self,name, data, **kw):
-        device.Device.__init__(self,name, data, **kw)
+
+    def __init__(self, name, data, **kw):
+        device.Device.__init__(self, name, data, **kw)
 
         self.text_config_files = ['test.conf']
 
         try:
             if not os.path.exists(os.path.join(self.get_config_folder(), 'test.conf')):
-                with open(os.path.join(self.get_config_folder(), 'test.conf'),"w") as f:
+                with open(os.path.join(self.get_config_folder(), 'test.conf'), "w") as f:
                     f.write("Testing")
         except Exception:
             pass
 
-
-        self.set_config_default("device.fixed_number_multiplier","1")
+        self.set_config_default("device.fixed_number_multiplier", "1")
 
         # Push type data point set by the device
         self.numeric_data_point("random")
-        self.set_data_point("random",random.random() * float(self.config['device.fixed_number_multiplier']))
-
+        self.set_data_point("random", random.random(
+        ) * float(self.config['device.fixed_number_multiplier']))
 
         # On demand requestable data point pulled by application.
         # All you have to do is set the val to a callable.
-        self.numeric_data_point("dyn_random")
+        self.numeric_data_point("dyn_random", interval=10)
         self.numeric_data_point("useless_toggle", subtype="bool")
         self.numeric_data_point("do_nothing", subtype="trigger")
         self.numeric_data_point("read_only", writable=False)
         self.set_data_point("read_only", random.random())
 
         self.set_data_point_getter("dyn_random", random.random)
 
         if not 'gen2' in data:
-            self.create_subdevice(DemoDevice, "subdevice",{"gen2":True})
+            self.create_subdevice(DemoDevice, "subdevice", {"gen2": True})
 
     @classmethod
     def discover_devices(cls, config={}, current_device=None, intent=None, **kw):
 
-    
         # Return a modified version of the existing.
         # Never get rid of existing user work for no reason
         cfg = {
-            'device.fixed_number_multiplier':"1000"
+            'device.fixed_number_multiplier': "1000"
         }
-        config= config.copy()
+        config = config.copy()
         config.update(cfg)
 
-        return{ "Big fixed numbers":config}
+        return {"Big fixed numbers": config}
```

### Comparing `iot_devices-0.1.17/iot_devices/devices/servermonitor/__init__.py` & `iot_devices-0.1.18/iot_devices/devices/servermonitor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         device.Device.__init__(self, name, data, **kw)
 
         self.set_config_default("device.target", "")
         self.set_config_default("device.expect_pattern", "")
         self.set_config_default("device.check_interval", "300")
 
         # Push type data point set by the device
-        self.numeric_data_point("status", subtype='bool')
+        self.numeric_data_point("status", subtype='bool', writable=False)
         self.set_alarm("External Server Down", 'status',
                        "value<1", priority="error")
 
         self.stop_flag = id(self)
 
         t = threading.Thread(target=self.work_loop, daemon=True,
                              name="Monitor for "+self.config['device.target'])
```

### Comparing `iot_devices-0.1.17/iot_devices/devices_manifest.json` & `iot_devices-0.1.18/iot_devices/devices_manifest.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666667%*

 * *Differences: {"'devices'": "{'GPIOOutput': OrderedDict([('submodule', 'devices.GPIODevice'), ('description', "*

 * *              "'Experimental. Represents a hardware output pin, possibly with PWM.  Supports RasPi "*

 * *              "and mocked fake pins.')]), 'GPIOInput': OrderedDict([('submodule', "*

 * *              "'devices.GPIODevice'), ('description', 'Experimental. Represents a hardware input "*

 * *              "pin. Supports RasPi and mocked fake pins.')])}"}*

```diff
@@ -8,14 +8,22 @@
             "description": "Just a demo device that makes pseudorandom numbers on request",
             "submodule": "devices.demo"
         },
         "ESPHomeDevice": {
             "description": "Represents one single ESPHome device.  Cannot flash or update the ESP, use the dashboard tool for that.",
             "submodule": "devices.ESPHomePlugin"
         },
+        "GPIOInput": {
+            "description": "Experimental. Represents a hardware input pin. Supports RasPi and mocked fake pins.",
+            "submodule": "devices.GPIODevice"
+        },
+        "GPIOOutput": {
+            "description": "Experimental. Represents a hardware output pin, possibly with PWM.  Supports RasPi and mocked fake pins.",
+            "submodule": "devices.GPIODevice"
+        },
         "RTL433Client": {
             "description": "Listen to messages from rtl_433 and decode them into things like weather station data",
             "submodule": "devices.RTL433"
         },
         "RokuRemoteApp": {
             "description": "Allow Roku ECP protocol remotes to discover this server and control a tag point.",
             "submodule": "devices.RokuRemoteApp"
```

### Comparing `iot_devices-0.1.17/iot_devices/host.py` & `iot_devices-0.1.18/iot_devices/host.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import importlib
 import json
 import copy
 import logging
 import threading
 import traceback
-from typing import Dict, Type
+from typing import Dict, Type, TypeVar, Generic
 from . import device
 
 
 _known_device_types: Dict[str, Dict] = {}
 """
 Cache of discovered data about devices
 """
@@ -170,7 +170,17 @@
 
 
 def register_subdevice(parent: object, child: object):
     """
     A device can create other devices.  This lets a host do something with them.
     """
     pass
+
+
+def create_device(cls: Type[device.Device], name: str, data: Dict) -> device.Device:
+    """
+    Create a new device from it's data, given the device class,
+    and add any framework specific hooks.
+    This function is meant to be overriden by the host app,
+    to add framework specific functionality
+    """
+    return cls(name, data)
```

### Comparing `iot_devices-0.1.17/iot_devices.egg-info/PKG-INFO` & `iot_devices-0.1.18/iot_devices.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iot-devices
-Version: 0.1.17
+Version: 0.1.18
 Summary: UNKNOWN
 Home-page: https://github.com/EternityForest/iot_devices
 Author: Daniel Dunn
 Author-email: dannydunn@eternityforest.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -110,44 +110,68 @@
 
 Note: We never have to import the module ourselves. It is imported on demand based on the data!  We automatically search sys.path.
 
 
 [Full host API docs](https://eternityforest.github.io/iot_devices/docs/iot_devices/host.html)
 
 ``` python
-from iot_devices.host import get_class
+from iot_devices.host import get_class, create_device
 
 data = {
-    "type": "RandomDevice"
+    "type": "DemoDevice"
 }
 
 
 # Get the class that would be able to construct a matching device given the data
 c = get_class(data)
 
-# Make an instance of that device
-device = c("Random Device", data)
+# Make an instance of that device.
+# Create device is very simple, it just calls cls(name, data),
+# But you can override it to add hooks whenever a device is created.
+device = create_device(c ,"Random Device", data)
 
 #One of the values this class exposes.
 # Note that values here can be "None" if there is no data yet.
 print(device.datapoints['random'])
 
 # This is an on-demand getter.  
 # This explicitly calls the getter we set.
 # It also sets the key in device.datapoints
 print(device.request_data_point('dyn_random'))
 
 # clean up
-c.close()
+device.close()
 ```
 
 ### Using subdevices
 
 See host_demo.py
 
 
 
 ### Docs for the included devices
 
-See devicedocs.md.  Note these are generated with tui-dash inspect-deep, an experimental
-command that actually creates an instance of every device.
+See devicedocs.md for a code example of each one.  Note these are generated with iot_devices_scan.py.  This script searches all of the python paths for any folder that contains devices,  creates
+an instance of each one, and inspects the object to generate report, including a usable code example.
+
+For example, here's an auto-generated example of using a GPIO input, powered by the GPIOZero library.
+
+```python
+from iot_devices.host import create_device
+from iot_devices.devices.GPIODevice import GPIOInput
+
+dev = create_device(GPIOInput, "name", {
+    'device.active_high': 'true',
+    'device.pull_up': 'false',
+    'device.pull_down': 'false',
+    'device.pin': 'MOCK1',
+    'device.debounce_time_ms': '0'
+})
+
+
+
+# boolean
+print(dev.datapoints['value'])
+# >>> 0
+
+```
```

### Comparing `iot_devices-0.1.17/iot_devices.egg-info/SOURCES.txt` & `iot_devices-0.1.18/iot_devices.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
 setup.py
 iot_devices/__init__.py
 iot_devices/device.py
 iot_devices/devices_manifest.json
 iot_devices/host.py
+iot_devices/iot_devices_scan.py
 iot_devices/tui_dash.py
 iot_devices.egg-info/PKG-INFO
 iot_devices.egg-info/SOURCES.txt
 iot_devices.egg-info/dependency_links.txt
 iot_devices.egg-info/entry_points.txt
 iot_devices.egg-info/requires.txt
 iot_devices.egg-info/top_level.txt
 iot_devices/devices/__init__.py
 iot_devices/devices/ESPHomePlugin/__init__.py
+iot_devices/devices/GPIODevice/__init__.py
 iot_devices/devices/RTL433/__init__.py
 iot_devices/devices/RokuRemoteApp/__init__.py
 iot_devices/devices/WeatherPlugin/__init__.py
 iot_devices/devices/Yeelight/__init__.py
 iot_devices/devices/YoLink/__init__.py
 iot_devices/devices/Zigbee2MQTTPlugin/__init__.py
 iot_devices/devices/alarm/__init__.py
```

### Comparing `iot_devices-0.1.17/setup.py` & `iot_devices-0.1.18/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iot_devices',
-    version='0.1.17',
+    version='0.1.18',
     author="Daniel Dunn",
     author_email="dannydunn@eternityforest.com",
     packages=find_packages(),
     package_data={'': ["*.json"]},
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
@@ -17,10 +17,11 @@
         ],
     },
     install_requires=[
         "paho-mqtt",
         "urwid",
         "scullery",
         "yeelight",
-        "colorzero"
+        "colorzero",
+        "gpiozero"
     ]
 )
```

