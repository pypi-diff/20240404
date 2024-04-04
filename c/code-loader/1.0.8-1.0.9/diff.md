# Comparing `tmp/code_loader-1.0.8.tar.gz` & `tmp/code_loader-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_loader-1.0.8.tar", max compression
+gzip compressed data, was "code_loader-1.0.9.tar", max compression
```

## Comparing `code_loader-1.0.8.tar` & `code_loader-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-08-22 13:21:37.210207 code_loader-1.0.8/LICENSE
--rw-r--r--   0        0        0       63 2023-08-22 13:21:37.210317 code_loader-1.0.8/README.md
--rw-r--r--   0        0        0      122 2023-08-22 13:21:37.210852 code_loader-1.0.8/code_loader/__init__.py
--rw-r--r--   0        0        0        0 2023-08-22 13:21:37.210953 code_loader-1.0.8/code_loader/contract/__init__.py
--rw-r--r--   0        0        0     4527 2023-08-22 13:21:37.211283 code_loader-1.0.8/code_loader/contract/datasetclasses.py
--rw-r--r--   0        0        0     1481 2023-08-22 13:21:37.211493 code_loader-1.0.8/code_loader/contract/enums.py
--rw-r--r--   0        0        0       51 2023-08-22 13:21:37.211682 code_loader-1.0.8/code_loader/contract/exceptions.py
--rw-r--r--   0        0        0     2658 2023-08-23 15:48:34.112699 code_loader-1.0.8/code_loader/contract/responsedataclasses.py
--rw-r--r--   0        0        0     5138 2023-08-23 15:51:29.825585 code_loader-1.0.8/code_loader/contract/visualizer_classes.py
--rw-r--r--   0        0        0       99 2023-08-22 13:21:37.212735 code_loader-1.0.8/code_loader/inner_leap_binder/__init__.py
--rw-r--r--   0        0        0    12853 2023-08-23 16:04:20.446230 code_loader-1.0.8/code_loader/inner_leap_binder/leapbinder.py
--rw-r--r--   0        0        0     4758 2023-08-22 13:21:37.213285 code_loader-1.0.8/code_loader/leap_loader_parallelized_base.py
--rw-r--r--   0        0        0    15424 2023-08-23 15:51:19.946039 code_loader-1.0.8/code_loader/leaploader.py
--rw-r--r--   0        0        0     2181 2023-08-22 13:21:37.213919 code_loader-1.0.8/code_loader/metric_calculator_parallelized.py
--rw-r--r--   0        0        0        0 2023-08-22 13:21:37.214026 code_loader-1.0.8/code_loader/metrics/__init__.py
--rw-r--r--   0        0        0     6727 2023-08-22 13:21:37.214204 code_loader-1.0.8/code_loader/metrics/default_metrics.py
--rw-r--r--   0        0        0     2376 2023-08-22 13:21:37.214476 code_loader-1.0.8/code_loader/samples_generator_parallelized.py
--rw-r--r--   0        0        0     1736 2023-08-22 13:21:37.214679 code_loader-1.0.8/code_loader/utils.py
--rw-r--r--   0        0        0     2523 2023-08-22 13:21:37.214895 code_loader-1.0.8/code_loader/visualizer_calculator_parallelized.py
--rw-r--r--   0        0        0        0 2023-08-22 13:21:37.214984 code_loader-1.0.8/code_loader/visualizers/__init__.py
--rw-r--r--   0        0        0     2226 2023-08-22 13:21:37.215191 code_loader-1.0.8/code_loader/visualizers/default_visualizers.py
--rw-r--r--   0        0        0      876 2023-08-23 16:06:37.651619 code_loader-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 code_loader-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-22 09:30:01.871991 code_loader-1.0.9/LICENSE
+-rw-r--r--   0        0        0       63 2023-08-22 09:30:01.872129 code_loader-1.0.9/README.md
+-rw-r--r--   0        0        0      122 2023-08-22 09:30:01.872353 code_loader-1.0.9/code_loader/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-22 09:30:01.872478 code_loader-1.0.9/code_loader/contract/__init__.py
+-rw-r--r--   0        0        0     4527 2023-08-22 09:30:01.872614 code_loader-1.0.9/code_loader/contract/datasetclasses.py
+-rw-r--r--   0        0        0     1481 2023-08-22 09:30:01.872742 code_loader-1.0.9/code_loader/contract/enums.py
+-rw-r--r--   0        0        0       51 2023-08-22 09:30:01.873397 code_loader-1.0.9/code_loader/contract/exceptions.py
+-rw-r--r--   0        0        0     2658 2023-08-28 16:11:11.909186 code_loader-1.0.9/code_loader/contract/responsedataclasses.py
+-rw-r--r--   0        0        0     5138 2023-08-28 16:11:11.909841 code_loader-1.0.9/code_loader/contract/visualizer_classes.py
+-rw-r--r--   0        0        0       99 2023-08-22 09:30:01.875408 code_loader-1.0.9/code_loader/inner_leap_binder/__init__.py
+-rw-r--r--   0        0        0    12883 2023-08-28 16:11:25.900115 code_loader-1.0.9/code_loader/inner_leap_binder/leapbinder.py
+-rw-r--r--   0        0        0     4758 2023-08-22 09:30:01.877156 code_loader-1.0.9/code_loader/leap_loader_parallelized_base.py
+-rw-r--r--   0        0        0    15424 2023-08-28 16:11:11.911137 code_loader-1.0.9/code_loader/leaploader.py
+-rw-r--r--   0        0        0     2181 2023-08-22 09:30:01.879178 code_loader-1.0.9/code_loader/metric_calculator_parallelized.py
+-rw-r--r--   0        0        0        0 2023-08-22 09:30:01.879494 code_loader-1.0.9/code_loader/metrics/__init__.py
+-rw-r--r--   0        0        0     6727 2023-08-22 09:30:01.880644 code_loader-1.0.9/code_loader/metrics/default_metrics.py
+-rw-r--r--   0        0        0     2376 2023-08-22 09:30:01.881295 code_loader-1.0.9/code_loader/samples_generator_parallelized.py
+-rw-r--r--   0        0        0     1736 2023-08-22 09:30:01.882229 code_loader-1.0.9/code_loader/utils.py
+-rw-r--r--   0        0        0     2523 2023-08-22 15:31:15.990204 code_loader-1.0.9/code_loader/visualizer_calculator_parallelized.py
+-rw-r--r--   0        0        0        0 2023-08-22 09:30:01.883099 code_loader-1.0.9/code_loader/visualizers/__init__.py
+-rw-r--r--   0        0        0     2226 2023-08-22 09:30:01.883772 code_loader-1.0.9/code_loader/visualizers/default_visualizers.py
+-rw-r--r--   0        0        0      876 2023-08-28 16:12:01.774758 code_loader-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 code_loader-1.0.9/PKG-INFO
```

### Comparing `code_loader-1.0.8/LICENSE` & `code_loader-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/contract/datasetclasses.py` & `code_loader-1.0.9/code_loader/contract/datasetclasses.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/contract/enums.py` & `code_loader-1.0.9/code_loader/contract/enums.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/contract/responsedataclasses.py` & `code_loader-1.0.9/code_loader/contract/responsedataclasses.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/contract/visualizer_classes.py` & `code_loader-1.0.9/code_loader/contract/visualizer_classes.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/inner_leap_binder/leapbinder.py` & `code_loader-1.0.9/code_loader/inner_leap_binder/leapbinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,7 +221,9 @@
                     continue
                 self.check_handler(preprocess_response, test_result, dataset_base_handler)
 
     def check(self) -> None:
         preprocess_result = self.get_preprocess_result()
         self.check_preprocess(preprocess_result)
         self.check_handlers(preprocess_result)
+        print("Successful!")
+
```

### Comparing `code_loader-1.0.8/code_loader/leap_loader_parallelized_base.py` & `code_loader-1.0.9/code_loader/leap_loader_parallelized_base.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/leaploader.py` & `code_loader-1.0.9/code_loader/leaploader.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/metric_calculator_parallelized.py` & `code_loader-1.0.9/code_loader/metric_calculator_parallelized.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/metrics/default_metrics.py` & `code_loader-1.0.9/code_loader/metrics/default_metrics.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/samples_generator_parallelized.py` & `code_loader-1.0.9/code_loader/samples_generator_parallelized.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/utils.py` & `code_loader-1.0.9/code_loader/utils.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/visualizer_calculator_parallelized.py` & `code_loader-1.0.9/code_loader/visualizer_calculator_parallelized.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/code_loader/visualizers/default_visualizers.py` & `code_loader-1.0.9/code_loader/visualizers/default_visualizers.py`

 * *Files identical despite different names*

### Comparing `code_loader-1.0.8/pyproject.toml` & `code_loader-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "code-loader"
-version = "1.0.8"
+version = "1.0.9"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/code-loader"
 homepage = "https://github.com/tensorleap/code-loader"
 include = [
```

### Comparing `code_loader-1.0.8/PKG-INFO` & `code_loader-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-loader
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Home-page: https://github.com/tensorleap/code-loader
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

