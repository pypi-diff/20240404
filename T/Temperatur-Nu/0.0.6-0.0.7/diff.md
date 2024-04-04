# Comparing `tmp/Temperatur_Nu-0.0.6.tar.gz` & `tmp/Temperatur_Nu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Temperatur_Nu-0.0.6.tar", last modified: Thu Apr  4 10:29:53 2024, max compression
+gzip compressed data, was "Temperatur_Nu-0.0.7.tar", last modified: Thu Apr  4 10:33:17 2024, max compression
```

## Comparing `Temperatur_Nu-0.0.6.tar` & `Temperatur_Nu-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:29:53.644515 Temperatur_Nu-0.0.6/
--rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      573 2024-04-04 10:29:53.642514 Temperatur_Nu-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 10:29:53.641513 Temperatur_Nu-0.0.6/Temperatur_Nu.egg-info/
--rw-rw-rw-   0        0        0      573 2024-04-04 10:29:53.000000 Temperatur_Nu-0.0.6/Temperatur_Nu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-04 10:29:53.000000 Temperatur_Nu-0.0.6/Temperatur_Nu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:29:53.000000 Temperatur_Nu-0.0.6/Temperatur_Nu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 10:29:53.000000 Temperatur_Nu-0.0.6/Temperatur_Nu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 10:29:53.000000 Temperatur_Nu-0.0.6/Temperatur_Nu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 10:29:53.644515 Temperatur_Nu-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      805 2024-04-04 10:29:44.000000 Temperatur_Nu-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:29:53.639519 Temperatur_Nu-0.0.6/temperaturnu/
--rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-0.0.6/temperaturnu/__init__.py
--rw-rw-rw-   0        0        0     1628 2024-04-04 10:29:29.000000 Temperatur_Nu-0.0.6/temperaturnu/temperaturnu.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:33:17.323884 Temperatur_Nu-0.0.7/
+-rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      573 2024-04-04 10:33:17.321884 Temperatur_Nu-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:33:17.320886 Temperatur_Nu-0.0.7/Temperatur_Nu.egg-info/
+-rw-rw-rw-   0        0        0      573 2024-04-04 10:33:17.000000 Temperatur_Nu-0.0.7/Temperatur_Nu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-04 10:33:17.000000 Temperatur_Nu-0.0.7/Temperatur_Nu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:33:17.000000 Temperatur_Nu-0.0.7/Temperatur_Nu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 10:33:17.000000 Temperatur_Nu-0.0.7/Temperatur_Nu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 10:33:17.000000 Temperatur_Nu-0.0.7/Temperatur_Nu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:33:17.323884 Temperatur_Nu-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-04 10:33:12.000000 Temperatur_Nu-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:33:17.318916 Temperatur_Nu-0.0.7/temperaturnu/
+-rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-0.0.7/temperaturnu/__init__.py
+-rw-rw-rw-   0        0        0     1586 2024-04-04 10:32:56.000000 Temperatur_Nu-0.0.7/temperaturnu/temperaturnu.py
```

### Comparing `Temperatur_Nu-0.0.6/LICENSE` & `Temperatur_Nu-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Temperatur_Nu-0.0.6/PKG-INFO` & `Temperatur_Nu-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 0.0.6
+Version: 0.0.7
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-0.0.6/Temperatur_Nu.egg-info/PKG-INFO` & `Temperatur_Nu-0.0.7/Temperatur_Nu.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 0.0.6
+Version: 0.0.7
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-0.0.6/setup.py` & `Temperatur_Nu-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="Temperatur_Nu",
-    version="0.0.6",
+    version="0.0.7",
     author="Patrik Johansson",
     author_email="github@popeen.com",
     description="Get and or publish temperatures to temperatur.nu",
     long_description="Get and or publish temperatures to temperatur.nu",
     long_description_content_type="text/markdown",
     url="https://github.com/popeen/PyPi-Temperatur_Nu",
     install_requires=[
```

### Comparing `Temperatur_Nu-0.0.6/temperaturnu/temperaturnu.py` & `Temperatur_Nu-0.0.7/temperaturnu/temperaturnu.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,26 @@
             return True
         else:
             return False
         
     async def get_temp_async(self, station):
         url = "http://api.temperatur.nu/tnu_1.17.php?p=" + station + "&cli=popeensPyPi"
         async with aiohttp.ClientSession() as session:
-            async with session.get('http://httpbin.org/get') as response:
+            async with session.get(url) as response:
                 data = await response.json()
                 if len(data) > 0:
                     return data['stations'][0]['temp']
                 else:
                     return None
         
 
     async def set_temp_async(self, token, temp):
         
         url="http://www.temperatur.nu/rapportera.php?hash=" + token + "&t=" + str(temp)
         async with aiohttp.ClientSession() as session:
-            async with session.get('http://httpbin.org/get') as response:
+            async with session.get(url) as response:
                 body = await response.content
                 if str("ok!") in str(body):
                     return True
                 else:
                     return False
```

