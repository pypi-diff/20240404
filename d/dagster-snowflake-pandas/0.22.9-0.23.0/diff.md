# Comparing `tmp/dagster-snowflake-pandas-0.22.9.tar.gz` & `tmp/dagster-snowflake-pandas-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pandas-0.22.9.tar", last modified: Fri Mar  8 00:29:21 2024, max compression
+gzip compressed data, was "dagster-snowflake-pandas-0.23.0.tar", last modified: Thu Apr  4 19:53:52 2024, max compression
```

## Comparing `dagster-snowflake-pandas-0.22.9.tar` & `dagster-snowflake-pandas-0.23.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:29:21.039868 dagster-snowflake-pandas-0.22.9/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagster-snowflake-pandas-0.22.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2024-03-08 00:17:46.000000 dagster-snowflake-pandas-0.22.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      739 2024-03-08 00:29:21.039868 dagster-snowflake-pandas-0.22.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2024-03-08 00:17:46.000000 dagster-snowflake-pandas-0.22.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:29:21.039868 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas/
--rw-r--r--   0 root         (0) root         (0)      413 2024-03-08 00:17:46.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-08 00:17:46.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)    12882 2024-03-08 00:17:46.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:29:21.039868 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      739 2024-03-08 00:29:20.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-03-08 00:29:20.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:29:20.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:29:20.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      144 2024-03-08 00:29:20.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-08 00:29:20.000000 dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2024-03-08 00:29:21.043868 dagster-snowflake-pandas-0.22.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1637 2024-03-08 00:17:46.000000 dagster-snowflake-pandas-0.22.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:52.491394 dagster-snowflake-pandas-0.23.0/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-snowflake-pandas-0.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-04 19:44:08.000000 dagster-snowflake-pandas-0.23.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      739 2024-04-04 19:53:52.491394 dagster-snowflake-pandas-0.23.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2024-04-04 19:44:08.000000 dagster-snowflake-pandas-0.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:52.491394 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas/
+-rw-r--r--   0 root         (0) root         (0)      413 2024-04-04 19:44:08.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)    12875 2024-04-04 19:44:08.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:53:52.491394 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      739 2024-04-04 19:53:52.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-04-04 19:53:52.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:53:52.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:53:52.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      144 2024-04-04 19:53:52.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-04 19:53:52.000000 dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2024-04-04 19:53:52.491394 dagster-snowflake-pandas-0.23.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1637 2024-04-04 19:44:08.000000 dagster-snowflake-pandas-0.23.0/setup.py
```

### Comparing `dagster-snowflake-pandas-0.22.9/LICENSE` & `dagster-snowflake-pandas-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pandas-0.22.9/PKG-INFO` & `dagster-snowflake-pandas-0.23.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas/snowflake_pandas_type_handler.py` & `dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas/snowflake_pandas_type_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,22 +114,22 @@
                 axis="index",
             )
 
         write_pandas(
             conn=connection,
             df=with_uppercase_cols,
             # originally we used pd.to_sql with pd_writer method to write the df to snowflake. pd_writer
-            # forced the table name to be uppercase, so we mimic that behavior here for feature parity
-            # in the future we could allow non-uppercase table names
+            # forced the database, schema, and table name to be uppercase, so we mimic that behavior here for feature parity
+            # in the future we could allow non-uppercase names
             table_name=table_slice.table.upper(),
-            schema=table_slice.schema,
-            database=table_slice.database,
+            schema=table_slice.schema.upper(),
+            database=table_slice.database.upper() if table_slice.database else None,
             auto_create_table=True,
             use_logical_type=True,
-            quote_identifiers=False,  # In the future we can set this to True to allow lowercase identifiers
+            quote_identifiers=True,
         )
 
         return {
             "row_count": obj.shape[0],
             "dataframe_columns": MetadataValue.table_schema(
                 TableSchema(
                     columns=[
```

### Comparing `dagster-snowflake-pandas-0.22.9/dagster_snowflake_pandas.egg-info/PKG-INFO` & `dagster-snowflake-pandas-0.23.0/dagster_snowflake_pandas.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.22.9
+Version: 0.23.0
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pandas-0.22.9/setup.py` & `dagster-snowflake-pandas-0.23.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pandas_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.6.9",
-        "dagster-snowflake==0.22.9",
+        "dagster==1.7.0",
+        "dagster-snowflake==0.23.0",
         "pandas",
         "requests",
         "snowflake-connector-python[pandas]>=3.4.0",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
```

