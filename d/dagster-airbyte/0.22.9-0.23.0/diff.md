# Comparing `tmp/dagster-airbyte-0.22.9.tar.gz` & `tmp/dagster-airbyte-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.22.9.tar", last modified: Fri Mar  8 00:26:00 2024, max compression
+gzip compressed data, was "dagster-airbyte-0.23.0.tar", last modified: Thu Apr  4 19:53:32 2024, max compression
```

## Comparing `dagster-airbyte-0.22.9.tar` & `dagster-airbyte-0.23.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:26:00.349877 dagster-airbyte-0.22.9/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      753 2024-03-08 00:26:00.349877 dagster-airbyte-0.22.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:26:00.345877 dagster-airbyte-0.22.9/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47809 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:26:00.345877 dagster-airbyte-0.22.9/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:26:00.345877 dagster-airbyte-0.22.9/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282784 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    34911 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14588 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    27040 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2823 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:26:00.345877 dagster-airbyte-0.22.9/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      753 2024-03-08 00:26:00.000000 dagster-airbyte-0.22.9/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2024-03-08 00:26:00.000000 dagster-airbyte-0.22.9/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:26:00.000000 dagster-airbyte-0.22.9/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-03-08 00:26:00.000000 dagster-airbyte-0.22.9/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:26:00.000000 dagster-airbyte-0.22.9/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2024-03-08 00:26:00.000000 dagster-airbyte-0.22.9/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-08 00:26:00.000000 dagster-airbyte-0.22.9/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-03-08 00:26:00.357877 dagster-airbyte-0.22.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1636 2024-03-08 00:17:46.000000 dagster-airbyte-0.22.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:32.159260 dagster-airbyte-0.23.0/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      753 2024-04-04 19:53:32.159260 dagster-airbyte-0.23.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:32.147260 dagster-airbyte-0.23.0/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47799 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:32.151260 dagster-airbyte-0.23.0/dagster_airbyte/managed/
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:32.155260 dagster-airbyte-0.23.0/dagster_airbyte/managed/generated/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119751 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 root         (0) root         (0)   282784 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 root         (0) root         (0)    34862 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    14588 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)    27040 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:32.147260 dagster-airbyte-0.23.0/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      753 2024-04-04 19:53:31.000000 dagster-airbyte-0.23.0/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      809 2024-04-04 19:53:31.000000 dagster-airbyte-0.23.0/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:53:31.000000 dagster-airbyte-0.23.0/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-04 19:53:31.000000 dagster-airbyte-0.23.0/dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:53:31.000000 dagster-airbyte-0.23.0/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-04 19:53:31.000000 dagster-airbyte-0.23.0/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-04 19:53:31.000000 dagster-airbyte-0.23.0/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-04 19:53:32.159260 dagster-airbyte-0.23.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1636 2024-04-04 19:44:08.000000 dagster-airbyte-0.23.0/setup.py
```

### Comparing `dagster-airbyte-0.22.9/LICENSE` & `dagster-airbyte-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/PKG-INFO` & `dagster-airbyte-0.23.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/__init__.py` & `dagster-airbyte-0.23.0/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/asset_defs.py` & `dagster-airbyte-0.23.0/dagster_airbyte/asset_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -770,16 +770,16 @@
                 ]
                 check.invariant(
                     len(state_files) > 0,
                     f"No state files found for connection {connection_name} in {connection_dir}",
                 )
                 check.invariant(
                     len(state_files) <= 1,
-                    "More than one state file found for connection {} in {}, specify a workspace_id"
-                    " to disambiguate".format(connection_name, connection_dir),
+                    f"More than one state file found for connection {connection_name} in {connection_dir}, specify a workspace_id"
+                    " to disambiguate",
                 )
                 state_file = state_files[0]
 
             with open(os.path.join(connection_dir, cast(str, state_file)), encoding="utf-8") as f:
                 state = yaml.safe_load(f.read())
                 connection_id = state.get("resource_id")
```

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/managed/generated/destinations.py` & `dagster-airbyte-0.23.0/dagster_airbyte/managed/generated/destinations.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/managed/generated/sources.py` & `dagster-airbyte-0.23.0/dagster_airbyte/managed/generated/sources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/managed/reconciliation.py` & `dagster-airbyte-0.23.0/dagster_airbyte/managed/reconciliation.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,17 +727,15 @@
         )
         self._connections: List[AirbyteConnection] = list(connections)
 
     def _get_connections(self) -> Sequence[Tuple[str, AirbyteConnectionMetadata]]:
         diff = reconcile_config(self._airbyte_instance, self._connections, dry_run=True)
         if isinstance(diff, ManagedElementDiff) and not diff.is_empty():
             raise ValueError(
-                "Airbyte connections are not in sync with provided configuration, diff:\n{}".format(
-                    str(diff)
-                )
+                f"Airbyte connections are not in sync with provided configuration, diff:\n{diff!s}"
             )
         elif isinstance(diff, ManagedElementError):
             raise ValueError(f"Error checking Airbyte connections: {diff}")
 
         return super()._get_connections()
```

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/managed/types.py` & `dagster-airbyte-0.23.0/dagster_airbyte/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/ops.py` & `dagster-airbyte-0.23.0/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/resources.py` & `dagster-airbyte-0.23.0/dagster_airbyte/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/types.py` & `dagster-airbyte-0.23.0/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte/utils.py` & `dagster-airbyte-0.23.0/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-0.23.0/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.22.9/dagster_airbyte.egg-info/SOURCES.txt` & `dagster-airbyte-0.23.0/dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.22.9/setup.py` & `dagster-airbyte-0.23.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airbyte_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.6.9",
+        "dagster==1.7.0",
         "requests",
     ],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-airbyte = dagster_airbyte.cli:main",
         ]
     },
     extras_require={
         "test": [
             "requests-mock",
         ],
         "managed": [
-            "dagster-managed-elements==0.22.9",
+            "dagster-managed-elements==0.23.0",
         ],
     },
 )
```

