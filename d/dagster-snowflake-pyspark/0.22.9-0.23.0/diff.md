# Comparing `tmp/dagster-snowflake-pyspark-0.22.9.tar.gz` & `tmp/dagster-snowflake-pyspark-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pyspark-0.22.9.tar", last modified: Fri Mar  8 00:25:55 2024, max compression
+gzip compressed data, was "dagster-snowflake-pyspark-0.23.0.tar", last modified: Thu Apr  4 19:55:36 2024, max compression
```

## Comparing `dagster-snowflake-pyspark-0.22.9.tar` & `dagster-snowflake-pyspark-0.23.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:55.773923 dagster-snowflake-pyspark-0.22.9/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-08 00:17:46.000000 dagster-snowflake-pyspark-0.22.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       77 2024-03-08 00:17:46.000000 dagster-snowflake-pyspark-0.22.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      640 2024-03-08 00:25:55.773923 dagster-snowflake-pyspark-0.22.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      161 2024-03-08 00:17:46.000000 dagster-snowflake-pyspark-0.22.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:55.773923 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark/
--rw-r--r--   0 root         (0) root         (0)      421 2024-03-08 00:17:46.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-08 00:17:46.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)    10896 2024-03-08 00:17:46.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:25:55.773923 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      640 2024-03-08 00:25:55.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      510 2024-03-08 00:25:55.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:25:55.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:25:55.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      103 2024-03-08 00:25:55.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-08 00:25:55.000000 dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-08 00:25:55.773923 dagster-snowflake-pyspark-0.22.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1503 2024-03-08 00:17:46.000000 dagster-snowflake-pyspark-0.22.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:36.700088 dagster-snowflake-pyspark-0.23.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-04 19:44:08.000000 dagster-snowflake-pyspark-0.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-04 19:44:08.000000 dagster-snowflake-pyspark-0.23.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      640 2024-04-04 19:55:36.700088 dagster-snowflake-pyspark-0.23.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-04 19:44:08.000000 dagster-snowflake-pyspark-0.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:36.700088 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      421 2024-04-04 19:44:08.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10896 2024-04-04 19:44:08.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:55:36.700088 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      640 2024-04-04 19:55:36.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      510 2024-04-04 19:55:36.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:36.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:55:36.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      103 2024-04-04 19:55:36.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-04 19:55:36.000000 dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-04 19:55:36.700088 dagster-snowflake-pyspark-0.23.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1503 2024-04-04 19:44:08.000000 dagster-snowflake-pyspark-0.23.0/setup.py
```

### Comparing `dagster-snowflake-pyspark-0.22.9/LICENSE` & `dagster-snowflake-pyspark-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pyspark-0.22.9/PKG-INFO` & `dagster-snowflake-pyspark-0.23.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py` & `dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark/snowflake_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pyspark-0.22.9/dagster_snowflake_pyspark.egg-info/PKG-INFO` & `dagster-snowflake-pyspark-0.23.0/dagster_snowflake_pyspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pyspark
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for integrating Snowflake and PySpark with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pyspark-0.22.9/setup.py` & `dagster-snowflake-pyspark-0.23.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pyspark_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.6.9",
-        "dagster-snowflake==0.22.9",
+        "dagster==1.7.0",
+        "dagster-snowflake==0.23.0",
         "pyspark",
         "requests",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
 )
```

