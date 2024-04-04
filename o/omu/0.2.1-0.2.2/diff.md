# Comparing `tmp/omu-0.2.1.tar.gz` & `tmp/omu-0.2.2.tar.gz`

## Comparing `omu-0.2.1.tar` & `omu-0.2.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 omu-0.2.1/.gitattributes
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omu-0.2.1/.prettierrc
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omu-0.2.1/.python-version
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 omu-0.2.1/run_client.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/__init__.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/app.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/event_emitter.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/helper.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/identifier.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/model.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/plugin.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/serializer.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/client/__init__.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/client/client.py
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/client/omuclient.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/extension.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/extension_manager.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/asset/__init__.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/asset/asset_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/dashboard/dashboard.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/endpoint/endpoint.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/message/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/message/message.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/message/message_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/permission/__init__.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/permission/permission.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/permission/permission_extension.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/registry/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/registry/registry.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/registry/registry_extension.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/server/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/server/server_extension.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/table/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/table/table.py
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/table/table_extension.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/interface/__init__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/interface/keyable.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/interface/named.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/address.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/bytebuffer.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/connection.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/network.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/packet_mapper.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/websocket_connection.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/packet/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/packet/packet.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/packet/packet_types.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omu-0.2.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.1/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 omu-0.2.2/.gitattributes
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omu-0.2.2/.prettierrc
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omu-0.2.2/.python-version
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 omu-0.2.2/run_client.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/__init__.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/app.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/event_emitter.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/helper.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/identifier.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/model.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/plugin.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/serializer.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/client/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/client/client.py
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/client/omuclient.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/extension.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/extension_registry.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/asset/__init__.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/dashboard/dashboard.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/endpoint/endpoint.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/message/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/message/message.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/message/message_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/permission/__init__.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/permission/permission.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/registry/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/registry/registry.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/server/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/server/server_extension.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/table/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/table/table.py
+-rw-r--r--   0        0        0    15093 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/extension/table/table_extension.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/interface/__init__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/interface/keyable.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/interface/named.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/address.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/bytebuffer.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/connection.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/network.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/packet_mapper.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/websocket_connection.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/packet/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/packet/packet.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.2/src/omu/network/packet/packet_types.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omu-0.2.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.2/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.2/PKG-INFO
```

### Comparing `omu-0.2.1/run_client.py` & `omu-0.2.2/run_client.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/app.py` & `omu-0.2.2/src/omu/app.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/event_emitter.py` & `omu-0.2.2/src/omu/event_emitter.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/helper.py` & `omu-0.2.2/src/omu/helper.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/identifier.py` & `omu-0.2.2/src/omu/identifier.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/serializer.py` & `omu-0.2.2/src/omu/serializer.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/client/client.py` & `omu-0.2.2/src/omu/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import asyncio
 from typing import TYPE_CHECKING
 
 from omu.event_emitter import EventEmitter
 
 if TYPE_CHECKING:
     from omu.app import App
-    from omu.extension import ExtensionManager
+    from omu.extension import ExtensionRegistry
     from omu.extension.dashboard import DashboardExtension
     from omu.extension.endpoint import EndpointExtension
     from omu.extension.message import MessageExtension
     from omu.extension.permission import PermissionExtension
     from omu.extension.registry import RegistryExtension
     from omu.extension.server import ServerExtension
     from omu.extension.table import TableExtension
@@ -39,15 +39,15 @@
 
     @property
     @abc.abstractmethod
     def network(self) -> Network: ...
 
     @property
     @abc.abstractmethod
-    def extensions(self) -> ExtensionManager: ...
+    def extensions(self) -> ExtensionRegistry: ...
 
     @property
     @abc.abstractmethod
     def endpoints(self) -> EndpointExtension: ...
 
     @property
     @abc.abstractmethod
```

### Comparing `omu-0.2.1/src/omu/client/omuclient.py` & `omu-0.2.2/src/omu/client/omuclient.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,74 @@
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING
 
 from loguru import logger
 
-from omu.extension.asset import ASSET_EXTENSION_TYPE, AssetExtension
+from omu.app import App
+from omu.extension import ExtensionRegistry
+from omu.extension.asset import (
+    ASSET_EXTENSION_TYPE,
+    AssetExtension,
+)
 from omu.extension.dashboard import (
     DASHBOARD_EXTENSION_TYPE,
     DashboardExtension,
 )
 from omu.extension.endpoint import (
     ENDPOINT_EXTENSION_TYPE,
     EndpointExtension,
 )
-from omu.extension.extension_manager import ExtensionManager
 from omu.extension.message import (
     MESSAGE_EXTENSION_TYPE,
     MessageExtension,
 )
-from omu.extension.permission import PERMISSION_EXTENSION_TYPE, PermissionExtension
+from omu.extension.permission import (
+    PERMISSION_EXTENSION_TYPE,
+    PermissionExtension,
+)
 from omu.extension.registry import (
     REGISTRY_EXTENSION_TYPE,
     RegistryExtension,
 )
-from omu.extension.server import SERVER_EXTENSION_TYPE, ServerExtension
-from omu.extension.table import TABLE_EXTENSION_TYPE, TableExtension
+from omu.extension.server import (
+    SERVER_EXTENSION_TYPE,
+    ServerExtension,
+)
+from omu.extension.table import (
+    TABLE_EXTENSION_TYPE,
+    TableExtension,
+)
 from omu.network import Address, Network
 from omu.network.packet import Packet, PacketType
 from omu.network.websocket_connection import WebsocketsConnection
 
 from .client import Client, ClientListeners
 
-if TYPE_CHECKING:
-    from omu.app import App
-    from omu.extension import ExtensionManager
-
 
 class OmuClient(Client):
     def __init__(
         self,
         app: App,
         address: Address,
         connection: WebsocketsConnection | None = None,
-        extension_registry: ExtensionManager | None = None,
+        extension_registry: ExtensionRegistry | None = None,
         loop: asyncio.AbstractEventLoop | None = None,
     ):
         self._loop = loop or asyncio.get_event_loop()
         self._running = False
         self._listeners = ClientListeners()
         self._app = app
         self._network = Network(
             self,
             address,
             connection or WebsocketsConnection(self, address),
         )
         self._network.listeners.connected += self._listeners.ready.emit
-        self._extensions = extension_registry or ExtensionManager(self)
+        self._extensions = extension_registry or ExtensionRegistry(self)
 
         self._endpoints = self.extensions.register(ENDPOINT_EXTENSION_TYPE)
         self._tables = self.extensions.register(TABLE_EXTENSION_TYPE)
         self._registry = self.extensions.register(REGISTRY_EXTENSION_TYPE)
         self._message = self.extensions.register(MESSAGE_EXTENSION_TYPE)
         self._assets = self.extensions.register(ASSET_EXTENSION_TYPE)
         self._server = self.extensions.register(SERVER_EXTENSION_TYPE)
@@ -78,15 +86,15 @@
         return self._loop
 
     @property
     def network(self) -> Network:
         return self._network
 
     @property
-    def extensions(self) -> ExtensionManager:
+    def extensions(self) -> ExtensionRegistry:
         return self._extensions
 
     @property
     def endpoints(self) -> EndpointExtension:
         return self._endpoints
 
     @property
```

### Comparing `omu-0.2.1/src/omu/extension/extension.py` & `omu-0.2.2/src/omu/extension/extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/extension_manager.py` & `omu-0.2.2/src/omu/extension/extension_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING, Dict
 
 if TYPE_CHECKING:
     from omu.client import Client
     from omu.extension import Extension, ExtensionType
 
 
-class ExtensionManager:
+class ExtensionRegistry:
     def __init__(self, client: Client) -> None:
         self._client = client
         self._extensions: Dict[str, Extension] = {}
 
     def register[T: Extension](self, type: ExtensionType[T]) -> T:
         if self.has(type):
             raise ValueError(f"Extension type {type} already registered")
```

### Comparing `omu-0.2.1/src/omu/extension/asset/asset_extension.py` & `omu-0.2.2/src/omu/extension/asset/asset_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 from typing import List, Mapping
 
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.extension.endpoint import EndpointType
-from omu.helper import instance
 from omu.identifier import Identifier
 from omu.network.bytebuffer import ByteReader, ByteWriter
-from omu.serializer import Serializable, Serializer
+from omu.serializer import Serializer
 
 ASSET_EXTENSION_TYPE = ExtensionType(
     "asset",
     lambda client: AssetExtension(client),
     lambda: [],
 )
 type Files = Mapping[Identifier, bytes]
 
 
-@instance
-class FILES_SERIALIZER(Serializable[Files, bytes]):
-    def serialize(self, item: Files) -> bytes:
+class FILES_SERIALIZER:
+    @classmethod
+    def serialize(cls, item: Files) -> bytes:
         writer = ByteWriter()
         writer.write_int(len(item))
         for identifier, value in item.items():
             writer.write_string(identifier.key())
             writer.write_byte_array(value)
         return writer.finish()
 
-    def deserialize(self, item: bytes) -> Files:
+    @classmethod
+    def deserialize(cls, item: bytes) -> Files:
         with ByteReader(item) as reader:
             count = reader.read_int()
             files: Files = {}
             for _ in range(count):
                 identifier = Identifier.from_key(reader.read_string())
                 value = reader.read_byte_array()
                 files[identifier] = value
```

### Comparing `omu-0.2.1/src/omu/extension/dashboard/dashboard.py` & `omu-0.2.2/src/omu/extension/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/dashboard/dashboard_extension.py` & `omu-0.2.2/src/omu/extension/dashboard/dashboard_extension.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,21 +29,18 @@
         )
 
 
 class DashboardSetResponse(TypedDict):
     success: bool
 
 
-DASHBOARD_SET_ENDPOINT = EndpointType[
-    Identifier, DashboardSetResponse
-].create_serialized(
+DASHBOARD_SET_ENDPOINT = EndpointType[Identifier, DashboardSetResponse].create_json(
     DASHBOARD_EXTENSION_TYPE,
     "set",
-    request_serializer=Serializer.model(Identifier).pipe(Serializer.json()),
-    response_serializer=Serializer.json(),
+    request_serializer=Serializer.model(Identifier),
 )
 DASHBOARD_PERMISSION_REQUEST_PACKET = PacketType.create_json(
     DASHBOARD_EXTENSION_TYPE,
     "permission_request",
     Serializer.model(PermissionRequest),
 )
 DASHBOARD_PERMISSION_ACCEPT_PACKET = PacketType[int].create_json(
```

### Comparing `omu-0.2.1/src/omu/extension/endpoint/endpoint.py` & `omu-0.2.2/src/omu/extension/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/endpoint/endpoint_extension.py` & `omu-0.2.2/src/omu/extension/endpoint/endpoint_extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 from __future__ import annotations
 
 from asyncio import Future
-from typing import Any, Callable, Dict, Tuple, TypedDict
+from typing import Any, Callable, Dict, List, Tuple, TypedDict
 
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.helper import Coro
+from omu.identifier import Identifier
 from omu.network.bytebuffer import ByteReader, ByteWriter
 from omu.network.packet import PacketType
-from omu.serializer import Serializable, Serializer
+from omu.serializer import Serializer
 
 from .endpoint import EndpointType
 
 ENDPOINT_EXTENSION_TYPE = ExtensionType(
     "endpoint",
     lambda client: EndpointExtension(client),
     lambda: [],
 )
 
 
 class EndpointExtension(Extension):
     def __init__(self, client: Client) -> None:
         self.client = client
         self.response_promises: Dict[int, Future] = {}
-        self.endpoints: Dict[str, Tuple[EndpointType, Coro[[Any], Any]]] = {}
+        self.endpoints: Dict[Identifier, Tuple[EndpointType, Coro[[Any], Any]]] = {}
         self.call_id = 0
         client.network.register_packet(
+            ENDPOINT_REGISTER_PACKET,
             ENDPOINT_CALL_PACKET,
             ENDPOINT_RECEIVE_PACKET,
             ENDPOINT_ERROR_PACKET,
         )
         client.network.add_packet_handler(ENDPOINT_RECEIVE_PACKET, self._on_receive)
         client.network.add_packet_handler(ENDPOINT_ERROR_PACKET, self._on_error)
         client.network.add_packet_handler(ENDPOINT_CALL_PACKET, self._on_call)
         client.network.listeners.connected += self.on_connected
 
-    async def _on_receive(self, data: EndpointDataReq) -> None:
+    async def _on_receive(self, data: EndpointDataPacket) -> None:
         if data["id"] not in self.response_promises:
             raise Exception(f"Received response for unknown call id {data['id']}")
         future = self.response_promises.pop(data["id"])
         future.set_result(data["data"])
 
-    async def _on_error(self, data: EndpointError) -> None:
+    async def _on_error(self, data: EndpointErrorPacket) -> None:
         if data["id"] not in self.response_promises:
             raise Exception(f"Received error for unknown call id {data['id']}")
         future = self.response_promises.pop(data["id"])
         future.set_exception(Exception(data["error"]))
 
-    async def _on_call(self, data: EndpointDataReq) -> None:
-        if data["type"] not in self.endpoints:
-            return
-        endpoint, func = self.endpoints[data["type"]]
+    async def _on_call(self, data: EndpointDataPacket) -> None:
+        endpoint_id = Identifier.from_key(data["type"])
+        if endpoint_id not in self.endpoints:
+            raise Exception(f"Received call for unknown endpoint {endpoint_id}")
+        endpoint, func = self.endpoints[endpoint_id]
         try:
             req = endpoint.request_serializer.deserialize(data["data"])
             res = await func(req)
             res_data = endpoint.response_serializer.serialize(res)
             await self.client.send(
                 ENDPOINT_RECEIVE_PACKET,
-                EndpointDataReq(type=data["type"], id=data["id"], data=res_data),
+                EndpointDataPacket(type=data["type"], id=data["id"], data=res_data),
             )
         except Exception as e:
             await self.client.send(
                 ENDPOINT_ERROR_PACKET,
-                EndpointError(type=data["type"], id=data["id"], error=str(e)),
+                EndpointErrorPacket(type=data["type"], id=data["id"], error=str(e)),
             )
             raise e
 
     async def on_connected(self) -> None:
-        for endpoint, _ in self.endpoints.values():
-            await self.client.send(ENDPOINT_REGISTER_PACKET, endpoint.identifier.key())
+        await self.client.send(ENDPOINT_REGISTER_PACKET, [*self.endpoints.keys()])
 
     def register[Req, Res](
         self, type: EndpointType[Req, Res], func: Coro[[Req], Res]
     ) -> None:
-        if type.identifier.key() in self.endpoints:
-            raise Exception(
-                f"Endpoint for key {type.identifier.key()} already registered"
-            )
-        self.endpoints[type.identifier.key()] = (type, func)
+        if type.identifier in self.endpoints:
+            raise Exception(f"Endpoint for key {type.identifier} already registered")
+        self.endpoints[type.identifier] = (type, func)
 
     def bind[T, R](
         self,
         func: Coro[[T], R] | None = None,
         endpoint_type: EndpointType[T, R] | None = None,
     ):
         if endpoint_type is None:
@@ -114,73 +114,69 @@
         try:
             self.call_id += 1
             future = Future[bytes]()
             self.response_promises[self.call_id] = future
             json = endpoint.request_serializer.serialize(data)
             await self.client.send(
                 ENDPOINT_CALL_PACKET,
-                EndpointDataReq(
+                EndpointDataPacket(
                     type=endpoint.identifier.key(), id=self.call_id, data=json
                 ),
             )
             res = await future
             return endpoint.response_serializer.deserialize(res)
         except Exception as e:
             raise Exception(
                 f"Error calling endpoint {endpoint.identifier.key()}"
             ) from e
 
 
-class EndpointReq(TypedDict):
+class EndpointPacket(TypedDict):
     type: str
     id: int
 
 
-class EndpointDataReq(EndpointReq):
-    type: str
-    id: int
+class EndpointDataPacket(EndpointPacket):
     data: bytes
 
 
-class EndpointError(EndpointReq):
-    type: str
-    id: int
+class EndpointErrorPacket(EndpointPacket):
     error: str
 
 
-class CallSerializer(Serializable[EndpointDataReq, bytes]):
-    def serialize(self, item: EndpointDataReq) -> bytes:
+class ENDPOINT_DATA_SERIALIZER:
+    @classmethod
+    def serialize(cls, item: EndpointDataPacket) -> bytes:
         writer = ByteWriter()
         writer.write_string(item["type"])
         writer.write_int(item["id"])
         writer.write_byte_array(item["data"])
         return writer.finish()
 
-    def deserialize(self, item: bytes) -> EndpointDataReq:
+    @classmethod
+    def deserialize(cls, item: bytes) -> EndpointDataPacket:
         with ByteReader(item) as reader:
             type = reader.read_string()
             id = reader.read_int()
             data = reader.read_byte_array()
-        return EndpointDataReq(type=type, id=id, data=data)
-
+        return EndpointDataPacket(type=type, id=id, data=data)
 
-CALL_SERIALIZER = CallSerializer()
 
-ENDPOINT_REGISTER_PACKET = PacketType[str].create_json(
+ENDPOINT_REGISTER_PACKET = PacketType[List[Identifier]].create_json(
     ENDPOINT_EXTENSION_TYPE,
     "register",
-    Serializer.json(),
+    Serializer.model(Identifier).array(),
 )
-ENDPOINT_CALL_PACKET = PacketType[EndpointDataReq].create_serialized(
+ENDPOINT_CALL_PACKET = PacketType[EndpointDataPacket].create_serialized(
     ENDPOINT_EXTENSION_TYPE,
     "call",
-    CALL_SERIALIZER,
+    ENDPOINT_DATA_SERIALIZER,
 )
-ENDPOINT_RECEIVE_PACKET = PacketType[EndpointDataReq].create_serialized(
+ENDPOINT_RECEIVE_PACKET = PacketType[EndpointDataPacket].create_serialized(
     ENDPOINT_EXTENSION_TYPE,
     "receive",
-    CALL_SERIALIZER,
+    ENDPOINT_DATA_SERIALIZER,
 )
-ENDPOINT_ERROR_PACKET = PacketType[EndpointError].create_json(
+ENDPOINT_ERROR_PACKET = PacketType[EndpointErrorPacket].create_json(
     ENDPOINT_EXTENSION_TYPE,
     "error",
 )
```

### Comparing `omu-0.2.1/src/omu/extension/message/message.py` & `omu-0.2.2/src/omu/extension/message/message.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/message/message_extension.py` & `omu-0.2.2/src/omu/extension/message/message_extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,50 +5,51 @@
 
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.helper import Coro
 from omu.identifier import Identifier
 from omu.network.bytebuffer import ByteReader, ByteWriter
 from omu.network.packet import PacketType
-from omu.serializer import Serializable
 
 from .message import Message, MessageType
 
 MESSAGE_EXTENSION_TYPE = ExtensionType(
     "message",
     lambda client: MessageExtension(client),
     lambda: [],
 )
 
 
 @dataclass
-class MessageData:
+class MessagePacket:
     key: str
     body: bytes
 
 
-class MessageSerializer(Serializable[MessageData, bytes]):
-    def serialize(self, item: MessageData) -> bytes:
+class MESSAGE_SERIALIZER:
+    @classmethod
+    def serialize(cls, item: MessagePacket) -> bytes:
         writer = ByteWriter()
         writer.write_string(item.key)
         writer.write_byte_array(item.body)
         return writer.finish()
 
-    def deserialize(self, item: bytes) -> MessageData:
+    @classmethod
+    def deserialize(cls, item: bytes) -> MessagePacket:
         with ByteReader(item) as reader:
             key = reader.read_string()
             body = reader.read_byte_array()
-        return MessageData(key=key, body=body)
+        return MessagePacket(key=key, body=body)
 
 
 MESSAGE_LISTEN_PACKET = PacketType[str].create_json(MESSAGE_EXTENSION_TYPE, "listen")
-MESSAGE_BROADCAST_PACKET = PacketType[MessageData].create_serialized(
+MESSAGE_BROADCAST_PACKET = PacketType[MessagePacket].create_serialized(
     MESSAGE_EXTENSION_TYPE,
     "broadcast",
-    MessageSerializer(),
+    MESSAGE_SERIALIZER(),
 )
 
 
 class MessageExtension(Extension):
     def __init__(self, client: Client):
         self.client = client
         self._message_identifiers: List[Identifier] = []
@@ -78,25 +79,25 @@
         self.listening = False
         client.network.add_packet_handler(MESSAGE_BROADCAST_PACKET, self._on_broadcast)
 
     async def broadcast(self, body: T) -> None:
         data = self.serializer.serialize(body)
         await self.client.send(
             MESSAGE_BROADCAST_PACKET,
-            MessageData(key=self.key, body=data),
+            MessagePacket(key=self.key, body=data),
         )
 
     def listen(self, listener: Coro[[T], None]) -> Callable[[], None]:
         self.listeners.append(listener)
         if not self.listening:
             self.client.network.add_task(self._listen)
             self.listening = True
         return lambda: self.listeners.remove(listener)
 
     async def _listen(self) -> None:
         await self.client.send(MESSAGE_LISTEN_PACKET, self.key)
 
-    async def _on_broadcast(self, data: MessageData) -> None:
+    async def _on_broadcast(self, data: MessagePacket) -> None:
         if data.key != self.key:
             return
         for listener in self.listeners:
             await listener(data.body)
```

### Comparing `omu-0.2.1/src/omu/extension/permission/permission.py` & `omu-0.2.2/src/omu/extension/permission/permission.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/permission/permission_extension.py` & `omu-0.2.2/src/omu/extension/permission/permission_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/plugin/plugin_extension.py` & `omu-0.2.2/src/omu/extension/plugin/plugin_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/registry/registry.py` & `omu-0.2.2/src/omu/extension/registry/registry.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/registry/registry_extension.py` & `omu-0.2.2/src/omu/extension/registry/registry_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,47 +18,49 @@
     "registry",
     lambda client: RegistryExtension(client),
     lambda: [],
 )
 
 
 @dataclass(frozen=True)
-class RegistryData:
+class RegistryPacket:
     key: str
     existing: bool
     value: bytes
 
 
-class RegistryDataSerializer(Serializable[RegistryData, bytes]):
-    def serialize(self, item: RegistryData) -> bytes:
+class REGISTRY_DATA_SERIALIZER:
+    @classmethod
+    def serialize(cls, item: RegistryPacket) -> bytes:
         writer = ByteWriter()
         writer.write_string(item.key)
         writer.write_boolean(item.existing)
         writer.write_byte_array(item.value)
         return writer.finish()
 
-    def deserialize(self, item: bytes) -> RegistryData:
+    @classmethod
+    def deserialize(cls, item: bytes) -> RegistryPacket:
         with ByteReader(item) as reader:
             key = reader.read_string()
             existing = reader.read_boolean()
             value = reader.read_byte_array()
-            return RegistryData(key, existing, value)
+            return RegistryPacket(key, existing, value)
 
 
-REGISTRY_UPDATE_PACKET = PacketType[RegistryData].create_serialized(
+REGISTRY_UPDATE_PACKET = PacketType[RegistryPacket].create_serialized(
     REGISTRY_EXTENSION_TYPE,
     "update",
-    serializer=RegistryDataSerializer(),
+    serializer=REGISTRY_DATA_SERIALIZER,
 )
 REGISTRY_LISTEN_PACKET = PacketType[str].create_json(REGISTRY_EXTENSION_TYPE, "listen")
-REGISTRY_GET_ENDPOINT = EndpointType[str, RegistryData].create_serialized(
+REGISTRY_GET_ENDPOINT = EndpointType[str, RegistryPacket].create_serialized(
     REGISTRY_EXTENSION_TYPE,
     "get",
     request_serializer=Serializer.json(),
-    response_serializer=RegistryDataSerializer(),
+    response_serializer=REGISTRY_DATA_SERIALIZER,
 )
 
 
 class RegistryExtension(Extension):
     def __init__(self, client: Client) -> None:
         self.client = client
         client.network.register_packet(REGISTRY_UPDATE_PACKET)
@@ -100,15 +102,15 @@
         return self.serializer.deserialize(result.value)
 
     async def update(self, handler: Coro[[T], T]) -> None:
         value = await self.get()
         new_value = await handler(value)
         await self.client.send(
             REGISTRY_UPDATE_PACKET,
-            RegistryData(
+            RegistryPacket(
                 self.key,
                 True,
                 self.serializer.serialize(new_value),
             ),
         )
 
     def listen(self, handler: Coro[[T], None]) -> Callable[[], None]:
@@ -117,15 +119,15 @@
                 lambda: self.client.send(REGISTRY_LISTEN_PACKET, self.key)
             )
             self.listening = True
 
         self.listeners.append(handler)
         return lambda: self.listeners.remove(handler)
 
-    async def _on_update(self, event: RegistryData) -> None:
+    async def _on_update(self, event: RegistryPacket) -> None:
         if event.key != self.key:
             return
         if event.existing:
             value = self.serializer.deserialize(event.value)
         else:
             value = self.default_value
         for listener in self.listeners:
```

### Comparing `omu-0.2.1/src/omu/extension/server/server_extension.py` & `omu-0.2.2/src/omu/extension/server/server_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/extension/table/table.py` & `omu-0.2.2/src/omu/extension/table/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     @abc.abstractmethod
     def set_cache_size(self, size: int) -> None: ...
 
     @abc.abstractmethod
     async def get(self, key: str) -> T | None: ...
 
     @abc.abstractmethod
+    async def get_many(self, *keys: str) -> Dict[str, T]: ...
+
+    @abc.abstractmethod
     async def add(self, *items: T) -> None: ...
 
     @abc.abstractmethod
     async def update(self, *items: T) -> None: ...
 
     @abc.abstractmethod
     async def remove(self, *items: T) -> None: ...
```

### Comparing `omu-0.2.1/src/omu/extension/table/table_extension.py` & `omu-0.2.2/src/omu/extension/table/table_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import (
     AsyncGenerator,
     Callable,
     Dict,
     Iterable,
     List,
     Mapping,
+    Sequence,
     TypedDict,
 )
 
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.extension.endpoint import EndpointType
 from omu.helper import AsyncCallback, Coro
@@ -29,15 +30,15 @@
 
 
 class TableExtension(Extension):
     def __init__(self, client: Client):
         self._client = client
         self._tables: Dict[Identifier, Table] = {}
         client.network.register_packet(
-            TABLE_CONFIG_SET_PACKET,
+            TABLE_CONFIG_PACKET,
             TABLE_LISTEN_PACKET,
             TABLE_PROXY_LISTEN_PACKET,
             TABLE_PROXY_PACKET,
             TABLE_ITEM_ADD_PACKET,
             TABLE_ITEM_UPDATE_PACKET,
             TABLE_ITEM_REMOVE_EVENT,
             TABLE_ITEM_CLEAR_PACKET,
@@ -91,55 +92,65 @@
 
 
 class TableItemsData(TableEventData):
     items: Dict[str, bytes]
 
 
 class TableKeysData(TableEventData):
-    keys: List[str]
+    keys: Sequence[str]
 
 
 class TableProxyData(TableItemsData):
     key: int
 
 
-class TableItemsSerielizer(Serializable[TableItemsData, bytes]):
-    def serialize(self, item: TableItemsData) -> bytes:
+class TableFetchReq(TableEventData):
+    before: int | None
+    after: int | None
+    cursor: str | None
+
+
+class ITEMS_SERIALIZER:
+    @classmethod
+    def serialize(cls, item: TableItemsData) -> bytes:
         writer = ByteWriter()
         writer.write_string(item["type"])
         writer.write_int(len(item["items"]))
         for key, value in item["items"].items():
             writer.write_string(key)
             writer.write_byte_array(value)
         return writer.finish()
 
-    def deserialize(self, item: bytes) -> TableItemsData:
+    @classmethod
+    def deserialize(cls, item: bytes) -> TableItemsData:
         with ByteReader(item) as reader:
             type = reader.read_string()
             item_count = reader.read_int()
             items: Mapping[str, bytes] = {}
             for _ in range(item_count):
                 key = reader.read_string()
                 value = reader.read_byte_array()
                 items[key] = value
         return {"type": type, "items": items}
 
 
-class TableProxySerielizer(Serializable[TableProxyData, bytes]):
-    def serialize(self, item: TableProxyData) -> bytes:
+class ITEM_PROXY_SERIALIZER:
+    @staticmethod
+    def serialize(item: TableProxyData) -> bytes:
         writer = ByteWriter()
         writer.write_string(item["type"])
         writer.write_int(item["key"])
         writer.write_int(len(item["items"]))
         for key, value in item["items"].items():
             writer.write_string(key)
             writer.write_byte_array(value)
         return writer.finish()
 
-    def deserialize(self, item: bytes) -> TableProxyData:
+    @staticmethod
+    def deserialize(item: bytes) -> TableProxyData:
         with ByteReader(item) as reader:
             type = reader.read_string()
             key = reader.read_int()
             item_count = reader.read_int()
             items: Dict[str, bytes] = {}
             for _ in range(item_count):
                 item_key = reader.read_string()
@@ -149,77 +160,71 @@
 
 
 class SetConfigReq(TypedDict):
     type: str
     config: TableConfig
 
 
-TABLE_CONFIG_SET_PACKET = PacketType[SetConfigReq].create_json(
-    TABLE_EXTENSION_TYPE, "config_set"
+TABLE_CONFIG_PACKET = PacketType[SetConfigReq].create_json(
+    TABLE_EXTENSION_TYPE,
+    "config",
+)
+TABLE_LISTEN_PACKET = PacketType[str].create_json(
+    TABLE_EXTENSION_TYPE,
+    "listen",
 )
-TABLE_LISTEN_PACKET = PacketType[str].create_json(TABLE_EXTENSION_TYPE, name="listen")
 TABLE_PROXY_LISTEN_PACKET = PacketType[str].create_json(
     TABLE_EXTENSION_TYPE, "proxy_listen"
 )
 TABLE_PROXY_PACKET = PacketType[TableProxyData].create_serialized(
     TABLE_EXTENSION_TYPE,
     "proxy",
-    serializer=TableProxySerielizer(),
-)
-TABLE_PROXY_ENDPOINT = EndpointType[TableProxyData, int].create_serialized(
-    TABLE_EXTENSION_TYPE,
-    "proxy",
-    request_serializer=TableProxySerielizer(),
-    response_serializer=Serializer.json(),
+    serializer=ITEM_PROXY_SERIALIZER,
 )
 TABLE_ITEM_ADD_PACKET = PacketType[TableItemsData].create_serialized(
-    TABLE_EXTENSION_TYPE, "item_add", TableItemsSerielizer()
+    TABLE_EXTENSION_TYPE,
+    "item_add",
+    ITEMS_SERIALIZER,
 )
 TABLE_ITEM_UPDATE_PACKET = PacketType[TableItemsData].create_serialized(
-    TABLE_EXTENSION_TYPE, "item_update", TableItemsSerielizer()
+    TABLE_EXTENSION_TYPE,
+    "item_update",
+    ITEMS_SERIALIZER,
 )
 TABLE_ITEM_REMOVE_EVENT = PacketType[TableItemsData].create_serialized(
-    TABLE_EXTENSION_TYPE, "item_remove", TableItemsSerielizer()
-)
-TABLE_ITEM_CLEAR_PACKET = PacketType[TableEventData].create_json(
-    TABLE_EXTENSION_TYPE, "item_clear"
+    TABLE_EXTENSION_TYPE,
+    "item_remove",
+    ITEMS_SERIALIZER,
 )
 TABLE_ITEM_GET_ENDPOINT = EndpointType[TableKeysData, TableItemsData].create_serialized(
     TABLE_EXTENSION_TYPE,
     "item_get",
     request_serializer=Serializer.json(),
-    response_serializer=TableItemsSerielizer(),
+    response_serializer=ITEMS_SERIALIZER,
 )
-
-
-class TableFetchReq(TypedDict):
-    type: str
-    before: int | None
-    after: int | None
-    cursor: str | None
-
-
-TABLE_ITEM_FETCH_ENDPOINT = EndpointType[
-    TableFetchReq, TableItemsData
-].create_serialized(
+TABLE_FETCH_ENDPOINT = EndpointType[TableFetchReq, TableItemsData].create_serialized(
     TABLE_EXTENSION_TYPE,
-    "item_fetch",
+    "fetch",
     request_serializer=Serializer.json(),
-    response_serializer=TableItemsSerielizer(),
+    response_serializer=ITEMS_SERIALIZER,
 )
-TABLE_ITEM_FETCH_ALL_ENDPOINT = EndpointType[
+TABLE_FETCH_ALL_ENDPOINT = EndpointType[
     TableEventData, TableItemsData
 ].create_serialized(
     TABLE_EXTENSION_TYPE,
-    "item_fetch_all",
+    "fetch_all",
     request_serializer=Serializer.json(),
-    response_serializer=TableItemsSerielizer(),
+    response_serializer=ITEMS_SERIALIZER,
 )
-TABLE_ITEM_SIZE_ENDPOINT = EndpointType[TableEventData, int].create_json(
-    TABLE_EXTENSION_TYPE, "item_size"
+TABLE_SIZE_ENDPOINT = EndpointType[TableEventData, int].create_json(
+    TABLE_EXTENSION_TYPE, "size"
+)
+TABLE_ITEM_CLEAR_PACKET = PacketType[TableEventData].create_json(
+    TABLE_EXTENSION_TYPE,
+    "clear",
 )
 
 
 class TableImpl[T](Table[T]):
     def __init__(
         self,
         client: Client,
@@ -261,14 +266,22 @@
         )
         items = self._parse_items(res["items"])
         self._cache.update(items)
         if key in items:
             return items[key]
         return None
 
+    async def get_many(self, *keys: str) -> Dict[str, T]:
+        res = await self._client.endpoints.call(
+            TABLE_ITEM_GET_ENDPOINT, TableKeysData(type=self.key, keys=keys)
+        )
+        items = self._parse_items(res["items"])
+        self._cache.update(items)
+        return items
+
     async def add(self, *items: T) -> None:
         data = self._serialize_items(items)
         await self._client.send(
             TABLE_ITEM_ADD_PACKET, TableItemsData(type=self.key, items=data)
         )
 
     async def update(self, *items: T) -> None:
@@ -289,24 +302,24 @@
     async def fetch_items(
         self,
         before: int | None = None,
         after: int | None = None,
         cursor: str | None = None,
     ) -> Dict[str, T]:
         items_response = await self._client.endpoints.call(
-            TABLE_ITEM_FETCH_ENDPOINT,
+            TABLE_FETCH_ENDPOINT,
             TableFetchReq(type=self.key, before=before, after=after, cursor=cursor),
         )
         items = self._parse_items(items_response["items"])
         await self.update_cache(items)
         return items
 
     async def fetch_all(self) -> Dict[str, T]:
         items_response = await self._client.endpoints.call(
-            TABLE_ITEM_FETCH_ALL_ENDPOINT, TableEventData(type=self.key)
+            TABLE_FETCH_ALL_ENDPOINT, TableEventData(type=self.key)
         )
         items = self._parse_items(items_response["items"])
         await self.update_cache(items)
         return items
 
     async def iterate(
         self,
@@ -329,15 +342,15 @@
             )
             for item in items.values():
                 yield item
             items.pop(cursor, None)
 
     async def size(self) -> int:
         res = await self._client.endpoints.call(
-            TABLE_ITEM_SIZE_ENDPOINT, TableEventData(type=self.key)
+            TABLE_SIZE_ENDPOINT, TableEventData(type=self.key)
         )
         return res
 
     def listen(
         self, listener: AsyncCallback[Mapping[str, T]] | None = None
     ) -> Callable[[], None]:
         self._listening = True
@@ -352,15 +365,15 @@
 
     def set_config(self, config: TableConfig) -> None:
         self._config = config
 
     async def on_connected(self) -> None:
         if self._config is not None:
             await self._client.send(
-                TABLE_CONFIG_SET_PACKET,
+                TABLE_CONFIG_PACKET,
                 SetConfigReq(type=self.key, config=self._config),
             )
         if self._listening:
             await self._client.send(TABLE_LISTEN_PACKET, self.key)
         if len(self._proxies) > 0:
             await self._client.send(TABLE_PROXY_LISTEN_PACKET, self.key)
 
@@ -372,16 +385,16 @@
             for key, item in list(items.items()):
                 updated_item = await proxy(item)
                 if updated_item is None:
                     del items[key]
                 else:
                     items[key] = updated_item
         serialized_items = self._serialize_items(items.values())
-        await self._client.endpoints.call(
-            TABLE_PROXY_ENDPOINT,
+        await self._client.send(
+            TABLE_PROXY_PACKET,
             TableProxyData(
                 type=self.key,
                 key=event["key"],
                 items=serialized_items,
             ),
         )
```

### Comparing `omu-0.2.1/src/omu/network/bytebuffer.py` & `omu-0.2.2/src/omu/network/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/network/connection.py` & `omu-0.2.2/src/omu/network/connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/network/network.py` & `omu-0.2.2/src/omu/network/network.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/network/packet_mapper.py` & `omu-0.2.2/src/omu/network/packet_mapper.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/network/websocket_connection.py` & `omu-0.2.2/src/omu/network/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/network/packet/packet.py` & `omu-0.2.2/src/omu/network/packet/packet.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/src/omu/network/packet/packet_types.py` & `omu-0.2.2/src/omu/network/packet/packet_types.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.1/pyproject.toml` & `omu-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omu"
-version = "0.2.1"
+version = "0.2.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["loguru>=0.7.2"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

