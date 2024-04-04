# Comparing `tmp/curlquest-0.1.0.tar.gz` & `tmp/curlquest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curlquest-0.1.0.tar", max compression
+gzip compressed data, was "curlquest-0.1.1.tar", max compression
```

## Comparing `curlquest-0.1.0.tar` & `curlquest-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2024-04-04 02:38:00.275545 curlquest-0.1.0/LICENSE
--rw-r--r--   0        0        0     4574 2024-04-04 02:38:00.275545 curlquest-0.1.0/README.md
--rw-r--r--   0        0        0      204 2024-04-04 02:38:00.278878 curlquest-0.1.0/curlquest/__init__.py
--rw-r--r--   0        0        0     2633 2024-04-04 02:38:00.278878 curlquest-0.1.0/curlquest/defaults.py
--rw-r--r--   0        0        0     1167 2024-04-04 02:38:00.278878 curlquest-0.1.0/curlquest/dict.py
--rw-r--r--   0        0        0     1765 2024-04-04 02:38:00.278878 curlquest-0.1.0/curlquest/helper.py
--rw-r--r--   0        0        0     6065 2024-04-04 02:44:00.134121 curlquest-0.1.0/curlquest/models.py
--rw-r--r--   0        0        0     9034 2024-04-04 02:42:56.525790 curlquest-0.1.0/curlquest/sessions.py
--rw-r--r--   0        0        0      864 2024-04-04 02:56:08.380505 curlquest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 curlquest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-04 02:38:00.275545 curlquest-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4493 2024-04-04 03:00:19.309015 curlquest-0.1.1/README.md
+-rw-r--r--   0        0        0      204 2024-04-04 02:38:00.278878 curlquest-0.1.1/curlquest/__init__.py
+-rw-r--r--   0        0        0     2633 2024-04-04 02:38:00.278878 curlquest-0.1.1/curlquest/defaults.py
+-rw-r--r--   0        0        0     1167 2024-04-04 02:38:00.278878 curlquest-0.1.1/curlquest/dict.py
+-rw-r--r--   0        0        0     1765 2024-04-04 02:38:00.278878 curlquest-0.1.1/curlquest/helper.py
+-rw-r--r--   0        0        0     6059 2024-04-04 03:00:43.623249 curlquest-0.1.1/curlquest/models.py
+-rw-r--r--   0        0        0     9016 2024-04-04 03:00:27.594850 curlquest-0.1.1/curlquest/sessions.py
+-rw-r--r--   0        0        0      828 2024-04-04 03:02:19.833800 curlquest-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5602 1970-01-01 00:00:00.000000 curlquest-0.1.1/PKG-INFO
```

### Comparing `curlquest-0.1.0/LICENSE` & `curlquest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curlquest-0.1.0/README.md` & `curlquest-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # Request Curl
 
 A user-friendly wrapper for pycurl that simplifies HTTP requests.
 
 ## Installation
 Use the package manager 
 [pip](https://pip.pypa.io/en/stable/) 
-to install [request_curl](https://pypi.org/project/request-curl/).
+to install [curlquest](https://pypi.org/project/request-curl/).
 
 > NOTE: You need Python and libcurl installed on your system to use or build pycurl. Some RPM distributions of curl/libcurl do not include everything necessary to build pycurl, in which case you need to install the developer specific RPM which is usually called curl-dev.
 
 
 ```
-pip install request_curl
+pip install curlquest
 ```
 
 # Quickstart
-A request_curl session manages cookies, connection pooling, and configurations.
+A curlquest session manages cookies, connection pooling, and configurations.
 
 Basic Usage:
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 s.get('https://httpbin.org/get') # returns <Response [200]>
 s.request('GET', 'https://httpbin.org/get') # returns <Response [200]>
 ```
 
 Using a Context Manager
 ```python
-import request_curl
-with request_curl.Session() as session:
+import curlquest
+with curlquest.Session() as session:
     session.get('https://httpbin.org/get') # returns <Response [200]>
 ```
 
 # Features
 
 ## Response Object
 
 The response object is similar to that of the [requests](https://pypi.org/project/requests/) library.
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 r = s.get("https://httpbin.org/get")
 
 print(r) # prints response object
 print(r.status_code) # prints status code
 print(r.content) # prints response content in bytes
 print(r.text) # prints response content as text
 print(r.json) # prints response content as JSON
@@ -52,104 +52,104 @@
 print(r.headers) # prints response headers
 ```
 
 ## Proxy Support
 Format the proxy as a string.
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 # supports authentication: r = s.get("https://httpbin.org/get", proxies="ip:port:user:password")
 r = s.get("https://httpbin.org/get", proxies="ip:port")
 ```
 
 ## HTTP2
 HTTP2 is disabled by default.
 
 ```python
-import request_curl
-s = request_curl.Session(http2=True)
+import curlquest
+s = curlquest.Session(http2=True)
 r = s.get("https://httpbin.org/get")
 ```
 
 ## Cipher Suites
 You can specify custom cipher suites as an array.
 
 ```python
-import request_curl
+import curlquest
 
 cipher_suite = [
     "AES128-SHA256",
     "AES256-SHA256",
     "AES128-GCM-SHA256",
     "AES256-GCM-SHA384"
 ]
-s = request_curl.Session(cipher_suite=cipher_suite)
+s = curlquest.Session(cipher_suite=cipher_suite)
 r = s.get("https://httpbin.org/get")
 ```
 
 ## Debug Request
 Set debug to True to print raw input and output headers.
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 r = s.get("https://httpbin.org/get", debug=True)
 ```
 
 ## Custom Headers
 Specify custom headers as a dictionary.
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 headers = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.163 Safari/537.36"
 }
 r = s.get("https://httpbin.org/get", headers=headers)
 ```
 
 ## Data
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 
 # sending form data
 form_data = {"key": "value"}
 response = s.post("https://httpbin.org/post", data=form_data)
 
 # sending json data
 json_data = {"key": "value"}
 response = s.post("https://httpbin.org/post", json=json_data)
 ```
 
 # Usage with Curl-Impersonate
-To use request_curl with [curl-impersonate](https://github.com/lwthiker/curl-impersonate), 
+To use curlquest with [curl-impersonate](https://github.com/lwthiker/curl-impersonate), 
 opt for our [custom Docker image](https://hub.docker.com/r/h3adex/request-curl-impersonate) by either pulling or building it. 
-The image comes with request_curl and curl-impersonate pre-installed. 
-Check below for a demonstration on impersonating firefox98 tls-fingerprint and request_curl with our custom Docker Image.
+The image comes with curlquest and curl-impersonate pre-installed. 
+Check below for a demonstration on impersonating firefox98 tls-fingerprint and curlquest with our custom Docker Image.
 
 **Note**: This feature is still considered experimental. Only tested with firefox fingerprint
 
 To pull the Docker image:
 
 ```bash
 docker pull h3adex/request-curl-impersonate:latest
 docker run --rm -it h3adex/request-curl-impersonate
 ```
 
 Example Python code for a target website:
 
 ```python
-import request_curl
-from request_curl import FIREFOX98_CIPHER_SUITE, FIREFOX98_HEADERS
+import curlquest
+from curlquest import FIREFOX98_CIPHER_SUITE, FIREFOX98_HEADERS
 
 # impersonates ff98
-session = request_curl.Session(
+session = curlquest.Session(
     http2=True, 
     cipher_suite=FIREFOX98_CIPHER_SUITE, 
     headers=FIREFOX98_HEADERS
 )
 response = session.get("https://tls.browserleaks.com/json")
 # <Response [200]>
 # "ja3_hash":"25e9b0dd5b8e9330b206eae87e885e19"
```

### Comparing `curlquest-0.1.0/curlquest/defaults.py` & `curlquest-0.1.1/curlquest/defaults.py`

 * *Files identical despite different names*

### Comparing `curlquest-0.1.0/curlquest/dict.py` & `curlquest-0.1.1/curlquest/dict.py`

 * *Files identical despite different names*

### Comparing `curlquest-0.1.0/curlquest/helper.py` & `curlquest-0.1.1/curlquest/helper.py`

 * *Files identical despite different names*

### Comparing `curlquest-0.1.0/curlquest/models.py` & `curlquest-0.1.1/curlquest/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from typing import List, Optional, Dict, Any
 import zlib
 from http.cookiejar import CookieJar
 
 import brotli
 import pycurl
 
-from request_curl.dict import CaseInsensitiveDict
-from request_curl.helper import to_cookiejar
+from curlquest.dict import CaseInsensitiveDict
+from curlquest.helper import to_cookiejar
 
 CURL_INFO_MAPPING: Dict[str, Any] = {
     "TOTAL_TIME": pycurl.TOTAL_TIME,
     "NAMELOOKUP_TIME": pycurl.NAMELOOKUP_TIME,
     "CONNECT_TIME": pycurl.CONNECT_TIME,
     "APPCONNECT_TIME": pycurl.APPCONNECT_TIME,
     "PRETRANSFER_TIME": pycurl.PRETRANSFER_TIME,
```

### Comparing `curlquest-0.1.0/curlquest/sessions.py` & `curlquest-0.1.1/curlquest/sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import json as _json
 from urllib.parse import quote_plus
 
 import certifi
 import pycurl
 from requests.cookies import cookiejar_from_dict, merge_cookies
 
-from request_curl.helper import get_cookie
-from request_curl.models import Response
+from curlquest.helper import get_cookie
+from curlquest.models import Response
 
 
 class Session:
-    """A request_curl session.
+    """A curlquest session.
     Provides cookie persistence, connection-pooling, and configuration.
 
     Basic Usage::
 
-      >>> import request_curl
-      >>> s = request_curl.Session()
+      >>> import curlquest
+      >>> s = curlquest.Session()
       >>> s.get('https://httpbin.org/get')
       <Response [200]>
 
     Or as a context manager::
 
-      >>> with request_curl.Session() as s:
+      >>> with curlquest.Session() as s:
       ...     s.get('https://httpbin.org/get')
       <Response [200]>
     """
 
     def __init__(
         self,
         headers: Dict[str, str] = None,
```

### Comparing `curlquest-0.1.0/pyproject.toml` & `curlquest-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "curlquest"
-version = "0.1.0"
-description = "A user-friendly wrapper for pycurl that simplifies HTTP requests (fork of curl_request with a few changes)"
+version = "0.1.1"
+description = "A user-friendly wrapper for pycurl that simplifies HTTP requests (fork of request_curl with a few changes)"
 authors = [
     "Mauritz Uphoff <mauritz.uphoff@hs-osnabrueck.de>",
     "Ennis Blank <Ennis.Blank@fau.de>",
 ]
 readme = "README.md"
 license = "MIT"
 maintainers = ["Mauritz Uphoff", "Ennis Blank"]
-homepage = "https://github.com/Notifysolutions/request_curl"
-repository = "https://github.com/Notifysolutions/request_curl"
-documentation = "https://github.com/Notifysolutions/request_curl/blob/main/README.md"
+homepage = "https://github.com/Sygmei/curlquest"
+repository = "https://github.com/Sygmei/curlquest"
+documentation = "https://github.com/Sygmei/curlquest/blob/main/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "^2.28.1"
 Brotli = "^1.0.9"
 pycurl = "^7.45.2"
 certifi = "^2024.2.2"
```

### Comparing `curlquest-0.1.0/PKG-INFO` & `curlquest-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: curlquest
-Version: 0.1.0
-Summary: A user-friendly wrapper for pycurl that simplifies HTTP requests (fork of curl_request with a few changes)
-Home-page: https://github.com/Notifysolutions/request_curl
+Version: 0.1.1
+Summary: A user-friendly wrapper for pycurl that simplifies HTTP requests (fork of request_curl with a few changes)
+Home-page: https://github.com/Sygmei/curlquest
 License: MIT
 Author: Mauritz Uphoff
 Author-email: mauritz.uphoff@hs-osnabrueck.de
 Maintainer: Mauritz Uphoff
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,61 +16,61 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Brotli (>=1.0.9,<2.0.0)
 Requires-Dist: certifi (>=2024.2.2,<2025.0.0)
 Requires-Dist: pycurl (>=7.45.2,<8.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Project-URL: Documentation, https://github.com/Notifysolutions/request_curl/blob/main/README.md
-Project-URL: Repository, https://github.com/Notifysolutions/request_curl
+Project-URL: Documentation, https://github.com/Sygmei/curlquest/blob/main/README.md
+Project-URL: Repository, https://github.com/Sygmei/curlquest
 Description-Content-Type: text/markdown
 
 # Request Curl
 
 A user-friendly wrapper for pycurl that simplifies HTTP requests.
 
 ## Installation
 Use the package manager 
 [pip](https://pip.pypa.io/en/stable/) 
-to install [request_curl](https://pypi.org/project/request-curl/).
+to install [curlquest](https://pypi.org/project/request-curl/).
 
 > NOTE: You need Python and libcurl installed on your system to use or build pycurl. Some RPM distributions of curl/libcurl do not include everything necessary to build pycurl, in which case you need to install the developer specific RPM which is usually called curl-dev.
 
 
 ```
-pip install request_curl
+pip install curlquest
 ```
 
 # Quickstart
-A request_curl session manages cookies, connection pooling, and configurations.
+A curlquest session manages cookies, connection pooling, and configurations.
 
 Basic Usage:
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 s.get('https://httpbin.org/get') # returns <Response [200]>
 s.request('GET', 'https://httpbin.org/get') # returns <Response [200]>
 ```
 
 Using a Context Manager
 ```python
-import request_curl
-with request_curl.Session() as session:
+import curlquest
+with curlquest.Session() as session:
     session.get('https://httpbin.org/get') # returns <Response [200]>
 ```
 
 # Features
 
 ## Response Object
 
 The response object is similar to that of the [requests](https://pypi.org/project/requests/) library.
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 r = s.get("https://httpbin.org/get")
 
 print(r) # prints response object
 print(r.status_code) # prints status code
 print(r.content) # prints response content in bytes
 print(r.text) # prints response content as text
 print(r.json) # prints response content as JSON
@@ -78,104 +78,104 @@
 print(r.headers) # prints response headers
 ```
 
 ## Proxy Support
 Format the proxy as a string.
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 # supports authentication: r = s.get("https://httpbin.org/get", proxies="ip:port:user:password")
 r = s.get("https://httpbin.org/get", proxies="ip:port")
 ```
 
 ## HTTP2
 HTTP2 is disabled by default.
 
 ```python
-import request_curl
-s = request_curl.Session(http2=True)
+import curlquest
+s = curlquest.Session(http2=True)
 r = s.get("https://httpbin.org/get")
 ```
 
 ## Cipher Suites
 You can specify custom cipher suites as an array.
 
 ```python
-import request_curl
+import curlquest
 
 cipher_suite = [
     "AES128-SHA256",
     "AES256-SHA256",
     "AES128-GCM-SHA256",
     "AES256-GCM-SHA384"
 ]
-s = request_curl.Session(cipher_suite=cipher_suite)
+s = curlquest.Session(cipher_suite=cipher_suite)
 r = s.get("https://httpbin.org/get")
 ```
 
 ## Debug Request
 Set debug to True to print raw input and output headers.
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 r = s.get("https://httpbin.org/get", debug=True)
 ```
 
 ## Custom Headers
 Specify custom headers as a dictionary.
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 headers = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.163 Safari/537.36"
 }
 r = s.get("https://httpbin.org/get", headers=headers)
 ```
 
 ## Data
 
 ```python
-import request_curl
-s = request_curl.Session()
+import curlquest
+s = curlquest.Session()
 
 # sending form data
 form_data = {"key": "value"}
 response = s.post("https://httpbin.org/post", data=form_data)
 
 # sending json data
 json_data = {"key": "value"}
 response = s.post("https://httpbin.org/post", json=json_data)
 ```
 
 # Usage with Curl-Impersonate
-To use request_curl with [curl-impersonate](https://github.com/lwthiker/curl-impersonate), 
+To use curlquest with [curl-impersonate](https://github.com/lwthiker/curl-impersonate), 
 opt for our [custom Docker image](https://hub.docker.com/r/h3adex/request-curl-impersonate) by either pulling or building it. 
-The image comes with request_curl and curl-impersonate pre-installed. 
-Check below for a demonstration on impersonating firefox98 tls-fingerprint and request_curl with our custom Docker Image.
+The image comes with curlquest and curl-impersonate pre-installed. 
+Check below for a demonstration on impersonating firefox98 tls-fingerprint and curlquest with our custom Docker Image.
 
 **Note**: This feature is still considered experimental. Only tested with firefox fingerprint
 
 To pull the Docker image:
 
 ```bash
 docker pull h3adex/request-curl-impersonate:latest
 docker run --rm -it h3adex/request-curl-impersonate
 ```
 
 Example Python code for a target website:
 
 ```python
-import request_curl
-from request_curl import FIREFOX98_CIPHER_SUITE, FIREFOX98_HEADERS
+import curlquest
+from curlquest import FIREFOX98_CIPHER_SUITE, FIREFOX98_HEADERS
 
 # impersonates ff98
-session = request_curl.Session(
+session = curlquest.Session(
     http2=True, 
     cipher_suite=FIREFOX98_CIPHER_SUITE, 
     headers=FIREFOX98_HEADERS
 )
 response = session.get("https://tls.browserleaks.com/json")
 # <Response [200]>
 # "ja3_hash":"25e9b0dd5b8e9330b206eae87e885e19"
```

