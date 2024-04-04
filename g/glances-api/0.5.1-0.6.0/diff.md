# Comparing `tmp/glances_api-0.5.1.tar.gz` & `tmp/glances_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glances_api-0.5.1.tar", max compression
+gzip compressed data, was "glances_api-0.6.0.tar", max compression
```

## Comparing `glances_api-0.5.1.tar` & `glances_api-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1110 2024-01-01 21:33:54.773932 glances_api-0.5.1/LICENSE
--rw-r--r--   0        0        0      956 2023-05-21 11:03:42.721345 glances_api-0.5.1/README.rst
--rw-r--r--   0        0        0     7524 2024-01-01 21:33:54.773932 glances_api-0.5.1/glances_api/__init__.py
--rw-r--r--   0        0        0      419 2024-01-01 21:33:54.773932 glances_api-0.5.1/glances_api/exceptions.py
--rw-r--r--   0        0        0     1389 2024-01-01 21:33:54.776932 glances_api-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 glances_api-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1110 2024-01-01 21:33:54.773932 glances_api-0.6.0/LICENSE
+-rw-r--r--   0        0        0      956 2023-05-21 11:03:42.721345 glances_api-0.6.0/README.rst
+-rw-r--r--   0        0        0     7969 2024-04-04 11:32:22.358861 glances_api-0.6.0/glances_api/__init__.py
+-rw-r--r--   0        0        0      419 2024-01-01 21:33:54.773932 glances_api-0.6.0/glances_api/exceptions.py
+-rw-r--r--   0        0        0     1385 2024-04-04 11:32:37.753003 glances_api-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 glances_api-0.6.0/PKG-INFO
```

### Comparing `glances_api-0.5.1/LICENSE` & `glances_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glances_api-0.5.1/README.rst` & `glances_api-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `glances_api-0.5.1/glances_api/__init__.py` & `glances_api-0.6.0/glances_api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Client to interact with the Glances API."""
+
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import httpx
 
@@ -149,18 +150,19 @@
             for cpu in data:
                 sensor_data["percpu"][str(cpu["cpu_number"])] = {
                     "cpu_use_percent": cpu["total"]
                 }
         if networks := self.data.get("network"):
             sensor_data["network"] = {}
             for network in networks:
+                time_since_update = network["time_since_update"]
                 sensor_data["network"][network["interface_name"]] = {
                     "is_up": network.get("is_up"),
-                    "rx": round(network["rx"] / 1024, 1),
-                    "tx": round(network["tx"] / 1024, 1),
+                    "rx": round(network["rx"] / time_since_update),
+                    "tx": round(network["tx"] / time_since_update),
                     "speed": round(network["speed"] / 1024**3, 1),
                 }
         data = self.data.get("dockers") or self.data.get("containers")
         if data and (containers_data := data.get("containers")):
             active_containers = [
                 container
                 for container in containers_data
@@ -178,15 +180,22 @@
         if data := self.data.get("raid"):
             sensor_data["raid"] = data
         if data := self.data.get("uptime"):
             sensor_data["uptime"] = data
         if data := self.data.get("gpu"):
             sensor_data["gpu"] = {}
             for sensor in data:
-                sensor_data["gpu"][f"GPU_{sensor['gpu_id']}__{sensor['name']}"] = {
-                    "name": sensor["name"],
-                    "temperature": sensor["temperature"],
-                    "mem": sensor["mem"],
-                    "proc": sensor["proc"],
-                    "fan_speed": sensor["fan_speed"] if "fan_speed" in sensor else 0,
+                sensor_data["gpu"][f"{sensor['name']} (GPU {sensor['gpu_id']})"] = {
+                    "temperature": sensor.get("temperature", 0),
+                    "mem": sensor.get("mem", 0),
+                    "proc": sensor.get("proc", 0),
+                    "fan_speed": sensor.get("fan_speed", 0),
+                }
+        if data := self.data.get("diskio"):
+            sensor_data["diskio"] = {}
+            for disk in data:
+                time_since_update = disk["time_since_update"]
+                sensor_data["diskio"][disk["disk_name"]] = {
+                    "read": round(disk["read_bytes"] / time_since_update),
+                    "write": round(disk["write_bytes"] / time_since_update),
                 }
         return sensor_data
```

### Comparing `glances_api-0.5.1/pyproject.toml` & `glances_api-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glances_api"
-version = "0.5.1"
+version = "0.6.0"
 description = "Python API for interacting with Glances"
 authors = ["Fabian Affolter <fabian@affolter-engineering.ch>"]
 homepage = "https://github.com/home-assistant-ecosystem/python-glances-api"
 repository = "https://github.com/home-assistant-ecosystem/python-glances-api/releases"
 readme = "README.rst"
 license = "MIT"
 classifiers = [
@@ -18,16 +18,16 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = ">=0.23,<1"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3"
-pytest = "^7.3.0"
+black = "^24.3"
+pytest = "^8"
 pytest-httpx = ">0.15,<1"
 pytest-asyncio = "^0.16.0"
 isort = "^5.10.0"
 mypy = "^0.971"
 
 [tool.mypy]
 check_untyped_defs = true
```

### Comparing `glances_api-0.5.1/PKG-INFO` & `glances_api-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glances_api
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python API for interacting with Glances
 Home-page: https://github.com/home-assistant-ecosystem/python-glances-api
 License: MIT
 Author: Fabian Affolter
 Author-email: fabian@affolter-engineering.ch
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

