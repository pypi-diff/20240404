# Comparing `tmp/ml-research-0.4a2.tar.gz` & `tmp/ml-research-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-research-0.4a2.tar", last modified: Mon Oct 10 09:38:02 2022, max compression
+gzip compressed data, was "ml-research-0.5.0.tar", last modified: Thu Apr  4 12:26:08 2024, max compression
```

## Comparing `ml-research-0.4a2.tar` & `ml-research-0.5.0.tar`

### file list

```diff
@@ -1,77 +1,89 @@
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.093639 ml-research-0.4a2/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1081 2022-02-14 04:38:40.000000 ml-research-0.4a2/LICENSE
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6059 2022-10-10 09:38:02.093639 ml-research-0.4a2/PKG-INFO
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     4978 2022-04-22 15:10:17.000000 ml-research-0.4a2/README.md
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.089638 ml-research-0.4a2/ml_research.egg-info/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6059 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/PKG-INFO
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     2247 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/SOURCES.txt
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        1 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/dependency_links.txt
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      936 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/requires.txt
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)       11 2022-10-10 09:38:02.000000 ml-research-0.4a2/ml_research.egg-info/top_level.txt
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.089638 ml-research-0.4a2/mlresearch/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1888 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     2258 2022-04-13 14:07:23.000000 ml-research-0.4a2/mlresearch/_min_dependencies.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      585 2022-10-10 09:26:21.000000 ml-research-0.4a2/mlresearch/_version.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.089638 ml-research-0.4a2/mlresearch/active_learning/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      247 2022-02-22 22:57:29.000000 ml-research-0.4a2/mlresearch/active_learning/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1025 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/active_learning/_acquisition_functions.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    14935 2022-03-09 17:13:27.000000 ml-research-0.4a2/mlresearch/active_learning/_active_learning.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1266 2022-03-14 16:14:24.000000 ml-research-0.4a2/mlresearch/active_learning/_deep_al.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    12402 2022-03-10 09:50:23.000000 ml-research-0.4a2/mlresearch/active_learning/base.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.090638 ml-research-0.4a2/mlresearch/active_learning/tests/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/active_learning/tests/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      441 2022-02-22 22:48:12.000000 ml-research-0.4a2/mlresearch/active_learning/tests/test_acquisition_functions.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6740 2022-03-10 09:58:24.000000 ml-research-0.4a2/mlresearch/active_learning/tests/test_active_learning_models.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.090638 ml-research-0.4a2/mlresearch/data_augmentation/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      423 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    25784 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/_gsmote.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     5375 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/_image_transforms.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     9301 2022-03-08 19:04:51.000000 ml-research-0.4a2/mlresearch/data_augmentation/_oversampling_augmentation.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.090638 ml-research-0.4a2/mlresearch/data_augmentation/tests/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/tests/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    15847 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/tests/test_gsmote.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      589 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/data_augmentation/tests/test_image_transforms.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6205 2022-03-08 19:07:38.000000 ml-research-0.4a2/mlresearch/data_augmentation/tests/test_oversampling_augmentation.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/datasets/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      493 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/datasets/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    16678 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/datasets/_binary.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3215 2022-04-13 10:45:51.000000 ml-research-0.4a2/mlresearch/datasets/_image.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    21236 2022-04-14 15:07:12.000000 ml-research-0.4a2/mlresearch/datasets/_multiclass.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     5522 2022-04-13 10:45:51.000000 ml-research-0.4a2/mlresearch/datasets/_remote_sensing.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)    13894 2022-04-16 12:13:40.000000 ml-research-0.4a2/mlresearch/datasets/base.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/datasets/tests/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/datasets/tests/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1833 2022-04-16 12:39:03.000000 ml-research-0.4a2/mlresearch/datasets/tests/test_datasets.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/metrics/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      511 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/metrics/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3683 2022-04-13 13:49:22.000000 ml-research-0.4a2/mlresearch/metrics/_metrics.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/metrics/tests/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/metrics/tests/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1953 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/metrics/tests/test_metrics.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.091638 ml-research-0.4a2/mlresearch/self_supervised/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)       85 2022-03-19 15:51:17.000000 ml-research-0.4a2/mlresearch/self_supervised/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6549 2022-03-19 13:55:53.000000 ml-research-0.4a2/mlresearch/self_supervised/_byol.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     6321 2022-03-18 17:26:17.000000 ml-research-0.4a2/mlresearch/self_supervised/_components.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     5889 2022-03-18 13:26:59.000000 ml-research-0.4a2/mlresearch/self_supervised/_lars.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     5142 2022-03-19 15:45:30.000000 ml-research-0.4a2/mlresearch/self_supervised/_simsiam.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.092638 ml-research-0.4a2/mlresearch/self_supervised/tests/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/self_supervised/tests/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      852 2022-03-18 17:26:17.000000 ml-research-0.4a2/mlresearch/self_supervised/tests/test_scheduler.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3029 2022-03-19 15:33:15.000000 ml-research-0.4a2/mlresearch/self_supervised/tests/test_ssl_models.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.092638 ml-research-0.4a2/mlresearch/tests/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/tests/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     8661 2022-02-23 00:15:38.000000 ml-research-0.4a2/mlresearch/tests/test_docstring_parameters.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.092638 ml-research-0.4a2/mlresearch/utils/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      820 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3368 2022-04-13 14:04:47.000000 ml-research-0.4a2/mlresearch/utils/_check_pipelines.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     2288 2022-02-23 18:59:45.000000 ml-research-0.4a2/mlresearch/utils/_data.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)      484 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/_image.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3678 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/_testing.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     3225 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/_utils.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1830 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/_visualization.py
-drwxr-xr-x   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-10-10 09:38:02.093639 ml-research-0.4a2/mlresearch/utils/tests/
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)        0 2022-02-14 04:38:40.000000 ml-research-0.4a2/mlresearch/utils/tests/__init__.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     9066 2022-04-13 14:04:47.000000 ml-research-0.4a2/mlresearch/utils/tests/test_check_pipelines.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     1719 2022-02-23 18:59:45.000000 ml-research-0.4a2/mlresearch/utils/tests/test_load_datasets.py
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)       38 2022-10-10 09:38:02.093639 ml-research-0.4a2/setup.cfg
--rw-r--r--   0 joaofonseca  (1000) joaofonseca  (1000)     2363 2022-04-14 00:35:14.000000 ml-research-0.4a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.468504 ml-research-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-04 12:25:55.000000 ml-research-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-04 12:26:08.468504 ml-research-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-04 12:25:55.000000 ml-research-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.464504 ml-research-0.5.0/ml_research.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-04-04 12:26:08.000000 ml-research-0.5.0/ml_research.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-04 12:26:08.000000 ml-research-0.5.0/ml_research.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:26:08.000000 ml-research-0.5.0/ml_research.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-04 12:26:08.000000 ml-research-0.5.0/ml_research.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 12:26:08.000000 ml-research-0.5.0/ml_research.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.456504 ml-research-0.5.0/mlresearch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/_min_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.456504 ml-research-0.5.0/mlresearch/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/active_learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/active_learning/_acquisition_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14938 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/active_learning/_active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/active_learning/_deep_al.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12410 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/active_learning/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.456504 ml-research-0.5.0/mlresearch/active_learning/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/active_learning/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/active_learning/tests/test_acquisition_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/active_learning/tests/test_active_learning_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.456504 ml-research-0.5.0/mlresearch/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17091 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/datasets/_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23425 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/datasets/_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/datasets/_remote_sensing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15072 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/datasets/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.456504 ml-research-0.5.0/mlresearch/datasets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/datasets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/datasets/tests/test_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.456504 ml-research-0.5.0/mlresearch/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12470 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/latex/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.456504 ml-research-0.5.0/mlresearch/latex/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/latex/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/latex/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.460504 ml-research-0.5.0/mlresearch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/metrics/_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/metrics/_rankings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12605 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/metrics/_synth_data_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.460504 ml-research-0.5.0/mlresearch/metrics/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/metrics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/metrics/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/metrics/tests/test_synth_data_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.460504 ml-research-0.5.0/mlresearch/neural_network/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/neural_network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19069 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/neural_network/_one_class_mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.460504 ml-research-0.5.0/mlresearch/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8608 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/preprocessing/_encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.460504 ml-research-0.5.0/mlresearch/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/preprocessing/tests/test_pipeline_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.460504 ml-research-0.5.0/mlresearch/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25930 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/synthetic_data/_gsmote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/synthetic_data/_oversampling_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.460504 ml-research-0.5.0/mlresearch/synthetic_data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/synthetic_data/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15833 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/synthetic_data/tests/test_gsmote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/synthetic_data/tests/test_oversampling_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.460504 ml-research-0.5.0/mlresearch/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8748 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/tests/test_docstring_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.464504 ml-research-0.5.0/mlresearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/_check_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:26:08.464504 ml-research-0.5.0/mlresearch/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/tests/test_check_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/tests/test_load_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/tests/test_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/tests/test_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-04 12:25:55.000000 ml-research-0.5.0/mlresearch/utils/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:26:08.468504 ml-research-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-04 12:25:55.000000 ml-research-0.5.0/setup.py
```

### Comparing `ml-research-0.4a2/LICENSE` & `ml-research-0.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 The MIT License (MIT)
-Copyright (c) 2022, Joao Fonseca
+Copyright (c) 2023, Joao Fonseca
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `ml-research-0.4a2/README.md` & `ml-research-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 ______________________________________________________________________
 
 <p align="center">
 <a href="https://github.com/joaopfonseca/ml-research/actions/workflows/ci.yml"><img alt="Github Actions" src="https://github.com/joaopfonseca/ml-research/actions/workflows/ci.yml/badge.svg"></a>
 <a href="https://codecov.io/gh/joaopfonseca/ml-research"><img alt="Codecov" src="https://codecov.io/gh/joaopfonseca/ml-research/branch/master/graph/badge.svg?token=J2EBA4YTMN"></a>
 <a href="https://mlresearch.readthedocs.io/en/latest/?badge=latest"><img alt="Documentation Status" src="https://readthedocs.org/projects/mlresearch/badge/?version=latest"></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-<a href="https://img.shields.io/badge/python-3.8%20|%203.9-blue"><img alt="Python Versions" src="https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue"></a>
-<a href="https://doi.org/10.3390/RS13132619"><img alt="DOI" src="https://zenodo.org/badge/DOI/10.3390/RS13132619.svg"></a>
+<a href="https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11%20|%203.12-blue"><img alt="Python Versions" src="https://img.shields.io/badge/python-3.9%20|%203.10%20|%203.11%20|%203.12-blue"></a>
+<a href="https://doi.org/10.1155/2023/7941878"><img alt="DOI" src="https://zenodo.org/badge/DOI/10.1155/2023/7941878.svg"></a>
 </p>
 <table align="center">
   <tr>
     <td>
       <b>PyPI</b>
     </td>
     <td>
@@ -29,47 +29,40 @@
     <td>
       <a href="https://anaconda.org/conda-forge/ml-research"><img alt="Conda Version" src="https://img.shields.io/conda/vn/conda-forge/ml-research.svg"></a>
       <a href="https://anaconda.org/conda-forge/ml-research"><img alt="Conda Downloads" src="https://img.shields.io/conda/dn/conda-forge/ml-research.svg"></a>
     </td>
   </tr>
 </table>
 
-``ML-Research`` is an open source library for machine learning research.  It
-contains the software implementation of most algorithms used or developed in
-my research. Specifically, it contains ``scikit-learn`` compatible
-implementations for Active Learning, Oversampling, Datasets and various
-utilities to assist in experiment design and results reporting. Other
-techniques, such as self-supervised learning and semi-supervised learning are
-currently under development and are being implemented in ``pytorch`` and
-intended to be ``scikit-learn`` compatible.
-
-The LaTeX and Python code for generating the
-paper, experiments' results and visualizations reported in each paper is
-available (whenever possible) in the [publications
-repo](https://github.com/joaopfonseca/publications).
-
-Contributions at the algorithm level are available in the
-package ``mlresearch``.
+``ML-Research`` is an open source library for machine learning research. It
+contains several utilities for Machine Learning research and algorithm
+implementations. Specifically, it contains ``scikit-learn`` compatible
+implementations for Active Learning and synthetic data generation, as well as
+datasets and various utilities to assist in experiment design and results
+reporting.
+
+The LaTeX and Python code for generating the paper, experiments' results and
+visualizations shown in each paper is available (whenever possible) in the
+[publications repo](https://github.com/joaopfonseca/publications).
 
 ## Installation
 
-A Python distribution of version 3.8, 3.9 or 3.10 is required to run this
+A Python distribution of version >= 3.9 is required to run this
 project. Earlier Python versions might work in most cases, but they are not
 tested. ``ML-Research`` requires:
 
-- numpy (>= 1.14.6)
-- pandas (>= 1.3.5)
-- sklearn (>= 1.0.0)
+- numpy (>= 1.20.0)
+- pandas (>= 2.1.0)
+- sklearn (>= 1.2.0)
 - imblearn (>= 0.8.0)
-- rich (>= 10.16.1)
-- matplotlib (>= 2.2.3)
-- seaborn (>= 0.9.0)
-- pytorch (>= 1.10.1)
-- torchvision (>= 0.11.2)
-- pytorch_lightning (>= 1.5.8)
+
+Some functions in the ``mlresearch.utils`` submodule (the ones in the script
+``_visualization.py``) require Matplotlib (>= 2.2.3). The
+``mlresearch.datasets`` submodule and ``mlresearch.utils.parallel_apply``
+function require tqdm (>= 4.46.0) to display progress bars.
 
 ### User Installation
 
 The easiest way to install ml-research is using ``pip`` :
 
     pip install -U ml-research
 
@@ -90,28 +83,23 @@
     cd ml-research
 
     # Create and activate an environment 
     make environment 
     conda activate mlresearch # Adapt this line accordingly if you're not running conda
 
     # Install project requirements and the research package. Dependecy group
-    # "all" will also install both dependency groups shown below.
-    pip install .[tests,docs] 
+    # "all" will also install the dependency groups shown below.
+    pip install .[optional,tests,docs] 
 
 ## Citing ML-Research
 
 If you use ML-Research in a scientific publication, we would appreciate
 citations to the following paper:
 
-    @article{Fonseca2021,
-      doi = {10.3390/RS13132619},
-      url = {https://doi.org/10.3390/RS13132619},
-      keywords = {SMOTE,active learning,artificial data generation,land use/land cover classification,oversampling},
-      year = {2021},
-      month = {jul},
-      publisher = {Multidisciplinary Digital Publishing Institute},
-      volume = {13},
-      pages = {2619},
-      author = {Fonseca, Joao and Douzas, Georgios and Bacao, Fernando},
-      title = {{Increasing the Effectiveness of Active Learning: Introducing Artificial Data Generation in Active Learning for Land Use/Land Cover Classification}},
-      journal = {Remote Sensing}
+    @article{fonseca2023improving,
+      title={Improving Active Learning Performance through the Use of Data Augmentation},
+      author={Fonseca, Joao and Bacao, Fernando and others},
+      journal={International Journal of Intelligent Systems},
+      volume={2023},
+      year={2023},
+      publisher={Hindawi}
     }
```

#### html2text {}

```diff
@@ -1,43 +1,37 @@
                             [docs/_static/logo.png]
 ______________________________________________________________________
  _[_G_i_t_h_u_b_ _A_c_t_i_o_n_s_]_[_C_o_d_e_c_o_v_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_B_l_a_c_k_]_[_P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_D_O_I_]
                    PPyyPPII     _[_P_y_p_i_ _V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                    AAnnaaccoonnddaa _[_C_o_n_d_a_ _V_e_r_s_i_o_n_]_[_C_o_n_d_a_ _D_o_w_n_l_o_a_d_s_]
 ``ML-Research`` is an open source library for machine learning research. It
-contains the software implementation of most algorithms used or developed in my
-research. Specifically, it contains ``scikit-learn`` compatible implementations
-for Active Learning, Oversampling, Datasets and various utilities to assist in
-experiment design and results reporting. Other techniques, such as self-
-supervised learning and semi-supervised learning are currently under
-development and are being implemented in ``pytorch`` and intended to be
-``scikit-learn`` compatible. The LaTeX and Python code for generating the
-paper, experiments' results and visualizations reported in each paper is
-available (whenever possible) in the [publications repo](https://github.com/
-joaopfonseca/publications). Contributions at the algorithm level are available
-in the package ``mlresearch``. ## Installation A Python distribution of version
-3.8, 3.9 or 3.10 is required to run this project. Earlier Python versions might
-work in most cases, but they are not tested. ``ML-Research`` requires: - numpy
-(>= 1.14.6) - pandas (>= 1.3.5) - sklearn (>= 1.0.0) - imblearn (>= 0.8.0) -
-rich (>= 10.16.1) - matplotlib (>= 2.2.3) - seaborn (>= 0.9.0) - pytorch (>=
-1.10.1) - torchvision (>= 0.11.2) - pytorch_lightning (>= 1.5.8) ### User
-Installation The easiest way to install ml-research is using ``pip`` : pip
-install -U ml-research Or ``conda`` : conda install -c conda-forge ml-research
-The documentation includes more detailed [installation instructions](https://
-mlresearch.readthedocs.io/en/latest/getting-started.html). ### Installing from
-source The following commands should allow you to setup the development version
-of the project with minimal effort: # Clone the project. git clone https://
-github.com/joaopfonseca/ml-research.git cd ml-research # Create and activate an
-environment make environment conda activate mlresearch # Adapt this line
-accordingly if you're not running conda # Install project requirements and the
-research package. Dependecy group # "all" will also install both dependency
-groups shown below. pip install .[tests,docs] ## Citing ML-Research If you use
-ML-Research in a scientific publication, we would appreciate citations to the
-following paper: @article{Fonseca2021, doi = {10.3390/RS13132619}, url =
-{https://doi.org/10.3390/RS13132619}, keywords = {SMOTE,active
-learning,artificial data generation,land use/land cover
-classification,oversampling}, year = {2021}, month = {jul}, publisher =
-{Multidisciplinary Digital Publishing Institute}, volume = {13}, pages =
-{2619}, author = {Fonseca, Joao and Douzas, Georgios and Bacao, Fernando},
-title = {{Increasing the Effectiveness of Active Learning: Introducing
-Artificial Data Generation in Active Learning for Land Use/Land Cover
-Classification}}, journal = {Remote Sensing} }
+contains several utilities for Machine Learning research and algorithm
+implementations. Specifically, it contains ``scikit-learn`` compatible
+implementations for Active Learning and synthetic data generation, as well as
+datasets and various utilities to assist in experiment design and results
+reporting. The LaTeX and Python code for generating the paper, experiments'
+results and visualizations shown in each paper is available (whenever possible)
+in the [publications repo](https://github.com/joaopfonseca/publications). ##
+Installation A Python distribution of version >= 3.9 is required to run this
+project. Earlier Python versions might work in most cases, but they are not
+tested. ``ML-Research`` requires: - numpy (>= 1.20.0) - pandas (>= 2.1.0) -
+sklearn (>= 1.2.0) - imblearn (>= 0.8.0) Some functions in the
+``mlresearch.utils`` submodule (the ones in the script ``_visualization.py``)
+require Matplotlib (>= 2.2.3). The ``mlresearch.datasets`` submodule and
+``mlresearch.utils.parallel_apply`` function require tqdm (>= 4.46.0) to
+display progress bars. ### User Installation The easiest way to install ml-
+research is using ``pip`` : pip install -U ml-research Or ``conda`` : conda
+install -c conda-forge ml-research The documentation includes more detailed
+[installation instructions](https://mlresearch.readthedocs.io/en/latest/
+getting-started.html). ### Installing from source The following commands should
+allow you to setup the development version of the project with minimal effort:
+# Clone the project. git clone https://github.com/joaopfonseca/ml-research.git
+cd ml-research # Create and activate an environment make environment conda
+activate mlresearch # Adapt this line accordingly if you're not running conda #
+Install project requirements and the research package. Dependecy group # "all"
+will also install the dependency groups shown below. pip install .
+[optional,tests,docs] ## Citing ML-Research If you use ML-Research in a
+scientific publication, we would appreciate citations to the following paper:
+@article{fonseca2023improving, title={Improving Active Learning Performance
+through the Use of Data Augmentation}, author={Fonseca, Joao and Bacao,
+Fernando and others}, journal={International Journal of Intelligent Systems},
+volume={2023}, year={2023}, publisher={Hindawi} }
```

### Comparing `ml-research-0.4a2/ml_research.egg-info/SOURCES.txt` & `ml-research-0.5.0/ml_research.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -13,47 +13,56 @@
 mlresearch/active_learning/_acquisition_functions.py
 mlresearch/active_learning/_active_learning.py
 mlresearch/active_learning/_deep_al.py
 mlresearch/active_learning/base.py
 mlresearch/active_learning/tests/__init__.py
 mlresearch/active_learning/tests/test_acquisition_functions.py
 mlresearch/active_learning/tests/test_active_learning_models.py
-mlresearch/data_augmentation/__init__.py
-mlresearch/data_augmentation/_gsmote.py
-mlresearch/data_augmentation/_image_transforms.py
-mlresearch/data_augmentation/_oversampling_augmentation.py
-mlresearch/data_augmentation/tests/__init__.py
-mlresearch/data_augmentation/tests/test_gsmote.py
-mlresearch/data_augmentation/tests/test_image_transforms.py
-mlresearch/data_augmentation/tests/test_oversampling_augmentation.py
 mlresearch/datasets/__init__.py
 mlresearch/datasets/_binary.py
-mlresearch/datasets/_image.py
 mlresearch/datasets/_multiclass.py
 mlresearch/datasets/_remote_sensing.py
 mlresearch/datasets/base.py
 mlresearch/datasets/tests/__init__.py
 mlresearch/datasets/tests/test_datasets.py
+mlresearch/latex/__init__.py
+mlresearch/latex/_utils.py
+mlresearch/latex/tests/__init__.py
+mlresearch/latex/tests/test_utils.py
 mlresearch/metrics/__init__.py
 mlresearch/metrics/_metrics.py
+mlresearch/metrics/_rankings.py
+mlresearch/metrics/_synth_data_quality.py
 mlresearch/metrics/tests/__init__.py
 mlresearch/metrics/tests/test_metrics.py
-mlresearch/self_supervised/__init__.py
-mlresearch/self_supervised/_byol.py
-mlresearch/self_supervised/_components.py
-mlresearch/self_supervised/_lars.py
-mlresearch/self_supervised/_simsiam.py
-mlresearch/self_supervised/tests/__init__.py
-mlresearch/self_supervised/tests/test_scheduler.py
-mlresearch/self_supervised/tests/test_ssl_models.py
+mlresearch/metrics/tests/test_synth_data_quality.py
+mlresearch/neural_network/__init__.py
+mlresearch/neural_network/_one_class_mlp.py
+mlresearch/preprocessing/__init__.py
+mlresearch/preprocessing/_encoders.py
+mlresearch/preprocessing/tests/__init__.py
+mlresearch/preprocessing/tests/test_pipeline_encoder.py
+mlresearch/synthetic_data/__init__.py
+mlresearch/synthetic_data/_gsmote.py
+mlresearch/synthetic_data/_oversampling_augmentation.py
+mlresearch/synthetic_data/tests/__init__.py
+mlresearch/synthetic_data/tests/test_gsmote.py
+mlresearch/synthetic_data/tests/test_oversampling_augmentation.py
 mlresearch/tests/__init__.py
 mlresearch/tests/test_docstring_parameters.py
 mlresearch/utils/__init__.py
 mlresearch/utils/_check_pipelines.py
 mlresearch/utils/_data.py
 mlresearch/utils/_image.py
+mlresearch/utils/_parallelize.py
+mlresearch/utils/_show_versions.py
 mlresearch/utils/_testing.py
 mlresearch/utils/_utils.py
 mlresearch/utils/_visualization.py
 mlresearch/utils/tests/__init__.py
 mlresearch/utils/tests/test_check_pipelines.py
-mlresearch/utils/tests/test_load_datasets.py
+mlresearch/utils/tests/test_image.py
+mlresearch/utils/tests/test_load_datasets.py
+mlresearch/utils/tests/test_parallelize.py
+mlresearch/utils/tests/test_show_versions.py
+mlresearch/utils/tests/test_utils.py
+mlresearch/utils/tests/test_visualization.py
```

### Comparing `ml-research-0.4a2/mlresearch/__init__.py` & `ml-research-0.5.0/mlresearch/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,52 +4,62 @@
 in Machine Learning research, as well as utilities to facilitate the formatting of pandas
 dataframes into LaTeX tables.
 
 Subpackages
 -----------
 active_learning
     Module which contains the code developed for experiments related to Active Learning.
-data_augmentation
+synthetic_data
     Module which contains the implementation of variations of oversampling/data
     augmentation algorithms, as well as helper classes to use oversampling algorithms as
     data augmentation techniques.
 datasets
     Module which contains code to download, transform and simulate various datasets.
 metrics
     Module which contains performance metrics/scorers that are not
     included in scikit-learn's scorers' dictionary.
+preprocessing
+    Contains preprocessing methods adapted or modified from sklearn.
+latex
+    This module contains several functions to prepare and format tables for LaTeX
+    documents.
 utils
-    contains a variety of general utility functions and tools used to format and prepare
+    Contains a variety of general utility functions and tools used to format and prepare
     tables to incorporate into LaTeX code.
 """
+
 import sys
 
 try:
     # This variable is injected in the __builtins__ by the build
-    # process. It is used to enable importing subpackages of sklearn when
+    # process. It is used to enable importing subpackages of mlresearch when
     # the binaries are not built
-    # mypy error: Cannot determine type of '__SKLEARN_SETUP__'
+    # mypy error: Cannot determine type of '__MLRESEARCH_SETUP__'
     __MLRESEARCH_SETUP__  # type: ignore
 except NameError:
     __MLRESEARCH_SETUP__ = False
 
 if __MLRESEARCH_SETUP__:
     sys.stderr.write("Partial import of imblearn during the build process.\n")
     # We are not importing the rest of scikit-learn during the build
     # process, as it may not be compiled yet
 else:
     from . import active_learning
-    from . import data_augmentation
+    from . import synthetic_data
     from . import datasets
     from . import metrics
+    from . import preprocessing
     from . import utils
-
     from ._version import __version__
+    from .utils._show_versions import show_versions
 
     __all__ = [
         "active_learning",
-        "data_augmentation",
+        "synthetic_data",
         "datasets",
         "metrics",
+        "preprocessing",
         "utils",
+        # Non-modules:
+        "show_versions",
         "__version__",
     ]
```

### Comparing `ml-research-0.4a2/mlresearch/_min_dependencies.py` & `ml-research-0.5.0/mlresearch/_min_dependencies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 """All minimum dependencies for ml-research."""
+
 import argparse
 
-NUMPY_MIN_VERSION = "1.14.6"
-PANDAS_MIN_VERSION = "1.3.5"
-SKLEARN_MIN_VERSION = "1.0.0"
+NUMPY_MIN_VERSION = "1.20.0"
+PANDAS_MIN_VERSION = "2.1.0"
+SKLEARN_MIN_VERSION = "1.2.0"
 IMBLEARN_MIN_VERSION = "0.8.0"
-RICH_MIN_VERSION = "10.16.1"
+TQDM_MIN_VERSION = "4.46.0"
 MATPLOTLIB_MIN_VERSION = "2.2.3"
-SEABORN_MIN_VERSION = "0.9.0"
-PYTORCH_MIN_VERSION = "1.10.1"
-TORCHVISION_MIN_VERSION = "0.11.2"
-PYTORCH_LIGHTNING_VERSION = "1.5.8"
 
 # The values are (version_spec, comma separated tags)
 dependent_packages = {
     "pandas": (PANDAS_MIN_VERSION, "install"),
     "numpy": (NUMPY_MIN_VERSION, "install"),
     "scikit-learn": (SKLEARN_MIN_VERSION, "install"),
     "imbalanced-learn": (IMBLEARN_MIN_VERSION, "install"),
-    "rich": (RICH_MIN_VERSION, "install"),
-    "matplotlib": (MATPLOTLIB_MIN_VERSION, "install"),
-    "seaborn": (SEABORN_MIN_VERSION, "install"),
     "requests": ("2.26.0", "install"),
-    "torch": (PYTORCH_MIN_VERSION, "install"),
-    "torchvision": (TORCHVISION_MIN_VERSION, "install"),
-    "pytorch-lightning": (PYTORCH_LIGHTNING_VERSION, "install"),
+    "tqdm": (TQDM_MIN_VERSION, "optional"),
+    "matplotlib": (MATPLOTLIB_MIN_VERSION, "optional"),
     "research-learn": ("0.3.0", "tests"),
     "pytest-cov": ("3.0.0", "tests"),
     "flake8": ("3.8.2", "tests"),
     "black": ("22.3", "tests"),
     "pylint": ("2.12.2", "tests"),
+    "mypy": ("1.6.1", "tests"),
+    "types-requests": ("2.31.0.10", "tests"),
     "coverage": ("6.2", "tests"),
     "sphinx": ("4.2.0", "docs"),
     "numpydoc": ("1.0.0", "docs, tests"),
     "sphinx-material": ("0.0.35", "docs"),
     "nbsphinx": ("0.8.7", "docs"),
     "recommonmark": ("0.7.1", "docs"),
     "sphinx-markdown-tables": ("0.0.15", "docs"),
```

### Comparing `ml-research-0.4a2/mlresearch/_version.py` & `ml-research-0.5.0/mlresearch/_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #   X.YrcN  # Release Candidate
 #   X.Y     # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
 
-__version__ = "0.4a2"
+__version__ = "0.5.0"
```

### Comparing `ml-research-0.4a2/mlresearch/active_learning/_acquisition_functions.py` & `ml-research-0.5.0/mlresearch/active_learning/_acquisition_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Acquisition functions that may be used along with Active Learning objects. All functions
 must be set up so that a higher value means higher uncertainty (higher likelihood of
 selection) and vice-versa.
 """
+
 import numpy as np
 
 
 def breaking_ties(probabilities):
     """Breaking Ties uncertainty measurement. The output is scaled and reversed."""
     probs_sorted = np.sort(probabilities, axis=1)[:, ::-1]
     # The extra minus is redundant but I kept as a highlight of the change in the
```

### Comparing `ml-research-0.4a2/mlresearch/active_learning/_active_learning.py` & `ml-research-0.5.0/mlresearch/active_learning/_active_learning.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     else:
         rng = np.random.RandomState(self.random_state)
         labeled_pool = np.zeros(shape=(X.shape[0])).astype(bool)
         ids = rng.choice(np.arange(X.shape[0]), self.n_init_, replace=False)
         if np.unique(y[ids]).shape[0] == 1:
             ids[-1] = rng.choice(
                 np.arange(X.shape[0])[y != y[ids][0]], 1, replace=False
-            )
+            ).squeeze()
         labeled_pool[ids] = True
     return labeled_pool
 
 
 class StandardAL(BaseActiveLearner, ClassifierMixin):
     """
     Standard Active Learning model with a random initial data selection
@@ -153,15 +153,15 @@
     cv : int, cross-validation generator or an iterable, default=None
         Determines the cross-validation splitting strategy. Used to optimize the
         classifier and generator hyperparameters at each iteration.
         Possible inputs for cv are:
 
         - None, to use the default 5-fold cross validation,
         - integer, to specify the number of folds in a `(Stratified)KFold`,
-        - :term:`CV splitter`.
+        - `CV splitter`.
 
         For integer/None inputs, if the estimator is a classifier and ``y`` is
         either binary or multiclass, :class:`StratifiedKFold` is used. In all
         other cases, :class:`KFold` is used. These splitters are instantiated
         with `shuffle=False` so the splits will be the same across calls.
 
     acquisition_func : function or {'entropy', 'breaking_ties', 'random'}, default=None
@@ -274,45 +274,45 @@
             generator = clone(self._generator)
             classifier = clone(self._classifier)
             self._classifier = Pipeline(
                 [("generator", generator), ("classifier", classifier)]
             )
 
         # Check if parameters in param_grid are valid
-        if type(self.param_grid) == dict:
+        if type(self.param_grid) is dict:
             for key in self.param_grid.keys():
                 if key not in self._classifier.get_params():
                     raise ValueError(
                         f"Invalid parameter {key} for generator or classifier in {self} "
                         "check the list of available parameters with "
                         "`almodel._classifier.get_params().keys()`."
                     )
         elif self.param_grid is not None:
             raise TypeError(
                 f"``param_grid`` must be a dict or None. Got {self.param_grid} instead."
             )
 
     def _save_metadata(self, X, y, **kwargs):
         super()._save_metadata(X, y, **kwargs)
-        if hasattr(self, "classifier_") and type(self.classifier_) == GridSearchCV:
+        if hasattr(self, "classifier_") and type(self.classifier_) is GridSearchCV:
             self.metadata_[self._current_iter]["parameters"] = {
                 k: v
                 for k, v in self.classifier_.best_estimator_.get_params().items()
                 if k in self.param_grid.keys()
             }
 
     def _check_cross_validation(self, y):
         """Define cross-validation object"""
 
         min_frequency = np.unique(y, return_counts=True)[-1].min()
         cv = deepcopy(self.cv)
 
         if hasattr(self.cv, "n_splits"):
             cv.n_splits = min(min_frequency, cv.n_splits)
-        elif type(self.cv) == int:
+        elif type(self.cv) is int:
             cv = min(min_frequency, cv)
         elif cv is None:
             cv = min(min_frequency, 5)
         else:
             raise TypeError(
                 "``cv`` object must be of type int or cross-validation generator. Got "
                 f"{self.cv} instead"
@@ -320,15 +320,14 @@
         return cv
 
     def _initialization(self, X=None, y=None, initial_selection=None):
         labeled_pool = _random_initialization(self, X, y, initial_selection)
         return labeled_pool
 
     def _iteration(self, X, y, **kwargs):
-
         # Set up parameter tuning within iterations
         cv = self._check_cross_validation(y[self.labeled_pool_])
         if self.param_grid is not None and cv != 1:
             self.classifier_ = GridSearchCV(
                 estimator=self.classifier_,
                 param_grid=self.param_grid,
                 scoring=self.evaluation_metric_,
```

### Comparing `ml-research-0.4a2/mlresearch/active_learning/_deep_al.py` & `ml-research-0.5.0/mlresearch/active_learning/_deep_al.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a2/mlresearch/active_learning/base.py` & `ml-research-0.5.0/mlresearch/active_learning/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Union
 import numpy as np
 from sklearn.base import ClassifierMixin, BaseEstimator, clone
 from sklearn.utils import check_X_y
 from sklearn.ensemble import RandomForestClassifier
 
 from ._acquisition_functions import ACQUISITION_FUNCTIONS
-from ..metrics import SCORERS
+from ..metrics import get_scorer
 
 
 class BaseActiveLearner(BaseEstimator, metaclass=ABCMeta):
     """
     Base class to implement Active Learning models.
 
     Parameters
@@ -148,15 +148,15 @@
             and self.random_state is not None
         ):
             self._classifier.set_params(random_state=self.random_state)
 
         # Acquisition function
         if self.acquisition_func is None:
             self.acquisition_func_ = ACQUISITION_FUNCTIONS["random"]
-        elif type(self.acquisition_func) == str:
+        elif type(self.acquisition_func) is str:
             self.acquisition_func_ = ACQUISITION_FUNCTIONS[self.acquisition_func]
         else:
             self.acquisition_func_ = self.acquisition_func
 
         # Number of initial observations
         if self.n_init is None or self.n_init < 1:
             perc = 0.02 if self.n_init is None else self.n_init
@@ -178,23 +178,23 @@
             self.max_iter
             if self.max_iter is not None
             else int(np.round((X.shape[0] - self.n_init_) / self.budget_))
         )
 
         # Evaluation metric
         if self.evaluation_metric is None:
-            self.evaluation_metric_ = SCORERS["accuracy"]
-        elif type(self.evaluation_metric) == str:
-            self.evaluation_metric_ = SCORERS[self.evaluation_metric]
+            self.evaluation_metric_ = get_scorer("accuracy")
+        elif type(self.evaluation_metric) is str:
+            self.evaluation_metric_ = get_scorer(self.evaluation_metric)
         else:
             self.evaluation_metric_ = self.evaluation_metric
 
         # Train a different classifier per iteration (as an alternative continue training
         # the classifier from previous iterations)
-        if type(self.continue_training) == bool:
+        if type(self.continue_training) is bool:
             self._continue_training = self.continue_training
         else:
             raise TypeError(
                 "``continue_training`` must be of type ``bool``. Got"
                 f" {self.continue_training} instead."
             )
 
@@ -291,15 +291,14 @@
 
         # Create base classifier if it is going to be trained across iterations
         if self._continue_training and not hasattr(self, "classifier_"):
             self.classifier_ = clone(self._classifier)
 
         # Iterate
         for iter_ in range(1, self.max_iter_ + 1):
-
             self.iteration(X, y, **kwargs)
 
             if self._early_stop():
                 break
 
         return self
```

### Comparing `ml-research-0.4a2/mlresearch/active_learning/tests/test_active_learning_models.py` & `ml-research-0.5.0/mlresearch/active_learning/tests/test_active_learning_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Testing active learning models."""
+
 import pytest
 from itertools import product
 import re
 import numpy as np
 from sklearn import datasets
 from sklearn.utils.validation import check_random_state
 from sklearn.utils._testing import assert_array_equal, ignore_warnings
 from sklearn.neural_network import MLPClassifier
 from sklearn.ensemble import RandomForestClassifier
 
-from ...data_augmentation import OverSamplingAugmentation, GeometricSMOTE
-from ...metrics import SCORERS
+from ...synthetic_data import OverSamplingAugmentation, GeometricSMOTE
+from ...metrics import get_scorer
 from .._acquisition_functions import ACQUISITION_FUNCTIONS
 from .._active_learning import StandardAL, AugmentationAL
 
 ACTIVE_LEARNERS = {"StandardAL": StandardAL, "AugmentationAL": AugmentationAL}
 
 RANDOM_STATE = 42
 
@@ -71,15 +72,15 @@
     exp_acquisition_func = ACQUISITION_FUNCTIONS["random"]
     exp_n_init = int(np.round(0.02 * np.array(X).shape[0]))
     exp_n_init = exp_n_init if exp_n_init >= 2 else 2
     exp_budget = int(np.round(0.02 * np.array(X).shape[0]))
     exp_budget = exp_budget if exp_budget >= 1 else 1
     exp_max_iter = int((np.array(X).shape[0] - exp_n_init) / exp_budget)
 
-    assert type(al_model.classifier_) == RandomForestClassifier
+    assert type(al_model.classifier_) is RandomForestClassifier
     assert al_model.acquisition_func_ == exp_acquisition_func
     assert al_model.n_init_ == exp_n_init
     assert al_model.budget_ == exp_budget
     assert al_model.max_iter_ == exp_max_iter
     assert al_model.random_state is None
     assert al_model.continue_training is False
 
@@ -161,15 +162,15 @@
         budget=1,
         max_iter=5,
     ).fit(X, y)
 
     # passing an evaluation metric as function
     ACTIVE_LEARNERS[name](
         classifier=classifier,
-        evaluation_metric=SCORERS["f1_macro"],
+        evaluation_metric=get_scorer("f1_macro"),
         n_init=2,
         budget=1,
         max_iter=5,
     ).fit(X, y)
 
     # fit with test set
     ACTIVE_LEARNERS[name](
```

### Comparing `ml-research-0.4a2/mlresearch/data_augmentation/_gsmote.py` & `ml-research-0.5.0/mlresearch/synthetic_data/_gsmote.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,14 @@
 )
 class GeometricSMOTE(BaseOverSampler):
     """Class to to perform over-sampling using Geometric SMOTE.
 
     This algorithm is an implementation of Geometric SMOTE, a geometrically
     enhanced drop-in replacement for SMOTE as presented in [1]_.
 
-    Read more in the :ref:`User Guide <user_guide>`.
-
     Parameters
     ----------
     categorical_features : ndarray of shape (n_cat_features,) or (n_features,)
         Specified which features are categorical. Can either be:
 
         - array of indices specifying the categorical features;
         - mask array of shape (n_features, ) and ``bool`` dtype for which
@@ -434,15 +432,14 @@
                 if self.selection_strategy_ in ("majority", "combined"):
                     X_neg = X[y != pos_class_label]
 
         # Generate new samples
         X_new = np.zeros((n_samples, X.shape[1]))
         all_neighbors_ = []
         for ind, (row, col) in enumerate(zip(rows, cols)):
-
             # Define center point
             center = X_pos[row]
 
             # Minority strategy
             if self.selection_strategy_ == "minority":
                 surface_point = X_pos[points_pos[row, col]]
                 all_neighbors = (
@@ -497,15 +494,18 @@
             # Append new sample - continuous features
             X_new[ind] = _make_categorical_sample(
                 X_new[ind], all_neighbors, categories_size, self.random_state_
             )
         return X_new, y_new
 
     def _encode_categorical(self, X, y):
-        """TODO"""
+        """
+        One-Hot encodes categorical features and replaces the 1 entries with the median
+        of the standard deviations divided by 2.
+        """
         # compute the median of the standard deviation of the minority class
         target_stats = Counter(y)
         class_minority = min(target_stats, key=target_stats.get)
 
         # Separate categorical features from continuous features
         X_continuous = X[:, self.continuous_features_]
         X_continuous = check_array(X_continuous, accept_sparse=["csr", "csc"])
@@ -521,15 +521,17 @@
             var = X_minority.var(axis=0)
         self.median_std_ = np.median(np.sqrt(var))
 
         if X_continuous.dtype.name != "object":
             dtype_ohe = X_continuous.dtype
         else:
             dtype_ohe = np.float64
-        self.ohe_ = OneHotEncoder(sparse=True, handle_unknown="ignore", dtype=dtype_ohe)
+        self.ohe_ = OneHotEncoder(
+            sparse_output=True, handle_unknown="ignore", dtype=dtype_ohe
+        )
 
         # the input of the OneHotEncoder needs to be dense
         X_ohe = self.ohe_.fit_transform(
             X_categorical.toarray() if sparse.issparse(X_categorical) else X_categorical
         )
 
         # we can replace the 1 entries of the categorical features with the
@@ -592,15 +594,14 @@
             X_resampled.indices = col_indices
         else:
             X_resampled = X_resampled[:, indices_reordered]
 
         return X_resampled
 
     def _fit_resample(self, X, y, sample_weight=None):
-
         # Save basic data
         self._issparse = sparse.issparse(X)
         X_dtype = X.dtype
 
         # Validate estimator's parameters
         self._validate_categorical()._validate_estimator()
 
@@ -612,15 +613,14 @@
             ]
 
         # Copy data
         X_resampled, y_resampled = X.copy(), y.copy()
 
         # Resample
         for class_label, n_samples in self.sampling_strategy_.items():
-
             # Apply gsmote mechanism
             X_new, y_new, all_neighbors_ = self._make_geometric_samples(
                 X, y, class_label, n_samples, sample_weight=sample_weight
             )
 
             # Apply smotenc mechanism
             if self.categorical_features is not None:
@@ -674,11 +674,13 @@
 
         self.sampling_strategy_ = check_sampling_strategy(
             self.sampling_strategy, y, self._sampling_type
         )
 
         output = self._fit_resample(X, y, sample_weight)
 
-        y_ = label_binarize(output[1], np.unique(y)) if binarize_y else output[1]
+        y_ = (
+            label_binarize(output[1], classes=np.unique(y)) if binarize_y else output[1]
+        )
 
         X_, y_ = arrays_transformer.transform(output[0], y_)
         return (X_, y_) if len(output) == 2 else (X_, y_, output[2])
```

### Comparing `ml-research-0.4a2/mlresearch/data_augmentation/_oversampling_augmentation.py` & `ml-research-0.5.0/mlresearch/synthetic_data/_oversampling_augmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 A wrapper to allow the use of oversampling algorithms for data augmentation
 in Active Learning experiments with multiple datasets.
 """
+
 import warnings
 from collections import Counter, OrderedDict
 import numpy as np
 from sklearn.base import clone
 from sklearn.neighbors import NearestNeighbors
 from imblearn.over_sampling.base import BaseOverSampler
 from imblearn.over_sampling import RandomOverSampler
@@ -193,17 +194,19 @@
                 else None
             )
 
         elif self.augmentation_strategy == "oversampling":
             counts = OrderedDict(Counter(y))
             max_freq = max(counts.values())
             self.sampling_strategy_ = {
-                k: int(np.round(max_freq * self.value))
-                if max_freq * self.value > freq
-                else freq
+                k: (
+                    int(np.round(max_freq * self.value))
+                    if max_freq * self.value > freq
+                    else freq
+                )
                 for k, freq in counts.items()
             }
 
         elif type(self.augmentation_strategy) in [int, float]:
             counts = OrderedDict(Counter(y))
             self.sampling_strategy_ = {
                 k: int(np.round(v * self.augmentation_strategy))
```

### Comparing `ml-research-0.4a2/mlresearch/data_augmentation/tests/test_gsmote.py` & `ml-research-0.5.0/mlresearch/synthetic_data/tests/test_gsmote.py`

 * *Files 1% similar despite different names*

```diff
@@ -321,15 +321,15 @@
 
 # part of the common test which apply to GSMOTE-NC even if it is not default
 # constructible
 def test_smotenc_check_target_type():
     X, _, categorical_features = data_heterogeneous_unordered()
     y = np.linspace(0, 1, 30)
     gsmote = GeometricSMOTE(categorical_features=categorical_features, random_state=0)
-    with pytest.raises(ValueError, match="Unknown label type: 'continuous'"):
+    with pytest.raises(ValueError, match="Unknown label type"):
         gsmote.fit_resample(X, y)
     rng = np.random.RandomState(42)
     y = rng.randint(2, size=(20, 3))
     msg = "Multilabel and multioutput targets are not supported."
     with pytest.raises(ValueError, match=msg):
         gsmote.fit_resample(X, y)
```

### Comparing `ml-research-0.4a2/mlresearch/data_augmentation/tests/test_oversampling_augmentation.py` & `ml-research-0.5.0/mlresearch/synthetic_data/tests/test_oversampling_augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a2/mlresearch/datasets/_binary.py` & `ml-research-0.5.0/mlresearch/datasets/_binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         X, y = check_X_y(data.loc[:, X_columns], data.target)
         if multiplication_factor > 1.0:
             sampling_strategy = self._calculate_ratio(multiplication_factor, y)
             X, y = make_imbalance(
                 X, y, sampling_strategy=sampling_strategy, random_state=RANDOM_STATE
             )
         data = pd.DataFrame(np.column_stack((X, y)))
-        data.iloc[:, -1] = data.iloc[:, -1].astype(int)
+        data[data.columns[-1]] = data[data.columns[-1]].astype(int)
+        data.rename(columns={data.columns[-1]: "target"}, inplace=True)
         return data
 
     def download(self):
         """Download the datasets and append undersampled versions of them."""
         super(ImbalancedBinaryDatasets, self).download()
         undersampled_datasets = []
         for (name, data), factor in list(
@@ -186,25 +187,27 @@
     def fetch_vehicle(self):
         """Download and transform the Vehicle Silhouettes Data Set.
         The minority class is identified as the `1` label
         and the majority class as the rest of the labels.
 
         https://archive.ics.uci.edu/ml/datasets/Statlog+(Vehicle+Silhouettes)
         """
-        data = pd.DataFrame()
+        data = []
         for letter in ascii_lowercase[0:9]:
             partial_data = pd.read_csv(
-                urljoin(FETCH_URLS["vehicle"], "xa%s.dat" % letter),
+                urljoin(
+                    FETCH_URLS["vehicle"].replace("Index", ""), "xa%s.dat" % letter
+                ),
                 header=None,
                 delim_whitespace=True,
             )
             partial_data = partial_data.rename(columns={18: "target"})
             partial_data["target"] = partial_data["target"].isin(["van"]).astype(int)
-            data = data.append(partial_data)
-        return data
+            data.append(partial_data)
+        return pd.concat(data)
 
     def fetch_wine(self):
         """Download and transform the Wine Data Set.
         The minority class is identified as the `2` label
         and the majority class as the rest of the labels.
 
         https://archive.ics.uci.edu/ml/datasets/wine
@@ -345,34 +348,43 @@
         return data
 
     def fetch_arcene(self):
         """Download and transform the Arcene Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Arcene
         """
-        url = FETCH_URLS["arcene"]
+
+        zipped_data = requests.get(FETCH_URLS["arcene"]).content
+        zipped_data = ZipFile(BytesIO(zipped_data))
+
         data, labels = [], []
         for data_type in ("train", "valid"):
             data.append(
                 pd.read_csv(
-                    urljoin(url, f"ARCENE/arcene_{data_type}.data"),
+                    StringIO(
+                        zipped_data.read(f"ARCENE/arcene_{data_type}.data").decode(
+                            "utf-8"
+                        )
+                    ),
                     header=None,
                     sep=" ",
                 ).drop(columns=list(range(1998, 10001)))
             )
             labels.append(
                 pd.read_csv(
-                    urljoin(
-                        url,
-                        ("ARCENE/" if data_type == "train" else "")
-                        + f"arcene_{data_type}.labels",
+                    StringIO(
+                        zipped_data.read(
+                            ("ARCENE/" if data_type == "train" else "")
+                            + f"arcene_{data_type}.labels"
+                        ).decode("utf-8")
                     ),
                     header=None,
                 ).rename(columns={0: "target"})
             )
+
         data = pd.concat(data, ignore_index=True)
         labels = pd.concat(labels, ignore_index=True)
         data = pd.concat([data, labels], axis=1)
         data["target"] = data["target"].isin([1]).astype(int)
         return data
 
     def fetch_audit(self):
```

### Comparing `ml-research-0.4a2/mlresearch/datasets/_multiclass.py` & `ml-research-0.5.0/mlresearch/datasets/_multiclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,24 @@
 # License: MIT
 
 import os
 from os.path import join
 from urllib.parse import urljoin
 from string import ascii_lowercase
 
-from rich.progress import track
+from io import BytesIO, StringIO
+from zipfile import ZipFile
+import tarfile
+import requests
+
 import numpy as np
 import pandas as pd
 
 from .base import Datasets, get_data_home, FETCH_URLS
+from ..utils._utils import _optional_import
 
 
 class ContinuousCategoricalDatasets(Datasets):
     """Class to download, transform and save datasets with both continuous
     and categorical features."""
 
     @staticmethod
@@ -34,22 +39,31 @@
         return pd.concat([X_metric, X_cat, y], axis=1)
 
     def download(self):
         """Download the datasets."""
         self.data_home_ = get_data_home(data_home=self.data_home)
         dataset_prefix = self.__class__.__name__.lower().replace("datasets", "")
 
+        # Get datasets to download
         if self.names == "all":
             func_names = [func_name for func_name in dir(self) if "fetch_" in func_name]
         else:
             func_names = [
                 f"fetch_{name}".lower().replace(" ", "_") for name in self.names
             ]
+
+        # Download datasets
+        try:
+            tqdm = _optional_import("tqdm.auto").tqdm
+            iterable = tqdm(func_names, desc="Datasets")
+        except ImportError:
+            iterable = func_names
+
         self.content_ = []
-        for func_name in track(func_names, description="Datasets"):
+        for func_name in iterable:
             dat_name = func_name.replace("fetch_", "")
             name = dat_name.upper().replace("_", " ")
             file_name = f"{dataset_prefix}_{dat_name}.csv"
 
             if (
                 file_name not in os.listdir(self.data_home_)
                 and self.download_if_missing
@@ -59,26 +73,70 @@
                 df.to_csv(join(self.data_home_, file_name), index=False)
 
             data = pd.read_csv(join(self.data_home_, file_name))
 
             self.content_.append((name, data))
         return self
 
+    def summarize_datasets(self):
+        """
+        Create a summary of the downloaded datasets.
+
+        Returns
+        -------
+        datasets_summary : pd.DataFrame
+            Dataframe with summary statistics of all datasets.
+        """
+
+        datasets_summary = super(
+            ContinuousCategoricalDatasets, self
+        ).summarize_datasets()
+        columns = datasets_summary.columns.tolist()
+
+        # Define summary table columns and empty list
+        summary_columns = ["Metric", "Non-Metric"]
+        extended_summary = []
+
+        # Populate empty list
+        for name, dataset in self.content_:
+            dataset = dataset.drop(columns="target")
+            values = [
+                name,
+                sum(~dataset.columns.str.startswith("cat_")),
+                sum(dataset.columns.str.startswith("cat_")),
+            ]
+            extended_summary.append(values)
+        extended_summary = pd.DataFrame(
+            extended_summary, columns=["Dataset name"] + summary_columns
+        ).set_index("Dataset name")
+        datasets_summary = pd.concat([datasets_summary, extended_summary], axis=1)
+
+        # Reorder columns
+        index = columns.index("Features") + 1
+        columns = [*columns[:index], *summary_columns, *columns[index:]]
+        return datasets_summary[columns]
+
     def fetch_adult(self):
         """Download and transform the Adult Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Adult
         """
         data = pd.read_csv(FETCH_URLS["adult"], header=None, na_values=" ?").dropna()
         data.rename(columns={data.columns[-1]: "target"}, inplace=True)
 
         mapper = {v: k for k, v in enumerate(data.target.unique())}
         data.target = data.target.map(mapper)
 
         categorical_features = [1, 3, 5, 6, 7, 8, 9, 13]
+
+        # Trim spaces in categorical features
+        data.iloc[:, categorical_features] = data.iloc[:, categorical_features].map(
+            lambda x: x.strip()
+        )
+
         return data, categorical_features
 
     def fetch_abalone(self):
         """Download and transform the Abalone Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Abalone
         """
@@ -124,17 +182,27 @@
 
         categorical_features = [0, 1, 5, 9]
         return data, categorical_features
 
     def fetch_census(self):
         """Download and transform the Census-Income (KDD) Data Set.
 
-        https://archive.ics.uci.edu/ml/datasets/Census-Income+%28KDD%29
+        https://archive.ics.uci.edu/dataset/117/census+income+kdd
         """
-        data = pd.read_csv(FETCH_URLS["census"], header=None)
+
+        zipped_data = requests.get(FETCH_URLS["census"]).content
+        zipped_data = ZipFile(BytesIO(zipped_data)).read("census.tar.gz")
+        zipped_data = tarfile.open(fileobj=BytesIO(zipped_data))
+
+        data = pd.read_csv(
+            StringIO(
+                zipped_data.extractfile("census-income.data").read().decode("utf-8")
+            ),
+            header=None,
+        )
 
         categorical_features = (
             list(range(1, 5))
             + list(range(6, 16))
             + list(range(19, 29))
             + list(range(30, 38))
             + [39]
@@ -148,17 +216,15 @@
                 .columns.astype("str")
                 .str.startswith("nom_"),
                 cols_ids,
             )
         ).squeeze()
         data = data.drop(columns=cols_ids).T.reset_index(drop=True).T
         # some rows are dropped; they have rare missing values
-        data = data.iloc[
-            data.applymap(lambda x: x != " Not in universe").all(1).values, :
-        ]
+        data = data.iloc[data.map(lambda x: x != " Not in universe").all(1).values, :]
 
         data.rename(columns={data.columns[-1]: "target"}, inplace=True)
 
         mapper = {v: k for k, v in enumerate(data.target.unique())}
         data.target = data.target.map(mapper)
 
         return data, categorical_features
@@ -494,24 +560,27 @@
         return data
 
     def fetch_vehicle(self):
         """Download and transform the Vehicle Silhouettes Data Set.
 
         https://archive.ics.uci.edu/ml/datasets/Statlog+(Vehicle+Silhouettes)
         """
-        data = pd.DataFrame()
+        data = []
         for letter in ascii_lowercase[0:9]:
             partial_data = pd.read_csv(
-                urljoin(FETCH_URLS["vehicle"], "xa%s.dat" % letter),
+                urljoin(
+                    FETCH_URLS["vehicle"].replace("Index", ""), "xa%s.dat" % letter
+                ),
                 header=None,
                 delim_whitespace=True,
             )
             partial_data = partial_data.rename(columns={18: "target"})
-            data = data.append(partial_data)
+            data.append(partial_data)
 
+        data = pd.concat(data)
         mapper = {v: k for k, v in enumerate(data.target.unique())}
         data.target = data.target.map(mapper)
 
         return data
 
     def fetch_asp_potassco(self):
         """Download and transform the ASP-POTASSCO Data Set.
```

### Comparing `ml-research-0.4a2/mlresearch/datasets/_remote_sensing.py` & `ml-research-0.5.0/mlresearch/datasets/_remote_sensing.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,37 +7,32 @@
 
 import io
 import requests
 import numpy as np
 from scipy.io import loadmat
 
 from .base import Datasets, FETCH_URLS
-from ..utils import img_array_to_pandas
+from ..utils import image_to_dataframe
 
 
 class RemoteSensingDatasets(Datasets):
     """Class to download, transform and save remote sensing datasets."""
 
     def __init__(
         self,
         names: str = "all",
-        return_coords: bool = False,
         data_home: str = None,
         download_if_missing: bool = True,
     ):
         """
         Parameters
         ----------
         names : str or list, default="all"
             List of dataset names to be downloaded. If ``all``, downloads all datasets.
 
-        return_coords : bool, default=False
-            If ``True``, two columns with x and y coordinates will be added to the
-            dataframe.
-
         data_home : str, default=None
             The path to the data directory. If `None`, the default path
             is `~/ml_research_data`.
 
         download_if_missing : bool, default=True
             If True, downloads the dataset from the internet and puts it in
             ``data_home``. If the dataset is already downloaded, it is not downloaded
@@ -48,30 +43,23 @@
         data_home_ : str
             Path were the data was stored.
 
         content_ : list
             List of tuples composed of (Dataset name, Dataframe).
         """
         self.names = names
-        self.return_coords = return_coords
         self.data_home = data_home
         self.download_if_missing = download_if_missing
 
     def download(self):
         """Download the datasets and append undersampled versions of them."""
-        super(RemoteSensingDatasets, self).download()
+        super(RemoteSensingDatasets, self).download(keep_index=True)
         content_ = []
-        for (name, data) in self.content_:
-            if not self.return_coords:
-                data = data.iloc[:, 2:]
-                new_cols = list(range(len(data.columns) - 1)) + ["target"]
-            else:
-                new_cols = ["x", "y"] + list(range(len(data.columns) - 3)) + ["target"]
-
-            data.columns = new_cols
+        for name, data in self.content_:
+            data = data.set_index(["h", "w"])
             content_.append((name, data))
         self.content_ = content_
 
         return self
 
     def _load_gic_dataset(self, dataset_name):
         for url in FETCH_URLS[dataset_name]:
@@ -86,63 +74,63 @@
 
     def fetch_indian_pines(self):
         """Download and transform the Indian Pines Data Set. Label "0" means
         the pixel is not labelled. It is therefore dropped.
 
         http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Indian_Pines
         """
-        df = img_array_to_pandas(*self._load_gic_dataset("indian_pines"))
+        df = image_to_dataframe(*self._load_gic_dataset("indian_pines"))
         return df[df.target != 0]
 
     def fetch_salinas(self):
         """Download and transform the Salinas Data Set. Label "0" means the pixel is
         not labelled. It is therefore dropped.
 
         http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Salinas_scene
         """
-        df = img_array_to_pandas(*self._load_gic_dataset("salinas"))
+        df = image_to_dataframe(*self._load_gic_dataset("salinas"))
         return df[df.target != 0]
 
     def fetch_salinas_a(self):
         """Download and transform the Salinas-A Data Set. Label "0" means the pixel is
         not labelled. It is therefore dropped.
 
         http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Salinas-A_scene
         """
-        df = img_array_to_pandas(*self._load_gic_dataset("salinas_a"))
+        df = image_to_dataframe(*self._load_gic_dataset("salinas_a"))
         return df[df.target != 0]
 
     def fetch_pavia_centre(self):
         """Download and transform the Pavia Centre Data Set. Label "0" means the pixel
         is not labelled. It is therefore dropped.
 
         http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Pavia_Centre_scene
         """
-        df = img_array_to_pandas(*self._load_gic_dataset("pavia_centre"))
+        df = image_to_dataframe(*self._load_gic_dataset("pavia_centre"))
         return df[df.target != 0]
 
     def fetch_pavia_university(self):
         """Download and transform the Pavia University Data Set. Label "0"
         means the pixel is not labelled. It is therefore dropped.
 
         http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Pavia_University_scene
         """
-        df = img_array_to_pandas(*self._load_gic_dataset("pavia_university"))
+        df = image_to_dataframe(*self._load_gic_dataset("pavia_university"))
         return df[df.target != 0]
 
     def fetch_kennedy_space_center(self):
         """Download and transform the Kennedy Space Center Data Set. Label "0"
         means the pixel is not labelled. It is therefore dropped.
 
         http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Kennedy_Space_Center_.28KSC.29
         """
-        df = img_array_to_pandas(*self._load_gic_dataset("kennedy_space_center"))
+        df = image_to_dataframe(*self._load_gic_dataset("kennedy_space_center"))
         return df[df.target != 0]
 
     def fetch_botswana(self):
         """Download and transform the Botswana Data Set. Label "0" means the pixel is
         not labelled. It is therefore dropped.
 
         http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes#Botswana
         """
-        df = img_array_to_pandas(*self._load_gic_dataset("botswana"))
+        df = image_to_dataframe(*self._load_gic_dataset("botswana"))
         return df[df.target != 0]
```

### Comparing `ml-research-0.4a2/mlresearch/datasets/base.py` & `ml-research-0.5.0/mlresearch/datasets/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 """
 Download, transform and simulate various datasets.
+
+Part of the code was adapted from
+https://github.com/NOVA-IMS-Innovation-and-Analytics-Lab/publications
 """
 
-# Author: Georgios Douzas <gdouzas@icloud.com>
-#         Joao Fonseca <jpfonseca@novaims.unl.pt>
+# Author: Joao Fonseca <jpfonseca@novaims.unl.pt>
 # License: MIT
 
 from typing import Optional, Union
 import os
 from os.path import expanduser, join
 from collections import Counter
 from urllib.parse import urljoin
 from sqlite3 import connect
-from rich.progress import track
 import numpy as np
 import pandas as pd
 from sklearn.utils import check_X_y
 from imblearn.datasets import make_imbalance
 
+from mlresearch.utils._utils import _optional_import
+
 UCI_URL = "https://archive.ics.uci.edu/ml/machine-learning-databases/"
+UCI_URL2 = "https://archive.ics.uci.edu/static/public/"
 GIC_URL = "http://www.ehu.eus/ccwintco/uploads/"
 OPENML_URL = "https://www.openml.org/data/get_csv/"
 FETCH_URLS = {
     "breast_tissue": urljoin(UCI_URL, "00192/BreastTissue.xls"),
     "ecoli": urljoin(UCI_URL, "ecoli/ecoli.data"),
     "eucalyptus": urljoin(OPENML_URL, "3625/dataset_194_eucalyptus.arff"),
     "glass": urljoin(UCI_URL, "glass/glass.data"),
     "haberman": urljoin(UCI_URL, "haberman/haberman.data"),
     "heart": urljoin(UCI_URL, "statlog/heart/heart.dat"),
     "iris": urljoin(UCI_URL, "iris/bezdekIris.data"),
     "libras": urljoin(UCI_URL, "libras/movement_libras.data"),
     "liver": urljoin(UCI_URL, "liver-disorders/bupa.data"),
     "pima": "https://gist.githubusercontent.com/ktisha/c21e73a1bd1700294ef790c56c8aec1f"
     "/raw/819b69b5736821ccee93d05b51de0510bea00294/pima-indians-diabetes.csv",
-    "vehicle": urljoin(UCI_URL, "statlog/vehicle/"),
+    "vehicle": urljoin(UCI_URL, "statlog/vehicle/Index"),
     "wine": urljoin(UCI_URL, "wine/wine.data"),
     "new_thyroid": urljoin(UCI_URL, "thyroid-disease/new-thyroid.data"),
     "cleveland": urljoin(UCI_URL, "heart-disease/processed.cleveland.data"),
     "led": urljoin(OPENML_URL, "4535757/phpSj3fWL"),
     "page_blocks": urljoin(OPENML_URL, "30/dataset_30_page-blocks.arff"),
     "yeast": urljoin(UCI_URL, "yeast/yeast.data"),
     "banknote_authentication": urljoin(
         UCI_URL, "00267/data_banknote_authentication.txt"
     ),
-    "arcene": urljoin(UCI_URL, "arcene/"),
+    "arcene": urljoin(UCI_URL2, "167/arcene.zip"),
     "audit": urljoin(UCI_URL, "00475/audit_data.zip"),
     "spambase": urljoin(UCI_URL, "spambase/spambase.data"),
     "parkinsons": urljoin(UCI_URL, "parkinsons/parkinsons.data"),
     "ionosphere": urljoin(UCI_URL, "ionosphere/ionosphere.data"),
     "breast_cancer": urljoin(UCI_URL, "breast-cancer-wisconsin/wdbc.data"),
     "adult": urljoin(UCI_URL, "adult/adult.data"),
     "abalone": urljoin(UCI_URL, "abalone/abalone.data"),
     "acute": urljoin(UCI_URL, "acute/diagnosis.data"),
     "annealing": urljoin(UCI_URL, "annealing/anneal.data"),
-    "census": urljoin(UCI_URL, "census-income-mld/census-income.data.gz"),
+    "census": urljoin(UCI_URL2, "117/census+income+kdd.zip"),
     "contraceptive": urljoin(UCI_URL, "cmc/cmc.data"),
     "covertype": urljoin(UCI_URL, "covtype/covtype.data.gz"),
     "credit_approval": urljoin(UCI_URL, "credit-screening/crx.data"),
     "dermatology": urljoin(UCI_URL, "dermatology/dermatology.data"),
     "echocardiogram": urljoin(UCI_URL, "echocardiogram/echocardiogram.data"),
     "flags": urljoin(UCI_URL, "flags/flag.data"),
     "heart_disease": [
@@ -177,19 +181,41 @@
         content_ : list
             List of tuples composed of (Dataset name, Dataframe).
         """
         self.names = names
         self.data_home = data_home
         self.download_if_missing = download_if_missing
 
+    def __getitem__(self, i):
+        if type(i) is str:
+            return dict(self.content_)[i]
+        else:
+            return self.content_[i]
+
+    def __setitem__(self, key, value):
+        self.content_.append((key, value))
+        return self
+
+    def __len__(self):
+        return len(self.content_)
+
+    def keys(self):
+        return dict(self.content_).keys()
+
+    def values(self):
+        return dict(self.content_).values()
+
+    def items(self):
+        return dict(self.content_).items()
+
     @staticmethod
-    def _modify_columns(data):
+    def _modify_columns(data, keep_index=False):
         """Rename and reorder columns of dataframe."""
         X, y = data.drop(columns="target"), data.target
-        X.columns = range(len(X.columns))
+        X.columns = X.columns if keep_index else range(len(X.columns))
         return pd.concat([X, y], axis=1)
 
     @staticmethod
     def _calculate_sampling_strategy(ir, y):
         """Calculate ratio based on the IR."""
         ratio = Counter(y).most_common()
         b = ratio[0][1]
@@ -201,58 +227,68 @@
             f_new = int(np.clip(m * x + b, 1, f))
             sampling_strategy[c] = f_new
 
         return sampling_strategy
 
     def _make_imbalance(self, data, sampling_strategy, random_state=None):
         """Undersample the minority class."""
-        X_columns = [col for col in data.columns if col != "target"]
-        X, y = check_X_y(data.loc[:, X_columns], data.target, dtype=None)
+        X, y = check_X_y(data.drop(columns="target"), data["target"], dtype=None)
         X, y = make_imbalance(
             X, y, sampling_strategy=sampling_strategy, random_state=random_state
         )
         data = pd.DataFrame(np.column_stack((X, y)))
-        data.iloc[:, -1] = data.iloc[:, -1].astype(int)
+        data[data.columns[-1]] = data[data.columns[-1]].astype(int)
         return data
 
-    def download(self):
+    def download(self, keep_index=False):
         """Download the datasets."""
         self.data_home_ = get_data_home(data_home=self.data_home)
         dataset_prefix = self.__class__.__name__.lower().replace("datasets", "")
 
+        # Get datasets to download
         if self.names == "all":
             func_names = [func_name for func_name in dir(self) if "fetch_" in func_name]
         else:
             func_names = [
                 f"fetch_{name}".lower().replace(" ", "_") for name in self.names
             ]
+
+        # Download datasets
+        try:
+            tqdm = _optional_import("tqdm.auto").tqdm
+            iterable = tqdm(func_names, desc="Datasets")
+        except ImportError:
+            iterable = func_names
+
         self.content_ = []
-        for func_name in track(func_names, description="Datasets"):
+        for func_name in iterable:
             dat_name = func_name.replace("fetch_", "")
             name = dat_name.upper().replace("_", " ")
             file_name = f"{dataset_prefix}_{dat_name}.csv"
 
+            # Save file locally if it doesn't exist
             if (
                 file_name not in os.listdir(self.data_home_)
                 and self.download_if_missing
             ):
                 df = getattr(self, func_name)()
-                df.to_csv(join(self.data_home_, file_name), index=False)
+                df.to_csv(join(self.data_home_, file_name), index=keep_index)
 
             data = pd.read_csv(join(self.data_home_, file_name))
-            data = self._modify_columns(data)
+            data = self._modify_columns(data, keep_index=keep_index)
             self.content_.append((name, data))
         return self
 
     def imbalance_datasets(self, imbalance_ratio: float, random_state: int = None):
         """
         Appends imbalanced versions of datasets with predefined imbalance ratios to
         ``self.content_``.
 
-        $IR = \frac{|C_{maj}|}{|C_{min}|}$
+        .. math::
+            IR = \\frac{|C_{maj}|}{|C_{min}|}
 
         Parameters
         ----------
         imbalance_ratio : float
             Final Imbalance Ratio expected in the datasets.
 
         random_state : int, RandomState instance, default=None
@@ -263,15 +299,15 @@
             - If ``RandomState`` instance, random_state is the random number
               generator;
             - If ``None``, the random number generator is the ``RandomState``
               instance used by ``np.random``.
 
         Returns
         -------
-        self
+        self : Datasets
 
         """
         imbalanced_content = []
         base_content = [
             dataset for dataset in self.content_ if not dataset[0].endswith(")")
         ]
         for name, data in base_content:
@@ -292,31 +328,40 @@
             if name_imb not in dict(self.content_).keys() and base_ir < new_ir:
                 imbalanced_content.append((name_imb, data_imb))
 
         self.content_.extend(imbalanced_content)
         return self
 
     def summarize_datasets(self):
-        """Create a summary of the downloaded datasets."""
+        """
+        Create a summary of the downloaded datasets.
+
+        Returns
+        -------
+        datasets_summary : pd.DataFrame
+            Dataframe with summary statistics of all datasets.
+        """
 
         # Check datasets format
         datasets = [
-            (name, (data.drop(columns="target"), data.target))
-            if type(data) == pd.DataFrame
-            else data
+            (
+                (name, (data.drop(columns="target"), data.target))
+                if type(data) is pd.DataFrame
+                else data
+            )
             for name, data in self.content_
         ]
 
         # Define summary table columns
         summary_columns = [
             "Dataset name",
             "Features",
-            "Instances",
-            "Minority instances",
-            "Majority instances",
+            "Observations",
+            "Minority Obs.",
+            "Majority Obs.",
             "Imbalance Ratio",
             "Classes",
         ]
 
         # Define empty summary table
         datasets_summary = []
 
@@ -340,16 +385,16 @@
         # Cast to integer columns
         int_cols = datasets_summary.columns.drop(["Dataset name", "Imbalance Ratio"])
         datasets_summary.loc[:, int_cols] = datasets_summary.loc[:, int_cols].astype(
             int
         )
 
         # Sort datasets summary
-        datasets_summary = datasets_summary.sort_values("Imbalance Ratio").reset_index(
-            drop=True
+        datasets_summary = datasets_summary.sort_values("Imbalance Ratio").set_index(
+            "Dataset name"
         )
 
         return datasets_summary
 
     def save(self, path, db_name):
         """Save datasets."""
         with connect(join(path, f"{db_name}.db")) as connection:
```

### Comparing `ml-research-0.4a2/mlresearch/metrics/_metrics.py` & `ml-research-0.5.0/mlresearch/metrics/_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import numpy as np
-from sklearn.metrics import SCORERS, make_scorer
-from sklearn.metrics._scorer import _PredictScorer
+from sklearn.metrics import make_scorer
+from sklearn.metrics._scorer import _Scorer, _SCORERS
 from imblearn.metrics import geometric_mean_score
 
 
-class ALScorer(_PredictScorer):
+class ALScorer(_Scorer):
     """
     Make an Active Learning scorer from a AL-specific metric or loss function.
 
     This factory class wraps scoring functions to be used in
     :class:`~rlearn.model_selection.ModelSearchCV` and
     :class:`~sklearn.model_selection.GridSearchCV`. It takes a score function, such as
-    :func:`~research.metrics.area_under_learning_curve` or
-    :func:`~research.metrics.data_utilization_rate` and is used to score an AL
+    :func:`~mlresearch.metrics.area_under_learning_curve` or
+    :func:`~mlresearch.metrics.data_utilization_rate` and is used to score an AL
     simulation. The signature of the call is `(estimator, X, y)` where `estimator` is the
     model to be evaluated, `X` is the data and `y` is the ground truth labeling (or
     `None` in the case of unsupervised models).
 
     Parameters
     ----------
     score_func : callable
@@ -28,16 +28,18 @@
 
     Returns
     -------
     scorer : callable
         Callable object that returns a scalar score.
     """
 
-    def __init__(self, score_func):
-        super().__init__(score_func=score_func, sign=1, kwargs={})
+    def __init__(self, score_func, sign=1, **kwargs):
+        self._score_func = score_func
+        self._sign = sign
+        self._kwargs = kwargs
 
     def _score(self, method_caller, estimator, X, y_true, sample_weight=None):
         """Evaluate predicted target values for X relative to y_true.
         Parameters
         ----------
         method_caller : callable
             Returns predictions given an estimator, method name, and other
@@ -58,39 +60,50 @@
             Score function applied to prediction of estimator on X.
         """
 
         metadata = estimator.metadata_
 
         return self._sign * self._score_func(metadata)
 
+    def set_score_request(self):
+        """
+        Placeholder to overwrite sklearn's ``_BaseScorer.set_score_request`` function.
+        It is not used and was raising a docstring error with scikit-learn v1.3.0.
+
+        Note
+        ----
+        This placeholder will be removed soon
+        """
+        pass
+
 
 def geometric_mean_score_macro(y_true, y_pred):
     """Geometric mean score with macro average."""
     return geometric_mean_score(y_true, y_pred, average="macro")
 
 
 def area_under_learning_curve(metadata, *args):
     """Area under the learning curve. Used in Active Learning experiments."""
-    iterations = np.sort([i for i in metadata.keys() if type(i) == int])[1:]
+    iterations = np.sort([i for i in metadata.keys() if type(i) is int])[1:]
     test_scores = [metadata[i]["test_score"] for i in iterations]
     auc = np.sum(test_scores) / len(test_scores)
     return auc
 
 
 def data_utilization_rate(metadata, threshold=0.8):
     """Data Utilization Rate. Used in Active Learning Experiments."""
-    iterations = np.sort([i for i in metadata.keys() if type(i) == int])[1:]
+    iterations = np.sort([i for i in metadata.keys() if type(i) is int])[1:]
     test_scores = [metadata[i]["test_score"] for i in iterations]
     n_obs = metadata["data"][0].shape[0]
     data_utilization = [
         metadata[i - 1]["labeled_pool"].sum() / n_obs for i in iterations
     ]
 
     indices = np.where(np.array(test_scores) >= threshold)[0]
     arg = indices[0] if len(indices) != 0 else -1
     dur = data_utilization[arg] if arg != -1 else np.nan
     return dur
 
 
-SCORERS["geometric_mean_score_macro"] = make_scorer(geometric_mean_score_macro)
-SCORERS["area_under_learning_curve"] = ALScorer(area_under_learning_curve)
-SCORERS["data_utilization_rate"] = ALScorer(data_utilization_rate)
+_SCORERS["geometric_mean_score_macro"] = make_scorer(geometric_mean_score_macro)
+_SCORERS["area_under_learning_curve"] = ALScorer(area_under_learning_curve)
+_SCORERS["data_utilization_rate"] = ALScorer(data_utilization_rate)
```

### Comparing `ml-research-0.4a2/mlresearch/metrics/tests/test_metrics.py` & `ml-research-0.5.0/mlresearch/metrics/tests/test_metrics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Test performance metrics"""
 
 # Author: Joao Fonseca <jpfonseca@novaims.unl.pt>
 
 import pytest
 import numpy as np
 from sklearn.utils._testing import ignore_warnings
+from sklearn.linear_model import LogisticRegression
 
-from ...active_learning import StandardAL
-from .._metrics import (
+from mlresearch.active_learning import StandardAL
+from mlresearch.metrics._metrics import (
     ALScorer,
     geometric_mean_score_macro,
     area_under_learning_curve,
     data_utilization_rate,
 )
+from mlresearch.metrics._rankings import RankingScorer, precision_at_k
 
 RANDOM_STATE = 42
 
 # toy sample
 X = [[-2, -1], [-1, -1], [-1, -2], [1, 1], [1, 2], [2, 1]]
 y = [-1, -1, -1, 1, 1, 1]
 T = [[-1, -1], [2, 2], [3, 2]]
@@ -55,7 +57,19 @@
 
 def test_al_metrics():
     al_model = StandardAL(random_state=RANDOM_STATE)
     al_model.fit(X, y, X_test=T, y_test=true_result)
 
     assert ALScorer(data_utilization_rate)(al_model, None, None) == 1 / 3
     assert ALScorer(area_under_learning_curve)(al_model, None, None) == 1
+
+
+def test_rank_metrics():
+    y_score = [0.7, 0.1, 0.5]
+    assert precision_at_k(true_result, y_score, k=1) == 0.0
+    assert precision_at_k(true_result, y_score, k=2) == 0.5
+    assert precision_at_k(true_result, y_score, k=3) == 2 / 3
+
+    # Check if scorer is being created properly
+    clf = LogisticRegression().fit(X, y)
+    assert RankingScorer(precision_at_k, k=3)(clf, T, true_result) == 2 / 3
+    assert RankingScorer(precision_at_k, k=2)(clf, T, true_result) == 1
```

### Comparing `ml-research-0.4a2/mlresearch/tests/test_docstring_parameters.py` & `ml-research-0.5.0/mlresearch/tests/test_docstring_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,31 @@
 from sklearn.datasets import make_classification
 from sklearn.linear_model import LogisticRegression
 from sklearn.utils import IS_PYPY
 from sklearn.utils._testing import check_docstring_parameters
 from sklearn.utils._testing import _get_func_name
 from sklearn.utils._testing import ignore_warnings
 from sklearn.utils.estimator_checks import _enforce_estimator_tags_y
-from sklearn.utils.estimator_checks import _enforce_estimator_tags_x
+from sklearn.utils.estimator_checks import _enforce_estimator_tags_X
 from sklearn.utils.estimator_checks import _construct_instance
 from sklearn.utils.deprecation import _is_deprecated
 
 import mlresearch
 from mlresearch.utils._testing import all_estimators
 
 
 def is_sampler(estimator):
-    """Return True if the given estimator is a sampler, False otherwise.
+    """
+    Return True if the given estimator is a sampler, False otherwise.
+
     Parameters
     ----------
     estimator : object
         Estimator to test.
+
     Returns
     -------
     is_sampler : bool
         True if estimator is a sampler, otherwise False.
     """
     if estimator._estimator_type == "sampler":
         return True
@@ -50,15 +53,15 @@
             pckg[1]
             for pckg in walk_packages(prefix="mlresearch.", path=imblearn_path)
             if not ("._" in pckg[1] or ".tests." in pckg[1])
         ]
     )
 
 # functions to ignore args / docstring of
-_DOCSTRING_IGNORES = []
+_DOCSTRING_IGNORES = []  # type: ignore
 
 # Methods where y param should be ignored if y=None by default
 _METHODS_IGNORE_NONE_Y = [
     "fit",
     "score",
     "fit_predict",
     "fit_transform",
@@ -66,15 +69,15 @@
     "predict",
 ]
 
 
 @pytest.mark.filterwarnings("ignore::FutureWarning")
 @pytest.mark.filterwarnings("ignore::DeprecationWarning")
 @pytest.mark.skipif(IS_PYPY, reason="test segfaults on PyPy")
-def test_docstring_parameters():
+def test_docstring_parameters():  # noqa: C901
     # Test module docstring formatting
 
     # Skip test if numpydoc is not found
     pytest.importorskip(
         "numpydoc", reason="numpydoc is required to test the docstrings"
     )
 
@@ -148,15 +151,14 @@
 
 @ignore_warnings(category=FutureWarning)
 def test_tabs():
     # Test that there are no tabs in our source files
     for importer, modname, ispkg in walk_packages(
         mlresearch.__path__, prefix="mlresearch."
     ):
-
         if IS_PYPY:
             continue
 
         # because we don't import
         mod = importlib.import_module(modname)
 
         try:
@@ -171,14 +173,15 @@
 
 def _construct_compose_pipeline_instance(Estimator):
     # Minimal / degenerate instances: only useful to test the docstrings.
     if Estimator.__name__ == "Pipeline":
         return Estimator(steps=[("clf", LogisticRegression())])
 
 
+@pytest.mark.filterwarnings("ignore::UserWarning")
 @pytest.mark.parametrize("name, Estimator", all_estimators())
 def test_fit_docstring_attributes(name, Estimator):
     pytest.importorskip("numpydoc")
     from numpydoc import docscrape
 
     if Estimator.__name__ in _DOCSTRING_IGNORES:
         return
@@ -196,15 +199,15 @@
         n_features=3,
         n_redundant=0,
         n_classes=2,
         random_state=2,
     )
 
     y = _enforce_estimator_tags_y(est, y)
-    X = _enforce_estimator_tags_x(est, X)
+    X = _enforce_estimator_tags_X(est, X)
 
     if "oob_score" in est.get_params():
         est.set_params(oob_score=True)
 
     if is_sampler(est):
         est.fit_resample(X, y)
     else:
```

### Comparing `ml-research-0.4a2/mlresearch/utils/_data.py` & `ml-research-0.5.0/mlresearch/utils/_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Data I/O utils. Later on I might add other data handling utilities.
 """
+
 from os import listdir
 from os.path import isdir, join
 import pandas as pd
 from sqlite3 import connect
 
 
 def load_datasets(
```

### Comparing `ml-research-0.4a2/mlresearch/utils/_testing.py` & `ml-research-0.5.0/mlresearch/utils/_testing.py`

 * *Files identical despite different names*

### Comparing `ml-research-0.4a2/mlresearch/utils/tests/test_check_pipelines.py` & `ml-research-0.5.0/mlresearch/utils/tests/test_check_pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test the check_pipelines module.
 """
+
 from itertools import product
 
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.decomposition import PCA
 from sklearn.datasets import load_iris
 from imblearn.over_sampling import SMOTE, BorderlineSMOTE
@@ -13,27 +14,29 @@
 
 from .._check_pipelines import (
     check_pipelines,
     check_pipelines_wrapper,
     check_random_states,
 )
 from ...active_learning import StandardAL
-from ...data_augmentation import OverSamplingAugmentation
+from ...synthetic_data import OverSamplingAugmentation
 
 
 def test_check_pipeline_single():
     """Test the check of pipelines with a single element."""
 
     # Initialization
     n_runs = 5
     rnd_seed = 0
     classifiers = [("clf", DecisionTreeClassifier(), {"max_depth": [3, 5]})]
 
     # Estimators and parameters grids
-    estimators, param_grids = check_pipelines([classifiers], rnd_seed, n_runs)
+    estimators, param_grids = check_pipelines(
+        classifiers, random_state=rnd_seed, n_runs=n_runs
+    )
     names, pips = zip(*estimators)
     steps = [
         [(step[0], step[1].__class__.__name__) for step in pip.steps] for pip in pips
     ]
 
     # Expected estimators and parameters grids
     exp_name = "clf"
@@ -74,15 +77,15 @@
     oversamplers = [
         ("ovs", BorderlineSMOTE(), [{"k_neighbors": [2, 4]}, {"m_neighbors": [6, 8]}])
     ]
     classifiers = [("clf", DecisionTreeClassifier(), {"max_depth": [3, 5]})]
 
     # Estimators and parameters grids
     estimators, param_grids = check_pipelines(
-        [oversamplers, classifiers], rnd_seed, n_runs
+        oversamplers, classifiers, random_state=rnd_seed, n_runs=n_runs
     )
     names, pips = zip(*estimators)
     steps = [
         [(step[0], step[1].__class__.__name__) for step in pip.steps] for pip in pips
     ]
 
     # Expected estimators and parameters grids
@@ -130,15 +133,15 @@
     n_runs = 2
     rnd_seed = 12
     oversamplers = [("ovs", None, {})]
     classifiers = [("clf", DecisionTreeClassifier(), {"max_depth": [3, 5, 8]})]
 
     # Estimators and parameters grids
     estimators, param_grids = check_pipelines(
-        [oversamplers, classifiers], rnd_seed, n_runs
+        oversamplers, classifiers, random_state=rnd_seed, n_runs=n_runs
     )
     names, pips = zip(*estimators)
     steps = [
         [(step[0], step[1].__class__.__name__) for step in pip.steps] for pip in pips
     ]
 
     # Expected names, steps and parameter grids
@@ -177,15 +180,15 @@
             Pipeline([("pca", PCA()), ("dtc", DecisionTreeClassifier())]),
             {"pca__n_components": [4, 8], "dtc__max_depth": [3, 5]},
         )
     ]
 
     # Estimators and parameters grids
     estimators, param_grids = check_pipelines(
-        [scalers, oversamplers, classifiers], rnd_seed, n_runs
+        scalers, oversamplers, classifiers, random_state=rnd_seed, n_runs=n_runs
     )
     names, pips = zip(*estimators)
     steps = [
         [(step[0], step[1].__class__.__name__) for step in pip.steps] for pip in pips
     ]
 
     # Expected names, steps and parameter grids
@@ -249,19 +252,24 @@
     al_model = (
         "AL-TEST",
         StandardAL(max_iter=2),
         {"acquisition_func": ["random", "entropy", "breaking_ties"]},
     )
 
     we_wpg = check_pipelines_wrapper(
-        [classifiers], al_model, random_state=rnd_seed, n_runs=n_runs, wrapped_only=True
+        classifiers,
+        wrapper=al_model,
+        random_state=rnd_seed,
+        n_runs=n_runs,
+        wrapped_only=True,
     )
 
     we_wpg2 = check_pipelines_wrapper(
-        [oversamplers, classifiers],
-        al_model,
+        oversamplers,
+        classifiers,
+        wrapper=al_model,
         random_state=rnd_seed,
         n_runs=n_runs,
         wrapped_only=True,
     )
     for we, wpg in [we_wpg, we_wpg2]:
         ModelSearchCV(estimators=we, cv=2, param_grids=wpg, n_jobs=-1).fit(X, y)
```

### Comparing `ml-research-0.4a2/mlresearch/utils/tests/test_load_datasets.py` & `ml-research-0.5.0/mlresearch/utils/tests/test_load_datasets.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,18 @@
     all_datasets = load_datasets(".", target_exists=False)
 
     # delete data files
     files = [f"{name}_data_file.csv" for name in DATASET_NAMES] + [
         "sample_data_base.db"
     ]
     for file in files:
-        remove(file)
+        try:
+            remove(file)
+        except PermissionError:
+            pass
 
     exp_csv_datasets = [f"{name.upper()} DATA FILE" for name in DATASET_NAMES]
     exp_db_datasets = [name.upper() for name in DATASET_NAMES]
     exp_all_datasets = [*exp_db_datasets, *exp_csv_datasets]
 
     assert len(csv_datasets) == len(DATASET_NAMES)
     assert len(db_datasets) == len(DATASET_NAMES)
```

### Comparing `ml-research-0.4a2/setup.py` & `ml-research-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,17 +43,18 @@
     "Programming Language :: Python",
     "Topic :: Software Development",
     "Topic :: Scientific/Engineering",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: MacOS",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 INSTALL_REQUIRES = (min_deps.tag_to_packages["install"],)
 EXTRAS_REQUIRE = {
     key: value for key, value in min_deps.tag_to_packages.items() if key != "install"
 }
 
 setup(
```

