# Comparing `tmp/deribit_wrapper-0.2.6.tar.gz` & `tmp/deribit_wrapper-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deribit_wrapper-0.2.6.tar", last modified: Thu Apr  4 14:19:50 2024, max compression
+gzip compressed data, was "deribit_wrapper-0.2.7.tar", last modified: Thu Apr  4 14:32:20 2024, max compression
```

## Comparing `deribit_wrapper-0.2.6.tar` & `deribit_wrapper-0.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/deribit_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/market_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/deribit_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:19:50.000000 deribit_wrapper-0.2.6/deribit_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:50.934612 deribit_wrapper-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-04 14:19:43.000000 deribit_wrapper-0.2.6/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/deribit_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/deribit_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:32:20.000000 deribit_wrapper-0.2.7/deribit_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:20.189991 deribit_wrapper-0.2.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-04 14:32:12.000000 deribit_wrapper-0.2.7/tests/test_base.py
```

### Comparing `deribit_wrapper-0.2.6/LICENSE` & `deribit_wrapper-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/PKG-INFO` & `deribit_wrapper-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit_wrapper
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.2.6/README.md` & `deribit_wrapper-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper/account_management.py` & `deribit_wrapper-0.2.7/deribit_wrapper/account_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             currency = self.currencies
         elif not isinstance(currency, list):
             currency = [currency]
         start_ts = from_dt_to_ts(pd.to_datetime(start, utc=True))
         end_ts = from_dt_to_ts(pd.to_datetime(end, utc=True))
         params['start_timestamp'] = start_ts
         params['end_timestamp'] = end_ts
-        results = pd.DataFrame(columns=['timestamp'])
+        results = pd.DataFrame()
         for q in query:
             if q is not None:
                 params['query'] = q
             for c in currency:
                 params['currency'] = c
                 params.pop('continuation', None)
                 continuation = True
```

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper/authentication.py` & `deribit_wrapper-0.2.7/deribit_wrapper/authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper/base.py` & `deribit_wrapper-0.2.7/deribit_wrapper/base.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper/core.py` & `deribit_wrapper-0.2.7/deribit_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper/market_data.py` & `deribit_wrapper-0.2.7/deribit_wrapper/market_data.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper/trading.py` & `deribit_wrapper-0.2.7/deribit_wrapper/trading.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,16 +71,16 @@
                           currency: str | list[str] = None, include_order_data: bool = False) -> pd.DataFrame:
         start = start or DEFAULT_START
         end = end or DEFAULT_END
         results = self.get_transaction_log(start, end, currency, query='trade')
         if not results.empty:
             if include_order_data:
                 results = self.add_order_data(results)
-        results.sort_values('timestamp', inplace=True)
-        results['id'] = results['id'].astype(int, errors='ignore')
+            results.sort_values('timestamp', inplace=True)
+            results['id'] = results['id'].astype(int, errors='ignore')
         return results
 
     def get_entire_trade_history(self, include_order_data: bool = False) -> pd.DataFrame:
         return self.get_trade_history(include_order_data=include_order_data)
 
     def _error_handler(self, ret: dict, uri: str, params: dict, exclude_codes: list[int] = None) -> dict:
         exclude_codes = exclude_codes or []
```

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper/utilities.py` & `deribit_wrapper-0.2.7/deribit_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper.egg-info/PKG-INFO` & `deribit_wrapper-0.2.7/deribit_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit-wrapper
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.2.6/deribit_wrapper.egg-info/SOURCES.txt` & `deribit_wrapper-0.2.7/deribit_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/setup.py` & `deribit_wrapper-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='deribit_wrapper',
-    version='0.2.6',
+    version='0.2.7',
     packages=find_packages(),
     description='A Python wrapper for seamless integration with Deribit\'s trading API, offering easy access to '
                 'market data, account management, and trading operations.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
```

### Comparing `deribit_wrapper-0.2.6/tests/test_authentication.py` & `deribit_wrapper-0.2.7/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.6/tests/test_base.py` & `deribit_wrapper-0.2.7/tests/test_base.py`

 * *Files identical despite different names*

