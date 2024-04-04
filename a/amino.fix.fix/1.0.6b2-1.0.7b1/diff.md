# Comparing `tmp/amino.fix.fix-1.0.6b2.tar.gz` & `tmp/amino.fix.fix-1.0.7b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.fix.fix-1.0.6b2.tar", last modified: Wed Mar 27 15:36:48 2024, max compression
+gzip compressed data, was "amino.fix.fix-1.0.7b1.tar", last modified: Thu Apr  4 01:04:20 2024, max compression
```

## Comparing `amino.fix.fix-1.0.6b2.tar` & `amino.fix.fix-1.0.7b1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.358505 amino.fix.fix-1.0.6b2/
--rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.6b2/LICENSE
--rw-rw-rw-   0        0        0     3895 2024-03-27 15:36:48.359499 amino.fix.fix-1.0.6b2/PKG-INFO
--rw-rw-rw-   0        0        0     3412 2024-03-27 12:39:00.000000 amino.fix.fix-1.0.6b2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.329113 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/
--rw-rw-rw-   0        0        0     3895 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-27 15:36:48.000000 amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.335195 amino.fix.fix-1.0.6b2/aminofixfix/
--rw-rw-rw-   0        0        0     1147 2024-03-09 18:08:07.000000 amino.fix.fix-1.0.6b2/aminofixfix/__init__.py
--rw-rw-rw-   0        0        0    24432 2024-03-27 15:36:06.000000 amino.fix.fix-1.0.6b2/aminofixfix/acm.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.343722 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/
--rw-rw-rw-   0        0        0     1148 2024-03-09 18:54:15.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/__init__.py
--rw-rw-rw-   0        0        0    16421 2024-03-27 15:23:30.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/acm.py
--rw-rw-rw-   0        0        0    94792 2024-03-27 14:17:41.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/client.py
--rw-rw-rw-   0        0        0    14927 2024-03-19 20:43:01.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/socket.py
--rw-rw-rw-   0        0        0   108618 2024-03-27 14:17:43.000000 amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/sub_client.py
--rw-rw-rw-   0        0        0   101218 2024-03-27 14:29:31.000000 amino.fix.fix-1.0.6b2/aminofixfix/client.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.351223 amino.fix.fix-1.0.6b2/aminofixfix/lib/
--rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/__init__.py
--rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:36:48.357504 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/
--rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/__init__.py
--rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/aiohttp.py
--rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/requests.py
--rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/unsuccessful_import.py
--rw-rw-rw-   0        0        0     4016 2024-03-15 22:31:38.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/headers.py
--rw-rw-rw-   0        0        0     4659 2024-03-27 15:36:30.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/helpers.py
--rw-rw-rw-   0        0        0   198008 2024-03-27 13:16:33.000000 amino.fix.fix-1.0.6b2/aminofixfix/lib/objects.py
--rw-rw-rw-   0        0        0    14925 2024-03-19 20:41:56.000000 amino.fix.fix-1.0.6b2/aminofixfix/socket.py
--rw-rw-rw-   0        0        0   144951 2024-03-27 15:36:10.000000 amino.fix.fix-1.0.6b2/aminofixfix/sub_client.py
--rw-rw-rw-   0        0        0       42 2024-03-27 15:36:48.360501 amino.fix.fix-1.0.6b2/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-03-27 15:36:33.000000 amino.fix.fix-1.0.6b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.371247 amino.fix.fix-1.0.7b1/
+-rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.7b1/LICENSE
+-rw-rw-rw-   0        0        0     4047 2024-04-04 01:04:20.371247 amino.fix.fix-1.0.7b1/PKG-INFO
+-rw-rw-rw-   0        0        0     3564 2024-04-04 01:03:33.000000 amino.fix.fix-1.0.7b1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.350220 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/
+-rw-rw-rw-   0        0        0     4047 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.355220 amino.fix.fix-1.0.7b1/aminofixfix/
+-rw-rw-rw-   0        0        0     1365 2024-04-04 01:01:01.000000 amino.fix.fix-1.0.7b1/aminofixfix/__init__.py
+-rw-rw-rw-   0        0        0    24271 2024-04-04 00:32:10.000000 amino.fix.fix-1.0.7b1/aminofixfix/acm.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.360733 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/
+-rw-rw-rw-   0        0        0     1366 2024-04-04 01:03:00.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/__init__.py
+-rw-rw-rw-   0        0        0    16275 2024-04-04 00:31:58.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/acm.py
+-rw-rw-rw-   0        0        0    95310 2024-04-04 00:38:37.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/client.py
+-rw-rw-rw-   0        0        0    14887 2024-04-04 00:45:22.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/socket.py
+-rw-rw-rw-   0        0        0   108095 2024-04-04 00:37:41.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/sub_client.py
+-rw-rw-rw-   0        0        0   101798 2024-04-04 00:43:54.000000 amino.fix.fix-1.0.7b1/aminofixfix/client.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.365734 amino.fix.fix-1.0.7b1/aminofixfix/lib/
+-rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/__init__.py
+-rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.370246 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/
+-rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/__init__.py
+-rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/aiohttp.py
+-rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/requests.py
+-rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/unsuccessful_import.py
+-rw-rw-rw-   0        0        0     5911 2024-04-04 00:41:52.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/headers.py
+-rw-rw-rw-   0        0        0     5144 2024-04-04 01:04:08.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/helpers.py
+-rw-rw-rw-   0        0        0   198878 2024-04-04 00:03:14.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/objects.py
+-rw-rw-rw-   0        0        0    14885 2024-04-04 00:10:47.000000 amino.fix.fix-1.0.7b1/aminofixfix/socket.py
+-rw-rw-rw-   0        0        0   144345 2024-04-04 00:38:17.000000 amino.fix.fix-1.0.7b1/aminofixfix/sub_client.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 01:04:20.372246 amino.fix.fix-1.0.7b1/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2024-04-04 01:04:11.000000 amino.fix.fix-1.0.7b1/setup.py
```

### Comparing `amino.fix.fix-1.0.6b2/LICENSE` & `amino.fix.fix-1.0.7b1/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b2/PKG-INFO` & `amino.fix.fix-1.0.7b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.6b2
+Version: 1.0.7b1
 Summary: Library for Aminoapps
 Home-page: https://github.com/imperialwool/Amino.fix.fix
 Author: imperialwool
 Author-email: hi@iwool.dev
 License: MIT
 Keywords: aminoapps,amino.fix,amino.fix.fix,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,imperialwool
 Requires-Python: >=3.8
@@ -12,15 +12,15 @@
 Provides-Extra: requests
 Provides-Extra: aiohttp
 License-File: LICENSE
 
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.6b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
@@ -42,14 +42,16 @@
 If you want to use Async version of library, you should `import aminofixfix.asyncfixfix`.
 
 Also instead HTTPX you can use aiohttp, Requests or Urllib3. Just install additional dependencies, if you wanna use them:
 
 - `pip install amino.fix.fix[requests]` # only sync
 - `pip install amino.fix.fix[aiohttp]` # only async
 
+Please report any issues and bugs that Request and aiohttp are causing when you use them instead of HTTPX! This feature in beta and not tested well.
+
 Example:
 
 ```python
 import aminofixfix
 
 client = aminofixfix.Client()
 client.login("she.a@lil.freak", "sheforthestreets")
```

### Comparing `amino.fix.fix-1.0.6b2/README.md` & `amino.fix.fix-1.0.7b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.6b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
@@ -27,14 +27,16 @@
 If you want to use Async version of library, you should `import aminofixfix.asyncfixfix`.
 
 Also instead HTTPX you can use aiohttp, Requests or Urllib3. Just install additional dependencies, if you wanna use them:
 
 - `pip install amino.fix.fix[requests]` # only sync
 - `pip install amino.fix.fix[aiohttp]` # only async
 
+Please report any issues and bugs that Request and aiohttp are causing when you use them instead of HTTPX! This feature in beta and not tested well.
+
 Example:
 
 ```python
 import aminofixfix
 
 client = aminofixfix.Client()
 client.login("she.a@lil.freak", "sheforthestreets")
```

### Comparing `amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/PKG-INFO` & `amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.6b2
+Version: 1.0.7b1
 Summary: Library for Aminoapps
 Home-page: https://github.com/imperialwool/Amino.fix.fix
 Author: imperialwool
 Author-email: hi@iwool.dev
 License: MIT
 Keywords: aminoapps,amino.fix,amino.fix.fix,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,imperialwool
 Requires-Python: >=3.8
@@ -12,15 +12,15 @@
 Provides-Extra: requests
 Provides-Extra: aiohttp
 License-File: LICENSE
 
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.6b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
@@ -42,14 +42,16 @@
 If you want to use Async version of library, you should `import aminofixfix.asyncfixfix`.
 
 Also instead HTTPX you can use aiohttp, Requests or Urllib3. Just install additional dependencies, if you wanna use them:
 
 - `pip install amino.fix.fix[requests]` # only sync
 - `pip install amino.fix.fix[aiohttp]` # only async
 
+Please report any issues and bugs that Request and aiohttp are causing when you use them instead of HTTPX! This feature in beta and not tested well.
+
 Example:
 
 ```python
 import aminofixfix
 
 client = aminofixfix.Client()
 client.login("she.a@lil.freak", "sheforthestreets")
```

### Comparing `amino.fix.fix-1.0.6b2/amino.fix.fix.egg-info/SOURCES.txt` & `amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/__init__.py` & `amino.fix.fix-1.0.7b1/aminofixfix/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from .acm import ACM
 from .client import Client
 from .sub_client import SubClient
 from .socket import Callbacks, SocketHandler
 from .lib import exceptions, helpers, objects, headers
 
-from httpx import get
+from json import loads
+from threading import Thread
+from urllib.request import urlopen
 from pkg_resources import parse_version as version
 
-try:
-    __newest__ = get("https://pypi.org/pypi/amino.fix.fix/json").json()["info"]["version"]
+def work():
+    try:
+        response = urlopen("https://pypi.org/pypi/amino.fix.fix/json")
+        data = loads(response.read())
 
-    if version(__newest__) > version(helpers.LIBRARY_VERSION):
-        print("\n!!! New version of amino.fix.fix is available !!!",
-            "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
-            "!!! Please, update library to last version !!!\n", sep="\n")
-    elif version(__newest__) < version(helpers.LIBRARY_VERSION):
-        print("\n!!! ATTENTION, MODIFIED LIBRARY OR PREVIEW VERSION !!!",
-            "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
-            "!!! Please, make sure that library installed from verified sources !!!",
-            "Example: pip install amino.fix.fix\n", sep="\n")
-except:
-    print("\nCan't check if amino.fix.fix needs update. Please, check internet connection or firewall.\n")
+        __newest__ = data["info"]["version"]
+
+        if version(__newest__) > version(helpers.LIBRARY_VERSION):
+            print("\n!!! New version of amino.fix.fix is available !!!",
+                "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
+                "!!! Please, update library to last version !!!\n", sep="\n")
+        elif version(__newest__) < version(helpers.LIBRARY_VERSION):
+            print("\n!!! ATTENTION, MODIFIED LIBRARY OR PREVIEW VERSION !!!",
+                "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
+                "!!! Please, make sure that library installed from verified sources !!!",
+                "Example: pip install amino.fix.fix\n", sep="\n")
+    except:
+        print("\nCan't check if amino.fix.fix needs update. Please, check internet connection or firewall.\n")
+
+Thread(target=work).start()
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/acm.py` & `amino.fix.fix-1.0.7b1/aminofixfix/acm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
+from json import dumps
 from typing import BinaryIO
-from json import loads, dumps
-from time import time as timestamp
 
 from .client import Client
+from .lib.helpers import inttime
 from .lib import exceptions, headers, objects
 
 class ACM(Client):
     """
     ACM is community manager.
 
     If you have leader or agent rights, you can edit your community.
@@ -82,15 +82,15 @@
             },
             "joinType": joinType,
             "name": name,
             "primaryLanguage": primaryLanguage,
             "tagline": tagline,
             "templateId": 9,
             "themeColor": themeColor,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/community", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def delete_community(self, email: str, password: str, verificationCode: str):
@@ -137,15 +137,15 @@
 
         Recieving:
         - object `dict`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         response = self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.CommunityList(loads(response.text)["communityList"]).CommunityList
+        else: return objects.CommunityList(response.json()["communityList"]).CommunityList
 
     def get_categories(self, start: int = 0, size: int = 25):
         """
         Getting categories of communities.
 
         Accepting:
         - start: int = 0
@@ -156,15 +156,15 @@
         Recieving:
         - object `dict`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return loads(response.text)
+        else: return response.json()
 
     def change_sidepanel_color(self, color: str):
         """
         Change sidepanel color.
 
         Accepting:
         - color: str
@@ -173,21 +173,21 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "path": "appearance.leftSidePanel.style.iconColor",
             "value": color if len(color) == 7 else "#000000",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return response.status_code
-        else: return loads(response.text)
+        else: return response.json()
 
     def get_themepack_info(self):
         """
         This method can be used for getting info about current themepack of community.
 
         Recieving:
         - object
@@ -272,15 +272,15 @@
         Recieving:
         - object
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return loads(response.text)
+        else: return response.json()
 
     def promote(self, userId: str, rank: str):
         """
         Promote user to curator, leader or agent.
 
         Accepting:
         - userId: str
@@ -315,15 +315,15 @@
         - object `JoinRequest`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         response = self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.JoinRequest(loads(response.text)).JoinRequest
+        else: return objects.JoinRequest(response.json()).JoinRequest
 
     def accept_join_request(self, userId: str):
         """
         Accept user to join your precious community.
 
         "Congratulations!
 
@@ -379,15 +379,15 @@
         - object `CommunityStats`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         response = self.session.get(f"/x{self.comId}/s/community/stats", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.CommunityStats(loads(response.text)["communityStats"]).CommunityStats
+        else: return objects.CommunityStats(response.json()["communityStats"]).CommunityStats
 
     def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
         """
         Get community user statistics.
 
         Accepting:
         - type: str
@@ -405,15 +405,15 @@
 
         if type.lower() == "leader": target = "leader"
         elif type.lower() == "curator": target = "curator"
         else: raise exceptions.WrongType(type)
 
         response = self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.UserProfileList(loads(response.text)["userProfileList"]).UserProfileList
+        else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def change_welcome_message(self, message: str, isEnabled: bool = True):
         """
         Change welcome message of community.
 
         Accepting:
         - message: str
@@ -425,15 +425,15 @@
         """
         data = dumps({
             "path": "general.welcomeMessage",
             "value": {
                 "enabled": isEnabled,
                 "text": message
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -446,15 +446,15 @@
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "endpoint": aminoId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"/x{self.comId}/s/community/settings", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -467,15 +467,15 @@
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "content": message,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -491,15 +491,15 @@
         - themePackUrl: str = None
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if name is not None: data["name"] = name
         if description is not None: data["content"] = description
         if aminoId is not None: data["endpoint"] = aminoId
         if primaryLanguage is not None: data["primaryLanguage"] = primaryLanguage
         if themePackUrl is not None: data["themePackUrl"] = themePackUrl
 
@@ -543,15 +543,15 @@
         elif module.lower() == "externalcontent": mod = "module.externalContent.enabled"
         elif module.lower() == "topiccategories": mod = "module.topicCategories.enabled"
         else: raise exceptions.SpecifyType()
 
         data = dumps({
             "path": mod,
             "value": isEnabled,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -566,15 +566,15 @@
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "monthlyFee": monthlyFee,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -607,15 +607,15 @@
         Recieving:
         - object `NoticeList`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.NoticeList(loads(response.text)["noticeList"]).NoticeList
+        else: return objects.NoticeList(response.json()["noticeList"]).NoticeList
 
     def delete_pending_role(self, noticeId: str):
         """
         Delete pending role.
 
         Accepting:
         - noticeId: str
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/__init__.py` & `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from .acm import ACM
 from .client import Client
 from .sub_client import SubClient
 from .socket import Callbacks, SocketHandler
 from ..lib import exceptions, helpers, objects, headers
 
-from httpx import get
+from json import loads
+from threading import Thread
+from urllib.request import urlopen
 from pkg_resources import parse_version as version
 
-try:
-    __newest__ = get("https://pypi.org/pypi/amino.fix.fix/json").json()["info"]["version"]
+def work():
+    try:
+        response = urlopen("https://pypi.org/pypi/amino.fix.fix/json")
+        data = loads(response.read())
 
-    if version(__newest__) > version(helpers.LIBRARY_VERSION):
-        print("\n!!! New version of amino.fix.fix is available !!!",
-            "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
-            "!!! Please, update library to last version !!!\n", sep="\n")
-    elif version(__newest__) < version(helpers.LIBRARY_VERSION):
-        print("\n!!! ATTENTION, MODIFIED LIBRARY OR PREVIEW VERSION !!!",
-            "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
-            "!!! Please, make sure that library installed from verified sources !!!",
-            "Example: pip install amino.fix.fix\n", sep="\n")
-except:
-    print("\nCan't check if amino.fix.fix needs update. Please, check internet connection or firewall.\n")
+        __newest__ = data["info"]["version"]
+
+        if version(__newest__) > version(helpers.LIBRARY_VERSION):
+            print("\n!!! New version of amino.fix.fix is available !!!",
+                "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
+                "!!! Please, update library to last version !!!\n", sep="\n")
+        elif version(__newest__) < version(helpers.LIBRARY_VERSION):
+            print("\n!!! ATTENTION, MODIFIED LIBRARY OR PREVIEW VERSION !!!",
+                "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
+                "!!! Please, make sure that library installed from verified sources !!!",
+                "Example: pip install amino.fix.fix\n", sep="\n")
+    except:
+        print("\nCan't check if amino.fix.fix needs update. Please, check internet connection or firewall.\n")
+
+Thread(target=work).start()
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/acm.py` & `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/acm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
+from json import dumps
 from typing import BinaryIO
-from json import loads, dumps
-from time import time as timestamp
 
 from . import client
+from ..lib.helpers import inttime
 from ..lib import exceptions, headers, objects
 
 class ACM(client.Client):
     def __init__(self, profile: objects.UserProfile, comId: str = None, proxies: dict = None):
         client.Client.__init__(self)
 
         self.profile = profile
@@ -29,15 +29,15 @@
             },
             "joinType": joinType,
             "name": name,
             "primaryLanguage": primaryLanguage,
             "tagline": tagline,
             "templateId": 9,
             "themeColor": themeColor,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/community", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def delete_community(self, email: str, password: str, verificationCode: str):
@@ -57,33 +57,33 @@
         response = await self.session.post(f"/g/s-x{self.comId}/community/delete-request", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def list_communities(self, start: int = 0, size: int = 25):
         response = await self.session.get(f"/g/s/community/managed?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.CommunityList(loads(response.text)["communityList"]).CommunityList
+        else: return objects.CommunityList(response.json()["communityList"]).CommunityList
 
     async def get_categories(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.get(f"/x{self.comId}/s/blog-category?start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return loads(response.text)
+        else: return response.json()
 
     async def change_sidepanel_color(self, color: str):
         data = dumps({
             "path": "appearance.leftSidePanel.style.iconColor",
             "value": color,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return response.status_code
-        else: return loads(response.text)
+        else: return response.json()
 
     async def get_themepack_info(self, file: BinaryIO):
         """
         This method can be used for getting info about current themepack of community.
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.get(f"/g/s-x{self.comId}/community/info?withTopicList=1&withInfluencerList=1&influencerListOrderStrategy=fansCount", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
@@ -157,15 +157,15 @@
                 - h = 64
         - you *can* specify "x" and "y" if you want
         - theoretically you can provide different "w" and "h"
         """
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.post(f"/x{self.comId}/s/media/upload/target/community-theme-pack", data=file.read(), headers=headers.Headers(data=file.read()).s_headers, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return loads(response.text)
+        else: return response.json()
 
     async def promote(self, userId: str, rank: str):
         rank = rank.lower().replace("agent", "transfer-agent")
 
         if rank.lower() not in ["transfer-agent", "leader", "curator"]:
             raise exceptions.WrongType(rank)
 
@@ -175,15 +175,15 @@
         else: return response.status_code
 
     async def get_join_requests(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         response = await self.session.get(f"/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.JoinRequest(loads(response.text)).JoinRequest
+        else: return objects.JoinRequest(response.json()).JoinRequest
 
     async def accept_join_request(self, userId: str):
         data = dumps({})
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.post(f"/x{self.comId}/s/community/membership-request/{userId}/accept", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
@@ -198,55 +198,55 @@
         else: return response.status_code
 
     async def get_community_stats(self):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         response = await self.session.get(f"/x{self.comId}/s/community/stats", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.CommunityStats(loads(response.text)["communityStats"]).CommunityStats
+        else: return objects.CommunityStats(response.json()["communityStats"]).CommunityStats
 
     async def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
 
         if type.lower() == "leader": target = "leader"
         elif type.lower() == "curator": target = "curator"
         else: raise exceptions.WrongType(type)
 
         response = await self.session.get(f"/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.UserProfileList(loads(response.text)["userProfileList"]).UserProfileList
+        else: return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     async def change_welcome_message(self, message: str, isEnabled: bool = True):
         data = dumps({
             "path": "general.welcomeMessage",
             "value": {
                 "enabled": isEnabled,
                 "text": message
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def change_guidelines(self, message: str):
         data = dumps({
             "content": message,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.post(f"/x{self.comId}/s/community/guideline", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def edit_community(self, name: str = None, description: str = None, aminoId: str = None, primaryLanguage: str = None, themePackUrl: str = None):
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if name is not None: data["name"] = name
         if description is not None: data["content"] = description
         if aminoId is not None: data["endpoint"] = aminoId
         if primaryLanguage is not None: data["primaryLanguage"] = primaryLanguage
         if themePackUrl is not None: data["themePackUrl"] = themePackUrl
 
@@ -275,26 +275,26 @@
         elif module.lower() == "externalcontent": mod = "module.externalContent.enabled"
         elif module.lower() == "topiccategories": mod = "module.topicCategories.enabled"
         else: raise exceptions.SpecifyType()
 
         data = dumps({
             "path": mod,
             "value": isEnabled,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.post(f"/x{self.comId}/s/community/configuration", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def add_influencer(self, userId: str, monthlyFee: int):
         data = dumps({
             "monthlyFee": monthlyFee,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.post(f"/x{self.comId}/s/influencer/{userId}", headers=self.additional_headers(data=data), data=data, proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -304,14 +304,14 @@
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def get_notice_list(self, start: int = 0, size: int = 25):
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.get(f"/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
-        else: return objects.NoticeList(loads(response.text)["noticeList"]).NoticeList
+        else: return objects.NoticeList(response.json()["noticeList"]).NoticeList
 
     async def delete_pending_role(self, noticeId: str):
         if self.comId is None: raise exceptions.CommunityNeeded()
         response = await self.session.delete(f"/x{self.comId}/s/notice/{noticeId}", headers=self.additional_headers(), proxies=self.proxies)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/client.py` & `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
-from uuid import UUID
-from os import urandom
-from base64 import b64encode
+from time import sleep
+from json import dumps
 from threading import Thread
-from binascii import hexlify
-from json import loads, dumps
-from time import timezone, sleep
 from typing import BinaryIO, Union
-from time import time as timestamp
 from httpx import Timeout as TimeoutConfig
 from httpx import AsyncClient as HttpxClient
-from locale import getdefaultlocale as locale
 
-from ..lib.helpers import gen_deviceId
 from .socket import Callbacks, SocketHandler
 from ..lib import exceptions, headers, objects, helpers
 from ..lib.facades import AiohttpClient, AiohttpResponse
+from ..lib.helpers import gen_deviceId, inttime, clientrefid, str_uuid4, bytes_to_b64, LOCAL_TIMEZONE
 
 class Client(Callbacks, SocketHandler):
     def __init__(
         self,
         deviceId: str = None, userAgent: str = None, proxies: dict = None,
         socket_trace = False, socketDebugging = False, socket_enabled = True,
         autoDevice = False, http2_enabled: bool = True,
@@ -35,14 +29,15 @@
         api_library: objects.APILibraries = objects.APILibraries.HTTPX
     ):
         self.api = "https://service.aminoapps.com/api/v1"
         self.proxies = proxies
         self.configured = False
         self.authenticated = False
         self.autoDevice = autoDevice
+        self.api_library = api_library
         self.socket_enabled = socket_enabled
         self.device_id = deviceId if deviceId else gen_deviceId()
         self.user_agent = userAgent if userAgent else helpers.gen_userAgent()
 
         if disable_timeout:
             self.timeout_settings = TimeoutConfig(None)
         elif isinstance(own_timeout, TimeoutConfig):
@@ -53,35 +48,36 @@
                 write=write_timeout,
                 pool=pool_timeout,
                 connect=connect_timeout
             )
         else:
             self.timeout_settings = TimeoutConfig(default_timeout or 60)
         
-        if self.api_library == objects.APILibraries.HTTPX:
-            self.session = HttpxClient(
+        if self.api_library == objects.APILibraries.REQUESTS:
+            raise Exception("You cant use requests in async client. Requests is sync library.")
+        elif self.api_library == objects.APILibraries.AIOHTTP:
+            self.session = AiohttpClient(
                 headers=headers.BASIC_HEADERS,
                 http2=http2_enabled,
                 base_url=self.api,
                 proxies=proxies,
                 timeout=self.timeout_settings
             )
-        elif self.api_library == objects.APILibraries.REQUESTS:
-            raise Exception("You cant use requests in async client. Requests is sync library.")
-        elif self.api_library == objects.APILibraries.AIOHTTP:
-            self.session = AiohttpClient(
+        else:
+            self.session = HttpxClient(
                 headers=headers.BASIC_HEADERS,
                 http2=http2_enabled,
                 base_url=self.api,
                 proxies=proxies,
                 timeout=self.timeout_settings
             )
-
-        SocketHandler.__init__(self, self, socket_trace=socket_trace, debug=socketDebugging)
-        Callbacks.__init__(self, self)
+            
+        if self.socket_enabled:
+            SocketHandler.__init__(self, self, socket_trace=socket_trace, debug=socketDebugging)
+            Callbacks.__init__(self, self)
         self.sid = None
         self.json = None
         self.secret = None
         self.userId = None
         self.account: objects.UserProfile = objects.UserProfile(None)
         self.profile: objects.UserProfile = objects.UserProfile(None)
 
@@ -102,15 +98,15 @@
         if "on" in status.lower(): status = 1
         elif "off" in status.lower(): status = 2
         else: raise exceptions.WrongType(status)
 
         data = dumps({
             "onlineStatus": status,
             "duration": 86400,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/g/s/user-profile/{self.profile.userId}/online-status", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -251,36 +247,37 @@
 
         self.account: objects.UserProfile = await self.get_user_info(uId)
         self.profile: objects.UserProfile = await self.get_user_info(uId)
 
         if self.socket_enabled:
             self.run_amino_socket()
 
-    async def login(self, email: str, password: str):
+    async def login(self, email: str, password: str, client_type: int = 100):
         """
         Login into an account.
 
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
+            - **client_type**: Type of Client.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "email": email,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
-            "clientType": 300,
+            "clientType": client_type,
             "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/auth/login", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: exceptions.CheckException(response)
         else:
             self.authenticated = True
             self.json = response.json()
@@ -291,35 +288,36 @@
             self.secret = self.json.get("secret")
 
             if self.socket_enabled:
                 self.run_amino_socket()
 
             return response.json()
 
-    async def login_phone(self, phoneNumber: str, password: str):
+    async def login_phone(self, phoneNumber: str, password: str, client_type: int = 100):
         """
         Login into an account.
 
         **Parameters**
             - **phoneNumber** : Phone number of the account.
             - **password** : Password of the account.
+            - **client_type**: Type of Client.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "phoneNumber": phoneNumber,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
-            "clientType": 300,
+            "clientType": client_type,
             "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/auth/login", headers=self.additional_headers(data=data), data=data)
         self.run_amino_socket()
         if response.status_code != 200: exceptions.CheckException(response)
 
         else:
@@ -351,15 +349,15 @@
         """
         data = dumps({
             "v": 2,
             "secret": secret,
             "deviceID": self.device_id,
             "clientType": 100,
             "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/auth/login", headers=self.additional_headers(data=data), data=data)
         self.run_amino_socket()
         if response.status_code != 200: exceptions.CheckException(response)
 
         else:
@@ -410,15 +408,15 @@
                     "code": verificationCode
                 },
                 "type": 1,
                 "identity": email
             },
             "type": 1,
             "identity": email,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })        
 
         response = await self.session.post(f"/g/s/auth/register", data=data, headers=self.additional_headers(data=data), timeout=timeout)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()
@@ -436,15 +434,15 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "secret": f"0 {password}",
             "deviceID": self.device_id,
             "email": email,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/account/delete-request/cancel", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -460,15 +458,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "deviceID": self.device_id,
             "clientType": 100,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/auth/logout", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
 
@@ -504,15 +502,15 @@
         else: raise exceptions.SpecifyType()
 
         if age <= 12: raise exceptions.AgeTooLow()
 
         data = dumps({
             "age": age,
             "gender": gender,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/persona/profile/basic", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -532,15 +530,15 @@
         """
         data = dumps({
             "validationContext": {
                 "type": 1,
                 "identity": email,
                 "data": {"code": code}},
             "deviceID": self.device_id,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/auth/check-security-validation", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -659,34 +657,35 @@
 
         response = await self.session.post(f"/g/s/auth/reset-password", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
-    async def check_device(self, deviceId: str):
+    async def check_device(self, deviceId: str, locale: str = "en_US"):
         """
         Check if the Device ID is valid.
 
         **Parameters**
             - **deviceId** : ID of the Device.
+            - **locale** : Locale like "ru_RU", "en_US"
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "deviceID": deviceId,
             "bundleID": "com.narvii.amino.master",
             "clientType": 100,
-            "timezone": -timezone // 1000,
+            "timezone": LOCAL_TIMEZONE,
             "systemPushEnabled": True,
-            "locale": locale()[0],
-            "timestamp": int(timestamp() * 1000)
+            "locale": locale,
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/device", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             self.configured = True; return response.status_code
@@ -710,19 +709,21 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if fileType == "audio":
             t = "audio/aac"
         elif fileType == "image":
             t = "image/jpg"
+        elif fileType == "gif":
+            t = "image/gif"
         else: raise exceptions.SpecifyType(fileType)
 
         data = file.read()
 
-        response = await self.session.post(f"/g/s/media/upload", data=data, headers=self.additional_headers(type=t, data=data))
+        response = await self.session.post(f"/g/s/media/upload", data=data, headers=self.additional_headers(content_type=t, data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["mediaValue"]
 
     def handle_socket_message(self, data):
         return self.resolve(data)
@@ -777,16 +778,16 @@
         response = await self.session.get(f"/g/s/user-profile/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfile(response.json()["userProfile"]).UserProfile
 
     async def watch_ad(self, userId: str = None):
-        data = dumps(headers.Tapjoy(userId if userId else self.userId).data) 
-        response = await self.session.post("https://ads.tapdaq.com/v4/analytics/reward", data=data, headers=headers.Tapjoy().headers)
+        data = headers.Tapjoy.Data(userId or self.userId)
+        response = await self.session.post("https://ads.tapdaq.com/v4/analytics/reward", data=data, headers=headers.Tapjoy.Headers())
         if response.status_code != 204: return exceptions.CheckException(response)
         else: return response.status_code
 
     async def get_chat_threads(self, start: int = 0, size: int = 25):
         """
         List of Chats the account is in.
 
@@ -888,15 +889,15 @@
         else: raise exceptions.WrongType()
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if isGlobal is True: data["type"] = 2; data["eventSource"] = "GlobalComposeMenu"
         else: data["type"] = 0
 
         if publishToGlobal is True: data["publishToGlobal"] = 1
         else: data["publishToGlobal"] = 0
@@ -925,15 +926,15 @@
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType
 
         data = dumps({
             "uids": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/chat/thread/{chatId}/member/invite", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1216,15 +1217,15 @@
         """
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
             "message": reason,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["objectId"] = userId
             data["objectType"] = 0
 
         elif blogId:
@@ -1267,76 +1268,87 @@
             - **fileType** : Type of the file.
                 - ``audio``, ``image``, ``gif``
             - **messageType** : Type of the Message.
             - **mentionUserIds** : List of User IDS to mention. '@' needed in the Message.
             - **replyTo** : Message ID to reply to.
             - **stickerId** : Sticker ID to be sent.
             - **embedType** : Type of the Embed. Can be aminofixfix.lib.objects.EmbedTypes only. By default it's LinkSnippet one.
-            - **embedLink** : Link of the Embed.
-            - **embedImage** : Image of the Embed. Required to send Embed.
-            - **embedId** : ID of the Embed. Works only in AttachedObject Embeds.
-            - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds.
-            - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds.
-            - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds.
+            - **embedLink** : Link of the Embed. Can be only "ndc://" link if its AttachedObject.
+            - **embedImage** : Image of the Embed. Required to send Embed, if its LinkSnippet. Can be only 1024x1024 max. Can be string to existing image uploaded to Amino or it can be opened (not readed) file.
+            - **embedId** : ID of the Embed. Works only in AttachedObject Embeds. It can be any ID, just gen it using str_uuid4().
+            - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds. Just look what values AttachedObjectTypes enum contains.
+            - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds. Can be empty.
+            - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds. Can be empty.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if message is not None and file is None:
             message = message.replace("<$", "‎‏").replace("$>", "‬‭")
 
         mentions = []
         if mentionUserIds:
             mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
 
-        if not isinstance(embedImage, BinaryIO):
-            embedType = None
+        if embedImage and not isinstance(embedImage, str):
+            try: readEmbed = embedImage.read()
+            except: embedType = None
 
         if embedType == objects.EmbedTypes.LINK_SNIPPET:
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "extensions": {
                     "linkSnippetList": [{
                         "link": embedLink,
                         "mediaType": 100,
-                        "mediaUploadValue": b64encode(embedImage.read()).decode(),
+                        "mediaUploadValue": bytes_to_b64(readEmbed),
                         "mediaUploadValueContentType": "image/png"
                     }],
                     "mentionedArray": mentions
                 },
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
         elif embedType == objects.EmbedTypes.ATTACHED_OBJECT:
+            try: embedObjectType.value
+            except: raise Exception("You SHOULD pass AttachedEmbedTypes.")
+
+            if isinstance(embedImage, str):
+                image = [[100, embedImage, None]]
+            elif embedImage:
+                image = [[100, await self.upload_media(embedImage, "image"), None]]
+            else:
+                image = None
+
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "attachedObject": {
                     "objectId": embedId,
-                    "objectType": embedObjectType,
+                    "objectType": embedObjectType.value,
                     "link": embedLink,
                     "title": embedTitle,
                     "content": embedContent,
-                    "mediaList": [[100, await self.upload_media(embedImage, "image"), None]]
+                    "mediaList": image
                 },
                 "extensions": {"mentionedArray": mentions},
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
         else:
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "extensions": {"mentionedArray": mentions},
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
 
         if replyTo: data["replyMessageId"] = replyTo
 
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
@@ -1356,15 +1368,15 @@
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
             else: raise exceptions.SpecifyType(fileType)
 
-            data["mediaUploadValue"] = b64encode(file.read()).decode()
+            data["mediaUploadValue"] = bytes_to_b64(file.read())
 
         data = dumps(data)
 
         response = await self.session.post(f"/g/s/chat/thread/{chatId}/message", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
@@ -1383,15 +1395,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "adminOpName": 102,
             "adminOpNote": {"content": reason},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         data = dumps(data)
         
         if not asStaff: response = await self.session.delete(f"/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         else: response = await self.session.post(f"/g/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
@@ -1410,15 +1422,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "messageId": messageId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/g/s/chat/thread/{chatId}/mark-as-read", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1446,15 +1458,15 @@
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if announcement: data["extensions"] = {"announcement": announcement}
         if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
@@ -1463,22 +1475,22 @@
         if publishToGlobal: data["publishToGlobal"] = 0
         if not publishToGlobal: data["publishToGlobal"] = 1
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
-                data = dumps({"alertOption": 2, "timestamp": int(timestamp() * 1000)})
+                data = dumps({"alertOption": 2, "timestamp": inttime()})
                 
                 response = await self.session.post(f"/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.additional_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
             if not doNotDisturb:
-                data = dumps({"alertOption": 1, "timestamp": int(timestamp() * 1000)})
+                data = dumps({"alertOption": 1, "timestamp": inttime()})
                 
                 response = await self.session.post(f"/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.additional_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
@@ -1488,22 +1500,22 @@
 
             if not pinChat:
                 response = await self.session.post(f"/g/s/chat/thread/{chatId}/unpin", data=data, headers=self.additional_headers())
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
         if backgroundImage is not None:
-            data = dumps({"media": [100, backgroundImage, None], "timestamp": int(timestamp() * 1000)})
+            data = dumps({"media": [100, backgroundImage, None], "timestamp": inttime()})
             
             response = await self.session.post(f"/g/s/chat/thread/{chatId}/member/{self.userId}/background", data=data, headers=self.additional_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response))
             else: res.append(response.status_code)
 
         if coHosts is not None:
-            data = dumps({"uidList": coHosts, "timestamp": int(timestamp() * 1000)})
+            data = dumps({"uidList": coHosts, "timestamp": inttime()})
             
             response = await self.session.post(f"/g/s/chat/thread/{chatId}/co-host", data=data, headers=self.additional_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response))
             else: res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
@@ -1568,20 +1580,20 @@
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     async def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
         url = None
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+        if transactionId is None: transactionId = str_uuid4()
 
         data = {
             "coins": coins,
             "tippingContext": {"transactionId": transactionId},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if blogId is not None: url = f"/g/s/blog/{blogId}/tipping"
         if chatId is not None: url = f"/g/s/chat/thread/{chatId}/tipping"
         if objectId is not None:
             data["objectId"] = objectId
             data["objectType"] = 2
@@ -1605,18 +1617,22 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str):
-            response = await self.session.post(f"/g/s/user-profile/{userId}/member", headers=self.additional_headers())
+            # looks like not working
+            # response = await self.session.post(f"/g/s/user-profile/{userId}/member", headers=self.additional_headers())
+            data = dumps({"targetUidList": [userId], "timestamp": inttime()})
+            
+            response = await self.session.post(f"/g/s/user-profile/{self.userId}/joined", headers=self.additional_headers(data=data), data=data)
 
         elif isinstance(userId, list):
-            data = dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
+            data = dumps({"targetUidList": userId, "timestamp": inttime()})
             
             response = await self.session.post(f"/g/s/user-profile/{self.userId}/joined", headers=self.additional_headers(data=data), data=data)
 
         else: raise exceptions.WrongType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -1686,15 +1702,15 @@
             - **invitationId** : ID of the Invitation Code.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
         if invitationId: data["invitationId"] = invitationId
 
         data = dumps(data)
         response = await self.session.post(f"/x{comId}/s/community/join", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1709,15 +1725,15 @@
             - **message** : Message to be sent.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = dumps({"message": message, "timestamp": int(timestamp() * 1000)})
+        data = dumps({"message": message, "timestamp": inttime()})
         response = await self.session.post(f"/x{comId}/s/community/membership-request", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     async def leave_community(self, comId: str):
@@ -1756,15 +1772,15 @@
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = dumps({
             "objectId": comId,
             "objectType": 16,
             "flagType": flagType,
             "message": reason,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if isGuest: flg = "g-flag"
         else: flg = "flag"
         
         response = await self.session.post(f"/x{comId}/s/{flg}", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
@@ -1791,15 +1807,15 @@
         """
         data = {
             "address": None,
             "latitude": 0,
             "longitude": 0,
             "mediaList": None,
             "eventSource": "UserProfileView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if nickname: data["nickname"] = nickname
         if icon: data["icon"] = self.upload_media(icon, "image")
         if content: data["content"] = content
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
@@ -1822,15 +1838,15 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if not isAnonymous: data["privacyMode"] = 1
         if isAnonymous: data["privacyMode"] = 2
         if not getNotifications: data["notificationStatus"] = 2
         if getNotifications: data["privacyMode"] = 1
 
         data = dumps(data)
@@ -1848,15 +1864,15 @@
             - **aminoId** : Amino ID of the Account.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = dumps({"aminoId": aminoId, "timestamp": int(timestamp() * 1000)})
+        data = dumps({"aminoId": aminoId, "timestamp": inttime()})
         response = await self.session.post(f"/g/s/account/change-amino-id", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     async def get_linked_communities(self, userId: str):
@@ -1903,15 +1919,15 @@
             - **comIds** : IDS of the Communities.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = dumps({"ndcIds": comIds, "timestamp": int(timestamp() * 1000)})
+        data = dumps({"ndcIds": comIds, "timestamp": inttime()})
         response = await self.session.post(f"/g/s/user-profile/{self.userId}/linked-community/reorder", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     async def add_linked_community(self, comId: str):
@@ -1968,15 +1984,15 @@
         """
         if message is None: raise exceptions.MessageNeeded
 
         data = {
             "content": message,
             "stickerId": None,
             "type": 0,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if replyTo: data["respondTo"] = replyTo
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = dumps(data)
@@ -2037,15 +2053,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if blogId:
             if isinstance(blogId, str):
                 data["eventSource"] = "UserProfileView"
                 data = dumps(data)
                 
@@ -2107,15 +2123,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = dumps(data)
             
             response = await self.session.post(f"/g/s/user-profile/{userId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.additional_headers(data=data), data=data)
@@ -2292,15 +2308,15 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "objectId": objectId,
             "targetCode": 1,
             "objectType": objectType,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         if comId: response = await self.session.post(f"/g/s-x{comId}/link-resolution", headers=self.additional_headers(data=data), data=data)
         else: response = await self.session.post(f"/g/s/link-resolution", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2432,15 +2448,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "adsLevel": level,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/wallet/ads/config", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -2451,19 +2467,19 @@
             "objectType": 114,
             "v": 1,
             "paymentContext":
             {
                 "discountStatus": 0,
                 "isAutoRenew": isAutoRenew
             },
-            "timestamp": timestamp()
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/g/s/store/purchase", headers=self.additional_headers(data=data), data=data)
-        if response.status_code != 200: return exceptions.CheckException(loads(response.text()))
+        if response.status_code != 200: return exceptions.CheckException(response.json())
         else: return response.status_code
 
     async def get_public_communities(self, language: str = "en", size: int = 25):
         """
         Get public communites
 
         **Parameters**
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/socket.py` & `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 import ssl
 import websocket
 from time import sleep
 from random import randint
 from json import loads, dumps
-from time import time as timestamp
 from datetime import datetime as dt
 
 from threading import Thread
 from sys import _getframe as getframe
 
 from ..lib import objects, helpers
-from ..lib.helpers import gen_deviceId
+from ..lib.helpers import gen_deviceId, inttime
 
 class SocketHandler:
     '''
         Sockets needs rewrite. Really.
 
         It's hard to add new features or support it, because code is mess of useless functions and things.
         It's LITTERALY a digital spaghetti that will poison you instead of healing you.
@@ -103,15 +102,15 @@
     def run_amino_socket(self):
         try:
             if self.client.sid is None:
                 return
 
             device = gen_deviceId() if self.client.autoDevice else self.client.device_id
 
-            final = f"{device}|{int(timestamp() * 1000)}"
+            final = f"{device}|{inttime()}"
 
             self.headers = {
                 "Accept-Encoding": "gzip, deflate, br",
                 "Connection": "Upgrade",
                 "AUID": self.client.userId,
                 "NDCAUTH": f"sid={self.client.sid}",
                 "NDCLANG": "en",
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/asyncfixfix/sub_client.py` & `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/sub_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,16 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
-from os import urandom
-from time import timezone
-from binascii import hexlify
-from base64 import b64encode
-from uuid import UUID, uuid4
-from json import loads, dumps
+from json import dumps
 from typing import BinaryIO, Union
-from time import time as timestamp
 
 from .client import Client
 from ..lib import exceptions, headers, objects
-from ..lib.helpers import gen_deviceId, json_minify
-
-class VCHeaders:
-    def __init__(self, data = None):
-        vc_headers = {
-            "Accept-Language": "en-US",
-            "Content-Type": "application/json",
-            "User-Agent": "Amino/45725 CFNetwork/1126 Darwin/19.5.0",  # Closest server (this one for me)
-            "Host": "rt.applovin.com",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Connection": "Keep-Alive",
-            "Accept": "*/*"
-        }
-
-        if data: vc_headers["Content-Length"] = str(len(data))
-        self.vc_headers = vc_headers
-
+from ..lib.helpers import gen_deviceId, json_minify, str_uuid4, inttime, clientrefid, b64_to_bytes, LOCAL_TIMEZONE
 
 class SubClient(Client):
     def __init__(
         self, mainClient: Client,
         comId: str = None, aminoId: str = None, *,
         deviceId: str = None, autoDevice: bool | None = None, proxies: dict = None,
         api_library: objects.APILibraries | None = None
@@ -90,15 +68,15 @@
             return exceptions.CheckException(response)
         else: return objects.InviteCodeList(response.json()["communityInvitationList"]).InviteCodeList
 
     async def generate_invite_code(self, duration: int = 0, force: bool = True) -> objects.InviteCode:
         data = dumps({
             "duration": duration,
             "force": force,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/g/s-x{self.comId}/community/invitation", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.InviteCode(response.json()["communityInvitation"]).InviteCode
 
@@ -131,15 +109,15 @@
             "content": content,
             "title": title,
             "mediaList": mediaList,
             "extensions": extensions,
             "latitude": 0,
             "longitude": 0,
             "eventSource": "GlobalComposeMenu",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
 
         data = dumps(data)
@@ -156,15 +134,15 @@
             mediaList.append([100, await self.upload_media(image, "image"), None])
 
         data = {
             "label": title,
             "content": content,
             "mediaList": mediaList,
             "eventSource": "GlobalComposeMenu",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         data = dumps(data)
@@ -182,15 +160,15 @@
 
         data = {
             "address": None,
             "mediaList": mediaList,
             "latitude": 0,
             "longitude": 0,
             "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if title: data["title"] = title
         if content: data["content"] = content
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
@@ -219,60 +197,60 @@
         else: raise exceptions.SpecifyType()
 
         data = dumps({
             "content": content,
             "refObjectId": refObjectId,
             "refObjectType": refObjectType,
             "type": 2,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/blog", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def check_in(self, tz: int = -timezone // 1000) -> int:
+    async def check_in(self, tz: int = LOCAL_TIMEZONE) -> int:
         data = dumps({
             "timezone": tz,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/check-in", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def repair_check_in(self, method: int = 0) -> int:
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
         if method == 0: data["repairMethod"] = "1"  # Coins
         if method == 1: data["repairMethod"] = "2"  # Amino+
 
         data = dumps(data)
         
         response = await self.session.post(f"/x{self.comId}/s/check-in/repair", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def lottery(self, tz: int = -timezone // 1000) -> objects.LotteryLog:
+    async def lottery(self, tz: int = LOCAL_TIMEZONE) -> objects.LotteryLog:
         data = dumps({
             "timezone": tz,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/check-in/lottery", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.LotteryLog(response.json()["lotteryLog"]).LotteryLog
 
     async def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None) -> int:
         mediaList = []
 
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if captionList is not None:
             for image, caption in zip(imageList, captionList):
                 mediaList.append([100, await self.upload_media(image, "image"), caption])
 
         else:
             if imageList is not None:
@@ -305,28 +283,28 @@
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def vote_poll(self, blogId: str, optionId: str) -> int:
         data = dumps({
             "value": 1,
             "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/blog/{blogId}/poll/option/{optionId}/vote", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def comment(self, message: str, userId: str = None, blogId: str = None, wikiId: str = None, replyTo: str = None, isGuest: bool = False) -> int:
         data = {
             "content": message,
             "stickerId": None,
             "type": 0,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if replyTo: data["respondTo"] = replyTo
 
         if isGuest: comType = "g-comment"
         else: comType = "comment"
 
@@ -374,15 +352,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if blogId:
             if isinstance(blogId, str):
                 data["eventSource"] = "UserProfileView"
                 data = dumps(data)
                 
@@ -415,15 +393,15 @@
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def like_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None) -> int:
         data = {
             "value": 1,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = dumps(data)
             
             response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.additional_headers(data=data), data=data)
@@ -455,27 +433,27 @@
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def upvote_comment(self, blogId: str, commentId: str):
         data = dumps({
             "value": 1,
             "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def downvote_comment(self, blogId: str, commentId: str):
         data = dumps({
             "value": -1,
             "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=-1", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -488,23 +466,23 @@
     async def reply_wall(self, userId: str, commentId: str, message: str):
         data = dumps({
             "content": message,
             "stackedId": None,
             "respondTo": commentId,
             "type": 0,
             "eventSource": "UserProfileView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/comment", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None, timestamp: int = int(timestamp() * 1000)): 
+    async def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = LOCAL_TIMEZONE, timers: list = None, timestamp: int = inttime()): 
         data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "timestamp": timestamp, "optInAdsFlags": optInAdsFlags, "timezone": tz} 
         if timers: data["userActiveTimeChunkList"] = timers 
         data = json_minify(dumps(data))  
         
         response = await self.session.post(f"/x{self.comId}/s/community/stats/user-active-time", headers=self.additional_headers(data=data), data=data) 
         if response.status_code != 200: 
             return exceptions.CheckException(response) 
@@ -514,29 +492,22 @@
         if "on" in status.lower(): status = 1
         elif "off" in status.lower(): status = 2
         else: raise exceptions.WrongType(status)
 
         data = dumps({
             "onlineStatus": status,
             "duration": 86400,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/user-profile/{self.profile.userId}/online-status", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
-
-    # TODO : Finish this
-    async def watch_ad(self):
-        response = await self.session.post(f"/g/s/wallet/ads/video/start", headers=self.additional_headers())
-        if response.status_code != 200: 
-            return exceptions.CheckException(response)
-        else: return response.status_code
-
+        
     async def check_notifications(self):
         response = await self.session.post(f"/x{self.comId}/s/notification/checked", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def delete_notification(self, notificationId: str):
@@ -557,15 +528,15 @@
         else: raise exceptions.WrongType(type(userId))
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if isGlobal is True: data["type"] = 2; data["eventSource"] = "GlobalComposeMenu"
         else: data["type"] = 0
 
         if publishToGlobal is True: data["publishToGlobal"] = 1
         else: data["publishToGlobal"] = 0
@@ -580,15 +551,15 @@
     async def invite_to_chat(self, userId: Union[str, list], chatId: str):
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = dumps({
             "uids": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/invite", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -596,20 +567,20 @@
         response = await self.session.post(f"/x{self.comId}/s/user-group/quick-access/{userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
         url = None
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+        if transactionId is None: transactionId = str_uuid4()
 
         data = {
             "coins": coins,
             "tippingContext": {"transactionId": transactionId},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if blogId is not None: url = f"/x{self.comId}/s/blog/{blogId}/tipping"
         if chatId is not None: url = f"/x{self.comId}/s/chat/thread/{chatId}/tipping"
         if objectId is not None:
             data["objectId"] = objectId
             data["objectType"] = 2
@@ -639,18 +610,22 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str):
-            response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/member", headers=self.additional_headers())
+            # looks like not working
+            # response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/member", headers=self.additional_headers())
+            data = dumps({"targetUidList": [userId], "timestamp": inttime()})
+            
+            response = await self.session.post(f"/x{self.comId}/s/user-profile/{self.profile.userId}/joined", headers=self.additional_headers(data=data), data=data)
 
         elif isinstance(userId, list):
-            data = dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
+            data = dumps({"targetUidList": userId, "timestamp": inttime()})
             
             response = await self.session.post(f"/x{self.comId}/s/user-profile/{self.profile.userId}/joined", headers=self.additional_headers(data=data), data=data)
 
         else: raise exceptions.WrongType(type(userId))
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -743,15 +718,15 @@
         """
         if reason is None: raise exceptions.ReasonNeeded()
         if flagType is None: raise exceptions.FlagTypeNeeded()
 
         data = {
             "flagType": flagType,
             "message": reason,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["objectId"] = userId
             data["objectType"] = 0
 
         elif blogId:
@@ -794,76 +769,87 @@
             - **fileType** : Type of the file.
                 - ``audio``, ``image``, ``gif``
             - **messageType** : Type of the Message.
             - **mentionUserIds** : List of User IDS to mention. '@' needed in the Message.
             - **replyTo** : Message ID to reply to.
             - **stickerId** : Sticker ID to be sent.
             - **embedType** : Type of the Embed. Can be aminofixfix.lib.objects.EmbedTypes only. By default it's LinkSnippet one.
-            - **embedLink** : Link of the Embed.
-            - **embedImage** : Image of the Embed. Required to send Embed.
-            - **embedId** : ID of the Embed. Works only in AttachedObject Embeds.
-            - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds.
-            - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds.
-            - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds.
+            - **embedLink** : Link of the Embed. Can be only "ndc://" link if its AttachedObject.
+            - **embedImage** : Image of the Embed. Required to send Embed, if its LinkSnippet. Can be only 1024x1024 max. Can be string to existing image uploaded to Amino or it can be opened (not readed) file.
+            - **embedId** : ID of the Embed. Works only in AttachedObject Embeds. It can be any ID, just gen it using str_uuid4().
+            - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds. Just look what values AttachedObjectTypes enum contains.
+            - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds. Can be empty.
+            - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds. Can be empty.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if message is not None and file is None:
             message = message.replace("<$", "‎‏").replace("$>", "‬‭")
 
         mentions = []
         if mentionUserIds:
             mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
 
-        if not isinstance(embedImage, BinaryIO):
-            embedType = None
+        if embedImage and not isinstance(embedImage, str):
+            try: readEmbed = embedImage.read()
+            except: embedType = None
 
         if embedType == objects.EmbedTypes.LINK_SNIPPET:
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "extensions": {
                     "linkSnippetList": [{
                         "link": embedLink,
                         "mediaType": 100,
-                        "mediaUploadValue": b64encode(embedImage.read()).decode(),
+                        "mediaUploadValue": b64_to_bytes(readEmbed),
                         "mediaUploadValueContentType": "image/png"
                     }],
                     "mentionedArray": mentions
                 },
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
         elif embedType == objects.EmbedTypes.ATTACHED_OBJECT:
+            try: embedObjectType.value
+            except: raise Exception("You SHOULD pass AttachedEmbedTypes.")
+
+            if isinstance(embedImage, str):
+                image = [[100, embedImage, None]]
+            elif embedImage:
+                image = [[100, await self.upload_media(embedImage, "image"), None]]
+            else:
+                image = None
+
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "attachedObject": {
                     "objectId": embedId,
-                    "objectType": embedObjectType,
+                    "objectType": embedObjectType.value,
                     "link": embedLink,
                     "title": embedTitle,
                     "content": embedContent,
-                    "mediaList": [[100, await self.upload_media(embedImage, "image"), None]]
+                    "mediaList": image
                 },
                 "extensions": {"mentionedArray": mentions},
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
         else:
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "extensions": {"mentionedArray": mentions},
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
 
         if replyTo: data["replyMessageId"] = replyTo
 
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
@@ -883,37 +869,37 @@
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
             else: raise exceptions.SpecifyType(fileType)
 
-            data["mediaUploadValue"] = b64encode(file.read()).decode()
+            data["mediaUploadValue"] = b64_to_bytes(file.read())
 
         data = dumps(data)
 
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def full_embed(self, link: str, image: BinaryIO, message: str, chatId: str):
         data = {
-        "type": 0,
-        "content": message,
-        "extensions": {
-            "linkSnippetList": [{
-                "link": link,
-                "mediaType": 100,
-                "mediaUploadValue": b64encode(image.read()).decode(),
-                "mediaUploadValueContentType": "image/png"
-            }]
-        },
-            "clientRefId": int(timestamp() / 10 % 100000000),
-            "timestamp": int(timestamp() * 1000),
+            "type": 0,
+            "content": message,
+            "extensions": {
+                "linkSnippetList": [{
+                    "link": link,
+                    "mediaType": 100,
+                    "mediaUploadValue": b64_to_bytes(image.read()),
+                    "mediaUploadValueContentType": "image/png"
+                }]
+            },
+            "clientRefId": clientrefid(),
+            "timestamp": inttime(),
             "attachedObject": None
         }
         
         data = dumps(data)
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
@@ -932,15 +918,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "adminOpName": 102,
             # "adminOpNote": {"content": reason},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
         if asStaff and reason:
             data["adminOpNote"] = {"content": reason}
 
         data = dumps(data)
         
         if not asStaff: response = await self.session.delete(f"/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
@@ -960,15 +946,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "messageId": messageId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -995,15 +981,15 @@
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if announcement: data["extensions"] = {"announcement": announcement}
         if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
@@ -1012,22 +998,22 @@
         if publishToGlobal: data["publishToGlobal"] = 0
         if not publishToGlobal: data["publishToGlobal"] = 1
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
-                data = dumps({"alertOption": 2, "timestamp": int(timestamp() * 1000)})
+                data = dumps({"alertOption": 2, "timestamp": inttime()})
                 
                 response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.additional_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
             if not doNotDisturb:
-                data = dumps({"alertOption": 1, "timestamp": int(timestamp() * 1000)})
+                data = dumps({"alertOption": 1, "timestamp": inttime()})
                 
                 response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.additional_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
@@ -1037,22 +1023,22 @@
 
             if not pinChat:
                 response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/unpin", data=data, headers=self.additional_headers())
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
         if backgroundImage is not None:
-            data = dumps({"media": [100, backgroundImage, None], "timestamp": int(timestamp() * 1000)})
+            data = dumps({"media": [100, backgroundImage, None], "timestamp": inttime()})
             
             response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/background", data=data, headers=self.additional_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response))
             else: res.append(response.status_code)
 
         if coHosts is not None:
-            data = dumps({"uidList": coHosts, "timestamp": int(timestamp() * 1000)})
+            data = dumps({"uidList": coHosts, "timestamp": inttime()})
             
             response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/co-host", data=data, headers=self.additional_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response))
             else: res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
@@ -1094,15 +1080,15 @@
         else: res.append(response.status_code)
 
         return res
 
     async def transfer_host(self, chatId: str, userIds: list):
         data = dumps({
             "uidList": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1176,22 +1162,22 @@
         """
         response = await self.session.delete(f"/x{self.comId}/s/chat/thread/{chatId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
         
     async def subscribe(self, userId: str, autoRenew: str = False, transactionId: str = None):
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+        if transactionId is None: transactionId = str_uuid4()
 
         data = dumps({
             "paymentContext": {
                 "transactionId": transactionId,
                 "isAutoRenew": autoRenew
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/influencer/{userId}/subscribe", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1201,38 +1187,36 @@
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def play_quiz_raw(self, quizId: str, quizAnswerList: list, quizMode: int = 0):
         data = dumps({
             "mode": quizMode,
             "quizAnswerList": quizAnswerList,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def play_quiz(self, quizId: str, questionIdsList: list, answerIdsList: list, quizMode: int = 0):
         quizAnswerList = []
 
         for question, answer in zip(questionIdsList, answerIdsList):
-            part = dumps({
+            quizAnswerList.append({
                 "optIdList": [answer],
                 "quizQuestionId": question,
                 "timeSpent": 0.0
             })
 
-            quizAnswerList.append(loads(part))
-
         data = dumps({
             "mode": quizMode,
             "quizAnswerList": quizAnswerList,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1240,15 +1224,15 @@
         """Voice Chat Join Permissions
         1 - Open to Everyone
         2 - Approval Required
         3 - Invite Only
         """
         data = dumps({
             "vvChatJoinType": permission,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1359,15 +1343,15 @@
         """
         response = await self.session.get(f"/x{self.comId}/s/user-profile/{userId}/visitors?start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.VisitorsList(response.json()).VisitorsList
 
     async def get_user_checkins(self, userId: str):
-        response = await self.session.get(f"/x{self.comId}/s/check-in/stats/{userId}?timezone={-timezone // 1000}", headers=self.additional_headers())
+        response = await self.session.get(f"/x{self.comId}/s/check-in/stats/{userId}?timezone={LOCAL_TIMEZONE}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserCheckIns(response.json()).UserCheckIns
 
     async def get_user_blogs(self, userId: str, start: int = 0, size: int = 25):
         response = await self.session.get(f"/x{self.comId}/s/blog?type=user&q={userId}&start={start}&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
@@ -1765,30 +1749,39 @@
         else: response = await self.session.get(f"/x{self.comId}/s/admin/operation?pagingType=t&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.AdminLogList(response.json()["adminLogList"]).AdminLogList
 
     async def feature(self, time: int, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
         if chatId:
-            if time == 1: time = 3600
-            if time == 1: time = 7200
-            if time == 1: time = 10800
+            if isinstance(time, int):
+                if time == 1: inttime = 3600
+                elif time == 2: inttime = 7200
+                elif time == 3: inttime = 10800
+                else: raise exceptions.WrongType(time)
+            else:
+                try: inttime = time.value
+                except: raise exceptions.WrongType(time)
 
         else:
-            if time == 1: time = 86400
-            elif time == 2: time = 172800
-            elif time == 3: time = 259200
-            else: raise exceptions.WrongType(time)
+            if isinstance(time, int):
+                if time == 1: inttime = 86400
+                elif time == 2: inttime = 172800
+                elif time == 3: inttime = 259200
+                else: raise exceptions.WrongType(time)
+            else:
+                try: inttime = time.value
+                except: raise exceptions.WrongType(time)
 
         data = {
             "adminOpName": 114,
             "adminOpValue": {
-                "featuredDuration": time
+                "featuredDuration": inttime
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["adminOpValue"] = {"featuredType": 4}
             data = dumps(data)
             response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
 
@@ -1812,15 +1805,15 @@
             return exceptions.CheckException(response)
         else: return response.json()
 
     async def unfeature(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
         data = {
             "adminOpName": 114,
             "adminOpValue": {},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["adminOpValue"] = {"featuredType": 0}
             data = dumps(data)
             response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
 
@@ -1845,15 +1838,15 @@
         else: return response.json()
 
     async def hide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
         data = {
             "adminOpNote": {
                 "content": reason
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["adminOpName"] = 18
             data = dumps(data)
             response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
 
@@ -1893,15 +1886,15 @@
         else: return response.json()
 
     async def unhide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
         data = {
             "adminOpNote": {
                 "content": reason
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["adminOpName"] = 19
             data = dumps(data)
             response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
 
@@ -1946,15 +1939,15 @@
             tlt.append({"title": titles, "color": colors})
 
         data = dumps({
             "adminOpName": 207,
             "adminOpValue": {
                 "titles": tlt
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -1967,82 +1960,83 @@
             "attachedObject": {
                 "objectId": userId,
                 "objectType": 0
             },
             "penaltyType": 0,
             "adminOpNote": {},
             "noticeType": 7,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/notice", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     # TODO : List all strike texts
     async def strike(self, userId: str, time: int, title: str = None, reason: str = None):
         if time == 1: time = 86400
         elif time == 2: time = 10800
         elif time == 3: time = 21600
         elif time == 4: time = 43200
         elif time == 5: time = 86400
+        elif time == 6: time = 259200
         else: raise exceptions.WrongType(time)
 
         data = dumps({
             "uid": userId,
             "title": title,
             "content": reason,
             "attachedObject": {
                 "objectId": userId,
                 "objectType": 0
             },
             "penaltyType": 1,
             "penaltyValue": time,
             "adminOpNote": {},
             "noticeType": 4,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/notice", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     async def ban(self, userId: str, reason: str, banType: int = None):
         data = dumps({
             "reasonType": banType,
             "note": {
                 "content": reason
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/ban", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     async def unban(self, userId: str, reason: str):
         data = dumps({
             "note": {
                 "content": reason
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/user-profile/{userId}/unban", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
     async def reorder_featured_users(self, userIds: list):
         data = dumps({
             "uidList": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/user-profile/featured/reorder", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -2108,15 +2102,15 @@
         return self.send(dumps(data))
 
     # Provided by "spectrum#4691"
     async def purchase(self, objectId: str, objectType: int, aminoPlus: bool = True, autoRenew: bool = False):
         data = {'objectId': objectId,
                 'objectType': objectType,
                 'v': 1,
-                "timestamp": int(timestamp() * 1000)}
+                "timestamp": inttime()}
 
         if aminoPlus: data['paymentContext'] = {'discountStatus': 1, 'discountValue': 1, 'isAutoRenew': autoRenew}
         else: data['paymentContext'] = {'discountStatus': 0, 'discountValue': 1, 'isAutoRenew': autoRenew}
 
         data = dumps(data)
         response = await self.session.post(f"/x{self.comId}/s/store/purchase", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
@@ -2137,15 +2131,15 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
 
         """
 
         data = {"frameId": avatarId,
                 "applyToAll": 0,
-                "timestamp": int(timestamp() * 1000)}
+                "timestamp": inttime()}
 
         if applyToAll: data["applyToAll"] = 1
 
         data = dumps(data)
         response = await self.session.post(f"/x{self.comId}/s/avatar-frame/apply", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -2175,64 +2169,64 @@
         else: return response.status_code
 
     async def add_poll_option(self, blogId: str, question: str):
         data = dumps({
             "mediaList": None,
             "title": question,
             "type": 0,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/blog/{blogId}/poll/option", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def create_wiki_category(self, title: str, parentCategoryId: str, content: str = None):
         data = dumps({
             "content": content,
             "icon": None,
             "label": title,
             "mediaList": None,
             "parentCategoryId": parentCategoryId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/item-category", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def create_shared_folder(self,title: str):
         data = dumps({
                 "title":title,
-                "timestamp":int(timestamp() * 1000)
+                "timestamp":inttime()
             })
         response = await self.session.post(f"/x{self.comId}/s/shared-folder/folders", headers=self.additional_headers(data=data),data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def submit_to_wiki(self, wikiId: str, message: str):
         data = dumps({
             "message": message,
             "itemId": wikiId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/knowledge-base-request", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     async def accept_wiki_request(self, requestId: str, destinationCategoryIdList: list):
         data = dumps({
             "destinationCategoryIdList": destinationCategoryIdList,
             "actionType": "create",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = await self.session.post(f"/x{self.comId}/s/knowledge-base-request/{requestId}/approve", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -2257,15 +2251,15 @@
         else: return objects.LiveLayer(response.json()["liveLayerList"]).LiveLayer
 
     async def apply_bubble(self, bubbleId: str, chatId: str, applyToAll: bool = False):
         data = {
             "applyToAll": 0,
             "bubbleId": bubbleId,
             "threadId": chatId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if applyToAll is True:
             data["applyToAll"] = 1
 
         data = dumps(data)
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/apply-bubble", headers=self.additional_headers(data=data), data=data)
@@ -2279,30 +2273,30 @@
 
             chatId: str
             message: str
             videoFile: BinaryIO [open(file, "rb")]
             imageFile: BinaryIO [open(file, "rb")]
             mediaUhqEnabled: bool = False
         """
-        i = str(uuid4()).upper()
+        i = str_uuid4().upper()
         cover = f"{i}_thumb.jpg"
         video = f"{i}.mp4"
         
         data = dumps({
-            "clientRefId": int(timestamp() / 10 % 1000000000),
+            "clientRefId": clientrefid(),
             "content": message,
             "mediaType": 123,
             "videoUpload":
             {
                 "contentType": "video/mp4",
                 "cover": cover,
                 "video": video
             },
             "type": 4,
-            "timestamp": int(timestamp() * 1000),
+            "timestamp": inttime(),
             "mediaUhqEnabled": mediaUhqEnabled,
             "extensions": {}    
         })
 
         files = {
             video: (video, videoFile.read(), 'video/mp4'),
             cover: (cover, imageFile.read(), 'application/octet-stream'),
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/client.py` & `amino.fix.fix-1.0.7b1/aminofixfix/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
-from uuid import UUID
-from os import urandom
-from base64 import b64encode
+from time import sleep
+from json import dumps
+from typing import BinaryIO
 from threading import Thread
-from binascii import hexlify
-from json import loads, dumps
-from time import timezone, sleep
-from typing import BinaryIO, Union
-from time import time as timestamp
 from httpx import Client as HttpxClient
 from httpx import Timeout as TimeoutConfig
-from locale import getdefaultlocale as locale
 
-from .lib.helpers import gen_deviceId
 from .lib.facades import RequestsClient
 from .socket import Callbacks, SocketHandler
 from .lib import exceptions, headers, objects, helpers
+from .lib.helpers import gen_deviceId, inttime, clientrefid, str_uuid4, bytes_to_b64, LOCAL_TIMEZONE
 
 class Client(Callbacks, SocketHandler):
     """
         Client to work with global in Amino.
         (aminoapps.com)
     """
     def __init__(
@@ -89,19 +83,19 @@
               but you probably want to import `objects` from `aminofixfix.lib`
         """
         self.api = "https://service.aminoapps.com/api/v1"
         self.proxies = proxies
         self.configured = False
         self.authenticated = False
         self.autoDevice = autoDevice
+        self.api_library = api_library
         self.http2_enabled = http2_enabled
         self.socket_enabled = socket_enabled
         self.device_id = deviceId if deviceId else gen_deviceId()
         self.user_agent = userAgent if userAgent else helpers.gen_userAgent()
-        self.api_library = api_library
 
         if disable_timeout:
             self.timeout_settings = TimeoutConfig(None)
         elif isinstance(own_timeout, TimeoutConfig):
             self.timeout_settings = own_timeout
         elif read_timeout or write_timeout or pool_timeout or connect_timeout:
             self.timeout_settings = TimeoutConfig(
@@ -109,56 +103,59 @@
                 write=write_timeout,
                 pool=pool_timeout,
                 connect=connect_timeout
             )
         else:
             self.timeout_settings = TimeoutConfig(default_timeout or 60)
 
-        if self.api_library == objects.APILibraries.HTTPX:
-            self.session = HttpxClient(
+        if self.api_library == objects.APILibraries.AIOHTTP:
+            raise Exception("You cant use aiohttp in sync client. Aiohttp is async library.")
+        elif self.api_library == objects.APILibraries.REQUESTS:
+            self.session = RequestsClient(
                 headers=headers.BASIC_HEADERS,
                 http2=http2_enabled,
                 base_url=self.api,
                 proxies=proxies,
                 timeout=self.timeout_settings
             )
-        elif self.api_library == objects.APILibraries.AIOHTTP:
-            raise Exception("You cant use aiohttp in sync client. Aiohttp is async library.")
-        elif self.api_library == objects.APILibraries.REQUESTS:
-            self.session = RequestsClient(
+        else:
+            self.session = HttpxClient(
                 headers=headers.BASIC_HEADERS,
                 http2=http2_enabled,
                 base_url=self.api,
                 proxies=proxies,
                 timeout=self.timeout_settings
             )
 
-        SocketHandler.__init__(self, self, socket_trace=socket_trace, debug=socketDebugging)
-        Callbacks.__init__(self, self)
+        if self.socket_enabled:
+            SocketHandler.__init__(self, self, socket_trace=socket_trace, debug=socketDebugging)
+            Callbacks.__init__(self, self)
         self.sid = None
         self.json = None
         self.secret = None
         self.userId = None
         self.account: objects.UserProfile = objects.UserProfile(None)
         self.profile: objects.UserProfile = objects.UserProfile(None)
 
         self.stop_loop = False
         self.active_live_chats = []
 
-    def additional_headers(self, data: str = None, content_type: str = None):
+    def additional_headers(self, data: str = None, json: dict = None, content_type: str = None) -> dict[str, str]:
         """
         Function to make additional headers, that API needs.
 
         Accepting:
         - data: str
         - content_type: str
 
         Recieving:
         - object `dict`
         """
+        if json:
+            data = dumps(data)
         return headers.additionals(
             data=data,
             content_type=content_type,
             user_agent=self.user_agent,
             sid=self.sid,
             auid=self.userId,
             deviceId=gen_deviceId() if self.autoDevice else self.device_id
@@ -179,15 +176,15 @@
         if "on" in status.lower(): status = 1
         elif "off" in status.lower(): status = 2
         else: raise exceptions.WrongType(status)
 
         data = dumps({
             "onlineStatus": status,
             "duration": 86400,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/g/s/user-profile/{self.profile.userId}/online-status", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -360,36 +357,37 @@
 
         self.account: objects.UserProfile = self.get_user_info(uId)
         self.profile: objects.UserProfile = self.get_user_info(uId)
 
         if self.socket_enabled:
             self.run_amino_socket()
 
-    def login(self, email: str, password: str):
+    def login(self, email: str, password: str, client_type: int = 100):
         """
         Login into an account.
 
         **Parameters**
             - **email** : Email of the account.
             - **password** : Password of the account.
+            - **client_type**: Type of Client.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "email": email,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
-            "clientType": 300,
+            "clientType": client_type,
             "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/auth/login", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: exceptions.CheckException(response)
         else:
             self.authenticated = True
             self.json = response.json()
@@ -400,35 +398,36 @@
             self.secret = self.json.get("secret")
 
             if self.socket_enabled:
                 self.run_amino_socket()
 
             return response.json()
 
-    def login_phone(self, phoneNumber: str, password: str):
+    def login_phone(self, phoneNumber: str, password: str, client_type: int = 100):
         """
         Login into an account.
 
         **Parameters**
             - **phoneNumber** : Phone number of the account.
             - **password** : Password of the account.
+            - **client_type**: Type of Client.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "phoneNumber": phoneNumber,
             "v": 2,
             "secret": f"0 {password}",
             "deviceID": self.device_id,
-            "clientType": 300,
+            "clientType": client_type,
             "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/auth/login", headers=self.additional_headers(data=data), data=data)
         self.run_amino_socket()
         if response.status_code != 200: exceptions.CheckException(response)
 
         else:
@@ -460,15 +459,15 @@
         """
         data = dumps({
             "v": 2,
             "secret": secret,
             "deviceID": self.device_id,
             "clientType": 100,
             "action": "normal",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/auth/login", headers=self.additional_headers(data=data), data=data)
         self.run_amino_socket()
         if response.status_code != 200: exceptions.CheckException(response)
 
         else:
@@ -519,15 +518,15 @@
                     "code": verificationCode
                 },
                 "type": 1,
                 "identity": email
             },
             "type": 1,
             "identity": email,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })        
 
         response = self.session.post(f"/g/s/auth/register", data=data, headers=self.additional_headers(data=data), timeout=timeout)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()
@@ -545,15 +544,15 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "secret": f"0 {password}",
             "deviceID": self.device_id,
             "email": email,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/account/delete-request/cancel", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -569,15 +568,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "deviceID": self.device_id,
             "clientType": 100,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/auth/logout", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
 
@@ -613,15 +612,15 @@
         else: raise exceptions.SpecifyType()
 
         if age <= 12: raise exceptions.AgeTooLow()
 
         data = dumps({
             "age": age,
             "gender": gender,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/persona/profile/basic", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -641,15 +640,15 @@
         """
         data = dumps({
             "validationContext": {
                 "type": 1,
                 "identity": email,
                 "data": {"code": code}},
             "deviceID": self.device_id,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/auth/check-security-validation", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -768,34 +767,35 @@
 
         response = self.session.post(f"/g/s/auth/reset-password", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
-    def check_device(self, deviceId: str):
+    def check_device(self, deviceId: str, locale: str = "en_US"):
         """
         Check if the Device ID is valid.
 
         **Parameters**
             - **deviceId** : ID of the Device.
+            - **locale** : Locale like "ru_RU", "en_US"
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "deviceID": deviceId,
             "bundleID": "com.narvii.amino.master",
             "clientType": 100,
-            "timezone": -timezone // 1000,
+            "timezone": LOCAL_TIMEZONE,
             "systemPushEnabled": True,
-            "locale": locale()[0],
-            "timestamp": int(timestamp() * 1000)
+            "locale": locale,
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/device", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             self.configured = True; return response.status_code
@@ -826,19 +826,21 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if fileType == "audio":
             t = "audio/aac"
         elif fileType == "image":
             t = "image/jpg"
+        elif fileType == "gif":
+            t = "image/gif"
         else: raise exceptions.SpecifyType(fileType)
 
         data = file.read()
 
-        response = self.session.post(f"/g/s/media/upload", data=data, headers=self.additional_headers(type=t, data=data))
+        response = self.session.post(f"/g/s/media/upload", data=data, headers=self.additional_headers(content_type=t, data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.json()["mediaValue"]
 
     def handle_socket_message(self, data):
         return self.resolve(data)
@@ -907,18 +909,19 @@
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.UserProfile(response.json()["userProfile"]).UserProfile
 
     def watch_ad(self, userId: str = None):
         """
-        Is this funcction even works?
+        Is this function even works?
         """
-        data = dumps(headers.Tapjoy(userId if userId else self.userId).data) 
-        response = self.session.post("https://ads.tapdaq.com/v4/analytics/reward", data=data, headers=headers.Tapjoy().headers)
+
+        data = headers.Tapjoy.Data(userId or self.userId)
+        response = self.session.post("https://ads.tapdaq.com/v4/analytics/reward", data=data, headers=headers.Tapjoy.Headers())
         if response.status_code != 204: return exceptions.CheckException(response)
         else: return response.status_code
 
     def get_chat_threads(self, start: int = 0, size: int = 25):
         """
         List of Chats the account is in.
 
@@ -1008,15 +1011,15 @@
         """
         response = self.session.delete(f"/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
-    def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
+    def start_chat(self, userId: str | list, message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
         """
         Start an Chat with an User or List of Users.
 
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **message** : Starting Message.
             - **title** : Title of Group Chat.
@@ -1034,15 +1037,15 @@
         else: raise exceptions.WrongType()
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if isGlobal is True: data["type"] = 2; data["eventSource"] = "GlobalComposeMenu"
         else: data["type"] = 0
 
         if publishToGlobal is True: data["publishToGlobal"] = 1
         else: data["publishToGlobal"] = 0
@@ -1052,15 +1055,15 @@
 
         response = self.session.post(f"/g/s/chat/thread", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Thread(response.json()["thread"]).Thread
 
-    def invite_to_chat(self, userId: Union[str, list], chatId: str):
+    def invite_to_chat(self, userId: str | list, chatId: str):
         """
         Invite a User or List of Users to a Chat.
 
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **chatId** : ID of the Chat.
 
@@ -1071,15 +1074,15 @@
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType
 
         data = dumps({
             "uids": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/chat/thread/{chatId}/member/invite", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1407,15 +1410,15 @@
         """
         if reason is None: raise exceptions.ReasonNeeded
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
             "message": reason,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["objectId"] = userId
             data["objectType"] = 0
 
         elif blogId:
@@ -1441,16 +1444,21 @@
     def send_message(
             self,
             chatId: str, message: str = None, messageType: int = 0,
             file: BinaryIO = None, fileType: str = None,
             replyTo: str = None, mentionUserIds: list = None,
             stickerId: str = None,
         
-            embedId: str = None, embedObjectType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None,
-            embedType: objects.EmbedTypes = objects.EmbedTypes.LINK_SNIPPET
+            embedId: str = None,
+            embedLink: str = None,
+            embedTitle: str = None,
+            embedContent: str = None,
+            embedImage: BinaryIO = None,
+            embedType: objects.EmbedTypes = None,
+            embedObjectType: objects.AttachedObjectTypes = None
         ):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **message** : Message to be sent
             - **chatId** : ID of the Chat.
@@ -1458,76 +1466,87 @@
             - **fileType** : Type of the file.
                 - ``audio``, ``image``, ``gif``
             - **messageType** : Type of the Message.
             - **mentionUserIds** : List of User IDS to mention. '@' needed in the Message.
             - **replyTo** : Message ID to reply to.
             - **stickerId** : Sticker ID to be sent.
             - **embedType** : Type of the Embed. Can be aminofixfix.lib.objects.EmbedTypes only. By default it's LinkSnippet one.
-            - **embedLink** : Link of the Embed.
-            - **embedImage** : Image of the Embed. Required to send Embed.
-            - **embedId** : ID of the Embed. Works only in AttachedObject Embeds.
-            - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds.
-            - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds.
-            - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds.
+            - **embedLink** : Link of the Embed. Can be only "ndc://" link if its AttachedObject.
+            - **embedImage** : Image of the Embed. Required to send Embed, if its LinkSnippet. Can be only 1024x1024 max. Can be string to existing image uploaded to Amino or it can be opened (not readed) file.
+            - **embedId** : ID of the Embed. Works only in AttachedObject Embeds. It can be any ID, just gen it using str_uuid4().
+            - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds. Just look what values AttachedObjectTypes enum contains.
+            - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds. Can be empty.
+            - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds. Can be empty.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if message is not None and file is None:
             message = message.replace("<$", "‎‏").replace("$>", "‬‭")
 
         mentions = []
         if mentionUserIds:
             mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
 
-        if not isinstance(embedImage, BinaryIO):
-            embedType = None
+        if embedImage and not isinstance(embedImage, str):
+            try: readEmbed = embedImage.read()
+            except: embedType = None
 
         if embedType == objects.EmbedTypes.LINK_SNIPPET:
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "extensions": {
                     "linkSnippetList": [{
                         "link": embedLink,
                         "mediaType": 100,
-                        "mediaUploadValue": b64encode(embedImage.read()).decode(),
+                        "mediaUploadValue": bytes_to_b64(readEmbed),
                         "mediaUploadValueContentType": "image/png"
                     }],
                     "mentionedArray": mentions
                 },
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
         elif embedType == objects.EmbedTypes.ATTACHED_OBJECT:
+            try: embedObjectType.value
+            except: raise Exception("You SHOULD pass AttachedEmbedTypes.")
+
+            if isinstance(embedImage, str):
+                image = [[100, embedImage, None]]
+            elif embedImage:
+                image = [[100, self.upload_media(embedImage, "image"), None]]
+            else:
+                image = None
+
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "attachedObject": {
                     "objectId": embedId,
-                    "objectType": embedObjectType,
+                    "objectType": embedObjectType.value,
                     "link": embedLink,
                     "title": embedTitle,
                     "content": embedContent,
-                    "mediaList": [[100, self.upload_media(embedImage, "image"), None]]
+                    "mediaList": image
                 },
                 "extensions": {"mentionedArray": mentions},
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
         else:
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "extensions": {"mentionedArray": mentions},
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
 
         if replyTo: data["replyMessageId"] = replyTo
 
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
@@ -1547,15 +1566,15 @@
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
             else: raise exceptions.SpecifyType(fileType)
 
-            data["mediaUploadValue"] = b64encode(file.read()).decode()
+            data["mediaUploadValue"] = bytes_to_b64(file.read())
 
         data = dumps(data)
 
         response = self.session.post(f"/g/s/chat/thread/{chatId}/message", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
@@ -1574,15 +1593,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "adminOpName": 102,
             "adminOpNote": {"content": reason},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         data = dumps(data)
         
         if not asStaff: response = self.session.delete(f"/g/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
         else: response = self.session.post(f"/g/s/chat/thread/{chatId}/message/{messageId}/admin", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
@@ -1601,15 +1620,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "messageId": messageId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/g/s/chat/thread/{chatId}/mark-as-read", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -1637,15 +1656,15 @@
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if announcement: data["extensions"] = {"announcement": announcement}
         if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
@@ -1654,22 +1673,22 @@
         if publishToGlobal: data["publishToGlobal"] = 0
         if not publishToGlobal: data["publishToGlobal"] = 1
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
-                data = dumps({"alertOption": 2, "timestamp": int(timestamp() * 1000)})
+                data = dumps({"alertOption": 2, "timestamp": inttime()})
                 
                 response = self.session.post(f"/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.additional_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
             if not doNotDisturb:
-                data = dumps({"alertOption": 1, "timestamp": int(timestamp() * 1000)})
+                data = dumps({"alertOption": 1, "timestamp": inttime()})
                 
                 response = self.session.post(f"/g/s/chat/thread/{chatId}/member/{self.userId}/alert", data=data, headers=self.additional_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
@@ -1679,22 +1698,22 @@
 
             if not pinChat:
                 response = self.session.post(f"/g/s/chat/thread/{chatId}/unpin", data=data, headers=self.additional_headers())
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
         if backgroundImage is not None:
-            data = dumps({"media": [100, backgroundImage, None], "timestamp": int(timestamp() * 1000)})
+            data = dumps({"media": [100, backgroundImage, None], "timestamp": inttime()})
             
             response = self.session.post(f"/g/s/chat/thread/{chatId}/member/{self.userId}/background", data=data, headers=self.additional_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response))
             else: res.append(response.status_code)
 
         if coHosts is not None:
-            data = dumps({"uidList": coHosts, "timestamp": int(timestamp() * 1000)})
+            data = dumps({"uidList": coHosts, "timestamp": inttime()})
             
             response = self.session.post(f"/g/s/chat/thread/{chatId}/co-host", data=data, headers=self.additional_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response))
             else: res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
@@ -1772,20 +1791,20 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         url = None
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+        if transactionId is None: transactionId = str_uuid4()
 
         data = {
             "coins": coins,
             "tippingContext": {"transactionId": transactionId},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if blogId is not None: url = f"/g/s/blog/{blogId}/tipping"
         if chatId is not None: url = f"/g/s/chat/thread/{chatId}/tipping"
         if objectId is not None:
             data["objectId"] = objectId
             data["objectType"] = 2
@@ -1796,31 +1815,36 @@
         data = dumps(data)
         response = self.session.post(url, headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
-    def follow(self, userId: Union[str, list]):
+    def follow(self, userId: str | list):
         """
         Follow an User or Multiple Users.
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str):
-            response = self.session.post(f"/g/s/user-profile/{userId}/member", headers=self.additional_headers())
+            # looks like not working
+            # response = self.session.post(f"/g/s/user-profile/{userId}/member", headers=self.additional_headers())
+            data = dumps({"targetUidList": [userId], "timestamp": inttime()})
+            
+            response = self.session.post(f"/g/s/user-profile/{self.userId}/joined", headers=self.additional_headers(data=data), data=data)
+
 
         elif isinstance(userId, list):
-            data = dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
+            data = dumps({"targetUidList": userId, "timestamp": inttime()})
             
             response = self.session.post(f"/g/s/user-profile/{self.userId}/joined", headers=self.additional_headers(data=data), data=data)
 
         else: raise exceptions.WrongType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -1890,15 +1914,15 @@
             - **invitationId** : ID of the Invitation Code.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
         if invitationId: data["invitationId"] = invitationId
 
         data = dumps(data)
         response = self.session.post(f"/x{comId}/s/community/join", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -1913,15 +1937,15 @@
             - **message** : Message to be sent.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = dumps({"message": message, "timestamp": int(timestamp() * 1000)})
+        data = dumps({"message": message, "timestamp": inttime()})
         response = self.session.post(f"/x{comId}/s/community/membership-request", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     def leave_community(self, comId: str):
@@ -1960,15 +1984,15 @@
         if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = dumps({
             "objectId": comId,
             "objectType": 16,
             "flagType": flagType,
             "message": reason,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         if isGuest: flg = "g-flag"
         else: flg = "flag"
         
         response = self.session.post(f"/x{comId}/s/{flg}", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
@@ -1995,15 +2019,15 @@
         """
         data = {
             "address": None,
             "latitude": 0,
             "longitude": 0,
             "mediaList": None,
             "eventSource": "UserProfileView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if nickname: data["nickname"] = nickname
         if icon: data["icon"] = self.upload_media(icon, "image")
         if content: data["content"] = content
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
@@ -2026,15 +2050,15 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if not isAnonymous: data["privacyMode"] = 1
         if isAnonymous: data["privacyMode"] = 2
         if not getNotifications: data["notificationStatus"] = 2
         if getNotifications: data["privacyMode"] = 1
 
         data = dumps(data)
@@ -2052,15 +2076,15 @@
             - **aminoId** : Amino ID of the Account.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = dumps({"aminoId": aminoId, "timestamp": int(timestamp() * 1000)})
+        data = dumps({"aminoId": aminoId, "timestamp": inttime()})
         response = self.session.post(f"/g/s/account/change-amino-id", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     def get_linked_communities(self, userId: str):
@@ -2107,15 +2131,15 @@
             - **comIds** : IDS of the Communities.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = dumps({"ndcIds": comIds, "timestamp": int(timestamp() * 1000)})
+        data = dumps({"ndcIds": comIds, "timestamp": inttime()})
         response = self.session.post(f"/g/s/user-profile/{self.userId}/linked-community/reorder", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
     def add_linked_community(self, comId: str):
@@ -2172,15 +2196,15 @@
         """
         if message is None: raise exceptions.MessageNeeded
 
         data = {
             "content": message,
             "stickerId": None,
             "type": 0,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if replyTo: data["respondTo"] = replyTo
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = dumps(data)
@@ -2226,30 +2250,30 @@
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
-    def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None):
+    def like_blog(self, blogId: str | list = None, wikiId: str = None):
         """
         Like a Blog, Multiple Blogs or a Wiki.
 
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if blogId:
             if isinstance(blogId, str):
                 data["eventSource"] = "UserProfileView"
                 data = dumps(data)
                 
@@ -2311,15 +2335,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = dumps(data)
             
             response = self.session.post(f"/g/s/user-profile/{userId}/comment/{commentId}/g-vote?cv=1.2&value=1", headers=self.additional_headers(data=data), data=data)
@@ -2496,15 +2520,15 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "objectId": objectId,
             "targetCode": 1,
             "objectType": objectType,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         if comId: response = self.session.post(f"/g/s-x{comId}/link-resolution", headers=self.additional_headers(data=data), data=data)
         else: response = self.session.post(f"/g/s/link-resolution", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
@@ -2672,15 +2696,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         data = dumps({
             "adsLevel": level,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/wallet/ads/config", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
@@ -2706,15 +2730,15 @@
             "objectType": 114,
             "v": 1,
             "paymentContext":
             {
                 "discountStatus": 0,
                 "isAutoRenew": isAutoRenew
             },
-            "timestamp": timestamp()
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/g/s/store/purchase", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: return exceptions.CheckException(response)
         else: return response.status_code
 
     def get_public_communities(self, language: str = "en", size: int = 25):
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/lib/exceptions.py` & `amino.fix.fix-1.0.7b1/aminofixfix/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/aiohttp.py` & `amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/aiohttp.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/requests.py` & `amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/requests.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/lib/facades/unsuccessful_import.py` & `amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/unsuccessful_import.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/lib/headers.py` & `amino.fix.fix-1.0.7b1/aminofixfix/lib/headers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from uuid import uuid4
-from .helpers import signature
+from .helpers import signature, str_uuid4
 
 BASIC_HEADERS = {
     "Accept": "*/*",
     "Accept-Encoding": "gzip, deflate, br",
     "Accept-Language": "en-US,en;q=0.9",
     "Host": "service.aminoapps.com",
     "Connection": "keep-alive",
     "NDCLANG": "en"
 }
 
 def additionals(data = None, user_agent = None, content_type = None, deviceId: str = None, sig: str = None, sid: str = None, auid: str = None):
     headers = {
-        "AUID": auid or str(uuid4())
+        "AUID": auid or str_uuid4()
     }
 
     if user_agent:
         headers['User-Agent'] = user_agent
     if deviceId:
         headers["NDCDEVICEID"] = deviceId
     if data:
@@ -28,29 +27,46 @@
         headers["NDC-MSG-SIG"] = sig
 
     if isinstance(content_type, str) and content_type.lower() == "default":
         pass # letting HTTPX do its job
     elif content_type: 
         headers["Content-Type"] = content_type
     else:
-        headers["Content-Type"] = "application/x-www-form-urlencoded"
+        headers["Content-Type"] = "application/json; charset=utf-8"
 
     return headers
 
 class Tapjoy:
-    def __init__(self, userId: str = None):
-        self.data = {
+    @staticmethod
+    def Headers() -> dict:
+        return {
+            "cookies": "__cfduid=d0c98f07df2594b5f4aad802942cae1f01619569096",
+            "authorization": "Basic NWJiNTM0OWUxYzlkNDQwMDA2NzUwNjgwOmM0ZDJmYmIxLTVlYjItNDM5MC05MDk3LTkxZjlmMjQ5NDI4OA==",
+            "X-Tapdaq-SDK-Version": "android-sdk_7.1.1",
+            "Content-Type": "application/x-www-form-urlencoded",
+            "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 10; Redmi Note 9 Pro Build/QQ3A.200805.001; com.narvii.amino.master/3.4.33585)"
+        }
+
+    @staticmethod
+    def Data(userId: str = None) -> str:
+        data = '{"reward":{"ad_unit_id":"t00_tapjoy_android_master_checkinwallet_rewardedvideo_322","credentials_type":"publisher","custom_json":{"hashed_user_id":"[$UID$]"},"demand_type":"sdk_bidding","event_id":"[$EID$]","network":"tapjoy","placement_tag":"default","reward_name":"Amino Coin","reward_valid":true,"reward_value":2,"shared_id":"4d7cc3d9-8c8a-4036-965c-60c091e90e7b","version_id":"1569147951493","waterfall_id":"4d7cc3d9-8c8a-4036-965c-60c091e90e7b"},"app":{"bundle_id":"com.narvii.amino.master","current_orientation":"portrait","release_version":"3.4.33585","user_agent":"Dalvik\\/2.1.0 (Linux; U; Android 10; G8231 Build\\/41.2.A.0.219; com.narvii.amino.master\\/3.4.33567)"},"device_user":{"country":"US","device":{"architecture":"aarch64","carrier":{"country_code":255,"name":"Vodafone","network_code":0},"is_phone":true,"model":"GT-S5360","model_type":"Samsung","operating_system":"android","operating_system_version":"29","screen_size":{"height":2300,"resolution":2.625,"width":1080}},"do_not_track":false,"idfa":"0c26b7c3-4801-4815-a155-50e0e6c27eeb","ip_address":"","locale":"ru","timezone":{"location":"Asia\\/Seoul","offset":"GMT+02:00"},"volume_enabled":true},"session_id":"7fe1956a-6184-4b59-8682-04ff31e24bc0","date_created": 1633283996}'
+        return data.replace("[$UID$]", userId).replace("[$EID$]", str_uuid4())
+    
+    # Just in case
+    @staticmethod
+    def Data_Legacy(userId: str = None) -> dict:
+        return {
             "reward": {
                 "ad_unit_id": "t00_tapjoy_android_master_checkinwallet_rewardedvideo_322",
                 "credentials_type": "publisher",
                 "custom_json": {
                     "hashed_user_id": userId
                 },
                 "demand_type": "sdk_bidding",
-                "event_id": str(uuid4()),
+                "event_id": str_uuid4(),
                 "network": "tapjoy",
                 "placement_tag": "default",
                 "reward_name": "Amino Coin",
                 "reward_valid": True,
                 "reward_value": 2,
                 "shared_id": "4d7cc3d9-8c8a-4036-965c-60c091e90e7b",
                 "version_id": "1569147951493",
@@ -91,17 +107,20 @@
                     "offset": "GMT+02:00"
                 },
                 "volume_enabled": True
             },
             "session_id": "7fe1956a-6184-4b59-8682-04ff31e24bc0",
             "date_created": 1633283996
         }
-    
-    @property
-    def headers(self):
-        return {
-            "cookies": "__cfduid=d0c98f07df2594b5f4aad802942cae1f01619569096",
-            "authorization": "Basic NWJiNTM0OWUxYzlkNDQwMDA2NzUwNjgwOmM0ZDJmYmIxLTVlYjItNDM5MC05MDk3LTkxZjlmMjQ5NDI4OA==",
-            "X-Tapdaq-SDK-Version": "android-sdk_7.1.1",
-            "Content-Type": "application/x-www-form-urlencoded",
-            "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 10; Redmi Note 9 Pro Build/QQ3A.200805.001; com.narvii.amino.master/3.4.33585)"
-        }
+
+def VCHeaders(data = None) -> dict:
+    headers = {
+        "Accept-Language": "en-US",
+        "Content-Type": "application/json",
+        "User-Agent": "Amino/45725 CFNetwork/1126 Darwin/19.5.0",  # Closest server (this one for me)
+        "Host": "rt.applovin.com",
+        "Accept-Encoding": "gzip, deflate, br",
+        "Connection": "Keep-Alive",
+        "Accept": "*/*"
+    }
+    if data: headers["Content-Length"] = str(len(data))
+    return headers
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/lib/helpers.py` & `amino.fix.fix-1.0.7b1/aminofixfix/lib/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 from base64 import b64decode, b64encode
+from time import timezone as tz_raw
+from time import time as timestamp
 from functools import reduce
 from random import choice
 from typing import Union
 from hashlib import sha1
 from os import urandom
 from json import loads
+from uuid import uuid4
 from hmac import new
 import re
 
-LIBRARY_VERSION = "1.0.6b2"
+LIBRARY_VERSION = "1.0.7b1"
 
 PREFIX = bytes.fromhex("19")
 SIG_KEY = bytes.fromhex("DFA5ED192DDA6E88A12FE12130DC6206B1251E44")
 DEVICE_KEY = bytes.fromhex("E7309ECC0953C6FA60005B2765F99DBBC965C8E9")
 
 IPHONE_IDS = [
     "11,2", "11,4", "11,6", "11,8",
@@ -28,17 +31,26 @@
 IOS_VERSIONS = [
     "14.2", "14.3", "14.4", "14.4.1", "14.4.2", "14.5", "14.5.1", "14.6", "14.7", "14.7.1", "14.8", "14.8.1",
     "15.0", "15.0.1", "15.0.2", "15.1", "15.1.1", "15.2", "15.2.1", "15.3", "15.3.1", "15.4", "15.4.1", "15.5", "15.6", "15.6.1", "15.7", "15.7.1",
     "16.0", "16.0.2", "16.0.3", "16.1", "16.1.1", "16.1.2", "16.2", "16.3", "16.3.1", "16.4", "16.4.1", "16.5", "16.5.1", "16.6", "16.6.1", "16.7", "16.7.1", "16.7.2",
     "17.0", "17.0.1", "17.0.2", "17.0.3", "17.1", "17.1.1", "17.1.2", "17.2", "17.2.1", "17.3", "17.3.1", "17.4"
 ]
 APP_VERSIONS = [
-    "3.22.0", "3.21.0", "3.20.0", "3.19.0", "3.18.0"
+    "3.23.0", "3.22.0", "3.21.0", "3.20.0"
 ]
 
+LOCAL_TIMEZONE = -tz_raw // 1000
+
+def str_uuid4() -> str: return str(uuid4())
+
+def inttime() -> int: return int(timestamp() * 1000)
+def clientrefid() -> int: return int(timestamp() / 10 % 1000000000)
+
+def b64_to_bytes(b64: str) -> str: b64decode(b64).decode()
+def bytes_to_b64(data: bytes) -> str: b64encode(data).decode()
 
 def gen_deviceId(data: bytes = None) -> str:
     identifier = PREFIX + ((data if isinstance(data, bytes) else bytes(data, 'utf-8')) if data else urandom(20))
     return "{}{}".format(identifier.hex(), new(DEVICE_KEY, identifier, sha1).hexdigest()).upper()
 
 def gen_userAgent() -> str:
     return "Apple iPhone{} iOS v{} Main/{}".format(
@@ -57,17 +69,19 @@
 
 def sid_to_uid(SID: str) -> str: return decode_sid(SID)["2"]
 
 def sid_to_ip_address(SID: str) -> str: return decode_sid(SID)["4"]
 
 def json_minify(string, strip_space=True):
     '''
-        Took from: https://github.com/getify/JSON.minify/
+        Took from: https://github.com/getify/JSON.minify/tree/python
+        Library under MIT license.
         
-        I think install library to just minify json is stupid sorry
+        I think install library to just minify json is stupid,
+        so I copied function, sorry.
     '''
     tokenizer = re.compile(r'"|(/\*)|(\*/)|(//)|\n|\r')
     end_slashes_re = re.compile(r'(\\)*$')
 
     in_string = False
     in_multi = False
     in_single = False
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/lib/objects.py` & `amino.fix.fix-1.0.7b1/aminofixfix/lib/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,69 @@
 # Enums
 
 from enum import Enum
 
+class PostFeatureDays(Enum):
+    """
+    Enum, containing all possible day values for post featuring.
+
+    - ONE_DAY (1)
+    - TWO_DAYS (2)
+    - THREE_DAYS (3)
+    """
+    ONE_DAY = 1
+    TWO_DAYS = 2
+    THREE_DAYS = 3
+
+class ChatFeatureDays(Enum):
+    """
+    Enum, containing all possible day values for chat featuring.
+
+    - ONE_HOUR (1)
+    - TWO_HOURS (2)
+    - THREE_HOURS (3)
+    """
+    ONE_DAY = 1
+    TWO_DAYS = 2
+    THREE_DAYS = 3
+
+class UserFeatureDays(Enum):
+    """
+    Enum, containing all possible day values for user featuring.
+
+    - ONE_DAY (1)
+    - TWO_DAYS (2)
+    """
+    ONE_DAY = 1
+    TWO_DAYS = 2
+
 class EmbedTypes(Enum):
     """
     Enum, containing all possible values for Embed.
 
     - LINK_SNIPPET (1)
     - ATTACHED_OBJECT (2)
     """
     LINK_SNIPPET = 1
     ATTACHED_OBJECT = 2
 
+class AttachedObjectTypes(Enum):
+    """
+    Enum, containing all possible values for Embed.
+
+    - PROFILE (0)
+    - POST (1)
+    - WIKI (2)
+    - PUBLIC_CHAT (12)
+    """
+    PROFILE = 0
+    POST = 1
+    WIKI = 2
+    PUBLIC_CHAT = 12
+    
 class APILibraries(Enum):
     """
     Enum, containing all possible values for API libraries.
 
     - HTTPX (1)
     - AIOHTTP (2)
     - REQUESTS (3)
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/socket.py` & `amino.fix.fix-1.0.7b1/aminofixfix/socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 import ssl
 import websocket
 from time import sleep
 from random import randint
 from json import loads, dumps
-from time import time as timestamp
 from datetime import datetime as dt
 
 from threading import Thread
 from sys import _getframe as getframe
 
 from .lib import objects, helpers
-from .lib.helpers import gen_deviceId
+from .lib.helpers import gen_deviceId, inttime
 
 class SocketHandler:
     '''
         Sockets needs rewrite. Really.
 
         It's hard to add new features or support it, because code is mess of useless functions and things.
         It's LITTERALY a digital spaghetti that will poison you instead of healing you.
@@ -103,15 +102,15 @@
     def run_amino_socket(self):
         try:
             if self.client.sid is None:
                 return
 
             device = gen_deviceId() if self.client.autoDevice else self.client.device_id
 
-            final = f"{device}|{int(timestamp() * 1000)}"
+            final = f"{device}|{inttime()}"
 
             self.headers = {
                 "Accept-Encoding": "gzip, deflate, br",
                 "Connection": "Upgrade",
                 "AUID": self.client.userId,
                 "NDCAUTH": f"sid={self.client.sid}",
                 "NDCLANG": "en",
```

### Comparing `amino.fix.fix-1.0.6b2/aminofixfix/sub_client.py` & `amino.fix.fix-1.0.7b1/aminofixfix/sub_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,16 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
-from os import urandom
-from time import timezone
-from binascii import hexlify
-from base64 import b64encode
-from uuid import UUID, uuid4
-from json import loads, dumps
-from typing import BinaryIO, Union
-from time import time as timestamp
+from json import dumps
+from typing import BinaryIO
 
 from .client import Client
 from .lib import exceptions, headers, objects
-from .lib.helpers import gen_deviceId, json_minify
-
-class VCHeaders:
-    def __init__(self, data = None):
-        vc_headers = {
-            "Accept-Language": "en-US",
-            "Content-Type": "application/json",
-            "User-Agent": "Amino/45725 CFNetwork/1126 Darwin/19.5.0",  # Closest server (this one for me)
-            "Host": "rt.applovin.com",
-            "Accept-Encoding": "gzip, deflate, br",
-            "Connection": "Keep-Alive",
-            "Accept": "*/*"
-        }
-
-        if data: vc_headers["Content-Length"] = str(len(data))
-        self.vc_headers = vc_headers
-
+from .lib.helpers import gen_deviceId, json_minify, str_uuid4, inttime, clientrefid, b64_to_bytes, LOCAL_TIMEZONE
 
 class SubClient(Client):
     """
         Client to work with community in Amino.
         (aminoapps.com)
     """
     def __init__(
@@ -140,15 +118,15 @@
         Recieving:
         - object `InviteCode`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "duration": duration,
             "force": force,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/g/s-x{self.comId}/community/invitation", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.InviteCode(response.json()["communityInvitation"]).InviteCode
 
@@ -241,15 +219,15 @@
             "content": content,
             "title": title,
             "mediaList": mediaList,
             "extensions": extensions,
             "latitude": 0,
             "longitude": 0,
             "eventSource": "GlobalComposeMenu",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor and len(backgroundColor) == 7: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
 
         data = dumps(data)
@@ -286,15 +264,15 @@
             mediaList.append([100, self.upload_media(image, "image"), None])
 
         data = {
             "label": title,
             "content": content,
             "mediaList": mediaList,
             "eventSource": "GlobalComposeMenu",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor and len(backgroundColor) == 7: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         data = dumps(data)
@@ -334,15 +312,15 @@
 
         data = {
             "address": None,
             "mediaList": mediaList,
             "latitude": 0,
             "longitude": 0,
             "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if title: data["title"] = title
         if content: data["content"] = content
         if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
@@ -406,37 +384,37 @@
         else: raise exceptions.SpecifyType()
 
         data = dumps({
             "content": content,
             "refObjectId": refObjectId,
             "refObjectType": refObjectType,
             "type": 2,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    def check_in(self, tz: int = -timezone // 1000) -> int:
+    def check_in(self, tz: int = LOCAL_TIMEZONE) -> int:
         """
         Check in community.
 
         Accepting:
         - tz: int
             - better dont touch
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "timezone": tz,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/check-in", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -449,40 +427,40 @@
             - if 0, it will use coins
             - if 1, it will use Amino+ superpower
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
         if method == 0: data["repairMethod"] = "1"  # Coins
         if method == 1: data["repairMethod"] = "2"  # Amino+
 
         data = dumps(data)
         
         response = self.session.post(f"/x{self.comId}/s/check-in/repair", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    def lottery(self, tz: int = -timezone // 1000) -> objects.LotteryLog:
+    def lottery(self, tz: int = LOCAL_TIMEZONE) -> objects.LotteryLog:
         """
         Testing your luck in lottery. Once a day, of course.
 
         Accepting:
         - tz: int 
             - better dont touch
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "timezone": tz,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/check-in/lottery", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.LotteryLog(response.json()["lotteryLog"]).LotteryLog
 
@@ -506,15 +484,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         mediaList = []
 
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if captionList is not None:
             for image, caption in zip(imageList, captionList):
                 mediaList.append([100, self.upload_media(image, "image"), caption])
 
         else:
             if imageList is not None:
@@ -547,15 +525,15 @@
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def vote_poll(self, blogId: str, optionId: str) -> int:
         data = dumps({
             "value": 1,
             "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}/poll/option/{optionId}/vote", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -576,15 +554,15 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "content": message,
             "stickerId": None,
             "type": 0,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if replyTo: data["respondTo"] = replyTo
 
         if isGuest: comType = "g-comment"
         else: comType = "comment"
 
@@ -631,30 +609,30 @@
         elif wikiId: response = self.session.delete(f"/x{self.comId}/s/item/{wikiId}/comment/{commentId}", headers=self.additional_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None) -> int:
+    def like_blog(self, blogId: str | list = None, wikiId: str = None) -> int:
         """
         Like a Blog, Multiple Blogs or a Wiki.
 
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 4,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if blogId:
             if isinstance(blogId, str):
                 data["eventSource"] = "UserProfileView"
                 data = dumps(data)
                 
@@ -713,15 +691,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "value": 1,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["eventSource"] = "UserProfileView"
             data = dumps(data)
             
             response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.additional_headers(data=data), data=data)
@@ -779,15 +757,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "value": 1,
             "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=1", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -803,15 +781,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "value": -1,
             "eventSource": "PostDetailView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}/comment/{commentId}/vote?cv=1.2&value=-1", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -849,23 +827,23 @@
         """
         data = dumps({
             "content": message,
             "stackedId": None,
             "respondTo": commentId,
             "type": 0,
             "eventSource": "UserProfileView",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/comment", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None, timestamp: int = int(timestamp() * 1000)): 
+    def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = LOCAL_TIMEZONE, timers: list = None, timestamp: int = inttime()): 
         """
         Sending mintues to Amino servers.
 
         Hey, is this method used in amino coin generators? And why there is now so tight limits that you can recieve "Too Many Requests" even in app?
 
         **Parameters**
             - **startTime** : Unixtime (int) of start time.
@@ -904,36 +882,22 @@
         if "on" in status.lower(): status = 1
         elif "off" in status.lower(): status = 2
         else: raise exceptions.WrongType(status)
 
         data = dumps({
             "onlineStatus": status,
             "duration": 86400,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/user-profile/{self.profile.userId}/online-status", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    # TODO : Finish this
-    def watch_ad(self):
-        """
-        "Watching" ad.
-
-        Recieving:
-        - object `int` (200)
-        - on exception, some exception from `aminofixfix.lib.exceptions`
-        """
-        response = self.session.post(f"/g/s/wallet/ads/video/start", headers=self.additional_headers())
-        if response.status_code != 200: 
-            return exceptions.CheckException(response)
-        else: return response.status_code
-
     def check_notifications(self):
         """
         Checking notifications as read.
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
@@ -968,15 +932,15 @@
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         response = self.session.delete(f"/x{self.comId}/s/notification", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
+    def start_chat(self, userId: str | list, message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
         """
         Start an Chat with an User or List of Users.
 
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **message** : Starting Message.
             - **title** : Title of Group Chat.
@@ -994,15 +958,15 @@
         else: raise exceptions.WrongType(type(userId))
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if isGlobal is True: data["type"] = 2; data["eventSource"] = "GlobalComposeMenu"
         else: data["type"] = 0
 
         if publishToGlobal is True: data["publishToGlobal"] = 1
         else: data["publishToGlobal"] = 0
@@ -1010,15 +974,15 @@
         data = dumps(data)
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Thread(response.json()["thread"]).Thread
 
-    def invite_to_chat(self, userId: Union[str, list], chatId: str):
+    def invite_to_chat(self, userId: str | list, chatId: str):
         """
         Invite a User or List of Users to a Chat.
 
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **chatId** : ID of the Chat.
 
@@ -1029,15 +993,15 @@
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = dumps({
             "uids": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/invite", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1069,20 +1033,20 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         url = None
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+        if transactionId is None: transactionId = str_uuid4()
 
         data = {
             "coins": coins,
             "tippingContext": {"transactionId": transactionId},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if blogId is not None: url = f"/x{self.comId}/s/blog/{blogId}/tipping"
         if chatId is not None: url = f"/x{self.comId}/s/chat/thread/{chatId}/tipping"
         if objectId is not None:
             data["objectId"] = objectId
             data["objectType"] = 2
@@ -1111,31 +1075,35 @@
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    def follow(self, userId: Union[str, list]):
+    def follow(self, userId: str | list):
         """
         Follow an User or Multiple Users.
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         if isinstance(userId, str):
-            response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/member", headers=self.additional_headers())
+            # looks like not working
+            # response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/member", headers=self.additional_headers())
+            data = dumps({"targetUidList": [userId], "timestamp": inttime()})
+            
+            response = self.session.post(f"/x{self.comId}/s/user-profile/{self.profile.userId}/joined", headers=self.additional_headers(data=data), data=data)
 
         elif isinstance(userId, list):
-            data = dumps({"targetUidList": userId, "timestamp": int(timestamp() * 1000)})
+            data = dumps({"targetUidList": userId, "timestamp": inttime()})
             
             response = self.session.post(f"/x{self.comId}/s/user-profile/{self.profile.userId}/joined", headers=self.additional_headers(data=data), data=data)
 
         else: raise exceptions.WrongType(type(userId))
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -1228,15 +1196,15 @@
         """
         if reason is None: raise exceptions.ReasonNeeded()
         if flagType is None: raise exceptions.FlagTypeNeeded()
 
         data = {
             "flagType": flagType,
             "message": reason,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["objectId"] = userId
             data["objectType"] = 0
 
         elif blogId:
@@ -1262,16 +1230,21 @@
     def send_message(
             self,
             chatId: str, message: str = None, messageType: int = 0,
             file: BinaryIO = None, fileType: str = None,
             replyTo: str = None, mentionUserIds: list = None,
             stickerId: str = None,
         
-            embedId: str = None, embedObjectType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None,
-            embedType: objects.EmbedTypes = objects.EmbedTypes.LINK_SNIPPET
+            embedId: str = None,
+            embedLink: str = None,
+            embedTitle: str = None,
+            embedContent: str = None,
+            embedImage: BinaryIO = None,
+            embedType: objects.EmbedTypes = None,
+            embedObjectType: objects.AttachedObjectTypes = None
         ):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **message** : Message to be sent
             - **chatId** : ID of the Chat.
@@ -1279,76 +1252,87 @@
             - **fileType** : Type of the file.
                 - ``audio``, ``image``, ``gif``
             - **messageType** : Type of the Message.
             - **mentionUserIds** : List of User IDS to mention. '@' needed in the Message.
             - **replyTo** : Message ID to reply to.
             - **stickerId** : Sticker ID to be sent.
             - **embedType** : Type of the Embed. Can be aminofixfix.lib.objects.EmbedTypes only. By default it's LinkSnippet one.
-            - **embedLink** : Link of the Embed.
-            - **embedImage** : Image of the Embed. Required to send Embed.
-            - **embedId** : ID of the Embed. Works only in AttachedObject Embeds.
-            - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds.
-            - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds.
-            - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds.
+            - **embedLink** : Link of the Embed. Can be only "ndc://" link if its AttachedObject.
+            - **embedImage** : Image of the Embed. Required to send Embed, if its LinkSnippet. Can be only 1024x1024 max. Can be string to existing image uploaded to Amino or it can be opened (not readed) file.
+            - **embedId** : ID of the Embed. Works only in AttachedObject Embeds. It can be any ID, just gen it using str_uuid4().
+            - **embedType** : Type of the AttachedObject Embed. Works only in AttachedObject Embeds. Just look what values AttachedObjectTypes enum contains.
+            - **embedTitle** : Title of the Embed. Works only in AttachedObject Embeds. Can be empty.
+            - **embedContent** : Content of the Embed. Works only in AttachedObject Embeds. Can be empty.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
 
         if message is not None and file is None:
             message = message.replace("<$", "‎‏").replace("$>", "‬‭")
 
         mentions = []
         if mentionUserIds:
             mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
 
-        if not isinstance(embedImage, BinaryIO):
-            embedType = None
+        if embedImage and not isinstance(embedImage, str):
+            try: readEmbed = embedImage.read()
+            except: embedType = None
 
         if embedType == objects.EmbedTypes.LINK_SNIPPET:
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "extensions": {
                     "linkSnippetList": [{
                         "link": embedLink,
                         "mediaType": 100,
-                        "mediaUploadValue": b64encode(embedImage.read()).decode(),
+                        "mediaUploadValue": b64_to_bytes(readEmbed),
                         "mediaUploadValueContentType": "image/png"
                     }],
                     "mentionedArray": mentions
                 },
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
         elif embedType == objects.EmbedTypes.ATTACHED_OBJECT:
+            try: embedObjectType.value
+            except: raise Exception("You SHOULD pass AttachedEmbedTypes.")
+
+            if isinstance(embedImage, str):
+                image = [[100, embedImage, None]]
+            elif embedImage:
+                image = [[100, self.upload_media(embedImage, "image"), None]]
+            else:
+                image = None
+
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "attachedObject": {
                     "objectId": embedId,
-                    "objectType": embedObjectType,
+                    "objectType": embedObjectType.value,
                     "link": embedLink,
                     "title": embedTitle,
                     "content": embedContent,
-                    "mediaList": [[100, self.upload_media(embedImage, "image"), None]]
+                    "mediaList": image
                 },
                 "extensions": {"mentionedArray": mentions},
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
         else:
             data = {
                 "type": messageType,
                 "content": message,
-                "clientRefId": int(timestamp() / 10 % 1000000000),
+                "clientRefId": clientrefid(),
                 "extensions": {"mentionedArray": mentions},
-                "timestamp": int(timestamp() * 1000)
+                "timestamp": inttime()
             }
 
         if replyTo: data["replyMessageId"] = replyTo
 
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
@@ -1368,17 +1352,18 @@
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
             else: raise exceptions.SpecifyType(fileType)
 
-            data["mediaUploadValue"] = b64encode(file.read()).decode()
+            data["mediaUploadValue"] = b64_to_bytes(file.read())
 
         data = dumps(data)
+        print(data)
 
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/message", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
@@ -1395,15 +1380,15 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = {
             "adminOpName": 102,
             # "adminOpNote": {"content": reason},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
         if asStaff and reason:
             data["adminOpNote"] = {"content": reason}
 
         data = dumps(data)
         
         if not asStaff: response = self.session.delete(f"/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}", headers=self.additional_headers())
@@ -1423,15 +1408,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
         data = dumps({
             "messageId": messageId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/mark-as-read", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1458,15 +1443,15 @@
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = {"timestamp": inttime()}
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if announcement: data["extensions"] = {"announcement": announcement}
         if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
@@ -1475,22 +1460,22 @@
         if publishToGlobal: data["publishToGlobal"] = 0
         if not publishToGlobal: data["publishToGlobal"] = 1
 
         res = []
 
         if doNotDisturb is not None:
             if doNotDisturb:
-                data = dumps({"alertOption": 2, "timestamp": int(timestamp() * 1000)})
+                data = dumps({"alertOption": 2, "timestamp": inttime()})
                 
                 response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.additional_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
             if not doNotDisturb:
-                data = dumps({"alertOption": 1, "timestamp": int(timestamp() * 1000)})
+                data = dumps({"alertOption": 1, "timestamp": inttime()})
                 
                 response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/alert", data=data, headers=self.additional_headers(data=data))
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
         if pinChat is not None:
             if pinChat:
@@ -1500,22 +1485,22 @@
 
             if not pinChat:
                 response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/unpin", data=data, headers=self.additional_headers())
                 if response.status_code != 200: res.append(exceptions.CheckException(response))
                 else: res.append(response.status_code)
 
         if backgroundImage is not None:
-            data = dumps({"media": [100, backgroundImage, None], "timestamp": int(timestamp() * 1000)})
+            data = dumps({"media": [100, backgroundImage, None], "timestamp": inttime()})
             
             response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/member/{self.profile.userId}/background", data=data, headers=self.additional_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response))
             else: res.append(response.status_code)
 
         if coHosts is not None:
-            data = dumps({"uidList": coHosts, "timestamp": int(timestamp() * 1000)})
+            data = dumps({"uidList": coHosts, "timestamp": inttime()})
             
             response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/co-host", data=data, headers=self.additional_headers(data=data))
             if response.status_code != 200: res.append(exceptions.CheckException(response))
             else: res.append(response.status_code)
 
         if viewOnly is not None:
             if viewOnly:
@@ -1569,15 +1554,15 @@
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "uidList": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/transfer-organizer", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1700,22 +1685,22 @@
         - transactionId: str = None
             - unique id of transaction
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
-        if transactionId is None: transactionId = str(UUID(hexlify(urandom(16)).decode('ascii')))
+        if transactionId is None: transactionId = str_uuid4()
 
         data = dumps({
             "paymentContext": {
                 "transactionId": transactionId,
                 "isAutoRenew": autoRenew
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/influencer/{userId}/subscribe", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1750,15 +1735,15 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "mode": quizMode,
             "quizAnswerList": quizAnswerList,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1775,26 +1760,24 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         quizAnswerList = []
 
         for question, answer in zip(questionIdsList, answerIdsList):
-            part = dumps({
+            quizAnswerList.append({
                 "optIdList": [answer],
                 "quizQuestionId": question,
                 "timeSpent": 0.0
             })
 
-            quizAnswerList.append(loads(part))
-
         data = dumps({
             "mode": quizMode,
             "quizAnswerList": quizAnswerList,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/blog/{quizId}/quiz/result", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -1811,15 +1794,15 @@
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "vvChatJoinType": permission,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
         
         response = self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/vvchat-permission", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -2001,15 +1984,15 @@
         Accepting:
         - userId: str
 
         Recieving:
         - object `UserCheckIns`
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
-        response = self.session.get(f"/x{self.comId}/s/check-in/stats/{userId}?timezone={-timezone // 1000}", headers=self.additional_headers())
+        response = self.session.get(f"/x{self.comId}/s/check-in/stats/{userId}?timezone={LOCAL_TIMEZONE}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.UserCheckIns(response.json()).UserCheckIns
 
     def get_user_blogs(self, userId: str, start: int = 0, size: int = 25):
         """
         Get info about user's blogs.
@@ -2791,51 +2774,62 @@
         elif wikiId: response = self.session.get(f"/x{self.comId}/s/admin/operation?objectId={wikiId}&objectType=2&pagingType=t&size={size}", headers=self.additional_headers())
         elif fileId: response = self.session.get(f"/x{self.comId}/s/admin/operation?objectId={fileId}&objectType=109&pagingType=t&size={size}", headers=self.additional_headers())
         else: response = self.session.get(f"/x{self.comId}/s/admin/operation?pagingType=t&size={size}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.AdminLogList(response.json()["adminLogList"]).AdminLogList
 
-    def feature(self, time: int, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
+    def feature(
+            self,
+            time: int | objects.PostFeatureDays | objects.ChatFeatureDays | objects.UserFeatureDays,
+            userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None
+        ):
         """
         Feature object.
 
         Accepting:
         - time: int
-            - time == 1 is one day (for chats its one hour)
-            - time == 2 is two days (for chats its two hours)
-            - time == 3 is three days (for chats its three hours)
+            - it can be int, but better if it will be enum
         - userId: str = None
         - blogId: str = None
         - wikiId: str = None
         - quizId: str = None
             - can be only one field
             - userId -> blogId -> wikiId -> fileId
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         if chatId:
-            if time == 1: time = 3600
-            if time == 2: time = 7200
-            if time == 3: time = 10800
+            if isinstance(time, int):
+                if time == 1: inttime = 3600
+                elif time == 2: inttime = 7200
+                elif time == 3: inttime = 10800
+                else: raise exceptions.WrongType(time)
+            else:
+                try: inttime = time.value
+                except: raise exceptions.WrongType(time)
 
         else:
-            if time == 1: time = 86400
-            elif time == 2: time = 172800
-            elif time == 3: time = 259200
-            else: raise exceptions.WrongType(time)
+            if isinstance(time, int):
+                if time == 1: inttime = 86400
+                elif time == 2: inttime = 172800
+                elif time == 3: inttime = 259200
+                else: raise exceptions.WrongType(time)
+            else:
+                try: inttime = time.value
+                except: raise exceptions.WrongType(time)
 
         data = {
             "adminOpName": 114,
             "adminOpValue": {
-                "featuredDuration": time
+                "featuredDuration": inttime
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["adminOpValue"] = {"featuredType": 4}
             data = dumps(data)
             response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
 
@@ -2874,15 +2868,15 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = {
             "adminOpName": 114,
             "adminOpValue": {},
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["adminOpValue"] = {"featuredType": 0}
             data = dumps(data)
             response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
 
@@ -2924,15 +2918,15 @@
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = {
             "adminOpNote": {
                 "content": reason or "[empty reason]"
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["adminOpName"] = 18
             data = dumps(data)
             response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
 
@@ -2990,15 +2984,15 @@
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         
         data = {
             "adminOpNote": {
                 "content": reason
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if userId:
             data["adminOpName"] = 19
             data = dumps(data)
             response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
 
@@ -3056,15 +3050,15 @@
             tlt.append({"title": titles, "color": colors})
 
         data = dumps({
             "adminOpName": 207,
             "adminOpValue": {
                 "titles": tlt
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -3089,15 +3083,15 @@
             tlt.append({"title": title, "color": color})
 
         data = dumps({
             "adminOpName": 207,
             "adminOpValue": {
                 "titles": tlt
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/admin", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -3122,15 +3116,15 @@
             "attachedObject": {
                 "objectId": userId,
                 "objectType": 0
             },
             "penaltyType": 0,
             "adminOpNote": {},
             "noticeType": 7,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/notice", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -3143,42 +3137,44 @@
         - userId: str
         - time: int
             - time == 1 is 1 hour
             - time == 2 is 4 hours
             - time == 3 is 8 hours
             - time == 4 is 12 hours
             - time == 5 is 24 hours
+            - time == 6 is 72 hours (visually, its 24 hours)
         - title: str = None
         - reason: str = None
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
 
         if time == 1: time = 3600
         elif time == 2: time = 10800
         elif time == 3: time = 21600
         elif time == 4: time = 43200
         elif time == 5: time = 86400
+        elif time == 6: time = 259200
         else: raise exceptions.WrongType(time)
 
         data = dumps({
             "uid": userId,
             "title": title or "You got striked by Knife of Justice!",
             "content": reason or "You got striked by Knife of Justice by this admin! Sadly, there is no reason. Admin thought that amino.fix.fix will forgive this, hehe. :з",
             "attachedObject": {
                 "objectId": userId,
                 "objectType": 0
             },
             "penaltyType": 1,
             "penaltyValue": time,
             "adminOpNote": {},
             "noticeType": 4,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/notice", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -3196,15 +3192,15 @@
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "reasonType": banType,
             "note": {
                 "content": reason or "No reason provided. (Amino.fix.fix will NOT allow fully empty ban reasons. It's not fair.)"
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/ban", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -3220,15 +3216,15 @@
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "note": {
                 "content": reason
             },
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/{userId}/unban", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -3241,15 +3237,15 @@
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "uidList": userIds,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/user-profile/featured/reorder", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.json()
 
@@ -3425,15 +3421,15 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = {'objectId': objectId,
                 'objectType': objectType,
                 'v': 1,
-                "timestamp": int(timestamp() * 1000)}
+                "timestamp": inttime()}
 
         if aminoPlus: data['paymentContext'] = {'discountStatus': 1, 'discountValue': 1, 'isAutoRenew': autoRenew}
         else: data['paymentContext'] = {'discountStatus': 0, 'discountValue': 1, 'isAutoRenew': autoRenew}
 
         data = dumps(data)
         response = self.session.post(f"/x{self.comId}/s/store/purchase", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
@@ -3454,15 +3450,15 @@
 
             - **Fail** : :meth:`Exceptions <aminofixfix.lib.exceptions>`
 
         """
 
         data = {"frameId": avatarId,
                 "applyToAll": 0,
-                "timestamp": int(timestamp() * 1000)}
+                "timestamp": inttime()}
 
         if applyToAll: data["applyToAll"] = 1
 
         data = dumps(data)
         response = self.session.post(f"/x{self.comId}/s/avatar-frame/apply", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
@@ -3503,15 +3499,15 @@
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "mediaList": None,
             "title": question,
             "type": 0,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/blog/{blogId}/poll/option", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -3530,15 +3526,15 @@
         """
         data = dumps({
             "content": content,
             "icon": None,
             "label": title,
             "mediaList": None,
             "parentCategoryId": parentCategoryId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/item-category", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -3551,15 +3547,15 @@
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
                 "title":title,
-                "timestamp":int(timestamp() * 1000)
+                "timestamp":inttime()
             })
         response = self.session.post(f"/x{self.comId}/s/shared-folder/folders", headers=self.additional_headers(data=data),data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
     def submit_to_wiki(self, wikiId: str, message: str):
@@ -3575,15 +3571,15 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "message": message,
             "itemId": wikiId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/knowledge-base-request", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -3604,15 +3600,15 @@
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = dumps({
             "destinationCategoryIdList": destinationCategoryIdList,
             "actionType": "create",
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         })
 
         response = self.session.post(f"/x{self.comId}/s/knowledge-base-request/{requestId}/approve", headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
@@ -3688,15 +3684,15 @@
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
         data = {
             "applyToAll": 0,
             "bubbleId": bubbleId,
             "threadId": chatId,
-            "timestamp": int(timestamp() * 1000)
+            "timestamp": inttime()
         }
 
         if applyToAll is True:
             data["applyToAll"] = 1
 
         data = dumps(data)
         response = self.session.post(f"/x{self.comId}/s/chat/thread/apply-bubble", headers=self.additional_headers(data=data), data=data)
@@ -3715,30 +3711,30 @@
         - imageFile: BinaryIO [open(file, "rb")]
         - mediaUhqEnabled: bool = False
 
         Recieving:
         - object `int` (200)
         - on exception, some exception from `aminofixfix.lib.exceptions`
         """
-        i = str(uuid4()).upper()
+        i = str_uuid4().upper()
         cover = f"{i}_thumb.jpg"
         video = f"{i}.mp4"
         
         data = dumps({
-            "clientRefId": int(timestamp() / 10 % 1000000000),
+            "clientRefId": clientrefid(),
             "content": message,
             "mediaType": 123,
             "videoUpload":
             {
                 "contentType": "video/mp4",
                 "cover": cover,
                 "video": video
             },
             "type": 4,
-            "timestamp": int(timestamp() * 1000),
+            "timestamp": inttime(),
             "mediaUhqEnabled": mediaUhqEnabled,
             "extensions": {}    
         })
 
         files = {
             video: (video, videoFile.read(), 'video/mp4'),
             cover: (cover, imageFile.read(), 'application/octet-stream'),
```

### Comparing `amino.fix.fix-1.0.6b2/setup.py` & `amino.fix.fix-1.0.7b1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-LIBRARY_VERSION = "1.0.6b2"
+LIBRARY_VERSION = "1.0.7b1"
 
 # REQUIREMENTS
 
 requirements = [
     "httpx>=0.27.0",
     "httpx[http2]",
     "httpx[socks]",
@@ -40,27 +40,30 @@
     'imperialwool',
 ]
 
 # setup
 
 setup(
     license="MIT",
+
     name="amino.fix.fix",
-    version=LIBRARY_VERSION,
     description="Library for Aminoapps",
+    
+    version=LIBRARY_VERSION,
     url="https://github.com/imperialwool/Amino.fix.fix",
-    long_description=open("README.md", encoding="utf-8").read(),
+
     long_description_content_type="text/markdown",
+    long_description=open("README.md", encoding="utf-8").read(),
 
     author="imperialwool",
     author_email="hi@iwool.dev",
     
     python_requires='>=3.8',
     packages=find_packages(),
-    keywords=keywords,
 
+    keywords=keywords,
     install_requires=requirements,
     extras_require={
         "requests": requests_requirements,
         "aiohttp": aiohttp_requirements,
     },
 )
```

