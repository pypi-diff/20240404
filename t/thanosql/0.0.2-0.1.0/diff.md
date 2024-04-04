# Comparing `tmp/thanosql-0.0.2.tar.gz` & `tmp/thanosql-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thanosql-0.0.2.tar", last modified: Wed Mar 27 00:09:06 2024, max compression
+gzip compressed data, was "thanosql-0.1.0.tar", last modified: Thu Apr  4 10:08:12 2024, max compression
```

## Comparing `thanosql-0.0.2.tar` & `thanosql-0.1.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:09:06.089758 thanosql-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-27 00:09:01.000000 thanosql-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-03-27 00:09:06.089758 thanosql-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-03-27 00:09:01.000000 thanosql-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 00:09:01.000000 thanosql-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 00:09:06.089758 thanosql-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-27 00:09:01.000000 thanosql-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:09:06.085758 thanosql-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-27 00:09:01.000000 thanosql-0.0.2/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-03-27 00:09:01.000000 thanosql-0.0.2/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-27 00:09:01.000000 thanosql-0.0.2/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9811 2024-03-27 00:09:01.000000 thanosql-0.0.2/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-03-27 00:09:01.000000 thanosql-0.0.2/tests/test_table_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-27 00:09:01.000000 thanosql-0.0.2/tests/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:09:06.085758 thanosql-0.0.2/thanosql/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/_service.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:09:06.089758 thanosql-0.0.2/thanosql/magic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/magic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/magic/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/magic/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/magic/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/magic/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:09:06.089758 thanosql-0.0.2/thanosql/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/resources/_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/resources/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/resources/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/resources/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-27 00:09:01.000000 thanosql-0.0.2/thanosql/resources/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:09:06.089758 thanosql-0.0.2/thanosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-03-27 00:09:06.000000 thanosql-0.0.2/thanosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-27 00:09:06.000000 thanosql-0.0.2/thanosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 00:09:06.000000 thanosql-0.0.2/thanosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 00:09:05.000000 thanosql-0.0.2/thanosql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-27 00:09:06.000000 thanosql-0.0.2/thanosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 00:09:06.000000 thanosql-0.0.2/thanosql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.623872 thanosql-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 10:08:08.000000 thanosql-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-04 10:08:12.623872 thanosql-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-04 10:08:08.000000 thanosql-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:08.000000 thanosql-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:08:12.623872 thanosql-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-04 10:08:08.000000 thanosql-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.615872 thanosql-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9839 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_table_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-04 10:08:08.000000 thanosql-0.1.0/tests/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.619872 thanosql-0.1.0/thanosql/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.619872 thanosql-0.1.0/thanosql/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/magic/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.619872 thanosql-0.1.0/thanosql/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-04 10:08:08.000000 thanosql-0.1.0/thanosql/resources/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:08:12.619872 thanosql-0.1.0/thanosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 10:08:12.000000 thanosql-0.1.0/thanosql.egg-info/top_level.txt
```

### Comparing `thanosql-0.0.2/LICENSE` & `thanosql-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/PKG-INFO` & `thanosql-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thanosql
-Version: 0.0.2
+Version: 0.1.0
 Summary: ThanoSQL SDK for Python
 Home-page: https://github.com/smartmind-team/thanosql-python
 Author: SmartMind
 Author-email: dev@smartmind.team
 License: MIT
 Keywords: smartmind thanosql sdk
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,17 @@
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: pydantic>=2.0
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: faker; extra == "dev"
+Requires-Dist: myst-nb; extra == "dev"
+Requires-Dist: sphinx-autoapi; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Provides-Extra: magic
 Requires-Dist: ipython; extra == "magic"
 Requires-Dist: pandas; extra == "magic"
 Requires-Dist: sqlalchemy; extra == "magic"
 Requires-Dist: numpy; extra == "magic"
 Requires-Dist: matplotlib; extra == "magic"
 Requires-Dist: websocket-client; extra == "magic"
@@ -51,29 +54,30 @@
 >
 > `pip install 'thanosql[magic]'`
 
 Alternatively, you can also install from source. First, clone this repository.
 
 ```bash
 git clone https://github.com/smartmind-team/thanosql-sdk-python.git
+cd thanosql-sdk-python
 ```
 
 Install the SDK by using `pip install`. Note that the Python version used during development is 3.8.10.
 
 ```bash
 pip install -e .
-pip install -e ."[dev]" # include unit test
+pip install -e ."[dev]" # include unit test & docs (requires python >= 3.9)
 pip install -e ."[magic]" # include magic
 ```
 
 ## Usage
 
-In order to use the library, a working workspace engine is required. Create a new Python or IPython notebook file. Import the `thanosql` package, create a `ThanoSQL` client with your API token and engine URL, and then you can use all the functions in the library. For more examples, head over to the [examples/](./examples/) directory.
+In order to use the library, a working workspace engine is required. Create a new Python or IPython notebook file. Import the `thanosql` package, create a `ThanoSQL` client with your API token and engine URL, and then you can use all the functions in the library. For more examples, head over to the [examples](./docs/examples/) directory.
 
-1. Set up your API_TOKEN and ENGINE_URL (recommended).
+1. First, set up your API_TOKEN and ENGINE_URL (recommended). You can find them by accessing your workspace's settings page. Head over to the `Developer` tab, and then copy your API Token and Engine URL.
 
    ```bash
    export THANOSQL_API_TOKEN='your-api-token-here'
    export THANOSQL_ENGINE_URL='your-engine-url-here'
    ```
 
 2. Import the ThanoSQL client and use it to query your ThanoSQL Workspace.
```

### Comparing `thanosql-0.0.2/README.md` & `thanosql-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,29 +19,30 @@
 >
 > `pip install 'thanosql[magic]'`
 
 Alternatively, you can also install from source. First, clone this repository.
 
 ```bash
 git clone https://github.com/smartmind-team/thanosql-sdk-python.git
+cd thanosql-sdk-python
 ```
 
 Install the SDK by using `pip install`. Note that the Python version used during development is 3.8.10.
 
 ```bash
 pip install -e .
-pip install -e ."[dev]" # include unit test
+pip install -e ."[dev]" # include unit test & docs (requires python >= 3.9)
 pip install -e ."[magic]" # include magic
 ```
 
 ## Usage
 
-In order to use the library, a working workspace engine is required. Create a new Python or IPython notebook file. Import the `thanosql` package, create a `ThanoSQL` client with your API token and engine URL, and then you can use all the functions in the library. For more examples, head over to the [examples/](./examples/) directory.
+In order to use the library, a working workspace engine is required. Create a new Python or IPython notebook file. Import the `thanosql` package, create a `ThanoSQL` client with your API token and engine URL, and then you can use all the functions in the library. For more examples, head over to the [examples](./docs/examples/) directory.
 
-1. Set up your API_TOKEN and ENGINE_URL (recommended).
+1. First, set up your API_TOKEN and ENGINE_URL (recommended). You can find them by accessing your workspace's settings page. Head over to the `Developer` tab, and then copy your API Token and Engine URL.
 
    ```bash
    export THANOSQL_API_TOKEN='your-api-token-here'
    export THANOSQL_ENGINE_URL='your-engine-url-here'
    ```
 
 2. Import the ThanoSQL client and use it to query your ThanoSQL Workspace.
```

### Comparing `thanosql-0.0.2/setup.py` & `thanosql-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     keywords="smartmind thanosql sdk",
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=["requests", "urllib3", "pydantic>=2.0", "tqdm"],
     extras_require={
         "dev": [
             "pytest",
             "faker",
+            "myst-nb",
+            "sphinx-autoapi",
+            "sphinx-rtd-theme"
         ],
         "magic": [
             "ipython",
             "pandas",
             "sqlalchemy",
             "numpy",
             "matplotlib",
```

### Comparing `thanosql-0.0.2/tests/test_file.py` & `thanosql-0.1.0/tests/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,52 +13,50 @@
 column_name = "name"
 int_column_name = "price"
 # ideally we should delete this dir after testing
 # but as there is no API for that, it is somewhat difficult and risky
 # so for now we will have a dedicated, fixed folder name for all tests
 dir_name = "test"
 file_name = "file_image.jpeg"
-default_file_path = f"drive/image/{file_name}"
+default_file_path = f"drive/{file_name}"
 
 
 def test_upload_file(client: ThanoSQL, basic_table_name: str):
-    # nonexistent dir
+    # dir not subpath of drive/
     with pytest.raises(ThanoSQLValueError):
-        client.file.upload(path=file_name, dir=dir_name)
-
-    dir = f"drive/{dir_name}"
+        client.file.upload(path=file_name, dir="..")
 
     # nonexistent table
     with pytest.raises(ThanoSQLNotFoundError):
         client.file.upload(
             path=file_name,
             db_commit=True,
             table=fake.unique.pystr(8),
             column=column_name,
-            dir=dir,
+            dir=dir_name,
         )
 
     # nonexistent column
     with pytest.raises(ThanoSQLNotFoundError):
         client.file.upload(
             path=file_name,
             db_commit=True,
             table=basic_table_name,
             column=fake.unique.pystr(8),
-            dir=dir,
+            dir=dir_name,
         )
 
     # trying to insert text into integer column
     with pytest.raises(ThanoSQLValueError):
         client.file.upload(
             path=file_name,
             db_commit=True,
             table=basic_table_name,
             column=int_column_name,
-            dir=dir,
+            dir=dir_name,
         )
 
     # upload without db_commit and dir
     # note that we cannot check the existence of uploaded files as it requires user_data_root
     # which can technically be saved, but it increases complexity and safety risk
     res = client.file.upload(path=file_name)
     assert res["data"]["file_path"] == default_file_path
@@ -68,16 +66,17 @@
     record_count_before = target_table.get_records()["total"]
 
     res = client.file.upload(
         path=file_name,
         db_commit=True,
         table=basic_table_name,
         column=column_name,
-        dir=dir,
+        dir=dir_name,
     )
+    assert res["data"]["file_path"] == f"drive/{dir_name}/{file_name}"
     assert res["data"]["table_name"] == basic_table_name
     assert res["data"]["column_name"] == column_name
 
     record_count_after = target_table.get_records()["total"]
     assert record_count_after == record_count_before + 1
```

### Comparing `thanosql-0.0.2/tests/test_query.py` & `thanosql-0.1.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/tests/test_schema.py` & `thanosql-0.1.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/tests/test_table.py` & `thanosql-0.1.0/tests/test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
 
 
 def test_create_table_success(client: ThanoSQL, new_schema: str):
     # create a table in a non-"public" schema properly without fixture
     res = client.table.create(
         name=test_table_name_old, schema=new_schema, table=TableObject()
     )
-    assert {"message", "table_name"} == set(res.keys())
-    assert res["table_name"] == test_table_name_old
+    assert isinstance(res, Table)
+    assert res.name == test_table_name_old
 
     # check that the table is indeed created
     res = client.table.get(name=test_table_name_old, schema=new_schema)
     assert res.name == test_table_name_old
 
 
 def test_get_tables_default(client: ThanoSQL):
@@ -86,15 +86,15 @@
 
 
 def test_get_tables_with_options(client: ThanoSQL, new_schema: str):
     res = client.table.list(schema=new_schema, verbose=True)
     assert isinstance(res, list)
     # we only have one table in this schema
     assert len(res) == 1
-    assert isinstance(res[0], BaseTable)
+    assert isinstance(res[0], Table)
 
 
 def test_update_table(client: ThanoSQL, new_schema: str):
     table_object = BaseTable(
         name=test_table_name,
         schema="public",
         columns=[BaseColumn(type="integer", name="number")],
@@ -103,16 +103,16 @@
                 name=f"pk_{fake.unique.pystr(8)}", columns=["number"]
             )
         ),
     )
     res = client.table.update(
         name=test_table_name_old, schema=new_schema, table=table_object
     )
-    assert {"message", "table_name"} == set(res.keys())
-    assert res["table_name"] == test_table_name_old
+    assert isinstance(res, Table)
+    assert res.name == test_table_name_old
 
     # make sure the old table is no longer retrievable
     with pytest.raises(ThanoSQLNotFoundError):
         client.table.get(name=test_table_name_old, schema=new_schema)
 
     # check that the update is successful
     res = client.table.get(name=test_table_name, schema="public")
@@ -188,15 +188,18 @@
         )
         client.table.upload(
             name=fake.unique.pystr(10), file="file_csv.csv", table=table_object
         )
 
 
 def test_upload_table_csv(client: ThanoSQL, basic_table_name: str):
-    client.table.upload(name=basic_table_name, file="file_csv.csv", if_exists="replace")
+    res = client.table.upload(
+        name=basic_table_name, file="file_csv.csv", if_exists="replace"
+    )
+    assert isinstance(res, Table)
 
     # check that the table and records are indeed uploaded
     target_table = client.table.get(name=basic_table_name)
     assert len(target_table.columns) == 9
 
     # check get records with limit in the meantime
     limit = 5
@@ -210,20 +213,21 @@
         columns=[
             BaseColumn(type="varchar", name="title"),
             BaseColumn(type="double precision", name="price"),
             BaseColumn(type="varchar", name="star_rating"),
         ]
     )
 
-    client.table.upload(
+    res = client.table.upload(
         name=test_table_name_excel,
         file="file_excel.xlsx",
         schema=new_schema,
         table=table_object,
     )
+    assert isinstance(res, Table)
 
     # check that the table and records are indeed uploaded
     target_table = client.table.get(name=test_table_name_excel, schema=new_schema)
     assert len(target_table.columns) == 3
 
     # check get records with limit in the meantime
     limit = 5
```

### Comparing `thanosql-0.0.2/tests/test_table_template.py` & `thanosql-0.1.0/tests/test_table_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,16 @@
 ):
     # creating the same template with different (valid) version should work
     res = client.table.template.create(
         name=empty_table_template_name,
         table_template=TableObject(),
         version=latest_version,
     )
-    assert {"message", "table_template_name"} == set(res.keys())
+    assert isinstance(res, TableTemplate)
+    assert res.name == empty_table_template_name
 
 
 def test_get_table_template_not_found(client: ThanoSQL):
     # random name that is yet to be used for creation should not work
     with pytest.raises(ThanoSQLNotFoundError):
         client.table.template.get(name=fake.unique.pystr(8))
```

### Comparing `thanosql-0.0.2/tests/test_view.py` & `thanosql-0.1.0/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/thanosql/_base_client.py` & `thanosql-0.1.0/thanosql/_base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import requests
 from tqdm import tqdm
 
 import thanosql._error as thanosql_error
 
 
 class ThanoSQLBaseClient:
-    def __init__(self, base_url: str, version: str, token: str) -> None:
+    def __init__(self, token: str, base_url: str, version: str) -> None:
+        self.token: str = token
         self.base_url: str = base_url.strip("/")
         self.version: str = version
-        self.token: str = token
 
         self.url: str = f"{self.base_url}/api/{version}"
 
     def _create_auth_header(self) -> dict:
         return {"Authorization": f"Bearer {self.token}"}
 
     def _create_full_url(
@@ -59,15 +59,17 @@
         headers = self._create_auth_header()
         headers["accept"] = "application/json"
 
         payload_json = {}
 
         try:
             if file:
-                payload_json["files"] = {"file": (file, open(file, "rb"))}
+                payload_json["files"] = {
+                    "file": (os.path.basename(file), open(file, "rb"))
+                }
                 if payload:
                     payload_json["files"]["body"] = (
                         None,
                         json.dumps(payload),
                         "application/json",
                     )
```

### Comparing `thanosql-0.0.2/thanosql/_error.py` & `thanosql-0.1.0/thanosql/_error.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/thanosql/_service.py` & `thanosql-0.1.0/thanosql/_service.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/thanosql/magic/magic.py` & `thanosql-0.1.0/thanosql/magic/magic.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/thanosql/magic/parse.py` & `thanosql-0.1.0/thanosql/magic/parse.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/thanosql/magic/util.py` & `thanosql-0.1.0/thanosql/magic/util.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/thanosql/resources/_file.py` & `thanosql-0.1.0/thanosql/resources/_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class FileService(ThanoSQLService):
     def __init__(self, client: ThanoSQL) -> None:
         super().__init__(client=client, tag="file")
 
     def list(self, path: Union[str, os.PathLike]) -> dict:
         api_path = f"/{self.tag}/"
-        query_params = self._create_input_dict(file_path=path)
+        query_params = self._create_input_dict(search_path=path)
 
         return self.client._request(
             method="get", path=api_path, query_params=query_params
         )
 
     def upload(
         self,
```

### Comparing `thanosql-0.0.2/thanosql/resources/_query.py` & `thanosql-0.1.0/thanosql/resources/_query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
 
+import enum
 from datetime import datetime
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, List, Optional
 
-from pydantic import BaseModel, TypeAdapter
+from pydantic import TypeAdapter
 
+from thanosql._error import ThanoSQLValueError
 from thanosql._service import ThanoSQLService
+from thanosql.resources._model import BaseModel
 
 if TYPE_CHECKING:
     from thanosql._client import ThanoSQL
 
 
 class QueryLog(BaseModel):
     query_id: Optional[str]
@@ -22,58 +25,65 @@
     destination_table_name: Optional[str]
     destination_schema: Optional[str]
     error_result: Optional[str]
     created_at: Optional[datetime]
     records: Optional[list] = None
 
 
+class QueryType(enum.Enum):
+    THANOSQL = "thanosql"
+    PSQL = "psql"
+
+
 class QueryService(ThanoSQLService):
     def __init__(self, client: ThanoSQL) -> None:
         super().__init__(client=client, tag="query")
 
         self.log: QueryLogService = QueryLogService(self)
         self.template: QueryTemplateService = QueryTemplateService(self)
 
     def execute(
         self,
-        query_type: str = "thanosql",
         query: Optional[str] = None,
+        query_type: str = "thanosql",
         template_id: Optional[int] = None,
         template_name: Optional[str] = None,
         parameters: Optional[dict] = None,
         schema: Optional[str] = None,
         table_name: Optional[str] = None,
         overwrite: Optional[bool] = None,
         max_results: Optional[int] = None,
-    ) -> Union[QueryLog, dict]:
+    ) -> QueryLog:
+        try:
+            query_type_enum = QueryType(query_type)
+        except Exception as e:
+            raise ThanoSQLValueError(str(e))
+
         path = f"/{self.tag}/"
         query_params = self._create_input_dict(
             schema=schema,
             table_name=table_name,
             overwrite=overwrite,
             max_results=max_results,
         )
         payload = self._create_input_dict(
-            query_type=query_type,
+            query_type=query_type_enum.value,
             query_string=query,
             template_id=template_id,
             template_name=template_name,
             parameters=parameters,
         )
 
         raw_response = self.client._request(
             method="post", path=path, query_params=query_params, payload=payload
         )
 
-        if "query_id" in raw_response:
-            query_log_adapter = TypeAdapter(QueryLog)
-            parsed_response = query_log_adapter.validate_python(raw_response)
-            return parsed_response
-
-        return raw_response
+        query_log_adapter = TypeAdapter(QueryLog)
+        parsed_response = query_log_adapter.validate_python(raw_response)
+        return parsed_response
 
 
 class QueryLogService(ThanoSQLService):
     """Cannot exist without a parent QueryService"""
 
     def __init__(self, query: QueryService) -> None:
         super().__init__(client=query.client, tag="log")
@@ -91,24 +101,22 @@
             search=search, offset=offset, limit=limit
         )
 
         raw_response = self.client._request(
             method="get", path=path, query_params=query_params
         )
 
-        if "query_logs" in raw_response:
-            query_logs_adapter = TypeAdapter(List[QueryLog])
-            parsed_response = {}
-            parsed_response["query_logs"] = query_logs_adapter.validate_python(
-                raw_response["query_logs"]
-            )
-            parsed_response["total"] = raw_response["total"]
-            return parsed_response
+        query_logs_adapter = TypeAdapter(List[QueryLog])
+        parsed_response = {}
+        parsed_response["query_logs"] = query_logs_adapter.validate_python(
+            raw_response["query_logs"]
+        )
+        parsed_response["total"] = raw_response["total"]
 
-        return raw_response
+        return parsed_response
 
 
 class QueryTemplate(BaseModel):
     id: Optional[int] = None
     name: str
     query: str
     parameters: Optional[List[str]] = []
@@ -120,93 +128,74 @@
     """Cannot exist without a parent QueryService"""
 
     def __init__(self, query: QueryService) -> None:
         super().__init__(client=query.client, tag="template")
 
         self.query: QueryService = query
 
+    def _parse_query_template_response(self, raw_response: dict):
+        query_template_adapter = TypeAdapter(QueryTemplate)
+        parsed_response = query_template_adapter.validate_python(
+            raw_response["query_template"]
+        )
+        return parsed_response
+
     def list(
         self,
         search: Optional[str] = None,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
         order_by: Optional[str] = None,
-    ) -> Union[List[QueryTemplate], dict]:
+    ) -> List[QueryTemplate]:
         path = f"/{self.query.tag}/{self.tag}"
         query_params = self._create_input_dict(
             search=search, offset=offset, limit=limit, order_by=order_by
         )
 
         raw_response = self.client._request(
             method="get", path=path, query_params=query_params
         )
 
-        if "query_templates" in raw_response:
-            query_templates_adapter = TypeAdapter(List[QueryTemplate])
-            parsed_response = query_templates_adapter.validate_python(
-                raw_response["query_templates"]
-            )
-            return parsed_response
-
-        return raw_response
+        query_templates_adapter = TypeAdapter(List[QueryTemplate])
+        parsed_response = query_templates_adapter.validate_python(
+            raw_response["query_templates"]
+        )
+        return parsed_response
 
     def create(
         self,
         name: Optional[str] = None,
         query: Optional[str] = None,
         dry_run: Optional[bool] = None,
-    ) -> Union[QueryTemplate, dict]:
+    ) -> QueryTemplate:
         path = f"/{self.query.tag}/{self.tag}"
         query_params = self._create_input_dict(dry_run=dry_run)
         payload = self._create_input_dict(name=name, query=query)
 
         raw_response = self.client._request(
             method="post", path=path, query_params=query_params, payload=payload
         )
 
-        if "query_template" in raw_response:
-            query_template_adapter = TypeAdapter(QueryTemplate)
-            parsed_response = query_template_adapter.validate_python(
-                raw_response["query_template"]
-            )
-            return parsed_response
-
-        return raw_response
+        return self._parse_query_template_response(raw_response)
 
-    def get(self, name: str) -> Union[QueryTemplate, dict]:
+    def get(self, name: str) -> QueryTemplate:
         path = f"/{self.query.tag}/{self.tag}/{name}"
-
         raw_response = self.client._request(method="get", path=path)
-
-        if "query_template" in raw_response:
-            query_template_adapter = TypeAdapter(QueryTemplate)
-            parsed_response = query_template_adapter.validate_python(
-                raw_response["query_template"]
-            )
-            return parsed_response
-
-        return raw_response
+        return self._parse_query_template_response(raw_response)
 
     def update(
         self,
         current_name: str,
         new_name: Optional[str] = None,
         query: Optional[str] = None,
-    ) -> Union[QueryTemplate, dict]:
+    ) -> QueryTemplate:
         path = f"/{self.query.tag}/{self.tag}/{current_name}"
         payload = self._create_input_dict(name=new_name, query=query)
 
         raw_response = self.client._request(method="put", path=path, payload=payload)
 
-        if "query_template" in raw_response:
-            query_template_adapter = TypeAdapter(QueryTemplate)
-            parsed_response = query_template_adapter.validate_python(
-                raw_response["query_template"]
-            )
-            return parsed_response
-
-        return raw_response
+        return self._parse_query_template_response(raw_response)
 
     def delete(self, name: str) -> dict:
         path = f"/{self.query.tag}/{self.tag}/{name}"
 
         return self.client._request(method="delete", path=path)
```

### Comparing `thanosql-0.0.2/thanosql/resources/_schema.py` & `thanosql-0.1.0/thanosql/resources/_schema.py`

 * *Files identical despite different names*

### Comparing `thanosql-0.0.2/thanosql/resources/_table.py` & `thanosql-0.1.0/thanosql/resources/_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import os
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field, TypeAdapter
+from pydantic import Field, TypeAdapter
 
 from thanosql._error import ThanoSQLValueError
 from thanosql._service import ThanoSQLService
+from thanosql.resources._model import BaseModel
 
 if TYPE_CHECKING:
     from thanosql._client import ThanoSQL
 
 
 class BaseColumn(BaseModel):
     default: Optional[str] = None
@@ -67,90 +68,89 @@
 
 class TableService(ThanoSQLService):
     def __init__(self, client: ThanoSQL) -> None:
         super().__init__(client=client, tag="table")
 
         self.template: TableTemplateService = TableTemplateService(client)
 
+    def _parse_table_response(self, raw_response: dict) -> Table:
+        table_adapter = TypeAdapter(Table)
+        parsed_response = table_adapter.validate_python(raw_response["table"])
+        parsed_response.service = self
+        return parsed_response
+
     def list(
         self,
         schema: Optional[str] = None,
         verbose: Optional[bool] = None,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
-    ) -> Union[List[BaseTable], dict]:
+    ) -> List[Table]:
         path = f"/{self.tag}/"
         query_params = self._create_input_dict(
             schema=schema, verbose=verbose, offset=offset, limit=limit
         )
 
         raw_response = self.client._request(
             method="get", path=path, query_params=query_params
         )
 
-        if "tables" in raw_response:
-            tables_adapter = TypeAdapter(List[BaseTable])
-            parsed_response = tables_adapter.validate_python(
-                raw_response["tables"]
-            )
-            return parsed_response
-
-        return raw_response
+        tables_adapter = TypeAdapter(List[Table])
+        parsed_response = tables_adapter.validate_python(raw_response["tables"])
+        for table in parsed_response:
+            table.service = self
+        return parsed_response
 
     def get(self, name: str, schema: Optional[str] = None) -> Union[Table, dict]:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(schema=schema)
 
         raw_response = self.client._request(
             method="get", path=path, query_params=query_params
         )
 
-        if "table" in raw_response:
-            table_adapter = TypeAdapter(Table)
-            parsed_response = table_adapter.validate_python(
-                raw_response["table"]
-            )
-            parsed_response.service = self
-            return parsed_response
-
-        return raw_response
+        return self._parse_table_response(raw_response)
 
     def update(
         self, name: str, schema: Optional[str] = None, table: Optional[BaseTable] = None
-    ) -> dict:
+    ) -> Table:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(schema=schema)
         payload = self._create_input_dict(table=table)
 
-        return self.client._request(
+        raw_response = self.client._request(
             method="put", path=path, query_params=query_params, payload=payload
         )
 
+        return self._parse_table_response(raw_response)
+
     def create(
         self,
         name: str,
         schema: Optional[str] = None,
         table: Optional[TableObject] = None,
-    ) -> dict:
+    ) -> Table:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(schema=schema)
         payload = self._create_input_dict(table=table)
 
-        return self.client._request(
+        raw_response = self.client._request(
             method="post", path=path, query_params=query_params, payload=payload
         )
 
+        return self._parse_table_response(raw_response)
+
     def upload(
         self,
         name: str,
         file: Union[str, os.PathLike],
         schema: Optional[str] = None,
         table: Optional[TableObject] = None,
         if_exists: Optional[str] = None,
-    ) -> dict:
+    ) -> Table:
         path = f"/{self.tag}/{name}/upload/"
 
         file_extension = Path(file).suffix.lower()
         if file_extension == ".csv":
             path = path + "csv"
         elif file_extension in [
             ".xls",
@@ -166,22 +166,24 @@
             raise ThanoSQLValueError(
                 "Invalid format: only CSV and Excel files possible."
             )
 
         query_params = self._create_input_dict(schema=schema, if_exists=if_exists)
         payload = self._create_input_dict(table=table)
 
-        return self.client._request(
+        raw_response = self.client._request(
             method="post",
             path=path,
             query_params=query_params,
             payload=payload,
             file=file,
         )
 
+        return self._parse_table_response(raw_response)
+
     def delete(self, name: str, schema: Optional[str] = None) -> dict:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(schema=schema)
 
         return self.client._request(
             method="delete", path=path, query_params=query_params
         )
@@ -200,84 +202,81 @@
         super().__init__(client=client, tag="table_template")
 
     def list(
         self,
         search: Optional[str] = None,
         order_by: Optional[str] = None,
         latest: Optional[bool] = None,
-    ) -> Union[List[TableTemplate], dict]:
+    ) -> List[TableTemplate]:
         path = f"/{self.tag}/"
         query_params = self._create_input_dict(
             search=search,
             order_by=order_by,
             latest=latest,
         )
 
         raw_response = self.client._request(
             method="get", path=path, query_params=query_params
         )
 
-        if "table_templates" in raw_response:
-            table_templates_adapter = TypeAdapter(List[TableTemplate])
-            parsed_response = table_templates_adapter.validate_python(
-                raw_response["table_templates"]
-            )
-            return parsed_response
-
-        return raw_response
+        table_templates_adapter = TypeAdapter(List[TableTemplate])
+        parsed_response = table_templates_adapter.validate_python(
+            raw_response["table_templates"]
+        )
+        return parsed_response
 
     def get(self, name: str, version: Optional[str] = None) -> dict:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(version=version)
 
         raw_response = self.client._request(
             method="get", path=path, query_params=query_params
         )
 
-        if "table_templates" in raw_response:
-            table_templates_adapter = TypeAdapter(List[TableTemplate])
-            parsed_response = {}
-            parsed_response[
-                "table_templates"
-            ] = table_templates_adapter.validate_python(
-                raw_response["table_templates"]
-            )
-            parsed_response["versions"] = raw_response["versions"]
-            return parsed_response
+        table_templates_adapter = TypeAdapter(List[TableTemplate])
+        parsed_response = {}
+        parsed_response["table_templates"] = table_templates_adapter.validate_python(
+            raw_response["table_templates"]
+        )
+        parsed_response["versions"] = raw_response["versions"]
 
-        return raw_response
+        return parsed_response
 
     def create(
         self,
         name: str,
         table_template: TableObject,
         version: Optional[str] = None,
         compatibility: Optional[str] = None,
-    ) -> dict:
+    ) -> TableTemplate:
         path = f"/{self.tag}/{name}"
         payload = self._create_input_dict(
             table_template=vars(table_template),
             version=version,
             compatibility=compatibility,
         )
 
-        return self.client._request(method="post", path=path, payload=payload)
+        raw_response = self.client._request(method="post", path=path, payload=payload)
+
+        table_template_adapter = TypeAdapter(TableTemplate)
+        parsed_response = table_template_adapter.validate_python(
+            raw_response["table_template"]
+        )
+        return parsed_response
 
     def delete(self, name: str, version: Optional[str] = None) -> dict:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(version=version)
 
         return self.client._request(
             method="delete", path=path, query_params=query_params
         )
 
 
 class Table(BaseTable):
-    model_config = ConfigDict(arbitrary_types_allowed=True)
-
     service: Optional[TableService] = None
 
     def get_records(
         self,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
     ) -> dict:
@@ -309,14 +308,16 @@
         self.service.client._request(
             method="get", path=path, query_params=query_params, stream=True
         )
 
     def insert(
         self,
         records: List[dict],
-    ) -> dict:
+    ) -> Union[Table, dict]:
         path = f"/{self.service.tag}/{self.name}/records"
         query_params = self.service._create_input_dict(schema=self.table_schema)
 
-        return self.service.client._request(
+        raw_response = self.service.client._request(
             method="post", path=path, query_params=query_params, payload=records
         )
+
+        return self.service._parse_table_response(raw_response)
```

### Comparing `thanosql-0.0.2/thanosql/resources/_view.py` & `thanosql-0.1.0/thanosql/resources/_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, List, Optional
 
-from pydantic import BaseModel, Field, TypeAdapter
+from pydantic import Field, TypeAdapter
 
 from thanosql._service import ThanoSQLService
 from thanosql.resources import Column
+from thanosql.resources._model import BaseModel
 
 if TYPE_CHECKING:
     from thanosql._client import ThanoSQL
 
 
 class View(BaseModel):
     name: str
@@ -24,50 +25,42 @@
 
     def list(
         self,
         schema: Optional[str] = None,
         verbose: Optional[bool] = None,
         offset: Optional[int] = None,
         limit: Optional[int] = None,
-    ) -> Union[List[View], dict]:
+    ) -> List[View]:
         path = f"/{self.tag}/"
         query_params = self._create_input_dict(
             schema=schema,
             verbose=verbose,
             offset=offset,
             limit=limit,
         )
 
         raw_response = self.client._request(
             method="get", path=path, query_params=query_params
         )
 
-        if "views" in raw_response:
-            views_adapter = TypeAdapter(List[View])
-            parsed_response = views_adapter.validate_python(
-                raw_response["views"]
-            )
-            return parsed_response
+        views_adapter = TypeAdapter(List[View])
+        parsed_response = views_adapter.validate_python(raw_response["views"])
+        return parsed_response
 
-        return raw_response
-
-    def get(self, name: str, schema: Optional[str] = None) -> Union[View, dict]:
+    def get(self, name: str, schema: Optional[str] = None) -> View:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(schema=schema)
 
         raw_response = self.client._request(
             method="get", path=path, query_params=query_params
         )
 
-        if "view" in raw_response:
-            view_adapter = TypeAdapter(View)
-            parsed_response = view_adapter.validate_python(raw_response["view"])
-            return parsed_response
-
-        return raw_response
+        view_adapter = TypeAdapter(View)
+        parsed_response = view_adapter.validate_python(raw_response["view"])
+        return parsed_response
 
     def delete(self, name: str, schema: Optional[str] = None) -> dict:
         path = f"/{self.tag}/{name}"
         query_params = self._create_input_dict(schema=schema)
 
         return self.client._request(
             method="delete", path=path, query_params=query_params
```

### Comparing `thanosql-0.0.2/thanosql.egg-info/PKG-INFO` & `thanosql-0.1.0/thanosql.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thanosql
-Version: 0.0.2
+Version: 0.1.0
 Summary: ThanoSQL SDK for Python
 Home-page: https://github.com/smartmind-team/thanosql-python
 Author: SmartMind
 Author-email: dev@smartmind.team
 License: MIT
 Keywords: smartmind thanosql sdk
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,17 @@
 Requires-Dist: requests
 Requires-Dist: urllib3
 Requires-Dist: pydantic>=2.0
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: faker; extra == "dev"
+Requires-Dist: myst-nb; extra == "dev"
+Requires-Dist: sphinx-autoapi; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Provides-Extra: magic
 Requires-Dist: ipython; extra == "magic"
 Requires-Dist: pandas; extra == "magic"
 Requires-Dist: sqlalchemy; extra == "magic"
 Requires-Dist: numpy; extra == "magic"
 Requires-Dist: matplotlib; extra == "magic"
 Requires-Dist: websocket-client; extra == "magic"
@@ -51,29 +54,30 @@
 >
 > `pip install 'thanosql[magic]'`
 
 Alternatively, you can also install from source. First, clone this repository.
 
 ```bash
 git clone https://github.com/smartmind-team/thanosql-sdk-python.git
+cd thanosql-sdk-python
 ```
 
 Install the SDK by using `pip install`. Note that the Python version used during development is 3.8.10.
 
 ```bash
 pip install -e .
-pip install -e ."[dev]" # include unit test
+pip install -e ."[dev]" # include unit test & docs (requires python >= 3.9)
 pip install -e ."[magic]" # include magic
 ```
 
 ## Usage
 
-In order to use the library, a working workspace engine is required. Create a new Python or IPython notebook file. Import the `thanosql` package, create a `ThanoSQL` client with your API token and engine URL, and then you can use all the functions in the library. For more examples, head over to the [examples/](./examples/) directory.
+In order to use the library, a working workspace engine is required. Create a new Python or IPython notebook file. Import the `thanosql` package, create a `ThanoSQL` client with your API token and engine URL, and then you can use all the functions in the library. For more examples, head over to the [examples](./docs/examples/) directory.
 
-1. Set up your API_TOKEN and ENGINE_URL (recommended).
+1. First, set up your API_TOKEN and ENGINE_URL (recommended). You can find them by accessing your workspace's settings page. Head over to the `Developer` tab, and then copy your API Token and Engine URL.
 
    ```bash
    export THANOSQL_API_TOKEN='your-api-token-here'
    export THANOSQL_ENGINE_URL='your-engine-url-here'
    ```
 
 2. Import the ThanoSQL client and use it to query your ThanoSQL Workspace.
```

### Comparing `thanosql-0.0.2/thanosql.egg-info/SOURCES.txt` & `thanosql-0.1.0/thanosql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 thanosql/magic/__init__.py
 thanosql/magic/exception.py
 thanosql/magic/magic.py
 thanosql/magic/parse.py
 thanosql/magic/util.py
 thanosql/resources/__init__.py
 thanosql/resources/_file.py
+thanosql/resources/_model.py
 thanosql/resources/_query.py
 thanosql/resources/_schema.py
 thanosql/resources/_table.py
 thanosql/resources/_view.py
```

