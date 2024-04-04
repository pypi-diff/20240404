# Comparing `tmp/pre5g-0.96.tar.gz` & `tmp/pre5g-0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-0.96.tar", last modified: Wed Apr  3 10:27:11 2024, max compression
+gzip compressed data, was "dist/pre5g-0.97.tar", last modified: Thu Apr  4 03:42:26 2024, max compression
```

## Comparing `pre5g-0.96.tar` & `pre5g-0.97.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-03 10:27:11.656141 pre5g-0.96/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.96/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-03 10:27:11.655141 pre5g-0.96/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.96/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-03 10:27:11.653141 pre5g-0.96/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      752 2024-04-03 10:26:39.000000 pre5g-0.96/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1625 2024-04-02 05:38:57.000000 pre5g-0.96/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-0.96/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1196 2024-04-03 10:26:05.000000 pre5g-0.96/pre5g/nullvalue.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1589 2024-04-02 05:34:03.000000 pre5g-0.96/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.96/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-0.96/pre5g/standardization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     4487 2024-04-03 05:36:40.000000 pre5g-0.96/pre5g/winsorization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-03 10:27:11.655141 pre5g-0.96/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-03 10:27:11.000000 pre5g-0.96/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-03 10:27:11.000000 pre5g-0.96/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-03 10:27:11.000000 pre5g-0.96/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-03 10:27:11.000000 pre5g-0.96/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-03 10:27:11.656141 pre5g-0.96/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      602 2024-04-03 10:26:43.000000 pre5g-0.96/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 03:42:26.885686 pre5g-0.97/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-0.97/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-04 03:42:26.885686 pre5g-0.97/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-0.97/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 03:42:26.879686 pre5g-0.97/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      817 2024-04-04 03:42:18.000000 pre5g-0.97/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1625 2024-04-02 05:38:57.000000 pre5g-0.97/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-0.97/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1745 2024-04-04 03:41:14.000000 pre5g-0.97/pre5g/nullvalue.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1589 2024-04-02 05:34:03.000000 pre5g-0.97/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2679 2024-04-01 11:29:12.000000 pre5g-0.97/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-0.97/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     4487 2024-04-03 05:36:40.000000 pre5g-0.97/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-04 03:42:26.884686 pre5g-0.97/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      492 2024-04-04 03:42:26.000000 pre5g-0.97/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-04 03:42:26.000000 pre5g-0.97/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-04 03:42:26.000000 pre5g-0.97/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-04 03:42:26.000000 pre5g-0.97/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-04 03:42:26.885686 pre5g-0.97/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      602 2024-04-04 03:41:32.000000 pre5g-0.97/setup.py
```

### Comparing `pre5g-0.96/LICENSE` & `pre5g-0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-0.96/pre5g/__init__.py` & `pre5g-0.97/pre5g/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,8 +5,9 @@
 from .robustscaler import rs_all
 from .robustscaler import rs_selected_columns
 # from .labelen import label_encoding_all
 from .labelen import label_encoding_selected
 # from .onehoten import one_hot_encoding_all
 from .onehoten import one_hot_encoding_selected
 from .nullvalue import drop_null_values_from_selected_columns
-__all__ = ['normalize_all','normalize_selected_columns','standardize_all','standardize_selected_columns','rs_all','rs_selected_columns','label_encoding_selected','one_hot_encoding_selected','drop_null_values_from_selected_columns']
+from .nullvalue import fill_null_with_mean
+__all__ = ['normalize_all','normalize_selected_columns','standardize_all','standardize_selected_columns','rs_all','rs_selected_columns','label_encoding_selected','one_hot_encoding_selected','drop_null_values_from_selected_columns','fill_null_with_mean']
```

### Comparing `pre5g-0.96/pre5g/labelen.py` & `pre5g-0.97/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.96/pre5g/normalization.py` & `pre5g-0.97/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.96/pre5g/onehoten.py` & `pre5g-0.97/pre5g/onehoten.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.96/pre5g/robustscaler.py` & `pre5g-0.97/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.96/pre5g/standardization.py` & `pre5g-0.97/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.96/pre5g/winsorization.py` & `pre5g-0.97/pre5g/winsorization.py`

 * *Files identical despite different names*

### Comparing `pre5g-0.96/setup.py` & `pre5g-0.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='0.96',
+    version='0.97',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

