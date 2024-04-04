# Comparing `tmp/eezo-0.1.5.tar.gz` & `tmp/eezo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eezo-0.1.5.tar", last modified: Tue Apr  2 20:38:15 2024, max compression
+gzip compressed data, was "eezo-0.1.6.tar", last modified: Thu Apr  4 16:48:48 2024, max compression
```

## Comparing `eezo-0.1.5.tar` & `eezo-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.326860 eezo-0.1.5/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-02 20:38:15.326742 eezo-0.1.5/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.5/README.md
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.324906 eezo-0.1.5/eezo/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.1.5/eezo/async_client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-03-27 15:07:04.000000 eezo-0.1.5/eezo/client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)    10624 2024-04-02 20:32:55.000000 eezo-0.1.5/eezo/connector.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.325848 eezo-0.1.5/eezo/interface/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       78 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/__init__.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.326591 eezo-0.1.5/eezo/interface/components/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/chart.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/component.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/image.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/text.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/components/youtube_video.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     3027 2024-03-19 14:09:37.000000 eezo-0.1.5/eezo/interface/interface.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.5/eezo/interface/message.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-02 20:38:15.325520 eezo-0.1.5/eezo.egg-info/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      533 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/SOURCES.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/dependency_links.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      353 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/requires.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-02 20:38:15.000000 eezo-0.1.5/eezo.egg-info/top_level.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-02 20:38:15.327023 eezo-0.1.5/setup.cfg
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1921 2024-04-02 20:36:22.000000 eezo-0.1.5/setup.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.212256 eezo-0.1.6/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-04 16:48:48.212136 eezo-0.1.6/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.6/README.md
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.208804 eezo-0.1.6/eezo/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.1.6/eezo/async_client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-03-27 15:07:04.000000 eezo-0.1.6/eezo/client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    11051 2024-04-04 16:40:31.000000 eezo-0.1.6/eezo/connector.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.210222 eezo-0.1.6/eezo/interface/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       78 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.211944 eezo-0.1.6/eezo/interface/components/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/chart.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/component.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/image.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/text.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/youtube_video.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     3027 2024-03-19 14:09:37.000000 eezo-0.1.6/eezo/interface/interface.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/message.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.209596 eezo-0.1.6/eezo.egg-info/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      533 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      353 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/requires.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/top_level.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-04 16:48:48.212291 eezo-0.1.6/setup.cfg
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1921 2024-04-04 16:45:52.000000 eezo-0.1.6/setup.py
```

### Comparing `eezo-0.1.5/PKG-INFO` & `eezo-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.5
+Version: 0.1.6
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.1.5/README.md` & `eezo-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `eezo-0.1.5/eezo/async_client.py` & `eezo-0.1.6/eezo/async_client.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.5/eezo/client.py` & `eezo-0.1.6/eezo/client.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.5/eezo/connector.py` & `eezo-0.1.6/eezo/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .interface import Interface, AsyncInterface
 
 import traceback
+import logging
 import asyncio
 import socketio
 import aiohttp
 import requests
 import time
 import os
 
@@ -39,14 +40,21 @@
         self.api_key = api_key
         self.logger = logger
         self.func = connector_function
         self.connector_id = connector_id
         self.job_responses = {}
         self.run_loop = True
 
+        if logger:
+            logging.basicConfig(
+                level=logging.INFO,
+                format="%(asctime)s: %(message)s",
+                datefmt="%Y-%m-%d %H:%M:%S",
+            )
+
         self.sio = socketio.AsyncClient(
             reconnection_attempts=0,
             reconnection_delay_max=10,
             reconnection_delay=1,
             engineio_logger=False,
             logger=False,
         )
@@ -61,15 +69,15 @@
                     "key": self.api_key,
                 },
             )
             self.__log(f" ✔ Connector {self.connector_id} connected")
 
     def __log(self, message):
         if self.logger:
-            print(message)
+            logging.info(message)
 
     async def __authenticate(self):
         async with aiohttp.ClientSession() as session:
             url = f"{SERVER}{API_VERSION}{REST_AUTH_URL}"
             async with session.post(url, json={"api_key": self.api_key}) as response:
                 if response.status == 200:
                     resp_json = await response.json()
@@ -167,14 +175,21 @@
         self.api_key = api_key
         self.logger = logger
         self.func = connector_function
         self.connector_id = connector_id
         self.job_responses = {}
         self.run_loop = True
 
+        if logger:
+            logging.basicConfig(
+                level=logging.INFO,
+                format="%(asctime)s: %(message)s",
+                datefmt="%Y-%m-%d %H:%M:%S",
+            )
+
         self.sio = socketio.Client(
             reconnection_attempts=0,
             reconnection_delay_max=10,
             reconnection_delay=1,
             engineio_logger=False,
             logger=False,
         )
@@ -189,15 +204,15 @@
                     "key": self.api_key,
                 },
             )
             self.__log(f" ✔ Connector {self.connector_id} connected")
 
     def __log(self, message):
         if self.logger:
-            print(message)
+            logging.info(message)
 
     def __authenticate(self):
         url = f"{SERVER}{API_VERSION}{REST_AUTH_URL}"
         response = requests.post(url, json={"api_key": self.api_key})
         if response.status_code == 200:
             self.auth_token = response.json().get("token")
         else:
```

### Comparing `eezo-0.1.5/eezo/interface/components/chart.py` & `eezo-0.1.6/eezo/interface/components/chart.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.5/eezo/interface/interface.py` & `eezo-0.1.6/eezo/interface/interface.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.5/eezo/interface/message.py` & `eezo-0.1.6/eezo/interface/message.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.5/eezo.egg-info/PKG-INFO` & `eezo-0.1.6/eezo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.5
+Version: 0.1.6
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.1.5/eezo.egg-info/SOURCES.txt` & `eezo-0.1.6/eezo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eezo-0.1.5/setup.py` & `eezo-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eezo",
-    version="0.1.5",
+    version="0.1.6",
     description="Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.",
     author="Daniel Schoenbohm",
     author_email="daniel@eezo.ai",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.9.3",
         "aiosignal==1.3.1",
```

