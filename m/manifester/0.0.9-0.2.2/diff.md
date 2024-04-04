# Comparing `tmp/manifester-0.0.9.tar.gz` & `tmp/manifester-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifester-0.0.9.tar", last modified: Tue Oct 18 18:50:46 2022, max compression
+gzip compressed data, was "manifester-0.2.2.tar", last modified: Thu Apr  4 18:37:18 2024, max compression
```

## Comparing `manifester-0.0.9.tar` & `manifester-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.781584 manifester-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-18 18:50:30.000000 manifester-0.0.9/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.777584 manifester-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.777584 manifester-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-10-18 18:50:30.000000 manifester-0.0.9/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-10-18 18:50:30.000000 manifester-0.0.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-10-18 18:50:30.000000 manifester-0.0.9/.github/workflows/update_manifester_image.yml
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-10-18 18:50:30.000000 manifester-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-10-18 18:50:30.000000 manifester-0.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-10-18 18:50:30.000000 manifester-0.0.9/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-18 18:50:30.000000 manifester-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-10-18 18:50:46.781584 manifester-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-10-18 18:50:30.000000 manifester-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.777584 manifester-0.0.9/logs/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-18 18:50:30.000000 manifester-0.0.9/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.781584 manifester-0.0.9/manifester/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)    16451 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/manifester.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 18:50:46.781584 manifester-0.0.9/manifester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3971 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 18:50:45.000000 manifester-0.0.9/manifester.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-18 18:50:46.000000 manifester-0.0.9/manifester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-10-18 18:50:30.000000 manifester-0.0.9/manifester_settings.yaml.example
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-10-18 18:50:46.781584 manifester-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-10-18 18:50:30.000000 manifester-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.527105 manifester-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 18:37:03.000000 manifester-0.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.523105 manifester-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-04 18:37:03.000000 manifester-0.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.523105 manifester-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 18:37:03.000000 manifester-0.2.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-04 18:37:03.000000 manifester-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-04 18:37:03.000000 manifester-0.2.2/.github/workflows/update_manifester_image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-04 18:37:03.000000 manifester-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-04 18:37:03.000000 manifester-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-04 18:37:03.000000 manifester-0.2.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 18:37:03.000000 manifester-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19631 2024-04-04 18:37:18.527105 manifester-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-04 18:37:03.000000 manifester-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.523105 manifester-0.2.2/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 18:37:03.000000 manifester-0.2.2/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.527105 manifester-0.2.2/manifester/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/manifester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.527105 manifester-0.2.2/manifester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19631 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester_inventory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester_settings.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-04 18:37:03.000000 manifester-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:37:18.527105 manifester-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.527105 manifester-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-04 18:37:03.000000 manifester-0.2.2/tests/test_manifester.py
```

### Comparing `manifester-0.0.9/.github/workflows/codeql-analysis.yml` & `manifester-0.2.2/.github/workflows/codeql-analysis.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 name: "CodeQL"
 
 on:
   push:
     branches: [master]
   pull_request:
     types: [opened, synchronize, reopened]
+    paths-ignore:
+        - "*.md"
+        - "*.example"
+        - ".gitignore"
 
 jobs:
   analyze:
     name: CodeQL Analysis
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.10", "3.11", "3.12"]
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
+      with:
+        ref: ${{ github.ref }}
 
     - name: Initialize CodeQL
-      uses: github/codeql-action/init@v1
+      uses: github/codeql-action/init@v3
       with:
         languages: ${{ matrix.language }}
 
     - name: Perform CodeQL Analysis
-      uses: github/codeql-action/analyze@v1
+      uses: github/codeql-action/analyze@v3
 
     - name: Setup Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Unit Tests
       run: |
         pip install -U pip
-        # pip install -U .[test]
+        pip install -U .[test]
         cp manifester_settings.yaml.example manifester_settings.yaml
-        # pytest -v tests/ --ignore tests/functional
+        pytest -v tests/
```

### Comparing `manifester-0.0.9/.github/workflows/python-publish.yml` & `manifester-0.2.2/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 jobs:
   publish:
     name: Build and Deploy to PyPi
     runs-on: ubuntu-latest
     strategy:
       matrix:
         # build/push in lowest support python version
-        python-version: [ 3.8 ]
+        python-version: [ "3.10" ]
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
 
-    - uses: actions/setup-python@v2
+    - uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Setup and Build
       run: |
         pip install -U pip
         pip install .[setup]
-        python setup.py sdist bdist_wheel
+        python -m build
         python -m twine check dist/*
 
     - name: Build and publish
-      uses: pypa/gh-action-pypi-publish@release/v1
+      uses: pypa/gh-action-pypi-publish@v1.8.14
       with:
         user: __token__
         password: ${{ secrets.PYPI_TOKEN }}
         skip_existing: true
```

### Comparing `manifester-0.0.9/.github/workflows/update_manifester_image.yml` & `manifester-0.2.2/.github/workflows/update_manifester_image.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 jobs:
   manifester_container:
     name: Update Manifester container image on Quay.
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
 
       - name: Set up QEMU
-        uses: docker/setup-qemu-action@v1
+        uses: docker/setup-qemu-action@v3
 
       - name: Set up Docker Buildx
-        uses: docker/setup-buildx-action@v1
+        uses: docker/setup-buildx-action@v3
 
       - name: Login to Quay Container Registry
-        uses: docker/login-action@v1
+        uses: docker/login-action@v3
         with:
           registry: ${{ secrets.QUAY_SERVER }}
           username: ${{ secrets.QUAY_USERNAME }}
           password: ${{ secrets.QUAY_PASSWORD }}
 
       - name: Build and push image to Quay
-        uses: docker/build-push-action@v2
+        uses: docker/build-push-action@v5
         with:
           file: ./Dockerfile
           push: true
           tags: ${{ secrets.QUAY_SERVER }}/${{ secrets.QUAY_NAMESPACE }}/manifester:latest
```

### Comparing `manifester-0.0.9/.gitignore` & `manifester-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `manifester-0.0.9/LICENSE` & `manifester-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `manifester-0.0.9/manifester/logger.py` & `manifester-0.2.2/manifester/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,24 @@
+"""Defines manifester's internal logging."""
 import logging
+from pathlib import Path
 
 import logzero
 
-from manifester.settings import settings
-
 
 def setup_logzero(level="info", path="logs/manifester.log", silent=True):
+    """Call logzero setup with the given settings."""
+    Path(path).parent.mkdir(parents=True, exist_ok=True)
     log_fmt = "%(color)s[%(levelname)s %(asctime)s]%(end_color)s %(message)s"
     debug_fmt = (
-        "%(color)s[%(levelname)1.1s %(asctime)s %(module)s:%(lineno)d]"
-        "%(end_color)s %(message)s"
+        "%(color)s[%(levelname)1.1s %(asctime)s %(module)s:%(lineno)d]%(end_color)s %(message)s"
     )
     log_level = getattr(logging, level.upper(), logging.INFO)
     # formatter for terminal
-    formatter = logzero.LogFormatter(
-        fmt=debug_fmt if log_level is logging.DEBUG else log_fmt
-    )
-    logzero.setup_default_logger(formatter=formatter, disableStderrLogger=silent)
+    formatter = logzero.LogFormatter(fmt=debug_fmt if log_level is logging.DEBUG else log_fmt)
+    logzero.setup_logger(formatter=formatter, disableStderrLogger=silent)
     logzero.loglevel(log_level)
     # formatter for file
     formatter = logzero.LogFormatter(
         fmt=debug_fmt if log_level is logging.DEBUG else log_fmt, color=False
     )
-    logzero.logfile(
-        path, loglevel=log_level, maxBytes=1e9, backupCount=3, formatter=formatter
-    )
-
-
-setup_logzero(level=settings.get("log_level", "info"))
+    logzero.logfile(path, loglevel=log_level, maxBytes=1e9, backupCount=3, formatter=formatter)
```

### Comparing `manifester-0.0.9/manifester/manifester.py` & `manifester-0.2.2/manifester/manifester.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,260 +1,290 @@
-import random
-import string
-from dynaconf.utils.boxing import DynaBox
+"""Main interface for the RHSM API.
+
+This module defines the `Manifester` class, which provides methods for authenticating to and
+interacting with the RHSM Subscription API for the purpose of generating a subscription manifest.
+"""
 from functools import cached_property
 from pathlib import Path
+import random
+import string
 
-import requests
+from dynaconf.utils.boxing import DynaBox
 from logzero import logger
+from requests.exceptions import Timeout
 
-from manifester.helpers import simple_retry
-from manifester.helpers import process_sat_version
+from manifester.helpers import (
+    fetch_paginated_data,
+    process_sat_version,
+    simple_retry,
+    update_inventory,
+)
 from manifester.logger import setup_logzero
 from manifester.settings import settings
 
+setup_logzero(level=settings.get("log_level", "info"))
+
 
 class Manifester:
-    def __init__(self, manifest_category, allocation_name=None, **kwargs):
-        if isinstance(manifest_category, dict):
-            self.manifest_data = DynaBox(manifest_category)
+    """Main Manifester class responsible for generating a manifest from the provided settings."""
+
+    def __init__(
+        self,
+        manifest_category=None,
+        allocation_name=None,
+        minimal_init=False,
+        proxies=None,
+        **kwargs,
+    ):
+        if minimal_init:
+            self.offline_token = settings.get("offline_token")
+            self.token_request_url = settings.get("url").get("token_request")
+            self.allocations_url = settings.get("url").get("allocations")
+            self._access_token = None
+            self._allocations = None
+            self.token_request_data = {
+                "grant_type": "refresh_token",
+                "client_id": "rhsm-api",
+                "refresh_token": self.offline_token,
+            }
+            self.manifest_data = {"proxies": proxies}
+            self.username_prefix = settings.get("username_prefix")
+            if kwargs.get("requester") is not None:
+                self.requester = kwargs["requester"]
+                self.is_mock = True
+            else:
+                import requests
+
+                self.requester = requests
+                self.is_mock = False
         else:
-            self.manifest_data = settings.manifest_category.get(manifest_category)
-        self.allocation_name = allocation_name or "".join(
-            random.sample(string.ascii_letters, 10)
-        )
-        self.offline_token = kwargs.get("offline_token", self.manifest_data.offline_token)
-        self.subscription_data = self.manifest_data.subscription_data
-        self.token_request_data = {
-            "grant_type": "refresh_token",
-            "client_id": "rhsm-api",
-            "refresh_token": self.offline_token,
-        }
-        self.simple_content_access = kwargs.get(
-            "simple_content_access", self.manifest_data.simple_content_access
-        )
-        self.token_request_url = self.manifest_data.get("url", {}).get("token_request", settings.url.token_request)
-        self.allocations_url = self.manifest_data.get("url", {}).get("allocations", settings.url.allocations)
-        self._access_token = None
-        self._subscription_pools = None
-        self.sat_version = process_sat_version(
-            kwargs.get("sat_version", self.manifest_data.sat_version),
-            self.valid_sat_versions,
-        )
+            if isinstance(manifest_category, dict):
+                self.manifest_data = DynaBox(manifest_category)
+            else:
+                self.manifest_data = settings.manifest_category.get(manifest_category)
+            if kwargs.get("requester") is not None:
+                self.requester = kwargs["requester"]
+                self.is_mock = True
+            else:
+                import requests
+
+                self.requester = requests
+                self.is_mock = False
+            self.username_prefix = (
+                self.manifest_data.get("username_prefix") or settings.username_prefix
+            )
+            self.allocation_name = allocation_name or f"{self.username_prefix}-" + "".join(
+                random.sample(string.ascii_letters, 8)
+            )
+            self.manifest_name = Path(f"{self.allocation_name}_manifest.zip")
+            self.offline_token = self.manifest_data.get(
+                "offline_token", settings.get("offline_token")
+            )
+            self.subscription_data = self.manifest_data.subscription_data
+            self.token_request_data = {
+                "grant_type": "refresh_token",
+                "client_id": "rhsm-api",
+                "refresh_token": self.offline_token,
+            }
+            self.simple_content_access = kwargs.get(
+                "simple_content_access", self.manifest_data.simple_content_access
+            )
+            self.token_request_url = self.manifest_data.get("url").get("token_request")
+            self.allocations_url = self.manifest_data.get("url").get("allocations")
+            self._access_token = None
+            self._allocations = None
+            self._subscription_pools = None
+            self._active_pools = []
+            self.sat_version = process_sat_version(
+                kwargs.get("sat_version", self.manifest_data.sat_version),
+                self.valid_sat_versions,
+            )
 
     @property
     def access_token(self):
+        """Representation of an RHSM API access token.
+
+        Used to authenticate requests to the RHSM API.
+        """
         if not self._access_token:
             token_request_data = {"data": self.token_request_data}
             logger.debug("Generating access token")
             token_data = simple_retry(
-                requests.post,
+                self.requester.post,
                 cmd_args=[f"{self.token_request_url}"],
                 cmd_kwargs=token_request_data,
             ).json()
-            self._access_token = token_data["access_token"]
+            if self.is_mock:
+                self._access_token = token_data.access_token
+            else:
+                self._access_token = token_data["access_token"]
         return self._access_token
-    
+
     @cached_property
     def valid_sat_versions(self):
+        """Retrieves the list of valid Satellite versions from the RHSM API."""
         headers = {
             "headers": {"Authorization": f"Bearer {self.access_token}"},
-            "proxies": self.manifest_data.get("proxies", settings.proxies),
+            "proxies": self.manifest_data.get("proxies"),
         }
-        valid_sat_versions = []
         sat_versions_response = simple_retry(
-            requests.get,
-            cmd_args=[
-                    f"{self.allocations_url}/versions"
-                ],
+            self.requester.get,
+            cmd_args=[f"{self.allocations_url}/versions"],
             cmd_kwargs=headers,
-            ).json()
-        for ver_dict in sat_versions_response["body"]:
-            valid_sat_versions.append(ver_dict["value"])
+        ).json()
+        if self.is_mock:
+            sat_versions_response = sat_versions_response.version_response
+        valid_sat_versions = [ver_dict["value"] for ver_dict in sat_versions_response["body"]]
         return valid_sat_versions
 
+    @property
+    def subscription_allocations(self):
+        """Representation of subscription allocations in an account.
+
+        Filtered by username_prefix.
+        """
+        return fetch_paginated_data(self, "allocations")
+
+    @property
+    def subscription_pools(self):
+        """Representation of subscription pools in an account."""
+        return fetch_paginated_data(self, "pools")
+
     def create_subscription_allocation(self):
+        """Creates a new consumer in the provided RHSM account and returns its UUID."""
         allocation_data = {
             "headers": {"Authorization": f"Bearer {self.access_token}"},
-            "proxies": self.manifest_data.get("proxies", settings.proxies),
+            "proxies": self.manifest_data.get("proxies"),
             "params": {
                 "name": f"{self.allocation_name}",
                 "version": f"{self.sat_version}",
                 "simpleContentAccess": f"{self.simple_content_access}",
             },
         }
         self.allocation = simple_retry(
-            requests.post,
+            self.requester.post,
             cmd_args=[f"{self.allocations_url}"],
             cmd_kwargs=allocation_data,
         ).json()
-        logger.debug(
-            f"Received response {self.allocation} when attempting to create allocation."
-        )
-        if ("error" in self.allocation.keys() and 
-            "invalid version" in self.allocation['error'].values()):
-            raise ValueError(
-                                f"{self.sat_version} is not a valid version number."
-                                "Versions must be in the form of \"sat-X.Y\". Current"
-                                f"valid versions are {self.valid_sat_versions}."
-                            )
+        logger.debug(f"Received response {self.allocation} when attempting to create allocation.")
         self.allocation_uuid = self.allocation["body"]["uuid"]
         if self.simple_content_access == "disabled":
             simple_retry(
-                requests.put,
+                self.requester.put,
                 cmd_args=[f"{self.allocations_url}/{self.allocation_uuid}"],
                 cmd_kwargs={
                     "headers": {"Authorization": f"Bearer {self.access_token}"},
-                    "proxies": self.manifest_data.get("proxies", settings.proxies),
+                    "proxies": self.manifest_data.get("proxies"),
                     "json": {"simpleContentAccess": "disabled"},
                 },
             )
         logger.info(
             f"Subscription allocation created with name {self.allocation_name} "
             f"and UUID {self.allocation_uuid}"
         )
+        update_inventory(self.subscription_allocations)
         return self.allocation_uuid
 
-    def delete_subscription_allocation(self):
+    def delete_subscription_allocation(self, uuid=None):
+        """Deletes the specified subscription allocation and returns the RHSM API's response."""
         self._access_token = None
         data = {
             "headers": {"Authorization": f"Bearer {self.access_token}"},
-            "proxies": self.manifest_data.get("proxies", settings.proxies),
+            "proxies": self.manifest_data.get("proxies"),
             "params": {"force": "true"},
         }
+        if self.is_mock:
+            self.allocation_uuid = self.allocation_uuid.uuid
         response = simple_retry(
-            requests.delete,
-            cmd_args=[f"{self.allocations_url}/{self.allocation_uuid}"],
+            self.requester.delete,
+            cmd_args=[f"{self.allocations_url}/{uuid if uuid else self.allocation_uuid}"],
             cmd_kwargs=data,
         )
+        update_inventory(self.subscription_allocations)
         return response
 
-    @property
-    def subscription_pools(self):
-        if not self._subscription_pools:
-            _offset = 0
-            data = {
-                "headers": {"Authorization": f"Bearer {self.access_token}"},
-                "proxies": self.manifest_data.get("proxies", settings.proxies),
-                "params": {"offset": _offset},
-            }
-            self._subscription_pools = simple_retry(
-                requests.get,
-                cmd_args=[
-                    f"{self.allocations_url}/{self.allocation_uuid}/pools"
-                ],
-                cmd_kwargs=data,
-            ).json()
-            _results = len(self._subscription_pools["body"])
-            # The endpoint used in the above API call can return a maximum of 50 subscription pools.
-            # For organizations with more than 50 subscription pools, the loop below works around
-            # this limit by repeating calls with a progressively larger value for the `offset`
-            # parameter.
-            while _results == 50:
-                _offset += 50
-                logger.debug(
-                    f"Fetching additional subscription pools with an offset of {_offset}."
-                )
-                data = {
-                    "headers": {"Authorization": f"Bearer {self.access_token}"},
-                    "proxies": self.manifest_data.get("proxies", settings.proxies),
-                    "params": {"offset": _offset},
-                }
-                offset_pools = simple_retry(
-                    requests.get,
-                    cmd_args=[
-                        f"{self.allocations_url}/{self.allocation_uuid}/pools"
-                    ],
-                    cmd_kwargs=data,
-                ).json()
-                self._subscription_pools["body"] += offset_pools["body"]
-                _results = len(offset_pools["body"])
-                total_pools = len(self._subscription_pools["body"])
-                logger.debug(
-                    f"Total subscription pools available for this allocation: {total_pools}"
-                )
-        return self._subscription_pools
-
     def add_entitlements_to_allocation(self, pool_id, entitlement_quantity):
+        """Attempts to add the set of subscriptions defined in the settings to the allocation."""
         data = {
             "headers": {"Authorization": f"Bearer {self.access_token}"},
-            "proxies": self.manifest_data.get("proxies", settings.proxies),
+            "proxies": self.manifest_data.get("proxies"),
             "params": {"pool": f"{pool_id}", "quantity": f"{entitlement_quantity}"},
         }
         add_entitlements = simple_retry(
-            requests.post,
-            cmd_args=[
-                f"{self.allocations_url}/{self.allocation_uuid}/entitlements"
-            ],
+            self.requester.post,
+            cmd_args=[f"{self.allocations_url}/{self.allocation_uuid}/entitlements"],
             cmd_kwargs=data,
         )
         return add_entitlements
 
     def verify_allocation_entitlements(self, entitlement_quantity, subscription_name):
-        logger.info(
-            f"Verifying the entitlement quantity of {subscription_name} on the allocation."
-        )
+        """Checks that the entitlements in the allocation match those defined in settings."""
+        logger.info(f"Verifying the entitlement quantity of {subscription_name} on the allocation.")
         data = {
             "headers": {"Authorization": f"Bearer {self.access_token}"},
-            "proxies": self.manifest_data.get("proxies", settings.proxies),
+            "proxies": self.manifest_data.get("proxies"),
             "params": {"include": "entitlements"},
         }
         self.entitlement_data = simple_retry(
-            requests.get,
+            self.requester.get,
             cmd_args=[f"{self.allocations_url}/{self.allocation_uuid}"],
             cmd_kwargs=data,
         ).json()
         current_entitlement = [
             d
             for d in self.entitlement_data["body"]["entitlementsAttached"]["value"]
             if d["subscriptionName"] == subscription_name
         ]
         if not current_entitlement:
             return
         logger.debug(f"Current entitlement is {current_entitlement}")
         self.attached_quantity = current_entitlement[0]["entitlementQuantity"]
         if self.attached_quantity == entitlement_quantity:
-            logger.debug(
-                f"Operation successful. Attached {self.attached_quantity} entitlements."
-            )
+            logger.debug(f"Operation successful. Attached {self.attached_quantity} entitlements.")
             return True
         elif self.attached_quantity < entitlement_quantity:
             logger.debug(
                 f"{self.attached_quantity} of {entitlement_quantity} attached. Trying again."
             )
             return
         else:
             logger.warning(
                 f"Something went wrong. Attached quantity {self.attached_quantity} is greater than "
                 f"requested quantity {entitlement_quantity}."
             )
             return True
 
     def process_subscription_pools(self, subscription_pools, subscription_data):
+        """Loops through the list of subscription pools in the account.
+
+        Identifies pools that match the subscription names and quantities defined in settings, then
+        attempts to add the specified quantity of each subscription to the allocation.
+        """
+        SUCCESS_CODE = 200
         logger.debug(f"Finding a matching pool for {subscription_data['name']}.")
         matching = [
             d
             for d in subscription_pools["body"]
             if d["subscriptionName"] == subscription_data["name"]
         ]
-        logger.debug(
-            f"The following pools are matches for this subscription: {matching}"
-        )
+        logger.debug(f"The following pools are matches for this subscription: {matching}")
         for match in matching:
-            if (match["entitlementsAvailable"] > subscription_data["quantity"] or
-                match["entitlementsAvailable"] == -1):
+            if (
+                match["entitlementsAvailable"] > subscription_data["quantity"]
+                or match["entitlementsAvailable"] == -1
+            ):
                 logger.debug(
                     f"Pool {match['id']} is a match for this subscription and has "
                     f"{match['entitlementsAvailable']} entitlements available."
                 )
                 add_entitlements = self.add_entitlements_to_allocation(
                     pool_id=match["id"],
                     entitlement_quantity=subscription_data["quantity"],
                 )
-                # if the above is using simple_rety, it will raise an exception
+                # if the above is using simple_retry, it will raise an exception
                 # and never trigger the following block
                 if add_entitlements.status_code in [404, 429, 500, 504]:
                     verify_entitlements = self.verify_allocation_entitlements(
                         entitlement_quantity=subscription_data["quantity"],
                         subscription_name=subscription_data["name"],
                     )
                     if not verify_entitlements:
@@ -283,102 +313,124 @@
                                 subscription_data=subscription_data,
                             )
                     else:
                         logger.debug(
                             f"Successfully added {subscription_data['quantity']} entitlements of "
                             f"{subscription_data['name']} to the allocation."
                         )
+                        self._active_pools.append(match)
+                        update_inventory(self.subscription_allocations)
                         break
-                elif add_entitlements.status_code == 200:
+                elif add_entitlements.status_code == SUCCESS_CODE:
                     logger.debug(
                         f"Successfully added {subscription_data['quantity']} entitlements of "
                         f"{subscription_data['name']} to the allocation."
                     )
+                    self._active_pools.append(match)
+                    update_inventory(self.subscription_allocations)
                     break
                 else:
-                    raise Exception(
+                    raise RuntimeError(
                         "Something went wrong while adding entitlements. Received response status "
                         f"{add_entitlements.status_code}."
                     )
 
     def trigger_manifest_export(self):
+        """Triggers job to export manifest from subscription allocation.
+
+        Starts the export job, monitors the status of the job, and downloads the manifest on
+        successful completion of the job.
+        """
+        MAX_REQUESTS = 50
+        SUCCESS_CODE = 200
         data = {
             "headers": {"Authorization": f"Bearer {self.access_token}"},
-            "proxies": self.manifest_data.get("proxies", settings.proxies),
+            "proxies": self.manifest_data.get("proxies"),
         }
-        # Should this use the XDG Base Directory Specification?
-        local_file = Path(f"manifests/{self.allocation_name}_manifest.zip")
+        local_file = Path(f"manifests/{self.manifest_name}")
         local_file.parent.mkdir(parents=True, exist_ok=True)
         logger.info(
             f"Triggering manifest export job for subscription allocation {self.allocation_name}"
         )
         trigger_export_job = simple_retry(
-            requests.get,
-            cmd_args=[
-                f"{self.allocations_url}/{self.allocation_uuid}/export"
-            ],
+            self.requester.get,
+            cmd_args=[f"{self.allocations_url}/{self.allocation_uuid}/export"],
             cmd_kwargs=data,
         ).json()
         export_job_id = trigger_export_job["body"]["exportJobID"]
         export_job = simple_retry(
-            requests.get,
-            cmd_args=[
-                f"{self.allocations_url}/{self.allocation_uuid}/exportJob/{export_job_id}"
-            ],
+            self.requester.get,
+            cmd_args=[f"{self.allocations_url}/{self.allocation_uuid}/exportJob/{export_job_id}"],
             cmd_kwargs=data,
         )
         request_count = 1
         limit_exceeded = False
-        while export_job.status_code != 200:
+        while export_job.status_code != SUCCESS_CODE:
             export_job = simple_retry(
-                requests.get,
+                self.requester.get,
                 cmd_args=[
                     f"{self.allocations_url}/{self.allocation_uuid}/exportJob/{export_job_id}"
                 ],
                 cmd_kwargs=data,
             )
-            logger.debug(
-                f"Attempting to export manifest. Attempt number: {request_count}"
-            )
-            if request_count > 50:
+            logger.debug(f"Attempting to export manifest. Attempt number: {request_count}")
+            if request_count > MAX_REQUESTS:
                 limit_exceeded = True
                 logger.info(
                     "Manifest export job status check limit exceeded. This may indicate an "
                     "upstream issue with Red Hat Subscription Management."
                 )
-                break
+                raise Timeout("Export timeout exceeded")
             request_count += 1
         if limit_exceeded:
-            return
+            self.content = None
+            return self
         export_job = export_job.json()
-        export_href = export_job["body"]["href"]
+        if self.is_mock:
+            export_href = export_job.body["href"]
+        else:
+            export_href = export_job["body"]["href"]
         manifest = simple_retry(
-            requests.get,
+            self.requester.get,
             cmd_args=[f"{export_href}"],
             cmd_kwargs=data,
         )
         logger.info(
             f"Writing manifest for subscription allocation {self.allocation_name} to location "
             f"{local_file}"
         )
         local_file.write_bytes(manifest.content)
         manifest.path = local_file
+        manifest.name = self.manifest_name
+        if self.is_mock:
+            manifest.uuid = self.allocation_uuid.uuid
+        else:
+            manifest.uuid = self.allocation_uuid
+        update_inventory(self.subscription_allocations)
         return manifest
 
     def get_manifest(self):
+        """Provides a subscription manifest based on settings.
+
+        Calls the methods required to create a new subscription allocation, add the appropriate
+        subscriptions to the allocation, export a manifest, and download the manifest.
+        """
         self.create_subscription_allocation()
         for sub in self.subscription_data:
             self.process_subscription_pools(
                 subscription_pools=self.subscription_pools,
                 subscription_data=sub,
             )
         return self.trigger_manifest_export()
 
     def __enter__(self):
+        """Generates and returns a manifest."""
         try:
             return self.get_manifest()
         except:
             self.delete_subscription_allocation()
             raise
 
     def __exit__(self, *tb_args):
+        """Deletes subscription allocation on teardown unless using CLI."""
         self.delete_subscription_allocation()
+        update_inventory(self.subscription_allocations)
```

### Comparing `manifester-0.0.9/manifester.egg-info/SOURCES.txt` & `manifester-0.2.2/manifester.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
 README.md
+manifester_inventory.yaml
 manifester_settings.yaml.example
-setup.cfg
-setup.py
+pyproject.toml
+.github/dependabot.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/python-publish.yml
 .github/workflows/update_manifester_image.yml
 logs/.gitignore
 manifester/__init__.py
 manifester/commands.py
 manifester/helpers.py
 manifester/logger.py
 manifester/manifester.py
 manifester/settings.py
 manifester.egg-info/PKG-INFO
 manifester.egg-info/SOURCES.txt
 manifester.egg-info/dependency_links.txt
-manifester.egg-info/entry_points.txt
-manifester.egg-info/not-zip-safe
 manifester.egg-info/requires.txt
-manifester.egg-info/top_level.txt
+manifester.egg-info/top_level.txt
+tests/test_manifester.py
```

### Comparing `manifester-0.0.9/manifester_settings.yaml.example` & `manifester-0.2.2/manifester_settings.yaml.example`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #rhsm-manifester settings
 log_level: "info"
 offline_token: ""
 proxies: {"https": ""}
+username_prefix: "example_username"  # replace value with a unique username
+inventory_path: "manifester_inventory.yaml"
 manifest_category:
   golden_ticket:
     # An offline token can be generated at https://access.redhat.com/management/api
     offline_token: ""
     # Value of sat_version setting should be in the form 'sat-6.10'
     sat_version: "sat-6.10"
     # golden_ticket manifests should not use a quantity higher than 1 for any subscription
```

