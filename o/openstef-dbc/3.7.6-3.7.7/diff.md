# Comparing `tmp/openstef_dbc-3.7.6.tar.gz` & `tmp/openstef_dbc-3.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstef_dbc-3.7.6.tar", last modified: Wed Apr  3 14:38:41 2024, max compression
+gzip compressed data, was "openstef_dbc-3.7.7.tar", last modified: Thu Apr  4 15:14:28 2024, max compression
```

## Comparing `openstef_dbc-3.7.6.tar` & `openstef_dbc-3.7.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:38:41.220819 openstef_dbc-3.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-03 14:38:41.220819 openstef_dbc-3.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:38:41.216819 openstef_dbc-3.7.6/openstef_dbc/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/data_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/ktp_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:38:41.216819 openstef_dbc-3.7.6/openstef_dbc/log/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/log/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/log/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:38:41.216819 openstef_dbc-3.7.6/openstef_dbc/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/models/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/models/switch_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:38:41.220819 openstef_dbc-3.7.6/openstef_dbc/services/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/ems.py
--rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/model_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/prediction_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/systems.py
--rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/services/write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/openstef_dbc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:38:41.220819 openstef_dbc-3.7.6/openstef_dbc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-03 14:38:41.000000 openstef_dbc-3.7.6/openstef_dbc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-03 14:38:41.000000 openstef_dbc-3.7.6/openstef_dbc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:38:41.000000 openstef_dbc-3.7.6/openstef_dbc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 14:38:41.000000 openstef_dbc-3.7.6/openstef_dbc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 14:38:41.000000 openstef_dbc-3.7.6/openstef_dbc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 14:38:41.220819 openstef_dbc-3.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-03 14:38:30.000000 openstef_dbc-3.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.170999 openstef_dbc-3.7.7/openstef_dbc/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/data_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13530 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/ktp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.170999 openstef_dbc-3.7.7/openstef_dbc/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/log/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/log/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.170999 openstef_dbc-3.7.7/openstef_dbc/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/models/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/models/switch_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/openstef_dbc/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/ems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/model_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/prediction_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14529 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/services/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/openstef_dbc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/openstef_dbc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 15:14:28.000000 openstef_dbc-3.7.7/openstef_dbc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 15:14:28.174999 openstef_dbc-3.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-04 15:14:13.000000 openstef_dbc-3.7.7/setup.py
```

### Comparing `openstef_dbc-3.7.6/LICENSE` & `openstef_dbc-3.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/PKG-INFO` & `openstef_dbc-3.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.7.6
+Version: 3.7.7
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Requires-Dist: openstef~=3.4.4
 Requires-Dist: pydantic-settings<3.0.0,>=2.1.0
 Requires-Dist: influxdb-client~=1.36.1
 Requires-Dist: mysql-connector-python~=8.3.0
 Requires-Dist: PyMySQL~=1.0.2
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: requests~=2.28.1
-Requires-Dist: SQLAlchemy~=2.0.21
+Requires-Dist: SQLAlchemy
 
 <!--
 SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com>
 
 SPDX-License-Identifier: MPL-2.0
 -->
 [![Python Build](https://github.com/openstef/openstef-dbc/actions/workflows/python-build.yaml/badge.svg?branch=master)](https://github.com/openstef/openstef-dbc/actions/workflows/python-build.yaml)
```

### Comparing `openstef_dbc-3.7.6/README.md` & `openstef_dbc-3.7.7/README.md`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/__init__.py` & `openstef_dbc-3.7.7/openstef_dbc/__init__.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/data_interface.py` & `openstef_dbc-3.7.7/openstef_dbc/data_interface.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/database.py` & `openstef_dbc-3.7.7/openstef_dbc/database.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/ktp_api.py` & `openstef_dbc-3.7.7/openstef_dbc/ktp_api.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/log/logging.py` & `openstef_dbc-3.7.7/openstef_dbc/log/logging.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/log/processors.py` & `openstef_dbc-3.7.7/openstef_dbc/log/processors.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/models/measurement.py` & `openstef_dbc-3.7.7/openstef_dbc/models/measurement.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/ems.py` & `openstef_dbc-3.7.7/openstef_dbc/services/ems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/model_input.py` & `openstef_dbc-3.7.7/openstef_dbc/services/model_input.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/prediction_job.py` & `openstef_dbc-3.7.7/openstef_dbc/services/prediction_job.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/predictions.py` & `openstef_dbc-3.7.7/openstef_dbc/services/predictions.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/predictor.py` & `openstef_dbc-3.7.7/openstef_dbc/services/predictor.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/splitting.py` & `openstef_dbc-3.7.7/openstef_dbc/services/splitting.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/systems.py` & `openstef_dbc-3.7.7/openstef_dbc/services/systems.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/weather.py` & `openstef_dbc-3.7.7/openstef_dbc/services/weather.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/services/write.py` & `openstef_dbc-3.7.7/openstef_dbc/services/write.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc/utils.py` & `openstef_dbc-3.7.7/openstef_dbc/utils.py`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/openstef_dbc.egg-info/PKG-INFO` & `openstef_dbc-3.7.7/openstef_dbc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstef_dbc
-Version: 3.7.6
+Version: 3.7.7
 Summary: Database Connection for OpenSTEF
 Home-page: https://github.com/openstef/openstef-dbc
 Author: Alliander N.V
 Author-email: korte.termijn.prognoses@alliander.com
 License: MPL-2.0
 Keywords: database,energy,forecasting,machinelearning
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Requires-Dist: openstef~=3.4.4
 Requires-Dist: pydantic-settings<3.0.0,>=2.1.0
 Requires-Dist: influxdb-client~=1.36.1
 Requires-Dist: mysql-connector-python~=8.3.0
 Requires-Dist: PyMySQL~=1.0.2
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: requests~=2.28.1
-Requires-Dist: SQLAlchemy~=2.0.21
+Requires-Dist: SQLAlchemy
 
 <!--
 SPDX-FileCopyrightText: 2017-2022 Contributors to the OpenSTEF project <korte.termijn.prognoses@alliander.com>
 
 SPDX-License-Identifier: MPL-2.0
 -->
 [![Python Build](https://github.com/openstef/openstef-dbc/actions/workflows/python-build.yaml/badge.svg?branch=master)](https://github.com/openstef/openstef-dbc/actions/workflows/python-build.yaml)
```

### Comparing `openstef_dbc-3.7.6/openstef_dbc.egg-info/SOURCES.txt` & `openstef_dbc-3.7.7/openstef_dbc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstef_dbc-3.7.6/setup.py` & `openstef_dbc-3.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def read_long_description_from_readme():
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 
 setup(
     name="openstef_dbc",
-    version="3.7.6",
+    version="3.7.7",
     packages=find_packages(include=["openstef_dbc", "openstef_dbc.*"]),
     description="Database Connection for OpenSTEF",
     long_description=read_long_description_from_readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/openstef/openstef-dbc",
     author="Alliander N.V",
     author_email="korte.termijn.prognoses@alliander.com",
```

