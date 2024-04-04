# Comparing `tmp/Temperatur_Nu-24.4.3.tar.gz` & `tmp/Temperatur_Nu-24.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Temperatur_Nu-24.4.3.tar", last modified: Thu Apr  4 12:48:53 2024, max compression
+gzip compressed data, was "Temperatur_Nu-24.4.4.tar", last modified: Thu Apr  4 13:07:28 2024, max compression
```

## Comparing `Temperatur_Nu-24.4.3.tar` & `Temperatur_Nu-24.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 12:48:53.648312 Temperatur_Nu-24.4.3/
--rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-24.4.3/LICENSE
--rw-rw-rw-   0        0        0      574 2024-04-04 12:48:53.646309 Temperatur_Nu-24.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-24.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 12:48:53.645302 Temperatur_Nu-24.4.3/Temperatur_Nu.egg-info/
--rw-rw-rw-   0        0        0      574 2024-04-04 12:48:53.000000 Temperatur_Nu-24.4.3/Temperatur_Nu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-04 12:48:53.000000 Temperatur_Nu-24.4.3/Temperatur_Nu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 12:48:53.000000 Temperatur_Nu-24.4.3/Temperatur_Nu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 12:48:53.000000 Temperatur_Nu-24.4.3/Temperatur_Nu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 12:48:53.000000 Temperatur_Nu-24.4.3/Temperatur_Nu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 12:48:53.648312 Temperatur_Nu-24.4.3/setup.cfg
--rw-rw-rw-   0        0        0      807 2024-04-04 12:48:39.000000 Temperatur_Nu-24.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 12:48:53.643796 Temperatur_Nu-24.4.3/temperaturnu/
--rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-24.4.3/temperaturnu/__init__.py
--rw-rw-rw-   0        0        0     2402 2024-04-04 12:48:24.000000 Temperatur_Nu-24.4.3/temperaturnu/temperaturnu.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:07:28.632733 Temperatur_Nu-24.4.4/
+-rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-24.4.4/LICENSE
+-rw-rw-rw-   0        0        0      574 2024-04-04 13:07:28.630730 Temperatur_Nu-24.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-24.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 13:07:28.629723 Temperatur_Nu-24.4.4/Temperatur_Nu.egg-info/
+-rw-rw-rw-   0        0        0      574 2024-04-04 13:07:28.000000 Temperatur_Nu-24.4.4/Temperatur_Nu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-04 13:07:28.000000 Temperatur_Nu-24.4.4/Temperatur_Nu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 13:07:28.000000 Temperatur_Nu-24.4.4/Temperatur_Nu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 13:07:28.000000 Temperatur_Nu-24.4.4/Temperatur_Nu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 13:07:28.000000 Temperatur_Nu-24.4.4/Temperatur_Nu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 13:07:28.632733 Temperatur_Nu-24.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      807 2024-04-04 13:07:19.000000 Temperatur_Nu-24.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:07:28.628252 Temperatur_Nu-24.4.4/temperaturnu/
+-rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-24.4.4/temperaturnu/__init__.py
+-rw-rw-rw-   0        0        0     3152 2024-04-04 13:06:58.000000 Temperatur_Nu-24.4.4/temperaturnu/temperaturnu.py
```

### Comparing `Temperatur_Nu-24.4.3/LICENSE` & `Temperatur_Nu-24.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Temperatur_Nu-24.4.3/PKG-INFO` & `Temperatur_Nu-24.4.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 24.4.3
+Version: 24.4.4
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-24.4.3/Temperatur_Nu.egg-info/PKG-INFO` & `Temperatur_Nu-24.4.4/Temperatur_Nu.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 24.4.3
+Version: 24.4.4
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-24.4.3/setup.py` & `Temperatur_Nu-24.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="Temperatur_Nu",
-    version="24.04.3",
+    version="24.04.4",
     author="Patrik Johansson",
     author_email="github@popeen.com",
     description="Get and or publish temperatures to temperatur.nu",
     long_description="Get and or publish temperatures to temperatur.nu",
     long_description_content_type="text/markdown",
     url="https://github.com/popeen/PyPi-Temperatur_Nu",
     install_requires=[
```

### Comparing `Temperatur_Nu-24.4.3/temperaturnu/temperaturnu.py` & `Temperatur_Nu-24.4.4/temperaturnu/temperaturnu.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 import requests
 
 class TemperaturNu:
 
     def __init__(self, cli):
         self.cli = cli
 
+    
+    
+    def is_valid_id(self, station):
+        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=" + self.cli
+        response = requests.get(url)
+        data = response.json()
+        if 'stations' in data:
+            return True
+        else:
+            return False
+        
     def get_name(self, station):
         url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=" + self.cli
         response = requests.get(url)
         data = response.json()
         if len(data) > 0:
             return data['stations'][0]['title']
         else:
@@ -29,14 +40,24 @@
         response = requests.get(url)
         body = response.content
         if str("ok!") in str(body):
             return True
         else:
             return False
         
+    async def is_valid_id_async(self, station):
+        url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=" + self.cli
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url) as response:
+                data = await response.json()
+                if 'stations' in data:
+                    return True
+                else:
+                    return False
+        
     async def get_name_async(self, station):
         url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=" + self.cli
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as response:
                 data = await response.json()
                 if len(data) > 0:
                     return data['stations'][0]['title']
```

