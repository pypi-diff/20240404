# Comparing `tmp/mostlyai-0.3.0.tar.gz` & `tmp/mostlyai-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mostlyai-0.3.0.tar", max compression
+gzip compressed data, was "mostlyai-0.3.1.tar", max compression
```

## Comparing `mostlyai-0.3.0.tar` & `mostlyai-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-03-08 15:08:04.881678 mostlyai-0.3.0/LICENSE
--rw-r--r--   0        0        0     2221 2024-03-19 14:08:19.117513 mostlyai-0.3.0/README.md
--rw-r--r--   0        0        0       26 2024-03-19 14:08:19.064057 mostlyai-0.3.0/mostlyai/__init__.py
--rw-r--r--   0        0        0    12586 2024-03-19 14:08:19.081011 mostlyai-0.3.0/mostlyai/api.py
--rw-r--r--   0        0        0     9037 2024-03-19 14:08:19.088066 mostlyai-0.3.0/mostlyai/base.py
--rw-r--r--   0        0        0     2667 2024-03-19 14:08:19.061597 mostlyai-0.3.0/mostlyai/connectors.py
--rw-r--r--   0        0        0      574 2024-03-19 14:08:19.083253 mostlyai-0.3.0/mostlyai/exceptions.py
--rw-r--r--   0        0        0     3986 2024-03-19 14:08:19.079843 mostlyai-0.3.0/mostlyai/generators.py
--rw-r--r--   0        0        0    38859 2024-03-19 14:08:19.079179 mostlyai-0.3.0/mostlyai/model.py
--rw-r--r--   0        0        0     1742 2024-03-19 14:08:19.085558 mostlyai-0.3.0/mostlyai/shares.py
--rw-r--r--   0        0        0     7008 2024-03-19 14:08:19.063174 mostlyai-0.3.0/mostlyai/synthetic_datasets.py
--rw-r--r--   0        0        0     5217 2024-03-19 14:08:19.082058 mostlyai-0.3.0/mostlyai/utils.py
--rw-r--r--   0        0        0     1263 2024-03-19 14:08:19.113999 mostlyai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 mostlyai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-12-22 12:47:38.462094 mostlyai-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2303 2024-04-02 17:48:15.885881 mostlyai-0.3.1/README.md
+-rw-r--r--   0        0        0       26 2024-03-13 18:10:22.492378 mostlyai-0.3.1/mostlyai/__init__.py
+-rw-r--r--   0        0        0    13016 2024-04-04 19:13:15.035679 mostlyai-0.3.1/mostlyai/api.py
+-rw-r--r--   0        0        0     9150 2024-04-04 19:13:15.037096 mostlyai-0.3.1/mostlyai/base.py
+-rw-r--r--   0        0        0     2667 2024-03-13 19:00:02.355471 mostlyai-0.3.1/mostlyai/connectors.py
+-rw-r--r--   0        0        0      574 2024-03-13 19:00:02.358865 mostlyai-0.3.1/mostlyai/exceptions.py
+-rw-r--r--   0        0        0     3986 2024-03-13 19:00:02.362753 mostlyai-0.3.1/mostlyai/generators.py
+-rw-r--r--   0        0        0    38859 2024-03-22 06:46:58.727500 mostlyai-0.3.1/mostlyai/model.py
+-rw-r--r--   0        0        0     1742 2024-03-22 06:46:58.729767 mostlyai-0.3.1/mostlyai/shares.py
+-rw-r--r--   0        0        0     7008 2024-03-13 19:00:02.364822 mostlyai-0.3.1/mostlyai/synthetic_datasets.py
+-rw-r--r--   0        0        0     5217 2024-03-13 18:10:22.527374 mostlyai-0.3.1/mostlyai/utils.py
+-rw-r--r--   0        0        0     1264 2024-04-04 19:22:11.858836 mostlyai-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 mostlyai-0.3.1/PKG-INFO
```

### Comparing `mostlyai-0.3.0/LICENSE` & `mostlyai-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.0/README.md` & `mostlyai-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 | Intent                                          | Primitive                  |
 |-------------------------------------------------|----------------------------|
 | Train a Generative AI on tabular data           | `g = mostly.train(data)`   |
 | Empower your team with safe synthetic data      | `mostly.share(g, email)`   |
 | Generate unlimited synthetic data on demand     | `mostly.generate(g, size)` |
 | Prompt the generator for the data that you need | `mostly.generate(g, seed)` |
 | Connect to any data source within your org      | `mostly.connect(config)`   |
+| Info about the current user                     | `mostly.me()`              |
+
 
 
 
 ## Installation
 ```shell
 pip install mostlyai
 ```
```

### Comparing `mostlyai-0.3.0/mostlyai/api.py` & `mostlyai-0.3.1/mostlyai/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from pathlib import Path
 from typing import Any, Optional, Union
 
 import pandas as pd
 import rich
 
-from mostlyai.base import _MostlyBaseClient
+from mostlyai.base import GET, _MostlyBaseClient
 from mostlyai.connectors import _MostlyConnectorsClient
 from mostlyai.generators import _MostlyGeneratorsClient
 from mostlyai.model import (
     Connector,
+    CurrentUser,
     Generator,
     PermissionLevel,
     ProgressStatus,
     SyntheticDataset,
 )
 from mostlyai.shares import _MostlySharesClient
 from mostlyai.synthetic_datasets import _MostlySyntheticDatasetsClient
@@ -26,27 +27,32 @@
 class MostlyAI(_MostlyBaseClient):
     """
     Client for interacting with the Mostly AI Public API.
 
     :param base_url: The base URL. If not provided, a default value is used.
     :param api_key: The API key for authenticating. If not provided, it would rely on env vars.
     :param timeout: Timeout for HTTPS requests in seconds.
+    :param ssl_verify: Whether to verify SSL certificates.
     """
 
     def __init__(
         self,
         base_url: Optional[str] = None,
         api_key: Optional[str] = None,
         timeout: float = 60.0,
+        ssl_verify: bool = True,
     ):
-        super().__init__(base_url=base_url, api_key=api_key, timeout=timeout)
+        super().__init__(
+            base_url=base_url, api_key=api_key, timeout=timeout, ssl_verify=ssl_verify
+        )
         client_kwargs = {
             "base_url": self.base_url,
             "api_key": self.api_key,
             "timeout": self.timeout,
+            "ssl_verify": self.ssl_verify,
         }
         self.connectors = _MostlyConnectorsClient(**client_kwargs)
         self.generators = _MostlyGeneratorsClient(**client_kwargs)
         self.synthetic_datasets = _MostlySyntheticDatasetsClient(**client_kwargs)
         self.shares = _MostlySharesClient(**client_kwargs)
 
     def connect(self, config: dict[str, Any]) -> Connector:
@@ -317,7 +323,15 @@
 
         :return: None. The function outputs a confirmation message with the details of the revocation action.
         """
         self.shares._unshare(resource, user_email)
         rich.print(
             f"Revoked access of resource [bold cyan]{resource.id}[/] for [bold]{user_email}[/]"
         )
+
+    def me(self) -> CurrentUser:
+        """
+        Retrieve current user info.
+
+        :return: info about the current user.
+        """
+        return self.request(verb=GET, path=["users", "me"], response_type=CurrentUser)
```

### Comparing `mostlyai-0.3.0/mostlyai/base.py` & `mostlyai-0.3.1/mostlyai/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,27 @@
     SECTION = []
 
     def __init__(
         self,
         base_url: Optional[str] = None,
         api_key: Optional[str] = None,
         timeout: float = 60.0,
+        ssl_verify: bool = True,
     ):
         self.base_url = (
             base_url or os.getenv("MOSTLY_BASE_URL") or DEFAULT_BASE_URL
         ).rstrip("/")
         self.api_key = api_key or os.getenv("MOSTLY_API_KEY")
         self.timeout = timeout
+        self.ssl_verify = ssl_verify
         if not self.api_key:
-            raise APIError("The API key must be either set by passing api_key to the client or by specifying a "
-                           "MOSTLY_API_KEY environment variable")
+            raise APIError(
+                "The API key must be either set by passing api_key to the client or by specifying a "
+                "MOSTLY_API_KEY environment variable"
+            )
 
     def headers(self):
         return {
             "Accept": "application/json",
             "X-MOSTLY-API-KEY": self.api_key,
         }
 
@@ -98,15 +102,15 @@
 
         if (request_size := _get_total_size(kwargs)) > MAX_REQUEST_SIZE:
             warnings.warn(
                 f"The overall {request_size=} exceeds {MAX_REQUEST_SIZE}.", UserWarning
             )
 
         try:
-            with httpx.Client(timeout=self.timeout) as client:
+            with httpx.Client(timeout=self.timeout, verify=self.ssl_verify) as client:
                 response = client.request(method=verb, url=full_url, **kwargs)
             response.raise_for_status()
         except httpx.HTTPStatusError as exc:
             try:
                 error_msg = exc.response.json()["message"]
             except Exception:
                 error_msg = exc.response.content
```

### Comparing `mostlyai-0.3.0/mostlyai/connectors.py` & `mostlyai-0.3.1/mostlyai/connectors.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.0/mostlyai/exceptions.py` & `mostlyai-0.3.1/mostlyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.0/mostlyai/generators.py` & `mostlyai-0.3.1/mostlyai/generators.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.0/mostlyai/model.py` & `mostlyai-0.3.1/mostlyai/model.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.0/mostlyai/shares.py` & `mostlyai-0.3.1/mostlyai/shares.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.0/mostlyai/synthetic_datasets.py` & `mostlyai-0.3.1/mostlyai/synthetic_datasets.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.0/mostlyai/utils.py` & `mostlyai-0.3.1/mostlyai/utils.py`

 * *Files identical despite different names*

### Comparing `mostlyai-0.3.0/pyproject.toml` & `mostlyai-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mostlyai"
-version = "0.3.0"
+version = "0.3.1"
 description = "The official Python client for the MOSTLY AI platform."
 homepage = "https://app.mostly.ai/"
 authors = ["MOSTLY AI <office@mostly.ai>"]
 license = "Proprietary"
 readme = "README.md"
 packages = [
     { include = "mostlyai" }
@@ -48,10 +48,11 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "poetry"
 update_changelog_on_bump = true
 major_version_zero = true
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mostlyai-0.3.0/PKG-INFO` & `mostlyai-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostlyai
-Version: 0.3.0
+Version: 0.3.1
 Summary: The official Python client for the MOSTLY AI platform.
 Home-page: https://app.mostly.ai/
 License: Proprietary
 Author: MOSTLY AI
 Author-email: office@mostly.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -27,14 +27,16 @@
 | Intent                                          | Primitive                  |
 |-------------------------------------------------|----------------------------|
 | Train a Generative AI on tabular data           | `g = mostly.train(data)`   |
 | Empower your team with safe synthetic data      | `mostly.share(g, email)`   |
 | Generate unlimited synthetic data on demand     | `mostly.generate(g, size)` |
 | Prompt the generator for the data that you need | `mostly.generate(g, seed)` |
 | Connect to any data source within your org      | `mostly.connect(config)`   |
+| Info about the current user                     | `mostly.me()`              |
+
 
 
 
 ## Installation
 ```shell
 pip install mostlyai
 ```
```

