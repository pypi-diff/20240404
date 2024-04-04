# Comparing `tmp/weave-db-1.7.1.tar.gz` & `tmp/weave-db-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weave-db-1.7.1.tar", last modified: Tue Mar 26 20:15:20 2024, max compression
+gzip compressed data, was "weave-db-1.7.2.tar", last modified: Thu Apr  4 13:55:10 2024, max compression
```

## Comparing `weave-db-1.7.1.tar` & `weave-db-1.7.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:15:20.352975 weave-db-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-03-26 20:15:20.352975 weave-db-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-03-26 20:15:16.000000 weave-db-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 20:15:20.352975 weave-db-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-26 20:15:16.000000 weave-db-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:15:20.348975 weave-db-1.7.1/weave/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/basket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:15:20.348975 weave-db-1.7.1/weave/index/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/index/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/index/index_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/index/index_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    31379 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/index/index_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/index/index_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/index/list_baskets.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/index/validate_basket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/metadata_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/mongo_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/pantry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:15:20.352975 weave-db-1.7.1/weave/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/pytest_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    26482 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_basket.py
--rw-r--r--   0 runner    (1001) docker     (127)    65508 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_index_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_index_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_index_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_mongo_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_pantry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)    44925 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    61528 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19221 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-03-26 20:15:16.000000 weave-db-1.7.1/weave/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 20:15:20.352975 weave-db-1.7.1/weave_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-03-26 20:15:20.000000 weave-db-1.7.1/weave_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-26 20:15:20.000000 weave-db-1.7.1/weave_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 20:15:20.000000 weave-db-1.7.1/weave_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-26 20:15:20.000000 weave-db-1.7.1/weave_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-26 20:15:20.000000 weave-db-1.7.1/weave_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.350135 weave-db-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-04 13:55:10.350135 weave-db-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-04 13:55:06.000000 weave-db-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:55:10.350135 weave-db-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-04 13:55:06.000000 weave-db-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.346135 weave-db-1.7.2/weave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/basket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.346135 weave-db-1.7.2/weave/index/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/index_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/index_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31379 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/index_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/index_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/list_baskets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/validate_basket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/metadata_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/mongo_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/pantry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.346135 weave-db-1.7.2/weave/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/pytest_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26482 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_basket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65508 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_index_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_index_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_index_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_mongo_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_pantry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44925 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61528 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19221 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.350135 weave-db-1.7.2/weave_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/top_level.txt
```

### Comparing `weave-db-1.7.1/PKG-INFO` & `weave-db-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-db
-Version: 1.7.1
+Version: 1.7.2
 Summary: Library to facilitate the creation and maintenance of complex data warehouses.
 Home-page: https://github.com/309thEDDGE/weave
 Author: 309thEDDGE
 License: GNU General Public
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `weave-db-1.7.1/README.md` & `weave-db-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/setup.py` & `weave-db-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/__init__.py` & `weave-db-1.7.2/weave/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .index.index_pandas import IndexPandas
 from .index.index_sqlite import IndexSQLite
 from .index.index_sql import IndexSQL
 from .pantry import Pantry
 from .metadata_db import load_mongo
 from .mongo_db import MongoDB
 
-__version__ = "1.7.1"
+__version__ = "1.7.2"
 
 __all__ = [
     "Basket",
     "IndexPandas",
     "IndexSQLite",
     "IndexSQL",
     "Pantry",
```

### Comparing `weave-db-1.7.1/weave/basket.py` & `weave-db-1.7.2/weave/basket.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/config.py` & `weave-db-1.7.2/weave/config.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/index/create_index.py` & `weave-db-1.7.2/weave/index/create_index.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/index/index_abc.py` & `weave-db-1.7.2/weave/index/index_abc.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/index/index_pandas.py` & `weave-db-1.7.2/weave/index/index_pandas.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/index/index_sql.py` & `weave-db-1.7.2/weave/index/index_sql.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/index/index_sqlite.py` & `weave-db-1.7.2/weave/index/index_sqlite.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/index/validate_basket.py` & `weave-db-1.7.2/weave/index/validate_basket.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/metadata_db.py` & `weave-db-1.7.2/weave/metadata_db.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/mongo_db.py` & `weave-db-1.7.2/weave/mongo_db.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/pantry.py` & `weave-db-1.7.2/weave/pantry.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/pytest_resources.py` & `weave-db-1.7.2/weave/tests/pytest_resources.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_basket.py` & `weave-db-1.7.2/weave/tests/test_basket.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_index.py` & `weave-db-1.7.2/weave/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_index_pandas.py` & `weave-db-1.7.2/weave/tests/test_index_pandas.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_index_sql.py` & `weave-db-1.7.2/weave/tests/test_index_sql.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_index_sqlite.py` & `weave-db-1.7.2/weave/tests/test_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_mongo_db.py` & `weave-db-1.7.2/weave/tests/test_mongo_db.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_pantry.py` & `weave-db-1.7.2/weave/tests/test_pantry.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_pytest.py` & `weave-db-1.7.2/weave/tests/test_pytest.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,20 @@
         user= os.environ["WEAVE_SQL_USERNAME"],
         password= os.environ["WEAVE_SQL_PASSWORD"],
         port= os.environ.get("WEAVE_SQL_PORT", 5432),
         )
     cur = conn.cursor()
 
     # Create a temporary table for testing.
-    cur.execute("CREATE SCHEMA dbo;")
+    cur.execute("""
+        SELECT schema_name FROM information_schema.schemata
+        WHERE schema_name = 'dbo';
+    """)
+    if cur.fetchall() == []:
+        cur.execute("CREATE SCHEMA dbo;")
     cur.execute("""
     CREATE TABLE IF NOT EXISTS dbo.test_table (
         uuid varchar(64),
         num int
     );
     """)
     conn.commit()
```

### Comparing `weave-db-1.7.1/weave/tests/test_uploader.py` & `weave-db-1.7.2/weave/tests/test_uploader.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/tests/test_validate.py` & `weave-db-1.7.2/weave/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/upload.py` & `weave-db-1.7.2/weave/upload.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave/validate.py` & `weave-db-1.7.2/weave/validate.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.1/weave_db.egg-info/PKG-INFO` & `weave-db-1.7.2/weave_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-db
-Version: 1.7.1
+Version: 1.7.2
 Summary: Library to facilitate the creation and maintenance of complex data warehouses.
 Home-page: https://github.com/309thEDDGE/weave
 Author: 309thEDDGE
 License: GNU General Public
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `weave-db-1.7.1/weave_db.egg-info/SOURCES.txt` & `weave-db-1.7.2/weave_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

