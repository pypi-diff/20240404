# Comparing `tmp/pixlr_private_api-0.1.1.tar.gz` & `tmp/pixlr_private_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixlr_private_api-0.1.1.tar", last modified: Thu Apr  4 03:03:52 2024, max compression
+gzip compressed data, was "pixlr_private_api-0.1.2.tar", last modified: Thu Apr  4 03:26:52 2024, max compression
```

## Comparing `pixlr_private_api-0.1.1.tar` & `pixlr_private_api-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:03:52.405807 pixlr_private_api-0.1.1/
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     1069 2024-04-01 06:31:04.000000 pixlr_private_api-0.1.1/LICENCE.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     4954 2024-04-04 03:03:52.405807 pixlr_private_api-0.1.1/PKG-INFO
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     3921 2024-04-01 08:53:23.000000 pixlr_private_api-0.1.1/README.md
-drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:03:52.403807 pixlr_private_api-0.1.1/pixlr_private_api/
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-01 06:31:04.000000 pixlr_private_api-0.1.1/pixlr_private_api/__init__.py
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)    18763 2024-04-01 08:50:37.000000 pixlr_private_api-0.1.1/pixlr_private_api/main.py
-drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:03:52.405807 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     4954 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/PKG-INFO
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)      290 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/SOURCES.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)        1 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/dependency_links.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       27 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/requires.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       18 2024-04-04 03:03:52.000000 pixlr_private_api-0.1.1/pixlr_private_api.egg-info/top_level.txt
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       38 2024-04-04 03:03:52.405807 pixlr_private_api-0.1.1/setup.cfg
--rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     1184 2024-04-04 03:03:31.000000 pixlr_private_api-0.1.1/setup.py
+drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:26:52.331022 pixlr_private_api-0.1.2/
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     1069 2024-04-01 06:31:04.000000 pixlr_private_api-0.1.2/LICENCE.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     4976 2024-04-04 03:26:52.331022 pixlr_private_api-0.1.2/PKG-INFO
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     3921 2024-04-01 08:53:23.000000 pixlr_private_api-0.1.2/README.md
+drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:26:52.330022 pixlr_private_api-0.1.2/pixlr_private_api/
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-01 06:31:04.000000 pixlr_private_api-0.1.2/pixlr_private_api/__init__.py
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)    18763 2024-04-01 08:50:37.000000 pixlr_private_api-0.1.2/pixlr_private_api/main.py
+drwxr-xr-x   0 adoniscodes  (1000) adoniscodes  (1000)        0 2024-04-04 03:26:52.331022 pixlr_private_api-0.1.2/pixlr_private_api.egg-info/
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     4976 2024-04-04 03:26:52.000000 pixlr_private_api-0.1.2/pixlr_private_api.egg-info/PKG-INFO
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)      290 2024-04-04 03:26:52.000000 pixlr_private_api-0.1.2/pixlr_private_api.egg-info/SOURCES.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)        1 2024-04-04 03:26:52.000000 pixlr_private_api-0.1.2/pixlr_private_api.egg-info/dependency_links.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       34 2024-04-04 03:26:52.000000 pixlr_private_api-0.1.2/pixlr_private_api.egg-info/requires.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       18 2024-04-04 03:26:52.000000 pixlr_private_api-0.1.2/pixlr_private_api.egg-info/top_level.txt
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)       38 2024-04-04 03:26:52.331022 pixlr_private_api-0.1.2/setup.cfg
+-rw-r--r--   0 adoniscodes  (1000) adoniscodes  (1000)     1194 2024-04-04 03:26:36.000000 pixlr_private_api-0.1.2/setup.py
```

### Comparing `pixlr_private_api-0.1.1/LICENCE.txt` & `pixlr_private_api-0.1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pixlr_private_api-0.1.1/PKG-INFO` & `pixlr_private_api-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixlr_private_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python Package to Generate Images with http://pixlr.com programmatically.
 Home-page: https://github.com/Automa-Automations/pixlr-private-api
 Author: Simon Ferns
 Author-email: business@simonferns.com
 License: MIT
 Keywords: temp-email automation email
 Classifier: Development Status :: 3 - Alpha
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: requests
 Requires-Dist: temp_email_automa
+Requires-Dist: pillow
 
 ### Pixlr API Usage Guide
 
 This Python module provides a simple interface for automating actions on the Pixlr platform, including registration, email verification, generating images, and deleting accounts. Below is a guide on how to use this module effectively:
 
 #### Prerequisites:
```

### Comparing `pixlr_private_api-0.1.1/README.md` & `pixlr_private_api-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pixlr_private_api-0.1.1/pixlr_private_api/main.py` & `pixlr_private_api-0.1.2/pixlr_private_api/main.py`

 * *Files identical despite different names*

### Comparing `pixlr_private_api-0.1.1/pixlr_private_api.egg-info/PKG-INFO` & `pixlr_private_api-0.1.2/pixlr_private_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixlr_private_api
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python Package to Generate Images with http://pixlr.com programmatically.
 Home-page: https://github.com/Automa-Automations/pixlr-private-api
 Author: Simon Ferns
 Author-email: business@simonferns.com
 License: MIT
 Keywords: temp-email automation email
 Classifier: Development Status :: 3 - Alpha
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 Requires-Dist: requests
 Requires-Dist: temp_email_automa
+Requires-Dist: pillow
 
 ### Pixlr API Usage Guide
 
 This Python module provides a simple interface for automating actions on the Pixlr platform, including registration, email verification, generating images, and deleting accounts. Below is a guide on how to use this module effectively:
 
 #### Prerequisites:
```

### Comparing `pixlr_private_api-0.1.1/setup.py` & `pixlr_private_api-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pixlr_private_api",
-    version="0.1.1",
+    version="0.1.2",
     description="A Python Package to Generate Images with http://pixlr.com programmatically.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Automa-Automations/pixlr-private-api",
     author="Simon Ferns",
     author_email="business@simonferns.com",
     license="MIT",
@@ -22,9 +22,9 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
     keywords="temp-email automation email",
     packages=find_packages(),
-    install_requires=["requests", "temp_email_automa"],
+    install_requires=["requests", "temp_email_automa", "pillow"],
 )
```

