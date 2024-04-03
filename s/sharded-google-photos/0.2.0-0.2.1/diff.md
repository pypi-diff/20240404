# Comparing `tmp/sharded_google_photos-0.2.0.tar.gz` & `tmp/sharded_google_photos-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharded_google_photos-0.2.0.tar", max compression
+gzip compressed data, was "sharded_google_photos-0.2.1.tar", max compression
```

## Comparing `sharded_google_photos-0.2.0.tar` & `sharded_google_photos-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2024-03-18 17:48:51.353682 sharded_google_photos-0.2.0/LICENSE
--rw-r--r--   0        0        0     4772 2024-03-29 18:32:42.107603 sharded_google_photos-0.2.0/README.md
--rw-r--r--   0        0        0      755 2024-03-29 18:32:42.109994 sharded_google_photos-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      464 2024-03-20 07:05:33.524175 sharded_google_photos-0.2.0/sharded_google_photos/backup/diffs_splitter.py
--rw-r--r--   0        0        0     8761 2024-03-29 18:32:42.111368 sharded_google_photos-0.2.0/sharded_google_photos/backup/gphotos_backup.py
--rw-r--r--   0        0        0      551 2024-03-27 17:57:15.555272 sharded_google_photos-0.2.0/sharded_google_photos/backup/gphotos_uploader.py
--rw-r--r--   0        0        0     2532 2024-03-27 17:57:15.556670 sharded_google_photos-0.2.0/sharded_google_photos/backup/media_item_repository.py
--rw-r--r--   0        0        0     2841 2024-03-27 17:57:15.558065 sharded_google_photos-0.2.0/sharded_google_photos/backup/shared_album_repository.py
--rw-r--r--   0        0        0     2193 2024-03-27 17:57:15.559288 sharded_google_photos-0.2.0/sharded_google_photos/cleanup/gphotos_cleaner.py
--rw-r--r--   0        0        0     8266 2024-03-29 18:32:42.113625 sharded_google_photos-0.2.0/sharded_google_photos/shared/gphotos_album_client.py
--rw-r--r--   0        0        0     4247 2024-03-27 17:57:15.562695 sharded_google_photos-0.2.0/sharded_google_photos/shared/gphotos_client.py
--rw-r--r--   0        0        0     8388 2024-03-29 18:32:42.114809 sharded_google_photos-0.2.0/sharded_google_photos/shared/gphotos_mediaitem_client.py
--rw-r--r--   0        0        0     1721 2024-03-27 17:57:15.565065 sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/fake_gphotos_album_client.py
--rw-r--r--   0        0        0     1540 2024-03-27 17:57:15.566785 sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/fake_gphotos_client.py
--rw-r--r--   0        0        0     1197 2024-03-27 17:57:15.567903 sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py
--rw-r--r--   0        0        0     9185 2024-03-27 17:57:15.569275 sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/fake_gphotos_repository.py
--rw-r--r--   0        0        0      616 2024-03-29 18:32:42.115559 sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 sharded_google_photos-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-18 17:48:51.353682 sharded_google_photos-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4795 2024-04-03 03:34:24.298488 sharded_google_photos-0.2.1/README.md
+-rw-r--r--   0        0        0      780 2024-04-03 23:10:55.108775 sharded_google_photos-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      464 2024-03-20 07:05:33.524175 sharded_google_photos-0.2.1/sharded_google_photos/backup/diffs_splitter.py
+-rw-r--r--   0        0        0     8761 2024-03-29 18:32:42.111368 sharded_google_photos-0.2.1/sharded_google_photos/backup/gphotos_backup.py
+-rw-r--r--   0        0        0      551 2024-03-27 17:57:15.555272 sharded_google_photos-0.2.1/sharded_google_photos/backup/gphotos_uploader.py
+-rw-r--r--   0        0        0     2532 2024-04-02 06:21:34.945407 sharded_google_photos-0.2.1/sharded_google_photos/backup/media_item_repository.py
+-rw-r--r--   0        0        0     2841 2024-03-27 17:57:15.558065 sharded_google_photos-0.2.1/sharded_google_photos/backup/shared_album_repository.py
+-rw-r--r--   0        0        0     2193 2024-03-27 17:57:15.559288 sharded_google_photos-0.2.1/sharded_google_photos/cleanup/gphotos_cleaner.py
+-rw-r--r--   0        0        0     6168 2024-04-03 23:06:18.951870 sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_album_client.py
+-rw-r--r--   0        0        0     4306 2024-04-01 07:46:11.129212 sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_client.py
+-rw-r--r--   0        0        0     8990 2024-04-03 23:09:52.803576 sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_mediaitem_client.py
+-rw-r--r--   0        0        0     1721 2024-03-27 17:57:15.565065 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_album_client.py
+-rw-r--r--   0        0        0     1540 2024-03-27 17:57:15.566785 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_client.py
+-rw-r--r--   0        0        0     1197 2024-03-27 17:57:15.567903 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py
+-rw-r--r--   0        0        0     9185 2024-03-27 17:57:15.569275 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_repository.py
+-rw-r--r--   0        0        0      616 2024-03-29 18:32:42.115559 sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 sharded_google_photos-0.2.1/PKG-INFO
```

### Comparing `sharded_google_photos-0.2.0/LICENSE` & `sharded_google_photos-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/README.md` & `sharded_google_photos-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 Running out of space in your Google Photos account? Wish you can upload an unlimited number of photos on Google Photos? Now you can! With this Python library, you can upload your photos to multiple Google Photo Accounts and then share those albums to your main Google Photos account. That way, you get to see all of your photos on one main Google Photos account.
 
 It works like this:
 
 1. Let's say you have three Google Accounts.
 
-2. Install the package by running `pip install sharded-google-photos`.
+2. Install `libmagic`
 
-3. Import the following code in your `main.py` app:
+3. Install the package by running `pip install sharded-google-photos`.
+
+4. Import the following code in your `main.py` app:
 
     ```python
     from sharded_google_photos.backup.gphotos_backup import GPhotosBackup
     from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
     clients = [
         GPhotosClient(creds_file = "credentials-1.json", client_secret="client_secret.json"),
@@ -23,15 +25,15 @@
     ]
     for client in clients:
         client.authenticate()
 
     backup_client = GPhotosBackup(clients)
     ```
 
-4. To upload four photos from two folders, run the following:
+5. To upload four photos from two folders, run the following:
 
     ```python
     new_album_uris = backup_client.backup([
         {
             "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
             "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/2.jpg",
             "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/3.jpg",
@@ -49,26 +51,26 @@
 
     3. Photos `1.jpg`, and `2.jpg` will be in the `Archives/Photos/2022/Trip to California` album.
 
     4. Photos `3.jpg`, and `4.jpg` will be in the `Archives/Photos/2022/Trip to Toronto` album.
 
     3. The url to those new albums will be in `new_album_uris` that you can share to.
 
-5. To update a file in a folder, run the following:
+6. To update a file in a folder, run the following:
 
     ```python
     backup_client.backup([
         {
             "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
             "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
         }
     ])
     ```
 
-6. To delete a file in a folder, run the following:
+7. To delete a file in a folder, run the following:
 
     ```python
     backup_client.backup([
         {
             "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
         }
     ])
```

### Comparing `sharded_google_photos-0.2.0/pyproject.toml` & `sharded_google_photos-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "sharded-google-photos"
-version = "0.2.0"
+version = "0.2.1"
 description = "A tool to shard photos across multiple Google Photo accounts"
 authors = ["Emilio K <e.kartonoe@gmail.com>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 google-api-python-client = "^2.122.0"
 google-auth-oauthlib = "^1.2.0"
 backoff = "^2.2.1"
+python-magic = "^0.4.27"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^8.1.1"
 flake8 = "^7.0.0"
 flake8-bugbear = "^24.2.6"
```

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/backup/gphotos_backup.py` & `sharded_google_photos-0.2.1/sharded_google_photos/backup/gphotos_backup.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/backup/gphotos_uploader.py` & `sharded_google_photos-0.2.1/sharded_google_photos/backup/gphotos_uploader.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/backup/media_item_repository.py` & `sharded_google_photos-0.2.1/sharded_google_photos/backup/media_item_repository.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/backup/shared_album_repository.py` & `sharded_google_photos-0.2.1/sharded_google_photos/backup/shared_album_repository.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/cleanup/gphotos_cleaner.py` & `sharded_google_photos-0.2.1/sharded_google_photos/cleanup/gphotos_cleaner.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/shared/gphotos_client.py` & `sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,20 @@
     "https://www.googleapis.com/auth/drive.photos.readonly",
 ]
 
 
 class GPhotosClient:
     def __init__(
         self,
+        name,
         creds_file,
         client_secret=DEFAULT_CLIENT_SECRETS_FILE,
         scopes=DEFAULT_SCOPES,
     ):
+        self.name = name
         self.creds_file = creds_file
         self.client_secret = client_secret
         self.scopes = scopes
 
         self.session: AuthorizedSession = None
         self._albums_client: GPhotosAlbumClient = None
         self._media_items_client: GPhotosMediaItemClient = None
@@ -88,15 +90,15 @@
     def __get_credentials_via_oauth__(self):
         """Use data in the given filename to get oauth data"""
         iaflow: InstalledAppFlow = InstalledAppFlow.from_client_secrets_file(
             self.client_secret, self.scopes
         )
         logger.debug("Obtained saved credentials from oauth2 flow")
         iaflow.run_local_server(
-            authorization_prompt_message="Please visit this URL: {url}",
+            authorization_prompt_message=f"For {self.name}, please visit this URL: {{url}}",
             success_message="The auth flow is complete; you may close this window.",
             open_browser=False,
         )
 
         return iaflow.credentials
 
     def get_storage_quota(self):
```

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/shared/gphotos_mediaitem_client.py` & `sharded_google_photos-0.2.1/sharded_google_photos/shared/gphotos_mediaitem_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,57 @@
 import json
 import logging
-import mimetypes
 import os
 import backoff
-from requests.exceptions import RequestException
+import magic
+from requests.exceptions import RequestException, HTTPError
 
 from google.auth.transport.requests import AuthorizedSession
 from google.auth.transport import DEFAULT_RETRYABLE_STATUS_CODES
 
 logger = logging.getLogger(__name__)
 
+DEFAULT_RETRYABLE_ERROR_CODES_FOR_UPLOADED_PHOTOS = set(
+    [
+        1,  # Cancelled
+        2,  # Unknown
+        4,  # DEADLINE_EXCEEDED,
+        10,  # 409 Conflict
+        12,  # 501 Not Implemented
+        13,  # 500 Internal Server Error
+        14,  # 503 Service Unavailable
+        15,  # 500 Internal Server Error
+    ]
+)
+
+ERROR_CODES_FOR_UPLOADED_PHOTOS_TO_MESSAGE = {
+    1: "Cancelled",
+    2: "UNKNOWN",
+    3: "INVALID_ARGUMENT",
+    4: "DEADLINE_EXCEEDED",
+    5: "NOT_FOUND",
+    7: "PERMISSION_DENIED",
+    8: "RESOURCE_EXHAUSTED",
+    9: "FAILED_PRECONDITION",
+    10: "ABORTED",
+    11: "OUT_OF_RANGE",
+    12: "UNIMPLEMENTED",
+    13: "INTERNAL",
+    14: "UNAVAILABLE",
+    15: "DATA_LOSS",
+    16: "UNAUTHENTICATED",
+}
+
+
+class IllegalStateException(ValueError):
+    """Exception raised when the state is invalid"""
+
+    def __init__(self, message: str):
+        super().__init__(message)
+
 
 class GPhotosMediaItemClient:
     def __init__(self, session: AuthorizedSession):
         self._session = session
 
     @backoff.on_exception(backoff.expo, (RequestException))
     def add_uploaded_photos_to_gphotos(
@@ -35,48 +73,56 @@
             indent=4,
         )
 
         res = self._session.post(
             "https://photoslibrary.googleapis.com/v1/mediaItems:batchCreate",
             create_body,
         )
+        res.raise_for_status()
+        res_json = res.json()
 
-        if res.status_code in DEFAULT_RETRYABLE_STATUS_CODES:
-            res.raise_for_status()
+        logger.debug(f"{res_json}")
 
-        if res.status_code != 200:
-            raise Exception(f"Failed to batch create: {res.status_code} {res.content}")
+        new_media_items = []
+        for result in res_json["newMediaItemResults"]:
+            if result["status"]["message"] == "Success":
+                new_media_items.append(result)
+            else:
+                code = result["status"]["code"]
+                message = result["status"]["message"]
+
+                if code == 6:
+                    continue
+                elif code in DEFAULT_RETRYABLE_ERROR_CODES_FOR_UPLOADED_PHOTOS:
+                    raise HTTPError(f"code: {code}, message: {message}")
+                else:
+                    raise ValueError(f"code: {code}, message: {message}")
 
-        return res.json()
+        return {"newMediaItemResults": new_media_items}
 
     def search_for_media_items(
         self, album_id: str = None, filters: str = None, order_by: str = None
     ):
         logger.debug(f"Listing media items with filter {album_id} {filters} {order_by}")
 
         page_token = None
         media_items = []
         while True:
-            response = self._search_media_items_in_pages(
+            res = self._search_media_items_in_pages(
                 album_id, filters, order_by, page_token
             )
-            if response.status_code != 200:
-                raise Exception(
-                    f"Fetching media items failed: {response.status_code} {response.content}"
-                )
-
-            response_body = response.json()
+            res_body = res.json()
 
-            if "mediaItems" not in response_body:
+            if "mediaItems" not in res_body:
                 break
 
-            media_items += response_body["mediaItems"]
+            media_items += res_body["mediaItems"]
 
-            if "nextPageToken" in response_body:
-                page_token = response_body["nextPageToken"]
+            if "nextPageToken" in res_body:
+                page_token = res_body["nextPageToken"]
             else:
                 break
 
         return media_items
 
     @backoff.on_exception(backoff.expo, (RequestException))
     def _search_media_items_in_pages(
@@ -93,62 +139,46 @@
                     "albumId": album_id,
                     "filters": filters,
                     "orderBy": order_by,
                     "pageToken": page_token,
                 }
             ),
         )
-        if res.status_code in DEFAULT_RETRYABLE_STATUS_CODES:
-            res.raise_for_status()
+        res.raise_for_status()
         return res
 
     @backoff.on_exception(backoff.expo, (RequestException))
     def upload_photo(self, photo_file_path: str, file_name: str):
         logger.debug(f"Uploading photo {photo_file_path}")
 
-        try:
-            photo_file = open(photo_file_path, mode="rb")
-            photo_bytes = photo_file.read()
-        except OSError as err:
-            logger.error(
-                "Could not read file '{0}' -- {1}".format(photo_file_path, err)
-            )
-            return
+        photo_file = open(photo_file_path, mode="rb")
+        photo_bytes = photo_file.read()
 
         self._session.headers["Content-type"] = "application/octet-stream"
         self._session.headers["X-Goog-Upload-Protocol"] = "raw"
         self._session.headers["X-Goog-Upload-File-Name"] = file_name
 
         res = self._session.post(
             "https://photoslibrary.googleapis.com/v1/uploads", photo_bytes
         )
-        if res.status_code in DEFAULT_RETRYABLE_STATUS_CODES:
-            res.raise_for_status()
-
-        if res.status_code != 200 or not res.content:
-            logger.error(f"No valid upload token {res.status_code} {res.content}")
-            return
+        res.raise_for_status()
 
         return res.content.decode()
 
+    @backoff.on_exception(backoff.expo, (IllegalStateException))
     def upload_photo_in_chunks(self, photo_file_path: str, file_name: str):
         upload_token = None
-        mime_type, _ = mimetypes.guess_type(photo_file_path)
+        mime_type = self._get_mime_type(photo_file_path)
         file_size_in_bytes = os.stat(photo_file_path).st_size
 
         logger.debug(
             f"Uploading in chunks with mime_type {mime_type} and file size {file_size_in_bytes}"
         )
 
         res_1 = self._initialize_chunked_upload(mime_type, file_size_in_bytes)
-        if res_1.status_code != 200:
-            raise Exception(
-                f"Unable to initialize chunked upload: {res_1.status_code} {res_1.content}"
-            )
-
         upload_url = res_1.headers["X-Goog-Upload-URL"]
         chunk_size = int(res_1.headers["X-Goog-Upload-Chunk-Granularity"])
 
         logger.debug(f"Obtained upload url and chunk size: {upload_url} {chunk_size}")
 
         with open(photo_file_path, "rb") as file_obj:
             cur_offset = 0
@@ -174,15 +204,15 @@
                     )
 
                     req_3 = self._query_chunked_upload(upload_url)
                     upload_status = req_3.headers["X-Goog-Upload-Status"]
                     size_received = int(req_3.headers["X-Goog-Upload-Size-Received"])
 
                     if upload_status != "active":
-                        raise Exception("Upload is no longer active")
+                        raise IllegalStateException("Upload is no longer active")
 
                     logger.debug(f"Adjusted seek to {size_received}")
                     file_obj.seek(size_received, 0)
                     cur_offset = size_received
                     next_chunk = file_obj.read(chunk_size)
                 else:
                     cur_offset += chunk_read
@@ -200,16 +230,15 @@
         self._session.headers["Content-Length"] = "0"
         self._session.headers["X-Goog-Upload-Command"] = "start"
         self._session.headers["X-Goog-Upload-Content-Type"] = mime_type
         self._session.headers["X-Goog-Upload-Protocol"] = "resumable"
         self._session.headers["X-Goog-Upload-Raw-Size"] = str(file_size_in_bytes)
 
         res = self._session.post("https://photoslibrary.googleapis.com/v1/uploads")
-        if res.status_code in DEFAULT_RETRYABLE_STATUS_CODES:
-            res.raise_for_status()
+        res.raise_for_status()
 
         return res
 
     @backoff.on_exception(backoff.expo, (RequestException))
     def _upload_photo_chunk(
         self, upload_url: str, cur_offset: int, chunk: bytes, is_last_chunk: bool
     ):
@@ -225,11 +254,13 @@
 
     @backoff.on_exception(backoff.expo, (RequestException))
     def _query_chunked_upload(self, upload_url):
         self._session.headers["Content-Length"] = "0"
         self._session.headers["X-Goog-Upload-Command"] = "query"
 
         res = self._session.post(upload_url)
-        if res.status_code in DEFAULT_RETRYABLE_STATUS_CODES:
-            res.raise_for_status()
+        res.raise_for_status()
 
         return res
+
+    def _get_mime_type(self, file_path):
+        return magic.from_file(file_path, mime=True)
```

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/fake_gphotos_album_client.py` & `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_album_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/fake_gphotos_client.py` & `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py` & `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_mediaitem_client.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/fake_gphotos_repository.py` & `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/fake_gphotos_repository.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py` & `sharded_google_photos-0.2.1/sharded_google_photos/shared/testing/mocked_saved_credentials_file.py`

 * *Files identical despite different names*

### Comparing `sharded_google_photos-0.2.0/PKG-INFO` & `sharded_google_photos-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 Metadata-Version: 2.1
 Name: sharded-google-photos
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool to shard photos across multiple Google Photo accounts
 License: GNU General Public License v3.0
 Author: Emilio K
 Author-email: e.kartonoe@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: google-api-python-client (>=2.122.0,<3.0.0)
 Requires-Dist: google-auth-oauthlib (>=1.2.0,<2.0.0)
+Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Sharded-Google-Photos
 
 ## Description
 
 Running out of space in your Google Photos account? Wish you can upload an unlimited number of photos on Google Photos? Now you can! With this Python library, you can upload your photos to multiple Google Photo Accounts and then share those albums to your main Google Photos account. That way, you get to see all of your photos on one main Google Photos account.
 
 It works like this:
 
 1. Let's say you have three Google Accounts.
 
-2. Install the package by running `pip install sharded-google-photos`.
+2. Install `libmagic`
 
-3. Import the following code in your `main.py` app:
+3. Install the package by running `pip install sharded-google-photos`.
+
+4. Import the following code in your `main.py` app:
 
     ```python
     from sharded_google_photos.backup.gphotos_backup import GPhotosBackup
     from sharded_google_photos.shared.gphotos_client import GPhotosClient
 
     clients = [
         GPhotosClient(creds_file = "credentials-1.json", client_secret="client_secret.json"),
@@ -39,15 +42,15 @@
     ]
     for client in clients:
         client.authenticate()
 
     backup_client = GPhotosBackup(clients)
     ```
 
-4. To upload four photos from two folders, run the following:
+5. To upload four photos from two folders, run the following:
 
     ```python
     new_album_uris = backup_client.backup([
         {
             "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
             "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/2.jpg",
             "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to Toronto/3.jpg",
@@ -65,26 +68,26 @@
 
     3. Photos `1.jpg`, and `2.jpg` will be in the `Archives/Photos/2022/Trip to California` album.
 
     4. Photos `3.jpg`, and `4.jpg` will be in the `Archives/Photos/2022/Trip to Toronto` album.
 
     3. The url to those new albums will be in `new_album_uris` that you can share to.
 
-5. To update a file in a folder, run the following:
+6. To update a file in a folder, run the following:
 
     ```python
     backup_client.backup([
         {
             "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
             "modifier": "+", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
         }
     ])
     ```
 
-6. To delete a file in a folder, run the following:
+7. To delete a file in a folder, run the following:
 
     ```python
     backup_client.backup([
         {
             "modifier": "-", "file_path": "./Archives/Photos/2022/Trip to California/1.jpg",
         }
     ])
```

