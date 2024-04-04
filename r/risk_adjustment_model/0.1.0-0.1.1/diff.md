# Comparing `tmp/risk_adjustment_model-0.1.0.tar.gz` & `tmp/risk_adjustment_model-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risk_adjustment_model-0.1.0.tar", max compression
+gzip compressed data, was "risk_adjustment_model-0.1.1.tar", max compression
```

## Comparing `risk_adjustment_model-0.1.0.tar` & `risk_adjustment_model-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1094 2024-03-02 18:04:38.539534 risk_adjustment_model-0.1.0/LICENSE
--rw-r--r--   0        0        0      576 2024-03-21 14:31:59.337543 risk_adjustment_model-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10787 2024-04-02 20:47:40.483931 risk_adjustment_model-0.1.0/README.md
--rw-r--r--   0        0        0      124 2024-04-02 20:46:05.407274 risk_adjustment_model-0.1.0/src/risk_adjustment_model/__init__.py
--rw-r--r--   0        0        0    10100 2024-04-02 20:46:05.409274 risk_adjustment_model-0.1.0/src/risk_adjustment_model/beneficiary.py
--rw-r--r--   0        0        0     3954 2024-04-02 20:46:05.409274 risk_adjustment_model-0.1.0/src/risk_adjustment_model/category.py
--rw-r--r--   0        0        0     3588 2024-04-02 20:46:05.410262 risk_adjustment_model-0.1.0/src/risk_adjustment_model/mapper.py
--rw-r--r--   0        0        0    23137 2024-04-02 20:46:05.410262 risk_adjustment_model-0.1.0/src/risk_adjustment_model/model.py
--rw-r--r--   0        0        0    15860 2024-03-26 15:37:03.243867 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2020/category_definition.json
--rw-r--r--   0        0        0   111168 2024-03-27 17:32:32.461025 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2020/diag_to_category_map.txt
--rw-r--r--   0        0        0     2511 2024-03-06 14:30:03.176261 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2020/hierarchy_definition.json
--rw-r--r--   0        0        0     9090 2024-03-21 18:41:48.637640 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2020/weights.csv
--rw-r--r--   0        0        0    15860 2024-03-26 15:37:03.245862 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2021/category_definition.json
--rw-r--r--   0        0        0   112256 2024-03-27 17:20:57.856254 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2021/diag_to_category_map.txt
--rw-r--r--   0        0        0     2513 2024-03-26 15:37:03.247857 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2021/hierarchy_definition.json
--rw-r--r--   0        0        0     9090 2024-03-26 15:37:03.248857 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2021/weights.csv
--rw-r--r--   0        0        0    15860 2024-03-26 15:37:03.249855 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2022/category_definition.json
--rw-r--r--   0        0        0   112447 2024-03-27 17:20:56.311661 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2022/diag_to_category_map.txt
--rw-r--r--   0        0        0     2513 2024-03-26 15:37:03.251849 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2022/hierarchy_definition.json
--rw-r--r--   0        0        0     9090 2024-03-26 15:37:03.251849 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2022/weights.csv
--rw-r--r--   0        0        0    15860 2024-03-26 15:37:03.252847 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2023/category_definition.json
--rw-r--r--   0        0        0   114703 2024-03-27 17:20:54.335063 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2023/diag_to_category_map.txt
--rw-r--r--   0        0        0     2513 2024-03-26 15:37:03.254841 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2023/hierarchy_definition.json
--rw-r--r--   0        0        0     9090 2024-03-26 15:37:03.254841 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2023/weights.csv
--rw-r--r--   0        0        0    15858 2024-03-06 19:19:09.352563 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2024/category_definition.json
--rw-r--r--   0        0        0   114727 2024-04-02 20:46:05.412255 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2024/diag_to_category_map.txt
--rw-r--r--   0        0        0     2511 2024-03-06 14:30:03.185237 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2024/hierarchy_definition.json
--rw-r--r--   0        0        0     9090 2024-03-21 18:41:48.638638 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2024/weights.csv
--rw-r--r--   0        0        0    18362 2024-03-26 15:37:03.256832 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v28/2024/category_definition.json
--rw-r--r--   0        0        0    92489 2024-03-26 15:37:03.257830 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v28/2024/diag_to_category_map.txt
--rw-r--r--   0        0        0     4417 2024-03-06 19:19:09.354558 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v28/2024/hierarchy_definition.json
--rw-r--r--   0        0        0    14676 2024-03-06 19:19:09.355555 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v28/2024/weights.csv
--rw-r--r--   0        0        0     7309 2024-04-02 20:46:05.412255 risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_files_loader.py
--rw-r--r--   0        0        0     2763 2024-04-02 20:46:05.413252 risk_adjustment_model-0.1.0/src/risk_adjustment_model/result.py
--rw-r--r--   0        0        0     1344 2024-04-02 20:46:05.413252 risk_adjustment_model-0.1.0/src/risk_adjustment_model/utilities.py
--rw-r--r--   0        0        0    13289 2024-04-02 20:46:05.414249 risk_adjustment_model-0.1.0/src/risk_adjustment_model/v24.py
--rw-r--r--   0        0        0    17300 2024-04-02 20:46:05.414249 risk_adjustment_model-0.1.0/src/risk_adjustment_model/v28.py
--rw-r--r--   0        0        0    11006 1970-01-01 00:00:00.000000 risk_adjustment_model-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-03-02 18:04:38.539534 risk_adjustment_model-0.1.1/LICENSE
+-rw-r--r--   0        0        0      578 2024-04-04 20:42:39.645772 risk_adjustment_model-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10787 2024-04-04 16:26:46.174119 risk_adjustment_model-0.1.1/README.md
+-rw-r--r--   0        0        0      124 2024-04-02 20:46:05.407274 risk_adjustment_model-0.1.1/src/risk_adjustment_model/__init__.py
+-rw-r--r--   0        0        0    10100 2024-04-02 20:46:05.409274 risk_adjustment_model-0.1.1/src/risk_adjustment_model/beneficiary.py
+-rw-r--r--   0        0        0     3954 2024-04-02 20:46:05.409274 risk_adjustment_model-0.1.1/src/risk_adjustment_model/category.py
+-rw-r--r--   0        0        0     3588 2024-04-02 20:46:05.410262 risk_adjustment_model-0.1.1/src/risk_adjustment_model/mapper.py
+-rw-r--r--   0        0        0    23137 2024-04-02 20:46:05.410262 risk_adjustment_model-0.1.1/src/risk_adjustment_model/model.py
+-rw-r--r--   0        0        0    15860 2024-03-26 15:37:03.243867 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2020/category_definition.json
+-rw-r--r--   0        0        0   111168 2024-03-27 17:32:32.461025 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2020/diag_to_category_map.txt
+-rw-r--r--   0        0        0     2511 2024-03-06 14:30:03.176261 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2020/hierarchy_definition.json
+-rw-r--r--   0        0        0     9090 2024-03-21 18:41:48.637640 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2020/weights.csv
+-rw-r--r--   0        0        0    15860 2024-03-26 15:37:03.245862 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2021/category_definition.json
+-rw-r--r--   0        0        0   112256 2024-03-27 17:20:57.856254 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2021/diag_to_category_map.txt
+-rw-r--r--   0        0        0     2513 2024-03-26 15:37:03.247857 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2021/hierarchy_definition.json
+-rw-r--r--   0        0        0     9090 2024-03-26 15:37:03.248857 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2021/weights.csv
+-rw-r--r--   0        0        0    15860 2024-03-26 15:37:03.249855 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2022/category_definition.json
+-rw-r--r--   0        0        0   112447 2024-03-27 17:20:56.311661 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2022/diag_to_category_map.txt
+-rw-r--r--   0        0        0     2513 2024-03-26 15:37:03.251849 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2022/hierarchy_definition.json
+-rw-r--r--   0        0        0     9090 2024-03-26 15:37:03.251849 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2022/weights.csv
+-rw-r--r--   0        0        0    15860 2024-03-26 15:37:03.252847 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2023/category_definition.json
+-rw-r--r--   0        0        0   114703 2024-03-27 17:20:54.335063 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2023/diag_to_category_map.txt
+-rw-r--r--   0        0        0     2513 2024-03-26 15:37:03.254841 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2023/hierarchy_definition.json
+-rw-r--r--   0        0        0     9090 2024-03-26 15:37:03.254841 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2023/weights.csv
+-rw-r--r--   0        0        0    15858 2024-03-06 19:19:09.352563 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2024/category_definition.json
+-rw-r--r--   0        0        0   114727 2024-04-02 20:46:05.412255 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2024/diag_to_category_map.txt
+-rw-r--r--   0        0        0     2511 2024-03-06 14:30:03.185237 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2024/hierarchy_definition.json
+-rw-r--r--   0        0        0     9090 2024-03-21 18:41:48.638638 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2024/weights.csv
+-rw-r--r--   0        0        0    18362 2024-03-26 15:37:03.256832 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v28/2024/category_definition.json
+-rw-r--r--   0        0        0    92489 2024-03-26 15:37:03.257830 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v28/2024/diag_to_category_map.txt
+-rw-r--r--   0        0        0     4417 2024-03-06 19:19:09.354558 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v28/2024/hierarchy_definition.json
+-rw-r--r--   0        0        0    14676 2024-03-06 19:19:09.355555 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v28/2024/weights.csv
+-rw-r--r--   0        0        0     7309 2024-04-02 20:46:05.412255 risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_files_loader.py
+-rw-r--r--   0        0        0     2763 2024-04-02 20:46:05.413252 risk_adjustment_model-0.1.1/src/risk_adjustment_model/result.py
+-rw-r--r--   0        0        0     1344 2024-04-02 20:46:05.413252 risk_adjustment_model-0.1.1/src/risk_adjustment_model/utilities.py
+-rw-r--r--   0        0        0    13289 2024-04-02 20:46:05.414249 risk_adjustment_model-0.1.1/src/risk_adjustment_model/v24.py
+-rw-r--r--   0        0        0    17300 2024-04-02 20:46:05.414249 risk_adjustment_model-0.1.1/src/risk_adjustment_model/v28.py
+-rw-r--r--   0        0        0    10963 1970-01-01 00:00:00.000000 risk_adjustment_model-0.1.1/PKG-INFO
```

### Comparing `risk_adjustment_model-0.1.0/LICENSE` & `risk_adjustment_model-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/pyproject.toml` & `risk_adjustment_model-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "risk_adjustment_model"
-version = "0.1.0"
+version = "0.1.1"
 authors = ["Phil Fehlinger <pjfehlinger@gmail.com>"]
 description = "Python implementation of healthcare risk adjustment models"
 readme = "README.md"
 packages = [{include = "risk_adjustment_model", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
-pre-commit = "^3.6.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
+pre-commit = "^3.6.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
-]
+]
```

### Comparing `risk_adjustment_model-0.1.0/README.md` & `risk_adjustment_model-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/beneficiary.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/beneficiary.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/category.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/category.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/mapper.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/mapper.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/model.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/model.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2020/category_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2020/category_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2020/diag_to_category_map.txt` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2020/diag_to_category_map.txt`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2020/hierarchy_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2020/hierarchy_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2020/weights.csv` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2020/weights.csv`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2021/category_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2021/category_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2021/diag_to_category_map.txt` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2021/diag_to_category_map.txt`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2021/hierarchy_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2021/hierarchy_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2021/weights.csv` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2021/weights.csv`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2022/category_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2022/category_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2022/diag_to_category_map.txt` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2022/diag_to_category_map.txt`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2022/hierarchy_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2022/hierarchy_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2022/weights.csv` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2022/weights.csv`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2023/category_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2023/category_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2023/diag_to_category_map.txt` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2023/diag_to_category_map.txt`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2023/hierarchy_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2023/hierarchy_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2023/weights.csv` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2023/weights.csv`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2024/category_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2024/category_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2024/diag_to_category_map.txt` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2024/diag_to_category_map.txt`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2024/hierarchy_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2024/hierarchy_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v24/2024/weights.csv` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v24/2024/weights.csv`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v28/2024/category_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v28/2024/category_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v28/2024/diag_to_category_map.txt` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v28/2024/diag_to_category_map.txt`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v28/2024/hierarchy_definition.json` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v28/2024/hierarchy_definition.json`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_data/medicare/v28/2024/weights.csv` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_data/medicare/v28/2024/weights.csv`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/reference_files_loader.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/reference_files_loader.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/result.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/result.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/utilities.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/utilities.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/v24.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/v24.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/src/risk_adjustment_model/v28.py` & `risk_adjustment_model-0.1.1/src/risk_adjustment_model/v28.py`

 * *Files identical despite different names*

### Comparing `risk_adjustment_model-0.1.0/PKG-INFO` & `risk_adjustment_model-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: risk_adjustment_model
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python implementation of healthcare risk adjustment models
 Author: Phil Fehlinger
 Author-email: pjfehlinger@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pre-commit (>=3.6.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 # risk_adjustment_model
 Python implementation of Healthcare Risk Adjustment Models
 
 This codebase implements the [Hierachical Condition Categories](https://www.cms.gov/cciio/resources/forms-reports-and-other-resources/downloads/ra-march-31-white-paper-032416.pdf) that undergrid the Medicare Advantage program.
 The SAS implementations can be found on [CMS's website](https://www.cms.gov/medicare/payment/medicare-advantage-rates-statistics/risk-adjustment) by year.
```

