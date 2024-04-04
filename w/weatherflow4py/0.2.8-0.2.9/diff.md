# Comparing `tmp/weatherflow4py-0.2.8.tar.gz` & `tmp/weatherflow4py-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherflow4py-0.2.8.tar", max compression
+gzip compressed data, was "weatherflow4py-0.2.9.tar", max compression
```

## Comparing `weatherflow4py-0.2.8.tar` & `weatherflow4py-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1066 2024-03-08 20:55:35.138633 weatherflow4py-0.2.8/LICENSE
--rw-r--r--   0        0        0      452 2024-03-08 20:55:35.138633 weatherflow4py-0.2.8/README.md
--rw-r--r--   0        0        0      991 2024-03-08 20:55:44.326667 weatherflow4py-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/__init__.py
--rw-r--r--   0        0        0     5698 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/api.py
--rw-r--r--   0        0        0      115 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/exceptions.py
--rw-r--r--   0        0        0       37 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/__init__.py
--rw-r--r--   0        0        0       25 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/rest/__init__.py
--rw-r--r--   0        0        0     1434 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/rest/device.py
--rw-r--r--   0        0        0     7902 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/rest/forecast.py
--rw-r--r--   0        0        0     4420 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/rest/observation.py
--rw-r--r--   0        0        0     2418 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/rest/station.py
--rw-r--r--   0        0        0      897 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/rest/unified.py
--rw-r--r--   0        0        0       31 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/ws/__init__.py
--rw-r--r--   0        0        0      610 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/ws/custom_types.py
--rw-r--r--   0        0        0     8503 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/ws/obs.py
--rw-r--r--   0        0        0      528 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/ws/types.py
--rw-r--r--   0        0        0     2407 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/ws/websocket_request.py
--rw-r--r--   0        0        0     4107 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/models/ws/websocket_response.py
--rw-r--r--   0        0        0     8258 2024-03-08 20:55:35.142633 weatherflow4py-0.2.8/weatherflow4py/ws.py
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 weatherflow4py-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-08 20:59:56.500386 weatherflow4py-0.2.9/LICENSE
+-rw-r--r--   0        0        0      452 2024-03-08 20:59:56.500386 weatherflow4py-0.2.9/README.md
+-rw-r--r--   0        0        0      991 2024-03-08 21:00:06.036379 weatherflow4py-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/__init__.py
+-rw-r--r--   0        0        0     5731 2024-03-08 21:00:06.036379 weatherflow4py-0.2.9/weatherflow4py/api.py
+-rw-r--r--   0        0        0       53 2024-03-08 21:00:06.036379 weatherflow4py-0.2.9/weatherflow4py/const.py
+-rw-r--r--   0        0        0      115 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/exceptions.py
+-rw-r--r--   0        0        0       37 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/__init__.py
+-rw-r--r--   0        0        0       25 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/rest/__init__.py
+-rw-r--r--   0        0        0     1434 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/rest/device.py
+-rw-r--r--   0        0        0     7902 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/rest/forecast.py
+-rw-r--r--   0        0        0     4420 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/rest/observation.py
+-rw-r--r--   0        0        0     2418 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/rest/station.py
+-rw-r--r--   0        0        0      897 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/rest/unified.py
+-rw-r--r--   0        0        0       31 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/ws/__init__.py
+-rw-r--r--   0        0        0      610 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/ws/custom_types.py
+-rw-r--r--   0        0        0     8503 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/ws/obs.py
+-rw-r--r--   0        0        0      528 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/ws/types.py
+-rw-r--r--   0        0        0     2407 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/ws/websocket_request.py
+-rw-r--r--   0        0        0     4107 2024-03-08 20:59:56.504386 weatherflow4py-0.2.9/weatherflow4py/models/ws/websocket_response.py
+-rw-r--r--   0        0        0     8195 2024-03-08 21:00:06.036379 weatherflow4py-0.2.9/weatherflow4py/ws.py
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 weatherflow4py-0.2.9/PKG-INFO
```

### Comparing `weatherflow4py-0.2.8/LICENSE` & `weatherflow4py-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/pyproject.toml` & `weatherflow4py-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weatherflow4py"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["Jeef <jeeftor@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `weatherflow4py-0.2.8/weatherflow4py/api.py` & `weatherflow4py-0.2.9/weatherflow4py/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from weatherflow4py.exceptions import TokenError
 from weatherflow4py.models.rest.device import DeviceObservationTempestREST
 from weatherflow4py.models.rest.forecast import WeatherData
 from weatherflow4py.models.rest.observation import StationObservation
 from weatherflow4py.models.rest.station import StationsResponse
 from weatherflow4py.models.rest.unified import WeatherFlowData
+from .const import LOGGER
 
 
 class WeatherFlowRestAPI:
     """Our REST rate limits are not connected to our web socket rate limits. For REST you can make 100 requests per
     minute. There is some burst capacity built into the system, but the general rule of thumb it to keep the number
     of REST requests per user to under 100 per minute."""
 
@@ -41,15 +42,15 @@
         async with self.session.get(url, params=full_params) as response:
             response.raise_for_status()
             data = await response.text()
 
         try:
             return response_model.from_json(data) if response_model else None
         except Exception as e:
-            print(
+            LOGGER.error(
                 f"An error occurred while converting data to response model: {str(e)}"
             )
             return None
 
     async def async_get_stations(self) -> StationsResponse:
         """
         Gets station data.
```

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/rest/device.py` & `weatherflow4py-0.2.9/weatherflow4py/models/rest/device.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/rest/forecast.py` & `weatherflow4py-0.2.9/weatherflow4py/models/rest/forecast.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/rest/observation.py` & `weatherflow4py-0.2.9/weatherflow4py/models/rest/observation.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/rest/station.py` & `weatherflow4py-0.2.9/weatherflow4py/models/rest/station.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/rest/unified.py` & `weatherflow4py-0.2.9/weatherflow4py/models/rest/unified.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/ws/custom_types.py` & `weatherflow4py-0.2.9/weatherflow4py/models/ws/custom_types.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/ws/obs.py` & `weatherflow4py-0.2.9/weatherflow4py/models/ws/obs.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/ws/types.py` & `weatherflow4py-0.2.9/weatherflow4py/models/ws/types.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/ws/websocket_request.py` & `weatherflow4py-0.2.9/weatherflow4py/models/ws/websocket_request.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/models/ws/websocket_response.py` & `weatherflow4py-0.2.9/weatherflow4py/models/ws/websocket_response.py`

 * *Files identical despite different names*

### Comparing `weatherflow4py-0.2.8/weatherflow4py/ws.py` & `weatherflow4py-0.2.9/weatherflow4py/ws.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import time
 from collections.abc import Callable
 
 import asyncio
 import websockets
 import json
 
@@ -14,27 +13,28 @@
 )
 from weatherflow4py.models.ws.websocket_response import (
     WebsocketResponseBuilder,
     ObservationTempestWS,
     RapidWindWS,
 )
 
+from .const import LOGGER
+
 
 class WeatherFlowWebsocketAPI:
     def __init__(self, device_id: str, access_token: str):
         self.device_id = device_id
         self.uri = f"wss://ws.weatherflow.com/swd/data?token={access_token}"
         self.websocket = None
         self.messages = {}
         self.is_listening = False
         self.listen_task = None  # To keep track of the listening task
         self.callbacks = {}
 
-        self.logger = logging.getLogger(__name__)
-        self.logger.debug("WebsocketAPI initialized with URI: " + self.uri)
+        LOGGER.debug("WebsocketAPI initialized with URI: " + self.uri)
 
     def _register_callback(
         self, message_type: EventType, callback: Callable[[str], None]
     ):
         """Register a callback for a specific message type"""
         self.callbacks[message_type.value] = callback
 
@@ -145,43 +145,43 @@
             last_observation_epoch = obs.epoch
             time_difference = current_epoch - last_observation_epoch
             return time_difference
         return None
 
     async def send_message(self, message_type: WebsocketRequest):
         message = message_type.json
-        self.logger.debug(f"Sending message: {message}")
+        LOGGER.debug(f"Sending message: {message}")
         await self._send(message)
 
     async def connect(self):
         self.websocket = await websockets.connect(self.uri)
         # Run the listen method in the background and name the task for easier debugging
         self.listen_task = asyncio.create_task(
             self.listen(), name="WebSocketListenTask"
         )
 
     async def listen(self):
         self.is_listening = True
         try:
             async for message in self.websocket:
-                self.logger.debug(f"Received message: {message}")
+                LOGGER.debug(f"Received message: {message}")
                 data = json.loads(message)
                 try:
                     response = WebsocketResponseBuilder.build_response(data)
                     self.messages[data["type"]] = response
 
                     if data["type"] in self.callbacks:
                         if asyncio.iscoroutinefunction(self.callbacks[data["type"]]):
-                            self.logger.debug(
+                            LOGGER.debug(
                                 f"Calling ASYNC callback for message type: {data['type']}"
                             )
                             # If it is, use 'await' to call it
                             await self.callbacks[data["type"]](response)
                         else:
-                            self.logger.debug(
+                            LOGGER.debug(
                                 f"Calling SYNC callback for message type: {data['type']}"
                             )
                             # If it's not, call it normally
                             self.callbacks[data["type"]](response)
 
                 except ValueError:
                     if EventType.INVALID.value in self.callbacks:
```

### Comparing `weatherflow4py-0.2.8/PKG-INFO` & `weatherflow4py-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weatherflow4py
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 License: MIT
 Author: Jeef
 Author-email: jeeftor@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

