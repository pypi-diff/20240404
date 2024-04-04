# Comparing `tmp/dagster-wandb-0.22.9.tar.gz` & `tmp/dagster-wandb-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-wandb-0.22.9.tar", last modified: Fri Mar  8 00:29:26 2024, max compression
+gzip compressed data, was "dagster-wandb-0.23.0.tar", last modified: Thu Apr  4 19:55:11 2024, max compression
```

## Comparing `dagster-wandb-0.22.9.tar` & `dagster-wandb-0.23.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:29:26.019818 dagster-wandb-0.22.9/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      665 2024-03-08 00:29:26.019818 dagster-wandb-0.22.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      151 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:29:26.015818 dagster-wandb-0.22.9/dagster_wandb/
--rw-r--r--   0 root         (0) root         (0)      613 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33981 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:29:26.019818 dagster-wandb-0.22.9/dagster_wandb/launch/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/launch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/launch/configs.py
--rw-r--r--   0 root         (0) root         (0)     5153 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/launch/ops.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/py.typed
--rw-r--r--   0 root         (0) root         (0)     2272 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/resources.py
--rw-r--r--   0 root         (0) root         (0)      774 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:29:26.019818 dagster-wandb-0.22.9/dagster_wandb/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2744 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/utils/errors.py
--rw-r--r--   0 root         (0) root         (0)     7890 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/utils/pickling.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/dagster_wandb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:29:26.019818 dagster-wandb-0.22.9/dagster_wandb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      665 2024-03-08 00:29:25.000000 dagster-wandb-0.22.9/dagster_wandb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      607 2024-03-08 00:29:25.000000 dagster-wandb-0.22.9/dagster_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:29:25.000000 dagster-wandb-0.22.9/dagster_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:29:25.000000 dagster-wandb-0.22.9/dagster_wandb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-08 00:29:25.000000 dagster-wandb-0.22.9/dagster_wandb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-03-08 00:29:25.000000 dagster-wandb-0.22.9/dagster_wandb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2024-03-08 00:29:26.019818 dagster-wandb-0.22.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1359 2024-03-08 00:17:46.000000 dagster-wandb-0.22.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.111917 dagster-wandb-0.23.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      665 2024-04-04 19:55:11.111917 dagster-wandb-0.23.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      151 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.103917 dagster-wandb-0.23.0/dagster_wandb/
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34086 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.107917 dagster-wandb-0.23.0/dagster_wandb/launch/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/launch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/launch/configs.py
+-rw-r--r--   0 root         (0) root         (0)     5153 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/launch/ops.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2272 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/resources.py
+-rw-r--r--   0 root         (0) root         (0)      774 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.111917 dagster-wandb-0.23.0/dagster_wandb/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2744 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/utils/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7890 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/utils/pickling.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/dagster_wandb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:11.103917 dagster-wandb-0.23.0/dagster_wandb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      665 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      607 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-04 19:55:10.000000 dagster-wandb-0.23.0/dagster_wandb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-04 19:55:11.111917 dagster-wandb-0.23.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1359 2024-04-04 19:44:08.000000 dagster-wandb-0.23.0/setup.py
```

### Comparing `dagster-wandb-0.22.9/LICENSE` & `dagster-wandb-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/PKG-INFO` & `dagster-wandb-0.23.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-wandb-0.22.9/dagster_wandb/__init__.py` & `dagster-wandb-0.23.0/dagster_wandb/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/dagster_wandb/io_manager.py` & `dagster-wandb-0.23.0/dagster_wandb/io_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 from .version import __version__
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+UNIT_TEST_RUN_ID = "0ab2e48b-6d63-4ff5-b160-662cc60145f4"
+
 
 class Config(TypedDict):
     dagster_run_id: str
     wandb_host: str
     wandb_entity: str
     wandb_project: str
     wandb_run_name: Optional[str]
@@ -157,16 +159,16 @@
                 " partitions at the same time within a single run. Please process each partition"
                 " separately. If you think this might be an error, don't hesitate to reach out to"
                 " Weights & Biases Support."
             )
 
         with self.wandb_run() as run:
             parameters = {}
-            if context.metadata is not None:
-                parameters = context.metadata.get("wandb_artifact_configuration", {})
+            if context.definition_metadata is not None:
+                parameters = context.definition_metadata.get("wandb_artifact_configuration", {})
 
             raise_on_unknown_write_configuration_keys(parameters)
 
             serialization_module = parameters.get("serialization_module", {})
             serialization_module_name = serialization_module.get("name", "pickle")
 
             if serialization_module_name not in ACCEPTED_SERIALIZATION_MODULES:
@@ -360,16 +362,16 @@
                 "wandb_run_url": MetadataValue.url(run.url),
             }
             context.add_output_metadata(output_metadata)
 
     def _download_artifact(self, context: InputContext):
         with self.wandb_run() as run:
             parameters = {}
-            if context.metadata is not None:
-                parameters = context.metadata.get("wandb_artifact_configuration", {})
+            if context.definition_metadata is not None:
+                parameters = context.definition_metadata.get("wandb_artifact_configuration", {})
 
             raise_on_unknown_read_configuration_keys(parameters)
 
             partitions_configuration = parameters.get("partitions", {})
 
             if not context.has_asset_partitions and len(partitions_configuration) > 0:
                 raise WandbArtifactsIOManagerError(
@@ -707,15 +709,15 @@
         wandb_run_name = context.resource_config.get("run_name")
         wandb_run_id = context.resource_config.get("run_id")
         wandb_run_tags = context.resource_config.get("run_tags")
         base_dir = context.resource_config.get("base_dir", base_dir)
         cache_duration_in_minutes = context.resource_config.get("cache_duration_in_minutes")
 
     if "PYTEST_CURRENT_TEST" in os.environ:
-        dagster_run_id = "unit-testing"
+        dagster_run_id = UNIT_TEST_RUN_ID
     else:
         dagster_run_id = context.run_id
 
     assert dagster_run_id is not None
 
     config: Config = {
         "dagster_run_id": dagster_run_id,
```

### Comparing `dagster-wandb-0.22.9/dagster_wandb/launch/configs.py` & `dagster-wandb-0.23.0/dagster_wandb/launch/configs.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/dagster_wandb/launch/ops.py` & `dagster-wandb-0.23.0/dagster_wandb/launch/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/dagster_wandb/resources.py` & `dagster-wandb-0.23.0/dagster_wandb/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/dagster_wandb/types.py` & `dagster-wandb-0.23.0/dagster_wandb/types.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/dagster_wandb/utils/errors.py` & `dagster-wandb-0.23.0/dagster_wandb/utils/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/dagster_wandb/utils/pickling.py` & `dagster-wandb-0.23.0/dagster_wandb/utils/pickling.py`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/dagster_wandb.egg-info/PKG-INFO` & `dagster-wandb-0.23.0/dagster_wandb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-wandb
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for wandb Dagster components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-wandb
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-wandb-0.22.9/dagster_wandb.egg-info/SOURCES.txt` & `dagster-wandb-0.23.0/dagster_wandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-wandb-0.22.9/setup.py` & `dagster-wandb-0.23.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,13 +30,13 @@
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_wandb_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.6.9",
+        "dagster==1.7.0",
         "wandb>=0.15.11,<1.0",
     ],
     extras_require={"dev": ["cloudpickle", "joblib", "callee", "dill"]},
     zip_safe=False,
 )
```

