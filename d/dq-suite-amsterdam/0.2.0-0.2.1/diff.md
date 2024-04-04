# Comparing `tmp/dq-suite-amsterdam-0.2.0.tar.gz` & `tmp/dq-suite-amsterdam-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dq-suite-amsterdam-0.2.0.tar", last modified: Fri Jan 12 15:14:50 2024, max compression
+gzip compressed data, was "dq-suite-amsterdam-0.2.1.tar", last modified: Thu Apr  4 11:48:29 2024, max compression
```

## Comparing `dq-suite-amsterdam-0.2.0.tar` & `dq-suite-amsterdam-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:14:50.347958 dq-suite-amsterdam-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-01-12 15:14:50.347958 dq-suite-amsterdam-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-01-12 15:14:42.000000 dq-suite-amsterdam-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-01-12 15:14:42.000000 dq-suite-amsterdam-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 15:14:50.347958 dq-suite-amsterdam-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:14:50.343958 dq-suite-amsterdam-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:14:50.347958 dq-suite-amsterdam-0.2.0/src/dq_suite/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-12 15:14:42.000000 dq-suite-amsterdam-0.2.0/src/dq_suite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-01-12 15:14:42.000000 dq-suite-amsterdam-0.2.0/src/dq_suite/df_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-12 15:14:42.000000 dq-suite-amsterdam-0.2.0/src/dq_suite/input_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-01-12 15:14:42.000000 dq-suite-amsterdam-0.2.0/src/dq_suite/output_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 15:14:50.347958 dq-suite-amsterdam-0.2.0/src/dq_suite_amsterdam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-01-12 15:14:50.000000 dq-suite-amsterdam-0.2.0/src/dq_suite_amsterdam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-12 15:14:50.000000 dq-suite-amsterdam-0.2.0/src/dq_suite_amsterdam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 15:14:50.000000 dq-suite-amsterdam-0.2.0/src/dq_suite_amsterdam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-12 15:14:50.000000 dq-suite-amsterdam-0.2.0/src/dq_suite_amsterdam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:48:29.217238 dq-suite-amsterdam-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-04 11:48:29.217238 dq-suite-amsterdam-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 11:48:25.000000 dq-suite-amsterdam-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-04 11:48:25.000000 dq-suite-amsterdam-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 11:48:29.217238 dq-suite-amsterdam-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:48:29.213238 dq-suite-amsterdam-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:48:29.217238 dq-suite-amsterdam-0.2.1/src/dq_suite/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-04 11:48:25.000000 dq-suite-amsterdam-0.2.1/src/dq_suite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-04 11:48:25.000000 dq-suite-amsterdam-0.2.1/src/dq_suite/df_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-04 11:48:25.000000 dq-suite-amsterdam-0.2.1/src/dq_suite/input_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-04 11:48:25.000000 dq-suite-amsterdam-0.2.1/src/dq_suite/output_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:48:29.217238 dq-suite-amsterdam-0.2.1/src/dq_suite_amsterdam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-04 11:48:29.000000 dq-suite-amsterdam-0.2.1/src/dq_suite_amsterdam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-04 11:48:29.000000 dq-suite-amsterdam-0.2.1/src/dq_suite_amsterdam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:48:29.000000 dq-suite-amsterdam-0.2.1/src/dq_suite_amsterdam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 11:48:29.000000 dq-suite-amsterdam-0.2.1/src/dq_suite_amsterdam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 11:48:29.000000 dq-suite-amsterdam-0.2.1/src/dq_suite_amsterdam.egg-info/top_level.txt
```

### Comparing `dq-suite-amsterdam-0.2.0/PKG-INFO` & `dq-suite-amsterdam-0.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 Metadata-Version: 2.1
 Name: dq-suite-amsterdam
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wrapper for Great Expectations to fit the requirements of the Gemeente Amsterdam.
 Author-email: Arthur Kordes <a.kordes@amsterdam.nl>, Aysegul Cayir Aydar <a.cayiraydar@amsterdam.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: great_expectations
 
 # Introduction 
-DISCLAIMER: Repo is in PoC phase
-DISCLAIMER: The functions can run on Databricks using a Personal Compute Cluster
+This repository contains functions that will ease the use of Great Expectations. Users can input data and data quality rules and get results in return.
 
-This repository contains functions that will ease the use of Great Expectations. Users can input data and data quality rules and get rules in return.
+DISCLAIMER: Repo is in PoC phase
 
 
 # Getting Started
-Prerequisites:
-
 Run the following code in your workspace:
 
+```
 pip install great_expectations
+```
 
-When working in Databricks you can clone this repo to Databricks Repos. Then you can access it in your workspace using:
+```
+pip install dq-suite-amsterdam
+```
 
-import sys
-sys.path.append("/Workspace/Repos/{user}/{repo_name}")
-from {file} import {function}
-
-Parameter examples:
-user: j.cruijff@amsterdam.nl
-repo_name: dq_repo
-file: df_checker
-function: df_check
+```
+import dq_suite
+```
 
-# Updates
+- Define 'dfs' as a list of dataframes that require a dq check
+- Define 'dq_rules' as a JSON as shown in dq_rules_example.json in this repo
+
+```
+results, brontabel_df, bronattribute_df, dqRegel_df = dq_suite.df_check(dfs, dq_rules, "showcase")
+```
 
+
+# Known exceptions
+The functions can run on Databricks using a Personal Compute Cluster or using a Job Cluster. Using a Shared Compute Cluster will results in an error, as it does not have the permissions that Great Expectations requires.
+
+
+# Updates
 version = "0.1.0" :
 dq_rules_example.json is updated.
 Added:
 "dataframe_parameters": {
         "unique_identifier": "id"
     }
```

### Comparing `dq-suite-amsterdam-0.2.0/README.md` & `dq-suite-amsterdam-0.2.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 # Introduction 
-DISCLAIMER: Repo is in PoC phase
-DISCLAIMER: The functions can run on Databricks using a Personal Compute Cluster
+This repository contains functions that will ease the use of Great Expectations. Users can input data and data quality rules and get results in return.
 
-This repository contains functions that will ease the use of Great Expectations. Users can input data and data quality rules and get rules in return.
+DISCLAIMER: Repo is in PoC phase
 
 
 # Getting Started
-Prerequisites:
-
 Run the following code in your workspace:
 
+```
 pip install great_expectations
+```
 
-When working in Databricks you can clone this repo to Databricks Repos. Then you can access it in your workspace using:
+```
+pip install dq-suite-amsterdam
+```
 
-import sys
-sys.path.append("/Workspace/Repos/{user}/{repo_name}")
-from {file} import {function}
-
-Parameter examples:
-user: j.cruijff@amsterdam.nl
-repo_name: dq_repo
-file: df_checker
-function: df_check
+```
+import dq_suite
+```
 
-# Updates
+- Define 'dfs' as a list of dataframes that require a dq check
+- Define 'dq_rules' as a JSON as shown in dq_rules_example.json in this repo
+
+```
+results, brontabel_df, bronattribute_df, dqRegel_df = dq_suite.df_check(dfs, dq_rules, "showcase")
+```
 
+
+# Known exceptions
+The functions can run on Databricks using a Personal Compute Cluster or using a Job Cluster. Using a Shared Compute Cluster will results in an error, as it does not have the permissions that Great Expectations requires.
+
+
+# Updates
 version = "0.1.0" :
 dq_rules_example.json is updated.
 Added:
 "dataframe_parameters": {
         "unique_identifier": "id"
     }
 
@@ -50,8 +56,8 @@
                             "min_value": 6,
                             "max_value": 10000
                         }
                     ]
                 }
             ]
         },
-        ....
+        ....
```

### Comparing `dq-suite-amsterdam-0.2.0/src/dq_suite/df_checker.py` & `dq-suite-amsterdam-0.2.1/src/dq_suite/df_checker.py`

 * *Files identical despite different names*

### Comparing `dq-suite-amsterdam-0.2.0/src/dq_suite/input_validator.py` & `dq-suite-amsterdam-0.2.1/src/dq_suite/input_validator.py`

 * *Files identical despite different names*

### Comparing `dq-suite-amsterdam-0.2.0/src/dq_suite/output_transformations.py` & `dq-suite-amsterdam-0.2.1/src/dq_suite/output_transformations.py`

 * *Files identical despite different names*

### Comparing `dq-suite-amsterdam-0.2.0/src/dq_suite_amsterdam.egg-info/PKG-INFO` & `dq-suite-amsterdam-0.2.1/src/dq_suite_amsterdam.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 Metadata-Version: 2.1
 Name: dq-suite-amsterdam
-Version: 0.2.0
+Version: 0.2.1
 Summary: Wrapper for Great Expectations to fit the requirements of the Gemeente Amsterdam.
 Author-email: Arthur Kordes <a.kordes@amsterdam.nl>, Aysegul Cayir Aydar <a.cayiraydar@amsterdam.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: great_expectations
 
 # Introduction 
-DISCLAIMER: Repo is in PoC phase
-DISCLAIMER: The functions can run on Databricks using a Personal Compute Cluster
+This repository contains functions that will ease the use of Great Expectations. Users can input data and data quality rules and get results in return.
 
-This repository contains functions that will ease the use of Great Expectations. Users can input data and data quality rules and get rules in return.
+DISCLAIMER: Repo is in PoC phase
 
 
 # Getting Started
-Prerequisites:
-
 Run the following code in your workspace:
 
+```
 pip install great_expectations
+```
 
-When working in Databricks you can clone this repo to Databricks Repos. Then you can access it in your workspace using:
+```
+pip install dq-suite-amsterdam
+```
 
-import sys
-sys.path.append("/Workspace/Repos/{user}/{repo_name}")
-from {file} import {function}
-
-Parameter examples:
-user: j.cruijff@amsterdam.nl
-repo_name: dq_repo
-file: df_checker
-function: df_check
+```
+import dq_suite
+```
 
-# Updates
+- Define 'dfs' as a list of dataframes that require a dq check
+- Define 'dq_rules' as a JSON as shown in dq_rules_example.json in this repo
+
+```
+results, brontabel_df, bronattribute_df, dqRegel_df = dq_suite.df_check(dfs, dq_rules, "showcase")
+```
 
+
+# Known exceptions
+The functions can run on Databricks using a Personal Compute Cluster or using a Job Cluster. Using a Shared Compute Cluster will results in an error, as it does not have the permissions that Great Expectations requires.
+
+
+# Updates
 version = "0.1.0" :
 dq_rules_example.json is updated.
 Added:
 "dataframe_parameters": {
         "unique_identifier": "id"
     }
```

