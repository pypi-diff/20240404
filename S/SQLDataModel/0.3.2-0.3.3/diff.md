# Comparing `tmp/SQLDataModel-0.3.2.tar.gz` & `tmp/SQLDataModel-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.2.tar", last modified: Wed Apr  3 00:30:59 2024, max compression
+gzip compressed data, was "SQLDataModel-0.3.3.tar", last modified: Wed Apr  3 22:34:10 2024, max compression
```

## Comparing `SQLDataModel-0.3.2.tar` & `SQLDataModel-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 00:30:59.002339 SQLDataModel-0.3.2/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.2/LICENSE
--rw-rw-rw-   0        0        0    27185 2024-04-03 00:30:58.991336 SQLDataModel-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.2/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 00:30:59.004340 SQLDataModel-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2312 2024-04-03 00:30:00.000000 SQLDataModel-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 00:30:56.439791 SQLDataModel-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 00:30:58.690779 SQLDataModel-0.3.2/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.2/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.2/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.2/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   541858 2024-04-03 00:30:27.000000 SQLDataModel-0.3.2/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.2/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.2/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.2/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.2/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.2/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-03 00:30:58.896461 SQLDataModel-0.3.2/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.2/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.2/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-03 00:30:58.982960 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27185 2024-04-03 00:30:56.000000 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-03 00:30:56.000000 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 00:30:56.000000 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-03 00:30:56.000000 SQLDataModel-0.3.2/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 00:30:58.916775 SQLDataModel-0.3.2/tests/
--rw-rw-rw-   0        0        0    41468 2024-04-01 21:30:07.000000 SQLDataModel-0.3.2/tests/test_Future.py
--rw-rw-rw-   0        0        0    41471 2024-04-01 21:30:05.000000 SQLDataModel-0.3.2/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.948078 SQLDataModel-0.3.3/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0    27185 2024-04-03 22:34:10.943078 SQLDataModel-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.3/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 22:34:10.949077 SQLDataModel-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2024-04-03 22:33:17.000000 SQLDataModel-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:34:09.587853 SQLDataModel-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.719510 SQLDataModel-0.3.3/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.3/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.3/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.3/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   543039 2024-04-03 22:30:42.000000 SQLDataModel-0.3.3/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.3/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.3/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.3/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.3/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.3/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.873275 SQLDataModel-0.3.3/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.3/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.3/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.939078 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27185 2024-04-03 22:34:09.000000 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-03 22:34:09.000000 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 22:34:09.000000 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-03 22:34:09.000000 SQLDataModel-0.3.3/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 22:34:10.884274 SQLDataModel-0.3.3/tests/
+-rw-rw-rw-   0        0        0    41468 2024-04-01 21:30:07.000000 SQLDataModel-0.3.3/tests/test_Future.py
+-rw-rw-rw-   0        0        0    41471 2024-04-01 21:30:05.000000 SQLDataModel-0.3.3/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.2/LICENSE` & `SQLDataModel-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/PKG-INFO` & `SQLDataModel-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.2
+Version: 0.3.3
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.2/README.md` & `SQLDataModel-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/setup.py` & `SQLDataModel-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.2',
+     version='0.3.3',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
      keywords='SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package',
      license_file='LICENSE',
      long_description=long_description,
```

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/ANSIColor.py` & `SQLDataModel-0.3.3/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/HTMLParser.py` & `SQLDataModel-0.3.3/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/JSONEncoder.py` & `SQLDataModel-0.3.3/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/SQLDataModel.py` & `SQLDataModel-0.3.3/src/SQLDataModel/SQLDataModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,15 +423,15 @@
         try:
             headers_with_sql_dtypes_str = ",".join(f'"{col}" {self.static_py_to_sql_map_dict[headers_to_py_dtypes_dict[col]]}' for col in self.headers)
         except KeyError as e:
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid data type {e}, values in ``data`` must be a list of lists comprised of types 'str', 'int', 'float', 'bytes', 'datetime' or 'bool' ")
             ) from None
         sql_create_stmt = f"""create table if not exists "{self.sql_model}" ("{self.sql_idx}" INTEGER PRIMARY KEY,{headers_with_sql_dtypes_str})"""
-        sql_insert_params = ','.join([f'''cast(nullif(nullif(?,'None'),'') as TEXT)''' if headers_to_py_dtypes_dict[col] in ('str','None','NoneType') else f"cast(nullif(?,'None') as {self.static_py_to_sql_map_dict[headers_to_py_dtypes_dict[col]]})" if headers_to_py_dtypes_dict[col] in ('int','float','bytes') else "datetime(?)" if headers_to_py_dtypes_dict[col] == 'datetime' else "date(?)" if headers_to_py_dtypes_dict[col] == 'date' else "cast(case coalesce(?,'None') when 'None' then null when 'False' then 0 when '0' then 0 when 0 then 0 else 1 end as int)" if headers_to_py_dtypes_dict[col] == 'bool' else "nullif(?,'None')" for col in self.headers])
+        sql_insert_params = ",".join([SQLDataModel.sqlite_cast_type_format(dtype=headers_to_py_dtypes_dict[col], as_binding=True) for col in self.headers])        
         sql_insert_stmt = f"""insert into "{self.sql_model}" ({dyn_add_idx_insert}{','.join([f'"{col}"' for col in self.headers])}) values ({dyn_idx_bind}{sql_insert_params})"""
         self.sql_db_conn = sqlite3.connect(":memory:", uri=True, detect_types=sqlite3.PARSE_DECLTYPES)
         """``sqlite3.Connection``: The in-memory sqlite3 connection object in use by the model."""
         try:
             self.sql_db_conn.execute(sql_create_stmt)
         except sqlite3.OperationalError as e:
             raise SQLProgrammingError(
@@ -694,14 +694,50 @@
                     continue
                 if 'int' in col_type_ocurx and 'float' in col_type_ocurx:
                     parsed_dtypes[cid] = 'float'
                     continue
         return parsed_dtypes
 
     @staticmethod
+    def sqlite_cast_type_format(param:str='?', dtype:Literal['None','int','float','str','bytes','date','datetime','NoneType','bool']='str', as_binding:bool=True, as_alias:bool=False):
+        """
+        Formats the specified param to be cast consistently into the python type specified for insert params or as a named alias param.
+
+        Parameters:
+            ``param`` (str): The parameter to be formatted.
+            ``dtype`` (Literal['None', 'int', 'float', 'str', 'bytes', 'date', 'datetime', 'NoneType', 'bool']): The python data type of the parameter as a string.
+            ``as_binding`` (bool, optional): Whether to format as a binding parameter (default is True).
+            ``as_alias`` (bool, optional): Whether to include an alias for the parameter (default is False).
+
+        Returns:
+            ``str``: The parameter formatted for SQL type casting.
+
+        Note:
+            - This function provides consistent formatting for casting parameters into specific data types for SQLite, changing it will lead to unexpected behaviors.
+        """
+        param_alias =  f'''as "{param}"''' if as_alias else ''''''
+        if dtype in ('str','None','NoneType'):
+            return '''cast(nullif(nullif(?,'None'),'') as TEXT)''' if as_binding else f'''cast(nullif(nullif("{param}",'None'),'') as TEXT) {param_alias}'''
+        elif dtype == 'int':
+            return '''cast(nullif(nullif(?,'None'),'') as INTEGER)''' if as_binding else f'''cast(nullif(nullif("{param}",'None'),'') as INTEGER) {param_alias}'''
+        elif dtype == 'float':
+            return '''cast(nullif(nullif(?,'None'),'') as REAL)''' if as_binding else f'''cast(nullif(nullif("{param}",'None'),'') as REAL) {param_alias}'''
+        elif dtype == 'bytes':
+            return '''cast(nullif(nullif(?,'None'),'') as BLOB)''' if as_binding else f"""cast(CASE WHEN (SUBSTR("{param}",1,2) = 'b''' AND SUBSTR("{param}",-1,1) ='''') THEN SUBSTR("{param}",3,LENGTH("{param}")-3) ELSE nullif(nullif("{param}",'None'),'') END as BLOB) {param_alias} """
+        elif dtype == 'date':
+            return '''DATE(nullif(nullif(?,'None'),''))''' if as_binding else f'''DATE(nullif(nullif("{param}",'None'),'')) {param_alias}'''
+        elif dtype == 'datetime':
+            return '''DATETIME(nullif(nullif(?,'None'),''))''' if as_binding else f'''DATETIME(nullif(nullif("{param}",'None'),'')) {param_alias}'''
+        elif dtype == 'bool':
+            return '''cast(case coalesce(nullif(?,''),'None') when 'None' then null when 'False' then 0 when '0' then 0 when 0 then 0 else 1 end as INTEGER)''' if as_binding else f'''cast(case coalesce(nullif("{param}",''),'None') when 'None' then null when 'False' then 0 when '0' then 0 when 0 then 0 else 1 end as INTEGER) {param_alias}'''
+        else:
+            return '''nullif(nullif(?,'None'),'')''' if as_binding else f'''nullif(nullif("{param}",'None'),'') {param_alias}'''
+
+
+    @staticmethod
     def sqlite_printf_format(column:str, dtype:str, max_pad_width:int, float_precision:int=4, alignment:str=None) -> str:
         """
         Formats SQLite SELECT clauses based on column parameters to provide preformatted fetches, providing most of the formatting for ``repr`` output.
 
         Parameters:
             ``column`` (str): The name of the column.
             ``dtype`` (str): The data type of the column ('float', 'int', 'index', or other).
@@ -8962,15 +8998,15 @@
                 ) from None
         if isinstance(column, str):
             if column not in self.headers:
                 raise ValueError(
                     SQLDataModel.ErrorFormat(f"ValueError: column not found '{column}', column must be in current model, use `get_headers()` to view valid arguments")
                 )
         col_sql_dtype = self.static_py_to_sql_map_dict[dtype]
-        dyn_dtype_cast = f"""cast(nullif(nullif("{column}",'None'),'') as {col_sql_dtype})""" if dtype not in ('bool','bytes','datetime','date','None') else f'datetime("{column}")' if dtype == 'datetime' else f'date("{column}")' if dtype == 'date' else f"""cast(case coalesce(nullif("{column}",''),'None') when 'None' then null when 'False' then 0 when '0' then 0 when 0 then 0 else 1 end as int)""" if dtype == 'bool' else f"""cast(CASE WHEN (SUBSTR("{column}",1,2) = 'b''' AND SUBSTR("{column}",-1,1) ='''') THEN SUBSTR("{column}",3,LENGTH("{column}")-3) ELSE "{column}" END as {col_sql_dtype})""" if dtype == 'bytes' else f"""nullif(trim(nullif("{column}",'None')),'')""" if dtype == 'None' else f'"{column}"'
+        dyn_dtype_cast = SQLDataModel.sqlite_cast_type_format(param=column, dtype=dtype, as_binding=False, as_alias=False)
         update_col_sql = f"""alter table "{self.sql_model}" add column "{column}_x" {col_sql_dtype}; update "{self.sql_model}" set "{column}_x" = {dyn_dtype_cast}; alter table "{self.sql_model}" drop column "{column}"; alter table "{self.sql_model}" rename column "{column}_x" to "{column}";"""
         self.execute_transaction(update_col_sql)
         
     def get_model_name(self) -> str:
         """
         Returns the ``SQLDataModel`` table name currently being used by the model as an alias for any SQL queries executed by the user and internally.
 
@@ -10207,12 +10243,11 @@
             - Unless the returned values are saved as a new column, using this method does not change the underlying column's type currently assigned to it, to modify the column type use :meth:`SQLDataModel.set_column_dtypes()` instead.
             - Any ``None`` or ``null`` values encountered will not be coerced to the specified ``dtype``, see :meth:`SQLDataModel.fillna()` for handling and filling null values appropriately.
         """
         if dtype not in ('bool','bytes','date','datetime','float','int','None','str'):
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: invalid value '{type(dtype).__name__}', argument for `dtype` must be one of 'bool','bytes','date','datetime','float','int','None' or 'str'")
             )        
-        col_sql_dtype = self.static_py_to_sql_map_dict[dtype]
-        str_col_cast = ",".join([f"""cast(nullif(nullif("{col}",'None'),'') as {col_sql_dtype}) as "{col}" """ if dtype not in ('bool','bytes','datetime','date','None') else f'datetime("{col}") as "{col}" ' if dtype == 'datetime' else f'date("{col}") as "{col}" ' if dtype == 'date' else f"""cast(case coalesce(nullif("{col}",''),'None') when 'None' then null when 'False' then 0 when '0' then 0 when 0 then 0 else 1 end as int) as "{col}" """ if dtype == 'bool' else f"""cast(CASE WHEN (SUBSTR("{col}",1,2) = 'b''' AND SUBSTR("{col}",-1,1) ='''') THEN SUBSTR("{col}",3,LENGTH("{col}")-3) ELSE "{col}" END as {col_sql_dtype}) as "{col}" """ if dtype == 'bytes' else f"""nullif(trim(nullif("{col}",'None')),'') as "{col}" """ if dtype == 'None' else f'"{col}" as "{col}" ' for col in self.headers])
+        str_col_cast = ",".join([SQLDataModel.sqlite_cast_type_format(param=col, dtype=dtype, as_binding=False, as_alias=True) for col in self.headers])        
         sql_stmt = " ".join(("select",str_col_cast,f'from "{self.sql_model}"'))
         dtype_dict = {col:dtype for col in self.headers}
         return self.execute_fetch(sql_stmt, dtypes=dtype_dict)
```

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/StandardDeviation.py` & `SQLDataModel-0.3.3/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/converters.py` & `SQLDataModel-0.3.3/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/demo.py` & `SQLDataModel-0.3.3/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/exceptions.py` & `SQLDataModel-0.3.3/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel/extensions/str_utils.c` & `SQLDataModel-0.3.3/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel.egg-info/PKG-INFO` & `SQLDataModel-0.3.3/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.2
+Version: 0.3.3
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.2/src/SQLDataModel.egg-info/SOURCES.txt` & `SQLDataModel-0.3.3/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/tests/test_Future.py` & `SQLDataModel-0.3.3/tests/test_Future.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.2/tests/test_SQLDataModel.py` & `SQLDataModel-0.3.3/tests/test_SQLDataModel.py`

 * *Files identical despite different names*

