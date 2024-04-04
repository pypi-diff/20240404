# Comparing `tmp/stadb-0.0.1.tar.gz` & `tmp/stadb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stadb-0.0.1.tar", last modified: Thu Apr  4 09:58:18 2024, max compression
+gzip compressed data, was "stadb-0.0.2.tar", last modified: Thu Apr  4 10:55:18 2024, max compression
```

## Comparing `stadb-0.0.1.tar` & `stadb-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 09:58:18.383956 stadb-0.0.1/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.1/LICENSE
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2498 2024-04-04 09:58:18.383956 stadb-0.0.1/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      152 2024-04-04 09:43:17.000000 stadb-0.0.1/README.md
--rw-rw-r--   0 enoc      (1000) enoc      (1000)     2252 2024-04-04 09:50:23.000000 stadb-0.0.1/pyproject.toml
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-04 09:58:18.383956 stadb-0.0.1/setup.cfg
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 09:58:18.379956 stadb-0.0.1/src/
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 09:58:18.379956 stadb-0.0.1/src/stadb/
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       49 2024-04-04 09:57:09.000000 stadb-0.0.1/src/stadb/__init__.py
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      375 2024-04-04 09:56:56.000000 stadb-0.0.1/src/stadb/sensorthings.py
-drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 09:58:18.383956 stadb-0.0.1/src/stadb.egg-info/
--rw-r--r--   0 enoc      (1000) enoc      (1000)     2498 2024-04-04 09:58:18.000000 stadb-0.0.1/src/stadb.egg-info/PKG-INFO
--rw-rw-r--   0 enoc      (1000) enoc      (1000)      244 2024-04-04 09:58:18.000000 stadb-0.0.1/src/stadb.egg-info/SOURCES.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-04 09:58:18.000000 stadb-0.0.1/src/stadb.egg-info/dependency_links.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)       27 2024-04-04 09:58:18.000000 stadb-0.0.1/src/stadb.egg-info/requires.txt
--rw-rw-r--   0 enoc      (1000) enoc      (1000)        6 2024-04-04 09:58:18.000000 stadb-0.0.1/src/stadb.egg-info/top_level.txt
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 10:55:18.839197 stadb-0.0.2/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1069 2024-04-04 09:35:28.000000 stadb-0.0.2/LICENSE
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-04 10:55:18.839197 stadb-0.0.2/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      565 2024-04-04 10:42:11.000000 stadb-0.0.2/README.md
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     2281 2024-04-04 10:38:18.000000 stadb-0.0.2/pyproject.toml
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       38 2024-04-04 10:55:18.839197 stadb-0.0.2/setup.cfg
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 10:55:18.839197 stadb-0.0.2/src/
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 10:55:18.839197 stadb-0.0.2/src/stadb/
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       43 2024-04-04 10:50:06.000000 stadb-0.0.2/src/stadb/__init__.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     1250 2024-04-04 10:27:53.000000 stadb-0.0.2/src/stadb/logger.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     3355 2024-04-04 10:30:39.000000 stadb-0.0.2/src/stadb/postgresql.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)    50745 2024-04-04 10:52:53.000000 stadb-0.0.2/src/stadb/sensorthings.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     7652 2024-04-04 10:34:28.000000 stadb-0.0.2/src/stadb/timescaledb.py
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)     4355 2024-04-04 10:52:53.000000 stadb-0.0.2/src/stadb/utils.py
+drwxrwxr-x   0 enoc      (1000) enoc      (1000)        0 2024-04-04 10:55:18.839197 stadb-0.0.2/src/stadb.egg-info/
+-rw-r--r--   0 enoc      (1000) enoc      (1000)     2949 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/PKG-INFO
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      344 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/SOURCES.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)        1 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/dependency_links.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       50 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/requires.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)       11 2024-04-04 10:55:18.000000 stadb-0.0.2/src/stadb.egg-info/top_level.txt
+-rw-rw-r--   0 enoc      (1000) enoc      (1000)      234 2024-04-04 10:49:56.000000 stadb-0.0.2/src/test.py
```

### Comparing `stadb-0.0.1/LICENSE` & `stadb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stadb-0.0.1/PKG-INFO` & `stadb-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.1
+Version: 0.0.2
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
         
@@ -41,10 +41,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich>=12.5.1
 Requires-Dist: pandas>=1.4.3
+Requires-Dist: psycopg2-binary>=2.9.1
 
 # SensorThings Database Connector
-Database connector for SensorThings API database for advanced interaction. It is based on FROST-Server implementation
+Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
+
+It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
+
+### Contact info ###
+
+* **author**: Enoc Martínez  
+* **version**: 0.0.2
+* **organization**: Universitat Politècnica de Catalunya (UPC)  
+* **contact**: enoc.martinez@upc.edu
```

### Comparing `stadb-0.0.1/pyproject.toml` & `stadb-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 
 
 [project]
 
 name = "stadb"  # REQUIRED, is the only field that cannot be marked as dynamic.
-version = "0.0.1"  # REQUIRED, although can be dynamic
+version = "0.0.2"  # REQUIRED, although can be dynamic
 description = "SensorThings API database connector for advanced functionalities"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["sta", "setuptools", "development", "sensorthings"]
 
 authors = [
@@ -56,15 +56,17 @@
 # Any package you put here will be installed by pip when your project is
 # installed, so they must be valid existing projects.
 #
 # For an analysis of this field vs pip's requirements files see:
 # https://packaging.python.org/discussions/install-requires-vs-requirements/
 dependencies = [
   "rich>=12.5.1",
-  "pandas>=1.4.3"
+  "pandas>=1.4.3",
+  "psycopg2-binary>=2.9.1"
 ]
+
 [project.urls]
 "Homepage" = "https://github.com/EnocMartinez/stadb"
 "Source" = "https://github.com/EnocMartinez/stadb"
 
 
 [tool.setuptools]
```

### Comparing `stadb-0.0.1/src/stadb.egg-info/PKG-INFO` & `stadb-0.0.2/src/stadb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stadb
-Version: 0.0.1
+Version: 0.0.2
 Summary: SensorThings API database connector for advanced functionalities
 Author-email: Enoc Martínez <enoc.martinez@upc.edu>
 Maintainer-email: Enoc Martínez <enoc.martinez@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 EnocMartinez
         
@@ -41,10 +41,20 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rich>=12.5.1
 Requires-Dist: pandas>=1.4.3
+Requires-Dist: psycopg2-binary>=2.9.1
 
 # SensorThings Database Connector
-Database connector for SensorThings API database for advanced interaction. It is based on FROST-Server implementation
+Database connector for SensorThings API database for advanced interaction. It is based on [FROST-Server](https://github.com/FraunhoferIOSB/FROST-Server) implementation.
+
+It also adds specific support for time-series data by extending the database with [TimescaleDB](https://www.timescale.com/), which allows for faster queries and optimized storage. 
+
+### Contact info ###
+
+* **author**: Enoc Martínez  
+* **version**: 0.0.2
+* **organization**: Universitat Politècnica de Catalunya (UPC)  
+* **contact**: enoc.martinez@upc.edu
```

