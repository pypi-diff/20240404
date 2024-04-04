# Comparing `tmp/nti.property-2.0.1.tar.gz` & `tmp/nti.property-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nti.property-2.0.1.tar", last modified: Fri Feb 16 16:05:28 2024, max compression
+gzip compressed data, was "nti.property-2.0.2.tar", last modified: Thu Apr  4 15:27:35 2024, max compression
```

## Comparing `nti.property-2.0.1.tar` & `nti.property-2.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.918865 nti.property-2.0.1/
--rw-r--r--   0 jmadden    (501) staff       (20)      431 2024-02-16 16:05:28.000000 nti.property-2.0.1/.coveragerc
--rw-r--r--   0 jmadden    (501) staff       (20)       13 2024-02-16 16:05:28.000000 nti.property-2.0.1/.nti_cover_package
--rw-r--r--   0 jmadden    (501) staff       (20)     8939 2024-02-16 16:05:28.000000 nti.property-2.0.1/.pylintrc
--rw-r--r--   0 jmadden    (501) staff       (20)      525 2024-02-16 16:05:28.000000 nti.property-2.0.1/.readthedocs.yml
--rw-r--r--   0 jmadden    (501) staff       (20)      125 2024-02-16 16:05:28.000000 nti.property-2.0.1/AUTHORS
--rw-r--r--   0 jmadden    (501) staff       (20)      816 2024-02-16 16:05:28.000000 nti.property-2.0.1/CHANGES.rst
--rw-r--r--   0 jmadden    (501) staff       (20)       73 2024-02-16 16:05:28.000000 nti.property-2.0.1/COPYRIGHT.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.000000 nti.property-2.0.1/INSTALL
--rw-r--r--   0 jmadden    (501) staff       (20)      529 2024-02-16 16:05:28.000000 nti.property-2.0.1/LICENSE
--rw-r--r--   0 jmadden    (501) staff       (20)      436 2024-02-16 16:05:28.000000 nti.property-2.0.1/MANIFEST.in
--rw-r--r--   0 jmadden    (501) staff       (20)     2896 2024-02-16 16:05:28.918803 nti.property-2.0.1/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)      717 2024-02-16 16:05:28.000000 nti.property-2.0.1/README.rst
--rw-r--r--   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.000000 nti.property-2.0.1/TODO
--rw-r--r--   0 jmadden    (501) staff       (20)      146 2024-02-16 16:05:28.000000 nti.property-2.0.1/babel.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)       75 2024-02-16 16:05:28.000000 nti.property-2.0.1/doc-requirements.txt
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.916103 nti.property-2.0.1/docs/
--rw-r--r--   0 jmadden    (501) staff       (20)     7610 2024-02-16 16:05:28.000000 nti.property-2.0.1/docs/Makefile
--rw-r--r--   0 jmadden    (501) staff       (20)      728 2024-02-16 16:05:28.000000 nti.property-2.0.1/docs/api.rst
--rw-r--r--   0 jmadden    (501) staff       (20)     4669 2024-02-16 16:05:28.000000 nti.property-2.0.1/docs/conf.py
--rw-r--r--   0 jmadden    (501) staff       (20)      225 2024-02-16 16:05:28.000000 nti.property-2.0.1/docs/index.rst
--rw-r--r--   0 jmadden    (501) staff       (20)      271 2024-02-16 16:05:28.000000 nti.property-2.0.1/nose2.cfg
--rw-r--r--   0 jmadden    (501) staff       (20)       88 2024-02-16 16:05:28.000000 nti.property-2.0.1/pyproject.toml
--rw-r--r--   0 jmadden    (501) staff       (20)      166 2024-02-16 16:05:28.919138 nti.property-2.0.1/setup.cfg
--rwxr-xr-x   0 jmadden    (501) staff       (20)     1917 2024-02-16 16:05:28.000000 nti.property-2.0.1/setup.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.913589 nti.property-2.0.1/src/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.913635 nti.property-2.0.1/src/nti/
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.917560 nti.property-2.0.1/src/nti/property/
--rw-r--r--   0 jmadden    (501) staff       (20)      185 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)      311 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/configure.zcml
--rw-r--r--   0 jmadden    (501) staff       (20)     4594 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/dataurl.py
--rw-r--r--   0 jmadden    (501) staff       (20)      378 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/meta.zcml
--rw-r--r--   0 jmadden    (501) staff       (20)     4680 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/property.py
--rw-r--r--   0 jmadden    (501) staff       (20)      975 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/schema.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.918183 nti.property-2.0.1/src/nti/property/tests/
--rw-r--r--   0 jmadden    (501) staff       (20)      228 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/tests/__init__.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1933 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/tests/test_dataurl.py
--rw-r--r--   0 jmadden    (501) staff       (20)     5449 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/tests/test_property.py
--rw-r--r--   0 jmadden    (501) staff       (20)     1263 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/tests/test_schema.py
--rw-r--r--   0 jmadden    (501) staff       (20)      258 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/tests/test_tunables.py
--rw-r--r--   0 jmadden    (501) staff       (20)     3564 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/tests/test_urlproperty.py
--rw-r--r--   0 jmadden    (501) staff       (20)    21742 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/tunables.py
--rw-r--r--   0 jmadden    (501) staff       (20)     6178 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti/property/urlproperty.py
-drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-02-16 16:05:28.918331 nti.property-2.0.1/src/nti.property.egg-info/
--rw-r--r--   0 jmadden    (501) staff       (20)     2896 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti.property.egg-info/PKG-INFO
--rw-r--r--   0 jmadden    (501) staff       (20)     1036 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti.property.egg-info/SOURCES.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti.property.egg-info/dependency_links.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti.property.egg-info/namespace_packages.txt
--rw-r--r--   0 jmadden    (501) staff       (20)      212 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti.property.egg-info/requires.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        4 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti.property.egg-info/top_level.txt
--rw-r--r--   0 jmadden    (501) staff       (20)        1 2024-02-16 16:05:28.000000 nti.property-2.0.1/src/nti.property.egg-info/zip-safe
--rw-r--r--   0 jmadden    (501) staff       (20)     1148 2024-02-16 16:05:28.000000 nti.property-2.0.1/tox.ini
--rw-r--r--   0 jmadden    (501) staff       (20)        6 2024-02-16 16:05:28.000000 nti.property-2.0.1/version.txt
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:35.087452 nti.property-2.0.2/
+-rw-r--r--   0 jmadden    (501) staff       (20)      431 2024-04-04 15:27:34.000000 nti.property-2.0.2/.coveragerc
+-rw-r--r--   0 jmadden    (501) staff       (20)       13 2024-04-04 15:27:34.000000 nti.property-2.0.2/.nti_cover_package
+-rw-r--r--   0 jmadden    (501) staff       (20)     8939 2024-04-04 15:27:34.000000 nti.property-2.0.2/.pylintrc
+-rw-r--r--   0 jmadden    (501) staff       (20)      525 2024-04-04 15:27:34.000000 nti.property-2.0.2/.readthedocs.yml
+-rw-r--r--   0 jmadden    (501) staff       (20)      125 2024-04-04 15:27:34.000000 nti.property-2.0.2/AUTHORS
+-rw-r--r--   0 jmadden    (501) staff       (20)     1004 2024-04-04 15:27:34.000000 nti.property-2.0.2/CHANGES.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)       73 2024-04-04 15:27:34.000000 nti.property-2.0.2/COPYRIGHT.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:34.000000 nti.property-2.0.2/INSTALL
+-rw-r--r--   0 jmadden    (501) staff       (20)      529 2024-04-04 15:27:34.000000 nti.property-2.0.2/LICENSE
+-rw-r--r--   0 jmadden    (501) staff       (20)      436 2024-04-04 15:27:34.000000 nti.property-2.0.2/MANIFEST.in
+-rw-r--r--   0 jmadden    (501) staff       (20)     3084 2024-04-04 15:27:35.087387 nti.property-2.0.2/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)      717 2024-04-04 15:27:34.000000 nti.property-2.0.2/README.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:34.000000 nti.property-2.0.2/TODO
+-rw-r--r--   0 jmadden    (501) staff       (20)      146 2024-04-04 15:27:34.000000 nti.property-2.0.2/babel.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)       75 2024-04-04 15:27:34.000000 nti.property-2.0.2/doc-requirements.txt
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:35.084344 nti.property-2.0.2/docs/
+-rw-r--r--   0 jmadden    (501) staff       (20)     7610 2024-04-04 15:27:34.000000 nti.property-2.0.2/docs/Makefile
+-rw-r--r--   0 jmadden    (501) staff       (20)      728 2024-04-04 15:27:34.000000 nti.property-2.0.2/docs/api.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)     4669 2024-04-04 15:27:34.000000 nti.property-2.0.2/docs/conf.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      225 2024-04-04 15:27:34.000000 nti.property-2.0.2/docs/index.rst
+-rw-r--r--   0 jmadden    (501) staff       (20)      271 2024-04-04 15:27:34.000000 nti.property-2.0.2/nose2.cfg
+-rw-r--r--   0 jmadden    (501) staff       (20)       88 2024-04-04 15:27:34.000000 nti.property-2.0.2/pyproject.toml
+-rw-r--r--   0 jmadden    (501) staff       (20)      166 2024-04-04 15:27:35.087661 nti.property-2.0.2/setup.cfg
+-rwxr-xr-x   0 jmadden    (501) staff       (20)     1917 2024-04-04 15:27:34.000000 nti.property-2.0.2/setup.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:35.081686 nti.property-2.0.2/src/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:35.081734 nti.property-2.0.2/src/nti/
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:35.086133 nti.property-2.0.2/src/nti/property/
+-rw-r--r--   0 jmadden    (501) staff       (20)      185 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      311 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/configure.zcml
+-rw-r--r--   0 jmadden    (501) staff       (20)     4594 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/dataurl.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      378 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/meta.zcml
+-rw-r--r--   0 jmadden    (501) staff       (20)     4680 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/property.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      975 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/schema.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:35.086758 nti.property-2.0.2/src/nti/property/tests/
+-rw-r--r--   0 jmadden    (501) staff       (20)      228 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/tests/__init__.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1933 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/tests/test_dataurl.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     5449 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/tests/test_property.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     1263 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/tests/test_schema.py
+-rw-r--r--   0 jmadden    (501) staff       (20)      472 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/tests/test_tunables.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     3564 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/tests/test_urlproperty.py
+-rw-r--r--   0 jmadden    (501) staff       (20)    23314 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/tunables.py
+-rw-r--r--   0 jmadden    (501) staff       (20)     6178 2024-04-04 15:27:34.000000 nti.property-2.0.2/src/nti/property/urlproperty.py
+drwxr-xr-x   0 jmadden    (501) staff       (20)        0 2024-04-04 15:27:35.086917 nti.property-2.0.2/src/nti.property.egg-info/
+-rw-r--r--   0 jmadden    (501) staff       (20)     3084 2024-04-04 15:27:35.000000 nti.property-2.0.2/src/nti.property.egg-info/PKG-INFO
+-rw-r--r--   0 jmadden    (501) staff       (20)     1036 2024-04-04 15:27:35.000000 nti.property-2.0.2/src/nti.property.egg-info/SOURCES.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2024-04-04 15:27:35.000000 nti.property-2.0.2/src/nti.property.egg-info/dependency_links.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2024-04-04 15:27:35.000000 nti.property-2.0.2/src/nti.property.egg-info/namespace_packages.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)      212 2024-04-04 15:27:35.000000 nti.property-2.0.2/src/nti.property.egg-info/requires.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        4 2024-04-04 15:27:35.000000 nti.property-2.0.2/src/nti.property.egg-info/top_level.txt
+-rw-r--r--   0 jmadden    (501) staff       (20)        1 2024-04-04 15:27:35.000000 nti.property-2.0.2/src/nti.property.egg-info/zip-safe
+-rw-r--r--   0 jmadden    (501) staff       (20)     1148 2024-04-04 15:27:34.000000 nti.property-2.0.2/tox.ini
+-rw-r--r--   0 jmadden    (501) staff       (20)        6 2024-04-04 15:27:34.000000 nti.property-2.0.2/version.txt
```

### Comparing `nti.property-2.0.1/.pylintrc` & `nti.property-2.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/.readthedocs.yml` & `nti.property-2.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/LICENSE` & `nti.property-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/PKG-INFO` & `nti.property-2.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nti.property
-Version: 2.0.1
+Version: 2.0.2
 Summary: NTI Property
 Home-page: https://github.com/OpenNTI/nti.property
 Author: Jason Madden
 Author-email: jason@nextthought.com
 License: Apache
 Keywords: Property
 Classifier: Intended Audience :: Developers
@@ -58,14 +58,22 @@
 
 
 =========
  Changes
 =========
 
 
+2.0.2 (2024-04-04)
+==================
+
+- Make ``Tunable`` search harder (farther up the call chain)
+  to find a logger. This should make finding a logger in a
+  class definition better.
+
+
 2.0.1 (2024-02-16)
 ==================
 
 - Updates to documentation and logging for tunables.
 
 
 2.0.0 (2024-01-29)
```

### Comparing `nti.property-2.0.1/README.rst` & `nti.property-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/docs/Makefile` & `nti.property-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/docs/api.rst` & `nti.property-2.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/docs/conf.py` & `nti.property-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/setup.py` & `nti.property-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti/property/dataurl.py` & `nti.property-2.0.2/src/nti/property/dataurl.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti/property/property.py` & `nti.property-2.0.2/src/nti/property/property.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti/property/schema.py` & `nti.property-2.0.2/src/nti/property/schema.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti/property/tests/test_dataurl.py` & `nti.property-2.0.2/src/nti/property/tests/test_dataurl.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti/property/tests/test_property.py` & `nti.property-2.0.2/src/nti/property/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti/property/tests/test_schema.py` & `nti.property-2.0.2/src/nti/property/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti/property/tests/test_urlproperty.py` & `nti.property-2.0.2/src/nti/property/tests/test_urlproperty.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti/property/tunables.py` & `nti.property-2.0.2/src/nti/property/tunables.py`

 * *Files 4% similar despite different names*

```diff
@@ -517,26 +517,48 @@
     >>> tunable.value
     True
     >>> os.environ['RS_TEST_VAL'] = '192.168.1.1:80'
     >>> tunable = Tunable(0, 'RS_TEST_VAL', 'inet-address')
     >>> tunable.value
     ('192.168.1.1', 80)
 
-    You can supply a logger, or one will be found for you:
+    You can supply a logger, or one will be found for you
+    by looking for a 'logger' in the calling frames:
 
     >>> from nti.property.tunables import default_logger
     >>> logger = None
     >>> Tunable(0, 'RS_TEST_VAL').logger is default_logger
     True
-    >>> logger = 1
-    >>> Tunable(0, 'RS_TEST_VAL').logger == 1
+    >>> logger = "from parent frame"
+    >>> Tunable(0, 'RS_TEST_VAL').logger
+    'from parent frame'
+    >>> Tunable(0, 'RS_TEST_VAL', logger=42).logger
+    42
+    >>> class WithTunable:
+    ...   TUNABLE = Tunable(0, 'RS_TEST_VAL')
+    >>> WithTunable.TUNABLE.logger
+    'from parent frame'
+
+    If the closest logger that we find isn't a
+    real logger, but we find one farther away that _is_ a
+    real logger, we'll use that one:
+
+    >>> import logging
+    >>> real_logger = logging.getLogger('real.logger')
+    >>> def make_class():
+    ...    logger = real_logger
+    ...    def do_it():
+    ...        logger = 'not a real logger'
+    ...        class WithTunable:
+    ...           TUNABLE = Tunable(0, 'RS_TEST_VAL')
+    ...        return WithTunable
+    ...    return do_it()
+    >>> WithTunable = make_class()
+    >>> WithTunable.TUNABLE.logger is real_logger
     True
-    >>> Tunable(0, 'RS_TEST_VAL', logger=42).logger == 42
-    True
-
     """
 
     _NOT_SET = object()
     _target_name = ''
 
     def __init__(self, default, env_name=None,
                  getter=get_positive_integer_from_environ,
@@ -553,31 +575,52 @@
            that interface and having that name will be searched for; as a fallback, the hard-coded
            list of utilities in this module will be used.
 
            All of the named datatypes supported by :mod:`ZConfig.datatypes` are available
            to use as names.
         :param logger: The logger used to record information about the
            value being used. If not given, tries to find the variable named "logger"
-           in the calling frame.
+           in a calling frame that looks-like a logger.
+
+        .. versionchanged:: 2.0.2
+           Now searches harder up the call chain to find a logger,
+           and accepts the first one that looks-like a logger. If no
+           real logger can be found, then the first 'logger' variable we see
+           is used.
         """
         self.default = default
         self.env_name = env_name
         self.getter = getter
         if not callable(getter):
             getter = component.queryUtility(IEnvironGetter, name=getter,
                                             default=ENVIRON_GETTERS.get(getter))
         self.getter = getter
-        if not logger:
-            try:
-                logger = sys._getframe(1).f_locals['logger']
-            except (ValueError, KeyError, AttributeError):
-                logger = _logger
-        self.logger = logger or _logger
+        self.logger = logger or self._find_logger() or _logger
         self._value = self._NOT_SET
 
+    @staticmethod
+    def _find_logger():
+        logger = None
+        closest_candidate = None
+        try:
+            frame = sys._getframe(1) # pylint:disable=protected-access
+        except (AttributeError, ValueError): # pragma: no cover
+            # Attribute: Not implemented; Value: wrong depth
+            frame = None
+
+        while frame is not None:
+            candidate = frame.f_locals.get('logger')
+            closest_candidate = closest_candidate or candidate
+            if hasattr(candidate, 'log'):
+                logger = candidate
+                break
+            frame = frame.f_back
+        return logger or closest_candidate
+
+
     def __set_name__(self, cls, name):
         self._target_name = cls.__name__ + '.' + name
         if self.env_name is not None: # pragma: no cover
             return
         self.env_name = ('%s_%s_%s' % (
             cls.__module__,
             cls.__name__,
```

### Comparing `nti.property-2.0.1/src/nti/property/urlproperty.py` & `nti.property-2.0.2/src/nti/property/urlproperty.py`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/src/nti.property.egg-info/PKG-INFO` & `nti.property-2.0.2/src/nti.property.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nti.property
-Version: 2.0.1
+Version: 2.0.2
 Summary: NTI Property
 Home-page: https://github.com/OpenNTI/nti.property
 Author: Jason Madden
 Author-email: jason@nextthought.com
 License: Apache
 Keywords: Property
 Classifier: Intended Audience :: Developers
@@ -58,14 +58,22 @@
 
 
 =========
  Changes
 =========
 
 
+2.0.2 (2024-04-04)
+==================
+
+- Make ``Tunable`` search harder (farther up the call chain)
+  to find a logger. This should make finding a logger in a
+  class definition better.
+
+
 2.0.1 (2024-02-16)
 ==================
 
 - Updates to documentation and logging for tunables.
 
 
 2.0.0 (2024-01-29)
```

### Comparing `nti.property-2.0.1/src/nti.property.egg-info/SOURCES.txt` & `nti.property-2.0.2/src/nti.property.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nti.property-2.0.1/tox.ini` & `nti.property-2.0.2/tox.ini`

 * *Files identical despite different names*

