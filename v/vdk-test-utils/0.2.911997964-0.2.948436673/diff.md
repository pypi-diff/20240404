# Comparing `tmp/vdk-test-utils-0.2.911997964.tar.gz` & `tmp/vdk-test-utils-0.2.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-test-utils-0.2.911997964.tar", last modified: Mon Jun 26 13:44:27 2023, max compression
+gzip compressed data, was "vdk-test-utils-0.2.948436673.tar", last modified: Fri Jul 28 09:43:48 2023, max compression
```

## Comparing `vdk-test-utils-0.2.911997964.tar` & `vdk-test-utils-0.2.948436673.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/
--rw-r--r--   0 root         (0) root         (0)     1501 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-06-26 13:44:17.000000 vdk-test-utils-0.2.911997964/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.599171 vdk-test-utils-0.2.911997964/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/
--rw-rw-rw-   0 root         (0) root         (0)     4347 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/ingest_util_plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     9551 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/util_funcs.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/util_plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1501 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-26 13:44:27.000000 vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 13:44:27.603170 vdk-test-utils-0.2.911997964/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/tests/test_util_funcs.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-26 13:44:13.000000 vdk-test-utils-0.2.911997964/tests/test_vdk_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:48.579027 vdk-test-utils-0.2.948436673/
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-07-28 09:43:48.579027 vdk-test-utils-0.2.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-07-28 09:43:27.000000 vdk-test-utils-0.2.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:48.579027 vdk-test-utils-0.2.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-07-28 09:43:36.000000 vdk-test-utils-0.2.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:48.575027 vdk-test-utils-0.2.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:48.575027 vdk-test-utils-0.2.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:48.575027 vdk-test-utils-0.2.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:48.579027 vdk-test-utils-0.2.948436673/src/vdk/plugin/test_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     4347 2023-07-28 09:43:27.000000 vdk-test-utils-0.2.948436673/src/vdk/plugin/test_utils/ingest_util_plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     9551 2023-07-28 09:43:27.000000 vdk-test-utils-0.2.948436673/src/vdk/plugin/test_utils/util_funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-07-28 09:43:27.000000 vdk-test-utils-0.2.948436673/src/vdk/plugin/test_utils/util_plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:48.579027 vdk-test-utils-0.2.948436673/src/vdk_test_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-07-28 09:43:48.000000 vdk-test-utils-0.2.948436673/src/vdk_test_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-28 09:43:48.000000 vdk-test-utils-0.2.948436673/src/vdk_test_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:48.000000 vdk-test-utils-0.2.948436673/src/vdk_test_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 09:43:48.000000 vdk-test-utils-0.2.948436673/src/vdk_test_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:48.000000 vdk-test-utils-0.2.948436673/src/vdk_test_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:48.579027 vdk-test-utils-0.2.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-28 09:43:27.000000 vdk-test-utils-0.2.948436673/tests/test_util_funcs.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-07-28 09:43:27.000000 vdk-test-utils-0.2.948436673/tests/test_vdk_test_utils.py
```

### Comparing `vdk-test-utils-0.2.911997964/PKG-INFO` & `vdk-test-utils-0.2.948436673/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-test-utils
-Version: 0.2.911997964
+Version: 0.2.948436673
 Summary: Provides utilities for testing Versatile Data Kit SDK plugins.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-test-utils-0.2.911997964/README.md` & `vdk-test-utils-0.2.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-test-utils-0.2.911997964/setup.py` & `vdk-test-utils-0.2.948436673/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.911997964"
+__version__ = "0.2.948436673"
 
 setuptools.setup(
     name="vdk-test-utils",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Provides utilities for testing Versatile Data Kit SDK plugins.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/ingest_util_plugins.py` & `vdk-test-utils-0.2.948436673/src/vdk/plugin/test_utils/ingest_util_plugins.py`

 * *Files identical despite different names*

### Comparing `vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/util_funcs.py` & `vdk-test-utils-0.2.948436673/src/vdk/plugin/test_utils/util_funcs.py`

 * *Files identical despite different names*

### Comparing `vdk-test-utils-0.2.911997964/src/vdk/plugin/test_utils/util_plugins.py` & `vdk-test-utils-0.2.948436673/src/vdk/plugin/test_utils/util_plugins.py`

 * *Files identical despite different names*

### Comparing `vdk-test-utils-0.2.911997964/src/vdk_test_utils.egg-info/PKG-INFO` & `vdk-test-utils-0.2.948436673/src/vdk_test_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-test-utils
-Version: 0.2.911997964
+Version: 0.2.948436673
 Summary: Provides utilities for testing Versatile Data Kit SDK plugins.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-test-utils-0.2.911997964/tests/test_util_funcs.py` & `vdk-test-utils-0.2.948436673/tests/test_util_funcs.py`

 * *Files identical despite different names*

