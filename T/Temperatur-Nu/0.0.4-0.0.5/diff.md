# Comparing `tmp/Temperatur_Nu-0.0.4.tar.gz` & `tmp/Temperatur_Nu-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Temperatur_Nu-0.0.4.tar", last modified: Thu Apr  4 10:17:10 2024, max compression
+gzip compressed data, was "Temperatur_Nu-0.0.5.tar", last modified: Thu Apr  4 10:25:41 2024, max compression
```

## Comparing `Temperatur_Nu-0.0.4.tar` & `Temperatur_Nu-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 10:17:10.415789 Temperatur_Nu-0.0.4/
--rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      573 2024-04-04 10:17:10.414790 Temperatur_Nu-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 10:17:10.413790 Temperatur_Nu-0.0.4/Temperatur_Nu.egg-info/
--rw-rw-rw-   0        0        0      573 2024-04-04 10:17:10.000000 Temperatur_Nu-0.0.4/Temperatur_Nu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-04-04 10:17:10.000000 Temperatur_Nu-0.0.4/Temperatur_Nu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 10:17:10.000000 Temperatur_Nu-0.0.4/Temperatur_Nu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 10:17:10.000000 Temperatur_Nu-0.0.4/Temperatur_Nu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-04 10:17:10.000000 Temperatur_Nu-0.0.4/Temperatur_Nu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 10:17:10.415789 Temperatur_Nu-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      805 2024-04-04 10:17:01.000000 Temperatur_Nu-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 10:17:10.412789 Temperatur_Nu-0.0.4/temperaturnu/
--rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-0.0.4/temperaturnu/__init__.py
--rw-rw-rw-   0        0        0      735 2024-04-04 09:48:08.000000 Temperatur_Nu-0.0.4/temperaturnu/temperaturnu.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:41.965906 Temperatur_Nu-0.0.5/
+-rw-rw-rw-   0        0        0     1073 2024-04-04 07:43:42.000000 Temperatur_Nu-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      573 2024-04-04 10:25:41.964899 Temperatur_Nu-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-01-04 23:25:24.000000 Temperatur_Nu-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:41.963395 Temperatur_Nu-0.0.5/Temperatur_Nu.egg-info/
+-rw-rw-rw-   0        0        0      573 2024-04-04 10:25:41.000000 Temperatur_Nu-0.0.5/Temperatur_Nu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-04-04 10:25:41.000000 Temperatur_Nu-0.0.5/Temperatur_Nu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:25:41.000000 Temperatur_Nu-0.0.5/Temperatur_Nu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 10:25:41.000000 Temperatur_Nu-0.0.5/Temperatur_Nu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 10:25:41.000000 Temperatur_Nu-0.0.5/Temperatur_Nu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:25:41.965906 Temperatur_Nu-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      805 2024-04-04 10:25:31.000000 Temperatur_Nu-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:41.961397 Temperatur_Nu-0.0.5/temperaturnu/
+-rw-rw-rw-   0        0        0       38 2024-04-04 08:11:59.000000 Temperatur_Nu-0.0.5/temperaturnu/__init__.py
+-rw-rw-rw-   0        0        0     1616 2024-04-04 10:25:20.000000 Temperatur_Nu-0.0.5/temperaturnu/temperaturnu.py
```

### Comparing `Temperatur_Nu-0.0.4/LICENSE` & `Temperatur_Nu-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Temperatur_Nu-0.0.4/PKG-INFO` & `Temperatur_Nu-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-0.0.4/Temperatur_Nu.egg-info/PKG-INFO` & `Temperatur_Nu-0.0.5/Temperatur_Nu.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Temperatur_Nu
-Version: 0.0.4
+Version: 0.0.5
 Summary: Get and or publish temperatures to temperatur.nu
 Home-page: https://github.com/popeen/PyPi-Temperatur_Nu
 Author: Patrik Johansson
 Author-email: github@popeen.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Temperatur_Nu-0.0.4/setup.py` & `Temperatur_Nu-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open(os.path.join(os.path.dirname(__file__), "README.md")) as readme:
     README = readme.read()
 
 setuptools.setup(
     name="Temperatur_Nu",
-    version="0.0.4",
+    version="0.0.5",
     author="Patrik Johansson",
     author_email="github@popeen.com",
     description="Get and or publish temperatures to temperatur.nu",
     long_description="Get and or publish temperatures to temperatur.nu",
     long_description_content_type="text/markdown",
     url="https://github.com/popeen/PyPi-Temperatur_Nu",
     install_requires=[
```

