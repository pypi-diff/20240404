# Comparing `tmp/blob-az-0.2.3.tar.gz` & `tmp/blob-az-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blob-az-0.2.3.tar", last modified: Sun Mar 17 17:02:50 2024, max compression
+gzip compressed data, was "blob-az-0.2.4.tar", last modified: Thu Apr  4 17:57:39 2024, max compression
```

## Comparing `blob-az-0.2.3.tar` & `blob-az-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.993920 blob-az-0.2.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1805 2024-03-17 17:02:49.993920 blob-az-0.2.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1334 2024-03-17 17:02:39.000000 blob-az-0.2.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      681 2024-03-17 17:02:43.000000 blob-az-0.2.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-03-17 17:02:49.993920 blob-az-0.2.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.983920 blob-az-0.2.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.983920 blob-az-0.2.3/src/blob_az/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      105 2024-03-17 15:52:25.000000 blob-az-0.2.3/src/blob_az/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.993920 blob-az-0.2.3/src/blob_az/blob/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       88 2024-03-17 14:57:22.000000 blob-az-0.2.3/src/blob_az/blob/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3292 2024-03-17 15:54:22.000000 blob-az-0.2.3/src/blob_az/blob/blob.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.993920 blob-az-0.2.3/src/blob_az/container/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-03-17 14:57:22.000000 blob-az-0.2.3/src/blob_az/container/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1915 2024-03-17 15:54:29.000000 blob-az-0.2.3/src/blob_az/container/container.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.993920 blob-az-0.2.3/src/blob_az/env/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-03-17 15:54:16.000000 blob-az-0.2.3/src/blob_az/env/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-03-17 15:52:19.000000 blob-az-0.2.3/src/blob_az/env/keys.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.993920 blob-az-0.2.3/src/blob_az/list/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-03-17 14:57:22.000000 blob-az-0.2.3/src/blob_az/list/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      500 2024-03-17 14:57:22.000000 blob-az-0.2.3/src/blob_az/list/list.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.993920 blob-az-0.2.3/src/blob_az/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       56 2024-03-17 14:57:22.000000 blob-az-0.2.3/src/blob_az/util/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-03-17 15:52:48.000000 blob-az-0.2.3/src/blob_az/util/util.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-03-17 17:02:49.993920 blob-az-0.2.3/src/blob_az.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1805 2024-03-17 17:02:49.000000 blob-az-0.2.3/src/blob_az.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-03-17 17:02:49.000000 blob-az-0.2.3/src/blob_az.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-03-17 17:02:49.000000 blob-az-0.2.3/src/blob_az.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-03-17 17:02:49.000000 blob-az-0.2.3/src/blob_az.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        8 2024-03-17 17:02:49.000000 blob-az-0.2.3/src/blob_az.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.034859 blob-az-0.2.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1810 2024-04-04 17:57:39.034859 blob-az-0.2.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1334 2024-03-17 17:02:39.000000 blob-az-0.2.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      686 2024-04-04 17:57:04.000000 blob-az-0.2.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 17:57:39.034859 blob-az-0.2.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.024859 blob-az-0.2.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.024859 blob-az-0.2.4/src/blob_az/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      105 2024-03-17 15:52:25.000000 blob-az-0.2.4/src/blob_az/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.034859 blob-az-0.2.4/src/blob_az/blob/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       88 2024-03-17 14:57:22.000000 blob-az-0.2.4/src/blob_az/blob/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3290 2024-04-04 17:57:14.000000 blob-az-0.2.4/src/blob_az/blob/blob.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.034859 blob-az-0.2.4/src/blob_az/container/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       79 2024-03-17 14:57:22.000000 blob-az-0.2.4/src/blob_az/container/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1915 2024-03-17 15:54:29.000000 blob-az-0.2.4/src/blob_az/container/container.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.034859 blob-az-0.2.4/src/blob_az/env/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       26 2024-03-17 15:54:16.000000 blob-az-0.2.4/src/blob_az/env/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-03-17 15:52:19.000000 blob-az-0.2.4/src/blob_az/env/keys.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.034859 blob-az-0.2.4/src/blob_az/list/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       35 2024-03-17 14:57:22.000000 blob-az-0.2.4/src/blob_az/list/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      498 2024-04-04 17:57:19.000000 blob-az-0.2.4/src/blob_az/list/list.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.034859 blob-az-0.2.4/src/blob_az/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       56 2024-03-17 14:57:22.000000 blob-az-0.2.4/src/blob_az/util/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-03-17 15:52:48.000000 blob-az-0.2.4/src/blob_az/util/util.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 17:57:39.034859 blob-az-0.2.4/src/blob_az.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1810 2024-04-04 17:57:39.000000 blob-az-0.2.4/src/blob_az.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      505 2024-04-04 17:57:39.000000 blob-az-0.2.4/src/blob_az.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 17:57:39.000000 blob-az-0.2.4/src/blob_az.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       43 2024-04-04 17:57:39.000000 blob-az-0.2.4/src/blob_az.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        8 2024-04-04 17:57:39.000000 blob-az-0.2.4/src/blob_az.egg-info/top_level.txt
```

### Comparing `blob-az-0.2.3/PKG-INFO` & `blob-az-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: blob-az
-Version: 0.2.3
+Version: 0.2.4
 Summary: Async Python SDK for Azure Blob Storage (both block and append blobs)
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: home, https://github.com/moveread/azure-sdks/tree/main/sdks/blob-az
 Project-URL: repo, https://github.com/moveread/azure-sdks
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
-Requires-Dist: haskellian
+Requires-Dist: haskellian-asyn
 
 # Azure Blob
 
 ## Installation
 
 ```bash
 pip install blob-az
```

### Comparing `blob-az-0.2.3/README.md` & `blob-az-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `blob-az-0.2.3/pyproject.toml` & `blob-az-0.2.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blob-az"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Async Python SDK for Azure Blob Storage (both block and append blobs)"
 dependencies = [
-    "azure-storage-blob", "aiohttp", "haskellian"    
+    "azure-storage-blob", "aiohttp", "haskellian-asyn"    
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 home = "https://github.com/moveread/azure-sdks/tree/main/sdks/blob-az"
 repo = "https://github.com/moveread/azure-sdks"
```

### Comparing `blob-az-0.2.3/src/blob_az/blob/blob.py` & `blob-az-0.2.4/src/blob_az/blob/blob.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timedelta
 from azure.storage.blob.aio import BlobServiceClient
 from azure.storage.blob import BlobType, BlobSasPermissions, generate_blob_sas
 from azure.core.exceptions import ResourceNotFoundError
-import haskellian.asynch as hka
+import haskellian.asyn as hka
 from .. import CONN_STR
 from ..container import create as container_create
 from ..util import with_client
 
 @with_client
 async def exists(
     container: str, blob: str,
```

### Comparing `blob-az-0.2.3/src/blob_az/container/container.py` & `blob-az-0.2.4/src/blob_az/container/container.py`

 * *Files identical despite different names*

### Comparing `blob-az-0.2.3/src/blob_az/util/util.py` & `blob-az-0.2.4/src/blob_az/util/util.py`

 * *Files identical despite different names*

### Comparing `blob-az-0.2.3/src/blob_az.egg-info/PKG-INFO` & `blob-az-0.2.4/src/blob_az.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: blob-az
-Version: 0.2.3
+Version: 0.2.4
 Summary: Async Python SDK for Azure Blob Storage (both block and append blobs)
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: home, https://github.com/moveread/azure-sdks/tree/main/sdks/blob-az
 Project-URL: repo, https://github.com/moveread/azure-sdks
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
-Requires-Dist: haskellian
+Requires-Dist: haskellian-asyn
 
 # Azure Blob
 
 ## Installation
 
 ```bash
 pip install blob-az
```

