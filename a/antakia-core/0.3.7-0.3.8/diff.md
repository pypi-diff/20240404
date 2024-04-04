# Comparing `tmp/antakia_core-0.3.7.tar.gz` & `tmp/antakia_core-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antakia_core-0.3.7.tar", max compression
+gzip compressed data, was "antakia_core-0.3.8.tar", max compression
```

## Comparing `antakia_core-0.3.7.tar` & `antakia_core-0.3.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1497 2024-03-19 14:18:22.609303 antakia_core-0.3.7/LICENSE
--rw-r--r--   0        0        0       54 2024-03-19 14:18:22.609385 antakia_core-0.3.7/README.md
--rw-r--r--   0        0        0      667 2024-03-29 14:17:37.357884 antakia_core-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      110 2024-03-19 14:18:22.610283 antakia_core-0.3.7/src/antakia_core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610377 antakia_core-0.3.7/src/antakia_core/compute/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610480 antakia_core-0.3.7/src/antakia_core/compute/dim_reduction/__init__.py
--rw-r--r--   0        0        0     5676 2024-03-29 13:03:55.191432 antakia_core-0.3.7/src/antakia_core/compute/dim_reduction/dim_reduc_method.py
--rw-r--r--   0        0        0     7771 2024-03-29 13:03:55.166286 antakia_core-0.3.7/src/antakia_core/compute/dim_reduction/dim_reduction.py
--rw-r--r--   0        0        0       75 2024-03-22 17:21:14.615326 antakia_core-0.3.7/src/antakia_core/compute/dim_reduction/pacmap_progress/__init__.py
--rw-r--r--   0        0        0    40149 2024-03-22 17:21:15.061170 antakia_core-0.3.7/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py
--rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610898 antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/__init__.py
--rw-r--r--   0        0        0      840 2024-03-21 16:04:55.999992 antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/classification_models.py
--rw-r--r--   0        0        0     3713 2024-03-19 14:18:22.611148 antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/model_class.py
--rw-r--r--   0        0        0     7347 2024-03-21 13:48:10.207887 antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/model_interface.py
--rw-r--r--   0        0        0     1842 2024-03-19 14:18:22.611366 antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/regression_models.py
--rw-r--r--   0        0        0     1702 2024-03-19 14:18:22.611529 antakia_core-0.3.7/src/antakia_core/compute/skope_rule/skope_rule.py
--rw-r--r--   0        0        0      192 2024-03-19 14:18:22.611682 antakia_core-0.3.7/src/antakia_core/data_handler/__init__.py
--rw-r--r--   0        0        0     3968 2024-03-29 13:03:54.732075 antakia_core-0.3.7/src/antakia_core/data_handler/projected_values.py
--rw-r--r--   0        0        0       98 2024-03-19 14:18:22.611895 antakia_core-0.3.7/src/antakia_core/data_handler/region.py
--rw-r--r--   0        0        0     8700 2024-03-21 17:21:13.833477 antakia_core-0.3.7/src/antakia_core/data_handler/region_.py
--rw-r--r--   0        0        0    10471 2024-03-19 15:16:36.155976 antakia_core-0.3.7/src/antakia_core/data_handler/region_set.py
--rw-r--r--   0        0        0     9227 2024-03-19 14:18:22.612332 antakia_core-0.3.7/src/antakia_core/data_handler/rule.py
--rw-r--r--   0        0        0     4176 2024-03-22 13:24:54.198488 antakia_core-0.3.7/src/antakia_core/data_handler/rules.py
--rw-r--r--   0        0        0      190 2024-03-19 14:18:22.612650 antakia_core-0.3.7/src/antakia_core/explanation/__init__.py
--rw-r--r--   0        0        0     2129 2024-03-29 12:59:56.497027 antakia_core-0.3.7/src/antakia_core/explanation/explanation_method.py
--rw-r--r--   0        0        0     4761 2024-03-29 13:03:54.922148 antakia_core-0.3.7/src/antakia_core/explanation/explanations.py
--rw-r--r--   0        0        0      307 2024-03-19 14:18:22.612977 antakia_core-0.3.7/src/antakia_core/utils/__init__.py
--rw-r--r--   0        0        0     1302 2024-03-29 13:06:13.987832 antakia_core-0.3.7/src/antakia_core/utils/long_task.py
--rw-r--r--   0        0        0      548 2024-03-29 13:08:53.274643 antakia_core-0.3.7/src/antakia_core/utils/splittable_callback.py
--rw-r--r--   0        0        0     4322 2024-03-19 14:18:22.613191 antakia_core-0.3.7/src/antakia_core/utils/utils.py
--rw-r--r--   0        0        0     6859 2024-03-29 11:27:00.874984 antakia_core-0.3.7/src/antakia_core/utils/variable.py
--rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 antakia_core-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-03-19 14:18:22.609303 antakia_core-0.3.8/LICENSE
+-rw-r--r--   0        0        0       54 2024-03-19 14:18:22.609385 antakia_core-0.3.8/README.md
+-rw-r--r--   0        0        0      667 2024-04-04 13:38:04.501132 antakia_core-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      110 2024-03-19 14:18:22.610283 antakia_core-0.3.8/src/antakia_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610377 antakia_core-0.3.8/src/antakia_core/compute/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610480 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/__init__.py
+-rw-r--r--   0        0        0     5676 2024-03-29 13:03:55.191432 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/dim_reduc_method.py
+-rw-r--r--   0        0        0     7771 2024-03-29 13:03:55.166286 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/dim_reduction.py
+-rw-r--r--   0        0        0       75 2024-03-22 17:21:14.615326 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/pacmap_progress/__init__.py
+-rw-r--r--   0        0        0    40149 2024-03-22 17:21:15.061170 antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py
+-rw-r--r--   0        0        0        0 2024-03-19 14:18:22.610898 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/__init__.py
+-rw-r--r--   0        0        0      840 2024-03-21 16:04:55.999992 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/classification_models.py
+-rw-r--r--   0        0        0     3713 2024-03-19 14:18:22.611148 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/model_class.py
+-rw-r--r--   0        0        0     7347 2024-03-21 13:48:10.207887 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/model_interface.py
+-rw-r--r--   0        0        0     1842 2024-03-19 14:18:22.611366 antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/regression_models.py
+-rw-r--r--   0        0        0     1702 2024-03-19 14:18:22.611529 antakia_core-0.3.8/src/antakia_core/compute/skope_rule/skope_rule.py
+-rw-r--r--   0        0        0      192 2024-03-19 14:18:22.611682 antakia_core-0.3.8/src/antakia_core/data_handler/__init__.py
+-rw-r--r--   0        0        0     3968 2024-03-29 13:03:54.732075 antakia_core-0.3.8/src/antakia_core/data_handler/projected_values.py
+-rw-r--r--   0        0        0       98 2024-03-19 14:18:22.611895 antakia_core-0.3.8/src/antakia_core/data_handler/region.py
+-rw-r--r--   0        0        0     8700 2024-03-21 17:21:13.833477 antakia_core-0.3.8/src/antakia_core/data_handler/region_.py
+-rw-r--r--   0        0        0    10471 2024-03-19 15:16:36.155976 antakia_core-0.3.8/src/antakia_core/data_handler/region_set.py
+-rw-r--r--   0        0        0     9227 2024-03-19 14:18:22.612332 antakia_core-0.3.8/src/antakia_core/data_handler/rule.py
+-rw-r--r--   0        0        0     4176 2024-03-22 13:24:54.198488 antakia_core-0.3.8/src/antakia_core/data_handler/rules.py
+-rw-r--r--   0        0        0      190 2024-03-19 14:18:22.612650 antakia_core-0.3.8/src/antakia_core/explanation/__init__.py
+-rw-r--r--   0        0        0     2129 2024-03-29 12:59:56.497027 antakia_core-0.3.8/src/antakia_core/explanation/explanation_method.py
+-rw-r--r--   0        0        0     4761 2024-03-29 13:03:54.922148 antakia_core-0.3.8/src/antakia_core/explanation/explanations.py
+-rw-r--r--   0        0        0      307 2024-03-19 14:18:22.612977 antakia_core-0.3.8/src/antakia_core/utils/__init__.py
+-rw-r--r--   0        0        0     1302 2024-03-29 13:06:13.987832 antakia_core-0.3.8/src/antakia_core/utils/long_task.py
+-rw-r--r--   0        0        0      548 2024-03-29 13:08:53.274643 antakia_core-0.3.8/src/antakia_core/utils/splittable_callback.py
+-rw-r--r--   0        0        0     4325 2024-04-04 10:22:26.379728 antakia_core-0.3.8/src/antakia_core/utils/utils.py
+-rw-r--r--   0        0        0     6859 2024-03-29 11:27:00.874984 antakia_core-0.3.8/src/antakia_core/utils/variable.py
+-rw-r--r--   0        0        0      832 1970-01-01 00:00:00.000000 antakia_core-0.3.8/PKG-INFO
```

### Comparing `antakia_core-0.3.7/LICENSE` & `antakia_core-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/pyproject.toml` & `antakia_core-0.3.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antakia-core"
-version = "0.3.7"
+version = "0.3.8"
 description = "Core modules for AntakIA"
 authors = ["Pierre Hulot <pierre@ai-vidence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 pandas = "^2.2.0"
```

### Comparing `antakia_core-0.3.7/src/antakia_core/compute/dim_reduction/dim_reduc_method.py` & `antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/dim_reduc_method.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/compute/dim_reduction/dim_reduction.py` & `antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/dim_reduction.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py` & `antakia_core-0.3.8/src/antakia_core/compute/dim_reduction/pacmap_progress/pacmap_progress.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/classification_models.py` & `antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/classification_models.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/model_class.py` & `antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/model_class.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/model_interface.py` & `antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/model_interface.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/compute/model_subtitution/regression_models.py` & `antakia_core-0.3.8/src/antakia_core/compute/model_subtitution/regression_models.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/compute/skope_rule/skope_rule.py` & `antakia_core-0.3.8/src/antakia_core/compute/skope_rule/skope_rule.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/data_handler/projected_values.py` & `antakia_core-0.3.8/src/antakia_core/data_handler/projected_values.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/data_handler/region_.py` & `antakia_core-0.3.8/src/antakia_core/data_handler/region_.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/data_handler/region_set.py` & `antakia_core-0.3.8/src/antakia_core/data_handler/region_set.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/data_handler/rule.py` & `antakia_core-0.3.8/src/antakia_core/data_handler/rule.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/data_handler/rules.py` & `antakia_core-0.3.8/src/antakia_core/data_handler/rules.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/explanation/explanation_method.py` & `antakia_core-0.3.8/src/antakia_core/explanation/explanation_method.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/explanation/explanations.py` & `antakia_core-0.3.8/src/antakia_core/explanation/explanations.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/utils/long_task.py` & `antakia_core-0.3.8/src/antakia_core/utils/long_task.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/utils/splittable_callback.py` & `antakia_core-0.3.8/src/antakia_core/utils/splittable_callback.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/src/antakia_core/utils/utils.py` & `antakia_core-0.3.8/src/antakia_core/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 def rows_to_mask(X: pd.DataFrame, rows_list: list[int]) -> pd.Series:
     """
     Converts DataFrame row numbers to Index numbers
     """
     mask = boolean_mask(X, False)
-    mask.iloc[rows_list] = 1
+    mask.iloc[rows_list] = True
     return mask.astype(bool)
 
 
 def indexes_to_rows(X: pd.DataFrame, indexes_list: list) -> list:
     """
     Converts DataFrame Index numbers to row numbers
     """
```

### Comparing `antakia_core-0.3.7/src/antakia_core/utils/variable.py` & `antakia_core-0.3.8/src/antakia_core/utils/variable.py`

 * *Files identical despite different names*

### Comparing `antakia_core-0.3.7/PKG-INFO` & `antakia_core-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antakia-core
-Version: 0.3.7
+Version: 0.3.8
 Summary: Core modules for AntakIA
 Author: Pierre Hulot
 Author-email: pierre@ai-vidence.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

