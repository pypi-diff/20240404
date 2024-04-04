# Comparing `tmp/rm3-mio-0.0.1.tar.gz` & `tmp/rm3-mio-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rm3-mio-0.0.1.tar", last modified: Thu Apr  4 06:45:08 2024, max compression
+gzip compressed data, was "rm3-mio-0.0.2.tar", last modified: Thu Apr  4 07:10:38 2024, max compression
```

## Comparing `rm3-mio-0.0.1.tar` & `rm3-mio-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 06:45:08.174076 rm3-mio-0.0.1/
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      649 2023-03-28 06:15:56.000000 rm3-mio-0.0.1/.gitignore
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1233 2024-02-09 06:06:21.000000 rm3-mio-0.0.1/MIO.sublime-project
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1424 2024-04-04 06:45:08.174076 rm3-mio-0.0.1/PKG-INFO
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1018 2024-04-04 06:44:06.000000 rm3-mio-0.0.1/README.md
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)    38661 2024-04-04 06:10:02.000000 rm3-mio-0.0.1/icon.jpg
-drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 06:45:08.174076 rm3-mio-0.0.1/mio/
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      126 2024-04-03 19:02:05.000000 rm3-mio-0.0.1/mio/__init__.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1691 2024-04-03 18:46:51.000000 rm3-mio-0.0.1/mio/platform.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     5020 2024-04-03 18:38:39.000000 rm3-mio-0.0.1/mio/storage.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      519 2024-04-03 21:46:02.000000 rm3-mio-0.0.1/mio/struct.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     4829 2024-04-03 18:36:46.000000 rm3-mio-0.0.1/mio/terminal.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      480 2024-04-03 19:00:35.000000 rm3-mio-0.0.1/mio/web.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     2317 2024-04-04 06:13:32.000000 rm3-mio-0.0.1/mio/webscrape.py
-drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 06:45:08.174076 rm3-mio-0.0.1/rm3_mio.egg-info/
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1424 2024-04-04 06:45:08.000000 rm3-mio-0.0.1/rm3_mio.egg-info/PKG-INFO
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      287 2024-04-04 06:45:08.000000 rm3-mio-0.0.1/rm3_mio.egg-info/SOURCES.txt
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)        1 2024-04-04 06:45:08.000000 rm3-mio-0.0.1/rm3_mio.egg-info/dependency_links.txt
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)        4 2024-04-04 06:45:08.000000 rm3-mio-0.0.1/rm3_mio.egg-info/top_level.txt
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)       38 2024-04-04 06:45:08.174076 rm3-mio-0.0.1/setup.cfg
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      762 2024-04-04 06:45:03.000000 rm3-mio-0.0.1/setup.py
+drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 07:10:38.310948 rm3-mio-0.0.2/
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      669 2024-04-04 07:03:07.000000 rm3-mio-0.0.2/.gitignore
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1233 2024-02-09 06:06:21.000000 rm3-mio-0.0.2/MIO.sublime-project
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1462 2024-04-04 07:10:38.310948 rm3-mio-0.0.2/PKG-INFO
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1056 2024-04-04 07:04:37.000000 rm3-mio-0.0.2/README.md
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)    38661 2024-04-04 06:10:02.000000 rm3-mio-0.0.2/icon.jpg
+drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 07:10:38.307615 rm3-mio-0.0.2/mio/
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      126 2024-04-03 19:02:05.000000 rm3-mio-0.0.2/mio/__init__.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1691 2024-04-03 18:46:51.000000 rm3-mio-0.0.2/mio/platform.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     5020 2024-04-03 18:38:39.000000 rm3-mio-0.0.2/mio/storage.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      519 2024-04-03 21:46:02.000000 rm3-mio-0.0.2/mio/struct.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     4829 2024-04-03 18:36:46.000000 rm3-mio-0.0.2/mio/terminal.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      480 2024-04-03 19:00:35.000000 rm3-mio-0.0.2/mio/web.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     2317 2024-04-04 06:13:32.000000 rm3-mio-0.0.2/mio/webscrape.py
+drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 07:10:38.307615 rm3-mio-0.0.2/rm3_mio.egg-info/
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1462 2024-04-04 07:10:38.000000 rm3-mio-0.0.2/rm3_mio.egg-info/PKG-INFO
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      287 2024-04-04 07:10:38.000000 rm3-mio-0.0.2/rm3_mio.egg-info/SOURCES.txt
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)        1 2024-04-04 07:10:38.000000 rm3-mio-0.0.2/rm3_mio.egg-info/dependency_links.txt
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)        4 2024-04-04 07:10:38.000000 rm3-mio-0.0.2/rm3_mio.egg-info/top_level.txt
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)       38 2024-04-04 07:10:38.310948 rm3-mio-0.0.2/setup.cfg
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      764 2024-04-04 07:09:36.000000 rm3-mio-0.0.2/setup.py
```

### Comparing `rm3-mio-0.0.1/.gitignore` & `rm3-mio-0.0.2/.gitignore`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # personal ignores
 *.sublime-workspace
 SECRET.py
-
+*.egg-info
+mio-token
 
 # large build files
 static/builds/*
 deployments/
 depl/
 __pycache__/
 virt/
```

### Comparing `rm3-mio-0.0.1/MIO.sublime-project` & `rm3-mio-0.0.2/MIO.sublime-project`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.1/PKG-INFO` & `rm3-mio-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rm3-mio
-Version: 0.0.1
+Version: 0.0.2
 Summary: Personal Python Utilites
 Home-page: https://gitlab.com/RoseMaster3000/mio
 Author: Shahrose Kasim
 Author-email: rosemaster3000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Overview
-My I/O library, aka "mio." A python module filled with general purpose utilities for IO with files, console, and web fetching. 
+My I/O library, aka "mio." A python module composed of general purpose utilities for hacking together quick scripts. 
 
 
 ### Installation
 * Test local installation with `source test.sh`
 * install from PyPi using `pip install rm3-mio` 
 
 
@@ -26,16 +26,16 @@
 * Struct (working with data structures)
 * Terminal (inputting / outputting text on the console)
 * Web (fetch resources from the internet)
 
 
 ### PyPi Instructions
 1. Make an account [here](https://pypi.org/)
-2. Build project `python3 setup.py sdist bdist_wheel`
-3. 
+2. Generate API token [here](https://pypi.org/manage/account/token/)
+3. Upload project `source upload.sh`
 
 
 # Author
 | Shahrose Kasim |             |
 |----------------|-------------|
 |*[shahros3@gmail.com](mailto:shahros3@gmail.com)*|[shahrose.com](http://shahrose.com)|
 |*[rosemaster3000@gmail.com](mailto:rosemaster3000@gmail.com)*|[florasoft.live](https://florasoft.live) |
```

### Comparing `rm3-mio-0.0.1/README.md` & `rm3-mio-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Overview
-My I/O library, aka "mio." A python module filled with general purpose utilities for IO with files, console, and web fetching. 
+My I/O library, aka "mio." A python module composed of general purpose utilities for hacking together quick scripts. 
 
 
 ### Installation
 * Test local installation with `source test.sh`
 * install from PyPi using `pip install rm3-mio` 
 
 
@@ -13,16 +13,16 @@
 * Struct (working with data structures)
 * Terminal (inputting / outputting text on the console)
 * Web (fetch resources from the internet)
 
 
 ### PyPi Instructions
 1. Make an account [here](https://pypi.org/)
-2. Build project `python3 setup.py sdist bdist_wheel`
-3. 
+2. Generate API token [here](https://pypi.org/manage/account/token/)
+3. Upload project `source upload.sh`
 
 
 # Author
 | Shahrose Kasim |             |
 |----------------|-------------|
 |*[shahros3@gmail.com](mailto:shahros3@gmail.com)*|[shahrose.com](http://shahrose.com)|
 |*[rosemaster3000@gmail.com](mailto:rosemaster3000@gmail.com)*|[florasoft.live](https://florasoft.live) |
```

### Comparing `rm3-mio-0.0.1/icon.jpg` & `rm3-mio-0.0.2/icon.jpg`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.1/mio/platform.py` & `rm3-mio-0.0.2/mio/platform.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.1/mio/storage.py` & `rm3-mio-0.0.2/mio/storage.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.1/mio/struct.py` & `rm3-mio-0.0.2/mio/struct.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.1/mio/terminal.py` & `rm3-mio-0.0.2/mio/terminal.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.1/mio/webscrape.py` & `rm3-mio-0.0.2/mio/webscrape.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.1/rm3_mio.egg-info/PKG-INFO` & `rm3-mio-0.0.2/rm3_mio.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rm3-mio
-Version: 0.0.1
+Version: 0.0.2
 Summary: Personal Python Utilites
 Home-page: https://gitlab.com/RoseMaster3000/mio
 Author: Shahrose Kasim
 Author-email: rosemaster3000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Overview
-My I/O library, aka "mio." A python module filled with general purpose utilities for IO with files, console, and web fetching. 
+My I/O library, aka "mio." A python module composed of general purpose utilities for hacking together quick scripts. 
 
 
 ### Installation
 * Test local installation with `source test.sh`
 * install from PyPi using `pip install rm3-mio` 
 
 
@@ -26,16 +26,16 @@
 * Struct (working with data structures)
 * Terminal (inputting / outputting text on the console)
 * Web (fetch resources from the internet)
 
 
 ### PyPi Instructions
 1. Make an account [here](https://pypi.org/)
-2. Build project `python3 setup.py sdist bdist_wheel`
-3. 
+2. Generate API token [here](https://pypi.org/manage/account/token/)
+3. Upload project `source upload.sh`
 
 
 # Author
 | Shahrose Kasim |             |
 |----------------|-------------|
 |*[shahros3@gmail.com](mailto:shahros3@gmail.com)*|[shahrose.com](http://shahrose.com)|
 |*[rosemaster3000@gmail.com](mailto:rosemaster3000@gmail.com)*|[florasoft.live](https://florasoft.live) |
```

### Comparing `rm3-mio-0.0.1/setup.py` & `rm3-mio-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
-with open("README.md", "r", encoding = "utf-8") as fh:
-    long_description = fh.read()
+with open("README.md", "r", encoding = "utf-8") as f:
+    long_description = f.read()
 
 setuptools.setup(
     # Titles
     name = "rm3-mio",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Shahrose Kasim",
     author_email = "rosemaster3000@gmail.com",
     url = "https://gitlab.com/RoseMaster3000/mio",
-
+    
     # Description
     description = "Personal Python Utilites",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     
     # Configs
     classifiers = [
```

