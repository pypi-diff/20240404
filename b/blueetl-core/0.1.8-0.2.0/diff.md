# Comparing `tmp/blueetl-core-0.1.8.tar.gz` & `tmp/blueetl-core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueetl-core-0.1.8.tar", last modified: Fri Mar 22 14:11:30 2024, max compression
+gzip compressed data, was "blueetl-core-0.2.0.tar", last modified: Thu Apr  4 07:57:25 2024, max compression
```

## Comparing `blueetl-core-0.1.8.tar` & `blueetl-core-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.174881 blueetl-core-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.166881 blueetl-core-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.170881 blueetl-core-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-03-22 14:11:30.174881 blueetl-core-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.170881 blueetl-core-0.1.8/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.170881 blueetl-core-0.1.8/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.170881 blueetl-core-0.1.8/doc/source/_images/
--rw-r--r--   0 runner    (1001) docker     (127)   186341 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/doc/source/_images/BlueETL.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 14:11:30.174881 blueetl-core-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.166881 blueetl-core-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.170881 blueetl-core-0.1.8/src/blueetl_core/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/src/blueetl_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-22 14:11:30.000000 blueetl-core-0.1.8/src/blueetl_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/src/blueetl_core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    21794 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/src/blueetl_core/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/src/blueetl_core/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/src/blueetl_core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/src/blueetl_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.174881 blueetl-core-0.1.8/src/blueetl_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-03-22 14:11:30.000000 blueetl-core-0.1.8/src/blueetl_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-22 14:11:30.000000 blueetl-core-0.1.8/src/blueetl_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:11:30.000000 blueetl-core-0.1.8/src/blueetl_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-22 14:11:30.000000 blueetl-core-0.1.8/src/blueetl_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-22 14:11:30.000000 blueetl-core-0.1.8/src/blueetl_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:30.174881 blueetl-core-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/tests/test_etl_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/tests/test_etl_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/tests/test_etl_series.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-03-22 14:11:24.000000 blueetl-core-0.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.262426 blueetl-core-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.254425 blueetl-core-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.258425 blueetl-core-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-04 07:57:25.262426 blueetl-core-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.258425 blueetl-core-0.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.258425 blueetl-core-0.2.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.258425 blueetl-core-0.2.0/doc/source/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)   186341 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/doc/source/_images/BlueETL.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:57:25.262426 blueetl-core-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.258425 blueetl-core-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.262426 blueetl-core-0.2.0/src/blueetl_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/src/blueetl_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 07:57:25.000000 blueetl-core-0.2.0/src/blueetl_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/src/blueetl_core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/src/blueetl_core/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/src/blueetl_core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/src/blueetl_core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/src/blueetl_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.262426 blueetl-core-0.2.0/src/blueetl_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-04 07:57:25.000000 blueetl-core-0.2.0/src/blueetl_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-04 07:57:25.000000 blueetl-core-0.2.0/src/blueetl_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:57:25.000000 blueetl-core-0.2.0/src/blueetl_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-04 07:57:25.000000 blueetl-core-0.2.0/src/blueetl_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 07:57:25.000000 blueetl-core-0.2.0/src/blueetl_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:25.262426 blueetl-core-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17938 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/tests/test_etl_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/tests/test_etl_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/tests/test_etl_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18018 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-04 07:57:19.000000 blueetl-core-0.2.0/tox.ini
```

### Comparing `blueetl-core-0.1.8/.github/workflows/publish-sdist.yml` & `blueetl-core-0.2.0/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/.github/workflows/run-tox.yml` & `blueetl-core-0.2.0/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/LICENSE.txt` & `blueetl-core-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/PKG-INFO` & `blueetl-core-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueetl-core
-Version: 0.1.8
+Version: 0.2.0
 Summary: Core transformations for BlueETL
 Author: Blue Brain Project, EPFL
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/BlueBrain/blueetl-core
 Project-URL: Repository, https://github.com/BlueBrain/blueetl-core.git
 Project-URL: Documentation, https://blueetl-core.readthedocs.io/
 Project-URL: Tracker, https://github.com/BlueBrain/blueetl-core/issues
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 Requires-Dist: numpy>=1.19.4
 Requires-Dist: pandas>=1.3.0
```

### Comparing `blueetl-core-0.1.8/README.rst` & `blueetl-core-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/doc/Makefile` & `blueetl-core-0.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/doc/source/_images/BlueETL.jpeg` & `blueetl-core-0.2.0/doc/source/_images/BlueETL.jpeg`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/doc/source/conf.py` & `blueetl-core-0.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/pyproject.toml` & `blueetl-core-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
 ]
 dependencies = [
     "numpy>=1.19.4",
     "pandas>=1.3.0",
     "joblib>=1.3.1",
     "packaging>=21.3",
```

### Comparing `blueetl-core-0.1.8/src/blueetl_core/constants.py` & `blueetl-core-0.2.0/src/blueetl_core/constants.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/src/blueetl_core/etl.py` & `blueetl-core-0.2.0/src/blueetl_core/etl.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,21 @@
         """
         columns = self._obj.columns
         for named_index, value in zip(
             self._obj.index.etl.iterdict(), self._obj.itertuples(index=False)
         ):
             yield named_index, dict(zip(columns, value))
 
+    def insert_columns(self, loc: int, columns: list, values: list) -> None:
+        """Insert multiple columns, similar to repeatedly calling DataFrame.insert()."""
+        if len(columns) != len(values):
+            raise ValueError("columns and values must have the same length")
+        for col, val in zip(reversed(columns), reversed(values)):
+            self._obj.insert(loc, col, val)
+
     def _query_list(self, query_list: list[dict[str, Any]]) -> pd.DataFrame:
         """Given a list of query dicts, return the DataFrame filtered by columns and index."""
         return query_frame(self._obj, query_list)
 
     def groupby_iter(
         self,
         groupby_columns: list[str],
```

### Comparing `blueetl-core-0.1.8/src/blueetl_core/parallel.py` & `blueetl-core-0.2.0/src/blueetl_core/parallel.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from collections.abc import Iterable
 from dataclasses import dataclass
 from typing import Any, Callable, Optional
 
 import numpy as np
 from joblib import Parallel, delayed
+from joblib.externals.loky import get_reusable_executor
 
 from blueetl_core.constants import (
     BLUEETL_JOBLIB_BACKEND,
     BLUEETL_JOBLIB_JOBS,
     BLUEETL_JOBLIB_VERBOSE,
     BLUEETL_SUBPROCESS_LOGGING_LEVEL,
 )
@@ -69,46 +70,53 @@
 
 def run_parallel(
     tasks: Iterable[Callable[[TaskContext], Any]],
     jobs: Optional[int] = None,
     backend: Optional[str] = None,
     verbose: Optional[int] = None,
     base_seed: Optional[int] = None,
+    shutdown_executor: bool = True,
 ) -> list[Any]:
     """Run tasks in parallel.
 
     Args:
         tasks: iterable of callable objects that will be called in separate threads or processes.
             The callable must accept a single parameter ctx, that will contain a TaskContext.
         jobs: number of jobs. If not specified, use the BLUEETL_JOBLIB_JOBS env variable,
             or use half of the available cpus. Set to 1 to disable parallelization.
         backend: backend passed to joblib. If not specified, use the BLUEETL_JOBLIB_BACKEND env
             variable, or use the joblib default (loky).
             Possible values: loky, multiprocessing, threading.
         verbose: verbosity of joblib. If not specified, use the BLUEETL_JOBLIB_VERBOSE.
         base_seed: initial base seed. If specified, a different seed is added to the task context,
             and passed to each callable object.
+        shutdown_executor: if True and using loky, shutdown the subprocesses before returning.
 
     Returns:
         list of objects returned by the callable objects, in the same order.
     """
     loglevel = L.getEffectiveLevel()
     if verbose is None:
         verbose_env = os.getenv(BLUEETL_JOBLIB_VERBOSE)
         verbose = int(verbose_env) if verbose_env else 0 if loglevel >= logging.WARNING else 10
     if not jobs:
         jobs_env = os.getenv(BLUEETL_JOBLIB_JOBS)
         jobs = int(jobs_env) if jobs_env else max((os.cpu_count() or 1) // 2, 1)
     if not backend:
         backend = os.getenv(BLUEETL_JOBLIB_BACKEND)
-    parallel = Parallel(n_jobs=jobs, backend=backend, verbose=verbose)
-    return parallel(
-        delayed(task)(
-            ctx=TaskContext(
-                task_id=i,
-                loglevel=loglevel,
-                seed=None if base_seed is None else base_seed + i,
-                ppid=os.getpid(),
+    try:
+        parallel = Parallel(n_jobs=jobs, backend=backend, verbose=verbose)
+        return parallel(
+            delayed(task)(
+                ctx=TaskContext(
+                    task_id=i,
+                    loglevel=loglevel,
+                    seed=None if base_seed is None else base_seed + i,
+                    ppid=os.getpid(),
+                )
             )
+            for i, task in enumerate(tasks)
         )
-        for i, task in enumerate(tasks)
-    )
+    finally:
+        if shutdown_executor and (not backend or backend == "loky"):
+            # shutdown the pool of processes used by loky
+            get_reusable_executor().shutdown(wait=True)
```

### Comparing `blueetl-core-0.1.8/src/blueetl_core/utils.py` & `blueetl-core-0.2.0/src/blueetl_core/utils.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/src/blueetl_core.egg-info/PKG-INFO` & `blueetl-core-0.2.0/src/blueetl_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueetl-core
-Version: 0.1.8
+Version: 0.2.0
 Summary: Core transformations for BlueETL
 Author: Blue Brain Project, EPFL
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/BlueBrain/blueetl-core
 Project-URL: Repository, https://github.com/BlueBrain/blueetl-core.git
 Project-URL: Documentation, https://blueetl-core.readthedocs.io/
 Project-URL: Tracker, https://github.com/BlueBrain/blueetl-core/issues
@@ -12,14 +12,15 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: AUTHORS.txt
 Requires-Dist: numpy>=1.19.4
 Requires-Dist: pandas>=1.3.0
```

### Comparing `blueetl-core-0.1.8/src/blueetl_core.egg-info/SOURCES.txt` & `blueetl-core-0.2.0/src/blueetl_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/tests/conftest.py` & `blueetl-core-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/tests/test_etl_dataframe.py` & `blueetl-core-0.2.0/tests/test_etl_dataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -468,14 +468,35 @@
     index, value = next(it)
     assert isinstance(index, dict)
     assert isinstance(value, dict)
     assert index == {"i0": "a", "i1": "c"}
     assert value == {"v0": 0, "v1": 4}
 
 
+def test_insert_columns(dataframe1):
+    columns = ["pre0", "pre1", "pre2"]
+    values = [111, [200, 201, 202, 203], np.nan]
+    original_columns = list(dataframe1.columns)
+
+    dataframe1.etl.insert_columns(loc=0, columns=columns, values=values)
+
+    assert_array_equal(dataframe1.columns, columns + original_columns)
+    assert_array_equal(dataframe1["pre0"], [111] * len(dataframe1))
+    assert_array_equal(dataframe1["pre1"], [200, 201, 202, 203])
+    assert_array_equal(dataframe1["pre2"], [np.nan] * len(dataframe1))
+
+
+def test_insert_columns_raises(dataframe1):
+    columns = ["pre0", "pre1", "pre2"]
+    values = [111]
+
+    with pytest.raises(ValueError, match="columns and values must have the same length"):
+        dataframe1.etl.insert_columns(loc=0, columns=columns, values=values)
+
+
 @pytest.mark.parametrize(
     "params, expected_key, expected_df",
     [
         pytest.param(
             {"groupby_columns": ["i1"]},
             ("c",),
             pd.DataFrame(
```

### Comparing `blueetl-core-0.1.8/tests/test_etl_index.py` & `blueetl-core-0.2.0/tests/test_etl_index.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/tests/test_etl_series.py` & `blueetl-core-0.2.0/tests/test_etl_series.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/tests/test_utils.py` & `blueetl-core-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueetl-core-0.1.8/tox.ini` & `blueetl-core-0.2.0/tox.ini`

 * *Files identical despite different names*

