# Comparing `tmp/opentakserver-1.0.1.tar.gz` & `tmp/opentakserver-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentakserver-1.0.1.tar", max compression
+gzip compressed data, was "opentakserver-1.1.0.tar", max compression
```

## Comparing `opentakserver-1.0.1.tar` & `opentakserver-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.0.1/LICENSE
--rw-r--r--   0        0        0      128 2024-03-29 17:32:09.213578 opentakserver-1.0.1/opentakserver/__init__.py
--rw-r--r--   0        0        0    10612 2024-03-28 15:08:51.810830 opentakserver-1.0.1/opentakserver/app.py
--rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.0.1/opentakserver/blueprints/__init__.py
--rw-r--r--   0        0        0    41543 2024-03-28 01:12:23.504315 opentakserver-1.0.1/opentakserver/blueprints/api.py
--rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.0.1/opentakserver/blueprints/config.py
--rw-r--r--   0        0        0    23224 2024-03-21 12:57:40.876747 opentakserver-1.0.1/opentakserver/blueprints/marti.py
--rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.0.1/opentakserver/blueprints/ots_socketio.py
--rw-r--r--   0        0        0     4588 2024-02-29 22:51:03.042964 opentakserver-1.0.1/opentakserver/blueprints/scheduled_jobs.py
--rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.0.1/opentakserver/blueprints/scheduler_api.py
--rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.0.1/opentakserver/ca_config.py
--rw-r--r--   0        0        0    20675 2024-03-27 20:06:53.804193 opentakserver-1.0.1/opentakserver/certificate_authority.py
--rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.0.1/opentakserver/controllers/__init__.py
--rw-r--r--   0        0        0     9877 2024-02-23 20:27:29.614744 opentakserver-1.0.1/opentakserver/controllers/client_controller.py
--rw-r--r--   0        0        0    34602 2024-03-26 20:47:05.986468 opentakserver-1.0.1/opentakserver/controllers/cot_controller.py
--rw-r--r--   0        0        0     3983 2024-03-22 03:19:30.991223 opentakserver-1.0.1/opentakserver/defaultconfig.py
--rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.0.1/opentakserver/EmailValidator.py
--rw-r--r--   0        0        0      430 2024-03-22 02:45:11.460029 opentakserver-1.0.1/opentakserver/extensions.py
--rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.0.1/opentakserver/forms/__init__.py
--rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.0.1/opentakserver/forms/MediaMTXGlobalConfig.py
--rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.0.1/opentakserver/forms/MediaMTXPathConfig.py
--rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.0.1/opentakserver/functions.py
--rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.0.1/opentakserver/models/__init__.py
--rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.0.1/opentakserver/models/Alert.py
--rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.0.1/opentakserver/models/Base.py
--rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.0.1/opentakserver/models/CasEvac.py
--rw-r--r--   0        0        0     2380 2024-01-25 16:00:51.701353 opentakserver-1.0.1/opentakserver/models/Certificate.py
--rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.0.1/opentakserver/models/Chatrooms.py
--rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.0.1/opentakserver/models/ChatroomsUids.py
--rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.0.1/opentakserver/models/Config.py
--rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.0.1/opentakserver/models/CoT.py
--rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.0.1/opentakserver/models/DataPackage.py
--rw-r--r--   0        0        0     3682 2024-03-20 13:22:31.542807 opentakserver-1.0.1/opentakserver/models/EUD.py
--rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.0.1/opentakserver/models/GeoChat.py
--rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.0.1/opentakserver/models/Icon.py
--rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.0.1/opentakserver/models/Marker.py
--rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.0.1/opentakserver/models/Point.py
--rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.0.1/opentakserver/models/RBLine.py
--rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.0.1/opentakserver/models/role.py
--rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.0.1/opentakserver/models/Team.py
--rw-r--r--   0        0        0     1158 2024-03-22 02:58:09.177612 opentakserver-1.0.1/opentakserver/models/user.py
--rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.0.1/opentakserver/models/VideoRecording.py
--rw-r--r--   0        0        0     5476 2024-03-08 05:21:32.683056 opentakserver-1.0.1/opentakserver/models/VideoStream.py
--rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.0.1/opentakserver/models/WebAuthn.py
--rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.0.1/opentakserver/models/ZMIST.py
--rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.0.1/opentakserver/mumble/__init__.py
--rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.0.1/opentakserver/mumble/mumble_authenticator.py
--rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.0.1/opentakserver/mumble/mumble_ice_app.py
--rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.0.1/opentakserver/mumble/Murmur.ice
--rw-r--r--   0        0        0     3444 2024-03-21 14:16:06.218434 opentakserver-1.0.1/opentakserver/SocketServer.py
--rw-r--r--   0        0        0     1739 2024-03-29 17:32:09.202610 opentakserver-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1647 2024-02-02 04:47:28.605667 opentakserver-1.0.1/README.md
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 opentakserver-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.0/LICENSE
+-rw-r--r--   0        0        0      128 2024-04-04 21:01:30.867409 opentakserver-1.1.0/opentakserver/__init__.py
+-rw-r--r--   0        0        0    10612 2024-04-03 23:02:30.004021 opentakserver-1.1.0/opentakserver/app.py
+-rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.0/opentakserver/blueprints/__init__.py
+-rw-r--r--   0        0        0    41950 2024-04-04 15:04:49.420951 opentakserver-1.1.0/opentakserver/blueprints/api.py
+-rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.0/opentakserver/blueprints/config.py
+-rw-r--r--   0        0        0    26182 2024-04-04 14:24:20.109147 opentakserver-1.1.0/opentakserver/blueprints/marti.py
+-rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.0/opentakserver/blueprints/ots_socketio.py
+-rw-r--r--   0        0        0     4588 2024-02-29 22:51:03.042964 opentakserver-1.1.0/opentakserver/blueprints/scheduled_jobs.py
+-rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.0/opentakserver/blueprints/scheduler_api.py
+-rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.0/opentakserver/ca_config.py
+-rw-r--r--   0        0        0    22887 2024-04-04 13:23:59.284952 opentakserver-1.1.0/opentakserver/certificate_authority.py
+-rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.0/opentakserver/controllers/__init__.py
+-rw-r--r--   0        0        0    10565 2024-04-03 18:07:25.951570 opentakserver-1.1.0/opentakserver/controllers/client_controller.py
+-rw-r--r--   0        0        0    34898 2024-04-03 23:05:12.049517 opentakserver-1.1.0/opentakserver/controllers/cot_controller.py
+-rw-r--r--   0        0        0     3983 2024-03-22 03:19:30.991223 opentakserver-1.1.0/opentakserver/defaultconfig.py
+-rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.0/opentakserver/EmailValidator.py
+-rw-r--r--   0        0        0      430 2024-03-22 02:45:11.460029 opentakserver-1.1.0/opentakserver/extensions.py
+-rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.0/opentakserver/forms/__init__.py
+-rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.0/opentakserver/forms/MediaMTXGlobalConfig.py
+-rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.0/opentakserver/forms/MediaMTXPathConfig.py
+-rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.0/opentakserver/functions.py
+-rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.0/opentakserver/models/__init__.py
+-rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.0/opentakserver/models/Alert.py
+-rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.0/opentakserver/models/Base.py
+-rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.0/opentakserver/models/CasEvac.py
+-rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.0/opentakserver/models/Certificate.py
+-rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.0/opentakserver/models/Chatrooms.py
+-rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.0/opentakserver/models/ChatroomsUids.py
+-rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.0/opentakserver/models/Config.py
+-rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.0/opentakserver/models/CoT.py
+-rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.0/opentakserver/models/DataPackage.py
+-rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.0/opentakserver/models/EUD.py
+-rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.0/opentakserver/models/GeoChat.py
+-rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.0/opentakserver/models/Icon.py
+-rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.0/opentakserver/models/Marker.py
+-rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.0/opentakserver/models/Point.py
+-rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.0/opentakserver/models/RBLine.py
+-rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.0/opentakserver/models/role.py
+-rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.0/opentakserver/models/Team.py
+-rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.0/opentakserver/models/user.py
+-rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.0/opentakserver/models/VideoRecording.py
+-rw-r--r--   0        0        0     5476 2024-03-08 05:21:32.683056 opentakserver-1.1.0/opentakserver/models/VideoStream.py
+-rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.0/opentakserver/models/WebAuthn.py
+-rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.0/opentakserver/models/ZMIST.py
+-rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.0/opentakserver/mumble/__init__.py
+-rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.0/opentakserver/mumble/mumble_authenticator.py
+-rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.0/opentakserver/mumble/mumble_ice_app.py
+-rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.0/opentakserver/mumble/Murmur.ice
+-rw-r--r--   0        0        0     3444 2024-03-21 14:16:06.218434 opentakserver-1.1.0/opentakserver/SocketServer.py
+-rw-r--r--   0        0        0     1739 2024-04-04 21:01:30.860428 opentakserver-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1647 2024-02-02 04:47:28.605667 opentakserver-1.1.0/README.md
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 opentakserver-1.1.0/PKG-INFO
```

### Comparing `opentakserver-1.0.1/LICENSE` & `opentakserver-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/app.py` & `opentakserver-1.1.0/opentakserver/app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/blueprints/api.py` & `opentakserver-1.1.0/opentakserver/blueprints/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,82 +211,82 @@
     else:
         return jsonify({'success': False, 'error': 'Valid actions are start and stop'}), 400
 
 
 @api_blueprint.route("/api/certificate", methods=['GET', 'POST'])
 @auth_required()
 def certificate():
-    if request.method == 'POST' and 'callsign' in request.json.keys() and 'uid' in request.json.keys():
+    if request.method == 'POST' and 'username' in request.json.keys():
         try:
-            callsign = bleach.clean(request.json.get('callsign'))
+            username = bleach.clean(request.json.get('username'))
             truststore_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', "opentakserver", "truststore-root.p12")
-            user_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', callsign,
-                                         "{}.p12".format(callsign))
+            user_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username,
+                                         "{}.p12".format(username))
 
-            eud = db.session.execute(db.session.query(EUD).where(EUD.callsign == callsign)).first()
+            user = app.security.datastore.find_user(username=username)
 
-            if not eud:
-                return ({'success': False, 'error': 'Invalid callsign: {}'.format(callsign)}, 400,
+            if not user:
+                return ({'success': False, 'error': 'Invalid username: {}'.format(username)}, 400,
                         {'Content-Type': 'application/json'})
 
-            eud = eud[0]
-
             ca = CertificateAuthority(logger, app)
-            filename = ca.issue_certificate(callsign, False)
+            filenames = ca.issue_certificate(username, False)
 
-            file_hash = hashlib.file_digest(open(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', callsign, filename),
-                                                 'rb'), 'sha256').hexdigest()
+            for filename in filenames:
+                file_hash = hashlib.file_digest(
+                    open(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, filename),
+                         'rb'), 'sha256').hexdigest()
+
+                data_package = DataPackage()
+                data_package.filename = filename
+                data_package.keywords = "public"
+                data_package.creator_uid = request.json['uid'] if 'uid' in request.json.keys() else str(uuid.uuid4())
+                data_package.submission_time = datetime.datetime.now()
+                data_package.mime_type = "application/x-zip-compressed"
+                data_package.size = os.path.getsize(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, filename))
+                data_package.hash = file_hash
+                data_package.submission_user = current_user.id
 
-            data_package = DataPackage()
-            data_package.filename = filename
-            data_package.keywords = "public"
-            data_package.creator_uid = request.json['uid']
-            data_package.submission_time = datetime.datetime.now()
-            data_package.mime_type = "application/x-zip-compressed"
-            data_package.size = os.path.getsize(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', callsign, filename))
-            data_package.hash = file_hash
-            data_package.submission_user = current_user.id
+                try:
+                    db.session.add(data_package)
+                    db.session.commit()
+                except sqlalchemy.exc.IntegrityError as e:
+                    db.session.rollback()
+                    logger.error(e)
+                    return ({'success': False, 'error': 'Certificate already exists for {}'.format(username)}, 400,
+                            {'Content-Type': 'application/json'})
+
+                copyfile(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, "{}".format(filename)),
+                         os.path.join(app.config.get("UPLOAD_FOLDER"), "{}.zip".format(file_hash)))
+
+                cert = Certificate()
+                cert.common_name = username
+                cert.username = username
+                cert.expiration_date = datetime.datetime.today() + datetime.timedelta(days=app.config.get("OTS_CA_EXPIRATION_TIME"))
+                cert.server_address = urlparse(request.url_root).hostname
+                cert.server_port = app.config.get("OTS_SSL_STREAMING_PORT")
+                cert.truststore_filename = truststore_filename
+                cert.user_cert_filename = user_filename
+                cert.cert_password = app.config.get("OTS_CA_PASSWORD")
+                cert.data_package_id = data_package.id if data_package else None
 
-            try:
-                db.session.add(data_package)
+                db.session.add(cert)
                 db.session.commit()
-            except sqlalchemy.exc.IntegrityError as e:
-                db.session.rollback()
-                logger.error(e)
-                return ({'success': False, 'error': 'Certificate already exists for {}'.format(callsign)}, 400,
-                        {'Content-Type': 'application/json'})
-
-            copyfile(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', callsign, "{}_CONFIG.zip".format(callsign)),
-                     os.path.join(app.config.get("UPLOAD_FOLDER"), "{}.zip".format(file_hash)))
-
-            cert = Certificate()
-            cert.common_name = callsign
-            cert.callsign = callsign
-            cert.expiration_date = datetime.datetime.today() + datetime.timedelta(days=app.config.get("OTS_CA_EXPIRATION_TIME"))
-            cert.server_address = urlparse(request.url_root).hostname
-            cert.server_port = app.config.get("OTS_SSL_STREAMING_PORT")
-            cert.truststore_filename = truststore_filename
-            cert.user_cert_filename = user_filename
-            cert.cert_password = app.config.get("OTS_CA_PASSWORD")
-            cert.data_package_id = data_package.id
-            cert.eud_uid = eud.uid
-
-            db.session.add(cert)
-            db.session.commit()
 
             return {'success': True}, 200, {'Content-Type': 'application/json'}
         except BaseException as e:
             logger.error(traceback.format_exc())
             return {'success': False, 'error': str(e)}, 500, {'Content-Type': 'application/json'}
     elif request.method == 'POST':
         return ({'success': False, 'error': "Please specify a callsign"}, 400,
                 {'Content-Type': 'application/json'})
     elif request.method == 'GET':
         query = db.session.query(Certificate)
         query = search(query, Certificate, 'callsign')
+        query = search(query, Certificate, 'username')
 
         return paginate(query)
 
 
 @api_blueprint.route('/api/me')
 @auth_required()
 def me():
@@ -318,15 +318,15 @@
         db.session.delete(data_package[0])
         db.session.commit()
         os.remove(os.path.join(app.config.get("UPLOAD_FOLDER"), "{}.zip".format(data_package[0].hash)))
 
         if data_package[0].certificate:
             Certificate.query.filter_by(id=data_package[0].certificate.id).delete()
             db.session.commit()
-            shutil.rmtree(os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", data_package[0].eud.callsign), ignore_errors=True)
+            shutil.rmtree(os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", data_package[0].certificate.common_name), ignore_errors=True)
     except BaseException as e:
         logger.error("Failed to delete data package")
         logger.error(traceback.format_exc())
         return jsonify({'success': False, 'error': str(e)}), 500
 
     return jsonify({'success': True})
 
@@ -1038,7 +1038,14 @@
 def get_icon():
     query = db.session.query(Icon)
     query = search(query, Icon, 'filename')
     query = search(query, Icon, 'groupName')
     query = search(query, Icon, 'type2525b')
 
     return paginate(query)
+
+
+@api_blueprint.route('/api/itak_qr_string')
+@auth_required()
+def get_settings():
+    url = urlparse(request.url_root).hostname
+    return "OpenTAKServer_{},{},{},SSL".format(url, url, app.config.get("OTS_SSL_STREAMING_PORT"))
```

### Comparing `opentakserver-1.0.1/opentakserver/blueprints/config.py` & `opentakserver-1.1.0/opentakserver/blueprints/config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/blueprints/marti.py` & `opentakserver-1.1.0/opentakserver/blueprints/marti.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,43 +105,49 @@
 @marti_blueprint.route('/Marti/api/tls/signClient/v2', methods=['POST'])
 def sign_csr_v2():
     if not basic_auth(request.headers.get('Authorization')):
         return '', 401
 
     try:
         uid = request.args.get("clientUid")
-        csr = '-----BEGIN CERTIFICATE REQUEST-----\n' + request.data.decode(
-            'utf-8') + '-----END CERTIFICATE REQUEST-----'
+
+        if "iTAK" not in request.user_agent.string:
+            csr = '-----BEGIN CERTIFICATE REQUEST-----\n' + request.data.decode(
+                'utf-8') + '-----END CERTIFICATE REQUEST-----'
+        else:
+            csr = request.data.decode('utf-8')
 
         x509 = crypto.load_certificate_request(crypto.FILETYPE_PEM, csr.encode())
         common_name = x509.get_subject().CN
         logger.debug("Attempting to sign CSR for {}".format(common_name))
 
         cert_authority = CertificateAuthority(logger, app)
 
         signed_csr = cert_authority.sign_csr(csr.encode(), common_name, False).decode("utf-8")
         signed_csr = signed_csr.replace("-----BEGIN CERTIFICATE-----\n", "")
         signed_csr = signed_csr.replace("\n-----END CERTIFICATE-----\n", "")
 
-        enrollment = Element('enrollment')
-        signed_cert = SubElement(enrollment, 'signedCert')
-        signed_cert.text = signed_csr
-        ca = SubElement(enrollment, 'ca')
-
         f = open(os.path.join(app.config.get("OTS_CA_FOLDER"), "ca.pem"), 'r')
         cert = f.read()
         f.close()
 
         cert = cert.replace("-----BEGIN CERTIFICATE-----\n", "")
         cert = cert.replace("\n-----END CERTIFICATE-----\n", "")
 
-        ca.text = cert
+        if "iTAK" in request.user_agent.string:
+            response = {'signedCert': signed_csr, 'ca0': cert, 'ca1': cert}
+        else:
+            enrollment = Element('enrollment')
+            signed_cert = SubElement(enrollment, 'signedCert')
+            signed_cert.text = signed_csr
+            ca = SubElement(enrollment, 'ca')
+            ca.text = cert
 
-        response = tostring(enrollment).decode('utf-8')
-        response = '<?xml version="1.0" encoding="UTF-8"?>\n' + response
+            response = tostring(enrollment).decode('utf-8')
+            response = '<?xml version="1.0" encoding="UTF-8"?>\n' + response
 
         username, password = base64.b64decode(
             request.headers.get("Authorization").split(" ")[-1].encode('utf-8')).decode(
             'utf-8').split(":")
         username = bleach.clean(username)
         user = app.security.datastore.find_user(username=username)
 
@@ -190,15 +196,18 @@
             certificate.user_cert_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", common_name,
                                                           common_name + ".pem")
             certificate.csr = os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", common_name, common_name + ".csr")
             certificate.cert_password = app.config.get("OTS_CA_PASSWORD")
 
             db.session.commit()
 
-        return response, 200, {'Content-Type': 'application/xml', 'Content-Encoding': 'charset=UTF-8'}
+        if "iTAK" in request.user_agent.string:
+            return response, 200, {'Content-Type': 'text/plain', 'Content-Encoding': 'charset=UTF-8'}
+        else:
+            return response, 200, {'Content-Type': 'application/xml', 'Content-Encoding': 'charset=UTF-8'}
     except BaseException as e:
         logger.error(traceback.format_exc())
         return jsonify({'error': str(e)}), 500
 
 
 @marti_blueprint.route('/Marti/api/version/config', methods=['GET'])
 def marti_config():
@@ -340,14 +349,56 @@
     response = {
         'version': 3, 'type': 'java.lang.Boolean', 'data': False, 'nodeId': app.config.get('OTS_NODE_ID')
     }
 
     return jsonify(response)
 
 
+@marti_blueprint.route('/Marti/sync/upload', methods=['POST'])
+def itak_data_package_upload():
+    if not request.content_length:
+        return {'error': 'no file'}, 400, {'Content-Type': 'application/json'}
+    elif request.content_type != 'application/x-zip-compressed':
+        logger.error("Not a zip")
+        return {'error': 'Please only upload zip files'}, 415, {'Content-Type': 'application/json'}
+
+    file = request.data
+    sha256 = hashlib.sha256()
+    sha256.update(file)
+    file_hash = sha256.hexdigest()
+    logger.debug("got sha256 {}".format(file_hash))
+    hash_filename = secure_filename(file_hash + '.zip')
+
+    with open(os.path.join(app.config.get("UPLOAD_FOLDER"), hash_filename), "wb") as f:
+        f.write(file)
+
+    try:
+        data_package = DataPackage()
+        data_package.filename = request.args.get('name')
+        data_package.hash = file_hash
+        data_package.creator_uid = request.args.get('CreatorUid') if request.args.get('CreatorUid') else str(
+            uuid.uuid4())
+        data_package.submission_user = current_user.id if current_user.is_authenticated else None
+        data_package.submission_time = datetime.datetime.now()
+        data_package.mime_type = request.content_type
+        data_package.size = os.path.getsize(os.path.join(app.config.get("UPLOAD_FOLDER"), hash_filename))
+        db.session.add(data_package)
+        db.session.commit()
+    except sqlalchemy.exc.IntegrityError as e:
+        db.session.rollback()
+        logger.error("Failed to save data package: {}".format(e))
+        return jsonify({'success': False, 'error': 'This data package has already been uploaded'}), 400
+
+    return_value = {"UID": data_package.hash, "SubmissionDateTime": data_package.submission_time, "Keywords": ["missionpackage"],
+                    "MIMEType": data_package.mime_type, "SubmissionUser": "anonymous", "PrimaryKey": "1",
+                    "Hash": data_package.hash, "CreatorUid": data_package.creator_uid, "Name": data_package.filename}
+
+    return jsonify(return_value)
+
+
 @marti_blueprint.route('/Marti/sync/missionupload', methods=['POST'])
 def data_package_share():
     if not len(request.files):
         return {'error': 'no file'}, 400, {'Content-Type': 'application/json'}
     for file in request.files:
         file = request.files[file]
 
@@ -426,15 +477,16 @@
         if data_package:
 
             url = urlparse(request.url_root)
             protocol = url.scheme
             hostname = url.hostname
             port = url.port
 
-            return '{}://{}:{}/Marti/api/sync/metadata/{}/tool'.format(protocol, hostname, port, request.args.get('hash')), 200
+            return '{}://{}:{}/Marti/api/sync/metadata/{}/tool'.format(protocol, hostname, port,
+                                                                       request.args.get('hash')), 200
         else:
             return {'error': '404'}, 404, {'Content-Type': 'application/json'}
     except sqlalchemy.exc.NoResultFound as e:
         return {'error': '404'}, 404, {'Content-Type': 'application/json'}
 
 
 @marti_blueprint.route('/Marti/sync/search', methods=['GET'])
@@ -443,17 +495,19 @@
     res = {'resultCount': 0, 'results': []}
     for dp in data_packages:
         submission_user = "anonymous"
         if dp.user:
             submission_user = dp.user.username
         res['results'].append(
             {'UID': dp.hash, 'Name': dp.filename, 'Hash': dp.hash, 'CreatorUid': dp.creator_uid,
-             "SubmissionDateTime": dp.submission_time.strftime('%Y-%m-%dT%H:%M:%S.000Z'), "Expiration": -1, "Keywords": "[missionpackage]",
-             "MIMEType": dp.mime_type, "Size": dp.size, "SubmissionUser": submission_user, "PrimaryKey": dp.id,
-             "Tool": dp.tool
+             "SubmissionDateTime": dp.submission_time.strftime('%Y-%m-%dT%H:%M:%S.000Z'), "EXPIRATION": "-1",
+             "Keywords": ["missionpackage"],
+             "MIMEType": dp.mime_type, "Size": "{}".format(dp.size), "SubmissionUser": submission_user,
+             "PrimaryKey": "{}".format(dp.id),
+             "Tool": dp.tool if dp.tool else "public"
              })
         res['resultCount'] += 1
 
     return json.dumps(res), 200, {'Content-Type': 'application/json'}
 
 
 @marti_blueprint.route('/Marti/sync/content', methods=['GET'])
@@ -537,19 +591,27 @@
                 videoconnections = Element('videoConnections')
 
                 for video in videos:
                     # Make sure videos have the correct address based off of the Flask request and not 127.0.0.1
                     # This also forces all streams to bounce through MediaMTX
                     feed = BeautifulSoup(video.xml, 'xml')
 
+                    url = urlparse(request.url_root).hostname
+                    path = feed.find('path').text
+                    if not path.startswith("/"):
+                        path = "/" + path
+
+                    if 'iTAK' in request.user_agent.string:
+                        url = feed.find('protocol').text + "://" + url + ":" + feed.find("port").text + path
+
                     if feed.find('address'):
-                        feed.find('address').string.replace_with(urlparse(request.url_root).hostname)
+                        feed.find('address').string.replace_with(url)
                     else:
                         address = feed.new_tag('address')
-                        address.string = urlparse(request.url_root).hostname
+                        address.string = url
                         feed.feed.append(address)
                     videoconnections.append(fromstring(str(feed)))
 
             return tostring(videoconnections), 200
         except BaseException as e:
             logger.error(traceback.format_exc())
             return '', 500
```

### Comparing `opentakserver-1.0.1/opentakserver/blueprints/ots_socketio.py` & `opentakserver-1.1.0/opentakserver/blueprints/ots_socketio.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/blueprints/scheduled_jobs.py` & `opentakserver-1.1.0/opentakserver/blueprints/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/blueprints/scheduler_api.py` & `opentakserver-1.1.0/opentakserver/blueprints/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/ca_config.py` & `opentakserver-1.1.0/opentakserver/ca_config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/certificate_authority.py` & `opentakserver-1.1.0/opentakserver/certificate_authority.py`

 * *Files 12% similar despite different names*

```diff
@@ -384,12 +384,48 @@
             for file in files:
                 zipp.write(os.path.join(root, file))
         for root, dirs, files in os.walk('MANIFEST'):
             for file in files:
                 zipp.write(os.path.join(root, file))
         zipp.close()
 
+        # Generate iTAK zip
+        itak_preferences = Template("""<?xml version='1.0' standalone='yes'?>
+<preferences>
+  <preference version="1" name="cot_streams">
+    <entry key="count" class="class java.lang.Integer">1</entry>
+    <entry key="description0" class="class java.lang.String">OpenTAKServer_{{ server }}</entry>
+    <entry key="enabled0" class="class java.lang.Boolean">true</entry>
+    <entry key="connectString0" class="class java.lang.String">{{ server }}:{{ ssl_port }}:ssl</entry>
+  </preference>
+  <preference version="1" name="com.atakmap.app_preferences">
+    <entry key="displayServerConnectionWidget" class="class java.lang.Boolean">true</entry>
+    <entry key="caLocation" class="class java.lang.String">cert/truststore-root.p12</entry>
+    <entry key="caPassword" class="class java.lang.String">{{ cert_password }}</entry>
+    <entry key="clientPassword" class="class java.lang.String">{{ cert_password }}</entry>
+    <entry key="certificateLocation" class="class java.lang.String">cert/{{ common_name }}.p12</entry>
+  </preference>
+</preferences>
+
+""")
+
+        f = open(os.path.join(user_file_path, "config.pref"), 'w')
+        f.write(itak_preferences.render(server=urlparse(request.url_root).hostname,
+                                        ssl_port=self.app.config.get("OTS_SSL_STREAMING_PORT"),
+                                        cert_password=self.app.config.get("OTS_CA_PASSWORD"),
+                                        common_name=common_name))
+        f.close()
+
+        self.logger.info("Generating {}_CONFIG_iTAK.zip...".format(common_name))
+        itak_zip = zipfile.ZipFile(os.path.join(user_file_path, "{}_CONFIG_iTAK.zip".format(common_name)), 'w',
+                                   zipfile.ZIP_DEFLATED)
+        itak_zip.write(os.path.join(user_file_path, "config.pref"), "config.pref")
+        itak_zip.write(os.path.join(user_file_path, common_name + ".p12"), common_name + ".p12")
+        itak_zip.write(os.path.join(self.app.config.get("OTS_CA_FOLDER"), "truststore-root.p12"), "truststore-root.p12")
+        itak_zip.close()
+
         rmtree(os.path.join(user_file_path, "MANIFEST"))
         rmtree(os.path.join(user_file_path, parent_folder))
         os.remove(os.path.join(user_file_path, "{}.zip".format(common_name)))
+        os.remove(os.path.join(user_file_path, "config.pref".format(common_name)))
 
-        return "{}_CONFIG.zip".format(common_name)
+        return ["{}_CONFIG.zip".format(common_name), "{}_CONFIG_iTAK.zip".format(common_name)]
```

### Comparing `opentakserver-1.0.1/opentakserver/controllers/client_controller.py` & `opentakserver-1.1.0/opentakserver/controllers/client_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,22 @@
         self.longitude = 0
         self.ce = 0
         self.hae = 0
         self.le = 0
         self.course = 0
         self.speed = 0
         self.location_source = None
+        self.common_name = None
+
+        if self.is_ssl:
+            self.sock.do_handshake()
+            for c in self.sock.getpeercert()['subject']:
+                if c[0][0] == 'commonName':
+                    self.common_name = c[0][1]
+                    self.logger.debug("Got common name {}".format(self.common_name))
 
         # RabbitMQ
         try:
             self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters('localhost'),
                                                            self.on_connection_open)
             self.rabbit_channel = None
             self.iothread = Thread(target=self.rabbit_connection.ioloop.start)
@@ -114,67 +122,76 @@
                         except (ConnectionError, TimeoutError, ConnectionResetError) as e:
                             break
 
                 soup = BeautifulSoup(data, 'xml')
 
                 event = soup.find('event')
                 auth = soup.find('auth')
+
+                if not self.is_authenticated and (auth or self.common_name):
+                    with self.app.app_context():
+                        if auth:
+                            cot = auth.find('cot')
+                            if cot:
+                                username = cot.attrs['username']
+                                password = cot.attrs['password']
+                                uid = cot.attrs['uid']
+                                user = self.app.security.datastore.find_user(username=username)
+                        elif self.common_name:
+                            user = self.app.security.datastore.find_user(username=self.common_name)
+
+                        if not user:
+                            self.logger.warning("User {} does not exist".format(username))
+                            self.close_connection()
+                            break
+                        elif not user.active:
+                            self.logger.warning("User {} is deactivated, disconnecting".format(username))
+                            self.close_connection()
+                            break
+                        elif self.common_name:
+                            self.logger.info("{} is ID'ed by cert".format(user.username))
+                            self.is_authenticated = True
+                        elif verify_password(password, user.password):
+                            self.logger.info("Successful login from {}".format(username))
+                            self.is_authenticated = True
+                            try:
+                                eud = self.db.session.execute(self.db.session.query(EUD).filter_by(uid=uid)).first()[0]
+                                self.logger.debug("Associating EUD uid {} to user {}".format(eud.uid, user.username))
+                                eud.user_id = user.id
+                                self.db.session.commit()
+                            except:
+                                self.logger.debug("This is a new eud: {} {}".format(uid, user.username))
+                                eud = EUD()
+                                eud.uid = uid
+                                eud.user_id = user.id
+                                self.db.session.add(eud)
+                                self.db.session.commit()
+
+                            else:
+                                self.logger.warning("Wrong password for user {}".format(username))
+                                self.close_connection()
+                                break
+
                 if event:
                     # If this client is connected via ssl, make sure they're authenticated
                     # before accepting any data from them
                     if self.is_ssl and not self.is_authenticated:
-                        self.logger.debug("EUD isn't authenticated, ignoring")
+                        self.logger.warning("EUD isn't authenticated, ignoring")
                         continue
 
                     if event and self.pong(event):
                         continue
 
                     if event and not self.uid:
                         self.parse_device_info(event)
 
                     message = {'uid': self.uid, 'cot': str(soup)}
                     if self.rabbit_channel:
                         self.rabbit_channel.basic_publish(exchange='cot_controller', routing_key='',
                                                           body=json.dumps(message))
-                elif auth:
-                    with self.app.app_context():
-                        cot = auth.find('cot')
-                        if cot:
-                            username = cot.attrs['username']
-                            password = cot.attrs['password']
-                            uid = cot.attrs['uid']
-                            user = self.app.security.datastore.find_user(username=username)
-                            if not user:
-                                self.logger.warning("User {} does not exist".format(username))
-                                self.close_connection()
-                                break
-                            elif not user.active:
-                                self.logger.warning("User {} is deactivated, disconnecting".format(username))
-                                self.close_connection()
-                                break
-                            elif verify_password(password, user.password):
-                                self.logger.info("Successful login from {}".format(username))
-                                self.is_authenticated = True
-                                try:
-                                    eud = self.db.session.execute(self.db.session.query(EUD).filter_by(uid=uid)).first()[0]
-                                    self.logger.debug("Associating EUD uid {} to user {}".format(eud.uid, user.username))
-                                    eud.user_id = user.id
-                                    self.db.session.commit()
-                                except:
-                                    self.logger.debug("This is a new eud: {} {}".format(uid, user.username))
-                                    eud = EUD()
-                                    eud.uid = uid
-                                    eud.user_id = user.id
-                                    self.db.session.add(eud)
-                                    self.db.session.commit()
-
-                            else:
-                                self.logger.warning("Wrong password for user {}".format(username))
-                                self.close_connection()
-                                break
 
             else:
                 self.send_disconnect_cot()
                 break
 
     def close_connection(self):
         self.send_disconnect_cot()
```

### Comparing `opentakserver-1.0.1/opentakserver/controllers/cot_controller.py` & `opentakserver-1.1.0/opentakserver/controllers/cot_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,16 +603,24 @@
         destinations = event.find_all('dest')
 
         if chat and 'chatroom' in chat.attrs and chat.attrs['chatroom'] == 'All Chat Rooms':
             self.rabbit_channel.basic_publish(exchange='chatrooms', routing_key='All Chat Rooms', body=json.dumps(data))
 
         elif destinations:
             for destination in destinations:
+                # ATAK and WinTAK use callsign, iTAK uses uid
+                if 'callsign' in destination.attrs:
+                    uid = self.online_callsigns[destination.attrs['callsign']]['uid']
+                elif 'uid' in destination.attrs:
+                    uid = destination.attrs['uid']
+                else:
+                    continue
+
                 self.rabbit_channel.basic_publish(exchange='dms',
-                                                  routing_key=self.online_callsigns[destination.attrs['callsign']]['uid'],
+                                                  routing_key=uid,
                                                   body=json.dumps(data))
 
         # If no destination or callsign is specified, broadcast to all TAK clients
         elif self.rabbit_channel and self.rabbit_channel.is_open:
             self.rabbit_channel.basic_publish(exchange='cot', routing_key="", body=json.dumps(data))
 
         # Do nothing because the RabbitMQ channel hasn't opened yet or has closed
```

### Comparing `opentakserver-1.0.1/opentakserver/defaultconfig.py` & `opentakserver-1.1.0/opentakserver/defaultconfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/EmailValidator.py` & `opentakserver-1.1.0/opentakserver/EmailValidator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/forms/MediaMTXGlobalConfig.py` & `opentakserver-1.1.0/opentakserver/forms/MediaMTXGlobalConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/forms/MediaMTXPathConfig.py` & `opentakserver-1.1.0/opentakserver/forms/MediaMTXPathConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/Alert.py` & `opentakserver-1.1.0/opentakserver/models/Alert.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/CasEvac.py` & `opentakserver-1.1.0/opentakserver/models/CasEvac.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/Certificate.py` & `opentakserver-1.1.0/opentakserver/models/Certificate.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,23 @@
     __tablename__ = 'certificates'
 
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     common_name: Mapped[str] = mapped_column(String)
     eud_uid: Mapped[str] = mapped_column(Integer, ForeignKey("euds.uid"), nullable=True)
     data_package_id: Mapped[int] = mapped_column(Integer, ForeignKey("data_packages.id"), nullable=True)
     callsign: Mapped[str] = mapped_column(String, nullable=True)
+    username: Mapped[str] = mapped_column(String, ForeignKey("user.username"), nullable=True)
     expiration_date: Mapped[datetime] = mapped_column(DateTime)
     server_address: Mapped[str] = mapped_column(String)
     server_port: Mapped[int] = mapped_column(Integer)
     truststore_filename: Mapped[str] = mapped_column(String)
     user_cert_filename: Mapped[str] = mapped_column(String)
     csr: Mapped[str] = mapped_column(String, nullable=True)
     cert_password: Mapped[str] = mapped_column(String)
+    user = relationship("User", back_populates="certificate", uselist=False)
     eud = relationship("EUD", back_populates="certificate", uselist=False)
     data_package = relationship("DataPackage", back_populates="certificate", uselist=False)
 
     def serialize(self):
         return {
             'callsign': self.callsign,
             'expiration_date': self.expiration_date,
```

### Comparing `opentakserver-1.0.1/opentakserver/models/Chatrooms.py` & `opentakserver-1.1.0/opentakserver/models/Chatrooms.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/ChatroomsUids.py` & `opentakserver-1.1.0/opentakserver/models/ChatroomsUids.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/CoT.py` & `opentakserver-1.1.0/opentakserver/models/CoT.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/DataPackage.py` & `opentakserver-1.1.0/opentakserver/models/DataPackage.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/EUD.py` & `opentakserver-1.1.0/opentakserver/models/EUD.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             'uid': self.uid,
             'callsign': self.callsign,
             'device': self.device,
             'os': self.os,
             'platform': self.platform,
             'version': self.version,
             'phone_number': self.phone_number,
-            'last_event_time': iso8601_string_from_datetime(self.last_event_time),
+            'last_event_time': iso8601_string_from_datetime(self.last_event_time) if self.last_event_time else None,
             'last_status': self.last_status,
             'username': self.user.username if self.user else None,
             'last_point': self.points[-1].to_json() if self.points else None,
             'team': self.team.name if self.team else None,
             'team_color': self.team.get_team_color() if self.team else None,
             'team_role': self.team_role,
             'data_packages': self.data_packages.to_json(False) if include_data_packages and self.data_packages else None,
```

### Comparing `opentakserver-1.0.1/opentakserver/models/GeoChat.py` & `opentakserver-1.1.0/opentakserver/models/GeoChat.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/Icon.py` & `opentakserver-1.1.0/opentakserver/models/Icon.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/Marker.py` & `opentakserver-1.1.0/opentakserver/models/Marker.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/Point.py` & `opentakserver-1.1.0/opentakserver/models/Point.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/RBLine.py` & `opentakserver-1.1.0/opentakserver/models/RBLine.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/Team.py` & `opentakserver-1.1.0/opentakserver/models/Team.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/user.py` & `opentakserver-1.1.0/opentakserver/models/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 @dataclass
 class User(db.Model, fsqla.FsUserMixin):
     email = db.Column(String, nullable=True)
     video_streams = relationship("VideoStream", back_populates="user")
     euds = relationship("EUD", back_populates="user")
     data_packages = relationship("DataPackage", back_populates="user")
+    certificate = relationship("Certificate", back_populates="user")
 
     def serialize(self):
         return {
             'username': self.username,
             'active': self.active,
             'last_login_at': self.last_login_at,
             'last_login_ip': self.last_login_ip,
```

### Comparing `opentakserver-1.0.1/opentakserver/models/VideoRecording.py` & `opentakserver-1.1.0/opentakserver/models/VideoRecording.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/VideoStream.py` & `opentakserver-1.1.0/opentakserver/models/VideoStream.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/models/ZMIST.py` & `opentakserver-1.1.0/opentakserver/models/ZMIST.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/mumble/mumble_authenticator.py` & `opentakserver-1.1.0/opentakserver/mumble/mumble_authenticator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/mumble/mumble_ice_app.py` & `opentakserver-1.1.0/opentakserver/mumble/mumble_ice_app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/mumble/Murmur.ice` & `opentakserver-1.1.0/opentakserver/mumble/Murmur.ice`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/opentakserver/SocketServer.py` & `opentakserver-1.1.0/opentakserver/SocketServer.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/pyproject.toml` & `opentakserver-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentakserver"
-version = "1.0.1"
+version = "1.1.0"
 description = "A server for ATAK, WinTAK, and iTAK"
 authors = ["OpenTAKServer <opentakserver@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/brian7704/OpenTAKServer"
 documentation = "https://docs.opentakserver.io"
```

### Comparing `opentakserver-1.0.1/README.md` & `opentakserver-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `opentakserver-1.0.1/PKG-INFO` & `opentakserver-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentakserver
-Version: 1.0.1
+Version: 1.1.0
 Summary: A server for ATAK, WinTAK, and iTAK
 Home-page: https://github.com/brian7704/OpenTAKServer
 License: GPL-3.0-or-later
 Author: OpenTAKServer
 Author-email: opentakserver@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

