# Comparing `tmp/dagster-duckdb-pyspark-0.22.9.tar.gz` & `tmp/dagster-duckdb-pyspark-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pyspark-0.22.9.tar", last modified: Fri Mar  8 00:30:58 2024, max compression
+gzip compressed data, was "dagster-duckdb-pyspark-0.23.0.tar", last modified: Thu Apr  4 19:54:02 2024, max compression
```

## Comparing `dagster-duckdb-pyspark-0.22.9.tar` & `dagster-duckdb-pyspark-0.23.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:30:58.766902 dagster-duckdb-pyspark-0.22.9/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagster-duckdb-pyspark-0.22.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2024-03-08 00:17:46.000000 dagster-duckdb-pyspark-0.22.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      623 2024-03-08 00:30:58.766902 dagster-duckdb-pyspark-0.22.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2024-03-08 00:17:46.000000 dagster-duckdb-pyspark-0.22.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:30:58.762902 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark/
--rw-r--r--   0 root         (0) root         (0)      382 2024-03-08 00:17:46.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9588 2024-03-08 00:17:46.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-08 00:17:46.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:30:58.766902 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      623 2024-03-08 00:30:58.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2024-03-08 00:30:58.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:30:58.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:30:58.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       68 2024-03-08 00:30:58.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:30:58.000000 dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      133 2024-03-08 00:30:58.766902 dagster-duckdb-pyspark-0.22.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1504 2024-03-08 00:17:46.000000 dagster-duckdb-pyspark-0.22.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:02.587461 dagster-duckdb-pyspark-0.23.0/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-duckdb-pyspark-0.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-04 19:44:08.000000 dagster-duckdb-pyspark-0.23.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      623 2024-04-04 19:54:02.587461 dagster-duckdb-pyspark-0.23.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-04 19:44:08.000000 dagster-duckdb-pyspark-0.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:02.587461 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      382 2024-04-04 19:44:08.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9588 2024-04-04 19:44:08.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-04 19:44:08.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:54:02.587461 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      623 2024-04-04 19:54:02.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-04 19:54:02.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:54:02.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:54:02.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-04 19:54:02.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:54:02.000000 dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      133 2024-04-04 19:54:02.591462 dagster-duckdb-pyspark-0.23.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1504 2024-04-04 19:44:08.000000 dagster-duckdb-pyspark-0.23.0/setup.py
```

### Comparing `dagster-duckdb-pyspark-0.22.9/LICENSE` & `dagster-duckdb-pyspark-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.22.9/PKG-INFO` & `dagster-duckdb-pyspark-0.23.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py` & `dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark/duckdb_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pyspark-0.22.9/dagster_duckdb_pyspark.egg-info/PKG-INFO` & `dagster-duckdb-pyspark-0.23.0/dagster_duckdb_pyspark.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pyspark
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for storing PySpark DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pyspark
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pyspark-0.22.9/setup.py` & `dagster-duckdb-pyspark-0.23.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pyspark_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.6.9",
-        "dagster-duckdb==0.22.9",
+        "dagster==1.7.0",
+        "dagster-duckdb==0.23.0",
         "pyspark>=3",
         # Pinned pending duckdb removal of broken pandas import. Pin can be
         # removed as soon as it produces a working build.
         "pandas<2.1",
         "pyarrow",
     ],
     zip_safe=False,
```

