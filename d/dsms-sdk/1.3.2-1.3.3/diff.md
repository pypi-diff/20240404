# Comparing `tmp/dsms_sdk-1.3.2.tar.gz` & `tmp/dsms_sdk-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsms_sdk-1.3.2.tar", last modified: Thu Mar 28 13:40:15 2024, max compression
+gzip compressed data, was "dsms_sdk-1.3.3.tar", last modified: Thu Apr  4 10:06:06 2024, max compression
```

## Comparing `dsms_sdk-1.3.2.tar` & `dsms_sdk-1.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.893092 dsms_sdk-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-28 13:40:15.893092 dsms_sdk-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.885091 dsms_sdk-1.3.2/dsms/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.885091 dsms_sdk-1.3.2/dsms/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/apps/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.885091 dsms_sdk-1.3.2/dsms/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/core/dsms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.889091 dsms_sdk-1.3.2/dsms/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14322 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/ktype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.889091 dsms_sdk-1.3.2/dsms/knowledge/properties/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/affiliations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/custom_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/linked_kitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/properties/user_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.889091 dsms_sdk-1.3.2/dsms/knowledge/sparql_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/sparql_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/sparql_interface/sparql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/sparql_interface/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/sparql_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/dsms/knowledge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.893092 dsms_sdk-1.3.2/dsms_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-03-28 13:40:15.000000 dsms_sdk-1.3.2/dsms_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-28 13:40:15.000000 dsms_sdk-1.3.2/dsms_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:40:15.000000 dsms_sdk-1.3.2/dsms_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-28 13:40:15.000000 dsms_sdk-1.3.2/dsms_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 13:40:15.000000 dsms_sdk-1.3.2/dsms_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-28 13:40:15.893092 dsms_sdk-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:15.893092 dsms_sdk-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/tests/test_kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-28 13:40:12.000000 dsms_sdk-1.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.702700 dsms_sdk-1.3.3/dsms/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.702700 dsms_sdk-1.3.3/dsms/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/apps/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.702700 dsms_sdk-1.3.3/dsms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/dsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.702700 dsms_sdk-1.3.3/dsms/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14322 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/ktype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.706700 dsms_sdk-1.3.3/dsms/knowledge/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/affiliations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/custom_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/linked_kitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/user_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.706700 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/sparql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/dsms_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/tests/test_kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/tests/test_utils.py
```

### Comparing `dsms_sdk-1.3.2/LICENSE` & `dsms_sdk-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/PKG-INFO` & `dsms_sdk-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.3.2/README.md` & `dsms_sdk-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/apps/apps.py` & `dsms_sdk-1.3.3/dsms/apps/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/apps/utils.py` & `dsms_sdk-1.3.3/dsms/apps/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/core/configuration.py` & `dsms_sdk-1.3.3/dsms/core/configuration.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/core/context.py` & `dsms_sdk-1.3.3/dsms/core/context.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/core/dsms.py` & `dsms_sdk-1.3.3/dsms/core/dsms.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/core/utils.py` & `dsms_sdk-1.3.3/dsms/core/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/kitem.py` & `dsms_sdk-1.3.3/dsms/knowledge/kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/ktype.py` & `dsms_sdk-1.3.3/dsms/knowledge/ktype.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/__init__.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/affiliations.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/affiliations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/annotations.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/annotations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/apps.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/attachments.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/attachments.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/authors.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/authors.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/base.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/contacts.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/contacts.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/custom_properties.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/custom_properties.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/external_links.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/external_links.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/hdf5.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/hdf5.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/linked_kitems.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/linked_kitems.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/summary.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/summary.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/properties/user_groups.py` & `dsms_sdk-1.3.3/dsms/knowledge/properties/user_groups.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/sparql_interface/sparql_interface.py` & `dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/sparql_interface.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/sparql_interface/subgraph.py` & `dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/subgraph.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/sparql_interface/utils.py` & `dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Sparql interface utilities for the DSMS"""
 import io
 from typing import TYPE_CHECKING
 
+from rdflib import Graph
 from rdflib.plugins.sparql.results.jsonresults import JSONResult
 
 from dsms.core.utils import _kitem_id2uri, _perform_request
 
 if TYPE_CHECKING:
     from typing import Any, Dict, Optional, TextIO, Union
 
-    from rdflib import Graph
-
 
 def _sparql_query(query: str, repository: str) -> "Dict[str, Any]":
     """Submit plain SPARQL-query to the DSMS instance."""
     response = _perform_request(
         "api/knowledge/sparql",
         "post",
         data={"query": query},
@@ -138,15 +137,17 @@
         BIND(
             <{identifier}> as ?g
             )
         {{
             GRAPH ?g {{ ?s ?p ?o . }}
         }}
     }}"""
+
+    graph = Graph(identifier=identifier)
     data = _sparql_query(query, repository)
-    graph = JSONResult(data)
-    graph.identifier = identifier
+    for row in JSONResult(data).bindings:
+        graph.add(row.values())
 
     if len(graph) == 0:
         raise ValueError(f"Subgraph for id `{identifier}` does not exist.")
 
     return graph
```

### Comparing `dsms_sdk-1.3.2/dsms/knowledge/utils.py` & `dsms_sdk-1.3.3/dsms/knowledge/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/dsms_sdk.egg-info/PKG-INFO` & `dsms_sdk-1.3.3/dsms_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.3.2/dsms_sdk.egg-info/SOURCES.txt` & `dsms_sdk-1.3.3/dsms_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/setup.cfg` & `dsms_sdk-1.3.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsms_sdk
-version = v1.3.2
+version = v1.3.3
 description = Python SDK core-package for working with the Dataspace Management System (DSMS).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 author = Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `dsms_sdk-1.3.2/tests/conftest.py` & `dsms_sdk-1.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/tests/test_kitem.py` & `dsms_sdk-1.3.3/tests/test_kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.2/tests/test_utils.py` & `dsms_sdk-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

