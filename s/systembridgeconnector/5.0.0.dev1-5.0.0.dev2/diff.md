# Comparing `tmp/systembridgeconnector-5.0.0.dev1.tar.gz` & `tmp/systembridgeconnector-5.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgeconnector-5.0.0.dev1.tar", last modified: Thu Apr  4 00:15:18 2024, max compression
+gzip compressed data, was "systembridgeconnector-5.0.0.dev2.tar", last modified: Thu Apr  4 01:18:01 2024, max compression
```

## Comparing `systembridgeconnector-5.0.0.dev1.tar` & `systembridgeconnector-5.0.0.dev2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:15:18.713850 systembridgeconnector-5.0.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 00:15:18.713850 systembridgeconnector-5.0.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:15:18.713850 systembridgeconnector-5.0.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:15:18.709850 systembridgeconnector-5.0.0.dev1/systembridgeconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:15:18.713850 systembridgeconnector-5.0.0.dev1/systembridgeconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 00:15:18.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-04 00:15:18.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:15:18.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 00:15:18.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 00:15:18.000000 systembridgeconnector-5.0.0.dev1/systembridgeconnector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:15:18.709850 systembridgeconnector-5.0.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/tests/test__version.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16794 2024-04-04 00:14:53.000000 systembridgeconnector-5.0.0.dev1/tests/test_websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:18:01.664317 systembridgeconnector-5.0.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 01:18:01.664317 systembridgeconnector-5.0.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:18:01.664317 systembridgeconnector-5.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:18:01.664317 systembridgeconnector-5.0.0.dev2/systembridgeconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22065 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:18:01.664317 systembridgeconnector-5.0.0.dev2/systembridgeconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 01:18:01.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 01:18:01.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:18:01.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 01:18:01.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 01:18:01.000000 systembridgeconnector-5.0.0.dev2/systembridgeconnector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:18:01.664317 systembridgeconnector-5.0.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/tests/test__version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16489 2024-04-04 01:17:41.000000 systembridgeconnector-5.0.0.dev2/tests/test_websocket_client.py
```

### Comparing `systembridgeconnector-5.0.0.dev1/LICENSE` & `systembridgeconnector-5.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/PKG-INFO` & `systembridgeconnector-5.0.0.dev2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: systembridgeconnector
-Version: 5.0.0.dev1
+Version: 5.0.0.dev2
 Summary: System Bridge Connector
 Home-page: https://github.com/timmo001/system-bridge-connector
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8.5; python_version < "3.12"
 Requires-Dist: aiohttp>=3.9.0b0; python_version >= "3.12"
 Requires-Dist: incremental>=22.10.0
 Requires-Dist: packaging>=24.0
-Requires-Dist: systembridgemodels>=4.0.4
+Requires-Dist: systembridgemodels>=4.1.0
 
 # System Bridge - Connector
 
 This is the connector package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
 
 Used in the System Bridge [Home Assistant](https://www.home-assistant.io/integrations/system_bridge) integration.
```

### Comparing `systembridgeconnector-5.0.0.dev1/pyproject.toml` & `systembridgeconnector-5.0.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/setup.py` & `systembridgeconnector-5.0.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/systembridgeconnector/exceptions.py` & `systembridgeconnector-5.0.0.dev2/systembridgeconnector/exceptions.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/systembridgeconnector/http_client.py` & `systembridgeconnector-5.0.0.dev2/systembridgeconnector/http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/systembridgeconnector/version.py` & `systembridgeconnector-5.0.0.dev2/systembridgeconnector/version.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/systembridgeconnector/websocket_client.py` & `systembridgeconnector-5.0.0.dev2/systembridgeconnector/websocket_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dataclasses import asdict
 import socket
 from typing import Any
 from uuid import uuid4
 
 import aiohttp
 
-from systembridgemodels.const import MODEL_MAP, MODEL_RESPONSE
+from systembridgemodels.const import MODEL_MAP, Model
 from systembridgemodels.keyboard_key import KeyboardKey
 from systembridgemodels.keyboard_text import KeyboardText
 from systembridgemodels.media_control import MediaControl
 from systembridgemodels.media_directories import MediaDirectory
 from systembridgemodels.media_files import MediaFile, MediaFiles
 from systembridgemodels.media_get_file import MediaGetFile
 from systembridgemodels.media_get_files import MediaGetFiles
@@ -24,59 +24,15 @@
 from systembridgemodels.open_path import OpenPath
 from systembridgemodels.open_url import OpenUrl
 from systembridgemodels.request import Request
 from systembridgemodels.response import Response
 from systembridgemodels.update import Update
 
 from .base import Base
-from .const import (
-    EVENT_DATA,
-    EVENT_ID,
-    EVENT_MESSAGE,
-    EVENT_MODULE,
-    EVENT_SUBTYPE,
-    EVENT_TYPE,
-    SUBTYPE_BAD_TOKEN,
-    SUBTYPE_LISTENER_ALREADY_REGISTERED,
-    TYPE_APPLICATION_UPDATE,
-    TYPE_DATA_GET,
-    TYPE_DATA_LISTENER_REGISTERED,
-    TYPE_DATA_UPDATE,
-    TYPE_DIRECTORIES,
-    TYPE_ERROR,
-    TYPE_EXIT_APPLICATION,
-    TYPE_FILE,
-    TYPE_FILES,
-    TYPE_GET_DATA,
-    TYPE_GET_DIRECTORIES,
-    TYPE_GET_FILE,
-    TYPE_GET_FILES,
-    TYPE_KEYBOARD_KEY_PRESSED,
-    TYPE_KEYBOARD_KEYPRESS,
-    TYPE_KEYBOARD_TEXT,
-    TYPE_KEYBOARD_TEXT_SENT,
-    TYPE_MEDIA_CONTROL,
-    TYPE_NOTIFICATION,
-    TYPE_NOTIFICATION_SENT,
-    TYPE_OPEN,
-    TYPE_OPENED,
-    TYPE_POWER_HIBERNATE,
-    TYPE_POWER_HIBERNATING,
-    TYPE_POWER_LOCK,
-    TYPE_POWER_LOCKING,
-    TYPE_POWER_LOGGINGOUT,
-    TYPE_POWER_LOGOUT,
-    TYPE_POWER_RESTART,
-    TYPE_POWER_RESTARTING,
-    TYPE_POWER_SHUTDOWN,
-    TYPE_POWER_SHUTTINGDOWN,
-    TYPE_POWER_SLEEP,
-    TYPE_POWER_SLEEPING,
-    TYPE_REGISTER_DATA_LISTENER,
-)
+from .const import EventKey, EventSubType, EventType
 from .exceptions import (
     AuthenticationException,
     BadMessageException,
     ConnectionClosedException,
     ConnectionErrorException,
     DataMissingException,
 )
@@ -147,15 +103,15 @@
             )
             try:
                 return await self._wait_for_future(future)
             except asyncio.TimeoutError:
                 self._logger.error("Timeout waiting for future: %s", request.id)
                 return Response(
                     id=request.id,
-                    type=TYPE_ERROR,
+                    type=EventType.ERROR,
                     subtype="TIMEOUT",
                     message="Timeout waiting for response",
                     data={},
                 )
             finally:
                 self._responses.pop(request.id)
 
@@ -205,28 +161,28 @@
         self,
         model: Update,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Update application."""
         self._logger.info("Updating application")
         return await self._send_message(
-            TYPE_APPLICATION_UPDATE,
+            EventType.APPLICATION_UPDATE,
             request_id,
             asdict(model),
             wait_for_response=False,
         )
 
     async def exit_backend(
         self,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Exit backend."""
         self._logger.info("Exiting backend")
         return await self._send_message(
-            TYPE_EXIT_APPLICATION,
+            EventType.EXIT_APPLICATION,
             request_id,
             {},
             wait_for_response=False,
         )
 
     async def get_data(
         self,
@@ -252,19 +208,19 @@
                 callback=handle_module,
                 accept_other_types=False,
             ),
             name="Get data WebSocket Listener",
         )
 
         await self._send_message(
-            TYPE_GET_DATA,
+            EventType.GET_DATA,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_DATA_GET,
+            response_type=EventType.DATA_GET,
         )
 
         # Wait for all data modules to be set
         try:
             async with asyncio.timeout(timeout):
                 while not all(
                     getattr(modules_data, module_name) is not None
@@ -285,19 +241,19 @@
     async def get_directories(
         self,
         request_id: str = uuid4().hex,
     ) -> list[MediaDirectory]:
         """Get directories."""
         self._logger.info("Getting directories..")
         response = await self._send_message(
-            TYPE_GET_DIRECTORIES,
+            EventType.GET_DIRECTORIES,
             request_id,
             {},
             wait_for_response=True,
-            response_type=TYPE_DIRECTORIES,
+            response_type=EventType.DIRECTORIES,
         )
 
         return (
             [MediaDirectory(**directory) for directory in response.data]
             if response.data is not None and isinstance(response.data, list)
             else []
         )
@@ -306,19 +262,19 @@
         self,
         model: MediaGetFiles,
         request_id: str = uuid4().hex,
     ) -> MediaFiles:
         """Get files."""
         self._logger.info("Getting files: %s", model)
         response = await self._send_message(
-            TYPE_GET_FILES,
+            EventType.GET_FILES,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_FILES,
+            response_type=EventType.FILES,
         )
 
         return (
             MediaFiles(
                 files=[MediaFile(**file) for file in response.data],
                 path=model.path if model.path is not None else "",
             )
@@ -333,19 +289,19 @@
         self,
         model: MediaGetFile,
         request_id: str = uuid4().hex,
     ) -> MediaFile | None:
         """Get files."""
         self._logger.info("Getting file: %s", model)
         response = await self._send_message(
-            TYPE_GET_FILE,
+            EventType.GET_FILE,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_FILE,
+            response_type=EventType.FILE,
         )
 
         return (
             MediaFile(**response.data)
             if response.data is not None and isinstance(response.data, dict)
             else None
         )
@@ -354,307 +310,318 @@
         self,
         model: RegisterDataListener,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Register data listener."""
         self._logger.info("Registering data listener: %s", model)
         return await self._send_message(
-            TYPE_REGISTER_DATA_LISTENER,
+            EventType.REGISTER_DATA_LISTENER,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_DATA_LISTENER_REGISTERED,
+            response_type=EventType.DATA_LISTENER_REGISTERED,
         )
 
     async def keyboard_keypress(
         self,
         model: KeyboardKey,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Keyboard keypress."""
         self._logger.info("Press key: %s", model)
         return await self._send_message(
-            TYPE_KEYBOARD_KEYPRESS,
+            EventType.KEYBOARD_KEYPRESS,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_KEYBOARD_KEY_PRESSED,
+            response_type=EventType.KEYBOARD_KEY_PRESSED,
         )
 
     async def keyboard_text(
         self,
         model: KeyboardText,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Keyboard keypress."""
         self._logger.info("Enter text: %s", model)
         return await self._send_message(
-            TYPE_KEYBOARD_TEXT,
+            EventType.KEYBOARD_TEXT,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_KEYBOARD_TEXT_SENT,
+            response_type=EventType.KEYBOARD_TEXT_SENT,
         )
 
     async def media_control(
         self,
         model: MediaControl,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Media control."""
         self._logger.info("Media control: %s", model)
         return await self._send_message(
-            TYPE_MEDIA_CONTROL,
+            EventType.MEDIA_CONTROL,
             request_id,
             asdict(model),
             wait_for_response=False,
         )
 
     async def send_notification(
         self,
         model: Notification,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Send notification."""
         self._logger.info("Send notification: %s", model)
         return await self._send_message(
-            TYPE_NOTIFICATION,
+            EventType.NOTIFICATION,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_NOTIFICATION_SENT,
+            response_type=EventType.NOTIFICATION_SENT,
         )
 
     async def open_path(
         self,
         model: OpenPath,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Open path."""
         self._logger.info("Opening path: %s", model)
         return await self._send_message(
-            TYPE_OPEN,
+            EventType.OPEN,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_OPENED,
+            response_type=EventType.OPENED,
         )
 
     async def open_url(
         self,
         model: OpenUrl,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Open url."""
         self._logger.info("Opening URL: %s", model)
         return await self._send_message(
-            TYPE_OPEN,
+            EventType.OPEN,
             request_id,
             asdict(model),
             wait_for_response=True,
-            response_type=TYPE_OPENED,
+            response_type=EventType.OPENED,
         )
 
     async def power_sleep(
         self,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Power sleep."""
         self._logger.info("Power sleep")
         return await self._send_message(
-            TYPE_POWER_SLEEP,
+            EventType.POWER_SLEEP,
             request_id,
             {},
             wait_for_response=True,
-            response_type=TYPE_POWER_SLEEPING,
+            response_type=EventType.POWER_SLEEPING,
         )
 
     async def power_hibernate(
         self,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Power hibernate."""
         self._logger.info("Power hibernate")
         return await self._send_message(
-            TYPE_POWER_HIBERNATE,
+            EventType.POWER_HIBERNATE,
             request_id,
             {},
             wait_for_response=True,
-            response_type=TYPE_POWER_HIBERNATING,
+            response_type=EventType.POWER_HIBERNATING,
         )
 
     async def power_restart(
         self,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Power restart."""
         self._logger.info("Power restart")
         return await self._send_message(
-            TYPE_POWER_RESTART,
+            EventType.POWER_RESTART,
             request_id,
             {},
             wait_for_response=True,
-            response_type=TYPE_POWER_RESTARTING,
+            response_type=EventType.POWER_RESTARTING,
         )
 
     async def power_shutdown(
         self,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Power shutdown."""
         self._logger.info("Power shutdown")
         return await self._send_message(
-            TYPE_POWER_SHUTDOWN,
+            EventType.POWER_SHUTDOWN,
             request_id,
             {},
             wait_for_response=True,
-            response_type=TYPE_POWER_SHUTTINGDOWN,
+            response_type=EventType.POWER_SHUTTINGDOWN,
         )
 
     async def power_lock(
         self,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Power lock."""
         self._logger.info("Power lock")
         return await self._send_message(
-            TYPE_POWER_LOCK,
+            EventType.POWER_LOCK,
             request_id,
             {},
             wait_for_response=True,
-            response_type=TYPE_POWER_LOCKING,
+            response_type=EventType.POWER_LOCKING,
         )
 
     async def power_logout(
         self,
         request_id: str = uuid4().hex,
     ) -> Response:
         """Power logout."""
         self._logger.info("Power logout")
         return await self._send_message(
-            TYPE_POWER_LOGOUT,
+            EventType.POWER_LOGOUT,
             request_id,
             {},
             wait_for_response=True,
-            response_type=TYPE_POWER_LOGGINGOUT,
+            response_type=EventType.POWER_LOGGINGOUT,
         )
 
     async def listen(
         self,
         callback: Callable[[str, Any], Awaitable[None]] | None = None,
         accept_other_types: bool = False,
         name: str = "WebSocket Client",
     ) -> None:
         """Listen for messages and map to modules."""
 
         async def _callback_message(message: dict) -> None:
             """Message Callback."""
-            self._logger.debug("[%s] New message: %s", name, message[EVENT_TYPE])
+            self._logger.debug("[%s] New message: %s", name, message[EventKey.TYPE])
 
             if (
-                message.get(EVENT_ID) is not None
-                and (response_tuple := self._responses.get(message[EVENT_ID]))
+                message.get(EventKey.ID) is not None
+                and (response_tuple := self._responses.get(message[EventKey.ID]))
                 is not None
             ):
                 future, response_type = response_tuple
-                if response_type is not None and response_type == message[EVENT_TYPE]:
+                if (
+                    response_type is not None
+                    and response_type == message[EventKey.TYPE]
+                ):
                     response = Response(**message)
 
                     if (
-                        response.type == TYPE_DATA_UPDATE
+                        response.type == EventType.DATA_UPDATE
                         and response.module is not None
-                        and message[EVENT_DATA] is not None
+                        and message[EventKey.DATA] is not None
                     ):
                         # Find model from module
-                        model = MODEL_MAP.get(message[EVENT_MODULE])
-                        if model is None:
+                        model_cls = MODEL_MAP.get(message[EventKey.MODULE])
+                        if model_cls is None:
                             self._logger.warning(
-                                "[%s] Unknown model: %s", name, message[EVENT_MODULE]
+                                "[%s] Unknown model: %s", name, message[EventKey.MODULE]
                             )
                         else:
                             self._logger.debug(
-                                "[%s] Mapping data to model: %s", name, model.__name__
+                                "[%s] Mapping data to model: %s",
+                                name,
+                                model_cls.__name__,
                             )
-                            if isinstance(message[EVENT_DATA], list):
+                            if isinstance(message[EventKey.DATA], list):
                                 response.data = [
-                                    model(**data) for data in message[EVENT_DATA]
+                                    model_cls(**data) for data in message[EventKey.DATA]
                                 ]
                             else:
-                                response.data = model(**message[EVENT_DATA])
+                                response.data = model_cls(**message[EventKey.DATA])
 
                     self._logger.info("[%s] Response: %s", name, response)
 
                     try:
                         future.set_result(response)
                     except asyncio.InvalidStateError:
                         self._logger.debug(
                             "[%s] Future already set for response ID: %s",
                             name,
-                            message[EVENT_ID],
+                            message[EventKey.ID],
                         )
 
-            if message[EVENT_TYPE] == TYPE_ERROR:
-                if message[EVENT_SUBTYPE] == SUBTYPE_LISTENER_ALREADY_REGISTERED:
+            if message[EventKey.TYPE] == EventType.ERROR:
+                if (
+                    message[EventKey.SUBTYPE]
+                    == EventSubType.LISTENER_ALREADY_REGISTERED
+                ):
                     self._logger.debug(
                         "[%s]: %s",
                         name,
                         message,
                     )
                 elif (
-                    message[EVENT_SUBTYPE] == SUBTYPE_BAD_TOKEN
-                    or message[EVENT_SUBTYPE] == "BAD_API_KEY"
+                    message[EventKey.SUBTYPE] == EventSubType.BAD_TOKEN
+                    or message[EventKey.SUBTYPE] == "BAD_API_KEY"
                 ):
                     self._logger.error(
                         "[%s]: %s",
                         name,
                         message,
                     )
-                    raise AuthenticationException(message[EVENT_MESSAGE])
+                    raise AuthenticationException(message[EventKey.MESSAGE])
                 else:
                     self._logger.warning(
                         "[%s]: %s",
                         name,
                         message,
                     )
             elif (
-                message[EVENT_TYPE] == TYPE_DATA_UPDATE
-                and message[EVENT_DATA] is not None
+                message[EventKey.TYPE] == EventType.DATA_UPDATE
+                and message[EventKey.DATA] is not None
             ):
                 self._logger.debug(
                     "[%s] New data for: %s\n%s",
                     name,
-                    message[EVENT_MODULE],
-                    message[EVENT_DATA],
+                    message[EventKey.MODULE],
+                    message[EventKey.DATA],
                 )
-                model = MODEL_MAP.get(message[EVENT_MODULE])
-                if model is None:
+                model_cls = MODEL_MAP.get(message[EventKey.MODULE])
+                if model_cls is None:
                     self._logger.warning(
                         "[%s] Unknown model: %s",
                         name,
-                        message[EVENT_MODULE],
+                        message[EventKey.MODULE],
                     )
                 elif callback is not None:
                     await callback(
-                        message[EVENT_MODULE],
-                        [model(**data) for data in message[EVENT_DATA]]
-                        if isinstance(message[EVENT_DATA], list)
-                        else model(**message[EVENT_DATA]),
+                        message[EventKey.MODULE],
+                        [model_cls(**data) for data in message[EventKey.DATA]]
+                        if isinstance(message[EventKey.DATA], list)
+                        else model_cls(**message[EventKey.DATA]),
                     )
             else:
                 self._logger.debug(
                     "[%s] Other message: %s",
                     name,
-                    message[EVENT_TYPE],
+                    message[EventKey.TYPE],
                 )
                 if accept_other_types:
-                    model = MODEL_MAP.get(EVENT_TYPE, MODEL_MAP[MODEL_RESPONSE])
-                    if model is not None and callback is not None:
+                    model_cls = MODEL_MAP.get(
+                        message[EventKey.TYPE],
+                        Model.RESPONSE,
+                    )
+                    if model_cls is not None and callback is not None:
                         await callback(
-                            message[EVENT_TYPE],
-                            model(**message),
+                            message[EventKey.TYPE],
+                            model_cls(**message),
                         )
 
         await self.listen_for_messages(
             callback=_callback_message,
             name=name,
         )
 
@@ -697,16 +664,16 @@
             aiohttp.WSMsgType.CLOSING,
         ):
             raise ConnectionClosedException("Connection closed to server")
 
         if message.type == aiohttp.WSMsgType.TEXT:
             message_json = message.json()
 
-            if message_json[EVENT_TYPE] == TYPE_ERROR and (
-                message_json[EVENT_SUBTYPE] == SUBTYPE_BAD_TOKEN
-                or message_json[EVENT_SUBTYPE] == "BAD_API_KEY"
+            if message_json[EventKey.TYPE] == EventType.ERROR and (
+                message_json[EventKey.SUBTYPE] == EventSubType.BAD_TOKEN
+                or message_json[EventKey.SUBTYPE] == "BAD_API_KEY"
             ):
-                raise AuthenticationException(message_json[EVENT_MESSAGE])
+                raise AuthenticationException(message_json[EventKey.MESSAGE])
 
             return message_json
 
         raise BadMessageException(f"Unknown message type: {message.type}")
```

### Comparing `systembridgeconnector-5.0.0.dev1/systembridgeconnector.egg-info/PKG-INFO` & `systembridgeconnector-5.0.0.dev2/systembridgeconnector.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: systembridgeconnector
-Version: 5.0.0.dev1
+Version: 5.0.0.dev2
 Summary: System Bridge Connector
 Home-page: https://github.com/timmo001/system-bridge-connector
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.8.5; python_version < "3.12"
 Requires-Dist: aiohttp>=3.9.0b0; python_version >= "3.12"
 Requires-Dist: incremental>=22.10.0
 Requires-Dist: packaging>=24.0
-Requires-Dist: systembridgemodels>=4.0.4
+Requires-Dist: systembridgemodels>=4.1.0
 
 # System Bridge - Connector
 
 This is the connector package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
 
 Used in the System Bridge [Home Assistant](https://www.home-assistant.io/integrations/system_bridge) integration.
```

### Comparing `systembridgeconnector-5.0.0.dev1/systembridgeconnector.egg-info/SOURCES.txt` & `systembridgeconnector-5.0.0.dev2/systembridgeconnector.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,12 +13,11 @@
 systembridgeconnector.egg-info/PKG-INFO
 systembridgeconnector.egg-info/SOURCES.txt
 systembridgeconnector.egg-info/dependency_links.txt
 systembridgeconnector.egg-info/requires.txt
 systembridgeconnector.egg-info/top_level.txt
 tests/test__version.py
 tests/test_base.py
-tests/test_const.py
 tests/test_exceptions.py
 tests/test_http_client.py
 tests/test_version.py
 tests/test_websocket_client.py
```

### Comparing `systembridgeconnector-5.0.0.dev1/tests/test_exceptions.py` & `systembridgeconnector-5.0.0.dev2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/tests/test_http_client.py` & `systembridgeconnector-5.0.0.dev2/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/tests/test_version.py` & `systembridgeconnector-5.0.0.dev2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `systembridgeconnector-5.0.0.dev1/tests/test_websocket_client.py` & `systembridgeconnector-5.0.0.dev2/tests/test_websocket_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,44 +4,31 @@
 from typing import Any
 from unittest.mock import patch
 
 import aiohttp
 import pytest
 from syrupy.assertion import SnapshotAssertion
 
-from systembridgeconnector.const import (
-    EVENT_MODULES,
-    TYPE_DATA_GET,
-    TYPE_DATA_LISTENER_REGISTERED,
-    TYPE_DIRECTORIES,
-    TYPE_FILE,
-    TYPE_FILES,
-    TYPE_KEYBOARD_KEY_PRESSED,
-    TYPE_KEYBOARD_TEXT_SENT,
-    TYPE_NOTIFICATION_SENT,
-    TYPE_OPENED,
-    TYPE_POWER_HIBERNATING,
-    TYPE_POWER_LOCKING,
-    TYPE_POWER_LOGGINGOUT,
-    TYPE_POWER_RESTARTING,
-    TYPE_POWER_SHUTTINGDOWN,
-    TYPE_POWER_SLEEPING,
-)
+from systembridgeconnector.const import EventKey, EventType
 from systembridgeconnector.exceptions import (
     ConnectionClosedException,
     ConnectionErrorException,
 )
 from systembridgeconnector.websocket_client import WebSocketClient
-from systembridgemodels.const import MODEL_SYSTEM
 from systembridgemodels.keyboard_key import KeyboardKey
 from systembridgemodels.keyboard_text import KeyboardText
 from systembridgemodels.media_control import MediaControl
 from systembridgemodels.media_get_file import MediaGetFile
 from systembridgemodels.media_get_files import MediaGetFiles
-from systembridgemodels.modules import GetData, ModulesData, RegisterDataListener
+from systembridgemodels.modules import (
+    GetData,
+    Module,
+    ModulesData,
+    RegisterDataListener,
+)
 from systembridgemodels.notification import Notification
 from systembridgemodels.open_path import OpenPath
 from systembridgemodels.open_url import OpenUrl
 from systembridgemodels.response import Response
 from systembridgemodels.update import Update
 
 from . import API_HOST, API_PORT, REQUEST_ID, TOKEN, WebSocketGenerator
@@ -125,15 +112,15 @@
 
     with patch(
         "systembridgeconnector.websocket_client.WebSocketClient._wait_for_future",
         side_effect=asyncio.TimeoutError,
     ):
         response = await websocket_client.get_data(
             GetData(
-                modules=[MODEL_SYSTEM],
+                modules=[Module.SYSTEM],
             ),
             request_id=REQUEST_ID,
         )
 
     assert response == snapshot(
         name="websocket_client_timeout",
     )
@@ -190,22 +177,22 @@
     ws_client: WebSocketGenerator,
 ):
     """Test get data."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_DATA_GET,
-            data={EVENT_MODULES: [MODEL_SYSTEM]},
+            type=EventType.DATA_GET,
+            data={EventKey.MODULES: [Module.SYSTEM]},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.get_data(
         GetData(
-            modules=[MODEL_SYSTEM],
+            modules=[Module.SYSTEM],
         ),
         request_id=REQUEST_ID,
     )
     assert response == snapshot(
         name="websocket_client_get_data",
     )
 
@@ -216,15 +203,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test get directories."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_DIRECTORIES,
+            type=EventType.DIRECTORIES,
             data=[{"key": "documents", "path": "/documents"}],
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.get_directories(
         request_id=REQUEST_ID,
     )
@@ -239,15 +226,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test get files."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_FILES,
+            type=EventType.FILES,
             data={
                 "files": [
                     {
                         "name": "test",
                         "path": "path/to",
                         "fullpath": "path/to/test",
                         "size": 0,
@@ -283,15 +270,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test get file."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_FILE,
+            type=EventType.FILE,
             data={
                 "name": "test",
                 "path": "path/to",
                 "fullpath": "path/to/test",
                 "size": 0,
                 "last_accessed": 0,
                 "created": 0,
@@ -322,22 +309,22 @@
     ws_client: WebSocketGenerator,
 ):
     """Test register data listener."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_DATA_LISTENER_REGISTERED,
-            data={EVENT_MODULES: [MODEL_SYSTEM]},
+            type=EventType.DATA_LISTENER_REGISTERED,
+            data={EventKey.MODULES: [Module.SYSTEM]},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.register_data_listener(
         RegisterDataListener(
-            modules=[MODEL_SYSTEM],
+            modules=[Module.SYSTEM],
         ),
         request_id=REQUEST_ID,
     )
     assert response == snapshot(
         name="websocket_client_register_data_listener",
     )
 
@@ -348,15 +335,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test keyboard keypress."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_KEYBOARD_KEY_PRESSED,
+            type=EventType.KEYBOARD_KEY_PRESSED,
             data={"key": "a"},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.keyboard_keypress(
         KeyboardKey(
             key="a",
@@ -374,15 +361,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test keyboard text."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_KEYBOARD_TEXT_SENT,
+            type=EventType.KEYBOARD_TEXT_SENT,
             data={"text": "test"},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.keyboard_text(
         KeyboardText(
             text="test",
@@ -426,15 +413,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test send notification."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_NOTIFICATION_SENT,
+            type=EventType.NOTIFICATION_SENT,
             data={"title": "test", "message": "test"},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.send_notification(
         Notification(
             title="test",
@@ -453,15 +440,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test open path."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_OPENED,
+            type=EventType.OPENED,
             data={"path": "test"},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.open_path(
         OpenPath(
             path="test",
@@ -479,15 +466,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test open url."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_OPENED,
+            type=EventType.OPENED,
             data={"url": "test"},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.open_url(
         OpenUrl(
             url="test",
@@ -505,15 +492,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test power control."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_POWER_SLEEPING,
+            type=EventType.POWER_SLEEPING,
             data={},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.power_sleep(
         request_id=REQUEST_ID,
     )
@@ -528,15 +515,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test power control."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_POWER_HIBERNATING,
+            type=EventType.POWER_HIBERNATING,
             data={},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.power_hibernate(
         request_id=REQUEST_ID,
     )
@@ -551,15 +538,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test power control."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_POWER_RESTARTING,
+            type=EventType.POWER_RESTARTING,
             data={},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.power_restart(
         request_id=REQUEST_ID,
     )
@@ -574,15 +561,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test power control."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_POWER_SHUTTINGDOWN,
+            type=EventType.POWER_SHUTTINGDOWN,
             data={},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.power_shutdown(
         request_id=REQUEST_ID,
     )
@@ -597,15 +584,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test power control."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_POWER_LOCKING,
+            type=EventType.POWER_LOCKING,
             data={},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.power_lock(
         request_id=REQUEST_ID,
     )
@@ -620,15 +607,15 @@
     ws_client: WebSocketGenerator,
 ):
     """Test power control."""
     websocket_client = await _get_websocket_client(
         ws_client,
         Response(
             id=REQUEST_ID,
-            type=TYPE_POWER_LOGGINGOUT,
+            type=EventType.POWER_LOGGINGOUT,
             data={},
         ),
     )
     assert websocket_client.connected is True
     response = await websocket_client.power_logout(
         request_id=REQUEST_ID,
     )
```

