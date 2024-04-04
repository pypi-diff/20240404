# Comparing `tmp/gidgetlab-2.0.0.tar.gz` & `tmp/gidgetlab-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gidgetlab-2.0.0.tar", last modified: Wed Feb 21 16:53:42 2024, max compression
+gzip compressed data, was "gidgetlab-2.0.1.tar", last modified: Thu Apr  4 14:57:00 2024, max compression
```

## Comparing `gidgetlab-2.0.0.tar` & `gidgetlab-2.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 16:53:42.036473 gidgetlab-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1170 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      873 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      506 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     1865 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)    11378 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    18008 2024-02-21 16:53:42.036473 gidgetlab-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2925 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 16:53:42.030473 gidgetlab-2.0.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      606 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     2575 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/abc.rst
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/aiohttp.rst
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     4024 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/httpx.rst
--rw-rw-rw-   0 root         (0) root         (0)     3727 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/routing.rst
--rw-rw-rw-   0 root         (0) root         (0)     2660 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/sansio.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/tornado.rst
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/docs/treq.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 16:53:42.032473 gidgetlab-2.0.0/gidgetlab/
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-02-21 16:53:41.000000 gidgetlab-2.0.0/gidgetlab/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    10831 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/abc.py
--rw-rw-rw-   0 root         (0) root         (0)     6819 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/aiohttp.py
--rw-rw-rw-   0 root         (0) root         (0)     3347 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/httpx.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     4884 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/routing.py
--rw-rw-rw-   0 root         (0) root         (0)    12222 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/sansio.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/tornado.py
--rw-rw-rw-   0 root         (0) root         (0)     2181 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/gidgetlab/treq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 16:53:42.034473 gidgetlab-2.0.0/gidgetlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18008 2024-02-21 16:53:42.000000 gidgetlab-2.0.0/gidgetlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      735 2024-02-21 16:53:42.000000 gidgetlab-2.0.0/gidgetlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 16:53:42.000000 gidgetlab-2.0.0/gidgetlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      449 2024-02-21 16:53:42.000000 gidgetlab-2.0.0/gidgetlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-21 16:53:42.000000 gidgetlab-2.0.0/gidgetlab.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1528 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-02-21 16:53:33.000000 gidgetlab-2.0.0/pytest.ini
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-21 16:53:42.036473 gidgetlab-2.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:57:00.599692 gidgetlab-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     1170 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      873 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11378 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    18013 2024-04-04 14:57:00.598692 gidgetlab-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:57:00.592692 gidgetlab-2.0.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/abc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/aiohttp.rst
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4024 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/httpx.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/routing.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2660 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/sansio.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/tornado.rst
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/docs/treq.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:57:00.594692 gidgetlab-2.0.1/gidgetlab/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-04 14:57:00.000000 gidgetlab-2.0.1/gidgetlab/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    10994 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6819 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/aiohttp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3347 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/httpx.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     4884 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/routing.py
+-rw-rw-rw-   0 root         (0) root         (0)    12222 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/sansio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/tornado.py
+-rw-rw-rw-   0 root         (0) root         (0)     2181 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/gidgetlab/treq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:57:00.595692 gidgetlab-2.0.1/gidgetlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18013 2024-04-04 14:57:00.000000 gidgetlab-2.0.1/gidgetlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      735 2024-04-04 14:57:00.000000 gidgetlab-2.0.1/gidgetlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 14:57:00.000000 gidgetlab-2.0.1/gidgetlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      449 2024-04-04 14:57:00.000000 gidgetlab-2.0.1/gidgetlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 14:57:00.000000 gidgetlab-2.0.1/gidgetlab.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1528 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-04 14:56:55.000000 gidgetlab-2.0.1/pytest.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 14:57:00.599692 gidgetlab-2.0.1/setup.cfg
```

### Comparing `gidgetlab-2.0.0/.gitignore` & `gidgetlab-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/.gitlab-ci.yml` & `gidgetlab-2.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/CHANGELOG.rst` & `gidgetlab-2.0.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2.0.1 (2024-04-04)
+------------------
+
+* Fix params typing (should accept value of both str and bool)
+* Update gitlab api clients link in README (thanks to Elan Ruusamäe)
+
 2.0.0 (2024-02-21)
 ------------------
 
 * Use OAuth-compliant headers for access token
   (allow to use Oauth 2.0 tokens as well as personal/group/project token)
 * Move from setup.py to pyproject.toml
 * Add Python 3.12 tests
```

### Comparing `gidgetlab-2.0.0/LICENSE` & `gidgetlab-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/PKG-INFO` & `gidgetlab-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gidgetlab
-Version: 2.0.0
+Version: 2.0.1
 Summary: An async GitLab API library
 Author-email: Benjamin Bertrand <beenje@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -333,12 +333,12 @@
 `Build-a-GitHub-Bot Workshop <http://github-bot-tutorial.readthedocs.io/en/latest/index.html>`_.
 
 
 Alternative libraries
 ---------------------
 
 If you think you want a different approach to the GitLab API,
-`GitLab maintains a list of libraries <https://about.gitlab.com/applications/#api-clients/>`_.
+`GitLab maintains a list of libraries <https://docs.gitlab.com/ee/api/rest/#third-party-clients>`_.
 
 .. _gidgethub: https://github.com/brettcannon/gidgethub
 .. _`GitLab API`: https://docs.gitlab.com/ce/api/
 .. _`sans-I/O`: https://sans-io.readthedocs.io/
```

### Comparing `gidgetlab-2.0.0/README.rst` & `gidgetlab-2.0.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -78,12 +78,12 @@
 `Build-a-GitHub-Bot Workshop <http://github-bot-tutorial.readthedocs.io/en/latest/index.html>`_.
 
 
 Alternative libraries
 ---------------------
 
 If you think you want a different approach to the GitLab API,
-`GitLab maintains a list of libraries <https://about.gitlab.com/applications/#api-clients/>`_.
+`GitLab maintains a list of libraries <https://docs.gitlab.com/ee/api/rest/#third-party-clients>`_.
 
 .. _gidgethub: https://github.com/brettcannon/gidgethub
 .. _`GitLab API`: https://docs.gitlab.com/ce/api/
 .. _`sans-I/O`: https://sans-io.readthedocs.io/
```

### Comparing `gidgetlab-2.0.0/docs/Makefile` & `gidgetlab-2.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/docs/abc.rst` & `gidgetlab-2.0.1/docs/abc.rst`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/docs/conf.py` & `gidgetlab-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/docs/index.rst` & `gidgetlab-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/docs/routing.rst` & `gidgetlab-2.0.1/docs/routing.rst`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/docs/sansio.rst` & `gidgetlab-2.0.1/docs/sansio.rst`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/gidgetlab/abc.py` & `gidgetlab-2.0.1/gidgetlab/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """Provide an abstract base class for easier requests."""
 
 import os
 import abc
 import http
 import json
 import urllib.parse
-from typing import Any, AsyncGenerator, Dict, Mapping, MutableMapping, Tuple, cast
+from typing import (
+    Any,
+    AsyncGenerator,
+    Dict,
+    Mapping,
+    MutableMapping,
+    Tuple,
+    cast,
+    Union,
+)
 from typing import Optional as Opt
 
 from . import sansio
 from .exceptions import (
     GitLabBroken,
     GraphQLException,
     GraphQLResponseTypeError,
@@ -102,15 +111,15 @@
             url_parts_with_params = url_parts._replace(
                 query=urllib.parse.urlencode(query, doseq=True)
             )
             return urllib.parse.urlunparse(url_parts_with_params)
         return url
 
     async def _make_request(
-        self, method: str, url: str, params: Dict[str, str], data: Any
+        self, method: str, url: str, params: Dict[str, Union[str, bool]], data: Any
     ) -> Tuple[bytes, Opt[str]]:
         """Construct and make an HTTP request."""
         filled_url = self.format_url(url, params)
         request_headers = sansio.create_headers(
             self.requester, access_token=self.access_token
         )
         cached = cacheable = False
@@ -143,26 +152,26 @@
             has_cache_details = "etag" in response[1] or "last-modified" in response[1]
             if self._cache is not None and cacheable and has_cache_details:
                 etag = response[1].get("etag")
                 last_modified = response[1].get("last-modified")
                 self._cache[filled_url] = etag, last_modified, data, more
         return data, more
 
-    async def getitem(self, url: str, params: Dict[str, str] = {}) -> Any:
+    async def getitem(self, url: str, params: Dict[str, Union[str, bool]] = {}) -> Any:
         """Get a single item from GitLab.
 
         .. note::
             For ``GET`` calls that can return multiple values and
             potentially require pagination, see ``getiter()``.
         """
         data, _ = await self._make_request("GET", url, params, b"")
         return data
 
     async def getiter(
-        self, url: str, params: Dict[str, str] = {}
+        self, url: str, params: Dict[str, Union[str, bool]] = {}
     ) -> AsyncGenerator[Any, None]:
         """Get all items from a GitLab API endpoint.
 
         An asynchronous iterable is returned which will yield all items
         from the endpoint (i.e. use ``async for`` on the result). Any
         `pagination <https://docs.gitlab.com/ee/api/README.html#pagination>`_
         will automatically be followed.
@@ -175,33 +184,37 @@
         for item in data:
             yield item
         if more:
             # `yield from` is not supported in coroutines.
             async for item in self.getiter(more, params):
                 yield item
 
-    async def post(self, url: str, params: Dict[str, str] = {}, *, data: Any) -> Any:
+    async def post(
+        self, url: str, params: Dict[str, Union[str, bool]] = {}, *, data: Any
+    ) -> Any:
         """Send a ``POST`` request to GitLab."""
         data, _ = await self._make_request("POST", url, params, data)
         return data
 
-    async def patch(self, url: str, params: Dict[str, str] = {}, *, data: Any) -> Any:
+    async def patch(
+        self, url: str, params: Dict[str, Union[str, bool]] = {}, *, data: Any
+    ) -> Any:
         """Send a ``PATCH`` request to GitLab."""
         data, _ = await self._make_request("PATCH", url, params, data)
         return data
 
     async def put(
-        self, url: str, params: Dict[str, str] = {}, *, data: Any = b""
+        self, url: str, params: Dict[str, Union[str, bool]] = {}, *, data: Any = b""
     ) -> Any:
         """Send a ``PUT`` request to GitLab."""
         data, _ = await self._make_request("PUT", url, params, data)
         return data
 
     async def delete(
-        self, url: str, params: Dict[str, str] = {}, *, data: Any = b""
+        self, url: str, params: Dict[str, Union[str, bool]] = {}, *, data: Any = b""
     ) -> None:
         """Send a ``DELETE`` request to GitLab."""
         await self._make_request("DELETE", url, params, data)
 
     async def graphql(
         self,
         query: str,
```

### Comparing `gidgetlab-2.0.0/gidgetlab/aiohttp.py` & `gidgetlab-2.0.1/gidgetlab/aiohttp.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/gidgetlab/exceptions.py` & `gidgetlab-2.0.1/gidgetlab/exceptions.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/gidgetlab/httpx.py` & `gidgetlab-2.0.1/gidgetlab/httpx.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/gidgetlab/routing.py` & `gidgetlab-2.0.1/gidgetlab/routing.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/gidgetlab/sansio.py` & `gidgetlab-2.0.1/gidgetlab/sansio.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/gidgetlab/tornado.py` & `gidgetlab-2.0.1/gidgetlab/tornado.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/gidgetlab/treq.py` & `gidgetlab-2.0.1/gidgetlab/treq.py`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/gidgetlab.egg-info/PKG-INFO` & `gidgetlab-2.0.1/gidgetlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gidgetlab
-Version: 2.0.0
+Version: 2.0.1
 Summary: An async GitLab API library
 Author-email: Benjamin Bertrand <beenje@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -333,12 +333,12 @@
 `Build-a-GitHub-Bot Workshop <http://github-bot-tutorial.readthedocs.io/en/latest/index.html>`_.
 
 
 Alternative libraries
 ---------------------
 
 If you think you want a different approach to the GitLab API,
-`GitLab maintains a list of libraries <https://about.gitlab.com/applications/#api-clients/>`_.
+`GitLab maintains a list of libraries <https://docs.gitlab.com/ee/api/rest/#third-party-clients>`_.
 
 .. _gidgethub: https://github.com/brettcannon/gidgethub
 .. _`GitLab API`: https://docs.gitlab.com/ce/api/
 .. _`sans-I/O`: https://sans-io.readthedocs.io/
```

### Comparing `gidgetlab-2.0.0/gidgetlab.egg-info/SOURCES.txt` & `gidgetlab-2.0.1/gidgetlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gidgetlab-2.0.0/pyproject.toml` & `gidgetlab-2.0.1/pyproject.toml`

 * *Files identical despite different names*

