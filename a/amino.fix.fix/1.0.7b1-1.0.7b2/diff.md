# Comparing `tmp/amino.fix.fix-1.0.7b1.tar.gz` & `tmp/amino.fix.fix-1.0.7b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.fix.fix-1.0.7b1.tar", last modified: Thu Apr  4 01:04:20 2024, max compression
+gzip compressed data, was "amino.fix.fix-1.0.7b2.tar", last modified: Thu Apr  4 01:09:04 2024, max compression
```

## Comparing `amino.fix.fix-1.0.7b1.tar` & `amino.fix.fix-1.0.7b2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.371247 amino.fix.fix-1.0.7b1/
--rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.7b1/LICENSE
--rw-rw-rw-   0        0        0     4047 2024-04-04 01:04:20.371247 amino.fix.fix-1.0.7b1/PKG-INFO
--rw-rw-rw-   0        0        0     3564 2024-04-04 01:03:33.000000 amino.fix.fix-1.0.7b1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.350220 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/
--rw-rw-rw-   0        0        0     4047 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-04 01:04:20.000000 amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.355220 amino.fix.fix-1.0.7b1/aminofixfix/
--rw-rw-rw-   0        0        0     1365 2024-04-04 01:01:01.000000 amino.fix.fix-1.0.7b1/aminofixfix/__init__.py
--rw-rw-rw-   0        0        0    24271 2024-04-04 00:32:10.000000 amino.fix.fix-1.0.7b1/aminofixfix/acm.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.360733 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/
--rw-rw-rw-   0        0        0     1366 2024-04-04 01:03:00.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/__init__.py
--rw-rw-rw-   0        0        0    16275 2024-04-04 00:31:58.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/acm.py
--rw-rw-rw-   0        0        0    95310 2024-04-04 00:38:37.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/client.py
--rw-rw-rw-   0        0        0    14887 2024-04-04 00:45:22.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/socket.py
--rw-rw-rw-   0        0        0   108095 2024-04-04 00:37:41.000000 amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/sub_client.py
--rw-rw-rw-   0        0        0   101798 2024-04-04 00:43:54.000000 amino.fix.fix-1.0.7b1/aminofixfix/client.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.365734 amino.fix.fix-1.0.7b1/aminofixfix/lib/
--rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/__init__.py
--rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:04:20.370246 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/
--rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/__init__.py
--rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/aiohttp.py
--rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/requests.py
--rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/unsuccessful_import.py
--rw-rw-rw-   0        0        0     5911 2024-04-04 00:41:52.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/headers.py
--rw-rw-rw-   0        0        0     5144 2024-04-04 01:04:08.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/helpers.py
--rw-rw-rw-   0        0        0   198878 2024-04-04 00:03:14.000000 amino.fix.fix-1.0.7b1/aminofixfix/lib/objects.py
--rw-rw-rw-   0        0        0    14885 2024-04-04 00:10:47.000000 amino.fix.fix-1.0.7b1/aminofixfix/socket.py
--rw-rw-rw-   0        0        0   144345 2024-04-04 00:38:17.000000 amino.fix.fix-1.0.7b1/aminofixfix/sub_client.py
--rw-rw-rw-   0        0        0       42 2024-04-04 01:04:20.372246 amino.fix.fix-1.0.7b1/setup.cfg
--rw-rw-rw-   0        0        0     1251 2024-04-04 01:04:11.000000 amino.fix.fix-1.0.7b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.243396 amino.fix.fix-1.0.7b2/
+-rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.7b2/LICENSE
+-rw-rw-rw-   0        0        0     4047 2024-04-04 01:09:04.243396 amino.fix.fix-1.0.7b2/PKG-INFO
+-rw-rw-rw-   0        0        0     3564 2024-04-04 01:08:16.000000 amino.fix.fix-1.0.7b2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.220859 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/
+-rw-rw-rw-   0        0        0     4047 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.226859 amino.fix.fix-1.0.7b2/aminofixfix/
+-rw-rw-rw-   0        0        0     1365 2024-04-04 01:01:01.000000 amino.fix.fix-1.0.7b2/aminofixfix/__init__.py
+-rw-rw-rw-   0        0        0    24271 2024-04-04 00:32:10.000000 amino.fix.fix-1.0.7b2/aminofixfix/acm.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.231885 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/
+-rw-rw-rw-   0        0        0     1366 2024-04-04 01:03:00.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/__init__.py
+-rw-rw-rw-   0        0        0    16275 2024-04-04 00:31:58.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/acm.py
+-rw-rw-rw-   0        0        0    95279 2024-04-04 01:07:10.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/client.py
+-rw-rw-rw-   0        0        0    14887 2024-04-04 00:45:22.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/socket.py
+-rw-rw-rw-   0        0        0   108064 2024-04-04 01:07:51.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/sub_client.py
+-rw-rw-rw-   0        0        0   101798 2024-04-04 00:43:54.000000 amino.fix.fix-1.0.7b2/aminofixfix/client.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.237390 amino.fix.fix-1.0.7b2/aminofixfix/lib/
+-rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/__init__.py
+-rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.242397 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/
+-rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/__init__.py
+-rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/aiohttp.py
+-rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/requests.py
+-rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/unsuccessful_import.py
+-rw-rw-rw-   0        0        0     5911 2024-04-04 00:41:52.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/headers.py
+-rw-rw-rw-   0        0        0     5113 2024-04-04 01:08:37.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/helpers.py
+-rw-rw-rw-   0        0        0   198878 2024-04-04 00:03:14.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/objects.py
+-rw-rw-rw-   0        0        0    14885 2024-04-04 00:10:47.000000 amino.fix.fix-1.0.7b2/aminofixfix/socket.py
+-rw-rw-rw-   0        0        0   144345 2024-04-04 00:38:17.000000 amino.fix.fix-1.0.7b2/aminofixfix/sub_client.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 01:09:04.244398 amino.fix.fix-1.0.7b2/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2024-04-04 01:08:12.000000 amino.fix.fix-1.0.7b2/setup.py
```

### Comparing `amino.fix.fix-1.0.7b1/LICENSE` & `amino.fix.fix-1.0.7b2/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/PKG-INFO` & `amino.fix.fix-1.0.7b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.7b1
+Version: 1.0.7b2
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
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b2-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b1/README.md` & `amino.fix.fix-1.0.7b2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b2-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/PKG-INFO` & `amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.7b1
+Version: 1.0.7b2
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
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b1-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b2-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b1/amino.fix.fix.egg-info/SOURCES.txt` & `amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/__init__.py` & `amino.fix.fix-1.0.7b2/aminofixfix/__init__.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/acm.py` & `amino.fix.fix-1.0.7b2/aminofixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/__init__.py` & `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/__init__.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/acm.py` & `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/client.py` & `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 from time import sleep
 from json import dumps
+from typing import BinaryIO
 from threading import Thread
-from typing import BinaryIO, Union
 from httpx import Timeout as TimeoutConfig
 from httpx import AsyncClient as HttpxClient
 
 from .socket import Callbacks, SocketHandler
 from ..lib import exceptions, headers, objects, helpers
 from ..lib.facades import AiohttpClient, AiohttpResponse
 from ..lib.helpers import gen_deviceId, inttime, clientrefid, str_uuid4, bytes_to_b64, LOCAL_TIMEZONE
@@ -863,15 +863,15 @@
         """
         response = await self.session.delete(f"/g/s/chat/thread/{chatId}/member/{self.userId}", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
-    async def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
+    async def start_chat(self, userId: str | list, message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
         """
         Start an Chat with an User or List of Users.
 
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **message** : Starting Message.
             - **title** : Title of Group Chat.
@@ -907,15 +907,15 @@
 
         response = await self.session.post(f"/g/s/chat/thread", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return objects.Thread(response.json()["thread"]).Thread
 
-    async def invite_to_chat(self, userId: Union[str, list], chatId: str):
+    async def invite_to_chat(self, userId: str | list, chatId: str):
         """
         Invite a User or List of Users to a Chat.
 
         **Parameters**
             - **userId** : ID of the User or List of User IDs.
             - **chatId** : ID of the Chat.
 
@@ -1604,15 +1604,15 @@
         data = dumps(data)
         response = await self.session.post(url, headers=self.additional_headers(data=data), data=data)
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
-    async def follow(self, userId: Union[str, list]):
+    async def follow(self, userId: str | list):
         """
         Follow an User or Multiple Users.
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
@@ -2038,15 +2038,15 @@
         else: raise exceptions.SpecifyType
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else:
             return response.status_code
 
-    async def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None):
+    async def like_blog(self, blogId: str | list = None, wikiId: str = None):
         """
         Like a Blog, Multiple Blogs or a Wiki.
 
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
```

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/socket.py` & `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/asyncfixfix/sub_client.py` & `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 from json import dumps
-from typing import BinaryIO, Union
+from typing import BinaryIO
 
 from .client import Client
 from ..lib import exceptions, headers, objects
 from ..lib.helpers import gen_deviceId, json_minify, str_uuid4, inttime, clientrefid, b64_to_bytes, LOCAL_TIMEZONE
 
 class SubClient(Client):
     def __init__(
@@ -337,15 +337,15 @@
         elif wikiId: response = await self.session.delete(f"/x{self.comId}/s/item/{wikiId}/comment/{commentId}", headers=self.additional_headers())
         else: raise exceptions.SpecifyType()
 
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None) -> int:
+    async def like_blog(self, blogId: str | list = None, wikiId: str = None) -> int:
         """
         Like a Blog, Multiple Blogs or a Wiki.
 
         **Parameters**
             - **blogId** : ID of the Blog or List of IDs of the Blogs. (for Blogs)
             - **wikiId** : ID of the Wiki. (for Wikis)
 
@@ -518,15 +518,15 @@
 
     async def clear_notifications(self):
         response = await self.session.delete(f"/x{self.comId}/s/notification", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
+    async def start_chat(self, userId: str | list, message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = {
             "title": title,
             "inviteeUids": userIds,
@@ -544,15 +544,15 @@
         data = dumps(data)
         
         response = await self.session.post(f"/x{self.comId}/s/chat/thread", data=data, headers=self.additional_headers(data=data))
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return objects.Thread(response.json()["thread"]).Thread
 
-    async def invite_to_chat(self, userId: Union[str, list], chatId: str):
+    async def invite_to_chat(self, userId: str | list, chatId: str):
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = dumps({
             "uids": userIds,
             "timestamp": inttime()
@@ -597,15 +597,15 @@
 
     async def thank_tip(self, chatId: str, userId: str):
         response = await self.session.post(f"/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank", headers=self.additional_headers())
         if response.status_code != 200: 
             return exceptions.CheckException(response)
         else: return response.status_code
 
-    async def follow(self, userId: Union[str, list]):
+    async def follow(self, userId: str | list):
         """
         Follow an User or Multiple Users.
 
         **Parameters**
             - **userId** : ID of the User or List of IDs of the Users.
 
         **Returns**
```

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/client.py` & `amino.fix.fix-1.0.7b2/aminofixfix/client.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/lib/exceptions.py` & `amino.fix.fix-1.0.7b2/aminofixfix/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/aiohttp.py` & `amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/aiohttp.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/requests.py` & `amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/requests.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/lib/facades/unsuccessful_import.py` & `amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/unsuccessful_import.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/lib/headers.py` & `amino.fix.fix-1.0.7b2/aminofixfix/lib/headers.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/lib/helpers.py` & `amino.fix.fix-1.0.7b2/aminofixfix/lib/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 # ^ this thing should fix problem for python3.9 and lower(?)
 
 from base64 import b64decode, b64encode
 from time import timezone as tz_raw
 from time import time as timestamp
 from functools import reduce
 from random import choice
-from typing import Union
 from hashlib import sha1
 from os import urandom
 from json import loads
 from uuid import uuid4
 from hmac import new
 import re
 
-LIBRARY_VERSION = "1.0.7b1"
+LIBRARY_VERSION = "1.0.7b2"
 
 PREFIX = bytes.fromhex("19")
 SIG_KEY = bytes.fromhex("DFA5ED192DDA6E88A12FE12130DC6206B1251E44")
 DEVICE_KEY = bytes.fromhex("E7309ECC0953C6FA60005B2765F99DBBC965C8E9")
 
 IPHONE_IDS = [
     "11,2", "11,4", "11,6", "11,8",
@@ -53,15 +52,15 @@
     return "{}{}".format(identifier.hex(), new(DEVICE_KEY, identifier, sha1).hexdigest()).upper()
 
 def gen_userAgent() -> str:
     return "Apple iPhone{} iOS v{} Main/{}".format(
         choice(IPHONE_IDS), choice(IOS_VERSIONS), choice(APP_VERSIONS)
     )
 
-def signature(data: Union[str, bytes]) -> str:
+def signature(data: str | bytes) -> str:
     data = data if isinstance(data, bytes) else data.encode("utf-8")
     return b64encode(PREFIX + new(SIG_KEY, data, sha1).digest()).decode("utf-8")
 
 def update_deviceId(device: str) -> str:
     return gen_deviceId(bytes.fromhex(device[2:42]))
 
 def decode_sid(sid: str) -> dict:
```

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/lib/objects.py` & `amino.fix.fix-1.0.7b2/aminofixfix/lib/objects.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/socket.py` & `amino.fix.fix-1.0.7b2/aminofixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/aminofixfix/sub_client.py` & `amino.fix.fix-1.0.7b2/aminofixfix/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b1/setup.py` & `amino.fix.fix-1.0.7b2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-LIBRARY_VERSION = "1.0.7b1"
+LIBRARY_VERSION = "1.0.7b2"
 
 # REQUIREMENTS
 
 requirements = [
     "httpx>=0.27.0",
     "httpx[http2]",
     "httpx[socks]",
```

