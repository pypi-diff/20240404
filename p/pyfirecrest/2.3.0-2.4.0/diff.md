# Comparing `tmp/pyfirecrest-2.3.0.tar.gz` & `tmp/pyfirecrest-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfirecrest-2.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyfirecrest-2.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyfirecrest-2.3.0.tar` & `pyfirecrest-2.4.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      549 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1699 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/.github/workflows/testing.yml
--rw-r--r--   0        0        0     2773 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/.gitignore
--rw-r--r--   0        0        0      318 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/.readthedocs.yml
--rw-r--r--   0        0        0     1515 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/LICENSE
--rw-r--r--   0        0        0     3245 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/README.md
--rw-r--r--   0        0        0     2522 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/async-example.md
--rw-r--r--   0        0        0      638 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/Makefile
--rw-r--r--   0        0        0     1639 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/authorization.rst
--rw-r--r--   0        0        0     2012 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/conf.py
--rw-r--r--   0        0        0      786 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/index.rst
--rw-r--r--   0        0        0      678 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/reference_async.rst
--rw-r--r--   0        0        0     1048 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/reference_basic.rst
--rw-r--r--   0        0        0      342 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/reference_cli.rst
--rw-r--r--   0        0        0      129 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/reference_index.rst
--rw-r--r--   0        0        0     4735 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/tutorial_async.rst
--rw-r--r--   0        0        0    10119 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/tutorial_basic.rst
--rw-r--r--   0        0        0     1499 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/tutorial_cli.rst
--rw-r--r--   0        0        0     1523 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/tutorial_errors.rst
--rw-r--r--   0        0        0      165 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/tutorial_index.rst
--rw-r--r--   0        0        0      679 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/docs/source/tutorial_logging.rst
--rw-r--r--   0        0        0    62621 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/firecrest/AsyncClient.py
--rw-r--r--   0        0        0     9887 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/firecrest/AsyncExternalStorage.py
--rw-r--r--   0        0        0     3794 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/firecrest/Authorization.py
--rw-r--r--   0        0        0    56089 2024-03-07 09:58:11.596676 pyfirecrest-2.3.0/firecrest/BasicClient.py
--rw-r--r--   0        0        0     9915 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/ExternalStorage.py
--rw-r--r--   0        0        0     2690 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/FirecrestException.py
--rw-r--r--   0        0        0     1082 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/__init__.py
--rw-r--r--   0        0        0    48797 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/cli/__init__.py
--rw-r--r--   0        0        0      329 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/cli_script.py
--rw-r--r--   0        0        0    22147 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/path.py
--rw-r--r--   0        0        0       26 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/py.typed
--rw-r--r--   0        0        0     3004 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/types.py
--rw-r--r--   0        0        0      268 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/firecrest/utilities.py
--rw-r--r--   0        0        0     1709 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      146 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/common.py
--rw-r--r--   0        0        0      123 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/context.py
--rw-r--r--   0        0        0     3069 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_authorisation.py
--rw-r--r--   0        0        0    44983 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_compute.py
--rw-r--r--   0        0        0    12812 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_compute_async.py
--rw-r--r--   0        0        0    11109 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_extras.py
--rw-r--r--   0        0        0     4808 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_extras_async.py
--rw-r--r--   0        0        0     6326 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_reservation.py
--rw-r--r--   0        0        0     3752 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_reservation_async.py
--rw-r--r--   0        0        0    14130 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_status.py
--rw-r--r--   0        0        0     6207 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_status_async.py
--rw-r--r--   0        0        0    25285 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_storage.py
--rw-r--r--   0        0        0     8947 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_storage_async.py
--rw-r--r--   0        0        0    50807 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_utilities.py
--rw-r--r--   0        0        0    21316 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tests/test_utilities_async.py
--rw-r--r--   0        0        0      255 2024-03-07 09:58:11.600676 pyfirecrest-2.3.0/tox.ini
--rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 pyfirecrest-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0      549 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1699 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0     2773 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/.gitignore
+-rw-r--r--   0        0        0      318 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1515 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/LICENSE
+-rw-r--r--   0        0        0     3245 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/README.md
+-rw-r--r--   0        0        0     2502 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/async-example.md
+-rw-r--r--   0        0        0      638 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/Makefile
+-rw-r--r--   0        0        0     1639 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/authorization.rst
+-rw-r--r--   0        0        0     2012 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0      786 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0      678 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/reference_async.rst
+-rw-r--r--   0        0        0     1048 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/reference_basic.rst
+-rw-r--r--   0        0        0      342 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/reference_cli.rst
+-rw-r--r--   0        0        0      129 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/reference_index.rst
+-rw-r--r--   0        0        0     4735 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_async.rst
+-rw-r--r--   0        0        0    10119 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_basic.rst
+-rw-r--r--   0        0        0     1499 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_cli.rst
+-rw-r--r--   0        0        0     1523 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_errors.rst
+-rw-r--r--   0        0        0      165 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_index.rst
+-rw-r--r--   0        0        0      679 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/docs/source/tutorial_logging.rst
+-rw-r--r--   0        0        0    63287 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/AsyncClient.py
+-rw-r--r--   0        0        0     9887 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/AsyncExternalStorage.py
+-rw-r--r--   0        0        0     3794 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/Authorization.py
+-rw-r--r--   0        0        0    56050 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/BasicClient.py
+-rw-r--r--   0        0        0     9908 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/ExternalStorage.py
+-rw-r--r--   0        0        0     2690 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/FirecrestException.py
+-rw-r--r--   0        0        0     1082 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/__init__.py
+-rw-r--r--   0        0        0    48797 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/cli/__init__.py
+-rw-r--r--   0        0        0      329 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/cli_script.py
+-rw-r--r--   0        0        0    22147 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/path.py
+-rw-r--r--   0        0        0       26 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/py.typed
+-rw-r--r--   0        0        0     3004 2024-04-04 13:04:24.122667 pyfirecrest-2.4.0/firecrest/types.py
+-rw-r--r--   0        0        0      268 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/firecrest/utilities.py
+-rw-r--r--   0        0        0     1709 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      146 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/common.py
+-rw-r--r--   0        0        0      123 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/context.py
+-rw-r--r--   0        0        0     3069 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_authorisation.py
+-rw-r--r--   0        0        0    44983 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_compute.py
+-rw-r--r--   0        0        0    12812 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_compute_async.py
+-rw-r--r--   0        0        0    11109 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_extras.py
+-rw-r--r--   0        0        0     4808 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_extras_async.py
+-rw-r--r--   0        0        0     6326 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_reservation.py
+-rw-r--r--   0        0        0     3752 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_reservation_async.py
+-rw-r--r--   0        0        0    14130 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_status.py
+-rw-r--r--   0        0        0     6207 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_status_async.py
+-rw-r--r--   0        0        0    25285 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_storage.py
+-rw-r--r--   0        0        0     8947 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_storage_async.py
+-rw-r--r--   0        0        0    50807 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_utilities.py
+-rw-r--r--   0        0        0    21316 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tests/test_utilities_async.py
+-rw-r--r--   0        0        0      255 2024-04-04 13:04:24.126667 pyfirecrest-2.4.0/tox.ini
+-rw-r--r--   0        0        0     4855 1970-01-01 00:00:00.000000 pyfirecrest-2.4.0/PKG-INFO
```

### Comparing `pyfirecrest-2.3.0/.github/workflows/python-publish.yml` & `pyfirecrest-2.4.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/.github/workflows/testing.yml` & `pyfirecrest-2.4.0/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/.gitignore` & `pyfirecrest-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/LICENSE` & `pyfirecrest-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/README.md` & `pyfirecrest-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/async-example.md` & `pyfirecrest-2.4.0/async-example.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,22 +47,22 @@
 
 async def main():
     auth = firecrest.ClientCredentialsAuth(client_id, client_secret, token_uri)
     client = firecrest.AsyncFirecrest(firecrest_url, authorization=auth)
 
     # Set up the desired polling rate for each microservice. The float number
     # represents the number of seconds between consecutive requests in each
-    # microservice. Default is 5 seconds for now.
+    # microservice.
     client.time_between_calls = {
-        "compute": 5,
-        "reservations": 5,
-        "status": 5,
-        "storage": 5,
-        "tasks": 5,
-        "utilities": 5,
+        "compute": 1,
+        "reservations": 0.5,
+        "status": 0.5,
+        "storage": 0.5,
+        "tasks": 0.5,
+        "utilities": 0.5,
     }
 
     workflows = [workflow(client, i) for i in range(5)]
     await asyncio.gather(*workflows)
 
 
 asyncio.run(main())
```

### Comparing `pyfirecrest-2.3.0/docs/Makefile` & `pyfirecrest-2.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/authorization.rst` & `pyfirecrest-2.4.0/docs/source/authorization.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/conf.py` & `pyfirecrest-2.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/index.rst` & `pyfirecrest-2.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/reference_async.rst` & `pyfirecrest-2.4.0/docs/source/reference_async.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/reference_basic.rst` & `pyfirecrest-2.4.0/docs/source/reference_basic.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/tutorial_async.rst` & `pyfirecrest-2.4.0/docs/source/tutorial_async.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/tutorial_basic.rst` & `pyfirecrest-2.4.0/docs/source/tutorial_basic.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/tutorial_cli.rst` & `pyfirecrest-2.4.0/docs/source/tutorial_cli.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/tutorial_errors.rst` & `pyfirecrest-2.4.0/docs/source/tutorial_errors.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/docs/source/tutorial_logging.rst` & `pyfirecrest-2.4.0/docs/source/tutorial_logging.rst`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/firecrest/AsyncClient.py` & `pyfirecrest-2.4.0/firecrest/AsyncClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,20 +174,20 @@
         #: client will keep trying until it gets a different status code than 429.
         self.num_retries_rate_limit: Optional[int] = None
         self._api_version: Version = parse("1.13.1")
         self._session = httpx.AsyncClient()
 
         #: Seconds between requests in each microservice
         self.time_between_calls: dict[str, float] = {  # TODO more detailed docs
-            "compute": 5,
-            "reservations": 5,
-            "status": 5,
-            "storage": 5,
-            "tasks": 5,
-            "utilities": 5,
+            "compute": 1,
+            "reservations": 0.1,
+            "status": 0.1,
+            "storage": 0.1,
+            "tasks": 0.1,
+            "utilities": 0.1,
         }
         self._next_request_ts: dict[str, float] = {
             "compute": 0,
             "reservations": 0,
             "status": 0,
             "storage": 0,
             "tasks": 0,
@@ -213,14 +213,30 @@
 
     def set_api_version(self, api_version: str) -> None:
         """Set the version of the api of firecrest. By default it will be assumed that you are
         using version 1.13.1 or compatible. The version is parsed by the `packaging` library.
         """
         self._api_version = parse(api_version)
 
+    async def close_session(self) -> None:
+        """Close the httpx session"""
+        await self._session.aclose()
+
+    async def create_new_session(self) -> None:
+        """Create a new httpx session"""
+        if not self._session.is_closed:
+            await self._session.aclose()
+
+        self._session = httpx.AsyncClient()
+
+    @property
+    def is_session_closed(self) -> bool:
+        """Check if the httpx session is closed"""
+        return self._session.is_closed
+
     @_retry_requests  # type: ignore
     async def _get_request(
         self, endpoint, additional_headers=None, params=None
     ) -> httpx.Response:
         microservice = endpoint.split("/")[1]
         url = f"{self._firecrest_url}{endpoint}"
 
@@ -353,30 +369,35 @@
             )
 
         return resp
 
     @_retry_requests  # type: ignore
     async def _delete_request(
         self, endpoint, additional_headers=None, data=None
-    ) -> requests.Response:
+    ) -> httpx.Response:
         microservice = endpoint.split("/")[1]
         url = f"{self._firecrest_url}{endpoint}"
         async with self._locks[microservice]:
             await self._stall_request(microservice)
             headers = {
                 "Authorization": f"Bearer {self._authorization.get_access_token()}"
             }
             if additional_headers:
                 headers.update(additional_headers)
 
             logger.info(f"Making DELETE request to {endpoint}")
-            # TODO: httpx doesn't support data in delete so we will have to
-            # keep using the `requests` package for this
-            resp = requests.delete(
-                url=url, headers=headers, data=data, timeout=self.timeout
+            # httpx doesn't support data in the `delete` method so we will have to
+            # use the generic `request` method
+            # https://www.python-httpx.org/compatibility/#request-body-on-http-methods
+            resp = await self._session.request(
+                method="DELETE",
+                url=url,
+                headers=headers,
+                data=data,
+                timeout=self.timeout,
             )
             self._next_request_ts[microservice] = (
                 time.time() + self.time_between_calls[microservice]
             )
 
         return resp
```

### Comparing `pyfirecrest-2.3.0/firecrest/AsyncExternalStorage.py` & `pyfirecrest-2.4.0/firecrest/AsyncExternalStorage.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/firecrest/Authorization.py` & `pyfirecrest-2.4.0/firecrest/Authorization.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/firecrest/BasicClient.py` & `pyfirecrest-2.4.0/firecrest/BasicClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -366,16 +366,17 @@
         )
         responses.append(resp)
         return self._json_response(responses, 201, allow_none_result=True)
 
     def _poll_tasks(self, task_id: str, final_status, sleep_time):
         logger.info(f"Polling task {task_id} until status is {final_status}")
         resp = self._task_safe(task_id)
+        t = 1
         while resp["status"] < final_status:
-            t = next(sleep_time)
+            t = next(sleep_time, t)
             logger.info(
                 f'Status of {task_id} is {resp["status"]}, sleeping for {t} sec'
             )
             time.sleep(t)
             resp = self._task_safe(task_id)
 
         logger.info(f'Status of {task_id} is {resp["status"]}')
@@ -999,15 +1000,15 @@
 
             env = json.dumps(env_vars) if env_vars else None
             json_response = self._submit_request(machine, job_script_file, is_local, account, env)
             logger.info(f"Job submission task: {json_response['task_id']}")
 
         # Inject taskid in the result
         result = self._poll_tasks(
-            json_response["task_id"], "200", itertools.cycle([1, 5, 10])
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
         result["firecrest_taskid"] = json_response["task_id"]
         return result
 
     def poll(
         self,
         machine: str,
@@ -1036,15 +1037,15 @@
                 f"`jobs` is meant to be a list, not a string. Will poll for jobs: {[str(j) for j in jobs]}"
             )
 
         jobids = [str(j) for j in jobs] if jobs else []
         json_response = self._acct_request(machine, jobids, start_time, end_time, page_size, page_number)
         logger.info(f"Job polling task: {json_response['task_id']}")
         res = self._poll_tasks(
-            json_response["task_id"], "200", itertools.cycle([1, 5, 10])
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
         # When there is no job in the sacct output firecrest will return an empty dictionary instead of list
         if isinstance(res, dict):
             return list(res.values())
         else:
             return res
 
@@ -1073,15 +1074,15 @@
             )
 
         jobs = jobs if jobs else []
         jobids = [str(j) for j in jobs]
         json_response = self._squeue_request(machine, jobids, page_size, page_number)
         logger.info(f"Job active polling task: {json_response['task_id']}")
         dict_result = self._poll_tasks(
-            json_response["task_id"], "200", itertools.cycle([1, 5, 10])
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
         return list(dict_result.values())
 
     def cancel(self, machine: str, job_id: str | int) -> str:
         """Cancels running job.
         This call uses the `scancel` command.
 
@@ -1096,15 +1097,15 @@
             endpoint=f"/compute/jobs/{job_id}",
             additional_headers={"X-Machine-Name": machine},
         )
         self._current_method_requests.append(resp)
         json_response = self._json_response(self._current_method_requests, 200)
         logger.info(f"Job cancellation task: {json_response['task_id']}")
         return self._poll_tasks(
-            json_response["task_id"], "200", itertools.cycle([1, 5, 10])
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
 
     # Storage
     def _internal_transfer(
         self,
         endpoint,
         machine,
@@ -1173,15 +1174,15 @@
             job_name,
             time,
             stage_out_job_id,
             account,
         )
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
-            json_response["task_id"], "200", itertools.cycle([1, 5, 10])
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
 
     def submit_copy_job(
         self,
         machine: str,
         source_path: str,
         target_path: str,
@@ -1216,15 +1217,15 @@
             job_name,
             time,
             stage_out_job_id,
             account,
         )
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
-            json_response["task_id"], "200", itertools.cycle([1, 5, 10])
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
 
     def submit_rsync_job(
         self,
         machine: str,
         source_path: str,
         target_path: str,
@@ -1259,15 +1260,15 @@
             job_name,
             time,
             stage_out_job_id,
             account,
         )
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
-            json_response["task_id"], "200", itertools.cycle([1, 5, 10])
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
 
     def submit_delete_job(
         self,
         machine: str,
         target_path: str,
         job_name: Optional[str] = None,
@@ -1300,15 +1301,15 @@
             job_name,
             time,
             stage_out_job_id,
             account,
         )
         logger.info(f"Job submission task: {json_response['task_id']}")
         return self._poll_tasks(
-            json_response["task_id"], "200", itertools.cycle([1, 5, 10])
+            json_response["task_id"], "200", iter([1, 0.5, 0.25])
         )
 
     def external_upload(
         self, machine: str, source_path: str, target_path: str
     ) -> ExternalUpload:
         """Non blocking call for the upload of larger files.
```

### Comparing `pyfirecrest-2.3.0/firecrest/ExternalStorage.py` & `pyfirecrest-2.4.0/firecrest/ExternalStorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         previous_responses = [] if previous_responses is None else previous_responses
         self._client = client
         self._task_id = task_id
         self._in_progress = True
         self._status: Optional[str] = None
         self._data = None
         self._object_storage_data = None
-        self._sleep_time = itertools.cycle([1, 5, 10])
+        self._sleep_time = itertools.cycle([1])
         self._responses = previous_responses
 
     @property
     def client(self) -> Firecrest:
         """Returns the client that will be used to get information for the task."""
         return self._client
```

### Comparing `pyfirecrest-2.3.0/firecrest/FirecrestException.py` & `pyfirecrest-2.4.0/firecrest/FirecrestException.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/firecrest/__init__.py` & `pyfirecrest-2.4.0/firecrest/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 #  Please, refer to the LICENSE file in the root directory.
 #  SPDX-License-Identifier: BSD-3-Clause
 #
 import sys
 
 
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 __app_name__ = "firecrest"
 MIN_PYTHON_VERSION = (3, 7, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
     sys.stderr.write(
         "Unsupported Python version: "
```

### Comparing `pyfirecrest-2.3.0/firecrest/cli/__init__.py` & `pyfirecrest-2.4.0/firecrest/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/firecrest/path.py` & `pyfirecrest-2.4.0/firecrest/path.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/firecrest/types.py` & `pyfirecrest-2.4.0/firecrest/types.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/pyproject.toml` & `pyfirecrest-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_authorisation.py` & `pyfirecrest-2.4.0/tests/test_authorisation.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_compute.py` & `pyfirecrest-2.4.0/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_compute_async.py` & `pyfirecrest-2.4.0/tests/test_compute_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_extras.py` & `pyfirecrest-2.4.0/tests/test_extras.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_extras_async.py` & `pyfirecrest-2.4.0/tests/test_extras_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_reservation.py` & `pyfirecrest-2.4.0/tests/test_reservation.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_reservation_async.py` & `pyfirecrest-2.4.0/tests/test_reservation_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_status.py` & `pyfirecrest-2.4.0/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_status_async.py` & `pyfirecrest-2.4.0/tests/test_status_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_storage.py` & `pyfirecrest-2.4.0/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_storage_async.py` & `pyfirecrest-2.4.0/tests/test_storage_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_utilities.py` & `pyfirecrest-2.4.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/tests/test_utilities_async.py` & `pyfirecrest-2.4.0/tests/test_utilities_async.py`

 * *Files identical despite different names*

### Comparing `pyfirecrest-2.3.0/PKG-INFO` & `pyfirecrest-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfirecrest
-Version: 2.3.0
+Version: 2.4.0
 Summary: pyFirecrest is a python wrapper for FirecREST
 Author: CSCS Swiss National Supercomputing Center
 Maintainer-email: Eirini Koutsaniti <eirini.koutsaniti@cscs.ch>, Juan Pablo Dorsch <juanpablo.dorsch@cscs.ch>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

