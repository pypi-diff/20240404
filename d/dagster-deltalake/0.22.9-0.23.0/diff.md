# Comparing `tmp/dagster-deltalake-0.22.9.tar.gz` & `tmp/dagster-deltalake-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-deltalake-0.22.9.tar", last modified: Fri Mar  8 00:28:54 2024, max compression
+gzip compressed data, was "dagster-deltalake-0.23.0.tar", last modified: Thu Apr  4 19:51:36 2024, max compression
```

## Comparing `dagster-deltalake-0.22.9.tar` & `dagster-deltalake-0.23.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:28:54.504132 dagster-deltalake-0.22.9/
--rw-r--r--   0 root         (0) root         (0)    11344 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       51 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      707 2024-03-08 00:28:54.504132 dagster-deltalake-0.22.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      137 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:28:54.504132 dagster-deltalake-0.22.9/dagster_deltalake/
--rw-r--r--   0 root         (0) root         (0)      990 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/dagster_deltalake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6650 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/dagster_deltalake/config.py
--rw-r--r--   0 root         (0) root         (0)     9929 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/dagster_deltalake/handler.py
--rw-r--r--   0 root         (0) root         (0)     9439 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/dagster_deltalake/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/dagster_deltalake/py.typed
--rw-r--r--   0 root         (0) root         (0)     1694 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/dagster_deltalake/resource.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/dagster_deltalake/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:28:54.504132 dagster-deltalake-0.22.9/dagster_deltalake.egg-info/
--rw-r--r--   0 root         (0) root         (0)      707 2024-03-08 00:28:54.000000 dagster-deltalake-0.22.9/dagster_deltalake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2024-03-08 00:28:54.000000 dagster-deltalake-0.22.9/dagster_deltalake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:28:54.000000 dagster-deltalake-0.22.9/dagster_deltalake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:28:54.000000 dagster-deltalake-0.22.9/dagster_deltalake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2024-03-08 00:28:54.000000 dagster-deltalake-0.22.9/dagster_deltalake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-08 00:28:54.000000 dagster-deltalake-0.22.9/dagster_deltalake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      128 2024-03-08 00:28:54.504132 dagster-deltalake-0.22.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1408 2024-03-08 00:17:46.000000 dagster-deltalake-0.22.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/
+-rw-r--r--   0 root         (0) root         (0)    11344 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      707 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      137 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/dagster_deltalake/
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6650 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/config.py
+-rw-r--r--   0 root         (0) root         (0)     9940 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/handler.py
+-rw-r--r--   0 root         (0) root         (0)     9439 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1694 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/resource.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/dagster_deltalake/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      707 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-04 19:51:35.000000 dagster-deltalake-0.23.0/dagster_deltalake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-04 19:51:36.030492 dagster-deltalake-0.23.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-04-04 19:44:08.000000 dagster-deltalake-0.23.0/setup.py
```

### Comparing `dagster-deltalake-0.22.9/LICENSE` & `dagster-deltalake-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.22.9/PKG-INFO` & `dagster-deltalake-0.23.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for Deltalake-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-0.22.9/dagster_deltalake/__init__.py` & `dagster-deltalake-0.23.0/dagster_deltalake/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.22.9/dagster_deltalake/config.py` & `dagster-deltalake-0.23.0/dagster_deltalake/config.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.22.9/dagster_deltalake/handler.py` & `dagster-deltalake-0.23.0/dagster_deltalake/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self,
         context: OutputContext,
         table_slice: TableSlice,
         obj: T,
         connection: TableConnection,
     ):
         """Stores pyarrow types in Delta table."""
-        metadata = context.metadata or {}
+        metadata = context.definition_metadata or {}
         resource_config = context.resource_config or {}
         reader, delta_params = self.to_arrow(obj=obj)
         delta_schema = Schema.from_pyarrow(reader.schema)
 
         engine = resource_config.get("writer_engine")
         save_mode = metadata.get("mode")
         main_save_mode = resource_config.get("mode")
```

### Comparing `dagster-deltalake-0.22.9/dagster_deltalake/io_manager.py` & `dagster-deltalake-0.23.0/dagster_deltalake/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.22.9/dagster_deltalake/resource.py` & `dagster-deltalake-0.23.0/dagster_deltalake/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-deltalake-0.22.9/dagster_deltalake.egg-info/PKG-INFO` & `dagster-deltalake-0.23.0/dagster_deltalake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-deltalake
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for Deltalake-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-deltalake
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-deltalake-0.22.9/setup.py` & `dagster-deltalake-0.23.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_deltalake_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
         "deltalake>=0.15",
-        "dagster==1.6.9",
+        "dagster==1.7.0",
     ],
     extras_require={
         "pandas": ["pandas"],
     },
     zip_safe=False,
 )
```

