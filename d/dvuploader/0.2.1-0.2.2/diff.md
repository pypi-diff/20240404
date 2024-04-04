# Comparing `tmp/dvuploader-0.2.1.tar.gz` & `tmp/dvuploader-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvuploader-0.2.1.tar", max compression
+gzip compressed data, was "dvuploader-0.2.2.tar", max compression
```

## Comparing `dvuploader-0.2.1.tar` & `dvuploader-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2024-01-16 21:26:32.358187 dvuploader-0.2.1/LICENSE
--rw-r--r--   0        0        0     4125 2024-01-16 21:26:32.358187 dvuploader-0.2.1/README.md
--rw-r--r--   0        0        0      134 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/__init__.py
--rw-r--r--   0        0        0     2436 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/checksum.py
--rw-r--r--   0        0        0     4719 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/cli.py
--rw-r--r--   0        0        0    15262 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/directupload.py
--rw-r--r--   0        0        0     8824 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/dvuploader.py
--rw-r--r--   0        0        0     2866 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/file.py
--rw-r--r--   0        0        0     6846 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/nativeupload.py
--rw-r--r--   0        0        0     3014 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/packaging.py
--rw-r--r--   0        0        0     4367 2024-01-16 21:26:32.358187 dvuploader-0.2.1/dvuploader/utils.py
--rw-r--r--   0        0        0      767 2024-01-16 21:26:32.358187 dvuploader-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5041 1970-01-01 00:00:00.000000 dvuploader-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-04 09:46:19.384892 dvuploader-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4125 2024-04-04 09:46:19.384892 dvuploader-0.2.2/README.md
+-rw-r--r--   0        0        0      134 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/__init__.py
+-rw-r--r--   0        0        0     2436 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/checksum.py
+-rw-r--r--   0        0        0     4719 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/cli.py
+-rw-r--r--   0        0        0    17166 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/directupload.py
+-rw-r--r--   0        0        0    10260 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/dvuploader.py
+-rw-r--r--   0        0        0     3004 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/file.py
+-rw-r--r--   0        0        0     6886 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/nativeupload.py
+-rw-r--r--   0        0        0     3018 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/packaging.py
+-rw-r--r--   0        0        0     4367 2024-04-04 09:46:19.384892 dvuploader-0.2.2/dvuploader/utils.py
+-rw-r--r--   0        0        0      767 2024-04-04 09:46:19.384892 dvuploader-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5041 1970-01-01 00:00:00.000000 dvuploader-0.2.2/PKG-INFO
```

### Comparing `dvuploader-0.2.1/LICENSE` & `dvuploader-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dvuploader-0.2.1/README.md` & `dvuploader-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dvuploader-0.2.1/dvuploader/checksum.py` & `dvuploader-0.2.2/dvuploader/checksum.py`

 * *Files identical despite different names*

### Comparing `dvuploader-0.2.1/dvuploader/cli.py` & `dvuploader-0.2.2/dvuploader/cli.py`

 * *Files identical despite different names*

### Comparing `dvuploader-0.2.1/dvuploader/directupload.py` & `dvuploader-0.2.2/dvuploader/directupload.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,23 +4,30 @@
 import os
 from typing import Dict, List, Optional, Tuple
 from urllib.parse import urljoin
 import aiofiles
 import aiohttp
 
 from dvuploader.file import File
-from dvuploader.nativeupload import file_sender
 from dvuploader.utils import build_url
 
 TESTING = bool(os.environ.get("DVUPLOADER_TESTING", False))
+MAX_FILE_DISPLAY = int(os.environ.get("DVUPLOADER_MAX_FILE_DISPLAY", 50))
+MAX_RETRIES = int(os.environ.get("DVUPLOADER_MAX_RETRIES", 10))
+
+assert isinstance(
+    MAX_FILE_DISPLAY, int
+), "DVUPLOADER_MAX_FILE_DISPLAY must be an integer"
+
+assert isinstance(MAX_RETRIES, int), "DVUPLOADER_MAX_RETRIES must be an integer"
 
 TICKET_ENDPOINT = "/api/datasets/:persistentId/uploadurls"
 ADD_FILE_ENDPOINT = "/api/datasets/:persistentId/addFiles"
-UPLOAD_ENDPOINT = "/api/datasets/:persistentId/add?persistentId="
-REPLACE_ENDPOINT = "/api/files/{FILE_ID}/replace"
+UPLOAD_ENDPOINT = "/api/datasets/:persistentId/addFiles?persistentId="
+REPLACE_ENDPOINT = "/api/datasets/:persistentId/replaceFiles?persistentId="
 
 
 async def direct_upload(
     files: List[File],
     dataverse_url: str,
     api_token: str,
     persistent_id: str,
@@ -40,26 +47,28 @@
         pbars: A list of progress bars to display the upload progress for each file.
         n_parallel_uploads (int): The number of parallel uploads to perform.
 
     Returns:
         None
     """
 
+    leave_bar = len(files) < MAX_FILE_DISPLAY
     connector = aiohttp.TCPConnector(limit=n_parallel_uploads)
     async with aiohttp.ClientSession(connector=connector) as session:
         tasks = [
             _upload_to_store(
                 session=session,
                 file=file,
                 dataverse_url=dataverse_url,
                 api_token=api_token,
                 persistent_id=persistent_id,
                 pbar=pbar,
                 progress=progress,
                 delay=0.0,
+                leave_bar=leave_bar,
             )
             for pbar, file in zip(pbars, files)
         ]
 
         upload_results = await asyncio.gather(*tasks)
 
     for status, file in upload_results:
@@ -69,60 +78,54 @@
         print(f"❌ Failed to upload file '{file.fileName}' to the S3 storage")
 
     headers = {
         "X-Dataverse-key": api_token,
         "x-amz-tagging": "dv-state=temp",
     }
 
-    connector = aiohttp.TCPConnector(limit=4)
-    pbar = progress.add_task("╰── [bold white]Registering files", total=len(files))
-    results = []
+    pbar = progress.add_task("╰── [bold white]Registering files", total=1)
+    connector = aiohttp.TCPConnector(limit=2)
     async with aiohttp.ClientSession(
         headers=headers,
         connector=connector,
     ) as session:
-        for file in files:
-            results.append(
-                await _add_file_to_ds(
-                    session=session,
-                    file=file,
-                    dataverse_url=dataverse_url,
-                    pid=persistent_id,
-                )
-            )
-
-            progress.update(pbar, advance=1)
-
-    for file, status in zip(files, results):
-        if status is False:
-            print(f"❌ Failed to register file '{file.fileName}' at Dataverse")
+        await _add_files_to_ds(
+            session=session,
+            files=files,
+            dataverse_url=dataverse_url,
+            pid=persistent_id,
+            progress=progress,
+            pbar=pbar,
+        )
 
 
 async def _upload_to_store(
     session: aiohttp.ClientSession,
     file: File,
     persistent_id: str,
     dataverse_url: str,
     api_token: str,
     pbar,
     progress,
     delay: float,
+    leave_bar: bool,
 ):
     """
     Uploads a file to a Dataverse collection using direct upload.
 
     Args:
         session (aiohttp.ClientSession): The aiohttp client session.
         file (File): The file object to upload.
         persistent_id (str): The persistent identifier of the Dataverse dataset to upload to.
         dataverse_url (str): The URL of the Dataverse instance to upload to.
         api_token (str): The API token to use for authentication.
         pbar: The progress bar object.
         progress: The progress object.
         delay (float): The delay in seconds before starting the upload.
+        leave_bar (bool): A flag indicating whether to keep the progress bar visible after the upload is complete.
 
     Returns:
         tuple: A tuple containing the upload status (bool) and the file object.
     """
 
     await asyncio.sleep(delay)
 
@@ -142,14 +145,15 @@
         status, storage_identifier = await _upload_singlepart(
             session=session,
             ticket=ticket,
             filepath=file.filepath,
             pbar=pbar,
             progress=progress,
             api_token=api_token,
+            leave_bar=leave_bar,
         )
 
     else:
         status, storage_identifier = await _upload_multipart(
             session=session,
             response=ticket,
             filepath=file.filepath,
@@ -203,24 +207,26 @@
 async def _upload_singlepart(
     session: aiohttp.ClientSession,
     ticket: Dict,
     filepath: str,
     pbar,
     progress,
     api_token: str,
+    leave_bar: bool,
 ) -> Tuple[bool, str]:
     """
     Uploads a single part of a file to a remote server using HTTP PUT method.
 
     Args:
         session (aiohttp.ClientSession): The aiohttp client session used for the upload.
         ticket (Dict): A dictionary containing the response from the server.
         filepath (str): The path to the file to be uploaded.
         pbar (tqdm): A progress bar object to track the upload progress.
         progress: The progress object used to update the progress bar.
+        leave_bar (bool): A flag indicating whether to keep the progress bar visible after the upload is complete.
 
     Returns:
         Tuple[bool, str]: A tuple containing the status of the upload (True for success, False for failure)
                           and the storage identifier of the uploaded file.
     """
     assert "url" in ticket, "Couldnt find 'url'"
 
@@ -231,27 +237,33 @@
         "X-Dataverse-key": api_token,
         "x-amz-tagging": "dv-state=temp",
     }
     storage_identifier = ticket["storageIdentifier"]
     params = {
         "headers": headers,
         "url": ticket["url"],
-        "data": file_sender(
-            file_name=filepath,
-            progress=progress,
-            pbar=pbar,
-        ),
+        "data": open(filepath, "rb"),
     }
 
     async with session.put(**params) as response:
         status = response.status == 200
         response.raise_for_status()
 
         if status:
-            progress.update(pbar, advance=os.path.getsize(filepath))
+            progress.update(
+                pbar,
+                advance=os.path.getsize(filepath),
+            )
+
+            await asyncio.sleep(0.1)
+
+            progress.update(
+                pbar,
+                visible=leave_bar,
+            )
 
         return status, storage_identifier
 
 
 async def _upload_multipart(
     session: aiohttp.ClientSession,
     response: Dict,
@@ -459,48 +471,101 @@
     Raises:
         aiohttp.ClientResponseError: If the DELETE request fails.
     """
     async with session.delete(urljoin(dataverse_url, url)) as response:
         response.raise_for_status()
 
 
-async def _add_file_to_ds(
+async def _add_files_to_ds(
     session: aiohttp.ClientSession,
     dataverse_url: str,
     pid: str,
-    file: File,
-) -> bool:
+    files: List[File],
+    progress,
+    pbar,
+) -> None:
     """
     Adds a file to a Dataverse dataset.
 
     Args:
         session (aiohttp.ClientSession): The aiohttp client session.
         dataverse_url (str): The URL of the Dataverse instance.
         pid (str): The persistent identifier of the dataset.
         file (File): The file to be added.
 
     Returns:
         bool: True if the file was added successfully, False otherwise.
     """
-    if not file.to_replace:
-        url = urljoin(dataverse_url, UPLOAD_ENDPOINT + pid)
-    else:
-        url = build_url(
-            dataverse_url=dataverse_url,
-            endpoint=urljoin(
-                dataverse_url,
-                REPLACE_ENDPOINT.format(FILE_ID=file.file_id),
-            ),
-        )
 
-    json_data = file.model_dump_json(
-        by_alias=True,
-        exclude={"to_replace", "file_id"},
+    novel_url = urljoin(dataverse_url, UPLOAD_ENDPOINT + pid)
+    replace_url = urljoin(dataverse_url, REPLACE_ENDPOINT + pid)
+
+    novel_json_data = _prepare_registration(files, use_replace=False)
+    replace_json_data = _prepare_registration(files, use_replace=True)
+
+    await _multipart_json_data_request(
+        session=session,
+        json_data=novel_json_data,
+        url=novel_url,
+    )
+
+    await _multipart_json_data_request(
+        session=session,
+        json_data=replace_json_data,
+        url=replace_url,
+    )
+
+    progress.update(pbar, advance=1)
+
+
+def _prepare_registration(files: List[File], use_replace: bool) -> str:
+    """
+    Prepares the files for registration at the Dataverse instance.
+
+    Args:
+        files (List[File]): The list of files to prepare.
+
+    Returns:
+        str: A JSON string containing the file data.
+    """
+
+    exclude = {"to_replace"} if use_replace else {"to_replace", "file_id"}
+
+    return json.dumps(
+        [
+            file.model_dump(
+                by_alias=True,
+                exclude=exclude,
+                exclude_none=True,
+            )
+            for file in files
+            if file.to_replace is use_replace
+        ],
         indent=2,
     )
 
+
+async def _multipart_json_data_request(
+    json_data: str,
+    url: str,
+    session: aiohttp.ClientSession,
+):
+    """
+    Sends a multipart/form-data POST request with JSON data to the specified URL using the provided session.
+
+    Args:
+        json_data (str): The JSON data to be sent in the request body.
+        url (str): The URL to send the request to.
+        session (aiohttp.ClientSession): The aiohttp client session to use for the request.
+
+    Raises:
+        aiohttp.ClientResponseError: If the response status code is not successful.
+
+    Returns:
+        None
+    """
     with aiohttp.MultipartWriter("form-data") as writer:
         json_part = writer.append(json_data)
         json_part.set_content_disposition("form-data", name="jsonData")
 
         async with session.post(url, data=writer) as response:
-            return response.status == 200
+            response.raise_for_status()
```

### Comparing `dvuploader-0.2.1/dvuploader/dvuploader.py` & `dvuploader-0.2.2/dvuploader/dvuploader.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import rich
 from typing import Dict, List, Optional
 
 from pydantic import BaseModel
 from rich.progress import Progress, TaskID
 from rich.table import Table
 from rich.console import Console
+from rich.panel import Panel
 
 from dvuploader.directupload import (
     TICKET_ENDPOINT,
     direct_upload,
 )
 from dvuploader.file import File
 from dvuploader.nativeupload import native_upload
@@ -36,28 +37,46 @@
 
     def upload(
         self,
         persistent_id: str,
         dataverse_url: str,
         api_token: str,
         n_parallel_uploads: int = 1,
+        force_native: bool = False,
     ) -> None:
         """
         Uploads the files to the specified Dataverse repository in parallel.
 
         Args:
             persistent_id (str): The persistent identifier of the Dataverse dataset.
             dataverse_url (str): The URL of the Dataverse repository.
             api_token (str): The API token for the Dataverse repository.
             n_parallel_uploads (int): The number of parallel uploads to execute. In the case of direct upload, this restricts the amount of parallel chunks per upload. Please use n_jobs to control parallel files.
 
         Returns:
             None
         """
-        # Validate and hash files
+
+        print("\n")
+        info = "\n".join(
+            [
+                f"Server: [bold]{dataverse_url}[/bold]",  # type: ignore
+                f"PID: [bold]{persistent_id}[/bold]",  # type: ignore
+                f"Files: {len(self.files)}",
+            ]
+        )
+
+        panel = Panel(
+            info,
+            title="[bold]DVUploader[/bold]",
+            expand=False,
+        )
+
+        rich.print(panel)
+
         asyncio.run(self._validate_and_hash_files())
 
         # Check for duplicates
         self._check_duplicates(
             dataverse_url=dataverse_url,
             persistent_id=persistent_id,
             api_token=api_token,
@@ -77,24 +96,24 @@
         # Check if direct upload is supported
         has_direct_upload = self._has_direct_upload(
             dataverse_url=dataverse_url,
             api_token=api_token,
             persistent_id=persistent_id,
         )
 
-        if not has_direct_upload:
+        if not has_direct_upload and not force_native:
             rich.print(
                 "\n[bold italic white]⚠️  Direct upload not supported. Falling back to Native API."
             )
 
         rich.print(f"\n[bold italic white]🚀 Uploading files\n")
 
         progress, pbars = self.setup_progress_bars(files=files)
 
-        if not has_direct_upload:
+        if not has_direct_upload or force_native:
             with progress:
                 asyncio.run(
                     native_upload(
                         files=files,
                         dataverse_url=dataverse_url,
                         api_token=api_token,
                         persistent_id=persistent_id,
@@ -123,23 +142,43 @@
         """
         Validates and hashes the files to be uploaded.
 
         Returns:
             None
         """
 
-        rich.print("\n[italic white]📝 Preparing upload\n")
+        print("\n")
+
+        progress = Progress()
+        task = progress.add_task(
+            "[bold italic white]📦 Preparing upload[/bold italic white]",
+            total=len(self.files),
+        )
+        with progress:
+            tasks = [
+                self._validate_and_hash_file(
+                    file=file,
+                    progress=progress,
+                    task_id=task,
+                )
+                for file in self.files
+            ]
 
-        tasks = [self._validate_and_hash_file(file=file) for file in self.files]
+            await asyncio.gather(*tasks)
 
-        await asyncio.gather(*tasks)
+        print("\n")
 
     @staticmethod
-    async def _validate_and_hash_file(file: File):
+    async def _validate_and_hash_file(
+        file: File,
+        progress: Progress,
+        task_id: TaskID,
+    ):
         file.extract_filename_hash_file()
+        progress.update(task_id, advance=1)
 
     def _check_duplicates(
         self,
         dataverse_url: str,
         persistent_id: str,
         api_token: str,
     ):
@@ -165,38 +204,51 @@
             title_justify="left",
         )
         table.add_column("File", style="cyan", no_wrap=True)
         table.add_column("Status")
         table.add_column("Action")
 
         to_remove = []
+        over_threshold = len(self.files) > 50
+        n_new_files = 0
+        n_skip_files = 0
 
         for file in self.files:
             has_same_hash = any(
                 map(lambda dsFile: self._check_hashes(file, dsFile), ds_files)
             )
 
             if has_same_hash and file.checksum:
+                n_skip_files += 1
                 table.add_row(
                     file.fileName, "[bright_black]Same hash", "[bright_black]Skip"
                 )
                 to_remove.append(file)
             else:
+                n_new_files += 1
                 table.add_row(
                     file.fileName, "[spring_green3]New", "[spring_green3]Upload"
                 )
 
                 # If present in dataset, replace file
                 file.file_id = self._get_file_id(file, ds_files)
                 file.to_replace = True if file.file_id else False
 
         for file in to_remove:
             self.files.remove(file)
 
         console = Console()
+
+        if over_threshold:
+            table = Table(title="[bold white]🔎 Checking dataset files")
+
+            table.add_column("New", style="spring_green3", no_wrap=True)
+            table.add_column("Skipped", style="bright_black", no_wrap=True)
+            table.add_row(str(n_new_files), str(n_skip_files))
+
         console.print(table)
 
     @staticmethod
     def _get_file_id(
         file: File,
         ds_files: List[Dict],
     ) -> Optional[str]:
```

### Comparing `dvuploader-0.2.1/dvuploader/file.py` & `dvuploader-0.2.2/dvuploader/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
-from typing import List, Optional
+from typing import List, Optional, Union
 
-from pydantic import BaseModel, Field, model_validator
+from pydantic import BaseModel, ConfigDict, Field, model_validator
 import rich
 
 from dvuploader.checksum import Checksum, ChecksumTypes
 
 
 class File(BaseModel):
     """
@@ -27,26 +27,28 @@
 
     Methods:
         _validate_filepath(path): Validates if the file path exists and is a file.
         _extract_filename_hash_file(): Extracts the filename from the filepath and calculates the file's checksum.
 
     """
 
+    model_config: ConfigDict = ConfigDict(populate_by_alias=True)
+
     filepath: str = Field(..., exclude=True)
     description: str = ""
     directoryLabel: str = ""
     mimeType: str = "text/plain"
     categories: List[str] = ["DATA"]
     restrict: bool = False
     checksum_type: ChecksumTypes = Field(default=ChecksumTypes.MD5, exclude=True)
     storageIdentifier: Optional[str] = None
     fileName: Optional[str] = None
     checksum: Optional[Checksum] = None
     to_replace: bool = False
-    file_id: Optional[str] = None
+    file_id: Optional[Union[str, int]] = Field(default=None, alias="fileToReplaceId")
 
     def extract_filename_hash_file(self):
         """
         Extracts the filename and calculates the hash of the file.
 
         Returns:
             self: The current instance of the class.
```

### Comparing `dvuploader-0.2.1/dvuploader/nativeupload.py` & `dvuploader-0.2.2/dvuploader/nativeupload.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     _reset_progress(pbars, progress)
 
     session_params = {
         "base_url": dataverse_url,
         "headers": {"X-Dataverse-key": api_token},
         "connector": aiohttp.TCPConnector(
             limit=n_parallel_uploads,
+            timeout_ceil_threshold=120,
         ),
     }
 
     async with aiohttp.ClientSession(**session_params) as session:
         with tempfile.TemporaryDirectory() as tmp_dir:
             packages = distribute_files(files)
             packaged_files = _zip_packages(
```

### Comparing `dvuploader-0.2.1/dvuploader/packaging.py` & `dvuploader-0.2.2/dvuploader/packaging.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import zipfile
 
 from typing import List, Tuple
 
 MAXIMUM_PACKAGE_SIZE = int(
     os.environ.get(
         "DVUPLOADER_MAX_PKG_SIZE",
-        1024**3,  # 1 GB
+        2 * 1024**3,  # 2 GB
     )
 )
 
 
 def distribute_files(dv_files: List["File"]):  # type: ignore
     """
     Distributes a list of files into packages based on their sizes.
```

### Comparing `dvuploader-0.2.1/dvuploader/utils.py` & `dvuploader-0.2.2/dvuploader/utils.py`

 * *Files identical despite different names*

### Comparing `dvuploader-0.2.1/pyproject.toml` & `dvuploader-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dvuploader"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python library for uploading (bulk) data to Dataverse"
 authors = ["Jan Range"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^2.5.3"
```

### Comparing `dvuploader-0.2.1/PKG-INFO` & `dvuploader-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvuploader
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for uploading (bulk) data to Dataverse
 Author: Jan Range
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dvuploader Version: 0.2.1 Summary: Python library
+Metadata-Version: 2.1 Name: dvuploader Version: 0.2.2 Summary: Python library
 for uploading (bulk) data to Dataverse Author: Jan Range Requires-Python:
 >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiodns (>=3.1.1,<4.0.0) Requires-Dist: aiofiles
 (>=23.2.1,<24.0.0) Requires-Dist: aiohttp (>=3.9.1,<4.0.0) Requires-Dist:
```

