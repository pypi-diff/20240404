# Comparing `tmp/personal-web-utility-0.0.8.tar.gz` & `tmp/personal-web-utility-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal-web-utility-0.0.8.tar", last modified: Mon Feb 12 16:04:21 2024, max compression
+gzip compressed data, was "personal-web-utility-0.0.9.tar", last modified: Sun Feb 18 18:33:00 2024, max compression
```

## Comparing `personal-web-utility-0.0.8.tar` & `personal-web-utility-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 16:04:21.293280 personal-web-utility-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      536 2024-02-12 16:04:21.293280 personal-web-utility-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-02-12 16:04:04.000000 personal-web-utility-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 16:04:21.293280 personal-web-utility-0.0.8/personal_web_utility.egg-info/
--rw-r--r--   0 root         (0) root         (0)      536 2024-02-12 16:04:21.000000 personal-web-utility-0.0.8/personal_web_utility.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2024-02-12 16:04:21.000000 personal-web-utility-0.0.8/personal_web_utility.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-12 16:04:21.000000 personal-web-utility-0.0.8/personal_web_utility.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-02-12 16:04:21.000000 personal-web-utility-0.0.8/personal_web_utility.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-12 16:04:21.293280 personal-web-utility-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      665 2024-02-12 16:03:51.000000 personal-web-utility-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 16:04:21.292280 personal-web-utility-0.0.8/web/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 16:04:04.000000 personal-web-utility-0.0.8/web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-02-12 16:04:04.000000 personal-web-utility-0.0.8/web/dao.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2024-02-12 16:04:04.000000 personal-web-utility-0.0.8/web/database.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2024-02-12 16:04:04.000000 personal-web-utility-0.0.8/web/dto.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-02-12 16:04:04.000000 personal-web-utility-0.0.8/web/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2024-02-12 16:04:04.000000 personal-web-utility-0.0.8/web/middlewares.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-02-12 16:04:04.000000 personal-web-utility-0.0.8/web/pg_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 18:33:00.869850 personal-web-utility-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      536 2024-02-18 18:33:00.869850 personal-web-utility-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 18:33:00.869850 personal-web-utility-0.0.9/personal_web_utility.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      536 2024-02-18 18:33:00.000000 personal-web-utility-0.0.9/personal_web_utility.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      316 2024-02-18 18:33:00.000000 personal-web-utility-0.0.9/personal_web_utility.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-18 18:33:00.000000 personal-web-utility-0.0.9/personal_web_utility.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-02-18 18:33:00.000000 personal-web-utility-0.0.9/personal_web_utility.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-18 18:33:00.869850 personal-web-utility-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      665 2024-02-18 18:32:33.000000 personal-web-utility-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-18 18:33:00.869850 personal-web-utility-0.0.9/web/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/web/dao.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/web/database.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/web/dto.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/web/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/web/middlewares.py
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/web/pg_database.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-18 18:32:45.000000 personal-web-utility-0.0.9/web/unit.py
```

### Comparing `personal-web-utility-0.0.8/PKG-INFO` & `personal-web-utility-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-web-utility
-Version: 0.0.8
+Version: 0.0.9
 Summary: Personal web application utility
 Home-page: https://gitlab.com/mihael97/web-utility
 Author: Mihael Macuka
 Author-email: mihaelmacuka2@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `personal-web-utility-0.0.8/personal_web_utility.egg-info/PKG-INFO` & `personal-web-utility-0.0.9/personal_web_utility.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-web-utility
-Version: 0.0.8
+Version: 0.0.9
 Summary: Personal web application utility
 Home-page: https://gitlab.com/mihael97/web-utility
 Author: Mihael Macuka
 Author-email: mihaelmacuka2@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `personal-web-utility-0.0.8/setup.py` & `personal-web-utility-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="personal-web-utility",
-    version="0.0.8",
+    version="0.0.9",
     author="Mihael Macuka",
     author_email="mihaelmacuka2@gmail.com",
     description="Personal web application utility",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/mihael97/web-utility",
     packages=setuptools.find_packages(),
```

### Comparing `personal-web-utility-0.0.8/web/database.py` & `personal-web-utility-0.0.9/web/database.py`

 * *Files identical despite different names*

### Comparing `personal-web-utility-0.0.8/web/dto.py` & `personal-web-utility-0.0.9/web/dto.py`

 * *Files identical despite different names*

### Comparing `personal-web-utility-0.0.8/web/middlewares.py` & `personal-web-utility-0.0.9/web/middlewares.py`

 * *Files identical despite different names*

