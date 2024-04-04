# Comparing `tmp/pf-azuredb-0.0.4.tar.gz` & `tmp/pf-azuredb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pf-azuredb-0.0.4.tar", last modified: Tue Mar 19 10:07:08 2024, max compression
+gzip compressed data, was "pf-azuredb-0.0.5.tar", last modified: Thu Apr  4 05:42:20 2024, max compression
```

## Comparing `pf-azuredb-0.0.4.tar` & `pf-azuredb-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 10:07:08.435529 pf-azuredb-0.0.4/
--rw-rw-rw-   0        0        0       30 2024-02-14 18:46:53.000000 pf-azuredb-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      316 2024-03-19 10:07:08.433527 pf-azuredb-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-19 10:07:08.432529 pf-azuredb-0.0.4/pf_azuredb.egg-info/
--rw-rw-rw-   0        0        0      316 2024-03-19 10:07:07.000000 pf-azuredb-0.0.4/pf_azuredb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-03-19 10:07:07.000000 pf-azuredb-0.0.4/pf_azuredb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 10:07:07.000000 pf-azuredb-0.0.4/pf_azuredb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-03-19 10:07:07.000000 pf-azuredb-0.0.4/pf_azuredb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       68 2024-03-19 10:07:07.000000 pf-azuredb-0.0.4/pf_azuredb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-19 10:07:07.000000 pf-azuredb-0.0.4/pf_azuredb.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-19 10:07:08.274973 pf-azuredb-0.0.4/pfazuredb/
--rw-rw-rw-   0        0        0       82 2024-02-14 18:46:53.000000 pf-azuredb-0.0.4/pfazuredb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 10:07:08.346496 pf-azuredb-0.0.4/pfazuredb/tools/
--rw-rw-rw-   0        0        0       82 2024-02-14 18:46:53.000000 pf-azuredb-0.0.4/pfazuredb/tools/__init__.py
--rw-rw-rw-   0        0        0     1200 2024-02-14 18:46:53.000000 pf-azuredb-0.0.4/pfazuredb/tools/mongodbvcore.py
--rw-rw-rw-   0        0        0     5241 2024-03-18 03:30:00.000000 pf-azuredb-0.0.4/pfazuredb/tools/postgrespg.py
--rw-rw-rw-   0        0        0      555 2024-02-14 18:46:53.000000 pf-azuredb-0.0.4/pfazuredb/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-19 10:07:08.381842 pf-azuredb-0.0.4/pfazuredb/yamls/
--rw-rw-rw-   0        0        0      504 2024-02-14 18:46:53.000000 pf-azuredb-0.0.4/pfazuredb/yamls/mongodbvcore.yaml
--rw-rw-rw-   0        0        0      661 2024-03-15 21:32:04.000000 pf-azuredb-0.0.4/pfazuredb/yamls/postgrespg.yaml
--rw-rw-rw-   0        0        0       42 2024-03-19 10:07:08.436103 pf-azuredb-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      663 2024-03-15 21:55:12.000000 pf-azuredb-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 10:07:08.428520 pf-azuredb-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-02-14 18:46:53.000000 pf-azuredb-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1966 2024-03-15 21:54:45.000000 pf-azuredb-0.0.4/tests/test_mongovcore.py
--rw-rw-rw-   0        0        0     2075 2024-03-15 21:54:45.000000 pf-azuredb-0.0.4/tests/test_postgres.py
+drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.886023 pf-azuredb-0.0.5/
+-rw-rw-rw-   0        0        0       30 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      316 2024-04-04 05:42:20.883041 pf-azuredb-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.881022 pf-azuredb-0.0.5/pf_azuredb.egg-info/
+-rw-rw-rw-   0        0        0      316 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       68 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-04 05:42:20.000000 pf-azuredb-0.0.5/pf_azuredb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.725044 pf-azuredb-0.0.5/pfazuredb/
+-rw-rw-rw-   0        0        0       82 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/pfazuredb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.778414 pf-azuredb-0.0.5/pfazuredb/tools/
+-rw-rw-rw-   0        0        0       82 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/pfazuredb/tools/__init__.py
+-rw-rw-rw-   0        0        0     2427 2024-04-04 05:42:11.000000 pf-azuredb-0.0.5/pfazuredb/tools/mongodbvcore.py
+-rw-rw-rw-   0        0        0     5241 2024-04-04 05:34:08.000000 pf-azuredb-0.0.5/pfazuredb/tools/postgrespg.py
+-rw-rw-rw-   0        0        0      555 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/pfazuredb/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.823161 pf-azuredb-0.0.5/pfazuredb/yamls/
+-rw-rw-rw-   0        0        0      724 2024-04-04 05:42:11.000000 pf-azuredb-0.0.5/pfazuredb/yamls/mongodbvcore.yaml
+-rw-rw-rw-   0        0        0      661 2024-04-04 05:34:08.000000 pf-azuredb-0.0.5/pfazuredb/yamls/postgrespg.yaml
+-rw-rw-rw-   0        0        0       42 2024-04-04 05:42:20.886023 pf-azuredb-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      663 2024-04-04 05:42:11.000000 pf-azuredb-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 05:42:20.879017 pf-azuredb-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-14 18:46:53.000000 pf-azuredb-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     1966 2024-04-04 05:31:30.000000 pf-azuredb-0.0.5/tests/test_mongovcore.py
+-rw-rw-rw-   0        0        0     2075 2024-03-15 21:54:45.000000 pf-azuredb-0.0.5/tests/test_postgres.py
```

### Comparing `pf-azuredb-0.0.4/pfazuredb/tools/postgrespg.py` & `pf-azuredb-0.0.5/pfazuredb/tools/postgrespg.py`

 * *Files identical despite different names*

### Comparing `pf-azuredb-0.0.4/pfazuredb/tools/utils.py` & `pf-azuredb-0.0.5/pfazuredb/tools/utils.py`

 * *Files identical despite different names*

### Comparing `pf-azuredb-0.0.4/pfazuredb/yamls/postgrespg.yaml` & `pf-azuredb-0.0.5/pfazuredb/yamls/postgrespg.yaml`

 * *Files identical despite different names*

### Comparing `pf-azuredb-0.0.4/setup.py` & `pf-azuredb-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "pf-azuredb"
 
 setup(
     name=PACKAGE_NAME,
     author="Hossein K. Heris and applied ai team@azure data",
-    version="0.0.4",
+    version="0.0.5",
     description="Package for use in promptflow for vector search in azure db",
     packages=find_packages(),
     entry_points={
         "package_tools": ["azuredb = pfazuredb.tools.utils:list_package_tools"],
     },
     include_package_data=True,  # This line tells setuptools to include files from MANIFEST.in
     install_requires=[
```

### Comparing `pf-azuredb-0.0.4/tests/test_mongovcore.py` & `pf-azuredb-0.0.5/tests/test_mongovcore.py`

 * *Files identical despite different names*

### Comparing `pf-azuredb-0.0.4/tests/test_postgres.py` & `pf-azuredb-0.0.5/tests/test_postgres.py`

 * *Files identical despite different names*

