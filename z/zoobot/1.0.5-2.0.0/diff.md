# Comparing `tmp/zoobot-1.0.5.tar.gz` & `tmp/zoobot-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoobot-1.0.5.tar", last modified: Mon Nov 13 20:16:09 2023, max compression
+gzip compressed data, was "zoobot-2.0.0.tar", last modified: Thu Apr  4 19:51:51 2024, max compression
```

## Comparing `zoobot-1.0.5.tar` & `zoobot-2.0.0.tar`

### file list

```diff
@@ -1,72 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.060448 zoobot-1.0.5/
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2023-11-13 20:15:56.000000 zoobot-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16383 2023-11-13 20:16:09.056448 zoobot-1.0.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    13090 2023-11-13 20:15:56.000000 zoobot-1.0.5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      103 2023-11-13 20:15:56.000000 zoobot-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 20:16:09.060448 zoobot-1.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     4088 2023-11-13 20:15:56.000000 zoobot-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.036448 zoobot-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2023-11-13 20:15:56.000000 zoobot-1.0.5/tests/test_loss_equivalence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.036448 zoobot-1.0.5/zoobot/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.036448 zoobot-1.0.5/zoobot/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.036448 zoobot-1.0.5/zoobot/pytorch/estimators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/estimators/cuda_check.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1604 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/estimators/custom_layers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16180 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/estimators/define_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3188 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/estimators/efficientnet_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/manchester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.040448 zoobot-1.0.5/zoobot/pytorch/predictions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/predictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/predictions/predict_on_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.040448 zoobot-1.0.5/zoobot/pytorch/training/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23061 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/training/finetune.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5860 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/training/representations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/training/tensorboard_writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16300 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/pytorch/training/train_with_pytorch_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.044448 zoobot-1.0.5/zoobot/shared/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/shared/benchmark_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4437 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/shared/compress_representations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/shared/label_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11035 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/shared/load_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2844 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/shared/save_predictions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12003 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/shared/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/shared/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.044448 zoobot-1.0.5/zoobot/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.044448 zoobot-1.0.5/zoobot/tensorflow/estimators/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/estimators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2508 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/estimators/alexnet_baseline.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1795 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/estimators/custom_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1370 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/estimators/custom_layers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7227 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/estimators/define_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2300 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/estimators/efficientnet_custom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    84167 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/estimators/efficientnet_standard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/estimators/small_cnn_baseline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.044448 zoobot-1.0.5/zoobot/tensorflow/predictions/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/predictions/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3417 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/predictions/predict_on_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5239 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.044448 zoobot-1.0.5/zoobot/tensorflow/stats/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/stats/coverage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14433 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/stats/dirichlet_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3526 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/stats/mixture_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.048448 zoobot-1.0.5/zoobot/tensorflow/training/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/training/custom_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/training/finetune.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6772 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/training/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/training/train_with_keras.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6505 2023-11-13 20:15:56.000000 zoobot-1.0.5/zoobot/tensorflow/training/training_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 20:16:09.036448 zoobot-1.0.5/zoobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16383 2023-11-13 20:16:08.000000 zoobot-1.0.5/zoobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-11-13 20:16:08.000000 zoobot-1.0.5/zoobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 20:16:08.000000 zoobot-1.0.5/zoobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-11-13 20:16:08.000000 zoobot-1.0.5/zoobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-13 20:16:08.000000 zoobot-1.0.5/zoobot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:51.006094 zoobot-2.0.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-04-04 19:51:42.000000 zoobot-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-04-04 19:51:51.006094 zoobot-2.0.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12454 2024-04-04 19:51:42.000000 zoobot-2.0.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      103 2024-04-04 19:51:42.000000 zoobot-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:51:51.010094 zoobot-2.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4602 2024-04-04 19:51:42.000000 zoobot-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.990094 zoobot-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-04 19:51:42.000000 zoobot-2.0.0/tests/test_from_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-04 19:51:42.000000 zoobot-2.0.0/tests/test_loss_equivalence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.990094 zoobot-2.0.0/zoobot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/datasets/webdatamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/datasets/webdataset_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/cuda_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1604 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/custom_layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22399 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/define_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3188 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/estimators/efficientnet_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/manchester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/predictions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/predictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/predictions/predict_on_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.994094 zoobot-2.0.0/zoobot/pytorch/training/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38788 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/finetune.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6800 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/tensorboard_writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19378 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/pytorch/training/train_with_pytorch_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/benchmark_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4437 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/compress_representations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/label_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/load_predictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3233 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/save_predictions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12868 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/shared/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/tensorflow/estimators/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2508 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/alexnet_baseline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1795 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/custom_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1370 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/custom_layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7227 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/define_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2300 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/efficientnet_custom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    84167 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/efficientnet_standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1134 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/estimators/small_cnn_baseline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/tensorflow/predictions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/predictions/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3417 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/predictions/predict_on_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5239 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:50.998094 zoobot-2.0.0/zoobot/tensorflow/stats/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/stats/coverage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14433 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/stats/dirichlet_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3526 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/stats/mixture_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:51.002094 zoobot-2.0.0/zoobot/tensorflow/training/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/custom_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/finetune.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6865 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/train_with_keras.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6505 2024-04-04 19:51:42.000000 zoobot-2.0.0/zoobot/tensorflow/training/training_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:51:51.002094 zoobot-2.0.0/zoobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 19:51:50.000000 zoobot-2.0.0/zoobot.egg-info/top_level.txt
```

### Comparing `zoobot-1.0.5/LICENSE` & `zoobot-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/PKG-INFO` & `zoobot-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7a6f 6f62  : 2.1.Name: zoob
-00000020: 6f74 0a56 6572 7369 6f6e 3a20 312e 302e  ot.Version: 1.0.
-00000030: 350a 5375 6d6d 6172 793a 2047 616c 6178  5.Summary: Galax
+00000020: 6f74 0a56 6572 7369 6f6e 3a20 322e 302e  ot.Version: 2.0.
+00000030: 300a 5375 6d6d 6172 793a 2047 616c 6178  0.Summary: Galax
 00000040: 7920 6d6f 7270 686f 6c6f 6779 2063 6c61  y morphology cla
 00000050: 7373 6966 6965 7273 0a48 6f6d 652d 7061  ssifiers.Home-pa
 00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000070: 7562 2e63 6f6d 2f6d 7761 6c6d 736c 6579  ub.com/mwalmsley
 00000080: 2f7a 6f6f 626f 740a 4175 7468 6f72 3a20  /zoobot.Author: 
 00000090: 4d69 6b65 2057 616c 6d73 6c65 790a 4175  Mike Walmsley.Au
 000000a0: 7468 6f72 2d65 6d61 696c 3a20 7761 6c6d  thor-email: walm
@@ -23,15 +23,15 @@
 00000160: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
 00000170: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
 00000180: 2053 7461 7475 7320 3a3a 2034 202d 2042   Status :: 4 - B
 00000190: 6574 610a 436c 6173 7369 6669 6572 3a20  eta.Classifier: 
 000001a0: 456e 7669 726f 6e6d 656e 7420 3a3a 2047  Environment :: G
 000001b0: 5055 203a 3a20 4e56 4944 4941 2043 5544  PU :: NVIDIA CUD
 000001c0: 410a 5265 7175 6972 6573 2d50 7974 686f  A.Requires-Pytho
-000001d0: 6e3a 203e 3d33 2e38 0a44 6573 6372 6970  n: >=3.8.Descrip
+000001d0: 6e3a 203e 3d33 2e39 0a44 6573 6372 6970  n: >=3.9.Descrip
 000001e0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
 000001f0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
 00000200: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
 00000210: 4943 454e 5345 0a52 6571 7569 7265 732d  ICENSE.Requires-
 00000220: 4469 7374 3a20 6835 7079 0a52 6571 7569  Dist: h5py.Requi
 00000230: 7265 732d 4469 7374 3a20 7471 646d 0a52  res-Dist: tqdm.R
 00000240: 6571 7569 7265 732d 4469 7374 3a20 7069  equires-Dist: pi
@@ -44,981 +44,981 @@
 000002b0: 6972 6573 2d44 6973 743a 2073 6369 6b69  ires-Dist: sciki
 000002c0: 742d 6c65 6172 6e3e 3d31 2e30 2e32 0a52  t-learn>=1.0.2.R
 000002d0: 6571 7569 7265 732d 4469 7374 3a20 6d61  equires-Dist: ma
 000002e0: 7470 6c6f 746c 6962 0a52 6571 7569 7265  tplotlib.Require
 000002f0: 732d 4469 7374 3a20 7079 6172 726f 770a  s-Dist: pyarrow.
 00000300: 5265 7175 6972 6573 2d44 6973 743a 2077  Requires-Dist: w
 00000310: 616e 6462 0a52 6571 7569 7265 732d 4469  andb.Requires-Di
-00000320: 7374 3a20 7365 7475 7074 6f6f 6c73 0a52  st: setuptools.R
-00000330: 6571 7569 7265 732d 4469 7374 3a20 6761  equires-Dist: ga
-00000340: 6c61 7879 2d64 6174 6173 6574 733e 3d30  laxy-datasets>=0
-00000350: 2e30 2e31 350a 5072 6f76 6964 6573 2d45  .0.15.Provides-E
-00000360: 7874 7261 3a20 7079 746f 7263 682d 6370  xtra: pytorch-cp
-00000370: 750a 5265 7175 6972 6573 2d44 6973 743a  u.Requires-Dist:
-00000380: 2074 6f72 6368 3d3d 312e 3132 2e31 2b63   torch==1.12.1+c
-00000390: 7075 3b20 6578 7472 6120 3d3d 2022 7079  pu; extra == "py
-000003a0: 746f 7263 682d 6370 7522 0a52 6571 7569  torch-cpu".Requi
-000003b0: 7265 732d 4469 7374 3a20 746f 7263 6876  res-Dist: torchv
-000003c0: 6973 696f 6e3d 3d30 2e31 332e 312b 6370  ision==0.13.1+cp
-000003d0: 753b 2065 7874 7261 203d 3d20 2270 7974  u; extra == "pyt
-000003e0: 6f72 6368 2d63 7075 220a 5265 7175 6972  orch-cpu".Requir
-000003f0: 6573 2d44 6973 743a 2074 6f72 6368 6175  es-Dist: torchau
-00000400: 6469 6f3d 3d30 2e31 322e 313b 2065 7874  dio==0.12.1; ext
-00000410: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
-00000420: 7075 220a 5265 7175 6972 6573 2d44 6973  pu".Requires-Dis
-00000430: 743a 2070 7974 6f72 6368 2d6c 6967 6874  t: pytorch-light
-00000440: 6e69 6e67 3e3d 322e 302e 303b 2065 7874  ning>=2.0.0; ext
-00000450: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
-00000460: 7075 220a 5265 7175 6972 6573 2d44 6973  pu".Requires-Dis
-00000470: 743a 2061 6c62 756d 656e 7461 7469 6f6e  t: albumentation
-00000480: 733b 2065 7874 7261 203d 3d20 2270 7974  s; extra == "pyt
-00000490: 6f72 6368 2d63 7075 220a 5265 7175 6972  orch-cpu".Requir
-000004a0: 6573 2d44 6973 743a 2070 7972 6f2d 7070  es-Dist: pyro-pp
-000004b0: 6c3d 3d31 2e38 2e30 3b20 6578 7472 6120  l==1.8.0; extra 
-000004c0: 3d3d 2022 7079 746f 7263 682d 6370 7522  == "pytorch-cpu"
-000004d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004e0: 746f 7263 686d 6574 7269 6373 3d3d 302e  torchmetrics==0.
-000004f0: 3131 2e30 3b20 6578 7472 6120 3d3d 2022  11.0; extra == "
-00000500: 7079 746f 7263 682d 6370 7522 0a52 6571  pytorch-cpu".Req
-00000510: 7569 7265 732d 4469 7374 3a20 7469 6d6d  uires-Dist: timm
-00000520: 3d3d 302e 362e 3132 3b20 6578 7472 6120  ==0.6.12; extra 
-00000530: 3d3d 2022 7079 746f 7263 682d 6370 7522  == "pytorch-cpu"
-00000540: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000550: 2070 7974 6f72 6368 2d6d 310a 5265 7175   pytorch-m1.Requ
-00000560: 6972 6573 2d44 6973 743a 2074 6f72 6368  ires-Dist: torch
-00000570: 3d3d 312e 3132 2e31 3b20 6578 7472 6120  ==1.12.1; extra 
-00000580: 3d3d 2022 7079 746f 7263 682d 6d31 220a  == "pytorch-m1".
-00000590: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-000005a0: 6f72 6368 7669 7369 6f6e 3d3d 302e 3133  orchvision==0.13
-000005b0: 2e31 3b20 6578 7472 6120 3d3d 2022 7079  .1; extra == "py
-000005c0: 746f 7263 682d 6d31 220a 5265 7175 6972  torch-m1".Requir
-000005d0: 6573 2d44 6973 743a 2074 6f72 6368 6175  es-Dist: torchau
-000005e0: 6469 6f3d 3d30 2e31 322e 313b 2065 7874  dio==0.12.1; ext
-000005f0: 7261 203d 3d20 2270 7974 6f72 6368 2d6d  ra == "pytorch-m
-00000600: 3122 0a52 6571 7569 7265 732d 4469 7374  1".Requires-Dist
-00000610: 3a20 7079 746f 7263 682d 6c69 6768 746e  : pytorch-lightn
-00000620: 696e 673e 3d32 2e30 2e30 3b20 6578 7472  ing>=2.0.0; extr
-00000630: 6120 3d3d 2022 7079 746f 7263 682d 6d31  a == "pytorch-m1
-00000640: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000650: 2061 6c62 756d 656e 7461 7469 6f6e 733b   albumentations;
-00000660: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
-00000670: 6368 2d6d 3122 0a52 6571 7569 7265 732d  ch-m1".Requires-
-00000680: 4469 7374 3a20 7079 726f 2d70 706c 3d3d  Dist: pyro-ppl==
-00000690: 312e 382e 303b 2065 7874 7261 203d 3d20  1.8.0; extra == 
-000006a0: 2270 7974 6f72 6368 2d6d 3122 0a52 6571  "pytorch-m1".Req
-000006b0: 7569 7265 732d 4469 7374 3a20 746f 7263  uires-Dist: torc
-000006c0: 686d 6574 7269 6373 3d3d 302e 3131 2e30  hmetrics==0.11.0
-000006d0: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
-000006e0: 7263 682d 6d31 220a 5265 7175 6972 6573  rch-m1".Requires
-000006f0: 2d44 6973 743a 2074 696d 6d3d 3d30 2e36  -Dist: timm==0.6
-00000700: 2e31 323b 2065 7874 7261 203d 3d20 2270  .12; extra == "p
-00000710: 7974 6f72 6368 2d6d 3122 0a50 726f 7669  ytorch-m1".Provi
-00000720: 6465 732d 4578 7472 613a 2070 7974 6f72  des-Extra: pytor
-00000730: 6368 2d63 7531 3133 0a52 6571 7569 7265  ch-cu113.Require
-00000740: 732d 4469 7374 3a20 746f 7263 683d 3d31  s-Dist: torch==1
-00000750: 2e31 322e 312b 6375 3131 333b 2065 7874  .12.1+cu113; ext
-00000760: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
-00000770: 7531 3133 220a 5265 7175 6972 6573 2d44  u113".Requires-D
-00000780: 6973 743a 2074 6f72 6368 7669 7369 6f6e  ist: torchvision
-00000790: 3d3d 302e 3133 2e31 2b63 7531 3133 3b20  ==0.13.1+cu113; 
-000007a0: 6578 7472 6120 3d3d 2022 7079 746f 7263  extra == "pytorc
-000007b0: 682d 6375 3131 3322 0a52 6571 7569 7265  h-cu113".Require
-000007c0: 732d 4469 7374 3a20 746f 7263 6861 7564  s-Dist: torchaud
-000007d0: 696f 3d3d 302e 3132 2e31 3b20 6578 7472  io==0.12.1; extr
-000007e0: 6120 3d3d 2022 7079 746f 7263 682d 6375  a == "pytorch-cu
-000007f0: 3131 3322 0a52 6571 7569 7265 732d 4469  113".Requires-Di
-00000800: 7374 3a20 7079 746f 7263 682d 6c69 6768  st: pytorch-ligh
-00000810: 746e 696e 673e 3d32 2e30 2e30 3b20 6578  tning>=2.0.0; ex
-00000820: 7472 6120 3d3d 2022 7079 746f 7263 682d  tra == "pytorch-
-00000830: 6375 3131 3322 0a52 6571 7569 7265 732d  cu113".Requires-
-00000840: 4469 7374 3a20 616c 6275 6d65 6e74 6174  Dist: albumentat
-00000850: 696f 6e73 3b20 6578 7472 6120 3d3d 2022  ions; extra == "
-00000860: 7079 746f 7263 682d 6375 3131 3322 0a52  pytorch-cu113".R
-00000870: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000880: 726f 2d70 706c 3d3d 312e 382e 303b 2065  ro-ppl==1.8.0; e
-00000890: 7874 7261 203d 3d20 2270 7974 6f72 6368  xtra == "pytorch
-000008a0: 2d63 7531 3133 220a 5265 7175 6972 6573  -cu113".Requires
-000008b0: 2d44 6973 743a 2074 6f72 6368 6d65 7472  -Dist: torchmetr
-000008c0: 6963 733d 3d30 2e31 312e 303b 2065 7874  ics==0.11.0; ext
-000008d0: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
-000008e0: 7531 3133 220a 5265 7175 6972 6573 2d44  u113".Requires-D
-000008f0: 6973 743a 2074 696d 6d3d 3d30 2e36 2e31  ist: timm==0.6.1
-00000900: 323b 2065 7874 7261 203d 3d20 2270 7974  2; extra == "pyt
-00000910: 6f72 6368 2d63 7531 3133 220a 5072 6f76  orch-cu113".Prov
-00000920: 6964 6573 2d45 7874 7261 3a20 7079 746f  ides-Extra: pyto
-00000930: 7263 682d 636f 6c61 620a 5265 7175 6972  rch-colab.Requir
-00000940: 6573 2d44 6973 743a 2070 7974 6f72 6368  es-Dist: pytorch
-00000950: 2d6c 6967 6874 6e69 6e67 3e3d 322e 302e  -lightning>=2.0.
-00000960: 303b 2065 7874 7261 203d 3d20 2270 7974  0; extra == "pyt
-00000970: 6f72 6368 2d63 6f6c 6162 220a 5265 7175  orch-colab".Requ
-00000980: 6972 6573 2d44 6973 743a 2061 6c62 756d  ires-Dist: album
-00000990: 656e 7461 7469 6f6e 733b 2065 7874 7261  entations; extra
-000009a0: 203d 3d20 2270 7974 6f72 6368 2d63 6f6c   == "pytorch-col
-000009b0: 6162 220a 5265 7175 6972 6573 2d44 6973  ab".Requires-Dis
-000009c0: 743a 2070 7972 6f2d 7070 6c3e 3d31 2e38  t: pyro-ppl>=1.8
-000009d0: 2e30 3b20 6578 7472 6120 3d3d 2022 7079  .0; extra == "py
-000009e0: 746f 7263 682d 636f 6c61 6222 0a52 6571  torch-colab".Req
-000009f0: 7569 7265 732d 4469 7374 3a20 746f 7263  uires-Dist: torc
-00000a00: 686d 6574 7269 6373 3d3d 302e 3131 2e30  hmetrics==0.11.0
-00000a10: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
-00000a20: 7263 682d 636f 6c61 6222 0a52 6571 7569  rch-colab".Requi
-00000a30: 7265 732d 4469 7374 3a20 7469 6d6d 3d3d  res-Dist: timm==
-00000a40: 302e 362e 3132 3b20 6578 7472 6120 3d3d  0.6.12; extra ==
-00000a50: 2022 7079 746f 7263 682d 636f 6c61 6222   "pytorch-colab"
-00000a60: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000a70: 2074 656e 736f 7266 6c6f 770a 5265 7175   tensorflow.Requ
-00000a80: 6972 6573 2d44 6973 743a 2074 656e 736f  ires-Dist: tenso
-00000a90: 7266 6c6f 773d 3d32 2e31 302e 303b 2065  rflow==2.10.0; e
-00000aa0: 7874 7261 203d 3d20 2274 656e 736f 7266  xtra == "tensorf
-00000ab0: 6c6f 7722 0a52 6571 7569 7265 732d 4469  low".Requires-Di
-00000ac0: 7374 3a20 6b65 7261 735f 6170 706c 6963  st: keras_applic
-00000ad0: 6174 696f 6e73 3b20 6578 7472 6120 3d3d  ations; extra ==
-00000ae0: 2022 7465 6e73 6f72 666c 6f77 220a 5265   "tensorflow".Re
-00000af0: 7175 6972 6573 2d44 6973 743a 2074 656e  quires-Dist: ten
-00000b00: 736f 7266 6c6f 775f 7072 6f62 6162 696c  sorflow_probabil
-00000b10: 6974 793d 3d30 2e31 382e 303b 2065 7874  ity==0.18.0; ext
-00000b20: 7261 203d 3d20 2274 656e 736f 7266 6c6f  ra == "tensorflo
-00000b30: 7722 0a52 6571 7569 7265 732d 4469 7374  w".Requires-Dist
-00000b40: 3a20 7072 6f74 6f62 7566 3c3d 332e 3139  : protobuf<=3.19
-00000b50: 3b20 6578 7472 6120 3d3d 2022 7465 6e73  ; extra == "tens
-00000b60: 6f72 666c 6f77 220a 5072 6f76 6964 6573  orflow".Provides
-00000b70: 2d45 7874 7261 3a20 7574 696c 6974 6965  -Extra: utilitie
-00000b80: 730a 5265 7175 6972 6573 2d44 6973 743a  s.Requires-Dist:
-00000b90: 2073 6561 626f 726e 3b20 6578 7472 6120   seaborn; extra 
-00000ba0: 3d3d 2022 7574 696c 6974 6965 7322 0a52  == "utilities".R
-00000bb0: 6571 7569 7265 732d 4469 7374 3a20 626f  equires-Dist: bo
-00000bc0: 746f 333b 2065 7874 7261 203d 3d20 2275  to3; extra == "u
-00000bd0: 7469 6c69 7469 6573 220a 5265 7175 6972  tilities".Requir
-00000be0: 6573 2d44 6973 743a 2070 7974 686f 6e2d  es-Dist: python-
-00000bf0: 6461 7465 7574 696c 3d3d 322e 382e 313b  dateutil==2.8.1;
-00000c00: 2065 7874 7261 203d 3d20 2275 7469 6c69   extra == "utili
-00000c10: 7469 6573 220a 5072 6f76 6964 6573 2d45  ties".Provides-E
-00000c20: 7874 7261 3a20 646f 6373 0a52 6571 7569  xtra: docs.Requi
-00000c30: 7265 732d 4469 7374 3a20 5370 6869 6e78  res-Dist: Sphinx
-00000c40: 3b20 6578 7472 6120 3d3d 2022 646f 6373  ; extra == "docs
-00000c50: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000c60: 2073 7068 696e 7863 6f6e 7472 6962 2d6e   sphinxcontrib-n
-00000c70: 6170 6f6c 656f 6e3b 2065 7874 7261 203d  apoleon; extra =
-00000c80: 3d20 2264 6f63 7322 0a52 6571 7569 7265  = "docs".Require
-00000c90: 732d 4469 7374 3a20 6675 726f 3b20 6578  s-Dist: furo; ex
-00000ca0: 7472 6120 3d3d 2022 646f 6373 220a 5265  tra == "docs".Re
-00000cb0: 7175 6972 6573 2d44 6973 743a 2064 6f63  quires-Dist: doc
-00000cc0: 7574 696c 733c 302e 3138 3b20 6578 7472  utils<0.18; extr
-00000cd0: 6120 3d3d 2022 646f 6373 220a 0a23 205a  a == "docs"..# Z
-00000ce0: 6f6f 626f 740a 0a5b 215b 446f 776e 6c6f  oobot..[![Downlo
-00000cf0: 6164 735d 2868 7474 7073 3a2f 2f70 6570  ads](https://pep
-00000d00: 792e 7465 6368 2f62 6164 6765 2f7a 6f6f  y.tech/badge/zoo
-00000d10: 626f 7429 5d28 6874 7470 733a 2f2f 7065  bot)](https://pe
-00000d20: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
-00000d30: 7a6f 6f62 6f74 290a 5b21 5b44 6f63 756d  zoobot).[![Docum
-00000d40: 656e 7461 7469 6f6e 2053 7461 7475 735d  entation Status]
-00000d50: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
-00000d60: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
-00000d70: 732f 7a6f 6f62 6f74 2f62 6164 6765 2f3f  s/zoobot/badge/?
-00000d80: 7665 7273 696f 6e3d 6c61 7465 7374 295d  version=latest)]
-00000d90: 2868 7474 7073 3a2f 2f7a 6f6f 626f 742e  (https://zoobot.
-00000da0: 7265 6164 7468 6564 6f63 732e 696f 2f29  readthedocs.io/)
-00000db0: 0a21 5b62 7569 6c64 5d28 6874 7470 733a  .![build](https:
-00000dc0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 7761  //github.com/mwa
-00000dd0: 6c6d 736c 6579 2f7a 6f6f 626f 742f 6163  lmsley/zoobot/ac
-00000de0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000df0: 7275 6e5f 4349 2e79 6d6c 2f62 6164 6765  run_CI.yml/badge
-00000e00: 2e73 7667 290a 215b 7075 626c 6973 685d  .svg).![publish]
-00000e10: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000e20: 636f 6d2f 6d77 616c 6d73 6c65 792f 7a6f  com/mwalmsley/zo
-00000e30: 6f62 6f74 2f61 6374 696f 6e73 2f77 6f72  obot/actions/wor
-00000e40: 6b66 6c6f 7773 2f70 7974 686f 6e2d 7075  kflows/python-pu
-00000e50: 626c 6973 682e 796d 6c2f 6261 6467 652e  blish.yml/badge.
-00000e60: 7376 6729 0a5b 215b 5079 5049 5d28 6874  svg).[![PyPI](ht
-00000e70: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-00000e80: 2e69 6f2f 7079 2f7a 6f6f 626f 742e 7376  .io/py/zoobot.sv
-00000e90: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
-00000ea0: 652e 6675 7279 2e69 6f2f 7079 2f7a 6f6f  e.fury.io/py/zoo
-00000eb0: 626f 7429 0a5b 215b 444f 495d 2868 7474  bot).[![DOI](htt
-00000ec0: 7073 3a2f 2f7a 656e 6f64 6f2e 6f72 672f  ps://zenodo.org/
-00000ed0: 6261 6467 652f 3334 3337 3837 3631 372e  badge/343787617.
-00000ee0: 7376 6729 5d28 6874 7470 733a 2f2f 7a65  svg)](https://ze
-00000ef0: 6e6f 646f 2e6f 7267 2f62 6164 6765 2f6c  nodo.org/badge/l
-00000f00: 6174 6573 7464 6f69 2f33 3433 3738 3736  atestdoi/3437876
-00000f10: 3137 290a 5b21 5b73 7461 7475 735d 2868  17).[![status](h
-00000f20: 7474 7073 3a2f 2f6a 6f73 732e 7468 656f  ttps://joss.theo
-00000f30: 6a2e 6f72 672f 7061 7065 7273 2f34 3437  j.org/papers/447
-00000f40: 3536 3165 6532 6465 3437 3039 6564 6462  561ee2de4709eddb
-00000f50: 3730 3465 3138 6265 6538 3436 662f 7374  704e18bee846f/st
-00000f60: 6174 7573 2e73 7667 295d 2868 7474 7073  atus.svg)](https
-00000f70: 3a2f 2f6a 6f73 732e 7468 656f 6a2e 6f72  ://joss.theoj.or
-00000f80: 672f 7061 7065 7273 2f34 3437 3536 3165  g/papers/447561e
-00000f90: 6532 6465 3437 3039 6564 6462 3730 3465  e2de4709eddb704e
-00000fa0: 3138 6265 6538 3436 6629 0a3c 6120 6872  18bee846f).<a hr
-00000fb0: 6566 3d22 6874 7470 733a 2f2f 6173 636c  ef="https://ascl
-00000fc0: 2e6e 6574 2f32 3230 332e 3032 3722 3e3c  .net/2203.027"><
-00000fd0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000fe0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000ff0: 6261 6467 652f 6173 636c 2d32 3230 332e  badge/ascl-2203.
-00001000: 3032 372d 626c 7565 2e73 7667 3f63 6f6c  027-blue.svg?col
-00001010: 6f72 423d 3236 3232 3535 2220 616c 743d  orB=262255" alt=
-00001020: 2261 7363 6c3a 3232 3033 2e30 3237 2220  "ascl:2203.027" 
-00001030: 2f3e 3c2f 613e 0a0a 5a6f 6f62 6f74 2063  /></a>..Zoobot c
-00001040: 6c61 7373 6966 6965 7320 6761 6c61 7879  lassifies galaxy
-00001050: 206d 6f72 7068 6f6c 6f67 7920 7769 7468   morphology with
-00001060: 2064 6565 7020 6c65 6172 6e69 6e67 2e0a   deep learning..
-00001070: 3c21 2d2d 2041 7420 4761 6c61 7879 205a  <!-- At Galaxy Z
-00001080: 6f6f 2c20 7765 2075 7365 205a 6f6f 626f  oo, we use Zoobo
-00001090: 7420 746f 2068 656c 7020 6f75 7220 766f  t to help our vo
-000010a0: 6c75 6e74 6565 7273 2063 6c61 7373 6966  lunteers classif
-000010b0: 7920 7468 6520 6761 6c61 7869 6573 2069  y the galaxies i
-000010c0: 6e20 616c 6c20 6f75 7220 7265 6365 6e74  n all our recent
-000010d0: 2063 6174 616c 6f67 7565 733a 2047 5a20   catalogues: GZ 
-000010e0: 4445 4361 4c53 2c20 475a 2044 4553 492c  DECaLS, GZ DESI,
-000010f0: 2047 5a20 5269 6e67 7320 616e 6420 475a   GZ Rings and GZ
-00001100: 2043 6f73 6d69 6320 4461 776e 2e20 2d2d   Cosmic Dawn. --
-00001110: 3e0a 0a5a 6f6f 626f 7420 6973 2074 7261  >..Zoobot is tra
-00001120: 696e 6564 2075 7369 6e67 206d 696c 6c69  ined using milli
-00001130: 6f6e 7320 6f66 2061 6e73 7765 7273 2062  ons of answers b
-00001140: 7920 4761 6c61 7879 205a 6f6f 2076 6f6c  y Galaxy Zoo vol
-00001150: 756e 7465 6572 732e 2054 6869 7320 636f  unteers. This co
-00001160: 6465 2077 696c 6c20 6c65 7420 796f 7520  de will let you 
-00001170: 2a2a 7265 7472 6169 6e2a 2a20 5a6f 6f62  **retrain** Zoob
-00001180: 6f74 2074 6f20 6163 6375 7261 7465 6c79  ot to accurately
-00001190: 2073 6f6c 7665 2079 6f75 7220 6f77 6e20   solve your own 
-000011a0: 7072 6564 6963 7469 6f6e 2074 6173 6b2e  prediction task.
-000011b0: 0a0a 2d20 5b49 6e73 7461 6c6c 5d28 2369  ..- [Install](#i
-000011c0: 6e73 7461 6c6c 6174 696f 6e29 0a2d 205b  nstallation).- [
-000011d0: 5175 6963 6b73 7461 7274 5d28 2371 7569  Quickstart](#qui
-000011e0: 636b 7374 6172 7429 0a2d 205b 576f 726b  ckstart).- [Work
-000011f0: 6564 2045 7861 6d70 6c65 735d 2823 776f  ed Examples](#wo
-00001200: 726b 6564 2d65 7861 6d70 6c65 7329 0a2d  rked-examples).-
-00001210: 205b 5072 6574 7261 696e 6564 2057 6569   [Pretrained Wei
-00001220: 6768 7473 5d28 6874 7470 733a 2f2f 7a6f  ghts](https://zo
-00001230: 6f62 6f74 2e72 6561 6474 6865 646f 6373  obot.readthedocs
-00001240: 2e69 6f2f 656e 2f6c 6174 6573 742f 6461  .io/en/latest/da
-00001250: 7461 5f6e 6f74 6573 2e68 746d 6c29 0a2d  ta_notes.html).-
-00001260: 205b 4461 7461 7365 7473 5d28 6874 7470   [Datasets](http
-00001270: 733a 2f2f 7777 772e 6769 7468 7562 2e63  s://www.github.c
-00001280: 6f6d 2f6d 7761 6c6d 736c 6579 2f67 616c  om/mwalmsley/gal
-00001290: 6178 792d 6461 7461 7365 7473 290a 2d20  axy-datasets).- 
-000012a0: 5b44 6f63 756d 656e 7461 7469 6f6e 5d28  [Documentation](
-000012b0: 6874 7470 733a 2f2f 7a6f 6f62 6f74 2e72  https://zoobot.r
-000012c0: 6561 6474 6865 646f 6373 2e69 6f2f 2920  eadthedocs.io/) 
-000012d0: 2866 6f72 2075 6e64 6572 7374 616e 6469  (for understandi
-000012e0: 6e67 2f72 6566 6572 656e 6365 290a 0a23  ng/reference)..#
-000012f0: 2320 496e 7374 616c 6c61 7469 6f6e 0a3c  # Installation.<
-00001300: 6120 6e61 6d65 3d22 696e 7374 616c 6c61  a name="installa
-00001310: 7469 6f6e 223e 3c2f 613e 0a0a 596f 7520  tion"></a>..You 
-00001320: 6361 6e20 7265 7472 6169 6e20 5a6f 6f62  can retrain Zoob
-00001330: 6f74 2069 6e20 7468 6520 636c 6f75 6420  ot in the cloud 
-00001340: 7769 7468 2061 2066 7265 6520 4750 5520  with a free GPU 
-00001350: 7573 696e 6720 7468 6973 205b 476f 6f67  using this [Goog
-00001360: 6c65 2043 6f6c 6162 206e 6f74 6562 6f6f  le Colab noteboo
-00001370: 6b5d 2868 7474 7073 3a2f 2f63 6f6c 6162  k](https://colab
-00001380: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00001390: 2e63 6f6d 2f64 7269 7665 2f31 3762 625f  .com/drive/17bb_
-000013a0: 4b62 4132 4a36 7972 496d 3470 3455 655f  KbA2J6yrIm4p4Ue_
-000013b0: 6c45 4248 4d4e 4331 4939 4a64 3f75 7370  lEBHMNC1I9Jd?usp
-000013c0: 3d73 6861 7269 6e67 292e 2054 6f20 696e  =sharing). To in
-000013d0: 7374 616c 6c20 6c6f 6361 6c6c 792c 206b  stall locally, k
-000013e0: 6565 7020 7265 6164 696e 672e 0a0a 446f  eep reading...Do
-000013f0: 776e 6c6f 6164 2074 6865 2063 6f64 6520  wnload the code 
-00001400: 7573 696e 6720 6769 743a 0a0a 2020 2020  using git:..    
-00001410: 6769 7420 636c 6f6e 6520 6769 7440 6769  git clone git@gi
-00001420: 7468 7562 2e63 6f6d 3a6d 7761 6c6d 736c  thub.com:mwalmsl
-00001430: 6579 2f7a 6f6f 626f 742e 6769 740a 0a41  ey/zoobot.git..A
-00001440: 6e64 2074 6865 6e20 7069 636b 206f 6e65  nd then pick one
-00001450: 206f 6620 7468 6520 7468 7265 6520 636f   of the three co
-00001460: 6d6d 616e 6473 2062 656c 6f77 2074 6f20  mmands below to 
-00001470: 696e 7374 616c 6c20 5a6f 6f62 6f74 2061  install Zoobot a
-00001480: 6e64 2065 6974 6865 7220 5079 546f 7263  nd either PyTorc
-00001490: 6820 2872 6563 6f6d 6d65 6e64 6564 2920  h (recommended) 
-000014a0: 6f72 2054 656e 736f 7246 6c6f 773a 0a0a  or TensorFlow:..
-000014b0: 2020 2020 2320 5a6f 6f62 6f74 2077 6974      # Zoobot wit
-000014c0: 6820 5079 546f 7263 6820 616e 6420 6120  h PyTorch and a 
-000014d0: 4750 552e 2052 6571 7569 7265 7320 4355  GPU. Requires CU
-000014e0: 4441 2031 312e 332e 0a20 2020 2070 6970  DA 11.3..    pip
-000014f0: 2069 6e73 7461 6c6c 202d 6520 227a 6f6f   install -e "zoo
-00001500: 626f 745b 7079 746f 7263 685f 6375 3131  bot[pytorch_cu11
-00001510: 335d 2220 2d2d 6578 7472 612d 696e 6465  3]" --extra-inde
-00001520: 782d 7572 6c20 6874 7470 733a 2f2f 646f  x-url https://do
-00001530: 776e 6c6f 6164 2e70 7974 6f72 6368 2e6f  wnload.pytorch.o
-00001540: 7267 2f77 686c 2f63 7531 3133 0a0a 2020  rg/whl/cu113..  
-00001550: 2020 2320 4f52 205a 6f6f 626f 7420 7769    # OR Zoobot wi
-00001560: 7468 2050 7954 6f72 6368 2061 6e64 206e  th PyTorch and n
-00001570: 6f20 4750 550a 2020 2020 7069 7020 696e  o GPU.    pip in
-00001580: 7374 616c 6c20 2d65 2022 7a6f 6f62 6f74  stall -e "zoobot
-00001590: 5b70 7974 6f72 6368 5f63 7075 5d22 202d  [pytorch_cpu]" -
-000015a0: 2d65 7874 7261 2d69 6e64 6578 2d75 726c  -extra-index-url
-000015b0: 2068 7474 7073 3a2f 2f64 6f77 6e6c 6f61   https://downloa
-000015c0: 642e 7079 746f 7263 682e 6f72 672f 7768  d.pytorch.org/wh
-000015d0: 6c2f 6370 750a 0a20 2020 2023 204f 5220  l/cpu..    # OR 
-000015e0: 5a6f 6f62 6f74 2077 6974 6820 5079 546f  Zoobot with PyTo
-000015f0: 7263 6820 6f6e 204d 6163 2077 6974 6820  rch on Mac with 
-00001600: 4d31 2063 6869 700a 2020 2020 7069 7020  M1 chip.    pip 
-00001610: 696e 7374 616c 6c20 2d65 2022 7a6f 6f62  install -e "zoob
-00001620: 6f74 5b70 7974 6f72 6368 5f6d 315d 220a  ot[pytorch_m1]".
-00001630: 0a20 2020 2023 204f 5220 5a6f 6f62 6f74  .    # OR Zoobot
-00001640: 2077 6974 6820 5465 6e73 6f72 466c 6f77   with TensorFlow
-00001650: 2e20 576f 726b 7320 7769 7468 2061 6e64  . Works with and
-00001660: 2077 6974 686f 7574 2061 2047 5055 2c20   without a GPU, 
-00001670: 6275 7420 6966 2079 6f75 2068 6176 6520  but if you have 
-00001680: 6120 4750 552c 2079 6f75 206e 6565 6420  a GPU, you need 
-00001690: 4355 4441 2031 312e 322e 200a 2020 2020  CUDA 11.2. .    
-000016a0: 7069 7020 696e 7374 616c 6c20 2d65 2022  pip install -e "
-000016b0: 7a6f 6f62 6f74 5b74 656e 736f 7266 6c6f  zoobot[tensorflo
-000016c0: 775d 0a0a 5468 6973 2069 6e73 7461 6c6c  w]..This install
-000016d0: 7320 7468 6520 646f 776e 6c6f 6164 6564  s the downloaded
-000016e0: 205a 6f6f 626f 7420 636f 6465 2075 7369   Zoobot code usi
-000016f0: 6e67 2070 6970 205b 6564 6974 6162 6c65  ng pip [editable
-00001700: 206d 6f64 655d 2868 7474 7073 3a2f 2f70   mode](https://p
-00001710: 6970 2e70 7970 612e 696f 2f65 6e2f 7374  ip.pypa.io/en/st
-00001720: 6162 6c65 2f74 6f70 6963 732f 6c6f 6361  able/topics/loca
-00001730: 6c2d 7072 6f6a 6563 742d 696e 7374 616c  l-project-instal
-00001740: 6c73 2f23 6564 6974 6162 6c65 2d69 6e73  ls/#editable-ins
-00001750: 7461 6c6c 7329 2073 6f20 796f 7520 6361  talls) so you ca
-00001760: 6e20 6561 7369 6c79 2063 6861 6e67 6520  n easily change 
-00001770: 7468 6520 636f 6465 206c 6f63 616c 6c79  the code locally
-00001780: 2e20 5a6f 6f62 6f74 2069 7320 616c 736f  . Zoobot is also
-00001790: 2061 7661 696c 6162 6c65 2064 6972 6563   available direc
-000017a0: 746c 7920 6672 6f6d 2070 6970 2028 6070  tly from pip (`p
-000017b0: 6970 2069 6e73 7461 6c6c 207a 6f6f 626f  ip install zoobo
-000017c0: 745b 6f70 7469 6f6e 5d60 292e 204f 6e6c  t[option]`). Onl
-000017d0: 7920 7573 6520 7468 6973 2069 6620 796f  y use this if yo
-000017e0: 7520 6172 6520 7375 7265 2079 6f75 2077  u are sure you w
-000017f0: 6f6e 2774 2062 6520 6d61 6b69 6e67 2063  on't be making c
-00001800: 6861 6e67 6573 2074 6f20 5a6f 6f62 6f74  hanges to Zoobot
-00001810: 2069 7473 656c 662e 2046 6f72 2047 6f6f   itself. For Goo
-00001820: 676c 6520 436f 6c61 622c 2075 7365 2060  gle Colab, use `
-00001830: 7069 7020 696e 7374 616c 6c20 7a6f 6f62  pip install zoob
-00001840: 6f74 5b70 7974 6f72 6368 5f63 6f6c 6162  ot[pytorch_colab
-00001850: 5d60 0a0a 546f 2075 7365 2061 2047 5055  ]`..To use a GPU
-00001860: 2c20 796f 7520 6d75 7374 202a 616c 7265  , you must *alre
-00001870: 6164 792a 2068 6176 6520 4355 4441 2069  ady* have CUDA i
-00001880: 6e73 7461 6c6c 6564 2061 6e64 206d 6174  nstalled and mat
-00001890: 6368 696e 6720 7468 6520 7665 7273 696f  ching the versio
-000018a0: 6e73 2061 626f 7665 2e0a 4920 7368 6172  ns above..I shar
-000018b0: 6520 6d79 2069 6e73 7461 6c6c 2073 7465  e my install ste
-000018c0: 7073 205b 6865 7265 5d28 2369 6e73 7461  ps [here](#insta
-000018d0: 6c6c 5f63 7564 6129 2e20 4750 5573 2061  ll_cuda). GPUs a
-000018e0: 7265 206f 7074 696f 6e61 6c20 2d20 5a6f  re optional - Zo
-000018f0: 6f62 6f74 2077 696c 6c20 7275 6e20 7265  obot will run re
-00001900: 7472 6169 6e20 6669 6e65 206f 6e20 4350  train fine on CP
-00001910: 552c 206a 7573 7420 736c 6f77 6572 2e0a  U, just slower..
-00001920: 0a23 2320 5175 6963 6b73 7461 7274 0a3c  .## Quickstart.<
-00001930: 6120 6e61 6d65 3d22 7175 6963 6b73 7461  a name="quicksta
-00001940: 7274 223e 3c2f 613e 0a0a 5468 6520 5b43  rt"></a>..The [C
-00001950: 6f6c 6162 206e 6f74 6562 6f6f 6b5d 2868  olab notebook](h
-00001960: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00001970: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00001980: 2f64 7269 7665 2f31 3762 625f 4b62 4132  /drive/17bb_KbA2
-00001990: 4a36 7972 496d 3470 3455 655f 6c45 4248  J6yrIm4p4Ue_lEBH
-000019a0: 4d4e 4331 4939 4a64 3f75 7370 3d73 6861  MNC1I9Jd?usp=sha
-000019b0: 7269 6e67 2920 6973 2074 6865 2071 7569  ring) is the qui
-000019c0: 636b 6573 7420 7761 7920 746f 2067 6574  ckest way to get
-000019d0: 2073 7461 7274 6564 2e20 416c 7465 726e   started. Altern
-000019e0: 6174 6976 656c 792c 2074 6865 206d 696e  atively, the min
-000019f0: 696d 616c 2065 7861 6d70 6c65 2062 656c  imal example bel
-00001a00: 6f77 2069 6c6c 7573 7472 6174 6573 2068  ow illustrates h
-00001a10: 6f77 205a 6f6f 626f 7420 776f 726b 732e  ow Zoobot works.
-00001a20: 0a0a 4c65 7427 7320 7361 7920 796f 7520  ..Let's say you 
-00001a30: 7761 6e74 2074 6f20 6669 6e64 2072 696e  want to find rin
-00001a40: 6765 6420 6761 6c61 7869 6573 2061 6e64  ged galaxies and
-00001a50: 2079 6f75 2068 6176 6520 6120 736d 616c   you have a smal
-00001a60: 6c20 6c61 6265 6c6c 6564 2064 6174 6173  l labelled datas
-00001a70: 6574 206f 6620 3530 3020 7269 6e67 6564  et of 500 ringed
-00001a80: 206f 7220 6e6f 742d 7269 6e67 6564 2067   or not-ringed g
-00001a90: 616c 6178 6965 732e 2059 6f75 2063 616e  alaxies. You can
-00001aa0: 2072 6574 7261 696e 205a 6f6f 626f 7420   retrain Zoobot 
-00001ab0: 746f 2066 696e 6420 7269 6e67 7320 6c69  to find rings li
-00001ac0: 6b65 2073 6f3a 0a0a 6060 6070 7974 686f  ke so:..```pytho
-00001ad0: 6e0a 0a20 2020 2069 6d70 6f72 7420 7061  n..    import pa
-00001ae0: 6e64 6173 2061 7320 7064 0a20 2020 2066  ndas as pd.    f
-00001af0: 726f 6d20 6761 6c61 7879 5f64 6174 6173  rom galaxy_datas
-00001b00: 6574 732e 7079 746f 7263 682e 6761 6c61  ets.pytorch.gala
-00001b10: 7879 5f64 6174 616d 6f64 756c 6520 696d  xy_datamodule im
-00001b20: 706f 7274 2047 616c 6178 7944 6174 614d  port GalaxyDataM
-00001b30: 6f64 756c 650a 2020 2020 6672 6f6d 207a  odule.    from z
-00001b40: 6f6f 626f 742e 7079 746f 7263 682e 7472  oobot.pytorch.tr
-00001b50: 6169 6e69 6e67 2069 6d70 6f72 7420 6669  aining import fi
-00001b60: 6e65 7475 6e65 0a0a 2020 2020 2320 6373  netune..    # cs
-00001b70: 7620 7769 7468 2027 7269 6e67 2720 636f  v with 'ring' co
-00001b80: 6c75 6d6e 2028 3020 6f72 2031 2920 616e  lumn (0 or 1) an
-00001b90: 6420 2766 696c 655f 6c6f 6327 2063 6f6c  d 'file_loc' col
-00001ba0: 756d 6e20 2870 6174 6820 746f 2069 6d61  umn (path to ima
-00001bb0: 6765 290a 2020 2020 6c61 6265 6c6c 6564  ge).    labelled
-00001bc0: 5f64 6620 3d20 7064 2e72 6561 645f 6373  _df = pd.read_cs
-00001bd0: 7628 272f 796f 7572 2f70 6174 682f 736f  v('/your/path/so
-00001be0: 6d65 5f6c 6162 656c 6c65 645f 6761 6c61  me_labelled_gala
-00001bf0: 7869 6573 2e63 7376 2729 0a0a 2020 2020  xies.csv')..    
-00001c00: 6461 7461 6d6f 6475 6c65 203d 2047 616c  datamodule = Gal
-00001c10: 6178 7944 6174 614d 6f64 756c 6528 0a20  axyDataModule(. 
-00001c20: 2020 2020 206c 6162 656c 5f63 6f6c 733d       label_cols=
-00001c30: 5b27 7269 6e67 275d 2c0a 2020 2020 2020  ['ring'],.      
-00001c40: 6361 7461 6c6f 673d 6c61 6265 6c6c 6564  catalog=labelled
-00001c50: 5f64 662c 0a20 2020 2020 2062 6174 6368  _df,.      batch
-00001c60: 5f73 697a 653d 3332 0a20 2020 2029 0a0a  _size=32.    )..
-00001c70: 2020 2020 2320 6c6f 6164 2074 7261 696e      # load train
-00001c80: 6564 205a 6f6f 626f 7420 6d6f 6465 6c0a  ed Zoobot model.
-00001c90: 2020 2020 6d6f 6465 6c20 3d20 6669 6e65      model = fine
-00001ca0: 7475 6e65 2e46 696e 6574 756e 6561 626c  tune.Finetuneabl
-00001cb0: 655a 6f6f 626f 7443 6c61 7373 6966 6965  eZoobotClassifie
-00001cc0: 7228 6368 6563 6b70 6f69 6e74 5f6c 6f63  r(checkpoint_loc
-00001cd0: 2c20 6e75 6d5f 636c 6173 7365 733d 3229  , num_classes=2)
-00001ce0: 2020 0a20 2020 200a 2020 2020 2320 7265    .    .    # re
-00001cf0: 7472 6169 6e20 746f 2066 696e 6420 7269  train to find ri
-00001d00: 6e67 730a 2020 2020 7472 6169 6e65 7220  ngs.    trainer 
-00001d10: 3d20 6669 6e65 7475 6e65 2e67 6574 5f74  = finetune.get_t
-00001d20: 7261 696e 6572 2873 6176 655f 6469 7229  rainer(save_dir)
-00001d30: 0a20 2020 2074 7261 696e 6572 2e66 6974  .    trainer.fit
-00001d40: 286d 6f64 656c 2c20 6461 7461 6d6f 6475  (model, datamodu
-00001d50: 6c65 290a 6060 600a 0a54 6865 6e20 796f  le).```..Then yo
-00001d60: 7520 6361 6e20 6d61 6b65 2070 7265 6469  u can make predi
-00001d70: 6374 2069 6620 6e65 7720 6761 6c61 7869  ct if new galaxi
-00001d80: 6573 2068 6176 6520 7269 6e67 733a 0a0a  es have rings:..
-00001d90: 6060 6070 7974 686f 6e0a 2020 2020 6672  ```python.    fr
-00001da0: 6f6d 207a 6f6f 626f 742e 7079 746f 7263  om zoobot.pytorc
-00001db0: 682e 7072 6564 6963 7469 6f6e 7320 696d  h.predictions im
-00001dc0: 706f 7274 2070 7265 6469 6374 5f6f 6e5f  port predict_on_
-00001dd0: 6361 7461 6c6f 670a 0a20 2020 2023 2063  catalog..    # c
-00001de0: 7376 2077 6974 6820 2766 696c 655f 6c6f  sv with 'file_lo
-00001df0: 6327 2063 6f6c 756d 6e20 2870 6174 6820  c' column (path 
-00001e00: 746f 2069 6d61 6765 292e 205a 6f6f 626f  to image). Zoobo
-00001e10: 7420 7769 6c6c 2070 7265 6469 6374 2074  t will predict t
-00001e20: 6865 206c 6162 656c 732e 0a20 2020 2075  he labels..    u
-00001e30: 6e6c 6162 656c 6c65 645f 6466 203d 2070  nlabelled_df = p
-00001e40: 642e 7265 6164 5f63 7376 2827 2f79 6f75  d.read_csv('/you
-00001e50: 722f 7061 7468 2f73 6f6d 655f 756e 6c61  r/path/some_unla
-00001e60: 6265 6c6c 6564 5f67 616c 6178 6965 732e  belled_galaxies.
-00001e70: 6373 7627 290a 0a20 2020 2070 7265 6469  csv')..    predi
-00001e80: 6374 5f6f 6e5f 6361 7461 6c6f 672e 7072  ct_on_catalog.pr
-00001e90: 6564 6963 7428 0a20 2020 2020 2075 6e6c  edict(.      unl
-00001ea0: 6162 656c 6c65 645f 6466 2c0a 2020 2020  abelled_df,.    
-00001eb0: 2020 6d6f 6465 6c2c 0a20 2020 2020 206c    model,.      l
-00001ec0: 6162 656c 5f63 6f6c 733d 5b27 7269 6e67  abel_cols=['ring
-00001ed0: 275d 2c20 2023 206f 6e6c 7920 7573 6564  '],  # only used
-00001ee0: 2066 6f72 200a 2020 2020 2020 7361 7665   for .      save
-00001ef0: 5f6c 6f63 3d27 2f79 6f75 722f 7061 7468  _loc='/your/path
-00001f00: 2f66 696e 6574 756e 6564 5f70 7265 6469  /finetuned_predi
-00001f10: 6374 696f 6e73 2e63 7376 270a 2020 2020  ctions.csv'.    
-00001f20: 290a 6060 600a 0a5a 6f6f 626f 7420 696e  ).```..Zoobot in
-00001f30: 636c 7564 6573 206d 616e 7920 6775 6964  cludes many guid
-00001f40: 6573 2061 6e64 2077 6f72 6b69 6e67 2065  es and working e
-00001f50: 7861 6d70 6c65 7320 2d20 7365 6520 7468  xamples - see th
-00001f60: 6520 5b47 6574 7469 6e67 2053 7461 7274  e [Getting Start
-00001f70: 6564 5d28 2367 6574 7469 6e67 2d73 7461  ed](#getting-sta
-00001f80: 7274 6564 2920 7365 6374 696f 6e20 6265  rted) section be
-00001f90: 6c6f 772e 0a0a 2323 2047 6574 7469 6e67  low...## Getting
-00001fa0: 2053 7461 7274 6564 0a3c 6120 6e61 6d65   Started.<a name
-00001fb0: 3d22 6765 7474 696e 675f 7374 6172 7465  ="getting_starte
-00001fc0: 6422 3e3c 2f61 3e0a 0a49 2073 7567 6765  d"></a>..I sugge
-00001fd0: 7374 2073 7461 7274 696e 6720 7769 7468  st starting with
-00001fe0: 2074 6865 205b 436f 6c61 6220 6e6f 7465   the [Colab note
-00001ff0: 626f 6f6b 5d28 6874 7470 733a 2f2f 636f  book](https://co
-00002000: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00002010: 676c 652e 636f 6d2f 6472 6976 652f 3137  gle.com/drive/17
-00002020: 6262 5f4b 6241 324a 3679 7249 6d34 7034  bb_KbA2J6yrIm4p4
-00002030: 5565 5f6c 4542 484d 4e43 3149 394a 643f  Ue_lEBHMNC1I9Jd?
-00002040: 7573 703d 7368 6172 696e 6729 206f 7220  usp=sharing) or 
-00002050: 7468 6520 776f 726b 6564 2065 7861 6d70  the worked examp
-00002060: 6c65 7320 6265 6c6f 772c 2077 6869 6368  les below, which
-00002070: 2079 6f75 2063 616e 2063 6f70 7920 616e   you can copy an
-00002080: 6420 6164 6170 742e 0a0a 466f 7220 636f  d adapt...For co
-00002090: 6e74 6578 7420 616e 6420 6578 706c 616e  ntext and explan
-000020a0: 6174 696f 6e2c 2073 6565 2074 6865 205b  ation, see the [
-000020b0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-000020c0: 7474 7073 3a2f 2f7a 6f6f 626f 742e 7265  ttps://zoobot.re
-000020d0: 6164 7468 6564 6f63 732e 696f 2f29 2e0a  adthedocs.io/)..
-000020e0: 0a46 6f72 2070 7265 7472 6169 6e65 6420  .For pretrained 
-000020f0: 6d6f 6465 6c20 7765 6967 6874 732c 2070  model weights, p
-00002100: 7265 6361 6c63 756c 6174 6564 2072 6570  recalculated rep
-00002110: 7265 7365 6e74 6174 696f 6e73 2c20 6361  resentations, ca
-00002120: 7461 6c6f 6775 6573 2c20 616e 6420 736f  talogues, and so
-00002130: 2066 6f72 7468 2c20 7365 6520 7468 6520   forth, see the 
-00002140: 5b64 6174 6120 6e6f 7465 735d 2868 7474  [data notes](htt
-00002150: 7073 3a2f 2f7a 6f6f 626f 742e 7265 6164  ps://zoobot.read
-00002160: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00002170: 7465 7374 2f64 6174 615f 6e6f 7465 732e  test/data_notes.
-00002180: 6874 6d6c 2920 696e 2070 6172 7469 6375  html) in particu
-00002190: 6c61 722e 0a0a 2323 2320 576f 726b 6564  lar...### Worked
-000021a0: 2045 7861 6d70 6c65 730a 3c61 206e 616d   Examples.<a nam
-000021b0: 653d 2277 6f72 6b65 645f 6578 616d 706c  e="worked_exampl
-000021c0: 6573 223e 3c2f 613e 0a0a 5079 546f 7263  es"></a>..PyTorc
-000021d0: 6820 2872 6563 6f6d 6d65 6e64 6564 293a  h (recommended):
-000021e0: 0a2d 205b 7079 746f 7263 682f 6578 616d  .- [pytorch/exam
-000021f0: 706c 6573 2f66 696e 6574 756e 696e 672f  ples/finetuning/
-00002200: 6669 6e65 7475 6e65 5f62 696e 6172 795f  finetune_binary_
-00002210: 636c 6173 7369 6669 6361 7469 6f6e 2e70  classification.p
-00002220: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00002230: 622e 636f 6d2f 6d77 616c 6d73 6c65 792f  b.com/mwalmsley/
-00002240: 7a6f 6f62 6f74 2f62 6c6f 622f 6d61 696e  zoobot/blob/main
-00002250: 2f7a 6f6f 626f 742f 7079 746f 7263 682f  /zoobot/pytorch/
-00002260: 6578 616d 706c 6573 2f66 696e 6574 756e  examples/finetun
-00002270: 696e 672f 6669 6e65 7475 6e65 5f62 696e  ing/finetune_bin
-00002280: 6172 795f 636c 6173 7369 6669 6361 7469  ary_classificati
-00002290: 6f6e 2e70 7929 0a2d 205b 7079 746f 7263  on.py).- [pytorc
-000022a0: 682f 6578 616d 706c 6573 2f66 696e 6574  h/examples/finet
-000022b0: 756e 696e 672f 6669 6e65 7475 6e65 5f63  uning/finetune_c
-000022c0: 6f75 6e74 735f 6675 6c6c 5f74 7265 652e  ounts_full_tree.
-000022d0: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-000022e0: 7562 2e63 6f6d 2f6d 7761 6c6d 736c 6579  ub.com/mwalmsley
-000022f0: 2f7a 6f6f 626f 742f 626c 6f62 2f6d 6169  /zoobot/blob/mai
-00002300: 6e2f 7a6f 6f62 6f74 2f70 7974 6f72 6368  n/zoobot/pytorch
-00002310: 2f65 7861 6d70 6c65 732f 6669 6e65 7475  /examples/finetu
-00002320: 6e69 6e67 2f66 696e 6574 756e 655f 636f  ning/finetune_co
-00002330: 756e 7473 5f66 756c 6c5f 7472 6565 2e70  unts_full_tree.p
-00002340: 7929 0a2d 205b 7079 746f 7263 682f 6578  y).- [pytorch/ex
-00002350: 616d 706c 6573 2f72 6570 7265 7365 6e74  amples/represent
-00002360: 6174 696f 6e73 2f67 6574 5f72 6570 7265  ations/get_repre
-00002370: 7365 6e74 6174 696f 6e73 2e70 795d 2868  sentations.py](h
-00002380: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002390: 6d2f 6d77 616c 6d73 6c65 792f 7a6f 6f62  m/mwalmsley/zoob
-000023a0: 6f74 2f62 6c6f 622f 6d61 696e 2f7a 6f6f  ot/blob/main/zoo
-000023b0: 626f 742f 7079 746f 7263 682f 6578 616d  bot/pytorch/exam
-000023c0: 706c 6573 2f72 6570 7265 7365 6e74 6174  ples/representat
-000023d0: 696f 6e73 2f67 6574 5f72 6570 7265 7365  ions/get_represe
-000023e0: 6e74 6174 696f 6e73 2e70 7929 0a2d 205b  ntations.py).- [
-000023f0: 7079 746f 7263 682f 6578 616d 706c 6573  pytorch/examples
-00002400: 2f74 7261 696e 5f6d 6f64 656c 5f6f 6e5f  /train_model_on_
-00002410: 6361 7461 6c6f 672e 7079 5d28 6874 7470  catalog.py](http
-00002420: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00002430: 7761 6c6d 736c 6579 2f7a 6f6f 626f 742f  walmsley/zoobot/
-00002440: 626c 6f62 2f6d 6169 6e2f 7a6f 6f62 6f74  blob/main/zoobot
-00002450: 2f70 7974 6f72 6368 2f65 7861 6d70 6c65  /pytorch/example
-00002460: 732f 7472 6169 6e5f 6d6f 6465 6c5f 6f6e  s/train_model_on
-00002470: 5f63 6174 616c 6f67 2e70 7929 2028 6f6e  _catalog.py) (on
-00002480: 6c79 206e 6563 6573 7361 7279 2074 6f20  ly necessary to 
-00002490: 7472 6169 6e20 6672 6f6d 2073 6372 6174  train from scrat
-000024a0: 6368 290a 0a54 656e 736f 7246 6c6f 773a  ch)..TensorFlow:
-000024b0: 0a2d 205b 7465 6e73 6f72 666c 6f77 2f65  .- [tensorflow/e
-000024c0: 7861 6d70 6c65 732f 7472 6169 6e5f 6d6f  xamples/train_mo
-000024d0: 6465 6c5f 6f6e 5f63 6174 616c 6f67 2e70  del_on_catalog.p
-000024e0: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-000024f0: 622e 636f 6d2f 6d77 616c 6d73 6c65 792f  b.com/mwalmsley/
-00002500: 7a6f 6f62 6f74 2f62 6c6f 622f 6d61 696e  zoobot/blob/main
-00002510: 2f7a 6f6f 626f 742f 7465 6e73 6f72 666c  /zoobot/tensorfl
-00002520: 6f77 2f65 7861 6d70 6c65 732f 7472 6169  ow/examples/trai
-00002530: 6e5f 6d6f 6465 6c5f 6f6e 5f63 6174 616c  n_model_on_catal
-00002540: 6f67 2e70 7929 2028 6f6e 6c79 206e 6563  og.py) (only nec
-00002550: 6573 7361 7279 2074 6f20 7472 6169 6e20  essary to train 
-00002560: 6672 6f6d 2073 6372 6174 6368 290a 2d20  from scratch).- 
-00002570: 5b74 656e 736f 7266 6c6f 772f 6578 616d  [tensorflow/exam
-00002580: 706c 6573 2f6d 616b 655f 7072 6564 6963  ples/make_predic
-00002590: 7469 6f6e 732e 7079 5d28 6874 7470 733a  tions.py](https:
-000025a0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 7761  //github.com/mwa
-000025b0: 6c6d 736c 6579 2f7a 6f6f 626f 742f 626c  lmsley/zoobot/bl
-000025c0: 6f62 2f6d 6169 6e2f 7a6f 6f62 6f74 2f74  ob/main/zoobot/t
-000025d0: 656e 736f 7266 6c6f 772f 6578 616d 706c  ensorflow/exampl
-000025e0: 6573 2f6d 616b 655f 7072 6564 6963 7469  es/make_predicti
-000025f0: 6f6e 732e 7079 290a 2d20 5b74 656e 736f  ons.py).- [tenso
-00002600: 7266 6c6f 772f 6578 616d 706c 6573 2f66  rflow/examples/f
-00002610: 696e 6574 756e 655f 6d69 6e69 6d61 6c2e  inetune_minimal.
-00002620: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-00002630: 7562 2e63 6f6d 2f6d 7761 6c6d 736c 6579  ub.com/mwalmsley
-00002640: 2f7a 6f6f 626f 742f 626c 6f62 2f6d 6169  /zoobot/blob/mai
-00002650: 6e2f 7a6f 6f62 6f74 2f74 656e 736f 7266  n/zoobot/tensorf
-00002660: 6c6f 772f 6578 616d 706c 6573 2f66 696e  low/examples/fin
-00002670: 6574 756e 655f 6d69 6e69 6d61 6c2e 7079  etune_minimal.py
-00002680: 290a 2d20 5b74 656e 736f 7266 6c6f 772f  ).- [tensorflow/
-00002690: 6578 616d 706c 6573 2f66 696e 6574 756e  examples/finetun
-000026a0: 655f 6164 7661 6e63 6564 2e70 795d 2868  e_advanced.py](h
-000026b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000026c0: 6d2f 6d77 616c 6d73 6c65 792f 7a6f 6f62  m/mwalmsley/zoob
-000026d0: 6f74 2f62 6c6f 622f 6d61 696e 2f7a 6f6f  ot/blob/main/zoo
-000026e0: 626f 742f 7465 6e73 6f72 666c 6f77 2f65  bot/tensorflow/e
-000026f0: 7861 6d70 6c65 732f 6669 6e65 7475 6e65  xamples/finetune
-00002700: 5f61 6476 616e 6365 642e 7079 290a 0a54  _advanced.py)..T
-00002710: 6865 7265 2069 7320 6d6f 7265 2065 7870  here is more exp
-00002720: 6c61 6e61 7469 6f6e 2061 6e64 2061 6e20  lanation and an 
-00002730: 4150 4920 7265 6665 7265 6e63 6520 6f6e  API reference on
-00002740: 2074 6865 205b 646f 6373 5d28 6874 7470   the [docs](http
-00002750: 733a 2f2f 7a6f 6f62 6f74 2e72 6561 6474  s://zoobot.readt
-00002760: 6865 646f 6373 2e69 6f2f 292e 0a0a 4920  hedocs.io/)...I 
-00002770: 616c 736f 205b 696e 636c 7564 655d 2868  also [include](h
-00002780: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002790: 6d2f 6d77 616c 6d73 6c65 792f 7a6f 6f62  m/mwalmsley/zoob
-000027a0: 6f74 2f62 6c6f 622f 6d61 696e 2f62 656e  ot/blob/main/ben
-000027b0: 6368 6d61 726b 7329 2074 6865 2073 6372  chmarks) the scr
-000027c0: 6970 7473 2075 7365 6420 746f 2063 7265  ipts used to cre
-000027d0: 6174 6520 616e 6420 6265 6e63 686d 6172  ate and benchmar
-000027e0: 6b20 6f75 7220 7072 6574 7261 696e 6564  k our pretrained
-000027f0: 206d 6f64 656c 732e 204d 616e 7920 7072   models. Many pr
-00002800: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
-00002810: 6172 6520 6176 6169 6c61 626c 6520 5b61  are available [a
-00002820: 6c72 6561 6479 5d28 6874 7470 733a 2f2f  lready](https://
-00002830: 7a6f 6f62 6f74 2e72 6561 6474 6865 646f  zoobot.readthedo
-00002840: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00002850: 6461 7461 5f6e 6f74 6573 2e68 746d 6c29  data_notes.html)
-00002860: 2c20 6275 7420 6966 2079 6f75 206e 6565  , but if you nee
-00002870: 6420 6f6e 6520 7472 6169 6e65 6420 6f6e  d one trained on
-00002880: 2065 2e67 2e20 6469 6666 6572 656e 7420   e.g. different 
-00002890: 696e 7075 7420 696d 6167 6520 7369 7a65  input image size
-000028a0: 7320 6f72 2077 6974 6820 6120 7370 6563  s or with a spec
-000028b0: 6966 6963 2061 7263 6869 7465 6374 7572  ific architectur
-000028c0: 652c 2049 2063 616e 2070 726f 6261 626c  e, I can probabl
-000028d0: 7920 6d61 6b65 2069 7420 666f 7220 796f  y make it for yo
-000028e0: 752e 0a0a 5768 656e 2074 7261 696e 6564  u...When trained
-000028f0: 2077 6974 6820 6120 6465 6369 7369 6f6e   with a decision
-00002900: 2074 7265 6520 6865 6164 2028 5a6f 6f62   tree head (Zoob
-00002910: 6f74 5472 6565 2c20 4669 6e65 7475 6e65  otTree, Finetune
-00002920: 6162 6c65 5a6f 6f62 6f74 5472 6565 292c  ableZoobotTree),
-00002930: 205a 6f6f 626f 7420 6361 6e20 6c65 6172   Zoobot can lear
-00002940: 6e20 6672 6f6d 2076 6f6c 756e 7465 6572  n from volunteer
-00002950: 206c 6162 656c 7320 6f66 2076 6172 7969   labels of varyi
-00002960: 6e67 2063 6f6e 6669 6465 6e63 6520 616e  ng confidence an
-00002970: 6420 7072 6564 6963 7420 706f 7374 6572  d predict poster
-00002980: 696f 7273 2066 6f72 2077 6861 7420 7468  iors for what th
-00002990: 6520 7479 7069 6361 6c20 766f 6c75 6e74  e typical volunt
-000029a0: 6565 7220 6d69 6768 7420 7361 792e 2053  eer might say. S
-000029b0: 7065 6369 6669 6361 6c6c 792c 2074 6869  pecifically, thi
-000029c0: 7320 5a6f 6f62 6f74 206d 6f64 6520 7072  s Zoobot mode pr
-000029d0: 6564 6963 7473 2074 6865 2070 6172 616d  edicts the param
-000029e0: 6574 6572 7320 666f 7220 6469 7374 7269  eters for distri
-000029f0: 6275 7469 6f6e 732c 206e 6f74 2073 696d  butions, not sim
-00002a00: 706c 6520 636c 6173 7320 6c61 6265 6c73  ple class labels
-00002a10: 2120 466f 7220 6120 6465 6d6f 6e73 7472  ! For a demonstr
-00002a20: 6174 696f 6e20 6f66 2068 6f77 2074 6f20  ation of how to 
-00002a30: 696e 7465 7270 7265 7420 7468 6573 6520  interpret these 
-00002a40: 7072 6564 6963 7469 6f6e 732c 2073 6565  predictions, see
-00002a50: 2074 6865 205b 677a 5f64 6563 616c 735f   the [gz_decals_
-00002a60: 6461 7461 5f72 656c 6561 7365 5f61 6e61  data_release_ana
-00002a70: 6c79 7369 735f 6465 6d6f 2e69 7079 6e62  lysis_demo.ipynb
-00002a80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002a90: 2e63 6f6d 2f6d 7761 6c6d 736c 6579 2f7a  .com/mwalmsley/z
-00002aa0: 6f6f 626f 742f 626c 6f62 2f6d 6169 6e2f  oobot/blob/main/
-00002ab0: 677a 5f64 6563 616c 735f 6461 7461 5f72  gz_decals_data_r
-00002ac0: 656c 6561 7365 5f61 6e61 6c79 7369 735f  elease_analysis_
-00002ad0: 6465 6d6f 2e69 7079 6e62 292e 0a0a 0a0a  demo.ipynb).....
-00002ae0: 2323 2320 284f 7074 696f 6e61 6c29 2049  ### (Optional) I
-00002af0: 6e73 7461 6c6c 2050 7954 6f72 6368 206f  nstall PyTorch o
-00002b00: 7220 5465 6e73 6f72 466c 6f77 2c20 7769  r TensorFlow, wi
-00002b10: 7468 2043 5544 410a 3c61 206e 616d 653d  th CUDA.<a name=
-00002b20: 2269 6e73 7461 6c6c 5f63 7564 6122 3e3c  "install_cuda"><
-00002b30: 2f61 3e0a 0a2a 4966 2079 6f75 2772 6520  /a>..*If you're 
-00002b40: 6e6f 7420 7573 696e 6720 6120 4750 552c  not using a GPU,
-00002b50: 2073 6b69 7020 7468 6973 2073 7465 702e   skip this step.
-00002b60: 2055 7365 2074 6865 2070 7974 6f72 6368   Use the pytorch
-00002b70: 5f63 7075 206f 7220 7465 6e73 6f72 666c  _cpu or tensorfl
-00002b80: 6f77 5f63 7075 206f 7074 696f 6e73 2069  ow_cpu options i
-00002b90: 6e20 7468 6520 7365 6374 696f 6e20 6265  n the section be
-00002ba0: 6c6f 772e 2a0a 0a49 6e73 7461 6c6c 2050  low.*..Install P
-00002bb0: 7954 6f72 6368 2031 2e31 322e 3120 6f72  yTorch 1.12.1 or
-00002bc0: 2054 656e 736f 7266 6c6f 7720 322e 3130   Tensorflow 2.10
-00002bd0: 2e30 2061 6e64 2063 6f6d 7061 7469 626c  .0 and compatibl
-00002be0: 6520 4355 4441 2064 7269 7665 7273 2e20  e CUDA drivers. 
-00002bf0: 4920 6869 6768 6c79 2072 6563 6f6d 6d65  I highly recomme
-00002c00: 6e64 2075 7369 6e67 205b 636f 6e64 615d  nd using [conda]
-00002c10: 2868 7474 7073 3a2f 2f64 6f63 732e 636f  (https://docs.co
-00002c20: 6e64 612e 696f 2f65 6e2f 6c61 7465 7374  nda.io/en/latest
-00002c30: 2f6d 696e 6963 6f6e 6461 2e68 746d 6c29  /miniconda.html)
-00002c40: 2074 6f20 646f 2074 6869 732e 2043 6f6e   to do this. Con
-00002c50: 6461 2077 696c 6c20 6861 6e64 6c65 2062  da will handle b
-00002c60: 6f74 6820 6372 6561 7469 6e67 2061 206e  oth creating a n
-00002c70: 6577 2076 6972 7475 616c 2065 6e76 6972  ew virtual envir
-00002c80: 6f6e 6d65 6e74 2028 6063 6f6e 6461 2063  onment (`conda c
-00002c90: 7265 6174 6560 2920 616e 6420 696e 7374  reate`) and inst
-00002ca0: 616c 6c69 6e67 2043 5544 4120 2860 6375  alling CUDA (`cu
-00002cb0: 6461 746f 6f6c 6b69 7460 2c20 6063 7564  datoolkit`, `cud
-00002cc0: 6e6e 6029 0a0a 4355 4441 2031 312e 3320  nn`)..CUDA 11.3 
-00002cd0: 666f 7220 5079 546f 7263 683a 0a0a 2020  for PyTorch:..  
-00002ce0: 2020 636f 6e64 6120 6372 6561 7465 202d    conda create -
-00002cf0: 2d6e 616d 6520 7a6f 6f62 6f74 3338 5f74  -name zoobot38_t
-00002d00: 6f72 6368 2070 7974 686f 6e3d 3d33 2e38  orch python==3.8
-00002d10: 0a20 2020 2063 6f6e 6461 2061 6374 6976  .    conda activ
-00002d20: 6174 6520 7a6f 6f62 6f74 3338 5f74 6f72  ate zoobot38_tor
-00002d30: 6368 0a20 2020 2063 6f6e 6461 2069 6e73  ch.    conda ins
-00002d40: 7461 6c6c 202d 6320 636f 6e64 612d 666f  tall -c conda-fo
-00002d50: 7267 6520 6375 6461 746f 6f6c 6b69 743d  rge cudatoolkit=
-00002d60: 3131 2e33 0a0a 4355 4441 2031 312e 3220  11.3..CUDA 11.2 
-00002d70: 616e 6420 4355 444e 4e20 382e 3120 666f  and CUDNN 8.1 fo
-00002d80: 7220 5465 6e73 6f72 466c 6f77 2032 2e31  r TensorFlow 2.1
-00002d90: 302e 303a 0a0a 2020 2020 636f 6e64 6120  0.0:..    conda 
-00002da0: 6372 6561 7465 202d 2d6e 616d 6520 7a6f  create --name zo
-00002db0: 6f62 6f74 3338 5f74 6620 7079 7468 6f6e  obot38_tf python
-00002dc0: 3d3d 332e 380a 2020 2020 636f 6e64 6120  ==3.8.    conda 
-00002dd0: 6163 7469 7661 7465 207a 6f6f 626f 7433  activate zoobot3
-00002de0: 385f 7466 0a20 2020 2063 6f6e 6461 2069  8_tf.    conda i
-00002df0: 6e73 7461 6c6c 202d 6320 636f 6e64 612d  nstall -c conda-
-00002e00: 666f 7267 6520 6375 6461 746f 6f6c 6b69  forge cudatoolki
-00002e10: 743d 3131 2e32 2063 7564 6e6e 3d38 2e31  t=11.2 cudnn=8.1
-00002e20: 2e30 0a20 2020 2065 7870 6f72 7420 4c44  .0.    export LD
-00002e30: 5f4c 4942 5241 5259 5f50 4154 483d 244c  _LIBRARY_PATH=$L
-00002e40: 445f 4c49 4252 4152 595f 5041 5448 3a24  D_LIBRARY_PATH:$
-00002e50: 434f 4e44 415f 5052 4546 4958 2f6c 6962  CONDA_PREFIX/lib
-00002e60: 2f20 2023 2061 6464 2074 6869 7320 656e  /  # add this en
-00002e70: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00002e80: 6c65 0a0a 2323 2320 4c61 7465 7374 206d  le..### Latest m
-00002e90: 696e 6f72 2066 6561 7475 7265 7320 2876  inor features (v
-00002ea0: 312e 302e 3429 0a0a 2d20 4e6f 7720 7375  1.0.4)..- Now su
-00002eb0: 7070 6f72 7473 206d 756c 7469 2d63 6c61  pports multi-cla
-00002ec0: 7373 2066 696e 6574 756e 696e 672e 2053  ss finetuning. S
-00002ed0: 6565 2060 7079 746f 7263 682f 6578 616d  ee `pytorch/exam
-00002ee0: 706c 6573 2f66 696e 6574 756e 696e 672f  ples/finetuning/
-00002ef0: 6669 6e65 7475 6e65 5f6d 756c 7469 636c  finetune_multicl
-00002f00: 6173 735f 636c 6173 7369 6669 6361 7469  ass_classificati
-00002f10: 6f6e 2e70 7960 0a2d 2052 656d 6f76 6564  on.py`.- Removed
-00002f20: 2060 7369 6d70 6c65 6a70 6567 6020 6465   `simplejpeg` de
-00002f30: 7065 6e64 656e 6379 2064 7565 2074 6f20  pendency due to 
-00002f40: 4d31 2069 6e73 7461 6c6c 2069 7373 7565  M1 install issue
-00002f50: 2e20 0a2d 2050 696e 6e65 6420 6074 696d  . .- Pinned `tim
-00002f60: 6d60 2076 6572 7369 6f6e 2074 6f20 656e  m` version to en
-00002f70: 7375 7265 204d 6158 2d56 6954 206d 6f64  sure MaX-ViT mod
-00002f80: 656c 7320 6c6f 6164 2063 6f72 7265 6374  els load correct
-00002f90: 6c79 2e20 4d6f 6465 6c73 2073 7570 706f  ly. Models suppo
-00002fa0: 7274 696e 6720 7468 6520 6c61 7465 7374  rting the latest
-00002fb0: 2060 7469 6d6d 6020 7769 6c6c 2066 6f6c   `timm` will fol
-00002fc0: 6c6f 772e 0a2d 2028 696e 7465 726e 616c  low..- (internal
-00002fd0: 2075 6e74 696c 2070 7562 6c69 7368 6564   until published
-00002fe0: 2920 475a 2045 766f 2076 3220 6e6f 7720  ) GZ Evo v2 now 
-00002ff0: 696e 636c 7564 6573 2043 6f73 6d69 6320  includes Cosmic 
-00003000: 4461 776e 2028 4853 4329 2e20 5369 676e  Dawn (HSC). Sign
-00003010: 6966 6963 616e 7420 7065 7266 6f72 6d61  ificant performa
-00003020: 6e63 6520 696d 7072 6f76 656d 656e 7420  nce improvement 
-00003030: 6f6e 2048 5343 2066 696e 6574 756e 696e  on HSC finetunin
-00003040: 672e 0a0a 2323 2320 4c61 7465 7374 206d  g...### Latest m
-00003050: 616a 6f72 2066 6561 7475 7265 7320 2876  ajor features (v
-00003060: 312e 302e 3029 0a0a 7631 2e30 2e30 2072  1.0.0)..v1.0.0 r
-00003070: 6563 6f67 6e69 7365 7320 7468 6174 206d  ecognises that m
-00003080: 6f73 7420 6f66 2074 6865 2063 6f6d 706c  ost of the compl
-00003090: 6578 6974 7920 696e 2074 6869 7320 7265  exity in this re
-000030a0: 706f 2069 7320 7472 6169 6e69 6e67 205a  po is training Z
-000030b0: 6f6f 626f 7420 6672 6f6d 2073 6372 6174  oobot from scrat
-000030c0: 6368 2c20 6275 7420 6d6f 7374 206e 6f6e  ch, but most non
-000030d0: 2d47 5a20 7573 6572 7320 7769 6c6c 2070  -GZ users will p
-000030e0: 726f 6261 626c 7920 7369 6d70 6c79 2077  robably simply w
-000030f0: 616e 7420 746f 206c 6f61 6420 7468 6520  ant to load the 
-00003100: 7072 6574 7261 696e 6564 205a 6f6f 626f  pretrained Zoobo
-00003110: 7420 616e 6420 6669 6e65 7475 6e65 2069  t and finetune i
-00003120: 7420 6f6e 2074 6865 6972 2064 6174 612e  t on their data.
-00003130: 0a0a 2d20 4164 6473 206e 6577 2066 696e  ..- Adds new fin
-00003140: 6574 756e 696e 6720 696e 7465 7266 6163  etuning interfac
-00003150: 6520 2860 6669 6e65 7475 6e65 2e72 756e  e (`finetune.run
-00003160: 5f66 696e 6574 756e 696e 6728 2960 292c  _finetuning()`),
-00003170: 2065 7861 6d70 6c65 732e 0a2d 2052 6566   examples..- Ref
-00003180: 6f63 7573 6573 2064 6f63 7320 6f6e 2066  ocuses docs on f
-00003190: 696e 6574 756e 696e 6720 7261 7468 6572  inetuning rather
-000031a0: 2074 6861 6e20 7472 6169 6e69 6e67 2066   than training f
-000031b0: 726f 6d20 7363 7261 7463 682e 0a2d 2052  rom scratch..- R
-000031c0: 6577 6f72 6b20 696e 7374 616c 6c61 7469  ework installati
-000031d0: 6f6e 2070 726f 6365 7373 2074 6f20 7365  on process to se
-000031e0: 7061 7261 7465 2043 5544 4120 6672 6f6d  parate CUDA from
-000031f0: 205a 6f6f 626f 7420 2873 696d 706c 6572   Zoobot (simpler
-00003200: 2c20 6561 7369 6572 290a 2d20 4265 7474  , easier).- Bett
-00003210: 6572 2077 616e 6462 206c 6f67 6769 6e67  er wandb logging
-00003220: 2074 6872 6f75 6768 6f75 742c 2074 6f20   throughout, to 
-00003230: 6d6f 6e69 746f 7220 7472 6169 6e69 6e67  monitor training
-00003240: 0a2d 2052 656d 6f76 6520 6e65 6564 2074  .- Remove need t
-00003250: 6f20 6d61 6b65 2054 4652 6563 6f72 6473  o make TFRecords
-00003260: 2e20 4e6f 7720 5446 2064 6972 6563 746c  . Now TF directl
-00003270: 7920 7573 6573 2069 6d61 6765 732e 0a2d  y uses images..-
-00003280: 2052 6566 6163 746f 7220 6f75 7420 6175   Refactor out au
-00003290: 676d 656e 7461 7469 6f6e 7320 616e 6420  gmentations and 
-000032a0: 6461 7461 7365 7473 2074 6f20 6067 616c  datasets to `gal
-000032b0: 6178 792d 6461 7461 7365 7473 6020 7265  axy-datasets` re
-000032c0: 706f 2e20 5446 2061 6e64 2054 6f72 6368  po. TF and Torch
-000032d0: 206e 6f77 2075 7365 2069 6465 6e74 6963   now use identic
-000032e0: 616c 2061 7567 6d65 6e74 6174 696f 6e73  al augmentations
-000032f0: 2028 7669 6120 616c 6275 6d65 6e74 6174   (via albumentat
-00003300: 696f 6e73 292e 0a2d 204d 616e 7920 736d  ions)..- Many sm
-00003310: 616c 6c20 7175 616c 6974 792d 6f66 2d6c  all quality-of-l
-00003320: 6966 6520 696d 7072 6f76 656d 656e 7473  ife improvements
-00003330: 0a0a 436f 6e74 7269 6275 7469 6f6e 7320  ..Contributions 
-00003340: 6172 6520 7665 7279 2077 656c 636f 6d65  are very welcome
-00003350: 2061 6e64 2077 696c 6c20 6265 2063 7265   and will be cre
-00003360: 6469 7465 6420 696e 2061 6e79 2066 7574  dited in any fut
-00003370: 7572 6520 776f 726b 2e20 506c 6561 7365  ure work. Please
-00003380: 2067 6574 2069 6e20 746f 7563 6821 2053   get in touch! S
-00003390: 6565 205b 434f 4e54 5249 4255 5449 4e47  ee [CONTRIBUTING
-000033a0: 2e6d 645d 2868 7474 7073 3a2f 2f67 6974  .md](https://git
-000033b0: 6875 622e 636f 6d2f 6d77 616c 6d73 6c65  hub.com/mwalmsle
-000033c0: 792f 7a6f 6f62 6f74 2f62 6c6f 622f 6d61  y/zoobot/blob/ma
-000033d0: 696e 2f62 656e 6368 6d61 726b 7329 2066  in/benchmarks) f
-000033e0: 6f72 206d 6f72 652e 0a0a 2323 2320 4265  or more...### Be
-000033f0: 6e63 686d 6172 6b73 2061 6e64 2052 6570  nchmarks and Rep
-00003400: 6c69 6361 7469 6f6e 202d 2054 7261 696e  lication - Train
-00003410: 696e 6720 6672 6f6d 2053 6372 6174 6368  ing from Scratch
-00003420: 0a0a 5468 6520 5b62 656e 6368 6d61 726b  ..The [benchmark
-00003430: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00003440: 622e 636f 6d2f 6d77 616c 6d73 6c65 792f  b.com/mwalmsley/
-00003450: 7a6f 6f62 6f74 2f62 6c6f 622f 6d61 696e  zoobot/blob/main
-00003460: 2f62 656e 6368 6d61 726b 7329 2066 6f6c  /benchmarks) fol
-00003470: 6465 7220 636f 6e74 6169 6e73 2073 6c75  der contains slu
-00003480: 726d 2061 6e64 2050 7974 686f 6e20 7363  rm and Python sc
-00003490: 7269 7074 7320 746f 2074 7261 696e 205a  ripts to train Z
-000034a0: 6f6f 626f 7420 6672 6f6d 2073 6372 6174  oobot from scrat
-000034b0: 6368 2e20 5765 2075 7365 2074 6865 7365  ch. We use these
-000034c0: 2073 6372 6970 7473 2074 6f20 6d61 6b65   scripts to make
-000034d0: 2073 7572 6520 6e65 7720 636f 6465 2076   sure new code v
-000034e0: 6572 7369 6f6e 7320 776f 726b 2077 656c  ersions work wel
-000034f0: 6c2c 2061 6e64 2074 6861 7420 5465 6e73  l, and that Tens
-00003500: 6f72 466c 6f77 2061 6e64 2050 7954 6f72  orFlow and PyTor
-00003510: 6368 2061 6368 6965 7665 2073 696d 696c  ch achieve simil
-00003520: 6172 2070 6572 666f 726d 616e 6365 2e0a  ar performance..
-00003530: 0a54 7261 696e 696e 6720 5a6f 6f62 6f74  .Training Zoobot
-00003540: 2075 7369 6e67 2074 6865 2047 5a20 4445   using the GZ DE
-00003550: 4361 4c53 2064 6174 6173 6574 206f 7074  CaLS dataset opt
-00003560: 696f 6e20 7769 6c6c 2063 7265 6174 6520  ion will create 
-00003570: 6d6f 6465 6c73 2076 6572 7920 7369 6d69  models very simi
-00003580: 6c61 7220 746f 2074 686f 7365 2075 7365  lar to those use
-00003590: 6420 666f 7220 7468 6520 475a 2044 4543  d for the GZ DEC
-000035a0: 614c 5320 6361 7461 6c6f 6775 6520 616e  aLS catalogue an
-000035b0: 6420 7368 6172 6564 2077 6974 6820 7468  d shared with th
-000035c0: 6520 6561 726c 7920 7665 7273 696f 6e73  e early versions
-000035d0: 206f 6620 7468 6973 2072 6570 6f2e 2054   of this repo. T
-000035e0: 6865 2047 5a20 4445 5349 205a 6f6f 626f  he GZ DESI Zoobo
-000035f0: 7420 6d6f 6465 6c20 6973 2074 7261 696e  t model is train
-00003600: 6564 206f 6e20 6164 6469 7469 6f6e 616c  ed on additional
-00003610: 2064 6174 6120 2847 5a44 2d31 2c20 475a   data (GZD-1, GZ
-00003620: 442d 3229 2c20 6173 2074 6865 2047 5a20  D-2), as the GZ 
-00003630: 4576 6f20 5a6f 6f62 6f74 206d 6f64 656c  Evo Zoobot model
-00003640: 2028 475a 442d 312f 322f 352c 2048 7562   (GZD-1/2/5, Hub
-00003650: 626c 652c 2043 616e 6465 6c73 2c20 475a  ble, Candels, GZ
-00003660: 3229 2e0a 0a23 2323 2043 6974 696e 670a  2)...### Citing.
-00003670: 0a49 6620 796f 7520 7573 6520 7468 6973  .If you use this
-00003680: 2073 6f66 7477 6172 652c 206f 7220 6f74   software, or ot
-00003690: 6865 7277 6973 6520 7769 7368 2074 6f20  herwise wish to 
-000036a0: 6369 7465 205a 6f6f 626f 7420 6173 2061  cite Zoobot as a
-000036b0: 2073 6f66 7477 6172 6520 7061 636b 6167   software packag
-000036c0: 652c 2070 6c65 6173 6520 7573 6520 7468  e, please use th
-000036d0: 6520 5b4a 4f53 5320 7061 7065 725d 2868  e [JOSS paper](h
-000036e0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-000036f0: 302e 3231 3130 352f 6a6f 7373 2e30 3533  0.21105/joss.053
-00003700: 3132 293a 0a0a 2020 2020 4061 7274 6963  12):..    @artic
-00003710: 6c65 7b57 616c 6d73 6c65 7932 3032 332c  le{Walmsley2023,
-00003720: 2064 6f69 203d 207b 3130 2e32 3131 3035   doi = {10.21105
-00003730: 2f6a 6f73 732e 3035 3331 327d 2c20 7572  /joss.05312}, ur
-00003740: 6c20 3d20 7b68 7474 7073 3a2f 2f64 6f69  l = {https://doi
-00003750: 2e6f 7267 2f31 302e 3231 3130 352f 6a6f  .org/10.21105/jo
-00003760: 7373 2e30 3533 3132 7d2c 2079 6561 7220  ss.05312}, year 
-00003770: 3d20 7b32 3032 337d 2c20 7075 626c 6973  = {2023}, publis
-00003780: 6865 7220 3d20 7b54 6865 204f 7065 6e20  her = {The Open 
-00003790: 4a6f 7572 6e61 6c7d 2c20 766f 6c75 6d65  Journal}, volume
-000037a0: 203d 207b 387d 2c20 6e75 6d62 6572 203d   = {8}, number =
-000037b0: 207b 3835 7d2c 2070 6167 6573 203d 207b   {85}, pages = {
-000037c0: 3533 3132 7d2c 2061 7574 686f 7220 3d20  5312}, author = 
-000037d0: 7b4d 696b 6520 5761 6c6d 736c 6579 2061  {Mike Walmsley a
-000037e0: 6e64 2043 616d 7062 656c 6c20 416c 6c65  nd Campbell Alle
-000037f0: 6e20 616e 6420 4265 6e20 4175 7373 656c  n and Ben Aussel
-00003800: 2061 6e64 204d 6963 6168 2042 6f77 6c65   and Micah Bowle
-00003810: 7320 616e 6420 4b61 7369 6120 4772 6567  s and Kasia Greg
-00003820: 6f72 6f77 6963 7a20 616e 6420 496e 6967  orowicz and Inig
-00003830: 6f20 5661 6c20 536c 696a 6570 6365 7669  o Val Slijepcevi
-00003840: 6320 616e 6420 4368 7269 7320 4a2e 204c  c and Chris J. L
-00003850: 696e 746f 7474 2061 6e64 2041 6e6e 6120  intott and Anna 
-00003860: 4d2e 206d 2e20 5363 6169 6665 2061 6e64  M. m. Scaife and
-00003870: 204d 616a 6120 4a61 62c5 826f c584 736b   Maja Jab..o..sk
-00003880: 6120 616e 6420 4b6f 7369 6f20 4b61 7263  a and Kosio Karc
-00003890: 6865 7620 616e 6420 4465 6e69 7365 204c  hev and Denise L
-000038a0: 616e 7a69 6572 6920 616e 6420 4465 7669  anzieri and Devi
-000038b0: 6e61 204d 6f68 616e 2061 6e64 2044 6176  na Mohan and Dav
-000038c0: 6964 204f e280 9952 7961 6e20 616e 6420  id O...Ryan and 
-000038d0: 4268 6172 6174 6820 5361 6967 7568 616e  Bharath Saiguhan
-000038e0: 2061 6e64 2043 7269 7365 6c20 5375 c3a1   and Crisel Su..
-000038f0: 7265 7a20 616e 6420 4e69 636f 6cc3 a173  rez and Nicol..s
-00003900: 2047 7565 7272 612d 5661 7261 7320 616e   Guerra-Varas an
-00003910: 6420 5265 6e75 6b61 2056 656c 757d 2c20  d Renuka Velu}, 
-00003920: 7469 746c 6520 3d20 7b5a 6f6f 626f 743a  title = {Zoobot:
-00003930: 2041 6461 7074 6162 6c65 2044 6565 7020   Adaptable Deep 
-00003940: 4c65 6172 6e69 6e67 204d 6f64 656c 7320  Learning Models 
-00003950: 666f 7220 4761 6c61 7879 204d 6f72 7068  for Galaxy Morph
-00003960: 6f6c 6f67 797d 2c20 6a6f 7572 6e61 6c20  ology}, journal 
-00003970: 3d20 7b4a 6f75 726e 616c 206f 6620 4f70  = {Journal of Op
-00003980: 656e 2053 6f75 7263 6520 536f 6674 7761  en Source Softwa
-00003990: 7265 7d20 7d20 0a0a 596f 7520 6d69 6768  re} } ..You migh
-000039a0: 7420 6265 2069 6e74 6572 6573 7465 6420  t be interested 
-000039b0: 696e 2072 6561 6469 6e67 2070 6170 6572  in reading paper
-000039c0: 7320 7573 696e 6720 5a6f 6f62 6f74 3a0a  s using Zoobot:.
-000039d0: 0a2d 205b 4761 6c61 7879 205a 6f6f 2044  .- [Galaxy Zoo D
-000039e0: 4543 614c 533a 2044 6574 6169 6c65 6420  ECaLS: Detailed 
-000039f0: 7669 7375 616c 206d 6f72 7068 6f6c 6f67  visual morpholog
-00003a00: 7920 6d65 6173 7572 656d 656e 7473 2066  y measurements f
-00003a10: 726f 6d20 766f 6c75 6e74 6565 7273 2061  rom volunteers a
-00003a20: 6e64 2064 6565 7020 6c65 6172 6e69 6e67  nd deep learning
-00003a30: 2066 6f72 2033 3134 2c30 3030 2067 616c   for 314,000 gal
-00003a40: 6178 6965 735d 2868 7474 7073 3a2f 2f61  axies](https://a
-00003a50: 7278 6976 2e6f 7267 2f61 6273 2f32 3130  rxiv.org/abs/210
-00003a60: 322e 3038 3431 3429 2028 3230 3232 290a  2.08414) (2022).
-00003a70: 2d20 5b41 2043 6f6d 7061 7269 736f 6e20  - [A Comparison 
-00003a80: 6f66 2044 6565 7020 4c65 6172 6e69 6e67  of Deep Learning
-00003a90: 2041 7263 6869 7465 6374 7572 6573 2066   Architectures f
-00003aa0: 6f72 204f 7074 6963 616c 2047 616c 6178  or Optical Galax
-00003ab0: 7920 4d6f 7270 686f 6c6f 6779 2043 6c61  y Morphology Cla
-00003ac0: 7373 6966 6963 6174 696f 6e5d 2868 7474  ssification](htt
-00003ad0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00003ae0: 6273 2f32 3131 312e 3034 3335 3329 2028  bs/2111.04353) (
-00003af0: 3230 3232 290a 2d20 5b50 7261 6374 6963  2022).- [Practic
-00003b00: 616c 2047 616c 6178 7920 4d6f 7270 686f  al Galaxy Morpho
-00003b10: 6c6f 6779 2054 6f6f 6c73 2066 726f 6d20  logy Tools from 
-00003b20: 4465 6570 2053 7570 6572 7669 7365 6420  Deep Supervised 
-00003b30: 5265 7072 6573 656e 7461 7469 6f6e 204c  Representation L
-00003b40: 6561 726e 696e 675d 2868 7474 7073 3a2f  earning](https:/
-00003b50: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00003b60: 3131 302e 3132 3733 3529 2028 3230 3232  110.12735) (2022
-00003b70: 290a 2d20 5b54 6f77 6172 6473 2046 6f75  ).- [Towards Fou
-00003b80: 6e64 6174 696f 6e20 4d6f 6465 6c73 2066  ndation Models f
-00003b90: 6f72 2047 616c 6178 7920 4d6f 7270 686f  or Galaxy Morpho
-00003ba0: 6c6f 6779 5d28 6874 7470 733a 2f2f 6172  logy](https://ar
-00003bb0: 7869 762e 6f72 672f 6162 732f 3232 3036  xiv.org/abs/2206
-00003bc0: 2e31 3139 3237 2920 2832 3032 3229 0a2d  .11927) (2022).-
-00003bd0: 205b 4861 726e 6573 7369 6e67 2074 6865   [Harnessing the
-00003be0: 2048 7562 626c 6520 5370 6163 6520 5465   Hubble Space Te
-00003bf0: 6c65 7363 6f70 6520 4172 6368 6976 6573  lescope Archives
-00003c00: 3a20 4120 4361 7461 6c6f 6775 6520 6f66  : A Catalogue of
-00003c10: 2032 312c 3932 3620 496e 7465 7261 6374   21,926 Interact
-00003c20: 696e 6720 4761 6c61 7869 6573 5d28 6874  ing Galaxies](ht
-00003c30: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00003c40: 6162 732f 3233 3033 2e30 3033 3636 2920  abs/2303.00366) 
-00003c50: 2832 3032 3329 0a2d 205b 4173 7472 6f6e  (2023).- [Astron
-00003c60: 6f6d 616c 7920 6174 2053 6361 6c65 3a20  omaly at Scale: 
-00003c70: 5365 6172 6368 696e 6720 666f 7220 416e  Searching for An
-00003c80: 6f6d 616c 6965 7320 416d 6f6e 6773 7420  omalies Amongst 
-00003c90: 3420 4d69 6c6c 696f 6e20 4761 6c61 7869  4 Million Galaxi
-00003ca0: 6573 5d28 6874 7470 733a 2f2f 6172 7869  es](https://arxi
-00003cb0: 762e 6f72 672f 6162 732f 3233 3039 2e30  v.org/abs/2309.0
-00003cc0: 3836 3630 2920 2832 3032 3329 0a2d 205b  8660) (2023).- [
-00003cd0: 4761 6c61 7879 205a 6f6f 2044 4553 493a  Galaxy Zoo DESI:
-00003ce0: 2044 6574 6169 6c65 6420 6d6f 7270 686f   Detailed morpho
-00003cf0: 6c6f 6779 206d 6561 7375 7265 6d65 6e74  logy measurement
-00003d00: 7320 666f 7220 382e 374d 2067 616c 6178  s for 8.7M galax
-00003d10: 6965 7320 696e 2074 6865 2044 4553 4920  ies in the DESI 
-00003d20: 4c65 6761 6379 2049 6d61 6769 6e67 2053  Legacy Imaging S
-00003d30: 7572 7665 7973 5d28 6874 7470 733a 2f2f  urveys](https://
-00003d40: 6163 6164 656d 6963 2e6f 7570 2e63 6f6d  academic.oup.com
-00003d50: 2f6d 6e72 6173 2f61 6476 616e 6365 2d61  /mnras/advance-a
-00003d60: 7274 6963 6c65 2f64 6f69 2f31 302e 3130  rticle/doi/10.10
-00003d70: 3933 2f6d 6e72 6173 2f73 7461 6432 3931  93/mnras/stad291
-00003d80: 392f 3732 3833 3136 393f 6c6f 6769 6e3d  9/7283169?login=
-00003d90: 6661 6c73 6529 2028 3230 3233 290a 2d20  false) (2023).- 
-00003da0: 5b47 616c 6178 7920 6d65 7267 6572 7320  [Galaxy mergers 
-00003db0: 696e 2053 7562 6172 7520 4853 432d 5353  in Subaru HSC-SS
-00003dc0: 503a 2041 2064 6565 7020 7265 7072 6573  P: A deep repres
-00003dd0: 656e 7461 7469 6f6e 206c 6561 726e 696e  entation learnin
-00003de0: 6720 6170 7072 6f61 6368 2066 6f72 2069  g approach for i
-00003df0: 6465 6e74 6966 6963 6174 696f 6e2c 2061  dentification, a
-00003e00: 6e64 2074 6865 2072 6f6c 6520 6f66 2065  nd the role of e
-00003e10: 6e76 6972 6f6e 6d65 6e74 206f 6e20 6d65  nvironment on me
-00003e20: 7267 6572 2069 6e63 6964 656e 6365 5d28  rger incidence](
-00003e30: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
-00003e40: 3130 2e31 3035 312f 3030 3034 2d36 3336  10.1051/0004-636
-00003e50: 312f 3230 3233 3436 3734 3329 2028 3230  1/202346743) (20
-00003e60: 3233 290a 0a3c 212d 2d20 7375 626d 6974  23)..<!-- submit
-00003e70: 7465 6420 7061 7065 7273 3a20 7369 6d75  ted papers: simu
-00003e80: 6c61 7465 6420 6d65 7267 6572 2063 6c61  lated merger cla
-00003e90: 7373 6966 6963 6174 696f 6e2c 2075 6e73  ssification, uns
-00003ea0: 7570 6572 7669 7365 6420 616e 6f6d 616c  upervised anomal
-00003eb0: 7920 6465 7465 6374 696f 6e2c 2073 7461  y detection, sta
-00003ec0: 7266 6f72 6d69 6e67 2063 6c75 6d70 206c  rforming clump l
-00003ed0: 6f63 616c 6973 6174 696f 6e2c 2061 6e64  ocalisation, and
-00003ee0: 206d 6f72 7068 6f6c 6f67 6963 616c 2073   morphological s
-00003ef0: 6567 6d65 6e74 6174 696f 6e2e 202d 2d3e  egmentation. -->
-00003f00: 0a0a 4d61 6e79 206f 7468 6572 2077 6f72  ..Many other wor
-00003f10: 6b73 2075 7365 205a 6f6f 626f 7420 696e  ks use Zoobot in
-00003f20: 6469 7265 6374 6c79 2076 6961 2074 6865  directly via the
-00003f30: 205b 4761 6c61 7879 205a 6f6f 2044 4543   [Galaxy Zoo DEC
-00003f40: 614c 535d 2868 7474 7073 3a2f 2f61 7278  aLS](https://arx
-00003f50: 6976 2e6f 7267 2f61 6273 2f32 3130 322e  iv.org/abs/2102.
-00003f60: 3038 3431 3429 2063 6174 616c 6f67 2028  08414) catalog (
-00003f70: 616e 6420 6e6f 7720 7669 6120 7468 6520  and now via the 
-00003f80: 6e65 7720 5b47 616c 6178 7920 5a6f 6f20  new [Galaxy Zoo 
-00003f90: 4445 5349 5d28 6874 7470 733a 2f2f 6163  DESI](https://ac
-00003fa0: 6164 656d 6963 2e6f 7570 2e63 6f6d 2f6d  ademic.oup.com/m
-00003fb0: 6e72 6173 2f61 6476 616e 6365 2d61 7274  nras/advance-art
-00003fc0: 6963 6c65 2f64 6f69 2f31 302e 3130 3933  icle/doi/10.1093
-00003fd0: 2f6d 6e72 6173 2f73 7461 6432 3931 392f  /mnras/stad2919/
-00003fe0: 3732 3833 3136 393f 6c6f 6769 6e3d 6661  7283169?login=fa
-00003ff0: 6c73 6529 2063 6174 616c 6f67 292e 0a    lse) catalog)..
+00000320: 7374 3a20 7765 6264 6174 6173 6574 0a52  st: webdataset.R
+00000330: 6571 7569 7265 732d 4469 7374 3a20 6875  equires-Dist: hu
+00000340: 6767 696e 6766 6163 655f 6875 620a 5265  ggingface_hub.Re
+00000350: 7175 6972 6573 2d44 6973 743a 2073 6574  quires-Dist: set
+00000360: 7570 746f 6f6c 730a 5265 7175 6972 6573  uptools.Requires
+00000370: 2d44 6973 743a 2067 616c 6178 792d 6461  -Dist: galaxy-da
+00000380: 7461 7365 7473 3e3d 302e 302e 3137 0a50  tasets>=0.0.17.P
+00000390: 726f 7669 6465 732d 4578 7472 613a 2070  rovides-Extra: p
+000003a0: 7974 6f72 6368 2d63 7075 0a52 6571 7569  ytorch-cpu.Requi
+000003b0: 7265 732d 4469 7374 3a20 746f 7263 683d  res-Dist: torch=
+000003c0: 3d32 2e31 2e30 2b63 7075 3b20 6578 7472  =2.1.0+cpu; extr
+000003d0: 6120 3d3d 2022 7079 746f 7263 682d 6370  a == "pytorch-cp
+000003e0: 7522 0a52 6571 7569 7265 732d 4469 7374  u".Requires-Dist
+000003f0: 3a20 746f 7263 6876 6973 696f 6e3d 3d30  : torchvision==0
+00000400: 2e31 362e 302b 6370 753b 2065 7874 7261  .16.0+cpu; extra
+00000410: 203d 3d20 2270 7974 6f72 6368 2d63 7075   == "pytorch-cpu
+00000420: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000430: 2074 6f72 6368 6175 6469 6f3e 3d32 2e31   torchaudio>=2.1
+00000440: 2e30 3b20 6578 7472 6120 3d3d 2022 7079  .0; extra == "py
+00000450: 746f 7263 682d 6370 7522 0a52 6571 7569  torch-cpu".Requi
+00000460: 7265 732d 4469 7374 3a20 6c69 6768 746e  res-Dist: lightn
+00000470: 696e 673e 3d32 2e30 2e30 3b20 6578 7472  ing>=2.0.0; extr
+00000480: 6120 3d3d 2022 7079 746f 7263 682d 6370  a == "pytorch-cp
+00000490: 7522 0a52 6571 7569 7265 732d 4469 7374  u".Requires-Dist
+000004a0: 3a20 616c 6275 6d65 6e74 6174 696f 6e73  : albumentations
+000004b0: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
+000004c0: 7263 682d 6370 7522 0a52 6571 7569 7265  rch-cpu".Require
+000004d0: 732d 4469 7374 3a20 7079 726f 2d70 706c  s-Dist: pyro-ppl
+000004e0: 3e3d 312e 382e 363b 2065 7874 7261 203d  >=1.8.6; extra =
+000004f0: 3d20 2270 7974 6f72 6368 2d63 7075 220a  = "pytorch-cpu".
+00000500: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000510: 6f72 6368 6d65 7472 6963 733d 3d30 2e31  orchmetrics==0.1
+00000520: 312e 303b 2065 7874 7261 203d 3d20 2270  1.0; extra == "p
+00000530: 7974 6f72 6368 2d63 7075 220a 5265 7175  ytorch-cpu".Requ
+00000540: 6972 6573 2d44 6973 743a 2074 696d 6d3d  ires-Dist: timm=
+00000550: 3d30 2e39 2e31 303b 2065 7874 7261 203d  =0.9.10; extra =
+00000560: 3d20 2270 7974 6f72 6368 2d63 7075 220a  = "pytorch-cpu".
+00000570: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000580: 7079 746f 7263 682d 6d31 0a52 6571 7569  pytorch-m1.Requi
+00000590: 7265 732d 4469 7374 3a20 746f 7263 683d  res-Dist: torch=
+000005a0: 3d32 2e31 2e30 3b20 6578 7472 6120 3d3d  =2.1.0; extra ==
+000005b0: 2022 7079 746f 7263 682d 6d31 220a 5265   "pytorch-m1".Re
+000005c0: 7175 6972 6573 2d44 6973 743a 2074 6f72  quires-Dist: tor
+000005d0: 6368 7669 7369 6f6e 3d3d 302e 3136 2e30  chvision==0.16.0
+000005e0: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
+000005f0: 7263 682d 6d31 220a 5265 7175 6972 6573  rch-m1".Requires
+00000600: 2d44 6973 743a 2074 6f72 6368 6175 6469  -Dist: torchaudi
+00000610: 6f3e 3d32 2e31 2e30 3b20 6578 7472 6120  o>=2.1.0; extra 
+00000620: 3d3d 2022 7079 746f 7263 682d 6d31 220a  == "pytorch-m1".
+00000630: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
+00000640: 6967 6874 6e69 6e67 3e3d 322e 302e 303b  ightning>=2.0.0;
+00000650: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
+00000660: 6368 2d6d 3122 0a52 6571 7569 7265 732d  ch-m1".Requires-
+00000670: 4469 7374 3a20 616c 6275 6d65 6e74 6174  Dist: albumentat
+00000680: 696f 6e73 3b20 6578 7472 6120 3d3d 2022  ions; extra == "
+00000690: 7079 746f 7263 682d 6d31 220a 5265 7175  pytorch-m1".Requ
+000006a0: 6972 6573 2d44 6973 743a 2070 7972 6f2d  ires-Dist: pyro-
+000006b0: 7070 6c3e 3d31 2e38 2e36 3b20 6578 7472  ppl>=1.8.6; extr
+000006c0: 6120 3d3d 2022 7079 746f 7263 682d 6d31  a == "pytorch-m1
+000006d0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000006e0: 2074 6f72 6368 6d65 7472 6963 733d 3d30   torchmetrics==0
+000006f0: 2e31 312e 303b 2065 7874 7261 203d 3d20  .11.0; extra == 
+00000700: 2270 7974 6f72 6368 2d6d 3122 0a52 6571  "pytorch-m1".Req
+00000710: 7569 7265 732d 4469 7374 3a20 7469 6d6d  uires-Dist: timm
+00000720: 3e3d 302e 392e 3130 3b20 6578 7472 6120  >=0.9.10; extra 
+00000730: 3d3d 2022 7079 746f 7263 682d 6d31 220a  == "pytorch-m1".
+00000740: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000750: 7079 746f 7263 682d 6375 3131 380a 5265  pytorch-cu118.Re
+00000760: 7175 6972 6573 2d44 6973 743a 2074 6f72  quires-Dist: tor
+00000770: 6368 3d3d 322e 312e 302b 6375 3131 383b  ch==2.1.0+cu118;
+00000780: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
+00000790: 6368 2d63 7531 3138 220a 5265 7175 6972  ch-cu118".Requir
+000007a0: 6573 2d44 6973 743a 2074 6f72 6368 7669  es-Dist: torchvi
+000007b0: 7369 6f6e 3d3d 302e 3136 2e30 2b63 7531  sion==0.16.0+cu1
+000007c0: 3138 3b20 6578 7472 6120 3d3d 2022 7079  18; extra == "py
+000007d0: 746f 7263 682d 6375 3131 3822 0a52 6571  torch-cu118".Req
+000007e0: 7569 7265 732d 4469 7374 3a20 746f 7263  uires-Dist: torc
+000007f0: 6861 7564 696f 3e3d 322e 312e 303b 2065  haudio>=2.1.0; e
+00000800: 7874 7261 203d 3d20 2270 7974 6f72 6368  xtra == "pytorch
+00000810: 2d63 7531 3138 220a 5265 7175 6972 6573  -cu118".Requires
+00000820: 2d44 6973 743a 206c 6967 6874 6e69 6e67  -Dist: lightning
+00000830: 3e3d 322e 302e 303b 2065 7874 7261 203d  >=2.0.0; extra =
+00000840: 3d20 2270 7974 6f72 6368 2d63 7531 3138  = "pytorch-cu118
+00000850: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000860: 2061 6c62 756d 656e 7461 7469 6f6e 733b   albumentations;
+00000870: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
+00000880: 6368 2d63 7531 3138 220a 5265 7175 6972  ch-cu118".Requir
+00000890: 6573 2d44 6973 743a 2070 7972 6f2d 7070  es-Dist: pyro-pp
+000008a0: 6c3e 3d31 2e38 2e36 3b20 6578 7472 6120  l>=1.8.6; extra 
+000008b0: 3d3d 2022 7079 746f 7263 682d 6375 3131  == "pytorch-cu11
+000008c0: 3822 0a52 6571 7569 7265 732d 4469 7374  8".Requires-Dist
+000008d0: 3a20 746f 7263 686d 6574 7269 6373 3d3d  : torchmetrics==
+000008e0: 302e 3131 2e30 3b20 6578 7472 6120 3d3d  0.11.0; extra ==
+000008f0: 2022 7079 746f 7263 682d 6375 3131 3822   "pytorch-cu118"
+00000900: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000910: 7469 6d6d 3e3d 302e 392e 3130 3b20 6578  timm>=0.9.10; ex
+00000920: 7472 6120 3d3d 2022 7079 746f 7263 682d  tra == "pytorch-
+00000930: 6375 3131 3822 0a50 726f 7669 6465 732d  cu118".Provides-
+00000940: 4578 7472 613a 2070 7974 6f72 6368 2d63  Extra: pytorch-c
+00000950: 7531 3231 0a52 6571 7569 7265 732d 4469  u121.Requires-Di
+00000960: 7374 3a20 746f 7263 683d 3d32 2e31 2e30  st: torch==2.1.0
+00000970: 2b63 7531 3231 3b20 6578 7472 6120 3d3d  +cu121; extra ==
+00000980: 2022 7079 746f 7263 682d 6375 3132 3122   "pytorch-cu121"
+00000990: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000009a0: 746f 7263 6876 6973 696f 6e3d 3d30 2e31  torchvision==0.1
+000009b0: 362e 302b 6375 3132 313b 2065 7874 7261  6.0+cu121; extra
+000009c0: 203d 3d20 2270 7974 6f72 6368 2d63 7531   == "pytorch-cu1
+000009d0: 3231 220a 5265 7175 6972 6573 2d44 6973  21".Requires-Dis
+000009e0: 743a 2074 6f72 6368 6175 6469 6f3e 3d32  t: torchaudio>=2
+000009f0: 2e31 2e30 3b20 6578 7472 6120 3d3d 2022  .1.0; extra == "
+00000a00: 7079 746f 7263 682d 6375 3132 3122 0a52  pytorch-cu121".R
+00000a10: 6571 7569 7265 732d 4469 7374 3a20 6c69  equires-Dist: li
+00000a20: 6768 746e 696e 673e 3d32 2e30 2e30 3b20  ghtning>=2.0.0; 
+00000a30: 6578 7472 6120 3d3d 2022 7079 746f 7263  extra == "pytorc
+00000a40: 682d 6375 3132 3122 0a52 6571 7569 7265  h-cu121".Require
+00000a50: 732d 4469 7374 3a20 616c 6275 6d65 6e74  s-Dist: albument
+00000a60: 6174 696f 6e73 3b20 6578 7472 6120 3d3d  ations; extra ==
+00000a70: 2022 7079 746f 7263 682d 6375 3132 3122   "pytorch-cu121"
+00000a80: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000a90: 7079 726f 2d70 706c 3e3d 312e 382e 363b  pyro-ppl>=1.8.6;
+00000aa0: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
+00000ab0: 6368 2d63 7531 3231 220a 5265 7175 6972  ch-cu121".Requir
+00000ac0: 6573 2d44 6973 743a 2074 6f72 6368 6d65  es-Dist: torchme
+00000ad0: 7472 6963 733d 3d30 2e31 312e 303b 2065  trics==0.11.0; e
+00000ae0: 7874 7261 203d 3d20 2270 7974 6f72 6368  xtra == "pytorch
+00000af0: 2d63 7531 3231 220a 5265 7175 6972 6573  -cu121".Requires
+00000b00: 2d44 6973 743a 2074 696d 6d3e 3d30 2e39  -Dist: timm>=0.9
+00000b10: 2e31 303b 2065 7874 7261 203d 3d20 2270  .10; extra == "p
+00000b20: 7974 6f72 6368 2d63 7531 3231 220a 5072  ytorch-cu121".Pr
+00000b30: 6f76 6964 6573 2d45 7874 7261 3a20 7079  ovides-Extra: py
+00000b40: 746f 7263 682d 636f 6c61 620a 5265 7175  torch-colab.Requ
+00000b50: 6972 6573 2d44 6973 743a 206c 6967 6874  ires-Dist: light
+00000b60: 6e69 6e67 3e3d 322e 302e 303b 2065 7874  ning>=2.0.0; ext
+00000b70: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
+00000b80: 6f6c 6162 220a 5265 7175 6972 6573 2d44  olab".Requires-D
+00000b90: 6973 743a 2061 6c62 756d 656e 7461 7469  ist: albumentati
+00000ba0: 6f6e 733b 2065 7874 7261 203d 3d20 2270  ons; extra == "p
+00000bb0: 7974 6f72 6368 2d63 6f6c 6162 220a 5265  ytorch-colab".Re
+00000bc0: 7175 6972 6573 2d44 6973 743a 2070 7972  quires-Dist: pyr
+00000bd0: 6f2d 7070 6c3e 3d31 2e38 2e30 3b20 6578  o-ppl>=1.8.0; ex
+00000be0: 7472 6120 3d3d 2022 7079 746f 7263 682d  tra == "pytorch-
+00000bf0: 636f 6c61 6222 0a52 6571 7569 7265 732d  colab".Requires-
+00000c00: 4469 7374 3a20 746f 7263 686d 6574 7269  Dist: torchmetri
+00000c10: 6373 3d3d 302e 3131 2e30 3b20 6578 7472  cs==0.11.0; extr
+00000c20: 6120 3d3d 2022 7079 746f 7263 682d 636f  a == "pytorch-co
+00000c30: 6c61 6222 0a52 6571 7569 7265 732d 4469  lab".Requires-Di
+00000c40: 7374 3a20 7469 6d6d 3e3d 302e 392e 3130  st: timm>=0.9.10
+00000c50: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
+00000c60: 7263 682d 636f 6c61 6222 0a52 6571 7569  rch-colab".Requi
+00000c70: 7265 732d 4469 7374 3a20 6761 6c61 7879  res-Dist: galaxy
+00000c80: 5f64 6174 6173 6574 733d 3d30 2e30 2e31  _datasets==0.0.1
+00000c90: 373b 2065 7874 7261 203d 3d20 2270 7974  7; extra == "pyt
+00000ca0: 6f72 6368 2d63 6f6c 6162 220a 5072 6f76  orch-colab".Prov
+00000cb0: 6964 6573 2d45 7874 7261 3a20 7465 6e73  ides-Extra: tens
+00000cc0: 6f72 666c 6f77 0a52 6571 7569 7265 732d  orflow.Requires-
+00000cd0: 4469 7374 3a20 7465 6e73 6f72 666c 6f77  Dist: tensorflow
+00000ce0: 3d3d 322e 3130 2e30 3b20 6578 7472 6120  ==2.10.0; extra 
+00000cf0: 3d3d 2022 7465 6e73 6f72 666c 6f77 220a  == "tensorflow".
+00000d00: 5265 7175 6972 6573 2d44 6973 743a 206b  Requires-Dist: k
+00000d10: 6572 6173 5f61 7070 6c69 6361 7469 6f6e  eras_application
+00000d20: 733b 2065 7874 7261 203d 3d20 2274 656e  s; extra == "ten
+00000d30: 736f 7266 6c6f 7722 0a52 6571 7569 7265  sorflow".Require
+00000d40: 732d 4469 7374 3a20 7465 6e73 6f72 666c  s-Dist: tensorfl
+00000d50: 6f77 5f70 726f 6261 6269 6c69 7479 3d3d  ow_probability==
+00000d60: 302e 3138 2e30 3b20 6578 7472 6120 3d3d  0.18.0; extra ==
+00000d70: 2022 7465 6e73 6f72 666c 6f77 220a 5265   "tensorflow".Re
+00000d80: 7175 6972 6573 2d44 6973 743a 2070 726f  quires-Dist: pro
+00000d90: 746f 6275 663c 3d33 2e31 393b 2065 7874  tobuf<=3.19; ext
+00000da0: 7261 203d 3d20 2274 656e 736f 7266 6c6f  ra == "tensorflo
+00000db0: 7722 0a50 726f 7669 6465 732d 4578 7472  w".Provides-Extr
+00000dc0: 613a 2075 7469 6c69 7469 6573 0a52 6571  a: utilities.Req
+00000dd0: 7569 7265 732d 4469 7374 3a20 7365 6162  uires-Dist: seab
+00000de0: 6f72 6e3b 2065 7874 7261 203d 3d20 2275  orn; extra == "u
+00000df0: 7469 6c69 7469 6573 220a 5265 7175 6972  tilities".Requir
+00000e00: 6573 2d44 6973 743a 2062 6f74 6f33 3b20  es-Dist: boto3; 
+00000e10: 6578 7472 6120 3d3d 2022 7574 696c 6974  extra == "utilit
+00000e20: 6965 7322 0a52 6571 7569 7265 732d 4469  ies".Requires-Di
+00000e30: 7374 3a20 7079 7468 6f6e 2d64 6174 6575  st: python-dateu
+00000e40: 7469 6c3d 3d32 2e38 2e31 3b20 6578 7472  til==2.8.1; extr
+00000e50: 6120 3d3d 2022 7574 696c 6974 6965 7322  a == "utilities"
+00000e60: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000e70: 2064 6f63 730a 5265 7175 6972 6573 2d44   docs.Requires-D
+00000e80: 6973 743a 2053 7068 696e 783b 2065 7874  ist: Sphinx; ext
+00000e90: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
+00000ea0: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
+00000eb0: 6e78 636f 6e74 7269 622d 6e61 706f 6c65  nxcontrib-napole
+00000ec0: 6f6e 3b20 6578 7472 6120 3d3d 2022 646f  on; extra == "do
+00000ed0: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
+00000ee0: 743a 2066 7572 6f3b 2065 7874 7261 203d  t: furo; extra =
+00000ef0: 3d20 2264 6f63 7322 0a52 6571 7569 7265  = "docs".Require
+00000f00: 732d 4469 7374 3a20 646f 6375 7469 6c73  s-Dist: docutils
+00000f10: 3c30 2e31 383b 2065 7874 7261 203d 3d20  <0.18; extra == 
+00000f20: 2264 6f63 7322 0a52 6571 7569 7265 732d  "docs".Requires-
+00000f30: 4469 7374 3a20 7370 6869 6e78 656d 6f6a  Dist: sphinxemoj
+00000f40: 693b 2065 7874 7261 203d 3d20 2264 6f63  i; extra == "doc
+00000f50: 7322 0a0a 2320 5a6f 6f62 6f74 0a0a 5b21  s"..# Zoobot..[!
+00000f60: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
+00000f70: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
+00000f80: 6467 652f 7a6f 6f62 6f74 295d 2868 7474  dge/zoobot)](htt
+00000f90: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00000fa0: 726f 6a65 6374 2f7a 6f6f 626f 7429 0a5b  roject/zoobot).[
+00000fb0: 215b 446f 6375 6d65 6e74 6174 696f 6e20  ![Documentation 
+00000fc0: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
+00000fd0: 7265 6164 7468 6564 6f63 732e 6f72 672f  readthedocs.org/
+00000fe0: 7072 6f6a 6563 7473 2f7a 6f6f 626f 742f  projects/zoobot/
+00000ff0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00001000: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
+00001010: 7a6f 6f62 6f74 2e72 6561 6474 6865 646f  zoobot.readthedo
+00001020: 6373 2e69 6f2f 290a 215b 6275 696c 645d  cs.io/).![build]
+00001030: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001040: 636f 6d2f 6d77 616c 6d73 6c65 792f 7a6f  com/mwalmsley/zo
+00001050: 6f62 6f74 2f61 6374 696f 6e73 2f77 6f72  obot/actions/wor
+00001060: 6b66 6c6f 7773 2f72 756e 5f43 492e 796d  kflows/run_CI.ym
+00001070: 6c2f 6261 6467 652e 7376 6729 0a21 5b70  l/badge.svg).![p
+00001080: 7562 6c69 7368 5d28 6874 7470 733a 2f2f  ublish](https://
+00001090: 6769 7468 7562 2e63 6f6d 2f6d 7761 6c6d  github.com/mwalm
+000010a0: 736c 6579 2f7a 6f6f 626f 742f 6163 7469  sley/zoobot/acti
+000010b0: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+000010c0: 7468 6f6e 2d70 7562 6c69 7368 2e79 6d6c  thon-publish.yml
+000010d0: 2f62 6164 6765 2e73 7667 290a 5b21 5b50  /badge.svg).[![P
+000010e0: 7950 495d 2868 7474 7073 3a2f 2f62 6164  yPI](https://bad
+000010f0: 6765 2e66 7572 792e 696f 2f70 792f 7a6f  ge.fury.io/py/zo
+00001100: 6f62 6f74 2e73 7667 295d 2868 7474 7073  obot.svg)](https
+00001110: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+00001120: 2f70 792f 7a6f 6f62 6f74 290a 5b21 5b44  /py/zoobot).[![D
+00001130: 4f49 5d28 6874 7470 733a 2f2f 7a65 6e6f  OI](https://zeno
+00001140: 646f 2e6f 7267 2f62 6164 6765 2f33 3433  do.org/badge/343
+00001150: 3738 3736 3137 2e73 7667 295d 2868 7474  787617.svg)](htt
+00001160: 7073 3a2f 2f7a 656e 6f64 6f2e 6f72 672f  ps://zenodo.org/
+00001170: 6261 6467 652f 6c61 7465 7374 646f 692f  badge/latestdoi/
+00001180: 3334 3337 3837 3631 3729 0a5b 215b 7374  343787617).[![st
+00001190: 6174 7573 5d28 6874 7470 733a 2f2f 6a6f  atus](https://jo
+000011a0: 7373 2e74 6865 6f6a 2e6f 7267 2f70 6170  ss.theoj.org/pap
+000011b0: 6572 732f 3434 3735 3631 6565 3264 6534  ers/447561ee2de4
+000011c0: 3730 3965 6464 6237 3034 6531 3862 6565  709eddb704e18bee
+000011d0: 3834 3666 2f73 7461 7475 732e 7376 6729  846f/status.svg)
+000011e0: 5d28 6874 7470 733a 2f2f 6a6f 7373 2e74  ](https://joss.t
+000011f0: 6865 6f6a 2e6f 7267 2f70 6170 6572 732f  heoj.org/papers/
+00001200: 3434 3735 3631 6565 3264 6534 3730 3965  447561ee2de4709e
+00001210: 6464 6237 3034 6531 3862 6565 3834 3666  ddb704e18bee846f
+00001220: 290a 3c61 2068 7265 663d 2268 7474 7073  ).<a href="https
+00001230: 3a2f 2f61 7363 6c2e 6e65 742f 3232 3033  ://ascl.net/2203
+00001240: 2e30 3237 223e 3c69 6d67 2073 7263 3d22  .027"><img src="
+00001250: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00001260: 6c64 732e 696f 2f62 6164 6765 2f61 7363  lds.io/badge/asc
+00001270: 6c2d 3232 3033 2e30 3237 2d62 6c75 652e  l-2203.027-blue.
+00001280: 7376 673f 636f 6c6f 7242 3d32 3632 3235  svg?colorB=26225
+00001290: 3522 2061 6c74 3d22 6173 636c 3a32 3230  5" alt="ascl:220
+000012a0: 332e 3032 3722 202f 3e3c 2f61 3e0a 0a5a  3.027" /></a>..Z
+000012b0: 6f6f 626f 7420 636c 6173 7369 6669 6573  oobot classifies
+000012c0: 2067 616c 6178 7920 6d6f 7270 686f 6c6f   galaxy morpholo
+000012d0: 6779 2077 6974 6820 6465 6570 206c 6561  gy with deep lea
+000012e0: 726e 696e 672e 0a3c 212d 2d20 4174 2047  rning..<!-- At G
+000012f0: 616c 6178 7920 5a6f 6f2c 2077 6520 7573  alaxy Zoo, we us
+00001300: 6520 5a6f 6f62 6f74 2074 6f20 6865 6c70  e Zoobot to help
+00001310: 206f 7572 2076 6f6c 756e 7465 6572 7320   our volunteers 
+00001320: 636c 6173 7369 6679 2074 6865 2067 616c  classify the gal
+00001330: 6178 6965 7320 696e 2061 6c6c 206f 7572  axies in all our
+00001340: 2072 6563 656e 7420 6361 7461 6c6f 6775   recent catalogu
+00001350: 6573 3a20 475a 2044 4543 614c 532c 2047  es: GZ DECaLS, G
+00001360: 5a20 4445 5349 2c20 475a 2052 696e 6773  Z DESI, GZ Rings
+00001370: 2061 6e64 2047 5a20 436f 736d 6963 2044   and GZ Cosmic D
+00001380: 6177 6e2e 202d 2d3e 0a0a 5a6f 6f62 6f74  awn. -->..Zoobot
+00001390: 2069 7320 7472 6169 6e65 6420 7573 696e   is trained usin
+000013a0: 6720 6d69 6c6c 696f 6e73 206f 6620 616e  g millions of an
+000013b0: 7377 6572 7320 6279 2047 616c 6178 7920  swers by Galaxy 
+000013c0: 5a6f 6f20 766f 6c75 6e74 6565 7273 2e20  Zoo volunteers. 
+000013d0: 5468 6973 2063 6f64 6520 7769 6c6c 206c  This code will l
+000013e0: 6574 2079 6f75 202a 2a72 6574 7261 696e  et you **retrain
+000013f0: 2a2a 205a 6f6f 626f 7420 746f 2061 6363  ** Zoobot to acc
+00001400: 7572 6174 656c 7920 736f 6c76 6520 796f  urately solve yo
+00001410: 7572 206f 776e 2070 7265 6469 6374 696f  ur own predictio
+00001420: 6e20 7461 736b 2e0a 0a2d 205b 496e 7374  n task...- [Inst
+00001430: 616c 6c5d 2823 696e 7374 616c 6c61 7469  all](#installati
+00001440: 6f6e 290a 2d20 5b51 7569 636b 7374 6172  on).- [Quickstar
+00001450: 745d 2823 7175 6963 6b73 7461 7274 290a  t](#quickstart).
+00001460: 2d20 5b57 6f72 6b65 6420 4578 616d 706c  - [Worked Exampl
+00001470: 6573 5d28 2377 6f72 6b65 642d 6578 616d  es](#worked-exam
+00001480: 706c 6573 290a 2d20 5b50 7265 7472 6169  ples).- [Pretrai
+00001490: 6e65 6420 5765 6967 6874 735d 2868 7474  ned Weights](htt
+000014a0: 7073 3a2f 2f7a 6f6f 626f 742e 7265 6164  ps://zoobot.read
+000014b0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000014c0: 7465 7374 2f70 7265 7472 6169 6e65 645f  test/pretrained_
+000014d0: 6d6f 6465 6c73 2e68 746d 6c29 0a2d 205b  models.html).- [
+000014e0: 4461 7461 7365 7473 5d28 6874 7470 733a  Datasets](https:
+000014f0: 2f2f 7777 772e 6769 7468 7562 2e63 6f6d  //www.github.com
+00001500: 2f6d 7761 6c6d 736c 6579 2f67 616c 6178  /mwalmsley/galax
+00001510: 792d 6461 7461 7365 7473 290a 2d20 5b44  y-datasets).- [D
+00001520: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00001530: 7470 733a 2f2f 7a6f 6f62 6f74 2e72 6561  tps://zoobot.rea
+00001540: 6474 6865 646f 6373 2e69 6f2f 2920 2866  dthedocs.io/) (f
+00001550: 6f72 2075 6e64 6572 7374 616e 6469 6e67  or understanding
+00001560: 2f72 6566 6572 656e 6365 290a 0a23 2320  /reference)..## 
+00001570: 496e 7374 616c 6c61 7469 6f6e 0a0a 3c61  Installation..<a
+00001580: 206e 616d 653d 2269 6e73 7461 6c6c 6174   name="installat
+00001590: 696f 6e22 3e3c 2f61 3e0a 0a59 6f75 2063  ion"></a>..You c
+000015a0: 616e 2072 6574 7261 696e 205a 6f6f 626f  an retrain Zoobo
+000015b0: 7420 696e 2074 6865 2063 6c6f 7564 2077  t in the cloud w
+000015c0: 6974 6820 6120 6672 6565 2047 5055 2075  ith a free GPU u
+000015d0: 7369 6e67 2074 6869 7320 5b47 6f6f 676c  sing this [Googl
+000015e0: 6520 436f 6c61 6220 6e6f 7465 626f 6f6b  e Colab notebook
+000015f0: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+00001600: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00001610: 636f 6d2f 6472 6976 652f 3141 5f2d 4d33  com/drive/1A_-M3
+00001620: 537a 356d 6151 6d79 6657 3241 3772 4575  Sz5maQmyfW2A7rEu
+00001630: 2d67 5f5a 6930 524d 477a 353f 7573 703d  -g_Zi0RMGz5?usp=
+00001640: 7368 6172 696e 6729 2e20 546f 2069 6e73  sharing). To ins
+00001650: 7461 6c6c 206c 6f63 616c 6c79 2c20 6b65  tall locally, ke
+00001660: 6570 2072 6561 6469 6e67 2e0a 0a44 6f77  ep reading...Dow
+00001670: 6e6c 6f61 6420 7468 6520 636f 6465 2075  nload the code u
+00001680: 7369 6e67 2067 6974 3a0a 0a20 2020 2067  sing git:..    g
+00001690: 6974 2063 6c6f 6e65 2067 6974 4067 6974  it clone git@git
+000016a0: 6875 622e 636f 6d3a 6d77 616c 6d73 6c65  hub.com:mwalmsle
+000016b0: 792f 7a6f 6f62 6f74 2e67 6974 0a0a 416e  y/zoobot.git..An
+000016c0: 6420 7468 656e 2070 6963 6b20 6f6e 6520  d then pick one 
+000016d0: 6f66 2074 6865 2074 6872 6565 2063 6f6d  of the three com
+000016e0: 6d61 6e64 7320 6265 6c6f 7720 746f 2069  mands below to i
+000016f0: 6e73 7461 6c6c 205a 6f6f 626f 7420 616e  nstall Zoobot an
+00001700: 6420 5079 546f 7263 683a 0a0a 2020 2020  d PyTorch:..    
+00001710: 2320 5a6f 6f62 6f74 2077 6974 6820 5079  # Zoobot with Py
+00001720: 546f 7263 6820 616e 6420 6120 4750 552e  Torch and a GPU.
+00001730: 2052 6571 7569 7265 7320 4355 4441 2031   Requires CUDA 1
+00001740: 322e 3120 286f 7220 4355 4441 2031 312e  2.1 (or CUDA 11.
+00001750: 382c 2069 6620 796f 7520 7573 6520 605f  8, if you use `_
+00001760: 6375 3131 3860 2069 6e73 7465 6164 290a  cu118` instead).
+00001770: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
+00001780: 2d65 2022 7a6f 6f62 6f74 5b70 7974 6f72  -e "zoobot[pytor
+00001790: 6368 2d63 7531 3231 5d22 202d 2d65 7874  ch-cu121]" --ext
+000017a0: 7261 2d69 6e64 6578 2d75 726c 2068 7474  ra-index-url htt
+000017b0: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
+000017c0: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
+000017d0: 3132 310a 0a20 2020 2023 204f 5220 5a6f  121..    # OR Zo
+000017e0: 6f62 6f74 2077 6974 6820 5079 546f 7263  obot with PyTorc
+000017f0: 6820 616e 6420 6e6f 2047 5055 0a20 2020  h and no GPU.   
+00001800: 2070 6970 2069 6e73 7461 6c6c 202d 6520   pip install -e 
+00001810: 227a 6f6f 626f 745b 7079 746f 7263 682d  "zoobot[pytorch-
+00001820: 6370 755d 2220 2d2d 6578 7472 612d 696e  cpu]" --extra-in
+00001830: 6465 782d 7572 6c20 6874 7470 733a 2f2f  dex-url https://
+00001840: 646f 776e 6c6f 6164 2e70 7974 6f72 6368  download.pytorch
+00001850: 2e6f 7267 2f77 686c 2f63 7075 0a0a 2020  .org/whl/cpu..  
+00001860: 2020 2320 4f52 205a 6f6f 626f 7420 7769    # OR Zoobot wi
+00001870: 7468 2050 7954 6f72 6368 206f 6e20 4d61  th PyTorch on Ma
+00001880: 6320 7769 7468 204d 3120 6368 6970 0a20  c with M1 chip. 
+00001890: 2020 2070 6970 2069 6e73 7461 6c6c 202d     pip install -
+000018a0: 6520 227a 6f6f 626f 745b 7079 746f 7263  e "zoobot[pytorc
+000018b0: 682d 6d31 5d22 0a0a 5468 6973 2069 6e73  h-m1]"..This ins
+000018c0: 7461 6c6c 7320 7468 6520 646f 776e 6c6f  talls the downlo
+000018d0: 6164 6564 205a 6f6f 626f 7420 636f 6465  aded Zoobot code
+000018e0: 2075 7369 6e67 2070 6970 205b 6564 6974   using pip [edit
+000018f0: 6162 6c65 206d 6f64 655d 2868 7474 7073  able mode](https
+00001900: 3a2f 2f70 6970 2e70 7970 612e 696f 2f65  ://pip.pypa.io/e
+00001910: 6e2f 7374 6162 6c65 2f74 6f70 6963 732f  n/stable/topics/
+00001920: 6c6f 6361 6c2d 7072 6f6a 6563 742d 696e  local-project-in
+00001930: 7374 616c 6c73 2f23 6564 6974 6162 6c65  stalls/#editable
+00001940: 2d69 6e73 7461 6c6c 7329 2073 6f20 796f  -installs) so yo
+00001950: 7520 6361 6e20 6561 7369 6c79 2063 6861  u can easily cha
+00001960: 6e67 6520 7468 6520 636f 6465 206c 6f63  nge the code loc
+00001970: 616c 6c79 2e20 5a6f 6f62 6f74 2069 7320  ally. Zoobot is 
+00001980: 616c 736f 2061 7661 696c 6162 6c65 2064  also available d
+00001990: 6972 6563 746c 7920 6672 6f6d 2070 6970  irectly from pip
+000019a0: 2028 6070 6970 2069 6e73 7461 6c6c 207a   (`pip install z
+000019b0: 6f6f 626f 745b 6f70 7469 6f6e 5d60 292e  oobot[option]`).
+000019c0: 204f 6e6c 7920 7573 6520 7468 6973 2069   Only use this i
+000019d0: 6620 796f 7520 6172 6520 7375 7265 2079  f you are sure y
+000019e0: 6f75 2077 6f6e 2774 2062 6520 6d61 6b69  ou won't be maki
+000019f0: 6e67 2063 6861 6e67 6573 2074 6f20 5a6f  ng changes to Zo
+00001a00: 6f62 6f74 2069 7473 656c 662e 2046 6f72  obot itself. For
+00001a10: 2047 6f6f 676c 6520 436f 6c61 622c 2075   Google Colab, u
+00001a20: 7365 2060 7069 7020 696e 7374 616c 6c20  se `pip install 
+00001a30: 7a6f 6f62 6f74 5b70 7974 6f72 6368 5f63  zoobot[pytorch_c
+00001a40: 6f6c 6162 5d60 0a0a 546f 2075 7365 2061  olab]`..To use a
+00001a50: 2047 5055 2c20 796f 7520 6d75 7374 202a   GPU, you must *
+00001a60: 616c 7265 6164 792a 2068 6176 6520 4355  already* have CU
+00001a70: 4441 2069 6e73 7461 6c6c 6564 2061 6e64  DA installed and
+00001a80: 206d 6174 6368 696e 6720 7468 6520 7665   matching the ve
+00001a90: 7273 696f 6e73 2061 626f 7665 2e0a 4920  rsions above..I 
+00001aa0: 7368 6172 6520 6d79 2069 6e73 7461 6c6c  share my install
+00001ab0: 2073 7465 7073 205b 6865 7265 5d28 2369   steps [here](#i
+00001ac0: 6e73 7461 6c6c 5f63 7564 6129 2e20 4750  nstall_cuda). GP
+00001ad0: 5573 2061 7265 206f 7074 696f 6e61 6c20  Us are optional 
+00001ae0: 2d20 5a6f 6f62 6f74 2077 696c 6c20 7275  - Zoobot will ru
+00001af0: 6e20 7265 7472 6169 6e20 6669 6e65 206f  n retrain fine o
+00001b00: 6e20 4350 552c 206a 7573 7420 736c 6f77  n CPU, just slow
+00001b10: 6572 2e0a 0a23 2320 5175 6963 6b73 7461  er...## Quicksta
+00001b20: 7274 0a0a 3c61 206e 616d 653d 2271 7569  rt..<a name="qui
+00001b30: 636b 7374 6172 7422 3e3c 2f61 3e0a 0a54  ckstart"></a>..T
+00001b40: 6865 205b 436f 6c61 6220 6e6f 7465 626f  he [Colab notebo
+00001b50: 6f6b 5d28 6874 7470 733a 2f2f 636f 6c61  ok](https://cola
+00001b60: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00001b70: 652e 636f 6d2f 6472 6976 652f 3141 5f2d  e.com/drive/1A_-
+00001b80: 4d33 537a 356d 6151 6d79 6657 3241 3772  M3Sz5maQmyfW2A7r
+00001b90: 4575 2d67 5f5a 6930 524d 477a 353f 7573  Eu-g_Zi0RMGz5?us
+00001ba0: 703d 7368 6172 696e 6729 2069 7320 7468  p=sharing) is th
+00001bb0: 6520 7175 6963 6b65 7374 2077 6179 2074  e quickest way t
+00001bc0: 6f20 6765 7420 7374 6172 7465 642e 2041  o get started. A
+00001bd0: 6c74 6572 6e61 7469 7665 6c79 2c20 7468  lternatively, th
+00001be0: 6520 6d69 6e69 6d61 6c20 6578 616d 706c  e minimal exampl
+00001bf0: 6520 6265 6c6f 7720 696c 6c75 7374 7261  e below illustra
+00001c00: 7465 7320 686f 7720 5a6f 6f62 6f74 2077  tes how Zoobot w
+00001c10: 6f72 6b73 2e0a 0a4c 6574 2773 2073 6179  orks...Let's say
+00001c20: 2079 6f75 2077 616e 7420 746f 2066 696e   you want to fin
+00001c30: 6420 7269 6e67 6564 2067 616c 6178 6965  d ringed galaxie
+00001c40: 7320 616e 6420 796f 7520 6861 7665 2061  s and you have a
+00001c50: 2073 6d61 6c6c 206c 6162 656c 6c65 6420   small labelled 
+00001c60: 6461 7461 7365 7420 6f66 2035 3030 2072  dataset of 500 r
+00001c70: 696e 6765 6420 6f72 206e 6f74 2d72 696e  inged or not-rin
+00001c80: 6765 6420 6761 6c61 7869 6573 2e20 596f  ged galaxies. Yo
+00001c90: 7520 6361 6e20 7265 7472 6169 6e20 5a6f  u can retrain Zo
+00001ca0: 6f62 6f74 2074 6f20 6669 6e64 2072 696e  obot to find rin
+00001cb0: 6773 206c 696b 6520 736f 3a0a 0a20 2020  gs like so:..   
+00001cc0: 2060 6060 7079 7468 6f6e 0a0a 2020 2020   ```python..    
+00001cd0: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
+00001ce0: 2070 640a 2020 2020 6672 6f6d 2067 616c   pd.    from gal
+00001cf0: 6178 795f 6461 7461 7365 7473 2e70 7974  axy_datasets.pyt
+00001d00: 6f72 6368 2e67 616c 6178 795f 6461 7461  orch.galaxy_data
+00001d10: 6d6f 6475 6c65 2069 6d70 6f72 7420 4761  module import Ga
+00001d20: 6c61 7879 4461 7461 4d6f 6475 6c65 0a20  laxyDataModule. 
+00001d30: 2020 2066 726f 6d20 7a6f 6f62 6f74 2e70     from zoobot.p
+00001d40: 7974 6f72 6368 2e74 7261 696e 696e 6720  ytorch.training 
+00001d50: 696d 706f 7274 2066 696e 6574 756e 650a  import finetune.
+00001d60: 0a20 2020 2023 2063 7376 2077 6974 6820  .    # csv with 
+00001d70: 2772 696e 6727 2063 6f6c 756d 6e20 2830  'ring' column (0
+00001d80: 206f 7220 3129 2061 6e64 2027 6669 6c65   or 1) and 'file
+00001d90: 5f6c 6f63 2720 636f 6c75 6d6e 2028 7061  _loc' column (pa
+00001da0: 7468 2074 6f20 696d 6167 6529 0a20 2020  th to image).   
+00001db0: 206c 6162 656c 6c65 645f 6466 203d 2070   labelled_df = p
+00001dc0: 642e 7265 6164 5f63 7376 2827 2f79 6f75  d.read_csv('/you
+00001dd0: 722f 7061 7468 2f73 6f6d 655f 6c61 6265  r/path/some_labe
+00001de0: 6c6c 6564 5f67 616c 6178 6965 732e 6373  lled_galaxies.cs
+00001df0: 7627 290a 0a20 2020 2064 6174 616d 6f64  v')..    datamod
+00001e00: 756c 6520 3d20 4761 6c61 7879 4461 7461  ule = GalaxyData
+00001e10: 4d6f 6475 6c65 280a 2020 2020 2020 6c61  Module(.      la
+00001e20: 6265 6c5f 636f 6c73 3d5b 2772 696e 6727  bel_cols=['ring'
+00001e30: 5d2c 0a20 2020 2020 2063 6174 616c 6f67  ],.      catalog
+00001e40: 3d6c 6162 656c 6c65 645f 6466 2c0a 2020  =labelled_df,.  
+00001e50: 2020 2020 6261 7463 685f 7369 7a65 3d33      batch_size=3
+00001e60: 320a 2020 2020 290a 0a20 2020 2023 206c  2.    )..    # l
+00001e70: 6f61 6420 7472 6169 6e65 6420 5a6f 6f62  oad trained Zoob
+00001e80: 6f74 206d 6f64 656c 0a20 2020 206d 6f64  ot model.    mod
+00001e90: 656c 203d 2066 696e 6574 756e 652e 4669  el = finetune.Fi
+00001ea0: 6e65 7475 6e65 6162 6c65 5a6f 6f62 6f74  netuneableZoobot
+00001eb0: 436c 6173 7369 6669 6572 2863 6865 636b  Classifier(check
+00001ec0: 706f 696e 745f 6c6f 632c 206e 756d 5f63  point_loc, num_c
+00001ed0: 6c61 7373 6573 3d32 2920 200a 2020 2020  lasses=2)  .    
+00001ee0: 0a20 2020 2023 2072 6574 7261 696e 2074  .    # retrain t
+00001ef0: 6f20 6669 6e64 2072 696e 6773 0a20 2020  o find rings.   
+00001f00: 2074 7261 696e 6572 203d 2066 696e 6574   trainer = finet
+00001f10: 756e 652e 6765 745f 7472 6169 6e65 7228  une.get_trainer(
+00001f20: 7361 7665 5f64 6972 290a 2020 2020 7472  save_dir).    tr
+00001f30: 6169 6e65 722e 6669 7428 6d6f 6465 6c2c  ainer.fit(model,
+00001f40: 2064 6174 616d 6f64 756c 6529 0a20 2020   datamodule).   
+00001f50: 2060 6060 0a0a 5468 656e 2079 6f75 2063   ```..Then you c
+00001f60: 616e 206d 616b 6520 7072 6564 6963 7420  an make predict 
+00001f70: 6966 206e 6577 2067 616c 6178 6965 7320  if new galaxies 
+00001f80: 6861 7665 2072 696e 6773 3a0a 0a20 2020  have rings:..   
+00001f90: 2060 6060 7079 7468 6f6e 0a20 2020 2066   ```python.    f
+00001fa0: 726f 6d20 7a6f 6f62 6f74 2e70 7974 6f72  rom zoobot.pytor
+00001fb0: 6368 2e70 7265 6469 6374 696f 6e73 2069  ch.predictions i
+00001fc0: 6d70 6f72 7420 7072 6564 6963 745f 6f6e  mport predict_on
+00001fd0: 5f63 6174 616c 6f67 0a0a 2020 2020 2320  _catalog..    # 
+00001fe0: 6373 7620 7769 7468 2027 6669 6c65 5f6c  csv with 'file_l
+00001ff0: 6f63 2720 636f 6c75 6d6e 2028 7061 7468  oc' column (path
+00002000: 2074 6f20 696d 6167 6529 2e20 5a6f 6f62   to image). Zoob
+00002010: 6f74 2077 696c 6c20 7072 6564 6963 7420  ot will predict 
+00002020: 7468 6520 6c61 6265 6c73 2e0a 2020 2020  the labels..    
+00002030: 756e 6c61 6265 6c6c 6564 5f64 6620 3d20  unlabelled_df = 
+00002040: 7064 2e72 6561 645f 6373 7628 272f 796f  pd.read_csv('/yo
+00002050: 7572 2f70 6174 682f 736f 6d65 5f75 6e6c  ur/path/some_unl
+00002060: 6162 656c 6c65 645f 6761 6c61 7869 6573  abelled_galaxies
+00002070: 2e63 7376 2729 0a0a 2020 2020 7072 6564  .csv')..    pred
+00002080: 6963 745f 6f6e 5f63 6174 616c 6f67 2e70  ict_on_catalog.p
+00002090: 7265 6469 6374 280a 2020 2020 2020 756e  redict(.      un
+000020a0: 6c61 6265 6c6c 6564 5f64 662c 0a20 2020  labelled_df,.   
+000020b0: 2020 206d 6f64 656c 2c0a 2020 2020 2020     model,.      
+000020c0: 6c61 6265 6c5f 636f 6c73 3d5b 2772 696e  label_cols=['rin
+000020d0: 6727 5d2c 2020 2320 6f6e 6c79 2075 7365  g'],  # only use
+000020e0: 6420 666f 7220 0a20 2020 2020 2073 6176  d for .      sav
+000020f0: 655f 6c6f 633d 272f 796f 7572 2f70 6174  e_loc='/your/pat
+00002100: 682f 6669 6e65 7475 6e65 645f 7072 6564  h/finetuned_pred
+00002110: 6963 7469 6f6e 732e 6373 7627 0a20 2020  ictions.csv'.   
+00002120: 2029 0a20 2020 2060 6060 0a0a 5a6f 6f62   ).    ```..Zoob
+00002130: 6f74 2069 6e63 6c75 6465 7320 6d61 6e79  ot includes many
+00002140: 2067 7569 6465 7320 616e 6420 776f 726b   guides and work
+00002150: 696e 6720 6578 616d 706c 6573 202d 2073  ing examples - s
+00002160: 6565 2074 6865 205b 4765 7474 696e 6720  ee the [Getting 
+00002170: 5374 6172 7465 645d 2823 6765 7474 696e  Started](#gettin
+00002180: 672d 7374 6172 7465 6429 2073 6563 7469  g-started) secti
+00002190: 6f6e 2062 656c 6f77 2e0a 0a23 2320 4765  on below...## Ge
+000021a0: 7474 696e 6720 5374 6172 7465 640a 0a3c  tting Started..<
+000021b0: 6120 6e61 6d65 3d22 6765 7474 696e 675f  a name="getting_
+000021c0: 7374 6172 7465 6422 3e3c 2f61 3e0a 0a49  started"></a>..I
+000021d0: 2073 7567 6765 7374 2073 7461 7274 696e   suggest startin
+000021e0: 6720 7769 7468 2074 6865 205b 436f 6c61  g with the [Cola
+000021f0: 6220 6e6f 7465 626f 6f6b 5d28 6874 7470  b notebook](http
+00002200: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00002210: 6368 2e67 6f6f 676c 652e 636f 6d2f 6472  ch.google.com/dr
+00002220: 6976 652f 3141 5f2d 4d33 537a 356d 6151  ive/1A_-M3Sz5maQ
+00002230: 6d79 6657 3241 3772 4575 2d67 5f5a 6930  myfW2A7rEu-g_Zi0
+00002240: 524d 477a 353f 7573 703d 7368 6172 696e  RMGz5?usp=sharin
+00002250: 6729 206f 7220 7468 6520 776f 726b 6564  g) or the worked
+00002260: 2065 7861 6d70 6c65 7320 6265 6c6f 772c   examples below,
+00002270: 2077 6869 6368 2079 6f75 2063 616e 2063   which you can c
+00002280: 6f70 7920 616e 6420 6164 6170 742e 0a0a  opy and adapt...
+00002290: 466f 7220 636f 6e74 6578 7420 616e 6420  For context and 
+000022a0: 6578 706c 616e 6174 696f 6e2c 2073 6565  explanation, see
+000022b0: 2074 6865 205b 646f 6375 6d65 6e74 6174   the [documentat
+000022c0: 696f 6e5d 2868 7474 7073 3a2f 2f7a 6f6f  ion](https://zoo
+000022d0: 626f 742e 7265 6164 7468 6564 6f63 732e  bot.readthedocs.
+000022e0: 696f 2f29 2e0a 0a50 7265 7472 6169 6e65  io/)...Pretraine
+000022f0: 6420 6d6f 6465 6c73 2061 7265 206c 6973  d models are lis
+00002300: 7465 6420 5b68 6572 655d 2868 7474 7073  ted [here](https
+00002310: 3a2f 2f7a 6f6f 626f 742e 7265 6164 7468  ://zoobot.readth
+00002320: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00002330: 7374 2f70 7265 7472 6169 6e65 645f 6d6f  st/pretrained_mo
+00002340: 6465 6c73 2e68 746d 6c29 2061 6e64 2061  dels.html) and a
+00002350: 7661 696c 6162 6c65 206f 6e20 5b48 7567  vailable on [Hug
+00002360: 6769 6e67 4661 6365 5d28 6874 7470 733a  gingFace](https:
+00002370: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00002380: 2f63 6f6c 6c65 6374 696f 6e73 2f6d 7761  /collections/mwa
+00002390: 6c6d 736c 6579 2f7a 6f6f 626f 742d 656e  lmsley/zoobot-en
+000023a0: 636f 6465 7273 2d36 3566 6131 3461 6539  coders-65fa14ae9
+000023b0: 3239 3131 6231 3733 3731 3262 3837 3429  2911b173712b874)
+000023c0: 0a0a 2323 2320 576f 726b 6564 2045 7861  ..### Worked Exa
+000023d0: 6d70 6c65 730a 0a3c 6120 6e61 6d65 3d22  mples..<a name="
+000023e0: 776f 726b 6564 5f65 7861 6d70 6c65 7322  worked_examples"
+000023f0: 3e3c 2f61 3e0a 0a50 7954 6f72 6368 2028  ></a>..PyTorch (
+00002400: 7265 636f 6d6d 656e 6465 6429 3a0a 0a2d  recommended):..-
+00002410: 205b 7079 746f 7263 682f 6578 616d 706c   [pytorch/exampl
+00002420: 6573 2f66 696e 6574 756e 696e 672f 6669  es/finetuning/fi
+00002430: 6e65 7475 6e65 5f62 696e 6172 795f 636c  netune_binary_cl
+00002440: 6173 7369 6669 6361 7469 6f6e 2e70 795d  assification.py]
+00002450: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002460: 636f 6d2f 6d77 616c 6d73 6c65 792f 7a6f  com/mwalmsley/zo
+00002470: 6f62 6f74 2f62 6c6f 622f 6d61 696e 2f7a  obot/blob/main/z
+00002480: 6f6f 626f 742f 7079 746f 7263 682f 6578  oobot/pytorch/ex
+00002490: 616d 706c 6573 2f66 696e 6574 756e 696e  amples/finetunin
+000024a0: 672f 6669 6e65 7475 6e65 5f62 696e 6172  g/finetune_binar
+000024b0: 795f 636c 6173 7369 6669 6361 7469 6f6e  y_classification
+000024c0: 2e70 7929 0a2d 205b 7079 746f 7263 682f  .py).- [pytorch/
+000024d0: 6578 616d 706c 6573 2f66 696e 6574 756e  examples/finetun
+000024e0: 696e 672f 6669 6e65 7475 6e65 5f63 6f75  ing/finetune_cou
+000024f0: 6e74 735f 6675 6c6c 5f74 7265 652e 7079  nts_full_tree.py
+00002500: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002510: 2e63 6f6d 2f6d 7761 6c6d 736c 6579 2f7a  .com/mwalmsley/z
+00002520: 6f6f 626f 742f 626c 6f62 2f6d 6169 6e2f  oobot/blob/main/
+00002530: 7a6f 6f62 6f74 2f70 7974 6f72 6368 2f65  zoobot/pytorch/e
+00002540: 7861 6d70 6c65 732f 6669 6e65 7475 6e69  xamples/finetuni
+00002550: 6e67 2f66 696e 6574 756e 655f 636f 756e  ng/finetune_coun
+00002560: 7473 5f66 756c 6c5f 7472 6565 2e70 7929  ts_full_tree.py)
+00002570: 0a2d 205b 7079 746f 7263 682f 6578 616d  .- [pytorch/exam
+00002580: 706c 6573 2f72 6570 7265 7365 6e74 6174  ples/representat
+00002590: 696f 6e73 2f67 6574 5f72 6570 7265 7365  ions/get_represe
+000025a0: 6e74 6174 696f 6e73 2e70 795d 2868 7474  ntations.py](htt
+000025b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000025c0: 6d77 616c 6d73 6c65 792f 7a6f 6f62 6f74  mwalmsley/zoobot
+000025d0: 2f62 6c6f 622f 6d61 696e 2f7a 6f6f 626f  /blob/main/zoobo
+000025e0: 742f 7079 746f 7263 682f 6578 616d 706c  t/pytorch/exampl
+000025f0: 6573 2f72 6570 7265 7365 6e74 6174 696f  es/representatio
+00002600: 6e73 2f67 6574 5f72 6570 7265 7365 6e74  ns/get_represent
+00002610: 6174 696f 6e73 2e70 7929 0a2d 205b 7079  ations.py).- [py
+00002620: 746f 7263 682f 6578 616d 706c 6573 2f74  torch/examples/t
+00002630: 7261 696e 5f6d 6f64 656c 5f6f 6e5f 6361  rain_model_on_ca
+00002640: 7461 6c6f 672e 7079 5d28 6874 7470 733a  talog.py](https:
+00002650: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 7761  //github.com/mwa
+00002660: 6c6d 736c 6579 2f7a 6f6f 626f 742f 626c  lmsley/zoobot/bl
+00002670: 6f62 2f6d 6169 6e2f 7a6f 6f62 6f74 2f70  ob/main/zoobot/p
+00002680: 7974 6f72 6368 2f65 7861 6d70 6c65 732f  ytorch/examples/
+00002690: 7472 6169 6e5f 6d6f 6465 6c5f 6f6e 5f63  train_model_on_c
+000026a0: 6174 616c 6f67 2e70 7929 2028 6f6e 6c79  atalog.py) (only
+000026b0: 206e 6563 6573 7361 7279 2074 6f20 7472   necessary to tr
+000026c0: 6169 6e20 6672 6f6d 2073 6372 6174 6368  ain from scratch
+000026d0: 290a 0a54 6865 7265 2069 7320 6d6f 7265  )..There is more
+000026e0: 2065 7870 6c61 6e61 7469 6f6e 2061 6e64   explanation and
+000026f0: 2061 6e20 4150 4920 7265 6665 7265 6e63   an API referenc
+00002700: 6520 6f6e 2074 6865 205b 646f 6373 5d28  e on the [docs](
+00002710: 6874 7470 733a 2f2f 7a6f 6f62 6f74 2e72  https://zoobot.r
+00002720: 6561 6474 6865 646f 6373 2e69 6f2f 292e  eadthedocs.io/).
+00002730: 0a0a 4920 616c 736f 205b 696e 636c 7564  ..I also [includ
+00002740: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00002750: 622e 636f 6d2f 6d77 616c 6d73 6c65 792f  b.com/mwalmsley/
+00002760: 7a6f 6f62 6f74 2f62 6c6f 622f 6d61 696e  zoobot/blob/main
+00002770: 2f62 656e 6368 6d61 726b 7329 2074 6865  /benchmarks) the
+00002780: 2073 6372 6970 7473 2075 7365 6420 746f   scripts used to
+00002790: 2063 7265 6174 6520 616e 6420 6265 6e63   create and benc
+000027a0: 686d 6172 6b20 6f75 7220 7072 6574 7261  hmark our pretra
+000027b0: 696e 6564 206d 6f64 656c 732e 204d 616e  ined models. Man
+000027c0: 7920 7072 6574 7261 696e 6564 206d 6f64  y pretrained mod
+000027d0: 656c 7320 6172 6520 6176 6169 6c61 626c  els are availabl
+000027e0: 6520 5b61 6c72 6561 6479 5d28 6874 7470  e [already](http
+000027f0: 733a 2f2f 7a6f 6f62 6f74 2e72 6561 6474  s://zoobot.readt
+00002800: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00002810: 6573 742f 6461 7461 5f6e 6f74 6573 2e68  est/data_notes.h
+00002820: 746d 6c29 2c20 6275 7420 6966 2079 6f75  tml), but if you
+00002830: 206e 6565 6420 6f6e 6520 7472 6169 6e65   need one traine
+00002840: 6420 6f6e 2065 2e67 2e20 6469 6666 6572  d on e.g. differ
+00002850: 656e 7420 696e 7075 7420 696d 6167 6520  ent input image 
+00002860: 7369 7a65 7320 6f72 2077 6974 6820 6120  sizes or with a 
+00002870: 7370 6563 6966 6963 2061 7263 6869 7465  specific archite
+00002880: 6374 7572 652c 2049 2063 616e 2070 726f  cture, I can pro
+00002890: 6261 626c 7920 6d61 6b65 2069 7420 666f  bably make it fo
+000028a0: 7220 796f 752e 0a0a 5768 656e 2074 7261  r you...When tra
+000028b0: 696e 6564 2077 6974 6820 6120 6465 6369  ined with a deci
+000028c0: 7369 6f6e 2074 7265 6520 6865 6164 2028  sion tree head (
+000028d0: 5a6f 6f62 6f74 5472 6565 2c20 4669 6e65  ZoobotTree, Fine
+000028e0: 7475 6e65 6162 6c65 5a6f 6f62 6f74 5472  tuneableZoobotTr
+000028f0: 6565 292c 205a 6f6f 626f 7420 6361 6e20  ee), Zoobot can 
+00002900: 6c65 6172 6e20 6672 6f6d 2076 6f6c 756e  learn from volun
+00002910: 7465 6572 206c 6162 656c 7320 6f66 2076  teer labels of v
+00002920: 6172 7969 6e67 2063 6f6e 6669 6465 6e63  arying confidenc
+00002930: 6520 616e 6420 7072 6564 6963 7420 706f  e and predict po
+00002940: 7374 6572 696f 7273 2066 6f72 2077 6861  steriors for wha
+00002950: 7420 7468 6520 7479 7069 6361 6c20 766f  t the typical vo
+00002960: 6c75 6e74 6565 7220 6d69 6768 7420 7361  lunteer might sa
+00002970: 792e 2053 7065 6369 6669 6361 6c6c 792c  y. Specifically,
+00002980: 2074 6869 7320 5a6f 6f62 6f74 206d 6f64   this Zoobot mod
+00002990: 6520 7072 6564 6963 7473 2074 6865 2070  e predicts the p
+000029a0: 6172 616d 6574 6572 7320 666f 7220 6469  arameters for di
+000029b0: 7374 7269 6275 7469 6f6e 732c 206e 6f74  stributions, not
+000029c0: 2073 696d 706c 6520 636c 6173 7320 6c61   simple class la
+000029d0: 6265 6c73 2120 466f 7220 6120 6465 6d6f  bels! For a demo
+000029e0: 6e73 7472 6174 696f 6e20 6f66 2068 6f77  nstration of how
+000029f0: 2074 6f20 696e 7465 7270 7265 7420 7468   to interpret th
+00002a00: 6573 6520 7072 6564 6963 7469 6f6e 732c  ese predictions,
+00002a10: 2073 6565 2074 6865 205b 677a 5f64 6563   see the [gz_dec
+00002a20: 616c 735f 6461 7461 5f72 656c 6561 7365  als_data_release
+00002a30: 5f61 6e61 6c79 7369 735f 6465 6d6f 2e69  _analysis_demo.i
+00002a40: 7079 6e62 5d28 6874 7470 733a 2f2f 6769  pynb](https://gi
+00002a50: 7468 7562 2e63 6f6d 2f6d 7761 6c6d 736c  thub.com/mwalmsl
+00002a60: 6579 2f7a 6f6f 626f 742f 626c 6f62 2f6d  ey/zoobot/blob/m
+00002a70: 6169 6e2f 677a 5f64 6563 616c 735f 6461  ain/gz_decals_da
+00002a80: 7461 5f72 656c 6561 7365 5f61 6e61 6c79  ta_release_analy
+00002a90: 7369 735f 6465 6d6f 2e69 7079 6e62 292e  sis_demo.ipynb).
+00002aa0: 0a0a 0a23 2323 2028 4f70 7469 6f6e 616c  ...### (Optional
+00002ab0: 2920 496e 7374 616c 6c20 5079 546f 7263  ) Install PyTorc
+00002ac0: 6820 7769 7468 2043 5544 410a 0a3c 6120  h with CUDA..<a 
+00002ad0: 6e61 6d65 3d22 696e 7374 616c 6c5f 6375  name="install_cu
+00002ae0: 6461 223e 3c2f 613e 0a0a 2a49 6620 796f  da"></a>..*If yo
+00002af0: 7527 7265 206e 6f74 2075 7369 6e67 2061  u're not using a
+00002b00: 2047 5055 2c20 736b 6970 2074 6869 7320   GPU, skip this 
+00002b10: 7374 6570 2e20 5573 6520 7468 6520 7079  step. Use the py
+00002b20: 746f 7263 682d 6370 7520 6f70 7469 6f6e  torch-cpu option
+00002b30: 2069 6e20 7468 6520 7365 6374 696f 6e20   in the section 
+00002b40: 6265 6c6f 772e 2a0a 0a49 6e73 7461 6c6c  below.*..Install
+00002b50: 2050 7954 6f72 6368 2032 2e31 2e30 206f   PyTorch 2.1.0 o
+00002b60: 7220 5465 6e73 6f72 666c 6f77 2032 2e31  r Tensorflow 2.1
+00002b70: 302e 3020 616e 6420 636f 6d70 6174 6962  0.0 and compatib
+00002b80: 6c65 2043 5544 4120 6472 6976 6572 732e  le CUDA drivers.
+00002b90: 2049 2068 6967 686c 7920 7265 636f 6d6d   I highly recomm
+00002ba0: 656e 6420 7573 696e 6720 5b63 6f6e 6461  end using [conda
+00002bb0: 5d28 6874 7470 733a 2f2f 646f 6373 2e63  ](https://docs.c
+00002bc0: 6f6e 6461 2e69 6f2f 656e 2f6c 6174 6573  onda.io/en/lates
+00002bd0: 742f 6d69 6e69 636f 6e64 612e 6874 6d6c  t/miniconda.html
+00002be0: 2920 746f 2064 6f20 7468 6973 2e20 436f  ) to do this. Co
+00002bf0: 6e64 6120 7769 6c6c 2068 616e 646c 6520  nda will handle 
+00002c00: 626f 7468 2063 7265 6174 696e 6720 6120  both creating a 
+00002c10: 6e65 7720 7669 7274 7561 6c20 656e 7669  new virtual envi
+00002c20: 726f 6e6d 656e 7420 2860 636f 6e64 6120  ronment (`conda 
+00002c30: 6372 6561 7465 6029 2061 6e64 2069 6e73  create`) and ins
+00002c40: 7461 6c6c 696e 6720 4355 4441 2028 6063  talling CUDA (`c
+00002c50: 7564 6174 6f6f 6c6b 6974 602c 2060 6375  udatoolkit`, `cu
+00002c60: 646e 6e60 290a 0a43 5544 4120 3132 2e31  dnn`)..CUDA 12.1
+00002c70: 2066 6f72 2050 7954 6f72 6368 2032 2e31   for PyTorch 2.1
+00002c80: 2e30 3a0a 0a20 2020 2063 6f6e 6461 2063  .0:..    conda c
+00002c90: 7265 6174 6520 2d2d 6e61 6d65 207a 6f6f  reate --name zoo
+00002ca0: 626f 7433 395f 746f 7263 6820 7079 7468  bot39_torch pyth
+00002cb0: 6f6e 3d3d 332e 390a 2020 2020 636f 6e64  on==3.9.    cond
+00002cc0: 6120 6163 7469 7661 7465 207a 6f6f 626f  a activate zoobo
+00002cd0: 7433 395f 746f 7263 680a 2020 2020 636f  t39_torch.    co
+00002ce0: 6e64 6120 696e 7374 616c 6c20 2d63 2063  nda install -c c
+00002cf0: 6f6e 6461 2d66 6f72 6765 2063 7564 6174  onda-forge cudat
+00002d00: 6f6f 6c6b 6974 3d31 322e 310a 0a23 2323  oolkit=12.1..###
+00002d10: 2052 6563 656e 7420 7265 6c65 6173 6520   Recent release 
+00002d20: 6665 6174 7572 6573 2028 7632 2e30 2e30  features (v2.0.0
+00002d30: 290a 0a2d 204e 6577 2070 7265 7472 6169  )..- New pretrai
+00002d40: 6e65 6420 6172 6368 6974 6563 7475 7265  ned architecture
+00002d50: 733a 2043 6f6e 764e 6558 542c 2045 6666  s: ConvNeXT, Eff
+00002d60: 6963 6965 6e74 4e65 7456 322c 204d 6178  icientNetV2, Max
+00002d70: 5669 542c 2061 6e64 206d 6f72 652e 2045  ViT, and more. E
+00002d80: 6163 6820 696e 2073 6576 6572 616c 2073  ach in several s
+00002d90: 697a 6573 2e0a 2d20 5265 776f 726b 6564  izes..- Reworked
+00002da0: 2066 696e 6574 756e 696e 6720 7072 6f63   finetuning proc
+00002db0: 6564 7572 652e 2041 6c6c 2074 6865 7365  edure. All these
+00002dc0: 2061 7263 6869 7465 6374 7572 6573 2061   architectures a
+00002dd0: 7265 2066 696e 6574 756e 6561 626c 6520  re finetuneable 
+00002de0: 7468 726f 7567 6820 6120 636f 6d6d 6f6e  through a common
+00002df0: 206d 6574 686f 642e 0a2d 2052 6577 6f72   method..- Rewor
+00002e00: 6b65 6420 6669 6e65 7475 6e69 6e67 206f  ked finetuning o
+00002e10: 7074 696f 6e73 2e20 4261 7463 6820 6e6f  ptions. Batch no
+00002e20: 726d 2066 696e 6574 756e 696e 6720 7265  rm finetuning re
+00002e30: 6d6f 7665 642e 2043 6f73 696e 6520 7363  moved. Cosine sc
+00002e40: 6865 6475 6c65 206f 7074 696f 6e20 6164  hedule option ad
+00002e50: 6465 642e 0a2d 2052 6577 6f72 6b65 6420  ded..- Reworked 
+00002e60: 6669 6e65 7475 6e69 6e67 2073 6176 696e  finetuning savin
+00002e70: 672f 6c6f 6164 696e 672e 2041 7574 6f2d  g/loading. Auto-
+00002e80: 646f 776e 6c6f 6164 7320 656e 636f 6465  downloads encode
+00002e90: 7220 6672 6f6d 2048 7567 6769 6e67 4661  r from HuggingFa
+00002ea0: 6365 2e0a 2d20 4e6f 7720 7375 7070 6f72  ce..- Now suppor
+00002eb0: 7473 2072 6567 7265 7373 696f 6e20 6669  ts regression fi
+00002ec0: 6e65 7475 6e69 6e67 2028 6173 2077 656c  netuning (as wel
+00002ed0: 6c20 6173 206d 756c 7469 2d63 6c61 7373  l as multi-class
+00002ee0: 2061 6e64 2062 696e 6172 7929 2e20 5365   and binary). Se
+00002ef0: 6520 6070 7974 6f72 6368 2f65 7861 6d70  e `pytorch/examp
+00002f00: 6c65 732f 6669 6e65 7475 6e69 6e67 600a  les/finetuning`.
+00002f10: 2d20 5570 6461 7465 6420 6074 696d 6d60  - Updated `timm`
+00002f20: 2074 6f20 302e 392e 3130 2c20 616c 6c6f   to 0.9.10, allo
+00002f30: 7769 6e67 206c 6174 6573 7420 6d6f 6465  wing latest mode
+00002f40: 6c20 6172 6368 6974 6563 7475 7265 732e  l architectures.
+00002f50: 2050 7265 7669 6f75 736c 7920 646f 776e   Previously down
+00002f60: 6c6f 6164 6564 2063 6865 636b 706f 696e  loaded checkpoin
+00002f70: 7473 206d 6179 206e 6f74 206c 6f61 6420  ts may not load 
+00002f80: 636f 7272 6563 746c 7921 0a2d 2028 696e  correctly!.- (in
+00002f90: 7465 726e 616c 2075 6e74 696c 2070 7562  ternal until pub
+00002fa0: 6c69 7368 6564 2920 475a 2045 766f 2076  lished) GZ Evo v
+00002fb0: 3220 6e6f 7720 696e 636c 7564 6573 2043  2 now includes C
+00002fc0: 6f73 6d69 6320 4461 776e 2028 4853 4320  osmic Dawn (HSC 
+00002fd0: 4832 4f29 2e20 5369 676e 6966 6963 616e  H2O). Significan
+00002fe0: 7420 7065 7266 6f72 6d61 6e63 6520 696d  t performance im
+00002ff0: 7072 6f76 656d 656e 7420 6f6e 2048 5343  provement on HSC
+00003000: 2066 696e 6574 756e 696e 672e 2041 6c73   finetuning. Als
+00003010: 6f20 6e6f 7720 696e 636c 7564 6573 2047  o now includes G
+00003020: 5a20 554b 4944 5353 2028 6472 6167 6765  Z UKIDSS (dragge
+00003030: 6420 6672 6f6d 206f 7572 2061 7263 6869  d from our archi
+00003040: 7665 7329 2e0a 2d20 5570 6461 7465 6420  ves)..- Updated 
+00003050: 6070 7974 6f72 6368 6020 746f 2060 322e  `pytorch` to `2.
+00003060: 312e 3060 0a2d 2041 6464 6564 2073 7570  1.0`.- Added sup
+00003070: 706f 7274 2066 6f72 2077 6562 6461 7461  port for webdata
+00003080: 7365 7473 2028 6f6e 6c79 2072 6563 6f6d  sets (only recom
+00003090: 6d65 6e64 6564 2066 6f72 206c 6172 6765  mended for large
+000030a0: 2d73 6361 6c65 2064 6973 7472 6962 7574  -scale distribut
+000030b0: 6564 2074 7261 696e 696e 6729 0a2d 2049  ed training).- I
+000030c0: 6d70 726f 7665 6420 7065 722d 7175 6573  mproved per-ques
+000030d0: 7469 6f6e 206c 6f67 6769 6e67 2077 6865  tion logging whe
+000030e0: 6e20 7472 6169 6e69 6e67 2066 726f 6d20  n training from 
+000030f0: 7363 7261 7463 680a 2d20 4164 6465 6420  scratch.- Added 
+00003100: 6f70 7469 6f6e 2074 6f20 636f 6d70 696c  option to compil
+00003110: 6520 656e 636f 6465 7220 666f 7220 6d61  e encoder for ma
+00003120: 7820 7370 6565 6420 286e 6f74 2072 6563  x speed (not rec
+00003130: 6f6d 6d65 6e64 6564 2066 6f72 2066 696e  ommended for fin
+00003140: 6574 756e 696e 672c 206f 6e6c 7920 666f  etuning, only fo
+00003150: 7220 7072 6574 7261 696e 696e 6729 2e0a  r pretraining)..
+00003160: 2d20 4465 7072 6563 6174 6573 2054 656e  - Deprecates Ten
+00003170: 736f 7246 6c6f 772e 2054 6865 2043 5320  sorFlow. The CS 
+00003180: 7265 7365 6172 6368 2063 6f6d 6d75 6e69  research communi
+00003190: 7479 2066 6f63 7573 6573 206f 6e20 5079  ty focuses on Py
+000031a0: 546f 7263 6820 616e 6420 6e65 7720 6672  Torch and new fr
+000031b0: 616d 6577 6f72 6b73 206c 696b 6520 4a41  ameworks like JA
+000031c0: 582e 0a0a 436f 6e74 7269 6275 7469 6f6e  X...Contribution
+000031d0: 7320 6172 6520 7665 7279 2077 656c 636f  s are very welco
+000031e0: 6d65 2061 6e64 2077 696c 6c20 6265 2063  me and will be c
+000031f0: 7265 6469 7465 6420 696e 2061 6e79 2066  redited in any f
+00003200: 7574 7572 6520 776f 726b 2e20 506c 6561  uture work. Plea
+00003210: 7365 2067 6574 2069 6e20 746f 7563 6821  se get in touch!
+00003220: 2053 6565 205b 434f 4e54 5249 4255 5449   See [CONTRIBUTI
+00003230: 4e47 2e6d 645d 2868 7474 7073 3a2f 2f67  NG.md](https://g
+00003240: 6974 6875 622e 636f 6d2f 6d77 616c 6d73  ithub.com/mwalms
+00003250: 6c65 792f 7a6f 6f62 6f74 2f62 6c6f 622f  ley/zoobot/blob/
+00003260: 6d61 696e 2f62 656e 6368 6d61 726b 7329  main/benchmarks)
+00003270: 2066 6f72 206d 6f72 652e 0a0a 2323 2320   for more...### 
+00003280: 4265 6e63 686d 6172 6b73 2061 6e64 2052  Benchmarks and R
+00003290: 6570 6c69 6361 7469 6f6e 202d 2054 7261  eplication - Tra
+000032a0: 696e 696e 6720 6672 6f6d 2053 6372 6174  ining from Scrat
+000032b0: 6368 0a0a 5468 6520 5b62 656e 6368 6d61  ch..The [benchma
+000032c0: 726b 735d 2868 7474 7073 3a2f 2f67 6974  rks](https://git
+000032d0: 6875 622e 636f 6d2f 6d77 616c 6d73 6c65  hub.com/mwalmsle
+000032e0: 792f 7a6f 6f62 6f74 2f62 6c6f 622f 6d61  y/zoobot/blob/ma
+000032f0: 696e 2f62 656e 6368 6d61 726b 7329 2066  in/benchmarks) f
+00003300: 6f6c 6465 7220 636f 6e74 6169 6e73 2073  older contains s
+00003310: 6c75 726d 2061 6e64 2050 7974 686f 6e20  lurm and Python 
+00003320: 7363 7269 7074 7320 746f 2074 7261 696e  scripts to train
+00003330: 205a 6f6f 626f 7420 6672 6f6d 2073 6372   Zoobot from scr
+00003340: 6174 6368 2e20 5765 2075 7365 2074 6865  atch. We use the
+00003350: 7365 2073 6372 6970 7473 2074 6f20 6d61  se scripts to ma
+00003360: 6b65 2073 7572 6520 6e65 7720 636f 6465  ke sure new code
+00003370: 2076 6572 7369 6f6e 7320 776f 726b 2077   versions work w
+00003380: 656c 6c2c 2061 6e64 2074 6861 7420 5465  ell, and that Te
+00003390: 6e73 6f72 466c 6f77 2061 6e64 2050 7954  nsorFlow and PyT
+000033a0: 6f72 6368 2061 6368 6965 7665 2073 696d  orch achieve sim
+000033b0: 696c 6172 2070 6572 666f 726d 616e 6365  ilar performance
+000033c0: 2e0a 0a54 7261 696e 696e 6720 5a6f 6f62  ...Training Zoob
+000033d0: 6f74 2075 7369 6e67 2074 6865 2047 5a20  ot using the GZ 
+000033e0: 4445 4361 4c53 2064 6174 6173 6574 206f  DECaLS dataset o
+000033f0: 7074 696f 6e20 7769 6c6c 2063 7265 6174  ption will creat
+00003400: 6520 6d6f 6465 6c73 2076 6572 7920 7369  e models very si
+00003410: 6d69 6c61 7220 746f 2074 686f 7365 2075  milar to those u
+00003420: 7365 6420 666f 7220 7468 6520 475a 2044  sed for the GZ D
+00003430: 4543 614c 5320 6361 7461 6c6f 6775 6520  ECaLS catalogue 
+00003440: 616e 6420 7368 6172 6564 2077 6974 6820  and shared with 
+00003450: 7468 6520 6561 726c 7920 7665 7273 696f  the early versio
+00003460: 6e73 206f 6620 7468 6973 2072 6570 6f2e  ns of this repo.
+00003470: 2054 6865 2047 5a20 4445 5349 205a 6f6f   The GZ DESI Zoo
+00003480: 626f 7420 6d6f 6465 6c20 6973 2074 7261  bot model is tra
+00003490: 696e 6564 206f 6e20 6164 6469 7469 6f6e  ined on addition
+000034a0: 616c 2064 6174 6120 2847 5a44 2d31 2c20  al data (GZD-1, 
+000034b0: 475a 442d 3229 2c20 6173 2074 6865 2047  GZD-2), as the G
+000034c0: 5a20 4576 6f20 5a6f 6f62 6f74 206d 6f64  Z Evo Zoobot mod
+000034d0: 656c 2028 475a 442d 312f 322f 352c 2048  el (GZD-1/2/5, H
+000034e0: 7562 626c 652c 2043 616e 6465 6c73 2c20  ubble, Candels, 
+000034f0: 475a 3229 2e0a 0a2a 2a50 7265 7472 6169  GZ2)...**Pretrai
+00003500: 6e69 6e67 2069 7320 6265 636f 6d69 6e67  ning is becoming
+00003510: 2069 6e63 7265 6173 696e 676c 7920 636f   increasingly co
+00003520: 6d70 6c65 7820 616e 6420 6973 206e 6f77  mplex and is now
+00003530: 2070 6172 7469 616c 6c79 2072 6566 6163   partially refac
+00003540: 746f 7265 6420 6f75 7420 746f 2061 2073  tored out to a s
+00003550: 6570 6172 6174 6520 7265 706f 7369 746f  eparate reposito
+00003560: 7279 2e20 5765 2061 7265 2067 7261 6475  ry. We are gradu
+00003570: 616c 6c79 206d 6967 7261 7469 6e67 2074  ally migrating t
+00003580: 6869 7320 607a 6f6f 626f 7460 2072 6570  his `zoobot` rep
+00003590: 6f73 6974 6f72 7920 746f 2066 6f63 7573  ository to focus
+000035a0: 206f 6e20 6669 6e65 7475 6e69 6e67 2e2a   on finetuning.*
+000035b0: 2a0a 0a23 2323 2043 6974 696e 670a 0a49  *..### Citing..I
+000035c0: 6620 796f 7520 7573 6520 7468 6973 2073  f you use this s
+000035d0: 6f66 7477 6172 652c 206f 7220 6f74 6865  oftware, or othe
+000035e0: 7277 6973 6520 7769 7368 2074 6f20 6369  rwise wish to ci
+000035f0: 7465 205a 6f6f 626f 7420 6173 2061 2073  te Zoobot as a s
+00003600: 6f66 7477 6172 6520 7061 636b 6167 652c  oftware package,
+00003610: 2070 6c65 6173 6520 7573 6520 7468 6520   please use the 
+00003620: 5b4a 4f53 5320 7061 7065 725d 2868 7474  [JOSS paper](htt
+00003630: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00003640: 3231 3130 352f 6a6f 7373 2e30 3533 3132  21105/joss.05312
+00003650: 293a 0a0a 2020 2020 4061 7274 6963 6c65  ):..    @article
+00003660: 7b57 616c 6d73 6c65 7932 3032 332c 2064  {Walmsley2023, d
+00003670: 6f69 203d 207b 3130 2e32 3131 3035 2f6a  oi = {10.21105/j
+00003680: 6f73 732e 3035 3331 327d 2c20 7572 6c20  oss.05312}, url 
+00003690: 3d20 7b68 7474 7073 3a2f 2f64 6f69 2e6f  = {https://doi.o
+000036a0: 7267 2f31 302e 3231 3130 352f 6a6f 7373  rg/10.21105/joss
+000036b0: 2e30 3533 3132 7d2c 2079 6561 7220 3d20  .05312}, year = 
+000036c0: 7b32 3032 337d 2c20 7075 626c 6973 6865  {2023}, publishe
+000036d0: 7220 3d20 7b54 6865 204f 7065 6e20 4a6f  r = {The Open Jo
+000036e0: 7572 6e61 6c7d 2c20 766f 6c75 6d65 203d  urnal}, volume =
+000036f0: 207b 387d 2c20 6e75 6d62 6572 203d 207b   {8}, number = {
+00003700: 3835 7d2c 2070 6167 6573 203d 207b 3533  85}, pages = {53
+00003710: 3132 7d2c 2061 7574 686f 7220 3d20 7b4d  12}, author = {M
+00003720: 696b 6520 5761 6c6d 736c 6579 2061 6e64  ike Walmsley and
+00003730: 2043 616d 7062 656c 6c20 416c 6c65 6e20   Campbell Allen 
+00003740: 616e 6420 4265 6e20 4175 7373 656c 2061  and Ben Aussel a
+00003750: 6e64 204d 6963 6168 2042 6f77 6c65 7320  nd Micah Bowles 
+00003760: 616e 6420 4b61 7369 6120 4772 6567 6f72  and Kasia Gregor
+00003770: 6f77 6963 7a20 616e 6420 496e 6967 6f20  owicz and Inigo 
+00003780: 5661 6c20 536c 696a 6570 6365 7669 6320  Val Slijepcevic 
+00003790: 616e 6420 4368 7269 7320 4a2e 204c 696e  and Chris J. Lin
+000037a0: 746f 7474 2061 6e64 2041 6e6e 6120 4d2e  tott and Anna M.
+000037b0: 206d 2e20 5363 6169 6665 2061 6e64 204d   m. Scaife and M
+000037c0: 616a 6120 4a61 62c5 826f c584 736b 6120  aja Jab..o..ska 
+000037d0: 616e 6420 4b6f 7369 6f20 4b61 7263 6865  and Kosio Karche
+000037e0: 7620 616e 6420 4465 6e69 7365 204c 616e  v and Denise Lan
+000037f0: 7a69 6572 6920 616e 6420 4465 7669 6e61  zieri and Devina
+00003800: 204d 6f68 616e 2061 6e64 2044 6176 6964   Mohan and David
+00003810: 204f e280 9952 7961 6e20 616e 6420 4268   O...Ryan and Bh
+00003820: 6172 6174 6820 5361 6967 7568 616e 2061  arath Saiguhan a
+00003830: 6e64 2043 7269 7365 6c20 5375 c3a1 7265  nd Crisel Su..re
+00003840: 7a20 616e 6420 4e69 636f 6cc3 a173 2047  z and Nicol..s G
+00003850: 7565 7272 612d 5661 7261 7320 616e 6420  uerra-Varas and 
+00003860: 5265 6e75 6b61 2056 656c 757d 2c20 7469  Renuka Velu}, ti
+00003870: 746c 6520 3d20 7b5a 6f6f 626f 743a 2041  tle = {Zoobot: A
+00003880: 6461 7074 6162 6c65 2044 6565 7020 4c65  daptable Deep Le
+00003890: 6172 6e69 6e67 204d 6f64 656c 7320 666f  arning Models fo
+000038a0: 7220 4761 6c61 7879 204d 6f72 7068 6f6c  r Galaxy Morphol
+000038b0: 6f67 797d 2c20 6a6f 7572 6e61 6c20 3d20  ogy}, journal = 
+000038c0: 7b4a 6f75 726e 616c 206f 6620 4f70 656e  {Journal of Open
+000038d0: 2053 6f75 7263 6520 536f 6674 7761 7265   Source Software
+000038e0: 7d20 7d20 0a0a 596f 7520 6d69 6768 7420  } } ..You might 
+000038f0: 6265 2069 6e74 6572 6573 7465 6420 696e  be interested in
+00003900: 2072 6561 6469 6e67 2070 6170 6572 7320   reading papers 
+00003910: 7573 696e 6720 5a6f 6f62 6f74 3a0a 0a2d  using Zoobot:..-
+00003920: 205b 4761 6c61 7879 205a 6f6f 2044 4543   [Galaxy Zoo DEC
+00003930: 614c 533a 2044 6574 6169 6c65 6420 7669  aLS: Detailed vi
+00003940: 7375 616c 206d 6f72 7068 6f6c 6f67 7920  sual morphology 
+00003950: 6d65 6173 7572 656d 656e 7473 2066 726f  measurements fro
+00003960: 6d20 766f 6c75 6e74 6565 7273 2061 6e64  m volunteers and
+00003970: 2064 6565 7020 6c65 6172 6e69 6e67 2066   deep learning f
+00003980: 6f72 2033 3134 2c30 3030 2067 616c 6178  or 314,000 galax
+00003990: 6965 735d 2868 7474 7073 3a2f 2f61 7278  ies](https://arx
+000039a0: 6976 2e6f 7267 2f61 6273 2f32 3130 322e  iv.org/abs/2102.
+000039b0: 3038 3431 3429 2028 3230 3232 290a 2d20  08414) (2022).- 
+000039c0: 5b41 2043 6f6d 7061 7269 736f 6e20 6f66  [A Comparison of
+000039d0: 2044 6565 7020 4c65 6172 6e69 6e67 2041   Deep Learning A
+000039e0: 7263 6869 7465 6374 7572 6573 2066 6f72  rchitectures for
+000039f0: 204f 7074 6963 616c 2047 616c 6178 7920   Optical Galaxy 
+00003a00: 4d6f 7270 686f 6c6f 6779 2043 6c61 7373  Morphology Class
+00003a10: 6966 6963 6174 696f 6e5d 2868 7474 7073  ification](https
+00003a20: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
+00003a30: 2f32 3131 312e 3034 3335 3329 2028 3230  /2111.04353) (20
+00003a40: 3232 290a 2d20 5b50 7261 6374 6963 616c  22).- [Practical
+00003a50: 2047 616c 6178 7920 4d6f 7270 686f 6c6f   Galaxy Morpholo
+00003a60: 6779 2054 6f6f 6c73 2066 726f 6d20 4465  gy Tools from De
+00003a70: 6570 2053 7570 6572 7669 7365 6420 5265  ep Supervised Re
+00003a80: 7072 6573 656e 7461 7469 6f6e 204c 6561  presentation Lea
+00003a90: 726e 696e 675d 2868 7474 7073 3a2f 2f61  rning](https://a
+00003aa0: 7278 6976 2e6f 7267 2f61 6273 2f32 3131  rxiv.org/abs/211
+00003ab0: 302e 3132 3733 3529 2028 3230 3232 290a  0.12735) (2022).
+00003ac0: 2d20 5b54 6f77 6172 6473 2046 6f75 6e64  - [Towards Found
+00003ad0: 6174 696f 6e20 4d6f 6465 6c73 2066 6f72  ation Models for
+00003ae0: 2047 616c 6178 7920 4d6f 7270 686f 6c6f   Galaxy Morpholo
+00003af0: 6779 5d28 6874 7470 733a 2f2f 6172 7869  gy](https://arxi
+00003b00: 762e 6f72 672f 6162 732f 3232 3036 2e31  v.org/abs/2206.1
+00003b10: 3139 3237 2920 2832 3032 3229 0a2d 205b  1927) (2022).- [
+00003b20: 4861 726e 6573 7369 6e67 2074 6865 2048  Harnessing the H
+00003b30: 7562 626c 6520 5370 6163 6520 5465 6c65  ubble Space Tele
+00003b40: 7363 6f70 6520 4172 6368 6976 6573 3a20  scope Archives: 
+00003b50: 4120 4361 7461 6c6f 6775 6520 6f66 2032  A Catalogue of 2
+00003b60: 312c 3932 3620 496e 7465 7261 6374 696e  1,926 Interactin
+00003b70: 6720 4761 6c61 7869 6573 5d28 6874 7470  g Galaxies](http
+00003b80: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00003b90: 732f 3233 3033 2e30 3033 3636 2920 2832  s/2303.00366) (2
+00003ba0: 3032 3329 0a2d 205b 4761 6c61 7879 205a  023).- [Galaxy Z
+00003bb0: 6f6f 2044 4553 493a 2044 6574 6169 6c65  oo DESI: Detaile
+00003bc0: 6420 6d6f 7270 686f 6c6f 6779 206d 6561  d morphology mea
+00003bd0: 7375 7265 6d65 6e74 7320 666f 7220 382e  surements for 8.
+00003be0: 374d 2067 616c 6178 6965 7320 696e 2074  7M galaxies in t
+00003bf0: 6865 2044 4553 4920 4c65 6761 6379 2049  he DESI Legacy I
+00003c00: 6d61 6769 6e67 2053 7572 7665 7973 5d28  maging Surveys](
+00003c10: 6874 7470 733a 2f2f 6163 6164 656d 6963  https://academic
+00003c20: 2e6f 7570 2e63 6f6d 2f6d 6e72 6173 2f61  .oup.com/mnras/a
+00003c30: 6476 616e 6365 2d61 7274 6963 6c65 2f64  dvance-article/d
+00003c40: 6f69 2f31 302e 3130 3933 2f6d 6e72 6173  oi/10.1093/mnras
+00003c50: 2f73 7461 6432 3931 392f 3732 3833 3136  /stad2919/728316
+00003c60: 393f 6c6f 6769 6e3d 6661 6c73 6529 2028  9?login=false) (
+00003c70: 3230 3233 290a 2d20 5b47 616c 6178 7920  2023).- [Galaxy 
+00003c80: 6d65 7267 6572 7320 696e 2053 7562 6172  mergers in Subar
+00003c90: 7520 4853 432d 5353 503a 2041 2064 6565  u HSC-SSP: A dee
+00003ca0: 7020 7265 7072 6573 656e 7461 7469 6f6e  p representation
+00003cb0: 206c 6561 726e 696e 6720 6170 7072 6f61   learning approa
+00003cc0: 6368 2066 6f72 2069 6465 6e74 6966 6963  ch for identific
+00003cd0: 6174 696f 6e2c 2061 6e64 2074 6865 2072  ation, and the r
+00003ce0: 6f6c 6520 6f66 2065 6e76 6972 6f6e 6d65  ole of environme
+00003cf0: 6e74 206f 6e20 6d65 7267 6572 2069 6e63  nt on merger inc
+00003d00: 6964 656e 6365 5d28 6874 7470 733a 2f2f  idence](https://
+00003d10: 646f 692e 6f72 672f 3130 2e31 3035 312f  doi.org/10.1051/
+00003d20: 3030 3034 2d36 3336 312f 3230 3233 3436  0004-6361/202346
+00003d30: 3734 3329 2028 3230 3233 290a 2d20 5b41  743) (2023).- [A
+00003d40: 7374 726f 6e6f 6d61 6c79 2061 7420 5363  stronomaly at Sc
+00003d50: 616c 653a 2053 6561 7263 6869 6e67 2066  ale: Searching f
+00003d60: 6f72 2041 6e6f 6d61 6c69 6573 2041 6d6f  or Anomalies Amo
+00003d70: 6e67 7374 2034 204d 696c 6c69 6f6e 2047  ngst 4 Million G
+00003d80: 616c 6178 6965 735d 2868 7474 7073 3a2f  alaxies](https:/
+00003d90: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00003da0: 3330 392e 3038 3636 3029 2028 3230 3233  309.08660) (2023
+00003db0: 2c20 7375 626d 6974 7465 6429 0a2d 205b  , submitted).- [
+00003dc0: 5472 616e 7366 6572 206c 6561 726e 696e  Transfer learnin
+00003dd0: 6720 666f 7220 6761 6c61 7879 2066 6561  g for galaxy fea
+00003de0: 7475 7265 2064 6574 6563 7469 6f6e 3a20  ture detection: 
+00003df0: 4669 6e64 696e 6720 4769 616e 7420 5374  Finding Giant St
+00003e00: 6172 2d66 6f72 6d69 6e67 2043 6c75 6d70  ar-forming Clump
+00003e10: 7320 696e 206c 6f77 2072 6564 7368 6966  s in low redshif
+00003e20: 7420 6761 6c61 7869 6573 2075 7369 6e67  t galaxies using
+00003e30: 2046 6173 7465 7220 522d 434e 4e5d 2868   Faster R-CNN](h
+00003e40: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00003e50: 2f61 6273 2f32 3331 322e 3033 3530 3329  /abs/2312.03503)
+00003e60: 2028 3230 3233 290a 2d20 5b45 7563 6c69   (2023).- [Eucli
+00003e70: 6420 7072 6570 6172 6174 696f 6e2e 204d  d preparation. M
+00003e80: 6561 7375 7269 6e67 2064 6574 6169 6c65  easuring detaile
+00003e90: 6420 6761 6c61 7879 206d 6f72 7068 6f6c  d galaxy morphol
+00003ea0: 6f67 6965 7320 666f 7220 4575 636c 6964  ogies for Euclid
+00003eb0: 2077 6974 6820 4d61 6368 696e 6520 4c65   with Machine Le
+00003ec0: 6172 6e69 6e67 5d28 6874 7470 733a 2f2f  arning](https://
+00003ed0: 6172 7869 762e 6f72 672f 6162 732f 3234  arxiv.org/abs/24
+00003ee0: 3032 2e31 3031 3837 2920 2832 3032 342c  02.10187) (2024,
+00003ef0: 2073 7562 6d69 7474 6564 290a 0a4d 616e   submitted)..Man
+00003f00: 7920 6f74 6865 7220 776f 726b 7320 7573  y other works us
+00003f10: 6520 5a6f 6f62 6f74 2069 6e64 6972 6563  e Zoobot indirec
+00003f20: 746c 7920 7669 6120 7468 6520 5b47 616c  tly via the [Gal
+00003f30: 6178 7920 5a6f 6f20 4445 4361 4c53 5d28  axy Zoo DECaLS](
+00003f40: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00003f50: 672f 6162 732f 3231 3032 2e30 3834 3134  g/abs/2102.08414
+00003f60: 2920 6361 7461 6c6f 6720 2861 6e64 206e  ) catalog (and n
+00003f70: 6f77 2076 6961 2074 6865 206e 6577 205b  ow via the new [
+00003f80: 4761 6c61 7879 205a 6f6f 2044 4553 495d  Galaxy Zoo DESI]
+00003f90: 2868 7474 7073 3a2f 2f61 6361 6465 6d69  (https://academi
+00003fa0: 632e 6f75 702e 636f 6d2f 6d6e 7261 732f  c.oup.com/mnras/
+00003fb0: 6164 7661 6e63 652d 6172 7469 636c 652f  advance-article/
+00003fc0: 646f 692f 3130 2e31 3039 332f 6d6e 7261  doi/10.1093/mnra
+00003fd0: 732f 7374 6164 3239 3139 2f37 3238 3331  s/stad2919/72831
+00003fe0: 3639 3f6c 6f67 696e 3d66 616c 7365 2920  69?login=false) 
+00003ff0: 6361 7461 6c6f 6729 2e0a                 catalog)..
```

### Comparing `zoobot-1.0.5/README.md` & `zoobot-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,54 +13,53 @@
 <!-- At Galaxy Zoo, we use Zoobot to help our volunteers classify the galaxies in all our recent catalogues: GZ DECaLS, GZ DESI, GZ Rings and GZ Cosmic Dawn. -->
 
 Zoobot is trained using millions of answers by Galaxy Zoo volunteers. This code will let you **retrain** Zoobot to accurately solve your own prediction task.
 
 - [Install](#installation)
 - [Quickstart](#quickstart)
 - [Worked Examples](#worked-examples)
-- [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/data_notes.html)
+- [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/pretrained_models.html)
 - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
 - [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
 
 ## Installation
+
 <a name="installation"></a>
 
-You can retrain Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing). To install locally, keep reading.
+You can retrain Zoobot in the cloud with a free GPU using this [Google Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing). To install locally, keep reading.
 
 Download the code using git:
 
     git clone git@github.com:mwalmsley/zoobot.git
 
-And then pick one of the three commands below to install Zoobot and either PyTorch (recommended) or TensorFlow:
+And then pick one of the three commands below to install Zoobot and PyTorch:
 
-    # Zoobot with PyTorch and a GPU. Requires CUDA 11.3.
-    pip install -e "zoobot[pytorch_cu113]" --extra-index-url https://download.pytorch.org/whl/cu113
+    # Zoobot with PyTorch and a GPU. Requires CUDA 12.1 (or CUDA 11.8, if you use `_cu118` instead)
+    pip install -e "zoobot[pytorch-cu121]" --extra-index-url https://download.pytorch.org/whl/cu121
 
     # OR Zoobot with PyTorch and no GPU
-    pip install -e "zoobot[pytorch_cpu]" --extra-index-url https://download.pytorch.org/whl/cpu
+    pip install -e "zoobot[pytorch-cpu]" --extra-index-url https://download.pytorch.org/whl/cpu
 
     # OR Zoobot with PyTorch on Mac with M1 chip
-    pip install -e "zoobot[pytorch_m1]"
-
-    # OR Zoobot with TensorFlow. Works with and without a GPU, but if you have a GPU, you need CUDA 11.2. 
-    pip install -e "zoobot[tensorflow]
+    pip install -e "zoobot[pytorch-m1]"
 
 This installs the downloaded Zoobot code using pip [editable mode](https://pip.pypa.io/en/stable/topics/local-project-installs/#editable-installs) so you can easily change the code locally. Zoobot is also available directly from pip (`pip install zoobot[option]`). Only use this if you are sure you won't be making changes to Zoobot itself. For Google Colab, use `pip install zoobot[pytorch_colab]`
 
 To use a GPU, you must *already* have CUDA installed and matching the versions above.
 I share my install steps [here](#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU, just slower.
 
 ## Quickstart
+
 <a name="quickstart"></a>
 
-The [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) is the quickest way to get started. Alternatively, the minimal example below illustrates how Zoobot works.
+The [Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing) is the quickest way to get started. Alternatively, the minimal example below illustrates how Zoobot works.
 
 Let's say you want to find ringed galaxies and you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find rings like so:
 
-```python
+    ```python
 
     import pandas as pd
     from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
     from zoobot.pytorch.training import finetune
 
     # csv with 'ring' column (0 or 1) and 'file_loc' column (path to image)
     labelled_df = pd.read_csv('/your/path/some_labelled_galaxies.csv')
@@ -73,126 +72,114 @@
 
     # load trained Zoobot model
     model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2)  
     
     # retrain to find rings
     trainer = finetune.get_trainer(save_dir)
     trainer.fit(model, datamodule)
-```
+    ```
 
 Then you can make predict if new galaxies have rings:
 
-```python
+    ```python
     from zoobot.pytorch.predictions import predict_on_catalog
 
     # csv with 'file_loc' column (path to image). Zoobot will predict the labels.
     unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
 
     predict_on_catalog.predict(
       unlabelled_df,
       model,
       label_cols=['ring'],  # only used for 
       save_loc='/your/path/finetuned_predictions.csv'
     )
-```
+    ```
 
 Zoobot includes many guides and working examples - see the [Getting Started](#getting-started) section below.
 
 ## Getting Started
+
 <a name="getting_started"></a>
 
-I suggest starting with the [Colab notebook](https://colab.research.google.com/drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below, which you can copy and adapt.
+I suggest starting with the [Colab notebook](https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing) or the worked examples below, which you can copy and adapt.
 
 For context and explanation, see the [documentation](https://zoobot.readthedocs.io/).
 
-For pretrained model weights, precalculated representations, catalogues, and so forth, see the [data notes](https://zoobot.readthedocs.io/en/latest/data_notes.html) in particular.
+Pretrained models are listed [here](https://zoobot.readthedocs.io/en/latest/pretrained_models.html) and available on [HuggingFace](https://huggingface.co/collections/mwalmsley/zoobot-encoders-65fa14ae92911b173712b874)
 
 ### Worked Examples
+
 <a name="worked_examples"></a>
 
 PyTorch (recommended):
+
 - [pytorch/examples/finetuning/finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py)
 - [pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py)
 - [pytorch/examples/representations/get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/representations/get_representations.py)
 - [pytorch/examples/train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/train_model_on_catalog.py) (only necessary to train from scratch)
 
-TensorFlow:
-- [tensorflow/examples/train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/train_model_on_catalog.py) (only necessary to train from scratch)
-- [tensorflow/examples/make_predictions.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/make_predictions.py)
-- [tensorflow/examples/finetune_minimal.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/finetune_minimal.py)
-- [tensorflow/examples/finetune_advanced.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/finetune_advanced.py)
-
 There is more explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
 
 I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to create and benchmark our pretrained models. Many pretrained models are available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html), but if you need one trained on e.g. different input image sizes or with a specific architecture, I can probably make it for you.
 
 When trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from volunteer labels of varying confidence and predict posteriors for what the typical volunteer might say. Specifically, this Zoobot mode predicts the parameters for distributions, not simple class labels! For a demonstration of how to interpret these predictions, see the [gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb).
 
 
+### (Optional) Install PyTorch with CUDA
 
-### (Optional) Install PyTorch or TensorFlow, with CUDA
 <a name="install_cuda"></a>
 
-*If you're not using a GPU, skip this step. Use the pytorch_cpu or tensorflow_cpu options in the section below.*
-
-Install PyTorch 1.12.1 or Tensorflow 2.10.0 and compatible CUDA drivers. I highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both creating a new virtual environment (`conda create`) and installing CUDA (`cudatoolkit`, `cudnn`)
+*If you're not using a GPU, skip this step. Use the pytorch-cpu option in the section below.*
 
-CUDA 11.3 for PyTorch:
+Install PyTorch 2.1.0 or Tensorflow 2.10.0 and compatible CUDA drivers. I highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both creating a new virtual environment (`conda create`) and installing CUDA (`cudatoolkit`, `cudnn`)
 
-    conda create --name zoobot38_torch python==3.8
-    conda activate zoobot38_torch
-    conda install -c conda-forge cudatoolkit=11.3
+CUDA 12.1 for PyTorch 2.1.0:
 
-CUDA 11.2 and CUDNN 8.1 for TensorFlow 2.10.0:
-
-    conda create --name zoobot38_tf python==3.8
-    conda activate zoobot38_tf
-    conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0
-    export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/  # add this environment variable
-
-### Latest minor features (v1.0.4)
-
-- Now supports multi-class finetuning. See `pytorch/examples/finetuning/finetune_multiclass_classification.py`
-- Removed `simplejpeg` dependency due to M1 install issue. 
-- Pinned `timm` version to ensure MaX-ViT models load correctly. Models supporting the latest `timm` will follow.
-- (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC). Significant performance improvement on HSC finetuning.
-
-### Latest major features (v1.0.0)
-
-v1.0.0 recognises that most of the complexity in this repo is training Zoobot from scratch, but most non-GZ users will probably simply want to load the pretrained Zoobot and finetune it on their data.
-
-- Adds new finetuning interface (`finetune.run_finetuning()`), examples.
-- Refocuses docs on finetuning rather than training from scratch.
-- Rework installation process to separate CUDA from Zoobot (simpler, easier)
-- Better wandb logging throughout, to monitor training
-- Remove need to make TFRecords. Now TF directly uses images.
-- Refactor out augmentations and datasets to `galaxy-datasets` repo. TF and Torch now use identical augmentations (via albumentations).
-- Many small quality-of-life improvements
+    conda create --name zoobot39_torch python==3.9
+    conda activate zoobot39_torch
+    conda install -c conda-forge cudatoolkit=12.1
+
+### Recent release features (v2.0.0)
+
+- New pretrained architectures: ConvNeXT, EfficientNetV2, MaxViT, and more. Each in several sizes.
+- Reworked finetuning procedure. All these architectures are finetuneable through a common method.
+- Reworked finetuning options. Batch norm finetuning removed. Cosine schedule option added.
+- Reworked finetuning saving/loading. Auto-downloads encoder from HuggingFace.
+- Now supports regression finetuning (as well as multi-class and binary). See `pytorch/examples/finetuning`
+- Updated `timm` to 0.9.10, allowing latest model architectures. Previously downloaded checkpoints may not load correctly!
+- (internal until published) GZ Evo v2 now includes Cosmic Dawn (HSC H2O). Significant performance improvement on HSC finetuning. Also now includes GZ UKIDSS (dragged from our archives).
+- Updated `pytorch` to `2.1.0`
+- Added support for webdatasets (only recommended for large-scale distributed training)
+- Improved per-question logging when training from scratch
+- Added option to compile encoder for max speed (not recommended for finetuning, only for pretraining).
+- Deprecates TensorFlow. The CS research community focuses on PyTorch and new frameworks like JAX.
 
 Contributions are very welcome and will be credited in any future work. Please get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) for more.
 
 ### Benchmarks and Replication - Training from Scratch
 
 The [benchmarks](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot from scratch. We use these scripts to make sure new code versions work well, and that TensorFlow and PyTorch achieve similar performance.
 
 Training Zoobot using the GZ DECaLS dataset option will create models very similar to those used for the GZ DECaLS catalogue and shared with the early versions of this repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2).
 
+**Pretraining is becoming increasingly complex and is now partially refactored out to a separate repository. We are gradually migrating this `zoobot` repository to focus on finetuning.**
+
 ### Citing
 
 If you use this software, or otherwise wish to cite Zoobot as a software package, please use the [JOSS paper](https://doi.org/10.21105/joss.05312):
 
     @article{Walmsley2023, doi = {10.21105/joss.05312}, url = {https://doi.org/10.21105/joss.05312}, year = {2023}, publisher = {The Open Journal}, volume = {8}, number = {85}, pages = {5312}, author = {Mike Walmsley and Campbell Allen and Ben Aussel and Micah Bowles and Kasia Gregorowicz and Inigo Val Slijepcevic and Chris J. Lintott and Anna M. m. Scaife and Maja Jabłońska and Kosio Karchev and Denise Lanzieri and Devina Mohan and David O’Ryan and Bharath Saiguhan and Crisel Suárez and Nicolás Guerra-Varas and Renuka Velu}, title = {Zoobot: Adaptable Deep Learning Models for Galaxy Morphology}, journal = {Journal of Open Source Software} } 
 
 You might be interested in reading papers using Zoobot:
 
 - [Galaxy Zoo DECaLS: Detailed visual morphology measurements from volunteers and deep learning for 314,000 galaxies](https://arxiv.org/abs/2102.08414) (2022)
 - [A Comparison of Deep Learning Architectures for Optical Galaxy Morphology Classification](https://arxiv.org/abs/2111.04353) (2022)
 - [Practical Galaxy Morphology Tools from Deep Supervised Representation Learning](https://arxiv.org/abs/2110.12735) (2022)
 - [Towards Foundation Models for Galaxy Morphology](https://arxiv.org/abs/2206.11927) (2022)
 - [Harnessing the Hubble Space Telescope Archives: A Catalogue of 21,926 Interacting Galaxies](https://arxiv.org/abs/2303.00366) (2023)
-- [Astronomaly at Scale: Searching for Anomalies Amongst 4 Million Galaxies](https://arxiv.org/abs/2309.08660) (2023)
 - [Galaxy Zoo DESI: Detailed morphology measurements for 8.7M galaxies in the DESI Legacy Imaging Surveys](https://academic.oup.com/mnras/advance-article/doi/10.1093/mnras/stad2919/7283169?login=false) (2023)
 - [Galaxy mergers in Subaru HSC-SSP: A deep representation learning approach for identification, and the role of environment on merger incidence](https://doi.org/10.1051/0004-6361/202346743) (2023)
-
-<!-- submitted papers: simulated merger classification, unsupervised anomaly detection, starforming clump localisation, and morphological segmentation. -->
+- [Astronomaly at Scale: Searching for Anomalies Amongst 4 Million Galaxies](https://arxiv.org/abs/2309.08660) (2023, submitted)
+- [Transfer learning for galaxy feature detection: Finding Giant Star-forming Clumps in low redshift galaxies using Faster R-CNN](https://arxiv.org/abs/2312.03503) (2023)
+- [Euclid preparation. Measuring detailed galaxy morphologies for Euclid with Machine Learning](https://arxiv.org/abs/2402.10187) (2024, submitted)
 
 Many other works use Zoobot indirectly via the [Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) catalog (and now via the new [Galaxy Zoo DESI](https://academic.oup.com/mnras/advance-article/doi/10.1093/mnras/stad2919/7283169?login=false) catalog).
```

#### html2text {}

```diff
@@ -9,42 +9,40 @@
 joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f/status.svg)](https://
 joss.theoj.org/papers/447561ee2de4709eddb704e18bee846f) _[_a_s_c_l_:_2_2_0_3_._0_2_7_]Zoobot
 classifies galaxy morphology with deep learning. Zoobot is trained using
 millions of answers by Galaxy Zoo volunteers. This code will let you
 **retrain** Zoobot to accurately solve your own prediction task. - [Install]
 (#installation) - [Quickstart](#quickstart) - [Worked Examples](#worked-
 examples) - [Pretrained Weights](https://zoobot.readthedocs.io/en/latest/
-data_notes.html) - [Datasets](https://www.github.com/mwalmsley/galaxy-datasets)
-- [Documentation](https://zoobot.readthedocs.io/) (for understanding/reference)
-## Installation You can retrain Zoobot in the cloud with a free GPU using this
-[Google Colab notebook](https://colab.research.google.com/drive/
-17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing). To install locally, keep
-reading. Download the code using git: git clone git@github.com:mwalmsley/
-zoobot.git And then pick one of the three commands below to install Zoobot and
-either PyTorch (recommended) or TensorFlow: # Zoobot with PyTorch and a GPU.
-Requires CUDA 11.3. pip install -e "zoobot[pytorch_cu113]" --extra-index-url
-https://download.pytorch.org/whl/cu113 # OR Zoobot with PyTorch and no GPU pip
-install -e "zoobot[pytorch_cpu]" --extra-index-url https://
+pretrained_models.html) - [Datasets](https://www.github.com/mwalmsley/galaxy-
+datasets) - [Documentation](https://zoobot.readthedocs.io/) (for understanding/
+reference) ## Installation You can retrain Zoobot in the cloud with a free GPU
+using this [Google Colab notebook](https://colab.research.google.com/drive/1A_-
+M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing). To install locally, keep reading.
+Download the code using git: git clone git@github.com:mwalmsley/zoobot.git And
+then pick one of the three commands below to install Zoobot and PyTorch: #
+Zoobot with PyTorch and a GPU. Requires CUDA 12.1 (or CUDA 11.8, if you use
+`_cu118` instead) pip install -e "zoobot[pytorch-cu121]" --extra-index-url
+https://download.pytorch.org/whl/cu121 # OR Zoobot with PyTorch and no GPU pip
+install -e "zoobot[pytorch-cpu]" --extra-index-url https://
 download.pytorch.org/whl/cpu # OR Zoobot with PyTorch on Mac with M1 chip pip
-install -e "zoobot[pytorch_m1]" # OR Zoobot with TensorFlow. Works with and
-without a GPU, but if you have a GPU, you need CUDA 11.2. pip install -
-e "zoobot[tensorflow] This installs the downloaded Zoobot code using pip
-[editable mode](https://pip.pypa.io/en/stable/topics/local-project-installs/
-#editable-installs) so you can easily change the code locally. Zoobot is also
-available directly from pip (`pip install zoobot[option]`). Only use this if
-you are sure you won't be making changes to Zoobot itself. For Google Colab,
-use `pip install zoobot[pytorch_colab]` To use a GPU, you must *already* have
-CUDA installed and matching the versions above. I share my install steps [here]
-(#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU, just
-slower. ## Quickstart The [Colab notebook](https://colab.research.google.com/
-drive/17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) is the quickest way to get
-started. Alternatively, the minimal example below illustrates how Zoobot works.
-Let's say you want to find ringed galaxies and you have a small labelled
-dataset of 500 ringed or not-ringed galaxies. You can retrain Zoobot to find
-rings like so: ```python import pandas as pd from
+install -e "zoobot[pytorch-m1]" This installs the downloaded Zoobot code using
+pip [editable mode](https://pip.pypa.io/en/stable/topics/local-project-
+installs/#editable-installs) so you can easily change the code locally. Zoobot
+is also available directly from pip (`pip install zoobot[option]`). Only use
+this if you are sure you won't be making changes to Zoobot itself. For Google
+Colab, use `pip install zoobot[pytorch_colab]` To use a GPU, you must *already*
+have CUDA installed and matching the versions above. I share my install steps
+[here](#install_cuda). GPUs are optional - Zoobot will run retrain fine on CPU,
+just slower. ## Quickstart The [Colab notebook](https://
+colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-g_Zi0RMGz5?usp=sharing)
+is the quickest way to get started. Alternatively, the minimal example below
+illustrates how Zoobot works. Let's say you want to find ringed galaxies and
+you have a small labelled dataset of 500 ringed or not-ringed galaxies. You can
+retrain Zoobot to find rings like so: ```python import pandas as pd from
 galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule from
 zoobot.pytorch.training import finetune # csv with 'ring' column (0 or 1) and
 'file_loc' column (path to image) labelled_df = pd.read_csv('/your/path/
 some_labelled_galaxies.csv') datamodule = GalaxyDataModule( label_cols=
 ['ring'], catalog=labelled_df, batch_size=32 ) # load trained Zoobot model
 model = finetune.FinetuneableZoobotClassifier(checkpoint_loc, num_classes=2) #
 retrain to find rings trainer = finetune.get_trainer(save_dir) trainer.fit
@@ -52,113 +50,108 @@
 ```python from zoobot.pytorch.predictions import predict_on_catalog # csv with
 'file_loc' column (path to image). Zoobot will predict the labels.
 unlabelled_df = pd.read_csv('/your/path/some_unlabelled_galaxies.csv')
 predict_on_catalog.predict( unlabelled_df, model, label_cols=['ring'], # only
 used for save_loc='/your/path/finetuned_predictions.csv' ) ``` Zoobot includes
 many guides and working examples - see the [Getting Started](#getting-started)
 section below. ## Getting Started I suggest starting with the [Colab notebook]
-(https://colab.research.google.com/drive/
-17bb_KbA2J6yrIm4p4Ue_lEBHMNC1I9Jd?usp=sharing) or the worked examples below,
-which you can copy and adapt. For context and explanation, see the
-[documentation](https://zoobot.readthedocs.io/). For pretrained model weights,
-precalculated representations, catalogues, and so forth, see the [data notes]
-(https://zoobot.readthedocs.io/en/latest/data_notes.html) in particular. ###
-Worked Examples PyTorch (recommended): - [pytorch/examples/finetuning/
-finetune_binary_classification.py](https://github.com/mwalmsley/zoobot/blob/
-main/zoobot/pytorch/examples/finetuning/finetune_binary_classification.py) -
-[pytorch/examples/finetuning/finetune_counts_full_tree.py](https://github.com/
-mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/
-finetune_counts_full_tree.py) - [pytorch/examples/representations/
-get_representations.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
-pytorch/examples/representations/get_representations.py) - [pytorch/examples/
-train_model_on_catalog.py](https://github.com/mwalmsley/zoobot/blob/main/
-zoobot/pytorch/examples/train_model_on_catalog.py) (only necessary to train
-from scratch) TensorFlow: - [tensorflow/examples/train_model_on_catalog.py]
-(https://github.com/mwalmsley/zoobot/blob/main/zoobot/tensorflow/examples/
-train_model_on_catalog.py) (only necessary to train from scratch) -
-[tensorflow/examples/make_predictions.py](https://github.com/mwalmsley/zoobot/
-blob/main/zoobot/tensorflow/examples/make_predictions.py) - [tensorflow/
-examples/finetune_minimal.py](https://github.com/mwalmsley/zoobot/blob/main/
-zoobot/tensorflow/examples/finetune_minimal.py) - [tensorflow/examples/
-finetune_advanced.py](https://github.com/mwalmsley/zoobot/blob/main/zoobot/
-tensorflow/examples/finetune_advanced.py) There is more explanation and an API
-reference on the [docs](https://zoobot.readthedocs.io/). I also [include]
-(https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the scripts used to
-create and benchmark our pretrained models. Many pretrained models are
-available [already](https://zoobot.readthedocs.io/en/latest/data_notes.html),
-but if you need one trained on e.g. different input image sizes or with a
-specific architecture, I can probably make it for you. When trained with a
-decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot can learn from
-volunteer labels of varying confidence and predict posteriors for what the
-typical volunteer might say. Specifically, this Zoobot mode predicts the
-parameters for distributions, not simple class labels! For a demonstration of
-how to interpret these predictions, see the
+(https://colab.research.google.com/drive/1A_-M3Sz5maQmyfW2A7rEu-
+g_Zi0RMGz5?usp=sharing) or the worked examples below, which you can copy and
+adapt. For context and explanation, see the [documentation](https://
+zoobot.readthedocs.io/). Pretrained models are listed [here](https://
+zoobot.readthedocs.io/en/latest/pretrained_models.html) and available on
+[HuggingFace](https://huggingface.co/collections/mwalmsley/zoobot-encoders-
+65fa14ae92911b173712b874) ### Worked Examples PyTorch (recommended): -
+[pytorch/examples/finetuning/finetune_binary_classification.py](https://
+github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/finetuning/
+finetune_binary_classification.py) - [pytorch/examples/finetuning/
+finetune_counts_full_tree.py](https://github.com/mwalmsley/zoobot/blob/main/
+zoobot/pytorch/examples/finetuning/finetune_counts_full_tree.py) - [pytorch/
+examples/representations/get_representations.py](https://github.com/mwalmsley/
+zoobot/blob/main/zoobot/pytorch/examples/representations/
+get_representations.py) - [pytorch/examples/train_model_on_catalog.py](https://
+github.com/mwalmsley/zoobot/blob/main/zoobot/pytorch/examples/
+train_model_on_catalog.py) (only necessary to train from scratch) There is more
+explanation and an API reference on the [docs](https://zoobot.readthedocs.io/).
+I also [include](https://github.com/mwalmsley/zoobot/blob/main/benchmarks) the
+scripts used to create and benchmark our pretrained models. Many pretrained
+models are available [already](https://zoobot.readthedocs.io/en/latest/
+data_notes.html), but if you need one trained on e.g. different input image
+sizes or with a specific architecture, I can probably make it for you. When
+trained with a decision tree head (ZoobotTree, FinetuneableZoobotTree), Zoobot
+can learn from volunteer labels of varying confidence and predict posteriors
+for what the typical volunteer might say. Specifically, this Zoobot mode
+predicts the parameters for distributions, not simple class labels! For a
+demonstration of how to interpret these predictions, see the
 [gz_decals_data_release_analysis_demo.ipynb](https://github.com/mwalmsley/
 zoobot/blob/main/gz_decals_data_release_analysis_demo.ipynb). ### (Optional)
-Install PyTorch or TensorFlow, with CUDA *If you're not using a GPU, skip this
-step. Use the pytorch_cpu or tensorflow_cpu options in the section below.*
-Install PyTorch 1.12.1 or Tensorflow 2.10.0 and compatible CUDA drivers. I
-highly recommend using [conda](https://docs.conda.io/en/latest/miniconda.html)
-to do this. Conda will handle both creating a new virtual environment (`conda
-create`) and installing CUDA (`cudatoolkit`, `cudnn`) CUDA 11.3 for PyTorch:
-conda create --name zoobot38_torch python==3.8 conda activate zoobot38_torch
-conda install -c conda-forge cudatoolkit=11.3 CUDA 11.2 and CUDNN 8.1 for
-TensorFlow 2.10.0: conda create --name zoobot38_tf python==3.8 conda activate
-zoobot38_tf conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0 export
-LD_LIBRARY_PATH=$LD_LIBRARY_PATH:$CONDA_PREFIX/lib/ # add this environment
-variable ### Latest minor features (v1.0.4) - Now supports multi-class
-finetuning. See `pytorch/examples/finetuning/
-finetune_multiclass_classification.py` - Removed `simplejpeg` dependency due to
-M1 install issue. - Pinned `timm` version to ensure MaX-ViT models load
-correctly. Models supporting the latest `timm` will follow. - (internal until
-published) GZ Evo v2 now includes Cosmic Dawn (HSC). Significant performance
-improvement on HSC finetuning. ### Latest major features (v1.0.0) v1.0.0
-recognises that most of the complexity in this repo is training Zoobot from
-scratch, but most non-GZ users will probably simply want to load the pretrained
-Zoobot and finetune it on their data. - Adds new finetuning interface
-(`finetune.run_finetuning()`), examples. - Refocuses docs on finetuning rather
-than training from scratch. - Rework installation process to separate CUDA from
-Zoobot (simpler, easier) - Better wandb logging throughout, to monitor training
-- Remove need to make TFRecords. Now TF directly uses images. - Refactor out
-augmentations and datasets to `galaxy-datasets` repo. TF and Torch now use
-identical augmentations (via albumentations). - Many small quality-of-life
-improvements Contributions are very welcome and will be credited in any future
-work. Please get in touch! See [CONTRIBUTING.md](https://github.com/mwalmsley/
-zoobot/blob/main/benchmarks) for more. ### Benchmarks and Replication -
-Training from Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/
+Install PyTorch with CUDA *If you're not using a GPU, skip this step. Use the
+pytorch-cpu option in the section below.* Install PyTorch 2.1.0 or Tensorflow
+2.10.0 and compatible CUDA drivers. I highly recommend using [conda](https://
+docs.conda.io/en/latest/miniconda.html) to do this. Conda will handle both
+creating a new virtual environment (`conda create`) and installing CUDA
+(`cudatoolkit`, `cudnn`) CUDA 12.1 for PyTorch 2.1.0: conda create --name
+zoobot39_torch python==3.9 conda activate zoobot39_torch conda install -
+c conda-forge cudatoolkit=12.1 ### Recent release features (v2.0.0) - New
+pretrained architectures: ConvNeXT, EfficientNetV2, MaxViT, and more. Each in
+several sizes. - Reworked finetuning procedure. All these architectures are
+finetuneable through a common method. - Reworked finetuning options. Batch norm
+finetuning removed. Cosine schedule option added. - Reworked finetuning saving/
+loading. Auto-downloads encoder from HuggingFace. - Now supports regression
+finetuning (as well as multi-class and binary). See `pytorch/examples/
+finetuning` - Updated `timm` to 0.9.10, allowing latest model architectures.
+Previously downloaded checkpoints may not load correctly! - (internal until
+published) GZ Evo v2 now includes Cosmic Dawn (HSC H2O). Significant
+performance improvement on HSC finetuning. Also now includes GZ UKIDSS (dragged
+from our archives). - Updated `pytorch` to `2.1.0` - Added support for
+webdatasets (only recommended for large-scale distributed training) - Improved
+per-question logging when training from scratch - Added option to compile
+encoder for max speed (not recommended for finetuning, only for pretraining). -
+Deprecates TensorFlow. The CS research community focuses on PyTorch and new
+frameworks like JAX. Contributions are very welcome and will be credited in any
+future work. Please get in touch! See [CONTRIBUTING.md](https://github.com/
+mwalmsley/zoobot/blob/main/benchmarks) for more. ### Benchmarks and Replication
+- Training from Scratch The [benchmarks](https://github.com/mwalmsley/zoobot/
 blob/main/benchmarks) folder contains slurm and Python scripts to train Zoobot
 from scratch. We use these scripts to make sure new code versions work well,
 and that TensorFlow and PyTorch achieve similar performance. Training Zoobot
 using the GZ DECaLS dataset option will create models very similar to those
 used for the GZ DECaLS catalogue and shared with the early versions of this
 repo. The GZ DESI Zoobot model is trained on additional data (GZD-1, GZD-2), as
-the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). ### Citing If you
-use this software, or otherwise wish to cite Zoobot as a software package,
-please use the [JOSS paper](https://doi.org/10.21105/joss.05312): @article
-{Walmsley2023, doi = {10.21105/joss.05312}, url = {https://doi.org/10.21105/
-joss.05312}, year = {2023}, publisher = {The Open Journal}, volume = {8},
-number = {85}, pages = {5312}, author = {Mike Walmsley and Campbell Allen and
-Ben Aussel and Micah Bowles and Kasia Gregorowicz and Inigo Val Slijepcevic and
-Chris J. Lintott and Anna M. m. Scaife and Maja JabÅoÅska and Kosio Karchev
-and Denise Lanzieri and Devina Mohan and David OâRyan and Bharath Saiguhan
-and Crisel SuÃ¡rez and NicolÃ¡s Guerra-Varas and Renuka Velu}, title = {Zoobot:
-Adaptable Deep Learning Models for Galaxy Morphology}, journal = {Journal of
-Open Source Software} } You might be interested in reading papers using Zoobot:
-- [Galaxy Zoo DECaLS: Detailed visual morphology measurements from volunteers
-and deep learning for 314,000 galaxies](https://arxiv.org/abs/2102.08414)
-(2022) - [A Comparison of Deep Learning Architectures for Optical Galaxy
-Morphology Classification](https://arxiv.org/abs/2111.04353) (2022) -
-[Practical Galaxy Morphology Tools from Deep Supervised Representation
-Learning](https://arxiv.org/abs/2110.12735) (2022) - [Towards Foundation Models
-for Galaxy Morphology](https://arxiv.org/abs/2206.11927) (2022) - [Harnessing
-the Hubble Space Telescope Archives: A Catalogue of 21,926 Interacting
-Galaxies](https://arxiv.org/abs/2303.00366) (2023) - [Astronomaly at Scale:
-Searching for Anomalies Amongst 4 Million Galaxies](https://arxiv.org/abs/
-2309.08660) (2023) - [Galaxy Zoo DESI: Detailed morphology measurements for
-8.7M galaxies in the DESI Legacy Imaging Surveys](https://academic.oup.com/
-mnras/advance-article/doi/10.1093/mnras/stad2919/7283169?login=false) (2023) -
-[Galaxy mergers in Subaru HSC-SSP: A deep representation learning approach for
+the GZ Evo Zoobot model (GZD-1/2/5, Hubble, Candels, GZ2). **Pretraining is
+becoming increasingly complex and is now partially refactored out to a separate
+repository. We are gradually migrating this `zoobot` repository to focus on
+finetuning.** ### Citing If you use this software, or otherwise wish to cite
+Zoobot as a software package, please use the [JOSS paper](https://doi.org/
+10.21105/joss.05312): @article{Walmsley2023, doi = {10.21105/joss.05312}, url =
+{https://doi.org/10.21105/joss.05312}, year = {2023}, publisher = {The Open
+Journal}, volume = {8}, number = {85}, pages = {5312}, author = {Mike Walmsley
+and Campbell Allen and Ben Aussel and Micah Bowles and Kasia Gregorowicz and
+Inigo Val Slijepcevic and Chris J. Lintott and Anna M. m. Scaife and Maja
+JabÅoÅska and Kosio Karchev and Denise Lanzieri and Devina Mohan and David
+OâRyan and Bharath Saiguhan and Crisel SuÃ¡rez and NicolÃ¡s Guerra-Varas and
+Renuka Velu}, title = {Zoobot: Adaptable Deep Learning Models for Galaxy
+Morphology}, journal = {Journal of Open Source Software} } You might be
+interested in reading papers using Zoobot: - [Galaxy Zoo DECaLS: Detailed
+visual morphology measurements from volunteers and deep learning for 314,000
+galaxies](https://arxiv.org/abs/2102.08414) (2022) - [A Comparison of Deep
+Learning Architectures for Optical Galaxy Morphology Classification](https://
+arxiv.org/abs/2111.04353) (2022) - [Practical Galaxy Morphology Tools from Deep
+Supervised Representation Learning](https://arxiv.org/abs/2110.12735) (2022) -
+[Towards Foundation Models for Galaxy Morphology](https://arxiv.org/abs/
+2206.11927) (2022) - [Harnessing the Hubble Space Telescope Archives: A
+Catalogue of 21,926 Interacting Galaxies](https://arxiv.org/abs/2303.00366)
+(2023) - [Galaxy Zoo DESI: Detailed morphology measurements for 8.7M galaxies
+in the DESI Legacy Imaging Surveys](https://academic.oup.com/mnras/advance-
+article/doi/10.1093/mnras/stad2919/7283169?login=false) (2023) - [Galaxy
+mergers in Subaru HSC-SSP: A deep representation learning approach for
 identification, and the role of environment on merger incidence](https://
-doi.org/10.1051/0004-6361/202346743) (2023) Many other works use Zoobot
-indirectly via the [Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414)
-catalog (and now via the new [Galaxy Zoo DESI](https://academic.oup.com/mnras/
-advance-article/doi/10.1093/mnras/stad2919/7283169?login=false) catalog).
+doi.org/10.1051/0004-6361/202346743) (2023) - [Astronomaly at Scale: Searching
+for Anomalies Amongst 4 Million Galaxies](https://arxiv.org/abs/2309.08660)
+(2023, submitted) - [Transfer learning for galaxy feature detection: Finding
+Giant Star-forming Clumps in low redshift galaxies using Faster R-CNN](https://
+arxiv.org/abs/2312.03503) (2023) - [Euclid preparation. Measuring detailed
+galaxy morphologies for Euclid with Machine Learning](https://arxiv.org/abs/
+2402.10187) (2024, submitted) Many other works use Zoobot indirectly via the
+[Galaxy Zoo DECaLS](https://arxiv.org/abs/2102.08414) catalog (and now via the
+new [Galaxy Zoo DESI](https://academic.oup.com/mnras/advance-article/doi/
+10.1093/mnras/stad2919/7283169?login=false) catalog).
```

### Comparing `zoobot-1.0.5/setup.py` & `zoobot-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zoobot",
-    version="1.0.5",
+    version="2.0.0",
     author="Mike Walmsley",
     author_email="walmsleymk1@gmail.com",
     description="Galaxy morphology classifiers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mwalmsley/zoobot",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License (GPL)",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Environment :: GPU :: NVIDIA CUDA"
     ],
     packages=setuptools.find_packages(),
-    python_requires=">=3.8",  # recommend 3.9 for new users. TF needs >=3.7.2, torchvision>=3.8
+    python_requires=">=3.9",  # bumped to 3.9 for typing
     extras_require={
-        'pytorch_cpu': [
+        'pytorch-cpu': [
             # A100 GPU currently only seems to support cuda 11.3 on manchester cluster, let's stick with this version for now
             # very latest version wants cuda 11.6
-            'torch == 1.12.1+cpu',
-            'torchvision == 0.13.1+cpu',
-            'torchaudio == 0.12.1',
-            'pytorch-lightning >= 2.0.0',
+            'torch == 2.1.0+cpu',
+            'torchvision == 0.16.0+cpu',
+            'torchaudio >= 2.1.0',
+            'lightning >= 2.0.0',
             # 'simplejpeg',
             'albumentations',
-            'pyro-ppl == 1.8.0',
+            'pyro-ppl >= 1.8.6',
             'torchmetrics == 0.11.0',
-            'timm == 0.6.12'
+            'timm == 0.9.10'
         ],
-        'pytorch_m1': [
+        'pytorch-m1': [
             # as above but without the +cpu (and the extra-index-url in readme has no effect)
             # all matching pytorch versions for an m1 system will be cpu
-            'torch == 1.12.1',
-            'torchvision == 0.13.1',
-            'torchaudio == 0.12.1',
-            'pytorch-lightning >= 2.0.0',
+            'torch == 2.1.0',
+            'torchvision == 0.16.0',
+            'torchaudio >= 2.1.0',
+            'lightning >= 2.0.0',
             'albumentations',
-            'pyro-ppl == 1.8.0',
+            'pyro-ppl >= 1.8.6',
             'torchmetrics == 0.11.0',
-            'timm == 0.6.12'
+            'timm >= 0.9.10'
         ],
         # as above but without pytorch itself
         # for GPU, you will also need e.g. cudatoolkit=11.3, 11.6
         # https://pytorch.org/get-started/previous-versions/#v1121
-        'pytorch_cu113': [
-            'torch == 1.12.1+cu113',
-            'torchvision == 0.13.1+cu113',
-            'torchaudio == 0.12.1',
-            'pytorch-lightning >= 2.0.0',
+        'pytorch-cu118': [
+            'torch == 2.1.0+cu118',
+            'torchvision == 0.16.0+cu118',
+            'torchaudio >= 2.1.0',
+            'lightning >= 2.0.0',
             'albumentations',
-            'pyro-ppl == 1.8.0',
+            'pyro-ppl >= 1.8.6',
             'torchmetrics == 0.11.0',
-            'timm == 0.6.12'
-        ],
-        'pytorch_colab': [
+            'timm >= 0.9.10'
+        ],  # exactly as above, but _cu121 for cuda 12.1 (the current default)
+        'pytorch-cu121': [
+            'torch == 2.1.0+cu121',
+            'torchvision == 0.16.0+cu121',
+            'torchaudio >= 2.1.0',
+            'lightning >= 2.0.0',
+            'albumentations',
+            'pyro-ppl >= 1.8.6',
+            'torchmetrics == 0.11.0',
+            'timm >= 0.9.10'
+        ],        
+        'pytorch-colab': [
             # colab includes pytorch already
-            'pytorch-lightning >= 2.0.0',
+            'lightning >= 2.0.0',
             'albumentations',
             'pyro-ppl>=1.8.0',
             'torchmetrics==0.11.0',
-            'timm == 0.6.12'
+            'timm >= 0.9.10',
+            'galaxy_datasets == 0.0.17'
         ],
         # TODO may add narval/Digital Research Canada config
-        'tensorflow': [
+        'tensorflow': [ # WARNING now deprecated
             'tensorflow == 2.10.0',  # 2.11.0 turns on XLA somewhere which then fails on multi-GPU...TODO
             'keras_applications',
             'tensorflow_probability == 0.18.0',  # 0.19 requires tf 2.11
             'protobuf <= 3.19'  # tensorflow incompatible above this (usually resolved by pip automatically)
         ],
         # for GPU, you will also need cudatoolkit=11.2 and cudnn=8.1.0 (note - 11.3 NOT supported by TF)
         # https://www.tensorflow.org/install/pip#step-by-step_instructions
@@ -82,15 +93,16 @@
             'boto3',    # for AWs s3 access
             'python-dateutil == 2.8.1',  # for boto3  
         ],
         'docs': [
             'Sphinx',
             'sphinxcontrib-napoleon',
             'furo',
-            'docutils<0.18'
+            'docutils<0.18',
+            'sphinxemoji'
         ]
     },
     install_requires=[
         'h5py',
         'tqdm',
         'pillow',
         'numpy',
@@ -98,11 +110,13 @@
         'scipy',
         'astropy',  # for reading fits
         'scikit-learn >= 1.0.2',
         'matplotlib',
         'pyarrow',  # to read parquet, which is very handy for big datasets
         # for saving metrics to weights&biases (cloud service, free within limits)
         'wandb',
+        'webdataset',  # for reading webdataset files
+        'huggingface_hub',  # login may be required
         'setuptools',  # no longer pinned
-        'galaxy-datasets>=0.0.15'  # for dataset loading in both TF and Torch (see github/mwalmsley/galaxy-datasets)
+        'galaxy-datasets>=0.0.17'  # for dataset loading in both TF and Torch (see github/mwalmsley/galaxy-datasets)
     ]
 )
```

### Comparing `zoobot-1.0.5/tests/test_loss_equivalence.py` & `zoobot-2.0.0/tests/test_loss_equivalence.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/pytorch/estimators/custom_layers.py` & `zoobot-2.0.0/zoobot/pytorch/estimators/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/pytorch/estimators/define_model.py` & `zoobot-2.0.0/zoobot/pytorch/estimators/define_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
 from functools import partial
 from typing import List
 
 import torch
 from torch import nn
 import pytorch_lightning as pl
-from torchmetrics import Accuracy
+import torchmetrics
 import timm
 
+from zoobot.shared import schemas
 from zoobot.pytorch.estimators import efficientnet_custom, custom_layers
-from zoobot.pytorch.training import losses
+from zoobot.pytorch.training import losses, schedulers
 
 # overall strategy
 # timm for defining complicated pytorch modules
 # manual modules for simple things (e.g. heads)
 # together, this give pure pytorch self.encoder and self.head
 # lightning modules with training instructions built out of those blocks (Zoobot, FinetuneableZooot)
 # FinetuneableZoobot could subclass Zoobot to have different optimisers/init args - first has arch stuff, second has optim stuff
@@ -51,64 +52,117 @@
 
     def __init__(
         self,
         *args,  # to be saved as hparams
         ):
         super().__init__()
         self.save_hyperparameters()  # saves all args by default
-        self.setup_metrics()
 
 
-    def setup_metrics(self):
-        # these are ignored unless output dim = 2
-        self.train_accuracy = Accuracy(task='binary')
-        self.val_accuracy = Accuracy(task='binary')
-        # self.log_on_step = False
-        # self.log_on_step is useful for debugging, but slower - best when log_every_n_steps is fairly large
+    def setup_metrics(self, nan_strategy='error'):  # may sometimes want to ignore nan even in main metrics
+        self.val_accuracy = torchmetrics.Accuracy(task='binary')
+
+        self.loss_metrics = torch.nn.ModuleDict({
+            'train/supervised_loss': torchmetrics.MeanMetric(nan_strategy=nan_strategy),
+            'validation/supervised_loss': torchmetrics.MeanMetric(nan_strategy=nan_strategy),
+            'test/supervised_loss': torchmetrics.MeanMetric(nan_strategy=nan_strategy),
+        })
+        
+        # TODO handle when schema doesn't exist
+        question_metric_dict = {}
+        for step_name in ['train', 'validation', 'test']:
+            question_metric_dict.update({
+                step_name + '/question_loss/' + question.text: torchmetrics.MeanMetric(nan_strategy='ignore')
+                for question in self.schema.questions
+            })
+        self.question_loss_metrics = torch.nn.ModuleDict(question_metric_dict)
+
+        campaigns = schema_to_campaigns(self.schema)
+        campaign_metric_dict = {}
+        for step_name in ['train', 'validation', 'test']:
+            campaign_metric_dict.update({
+                            step_name + '/campaign_loss/' + campaign: torchmetrics.MeanMetric(nan_strategy='ignore')
+                for campaign in campaigns
+            })
+        self.campaign_loss_metrics = torch.nn.ModuleDict(campaign_metric_dict)
 
 
     def forward(self, x):
+        assert x.shape[1] < 4  # torchlike BCHW
         x = self.encoder(x)
         return self.head(x)
     
-    def make_step(self, batch, batch_idx, step_name):
+    def make_step(self, batch, step_name):
         x, labels = batch
         predictions = self(x)  # by default, these are Dirichlet concentrations
-        loss = self.calculate_and_log_loss(predictions, labels, step_name)      
-        return {'loss': loss, 'predictions': predictions, 'labels': labels}
-
-    def calculate_and_log_loss(self, predictions, labels, step_name):
-        raise NotImplementedError('Must be subclassed')
+        loss = self.calculate_loss_and_update_loss_metrics(predictions, labels, step_name)      
+        outputs = {'loss': loss, 'predictions': predictions, 'labels': labels}
+        # self.update_other_metrics(outputs, step_name=step_name)
+        return outputs
 
     def configure_optimizers(self):
         raise NotImplementedError('Must be subclassed')
 
     def training_step(self, batch, batch_idx):
-        return self.make_step(batch, batch_idx, step_name='train')
-
-    def on_train_batch_end(self, outputs, *args):
-        self.log_outputs(outputs, step_name='train')
+        return self.make_step(batch, step_name='train')
 
     def validation_step(self, batch, batch_idx):
-        return self.make_step(batch, batch_idx, step_name='validation')
+        return self.make_step(batch, step_name='validation')
+    
+    def test_step(self, batch, batch_idx):
+        return self.make_step(batch, step_name='test')
+
+    # def on_train_batch_end(self, outputs, *args):
+    #     pass
 
-    def on_validation_batch_end(self, outputs, *args):
-        self.log_outputs(outputs, step_name='validation')
+    # def on_validation_batch_end(self, outputs, *args):
+    #     pass
 
-    def log_outputs(self, outputs, step_name):
+    def on_train_epoch_end(self) -> None:
+        # called *after* on_validation_epoch_end, confusingly
+        # do NOT log_all_metrics here. 
+        # logging a metric resets it, and on_validation_epoch_end just logged and reset everything, so you will only log nans
+        self.log_all_metrics(subset='train')
+
+    def on_validation_epoch_end(self) -> None:
+        self.log_all_metrics(subset='validation')
+
+    def on_test_epoch_end(self) -> None:
+        # logging.info('start test epoch end')
+        self.log_all_metrics(subset='test')
+        # logging.info('end test epoch end')
+    
+    def calculate_loss_and_update_loss_metrics(self, predictions, labels, step_name):
+        raise NotImplementedError('Must be subclassed')
+    
+    def update_other_metrics(self, outputs, step_name):
         raise NotImplementedError('Must be subclassed')
 
-    def test_step(self, batch, batch_idx):
-        return self.make_step(batch, batch_idx, step_name='test')
+    def log_all_metrics(self, subset=None):
+        if subset is not None:
+            for metric_collection in (self.loss_metrics, self.question_loss_metrics, self.campaign_loss_metrics):
+                prog_bar = metric_collection == self.loss_metrics
+                for name, metric in metric_collection.items():
+                    if subset in name:
+                        # logging.info(name)
+                        self.log(name, metric, on_epoch=True, on_step=False, prog_bar=prog_bar, logger=True)
+        else:  # just log everything
+            self.log_dict(self.loss_metrics, on_epoch=True, on_step=False, prog_bar=True, logger=True)
+            self.log_dict(self.question_loss_metrics, on_step=False, on_epoch=True, logger=True)
+            self.log_dict(self.campaign_loss_metrics, on_step=False, on_epoch=True, logger=True)
+
 
-    def on_test_batch_end(self, outputs, *args):
-         self.log_outputs(outputs, step_name='test')
 
     
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
+        # I can't work out how to get webdataset to return a single item im, not a tuple (im,).
+        # this is fine for training but annoying for predict
+        # help welcome. meanwhile, this works around it
+        if isinstance(batch, list) and len(batch) == 1:
+            return self(batch[0])
         # https://pytorch-lightning.readthedocs.io/en/stable/common/lightning_module.html#inference
         # this calls forward, while avoiding the need for e.g. model.eval(), torch.no_grad()
         # x, y = batch  # would be usual format, but here, batch does not include labels
         return self(batch)
 
 
 class ZoobotTree(GenericLightningModule):
@@ -119,78 +173,100 @@
     PyTorch LightningModule describing how to train the encoder and head (described below).
     Trains using Dirichlet loss. Labels should be num. volunteers giving each answer to each question. 
 
     See the code for exact training step, logging, etc - there's a lot of detail.
 
     Args:
         output_dim (int): Output dimension of model's head e.g. 34 for predicting a 34-answer decision tree.
-        question_index_groups (List): Mapping of which label indices are part of the same question. See :ref:`training_on_vote_counts`.
         architecture_name (str, optional): Architecture to use. Passed to timm. Must be in timm.list_models(). Defaults to "efficientnet_b0".
         channels (int, optional): Num. input channels. Probably 3 or 1. Defaults to 1.
-        use_imagenet_weights (bool, optional): Load weights pretrained on ImageNet (NOT galaxies!). Defaults to False.
         test_time_dropout (bool, optional): Apply dropout at test time, to pretend to be Bayesian. Defaults to True.
         timm_kwargs (dict, optional): passed to timm.create_model e.g. drop_path_rate=0.2 for effnet. Defaults to {}.
         learning_rate (float, optional): AdamW learning rate. Defaults to 1e-3.
     """
 
     # lightning only supports checkpoint loading / hparams which are not fancy classes
     # therefore, can't nicely wrap these arguments. So it goes.
     # override GenericLightningModule above, only this init
     def __init__(
         self,
         output_dim: int,
-        question_index_groups: List,
+        # in the simplest case, this is all zoobot needs: grouping of label col indices as questions
+        # question_index_groups: List=None,
+        # BUT
+        # if you pass these, it enables better per-question and per-survey logging (because we have names) 
+        # must be passed as simple dicts, not objects, so can't just pass schema in
+        question_answer_pairs: dict=None,
+        dependencies: dict=None,
         # encoder args
         architecture_name="efficientnet_b0",
         channels=1,
-        use_imagenet_weights=False,
+        # use_imagenet_weights=False,
         test_time_dropout=True,
+        compile_encoder=False,
         timm_kwargs={},  # passed to timm.create_model e.g. drop_path_rate=0.2 for effnet
         # head args
         dropout_rate=0.2,
         learning_rate=1e-3,  # PyTorch default
         # optim args
         betas=(0.9, 0.999),  # PyTorch default
         weight_decay=0.01,  # AdamW PyTorch default
         scheduler_params={}  # no scheduler by default
         ):
 
         # now, finally, can pass only standard variables as hparams to save
         # will still need to actually use these variables later, this super init only saves them
         super().__init__(
+            # these all do nothing, they are simply saved by lightning as hparams
             output_dim,
-            question_index_groups,
+            question_answer_pairs,
+            dependencies,
             architecture_name,
             channels,
             timm_kwargs,
+            compile_encoder,
             test_time_dropout,
             dropout_rate,
             learning_rate,
             betas,
             weight_decay,
             scheduler_params
         )
 
         logging.info('Generic __init__ complete - moving to Zoobot __init__')
 
+        # logging.info('question_index_groups/dependencies passed to Zoobot, constructing schema in __init__')
+        # assert question_index_groups is None,  "Don't pass both question_index_groups and question_answer_pairs/dependencies"
+        assert dependencies is not None
+        self.schema = schemas.Schema(question_answer_pairs, dependencies)
+        # replace with schema-derived version
+        question_index_groups = self.schema.question_index_groups
+
+        self.setup_metrics()
+
         # set attributes for learning rate, betas, used by self.configure_optimizers()
         # TODO refactor to optimizer params
         self.learning_rate = learning_rate
         self.betas = betas
         self.weight_decay = weight_decay
         self.scheduler_params = scheduler_params
 
         self.encoder = get_pytorch_encoder(
             architecture_name,
             channels,
-            use_imagenet_weights=use_imagenet_weights,
+            # use_imagenet_weights=use_imagenet_weights,
             **timm_kwargs
         )
+        if compile_encoder:
+            logging.warning('Using torch.compile on encoder')
+            self.encoder = torch.compile(self.encoder)
+
         # bit lazy assuming 224 input size
-        self.encoder_dim = get_encoder_dim(self.encoder, input_size=224, channels=channels)
+        # logging.warning(channels)
+        self.encoder_dim = get_encoder_dim(self.encoder, channels)
         # typically encoder_dim=1280 for effnetb0
         logging.info('encoder dim: {}'.format(self.encoder_dim))
 
 
         self.head = get_pytorch_dirichlet_head(
             self.encoder_dim,
             output_dim=output_dim,
@@ -199,23 +275,23 @@
         )
 
         self.loss_func = get_dirichlet_loss_func(question_index_groups)
 
         logging.info('Zoobot __init__ complete')
 
 
-    def calculate_and_log_loss(self, predictions, labels, step_name):
+    def calculate_loss_and_update_loss_metrics(self, predictions, labels, step_name):
         # self.loss_func returns shape of (galaxy, question), mean to ()
         multiq_loss = self.loss_func(predictions, labels, sum_over_questions=False)
-        # if hasattr(self, 'schema'):
-        self.log_loss_per_question(multiq_loss, prefix=step_name)
+        self.update_per_question_loss_metric(multiq_loss, step_name=step_name)
         # sum over questions and take a per-device mean
         # for DDP strategy, batch size is constant (batches are not divided, data pool is divided)
         # so this will be the global per-example mean
         loss = torch.mean(torch.sum(multiq_loss, axis=1))
+        self.loss_metrics[step_name + '/supervised_loss'](loss)
         return loss
 
 
     def configure_optimizers(self):
         # designed for training from scratch
         # parameters = list(self.head.parameters()) + list(self.encoder.parameters()) TODO should happen automatically?
         optimizer = torch.optim.AdamW(
@@ -228,39 +304,67 @@
             logging.info(f'Using Plateau scheduler with {self.scheduler_params}')
             # TODO could generalise this if needed
             scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(
                 optimizer, 
                 min_lr=1e-6,
                 patience=self.scheduler_params.get('patience', 5)
             )
-            return {'optimizer': optimizer, 'lr_scheduler': scheduler, 'monitor': 'validation/epoch_loss'}
+            return {'optimizer': optimizer, 'lr_scheduler': scheduler, 'monitor': 'validation/loss'}
+        elif self.scheduler_params.get('cosine_schedule', False):
+            logging.info('Using cosine schedule')
+            scheduler = schedulers.CosineWarmupScheduler(
+                optimizer=optimizer,
+                warmup_epochs=self.scheduler_params['warmup_epochs'],
+                max_epochs=self.scheduler_params['max_cosine_epochs'],
+                start_value=self.learning_rate,
+                end_value=self.learning_rate * self.scheduler_params['max_learning_rate_reduction_factor']
+            )
+            return {'optimizer': optimizer, 'lr_scheduler': scheduler, 'monitor': 'validation/loss'}
         else:
             logging.info('No scheduler used')
             return optimizer  # no scheduler
 
 
-    def log_outputs(self, outputs, step_name):
-        self.log("{}/epoch_loss".format(step_name), outputs['loss'], on_epoch=True, on_step=False,prog_bar=True, logger=True, sync_dist=True)
-        # if self.log_on_step:
-        #     # seperate call to allow for different name, to allow for consistency with TF.keras auto-names
-        #     self.log(
-        #         "{}/step_loss".format(step_name), outputs['loss'], on_epoch=False, on_step=True, prog_bar=True, logger=True, sync_dist=True)
-        if outputs['predictions'].shape[1] == 2:  # will only do for binary classifications
-            # logging.info(predictions.shape, labels.shape)
-            self.log(
-                "{}_accuracy".format(step_name), self.train_accuracy(outputs['predictions'], torch.argmax(outputs['labels'], dim=1, keepdim=False)), prog_bar=True, sync_dist=True)
-
 
-    def log_loss_per_question(self, multiq_loss, prefix):
+    def update_per_question_loss_metric(self, multiq_loss, step_name):
         # log questions individually
         # TODO need schema attribute or similar to have access to question names, this will do for now
         # unlike Finetuneable..., does not use TorchMetrics, simply logs directly
         # TODO could use TorchMetrics and for q in schema, self.q_metric loop
-        for question_n in range(multiq_loss.shape[1]):
-            self.log(f'{prefix}/epoch_questions/question_{question_n}_loss:0', torch.mean(multiq_loss[:, question_n]), on_epoch=True, on_step=False, sync_dist=True)
+
+        # if hasattr(self, 'schema'):
+            # use schema metadata to log intelligently
+            # will have schema if question_answer_pairs and dependencies are passed to __init__
+            # assume that questions are named like smooth-or-featured-CAMPAIGN
+        for question_n, question in enumerate(self.schema.questions):
+            # for logging comparison, want to ignore loss on unlablled examples, i.e. take mean ignoring zeros
+            # could sum, but then this would vary with batch size
+            nontrivial_loss_mask = multiq_loss[:, question_n] > 0  # 'zero' seems to be ~5e-5 floor in practice
+
+            this_question_metric = self.question_loss_metrics[step_name + '/question_loss/' + question.text]
+            # raise ValueError
+            this_question_metric(torch.mean(multiq_loss[nontrivial_loss_mask, question_n]))
+
+        campaigns = schema_to_campaigns(self.schema)
+        for campaign in campaigns:
+            campaign_questions = [q for q in self.schema.questions if campaign in q.text]
+            campaign_q_indices = [self.schema.questions.index(q) for q in campaign_questions]  # shape (num q in this campaign e.g. 10)
+
+            # similarly to per-question, only include in mean if (any) q in this campaign has a non-trivial loss
+            nontrivial_loss_mask = multiq_loss[:, campaign_q_indices].sum(axis=1) > 0 # shape batch size
+
+            this_campaign_metric = self.campaign_loss_metrics[step_name + '/campaign_loss/' + campaign]
+            this_campaign_metric(torch.mean(multiq_loss[nontrivial_loss_mask][:, campaign_q_indices]))
+
+    # else:
+    #     # fallback to logging with question_n
+    #     for question_n in range(multiq_loss.shape[1]):
+    #         self.log(f'{step_name}/questions/question_{question_n}_loss:0', torch.mean(multiq_loss[:, question_n]), on_epoch=True, on_step=False, sync_dist=True)
+        
+            
 
 
     
 
 def get_dirichlet_loss_func(question_index_groups):
     # This just adds schema.question_index_groups as an arg to the usual (labels, preds) loss arg format
     # Would use lambda but multi-gpu doesn't support as lambda can't be pickled
@@ -270,30 +374,42 @@
     # accept (labels, preds), return losses of shape (batch, question)
 def dirichlet_loss(preds, labels, question_index_groups, sum_over_questions=False):
     # pytorch convention is preds, labels for loss func
     # my and sklearn convention is labels, preds for loss func
 
     # multiquestion_loss returns loss of shape (batch, question)
     # torch.sum(multiquestion_loss, axis=1) gives loss of shape (batch). Equiv. to non-log product of question likelihoods.
-    multiq_loss = losses.calculate_multiquestion_loss(labels, preds, question_index_groups)
+    multiq_loss = losses.calculate_multiquestion_loss(labels, preds, question_index_groups, careful=True)
     if sum_over_questions:
         return torch.sum(multiq_loss, axis=1)
     else:
         return multiq_loss
 
 
-def get_encoder_dim(encoder, input_size, channels):
-    x = torch.randn(1, channels, input_size, input_size)  # batch size of 1
-    return encoder(x).shape[-1]
-
+# input_size doesn't matter as long as it's large enough to not be pooled to zero
+# channels doesn't matter at all but has to match encoder channels or shape error
+def get_encoder_dim(encoder, channels=3):
+    device = next(encoder.parameters()).device
+    try:
+        x = torch.randn(2, channels, 224, 224, device=device) # BCHW
+        return encoder(x).shape[-1]
+    except RuntimeError as e:
+        if 'channels instead' in str(e):
+            logging.info('encoder dim search failed on channels, trying with channels=1')
+            channels = 1
+            x = torch.randn(2, channels, 224, 224, device=device) # BCHW
+            return encoder(x).shape[-1]
+        else:
+            raise e
 
+        
 def get_pytorch_encoder(
     architecture_name='efficientnet_b0',
     channels=1,
-    use_imagenet_weights=False,
+    # use_imagenet_weights=False,
     **timm_kwargs
     ) -> nn.Module:
     """
     Create a trainable efficientnet model.
     First layers are galaxy-appropriate augmentation layers - see :meth:`zoobot.estimators.define_model.add_augmentation_layers`.
     Expects single channel image e.g. (300, 300, 1), likely with leading batch dimension.
 
@@ -312,20 +428,24 @@
         channels (int, default 1): Number of channels i.e. C in NHWC-dimension inputs. 
 
     Returns:
         torch.nn.Sequential: trainable efficientnet model including augmentations and optional head
     """
     # num_classes=0 gives pooled encoder
     # https://github.com/rwightman/pytorch-image-models/blob/main/timm/models/efficientnet.py
+
+    # if architecture_name == 'toy':
+    #     logging.warning('Using toy encoder')
+    #     return ToyEncoder()
     
     # support older code that didn't specify effnet version
     if architecture_name == 'efficientnet':
         logging.warning('efficientnet variant not specified - please set architecture_name=efficientnet_b0 (or similar)')
         architecture_name = 'efficientnet_b0'
-    return timm.create_model(architecture_name, in_chans=channels, num_classes=0, pretrained=use_imagenet_weights, **timm_kwargs)
+    return timm.create_model(architecture_name, in_chans=channels, num_classes=0, **timm_kwargs)
 
 
 def get_pytorch_dirichlet_head(encoder_dim: int, output_dim: int, test_time_dropout: bool, dropout_rate: float) -> torch.nn.Sequential:
     """
     Head to combine with encoder (above) when predicting Galaxy Zoo decision tree answers.
     Pytorch Sequential model.
     Predicts Dirichlet concentration parameters.
@@ -353,7 +473,21 @@
         logging.info('Not using test-time dropout')
         dropout_layer = torch.nn.Dropout
     modules_to_use.append(dropout_layer(dropout_rate))
     # TODO could optionally add a bottleneck layer here
     modules_to_use.append(efficientnet_custom.custom_top_dirichlet(encoder_dim, output_dim))
 
     return nn.Sequential(*modules_to_use)
+
+
+def schema_to_campaigns(schema):
+    # e.g. [gz2, dr12, ...]
+    return [question.text.split('-')[-1] for question in schema.questions]
+
+
+if __name__ == '__main__':
+    encoder = get_pytorch_encoder(channels=1)
+    dim = get_encoder_dim(encoder, channels=1)
+    print(dim)
+
+
+    ZoobotTree.load_from_checkpoint
```

### Comparing `zoobot-1.0.5/zoobot/pytorch/estimators/efficientnet_custom.py` & `zoobot-2.0.0/zoobot/pytorch/estimators/efficientnet_custom.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/pytorch/manchester.py` & `zoobot-2.0.0/zoobot/pytorch/manchester.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 import logging
+import os
 
-from lightning_lite.plugins.environments import SLURMEnvironment
 
-# https://pytorch-lightning.readthedocs.io/en/stable/_modules/lightning_lite/plugins/environments/slurm.html#SLURMEnvironment
-# https://github.com/Lightning-AI/lightning/blob/9c20cad40e4142f8a5e945fe26e919e598f2bd56/src/lightning_lite/plugins/environments/slurm.py
-class ManchesterEnvironment(SLURMEnvironment):
-
-    def __init__(self, auto_requeue: bool = True, requeue_signal=None) -> None:
-        logging.info('Using Manchester SLURM environment')
-        super().__init__(auto_requeue, requeue_signal)
-
-    # @staticmethod
-    # def resolve_root_node_address(nodes: str) -> str:
-    #     root_node_address = super().resolve_root_node_address(nodes)
-    #     logging.info(f'root_node_address: {root_node_address}')
-    #     return root_node_address
-
-    @staticmethod
-    def detect() -> bool:
-        return True
+# from lightning_lite.plugins.environments import SLURMEnvironment
+
+# # https://pytorch-lightning.readthedocs.io/en/stable/_modules/lightning_lite/plugins/environments/slurm.html#SLURMEnvironment
+# # https://github.com/Lightning-AI/lightning/blob/9c20cad40e4142f8a5e945fe26e919e598f2bd56/src/lightning_lite/plugins/environments/slurm.py
+# class ManchesterEnvironment(SLURMEnvironment):
+
+#     def __init__(self, auto_requeue: bool = True, requeue_signal=None) -> None:
+#         logging.info('Using Manchester SLURM environment')
+#         super().__init__(auto_requeue, requeue_signal)
+
+#     # @staticmethod
+#     # def resolve_root_node_address(nodes: str) -> str:
+#     #     root_node_address = super().resolve_root_node_address(nodes)
+#     #     logging.info(f'root_node_address: {root_node_address}')
+#     #     return root_node_address
+
+#     @staticmethod
+#     def detect() -> bool:
+#         return True
         
-    @property
-    def main_port(self) -> int:
-        main_port = super().main_port
-        logging.info(f'main_port: {main_port}')
-        return main_port
-        # MASTER_PORT will override
+#     @property
+#     def main_port(self) -> int:
+#         main_port = super().main_port
+#         logging.info(f'main_port: {main_port}')
+#         return main_port
+#         # MASTER_PORT will override
+
+
+from pytorch_lightning.plugins.environments import SLURMEnvironment
+class GalahadEnvironment(SLURMEnvironment):
+    def __init__(self, **kwargs):
+        ntasks_per_node = os.environ["SLURM_TASKS_PER_NODE"].split("(")[0]
+        os.environ["SLURM_NTASKS_PER_NODE"] = ntasks_per_node
+        logging.warning(f'Within custom slurm environment, --n-tasks-per-node={ntasks_per_node}')
+        # os.environ["SLURM_NTASKS"] = str(os.environ["SLURM_NTASKS_PER_NODE"])
+        super().__init__(**kwargs)
+        self.nnodes = int(os.environ["SLURM_NNODES"])
+
 
-if __name__ == '__main__':
+# if __name__ == '__main__':
 
-    logging.basicConfig(level=logging.INFO)
+#     logging.basicConfig(level=logging.INFO)
 
-    # slurm_nodelist = "compute-0-[0,9]" # 0,9 works
-    slurm_nodelist = "compute-0-[0,11]"  # 0,11 hangs
-    # 70017 8-9 works
+#     # slurm_nodelist = "compute-0-[0,9]" # 0,9 works
+#     slurm_nodelist = "compute-0-[0,11]"  # 0,11 hangs
+#     # 70017 8-9 works
 
-    env = ManchesterEnvironment()
-    root = env.resolve_root_node_address(slurm_nodelist)
-    print(root)
+#     env = GalahadEnvironment()
+#     root = env.resolve_root_node_address(slurm_nodelist)
+#     print(root)
 
-    print(env.detect())
+#     print(env.detect())
 
-    print(env.main_port)
+#     print(env.main_port)
```

### Comparing `zoobot-1.0.5/zoobot/pytorch/predictions/predict_on_catalog.py` & `zoobot-2.0.0/zoobot/pytorch/predictions/predict_on_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,22 +34,22 @@
         # 
         **datamodule_kwargs  # e.g. batch_size, resize_size, crop_scale_bounds, etc.
     )
     # with this stage arg, will only use predict_catalog 
     # crucial to specify the stage, or will error (as missing other catalogs)
     predict_datamodule.setup(stage='predict')  
     # for images in predict_datamodule.predict_dataloader():
-    #     print(images)
-    #     print(images.shape)
+        # print(images)
+        # print(images.shape)
+        # exit()
 
 
     # set up trainer (again)
     trainer = pl.Trainer(
         max_epochs=-1,  # does nothing in this context, suppresses warning
-        inference_mode=True,  # no grads needed
         **trainer_kwargs  # e.g. gpus
     )
 
     # from here, very similar to tensorflow version - could potentially refactor
 
     logging.info('Beginning predictions')
     start = datetime.datetime.fromtimestamp(time.time())
@@ -81,7 +81,9 @@
         save_predictions.predictions_to_csv(predictions, image_id_strs, label_cols, save_loc)
 
     logging.info(f'Predictions saved to {save_loc}')
 
     end = datetime.datetime.fromtimestamp(time.time())
     logging.info('Completed at: {}'.format(end.strftime('%Y-%m-%d %H:%M:%S')))
     logging.info('Time elapsed: {}'.format(end - start))
+
+    return predictions
```

### Comparing `zoobot-1.0.5/zoobot/pytorch/training/losses.py` & `zoobot-2.0.0/zoobot/pytorch/training/losses.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 from typing import Tuple
+import logging
 
 import torch
 import pyro
 
 
-def calculate_multiquestion_loss(labels: torch.Tensor, predictions: torch.Tensor, question_index_groups: Tuple) -> torch.Tensor:
+def calculate_multiquestion_loss(labels: torch.Tensor, predictions: torch.Tensor, question_index_groups: Tuple, careful=True) -> torch.Tensor:
     """
     The full decision tree loss used for training GZ DECaLS models
 
     Negative log likelihood of observing ``labels`` (volunteer answers to all questions)
     from Dirichlet-Multinomial distributions for each question, using concentrations ``predictions``.
     
     Args:
         labels (torch.Tensor): (galaxy, k successes) where k successes dimension is indexed by question_index_groups.
         predictions (torch.Tensor):  Dirichlet concentrations, matching shape of labels
-        question_index_groups (list): Paired (tuple) integers of (first, last) indices of answers to each question, listed for all questions. See :ref:`schemas`.
+        question_index_groups (list): Answer indices for each question i.e. [(question.start_index, question.end_index), ...] for all questions. Useful for slicing model predictions by question. See :ref:`schemas`.
     
     Returns:
         torch.Tensor: neg. log likelihood of shape (batch, question).
     """
+    if careful:
+        # some models give occasional nans for all predictions on a specific galaxy/row
+        # these are inputs to the loss and only happen many epochs in so probably not a case of bad labels, but rather some instability during training
+        # handle this by setting loss=0 for those rows and throwing a warning
+        nan_prediction = torch.isnan(predictions) | torch.isinf(predictions)
+        if nan_prediction.any():
+            logging.warning(f'Found nan values in predictions: {predictions}')
+        safety_value = torch.ones(1, device=predictions.device, dtype=predictions.dtype)  # fill with 1 everywhere i.e. fully uncertain
+        predictions = torch.where(condition=nan_prediction, input=safety_value, other=predictions)
+
     # very important that question_index_groups is fixed and discrete, else tf.function autograph will mess up 
     q_losses = []
     # will give shape errors if model output dim is not labels dim, which can happen if losses.py substrings are missing an answer
     for q_n in range(len(question_index_groups)):
         q_indices = question_index_groups[q_n]
         q_start = q_indices[0]
         q_end = q_indices[1]
-
         q_loss = dirichlet_loss(labels[:, q_start:q_end+1], predictions[:, q_start:q_end+1])
 
         q_losses.append(q_loss)
     
     total_loss = torch.stack(q_losses, axis=1)
 
     return total_loss  # leave the reduction to pytorch lightning
@@ -50,15 +60,14 @@
         tf.constant: negative log. prob per galaxy, of shape (batch_dim).
     """
     # if you get a dimension mismatch here like [16, 2] vs. [64, 2], for example, check --shard-img-size is correct in train_model.py.
     # images may be being reshaped to the wrong expected size e.g. if they are saved as 32x32, but you put --shard-img-size=64,
     # you will get image batches of shape [N/4, 64, 64, 1] and hence have the wrong number of images vs. labels (and meaningless images)
     # so check --shard-img-size carefully!
     total_count = torch.sum(labels_for_q, axis=1)
-    # logging.info(total_count)
 
     # pytorch dirichlet multinomial implementation will not accept zero total votes, need to handle separately
     return get_dirichlet_neg_log_prob(labels_for_q, total_count, concentrations_for_q)
 
 
     # # return tf.where(
     # #     tf.math.equal(total_count, 0),  # if total_count is 0 (i.e. no votes)
@@ -101,9 +110,11 @@
 
 
     # # return get_dirichlet_neg_log_prob(labels_for_q, total_count, concentrations_for_q)
 
 
 def get_dirichlet_neg_log_prob(labels_for_q, total_count, concentrations_for_q):
     # https://docs.pyro.ai/en/stable/distributions.html#dirichletmultinomial
-    dist = pyro.distributions.DirichletMultinomial(total_count=total_count, concentration=concentrations_for_q, is_sparse=False)
-    return -dist.log_prob(labels_for_q)  # important minus sign
+    # .int()s avoid rounding errors causing loss of around 1e-5 for questions with 0 votes
+    dist = pyro.distributions.DirichletMultinomial(
+        total_count=total_count.int(), concentration=concentrations_for_q, is_sparse=False, validate_args=True)
+    return -dist.log_prob(labels_for_q.int())  # important minus sign
```

### Comparing `zoobot-1.0.5/zoobot/pytorch/training/tensorboard_writers.py` & `zoobot-2.0.0/zoobot/pytorch/training/tensorboard_writers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/pytorch/training/train_with_pytorch_lightning.py` & `zoobot-2.0.0/zoobot/pytorch/training/train_with_pytorch_lightning.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,143 +1,162 @@
 import logging
 import os
 from typing import Tuple
 
 import torch
 import pytorch_lightning as pl
+from pytorch_lightning.plugins import TorchSyncBatchNorm
 from pytorch_lightning.strategies.ddp import DDPStrategy
 from pytorch_lightning.callbacks import ModelCheckpoint
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
+from pytorch_lightning.loggers import CSVLogger
 
 from galaxy_datasets.pytorch.galaxy_datamodule import GalaxyDataModule
 
 from zoobot.pytorch.estimators import define_model
+from zoobot.pytorch.datasets import webdatamodule
+
 
 
 def train_default_zoobot_from_scratch(    
     # absolutely crucial arguments
     save_dir: str,  # save model here
     schema,  # answer these questions
     # input data - specify *either* catalog (to be split) or the splits themselves
     catalog=None,
     train_catalog=None,
     val_catalog=None,
     test_catalog=None,
+    train_urls=None,
+    val_urls=None,
+    test_urls=None,
+    cache_dir=None,  # only works with webdataset urls
     # training time parameters
     epochs=1000,
     patience=8,
     # model hparams
-    architecture_name='efficientnet_b0',  # recently changed
+    architecture_name='efficientnet_b0',
+    timm_kwargs = {}, # e.g. {'drop_path_rate': 0.2, 'num_features': 1280}. Passed to timm model init method, depends on arch.
     batch_size=128,
     dropout_rate=0.2,
-    drop_connect_rate=0.2,
     learning_rate=1e-3,
     betas=(0.9, 0.999),
     weight_decay=0.01,
     scheduler_params={},
     # data and augmentation parameters
     color=False,
     resize_after_crop=224,
     crop_scale_bounds=(0.7, 0.8),
     crop_ratio_bounds=(0.9, 1.1),
     # hardware parameters
     nodes=1,
     gpus=2,
+    sync_batchnorm=False,
     num_workers=4,
     prefetch_factor=4,
     mixed_precision=False,
+    compile_encoder=False,
     # checkpointing / logging
     wandb_logger=None,
     checkpoint_file_template=None,
     auto_insert_metric_name=True,
     save_top_k=3,
     extra_callbacks=None,
     # replication parameters
     random_state=42
 ) -> Tuple[define_model.ZoobotTree, pl.Trainer]:
     """
     Train Zoobot from scratch on a big galaxy catalog.
-    Zoobot is a base deep learning model (anything from timm, typically a CNN) plus a dirichlet head.
-    Images are augmented using the default transforms (flips, rotations, zooms)
-    from `the galaxy-datasets repo <https://github.com/mwalmsley/galaxy-datasets/blob/main/galaxy_datasets/transforms.py>`_.
-
-    Once trained, Zoobot can be finetuned to new data.
-    For finetuning, see zoobot/pytorch/training/finetune.py.
-    Many pretrained models are already available - see :ref:`datanotes`.
+
+    **You don't need to use this**. 
+    Training from scratch is becoming increasingly complicated (as you can see from the arguments) due to ongoing research on the best methods.
+    This will be refactored to a dedicated "foundation" repo.
 
     Args:
         save_dir (str): folder to save training logs and trained model checkpoints
+        schema (shared.schemas.Schema): Schema object with label_cols, question_answer_pairs, and dependencies
         catalog (pd.DataFrame, optional): Galaxy catalog with columns `id_str` and `file_loc`. Will be automatically split to train and val (no test). Defaults to None. 
         train_catalog (pd.DataFrame, optional): As above, but already split by you for training. Defaults to None.
         val_catalog (pd.DataFrame, optional): As above, for validation. Defaults to None.
         test_catalog (pd.DataFrame, optional): As above, for testing. Defaults to None.
+        train_urls (list, optional): List of URLs to webdatasets for training. Defaults to None.
+        val_urls (list, optional): List of URLs to webdatasets for validation. Defaults to None.
+        test_urls (list, optional): List of URLs to webdatasets for testing. Defaults to None.
+        cache_dir (str, optional): Directory to cache webdatasets. Defaults to None.
         epochs (int, optional): Max. number of epochs to train for. Defaults to 1000.
         patience (int, optional): Max. number of epochs to wait for any loss improvement before ending training. Defaults to 8.
         architecture_name (str, optional): Architecture to use. Passed to timm. Must be in timm.list_models(). Defaults to 'efficientnet_b0'.
+        timm_kwargs (dict, optional): Additional kwargs to pass to timm model init method, for example {'drop_connect_rate': 0.2}. Defaults to {}.
+        batch_size (int, optional): Batch size. Defaults to 128.
         dropout_rate (float, optional): Randomly drop activations prior to the output layer, with this probability. Defaults to 0.2.
-        drop_connect_rate (float, optional): Randomly drop blocks with this probability, for regularisation. For supported timm models only. Defaults to 0.2.
         learning_rate (float, optional): Base learning rate for AdamW. Defaults to 1e-3.
         betas (tuple, optional): Beta args (i.e. momentum) for adamW. Defaults to (0.9, 0.999).
         weight_decay (float, optional): Weight decay arg (i.e. L2 penalty) for AdamW. Defaults to 0.01.
-        scheduler_params (dict, optional): Specify a learning rate scheduler. See code. Not recommended with AdamW. Defaults to {}.
+        scheduler_params (dict, optional): Specify a learning rate scheduler. See code below. Defaults to {}.
         color (bool, optional): Train on RGB images rather than channel-averaged. Defaults to False.
         resize_after_crop (int, optional): Input image size. After all transforms, images will be resized to this size. Defaults to 224.
         crop_scale_bounds (tuple, optional): Off-center crop fraction (<1 means zoom in). Defaults to (0.7, 0.8).
         crop_ratio_bounds (tuple, optional): Aspect ratio of crop above. Defaults to (0.9, 1.1).
         nodes (int, optional): Multi-node training Unlikely to work on your cluster without tinkering. Defaults to 1 (i.e. one node).
         gpus (int, optional): Multi-GPU training. Uses distributed data parallel - essentially, full dataset is split by GPU. See torch docs. Defaults to 2.
+        sync_batchnorm (bool, optional): Use synchronized batchnorm. Defaults to False.
         num_workers (int, optional): Processes for loading data. See torch dataloader docs. Should be < num cpus. Defaults to 4.
         prefetch_factor (int, optional): Num. batches to queue in memory per dataloader. See torch dataloader docs. Defaults to 4.
         mixed_precision (bool, optional): Use (mostly) half-precision to halve memory requirements. May cause instability. See Lightning Trainer docs. Defaults to False.
+        compile_encoder (bool, optional): Compile the encoder with torch.compile (new in torch v2). Defaults to False.
         wandb_logger (pl.loggers.wandb.WandbLogger, optional): Logger to track experiments on Weights and Biases. Defaults to None.
         checkpoint_file_template (str, optional): formatting for checkpoint filename. See Lightning docs. Defaults to None.
         auto_insert_metric_name (bool, optional): escape "/" in metric names when naming checkpoints. See Lightning docs. Defaults to True.
         save_top_k (int, optional): Keep the k best checkpoints. See Lightning docs. Defaults to 3.
+        extra_callbacks (list, optional): Additional callbacks to pass to the Trainer. Defaults to None.
         random_state (int, optional): Seed. Defaults to 42.
 
     Returns:
         Tuple[define_model.ZoobotTree, pl.Trainer]: Trained ZoobotTree model, and Trainer with which it was trained.
     """
 
     # some optional logging.debug calls recording cluster environment
     slurm_debugging_logs()
 
     # redundant when already called before this, but no harm doing twice
     pl.seed_everything(random_state)
 
     assert save_dir is not None
     if not os.path.isdir(save_dir):
-        os.mkdir(save_dir)
+        try:
+            os.mkdir(save_dir)
+        except FileExistsError:
+            pass # another gpu process may have just made it
+    logging.info(f'Saving to {save_dir}')
 
     if color:
         logging.warning(
             'Training on color images, not converting to greyscale')
         channels = 3
     else:
         logging.info('Converting images to greyscale before training')
         channels = 1
 
     strategy = 'auto'
     plugins = None
     if (gpus is not None) and (gpus > 1):
         strategy = DDPStrategy(find_unused_parameters=False)  # static_graph=True TODO
         logging.info('Using multi-gpu training')
-        if nodes > 1:  # I assume nobody is doing multi-node cpu training...
-            logging.info('Using multi-node training')  # purely for your info
+        # if nodes > 1:  # I assume nobody is doing multi-node cpu training...
+            # logging.info('Using multi-node training')  # purely for your info
             # this is only needed for multi-node training
             # our cluster sets TASKS_PER_NODE not NTASKS_PER_NODE
             # (with srun, SLURM_STEP_TASKS_PER_NODE)
             # https://slurm.schedmd.com/srun.html#OPT_SLURM_STEP_TASKS_PER_NODE
-            if 'SLURM_NTASKS_PER_NODE' not in os.environ.keys():
-                os.environ['SLURM_NTASKS_PER_NODE'] = os.environ['SLURM_TASKS_PER_NODE']
-                # from lightning_lite.plugins.environments import SLURMEnvironment
-                from zoobot.pytorch import manchester
-                logging.warning('Using custom slurm environment')
-                # https://pytorch-lightning.readthedocs.io/en/stable/clouds/cluster_advanced.html#enable-auto-wall-time-resubmitions
-                plugins = [manchester.ManchesterEnvironment(auto_requeue=False)]
+        if 'SLURM_NTASKS_PER_NODE' not in os.environ.keys():
+            os.environ['SLURM_NTASKS_PER_NODE'] = os.environ['SLURM_TASKS_PER_NODE']
+            from zoobot.pytorch import manchester
+            logging.warning(f'Using custom slurm environment, --n-tasks-per-node={os.environ["SLURM_NTASKS_PER_NODE"]}')
+            # https://pytorch-lightning.readthedocs.io/en/stable/clouds/cluster_advanced.html#enable-auto-wall-time-resubmitions
+            plugins = [manchester.GalahadEnvironment(auto_requeue=False)]
 
     if gpus > 0:
         accelerator = 'gpu'
         devices = gpus
     else:
         accelerator = 'cpu'
         devices = 'auto'  # all
@@ -163,30 +182,14 @@
     if num_workers > os.cpu_count():
         logging.warning(
             """num_workers > num cpu.
             You may be spawning more dataloader workers than you have cpus, causing bottlenecks.
             Suggest reducing num_workers."""
         )
         
-    
-    if catalog is not None:
-        assert train_catalog is None
-        assert val_catalog is None
-        assert test_catalog is None
-        catalogs_to_use = {
-            'catalog': catalog
-        }
-    else:
-        assert catalog is None
-        catalogs_to_use = {
-            'train_catalog': train_catalog,
-            'val_catalog': val_catalog,
-            'test_catalog': test_catalog  # may be None
-        }
-
     if wandb_logger is not None:
         wandb_logger.log_hyperparams({
             'random_state': random_state,
             'epochs': epochs,
             'accelerator': accelerator,
             'gpus': gpus,
             'nodes': nodes,
@@ -196,106 +199,163 @@
             'crop_scale_bounds': crop_scale_bounds,
             'crop_ratio_bounds': crop_ratio_bounds,
             'resize_after_crop': resize_after_crop,
             'num_workers': num_workers,
             'prefetch_factor': prefetch_factor,
             'framework': 'pytorch'
         })
+    else:
+        logging.warning('No wandb_logger passed. Using CSV logging only')
+        wandb_logger = CSVLogger(save_dir=save_dir)
 
-    datamodule = GalaxyDataModule(
-        label_cols=schema.label_cols,
-        # can take either a catalog (and split it), or a pre-split catalog
-        **catalogs_to_use,
-        # augmentations parameters
-        greyscale=not color,
-        crop_scale_bounds=crop_scale_bounds,
-        crop_ratio_bounds=crop_ratio_bounds,
-        resize_after_crop=resize_after_crop,
-        # hardware parameters
-        batch_size=batch_size, # on 2xA100s, 256 with DDP, 512 with distributed (i.e. split batch)
-        num_workers=num_workers,
-        prefetch_factor=prefetch_factor
-    )
+    # work out what dataset the user has passed
+    single_catalog = catalog is not None
+    split_catalogs = train_catalog is not None
+    webdatasets = train_urls is not None
+
+    if single_catalog or split_catalogs:
+        # this branch will use GalaxyDataModule to load catalogs
+        assert not webdatasets
+        if single_catalog:
+            assert not split_catalogs
+            data_to_use = {
+                'catalog': catalog
+            }
+        else:
+            data_to_use = {
+                'train_catalog': train_catalog,
+                'val_catalog': val_catalog,
+                'test_catalog': test_catalog  # may be None
+            }
+        datamodule = GalaxyDataModule(
+            label_cols=schema.label_cols,
+            # can take either a catalog (and split it), or a pre-split catalog
+            **data_to_use,
+            # augmentations parameters
+            greyscale=not color,
+            crop_scale_bounds=crop_scale_bounds,
+            crop_ratio_bounds=crop_ratio_bounds,
+            resize_after_crop=resize_after_crop,
+            # hardware parameters
+            batch_size=batch_size, # on 2xA100s, 256 with DDP, 512 with distributed (i.e. split batch)
+            num_workers=num_workers,
+            prefetch_factor=prefetch_factor
+        )
+    else:
+        # this branch will use WebDataModule to load premade webdatasets
+
+        # temporary: use SSL-like transform
+        # from foundation.models import transforms
+        # train_transform_cfg = transforms.default_view_config()
+        # inference_transform_cfg = transforms.minimal_view_config()
+        # train_transform_cfg.output_size = resize_after_crop
+        # inference_transform_cfg.output_size = resize_after_crop
+
+        datamodule = webdatamodule.WebDataModule(
+            train_urls=train_urls,
+            val_urls=val_urls,
+            test_urls=test_urls,
+            label_cols=schema.label_cols,
+            # hardware
+            batch_size=batch_size,
+            num_workers=num_workers,
+            prefetch_factor=prefetch_factor,
+            cache_dir=cache_dir,
+            # augmentation args
+            greyscale=not color,
+            crop_scale_bounds=crop_scale_bounds,
+            crop_ratio_bounds=crop_ratio_bounds,
+            resize_after_crop=resize_after_crop,
+            # temporary: use SSL-like transform
+            # train_transform=transforms.GalaxyViewTransform(train_transform_cfg),
+            # inference_transform=transforms.GalaxyViewTransform(inference_transform_cfg),
+        )
+
+    # debug - check range of loaded images, should be 0-1
     datamodule.setup(stage='fit')
+    for (images, _) in datamodule.train_dataloader():
+        logging.info(f'Using batches of {images.shape[0]} images for training')
+        logging.info('First batch image min/max: {}/{}'.format(images.min(), images.max()))
+        assert images.max() <= 1.0
+        assert images.min() >= 0.0
+        break
+    # exit()
 
     # these args are automatically logged
     lightning_model = define_model.ZoobotTree(
         output_dim=len(schema.label_cols),
-        question_index_groups=schema.question_index_groups,
+        # NEW - pass these from schema, for better logging
+        question_answer_pairs=schema.question_answer_pairs,
+        dependencies=schema.dependencies,
         architecture_name=architecture_name,
         channels=channels,
-        use_imagenet_weights=False,
         test_time_dropout=True,
         dropout_rate=dropout_rate,
         learning_rate=learning_rate,
-        timm_kwargs={'drop_path_rate': drop_connect_rate},
+        # https://github.com/huggingface/pytorch-image-models/blob/main/timm/models/efficientnet.py#L75C9-L75C17
+        timm_kwargs=timm_kwargs,
+        compile_encoder=compile_encoder,
         betas=betas,
         weight_decay=weight_decay,
         scheduler_params=scheduler_params
     )
+
+    if sync_batchnorm:
+        logging.info('Using sync batchnorm')
+        lightning_model = TorchSyncBatchNorm().apply(lightning_model)
+    
     
     extra_callbacks = extra_callbacks if extra_callbacks else []
 
+    monitor_metric = 'validation/supervised_loss'
+
     # used later for checkpoint_callback.best_model_path
     checkpoint_callback = ModelCheckpoint(
             dirpath=os.path.join(save_dir, 'checkpoints'),
-            monitor="validation/epoch_loss",
+            monitor=monitor_metric,
             save_weights_only=True,
             mode='min',
             # custom filename for checkpointing due to / in metric
             filename=checkpoint_file_template,
             # https://pytorch-lightning.readthedocs.io/en/stable/api/pytorch_lightning.callbacks.ModelCheckpoint.html#pytorch_lightning.callbacks.ModelCheckpoint.params.auto_insert_metric_name
             # avoids extra folders from the checkpoint name
             auto_insert_metric_name=auto_insert_metric_name,
             save_top_k=save_top_k
     )
 
-    early_stopping_callback = EarlyStopping(monitor='validation/epoch_loss', patience=patience, check_finite=True)
-
+    early_stopping_callback = EarlyStopping(monitor=monitor_metric, patience=patience, check_finite=True)
     callbacks = [checkpoint_callback, early_stopping_callback] + extra_callbacks
 
     trainer = pl.Trainer(
-        log_every_n_steps=150,  # at batch 512 (A100 MP max), DR5 has ~161 train steps
+        num_sanity_val_steps=0,
+        log_every_n_steps=150,
         accelerator=accelerator,
         devices=devices,  # per node
         num_nodes=nodes,
         strategy=strategy,
         precision=precision,
         logger=wandb_logger,
         callbacks=callbacks,
         max_epochs=epochs,
         default_root_dir=save_dir,
-        plugins=plugins
+        plugins=plugins,
+        gradient_clip_val=.3  # reduced from 1 to .3, having some nan issues
     )
 
-    logging.info((trainer.strategy, trainer.world_size,
-                 trainer.local_rank, trainer.global_rank, trainer.node_rank))
-
     trainer.fit(lightning_model, datamodule)  # uses batch size of datamodule
 
-    test_trainer = pl.Trainer(
-        accelerator=accelerator,
-        devices=1,
-        precision=precision,
-        logger=wandb_logger,
-        default_root_dir=save_dir
-    )
-
     best_model_path = trainer.checkpoint_callback.best_model_path
 
     # can test as per the below, but note that datamodule must have a test dataset attribute as per pytorch lightning docs.
     # also be careful not to test regularly, as this breaks train/val/test conceptual separation and may cause hparam overfitting
-    if test_catalog is not None:
+    if datamodule.test_dataloader is not None:
         logging.info(f'Testing on {checkpoint_callback.best_model_path} with single GPU. Be careful not to overfit your choices to the test data...')
-        test_trainer.validate(
-            model=lightning_model,
-            datamodule=datamodule,
-            ckpt_path=checkpoint_callback.best_model_path  # can optionally point to a specific checkpoint here e.g. "/share/nas2/walml/repos/gz-decals-classifiers/results/early_stopping_1xgpu_greyscale/checkpoints/epoch=26-step=16847.ckpt"
-        )
-        test_trainer.test(
+        datamodule.setup(stage='test')
+        # TODO with webdataset, no need for new trainer/datamodule (actually it breaks), but might still be needed with normal dataset?
+        trainer.test(
             model=lightning_model,
             datamodule=datamodule,
             ckpt_path=checkpoint_callback.best_model_path  # can optionally point to a specific checkpoint here e.g. "/share/nas2/walml/repos/gz-decals-classifiers/results/early_stopping_1xgpu_greyscale/checkpoints/epoch=26-step=16847.ckpt"
         )
 
     # explicitly update the model weights to the best checkpoint before returning
     # (assumes only one checkpoint callback, very likely in practice)
```

### Comparing `zoobot-1.0.5/zoobot/shared/benchmark_datasets.py` & `zoobot-2.0.0/zoobot/shared/benchmark_datasets.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/shared/compress_representations.py` & `zoobot-2.0.0/zoobot/shared/compress_representations.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/shared/label_metadata.py` & `zoobot-2.0.0/zoobot/shared/label_metadata.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/shared/load_predictions.py` & `zoobot-2.0.0/zoobot/shared/load_predictions.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
                     logging.debug(f.keys())
                     these_predictions = f['predictions'][:]
                     these_prediction_metadata = {
                         'id_str': f['id_str'].asstr()[:],
                         'hdf5_loc': [os.path.basename(loc) for _ in these_predictions]
                 }
+                    assert len(these_predictions) == len(these_prediction_metadata['id_str']), (loc, len(these_predictions), len(these_prediction_metadata['id_str']) )
                     predictions.append(these_predictions)  # will create a list where each element is 3D predictions stored in each hdf5
                     prediction_metadata.append(these_prediction_metadata)  # also track id_str, similarly
 
                     if template_label_cols is None:  # first file to load, use this as the expected template
                         template_label_cols = f['label_cols'].asstr()[:]
                         logging.info('Using label columns {} from first hdf5 {}'.format(template_label_cols, loc))
                     else:
@@ -68,15 +69,15 @@
     # it just maps a set of hdf5 files, each with predictions, to a df of id_str and those loaded predictions (matching row-wise)
     logging.info('All hdf5 loaded, beginning concat.')
     predictions = np.concatenate(predictions, axis=0)
     prediction_metadata = {
         'id_str': [p for metadata in prediction_metadata for p in metadata['id_str']],
         'hdf5_loc': [l for metadata in prediction_metadata for l in metadata['hdf5_loc']]
     }
-    assert len(prediction_metadata['id_str']) == len(predictions)
+    assert len(prediction_metadata['id_str']) == len(predictions), (len(prediction_metadata['id_str']), len(predictions))
 
     galaxy_id_df = pd.DataFrame(data=prediction_metadata)
 
     return galaxy_id_df, predictions, template_label_cols
 
 
 def prediction_hdf5_to_summary_parquet(hdf5_loc: str, save_loc: str, schema: schemas.Schema, debug=False):
@@ -159,33 +160,43 @@
 
     # define useful cols
     fraction_cols = [col + '_fraction' for col in label_cols]
     lower_edge_cols = [col + '_90pc-lower' for col in label_cols]
     upper_edge_cols = [col + '_90pc-upper' for col in label_cols]
     proportion_asked_cols = [col + '_proportion-asked' for col in label_cols]
 
+
     # make friendly dataframe with just masked fraction and description string
     friendly_loc = save_loc.replace('.parquet', '_friendly.parquet')
     fraction_df = pd.DataFrame(data=masked_fractions, columns=fraction_cols)
     friendly_df = pd.concat([galaxy_id_df, fraction_df], axis=1)
+    friendly_df = convert_halfprecision_cols(friendly_df)
     friendly_df.to_parquet(friendly_loc, index=False)
     logging.info('Friendly summary table saved to {}'.format(friendly_loc))
 
     # make advanced dataframe with unmasked fractions, error bars, proportion_asked
     advanced_loc = save_loc.replace('.parquet', '_advanced.parquet')
     fraction_df = pd.DataFrame(data=unmasked_fractions, columns=fraction_cols)
     lower_edge_df = pd.DataFrame(data=all_lower_edges, columns=lower_edge_cols)
     upper_edge_df = pd.DataFrame(data=all_upper_edges, columns=upper_edge_cols)
     proportion_df = pd.DataFrame(data=prob_of_asked_by_answer, columns=proportion_asked_cols)
     advanced_df = pd.concat([galaxy_id_df, fraction_df, lower_edge_df, upper_edge_df, proportion_df], axis=1)
+    advanced_df = convert_halfprecision_cols(advanced_df)
     advanced_df.to_parquet(advanced_loc, index=False)
     logging.info('Advanced summary table saved to {}'.format(advanced_loc))
 
 
-def single_forward_pass_hdf5s_to_df(hdf5_locs: List, drop_extra_dims=False):
+def convert_halfprecision_cols(df):
+    # convert any half-precision columns, parquet can't save these
+    half_floats = df.select_dtypes(include="float16")
+    df[half_floats.columns] = half_floats.astype("float32")
+    return df
+
+
+def single_forward_pass_hdf5s_to_df(hdf5_locs: List, drop_extra_dims=False, subset_frac=None):
     """
     Load predictions (or representations) saved as hdf5 into pd.DataFrame with id_str and label_cols columns
 
     Best used when not using test-time dropout i.e. when you have a single forward pass per galaxy. 
     Otherwise, with test-time dropout on, aanswer columns (keyed by each value in label_cols) will be
     `np.ndarray` of length (n forward passes) for each galaxy and answer, *not* 1D scalars.
     This is quite awkward to work with. I suggest using `load_hdf5s` directly when using test-time dropout
@@ -193,30 +204,41 @@
     Args:
         hdf5_locs (List): _description_
 
     Returns:
         _type_: _description_
     """
     galaxy_id_df, predictions, label_cols = load_hdf5s(hdf5_locs)
+    logging.info('HDF5s loaded.')
 
     predictions = predictions.squeeze()
-    
+
+
     if len(predictions.shape) > 2:
         if drop_extra_dims:
             predictions = predictions[:, :, 0]
             logging.warning('Dropped extra dimensions')
         else:
             logging.critical(
                 'Predictions are of shape {}, greater than rank 2. \
                 I suggest using load_hdf5s directly to work with np.arrays, not with DataFrame - see docstring'
             )
     prediction_df = pd.DataFrame(data=predictions, columns=label_cols)
+
+    if subset_frac is not None:
+        logging.warning('Selecting a random subset: {}'.format(subset_frac))
+        prediction_df = prediction_df.sample(frac=subset_frac, random_state=42)
+    
+
+    del predictions
+    logging.info('Saving')
     # copy over metadata (indices will align)
     prediction_df['id_str'] = galaxy_id_df['id_str']
     prediction_df['hdf5_loc'] = galaxy_id_df['hdf5_loc']
+    prediction_df = convert_halfprecision_cols(prediction_df)
     return prediction_df
 
 
 if __name__ == '__main__':
 
     logging.basicConfig(level=logging.INFO)
     # simple tests
```

### Comparing `zoobot-1.0.5/zoobot/shared/save_predictions.py` & `zoobot-2.0.0/zoobot/shared/save_predictions.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 import pandas as pd
 import h5py
 
 
 def predictions_to_hdf5(predictions, id_str, label_cols, save_loc, compression="gzip"):
     logging.info(f'Saving predictions to {save_loc}')
     assert save_loc.endswith('.hdf5')
+    if label_cols is None:
+        label_cols = get_default_label_cols(predictions)
+    # sometimes throws a "could not lock file" error but still saves fine. I don't understand why
     with h5py.File(save_loc, "w") as f:
         f.create_dataset(name='predictions', data=predictions, compression=compression)
         # https://docs.h5py.org/en/stable/special.html#h5py.string_dtype
         dt = h5py.string_dtype(encoding='utf-8')
         # predictions_dset.attrs['label_cols'] = label_cols  # would be more conventional but is a little awkward
         f.create_dataset(name='id_str', data=id_str, dtype=dt)
         f.create_dataset(name='label_cols', data=label_cols, dtype=dt)
-        # sometimes throws a "could not lock file" error but still saves fine. I don't understand why
-
 
 def predictions_to_csv(predictions, id_str, label_cols, save_loc):
+    
     # not recommended - hdf5 is much more flexible and pretty easy to use once you check the package quickstart
     assert save_loc.endswith('.csv')
+    if label_cols is None:
+        label_cols = get_default_label_cols(predictions)
     data = [prediction_to_row(predictions[n], id_str[n], label_cols=label_cols) for n in range(len(predictions))]
     predictions_df = pd.DataFrame(data)
     # logging.info(predictions_df)
     predictions_df.to_csv(save_loc, index=False)
 
 
 def prediction_to_row(prediction: np.ndarray, id_str: str, label_cols: List):
@@ -53,7 +57,12 @@
         if isinstance(answer_pred, float) or isinstance(answer_pred, np.float64):
             row[answer + '_pred'] = answer_pred  # it's a scalar already, life is good
         elif len(answer_pred) == 1:  # i.e. if only one sample
             row[answer + '_pred'] = answer_pred.squeeze()  # it's a scalar in disguise, make it a scalar 
         else:
             row[answer + '_pred'] = json.dumps(list(answer_pred))  # it's not a scalar, write as json
     return row
+
+def get_default_label_cols(predictions):
+    logging.warning('No label_cols passed - using default names e.g. feat_0, feat_1...')
+    label_cols = [f'feat_{n}' for n in range(predictions.shape[1])]
+    return label_cols
```

### Comparing `zoobot-1.0.5/zoobot/shared/schemas.py` & `zoobot-2.0.0/zoobot/shared/schemas.py`

 * *Files 16% similar despite different names*

```diff
@@ -126,25 +126,43 @@
             except IndexError:
                 raise ValueError(f'{prev_answer_text} not found in dependencies')
             prev_answer._next_question = question
             question._asked_after = prev_answer
 
 
 class Schema():
-    def __init__(self, question_answer_pairs:dict, dependencies):
+    
+    def __init__(self, question_answer_pairs:dict, dependencies: dict):
         """
         Relate the df label columns tor question/answer groups and to tfrecod label indices
         Requires that labels be continguous by question - easily satisfied
 
         Be careful with dependencies:
         - first entry should be the first answer to that question, by df column order
         - second entry should be the last answer to that question, similarly
         - answers in between will be included: these are used to slice
         - df columns must be contigious by question (e.g. not smooth_yes, bar_no, smooth_no) for this to work!
 
+        The following schemas are available via the module (e.g. `from zoobot.shared.schemas import decals_dr5_ortho_schema`):
+        - decals_dr5_ortho_schema
+        - decals_dr8_ortho_schema
+        - decals_all_campaigns_ortho_schema
+        - gz2_ortho_schema
+        - gz_candels_ortho_schema
+        - gz_hubble_ortho_schema
+        - cosmic_dawn_ortho_schema
+        - cosmic_dawn_schema
+        - gz_rings_schema
+        - desi_schema
+        - gz_evo_v1_schema (this is the schema currently used for pretraining)
+        - gz_ukidss_schema
+        - gz_jwst_schema
+
+        "ortho" refers to the orthogonal question suffix (-cd, -dr8, etc).
+
         Args:
             question_answer_pairs (dict): e.g. {'smooth-or-featured: ['_smooth, _featured-or-disk, ...], ...}
             dependencies (dict): dict mapping each question (e.g. disk-edge-on) to the answer on which it depends (e.g. smooth-or-featured_featured-or-disk)
         """
         self.question_answer_pairs = question_answer_pairs
         _, self.label_cols = label_metadata.extract_questions_and_label_cols(question_answer_pairs)
         self.dependencies = dependencies
@@ -274,7 +292,10 @@
 gz_rings_schema = Schema(label_metadata.rings_pairs, label_metadata.rings_dependencies)
 desi_schema = Schema(label_metadata.desi_pairs, label_metadata.desi_dependencies)  # for DESI data release prediction users, not for ML training - no -dr5, -dr8, etc
 # note that as this is a call to Schema (and Question and Answer), any logging within those will 
 # trigger basicConfig() and prevent user setting their own logging.
 # so don't log anything during Schema.__init__!
 
 gz_evo_v1_schema = Schema(label_metadata.gz_evo_v1_pairs, label_metadata.gz_evo_v1_dependencies)
+
+gz_ukidss_schema = Schema(label_metadata.ukidss_ortho_pairs, label_metadata.ukidss_ortho_dependencies)
+gz_jwst_schema = Schema(label_metadata.jwst_ortho_pairs, label_metadata.jwst_ortho_dependencies)
```

### Comparing `zoobot-1.0.5/zoobot/shared/stats.py` & `zoobot-2.0.0/zoobot/shared/stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/estimators/alexnet_baseline.py` & `zoobot-2.0.0/zoobot/tensorflow/estimators/alexnet_baseline.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/estimators/custom_callbacks.py` & `zoobot-2.0.0/zoobot/tensorflow/estimators/custom_callbacks.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/estimators/custom_layers.py` & `zoobot-2.0.0/zoobot/tensorflow/estimators/custom_layers.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/estimators/define_model.py` & `zoobot-2.0.0/zoobot/tensorflow/estimators/define_model.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/estimators/efficientnet_custom.py` & `zoobot-2.0.0/zoobot/tensorflow/estimators/efficientnet_custom.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/estimators/efficientnet_standard.py` & `zoobot-2.0.0/zoobot/tensorflow/estimators/efficientnet_standard.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/estimators/small_cnn_baseline.py` & `zoobot-2.0.0/zoobot/tensorflow/estimators/small_cnn_baseline.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/predictions/predict_on_dataset.py` & `zoobot-2.0.0/zoobot/tensorflow/predictions/predict_on_dataset.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py` & `zoobot-2.0.0/zoobot/tensorflow/predictions/visualize_dirichlet_predictions.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/stats/coverage.py` & `zoobot-2.0.0/zoobot/tensorflow/stats/coverage.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/stats/dirichlet_stats.py` & `zoobot-2.0.0/zoobot/tensorflow/stats/dirichlet_stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/stats/mixture_stats.py` & `zoobot-2.0.0/zoobot/tensorflow/stats/mixture_stats.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/training/custom_metrics.py` & `zoobot-2.0.0/zoobot/tensorflow/training/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/training/finetune.py` & `zoobot-2.0.0/zoobot/tensorflow/training/finetune.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/training/losses.py` & `zoobot-2.0.0/zoobot/tensorflow/training/losses.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Get subclass of tf.keras.losses.Loss which wraps ``calculate_multiquestion_loss`` and sums over batch.
 
     tf.keras.losses.Reduction.SUM_OVER_BATCH_SIZE will assume the question dimension (10) is also part of the batch, and divide by an extra factor of 10
     tf.keras.losses.Reduction.SUM_OVER_BATCH_SIZE also does not work in distributed training (as batch size is split between replicas)
     tf.keras.losses.Reduction.SUM will simply add everything up, so divide by the global batch size externally with tf.reduce_sum
 
     Args:
-        question_index_groups (list): Answer indices for each question i.e. [(question.start_index, question.end_index), ...] for all questions. Useful for slicing model predictions by question.
+        question_index_groups (list): Answer indices for each question i.e. [(question.start_index, question.end_index), ...] for all questions. Useful for slicing model predictions by question. See :ref:`schemas`.
 
     Returns:
         MultiquestionLoss: see above.
     """
 
     class MultiquestionLoss(tf.keras.losses.Loss):
 
@@ -32,15 +32,15 @@
 
     Negative log likelihood of observing ``labels`` (volunteer answers to all questions)
     from Dirichlet-Multinomial distributions for each question, using concentrations ``predictions``.
     
     Args:
         labels (tf.Tensor): (galaxy, k successes) where k successes dimension is indexed by question_index_groups.
         predictions (tf.Tensor):  Dirichlet concentrations, matching shape of labels
-        question_index_groups (list): Paired (tuple) integers of (first, last) indices of answers to each question, listed for all questions.
+        question_index_groups (list): Answer indices for each question i.e. [(question.start_index, question.end_index), ...] for all questions. Useful for slicing model predictions by question. See :ref:`schemas`.
     
     Returns:
         tf.Tensor: neg. log likelihood of shape (batch, question).
     """
     # very important that question_index_groups is fixed and discrete, else tf.function autograph will mess up 
     q_losses = []
     # will give shape errors if model output dim is not labels dim, which can happen if losses.py substrings are missing an answer
```

### Comparing `zoobot-1.0.5/zoobot/tensorflow/training/train_with_keras.py` & `zoobot-2.0.0/zoobot/tensorflow/training/train_with_keras.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot/tensorflow/training/training_config.py` & `zoobot-2.0.0/zoobot/tensorflow/training/training_config.py`

 * *Files identical despite different names*

### Comparing `zoobot-1.0.5/zoobot.egg-info/PKG-INFO` & `zoobot-2.0.0/zoobot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7a6f 6f62  : 2.1.Name: zoob
-00000020: 6f74 0a56 6572 7369 6f6e 3a20 312e 302e  ot.Version: 1.0.
-00000030: 350a 5375 6d6d 6172 793a 2047 616c 6178  5.Summary: Galax
+00000020: 6f74 0a56 6572 7369 6f6e 3a20 322e 302e  ot.Version: 2.0.
+00000030: 300a 5375 6d6d 6172 793a 2047 616c 6178  0.Summary: Galax
 00000040: 7920 6d6f 7270 686f 6c6f 6779 2063 6c61  y morphology cla
 00000050: 7373 6966 6965 7273 0a48 6f6d 652d 7061  ssifiers.Home-pa
 00000060: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
 00000070: 7562 2e63 6f6d 2f6d 7761 6c6d 736c 6579  ub.com/mwalmsley
 00000080: 2f7a 6f6f 626f 740a 4175 7468 6f72 3a20  /zoobot.Author: 
 00000090: 4d69 6b65 2057 616c 6d73 6c65 790a 4175  Mike Walmsley.Au
 000000a0: 7468 6f72 2d65 6d61 696c 3a20 7761 6c6d  thor-email: walm
@@ -23,15 +23,15 @@
 00000160: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
 00000170: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
 00000180: 2053 7461 7475 7320 3a3a 2034 202d 2042   Status :: 4 - B
 00000190: 6574 610a 436c 6173 7369 6669 6572 3a20  eta.Classifier: 
 000001a0: 456e 7669 726f 6e6d 656e 7420 3a3a 2047  Environment :: G
 000001b0: 5055 203a 3a20 4e56 4944 4941 2043 5544  PU :: NVIDIA CUD
 000001c0: 410a 5265 7175 6972 6573 2d50 7974 686f  A.Requires-Pytho
-000001d0: 6e3a 203e 3d33 2e38 0a44 6573 6372 6970  n: >=3.8.Descrip
+000001d0: 6e3a 203e 3d33 2e39 0a44 6573 6372 6970  n: >=3.9.Descrip
 000001e0: 7469 6f6e 2d43 6f6e 7465 6e74 2d54 7970  tion-Content-Typ
 000001f0: 653a 2074 6578 742f 6d61 726b 646f 776e  e: text/markdown
 00000200: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
 00000210: 4943 454e 5345 0a52 6571 7569 7265 732d  ICENSE.Requires-
 00000220: 4469 7374 3a20 6835 7079 0a52 6571 7569  Dist: h5py.Requi
 00000230: 7265 732d 4469 7374 3a20 7471 646d 0a52  res-Dist: tqdm.R
 00000240: 6571 7569 7265 732d 4469 7374 3a20 7069  equires-Dist: pi
@@ -44,981 +44,981 @@
 000002b0: 6972 6573 2d44 6973 743a 2073 6369 6b69  ires-Dist: sciki
 000002c0: 742d 6c65 6172 6e3e 3d31 2e30 2e32 0a52  t-learn>=1.0.2.R
 000002d0: 6571 7569 7265 732d 4469 7374 3a20 6d61  equires-Dist: ma
 000002e0: 7470 6c6f 746c 6962 0a52 6571 7569 7265  tplotlib.Require
 000002f0: 732d 4469 7374 3a20 7079 6172 726f 770a  s-Dist: pyarrow.
 00000300: 5265 7175 6972 6573 2d44 6973 743a 2077  Requires-Dist: w
 00000310: 616e 6462 0a52 6571 7569 7265 732d 4469  andb.Requires-Di
-00000320: 7374 3a20 7365 7475 7074 6f6f 6c73 0a52  st: setuptools.R
-00000330: 6571 7569 7265 732d 4469 7374 3a20 6761  equires-Dist: ga
-00000340: 6c61 7879 2d64 6174 6173 6574 733e 3d30  laxy-datasets>=0
-00000350: 2e30 2e31 350a 5072 6f76 6964 6573 2d45  .0.15.Provides-E
-00000360: 7874 7261 3a20 7079 746f 7263 682d 6370  xtra: pytorch-cp
-00000370: 750a 5265 7175 6972 6573 2d44 6973 743a  u.Requires-Dist:
-00000380: 2074 6f72 6368 3d3d 312e 3132 2e31 2b63   torch==1.12.1+c
-00000390: 7075 3b20 6578 7472 6120 3d3d 2022 7079  pu; extra == "py
-000003a0: 746f 7263 682d 6370 7522 0a52 6571 7569  torch-cpu".Requi
-000003b0: 7265 732d 4469 7374 3a20 746f 7263 6876  res-Dist: torchv
-000003c0: 6973 696f 6e3d 3d30 2e31 332e 312b 6370  ision==0.13.1+cp
-000003d0: 753b 2065 7874 7261 203d 3d20 2270 7974  u; extra == "pyt
-000003e0: 6f72 6368 2d63 7075 220a 5265 7175 6972  orch-cpu".Requir
-000003f0: 6573 2d44 6973 743a 2074 6f72 6368 6175  es-Dist: torchau
-00000400: 6469 6f3d 3d30 2e31 322e 313b 2065 7874  dio==0.12.1; ext
-00000410: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
-00000420: 7075 220a 5265 7175 6972 6573 2d44 6973  pu".Requires-Dis
-00000430: 743a 2070 7974 6f72 6368 2d6c 6967 6874  t: pytorch-light
-00000440: 6e69 6e67 3e3d 322e 302e 303b 2065 7874  ning>=2.0.0; ext
-00000450: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
-00000460: 7075 220a 5265 7175 6972 6573 2d44 6973  pu".Requires-Dis
-00000470: 743a 2061 6c62 756d 656e 7461 7469 6f6e  t: albumentation
-00000480: 733b 2065 7874 7261 203d 3d20 2270 7974  s; extra == "pyt
-00000490: 6f72 6368 2d63 7075 220a 5265 7175 6972  orch-cpu".Requir
-000004a0: 6573 2d44 6973 743a 2070 7972 6f2d 7070  es-Dist: pyro-pp
-000004b0: 6c3d 3d31 2e38 2e30 3b20 6578 7472 6120  l==1.8.0; extra 
-000004c0: 3d3d 2022 7079 746f 7263 682d 6370 7522  == "pytorch-cpu"
-000004d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000004e0: 746f 7263 686d 6574 7269 6373 3d3d 302e  torchmetrics==0.
-000004f0: 3131 2e30 3b20 6578 7472 6120 3d3d 2022  11.0; extra == "
-00000500: 7079 746f 7263 682d 6370 7522 0a52 6571  pytorch-cpu".Req
-00000510: 7569 7265 732d 4469 7374 3a20 7469 6d6d  uires-Dist: timm
-00000520: 3d3d 302e 362e 3132 3b20 6578 7472 6120  ==0.6.12; extra 
-00000530: 3d3d 2022 7079 746f 7263 682d 6370 7522  == "pytorch-cpu"
-00000540: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000550: 2070 7974 6f72 6368 2d6d 310a 5265 7175   pytorch-m1.Requ
-00000560: 6972 6573 2d44 6973 743a 2074 6f72 6368  ires-Dist: torch
-00000570: 3d3d 312e 3132 2e31 3b20 6578 7472 6120  ==1.12.1; extra 
-00000580: 3d3d 2022 7079 746f 7263 682d 6d31 220a  == "pytorch-m1".
-00000590: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
-000005a0: 6f72 6368 7669 7369 6f6e 3d3d 302e 3133  orchvision==0.13
-000005b0: 2e31 3b20 6578 7472 6120 3d3d 2022 7079  .1; extra == "py
-000005c0: 746f 7263 682d 6d31 220a 5265 7175 6972  torch-m1".Requir
-000005d0: 6573 2d44 6973 743a 2074 6f72 6368 6175  es-Dist: torchau
-000005e0: 6469 6f3d 3d30 2e31 322e 313b 2065 7874  dio==0.12.1; ext
-000005f0: 7261 203d 3d20 2270 7974 6f72 6368 2d6d  ra == "pytorch-m
-00000600: 3122 0a52 6571 7569 7265 732d 4469 7374  1".Requires-Dist
-00000610: 3a20 7079 746f 7263 682d 6c69 6768 746e  : pytorch-lightn
-00000620: 696e 673e 3d32 2e30 2e30 3b20 6578 7472  ing>=2.0.0; extr
-00000630: 6120 3d3d 2022 7079 746f 7263 682d 6d31  a == "pytorch-m1
-00000640: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000650: 2061 6c62 756d 656e 7461 7469 6f6e 733b   albumentations;
-00000660: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
-00000670: 6368 2d6d 3122 0a52 6571 7569 7265 732d  ch-m1".Requires-
-00000680: 4469 7374 3a20 7079 726f 2d70 706c 3d3d  Dist: pyro-ppl==
-00000690: 312e 382e 303b 2065 7874 7261 203d 3d20  1.8.0; extra == 
-000006a0: 2270 7974 6f72 6368 2d6d 3122 0a52 6571  "pytorch-m1".Req
-000006b0: 7569 7265 732d 4469 7374 3a20 746f 7263  uires-Dist: torc
-000006c0: 686d 6574 7269 6373 3d3d 302e 3131 2e30  hmetrics==0.11.0
-000006d0: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
-000006e0: 7263 682d 6d31 220a 5265 7175 6972 6573  rch-m1".Requires
-000006f0: 2d44 6973 743a 2074 696d 6d3d 3d30 2e36  -Dist: timm==0.6
-00000700: 2e31 323b 2065 7874 7261 203d 3d20 2270  .12; extra == "p
-00000710: 7974 6f72 6368 2d6d 3122 0a50 726f 7669  ytorch-m1".Provi
-00000720: 6465 732d 4578 7472 613a 2070 7974 6f72  des-Extra: pytor
-00000730: 6368 2d63 7531 3133 0a52 6571 7569 7265  ch-cu113.Require
-00000740: 732d 4469 7374 3a20 746f 7263 683d 3d31  s-Dist: torch==1
-00000750: 2e31 322e 312b 6375 3131 333b 2065 7874  .12.1+cu113; ext
-00000760: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
-00000770: 7531 3133 220a 5265 7175 6972 6573 2d44  u113".Requires-D
-00000780: 6973 743a 2074 6f72 6368 7669 7369 6f6e  ist: torchvision
-00000790: 3d3d 302e 3133 2e31 2b63 7531 3133 3b20  ==0.13.1+cu113; 
-000007a0: 6578 7472 6120 3d3d 2022 7079 746f 7263  extra == "pytorc
-000007b0: 682d 6375 3131 3322 0a52 6571 7569 7265  h-cu113".Require
-000007c0: 732d 4469 7374 3a20 746f 7263 6861 7564  s-Dist: torchaud
-000007d0: 696f 3d3d 302e 3132 2e31 3b20 6578 7472  io==0.12.1; extr
-000007e0: 6120 3d3d 2022 7079 746f 7263 682d 6375  a == "pytorch-cu
-000007f0: 3131 3322 0a52 6571 7569 7265 732d 4469  113".Requires-Di
-00000800: 7374 3a20 7079 746f 7263 682d 6c69 6768  st: pytorch-ligh
-00000810: 746e 696e 673e 3d32 2e30 2e30 3b20 6578  tning>=2.0.0; ex
-00000820: 7472 6120 3d3d 2022 7079 746f 7263 682d  tra == "pytorch-
-00000830: 6375 3131 3322 0a52 6571 7569 7265 732d  cu113".Requires-
-00000840: 4469 7374 3a20 616c 6275 6d65 6e74 6174  Dist: albumentat
-00000850: 696f 6e73 3b20 6578 7472 6120 3d3d 2022  ions; extra == "
-00000860: 7079 746f 7263 682d 6375 3131 3322 0a52  pytorch-cu113".R
-00000870: 6571 7569 7265 732d 4469 7374 3a20 7079  equires-Dist: py
-00000880: 726f 2d70 706c 3d3d 312e 382e 303b 2065  ro-ppl==1.8.0; e
-00000890: 7874 7261 203d 3d20 2270 7974 6f72 6368  xtra == "pytorch
-000008a0: 2d63 7531 3133 220a 5265 7175 6972 6573  -cu113".Requires
-000008b0: 2d44 6973 743a 2074 6f72 6368 6d65 7472  -Dist: torchmetr
-000008c0: 6963 733d 3d30 2e31 312e 303b 2065 7874  ics==0.11.0; ext
-000008d0: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
-000008e0: 7531 3133 220a 5265 7175 6972 6573 2d44  u113".Requires-D
-000008f0: 6973 743a 2074 696d 6d3d 3d30 2e36 2e31  ist: timm==0.6.1
-00000900: 323b 2065 7874 7261 203d 3d20 2270 7974  2; extra == "pyt
-00000910: 6f72 6368 2d63 7531 3133 220a 5072 6f76  orch-cu113".Prov
-00000920: 6964 6573 2d45 7874 7261 3a20 7079 746f  ides-Extra: pyto
-00000930: 7263 682d 636f 6c61 620a 5265 7175 6972  rch-colab.Requir
-00000940: 6573 2d44 6973 743a 2070 7974 6f72 6368  es-Dist: pytorch
-00000950: 2d6c 6967 6874 6e69 6e67 3e3d 322e 302e  -lightning>=2.0.
-00000960: 303b 2065 7874 7261 203d 3d20 2270 7974  0; extra == "pyt
-00000970: 6f72 6368 2d63 6f6c 6162 220a 5265 7175  orch-colab".Requ
-00000980: 6972 6573 2d44 6973 743a 2061 6c62 756d  ires-Dist: album
-00000990: 656e 7461 7469 6f6e 733b 2065 7874 7261  entations; extra
-000009a0: 203d 3d20 2270 7974 6f72 6368 2d63 6f6c   == "pytorch-col
-000009b0: 6162 220a 5265 7175 6972 6573 2d44 6973  ab".Requires-Dis
-000009c0: 743a 2070 7972 6f2d 7070 6c3e 3d31 2e38  t: pyro-ppl>=1.8
-000009d0: 2e30 3b20 6578 7472 6120 3d3d 2022 7079  .0; extra == "py
-000009e0: 746f 7263 682d 636f 6c61 6222 0a52 6571  torch-colab".Req
-000009f0: 7569 7265 732d 4469 7374 3a20 746f 7263  uires-Dist: torc
-00000a00: 686d 6574 7269 6373 3d3d 302e 3131 2e30  hmetrics==0.11.0
-00000a10: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
-00000a20: 7263 682d 636f 6c61 6222 0a52 6571 7569  rch-colab".Requi
-00000a30: 7265 732d 4469 7374 3a20 7469 6d6d 3d3d  res-Dist: timm==
-00000a40: 302e 362e 3132 3b20 6578 7472 6120 3d3d  0.6.12; extra ==
-00000a50: 2022 7079 746f 7263 682d 636f 6c61 6222   "pytorch-colab"
-00000a60: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000a70: 2074 656e 736f 7266 6c6f 770a 5265 7175   tensorflow.Requ
-00000a80: 6972 6573 2d44 6973 743a 2074 656e 736f  ires-Dist: tenso
-00000a90: 7266 6c6f 773d 3d32 2e31 302e 303b 2065  rflow==2.10.0; e
-00000aa0: 7874 7261 203d 3d20 2274 656e 736f 7266  xtra == "tensorf
-00000ab0: 6c6f 7722 0a52 6571 7569 7265 732d 4469  low".Requires-Di
-00000ac0: 7374 3a20 6b65 7261 735f 6170 706c 6963  st: keras_applic
-00000ad0: 6174 696f 6e73 3b20 6578 7472 6120 3d3d  ations; extra ==
-00000ae0: 2022 7465 6e73 6f72 666c 6f77 220a 5265   "tensorflow".Re
-00000af0: 7175 6972 6573 2d44 6973 743a 2074 656e  quires-Dist: ten
-00000b00: 736f 7266 6c6f 775f 7072 6f62 6162 696c  sorflow_probabil
-00000b10: 6974 793d 3d30 2e31 382e 303b 2065 7874  ity==0.18.0; ext
-00000b20: 7261 203d 3d20 2274 656e 736f 7266 6c6f  ra == "tensorflo
-00000b30: 7722 0a52 6571 7569 7265 732d 4469 7374  w".Requires-Dist
-00000b40: 3a20 7072 6f74 6f62 7566 3c3d 332e 3139  : protobuf<=3.19
-00000b50: 3b20 6578 7472 6120 3d3d 2022 7465 6e73  ; extra == "tens
-00000b60: 6f72 666c 6f77 220a 5072 6f76 6964 6573  orflow".Provides
-00000b70: 2d45 7874 7261 3a20 7574 696c 6974 6965  -Extra: utilitie
-00000b80: 730a 5265 7175 6972 6573 2d44 6973 743a  s.Requires-Dist:
-00000b90: 2073 6561 626f 726e 3b20 6578 7472 6120   seaborn; extra 
-00000ba0: 3d3d 2022 7574 696c 6974 6965 7322 0a52  == "utilities".R
-00000bb0: 6571 7569 7265 732d 4469 7374 3a20 626f  equires-Dist: bo
-00000bc0: 746f 333b 2065 7874 7261 203d 3d20 2275  to3; extra == "u
-00000bd0: 7469 6c69 7469 6573 220a 5265 7175 6972  tilities".Requir
-00000be0: 6573 2d44 6973 743a 2070 7974 686f 6e2d  es-Dist: python-
-00000bf0: 6461 7465 7574 696c 3d3d 322e 382e 313b  dateutil==2.8.1;
-00000c00: 2065 7874 7261 203d 3d20 2275 7469 6c69   extra == "utili
-00000c10: 7469 6573 220a 5072 6f76 6964 6573 2d45  ties".Provides-E
-00000c20: 7874 7261 3a20 646f 6373 0a52 6571 7569  xtra: docs.Requi
-00000c30: 7265 732d 4469 7374 3a20 5370 6869 6e78  res-Dist: Sphinx
-00000c40: 3b20 6578 7472 6120 3d3d 2022 646f 6373  ; extra == "docs
-00000c50: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00000c60: 2073 7068 696e 7863 6f6e 7472 6962 2d6e   sphinxcontrib-n
-00000c70: 6170 6f6c 656f 6e3b 2065 7874 7261 203d  apoleon; extra =
-00000c80: 3d20 2264 6f63 7322 0a52 6571 7569 7265  = "docs".Require
-00000c90: 732d 4469 7374 3a20 6675 726f 3b20 6578  s-Dist: furo; ex
-00000ca0: 7472 6120 3d3d 2022 646f 6373 220a 5265  tra == "docs".Re
-00000cb0: 7175 6972 6573 2d44 6973 743a 2064 6f63  quires-Dist: doc
-00000cc0: 7574 696c 733c 302e 3138 3b20 6578 7472  utils<0.18; extr
-00000cd0: 6120 3d3d 2022 646f 6373 220a 0a23 205a  a == "docs"..# Z
-00000ce0: 6f6f 626f 740a 0a5b 215b 446f 776e 6c6f  oobot..[![Downlo
-00000cf0: 6164 735d 2868 7474 7073 3a2f 2f70 6570  ads](https://pep
-00000d00: 792e 7465 6368 2f62 6164 6765 2f7a 6f6f  y.tech/badge/zoo
-00000d10: 626f 7429 5d28 6874 7470 733a 2f2f 7065  bot)](https://pe
-00000d20: 7079 2e74 6563 682f 7072 6f6a 6563 742f  py.tech/project/
-00000d30: 7a6f 6f62 6f74 290a 5b21 5b44 6f63 756d  zoobot).[![Docum
-00000d40: 656e 7461 7469 6f6e 2053 7461 7475 735d  entation Status]
-00000d50: 2868 7474 7073 3a2f 2f72 6561 6474 6865  (https://readthe
-00000d60: 646f 6373 2e6f 7267 2f70 726f 6a65 6374  docs.org/project
-00000d70: 732f 7a6f 6f62 6f74 2f62 6164 6765 2f3f  s/zoobot/badge/?
-00000d80: 7665 7273 696f 6e3d 6c61 7465 7374 295d  version=latest)]
-00000d90: 2868 7474 7073 3a2f 2f7a 6f6f 626f 742e  (https://zoobot.
-00000da0: 7265 6164 7468 6564 6f63 732e 696f 2f29  readthedocs.io/)
-00000db0: 0a21 5b62 7569 6c64 5d28 6874 7470 733a  .![build](https:
-00000dc0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 7761  //github.com/mwa
-00000dd0: 6c6d 736c 6579 2f7a 6f6f 626f 742f 6163  lmsley/zoobot/ac
-00000de0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000df0: 7275 6e5f 4349 2e79 6d6c 2f62 6164 6765  run_CI.yml/badge
-00000e00: 2e73 7667 290a 215b 7075 626c 6973 685d  .svg).![publish]
-00000e10: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000e20: 636f 6d2f 6d77 616c 6d73 6c65 792f 7a6f  com/mwalmsley/zo
-00000e30: 6f62 6f74 2f61 6374 696f 6e73 2f77 6f72  obot/actions/wor
-00000e40: 6b66 6c6f 7773 2f70 7974 686f 6e2d 7075  kflows/python-pu
-00000e50: 626c 6973 682e 796d 6c2f 6261 6467 652e  blish.yml/badge.
-00000e60: 7376 6729 0a5b 215b 5079 5049 5d28 6874  svg).[![PyPI](ht
-00000e70: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-00000e80: 2e69 6f2f 7079 2f7a 6f6f 626f 742e 7376  .io/py/zoobot.sv
-00000e90: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
-00000ea0: 652e 6675 7279 2e69 6f2f 7079 2f7a 6f6f  e.fury.io/py/zoo
-00000eb0: 626f 7429 0a5b 215b 444f 495d 2868 7474  bot).[![DOI](htt
-00000ec0: 7073 3a2f 2f7a 656e 6f64 6f2e 6f72 672f  ps://zenodo.org/
-00000ed0: 6261 6467 652f 3334 3337 3837 3631 372e  badge/343787617.
-00000ee0: 7376 6729 5d28 6874 7470 733a 2f2f 7a65  svg)](https://ze
-00000ef0: 6e6f 646f 2e6f 7267 2f62 6164 6765 2f6c  nodo.org/badge/l
-00000f00: 6174 6573 7464 6f69 2f33 3433 3738 3736  atestdoi/3437876
-00000f10: 3137 290a 5b21 5b73 7461 7475 735d 2868  17).[![status](h
-00000f20: 7474 7073 3a2f 2f6a 6f73 732e 7468 656f  ttps://joss.theo
-00000f30: 6a2e 6f72 672f 7061 7065 7273 2f34 3437  j.org/papers/447
-00000f40: 3536 3165 6532 6465 3437 3039 6564 6462  561ee2de4709eddb
-00000f50: 3730 3465 3138 6265 6538 3436 662f 7374  704e18bee846f/st
-00000f60: 6174 7573 2e73 7667 295d 2868 7474 7073  atus.svg)](https
-00000f70: 3a2f 2f6a 6f73 732e 7468 656f 6a2e 6f72  ://joss.theoj.or
-00000f80: 672f 7061 7065 7273 2f34 3437 3536 3165  g/papers/447561e
-00000f90: 6532 6465 3437 3039 6564 6462 3730 3465  e2de4709eddb704e
-00000fa0: 3138 6265 6538 3436 6629 0a3c 6120 6872  18bee846f).<a hr
-00000fb0: 6566 3d22 6874 7470 733a 2f2f 6173 636c  ef="https://ascl
-00000fc0: 2e6e 6574 2f32 3230 332e 3032 3722 3e3c  .net/2203.027"><
-00000fd0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000fe0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000ff0: 6261 6467 652f 6173 636c 2d32 3230 332e  badge/ascl-2203.
-00001000: 3032 372d 626c 7565 2e73 7667 3f63 6f6c  027-blue.svg?col
-00001010: 6f72 423d 3236 3232 3535 2220 616c 743d  orB=262255" alt=
-00001020: 2261 7363 6c3a 3232 3033 2e30 3237 2220  "ascl:2203.027" 
-00001030: 2f3e 3c2f 613e 0a0a 5a6f 6f62 6f74 2063  /></a>..Zoobot c
-00001040: 6c61 7373 6966 6965 7320 6761 6c61 7879  lassifies galaxy
-00001050: 206d 6f72 7068 6f6c 6f67 7920 7769 7468   morphology with
-00001060: 2064 6565 7020 6c65 6172 6e69 6e67 2e0a   deep learning..
-00001070: 3c21 2d2d 2041 7420 4761 6c61 7879 205a  <!-- At Galaxy Z
-00001080: 6f6f 2c20 7765 2075 7365 205a 6f6f 626f  oo, we use Zoobo
-00001090: 7420 746f 2068 656c 7020 6f75 7220 766f  t to help our vo
-000010a0: 6c75 6e74 6565 7273 2063 6c61 7373 6966  lunteers classif
-000010b0: 7920 7468 6520 6761 6c61 7869 6573 2069  y the galaxies i
-000010c0: 6e20 616c 6c20 6f75 7220 7265 6365 6e74  n all our recent
-000010d0: 2063 6174 616c 6f67 7565 733a 2047 5a20   catalogues: GZ 
-000010e0: 4445 4361 4c53 2c20 475a 2044 4553 492c  DECaLS, GZ DESI,
-000010f0: 2047 5a20 5269 6e67 7320 616e 6420 475a   GZ Rings and GZ
-00001100: 2043 6f73 6d69 6320 4461 776e 2e20 2d2d   Cosmic Dawn. --
-00001110: 3e0a 0a5a 6f6f 626f 7420 6973 2074 7261  >..Zoobot is tra
-00001120: 696e 6564 2075 7369 6e67 206d 696c 6c69  ined using milli
-00001130: 6f6e 7320 6f66 2061 6e73 7765 7273 2062  ons of answers b
-00001140: 7920 4761 6c61 7879 205a 6f6f 2076 6f6c  y Galaxy Zoo vol
-00001150: 756e 7465 6572 732e 2054 6869 7320 636f  unteers. This co
-00001160: 6465 2077 696c 6c20 6c65 7420 796f 7520  de will let you 
-00001170: 2a2a 7265 7472 6169 6e2a 2a20 5a6f 6f62  **retrain** Zoob
-00001180: 6f74 2074 6f20 6163 6375 7261 7465 6c79  ot to accurately
-00001190: 2073 6f6c 7665 2079 6f75 7220 6f77 6e20   solve your own 
-000011a0: 7072 6564 6963 7469 6f6e 2074 6173 6b2e  prediction task.
-000011b0: 0a0a 2d20 5b49 6e73 7461 6c6c 5d28 2369  ..- [Install](#i
-000011c0: 6e73 7461 6c6c 6174 696f 6e29 0a2d 205b  nstallation).- [
-000011d0: 5175 6963 6b73 7461 7274 5d28 2371 7569  Quickstart](#qui
-000011e0: 636b 7374 6172 7429 0a2d 205b 576f 726b  ckstart).- [Work
-000011f0: 6564 2045 7861 6d70 6c65 735d 2823 776f  ed Examples](#wo
-00001200: 726b 6564 2d65 7861 6d70 6c65 7329 0a2d  rked-examples).-
-00001210: 205b 5072 6574 7261 696e 6564 2057 6569   [Pretrained Wei
-00001220: 6768 7473 5d28 6874 7470 733a 2f2f 7a6f  ghts](https://zo
-00001230: 6f62 6f74 2e72 6561 6474 6865 646f 6373  obot.readthedocs
-00001240: 2e69 6f2f 656e 2f6c 6174 6573 742f 6461  .io/en/latest/da
-00001250: 7461 5f6e 6f74 6573 2e68 746d 6c29 0a2d  ta_notes.html).-
-00001260: 205b 4461 7461 7365 7473 5d28 6874 7470   [Datasets](http
-00001270: 733a 2f2f 7777 772e 6769 7468 7562 2e63  s://www.github.c
-00001280: 6f6d 2f6d 7761 6c6d 736c 6579 2f67 616c  om/mwalmsley/gal
-00001290: 6178 792d 6461 7461 7365 7473 290a 2d20  axy-datasets).- 
-000012a0: 5b44 6f63 756d 656e 7461 7469 6f6e 5d28  [Documentation](
-000012b0: 6874 7470 733a 2f2f 7a6f 6f62 6f74 2e72  https://zoobot.r
-000012c0: 6561 6474 6865 646f 6373 2e69 6f2f 2920  eadthedocs.io/) 
-000012d0: 2866 6f72 2075 6e64 6572 7374 616e 6469  (for understandi
-000012e0: 6e67 2f72 6566 6572 656e 6365 290a 0a23  ng/reference)..#
-000012f0: 2320 496e 7374 616c 6c61 7469 6f6e 0a3c  # Installation.<
-00001300: 6120 6e61 6d65 3d22 696e 7374 616c 6c61  a name="installa
-00001310: 7469 6f6e 223e 3c2f 613e 0a0a 596f 7520  tion"></a>..You 
-00001320: 6361 6e20 7265 7472 6169 6e20 5a6f 6f62  can retrain Zoob
-00001330: 6f74 2069 6e20 7468 6520 636c 6f75 6420  ot in the cloud 
-00001340: 7769 7468 2061 2066 7265 6520 4750 5520  with a free GPU 
-00001350: 7573 696e 6720 7468 6973 205b 476f 6f67  using this [Goog
-00001360: 6c65 2043 6f6c 6162 206e 6f74 6562 6f6f  le Colab noteboo
-00001370: 6b5d 2868 7474 7073 3a2f 2f63 6f6c 6162  k](https://colab
-00001380: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00001390: 2e63 6f6d 2f64 7269 7665 2f31 3762 625f  .com/drive/17bb_
-000013a0: 4b62 4132 4a36 7972 496d 3470 3455 655f  KbA2J6yrIm4p4Ue_
-000013b0: 6c45 4248 4d4e 4331 4939 4a64 3f75 7370  lEBHMNC1I9Jd?usp
-000013c0: 3d73 6861 7269 6e67 292e 2054 6f20 696e  =sharing). To in
-000013d0: 7374 616c 6c20 6c6f 6361 6c6c 792c 206b  stall locally, k
-000013e0: 6565 7020 7265 6164 696e 672e 0a0a 446f  eep reading...Do
-000013f0: 776e 6c6f 6164 2074 6865 2063 6f64 6520  wnload the code 
-00001400: 7573 696e 6720 6769 743a 0a0a 2020 2020  using git:..    
-00001410: 6769 7420 636c 6f6e 6520 6769 7440 6769  git clone git@gi
-00001420: 7468 7562 2e63 6f6d 3a6d 7761 6c6d 736c  thub.com:mwalmsl
-00001430: 6579 2f7a 6f6f 626f 742e 6769 740a 0a41  ey/zoobot.git..A
-00001440: 6e64 2074 6865 6e20 7069 636b 206f 6e65  nd then pick one
-00001450: 206f 6620 7468 6520 7468 7265 6520 636f   of the three co
-00001460: 6d6d 616e 6473 2062 656c 6f77 2074 6f20  mmands below to 
-00001470: 696e 7374 616c 6c20 5a6f 6f62 6f74 2061  install Zoobot a
-00001480: 6e64 2065 6974 6865 7220 5079 546f 7263  nd either PyTorc
-00001490: 6820 2872 6563 6f6d 6d65 6e64 6564 2920  h (recommended) 
-000014a0: 6f72 2054 656e 736f 7246 6c6f 773a 0a0a  or TensorFlow:..
-000014b0: 2020 2020 2320 5a6f 6f62 6f74 2077 6974      # Zoobot wit
-000014c0: 6820 5079 546f 7263 6820 616e 6420 6120  h PyTorch and a 
-000014d0: 4750 552e 2052 6571 7569 7265 7320 4355  GPU. Requires CU
-000014e0: 4441 2031 312e 332e 0a20 2020 2070 6970  DA 11.3..    pip
-000014f0: 2069 6e73 7461 6c6c 202d 6520 227a 6f6f   install -e "zoo
-00001500: 626f 745b 7079 746f 7263 685f 6375 3131  bot[pytorch_cu11
-00001510: 335d 2220 2d2d 6578 7472 612d 696e 6465  3]" --extra-inde
-00001520: 782d 7572 6c20 6874 7470 733a 2f2f 646f  x-url https://do
-00001530: 776e 6c6f 6164 2e70 7974 6f72 6368 2e6f  wnload.pytorch.o
-00001540: 7267 2f77 686c 2f63 7531 3133 0a0a 2020  rg/whl/cu113..  
-00001550: 2020 2320 4f52 205a 6f6f 626f 7420 7769    # OR Zoobot wi
-00001560: 7468 2050 7954 6f72 6368 2061 6e64 206e  th PyTorch and n
-00001570: 6f20 4750 550a 2020 2020 7069 7020 696e  o GPU.    pip in
-00001580: 7374 616c 6c20 2d65 2022 7a6f 6f62 6f74  stall -e "zoobot
-00001590: 5b70 7974 6f72 6368 5f63 7075 5d22 202d  [pytorch_cpu]" -
-000015a0: 2d65 7874 7261 2d69 6e64 6578 2d75 726c  -extra-index-url
-000015b0: 2068 7474 7073 3a2f 2f64 6f77 6e6c 6f61   https://downloa
-000015c0: 642e 7079 746f 7263 682e 6f72 672f 7768  d.pytorch.org/wh
-000015d0: 6c2f 6370 750a 0a20 2020 2023 204f 5220  l/cpu..    # OR 
-000015e0: 5a6f 6f62 6f74 2077 6974 6820 5079 546f  Zoobot with PyTo
-000015f0: 7263 6820 6f6e 204d 6163 2077 6974 6820  rch on Mac with 
-00001600: 4d31 2063 6869 700a 2020 2020 7069 7020  M1 chip.    pip 
-00001610: 696e 7374 616c 6c20 2d65 2022 7a6f 6f62  install -e "zoob
-00001620: 6f74 5b70 7974 6f72 6368 5f6d 315d 220a  ot[pytorch_m1]".
-00001630: 0a20 2020 2023 204f 5220 5a6f 6f62 6f74  .    # OR Zoobot
-00001640: 2077 6974 6820 5465 6e73 6f72 466c 6f77   with TensorFlow
-00001650: 2e20 576f 726b 7320 7769 7468 2061 6e64  . Works with and
-00001660: 2077 6974 686f 7574 2061 2047 5055 2c20   without a GPU, 
-00001670: 6275 7420 6966 2079 6f75 2068 6176 6520  but if you have 
-00001680: 6120 4750 552c 2079 6f75 206e 6565 6420  a GPU, you need 
-00001690: 4355 4441 2031 312e 322e 200a 2020 2020  CUDA 11.2. .    
-000016a0: 7069 7020 696e 7374 616c 6c20 2d65 2022  pip install -e "
-000016b0: 7a6f 6f62 6f74 5b74 656e 736f 7266 6c6f  zoobot[tensorflo
-000016c0: 775d 0a0a 5468 6973 2069 6e73 7461 6c6c  w]..This install
-000016d0: 7320 7468 6520 646f 776e 6c6f 6164 6564  s the downloaded
-000016e0: 205a 6f6f 626f 7420 636f 6465 2075 7369   Zoobot code usi
-000016f0: 6e67 2070 6970 205b 6564 6974 6162 6c65  ng pip [editable
-00001700: 206d 6f64 655d 2868 7474 7073 3a2f 2f70   mode](https://p
-00001710: 6970 2e70 7970 612e 696f 2f65 6e2f 7374  ip.pypa.io/en/st
-00001720: 6162 6c65 2f74 6f70 6963 732f 6c6f 6361  able/topics/loca
-00001730: 6c2d 7072 6f6a 6563 742d 696e 7374 616c  l-project-instal
-00001740: 6c73 2f23 6564 6974 6162 6c65 2d69 6e73  ls/#editable-ins
-00001750: 7461 6c6c 7329 2073 6f20 796f 7520 6361  talls) so you ca
-00001760: 6e20 6561 7369 6c79 2063 6861 6e67 6520  n easily change 
-00001770: 7468 6520 636f 6465 206c 6f63 616c 6c79  the code locally
-00001780: 2e20 5a6f 6f62 6f74 2069 7320 616c 736f  . Zoobot is also
-00001790: 2061 7661 696c 6162 6c65 2064 6972 6563   available direc
-000017a0: 746c 7920 6672 6f6d 2070 6970 2028 6070  tly from pip (`p
-000017b0: 6970 2069 6e73 7461 6c6c 207a 6f6f 626f  ip install zoobo
-000017c0: 745b 6f70 7469 6f6e 5d60 292e 204f 6e6c  t[option]`). Onl
-000017d0: 7920 7573 6520 7468 6973 2069 6620 796f  y use this if yo
-000017e0: 7520 6172 6520 7375 7265 2079 6f75 2077  u are sure you w
-000017f0: 6f6e 2774 2062 6520 6d61 6b69 6e67 2063  on't be making c
-00001800: 6861 6e67 6573 2074 6f20 5a6f 6f62 6f74  hanges to Zoobot
-00001810: 2069 7473 656c 662e 2046 6f72 2047 6f6f   itself. For Goo
-00001820: 676c 6520 436f 6c61 622c 2075 7365 2060  gle Colab, use `
-00001830: 7069 7020 696e 7374 616c 6c20 7a6f 6f62  pip install zoob
-00001840: 6f74 5b70 7974 6f72 6368 5f63 6f6c 6162  ot[pytorch_colab
-00001850: 5d60 0a0a 546f 2075 7365 2061 2047 5055  ]`..To use a GPU
-00001860: 2c20 796f 7520 6d75 7374 202a 616c 7265  , you must *alre
-00001870: 6164 792a 2068 6176 6520 4355 4441 2069  ady* have CUDA i
-00001880: 6e73 7461 6c6c 6564 2061 6e64 206d 6174  nstalled and mat
-00001890: 6368 696e 6720 7468 6520 7665 7273 696f  ching the versio
-000018a0: 6e73 2061 626f 7665 2e0a 4920 7368 6172  ns above..I shar
-000018b0: 6520 6d79 2069 6e73 7461 6c6c 2073 7465  e my install ste
-000018c0: 7073 205b 6865 7265 5d28 2369 6e73 7461  ps [here](#insta
-000018d0: 6c6c 5f63 7564 6129 2e20 4750 5573 2061  ll_cuda). GPUs a
-000018e0: 7265 206f 7074 696f 6e61 6c20 2d20 5a6f  re optional - Zo
-000018f0: 6f62 6f74 2077 696c 6c20 7275 6e20 7265  obot will run re
-00001900: 7472 6169 6e20 6669 6e65 206f 6e20 4350  train fine on CP
-00001910: 552c 206a 7573 7420 736c 6f77 6572 2e0a  U, just slower..
-00001920: 0a23 2320 5175 6963 6b73 7461 7274 0a3c  .## Quickstart.<
-00001930: 6120 6e61 6d65 3d22 7175 6963 6b73 7461  a name="quicksta
-00001940: 7274 223e 3c2f 613e 0a0a 5468 6520 5b43  rt"></a>..The [C
-00001950: 6f6c 6162 206e 6f74 6562 6f6f 6b5d 2868  olab notebook](h
-00001960: 7474 7073 3a2f 2f63 6f6c 6162 2e72 6573  ttps://colab.res
-00001970: 6561 7263 682e 676f 6f67 6c65 2e63 6f6d  earch.google.com
-00001980: 2f64 7269 7665 2f31 3762 625f 4b62 4132  /drive/17bb_KbA2
-00001990: 4a36 7972 496d 3470 3455 655f 6c45 4248  J6yrIm4p4Ue_lEBH
-000019a0: 4d4e 4331 4939 4a64 3f75 7370 3d73 6861  MNC1I9Jd?usp=sha
-000019b0: 7269 6e67 2920 6973 2074 6865 2071 7569  ring) is the qui
-000019c0: 636b 6573 7420 7761 7920 746f 2067 6574  ckest way to get
-000019d0: 2073 7461 7274 6564 2e20 416c 7465 726e   started. Altern
-000019e0: 6174 6976 656c 792c 2074 6865 206d 696e  atively, the min
-000019f0: 696d 616c 2065 7861 6d70 6c65 2062 656c  imal example bel
-00001a00: 6f77 2069 6c6c 7573 7472 6174 6573 2068  ow illustrates h
-00001a10: 6f77 205a 6f6f 626f 7420 776f 726b 732e  ow Zoobot works.
-00001a20: 0a0a 4c65 7427 7320 7361 7920 796f 7520  ..Let's say you 
-00001a30: 7761 6e74 2074 6f20 6669 6e64 2072 696e  want to find rin
-00001a40: 6765 6420 6761 6c61 7869 6573 2061 6e64  ged galaxies and
-00001a50: 2079 6f75 2068 6176 6520 6120 736d 616c   you have a smal
-00001a60: 6c20 6c61 6265 6c6c 6564 2064 6174 6173  l labelled datas
-00001a70: 6574 206f 6620 3530 3020 7269 6e67 6564  et of 500 ringed
-00001a80: 206f 7220 6e6f 742d 7269 6e67 6564 2067   or not-ringed g
-00001a90: 616c 6178 6965 732e 2059 6f75 2063 616e  alaxies. You can
-00001aa0: 2072 6574 7261 696e 205a 6f6f 626f 7420   retrain Zoobot 
-00001ab0: 746f 2066 696e 6420 7269 6e67 7320 6c69  to find rings li
-00001ac0: 6b65 2073 6f3a 0a0a 6060 6070 7974 686f  ke so:..```pytho
-00001ad0: 6e0a 0a20 2020 2069 6d70 6f72 7420 7061  n..    import pa
-00001ae0: 6e64 6173 2061 7320 7064 0a20 2020 2066  ndas as pd.    f
-00001af0: 726f 6d20 6761 6c61 7879 5f64 6174 6173  rom galaxy_datas
-00001b00: 6574 732e 7079 746f 7263 682e 6761 6c61  ets.pytorch.gala
-00001b10: 7879 5f64 6174 616d 6f64 756c 6520 696d  xy_datamodule im
-00001b20: 706f 7274 2047 616c 6178 7944 6174 614d  port GalaxyDataM
-00001b30: 6f64 756c 650a 2020 2020 6672 6f6d 207a  odule.    from z
-00001b40: 6f6f 626f 742e 7079 746f 7263 682e 7472  oobot.pytorch.tr
-00001b50: 6169 6e69 6e67 2069 6d70 6f72 7420 6669  aining import fi
-00001b60: 6e65 7475 6e65 0a0a 2020 2020 2320 6373  netune..    # cs
-00001b70: 7620 7769 7468 2027 7269 6e67 2720 636f  v with 'ring' co
-00001b80: 6c75 6d6e 2028 3020 6f72 2031 2920 616e  lumn (0 or 1) an
-00001b90: 6420 2766 696c 655f 6c6f 6327 2063 6f6c  d 'file_loc' col
-00001ba0: 756d 6e20 2870 6174 6820 746f 2069 6d61  umn (path to ima
-00001bb0: 6765 290a 2020 2020 6c61 6265 6c6c 6564  ge).    labelled
-00001bc0: 5f64 6620 3d20 7064 2e72 6561 645f 6373  _df = pd.read_cs
-00001bd0: 7628 272f 796f 7572 2f70 6174 682f 736f  v('/your/path/so
-00001be0: 6d65 5f6c 6162 656c 6c65 645f 6761 6c61  me_labelled_gala
-00001bf0: 7869 6573 2e63 7376 2729 0a0a 2020 2020  xies.csv')..    
-00001c00: 6461 7461 6d6f 6475 6c65 203d 2047 616c  datamodule = Gal
-00001c10: 6178 7944 6174 614d 6f64 756c 6528 0a20  axyDataModule(. 
-00001c20: 2020 2020 206c 6162 656c 5f63 6f6c 733d       label_cols=
-00001c30: 5b27 7269 6e67 275d 2c0a 2020 2020 2020  ['ring'],.      
-00001c40: 6361 7461 6c6f 673d 6c61 6265 6c6c 6564  catalog=labelled
-00001c50: 5f64 662c 0a20 2020 2020 2062 6174 6368  _df,.      batch
-00001c60: 5f73 697a 653d 3332 0a20 2020 2029 0a0a  _size=32.    )..
-00001c70: 2020 2020 2320 6c6f 6164 2074 7261 696e      # load train
-00001c80: 6564 205a 6f6f 626f 7420 6d6f 6465 6c0a  ed Zoobot model.
-00001c90: 2020 2020 6d6f 6465 6c20 3d20 6669 6e65      model = fine
-00001ca0: 7475 6e65 2e46 696e 6574 756e 6561 626c  tune.Finetuneabl
-00001cb0: 655a 6f6f 626f 7443 6c61 7373 6966 6965  eZoobotClassifie
-00001cc0: 7228 6368 6563 6b70 6f69 6e74 5f6c 6f63  r(checkpoint_loc
-00001cd0: 2c20 6e75 6d5f 636c 6173 7365 733d 3229  , num_classes=2)
-00001ce0: 2020 0a20 2020 200a 2020 2020 2320 7265    .    .    # re
-00001cf0: 7472 6169 6e20 746f 2066 696e 6420 7269  train to find ri
-00001d00: 6e67 730a 2020 2020 7472 6169 6e65 7220  ngs.    trainer 
-00001d10: 3d20 6669 6e65 7475 6e65 2e67 6574 5f74  = finetune.get_t
-00001d20: 7261 696e 6572 2873 6176 655f 6469 7229  rainer(save_dir)
-00001d30: 0a20 2020 2074 7261 696e 6572 2e66 6974  .    trainer.fit
-00001d40: 286d 6f64 656c 2c20 6461 7461 6d6f 6475  (model, datamodu
-00001d50: 6c65 290a 6060 600a 0a54 6865 6e20 796f  le).```..Then yo
-00001d60: 7520 6361 6e20 6d61 6b65 2070 7265 6469  u can make predi
-00001d70: 6374 2069 6620 6e65 7720 6761 6c61 7869  ct if new galaxi
-00001d80: 6573 2068 6176 6520 7269 6e67 733a 0a0a  es have rings:..
-00001d90: 6060 6070 7974 686f 6e0a 2020 2020 6672  ```python.    fr
-00001da0: 6f6d 207a 6f6f 626f 742e 7079 746f 7263  om zoobot.pytorc
-00001db0: 682e 7072 6564 6963 7469 6f6e 7320 696d  h.predictions im
-00001dc0: 706f 7274 2070 7265 6469 6374 5f6f 6e5f  port predict_on_
-00001dd0: 6361 7461 6c6f 670a 0a20 2020 2023 2063  catalog..    # c
-00001de0: 7376 2077 6974 6820 2766 696c 655f 6c6f  sv with 'file_lo
-00001df0: 6327 2063 6f6c 756d 6e20 2870 6174 6820  c' column (path 
-00001e00: 746f 2069 6d61 6765 292e 205a 6f6f 626f  to image). Zoobo
-00001e10: 7420 7769 6c6c 2070 7265 6469 6374 2074  t will predict t
-00001e20: 6865 206c 6162 656c 732e 0a20 2020 2075  he labels..    u
-00001e30: 6e6c 6162 656c 6c65 645f 6466 203d 2070  nlabelled_df = p
-00001e40: 642e 7265 6164 5f63 7376 2827 2f79 6f75  d.read_csv('/you
-00001e50: 722f 7061 7468 2f73 6f6d 655f 756e 6c61  r/path/some_unla
-00001e60: 6265 6c6c 6564 5f67 616c 6178 6965 732e  belled_galaxies.
-00001e70: 6373 7627 290a 0a20 2020 2070 7265 6469  csv')..    predi
-00001e80: 6374 5f6f 6e5f 6361 7461 6c6f 672e 7072  ct_on_catalog.pr
-00001e90: 6564 6963 7428 0a20 2020 2020 2075 6e6c  edict(.      unl
-00001ea0: 6162 656c 6c65 645f 6466 2c0a 2020 2020  abelled_df,.    
-00001eb0: 2020 6d6f 6465 6c2c 0a20 2020 2020 206c    model,.      l
-00001ec0: 6162 656c 5f63 6f6c 733d 5b27 7269 6e67  abel_cols=['ring
-00001ed0: 275d 2c20 2023 206f 6e6c 7920 7573 6564  '],  # only used
-00001ee0: 2066 6f72 200a 2020 2020 2020 7361 7665   for .      save
-00001ef0: 5f6c 6f63 3d27 2f79 6f75 722f 7061 7468  _loc='/your/path
-00001f00: 2f66 696e 6574 756e 6564 5f70 7265 6469  /finetuned_predi
-00001f10: 6374 696f 6e73 2e63 7376 270a 2020 2020  ctions.csv'.    
-00001f20: 290a 6060 600a 0a5a 6f6f 626f 7420 696e  ).```..Zoobot in
-00001f30: 636c 7564 6573 206d 616e 7920 6775 6964  cludes many guid
-00001f40: 6573 2061 6e64 2077 6f72 6b69 6e67 2065  es and working e
-00001f50: 7861 6d70 6c65 7320 2d20 7365 6520 7468  xamples - see th
-00001f60: 6520 5b47 6574 7469 6e67 2053 7461 7274  e [Getting Start
-00001f70: 6564 5d28 2367 6574 7469 6e67 2d73 7461  ed](#getting-sta
-00001f80: 7274 6564 2920 7365 6374 696f 6e20 6265  rted) section be
-00001f90: 6c6f 772e 0a0a 2323 2047 6574 7469 6e67  low...## Getting
-00001fa0: 2053 7461 7274 6564 0a3c 6120 6e61 6d65   Started.<a name
-00001fb0: 3d22 6765 7474 696e 675f 7374 6172 7465  ="getting_starte
-00001fc0: 6422 3e3c 2f61 3e0a 0a49 2073 7567 6765  d"></a>..I sugge
-00001fd0: 7374 2073 7461 7274 696e 6720 7769 7468  st starting with
-00001fe0: 2074 6865 205b 436f 6c61 6220 6e6f 7465   the [Colab note
-00001ff0: 626f 6f6b 5d28 6874 7470 733a 2f2f 636f  book](https://co
-00002000: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-00002010: 676c 652e 636f 6d2f 6472 6976 652f 3137  gle.com/drive/17
-00002020: 6262 5f4b 6241 324a 3679 7249 6d34 7034  bb_KbA2J6yrIm4p4
-00002030: 5565 5f6c 4542 484d 4e43 3149 394a 643f  Ue_lEBHMNC1I9Jd?
-00002040: 7573 703d 7368 6172 696e 6729 206f 7220  usp=sharing) or 
-00002050: 7468 6520 776f 726b 6564 2065 7861 6d70  the worked examp
-00002060: 6c65 7320 6265 6c6f 772c 2077 6869 6368  les below, which
-00002070: 2079 6f75 2063 616e 2063 6f70 7920 616e   you can copy an
-00002080: 6420 6164 6170 742e 0a0a 466f 7220 636f  d adapt...For co
-00002090: 6e74 6578 7420 616e 6420 6578 706c 616e  ntext and explan
-000020a0: 6174 696f 6e2c 2073 6565 2074 6865 205b  ation, see the [
-000020b0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-000020c0: 7474 7073 3a2f 2f7a 6f6f 626f 742e 7265  ttps://zoobot.re
-000020d0: 6164 7468 6564 6f63 732e 696f 2f29 2e0a  adthedocs.io/)..
-000020e0: 0a46 6f72 2070 7265 7472 6169 6e65 6420  .For pretrained 
-000020f0: 6d6f 6465 6c20 7765 6967 6874 732c 2070  model weights, p
-00002100: 7265 6361 6c63 756c 6174 6564 2072 6570  recalculated rep
-00002110: 7265 7365 6e74 6174 696f 6e73 2c20 6361  resentations, ca
-00002120: 7461 6c6f 6775 6573 2c20 616e 6420 736f  talogues, and so
-00002130: 2066 6f72 7468 2c20 7365 6520 7468 6520   forth, see the 
-00002140: 5b64 6174 6120 6e6f 7465 735d 2868 7474  [data notes](htt
-00002150: 7073 3a2f 2f7a 6f6f 626f 742e 7265 6164  ps://zoobot.read
-00002160: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-00002170: 7465 7374 2f64 6174 615f 6e6f 7465 732e  test/data_notes.
-00002180: 6874 6d6c 2920 696e 2070 6172 7469 6375  html) in particu
-00002190: 6c61 722e 0a0a 2323 2320 576f 726b 6564  lar...### Worked
-000021a0: 2045 7861 6d70 6c65 730a 3c61 206e 616d   Examples.<a nam
-000021b0: 653d 2277 6f72 6b65 645f 6578 616d 706c  e="worked_exampl
-000021c0: 6573 223e 3c2f 613e 0a0a 5079 546f 7263  es"></a>..PyTorc
-000021d0: 6820 2872 6563 6f6d 6d65 6e64 6564 293a  h (recommended):
-000021e0: 0a2d 205b 7079 746f 7263 682f 6578 616d  .- [pytorch/exam
-000021f0: 706c 6573 2f66 696e 6574 756e 696e 672f  ples/finetuning/
-00002200: 6669 6e65 7475 6e65 5f62 696e 6172 795f  finetune_binary_
-00002210: 636c 6173 7369 6669 6361 7469 6f6e 2e70  classification.p
-00002220: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-00002230: 622e 636f 6d2f 6d77 616c 6d73 6c65 792f  b.com/mwalmsley/
-00002240: 7a6f 6f62 6f74 2f62 6c6f 622f 6d61 696e  zoobot/blob/main
-00002250: 2f7a 6f6f 626f 742f 7079 746f 7263 682f  /zoobot/pytorch/
-00002260: 6578 616d 706c 6573 2f66 696e 6574 756e  examples/finetun
-00002270: 696e 672f 6669 6e65 7475 6e65 5f62 696e  ing/finetune_bin
-00002280: 6172 795f 636c 6173 7369 6669 6361 7469  ary_classificati
-00002290: 6f6e 2e70 7929 0a2d 205b 7079 746f 7263  on.py).- [pytorc
-000022a0: 682f 6578 616d 706c 6573 2f66 696e 6574  h/examples/finet
-000022b0: 756e 696e 672f 6669 6e65 7475 6e65 5f63  uning/finetune_c
-000022c0: 6f75 6e74 735f 6675 6c6c 5f74 7265 652e  ounts_full_tree.
-000022d0: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-000022e0: 7562 2e63 6f6d 2f6d 7761 6c6d 736c 6579  ub.com/mwalmsley
-000022f0: 2f7a 6f6f 626f 742f 626c 6f62 2f6d 6169  /zoobot/blob/mai
-00002300: 6e2f 7a6f 6f62 6f74 2f70 7974 6f72 6368  n/zoobot/pytorch
-00002310: 2f65 7861 6d70 6c65 732f 6669 6e65 7475  /examples/finetu
-00002320: 6e69 6e67 2f66 696e 6574 756e 655f 636f  ning/finetune_co
-00002330: 756e 7473 5f66 756c 6c5f 7472 6565 2e70  unts_full_tree.p
-00002340: 7929 0a2d 205b 7079 746f 7263 682f 6578  y).- [pytorch/ex
-00002350: 616d 706c 6573 2f72 6570 7265 7365 6e74  amples/represent
-00002360: 6174 696f 6e73 2f67 6574 5f72 6570 7265  ations/get_repre
-00002370: 7365 6e74 6174 696f 6e73 2e70 795d 2868  sentations.py](h
-00002380: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002390: 6d2f 6d77 616c 6d73 6c65 792f 7a6f 6f62  m/mwalmsley/zoob
-000023a0: 6f74 2f62 6c6f 622f 6d61 696e 2f7a 6f6f  ot/blob/main/zoo
-000023b0: 626f 742f 7079 746f 7263 682f 6578 616d  bot/pytorch/exam
-000023c0: 706c 6573 2f72 6570 7265 7365 6e74 6174  ples/representat
-000023d0: 696f 6e73 2f67 6574 5f72 6570 7265 7365  ions/get_represe
-000023e0: 6e74 6174 696f 6e73 2e70 7929 0a2d 205b  ntations.py).- [
-000023f0: 7079 746f 7263 682f 6578 616d 706c 6573  pytorch/examples
-00002400: 2f74 7261 696e 5f6d 6f64 656c 5f6f 6e5f  /train_model_on_
-00002410: 6361 7461 6c6f 672e 7079 5d28 6874 7470  catalog.py](http
-00002420: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00002430: 7761 6c6d 736c 6579 2f7a 6f6f 626f 742f  walmsley/zoobot/
-00002440: 626c 6f62 2f6d 6169 6e2f 7a6f 6f62 6f74  blob/main/zoobot
-00002450: 2f70 7974 6f72 6368 2f65 7861 6d70 6c65  /pytorch/example
-00002460: 732f 7472 6169 6e5f 6d6f 6465 6c5f 6f6e  s/train_model_on
-00002470: 5f63 6174 616c 6f67 2e70 7929 2028 6f6e  _catalog.py) (on
-00002480: 6c79 206e 6563 6573 7361 7279 2074 6f20  ly necessary to 
-00002490: 7472 6169 6e20 6672 6f6d 2073 6372 6174  train from scrat
-000024a0: 6368 290a 0a54 656e 736f 7246 6c6f 773a  ch)..TensorFlow:
-000024b0: 0a2d 205b 7465 6e73 6f72 666c 6f77 2f65  .- [tensorflow/e
-000024c0: 7861 6d70 6c65 732f 7472 6169 6e5f 6d6f  xamples/train_mo
-000024d0: 6465 6c5f 6f6e 5f63 6174 616c 6f67 2e70  del_on_catalog.p
-000024e0: 795d 2868 7474 7073 3a2f 2f67 6974 6875  y](https://githu
-000024f0: 622e 636f 6d2f 6d77 616c 6d73 6c65 792f  b.com/mwalmsley/
-00002500: 7a6f 6f62 6f74 2f62 6c6f 622f 6d61 696e  zoobot/blob/main
-00002510: 2f7a 6f6f 626f 742f 7465 6e73 6f72 666c  /zoobot/tensorfl
-00002520: 6f77 2f65 7861 6d70 6c65 732f 7472 6169  ow/examples/trai
-00002530: 6e5f 6d6f 6465 6c5f 6f6e 5f63 6174 616c  n_model_on_catal
-00002540: 6f67 2e70 7929 2028 6f6e 6c79 206e 6563  og.py) (only nec
-00002550: 6573 7361 7279 2074 6f20 7472 6169 6e20  essary to train 
-00002560: 6672 6f6d 2073 6372 6174 6368 290a 2d20  from scratch).- 
-00002570: 5b74 656e 736f 7266 6c6f 772f 6578 616d  [tensorflow/exam
-00002580: 706c 6573 2f6d 616b 655f 7072 6564 6963  ples/make_predic
-00002590: 7469 6f6e 732e 7079 5d28 6874 7470 733a  tions.py](https:
-000025a0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 7761  //github.com/mwa
-000025b0: 6c6d 736c 6579 2f7a 6f6f 626f 742f 626c  lmsley/zoobot/bl
-000025c0: 6f62 2f6d 6169 6e2f 7a6f 6f62 6f74 2f74  ob/main/zoobot/t
-000025d0: 656e 736f 7266 6c6f 772f 6578 616d 706c  ensorflow/exampl
-000025e0: 6573 2f6d 616b 655f 7072 6564 6963 7469  es/make_predicti
-000025f0: 6f6e 732e 7079 290a 2d20 5b74 656e 736f  ons.py).- [tenso
-00002600: 7266 6c6f 772f 6578 616d 706c 6573 2f66  rflow/examples/f
-00002610: 696e 6574 756e 655f 6d69 6e69 6d61 6c2e  inetune_minimal.
-00002620: 7079 5d28 6874 7470 733a 2f2f 6769 7468  py](https://gith
-00002630: 7562 2e63 6f6d 2f6d 7761 6c6d 736c 6579  ub.com/mwalmsley
-00002640: 2f7a 6f6f 626f 742f 626c 6f62 2f6d 6169  /zoobot/blob/mai
-00002650: 6e2f 7a6f 6f62 6f74 2f74 656e 736f 7266  n/zoobot/tensorf
-00002660: 6c6f 772f 6578 616d 706c 6573 2f66 696e  low/examples/fin
-00002670: 6574 756e 655f 6d69 6e69 6d61 6c2e 7079  etune_minimal.py
-00002680: 290a 2d20 5b74 656e 736f 7266 6c6f 772f  ).- [tensorflow/
-00002690: 6578 616d 706c 6573 2f66 696e 6574 756e  examples/finetun
-000026a0: 655f 6164 7661 6e63 6564 2e70 795d 2868  e_advanced.py](h
-000026b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000026c0: 6d2f 6d77 616c 6d73 6c65 792f 7a6f 6f62  m/mwalmsley/zoob
-000026d0: 6f74 2f62 6c6f 622f 6d61 696e 2f7a 6f6f  ot/blob/main/zoo
-000026e0: 626f 742f 7465 6e73 6f72 666c 6f77 2f65  bot/tensorflow/e
-000026f0: 7861 6d70 6c65 732f 6669 6e65 7475 6e65  xamples/finetune
-00002700: 5f61 6476 616e 6365 642e 7079 290a 0a54  _advanced.py)..T
-00002710: 6865 7265 2069 7320 6d6f 7265 2065 7870  here is more exp
-00002720: 6c61 6e61 7469 6f6e 2061 6e64 2061 6e20  lanation and an 
-00002730: 4150 4920 7265 6665 7265 6e63 6520 6f6e  API reference on
-00002740: 2074 6865 205b 646f 6373 5d28 6874 7470   the [docs](http
-00002750: 733a 2f2f 7a6f 6f62 6f74 2e72 6561 6474  s://zoobot.readt
-00002760: 6865 646f 6373 2e69 6f2f 292e 0a0a 4920  hedocs.io/)...I 
-00002770: 616c 736f 205b 696e 636c 7564 655d 2868  also [include](h
-00002780: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002790: 6d2f 6d77 616c 6d73 6c65 792f 7a6f 6f62  m/mwalmsley/zoob
-000027a0: 6f74 2f62 6c6f 622f 6d61 696e 2f62 656e  ot/blob/main/ben
-000027b0: 6368 6d61 726b 7329 2074 6865 2073 6372  chmarks) the scr
-000027c0: 6970 7473 2075 7365 6420 746f 2063 7265  ipts used to cre
-000027d0: 6174 6520 616e 6420 6265 6e63 686d 6172  ate and benchmar
-000027e0: 6b20 6f75 7220 7072 6574 7261 696e 6564  k our pretrained
-000027f0: 206d 6f64 656c 732e 204d 616e 7920 7072   models. Many pr
-00002800: 6574 7261 696e 6564 206d 6f64 656c 7320  etrained models 
-00002810: 6172 6520 6176 6169 6c61 626c 6520 5b61  are available [a
-00002820: 6c72 6561 6479 5d28 6874 7470 733a 2f2f  lready](https://
-00002830: 7a6f 6f62 6f74 2e72 6561 6474 6865 646f  zoobot.readthedo
-00002840: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00002850: 6461 7461 5f6e 6f74 6573 2e68 746d 6c29  data_notes.html)
-00002860: 2c20 6275 7420 6966 2079 6f75 206e 6565  , but if you nee
-00002870: 6420 6f6e 6520 7472 6169 6e65 6420 6f6e  d one trained on
-00002880: 2065 2e67 2e20 6469 6666 6572 656e 7420   e.g. different 
-00002890: 696e 7075 7420 696d 6167 6520 7369 7a65  input image size
-000028a0: 7320 6f72 2077 6974 6820 6120 7370 6563  s or with a spec
-000028b0: 6966 6963 2061 7263 6869 7465 6374 7572  ific architectur
-000028c0: 652c 2049 2063 616e 2070 726f 6261 626c  e, I can probabl
-000028d0: 7920 6d61 6b65 2069 7420 666f 7220 796f  y make it for yo
-000028e0: 752e 0a0a 5768 656e 2074 7261 696e 6564  u...When trained
-000028f0: 2077 6974 6820 6120 6465 6369 7369 6f6e   with a decision
-00002900: 2074 7265 6520 6865 6164 2028 5a6f 6f62   tree head (Zoob
-00002910: 6f74 5472 6565 2c20 4669 6e65 7475 6e65  otTree, Finetune
-00002920: 6162 6c65 5a6f 6f62 6f74 5472 6565 292c  ableZoobotTree),
-00002930: 205a 6f6f 626f 7420 6361 6e20 6c65 6172   Zoobot can lear
-00002940: 6e20 6672 6f6d 2076 6f6c 756e 7465 6572  n from volunteer
-00002950: 206c 6162 656c 7320 6f66 2076 6172 7969   labels of varyi
-00002960: 6e67 2063 6f6e 6669 6465 6e63 6520 616e  ng confidence an
-00002970: 6420 7072 6564 6963 7420 706f 7374 6572  d predict poster
-00002980: 696f 7273 2066 6f72 2077 6861 7420 7468  iors for what th
-00002990: 6520 7479 7069 6361 6c20 766f 6c75 6e74  e typical volunt
-000029a0: 6565 7220 6d69 6768 7420 7361 792e 2053  eer might say. S
-000029b0: 7065 6369 6669 6361 6c6c 792c 2074 6869  pecifically, thi
-000029c0: 7320 5a6f 6f62 6f74 206d 6f64 6520 7072  s Zoobot mode pr
-000029d0: 6564 6963 7473 2074 6865 2070 6172 616d  edicts the param
-000029e0: 6574 6572 7320 666f 7220 6469 7374 7269  eters for distri
-000029f0: 6275 7469 6f6e 732c 206e 6f74 2073 696d  butions, not sim
-00002a00: 706c 6520 636c 6173 7320 6c61 6265 6c73  ple class labels
-00002a10: 2120 466f 7220 6120 6465 6d6f 6e73 7472  ! For a demonstr
-00002a20: 6174 696f 6e20 6f66 2068 6f77 2074 6f20  ation of how to 
-00002a30: 696e 7465 7270 7265 7420 7468 6573 6520  interpret these 
-00002a40: 7072 6564 6963 7469 6f6e 732c 2073 6565  predictions, see
-00002a50: 2074 6865 205b 677a 5f64 6563 616c 735f   the [gz_decals_
-00002a60: 6461 7461 5f72 656c 6561 7365 5f61 6e61  data_release_ana
-00002a70: 6c79 7369 735f 6465 6d6f 2e69 7079 6e62  lysis_demo.ipynb
-00002a80: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00002a90: 2e63 6f6d 2f6d 7761 6c6d 736c 6579 2f7a  .com/mwalmsley/z
-00002aa0: 6f6f 626f 742f 626c 6f62 2f6d 6169 6e2f  oobot/blob/main/
-00002ab0: 677a 5f64 6563 616c 735f 6461 7461 5f72  gz_decals_data_r
-00002ac0: 656c 6561 7365 5f61 6e61 6c79 7369 735f  elease_analysis_
-00002ad0: 6465 6d6f 2e69 7079 6e62 292e 0a0a 0a0a  demo.ipynb).....
-00002ae0: 2323 2320 284f 7074 696f 6e61 6c29 2049  ### (Optional) I
-00002af0: 6e73 7461 6c6c 2050 7954 6f72 6368 206f  nstall PyTorch o
-00002b00: 7220 5465 6e73 6f72 466c 6f77 2c20 7769  r TensorFlow, wi
-00002b10: 7468 2043 5544 410a 3c61 206e 616d 653d  th CUDA.<a name=
-00002b20: 2269 6e73 7461 6c6c 5f63 7564 6122 3e3c  "install_cuda"><
-00002b30: 2f61 3e0a 0a2a 4966 2079 6f75 2772 6520  /a>..*If you're 
-00002b40: 6e6f 7420 7573 696e 6720 6120 4750 552c  not using a GPU,
-00002b50: 2073 6b69 7020 7468 6973 2073 7465 702e   skip this step.
-00002b60: 2055 7365 2074 6865 2070 7974 6f72 6368   Use the pytorch
-00002b70: 5f63 7075 206f 7220 7465 6e73 6f72 666c  _cpu or tensorfl
-00002b80: 6f77 5f63 7075 206f 7074 696f 6e73 2069  ow_cpu options i
-00002b90: 6e20 7468 6520 7365 6374 696f 6e20 6265  n the section be
-00002ba0: 6c6f 772e 2a0a 0a49 6e73 7461 6c6c 2050  low.*..Install P
-00002bb0: 7954 6f72 6368 2031 2e31 322e 3120 6f72  yTorch 1.12.1 or
-00002bc0: 2054 656e 736f 7266 6c6f 7720 322e 3130   Tensorflow 2.10
-00002bd0: 2e30 2061 6e64 2063 6f6d 7061 7469 626c  .0 and compatibl
-00002be0: 6520 4355 4441 2064 7269 7665 7273 2e20  e CUDA drivers. 
-00002bf0: 4920 6869 6768 6c79 2072 6563 6f6d 6d65  I highly recomme
-00002c00: 6e64 2075 7369 6e67 205b 636f 6e64 615d  nd using [conda]
-00002c10: 2868 7474 7073 3a2f 2f64 6f63 732e 636f  (https://docs.co
-00002c20: 6e64 612e 696f 2f65 6e2f 6c61 7465 7374  nda.io/en/latest
-00002c30: 2f6d 696e 6963 6f6e 6461 2e68 746d 6c29  /miniconda.html)
-00002c40: 2074 6f20 646f 2074 6869 732e 2043 6f6e   to do this. Con
-00002c50: 6461 2077 696c 6c20 6861 6e64 6c65 2062  da will handle b
-00002c60: 6f74 6820 6372 6561 7469 6e67 2061 206e  oth creating a n
-00002c70: 6577 2076 6972 7475 616c 2065 6e76 6972  ew virtual envir
-00002c80: 6f6e 6d65 6e74 2028 6063 6f6e 6461 2063  onment (`conda c
-00002c90: 7265 6174 6560 2920 616e 6420 696e 7374  reate`) and inst
-00002ca0: 616c 6c69 6e67 2043 5544 4120 2860 6375  alling CUDA (`cu
-00002cb0: 6461 746f 6f6c 6b69 7460 2c20 6063 7564  datoolkit`, `cud
-00002cc0: 6e6e 6029 0a0a 4355 4441 2031 312e 3320  nn`)..CUDA 11.3 
-00002cd0: 666f 7220 5079 546f 7263 683a 0a0a 2020  for PyTorch:..  
-00002ce0: 2020 636f 6e64 6120 6372 6561 7465 202d    conda create -
-00002cf0: 2d6e 616d 6520 7a6f 6f62 6f74 3338 5f74  -name zoobot38_t
-00002d00: 6f72 6368 2070 7974 686f 6e3d 3d33 2e38  orch python==3.8
-00002d10: 0a20 2020 2063 6f6e 6461 2061 6374 6976  .    conda activ
-00002d20: 6174 6520 7a6f 6f62 6f74 3338 5f74 6f72  ate zoobot38_tor
-00002d30: 6368 0a20 2020 2063 6f6e 6461 2069 6e73  ch.    conda ins
-00002d40: 7461 6c6c 202d 6320 636f 6e64 612d 666f  tall -c conda-fo
-00002d50: 7267 6520 6375 6461 746f 6f6c 6b69 743d  rge cudatoolkit=
-00002d60: 3131 2e33 0a0a 4355 4441 2031 312e 3220  11.3..CUDA 11.2 
-00002d70: 616e 6420 4355 444e 4e20 382e 3120 666f  and CUDNN 8.1 fo
-00002d80: 7220 5465 6e73 6f72 466c 6f77 2032 2e31  r TensorFlow 2.1
-00002d90: 302e 303a 0a0a 2020 2020 636f 6e64 6120  0.0:..    conda 
-00002da0: 6372 6561 7465 202d 2d6e 616d 6520 7a6f  create --name zo
-00002db0: 6f62 6f74 3338 5f74 6620 7079 7468 6f6e  obot38_tf python
-00002dc0: 3d3d 332e 380a 2020 2020 636f 6e64 6120  ==3.8.    conda 
-00002dd0: 6163 7469 7661 7465 207a 6f6f 626f 7433  activate zoobot3
-00002de0: 385f 7466 0a20 2020 2063 6f6e 6461 2069  8_tf.    conda i
-00002df0: 6e73 7461 6c6c 202d 6320 636f 6e64 612d  nstall -c conda-
-00002e00: 666f 7267 6520 6375 6461 746f 6f6c 6b69  forge cudatoolki
-00002e10: 743d 3131 2e32 2063 7564 6e6e 3d38 2e31  t=11.2 cudnn=8.1
-00002e20: 2e30 0a20 2020 2065 7870 6f72 7420 4c44  .0.    export LD
-00002e30: 5f4c 4942 5241 5259 5f50 4154 483d 244c  _LIBRARY_PATH=$L
-00002e40: 445f 4c49 4252 4152 595f 5041 5448 3a24  D_LIBRARY_PATH:$
-00002e50: 434f 4e44 415f 5052 4546 4958 2f6c 6962  CONDA_PREFIX/lib
-00002e60: 2f20 2023 2061 6464 2074 6869 7320 656e  /  # add this en
-00002e70: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00002e80: 6c65 0a0a 2323 2320 4c61 7465 7374 206d  le..### Latest m
-00002e90: 696e 6f72 2066 6561 7475 7265 7320 2876  inor features (v
-00002ea0: 312e 302e 3429 0a0a 2d20 4e6f 7720 7375  1.0.4)..- Now su
-00002eb0: 7070 6f72 7473 206d 756c 7469 2d63 6c61  pports multi-cla
-00002ec0: 7373 2066 696e 6574 756e 696e 672e 2053  ss finetuning. S
-00002ed0: 6565 2060 7079 746f 7263 682f 6578 616d  ee `pytorch/exam
-00002ee0: 706c 6573 2f66 696e 6574 756e 696e 672f  ples/finetuning/
-00002ef0: 6669 6e65 7475 6e65 5f6d 756c 7469 636c  finetune_multicl
-00002f00: 6173 735f 636c 6173 7369 6669 6361 7469  ass_classificati
-00002f10: 6f6e 2e70 7960 0a2d 2052 656d 6f76 6564  on.py`.- Removed
-00002f20: 2060 7369 6d70 6c65 6a70 6567 6020 6465   `simplejpeg` de
-00002f30: 7065 6e64 656e 6379 2064 7565 2074 6f20  pendency due to 
-00002f40: 4d31 2069 6e73 7461 6c6c 2069 7373 7565  M1 install issue
-00002f50: 2e20 0a2d 2050 696e 6e65 6420 6074 696d  . .- Pinned `tim
-00002f60: 6d60 2076 6572 7369 6f6e 2074 6f20 656e  m` version to en
-00002f70: 7375 7265 204d 6158 2d56 6954 206d 6f64  sure MaX-ViT mod
-00002f80: 656c 7320 6c6f 6164 2063 6f72 7265 6374  els load correct
-00002f90: 6c79 2e20 4d6f 6465 6c73 2073 7570 706f  ly. Models suppo
-00002fa0: 7274 696e 6720 7468 6520 6c61 7465 7374  rting the latest
-00002fb0: 2060 7469 6d6d 6020 7769 6c6c 2066 6f6c   `timm` will fol
-00002fc0: 6c6f 772e 0a2d 2028 696e 7465 726e 616c  low..- (internal
-00002fd0: 2075 6e74 696c 2070 7562 6c69 7368 6564   until published
-00002fe0: 2920 475a 2045 766f 2076 3220 6e6f 7720  ) GZ Evo v2 now 
-00002ff0: 696e 636c 7564 6573 2043 6f73 6d69 6320  includes Cosmic 
-00003000: 4461 776e 2028 4853 4329 2e20 5369 676e  Dawn (HSC). Sign
-00003010: 6966 6963 616e 7420 7065 7266 6f72 6d61  ificant performa
-00003020: 6e63 6520 696d 7072 6f76 656d 656e 7420  nce improvement 
-00003030: 6f6e 2048 5343 2066 696e 6574 756e 696e  on HSC finetunin
-00003040: 672e 0a0a 2323 2320 4c61 7465 7374 206d  g...### Latest m
-00003050: 616a 6f72 2066 6561 7475 7265 7320 2876  ajor features (v
-00003060: 312e 302e 3029 0a0a 7631 2e30 2e30 2072  1.0.0)..v1.0.0 r
-00003070: 6563 6f67 6e69 7365 7320 7468 6174 206d  ecognises that m
-00003080: 6f73 7420 6f66 2074 6865 2063 6f6d 706c  ost of the compl
-00003090: 6578 6974 7920 696e 2074 6869 7320 7265  exity in this re
-000030a0: 706f 2069 7320 7472 6169 6e69 6e67 205a  po is training Z
-000030b0: 6f6f 626f 7420 6672 6f6d 2073 6372 6174  oobot from scrat
-000030c0: 6368 2c20 6275 7420 6d6f 7374 206e 6f6e  ch, but most non
-000030d0: 2d47 5a20 7573 6572 7320 7769 6c6c 2070  -GZ users will p
-000030e0: 726f 6261 626c 7920 7369 6d70 6c79 2077  robably simply w
-000030f0: 616e 7420 746f 206c 6f61 6420 7468 6520  ant to load the 
-00003100: 7072 6574 7261 696e 6564 205a 6f6f 626f  pretrained Zoobo
-00003110: 7420 616e 6420 6669 6e65 7475 6e65 2069  t and finetune i
-00003120: 7420 6f6e 2074 6865 6972 2064 6174 612e  t on their data.
-00003130: 0a0a 2d20 4164 6473 206e 6577 2066 696e  ..- Adds new fin
-00003140: 6574 756e 696e 6720 696e 7465 7266 6163  etuning interfac
-00003150: 6520 2860 6669 6e65 7475 6e65 2e72 756e  e (`finetune.run
-00003160: 5f66 696e 6574 756e 696e 6728 2960 292c  _finetuning()`),
-00003170: 2065 7861 6d70 6c65 732e 0a2d 2052 6566   examples..- Ref
-00003180: 6f63 7573 6573 2064 6f63 7320 6f6e 2066  ocuses docs on f
-00003190: 696e 6574 756e 696e 6720 7261 7468 6572  inetuning rather
-000031a0: 2074 6861 6e20 7472 6169 6e69 6e67 2066   than training f
-000031b0: 726f 6d20 7363 7261 7463 682e 0a2d 2052  rom scratch..- R
-000031c0: 6577 6f72 6b20 696e 7374 616c 6c61 7469  ework installati
-000031d0: 6f6e 2070 726f 6365 7373 2074 6f20 7365  on process to se
-000031e0: 7061 7261 7465 2043 5544 4120 6672 6f6d  parate CUDA from
-000031f0: 205a 6f6f 626f 7420 2873 696d 706c 6572   Zoobot (simpler
-00003200: 2c20 6561 7369 6572 290a 2d20 4265 7474  , easier).- Bett
-00003210: 6572 2077 616e 6462 206c 6f67 6769 6e67  er wandb logging
-00003220: 2074 6872 6f75 6768 6f75 742c 2074 6f20   throughout, to 
-00003230: 6d6f 6e69 746f 7220 7472 6169 6e69 6e67  monitor training
-00003240: 0a2d 2052 656d 6f76 6520 6e65 6564 2074  .- Remove need t
-00003250: 6f20 6d61 6b65 2054 4652 6563 6f72 6473  o make TFRecords
-00003260: 2e20 4e6f 7720 5446 2064 6972 6563 746c  . Now TF directl
-00003270: 7920 7573 6573 2069 6d61 6765 732e 0a2d  y uses images..-
-00003280: 2052 6566 6163 746f 7220 6f75 7420 6175   Refactor out au
-00003290: 676d 656e 7461 7469 6f6e 7320 616e 6420  gmentations and 
-000032a0: 6461 7461 7365 7473 2074 6f20 6067 616c  datasets to `gal
-000032b0: 6178 792d 6461 7461 7365 7473 6020 7265  axy-datasets` re
-000032c0: 706f 2e20 5446 2061 6e64 2054 6f72 6368  po. TF and Torch
-000032d0: 206e 6f77 2075 7365 2069 6465 6e74 6963   now use identic
-000032e0: 616c 2061 7567 6d65 6e74 6174 696f 6e73  al augmentations
-000032f0: 2028 7669 6120 616c 6275 6d65 6e74 6174   (via albumentat
-00003300: 696f 6e73 292e 0a2d 204d 616e 7920 736d  ions)..- Many sm
-00003310: 616c 6c20 7175 616c 6974 792d 6f66 2d6c  all quality-of-l
-00003320: 6966 6520 696d 7072 6f76 656d 656e 7473  ife improvements
-00003330: 0a0a 436f 6e74 7269 6275 7469 6f6e 7320  ..Contributions 
-00003340: 6172 6520 7665 7279 2077 656c 636f 6d65  are very welcome
-00003350: 2061 6e64 2077 696c 6c20 6265 2063 7265   and will be cre
-00003360: 6469 7465 6420 696e 2061 6e79 2066 7574  dited in any fut
-00003370: 7572 6520 776f 726b 2e20 506c 6561 7365  ure work. Please
-00003380: 2067 6574 2069 6e20 746f 7563 6821 2053   get in touch! S
-00003390: 6565 205b 434f 4e54 5249 4255 5449 4e47  ee [CONTRIBUTING
-000033a0: 2e6d 645d 2868 7474 7073 3a2f 2f67 6974  .md](https://git
-000033b0: 6875 622e 636f 6d2f 6d77 616c 6d73 6c65  hub.com/mwalmsle
-000033c0: 792f 7a6f 6f62 6f74 2f62 6c6f 622f 6d61  y/zoobot/blob/ma
-000033d0: 696e 2f62 656e 6368 6d61 726b 7329 2066  in/benchmarks) f
-000033e0: 6f72 206d 6f72 652e 0a0a 2323 2320 4265  or more...### Be
-000033f0: 6e63 686d 6172 6b73 2061 6e64 2052 6570  nchmarks and Rep
-00003400: 6c69 6361 7469 6f6e 202d 2054 7261 696e  lication - Train
-00003410: 696e 6720 6672 6f6d 2053 6372 6174 6368  ing from Scratch
-00003420: 0a0a 5468 6520 5b62 656e 6368 6d61 726b  ..The [benchmark
-00003430: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00003440: 622e 636f 6d2f 6d77 616c 6d73 6c65 792f  b.com/mwalmsley/
-00003450: 7a6f 6f62 6f74 2f62 6c6f 622f 6d61 696e  zoobot/blob/main
-00003460: 2f62 656e 6368 6d61 726b 7329 2066 6f6c  /benchmarks) fol
-00003470: 6465 7220 636f 6e74 6169 6e73 2073 6c75  der contains slu
-00003480: 726d 2061 6e64 2050 7974 686f 6e20 7363  rm and Python sc
-00003490: 7269 7074 7320 746f 2074 7261 696e 205a  ripts to train Z
-000034a0: 6f6f 626f 7420 6672 6f6d 2073 6372 6174  oobot from scrat
-000034b0: 6368 2e20 5765 2075 7365 2074 6865 7365  ch. We use these
-000034c0: 2073 6372 6970 7473 2074 6f20 6d61 6b65   scripts to make
-000034d0: 2073 7572 6520 6e65 7720 636f 6465 2076   sure new code v
-000034e0: 6572 7369 6f6e 7320 776f 726b 2077 656c  ersions work wel
-000034f0: 6c2c 2061 6e64 2074 6861 7420 5465 6e73  l, and that Tens
-00003500: 6f72 466c 6f77 2061 6e64 2050 7954 6f72  orFlow and PyTor
-00003510: 6368 2061 6368 6965 7665 2073 696d 696c  ch achieve simil
-00003520: 6172 2070 6572 666f 726d 616e 6365 2e0a  ar performance..
-00003530: 0a54 7261 696e 696e 6720 5a6f 6f62 6f74  .Training Zoobot
-00003540: 2075 7369 6e67 2074 6865 2047 5a20 4445   using the GZ DE
-00003550: 4361 4c53 2064 6174 6173 6574 206f 7074  CaLS dataset opt
-00003560: 696f 6e20 7769 6c6c 2063 7265 6174 6520  ion will create 
-00003570: 6d6f 6465 6c73 2076 6572 7920 7369 6d69  models very simi
-00003580: 6c61 7220 746f 2074 686f 7365 2075 7365  lar to those use
-00003590: 6420 666f 7220 7468 6520 475a 2044 4543  d for the GZ DEC
-000035a0: 614c 5320 6361 7461 6c6f 6775 6520 616e  aLS catalogue an
-000035b0: 6420 7368 6172 6564 2077 6974 6820 7468  d shared with th
-000035c0: 6520 6561 726c 7920 7665 7273 696f 6e73  e early versions
-000035d0: 206f 6620 7468 6973 2072 6570 6f2e 2054   of this repo. T
-000035e0: 6865 2047 5a20 4445 5349 205a 6f6f 626f  he GZ DESI Zoobo
-000035f0: 7420 6d6f 6465 6c20 6973 2074 7261 696e  t model is train
-00003600: 6564 206f 6e20 6164 6469 7469 6f6e 616c  ed on additional
-00003610: 2064 6174 6120 2847 5a44 2d31 2c20 475a   data (GZD-1, GZ
-00003620: 442d 3229 2c20 6173 2074 6865 2047 5a20  D-2), as the GZ 
-00003630: 4576 6f20 5a6f 6f62 6f74 206d 6f64 656c  Evo Zoobot model
-00003640: 2028 475a 442d 312f 322f 352c 2048 7562   (GZD-1/2/5, Hub
-00003650: 626c 652c 2043 616e 6465 6c73 2c20 475a  ble, Candels, GZ
-00003660: 3229 2e0a 0a23 2323 2043 6974 696e 670a  2)...### Citing.
-00003670: 0a49 6620 796f 7520 7573 6520 7468 6973  .If you use this
-00003680: 2073 6f66 7477 6172 652c 206f 7220 6f74   software, or ot
-00003690: 6865 7277 6973 6520 7769 7368 2074 6f20  herwise wish to 
-000036a0: 6369 7465 205a 6f6f 626f 7420 6173 2061  cite Zoobot as a
-000036b0: 2073 6f66 7477 6172 6520 7061 636b 6167   software packag
-000036c0: 652c 2070 6c65 6173 6520 7573 6520 7468  e, please use th
-000036d0: 6520 5b4a 4f53 5320 7061 7065 725d 2868  e [JOSS paper](h
-000036e0: 7474 7073 3a2f 2f64 6f69 2e6f 7267 2f31  ttps://doi.org/1
-000036f0: 302e 3231 3130 352f 6a6f 7373 2e30 3533  0.21105/joss.053
-00003700: 3132 293a 0a0a 2020 2020 4061 7274 6963  12):..    @artic
-00003710: 6c65 7b57 616c 6d73 6c65 7932 3032 332c  le{Walmsley2023,
-00003720: 2064 6f69 203d 207b 3130 2e32 3131 3035   doi = {10.21105
-00003730: 2f6a 6f73 732e 3035 3331 327d 2c20 7572  /joss.05312}, ur
-00003740: 6c20 3d20 7b68 7474 7073 3a2f 2f64 6f69  l = {https://doi
-00003750: 2e6f 7267 2f31 302e 3231 3130 352f 6a6f  .org/10.21105/jo
-00003760: 7373 2e30 3533 3132 7d2c 2079 6561 7220  ss.05312}, year 
-00003770: 3d20 7b32 3032 337d 2c20 7075 626c 6973  = {2023}, publis
-00003780: 6865 7220 3d20 7b54 6865 204f 7065 6e20  her = {The Open 
-00003790: 4a6f 7572 6e61 6c7d 2c20 766f 6c75 6d65  Journal}, volume
-000037a0: 203d 207b 387d 2c20 6e75 6d62 6572 203d   = {8}, number =
-000037b0: 207b 3835 7d2c 2070 6167 6573 203d 207b   {85}, pages = {
-000037c0: 3533 3132 7d2c 2061 7574 686f 7220 3d20  5312}, author = 
-000037d0: 7b4d 696b 6520 5761 6c6d 736c 6579 2061  {Mike Walmsley a
-000037e0: 6e64 2043 616d 7062 656c 6c20 416c 6c65  nd Campbell Alle
-000037f0: 6e20 616e 6420 4265 6e20 4175 7373 656c  n and Ben Aussel
-00003800: 2061 6e64 204d 6963 6168 2042 6f77 6c65   and Micah Bowle
-00003810: 7320 616e 6420 4b61 7369 6120 4772 6567  s and Kasia Greg
-00003820: 6f72 6f77 6963 7a20 616e 6420 496e 6967  orowicz and Inig
-00003830: 6f20 5661 6c20 536c 696a 6570 6365 7669  o Val Slijepcevi
-00003840: 6320 616e 6420 4368 7269 7320 4a2e 204c  c and Chris J. L
-00003850: 696e 746f 7474 2061 6e64 2041 6e6e 6120  intott and Anna 
-00003860: 4d2e 206d 2e20 5363 6169 6665 2061 6e64  M. m. Scaife and
-00003870: 204d 616a 6120 4a61 62c5 826f c584 736b   Maja Jab..o..sk
-00003880: 6120 616e 6420 4b6f 7369 6f20 4b61 7263  a and Kosio Karc
-00003890: 6865 7620 616e 6420 4465 6e69 7365 204c  hev and Denise L
-000038a0: 616e 7a69 6572 6920 616e 6420 4465 7669  anzieri and Devi
-000038b0: 6e61 204d 6f68 616e 2061 6e64 2044 6176  na Mohan and Dav
-000038c0: 6964 204f e280 9952 7961 6e20 616e 6420  id O...Ryan and 
-000038d0: 4268 6172 6174 6820 5361 6967 7568 616e  Bharath Saiguhan
-000038e0: 2061 6e64 2043 7269 7365 6c20 5375 c3a1   and Crisel Su..
-000038f0: 7265 7a20 616e 6420 4e69 636f 6cc3 a173  rez and Nicol..s
-00003900: 2047 7565 7272 612d 5661 7261 7320 616e   Guerra-Varas an
-00003910: 6420 5265 6e75 6b61 2056 656c 757d 2c20  d Renuka Velu}, 
-00003920: 7469 746c 6520 3d20 7b5a 6f6f 626f 743a  title = {Zoobot:
-00003930: 2041 6461 7074 6162 6c65 2044 6565 7020   Adaptable Deep 
-00003940: 4c65 6172 6e69 6e67 204d 6f64 656c 7320  Learning Models 
-00003950: 666f 7220 4761 6c61 7879 204d 6f72 7068  for Galaxy Morph
-00003960: 6f6c 6f67 797d 2c20 6a6f 7572 6e61 6c20  ology}, journal 
-00003970: 3d20 7b4a 6f75 726e 616c 206f 6620 4f70  = {Journal of Op
-00003980: 656e 2053 6f75 7263 6520 536f 6674 7761  en Source Softwa
-00003990: 7265 7d20 7d20 0a0a 596f 7520 6d69 6768  re} } ..You migh
-000039a0: 7420 6265 2069 6e74 6572 6573 7465 6420  t be interested 
-000039b0: 696e 2072 6561 6469 6e67 2070 6170 6572  in reading paper
-000039c0: 7320 7573 696e 6720 5a6f 6f62 6f74 3a0a  s using Zoobot:.
-000039d0: 0a2d 205b 4761 6c61 7879 205a 6f6f 2044  .- [Galaxy Zoo D
-000039e0: 4543 614c 533a 2044 6574 6169 6c65 6420  ECaLS: Detailed 
-000039f0: 7669 7375 616c 206d 6f72 7068 6f6c 6f67  visual morpholog
-00003a00: 7920 6d65 6173 7572 656d 656e 7473 2066  y measurements f
-00003a10: 726f 6d20 766f 6c75 6e74 6565 7273 2061  rom volunteers a
-00003a20: 6e64 2064 6565 7020 6c65 6172 6e69 6e67  nd deep learning
-00003a30: 2066 6f72 2033 3134 2c30 3030 2067 616c   for 314,000 gal
-00003a40: 6178 6965 735d 2868 7474 7073 3a2f 2f61  axies](https://a
-00003a50: 7278 6976 2e6f 7267 2f61 6273 2f32 3130  rxiv.org/abs/210
-00003a60: 322e 3038 3431 3429 2028 3230 3232 290a  2.08414) (2022).
-00003a70: 2d20 5b41 2043 6f6d 7061 7269 736f 6e20  - [A Comparison 
-00003a80: 6f66 2044 6565 7020 4c65 6172 6e69 6e67  of Deep Learning
-00003a90: 2041 7263 6869 7465 6374 7572 6573 2066   Architectures f
-00003aa0: 6f72 204f 7074 6963 616c 2047 616c 6178  or Optical Galax
-00003ab0: 7920 4d6f 7270 686f 6c6f 6779 2043 6c61  y Morphology Cla
-00003ac0: 7373 6966 6963 6174 696f 6e5d 2868 7474  ssification](htt
-00003ad0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00003ae0: 6273 2f32 3131 312e 3034 3335 3329 2028  bs/2111.04353) (
-00003af0: 3230 3232 290a 2d20 5b50 7261 6374 6963  2022).- [Practic
-00003b00: 616c 2047 616c 6178 7920 4d6f 7270 686f  al Galaxy Morpho
-00003b10: 6c6f 6779 2054 6f6f 6c73 2066 726f 6d20  logy Tools from 
-00003b20: 4465 6570 2053 7570 6572 7669 7365 6420  Deep Supervised 
-00003b30: 5265 7072 6573 656e 7461 7469 6f6e 204c  Representation L
-00003b40: 6561 726e 696e 675d 2868 7474 7073 3a2f  earning](https:/
-00003b50: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00003b60: 3131 302e 3132 3733 3529 2028 3230 3232  110.12735) (2022
-00003b70: 290a 2d20 5b54 6f77 6172 6473 2046 6f75  ).- [Towards Fou
-00003b80: 6e64 6174 696f 6e20 4d6f 6465 6c73 2066  ndation Models f
-00003b90: 6f72 2047 616c 6178 7920 4d6f 7270 686f  or Galaxy Morpho
-00003ba0: 6c6f 6779 5d28 6874 7470 733a 2f2f 6172  logy](https://ar
-00003bb0: 7869 762e 6f72 672f 6162 732f 3232 3036  xiv.org/abs/2206
-00003bc0: 2e31 3139 3237 2920 2832 3032 3229 0a2d  .11927) (2022).-
-00003bd0: 205b 4861 726e 6573 7369 6e67 2074 6865   [Harnessing the
-00003be0: 2048 7562 626c 6520 5370 6163 6520 5465   Hubble Space Te
-00003bf0: 6c65 7363 6f70 6520 4172 6368 6976 6573  lescope Archives
-00003c00: 3a20 4120 4361 7461 6c6f 6775 6520 6f66  : A Catalogue of
-00003c10: 2032 312c 3932 3620 496e 7465 7261 6374   21,926 Interact
-00003c20: 696e 6720 4761 6c61 7869 6573 5d28 6874  ing Galaxies](ht
-00003c30: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-00003c40: 6162 732f 3233 3033 2e30 3033 3636 2920  abs/2303.00366) 
-00003c50: 2832 3032 3329 0a2d 205b 4173 7472 6f6e  (2023).- [Astron
-00003c60: 6f6d 616c 7920 6174 2053 6361 6c65 3a20  omaly at Scale: 
-00003c70: 5365 6172 6368 696e 6720 666f 7220 416e  Searching for An
-00003c80: 6f6d 616c 6965 7320 416d 6f6e 6773 7420  omalies Amongst 
-00003c90: 3420 4d69 6c6c 696f 6e20 4761 6c61 7869  4 Million Galaxi
-00003ca0: 6573 5d28 6874 7470 733a 2f2f 6172 7869  es](https://arxi
-00003cb0: 762e 6f72 672f 6162 732f 3233 3039 2e30  v.org/abs/2309.0
-00003cc0: 3836 3630 2920 2832 3032 3329 0a2d 205b  8660) (2023).- [
-00003cd0: 4761 6c61 7879 205a 6f6f 2044 4553 493a  Galaxy Zoo DESI:
-00003ce0: 2044 6574 6169 6c65 6420 6d6f 7270 686f   Detailed morpho
-00003cf0: 6c6f 6779 206d 6561 7375 7265 6d65 6e74  logy measurement
-00003d00: 7320 666f 7220 382e 374d 2067 616c 6178  s for 8.7M galax
-00003d10: 6965 7320 696e 2074 6865 2044 4553 4920  ies in the DESI 
-00003d20: 4c65 6761 6379 2049 6d61 6769 6e67 2053  Legacy Imaging S
-00003d30: 7572 7665 7973 5d28 6874 7470 733a 2f2f  urveys](https://
-00003d40: 6163 6164 656d 6963 2e6f 7570 2e63 6f6d  academic.oup.com
-00003d50: 2f6d 6e72 6173 2f61 6476 616e 6365 2d61  /mnras/advance-a
-00003d60: 7274 6963 6c65 2f64 6f69 2f31 302e 3130  rticle/doi/10.10
-00003d70: 3933 2f6d 6e72 6173 2f73 7461 6432 3931  93/mnras/stad291
-00003d80: 392f 3732 3833 3136 393f 6c6f 6769 6e3d  9/7283169?login=
-00003d90: 6661 6c73 6529 2028 3230 3233 290a 2d20  false) (2023).- 
-00003da0: 5b47 616c 6178 7920 6d65 7267 6572 7320  [Galaxy mergers 
-00003db0: 696e 2053 7562 6172 7520 4853 432d 5353  in Subaru HSC-SS
-00003dc0: 503a 2041 2064 6565 7020 7265 7072 6573  P: A deep repres
-00003dd0: 656e 7461 7469 6f6e 206c 6561 726e 696e  entation learnin
-00003de0: 6720 6170 7072 6f61 6368 2066 6f72 2069  g approach for i
-00003df0: 6465 6e74 6966 6963 6174 696f 6e2c 2061  dentification, a
-00003e00: 6e64 2074 6865 2072 6f6c 6520 6f66 2065  nd the role of e
-00003e10: 6e76 6972 6f6e 6d65 6e74 206f 6e20 6d65  nvironment on me
-00003e20: 7267 6572 2069 6e63 6964 656e 6365 5d28  rger incidence](
-00003e30: 6874 7470 733a 2f2f 646f 692e 6f72 672f  https://doi.org/
-00003e40: 3130 2e31 3035 312f 3030 3034 2d36 3336  10.1051/0004-636
-00003e50: 312f 3230 3233 3436 3734 3329 2028 3230  1/202346743) (20
-00003e60: 3233 290a 0a3c 212d 2d20 7375 626d 6974  23)..<!-- submit
-00003e70: 7465 6420 7061 7065 7273 3a20 7369 6d75  ted papers: simu
-00003e80: 6c61 7465 6420 6d65 7267 6572 2063 6c61  lated merger cla
-00003e90: 7373 6966 6963 6174 696f 6e2c 2075 6e73  ssification, uns
-00003ea0: 7570 6572 7669 7365 6420 616e 6f6d 616c  upervised anomal
-00003eb0: 7920 6465 7465 6374 696f 6e2c 2073 7461  y detection, sta
-00003ec0: 7266 6f72 6d69 6e67 2063 6c75 6d70 206c  rforming clump l
-00003ed0: 6f63 616c 6973 6174 696f 6e2c 2061 6e64  ocalisation, and
-00003ee0: 206d 6f72 7068 6f6c 6f67 6963 616c 2073   morphological s
-00003ef0: 6567 6d65 6e74 6174 696f 6e2e 202d 2d3e  egmentation. -->
-00003f00: 0a0a 4d61 6e79 206f 7468 6572 2077 6f72  ..Many other wor
-00003f10: 6b73 2075 7365 205a 6f6f 626f 7420 696e  ks use Zoobot in
-00003f20: 6469 7265 6374 6c79 2076 6961 2074 6865  directly via the
-00003f30: 205b 4761 6c61 7879 205a 6f6f 2044 4543   [Galaxy Zoo DEC
-00003f40: 614c 535d 2868 7474 7073 3a2f 2f61 7278  aLS](https://arx
-00003f50: 6976 2e6f 7267 2f61 6273 2f32 3130 322e  iv.org/abs/2102.
-00003f60: 3038 3431 3429 2063 6174 616c 6f67 2028  08414) catalog (
-00003f70: 616e 6420 6e6f 7720 7669 6120 7468 6520  and now via the 
-00003f80: 6e65 7720 5b47 616c 6178 7920 5a6f 6f20  new [Galaxy Zoo 
-00003f90: 4445 5349 5d28 6874 7470 733a 2f2f 6163  DESI](https://ac
-00003fa0: 6164 656d 6963 2e6f 7570 2e63 6f6d 2f6d  ademic.oup.com/m
-00003fb0: 6e72 6173 2f61 6476 616e 6365 2d61 7274  nras/advance-art
-00003fc0: 6963 6c65 2f64 6f69 2f31 302e 3130 3933  icle/doi/10.1093
-00003fd0: 2f6d 6e72 6173 2f73 7461 6432 3931 392f  /mnras/stad2919/
-00003fe0: 3732 3833 3136 393f 6c6f 6769 6e3d 6661  7283169?login=fa
-00003ff0: 6c73 6529 2063 6174 616c 6f67 292e 0a    lse) catalog)..
+00000320: 7374 3a20 7765 6264 6174 6173 6574 0a52  st: webdataset.R
+00000330: 6571 7569 7265 732d 4469 7374 3a20 6875  equires-Dist: hu
+00000340: 6767 696e 6766 6163 655f 6875 620a 5265  ggingface_hub.Re
+00000350: 7175 6972 6573 2d44 6973 743a 2073 6574  quires-Dist: set
+00000360: 7570 746f 6f6c 730a 5265 7175 6972 6573  uptools.Requires
+00000370: 2d44 6973 743a 2067 616c 6178 792d 6461  -Dist: galaxy-da
+00000380: 7461 7365 7473 3e3d 302e 302e 3137 0a50  tasets>=0.0.17.P
+00000390: 726f 7669 6465 732d 4578 7472 613a 2070  rovides-Extra: p
+000003a0: 7974 6f72 6368 2d63 7075 0a52 6571 7569  ytorch-cpu.Requi
+000003b0: 7265 732d 4469 7374 3a20 746f 7263 683d  res-Dist: torch=
+000003c0: 3d32 2e31 2e30 2b63 7075 3b20 6578 7472  =2.1.0+cpu; extr
+000003d0: 6120 3d3d 2022 7079 746f 7263 682d 6370  a == "pytorch-cp
+000003e0: 7522 0a52 6571 7569 7265 732d 4469 7374  u".Requires-Dist
+000003f0: 3a20 746f 7263 6876 6973 696f 6e3d 3d30  : torchvision==0
+00000400: 2e31 362e 302b 6370 753b 2065 7874 7261  .16.0+cpu; extra
+00000410: 203d 3d20 2270 7974 6f72 6368 2d63 7075   == "pytorch-cpu
+00000420: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000430: 2074 6f72 6368 6175 6469 6f3e 3d32 2e31   torchaudio>=2.1
+00000440: 2e30 3b20 6578 7472 6120 3d3d 2022 7079  .0; extra == "py
+00000450: 746f 7263 682d 6370 7522 0a52 6571 7569  torch-cpu".Requi
+00000460: 7265 732d 4469 7374 3a20 6c69 6768 746e  res-Dist: lightn
+00000470: 696e 673e 3d32 2e30 2e30 3b20 6578 7472  ing>=2.0.0; extr
+00000480: 6120 3d3d 2022 7079 746f 7263 682d 6370  a == "pytorch-cp
+00000490: 7522 0a52 6571 7569 7265 732d 4469 7374  u".Requires-Dist
+000004a0: 3a20 616c 6275 6d65 6e74 6174 696f 6e73  : albumentations
+000004b0: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
+000004c0: 7263 682d 6370 7522 0a52 6571 7569 7265  rch-cpu".Require
+000004d0: 732d 4469 7374 3a20 7079 726f 2d70 706c  s-Dist: pyro-ppl
+000004e0: 3e3d 312e 382e 363b 2065 7874 7261 203d  >=1.8.6; extra =
+000004f0: 3d20 2270 7974 6f72 6368 2d63 7075 220a  = "pytorch-cpu".
+00000500: 5265 7175 6972 6573 2d44 6973 743a 2074  Requires-Dist: t
+00000510: 6f72 6368 6d65 7472 6963 733d 3d30 2e31  orchmetrics==0.1
+00000520: 312e 303b 2065 7874 7261 203d 3d20 2270  1.0; extra == "p
+00000530: 7974 6f72 6368 2d63 7075 220a 5265 7175  ytorch-cpu".Requ
+00000540: 6972 6573 2d44 6973 743a 2074 696d 6d3d  ires-Dist: timm=
+00000550: 3d30 2e39 2e31 303b 2065 7874 7261 203d  =0.9.10; extra =
+00000560: 3d20 2270 7974 6f72 6368 2d63 7075 220a  = "pytorch-cpu".
+00000570: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000580: 7079 746f 7263 682d 6d31 0a52 6571 7569  pytorch-m1.Requi
+00000590: 7265 732d 4469 7374 3a20 746f 7263 683d  res-Dist: torch=
+000005a0: 3d32 2e31 2e30 3b20 6578 7472 6120 3d3d  =2.1.0; extra ==
+000005b0: 2022 7079 746f 7263 682d 6d31 220a 5265   "pytorch-m1".Re
+000005c0: 7175 6972 6573 2d44 6973 743a 2074 6f72  quires-Dist: tor
+000005d0: 6368 7669 7369 6f6e 3d3d 302e 3136 2e30  chvision==0.16.0
+000005e0: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
+000005f0: 7263 682d 6d31 220a 5265 7175 6972 6573  rch-m1".Requires
+00000600: 2d44 6973 743a 2074 6f72 6368 6175 6469  -Dist: torchaudi
+00000610: 6f3e 3d32 2e31 2e30 3b20 6578 7472 6120  o>=2.1.0; extra 
+00000620: 3d3d 2022 7079 746f 7263 682d 6d31 220a  == "pytorch-m1".
+00000630: 5265 7175 6972 6573 2d44 6973 743a 206c  Requires-Dist: l
+00000640: 6967 6874 6e69 6e67 3e3d 322e 302e 303b  ightning>=2.0.0;
+00000650: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
+00000660: 6368 2d6d 3122 0a52 6571 7569 7265 732d  ch-m1".Requires-
+00000670: 4469 7374 3a20 616c 6275 6d65 6e74 6174  Dist: albumentat
+00000680: 696f 6e73 3b20 6578 7472 6120 3d3d 2022  ions; extra == "
+00000690: 7079 746f 7263 682d 6d31 220a 5265 7175  pytorch-m1".Requ
+000006a0: 6972 6573 2d44 6973 743a 2070 7972 6f2d  ires-Dist: pyro-
+000006b0: 7070 6c3e 3d31 2e38 2e36 3b20 6578 7472  ppl>=1.8.6; extr
+000006c0: 6120 3d3d 2022 7079 746f 7263 682d 6d31  a == "pytorch-m1
+000006d0: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+000006e0: 2074 6f72 6368 6d65 7472 6963 733d 3d30   torchmetrics==0
+000006f0: 2e31 312e 303b 2065 7874 7261 203d 3d20  .11.0; extra == 
+00000700: 2270 7974 6f72 6368 2d6d 3122 0a52 6571  "pytorch-m1".Req
+00000710: 7569 7265 732d 4469 7374 3a20 7469 6d6d  uires-Dist: timm
+00000720: 3e3d 302e 392e 3130 3b20 6578 7472 6120  >=0.9.10; extra 
+00000730: 3d3d 2022 7079 746f 7263 682d 6d31 220a  == "pytorch-m1".
+00000740: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000750: 7079 746f 7263 682d 6375 3131 380a 5265  pytorch-cu118.Re
+00000760: 7175 6972 6573 2d44 6973 743a 2074 6f72  quires-Dist: tor
+00000770: 6368 3d3d 322e 312e 302b 6375 3131 383b  ch==2.1.0+cu118;
+00000780: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
+00000790: 6368 2d63 7531 3138 220a 5265 7175 6972  ch-cu118".Requir
+000007a0: 6573 2d44 6973 743a 2074 6f72 6368 7669  es-Dist: torchvi
+000007b0: 7369 6f6e 3d3d 302e 3136 2e30 2b63 7531  sion==0.16.0+cu1
+000007c0: 3138 3b20 6578 7472 6120 3d3d 2022 7079  18; extra == "py
+000007d0: 746f 7263 682d 6375 3131 3822 0a52 6571  torch-cu118".Req
+000007e0: 7569 7265 732d 4469 7374 3a20 746f 7263  uires-Dist: torc
+000007f0: 6861 7564 696f 3e3d 322e 312e 303b 2065  haudio>=2.1.0; e
+00000800: 7874 7261 203d 3d20 2270 7974 6f72 6368  xtra == "pytorch
+00000810: 2d63 7531 3138 220a 5265 7175 6972 6573  -cu118".Requires
+00000820: 2d44 6973 743a 206c 6967 6874 6e69 6e67  -Dist: lightning
+00000830: 3e3d 322e 302e 303b 2065 7874 7261 203d  >=2.0.0; extra =
+00000840: 3d20 2270 7974 6f72 6368 2d63 7531 3138  = "pytorch-cu118
+00000850: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
+00000860: 2061 6c62 756d 656e 7461 7469 6f6e 733b   albumentations;
+00000870: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
+00000880: 6368 2d63 7531 3138 220a 5265 7175 6972  ch-cu118".Requir
+00000890: 6573 2d44 6973 743a 2070 7972 6f2d 7070  es-Dist: pyro-pp
+000008a0: 6c3e 3d31 2e38 2e36 3b20 6578 7472 6120  l>=1.8.6; extra 
+000008b0: 3d3d 2022 7079 746f 7263 682d 6375 3131  == "pytorch-cu11
+000008c0: 3822 0a52 6571 7569 7265 732d 4469 7374  8".Requires-Dist
+000008d0: 3a20 746f 7263 686d 6574 7269 6373 3d3d  : torchmetrics==
+000008e0: 302e 3131 2e30 3b20 6578 7472 6120 3d3d  0.11.0; extra ==
+000008f0: 2022 7079 746f 7263 682d 6375 3131 3822   "pytorch-cu118"
+00000900: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000910: 7469 6d6d 3e3d 302e 392e 3130 3b20 6578  timm>=0.9.10; ex
+00000920: 7472 6120 3d3d 2022 7079 746f 7263 682d  tra == "pytorch-
+00000930: 6375 3131 3822 0a50 726f 7669 6465 732d  cu118".Provides-
+00000940: 4578 7472 613a 2070 7974 6f72 6368 2d63  Extra: pytorch-c
+00000950: 7531 3231 0a52 6571 7569 7265 732d 4469  u121.Requires-Di
+00000960: 7374 3a20 746f 7263 683d 3d32 2e31 2e30  st: torch==2.1.0
+00000970: 2b63 7531 3231 3b20 6578 7472 6120 3d3d  +cu121; extra ==
+00000980: 2022 7079 746f 7263 682d 6375 3132 3122   "pytorch-cu121"
+00000990: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000009a0: 746f 7263 6876 6973 696f 6e3d 3d30 2e31  torchvision==0.1
+000009b0: 362e 302b 6375 3132 313b 2065 7874 7261  6.0+cu121; extra
+000009c0: 203d 3d20 2270 7974 6f72 6368 2d63 7531   == "pytorch-cu1
+000009d0: 3231 220a 5265 7175 6972 6573 2d44 6973  21".Requires-Dis
+000009e0: 743a 2074 6f72 6368 6175 6469 6f3e 3d32  t: torchaudio>=2
+000009f0: 2e31 2e30 3b20 6578 7472 6120 3d3d 2022  .1.0; extra == "
+00000a00: 7079 746f 7263 682d 6375 3132 3122 0a52  pytorch-cu121".R
+00000a10: 6571 7569 7265 732d 4469 7374 3a20 6c69  equires-Dist: li
+00000a20: 6768 746e 696e 673e 3d32 2e30 2e30 3b20  ghtning>=2.0.0; 
+00000a30: 6578 7472 6120 3d3d 2022 7079 746f 7263  extra == "pytorc
+00000a40: 682d 6375 3132 3122 0a52 6571 7569 7265  h-cu121".Require
+00000a50: 732d 4469 7374 3a20 616c 6275 6d65 6e74  s-Dist: albument
+00000a60: 6174 696f 6e73 3b20 6578 7472 6120 3d3d  ations; extra ==
+00000a70: 2022 7079 746f 7263 682d 6375 3132 3122   "pytorch-cu121"
+00000a80: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000a90: 7079 726f 2d70 706c 3e3d 312e 382e 363b  pyro-ppl>=1.8.6;
+00000aa0: 2065 7874 7261 203d 3d20 2270 7974 6f72   extra == "pytor
+00000ab0: 6368 2d63 7531 3231 220a 5265 7175 6972  ch-cu121".Requir
+00000ac0: 6573 2d44 6973 743a 2074 6f72 6368 6d65  es-Dist: torchme
+00000ad0: 7472 6963 733d 3d30 2e31 312e 303b 2065  trics==0.11.0; e
+00000ae0: 7874 7261 203d 3d20 2270 7974 6f72 6368  xtra == "pytorch
+00000af0: 2d63 7531 3231 220a 5265 7175 6972 6573  -cu121".Requires
+00000b00: 2d44 6973 743a 2074 696d 6d3e 3d30 2e39  -Dist: timm>=0.9
+00000b10: 2e31 303b 2065 7874 7261 203d 3d20 2270  .10; extra == "p
+00000b20: 7974 6f72 6368 2d63 7531 3231 220a 5072  ytorch-cu121".Pr
+00000b30: 6f76 6964 6573 2d45 7874 7261 3a20 7079  ovides-Extra: py
+00000b40: 746f 7263 682d 636f 6c61 620a 5265 7175  torch-colab.Requ
+00000b50: 6972 6573 2d44 6973 743a 206c 6967 6874  ires-Dist: light
+00000b60: 6e69 6e67 3e3d 322e 302e 303b 2065 7874  ning>=2.0.0; ext
+00000b70: 7261 203d 3d20 2270 7974 6f72 6368 2d63  ra == "pytorch-c
+00000b80: 6f6c 6162 220a 5265 7175 6972 6573 2d44  olab".Requires-D
+00000b90: 6973 743a 2061 6c62 756d 656e 7461 7469  ist: albumentati
+00000ba0: 6f6e 733b 2065 7874 7261 203d 3d20 2270  ons; extra == "p
+00000bb0: 7974 6f72 6368 2d63 6f6c 6162 220a 5265  ytorch-colab".Re
+00000bc0: 7175 6972 6573 2d44 6973 743a 2070 7972  quires-Dist: pyr
+00000bd0: 6f2d 7070 6c3e 3d31 2e38 2e30 3b20 6578  o-ppl>=1.8.0; ex
+00000be0: 7472 6120 3d3d 2022 7079 746f 7263 682d  tra == "pytorch-
+00000bf0: 636f 6c61 6222 0a52 6571 7569 7265 732d  colab".Requires-
+00000c00: 4469 7374 3a20 746f 7263 686d 6574 7269  Dist: torchmetri
+00000c10: 6373 3d3d 302e 3131 2e30 3b20 6578 7472  cs==0.11.0; extr
+00000c20: 6120 3d3d 2022 7079 746f 7263 682d 636f  a == "pytorch-co
+00000c30: 6c61 6222 0a52 6571 7569 7265 732d 4469  lab".Requires-Di
+00000c40: 7374 3a20 7469 6d6d 3e3d 302e 392e 3130  st: timm>=0.9.10
+00000c50: 3b20 6578 7472 6120 3d3d 2022 7079 746f  ; extra == "pyto
+00000c60: 7263 682d 636f 6c61 6222 0a52 6571 7569  rch-colab".Requi
+00000c70: 7265 732d 4469 7374 3a20 6761 6c61 7879  res-Dist: galaxy
+00000c80: 5f64 6174 6173 6574 733d 3d30 2e30 2e31  _datasets==0.0.1
+00000c90: 373b 2065 7874 7261 203d 3d20 2270 7974  7; extra == "pyt
+00000ca0: 6f72 6368 2d63 6f6c 6162 220a 5072 6f76  orch-colab".Prov
+00000cb0: 6964 6573 2d45 7874 7261 3a20 7465 6e73  ides-Extra: tens
+00000cc0: 6f72 666c 6f77 0a52 6571 7569 7265 732d  orflow.Requires-
+00000cd0: 4469 7374 3a20 7465 6e73 6f72 666c 6f77  Dist: tensorflow
+00000ce0: 3d3d 322e 3130 2e30 3b20 6578 7472 6120  ==2.10.0; extra 
+00000cf0: 3d3d 2022 7465 6e73 6f72 666c 6f77 220a  == "tensorflow".
+00000d00: 5265 7175 6972 6573 2d44 6973 743a 206b  Requires-Dist: k
+00000d10: 6572 6173 5f61 7070 6c69 6361 7469 6f6e  eras_application
+00000d20: 733b 2065 7874 7261 203d 3d20 2274 656e  s; extra == "ten
+00000d30: 736f 7266 6c6f 7722 0a52 6571 7569 7265  sorflow".Require
+00000d40: 732d 4469 7374 3a20 7465 6e73 6f72 666c  s-Dist: tensorfl
+00000d50: 6f77 5f70 726f 6261 6269 6c69 7479 3d3d  ow_probability==
+00000d60: 302e 3138 2e30 3b20 6578 7472 6120 3d3d  0.18.0; extra ==
+00000d70: 2022 7465 6e73 6f72 666c 6f77 220a 5265   "tensorflow".Re
+00000d80: 7175 6972 6573 2d44 6973 743a 2070 726f  quires-Dist: pro
+00000d90: 746f 6275 663c 3d33 2e31 393b 2065 7874  tobuf<=3.19; ext
+00000da0: 7261 203d 3d20 2274 656e 736f 7266 6c6f  ra == "tensorflo
+00000db0: 7722 0a50 726f 7669 6465 732d 4578 7472  w".Provides-Extr
+00000dc0: 613a 2075 7469 6c69 7469 6573 0a52 6571  a: utilities.Req
+00000dd0: 7569 7265 732d 4469 7374 3a20 7365 6162  uires-Dist: seab
+00000de0: 6f72 6e3b 2065 7874 7261 203d 3d20 2275  orn; extra == "u
+00000df0: 7469 6c69 7469 6573 220a 5265 7175 6972  tilities".Requir
+00000e00: 6573 2d44 6973 743a 2062 6f74 6f33 3b20  es-Dist: boto3; 
+00000e10: 6578 7472 6120 3d3d 2022 7574 696c 6974  extra == "utilit
+00000e20: 6965 7322 0a52 6571 7569 7265 732d 4469  ies".Requires-Di
+00000e30: 7374 3a20 7079 7468 6f6e 2d64 6174 6575  st: python-dateu
+00000e40: 7469 6c3d 3d32 2e38 2e31 3b20 6578 7472  til==2.8.1; extr
+00000e50: 6120 3d3d 2022 7574 696c 6974 6965 7322  a == "utilities"
+00000e60: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000e70: 2064 6f63 730a 5265 7175 6972 6573 2d44   docs.Requires-D
+00000e80: 6973 743a 2053 7068 696e 783b 2065 7874  ist: Sphinx; ext
+00000e90: 7261 203d 3d20 2264 6f63 7322 0a52 6571  ra == "docs".Req
+00000ea0: 7569 7265 732d 4469 7374 3a20 7370 6869  uires-Dist: sphi
+00000eb0: 6e78 636f 6e74 7269 622d 6e61 706f 6c65  nxcontrib-napole
+00000ec0: 6f6e 3b20 6578 7472 6120 3d3d 2022 646f  on; extra == "do
+00000ed0: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
+00000ee0: 743a 2066 7572 6f3b 2065 7874 7261 203d  t: furo; extra =
+00000ef0: 3d20 2264 6f63 7322 0a52 6571 7569 7265  = "docs".Require
+00000f00: 732d 4469 7374 3a20 646f 6375 7469 6c73  s-Dist: docutils
+00000f10: 3c30 2e31 383b 2065 7874 7261 203d 3d20  <0.18; extra == 
+00000f20: 2264 6f63 7322 0a52 6571 7569 7265 732d  "docs".Requires-
+00000f30: 4469 7374 3a20 7370 6869 6e78 656d 6f6a  Dist: sphinxemoj
+00000f40: 693b 2065 7874 7261 203d 3d20 2264 6f63  i; extra == "doc
+00000f50: 7322 0a0a 2320 5a6f 6f62 6f74 0a0a 5b21  s"..# Zoobot..[!
+00000f60: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
+00000f70: 733a 2f2f 7065 7079 2e74 6563 682f 6261  s://pepy.tech/ba
+00000f80: 6467 652f 7a6f 6f62 6f74 295d 2868 7474  dge/zoobot)](htt
+00000f90: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00000fa0: 726f 6a65 6374 2f7a 6f6f 626f 7429 0a5b  roject/zoobot).[
+00000fb0: 215b 446f 6375 6d65 6e74 6174 696f 6e20  ![Documentation 
+00000fc0: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
+00000fd0: 7265 6164 7468 6564 6f63 732e 6f72 672f  readthedocs.org/
+00000fe0: 7072 6f6a 6563 7473 2f7a 6f6f 626f 742f  projects/zoobot/
+00000ff0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+00001000: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
+00001010: 7a6f 6f62 6f74 2e72 6561 6474 6865 646f  zoobot.readthedo
+00001020: 6373 2e69 6f2f 290a 215b 6275 696c 645d  cs.io/).![build]
+00001030: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001040: 636f 6d2f 6d77 616c 6d73 6c65 792f 7a6f  com/mwalmsley/zo
+00001050: 6f62 6f74 2f61 6374 696f 6e73 2f77 6f72  obot/actions/wor
+00001060: 6b66 6c6f 7773 2f72 756e 5f43 492e 796d  kflows/run_CI.ym
+00001070: 6c2f 6261 6467 652e 7376 6729 0a21 5b70  l/badge.svg).![p
+00001080: 7562 6c69 7368 5d28 6874 7470 733a 2f2f  ublish](https://
+00001090: 6769 7468 7562 2e63 6f6d 2f6d 7761 6c6d  github.com/mwalm
+000010a0: 736c 6579 2f7a 6f6f 626f 742f 6163 7469  sley/zoobot/acti
+000010b0: 6f6e 732f 776f 726b 666c 6f77 732f 7079  ons/workflows/py
+000010c0: 7468 6f6e 2d70 7562 6c69 7368 2e79 6d6c  thon-publish.yml
+000010d0: 2f62 6164 6765 2e73 7667 290a 5b21 5b50  /badge.svg).[![P
+000010e0: 7950 495d 2868 7474 7073 3a2f 2f62 6164  yPI](https://bad
+000010f0: 6765 2e66 7572 792e 696f 2f70 792f 7a6f  ge.fury.io/py/zo
+00001100: 6f62 6f74 2e73 7667 295d 2868 7474 7073  obot.svg)](https
+00001110: 3a2f 2f62 6164 6765 2e66 7572 792e 696f  ://badge.fury.io
+00001120: 2f70 792f 7a6f 6f62 6f74 290a 5b21 5b44  /py/zoobot).[![D
+00001130: 4f49 5d28 6874 7470 733a 2f2f 7a65 6e6f  OI](https://zeno
+00001140: 646f 2e6f 7267 2f62 6164 6765 2f33 3433  do.org/badge/343
+00001150: 3738 3736 3137 2e73 7667 295d 2868 7474  787617.svg)](htt
+00001160: 7073 3a2f 2f7a 656e 6f64 6f2e 6f72 672f  ps://zenodo.org/
+00001170: 6261 6467 652f 6c61 7465 7374 646f 692f  badge/latestdoi/
+00001180: 3334 3337 3837 3631 3729 0a5b 215b 7374  343787617).[![st
+00001190: 6174 7573 5d28 6874 7470 733a 2f2f 6a6f  atus](https://jo
+000011a0: 7373 2e74 6865 6f6a 2e6f 7267 2f70 6170  ss.theoj.org/pap
+000011b0: 6572 732f 3434 3735 3631 6565 3264 6534  ers/447561ee2de4
+000011c0: 3730 3965 6464 6237 3034 6531 3862 6565  709eddb704e18bee
+000011d0: 3834 3666 2f73 7461 7475 732e 7376 6729  846f/status.svg)
+000011e0: 5d28 6874 7470 733a 2f2f 6a6f 7373 2e74  ](https://joss.t
+000011f0: 6865 6f6a 2e6f 7267 2f70 6170 6572 732f  heoj.org/papers/
+00001200: 3434 3735 3631 6565 3264 6534 3730 3965  447561ee2de4709e
+00001210: 6464 6237 3034 6531 3862 6565 3834 3666  ddb704e18bee846f
+00001220: 290a 3c61 2068 7265 663d 2268 7474 7073  ).<a href="https
+00001230: 3a2f 2f61 7363 6c2e 6e65 742f 3232 3033  ://ascl.net/2203
+00001240: 2e30 3237 223e 3c69 6d67 2073 7263 3d22  .027"><img src="
+00001250: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00001260: 6c64 732e 696f 2f62 6164 6765 2f61 7363  lds.io/badge/asc
+00001270: 6c2d 3232 3033 2e30 3237 2d62 6c75 652e  l-2203.027-blue.
+00001280: 7376 673f 636f 6c6f 7242 3d32 3632 3235  svg?colorB=26225
+00001290: 3522 2061 6c74 3d22 6173 636c 3a32 3230  5" alt="ascl:220
+000012a0: 332e 3032 3722 202f 3e3c 2f61 3e0a 0a5a  3.027" /></a>..Z
+000012b0: 6f6f 626f 7420 636c 6173 7369 6669 6573  oobot classifies
+000012c0: 2067 616c 6178 7920 6d6f 7270 686f 6c6f   galaxy morpholo
+000012d0: 6779 2077 6974 6820 6465 6570 206c 6561  gy with deep lea
+000012e0: 726e 696e 672e 0a3c 212d 2d20 4174 2047  rning..<!-- At G
+000012f0: 616c 6178 7920 5a6f 6f2c 2077 6520 7573  alaxy Zoo, we us
+00001300: 6520 5a6f 6f62 6f74 2074 6f20 6865 6c70  e Zoobot to help
+00001310: 206f 7572 2076 6f6c 756e 7465 6572 7320   our volunteers 
+00001320: 636c 6173 7369 6679 2074 6865 2067 616c  classify the gal
+00001330: 6178 6965 7320 696e 2061 6c6c 206f 7572  axies in all our
+00001340: 2072 6563 656e 7420 6361 7461 6c6f 6775   recent catalogu
+00001350: 6573 3a20 475a 2044 4543 614c 532c 2047  es: GZ DECaLS, G
+00001360: 5a20 4445 5349 2c20 475a 2052 696e 6773  Z DESI, GZ Rings
+00001370: 2061 6e64 2047 5a20 436f 736d 6963 2044   and GZ Cosmic D
+00001380: 6177 6e2e 202d 2d3e 0a0a 5a6f 6f62 6f74  awn. -->..Zoobot
+00001390: 2069 7320 7472 6169 6e65 6420 7573 696e   is trained usin
+000013a0: 6720 6d69 6c6c 696f 6e73 206f 6620 616e  g millions of an
+000013b0: 7377 6572 7320 6279 2047 616c 6178 7920  swers by Galaxy 
+000013c0: 5a6f 6f20 766f 6c75 6e74 6565 7273 2e20  Zoo volunteers. 
+000013d0: 5468 6973 2063 6f64 6520 7769 6c6c 206c  This code will l
+000013e0: 6574 2079 6f75 202a 2a72 6574 7261 696e  et you **retrain
+000013f0: 2a2a 205a 6f6f 626f 7420 746f 2061 6363  ** Zoobot to acc
+00001400: 7572 6174 656c 7920 736f 6c76 6520 796f  urately solve yo
+00001410: 7572 206f 776e 2070 7265 6469 6374 696f  ur own predictio
+00001420: 6e20 7461 736b 2e0a 0a2d 205b 496e 7374  n task...- [Inst
+00001430: 616c 6c5d 2823 696e 7374 616c 6c61 7469  all](#installati
+00001440: 6f6e 290a 2d20 5b51 7569 636b 7374 6172  on).- [Quickstar
+00001450: 745d 2823 7175 6963 6b73 7461 7274 290a  t](#quickstart).
+00001460: 2d20 5b57 6f72 6b65 6420 4578 616d 706c  - [Worked Exampl
+00001470: 6573 5d28 2377 6f72 6b65 642d 6578 616d  es](#worked-exam
+00001480: 706c 6573 290a 2d20 5b50 7265 7472 6169  ples).- [Pretrai
+00001490: 6e65 6420 5765 6967 6874 735d 2868 7474  ned Weights](htt
+000014a0: 7073 3a2f 2f7a 6f6f 626f 742e 7265 6164  ps://zoobot.read
+000014b0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000014c0: 7465 7374 2f70 7265 7472 6169 6e65 645f  test/pretrained_
+000014d0: 6d6f 6465 6c73 2e68 746d 6c29 0a2d 205b  models.html).- [
+000014e0: 4461 7461 7365 7473 5d28 6874 7470 733a  Datasets](https:
+000014f0: 2f2f 7777 772e 6769 7468 7562 2e63 6f6d  //www.github.com
+00001500: 2f6d 7761 6c6d 736c 6579 2f67 616c 6178  /mwalmsley/galax
+00001510: 792d 6461 7461 7365 7473 290a 2d20 5b44  y-datasets).- [D
+00001520: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00001530: 7470 733a 2f2f 7a6f 6f62 6f74 2e72 6561  tps://zoobot.rea
+00001540: 6474 6865 646f 6373 2e69 6f2f 2920 2866  dthedocs.io/) (f
+00001550: 6f72 2075 6e64 6572 7374 616e 6469 6e67  or understanding
+00001560: 2f72 6566 6572 656e 6365 290a 0a23 2320  /reference)..## 
+00001570: 496e 7374 616c 6c61 7469 6f6e 0a0a 3c61  Installation..<a
+00001580: 206e 616d 653d 2269 6e73 7461 6c6c 6174   name="installat
+00001590: 696f 6e22 3e3c 2f61 3e0a 0a59 6f75 2063  ion"></a>..You c
+000015a0: 616e 2072 6574 7261 696e 205a 6f6f 626f  an retrain Zoobo
+000015b0: 7420 696e 2074 6865 2063 6c6f 7564 2077  t in the cloud w
+000015c0: 6974 6820 6120 6672 6565 2047 5055 2075  ith a free GPU u
+000015d0: 7369 6e67 2074 6869 7320 5b47 6f6f 676c  sing this [Googl
+000015e0: 6520 436f 6c61 6220 6e6f 7465 626f 6f6b  e Colab notebook
+000015f0: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
+00001600: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
+00001610: 636f 6d2f 6472 6976 652f 3141 5f2d 4d33  com/drive/1A_-M3
+00001620: 537a 356d 6151 6d79 6657 3241 3772 4575  Sz5maQmyfW2A7rEu
+00001630: 2d67 5f5a 6930 524d 477a 353f 7573 703d  -g_Zi0RMGz5?usp=
+00001640: 7368 6172 696e 6729 2e20 546f 2069 6e73  sharing). To ins
+00001650: 7461 6c6c 206c 6f63 616c 6c79 2c20 6b65  tall locally, ke
+00001660: 6570 2072 6561 6469 6e67 2e0a 0a44 6f77  ep reading...Dow
+00001670: 6e6c 6f61 6420 7468 6520 636f 6465 2075  nload the code u
+00001680: 7369 6e67 2067 6974 3a0a 0a20 2020 2067  sing git:..    g
+00001690: 6974 2063 6c6f 6e65 2067 6974 4067 6974  it clone git@git
+000016a0: 6875 622e 636f 6d3a 6d77 616c 6d73 6c65  hub.com:mwalmsle
+000016b0: 792f 7a6f 6f62 6f74 2e67 6974 0a0a 416e  y/zoobot.git..An
+000016c0: 6420 7468 656e 2070 6963 6b20 6f6e 6520  d then pick one 
+000016d0: 6f66 2074 6865 2074 6872 6565 2063 6f6d  of the three com
+000016e0: 6d61 6e64 7320 6265 6c6f 7720 746f 2069  mands below to i
+000016f0: 6e73 7461 6c6c 205a 6f6f 626f 7420 616e  nstall Zoobot an
+00001700: 6420 5079 546f 7263 683a 0a0a 2020 2020  d PyTorch:..    
+00001710: 2320 5a6f 6f62 6f74 2077 6974 6820 5079  # Zoobot with Py
+00001720: 546f 7263 6820 616e 6420 6120 4750 552e  Torch and a GPU.
+00001730: 2052 6571 7569 7265 7320 4355 4441 2031   Requires CUDA 1
+00001740: 322e 3120 286f 7220 4355 4441 2031 312e  2.1 (or CUDA 11.
+00001750: 382c 2069 6620 796f 7520 7573 6520 605f  8, if you use `_
+00001760: 6375 3131 3860 2069 6e73 7465 6164 290a  cu118` instead).
+00001770: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
+00001780: 2d65 2022 7a6f 6f62 6f74 5b70 7974 6f72  -e "zoobot[pytor
+00001790: 6368 2d63 7531 3231 5d22 202d 2d65 7874  ch-cu121]" --ext
+000017a0: 7261 2d69 6e64 6578 2d75 726c 2068 7474  ra-index-url htt
+000017b0: 7073 3a2f 2f64 6f77 6e6c 6f61 642e 7079  ps://download.py
+000017c0: 746f 7263 682e 6f72 672f 7768 6c2f 6375  torch.org/whl/cu
+000017d0: 3132 310a 0a20 2020 2023 204f 5220 5a6f  121..    # OR Zo
+000017e0: 6f62 6f74 2077 6974 6820 5079 546f 7263  obot with PyTorc
+000017f0: 6820 616e 6420 6e6f 2047 5055 0a20 2020  h and no GPU.   
+00001800: 2070 6970 2069 6e73 7461 6c6c 202d 6520   pip install -e 
+00001810: 227a 6f6f 626f 745b 7079 746f 7263 682d  "zoobot[pytorch-
+00001820: 6370 755d 2220 2d2d 6578 7472 612d 696e  cpu]" --extra-in
+00001830: 6465 782d 7572 6c20 6874 7470 733a 2f2f  dex-url https://
+00001840: 646f 776e 6c6f 6164 2e70 7974 6f72 6368  download.pytorch
+00001850: 2e6f 7267 2f77 686c 2f63 7075 0a0a 2020  .org/whl/cpu..  
+00001860: 2020 2320 4f52 205a 6f6f 626f 7420 7769    # OR Zoobot wi
+00001870: 7468 2050 7954 6f72 6368 206f 6e20 4d61  th PyTorch on Ma
+00001880: 6320 7769 7468 204d 3120 6368 6970 0a20  c with M1 chip. 
+00001890: 2020 2070 6970 2069 6e73 7461 6c6c 202d     pip install -
+000018a0: 6520 227a 6f6f 626f 745b 7079 746f 7263  e "zoobot[pytorc
+000018b0: 682d 6d31 5d22 0a0a 5468 6973 2069 6e73  h-m1]"..This ins
+000018c0: 7461 6c6c 7320 7468 6520 646f 776e 6c6f  talls the downlo
+000018d0: 6164 6564 205a 6f6f 626f 7420 636f 6465  aded Zoobot code
+000018e0: 2075 7369 6e67 2070 6970 205b 6564 6974   using pip [edit
+000018f0: 6162 6c65 206d 6f64 655d 2868 7474 7073  able mode](https
+00001900: 3a2f 2f70 6970 2e70 7970 612e 696f 2f65  ://pip.pypa.io/e
+00001910: 6e2f 7374 6162 6c65 2f74 6f70 6963 732f  n/stable/topics/
+00001920: 6c6f 6361 6c2d 7072 6f6a 6563 742d 696e  local-project-in
+00001930: 7374 616c 6c73 2f23 6564 6974 6162 6c65  stalls/#editable
+00001940: 2d69 6e73 7461 6c6c 7329 2073 6f20 796f  -installs) so yo
+00001950: 7520 6361 6e20 6561 7369 6c79 2063 6861  u can easily cha
+00001960: 6e67 6520 7468 6520 636f 6465 206c 6f63  nge the code loc
+00001970: 616c 6c79 2e20 5a6f 6f62 6f74 2069 7320  ally. Zoobot is 
+00001980: 616c 736f 2061 7661 696c 6162 6c65 2064  also available d
+00001990: 6972 6563 746c 7920 6672 6f6d 2070 6970  irectly from pip
+000019a0: 2028 6070 6970 2069 6e73 7461 6c6c 207a   (`pip install z
+000019b0: 6f6f 626f 745b 6f70 7469 6f6e 5d60 292e  oobot[option]`).
+000019c0: 204f 6e6c 7920 7573 6520 7468 6973 2069   Only use this i
+000019d0: 6620 796f 7520 6172 6520 7375 7265 2079  f you are sure y
+000019e0: 6f75 2077 6f6e 2774 2062 6520 6d61 6b69  ou won't be maki
+000019f0: 6e67 2063 6861 6e67 6573 2074 6f20 5a6f  ng changes to Zo
+00001a00: 6f62 6f74 2069 7473 656c 662e 2046 6f72  obot itself. For
+00001a10: 2047 6f6f 676c 6520 436f 6c61 622c 2075   Google Colab, u
+00001a20: 7365 2060 7069 7020 696e 7374 616c 6c20  se `pip install 
+00001a30: 7a6f 6f62 6f74 5b70 7974 6f72 6368 5f63  zoobot[pytorch_c
+00001a40: 6f6c 6162 5d60 0a0a 546f 2075 7365 2061  olab]`..To use a
+00001a50: 2047 5055 2c20 796f 7520 6d75 7374 202a   GPU, you must *
+00001a60: 616c 7265 6164 792a 2068 6176 6520 4355  already* have CU
+00001a70: 4441 2069 6e73 7461 6c6c 6564 2061 6e64  DA installed and
+00001a80: 206d 6174 6368 696e 6720 7468 6520 7665   matching the ve
+00001a90: 7273 696f 6e73 2061 626f 7665 2e0a 4920  rsions above..I 
+00001aa0: 7368 6172 6520 6d79 2069 6e73 7461 6c6c  share my install
+00001ab0: 2073 7465 7073 205b 6865 7265 5d28 2369   steps [here](#i
+00001ac0: 6e73 7461 6c6c 5f63 7564 6129 2e20 4750  nstall_cuda). GP
+00001ad0: 5573 2061 7265 206f 7074 696f 6e61 6c20  Us are optional 
+00001ae0: 2d20 5a6f 6f62 6f74 2077 696c 6c20 7275  - Zoobot will ru
+00001af0: 6e20 7265 7472 6169 6e20 6669 6e65 206f  n retrain fine o
+00001b00: 6e20 4350 552c 206a 7573 7420 736c 6f77  n CPU, just slow
+00001b10: 6572 2e0a 0a23 2320 5175 6963 6b73 7461  er...## Quicksta
+00001b20: 7274 0a0a 3c61 206e 616d 653d 2271 7569  rt..<a name="qui
+00001b30: 636b 7374 6172 7422 3e3c 2f61 3e0a 0a54  ckstart"></a>..T
+00001b40: 6865 205b 436f 6c61 6220 6e6f 7465 626f  he [Colab notebo
+00001b50: 6f6b 5d28 6874 7470 733a 2f2f 636f 6c61  ok](https://cola
+00001b60: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00001b70: 652e 636f 6d2f 6472 6976 652f 3141 5f2d  e.com/drive/1A_-
+00001b80: 4d33 537a 356d 6151 6d79 6657 3241 3772  M3Sz5maQmyfW2A7r
+00001b90: 4575 2d67 5f5a 6930 524d 477a 353f 7573  Eu-g_Zi0RMGz5?us
+00001ba0: 703d 7368 6172 696e 6729 2069 7320 7468  p=sharing) is th
+00001bb0: 6520 7175 6963 6b65 7374 2077 6179 2074  e quickest way t
+00001bc0: 6f20 6765 7420 7374 6172 7465 642e 2041  o get started. A
+00001bd0: 6c74 6572 6e61 7469 7665 6c79 2c20 7468  lternatively, th
+00001be0: 6520 6d69 6e69 6d61 6c20 6578 616d 706c  e minimal exampl
+00001bf0: 6520 6265 6c6f 7720 696c 6c75 7374 7261  e below illustra
+00001c00: 7465 7320 686f 7720 5a6f 6f62 6f74 2077  tes how Zoobot w
+00001c10: 6f72 6b73 2e0a 0a4c 6574 2773 2073 6179  orks...Let's say
+00001c20: 2079 6f75 2077 616e 7420 746f 2066 696e   you want to fin
+00001c30: 6420 7269 6e67 6564 2067 616c 6178 6965  d ringed galaxie
+00001c40: 7320 616e 6420 796f 7520 6861 7665 2061  s and you have a
+00001c50: 2073 6d61 6c6c 206c 6162 656c 6c65 6420   small labelled 
+00001c60: 6461 7461 7365 7420 6f66 2035 3030 2072  dataset of 500 r
+00001c70: 696e 6765 6420 6f72 206e 6f74 2d72 696e  inged or not-rin
+00001c80: 6765 6420 6761 6c61 7869 6573 2e20 596f  ged galaxies. Yo
+00001c90: 7520 6361 6e20 7265 7472 6169 6e20 5a6f  u can retrain Zo
+00001ca0: 6f62 6f74 2074 6f20 6669 6e64 2072 696e  obot to find rin
+00001cb0: 6773 206c 696b 6520 736f 3a0a 0a20 2020  gs like so:..   
+00001cc0: 2060 6060 7079 7468 6f6e 0a0a 2020 2020   ```python..    
+00001cd0: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
+00001ce0: 2070 640a 2020 2020 6672 6f6d 2067 616c   pd.    from gal
+00001cf0: 6178 795f 6461 7461 7365 7473 2e70 7974  axy_datasets.pyt
+00001d00: 6f72 6368 2e67 616c 6178 795f 6461 7461  orch.galaxy_data
+00001d10: 6d6f 6475 6c65 2069 6d70 6f72 7420 4761  module import Ga
+00001d20: 6c61 7879 4461 7461 4d6f 6475 6c65 0a20  laxyDataModule. 
+00001d30: 2020 2066 726f 6d20 7a6f 6f62 6f74 2e70     from zoobot.p
+00001d40: 7974 6f72 6368 2e74 7261 696e 696e 6720  ytorch.training 
+00001d50: 696d 706f 7274 2066 696e 6574 756e 650a  import finetune.
+00001d60: 0a20 2020 2023 2063 7376 2077 6974 6820  .    # csv with 
+00001d70: 2772 696e 6727 2063 6f6c 756d 6e20 2830  'ring' column (0
+00001d80: 206f 7220 3129 2061 6e64 2027 6669 6c65   or 1) and 'file
+00001d90: 5f6c 6f63 2720 636f 6c75 6d6e 2028 7061  _loc' column (pa
+00001da0: 7468 2074 6f20 696d 6167 6529 0a20 2020  th to image).   
+00001db0: 206c 6162 656c 6c65 645f 6466 203d 2070   labelled_df = p
+00001dc0: 642e 7265 6164 5f63 7376 2827 2f79 6f75  d.read_csv('/you
+00001dd0: 722f 7061 7468 2f73 6f6d 655f 6c61 6265  r/path/some_labe
+00001de0: 6c6c 6564 5f67 616c 6178 6965 732e 6373  lled_galaxies.cs
+00001df0: 7627 290a 0a20 2020 2064 6174 616d 6f64  v')..    datamod
+00001e00: 756c 6520 3d20 4761 6c61 7879 4461 7461  ule = GalaxyData
+00001e10: 4d6f 6475 6c65 280a 2020 2020 2020 6c61  Module(.      la
+00001e20: 6265 6c5f 636f 6c73 3d5b 2772 696e 6727  bel_cols=['ring'
+00001e30: 5d2c 0a20 2020 2020 2063 6174 616c 6f67  ],.      catalog
+00001e40: 3d6c 6162 656c 6c65 645f 6466 2c0a 2020  =labelled_df,.  
+00001e50: 2020 2020 6261 7463 685f 7369 7a65 3d33      batch_size=3
+00001e60: 320a 2020 2020 290a 0a20 2020 2023 206c  2.    )..    # l
+00001e70: 6f61 6420 7472 6169 6e65 6420 5a6f 6f62  oad trained Zoob
+00001e80: 6f74 206d 6f64 656c 0a20 2020 206d 6f64  ot model.    mod
+00001e90: 656c 203d 2066 696e 6574 756e 652e 4669  el = finetune.Fi
+00001ea0: 6e65 7475 6e65 6162 6c65 5a6f 6f62 6f74  netuneableZoobot
+00001eb0: 436c 6173 7369 6669 6572 2863 6865 636b  Classifier(check
+00001ec0: 706f 696e 745f 6c6f 632c 206e 756d 5f63  point_loc, num_c
+00001ed0: 6c61 7373 6573 3d32 2920 200a 2020 2020  lasses=2)  .    
+00001ee0: 0a20 2020 2023 2072 6574 7261 696e 2074  .    # retrain t
+00001ef0: 6f20 6669 6e64 2072 696e 6773 0a20 2020  o find rings.   
+00001f00: 2074 7261 696e 6572 203d 2066 696e 6574   trainer = finet
+00001f10: 756e 652e 6765 745f 7472 6169 6e65 7228  une.get_trainer(
+00001f20: 7361 7665 5f64 6972 290a 2020 2020 7472  save_dir).    tr
+00001f30: 6169 6e65 722e 6669 7428 6d6f 6465 6c2c  ainer.fit(model,
+00001f40: 2064 6174 616d 6f64 756c 6529 0a20 2020   datamodule).   
+00001f50: 2060 6060 0a0a 5468 656e 2079 6f75 2063   ```..Then you c
+00001f60: 616e 206d 616b 6520 7072 6564 6963 7420  an make predict 
+00001f70: 6966 206e 6577 2067 616c 6178 6965 7320  if new galaxies 
+00001f80: 6861 7665 2072 696e 6773 3a0a 0a20 2020  have rings:..   
+00001f90: 2060 6060 7079 7468 6f6e 0a20 2020 2066   ```python.    f
+00001fa0: 726f 6d20 7a6f 6f62 6f74 2e70 7974 6f72  rom zoobot.pytor
+00001fb0: 6368 2e70 7265 6469 6374 696f 6e73 2069  ch.predictions i
+00001fc0: 6d70 6f72 7420 7072 6564 6963 745f 6f6e  mport predict_on
+00001fd0: 5f63 6174 616c 6f67 0a0a 2020 2020 2320  _catalog..    # 
+00001fe0: 6373 7620 7769 7468 2027 6669 6c65 5f6c  csv with 'file_l
+00001ff0: 6f63 2720 636f 6c75 6d6e 2028 7061 7468  oc' column (path
+00002000: 2074 6f20 696d 6167 6529 2e20 5a6f 6f62   to image). Zoob
+00002010: 6f74 2077 696c 6c20 7072 6564 6963 7420  ot will predict 
+00002020: 7468 6520 6c61 6265 6c73 2e0a 2020 2020  the labels..    
+00002030: 756e 6c61 6265 6c6c 6564 5f64 6620 3d20  unlabelled_df = 
+00002040: 7064 2e72 6561 645f 6373 7628 272f 796f  pd.read_csv('/yo
+00002050: 7572 2f70 6174 682f 736f 6d65 5f75 6e6c  ur/path/some_unl
+00002060: 6162 656c 6c65 645f 6761 6c61 7869 6573  abelled_galaxies
+00002070: 2e63 7376 2729 0a0a 2020 2020 7072 6564  .csv')..    pred
+00002080: 6963 745f 6f6e 5f63 6174 616c 6f67 2e70  ict_on_catalog.p
+00002090: 7265 6469 6374 280a 2020 2020 2020 756e  redict(.      un
+000020a0: 6c61 6265 6c6c 6564 5f64 662c 0a20 2020  labelled_df,.   
+000020b0: 2020 206d 6f64 656c 2c0a 2020 2020 2020     model,.      
+000020c0: 6c61 6265 6c5f 636f 6c73 3d5b 2772 696e  label_cols=['rin
+000020d0: 6727 5d2c 2020 2320 6f6e 6c79 2075 7365  g'],  # only use
+000020e0: 6420 666f 7220 0a20 2020 2020 2073 6176  d for .      sav
+000020f0: 655f 6c6f 633d 272f 796f 7572 2f70 6174  e_loc='/your/pat
+00002100: 682f 6669 6e65 7475 6e65 645f 7072 6564  h/finetuned_pred
+00002110: 6963 7469 6f6e 732e 6373 7627 0a20 2020  ictions.csv'.   
+00002120: 2029 0a20 2020 2060 6060 0a0a 5a6f 6f62   ).    ```..Zoob
+00002130: 6f74 2069 6e63 6c75 6465 7320 6d61 6e79  ot includes many
+00002140: 2067 7569 6465 7320 616e 6420 776f 726b   guides and work
+00002150: 696e 6720 6578 616d 706c 6573 202d 2073  ing examples - s
+00002160: 6565 2074 6865 205b 4765 7474 696e 6720  ee the [Getting 
+00002170: 5374 6172 7465 645d 2823 6765 7474 696e  Started](#gettin
+00002180: 672d 7374 6172 7465 6429 2073 6563 7469  g-started) secti
+00002190: 6f6e 2062 656c 6f77 2e0a 0a23 2320 4765  on below...## Ge
+000021a0: 7474 696e 6720 5374 6172 7465 640a 0a3c  tting Started..<
+000021b0: 6120 6e61 6d65 3d22 6765 7474 696e 675f  a name="getting_
+000021c0: 7374 6172 7465 6422 3e3c 2f61 3e0a 0a49  started"></a>..I
+000021d0: 2073 7567 6765 7374 2073 7461 7274 696e   suggest startin
+000021e0: 6720 7769 7468 2074 6865 205b 436f 6c61  g with the [Cola
+000021f0: 6220 6e6f 7465 626f 6f6b 5d28 6874 7470  b notebook](http
+00002200: 733a 2f2f 636f 6c61 622e 7265 7365 6172  s://colab.resear
+00002210: 6368 2e67 6f6f 676c 652e 636f 6d2f 6472  ch.google.com/dr
+00002220: 6976 652f 3141 5f2d 4d33 537a 356d 6151  ive/1A_-M3Sz5maQ
+00002230: 6d79 6657 3241 3772 4575 2d67 5f5a 6930  myfW2A7rEu-g_Zi0
+00002240: 524d 477a 353f 7573 703d 7368 6172 696e  RMGz5?usp=sharin
+00002250: 6729 206f 7220 7468 6520 776f 726b 6564  g) or the worked
+00002260: 2065 7861 6d70 6c65 7320 6265 6c6f 772c   examples below,
+00002270: 2077 6869 6368 2079 6f75 2063 616e 2063   which you can c
+00002280: 6f70 7920 616e 6420 6164 6170 742e 0a0a  opy and adapt...
+00002290: 466f 7220 636f 6e74 6578 7420 616e 6420  For context and 
+000022a0: 6578 706c 616e 6174 696f 6e2c 2073 6565  explanation, see
+000022b0: 2074 6865 205b 646f 6375 6d65 6e74 6174   the [documentat
+000022c0: 696f 6e5d 2868 7474 7073 3a2f 2f7a 6f6f  ion](https://zoo
+000022d0: 626f 742e 7265 6164 7468 6564 6f63 732e  bot.readthedocs.
+000022e0: 696f 2f29 2e0a 0a50 7265 7472 6169 6e65  io/)...Pretraine
+000022f0: 6420 6d6f 6465 6c73 2061 7265 206c 6973  d models are lis
+00002300: 7465 6420 5b68 6572 655d 2868 7474 7073  ted [here](https
+00002310: 3a2f 2f7a 6f6f 626f 742e 7265 6164 7468  ://zoobot.readth
+00002320: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00002330: 7374 2f70 7265 7472 6169 6e65 645f 6d6f  st/pretrained_mo
+00002340: 6465 6c73 2e68 746d 6c29 2061 6e64 2061  dels.html) and a
+00002350: 7661 696c 6162 6c65 206f 6e20 5b48 7567  vailable on [Hug
+00002360: 6769 6e67 4661 6365 5d28 6874 7470 733a  gingFace](https:
+00002370: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00002380: 2f63 6f6c 6c65 6374 696f 6e73 2f6d 7761  /collections/mwa
+00002390: 6c6d 736c 6579 2f7a 6f6f 626f 742d 656e  lmsley/zoobot-en
+000023a0: 636f 6465 7273 2d36 3566 6131 3461 6539  coders-65fa14ae9
+000023b0: 3239 3131 6231 3733 3731 3262 3837 3429  2911b173712b874)
+000023c0: 0a0a 2323 2320 576f 726b 6564 2045 7861  ..### Worked Exa
+000023d0: 6d70 6c65 730a 0a3c 6120 6e61 6d65 3d22  mples..<a name="
+000023e0: 776f 726b 6564 5f65 7861 6d70 6c65 7322  worked_examples"
+000023f0: 3e3c 2f61 3e0a 0a50 7954 6f72 6368 2028  ></a>..PyTorch (
+00002400: 7265 636f 6d6d 656e 6465 6429 3a0a 0a2d  recommended):..-
+00002410: 205b 7079 746f 7263 682f 6578 616d 706c   [pytorch/exampl
+00002420: 6573 2f66 696e 6574 756e 696e 672f 6669  es/finetuning/fi
+00002430: 6e65 7475 6e65 5f62 696e 6172 795f 636c  netune_binary_cl
+00002440: 6173 7369 6669 6361 7469 6f6e 2e70 795d  assification.py]
+00002450: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00002460: 636f 6d2f 6d77 616c 6d73 6c65 792f 7a6f  com/mwalmsley/zo
+00002470: 6f62 6f74 2f62 6c6f 622f 6d61 696e 2f7a  obot/blob/main/z
+00002480: 6f6f 626f 742f 7079 746f 7263 682f 6578  oobot/pytorch/ex
+00002490: 616d 706c 6573 2f66 696e 6574 756e 696e  amples/finetunin
+000024a0: 672f 6669 6e65 7475 6e65 5f62 696e 6172  g/finetune_binar
+000024b0: 795f 636c 6173 7369 6669 6361 7469 6f6e  y_classification
+000024c0: 2e70 7929 0a2d 205b 7079 746f 7263 682f  .py).- [pytorch/
+000024d0: 6578 616d 706c 6573 2f66 696e 6574 756e  examples/finetun
+000024e0: 696e 672f 6669 6e65 7475 6e65 5f63 6f75  ing/finetune_cou
+000024f0: 6e74 735f 6675 6c6c 5f74 7265 652e 7079  nts_full_tree.py
+00002500: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002510: 2e63 6f6d 2f6d 7761 6c6d 736c 6579 2f7a  .com/mwalmsley/z
+00002520: 6f6f 626f 742f 626c 6f62 2f6d 6169 6e2f  oobot/blob/main/
+00002530: 7a6f 6f62 6f74 2f70 7974 6f72 6368 2f65  zoobot/pytorch/e
+00002540: 7861 6d70 6c65 732f 6669 6e65 7475 6e69  xamples/finetuni
+00002550: 6e67 2f66 696e 6574 756e 655f 636f 756e  ng/finetune_coun
+00002560: 7473 5f66 756c 6c5f 7472 6565 2e70 7929  ts_full_tree.py)
+00002570: 0a2d 205b 7079 746f 7263 682f 6578 616d  .- [pytorch/exam
+00002580: 706c 6573 2f72 6570 7265 7365 6e74 6174  ples/representat
+00002590: 696f 6e73 2f67 6574 5f72 6570 7265 7365  ions/get_represe
+000025a0: 6e74 6174 696f 6e73 2e70 795d 2868 7474  ntations.py](htt
+000025b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000025c0: 6d77 616c 6d73 6c65 792f 7a6f 6f62 6f74  mwalmsley/zoobot
+000025d0: 2f62 6c6f 622f 6d61 696e 2f7a 6f6f 626f  /blob/main/zoobo
+000025e0: 742f 7079 746f 7263 682f 6578 616d 706c  t/pytorch/exampl
+000025f0: 6573 2f72 6570 7265 7365 6e74 6174 696f  es/representatio
+00002600: 6e73 2f67 6574 5f72 6570 7265 7365 6e74  ns/get_represent
+00002610: 6174 696f 6e73 2e70 7929 0a2d 205b 7079  ations.py).- [py
+00002620: 746f 7263 682f 6578 616d 706c 6573 2f74  torch/examples/t
+00002630: 7261 696e 5f6d 6f64 656c 5f6f 6e5f 6361  rain_model_on_ca
+00002640: 7461 6c6f 672e 7079 5d28 6874 7470 733a  talog.py](https:
+00002650: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 7761  //github.com/mwa
+00002660: 6c6d 736c 6579 2f7a 6f6f 626f 742f 626c  lmsley/zoobot/bl
+00002670: 6f62 2f6d 6169 6e2f 7a6f 6f62 6f74 2f70  ob/main/zoobot/p
+00002680: 7974 6f72 6368 2f65 7861 6d70 6c65 732f  ytorch/examples/
+00002690: 7472 6169 6e5f 6d6f 6465 6c5f 6f6e 5f63  train_model_on_c
+000026a0: 6174 616c 6f67 2e70 7929 2028 6f6e 6c79  atalog.py) (only
+000026b0: 206e 6563 6573 7361 7279 2074 6f20 7472   necessary to tr
+000026c0: 6169 6e20 6672 6f6d 2073 6372 6174 6368  ain from scratch
+000026d0: 290a 0a54 6865 7265 2069 7320 6d6f 7265  )..There is more
+000026e0: 2065 7870 6c61 6e61 7469 6f6e 2061 6e64   explanation and
+000026f0: 2061 6e20 4150 4920 7265 6665 7265 6e63   an API referenc
+00002700: 6520 6f6e 2074 6865 205b 646f 6373 5d28  e on the [docs](
+00002710: 6874 7470 733a 2f2f 7a6f 6f62 6f74 2e72  https://zoobot.r
+00002720: 6561 6474 6865 646f 6373 2e69 6f2f 292e  eadthedocs.io/).
+00002730: 0a0a 4920 616c 736f 205b 696e 636c 7564  ..I also [includ
+00002740: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00002750: 622e 636f 6d2f 6d77 616c 6d73 6c65 792f  b.com/mwalmsley/
+00002760: 7a6f 6f62 6f74 2f62 6c6f 622f 6d61 696e  zoobot/blob/main
+00002770: 2f62 656e 6368 6d61 726b 7329 2074 6865  /benchmarks) the
+00002780: 2073 6372 6970 7473 2075 7365 6420 746f   scripts used to
+00002790: 2063 7265 6174 6520 616e 6420 6265 6e63   create and benc
+000027a0: 686d 6172 6b20 6f75 7220 7072 6574 7261  hmark our pretra
+000027b0: 696e 6564 206d 6f64 656c 732e 204d 616e  ined models. Man
+000027c0: 7920 7072 6574 7261 696e 6564 206d 6f64  y pretrained mod
+000027d0: 656c 7320 6172 6520 6176 6169 6c61 626c  els are availabl
+000027e0: 6520 5b61 6c72 6561 6479 5d28 6874 7470  e [already](http
+000027f0: 733a 2f2f 7a6f 6f62 6f74 2e72 6561 6474  s://zoobot.readt
+00002800: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00002810: 6573 742f 6461 7461 5f6e 6f74 6573 2e68  est/data_notes.h
+00002820: 746d 6c29 2c20 6275 7420 6966 2079 6f75  tml), but if you
+00002830: 206e 6565 6420 6f6e 6520 7472 6169 6e65   need one traine
+00002840: 6420 6f6e 2065 2e67 2e20 6469 6666 6572  d on e.g. differ
+00002850: 656e 7420 696e 7075 7420 696d 6167 6520  ent input image 
+00002860: 7369 7a65 7320 6f72 2077 6974 6820 6120  sizes or with a 
+00002870: 7370 6563 6966 6963 2061 7263 6869 7465  specific archite
+00002880: 6374 7572 652c 2049 2063 616e 2070 726f  cture, I can pro
+00002890: 6261 626c 7920 6d61 6b65 2069 7420 666f  bably make it fo
+000028a0: 7220 796f 752e 0a0a 5768 656e 2074 7261  r you...When tra
+000028b0: 696e 6564 2077 6974 6820 6120 6465 6369  ined with a deci
+000028c0: 7369 6f6e 2074 7265 6520 6865 6164 2028  sion tree head (
+000028d0: 5a6f 6f62 6f74 5472 6565 2c20 4669 6e65  ZoobotTree, Fine
+000028e0: 7475 6e65 6162 6c65 5a6f 6f62 6f74 5472  tuneableZoobotTr
+000028f0: 6565 292c 205a 6f6f 626f 7420 6361 6e20  ee), Zoobot can 
+00002900: 6c65 6172 6e20 6672 6f6d 2076 6f6c 756e  learn from volun
+00002910: 7465 6572 206c 6162 656c 7320 6f66 2076  teer labels of v
+00002920: 6172 7969 6e67 2063 6f6e 6669 6465 6e63  arying confidenc
+00002930: 6520 616e 6420 7072 6564 6963 7420 706f  e and predict po
+00002940: 7374 6572 696f 7273 2066 6f72 2077 6861  steriors for wha
+00002950: 7420 7468 6520 7479 7069 6361 6c20 766f  t the typical vo
+00002960: 6c75 6e74 6565 7220 6d69 6768 7420 7361  lunteer might sa
+00002970: 792e 2053 7065 6369 6669 6361 6c6c 792c  y. Specifically,
+00002980: 2074 6869 7320 5a6f 6f62 6f74 206d 6f64   this Zoobot mod
+00002990: 6520 7072 6564 6963 7473 2074 6865 2070  e predicts the p
+000029a0: 6172 616d 6574 6572 7320 666f 7220 6469  arameters for di
+000029b0: 7374 7269 6275 7469 6f6e 732c 206e 6f74  stributions, not
+000029c0: 2073 696d 706c 6520 636c 6173 7320 6c61   simple class la
+000029d0: 6265 6c73 2120 466f 7220 6120 6465 6d6f  bels! For a demo
+000029e0: 6e73 7472 6174 696f 6e20 6f66 2068 6f77  nstration of how
+000029f0: 2074 6f20 696e 7465 7270 7265 7420 7468   to interpret th
+00002a00: 6573 6520 7072 6564 6963 7469 6f6e 732c  ese predictions,
+00002a10: 2073 6565 2074 6865 205b 677a 5f64 6563   see the [gz_dec
+00002a20: 616c 735f 6461 7461 5f72 656c 6561 7365  als_data_release
+00002a30: 5f61 6e61 6c79 7369 735f 6465 6d6f 2e69  _analysis_demo.i
+00002a40: 7079 6e62 5d28 6874 7470 733a 2f2f 6769  pynb](https://gi
+00002a50: 7468 7562 2e63 6f6d 2f6d 7761 6c6d 736c  thub.com/mwalmsl
+00002a60: 6579 2f7a 6f6f 626f 742f 626c 6f62 2f6d  ey/zoobot/blob/m
+00002a70: 6169 6e2f 677a 5f64 6563 616c 735f 6461  ain/gz_decals_da
+00002a80: 7461 5f72 656c 6561 7365 5f61 6e61 6c79  ta_release_analy
+00002a90: 7369 735f 6465 6d6f 2e69 7079 6e62 292e  sis_demo.ipynb).
+00002aa0: 0a0a 0a23 2323 2028 4f70 7469 6f6e 616c  ...### (Optional
+00002ab0: 2920 496e 7374 616c 6c20 5079 546f 7263  ) Install PyTorc
+00002ac0: 6820 7769 7468 2043 5544 410a 0a3c 6120  h with CUDA..<a 
+00002ad0: 6e61 6d65 3d22 696e 7374 616c 6c5f 6375  name="install_cu
+00002ae0: 6461 223e 3c2f 613e 0a0a 2a49 6620 796f  da"></a>..*If yo
+00002af0: 7527 7265 206e 6f74 2075 7369 6e67 2061  u're not using a
+00002b00: 2047 5055 2c20 736b 6970 2074 6869 7320   GPU, skip this 
+00002b10: 7374 6570 2e20 5573 6520 7468 6520 7079  step. Use the py
+00002b20: 746f 7263 682d 6370 7520 6f70 7469 6f6e  torch-cpu option
+00002b30: 2069 6e20 7468 6520 7365 6374 696f 6e20   in the section 
+00002b40: 6265 6c6f 772e 2a0a 0a49 6e73 7461 6c6c  below.*..Install
+00002b50: 2050 7954 6f72 6368 2032 2e31 2e30 206f   PyTorch 2.1.0 o
+00002b60: 7220 5465 6e73 6f72 666c 6f77 2032 2e31  r Tensorflow 2.1
+00002b70: 302e 3020 616e 6420 636f 6d70 6174 6962  0.0 and compatib
+00002b80: 6c65 2043 5544 4120 6472 6976 6572 732e  le CUDA drivers.
+00002b90: 2049 2068 6967 686c 7920 7265 636f 6d6d   I highly recomm
+00002ba0: 656e 6420 7573 696e 6720 5b63 6f6e 6461  end using [conda
+00002bb0: 5d28 6874 7470 733a 2f2f 646f 6373 2e63  ](https://docs.c
+00002bc0: 6f6e 6461 2e69 6f2f 656e 2f6c 6174 6573  onda.io/en/lates
+00002bd0: 742f 6d69 6e69 636f 6e64 612e 6874 6d6c  t/miniconda.html
+00002be0: 2920 746f 2064 6f20 7468 6973 2e20 436f  ) to do this. Co
+00002bf0: 6e64 6120 7769 6c6c 2068 616e 646c 6520  nda will handle 
+00002c00: 626f 7468 2063 7265 6174 696e 6720 6120  both creating a 
+00002c10: 6e65 7720 7669 7274 7561 6c20 656e 7669  new virtual envi
+00002c20: 726f 6e6d 656e 7420 2860 636f 6e64 6120  ronment (`conda 
+00002c30: 6372 6561 7465 6029 2061 6e64 2069 6e73  create`) and ins
+00002c40: 7461 6c6c 696e 6720 4355 4441 2028 6063  talling CUDA (`c
+00002c50: 7564 6174 6f6f 6c6b 6974 602c 2060 6375  udatoolkit`, `cu
+00002c60: 646e 6e60 290a 0a43 5544 4120 3132 2e31  dnn`)..CUDA 12.1
+00002c70: 2066 6f72 2050 7954 6f72 6368 2032 2e31   for PyTorch 2.1
+00002c80: 2e30 3a0a 0a20 2020 2063 6f6e 6461 2063  .0:..    conda c
+00002c90: 7265 6174 6520 2d2d 6e61 6d65 207a 6f6f  reate --name zoo
+00002ca0: 626f 7433 395f 746f 7263 6820 7079 7468  bot39_torch pyth
+00002cb0: 6f6e 3d3d 332e 390a 2020 2020 636f 6e64  on==3.9.    cond
+00002cc0: 6120 6163 7469 7661 7465 207a 6f6f 626f  a activate zoobo
+00002cd0: 7433 395f 746f 7263 680a 2020 2020 636f  t39_torch.    co
+00002ce0: 6e64 6120 696e 7374 616c 6c20 2d63 2063  nda install -c c
+00002cf0: 6f6e 6461 2d66 6f72 6765 2063 7564 6174  onda-forge cudat
+00002d00: 6f6f 6c6b 6974 3d31 322e 310a 0a23 2323  oolkit=12.1..###
+00002d10: 2052 6563 656e 7420 7265 6c65 6173 6520   Recent release 
+00002d20: 6665 6174 7572 6573 2028 7632 2e30 2e30  features (v2.0.0
+00002d30: 290a 0a2d 204e 6577 2070 7265 7472 6169  )..- New pretrai
+00002d40: 6e65 6420 6172 6368 6974 6563 7475 7265  ned architecture
+00002d50: 733a 2043 6f6e 764e 6558 542c 2045 6666  s: ConvNeXT, Eff
+00002d60: 6963 6965 6e74 4e65 7456 322c 204d 6178  icientNetV2, Max
+00002d70: 5669 542c 2061 6e64 206d 6f72 652e 2045  ViT, and more. E
+00002d80: 6163 6820 696e 2073 6576 6572 616c 2073  ach in several s
+00002d90: 697a 6573 2e0a 2d20 5265 776f 726b 6564  izes..- Reworked
+00002da0: 2066 696e 6574 756e 696e 6720 7072 6f63   finetuning proc
+00002db0: 6564 7572 652e 2041 6c6c 2074 6865 7365  edure. All these
+00002dc0: 2061 7263 6869 7465 6374 7572 6573 2061   architectures a
+00002dd0: 7265 2066 696e 6574 756e 6561 626c 6520  re finetuneable 
+00002de0: 7468 726f 7567 6820 6120 636f 6d6d 6f6e  through a common
+00002df0: 206d 6574 686f 642e 0a2d 2052 6577 6f72   method..- Rewor
+00002e00: 6b65 6420 6669 6e65 7475 6e69 6e67 206f  ked finetuning o
+00002e10: 7074 696f 6e73 2e20 4261 7463 6820 6e6f  ptions. Batch no
+00002e20: 726d 2066 696e 6574 756e 696e 6720 7265  rm finetuning re
+00002e30: 6d6f 7665 642e 2043 6f73 696e 6520 7363  moved. Cosine sc
+00002e40: 6865 6475 6c65 206f 7074 696f 6e20 6164  hedule option ad
+00002e50: 6465 642e 0a2d 2052 6577 6f72 6b65 6420  ded..- Reworked 
+00002e60: 6669 6e65 7475 6e69 6e67 2073 6176 696e  finetuning savin
+00002e70: 672f 6c6f 6164 696e 672e 2041 7574 6f2d  g/loading. Auto-
+00002e80: 646f 776e 6c6f 6164 7320 656e 636f 6465  downloads encode
+00002e90: 7220 6672 6f6d 2048 7567 6769 6e67 4661  r from HuggingFa
+00002ea0: 6365 2e0a 2d20 4e6f 7720 7375 7070 6f72  ce..- Now suppor
+00002eb0: 7473 2072 6567 7265 7373 696f 6e20 6669  ts regression fi
+00002ec0: 6e65 7475 6e69 6e67 2028 6173 2077 656c  netuning (as wel
+00002ed0: 6c20 6173 206d 756c 7469 2d63 6c61 7373  l as multi-class
+00002ee0: 2061 6e64 2062 696e 6172 7929 2e20 5365   and binary). Se
+00002ef0: 6520 6070 7974 6f72 6368 2f65 7861 6d70  e `pytorch/examp
+00002f00: 6c65 732f 6669 6e65 7475 6e69 6e67 600a  les/finetuning`.
+00002f10: 2d20 5570 6461 7465 6420 6074 696d 6d60  - Updated `timm`
+00002f20: 2074 6f20 302e 392e 3130 2c20 616c 6c6f   to 0.9.10, allo
+00002f30: 7769 6e67 206c 6174 6573 7420 6d6f 6465  wing latest mode
+00002f40: 6c20 6172 6368 6974 6563 7475 7265 732e  l architectures.
+00002f50: 2050 7265 7669 6f75 736c 7920 646f 776e   Previously down
+00002f60: 6c6f 6164 6564 2063 6865 636b 706f 696e  loaded checkpoin
+00002f70: 7473 206d 6179 206e 6f74 206c 6f61 6420  ts may not load 
+00002f80: 636f 7272 6563 746c 7921 0a2d 2028 696e  correctly!.- (in
+00002f90: 7465 726e 616c 2075 6e74 696c 2070 7562  ternal until pub
+00002fa0: 6c69 7368 6564 2920 475a 2045 766f 2076  lished) GZ Evo v
+00002fb0: 3220 6e6f 7720 696e 636c 7564 6573 2043  2 now includes C
+00002fc0: 6f73 6d69 6320 4461 776e 2028 4853 4320  osmic Dawn (HSC 
+00002fd0: 4832 4f29 2e20 5369 676e 6966 6963 616e  H2O). Significan
+00002fe0: 7420 7065 7266 6f72 6d61 6e63 6520 696d  t performance im
+00002ff0: 7072 6f76 656d 656e 7420 6f6e 2048 5343  provement on HSC
+00003000: 2066 696e 6574 756e 696e 672e 2041 6c73   finetuning. Als
+00003010: 6f20 6e6f 7720 696e 636c 7564 6573 2047  o now includes G
+00003020: 5a20 554b 4944 5353 2028 6472 6167 6765  Z UKIDSS (dragge
+00003030: 6420 6672 6f6d 206f 7572 2061 7263 6869  d from our archi
+00003040: 7665 7329 2e0a 2d20 5570 6461 7465 6420  ves)..- Updated 
+00003050: 6070 7974 6f72 6368 6020 746f 2060 322e  `pytorch` to `2.
+00003060: 312e 3060 0a2d 2041 6464 6564 2073 7570  1.0`.- Added sup
+00003070: 706f 7274 2066 6f72 2077 6562 6461 7461  port for webdata
+00003080: 7365 7473 2028 6f6e 6c79 2072 6563 6f6d  sets (only recom
+00003090: 6d65 6e64 6564 2066 6f72 206c 6172 6765  mended for large
+000030a0: 2d73 6361 6c65 2064 6973 7472 6962 7574  -scale distribut
+000030b0: 6564 2074 7261 696e 696e 6729 0a2d 2049  ed training).- I
+000030c0: 6d70 726f 7665 6420 7065 722d 7175 6573  mproved per-ques
+000030d0: 7469 6f6e 206c 6f67 6769 6e67 2077 6865  tion logging whe
+000030e0: 6e20 7472 6169 6e69 6e67 2066 726f 6d20  n training from 
+000030f0: 7363 7261 7463 680a 2d20 4164 6465 6420  scratch.- Added 
+00003100: 6f70 7469 6f6e 2074 6f20 636f 6d70 696c  option to compil
+00003110: 6520 656e 636f 6465 7220 666f 7220 6d61  e encoder for ma
+00003120: 7820 7370 6565 6420 286e 6f74 2072 6563  x speed (not rec
+00003130: 6f6d 6d65 6e64 6564 2066 6f72 2066 696e  ommended for fin
+00003140: 6574 756e 696e 672c 206f 6e6c 7920 666f  etuning, only fo
+00003150: 7220 7072 6574 7261 696e 696e 6729 2e0a  r pretraining)..
+00003160: 2d20 4465 7072 6563 6174 6573 2054 656e  - Deprecates Ten
+00003170: 736f 7246 6c6f 772e 2054 6865 2043 5320  sorFlow. The CS 
+00003180: 7265 7365 6172 6368 2063 6f6d 6d75 6e69  research communi
+00003190: 7479 2066 6f63 7573 6573 206f 6e20 5079  ty focuses on Py
+000031a0: 546f 7263 6820 616e 6420 6e65 7720 6672  Torch and new fr
+000031b0: 616d 6577 6f72 6b73 206c 696b 6520 4a41  ameworks like JA
+000031c0: 582e 0a0a 436f 6e74 7269 6275 7469 6f6e  X...Contribution
+000031d0: 7320 6172 6520 7665 7279 2077 656c 636f  s are very welco
+000031e0: 6d65 2061 6e64 2077 696c 6c20 6265 2063  me and will be c
+000031f0: 7265 6469 7465 6420 696e 2061 6e79 2066  redited in any f
+00003200: 7574 7572 6520 776f 726b 2e20 506c 6561  uture work. Plea
+00003210: 7365 2067 6574 2069 6e20 746f 7563 6821  se get in touch!
+00003220: 2053 6565 205b 434f 4e54 5249 4255 5449   See [CONTRIBUTI
+00003230: 4e47 2e6d 645d 2868 7474 7073 3a2f 2f67  NG.md](https://g
+00003240: 6974 6875 622e 636f 6d2f 6d77 616c 6d73  ithub.com/mwalms
+00003250: 6c65 792f 7a6f 6f62 6f74 2f62 6c6f 622f  ley/zoobot/blob/
+00003260: 6d61 696e 2f62 656e 6368 6d61 726b 7329  main/benchmarks)
+00003270: 2066 6f72 206d 6f72 652e 0a0a 2323 2320   for more...### 
+00003280: 4265 6e63 686d 6172 6b73 2061 6e64 2052  Benchmarks and R
+00003290: 6570 6c69 6361 7469 6f6e 202d 2054 7261  eplication - Tra
+000032a0: 696e 696e 6720 6672 6f6d 2053 6372 6174  ining from Scrat
+000032b0: 6368 0a0a 5468 6520 5b62 656e 6368 6d61  ch..The [benchma
+000032c0: 726b 735d 2868 7474 7073 3a2f 2f67 6974  rks](https://git
+000032d0: 6875 622e 636f 6d2f 6d77 616c 6d73 6c65  hub.com/mwalmsle
+000032e0: 792f 7a6f 6f62 6f74 2f62 6c6f 622f 6d61  y/zoobot/blob/ma
+000032f0: 696e 2f62 656e 6368 6d61 726b 7329 2066  in/benchmarks) f
+00003300: 6f6c 6465 7220 636f 6e74 6169 6e73 2073  older contains s
+00003310: 6c75 726d 2061 6e64 2050 7974 686f 6e20  lurm and Python 
+00003320: 7363 7269 7074 7320 746f 2074 7261 696e  scripts to train
+00003330: 205a 6f6f 626f 7420 6672 6f6d 2073 6372   Zoobot from scr
+00003340: 6174 6368 2e20 5765 2075 7365 2074 6865  atch. We use the
+00003350: 7365 2073 6372 6970 7473 2074 6f20 6d61  se scripts to ma
+00003360: 6b65 2073 7572 6520 6e65 7720 636f 6465  ke sure new code
+00003370: 2076 6572 7369 6f6e 7320 776f 726b 2077   versions work w
+00003380: 656c 6c2c 2061 6e64 2074 6861 7420 5465  ell, and that Te
+00003390: 6e73 6f72 466c 6f77 2061 6e64 2050 7954  nsorFlow and PyT
+000033a0: 6f72 6368 2061 6368 6965 7665 2073 696d  orch achieve sim
+000033b0: 696c 6172 2070 6572 666f 726d 616e 6365  ilar performance
+000033c0: 2e0a 0a54 7261 696e 696e 6720 5a6f 6f62  ...Training Zoob
+000033d0: 6f74 2075 7369 6e67 2074 6865 2047 5a20  ot using the GZ 
+000033e0: 4445 4361 4c53 2064 6174 6173 6574 206f  DECaLS dataset o
+000033f0: 7074 696f 6e20 7769 6c6c 2063 7265 6174  ption will creat
+00003400: 6520 6d6f 6465 6c73 2076 6572 7920 7369  e models very si
+00003410: 6d69 6c61 7220 746f 2074 686f 7365 2075  milar to those u
+00003420: 7365 6420 666f 7220 7468 6520 475a 2044  sed for the GZ D
+00003430: 4543 614c 5320 6361 7461 6c6f 6775 6520  ECaLS catalogue 
+00003440: 616e 6420 7368 6172 6564 2077 6974 6820  and shared with 
+00003450: 7468 6520 6561 726c 7920 7665 7273 696f  the early versio
+00003460: 6e73 206f 6620 7468 6973 2072 6570 6f2e  ns of this repo.
+00003470: 2054 6865 2047 5a20 4445 5349 205a 6f6f   The GZ DESI Zoo
+00003480: 626f 7420 6d6f 6465 6c20 6973 2074 7261  bot model is tra
+00003490: 696e 6564 206f 6e20 6164 6469 7469 6f6e  ined on addition
+000034a0: 616c 2064 6174 6120 2847 5a44 2d31 2c20  al data (GZD-1, 
+000034b0: 475a 442d 3229 2c20 6173 2074 6865 2047  GZD-2), as the G
+000034c0: 5a20 4576 6f20 5a6f 6f62 6f74 206d 6f64  Z Evo Zoobot mod
+000034d0: 656c 2028 475a 442d 312f 322f 352c 2048  el (GZD-1/2/5, H
+000034e0: 7562 626c 652c 2043 616e 6465 6c73 2c20  ubble, Candels, 
+000034f0: 475a 3229 2e0a 0a2a 2a50 7265 7472 6169  GZ2)...**Pretrai
+00003500: 6e69 6e67 2069 7320 6265 636f 6d69 6e67  ning is becoming
+00003510: 2069 6e63 7265 6173 696e 676c 7920 636f   increasingly co
+00003520: 6d70 6c65 7820 616e 6420 6973 206e 6f77  mplex and is now
+00003530: 2070 6172 7469 616c 6c79 2072 6566 6163   partially refac
+00003540: 746f 7265 6420 6f75 7420 746f 2061 2073  tored out to a s
+00003550: 6570 6172 6174 6520 7265 706f 7369 746f  eparate reposito
+00003560: 7279 2e20 5765 2061 7265 2067 7261 6475  ry. We are gradu
+00003570: 616c 6c79 206d 6967 7261 7469 6e67 2074  ally migrating t
+00003580: 6869 7320 607a 6f6f 626f 7460 2072 6570  his `zoobot` rep
+00003590: 6f73 6974 6f72 7920 746f 2066 6f63 7573  ository to focus
+000035a0: 206f 6e20 6669 6e65 7475 6e69 6e67 2e2a   on finetuning.*
+000035b0: 2a0a 0a23 2323 2043 6974 696e 670a 0a49  *..### Citing..I
+000035c0: 6620 796f 7520 7573 6520 7468 6973 2073  f you use this s
+000035d0: 6f66 7477 6172 652c 206f 7220 6f74 6865  oftware, or othe
+000035e0: 7277 6973 6520 7769 7368 2074 6f20 6369  rwise wish to ci
+000035f0: 7465 205a 6f6f 626f 7420 6173 2061 2073  te Zoobot as a s
+00003600: 6f66 7477 6172 6520 7061 636b 6167 652c  oftware package,
+00003610: 2070 6c65 6173 6520 7573 6520 7468 6520   please use the 
+00003620: 5b4a 4f53 5320 7061 7065 725d 2868 7474  [JOSS paper](htt
+00003630: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00003640: 3231 3130 352f 6a6f 7373 2e30 3533 3132  21105/joss.05312
+00003650: 293a 0a0a 2020 2020 4061 7274 6963 6c65  ):..    @article
+00003660: 7b57 616c 6d73 6c65 7932 3032 332c 2064  {Walmsley2023, d
+00003670: 6f69 203d 207b 3130 2e32 3131 3035 2f6a  oi = {10.21105/j
+00003680: 6f73 732e 3035 3331 327d 2c20 7572 6c20  oss.05312}, url 
+00003690: 3d20 7b68 7474 7073 3a2f 2f64 6f69 2e6f  = {https://doi.o
+000036a0: 7267 2f31 302e 3231 3130 352f 6a6f 7373  rg/10.21105/joss
+000036b0: 2e30 3533 3132 7d2c 2079 6561 7220 3d20  .05312}, year = 
+000036c0: 7b32 3032 337d 2c20 7075 626c 6973 6865  {2023}, publishe
+000036d0: 7220 3d20 7b54 6865 204f 7065 6e20 4a6f  r = {The Open Jo
+000036e0: 7572 6e61 6c7d 2c20 766f 6c75 6d65 203d  urnal}, volume =
+000036f0: 207b 387d 2c20 6e75 6d62 6572 203d 207b   {8}, number = {
+00003700: 3835 7d2c 2070 6167 6573 203d 207b 3533  85}, pages = {53
+00003710: 3132 7d2c 2061 7574 686f 7220 3d20 7b4d  12}, author = {M
+00003720: 696b 6520 5761 6c6d 736c 6579 2061 6e64  ike Walmsley and
+00003730: 2043 616d 7062 656c 6c20 416c 6c65 6e20   Campbell Allen 
+00003740: 616e 6420 4265 6e20 4175 7373 656c 2061  and Ben Aussel a
+00003750: 6e64 204d 6963 6168 2042 6f77 6c65 7320  nd Micah Bowles 
+00003760: 616e 6420 4b61 7369 6120 4772 6567 6f72  and Kasia Gregor
+00003770: 6f77 6963 7a20 616e 6420 496e 6967 6f20  owicz and Inigo 
+00003780: 5661 6c20 536c 696a 6570 6365 7669 6320  Val Slijepcevic 
+00003790: 616e 6420 4368 7269 7320 4a2e 204c 696e  and Chris J. Lin
+000037a0: 746f 7474 2061 6e64 2041 6e6e 6120 4d2e  tott and Anna M.
+000037b0: 206d 2e20 5363 6169 6665 2061 6e64 204d   m. Scaife and M
+000037c0: 616a 6120 4a61 62c5 826f c584 736b 6120  aja Jab..o..ska 
+000037d0: 616e 6420 4b6f 7369 6f20 4b61 7263 6865  and Kosio Karche
+000037e0: 7620 616e 6420 4465 6e69 7365 204c 616e  v and Denise Lan
+000037f0: 7a69 6572 6920 616e 6420 4465 7669 6e61  zieri and Devina
+00003800: 204d 6f68 616e 2061 6e64 2044 6176 6964   Mohan and David
+00003810: 204f e280 9952 7961 6e20 616e 6420 4268   O...Ryan and Bh
+00003820: 6172 6174 6820 5361 6967 7568 616e 2061  arath Saiguhan a
+00003830: 6e64 2043 7269 7365 6c20 5375 c3a1 7265  nd Crisel Su..re
+00003840: 7a20 616e 6420 4e69 636f 6cc3 a173 2047  z and Nicol..s G
+00003850: 7565 7272 612d 5661 7261 7320 616e 6420  uerra-Varas and 
+00003860: 5265 6e75 6b61 2056 656c 757d 2c20 7469  Renuka Velu}, ti
+00003870: 746c 6520 3d20 7b5a 6f6f 626f 743a 2041  tle = {Zoobot: A
+00003880: 6461 7074 6162 6c65 2044 6565 7020 4c65  daptable Deep Le
+00003890: 6172 6e69 6e67 204d 6f64 656c 7320 666f  arning Models fo
+000038a0: 7220 4761 6c61 7879 204d 6f72 7068 6f6c  r Galaxy Morphol
+000038b0: 6f67 797d 2c20 6a6f 7572 6e61 6c20 3d20  ogy}, journal = 
+000038c0: 7b4a 6f75 726e 616c 206f 6620 4f70 656e  {Journal of Open
+000038d0: 2053 6f75 7263 6520 536f 6674 7761 7265   Source Software
+000038e0: 7d20 7d20 0a0a 596f 7520 6d69 6768 7420  } } ..You might 
+000038f0: 6265 2069 6e74 6572 6573 7465 6420 696e  be interested in
+00003900: 2072 6561 6469 6e67 2070 6170 6572 7320   reading papers 
+00003910: 7573 696e 6720 5a6f 6f62 6f74 3a0a 0a2d  using Zoobot:..-
+00003920: 205b 4761 6c61 7879 205a 6f6f 2044 4543   [Galaxy Zoo DEC
+00003930: 614c 533a 2044 6574 6169 6c65 6420 7669  aLS: Detailed vi
+00003940: 7375 616c 206d 6f72 7068 6f6c 6f67 7920  sual morphology 
+00003950: 6d65 6173 7572 656d 656e 7473 2066 726f  measurements fro
+00003960: 6d20 766f 6c75 6e74 6565 7273 2061 6e64  m volunteers and
+00003970: 2064 6565 7020 6c65 6172 6e69 6e67 2066   deep learning f
+00003980: 6f72 2033 3134 2c30 3030 2067 616c 6178  or 314,000 galax
+00003990: 6965 735d 2868 7474 7073 3a2f 2f61 7278  ies](https://arx
+000039a0: 6976 2e6f 7267 2f61 6273 2f32 3130 322e  iv.org/abs/2102.
+000039b0: 3038 3431 3429 2028 3230 3232 290a 2d20  08414) (2022).- 
+000039c0: 5b41 2043 6f6d 7061 7269 736f 6e20 6f66  [A Comparison of
+000039d0: 2044 6565 7020 4c65 6172 6e69 6e67 2041   Deep Learning A
+000039e0: 7263 6869 7465 6374 7572 6573 2066 6f72  rchitectures for
+000039f0: 204f 7074 6963 616c 2047 616c 6178 7920   Optical Galaxy 
+00003a00: 4d6f 7270 686f 6c6f 6779 2043 6c61 7373  Morphology Class
+00003a10: 6966 6963 6174 696f 6e5d 2868 7474 7073  ification](https
+00003a20: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
+00003a30: 2f32 3131 312e 3034 3335 3329 2028 3230  /2111.04353) (20
+00003a40: 3232 290a 2d20 5b50 7261 6374 6963 616c  22).- [Practical
+00003a50: 2047 616c 6178 7920 4d6f 7270 686f 6c6f   Galaxy Morpholo
+00003a60: 6779 2054 6f6f 6c73 2066 726f 6d20 4465  gy Tools from De
+00003a70: 6570 2053 7570 6572 7669 7365 6420 5265  ep Supervised Re
+00003a80: 7072 6573 656e 7461 7469 6f6e 204c 6561  presentation Lea
+00003a90: 726e 696e 675d 2868 7474 7073 3a2f 2f61  rning](https://a
+00003aa0: 7278 6976 2e6f 7267 2f61 6273 2f32 3131  rxiv.org/abs/211
+00003ab0: 302e 3132 3733 3529 2028 3230 3232 290a  0.12735) (2022).
+00003ac0: 2d20 5b54 6f77 6172 6473 2046 6f75 6e64  - [Towards Found
+00003ad0: 6174 696f 6e20 4d6f 6465 6c73 2066 6f72  ation Models for
+00003ae0: 2047 616c 6178 7920 4d6f 7270 686f 6c6f   Galaxy Morpholo
+00003af0: 6779 5d28 6874 7470 733a 2f2f 6172 7869  gy](https://arxi
+00003b00: 762e 6f72 672f 6162 732f 3232 3036 2e31  v.org/abs/2206.1
+00003b10: 3139 3237 2920 2832 3032 3229 0a2d 205b  1927) (2022).- [
+00003b20: 4861 726e 6573 7369 6e67 2074 6865 2048  Harnessing the H
+00003b30: 7562 626c 6520 5370 6163 6520 5465 6c65  ubble Space Tele
+00003b40: 7363 6f70 6520 4172 6368 6976 6573 3a20  scope Archives: 
+00003b50: 4120 4361 7461 6c6f 6775 6520 6f66 2032  A Catalogue of 2
+00003b60: 312c 3932 3620 496e 7465 7261 6374 696e  1,926 Interactin
+00003b70: 6720 4761 6c61 7869 6573 5d28 6874 7470  g Galaxies](http
+00003b80: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00003b90: 732f 3233 3033 2e30 3033 3636 2920 2832  s/2303.00366) (2
+00003ba0: 3032 3329 0a2d 205b 4761 6c61 7879 205a  023).- [Galaxy Z
+00003bb0: 6f6f 2044 4553 493a 2044 6574 6169 6c65  oo DESI: Detaile
+00003bc0: 6420 6d6f 7270 686f 6c6f 6779 206d 6561  d morphology mea
+00003bd0: 7375 7265 6d65 6e74 7320 666f 7220 382e  surements for 8.
+00003be0: 374d 2067 616c 6178 6965 7320 696e 2074  7M galaxies in t
+00003bf0: 6865 2044 4553 4920 4c65 6761 6379 2049  he DESI Legacy I
+00003c00: 6d61 6769 6e67 2053 7572 7665 7973 5d28  maging Surveys](
+00003c10: 6874 7470 733a 2f2f 6163 6164 656d 6963  https://academic
+00003c20: 2e6f 7570 2e63 6f6d 2f6d 6e72 6173 2f61  .oup.com/mnras/a
+00003c30: 6476 616e 6365 2d61 7274 6963 6c65 2f64  dvance-article/d
+00003c40: 6f69 2f31 302e 3130 3933 2f6d 6e72 6173  oi/10.1093/mnras
+00003c50: 2f73 7461 6432 3931 392f 3732 3833 3136  /stad2919/728316
+00003c60: 393f 6c6f 6769 6e3d 6661 6c73 6529 2028  9?login=false) (
+00003c70: 3230 3233 290a 2d20 5b47 616c 6178 7920  2023).- [Galaxy 
+00003c80: 6d65 7267 6572 7320 696e 2053 7562 6172  mergers in Subar
+00003c90: 7520 4853 432d 5353 503a 2041 2064 6565  u HSC-SSP: A dee
+00003ca0: 7020 7265 7072 6573 656e 7461 7469 6f6e  p representation
+00003cb0: 206c 6561 726e 696e 6720 6170 7072 6f61   learning approa
+00003cc0: 6368 2066 6f72 2069 6465 6e74 6966 6963  ch for identific
+00003cd0: 6174 696f 6e2c 2061 6e64 2074 6865 2072  ation, and the r
+00003ce0: 6f6c 6520 6f66 2065 6e76 6972 6f6e 6d65  ole of environme
+00003cf0: 6e74 206f 6e20 6d65 7267 6572 2069 6e63  nt on merger inc
+00003d00: 6964 656e 6365 5d28 6874 7470 733a 2f2f  idence](https://
+00003d10: 646f 692e 6f72 672f 3130 2e31 3035 312f  doi.org/10.1051/
+00003d20: 3030 3034 2d36 3336 312f 3230 3233 3436  0004-6361/202346
+00003d30: 3734 3329 2028 3230 3233 290a 2d20 5b41  743) (2023).- [A
+00003d40: 7374 726f 6e6f 6d61 6c79 2061 7420 5363  stronomaly at Sc
+00003d50: 616c 653a 2053 6561 7263 6869 6e67 2066  ale: Searching f
+00003d60: 6f72 2041 6e6f 6d61 6c69 6573 2041 6d6f  or Anomalies Amo
+00003d70: 6e67 7374 2034 204d 696c 6c69 6f6e 2047  ngst 4 Million G
+00003d80: 616c 6178 6965 735d 2868 7474 7073 3a2f  alaxies](https:/
+00003d90: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00003da0: 3330 392e 3038 3636 3029 2028 3230 3233  309.08660) (2023
+00003db0: 2c20 7375 626d 6974 7465 6429 0a2d 205b  , submitted).- [
+00003dc0: 5472 616e 7366 6572 206c 6561 726e 696e  Transfer learnin
+00003dd0: 6720 666f 7220 6761 6c61 7879 2066 6561  g for galaxy fea
+00003de0: 7475 7265 2064 6574 6563 7469 6f6e 3a20  ture detection: 
+00003df0: 4669 6e64 696e 6720 4769 616e 7420 5374  Finding Giant St
+00003e00: 6172 2d66 6f72 6d69 6e67 2043 6c75 6d70  ar-forming Clump
+00003e10: 7320 696e 206c 6f77 2072 6564 7368 6966  s in low redshif
+00003e20: 7420 6761 6c61 7869 6573 2075 7369 6e67  t galaxies using
+00003e30: 2046 6173 7465 7220 522d 434e 4e5d 2868   Faster R-CNN](h
+00003e40: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00003e50: 2f61 6273 2f32 3331 322e 3033 3530 3329  /abs/2312.03503)
+00003e60: 2028 3230 3233 290a 2d20 5b45 7563 6c69   (2023).- [Eucli
+00003e70: 6420 7072 6570 6172 6174 696f 6e2e 204d  d preparation. M
+00003e80: 6561 7375 7269 6e67 2064 6574 6169 6c65  easuring detaile
+00003e90: 6420 6761 6c61 7879 206d 6f72 7068 6f6c  d galaxy morphol
+00003ea0: 6f67 6965 7320 666f 7220 4575 636c 6964  ogies for Euclid
+00003eb0: 2077 6974 6820 4d61 6368 696e 6520 4c65   with Machine Le
+00003ec0: 6172 6e69 6e67 5d28 6874 7470 733a 2f2f  arning](https://
+00003ed0: 6172 7869 762e 6f72 672f 6162 732f 3234  arxiv.org/abs/24
+00003ee0: 3032 2e31 3031 3837 2920 2832 3032 342c  02.10187) (2024,
+00003ef0: 2073 7562 6d69 7474 6564 290a 0a4d 616e   submitted)..Man
+00003f00: 7920 6f74 6865 7220 776f 726b 7320 7573  y other works us
+00003f10: 6520 5a6f 6f62 6f74 2069 6e64 6972 6563  e Zoobot indirec
+00003f20: 746c 7920 7669 6120 7468 6520 5b47 616c  tly via the [Gal
+00003f30: 6178 7920 5a6f 6f20 4445 4361 4c53 5d28  axy Zoo DECaLS](
+00003f40: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00003f50: 672f 6162 732f 3231 3032 2e30 3834 3134  g/abs/2102.08414
+00003f60: 2920 6361 7461 6c6f 6720 2861 6e64 206e  ) catalog (and n
+00003f70: 6f77 2076 6961 2074 6865 206e 6577 205b  ow via the new [
+00003f80: 4761 6c61 7879 205a 6f6f 2044 4553 495d  Galaxy Zoo DESI]
+00003f90: 2868 7474 7073 3a2f 2f61 6361 6465 6d69  (https://academi
+00003fa0: 632e 6f75 702e 636f 6d2f 6d6e 7261 732f  c.oup.com/mnras/
+00003fb0: 6164 7661 6e63 652d 6172 7469 636c 652f  advance-article/
+00003fc0: 646f 692f 3130 2e31 3039 332f 6d6e 7261  doi/10.1093/mnra
+00003fd0: 732f 7374 6164 3239 3139 2f37 3238 3331  s/stad2919/72831
+00003fe0: 3639 3f6c 6f67 696e 3d66 616c 7365 2920  69?login=false) 
+00003ff0: 6361 7461 6c6f 6729 2e0a                 catalog)..
```

### Comparing `zoobot-1.0.5/zoobot.egg-info/SOURCES.txt` & `zoobot-2.0.0/zoobot.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
+tests/test_from_hub.py
 tests/test_loss_equivalence.py
 zoobot/__init__.py
 zoobot.egg-info/PKG-INFO
 zoobot.egg-info/SOURCES.txt
 zoobot.egg-info/dependency_links.txt
 zoobot.egg-info/requires.txt
 zoobot.egg-info/top_level.txt
 zoobot/pytorch/__init__.py
 zoobot/pytorch/manchester.py
+zoobot/pytorch/datasets/__init__.py
+zoobot/pytorch/datasets/webdatamodule.py
+zoobot/pytorch/datasets/webdataset_utils.py
 zoobot/pytorch/estimators/__init__.py
 zoobot/pytorch/estimators/cuda_check.py
 zoobot/pytorch/estimators/custom_layers.py
 zoobot/pytorch/estimators/define_model.py
 zoobot/pytorch/estimators/efficientnet_custom.py
 zoobot/pytorch/predictions/__init__.py
 zoobot/pytorch/predictions/predict_on_catalog.py
 zoobot/pytorch/training/__init__.py
 zoobot/pytorch/training/finetune.py
 zoobot/pytorch/training/losses.py
 zoobot/pytorch/training/representations.py
+zoobot/pytorch/training/schedulers.py
 zoobot/pytorch/training/tensorboard_writers.py
 zoobot/pytorch/training/train_with_pytorch_lightning.py
 zoobot/shared/__init__.py
 zoobot/shared/benchmark_datasets.py
 zoobot/shared/compress_representations.py
 zoobot/shared/label_metadata.py
 zoobot/shared/load_predictions.py
```

### Comparing `zoobot-1.0.5/zoobot.egg-info/requires.txt` & `zoobot-2.0.0/zoobot.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -5,59 +5,73 @@
 pandas
 scipy
 astropy
 scikit-learn>=1.0.2
 matplotlib
 pyarrow
 wandb
+webdataset
+huggingface_hub
 setuptools
-galaxy-datasets>=0.0.15
+galaxy-datasets>=0.0.17
 
 [docs]
 Sphinx
 sphinxcontrib-napoleon
 furo
 docutils<0.18
+sphinxemoji
 
-[pytorch_colab]
-pytorch-lightning>=2.0.0
+[pytorch-colab]
+lightning>=2.0.0
 albumentations
 pyro-ppl>=1.8.0
 torchmetrics==0.11.0
-timm==0.6.12
+timm>=0.9.10
+galaxy_datasets==0.0.17
 
-[pytorch_cpu]
-torch==1.12.1+cpu
-torchvision==0.13.1+cpu
-torchaudio==0.12.1
-pytorch-lightning>=2.0.0
+[pytorch-cpu]
+torch==2.1.0+cpu
+torchvision==0.16.0+cpu
+torchaudio>=2.1.0
+lightning>=2.0.0
 albumentations
-pyro-ppl==1.8.0
+pyro-ppl>=1.8.6
 torchmetrics==0.11.0
-timm==0.6.12
+timm==0.9.10
 
-[pytorch_cu113]
-torch==1.12.1+cu113
-torchvision==0.13.1+cu113
-torchaudio==0.12.1
-pytorch-lightning>=2.0.0
+[pytorch-cu118]
+torch==2.1.0+cu118
+torchvision==0.16.0+cu118
+torchaudio>=2.1.0
+lightning>=2.0.0
 albumentations
-pyro-ppl==1.8.0
+pyro-ppl>=1.8.6
 torchmetrics==0.11.0
-timm==0.6.12
+timm>=0.9.10
 
-[pytorch_m1]
-torch==1.12.1
-torchvision==0.13.1
-torchaudio==0.12.1
-pytorch-lightning>=2.0.0
+[pytorch-cu121]
+torch==2.1.0+cu121
+torchvision==0.16.0+cu121
+torchaudio>=2.1.0
+lightning>=2.0.0
 albumentations
-pyro-ppl==1.8.0
+pyro-ppl>=1.8.6
 torchmetrics==0.11.0
-timm==0.6.12
+timm>=0.9.10
+
+[pytorch-m1]
+torch==2.1.0
+torchvision==0.16.0
+torchaudio>=2.1.0
+lightning>=2.0.0
+albumentations
+pyro-ppl>=1.8.6
+torchmetrics==0.11.0
+timm>=0.9.10
 
 [tensorflow]
 tensorflow==2.10.0
 keras_applications
 tensorflow_probability==0.18.0
 protobuf<=3.19
```

