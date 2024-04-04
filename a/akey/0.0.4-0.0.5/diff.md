# Comparing `tmp/akey-0.0.4.tar.gz` & `tmp/akey-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akey-0.0.4.tar", last modified: Thu Apr  4 12:53:57 2024, max compression
+gzip compressed data, was "akey-0.0.5.tar", last modified: Thu Apr  4 12:58:59 2024, max compression
```

## Comparing `akey-0.0.4.tar` & `akey-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:53:57.191879 akey-0.0.4/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-27 18:20:15.000000 akey-0.0.4/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-27 18:20:15.000000 akey-0.0.4/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2044 2024-04-04 12:53:57.191491 akey-0.0.4/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1431 2023-11-30 20:00:19.000000 akey-0.0.4/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:53:57.190448 akey-0.0.4/akey/
--rw-r--r--   0 solst      (501) staff       (20)      384 2024-04-04 12:53:50.000000 akey-0.0.4/akey/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     2082 2024-04-04 12:53:50.000000 akey-0.0.4/akey/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2477 2024-04-04 12:53:50.000000 akey-0.0.4/akey/dims.py
--rw-r--r--   0 solst      (501) staff       (20)    11290 2024-04-04 12:53:50.000000 akey-0.0.4/akey/keys.py
--rw-r--r--   0 solst      (501) staff       (20)     7658 2024-04-04 12:53:50.000000 akey-0.0.4/akey/mock.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:53:57.191316 akey-0.0.4/akey.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2044 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      320 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-30 13:48:14.000000 akey-0.0.4/akey.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      186 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      987 2023-12-08 21:07:08.000000 akey-0.0.4/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-04 12:53:57.191980 akey-0.0.4/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2023-11-27 18:20:15.000000 akey-0.0.4/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:58:59.837184 akey-0.0.5/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-27 18:20:15.000000 akey-0.0.5/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-27 18:20:15.000000 akey-0.0.5/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2044 2024-04-04 12:58:59.836948 akey-0.0.5/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1431 2023-11-30 20:00:19.000000 akey-0.0.5/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:58:59.835313 akey-0.0.5/akey/
+-rw-r--r--   0 solst      (501) staff       (20)      384 2024-04-04 12:58:54.000000 akey-0.0.5/akey/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     2082 2024-04-04 12:58:54.000000 akey-0.0.5/akey/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     2477 2024-04-04 12:58:54.000000 akey-0.0.5/akey/dims.py
+-rw-r--r--   0 solst      (501) staff       (20)    11290 2024-04-04 12:58:54.000000 akey-0.0.5/akey/keys.py
+-rw-r--r--   0 solst      (501) staff       (20)     7658 2024-04-04 12:58:54.000000 akey-0.0.5/akey/mock.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:58:59.836645 akey-0.0.5/akey.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2044 2024-04-04 12:58:59.000000 akey-0.0.5/akey.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      320 2024-04-04 12:58:59.000000 akey-0.0.5/akey.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-04 12:58:59.000000 akey-0.0.5/akey.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-04 12:58:59.000000 akey-0.0.5/akey.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-30 13:48:14.000000 akey-0.0.5/akey.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      171 2024-04-04 12:58:59.000000 akey-0.0.5/akey.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-04 12:58:59.000000 akey-0.0.5/akey.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      972 2024-04-04 12:58:51.000000 akey-0.0.5/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-04 12:58:59.837247 akey-0.0.5/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2023-11-27 18:20:15.000000 akey-0.0.5/setup.py
```

### Comparing `akey-0.0.4/LICENSE` & `akey-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `akey-0.0.4/PKG-INFO` & `akey-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akey
-Version: 0.0.4
+Version: 0.0.5
 Summary: akey
 Home-page: https://github.com/dsm-72/akey
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: akey extra extras single cell sc scanpy anndata RNA-seq seq
 Classifier: Development Status :: 4 - Beta
```

### Comparing `akey-0.0.4/README.md` & `akey-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `akey-0.0.4/akey/_modidx.py` & `akey-0.0.5/akey/_modidx.py`

 * *Files identical despite different names*

### Comparing `akey-0.0.4/akey/dims.py` & `akey-0.0.5/akey/dims.py`

 * *Files identical despite different names*

### Comparing `akey-0.0.4/akey/keys.py` & `akey-0.0.5/akey/keys.py`

 * *Files identical despite different names*

### Comparing `akey-0.0.4/akey/mock.py` & `akey-0.0.5/akey/mock.py`

 * *Files identical despite different names*

### Comparing `akey-0.0.4/akey.egg-info/PKG-INFO` & `akey-0.0.5/akey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akey
-Version: 0.0.4
+Version: 0.0.5
 Summary: akey
 Home-page: https://github.com/dsm-72/akey
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: akey extra extras single cell sc scanpy anndata RNA-seq seq
 Classifier: Development Status :: 4 - Beta
```

### Comparing `akey-0.0.4/settings.ini` & `akey-0.0.5/settings.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = akey
 lib_name = akey
-version = 0.0.4
+version = 0.0.5
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = akey
 nbs_path = nbs
 recursive = True
@@ -29,10 +29,10 @@
 conda_user = dsm-72
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
-requirements = atyp psrc nchr nlit chck hasr asto calr fpos ltyp
+requirements = atup nchr nlit chck asto sigr quac
 dev_requirements = pandas numpy>=1.22 scipy anndata scanpy scrublet scprep phate magic-impute graphtools matplotlib seaborn excs torch scikit-learn
```

### Comparing `akey-0.0.4/setup.py` & `akey-0.0.5/setup.py`

 * *Files identical despite different names*

