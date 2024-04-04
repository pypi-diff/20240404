# Comparing `tmp/wasdi-0.8.6.2.tar.gz` & `tmp/wasdi-0.8.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasdi-0.8.6.2.tar", last modified: Mon Mar  4 10:10:44 2024, max compression
+gzip compressed data, was "wasdi-0.8.6.3.tar", last modified: Thu Apr  4 16:20:23 2024, max compression
```

## Comparing `wasdi-0.8.6.2.tar` & `wasdi-0.8.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 10:10:44.808417 wasdi-0.8.6.2/
--rw-rw-rw-   0        0        0     1063 2023-01-25 18:34:50.000000 wasdi-0.8.6.2/LICENSE
--rw-rw-rw-   0        0        0    19253 2024-03-04 10:10:44.805417 wasdi-0.8.6.2/PKG-INFO
--rw-rw-rw-   0        0        0    14905 2023-01-25 18:34:50.000000 wasdi-0.8.6.2/README.md
--rw-rw-rw-   0        0        0       42 2024-03-04 10:10:44.809415 wasdi-0.8.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1538 2024-03-04 10:09:39.000000 wasdi-0.8.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-04 10:10:44.763419 wasdi-0.8.6.2/test/
--rw-rw-rw-   0        0        0    10190 2023-01-25 18:34:50.000000 wasdi-0.8.6.2/test/testSearchEOImages.py
-drwxrwxrwx   0        0        0        0 2024-03-04 10:10:44.777420 wasdi-0.8.6.2/wasdi/
--rw-rw-rw-   0        0        0   170253 2024-03-04 10:09:21.000000 wasdi-0.8.6.2/wasdi/__init__.py
--rw-rw-rw-   0        0        0     1899 2020-06-26 18:34:48.000000 wasdi-0.8.6.2/wasdi/waspyLogFormatter.py
-drwxrwxrwx   0        0        0        0 2024-03-04 10:10:44.803419 wasdi-0.8.6.2/wasdi.egg-info/
--rw-rw-rw-   0        0        0    19253 2024-03-04 10:10:44.000000 wasdi-0.8.6.2/wasdi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-03-04 10:10:44.000000 wasdi-0.8.6.2/wasdi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 10:10:44.000000 wasdi-0.8.6.2/wasdi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-04 10:10:44.000000 wasdi-0.8.6.2/wasdi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-04 10:10:44.000000 wasdi-0.8.6.2/wasdi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 16:20:23.199145 wasdi-0.8.6.3/
+-rw-rw-rw-   0        0        0     1063 2023-01-25 18:34:50.000000 wasdi-0.8.6.3/LICENSE
+-rw-rw-rw-   0        0        0    19231 2024-04-04 16:20:23.198863 wasdi-0.8.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0    14905 2023-01-25 18:34:50.000000 wasdi-0.8.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 16:20:23.199718 wasdi-0.8.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1540 2024-04-04 16:20:16.000000 wasdi-0.8.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:20:23.183617 wasdi-0.8.6.3/test/
+-rw-rw-rw-   0        0        0    10190 2023-01-25 18:34:50.000000 wasdi-0.8.6.3/test/testSearchEOImages.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:20:23.190831 wasdi-0.8.6.3/wasdi/
+-rw-rw-rw-   0        0        0   170253 2024-04-04 16:03:12.000000 wasdi-0.8.6.3/wasdi/__init__.py
+-rw-rw-rw-   0        0        0     1899 2020-06-26 18:34:48.000000 wasdi-0.8.6.3/wasdi/waspyLogFormatter.py
+drwxrwxrwx   0        0        0        0 2024-04-04 16:20:23.196944 wasdi-0.8.6.3/wasdi.egg-info/
+-rw-rw-rw-   0        0        0    19231 2024-04-04 16:20:23.000000 wasdi-0.8.6.3/wasdi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-04 16:20:23.000000 wasdi-0.8.6.3/wasdi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 16:20:23.000000 wasdi-0.8.6.3/wasdi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-04 16:20:23.000000 wasdi-0.8.6.3/wasdi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-04 16:20:23.000000 wasdi-0.8.6.3/wasdi.egg-info/top_level.txt
```

### Comparing `wasdi-0.8.6.2/LICENSE` & `wasdi-0.8.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wasdi-0.8.6.2/PKG-INFO` & `wasdi-0.8.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: wasdi
-Version: 0.8.6.2
+Version: 0.8.6.3
 Summary: The WASDI Python library
 Home-page: https://www.wasdi.net
 Author: WASDI Sarl
 Author-email: info@wasdi.cloud
-License: UNKNOWN
+License: CC-BY License
 Project-URL: Source, https://github.com/fadeoutsoftware/WASDI/tree/develop/libraries/waspy
 Project-URL: Tracker, https://github.com/fadeoutsoftware/WASDI/issues
 Description: # WASDI Python Library
         
         WASDI is the Web Advanced Space Developer Interface. This software is a **preliminary version** of the Python Library you can use to access the [WASDI](http://www.wasdi.net) platform functionalities from your Python code.
         
         Visit us at [http://www.wasdi.net](http://www.wasdi.net)
@@ -420,15 +420,15 @@
         ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `wasdi-0.8.6.2/README.md` & `wasdi-0.8.6.3/README.md`

 * *Files identical despite different names*

### Comparing `wasdi-0.8.6.2/setup.py` & `wasdi-0.8.6.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,31 +10,32 @@
 import io
 
 with io.open("README.md", "r", encoding="utf8") as oFh:
     sLong_description = oFh.read()
 
 setuptools.setup(
     name="wasdi",
-    version="0.8.6.2",
+    version="0.8.6.3",
     author="WASDI Sarl",
     author_email="info@wasdi.cloud",
     description="The WASDI Python library",
     long_description=sLong_description,
     long_description_content_type="text/markdown",
     url="https://www.wasdi.net",
     packages=setuptools.find_packages(),
+    license='CC-BY License',
     install_requires=[
         'requests',
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Atmospheric Science",
         "Topic :: Scientific/Engineering :: GIS",
         "Topic :: Scientific/Engineering :: Image Processing",
         "Topic :: Software Development :: Libraries"
```

### Comparing `wasdi-0.8.6.2/test/testSearchEOImages.py` & `wasdi-0.8.6.3/test/testSearchEOImages.py`

 * *Files identical despite different names*

### Comparing `wasdi-0.8.6.2/wasdi/__init__.py` & `wasdi-0.8.6.3/wasdi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 Note:
 the philosophy of safe programming is adopted as widely as possible, the lib will try to workaround issues such as
 faulty input, and print an error rather than raise an exception, so that your program can possibly go on. Please check
 the return statues
 
 Version 0.8.6.3
 
-Last Update: 04/03/2024
+Last Update: 19/03/2024
 
 Tested with: Python 3.7, Python 3.8, Python 3.9, Python 3.10
 
 Created on 11 Jun 2018
 
 @author: p.campanella
 """
```

### Comparing `wasdi-0.8.6.2/wasdi/waspyLogFormatter.py` & `wasdi-0.8.6.3/wasdi/waspyLogFormatter.py`

 * *Files identical despite different names*

### Comparing `wasdi-0.8.6.2/wasdi.egg-info/PKG-INFO` & `wasdi-0.8.6.3/wasdi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: wasdi
-Version: 0.8.6.2
+Version: 0.8.6.3
 Summary: The WASDI Python library
 Home-page: https://www.wasdi.net
 Author: WASDI Sarl
 Author-email: info@wasdi.cloud
-License: UNKNOWN
+License: CC-BY License
 Project-URL: Source, https://github.com/fadeoutsoftware/WASDI/tree/develop/libraries/waspy
 Project-URL: Tracker, https://github.com/fadeoutsoftware/WASDI/issues
 Description: # WASDI Python Library
         
         WASDI is the Web Advanced Space Developer Interface. This software is a **preliminary version** of the Python Library you can use to access the [WASDI](http://www.wasdi.net) platform functionalities from your Python code.
         
         Visit us at [http://www.wasdi.net](http://www.wasdi.net)
@@ -420,15 +420,15 @@
         ```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Software Development :: Libraries
```

