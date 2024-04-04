# Comparing `tmp/deribit_wrapper-0.2.5.tar.gz` & `tmp/deribit_wrapper-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deribit_wrapper-0.2.5.tar", last modified: Thu Apr  4 14:11:07 2024, max compression
+gzip compressed data, was "deribit_wrapper-0.2.6.tar", last modified: Thu Apr  4 14:19:50 2024, max compression
```

## Comparing `deribit_wrapper-0.2.5.tar` & `deribit_wrapper-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:07.773854 deribit_wrapper-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-04 14:11:07.773854 deribit_wrapper-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:07.773854 deribit_wrapper-0.2.5/deribit_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/market_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/deribit_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:07.773854 deribit_wrapper-0.2.5/deribit_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-04 14:11:07.000000 deribit_wrapper-0.2.5/deribit_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-04 14:11:07.000000 deribit_wrapper-0.2.5/deribit_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:11:07.000000 deribit_wrapper-0.2.5/deribit_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 14:11:07.000000 deribit_wrapper-0.2.5/deribit_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:11:07.000000 deribit_wrapper-0.2.5/deribit_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:11:07.773854 deribit_wrapper-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:07.773854 deribit_wrapper-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-04 14:10:57.000000 deribit_wrapper-0.2.5/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/deribit_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/tests/test_base.py
```

### Comparing `deribit_wrapper-0.2.5/LICENSE` & `deribit_wrapper-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/PKG-INFO` & `deribit_wrapper-0.2.6/deribit_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: deribit_wrapper
-Version: 0.2.5
+Name: deribit-wrapper
+Version: 0.2.6
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # deribit-wrapper
 
 ## Overview
 
-This Python script provides a comprehensive client for interacting with the Deribit API.
+This Python script provides a comprehensive client for interacting with the [Deribit API](https://docs.deribit.com/).
 It encapsulates functionality for both public and private endpoints, covering market data, account information, trading
 operations, and more.
 It supports both the production and test environments, making it suitable for developers at all stages of application
 development.
 
 ## Features
```

### Comparing `deribit_wrapper-0.2.5/README.md` & `deribit_wrapper-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # deribit-wrapper
 
 ## Overview
 
-This Python script provides a comprehensive client for interacting with the Deribit API.
+This Python script provides a comprehensive client for interacting with the [Deribit API](https://docs.deribit.com/).
 It encapsulates functionality for both public and private endpoints, covering market data, account information, trading
 operations, and more.
 It supports both the production and test environments, making it suitable for developers at all stages of application
 development.
 
 ## Features
```

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper/account_management.py` & `deribit_wrapper-0.2.6/deribit_wrapper/account_management.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper/authentication.py` & `deribit_wrapper-0.2.6/deribit_wrapper/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,18 @@
                         ret = self._request(uri, params, give_results=give_results)
                 elif error_code == 13028:
                     max_attempts = 60
                     for i in range(max_attempts):
                         print(f'Temporarily unavailable. Waiting 1 minute [{i + 1}/{max_attempts}]...')
                         time.sleep(60)
                         ret = self._request(uri, params, give_results=give_results)
+                        if ret.get('code') != 13028:
+                            break
+                    if ret.get('code') == 13028:
+                        raise Exception('Service temporarily unavailable.')
                 else:
                     print(f'Error code {error_code} for request {uri} with params {params}.')
                     print(ret)
             else:
                 raise Exception(ret)
         else:
             ret = r
```

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper/base.py` & `deribit_wrapper-0.2.6/deribit_wrapper/base.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper/core.py` & `deribit_wrapper-0.2.6/deribit_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper/market_data.py` & `deribit_wrapper-0.2.6/deribit_wrapper/market_data.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper/trading.py` & `deribit_wrapper-0.2.6/deribit_wrapper/trading.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper/utilities.py` & `deribit_wrapper-0.2.6/deribit_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper.egg-info/PKG-INFO` & `deribit_wrapper-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: deribit-wrapper
-Version: 0.2.5
+Name: deribit_wrapper
+Version: 0.2.6
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # deribit-wrapper
 
 ## Overview
 
-This Python script provides a comprehensive client for interacting with the Deribit API.
+This Python script provides a comprehensive client for interacting with the [Deribit API](https://docs.deribit.com/).
 It encapsulates functionality for both public and private endpoints, covering market data, account information, trading
 operations, and more.
 It supports both the production and test environments, making it suitable for developers at all stages of application
 development.
 
 ## Features
```

### Comparing `deribit_wrapper-0.2.5/deribit_wrapper.egg-info/SOURCES.txt` & `deribit_wrapper-0.2.6/deribit_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/setup.py` & `deribit_wrapper-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='deribit_wrapper',
-    version='0.2.5',
+    version='0.2.6',
     packages=find_packages(),
     description='A Python wrapper for seamless integration with Deribit\'s trading API, offering easy access to '
                 'market data, account management, and trading operations.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
```

### Comparing `deribit_wrapper-0.2.5/tests/test_authentication.py` & `deribit_wrapper-0.2.6/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.5/tests/test_base.py` & `deribit_wrapper-0.2.6/tests/test_base.py`

 * *Files identical despite different names*

