# Comparing `tmp/sqlx-orm-0.0.1.tar.gz` & `tmp/sqlx-orm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlx-orm-0.0.1.tar", last modified: Thu Apr  4 10:07:39 2024, max compression
+gzip compressed data, was "sqlx-orm-0.0.2.tar", last modified: Thu Apr  4 10:08:35 2024, max compression
```

## Comparing `sqlx-orm-0.0.1.tar` & `sqlx-orm-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:07:39.316251 sqlx-orm-0.0.1/
--rw-r--r--   0 summy      (501) staff       (20)     2170 2024-04-04 10:07:39.314035 sqlx-orm-0.0.1/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)     1758 2024-04-04 09:58:39.000000 sqlx-orm-0.0.1/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:07:39.302667 sqlx-orm-0.0.1/orm/
--rw-r--r--   0 summy      (501) staff       (20)      288 2024-04-04 08:43:34.000000 sqlx-orm-0.0.1/orm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)      867 2024-04-04 01:04:08.000000 sqlx-orm-0.0.1/orm/constant.py
--rw-r--r--   0 summy      (501) staff       (20)     3657 2024-04-04 01:03:37.000000 sqlx-orm-0.0.1/orm/log_support.py
--rw-r--r--   0 summy      (501) staff       (20)    29103 2024-04-04 01:10:00.000000 sqlx-orm-0.0.1/orm/orm.py
--rw-r--r--   0 summy      (501) staff       (20)    12126 2024-04-04 01:02:32.000000 sqlx-orm-0.0.1/orm/orm_support.py
--rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlx-orm-0.0.1/orm/snowflake.py
--rw-r--r--   0 summy      (501) staff       (20)      991 2024-04-04 01:12:05.000000 sqlx-orm-0.0.1/orm/sql_support.py
--rw-r--r--   0 summy      (501) staff       (20)      128 2024-04-04 01:12:05.000000 sqlx-orm-0.0.1/orm/support.py
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-04 10:07:39.316531 sqlx-orm-0.0.1/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1206 2024-04-04 10:07:36.000000 sqlx-orm-0.0.1/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:07:39.311849 sqlx-orm-0.0.1/sqlx_orm.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     2170 2024-04-04 10:07:39.000000 sqlx-orm-0.0.1/sqlx_orm.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      341 2024-04-04 10:07:39.000000 sqlx-orm-0.0.1/sqlx_orm.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:07:39.000000 sqlx-orm-0.0.1/sqlx_orm.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:07:39.000000 sqlx-orm-0.0.1/sqlx_orm.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       17 2024-04-04 10:07:39.000000 sqlx-orm-0.0.1/sqlx_orm.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)        4 2024-04-04 10:07:39.000000 sqlx-orm-0.0.1/sqlx_orm.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:08:35.456204 sqlx-orm-0.0.2/
+-rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-04 10:08:35.455385 sqlx-orm-0.0.2/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)     1733 2024-04-04 10:08:32.000000 sqlx-orm-0.0.2/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:08:35.448193 sqlx-orm-0.0.2/orm/
+-rw-r--r--   0 summy      (501) staff       (20)      288 2024-04-04 08:43:34.000000 sqlx-orm-0.0.2/orm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)      867 2024-04-04 01:04:08.000000 sqlx-orm-0.0.2/orm/constant.py
+-rw-r--r--   0 summy      (501) staff       (20)     3657 2024-04-04 01:03:37.000000 sqlx-orm-0.0.2/orm/log_support.py
+-rw-r--r--   0 summy      (501) staff       (20)    29103 2024-04-04 01:10:00.000000 sqlx-orm-0.0.2/orm/orm.py
+-rw-r--r--   0 summy      (501) staff       (20)    12126 2024-04-04 01:02:32.000000 sqlx-orm-0.0.2/orm/orm_support.py
+-rw-r--r--   0 summy      (501) staff       (20)     2603 2024-04-04 01:12:05.000000 sqlx-orm-0.0.2/orm/snowflake.py
+-rw-r--r--   0 summy      (501) staff       (20)      991 2024-04-04 01:12:05.000000 sqlx-orm-0.0.2/orm/sql_support.py
+-rw-r--r--   0 summy      (501) staff       (20)      128 2024-04-04 01:12:05.000000 sqlx-orm-0.0.2/orm/support.py
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-04-04 10:08:35.456496 sqlx-orm-0.0.2/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1206 2024-04-04 10:08:32.000000 sqlx-orm-0.0.2/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-04-04 10:08:35.454157 sqlx-orm-0.0.2/sqlx_orm.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     2145 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      341 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-04-04 10:07:39.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       17 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)        4 2024-04-04 10:08:35.000000 sqlx-orm-0.0.2/sqlx_orm.egg-info/top_level.txt
```

### Comparing `sqlx-orm-0.0.1/PKG-INFO` & `sqlx-orm-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: sqlx-orm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlx-orm
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
-Mapper file
-'''''''''''
-
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
     from orm import Model, db
     from typing import List, Tuple, Mapping
```

### Comparing `sqlx-orm-0.0.1/README.rst` & `sqlx-orm-0.0.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-Mapper file
-'''''''''''
-
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
     from orm import Model, db
     from typing import List, Tuple, Mapping
```

### Comparing `sqlx-orm-0.0.1/orm/constant.py` & `sqlx-orm-0.0.2/orm/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.1/orm/log_support.py` & `sqlx-orm-0.0.2/orm/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.1/orm/orm.py` & `sqlx-orm-0.0.2/orm/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.1/orm/orm_support.py` & `sqlx-orm-0.0.2/orm/orm_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.1/orm/snowflake.py` & `sqlx-orm-0.0.2/orm/snowflake.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.1/orm/sql_support.py` & `sqlx-orm-0.0.2/orm/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-orm-0.0.1/setup.py` & `sqlx-orm-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-orm',
     packages=['orm'],
     description="A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.0.1',
+    version='0.0.2',
     install_requires=[
         'sqlx-exec>=2.3.3',
     ],
     url='https://gitee.com/summry/sqlx-orm',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python', 'RDB'],
```

### Comparing `sqlx-orm-0.0.1/sqlx_orm.egg-info/PKG-INFO` & `sqlx-orm-0.0.2/sqlx_orm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 Metadata-Version: 2.1
 Name: sqlx-orm
-Version: 0.0.1
+Version: 0.0.2
 Summary: A single table ORM framework for python. Support MySQL, PostgreSQL, SQLite etc.
 Home-page: https://gitee.com/summry/sqlx-orm
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python,RDB
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 
-Mapper file
-'''''''''''
-
 Usage Sample
 ''''''''''''
 
 .. code:: python
 
     from orm import Model, db
     from typing import List, Tuple, Mapping
```

