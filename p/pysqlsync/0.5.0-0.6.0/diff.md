# Comparing `tmp/pysqlsync-0.5.0.tar.gz` & `tmp/pysqlsync-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqlsync-0.5.0.tar", last modified: Thu Mar  7 14:26:47 2024, max compression
+gzip compressed data, was "pysqlsync-0.6.0.tar", last modified: Thu Apr  4 09:19:36 2024, max compression
```

## Comparing `pysqlsync-0.5.0.tar` & `pysqlsync-0.6.0.tar`

### file list

```diff
@@ -1,129 +1,130 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.523229 pysqlsync-0.5.0/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1077 2024-01-09 18:31:29.000000 pysqlsync-0.5.0/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       29 2023-10-12 10:08:53.000000 pysqlsync-0.5.0/MANIFEST.in
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12929 2024-03-07 14:26:47.522070 pysqlsync-0.5.0/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11382 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/README.md
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-02-26 22:48:42.000000 pysqlsync-0.5.0/pyproject.toml
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.400780 pysqlsync-0.5.0/pysqlsync/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      484 2024-03-07 14:18:30.000000 pysqlsync-0.5.0/pysqlsync/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    44164 2024-01-09 21:01:26.000000 pysqlsync-0.5.0/pysqlsync/base.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.407496 pysqlsync-0.5.0/pysqlsync/data/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-10-12 10:02:10.000000 pysqlsync-0.5.0/pysqlsync/data/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5235 2023-11-19 23:44:07.000000 pysqlsync-0.5.0/pysqlsync/data/exchange.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11076 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/data/generator.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.408576 pysqlsync-0.5.0/pysqlsync/dialect/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-17 09:48:30.000000 pysqlsync-0.5.0/pysqlsync/dialect/__init__.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.416003 pysqlsync-0.5.0/pysqlsync/dialect/mssql/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-10-16 09:03:38.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4755 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3310 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/data_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      207 2023-12-05 20:17:49.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/dependency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3396 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/discovery.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      552 2023-10-24 09:16:44.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/engine.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3768 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/generator.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1851 2024-03-05 22:18:04.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/mutation.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2887 2024-03-05 22:19:13.000000 pysqlsync-0.5.0/pysqlsync/dialect/mssql/object_types.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.423318 pysqlsync-0.5.0/pysqlsync/dialect/mysql/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-17 09:59:28.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3355 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1286 2023-10-27 11:19:12.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/data_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      228 2023-12-05 20:17:49.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/dependency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6555 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/discovery.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      552 2023-10-08 17:09:14.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/engine.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6504 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/generator.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2859 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/mutation.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2544 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/mysql/object_types.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.432287 pysqlsync-0.5.0/pysqlsync/dialect/oracle/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4381 2023-12-21 09:21:09.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3399 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/data_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      195 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/dependency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8614 2024-01-31 19:48:29.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/discovery.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      560 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/engine.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4691 2024-01-11 22:52:45.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/generator.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1310 2023-12-21 09:21:09.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/mutation.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1720 2024-03-05 22:19:28.000000 pysqlsync-0.5.0/pysqlsync/dialect/oracle/object_types.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.439962 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-26 23:17:21.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3913 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      145 2023-10-27 11:23:57.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/data_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      198 2023-12-05 20:17:49.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/dependency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    15967 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/discovery.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      592 2023-10-03 23:39:29.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/engine.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4240 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/generator.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2874 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/mutation.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2804 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/dialect/postgresql/object_types.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.446110 pysqlsync-0.5.0/pysqlsync/dialect/redshift/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/redshift/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5348 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/redshift/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      303 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/redshift/data_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      211 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/redshift/dependency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      592 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/redshift/engine.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3437 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/redshift/generator.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.447860 pysqlsync-0.5.0/pysqlsync/dialect/test/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-12-05 20:17:49.000000 pysqlsync-0.5.0/pysqlsync/dialect/test/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      260 2023-12-05 20:17:49.000000 pysqlsync-0.5.0/pysqlsync/dialect/test/dependency.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.454469 pysqlsync-0.5.0/pysqlsync/dialect/trino/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-17 09:48:43.000000 pysqlsync-0.5.0/pysqlsync/dialect/trino/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2759 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/trino/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      218 2023-12-05 20:17:49.000000 pysqlsync-0.5.0/pysqlsync/dialect/trino/dependency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      698 2023-10-24 19:28:46.000000 pysqlsync-0.5.0/pysqlsync/dialect/trino/discovery.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      552 2023-10-21 22:26:33.000000 pysqlsync-0.5.0/pysqlsync/dialect/trino/engine.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1035 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/dialect/trino/generator.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4425 2023-12-05 20:17:49.000000 pysqlsync-0.5.0/pysqlsync/factory.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.465882 pysqlsync-0.5.0/pysqlsync/formation/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-01 17:58:22.000000 pysqlsync-0.5.0/pysqlsync/formation/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2456 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/formation/constraints.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7494 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/formation/data_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    16739 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/formation/discovery.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5046 2023-12-09 10:29:59.000000 pysqlsync-0.5.0/pysqlsync/formation/inspection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13311 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/formation/mutation.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2564 2023-12-09 10:29:59.000000 pysqlsync-0.5.0/pysqlsync/formation/object_dict.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    25020 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/formation/object_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    39578 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/formation/py_to_sql.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7038 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/formation/sql_to_py.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.472786 pysqlsync-0.5.0/pysqlsync/model/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-03 22:18:33.000000 pysqlsync-0.5.0/pysqlsync/model/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9493 2023-12-21 09:21:09.000000 pysqlsync-0.5.0/pysqlsync/model/data_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2253 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/model/entity_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4273 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/pysqlsync/model/id_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      739 2023-12-15 15:04:38.000000 pysqlsync-0.5.0/pysqlsync/model/key_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7348 2023-12-09 10:29:59.000000 pysqlsync-0.5.0/pysqlsync/model/properties.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-16 08:19:48.000000 pysqlsync-0.5.0/pysqlsync/py.typed
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6393 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/pysqlsync/python_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3555 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/pysqlsync/resultset.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.476201 pysqlsync-0.5.0/pysqlsync/util/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-10-25 19:55:04.000000 pysqlsync-0.5.0/pysqlsync/util/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      932 2023-11-12 15:30:43.000000 pysqlsync-0.5.0/pysqlsync/util/dispatch.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      478 2023-11-14 21:10:43.000000 pysqlsync-0.5.0/pysqlsync/util/typing.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.516625 pysqlsync-0.5.0/pysqlsync.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12929 2024-03-07 14:26:47.000000 pysqlsync-0.5.0/pysqlsync.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3437 2024-03-07 14:26:47.000000 pysqlsync-0.5.0/pysqlsync.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-03-07 14:26:47.000000 pysqlsync-0.5.0/pysqlsync.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      228 2024-03-07 14:26:47.000000 pysqlsync-0.5.0/pysqlsync.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       10 2024-03-07 14:26:47.000000 pysqlsync-0.5.0/pysqlsync.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-01-29 11:32:47.000000 pysqlsync-0.5.0/pysqlsync.egg-info/zip-safe
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1458 2024-03-07 14:26:47.525063 pysqlsync-0.5.0/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      257 2023-10-24 18:23:35.000000 pysqlsync-0.5.0/setup.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.506287 pysqlsync-0.5.0/tests/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-01-19 19:01:00.000000 pysqlsync-0.5.0/tests/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3406 2023-12-09 10:29:59.000000 pysqlsync-0.5.0/tests/example.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1201 2023-11-14 21:21:57.000000 pysqlsync-0.5.0/tests/measure.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-03-07 14:26:47.512801 pysqlsync-0.5.0/tests/model/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-10-29 17:20:40.000000 pysqlsync-0.5.0/tests/model/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1686 2023-11-30 20:29:28.000000 pysqlsync-0.5.0/tests/model/event.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      553 2023-10-29 17:25:49.000000 pysqlsync-0.5.0/tests/model/school.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      397 2024-03-02 21:32:04.000000 pysqlsync-0.5.0/tests/model/user.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3441 2024-01-11 23:04:45.000000 pysqlsync-0.5.0/tests/params.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4390 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/tests/tables.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8307 2024-01-09 17:26:59.000000 pysqlsync-0.5.0/tests/test_connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    15521 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/tests/test_converter.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4892 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/tests/test_discovery.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2749 2023-11-17 20:44:25.000000 pysqlsync-0.5.0/tests/test_exchange.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    29603 2024-01-11 22:58:08.000000 pysqlsync-0.5.0/tests/test_generator.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      509 2024-01-11 23:14:38.000000 pysqlsync-0.5.0/tests/test_import.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3281 2023-12-13 15:01:43.000000 pysqlsync-0.5.0/tests/test_performance.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13647 2024-03-07 14:04:30.000000 pysqlsync-0.5.0/tests/test_synchronize.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2973 2023-12-21 09:21:09.000000 pysqlsync-0.5.0/tests/test_types.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      352 2023-02-26 20:14:36.000000 pysqlsync-0.5.0/tests/timed_test.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1175 2023-12-09 10:29:59.000000 pysqlsync-0.5.0/tests/update_readme.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.106997 pysqlsync-0.6.0/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1077 2024-01-09 18:31:29.000000 pysqlsync-0.6.0/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       29 2023-10-12 10:08:53.000000 pysqlsync-0.6.0/MANIFEST.in
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12929 2024-04-04 09:19:36.106545 pysqlsync-0.6.0/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11382 2024-03-07 14:04:30.000000 pysqlsync-0.6.0/README.md
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-02-26 22:48:42.000000 pysqlsync-0.6.0/pyproject.toml
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.044700 pysqlsync-0.6.0/pysqlsync/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      484 2024-04-04 09:18:56.000000 pysqlsync-0.6.0/pysqlsync/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    44215 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/base.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.049252 pysqlsync-0.6.0/pysqlsync/data/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-10-12 10:02:10.000000 pysqlsync-0.6.0/pysqlsync/data/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5235 2023-11-19 23:44:07.000000 pysqlsync-0.6.0/pysqlsync/data/exchange.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11076 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/pysqlsync/data/generator.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.049938 pysqlsync-0.6.0/pysqlsync/dialect/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-17 09:48:30.000000 pysqlsync-0.6.0/pysqlsync/dialect/__init__.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.055365 pysqlsync-0.6.0/pysqlsync/dialect/mssql/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-10-16 09:03:38.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4755 2024-04-04 09:10:13.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3310 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/data_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      207 2023-12-05 20:17:49.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/dependency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3396 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/discovery.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      552 2023-10-24 09:16:44.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/engine.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3829 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1851 2024-03-05 22:18:04.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/mutation.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3054 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/mssql/object_types.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.060034 pysqlsync-0.6.0/pysqlsync/dialect/mysql/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-17 09:59:28.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3355 2024-04-04 09:10:15.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1286 2023-10-27 11:19:12.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/data_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      228 2023-12-05 20:17:49.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/dependency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6555 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/discovery.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      552 2023-10-08 17:09:14.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/engine.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6565 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2859 2024-03-07 19:40:47.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/mutation.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2846 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/mysql/object_types.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.064707 pysqlsync-0.6.0/pysqlsync/dialect/oracle/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4381 2023-12-21 09:21:09.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3399 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/data_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      195 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/dependency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8614 2024-01-31 19:48:29.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/discovery.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      560 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/engine.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4752 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1310 2023-12-21 09:21:09.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/mutation.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1886 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/oracle/object_types.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.069383 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-26 23:17:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3913 2024-04-04 09:17:01.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      145 2023-10-27 11:23:57.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/data_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      198 2023-12-05 20:17:49.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/dependency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    15967 2024-03-07 14:04:30.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/discovery.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      592 2023-10-03 23:39:29.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/engine.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4301 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3202 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/mutation.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3007 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/postgresql/object_types.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.074543 pysqlsync-0.6.0/pysqlsync/dialect/redshift/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/dialect/redshift/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5348 2024-04-04 09:10:17.000000 pysqlsync-0.6.0/pysqlsync/dialect/redshift/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      303 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/dialect/redshift/data_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      211 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/dialect/redshift/dependency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      592 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/dialect/redshift/engine.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3498 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/redshift/generator.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.076052 pysqlsync-0.6.0/pysqlsync/dialect/test/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-12-05 20:17:49.000000 pysqlsync-0.6.0/pysqlsync/dialect/test/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      260 2023-12-05 20:17:49.000000 pysqlsync-0.6.0/pysqlsync/dialect/test/dependency.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.080568 pysqlsync-0.6.0/pysqlsync/dialect/trino/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-17 09:48:43.000000 pysqlsync-0.6.0/pysqlsync/dialect/trino/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2759 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/dialect/trino/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      218 2023-12-05 20:17:49.000000 pysqlsync-0.6.0/pysqlsync/dialect/trino/dependency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      698 2023-10-24 19:28:46.000000 pysqlsync-0.6.0/pysqlsync/dialect/trino/discovery.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      552 2023-10-21 22:26:33.000000 pysqlsync-0.6.0/pysqlsync/dialect/trino/engine.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1096 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/dialect/trino/generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5170 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/factory.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.087608 pysqlsync-0.6.0/pysqlsync/formation/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-01 17:58:22.000000 pysqlsync-0.6.0/pysqlsync/formation/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2456 2024-03-07 14:04:30.000000 pysqlsync-0.6.0/pysqlsync/formation/constraints.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7494 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/pysqlsync/formation/data_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    16739 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/formation/discovery.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5046 2023-12-09 10:29:59.000000 pysqlsync-0.6.0/pysqlsync/formation/inspection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13407 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/formation/mutation.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2564 2023-12-09 10:29:59.000000 pysqlsync-0.6.0/pysqlsync/formation/object_dict.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    26462 2024-04-04 09:18:07.000000 pysqlsync-0.6.0/pysqlsync/formation/object_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    43219 2024-04-04 09:12:40.000000 pysqlsync-0.6.0/pysqlsync/formation/py_to_sql.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7038 2024-03-07 14:04:30.000000 pysqlsync-0.6.0/pysqlsync/formation/sql_to_py.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.091128 pysqlsync-0.6.0/pysqlsync/model/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-03 22:18:33.000000 pysqlsync-0.6.0/pysqlsync/model/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    10394 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/pysqlsync/model/data_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2253 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/model/entity_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4273 2024-03-07 14:04:30.000000 pysqlsync-0.6.0/pysqlsync/model/id_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      739 2023-12-15 15:04:38.000000 pysqlsync-0.6.0/pysqlsync/model/key_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7348 2024-03-21 10:46:24.000000 pysqlsync-0.6.0/pysqlsync/model/properties.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-09-16 08:19:48.000000 pysqlsync-0.6.0/pysqlsync/py.typed
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6393 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/pysqlsync/python_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3555 2024-04-04 09:17:25.000000 pysqlsync-0.6.0/pysqlsync/resultset.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.092685 pysqlsync-0.6.0/pysqlsync/util/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-10-25 19:55:04.000000 pysqlsync-0.6.0/pysqlsync/util/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      932 2023-11-12 15:30:43.000000 pysqlsync-0.6.0/pysqlsync/util/dispatch.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      478 2023-11-14 21:10:43.000000 pysqlsync-0.6.0/pysqlsync/util/typing.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.104601 pysqlsync-0.6.0/pysqlsync.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    12929 2024-04-04 09:19:36.000000 pysqlsync-0.6.0/pysqlsync.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3457 2024-04-04 09:19:36.000000 pysqlsync-0.6.0/pysqlsync.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-04-04 09:19:36.000000 pysqlsync-0.6.0/pysqlsync.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      228 2024-04-04 09:19:36.000000 pysqlsync-0.6.0/pysqlsync.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       10 2024-04-04 09:19:36.000000 pysqlsync-0.6.0/pysqlsync.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2024-04-04 09:19:35.000000 pysqlsync-0.6.0/pysqlsync.egg-info/zip-safe
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1458 2024-04-04 09:19:36.107884 pysqlsync-0.6.0/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      257 2023-10-24 18:23:35.000000 pysqlsync-0.6.0/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.101030 pysqlsync-0.6.0/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-01-19 19:01:00.000000 pysqlsync-0.6.0/tests/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3406 2023-12-09 10:29:59.000000 pysqlsync-0.6.0/tests/example.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1201 2023-11-14 21:21:57.000000 pysqlsync-0.6.0/tests/measure.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2024-04-04 09:19:36.104009 pysqlsync-0.6.0/tests/model/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-10-29 17:20:40.000000 pysqlsync-0.6.0/tests/model/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1321 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/tests/model/country.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1686 2023-11-30 20:29:28.000000 pysqlsync-0.6.0/tests/model/event.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      553 2023-10-29 17:25:49.000000 pysqlsync-0.6.0/tests/model/school.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      397 2024-03-02 21:32:04.000000 pysqlsync-0.6.0/tests/model/user.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3429 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/tests/params.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4390 2024-03-17 10:05:18.000000 pysqlsync-0.6.0/tests/tables.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1353 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/tests/test_api.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8307 2024-01-09 17:26:59.000000 pysqlsync-0.6.0/tests/test_connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    17937 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/tests/test_converter.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4892 2024-03-07 14:04:30.000000 pysqlsync-0.6.0/tests/test_discovery.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2749 2023-11-17 20:44:25.000000 pysqlsync-0.6.0/tests/test_exchange.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    33344 2024-03-22 08:53:21.000000 pysqlsync-0.6.0/tests/test_generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3281 2023-12-13 15:01:43.000000 pysqlsync-0.6.0/tests/test_performance.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13647 2024-03-07 19:59:13.000000 pysqlsync-0.6.0/tests/test_synchronize.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2973 2023-12-21 09:21:09.000000 pysqlsync-0.6.0/tests/test_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      352 2023-02-26 20:14:36.000000 pysqlsync-0.6.0/tests/timed_test.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1175 2023-12-09 10:29:59.000000 pysqlsync-0.6.0/tests/update_readme.py
```

### Comparing `pysqlsync-0.5.0/LICENSE` & `pysqlsync-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/PKG-INFO` & `pysqlsync-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqlsync
-Version: 0.5.0
+Version: 0.6.0
 Summary: Synchronize schema and large volumes of data
 Home-page: https://github.com/hunyadi/pysqlsync
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pysqlsync-0.5.0/README.md` & `pysqlsync-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/base.py` & `pysqlsync-0.6.0/pysqlsync/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import abc
 import dataclasses
 import json
 import logging
 import types
 from dataclasses import dataclass
 from typing import Any, Callable, Iterable, Optional, Sized, TypeVar, Union, overload
+from urllib.parse import quote
 
 from strong_typing.inspection import DataclassInstance, is_dataclass_type, is_type_enum
 from strong_typing.name import python_type_to_str
 
 from pysqlsync.python_types import dataclass_to_code, module_to_code
 
 from .formation.inspection import get_entity_types
@@ -107,25 +108,27 @@
     """
     Database-agnostic generator options.
 
     :param enum_mode: Conversion mode for enumeration types.
     :param struct_mode: Conversion mode for composite types.
     :param namespaces: Maps Python modules into SQL namespaces (a.k.a. schemas).
     :param foreign_constraints: Whether to create foreign/primary key relationships between tables.
+    :param initialize_tables: Whether to populate special tables (e.g. enumerations) with data.
     :param synchronization: Synchronization options.
     :param skip_annotations: Annotation classes to ignore on table column types.
     """
 
     enum_mode: Optional[EnumMode] = None
     struct_mode: Optional[StructMode] = None
     array_mode: Optional[ArrayMode] = None
     namespaces: dict[types.ModuleType, Optional[str]] = dataclasses.field(
         default_factory=dict
     )
     foreign_constraints: bool = True
+    initialize_tables: bool = False
     synchronization: MutatorOptions = dataclasses.field(default_factory=MutatorOptions)
     skip_annotations: tuple[type, ...] = ()
 
 
 class BaseGenerator(abc.ABC):
     """
     Generates SQL statements for creating or dropping tables, and inserting, updating or deleting data.
@@ -153,20 +156,18 @@
         self.mutator = mutator if mutator is not None else Mutator()
         self.reset()
 
     def reset(self) -> None:
         self.state = Catalog([])
 
     @overload
-    def create(self, *, tables: list[type[DataclassInstance]]) -> Optional[str]:
-        ...
+    def create(self, *, tables: list[type[DataclassInstance]]) -> Optional[str]: ...
 
     @overload
-    def create(self, *, modules: list[types.ModuleType]) -> Optional[str]:
-        ...
+    def create(self, *, modules: list[types.ModuleType]) -> Optional[str]: ...
 
     def create(
         self,
         *,
         tables: Optional[list[type[DataclassInstance]]] = None,
         modules: Optional[list[types.ModuleType]] = None,
     ) -> Optional[str]:
@@ -465,16 +466,16 @@
     username: Optional[str] = None
     password: Optional[str] = None
     database: Optional[str] = None
 
     def __str__(self) -> str:
         host = self.host or "localhost"
         port = f":{self.port}" if self.port else ""
-        username = f"{self.username}@" if self.username else ""
-        database = f"/{self.database}" if self.database else ""
+        username = f"{quote(self.username, safe='')}@" if self.username else ""
+        database = f"/{quote(self.database, safe='')}" if self.database else ""
         return f"{username}{host}{port}{database}"
 
 
 class BaseConnection(abc.ABC):
     "An active connection to a database."
 
     generator: BaseGenerator
@@ -496,20 +497,18 @@
         exc_type: Optional[type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[types.TracebackType],
     ) -> None:
         await self.close()
 
     @abc.abstractmethod
-    async def open(self) -> "BaseContext":
-        ...
+    async def open(self) -> "BaseContext": ...
 
     @abc.abstractmethod
-    async def close(self) -> None:
-        ...
+    async def close(self) -> None: ...
 
 
 class BaseContext(abc.ABC):
     "Context object returned by a connection object."
 
     connection: BaseConnection
 
@@ -624,20 +623,18 @@
         if stmt:
             await self.execute(stmt)
 
     def get_table_id(self, ref: ClassRef) -> SupportsQualifiedId:
         return self.connection.generator.get_qualified_id(ref)
 
     @overload
-    def get_table(self, __ref: ClassRef) -> Table:
-        ...
+    def get_table(self, __ref: ClassRef) -> Table: ...
 
     @overload
-    def get_table(self, __table: type[DataclassInstance]) -> Table:
-        ...
+    def get_table(self, __table: type[DataclassInstance]) -> Table: ...
 
     def get_table(
         self, __table_or_ref: Union[ClassRef, type[DataclassInstance]]
     ) -> Table:
         if isinstance(__table_or_ref, ClassRef):
             table_id = self.get_table_id(__table_or_ref)
         elif is_dataclass_type(__table_or_ref):
@@ -1045,48 +1042,42 @@
 
     def get_qualified_id(
         self, namespace: Optional[str], id: str
     ) -> SupportsQualifiedId:
         return QualifiedId(namespace, id)
 
     @abc.abstractmethod
-    async def get_table_names(self) -> list[QualifiedId]:
-        ...
+    async def get_table_names(self) -> list[QualifiedId]: ...
 
     @abc.abstractmethod
-    async def has_table(self, table_id: SupportsQualifiedId) -> bool:
-        ...
+    async def has_table(self, table_id: SupportsQualifiedId) -> bool: ...
 
     @abc.abstractmethod
     async def has_column(
         self, table_id: SupportsQualifiedId, column_id: LocalId
-    ) -> bool:
-        ...
+    ) -> bool: ...
 
     @abc.abstractmethod
-    async def get_table(self, table_id: SupportsQualifiedId) -> Table:
-        ...
+    async def get_table(self, table_id: SupportsQualifiedId) -> Table: ...
 
     @abc.abstractmethod
     async def get_namespace(self, namespace_id: LocalId) -> Namespace:
         "Constructs a database object model of a namespace (database schema)."
         ...
 
     @abc.abstractmethod
     async def get_namespace_current(self) -> Namespace:
         "Constructs a database object model of the current namespace (database schema)."
         ...
 
     @overload
-    async def discover(self, *, module: types.ModuleType) -> None:
-        ...
+    async def discover(self, *, module: types.ModuleType) -> None: ...
 
     @overload
-    async def discover(self, *, modules: list[types.ModuleType]) -> None:
-        ...
+    async def discover(self, *, modules: list[types.ModuleType]) -> None: ...
 
     async def discover(
         self,
         *,
         module: Optional[types.ModuleType] = None,
         modules: Optional[list[types.ModuleType]] = None,
     ) -> None:
@@ -1120,20 +1111,18 @@
         for ns in generator.state.namespaces.values():
             LOGGER.debug(f"found {len(ns.enums)} enum(s) in namespace {ns.name}")
             LOGGER.debug(f"found {len(ns.structs)} struct(s) in namespace {ns.name}")
             LOGGER.debug(f"found {len(ns.tables)} table(s) in namespace {ns.name}")
         LOGGER.debug(f"discovered state:\n{str(generator.state)}")
 
     @overload
-    async def synchronize(self, *, module: types.ModuleType) -> None:
-        ...
+    async def synchronize(self, *, module: types.ModuleType) -> None: ...
 
     @overload
-    async def synchronize(self, *, modules: list[types.ModuleType]) -> None:
-        ...
+    async def synchronize(self, *, modules: list[types.ModuleType]) -> None: ...
 
     async def synchronize(
         self,
         *,
         module: Optional[types.ModuleType] = None,
         modules: Optional[list[types.ModuleType]] = None,
     ) -> None:
@@ -1173,28 +1162,24 @@
             generator.state = target_state
 
 
 class BaseEngine(abc.ABC):
     "Represents a specific database server type."
 
     @abc.abstractproperty
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
     @abc.abstractmethod
-    def get_generator_type(self) -> type[BaseGenerator]:
-        ...
+    def get_generator_type(self) -> type[BaseGenerator]: ...
 
     @abc.abstractmethod
-    def get_connection_type(self) -> type[BaseConnection]:
-        ...
+    def get_connection_type(self) -> type[BaseConnection]: ...
 
     @abc.abstractmethod
-    def get_explorer_type(self) -> type[Explorer]:
-        ...
+    def get_explorer_type(self) -> type[Explorer]: ...
 
     def create_connection(
         self, params: ConnectionParameters, options: Optional[GeneratorOptions] = None
     ) -> BaseConnection:
         "Opens a connection to a database server."
 
         generator_options = options if options is not None else GeneratorOptions()
```

### Comparing `pysqlsync-0.5.0/pysqlsync/data/exchange.py` & `pysqlsync-0.6.0/pysqlsync/data/exchange.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/data/generator.py` & `pysqlsync-0.6.0/pysqlsync/data/generator.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mssql/connection.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mssql/connection.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mssql/data_types.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mssql/data_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mssql/discovery.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mssql/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mssql/engine.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mssql/engine.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mssql/generator.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mssql/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         self.converter = DataclassConverter(
             options=DataclassConverterOptions(
                 enum_mode=options.enum_mode or EnumMode.RELATION,
                 struct_mode=options.struct_mode or StructMode.JSON,
                 array_mode=options.array_mode or ArrayMode.JSON,
                 namespaces=NamespaceMapping(options.namespaces),
                 foreign_constraints=options.foreign_constraints,
+                initialize_tables=options.initialize_tables,
                 substitutions={
                     bool: MSSQLBooleanType(),
                     datetime.datetime: MSSQLDateTimeType(),
                     str: MSSQLVariableCharacterType(),
                     uuid.UUID: SqlFixedBinaryType(16),
                     JsonType: MSSQLVariableCharacterType(),
                     ipaddress.IPv4Address: SqlFixedBinaryType(4),
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mssql/mutation.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mssql/mutation.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mssql/object_types.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mssql/object_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 from pysqlsync.formation.object_types import (
     Column,
+    EnumTable,
     Namespace,
     ObjectFactory,
     Table,
     join_or_none,
 )
 from pysqlsync.model.data_types import quote
 from pysqlsync.model.id_types import LocalId
@@ -66,14 +67,18 @@
                 + ",\n".join(f"CONSTRAINT {c.name}" for c in self.table_constraints)
                 + "\n;"
             )
 
         return join_or_none(statements)
 
 
+class MSSQLEnumTable(EnumTable, MSSQLTable):
+    pass
+
+
 class MSSQLNamespace(Namespace):
     def create_schema_stmt(self) -> Optional[str]:
         if self.name.local_id:
             # Microsoft SQL Server requires a separate batch for creating a schema
             return f"IF NOT EXISTS ( SELECT * FROM sys.schemas WHERE name = N{quote(self.name.id)} ) EXEC('CREATE SCHEMA {self.name}');"
         else:
             return None
@@ -85,9 +90,13 @@
         return MSSQLColumn
 
     @property
     def table_class(self) -> type[Table]:
         return MSSQLTable
 
     @property
+    def enum_table_class(self) -> type[EnumTable]:
+        return MSSQLEnumTable
+
+    @property
     def namespace_class(self) -> type[Namespace]:
         return MSSQLNamespace
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mysql/connection.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mysql/connection.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mysql/data_types.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mysql/data_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mysql/discovery.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mysql/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mysql/engine.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mysql/engine.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mysql/generator.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mysql/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
             options=DataclassConverterOptions(
                 enum_mode=options.enum_mode or EnumMode.INLINE,
                 struct_mode=options.struct_mode or StructMode.JSON,
                 array_mode=options.array_mode or ArrayMode.JSON,
                 qualified_names=False,
                 namespaces=NamespaceMapping(options.namespaces),
                 foreign_constraints=options.foreign_constraints,
+                initialize_tables=options.initialize_tables,
                 substitutions={
                     bool: SqlIntegerType(1),
                     datetime.datetime: MySQLDateTimeType(),
                     uuid.UUID: SqlFixedBinaryType(16),
                     str: MySQLVariableCharacterType(16777215),
                     ipaddress.IPv4Address: SqlFixedBinaryType(4),
                     ipaddress.IPv6Address: SqlFixedBinaryType(16),
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mysql/mutation.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mysql/mutation.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/mysql/object_types.py` & `pysqlsync-0.6.0/pysqlsync/dialect/mysql/object_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from dataclasses import dataclass
 from typing import Optional
 
 from pysqlsync.formation.object_types import (
     Column,
+    EnumTable,
     FormationError,
     ObjectFactory,
     Table,
+    identifier,
 )
 from pysqlsync.model.data_types import SqlEnumType, quote
 
 
 class MySQLTable(Table):
     @property
     def short_description(self) -> Optional[str]:
@@ -34,14 +36,18 @@
             f"\nCOMMENT = {quote(self.short_description)}"
             if self.short_description
             else ""
         )
         return f"CREATE TABLE {self.name} (\n{definition}\n){comment};"
 
 
+class MySQLEnumTable(EnumTable, MySQLTable):
+    pass
+
+
 @dataclass(eq=True)
 class MySQLColumn(Column):
     @property
     def data_spec(self) -> str:
         charset = (
             " CHARACTER SET ascii COLLATE ascii_bin"
             if isinstance(self.data_type, SqlEnumType)
@@ -67,16 +73,23 @@
                     f"comment for column {self.name} too long, expected: maximum 1024; got: {len(description)}"
                 )
 
             return quote(description)
         else:
             return None
 
+    def rename_stmt(self, name: str) -> str:
+        return f"CHANGE {self.name} {identifier(name)} {self.data_spec}"
+
 
 class MySQLObjectFactory(ObjectFactory):
     @property
     def column_class(self) -> type[Column]:
         return MySQLColumn
 
     @property
     def table_class(self) -> type[Table]:
         return MySQLTable
+
+    @property
+    def enum_table_class(self) -> type[EnumTable]:
+        return MySQLEnumTable
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/oracle/connection.py` & `pysqlsync-0.6.0/pysqlsync/dialect/oracle/connection.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/oracle/data_types.py` & `pysqlsync-0.6.0/pysqlsync/dialect/oracle/data_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/oracle/discovery.py` & `pysqlsync-0.6.0/pysqlsync/dialect/oracle/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/oracle/engine.py` & `pysqlsync-0.6.0/pysqlsync/dialect/oracle/engine.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/oracle/generator.py` & `pysqlsync-0.6.0/pysqlsync/dialect/oracle/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             options=DataclassConverterOptions(
                 enum_mode=options.enum_mode or EnumMode.RELATION,
                 struct_mode=options.struct_mode or StructMode.JSON,
                 array_mode=options.array_mode or ArrayMode.JSON,
                 qualified_names=False,
                 namespaces=NamespaceMapping(options.namespaces),
                 foreign_constraints=options.foreign_constraints,
+                initialize_tables=options.initialize_tables,
                 substitutions={
                     bytes: OracleVariableBinaryType(),
                     datetime.time: OracleTimeType(),
                     datetime.datetime: OracleTimestampType(),
                     int: OracleIntegerType(),
                     int8: OracleIntegerType(),
                     int16: OracleIntegerType(),
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/oracle/mutation.py` & `pysqlsync-0.6.0/pysqlsync/dialect/oracle/mutation.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/oracle/object_types.py` & `pysqlsync-0.6.0/pysqlsync/dialect/oracle/object_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from pysqlsync.formation.object_types import Column, ObjectFactory, Table
+from pysqlsync.formation.object_types import Column, EnumTable, ObjectFactory, Table
 from pysqlsync.model.data_types import SqlTimestampType
 
 
 class OracleColumn(Column):
     @property
     def default_expr(self) -> str:
         if self.default is None:
@@ -39,15 +39,23 @@
             "BEGIN\n"
             f"    EXECUTE IMMEDIATE 'DROP TABLE {self.name} CASCADE CONSTRAINTS PURGE';\n"
             "EXCEPTION WHEN OTHERS THEN IF SQLCODE != -942 THEN RAISE; END IF;\n"
             "END;"
         )
 
 
+class OracleEnumTable(EnumTable, OracleTable):
+    pass
+
+
 class OracleObjectFactory(ObjectFactory):
     @property
     def column_class(self) -> type[Column]:
         return OracleColumn
 
     @property
     def table_class(self) -> type[Table]:
         return OracleTable
+
+    @property
+    def enum_table_class(self) -> type[EnumTable]:
+        return OracleEnumTable
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/postgresql/connection.py` & `pysqlsync-0.6.0/pysqlsync/dialect/postgresql/connection.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/postgresql/discovery.py` & `pysqlsync-0.6.0/pysqlsync/dialect/postgresql/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/postgresql/engine.py` & `pysqlsync-0.6.0/pysqlsync/dialect/postgresql/engine.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/postgresql/generator.py` & `pysqlsync-0.6.0/pysqlsync/dialect/postgresql/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
             options=DataclassConverterOptions(
                 enum_mode=options.enum_mode or EnumMode.TYPE,
                 struct_mode=options.struct_mode or StructMode.TYPE,
                 array_mode=options.array_mode or ArrayMode.ARRAY,
                 unique_constraint_names=False,
                 namespaces=NamespaceMapping(options.namespaces),
                 foreign_constraints=options.foreign_constraints,
+                initialize_tables=options.initialize_tables,
                 substitutions={
                     JsonType: PostgreSQLJsonType(),
                 },
                 skip_annotations=options.skip_annotations,
                 factory=self.factory,
             )
         )
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/postgresql/mutation.py` & `pysqlsync-0.6.0/pysqlsync/dialect/postgresql/mutation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 from typing import Optional
 
 from pysqlsync.formation.mutation import Mutator
 from pysqlsync.formation.object_types import (
     Column,
+    EnumType,
     StatementList,
     StructType,
     Table,
     deleted,
     join_or_none,
 )
+from pysqlsync.model.data_types import quote
 from pysqlsync.model.id_types import LocalId
 
 from .object_types import sql_quoted_string
 
 
 class PostgreSQLMutator(Mutator):
+    def migrate_enum_stmt(self, enum_type: EnumType, table: Table) -> Optional[str]:
+        enum_values = ", ".join(f"({quote(v)})" for v in enum_type.values)
+        return f'INSERT INTO {table.name} ("value") VALUES {enum_values} ON CONFLICT ("value") DO NOTHING;'
+
     def migrate_column_stmt(
         self, source_table: Table, source: Column, target_table: Table, target: Column
     ) -> Optional[str]:
         ref = target_table.get_constraint(target.name)
         return (
             f"UPDATE {source_table.name} data_table\n"
             f'SET {target.name} = enum_table."id"\n'
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/postgresql/object_types.py` & `pysqlsync-0.6.0/pysqlsync/dialect/postgresql/object_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import re
 from typing import Optional
 
-from pysqlsync.formation.object_types import Namespace, ObjectFactory, StructType, Table
+from pysqlsync.formation.object_types import (
+    EnumTable,
+    Namespace,
+    ObjectFactory,
+    StructType,
+    Table,
+)
 from pysqlsync.model.id_types import LocalId
 
 _sql_quoted_str_table = str.maketrans(
     {
         "\\": "\\\\",
         "'": "\\'",
         "\b": "\\b",
@@ -44,14 +50,18 @@
         return "\n".join(statements)
 
     @property
     def primary_key_constraint_id(self) -> LocalId:
         return LocalId(f"pk_{self.name.local_id.replace('.', '_')}")
 
 
+class PostgreSQLEnumTable(EnumTable, PostgreSQLTable):
+    pass
+
+
 class PostgreSQLStructType(StructType):
     def create_stmt(self) -> str:
         statements: list[str] = []
         statements.append(super().create_stmt())
 
         if self.description is not None:
             statements.append(
@@ -81,13 +91,17 @@
 
 class PostgreSQLObjectFactory(ObjectFactory):
     @property
     def table_class(self) -> type[Table]:
         return PostgreSQLTable
 
     @property
+    def enum_table_class(self) -> type[EnumTable]:
+        return PostgreSQLEnumTable
+
+    @property
     def struct_class(self) -> type[StructType]:
         return PostgreSQLStructType
 
     @property
     def namespace_class(self) -> type[Namespace]:
         return PostgreSQLNamespace
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/redshift/connection.py` & `pysqlsync-0.6.0/pysqlsync/dialect/redshift/connection.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/redshift/engine.py` & `pysqlsync-0.6.0/pysqlsync/dialect/redshift/engine.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/redshift/generator.py` & `pysqlsync-0.6.0/pysqlsync/dialect/redshift/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         self.converter = DataclassConverter(
             options=DataclassConverterOptions(
                 enum_mode=options.enum_mode or EnumMode.RELATION,
                 struct_mode=options.struct_mode or StructMode.JSON,
                 array_mode=options.array_mode or ArrayMode.JSON,
                 namespaces=NamespaceMapping(options.namespaces),
                 foreign_constraints=False,
+                initialize_tables=options.initialize_tables,
                 substitutions={
                     uuid.UUID: RedshiftVariableBinaryType(16),
                     JsonType: SqlVariableCharacterType(),
                     ipaddress.IPv4Address: RedshiftVariableBinaryType(4),
                     ipaddress.IPv6Address: RedshiftVariableBinaryType(16),
                 },
                 skip_annotations=options.skip_annotations,
```

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/trino/connection.py` & `pysqlsync-0.6.0/pysqlsync/dialect/trino/connection.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/trino/discovery.py` & `pysqlsync-0.6.0/pysqlsync/dialect/trino/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/trino/engine.py` & `pysqlsync-0.6.0/pysqlsync/dialect/trino/engine.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/dialect/trino/generator.py` & `pysqlsync-0.6.0/pysqlsync/dialect/trino/generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         self.converter = DataclassConverter(
             options=DataclassConverterOptions(
                 enum_mode=options.enum_mode or EnumMode.CHECK,
                 struct_mode=options.struct_mode or StructMode.JSON,
                 array_mode=options.array_mode or ArrayMode.JSON,
                 namespaces=NamespaceMapping(options.namespaces),
                 foreign_constraints=options.foreign_constraints,
+                initialize_tables=options.initialize_tables,
                 skip_annotations=options.skip_annotations,
             )
         )
 
     @override
     def placeholder(self, index: int) -> str:
         raise NotImplementedError("operation not supported for Trino")
```

### Comparing `pysqlsync-0.5.0/pysqlsync/factory.py` & `pysqlsync-0.6.0/pysqlsync/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import importlib
 import importlib.resources
 import logging
 import re
 import typing
-from urllib.parse import urlparse
+from urllib.parse import unquote, urlparse
 
 from strong_typing.inspection import get_module_classes
 
 from .base import (
     BaseConnection,
     BaseEngine,
     BaseGenerator,
@@ -62,20 +62,38 @@
     except KeyError:
         raise ValueError(f"unrecognized dialect: {engine_name}")
     else:
         return engine_factory
 
 
 def get_parameters(url: str) -> tuple[str, ConnectionParameters]:
-    parts = urlparse(url)
+    """
+    Extracts dialect and connection parameters from a connection string URL.
+
+    The connection string URL has the following structure:
+    ```
+    dialect://username:password@hostname:port/database
+    ```
+
+    For example,
+    ```
+    postgresql://root:%3C%3FYour%3AStrong%40Pass%2Fw0rd%3E@server.example.com:5432/public
+    ```
+
+    In the example above, dialect is `postgresql`, username is `root`, password is `<?Your:Strong@Pass/w0rd>`,
+    hostname is `server.example.com`, port is `5432` and the database name is `public`. Note how components are
+    URL-encoded (a.k.a. percent-encoded) to comply with RFC 3986.
+    """
+
+    parts = urlparse(url, allow_fragments=False)
     return parts.scheme, ConnectionParameters(
         host=parts.hostname,
         port=parts.port,
-        username=parts.username,
-        password=parts.password,
+        username=unquote(parts.username) if parts.username else None,
+        password=unquote(parts.password) if parts.password else None,
         database=parts.path.lstrip("/") if parts.path else None,
     )
 
 
 class UnavailableEngine(BaseEngine):
     _name: str
     _module: str
```

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/constraints.py` & `pysqlsync-0.6.0/pysqlsync/formation/constraints.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/data_types.py` & `pysqlsync-0.6.0/pysqlsync/formation/data_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/discovery.py` & `pysqlsync-0.6.0/pysqlsync/formation/discovery.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/inspection.py` & `pysqlsync-0.6.0/pysqlsync/formation/inspection.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/mutation.py` & `pysqlsync-0.6.0/pysqlsync/formation/mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,18 @@
     def __init__(self, options: Optional[MutatorOptions] = None) -> None:
         self.options = options or MutatorOptions()
 
     def check_identity(self, source: SupportsName, target: SupportsName) -> None:
         if source.name != target.name:
             raise FormationError(f"object mismatch: {source.name} != {target.name}")
 
+    def migrate_enum_stmt(self, enum_type: EnumType, table: Table) -> Optional[str]:
+        enum_values = ", ".join(f"({quote(v)})" for v in enum_type.values)
+        return f'INSERT INTO {table.name} ("value") VALUES {enum_values};'
+
     def mutate_enum_stmt(self, source: EnumType, target: EnumType) -> Optional[str]:
         self.check_identity(source, target)
 
         removed_values = [
             value for value in source.values if value not in target.values
         ]
         if removed_values:
@@ -278,18 +282,15 @@
 
         # populate new objects with data
         for enum_type in enum_drop:
             for table in table_create:
                 if enum_type.name != table.name:
                     continue
 
-                enum_values = ", ".join(f"({quote(v)})" for v in enum_type.values)
-                statements.append(
-                    f'INSERT INTO {table.name} ("value") VALUES {enum_values};'
-                )
+                statements.append(self.migrate_enum_stmt(enum_type, table))
 
         # mutate existing object
         enum_mutate = list(source.enums.intersection(target.enums))
         statements.extend(
             self.mutate_enum_stmt(source_enum, target_enum)
             for source_enum, target_enum in enum_mutate
         )
```

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/object_dict.py` & `pysqlsync-0.6.0/pysqlsync/formation/object_dict.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/object_types.py` & `pysqlsync-0.6.0/pysqlsync/formation/object_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 import copy
 from dataclasses import dataclass
-from typing import Iterable, Optional, overload
+from typing import Any, Iterable, Optional, overload
 
+from strong_typing.inspection import is_dataclass_instance
 from strong_typing.topological import topological_sort
 
 from ..model.data_types import SqlDataType, SqlUserDefinedType, constant
 from ..model.id_types import LocalId, SupportsQualifiedId
 from .object_dict import ObjectDict
 
 
@@ -546,14 +547,54 @@
             return None
 
     @property
     def table_constraints(self) -> list[Constraint]:
         return [c for c in self.constraints.values() if c.is_alter_table()]
 
 
+class EnumTable(Table):
+    values: list[Any]
+
+    def __init__(
+        self,
+        name: SupportsQualifiedId,
+        columns: list[Column],
+        *,
+        values: list[Any],
+        primary_key: tuple[LocalId, ...],
+        constraints: Optional[list[Constraint]] = None,
+        description: Optional[str] = None,
+    ) -> None:
+        super().__init__(
+            name,
+            columns,
+            primary_key=primary_key,
+            constraints=constraints,
+            description=description,
+        )
+        self.values = values
+
+    def create_stmt(self) -> str:
+        statements: list[str] = []
+        statements.append(super().create_stmt())
+        column_list = ", ".join(str(col.name) for col in self.get_value_columns())
+        values: list[str] = []
+        for value in self.values:
+            if isinstance(value, tuple) or is_dataclass_instance(value):
+                values.append(constant(value))
+            else:
+                values.append(f"({constant(value)})")
+        value_list = ", ".join(values)
+
+        statements.append(
+            f"INSERT INTO {self.name} ({column_list}) VALUES {value_list};"
+        )
+        return "\n".join(statements)
+
+
 @dataclass
 class Namespace(DatabaseObject):
     "A namespace that multiple objects can share. Typically corresponds to a database schema."
 
     name: LocalId
     enums: ObjectDict[EnumType]
     structs: ObjectDict[StructType]
@@ -789,14 +830,20 @@
     @property
     def table_class(self) -> type[Table]:
         "The object type instantiated for tables."
 
         return Table
 
     @property
+    def enum_table_class(self) -> type[EnumTable]:
+        "The object type instantiated for tables that store enumeration values."
+
+        return EnumTable
+
+    @property
     def struct_class(self) -> type[StructType]:
         "The object type instantiated for struct types."
 
         return StructType
 
     @property
     def namespace_class(self) -> type[Namespace]:
```

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/py_to_sql.py` & `pysqlsync-0.6.0/pysqlsync/formation/py_to_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import copy
 import dataclasses
 import datetime
 import decimal
 import enum
+import inspect
 import ipaddress
 import sys
 import types
 import typing
 import uuid
-from typing import Annotated, Iterable, Optional, TypeVar
+from typing import Annotated, Callable, Iterable, Optional, TypeVar
 
 from strong_typing.auxiliary import (
     MaxLength,
     float32,
     float64,
     int8,
     int16,
@@ -115,14 +116,22 @@
         raise TypeError(
             f"inconsistent enumeration value types for type {enum_type.__name__}: {value_types}"
         )
     value_type = value_types.pop()
     return value_type if value_type is not str else ENUM_LABEL_TYPE
 
 
+def is_type_enum_list(typ: TypeLike) -> bool:
+    if not is_generic_list(typ):
+        return False
+
+    elem_type = unwrap_generic_list(typ)
+    return is_type_enum(elem_type)
+
+
 def is_extensible_enum_type(typ: TypeLike, cls: type) -> bool:
     """
     True if the type represents an extensible enumeration type.
 
     :param typ: A type to check.
     :param cls: Context in which to evaluate the type (e.g. a class).
     """
@@ -148,20 +157,21 @@
                 return member_type
     raise TypeError(
         "extensible enum types are of the form `E | str` where `E` is a subclass of `enum.Enum`"
     )
 
 
 def dataclass_fields_as_required(
-    cls: type[DataclassInstance],
+    cls: type[DataclassInstance], pred: Optional[Callable[[TypeLike], bool]] = None
 ) -> Iterable[DataclassField]:
     for field in dataclass_fields(cls):
         props = get_field_properties(field.type)
         ref = evaluate_member_type(props.field_type, cls)
-        yield DataclassField(field.name, ref, field.default)
+        if pred is None or pred(ref):
+            yield DataclassField(field.name, ref, field.default)
 
 
 def _topological_sort(class_types: list[type]) -> list[type]:
     """
     Returns a list of types in topological order.
 
     Types that don't depend on other types (i.e. fundamental types) are first. Types on which no other types depend are last.
@@ -175,30 +185,14 @@
 
 @dataclasses.dataclass
 class DataclassEnumField:
     name: str
     type: type[enum.Enum]
 
 
-def dataclass_enum_fields(cls: type[DataclassInstance]) -> Iterable[DataclassEnumField]:
-    for field in dataclass_fields_as_required(cls):
-        if is_type_enum(field.type):
-            yield DataclassEnumField(field.name, field.type)
-
-
-def dataclass_extensible_enum_fields(
-    cls: type[DataclassInstance],
-) -> Iterable[DataclassEnumField]:
-    for field in dataclass_fields_as_required(cls):
-        if is_extensible_enum_type(field.type, cls):
-            yield DataclassEnumField(
-                field.name, unwrap_extensible_enum_type(field.type, cls)
-            )
-
-
 class NamespaceMapping:
     """
     Associates Python modules with SQL namespaces (schemas).
 
     :param dictionary: Maps a Python module to a SQL namespace, or `None` to use the default namespace.
     """
 
@@ -274,27 +268,29 @@
     :param struct_mode: Conversion mode for structure types that are not entities.
     :param array_mode: Conversion mode for array types.
     :param extra_numeric_types: Whether to use extra numeric types like `int1` or `uint4`.
     :param qualified_names: Whether to use fully qualified names (True) or string-prefixed names (False).
     :param unique_constraint_names: Whether to generate constraint names that are globally unique.
     :param namespaces: Maps Python modules to SQL namespaces (schemas).
     :param foreign_constraints: Whether to create foreign/primary key relationships between tables.
+    :param initialize_tables: Whether to populate special tables (e.g. enumerations) with data.
     :param substitutions: SQL type to be substituted for a specific Python type.
     :param factory: Creates new column, table, struct and namespace instances.
     :param skip_annotations: Annotation classes to ignore on table column types.
     """
 
     enum_mode: EnumMode = EnumMode.TYPE
     struct_mode: StructMode = StructMode.TYPE
     array_mode: ArrayMode = ArrayMode.ARRAY
     extra_numeric_types: bool = False
     qualified_names: bool = True
     unique_constraint_names: bool = True
     namespaces: NamespaceMapping = dataclasses.field(default_factory=NamespaceMapping)
     foreign_constraints: bool = True
+    initialize_tables: bool = False
     substitutions: dict[TypeLike, SqlDataType] = dataclasses.field(default_factory=dict)
     factory: ObjectFactory = dataclasses.field(default_factory=ObjectFactory)
     skip_annotations: tuple[type, ...] = ()
 
 
 class DataclassConverter:
     options: DataclassConverterOptions
@@ -404,14 +400,16 @@
 
         metadata = getattr(typ, "__metadata__", None)
         if metadata:
             unadorned_type = unwrap_annotated_type(typ)
             substitute = self.options.substitutions.get(unadorned_type)
             if substitute is not None:
                 sql_type = copy.copy(substitute)
+            elif unadorned_type is int:
+                sql_type = SqlIntegerType(8)
             elif unadorned_type is str:
                 sql_type = SqlVariableCharacterType()
             elif unadorned_type is float:
                 sql_type = SqlFloatType()
             elif unadorned_type is decimal.Decimal:
                 sql_type = SqlDecimalType()
             elif unadorned_type is datetime.datetime:
@@ -432,25 +430,36 @@
             if sql_type:
                 return sql_type
 
             typ = unadorned_type
 
         if is_type_enum(typ):
             value_type = enum_value_type(typ)
+            unadorned_value_type = unwrap_annotated_type(value_type)
 
-            if self.options.enum_mode is EnumMode.TYPE:
-                return SqlUserDefinedType(
-                    self.create_qualified_id(typ.__module__, typ.__name__)
-                )
-            elif self.options.enum_mode is EnumMode.INLINE:
-                return SqlEnumType([str(e.value) for e in typ])
-            elif self.options.enum_mode is EnumMode.RELATION:
-                return self._enumeration_key_type()
-            elif self.options.enum_mode is EnumMode.CHECK:
-                return self.simple_type_to_sql_data_type(value_type)
+            if unadorned_value_type is int or unadorned_value_type is str:
+                if self.options.enum_mode is EnumMode.TYPE:
+                    return SqlUserDefinedType(
+                        self.create_qualified_id(typ.__module__, typ.__name__)
+                    )
+                elif self.options.enum_mode is EnumMode.INLINE:
+                    return SqlEnumType([str(e.value) for e in typ])
+                elif self.options.enum_mode is EnumMode.RELATION:
+                    return self._enumeration_key_type()
+                elif self.options.enum_mode is EnumMode.CHECK:
+                    return self.simple_type_to_sql_data_type(value_type)
+                else:
+                    raise NotImplementedError(f"match not exhaustive: {EnumMode}")
+            else:
+                if self.options.enum_mode is EnumMode.RELATION:
+                    return self._enumeration_key_type()
+                else:
+                    raise TypeError(
+                        f"enumeration mode {self.options.enum_mode} not valid for complex member types in enumeration `{typ.__name__}`"
+                    )
 
         raise TypeError(f"not a simple type: {typ}")
 
     def _enumeration_key_type(self) -> SqlDataType:
         "Key type for storing enumeration values in a dedicated table."
 
         return self.simple_type_to_sql_data_type(int32)
@@ -624,62 +633,88 @@
 
         # foreign/primary key constraints
         constraints = []
         if self.options.foreign_constraints:
             constraints.extend(self.dataclass_to_constraints(cls))
 
         # relationships for extensible enumeration types ignore foreign constraints option and always create a foreign key
-        for enum_field in dataclass_extensible_enum_fields(cls):
+        for enum_field in dataclass_fields_as_required(
+            cls, lambda t: is_extensible_enum_type(t, cls)
+        ):
+            enum_type = unwrap_extensible_enum_type(enum_field.type, cls)
             constraints.append(
                 ForeignConstraint(
                     LocalId(self.create_foreign_key_name(cls, enum_field.name)),
                     (LocalId(enum_field.name),),
                     ConstraintReference(
                         self.create_qualified_id(
-                            enum_field.type.__module__, enum_field.type.__name__
+                            enum_type.__module__, enum_type.__name__
                         ),
                         (LocalId("id"),),
                     ),
                 ),
             )
 
         # relationships for enumeration types ignore foreign constraints option and always create a foreign key
         if self.options.enum_mode is EnumMode.RELATION:
-            for enum_field in dataclass_enum_fields(cls):
+            for enum_field in dataclass_fields_as_required(cls, is_type_enum):
                 constraints.append(
                     ForeignConstraint(
                         LocalId(self.create_foreign_key_name(cls, enum_field.name)),
                         (LocalId(enum_field.name),),
                         ConstraintReference(
                             self.create_qualified_id(
                                 enum_field.type.__module__, enum_field.type.__name__
                             ),
                             (LocalId("id"),),
                         ),
                     ),
                 )
 
         if self.options.enum_mode is EnumMode.CHECK:
-            for enum_field in dataclass_enum_fields(cls):
+            for enum_field in dataclass_fields_as_required(cls, is_type_enum):
                 enum_values = ", ".join(constant(e.value) for e in enum_field.type)
                 constraints.append(
                     CheckConstraint(
                         LocalId(self.create_check_name(cls, enum_field.name)),
                         f"{LocalId(enum_field.name)} IN ({enum_values})",
                     ),
                 )
 
+        for column in columns:
+            check_constraint = self.create_check_constraint(column)
+            if check_constraint:
+                constraints.append(
+                    CheckConstraint(
+                        LocalId(self.create_check_name(cls, column.name.id)),
+                        check_constraint,
+                    ),
+                )
+
         return self.options.factory.table_class(
             name=self.create_qualified_id(cls.__module__, cls.__name__),
             columns=columns,
             primary_key=(LocalId(dataclass_primary_key_name(cls)),),
             constraints=constraints or None,
             description=doc.full_description,
         )
 
+    def create_check_constraint(self, column: Column) -> Optional[str]:
+        conditions: list[str] = []
+        data_type = column.data_type
+        if isinstance(data_type, SqlIntegerType):
+            if data_type.minimum is not None:
+                conditions.append(f"{column.name} >= {data_type.minimum}")
+            if data_type.maximum is not None:
+                conditions.append(f"{column.name} <= {data_type.maximum}")
+        if conditions:
+            return " AND ".join(f"({c})" for c in conditions)
+        else:
+            return None
+
     def dataclass_to_constraints(
         self, cls: type[DataclassInstance]
     ) -> list[Constraint]:
         "Extracts the foreign/primary key relationships from a data-class."
 
         constraints: list[Constraint] = []
 
@@ -772,56 +807,97 @@
             name=self.create_qualified_id(cls.__module__, cls.__name__),
             members=members,
             description=doc.full_description,
         )
 
     def _enum_table(self, enum_type: type[enum.Enum]) -> Table:
         enum_table_name = enum_type.__name__
-        return self.options.factory.table_class(
-            self.create_qualified_id(enum_type.__module__, enum_table_name),
-            [
-                self.options.factory.column_class(
-                    LocalId("id"),
-                    self._enumeration_key_type(),
-                    False,
-                    identity=True,
-                ),
+        id = self.create_qualified_id(enum_type.__module__, enum_table_name)
+        columns = [
+            self.options.factory.column_class(
+                LocalId("id"),
+                self._enumeration_key_type(),
+                False,
+                identity=True,
+            )
+        ]
+        primary_key = (LocalId("id"),)
+        constraints: list[Constraint] = []
+
+        enum_member_types: set[type] = set(type(e.value) for e in enum_type)
+        if len(enum_member_types) > 1:
+            raise TypeError(
+                f"inconsistent member types in enumeration `{enum_type.__name__}`: {sorted(list(e.__name__ for e in enum_member_types))}"
+            )
+        enum_member_type = enum_member_types.pop()
+        unadorned_member_type = unwrap_annotated_type(enum_member_type)
+
+        if unadorned_member_type is int or unadorned_member_type is str:
+            columns.append(
                 self.options.factory.column_class(
                     LocalId("value"),
                     self.member_to_sql_data_type(ENUM_LABEL_TYPE, type(None)),
                     False,
-                ),
-            ],
-            primary_key=(LocalId("id"),),
-            constraints=[
+                )
+            )
+            constraints.append(
                 UniqueConstraint(
                     LocalId(f"uq_{enum_table_name}"),
                     (LocalId("value"),),
                 )
-            ],
-        )
+            )
+        elif is_dataclass_type(unadorned_member_type):
+            columns.extend(
+                self.member_to_column(
+                    field, enum_member_type, parse_type(unadorned_member_type)
+                )
+                for field in dataclass_fields(unadorned_member_type)
+            )
+        else:
+            raise TypeError(
+                f"unsupported member type in enumeration `{enum_type.__name__}`: {enum_member_type}"
+            )
+
+        if self.options.initialize_tables:
+            return self.options.factory.enum_table_class(
+                id,
+                columns,
+                values=[e.value for e in enum_type],
+                primary_key=primary_key,
+                constraints=constraints,
+            )
+        else:
+            return self.options.factory.table_class(
+                id,
+                columns,
+                primary_key=primary_key,
+                constraints=constraints,
+            )
 
     def dataclasses_to_catalog(
         self, entity_types: list[type[DataclassInstance]]
     ) -> Catalog:
         "Converts a list of Python data-class types into a database object catalog."
 
+        # omit abstract base classes
+        entity_types = [t for t in entity_types if not inspect.isabstract(t)]
+
         # collect all dependent types
         referenced_types: set[type] = set(entity_types)
         for entity_type in entity_types:
             for ref_type in get_referenced_types(entity_type):
                 referenced_types.add(ref_type)
 
         # collect all enumeration types in alphabetical order
         enums: dict[str, list[EnumType]] = {}
         if self.options.enum_mode is EnumMode.TYPE:
             enum_types = [obj for obj in referenced_types if is_type_enum(obj)]
             enum_types.sort(key=lambda e: e.__name__)
             for enum_type in enum_types:
-                enum_values = [str(e.value) for e in enum_type]
+                enum_values = [str(e.value) for e in enum_type]  # type: ignore
                 if len(enum_values) < 2:
                     # enumerations with too few members expand into extensible enumeration tables
                     continue
 
                 enum_defs = enums.setdefault(enum_type.__module__, [])
                 enum_defs.append(
                     EnumType(
@@ -851,25 +927,32 @@
             table_defs = tables.setdefault(table_type.__module__, [])
             table_defs.append(self.dataclass_to_table(table_type))
 
         # discover regular enumerations
         regular_enum_types: set[type[enum.Enum]] = set()
         if self.options.enum_mode is EnumMode.RELATION:
             for entity in table_types:
-                for enum_field in dataclass_enum_fields(entity):
+                for enum_field in dataclass_fields_as_required(entity, is_type_enum):
                     regular_enum_types.add(enum_field.type)
+                for enum_field in dataclass_fields_as_required(
+                    entity, is_type_enum_list
+                ):
+                    regular_enum_types.add(unwrap_generic_list(enum_field.type))
         for enum_type in sorted(list(regular_enum_types), key=lambda e: e.__name__):
             table_defs = tables.setdefault(enum_type.__module__, [])
             table_defs.append(self._enum_table(enum_type))
 
         # discover extensible enumerations
         extensible_enum_types: set[type[enum.Enum]] = set()
         for entity in table_types:
-            for enum_field in dataclass_extensible_enum_fields(entity):
-                extensible_enum_types.add(enum_field.type)
+            for enum_field in dataclass_fields_as_required(
+                entity, lambda t: is_extensible_enum_type(t, entity)
+            ):
+                enum_type = unwrap_extensible_enum_type(enum_field.type, entity)
+                extensible_enum_types.add(enum_type)
         for enum_type in sorted(list(extensible_enum_types), key=lambda e: e.__name__):
             table_defs = tables.setdefault(enum_type.__module__, [])
             table_defs.append(self._enum_table(enum_type))
 
         # create join tables for one-to-many relationships
         for entity in table_types:
             for field in dataclass_fields(entity):
```

### Comparing `pysqlsync-0.5.0/pysqlsync/formation/sql_to_py.py` & `pysqlsync-0.6.0/pysqlsync/formation/sql_to_py.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/model/data_types.py` & `pysqlsync-0.6.0/pysqlsync/model/data_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import datetime
 from dataclasses import dataclass
 from functools import reduce
 from typing import Any, Optional
 
-from strong_typing.auxiliary import MaxLength, Precision, Storage, TimePrecision
+from strong_typing.auxiliary import (
+    IntegerRange,
+    MaxLength,
+    Precision,
+    Signed,
+    Storage,
+    TimePrecision,
+)
+from strong_typing.inspection import dataclass_fields, is_dataclass_instance
 
 from .id_types import SupportsQualifiedId
 
 
 def quote(s: str) -> str:
     "Quotes a string to be embedded in an SQL statement."
 
@@ -22,14 +30,22 @@
     elif isinstance(v, (int, float)):
         return str(v)
     elif isinstance(v, bool):
         return "TRUE" if v else "FALSE"
     elif isinstance(v, datetime.datetime):
         timestamp = v.astimezone(tz=datetime.timezone.utc).replace(tzinfo=None)
         return quote(timestamp.isoformat(sep=" "))
+    elif isinstance(v, tuple):
+        values = ", ".join(constant(value) for value in v)
+        return f"({values})"
+    elif is_dataclass_instance(v):
+        values = ", ".join(
+            constant(getattr(v, field.name)) for field in dataclass_fields(type(v))
+        )
+        return f"({values})"
     else:
         raise NotImplementedError(f"unknown constant representation for value: {v}")
 
 
 def escape_like(value: str, escape_char: str) -> str:
     "Escapes a string to be embedded in an SQL LIKE '...' ESCAPE '...' expression."
 
@@ -68,27 +84,41 @@
     def __str__(self) -> str:
         return "boolean"
 
 
 @dataclass
 class SqlIntegerType(SqlDataType):
     width: int
+    signed: bool = True
+    minimum: Optional[int] = None
+    maximum: Optional[int] = None
 
     def __str__(self) -> str:
         if self.width == 1:
             return "tinyint"
         elif self.width == 2:
             return "smallint"
         elif self.width == 4:
             return "integer"
         elif self.width == 8:
             return "bigint"
 
         raise TypeError(f"invalid integer width: {self.width}")
 
+    def parse_meta(self, meta: Any) -> None:
+        if isinstance(meta, IntegerRange):
+            self.minimum = meta.minimum
+            self.maximum = meta.maximum
+        elif isinstance(meta, Signed):
+            self.signed = meta.is_signed
+        elif isinstance(meta, Storage):
+            self.width = meta.bytes
+        else:
+            super().parse_meta(meta)
+
 
 @dataclass
 class SqlFloatType(SqlDataType):
     """
     Floating-point numeric type.
 
     :param precision: Numeric precision in base 2.
```

### Comparing `pysqlsync-0.5.0/pysqlsync/model/entity_types.py` & `pysqlsync-0.6.0/pysqlsync/model/entity_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/model/id_types.py` & `pysqlsync-0.6.0/pysqlsync/model/id_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/model/key_types.py` & `pysqlsync-0.6.0/pysqlsync/model/key_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/model/properties.py` & `pysqlsync-0.6.0/pysqlsync/model/properties.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/python_types.py` & `pysqlsync-0.6.0/pysqlsync/python_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/resultset.py` & `pysqlsync-0.6.0/pysqlsync/resultset.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync/util/dispatch.py` & `pysqlsync-0.6.0/pysqlsync/util/dispatch.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/pysqlsync.egg-info/PKG-INFO` & `pysqlsync-0.6.0/pysqlsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqlsync
-Version: 0.5.0
+Version: 0.6.0
 Summary: Synchronize schema and large volumes of data
 Home-page: https://github.com/hunyadi/pysqlsync
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pysqlsync-0.5.0/pysqlsync.egg-info/SOURCES.txt` & `pysqlsync-0.6.0/pysqlsync.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -90,22 +90,23 @@
 pysqlsync/util/dispatch.py
 pysqlsync/util/typing.py
 tests/__init__.py
 tests/example.py
 tests/measure.py
 tests/params.py
 tests/tables.py
+tests/test_api.py
 tests/test_connection.py
 tests/test_converter.py
 tests/test_discovery.py
 tests/test_exchange.py
 tests/test_generator.py
-tests/test_import.py
 tests/test_performance.py
 tests/test_synchronize.py
 tests/test_types.py
 tests/timed_test.py
 tests/update_readme.py
 tests/model/__init__.py
+tests/model/country.py
 tests/model/event.py
 tests/model/school.py
 tests/model/user.py
```

### Comparing `pysqlsync-0.5.0/setup.cfg` & `pysqlsync-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/example.py` & `pysqlsync-0.6.0/tests/example.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/measure.py` & `pysqlsync-0.6.0/tests/measure.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/model/event.py` & `pysqlsync-0.6.0/tests/model/event.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/model/school.py` & `pysqlsync-0.6.0/tests/model/school.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/params.py` & `pysqlsync-0.6.0/tests/params.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 
 from pysqlsync.base import BaseEngine, ConnectionParameters
 from pysqlsync.factory import get_dialect
 
 
 class TestEngineBase(abc.ABC):
     @abc.abstractproperty
-    def engine(self) -> BaseEngine:
-        ...
+    def engine(self) -> BaseEngine: ...
 
     @abc.abstractproperty
-    def parameters(self) -> ConnectionParameters:
-        ...
+    def parameters(self) -> ConnectionParameters: ...
 
 
 class OracleBase(TestEngineBase):
     "Base class for testing Oracle features."
 
     @property
     def engine(self) -> BaseEngine:
@@ -26,15 +24,15 @@
 
     @property
     def parameters(self) -> ConnectionParameters:
         return ConnectionParameters(
             host="localhost",
             port=1521,
             username="system",
-            password="<YourStrong@Passw0rd>",
+            password="<?YourStrong@Passw0rd>",
             database="FREEPDB1",
         )
 
 
 class PostgreSQLBase(TestEngineBase):
     "Base class for testing PostgreSQL features."
 
@@ -44,15 +42,15 @@
 
     @property
     def parameters(self) -> ConnectionParameters:
         return ConnectionParameters(
             host="localhost",
             port=5432,
             username="levente.hunyadi",
-            password="<YourStrong@Passw0rd>",
+            password="<?YourStrong@Passw0rd>",
             database="levente.hunyadi",
         )
 
 
 class MSSQLBase(TestEngineBase):
     "Base class for testing Microsoft SQL Server features."
 
@@ -62,15 +60,15 @@
 
     @property
     def parameters(self) -> ConnectionParameters:
         return ConnectionParameters(
             host="127.0.0.1",
             port=None,
             username="SA",
-            password="<YourStrong@Passw0rd>",
+            password="<?YourStrong@Passw0rd>",
             database=None,
         )
 
 
 class MySQLBase(TestEngineBase):
     "Base class for testing MySQL features."
 
@@ -80,15 +78,15 @@
 
     @property
     def parameters(self) -> ConnectionParameters:
         return ConnectionParameters(
             host="localhost",
             port=3306,
             username="root",
-            password="<YourStrong@Passw0rd>",
+            password="<?YourStrong@Passw0rd>",
             database="levente_hunyadi",
         )
 
 
 class RedshiftBase(TestEngineBase):
     "Base class for testing AWS Redshift features."
```

### Comparing `pysqlsync-0.5.0/tests/tables.py` & `pysqlsync-0.6.0/tests/tables.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/test_connection.py` & `pysqlsync-0.6.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/test_converter.py` & `pysqlsync-0.6.0/tests/test_converter.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     SqlUserDefinedType,
     SqlUuidType,
     SqlVariableCharacterType,
 )
 from pysqlsync.model.id_types import LocalId, QualifiedId
 from pysqlsync.python_types import dataclass_to_code, module_to_code
 from tests import tables
-from tests.model import user
+from tests.model import country, user
 
 
 class TestConverter(unittest.TestCase):
     @property
     def options(self) -> DataclassConverterOptions:
         return DataclassConverterOptions(namespaces=NamespaceMapping({tables: None}))
 
@@ -255,14 +255,75 @@
                     reference=ConstraintReference(
                         table=QualifiedId(namespace=None, id=enum_name),
                         columns=(LocalId(id="id"),),
                     ),
                 ),
             ],
         )
+
+    def test_dataclass_enum_relation(self) -> None:
+        options = DataclassConverterOptions(
+            enum_mode=EnumMode.RELATION, namespaces=NamespaceMapping({country: None})
+        )
+        converter = DataclassConverter(options=options)
+        catalog = converter.dataclasses_to_catalog([country.DataclassEnumTable])
+        table_name = country.DataclassEnumTable.__name__
+        table_def = catalog.get_table(QualifiedId(None, table_name))
+        self.assertListEqual(
+            list(table_def.columns.values()),
+            [
+                Column(LocalId("id"), SqlIntegerType(8), False),
+                Column(LocalId("country"), SqlIntegerType(4), False),
+                Column(LocalId("optional_country"), SqlIntegerType(4), True),
+            ],
+        )
+        enum_name = country.CountryEnum.__name__
+        enum_def = catalog.get_table(QualifiedId(None, enum_name))
+        self.assertListEqual(
+            list(enum_def.columns.values()),
+            [
+                Column(
+                    LocalId("id"),
+                    SqlIntegerType(4),
+                    False,
+                    identity=True,
+                ),
+                Column(
+                    LocalId("iso_code"),
+                    SqlVariableCharacterType(),
+                    False,
+                ),
+                Column(
+                    LocalId("name"),
+                    SqlVariableCharacterType(),
+                    False,
+                ),
+            ],
+        )
+        self.assertListEqual(
+            list(table_def.constraints.values()),
+            [
+                ForeignConstraint(
+                    name=LocalId(id=f"fk_{table_name}_country"),
+                    foreign_columns=(LocalId(id="country"),),
+                    reference=ConstraintReference(
+                        table=QualifiedId(namespace=None, id=enum_name),
+                        columns=(LocalId(id="id"),),
+                    ),
+                ),
+                ForeignConstraint(
+                    name=LocalId(id=f"fk_{table_name}_optional_country"),
+                    foreign_columns=(LocalId(id="optional_country"),),
+                    reference=ConstraintReference(
+                        table=QualifiedId(namespace=None, id=enum_name),
+                        columns=(LocalId(id="id"),),
+                    ),
+                ),
+            ],
+        )
 
     def test_literal_type(self) -> None:
         table_def = dataclass_to_table(tables.LiteralTable, options=self.options)
         self.assertListEqual(
             list(table_def.columns.values()),
             [
                 Column(LocalId("id"), SqlIntegerType(8), False),
```

### Comparing `pysqlsync-0.5.0/tests/test_discovery.py` & `pysqlsync-0.6.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/test_exchange.py` & `pysqlsync-0.6.0/tests/test_exchange.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/test_generator.py` & `pysqlsync-0.6.0/tests/test_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ipaddress
 import unittest
 from datetime import date, datetime, time, timedelta, timezone
 
 from strong_typing.inspection import DataclassInstance
 
 from pysqlsync.base import GeneratorOptions
+from pysqlsync.formation.py_to_sql import EnumMode
 from tests import tables
 from tests.params import (
     MSSQLBase,
     MySQLBase,
     OracleBase,
     PostgreSQLBase,
     TestEngineBase,
@@ -24,20 +25,27 @@
     @property
     def options(self) -> GeneratorOptions:
         return GeneratorOptions(namespaces={tables: None})
 
     def assertMatchSQLCreate(
         self, dialect: str, table: type[DataclassInstance], sql: str
     ) -> None:
+        return self.assertMatchSQLCreateOptions(self.options, dialect, table, sql)
+
+    def assertMatchSQLCreateOptions(
+        self,
+        options: GeneratorOptions,
+        dialect: str,
+        table: type[DataclassInstance],
+        sql: str,
+    ) -> None:
         if dialect != self.engine.name:
             return
 
-        statement = (
-            self.engine.create_generator(self.options).create(tables=[table]) or ""
-        )
+        statement = self.engine.create_generator(options).create(tables=[table]) or ""
         self.assertMultiLineEqual(statement, sql)
 
     def assertMatchSQLUpsert(
         self, dialect: str, table: type[DataclassInstance], sql: str
     ) -> None:
         if dialect != self.engine.name:
             return
@@ -287,14 +295,15 @@
             'CONSTRAINT "pk_DefaultDateTimeTable" PRIMARY KEY ("id")\n'
             ");\n"
             """ALTER TABLE "DefaultDateTimeTable" ADD CONSTRAINT "df_iso_date_time" DEFAULT '1989-10-24 23:59:59' FOR "iso_date_time";""",
         )
 
     def test_create_enum_table(self) -> None:
         self.maxDiff = None
+        options = GeneratorOptions(initialize_tables=True, namespaces={tables: None})
         self.assertMatchSQLCreate(
             "postgresql",
             tables.EnumTable,
             """CREATE TYPE "WorkflowState" AS ENUM ('active', 'inactive', 'deleted');\n"""
             'CREATE TABLE "EnumTable" (\n'
             '"id" bigint NOT NULL,\n'
             '"state" "WorkflowState" NOT NULL,\n'
@@ -308,35 +317,104 @@
             'CREATE TABLE "EnumTable" (\n'
             '"id" bigint NOT NULL,\n'
             """"state" ENUM ('active', 'inactive', 'deleted') CHARACTER SET ascii COLLATE ascii_bin NOT NULL,\n"""
             """"optional_state" ENUM ('active', 'inactive', 'deleted') CHARACTER SET ascii COLLATE ascii_bin,\n"""
             'CONSTRAINT "pk_EnumTable" PRIMARY KEY ("id")\n'
             ");",
         )
-        self.assertMatchSQLCreate(
+        self.assertMatchSQLCreateOptions(
+            options,
             "mssql",
             tables.EnumTable,
             'CREATE TABLE "EnumTable" (\n'
             '"id" bigint NOT NULL,\n'
             '"state" integer NOT NULL,\n'
             '"optional_state" integer,\n'
             'CONSTRAINT "pk_EnumTable" PRIMARY KEY ("id")\n'
             ");\n"
             'CREATE TABLE "WorkflowState" (\n'
             '"id" integer NOT NULL IDENTITY,\n'
             '"value" varchar(64) NOT NULL,\n'
             'CONSTRAINT "pk_WorkflowState" PRIMARY KEY ("id")\n'
             ");\n"
+            """INSERT INTO "WorkflowState" ("value") VALUES ('active'), ('inactive'), ('deleted');\n"""
             'ALTER TABLE "EnumTable" ADD\n'
             'CONSTRAINT "fk_EnumTable_state" FOREIGN KEY ("state") REFERENCES "WorkflowState" ("id"),\n'
             'CONSTRAINT "fk_EnumTable_optional_state" FOREIGN KEY ("optional_state") REFERENCES "WorkflowState" ("id");\n'
             'ALTER TABLE "WorkflowState" ADD\n'
             'CONSTRAINT "uq_WorkflowState" UNIQUE ("value");',
         )
 
+    def test_create_enum_array_table(self) -> None:
+        self.maxDiff = None
+        self.assertMatchSQLCreate(
+            "postgresql",
+            tables.EnumArrayTable,
+            """CREATE TYPE "WorkflowState" AS ENUM ('active', 'inactive', 'deleted');\n"""
+            'CREATE TABLE "EnumArrayTable" (\n'
+            '"id" bigint NOT NULL,\n'
+            '"states" "WorkflowState" ARRAY NOT NULL,\n'
+            'CONSTRAINT "pk_EnumArrayTable" PRIMARY KEY ("id")\n'
+            ");",
+        )
+        options = GeneratorOptions(
+            enum_mode=EnumMode.RELATION, namespaces={tables: None}
+        )
+        self.assertMatchSQLCreateOptions(
+            options,
+            "mysql",
+            tables.EnumArrayTable,
+            'CREATE TABLE "EnumArrayTable" (\n'
+            '"id" bigint NOT NULL,\n'
+            'CONSTRAINT "pk_EnumArrayTable" PRIMARY KEY ("id")\n'
+            ");\n"
+            'CREATE TABLE "WorkflowState" (\n'
+            '"id" integer NOT NULL AUTO_INCREMENT,\n'
+            '"value" varchar(64) NOT NULL,\n'
+            'CONSTRAINT "pk_WorkflowState" PRIMARY KEY ("id")\n'
+            ");\n"
+            'CREATE TABLE "EnumArrayTable_states_WorkflowState" (\n'
+            '"uuid" binary(16) NOT NULL,\n'
+            '"EnumArrayTable_states" bigint NOT NULL,\n'
+            '"WorkflowState_id" integer NOT NULL,\n'
+            'CONSTRAINT "pk_EnumArrayTable_states_WorkflowState" PRIMARY KEY ("uuid")\n'
+            ");\n"
+            'ALTER TABLE "WorkflowState"\n'
+            'ADD CONSTRAINT "uq_WorkflowState" UNIQUE ("value");\n'
+            'ALTER TABLE "EnumArrayTable_states_WorkflowState"\n'
+            'ADD CONSTRAINT "jk_EnumArrayTable_states" FOREIGN KEY ("EnumArrayTable_states") REFERENCES "EnumArrayTable" ("id"),\n'
+            'ADD CONSTRAINT "jk_WorkflowState_id" FOREIGN KEY ("WorkflowState_id") REFERENCES "WorkflowState" ("id");',
+        )
+
+    def test_create_extensible_enum_table(self) -> None:
+        self.maxDiff = None
+        options = GeneratorOptions(initialize_tables=True, namespaces={tables: None})
+        self.assertMatchSQLCreateOptions(
+            options,
+            "postgresql",
+            tables.ExtensibleEnumTable,
+            'CREATE TABLE "ExtensibleEnumTable" (\n'
+            '"id" bigint NOT NULL,\n'
+            '"state" integer NOT NULL,\n'
+            '"optional_state" integer,\n'
+            'CONSTRAINT "pk_ExtensibleEnumTable" PRIMARY KEY ("id")\n'
+            ");\n"
+            'CREATE TABLE "ExtensibleEnum" (\n'
+            '"id" integer GENERATED BY DEFAULT AS IDENTITY,\n'
+            '"value" varchar(64) NOT NULL,\n'
+            'CONSTRAINT "pk_ExtensibleEnum" PRIMARY KEY ("id")\n'
+            ");\n"
+            """INSERT INTO "ExtensibleEnum" ("value") VALUES ('__unspecified__');\n"""
+            'ALTER TABLE "ExtensibleEnumTable"\n'
+            'ADD CONSTRAINT "fk_ExtensibleEnumTable_state" FOREIGN KEY ("state") REFERENCES "ExtensibleEnum" ("id"),\n'
+            'ADD CONSTRAINT "fk_ExtensibleEnumTable_optional_state" FOREIGN KEY ("optional_state") REFERENCES "ExtensibleEnum" ("id");\n'
+            'ALTER TABLE "ExtensibleEnum"\n'
+            'ADD CONSTRAINT "uq_ExtensibleEnum" UNIQUE ("value");',
+        )
+
     def test_create_ipaddress_table(self) -> None:
         self.maxDiff = None
         self.assertMatchSQLCreate(
             "postgresql",
             tables.IPAddressTable,
             'CREATE TABLE "IPAddressTable" (\n'
             '"id" bigint NOT NULL,\n'
```

### Comparing `pysqlsync-0.5.0/tests/test_performance.py` & `pysqlsync-0.6.0/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/test_synchronize.py` & `pysqlsync-0.6.0/tests/test_synchronize.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/test_types.py` & `pysqlsync-0.6.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pysqlsync-0.5.0/tests/update_readme.py` & `pysqlsync-0.6.0/tests/update_readme.py`

 * *Files identical despite different names*

