# Comparing `tmp/dmk_packages-0.4.2.tar.gz` & `tmp/dmk_packages-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmk_packages-0.4.2.tar", last modified: Tue Mar 26 15:03:32 2024, max compression
+gzip compressed data, was "dmk_packages-0.5.0.tar", last modified: Thu Apr  4 02:58:35 2024, max compression
```

## Comparing `dmk_packages-0.4.2.tar` & `dmk_packages-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-03-26 15:03:32.977666 dmk_packages-0.4.2/
--rw-r--r--   0 vincent    (501) staff       (20)    11347 2024-02-13 02:46:15.000000 dmk_packages-0.4.2/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)     1854 2024-03-26 15:03:32.977347 dmk_packages-0.4.2/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)     1365 2024-02-13 08:52:43.000000 dmk_packages-0.4.2/README.md
--rw-r--r--   0 vincent    (501) staff       (20)      584 2024-03-26 15:03:16.000000 dmk_packages-0.4.2/pyproject.toml
--rw-r--r--   0 vincent    (501) staff       (20)       38 2024-03-26 15:03:32.977734 dmk_packages-0.4.2/setup.cfg
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-03-26 15:03:32.972611 dmk_packages-0.4.2/src/
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-03-26 15:03:32.974138 dmk_packages-0.4.2/src/dmk_packages/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2024-02-13 02:46:15.000000 dmk_packages-0.4.2/src/dmk_packages/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-03-26 15:03:32.975922 dmk_packages-0.4.2/src/dmk_packages/crawler/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2024-03-19 09:21:56.000000 dmk_packages-0.4.2/src/dmk_packages/crawler/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     2321 2024-03-26 12:16:25.000000 dmk_packages-0.4.2/src/dmk_packages/crawler/naver_blog.py
--rw-r--r--   0 vincent    (501) staff       (20)    15349 2024-03-20 08:21:00.000000 dmk_packages-0.4.2/src/dmk_packages/crawler/naver_search_volume.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-03-26 15:03:32.976643 dmk_packages-0.4.2/src/dmk_packages/database/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2024-03-20 08:20:26.000000 dmk_packages-0.4.2/src/dmk_packages/database/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3054 2024-03-26 15:03:11.000000 dmk_packages-0.4.2/src/dmk_packages/database/database.py
--rw-r--r--   0 vincent    (501) staff       (20)     1895 2024-02-29 02:00:03.000000 dmk_packages-0.4.2/src/dmk_packages/naver_datalab.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-03-26 15:03:32.977058 dmk_packages-0.4.2/src/dmk_packages.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)     1854 2024-03-26 15:03:32.000000 dmk_packages-0.4.2/src/dmk_packages.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      494 2024-03-26 15:03:32.000000 dmk_packages-0.4.2/src/dmk_packages.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2024-03-26 15:03:32.000000 dmk_packages-0.4.2/src/dmk_packages.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       41 2024-03-26 15:03:32.000000 dmk_packages-0.4.2/src/dmk_packages.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       13 2024-03-26 15:03:32.000000 dmk_packages-0.4.2/src/dmk_packages.egg-info/top_level.txt
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.611972 dmk_packages-0.5.0/
+-rw-r--r--   0 layla      (501) staff       (20)    11347 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/LICENSE
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-04 02:58:35.611608 dmk_packages-0.5.0/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)     1365 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/README.md
+-rw-r--r--   0 layla      (501) staff       (20)      584 2024-04-04 02:20:18.000000 dmk_packages-0.5.0/pyproject.toml
+-rw-r--r--   0 layla      (501) staff       (20)       38 2024-04-04 02:58:35.612067 dmk_packages-0.5.0/setup.cfg
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.599755 dmk_packages-0.5.0/src/
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.603373 dmk_packages-0.5.0/src/dmk_packages/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/src/dmk_packages/__init__.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.609429 dmk_packages-0.5.0/src/dmk_packages/crawler/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     2321 2024-04-03 06:07:52.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/naver_blog.py
+-rw-r--r--   0 layla      (501) staff       (20)    15349 2024-04-01 06:49:53.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/naver_search_volume.py
+-rw-r--r--   0 layla      (501) staff       (20)    12855 2024-04-04 02:18:34.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/youtube.py
+-rw-r--r--   0 layla      (501) staff       (20)     2258 2024-04-04 01:44:42.000000 dmk_packages-0.5.0/src/dmk_packages/crawler/youtube_test.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.610452 dmk_packages-0.5.0/src/dmk_packages/database/
+-rw-r--r--   0 layla      (501) staff       (20)        0 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/src/dmk_packages/database/__init__.py
+-rw-r--r--   0 layla      (501) staff       (20)     3057 2024-04-03 06:07:52.000000 dmk_packages-0.5.0/src/dmk_packages/database/database.py
+-rw-r--r--   0 layla      (501) staff       (20)     1895 2024-03-25 06:00:17.000000 dmk_packages-0.5.0/src/dmk_packages/naver_datalab.py
+drwxr-xr-x   0 layla      (501) staff       (20)        0 2024-04-04 02:58:35.611084 dmk_packages-0.5.0/src/dmk_packages.egg-info/
+-rw-r--r--   0 layla      (501) staff       (20)     1854 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/PKG-INFO
+-rw-r--r--   0 layla      (501) staff       (20)      571 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 layla      (501) staff       (20)        1 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 layla      (501) staff       (20)       41 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/requires.txt
+-rw-r--r--   0 layla      (501) staff       (20)       13 2024-04-04 02:58:35.000000 dmk_packages-0.5.0/src/dmk_packages.egg-info/top_level.txt
```

### Comparing `dmk_packages-0.4.2/LICENSE` & `dmk_packages-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.4.2/PKG-INFO` & `dmk_packages-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.4.2
+Version: 0.5.0
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `dmk_packages-0.4.2/README.md` & `dmk_packages-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.4.2/pyproject.toml` & `dmk_packages-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmk_packages"
-version = "0.4.2"
+version = "0.5.0"
 authors = [{ name = "DataMarketingKorea", email = "infra@datamarketing.co.kr" }]
 description = "Common packages for DataMKTKorea"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["SQLAlchemy", "python-dotenv", "psycopg2-binary"]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `dmk_packages-0.4.2/src/dmk_packages/crawler/naver_blog.py` & `dmk_packages-0.5.0/src/dmk_packages/crawler/naver_blog.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.4.2/src/dmk_packages/crawler/naver_search_volume.py` & `dmk_packages-0.5.0/src/dmk_packages/crawler/naver_search_volume.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.4.2/src/dmk_packages/database/database.py` & `dmk_packages-0.5.0/src/dmk_packages/database/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,56 +55,59 @@
     except Exception as error:
         logger.error(error)
 
 
 def create_to_postgres(
     engine: Engine, name: str, *columns: Tuple[Column[Any]], metadata=MetaData()
 ):
+    """
+    예시 코드:
+
+    create_to_postgres(
+        get_engine("TARGET_DB"),
+        "users",
+        Column("id", Integer, primary_key=True),
+        Column("name", String),
+        Column("age", Integer),
+        Column("contact", String),
+        UniqueConstraint("name", "contact"),
+    )
+    """
+
     try:
         new_table = Table(name, metadata, *columns)
         new_table.create(engine, checkfirst=True)
     except Exception as error:
         logger.error(error)
 
 
 def insert_to_postgres(
     engine: Engine,
     name: str,
     values: List[dict],
     metadata=MetaData(),
     index_elements=None,
 ):
+    """
+    예시 코드:
+
+    users = [
+        {"name": "허해준", "age": "29", "contact": "01012345678"},
+        {"name": "권재선", "age": "30", "contact": "01087654321"},
+    ]
+    insert_to_postgres(get_engine("TARGET_DB"), "users", users, index_elements=["name", "contact"])
+    """
+
     try:
         metadata.bind = engine
         table = Table(name, metadata, autoload_with=engine)
 
         stmt = (
             insert(table)
             .values(values)
             .on_conflict_do_nothing(index_elements=index_elements)
         )
 
         with engine.begin() as connection:
             connection.execute(stmt)
     except Exception as error:
         logger.error(error)
-
-
-# if __name__ == "__main__":
-#     create_to_postgres(
-#         get_engine("TEST"),
-#         "users",
-#         Column("id", Integer, primary_key=True),
-#         Column("name", String),
-#         Column("age", Integer),
-#         Column("contact", String),
-#         UniqueConstraint("name", "contact"),
-#     )
-
-#     people = [
-#         {"name": "파이썬", "age": "29", "contact": "01012345678"},
-#         {"name": "오라클", "age": "30", "contact": "01087654321"},
-#     ]
-
-#     insert_to_postgres(
-#         get_engine("TEST"), "users", people, index_elements=["name", "contact"]
-#     )
```

### Comparing `dmk_packages-0.4.2/src/dmk_packages/naver_datalab.py` & `dmk_packages-0.5.0/src/dmk_packages/naver_datalab.py`

 * *Files identical despite different names*

### Comparing `dmk_packages-0.4.2/src/dmk_packages.egg-info/PKG-INFO` & `dmk_packages-0.5.0/src/dmk_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmk_packages
-Version: 0.4.2
+Version: 0.5.0
 Summary: Common packages for DataMKTKorea
 Author-email: DataMarketingKorea <infra@datamarketing.co.kr>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

