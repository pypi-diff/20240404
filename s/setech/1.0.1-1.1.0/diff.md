# Comparing `tmp/setech-1.0.1.tar.gz` & `tmp/setech-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setech-1.0.1.tar", last modified: Wed Apr  3 21:50:04 2024, max compression
+gzip compressed data, was "setech-1.1.0.tar", last modified: Thu Apr  4 13:25:32 2024, max compression
```

## Comparing `setech-1.0.1.tar` & `setech-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-03 21:50:04.103364 setech-1.0.1/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.0.1/LICENCE
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-03 21:50:04.103364 setech-1.0.1/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.0.1/README.md
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1912 2024-04-03 21:49:59.000000 setech-1.0.1/pyproject.toml
--rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-03 21:50:04.103364 setech-1.0.1/setup.cfg
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-03 21:50:04.103364 setech-1.0.1/src/
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-03 21:50:04.103364 setech-1.0.1/src/setech/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-03 21:49:59.000000 setech-1.0.1/src/setech/__init__.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-03 21:50:04.103364 setech-1.0.1/src/setech/api_client/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.0.1/src/setech/api_client/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4832 2024-04-03 09:38:51.000000 setech-1.0.1/src/setech/api_client/_base.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2258 2024-04-03 09:38:51.000000 setech-1.0.1/src/setech/api_client/async_client.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2163 2024-04-03 09:38:59.000000 setech-1.0.1/src/setech/api_client/sync_client.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-03 21:50:04.103364 setech-1.0.1/src/setech/constants/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-03 14:55:19.000000 setech-1.0.1/src/setech/constants/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-03 14:22:18.000000 setech-1.0.1/src/setech/constants/date.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-03 21:50:04.103364 setech-1.0.1/src/setech/logging/
--rw-r--r--   0 eriks     (1000) eriks     (1000)       73 2024-04-03 13:03:49.000000 setech-1.0.1/src/setech/logging/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.0.1/src/setech/logging/formatters.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.0.1/src/setech/py.typed
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-03 21:50:04.103364 setech-1.0.1/src/setech/utils/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      933 2024-04-03 21:49:44.000000 setech-1.0.1/src/setech/utils/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      772 2024-04-03 21:00:04.000000 setech-1.0.1/src/setech/utils/numeric.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2133 2024-04-03 21:49:42.000000 setech-1.0.1/src/setech/utils/parse.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5555 2024-04-03 14:57:53.000000 setech-1.0.1/src/setech/utils/ssn.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1097 2024-04-03 14:55:19.000000 setech-1.0.1/src/setech/utils/text.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1034 2024-04-03 15:03:11.000000 setech-1.0.1/src/setech/utils/validators.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      874 2024-04-03 20:52:45.000000 setech-1.0.1/src/setech/utils/various.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-03 21:50:04.103364 setech-1.0.1/src/setech.egg-info/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-03 21:50:04.000000 setech-1.0.1/src/setech.egg-info/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)      701 2024-04-03 21:50:04.000000 setech-1.0.1/src/setech.egg-info/SOURCES.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-03 21:50:04.000000 setech-1.0.1/src/setech.egg-info/dependency_links.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)       50 2024-04-03 21:50:04.000000 setech-1.0.1/src/setech.egg-info/requires.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-03 21:50:04.000000 setech-1.0.1/src/setech.egg-info/top_level.txt
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:25:32.325823 setech-1.1.0/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.1.0/LICENCE
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-04 13:25:32.325823 setech-1.1.0/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.1.0/README.md
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1912 2024-04-04 13:25:13.000000 setech-1.1.0/pyproject.toml
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-04-04 13:25:32.325823 setech-1.1.0/setup.cfg
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:25:32.319158 setech-1.1.0/src/
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:25:32.322491 setech-1.1.0/src/setech/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-04-04 13:25:13.000000 setech-1.1.0/src/setech/__init__.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:25:32.322491 setech-1.1.0/src/setech/api_client/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.1.0/src/setech/api_client/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4832 2024-04-03 09:38:51.000000 setech-1.1.0/src/setech/api_client/_base.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2258 2024-04-03 09:38:51.000000 setech-1.1.0/src/setech/api_client/async_client.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2163 2024-04-03 09:38:59.000000 setech-1.1.0/src/setech/api_client/sync_client.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:25:32.322491 setech-1.1.0/src/setech/constants/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-03 14:55:19.000000 setech-1.1.0/src/setech/constants/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-03 14:22:18.000000 setech-1.1.0/src/setech/constants/date.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:25:32.325823 setech-1.1.0/src/setech/logging/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       73 2024-04-03 13:03:49.000000 setech-1.1.0/src/setech/logging/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.1.0/src/setech/logging/formatters.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-04-04 13:24:48.000000 setech-1.1.0/src/setech/logging/handlers.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.1.0/src/setech/py.typed
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:25:32.325823 setech-1.1.0/src/setech/utils/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      933 2024-04-03 21:49:44.000000 setech-1.1.0/src/setech/utils/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      848 2024-04-03 22:46:33.000000 setech-1.1.0/src/setech/utils/numeric.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2133 2024-04-03 21:49:42.000000 setech-1.1.0/src/setech/utils/parse.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5555 2024-04-03 14:57:53.000000 setech-1.1.0/src/setech/utils/ssn.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1097 2024-04-03 14:55:19.000000 setech-1.1.0/src/setech/utils/text.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1034 2024-04-03 15:03:11.000000 setech-1.1.0/src/setech/utils/validators.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      874 2024-04-03 20:52:45.000000 setech-1.1.0/src/setech/utils/various.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-04-04 13:25:32.325823 setech-1.1.0/src/setech.egg-info/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5345 2024-04-04 13:25:32.000000 setech-1.1.0/src/setech.egg-info/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      732 2024-04-04 13:25:32.000000 setech-1.1.0/src/setech.egg-info/SOURCES.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-04-04 13:25:32.000000 setech-1.1.0/src/setech.egg-info/dependency_links.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       50 2024-04-04 13:25:32.000000 setech-1.1.0/src/setech.egg-info/requires.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-04-04 13:25:32.000000 setech-1.1.0/src/setech.egg-info/top_level.txt
```

### Comparing `setech-1.0.1/LICENCE` & `setech-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/PKG-INFO` & `setech-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.0.1
+Version: 1.1.0
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.0.1/README.md` & `setech-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/pyproject.toml` & `setech-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 [tool.setuptools.dynamic]
 version = { attr = "setech.__version__" }
 
 
 [tool.bumpversion]
-current_version = "1.0.1"
+current_version = "1.1.0"
 commit = true
 tag = true
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
```

### Comparing `setech-1.0.1/src/setech/api_client/_base.py` & `setech-1.1.0/src/setech/api_client/_base.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/api_client/async_client.py` & `setech-1.1.0/src/setech/api_client/async_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/api_client/sync_client.py` & `setech-1.1.0/src/setech/api_client/sync_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/constants/date.py` & `setech-1.1.0/src/setech/constants/date.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/logging/formatters.py` & `setech-1.1.0/src/setech/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/utils/__init__.py` & `setech-1.1.0/src/setech/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/utils/numeric.py` & `setech-1.1.0/src/setech/utils/numeric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import decimal
 
 
 def round_decimal(dec: decimal.Decimal, precision: int = 4) -> decimal.Decimal:
-    """
+    """Round decimal value to a predefined precision from the start of the value. Examples:
+        - dec=123.456, precision=7 -> 123.4560,
+        - dec=123.456, precision=5 -> 123.46,
+        - dec=123.456, precision=3 -> 123,
+        - dec=123.456, precision=2 -> 120;
     :param dec: Decimal value to round
     :param precision: how many digits since the start of the value to keep
-            dec=123.456, precision=7 -> 123.4560,
-            dec=123.456, precision=5 -> 123.46,
-            dec=123.456, precision=3 -> 123,
-            dec=123.456, precision=2 -> 120;
     :return: rounded Decimal
     """
     with decimal.localcontext() as ctx:
         ctx.rounding = decimal.ROUND_HALF_UP
         value = decimal.Decimal(dec)
         dec_tuple = dec.as_tuple()
         whole_numbers = len(dec_tuple.digits) + dec_tuple.exponent  # type: ignore
```

### Comparing `setech-1.0.1/src/setech/utils/parse.py` & `setech-1.1.0/src/setech/utils/parse.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/utils/ssn.py` & `setech-1.1.0/src/setech/utils/ssn.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/utils/text.py` & `setech-1.1.0/src/setech/utils/text.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/utils/validators.py` & `setech-1.1.0/src/setech/utils/validators.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech/utils/various.py` & `setech-1.1.0/src/setech/utils/various.py`

 * *Files identical despite different names*

### Comparing `setech-1.0.1/src/setech.egg-info/PKG-INFO` & `setech-1.1.0/src/setech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.0.1
+Version: 1.1.0
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.0.1/src/setech.egg-info/SOURCES.txt` & `setech-1.1.0/src/setech.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/setech/api_client/_base.py
 src/setech/api_client/async_client.py
 src/setech/api_client/sync_client.py
 src/setech/constants/__init__.py
 src/setech/constants/date.py
 src/setech/logging/__init__.py
 src/setech/logging/formatters.py
+src/setech/logging/handlers.py
 src/setech/utils/__init__.py
 src/setech/utils/numeric.py
 src/setech/utils/parse.py
 src/setech/utils/ssn.py
 src/setech/utils/text.py
 src/setech/utils/validators.py
 src/setech/utils/various.py
```

