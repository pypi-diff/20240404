# Comparing `tmp/omuserver-0.2.1.tar.gz` & `tmp/omuserver-0.2.2.tar.gz`

## Comparing `omuserver-0.2.1.tar` & `omuserver-0.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuserver-0.2.1/.python-version
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuserver-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/__init__.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/__main__.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/config.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/directories.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/helper.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/extension.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/asset/__init__.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/asset/asset_extension.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/message/__init__.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/message/message_extension.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/permission/__init__.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/permission/permission_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/plugin/plugin_connection.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/plugin/plugin_loader.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/plugin/plugin_session_connection.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/registry/__init__.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/registry/registry.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/registry/registry_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/server/__init__.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/server/server_extension.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/__init__.py
--rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/cached_table.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/serialized_table.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/server_table.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/session_table_handler.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/table_extension.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/adapters/__init__.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/adapters/sqlitetable.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/extension/table/adapters/tableadapter.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/network/__init__.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/network/network.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/network/packet_dispatcher.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/security/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/security/security.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/server/__init__.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/server/omuserver.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/server/server.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/session/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/session/aiohttp_connection.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 omuserver-0.2.1/src/omuserver/session/session.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.2.1/test/helper_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuserver-0.2.1/.gitignore
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.2.1/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 omuserver-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 omuserver-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuserver-0.2.2/.python-version
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuserver-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/__init__.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/__main__.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/config.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/directories.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/helper.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/extension.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/asset/__init__.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/message/__init__.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/message/message_extension.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/permission/__init__.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/plugin/plugin_connection.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/plugin/plugin_loader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/plugin/plugin_session_connection.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/registry/__init__.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/registry/registry.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/server/__init__.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/server/server_extension.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/__init__.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/cached_table.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/serialized_table.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/server_table.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/session_table_handler.py
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/table_extension.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/adapters/__init__.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/adapters/sqlitetable.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/extension/table/adapters/tableadapter.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/network/__init__.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/network/network.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/network/packet_dispatcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/security/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/security/security.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/server/__init__.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/server/omuserver.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/server/server.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/session/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/session/aiohttp_connection.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 omuserver-0.2.2/src/omuserver/session/session.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.2.2/test/helper_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuserver-0.2.2/.gitignore
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.2.2/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 omuserver-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 omuserver-0.2.2/PKG-INFO
```

### Comparing `omuserver-0.2.1/src/omuserver/__main__.py` & `omuserver-0.2.2/src/omuserver/__main__.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/directories.py` & `omuserver-0.2.2/src/omuserver/directories.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/helper.py` & `omuserver-0.2.2/src/omuserver/helper.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/asset/asset_extension.py` & `omuserver-0.2.2/src/omuserver/extension/asset/asset_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/dashboard/dashboard_extension.py` & `omuserver-0.2.2/src/omuserver/extension/dashboard/dashboard_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/message/message_extension.py` & `omuserver-0.2.2/src/omuserver/extension/message/message_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict
 
 from omu.extension.message.message_extension import (
     MESSAGE_BROADCAST_PACKET,
     MESSAGE_LISTEN_PACKET,
-    MessageData,
+    MessagePacket,
 )
 
 if TYPE_CHECKING:
     from omuserver import Server
     from omuserver.session.session import Session
 
 
@@ -50,14 +50,14 @@
 
     async def _on_listen(self, session: Session, key: str) -> None:
         if key not in self._keys:
             self._keys[key] = Message(key)
         message = self._keys[key]
         message.add_listener(session)
 
-    async def _on_broadcast(self, session: Session, data: MessageData) -> None:
+    async def _on_broadcast(self, session: Session, data: MessagePacket) -> None:
         key = data.key
         if key not in self._keys:
             self._keys[key] = Message(key)
         message = self._keys[key]
         for listener in message.listeners:
             await listener.send(MESSAGE_BROADCAST_PACKET, data)
```

### Comparing `omuserver-0.2.1/src/omuserver/extension/permission/permission_extension.py` & `omuserver-0.2.2/src/omuserver/extension/permission/permission_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/plugin/plugin_connection.py` & `omuserver-0.2.2/src/omuserver/extension/plugin/plugin_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/plugin/plugin_extension.py` & `omuserver-0.2.2/src/omuserver/extension/plugin/plugin_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/plugin/plugin_loader.py` & `omuserver-0.2.2/src/omuserver/extension/plugin/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/plugin/plugin_session_connection.py` & `omuserver-0.2.2/src/omuserver/extension/plugin/plugin_session_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/registry/registry.py` & `omuserver-0.2.2/src/omuserver/extension/registry/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict
 
 from omu import Identifier
 from omu.extension.registry.registry_extension import (
     REGISTRY_UPDATE_PACKET,
-    RegistryData,
+    RegistryPacket,
 )
 from omu.serializer import Serializable
 
 from omuserver.server import Server
 from omuserver.session import Session
 
 
@@ -38,25 +38,25 @@
 
     async def _notify(self) -> None:
         for listener in self._listeners.values():
             if listener.closed:
                 raise Exception(f"Session {listener.app=} closed")
             await listener.send(
                 REGISTRY_UPDATE_PACKET,
-                RegistryData(key=self._key, existing=self.existing, value=self.data),
+                RegistryPacket(key=self._key, existing=self.existing, value=self.data),
             )
 
     async def attach_session(self, session: Session) -> None:
         if session.app.key() in self._listeners:
             del self._listeners[session.app.key()]
         self._listeners[session.app.key()] = session
         session.listeners.disconnected += self.detach_session
         await session.send(
             REGISTRY_UPDATE_PACKET,
-            RegistryData(key=self._key, existing=self.existing, value=self.data),
+            RegistryPacket(key=self._key, existing=self.existing, value=self.data),
         )
 
     async def detach_session(self, session: Session) -> None:
         if session.app.key() not in self._listeners:
             raise Exception("Session not attached")
         del self._listeners[session.app.key()]
         session.listeners.disconnected -= self.detach_session
```

### Comparing `omuserver-0.2.1/src/omuserver/extension/registry/registry_extension.py` & `omuserver-0.2.2/src/omuserver/extension/registry/registry_extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import TYPE_CHECKING, Dict
 
 from omu.extension.registry.registry_extension import (
     REGISTRY_GET_ENDPOINT,
     REGISTRY_LISTEN_PACKET,
     REGISTRY_UPDATE_PACKET,
-    RegistryData,
+    RegistryPacket,
 )
 from omu.identifier import Identifier
 from omu.serializer import Serializable
 
 from omuserver.session import Session
 
 from .registry import Registry, ServerRegistry
@@ -34,21 +34,21 @@
         server.endpoints.bind_endpoint(REGISTRY_GET_ENDPOINT, self._on_get)
         self.registries: Dict[Identifier, ServerRegistry] = {}
 
     async def _on_listen(self, session: Session, key: str) -> None:
         registry = await self.get(key)
         await registry.attach_session(session)
 
-    async def _on_update(self, session: Session, event: RegistryData) -> None:
+    async def _on_update(self, session: Session, event: RegistryPacket) -> None:
         registry = await self.get(event.key)
         await registry.store(event.value)
 
-    async def _on_get(self, session: Session, key: str) -> RegistryData:
+    async def _on_get(self, session: Session, key: str) -> RegistryPacket:
         registry = await self.get(key)
-        return RegistryData(key, registry.existing, registry.data)
+        return RegistryPacket(key, registry.existing, registry.data)
 
     async def get(self, key: str) -> ServerRegistry:
         identifier = Identifier.from_key(key)
         registry = self.registries.get(identifier)
         if registry is None:
             registry = ServerRegistry(self._server, identifier)
             self.registries[identifier] = registry
```

### Comparing `omuserver-0.2.1/src/omuserver/extension/server/server_extension.py` & `omuserver-0.2.2/src/omuserver/extension/server/server_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/table/cached_table.py` & `omuserver-0.2.2/src/omuserver/extension/table/cached_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,26 @@
             return self._cache[key]
         data = await self._adapter.get(key)
         if data is None:
             return None
         await self.update_cache({key: data})
         return data
 
-    async def get_all(self, keys: List[str]) -> Dict[str, bytes]:
+    async def get_many(self, *keys: str) -> Dict[str, bytes]:
+        key_list = list(keys)
         if self._adapter is None:
             raise Exception("Table not set")
         items: Dict[str, bytes] = {}
-        for key in tuple(keys):
+        for key in tuple(key_list):
             if key in self._cache:
                 items[key] = self._cache[key]
-                keys.remove(key)
-        if len(keys) == 0:
+                key_list.remove(key)
+        if len(key_list) == 0:
             return items
-        data = await self._adapter.get_all(keys)
+        data = await self._adapter.get_many(key_list)
         for key, value in data.items():
             items[key] = value
         await self.update_cache(items)
         return items
 
     async def add(self, items: Dict[str, bytes]) -> None:
         if self._adapter is None:
@@ -164,15 +165,15 @@
         await self._listeners.update(items)
         await self.update_cache(items)
         self.mark_changed()
 
     async def remove(self, keys: List[str]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
-        removed = await self._adapter.get_all(keys)
+        removed = await self._adapter.get_many(keys)
         await self._adapter.remove_all(keys)
         for key in keys:
             if key in self._cache:
                 del self._cache[key]
         await self._listeners.remove(removed)
         self.mark_changed()
```

### Comparing `omuserver-0.2.1/src/omuserver/extension/table/serialized_table.py` & `omuserver-0.2.2/src/omuserver/extension/table/serialized_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,20 @@
         if key in self._table.cache:
             return self._type.serializer.deserialize(self._table.cache[key])
         item = await self._table.get(key)
         if item is None:
             return None
         return self._type.serializer.deserialize(item)
 
+    async def get_many(self, *keys: str) -> Dict[str, T]:
+        items = await self._table.get_many(*keys)
+        return {
+            key: self._type.serializer.deserialize(item) for key, item in items.items()
+        }
+
     async def add(self, *items: T) -> None:
         data = {item.key(): self._type.serializer.serialize(item) for item in items}
         await self._table.add(data)
 
     async def update(self, *items: T) -> None:
         data = {item.key(): self._type.serializer.serialize(item) for item in items}
         await self._table.update(data)
```

### Comparing `omuserver-0.2.1/src/omuserver/extension/table/server_table.py` & `omuserver-0.2.2/src/omuserver/extension/table/server_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     @abc.abstractmethod
     async def store(self) -> None: ...
 
     @abc.abstractmethod
     async def get(self, key: str) -> bytes | None: ...
 
     @abc.abstractmethod
-    async def get_all(self, keys: List[str]) -> Dict[str, bytes]: ...
+    async def get_many(self, *keys: str) -> Dict[str, bytes]: ...
 
     @abc.abstractmethod
     async def add(self, items: Dict[str, bytes]) -> None: ...
 
     @abc.abstractmethod
     async def update(self, items: Dict[str, bytes]) -> None: ...
```

### Comparing `omuserver-0.2.1/src/omuserver/extension/table/session_table_handler.py` & `omuserver-0.2.2/src/omuserver/extension/table/session_table_handler.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/extension/table/table_extension.py` & `omuserver-0.2.2/src/omuserver/extension/table/table_extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Dict, List
 
 from omu.extension.table import Table, TableType
 from omu.extension.table.table_extension import (
-    TABLE_CONFIG_SET_PACKET,
+    TABLE_CONFIG_PACKET,
+    TABLE_FETCH_ALL_ENDPOINT,
+    TABLE_FETCH_ENDPOINT,
     TABLE_ITEM_ADD_PACKET,
     TABLE_ITEM_CLEAR_PACKET,
-    TABLE_ITEM_FETCH_ALL_ENDPOINT,
-    TABLE_ITEM_FETCH_ENDPOINT,
     TABLE_ITEM_GET_ENDPOINT,
     TABLE_ITEM_REMOVE_EVENT,
-    TABLE_ITEM_SIZE_ENDPOINT,
     TABLE_ITEM_UPDATE_PACKET,
     TABLE_LISTEN_PACKET,
-    TABLE_PROXY_ENDPOINT,
     TABLE_PROXY_LISTEN_PACKET,
     TABLE_PROXY_PACKET,
+    TABLE_SIZE_ENDPOINT,
     SetConfigReq,
     TableEventData,
     TableFetchReq,
     TableItemsData,
     TableKeysData,
     TableProxyData,
 )
@@ -40,62 +39,60 @@
 
 class TableExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
         self._tables: Dict[Identifier, ServerTable] = {}
         self._adapters: List[TableAdapter] = []
         server.packet_dispatcher.register(
-            TABLE_CONFIG_SET_PACKET,
+            TABLE_CONFIG_PACKET,
             TABLE_LISTEN_PACKET,
             TABLE_PROXY_LISTEN_PACKET,
             TABLE_PROXY_PACKET,
             TABLE_ITEM_ADD_PACKET,
             TABLE_ITEM_UPDATE_PACKET,
             TABLE_ITEM_REMOVE_EVENT,
             TABLE_ITEM_CLEAR_PACKET,
         )
         server.packet_dispatcher.add_packet_handler(
-            TABLE_CONFIG_SET_PACKET, self._on_table_set_config
+            TABLE_CONFIG_PACKET, self._on_table_set_config
         )
         server.packet_dispatcher.add_packet_handler(
             TABLE_LISTEN_PACKET, self._on_table_listen
         )
         server.packet_dispatcher.add_packet_handler(
             TABLE_PROXY_LISTEN_PACKET, self._on_table_proxy_listen
         )
         server.packet_dispatcher.add_packet_handler(
+            TABLE_PROXY_PACKET, self._on_table_proxy
+        )
+        server.packet_dispatcher.add_packet_handler(
             TABLE_ITEM_ADD_PACKET, self._on_table_item_add
         )
         server.packet_dispatcher.add_packet_handler(
             TABLE_ITEM_UPDATE_PACKET, self._on_table_item_update
         )
         server.packet_dispatcher.add_packet_handler(
             TABLE_ITEM_REMOVE_EVENT, self._on_table_item_remove
         )
         server.packet_dispatcher.add_packet_handler(
             TABLE_ITEM_CLEAR_PACKET, self._on_table_item_clear
         )
         server.endpoints.bind_endpoint(TABLE_ITEM_GET_ENDPOINT, self._on_table_item_get)
+        server.endpoints.bind_endpoint(TABLE_FETCH_ENDPOINT, self._on_table_item_fetch)
         server.endpoints.bind_endpoint(
-            TABLE_ITEM_FETCH_ENDPOINT, self._on_table_item_fetch
-        )
-        server.endpoints.bind_endpoint(
-            TABLE_ITEM_FETCH_ALL_ENDPOINT, self._on_table_item_fetch_all
-        )
-        server.endpoints.bind_endpoint(
-            TABLE_ITEM_SIZE_ENDPOINT, self._on_table_item_size
+            TABLE_FETCH_ALL_ENDPOINT, self._on_table_item_fetch_all
         )
-        server.endpoints.bind_endpoint(TABLE_PROXY_ENDPOINT, self._on_table_proxy)
+        server.endpoints.bind_endpoint(TABLE_SIZE_ENDPOINT, self._on_table_item_size)
         server.listeners.stop += self.on_server_stop
 
     async def _on_table_item_get(
         self, session: Session, req: TableKeysData
     ) -> TableItemsData:
         table = await self.get_table(req["type"])
-        items = await table.get_all(req["keys"])
+        items = await table.get_many(*req["keys"])
         return TableItemsData(
             type=req["type"],
             items=items,
         )
 
     async def _on_table_item_fetch(
         self, session: Session, req: TableFetchReq
@@ -135,18 +132,17 @@
         table = await self.get_table(type)
         table.attach_session(session)
 
     async def _on_table_proxy_listen(self, session: Session, type: str) -> None:
         table = await self.get_table(type)
         table.attach_proxy_session(session)
 
-    async def _on_table_proxy(self, session: Session, event: TableProxyData) -> int:
+    async def _on_table_proxy(self, session: Session, event: TableProxyData) -> None:
         table = await self.get_table(event["type"])
-        key = await table.proxy(session, event["key"], event["items"])
-        return key
+        await table.proxy(session, event["key"], event["items"])
 
     async def _on_table_item_add(self, session: Session, event: TableItemsData) -> None:
         table = await self.get_table(event["type"])
         await table.add(event["items"])
 
     async def _on_table_item_update(
         self, session: Session, event: TableItemsData
```

### Comparing `omuserver-0.2.1/src/omuserver/extension/table/adapters/sqlitetable.py` & `omuserver-0.2.2/src/omuserver/extension/table/adapters/sqlitetable.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     async def get(self, key: str) -> bytes | None:
         cursor = self._conn.execute("SELECT value FROM data WHERE key = ?", (key,))
         row = cursor.fetchone()
         if row is None:
             return None
         return row[0]
 
-    async def get_all(self, keys: list[str]) -> Dict[str, bytes]:
+    async def get_many(self, keys: list[str]) -> Dict[str, bytes]:
         cursor = self._conn.execute(
             f"SELECT key, value FROM data WHERE key IN ({','.join('?' for _ in keys)})",
             keys,
         )
         rows = cursor.fetchall()
         return {row[0]: row[1] for row in rows}
```

### Comparing `omuserver-0.2.1/src/omuserver/extension/table/adapters/tableadapter.py` & `omuserver-0.2.2/src/omuserver/extension/table/adapters/tableadapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     @abc.abstractmethod
     async def load(self): ...
 
     @abc.abstractmethod
     async def get(self, key: str) -> bytes | None: ...
 
     @abc.abstractmethod
-    async def get_all(self, keys: List[str]) -> Dict[str, bytes]: ...
+    async def get_many(self, keys: List[str]) -> Dict[str, bytes]: ...
 
     @abc.abstractmethod
     async def set(self, key: str, value: bytes) -> None: ...
 
     @abc.abstractmethod
     async def set_all(self, items: Mapping[str, bytes]) -> None: ...
```

### Comparing `omuserver-0.2.1/src/omuserver/network/network.py` & `omuserver-0.2.2/src/omuserver/network/network.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/network/packet_dispatcher.py` & `omuserver-0.2.2/src/omuserver/network/packet_dispatcher.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/security/security.py` & `omuserver-0.2.2/src/omuserver/security/security.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/server/omuserver.py` & `omuserver-0.2.2/src/omuserver/server/omuserver.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/server/server.py` & `omuserver-0.2.2/src/omuserver/server/server.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/session/aiohttp_connection.py` & `omuserver-0.2.2/src/omuserver/session/aiohttp_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/src/omuserver/session/session.py` & `omuserver-0.2.2/src/omuserver/session/session.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.1/pyproject.toml` & `omuserver-0.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuserver"
-version = "0.2.1"
+version = "0.2.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "sqlitedict>=2.1.0",
     "click>=8.1.7",
```

### Comparing `omuserver-0.2.1/PKG-INFO` & `omuserver-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omuserver
-Version: 0.2.1
+Version: 0.2.2
 Summary: Add your description here
 Author-email: am230 <111672334+am230@users.noreply.github.com>
 Requires-Python: >=3.12
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: aiosqlite>=0.19.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: loguru>=0.7.2
```

