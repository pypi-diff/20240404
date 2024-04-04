# Comparing `tmp/py_valid_proxy-0.2.6.tar.gz` & `tmp/py_valid_proxy-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_valid_proxy-0.2.6.tar", max compression
+gzip compressed data, was "py_valid_proxy-0.2.7.tar", max compression
```

## Comparing `py_valid_proxy-0.2.6.tar` & `py_valid_proxy-0.2.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1003 2024-01-04 08:06:17.202366 py_valid_proxy-0.2.6/README.md
--rw-r--r--   0        0        0      441 2024-01-04 03:08:20.465258 py_valid_proxy-0.2.6/py_valid_proxy/__init__.py
--rw-r--r--   0        0        0      238 2023-11-20 15:59:28.750899 py_valid_proxy-0.2.6/py_valid_proxy/__main__.py
--rw-r--r--   0        0        0  6266981 2023-11-15 16:20:05.685165 py_valid_proxy-0.2.6/py_valid_proxy/data/GeoLite2-Country.mmdb
--rw-r--r--   0        0        0     2538 2023-12-13 05:43:46.673826 py_valid_proxy-0.2.6/py_valid_proxy/main.py
--rw-r--r--   0        0        0     3582 2023-12-21 09:30:43.111043 py_valid_proxy-0.2.6/py_valid_proxy/valid_proxy.py
--rw-r--r--   0        0        0      486 2024-01-04 03:08:05.025457 py_valid_proxy-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 py_valid_proxy-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1020 2024-04-04 07:44:54.866879 py_valid_proxy-0.2.7/README.md
+-rw-r--r--   0        0        0      503 2024-04-04 07:47:58.493022 py_valid_proxy-0.2.7/py_valid_proxy/__init__.py
+-rw-r--r--   0        0        0      238 2023-11-20 15:59:28.750899 py_valid_proxy-0.2.7/py_valid_proxy/__main__.py
+-rw-r--r--   0        0        0  6266981 2023-11-15 16:20:05.685165 py_valid_proxy-0.2.7/py_valid_proxy/data/GeoLite2-Country.mmdb
+-rw-r--r--   0        0        0     2459 2024-04-04 07:46:27.183964 py_valid_proxy-0.2.7/py_valid_proxy/main.py
+-rw-r--r--   0        0        0     4128 2024-04-04 07:39:33.487215 py_valid_proxy-0.2.7/py_valid_proxy/valid_proxy.py
+-rw-r--r--   0        0        0      486 2024-04-04 07:45:10.095059 py_valid_proxy-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 py_valid_proxy-0.2.7/PKG-INFO
```

### Comparing `py_valid_proxy-0.2.6/README.md` & `py_valid_proxy-0.2.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,22 +34,22 @@
 	print('is alive')
 	pprint(proxy_info)
 else:
 	print('is dead')
 ```
 
 ```shell
-$ valid_proxy http://12.186.205.120:80
+$ valid_proxy -ip 12.186.205.120 -p 80 -s http
 http://12.186.205.120:80 ... is alive
 anonymity: high_anonymous
 country: US
 response time: 4.71 (secs)
 
-$ valid_proxy https://12.186.205.120:80
+$ valid_proxy -ip 12.186.205.120 -p 80 -s https 
 https://12.186.205.120:80 ... is alive
 anonymity: transparent
 country: US
 response time: 0.5 (secs)
 
-$ valid_proxy http://2.189.59.54:80
+$ valid_proxy -ip 2.189.59.54 -p 80
 http://2.189.59.54:80 ... is dead
 ```
```

### Comparing `py_valid_proxy-0.2.6/py_valid_proxy/data/GeoLite2-Country.mmdb` & `py_valid_proxy-0.2.7/py_valid_proxy/data/GeoLite2-Country.mmdb`

 * *Files identical despite different names*

### Comparing `py_valid_proxy-0.2.6/py_valid_proxy/valid_proxy.py` & `py_valid_proxy-0.2.7/py_valid_proxy/valid_proxy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 # @Author: Suvorinov Oleg
 # @Date:   2023-11-19 13:52:25
 # @Last Modified by:   Suvorinov Oleg
-# @Last Modified time: 2023-12-21 12:30:43
+# @Last Modified time: 2024-04-04 10:39:33
 
 import os
 import time
+import re
 from typing import List
+from datetime import datetime
 import json
 from dataclasses import dataclass, field
 
 import geoip2.database
 import requests
 from dataclasses_json import dataclass_json
 
@@ -23,39 +25,56 @@
         requests.exceptions.ReadTimeout,
         requests.exceptions.InvalidProxyURL,
         requests.exceptions.ProxyError,
         requests.exceptions.JSONDecodeError):
     pass
 
 
+now = datetime.now().strftime("%d-%m-%Y %H:%M:%S")
+
+
 @dataclass_json
 @dataclass
 class Proxy:
-    scheme: str = field(default='')
+    scheme: str = field(default='http')
     host: str = field(default='')
     port: int = field(default=80)
     export_address: List[str] = field(default_factory=list)
-    anonymity: str = field(default='')
+    anonymity: str = field(default='transparent')
     country: str = field(default='US')
     response_time: float = field(default=0.0)
-    to_from: str = field(default='valid_proxy')
+    to_from: str = field(default='')
+    last_checked: str = field(default=now)
 
 
 def get_origin_ip(timeout: int = 5) -> str:
     try:
         resp = requests.get(
             'http://httpbin.org/get',
             headers={"User-Agent": USER_AGENT},
             timeout=timeout
         ).json()
     except ValidProxyException:
         return ''
     return resp.get('origin', '')
 
 
+def valid_proxy_ip(ip_address: str) -> bool:
+    match = re.match(r"[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}", ip_address) # noqa
+
+    if not bool(match):
+        return False
+
+    bytes = ip_address.split(".")
+    for ip_byte in bytes:
+        if int(ip_byte) < 0 or int(ip_byte) > 255:
+            return False
+    return True
+
+
 def valid_proxy(
         host: str,
         port: int,
         scheme: str = 'http',
         timeout: int = 5) -> Proxy:
     """Valid proxy server ('alive' or 'dead')
 
@@ -71,14 +90,17 @@
         Connect timeout is number of seconds (default is 5 sec.)
     Returns
     -------
         None if proxy is 'dead'
         class Proxy if proxy is 'alive'
     """
     _proxy = None
+    if not valid_proxy_ip(host): 
+        raise ValidProxyException
+
     origin_ip = get_origin_ip()
 
     def _anonymity(origin_ip, response) -> str:
         via = response.get('headers', {}).get('Via', '')
 
         if origin_ip in json.dumps(response):
             return 'transparent'
```

### Comparing `py_valid_proxy-0.2.6/PKG-INFO` & `py_valid_proxy-0.2.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-valid-proxy
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Home-page: https://github.com/suvorinov/py_valid_proxy.git
 Author: Suvorinov Oleg
 Author-email: suvorinovoleg@yandex.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -50,22 +50,22 @@
 	print('is alive')
 	pprint(proxy_info)
 else:
 	print('is dead')
 ```
 
 ```shell
-$ valid_proxy http://12.186.205.120:80
+$ valid_proxy -ip 12.186.205.120 -p 80 -s http
 http://12.186.205.120:80 ... is alive
 anonymity: high_anonymous
 country: US
 response time: 4.71 (secs)
 
-$ valid_proxy https://12.186.205.120:80
+$ valid_proxy -ip 12.186.205.120 -p 80 -s https 
 https://12.186.205.120:80 ... is alive
 anonymity: transparent
 country: US
 response time: 0.5 (secs)
 
-$ valid_proxy http://2.189.59.54:80
+$ valid_proxy -ip 2.189.59.54 -p 80
 http://2.189.59.54:80 ... is dead
 ```
```

