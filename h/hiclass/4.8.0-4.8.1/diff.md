# Comparing `tmp/hiclass-4.8.0.tar.gz` & `tmp/hiclass-4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiclass-4.8.0.tar", last modified: Wed Mar 27 13:34:58 2024, max compression
+gzip compressed data, was "hiclass-4.8.1.tar", last modified: Thu Apr  4 11:01:05 2024, max compression
```

## Comparing `hiclass-4.8.0.tar` & `hiclass-4.8.1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:34:58.818503 hiclass-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-27 13:34:39.000000 hiclass-4.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 13:34:39.000000 hiclass-4.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-03-27 13:34:58.818503 hiclass-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-03-27 13:34:39.000000 hiclass-4.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:34:58.818503 hiclass-4.8.0/hiclass/
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/BinaryPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/ConstantClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/Explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/HierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/LocalClassifierPerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/LocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/LocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    16260 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/MultiLabelHierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/MultiLabelLocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/MultiLabelLocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-27 13:34:58.818503 hiclass-4.8.0/hiclass/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-03-27 13:34:39.000000 hiclass-4.8.0/hiclass/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:34:58.814504 hiclass-4.8.0/hiclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-03-27 13:34:58.000000 hiclass-4.8.0/hiclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-27 13:34:58.000000 hiclass-4.8.0/hiclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:34:58.000000 hiclass-4.8.0/hiclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-27 13:34:58.000000 hiclass-4.8.0/hiclass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-27 13:34:58.000000 hiclass-4.8.0/hiclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 13:34:58.000000 hiclass-4.8.0/hiclass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-27 13:34:58.818503 hiclass-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-27 13:34:39.000000 hiclass-4.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:34:58.814504 hiclass-4.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29992 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_BinaryPolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_ConstantClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_Explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_HierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_LocalClassifierPerLevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_LocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_LocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_LocalClassifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_MultiLabelHierarchicalClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_MultiLabelLocalClassifierPerNode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12129 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_MultiLabelLocalClassifierPerParentNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-03-27 13:34:39.000000 hiclass-4.8.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-03-27 13:34:39.000000 hiclass-4.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:01:05.905362 hiclass-4.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-04 11:00:51.000000 hiclass-4.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 11:00:51.000000 hiclass-4.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-04-04 11:01:05.905362 hiclass-4.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-04 11:00:51.000000 hiclass-4.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:01:05.905362 hiclass-4.8.1/hiclass/
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/BinaryPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/ConstantClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10386 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/Explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/HierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/LocalClassifierPerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/LocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8943 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/LocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16260 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/MultiLabelHierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/MultiLabelLocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/MultiLabelLocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 11:01:05.905362 hiclass-4.8.1/hiclass/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-04-04 11:00:51.000000 hiclass-4.8.1/hiclass/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:01:05.905362 hiclass-4.8.1/hiclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17758 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 11:01:05.000000 hiclass-4.8.1/hiclass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 11:01:05.905362 hiclass-4.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-04 11:00:51.000000 hiclass-4.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:01:05.905362 hiclass-4.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29992 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_BinaryPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_ConstantClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_Datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4924 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_Explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_HierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_LocalClassifierPerLevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_LocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_LocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_LocalClassifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_MultiLabelHierarchicalClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_MultiLabelLocalClassifierPerNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12129 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_MultiLabelLocalClassifierPerParentNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-04 11:00:51.000000 hiclass-4.8.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-04-04 11:00:51.000000 hiclass-4.8.1/versioneer.py
```

### Comparing `hiclass-4.8.0/LICENSE` & `hiclass-4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/PKG-INFO` & `hiclass-4.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclass
-Version: 4.8.0
+Version: 4.8.1
 Summary: Hierarchical Classification Library.
 Author: Fabio Malcher Miranda, Niklas Koehnecke
 Author-email: fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/hiclass/issues
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/hiclass
 Project-URL: Related Software, https://gitlab.com/dacs-hpi
```

### Comparing `hiclass-4.8.0/README.md` & `hiclass-4.8.1/README.md`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/BinaryPolicy.py` & `hiclass-4.8.1/hiclass/BinaryPolicy.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/ConstantClassifier.py` & `hiclass-4.8.1/hiclass/ConstantClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/Explainer.py` & `hiclass-4.8.1/hiclass/Explainer.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/HierarchicalClassifier.py` & `hiclass-4.8.1/hiclass/HierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/LocalClassifierPerLevel.py` & `hiclass-4.8.1/hiclass/LocalClassifierPerLevel.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/LocalClassifierPerNode.py` & `hiclass-4.8.1/hiclass/LocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/LocalClassifierPerParentNode.py` & `hiclass-4.8.1/hiclass/LocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/MultiLabelHierarchicalClassifier.py` & `hiclass-4.8.1/hiclass/MultiLabelHierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/MultiLabelLocalClassifierPerNode.py` & `hiclass-4.8.1/hiclass/MultiLabelLocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/MultiLabelLocalClassifierPerParentNode.py` & `hiclass-4.8.1/hiclass/MultiLabelLocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass/__init__.py` & `hiclass-4.8.1/hiclass/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 __all__ = [
     "LocalClassifierPerNode",
     "LocalClassifierPerParentNode",
     "LocalClassifierPerLevel",
     "Explainer",
     "MultiLabelLocalClassifierPerNode",
     "MultiLabelLocalClassifierPerParentNode",
+    "datasets",
 ]
```

### Comparing `hiclass-4.8.0/hiclass/metrics.py` & `hiclass-4.8.1/hiclass/metrics.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/hiclass.egg-info/PKG-INFO` & `hiclass-4.8.1/hiclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiclass
-Version: 4.8.0
+Version: 4.8.1
 Summary: Hierarchical Classification Library.
 Author: Fabio Malcher Miranda, Niklas Koehnecke
 Author-email: fabio.malchermiranda@hpi.de, Niklas.Koehnecke@student.hpi.uni-potsdam.de
 License: BSD 3-Clause
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/hiclass/issues
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/hiclass
 Project-URL: Related Software, https://gitlab.com/dacs-hpi
```

### Comparing `hiclass-4.8.0/hiclass.egg-info/SOURCES.txt` & `hiclass-4.8.1/hiclass.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 hiclass/LocalClassifierPerNode.py
 hiclass/LocalClassifierPerParentNode.py
 hiclass/MultiLabelHierarchicalClassifier.py
 hiclass/MultiLabelLocalClassifierPerNode.py
 hiclass/MultiLabelLocalClassifierPerParentNode.py
 hiclass/__init__.py
 hiclass/_version.py
+hiclass/datasets.py
 hiclass/metrics.py
 hiclass.egg-info/PKG-INFO
 hiclass.egg-info/SOURCES.txt
 hiclass.egg-info/dependency_links.txt
 hiclass.egg-info/entry_points.txt
 hiclass.egg-info/requires.txt
 hiclass.egg-info/top_level.txt
 tests/test_BinaryPolicy.py
 tests/test_ConstantClassifier.py
+tests/test_Datasets.py
 tests/test_Explainer.py
 tests/test_HierarchicalClassifier.py
 tests/test_LocalClassifierPerLevel.py
 tests/test_LocalClassifierPerNode.py
 tests/test_LocalClassifierPerParentNode.py
 tests/test_LocalClassifiers.py
 tests/test_MultiLabelHierarchicalClassifier.py
```

### Comparing `hiclass-4.8.0/setup.py` & `hiclass-4.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_BinaryPolicy.py` & `hiclass-4.8.1/tests/test_BinaryPolicy.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_ConstantClassifier.py` & `hiclass-4.8.1/tests/test_ConstantClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_Explainer.py` & `hiclass-4.8.1/tests/test_Explainer.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_HierarchicalClassifier.py` & `hiclass-4.8.1/tests/test_HierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_LocalClassifierPerLevel.py` & `hiclass-4.8.1/tests/test_LocalClassifierPerLevel.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_LocalClassifierPerNode.py` & `hiclass-4.8.1/tests/test_LocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_LocalClassifierPerParentNode.py` & `hiclass-4.8.1/tests/test_LocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_LocalClassifiers.py` & `hiclass-4.8.1/tests/test_LocalClassifiers.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_MultiLabelHierarchicalClassifier.py` & `hiclass-4.8.1/tests/test_MultiLabelHierarchicalClassifier.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_MultiLabelLocalClassifierPerNode.py` & `hiclass-4.8.1/tests/test_MultiLabelLocalClassifierPerNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_MultiLabelLocalClassifierPerParentNode.py` & `hiclass-4.8.1/tests/test_MultiLabelLocalClassifierPerParentNode.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/tests/test_metrics.py` & `hiclass-4.8.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hiclass-4.8.0/versioneer.py` & `hiclass-4.8.1/versioneer.py`

 * *Files identical despite different names*

