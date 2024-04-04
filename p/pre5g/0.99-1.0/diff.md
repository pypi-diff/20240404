# Comparing `tmp/pre5g-0.99.tar.gz` & `tmp/pre5g-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-0.99.tar", last modified: Thu Apr  4 10:32:43 2024, max compression
+gzip compressed data, was "dist/pre5g-1.0.tar", last modified: Thu Apr  4 11:17:09 2024, max compression
```

## Comparing `pre5g-0.99.tar` & `pre5g-1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 10:32:43.576794 pre5g-0.99/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.99/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-04 10:32:43.576794 pre5g-0.99/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.99/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 10:32:43.567794 pre5g-0.99/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1141 2024-04-04 10:32:03.000000 pre5g-0.99/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1625 2024-04-02 05:38:57.000000 pre5g-0.99/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-0.99/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     4176 2024-04-04 10:32:21.000000 pre5g-0.99/pre5g/nullvalue.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1589 2024-04-02 05:34:03.000000 pre5g-0.99/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.99/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-0.99/pre5g/standardization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     4487 2024-04-03 05:36:40.000000 pre5g-0.99/pre5g/winsorization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 10:32:43.575794 pre5g-0.99/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-04 10:32:43.000000 pre5g-0.99/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-04 10:32:43.000000 pre5g-0.99/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-04 10:32:43.000000 pre5g-0.99/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-04 10:32:43.000000 pre5g-0.99/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-04 10:32:43.576794 pre5g-0.99/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      602 2024-04-04 10:32:27.000000 pre5g-0.99/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 11:17:09.049505 pre5g-1.0/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-1.0/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-04 11:17:09.049505 pre5g-1.0/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-1.0/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 11:17:09.047505 pre5g-1.0/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-1.0/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1625 2024-04-02 05:38:57.000000 pre5g-1.0/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-1.0/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     4305 2024-04-04 11:14:21.000000 pre5g-1.0/pre5g/nullvalue.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1589 2024-04-02 05:34:03.000000 pre5g-1.0/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-1.0/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-1.0/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     4487 2024-04-03 05:36:40.000000 pre5g-1.0/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 11:17:09.048505 pre5g-1.0/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-04 11:17:08.000000 pre5g-1.0/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-04 11:17:09.000000 pre5g-1.0/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-04 11:17:08.000000 pre5g-1.0/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-04 11:17:08.000000 pre5g-1.0/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-04 11:17:09.049505 pre5g-1.0/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      601 2024-04-04 11:14:59.000000 pre5g-1.0/setup.py
```

### Comparing `pre5g-0.99/LICENSE` & `pre5g-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-0.99/pre5g/__init__.py` & `pre5g-1.0/pre5g/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 from .labelen import label_encoding_selected
 # from .onehoten import one_hot_encoding_all
 from .onehoten import one_hot_encoding_selected
 from .nullvalue import drop_null_values_from_selected_columns
 from .nullvalue import fill_null_with_mean
 from .nullvalue import fill_null_with_mode
 from .nullvalue import fill_null_with_median
-from .nullvalue import drop_duplicates_selected_rows
+from .nullvalue import drop_duplicates_all_columns
 from .nullvalue import remove_duplicates_from_specific_columns
-__all__ = ['normalize_all','normalize_selected_columns','standardize_all','standardize_selected_columns','rs_all','rs_selected_columns','label_encoding_selected','one_hot_encoding_selected','drop_null_values_from_selected_columns','fill_null_with_mean','fill_null_with_mode','fill_null_with_median','drop_duplicates_selected_rows','remove_duplicates_from_specific_columns']
+__all__ = ['normalize_all','normalize_selected_columns','standardize_all','standardize_selected_columns','rs_all','rs_selected_columns','label_encoding_selected','one_hot_encoding_selected','drop_null_values_from_selected_columns','fill_null_with_mean','fill_null_with_mode','fill_null_with_median','drop_duplicates_all_columns','remove_duplicates_from_specific_columns']
```

### Comparing `pre5g-0.99/pre5g/labelen.py` & `pre5g-1.0/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.99/pre5g/normalization.py` & `pre5g-1.0/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.99/pre5g/nullvalue.py` & `pre5g-1.0/pre5g/nullvalue.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,28 +89,32 @@
 
 import pandas as pd
 
 
 
 
 
-def drop_duplicates_selected_rows(data, selected_columns):
+def drop_duplicates_all_columns(data):
+    """
+    Remove duplicate rows from a list of lists representing tabular data.
+    :param data: List of lists representing the data
+    :return: List of lists with duplicate rows removed
+    """
     # Convert input data to DataFrame
-    df = pd.DataFrame(data, columns=selected_columns)
+    df = pd.DataFrame(data)
     
-    # Drop duplicates based on selected columns
+    # Drop duplicate rows
     df.drop_duplicates(inplace=True)
     
     # Convert DataFrame back to list of lists
     cleaned_data = df.values.tolist()
     
     return cleaned_data
 
 
-
 def remove_duplicates_from_specific_columns(data, columns):
     """
     Remove duplicate values from specific columns of a list of lists.
     :param data: List of lists representing the data
     :param columns: List of column indices to remove duplicates from
     :return: List of lists with duplicates removed from specified columns
     """
```

### Comparing `pre5g-0.99/pre5g/onehoten.py` & `pre5g-1.0/pre5g/onehoten.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.99/pre5g/robustscaler.py` & `pre5g-1.0/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.99/pre5g/standardization.py` & `pre5g-1.0/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.99/pre5g/winsorization.py` & `pre5g-1.0/pre5g/winsorization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.99/setup.py` & `pre5g-1.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='0.99',
+    version='1.0',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

