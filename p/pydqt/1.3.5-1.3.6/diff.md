# Comparing `tmp/pydqt-1.3.5.tar.gz` & `tmp/pydqt-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydqt-1.3.5.tar", max compression
+gzip compressed data, was "pydqt-1.3.6.tar", max compression
```

## Comparing `pydqt-1.3.5.tar` & `pydqt-1.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    16972 2024-02-20 16:09:32.452077 pydqt-1.3.5/README.md
--rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.3.5/pydqt/__init__.py
--rw-r--r--   0        0        0    33523 2024-02-20 16:05:09.092583 pydqt-1.3.5/pydqt/pydqt.py
--rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.3.5/pydqt/sql/templates/macros/macros.jinja
--rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.3.5/pydqt/test.csv
--rw-r--r--   0        0        0     5172 2024-01-05 13:40:57.843834 pydqt-1.3.5/pydqt/tests/test_querying.py
--rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.3.5/pydqt/utils/__init__.py
--rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.3.5/pydqt/utils/custom_filters.py
--rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.3.5/pydqt/workspaces/main/templates/base.sql
--rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.3.5/pydqt/workspaces/main/templates/example.sql
--rw-r--r--   0        0        0      684 2024-02-20 16:09:54.038035 pydqt-1.3.5/pyproject.toml
--rw-r--r--   0        0        0    17868 1970-01-01 00:00:00.000000 pydqt-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0    17339 2024-04-04 14:56:15.673262 pydqt-1.3.6/README.md
+-rw-r--r--   0        0        0     1202 2024-01-21 00:51:50.668840 pydqt-1.3.6/pydqt/__init__.py
+-rw-r--r--   0        0        0    35249 2024-04-04 14:49:31.652917 pydqt-1.3.6/pydqt/pydqt.py
+-rw-r--r--   0        0        0     1976 2023-10-21 17:25:29.558640 pydqt-1.3.6/pydqt/sql/templates/macros/macros.jinja
+-rw-r--r--   0        0        0    15211 2023-10-23 13:44:10.606676 pydqt-1.3.6/pydqt/test.csv
+-rw-r--r--   0        0        0     6669 2024-04-04 14:51:27.612073 pydqt-1.3.6/pydqt/tests/test_querying.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:56:59.448321 pydqt-1.3.6/pydqt/utils/__init__.py
+-rw-r--r--   0        0        0      237 2024-01-18 10:37:58.921832 pydqt-1.3.6/pydqt/utils/custom_filters.py
+-rw-r--r--   0        0        0      319 2024-01-05 09:56:24.111496 pydqt-1.3.6/pydqt/workspaces/main/templates/base.sql
+-rw-r--r--   0        0        0      371 2024-01-05 09:56:27.441110 pydqt-1.3.6/pydqt/workspaces/main/templates/example.sql
+-rw-r--r--   0        0        0      684 2024-04-04 14:57:26.436994 pydqt-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0    18235 1970-01-01 00:00:00.000000 pydqt-1.3.6/PKG-INFO
```

### Comparing `pydqt-1.3.5/README.md` & `pydqt-1.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -277,14 +277,17 @@
 column, which you know is column of date objects and you want this to be preserved on your SQL table.  Then you
 would do:
 
 <pre>
 query.write_sql("my_table", schema="SCHEMA_NAME", append=False, write_timestamp=False, EVENT_DS="DATE")
 </pre>
 
+You can also specify that a column is unique when writing data.  If inserting records this will check both what is already
+there as well as what is being added.  If not append=False, then a new table is created, in which case only the data being
+added is de-duplicated.  The first record of the specified column sorted in ascending order is the one that is retained.
 
 See write_sql help for more details
 
 ### Example 5: testing data
 DQT can test data for simple tests such as non null as well as testing combinations of columns
 
 Get some data:
```

### Comparing `pydqt-1.3.5/pydqt/__init__.py` & `pydqt-1.3.6/pydqt/__init__.py`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.5/pydqt/pydqt.py` & `pydqt-1.3.6/pydqt/pydqt.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class NoDataException(Exception):
     pass
 
 def env_file_full_path():
     return os.path.join(Path(__file__).parents[0],'.env')
 
-def test_data_file_full_path():
+def test_data_file_full_path(dups=True):
     return os.path.join(Path(__file__).parents[0],'test.csv')
 
 def test_data_exists():
     test_data_file = test_data_file_full_path()
     if os.path.exists(test_data_file):
         return True
     return False
@@ -710,15 +710,15 @@
                     else:
                         print('Test failed!')
                         test_report[test["name"]] = "Failed"    
             self.tests[json_file.replace('.json','')] = test_report        
 
 
 
-    def write_sql(self, table, warehouse=get_warehouse(), database=get_database(), schema=get_schema(), append=False, write_timestamp=True, **kwargs):
+    def write_sql(self, table, warehouse=get_warehouse(), database=get_database(), schema=get_schema(), append=False, write_timestamp=True, unique='',**kwargs):
         """
         writes result to sql table.  Note: only works for Snowflake at the moment.  If the table does not exist
         then one is automatically created, which may result in fields being of an unexpected type (eg dates are 
         often converted to integers by Snowflake).  To avoid unexpected results, it is advised to create your table 
         in advance.
 
         This works by opening a new db connection where you can specify the optional params:
@@ -783,29 +783,64 @@
                         sf_dtypes[cols.index(key.upper())] = kwargs[key].upper()
 
             table_metadata = ", ". join([" ".join([y.upper(), x]) for x, y in zip(sf_dtypes, list(df.columns))])
 
             return table_metadata
 
 
-        def df_to_snowflake_table(table_name, operation, df, conn=conn, **kwargs): 
+        def df_to_snowflake_table(table_name, operation, df, conn=conn, unique=unique, **kwargs): 
             if operation=='create_replace':
                 df.columns = [c.upper() for c in df.columns]
                 table_metadata = get_table_metadata(df,**kwargs)
                 conn.cursor().execute(f"CREATE OR REPLACE TABLE {table_name} ({table_metadata})")
+
+                if unique:
+                    assert unique in df.columns, f'"{unique}" is not in the dataframe columns'
+                    df = df.drop_duplicates(subset=[unique])    
                 write_pandas(conn, df, table_name.upper())
             elif operation=='insert':
+                if unique:
+                    assert unique in df.columns, f'"{unique}" is not in the dataframe columns'
+                    df = df.drop_duplicates(subset=[unique])
+
                 table_rows = str(list(df.itertuples(index=False, name=None))).replace('[','').replace(']','')
-                conn.cursor().execute(f"INSERT INTO {table_name} VALUES {table_rows}")
+
+                if unique:
+                    cols = df.columns
+                    temp_table = f't('
+                    for c in cols:
+                        temp_table+=c+','
+                    temp_table = temp_table[:-1] + ')'                        
+                    sql_statement = f"""
+                        INSERT INTO {table_name}
+                        SELECT *
+                        FROM (VALUES
+                            {table_rows}
+                        ) AS {temp_table}
+                        -- Make sure the table doesn't already contain the IDs we're trying to insert
+                        WHERE {unique} NOT IN (
+                        SELECT {unique} FROM {table_name}
+                        )
+                        -- Make sure the data we're inserting doesn't contain duplicate IDs
+                        -- If it does, only the first record will be inserted (based on the ORDER BY)
+                        -- Ideally, we would want to order by a timestamp to select the latest record
+                        QUALIFY ROW_NUMBER() OVER (
+                        PARTITION BY {unique}
+                        ORDER BY {unique} ASC
+                        ) = 1;
+                    """
+                else:
+                    sql_statement = f"INSERT INTO {table_name} VALUES {table_rows}"
+                conn.cursor().execute(sql_statement)
 
         operation = 'create_replace'
         if append==True:
             operation = 'insert'
 
-        df_to_snowflake_table(table, operation, df, conn=conn, **kwargs)
+        df_to_snowflake_table(table, operation, df, conn=conn, unique=unique, **kwargs)
 
         # success, nchunks, nrows, output  = write_pandas(conn=conn,df=self.df,table_name=table,database=database,schema=schema,overwrite=True,quote_identifiers=False,auto_create_table=True)
 
 class Test(Query):
     """
     DQT Test Class
```

### Comparing `pydqt-1.3.5/pydqt/sql/templates/macros/macros.jinja` & `pydqt-1.3.6/pydqt/sql/templates/macros/macros.jinja`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.5/pydqt/test.csv` & `pydqt-1.3.6/pydqt/test.csv`

 * *Files identical despite different names*

### Comparing `pydqt-1.3.5/pydqt/tests/test_querying.py` & `pydqt-1.3.6/pydqt/tests/test_querying.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,14 +64,40 @@
     """
     tests dqt's writing to sql
     """    
     query = Query(query="select * from '{{table}}' limit 10;",table=full_path_test_data_file())
     query.load()
     query.write_sql("dqt_delme_test",schema="CORE_WIP", append=True)
 
+def test_write_sql_unique_on_append():
+    """
+    tests dqt's writing to sql if unique is specified.  This should prevents any duplicates of a particular column
+    """    
+    query = Query(query="select * from '{{table}}' limit 100;",table=full_path_test_data_file())
+    query.load()
+    df_no_dups = query.df.drop_duplicates(subset=['source'])
+    df_to_append = pd.DataFrame(data=np.array([[pd.to_datetime('2022-01-31'),94,584.37,'US','css'],[pd.to_datetime('2022-03-30'),103,523.10,'NZ','new_source']]),columns=['dates','orders','gmv','region','source'])
+    query.df = pd.concat([df_no_dups, df_to_append]).reset_index(drop=True)
+    query.write_sql("dqt_delme_test",schema="CORE_WIP", append=True, unique='source')
+    query_check = Query(query='select * from dqt_delme_test')
+    query_check.run(schema='core_wip', database='lyst')
+    tf = query_check.df.duplicated(subset=['SOURCE'])
+    assert tf.any()==False
+
+def test_write_sql_unique_on_create():
+    """
+    tests dqt's writing to sql if unique is specified.  This should prevents any duplicates of a particular column
+    """    
+    query = Query(query="select * from '{{table}}' limit 10;",table=full_path_test_data_file())
+    query.load()
+    query.write_sql("dqt_delme_test",schema="CORE_WIP", append=False, unique='SOURCE')
+    query_check = Query(query='select * from dqt_delme_test')
+    query_check.run(schema='core_wip', database='lyst')
+    tf = query_check.df.duplicated(subset=['SOURCE'])
+    assert tf.any()==False
 
 def test_macro():
     """
     test a sql command
     """
     if not does_test_data_exist():
         create_test_data()
```

### Comparing `pydqt-1.3.5/pyproject.toml` & `pydqt-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydqt"
-version = "1.3.5"
+version = "1.3.6"
 description = "A package to help parameterise and macrofy sql queries"
 authors = ["Mark Ingham <mark.ingham@ly.st>"]
 readme = "README.md"
 repository = "https://github.com/markingham77/dqt"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `pydqt-1.3.5/PKG-INFO` & `pydqt-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydqt
-Version: 1.3.5
+Version: 1.3.6
 Summary: A package to help parameterise and macrofy sql queries
 Home-page: https://github.com/markingham77/dqt
 License: MIT
 Author: Mark Ingham
 Author-email: mark.ingham@ly.st
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -301,14 +301,17 @@
 column, which you know is column of date objects and you want this to be preserved on your SQL table.  Then you
 would do:
 
 <pre>
 query.write_sql("my_table", schema="SCHEMA_NAME", append=False, write_timestamp=False, EVENT_DS="DATE")
 </pre>
 
+You can also specify that a column is unique when writing data.  If inserting records this will check both what is already
+there as well as what is being added.  If not append=False, then a new table is created, in which case only the data being
+added is de-duplicated.  The first record of the specified column sorted in ascending order is the one that is retained.
 
 See write_sql help for more details
 
 ### Example 5: testing data
 DQT can test data for simple tests such as non null as well as testing combinations of columns
 
 Get some data:
```

