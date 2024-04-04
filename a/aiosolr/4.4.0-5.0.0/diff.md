# Comparing `tmp/aiosolr-4.4.0.tar.gz` & `tmp/aiosolr-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosolr-4.4.0.tar", last modified: Fri Oct 13 18:33:36 2023, max compression
+gzip compressed data, was "aiosolr-5.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiosolr-4.4.0.tar` & `aiosolr-5.0.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2023-10-13 18:33:36.216342 aiosolr-4.4.0/
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     5027 2023-10-13 18:33:36.216544 aiosolr-4.4.0/PKG-INFO
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     3456 2022-02-08 22:46:58.000000 aiosolr-4.4.0/README.md
-drwxrwxrwx   0 brad.belyeu   (501) staff       (20)        0 2023-10-13 18:33:36.215944 aiosolr-4.4.0/aiosolr.egg-info/
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     5027 2023-10-13 18:33:36.000000 aiosolr-4.4.0/aiosolr.egg-info/PKG-INFO
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      208 2023-10-13 18:33:36.000000 aiosolr-4.4.0/aiosolr.egg-info/SOURCES.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)        1 2023-10-13 18:33:36.000000 aiosolr-4.4.0/aiosolr.egg-info/dependency_links.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)       15 2023-10-13 18:33:36.000000 aiosolr-4.4.0/aiosolr.egg-info/requires.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)        8 2023-10-13 18:33:36.000000 aiosolr-4.4.0/aiosolr.egg-info/top_level.txt
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)    21665 2023-10-13 18:32:18.000000 aiosolr-4.4.0/aiosolr.py
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      537 2021-06-10 19:49:07.000000 aiosolr-4.4.0/pyproject.toml
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)      282 2023-10-13 18:33:36.217273 aiosolr-4.4.0/setup.cfg
--rw-rw-rw-   0 brad.belyeu   (501) staff       (20)     1138 2023-10-13 18:32:47.000000 aiosolr-4.4.0/setup.py
+-rw-r--r--   0        0        0      865 2020-07-02 02:10:06.000000 aiosolr-5.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1217 2019-08-23 19:48:55.000000 aiosolr-5.0.0/.gitignore
+-rw-r--r--   0        0        0    12471 2024-03-05 16:14:27.227899 aiosolr-5.0.0/.pylintrc
+-rw-r--r--   0        0        0      447 2021-06-10 19:49:05.087000 aiosolr-5.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1073 2021-06-10 19:49:05.087359 aiosolr-5.0.0/LICENSE.md
+-rw-r--r--   0        0        0     1529 2024-04-04 15:56:49.098443 aiosolr-5.0.0/Makefile
+-rw-r--r--   0        0        0     3923 2024-04-04 15:47:10.871940 aiosolr-5.0.0/README.md
+-rw-r--r--   0        0        0    22806 2024-04-04 15:54:26.819827 aiosolr-5.0.0/aiosolr.py
+-rwxr-xr-x   0        0        0       48 2021-06-10 19:49:07.028510 aiosolr-5.0.0/githooks/pre-commit
+-rw-r--r--   0        0        0      787 2024-04-04 16:05:32.241358 aiosolr-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0       92 2024-04-04 15:57:58.073707 aiosolr-5.0.0/requirements.in
+-rw-r--r--   0        0        0     3271 2024-04-04 15:59:01.350044 aiosolr-5.0.0/requirements.txt
+-rw-r--r--   0        0        0      227 2021-06-10 19:49:05.089652 aiosolr-5.0.0/setup.cfg
+-rw-r--r--   0        0        0     1222 2024-04-04 16:04:55.947358 aiosolr-5.0.0/setup.py
+-rw-r--r--   0        0        0      517 2024-03-05 16:14:27.230893 aiosolr-5.0.0/tests/test_clean.py
+-rw-r--r--   0        0        0      222 1970-01-01 00:00:00.000000 aiosolr-5.0.0/PKG-INFO
```

### Comparing `aiosolr-4.4.0/aiosolr.py` & `aiosolr-5.0.0/aiosolr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
-AsyncIO Python client for Apache Solr
+Lightweight AsyncIO Python client for Apache Solr
 
 The idea behind this module is to provide easy access to Solr in an efficient manner.
 This is achieved through using AIOHTTP client sessions with shared connection pooling.
 Ease of use is provided by mapping Solr Handlers to methods making it RPC like.
 """
 
 import asyncio
 import json
 import logging
 import re
 import urllib.parse
+from typing import TYPE_CHECKING
 
 import aiohttp
 import bleach
 
+__version__ = "5.0.0"
+
 LOGGER = logging.getLogger("aiosolr")
 
 
 class SolrError(Exception):
     """Base class for exceptions in this module."""
 
     def __init__(self, message, *args, trace=None, **kwargs):
@@ -72,28 +75,30 @@
 
     def get(self, name, default=None):
         """Get an attribute or return default value."""
         return getattr(self, name, default)
 
 
 # TODO Support something other than JSON
-class Client:
+class Client:  # pylint: disable=too-many-instance-attributes
     """Class representing a client connection to Solr."""
 
-    def __init__(  # pylint: disable=dangerous-default-value
+    def __init__(
         self,
         *,
         collection="",
-        connection_url=None,
+        connection_url: str | None = None,
         debug=False,
         host="127.0.0.1",
         port="80",
         scheme="http",
-        timeout=(1, 3),
-        trace_configs=[],
+        read_timeout: int | None = None,
+        write_timeout: int | None = None,
+        client_timeout: aiohttp.ClientTimeout = aiohttp.ClientTimeout(sock_connect=1, sock_read=3),
+        trace_configs: list[aiohttp.TraceConfig] | None = None,
         ttl_dns_cache=3600,
     ):
         """Init to instantiate Solr class.
 
         If the core/collection is not provided it should be passed to the methods as required.
         timeout, ttl_dns_cache, and trace_configs arguments are stored to be used when setting up
         the AIOHTTP ClientSession class.
@@ -105,27 +110,27 @@
         else:
             url = urllib.parse.urlparse(connection_url)
             base_path, collection = url.path.rsplit("/", 1)
             self.base_url = f"{url.scheme}://{url.netloc}{base_path}"
             self.collection = collection or None
 
         self.response_writer = "json"
-        if isinstance(timeout, tuple):
-            # In some cases you may want to set the
-            # connection timeout to 4 b/c of the TCP packet retransmission window
-            # http://docs.python-requests.org/en/master/user/advanced/#timeouts
-            # But in many cases that will be too slow
-            self.timeout = aiohttp.ClientTimeout(sock_connect=timeout[0], sock_read=timeout[1])
-        else:
-            self.timeout = aiohttp.ClientTimeout(total=timeout)
+        # In some cases you may want to set the
+        # connection timeout to 4 b/c of the TCP packet retransmission window
+        # http://docs.python-requests.org/en/master/user/advanced/#timeouts
+        # But in many cases that will be too slow
+        self.client_timeout = client_timeout
 
         self.session = None
         self.trace_configs = trace_configs
         self.ttl_dns_cache = ttl_dns_cache
 
+        self.read_timeout = read_timeout
+        self.write_timeout = write_timeout
+
         if debug:
             LOGGER.setLevel(logging.DEBUG)
             logging.getLogger("aiohttp.client").setLevel(logging.DEBUG)
 
     def _deserialize(self, resp):
         """Deserialize Solr response to Python object."""
         # TODO Handle types other than json
@@ -140,21 +145,23 @@
     async def _get(self, url, *, body={}, headers={}):
         """Network request to get data from a server."""
         if "Accept" not in headers and self.response_writer == "json":
             headers["Accept"] = "application/json"
 
         if not self.session:
             await self.setup()
+            if TYPE_CHECKING:
+                assert self.session
 
         LOGGER.debug(url)
         LOGGER.debug(headers)
         if body:
             LOGGER.debug(body)
             headers["Content-Type"] = "application/json"
-            async with self.session.request("POST", url, headers=headers, json=body) as response:
+            async with self.session.post(url, headers=headers, json=body) as response:
                 response.body = await response.text()
         else:
             async with self.session.get(url, headers=headers) as response:
                 response.body = await response.text()
 
         return response
 
@@ -229,14 +236,15 @@
                         "pf2",
                         "pf3",
                         "qf",
                     )
                     else ","
                 )
                 clean_vals = [urllib.parse.quote_plus(str(i), encoding="utf8") for i in value]
+                # pylint: disable=consider-using-f-string
                 query_string += "&{}={}".format(param, separator.join(clean_vals))
             elif isinstance(value, bool):
                 # using title cased bools results in the following error in Solr logs
                 # org.apache.solr.common.SolrException: invalid boolean value: False
                 query_string += f"&{param}=true" if value else f"&{param}=false"
             else:
                 clean_val = urllib.parse.quote_plus(str(value), encoding="utf8")
@@ -244,14 +252,16 @@
 
         return query_string
 
     async def _post(self, url, data, headers=None):
         """Network request to post data to a server."""
         if not self.session:
             await self.setup()
+            if TYPE_CHECKING:
+                assert self.session
 
         if isinstance(data, (dict, list)):
             if headers:
                 headers["Content-Type"] = "application/json"
             else:
                 headers = {"Content-Type": "application/json"}
 
@@ -341,35 +351,38 @@
 
     @staticmethod
     def clean(
         query,  # end user query
         allow_html_tags=False,
         allow_http=False,
         allow_wildcard=False,
-        escape_chars=(":", r"\:"),  # tuple of (replace_me, replace_with)
+        find_and_replace: tuple[tuple[str, str]] = (
+            (":", r"\:"),
+            ("|", " "),
+        ),  # tuple of tuples (find_me, replace_with)
         max_len=0,
         # regex of chars to remove
-        remove_chars=r'[\&\|\!\(\)\{\}\[\]\^"~\?\\;]',
+        remove_chars=r'[\"\&\!\(\)\{\}\[\]\^"~\?\\;#,]',
         urlencode=False,
     ):
         """Typical query cleaning."""
         if not allow_http:
             query = re.sub(r"http\S+", "", query)
 
         # Remove these chars
         query = re.sub(remove_chars, "", query)
 
         if not allow_wildcard:
             query = query.replace("*", "")
             # Also remove urlencoded wildcard (*)
             query = query.replace("%2a", "")
 
-        if escape_chars:
-            # Escape these chars
-            query = re.sub(escape_chars[0], escape_chars[1], query)
+        if find_and_replace:
+            for find, replace in find_and_replace:
+                query = query.replace(find, replace)
 
         if not allow_html_tags:
             # bleach it to prevent JS injection or other unwanted html
             # when displaying the query back to the user in a web page
             query = bleach.clean(query, strip=True)
 
         if max_len:
@@ -402,23 +415,26 @@
         LOGGER.debug("Calling dataimport handler /%s...", handler)
         collection = self._get_collection(kwargs)
         url = f"{self.base_url}/{collection}/{handler}?wt={self.response_writer}"
         url += self._kwargs_to_query_string(kwargs)
         solr_response = await self._get(url)
         return self._deserialize(solr_response)
 
-    async def get(self, _id, handler="get", **kwargs):
+    async def get(self, _id, handler="get", read_timeout: int | None = None, **kwargs):
         """Use Solr's built-in get handler to retrieve a single document by id."""
         collection = self._get_collection(kwargs)
         LOGGER.debug(
             "Getting document from Solr collection %s via handler %s...", collection, handler
         )
         url = f"{self.base_url}/{collection}/{handler}?id={_id}&wt={self.response_writer}"
         url += self._kwargs_to_query_string(kwargs)
-        return await self._get_check_ok_deserialize(url)
+        return await asyncio.wait_for(
+            self._get_check_ok_deserialize(url),
+            read_timeout if read_timeout is not None else self.read_timeout,
+        )
 
     async def ping(self, handler="ping", action="status", **kwargs):
         """Use Solr's ping handler to check status of, enable, or disable a node."""
         assert action.lower() in ("status", "enable", "disable")
         LOGGER.debug("Pinging Solr...")
         collection = self._get_collection(kwargs)
         url = (
@@ -429,15 +445,15 @@
 
     async def setup(self):
         """Setup the ClientSession for use."""
         LOGGER.debug("Creating Solr session connection...")
         tcp_conn = aiohttp.TCPConnector(ttl_dns_cache=self.ttl_dns_cache)
         self.session = aiohttp.ClientSession(
             connector=tcp_conn,
-            timeout=self.timeout,
+            timeout=self.client_timeout,
             trace_configs=self.trace_configs,
         )
 
     async def suggestions(self, handler, query=None, build=False, **kwargs):
         """
         Query a RequestHandler of class SearchHandler using the SuggestComponent.
 
@@ -469,15 +485,15 @@
                         for s in response.data["suggest"][name][query]["suggestions"]
                     ]
                 except KeyError:
                     pass
 
         return response, suggestions
 
-    async def query(self, *, handler="select", **kwargs):
+    async def query(self, *, handler="select", read_timeout: int | None = None, **kwargs):
         """Query a requestHandler of class SearchHandler."""
         LOGGER.debug("Querying Solr %s handler...", handler)
         collection = self._get_collection(kwargs)
 
         if handler in ("select", "mlt", "query") and "q" not in kwargs:
             if "query" not in kwargs:
                 kwargs["q"] = "*"
@@ -497,18 +513,24 @@
 
             if "prefer_local" in kwargs:
                 kwargs.pop("prefer_local")
                 url += "&shards.preference=replica.location:local"
 
             if handler == "select":
                 body = self._kwargs_to_json_body(kwargs)
-                solr_response = await self._get(url, body=body)
+                solr_response = await asyncio.wait_for(
+                    self._get(url, body=body),
+                    read_timeout if read_timeout is not None else self.read_timeout,
+                )
             else:  # mlt handler and some others don't support params in body
                 url += self._kwargs_to_query_string(kwargs)
-                solr_response = await self._get(url)
+                solr_response = await asyncio.wait_for(
+                    self._get(url),
+                    read_timeout if read_timeout is not None else self.read_timeout,
+                )
 
             if solr_response.status != 200:
                 msg, trace = None, None
                 try:
                     error = self._deserialize(solr_response)
                     msg = error.data.get("error", {}).get("msg", error)
                     trace = error.data.get("error", {}).get("trace")
@@ -518,24 +540,34 @@
 
                 raise SolrError(msg, trace)
         else:
             raise SolrError("Non json responses not yet supported.")
 
         return self._deserialize(solr_response)
 
-    async def update(self, data, handler="update", overwrite=True, **kwargs):
+    async def update(
+        self,
+        data,
+        handler="update",
+        overwrite=True,
+        write_timeout: int | None = None,
+        **kwargs,
+    ):
         """Update a document using Solr's update handler."""
         collection = self._get_collection(kwargs)
         LOGGER.debug("Updating %s data in Solr via %s handler...", collection, handler)
         url = f"{self.base_url}/{collection}/{handler}?wt={self.response_writer}"
         if overwrite:
             url += "&overwrite=true"
         url += self._kwargs_to_query_string(kwargs)
 
-        response = await self._post(url, data)
+        response = await asyncio.wait_for(
+            self._post(url, data),
+            write_timeout if write_timeout is not None else self.write_timeout,
+        )
         if response.status == 200:
             data = self._deserialize(response)
         else:
             msg, trace = None, None
             try:
                 error = self._deserialize(response)
                 msg = error.data.get("error", {}).get("msg", error)
```

### Comparing `aiosolr-4.4.0/setup.py` & `aiosolr-5.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 #!/usr/bin/env python
-"""Lightweight Python client for Apache Solr."""
+
+"""Lightweight AsyncIO Python client for Apache Solr."""
+
+# pylint: disable=consider-using-with
+
 import sys
 
 from setuptools import setup
 
+import aiosolr
+
 if sys.version_info < (3, 7):
     sys.exit("Sorry, Python < 3.7 is not supported")
 
-__version__ = "4.4.0"
-
 setup(
     name="aiosolr",
-    version=__version__,
+    version=aiosolr.__version__,
     description=__doc__,
     author="Brad Belyeu",
-    author_email="bradley.belyeu@life.church",
+    author_email="bradley.belyeu@youversion.com",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
         "Programming Language :: Python :: 3",
     ],
-    download_url=f"https://github.com/bbelyeu/aiosolr/archive/{__version__}.zip",
+    download_url=f"https://github.com/bbelyeu/aiosolr/archive/{aiosolr.__version__}.zip",
     install_requires=["aiohttp", "bleach"],
     keywords=["solr", "asyncio", "aiohttp", "search"],
     license="MIT",
-    long_description=open("README.md", "r").read(),
+    long_description=open("README.md", encoding="utf8", mode="r").read(),
     long_description_content_type="text/markdown",
     platforms="any",
     py_modules=["aiosolr"],
-    python_requires=">3.7.0",
+    python_requires=">=3.7.0",
     test_suite="tests",
     url="https://github.com/bbelyeu/aiosolr/",
 )
```

