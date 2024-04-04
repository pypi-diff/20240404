# Comparing `tmp/opentakserver-1.1.0.tar.gz` & `tmp/opentakserver-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentakserver-1.1.0.tar", max compression
+gzip compressed data, was "opentakserver-1.1.1.tar", max compression
```

## Comparing `opentakserver-1.1.0.tar` & `opentakserver-1.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.0/LICENSE
--rw-r--r--   0        0        0      128 2024-04-04 21:01:30.867409 opentakserver-1.1.0/opentakserver/__init__.py
--rw-r--r--   0        0        0    10612 2024-04-03 23:02:30.004021 opentakserver-1.1.0/opentakserver/app.py
--rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.0/opentakserver/blueprints/__init__.py
--rw-r--r--   0        0        0    41950 2024-04-04 15:04:49.420951 opentakserver-1.1.0/opentakserver/blueprints/api.py
--rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.0/opentakserver/blueprints/config.py
--rw-r--r--   0        0        0    26182 2024-04-04 14:24:20.109147 opentakserver-1.1.0/opentakserver/blueprints/marti.py
--rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.0/opentakserver/blueprints/ots_socketio.py
--rw-r--r--   0        0        0     4588 2024-02-29 22:51:03.042964 opentakserver-1.1.0/opentakserver/blueprints/scheduled_jobs.py
--rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.0/opentakserver/blueprints/scheduler_api.py
--rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.0/opentakserver/ca_config.py
--rw-r--r--   0        0        0    22887 2024-04-04 13:23:59.284952 opentakserver-1.1.0/opentakserver/certificate_authority.py
--rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.0/opentakserver/controllers/__init__.py
--rw-r--r--   0        0        0    10565 2024-04-03 18:07:25.951570 opentakserver-1.1.0/opentakserver/controllers/client_controller.py
--rw-r--r--   0        0        0    34898 2024-04-03 23:05:12.049517 opentakserver-1.1.0/opentakserver/controllers/cot_controller.py
--rw-r--r--   0        0        0     3983 2024-03-22 03:19:30.991223 opentakserver-1.1.0/opentakserver/defaultconfig.py
--rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.0/opentakserver/EmailValidator.py
--rw-r--r--   0        0        0      430 2024-03-22 02:45:11.460029 opentakserver-1.1.0/opentakserver/extensions.py
--rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.0/opentakserver/forms/__init__.py
--rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.0/opentakserver/forms/MediaMTXGlobalConfig.py
--rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.0/opentakserver/forms/MediaMTXPathConfig.py
--rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.0/opentakserver/functions.py
--rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.0/opentakserver/models/__init__.py
--rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.0/opentakserver/models/Alert.py
--rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.0/opentakserver/models/Base.py
--rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.0/opentakserver/models/CasEvac.py
--rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.0/opentakserver/models/Certificate.py
--rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.0/opentakserver/models/Chatrooms.py
--rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.0/opentakserver/models/ChatroomsUids.py
--rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.0/opentakserver/models/Config.py
--rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.0/opentakserver/models/CoT.py
--rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.0/opentakserver/models/DataPackage.py
--rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.0/opentakserver/models/EUD.py
--rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.0/opentakserver/models/GeoChat.py
--rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.0/opentakserver/models/Icon.py
--rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.0/opentakserver/models/Marker.py
--rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.0/opentakserver/models/Point.py
--rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.0/opentakserver/models/RBLine.py
--rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.0/opentakserver/models/role.py
--rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.0/opentakserver/models/Team.py
--rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.0/opentakserver/models/user.py
--rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.0/opentakserver/models/VideoRecording.py
--rw-r--r--   0        0        0     5476 2024-03-08 05:21:32.683056 opentakserver-1.1.0/opentakserver/models/VideoStream.py
--rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.0/opentakserver/models/WebAuthn.py
--rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.0/opentakserver/models/ZMIST.py
--rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.0/opentakserver/mumble/__init__.py
--rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.0/opentakserver/mumble/mumble_authenticator.py
--rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.0/opentakserver/mumble/mumble_ice_app.py
--rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.0/opentakserver/mumble/Murmur.ice
--rw-r--r--   0        0        0     3444 2024-03-21 14:16:06.218434 opentakserver-1.1.0/opentakserver/SocketServer.py
--rw-r--r--   0        0        0     1739 2024-04-04 21:01:30.860428 opentakserver-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1647 2024-02-02 04:47:28.605667 opentakserver-1.1.0/README.md
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 opentakserver-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.1/LICENSE
+-rw-r--r--   0        0        0      128 2024-04-04 21:44:21.774113 opentakserver-1.1.1/opentakserver/__init__.py
+-rw-r--r--   0        0        0    10612 2024-04-03 23:02:30.004021 opentakserver-1.1.1/opentakserver/app.py
+-rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.1/opentakserver/blueprints/__init__.py
+-rw-r--r--   0        0        0    41916 2024-04-04 21:36:33.553055 opentakserver-1.1.1/opentakserver/blueprints/api.py
+-rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.1/opentakserver/blueprints/config.py
+-rw-r--r--   0        0        0    26182 2024-04-04 14:24:20.109147 opentakserver-1.1.1/opentakserver/blueprints/marti.py
+-rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.1/opentakserver/blueprints/ots_socketio.py
+-rw-r--r--   0        0        0     4588 2024-02-29 22:51:03.042964 opentakserver-1.1.1/opentakserver/blueprints/scheduled_jobs.py
+-rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.1/opentakserver/blueprints/scheduler_api.py
+-rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.1/opentakserver/ca_config.py
+-rw-r--r--   0        0        0    22887 2024-04-04 13:23:59.284952 opentakserver-1.1.1/opentakserver/certificate_authority.py
+-rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.1/opentakserver/controllers/__init__.py
+-rw-r--r--   0        0        0    10565 2024-04-03 18:07:25.951570 opentakserver-1.1.1/opentakserver/controllers/client_controller.py
+-rw-r--r--   0        0        0    34898 2024-04-03 23:05:12.049517 opentakserver-1.1.1/opentakserver/controllers/cot_controller.py
+-rw-r--r--   0        0        0     3983 2024-03-22 03:19:30.991223 opentakserver-1.1.1/opentakserver/defaultconfig.py
+-rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.1/opentakserver/EmailValidator.py
+-rw-r--r--   0        0        0      430 2024-03-22 02:45:11.460029 opentakserver-1.1.1/opentakserver/extensions.py
+-rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.1/opentakserver/forms/__init__.py
+-rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.1/opentakserver/forms/MediaMTXGlobalConfig.py
+-rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.1/opentakserver/forms/MediaMTXPathConfig.py
+-rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.1/opentakserver/functions.py
+-rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.1/opentakserver/models/__init__.py
+-rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.1/opentakserver/models/Alert.py
+-rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.1/opentakserver/models/Base.py
+-rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.1/opentakserver/models/CasEvac.py
+-rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.1/opentakserver/models/Certificate.py
+-rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.1/opentakserver/models/Chatrooms.py
+-rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.1/opentakserver/models/ChatroomsUids.py
+-rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.1/opentakserver/models/Config.py
+-rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.1/opentakserver/models/CoT.py
+-rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.1/opentakserver/models/DataPackage.py
+-rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.1/opentakserver/models/EUD.py
+-rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.1/opentakserver/models/GeoChat.py
+-rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.1/opentakserver/models/Icon.py
+-rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.1/opentakserver/models/Marker.py
+-rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.1/opentakserver/models/Point.py
+-rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.1/opentakserver/models/RBLine.py
+-rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.1/opentakserver/models/role.py
+-rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.1/opentakserver/models/Team.py
+-rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.1/opentakserver/models/user.py
+-rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.1/opentakserver/models/VideoRecording.py
+-rw-r--r--   0        0        0     5476 2024-03-08 05:21:32.683056 opentakserver-1.1.1/opentakserver/models/VideoStream.py
+-rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.1/opentakserver/models/WebAuthn.py
+-rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.1/opentakserver/models/ZMIST.py
+-rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.1/opentakserver/mumble/__init__.py
+-rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.1/opentakserver/mumble/mumble_authenticator.py
+-rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.1/opentakserver/mumble/mumble_ice_app.py
+-rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.1/opentakserver/mumble/Murmur.ice
+-rw-r--r--   0        0        0     3444 2024-03-21 14:16:06.218434 opentakserver-1.1.1/opentakserver/SocketServer.py
+-rw-r--r--   0        0        0     1739 2024-04-04 21:44:21.765184 opentakserver-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1647 2024-02-02 04:47:28.605667 opentakserver-1.1.1/README.md
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 opentakserver-1.1.1/PKG-INFO
```

### Comparing `opentakserver-1.1.0/LICENSE` & `opentakserver-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/app.py` & `opentakserver-1.1.1/opentakserver/app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/blueprints/api.py` & `opentakserver-1.1.1/opentakserver/blueprints/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,17 +228,16 @@
                 return ({'success': False, 'error': 'Invalid username: {}'.format(username)}, 400,
                         {'Content-Type': 'application/json'})
 
             ca = CertificateAuthority(logger, app)
             filenames = ca.issue_certificate(username, False)
 
             for filename in filenames:
-                file_hash = hashlib.file_digest(
-                    open(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, filename),
-                         'rb'), 'sha256').hexdigest()
+                file_hash = hashlib.sha256(
+                    open(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, filename),'rb').read()).hexdigest()
 
                 data_package = DataPackage()
                 data_package.filename = filename
                 data_package.keywords = "public"
                 data_package.creator_uid = request.json['uid'] if 'uid' in request.json.keys() else str(uuid.uuid4())
                 data_package.submission_time = datetime.datetime.now()
                 data_package.mime_type = "application/x-zip-compressed"
```

### Comparing `opentakserver-1.1.0/opentakserver/blueprints/config.py` & `opentakserver-1.1.1/opentakserver/blueprints/config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/blueprints/marti.py` & `opentakserver-1.1.1/opentakserver/blueprints/marti.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/blueprints/ots_socketio.py` & `opentakserver-1.1.1/opentakserver/blueprints/ots_socketio.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/blueprints/scheduled_jobs.py` & `opentakserver-1.1.1/opentakserver/blueprints/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/blueprints/scheduler_api.py` & `opentakserver-1.1.1/opentakserver/blueprints/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/ca_config.py` & `opentakserver-1.1.1/opentakserver/ca_config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/certificate_authority.py` & `opentakserver-1.1.1/opentakserver/certificate_authority.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/controllers/client_controller.py` & `opentakserver-1.1.1/opentakserver/controllers/client_controller.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/controllers/cot_controller.py` & `opentakserver-1.1.1/opentakserver/controllers/cot_controller.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/defaultconfig.py` & `opentakserver-1.1.1/opentakserver/defaultconfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/EmailValidator.py` & `opentakserver-1.1.1/opentakserver/EmailValidator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/forms/MediaMTXGlobalConfig.py` & `opentakserver-1.1.1/opentakserver/forms/MediaMTXGlobalConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/forms/MediaMTXPathConfig.py` & `opentakserver-1.1.1/opentakserver/forms/MediaMTXPathConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/Alert.py` & `opentakserver-1.1.1/opentakserver/models/Alert.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/CasEvac.py` & `opentakserver-1.1.1/opentakserver/models/CasEvac.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/Certificate.py` & `opentakserver-1.1.1/opentakserver/models/Certificate.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/Chatrooms.py` & `opentakserver-1.1.1/opentakserver/models/Chatrooms.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/ChatroomsUids.py` & `opentakserver-1.1.1/opentakserver/models/ChatroomsUids.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/CoT.py` & `opentakserver-1.1.1/opentakserver/models/CoT.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/DataPackage.py` & `opentakserver-1.1.1/opentakserver/models/DataPackage.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/EUD.py` & `opentakserver-1.1.1/opentakserver/models/EUD.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/GeoChat.py` & `opentakserver-1.1.1/opentakserver/models/GeoChat.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/Icon.py` & `opentakserver-1.1.1/opentakserver/models/Icon.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/Marker.py` & `opentakserver-1.1.1/opentakserver/models/Marker.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/Point.py` & `opentakserver-1.1.1/opentakserver/models/Point.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/RBLine.py` & `opentakserver-1.1.1/opentakserver/models/RBLine.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/Team.py` & `opentakserver-1.1.1/opentakserver/models/Team.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/user.py` & `opentakserver-1.1.1/opentakserver/models/user.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/VideoRecording.py` & `opentakserver-1.1.1/opentakserver/models/VideoRecording.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/VideoStream.py` & `opentakserver-1.1.1/opentakserver/models/VideoStream.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/models/ZMIST.py` & `opentakserver-1.1.1/opentakserver/models/ZMIST.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/mumble/mumble_authenticator.py` & `opentakserver-1.1.1/opentakserver/mumble/mumble_authenticator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/mumble/mumble_ice_app.py` & `opentakserver-1.1.1/opentakserver/mumble/mumble_ice_app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/mumble/Murmur.ice` & `opentakserver-1.1.1/opentakserver/mumble/Murmur.ice`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/opentakserver/SocketServer.py` & `opentakserver-1.1.1/opentakserver/SocketServer.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/pyproject.toml` & `opentakserver-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentakserver"
-version = "1.1.0"
+version = "1.1.1"
 description = "A server for ATAK, WinTAK, and iTAK"
 authors = ["OpenTAKServer <opentakserver@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/brian7704/OpenTAKServer"
 documentation = "https://docs.opentakserver.io"
```

### Comparing `opentakserver-1.1.0/README.md` & `opentakserver-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.0/PKG-INFO` & `opentakserver-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentakserver
-Version: 1.1.0
+Version: 1.1.1
 Summary: A server for ATAK, WinTAK, and iTAK
 Home-page: https://github.com/brian7704/OpenTAKServer
 License: GPL-3.0-or-later
 Author: OpenTAKServer
 Author-email: opentakserver@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

