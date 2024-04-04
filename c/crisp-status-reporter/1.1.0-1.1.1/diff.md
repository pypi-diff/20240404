# Comparing `tmp/crisp-status-reporter-1.1.0.tar.gz` & `tmp/crisp-status-reporter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crisp-status-reporter-1.1.0.tar", last modified: Mon Aug 28 15:58:40 2023, max compression
+gzip compressed data, was "crisp-status-reporter-1.1.1.tar", last modified: Thu Apr  4 08:09:52 2024, max compression
```

## Comparing `crisp-status-reporter-1.1.0.tar` & `crisp-status-reporter-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:58:40.007083 crisp-status-reporter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (999)       47 2023-08-28 15:58:27.000000 crisp-status-reporter-1.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (999)     1506 2023-08-28 15:58:27.000000 crisp-status-reporter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       64 2023-08-28 15:58:27.000000 crisp-status-reporter-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     2407 2023-08-28 15:58:40.007083 crisp-status-reporter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1847 2023-08-28 15:58:27.000000 crisp-status-reporter-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:58:40.007083 crisp-status-reporter-1.1.0/crisp_status_reporter/
--rw-r--r--   0 runner    (1001) docker     (999)     4447 2023-08-28 15:58:27.000000 crisp-status-reporter-1.1.0/crisp_status_reporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:58:40.007083 crisp-status-reporter-1.1.0/crisp_status_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2407 2023-08-28 15:58:39.000000 crisp-status-reporter-1.1.0/crisp_status_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      304 2023-08-28 15:58:39.000000 crisp-status-reporter-1.1.0/crisp_status_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 15:58:39.000000 crisp-status-reporter-1.1.0/crisp_status_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 15:58:39.000000 crisp-status-reporter-1.1.0/crisp_status_reporter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)       22 2023-08-28 15:58:39.000000 crisp-status-reporter-1.1.0/crisp_status_reporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 15:58:40.007083 crisp-status-reporter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      842 2023-08-28 15:58:27.000000 crisp-status-reporter-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:09:52.803499 crisp-status-reporter-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 08:09:40.000000 crisp-status-reporter-1.1.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-04 08:09:40.000000 crisp-status-reporter-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 08:09:40.000000 crisp-status-reporter-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-04 08:09:52.803499 crisp-status-reporter-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-04 08:09:40.000000 crisp-status-reporter-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:09:52.803499 crisp-status-reporter-1.1.1/crisp_status_reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-04 08:09:40.000000 crisp-status-reporter-1.1.1/crisp_status_reporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 08:09:52.803499 crisp-status-reporter-1.1.1/crisp_status_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-04 08:09:52.000000 crisp-status-reporter-1.1.1/crisp_status_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-04 08:09:52.000000 crisp-status-reporter-1.1.1/crisp_status_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:09:52.000000 crisp-status-reporter-1.1.1/crisp_status_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 08:09:52.000000 crisp-status-reporter-1.1.1/crisp_status_reporter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 08:09:52.000000 crisp-status-reporter-1.1.1/crisp_status_reporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 08:09:52.803499 crisp-status-reporter-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-04 08:09:40.000000 crisp-status-reporter-1.1.1/setup.py
```

### Comparing `crisp-status-reporter-1.1.0/LICENSE` & `crisp-status-reporter-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crisp-status-reporter-1.1.0/PKG-INFO` & `crisp-status-reporter-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crisp-status-reporter
-Version: 1.1.0
+Version: 1.1.1
 Summary: Crisp Status Reporter for Python.
 Home-page: https://github.com/crisp-im/python-crisp-status-reporter
 Author: Valerian Saliou
 Author-email: valerian@valeriansaliou.name
 License: MIT - http://opensource.org/licenses/mit-license.php
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `crisp-status-reporter-1.1.0/README.md` & `crisp-status-reporter-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `crisp-status-reporter-1.1.0/crisp_status_reporter/__init__.py` & `crisp-status-reporter-1.1.1/crisp_status_reporter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import urllib.error
 import urllib.request
 
 from threading import Thread
 
 REPORT_URL = "https://report.crisp.watch/v1"
 REPORT_ACCEPT = "application/json"
-REPORT_USERAGENT = "python-crisp-status-reporter/1.1.0"
+REPORT_USERAGENT = "python-crisp-status-reporter/1.1.1"
+REPORT_TIMEOUT = 10
 REPORT_INITIAL_DELAY = 10
 REPORT_INTERVAL_DEFAULT = 30
 
 class Reporter:
   def __init__(
     self, token, service_id, node_id, replica_id, interval=None, logger=None
   ):
@@ -119,15 +120,15 @@
 
         method="POST",
         headers=self.__report_headers,
         data=json.dumps(data).encode()
       )
 
       # Execute request
-      with urllib.request.urlopen(request) as response:
+      with urllib.request.urlopen(request, timeout=REPORT_TIMEOUT) as response:
         # Response is success?
         if response.status == 200:
           self.__log_debug("(status) Reporter request got success status")
 
           # Report succeeded (cut short)
           return True
```

### Comparing `crisp-status-reporter-1.1.0/crisp_status_reporter.egg-info/PKG-INFO` & `crisp-status-reporter-1.1.1/crisp_status_reporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crisp-status-reporter
-Version: 1.1.0
+Version: 1.1.1
 Summary: Crisp Status Reporter for Python.
 Home-page: https://github.com/crisp-im/python-crisp-status-reporter
 Author: Valerian Saliou
 Author-email: valerian@valeriansaliou.name
 License: MIT - http://opensource.org/licenses/mit-license.php
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `crisp-status-reporter-1.1.0/setup.py` & `crisp-status-reporter-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from distutils.core import setup
 from setuptools import find_packages
 
 
 setup(
     name='crisp-status-reporter',
-    version='1.1.0',
+    version='1.1.1',
     author=u'Valerian Saliou',
     author_email='valerian@valeriansaliou.name',
     packages=find_packages(),
     include_package_data=True,
     url='https://github.com/crisp-im/python-crisp-status-reporter',
     license='MIT - http://opensource.org/licenses/mit-license.php',
     description='Crisp Status Reporter for Python.',
```

