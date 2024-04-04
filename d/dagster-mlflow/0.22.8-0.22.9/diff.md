# Comparing `tmp/dagster-mlflow-0.22.8.tar.gz` & `tmp/dagster-mlflow-0.22.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mlflow-0.22.8.tar", last modified: Fri Mar  1 19:32:13 2024, max compression
+gzip compressed data, was "dagster-mlflow-0.22.9.tar", last modified: Fri Mar  8 00:31:50 2024, max compression
```

## Comparing `dagster-mlflow-0.22.8.tar` & `dagster-mlflow-0.22.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:32:13.847762 dagster-mlflow-0.22.8/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      607 2024-03-01 19:32:13.847762 dagster-mlflow-0.22.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:32:13.847762 dagster-mlflow-0.22.8/dagster_mlflow/
--rw-r--r--   0 root         (0) root         (0)      303 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/dagster_mlflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/dagster_mlflow/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/dagster_mlflow/py.typed
--rw-r--r--   0 root         (0) root         (0)    10923 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/dagster_mlflow/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/dagster_mlflow/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 19:32:13.847762 dagster-mlflow-0.22.8/dagster_mlflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      607 2024-03-01 19:32:13.000000 dagster-mlflow-0.22.8/dagster_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      403 2024-03-01 19:32:13.000000 dagster-mlflow-0.22.8/dagster_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 19:32:13.000000 dagster-mlflow-0.22.8/dagster_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 19:32:13.000000 dagster-mlflow-0.22.8/dagster_mlflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-01 19:32:13.000000 dagster-mlflow-0.22.8/dagster_mlflow.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-01 19:32:13.000000 dagster-mlflow-0.22.8/dagster_mlflow.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-03-01 19:32:13.855762 dagster-mlflow-0.22.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1225 2024-03-01 19:11:22.000000 dagster-mlflow-0.22.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:50.258394 dagster-mlflow-0.22.9/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      607 2024-03-08 00:31:50.258394 dagster-mlflow-0.22.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:50.258394 dagster-mlflow-0.22.9/dagster_mlflow/
+-rw-r--r--   0 root         (0) root         (0)      303 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/dagster_mlflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/dagster_mlflow/hooks.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/dagster_mlflow/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10924 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/dagster_mlflow/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/dagster_mlflow/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:50.258394 dagster-mlflow-0.22.9/dagster_mlflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      607 2024-03-08 00:31:50.000000 dagster-mlflow-0.22.9/dagster_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2024-03-08 00:31:50.000000 dagster-mlflow-0.22.9/dagster_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:31:50.000000 dagster-mlflow-0.22.9/dagster_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:31:50.000000 dagster-mlflow-0.22.9/dagster_mlflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       29 2024-03-08 00:31:50.000000 dagster-mlflow-0.22.9/dagster_mlflow.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-03-08 00:31:50.000000 dagster-mlflow-0.22.9/dagster_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-03-08 00:31:50.262394 dagster-mlflow-0.22.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-03-08 00:17:46.000000 dagster-mlflow-0.22.9/setup.py
```

### Comparing `dagster-mlflow-0.22.8/LICENSE` & `dagster-mlflow-0.22.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.22.8/PKG-INFO` & `dagster-mlflow-0.22.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.22.8
+Version: 0.22.9
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.22.8/dagster_mlflow/hooks.py` & `dagster-mlflow-0.22.9/dagster_mlflow/hooks.py`

 * *Files identical despite different names*

### Comparing `dagster-mlflow-0.22.8/dagster_mlflow/resources.py` & `dagster-mlflow-0.22.9/dagster_mlflow/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module contains the mlflow resource provided by the MlFlow
 class. This resource provides an easy way to configure mlflow for logging various
 things from dagster runs.
 """
+
 import atexit
 import sys
 from itertools import islice
 from os import environ
 from typing import Any, Optional
 
 import mlflow
```

### Comparing `dagster-mlflow-0.22.8/dagster_mlflow.egg-info/PKG-INFO` & `dagster-mlflow-0.22.9/dagster_mlflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-mlflow
-Version: 0.22.8
+Version: 0.22.9
 Summary: Package for mlflow Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mlflow
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-mlflow-0.22.8/setup.py` & `dagster-mlflow-0.22.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_mlflow_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.6.8", "mlflow", "pandas"],
+    install_requires=["dagster==1.6.9", "mlflow", "pandas"],
     zip_safe=False,
 )
```

