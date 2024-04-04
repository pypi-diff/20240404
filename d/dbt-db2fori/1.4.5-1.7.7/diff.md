# Comparing `tmp/dbt_db2fori-1.4.5.tar.gz` & `tmp/dbt_db2fori-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_db2fori-1.4.5.tar", max compression
+gzip compressed data, was "dbt_db2fori-1.7.7.tar", max compression
```

## Comparing `dbt_db2fori-1.4.5.tar` & `dbt_db2fori-1.7.7.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     1063 2021-10-17 19:23:28.613106 dbt_db2fori-1.4.5/LICENSE
--rw-r--r--   0        0        0     1280 2021-10-22 01:03:55.829895 dbt_db2fori-1.4.5/README.md
--rw-r--r--   0        0        0       22 2023-02-01 03:53:39.139502 dbt_db2fori-1.4.5/dbt/__init__.py
--rw-r--r--   0        0        0      356 2023-03-02 06:41:54.087569 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/__init__.py
--rw-r--r--   0        0        0       17 2023-05-31 06:40:33.026887 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/__version__.py
--rw-r--r--   0        0        0     5764 2023-02-01 03:52:27.823841 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/connections.py
--rw-r--r--   0        0        0     4167 2023-02-01 03:21:09.060777 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/impl.py
--rw-r--r--   0        0        0      701 2023-05-31 06:34:29.604677 dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/relation.py
--rw-r--r--   0        0        0       51 2021-10-20 08:48:28.010000 dbt_db2fori-1.4.5/dbt/include/db2_for_i/__init__.py
--rw-r--r--   0        0        0      140 2021-10-20 09:31:24.618814 dbt_db2fori-1.4.5/dbt/include/db2_for_i/dbt_project.yml
--rw-r--r--   0        0        0    11746 2023-01-15 23:08:34.553060 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/adapters.sql
--rw-r--r--   0        0        0     4050 2021-10-20 08:57:53.402901 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/catalog.sql
--rw-r--r--   0        0        0     5501 2023-01-15 23:08:34.553851 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql
--rw-r--r--   0        0        0     4578 2023-01-15 23:08:34.554699 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql
--rw-r--r--   0        0        0     6053 2023-01-15 23:08:34.555800 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/seed/seed.sql
--rw-r--r--   0        0        0     8852 2021-10-20 09:12:37.134945 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0        0        0      914 2021-10-20 09:13:33.996765 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0        0        0     2543 2021-10-20 09:17:52.225120 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql
--rw-r--r--   0        0        0      589 2023-01-15 23:08:34.556422 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql
--rw-r--r--   0        0        0      493 2023-01-15 23:08:34.557021 dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/tests/where_subquery.sql
--rw-r--r--   0        0        0      598 2023-05-31 06:35:35.448664 dbt_db2fori-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 dbt_db2fori-1.4.5/setup.py
--rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 dbt_db2fori-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2021-10-17 19:23:28.613106 dbt_db2fori-1.7.7/LICENSE
+-rw-r--r--   0        0        0     1317 2024-04-04 05:14:14.858371 dbt_db2fori-1.7.7/README.md
+-rw-r--r--   0        0        0       22 2024-04-04 05:12:56.031050 dbt_db2fori-1.7.7/dbt/__init__.py
+-rw-r--r--   0        0        0      356 2023-03-02 06:41:54.087569 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-04 03:45:12.537919 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/__version__.py
+-rw-r--r--   0        0        0     1420 2024-04-04 04:31:21.786927 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/column.py
+-rw-r--r--   0        0        0     5119 2024-04-04 04:46:50.460933 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/connections.py
+-rw-r--r--   0        0        0     4252 2024-04-04 04:50:16.929244 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/impl.py
+-rw-r--r--   0        0        0      727 2024-04-04 04:51:59.209068 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/relation.py
+-rw-r--r--   0        0        0       51 2021-10-20 08:48:28.010000 dbt_db2fori-1.7.7/dbt/include/db2_for_i/__init__.py
+-rw-r--r--   0        0        0      140 2021-10-20 09:31:24.618814 dbt_db2fori-1.7.7/dbt/include/db2_for_i/dbt_project.yml
+-rw-r--r--   0        0        0    10037 2024-04-04 05:10:45.251998 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/adapters.sql
+-rw-r--r--   0        0        0      705 2024-04-04 05:12:31.333670 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/apply_grants.sql
+-rw-r--r--   0        0        0     4050 2021-10-20 08:57:53.402901 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/catalog.sql
+-rw-r--r--   0        0        0     5501 2023-01-15 23:08:34.553851 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0        0        0     4667 2024-04-04 05:03:45.076257 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql
+-rw-r--r--   0        0        0     6053 2023-01-15 23:08:34.555800 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/seed/seed.sql
+-rw-r--r--   0        0        0     8852 2021-10-20 09:12:37.134945 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0        0        0      914 2021-10-20 09:13:33.996765 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0        0        0     2543 2021-10-20 09:17:52.225120 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql
+-rw-r--r--   0        0        0     2542 2024-04-04 04:56:31.100171 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/table/table.sql
+-rw-r--r--   0        0        0      589 2023-01-15 23:08:34.556422 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql
+-rw-r--r--   0        0        0      493 2023-01-15 23:08:34.557021 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/tests/where_subquery.sql
+-rw-r--r--   0        0        0     3182 2024-04-04 04:56:17.897863 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/view/view.sql
+-rw-r--r--   0        0        0      600 2024-04-04 04:30:47.422569 dbt_db2fori-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 dbt_db2fori-1.7.7/PKG-INFO
```

### Comparing `dbt_db2fori-1.4.5/LICENSE` & `dbt_db2fori-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.5/README.md` & `dbt_db2fori-1.7.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 default:
     outputs:
         dev:
             type: db2_for_i
             threads: 4
             driver: IBM i Access ODBC Driver
             system: system
-            username: username
-            password: password
+            username: "{{ env_var('USER_NAME) }}"
+            password: "{{ env_var('PASSWORD) }}"
             database: db
             schema: schema
 
     target: dev
 ```
 
 To report a bug or request a feature, open an [issue](https://github.com/kaysef/dbt-db2fori/issues/new)
```

### Comparing `dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/connections.py` & `dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/connections.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,32 +55,24 @@
     TYPE = 'db2_for_i'
 
     @contextmanager
     def exception_handler(self, sql: str):
         try:
             yield
         except pyodbc.DatabaseError as e:
-            logger.debug(f'Database error: {str(e)} {sql}')
-
-            try:
-                self.release()
-            except pyodbc.Error:
-                logger.debug("Failed to release connection!")
-                pass
-
-            raise dbt.exceptions.DbtDatabaseError(str(e).strip()) from e
-
+            self.release()
+            logger.debug(f'IBM Db2 error: {str(e)}')
+            logger.debug(f'Error running SQL: {str(sql)}')
+            raise dbt.exceptions.DbtDatabaseError(str(e))
         except Exception as e:
+            self.release()
             logger.debug(f"Error running SQL: {sql}")
             logger.debug("Rolling back transaction.")
             self.release()
-            if isinstance(e, dbt.exceptions.DbtRuntimeError):
-                raise
-
-            raise dbt.exceptions.DbtRuntimeError(e)
+            raise dbt.exceptions.DbtRuntimeError(str(e))
 
 
     @classmethod
     def open(cls, connection):
         if connection.state == "open":
             logger.debug("Connection is already open, skipping open.")
             return connection
@@ -127,16 +119,21 @@
 
             raise dbt.exceptions.FailedToConnectError(str(e))
 
         return connection
 
 
     def cancel(self, connection):
+        connection_name = connection.name
         logger.debug("Cancel query")
-        pass
+        try:
+            connection.handle.close()
+        except Exception as e:
+            logger.error("Error closing connection for cancel request")
+            raise Exception(str(e))
 
     def add_begin_query(self):
         pass
 
     def add_commit_query(self):
         pass
 
@@ -184,24 +181,7 @@
 
         return AdapterResponse(
             _message=message,
             rows_affected=rows
         )
 
 
-    def execute(self, sql: str, auto_begin: bool = False, fetch: bool = False) -> Tuple[Union[AdapterResponse, str], agate.Table]:
-        _, cursor = self.add_query(sql, auto_begin)
-        response = self.get_response(cursor)
-        if fetch:
-            # Get the result of the first non-empty result set (if any)
-            while cursor.description is None:
-                if not cursor.nextset(): 
-                    break
-            table = self.get_result_from_cursor(cursor)
-        else:
-            table = dbt.clients.agate_helper.empty_table()
-        # Step through all result sets so we process all errors
-        while cursor.nextset(): 
-            pass
-        return response, table
-
-
```

### Comparing `dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/impl.py` & `dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.db2_for_i import DB2ForIConnectionManager
 import dbt.exceptions
 from dbt.adapters.db2_for_i.relation import DB2ForIRelation
+from dbt.adapters.db2_for_i.column import DB2ForIColumn
 
 import agate
 
 from typing import (
     Optional, List
 )
 
 
 class DB2ForIAdapter(SQLAdapter):
     ConnectionManager = DB2ForIConnectionManager
     Relation = DB2ForIRelation
+    Column = DB2ForIColumn
 
     @classmethod
     def date_function(cls):
         return "current_timestamp"
 
 
     @classmethod
@@ -33,15 +35,15 @@
     def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         return "timestamp"
 
 
     @classmethod
     def convert_boolean_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         # some db2 for i versions do not support boolean data types, so I will use smallint here for now 
-        return "smallint"
+        return "decimal(1)"
 
     @classmethod
     def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))
         return "float" if decimals else "int"
```

### Comparing `dbt_db2fori-1.4.5/dbt/adapters/db2_for_i/relation.py` & `dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/relation.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,13 +13,13 @@
     database: bool = False
     schema: bool = True
     identifier: bool = True
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class DB2ForIRelation(BaseRelation):
-    quote_policy: Policy = field(default_factory = lambda: DB2ForIQuotePolicy())
-    include_policy: Policy = field(default_factory = lambda: DB2ForIIncludePolicy())
+    quote_policy: DB2ForIQuotePolicy = field(default_factory = lambda: DB2ForIQuotePolicy())
+    include_policy: DB2ForIIncludePolicy = field(default_factory = lambda: DB2ForIIncludePolicy())
 
     @staticmethod
     def add_ephemeral_prefix(name: str):
         return f'DBT_CTE__{name}'
```

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/adapters.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/adapters.sql`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+
+{% macro calse_relation_part(quoting, relation_part) %}
+  {% if quoting == False %}
+    {% set relation_part = relation_part | upper -%}
+  {% endif %}
+  {{ return(relation_part) }}
+{% endmacro %}
+
+
 {% macro information_schema_name(database) -%}
   qsys2
 {%- endmacro %}
 
 
 {% macro get_columns_in_query(select_sql) %}
     {% call statement('get_columns_in_query', fetch_result=True, auto_begin=False) -%}
@@ -151,63 +160,22 @@
   ) WITH DATA
 
 {%- endmacro %}
 
 
 {% macro db2_for_i__rename_relation(from_relation, to_relation) -%}
   {% call statement('rename_relation') -%}
-    {#
-      Not possible to rename views in DB2 so we have to do some work. The DDL
-      is selected from syscat.views and a new renamed view is created based on
-      this DDL. Comments is removed from the DDL by using regexp but this could
-      probably be done better.
-    #}
-    BEGIN
-      DECLARE rename_stmt VARCHAR(1000);
-      DECLARE create_stmt VARCHAR(10000);
-      DECLARE delete_stmt VARCHAR(1000);
+  {% if from_relation.is_table %}
+    RENAME TABLE {{ from_relation.quote(schema=False, identifier=False) }} TO {{ to_relation.replace_path(schema=None) }}
+  {% endif %}
+
+  {% if from_relation.is_view %}
+    {% do exceptions.raise_compiler_error('DB2orI Adapter Error: Renaming of views is not supported') }
+  {% endif %}
 
-      IF EXISTS (
-        SELECT TABLE_NAME
-        FROM QSYS2.TABLES
-        WHERE TABLE_NAME = UPPER('{{ from_relation.identifier }}') AND TABLE_SCHEMA = UPPER('{{ from_relation.schema }}') AND TABLE_TYPE LIKE '%TABLE%'
-      ) THEN
-        SET rename_stmt = 'RENAME TABLE {{ from_relation.quote(schema=False, identifier=False) }} TO {{ to_relation.quote(identifier=False).identifier }}';
-        PREPARE stmt FROM rename_stmt;
-        EXECUTE stmt;
-      ELSEIF EXISTS (
-        SELECT TABLE_NAME
-        FROM QSYS2.TABLES
-        WHERE TABLE_NAME = UPPER('{{ from_relation.identifier }}') AND TABLE_SCHEMA = UPPER('{{ from_relation.schema }}') AND TABLE_TYPE = 'VIEW'
-      ) THEN
-        SET create_stmt = (
-          -- improve regexp here, use regexp_replace instead?
-          -- ...or (much better solution if possible) rename view.
-          SELECT
-            CONCAT(
-              'CREATE VIEW {{ to_relation.quote(schema=False, identifier=False) }} AS ',
-              -- remove 'create view as'
-              REGEXP_REPLACE(
-                -- remove comments here (single and multiline)
-                REGEXP_REPLACE(
-                  view_definition, --- This is the column that holds the view
-                  '(/\*(.|[\r\n])*?\*/)|(--(.*|[\r\n]))','', 1, 1, 'i' -- removing comments
-                ),
-                '.*CREATE.+VIEW.+AS', '', 1, 1, 'i' -- removing CREATE (OR REPLACE) VIEW AS'
-              )
-            )
-          FROM QSYS2.VIEWS
-          WHERE TABLE_SCHEMA = UPPER('{{ from_relation.schema }}') AND TABLE_NAME = UPPER('{{ from_relation.identifier }}')
-        );
-        PREPARE stmt FROM create_stmt;
-        EXECUTE stmt;
-        PREPARE stmt FROM 'DROP VIEW {{ from_relation.quote(schema=False, identifier=False) }}';
-        EXECUTE stmt;
-      END IF;
-    END    
   {%- endcall %}
 {% endmacro %}
 
 
 {% macro db2_for_i__current_timestamp() -%}
   CURRENT_TIMESTAMP
 {%- endmacro %}
```

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/catalog.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql`

 * *Files 10% similar despite different names*

```diff
@@ -59,21 +59,23 @@
 
 {% macro db2_for_i__get_delete_insert_merge_sql(target, source, unique_key, dest_columns) -%}
 
     {%- set dest_cols_csv = get_quoted_csv(dest_columns | map(attribute="name")) -%}
 
     {% if unique_key %}
         {% if unique_key is sequence and unique_key is not string %}
-            delete from {{target }}
-            using {{ source }}
-            where (
-                {% for key in unique_key %}
-                    {{ source }}.{{ key }} = {{ target }}.{{ key }}
-                    {{ "and " if not loop.last }}
-                {% endfor %}
+            DELETE FROM {{target }} AS _target
+            WHERE EXISTS (
+                SELECT * FROM {{ source }} AS _source
+                WHERE (
+                    {% for key in unique_key %}
+                        _source.{{ key }} = _target.{{ key }}
+                        {{ "and " if not loop.last }}
+                    {% endfor %}
+                )
             );
         {% else %}
             delete from {{ target }}
             where (
                 {{ unique_key }}) in (
                 select ({{ unique_key }})
                 from {{ source }}
```

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/seed/seed.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.5/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql` & `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.4.5/pyproject.toml` & `dbt_db2fori-1.7.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "dbt-db2fori"
-version = "1.4.5"
+version = "1.7.7"
 description = "dbt adapter for IBM db2 for i"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kaysef/dbt-db2fori"
 repository = "https://github.com/kaysef/dbt-db2fori"
 documentation = "https://github.com/kaysef/dbt-db2fori"
 authors = ["Seth O <sdowusu@gmail.com>"]
 packages = [
     { include = "dbt" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-pyodbc = "^4.0.39"
-dbt-core = "1.4.5"
+python = "^3.12"
+pyodbc = "^5.1.0"
+dbt-core = "^1.7.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dbt_db2fori-1.4.5/PKG-INFO` & `dbt_db2fori-1.7.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: dbt-db2fori
-Version: 1.4.5
+Version: 1.7.7
 Summary: dbt adapter for IBM db2 for i
 Home-page: https://github.com/kaysef/dbt-db2fori
 License: MIT
 Author: Seth O
 Author-email: sdowusu@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dbt-core (==1.4.5)
-Requires-Dist: pyodbc (>=4.0.39,<5.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dbt-core (>=1.7.11,<2.0.0)
+Requires-Dist: pyodbc (>=5.1.0,<6.0.0)
 Project-URL: Documentation, https://github.com/kaysef/dbt-db2fori
 Project-URL: Repository, https://github.com/kaysef/dbt-db2fori
 Description-Content-Type: text/markdown
 
 # dbt-db2fori
 
 A [dbt](https://www.getdbt.com/) adapter for IBM's DB2 for i v7.2+. The connection to the warehouse is through `ODBC` and requires that `pyodbc` is installed. All credits to [dbt-sqlserver adapter](https://github.com/dbt-msft/dbt-sqlserver) and [dbt-ibmdb2](https://github.com/aurany/dbt-ibmdb2) projects that heavily inspired this adapter.
@@ -47,16 +44,16 @@
 default:
     outputs:
         dev:
             type: db2_for_i
             threads: 4
             driver: IBM i Access ODBC Driver
             system: system
-            username: username
-            password: password
+            username: "{{ env_var('USER_NAME) }}"
+            password: "{{ env_var('PASSWORD) }}"
             database: db
             schema: schema
 
     target: dev
 ```
 
 To report a bug or request a feature, open an [issue](https://github.com/kaysef/dbt-db2fori/issues/new)
```

