# Comparing `tmp/rm3-mio-0.0.2.tar.gz` & `tmp/rm3-mio-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rm3-mio-0.0.2.tar", last modified: Thu Apr  4 07:10:38 2024, max compression
+gzip compressed data, was "rm3-mio-0.0.3.tar", last modified: Thu Apr  4 08:26:16 2024, max compression
```

## Comparing `rm3-mio-0.0.2.tar` & `rm3-mio-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 07:10:38.310948 rm3-mio-0.0.2/
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      669 2024-04-04 07:03:07.000000 rm3-mio-0.0.2/.gitignore
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1233 2024-02-09 06:06:21.000000 rm3-mio-0.0.2/MIO.sublime-project
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1462 2024-04-04 07:10:38.310948 rm3-mio-0.0.2/PKG-INFO
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1056 2024-04-04 07:04:37.000000 rm3-mio-0.0.2/README.md
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)    38661 2024-04-04 06:10:02.000000 rm3-mio-0.0.2/icon.jpg
-drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 07:10:38.307615 rm3-mio-0.0.2/mio/
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      126 2024-04-03 19:02:05.000000 rm3-mio-0.0.2/mio/__init__.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1691 2024-04-03 18:46:51.000000 rm3-mio-0.0.2/mio/platform.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     5020 2024-04-03 18:38:39.000000 rm3-mio-0.0.2/mio/storage.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      519 2024-04-03 21:46:02.000000 rm3-mio-0.0.2/mio/struct.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     4829 2024-04-03 18:36:46.000000 rm3-mio-0.0.2/mio/terminal.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      480 2024-04-03 19:00:35.000000 rm3-mio-0.0.2/mio/web.py
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     2317 2024-04-04 06:13:32.000000 rm3-mio-0.0.2/mio/webscrape.py
-drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 07:10:38.307615 rm3-mio-0.0.2/rm3_mio.egg-info/
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1462 2024-04-04 07:10:38.000000 rm3-mio-0.0.2/rm3_mio.egg-info/PKG-INFO
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      287 2024-04-04 07:10:38.000000 rm3-mio-0.0.2/rm3_mio.egg-info/SOURCES.txt
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)        1 2024-04-04 07:10:38.000000 rm3-mio-0.0.2/rm3_mio.egg-info/dependency_links.txt
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)        4 2024-04-04 07:10:38.000000 rm3-mio-0.0.2/rm3_mio.egg-info/top_level.txt
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)       38 2024-04-04 07:10:38.310948 rm3-mio-0.0.2/setup.cfg
--rw-r--r--   0 shahrose  (1000) shahrose  (1001)      764 2024-04-04 07:09:36.000000 rm3-mio-0.0.2/setup.py
+drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 08:26:16.841400 rm3-mio-0.0.3/
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      676 2024-04-04 07:13:55.000000 rm3-mio-0.0.3/.gitignore
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1233 2024-02-09 06:06:21.000000 rm3-mio-0.0.3/MIO.sublime-project
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1603 2024-04-04 08:26:16.841400 rm3-mio-0.0.3/PKG-INFO
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1197 2024-04-04 07:23:35.000000 rm3-mio-0.0.3/README.md
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)    38661 2024-04-04 06:10:02.000000 rm3-mio-0.0.3/icon.jpg
+drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 08:26:16.838067 rm3-mio-0.0.3/mio/
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      126 2024-04-03 19:02:05.000000 rm3-mio-0.0.3/mio/__init__.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1691 2024-04-03 18:46:51.000000 rm3-mio-0.0.3/mio/platform.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     5020 2024-04-03 18:38:39.000000 rm3-mio-0.0.3/mio/storage.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      519 2024-04-03 21:46:02.000000 rm3-mio-0.0.3/mio/struct.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     4829 2024-04-03 18:36:46.000000 rm3-mio-0.0.3/mio/terminal.py
+drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 08:26:16.838067 rm3-mio-0.0.3/mio/tests/
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      326 2024-04-04 05:45:32.000000 rm3-mio-0.0.3/mio/tests/test_web.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      480 2024-04-03 19:00:35.000000 rm3-mio-0.0.3/mio/web.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     2442 2024-04-04 08:25:16.000000 rm3-mio-0.0.3/mio/webscrape.py
+drwxr-xr-x   0 shahrose  (1000) shahrose  (1001)        0 2024-04-04 08:26:16.841400 rm3-mio-0.0.3/rm3_mio.egg-info/
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)     1603 2024-04-04 08:26:16.000000 rm3-mio-0.0.3/rm3_mio.egg-info/PKG-INFO
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      327 2024-04-04 08:26:16.000000 rm3-mio-0.0.3/rm3_mio.egg-info/SOURCES.txt
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)        1 2024-04-04 08:26:16.000000 rm3-mio-0.0.3/rm3_mio.egg-info/dependency_links.txt
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)        4 2024-04-04 08:26:16.000000 rm3-mio-0.0.3/rm3_mio.egg-info/top_level.txt
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)       38 2024-04-04 08:26:16.841400 rm3-mio-0.0.3/setup.cfg
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      764 2024-04-04 08:25:20.000000 rm3-mio-0.0.3/setup.py
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      167 2024-04-04 06:49:21.000000 rm3-mio-0.0.3/test.sh
+-rw-r--r--   0 shahrose  (1000) shahrose  (1001)      173 2024-04-04 08:26:09.000000 rm3-mio-0.0.3/upload.sh
```

### Comparing `rm3-mio-0.0.2/.gitignore` & `rm3-mio-0.0.3/.gitignore`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # large build files
 static/builds/*
 deployments/
 depl/
 __pycache__/
 virt/
+virt2/
 build/
 dist/
 
 
 # password files
 credentials/*
 *.pem
```

### Comparing `rm3-mio-0.0.2/MIO.sublime-project` & `rm3-mio-0.0.3/MIO.sublime-project`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.2/PKG-INFO` & `rm3-mio-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rm3-mio
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personal Python Utilites
 Home-page: https://gitlab.com/RoseMaster3000/mio
 Author: Shahrose Kasim
 Author-email: rosemaster3000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,30 +13,30 @@
 
 # Overview
 My I/O library, aka "mio." A python module composed of general purpose utilities for hacking together quick scripts. 
 
 
 ### Installation
 * Test local installation with `source test.sh`
-* install from PyPi using `pip install rm3-mio` 
+* install from [PyPi](https://pypi.org/project/rm3-mio/) using `pip install rm3-mio` 
 
 
 ### Modules
 * Platform (system threading, shell commands, popups)
 * Storage (reading / writing files and directories)
 * Struct (working with data structures)
 * Terminal (inputting / outputting text on the console)
 * Web (fetch resources from the internet)
 
 
 ### PyPi Instructions
-1. Make an account [here](https://pypi.org/)
+1. Make an account [here](https://pypi.org/account/register/)
 2. Generate API token [here](https://pypi.org/manage/account/token/)
 3. Upload project `source upload.sh`
-
+4. Implement a [CI pipeline](https://docs.gitlab.com/ee/user/packages/pypi_repository/)
 
 # Author
 | Shahrose Kasim |             |
 |----------------|-------------|
 |*[shahros3@gmail.com](mailto:shahros3@gmail.com)*|[shahrose.com](http://shahrose.com)|
 |*[rosemaster3000@gmail.com](mailto:rosemaster3000@gmail.com)*|[florasoft.live](https://florasoft.live) |
 |*[RoseMaster#3000](https://discordapp.com/users/122224041296789508)*|[discord.com](https://discord.com/)|
```

### Comparing `rm3-mio-0.0.2/README.md` & `rm3-mio-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # Overview
 My I/O library, aka "mio." A python module composed of general purpose utilities for hacking together quick scripts. 
 
 
 ### Installation
 * Test local installation with `source test.sh`
-* install from PyPi using `pip install rm3-mio` 
+* install from [PyPi](https://pypi.org/project/rm3-mio/) using `pip install rm3-mio` 
 
 
 ### Modules
 * Platform (system threading, shell commands, popups)
 * Storage (reading / writing files and directories)
 * Struct (working with data structures)
 * Terminal (inputting / outputting text on the console)
 * Web (fetch resources from the internet)
 
 
 ### PyPi Instructions
-1. Make an account [here](https://pypi.org/)
+1. Make an account [here](https://pypi.org/account/register/)
 2. Generate API token [here](https://pypi.org/manage/account/token/)
 3. Upload project `source upload.sh`
-
+4. Implement a [CI pipeline](https://docs.gitlab.com/ee/user/packages/pypi_repository/)
 
 # Author
 | Shahrose Kasim |             |
 |----------------|-------------|
 |*[shahros3@gmail.com](mailto:shahros3@gmail.com)*|[shahrose.com](http://shahrose.com)|
 |*[rosemaster3000@gmail.com](mailto:rosemaster3000@gmail.com)*|[florasoft.live](https://florasoft.live) |
 |*[RoseMaster#3000](https://discordapp.com/users/122224041296789508)*|[discord.com](https://discord.com/)|
```

### Comparing `rm3-mio-0.0.2/icon.jpg` & `rm3-mio-0.0.3/icon.jpg`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.2/mio/platform.py` & `rm3-mio-0.0.3/mio/platform.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.2/mio/storage.py` & `rm3-mio-0.0.3/mio/storage.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.2/mio/struct.py` & `rm3-mio-0.0.3/mio/struct.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.2/mio/terminal.py` & `rm3-mio-0.0.3/mio/terminal.py`

 * *Files identical despite different names*

### Comparing `rm3-mio-0.0.2/mio/webscrape.py` & `rm3-mio-0.0.3/mio/webscrape.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
 
 # scroll to specific text on page
 def scrollToText(driver, text):
     element = driver.find_element("xpath", f"//*[text()[contains(., '{text}')]]")
     scrollToElement(driver, element)
 
+# get preceeding element in HTML tree
+def next(element):
+    return element.find_element(By.XPATH, "./following-sibling::*")
 
 # example Selenium usage
 if __name__=="__main__":
     driver = makeDriver(headless=False)
     driver.get("https://google.com")
 
     e = driver.find_element(By.CLASS_NAME, "class_name") # class="class_name"
```

### Comparing `rm3-mio-0.0.2/rm3_mio.egg-info/PKG-INFO` & `rm3-mio-0.0.3/rm3_mio.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rm3-mio
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personal Python Utilites
 Home-page: https://gitlab.com/RoseMaster3000/mio
 Author: Shahrose Kasim
 Author-email: rosemaster3000@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,30 +13,30 @@
 
 # Overview
 My I/O library, aka "mio." A python module composed of general purpose utilities for hacking together quick scripts. 
 
 
 ### Installation
 * Test local installation with `source test.sh`
-* install from PyPi using `pip install rm3-mio` 
+* install from [PyPi](https://pypi.org/project/rm3-mio/) using `pip install rm3-mio` 
 
 
 ### Modules
 * Platform (system threading, shell commands, popups)
 * Storage (reading / writing files and directories)
 * Struct (working with data structures)
 * Terminal (inputting / outputting text on the console)
 * Web (fetch resources from the internet)
 
 
 ### PyPi Instructions
-1. Make an account [here](https://pypi.org/)
+1. Make an account [here](https://pypi.org/account/register/)
 2. Generate API token [here](https://pypi.org/manage/account/token/)
 3. Upload project `source upload.sh`
-
+4. Implement a [CI pipeline](https://docs.gitlab.com/ee/user/packages/pypi_repository/)
 
 # Author
 | Shahrose Kasim |             |
 |----------------|-------------|
 |*[shahros3@gmail.com](mailto:shahros3@gmail.com)*|[shahrose.com](http://shahrose.com)|
 |*[rosemaster3000@gmail.com](mailto:rosemaster3000@gmail.com)*|[florasoft.live](https://florasoft.live) |
 |*[RoseMaster#3000](https://discordapp.com/users/122224041296789508)*|[discord.com](https://discord.com/)|
```

### Comparing `rm3-mio-0.0.2/setup.py` & `rm3-mio-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding = "utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     # Titles
     name = "rm3-mio",
-    version = "0.0.2",
+    version = "0.0.3",
     author = "Shahrose Kasim",
     author_email = "rosemaster3000@gmail.com",
     url = "https://gitlab.com/RoseMaster3000/mio",
     
     # Description
     description = "Personal Python Utilites",
     long_description = long_description,
```

