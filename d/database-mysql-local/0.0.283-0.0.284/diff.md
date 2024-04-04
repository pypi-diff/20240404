# Comparing `tmp/database-mysql-local-0.0.283.tar.gz` & `tmp/database-mysql-local-0.0.284.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-mysql-local-0.0.283.tar", last modified: Fri Mar 29 22:52:40 2024, max compression
+gzip compressed data, was "database-mysql-local-0.0.284.tar", last modified: Thu Apr  4 20:00:35 2024, max compression
```

## Comparing `database-mysql-local-0.0.283.tar` & `database-mysql-local-0.0.284.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:52:40.554223 database-mysql-local-0.0.283/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-29 22:52:40.554223 database-mysql-local-0.0.283/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:52:40.550223 database-mysql-local-0.0.283/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:52:40.554223 database-mysql-local-0.0.283/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38968 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30954 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-03-29 22:52:10.000000 database-mysql-local-0.0.283/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:52:40.554223 database-mysql-local-0.0.283/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-29 22:52:40.000000 database-mysql-local-0.0.283/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-29 22:52:40.000000 database-mysql-local-0.0.283/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 22:52:40.000000 database-mysql-local-0.0.283/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-29 22:52:40.000000 database-mysql-local-0.0.283/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-29 22:52:40.000000 database-mysql-local-0.0.283/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-29 22:51:49.000000 database-mysql-local-0.0.283/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 22:52:40.554223 database-mysql-local-0.0.283/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-29 22:52:13.000000 database-mysql-local-0.0.283/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:00:35.802778 database-mysql-local-0.0.284/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 20:00:35.802778 database-mysql-local-0.0.284/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:00:35.794778 database-mysql-local-0.0.284/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:00:35.798778 database-mysql-local-0.0.284/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38968 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31706 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-04-04 20:00:01.000000 database-mysql-local-0.0.284/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:00:35.802778 database-mysql-local-0.0.284/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 20:00:35.000000 database-mysql-local-0.0.284/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:00:35.802778 database-mysql-local-0.0.284/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-04 19:59:35.000000 database-mysql-local-0.0.284/setup.py
```

### Comparing `database-mysql-local-0.0.283/PKG-INFO` & `database-mysql-local-0.0.284/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.283
+Version: 0.0.284
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database-mysql-local-0.0.283/README.md` & `database-mysql-local-0.0.284/README.md`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/connector.py` & `database-mysql-local-0.0.284/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/constants.py` & `database-mysql-local-0.0.284/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/cursor.py` & `database-mysql-local-0.0.284/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/generic_crud.py` & `database-mysql-local-0.0.284/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/generic_crud_ml.py` & `database-mysql-local-0.0.284/database_mysql_local/src/generic_crud_ml.py`

 * *Files 6% similar despite different names*

```diff
@@ -179,14 +179,15 @@
             cursor.close()
         return table_id, ml_table_id
 
     def upsert_value(self, data_ml_json: dict, table_id: int = None, 
                      data_json_compare: dict = None, lang_code: LangCode = None,
                      is_main: int = 0, data_json: dict = None, table_name: str = None,
                      ml_table_name: str = None, schema_name: str = None,
+                     compare_view_name: str = None,
                      limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> tuple:
         self.schema_name = schema_name or self.schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         id_column_name = GenericCRUD.generate_id_column_name(table_name)
         ml_id_column_name = GenericCRUD.generate_id_column_name(ml_table_name)
 
@@ -195,17 +196,18 @@
         name_compare = name
         if not name:
             raise ValueError("name or title is required for upsert_value")
         if data_json_compare:
             name_compare = data_json_compare.get("title") or data_json_compare.get("name")
 
         table_id = table_id or self.get_id_by_name(table_name=table_name, ml_table_name=ml_table_name, name=name_compare,
-                                                   lang_code=lang_code,
+                                                   lang_code=lang_code, compare_view_name=compare_view_name,
                                                    id_column_name=id_column_name, order_by=order_by)
         ml_table_id = self.get_ml_id_by_name(ml_table_name=ml_table_name, name=name_compare, lang_code=lang_code,
+                                             compare_view_name=compare_view_name,
                                              id_column_name=ml_id_column_name, order_by=order_by)
         if not table_id:
             return self.add_value(data_ml_json=data_ml_json, table_id=table_id, lang_code=lang_code, is_main=is_main,
                                   data_json=data_json, table_name=table_name, ml_table_name=ml_table_name)
         else:
             return self.update_value_by_id(data_ml_json=data_ml_json, ml_table_id=ml_table_id, table_id=table_id,
                                            lang_code=lang_code, is_main=is_main, data_json=data_json,
@@ -213,14 +215,15 @@
                                            ml_table_name=ml_table_name, schema_name=schema_name,
                                            limit=limit, order_by=order_by)
 
     def upsert_value_with_abbreviations(self, data_ml_json: dict,  data_json_compare: dict = None,
                                         table_id: int = None, lang_code: LangCode = None,
                                         data_json: dict = None, table_name: str = None,
                                         ml_table_name: str = None, schema_name: str = None,
+                                        compare_view_name: str = None,
                                         limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> tuple:
         self.schema_name = schema_name or self.schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
         id_column_name = GenericCRUD.generate_id_column_name(table_name)
         ml_id_column_name = GenericCRUD.generate_id_column_name(ml_table_name)
 
@@ -242,17 +245,18 @@
         data_ml_json_with_abbreviation_list = []
         for abbreviation in abbreviations_list:
             data_ml_json_with_abbreviation = data_ml_json.copy()
             data_ml_json_with_abbreviation["title"] = abbreviation
             data_ml_json_with_abbreviation_list.append(data_ml_json_with_abbreviation)
 
         table_id = table_id or self.get_id_by_name(table_name=table_name, ml_table_name=ml_table_name, name=name_compare,
-                                                   lang_code=lang_code,
+                                                   lang_code=lang_code, compare_view_name=compare_view_name,
                                                    id_column_name=id_column_name, order_by=order_by)
         ml_table_id = self.get_ml_id_by_name(ml_table_name=ml_table_name, name=name_compare, lang_code=lang_code,
+                                             compare_view_name=compare_view_name,
                                              id_column_name=ml_id_column_name, order_by=order_by)
         ml_ids_list = []
         if not table_id:
             table_id, ml_table_id = self.add_value(data_ml_json=data_ml_json_with_name, table_id=table_id, lang_code=lang_code,
                                                    is_main=1, data_json=data_json, table_name=table_name,
                                                    ml_table_name=ml_table_name)
             ml_ids_list.append(ml_table_id)
@@ -260,14 +264,15 @@
                 table_id, ml_table_id = self.add_value(data_ml_json=data_ml_json_with_abbreviation, table_id=table_id,
                                                        lang_code=lang_code, is_main=0, data_json=data_json,
                                                        table_name=table_name, ml_table_name=ml_table_name)
                 ml_ids_list.append(ml_table_id)
         else:
             ml_ids_list = self.get_ml_ids_by_id(table_id=table_id, ml_table_name=ml_table_name, lang_code=lang_code,
                                                 id_column_name=id_column_name, ml_id_column_name=ml_id_column_name,
+                                                compare_view_name=compare_view_name,
                                                 order_by=order_by)
             ml_ids_list.remove(ml_table_id)
             table_id, main_ml_table_id = self.update_value_by_id(data_ml_json=data_ml_json_with_name, ml_table_id=ml_table_id,
                                                                  table_id=table_id,
                                                                  lang_code=lang_code, is_main=1, data_json=data_json,
                                                                  table_name=table_name,
                                                                  ml_table_name=ml_table_name, schema_name=schema_name,
@@ -347,66 +352,70 @@
                                                params=(table_id,),
                                                select_clause_value=select_clause_value,
                                                order_by=order_by)
 
         return result
 
     def get_id_by_name(self, name: str, table_name: str = None, ml_table_name: str = None, lang_code: LangCode = None,
-                       id_column_name: str = None, order_by: str = None) -> Optional[int]:
+                       id_column_name: str = None, order_by: str = None,
+                       compare_view_name: str = None) -> Optional[int]:
 
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, name=name)
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
-        ml_view_name = self._get_view_name(ml_table_name)
+        compare_view_name = compare_view_name or self._get_view_name(ml_table_name)
         id_column_name = id_column_name or GenericCRUD.generate_id_column_name(table_name)
         if GenericCRUD.is_column_in_table(self, table_name=ml_table_name, column_name="title"):
-            result = self.select_one_tuple_by_where(view_table_name=ml_view_name,
+            result = self.select_one_tuple_by_where(view_table_name=compare_view_name,
                                                     select_clause_value=id_column_name,
                                                     where="title=%s AND lang_code=%s",
                                                     params=(name, lang_code_str),
                                                     order_by=order_by)
         else:
-            result = self.select_one_tuple_by_where(view_table_name=ml_view_name,
+            result = self.select_one_tuple_by_where(view_table_name=compare_view_name,
                                                     select_clause_value=id_column_name,
                                                     where="`name`=%s AND lang_code=%s",
                                                     params=(name, lang_code_str),
                                                     order_by=order_by)
         if result:
             return result[0]
         else:
             return None
 
     def get_ml_id_by_name(self, name: str, ml_table_name: str = None, lang_code: LangCode = None,
-                          id_column_name: str = None, order_by: str = None) -> Optional[int]:
+                          id_column_name: str = None, order_by: str = None,
+                          compare_view_name: str = None) -> Optional[int]:
 
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, name=name)
         ml_table_name = ml_table_name or self.default_ml_table_name
-        ml_view_name = self._get_view_name(ml_table_name)
+        compare_view_name = compare_view_name or self._get_view_name(ml_table_name)
         ml_id_column_name = id_column_name or GenericCRUD.generate_id_column_name(ml_table_name)
         if GenericCRUD.is_column_in_table(self, table_name=ml_table_name, column_name="title"):
-            result = self.select_one_tuple_by_where(view_table_name=ml_view_name,
+            result = self.select_one_tuple_by_where(view_table_name=compare_view_name,
                                                     select_clause_value=ml_id_column_name,
                                                     where="title=%s AND lang_code=%s",
                                                     params=(name, lang_code_str),
                                                     order_by=order_by)
         else:
-            result = self.select_one_tuple_by_where(view_table_name=ml_view_name,
+            result = self.select_one_tuple_by_where(view_table_name=compare_view_name,
                                                     select_clause_value=ml_id_column_name,
                                                     where="`name`=%s AND lang_code=%s",
                                                     params=(name, lang_code_str),
                                                     order_by=order_by)
         if result:
             return result[0]
         else:
             return None
 
     def get_ml_ids_by_id(self, table_id: int, ml_table_name: str = None, lang_code: LangCode = None,
-                         id_column_name: str = None, ml_id_column_name: str = None, order_by: str = None) -> list:
+                         id_column_name: str = None, ml_id_column_name: str = None, order_by: str = None,
+                         compare_view_name: str = None) -> list:
         lang_code_str = None if lang_code is None else lang_code.value
-        result = self.select_multi_tuple_by_where(view_table_name=self._get_view_name(ml_table_name),
+        compare_view_name = compare_view_name or self._get_view_name(ml_table_name)
+        result = self.select_multi_tuple_by_where(view_table_name=compare_view_name,
                                                   select_clause_value=ml_id_column_name,
                                                   where=f"{id_column_name}=%s AND lang_code=%s",
                                                   params=(table_id, lang_code_str),
                                                   order_by=order_by)
         return [row[0] for row in result]
 
     def delete_by_name(self, name: str,
```

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/generic_mapping.py` & `database-mysql-local-0.0.284/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/point.py` & `database-mysql-local-0.0.284/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/polygon.py` & `database-mysql-local-0.0.284/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/table_definition.py` & `database-mysql-local-0.0.284/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/to_sql_interface.py` & `database-mysql-local-0.0.284/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local/src/utils.py` & `database-mysql-local-0.0.284/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/database_mysql_local.egg-info/PKG-INFO` & `database-mysql-local-0.0.284/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.283
+Version: 0.0.284
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database-mysql-local-0.0.283/database_mysql_local.egg-info/SOURCES.txt` & `database-mysql-local-0.0.284/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-mysql-local-0.0.283/pyproject.toml` & `database-mysql-local-0.0.284/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "database-mysql-local"
-version = "0.0.278" # https://pypi.org/project/database-mysql-local
+version = "0.0.284" # https://pypi.org/project/database-mysql-local
 description = "database-mysql-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
 
 # dephell deps convert --from pyproject.toml --from-format poetry --to setup.py --to-format setuppy
```

### Comparing `database-mysql-local-0.0.283/setup.py` & `database-mysql-local-0.0.284/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from circles_local_database_python to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "circles_local_database_python"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.283',
+    version='0.0.284',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

