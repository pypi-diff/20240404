# Comparing `tmp/dagit-1.6.8.tar.gz` & `tmp/dagit-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagit-1.6.8.tar", last modified: Fri Mar  1 19:13:10 2024, max compression
+gzip compressed data, was "dagit-1.6.9.tar", last modified: Fri Mar  8 00:18:45 2024, max compression
```

## Comparing `dagit-1.6.8.tar` & `dagit-1.6.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:13:10.428468 dagit-1.6.8/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-01 19:11:21.000000 dagit-1.6.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       58 2024-03-01 19:11:21.000000 dagit-1.6.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      917 2024-03-01 19:13:10.428468 dagit-1.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2024-03-01 19:11:21.000000 dagit-1.6.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:13:10.428468 dagit-1.6.8/dagit/
--rw-r--r--   0 root         (0) root         (0)      148 2024-03-01 19:11:21.000000 dagit-1.6.8/dagit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-01 19:11:21.000000 dagit-1.6.8/dagit/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:13:10.428468 dagit-1.6.8/dagit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      917 2024-03-01 19:13:10.000000 dagit-1.6.8/dagit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      260 2024-03-01 19:13:10.000000 dagit-1.6.8/dagit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 19:13:10.000000 dagit-1.6.8/dagit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-03-01 19:13:10.000000 dagit-1.6.8/dagit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      111 2024-03-01 19:13:10.000000 dagit-1.6.8/dagit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-03-01 19:13:10.000000 dagit-1.6.8/dagit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      153 2024-03-01 19:13:10.432468 dagit-1.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1819 2024-03-01 19:11:21.000000 dagit-1.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:45.330274 dagit-1.6.9/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagit-1.6.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       58 2024-03-08 00:17:46.000000 dagit-1.6.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      917 2024-03-08 00:18:45.330274 dagit-1.6.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2024-03-08 00:17:46.000000 dagit-1.6.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:45.330274 dagit-1.6.9/dagit/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-03-08 00:17:46.000000 dagit-1.6.9/dagit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-08 00:17:46.000000 dagit-1.6.9/dagit/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:18:45.330274 dagit-1.6.9/dagit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      917 2024-03-08 00:18:45.000000 dagit-1.6.9/dagit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      260 2024-03-08 00:18:45.000000 dagit-1.6.9/dagit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:18:45.000000 dagit-1.6.9/dagit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-03-08 00:18:45.000000 dagit-1.6.9/dagit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2024-03-08 00:18:45.000000 dagit-1.6.9/dagit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-03-08 00:18:45.000000 dagit-1.6.9/dagit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2024-03-08 00:18:45.330274 dagit-1.6.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1819 2024-03-08 00:17:46.000000 dagit-1.6.9/setup.py
```

### Comparing `dagit-1.6.8/LICENSE` & `dagit-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dagit-1.6.8/PKG-INFO` & `dagit-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagit
-Version: 1.6.8
+Version: 1.6.9
 Summary: Web UI for dagster.
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagit-1.6.8/dagit.egg-info/PKG-INFO` & `dagit-1.6.9/dagit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagit
-Version: 1.6.8
+Version: 1.6.9
 Summary: Web UI for dagster.
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagit-1.6.8/setup.py` & `dagit-1.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagit_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster-webserver==1.6.8",
+        "dagster-webserver==1.6.9",
     ],
     extras_require={
         "notebook": [f"dagster-webserver[notebook]{pin}"],  # notebooks support
         "test": [f"dagster-webserver[test]{pin}"],  # TestClient deps in full
     },
     entry_points={
         "console_scripts": [
```

