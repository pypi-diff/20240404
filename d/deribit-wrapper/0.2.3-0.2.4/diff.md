# Comparing `tmp/deribit_wrapper-0.2.3.tar.gz` & `tmp/deribit_wrapper-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deribit_wrapper-0.2.3.tar", last modified: Wed Apr  3 17:30:01 2024, max compression
+gzip compressed data, was "deribit_wrapper-0.2.4.tar", last modified: Thu Apr  4 14:05:02 2024, max compression
```

## Comparing `deribit_wrapper-0.2.3.tar` & `deribit_wrapper-0.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:01.265299 deribit_wrapper-0.2.3/deribit_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/account_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/core.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/market_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8083 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/trading.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/deribit_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:30:01.000000 deribit_wrapper-0.2.3/deribit_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:01.269299 deribit_wrapper-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-03 17:29:53.000000 deribit_wrapper-0.2.3/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:02.178044 deribit_wrapper-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-04 14:05:02.178044 deribit_wrapper-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:02.174044 deribit_wrapper-0.2.4/deribit_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/account_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/market_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7829 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/trading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/deribit_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:02.178044 deribit_wrapper-0.2.4/deribit_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-04 14:05:02.000000 deribit_wrapper-0.2.4/deribit_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-04 14:05:02.000000 deribit_wrapper-0.2.4/deribit_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:05:02.000000 deribit_wrapper-0.2.4/deribit_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 14:05:02.000000 deribit_wrapper-0.2.4/deribit_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 14:05:02.000000 deribit_wrapper-0.2.4/deribit_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:05:02.178044 deribit_wrapper-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:05:02.178044 deribit_wrapper-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-04 14:04:52.000000 deribit_wrapper-0.2.4/tests/test_base.py
```

### Comparing `deribit_wrapper-0.2.3/LICENSE` & `deribit_wrapper-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/PKG-INFO` & `deribit_wrapper-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit_wrapper
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.2.3/README.md` & `deribit_wrapper-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper/account_management.py` & `deribit_wrapper-0.2.4/deribit_wrapper/account_management.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper/authentication.py` & `deribit_wrapper-0.2.4/deribit_wrapper/authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper/base.py` & `deribit_wrapper-0.2.4/deribit_wrapper/base.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper/core.py` & `deribit_wrapper-0.2.4/deribit_wrapper/core.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper/market_data.py` & `deribit_wrapper-0.2.4/deribit_wrapper/market_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             ret = r['contract_size']
         except KeyError:
             logging.warning('No result found for asset {}.'.format(asset))
             return {}
         return ret
 
     def get_currencies(self) -> list[dict]:
-        r = self._session.get(self.api_url + self.__GET_CURRENCY_URI)
+        r = self._request(self.__GET_CURRENCY_URI, {})
         ret = r.json()['result']
         return ret
 
     @property
     def currencies(self) -> list[str]:
         df = pd.DataFrame(self.get_currencies())
         currency = list(df['currency'])
```

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper/trading.py` & `deribit_wrapper-0.2.4/deribit_wrapper/trading.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,44 +82,42 @@
     def get_entire_trade_history(self, include_order_data: bool = False) -> pd.DataFrame:
         return self.get_trade_history(include_order_data=include_order_data)
 
     def _error_handler(self, ret: dict, uri: str, params: dict, exclude_codes: list[int] = None) -> dict:
         exclude_codes = exclude_codes or []
         code = ret.get('code')
 
+        if code in exclude_codes:
+            return ret
+
         # 0: no error
         if code == 0 or code is None:
             pass
 
         # 10009: not enough funds
-        elif code == 10009 and 10009 not in exclude_codes:
+        elif code == 10009:
             if params.get('reduce_only'):
                 print('Not enough funds. Already tried as reduce only.')
             else:
+                print(f'Not enough funds. Attempt as reduce only...')
                 params['reduce_only'] = True
-                max_attempts = 3
-                for i in range(max_attempts):
-                    print(f'Not enough funds. Attempt {i + 1} of {max_attempts} as reduce only...')
-                    ret = self._order_with_error_handling(uri, params, exclude_codes=[10009])
-                    code = ret.get('code')
-                    if code != 10009:
-                        break
+                ret = self._order_with_error_handling(uri, params, exclude_codes=[10009])
 
         # 10041: settlement in progress
-        elif code == 10041 and 10041 not in exclude_codes:
+        elif code == 10041:
             max_attempts = 60
             for i in range(max_attempts):
                 print('Settlement in progress. Waiting 1 second...')
                 time.sleep(1)
                 ret = self._order_with_error_handling(uri, params, exclude_codes=[10041])
                 code = ret.get('code')
                 if code != 10041:
                     break
 
-        elif code not in exclude_codes:
+        else:
             print(f'Error code {code} not handled yet.')
 
         return ret
 
     def _order_with_error_handling(self, uri: str, params: dict, handle_error: bool = True,
                                    exclude_codes: list[int] = None) -> dict:
         ret = self._request(uri, params)
```

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper/utilities.py` & `deribit_wrapper-0.2.4/deribit_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper.egg-info/PKG-INFO` & `deribit_wrapper-0.2.4/deribit_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deribit-wrapper
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python wrapper for seamless integration with Deribit's trading API, offering easy access to market data, account management, and trading operations.
 Home-page: https://github.com/AntonioVentilii/deribit-wrapper
 Author: Antonio Ventilii
 Author-email: antonioventilii@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/AntonioVentilii/deribit-wrapper
 Project-URL: Issue Tracker, https://github.com/AntonioVentilii/deribit-wrapper/issues
```

### Comparing `deribit_wrapper-0.2.3/deribit_wrapper.egg-info/SOURCES.txt` & `deribit_wrapper-0.2.4/deribit_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/setup.py` & `deribit_wrapper-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='deribit_wrapper',
-    version='0.2.3',
+    version='0.2.4',
     packages=find_packages(),
     description='A Python wrapper for seamless integration with Deribit\'s trading API, offering easy access to '
                 'market data, account management, and trading operations.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Antonio Ventilii',
     author_email='antonioventilii@gmail.com',
```

### Comparing `deribit_wrapper-0.2.3/tests/test_authentication.py` & `deribit_wrapper-0.2.4/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `deribit_wrapper-0.2.3/tests/test_base.py` & `deribit_wrapper-0.2.4/tests/test_base.py`

 * *Files identical despite different names*

