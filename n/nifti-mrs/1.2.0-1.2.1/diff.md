# Comparing `tmp/nifti_mrs-1.2.0.tar.gz` & `tmp/nifti_mrs-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nifti_mrs-1.2.0.tar", last modified: Mon Apr  1 20:35:41 2024, max compression
+gzip compressed data, was "nifti_mrs-1.2.1.tar", last modified: Thu Apr  4 10:21:15 2024, max compression
```

## Comparing `nifti_mrs-1.2.0.tar` & `nifti_mrs-1.2.1.tar`

### file list

```diff
@@ -1,49 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.812173 nifti_mrs-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/mrs_tools/
--rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/mrs_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/mrs_tools/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/nifti_mrs/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/src/nifti_mrs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/create_nmrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/hdr_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/nifti_mrs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/nifti_mrs/standard/
--rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-04-01 20:35:33.000000 nifti_mrs-1.2.0/src/nifti_mrs/standard/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/nifti_mrs/standard/explanatory_doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-01 20:35:33.000000 nifti_mrs-1.2.0/src/nifti_mrs/standard/explanatory_doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.816174 nifti_mrs-1.2.0/src/nifti_mrs/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/tools/split_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/src/nifti_mrs/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 20:35:41.000000 nifti_mrs-1.2.0/src/nifti_mrs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:35:41.820174 nifti_mrs-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_create_nmrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_hdr_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)    27119 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_split_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_script_mrs_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-01 20:35:31.000000 nifti_mrs-1.2.0/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:21:15.820712 nifti_mrs-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-04 10:21:15.820712 nifti_mrs-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-04 10:21:15.824712 nifti_mrs-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:21:15.816712 nifti_mrs-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:21:15.816712 nifti_mrs-1.2.1/src/mrs_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    16945 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/mrs_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/mrs_tools/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:21:15.816712 nifti_mrs-1.2.1/src/nifti_mrs/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 10:21:15.824712 nifti_mrs-1.2.1/src/nifti_mrs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/create_nmrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/hdr_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24172 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/nifti_mrs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:21:15.820712 nifti_mrs-1.2.1/src/nifti_mrs/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/standard/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:21:15.820712 nifti_mrs-1.2.1/src/nifti_mrs/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/tools/reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/tools/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/tools/split_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/src/nifti_mrs/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:21:15.820712 nifti_mrs-1.2.1/src/nifti_mrs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-04 10:21:15.000000 nifti_mrs-1.2.1/src/nifti_mrs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 10:21:15.000000 nifti_mrs-1.2.1/src/nifti_mrs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:21:15.000000 nifti_mrs-1.2.1/src/nifti_mrs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 10:21:15.000000 nifti_mrs-1.2.1/src/nifti_mrs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-04 10:21:15.000000 nifti_mrs-1.2.1/src/nifti_mrs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 10:21:15.000000 nifti_mrs-1.2.1/src/nifti_mrs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:21:15.820712 nifti_mrs-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_create_nmrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_hdr_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_nifti_mrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27119 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_split_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_script_mrs_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-04 10:21:09.000000 nifti_mrs-1.2.1/tests/test_validator.py
```

### Comparing `nifti_mrs-1.2.0/LICENSE` & `nifti_mrs-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/PKG-INFO` & `nifti_mrs-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti_mrs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Software tools for the NIfTI-MRS data format
 Home-page: https://github.com/wtclarke/nifti_mrs_tools
 Author: William Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 License: BSD 3-Clause License
 Keywords: MRS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nifti_mrs-1.2.0/README.md` & `nifti_mrs-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/setup.cfg` & `nifti_mrs-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/mrs_tools/__init__.py` & `nifti_mrs-1.2.1/src/mrs_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/create_nmrs.py` & `nifti_mrs-1.2.1/src/nifti_mrs/create_nmrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/definitions.py` & `nifti_mrs-1.2.1/src/nifti_mrs/definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 version_info = sys.version_info
 if sys.version_info.minor >= 10:
     from importlib.resources import files
 else:
     # See https://setuptools.pypa.io/en/latest/userguide/datafiles.html#accessing-data-files-at-runtime
     from importlib_resources import files
 
-data_text = files('nifti_mrs.standard').joinpath('definitions.json').read_text()
+data_text = files('nifti_mrs.standard').joinpath('definitions.json').read_text(encoding='utf-8')
 json_def = json.loads(data_text)
 
 # Carry out translation
 nifti_mrs_version = [
     json_def['nifti_mrs_version']['major'],
     json_def['nifti_mrs_version']['minor']]
```

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/hdr_ext.py` & `nifti_mrs-1.2.1/src/nifti_mrs/hdr_ext.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/nifti_mrs.py` & `nifti_mrs-1.2.1/src/nifti_mrs/nifti_mrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/standard/definitions.json` & `nifti_mrs-1.2.1/src/nifti_mrs/standard/definitions.json`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/tools/reorder.py` & `nifti_mrs-1.2.1/src/nifti_mrs/tools/reorder.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/tools/reshape.py` & `nifti_mrs-1.2.1/src/nifti_mrs/tools/reshape.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/tools/split_merge.py` & `nifti_mrs-1.2.1/src/nifti_mrs/tools/split_merge.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/utils.py` & `nifti_mrs-1.2.1/src/nifti_mrs/utils.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs/validator.py` & `nifti_mrs-1.2.1/src/nifti_mrs/validator.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs.egg-info/PKG-INFO` & `nifti_mrs-1.2.1/src/nifti_mrs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nifti_mrs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Software tools for the NIfTI-MRS data format
 Home-page: https://github.com/wtclarke/nifti_mrs_tools
 Author: William Clarke
 Author-email: william.clarke@ndcn.ox.ac.uk
 License: BSD 3-Clause License
 Keywords: MRS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nifti_mrs-1.2.0/src/nifti_mrs.egg-info/SOURCES.txt` & `nifti_mrs-1.2.1/src/nifti_mrs.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 src/nifti_mrs.egg-info/PKG-INFO
 src/nifti_mrs.egg-info/SOURCES.txt
 src/nifti_mrs.egg-info/dependency_links.txt
 src/nifti_mrs.egg-info/entry_points.txt
 src/nifti_mrs.egg-info/requires.txt
 src/nifti_mrs.egg-info/top_level.txt
 src/nifti_mrs/standard/definitions.json
-src/nifti_mrs/standard/explanatory_doc/conf.py
 src/nifti_mrs/tools/__init__.py
 src/nifti_mrs/tools/misc.py
 src/nifti_mrs/tools/reorder.py
 src/nifti_mrs/tools/reshape.py
 src/nifti_mrs/tools/split_merge.py
 tests/test_create_nmrs.py
 tests/test_hdr_ext.py
```

### Comparing `nifti_mrs-1.2.0/tests/test_create_nmrs.py` & `nifti_mrs-1.2.1/tests/test_create_nmrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/tests/test_hdr_ext.py` & `nifti_mrs-1.2.1/tests/test_hdr_ext.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/tests/test_nifti_mrs.py` & `nifti_mrs-1.2.1/tests/test_nifti_mrs.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_reorder.py` & `nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_reorder.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_reshape.py` & `nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_reshape.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_split_merge.py` & `nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_split_merge.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/tests/test_nifti_mrs_tools_utils.py` & `nifti_mrs-1.2.1/tests/test_nifti_mrs_tools_utils.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/tests/test_script_mrs_tools.py` & `nifti_mrs-1.2.1/tests/test_script_mrs_tools.py`

 * *Files identical despite different names*

### Comparing `nifti_mrs-1.2.0/tests/test_validator.py` & `nifti_mrs-1.2.1/tests/test_validator.py`

 * *Files identical despite different names*

