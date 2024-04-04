# Comparing `tmp/execdata-5.2.2.tar.gz` & `tmp/execdata-5.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "execdata-5.2.2.tar", last modified: Thu Mar 14 19:52:17 2024, max compression
+gzip compressed data, was "execdata-5.2.3.tar", last modified: Thu Apr  4 20:31:23 2024, max compression
```

## Comparing `execdata-5.2.2.tar` & `execdata-5.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:52:17.600813 execdata-5.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-14 19:52:10.000000 execdata-5.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-14 19:52:17.600813 execdata-5.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-14 19:52:10.000000 execdata-5.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:52:17.596813 execdata-5.2.2/execdata/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:52:17.596813 execdata-5.2.2/execdata/eda/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/eda/_data_mining.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/eda/_data_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/eda/_feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/eda/_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:52:17.596813 execdata-5.2.2/execdata/format/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/format/_data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/format/_format_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:52:17.600813 execdata-5.2.2/execdata/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/graph/_data_analysis_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/graph/_data_mining_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/graph/_linear_regression_type_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/graph/_logistic_regression_type_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:52:17.600813 execdata-5.2.2/execdata/model/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/model/_model_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-14 19:52:10.000000 execdata-5.2.2/execdata/model/_regression_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 19:52:17.600813 execdata-5.2.2/execdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-03-14 19:52:17.000000 execdata-5.2.2/execdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-14 19:52:17.000000 execdata-5.2.2/execdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 19:52:17.000000 execdata-5.2.2/execdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 19:52:17.000000 execdata-5.2.2/execdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-14 19:52:10.000000 execdata-5.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 19:52:17.600813 execdata-5.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-14 19:52:10.000000 execdata-5.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.463508 execdata-5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 20:31:19.000000 execdata-5.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 20:31:23.459508 execdata-5.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 20:31:19.000000 execdata-5.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/eda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/_data_mining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/_data_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/_feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/eda/_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/format/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/format/_data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/format/_format_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/_data_analysis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/_data_mining_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/_linear_regression_type_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/graph/_logistic_regression_type_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/model/_model_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-04 20:31:19.000000 execdata-5.2.3/execdata/model/_regression_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:31:23.459508 execdata-5.2.3/execdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-04 20:31:23.000000 execdata-5.2.3/execdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 20:31:23.000000 execdata-5.2.3/execdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:31:23.000000 execdata-5.2.3/execdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 20:31:23.000000 execdata-5.2.3/execdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 20:31:19.000000 execdata-5.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:31:23.463508 execdata-5.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 20:31:19.000000 execdata-5.2.3/setup.py
```

### Comparing `execdata-5.2.2/LICENSE` & `execdata-5.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/PKG-INFO` & `execdata-5.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.2.2
+Version: 5.2.3
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.2.2/README.md` & `execdata-5.2.3/README.md`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/__init__.py` & `execdata-5.2.3/execdata/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/eda/__init__.py` & `execdata-5.2.3/execdata/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/eda/_data_mining.py` & `execdata-5.2.3/execdata/eda/_data_mining.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 '''
 Date         : 2023-10-12 14:56:26
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2023-11-13 16:24:05
-LastEditors  : BDFD
+LastEditTime : 2024-04-04 16:28:24
+LastEditors  : <BDFD>
 Description  : 
 FilePath     : \execdata\eda\_data_mining.py
 Copyright (c) 2023 by BDFD, All Rights Reserved. 
 '''
 import numpy as np
 import pandas as pd
 
 
 def high_miss_rate_column(df, missing_rate_column, corresponding_name_column, miss_rate=5):
     # combine use with function[exe.analysis_graph.missing_value_analysis]
     filtered_df = df[df[missing_rate_column] > miss_rate]
     delete_column_name_list = filtered_df[corresponding_name_column].tolist()
     return delete_column_name_list
 
+
 def numerical_features_list(df):
     # list for numerical variables
-    numerical_features_list = [feature for feature in df.columns if df[feature].dtypes != 'O']
+    numerical_features_list = [
+        feature for feature in df.columns if df[feature].dtypes != 'O']
     print('Number of Numerical Variables:', len(numerical_features_list))
 
-    #visualize the numerical variables
+    # visualize the numerical variables
     print(df[numerical_features_list].head())
     return numerical_features_list
 
+
 def categorical_features_list(df):
     # list for categorical variables
-    categorical_features_list = [feature for feature in df.columns if df[feature].dtypes == 'O']
+    categorical_features_list = [
+        feature for feature in df.columns if df[feature].dtypes == 'O']
     print('Number of Categorical Variables:', len(categorical_features_list))
 
-    #visualize the categorical variables
+    # visualize the categorical variables
     print(df[categorical_features_list].head())
     return categorical_features_list
 
 
 def column_identify(df, column_lists):
     column_indentify = {}
     for col in column_lists:
@@ -65,19 +69,19 @@
     majornity_target_value_count = df.loc[df[target_feature] == majornity_target_value].count()[
         0]
     number_of_value = len(df[target_feature].unique())
     data_length = len(df[target_feature])
     target_value_percentage = (majornity_target_value_count/data_length)
     upper_limit = round(data_length/number_of_value*1.3)
     lower_limit = round(data_length/number_of_value*0.7)
-    # print(lower_limit, upper_limit)
+    print('lower limit for one value is', lower_limit,
+          'and upper limit for one value is', upper_limit)
     print('The Dataframe Value Count is:', data_length,
           ', and includes', number_of_value, 'values')
     print('The Majornity Target Value Count is:', majornity_target_value_count)
-    # print('The Majornity Target Value Percentage is:', target_value_percentage)
     print(
         f"Majornity Target Value Percentage: {np.round(target_value_percentage*100,2)}%")
-    if lower_limit <= target_value_percentage <= upper_limit:
+    if lower_limit <= majornity_target_value_count <= upper_limit:
         print("This is a balance dataset.")
     else:
         print("This is a imbalance dataset.")
     return target_value_percentage
```

### Comparing `execdata-5.2.2/execdata/eda/_data_preprocess.py` & `execdata-5.2.3/execdata/eda/_data_preprocess.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/eda/_feature_selection.py` & `execdata-5.2.3/execdata/eda/_feature_selection.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/eda/_standardization.py` & `execdata-5.2.3/execdata/eda/_standardization.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/format/_data_conversion.py` & `execdata-5.2.3/execdata/format/_data_conversion.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/format/_format_data.py` & `execdata-5.2.3/execdata/format/_format_data.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/graph/_data_analysis_graph.py` & `execdata-5.2.3/execdata/graph/_data_analysis_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/graph/_data_mining_graph.py` & `execdata-5.2.3/execdata/graph/_data_mining_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/graph/_linear_regression_type_graph.py` & `execdata-5.2.3/execdata/graph/_linear_regression_type_graph.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/model/_model_evaluate.py` & `execdata-5.2.3/execdata/model/_model_evaluate.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata/model/_regression_model.py` & `execdata-5.2.3/execdata/model/_regression_model.py`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/execdata.egg-info/PKG-INFO` & `execdata-5.2.3/execdata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execdata
-Version: 5.2.2
+Version: 5.2.3
 Summary: Preprocessing dataset
 Home-page: https://github.com/bdfd
 Author: BDFD
 Author-email: bdfd2005@gmail.com
 Project-URL: Bug Tracker, https://github.com/bdfd
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `execdata-5.2.2/execdata.egg-info/SOURCES.txt` & `execdata-5.2.3/execdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `execdata-5.2.2/setup.py` & `execdata-5.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''
 Date         : 2022-10-25 15:44:41
 Author       : BDFD,bdfd2005@gmail.com
 Github       : https://github.com/bdfd
-LastEditTime : 2024-03-14 15:49:59
+LastEditTime : 2024-04-04 16:30:04
 LastEditors  : <BDFD>
 Description  : 
 FilePath     : \setup.py
 Copyright (c) 2022 by BDFD, All Rights Reserved. 
 '''
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-VERSION = '5.2.2'
+VERSION = '5.2.3'
 DESCRIPTION = 'Preprocessing dataset'
 PACKAGE_NAME = 'execdata'
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     author="BDFD",
```

