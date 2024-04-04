# Comparing `tmp/holcstore-0.1.5.tar.gz` & `tmp/holcstore-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holcstore-0.1.5.tar", last modified: Thu Mar 21 16:22:56 2024, max compression
+gzip compressed data, was "holcstore-0.1.6.tar", last modified: Thu Apr  4 07:06:00 2024, max compression
```

## Comparing `holcstore-0.1.5.tar` & `holcstore-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:22:56.206966 holcstore-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-21 16:22:50.000000 holcstore-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-21 16:22:50.000000 holcstore-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-21 16:22:56.206966 holcstore-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-21 16:22:50.000000 holcstore-0.1.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:22:56.206966 holcstore-0.1.5/holcstore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:22:50.000000 holcstore-0.1.5/holcstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-21 16:22:50.000000 holcstore-0.1.5/holcstore/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-03-21 16:22:50.000000 holcstore-0.1.5/holcstore/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-21 16:22:50.000000 holcstore-0.1.5/holcstore/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-21 16:22:50.000000 holcstore-0.1.5/holcstore/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:22:56.206966 holcstore-0.1.5/holcstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-21 16:22:56.000000 holcstore-0.1.5/holcstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-21 16:22:56.000000 holcstore-0.1.5/holcstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 16:22:56.000000 holcstore-0.1.5/holcstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-21 16:22:56.000000 holcstore-0.1.5/holcstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-21 16:22:56.000000 holcstore-0.1.5/holcstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:22:56.206966 holcstore-0.1.5/hostore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 16:22:56.206966 holcstore-0.1.5/hostore/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-21 16:22:50.000000 holcstore-0.1.5/hostore/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-21 16:22:50.000000 holcstore-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-21 16:22:56.206966 holcstore-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-21 16:22:50.000000 holcstore-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.050542 holcstore-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-04 07:05:56.000000 holcstore-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 07:05:56.000000 holcstore-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-04 07:06:00.050542 holcstore-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-04 07:05:56.000000 holcstore-0.1.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.046542 holcstore-0.1.6/holcstore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.050542 holcstore-0.1.6/holcstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.046542 holcstore-0.1.6/hostore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.046542 holcstore-0.1.6/hostore/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.050542 holcstore-0.1.6/hostore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/utils/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 07:05:56.000000 holcstore-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-04 07:06:00.050542 holcstore-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 07:05:56.000000 holcstore-0.1.6/setup.py
```

### Comparing `holcstore-0.1.5/LICENSE` & `holcstore-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.5/PKG-INFO` & `holcstore-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.1.5/README.rst` & `holcstore-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.5/holcstore/settings.py` & `holcstore-0.1.6/holcstore/settings.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.5/holcstore/urls.py` & `holcstore-0.1.6/holcstore/urls.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.5/holcstore.egg-info/PKG-INFO` & `holcstore-0.1.6/holcstore.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.1.5/holcstore.egg-info/SOURCES.txt` & `holcstore-0.1.6/holcstore.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 hostore/apps.py
 hostore/manager.py
 hostore/models.py
 hostore/tests.py
 hostore/views.py
 hostore/migrations/0001_initial.py
 hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
-hostore/migrations/__init__.py
+hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
+hostore/migrations/__init__.py
+hostore/utils/__init__.py
+hostore/utils/timeseries.py
```

### Comparing `holcstore-0.1.5/hostore/migrations/0001_initial.py` & `holcstore-0.1.6/hostore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.5/setup.cfg` & `holcstore-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = holcstore
-version = 0.1.5
+version = 0.1.6
 description = A Django App to use a simple load curve store
 long_description = file: README.rst
 url = 
 author = Jean-Pierre Lartigue
 author_email = 
 license = BSD-3-Clause
 classifiers =
```

