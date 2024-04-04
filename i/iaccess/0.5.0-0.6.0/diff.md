# Comparing `tmp/iaccess-0.5.0.tar.gz` & `tmp/iaccess-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iaccess-0.5.0.tar", last modified: Mon Mar  4 21:40:23 2024, max compression
+gzip compressed data, was "iaccess-0.6.0.tar", last modified: Thu Apr  4 14:27:13 2024, max compression
```

## Comparing `iaccess-0.5.0.tar` & `iaccess-0.6.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 21:40:23.879871 iaccess-0.5.0/
--rw-rw-rw-   0        0        0      184 2021-05-11 17:40:52.000000 iaccess-0.5.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3686 2021-05-11 17:40:52.000000 iaccess-0.5.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      666 2022-04-22 14:26:14.000000 iaccess-0.5.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1101 2021-05-11 17:40:52.000000 iaccess-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      273 2021-05-11 17:40:52.000000 iaccess-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5252 2024-03-04 21:40:23.878870 iaccess-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3645 2021-05-11 17:40:52.000000 iaccess-0.5.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-04 21:40:23.832960 iaccess-0.5.0/docs/
--rw-rw-rw-   0        0        0      628 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/Makefile
--rw-rw-rw-   0        0        0       29 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/authors.rst
--rw-rw-rw-   0        0        0     5056 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/history.rst
--rw-rw-rw-   0        0        0      440 2021-11-18 17:22:34.000000 iaccess-0.5.0/docs/iaccess.information_schema.rst
--rw-rw-rw-   0        0        0     1014 2021-11-18 17:22:34.000000 iaccess-0.5.0/docs/iaccess.rst
--rw-rw-rw-   0        0        0      367 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/index.rst
--rw-rw-rw-   0        0        0     1246 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/installation.rst
--rwxrwxrwx   0        0        0      805 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/make.bat
--rw-rw-rw-   0        0        0       65 2021-11-18 17:22:34.000000 iaccess-0.5.0/docs/modules.rst
--rw-rw-rw-   0        0        0       28 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/readme.rst
--rw-rw-rw-   0        0        0     1852 2021-05-11 17:40:52.000000 iaccess-0.5.0/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2024-03-04 21:40:23.847713 iaccess-0.5.0/iaccess/
--rw-rw-rw-   0        0        0      184 2024-03-04 21:39:40.000000 iaccess-0.5.0/iaccess/__init__.py
--rw-rw-rw-   0        0        0     4118 2021-11-18 17:10:34.000000 iaccess-0.5.0/iaccess/compiler.py
--rw-rw-rw-   0        0        0     1459 2022-04-22 14:26:14.000000 iaccess-0.5.0/iaccess/connector.py
--rw-rw-rw-   0        0        0    14556 2024-03-04 21:31:53.000000 iaccess-0.5.0/iaccess/dialect.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:40:23.865694 iaccess-0.5.0/iaccess/information_schema/
--rw-rw-rw-   0        0        0        0 2021-05-11 17:40:52.000000 iaccess-0.5.0/iaccess/information_schema/__init__.py
--rw-rw-rw-   0        0        0     2957 2021-05-13 13:44:55.000000 iaccess-0.5.0/iaccess/information_schema/iseries.py
--rw-rw-rw-   0        0        0      227 2021-11-18 17:12:54.000000 iaccess-0.5.0/iaccess/provision.py
--rw-rw-rw-   0        0        0     1441 2021-05-12 12:45:29.000000 iaccess-0.5.0/iaccess/requirements.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:40:23.876868 iaccess-0.5.0/iaccess.egg-info/
--rw-rw-rw-   0        0        0     5252 2024-03-04 21:40:23.000000 iaccess-0.5.0/iaccess.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      801 2024-03-04 21:40:23.000000 iaccess-0.5.0/iaccess.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 21:40:23.000000 iaccess-0.5.0/iaccess.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2024-03-04 21:40:23.000000 iaccess-0.5.0/iaccess.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2021-05-11 17:41:25.000000 iaccess-0.5.0/iaccess.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-03-04 21:40:23.000000 iaccess-0.5.0/iaccess.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-04 21:40:23.000000 iaccess-0.5.0/iaccess.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      480 2024-03-04 21:40:23.881867 iaccess-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1863 2021-11-18 01:26:23.000000 iaccess-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-04 21:40:23.872704 iaccess-0.5.0/tests/
--rw-rw-rw-   0        0        0       38 2021-05-11 17:40:52.000000 iaccess-0.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0      443 2021-05-11 17:40:52.000000 iaccess-0.5.0/tests/conftest.py
--rw-rw-rw-   0        0        0     4591 2021-11-18 02:00:25.000000 iaccess-0.5.0/tests/test_suite.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:27:13.735008 iaccess-0.6.0/
+-rw-rw-rw-   0        0        0      184 2021-05-11 17:40:52.000000 iaccess-0.6.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3686 2021-05-11 17:40:52.000000 iaccess-0.6.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      666 2022-04-22 14:26:14.000000 iaccess-0.6.0/HISTORY.rst
+-rw-rw-rw-   0        0        0     1101 2021-05-11 17:40:52.000000 iaccess-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      273 2021-05-11 17:40:52.000000 iaccess-0.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5252 2024-04-04 14:27:13.734005 iaccess-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3645 2021-05-11 17:40:52.000000 iaccess-0.6.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-04 14:27:13.693494 iaccess-0.6.0/docs/
+-rw-rw-rw-   0        0        0      628 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/authors.rst
+-rw-rw-rw-   0        0        0     5056 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/history.rst
+-rw-rw-rw-   0        0        0      440 2021-11-18 17:22:34.000000 iaccess-0.6.0/docs/iaccess.information_schema.rst
+-rw-rw-rw-   0        0        0     1014 2021-11-18 17:22:34.000000 iaccess-0.6.0/docs/iaccess.rst
+-rw-rw-rw-   0        0        0      367 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1246 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      805 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/make.bat
+-rw-rw-rw-   0        0        0       65 2021-11-18 17:22:34.000000 iaccess-0.6.0/docs/modules.rst
+-rw-rw-rw-   0        0        0       28 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/readme.rst
+-rw-rw-rw-   0        0        0     1852 2021-05-11 17:40:52.000000 iaccess-0.6.0/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2024-04-04 14:27:13.707007 iaccess-0.6.0/iaccess/
+-rw-rw-rw-   0        0        0      168 2024-04-04 14:26:58.000000 iaccess-0.6.0/iaccess/__init__.py
+-rw-rw-rw-   0        0        0     4118 2021-11-18 17:10:34.000000 iaccess-0.6.0/iaccess/compiler.py
+-rw-rw-rw-   0        0        0     1459 2022-04-22 14:26:14.000000 iaccess-0.6.0/iaccess/connector.py
+-rw-rw-rw-   0        0        0    14582 2024-04-04 14:11:15.000000 iaccess-0.6.0/iaccess/dialect.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:27:13.723026 iaccess-0.6.0/iaccess/information_schema/
+-rw-rw-rw-   0        0        0        0 2021-05-11 17:40:52.000000 iaccess-0.6.0/iaccess/information_schema/__init__.py
+-rw-rw-rw-   0        0        0     2957 2021-05-13 13:44:55.000000 iaccess-0.6.0/iaccess/information_schema/iseries.py
+-rw-rw-rw-   0        0        0      227 2021-11-18 17:12:54.000000 iaccess-0.6.0/iaccess/provision.py
+-rw-rw-rw-   0        0        0     1441 2021-05-12 12:45:29.000000 iaccess-0.6.0/iaccess/requirements.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:27:13.732005 iaccess-0.6.0/iaccess.egg-info/
+-rw-rw-rw-   0        0        0     5252 2024-04-04 14:27:13.000000 iaccess-0.6.0/iaccess.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2024-04-04 14:27:13.000000 iaccess-0.6.0/iaccess.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 14:27:13.000000 iaccess-0.6.0/iaccess.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2024-04-04 14:27:13.000000 iaccess-0.6.0/iaccess.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2021-05-11 17:41:25.000000 iaccess-0.6.0/iaccess.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-04-04 14:27:13.000000 iaccess-0.6.0/iaccess.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 14:27:13.000000 iaccess-0.6.0/iaccess.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      480 2024-04-04 14:27:13.736006 iaccess-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1863 2021-11-18 01:26:23.000000 iaccess-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:27:13.729007 iaccess-0.6.0/tests/
+-rw-rw-rw-   0        0        0       38 2021-05-11 17:40:52.000000 iaccess-0.6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      443 2021-05-11 17:40:52.000000 iaccess-0.6.0/tests/conftest.py
+-rw-rw-rw-   0        0        0     4591 2021-11-18 02:00:25.000000 iaccess-0.6.0/tests/test_suite.py
```

### Comparing `iaccess-0.5.0/CONTRIBUTING.rst` & `iaccess-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/HISTORY.rst` & `iaccess-0.6.0/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/LICENSE` & `iaccess-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/PKG-INFO` & `iaccess-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaccess
-Version: 0.5.0
+Version: 0.6.0
 Summary: Provides support for DB2 for iSeries for remote python clients using IBM i Access Client Solutions ODBC driver
 Home-page: https://github.com/soundstripe/iaccess
 Author: Steven Clayton James
 Author-email: steven@waitforitjames.com
 License: MIT license
 Keywords: iaccess
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iaccess-0.5.0/README.rst` & `iaccess-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/docs/Makefile` & `iaccess-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/docs/conf.py` & `iaccess-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/docs/iaccess.rst` & `iaccess-0.6.0/docs/iaccess.rst`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/docs/installation.rst` & `iaccess-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/docs/make.bat` & `iaccess-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/docs/usage.rst` & `iaccess-0.6.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/iaccess/compiler.py` & `iaccess-0.6.0/iaccess/compiler.py`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/iaccess/connector.py` & `iaccess-0.6.0/iaccess/connector.py`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/iaccess/dialect.py` & `iaccess-0.6.0/iaccess/dialect.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
         whereclause = sql.and_(
             tables.c.table_name == table_name,
             tables.c.table_type == 'T',
             tables.c.table_schema == sql.func.coalesce(schema, sql.literal_column('CURRENT_SCHEMA'))
         )
 
-        s = sql.select([tables], whereclause)
+        s = sql.select(tables).where(whereclause)
         c = connection.execute(s)
         return c.first() is not None
 
     def _get_default_schema_name(self, connection):
         query = sql.text("select CURRENT_SCHEMA from sysibm.sysdummy1")
         default_schema_name = connection.scalar(query)
         if default_schema_name is not None:
@@ -141,15 +141,16 @@
             return self.schema_name
 
     @reflection.cache
     def get_table_names(self, connection, schema=None, **kw):
         tables = ischema.tables
         schema = self.denormalize_name(schema or self.default_schema_name)
         s = sql.select(
-            [tables.c.table_name],
+            tables.c.table_name
+        ).where(
             sql.and_(
                 tables.c.table_schema == schema,
                 tables.c.table_type == 'T',
             ),
             order_by=[tables.c.table_name],
         )
         table_names = [self.normalize_name(r.table_name) for r in connection.execute(s)]
@@ -199,15 +200,15 @@
         return results
 
     @reflection.cache
     def get_columns(self, connection, table_name, schema=None, **kw):
         current_schema = self.denormalize_name(schema or self.default_schema_name)
         table_name = self.denormalize_name(table_name)
         columns = ischema.columns
-        s = sql.select([
+        s = sql.select(
             columns.c.column_name,
             columns.c.data_type,
             columns.c.length,
             columns.c.numeric_precision,
             columns.c.numeric_scale,
             columns.c.is_nullable,
             columns.c.column_default,
@@ -216,15 +217,15 @@
             columns.c.identity_start,
             columns.c.identity_increment,
             columns.c.identity_minimum,
             columns.c.identity_maximum,
             columns.c.identity_cycle,
             columns.c.identity_cache,
             columns.c.identity_order,
-        ], sql.and_(
+        ).where(sql.and_(
             columns.c.table_name == table_name,
             columns.c.table_schema == current_schema,
         ))
         r = connection.execute(s)
 
         results = []
         for col in r:
@@ -273,19 +274,19 @@
     @reflection.cache
     def get_indexes(self, connection, table_name, schema=None, **kw):
         table_name = self.denormalize_name(table_name)
         schema = self.denormalize_name(schema or self.default_schema_name)
         indexes = ischema.indexes
         keys = ischema.keys
         j = indexes.join(keys, indexes.c.index_name == keys.c.index_name)
-        s = sql.select([
+        s = sql.select(
             indexes.c.index_name,
             indexes.c.is_unique,
             keys.c.column_name,
-        ], and_(
+        ).where(and_(
             indexes.c.table_schema == schema,
             indexes.c.table_name == table_name,
         )).select_from(j).order_by(indexes.c.index_name, keys.c.ordinal_position)
         r = connection.execute(s)
         grouped = groupby(r, lambda x: (x.index_name, x.is_unique in 'VU'))
         results = [dict(name=self.normalize_name(index_name),
                         column_names=[self.normalize_name(c.column_name) for c in columns],
@@ -300,18 +301,18 @@
         constraints = ischema.constraints
         constraint_columns = ischema.constraint_columns
         j = constraints.join(constraint_columns, and_(
             constraints.c.table_schema == constraint_columns.c.table_schema,
             constraints.c.table_name == constraint_columns.c.table_name,
             constraints.c.constraint_name == constraint_columns.c.constraint_name,
         ))
-        s = sql.select([
+        s = sql.select(
             constraint_columns.c.constraint_name,
             constraint_columns.c.column_name,
-        ], and_(
+        ).where(and_(
             constraints.c.constraint_type == 'PRIMARY KEY',
             constraints.c.table_name == table_name,
             constraints.c.table_schema == schema,
         )).select_from(j)
         r = connection.execute(s)
         grouped = groupby(r, lambda x: self.normalize_name(x.constraint_name))
         results = [{
@@ -329,18 +330,18 @@
         constraints = ischema.constraints
         constraint_columns = ischema.constraint_columns
         j = constraints.join(constraint_columns, and_(
             constraints.c.table_schema == constraint_columns.c.table_schema,
             constraints.c.table_name == constraint_columns.c.table_name,
             constraints.c.constraint_name == constraint_columns.c.constraint_name,
         ))
-        s = sql.select([
+        s = sql.select(
             constraint_columns.c.constraint_name,
             constraint_columns.c.column_name,
-        ], and_(
+        ).where(and_(
             constraints.c.constraint_type == 'UNIQUE',
             constraints.c.table_name == table_name,
             constraints.c.table_schema == schema,
         )).select_from(j)
         r = connection.execute(s)
         grouped = groupby(r, lambda x: self.normalize_name(x.constraint_name))
         results = [{
@@ -349,16 +350,15 @@
         } for (cst_name, columns) in grouped]
         return results
 
     def has_sequence(self, connection, sequence_name, schema=None):
         schema = self.denormalize_name(schema or self.default_schema_name)
         sequence_name = self.denormalize_name(sequence_name)
         sequences = ischema.sequences
-        s = sql.select(
-            [sequences.c.sequence_name],
+        s = sql.select(sequences.c.sequence_name).where(
             and_(
                 sequences.c.sequence_name == sequence_name,
                 sequences.c.sequence_schema == schema,
             ))
         r = connection.execute(s)
         return r.first() is not None
```

### Comparing `iaccess-0.5.0/iaccess/information_schema/iseries.py` & `iaccess-0.6.0/iaccess/information_schema/iseries.py`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/iaccess/requirements.py` & `iaccess-0.6.0/iaccess/requirements.py`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/iaccess.egg-info/PKG-INFO` & `iaccess-0.6.0/iaccess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iaccess
-Version: 0.5.0
+Version: 0.6.0
 Summary: Provides support for DB2 for iSeries for remote python clients using IBM i Access Client Solutions ODBC driver
 Home-page: https://github.com/soundstripe/iaccess
 Author: Steven Clayton James
 Author-email: steven@waitforitjames.com
 License: MIT license
 Keywords: iaccess
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iaccess-0.5.0/iaccess.egg-info/SOURCES.txt` & `iaccess-0.6.0/iaccess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/setup.py` & `iaccess-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `iaccess-0.5.0/tests/test_suite.py` & `iaccess-0.6.0/tests/test_suite.py`

 * *Files identical despite different names*

