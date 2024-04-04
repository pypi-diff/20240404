# Comparing `tmp/Temperatur_Nu-24.4.1.tar.gz` & `tmp/Temperatur_Nu-24.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Temperatur_Nu-24.4.1.tar", last modified: Thu Apr  4 11:52:48 2024, max compression
+gzip compressed data, was "Temperatur_Nu-24.4.2.tar", last modified: Thu Apr  4 12:40:04 2024, max compression
```

## Comparing `Temperatur_Nu-24.4.1.tar` & `Temperatur_Nu-24.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:52:48.628572 Temperatur_Nu-24.4.1/
--rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-24.4.1/LICENSE
--rw-rw-rw-   0        0        0      574 2024-04-04 11:52:48.626571 Temperatur_Nu-24.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-24.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 11:52:48.625572 Temperatur_Nu-24.4.1/Temperatur_Nu.egg-info/
--rw-rw-rw-   0        0        0      574 2024-04-04 11:52:48.000000 Temperatur_Nu-24.4.1/Temperatur_Nu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-04 11:52:48.000000 Temperatur_Nu-24.4.1/Temperatur_Nu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:52:48.000000 Temperatur_Nu-24.4.1/Temperatur_Nu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 11:52:48.000000 Temperatur_Nu-24.4.1/Temperatur_Nu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 11:52:48.000000 Temperatur_Nu-24.4.1/Temperatur_Nu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 11:52:48.628572 Temperatur_Nu-24.4.1/setup.cfg
--rw-rw-rw-   0        0        0      807 2024-04-04 11:52:28.000000 Temperatur_Nu-24.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:52:48.624585 Temperatur_Nu-24.4.1/temperaturnu/
--rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-24.4.1/temperaturnu/__init__.py
--rw-rw-rw-   0        0        0     2346 2024-04-04 11:20:06.000000 Temperatur_Nu-24.4.1/temperaturnu/temperaturnu.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:40:04.725591 Temperatur_Nu-24.4.2/
+-rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-24.4.2/LICENSE
+-rw-rw-rw-   0        0        0      574 2024-04-04 12:40:04.724590 Temperatur_Nu-24.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-24.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:40:04.723584 Temperatur_Nu-24.4.2/Temperatur_Nu.egg-info/
+-rw-rw-rw-   0        0        0      574 2024-04-04 12:40:04.000000 Temperatur_Nu-24.4.2/Temperatur_Nu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-04 12:40:04.000000 Temperatur_Nu-24.4.2/Temperatur_Nu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:40:04.000000 Temperatur_Nu-24.4.2/Temperatur_Nu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 12:40:04.000000 Temperatur_Nu-24.4.2/Temperatur_Nu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 12:40:04.000000 Temperatur_Nu-24.4.2/Temperatur_Nu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:40:04.726591 Temperatur_Nu-24.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      807 2024-04-04 12:39:11.000000 Temperatur_Nu-24.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:40:04.722077 Temperatur_Nu-24.4.2/temperaturnu/
+-rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-24.4.2/temperaturnu/__init__.py
+-rw-rw-rw-   0        0        0     2396 2024-04-04 12:15:06.000000 Temperatur_Nu-24.4.2/temperaturnu/temperaturnu.py
```

### Comparing `Temperatur_Nu-24.4.1/LICENSE` & `Temperatur_Nu-24.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Temperatur_Nu-24.4.1/PKG-INFO` & `Temperatur_Nu-24.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 24.4.1
+Version: 24.4.2
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-24.4.1/Temperatur_Nu.egg-info/PKG-INFO` & `Temperatur_Nu-24.4.2/Temperatur_Nu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 24.4.1
+Version: 24.4.2
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-24.4.1/setup.py` & `Temperatur_Nu-24.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="Temperatur_Nu",
-    version="24.04.1",
+    version="24.04.2",
     author="Patrik Johansson",
     author_email="github@popeen.com",
     description="Get and or publish temperatures to temperatur.nu",
     long_description="Get and or publish temperatures to temperatur.nu",
     long_description_content_type="text/markdown",
     url="https://github.com/popeen/PyPi-Temperatur_Nu",
     install_requires=[
```

### Comparing `Temperatur_Nu-24.4.1/temperaturnu/temperaturnu.py` & `Temperatur_Nu-24.4.2/temperaturnu/temperaturnu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import aiohttp
 import requests
 
 class TemperaturNu:
 
+    def __init__(cli):
+        self.cli = cli
+
     def get_name(self, station):
-        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=popeensPyPi"
+        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=" + self.cli
         response = requests.get(url)
         data = response.json()
         if len(data) > 0:
             return data['stations'][0]['title']
         else:
             return None
 
     def get_temp(self, station):
-        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=popeensPyPi"
+        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=" + self.cli
         response = requests.get(url)
         data = response.json()
         if len(data) > 0:
             return data['stations'][0]['temp']
         else:
             return None
 
@@ -27,25 +30,25 @@
         body = response.content
         if str("ok!") in str(body):
             return True
         else:
             return False
         
     async def get_name_async(self, station):
-        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=popeensPyPi"
+        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=" + self.cli
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as response:
                 data = await response.json()
                 if len(data) > 0:
                     return data['stations'][0]['title']
                 else:
                     return None
         
     async def get_temp_async(self, station):
-        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=popeensPyPi"
+        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=" + self.cli
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as response:
                 data = await response.json()
                 if len(data) > 0:
                     return data['stations'][0]['temp']
                 else:
                     return None
```

