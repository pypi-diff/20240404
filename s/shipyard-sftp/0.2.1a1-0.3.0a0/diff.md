# Comparing `tmp/shipyard_sftp-0.2.1a1.tar.gz` & `tmp/shipyard_sftp-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_sftp-0.2.1a1.tar", max compression
+gzip compressed data, was "shipyard_sftp-0.3.0a0.tar", max compression
```

## Comparing `shipyard_sftp-0.2.1a1.tar` & `shipyard_sftp-0.3.0a0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-05-12 18:48:21.840614 shipyard_sftp-0.2.1a1/README.md
--rw-r--r--   0        0        0      553 2024-04-03 16:57:47.470431 shipyard_sftp-0.2.1a1/pyproject.toml
--rw-r--r--   0        0        0        1 2024-03-06 14:22:56.719708 shipyard_sftp-0.2.1a1/shipyard_sftp/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 03:34:57.761954 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/__init__.py
--rw-r--r--   0        0        0      474 2024-03-06 14:22:56.720339 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/authtest.py
--rw-r--r--   0        0        0     3199 2024-04-03 16:43:54.708590 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/delete_file.py
--rw-r--r--   0        0        0     3396 2024-04-03 16:52:45.266419 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/download_file.py
--rw-r--r--   0        0        0     3862 2024-04-03 16:52:45.262531 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/move_file.py
--rw-r--r--   0        0        0     3223 2024-04-03 16:52:45.270196 shipyard_sftp-0.2.1a1/shipyard_sftp/cli/upload_file.py
--rw-r--r--   0        0        0     3387 2024-03-29 15:30:29.284848 shipyard_sftp-0.2.1a1/shipyard_sftp/exceptions.py
--rw-r--r--   0        0        0    13970 2024-04-03 16:41:50.563392 shipyard_sftp-0.2.1a1/shipyard_sftp/sftp.py
--rw-r--r--   0        0        0     1638 2024-04-03 16:43:54.711437 shipyard_sftp-0.2.1a1/shipyard_sftp/utils.py
--rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 shipyard_sftp-0.2.1a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-12 18:48:21.840614 shipyard_sftp-0.3.0a0/README.md
+-rw-r--r--   0        0        0      553 2024-04-04 16:34:42.099203 shipyard_sftp-0.3.0a0/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-03-06 14:22:56.719708 shipyard_sftp-0.3.0a0/shipyard_sftp/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-11 03:34:57.761954 shipyard_sftp-0.3.0a0/shipyard_sftp/cli/__init__.py
+-rw-r--r--   0        0        0      474 2024-03-06 14:22:56.720339 shipyard_sftp-0.3.0a0/shipyard_sftp/cli/authtest.py
+-rw-r--r--   0        0        0     3363 2024-04-04 16:30:12.496510 shipyard_sftp-0.3.0a0/shipyard_sftp/cli/delete_file.py
+-rw-r--r--   0        0        0     4075 2024-04-04 16:29:49.492357 shipyard_sftp-0.3.0a0/shipyard_sftp/cli/download_file.py
+-rw-r--r--   0        0        0     4027 2024-04-04 16:29:49.485720 shipyard_sftp-0.3.0a0/shipyard_sftp/cli/move_file.py
+-rw-r--r--   0        0        0     3387 2024-04-04 16:29:49.499113 shipyard_sftp-0.3.0a0/shipyard_sftp/cli/upload_file.py
+-rw-r--r--   0        0        0     3387 2024-04-04 15:32:48.428604 shipyard_sftp-0.3.0a0/shipyard_sftp/exceptions.py
+-rw-r--r--   0        0        0    14000 2024-04-04 16:31:32.690031 shipyard_sftp-0.3.0a0/shipyard_sftp/sftp.py
+-rw-r--r--   0        0        0     1638 2024-04-04 15:32:48.429805 shipyard_sftp-0.3.0a0/shipyard_sftp/utils.py
+-rw-r--r--   0        0        0      659 1970-01-01 00:00:00.000000 shipyard_sftp-0.3.0a0/PKG-INFO
```

### Comparing `shipyard_sftp-0.2.1a1/pyproject.toml` & `shipyard_sftp-0.3.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-sftp"
-version = "0.2.1a1"
+version = "0.3.0a0"
 description = "A local client for connecting and working with SFTP servers"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "shipyard_sftp" }]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_sftp-0.2.1a1/shipyard_sftp/cli/delete_file.py` & `shipyard_sftp-0.3.0a0/shipyard_sftp/cli/delete_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import CloudStorage, ExitCodeException
 from shipyard_templates.shipyard_logger import ShipyardLogger
 
 from shipyard_sftp.sftp import SftpClient
 from shipyard_sftp.utils import setup_connection, tear_down
-
+from shipyard_sftp.exceptions import InvalidCredentialsError
 logger = ShipyardLogger().get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--source-file-name-match-type",
@@ -37,16 +37,19 @@
     exit_code = 0
     key_path = None
     sftp = None
 
     try:
 
         args = get_args()
-        connection_args, key_path = setup_connection(args)
-        sftp = SftpClient(**connection_args)
+        try:
+            connection_args, key_path = setup_connection(args)
+            sftp = SftpClient(**connection_args)
+        except Exception as e:
+            raise InvalidCredentialsError(e) from e
 
         source_file_name = args.source_file_name
         source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
         source_full_path = shipyard.combine_folder_and_file_name(
             source_folder_name, source_file_name
         )
         source_file_name_match_type = args.source_file_name_match_type or "exact_match"
```

### Comparing `shipyard_sftp-0.2.1a1/shipyard_sftp/cli/download_file.py` & `shipyard_sftp-0.3.0a0/shipyard_sftp/cli/upload_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,87 +4,88 @@
 
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import CloudStorage, ExitCodeException
 from shipyard_templates.shipyard_logger import ShipyardLogger
 
 from shipyard_sftp.sftp import SftpClient
 from shipyard_sftp.utils import setup_connection, tear_down
+from shipyard_sftp.exceptions import InvalidCredentialsError
 
 logger = ShipyardLogger().get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--source-file-name-match-type",
         dest="source_file_name_match_type",
         choices={"exact_match", "regex_match"},
         required=True,
     )
-    parser.add_argument(
-        "--source-folder-name", dest="source_folder_name", default="", required=False
-    )
     parser.add_argument("--source-file-name", dest="source_file_name", required=True)
     parser.add_argument(
-        "--destination-file-name",
-        dest="destination_file_name",
-        default=None,
-        required=False,
+        "--source-folder-name", dest="source_folder_name", default="", required=False
     )
     parser.add_argument(
         "--destination-folder-name",
         dest="destination_folder_name",
         default="",
         required=False,
     )
+    parser.add_argument(
+        "--destination-file-name",
+        dest="destination_file_name",
+        default=None,
+        required=False,
+    )
     parser.add_argument("--host", dest="host", default=None, required=True)
     parser.add_argument("--port", dest="port", default=21, required=True)
     parser.add_argument("--username", dest="username", default=None, required=False)
     parser.add_argument("--password", dest="password", default=None, required=False)
     parser.add_argument("--key", dest="key", default=None, required=False)
     return parser.parse_args()
 
 
 def main():
-    exit_code = 0
-    key_path = None
     sftp = None
+    key_path = None
+    exit_code = 0
     try:
         args = get_args()
-        connection_args, key_path = setup_connection(args)
-        sftp = SftpClient(**connection_args)
 
-        source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
-        source_file_name_match_type = args.source_file_name_match_type or "exact_match"
+        try:
+            connection_args, key_path = setup_connection(args)
+            sftp = SftpClient(**connection_args)
+        except Exception as e:
+            raise InvalidCredentialsError(e) from e
+
+        source_folder_name = args.source_folder_name
 
         destination_folder_name = shipyard.clean_folder_name(
             args.destination_folder_name.strip("/")
         )
-        shipyard.create_folder_if_dne(destination_folder_name)
-        sftp_files_full_paths = sftp.list_files_recursive(source_folder_name or ".")
-
-        # Get the relative path of the files which is the format that shipyard.file_match expects
-        sftp_files = [
-            os.path.relpath(path, start=source_folder_name)
-            for path in sftp_files_full_paths
-        ]
 
+        source_file_name_match_type = args.source_file_name_match_type or "exact_match"
         files = shipyard.file_match(
             search_term=args.source_file_name,
-            files=sftp_files,
+            files=shipyard.fetch_file_paths_from_directory(source_folder_name),
             source_directory=source_folder_name,
             destination_directory=destination_folder_name,
             destination_filename=args.destination_file_name,
             match_type=source_file_name_match_type,
         )
 
         for file in files:
             source_file = file["source_path"]
             destination_full_path = file["destination_filename"]
-            sftp.download(source_file, destination_full_path)
+            if not os.path.isfile(source_file):
+                raise ExitCodeException(
+                    f"{source_file} is not a file", sftp.EXIT_CODE_FILE_MATCH_ERROR
+                )
+            sftp.upload(source_file, destination_full_path)
 
     except ExitCodeException as e:
         logger.error(e)
         exit_code = e.exit_code
     except FileNotFoundError as e:
         logger.error(e)
         exit_code = CloudStorage.EXIT_CODE_FILE_NOT_FOUND
```

### Comparing `shipyard_sftp-0.2.1a1/shipyard_sftp/cli/move_file.py` & `shipyard_sftp-0.3.0a0/shipyard_sftp/cli/move_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import CloudStorage, ExitCodeException
 from shipyard_templates.shipyard_logger import ShipyardLogger
 
 from shipyard_sftp.sftp import SftpClient
 from shipyard_sftp.utils import setup_connection, tear_down
+from shipyard_sftp.exceptions import InvalidCredentialsError
 
 logger = ShipyardLogger().get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -47,16 +48,19 @@
 
 def main():
     key_path = None
     sftp = None
     exit_code = 0
     try:
         args = get_args()
-        connection_args, key_path = setup_connection(args)
-        sftp = SftpClient(**connection_args)
+        try:
+            connection_args, key_path = setup_connection(args)
+            sftp = SftpClient(**connection_args)
+        except Exception as e:
+            raise InvalidCredentialsError(e) from e
 
         source_file_name = args.source_file_name
         source_folder_name = args.source_folder_name
         source_full_path = shipyard.combine_folder_and_file_name(
             source_folder_name, source_file_name
         )
         destination_folder_name = shipyard.clean_folder_name(
```

### Comparing `shipyard_sftp-0.2.1a1/shipyard_sftp/cli/upload_file.py` & `shipyard_sftp-0.3.0a0/shipyard_sftp/cli/download_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,88 +1,108 @@
 import argparse
 import os
 import sys
 
+import paramiko
 from shipyard_bp_utils import files as shipyard
 from shipyard_templates import CloudStorage, ExitCodeException
 from shipyard_templates.shipyard_logger import ShipyardLogger
 
+from shipyard_sftp.exceptions import InvalidCredentialsError
 from shipyard_sftp.sftp import SftpClient
 from shipyard_sftp.utils import setup_connection, tear_down
 
 logger = ShipyardLogger().get_logger()
 
+DEFAULT_WINDOW_SIZE = 4294967294
+DEFAULT_REKEY_BYTES = pow(2, 40)
+DEFAULT_REKEY_PACKETS = pow(2, 40)
+
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--source-file-name-match-type",
         dest="source_file_name_match_type",
         choices={"exact_match", "regex_match"},
         required=True,
     )
-    parser.add_argument("--source-file-name", dest="source_file_name", required=True)
     parser.add_argument(
         "--source-folder-name", dest="source_folder_name", default="", required=False
     )
-    parser.add_argument(
-        "--destination-folder-name",
-        dest="destination_folder_name",
-        default="",
-        required=False,
-    )
+    parser.add_argument("--source-file-name", dest="source_file_name", required=True)
     parser.add_argument(
         "--destination-file-name",
         dest="destination_file_name",
         default=None,
         required=False,
     )
+    parser.add_argument(
+        "--destination-folder-name",
+        dest="destination_folder_name",
+        default="",
+        required=False,
+    )
     parser.add_argument("--host", dest="host", default=None, required=True)
     parser.add_argument("--port", dest="port", default=21, required=True)
     parser.add_argument("--username", dest="username", default=None, required=False)
     parser.add_argument("--password", dest="password", default=None, required=False)
     parser.add_argument("--key", dest="key", default=None, required=False)
     return parser.parse_args()
 
 
 def main():
-    sftp = None
-    key_path = None
     exit_code = 0
+    key_path = None
+    sftp = None
     try:
         args = get_args()
 
-        connection_args, key_path = setup_connection(args)
+        try:
+            connection_args, key_path = setup_connection(args)
 
-        sftp = SftpClient(**connection_args)
+            transport = paramiko.Transport((args.host, int(args.port)))
+            transport.default_window_size = DEFAULT_WINDOW_SIZE
+            transport.packetizer.REKEY_BYTES = DEFAULT_REKEY_BYTES
+            transport.packetizer.REKEY_PACKETS = DEFAULT_REKEY_PACKETS
+            transport.connect(None, args.username, args.password)
+
+            connection_args["transport"] = transport
+            sftp = SftpClient(**connection_args)
+        except Exception as e:
+            raise InvalidCredentialsError(e) from e
 
-        source_folder_name = args.source_folder_name
+        source_folder_name = shipyard.clean_folder_name(args.source_folder_name)
+        source_file_name_match_type = args.source_file_name_match_type or "exact_match"
 
         destination_folder_name = shipyard.clean_folder_name(
             args.destination_folder_name.strip("/")
         )
+        shipyard.create_folder_if_dne(destination_folder_name)
+        sftp_files_full_paths = sftp.list_files_recursive(source_folder_name or ".")
+
+        # Get the relative path of the files which is the format that shipyard.file_match expects
+        sftp_files = [
+            os.path.relpath(path, start=source_folder_name)
+            for path in sftp_files_full_paths
+        ]
 
-        source_file_name_match_type = args.source_file_name_match_type or "exact_match"
         files = shipyard.file_match(
             search_term=args.source_file_name,
-            files=shipyard.fetch_file_paths_from_directory(source_folder_name),
+            files=sftp_files,
             source_directory=source_folder_name,
             destination_directory=destination_folder_name,
             destination_filename=args.destination_file_name,
             match_type=source_file_name_match_type,
         )
 
         for file in files:
             source_file = file["source_path"]
             destination_full_path = file["destination_filename"]
-            if not os.path.isfile(source_file):
-                raise ExitCodeException(
-                    f"{source_file} is not a file", sftp.EXIT_CODE_FILE_MATCH_ERROR
-                )
-            sftp.upload(source_file, destination_full_path)
+            sftp.download(source_file, destination_full_path)
 
     except ExitCodeException as e:
         logger.error(e)
         exit_code = e.exit_code
     except FileNotFoundError as e:
         logger.error(e)
         exit_code = CloudStorage.EXIT_CODE_FILE_NOT_FOUND
```

### Comparing `shipyard_sftp-0.2.1a1/shipyard_sftp/exceptions.py` & `shipyard_sftp-0.3.0a0/shipyard_sftp/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.2.1a1/shipyard_sftp/sftp.py` & `shipyard_sftp-0.3.0a0/shipyard_sftp/sftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,22 @@
     DownloadException,
     FileNotFound,
     DeleteException,
 )
 
 logger = ShipyardLogger().get_logger()
 
-DEFAULT_WINDOW_SIZE = 4294967294
-DEFAULT_REKEY_BYTES = pow(2, 40)
-DEFAULT_REKEY_PACKETS = pow(2, 40)
+
 
 
 class SftpClient(CloudStorage):
     EXIT_CODE_DELETE_ERROR = 100
 
     def __init__(
-            self, host: str, port: int, key: str = None, user: str = None, pwd: str = None
+            self, host: str, port: int, key: str = None, user: str = None, pwd: str = None, transport=None
     ) -> None:
         """
         Initializes an SFTP client with the given connection parameters.
 
         Parameters:
         - host (str): The hostname or IP address of the SFTP server.
         - port (int): The port number of the SFTP server.
@@ -40,14 +38,15 @@
         - pwd (str, optional): The password for authentication (if password-based authentication is used).
 
         Note: This class can use out-of-the-box paramiko for SFTP operations by calling the client property.
         ex:
             sftp = SftpClient(host, port, key, user, pwd)
             sftp.client.listdir()
         """
+        self.transport = transport
         self.host = host
         self.port = port
         self.key = key
         self.user = user
         self.pwd = pwd
         self._client = None
 
@@ -268,19 +267,22 @@
                 )
                 return ssh.open_sftp()
 
             else:
                 logger.debug(
                     f"Connecting to {self.host} using password-based authentication"
                 )
-                transport = paramiko.Transport((self.host, int(self.port)))
-                transport.default_window_size = 4294967294
-                transport.packetizer.REKEY_BYTES = pow(2, 40)
-                transport.packetizer.REKEY_PACKETS = pow(2, 40)
-                transport.connect(None, self.user, self.pwd)
+                if self.transport is None:
+                    logger.debug(f"Creating simple transport to {self.host}")
+                    transport = paramiko.Transport((self.host, int(self.port)))
+                    transport.connect(None, self.user, self.pwd)
+                else:
+                    logger.debug("Explicit transport provided.")
+                    transport = self.transport
+
                 return paramiko.SFTPClient.from_transport(transport)
 
         except (
                 paramiko.SSHException,
                 paramiko.AuthenticationException,
                 ValueError,
                 FileNotFoundError,
```

### Comparing `shipyard_sftp-0.2.1a1/shipyard_sftp/utils.py` & `shipyard_sftp-0.3.0a0/shipyard_sftp/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_sftp-0.2.1a1/PKG-INFO` & `shipyard_sftp-0.3.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-sftp
-Version: 0.2.1a1
+Version: 0.3.0a0
 Summary: A local client for connecting and working with SFTP servers
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

