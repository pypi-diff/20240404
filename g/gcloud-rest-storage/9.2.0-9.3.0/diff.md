# Comparing `tmp/gcloud_rest_storage-9.2.0.tar.gz` & `tmp/gcloud_rest_storage-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud_rest_storage-9.2.0.tar", max compression
+gzip compressed data, was "gcloud_rest_storage-9.3.0.tar", max compression
```

## Comparing `gcloud_rest_storage-9.2.0.tar` & `gcloud_rest_storage-9.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1063 2024-02-16 16:52:12.000000 gcloud_rest_storage-9.2.0/LICENSE
--rw-r--r--   0        0        0     1000 2024-02-16 16:52:12.000000 gcloud_rest_storage-9.2.0/README.rst
--rw-r--r--   0        0        0        0 2024-02-16 16:52:12.000000 gcloud_rest_storage-9.2.0/gcloud/py.typed
--rw-r--r--   0        0        0        0 2024-02-16 16:52:12.000000 gcloud_rest_storage-9.2.0/gcloud/rest/py.typed
--rw-r--r--   0        0        0     5712 2024-02-16 16:52:13.000000 gcloud_rest_storage-9.2.0/gcloud/rest/storage/__init__.py
--rw-r--r--   0        0        0     9099 2024-02-16 16:52:13.000000 gcloud_rest_storage-9.2.0/gcloud/rest/storage/blob.py
--rw-r--r--   0        0        0     2769 2024-02-16 16:52:13.000000 gcloud_rest_storage-9.2.0/gcloud/rest/storage/bucket.py
--rw-r--r--   0        0        0       70 2024-02-16 16:52:13.000000 gcloud_rest_storage-9.2.0/gcloud/rest/storage/constants.py
--rw-r--r--   0        0        0        0 2024-02-16 16:52:12.000000 gcloud_rest_storage-9.2.0/gcloud/rest/storage/py.typed
--rw-r--r--   0        0        0    28611 2024-02-16 16:52:13.000000 gcloud_rest_storage-9.2.0/gcloud/rest/storage/storage.py
--rw-r--r--   0        0        0     1056 2024-02-16 16:52:12.000000 gcloud_rest_storage-9.2.0/pyproject.toml
--rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 gcloud_rest_storage-9.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-04 13:40:07.000000 gcloud_rest_storage-9.3.0/LICENSE
+-rw-r--r--   0        0        0     1000 2024-04-04 13:40:07.000000 gcloud_rest_storage-9.3.0/README.rst
+-rw-r--r--   0        0        0        0 2024-04-04 13:40:07.000000 gcloud_rest_storage-9.3.0/gcloud/py.typed
+-rw-r--r--   0        0        0        0 2024-04-04 13:40:07.000000 gcloud_rest_storage-9.3.0/gcloud/rest/py.typed
+-rw-r--r--   0        0        0     5712 2024-04-04 13:40:08.000000 gcloud_rest_storage-9.3.0/gcloud/rest/storage/__init__.py
+-rw-r--r--   0        0        0     9241 2024-04-04 13:40:08.000000 gcloud_rest_storage-9.3.0/gcloud/rest/storage/blob.py
+-rw-r--r--   0        0        0     2769 2024-04-04 13:40:08.000000 gcloud_rest_storage-9.3.0/gcloud/rest/storage/bucket.py
+-rw-r--r--   0        0        0       70 2024-04-04 13:40:08.000000 gcloud_rest_storage-9.3.0/gcloud/rest/storage/constants.py
+-rw-r--r--   0        0        0        0 2024-04-04 13:40:07.000000 gcloud_rest_storage-9.3.0/gcloud/rest/storage/py.typed
+-rw-r--r--   0        0        0    30871 2024-04-04 13:40:08.000000 gcloud_rest_storage-9.3.0/gcloud/rest/storage/storage.py
+-rw-r--r--   0        0        0     1056 2024-04-04 13:40:07.000000 gcloud_rest_storage-9.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 gcloud_rest_storage-9.3.0/PKG-INFO
```

### Comparing `gcloud_rest_storage-9.2.0/LICENSE` & `gcloud_rest_storage-9.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-9.2.0/README.rst` & `gcloud_rest_storage-9.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-9.2.0/gcloud/rest/storage/__init__.py` & `gcloud_rest_storage-9.3.0/gcloud/rest/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-9.2.0/gcloud/rest/storage/blob.py` & `gcloud_rest_storage-9.3.0/gcloud/rest/storage/blob.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,20 +95,23 @@
     @property
     def chunk_size(self) -> int:
         return self.size + (262144 - (self.size % 262144))
 
     def download(
         self, timeout: int = DEFAULT_TIMEOUT,
         session: Optional[Session] = None,
+        auto_decompress: bool = True,
     ) -> Any:
+        headers = None if auto_decompress else {'accept-encoding': 'gzip'}
         return self.bucket.storage.download(
             self.bucket.name,
             self.name,
             timeout=timeout,
             session=session,
+            headers=headers,
         )
 
     def upload(
         self, data: Any,
         content_type: Optional[str] = None,
         session: Optional[Session] = None,
     ) -> Dict[str, Any]:
```

### Comparing `gcloud_rest_storage-9.2.0/gcloud/rest/storage/bucket.py` & `gcloud_rest_storage-9.3.0/gcloud/rest/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_storage-9.2.0/gcloud/rest/storage/storage.py` & `gcloud_rest_storage-9.3.0/gcloud/rest/storage/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import binascii
 import enum
+import gzip
 import io
 import json
 import logging
 import mimetypes
 import os
 import warnings
 from typing import Any
@@ -411,32 +412,38 @@
         self, bucket: str, object_name: str, file_data: Any,
         *, content_type: Optional[str] = None,
         parameters: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         session: Optional[Session] = None,
         force_resumable_upload: Optional[bool] = None,
+        zipped: bool = False,
         timeout: int = 30,
     ) -> Dict[str, Any]:
         url = f'{self._api_root_write}/{bucket}/o'
-
         stream = self._preprocess_data(file_data)
 
+        parameters = parameters or {}
+        if zipped:
+            parameters['contentEncoding'] = 'gzip'
+            # Here we load the file-like object data into memory in chunks and
+            # re-write it compressed. This is implemented like this so we don't
+            # load the whole file into memory at once.
+            stream = self._compress_file_in_chunks(input_stream=stream)
+
         if BUILD_GCLOUD_REST and isinstance(stream, io.StringIO):
             # HACK: `requests` library does not accept `str` as `data` in `put`
             # HTTP request.
             stream = io.BytesIO(stream.getvalue().encode('utf-8'))
 
         content_length = self._get_stream_len(stream)
 
         # mime detection method same as in aiohttp 3.4.4
         content_type = content_type or mimetypes.guess_type(object_name)[0]
 
-        parameters = parameters or {}
-
         headers = headers or {}
         headers.update(self._headers())
         headers.update({
             'Content-Length': str(content_length),
             'Content-Type': content_type or '',
         })
 
@@ -495,14 +502,42 @@
             return io.StringIO(data)
         if isinstance(data, io.IOBase):
             return data  # type: ignore[return-value]
 
         raise TypeError(f'unsupported upload type: "{type(data)}"')
 
     @staticmethod
+    def _compress_file_in_chunks(input_stream: IO[AnyStr],
+                                 chunk_size: int = 8192) -> IO[bytes]:
+        """
+        Reads the contents of input_stream and writes it gzip-compressed to
+        output_stream in chunks. The chunk size is 8Kb by default, which is a
+        standard filesystem block size.
+        """
+        compressed_stream = io.BytesIO()
+
+        with gzip.open(compressed_stream, 'wb') as gzipped_file:
+            chunk_bytes: bytes
+            while True:
+                chunk = input_stream.read(chunk_size)
+                if not chunk:
+                    break
+                if isinstance(chunk, str):
+                    chunk_bytes = chunk.encode('utf-8')
+                else:
+                    chunk_bytes = chunk
+
+                gzipped_file.write(chunk_bytes)
+
+        # After finishing writing, reset the buffer position so it can be read
+        compressed_stream.seek(0)
+
+        return compressed_stream
+
+    @staticmethod
     def _decide_upload_type(
         force_resumable_upload: Optional[bool],
         content_length: int,
     ) -> UploadType:
         # force resumable
         if force_resumable_upload is True:
             return UploadType.RESUMABLE
@@ -549,27 +584,43 @@
     ) -> bytes:
         # https://cloud.google.com/storage/docs/request-endpoints#encoding
         encoded_object_name = quote(object_name, safe='')
         url = f'{self._api_root_read}/{bucket}/o/{encoded_object_name}'
         headers = headers or {}
         headers.update(self._headers())
 
+        # aiohttp and requests automatically decompress the body if this
+        # argument is not passed. We assume that if the Accept-Encoding header
+        # is present, then the client will handle the decompression
+        auto_decompress = 'accept-encoding' not in {k.lower() for k in headers}
+
         s = SyncSession(session) if session else self.session
-        response = s.get(
-            url, headers=headers, params=params or {},
-            timeout=timeout,
-        )
 
-        # N.B. the GCS API sometimes returns 'application/octet-stream' when a
-        # string was uploaded. To avoid potential weirdness, always return a
-        # bytes object.
-        try:
-            data: bytes = response.read()
-        except (AttributeError, TypeError):
-            data = response.content  # type: ignore[assignment]
+        data: bytes
+        if not auto_decompress and BUILD_GCLOUD_REST:
+            # Requests lib has a different way of reading compressed data. We
+            # must pass the stream=True argument and read the response using
+            # the 'raw' property.
+            response = s.get(
+                url, headers=headers, params=params or {},
+                timeout=timeout, stream=True,
+            )
+            data = response.raw.read()  # type: ignore[attr-defined]
+        else:
+            response = s.get(
+                url, headers=headers, params=params or {},
+                timeout=timeout, auto_decompress=auto_decompress,
+            )
+            # N.B. the GCS API sometimes returns 'application/octet-stream'
+            # when a string was uploaded. To avoid potential weirdness, always
+            # return a bytes object.
+            try:
+                data = response.read()
+            except (AttributeError, TypeError):
+                data = response.content  # type: ignore[assignment]
 
         return data
 
     def _download_stream(
         self, bucket: str, object_name: str, *,
         params: Optional[Dict[str, str]] = None,
         headers: Optional[Dict[str, str]] = None,
```

### Comparing `gcloud_rest_storage-9.2.0/pyproject.toml` & `gcloud_rest_storage-9.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcloud-rest-storage"
-version = "9.2.0"
+version = "9.3.0"
 description = "Python Client for Google Cloud Storage"
 readme = "README.rst"
 
 repository = "https://github.com/talkiq/gcloud-aio"
 authors = ["Vi Engineering <voiceai-eng@dialpad.com>"]
 license = "MIT"
 
@@ -18,23 +18,23 @@
     'Operating System :: OS Independent',
     'Topic :: Internet',
 ]
 
 [tool.poetry.dependencies]
 python = ">= 3.8, < 4.0"
 # aiofiles = ">= 0.6.0, < 24.0.0"
-gcloud-rest-auth = ">= 3.6.0, < 6.0.0"
-pyasn1-modules = ">= 0.2.1, < 0.4.0"
+gcloud-rest-auth = ">= 5.3.0, < 6.0.0"
+pyasn1-modules = ">= 0.2.1, < 0.4.1"
 rsa = ">= 3.1.4, < 5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 gcloud-rest-auth = { path = "../auth" }
-pytest = "8.0.0"
-# pytest-asyncio = "0.23.5"
-pytest-mock = "3.12.0"
+pytest = "8.1.1"
+# pytest-asyncio = "0.23.6"
+pytest-mock = "3.14.0"
 
 [[tool.poetry.source]]
 name = "pypi"
 priority = "primary"
 
 [tool.pytest.ini_options]
 # addopts = "-Werror"  # TODO: fixme
```

### Comparing `gcloud_rest_storage-9.2.0/PKG-INFO` & `gcloud_rest_storage-9.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-rest-storage
-Version: 9.2.0
+Version: 9.3.0
 Summary: Python Client for Google Cloud Storage
 Home-page: https://github.com/talkiq/gcloud-aio
 License: MIT
 Author: Vi Engineering
 Author-email: voiceai-eng@dialpad.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
-Requires-Dist: gcloud-rest-auth (>=3.6.0,<6.0.0)
-Requires-Dist: pyasn1-modules (>=0.2.1,<0.4.0)
+Requires-Dist: gcloud-rest-auth (>=5.3.0,<6.0.0)
+Requires-Dist: pyasn1-modules (>=0.2.1,<0.4.1)
 Requires-Dist: rsa (>=3.1.4,<5.0.0)
 Project-URL: Repository, https://github.com/talkiq/gcloud-aio
 Description-Content-Type: text/x-rst
 
 (Asyncio OR Threadsafe) Python Client for Google Cloud Storage
 ==============================================================
```

