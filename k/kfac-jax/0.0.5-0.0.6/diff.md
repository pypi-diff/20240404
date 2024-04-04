# Comparing `tmp/kfac-jax-0.0.5.tar.gz` & `tmp/kfac-jax-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfac-jax-0.0.5.tar", last modified: Tue May 16 18:04:01 2023, max compression
+gzip compressed data, was "kfac-jax-0.0.6.tar", last modified: Thu Apr  4 10:59:12 2024, max compression
```

## Comparing `kfac-jax-0.0.5.tar` & `kfac-jax-0.0.6.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/docs/ext/coverage_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/autoencoder_mnist/
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/autoencoder_mnist/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/autoencoder_mnist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/classifier_mnist/
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/classifier_mnist/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/classifier_mnist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/lrelunet101_imagenet/
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/lrelunet101_imagenet/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/lrelunet101_imagenet/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/resnet50_imagenet/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/resnet50_imagenet/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/resnet50_imagenet/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/kfac_jax/
--rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/kfac_jax/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65212 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/curvature_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    59298 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/curvature_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/layers_and_loss_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    48018 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    57327 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/patches_second_moment.py
--rw-r--r--   0 runner    (1001) docker     (123)    58900 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/tag_graph_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    37478 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/kfac_jax/_src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/accumulators.py
--rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/kfac_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/requirements_examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.540849 kfac-jax-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-04 10:59:12.540849 kfac-jax-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.532849 kfac-jax-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.532849 kfac-jax-0.0.6/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/docs/ext/coverage_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.528849 kfac-jax-0.0.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.532849 kfac-jax-0.0.6/examples/autoencoder_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/examples/autoencoder_mnist/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/examples/autoencoder_mnist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.532849 kfac-jax-0.0.6/examples/classifier_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/examples/classifier_mnist/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/examples/classifier_mnist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.532849 kfac-jax-0.0.6/examples/lrelunet101_imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/examples/lrelunet101_imagenet/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/examples/lrelunet101_imagenet/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.532849 kfac-jax-0.0.6/examples/resnet50_imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/examples/resnet50_imagenet/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/examples/resnet50_imagenet/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.532849 kfac-jax-0.0.6/kfac_jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.536849 kfac-jax-0.0.6/kfac_jax/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68034 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/curvature_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63406 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/curvature_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/layers_and_loss_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52339 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66190 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36908 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/patches_second_moment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59297 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/tag_graph_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38422 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.536849 kfac-jax-0.0.6/kfac_jax/_src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/utils/accumulators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37111 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/_src/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/kfac_jax/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.540849 kfac-jax-0.0.6/kfac_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-04 10:59:12.000000 kfac-jax-0.0.6/kfac_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-04 10:59:12.000000 kfac-jax-0.0.6/kfac_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:59:12.000000 kfac-jax-0.0.6/kfac_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:59:12.000000 kfac-jax-0.0.6/kfac_jax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-04 10:59:12.000000 kfac-jax-0.0.6/kfac_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 10:59:12.000000 kfac-jax-0.0.6/kfac_jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/requirements_examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:59:12.540849 kfac-jax-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:59:12.536849 kfac-jax-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23102 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/tests/test_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/tests/test_graph_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/tests/test_patches_second_moment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-04-04 10:59:01.000000 kfac-jax-0.0.6/tests/test_tracer.py
```

### Comparing `kfac-jax-0.0.5/LICENSE` & `kfac-jax-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.5/PKG-INFO` & `kfac-jax-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,35 @@
-Metadata-Version: 2.1
-Name: kfac-jax
-Version: 0.0.5
-Summary: A Jax package for approximate curvature estimation and optimization using KFAC.
-Home-page: https://github.com/deepmind/kfac-jax
-Author: DeepMind
-Author-email: kfac-jax-dev@google.com
-License: Apache 2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
 # KFAC-JAX - Second Order Optimization with Approximate Curvature in JAX
 
 [**Installation**](#installation)
 | [**Quickstart**](#quickstart)
 | [**Documentation**](https://kfac-jax.readthedocs.io/)
-| [**Examples**](https://github.com/deepmind/kfac-jax/tree/main/examples/)
+| [**Examples**](https://github.com/google-deepmind/kfac-jax/tree/main/examples/)
 | [**Citing KFAC-JAX**](#citing-kfac-jax)
 
-![CI status](https://github.com/deepmind/kfac-jax/workflows/ci/badge.svg)
+![CI status](https://github.com/google-deepmind/kfac-jax/workflows/ci/badge.svg)
 ![docs](https://readthedocs.org/projects/kfac-jax/badge/?version=latest)
 ![pypi](https://img.shields.io/pypi/v/kfac-jax)
 
-KFAC-JAX is a library built on top of [JAX] for second-order optimization of 
+KFAC-JAX is a library built on top of [JAX] for second-order optimization of
 neural networks and for computing scalable curvature approximations.
-The main goal of the library is to provide researchers with an easy-to-use 
+The main goal of the library is to provide researchers with an easy-to-use
 implementation of the [K-FAC] optimizer and curvature estimator.
 
 ## Installation<a id="installation"></a>
 
 KFAC-JAX is written in pure Python, but depends on C++ code via JAX.
 
 First, follow [these instructions](https://github.com/google/jax#installation)
 to install JAX with the relevant accelerator support.
 
 Then, install KFAC-JAX using pip:
 
 ```bash
-$ pip install git+https://github.com/deepmind/kfac-jax
+$ pip install git+https://github.com/google-deepmind/kfac-jax
 ```
 
 Alternatively, you can install via PyPI:
 
 ```bash
 $ pip install -U kfac-jax
 ```
@@ -62,15 +38,15 @@
 
 ```bash
 $ pip install -r requirements_examples.txt
 ```
 
 ## Quickstart<a id="quickstart"></a>
 
-Let's take a look at a simple example of training a neural network, defined 
+Let's take a look at a simple example of training a neural network, defined
 using [Haiku], with the K-FAC optimizer:
 
 ```python
 import haiku as hk
 import jax
 import jax.numpy as jnp
 import kfac_jax
@@ -80,22 +56,22 @@
 L2_REG = 1e-3
 NUM_BATCHES = 100
 
 
 def make_dataset_iterator(batch_size):
   # Dummy dataset, in practice this should be your dataset pipeline
   for _ in range(NUM_BATCHES):
-    yield jnp.zeros([batch_size, 100]), jnp.ones([batch_size], dtype="int32") 
+    yield jnp.zeros([batch_size, 100]), jnp.ones([batch_size], dtype="int32")
 
 
 def softmax_cross_entropy(logits: jnp.ndarray, targets: jnp.ndarray):
   """Softmax cross entropy loss."""
   # We assume integer labels
   assert logits.ndim == targets.ndim + 1
-  
+
   # Tell KFAC-JAX this model represents a classifier
   # See https://kfac-jax.readthedocs.io/en/latest/overview.html#supported-losses
   kfac_jax.register_softmax_cross_entropy_loss(logits, targets)
   log_p = jax.nn.log_softmax(logits, axis=-1)
   return - jax.vmap(lambda x, y: x[y])(log_p, targets)
 
 
@@ -113,15 +89,15 @@
 
 
 def loss_fn(model_params, model_batch):
   """The loss function to optimize."""
   x, y = model_batch
   logits = hk_model.apply(model_params, x)
   loss = jnp.mean(softmax_cross_entropy(logits, y))
-  
+
   # The optimizer assumes that the function you provide has already added
   # the L2 regularizer to its gradients.
   return loss + L2_REG * kfac_jax.utils.inner_product(params, params) / 2.0
 
 
 # Create the optimizer
 optimizer = kfac_jax.Optimizer(
@@ -155,55 +131,55 @@
 
 ### Do not stage (``jit`` or ``pmap``) the optimizer
 
 You should not apply `jax.jit` or `jax.pmap` to the call to `Optimizer.step`.
 This is already done for you automatically by the optimizer class.
 To control the staging behaviour of the optimizer set the flag ``multi_device``
 to ``True`` for ``pmap`` and to ``False`` for ``jit``.
- 
+
 ### Do not stage (``jit`` or ``pmap``) the loss function
 
-The ``value_and_grad_func`` argument provided to the optimizer should compute 
-the loss function value and its gradients. Since the optimizer already stages 
+The ``value_and_grad_func`` argument provided to the optimizer should compute
+the loss function value and its gradients. Since the optimizer already stages
 its step function internally, applying ``jax.jit`` to ``value_and_grad_func`` is
 **NOT** recommended.
 Importantly, applying ``jax.pmap`` is **WRONG** and most likely will lead to
 errors.
 
 ### Registering the model loss function
 
 In order for KFAC-JAX to be able to correctly approximate the curvature matrix
 of the model it needs to know the precise loss function that you want to
-optimize. 
+optimize.
 This is done via registration with certain functions provided by the library.
-For instance, in the example above this is done via the call to 
-``kfac_jax.register_softmax_cross_entropy_loss``, which tells the optimizer that 
+For instance, in the example above this is done via the call to
+``kfac_jax.register_softmax_cross_entropy_loss``, which tells the optimizer that
 the loss is the standard softmax cross-entropy.
-If you don't do this you will get an error when you try to call the optimizer. 
+If you don't do this you will get an error when you try to call the optimizer.
 For all supported loss functions please read the [documentation].
 
-``Important:`` The optimizer assumes that the loss is averaged over examples in 
+``Important:`` The optimizer assumes that the loss is averaged over examples in
 the minibatch. It is crucial that you follow this convention.
 
 ### Other model function options
 
-Oftentimes, one will want to output some auxiliary statistics or metrics in 
+Oftentimes, one will want to output some auxiliary statistics or metrics in
 addition to the loss value.
 This can already be done in the ``value_and_grad_func``, in which case we follow
-the same conventions as JAX and expect the output to be ``(loss, aux), grads``. 
-Similarly, the loss function can take an additional function state (batch norm 
+the same conventions as JAX and expect the output to be ``(loss, aux), grads``.
+Similarly, the loss function can take an additional function state (batch norm
 layers usually have this) or an PRNG key (used in stochastic layers). All of
 these, however, need to be explicitly told to the optimizer via its arguments
 ``value_func_has_aux``, ``value_func_has_state`` and ``value_func_has_rng``.
 
 ### Verify optimizer registrations
 
-We strongly encourage the user to pay attention to the logging messages produced 
-by the automatic registration system, in order to ensure that it has correctly 
-understood your model. 
+We strongly encourage the user to pay attention to the logging messages produced
+by the automatic registration system, in order to ensure that it has correctly
+understood your model.
 For the example above this looks like this:
 
 ```python
 ==================================================
 Graph parameter registrations:
 {'mlp/~/linear_0': {'b': 'Auto[dense_with_bias_3]',
                     'w': 'Auto[dense_with_bias_3]'},
@@ -216,33 +192,33 @@
 ==================================================
 ```
 
 As can be seen from this message, the library has correctly detected all
 parameters of the model to be part of dense layers.
 
 ### Further reading
-For a high level overview of the optimizer, the different curvature 
+For a high level overview of the optimizer, the different curvature
 approximations, and the supported layers, please see the [documentation].
 
 ## Citing KFAC-JAX<a id="citing-kfac-jax"></a>
 
 To cite this repository:
 
 ```
 @software{kfac-jax2022github,
   author = {Aleksandar Botev and James Martens},
   title = {{KFAC-JAX}},
-  url = {http://github.com/deepmind/kfac-jax},
+  url = {https://github.com/google-deepmind/kfac-jax},
   version = {0.0.2},
   year = {2022},
 }
 ```
 
 In this bibtex entry, the version number is intended to be from
-[`kfac_jax/__init__.py`](https://github.com/deepmind/kfac-jax/blob/main/kfac_jax/__init__.py),
+[`kfac_jax/__init__.py`](https://github.com/google-deepmind/kfac-jax/blob/main/kfac_jax/__init__.py),
 and the year corresponds to the project's open-source release.
 
 
 [K-FAC]: https://arxiv.org/abs/1503.05671
 [JAX]: https://github.com/google/jax
-[Haiku]: https://github.com/deepmind/dm-haiku
+[Haiku]: https://github.com/google-deepmind/dm-haiku
 [documentation]: https://kfac-jax.readthedocs.io/
```

### Comparing `kfac-jax-0.0.5/README.md` & `kfac-jax-0.0.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,78 @@
+Metadata-Version: 2.1
+Name: kfac-jax
+Version: 0.0.6
+Summary: A Jax package for approximate curvature estimation and optimization using KFAC.
+Home-page: https://github.com/google-deepmind/kfac-jax
+Author: DeepMind
+Author-email: kfac-jax-dev@google.com
+License: Apache 2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: absl-py>=0.12.0
+Requires-Dist: immutabledict>=2.2.1
+Requires-Dist: numpy>=1.21
+Requires-Dist: distrax>=0.1.3
+Requires-Dist: jax>=0.4.7
+Requires-Dist: jaxlib>=0.4.7
+Requires-Dist: dm-tree>=0.1.7
+Requires-Dist: optax>=0.1.4
+Requires-Dist: typing_extensions>=4.2.0; python_version < "3.10"
+Provides-Extra: tests
+Requires-Dist: pytest-xdist; extra == "tests"
+Requires-Dist: absl-py==0.12.0; extra == "tests"
+Requires-Dist: immutabledict==2.2.1; extra == "tests"
+Requires-Dist: numpy==1.21; extra == "tests"
+Requires-Dist: distrax==0.1.3; extra == "tests"
+Requires-Dist: jax==0.4.7; extra == "tests"
+Requires-Dist: jaxlib==0.4.7; extra == "tests"
+Requires-Dist: dm-haiku==0.0.9; extra == "tests"
+Requires-Dist: dm-tree==0.1.7; extra == "tests"
+Requires-Dist: optax==0.1.4; extra == "tests"
+
 # KFAC-JAX - Second Order Optimization with Approximate Curvature in JAX
 
 [**Installation**](#installation)
 | [**Quickstart**](#quickstart)
 | [**Documentation**](https://kfac-jax.readthedocs.io/)
-| [**Examples**](https://github.com/deepmind/kfac-jax/tree/main/examples/)
+| [**Examples**](https://github.com/google-deepmind/kfac-jax/tree/main/examples/)
 | [**Citing KFAC-JAX**](#citing-kfac-jax)
 
-![CI status](https://github.com/deepmind/kfac-jax/workflows/ci/badge.svg)
+![CI status](https://github.com/google-deepmind/kfac-jax/workflows/ci/badge.svg)
 ![docs](https://readthedocs.org/projects/kfac-jax/badge/?version=latest)
 ![pypi](https://img.shields.io/pypi/v/kfac-jax)
 
-KFAC-JAX is a library built on top of [JAX] for second-order optimization of 
+KFAC-JAX is a library built on top of [JAX] for second-order optimization of
 neural networks and for computing scalable curvature approximations.
-The main goal of the library is to provide researchers with an easy-to-use 
+The main goal of the library is to provide researchers with an easy-to-use
 implementation of the [K-FAC] optimizer and curvature estimator.
 
 ## Installation<a id="installation"></a>
 
 KFAC-JAX is written in pure Python, but depends on C++ code via JAX.
 
 First, follow [these instructions](https://github.com/google/jax#installation)
 to install JAX with the relevant accelerator support.
 
 Then, install KFAC-JAX using pip:
 
 ```bash
-$ pip install git+https://github.com/deepmind/kfac-jax
+$ pip install git+https://github.com/google-deepmind/kfac-jax
 ```
 
 Alternatively, you can install via PyPI:
 
 ```bash
 $ pip install -U kfac-jax
 ```
@@ -38,15 +81,15 @@
 
 ```bash
 $ pip install -r requirements_examples.txt
 ```
 
 ## Quickstart<a id="quickstart"></a>
 
-Let's take a look at a simple example of training a neural network, defined 
+Let's take a look at a simple example of training a neural network, defined
 using [Haiku], with the K-FAC optimizer:
 
 ```python
 import haiku as hk
 import jax
 import jax.numpy as jnp
 import kfac_jax
@@ -56,22 +99,22 @@
 L2_REG = 1e-3
 NUM_BATCHES = 100
 
 
 def make_dataset_iterator(batch_size):
   # Dummy dataset, in practice this should be your dataset pipeline
   for _ in range(NUM_BATCHES):
-    yield jnp.zeros([batch_size, 100]), jnp.ones([batch_size], dtype="int32") 
+    yield jnp.zeros([batch_size, 100]), jnp.ones([batch_size], dtype="int32")
 
 
 def softmax_cross_entropy(logits: jnp.ndarray, targets: jnp.ndarray):
   """Softmax cross entropy loss."""
   # We assume integer labels
   assert logits.ndim == targets.ndim + 1
-  
+
   # Tell KFAC-JAX this model represents a classifier
   # See https://kfac-jax.readthedocs.io/en/latest/overview.html#supported-losses
   kfac_jax.register_softmax_cross_entropy_loss(logits, targets)
   log_p = jax.nn.log_softmax(logits, axis=-1)
   return - jax.vmap(lambda x, y: x[y])(log_p, targets)
 
 
@@ -89,15 +132,15 @@
 
 
 def loss_fn(model_params, model_batch):
   """The loss function to optimize."""
   x, y = model_batch
   logits = hk_model.apply(model_params, x)
   loss = jnp.mean(softmax_cross_entropy(logits, y))
-  
+
   # The optimizer assumes that the function you provide has already added
   # the L2 regularizer to its gradients.
   return loss + L2_REG * kfac_jax.utils.inner_product(params, params) / 2.0
 
 
 # Create the optimizer
 optimizer = kfac_jax.Optimizer(
@@ -131,55 +174,55 @@
 
 ### Do not stage (``jit`` or ``pmap``) the optimizer
 
 You should not apply `jax.jit` or `jax.pmap` to the call to `Optimizer.step`.
 This is already done for you automatically by the optimizer class.
 To control the staging behaviour of the optimizer set the flag ``multi_device``
 to ``True`` for ``pmap`` and to ``False`` for ``jit``.
- 
+
 ### Do not stage (``jit`` or ``pmap``) the loss function
 
-The ``value_and_grad_func`` argument provided to the optimizer should compute 
-the loss function value and its gradients. Since the optimizer already stages 
+The ``value_and_grad_func`` argument provided to the optimizer should compute
+the loss function value and its gradients. Since the optimizer already stages
 its step function internally, applying ``jax.jit`` to ``value_and_grad_func`` is
 **NOT** recommended.
 Importantly, applying ``jax.pmap`` is **WRONG** and most likely will lead to
 errors.
 
 ### Registering the model loss function
 
 In order for KFAC-JAX to be able to correctly approximate the curvature matrix
 of the model it needs to know the precise loss function that you want to
-optimize. 
+optimize.
 This is done via registration with certain functions provided by the library.
-For instance, in the example above this is done via the call to 
-``kfac_jax.register_softmax_cross_entropy_loss``, which tells the optimizer that 
+For instance, in the example above this is done via the call to
+``kfac_jax.register_softmax_cross_entropy_loss``, which tells the optimizer that
 the loss is the standard softmax cross-entropy.
-If you don't do this you will get an error when you try to call the optimizer. 
+If you don't do this you will get an error when you try to call the optimizer.
 For all supported loss functions please read the [documentation].
 
-``Important:`` The optimizer assumes that the loss is averaged over examples in 
+``Important:`` The optimizer assumes that the loss is averaged over examples in
 the minibatch. It is crucial that you follow this convention.
 
 ### Other model function options
 
-Oftentimes, one will want to output some auxiliary statistics or metrics in 
+Oftentimes, one will want to output some auxiliary statistics or metrics in
 addition to the loss value.
 This can already be done in the ``value_and_grad_func``, in which case we follow
-the same conventions as JAX and expect the output to be ``(loss, aux), grads``. 
-Similarly, the loss function can take an additional function state (batch norm 
+the same conventions as JAX and expect the output to be ``(loss, aux), grads``.
+Similarly, the loss function can take an additional function state (batch norm
 layers usually have this) or an PRNG key (used in stochastic layers). All of
 these, however, need to be explicitly told to the optimizer via its arguments
 ``value_func_has_aux``, ``value_func_has_state`` and ``value_func_has_rng``.
 
 ### Verify optimizer registrations
 
-We strongly encourage the user to pay attention to the logging messages produced 
-by the automatic registration system, in order to ensure that it has correctly 
-understood your model. 
+We strongly encourage the user to pay attention to the logging messages produced
+by the automatic registration system, in order to ensure that it has correctly
+understood your model.
 For the example above this looks like this:
 
 ```python
 ==================================================
 Graph parameter registrations:
 {'mlp/~/linear_0': {'b': 'Auto[dense_with_bias_3]',
                     'w': 'Auto[dense_with_bias_3]'},
@@ -192,33 +235,33 @@
 ==================================================
 ```
 
 As can be seen from this message, the library has correctly detected all
 parameters of the model to be part of dense layers.
 
 ### Further reading
-For a high level overview of the optimizer, the different curvature 
+For a high level overview of the optimizer, the different curvature
 approximations, and the supported layers, please see the [documentation].
 
 ## Citing KFAC-JAX<a id="citing-kfac-jax"></a>
 
 To cite this repository:
 
 ```
 @software{kfac-jax2022github,
   author = {Aleksandar Botev and James Martens},
   title = {{KFAC-JAX}},
-  url = {http://github.com/deepmind/kfac-jax},
+  url = {https://github.com/google-deepmind/kfac-jax},
   version = {0.0.2},
   year = {2022},
 }
 ```
 
 In this bibtex entry, the version number is intended to be from
-[`kfac_jax/__init__.py`](https://github.com/deepmind/kfac-jax/blob/main/kfac_jax/__init__.py),
+[`kfac_jax/__init__.py`](https://github.com/google-deepmind/kfac-jax/blob/main/kfac_jax/__init__.py),
 and the year corresponds to the project's open-source release.
 
 
 [K-FAC]: https://arxiv.org/abs/1503.05671
 [JAX]: https://github.com/google/jax
-[Haiku]: https://github.com/deepmind/dm-haiku
+[Haiku]: https://github.com/google-deepmind/dm-haiku
 [documentation]: https://kfac-jax.readthedocs.io/
```

### Comparing `kfac-jax-0.0.5/docs/conf.py` & `kfac-jax-0.0.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,16 @@
     'sphinxcontrib.katex',
     'sphinx_autodoc_typehints',
     'sphinx_rtd_theme',
     'coverage_check',
     'myst_nb',  # This is used for the .ipynb notebooks
 ]
 
+bibtex_bibfiles = []
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
@@ -177,18 +179,19 @@
   except TypeError:
     return None
 
   try:
     source, lineno = inspect.getsourcelines(obj)
   except OSError:
     return None
-
-  return 'https://github.com/deepmind/kfac-jax/tree/master/kfac_jax/%s#L%d#L%d' % (
+  prefix = 'https://github.com/google-deepmind/kfac-jax/tree/master/kfac_jax/'
+  version = '%s#L%d#L%d' % (
       os.path.relpath(filename, start=os.path.dirname(
           kfac_jax.__file__)), lineno, lineno + len(source) - 1)
+  return prefix + version
 
 
 # -- Intersphinx configuration -----------------------------------------------
 
 intersphinx_mapping = {
     'jax': ('https://jax.readthedocs.io/en/latest/', None),
 }
```

### Comparing `kfac-jax-0.0.5/docs/ext/coverage_check.py` & `kfac-jax-0.0.6/docs/ext/coverage_check.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.5/examples/autoencoder_mnist/experiment.py` & `kfac-jax-0.0.6/examples/autoencoder_mnist/experiment.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.5/examples/autoencoder_mnist/pipeline.py` & `kfac-jax-0.0.6/examples/autoencoder_mnist/pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,29 +45,32 @@
               l2_reg=1e-5,
               training=dict(
                   steps=5_000,
                   epochs=None,
               ),
               batch_size=dict(
                   train=dict(
-                      total=60_000,
+                      total=60_000,  # the entire dataset
                       per_device=-1,
                   ),
                   eval=dict(
                       total=10_000,
                       per_device=-1,
                   ),
               ),
               optimizer=dict(
                   name="kfac",
                   kfac=dict(
                       inverse_update_period=5,
                       damping_adaptation_interval=5,
                       num_burnin_steps=5,
                       curvature_ema=0.95,
+                      # As mentioned in examples/README.md, we do NOT recommend
+                      # using these adaptive options for stochastic
+                      # optimization:
                       use_adaptive_damping=True,
                       use_adaptive_learning_rate=True,
                       use_adaptive_momentum=True,
                       damping_adaptation_decay=0.95,
                       initial_damping=150.0,
                       min_damping=1e-5,
                       max_damping=1000.0,
```

### Comparing `kfac-jax-0.0.5/examples/classifier_mnist/experiment.py` & `kfac-jax-0.0.6/examples/classifier_mnist/experiment.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.5/examples/classifier_mnist/pipeline.py` & `kfac-jax-0.0.6/examples/classifier_mnist/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,29 +45,32 @@
               l2_reg=1e-5,
               training=dict(
                   steps=5_000,
                   epochs=None,
               ),
               batch_size=dict(
                   train=dict(
-                      total=60_000,
+                      total=60_000,  # the entire dataset
                       per_device=-1,
                   ),
                   eval=dict(
                       total=10_000,
                       per_device=-1,
                   ),
               ),
               optimizer=dict(
                   name="kfac",
                   kfac=dict(
                       inverse_update_period=5,
                       damping_adaptation_interval=5,
                       num_burnin_steps=5,
                       curvature_ema=0.95,
+                      # As mentioned in examples/README.md, we do NOT recommend
+                      # using these adaptive options for stochastic
+                      # optimization:
                       use_adaptive_damping=True,
                       use_adaptive_learning_rate=True,
                       use_adaptive_momentum=True,
                       damping_adaptation_decay=0.95,
                       initial_damping=150.0,
                       min_damping=1e-5,
                       max_damping=1000.0,
```

### Comparing `kfac-jax-0.0.5/examples/lrelunet101_imagenet/experiment.py` & `kfac-jax-0.0.6/examples/lrelunet101_imagenet/experiment.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.5/examples/lrelunet101_imagenet/pipeline.py` & `kfac-jax-0.0.6/examples/lrelunet101_imagenet/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                       num_burnin_steps=5,
                       curvature_ema=0.99,
                       norm_constraint=0.001,
                       use_adaptive_learning_rate=False,
                       use_adaptive_momentum=False,
                       use_adaptive_damping=False,
                       learning_rate_schedule=dict(
-                          initial_learning_rate=3e-4,
+                          peak_learning_rate=3e-4,
                           warmup_epochs=5,
                           name="cosine",
                       ),
                       momentum_schedule=dict(
                           name="fixed",
                           value=0.9,
                       ),
@@ -90,15 +90,15 @@
                           value=0.001,
                       ),
                   ),
                   sgd=dict(
                       decay=0.9,
                       nesterov=True,
                       learning_rate_schedule=dict(
-                          initial_learning_rate=0.1,
+                          peak_learning_rate=0.1,
                           warmup_epochs=5,
                           name="cosine",
                       ),
                   ),
               )
           )
       )
```

### Comparing `kfac-jax-0.0.5/examples/resnet50_imagenet/experiment.py` & `kfac-jax-0.0.6/examples/resnet50_imagenet/experiment.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.5/examples/resnet50_imagenet/pipeline.py` & `kfac-jax-0.0.6/examples/resnet50_imagenet/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.5/kfac_jax/__init__.py` & `kfac-jax-0.0.6/kfac_jax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from kfac_jax._src import optimizer
 from kfac_jax._src import patches_second_moment
 from kfac_jax._src import tag_graph_matcher
 from kfac_jax._src import tracer
 from kfac_jax._src import utils
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 # Patches Second Moments
 patches_moments = patches_second_moment.patches_moments
 patches_moments_explicit = patches_second_moment.patches_moments_explicit
 
 # Layers and loss tags
 LossTag = layers_and_loss_tags.LossTag
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/__init__.py` & `kfac-jax-0.0.6/kfac_jax/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/curvature_blocks.py` & `kfac-jax-0.0.6/kfac_jax/_src/curvature_blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 import collections
 import functools
 import string
 from typing import Optional, Sequence, Any, Set, Tuple, Union, Dict, Mapping
 
 import jax
 import jax.numpy as jnp
+import jax.scipy
+
 from kfac_jax._src import layers_and_loss_tags as tags
 from kfac_jax._src import patches_second_moment as psm
 from kfac_jax._src import tag_graph_matcher as tgm
 from kfac_jax._src import utils
 import numpy as np
 
 # Types for annotation
@@ -250,29 +252,35 @@
       state: The state for this block.
       use_cache: Whether the method requesting this is using cached values or
         not.
 
     Returns:
       A scalar value to be multiplied with any unscaled block representation.
     """
+
+    # TODO(jamesmartens,botev): This way of handling state dependent scale is
+    # a bit hacky and leads to complexity in other parts of the code that must
+    # be aware of how this part works. Should try to replace this with something
+    # better.
+
     if use_cache:
       return self.fixed_scale()
 
     return self.fixed_scale() * self.state_dependent_scale(state)
 
   def fixed_scale(self) -> Numeric:
     """A fixed scalar pre-factor of the curvature (e.g. constant)."""
     return 1.0
 
   def state_dependent_scale(self, state: "CurvatureBlock.State") -> Numeric:
     """A scalar pre-factor of the curvature, computed from the most fresh curvature estimate."""
+    del state  # Unused
     return 1.0
 
   def __str__(self):
-
     return f"{self._name!r}[{self.parameters_shapes!r}]"
 
   @utils.auto_scope_method
   def init(
       self,
       rng: PRNGKey,
       exact_powers_to_cache: Optional[ScalarOrSequence],
@@ -314,14 +322,22 @@
       rng: PRNGKey,
       exact_powers_to_cache: Set[Scalar],
       approx_powers_to_cache: Set[Scalar],
       cache_eigenvalues: bool,
   ) -> "CurvatureBlock.State":
     """The non-public interface of ``init``."""
 
+  @abc.abstractmethod
+  def sync(
+      self,
+      state: "CurvatureBlock.State",
+      pmap_axis_name: str,
+  ) -> "CurvatureBlock.State":
+    """Syncs the state across different devices (does not sync the cache)."""
+
   @utils.auto_scope_method
   def multiply_matpower(
       self,
       state: "CurvatureBlock.State",
       vector: Sequence[Array],
       identity_weight: Numeric,
       power: Scalar,
@@ -353,15 +369,17 @@
         to use the most recent curvature estimates. The cached version is
         going to be *at least* as fresh as the value provided to the last call
         to :func:`~CurvatureBlock.update_cache` with the same value of ``power``
 
     Returns:
       A tuple of arrays, representing the result of the matrix-vector product.
     """
+
     scale = self.scale(state, use_cached)
+
     result = self._multiply_matpower_unscaled(
         state=state,
         vector=vector,
         identity_weight=identity_weight / scale,
         power=power,
         exact_power=exact_power,
         use_cached=use_cached,
@@ -455,15 +473,14 @@
   def update_curvature_matrix_estimate(
       self,
       state: "CurvatureBlock.State",
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
-      pmap_axis_name: Optional[str],
   ) -> "CurvatureBlock.State":
     """Updates the block's curvature estimates using the ``info`` provided.
 
     Each block *in general* estimates a moving average of its associated
     curvature matrix. If you don't want a moving average you can set
     ``ema_old=0`` and ``ema_new=1``.
 
@@ -475,16 +492,14 @@
           implementation for more details on the name of the fields and how they
           are constructed.
       ema_old: Specifies the weight of the old value when computing the updated
           estimate in the moving average.
       ema_new: Specifies the weight of the new value when computing the updated
           estimate in the moving average.
       batch_size: The batch size used in computing the values in ``info``.
-      pmap_axis_name: The name of any pmap axis, which might be needed for
-          computing the updates.
     """
 
   @utils.auto_scope_method
   def update_cache(
       self,
       state: "CurvatureBlock.State",
       identity_weight: Numeric,
@@ -532,14 +547,27 @@
     """Returns a dense representation of the approximate curvature matrix."""
     return self.scale(state, False) * self._to_dense_unscaled(state)
 
   @abc.abstractmethod
   def _to_dense_unscaled(self, state: "CurvatureBlock.State") -> Array:
     """A dense representation of the curvature, ignoring ``self.scale``."""
 
+  def norm(self, state: "CurvatureBlock.State", norm_type: str) -> Numeric:
+    """Computes the norm of the curvature block, according to ``norm_type``."""
+
+    return self.scale(state, False) * self._norm_unscaled(state, norm_type)
+
+  @abc.abstractmethod
+  def _norm_unscaled(
+      self,
+      state: "CurvatureBlock.State",
+      norm_type: str
+  ) -> Numeric:
+    """Like ``norm`` but with ``self.scale`` not included."""
+
 
 class ScaledIdentity(CurvatureBlock):
   """A block that assumes that the curvature is a scaled identity matrix."""
 
   def __init__(
       self,
       layer_tag_eq: tags.LayerTagEqn,
@@ -570,27 +598,38 @@
 
     del rng, exact_powers_to_cache, approx_powers_to_cache  # Unused
 
     return CurvatureBlock.State(
         cache=None,
     )
 
+  def sync(
+      self,
+      state: CurvatureBlock.State,
+      pmap_axis_name: str,
+  ) -> CurvatureBlock.State:
+    return state
+
   def _multiply_matpower_unscaled(
       self,
       state: CurvatureBlock.State,
       vector: Sequence[Array],
       identity_weight: Numeric,
       power: Scalar,
       exact_power: bool,
       use_cached: bool,
   ) -> Tuple[Array, ...]:
 
-    del exact_power, use_cached  # Unused
+    del exact_power  # Unused
+
+    # state_dependent_scale needs to be included because it won't be by the
+    # caller of this function (multiply_matpower) when use_cached=True
+    scale = self.state_dependent_scale(state) if use_cached else 1.0
 
-    identity_weight = identity_weight + 1.0
+    identity_weight = identity_weight + scale
 
     if power == 1:
       return jax.tree_util.tree_map(lambda x: identity_weight * x, vector)
 
     elif power == -1:
       return jax.tree_util.tree_map(lambda x: x / identity_weight, vector)
 
@@ -609,15 +648,14 @@
   def update_curvature_matrix_estimate(
       self,
       state: CurvatureBlock.State,
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
-      pmap_axis_name: Optional[str],
   ) -> CurvatureBlock.State:
 
     return state.copy()
 
   def _update_cache(
       self,
       state: CurvatureBlock.State,
@@ -629,14 +667,22 @@
 
     return state.copy()
 
   def _to_dense_unscaled(self, state: CurvatureBlock.State) -> Array:
     del state  # not used
     return jnp.eye(self.dim)
 
+  def _norm_unscaled(
+      self,
+      state: CurvatureBlock.State,
+      norm_type: str
+  ) -> Numeric:
+
+    return utils.psd_matrix_norm(jnp.ones([self.dim]), norm_type=norm_type)
+
 
 class Diagonal(CurvatureBlock, abc.ABC):
   """An abstract class for approximating only the diagonal of curvature."""
 
   @utils.register_state_class
   class State(CurvatureBlock.State):
     """Persistent state of the block.
@@ -656,29 +702,50 @@
       cache_eigenvalues: bool,
   ) -> "Diagonal.State":
 
     del rng
 
     return Diagonal.State(
         cache=None,
-        diagonal_factors=tuple(utils.WeightedMovingAverage.zeros_array(
-            shape, self.dtype) for shape in self.parameters_shapes),
+        diagonal_factors=tuple(
+            utils.WeightedMovingAverage.zeros_array(shape, self.dtype)
+            for shape in self.parameters_shapes
+        ),
     )
 
+  def sync(
+      self,
+      state: "Diagonal.State",
+      pmap_axis_name: str,
+  ) -> "Diagonal.State":
+
+    # Copy this first since we mutate it later in this function.
+    state = state.copy()
+
+    for factor in state.diagonal_factors:
+      factor.sync(pmap_axis_name)
+
+    return state
+
   def _multiply_matpower_unscaled(
       self,
       state: "Diagonal.State",
       vector: Sequence[Array],
       identity_weight: Numeric,
       power: Scalar,
       exact_power: bool,
       use_cached: bool,
   ) -> Tuple[Array, ...]:
 
-    factors = tuple(f.value + identity_weight for f in state.diagonal_factors)
+    # state_dependent_scale needs to be included because it won't be by the
+    # caller of this function (multiply_matpower) when use_cached=True
+    scale = self.state_dependent_scale(state) if use_cached else 1.0
+
+    factors = tuple(scale * f.value + identity_weight
+                    for f in state.diagonal_factors)
 
     assert len(factors) == len(vector)
 
     if power == 1:
       return tuple(f * v for f, v in zip(factors, vector))
     elif power == -1:
       return tuple(v / f for f, v in zip(factors, vector))
@@ -689,64 +756,44 @@
       self,
       state: "Diagonal.State",
       use_cached: bool,
   ) -> Array:
     return jnp.concatenate([f.value.flatten() for f in state.diagonal_factors],
                            axis=0)
 
-  @utils.auto_scope_method
-  def update_curvature_matrix_estimate(
-      self,
-      state: "Diagonal.State",
-      estimation_data: Dict[str, Sequence[Array]],
-      ema_old: Numeric,
-      ema_new: Numeric,
-      batch_size: Numeric,
-      pmap_axis_name: Optional[str],
-  ) -> "Diagonal.State":
-
-    # This function call will return a copy of state:
-    state = self._update_curvature_matrix_estimate(
-        state, estimation_data, ema_old, ema_new, batch_size)
-
-    for factor in state.diagonal_factors:
-      factor.sync(pmap_axis_name)
-
-    return state
-
-  @abc.abstractmethod
-  def _update_curvature_matrix_estimate(
-      self,
-      state: "Diagonal.State",
-      estimation_data: Dict[str, Sequence[Array]],
-      ema_old: Numeric,
-      ema_new: Numeric,
-      batch_size: Numeric,
-  ) -> "Diagonal.State":
-    pass
-
   def _update_cache(
       self,
       state: "Diagonal.State",
       identity_weight: Numeric,
       exact_powers: Set[Scalar],
       approx_powers: Set[Scalar],
       eigenvalues: bool,
   ) -> "Diagonal.State":
+
     return state.copy()
 
   def _to_dense_unscaled(self, state: "Diagonal.State") -> Array:
 
     # Extract factors in canonical order
     factors = [state.diagonal_factors[i].value.flatten()
                for i in self.parameters_canonical_order]
 
     # Construct diagonal matrix
     return jnp.diag(jnp.concatenate(factors, axis=0))
 
+  def _norm_unscaled(
+      self,
+      state: CurvatureBlock.State,
+      norm_type: str
+  ) -> Numeric:
+
+    return utils.product(
+        utils.psd_matrix_norm(f.value.flatten(), norm_type=norm_type)
+        for f in state.diagonal_factors)
+
 
 class Full(CurvatureBlock, abc.ABC):
   """An abstract class for approximating the block matrix with a full matrix."""
 
   @utils.register_state_class
   class State(CurvatureBlock.State):
     """Persistent state of the block.
@@ -776,30 +823,33 @@
        any matrix power). If this is ``None`` will use the value returned from
        :func:`~get_default_eigen_decomposition_threshold()`.
     """
 
     if eigen_decomposition_threshold is None:
       threshold = get_default_eigen_decomposition_threshold()
       self._eigen_decomposition_threshold = threshold
+
     else:
       self._eigen_decomposition_threshold = eigen_decomposition_threshold
 
     super().__init__(layer_tag_eq, name)
 
   def parameters_list_to_single_vector(
       self,
       parameters_shaped_list: Sequence[Array],
   ) -> Array:
     """Converts values corresponding to parameters of the block to vector."""
 
     if len(parameters_shaped_list) != self.number_of_parameters:
+
       raise ValueError(f"Expected a list of {self.number_of_parameters} values,"
                        f" but got {len(parameters_shaped_list)} instead.")
 
     for array, shape in zip(parameters_shaped_list, self.parameters_shapes):
+
       if array.shape != shape:
         raise ValueError(f"Expected a value of shape {shape}, but got "
                          f"{array.shape} instead.")
 
     return jnp.concatenate([v.flatten() for v in parameters_shaped_list])
 
   def single_vector_to_parameters_list(
@@ -815,14 +865,15 @@
       raise ValueError(f"Expected a vector of size {self.dim}, but got "
                        f"{vector.size} instead.")
 
     parameters_shaped_list = []
     index = 0
 
     for shape in self.parameters_shapes:
+
       size = utils.product(shape)
       parameters_shaped_list.append(vector[index: index + size].reshape(shape))
       index += size
 
     assert index == self.dim
 
     return tuple(parameters_shaped_list)
@@ -854,37 +905,61 @@
 
     return Full.State(
         cache=cache,
         matrix=utils.WeightedMovingAverage.zeros_array(
             [self.dim, self.dim], self.dtype),
     )
 
+  def sync(
+      self,
+      state: "Full.State",
+      pmap_axis_name: str,
+  ) -> "Full.State":
+
+    # Copy this first since we mutate it later in this function.
+    state = state.copy()
+
+    state.matrix.sync(pmap_axis_name)
+
+    return state
+
   def _multiply_matpower_unscaled(
       self,
       state: "Full.State",
       vector: Sequence[Array],
       identity_weight: Numeric,
       power: Scalar,
       exact_power: bool,
       use_cached: bool,
   ) -> Tuple[Array, ...]:
 
     vector = self.parameters_list_to_single_vector(vector)
 
     if power == 1:
 
-      result = jnp.matmul(state.matrix.value, vector) + identity_weight * vector
+      result = jnp.matmul(state.matrix.value, vector)
+
+      if use_cached:
+        # state_dependent_scale needs to be included here because it won't be by
+        # the caller of this function (multiply_matpower) when use_cached=True.
+        # This is not an issue for other powers because they bake in
+        # state_dependent_scale.
+        result *= self.state_dependent_scale(state)
+
+      result += identity_weight * vector
 
     elif not use_cached:
 
       matrix = state.matrix.value + identity_weight * jnp.eye(self.dim)
 
       if power == -1:
-        result = jnp.linalg.solve(matrix, vector)
+        result = utils.psd_solve(matrix, vector)
       else:
+        # TODO(jamesmartens,botev): investigate this for determinism on GPUs
+        # NOTE: this function only works for integer powers
         result = jnp.matmul(jnp.linalg.matrix_power(matrix, power), vector)
 
     else:
 
       if str(power) in state.cache:
         result = jnp.matmul(state.cache[str(power)], vector)
 
@@ -899,49 +974,21 @@
     return self.single_vector_to_parameters_list(result)
 
   def _eigenvalues_unscaled(
       self,
       state: "Full.State",
       use_cached: bool,
   ) -> Array:
+
     if not use_cached:
       return utils.safe_psd_eigh(state.matrix.value)[0]
+
     else:
       return state.cache["eigenvalues"]
 
-  @utils.auto_scope_method
-  def update_curvature_matrix_estimate(
-      self,
-      state: "Full.State",
-      estimation_data: Dict[str, Sequence[Array]],
-      ema_old: Numeric,
-      ema_new: Numeric,
-      batch_size: Numeric,
-      pmap_axis_name: Optional[str],
-  ) -> "Full.State":
-
-    # This function call will return a copy of state:
-    state = self._update_curvature_matrix_estimate(
-        state, estimation_data, ema_old, ema_new, batch_size)
-
-    state.matrix.sync(pmap_axis_name)
-
-    return state
-
-  @abc.abstractmethod
-  def _update_curvature_matrix_estimate(
-      self,
-      state: "Full.State",
-      estimation_data: Dict[str, Sequence[Array]],
-      ema_old: Numeric,
-      ema_new: Numeric,
-      batch_size: Numeric,
-  ) -> "Full.State":
-    pass
-
   def _update_cache(
       self,
       state: "Full.State",
       identity_weight: Numeric,
       exact_powers: Set[Scalar],
       approx_powers: Set[Scalar],
       eigenvalues: bool,
@@ -965,31 +1012,40 @@
       if eigenvalues:
         state.cache["eigenvalues"] = scale * utils.safe_psd_eigh(
             state.matrix.value)[0]
 
       for power in exact_powers:
 
         if power == -1:
-          state.cache[str(power)] = utils.psd_inv_cholesky(
-              state.matrix.value, identity_weight) / scale
+          state.cache[str(power)] = utils.psd_inv(
+              state.matrix.value + identity_weight * jnp.eye(self.dim)) / scale
         else:
           matrix = state.matrix.value + identity_weight * jnp.eye(self.dim)
           state.cache[str(power)] = (
               (scale ** power) * jnp.linalg.matrix_power(matrix, power))
 
     return state
 
   def _to_dense_unscaled(self, state: "Full.State") -> Array:
+
     # Permute the matrix according to the parameters canonical order
     return utils.block_permuted(
         state.matrix.value,
         block_sizes=[utils.product(shape) for shape in self.parameters_shapes],
         block_order=self.parameters_canonical_order
     )
 
+  def _norm_unscaled(
+      self,
+      state: CurvatureBlock.State,
+      norm_type: str
+  ) -> Numeric:
+
+    return utils.psd_matrix_norm(state.matrix.value, norm_type=norm_type)
+
 
 class KroneckerFactored(CurvatureBlock, abc.ABC):
   """An abstract class for approximating the block with a Kronecker product."""
 
   @utils.register_state_class
   class State(CurvatureBlock.State):
     """Persistent state of the block.
@@ -1014,14 +1070,17 @@
 
   def __init__(
       self,
       layer_tag_eq: tags.LayerTagEqn,
       name: str,
       axis_groups: Optional[Sequence[Sequence[int]]] = None,
   ):
+
+    # Even though the superclass constructor will set this later, we need to do
+    # it now since it's used below.
     self._layer_tag_eq = layer_tag_eq
 
     if axis_groups is None:
       self.axis_groups = tuple((i,) for i in range(self.array_ndim))
     else:
       self.axis_groups = tuple(tuple(g) for g in axis_groups)
 
@@ -1044,15 +1103,15 @@
   @abc.abstractmethod
   def array_to_parameters_shaped_list(self, array: Array) -> Tuple[Array, ...]:
     """An inverse transformation of ``self.parameters_shaped_list_to_array``."""
 
   @property
   def array_shape(self) -> Shape:
     """The shape of the single non axis grouped array."""
-    avals = [jnp.zeros(v.aval.shape) for v in self.parameter_variables]
+    avals = [jnp.zeros(v.aval.shape) for v in self.parameter_variables]  # pytype: disable=attribute-error  # always-use-property-annotation
     return self.parameters_shaped_list_to_array(avals).shape
 
   @property
   def array_ndim(self) -> int:
     """The number of dimensions of the single non axis grouped array."""
     return len(self.array_shape)
 
@@ -1063,15 +1122,15 @@
         utils.product([self.array_shape[i] for i in group])
         for group in self.axis_groups
     )
 
   @property
   def grouped_array_ndim(self) -> int:
     """The number of dimensions of the grouped array."""
-    return len(self.axis_groups)
+    return len(self.grouped_array_shape)
 
   def parameter_shaped_list_to_grouped_array(
       self,
       parameters_shaped_list: Sequence[Array],
   ) -> Array:
     """Combines all parameters to a single grouped array."""
     array = self.parameters_shaped_list_to_array(parameters_shaped_list)
@@ -1088,59 +1147,101 @@
   def _init(
       self,
       rng: PRNGKey,
       exact_powers_to_cache: Set[Scalar],
       approx_powers_to_cache: Set[Scalar],
       cache_eigenvalues: bool,
   ) -> "KroneckerFactored.State":
+
     cache = {}
     factors = []
 
     for i, d in enumerate(self.grouped_array_shape):
+
       factors.append(
           utils.WeightedMovingAverage.zeros_array((d, d), self.dtype)
       )
 
       if cache_eigenvalues or exact_powers_to_cache:
         cache[f"{i}_factor_eigenvalues"] = jnp.zeros((d,), dtype=self.dtype)
 
       if exact_powers_to_cache:
         cache[f"{i}_factor_eigen_vectors"] = jnp.zeros((d, d), dtype=self.dtype)
 
       for power in approx_powers_to_cache:
+
         if power != -1:
           raise NotImplementedError(
               f"Approximations for power {power} is not yet implemented."
           )
+
         if str(power) not in cache:
           cache[str(power)] = {}
 
         cache[str(power)][f"{i}_factor"] = jnp.zeros((d, d), dtype=self.dtype)
 
-    return KroneckerFactored.State(cache=cache, factors=tuple(factors))
+    return KroneckerFactored.State(
+        cache=cache,
+        factors=tuple(factors),
+    )
+
+  def sync(
+      self,
+      state: "KroneckerFactored.State",
+      pmap_axis_name: str,
+  ) -> "KroneckerFactored.State":
+
+    # Copy this first since we mutate it later in this function.
+    state = state.copy()
+
+    for factor in state.factors:
+      factor.sync(pmap_axis_name)
+
+    return state
 
   def _multiply_matpower_unscaled(
       self,
       state: "KroneckerFactored.State",
       vector: Sequence[Array],
       identity_weight: Numeric,
       power: Scalar,
       exact_power: bool,
       use_cached: bool,
   ) -> Tuple[Array, ...]:
-    assert len(state.factors) == len(self.axis_groups)
+
+    assert len(state.factors) == self.grouped_array_ndim
 
     vector = self.parameter_shaped_list_to_grouped_array(vector)
 
     if power == 1:
+
       factors = [f.value for f in state.factors]
-      result = utils.kronecker_product_axis_mul_v(factors, vector)
-      result = result + identity_weight * vector
+
+      # state_dependent_scale needs to be included here because it won't be by
+      # the caller of this function (multiply_matpower) when use_cached=True.
+      # This is not an issue for other powers because they bake in
+      # state_dependent_scale.
+      scale = self.state_dependent_scale(state) if use_cached else 1.0
+
+      if exact_power:
+        result = scale * utils.kronecker_product_axis_mul_v(factors, vector)
+        result = result + identity_weight * vector
+
+      else:
+        # If compute pi_adjusted_kronecker_factors used a more expensive matrix
+        # norm in its computation, it might make sense to cache it. But we
+        # currently don't do that.
+
+        result = scale * utils.kronecker_product_axis_mul_v(
+            utils.pi_adjusted_kronecker_factors(
+                *factors, damping=identity_weight / scale),
+            vector)
 
     elif exact_power:
+
       if use_cached:
         s = [
             state.cache[f"{i}_factor_eigenvalues"]
             for i in range(len(state.factors))
         ]
         q = [
             state.cache[f"{i}_factor_eigen_vectors"]
@@ -1154,184 +1255,175 @@
 
       eigenvalues = utils.outer_product(*s) + identity_weight
       eigenvalues = jnp.power(eigenvalues, power)
 
       result = utils.kronecker_eigen_basis_axis_mul_v(q, eigenvalues, vector)
 
     else:
-      if power != -1:
+
+      if power != -1 and power != -0.5:
         raise NotImplementedError(
             f"Approximations for power {power} is not yet implemented."
         )
 
       if use_cached:
+
+        assert power != -0.5
+
         factors = [
             state.cache[str(power)][f"{i}_factor"]
             for i in range(len(state.factors))
         ]
 
       else:
-        factors = utils.pi_adjusted_kronecker_inverse(
-            *[factor.value for factor in state.factors],
-            damping=identity_weight,
-        )
+
+        factors = [factor.value for factor in state.factors]
+
+        factors = utils.pi_adjusted_kronecker_factors(
+            *factors, damping=identity_weight)
+
+        if power == -1:
+          factors = utils.invert_psd_matrices(factors)
+        elif power == -0.5:
+          factors = utils.inverse_sqrt_psd_matrices(factors)
+        else:
+          raise NotImplementedError()
 
       result = utils.kronecker_product_axis_mul_v(factors, vector)
 
     return self.grouped_array_to_parameters_shaped_list(result)
 
   def _eigenvalues_unscaled(
       self,
       state: "KroneckerFactored.State",
       use_cached: bool,
   ) -> Array:
-    assert len(state.factors) == len(self.axis_groups)
+
+    assert len(state.factors) == self.grouped_array_ndim
 
     if use_cached:
       s = [
           state.cache[f"{i}_factor_eigenvalues"]
           for i in range(len(state.factors))
       ]
     else:
       s_q = [utils.safe_psd_eigh(factor.value) for factor in state.factors]
       s, _ = zip(*s_q)
 
     return utils.outer_product(*s)
 
-  @utils.auto_scope_method
-  def update_curvature_matrix_estimate(
-      self,
-      state: "KroneckerFactored.State",
-      estimation_data: Mapping[str, Sequence[Array]],
-      ema_old: Numeric,
-      ema_new: Numeric,
-      batch_size: Numeric,
-      pmap_axis_name: Optional[str],
-  ) -> "KroneckerFactored.State":
-    assert len(state.factors) == len(self.axis_groups)
-
-    # This function call will return a copy of state:
-    state = self._update_curvature_matrix_estimate(
-        state, estimation_data, ema_old, ema_new, batch_size
-    )
-
-    for factor in state.factors:
-      factor.sync(pmap_axis_name)
-
-    return state
-
-  @abc.abstractmethod
-  def _update_curvature_matrix_estimate(
-      self,
-      state: "KroneckerFactored.State",
-      estimation_data: Mapping[str, Sequence[Array]],
-      ema_old: Numeric,
-      ema_new: Numeric,
-      batch_size: Numeric,
-  ) -> "KroneckerFactored.State":
-    pass
-
   def _update_cache(  # pytype: disable=signature-mismatch  # numpy-scalars
       self,
       state: "KroneckerFactored.State",
       identity_weight: Numeric,
       exact_powers: Numeric,
       approx_powers: Numeric,
       eigenvalues: bool,
   ) -> "KroneckerFactored.State":
-    assert len(state.factors) == len(self.axis_groups)
+
+    assert len(state.factors) == self.grouped_array_ndim
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     scale = self.state_dependent_scale(state)
     factor_scale = jnp.power(scale, 1.0 / len(self.axis_groups))
 
     if eigenvalues or exact_powers:
+
       s_q = [utils.safe_psd_eigh(factor.value) for factor in state.factors]
+
       s, q = zip(*s_q)
+
       for i in range(len(state.factors)):
         state.cache[f"{i}_factor_eigenvalues"] = factor_scale * s[i]
 
         if exact_powers:
           state.cache[f"{i}_factor_eigen_vectors"] = q[i]
 
     for power in approx_powers:
+
       if power != -1:
         raise NotImplementedError(
             f"Approximations for power {power} is not yet implemented."
         )
 
       cache = state.cache[str(power)]
+
       # This computes the approximate inverse factors using the generalization
       # of the pi-adjusted inversion from the original KFAC paper.
-
       inv_factors = utils.pi_adjusted_kronecker_inverse(
           *[factor.value for factor in state.factors],
           damping=identity_weight,
       )
+
       for i in range(len(state.factors)):
         cache[f"{i}_factor"] = inv_factors[i] / factor_scale
 
     return state
 
+  def _norm_unscaled(
+      self,
+      state: CurvatureBlock.State,
+      norm_type: str
+  ) -> Numeric:
+
+    return utils.product(
+        utils.psd_matrix_norm(f.value, norm_type=norm_type)
+        for f in state.factors)
+
 
 class TwoKroneckerFactored(KroneckerFactored):
   """A Kronecker factored block for layers with weights and an optional bias."""
 
   def __init__(
       self,
       layer_tag_eq: tags.LayerTagEqn,
       name: str,
   ):
     super().__init__(layer_tag_eq, name, ((0,), (1,)))
 
   @property
   def has_bias(self) -> bool:
     """Whether this layer's equation has a bias."""
-    return len(self._layer_tag_eq.invars) == 4
-
-  @abc.abstractmethod
-  def _update_curvature_matrix_estimate(
-      self,
-      state: "KroneckerFactored.State",
-      estimation_data: Mapping[str, Sequence[Array]],
-      ema_old: Numeric,
-      ema_new: Numeric,
-      batch_size: Numeric,
-  ) -> "KroneckerFactored.State":
-    pass
+    return len(self.parameter_variables) == 2
 
   def parameters_shaped_list_to_array(
       self,
       parameters_shaped_list: Sequence[Array],
   ) -> Array:
+
     for p, s in zip(parameters_shaped_list, self.parameters_shapes):
       assert p.shape == s
 
     if self.has_bias:
       w, b = parameters_shaped_list
       return jnp.concatenate([w.reshape([-1, w.shape[-1]]), b[None]], axis=0)
+
     else:
       # This correctly reshapes the parameters of both dense and conv2d blocks
       [w] = parameters_shaped_list
       return w.reshape([-1, w.shape[-1]])
 
   def array_to_parameters_shaped_list(self, array: Array) -> Tuple[Array, ...]:
+
     if self.has_bias:
       w, b = array[:-1], array[-1]
       return w.reshape(self.parameters_shapes[0]), b
+
     else:
       return tuple([array.reshape(self.parameters_shapes[0])])
 
   def _to_dense_unscaled(self, state: "KroneckerFactored.State") -> Array:
+
     assert 0 < self.number_of_parameters <= 2
     inputs_factor = state.factors[0].value
 
     if self.has_bias and self.parameters_canonical_order[0] != 0:
+
       # Permute the matrix according to the parameters canonical order
       inputs_factor = utils.block_permuted(
           state.factors[0].value,
           block_sizes=[state.factors[0].raw_value.shape[0] - 1, 1],
           block_order=(1, 0),
       )
 
@@ -1342,58 +1434,78 @@
   """Approximates the diagonal of the curvature with in the most obvious way.
 
   The update to the curvature estimate is computed by ``(sum_i g_i) ** 2 / N``.
   where `g_i` is the gradient of each individual data point, and ``N`` is the
   batch size.
   """
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: "NaiveDiagonal.State",
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> "NaiveDiagonal.State":
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     for factor, dw in zip(state.diagonal_factors,
                           estimation_data["params_tangent"]):
+
       factor.update(dw * dw / batch_size, ema_old, ema_new)
 
     return state
 
 
 class NaiveFull(Full):
   """Approximates the full curvature with in the most obvious way.
 
   The update to the curvature estimate is computed by
   ``(sum_i g_i) (sum_i g_i)^T / N``, where ``g_i`` is the gradient of each
   individual data point, and ``N`` is the batch size.
   """
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: Full.State,
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> Full.State:
 
+    # This method supports the case where the param tangents have an extra
+    # leading dimension that should be summed over (after the outer products).
+    # TODO(jamesmartens): add support for this to NaiveDiagonal
+
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
-    params_grads = jax.tree_util.tree_leaves(estimation_data["params_tangent"])
-    params_grads = jax.tree_map(lambda x: x.flatten(), params_grads)
-    grads = jnp.concatenate(params_grads, axis=0)
+    params_tangents = jax.tree_util.tree_leaves(
+        estimation_data["params_tangent"])
+
+    params_tangents_flattened = []
+
+    assert len(params_tangents) == self.number_of_parameters
 
-    state.matrix.update(jnp.outer(grads, grads) / batch_size, ema_old, ema_new)
+    for p_shape, pt in zip(self.parameters_shapes, params_tangents):
+
+      assert pt.shape[-len(p_shape):] == p_shape
+      p_size = utils.product(p_shape)
+
+      params_tangents_flattened.append(pt.reshape([-1, p_size]))
+
+    tangents = jnp.concatenate(params_tangents_flattened, axis=1)
+
+    stats = jnp.einsum("ay,az->yz", tangents, tangents) / batch_size
+    state.matrix.update(stats, ema_old, ema_new)
 
     return state
 
 
 #  _____
 # |  __ \
 # | |  | | ___ _ __  ___  ___
@@ -1405,17 +1517,18 @@
 
 class DenseDiagonal(Diagonal):
   """A `Diagonal` block specifically for dense layers."""
 
   @property
   def has_bias(self) -> bool:
     """Whether the layer has a bias parameter."""
-    return len(self.parameters_shapes) == 2
+    return len(self.parameter_variables) == 2
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: "Diagonal.State",
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> "Diagonal.State":
@@ -1439,15 +1552,16 @@
 
     return state
 
 
 class DenseFull(Full):
   """A `Full` block specifically for dense layers."""
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: "Full.State",
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> "Full.State":
@@ -1457,28 +1571,31 @@
 
     x, = estimation_data["inputs"]
     dy, = estimation_data["outputs_tangent"]
 
     assert utils.first_dim_is_size(batch_size, x, dy)
 
     params_tangents = x[:, :, None] * dy[:, None, :]
+
     if self.number_of_parameters == 2:
       params_tangents = jnp.concatenate([params_tangents, dy[:, None]], axis=1)
+
     params_tangents = jnp.reshape(params_tangents, [batch_size, -1])
 
     matrix_update = jnp.matmul(params_tangents.T, params_tangents) / batch_size
     state.matrix.update(matrix_update, ema_old, ema_new)
 
     return state
 
 
 class DenseTwoKroneckerFactored(TwoKroneckerFactored):
   """A :class:`~TwoKroneckerFactored` block specifically for dense layers."""
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: KroneckerFactored.State,
       estimation_data: Mapping[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> KroneckerFactored.State:
@@ -1548,15 +1665,15 @@
         func=self.conv2d_tangent_squared,
         max_parallel_size=max_elements_for_vmap or get_max_parallel_elements(),
     )
     super().__init__(layer_tag_eq, name)
 
   @property
   def has_bias(self) -> bool:
-    return len(self.parameters_shapes) == 2
+    return len(self.parameter_variables) == 2
 
   def conv2d_tangent_squared(
       self,
       image_features_map: Array,
       output_tangent: Array,
   ) -> Array:
     """Computes the elementwise square of a tangent for a single feature map."""
@@ -1570,15 +1687,16 @@
             **extra_params
         ),
         image_features_map[None], jnp.zeros(self.parameters_shapes[0])
     )
 
     return jnp.square(vjp(output_tangent[None])[1])
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: Diagonal.State,
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> Diagonal.State:
@@ -1672,15 +1790,16 @@
       sum_axis = tuple(range(num_axis))
       tangents += (jnp.sum(tangent_of_outputs, axis=sum_axis),)
 
     flat_tangents = self.parameters_list_to_single_vector(tangents)
 
     return jnp.outer(flat_tangents, flat_tangents)
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: Full.State,
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> Full.State:
@@ -1817,15 +1936,16 @@
     ein_str = f"{lhs_str},{rhs_str}->yz"
     stats = jnp.einsum(ein_str, tangent_of_output, tangent_of_output)
 
     # Normalize by the `batch size` * `num_locations`
     normalizer = tangent_of_output.shape[0] * self.num_locations
     return stats / normalizer
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: TwoKroneckerFactored.State,
       estimation_data: Mapping[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> TwoKroneckerFactored.State:
@@ -1893,15 +2013,16 @@
     return self._layer_tag_eq.params["has_scale"]
 
   @property
   def has_shift(self) -> bool:
     """Whether this layer's equation has a shift."""
     return self._layer_tag_eq.params["has_shift"]
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: Diagonal.State,
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> Diagonal.State:
@@ -1954,15 +2075,16 @@
     return self._layer_tag_eq.params["has_scale"]
 
   @property
   def _has_shift(self) -> bool:
     """Whether this layer's equation has a shift."""
     return self._layer_tag_eq.params["has_shift"]
 
-  def _update_curvature_matrix_estimate(
+  @utils.auto_scope_method
+  def update_curvature_matrix_estimate(
       self,
       state: Full.State,
       estimation_data: Dict[str, Sequence[Array]],
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
   ) -> Full.State:
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/curvature_estimator.py` & `kfac-jax-0.0.6/kfac_jax/_src/curvature_estimator.py`

 * *Files 8% similar despite different names*

```diff
@@ -63,14 +63,20 @@
 
 # Types for annotation
 Array = utils.Array
 PRNGKey = utils.PRNGKey
 Numeric = utils.Numeric
 Scalar = utils.Scalar
 Shape = utils.Shape
+LossFunction = loss_functions.LossFunction
+LossFunctionsTuple = Tuple[loss_functions.LossFunction, ...]
+LossFunctionsSequence = Sequence[loss_functions.LossFunction]
+LossFunctionInputs = loss_functions.LossFunctionInputs
+LossFunctionInputsSequence = Sequence[loss_functions.LossFunctionInputs]
+LossFunctionInputsTuple = Tuple[loss_functions.LossFunctionInputs, ...]
 CurvatureBlockCtor = Callable[
     [tags.LayerTagEqn, str],
     curvature_blocks.CurvatureBlock
 ]
 StateType = TypeVar("StateType")
 
 # Special global variables
@@ -122,14 +128,18 @@
       func: The model function, which should have at least one registered loss.
       params_index: The index of the parameters argument in arguments list of
         ``func``.
       batch_size_extractor: A function that takes as input the function
         arguments and returns the batch size for a single device.
         (Default: ``kfac.utils.default_batch_size_extractor``)
     """
+    self.compute_losses = tracer.compute_all_losses(
+        func=func,
+        params_index=params_index
+    )
     self._loss_tags_vjp = tracer.loss_tags_vjp(
         func=func,
         params_index=params_index
     )
     self._loss_tags_jvp = tracer.loss_tags_jvp(
         func=func,
         params_index=params_index,
@@ -144,37 +154,37 @@
     """The expected batch size given a list of loss instances."""
     return self._batch_size_extractor(func_args[-1])
 
   @classmethod
   def _multiply_loss_fisher(
       cls,
       losses: Sequence[loss_functions.NegativeLogProbLoss],
-      loss_vectors: Sequence[Sequence[Array]]
-  ) -> Tuple[Tuple[Array, ...], ...]:
+      loss_vectors: LossFunctionInputsSequence,
+  ) -> LossFunctionInputsTuple:
     """Multiplies ``loss_vectors`` by the Fisher of the total loss."""
     assert len(losses) == len(loss_vectors)
     return tuple(loss.multiply_fisher(vec)
                  for loss, vec in zip(losses, loss_vectors))
 
   @classmethod
   def _multiply_loss_ggn(
       cls,
-      losses: Sequence[loss_functions.LossFunction],
-      loss_vectors: Sequence[Sequence[Array]]
-  ) -> Tuple[Tuple[Array, ...], ...]:
+      losses: LossFunctionsSequence,
+      loss_vectors: LossFunctionInputsSequence,
+  ) -> LossFunctionInputsTuple:
     """Multiplies ``loss_vectors`` by the GGN of the total loss."""
     return tuple(loss.multiply_ggn(vec)
                  for loss, vec in zip(losses, loss_vectors))
 
   @classmethod
   def _multiply_loss_fisher_factor(
       cls,
       losses: Sequence[loss_functions.NegativeLogProbLoss],
       loss_inner_vectors: Sequence[Array],
-  ) -> Tuple[Tuple[Array, ...], ...]:
+  ) -> LossFunctionInputsTuple:
     """Multiplies the vectors with the Fisher factors of each loss.
 
     Args:
       losses: A sequence of loss instances.
       loss_inner_vectors: A sequence of vectors, each corresponding to one
         instance of a loss in losses.
 
@@ -187,15 +197,15 @@
                  for loss, vec in zip(losses, loss_inner_vectors))
 
   @classmethod
   def _multiply_loss_ggn_factor(
       cls,
       losses: Sequence[loss_functions.LossFunction],
       loss_inner_vectors: Sequence[Array],
-  ) -> Tuple[Tuple[Array, ...], ...]:
+  ) -> LossFunctionInputsTuple:
     """Multiplies the vectors with the GGN factors of each loss.
 
     Args:
       losses: A sequence of loss instances.
       loss_inner_vectors: A sequence of vectors, each corresponding to one
         instance of a loss in losses.
 
@@ -206,15 +216,15 @@
     return tuple(loss.multiply_ggn_factor(vec)
                  for loss, vec in zip(losses, loss_inner_vectors))
 
   @classmethod
   def _multiply_loss_fisher_factor_transpose(
       cls,
       losses: Sequence[loss_functions.NegativeLogProbLoss],
-      loss_vectors: Sequence[Sequence[Array]]
+      loss_vectors: LossFunctionInputsSequence,
   ) -> Tuple[Array, ...]:
     """Multiplies the vectors with the transposed Fisher factors of each loss.
 
     Args:
       losses: A sequence of loss instances.
       loss_vectors: A sequence of vectors, each corresponding to one instance of
         a loss in losses.
@@ -226,16 +236,16 @@
     assert len(losses) == len(loss_vectors)
     return tuple(loss.multiply_fisher_factor_transpose(vec)
                  for loss, vec in zip(losses, loss_vectors))
 
   @classmethod
   def _multiply_loss_ggn_factor_transpose(
       cls,
-      losses: Sequence[loss_functions.LossFunction],
-      loss_vectors: Sequence[Sequence[Array]]
+      losses: LossFunctionsSequence,
+      loss_vectors: LossFunctionInputsSequence,
   ) -> Tuple[Array, ...]:
     """Multiplies the vectors with the transposed GGN factors of each loss.
 
     Args:
       losses: A sequence of loss instances.
       loss_vectors: A sequence of vectors, each corresponding to one instance of
         a loss in losses.
@@ -284,14 +294,73 @@
     batch_size = self.batch_size(func_args)
 
     assert utils.abstract_objects_equal(parameter_structured_vector, vector)
 
     return utils.scalar_div(vector, batch_size)
 
   @utils.auto_scope_method
+  def multiply_jacobian(
+      self,
+      func_args: utils.FuncArgs,
+      parameter_structured_vector: utils.Params,
+      return_loss_objects: bool = False,
+  ) -> Union[
+      LossFunctionInputsTuple,
+      Tuple[LossFunctionInputsTuple, LossFunctionsTuple],
+  ]:
+    """Multiplies a vector by the model's Jacobian.
+
+    Args:
+      func_args: The inputs to the model function.
+      parameter_structured_vector: A vector in the same structure as the
+        parameters of the model.
+      return_loss_objects: If set to `True` will return as an additional output
+        the loss objects evaluated at the provided function arguments.
+
+    Returns:
+      The product ``J v``, where ``J`` is the model's Jacobian and ``v`` is
+      given by ``parameter_structured_vector``.
+    """
+    losses, jacobian_vectors = self._loss_tags_jvp(
+        func_args, parameter_structured_vector)
+    if return_loss_objects:
+      return jacobian_vectors, losses
+    return jacobian_vectors
+
+  @utils.auto_scope_method
+  def multiply_jacobian_transpose(
+      self,
+      func_args: utils.FuncArgs,
+      loss_input_vectors: LossFunctionInputsSequence,
+      return_loss_objects: bool = False,
+  ) -> Union[
+      utils.Params,
+      Tuple[utils.Params, LossFunctionsTuple]
+  ]:
+    """Multiplies a vector by the model's transposed Jacobian.
+
+    Args:
+      func_args: The inputs to the model function.
+      loss_input_vectors: A sequence over losses of sequences of arrays that
+        are the size of the loss's inputs. This represents the vector to be
+        multiplied.
+      return_loss_objects: If set to `True` will return as an additional output
+        the loss objects evaluated at the provided function arguments.
+
+    Returns:
+      The product ``J^T v``, where ``J`` is the model's Jacobian and ``v`` is
+      given by ``loss_inner_vectors``.
+    """
+    losses, vjp = self._loss_tags_vjp(func_args)
+    vector = vjp(loss_input_vectors)
+    if return_loss_objects:
+      return vector, losses
+    return vector
+
+  @utils.auto_scope_method
   def multiply_fisher(
       self,
       func_args: utils.FuncArgs,
       parameter_structured_vector: utils.Params,
   ) -> utils.Params:
     """Multiplies the vector with the Fisher matrix of the total loss.
 
@@ -301,26 +370,27 @@
       parameter_structured_vector: The vector which to multiply with the Fisher
         matrix.
 
     Returns:
       The product ``Fv``.
     """
     losses: Sequence[loss_functions.NegativeLogProbLoss]
-    losses, jacobian_vectors = self._loss_tags_jvp(
-        func_args, parameter_structured_vector)
+    jacobian_vectors, losses = self.multiply_jacobian(
+        func_args, parameter_structured_vector, True)
+
     if any(not isinstance(l, loss_functions.NegativeLogProbLoss)
            for l in losses):
       raise ValueError("To use `multiply_fisher` all registered losses must "
                        "be a subclass of `NegativeLogProbLoss`.")
-    _, vjp = self._loss_tags_vjp(func_args)
-    self._assert_losses_same(losses, _)
 
     loss_fisher_jacobian_vectors = self._multiply_loss_fisher(
         losses, jacobian_vectors)
-    vector = vjp(loss_fisher_jacobian_vectors)
+
+    vector = self.multiply_jacobian_transpose(
+        func_args, loss_fisher_jacobian_vectors)
     batch_size = self.batch_size(func_args)
 
     assert utils.abstract_objects_equal(parameter_structured_vector, vector)
 
     return utils.scalar_div(vector, batch_size)
 
   @utils.auto_scope_method
@@ -336,22 +406,22 @@
         matrix.
       parameter_structured_vector: The vector which to multiply with the GGN
         matrix.
 
     Returns:
       The product ``Gv``.
     """
-    losses, jacobian_vectors = self._loss_tags_jvp(
-        func_args, parameter_structured_vector)
-    _, vjp = self._loss_tags_vjp(func_args)
-    self._assert_losses_same(losses, _)
+    jacobian_vectors, losses = self.multiply_jacobian(
+        func_args, parameter_structured_vector, True)
 
     loss_ggn_jacobian_vectors = self._multiply_loss_ggn(
         losses, jacobian_vectors)
-    vector = vjp(loss_ggn_jacobian_vectors)
+
+    vector = self.multiply_jacobian_transpose(
+        func_args, loss_ggn_jacobian_vectors)
     batch_size = self.batch_size(func_args)
 
     assert utils.abstract_objects_equal(parameter_structured_vector, vector)
 
     return utils.scalar_div(vector, batch_size)
 
   @utils.auto_scope_method
@@ -367,24 +437,26 @@
         Fisher matrix.
       parameter_structured_vector: The vector which to multiply with the Fisher
         matrix.
 
     Returns:
       The product ``B^T v``, where ``F = BB^T``.
     """
-    losses: Sequence[loss_functions.NegativeLogProbLoss]
-    losses, jacobian_vectors = self._loss_tags_jvp(
-        func_args, parameter_structured_vector)
+    jacobian_vectors, losses = self.multiply_jacobian(
+        func_args, parameter_structured_vector, True)
+
     if any(not isinstance(l, loss_functions.NegativeLogProbLoss)
            for l in losses):
       raise ValueError("To use `multiply_fisher` all registered losses must "
                        "be a subclass of `NegativeLogProbLoss`.")
+
     loss_vectors = self._multiply_loss_fisher_factor_transpose(
         losses, jacobian_vectors)
     batch_size = self.batch_size(func_args)
+
     return utils.scalar_div(loss_vectors, jnp.sqrt(batch_size))
 
   @utils.auto_scope_method
   def multiply_ggn_factor_transpose(
       self,
       func_args: utils.FuncArgs,
       parameter_structured_vector: utils.Params,
@@ -396,18 +468,20 @@
         matrix.
       parameter_structured_vector: The vector which to multiply with the GGN
         matrix.
 
     Returns:
       The product ``B^T v``, where ``G = BB^T``.
     """
-    losses, jacobian_vectors = self._loss_tags_jvp(
-        func_args, parameter_structured_vector)
+    jacobian_vectors, losses = self.multiply_jacobian(
+        func_args, parameter_structured_vector, True)
+
     vectors = self._multiply_loss_ggn_factor_transpose(losses, jacobian_vectors)
     batch_size = self.batch_size(func_args)
+
     return utils.scalar_div(vectors, jnp.sqrt(batch_size))
 
   @utils.auto_scope_method
   def multiply_fisher_factor(
       self,
       func_args: utils.FuncArgs,
       loss_inner_vectors: Sequence[Array],
@@ -463,35 +537,14 @@
 
     vectors = vjp(ggn_factor_vectors)
 
     batch_size = self.batch_size(func_args)
 
     return utils.scalar_div(vectors, jnp.sqrt(batch_size))
 
-  @utils.auto_scope_method
-  def multiply_jacobian_transpose(
-      self,
-      func_args: utils.FuncArgs,
-      loss_input_vectors: Sequence[Sequence[Array]],
-  ) -> utils.Params:
-    """Multiplies a vector by the model's transposed Jacobian.
-
-    Args:
-      func_args: The inputs to the model function.
-      loss_input_vectors: A sequence over losses of sequences of arrays that
-        are the size of the loss's inputs. This represents the vector to be
-        multiplied.
-
-    Returns:
-      The product ``J^T v``, where ``J`` is the model's Jacobian and ``v`` is
-      is given by ``loss_inner_vectors``.
-    """
-    _, vjp = self._loss_tags_vjp(func_args)
-    return vjp(loss_input_vectors)
-
   def get_loss_inner_vector_shapes_and_batch_size(
       self,
       func_args: utils.FuncArgs,
       mode: str
   ) -> Tuple[Tuple[Shape, ...], int]:
     """Get shapes of loss inner vectors, and the batch size.
 
@@ -542,16 +595,16 @@
   matrix and provides many useful functionalities for interacting with it.
   The state of the estimator contains two parts: the estimated curvature
   internal representation, as well as potential cached values of different
   expression involving the curvature matrix (for example matrix powers).
   The cached values are only updated once you call the method
   :func:`~CurvatureEstimator.update_cache`. Multiple methods contain the keyword
   argument ``use_cached`` which specify whether you want to compute the
-  corresponding expression using the current curvature estimate or used a cached
-  version.
+  corresponding expression using the current curvature estimate or using a
+  cached version.
 
   Attributes:
     func: The model evaluation function.
     params_index: The index of the parameters argument in arguments list of
       ``func``.
     default_estimation_mode: The estimation mode which to use by default when
       calling :func:`~CurvatureEstimator.update_curvature_matrix_estimate`.
@@ -568,21 +621,27 @@
     Args:
       func: The model function, which should have at least one registered loss.
       params_index: The index of the parameters argument in arguments list of
         ``func``.
       default_estimation_mode: The estimation mode which to use by default when
         calling :func:`~CurvatureEstimator.update_curvature_matrix_estimate`.
     """
+
     if default_estimation_mode not in _ESTIMATION_MODES:
       raise ValueError("Unrecognised default_estimation_mode "
                        f"{default_estimation_mode}.")
+
     super().__init__()
+
     self.func = func
     self.params_index = params_index
     self.default_estimation_mode = default_estimation_mode
+    self.compute_losses = tracer.compute_all_losses(
+        func=func, params_index=params_index
+    )
 
   @property
   def default_mat_type(self) -> str:
     """The type of matrix that this estimator is approximating."""
     idx = self.default_estimation_mode.index("_")
     return self.default_estimation_mode[:idx]
 
@@ -622,23 +681,32 @@
       cache_eigenvalues: Specifies whether each block should be caching the
           eigenvalues of its approximate curvature.
     Returns:
       The initialized state of the estimator.
     """
 
   @abc.abstractmethod
+  def sync(
+      self,
+      state: StateType,
+      pmap_axis_name: Optional[str],
+  ) -> StateType:
+    """Synchronizes across devices the state of the estimator."""
+
+  @abc.abstractmethod
   def multiply_matpower(
       self,
       state: StateType,
       parameter_structured_vector: utils.Params,
       identity_weight: Numeric,
       power: Scalar,
       exact_power: bool,
       use_cached: bool,
       pmap_axis_name: Optional[str],
+      norm_to_scale_identity_weight_per_block: Optional[str] = None,
   ) -> utils.Params:
     """Computes ``(CurvatureMatrix + identity_weight I)**power`` times ``vector``.
 
     Args:
       state: The state of the estimator.
       parameter_structured_vector: A vector in the same structure as the
           parameters of the model.
@@ -653,59 +721,66 @@
           Otherwise this method might use a cheaper approximation, which *may*
           vary across different blocks.
       use_cached: Whether to use a cached (and possibly stale) version of the
           curvature matrix estimate.
       pmap_axis_name: The name of any pmap axis, which will be used for
           aggregating any computed values over multiple devices, as well as
           parallelizing the computation over devices in a block-wise fashion.
+      norm_to_scale_identity_weight_per_block: The name of a norm to use to
+          compute extra per-block scaling for identity_weight. See
+          psd_matrix_norm() in utils/math.py for the definition of these.
 
     Returns:
       A parameter structured vector containing the product.
     """
 
   def multiply(
       self,
       state: StateType,
       parameter_structured_vector: utils.Params,
       identity_weight: Numeric,
       exact_power: bool,
       use_cached: bool,
       pmap_axis_name: Optional[str],
+      norm_to_scale_identity_weight_per_block: Optional[str] = None,
   ) -> utils.Params:
     """Computes ``(CurvatureMatrix + identity_weight I)`` times ``vector``."""
 
     return self.multiply_matpower(
         state=state,
         parameter_structured_vector=parameter_structured_vector,
         identity_weight=identity_weight,
         power=1,
         exact_power=exact_power,
         use_cached=use_cached,
-        pmap_axis_name=pmap_axis_name
+        pmap_axis_name=pmap_axis_name,
+        norm_to_scale_identity_weight_per_block=norm_to_scale_identity_weight_per_block,
     )
 
   def multiply_inverse(
       self,
       state: StateType,
       parameter_structured_vector: utils.Params,
       identity_weight: Numeric,
       exact_power: bool,
       use_cached: bool,
       pmap_axis_name: Optional[str],
+      norm_to_scale_identity_weight_per_block: Optional[str] = None,
   ) -> utils.Params:
     """Computes ``(CurvatureMatrix + identity_weight I)^-1`` times ``vector``."""
 
     return self.multiply_matpower(
         state=state,
         parameter_structured_vector=parameter_structured_vector,
         identity_weight=identity_weight,
         power=-1,
         exact_power=exact_power,
         use_cached=use_cached,
-        pmap_axis_name=pmap_axis_name
+        pmap_axis_name=pmap_axis_name,
+        norm_to_scale_identity_weight_per_block=norm_to_scale_identity_weight_per_block,
     )
 
   @abc.abstractmethod
   def eigenvalues(
       self,
       state: StateType,
       use_cached: bool,
@@ -728,15 +803,14 @@
       self,
       state: StateType,
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
       rng: PRNGKey,
       func_args: utils.FuncArgs,
-      pmap_axis_name: Optional[str],
       estimation_mode: Optional[str] = None,
   ) -> StateType:
     """Updates the estimator's curvature estimates.
 
     Args:
       state: The state of the estimator to update.
       ema_old: Specifies the weight of the old value when computing the updated
@@ -746,17 +820,14 @@
       batch_size: The batch size.
       rng: A PRNGKey to be used for any potential sampling in the estimation
         process.
       func_args: A structure with the values of the inputs to the traced
         function (the ``tagged_func`` passed into the constructor) which to be
         used for the estimation process. Should have the same structure as the
         argument ``func_args`` passed in the constructor.
-      pmap_axis_name: When calling this method within a pmap context this
-        argument specifies the axis name over which to aggregate across
-        multiple devices/hosts.
       estimation_mode: The type of curvature estimator to use. By default
         (e.g. if ``None``) will use ``self.default_estimation_mode``. One of:
 
         * fisher_gradients - the basic estimation approach from the original
           K-FAC paper.
 
         * fisher_curvature_prop - method which estimates the Fisher using
@@ -818,51 +889,68 @@
       The updated state.
     """
 
   @abc.abstractmethod
   def to_dense_matrix(self, state: StateType) -> Array:
     """Returns an explicit dense array representing the curvature matrix."""
 
+  def compute_func_from_registered(self, func_args, batch_size) -> Array:
+
+    losses = self.compute_losses(func_args)
+
+    loss_values = tuple(
+        jnp.sum(loss.evaluate(None, coefficient_mode="regular"))
+        for loss in losses)
+
+    return sum(loss_values) / batch_size
+
 
 class BlockDiagonalCurvature(
     CurvatureEstimator["BlockDiagonalCurvature.State"]):
   """Block diagonal curvature estimator class."""
 
   @utils.register_state_class
   class State(utils.State):
     """Persistent state of the estimator.
 
     Attributes:
+      synced: A Jax boolean, specifying if the state has been synced across
+        devices (this does not include the cache, which is never explicitly
+        synced).
       blocks_states: A tuple of the state of the estimator corresponding to each
         block.
     """
+    synced: Array
     blocks_states: Tuple[curvature_blocks.CurvatureBlock.State, ...]
 
   def __init__(
       self,
       func: utils.Func,
       params_index: int = 0,
-      default_estimation_mode: str = "fisher_gradients",
+      default_estimation_mode: Optional[str] = None,
       layer_tag_to_block_ctor:
       Optional[Mapping[str, CurvatureBlockCtor]] = None,
       index_to_block_ctor:
       Optional[Mapping[Tuple[int, ...], CurvatureBlockCtor]] = None,
       auto_register_tags: bool = True,
       distributed_multiplies: bool = True,
       distributed_cache_updates: bool = True,
+      num_samples: int = 1,
+      should_vmap_samples: bool = False,
       **auto_register_kwargs: Any,
   ):
     """Initializes the curvature instance.
 
     Args:
       func: The model function, which should have at least one registered loss.
       params_index: The index of the parameters argument in arguments list of
         ``func``.
       default_estimation_mode: The estimation mode which to use by default when
-        calling ``self.update_curvature_matrix_estimate``.
+        calling ``self.update_curvature_matrix_estimate``. If ``None`` this will
+        be ``'fisher_gradients'``.
       layer_tag_to_block_ctor: An optional dict mapping tags to specific classes
         of block approximations, which to override the default ones.
       index_to_block_ctor: An optional dict mapping a specific block parameter
         indices to specific classes of block approximation, which to override
         the default ones. To get the correct indices check
         ``estimator.indices_to_block_map``.
       auto_register_tags: Whether to automatically register layer tags for
@@ -872,42 +960,56 @@
         multiplication operations across the different devices in a block-wise
         fashion. If False, each device will (redundantly) perform the operations
         for all of the blocks.
       distributed_cache_updates: Whether to distribute the cache
         update multiplication operations across the different devices in a
         block-wise fashion. If False, each device will (redundantly) perform
         the operations for all of the blocks.
+      num_samples: Number of samples (per case) to use when computing stochastic
+        curvature matrix estimates. This option is only used when
+        ``estimation_mode == 'fisher_gradients'`` or ``estimation_mode ==
+        '[fisher,ggn]_curvature_prop'``.
+      should_vmap_samples: Whether to use ``jax.vmap`` to compute samples
+        when ``num_samples > 1``.
       **auto_register_kwargs: Any keyword arguments to pass to into the auto
         registration function.
     """
-    super().__init__(func, params_index, default_estimation_mode)
+
+    super().__init__(
+        func, params_index, default_estimation_mode or "fisher_gradients")
+
     self._index_to_block_ctor = index_to_block_ctor or dict()
     self._layer_tag_to_block_ctor = layer_tag_to_block_ctor or dict()
     self._auto_register_tags = auto_register_tags
     self._auto_register_kwargs = auto_register_kwargs
     self._vjp = tracer.layer_tags_vjp(
         func=func,
         params_index=params_index,
         auto_register_tags=auto_register_tags,
         **auto_register_kwargs
     )
+
     # Initialized during finalization
     self._jaxpr: Optional[tracer.ProcessedJaxpr] = None
     self._blocks: Optional[Tuple[curvature_blocks.CurvatureBlock]] = None
 
     self._distributed_multiplies = distributed_multiplies
     self._distributed_cache_updates = distributed_cache_updates
 
+    self._num_samples = num_samples
+    self._should_vmap_samples = should_vmap_samples
+
   def _check_finalized(self):
     if not self.finalized:
       raise ValueError("The estimator has not been finalized. Call `init` or "
                        "`finalize` first.")
 
   def _create_blocks(self):
     """Creates all the curvature blocks instances in ``self._blocks``."""
+
     assert self._jaxpr is not None
 
     blocks_list = []
     counters = dict()
 
     for tag_eqn, idx in zip(self._jaxpr.layer_tags, self._jaxpr.layer_indices):  # pytype: disable=attribute-error  # always-use-return-annotations
 
@@ -1012,14 +1114,20 @@
     return len(self.jaxpr.params_vars_flat)
 
   @utils.auto_scope_method
   def _compute_losses_vjp(self, func_args: utils.FuncArgs):
     """Computes all model statistics needed for estimating the curvature."""
     return self._vjp(func_args)
 
+  @property
+  def param_order(self):
+    # is there a nicer way to do this?
+    params_vars = self.params_vector_to_blocks_vectors(self.jaxpr.params_vars)
+    return np.argsort([p.count for p in jax.tree_util.tree_leaves(params_vars)])
+
   def params_vector_to_blocks_vectors(
       self,
       parameter_structured_vector: utils.Params,
   ) -> Tuple[Tuple[Array, ...]]:
     """Splits the parameters to values for each corresponding block."""
 
     params_values_flat = jax.tree_util.tree_leaves(parameter_structured_vector)
@@ -1066,14 +1174,15 @@
       self,
       rng: PRNGKey,
       func_args: utils.FuncArgs,
       exact_powers_to_cache: Optional[curvature_blocks.ScalarOrSequence],
       approx_powers_to_cache: Optional[curvature_blocks.ScalarOrSequence],
       cache_eigenvalues: bool = False,
   ) -> "BlockDiagonalCurvature.State":
+
     if not self.finalized:
       self.finalize(func_args)
 
     blocks_init = []
     blocks_rng = jax.random.split(rng, self.num_blocks)
 
     for block, block_rng in zip(self.blocks, blocks_rng):
@@ -1082,48 +1191,96 @@
           rng=block_rng,
           exact_powers_to_cache=exact_powers_to_cache,
           approx_powers_to_cache=approx_powers_to_cache,
           cache_eigenvalues=cache_eigenvalues)
 
       blocks_init.append(block_init)
 
-    return BlockDiagonalCurvature.State(blocks_states=tuple(blocks_init))
+    return BlockDiagonalCurvature.State(
+        synced=jnp.asarray(True),
+        blocks_states=tuple(blocks_init),
+    )
+
+  def _sync_state(
+      self,
+      state: "BlockDiagonalCurvature.State",
+      pmap_axis_name: Optional[str],
+  ) -> "BlockDiagonalCurvature.State":
+
+    block_states = []
+
+    for block, block_state in zip(self.blocks, state.blocks_states):
+      block_states.append(block.sync(block_state.copy(), pmap_axis_name))
+
+    return BlockDiagonalCurvature.State(
+        synced=jnp.asarray(True),
+        blocks_states=tuple(block_states),
+    )
+
+  @utils.auto_scope_method
+  def sync(
+      self,
+      state: "BlockDiagonalCurvature.State",
+      pmap_axis_name: Optional[str],
+  ) -> "BlockDiagonalCurvature.State":
+
+    return jax.lax.cond(
+        state.synced,
+        lambda s: s,
+        functools.partial(self._sync_state, pmap_axis_name=pmap_axis_name),
+        state,
+    )
 
   @utils.auto_scope_method
   def multiply_matpower(
       self,
       state: "BlockDiagonalCurvature.State",
       parameter_structured_vector: utils.Params,
       identity_weight: Union[Numeric, Sequence[Numeric]],
       power: Scalar,
       exact_power: bool,
       use_cached: bool,
       pmap_axis_name: Optional[str],
+      norm_to_scale_identity_weight_per_block: Optional[str] = None,
   ) -> utils.Params:
 
     blocks_vectors = self.params_vector_to_blocks_vectors(
         parameter_structured_vector)
 
     identity_weight = utils.to_tuple_or_repeat(identity_weight, self.num_blocks)
 
+    def make_thunk(block, block_state, block_vector, block_identity_weight):
+
+      def thunk():
+
+        weight = block_identity_weight
+
+        if (norm_to_scale_identity_weight_per_block is not None
+            and norm_to_scale_identity_weight_per_block != "none"):
+
+          weight *= block.norm(
+              block_state, norm_to_scale_identity_weight_per_block)
+
+        return block.multiply_matpower(
+            state=block_state,
+            vector=block_vector,
+            identity_weight=weight,
+            power=power,
+            exact_power=exact_power,
+            use_cached=use_cached,
+        )
+
+      return thunk
+
     thunks = []
     for block, block_state, block_vector, block_identity_weight in zip(
         self.blocks, state.blocks_states, blocks_vectors, identity_weight):
 
       thunks.append(
-          functools.partial(
-              block.multiply_matpower,
-              state=block_state,
-              vector=block_vector,
-              identity_weight=block_identity_weight,
-              power=power,
-              exact_power=exact_power,
-              use_cached=use_cached,
-              )
-          )
+          make_thunk(block, block_state, block_vector, block_identity_weight))
 
     if self._distributed_multiplies and pmap_axis_name is not None:
 
       result = utils.distribute_thunks(thunks, pmap_axis_name)
 
     else:
       result = tuple(thunk() for thunk in thunks)
@@ -1165,24 +1322,84 @@
       state: "BlockDiagonalCurvature.State",
       use_cached: bool,
   ) -> Array:
 
     blocks_eigenvalues = self.block_eigenvalues(state, use_cached)
     return jnp.concatenate(blocks_eigenvalues, axis=0)
 
+  # Helper function that updates the blocks given a vjp vector
+  def _update_blocks(self, vjp_vec, losses_vjp, state, ema_old, ema_new,
+                     batch_size):
+
+    blocks_info = losses_vjp(vjp_vec)
+    assert len(blocks_info) == self.num_blocks
+
+    new_state = []
+    for block, block_state, block_info in zip(
+        self.blocks, state.blocks_states, blocks_info):
+
+      new_state.append(block.update_curvature_matrix_estimate(
+          block_state, block_info, ema_old, ema_new,
+          batch_size))
+
+    return BlockDiagonalCurvature.State(
+        synced=jnp.asarray(False),
+        blocks_states=tuple(new_state),
+    )
+
+  def _maybe_do_multiple_updates(self, update_func, state, rng, ema_old):
+
+    if self._num_samples > 1 and self._should_vmap_samples:
+
+      def f(rng_i):
+        return update_func(state, rng_i, ema_old)
+
+      states = jax.vmap(f)(jax.random.split(rng, self._num_samples))
+
+      # This implementation is quick and hacky and might break in the future.
+      # It works by averaging the states only for their floating point leaves,
+      # which are assumed to be statistics tensors.
+      return jax.tree_util.tree_map(
+          lambda x: (  # pylint: disable=g-long-lambda
+              jnp.mean(x, axis=0) if jnp.issubdtype(x.dtype, jnp.floating)
+              else x[0]),
+          states)
+
+    elif self._num_samples > 1:
+
+      def f(carry, rng_i):
+
+        state_i, ema_old_i = carry
+        new_state_i = update_func(state_i, rng_i, ema_old_i)
+
+        return (new_state_i, jnp.ones_like(ema_old_i)), None
+
+      (new_state, _), _ = jax.lax.scan(
+          f,
+          init=(state, jnp.asarray(ema_old)),
+          xs=jax.random.split(rng, self._num_samples)
+      )
+      return new_state
+
+    elif self._num_samples == 1:
+      return update_func(state, rng, ema_old)
+
+    else:
+      # Don't update the preconditioner at all.
+      return state
+
   @utils.auto_scope_method
   def update_curvature_matrix_estimate(
       self,
       state: "BlockDiagonalCurvature.State",
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
       rng: PRNGKey,
       func_args: utils.FuncArgs,
-      pmap_axis_name: Optional[str],
       estimation_mode: Optional[str] = None,
   ) -> "BlockDiagonalCurvature.State":
 
     if not self.finalized:
       self.finalize(func_args)
 
     estimation_mode = estimation_mode or self.default_estimation_mode
@@ -1194,113 +1411,112 @@
       if any(not isinstance(l, loss_functions.NegativeLogProbLoss)
              for l in losses):
         raise ValueError(
             f"One of the losses in the function is not an instance of "
             f"`loss_functions.NegativeLogProbLoss`, which is incompatible "
             f"with the estimation mode provided - {estimation_mode}.")
 
-    # Helper function that updates the blocks given a vjp vector
-    def update_blocks(vjp_vec_, state_, ema_old_, ema_new_):
-
-      blocks_info_ = losses_vjp(vjp_vec_)
-      assert len(blocks_info_) == self.num_blocks
+    if estimation_mode == "fisher_gradients":
 
-      new_state = []
-      for block_, block_state_, block_info_ in zip(
-          self.blocks, state_.blocks_states, blocks_info_):
+      def update_func(state_i, rng_i, ema_old_i):
 
-        new_state.append(block_.update_curvature_matrix_estimate(
-            block_state_, block_info_, ema_old_, ema_new_,
-            batch_size, pmap_axis_name))
+        keys = jax.random.split(
+            rng_i, len(losses)) if len(losses) > 1 else [rng_i]
 
-      return BlockDiagonalCurvature.State(blocks_states=tuple(new_state))
+        vjp_vec = tuple(
+            loss.grad_of_evaluate_on_sample(key, coefficient_mode="sqrt")
+            for loss, key in zip(losses, keys))
 
-    if estimation_mode == "fisher_gradients":
+        return self._update_blocks(
+            vjp_vec, losses_vjp, state_i, ema_old_i, ema_new, batch_size)
 
-      keys = jax.random.split(rng, len(losses)) if len(losses) > 1 else [rng]
-      vjp_vec = tuple(
-          loss.grad_of_evaluate_on_sample(key, coefficient_mode="sqrt")
-          for loss, key in zip(losses, keys))
-
-      return update_blocks(vjp_vec, state, ema_old, ema_new)
+      return self._maybe_do_multiple_updates(update_func, state, rng, ema_old)
 
     elif estimation_mode == "fisher_empirical":
 
       vjp_vec = tuple(
           loss.grad_of_evaluate(None, coefficient_mode="regular")
           for loss in losses)
 
-      return update_blocks(vjp_vec, state, ema_old, ema_new)
+      return self._update_blocks(vjp_vec, losses_vjp, state, ema_old, ema_new,
+                                 batch_size)
 
     elif estimation_mode in ("fisher_curvature_prop", "ggn_curvature_prop"):
 
-      keys = jax.random.split(rng, len(losses)) if len(losses) > 1 else [rng]
-      vjp_vec = []
+      def update_func(state_i, rng_i, ema_old_i):
 
-      for loss, key in zip(losses, keys):
+        keys = jax.random.split(
+            rng_i, len(losses)) if len(losses) > 1 else [rng_i]
 
-        if estimation_mode == "fisher_curvature_prop":
-          shape = loss.fisher_factor_inner_shape
-          random_b = jax.random.bernoulli(key, shape=shape)
-          vjp_vec.append(loss.multiply_fisher_factor(random_b * 2.0 - 1.0))
+        vjp_vec = []
 
-        else:
-          shape = loss.ggn_factor_inner_shape
-          random_b = jax.random.bernoulli(key, shape=shape)
-          vjp_vec.append(loss.multiply_ggn_factor(random_b * 2.0 - 1.0))
+        for loss, key in zip(losses, keys):
 
-      return update_blocks(tuple(vjp_vec), state, ema_old, ema_new)
+          if estimation_mode == "fisher_curvature_prop":
+            shape = loss.fisher_factor_inner_shape
+            random_b = jax.random.bernoulli(key, shape=shape)
+            vjp_vec.append(loss.multiply_fisher_factor(random_b * 2.0 - 1.0))
+
+          else:
+            shape = loss.ggn_factor_inner_shape
+            random_b = jax.random.bernoulli(key, shape=shape)
+            vjp_vec.append(loss.multiply_ggn_factor(random_b * 2.0 - 1.0))
+
+        return self._update_blocks(
+            tuple(vjp_vec), losses_vjp, state_i, ema_old_i, ema_new, batch_size)
+
+      return self._maybe_do_multiple_updates(update_func, state, rng, ema_old)
 
     elif estimation_mode in ("fisher_exact", "ggn_exact"):
-      # We use the following trick to simulate summation. The equation is:
-      #   estimate = ema_old * estimate + ema_new * (sum_i estimate_index_i^2)
-      #   weight = ema_old * weight + ema_new
-      # Instead we update the estimate n times with the following updates:
-      #   for k = 1
-      #     estimate_k = ema_old * estimate + (ema_new/n) * n*estimate_index_k^2
-      #     weight_k = ema_old * weight + (ema_new/n)
-      #   for k > 1:
-      #     estimate_k = 1.0 * estimate_k-1 + (ema_new/n) * n*estimate_index_k^2
-      #     weight_k = 1.0 * weight_k-1 + (ema_new/n)
-      # Which is mathematically equivalent to the original version.
 
       zero_tangents = jax.tree_util.tree_map(
           jnp.zeros_like, list(loss.parameter_dependants for loss in losses))
 
       if estimation_mode == "fisher_exact":
         shapes = [l.fisher_factor_inner_shape[1:] for l in losses]
       else:
         shapes = [l.ggn_factor_inner_shape[1:] for l in losses]
 
-      total_num_indices = sum(sum(s) for s in shapes)
-      ema_new = ema_new / total_num_indices
-
       # For now we support only inner shapes of 1 dimension, hence below the
       # (loss_num_indices,).
       assert all(len(s) == 1 for s in shapes)
 
+      total_num_indices = sum(sum(s) for s in shapes)
+
+      # This doesn't affect how the averaging is done except how the new stats
+      # are weighted vs the old stats (which if they also used this correction
+      # will just be 1:1).
+      ema_new = ema_new / total_num_indices
+
+      # This loop should probably be converted into a JAX loop for the sake of
+      # efficient compilation.
       for i, (loss, (loss_num_indices,)) in enumerate(zip(losses, shapes)):
+
         for index in range(loss_num_indices):
 
           vjp_vec = zero_tangents.copy()
 
           if estimation_mode == "fisher_exact":
             vjp_vec[i] = loss.multiply_fisher_factor_replicated_one_hot([index])
           else:
             vjp_vec[i] = loss.multiply_ggn_factor_replicated_one_hot([index])
 
           if isinstance(vjp_vec[i], Array):
             # In the special case of only one parameter, it still needs to be a
             # tuple for the tangents.
             vjp_vec[i] = (vjp_vec[i],)
 
+          # This will affect the tangent stat but not the activation stats. We
+          # do it because we want an average over loss indices for the
+          # activation stats, but a sum for the tangent stats.
           vjp_vec[i] = jax.tree_util.tree_map(
               lambda x: x * jnp.sqrt(total_num_indices), vjp_vec[i])
 
-          state = update_blocks(tuple(vjp_vec), state, ema_old, ema_new)
+          state = self._update_blocks(
+              tuple(vjp_vec), losses_vjp, state, ema_old, ema_new, batch_size)
 
           ema_old = 1.0
 
       return state
 
     else:
       raise ValueError(f"Unrecognised estimation_mode {estimation_mode}.")
@@ -1310,31 +1526,47 @@
       self,
       state: "BlockDiagonalCurvature.State",
       identity_weight: Union[Numeric, Sequence[Numeric]],
       exact_powers: Optional[curvature_blocks.ScalarOrSequence],
       approx_powers: Optional[curvature_blocks.ScalarOrSequence],
       eigenvalues: bool,
       pmap_axis_name: Optional[str],
+      norm_to_scale_identity_weight_per_block: Optional[str] = None,
   ) -> "BlockDiagonalCurvature.State":
+
     identity_weight = utils.to_tuple_or_repeat(identity_weight, self.num_blocks)
 
+    def make_thunk(block, block_state, block_identity_weight):
+
+      def thunk():
+
+        weight = block_identity_weight
+
+        if (norm_to_scale_identity_weight_per_block is not None
+            and norm_to_scale_identity_weight_per_block != "none"):
+
+          weight *= block.norm(
+              block_state, norm_to_scale_identity_weight_per_block)
+
+        return block.update_cache(
+            state=block_state,
+            identity_weight=block_identity_weight,
+            exact_powers=exact_powers,
+            approx_powers=approx_powers,
+            eigenvalues=eigenvalues,
+        )
+
+      return thunk
+
     thunks = []
     for block, block_state, block_identity_weight in zip(self.blocks,
                                                          state.blocks_states,
                                                          identity_weight):
-      thunks.append(
-          functools.partial(
-              block.update_cache,
-              state=block_state,
-              identity_weight=block_identity_weight,
-              exact_powers=exact_powers,
-              approx_powers=approx_powers,
-              eigenvalues=eigenvalues,
-              )
-          )
+
+      thunks.append(make_thunk(block, block_state, block_identity_weight))
 
     if self._distributed_cache_updates and pmap_axis_name is not None:
 
       assert utils.in_pmap(pmap_axis_name)
 
       def filter_outputs(thunk, vals):
 
@@ -1361,15 +1593,18 @@
       # Restore all of the unmodified state arrays.
       new_states = jax.tree_util.tree_map(lambda s, n: s if n is None else n,
                                           state.blocks_states, new_states)
 
     else:
       new_states = tuple(thunk() for thunk in thunks)
 
-    return BlockDiagonalCurvature.State(blocks_states=new_states)
+    return BlockDiagonalCurvature.State(
+        synced=state.synced,
+        blocks_states=new_states,
+    )
 
   @utils.auto_scope_method
   def to_diagonal_block_dense_matrix(
       self,
       state: "BlockDiagonalCurvature.State",
   ) -> Tuple[Array, ...]:
     """Returns a tuple of arrays with explicit dense matrices of each block."""
@@ -1389,200 +1624,117 @@
 
   This class estimates the full curvature matrix by looping over the batch
   dimension of the input data and for each single example computes an estimate
   of the curvature matrix and then averages over all examples in the input data.
   This implies that the computation scales linearly (without parallelism) with
   the batch size. The class stores the estimated curvature as a dense matrix,
   hence its memory requirement is (number of parameters)^2. If
-  ``estimation_mode`` is ``fisher_exact`` or ``ggn_exact`` than this would
+  ``estimation_mode`` is ``fisher_exact`` or ``ggn_exact`` then this would
   compute the exact curvature, but other modes are also supported. As a result
   of looping over the input data this class needs to know the index of the batch
   in the arguments to the model function and additionally, since the loop is
   achieved through indexing, each array leaf of that argument must have the same
   first dimension size, which will be interpreted as the batch size.
   """
 
   def __init__(
       self,
       func: utils.Func,
-      params_index: int = 0,
       batch_index: int = 1,
-      default_estimation_mode: str = "fisher_exact",
+      default_estimation_mode: Optional[str] = None,
       layer_tag_to_block_ctor:
       Optional[Mapping[str, CurvatureBlockCtor]] = None,
-      index_to_block_ctor:
-      Optional[Mapping[Tuple[int, ...], CurvatureBlockCtor]] = None,
-      auto_register_tags: bool = True,
-      **auto_register_kwargs
+      auto_register_tags: bool = False,
+      param_order: Optional[Tuple[int]] = None,
+      **kwargs: Any,
   ):
     """Initializes the curvature instance.
 
     Args:
       func: The model function, which should have at least one registered loss.
-      params_index: The index of the parameters argument in arguments list of
-        ``func``.
       batch_index: Specifies at which index of the inputs to ``func`` is the
         batch, representing data over which we average the curvature.
       default_estimation_mode: The estimation mode which to use by default when
-        calling ``self.update_curvature_matrix_estimate``.
+        calling ``self.update_curvature_matrix_estimate``. If ``None`` this will
+        be ``'fisher_exact'``.
       layer_tag_to_block_ctor: An optional dict mapping tags to specific classes
         of block approximations, which to override the default ones.
-      index_to_block_ctor: An optional dict mapping a specific block parameter
-        indices to specific classes of block approximation, which to override
-        the default ones. To get the correct indices check
-        ``estimator.indices_to_block_map``.
-      auto_register_tags: Whether to automatically register layer tags for
-        parameters that have not been manually registered. For further details
-        see :func:``~auto_register_tags``.
-      **auto_register_kwargs: Any keyword arguments to pass to into the auto
-        registration function.
+      auto_register_tags: This argument will be ignored since this subclass
+        doesn't use automatic registration.
+      param_order: An optional tuple of ints specifying the order of parameters
+        (with the reference order being the one used by ``func``). If not
+        specified, the reference order is used. The parameter order will
+        determine the order of blocks returned by
+        ``to_diagonal_block_dense_matrix``, and the order of the rows and
+        columns of ``to_dense_matrix``.
+      **kwargs: Addiional keyword arguments passed to the superclass
+        ``BlockDiagonalCurvature``.
     """
-    super().__init__(
-        func=func,
-        default_estimation_mode=default_estimation_mode,
-        params_index=params_index,
-        layer_tag_to_block_ctor=layer_tag_to_block_ctor,
-        index_to_block_ctor=index_to_block_ctor,
-        auto_register_tags=auto_register_tags,
-        **auto_register_kwargs
-    )
-    self._batch_index = batch_index
-
-  @property
-  def batch_index(self) -> int:
-    """The index in the inputs of the model function, which is the batch."""
-    return self._batch_index
-
-  def _create_blocks(self):
-    # Here in order to be able to have a block together for all parameters, we
-    # create a non-existing (in the original graph) generic layer tag equation.
-    assert self._jaxpr is not None
 
-    jax_version = (
-        jax.__version_info__ if hasattr(jax, "__version_info__")
-        else tuple(map(int, jax.__version__.split("."))))
-
-    if jax_version > (0, 3, 4):
-      self._blocks = (curvature_blocks.NaiveFull(
-          layer_tag_eq=tags.LayerTagEqn(
-              primitive=tags.generic,
-              invars=list(self._jaxpr.params_vars_flat),
-              outvars=list(self._jaxpr.params_vars_flat),
-              params={},
-              effects=jax.core.no_effects,
-              source_info=jax.core.source_info_util.new_source_info()
-          ),
-          name="ExactCurvature"
-      ),)
+    self._batch_index = batch_index
 
-    else:
-      self._blocks = (curvature_blocks.NaiveFull(
-          layer_tag_eq=tags.LayerTagEqn(
-              primitive=tags.generic,
-              invars=list(self._jaxpr.params_vars_flat),
-              outvars=list(self._jaxpr.params_vars_flat),
-              params={},
-              source_info=jax.core.source_info_util.new_source_info()  # pytype: disable=missing-parameter
-          ),
-          name="ExactCurvature"
-      ),)
-
-  def _compute_losses_vjp(self, func_args):
-
-    # For some reason pytype can't detect that this attribute exists from the
-    # super class.
-    losses, losses_vjp = self._vjp(func_args)  # pytype: disable=attribute-error
-
-    def modified_losses_jvp(vjp_vec):
-
-      blocks_info = losses_vjp(vjp_vec)
-
-      tangents = [block["params_tangent"] for block in blocks_info]
-      tangents = jax.tree_util.tree_leaves(tangents)
-
-      # Need to reorder all of the block information to follow the canonical
-      # order of variables
-      params_vars = BlockDiagonalCurvature.params_vector_to_blocks_vectors(
-          self, self.jaxpr.params_vars)  # pytype: disable=wrong-arg-types
-      order = np.argsort([p.count
-                          for p in jax.tree_util.tree_leaves(params_vars)])
+    if layer_tag_to_block_ctor is None:
+      layer_tag_to_block_ctor = dict(generic_tag=curvature_blocks.NaiveFull)
 
-      return [dict(params_tangent=tuple(tangents[i] for i in order))]
+    def retagged_func(params, *args):
 
-    return losses, modified_losses_jvp
+      params_flat, params_treedef = jax.tree_util.tree_flatten(params)
 
-  def params_vector_to_blocks_vectors(
-      self,
-      parameter_structured_vector: utils.Params,
-  ) -> Tuple[Tuple[Array, ...]]:
+      if param_order is not None:
+        params_flat_canonical_order = [params_flat[i] for i in param_order]
+        params_flat[param_order[0]] = tags.register_generic(
+            *params_flat_canonical_order)
 
-    return (tuple(jax.tree_util.tree_leaves(parameter_structured_vector)),)
+      else:
+        params_flat[0] = tags.register_generic(*params_flat)
 
-  def blocks_vectors_to_params_vector(
-      self,
-      blocks_vectors: Sequence[Sequence[Array]],
-  ) -> utils.Params:
+      params = jax.tree_util.tree_unflatten(params_treedef, params_flat)
 
-    assert len(blocks_vectors) == self.num_blocks
+      return func(params, *args)
 
-    return jax.tree_util.tree_unflatten(
-        self.jaxpr.params_tree, blocks_vectors[0])
+    super().__init__(
+        func=retagged_func,
+        default_estimation_mode=default_estimation_mode or "fisher_exact",
+        layer_tag_to_block_ctor=layer_tag_to_block_ctor,
+        auto_register_tags=False,
+        **kwargs,
+    )
 
+  @utils.auto_scope_method
   def update_curvature_matrix_estimate(
       self,
       state: BlockDiagonalCurvature.State,
       ema_old: Numeric,
       ema_new: Numeric,
       batch_size: Numeric,
       rng: PRNGKey,
       func_args: utils.FuncArgs,
-      pmap_axis_name: Optional[str],
       estimation_mode: Optional[str] = None,
-  ) -> curvature_blocks.Full.State:
+  ) -> BlockDiagonalCurvature.State:
 
     rng = jax.random.split(rng, batch_size)
 
+    super_ = super()
+
     def single_state_update(
         index: Numeric,
-        state_: curvature_blocks.Full.State
-    ) -> curvature_blocks.Full.State:
+        state_: BlockDiagonalCurvature.State
+    ) -> BlockDiagonalCurvature.State:
 
       is_first = index == 0
       args = list(func_args)
 
       # Index the batch for the `index` arguments.
       args[self._batch_index] = jax.tree_util.tree_map(
           lambda x: x[index][None], args[self._batch_index])
 
-      return BlockDiagonalCurvature.update_curvature_matrix_estimate(
-          self,
+      return super_.update_curvature_matrix_estimate(
           state=state_,
           ema_old=is_first * ema_old + (1 - is_first) * 1.0,
           ema_new=ema_new / batch_size,
           batch_size=1,
           rng=rng[index],
           func_args=args,
-          pmap_axis_name=pmap_axis_name,
           estimation_mode=estimation_mode,
       )
 
     return jax.lax.fori_loop(0, batch_size, single_state_update, state)
-
-  def update_cache(
-      self,
-      state: BlockDiagonalCurvature.State,
-      identity_weight: Numeric,
-      exact_powers: Optional[curvature_blocks.ScalarOrSequence],
-      approx_powers: Optional[curvature_blocks.ScalarOrSequence],
-      eigenvalues: bool,
-      pmap_axis_name: Optional[str],
-  ) -> curvature_blocks.Full.State:
-
-    block_state = self.blocks[0].update_cache(
-        state=state.blocks_states[0],
-        identity_weight=identity_weight,
-        exact_powers=exact_powers,
-        approx_powers=approx_powers,
-        eigenvalues=eigenvalues,
-    )
-
-    return BlockDiagonalCurvature.State(blocks_states=(block_state,))
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/layers_and_loss_tags.py` & `kfac-jax-0.0.6/kfac_jax/_src/layers_and_loss_tags.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,19 @@
 # limitations under the License.
 """K-FAC losses and layers tagging Jax primitives."""
 import types
 from typing import Any, Generic, Optional, Sequence, Type, TypeVar, Tuple, Union
 
 import jax
 from jax import core
-from jax.interpreters import batching as jax_batching
 
 # Types for annotation
 T = TypeVar("T")
 Array = jax.Array
 Arrays = Tuple[Array, ...]
-ArrayOrXla = TypeVar("ArrayOrXla", Array, jax.interpreters.xla.XlaOp)
 
 
 class LossTag(core.Primitive, Generic[T]):
   """A Jax primitive for tagging K-FAC losses.
 
   The primitive is no-op at runtime, however its goal is to tag (annotate) the
   Jax computation graph what expression exactly is the loss and what type of
@@ -57,26 +55,28 @@
         represents.
       parameter_dependants: The names of each of the parameter **dependent**
         inputs to the tag.
       parameter_independants: The names of each of the parameter **independent**
         inputs to the tag.
     """
     super().__init__(cls.__name__ + "_tag")
+
     self._cls = cls
     self._parameter_dependants = tuple(parameter_dependants)
     self._parameter_independants = tuple(parameter_independants)
 
-    jax.interpreters.xla.register_translation(self, self._xla_translation)
+    jax.interpreters.mlir.register_lowering(self, self._mlir_lowering)
     jax.interpreters.ad.primitive_jvps[self] = self._jvp
+
     # This line defines how does the tag behave under vmap. It is required for
     # any primitive that can be used inside a vmap. The reason why we want to
     # allow this is two fold - one to not break user code when the tags are not
     # used at all, and two - to be able to define a network with code for a
     # single example which is the vmap-ed for a batch.
-    jax_batching.primitive_batchers[self] = self._batching
+    jax.interpreters.batching.primitive_batchers[self] = self._batching
 
   @property
   def parameter_dependants_names(self) -> Tuple[str, ...]:
     """The number of parameter dependent inputs to the tag primitive."""
     return self._parameter_dependants
 
   @property
@@ -89,78 +89,91 @@
     return self.parameter_dependants_names + self.parameter_independants_names
 
   def extract_parameter_dependants(
       self,
       *args: T,
       args_names: Sequence[str],
   ) -> Tuple[T, ...]:
+
     assert len(args) == len(args_names)
+
     arg_map = dict(zip(args_names, args))
+
     return tuple(arg_map[name] for name in self.parameter_dependants_names)
 
   def loss(self, *args: Array, args_names: Sequence[str]) -> T:
     """Constructs an instance of the corresponding :class:`~LossFunction` class."""
+
     assert len(args) == len(args_names)
+
     arg_map = dict(zip(args_names, args))
     return self._cls(**arg_map)
 
   def get_outputs(
       self,
-      *args: ArrayOrXla,
+      *args: Array,
       args_names: Sequence[str],
-  ) -> Tuple[ArrayOrXla, ...]:
+  ) -> Tuple[Array, ...]:
     """Verifies that the number of arguments matches expectations."""
+
     assert len(args) == len(args_names)
+
     return tuple(arg for name, arg in zip(args_names, args)
                  if name in self.parameter_dependants_names)
 
   def impl(self, *operands: Array, args_names: Sequence[str]) -> Arrays:
     return self.get_outputs(*operands, args_names=args_names)
 
   def abstract_eval(
       self,
       *operands: Array,
       args_names: Sequence[str],
   ) -> Tuple[Arrays, jax.core.Effects]:
+
     return (self.get_outputs(*operands, args_names=args_names),
             jax.core.no_effects)
 
-  def _xla_translation(
+  def _mlir_lowering(
       self,
-      xla_context: jax.interpreters.xla.TranslationContext,
-      avals_in: Sequence[core.AbstractValue],
-      avals_out: Sequence[core.AbstractValue],
-      *args: jax.interpreters.xla.XlaOp,
+      context: jax.interpreters.mlir.LoweringRuleContext,
+      *args,
       args_names: Sequence[str],
-  ) -> Tuple[jax.interpreters.xla.XlaOp, ...]:
+  ) -> Tuple[Any, ...]:
     """The XLA translation rule for this primitive (creates a no-op tuple)."""
-    del avals_in, avals_out  # not used
+
+    del context
+
     return self.get_outputs(*args, args_names=args_names)
 
   def _jvp(
       self,
       arg_values: Sequence[Array],
       arg_tangents: Sequence[Array],
       args_names: Sequence[str],
   ) -> Tuple[Arrays, Arrays]:
     """Computes the Jacobian-vector product for the primitive."""
+
     if len(arg_values) != len(arg_tangents):
       raise ValueError("Values and tangents are not the same length.")
-    primal_output = self.bind(*arg_values, args_names=args_names)
+
+    primal_output = self.bind(*arg_values, args_names=tuple(args_names))
     tangent_output = self.get_outputs(*arg_tangents, args_names=args_names)
+
     return primal_output, tangent_output
 
   def _batching(
       self,
       batched_args: Sequence[Array],
       batched_dims: Union[int, Tuple[int, ...]],
       args_names: Sequence[str],
   ) -> Tuple[Array, Union[int, Tuple[int, ...]]]:
     """Defines how the primitive behaves under :func:`jax.vmap`."""
-    return self.bind(*batched_args, args_names=args_names), batched_dims
+
+    return (self.bind(*batched_args, args_names=tuple(args_names)),
+            batched_dims[:1])
 
 
 class LayerTag(core.Primitive):
   """A Jax primitive for tagging K-FAC layers.
 
   The primitive is no-op at runtime, however its goal is to tag (annotate) the
   Jax computation graph what expressions represents a single unique layer type.
@@ -190,23 +203,23 @@
     super().__init__(name)
     if num_outputs > 1:
       raise NotImplementedError(
           f"Only single outputs are supported, got: num_outputs={num_outputs}.")
     self._num_outputs = num_outputs
     self._num_inputs = num_inputs
 
-    jax.interpreters.xla.register_translation(self, self._xla_translation)  # pytype: disable=wrong-arg-types  # numpy-scalars
+    jax.interpreters.mlir.register_lowering(self, self._mlir_lowering)  # pytype: disable=wrong-arg-types  # numpy-scalars
     jax.interpreters.ad.deflinear(self, self._transpose)
     jax.interpreters.ad.primitive_transposes[self] = self._transpose
     # This line defines how does the tag behave under vmap. It is required for
     # any primitive that can be used inside a vmap. The reason why we want to
     # allow this is two fold - one to not break user code when the tags are not
     # used at all, and two - to be able to define a network with code for a
     # single example which is the vmap-ed for a batch.
-    jax_batching.primitive_batchers[self] = self._batching
+    jax.interpreters.batching.primitive_batchers[self] = self._batching
 
   @property
   def num_outputs(self) -> int:
     """The number of outputs of the layer tag that this primitive represents."""
     return self._num_outputs
 
   @property
@@ -219,36 +232,35 @@
       all_inputs: Sequence[T],
   ) -> Tuple[
       Tuple[T, ...],
       Tuple[T, ...],
       Tuple[T, ...]
   ]:
     """Splits the operands of the primitive into ``(outputs, inputs, params)``."""
+
     outputs = tuple(all_inputs[:self.num_outputs])
     inputs = tuple(all_inputs[self.num_outputs:self.num_outputs +
                               self.num_inputs])
     params = tuple(all_inputs[self.num_outputs + self.num_inputs:])
+
     return outputs, inputs, params
 
   def get_outputs(self, *operands: Array, **_: Any) -> Array:
     """Extracts the ``outputs`` of a layer from the operands of the primitive."""
     outputs = self.split_all_inputs(operands)[0]
     assert self.num_outputs == len(outputs) == 1
     return outputs[0]
 
-  def _xla_translation(
+  def _mlir_lowering(
       self,
-      xla_context: jax.interpreters.xla.TranslationContext,
-      avals_in: Sequence[core.AbstractValue],
-      avals_out: Sequence[core.AbstractValue],
-      *args: jax.interpreters.xla.XlaOp,
+      context: jax.interpreters.mlir.LoweringRuleContext,
+      *args,
       **_: Any,
-  ) -> Tuple[Array, ...]:
+  ) -> Tuple[Any, ...]:
     """The XLA translation rule for this primitive - returns the ``outputs`` ."""
-    del xla_context, avals_in, avals_out  # not used
     # Need to return a sequence
     return (self.get_outputs(*args),)
 
   @classmethod
   def _transpose(
       cls,
       cotangent: Array,
@@ -281,31 +293,30 @@
 
 
 def generic_get_outputs(
     self: LayerTag,
     *operands: Array,
 ) -> Array:
   """Special logic for generic tag's ``get_outputs``."""
-  # The generic tags have no `inputs` and `outputs` so instead they return just
-  # the parameters.
   assert self.num_inputs == self.num_outputs == 0
   params = self.split_all_inputs(operands)[2]
-  if len(params) != 1:
-    raise ValueError("A generic tag can have only one parameter.")
+
+  # The generic tags have no `inputs` and `outputs` so instead they return just
+  # the first parameter array.
   return params[0]
 
 
 generic = LayerTag(name="generic_tag", num_inputs=0, num_outputs=0)
 setattr(generic, "get_outputs",
         types.MethodType(generic_get_outputs, generic))
 
 
-def register_generic(parameter: Array) -> Array:
+def register_generic(*parameters: Array) -> Array:
   """Registers a generic tag around the provided parameter array."""
-  return generic.bind(parameter)
+  return generic.bind(*parameters)
 
 
 dense = LayerTag(name="dense_tag", num_inputs=1, num_outputs=1)
 
 
 def register_dense(
     y: Array,
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/loss_functions.py` & `kfac-jax-0.0.6/kfac_jax/_src/loss_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """"K-FAC loss functions objects, tags and registration functions."""
 import abc
-from typing import Optional, Sequence, Tuple
+from typing import Dict, Optional, Sequence, Tuple, Type
 
 import distrax
 import jax
 import jax.numpy as jnp
 
 from kfac_jax._src import layers_and_loss_tags as tags
 from kfac_jax._src import utils
 
 
 Array = utils.Array
 Numeric = utils.Numeric
 PRNGKey = utils.PRNGKey
 Shape = utils.Shape
 DType = utils.DType
+LossFunctionInputs = Tuple[Array, ...]
+
+
+# pylint: disable=g-one-element-tuple
 
 
 class LossFunction(utils.Finalizable):
   """Abstract base class for loss functions.
 
   Note that unlike typical loss functions used in neural networks these are
   neither summed nor averaged over the batch and the output of evaluate() will
@@ -41,15 +45,15 @@
 
   def __init__(self, weight: Numeric):
     """Initializes the loss instance.
 
     Args:
       weight: The relative weight attributed to the loss.
     """
-    if not isinstance(weight, (int, float)):
+    if not isinstance(weight, (int, float)) and type(weight) is not object:  # pylint: disable=unidiomatic-typecheck
       if not isinstance(weight, Array) or weight.size > 1:
         raise ValueError("`weight` must be a scalar value.")
     super().__init__()
     self._weight = weight
     self.finalize()
 
   @property
@@ -82,20 +86,37 @@
     """All the parameter independent arrays of the loss."""
 
   @property
   def num_parameter_independants(self) -> int:
     """Number of parameter independent arrays of the loss."""
     return len(self.parameter_independants)
 
-  @abc.abstractmethod
   def copy_with_different_inputs(
       self,
       parameter_dependants: Sequence[Array],
   ) -> "LossFunction":
     """Creates a copy of the loss function object, but with different inputs."""
+    array_args, aux = self.tree_flatten()
+    array_args = (tuple(parameter_dependants) +
+                  tuple(array_args[self.num_parameter_dependants:]))
+    return self.tree_unflatten(aux, array_args)
+
+  @abc.abstractmethod
+  def tree_flatten(
+      self,
+  ) -> Tuple[Tuple[Optional[Array], ...], Dict[str, utils.Numeric]]:
+    pass
+
+  @classmethod
+  def tree_unflatten(
+      cls: Type["LossFunction"],
+      aux_data: Dict[str, utils.Numeric],
+      children: Tuple[Optional[Array], ...],
+  ) -> "LossFunction":
+    return cls(*children, **aux_data)  # pytype: disable=not-instantiable
 
   def evaluate(
       self,
       targets: Optional[Array] = None,
       coefficient_mode: str = "regular",
   ) -> Array:
     """Evaluates the loss function on the targets.
@@ -525,14 +546,15 @@
 
   @property
   def fisher_factor_inner_shape(self) -> Shape:
     return jax.eval_shape(
         lambda: self.sample(rng=jax.random.PRNGKey(0))).shape
 
 
+@jax.tree_util.register_pytree_node_class
 class NormalMeanNegativeLogProbLoss(DistributionNegativeLogProbLoss,
                                     NaturalParamsNegativeLogProbLoss):
   """Loss log prob loss for a normal distribution parameterized by a mean vector.
 
   Note that the covariance is treated as the identity divided by 2.
   Also note that the Fisher for such a normal distribution with respect the mean
   parameter is given by:
@@ -544,30 +566,37 @@
 
   def __init__(
       self,
       mean: Array,
       targets: Optional[Array] = None,
       variance: Numeric = 0.5,
       weight: Numeric = 1.0,
+      normalize_log_prob: bool = True,
   ):
     """Initializes the loss instance.
 
     Args:
       mean: The mean of the normal distribution.
       targets: Optional targets to use for evaluation.
       variance: The scalar variance of the normal distribution.
       weight: The relative weight of the loss.
+      normalize_log_prob: Whether the log prob should include the standard
+        normalization constant for Gaussians (which is additive and depends
+        on the variance).
     """
-    if not isinstance(variance, (int, float)):
+
+    if not isinstance(variance, (int, float)) and type(variance) is not object:  # pylint: disable=unidiomatic-typecheck
       if not isinstance(variance, Array) or variance.size > 1:
         raise ValueError("`variance` must be either a python scalar or a "
                          "scalar array.")
     self._mean = mean
     self._targets = targets
     self._variance = variance
+    self._normalize_log_prob = normalize_log_prob
+
     super().__init__(weight=weight)
 
   @property
   def mean(self) -> Array:
     return self._mean
 
   @property
@@ -575,82 +604,81 @@
     return self._variance
 
   @property
   def targets(self) -> Optional[Array]:
     return self._targets
 
   @property
+  def normalize_log_prob(self) -> bool:
+    return self._normalize_log_prob
+
+  @property
   def parameter_independants(self) -> Tuple[Numeric, ...]:
+
     arrays = (self.variance, self.weight)
+
     if self._targets is not None:
       arrays = (self._targets,) + arrays
+
     return arrays
 
   @property
   def dist(self) -> distrax.MultivariateNormalDiag:
     scale_diag = jnp.full_like(self.mean, jnp.sqrt(self.variance))
     return distrax.MultivariateNormalDiag(loc=self.mean, scale_diag=scale_diag)
 
   @property
   def params(self) -> Tuple[Array]:
     return (self.mean,)
 
-  def copy_with_different_inputs(
-      self,
-      parameter_dependants: Sequence[Array],
-  ) -> "NormalMeanNegativeLogProbLoss":
-    """Creates the same :class:`~LossFunction` object, but with different inputs.
-
-    Args:
-      parameter_dependants: The inputs to use to the constructor of a class
-        instance. This must be a sequence of length 1.
+  def _evaluate(self, targets: Array) -> Array:
 
-    Returns:
-      An instance of :class:`~NormalMeanNegativeLogPorLoss` with the provided
-        inputs.
-    Raises:
-      A ValueError if the ``inputs`` is a sequence of different length than 1.
-    """
-    [mean] = parameter_dependants
-    return NormalMeanNegativeLogProbLoss(
-        mean=mean,
-        targets=self._targets,
-        variance=self._variance,
-        weight=self._weight,
-    )
+    if self.normalize_log_prob:
+      return super()._evaluate(targets)
+    else:
+      # keeps leading dims intact
+      return 0.5 * jnp.sum(jnp.square(
+          self.mean - targets), axis=range(1, targets.ndim)) / self.variance
 
   def multiply_fisher_unweighted(
       self,
       vector: Sequence[Array]
   ) -> Tuple[Array]:
-    return (vector[0] / self._variance,)
+    return (vector[0] / self.variance,)
 
   def multiply_fisher_factor_unweighted(
       self,
       vector: Array,
   ) -> Tuple[Array]:
-    return (vector / jnp.sqrt(self._variance),)
+    return (vector / jnp.sqrt(self.variance),)
 
   def multiply_fisher_factor_transpose_unweighted(
       self,
       vector: Sequence[Array],
   )  -> Array:
     # it's symmetric
     return self.multiply_fisher_factor_unweighted(vector[0])[0]
 
   def multiply_fisher_factor_replicated_one_hot_unweighted(
       self,
       index: Sequence[int],
   ) -> Tuple[Array]:
     index = index[0]
-    ones_slice = jnp.ones([self._mean.shape[0]])[..., None]
-    output_slice = ones_slice / jnp.sqrt(self._variance)
-    return (insert_slice_in_zeros(output_slice, 1, self._mean.shape[1], index),)
+    ones_slice = jnp.ones([self.mean.shape[0]])[..., None]
+    output_slice = ones_slice / jnp.sqrt(self.variance)
+    return (insert_slice_in_zeros(output_slice, 1, self.mean.shape[1], index),)
+
+  def tree_flatten(
+      self,
+  ) -> Tuple[Tuple[Array, Optional[Array]], Dict[str, utils.Numeric]]:
+    aux = dict(variance=self.variance, weight=self.weight)
+    return (self.mean, self.targets), aux
 
 
+@jax.tree_util.register_pytree_node_class
 class NormalMeanVarianceNegativeLogProbLoss(DistributionNegativeLogProbLoss):
   """Negative log prob loss for a normal distribution with mean and variance.
 
   This class parameterizes a multivariate normal distribution with n independent
   dimensions. Unlike :class:`~NormalMeanNegativeLogProbLoss`, this class does
   not assume the variance is held constant. The Fisher Information for n = 1 is
   given by:
@@ -705,34 +733,14 @@
     return distrax.MultivariateNormalDiag(
         loc=self._mean, scale_diag=jnp.sqrt(self._variance))
 
   @property
   def params(self) -> Tuple[Array, Array]:
     return self._mean, self._variance
 
-  def copy_with_different_inputs(
-      self,
-      parameter_dependants: Sequence[Array]
-  ) -> "NormalMeanVarianceNegativeLogProbLoss":
-    """Creates the same :class:`~LossFunction` object, but with different inputs.
-
-    Args:
-      parameter_dependants: The inputs to use to the constructor of a class
-        instance. This must be a sequence of length 2.
-
-    Returns:
-      An instance of :class:`~NormalMeanVarianceNegativeLogProbLoss` with the
-      provided inputs.
-    Raises:
-      A ValueError if the ``inputs`` is a sequence of different length than 2.
-    """
-    [mean, variance] = parameter_dependants
-    return NormalMeanVarianceNegativeLogProbLoss(
-        mean, variance, targets=self._targets, weight=self._weight)
-
   @property
   def _fisher_mean(self) -> Array:
     """The Fisher w.r.t. to the mean parameters."""
     return 1. / self._variance
 
   @property
   def _fisher_mean_factor(self) -> Array:
@@ -823,15 +831,22 @@
   ) -> Tuple[Array, ...]:
     raise NotImplementedError()
 
   @property
   def ggn_factor_inner_shape(self) -> Shape:
     raise NotImplementedError()
 
+  def tree_flatten(
+      self,
+  ) -> Tuple[Tuple[Array, Array, Optional[Array]], Dict[str, utils.Numeric]]:
+    aux = dict(weight=self._weight)
+    return (self._mean, self._variance, self._targets), aux
 
+
+@jax.tree_util.register_pytree_node_class
 class MultiBernoulliNegativeLogProbLoss(DistributionNegativeLogProbLoss,
                                         NaturalParamsNegativeLogProbLoss):
   """Negative log prob loss for multiple Bernoulli distributions parametrized by logits.
 
   Represents N independent Bernoulli distributions where N = len(logits). Its
   Fisher Information matrix is given by ``F = diag(p * (1-p))``, where
   ``p = sigmoid(logits)``.
@@ -877,22 +892,14 @@
     """The probabilities of the underlying Bernoulli distribution."""
     return self.dist.probs  # pytype: disable=bad-return-type
 
   @property
   def params(self) -> Tuple[Array]:
     return (self._logits,)
 
-  def copy_with_different_inputs(
-      self,
-      parameter_dependants: Sequence[Array]
-  ) -> "MultiBernoulliNegativeLogProbLoss":
-    [logits] = parameter_dependants
-    return MultiBernoulliNegativeLogProbLoss(
-        logits, targets=self._targets, weight=self._weight)
-
   def multiply_fisher_unweighted(
       self,
       vector: Sequence[Array]
   ) -> Tuple[Array]:
     return (self._probs * (1 - self._probs) * vector[0],)
 
   def multiply_fisher_factor_unweighted(
@@ -914,15 +921,22 @@
   ) -> Tuple[Array]:
     [index] = index
     probs_slice = self._probs[:, index][..., None]
     output_slice = jnp.sqrt(probs_slice * (1 - probs_slice))
     return (insert_slice_in_zeros(
         output_slice, 1, self._logits.shape[1], index),)
 
+  def tree_flatten(
+      self,
+  ) -> Tuple[Tuple[Array, Optional[Array]], Dict[str, utils.Numeric]]:
+    aux = dict(weight=self._weight)
+    return (self._logits, self._targets), aux
 
+
+@jax.tree_util.register_pytree_node_class
 class CategoricalLogitsNegativeLogProbLoss(DistributionNegativeLogProbLoss,
                                            NaturalParamsNegativeLogProbLoss):
   """Negative log prob loss for a categorical distribution parameterized by logits.
 
 
   Note that the Fisher (for a single case) of a categorical distribution, with
   respect to the natural parameters (i.e. the logits), is given by
@@ -949,18 +963,18 @@
       mask: Optional mask to apply to losses over the batch. Should be
         0/1-valued and of shape ``(batch_size,)``. The tensors returned by
         ``evaluate`` and ``grad_of_evaluate``, as well as the various matrix
         vector products, will be multiplied by mask (with broadcasting to later
         dimensions).
       weight: The relative weight of the loss.
     """
-
-    if mask is not None and mask.shape != logits.shape[:1]:
+    if (mask is not None and type(mask) is not object and  # pylint: disable=unidiomatic-typecheck
+        mask.shape != logits.shape[:-1]):
       raise ValueError("If provided, mask.shape must be equal to "
-                       "logits.shape[:1].")
+                       "logits.shape[:-1].")
 
     self._logits = logits
     self._targets = targets
     self._mask = mask
 
     super().__init__(weight=weight)
 
@@ -970,21 +984,21 @@
 
   @property
   def mask(self) -> Optional[Array]:
     return self._mask
 
   @property
   def parameter_independants(self) -> Tuple[Numeric, ...]:
-    arrays = (self.weight,)
+    arrays: Tuple[Numeric, ...] = (self.weight,)  # pytype: disable=annotation-type-mismatch
 
     if self.mask is not None:
-      arrays = (self.mask,) + arrays
+      arrays: Tuple[Numeric, ...] = (self.mask,) + arrays  # pytype: disable=annotation-type-mismatch
 
     if self.targets is not None:
-      arrays = (self.targets,) + arrays
+      arrays: Tuple[Numeric, ...] = (self.targets,) + arrays  # pytype: disable=annotation-type-mismatch
 
     return arrays
 
   @property
   def dist(self) -> distrax.Categorical:
     return distrax.Categorical(logits=self._logits, dtype=jnp.int32)
 
@@ -1020,52 +1034,47 @@
   def params(self) -> Tuple[Array]:
     return (self._logits,)
 
   @property
   def fisher_factor_inner_shape(self) -> Shape:
     return self._logits.shape
 
-  def copy_with_different_inputs(
-      self,
-      parameter_dependants: Sequence[Array]
-  ) -> "CategoricalLogitsNegativeLogProbLoss":
-
-    [logits] = parameter_dependants
-
-    return CategoricalLogitsNegativeLogProbLoss(
-        logits, targets=self.targets, mask=self.mask, weight=self.weight)
-
   def multiply_fisher_unweighted(
       self,
       vector: Sequence[Array]
   ) -> Tuple[Array]:
 
+    assert len(vector) == 1
+
     probs = self._probs
 
     fisher_product = vector[0] * probs - probs * jnp.sum(
         vector[0] * probs, axis=-1, keepdims=True)
 
     return (fisher_product,)
 
   def multiply_fisher_factor_unweighted(
       self,
       vector: Array
   ) -> Tuple[Array]:
+
     probs = self._probs
 
     sqrt_probs = self._sqrt_probs
 
     return (sqrt_probs * vector - probs * jnp.sum(
         sqrt_probs * vector, axis=-1, keepdims=True),)
 
   def multiply_fisher_factor_transpose_unweighted(
       self,
       vector: Sequence[Array]
   ) -> Array:
 
+    assert len(vector) == 1
+
     probs = self._probs
 
     sqrt_probs = self._sqrt_probs
 
     return sqrt_probs * vector[0] - sqrt_probs * jnp.sum(
         probs * vector[0], axis=-1, keepdims=True)
 
@@ -1079,35 +1088,37 @@
 
     sqrt_probs_slice = self._sqrt_probs[:, index][..., None]
 
     padded_slice = insert_slice_in_zeros(sqrt_probs_slice, 1, probs.shape[1],
                                          index)
     return (padded_slice - probs * sqrt_probs_slice,)
 
+  def tree_flatten(
+      self,
+  ) -> Tuple[
+      Tuple[Array, Optional[Array], Optional[Array]],
+      Dict[str, utils.Numeric]
+  ]:
+    aux = dict(weight=self._weight)
+    return (self._logits, self._targets, self._mask), aux
+
 
+@jax.tree_util.register_pytree_node_class
 class OneHotCategoricalLogitsNegativeLogProbLoss(
     CategoricalLogitsNegativeLogProbLoss):
   """Neg log prob loss for a categorical distribution with onehot targets.
 
   Identical to CategoricalLogitsNegativeLogProbLoss except that the underlying
   distribution is OneHotCategorical as opposed to Categorical.
   """
 
   @property
   def dist(self) -> distrax.OneHotCategorical:
     return distrax.OneHotCategorical(logits=self._logits, dtype=jnp.int32)
 
-  def copy_with_different_inputs(
-      self,
-      parameter_dependants: Sequence[Array]
-  ) -> "OneHotCategoricalLogitsNegativeLogProbLoss":
-    [logits] = parameter_dependants
-    return OneHotCategoricalLogitsNegativeLogProbLoss(
-        logits, targets=self.targets, mask=self.mask, weight=self.weight)
-
 
 def insert_slice_in_zeros(
     slice_to_insert: Array,
     dim: int,
     dim_size: int,
     position: int,
 ) -> Array:
@@ -1152,15 +1163,16 @@
 #    |_|\__,_|\__, | |_|  \_\___|\__, |_|___/\__|_|  \__,_|\__|_|\___/|_| |_|
 #              __/ |              __/ |
 #             |___/              |___/
 
 NormalMeanNegativeLogProbLoss_tag = tags.LossTag(
     NormalMeanNegativeLogProbLoss,
     parameter_dependants=["mean"],
-    parameter_independants=["targets", "variance", "weight"],
+    parameter_independants=["targets", "variance", "weight",
+                            "normalize_log_prob"],
 )
 
 NormalMeanVarianceNegativeLogProbLoss_tag = tags.LossTag(
     NormalMeanVarianceNegativeLogProbLoss,
     parameter_dependants=["mean", "variance"],
     parameter_independants=["targets", "weight"],
 )
@@ -1185,148 +1197,220 @@
 
 
 def register_normal_predictive_distribution(
     mean: Array,
     targets: Optional[Array] = None,
     variance: float = 0.5,
     weight: Numeric = 1.0,
+    normalize_log_prob: bool = True,
 ):
   """Registers a normal predictive distribution.
 
   This corresponds to a squared error loss of the form
-     ``weight/(2*var) * ||target - mean||^2``
+     ``weight/(2*var) * jnp.sum((targets - mean)**2) / batch_size``.
+
+  NOTE: this function assumes you are *not* averaging over non-batch dimensions
+  when computing the loss. e.g. if dimension 0 were the batch dimension, this
+  corresponds to
+  ``jnp.mean(jnp.sum((target - prediction)**2,
+                     axis=range(1,target.ndims)), axis=0)``
+  and not
+  ``jnp.mean((target - prediction)**2)``.
+  If your loss is of the latter form you can compensate for it by passing the
+  appropriate value to ``weight``.
 
   Args:
     mean: A tensor defining the mean vector of the distribution. The first
       dimension will usually be the batch size, but doesn't need to be (unless
       using ``estimation_mode='fisher_exact'`` or
       ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
     targets: (OPTIONAL) The targets for the loss function. Only required if
       using ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
-    variance: float. The variance of the distribution. Note that the default
-      value of 0.5 corresponds to a standard squared error loss weight *
-      ||target - prediction||^2. If you want your squared error loss to be of
-      the form ``0.5*coeff*||target - prediction||^2`` you should use
-      variance=1.0.
-      (Default: 0.5)
-    weight: A scalar coefficient to multiply the log prob loss associated with
-      this distribution. The Fisher will be multiplied by the corresponding
-      factor. In general this is NOT equivalent to changing the temperature of
-      the distribution, but in the ase of normal distributions it may be.
-      (Default: 1.0)
+    variance: The variance of the distribution. Must be a constant scalar,
+      independent of the network's parameters. Note that the default value of
+      0.5 corresponds to a standard squared error loss
+      ``weight * jnp.sum((target - prediction)**2)``. If you want your squared
+      error loss to be of the form
+      ``0.5*coeff*jnp.sum((target - prediction)**2)`` you should use
+      variance=1.0. (Default: 0.5)
+    weight: A constant scalar coefficient that the log prob loss associated with
+      this distribution is multiplied by. In general this is NOT equivalent to
+      changing the temperature of the distribution, but in the case of normal
+      distributions it may be. Note that this must be constant and independent
+      of the network's parameters. (Default: 1.0)
+    normalize_log_prob: Whether the negative log prob loss associated to this
+      this distribution should include the additive normalization constant
+      (which is constant and depends on ``variance``) that makes it a true log
+      prob, and not just a squared error loss. Note that this has no effect on
+      the behavior of optimizer with the exception of in niche situations where
+      the loss value is computed from the registrations. e.g., when
+      ``include_registered_loss_in_stats=True`` is used. (Default: True)
   """
   if targets is None:
-    args = [mean, variance, weight]
-    args_names = ["mean", "variance", "weight"]
+    args = [mean, variance, weight, normalize_log_prob]
+    args_names = ["mean", "variance", "weight", "normalize_log_prob"]
   else:
-    args = [mean, targets, variance, weight]
-    args_names = ["mean", "targets", "variance", "weight"]
+    args = [mean, targets, variance, weight, normalize_log_prob]
+    args_names = ["mean", "targets", "variance", "weight", "normalize_log_prob"]
 
-  NormalMeanNegativeLogProbLoss_tag.bind(*args, args_names=args_names)
+  NormalMeanNegativeLogProbLoss_tag.bind(*args, args_names=tuple(args_names))
 
 
 def register_squared_error_loss(
     prediction: Array,
     targets: Optional[Array] = None,
     weight: Numeric = 1.0,
-) -> Array:
+):
   """Registers a squared error loss function.
 
-  This assumes the squared error loss of the form ``||target - prediction||^2``,
-  averaged across the mini-batch. If your loss uses a coefficient of 0.5
-  you need to set the "weight" argument to reflect this.
+  This assumes a squared error loss of the form
+  ``weight * jnp.sum((targets - prediction)**2) / batch_size``.
+
+  If your loss uses a coefficient of 0.5 you need to set the ``weight`` argument
+  to reflect this.
+
+  NOTE: this function assumes you are *not* averaging over non-batch dimensions
+  when computing the loss. e.g. if dimension 0 were the batch dimension, this
+  corresponds to
+  ``jnp.mean(jnp.sum((target - prediction)**2,
+                     axis=range(1, target.ndims)), axis=0)``
+  and not
+  ``jnp.mean((target - prediction)**2)``
+  If your loss is of the latter form you can compensate for it by passing the
+  appropriate value to ``weight``.
+
+  NOTE: even though ``prediction`` and ``targets`` are interchangeable in the
+  definition of the squared error loss, they are not interchangeable in this
+  function. ``prediction`` must be the output of your parameterized function
+  (e.g. neural network), and ``targets`` must not depend on the parameters.
+  Mixing the two up could lead to a silent failure of the curvature estimation.
 
   Args:
     prediction: The prediction made by the network (i.e. its output). The first
       dimension will usually be the batch size, but doesn't need to be (unless
       using ``estimation_mode='fisher_exact'`` or
       ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
     targets: (OPTIONAL) The targets for the loss function. Only required if
       using ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
-    weight: A float coefficient to multiply the loss function by.
-      (Default: 1.0)
+    weight: The constant scalar coefficient which this loss is multiplied by.
+      Note that this must be constant and independent of the network's
+      parameters. (Default: 1.0)
   """
   register_normal_predictive_distribution(
-      prediction, targets, variance=0.5, weight=weight)  # pytype: disable=bad-return-type  # numpy-scalars
+      prediction, targets, variance=0.5,
+      weight=weight, normalize_log_prob=False)
 
 
 def register_multi_bernoulli_predictive_distribution(
     logits: Array,
     targets: Optional[Array] = None,
     weight: Numeric = 1.0,
 ):
   """Registers a multi-Bernoulli predictive distribution.
 
-  Note that this is distinct from
+  This corresponds to a sigmoid cross-entropy loss of the form
+  ``weight * jnp.sum(sigmoid_cross_entropy(logits, targets)) / batch_size``.
+
+  NOTE: this function assumes you are *not* averaging over non-batch dimensions
+  when computing the loss. e.g. if dimension 0 were the batch dimension, this
+  corresponds to
+  ``jnp.mean(jnp.sum(sigmoid_cross_entropy(logits, targets),
+                     axis=range(1, target.ndims)), axis=0)``
+  and not
+  ``jnp.mean(sigmoid_cross_entropy(logits, targets))``
+  If your loss is of the latter form you can compensate for it by passing the
+  appropriate value to ``weight``.
+
+  NOTE: this is distinct from
   :func:`~register_categorical_predictive_distribution` and should not be
   confused with it.
 
   Args:
     logits: The logits of the distribution (i.e. its parameters) as a 2D array
       of floats. The first dimension will usually be the batch size, but doesn't
       need to be (unless using ``estimation_mode='fisher_exact'`` or
       ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
     targets: (OPTIONAL) The targets for the loss function.  Only required if
       using ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
-    weight: (OPTIONAL) a scalar. A coefficient to multiply the log prob loss
-      associated with this distribution. The Fisher will be multiplied by the
-      corresponding factor. This is NOT equivalent to changing the temperature
-      of the distribution since we don't renormalize the log prob in the
-      objective function. (Default: 1.0)
+    weight: The constant scalar coefficient that the log prob loss associated
+      with this distribution is multiplied by. This is NOT equivalent to
+      changing the temperature of the distribution since we don't renormalize
+      the log prob in the objective function. Note that this must be constant
+      and independent of the network's parameters. (Default: 1.0)
   """
   if targets is None:
     args = [logits, weight]
     args_names = ["logits", "weight"]
   else:
     args = [logits, targets, weight]
     args_names = ["logits", "targets", "weight"]
 
-  MultiBernoulliNegativeLogProbLoss_tag.bind(*args, args_names=args_names)
+  MultiBernoulliNegativeLogProbLoss_tag.bind(
+      *args, args_names=tuple(args_names))
 
 
 def register_sigmoid_cross_entropy_loss(
     logits: Array,
     targets: Optional[Array] = None,
     weight: Numeric = 1.0,
 ):
   """Registers a sigmoid cross-entropy loss function.
 
-  Note that this is distinct from :func:`~register_softmax_cross_entropy_loss`
-  and should not be confused with it. It is similar to
-  :func:`~register_multi_bernoulli_predictive_distribution` but without the
-  explicit probabilistic interpretation. It behaves identically for now.
+  This assumes a sigmoid cross-entropy loss of the form
+  ``weight * jnp.sum(sigmoid_cross_entropy(logits, targets)) / batch_size``.
+
+  NOTE: this function assumes you are *not* averaging over non-batch dimensions
+  when computing the loss. e.g. if dimension 0 were the batch dimension, this
+  corresponds to
+  ``jnp.mean(jnp.sum(sigmoid_cross_entropy(logits, targets),
+                     axis=range(1, target.ndims)), axis=0)``
+  and not
+  ``jnp.mean(sigmoid_cross_entropy(logits, targets))``
+  If your loss is of the latter form you can compensate for this by passing the
+  appropriate value to ``weight``.
+
+  NOTE: this function is distinct from
+  :func:`~register_softmax_cross_entropy_loss` and should not be confused with
+  it. It is similar to :func:`~register_multi_bernoulli_predictive_distribution`
+  but without the explicit probabilistic interpretation. It behaves identically
+  for now.
 
   Args:
     logits: The input logits of the loss as a 2D array of floats. The first
       dimension will usually be the batch size, but doesn't need to be (unless
       using ``estimation_mode='fisher_exact'`` or
       ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
     targets: (OPTIONAL) The targets for the loss function. Must be of the same
       shape as ``logits``. Only required if using
       ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
-    weight: (OPTIONAL) a scalar. A coefficient to multiply the loss function by.
-      (Default: 1.0)
+    weight: The constant scalar coefficient which this loss is multiplied by.
+      Note that this must be constant and independent of the network's
+      parameters. (Default: 1.0)
   """
   register_multi_bernoulli_predictive_distribution(
       logits, targets, weight=weight)
 
 
 def register_categorical_predictive_distribution(
     logits: Array,
     targets: Optional[Array] = None,
     mask: Optional[Array] = None,
     weight: Numeric = 1.0,
 ):
   """Registers a categorical predictive distribution.
 
-  Note that this is distinct from
+  This corresponds to a softmax cross-entropy loss of the form
+
+  ``weight * jnp.sum(softmax_cross_entropy(logits, targets)) / batch_size``.
+
+  NOTE: this is distinct from
   :func:`~register_multi_bernoulli_predictive_distribution` and should not be
   confused with it.
 
   Args:
     logits: The logits of the distribution (i.e. its parameters) as a 2D array
       of floats. The first dimension will usually be the batch size, but doesn't
       need to be (unless using ``estimation_mode='fisher_exact'`` or
@@ -1337,19 +1421,19 @@
       integers with shape ``(logits.shape[0],)``. Only required if using
       ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
     mask: (OPTIONAL) Mask to apply to log probabilities generated by the
       distribution. Should be 0/1-valued and of shape ``(logits.shape[0],)``.
       Log probablities corresponding to mask values of False will be treated
       as constant and equal to 0. (Default: None)
-    weight: (OPTIONAL) a scalar. A coefficient to multiply the
-      log prob loss associated with this distribution. The Fisher will be
-      multiplied by the corresponding factor. This is NOT equivalent to
+    weight: The constant scalar coefficient that the log prob loss associated
+      with this distribution is multiplied by. This is NOT equivalent to
       changing the temperature of the distribution since we don't renormalize
-      the log prob in the objective function. (Default: 1.0)
+      the log prob in the objective function. Note that this must be constant
+      and independent of the network's parameters. (Default: 1.0)
   """
   if targets is not None:
 
     if targets.ndim == logits.ndim:
       tag_cls = OneHotCategoricalLogitsNegativeLogProbLoss_tag
 
     elif targets.ndim == logits.ndim - 1:
@@ -1373,27 +1457,31 @@
   if mask is not None:
     args = args + [mask]
     args_names = args_names + ["mask"]
 
   args = args + [weight]
   args_names = args_names + ["weight"]
 
-  tag_cls.bind(*args, args_names=args_names)
+  tag_cls.bind(*args, args_names=tuple(args_names))
 
 
 def register_softmax_cross_entropy_loss(
     logits: Array,
     targets: Optional[Array] = None,
     mask: Optional[Array] = None,
     weight: Numeric = 1.0,
-) -> Array:
+):
   """Registers a softmax cross-entropy loss function.
 
-  Note that this is distinct from :func:`~register_sigmoid_cross_entropy_loss`
-  and should not be confused with it. It is similar to
+  This assumes a softmax cross-entropy loss of the form
+
+  ``weight * jnp.sum(softmax_cross_entropy(logits, targets)) / batch_size``.
+
+  NOTE:this is distinct from :func:`~register_sigmoid_cross_entropy_loss` and
+  should not be confused with it. It is similar to
   :func:`~register_categorical_predictive_distribution` but without the explicit
   probabilistic interpretation. It behaves identically for now.
 
   Args:
     logits: The input logits of the loss as a 2D array of floats. The first
       dimension will usually be the batch size, but doesn't need to be (unless
       using ``estimation_mode='fisher_exact'`` or
@@ -1402,14 +1490,15 @@
     targets: (OPTIONAL) The targets for the loss function. Must be a 1D array of
       integers with shape ``(logits.shape[0],)``. Only required if using
       ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
     mask: (OPTIONAL) Mask to apply to losses. Should be 0/1-valued and of shape
       ``(logits.shape[0],)``. Losses corresponding to mask values of False will
       be treated as constant and equal to 0. (Default: None)
-    weight: (OPTIONAL) a scalar. A coefficient to multiply the loss function by.
-      (Default: 1.0)
+    weight: The constant scalar coefficient which this loss is multiplied by.
+      Note that this must be constant and independent of the network's
+      parameters. (Default: 1.0)
   """
   register_categorical_predictive_distribution(logits,
                                                targets=targets,
                                                mask=mask,
-                                               weight=weight)  # pytype: disable=bad-return-type  # numpy-scalars
+                                               weight=weight)
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/optimizer.py` & `kfac-jax-0.0.6/kfac_jax/_src/optimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 Params = utils.Params
 Batch = utils.Batch
 FuncState = Any
 # FuncState = utils.FuncState
 FuncAux = utils.FuncAux
 
 OptimizerState: TypeAlias = "Optimizer.State"
-ScheduleType = Callable[[Array], Optional[Array]]
+ScheduleType = Union[Callable[[Numeric, Optional[Numeric]], Numeric],
+                     Callable[[Numeric], Numeric]]
 FuncArgsVariants = Union[
     Tuple[Params, Batch],
     Tuple[Params, FuncState, Batch],
     Tuple[Params, PRNGKey, Batch],
     Tuple[Params, FuncState, PRNGKey, Batch],
 ]
 FuncOutputs = Union[
@@ -108,41 +109,55 @@
       max_damping: Numeric = jnp.inf,
       include_damping_in_quad_change: bool = False,
       damping_adaptation_interval: int = 5,
       damping_adaptation_decay: Numeric = 0.9,
       damping_lower_threshold: Numeric = 0.25,
       damping_upper_threshold: Numeric = 0.75,
       always_use_exact_qmodel_for_damping_adjustment: bool = False,
+      precon_damping_mult: Numeric = 1.0,
       norm_constraint: Optional[Numeric] = None,
       num_burnin_steps: int = 10,
-      estimation_mode: str = "fisher_gradients",
+      estimation_mode: Optional[str] = None,
+      custom_estimator_ctor: Optional[
+          Callable[..., curvature_estimator.BlockDiagonalCurvature]] = None,
       curvature_ema: Numeric = 0.95,
+      curvature_update_period: int = 1,
       inverse_update_period: int = 5,
       use_exact_inverses: bool = False,
       batch_process_func: Optional[Callable[[Batch], Batch]] = None,
       register_only_generic: bool = False,
       patterns_to_skip: Sequence[str] = (),
+      use_automatic_registration: bool = True,
       auto_register_kwargs: Optional[Dict[str, Any]] = None,
-      layer_tag_to_block_ctor:
-      Optional[Dict[str, curvature_estimator.CurvatureBlockCtor]] = None,
+      layer_tag_to_block_ctor: Optional[
+          Dict[str, curvature_estimator.CurvatureBlockCtor]
+      ] = None,
       multi_device: bool = False,
       debug: bool = False,
-      batch_size_extractor: Callable[[Batch], Numeric] =
-      utils.default_batch_size_extractor,
+      batch_size_extractor: Callable[
+          [Batch], Numeric
+      ] = utils.default_batch_size_extractor,
       pmap_axis_name: str = "kfac_axis",
       forbid_setting_attributes_after_finalize: bool = True,
       modifiable_attribute_exceptions: Sequence[str] = (),
       include_norms_in_stats: bool = False,
       include_per_param_norms_in_stats: bool = False,
+      include_registered_loss_in_stats: bool = False,
       distributed_precon_apply: bool = True,
       distributed_inverses: bool = True,
+      num_estimator_samples: int = 1,
+      should_vmap_estimator_samples: bool = False,
+      norm_to_scale_identity_weight_per_block: Optional[str] = None,
   ):
     """Initializes the K-FAC optimizer with the provided settings.
 
-    A note on damping:
+    NOTE: Please read the docstring for this constructor carefully. Especially
+    the description of ``value_and_grad_func``.
+
+    A note on the "damping" parameter:
 
     One of the main complications of using second-order optimizers like K-FAC is
     the "damping" parameter. This parameter is multiplied by the identity matrix
     and (approximately) added to the curvature matrix (i.e. the Fisher or GGN)
     before it is inverted and multiplied by the gradient when computing the
     update (before any learning rate scaling). The damping should follow the
     scale of the objective, so that if you multiply your loss by some factor you
@@ -151,35 +166,41 @@
     in general since the second-order approximations that underly second-order
     methods can break down for large updates. (In gradient descent the learning
     rate plays an analogous role.) The relationship between the damping
     parameter and the radius of this region is complicated and depends on the
     scale of the objective amongst other things.
 
     The optimizer provides a system for adjusting the damping automatically via
-    the ``use_adaptive_damping`` argument, although this system is not
-    completely reliable. Using a fixed value or a manually tuned schedule can
-    work as good or better for some problems, while it can be a very poor choice
-    for others (like deep autoencoders). Empirically we have found that using
-    a fixed value works well enough for common architectures like convnets and
-    transformers.
+    the ``use_adaptive_damping`` argument, although this system is not reliable,
+    especially for highly stochastic objectives. Using a fixed value or a
+    manually tuned schedule can work as good or better for some problems, while
+    it can be a very poor choice for others (like deep autoencoders).
+    Empirically we have found that using a fixed value works well enough for
+    common architectures like convnets and transformers.
 
     Args:
-      value_and_grad_func: Python callable. The function should return the value
-        of the loss to be optimized and its gradients, and optionally the model
-        state and auxiliary information (usually statistics to log). The
-        interface should be: ``out_args, loss_grads =
+      value_and_grad_func: Python callable. This function should return the
+        value of the loss to be optimized and its gradients, and optionally the
+        model state and auxiliary information in the form of a a dict mapping
+        strings to scalar arrays (usually statistics to log). Note that it
+        should *not* be jitted/pmapped or otherwise compiled by JAX, as this can
+        lead to errors. (Compilation is done internally by the optimizer.) The
+        interface of this function should be: ``out_args, loss_grads =
         value_and_grad_func(*in_args)``. Here, ``in_args`` is ``(params,
         func_state, rng, batch)``, with ``rng`` omitted if
         ``value_func_has_rng`` is ``False``, and with ``func_state`` omitted if
         ``value_func_has_state`` is ``False``. Meanwhile, ``out_args`` is
-        ``(loss, func_state, aux)``, with ``func_state`` omitted if
-        ``value_func_has_state`` is ``False``, and with ``aux`` omitted if
-        ``value_func_has_aux`` is ``False``. If both ``value_func_has_state``
-        and ``value_func_has_aux`` are ``False``, ``out_args`` should just be
-        ``loss`` and not ``(loss,)``.
+        ``(loss, (func_state, aux))`` if ``value_func_has_state`` and
+        ``value_func_has_aux`` are both ``True``, ``(loss, func_state)`` if
+        ``value_func_has_state`` is ``True`` and ``value_func_has_aux`` is
+        ``False``, ``(loss, aux)`` if ``value_func_has_state`` is ``False`` and
+        ``value_func_has_aux`` is ``True``, and finally ``loss`` if
+        ``value_func_has_state`` and ``value_func_has_aux`` are both ``False``.
+        This should be consistent with how JAX's ``value_and_grad`` API function
+        is typically used.
       l2_reg: Scalar. Set this value to tell the optimizer what L2
         regularization coefficient you are using (if any). Note the coefficient
         appears in the regularizer as ``coeff / 2 * sum(param**2)``. This adds
         an additional diagonal term to the curvature and hence will affect the
         quadratic model when using adaptive damping. Note that the user is still
         responsible for adding regularization to the loss.
       value_func_has_aux: Boolean. Specifies whether the provided callable
@@ -193,35 +214,38 @@
       use_adaptive_learning_rate: Boolean. Specifies whether to use the special
         rule from the original K-FAC paper for picking the learning rate at each
         step. Note that this won't work well for stochastic objectives. If this
         is ``False``, the user must use the ``learning_rate`` argument of the
         step function, or the constructor argument ``learning_rate_schedule``.
         (Default: ``False``)
       learning_rate_schedule: Callable. A schedule for the learning rate. This
-        should take as input the current step number and return a single array
-        that represents the learning rate. (Default: ``None``)
-      use_adaptive_momentum: Boolean. Specifies whether to use the special
-        rule from the original K-FAC paper for picking the momentum "decay"
-        parameter at each step. Note that this won't work well for stochastic
-        bjectives. If this is ``False``, the user must use the ``momentum``
-        argument of the step function, or the constructor argument
-        ``momentum_schedule``. (Default: ``False``)
+        should take as input the current step number, and optionally the amount
+        of data seen so far as a keyword argument ``data_seen``, and return a
+        single array that represents the learning rate. (Default: ``None``)
+      use_adaptive_momentum: Boolean. Specifies whether to use the special rule
+        from the original K-FAC paper for picking the momentum "decay" parameter
+        at each step. Note that this won't work well for stochastic objectives.
+        If this is ``False``, the user must use the ``momentum`` argument of the
+        step function, or the constructor argument ``momentum_schedule``.
+        (Default: ``False``)
       momentum_schedule: Callable. A schedule for the momentum parameter. This
-        should take as input the current step number and return a single array
-        that represents the momentum. (Default: ``None``)
+        should take as input the current step number, and optionally the amount
+        of data seen so far as a keyword argument ``data_seen``, and return a
+        single array that represents the momentum. (Default: ``None``)
       use_adaptive_damping: Boolean. Specifies whether the optimizer will use
         the Levenberg-Marquardt method to automatically adjust the damping every
         ``damping_adaptation_interval`` iterations. If this is set to ``False``
         the user must provide a value to the damping argument of the step
         function at each iteration, or use the ``damping_schedule`` constructor
         argument. Note that the effectiveness of this technique seems to vary
         between problems. (Default: ``False``)
       damping_schedule: Callable. A schedule for the damping. This should take
-        as input the current step number and return a single array that
-        represents the learning rate. (Default: ``None``)
+        as input the current step number, and optionally the amount of data seen
+        so far as a keyword argument ``data_seen``, and return a single array
+        that represents the learning rate. (Default: ``None``)
       initial_damping: Scalar or None. This specifies the initial value of the
         damping that the optimizer will use when using automatic damping
         adaptation. (Default: ``None``)
       min_damping: Scalar. Minimum value the damping parameter can take when
         using automatic damping adaptation. Note that the default value of 1e-8
         is quite arbitrary, and you may have to adjust this up or down for your
         particular problem. If you are using a non-zero value of l2_reg you
@@ -247,62 +271,74 @@
         learning rate and/or momentum adaptation, the quadratic model change
         used for damping adaption is always computed using the exact curvature
         matrix. Otherwise, there is an option to use either the exact or
         approximate curvature matrix to compute the quadratic model change,
         which is what this argument controls. When True, the exact curvature
         matrix will be used, which is more expensive, but could possibly produce
         a better damping schedule. (Default: ``False``)
+      precon_damping_mult: Scalar. Multiplies the damping used in the
+        preconditioner (vs the exact quadratic model) by this value.
+        (Default: 1.0)
       norm_constraint: Scalar. If specified, the update is scaled down so that
         its approximate squared Fisher norm ``v^T F v`` is at most the specified
         value. (Note that here ``F`` is the approximate curvature matrix, not
         the exact.) May only be used when ``use_adaptive_learning_rate`` is
         ``False``. (Default: ``None``)
       num_burnin_steps: Int. At the start of optimization, e.g. the first step,
         before performing the actual step the optimizer will perform this many
         times updates to the curvature approximation without updating the actual
         parameters. (Default: ``10``)
       estimation_mode: String. The type of estimator to use for the curvature
         matrix. See the documentation for :class:`~CurvatureEstimator` for a
-        detailed description of the possible options. (Default:
-        ``fisher_gradients``).
+        detailed description of the possible options. If ``None`` will use
+        default estimation_mode mode of the used CurvatureEstimator subclass,
+        which is typically "fisher_gradients". (Default: ``None``)
+      custom_estimator_ctor: Optional constructor for subclass of
+        :class:`~BlockDiagonalCurvature`. If specified, the optimizer will use
+        this conastructor instead of the default
+        :class:`~BlockDiagonalCurvature`. (Default: ``None``)
       curvature_ema: The decay factor used when calculating the covariance
         estimate moving averages. (Default: ``0.95``)
+      curvature_update_period: Int. The number of steps in between updating the
+        the curvature estimates. (Default: ``1``)
       inverse_update_period: Int. The number of steps in between updating the
         the computation of the inverse curvature approximation. (Default: ``5``)
       use_exact_inverses: Bool. If ``True``, preconditioner inverses are
         computed "exactly" without the pi-adjusted factored damping approach.
         Note that this involves the use of eigendecompositions, which can
         sometimes be much more expensive. (Default: ``False``)
       batch_process_func: Callable. A function which to be called on each batch
         before feeding to the KFAC on device. This could be useful for specific
         device input optimizations. (Default: ``None``)
       register_only_generic: Boolean. Whether when running the auto-tagger to
         register only generic parameters, or allow it to use the graph matcher
         to automatically pick up any kind of layer tags. (Default: ``False``)
       patterns_to_skip: Tuple. A list of any patterns that should be skipped by
         the graph matcher when auto-tagging. (Default: ``()``)
+      use_automatic_registration: Bool. If ``True``, the optimizer will try to
+        automatically register the layers of your network. (Default: ``True``)
       auto_register_kwargs: Any additional kwargs to be passed down to
         :func:`~auto_register_tags`, which is called by the curvature estimator.
         (Default: ``None``)
       layer_tag_to_block_ctor: Dictionary. A mapping from layer tags to block
         classes which to override the default choices of block approximation for
         that specific tag. See the documentation for
         :class:`~CurvatureEstimator` for a more detailed description. (Default:
         ``None``)
       multi_device: Boolean. Whether to use pmap and run the optimizer on
         multiple devices. (Default: ``False``)
       debug: Boolean. If neither the step or init functions should be jitted.
         Note that this also overrides ``multi_device`` and prevents using pmap.
         (Default: ``False``)
       batch_size_extractor: A function that takes as input the function
-        arguments and returns the batch size for a single device.
-        (Default: ``kfac.utils.default_batch_size_extractor``)
+        arguments and returns the batch size for a single device. (Default:
+        ``kfac.utils.default_batch_size_extractor``)
       pmap_axis_name: String. The name of the pmap axis to use when
         ``multi_device`` is set to True. (Default: ``kfac_axis``)
-      forbid_setting_attributes_after_finalize: Boolean. By default after the
+      forbid_setting_attributes_after_finalize: Boolean. By default, after the
         object is finalized, you can not set any of its properties. This is done
         in order to protect the user from making changes to the object
         attributes that would not be picked up by various internal methods after
         they have been compiled. However, if you are extending this class, and
         clearly understand the risks of modifying attributes, setting this to
         ``False`` will remove the restriction. (Default: ``True``)
       modifiable_attribute_exceptions: Sequence of strings. Gives a list of
@@ -312,24 +348,42 @@
       include_norms_in_stats: Boolean. It True, the vector norms of the
         gradient, preconditioned gradient, and parameter update are included in
         the statistics returned by the step function. (Default: ``False``)
       include_per_param_norms_in_stats: Boolean. It True, the per-parameter
         vector norms of the gradient, preconditioned gradient, and parameter
         update are included in the statistics returned by the step function.
         (Default: ``False``)
+      include_registered_loss_in_stats: Boolean. If True, we include the loss,
+        as computed from the registered losses, in the stats. Also included is
+        the relative difference between this as the loss computed from
+        ``value_and_grad_func``. This is useful for debugging registration
+        errors. Note this for this option to work it's required that the targets
+        are passed for each loss function registration. (Default: ``False``)
       distributed_precon_apply: Boolean. Whether to distribute the application
         of the preconditioner across the different devices in a layer-wise
         fashion. If False, each device will (redundantly) perform the required
-        operations for all of the layers. (Default: True)
+        operations for all the layers. (Default: True)
       distributed_inverses: Boolean. Whether to distribute the inverse
         computations (required to compute the preconditioner) across the
         different devices in a layer-wise fashion. If False, each device will
-        (redundantly) perform the required computations for all of the layers.
+        (redundantly) perform the required computations for all the layers.
         (Default: True)
+      num_estimator_samples: Number of samples (per case) to use when computing
+        stochastic curvature matrix estimates. This option is only used when
+        ``estimation_mode == 'fisher_gradients'`` or ``estimation_mode ==
+        '[fisher,ggn]_curvature_prop'``. (Default: 1)
+      should_vmap_estimator_samples: Whether to use ``jax.vmap`` to compute
+        samples when ``num_estimator_samples > 1``. (Default: False)
+      norm_to_scale_identity_weight_per_block: The name of a norm to use to
+        compute extra per-block scaling for the damping. See psd_matrix_norm()
+        in utils/math.py for the definition of these. Note that this will not
+        affect the exact quadratic model that is used as part of the "adaptive"
+        learning rate, momentum, and damping methods. (Default: None)
     """
+
     super().__init__(
         multi_device=multi_device,
         pmap_axis_name=pmap_axis_name if multi_device else None,
         debug=debug,
         forbid_setting_attributes_after_finalize=
         forbid_setting_attributes_after_finalize,
         excluded_attribute_names=modifiable_attribute_exceptions,
@@ -353,26 +407,33 @@
 
     self._value_and_grad_func = value_and_grad_func
     self._value_func_has_aux = value_func_has_aux
     self._value_func_has_state = value_func_has_state
     self._value_func_has_rng = value_func_has_rng
     self._value_func: ValueFunc = convert_value_and_grad_to_value_func(
         value_and_grad_func,
-        has_aux=value_func_has_aux,
+        has_aux=value_func_has_aux or value_func_has_state,
     )
-    self._l2_reg = jnp.asarray(l2_reg)
+    self._l2_reg = l2_reg
     self._use_adaptive_learning_rate = use_adaptive_learning_rate
     self._learning_rate_schedule = learning_rate_schedule
     self._use_adaptive_momentum = use_adaptive_momentum
 
     if momentum_schedule is not None:
 
-      def schedule_with_first_step_zero(global_step: Array) -> Array:
-        value = momentum_schedule(global_step)
+      # TODO(jamesmartens,botev): invesigate if we actually need this anymore.
+      def schedule_with_first_step_zero(
+          global_step: Array,
+          data_seen: Optional[Numeric] = None,
+      ) -> Array:
+
+        value = utils.call_func_with_conditional_kwargs(
+            momentum_schedule, global_step, data_seen=data_seen)
         check = jnp.equal(global_step, 0)
+
         return check * jnp.zeros_like(value) + (1 - check) * value
 
       self._momentum_schedule = schedule_with_first_step_zero
 
     else:
       self._momentum_schedule = None
 
@@ -384,60 +445,87 @@
     self._include_damping_in_quad_change = include_damping_in_quad_change
     self._damping_adaptation_decay = damping_adaptation_decay
     self._damping_adaptation_interval = damping_adaptation_interval
     self._damping_lower_threshold = damping_lower_threshold
     self._damping_upper_threshold = damping_upper_threshold
     self._always_use_exact_qmodel_for_damping_adjustment = (
         always_use_exact_qmodel_for_damping_adjustment)
+    self._precon_damping_mult = precon_damping_mult
     self._norm_constraint = norm_constraint
     self._num_burnin_steps = num_burnin_steps
-    self._estimation_mode = estimation_mode
     self._curvature_ema = curvature_ema
+    if curvature_update_period > inverse_update_period:
+      raise ValueError(
+          "curvature_update_period ({}) cannot be larger than"
+          " inverse_update_period ({}) as the identical matrix inversion would"
+          " be redundantly performed. Set inverse_update_period larger instead."
+          .format(curvature_update_period, inverse_update_period)
+      )
+    self._curvature_update_period = curvature_update_period
     self._inverse_update_period = inverse_update_period
     self._register_only_generic = register_only_generic
     self._layer_tag_to_block_cls = layer_tag_to_block_ctor
     self._patterns_to_skip = patterns_to_skip
     self._batch_process_func = batch_process_func or (lambda x: x)
     self._include_norms_in_stats = include_norms_in_stats
     self._include_per_param_norms_in_stats = include_per_param_norms_in_stats
+    self._include_registered_loss_in_stats = include_registered_loss_in_stats
     self._batch_size_extractor = batch_size_extractor
 
     self._use_cached_inverses = (self._inverse_update_period != 1)
     self._use_exact_inverses = use_exact_inverses
 
+    self._norm_to_scale_identity_weight_per_block = (
+        norm_to_scale_identity_weight_per_block
+    )
+
+    self._params_index = 0
+
+    if (norm_to_scale_identity_weight_per_block is not None
+        and norm_to_scale_identity_weight_per_block != "none"):
+
+      assert (not use_adaptive_learning_rate and not use_adaptive_momentum
+              and not use_adaptive_damping)  # not currently supported
+
+    estimator_ctor = (
+        custom_estimator_ctor or curvature_estimator.BlockDiagonalCurvature)
+
     # Curvature estimator
-    self._estimator = curvature_estimator.BlockDiagonalCurvature(
+    self._estimator = estimator_ctor(
         func=self._value_func,
         default_estimation_mode=estimation_mode,
-        params_index=0,
+        params_index=self._params_index,
         layer_tag_to_block_ctor=layer_tag_to_block_ctor,
         register_only_generic=register_only_generic,
         patterns_to_skip=patterns_to_skip,
         distributed_multiplies=distributed_precon_apply,
         distributed_cache_updates=distributed_inverses,
+        num_samples=num_estimator_samples,
+        should_vmap_samples=should_vmap_estimator_samples,
+        auto_register_tags=use_automatic_registration,
         **(auto_register_kwargs or {}),
     )
     self._implicit = curvature_estimator.ImplicitExactCurvature(
         self._value_func,
-        params_index=0,
+        params_index=self._params_index,
         batch_size_extractor=batch_size_extractor,
     )
 
     # Each subclass should call finalize on its own, so this gets called only
     # for instances of exactly this class type.
     if type(self) == Optimizer:  # pylint: disable=unidiomatic-typecheck
       self.finalize()
 
   @property
   def num_burnin_steps(self) -> int:
     """The number of burnin steps to run before the first parameter update."""
     return self._num_burnin_steps
 
   @property
-  def l2_reg(self) -> Array:
+  def l2_reg(self) -> Numeric:
     """The weight of the additional diagonal term added to the curvature."""
     return self._l2_reg
 
   @property
   def estimator(self) -> curvature_estimator.BlockDiagonalCurvature:
     """The underlying curvature estimator used by the optimizer."""
     return self._estimator
@@ -464,14 +552,39 @@
   def should_update_damping(
       self,
       state: "Optimizer.State",
   ) -> Array:
     """Whether at the current step the optimizer should update the damping."""
     return (state.step_counter + 1) % self._damping_adaptation_interval == 0
 
+  def should_update_estimate_curvature(
+      self, state: "Optimizer.State"
+  ) -> Union[Array, bool]:
+    """Whether at the current step the optimizer should update the curvature estimates."""
+    if self._curvature_update_period == 1:
+      return True
+    return state.step_counter % self._curvature_update_period == 0
+
+  def should_update_inverse_cache(
+      self, state: "Optimizer.State"
+  ) -> Union[Array, bool]:
+    """Whether at the current step the optimizer should update the inverse curvature approximation."""
+    return self._use_cached_inverses and (
+        state.step_counter % self._inverse_update_period == 0)
+
+  def should_sync_estimator(
+      self, state: "Optimizer.State"
+  ) -> Union[Array, bool]:
+    """Whether at the current step the optimizer should update the inverse curvature approximation."""
+
+    if self._use_cached_inverses:
+      return self.should_update_inverse_cache(state)
+
+    return True
+
   @functools.partial(utils.staged, static_argnums=1)
   def _rng_split(
       self,
       rng: PRNGKey,
       num: int,
   ) -> Tuple[Array, ...]:
     """Splits the ``rng`` key."""
@@ -545,30 +658,35 @@
 
   @utils.staged
   def _setup_state_and_schedules(
       self,
       learning_rate: Optional[Array],
       momentum: Optional[Array],
       damping: Optional[Array],
-      step_counter: Array
+      step_counter: Array,
+      data_seen: Array,
   ) -> Tuple[Optional[Array], Optional[Array], Array]:
     """Helper function for setting up learning rate, momentum and damping."""
 
     # Compute schedules if applicable
     if self._learning_rate_schedule is not None:
+
       assert learning_rate is None
-      learning_rate = self._learning_rate_schedule(step_counter)
+      learning_rate = utils.call_func_with_conditional_kwargs(
+          self._learning_rate_schedule, step_counter, data_seen=data_seen)
 
     if self._momentum_schedule is not None:
       assert momentum is None
-      momentum = self._momentum_schedule(step_counter)
+      momentum = utils.call_func_with_conditional_kwargs(
+          self._momentum_schedule, step_counter, data_seen=data_seen)
 
     if self._damping_schedule is not None:
       assert damping is None
-      damping = self._damping_schedule(step_counter)
+      damping = utils.call_func_with_conditional_kwargs(
+          self._damping_schedule, step_counter, data_seen=data_seen)
 
     else:
       assert damping is not None
 
     return learning_rate, momentum, damping
 
   def _setup_func_args_and_rng(
@@ -596,112 +714,161 @@
         batch=batch,
         has_state=self._value_func_has_state,
         has_rng=self._value_func_has_rng,
     )
 
     return func_args, rng
 
+  def _maybe_update_estimator_state(
+      self,
+      state: "Optimizer.State",
+      should_update: Union[Array, bool],
+      update_func: Callable[
+          ..., curvature_estimator.BlockDiagonalCurvature.State
+      ],
+      **update_func_kwargs,
+  ) -> "Optimizer.State":
+    """Updates the estimator state if it is the right iteration."""
+
+    # Copy this first since we mutate it later in this function.
+    state = state.copy()
+
+    state.estimator_state = lax.cond(
+        should_update,
+        functools.partial(update_func, **update_func_kwargs),
+        lambda state_: state_,
+        state.estimator_state,
+    )
+    return state
+
   def _update_estimator_curvature(
       self,
       estimator_state: curvature_estimator.BlockDiagonalCurvature.State,
       func_args: FuncArgsVariants,
       rng: PRNGKey,
       ema_old: Numeric,
       ema_new: Numeric,
+      sync: Union[Array, bool] = True
   ) -> curvature_estimator.BlockDiagonalCurvature.State:
     """Updates the curvature estimator state."""
 
-    return self.estimator.update_curvature_matrix_estimate(
+    state = self.estimator.update_curvature_matrix_estimate(
         state=estimator_state,
         ema_old=ema_old,
         ema_new=ema_new,
         # Note that the batch is always the last entry of FuncArgsVariantsdef
         batch_size=self._batch_size_extractor(func_args[-1]),
         rng=rng,
         func_args=func_args,
-        pmap_axis_name=self.pmap_axis_name
+    )
+    return jax.lax.cond(
+        sync,
+        functools.partial(self.estimator.sync,
+                          pmap_axis_name=self.pmap_axis_name),
+        lambda state_: state_,
+        state,
+    )
+
+  def _maybe_update_estimator_curvature(
+      self,
+      state: "Optimizer.State",
+      func_args: FuncArgsVariants,
+      rng: PRNGKey,
+      ema_old: Numeric,
+      ema_new: Numeric,
+      sync: Union[Array, bool] = True,
+  ) -> "Optimizer.State":
+    """Updates the curvature estimates if it is the right iteration."""
+    return self._maybe_update_estimator_state(
+        state,
+        self.should_update_estimate_curvature(state),
+        self._update_estimator_curvature,
+        func_args=func_args,
+        rng=rng,
+        ema_old=ema_old,
+        ema_new=ema_new,
+        sync=sync,
     )
 
   @utils.auto_scope_method
   def _compute_loss_and_grads(
       self,
       func_args: FuncArgsVariants,
-  ) -> Tuple[Array, Params, FuncState, FuncAux]:
+      state: Optional["Optimizer.State"] = None,
+  ) -> Tuple[Array, Params, Optional[FuncState], Optional[FuncAux]]:
     """Computes the model loss value and its gradients."""
 
+    del state
+
     out, grads = self._value_and_grad_func(*func_args)
 
     loss, func_state, aux = extract_func_outputs(
         out, self._value_func_has_aux, self._value_func_has_state)
 
-    return loss, grads, func_state, aux
+    if self._include_registered_loss_in_stats:
+      aux = aux or {}
+      aux["loss_registered"] = self.compute_loss_from_registrations(func_args)
+
+    return loss, grads, func_state, aux  # pytype: disable=bad-return-type
 
   def _maybe_update_inverse_cache(
       self,
       state: "Optimizer.State",
       damping: Array,
   ) -> "Optimizer.State":
     """Updates the estimator state cache if it is the right iteration."""
-
-    # Copy this first since we mutate it later in this function.
-    state = state.copy()
-
-    state.estimator_state = lax.cond(
-        state.step_counter % self._inverse_update_period == 0,
-        functools.partial(
-            self.estimator.update_cache,
-            identity_weight=self.l2_reg + damping,
-            exact_powers=self._exact_powers_to_cache,
-            approx_powers=self._approx_powers_to_cache,
-            eigenvalues=False,
-            pmap_axis_name=self.pmap_axis_name,
-        ),
-        lambda state_: state_,
-        state.estimator_state
+    return self._maybe_update_estimator_state(
+        state,
+        self.should_update_inverse_cache(state),
+        self.estimator.update_cache,
+        identity_weight=self.l2_reg + damping,
+        exact_powers=self._exact_powers_to_cache,
+        approx_powers=self._approx_powers_to_cache,
+        eigenvalues=False,
+        pmap_axis_name=self.pmap_axis_name,
     )
-    return state
 
-  # TODO(jamesmartens, botev): It's ugly that this method implements the norm
-  # constraint on top of computing the preconditioned gradient. Should refactor.
   @utils.staged
   def _compute_preconditioned_gradient(
       self,
       state: "Optimizer.State",
       grads: Params,
-      coefficient: Optional[Array],
       damping: Array,
-  ) -> Tuple[Params, Optional[Array]]:
-    """Computes the preconditioned gradient, maybe applying norm-constraint."""
+  ) -> Params:
+    """Computes the preconditioned gradient."""
 
-    preconditioned_grads = self.estimator.multiply_inverse(
+    return self.estimator.multiply_inverse(
         state=state.estimator_state,
         parameter_structured_vector=grads,
-        identity_weight=self.l2_reg + damping,
+        identity_weight=(self.l2_reg + damping) * self._precon_damping_mult,
         exact_power=self._use_exact_inverses,
         use_cached=self._use_cached_inverses,
         pmap_axis_name=self.pmap_axis_name,
+        norm_to_scale_identity_weight_per_block=self._norm_to_scale_identity_weight_per_block,
     )
 
-    if self._norm_constraint is not None:
-
-      assert not self._use_adaptive_learning_rate
-      assert coefficient is not None
+  @utils.staged
+  def _maybe_apply_norm_constraint(
+      self, grads: Params, preconditioned_grads: Params, coefficient: Array
+  ) -> Tuple[Params, Optional[Params]]:
+    """Scales precon grad to have F-weighted norm <= norm_constraint."""
+    if self._norm_constraint is None:
+      return preconditioned_grads, None
 
-      sq_norm_grads = utils.inner_product(preconditioned_grads, grads)
+    assert not self._use_adaptive_learning_rate
 
-      sq_norm_scaled_grads = sq_norm_grads * coefficient ** 2
+    sq_norm_grads = utils.inner_product(preconditioned_grads, grads)
+    sq_norm_scaled_grads = sq_norm_grads * coefficient ** 2
 
-      max_coefficient = jnp.sqrt(self._norm_constraint / sq_norm_scaled_grads)
-      coefficient = jnp.minimum(max_coefficient, 1)
+    max_coefficient = jnp.sqrt(self._norm_constraint / sq_norm_scaled_grads)
+    coefficient = jnp.minimum(max_coefficient, 1)
 
-      preconditioned_grads = utils.scalar_mul(preconditioned_grads, coefficient)
-    else:
-      sq_norm_scaled_grads = None
+    precon_grad = utils.scalar_mul(preconditioned_grads, coefficient)
 
-    return preconditioned_grads, sq_norm_scaled_grads
+    return precon_grad, sq_norm_scaled_grads
 
   def _compute_quad_change_for_damping(
       self,
       state: "Optimizer.State",
       delta: Params,
       grads: Params,
       damping: Array,
@@ -709,45 +876,46 @@
   ) -> Array:
     """The quadratic model change, when lr and momentum are non-adaptive."""
 
     assert not (self._use_adaptive_learning_rate or self._use_adaptive_momentum)
 
     if self._always_use_exact_qmodel_for_damping_adjustment:
       quad_model = self.compute_exact_quad_model(
-          [delta], grads, func_args)
+          [delta], grads, func_args, state=state)
     else:
       quad_model = self.compute_approx_quad_model(state, [delta], grads)
 
     w = jnp.ones([])
     return self._solve_quad_model(quad_model, damping, [delta], [w])[1]
 
   def _coefficients_and_quad_change(
       self,
       state: "Optimizer.State",
       vectors: Sequence[Params],
       grads: Params,
       learning_rate: Optional[Array],
       momentum: Optional[Array],
       damping: Array,
-      func_args: Optional[FuncArgsVariants] = None,
+      func_args: FuncArgsVariants,
   ) -> Tuple[Tuple[Optional[Array], Optional[Array]], Array]:
     """The correct update coefficients and corresponding quadratic change."""
 
     # Compute the coefficients of the update vectors
     # The learning rate is defined as the negative of the coefficient by which
     # we multiply the gradients, while the momentum is the coefficient by
     # which we multiply the velocities.
-    neg_learning_rate = - learning_rate if learning_rate is not None else None
+    neg_learning_rate = -learning_rate if learning_rate is not None else None
     coefficients = (neg_learning_rate, momentum)
 
     if self._use_adaptive_learning_rate or self._use_adaptive_momentum:
 
-      quad_model = self.compute_exact_quad_model(vectors, grads, func_args)
-
+      quad_model = self.compute_exact_quad_model(vectors, grads, func_args,
+                                                 state=state)
       return self._solve_quad_model(quad_model, damping, vectors, coefficients)
+
     else:
       assert all(c is not None for c in coefficients)
 
       if self._use_adaptive_damping:
         delta = self.weighted_sum_of_objects(vectors, coefficients)
 
         quad_change = lax.cond(
@@ -756,15 +924,33 @@
             lambda args: jnp.nan,
             (state, delta, grads, damping, func_args),
         )
 
       else:
         quad_change = jnp.nan
 
-      return coefficients, quad_change
+      return coefficients, quad_change  # pytype: disable=bad-return-type  # jnp-type
+
+  @utils.staged
+  def compute_loss_from_registrations(
+      self,
+      func_args: FuncArgsVariants
+  ) -> Array:
+
+    loss = self.estimator.compute_func_from_registered(
+        func_args, self._batch_size_extractor(func_args[-1]))
+
+    if self.l2_reg > 0.0:
+
+      l2_reg_val = self.l2_reg / 2 * utils.squared_norm(
+          func_args[self._params_index])
+
+      loss += l2_reg_val
+
+    return loss
 
   @utils.auto_scope_method
   def _update_damping(
       self,
       old_damping: Array,
       old_loss: Array,
       quad_change: Array,
@@ -788,14 +974,17 @@
       params: Params,
       rng: PRNGKey,
       batch: Batch,
       func_state: Optional[FuncState] = None,
   ) -> "Optimizer.State":
     """A staged function to initialize the optimizer state ."""
 
+    # Note that we can reuse the ng in the func_args construction below, as
+    # these are just dummy values used to perform the tracing.
+
     return Optimizer.State(
         velocities=jax.tree_util.tree_map(jnp.zeros_like, params),
         estimator_state=self.estimator.init(
             rng=rng,
             func_args=make_func_args(
                 params=params,
                 func_state=func_state,
@@ -832,27 +1021,28 @@
   def _burnin(
       self,
       params: Params,
       state: "Optimizer.State",
       rng: Array,
       batch: Batch,
       func_state: Optional[FuncState],
-      accumulator: utils.MultiChunkAccumulator
+      accumulator: utils.MultiChunkAccumulator,
+      sync: Union[Array, bool],
   ) -> Tuple["Optimizer.State", utils.MultiChunkAccumulator]:
     """A single burnin step, updating only the curvature estimate."""
 
     # Copy this first since we mutate it later in this function.
     accumulator = accumulator.copy()
 
     func_args, rng = self._setup_func_args_and_rng(
         params, rng, batch, func_state)
 
     # Update curvature estimate
     state.estimator_state = self._update_estimator_curvature(
-        state.estimator_state, func_args, rng, 1.0, 1.0)
+        state.estimator_state, func_args, rng, 1.0, 1.0, sync=sync)
 
     # Optionally update func_state
     if func_state is not None:
       out, _ = self._value_and_grad_func(*func_args)
       _, func_state, _ = extract_func_outputs(
           out, self._value_func_has_aux, self._value_func_has_state)
 
@@ -868,24 +1058,26 @@
       rng: PRNGKey,
       data_iterator: Iterator[Batch],
       func_state: Optional[FuncState] = None,
   ) -> Tuple["Optimizer.State", Optional[FuncState]]:
     """Runs all burnin steps required."""
 
     if num_steps > 0:
+
       rng = self._rng_split(rng, num_steps)
 
       accumulator = utils.MultiChunkAccumulator.zeros_like(
           func_state, self.multi_device)
 
-      for rng_i in rng:
+      for i, rng_i in enumerate(rng):
         batch = next(data_iterator)
 
         state, accumulator = self._burnin(
-            params, state, rng_i, batch, func_state, accumulator)
+            params, state, rng_i, batch, func_state, accumulator,
+            i == num_steps - 1)
 
       func_state = accumulator.value_and_clear()
 
     return state, func_state
 
   @functools.partial(utils.staged, donate_argnums=(0, 1, 4))
   @utils.auto_scope_method
@@ -905,77 +1097,69 @@
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     # Setup arguments
     learning_rate, momentum, damping = self._setup_state_and_schedules(
         learning_rate, momentum,
         state.damping if self._use_adaptive_damping else damping,
-        state.step_counter)
+        state.step_counter, state.data_seen)
+
     func_args, rng = self._setup_func_args_and_rng(
         params, rng, batch, func_state)
 
     # Update curvature estimate
-    state.estimator_state = self._update_estimator_curvature(
-        state.estimator_state, func_args, rng, self._curvature_ema, 1.0)
+    state = self._maybe_update_estimator_curvature(
+        state,
+        func_args,
+        rng,
+        self._curvature_ema,
+        1.0,
+        sync=self.should_sync_estimator(state),
+    )
 
     del rng  # should not be used after this point!
 
-    if self._include_norms_in_stats:
-      param_norm = utils.norm(params)
-    if self._include_per_param_norms_in_stats:
-      param_norm_per_param = utils.per_parameter_norm(params, "param_norm")
-
     # Compute loss and gradients
-    loss, grads, func_state, aux = self._compute_loss_and_grads(func_args)
+    loss, grads, func_state, aux = self._compute_loss_and_grads(
+        func_args, state=state)
 
     # Sync
     loss, grads = utils.pmean_if_pmap((loss, grads), self.pmap_axis_name)
 
-    if self._include_norms_in_stats:
-      grad_norm = utils.norm(grads)
-
-    if self._include_per_param_norms_in_stats:
-      grad_norm_per_param = utils.per_parameter_norm(grads, "grad_norm")
-
     # Update the inverse curvature
     state = self._maybe_update_inverse_cache(state, damping)
 
     # Compute proposed directions
+    preconditioned_gradient = self._compute_preconditioned_gradient(
+        state, grads, damping
+    )
+
+    # constrain the norms
     preconditioned_gradient, sq_norm_scaled_grads = (
-        self._compute_preconditioned_gradient(state, grads, learning_rate,
-                                              damping)
+        self._maybe_apply_norm_constraint(
+            grads, preconditioned_gradient, learning_rate,
+        )
     )
 
     vectors = (preconditioned_gradient, state.velocities)
 
-    if self._include_norms_in_stats:
-      precon_grad_norm = utils.norm(preconditioned_gradient)
-    if self._include_per_param_norms_in_stats:
-      precon_grad_norm_per_param = utils.per_parameter_norm(
-          preconditioned_gradient, "precon_grad_norm")
-
     # Compute the coefficients for the vectors
     coefficients, quad_model_change = self._coefficients_and_quad_change(
         state=state,
         vectors=vectors,
         grads=grads,
         learning_rate=learning_rate,
         momentum=momentum,
         damping=damping,
         func_args=func_args)
 
     # Compute delta and update velocities
     delta = self.weighted_sum_of_objects(vectors, coefficients)
     state.velocities = delta
 
-    if self._include_norms_in_stats:
-      update_norm = utils.norm(delta)
-    if self._include_per_param_norms_in_stats:
-      update_norm_per_param = utils.per_parameter_norm(delta, "update_norm")
-
     # Update parameters
     params = jax.tree_util.tree_map(jnp.add, params, delta)
 
     # Optionally compute the reduction ratio and update the damping
     if self._use_adaptive_damping:
 
       state.damping, rho, new_loss = lax.cond(
@@ -1015,34 +1199,48 @@
         momentum=coefficients[1],
         damping=damping,
         rho=rho,
         quad_model_change=quad_model_change,
         scaled_grad_norm_sq=sq_norm_scaled_grads,
     )
 
-    if self._value_func_has_aux:
+    if aux is not None:
+      aux = utils.pmean_if_pmap(aux, self.pmap_axis_name)
       stats["aux"] = aux
 
     if self._include_norms_in_stats:
-      stats["param_norm"] = param_norm
-      stats["grad_norm"] = grad_norm
-      stats["precon_grad_norm"] = precon_grad_norm
-      stats["update_norm"] = update_norm
+      stats["param_norm"] = utils.norm(params)
+      stats["grad_norm"] = utils.norm(grads)
+      stats["precon_grad_norm"] = utils.norm(preconditioned_gradient)
+      stats["update_norm"] = utils.norm(delta)
 
     if self._include_per_param_norms_in_stats:
-      stats.update(param_norm_per_param)
-      stats.update(grad_norm_per_param)
-      stats.update(precon_grad_norm_per_param)
-      stats.update(update_norm_per_param)
+      stats.update(utils.per_parameter_norm(params, "param_norm"))
+      stats.update(utils.per_parameter_norm(grads, "grad_norm"))
+      stats.update(
+          utils.per_parameter_norm(preconditioned_gradient, "precon_grad_norm")
+      )
+      stats.update(utils.per_parameter_norm(delta, "update_norm"))
 
+    if self._include_registered_loss_in_stats:
+      assert aux is not None
+      stats["loss_registered"] = aux.pop("loss_registered")
+      stats["loss_registered"] = utils.pmean_if_pmap(stats["loss_registered"],
+                                                     self.pmap_axis_name)
+      stats["loss_registered_reldiff"] = (
+          stats["loss_registered"] - loss) / loss
+
+    # There seems to be a bug in PyType that is messing up the annotated return
+    # type function this function, causing it to be 'tuple' instead of what it
+    # actually is.
     if self._value_func_has_state:
-      return params, state, func_state, stats
+      return params, state, func_state, stats  # pytype: disable=bad-return-type
     else:
       assert func_state is None
-      return params, state, stats
+      return params, state, stats  # pytype: disable=bad-return-type
 
   def step(
       self,
       params: Params,
       state: "Optimizer.State",
       rng: PRNGKey,
       data_iterator: Optional[Iterator[Batch]] = None,
@@ -1051,14 +1249,18 @@
       learning_rate: Optional[Array] = None,
       momentum: Optional[Array] = None,
       damping: Optional[Array] = None,
       global_step_int: Optional[int] = None
   )-> ReturnEither:
     """Performs a single update step using the optimizer.
 
+    NOTE: please do not jit/pmap or otherwise compile this function with JAX,
+    as this can lead to errors. Compilation is handled internally by the
+    optimizer.
+
     Args:
       params: The current parameters of the model.
       state: The current state of the optimizer.
       rng: A Jax PRNG key. Should be different for each iteration and
         each Jax process/host.
       data_iterator: A data iterator to use (if not passing ``batch``).
       batch: A single batch used to compute the update. Should only pass one
@@ -1136,20 +1338,21 @@
     return self.l2_reg * utils.matrix_of_inner_products(vectors)
 
   @utils.auto_scope_method
   def compute_exact_quad_model(
       self,
       vectors: Sequence[Params],
       grads: Params,
-      func_args: Optional[FuncArgsVariants] = None,
+      func_args: FuncArgsVariants,
+      state: Optional["Optimizer.State"] = None,
   ) -> Tuple[Array, Array, Array]:
     """Computes the components of the exact quadratic model."""
-    if func_args is None:
-      raise ValueError("When you have not provided `c_factor_v` you must "
-                       "provide `func_args`.")
+
+    del state
+
     if self.estimator.default_mat_type == "fisher":
       c_factor_v = tuple(self._implicit.multiply_fisher_factor_transpose
                          (func_args, vi) for vi in vectors)
     elif self.estimator.default_mat_type == "ggn":
       c_factor_v = tuple(self._implicit.multiply_ggn_factor_transpose
                          (func_args, vi) for vi in vectors)
     else:
@@ -1175,22 +1378,24 @@
       return self.estimator.multiply(
           state=state.estimator_state,
           parameter_structured_vector=v,
           identity_weight=0.0,
           exact_power=True,
           use_cached=False,
           pmap_axis_name=self.pmap_axis_name,
+          norm_to_scale_identity_weight_per_block=self._norm_to_scale_identity_weight_per_block,
       )
 
     c_vectors = [c_times_v(v_i) for v_i in vectors]
 
     return (utils.symmetric_matrix_inner_products(c_vectors, vectors),
             utils.matrix_of_inner_products(vectors),
             utils.vector_of_inner_products(grads, vectors))
 
+  @utils.staged
   def compute_quadratic_model_value(
       self,
       a: Array,
       a_damped: Array,
       b: Array,
       w: Array,
   ) -> Array:
@@ -1203,15 +1408,15 @@
   @utils.staged
   def _solve_quad_model(
       self,
       quad_model_parameters: Tuple[Array, Array, Array],
       damping: Array,
       vectors: Sequence[Params],
       fixed_coefficients: Optional[Sequence[Union[Numeric, None]]] = None,
-  ) -> Tuple[Tuple[Optional[Array], ...], Array]:
+  ) -> Tuple[Tuple[Array, ...], Array]:
     """Solves for the optimal learning rate and momentum of the quadratic model.
 
     The quadratic model is represented as:
       Q(w) = w^T V^T (C + damping * I) V w / 2.0 + w^T V^T g
     where (n - number of vectors, d - dimensions of each vector):
       w (n,) - the vector of free weights (learning rate and momentum)
       V (d, n) - the matrix of proposed vectors for each weight
@@ -1234,14 +1439,18 @@
      A list of coefficients which are the solution (and include any values that
      are not None from fixed_weights) and the value of the quadratic model
      function for this solution (as a scalar).
     Raises:
       The function currently supports only up to two vectors, hence if you
       provide more, it will raise a ``NotImplementedError``.
     """
+    # TODO(jamesmartens,botev): it would be better if this method didn't need
+    # to have 'vectors' passed. We could instead use the 'D' matrix to get the
+    # to get the matrix for the l2 regularization.
+
     if fixed_coefficients is None:
       fixed_coefficients = (None,) * len(vectors)
 
     if len(vectors) != len(fixed_coefficients):
       raise ValueError("The length of `vectors` must be equal to the length of "
                        "`fixed_coefficients`.")
 
@@ -1261,28 +1470,21 @@
 
     if all(c is None for c in fixed_coefficients):
       # Adapt all coefficients
 
       if len(fixed_coefficients) == 1:
         # This special case arises at the first iteration, because all
         # velocities are zeros.
-
         special_case = jnp.logical_and(A_damped[0, 0] == 0, b[0] == 0)
         w = - lax.cond(special_case, lambda: b, lambda: b / A_damped[0])
 
       elif len(fixed_coefficients) == 2:
         # This special case arises at the first iteration, because all
         # velocities are zeros.
-
-        to_check = jnp.asarray([A_damped[0, 1], A_damped[1, 0],
-                                A_damped[1, 1], b[1]])
-
-        w = - lax.cond(jnp.all(to_check == 0),
-                       lambda: jnp.stack([b[0] / A_damped[0, 0], b[1]]),
-                       lambda: jnp.linalg.solve(A_damped, b))
+        w = - utils.psd_solve_maybe_zero_last_idx(A_damped, b)
       else:
         raise NotImplementedError()
 
     elif all(c is not None for c in fixed_coefficients):
       # No coefficients adapted
 
       w = jnp.asarray(fixed_coefficients)
@@ -1357,16 +1559,17 @@
       gradients w.r.t. parameters.
     has_aux: Similar to the meaning in :func:`jax.grad`, whether the
       ``value_and_grad_func`` returns with the loss value any auxiliary data.
 
   Returns:
     A function that returns only the loss value.
   """
-  def value_func(*args) -> Array:
-    out, _ = value_and_grad_func(*args)
+
+  def value_func(*args, **kwargs) -> Array:
+    out, _ = value_and_grad_func(*args, **kwargs)
     return out[0] if has_aux else out
 
   return value_func
 
 
 def make_func_args(
     params: Params,
@@ -1429,14 +1632,15 @@
   Returns:
     A triple ``(loss, func_state, aux)``. If the model function does not return
     any auxiliary data than ``aux`` will be ``None`` and if it does not have a
     state ``func_state`` will be ``None``.
   """
 
   if not has_aux and not has_state:
+    assert isinstance(raw_outputs, Array)
     return raw_outputs, None, None
 
   loss, other = raw_outputs
 
   if has_aux and has_state:
     func_state, aux = other
   elif has_aux:
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/patches_second_moment.py` & `kfac-jax-0.0.6/kfac_jax/_src/patches_second_moment.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     """Swaps the batch and channel indices of the layout."""
     return _ConvSpec([self.c_axis, self.n_axis, *self.spatial_axes])
 
   def create_shape(self, n: T, c: T, *spatial_dims: T) -> Tuple[T, ...]:
     """Creates a shape according to this layout specification."""
     if len(spatial_dims) != len(self.order) - 2:
       raise ValueError("Incorrect number of spatial dimensions.")
-    result: List[T] = [None] * len(self)
+    result: List[T] = [None] * len(self)  # pytype: disable=annotation-type-mismatch
     result[self.n_axis] = n
     result[self.c_axis] = c
     for ax, dim in zip(self.spatial_axes, spatial_dims):
       result[ax] = dim
     assert all(r is not None for r in result)
     return tuple(result)
 
@@ -624,15 +624,15 @@
     # Index the weighting function
     if weighting_array is not None:
       if weighting_array.shape[in_spec.c_axis] == 1:
         wf_i = weighting_array
       else:
         wf_n = weighting_array[in_spec.n_axis]
         wf_spatial = [weighting_array.shape[a] for a in in_spec.spatial_axes]
-        wf_sizes = in_spec.create_shape(wf_n, jnp.ones([]), *wf_spatial)
+        wf_sizes = in_spec.create_shape(wf_n, jnp.ones([]), *wf_spatial)  # pytype: disable=wrong-arg-types  # jnp-type
         wf_i = _slice_array(weighting_array, index, wf_sizes)
     else:
       wf_i = None
 
     matrix, vector = patches_moments_explicit(
         image_channel,
         kernel_spatial_shape=kernel_spatial_shape,
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/tag_graph_matcher.py` & `kfac-jax-0.0.6/kfac_jax/_src/tag_graph_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,23 @@
 import itertools
 import pprint
 from typing import Any, Callable, Mapping, Optional, Sequence, TypeVar, Tuple, Union, Dict, Set
 
 from absl import logging
 import immutabledict
 import jax
-import jax.numpy as jnp
+
+jax_version = (
+    jax.__version_info__ if hasattr(jax, "__version_info__")
+    else tuple(map(int, jax.__version__.split("."))))
+
+if jax_version > (0, 4, 11):
+  import jax.extend as jax_extend  # pylint: disable=g-import-not-at-top
+
+import jax.numpy as jnp  # pylint: disable=g-import-not-at-top
 from kfac_jax._src import layers_and_loss_tags as tags
 from kfac_jax._src import utils
 import numpy as np
 
 HIGHER_ORDER_NAMES = ("cond", "while", "scan", "xla_call", "xla_pmap")
 
 # Types for annotation
@@ -46,17 +54,23 @@
 PatternComputeFunc = Callable[[Array, Sequence[Array]], Array]
 ParameterExtractorFunc = Callable[[JaxprEqns], Mapping[str, Any]]
 TagCtor = Callable[[Vars, Vars, JaxprEqns, MakeVarFunc], JaxprEqn]
 
 
 def eval_jaxpr_eqn(eqn: JaxprEqn, in_values: Vars) -> Var:
   """Computes the outputs of the given Jaxpr equation."""
+
   subfuns, bind_params = eqn.primitive.get_bind_params(eqn.params)
-  with jax.core.source_info_util.user_context(
-      eqn.source_info.traceback):
+
+  if jax_version > (0, 4, 11):
+    user_context = jax_extend.source_info_util.user_context
+  else:
+    user_context = jax.core.source_info_util.user_context  # pytype: disable=module-attr
+
+  with user_context(eqn.source_info.traceback):
     return eqn.primitive.bind(*subfuns, *in_values, **bind_params)
 
 
 def reshape_equivalent(
     equation1: JaxprEqn,
     equation2: JaxprEqn,
 ) -> bool:
@@ -327,15 +341,15 @@
     tag_ctor: Optional[TagCtor] = None,
 ) -> JaxprGraph:
   """Creates a :class:`~JaxGraph` instance from the provided function and arguments."""
   in_tree = jax.tree_util.tree_structure(func_args)
   closed_jaxpr, out_shapes = jax.make_jaxpr(func, return_shape=True)(*func_args)
 
   if compute_only_loss_tags:
-    make_var_func = jax.core.gensym([closed_jaxpr.jaxpr])
+    make_var_func = jax.core.gensym()
     eqns = []
     sub_graph_vars = set()
     loss_tags_output_vars = []
     for eqn in reversed(closed_jaxpr.jaxpr.eqns):
       if (isinstance(eqn.primitive, tags.LossTag) or
           any(v in sub_graph_vars for v in eqn.outvars)):
         if isinstance(eqn.primitive, tags.LossTag):
@@ -1451,15 +1465,15 @@
 
   # Automatically detect registrations
   for match in matches.values():
     for p in match.param_graph_variables:
       tagged_params.add(p)
 
   # Create the Jaxpr with all the tag registrations
-  make_var_func = jax.core.gensym([mid_graph.jaxpr])
+  make_var_func = jax.core.gensym()
   eqns = list()
   env = {}
   pattern_counters = {}
 
   if register_orphans:
     for param in mid_graph.params_vars:
       if param not in tagged_params:
@@ -1558,14 +1572,15 @@
       compute_only_loss_tags=compute_only_loss_tags,
       clean_broadcasts=True,
   )
 
   patterns = () if register_only_generic else  tuple(
       pattern for pattern in graph_patterns
       if pattern.name not in patterns_to_skip)
+
   func_graph, tagged_locations = _auto_register_tags(
       graph=graph,
       graph_matcher_rules=graph_matcher_rules,
       graph_patterns=patterns,
       register_orphans=True,
       register_only_until_losses=True
   )
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/tracer.py` & `kfac-jax-0.0.6/kfac_jax/_src/tracer.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,37 +26,37 @@
 # Types for annotations
 Array = utils.Array
 Shape = utils.Shape
 Params = utils.Params
 FuncArgs = utils.FuncArgs
 FuncOuts = utils.FuncOuts
 Var = jax.core.Var
+LossFunction = loss_functions.LossFunction
+LossFunctionInputs = loss_functions.LossFunctionInputs
 
 T = TypeVar("T")
 # J = TypeVar("J", jax.core.Jaxpr, jax.core.ClosedJaxpr)
 ProcJaxpr: TypeAlias = "ProcessedJaxpr"
-TaggedFunction = Callable[..., Tuple[loss_functions.LossFunction, ...]]
+TaggedFunction = Callable[..., Tuple[LossFunction, ...]]
 FuncWithTags = Callable[..., Any]
-LossTagInputs = Tuple[Array, ...]
-LayerTagInputs = Tuple[Array, ...]
 
 FunctionTransformation = Callable[..., Union[ProcJaxpr, T]]
 TransformedFunction = Callable[..., Union[ProcJaxpr, T]]
 
 LossTagsVjp = Tuple[
-    Tuple[loss_functions.LossFunction, ...],
-    Callable[[Sequence[LossTagInputs]], Params]
+    Tuple[LossFunction, ...],
+    Callable[[Sequence[LossFunctionInputs]], Params]
 ]
 LossTagsJvp = Tuple[
-    Tuple[loss_functions.LossFunction, ...],
-    Tuple[LossTagInputs, ...],
+    Tuple[LossFunction, ...],
+    Tuple[LossFunctionInputs, ...],
 ]
 LayerTagVjp = Tuple[
-    Tuple[loss_functions.LossFunction, ...],
-    Callable[[Tuple[LossTagInputs, ...]], Tuple[Dict[str, Array], ...]]
+    Tuple[LossFunction, ...],
+    Callable[[Tuple[LossFunctionInputs, ...]], Tuple[Dict[str, Array], ...]]
 ]
 JaxprOrClosedJaxpr = Union[jax.core.Jaxpr, jax.core.ClosedJaxpr]
 
 
 def shape_and_type(x: Array) -> Tuple[Shape, jnp.dtype]:
   """Returns the shape and type of the given array."""
   return x.shape, x.dtype
@@ -284,15 +284,15 @@
       return False
 
     if any(ref_tag.primitive != tag.primitive
            for ref_tag, tag in zip(self.layer_tags, other.layer_tags)):
       return False
 
     # Verify whether parameter shapes are equivalent
-    if any(p_i.aval.shape != p_j.aval.shape
+    if any(p_i.aval.shape != p_j.aval.shape  # pytype: disable=attribute-error  # always-use-property-annotation
            for p_i, p_j in zip(self.params_vars_flat, other.params_vars_flat)):
       return False
 
     return True
 
 
 def cached_transformation(
@@ -384,18 +384,18 @@
 
 
 def construct_compute_losses_inputs(
     jaxpr: jax.core.Jaxpr,
     consts: Sequence[Any],
     num_losses: int,
     primal_func_args: FuncArgs,
-    params_index: int
+    params_index: int,
 ) -> Callable[
     [Params],
-    Tuple[Tuple[LossTagInputs, ...], Tuple[LossTagInputs, ...]]
+    Tuple[Tuple[LossFunctionInputs, ...], Tuple[LossFunction, ...]],
 ]:
   """Constructs a function that computes the inputs to all loss tags.
 
   The returned function takes as input only the parameters, as specified by
   ``params_index``, and returns a tuple containing the input values to the first
   ``num_losses`` loss tags in the Jaxpr. This is done by iterating sequentially
   over all equations in the Jaxpr, evaluating each equation, until the correct
@@ -414,15 +414,15 @@
 
   Returns:
     A function which computes the inputs to the first ``num_losses`` loss tags.
   """
 
   def forward_compute_losses(
       primal_params: Params
-  ) -> Tuple[Tuple[LossTagInputs, ...], Tuple[LossTagInputs, ...]]:
+  ) -> Tuple[Tuple[LossFunctionInputs, ...], Tuple[LossFunction, ...]]:
     """Computes and returns the inputs to the first ``num_losses`` loss tags."""
 
     # Check the provided inputs match the original primals.
     local_func_args = list(primal_func_args)
     original_params = local_func_args[params_index]
 
     if not utils.abstract_objects_equal(original_params, primal_params):
@@ -440,34 +440,55 @@
 
     # Bind args and consts to environment
     write(jaxpr.invars, flat_args)
     write(jaxpr.constvars, consts)
 
     # Loop through equations and evaluate primitives using `bind`
     losses_so_far = 0
+    losses = []
     losses_p_deps = []
     losses_inputs = []
     for eqn in jaxpr.eqns:
-
       write(eqn.outvars, tgm.eval_jaxpr_eqn(eqn, read(eqn.invars)))
 
       if isinstance(eqn.primitive, tags.LossTag):
+        loss_tag: tags.LossTag = eqn.primitive
         losses_inputs.append(read(eqn.invars))
-        losses_p_deps.append(eqn.primitive.extract_parameter_dependants(
+        losses.append(loss_tag.loss(*losses_inputs[-1], **eqn.params))
+        losses_p_deps.append(loss_tag.extract_parameter_dependants(
             *losses_inputs[-1], **eqn.params))
         losses_so_far += 1
 
       if num_losses is not None and losses_so_far == num_losses:
         break
 
-    return tuple(losses_p_deps), tuple(losses_inputs)
+    return tuple(losses_p_deps), tuple(losses)
 
   return forward_compute_losses
 
 
+def _compute_all_losses(
+    p_jaxpr: ProcessedJaxpr,
+    primal_func_args: FuncArgs,
+) -> Tuple[LossFunction, ...]:
+  """Returns all loss functions objects."""
+  if not p_jaxpr.loss_tags:
+    raise ValueError("The provided `ProcessedJaxpr` has no loss tags.")
+
+  losses_func = construct_compute_losses_inputs(
+      jaxpr=p_jaxpr.jaxpr,
+      consts=p_jaxpr.consts,
+      num_losses=len(p_jaxpr.loss_tags),
+      primal_func_args=primal_func_args,
+      params_index=p_jaxpr.params_index,
+  )
+  _, losses = losses_func(primal_func_args[p_jaxpr.params_index])
+  return losses
+
+
 def _loss_tags_vjp(
     p_jaxpr: ProcessedJaxpr,
     primal_func_args: FuncArgs,
 ) -> LossTagsVjp:
   """Computes a (backward-mode) vector-Jacobian product w.r.t. all loss tags.
 
   The function has similar interface to :func:`jax.vjp`. It takes as inputs the
@@ -494,23 +515,17 @@
       jaxpr=p_jaxpr.jaxpr,
       consts=p_jaxpr.consts,
       num_losses=len(p_jaxpr.loss_tags),
       primal_func_args=primal_func_args,
       params_index=p_jaxpr.params_index)
 
   primal_params = primal_func_args[p_jaxpr.params_index]
+  _, full_vjp_func, losses = jax.vjp(losses_func, primal_params, has_aux=True)
 
-  (_, losses_inputs), full_vjp_func = jax.vjp(losses_func, primal_params)
-
-  losses = tuple(tag.primitive.loss(*inputs, **tag.params)
-                 for tag, inputs in zip(p_jaxpr.loss_tags, losses_inputs))
-
-  zero_tangents = jax.tree_util.tree_map(jnp.zeros_like, losses_inputs)
-
-  def losses_vjp_func(losses_tangents: Sequence[LossTagInputs]) -> Params:
+  def losses_vjp_func(losses_tangents: Sequence[LossFunctionInputs]) -> Params:
     """Computes the vector-Jacobian product w.r.t. the parameters.
 
     Args:
       losses_tangents: The tangents to all loss tag's inputs.
 
     Returns:
       The parameters' tangents, as a result of the vector-Jacobian product.
@@ -525,17 +540,15 @@
 
     for i, loss_tangents in enumerate(losses_tangents):
       if not isinstance(loss_tangents, Sequence):
         raise ValueError("Each element of the argument `tangents` must be "
                          f"a sequence, but tangents[{i}] has type "
                          f"{type(loss_tangents)}.")
 
-    # The tangents of the second entry are always zero, as we compute this only
-    # for the parameter dependent arrays.
-    params_tangents, = full_vjp_func((losses_tangents, zero_tangents))
+    [params_tangents] = full_vjp_func(losses_tangents)
 
     return params_tangents
 
   return losses, losses_vjp_func
 
 
 def _loss_tags_jvp(
@@ -574,33 +587,25 @@
       primal_func_args=primal_func_args,
       params_index=p_jaxpr.params_index)
 
   primal_params = (primal_func_args[p_jaxpr.params_index],)
 
   tangents = (params_tangents,)
 
-  (primals_out, tangents_out) = jax.jvp(losses_func, primal_params, tangents)
-
-  _, losses_inputs_primals = primals_out
-
-  losses_tangents, _ = tangents_out
-
-  losses = tuple(
-      tag.primitive.loss(*inputs, **tag.params)
-      for tag, inputs in zip(p_jaxpr.loss_tags, losses_inputs_primals)
-  )
+  (_, losses_tangents, losses) = jax.jvp(
+      losses_func, primal_params, tangents, has_aux=True)
 
   return losses, losses_tangents
 
 
 def _loss_tags_hvp(
     processed_jaxpr: ProcessedJaxpr,
     primal_func_args: FuncArgs,
     params_tangents: Params,
-) -> Tuple[Params, Tuple[loss_functions.LossFunction, ...]]:
+) -> Tuple[Params, Tuple[LossFunction, ...]]:
   """Computes a Hessian-vector product of the function w.r.t. all loss tags.
 
   The function takes as inputs the concrete values of the primals for the
   function arguments at which the Hessian will be evaluated at and the concrete
   values of the tangents for the **parameters**, as specified by
   ``processed_jaxpr.params_index``. It returns the product of the Hessian with
   this tangents via backward-over-forward mode.
@@ -623,35 +628,26 @@
   losses_func = construct_compute_losses_inputs(
       jaxpr=processed_jaxpr.jaxpr,
       consts=processed_jaxpr.consts,
       num_losses=len(processed_jaxpr.loss_tags),
       primal_func_args=primal_func_args,
       params_index=processed_jaxpr.params_index)
 
-  def compute_losses(
-      param_primals: Params
-  ) -> Tuple[loss_functions.LossFunction, ...]:
-    """Computes the sum of all losses as a scalar."""
-
-    _, loss_inputs = losses_func(param_primals)
-
-    return tuple(tag.primitive.loss(*inputs, **tag.params)
-                 for tag, inputs in zip(processed_jaxpr.loss_tags, loss_inputs))
-
   def losses_sum(param_primals: Params) -> Array:
     # This computes the sum of losses evaluated. Makes it easier because we can
     # now use jax.grad rather than jax.vjp for taking derivatives.
-    return sum(jnp.sum(loss.evaluate()) for loss in
-               compute_losses(param_primals))
+    _, losses = losses_func(param_primals)
+    return sum(jnp.sum(loss.evaluate()) for loss in losses)
 
   # Directional derivative function
   df_dot_dv = lambda p: (jax.jvp(losses_sum, [p], [params_tangents])[1])
   hvp = jax.grad(df_dot_dv)(primal_func_args[processed_jaxpr.params_index])
 
-  return hvp, compute_losses(primal_func_args[processed_jaxpr.params_index])
+  _, losses = losses_func(primal_func_args[processed_jaxpr.params_index])
+  return hvp, losses
 
 
 def _layer_tag_vjp(
     processed_jaxpr: ProcessedJaxpr,
     primal_func_args: FuncArgs,
 ) -> LayerTagVjp:
   """Computes primal values and tangents w.r.t. all layer tags.
@@ -708,15 +704,15 @@
 
     assert num_losses_passed == len(processed_jaxpr.loss_tags)
 
     return read(layer_input_vars)
 
   def forward_aux(
       aux: Dict[Var, Array]
-  ) -> Tuple[Tuple[LossTagInputs, ...], Tuple[LossTagInputs, ...]]:
+  ) -> Tuple[Tuple[LossFunctionInputs, ...], Tuple[LossFunctionInputs, ...]]:
     """Computes the inputs and kwargs of all **loss** tags.
 
     Args:
       aux: A mapping from an Jaxpr variable to an additional auxiliary value.
         For each variable in this mapping, we add to the value computed during
         standard evaluation the auxiliary value. This is done in order to be
         able to compute gradients wrt all intermediate expressions
@@ -799,15 +795,15 @@
       forward_aux, aux_dict, has_aux=True)
 
   # Compute the actual loss objects.
   losses = tuple(tag.primitive.loss(*inputs, **tag.params) for tag, inputs in
                  zip(processed_jaxpr.loss_tags, losses_inputs))
 
   def vjp_func(
-      tangents: Tuple[LossTagInputs, ...]
+      tangents: Tuple[LossFunctionInputs, ...]
   ) -> Tuple[Dict[str, Array], ...]:
     """Computes a (reverse-mode) vector-Jacobian product w.r.t. all layer tags.
 
     Args:
       tangents: The concrete tangent values for the tangents of the inputs to
         all **loss** tags.
 
@@ -847,14 +843,45 @@
       layers_info.append(info)
 
     return tuple(layers_info)  # pytype: disable=bad-return-type  # numpy-scalars
 
   return losses, vjp_func
 
 
+def compute_all_losses(
+    func: utils.Func,
+    params_index: int = 0,
+) -> TransformedFunction[Tuple[LossFunction, ...]]:
+  """Creates a function that when called, returns all loss objects.
+
+  The returned function takes as inputs the concrete values of the primals for
+  which to compute the loss objects.
+
+  Args:
+    func: The model function, which must include at least one loss registration.
+    params_index: The variables from the function arguments which are at this
+      index (e.g. `func_args[params_index]`) are to be considered model
+      parameters.
+
+  Returns:
+    A function that computes the Jacobian-vector product with signature
+    `Callable[[FuncArgs], Tuple[LossFunction, ...]]`.
+  """
+  # Note that this function is independent of any layer tags, hence we can avoid
+  # calling the auto registration.
+  return cached_transformation(
+      func=func,
+      transformation=_compute_all_losses,
+      verifier=lambda: None,
+      params_index=params_index,
+      auto_register_tags=False,
+      allow_left_out_params=True,
+  )
+
+
 def loss_tags_vjp(
     func: utils.Func,
     params_index: int = 0,
 ) -> TransformedFunction[LossTagsVjp]:
   """Creates a function for the vector-Jacobian product w.r.t. all loss tags.
 
   The returned function has a similar interface to :func:`jax.vjp`. It takes as
@@ -941,15 +968,15 @@
     params_index: The variables from the function arguments which are at this
       index (e.g. `func_args[params_index]`) are to be considered model
       parameters.
 
   Returns:
     A function that computes the Hessian-vector product and also returns all
     losses, with signature `Callable[[FuncArgs, Params],
-    Tuple[LossTagsVjp, Tuple[loss_functions.LossFunction, ...]]`.
+    Tuple[LossTagsVjp, Tuple[LossFunction, ...]]`.
   """
   # Note that this function is independent of any layer tags, hence we can avoid
   # calling the auto registration.
   return cached_transformation(
       func=func,
       transformation=_loss_tags_hvp,
       verifier=lambda: None,
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/utils/__init__.py` & `kfac-jax-0.0.6/kfac_jax/_src/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,81 +44,93 @@
 tree_is_empty = types.tree_is_empty
 abstract_objects_equal = types.abstract_objects_equal
 get_float_dtype_and_check_consistency = (
     types.get_float_dtype_and_check_consistency)
 del types
 
 # misc
+deserialize_state_tree = misc.deserialize_state_tree
+serialize_state_tree = misc.serialize_state_tree
 to_tuple_or_repeat = misc.to_tuple_or_repeat
 first_dim_is_size = misc.first_dim_is_size
 fake_element_from_iterator = misc.fake_element_from_iterator
 default_batch_size_extractor = misc.default_batch_size_extractor
 auto_scope_function = misc.auto_scope_function
 auto_scope_method = misc.auto_scope_method
 register_state_class = misc.register_state_class
 replace_char = misc.replace_char
+call_func_with_conditional_kwargs = misc.call_func_with_conditional_kwargs
 Finalizable = misc.Finalizable
 State = misc.State
 del misc
 
 # parallel
 in_pmap = parallel.in_pmap
 wrap_if_pmap = parallel.wrap_if_pmap
 pmean_if_pmap = parallel.pmean_if_pmap
 psum_if_pmap = parallel.psum_if_pmap
-compute_mean = parallel.compute_mean
-compute_sum = parallel.compute_sum
+pmap_mean = parallel.pmap_mean
+pmap_sum = parallel.pmap_sum
 index_if_not_scalar = parallel.index_if_not_scalar
 get_first = parallel.get_first
 get_mean = parallel.get_mean
 get_sum = parallel.get_sum
 broadcast_all_local_devices = parallel.broadcast_all_local_devices
 pmap_zeros_like = parallel.pmap_zeros_like
 jit_zeros_like = parallel.jit_zeros_like
 replicate_all_local_devices = parallel.replicate_all_local_devices
 make_different_rng_key_on_all_devices = (
     parallel.make_different_rng_key_on_all_devices)
 p_split = parallel.p_split
 p_split_num = parallel.p_split_num
-check_and_fix_format_for_pmap = parallel.check_and_fix_format_for_pmap
 host_sync = parallel.host_sync
 host_all_gather = parallel.host_all_gather
 host_mean = parallel.host_mean
 pmap_sync_and_divide_value = parallel.pmap_sync_and_divide_value
 jit_sync_and_divide_value = parallel.jit_sync_and_divide_value
 copy_array = parallel.copy_array
 copy_obj = parallel.copy_obj
 pmap_copy_obj = parallel.pmap_copy_obj
 distribute_thunks = parallel.distribute_thunks
 del parallel
 
 # math
 set_special_case_zero_inv = math.set_special_case_zero_inv
 get_special_case_zero_inv = math.get_special_case_zero_inv
+set_use_cholesky_inversion = math.set_use_cholesky_inversion
+get_use_cholesky_inversion = math.get_use_cholesky_inversion
 product = math.product
 outer_product = math.outer_product
 scalar_mul = math.scalar_mul
 scalar_div = math.scalar_div
 weighted_sum_of_objects = math.weighted_sum_of_objects
+sum_of_objects = math.sum_objects
 inner_product = math.inner_product
 symmetric_matrix_inner_products = math.symmetric_matrix_inner_products
 matrix_of_inner_products = math.matrix_of_inner_products
 vector_of_inner_products = math.vector_of_inner_products
 block_permuted = math.block_permuted
 norm = math.norm
+squared_norm = math.squared_norm
 per_parameter_norm = math.per_parameter_norm
-psd_inv_cholesky = math.psd_inv_cholesky
+psd_inv = math.psd_inv
+psd_solve = math.psd_solve
+psd_solve_maybe_zero_last_idx = math.psd_solve_maybe_zero_last_idx
+pi_adjusted_kronecker_factors = math.pi_adjusted_kronecker_factors
 pi_adjusted_kronecker_inverse = math.pi_adjusted_kronecker_inverse
 kronecker_product_axis_mul_v = math.kronecker_product_axis_mul_v
 kronecker_eigen_basis_axis_mul_v = math.kronecker_eigen_basis_axis_mul_v
 kronecker_product_mul_v = math.kronecker_product_mul_v
 kronecker_eigen_basis_mul_v = math.kronecker_eigen_basis_mul_v
 safe_psd_eigh = math.safe_psd_eigh
 loop_and_parallelize_average = math.loop_and_parallelize_average
 psd_matrix_norm = math.psd_matrix_norm
+invert_psd_matrices = math.invert_psd_matrices
+inverse_sqrt_psd_matrices = math.inverse_sqrt_psd_matrices
+
 del math
 
 # accumulators
 WeightedMovingAverage = accumulators.WeightedMovingAverage
 MultiChunkAccumulator = accumulators.MultiChunkAccumulator
 del accumulators
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/utils/accumulators.py` & `kfac-jax-0.0.6/kfac_jax/_src/utils/accumulators.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ArrayTree = types.ArrayTree
 TArrayTree = types.TArrayTree
 
 
 @misc.register_state_class
 class WeightedMovingAverage(Generic[TArrayTree], misc.State):
   """A wrapped class for an arbitrary weighted moving average."""
+
   weight: Numeric
   raw_value: Optional[TArrayTree]
 
   @property
   def value(self) -> TArrayTree:
     """The value of the underlying arrays data structure."""
     return jax.tree_util.tree_map(lambda x: x / self.weight, self.raw_value)
@@ -43,71 +44,78 @@
   def update(
       self,
       value: TArrayTree,
       old_weight_multiplier: Numeric,
       new_weight: Numeric,
   ):
     """Updates the underlying array and weight accordingly."""
-    if self.raw_value is None:
-      self.raw_value = value
-      self.weight = jnp.asarray(new_weight).astype(self.weight.dtype)
 
-    else:
-      self.weight = self.weight * old_weight_multiplier + new_weight
-      self.raw_value = jax.tree_util.tree_map(
-          lambda x, y: x * old_weight_multiplier + y * new_weight,
-          self.raw_value,
-          value,
-      )
+    assert self.raw_value is not None
+
+    # A negative value of new_weight means we should only update the value
+    # (with -new_weight) and not the total running weight. This roughly
+    # corresponds to summation instead of averaging, and is useful in a few
+    # contexts.
+    new_weight_for_value = jnp.abs(new_weight)
+    new_weight_for_weight = jax.nn.relu(new_weight)
+
+    self.weight = self.weight * old_weight_multiplier + new_weight_for_weight
+
+    self.raw_value = jax.tree_util.tree_map(
+        lambda x, y: x * old_weight_multiplier + y * new_weight_for_value,
+        self.raw_value,
+        value,
+    )
 
   def sync(self, pmap_axis_name: Optional[str]):
     """Syncs the underlying array across devices."""
+
     if self.raw_value is None:
       raise ValueError("`raw_value` has not been set yet.")
+
     self.raw_value = parallel.pmean_if_pmap(self.raw_value, pmap_axis_name)
 
   def clear(self, value_to_none: bool = False):
     """Resets the weighted average."""
+
     self.weight = jnp.zeros_like(self.weight)
     self.raw_value = None if value_to_none else jnp.zeros_like(self.raw_value)
 
   def value_and_clear(self) -> TArrayTree:
     """Retrieves the value of the weighted average and clears it."""
+
     value = self.value
     self.clear()
+
     return value
 
   @classmethod
   def zeros_array(
       cls,
       shape: Shape,
       dtype: Optional[DType] = None,
   ) -> "WeightedMovingAverage[Array]":
     """Initializes a `WeightedMovingAverage` with a single array of zeros."""
-    return WeightedMovingAverage(
+
+    return cls(  # pytype: disable=wrong-keyword-args
         weight=jnp.zeros([], dtype=dtype),
         raw_value=jnp.zeros(shape, dtype=dtype),
     )
 
   @classmethod
   def zeros_like(cls, value: TArrayTree) -> "WeightedMovingAverage[TArrayTree]":
     """Initializes a `WeightedMovingAverage` with zeros structure like `value`."""
-    return WeightedMovingAverage(
+
+    return cls(  # pytype: disable=wrong-keyword-args
         weight=jnp.array(
             0.0, dtype=types.get_float_dtype_and_check_consistency(value)
         ),
         raw_value=jax.tree_util.tree_map(jnp.zeros_like, value),
     )
 
-  @classmethod
-  def empty(cls, dtype: Optional[DType] = None) -> "WeightedMovingAverage[Any]":
-    """Returns an empty moving average instance."""
-    weight = jnp.zeros([]) if dtype is None else jnp.zeros([], dtype=dtype)
-    return WeightedMovingAverage(weight=weight, raw_value=None)
-
 
 class MultiChunkAccumulator(Generic[TArrayTree]):
   """Statistics accumulation, abstracted over multiple chunks."""
 
   def __init__(
       self,
       init_obj_value: Optional[TArrayTree],
@@ -157,16 +165,18 @@
   def clear(self) -> None:
     """Sets the underlying accumulator and weight to `None`."""
     self._accumulator = None
     self._weight = None
 
   def value_and_clear(self) -> TArrayTree:
     """Retrieves the normalized value of the accumulator and clears it."""
+
     value = self.value
     self.clear()
+
     return value
 
   def add(self, value_obj: TArrayTree, weight: Numeric = 1):
     """Adds an element to the moving average and the max.
 
     The exact update equation for the statistics are:
       raw_value_t = raw_value_{t-1} + value_obj * weight
@@ -250,15 +260,17 @@
 
   def __repr__(self):
     return (f"{self.__class__.__name__}({self._accumulator!r}, "
             f"{self._weight!r}, {self._multi_device})")
 
   def copy(self):
     """Returns a copy of the PyTree structure (but not the JAX arrays)."""
+
     (flattened, structure) = jax.tree_util.tree_flatten(self)
+
     return jax.tree_util.tree_unflatten(structure, flattened)
 
 
 jax.tree_util.register_pytree_node(
     MultiChunkAccumulator,
     lambda x: ((x.accumulator, x.weight), (x.multi_device,)),
     lambda fixed, arrays: MultiChunkAccumulator(*arrays, *fixed)
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/utils/math.py` & `kfac-jax-0.0.6/kfac_jax/_src/utils/math.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,26 +38,44 @@
 
 _ALPHABET = string.ascii_lowercase
 
 # If true we use a special case formula for when a block has one or more zero
 # factors.
 _SPECIAL_CASE_ZERO_INV: bool = True
 
+# Cholesky inverses are deterministic on GPUs and somewhat faster to compute,
+# but tend to perform a bit worse and not tolerate very low damping values.
+# If disabling Cholesky inverses and using GPUs, one must make sure to set
+# distributed_inverses=True, since otherwise the devices can potentially become
+# out of sync, which is a silent and very serious failure
+_USE_CHOLESKY_INVERSION: bool = False
+
 
 def set_special_case_zero_inv(value: bool):
   """Sets whether `pi_adjusted_inverse` handles zero and nan matrices."""
   global _SPECIAL_CASE_ZERO_INV
   _SPECIAL_CASE_ZERO_INV = value
 
 
 def get_special_case_zero_inv() -> bool:
   """Returns whether `pi_adjusted_inverse` handles zero and nan matrices."""
   return _SPECIAL_CASE_ZERO_INV
 
 
+def set_use_cholesky_inversion(value: bool):
+  """Sets whether `pi_adjusted_inverse` handles zero and nan matrices."""
+  global _USE_CHOLESKY_INVERSION
+  _USE_CHOLESKY_INVERSION = value
+
+
+def get_use_cholesky_inversion() -> bool:
+  """Returns whether `pi_adjusted_inverse` handles zero and nan matrices."""
+  return _USE_CHOLESKY_INVERSION
+
+
 def product(iterable_object: Iterable[TNumeric]) -> TNumeric:
   """Computes the product of all elements in the iterable."""
   x = 1
 
   for element in iterable_object:
     x = x * element
 
@@ -130,14 +148,18 @@
                        "structure.")
     accumulator = jax.tree_util.tree_map(
         jnp.add, accumulator, scalar_mul(o_i, c_i))
 
   return accumulator
 
 
+def sum_objects(objects: Sequence[TArrayTree]) -> TArrayTree:
+  return weighted_sum_of_objects(objects, [1] * len(objects))
+
+
 def _inner_product_float64(obj1: ArrayTree, obj2: ArrayTree) -> Array:
   """Computes inner product explicitly in float64 precision."""
 
   raise NotImplementedError()
 
   # This function isn't currently working due to a break in
   # jax.experimental.enable_x64.
@@ -307,14 +329,22 @@
   indices = np.cumsum(block_sizes)[:-1]
   blocks = [jnp.split(row, indices, 1) for row in jnp.split(matrix, indices, 0)]
   reordered_blocks = [[blocks[i][j] for j in block_order] for i in block_order]
 
   return jnp.block(reordered_blocks)
 
 
+def squared_norm(obj: ArrayTree) -> Array:
+  """Computes the squared Euclidean norm of the provided PyTree object."""
+  elements_squared_norm = jax.tree_util.tree_map(
+      lambda x: jnp.sum(jnp.square(x)), obj)
+
+  return sum(jax.tree_util.tree_leaves(elements_squared_norm))
+
+
 def norm(obj: ArrayTree) -> Array:
   """Computes the Euclidean norm of the provided PyTree object."""
   elements_squared_norm = jax.tree_util.tree_map(
       lambda x: jnp.sum(jnp.square(x)), obj)
 
   return jnp.sqrt(sum(jax.tree_util.tree_leaves(elements_squared_norm)))
 
@@ -325,39 +355,70 @@
   per_param_norm = tree.flatten_with_path(per_param_norm)
 
   return {
       key_prefix + "(" + "/".join(k) + ")": v for k, v in per_param_norm
   }
 
 
-def psd_inv_cholesky(matrix: Array, damping: Array) -> Array:
-  """Computes the inverse of `matrix + damping*I`, with matrix assumed PSD."""
+def psd_inv(matrix: Array) -> Array:
+  """Computes the inverse of `matrix`, which is assumed PSD."""
+
+  if matrix.shape[:1] != matrix.shape[1:]:
+    raise ValueError(f"Expected square matrix, but got shape {matrix.shape}.")
+
+  if get_use_cholesky_inversion():
+    identity = jnp.eye(matrix.shape[0], dtype=matrix.dtype)
+    return linalg.solve(matrix, identity, assume_a="pos")
+  else:
+    return linalg.inv(matrix)
+
+
+def psd_solve(matrix: Array, vector: Array) -> Array:
+  """Computes the solution of `matrix * x = vector`, for a PSD `matrix`."""
 
   if matrix.shape[:1] != matrix.shape[1:]:
     raise ValueError(f"Expected square matrix, but got shape {matrix.shape}.")
 
-  identity = jnp.eye(matrix.shape[0], dtype=matrix.dtype)
+  if get_use_cholesky_inversion():
+    return linalg.solve(matrix, vector, assume_a="pos")
+
+  else:
+    return linalg.solve(matrix, vector)
 
-  return linalg.solve(matrix + damping * identity, identity, assume_a="pos")
+
+def psd_solve_without_last_idx(a: Array, b: Array) -> Array:
+  sub_a = a[..., :-1, :-1]
+  sub_b = b[..., :-1]
+  sub_x = psd_solve(sub_a, sub_b)
+  return jnp.concatenate([sub_x, jnp.zeros_like(b[..., :1])], axis=-1)
+
+
+def psd_solve_maybe_zero_last_idx(a: Array, b: Array) -> Array:
+  # Check the last column and row are zero.
+  check = jnp.logical_and(jnp.all(a[..., -1] == 0), jnp.all(a[..., -1, :] == 0))
+  return jax.lax.cond(check, psd_solve_without_last_idx, psd_solve, a, b)
 
 
 def psd_matrix_norm(
     matrix: Array,
-    norm_type: str = "avg_trace",
+    norm_type: str = "avg_diag",
     method_2norm: str = "lobpcg",
     rng_key: Optional[PRNGKey] = None
-) -> Array:
+) -> Numeric:
   """Computes one of several different matrix norms for PSD matrices.
 
+  NOTE: not all the functions options provided here are actually norms, but most
+  are.
+
   Args:
     matrix: a square matrix represented as a 2D array, a 1D vector giving the
       diagonal, or a 0D scalar (which gets interpreted as a 1x1 matrix). Must be
       positive semi-definite (PSD).
     norm_type: a string specifying the type of matrix norm. Can be "2_norm" for
-      the matrix 2-norm aka the spectral norm, "avg_trace" for the average of
+      the matrix 2-norm aka the spectral norm, "avg_diag" for the average of
       diagonal entries, "1_norm" for the matrix 1-norm, or "avg_fro" for the
       Frobenius norm divided by the square root of the number of rows.
     method_2norm: a string specifying the method used to compute 2-norms. Can
       be "lobpcg" (recommended) or "power_iteration".
     rng_key: an optional JAX PRNGKey key to used initialize the lobpcg method
       for computing the 2-norm.
 
@@ -382,38 +443,97 @@
 
         v = jax.random.normal(rng_key, shape=[matrix.shape[0], 1])
 
         return experimental_splinalg.lobpcg_standard(
             matrix, v, m=300, tol=1e-8)[0][0]
 
       elif method_2norm == "power_iteration":
-        return optax.power_iteration(
-            matrix, num_iters=300, error_tolerance=1e-7)[1]
+
+        return float(optax.power_iteration(
+            matrix, num_iters=300, error_tolerance=1e-7)[0])
 
       else:
         raise ValueError(f"Unrecognized method string: '{norm_type}'")
 
     else:
       raise ValueError(f"Unsupported shape for factor array: {matrix.shape}")
 
-  elif norm_type == "avg_trace":
+  elif norm_type == "avg_diag":
 
     if matrix.ndim == 0:
       return matrix
 
     elif matrix.ndim == 1:
       return jnp.sum(matrix) / matrix.shape[0]
 
     elif matrix.ndim == 2 and matrix.shape[0] == matrix.shape[1]:
       return jnp.trace(matrix) / matrix.shape[0]
 
     else:
       raise ValueError(f"Unsupported shape for factor array: {matrix.shape}")
 
-  elif norm_type == "1_norm":
+  elif norm_type == "median_diag":
+
+    if matrix.ndim == 0:
+      return matrix
+
+    elif matrix.ndim == 1:
+      return jnp.median(matrix)
+
+    elif matrix.ndim == 2 and matrix.shape[0] == matrix.shape[1]:
+      return jnp.median(jnp.diag(matrix))
+
+    else:
+      raise ValueError(f"Unsupported shape for factor array: {matrix.shape}")
+
+  elif norm_type == "trace":
+
+    if matrix.ndim == 0:
+      return matrix
+
+    elif matrix.ndim == 1:
+      return jnp.sum(matrix)
+
+    elif matrix.ndim == 2 and matrix.shape[0] == matrix.shape[1]:
+      return jnp.trace(matrix)
+
+    else:
+      raise ValueError(f"Unsupported shape for factor array: {matrix.shape}")
+
+  elif norm_type == "median_eig":
+
+    if matrix.ndim == 0:
+      return matrix
+
+    elif matrix.ndim == 1:
+      return jnp.median(matrix)
+
+    elif matrix.ndim == 2 and matrix.shape[0] == matrix.shape[1]:
+      # call safe_psd_eigh instead?
+      s, _ = jnp.linalg.eigh(matrix)
+      return jnp.median(s)
+
+    else:
+      raise ValueError(f"Unsupported shape for factor array: {matrix.shape}")
+
+  elif norm_type == "one_over_dim":  # this isn't a norm
+
+    if matrix.ndim == 0:
+      return 1.0
+
+    elif matrix.ndim == 1:
+      return 1.0 / matrix.shape[0]
+
+    elif matrix.ndim == 2 and matrix.shape[0] == matrix.shape[1]:
+      return 1.0 / matrix.shape[0]
+
+    else:
+      raise ValueError(f"Unsupported shape for factor array: {matrix.shape}")
+
+  elif norm_type == "1_norm":  # equiv to inf norm for symmetric matrices
 
     if matrix.ndim == 0:
       return matrix
 
     elif matrix.ndim == 1:
       return jnp.max(matrix)
 
@@ -433,127 +553,234 @@
 
     elif matrix.ndim == 2 and matrix.shape[0] == matrix.shape[1]:
       return jnp.linalg.norm(matrix) / jnp.sqrt(matrix.shape[0])
 
     else:
       raise ValueError(f"Unsupported shape for factor array: {matrix.shape}")
 
-  else:
-    raise ValueError(f"Unrecognized norm type: '{norm_type}'")
+  elif norm_type == "fro":
 
+    if matrix.ndim == 0:
+      return matrix
 
-def pi_adjusted_kronecker_inverse(
-    *arrays: Array,
-    damping: Numeric,
+    elif matrix.ndim == 1:
+      return jnp.linalg.norm(matrix)
+
+    elif matrix.ndim == 2 and matrix.shape[0] == matrix.shape[1]:
+      return jnp.linalg.norm(matrix)
+
+    else:
+      raise ValueError(f"Unsupported shape for factor array: {matrix.shape}")
+
+  raise ValueError(f"Unrecognized norm type: '{norm_type}'")
+
+
+def pi_adjusted_kronecker_factors(
+    *factors: Array,
+    damping: Numeric
 ) -> Tuple[Array, ...]:
-  """Computes pi-adjusted factored damping inverses.
+  """Computes Kronecker factors with pi-adjusted factored damping.
 
-  The inverse of `a_1 kron a_2 kron ... kron a_n + damping * I` is not Kronecker
-  factored in general, because of the added identity. [1] proposed a pi-adjusted
-  factored damping approach to approximate the inverse as a Kronecker product.
-  [2] generalized this approach from two to tree factors, and [3] generalized it
-  to arbitrary numbers of factors. This function implements the generalized
-  approach.
+  The `f1 kron f2 kron ... kron fn + damping * I` is not a Kronecker product
+  in general, because of the added identity. [1] proposed a pi-adjusted factored
+  damping approach to approximate it as a Kronecker product. [2] generalized
+  this approach from two to tree factors, and [3] generalized it to arbitrary
+  numbers of factors. This function implements the generalized approach.
 
   [1] - https://arxiv.org/abs/1503.05671
   [2] - https://openreview.net/forum?id=SkkTMpjex
   [3] - https://ui.adsabs.harvard.edu/abs/2021arXiv210602925R/abstract
 
   Args:
-    *arrays: A list of matrices, vectors (which are interpreted
-      as representing the diagonal of a matrix) or scalars (which are
-      interpreted as being a 1x1 matrix). All matrices must be PSD.
+    *factors: A list of factors represented as 2D arrays, vectors (which are
+      interpreted as representing the diagonal of a matrix) or scalars (which
+      are interpreted as being a 1x1 matrix). All factors must be PSD.
     damping: The weight of the identity added to the Kronecker product.
 
   Returns:
-    A list of factors with the same length as the input `arrays` whose Kronecker
-    product approximates the inverse of `a_1 kron ... kron a_n + damping * I`.
+    A list of factors with the same length as `factors`, and with the same
+    corresponding representations, whose Kronecker product approximates
+    `(f1 kron f2 kron ... kron fn) + damping * I` according to the
+    pi-adjusted factored-damping approach.
   """
+
   # The implementation writes each single factor as `c_i u_i`, where the matrix
   # `u_i` is such that `trace(u_i) / dim(u_i) = 1`. We then factor out all the
   # scalar factors `c_i` into a single overall scaling coefficient and
-  # distribute the damping to each single non-scalar factor `u_i` equally before
-  # inverting them.
+  # distribute the damping to each single non-scalar factor `u_i` equally.
 
-  norm_type = "avg_trace"
+  norm_type = "avg_diag"
 
-  norms = [psd_matrix_norm(a, norm_type=norm_type) for a in arrays]
+  norms = jnp.array([psd_matrix_norm(f, norm_type=norm_type) for f in factors])
 
   # Compute the normalized factors `u_i`, such that Trace(u_i) / dim(u_i) = 1
-  us = [ai / ni for ai, ni in zip(arrays, norms)]
+  us = [fi / ni for fi, ni in zip(factors, norms)]
+
+  k = len(factors)
+
+  # TODO(jamesmartens,botev): consider making the use of special behavior for
+  # scalar factors a module-level configurable option. One can argue that scalar
+  # factors should behave the same as non-scalar factors for the sake of
+  # consistent behavior as the layer widths shrink to 1.
+
+  def regular_case() -> Tuple[Array, ...]:
+
+    num_non_scalars = sum(1 if f.size != 1 else 0 for f in factors)
+
+    if num_non_scalars != 0:
+
+      # Distribute c and damping/c among k factors, where c = jnp.prod(norms),
+      # satisfying kron(factors) = c * kron(us).
 
-  # kron(arrays) = c * kron(us)
+      # NOTE: c_k (geometric mean of norms) can also be calculated by
+      # c ** (1/k) = jnp.prod(norms) ** (1 / len(norms)), but this alternative
+      # can make the result zero due to the multiplication of (potentially)
+      # small values, i.e. jnp.prod(norms).
+      c_k = jnp.exp(jnp.mean(jnp.log(norms)))
 
-  c = jnp.prod(jnp.array(norms))
+      d_k = jnp.power(damping, 1.0 / k) / c_k
 
-  damping = damping.astype(c.dtype)  # pytype: disable=attribute-error  # numpy-scalars
+      if k > num_non_scalars:
 
-  def regular_inverse() -> Tuple[Array, ...]:
+        c_non_scalar = c_k ** (float(k) / num_non_scalars)
 
-    non_scalars = sum(1 if a.size != 1 else 0 for a in arrays)
+        # We distribute the damping only inside the non-scalar factors
+        d_hat = jnp.power(damping, 1.0 / num_non_scalars) / c_non_scalar
 
-    # We distribute the damping only inside the non-scalar factors
-    d_hat = jnp.power(damping / c, 1.0 / non_scalars)
+      else:
+        d_hat = d_k
 
-    # We distribute the overall scale over each factor, including scalars
-    if non_scalars == 0:
-      # In the case where all factors are scalar we need to add the damping
-      c_k = jnp.power(c + damping, 1.0 / len(arrays))
     else:
-      c_k = jnp.power(c, 1.0 / len(arrays))
 
-    u_hats_inv = []
+      # This could cause under/overflow, but it's unavoidable here.
+      c = jnp.prod(jnp.array(norms))
+
+      # In the case where all factors are scalar we need to add the damping and
+      # then take the k-th root
+      c_k = jnp.power(c + damping, 1.0 / k)
+
+    u_hats = []
 
     for u in us:
 
-      if u.size == 1:
-        inv = jnp.ones_like(u)  # damping not used in the scalar factors
+      if u.size == 1:  # scalar case
+        u_hat = jnp.ones_like(u)  # damping not used in the scalar factors
 
       elif u.ndim == 2:
-        inv = psd_inv_cholesky(u, d_hat)
+        u_hat = u + d_hat * jnp.eye(u.shape[0], dtype=u.dtype)
 
       else:  # diagonal case
         assert u.ndim == 1
-        inv = 1.0 / (u + d_hat)
+        u_hat = u + d_hat
 
-      u_hats_inv.append(inv / c_k)
+      u_hats.append(u_hat * c_k)
 
-    return tuple(u_hats_inv)
+    return tuple(u_hats)
 
-  def zero_inverse() -> Tuple[Array, ...]:
+  def zero_case() -> Tuple[Array, ...]:
 
     # In the special case where for some reason one of the factors is zero, then
-    # the inverse is just `damping^-1 * I`, hence we write each factor as
-    # `damping^(1/k) * I`.
+    # the we write each factor as `damping^(1/k) * I`.
 
-    c_k = jnp.power(damping, 1.0 / len(arrays))
+    c_k = jnp.power(damping, 1.0 / k)
 
-    u_hats_inv = []
+    u_hats = []
 
     for u in us:
 
       if u.ndim == 2:
-        inv = jnp.eye(u.shape[0], dtype=u.dtype)
+        u_hat = jnp.eye(u.shape[0], dtype=u.dtype)
 
       else:
-        inv = jnp.ones_like(u)
+        u_hat = jnp.ones_like(u)
 
-      u_hats_inv.append(inv / c_k)
+      u_hats.append(u_hat * c_k)
 
-    return tuple(u_hats_inv)
+    return tuple(u_hats)
 
   if get_special_case_zero_inv():
-
-    return lax.cond(
-        jnp.greater(c, 0.0),
-        regular_inverse,
-        zero_inverse)
+    return lax.cond(jnp.greater(jnp.min(norms), 0.0), regular_case, zero_case)
 
   else:
-    return regular_inverse()
+    return regular_case()
+
+
+def invert_psd_matrices(
+    matrices: ArrayTree
+) -> ArrayTree:
+  """Inverts a PyTree of matrices.
+
+  Args:
+    matrices: A PyTree of 2D arrays, vectors (which are interpreted as
+      representing the diagonal of a matrix) or scalars (which are interpreted
+      as being a 1x1 matrix) representing the matrices to be inverted. All
+      matrices must be PSD.
+
+  Returns:
+    A PyTree of matrices giving the inverses of the corresponding matrices
+    passed as arguments (with the same respective representations).
+  """
+
+  def invert_psd_matrix(m):
+
+    if m.ndim == 2:
+      return psd_inv(m)
+
+    assert m.ndim <= 1
+    return 1.0 / m
+
+  return jax.tree_map(invert_psd_matrix, matrices)
+
+
+def inverse_sqrt_psd_matrices(matrices: ArrayTree) -> ArrayTree:
+
+  def inverse_sqrt_psd_matrix(m):
+
+    if m.ndim == 2:
+      # Check copy.bara.sky before changing the next line:
+      return qr_pth_inv_root.qr_pth_inv_root(4, m, cholesky_qr=True)
+
+    assert m.ndim <= 1
+    return 1.0 / jnp.sqrt(m)
+
+  return jax.tree_map(inverse_sqrt_psd_matrix, matrices)
+
+
+def pi_adjusted_kronecker_inverse(
+    *factors: Array,
+    damping: Numeric,
+) -> Tuple[Array, ...]:
+  """Computes pi-adjusted factored damping inverses.
+
+  The inverse of `(f1 kron f2 kron ... kron fn) + damping * I` is not Kronecker
+  factored in general, because of the added identity. [1] proposed a pi-adjusted
+  factored damping approach to approximate the inverse as a Kronecker product.
+  [2] generalized this approach from two to tree factors, and [3] generalized it
+  to arbitrary numbers of factors. This function implements the generalized
+  approach.
+
+  [1] - https://arxiv.org/abs/1503.05671
+  [2] - https://openreview.net/forum?id=SkkTMpjex
+  [3] - https://ui.adsabs.harvard.edu/abs/2021arXiv210602925R/abstract
+
+  Args:
+    *factors: A list of factors represented as 2D arrays, vectors (which are
+      interpreted as representing the diagonal of a matrix) or scalars (which
+      are interpreted as being a 1x1 matrix). All factors must be PSD.
+    damping: The weight of the identity added to the Kronecker product.
+
+  Returns:
+    A list of factors with the same length as `factors`, and with the same
+    corresponding representations, whose Kronecker product approximates the
+    inverse of `(f1 kron f2 kron ... kron fn) + damping * I` according to the
+    pi-adjusted factored-damping approach.
+  """
+
+  return invert_psd_matrices(
+      pi_adjusted_kronecker_factors(*factors, damping=damping))  # pytype: disable=bad-return-type
 
 
 def kronecker_product_axis_mul_v(
     factors: Sequence[Array],
     v: Array,
     axis_groups: Optional[Sequence[Sequence[int]]] = None,
     transpose: Union[bool, Sequence[bool]] = False,
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/utils/misc.py` & `kfac-jax-0.0.6/kfac_jax/_src/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC related utility classes and functions."""
 import abc
 import dataclasses
 import functools
-from typing import Any, Iterator, Sequence, Type, Tuple, Union, Dict, TypeVar
+import inspect
+from typing import Any, Callable, Iterator, Sequence, Type, Tuple, Union, Dict, TypeVar
 
 import jax
 import jax.numpy as jnp
 from kfac_jax._src.utils import types
 
+T = types.T
 Array = types.Array
 Numeric = types.Numeric
 ArrayTree = types.ArrayTree
 TArrayTree = types.TArrayTree
 StateType = TypeVar("StateType")
 StateTree = types.PyTree["State"]
 
@@ -108,43 +110,42 @@
   def field_types(cls) -> Dict[str, Type[Any]]:
     return {field.name: field.type for field in dataclasses.fields(cls)}  # pytype: disable=wrong-arg-types
 
   @property
   def field_values(self) -> Tuple[ArrayTree, ...]:
     return tuple(getattr(self, name) for name in self.field_names())
 
-  def copy(self):
+  def copy(self: StateType) -> StateType:
     """Returns a copy of the PyTree structure (but not the JAX arrays)."""
     (flattened, structure) = jax.tree_util.tree_flatten(self)
     return jax.tree_util.tree_unflatten(structure, flattened)
 
-  def tree_flatten(self) -> Tuple[Tuple[ArrayTree, ...], None]:
-    return self.field_values, None
+  def tree_flatten(self) -> Tuple[Tuple[ArrayTree, ...], Tuple[str, ...]]:
+    return self.field_values, self.field_names()
 
   @classmethod
   def tree_unflatten(
       cls,
-      aux_data: None,
+      aux_data: Tuple[str, ...],
       children: Tuple[ArrayTree, ...],
   ):
-    del aux_data  # not used
-    return cls(**dict(zip(cls.field_names(), children)))
+    return cls(**dict(zip(aux_data, children)))
 
   def __repr__(self) -> str:
     return (f"{self.__class__.__name__}(" +
             ",".join(f"{name}={v!r}" for name, v in self.field_values) +
             ")")
 
 
 def register_state_class(class_type: Type[Any]) -> Type[Any]:
   """Extended dataclass decorator, which also registers the class as a PyTree.
 
   The function is equivalent to `dataclasses.dataclass`, but additionally
-  registers the `class_type` as a PyTree. This is done done by setting the
-  PyTree nodes to all of the `dataclasses.fields` of the class.
+  registers the `class_type` as a PyTree. This is done by setting the PyTree
+  nodes of all `dataclasses.fields` of the class.
 
   Args:
     class_type: The class type to transform.
 
   Returns:
     The transformed `class_type` which is now a dataclass and also registered as
     a PyTree.
@@ -269,29 +270,29 @@
 
       super().__setattr__(name, value)
 
     else:
       raise AttributeError("Can't set attributes after finalization.")
 
 
-def auto_scope_method(method):
+def auto_scope_method(method: Callable[..., T]) -> Callable[..., T]:
   """Wraps the method call to have automatically generated Jax name scope."""
   @functools.wraps(method)
   def wrapped(instance, *args, **kwargs):
     class_name = type(instance).__name__
     method_name = method.__name__
     if method_name.startswith("_"):
       method_name = method_name[1:]
     with jax.named_scope(f"{class_name}_{method_name}"):
       return method(instance, *args, **kwargs)
 
   return wrapped
 
 
-def auto_scope_function(func):
+def auto_scope_function(func: Callable[..., T]) -> Callable[..., T]:
   """Wraps the function call to have automatically generated Jax name scope."""
   @functools.wraps(func)
   def wrapped(*args, **kwargs):
     with jax.named_scope(func.__name__):
       return func(*args, **kwargs)
 
   return wrapped
@@ -301,7 +302,19 @@
   """Computes the batch size as the size of axis `0` of the first element."""
   return jax.tree_util.tree_leaves(batch)[0].shape[0]
 
 
 def replace_char(original: str, new_str: str, index: int) -> str:
   """Replaces the character at a given location."""
   return original[:index] + new_str + original[index + 1 :]
+
+
+def call_func_with_conditional_kwargs(
+    func: Callable[..., T],
+    *func_args: Any,
+    **kwargs: Any,
+) -> T:
+
+  sig = inspect.signature(func)
+  func_kwargs = {k: v for k, v in kwargs.items() if k in sig.parameters}
+
+  return func(*func_args, **func_kwargs)
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/utils/parallel.py` & `kfac-jax-0.0.6/kfac_jax/_src/utils/parallel.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC utilities for multi-device execution."""
 import functools
-import numbers
 from typing import Callable, Optional, Sequence
 
 import jax
 from jax import core
 from jax import lax
 import jax.numpy as jnp
 
@@ -56,19 +55,28 @@
   def p_func_if_pmap(obj: TArrayTree, axis_name: Optional[str]) -> TArrayTree:
 
     return p_func(obj, axis_name) if in_pmap(axis_name) else obj
 
   return p_func_if_pmap
 
 
-pmean_if_pmap = wrap_if_pmap(lax.pmean)
-psum_if_pmap = wrap_if_pmap(lax.psum)
+# TODO(jamesmartens,botev): We no longer use wrap_if_pmap in the below
+# definitions since it doesn't seem to transmit type info properly. Investigate?
+def pmean_if_pmap(obj: TArrayTree, axis_name: Optional[str]) -> TArrayTree:
 
-compute_mean = jax.pmap(lambda x: lax.pmean(x, "i"), axis_name="i")
-compute_sum = jax.pmap(lambda x: lax.psum(x, "i"), axis_name="i")
+  return lax.pmean(obj, axis_name) if in_pmap(axis_name) else obj
+
+
+def psum_if_pmap(obj: TArrayTree, axis_name: Optional[str]) -> TArrayTree:
+
+  return lax.psum(obj, axis_name) if in_pmap(axis_name) else obj
+
+
+pmap_mean = jax.pmap(lambda x: lax.pmean(x, "i"), axis_name="i")
+pmap_sum = jax.pmap(lambda x: lax.psum(x, "i"), axis_name="i")
 
 
 def index_if_not_scalar(value: Numeric, index: int = 0) -> Numeric:
   """Index `value` at axis 0 if it is not a scalar, otherwise return it."""
 
   if isinstance(value, Array):
 
@@ -80,28 +88,27 @@
   elif isinstance(value, (float, int)):
     return value
 
   else:
     raise ValueError("The input should be an instance of `Numeric`.")
 
 
-@jax.jit
 def get_first(obj: TArrayTree) -> TArrayTree:
   """Index the PyTree leaves `x` of `obj` by `x[0]` if they are not scalars."""
   return jax.tree_util.tree_map(index_if_not_scalar, obj)
 
 
 def get_mean(obj: TArrayTree) -> TArrayTree:
   """Returns the average of `obj` over different devices."""
-  return get_first(compute_mean(obj))
+  return get_first(pmap_mean(obj))
 
 
 def get_sum(obj: TArrayTree) -> TArrayTree:
   """Returns the sum of `obj` over different devices."""
-  return get_first(compute_sum(obj))
+  return get_first(pmap_sum(obj))
 
 
 broadcast_all_local_devices = jax.pmap(lambda x: x)
 pmap_zeros_like = jax.pmap(lambda x: jax.tree_util.tree_map(jnp.zeros_like, x))
 jit_zeros_like = jax.jit(lambda x: jax.tree_util.tree_map(jnp.zeros_like, x))
 
 
@@ -123,32 +130,14 @@
 
 
 p_split = jax.pmap(lambda key: tuple(jax.random.split(key)))
 p_split_num = jax.pmap(lambda key, num: tuple(jax.random.split(key, num)),
                        static_broadcasted_argnums=1)
 
 
-def check_and_fix_format_for_pmap(obj: TArrayTree) -> TArrayTree:
-  """Checks shape[0]==device_count and broadcasts scalars to [device_count]."""
-  device_count = jax.local_device_count()
-
-  def check_and_fix(x: Numeric) -> Array:
-
-    # broadcast any 0D scalars
-    if isinstance(x, numbers.Number) or not x.shape:  # pytype: disable=attribute-error  # numpy-scalars
-      return jnp.stack([x] * device_count, axis=0)
-
-    # otherwise, ensure that arrays have the right shape
-    assert x.shape[0] == device_count  # pytype: disable=attribute-error  # numpy-scalars
-
-    return x  # pytype: disable=bad-return-type  # numpy-scalars
-
-  return jax.tree_util.tree_map(check_and_fix, obj)
-
-
 default_device_sync = None
 
 
 def host_sync(
     obj: TArrayTree,
     sync_op: Callable[[TArrayTree, str], TArrayTree],
 ) -> TArrayTree:
@@ -198,30 +187,44 @@
     axis_name: Optional[str] = None,
 ) -> TArrayTree:
   """Computes the mean of `value` over all hosts and divides it by `counter`."""
   value = jax.tree_util.tree_map(lambda x: x / counter, value)
   return pmean_if_pmap(value, axis_name)
 
 
-jit_sync_and_divide_value = jax.jit(sync_and_divide_value, donate_argnums=0)
+jit_sync_and_divide_value = jax.jit(sync_and_divide_value)
 pmap_sync_and_divide_value = jax.pmap(
     functools.partial(sync_and_divide_value, axis_name="i"),
     axis_name="i",
-    donate_argnums=0,
 )
 
 
-# We might be able to change this to "return jnp.array(x)" in newer JAX versions
+# We might be able to change this to "return jnp.array(x)" in newer JAX
+# versions. Or maybe we can use jnp.copy now?
 def copy_array(x: Array) -> Array:
   """Copies a Jax array so that it can be donated freely."""
   return x + jnp.zeros_like(x)
 
 
 copy_obj = jax.jit(lambda x: jax.tree_util.tree_map(copy_array, x))
-pmap_copy_obj = jax.pmap(copy_obj)
+_pmap_copy_obj = jax.pmap(copy_obj)
+
+
+def pmap_copy_obj(x: Optional[TArrayTree]) -> Optional[TArrayTree]:
+
+  # pmap will fail to work if passed a totally empty tree
+  if x is None:
+    return None
+
+  if types.tree_is_empty(x):
+    # this does a shallow copy of the tree similar to .copy():
+    (flattened, structure) = jax.tree_util.tree_flatten(x)
+    return jax.tree_util.tree_unflatten(structure, flattened)
+
+  return _pmap_copy_obj(x)
 
 
 def distribute_thunks(
     thunks: Sequence[Callable[[], TArrayTree]],
     pmap_axis_name: str,
     ) -> TArrayTree:
   """Distributes the computation of a list of thunks over the pmapped devices.
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/utils/staging.py` & `kfac-jax-0.0.6/kfac_jax/_src/utils/staging.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC utilities for classes with staged methods."""
 import functools
+import numbers
 import operator
 from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 
 from kfac_jax._src.utils import misc
@@ -112,15 +113,15 @@
     """Returns a staging context manager, linked to this instance."""
     return self.StagingContext(self)
 
   def get_first(self, obj: TArrayTree) -> TArrayTree:
     """Indexes the `obj` PyTree leaves over leading axis if `multi_device`."""
     return parallel.get_first(obj) if self.multi_device else obj
 
-  def copy_obj(self, obj: TArrayTree) -> TArrayTree:
+  def copy_obj(self, obj: Optional[TArrayTree]) -> Optional[TArrayTree]:
     """Copies the object."""
     if self.multi_device:
       return parallel.pmap_copy_obj(obj)
     else:
       return parallel.copy_obj(obj)
 
   def replicate(self, obj: TArrayTree) -> TArrayTree:
@@ -216,33 +217,39 @@
 
         outs = jax.tree_util.tree_map(lambda *args_: jnp.stack(args_), *outs)
 
       elif instance.debug:
         outs = method(instance, *args)
 
       elif instance.multi_device:
-
-        new_args = list(args)
-
+        # Compute in_axes so we broadcast any argument that is a scalar
+        in_axes = [None]
         for i in range(len(args)):
-          if i + 1 not in static_argnums:
-            new_args[i] = parallel.check_and_fix_format_for_pmap(args[i])
-
-        func = pmap_funcs.get(instance.pmap_axis_name)
+          if (isinstance(args[i], numbers.Number) or
+              (isinstance(args[i], jax.Array) and not args[i].shape)):
+            # Single scalar
+            in_axes.append(None)
+          else:
+            in_axes.append(0)
+
+        in_axes = tuple(in_axes)
+        key = (instance.pmap_axis_name, in_axes)
+        func = pmap_funcs.get(key)
 
         if func is None:
           func = jax.pmap(
               method,
               static_broadcasted_argnums=static_argnums,
               donate_argnums=donate_argnums,
               axis_name=instance.pmap_axis_name,
+              in_axes=in_axes,
           )
-          pmap_funcs[instance.pmap_axis_name] = func
+          pmap_funcs[key] = func
 
-        outs = func(instance, *new_args)
+        outs = func(instance, *args)
 
       else:
         outs = jitted_func(instance, *args)
 
     return outs
 
   return decorated
```

### Comparing `kfac-jax-0.0.5/kfac_jax/_src/utils/types.py` & `kfac-jax-0.0.6/kfac_jax/_src/utils/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC annotation types and general tree operations."""
-from typing import Callable, TypeVar, Sequence, Mapping, Tuple, Union
+from typing import Dict, Callable, Mapping, Sequence, Tuple, TypeVar, Union
 
 import jax
 import jax.numpy as jnp
 
 # Types for annotation
 T = TypeVar("T")
 Array = jax.Array
@@ -27,15 +27,15 @@
 DType = jnp.dtype
 PyTree = Union[T, Sequence["PyTree[T]"], Mapping[str, "PyTree[T]"]]
 ArrayTree = PyTree[Array]
 TArrayTree = TypeVar("TArrayTree", bound=ArrayTree)
 Params = TypeVar("Params", bound=ArrayTree)
 Batch = TypeVar("Batch", bound=ArrayTree)
 FuncState = TypeVar("FuncState", bound=ArrayTree)
-FuncAux = TypeVar("FuncAux", bound=ArrayTree)
+FuncAux = Dict[str, ArrayTree]
 PyTreeDef = jax.tree_util.PyTreeDef
 FuncArgs = Sequence[ArrayTree]
 FuncOuts = Union[Array, Tuple[Array, FuncAux]]
 Func = Callable[..., FuncOuts]
 ValueFunc = Callable[..., Array]
 ValueAndGradFunc = Callable[..., Tuple[Array, Params]]
 AssumedFuncOutput = Union[Array, Tuple[Array, FuncAux],
@@ -66,18 +66,19 @@
 
   leaves = jax.tree_util.tree_leaves(obj)
 
   dtype = None
 
   for leaf in leaves:
 
-    if leaf.dtype in (jnp.float16, jnp.bfloat16, jnp.float32, jnp.float64):
+    if (leaf.dtype == jnp.float16 or leaf.dtype == jnp.bfloat16
+        or leaf.dtype == jnp.float32 or leaf.dtype == jnp.float64):
 
       if dtype is not None and leaf.dtype != dtype:
         raise ValueError("Inconsistent dtypes detected.")
       else:
         dtype = leaf.dtype
 
     else:
       raise ValueError("Non-float dtype detected.")
 
-  return dtype
+  return dtype  # pytype: disable=bad-return-type  # jnp-type
```

### Comparing `kfac-jax-0.0.5/kfac_jax.egg-info/PKG-INFO` & `kfac-jax-0.0.6/kfac_jax.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: kfac-jax
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Jax package for approximate curvature estimation and optimization using KFAC.
-Home-page: https://github.com/deepmind/kfac-jax
+Home-page: https://github.com/google-deepmind/kfac-jax
 Author: DeepMind
 Author-email: kfac-jax-dev@google.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -15,45 +15,64 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: absl-py>=0.12.0
+Requires-Dist: immutabledict>=2.2.1
+Requires-Dist: numpy>=1.21
+Requires-Dist: distrax>=0.1.3
+Requires-Dist: jax>=0.4.7
+Requires-Dist: jaxlib>=0.4.7
+Requires-Dist: dm-tree>=0.1.7
+Requires-Dist: optax>=0.1.4
+Requires-Dist: typing_extensions>=4.2.0; python_version < "3.10"
+Provides-Extra: tests
+Requires-Dist: pytest-xdist; extra == "tests"
+Requires-Dist: absl-py==0.12.0; extra == "tests"
+Requires-Dist: immutabledict==2.2.1; extra == "tests"
+Requires-Dist: numpy==1.21; extra == "tests"
+Requires-Dist: distrax==0.1.3; extra == "tests"
+Requires-Dist: jax==0.4.7; extra == "tests"
+Requires-Dist: jaxlib==0.4.7; extra == "tests"
+Requires-Dist: dm-haiku==0.0.9; extra == "tests"
+Requires-Dist: dm-tree==0.1.7; extra == "tests"
+Requires-Dist: optax==0.1.4; extra == "tests"
 
 # KFAC-JAX - Second Order Optimization with Approximate Curvature in JAX
 
 [**Installation**](#installation)
 | [**Quickstart**](#quickstart)
 | [**Documentation**](https://kfac-jax.readthedocs.io/)
-| [**Examples**](https://github.com/deepmind/kfac-jax/tree/main/examples/)
+| [**Examples**](https://github.com/google-deepmind/kfac-jax/tree/main/examples/)
 | [**Citing KFAC-JAX**](#citing-kfac-jax)
 
-![CI status](https://github.com/deepmind/kfac-jax/workflows/ci/badge.svg)
+![CI status](https://github.com/google-deepmind/kfac-jax/workflows/ci/badge.svg)
 ![docs](https://readthedocs.org/projects/kfac-jax/badge/?version=latest)
 ![pypi](https://img.shields.io/pypi/v/kfac-jax)
 
-KFAC-JAX is a library built on top of [JAX] for second-order optimization of 
+KFAC-JAX is a library built on top of [JAX] for second-order optimization of
 neural networks and for computing scalable curvature approximations.
-The main goal of the library is to provide researchers with an easy-to-use 
+The main goal of the library is to provide researchers with an easy-to-use
 implementation of the [K-FAC] optimizer and curvature estimator.
 
 ## Installation<a id="installation"></a>
 
 KFAC-JAX is written in pure Python, but depends on C++ code via JAX.
 
 First, follow [these instructions](https://github.com/google/jax#installation)
 to install JAX with the relevant accelerator support.
 
 Then, install KFAC-JAX using pip:
 
 ```bash
-$ pip install git+https://github.com/deepmind/kfac-jax
+$ pip install git+https://github.com/google-deepmind/kfac-jax
 ```
 
 Alternatively, you can install via PyPI:
 
 ```bash
 $ pip install -U kfac-jax
 ```
@@ -62,15 +81,15 @@
 
 ```bash
 $ pip install -r requirements_examples.txt
 ```
 
 ## Quickstart<a id="quickstart"></a>
 
-Let's take a look at a simple example of training a neural network, defined 
+Let's take a look at a simple example of training a neural network, defined
 using [Haiku], with the K-FAC optimizer:
 
 ```python
 import haiku as hk
 import jax
 import jax.numpy as jnp
 import kfac_jax
@@ -80,22 +99,22 @@
 L2_REG = 1e-3
 NUM_BATCHES = 100
 
 
 def make_dataset_iterator(batch_size):
   # Dummy dataset, in practice this should be your dataset pipeline
   for _ in range(NUM_BATCHES):
-    yield jnp.zeros([batch_size, 100]), jnp.ones([batch_size], dtype="int32") 
+    yield jnp.zeros([batch_size, 100]), jnp.ones([batch_size], dtype="int32")
 
 
 def softmax_cross_entropy(logits: jnp.ndarray, targets: jnp.ndarray):
   """Softmax cross entropy loss."""
   # We assume integer labels
   assert logits.ndim == targets.ndim + 1
-  
+
   # Tell KFAC-JAX this model represents a classifier
   # See https://kfac-jax.readthedocs.io/en/latest/overview.html#supported-losses
   kfac_jax.register_softmax_cross_entropy_loss(logits, targets)
   log_p = jax.nn.log_softmax(logits, axis=-1)
   return - jax.vmap(lambda x, y: x[y])(log_p, targets)
 
 
@@ -113,15 +132,15 @@
 
 
 def loss_fn(model_params, model_batch):
   """The loss function to optimize."""
   x, y = model_batch
   logits = hk_model.apply(model_params, x)
   loss = jnp.mean(softmax_cross_entropy(logits, y))
-  
+
   # The optimizer assumes that the function you provide has already added
   # the L2 regularizer to its gradients.
   return loss + L2_REG * kfac_jax.utils.inner_product(params, params) / 2.0
 
 
 # Create the optimizer
 optimizer = kfac_jax.Optimizer(
@@ -155,55 +174,55 @@
 
 ### Do not stage (``jit`` or ``pmap``) the optimizer
 
 You should not apply `jax.jit` or `jax.pmap` to the call to `Optimizer.step`.
 This is already done for you automatically by the optimizer class.
 To control the staging behaviour of the optimizer set the flag ``multi_device``
 to ``True`` for ``pmap`` and to ``False`` for ``jit``.
- 
+
 ### Do not stage (``jit`` or ``pmap``) the loss function
 
-The ``value_and_grad_func`` argument provided to the optimizer should compute 
-the loss function value and its gradients. Since the optimizer already stages 
+The ``value_and_grad_func`` argument provided to the optimizer should compute
+the loss function value and its gradients. Since the optimizer already stages
 its step function internally, applying ``jax.jit`` to ``value_and_grad_func`` is
 **NOT** recommended.
 Importantly, applying ``jax.pmap`` is **WRONG** and most likely will lead to
 errors.
 
 ### Registering the model loss function
 
 In order for KFAC-JAX to be able to correctly approximate the curvature matrix
 of the model it needs to know the precise loss function that you want to
-optimize. 
+optimize.
 This is done via registration with certain functions provided by the library.
-For instance, in the example above this is done via the call to 
-``kfac_jax.register_softmax_cross_entropy_loss``, which tells the optimizer that 
+For instance, in the example above this is done via the call to
+``kfac_jax.register_softmax_cross_entropy_loss``, which tells the optimizer that
 the loss is the standard softmax cross-entropy.
-If you don't do this you will get an error when you try to call the optimizer. 
+If you don't do this you will get an error when you try to call the optimizer.
 For all supported loss functions please read the [documentation].
 
-``Important:`` The optimizer assumes that the loss is averaged over examples in 
+``Important:`` The optimizer assumes that the loss is averaged over examples in
 the minibatch. It is crucial that you follow this convention.
 
 ### Other model function options
 
-Oftentimes, one will want to output some auxiliary statistics or metrics in 
+Oftentimes, one will want to output some auxiliary statistics or metrics in
 addition to the loss value.
 This can already be done in the ``value_and_grad_func``, in which case we follow
-the same conventions as JAX and expect the output to be ``(loss, aux), grads``. 
-Similarly, the loss function can take an additional function state (batch norm 
+the same conventions as JAX and expect the output to be ``(loss, aux), grads``.
+Similarly, the loss function can take an additional function state (batch norm
 layers usually have this) or an PRNG key (used in stochastic layers). All of
 these, however, need to be explicitly told to the optimizer via its arguments
 ``value_func_has_aux``, ``value_func_has_state`` and ``value_func_has_rng``.
 
 ### Verify optimizer registrations
 
-We strongly encourage the user to pay attention to the logging messages produced 
-by the automatic registration system, in order to ensure that it has correctly 
-understood your model. 
+We strongly encourage the user to pay attention to the logging messages produced
+by the automatic registration system, in order to ensure that it has correctly
+understood your model.
 For the example above this looks like this:
 
 ```python
 ==================================================
 Graph parameter registrations:
 {'mlp/~/linear_0': {'b': 'Auto[dense_with_bias_3]',
                     'w': 'Auto[dense_with_bias_3]'},
@@ -216,33 +235,33 @@
 ==================================================
 ```
 
 As can be seen from this message, the library has correctly detected all
 parameters of the model to be part of dense layers.
 
 ### Further reading
-For a high level overview of the optimizer, the different curvature 
+For a high level overview of the optimizer, the different curvature
 approximations, and the supported layers, please see the [documentation].
 
 ## Citing KFAC-JAX<a id="citing-kfac-jax"></a>
 
 To cite this repository:
 
 ```
 @software{kfac-jax2022github,
   author = {Aleksandar Botev and James Martens},
   title = {{KFAC-JAX}},
-  url = {http://github.com/deepmind/kfac-jax},
+  url = {https://github.com/google-deepmind/kfac-jax},
   version = {0.0.2},
   year = {2022},
 }
 ```
 
 In this bibtex entry, the version number is intended to be from
-[`kfac_jax/__init__.py`](https://github.com/deepmind/kfac-jax/blob/main/kfac_jax/__init__.py),
+[`kfac_jax/__init__.py`](https://github.com/google-deepmind/kfac-jax/blob/main/kfac_jax/__init__.py),
 and the year corresponds to the project's open-source release.
 
 
 [K-FAC]: https://arxiv.org/abs/1503.05671
 [JAX]: https://github.com/google/jax
-[Haiku]: https://github.com/deepmind/dm-haiku
+[Haiku]: https://github.com/google-deepmind/dm-haiku
 [documentation]: https://kfac-jax.readthedocs.io/
```

### Comparing `kfac-jax-0.0.5/kfac_jax.egg-info/SOURCES.txt` & `kfac-jax-0.0.6/kfac_jax.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -35,8 +35,12 @@
 kfac_jax/_src/tracer.py
 kfac_jax/_src/utils/__init__.py
 kfac_jax/_src/utils/accumulators.py
 kfac_jax/_src/utils/math.py
 kfac_jax/_src/utils/misc.py
 kfac_jax/_src/utils/parallel.py
 kfac_jax/_src/utils/staging.py
-kfac_jax/_src/utils/types.py
+kfac_jax/_src/utils/types.py
+tests/test_estimator.py
+tests/test_graph_matcher.py
+tests/test_patches_second_moment.py
+tests/test_tracer.py
```

### Comparing `kfac-jax-0.0.5/setup.py` & `kfac-jax-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 _VERSION = _get_version()
 
 setuptools.setup(
     name="kfac-jax",
     version=_VERSION,
-    url="https://github.com/deepmind/kfac-jax",
+    url="https://github.com/google-deepmind/kfac-jax",
     license="Apache 2.0",
     author="DeepMind",
     description=(
         "A Jax package for approximate curvature estimation and "
         "optimization using KFAC."
     ),
     long_description=open(os.path.join(_CURRENT_DIR, "README.md")).read(),
```

