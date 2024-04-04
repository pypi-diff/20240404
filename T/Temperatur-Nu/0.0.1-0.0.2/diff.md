# Comparing `tmp/Temperatur_Nu-0.0.1.tar.gz` & `tmp/Temperatur_Nu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Temperatur_Nu-0.0.1.tar", last modified: Thu Apr  4 09:09:15 2024, max compression
+gzip compressed data, was "Temperatur_Nu-0.0.2.tar", last modified: Thu Apr  4 09:43:43 2024, max compression
```

## Comparing `Temperatur_Nu-0.0.1.tar` & `Temperatur_Nu-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 09:09:15.777986 Temperatur_Nu-0.0.1/
--rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      549 2024-04-04 09:09:15.777057 Temperatur_Nu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 09:09:15.775990 Temperatur_Nu-0.0.1/Temperatur_Nu.egg-info/
--rw-rw-rw-   0        0        0      549 2024-04-04 09:09:15.000000 Temperatur_Nu-0.0.1/Temperatur_Nu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-04 09:09:15.000000 Temperatur_Nu-0.0.1/Temperatur_Nu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 09:09:15.000000 Temperatur_Nu-0.0.1/Temperatur_Nu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-04 09:09:15.000000 Temperatur_Nu-0.0.1/Temperatur_Nu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 09:09:15.000000 Temperatur_Nu-0.0.1/Temperatur_Nu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 09:09:15.778540 Temperatur_Nu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      785 2024-04-04 09:09:00.000000 Temperatur_Nu-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 09:09:15.774355 Temperatur_Nu-0.0.1/temperaturnu/
--rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-0.0.1/temperaturnu/__init__.py
--rw-rw-rw-   0        0        0      651 2024-04-04 09:02:21.000000 Temperatur_Nu-0.0.1/temperaturnu/temperaturnu.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:43:43.560203 Temperatur_Nu-0.0.2/
+-rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      549 2024-04-04 09:43:43.558203 Temperatur_Nu-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 09:43:43.557203 Temperatur_Nu-0.0.2/Temperatur_Nu.egg-info/
+-rw-rw-rw-   0        0        0      549 2024-04-04 09:43:43.000000 Temperatur_Nu-0.0.2/Temperatur_Nu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-04 09:43:43.000000 Temperatur_Nu-0.0.2/Temperatur_Nu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 09:43:43.000000 Temperatur_Nu-0.0.2/Temperatur_Nu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-04 09:43:43.000000 Temperatur_Nu-0.0.2/Temperatur_Nu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 09:43:43.000000 Temperatur_Nu-0.0.2/Temperatur_Nu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 09:43:43.560203 Temperatur_Nu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      785 2024-04-04 09:43:11.000000 Temperatur_Nu-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 09:43:43.555200 Temperatur_Nu-0.0.2/temperaturnu/
+-rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-0.0.2/temperaturnu/__init__.py
+-rw-rw-rw-   0        0        0      733 2024-04-04 09:42:07.000000 Temperatur_Nu-0.0.2/temperaturnu/temperaturnu.py
```

### Comparing `Temperatur_Nu-0.0.1/LICENSE` & `Temperatur_Nu-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Temperatur_Nu-0.0.1/PKG-INFO` & `Temperatur_Nu-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-0.0.1/Temperatur_Nu.egg-info/PKG-INFO` & `Temperatur_Nu-0.0.2/Temperatur_Nu.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-0.0.1/setup.py` & `Temperatur_Nu-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="Temperatur_Nu",
-    version="0.0.1",
+    version="0.0.2",
     author="Patrik Johansson",
     author_email="github@popeen.com",
     description="Get and or publish temperatures to temperatur.nu",
     long_description="Get and or publish temperatures to temperatur.nu",
     long_description_content_type="text/markdown",
     url="https://github.com/popeen/PyPi-Temperatur_Nu",
     install_requires=[
```

### Comparing `Temperatur_Nu-0.0.1/temperaturnu/temperaturnu.py` & `Temperatur_Nu-0.0.2/temperaturnu/temperaturnu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import requests
 
 class TemperaturNu:
 
-    def get_temp(self, station):
+    async def get_temp(self, station):
         url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=popeensPyPi"
-        response = requests.get(url)
-        data = response.json()
-        if len(data) > 0:
-            return data['stations'][0]['temp']
-        else:
-            return None
+        async with session.get(url) as resp:
+            data = await resp.json()
+            if len(data) > 0:
+                return data['stations'][0]['temp']
+            else:
+                return None
 
-    def set_temp(self, token, temp):
+    async def set_temp(self, token, temp):
+        
         url="http://www.temperatur.nu/rapportera.php?hash=" + token + "&t=" + str(temp)
-        response = requests.get(url)
-        body = response.content
-        if str("ok!") in str(body):
-            return True
-        else:
-            return False
+        async with session.get(url) as resp:
+            body = await resp.content
+            if str("ok!") in str(body):
+                return True
+            else:
+                return False
```

