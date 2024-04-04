# Comparing `tmp/amino.fix.fix-1.0.7b2.tar.gz` & `tmp/amino.fix.fix-1.0.7b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.fix.fix-1.0.7b2.tar", last modified: Thu Apr  4 01:09:04 2024, max compression
+gzip compressed data, was "amino.fix.fix-1.0.7b3.tar", last modified: Thu Apr  4 01:31:45 2024, max compression
```

## Comparing `amino.fix.fix-1.0.7b2.tar` & `amino.fix.fix-1.0.7b3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.243396 amino.fix.fix-1.0.7b2/
--rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.7b2/LICENSE
--rw-rw-rw-   0        0        0     4047 2024-04-04 01:09:04.243396 amino.fix.fix-1.0.7b2/PKG-INFO
--rw-rw-rw-   0        0        0     3564 2024-04-04 01:08:16.000000 amino.fix.fix-1.0.7b2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.220859 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/
--rw-rw-rw-   0        0        0     4047 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-04 01:09:04.000000 amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.226859 amino.fix.fix-1.0.7b2/aminofixfix/
--rw-rw-rw-   0        0        0     1365 2024-04-04 01:01:01.000000 amino.fix.fix-1.0.7b2/aminofixfix/__init__.py
--rw-rw-rw-   0        0        0    24271 2024-04-04 00:32:10.000000 amino.fix.fix-1.0.7b2/aminofixfix/acm.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.231885 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/
--rw-rw-rw-   0        0        0     1366 2024-04-04 01:03:00.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/__init__.py
--rw-rw-rw-   0        0        0    16275 2024-04-04 00:31:58.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/acm.py
--rw-rw-rw-   0        0        0    95279 2024-04-04 01:07:10.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/client.py
--rw-rw-rw-   0        0        0    14887 2024-04-04 00:45:22.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/socket.py
--rw-rw-rw-   0        0        0   108064 2024-04-04 01:07:51.000000 amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/sub_client.py
--rw-rw-rw-   0        0        0   101798 2024-04-04 00:43:54.000000 amino.fix.fix-1.0.7b2/aminofixfix/client.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.237390 amino.fix.fix-1.0.7b2/aminofixfix/lib/
--rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/__init__.py
--rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-04 01:09:04.242397 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/
--rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/__init__.py
--rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/aiohttp.py
--rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/requests.py
--rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/unsuccessful_import.py
--rw-rw-rw-   0        0        0     5911 2024-04-04 00:41:52.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/headers.py
--rw-rw-rw-   0        0        0     5113 2024-04-04 01:08:37.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/helpers.py
--rw-rw-rw-   0        0        0   198878 2024-04-04 00:03:14.000000 amino.fix.fix-1.0.7b2/aminofixfix/lib/objects.py
--rw-rw-rw-   0        0        0    14885 2024-04-04 00:10:47.000000 amino.fix.fix-1.0.7b2/aminofixfix/socket.py
--rw-rw-rw-   0        0        0   144345 2024-04-04 00:38:17.000000 amino.fix.fix-1.0.7b2/aminofixfix/sub_client.py
--rw-rw-rw-   0        0        0       42 2024-04-04 01:09:04.244398 amino.fix.fix-1.0.7b2/setup.cfg
--rw-rw-rw-   0        0        0     1251 2024-04-04 01:08:12.000000 amino.fix.fix-1.0.7b2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.414304 amino.fix.fix-1.0.7b3/
+-rw-rw-rw-   0        0        0     1095 2024-03-07 00:20:09.000000 amino.fix.fix-1.0.7b3/LICENSE
+-rw-rw-rw-   0        0        0     4047 2024-04-04 01:31:45.414304 amino.fix.fix-1.0.7b3/PKG-INFO
+-rw-rw-rw-   0        0        0     3564 2024-04-04 01:15:28.000000 amino.fix.fix-1.0.7b3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.393285 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/
+-rw-rw-rw-   0        0        0     4047 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-04 01:31:45.000000 amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.398280 amino.fix.fix-1.0.7b3/aminofixfix/
+-rw-rw-rw-   0        0        0     1269 2024-04-04 01:14:49.000000 amino.fix.fix-1.0.7b3/aminofixfix/__init__.py
+-rw-rw-rw-   0        0        0    24271 2024-04-04 00:32:10.000000 amino.fix.fix-1.0.7b3/aminofixfix/acm.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.403791 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/
+-rw-rw-rw-   0        0        0     1270 2024-04-04 01:15:01.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/__init__.py
+-rw-rw-rw-   0        0        0    16275 2024-04-04 00:31:58.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/acm.py
+-rw-rw-rw-   0        0        0    95279 2024-04-04 01:07:10.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/client.py
+-rw-rw-rw-   0        0        0    14887 2024-04-04 00:45:22.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/socket.py
+-rw-rw-rw-   0        0        0   109087 2024-04-04 01:28:18.000000 amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/sub_client.py
+-rw-rw-rw-   0        0        0   101936 2024-04-04 01:30:42.000000 amino.fix.fix-1.0.7b3/aminofixfix/client.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.408792 amino.fix.fix-1.0.7b3/aminofixfix/lib/
+-rw-rw-rw-   0        0        0       95 2024-03-06 23:42:06.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/__init__.py
+-rw-rw-rw-   0        0        0    33502 2024-03-18 19:32:24.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:31:45.413304 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/
+-rw-rw-rw-   0        0        0      251 2024-03-27 13:19:12.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/__init__.py
+-rw-rw-rw-   0        0        0     3494 2024-03-27 13:09:18.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/aiohttp.py
+-rw-rw-rw-   0        0        0     2688 2024-03-27 11:57:04.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/requests.py
+-rw-rw-rw-   0        0        0      668 2024-03-27 13:18:55.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/unsuccessful_import.py
+-rw-rw-rw-   0        0        0     5911 2024-04-04 00:41:52.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/headers.py
+-rw-rw-rw-   0        0        0     5113 2024-04-04 01:15:40.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/helpers.py
+-rw-rw-rw-   0        0        0   198878 2024-04-04 00:03:14.000000 amino.fix.fix-1.0.7b3/aminofixfix/lib/objects.py
+-rw-rw-rw-   0        0        0    14885 2024-04-04 00:10:47.000000 amino.fix.fix-1.0.7b3/aminofixfix/socket.py
+-rw-rw-rw-   0        0        0   145086 2024-04-04 01:28:10.000000 amino.fix.fix-1.0.7b3/aminofixfix/sub_client.py
+-rw-rw-rw-   0        0        0       42 2024-04-04 01:31:45.415305 amino.fix.fix-1.0.7b3/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2024-04-04 01:15:32.000000 amino.fix.fix-1.0.7b3/setup.py
```

### Comparing `amino.fix.fix-1.0.7b2/LICENSE` & `amino.fix.fix-1.0.7b3/LICENSE`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/PKG-INFO` & `amino.fix.fix-1.0.7b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.7b2
+Version: 1.0.7b3
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
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b2-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b3-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b2/README.md` & `amino.fix.fix-1.0.7b3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b2-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b3-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/PKG-INFO` & `amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amino.fix.fix
-Version: 1.0.7b2
+Version: 1.0.7b3
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
-[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b2-blue)](https://pypi.org/project/amino.fix.fix/#history)
+[![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b3-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.9-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
 Fork of Amino.fix to improve this library.
 
 ## Important notices
```

### Comparing `amino.fix.fix-1.0.7b2/amino.fix.fix.egg-info/SOURCES.txt` & `amino.fix.fix-1.0.7b3/amino.fix.fix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/__init__.py` & `amino.fix.fix-1.0.7b3/aminofixfix/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,19 +13,24 @@
     try:
         response = urlopen("https://pypi.org/pypi/amino.fix.fix/json")
         data = loads(response.read())
 
         __newest__ = data["info"]["version"]
 
         if version(__newest__) > version(helpers.LIBRARY_VERSION):
-            print("\n!!! New version of amino.fix.fix is available !!!",
-                "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
-                "!!! Please, update library to last version !!!\n", sep="\n")
+            print(
+                "\n! New version of amino.fix.fix is available !",
+                "| Using: {} | Available: {} |\n".format(helpers.LIBRARY_VERSION, __newest__),
+                
+                sep="\n"
+            )
         elif version(__newest__) < version(helpers.LIBRARY_VERSION):
-            print("\n!!! ATTENTION, MODIFIED LIBRARY OR PREVIEW VERSION !!!",
-                "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
-                "!!! Please, make sure that library installed from verified sources !!!",
-                "Example: pip install amino.fix.fix\n", sep="\n")
+            print(
+                "\n! Using preview version {} of amino.fix.fix !".format(helpers.LIBRARY_VERSION),
+                "| Latest stable available: {} |\n".format(__newest__),
+                
+                sep="\n"
+            )
     except:
         print("\nCan't check if amino.fix.fix needs update. Please, check internet connection or firewall.\n")
 
 Thread(target=work).start()
```

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/acm.py` & `amino.fix.fix-1.0.7b3/aminofixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/__init__.py` & `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,19 +13,24 @@
     try:
         response = urlopen("https://pypi.org/pypi/amino.fix.fix/json")
         data = loads(response.read())
 
         __newest__ = data["info"]["version"]
 
         if version(__newest__) > version(helpers.LIBRARY_VERSION):
-            print("\n!!! New version of amino.fix.fix is available !!!",
-                "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
-                "!!! Please, update library to last version !!!\n", sep="\n")
+            print(
+                "\n! New version of amino.fix.fix is available !",
+                "| Using: {} | Available: {} |\n".format(helpers.LIBRARY_VERSION, __newest__),
+                
+                sep="\n"
+            )
         elif version(__newest__) < version(helpers.LIBRARY_VERSION):
-            print("\n!!! ATTENTION, MODIFIED LIBRARY OR PREVIEW VERSION !!!",
-                "||| Using: {} | Available: {} |||".format(helpers.LIBRARY_VERSION, __newest__),
-                "!!! Please, make sure that library installed from verified sources !!!",
-                "Example: pip install amino.fix.fix\n", sep="\n")
+            print(
+                "\n! Using preview version {} of amino.fix.fix !".format(helpers.LIBRARY_VERSION),
+                "| Latest stable available: {} |\n".format(__newest__),
+                
+                sep="\n"
+            )
     except:
         print("\nCan't check if amino.fix.fix needs update. Please, check internet connection or firewall.\n")
 
 Thread(target=work).start()
```

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/acm.py` & `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/client.py` & `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/client.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/socket.py` & `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/asyncfixfix/sub_client.py` & `amino.fix.fix-1.0.7b3/aminofixfix/asyncfixfix/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,55 +5,89 @@
 from typing import BinaryIO
 
 from .client import Client
 from ..lib import exceptions, headers, objects
 from ..lib.helpers import gen_deviceId, json_minify, str_uuid4, inttime, clientrefid, b64_to_bytes, LOCAL_TIMEZONE
 
 class SubClient(Client):
+    """
+        Client to work with community in Amino.
+        (aminoapps.com)
+    """
     def __init__(
         self, mainClient: Client,
-        comId: str = None, aminoId: str = None, *,
-        deviceId: str = None, autoDevice: bool | None = None, proxies: dict = None,
-        api_library: objects.APILibraries | None = None
+        comId: str = None, aminoId: str = None,
+         
+        get_community: bool = False,
+        get_profile: bool = False,
+        **kwargs
     ):
+        """
+        Init subclient.
+
+        Accepting:
+        - mainClient: aminofixfix.Client
+        - comId: str | int | None = None
+        - aminoId: str | None = None
+            - you can pass only one thing
+            - comId will be taken first
+        - get_community: bool = False
+            - should subclient get info about community you passed?
+            - False for no (default), True for yes
+        - get_profile: bool = False
+            - should subclient get info about your profile in community you passed?
+            - False for no (default), True for yes
+    
+        
+        \- imperialwool, where is another fields of subclient??? ;-;
+
+        \- its in main client lol why you need to pass them again
+        """
         Client.__init__(
-            self, deviceId=deviceId, proxies=proxies,
-            autoDevice=autoDevice or mainClient.autoDevice, userAgent=mainClient.user_agent,
+            self, deviceId=mainClient.device_id, proxies=mainClient.proxies,
+            autoDevice=mainClient.autoDevice, userAgent=mainClient.user_agent,
             http2_enabled=mainClient.http2_enabled,
             own_timeout=mainClient.timeout_settings,
             socket_enabled=False,
-            api_library=api_library or mainClient.api_library or objects.APILibraries.HTTPX
+            api_library=mainClient.api_library or objects.APILibraries.HTTPX
         )
-        self.comId = comId
-        self.aminoId = aminoId
-        self.vc_connect = False
-        self.mainClient = mainClient
-        
-        self.sid = self.mainClient.sid
-        self.userId = self.mainClient.userId
-        self.device_id = self.mainClient.device_id
-        self.user_agent = self.mainClient.user_agent
-        
-        self.community: objects.Community
-        self.profile: objects.UserProfile = self.mainClient.profile
+        self.vc_connect: bool = False
+        self.sid: str = mainClient.sid
+        self.device_id: str = mainClient.device_id
+        self.user_agent: str = mainClient.user_agent
+        self.profile: objects.UserProfile = mainClient.profile
+        self.userId: str = mainClient.userId
+
+        self.community: objects.Community | None = None
+        self.profile: objects.UserProfile | None = objects.UserProfile(None)
+
+        self.aminoId: str = aminoId
+        self.comId: str | int = comId
+
+        self.__get_profile: bool = get_profile
+        self.__get_community: bool = get_community
         
 
     def __await__(self):
         return self._init().__await__()
 
     async def _init(self):
-        if self.comId is not None:
-            self.community: objects.Community = await self.get_community_info(self.comId)
+        if self.comId is not None and self.__get_community:
+            self.community = await self.get_community_info(self.comId)
         if self.aminoId is not None:
             self.comId = (await self.mainClient.search_community(self.aminoId)).comId[0]
-            self.community: objects.Community = await self.mainClient.get_community_info(self.comId)
-        if self.comId is None and self.aminoId is None: raise exceptions.NoCommunity()
-        try: self.profile: objects.UserProfile = await self.get_user_info(userId=self.profile.userId)
-        except AttributeError: raise exceptions.FailedLogin()
-        except exceptions.UserUnavailable(): pass
+            if self.__get_community:
+                self.community = await self.mainClient.get_community_info(self.comId)
+        if self.comId is None and self.aminoId is None:
+            raise exceptions.NoCommunity()
+
+        if self.__get_profile:
+            try: self.profile: objects.UserProfile = await self.get_user_info(userId=self.profile.userId)
+            except AttributeError: raise exceptions.FailedLogin()
+            except exceptions.UserUnavailable(): pass
         return self
 
     def additional_headers(self, data: str = None, content_type: str = None):
         return headers.additionals(
             data=data,
             content_type=content_type,
             user_agent=self.user_agent,
```

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/client.py` & `amino.fix.fix-1.0.7b3/aminofixfix/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,24 +78,26 @@
         - api_library: objects.APILibraries = objects.APILibraries.HTTPX
             - choicing library for API requests
             - can be useful if you have troubles with HTTPX
             - *can* be not so stable as HTTPX
             - you can choice library like `aminofixfix.lib.objects.APILibraries.HTTPX`,
               but you probably want to import `objects` from `aminofixfix.lib`
         """
-        self.api = "https://service.aminoapps.com/api/v1"
-        self.proxies = proxies
-        self.configured = False
-        self.authenticated = False
-        self.autoDevice = autoDevice
-        self.api_library = api_library
-        self.http2_enabled = http2_enabled
-        self.socket_enabled = socket_enabled
-        self.device_id = deviceId if deviceId else gen_deviceId()
-        self.user_agent = userAgent if userAgent else helpers.gen_userAgent()
+        self.api: str = "https://service.aminoapps.com/api/v1"
+
+        self.configured: bool = False
+        self.authenticated: bool = False
+        self.autoDevice: bool = autoDevice
+        self.proxies: str | dict = proxies
+        self.timeout_settings: TimeoutConfig
+        self.http2_enabled: bool = http2_enabled
+        self.socket_enabled: bool = socket_enabled
+        self.api_library: objects.APILibraries = api_library
+        self.device_id: str = deviceId if deviceId else gen_deviceId()
+        self.user_agent: str = userAgent if userAgent else helpers.gen_userAgent()
 
         if disable_timeout:
             self.timeout_settings = TimeoutConfig(None)
         elif isinstance(own_timeout, TimeoutConfig):
             self.timeout_settings = own_timeout
         elif read_timeout or write_timeout or pool_timeout or connect_timeout:
             self.timeout_settings = TimeoutConfig(
@@ -125,14 +127,15 @@
                 proxies=proxies,
                 timeout=self.timeout_settings
             )
 
         if self.socket_enabled:
             SocketHandler.__init__(self, self, socket_trace=socket_trace, debug=socketDebugging)
             Callbacks.__init__(self, self)
+            
         self.sid = None
         self.json = None
         self.secret = None
         self.userId = None
         self.account: objects.UserProfile = objects.UserProfile(None)
         self.profile: objects.UserProfile = objects.UserProfile(None)
```

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/lib/exceptions.py` & `amino.fix.fix-1.0.7b3/aminofixfix/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/aiohttp.py` & `amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/aiohttp.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/requests.py` & `amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/requests.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/lib/facades/unsuccessful_import.py` & `amino.fix.fix-1.0.7b3/aminofixfix/lib/facades/unsuccessful_import.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/lib/headers.py` & `amino.fix.fix-1.0.7b3/aminofixfix/lib/headers.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/lib/helpers.py` & `amino.fix.fix-1.0.7b3/aminofixfix/lib/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from hashlib import sha1
 from os import urandom
 from json import loads
 from uuid import uuid4
 from hmac import new
 import re
 
-LIBRARY_VERSION = "1.0.7b2"
+LIBRARY_VERSION = "1.0.7b3"
 
 PREFIX = bytes.fromhex("19")
 SIG_KEY = bytes.fromhex("DFA5ED192DDA6E88A12FE12130DC6206B1251E44")
 DEVICE_KEY = bytes.fromhex("E7309ECC0953C6FA60005B2765F99DBBC965C8E9")
 
 IPHONE_IDS = [
     "11,2", "11,4", "11,6", "11,8",
```

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/lib/objects.py` & `amino.fix.fix-1.0.7b3/aminofixfix/lib/objects.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/socket.py` & `amino.fix.fix-1.0.7b3/aminofixfix/socket.py`

 * *Files identical despite different names*

### Comparing `amino.fix.fix-1.0.7b2/aminofixfix/sub_client.py` & `amino.fix.fix-1.0.7b3/aminofixfix/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,63 +11,80 @@
 class SubClient(Client):
     """
         Client to work with community in Amino.
         (aminoapps.com)
     """
     def __init__(
         self, mainClient: Client,
-        comId: str = None, aminoId: str = None, **kwargs
+        comId: str = None, aminoId: str = None,
+         
+        get_community: bool = False,
+        get_profile: bool = False,
+        **kwargs
     ):
         """
         Init subclient.
 
         Accepting:
         - mainClient: aminofixfix.Client
-        - comId: str | int | None
-        - aminoId: str | None
+        - comId: str | int | None = None
+        - aminoId: str | None = None
             - you can pass only one thing
             - comId will be taken first
-
+        - get_community: bool = False
+            - should subclient get info about community you passed?
+            - False for no (default), True for yes
+        - get_profile: bool = False
+            - should subclient get info about your profile in community you passed?
+            - False for no (default), True for yes
     
         
         \- imperialwool, where is another fields of subclient??? ;-;
 
         \- its in main client lol why you need to pass them again
         """
         Client.__init__(
             self, deviceId=mainClient.device_id, proxies=mainClient.proxies,
             autoDevice=mainClient.autoDevice, userAgent=mainClient.user_agent,
             http2_enabled=mainClient.http2_enabled,
             own_timeout=mainClient.timeout_settings,
             socket_enabled=False,
             api_library=mainClient.api_library or objects.APILibraries.HTTPX
         )
-        self.vc_connect = False
-        self.sid = mainClient.sid
-        self.device_id = mainClient.device_id
-        self.user_agent = mainClient.user_agent
-        self.profile = mainClient.profile
-        self.userId = mainClient.userId
+        self.vc_connect: bool = False
+        self.sid: str = mainClient.sid
+        self.userId: str = mainClient.userId
+        self.device_id: str = mainClient.device_id
+        self.user_agent: str = mainClient.user_agent
+        self.profile: objects.UserProfile = mainClient.profile
+
+        self.comId: str | None = None
+        self.aminoId: str | None = None
+
+        self.community: objects.Community | None = None
+        self.profile: objects.UserProfile | None = objects.UserProfile(None)
 
         if comId is not None:
             self.comId = comId
-            self.community: objects.Community = self.get_community_info(comId)
+            if get_community:
+                self.community = self.get_community_info(comId)
 
         if aminoId is not None:
             link = "http://aminoapps.com/c/"
             self.comId = self.get_from_code(link + aminoId).comId
-            self.community: objects.Community = self.get_community_info(self.comId)
+            self.community = self.get_community_info(self.comId)
 
         if comId is None and aminoId is None: raise exceptions.NoCommunity()
 
-        try: self.profile: objects.UserProfile = self.get_user_info(userId=self.profile.userId)
-        except AttributeError: raise exceptions.FailedLogin()
-        except exceptions.UserUnavailable: pass
+        if get_profile:
+            try: self.profile: objects.UserProfile = self.get_user_info(userId=self.profile.userId)
+            except AttributeError: raise exceptions.FailedLogin()
+            except exceptions.UserUnavailable: pass
 
-    def additional_headers(self, data: str = None, content_type: str = None):
+    def additional_headers(self, data: str = None, content_type: str = None) -> dict[str, str]:
         """
         Function to make additional headers, that API needs.
 
         Accepting:
         - data: str
         - content_type: str
```

### Comparing `amino.fix.fix-1.0.7b2/setup.py` & `amino.fix.fix-1.0.7b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-LIBRARY_VERSION = "1.0.7b2"
+LIBRARY_VERSION = "1.0.7b3"
 
 # REQUIREMENTS
 
 requirements = [
     "httpx>=0.27.0",
     "httpx[http2]",
     "httpx[socks]",
```

