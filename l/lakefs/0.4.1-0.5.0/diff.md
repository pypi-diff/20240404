# Comparing `tmp/lakefs-0.4.1.tar.gz` & `tmp/lakefs-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakefs-0.4.1.tar", last modified: Mon Feb 26 13:10:59 2024, max compression
+gzip compressed data, was "lakefs-0.5.0.tar", last modified: Thu Apr  4 08:54:32 2024, max compression
```

## Comparing `lakefs-0.4.1.tar` & `lakefs-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0     1001      127        0 2024-02-26 13:10:59.470327 lakefs-0.4.1/
--rw-r--r--   0     1001      127     3695 2024-02-26 13:10:59.470327 lakefs-0.4.1/PKG-INFO
--rw-r--r--   0     1001      127     3199 2024-02-26 13:10:05.000000 lakefs-0.4.1/README.md
-drwxr-xr-x   0     1001      127        0 2024-02-26 13:10:59.462328 lakefs-0.4.1/lakefs/
--rw-r--r--   0     1001      127      931 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/__init__.py
--rw-r--r--   0     1001      127    18144 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/branch.py
--rw-r--r--   0     1001      127     4041 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/client.py
--rw-r--r--   0     1001      127     3172 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/config.py
--rw-r--r--   0     1001      127     4235 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/exceptions.py
--rw-r--r--   0     1001      127     9022 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/import_manager.py
--rw-r--r--   0     1001      127     2810 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/models.py
--rw-r--r--   0     1001      127     1650 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/namedtuple.py
--rw-r--r--   0     1001      127    29651 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/object.py
--rw-r--r--   0     1001      127     8688 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/reference.py
--rw-r--r--   0     1001      127     8167 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/repository.py
--rw-r--r--   0     1001      127     2153 2024-02-26 13:10:05.000000 lakefs-0.4.1/lakefs/tag.py
-drwxr-xr-x   0     1001      127        0 2024-02-26 13:10:59.470327 lakefs-0.4.1/lakefs.egg-info/
--rw-r--r--   0     1001      127     3695 2024-02-26 13:10:59.000000 lakefs-0.4.1/lakefs.egg-info/PKG-INFO
--rw-r--r--   0     1001      127      948 2024-02-26 13:10:59.000000 lakefs-0.4.1/lakefs.egg-info/SOURCES.txt
--rw-r--r--   0     1001      127        1 2024-02-26 13:10:59.000000 lakefs-0.4.1/lakefs.egg-info/dependency_links.txt
--rw-r--r--   0     1001      127       69 2024-02-26 13:10:59.000000 lakefs-0.4.1/lakefs.egg-info/requires.txt
--rw-r--r--   0     1001      127       13 2024-02-26 13:10:59.000000 lakefs-0.4.1/lakefs.egg-info/top_level.txt
--rw-r--r--   0     1001      127       95 2024-02-26 13:10:59.470327 lakefs-0.4.1/setup.cfg
--rw-r--r--   0     1001      127     1183 2024-02-26 13:10:05.000000 lakefs-0.4.1/setup.py
-drwxr-xr-x   0     1001      127        0 2024-02-26 13:10:59.458328 lakefs-0.4.1/tests/
-drwxr-xr-x   0     1001      127        0 2024-02-26 13:10:59.466328 lakefs-0.4.1/tests/integration/
--rw-r--r--   0     1001      127        0 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/integration/__init__.py
--rw-r--r--   0     1001      127     2128 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/integration/conftest.py
--rw-r--r--   0     1001      127     7904 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/integration/test_branch.py
--rw-r--r--   0     1001      127     3284 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/integration/test_import.py
--rw-r--r--   0     1001      127    13965 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/integration/test_object.py
--rw-r--r--   0     1001      127     2754 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/integration/test_reference.py
--rw-r--r--   0     1001      127     1679 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/integration/test_repository.py
--rw-r--r--   0     1001      127     4623 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/integration/test_sanity.py
-drwxr-xr-x   0     1001      127        0 2024-02-26 13:10:59.466328 lakefs-0.4.1/tests/utests/
--rw-r--r--   0     1001      127        0 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/__init__.py
--rw-r--r--   0     1001      127     2373 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/common.py
--rw-r--r--   0     1001      127     6058 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/test_branch.py
--rw-r--r--   0     1001      127     1665 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/test_client.py
--rw-r--r--   0     1001      127     1913 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/test_import.py
--rw-r--r--   0     1001      127     1440 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/test_namedtuple.py
--rw-r--r--   0     1001      127    10028 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/test_object.py
--rw-r--r--   0     1001      127     5167 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/test_reference.py
--rw-r--r--   0     1001      127     5281 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/test_repository.py
--rw-r--r--   0     1001      127      381 2024-02-26 13:10:05.000000 lakefs-0.4.1/tests/utests/test_tag.py
+drwxr-xr-x   0     1001      127        0 2024-04-04 08:54:32.847713 lakefs-0.5.0/
+-rw-r--r--   0     1001      127     3695 2024-04-04 08:54:32.847713 lakefs-0.5.0/PKG-INFO
+-rw-r--r--   0     1001      127     3199 2024-04-04 08:53:46.000000 lakefs-0.5.0/README.md
+drwxr-xr-x   0     1001      127        0 2024-04-04 08:54:32.843713 lakefs-0.5.0/lakefs/
+-rw-r--r--   0     1001      127      931 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/__init__.py
+-rw-r--r--   0     1001      127    18144 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/branch.py
+-rw-r--r--   0     1001      127     5062 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/client.py
+-rw-r--r--   0     1001      127     3172 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/config.py
+-rw-r--r--   0     1001      127     4235 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/exceptions.py
+-rw-r--r--   0     1001      127     9021 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/import_manager.py
+-rw-r--r--   0     1001      127     2810 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/models.py
+-rw-r--r--   0     1001      127     1650 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/namedtuple.py
+-rw-r--r--   0     1001      127    29651 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/object.py
+-rw-r--r--   0     1001      127     8688 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/reference.py
+-rw-r--r--   0     1001      127     8167 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/repository.py
+-rw-r--r--   0     1001      127     2153 2024-04-04 08:53:46.000000 lakefs-0.5.0/lakefs/tag.py
+drwxr-xr-x   0     1001      127        0 2024-04-04 08:54:32.847713 lakefs-0.5.0/lakefs.egg-info/
+-rw-r--r--   0     1001      127     3695 2024-04-04 08:54:32.000000 lakefs-0.5.0/lakefs.egg-info/PKG-INFO
+-rw-r--r--   0     1001      127      948 2024-04-04 08:54:32.000000 lakefs-0.5.0/lakefs.egg-info/SOURCES.txt
+-rw-r--r--   0     1001      127        1 2024-04-04 08:54:32.000000 lakefs-0.5.0/lakefs.egg-info/dependency_links.txt
+-rw-r--r--   0     1001      127       69 2024-04-04 08:54:32.000000 lakefs-0.5.0/lakefs.egg-info/requires.txt
+-rw-r--r--   0     1001      127       13 2024-04-04 08:54:32.000000 lakefs-0.5.0/lakefs.egg-info/top_level.txt
+-rw-r--r--   0     1001      127       95 2024-04-04 08:54:32.847713 lakefs-0.5.0/setup.cfg
+-rw-r--r--   0     1001      127     1183 2024-04-04 08:53:46.000000 lakefs-0.5.0/setup.py
+drwxr-xr-x   0     1001      127        0 2024-04-04 08:54:32.839713 lakefs-0.5.0/tests/
+drwxr-xr-x   0     1001      127        0 2024-04-04 08:54:32.843713 lakefs-0.5.0/tests/integration/
+-rw-r--r--   0     1001      127        0 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/integration/__init__.py
+-rw-r--r--   0     1001      127     2128 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/integration/conftest.py
+-rw-r--r--   0     1001      127     7904 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/integration/test_branch.py
+-rw-r--r--   0     1001      127     3284 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/integration/test_import.py
+-rw-r--r--   0     1001      127    13965 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/integration/test_object.py
+-rw-r--r--   0     1001      127     2754 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/integration/test_reference.py
+-rw-r--r--   0     1001      127     1679 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/integration/test_repository.py
+-rw-r--r--   0     1001      127     4623 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/integration/test_sanity.py
+drwxr-xr-x   0     1001      127        0 2024-04-04 08:54:32.847713 lakefs-0.5.0/tests/utests/
+-rw-r--r--   0     1001      127        0 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/__init__.py
+-rw-r--r--   0     1001      127     2373 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/common.py
+-rw-r--r--   0     1001      127     6058 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/test_branch.py
+-rw-r--r--   0     1001      127     1665 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/test_client.py
+-rw-r--r--   0     1001      127     1913 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/test_import.py
+-rw-r--r--   0     1001      127     1440 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/test_namedtuple.py
+-rw-r--r--   0     1001      127    10028 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/test_object.py
+-rw-r--r--   0     1001      127     5167 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/test_reference.py
+-rw-r--r--   0     1001      127     5281 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/test_repository.py
+-rw-r--r--   0     1001      127      381 2024-04-04 08:53:46.000000 lakefs-0.5.0/tests/utests/test_tag.py
```

### Comparing `lakefs-0.4.1/PKG-INFO` & `lakefs-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs
-Version: 0.4.1
+Version: 0.5.0
 Summary: lakeFS Python SDK Wrapper
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python-wrapper
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API,Python Wrapper
 Requires-Python: >=3.9
```

### Comparing `lakefs-0.4.1/README.md` & `lakefs-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/__init__.py` & `lakefs-0.5.0/lakefs/__init__.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/branch.py` & `lakefs-0.5.0/lakefs/branch.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/client.py` & `lakefs-0.5.0/lakefs/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Optional
 from threading import Lock
 
 import lakefs_sdk
 from lakefs_sdk.client import LakeFSClient
 
 from lakefs.config import ClientConfig
-from lakefs.exceptions import NotAuthorizedException, ServerException
+from lakefs.exceptions import NotAuthorizedException, ServerException, api_exception_handler
 from lakefs.models import ServerStorageConfiguration
 
 
 class ServerConfiguration:
     """
     Represent a lakeFS server's configuration
     """
@@ -102,14 +102,34 @@
         lakeFS Server version, lazy evaluated.
         """
         if self._server_conf is None:
             self._server_conf = ServerConfiguration(self)
         return self._server_conf.version
 
 
+def from_web_identity(code: str, state: str, redirect_uri: str, ttl_seconds: int = 3600, **kwargs) -> Client:
+    """
+    Authenticate against lakeFS using a code received from an identity provider
+
+    :param code: The code received from the identity provider
+    :param state: The state received from the identity provider
+    :param redirect_uri: The redirect URI used in the authentication process
+    :param ttl_seconds: The token's time-to-live in seconds
+    :param kwargs: Remaining arguments for the Client object
+    :return: The authenticated Client object
+    :raise NotAuthorizedException: if user is not authorized to perform this operation
+    """
+    client = Client(**kwargs)
+    sts_requests = lakefs_sdk.StsAuthRequest(code=code, state=state, redirect_uri=redirect_uri, ttl_seconds=ttl_seconds)
+    with api_exception_handler():
+        auth_token = client.sdk_client.experimental_api.sts_login(sts_requests)
+    client.config.access_token = auth_token.token
+    return client
+
+
 class _BaseLakeFSObject:
     """
     Base class for all lakeFS SDK objects, holds the client object and handles errors where no authentication method
     found for client. Attempts to reload client dynamically in case of changes in the environment.
     """
     __mutex: Lock = Lock()
     __client: Optional[Client] = None
```

### Comparing `lakefs-0.4.1/lakefs/config.py` & `lakefs-0.5.0/lakefs/config.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/exceptions.py` & `lakefs-0.5.0/lakefs/exceptions.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/import_manager.py` & `lakefs-0.5.0/lakefs/import_manager.py`

 * *Files identical despite different names*

```diff
@@ -118,25 +118,24 @@
             self._import_id = res.id
             self._in_progress = True
 
         return self._import_id
 
     async def _wait_for_completion(self, poll_interval: timedelta) -> lakefs_sdk.ImportStatus:
         while True:
+            await asyncio.sleep(poll_interval.total_seconds())
             with api_exception_handler():
                 resp = self._client.sdk_client.import_api.import_status(repository=self._repo_id,
                                                                         branch=self._branch_id,
                                                                         id=self._import_id)
             if resp.completed:
                 return resp
             if resp.error is not None:
                 raise ImportManagerException(f"Import Error: {resp.error.message}")
 
-            await asyncio.sleep(poll_interval.total_seconds())
-
     def wait(self, poll_interval: Optional[timedelta] = timedelta(seconds=2)) -> ImportStatus:
         """
         Poll a started import task ID, blocking until completion
 
         :param poll_interval: The interval for polling the import status.
         :return: Import status as returned by the lakeFS server
         :raise ImportManagerException: if no import is in progress
```

### Comparing `lakefs-0.4.1/lakefs/models.py` & `lakefs-0.5.0/lakefs/models.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/namedtuple.py` & `lakefs-0.5.0/lakefs/namedtuple.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/object.py` & `lakefs-0.5.0/lakefs/object.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/reference.py` & `lakefs-0.5.0/lakefs/reference.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/repository.py` & `lakefs-0.5.0/lakefs/repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs/tag.py` & `lakefs-0.5.0/lakefs/tag.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/lakefs.egg-info/PKG-INFO` & `lakefs-0.5.0/lakefs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs
-Version: 0.4.1
+Version: 0.5.0
 Summary: lakeFS Python SDK Wrapper
 Home-page: https://github.com/treeverse/lakeFS/tree/master/clients/python-wrapper
 Author: Treeverse
 Author-email: services@treeverse.io
 License: Apache 2.0
 Keywords: OpenAPI,OpenAPI-Generator,lakeFS API,Python Wrapper
 Requires-Python: >=3.9
```

### Comparing `lakefs-0.4.1/lakefs.egg-info/SOURCES.txt` & `lakefs-0.5.0/lakefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/setup.py` & `lakefs-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "lakefs"
-VERSION = "0.4.1"
+VERSION = "0.5.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `lakefs-0.4.1/tests/integration/conftest.py` & `lakefs-0.5.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/integration/test_branch.py` & `lakefs-0.5.0/tests/integration/test_branch.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/integration/test_import.py` & `lakefs-0.5.0/tests/integration/test_import.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/integration/test_object.py` & `lakefs-0.5.0/tests/integration/test_object.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/integration/test_reference.py` & `lakefs-0.5.0/tests/integration/test_reference.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/integration/test_repository.py` & `lakefs-0.5.0/tests/integration/test_repository.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/integration/test_sanity.py` & `lakefs-0.5.0/tests/integration/test_sanity.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/utests/common.py` & `lakefs-0.5.0/tests/utests/common.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/utests/test_branch.py` & `lakefs-0.5.0/tests/utests/test_branch.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/utests/test_client.py` & `lakefs-0.5.0/tests/utests/test_client.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/utests/test_import.py` & `lakefs-0.5.0/tests/utests/test_import.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/utests/test_namedtuple.py` & `lakefs-0.5.0/tests/utests/test_namedtuple.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/utests/test_object.py` & `lakefs-0.5.0/tests/utests/test_object.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/utests/test_reference.py` & `lakefs-0.5.0/tests/utests/test_reference.py`

 * *Files identical despite different names*

### Comparing `lakefs-0.4.1/tests/utests/test_repository.py` & `lakefs-0.5.0/tests/utests/test_repository.py`

 * *Files identical despite different names*

