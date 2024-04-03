# Comparing `tmp/ncm-0.0.31.tar.gz` & `tmp/ncm-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncm-0.0.31.tar", last modified: Tue Apr  2 16:39:21 2024, max compression
+gzip compressed data, was "ncm-0.0.32.tar", last modified: Wed Apr  3 22:07:45 2024, max compression
```

## Comparing `ncm-0.0.31.tar` & `ncm-0.0.32.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-02 16:39:21.491657 ncm-0.0.31/
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1083 2024-04-01 16:31:07.000000 ncm-0.0.31/LICENSE
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-02 16:39:21.491657 ncm-0.0.31/PKG-INFO
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1932 2024-04-01 16:31:07.000000 ncm-0.0.31/README.md
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-02 16:39:21.490657 ncm-0.0.31/ncm/
--rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:31:07.000000 ncm-0.0.31/ncm/__init__.py
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)   150130 2024-04-02 16:33:35.000000 ncm-0.0.31/ncm/ncm.py
-drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-02 16:39:21.491657 ncm-0.0.31/ncm.egg-info/
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-02 16:39:21.000000 ncm-0.0.31/ncm.egg-info/PKG-INFO
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)      187 2024-04-02 16:39:21.000000 ncm-0.0.31/ncm.egg-info/SOURCES.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        1 2024-04-02 16:39:21.000000 ncm-0.0.31/ncm.egg-info/dependency_links.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       17 2024-04-02 16:39:21.000000 ncm-0.0.31/ncm.egg-info/requires.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        4 2024-04-02 16:39:21.000000 ncm-0.0.31/ncm.egg-info/top_level.txt
--rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       38 2024-04-02 16:39:21.491657 ncm-0.0.31/setup.cfg
--rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)      602 2024-04-02 16:34:05.000000 ncm-0.0.31/setup.py
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-03 22:07:45.461346 ncm-0.0.32/
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1083 2024-04-01 16:31:07.000000 ncm-0.0.32/LICENSE
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-03 22:07:45.460346 ncm-0.0.32/PKG-INFO
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     1932 2024-04-01 16:31:07.000000 ncm-0.0.32/README.md
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-03 22:07:45.459346 ncm-0.0.32/ncm/
+-rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-01 16:31:07.000000 ncm-0.0.32/ncm/__init__.py
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)   150635 2024-04-03 21:55:00.000000 ncm-0.0.32/ncm/ncm.py
+drwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)        0 2024-04-03 22:07:45.460346 ncm-0.0.32/ncm.egg-info/
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)     2316 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/PKG-INFO
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)      187 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/SOURCES.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        1 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/dependency_links.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       17 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/requires.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)        4 2024-04-03 22:07:45.000000 ncm-0.0.32/ncm.egg-info/top_level.txt
+-rw-r--r--   0 dapplegate  (1000) dapplegate  (1000)       38 2024-04-03 22:07:45.461346 ncm-0.0.32/setup.cfg
+-rwxr-xr-x   0 dapplegate  (1000) dapplegate  (1000)      602 2024-04-03 21:56:14.000000 ncm-0.0.32/setup.py
```

### Comparing `ncm-0.0.31/LICENSE` & `ncm-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-0.0.31/PKG-INFO` & `ncm-0.0.32/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.31
+Version: 0.0.32
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.31/README.md` & `ncm-0.0.32/README.md`

 * *Files identical despite different names*

### Comparing `ncm-0.0.31/ncm/ncm.py` & `ncm-0.0.32/ncm/ncm.py`

 * *Files 1% similar despite different names*

```diff
@@ -3827,20 +3827,15 @@
             if kwargs['search']:
                 params = self.__parse_search_kwargs(kwargs, allowed_params)
             else:
                 params = self.__parse_kwargs(kwargs, allowed_params)
         return self.__get_json(get_url, call_type, params=params)
 '''
 
-class NcmClient:
-    """
-    This NCM Client class provides functions for interacting with =
-    the Cradlepoint NCM API. Full documentation of the Cradlepoint API can be
-    found at: https://developer.cradlepoint.com
-    """
+class NcmClientv2v3:
 
     def __init__(self, 
               api_keys=None,
               api_key=None,
               log_events=True,
               logger=None,
               retries=5,
@@ -3884,7 +3879,27 @@
         except AttributeError:
             # Prioritize v3 over v2
             if self.v3 and hasattr(self.v3, name):
                 return getattr(self.v3, name)
             if self.v2 and hasattr(self.v2, name):
                 return getattr(self.v2, name)
             raise
+
+
+class NcmClient:
+    """
+    This NCM Client class provides functions for interacting with =
+    the Cradlepoint NCM API. Full documentation of the Cradlepoint API can be
+    found at: https://developer.cradlepoint.com
+    """
+
+    def __new__(cls, api_keys=None, api_key=None, **kwargs):
+        api_keys = api_keys or {}
+        apiv3_key = api_keys.pop('token', None) or api_key
+        v2 = bool(api_keys)
+        v3 = bool(apiv3_key)
+        if v2 and v3:
+            return NcmClientv2v3(api_keys=api_keys, api_key=apiv3_key, **kwargs)
+        if v2 or not (v2 or v3):
+            return NcmClientv2(api_keys=api_keys, **kwargs)
+        else:
+            return NcmClientv3(api_key=apiv3_key, **kwargs)
```

### Comparing `ncm-0.0.31/ncm.egg-info/PKG-INFO` & `ncm-0.0.32/ncm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.31
+Version: 0.0.32
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.31/setup.py` & `ncm-0.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncm",
-    version="0.0.31",
+    version="0.0.32",
     author="Nathan Wiens - Cradlepoint",
     author_email="nathan.wiens@cradlepoint.com",
     description="Python client library for Cradlepoint NCM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cradlepoint/api-samples/tree/master/ncm",
     packages=find_packages(),
```

