# Comparing `tmp/nobrainer-1.2.0.tar.gz` & `tmp/nobrainer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobrainer-1.2.0.tar", last modified: Fri Mar 22 21:57:01 2024, max compression
+gzip compressed data, was "nobrainer-1.2.1.tar", last modified: Thu Apr  4 00:03:21 2024, max compression
```

## Comparing `nobrainer-1.2.0.tar` & `nobrainer-1.2.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.158212 nobrainer-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    23894 2024-03-22 21:56:53.000000 nobrainer-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-22 21:56:53.000000 nobrainer-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-22 21:56:53.000000 nobrainer-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-03-22 21:57:01.158212 nobrainer-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-03-22 21:56:53.000000 nobrainer-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.158212 nobrainer-1.2.0/nobrainer/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-22 21:57:01.158212 nobrainer-1.2.0/nobrainer/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/bayesian_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.150212 nobrainer-1.2.0/nobrainer/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16689 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.150212 nobrainer-1.2.0/nobrainer/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/cli/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13202 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.150212 nobrainer-1.2.0/nobrainer/distributed_learning/
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/distributed_learning/dwc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/intensity_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.150212 nobrainer-1.2.0/nobrainer/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    26369 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/Conv_v.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/InstanceNorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/groupnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/max_pool4d.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/padding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.150212 nobrainer-1.2.0/nobrainer/layers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43487 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/tests/dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/layers/tests/layers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.154212 nobrainer-1.2.0/nobrainer/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/attention_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/attention_unet_with_inception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/bayesian_meshnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/bayesian_vnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/bayesian_vnet_semi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/brainsiam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/dcgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/meshnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/progressiveae.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/progressivegan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.154212 nobrainer-1.2.0/nobrainer/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/tests/models_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/unet_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/unetr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/vnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/models/vox2vox.py
--rw-r--r--   0 runner    (1001) docker     (127)    22631 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.154212 nobrainer-1.2.0/nobrainer/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/processing/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/processing/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/processing/segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/spatial_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.158212 nobrainer-1.2.0/nobrainer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/checkpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/io_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/losses_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/prediction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/test_intensity_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/test_spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/tfrecord_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/transform_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tests/volume_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14500 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/training.py
--rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-03-22 21:56:53.000000 nobrainer-1.2.0/nobrainer/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:57:01.158212 nobrainer-1.2.0/nobrainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16981 2024-03-22 21:57:01.000000 nobrainer-1.2.0/nobrainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-03-22 21:57:01.000000 nobrainer-1.2.0/nobrainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 21:57:01.000000 nobrainer-1.2.0/nobrainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-22 21:57:01.000000 nobrainer-1.2.0/nobrainer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 21:57:00.000000 nobrainer-1.2.0/nobrainer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-22 21:57:01.000000 nobrainer-1.2.0/nobrainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 21:57:01.000000 nobrainer-1.2.0/nobrainer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-22 21:56:53.000000 nobrainer-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-22 21:57:01.158212 nobrainer-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-22 21:56:53.000000 nobrainer-1.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-03-22 21:56:53.000000 nobrainer-1.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.639351 nobrainer-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    24787 2024-04-04 00:03:13.000000 nobrainer-1.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-04 00:03:13.000000 nobrainer-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-04 00:03:13.000000 nobrainer-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-04 00:03:21.639351 nobrainer-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15203 2024-04-04 00:03:13.000000 nobrainer-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.639351 nobrainer-1.2.1/nobrainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 00:03:21.639351 nobrainer-1.2.1/nobrainer/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/bayesian_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.627350 nobrainer-1.2.1/nobrainer/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16689 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.627350 nobrainer-1.2.1/nobrainer/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/cli/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13202 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.627350 nobrainer-1.2.1/nobrainer/distributed_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/distributed_learning/dwc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/intensity_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.631350 nobrainer-1.2.1/nobrainer/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    26369 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/Conv_v.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/InstanceNorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/groupnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/max_pool4d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/padding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.631350 nobrainer-1.2.1/nobrainer/layers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43487 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/tests/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/layers/tests/layers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.635351 nobrainer-1.2.1/nobrainer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/attention_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/attention_unet_with_inception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/bayesian_meshnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/bayesian_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/bayesian_vnet_semi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/brainsiam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/dcgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/meshnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/progressiveae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/progressivegan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.635351 nobrainer-1.2.1/nobrainer/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/tests/models_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/unet_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/models/vox2vox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22631 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.635351 nobrainer-1.2.1/nobrainer/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/processing/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8216 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/processing/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/processing/segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/spatial_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.639351 nobrainer-1.2.1/nobrainer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/checkpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/io_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/losses_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/prediction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/test_intensity_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/test_spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/tfrecord_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/transform_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tests/volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14500 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10769 2024-04-04 00:03:13.000000 nobrainer-1.2.1/nobrainer/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:03:21.639351 nobrainer-1.2.1/nobrainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-04 00:03:21.000000 nobrainer-1.2.1/nobrainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-04 00:03:21.000000 nobrainer-1.2.1/nobrainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:03:21.000000 nobrainer-1.2.1/nobrainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 00:03:21.000000 nobrainer-1.2.1/nobrainer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:03:21.000000 nobrainer-1.2.1/nobrainer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-04 00:03:21.000000 nobrainer-1.2.1/nobrainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 00:03:21.000000 nobrainer-1.2.1/nobrainer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-04 00:03:13.000000 nobrainer-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-04 00:03:21.639351 nobrainer-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 00:03:13.000000 nobrainer-1.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-04-04 00:03:13.000000 nobrainer-1.2.1/versioneer.py
```

### Comparing `nobrainer-1.2.0/CHANGELOG.md` & `nobrainer-1.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# 1.2.1 (Thu Apr 04 2024)
+
+#### 🐛 Bug Fix
+
+- Fix PGAN notebook [#319](https://github.com/neuronets/nobrainer/pull/319) ([@satra](https://github.com/satra) [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]))
+- fix dependencies [#318](https://github.com/neuronets/nobrainer/pull/318) ([@satra](https://github.com/satra))
+- Update setup.cfg to add cuda option [#309](https://github.com/neuronets/nobrainer/pull/309) ([@satra](https://github.com/satra))
+- [pre-commit.ci] pre-commit autoupdate [#294](https://github.com/neuronets/nobrainer/pull/294) ([@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]) [@satra](https://github.com/satra) [@hvgazula](https://github.com/hvgazula))
+
+#### Authors: 3
+
+- [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot])
+- H Gazula ([@hvgazula](https://github.com/hvgazula))
+- Satrajit Ghosh ([@satra](https://github.com/satra))
+
+---
+
 # 1.2.0 (Fri Mar 22 2024)
 
 #### 🚀 Enhancement
 
 - Dev [#295](https://github.com/neuronets/nobrainer/pull/295) ([@hvgazula](https://github.com/hvgazula) [@pre-commit-ci[bot]](https://github.com/pre-commit-ci[bot]) [@satra](https://github.com/satra))
 - Update setup.cfg [#299](https://github.com/neuronets/nobrainer/pull/299) ([@satra](https://github.com/satra))
```

### Comparing `nobrainer-1.2.0/LICENSE` & `nobrainer-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/PKG-INFO` & `nobrainer-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobrainer
-Version: 1.2.0
+Version: 1.2.1
 Summary: A framework for developing neural network models for 3D image processing.
 Home-page: https://neuronets.github.io
 Author: Nobrainer Developers
 Author-email: jakub.kaczmarzyk@gmail.com
 License: Apache License, 2.0
 Project-URL: Source Code, https://github.com/neuronets/nobrainer
 Classifier: Development Status :: 3 - Alpha
@@ -29,18 +29,20 @@
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: fsspec
 Requires-Dist: joblib
 Requires-Dist: nibabel
 Requires-Dist: numpy
 Requires-Dist: scikit-image
-Requires-Dist: tensorflow-probability~=0.22.0
-Requires-Dist: tensorflow<=2.15.1,>=2.13
-Requires-Dist: tensorflow-addons~=0.21.0
+Requires-Dist: tensorflow-probability<0.24
+Requires-Dist: tensorflow<2.16,>=2.13
+Requires-Dist: tensorflow-addons~=0.23.0
 Requires-Dist: psutil
+Provides-Extra: and-cuda
+Requires-Dist: tensorflow[and-cuda]<2.16,>=2.13; extra == "and-cuda"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: scipy; extra == "dev"
 
 # Nobrainer
```

### Comparing `nobrainer-1.2.0/README.md` & `nobrainer-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/bayesian_utils.py` & `nobrainer-1.2.1/nobrainer/bayesian_utils.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/cli/main.py` & `nobrainer-1.2.1/nobrainer/cli/main.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/cli/tests/main_test.py` & `nobrainer-1.2.1/nobrainer/cli/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/dataset.py` & `nobrainer-1.2.1/nobrainer/dataset.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/distributed_learning/dwc.py` & `nobrainer-1.2.1/nobrainer/distributed_learning/dwc.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/intensity_transforms.py` & `nobrainer-1.2.1/nobrainer/intensity_transforms.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/io.py` & `nobrainer-1.2.1/nobrainer/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Input/output methods."""
+
 import csv
 import functools
 import multiprocessing
 import os
 
 from fsspec.implementations.local import LocalFileSystem
 import nibabel as nib
```

### Comparing `nobrainer-1.2.0/nobrainer/layers/Conv_v.py` & `nobrainer-1.2.1/nobrainer/layers/Conv_v.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/layers/InstanceNorm.py` & `nobrainer-1.2.1/nobrainer/layers/InstanceNorm.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/layers/dropout.py` & `nobrainer-1.2.1/nobrainer/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/layers/groupnorm.py` & `nobrainer-1.2.1/nobrainer/layers/groupnorm.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/layers/max_pool4d.py` & `nobrainer-1.2.1/nobrainer/layers/max_pool4d.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/layers/padding.py` & `nobrainer-1.2.1/nobrainer/layers/padding.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/layers/tests/dropout_test.py` & `nobrainer-1.2.1/nobrainer/layers/tests/dropout_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/layers/tests/layers_test.py` & `nobrainer-1.2.1/nobrainer/layers/tests/layers_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/losses.py` & `nobrainer-1.2.1/nobrainer/losses.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/metrics.py` & `nobrainer-1.2.1/nobrainer/metrics.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/__init__.py` & `nobrainer-1.2.1/nobrainer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/attention_unet.py` & `nobrainer-1.2.1/nobrainer/models/attention_unet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/attention_unet_with_inception.py` & `nobrainer-1.2.1/nobrainer/models/attention_unet_with_inception.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/autoencoder.py` & `nobrainer-1.2.1/nobrainer/models/autoencoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Model definition for Autoencoder.
 """
+
 import math
 
 from tensorflow.keras import layers, models
 
 
 def autoencoder(
     input_shape,
```

### Comparing `nobrainer-1.2.0/nobrainer/models/bayesian_meshnet.py` & `nobrainer-1.2.1/nobrainer/models/bayesian_meshnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/bayesian_vnet.py` & `nobrainer-1.2.1/nobrainer/models/bayesian_vnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/bayesian_vnet_semi.py` & `nobrainer-1.2.1/nobrainer/models/bayesian_vnet_semi.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/brainsiam.py` & `nobrainer-1.2.1/nobrainer/models/brainsiam.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/dcgan.py` & `nobrainer-1.2.1/nobrainer/models/dcgan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Model definition for DCGAN.
 """
+
 import math
 
 from tensorflow.keras import layers, models
 
 
 def dcgan(
     output_shape,
```

### Comparing `nobrainer-1.2.0/nobrainer/models/highresnet.py` & `nobrainer-1.2.1/nobrainer/models/highresnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/meshnet.py` & `nobrainer-1.2.1/nobrainer/models/meshnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/progressiveae.py` & `nobrainer-1.2.1/nobrainer/models/progressiveae.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Model definition for ProgressiveAE.
 """
+
 import tensorflow as tf
 from tensorflow.keras import layers, models
 
 
 def progressiveae(
     latent_size,
     label_size=0,
```

### Comparing `nobrainer-1.2.0/nobrainer/models/progressivegan.py` & `nobrainer-1.2.1/nobrainer/models/progressivegan.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/tests/models_test.py` & `nobrainer-1.2.1/nobrainer/models/tests/models_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/unet.py` & `nobrainer-1.2.1/nobrainer/models/unet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/unet_lstm.py` & `nobrainer-1.2.1/nobrainer/models/unet_lstm.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/unetr.py` & `nobrainer-1.2.1/nobrainer/models/unetr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """UNETR implementation in Tensorflow 2.0.
 
 Adapted from https://www.kaggle.com/code/usharengaraju/tensorflow-unetr-w-b
 """
+
 import math
 
 import tensorflow as tf
 
 
 class SingleDeconv3DBlock(tf.keras.layers.Layer):
     def __init__(self, filters):
```

### Comparing `nobrainer-1.2.0/nobrainer/models/vnet.py` & `nobrainer-1.2.1/nobrainer/models/vnet.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/models/vox2vox.py` & `nobrainer-1.2.1/nobrainer/models/vox2vox.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/prediction.py` & `nobrainer-1.2.1/nobrainer/prediction.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/processing/base.py` & `nobrainer-1.2.1/nobrainer/processing/base.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/processing/checkpoint.py` & `nobrainer-1.2.1/nobrainer/processing/checkpoint.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/processing/generation.py` & `nobrainer-1.2.1/nobrainer/processing/generation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from pathlib import Path
 
 import tensorflow as tf
 
 from .base import BaseEstimator
 from .. import losses
-from ..dataset import get_dataset
+from ..dataset import Dataset
 
 
 class ProgressiveGeneration(BaseEstimator):
     """Perform generation type operations"""
 
     state_variables = ["current_resolution_"]
 
@@ -143,34 +143,34 @@
             if resolution < self.current_resolution_:
                 continue
             # create a train dataset with features for resolution
             batch_size = info.get("batch_size")
             if batch_size % self.strategy.num_replicas_in_sync:
                 raise ValueError("batch size must be a multiple of the number of GPUs")
 
-            dataset = get_dataset(
+            dataset = Dataset.from_tfrecords(
                 file_pattern=info.get("file_pattern"),
-                batch_size=batch_size,
                 num_parallel_calls=num_parallel_calls,
                 volume_shape=(resolution, resolution, resolution),
                 n_classes=1,
-                scalar_label=True,
-                normalizer=info.get("normalizer") or normalizer,
+                scalar_labels=True,
             )
+            n_epochs = info.get("epochs") or epochs
+            dataset.batch(batch_size).normalize(
+                info.get("normalizer") or normalizer
+            ).repeat(n_epochs)
 
             with self.strategy.scope():
                 # grow the networks by one (2^x) resolution
                 if resolution > self.current_resolution_:
                     self.model_.generator.add_resolution()
                     self.model_.discriminator.add_resolution()
                 _compile()
 
-                steps_per_epoch = (info.get("epochs") or epochs) // info.get(
-                    "batch_size"
-                )
+                steps_per_epoch = n_epochs // info.get("batch_size")
 
                 # save_best_only is set to False as it is an adversarial loss
                 model_checkpoint_callback = tf.keras.callbacks.ModelCheckpoint(
                     str(model_dir),
                     save_weights_only=True,
                     save_best_only=False,
                     save_freq=save_freq,
@@ -178,24 +178,24 @@
                 )
 
             # Train at resolution
             print("Resolution : {}".format(resolution))
 
             print("Transition phase")
             self.model_.fit(
-                dataset,
+                dataset.dataset,
                 phase="transition",
                 resolution=resolution,
                 steps_per_epoch=steps_per_epoch,  # necessary for repeat dataset
                 callbacks=[model_checkpoint_callback],
             )
 
             print("Resolution phase")
             self.model_.fit(
-                dataset,
+                dataset.dataset,
                 phase="resolution",
                 resolution=resolution,
                 steps_per_epoch=steps_per_epoch,
                 callbacks=[model_checkpoint_callback],
             )
             self.current_resolution_ = resolution
             # save the final weights
```

### Comparing `nobrainer-1.2.0/nobrainer/processing/segmentation.py` & `nobrainer-1.2.1/nobrainer/processing/segmentation.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/spatial_transforms.py` & `nobrainer-1.2.1/nobrainer/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/checkpoint_test.py` & `nobrainer-1.2.1/nobrainer/tests/checkpoint_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/dataset_test.py` & `nobrainer-1.2.1/nobrainer/tests/dataset_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/io_test.py` & `nobrainer-1.2.1/nobrainer/tests/io_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/losses_test.py` & `nobrainer-1.2.1/nobrainer/tests/losses_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/metrics_test.py` & `nobrainer-1.2.1/nobrainer/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/prediction_test.py` & `nobrainer-1.2.1/nobrainer/tests/prediction_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/test_intensity_transforms.py` & `nobrainer-1.2.1/nobrainer/tests/test_intensity_transforms.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/test_spatial_transforms.py` & `nobrainer-1.2.1/nobrainer/tests/test_spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/test_utils.py` & `nobrainer-1.2.1/nobrainer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/tfrecord_test.py` & `nobrainer-1.2.1/nobrainer/tests/tfrecord_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/transform_test.py` & `nobrainer-1.2.1/nobrainer/tests/transform_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/utils.py` & `nobrainer-1.2.1/nobrainer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tests/volume_test.py` & `nobrainer-1.2.1/nobrainer/tests/volume_test.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/tfrecord.py` & `nobrainer-1.2.1/nobrainer/tfrecord.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/training.py` & `nobrainer-1.2.1/nobrainer/training.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/transform.py` & `nobrainer-1.2.1/nobrainer/transform.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/utils.py` & `nobrainer-1.2.1/nobrainer/utils.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/validation.py` & `nobrainer-1.2.1/nobrainer/validation.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer/volume.py` & `nobrainer-1.2.1/nobrainer/volume.py`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/nobrainer.egg-info/PKG-INFO` & `nobrainer-1.2.1/nobrainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobrainer
-Version: 1.2.0
+Version: 1.2.1
 Summary: A framework for developing neural network models for 3D image processing.
 Home-page: https://neuronets.github.io
 Author: Nobrainer Developers
 Author-email: jakub.kaczmarzyk@gmail.com
 License: Apache License, 2.0
 Project-URL: Source Code, https://github.com/neuronets/nobrainer
 Classifier: Development Status :: 3 - Alpha
@@ -29,18 +29,20 @@
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: fsspec
 Requires-Dist: joblib
 Requires-Dist: nibabel
 Requires-Dist: numpy
 Requires-Dist: scikit-image
-Requires-Dist: tensorflow-probability~=0.22.0
-Requires-Dist: tensorflow<=2.15.1,>=2.13
-Requires-Dist: tensorflow-addons~=0.21.0
+Requires-Dist: tensorflow-probability<0.24
+Requires-Dist: tensorflow<2.16,>=2.13
+Requires-Dist: tensorflow-addons~=0.23.0
 Requires-Dist: psutil
+Provides-Extra: and-cuda
+Requires-Dist: tensorflow[and-cuda]<2.16,>=2.13; extra == "and-cuda"
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: scipy; extra == "dev"
 
 # Nobrainer
```

### Comparing `nobrainer-1.2.0/nobrainer.egg-info/SOURCES.txt` & `nobrainer-1.2.1/nobrainer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/pyproject.toml` & `nobrainer-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nobrainer-1.2.0/setup.cfg` & `nobrainer-1.2.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -34,27 +34,29 @@
 install_requires = 
 	click
 	fsspec
 	joblib
 	nibabel
 	numpy
 	scikit-image
-	tensorflow-probability ~= 0.22.0
-	tensorflow >=2.13, <= 2.15.1
-	tensorflow-addons ~= 0.21.0
+	tensorflow-probability < 0.24
+	tensorflow >=2.13, < 2.16
+	tensorflow-addons ~= 0.23.0
 	psutil
 zip_safe = False
 packages = find:
 include_package_data = True
 
 [options.entry_points]
 console_scripts = 
 	nobrainer=nobrainer.cli.main:cli
 
 [options.extras_require]
+and-cuda = 
+	tensorflow[and-cuda] >=2.13, < 2.16
 dev = 
 	pre-commit
 	pytest
 	pytest-cov
 	scipy
 
 [tool:pytest]
```

### Comparing `nobrainer-1.2.0/setup.py` & `nobrainer-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Setup script for nobrainer.
 
 To install, run `python3 setup.py install`.
 """
+
 import os
 import sys
 
 from setuptools import setup
 
 # This is needed for versioneer to be importable when building with PEP 517.
 # See <https://github.com/warner/python-versioneer/issues/193> and links
```

### Comparing `nobrainer-1.2.0/versioneer.py` & `nobrainer-1.2.1/versioneer.py`

 * *Files identical despite different names*

