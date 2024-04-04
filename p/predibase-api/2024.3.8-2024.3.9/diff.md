# Comparing `tmp/predibase-api-2024.3.8.tar.gz` & `tmp/predibase-api-2024.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2024.3.8.tar", last modified: Fri Mar 29 01:59:04 2024, max compression
+gzip compressed data, was "predibase-api-2024.3.9.tar", last modified: Fri Mar 29 02:45:27 2024, max compression
```

## Comparing `predibase-api-2024.3.8.tar` & `predibase-api-2024.3.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.867169 predibase-api-2024.3.8/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.867169 predibase-api-2024.3.8/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.867169 predibase-api-2024.3.8/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-29 01:59:03.000000 predibase-api-2024.3.8/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.867169 predibase-api-2024.3.8/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-29 01:59:00.000000 predibase-api-2024.3.8/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-29 01:58:59.000000 predibase-api-2024.3.8/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-29 01:59:01.000000 predibase-api-2024.3.8/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-03-29 01:59:04.000000 predibase-api-2024.3.8/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-29 01:59:02.000000 predibase-api-2024.3.8/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:59:04.867169 predibase-api-2024.3.8/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-29 01:59:04.000000 predibase-api-2024.3.8/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-29 01:59:04.000000 predibase-api-2024.3.8/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 01:59:04.000000 predibase-api-2024.3.8/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 01:58:16.000000 predibase-api-2024.3.8/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 01:59:04.000000 predibase-api-2024.3.8/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 01:59:04.000000 predibase-api-2024.3.8/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 01:59:04.871168 predibase-api-2024.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-29 01:57:51.000000 predibase-api-2024.3.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 01:58:58.000000 predibase-api-2024.3.8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.165552 predibase-api-2024.3.9/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.165552 predibase-api-2024.3.9/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-29 02:45:25.000000 predibase-api-2024.3.9/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-29 02:45:22.000000 predibase-api-2024.3.9/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-29 02:45:21.000000 predibase-api-2024.3.9/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-29 02:45:23.000000 predibase-api-2024.3.9/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-03-29 02:45:26.000000 predibase-api-2024.3.9/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-29 02:45:24.000000 predibase-api-2024.3.9/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:45:27.165552 predibase-api-2024.3.9/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-29 02:45:27.000000 predibase-api-2024.3.9/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-29 02:45:27.000000 predibase-api-2024.3.9/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 02:45:27.000000 predibase-api-2024.3.9/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 02:44:36.000000 predibase-api-2024.3.9/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 02:45:27.000000 predibase-api-2024.3.9/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 02:45:27.000000 predibase-api-2024.3.9/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 02:45:27.169552 predibase-api-2024.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-29 02:44:11.000000 predibase-api-2024.3.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-29 02:45:19.000000 predibase-api-2024.3.9/version.txt
```

### Comparing `predibase-api-2024.3.8/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2024.3.9/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.3.8/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2024.3.9/predibase_api/foobar/v1/bar_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.3.8/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2024.3.9/predibase_api/foobar/v1/foo_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.3.8/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2024.3.9/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.3.8/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2024.3.9/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.3.8/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2024.3.9/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.3.8/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2024.3.9/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.3.8/setup.py` & `predibase-api-2024.3.9/setup.py`

 * *Files identical despite different names*

