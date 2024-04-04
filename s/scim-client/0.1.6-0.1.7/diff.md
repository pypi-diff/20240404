# Comparing `tmp/scim_client-0.1.6.tar.gz` & `tmp/scim_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scim_client-0.1.6.tar", last modified: Mon Apr  1 11:01:38 2024, max compression
+gzip compressed data, was "scim_client-0.1.7.tar", last modified: Thu Apr  4 07:48:36 2024, max compression
```

## Comparing `scim_client-0.1.6.tar` & `scim_client-0.1.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.269898 scim_client-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-01 11:01:34.000000 scim_client-0.1.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-01 11:01:34.000000 scim_client-0.1.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-01 11:01:34.000000 scim_client-0.1.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-01 11:01:34.000000 scim_client-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 11:01:34.000000 scim_client-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-01 11:01:38.269898 scim_client-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-01 11:01:34.000000 scim_client-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.265898 scim_client-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4842 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 11:01:34.000000 scim_client-0.1.6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.269898 scim_client-0.1.6/scim_client/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/scim_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-01 11:01:34.000000 scim_client-0.1.6/scim_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.269898 scim_client-0.1.6/scim_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 11:01:38.000000 scim_client-0.1.6/scim_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-01 11:01:38.269898 scim_client-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-01 11:01:34.000000 scim_client-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:38.269898 scim_client-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 11:01:34.000000 scim_client-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-01 11:01:34.000000 scim_client-0.1.6/tests/test_scim_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.287819 scim_client-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 07:48:32.000000 scim_client-0.1.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-04 07:48:32.000000 scim_client-0.1.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-04 07:48:32.000000 scim_client-0.1.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-04 07:48:32.000000 scim_client-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-04 07:48:32.000000 scim_client-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-04 07:48:36.287819 scim_client-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-04 07:48:32.000000 scim_client-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.283819 scim_client-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4842 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 07:48:32.000000 scim_client-0.1.7/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.283819 scim_client-0.1.7/scim_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/scim_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-04 07:48:32.000000 scim_client-0.1.7/scim_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.287819 scim_client-0.1.7/scim_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 07:48:36.000000 scim_client-0.1.7/scim_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-04 07:48:36.287819 scim_client-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-04 07:48:32.000000 scim_client-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:48:36.287819 scim_client-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-04 07:48:32.000000 scim_client-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-04 07:48:32.000000 scim_client-0.1.7/tests/test_scim_client.py
```

### Comparing `scim_client-0.1.6/CONTRIBUTING.rst` & `scim_client-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/LICENSE` & `scim_client-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/PKG-INFO` & `scim_client-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim_client
-Version: 0.1.6
+Version: 0.1.7
 Summary: SCIM v2 API client
 Home-page: https://github.com/Aplopio/python-scim-client
 Author: Mitratech Development Team
 Author-email: devs@mitratech.com
 License: MIT license
 Keywords: scim_client
 Classifier: Development Status :: 4 - Beta
```

### Comparing `scim_client-0.1.6/README.rst` & `scim_client-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/docs/Makefile` & `scim_client-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/docs/conf.py` & `scim_client-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/docs/installation.rst` & `scim_client-0.1.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/docs/make.bat` & `scim_client-0.1.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/scim_client/resources.py` & `scim_client-0.1.7/scim_client/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,17 @@
                     extension_key = _to_snake_case_key(_get_extension_key(sc))
                     setattr(
                         self,
                         extension_key,
                         UserExtension(**kwargs.get(extension_key, {})),
                     )
 
+    def __eq__(self, other: "User") -> bool:
+        return self.id == other.id
+
 
 class UserSearch(BaseResource):
     CORE_SCHEMA = "urn:ietf:params:scim:api:messages:2.0:ListResponse"
 
     resources: List[User]
     total_results: int
     items_per_page: int
```

### Comparing `scim_client-0.1.6/scim_client/response.py` & `scim_client-0.1.7/scim_client/response.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/scim_client/scim_client.py` & `scim_client-0.1.7/scim_client/scim_client.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/scim_client/utils.py` & `scim_client-0.1.7/scim_client/utils.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/scim_client.egg-info/PKG-INFO` & `scim_client-0.1.7/scim_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scim_client
-Version: 0.1.6
+Version: 0.1.7
 Summary: SCIM v2 API client
 Home-page: https://github.com/Aplopio/python-scim-client
 Author: Mitratech Development Team
 Author-email: devs@mitratech.com
 License: MIT license
 Keywords: scim_client
 Classifier: Development Status :: 4 - Beta
```

### Comparing `scim_client-0.1.6/scim_client.egg-info/SOURCES.txt` & `scim_client-0.1.7/scim_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/setup.py` & `scim_client-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `scim_client-0.1.6/tests/test_scim_client.py` & `scim_client-0.1.7/tests/test_scim_client.py`

 * *Files identical despite different names*

