# Comparing `tmp/linkai-0.0.3.5-py3-none-any.whl.zip` & `tmp/linkai-0.0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4888 bytes, number of entries: 10
+Zip file size: 4942 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      111 b- defN 24-Jan-06 15:46 linkai/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/_common/__init__.py
 -rw-r--r--  2.0 unx      714 b- defN 24-Jan-29 04:16 linkai/_common/log.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/api/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-06 15:25 linkai/api/client/__init__.py
--rw-r--r--  2.0 unx     8743 b- defN 24-Feb-19 05:18 linkai/api/client/client.py
--rw-r--r--  2.0 unx      516 b- defN 24-Feb-19 05:28 linkai-0.0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-19 05:28 linkai-0.0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Feb-19 05:28 linkai-0.0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      774 b- defN 24-Feb-19 05:28 linkai-0.0.3.5.dist-info/RECORD
-10 files, 10957 bytes uncompressed, 3556 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx     9072 b- defN 24-Apr-04 15:36 linkai/api/client/client.py
+-rw-r--r--  2.0 unx      516 b- defN 24-Apr-04 16:43 linkai-0.0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 16:43 linkai-0.0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-04 16:43 linkai-0.0.3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      774 b- defN 24-Apr-04 16:43 linkai-0.0.3.6.dist-info/RECORD
+10 files, 11286 bytes uncompressed, 3610 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: linkai/api/client/__init__.py
 Comment: 
 
 Filename: linkai/api/client/client.py
 Comment: 
 
-Filename: linkai-0.0.3.5.dist-info/METADATA
+Filename: linkai-0.0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: linkai-0.0.3.5.dist-info/WHEEL
+Filename: linkai-0.0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: linkai-0.0.3.5.dist-info/top_level.txt
+Filename: linkai-0.0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: linkai-0.0.3.5.dist-info/RECORD
+Filename: linkai-0.0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## linkai/api/client/client.py

```diff
@@ -19,14 +19,15 @@
     LOGIN = "LOGIN"
     CONFIG = "CONFIG"
     PUSH = "PUSH"
     HEARTBEAT = "HEARTBEAT"
     CHANNEL_LOGIN = "CHANNEL_LOGIN"
     CHANNEL_LOGOUT = "CHANNEL_LOGOUT"
     CHANNEL_QRCODE = "CHANNEL_QRCODE"
+    LOCAL_CONFIG = "LOCAL_CONFIG"
 
     def __str__(self):
         return self.name
 
 
 class PushMsg:
     def __init__(self, session_id: str, msg_content: str, is_group: bool = False):
@@ -51,14 +52,15 @@
         self.socket = None
         self.connected = False
         self.connect_failed_times = 0
         self.heartbeat_interval = heartbeat_interval
         self.reconnect_times = reconnect_times
         self.reconnect_interval = reconnect_interval
         self.need_connect = True
+        self.config = {}
 
     def on_message(self, push_msg: PushMsg):
         """
         client push msg callback
         :param push_msg: manual push msg
         :return:
         """
@@ -145,14 +147,20 @@
 
     def send_qrcode(self, urls: list):
         if self.client_id:
             msg = self._build_package(ClientMsgType.CHANNEL_QRCODE)
             msg["data"]["qrcodeUrls"] = urls
             self._send_package(msg)
 
+    def _send_local_config(self):
+        if self.client_id and self.config:
+            msg = self._build_package(ClientMsgType.LOCAL_CONFIG)
+            msg["data"]["config"] = self.config
+            self._send_package(msg)
+
     def _build_package(self, msg_type: ClientMsgType):
         data = {
             "apiKey": self.api_key,
             "clientType": self.client_type,
             "clientId": self.client_id
         }
         msg = {
@@ -240,14 +248,15 @@
                     client_id = msg.get("data").get("clientId")
                     self.client_id = client_id
                     self.save_client_id(client_id)
                 config = msg.get("data").get("config")
                 if config:
                     self.on_config(config)
                 logger.info(f"Client login success")
+                self._send_local_config()
             elif msg.get("code") == 409:
                 logger.info(f"Client no need connect, ignore")
                 self.need_connect = False
                 self.socket.close()
             else:
                 logger.warn(f"Client login failed, res={msg}")
```

## Comparing `linkai-0.0.3.5.dist-info/METADATA` & `linkai-0.0.3.6.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkai
-Version: 0.0.3.5
+Version: 0.0.3.6
 Summary: LinkAI python sdk
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `linkai-0.0.3.5.dist-info/RECORD` & `linkai-0.0.3.6.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 linkai/__init__.py,sha256=JSbbcxuUYRUgT4EP-m3WKukCjakcoQJnJtsLlxUTKCY,111
 linkai/_common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 linkai/_common/log.py,sha256=RSAy3N5t_Rn0yoQU3-4-kurEZA6cANCMGiQgv0FSgfA,714
 linkai/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 linkai/api/client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-linkai/api/client/client.py,sha256=zQkpMMOk-8ciqtaIbRuUh68lkrlE3LAE0W_MzaKT9o4,8743
-linkai-0.0.3.5.dist-info/METADATA,sha256=YBfZ4yXO0OWtJ8En8ObR_ONc27CkCDXEuNBo203s7KI,516
-linkai-0.0.3.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-linkai-0.0.3.5.dist-info/top_level.txt,sha256=6gMseb-hjwjOWwaqKNCqTQzpa7ZQROxu4VUkP2JbT5g,7
-linkai-0.0.3.5.dist-info/RECORD,,
+linkai/api/client/client.py,sha256=DexKbkysmr5nofm5QPApMu8wo8OMLW_oOcq973IQmnI,9072
+linkai-0.0.3.6.dist-info/METADATA,sha256=jzhPSYGxAGVhmDoQRa1m4lniLqB2zTYJ4CwajezdPnk,516
+linkai-0.0.3.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+linkai-0.0.3.6.dist-info/top_level.txt,sha256=6gMseb-hjwjOWwaqKNCqTQzpa7ZQROxu4VUkP2JbT5g,7
+linkai-0.0.3.6.dist-info/RECORD,,
```

