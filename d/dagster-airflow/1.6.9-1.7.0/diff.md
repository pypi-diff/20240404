# Comparing `tmp/dagster-airflow-1.6.9.tar.gz` & `tmp/dagster-airflow-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airflow-1.6.9.tar", last modified: Fri Mar  8 00:25:36 2024, max compression
+gzip compressed data, was "dagster-airflow-1.7.0.tar", last modified: Thu Apr  4 19:55:15 2024, max compression
```

## Comparing `dagster-airflow-1.6.9.tar` & `dagster-airflow-1.7.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:36.190116 dagster-airflow-1.6.9/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      105 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      656 2024-03-08 00:25:36.190116 dagster-airflow-1.6.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:36.190116 dagster-airflow-1.6.9/dagster_airflow/
--rw-r--r--   0 root         (0) root         (0)     2474 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3815 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/airflow_dag_converter.py
--rw-r--r--   0 root         (0) root         (0)     7765 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/dagster_asset_factory.py
--rw-r--r--   0 root         (0) root         (0)     8234 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/dagster_factory.py
--rw-r--r--   0 root         (0) root         (0)     3898 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/dagster_job_factory.py
--rw-r--r--   0 root         (0) root         (0)     1763 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/dagster_schedule_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:36.190116 dagster-airflow-1.6.9/dagster_airflow/hooks/
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9070 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/hooks/dagster_hook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:36.190116 dagster-airflow-1.6.9/dagster_airflow/links/
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)      842 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/links/dagster_link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:36.190116 dagster-airflow-1.6.9/dagster_airflow/operators/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/operators/dagster_operator.py
--rw-r--r--   0 root         (0) root         (0)      651 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/patch_airflow_example_dag.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:36.190116 dagster-airflow-1.6.9/dagster_airflow/resources/
--rw-r--r--   0 root         (0) root         (0)      324 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3651 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/resources/airflow_db.py
--rw-r--r--   0 root         (0) root         (0)     3659 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/resources/airflow_ephemeral_db.py
--rw-r--r--   0 root         (0) root         (0)     4037 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/resources/airflow_persistent_db.py
--rw-r--r--   0 root         (0) root         (0)     4496 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/dagster_airflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:36.190116 dagster-airflow-1.6.9/dagster_airflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      656 2024-03-08 00:25:35.000000 dagster-airflow-1.6.9/dagster_airflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2024-03-08 00:25:35.000000 dagster-airflow-1.6.9/dagster_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:25:35.000000 dagster-airflow-1.6.9/dagster_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      168 2024-03-08 00:25:35.000000 dagster-airflow-1.6.9/dagster_airflow.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      551 2024-03-08 00:25:35.000000 dagster-airflow-1.6.9/dagster_airflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-08 00:25:35.000000 dagster-airflow-1.6.9/dagster_airflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      192 2024-03-08 00:25:36.194116 dagster-airflow-1.6.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3111 2024-03-08 00:17:46.000000 dagster-airflow-1.6.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:15.923949 dagster-airflow-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      105 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      656 2024-04-04 19:55:15.923949 dagster-airflow-1.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:15.915949 dagster-airflow-1.7.0/dagster_airflow/
+-rw-r--r--   0 root         (0) root         (0)     2474 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/airflow_dag_converter.py
+-rw-r--r--   0 root         (0) root         (0)     7765 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/dagster_asset_factory.py
+-rw-r--r--   0 root         (0) root         (0)     8234 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/dagster_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/dagster_job_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1763 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/dagster_schedule_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:15.915949 dagster-airflow-1.7.0/dagster_airflow/hooks/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9070 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/hooks/dagster_hook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:15.919949 dagster-airflow-1.7.0/dagster_airflow/links/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/links/dagster_link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:15.919949 dagster-airflow-1.7.0/dagster_airflow/operators/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/operators/dagster_operator.py
+-rw-r--r--   0 root         (0) root         (0)      651 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/patch_airflow_example_dag.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:15.923949 dagster-airflow-1.7.0/dagster_airflow/resources/
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3651 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/resources/airflow_db.py
+-rw-r--r--   0 root         (0) root         (0)     3659 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/resources/airflow_ephemeral_db.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/resources/airflow_persistent_db.py
+-rw-r--r--   0 root         (0) root         (0)     4496 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/dagster_airflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:15.915949 dagster-airflow-1.7.0/dagster_airflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      656 2024-04-04 19:55:15.000000 dagster-airflow-1.7.0/dagster_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-04-04 19:55:15.000000 dagster-airflow-1.7.0/dagster_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:15.000000 dagster-airflow-1.7.0/dagster_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-04 19:55:15.000000 dagster-airflow-1.7.0/dagster_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      551 2024-04-04 19:55:15.000000 dagster-airflow-1.7.0/dagster_airflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-04 19:55:15.000000 dagster-airflow-1.7.0/dagster_airflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2024-04-04 19:55:15.923949 dagster-airflow-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3111 2024-04-04 19:44:08.000000 dagster-airflow-1.7.0/setup.py
```

### Comparing `dagster-airflow-1.6.9/LICENSE` & `dagster-airflow-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/PKG-INFO` & `dagster-airflow-1.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.6.9
+Version: 1.7.0
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-airflow-1.6.9/dagster_airflow/__init__.py` & `dagster-airflow-1.7.0/dagster_airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/airflow_dag_converter.py` & `dagster-airflow-1.7.0/dagster_airflow/airflow_dag_converter.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/dagster_asset_factory.py` & `dagster-airflow-1.7.0/dagster_airflow/dagster_asset_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/dagster_factory.py` & `dagster-airflow-1.7.0/dagster_airflow/dagster_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/dagster_job_factory.py` & `dagster-airflow-1.7.0/dagster_airflow/dagster_job_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from airflow.models.dag import DAG
 from dagster import (
     GraphDefinition,
     JobDefinition,
     ResourceDefinition,
     _check as check,
 )
-from dagster._core.definitions.utils import validate_tags
+from dagster._core.definitions.utils import normalize_tags
 from dagster._core.instance import IS_AIRFLOW_INGEST_PIPELINE_STR
 
 from dagster_airflow.airflow_dag_converter import get_graph_definition_args
 from dagster_airflow.resources import (
     make_ephemeral_airflow_db_resource as make_ephemeral_airflow_db_resource,
 )
 from dagster_airflow.utils import (
@@ -73,15 +73,15 @@
     tags = check.opt_mapping_param(tags, "tags")
     connections = check.opt_list_param(connections, "connections", of_type=Connection)
 
     mutated_tags = dict(tags)
     if IS_AIRFLOW_INGEST_PIPELINE_STR not in tags:
         mutated_tags[IS_AIRFLOW_INGEST_PIPELINE_STR] = "true"
 
-    mutated_tags = validate_tags(mutated_tags)
+    mutated_tags = normalize_tags(mutated_tags)
 
     node_dependencies, node_defs = get_graph_definition_args(dag=dag)
 
     graph_def = GraphDefinition(
         name=normalized_name(dag.dag_id),
         description="",
         node_defs=node_defs,
```

### Comparing `dagster-airflow-1.6.9/dagster_airflow/dagster_schedule_factory.py` & `dagster-airflow-1.7.0/dagster_airflow/dagster_schedule_factory.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/hooks/dagster_hook.py` & `dagster-airflow-1.7.0/dagster_airflow/hooks/dagster_hook.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/links/dagster_link.py` & `dagster-airflow-1.7.0/dagster_airflow/links/dagster_link.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/operators/dagster_operator.py` & `dagster-airflow-1.7.0/dagster_airflow/operators/dagster_operator.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/patch_airflow_example_dag.py` & `dagster-airflow-1.7.0/dagster_airflow/patch_airflow_example_dag.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/resources/airflow_db.py` & `dagster-airflow-1.7.0/dagster_airflow/resources/airflow_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/resources/airflow_ephemeral_db.py` & `dagster-airflow-1.7.0/dagster_airflow/resources/airflow_ephemeral_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/resources/airflow_persistent_db.py` & `dagster-airflow-1.7.0/dagster_airflow/resources/airflow_persistent_db.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow/utils.py` & `dagster-airflow-1.7.0/dagster_airflow/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow.egg-info/PKG-INFO` & `dagster-airflow-1.7.0/dagster_airflow.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airflow
-Version: 1.6.9
+Version: 1.7.0
 Summary: Airflow plugin for Dagster
 Home-page: https://github.com/dagster-io/dagster
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: project-url/documentation, https://docs.dagster.io
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-airflow-1.6.9/dagster_airflow.egg-info/SOURCES.txt` & `dagster-airflow-1.7.0/dagster_airflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airflow-1.6.9/dagster_airflow.egg-info/requires.txt` & `dagster-airflow-1.7.0/dagster_airflow.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dagster==1.6.9
+dagster==1.7.0
 docker<6.0.0,>=5.0.3
 urllib3<2
 lazy_object_proxy
 
 [kubernetes]
 kubernetes>=3.0.0
 cryptography>=2.0.0
```

### Comparing `dagster-airflow-1.6.9/setup.py` & `dagster-airflow-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airflow_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.6.9",
+        "dagster==1.7.0",
         "docker>=5.0.3,<6.0.0",
         "urllib3<2",  # docker version pinned above requires this but has no pin
         "lazy_object_proxy",
     ],
     project_urls={
         # airflow will embed a link this in the providers page UI
         "project-url/documentation": "https://docs.dagster.io",
```

