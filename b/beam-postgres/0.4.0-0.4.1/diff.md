# Comparing `tmp/beam-postgres-0.4.0.tar.gz` & `tmp/beam-postgres-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam-postgres-0.4.0.tar", last modified: Thu Jan 11 13:00:51 2024, max compression
+gzip compressed data, was "beam-postgres-0.4.1.tar", last modified: Thu Apr  4 14:26:17 2024, max compression
```

## Comparing `beam-postgres-0.4.0.tar` & `beam-postgres-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 amedzinski   (501) staff       (20)        0 2024-01-11 13:00:51.028890 beam-postgres-0.4.0/
--rw-r--r--   0 amedzinski   (501) staff       (20)    11345 2024-01-02 12:27:35.000000 beam-postgres-0.4.0/LICENSE
--rw-r--r--   0 amedzinski   (501) staff       (20)     3258 2024-01-11 13:00:51.028815 beam-postgres-0.4.0/PKG-INFO
--rw-r--r--   0 amedzinski   (501) staff       (20)     1917 2024-01-11 12:53:47.000000 beam-postgres-0.4.0/README.md
-drwxr-xr-x   0 amedzinski   (501) staff       (20)        0 2024-01-11 13:00:51.024684 beam-postgres-0.4.0/beam_postgres/
--rw-r--r--   0 amedzinski   (501) staff       (20)       22 2024-01-11 12:57:54.000000 beam-postgres-0.4.0/beam_postgres/__init__.py
-drwxr-xr-x   0 amedzinski   (501) staff       (20)        0 2024-01-11 13:00:51.025668 beam-postgres-0.4.0/beam_postgres/io/
--rw-r--r--   0 amedzinski   (501) staff       (20)      188 2024-01-11 12:53:47.000000 beam-postgres-0.4.0/beam_postgres/io/__init__.py
--rw-r--r--   0 amedzinski   (501) staff       (20)    11023 2024-01-11 12:53:47.000000 beam-postgres-0.4.0/beam_postgres/io/postgres.py
--rw-r--r--   0 amedzinski   (501) staff       (20)     1336 2024-01-02 12:27:35.000000 beam-postgres-0.4.0/beam_postgres/io/retry.py
-drwxr-xr-x   0 amedzinski   (501) staff       (20)        0 2024-01-11 13:00:51.028299 beam-postgres-0.4.0/beam_postgres.egg-info/
--rw-r--r--   0 amedzinski   (501) staff       (20)     3258 2024-01-11 13:00:51.000000 beam-postgres-0.4.0/beam_postgres.egg-info/PKG-INFO
--rw-r--r--   0 amedzinski   (501) staff       (20)      345 2024-01-11 13:00:51.000000 beam-postgres-0.4.0/beam_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 amedzinski   (501) staff       (20)        1 2024-01-11 13:00:51.000000 beam-postgres-0.4.0/beam_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 amedzinski   (501) staff       (20)      121 2024-01-11 13:00:51.000000 beam-postgres-0.4.0/beam_postgres.egg-info/requires.txt
--rw-r--r--   0 amedzinski   (501) staff       (20)       14 2024-01-11 13:00:51.000000 beam-postgres-0.4.0/beam_postgres.egg-info/top_level.txt
--rw-r--r--   0 amedzinski   (501) staff       (20)     1729 2024-01-11 12:57:54.000000 beam-postgres-0.4.0/pyproject.toml
--rw-r--r--   0 amedzinski   (501) staff       (20)      150 2024-01-11 13:00:51.029083 beam-postgres-0.4.0/setup.cfg
--rw-r--r--   0 amedzinski   (501) staff       (20)       38 2024-01-02 12:27:35.000000 beam-postgres-0.4.0/setup.py
+drwxr-xr-x   0 amedzinski   (501) staff       (20)        0 2024-04-04 14:26:17.856959 beam-postgres-0.4.1/
+-rw-r--r--   0 amedzinski   (501) staff       (20)    11345 2024-01-02 12:27:35.000000 beam-postgres-0.4.1/LICENSE
+-rw-r--r--   0 amedzinski   (501) staff       (20)     3625 2024-04-04 14:26:17.849009 beam-postgres-0.4.1/PKG-INFO
+-rw-r--r--   0 amedzinski   (501) staff       (20)     2183 2024-01-11 13:19:11.000000 beam-postgres-0.4.1/README.md
+drwxr-xr-x   0 amedzinski   (501) staff       (20)        0 2024-04-04 14:26:17.846701 beam-postgres-0.4.1/beam_postgres/
+-rw-r--r--   0 amedzinski   (501) staff       (20)       22 2024-04-04 14:19:57.000000 beam-postgres-0.4.1/beam_postgres/__init__.py
+drwxr-xr-x   0 amedzinski   (501) staff       (20)        0 2024-04-04 14:26:17.847902 beam-postgres-0.4.1/beam_postgres/io/
+-rw-r--r--   0 amedzinski   (501) staff       (20)      188 2024-01-11 12:53:47.000000 beam-postgres-0.4.1/beam_postgres/io/__init__.py
+-rw-r--r--   0 amedzinski   (501) staff       (20)    11039 2024-01-11 13:12:55.000000 beam-postgres-0.4.1/beam_postgres/io/postgres.py
+-rw-r--r--   0 amedzinski   (501) staff       (20)     1336 2024-01-02 12:27:35.000000 beam-postgres-0.4.1/beam_postgres/io/retry.py
+drwxr-xr-x   0 amedzinski   (501) staff       (20)        0 2024-04-04 14:26:17.848375 beam-postgres-0.4.1/beam_postgres.egg-info/
+-rw-r--r--   0 amedzinski   (501) staff       (20)     3625 2024-04-04 14:26:17.000000 beam-postgres-0.4.1/beam_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 amedzinski   (501) staff       (20)      345 2024-04-04 14:26:17.000000 beam-postgres-0.4.1/beam_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 amedzinski   (501) staff       (20)        1 2024-04-04 14:26:17.000000 beam-postgres-0.4.1/beam_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 amedzinski   (501) staff       (20)      121 2024-04-04 14:26:17.000000 beam-postgres-0.4.1/beam_postgres.egg-info/requires.txt
+-rw-r--r--   0 amedzinski   (501) staff       (20)       14 2024-04-04 14:26:17.000000 beam-postgres-0.4.1/beam_postgres.egg-info/top_level.txt
+-rw-r--r--   0 amedzinski   (501) staff       (20)     1820 2024-04-04 14:19:57.000000 beam-postgres-0.4.1/pyproject.toml
+-rw-r--r--   0 amedzinski   (501) staff       (20)      150 2024-04-04 14:26:17.857264 beam-postgres-0.4.1/setup.cfg
+-rw-r--r--   0 amedzinski   (501) staff       (20)       38 2024-01-02 12:27:35.000000 beam-postgres-0.4.1/setup.py
```

### Comparing `beam-postgres-0.4.0/LICENSE` & `beam-postgres-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beam-postgres-0.4.0/PKG-INFO` & `beam-postgres-0.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: beam-postgres
-Version: 0.4.0
+Version: 0.4.1
 Summary: Light IO transforms for Postgres read/write in Apache Beam pipelines.
 Author: Adam Medziński
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/medzin/beam-postgres
 Keywords: apache beam,beam,postgres,postgresql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-beam<3,>=2.42.0
 Requires-Dist: psycopg[binary]<4,>=3.1.4
 Provides-Extra: dev
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
@@ -98,9 +100,16 @@
         "insert into sink (data) values (%s)",
     )
 
 ```
 
 See [here][examples] for more examples.
 
+### Reading in batches
+
+There may be situations when you have so much data that it will not fit into the
+memory - then you want to read your table data in batches. You can see an
+example code [here](examples/read.py#L11) (the code reads records in a batches of
+1).
+
 [pypi-project]: https://pypi.org/project/beam-postgres
 [examples]: https://github.com/medzin/beam-postgres/tree/main/examples
```

### Comparing `beam-postgres-0.4.0/README.md` & `beam-postgres-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -64,9 +64,16 @@
         "insert into sink (data) values (%s)",
     )
 
 ```
 
 See [here][examples] for more examples.
 
+### Reading in batches
+
+There may be situations when you have so much data that it will not fit into the
+memory - then you want to read your table data in batches. You can see an
+example code [here](examples/read.py#L11) (the code reads records in a batches of
+1).
+
 [pypi-project]: https://pypi.org/project/beam-postgres
 [examples]: https://github.com/medzin/beam-postgres/tree/main/examples
```

### Comparing `beam-postgres-0.4.0/beam_postgres/io/postgres.py` & `beam-postgres-0.4.1/beam_postgres/io/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         self._rows_buffer = []
 
         return itertools.chain(
             [
                 WindowedValue(
                     (row, err),
                     GlobalWindow().max_timestamp(),
-                    [_IntervalWindowBase(0, GlobalWindow().max_timestamp())],
+                    [_IntervalWindowBase(0, GlobalWindow().max_timestamp())],  # type: ignore
                 )
                 for row, err in failed_rows
             ],
         )
 
 
 class WriteToPostgres(PTransform):
```

### Comparing `beam-postgres-0.4.0/beam_postgres/io/retry.py` & `beam-postgres-0.4.1/beam_postgres/io/retry.py`

 * *Files identical despite different names*

### Comparing `beam-postgres-0.4.0/beam_postgres.egg-info/PKG-INFO` & `beam-postgres-0.4.1/beam_postgres.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: beam-postgres
-Version: 0.4.0
+Version: 0.4.1
 Summary: Light IO transforms for Postgres read/write in Apache Beam pipelines.
 Author: Adam Medziński
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/medzin/beam-postgres
 Keywords: apache beam,beam,postgres,postgresql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: apache-beam<3,>=2.42.0
 Requires-Dist: psycopg[binary]<4,>=3.1.4
 Provides-Extra: dev
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
@@ -98,9 +100,16 @@
         "insert into sink (data) values (%s)",
     )
 
 ```
 
 See [here][examples] for more examples.
 
+### Reading in batches
+
+There may be situations when you have so much data that it will not fit into the
+memory - then you want to read your table data in batches. You can see an
+example code [here](examples/read.py#L11) (the code reads records in a batches of
+1).
+
 [pypi-project]: https://pypi.org/project/beam-postgres
 [examples]: https://github.com/medzin/beam-postgres/tree/main/examples
```

### Comparing `beam-postgres-0.4.0/pyproject.toml` & `beam-postgres-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [project]
 name = "beam-postgres"
-version = "0.4.0"
+version = "0.4.1"
 description = "Light IO transforms for Postgres read/write in Apache Beam pipelines."
 readme = "README.md"
 authors = [{ name = "Adam Medziński" }]
 license = { text = "Apache-2.0" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["apache beam", "beam", "postgres", "postgresql"]
 dependencies = [
     "apache-beam>=2.42.0,<3",
     "psycopg[binary]>=3.1.4,<4",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 
 [project.optional-dependencies]
 dev = ["bumpver", "pip-tools", "tox"]
 tests = ["black", "flake8", "isort", "mypy", "pytest>=7"]
 
 [project.urls]
 Homepage = "https://github.com/medzin/beam-postgres"
@@ -35,15 +37,15 @@
 requires = ["setuptools>=65.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["beam_postgres", "beam_postgres.io"]
 
 [tool.bumpver]
-current_version = "0.4.0"
+current_version = "0.4.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

