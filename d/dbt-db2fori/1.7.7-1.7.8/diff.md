# Comparing `tmp/dbt_db2fori-1.7.7.tar.gz` & `tmp/dbt_db2fori-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_db2fori-1.7.7.tar", max compression
+gzip compressed data, was "dbt_db2fori-1.7.8.tar", max compression
```

## Comparing `dbt_db2fori-1.7.7.tar` & `dbt_db2fori-1.7.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1063 2021-10-17 19:23:28.613106 dbt_db2fori-1.7.7/LICENSE
--rw-r--r--   0        0        0     1317 2024-04-04 05:14:14.858371 dbt_db2fori-1.7.7/README.md
--rw-r--r--   0        0        0       22 2024-04-04 05:12:56.031050 dbt_db2fori-1.7.7/dbt/__init__.py
--rw-r--r--   0        0        0      356 2023-03-02 06:41:54.087569 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/__init__.py
--rw-r--r--   0        0        0       17 2024-04-04 03:45:12.537919 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/__version__.py
--rw-r--r--   0        0        0     1420 2024-04-04 04:31:21.786927 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/column.py
--rw-r--r--   0        0        0     5119 2024-04-04 04:46:50.460933 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/connections.py
--rw-r--r--   0        0        0     4252 2024-04-04 04:50:16.929244 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/impl.py
--rw-r--r--   0        0        0      727 2024-04-04 04:51:59.209068 dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/relation.py
--rw-r--r--   0        0        0       51 2021-10-20 08:48:28.010000 dbt_db2fori-1.7.7/dbt/include/db2_for_i/__init__.py
--rw-r--r--   0        0        0      140 2021-10-20 09:31:24.618814 dbt_db2fori-1.7.7/dbt/include/db2_for_i/dbt_project.yml
--rw-r--r--   0        0        0    10037 2024-04-04 05:10:45.251998 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/adapters.sql
--rw-r--r--   0        0        0      705 2024-04-04 05:12:31.333670 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/apply_grants.sql
--rw-r--r--   0        0        0     4050 2021-10-20 08:57:53.402901 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/catalog.sql
--rw-r--r--   0        0        0     5501 2023-01-15 23:08:34.553851 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql
--rw-r--r--   0        0        0     4667 2024-04-04 05:03:45.076257 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql
--rw-r--r--   0        0        0     6053 2023-01-15 23:08:34.555800 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/seed/seed.sql
--rw-r--r--   0        0        0     8852 2021-10-20 09:12:37.134945 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0        0        0      914 2021-10-20 09:13:33.996765 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0        0        0     2543 2021-10-20 09:17:52.225120 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql
--rw-r--r--   0        0        0     2542 2024-04-04 04:56:31.100171 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/table/table.sql
--rw-r--r--   0        0        0      589 2023-01-15 23:08:34.556422 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql
--rw-r--r--   0        0        0      493 2023-01-15 23:08:34.557021 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/tests/where_subquery.sql
--rw-r--r--   0        0        0     3182 2024-04-04 04:56:17.897863 dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/view/view.sql
--rw-r--r--   0        0        0      600 2024-04-04 04:30:47.422569 dbt_db2fori-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 dbt_db2fori-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2021-10-17 19:23:28.613106 dbt_db2fori-1.7.8/LICENSE
+-rw-r--r--   0        0        0     1317 2024-04-04 05:14:14.858371 dbt_db2fori-1.7.8/README.md
+-rw-r--r--   0        0        0       22 2024-04-04 05:52:06.467134 dbt_db2fori-1.7.8/dbt/__init__.py
+-rw-r--r--   0        0        0      356 2023-03-02 06:41:54.087569 dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/__init__.py
+-rw-r--r--   0        0        0       17 2024-04-04 05:52:26.488334 dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/__version__.py
+-rw-r--r--   0        0        0     1420 2024-04-04 04:31:21.786927 dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/column.py
+-rw-r--r--   0        0        0     5092 2024-04-04 05:51:06.576716 dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/connections.py
+-rw-r--r--   0        0        0     4252 2024-04-04 04:50:16.929244 dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/impl.py
+-rw-r--r--   0        0        0      727 2024-04-04 04:51:59.209068 dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/relation.py
+-rw-r--r--   0        0        0       51 2021-10-20 08:48:28.010000 dbt_db2fori-1.7.8/dbt/include/db2_for_i/__init__.py
+-rw-r--r--   0        0        0      140 2021-10-20 09:31:24.618814 dbt_db2fori-1.7.8/dbt/include/db2_for_i/dbt_project.yml
+-rw-r--r--   0        0        0    10036 2024-04-04 05:49:34.408893 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/adapters.sql
+-rw-r--r--   0        0        0      705 2024-04-04 05:12:31.333670 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/apply_grants.sql
+-rw-r--r--   0        0        0     4050 2021-10-20 08:57:53.402901 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/catalog.sql
+-rw-r--r--   0        0        0     5501 2023-01-15 23:08:34.553851 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0        0        0     4668 2024-04-04 05:50:58.011745 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql
+-rw-r--r--   0        0        0     6053 2023-01-15 23:08:34.555800 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/seed/seed.sql
+-rw-r--r--   0        0        0     8852 2021-10-20 09:12:37.134945 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0        0        0      914 2021-10-20 09:13:33.996765 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0        0        0     2543 2021-10-20 09:17:52.225120 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql
+-rw-r--r--   0        0        0     2542 2024-04-04 04:56:31.100171 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/table/table.sql
+-rw-r--r--   0        0        0      589 2023-01-15 23:08:34.556422 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql
+-rw-r--r--   0        0        0      493 2023-01-15 23:08:34.557021 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/tests/where_subquery.sql
+-rw-r--r--   0        0        0     3182 2024-04-04 04:56:17.897863 dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/view/view.sql
+-rw-r--r--   0        0        0      600 2024-04-04 05:51:52.582205 dbt_db2fori-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 dbt_db2fori-1.7.8/PKG-INFO
```

### Comparing `dbt_db2fori-1.7.7/LICENSE` & `dbt_db2fori-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/README.md` & `dbt_db2fori-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/column.py` & `dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/column.py`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/connections.py` & `dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             logger.debug(f'IBM Db2 error: {str(e)}')
             logger.debug(f'Error running SQL: {str(sql)}')
             raise dbt.exceptions.DbtDatabaseError(str(e))
         except Exception as e:
             self.release()
             logger.debug(f"Error running SQL: {sql}")
             logger.debug("Rolling back transaction.")
-            self.release()
             raise dbt.exceptions.DbtRuntimeError(str(e))
 
 
     @classmethod
     def open(cls, connection):
         if connection.state == "open":
             logger.debug("Connection is already open, skipping open.")
```

### Comparing `dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/impl.py` & `dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/adapters/db2_for_i/relation.py` & `dbt_db2fori-1.7.8/dbt/adapters/db2_for_i/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/adapters.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/adapters.sql`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
-{% macro calse_relation_part(quoting, relation_part) %}
+{% macro case_relation_part(quoting, relation_part) %}
   {% if quoting == False %}
-    {% set relation_part = relation_part | upper -%}
+    {%- set relation_part = relation_part|upper -%}
   {% endif %}
   {{ return(relation_part) }}
 {% endmacro %}
 
 
 {% macro information_schema_name(database) -%}
   qsys2
@@ -165,15 +165,15 @@
 {% macro db2_for_i__rename_relation(from_relation, to_relation) -%}
   {% call statement('rename_relation') -%}
   {% if from_relation.is_table %}
     RENAME TABLE {{ from_relation.quote(schema=False, identifier=False) }} TO {{ to_relation.replace_path(schema=None) }}
   {% endif %}
 
   {% if from_relation.is_view %}
-    {% do exceptions.raise_compiler_error('DB2orI Adapter Error: Renaming of views is not supported') }
+    {% do exceptions.raise_compiler_error('DB2orI Adapter Error: Renaming of views is not supported') %}
   {% endif %}
 
   {%- endcall %}
 {% endmacro %}
 
 
 {% macro db2_for_i__current_timestamp() -%}
```

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/apply_grants.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/catalog.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/incremental/merge.sql`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 {% macro db2_for_i__get_delete_insert_merge_sql(target, source, unique_key, dest_columns) -%}
 
     {%- set dest_cols_csv = get_quoted_csv(dest_columns | map(attribute="name")) -%}
 
     {% if unique_key %}
         {% if unique_key is sequence and unique_key is not string %}
-            DELETE FROM {{target }} AS _target
+            DELETE FROM {{ target }} AS _target
             WHERE EXISTS (
                 SELECT * FROM {{ source }} AS _source
                 WHERE (
                     {% for key in unique_key %}
                         _source.{{ key }} = _target.{{ key }}
                         {{ "and " if not loop.last }}
                     {% endfor %}
```

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/seed/seed.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/table/table.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/dbt/include/db2_for_i/macros/materializations/view/view.sql` & `dbt_db2fori-1.7.8/dbt/include/db2_for_i/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_db2fori-1.7.7/pyproject.toml` & `dbt_db2fori-1.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-db2fori"
-version = "1.7.7"
+version = "1.7.8"
 description = "dbt adapter for IBM db2 for i"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kaysef/dbt-db2fori"
 repository = "https://github.com/kaysef/dbt-db2fori"
 documentation = "https://github.com/kaysef/dbt-db2fori"
 authors = ["Seth O <sdowusu@gmail.com>"]
```

### Comparing `dbt_db2fori-1.7.7/PKG-INFO` & `dbt_db2fori-1.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-db2fori
-Version: 1.7.7
+Version: 1.7.8
 Summary: dbt adapter for IBM db2 for i
 Home-page: https://github.com/kaysef/dbt-db2fori
 License: MIT
 Author: Seth O
 Author-email: sdowusu@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

