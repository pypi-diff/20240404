# Comparing `tmp/omu-0.2.0.tar.gz` & `tmp/omu-0.2.1.tar.gz`

## Comparing `omu-0.2.0.tar` & `omu-0.2.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 omu-0.2.0/.gitattributes
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omu-0.2.0/.prettierrc
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omu-0.2.0/.python-version
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 omu-0.2.0/run_client.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/__init__.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/app.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/event_emitter.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/helper.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/identifier.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/model.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/plugin.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/serializer.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/client/__init__.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/client/client.py
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/client/omuclient.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/extension.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/extension_manager.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/asset/__init__.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/asset/asset_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/dashboard/dashboard.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/endpoint/endpoint.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/message/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/message/message.py
--rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/message/message_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/permission/__init__.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/permission/permission.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/permission/permission_extension.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/registry/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/registry/registry.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/registry/registry_extension.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/server/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/server/server_extension.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/table/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/table/table.py
--rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/extension/table/table_extension.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/interface/__init__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/interface/keyable.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/interface/named.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/address.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/bytebuffer.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/connection.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/network.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/packet_mapper.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/websocket_connection.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/packet/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/packet/packet.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.0/src/omu/network/packet/packet_types.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omu-0.2.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.0/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 omu-0.2.1/.gitattributes
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omu-0.2.1/.prettierrc
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omu-0.2.1/.python-version
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 omu-0.2.1/run_client.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/__init__.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/app.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/event_emitter.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/helper.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/identifier.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/model.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/plugin.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/serializer.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/client/__init__.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/client/client.py
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/client/omuclient.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/extension.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/extension_manager.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/asset/__init__.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/dashboard/dashboard.py
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/endpoint/endpoint.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/message/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/message/message.py
+-rw-r--r--   0        0        0     3330 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/message/message_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/permission/__init__.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/permission/permission.py
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/registry/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/registry/registry.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/server/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/server/server_extension.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/table/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/table/table.py
+-rw-r--r--   0        0        0    15094 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/extension/table/table_extension.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/interface/__init__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/interface/keyable.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/interface/named.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/address.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/bytebuffer.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/connection.py
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/network.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/packet_mapper.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/websocket_connection.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/packet/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/packet/packet.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.1/src/omu/network/packet/packet_types.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omu-0.2.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.1/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.1/PKG-INFO
```

### Comparing `omu-0.2.0/run_client.py` & `omu-0.2.1/run_client.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/app.py` & `omu-0.2.1/src/omu/app.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/event_emitter.py` & `omu-0.2.1/src/omu/event_emitter.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/helper.py` & `omu-0.2.1/src/omu/helper.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/identifier.py` & `omu-0.2.1/src/omu/identifier.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/serializer.py` & `omu-0.2.1/src/omu/serializer.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/client/client.py` & `omu-0.2.1/src/omu/client/client.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/client/omuclient.py` & `omu-0.2.1/src/omu/client/omuclient.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/extension.py` & `omu-0.2.1/src/omu/extension/extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/extension_manager.py` & `omu-0.2.1/src/omu/extension/extension_manager.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/asset/asset_extension.py` & `omu-0.2.1/src/omu/extension/asset/asset_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/dashboard/dashboard.py` & `omu-0.2.1/src/omu/extension/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/dashboard/dashboard_extension.py` & `omu-0.2.1/src/omu/extension/dashboard/dashboard_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/endpoint/endpoint.py` & `omu-0.2.1/src/omu/extension/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/endpoint/endpoint_extension.py` & `omu-0.2.1/src/omu/extension/endpoint/endpoint_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/message/message.py` & `omu-0.2.1/src/omu/extension/message/message.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/message/message_extension.py` & `omu-0.2.1/src/omu/extension/message/message_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/permission/permission.py` & `omu-0.2.1/src/omu/extension/permission/permission.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/permission/permission_extension.py` & `omu-0.2.1/src/omu/extension/permission/permission_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/plugin/plugin_extension.py` & `omu-0.2.1/src/omu/extension/plugin/plugin_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/registry/registry.py` & `omu-0.2.1/src/omu/extension/registry/registry.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/registry/registry_extension.py` & `omu-0.2.1/src/omu/extension/registry/registry_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/server/server_extension.py` & `omu-0.2.1/src/omu/extension/server/server_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/table/table.py` & `omu-0.2.1/src/omu/extension/table/table.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/extension/table/table_extension.py` & `omu-0.2.1/src/omu/extension/table/table_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/network/bytebuffer.py` & `omu-0.2.1/src/omu/network/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/network/connection.py` & `omu-0.2.1/src/omu/network/connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/network/network.py` & `omu-0.2.1/src/omu/network/network.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/network/packet_mapper.py` & `omu-0.2.1/src/omu/network/packet_mapper.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/network/websocket_connection.py` & `omu-0.2.1/src/omu/network/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/network/packet/packet.py` & `omu-0.2.1/src/omu/network/packet/packet.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/src/omu/network/packet/packet_types.py` & `omu-0.2.1/src/omu/network/packet/packet_types.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.0/pyproject.toml` & `omu-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omu"
-version = "0.2.0"
+version = "0.2.1"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["loguru>=0.7.2"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

