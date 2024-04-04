# Comparing `tmp/thingsvision-2.5.0.tar.gz` & `tmp/thingsvision-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thingsvision-2.5.0.tar", last modified: Thu Mar 28 18:02:14 2024, max compression
+gzip compressed data, was "thingsvision-2.5.1.tar", last modified: Thu Apr  4 09:43:35 2024, max compression
```

## Comparing `thingsvision-2.5.0.tar` & `thingsvision-2.5.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.595939 thingsvision-2.5.0/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.0/LICENSE
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15101 2024-03-28 18:02:14.595618 thingsvision-2.5.0/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14498 2024-03-28 13:21:35.000000 thingsvision-2.5.0/README.md
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-03-28 18:02:14.596051 thingsvision-2.5.0/setup.cfg
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.0/setup.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.559267 thingsvision-2.5.0/tests/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.0/tests/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.560150 thingsvision-2.5.0/tests/extractor/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.0/tests/extractor/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.562253 thingsvision-2.5.0/tests/extractor/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.0/tests/extractor/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.5.0/tests/extractor/extraction/test_custom_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2023-02-24 09:48:38.000000 thingsvision-2.5.0/tests/extractor/extraction/test_model_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2352 2024-03-28 17:54:26.000000 thingsvision-2.5.0/tests/extractor/extraction/test_pretrained_model.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2359 2023-01-17 18:07:38.000000 thingsvision-2.5.0/tests/extractor/extraction/test_torch_vs_tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2022-10-26 15:18:20.000000 thingsvision-2.5.0/tests/extractor/test_load_extractor.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.0/tests/extractor/test_transformations.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    12104 2024-03-28 14:26:15.000000 thingsvision-2.5.0/tests/helper.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.0/tests/test_features.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.0/tests/test_rest.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.563129 thingsvision-2.5.0/thingsvision/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.0/thingsvision/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-03-28 13:19:33.000000 thingsvision-2.5.0/thingsvision/_version.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.565446 thingsvision-2.5.0/thingsvision/core/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.0/thingsvision/core/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.566265 thingsvision-2.5.0/thingsvision/core/cka/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/core/cka/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/core/cka/base.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.568470 thingsvision-2.5.0/thingsvision/core/extraction/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-03-28 14:09:43.000000 thingsvision-2.5.0/thingsvision/core/extraction/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     9193 2024-03-28 13:19:33.000000 thingsvision-2.5.0/thingsvision/core/extraction/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15363 2024-03-28 14:29:36.000000 thingsvision-2.5.0/thingsvision/core/extraction/extractors.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-03-28 17:59:49.000000 thingsvision-2.5.0/thingsvision/core/extraction/helpers.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2774 2024-03-28 14:29:08.000000 thingsvision-2.5.0/thingsvision/core/extraction/tensorflow.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     6973 2024-03-28 14:28:57.000000 thingsvision-2.5.0/thingsvision/core/extraction/torch.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.569129 thingsvision-2.5.0/thingsvision/core/rsa/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/core/rsa/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.0/thingsvision/core/rsa/base.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.0/thingsvision/core/rsa/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.572680 thingsvision-2.5.0/thingsvision/custom_models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.0/thingsvision/custom_models/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.0/thingsvision/custom_models/alexnet_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.0/thingsvision/custom_models/alexnet_salobjsub.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.588743 thingsvision-2.5.0/thingsvision/custom_models/cornet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/custom_models/cornet/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/custom_models/cornet/cornet_r.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/custom_models/cornet/cornet_rt.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/custom_models/cornet/cornet_s.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/custom_models/cornet/cornet_z.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.0/thingsvision/custom_models/custom.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.589301 thingsvision-2.5.0/thingsvision/custom_models/dreamsim/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.0/thingsvision/custom_models/dreamsim/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.0/thingsvision/custom_models/dreamsim/dreamsim.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.589998 thingsvision-2.5.0/thingsvision/custom_models/harmonization/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.0/thingsvision/custom_models/harmonization/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.0/thingsvision/custom_models/harmonization/harmonization.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.0/thingsvision/custom_models/inception_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.0/thingsvision/custom_models/official_clip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.0/thingsvision/custom_models/openclip.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.0/thingsvision/custom_models/resnet50_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.0/thingsvision/custom_models/vgg16_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.0/thingsvision/custom_models/vgg16bn_ecoset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5980 2024-03-19 09:46:42.000000 thingsvision-2.5.0/thingsvision/thingsvision.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.590315 thingsvision-2.5.0/thingsvision/utils/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.0/thingsvision/utils/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.590919 thingsvision-2.5.0/thingsvision/utils/alignment/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.0/thingsvision/utils/alignment/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.0/thingsvision/utils/alignment/transforms.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.591185 thingsvision-2.5.0/thingsvision/utils/checkpointing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.0/thingsvision/utils/checkpointing/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.592629 thingsvision-2.5.0/thingsvision/utils/data/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.0/thingsvision/utils/data/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.0/thingsvision/utils/data/data_loader.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.0/thingsvision/utils/data/dataset.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.0/thingsvision/utils/data/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.592910 thingsvision-2.5.0/thingsvision/utils/imagenet/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/utils/imagenet/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.593225 thingsvision-2.5.0/thingsvision/utils/models/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.0/thingsvision/utils/models/__init__.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.594048 thingsvision-2.5.0/thingsvision/utils/models/dino/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2023-08-08 13:01:35.000000 thingsvision-2.5.0/thingsvision/utils/models/dino/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.0/thingsvision/utils/models/dino/utils.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.0/thingsvision/utils/models/dino/vision_transformer.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.595147 thingsvision-2.5.0/thingsvision/utils/storing/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.0/thingsvision/utils/storing/__init__.py
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.0/thingsvision/utils/storing/helpers.py
-drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-03-28 18:02:14.565054 thingsvision-2.5.0/thingsvision.egg-info/
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15101 2024-03-28 18:02:14.000000 thingsvision-2.5.0/thingsvision.egg-info/PKG-INFO
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2651 2024-03-28 18:02:14.000000 thingsvision-2.5.0/thingsvision.egg-info/SOURCES.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-03-28 18:02:14.000000 thingsvision-2.5.0/thingsvision.egg-info/dependency_links.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-03-28 18:02:14.000000 thingsvision-2.5.0/thingsvision.egg-info/entry_points.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-03-28 18:02:14.000000 thingsvision-2.5.0/thingsvision.egg-info/requires.txt
--rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-03-28 18:02:14.000000 thingsvision-2.5.0/thingsvision.egg-info/top_level.txt
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.849491 thingsvision-2.5.1/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1097 2021-01-22 09:49:59.000000 thingsvision-2.5.1/LICENSE
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15110 2024-04-04 09:43:35.849237 thingsvision-2.5.1/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    14507 2024-04-04 09:43:21.000000 thingsvision-2.5.1/README.md
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       38 2024-04-04 09:43:35.849608 thingsvision-2.5.1/setup.cfg
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1747 2023-04-30 10:17:04.000000 thingsvision-2.5.1/setup.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.832114 thingsvision-2.5.1/tests/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-02-02 09:19:53.000000 thingsvision-2.5.1/tests/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.832928 thingsvision-2.5.1/tests/extractor/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.1/tests/extractor/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.834575 thingsvision-2.5.1/tests/extractor/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-22 09:49:44.000000 thingsvision-2.5.1/tests/extractor/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2452 2023-01-17 18:07:55.000000 thingsvision-2.5.1/tests/extractor/extraction/test_custom_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3196 2024-04-01 11:22:39.000000 thingsvision-2.5.1/tests/extractor/extraction/test_model_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1954 2024-04-01 11:25:01.000000 thingsvision-2.5.1/tests/extractor/extraction/test_pretrained_model.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2851 2024-04-04 09:43:21.000000 thingsvision-2.5.1/tests/extractor/extraction/test_torch_vs_tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4459 2024-04-01 11:29:46.000000 thingsvision-2.5.1/tests/extractor/test_load_extractor.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1487 2023-02-22 09:56:38.000000 thingsvision-2.5.1/tests/extractor/test_transformations.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11635 2024-04-04 09:43:21.000000 thingsvision-2.5.1/tests/helper.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4447 2023-02-22 09:56:38.000000 thingsvision-2.5.1/tests/test_features.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3719 2022-08-31 09:02:04.000000 thingsvision-2.5.1/tests/test_rest.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.835364 thingsvision-2.5.1/thingsvision/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      103 2022-11-09 16:59:35.000000 thingsvision-2.5.1/thingsvision/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       22 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/_version.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.837103 thingsvision-2.5.1/thingsvision/core/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-23 10:25:59.000000 thingsvision-2.5.1/thingsvision/core/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.837563 thingsvision-2.5.1/thingsvision/core/cka/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       21 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/core/cka/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1974 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/core/cka/base.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.838969 thingsvision-2.5.1/thingsvision/core/extraction/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      176 2024-04-01 11:36:55.000000 thingsvision-2.5.1/thingsvision/core/extraction/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    10749 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15362 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/extractors.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     8452 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/helpers.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3134 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/tensorflow.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7683 2024-04-04 09:43:21.000000 thingsvision-2.5.1/thingsvision/core/extraction/torch.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.839620 thingsvision-2.5.1/thingsvision/core/rsa/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       59 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/core/rsa/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-08-29 15:24:25.000000 thingsvision-2.5.1/thingsvision/core/rsa/base.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4651 2022-08-31 09:02:04.000000 thingsvision-2.5.1/thingsvision/core/rsa/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.842341 thingsvision-2.5.1/thingsvision/custom_models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      286 2023-08-04 09:46:20.000000 thingsvision-2.5.1/thingsvision/custom_models/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      620 2023-07-11 09:50:14.000000 thingsvision-2.5.1/thingsvision/custom_models/alexnet_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      627 2023-07-11 09:50:14.000000 thingsvision-2.5.1/thingsvision/custom_models/alexnet_salobjsub.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.843797 thingsvision-2.5.1/thingsvision/custom_models/cornet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1474 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3588 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_r.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     3682 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_rt.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     4203 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_s.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_z.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      287 2023-01-18 14:03:54.000000 thingsvision-2.5.1/thingsvision/custom_models/custom.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.844294 thingsvision-2.5.1/thingsvision/custom_models/dreamsim/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2023-08-04 09:46:20.000000 thingsvision-2.5.1/thingsvision/custom_models/dreamsim/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1999 2024-03-19 09:46:42.000000 thingsvision-2.5.1/thingsvision/custom_models/dreamsim/dreamsim.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.844827 thingsvision-2.5.1/thingsvision/custom_models/harmonization/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       41 2023-03-06 11:11:47.000000 thingsvision-2.5.1/thingsvision/custom_models/harmonization/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1366 2023-03-06 11:11:52.000000 thingsvision-2.5.1/thingsvision/custom_models/harmonization/harmonization.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      629 2023-08-04 09:17:34.000000 thingsvision-2.5.1/thingsvision/custom_models/inception_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      453 2023-07-26 10:09:51.000000 thingsvision-2.5.1/thingsvision/custom_models/official_clip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1033 2023-07-11 09:50:14.000000 thingsvision-2.5.1/thingsvision/custom_models/openclip.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      623 2023-08-04 09:16:38.000000 thingsvision-2.5.1/thingsvision/custom_models/resnet50_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      614 2023-08-04 09:31:47.000000 thingsvision-2.5.1/thingsvision/custom_models/vgg16_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      621 2023-08-04 09:46:20.000000 thingsvision-2.5.1/thingsvision/custom_models/vgg16bn_ecoset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     5980 2024-03-19 09:46:42.000000 thingsvision-2.5.1/thingsvision/thingsvision.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.845133 thingsvision-2.5.1/thingsvision/utils/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2022-09-26 11:38:32.000000 thingsvision-2.5.1/thingsvision/utils/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.845577 thingsvision-2.5.1/thingsvision/utils/alignment/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       31 2024-03-28 13:19:33.000000 thingsvision-2.5.1/thingsvision/utils/alignment/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2633 2024-03-28 13:33:43.000000 thingsvision-2.5.1/thingsvision/utils/alignment/transforms.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.845856 thingsvision-2.5.1/thingsvision/utils/checkpointing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      522 2023-07-26 10:09:51.000000 thingsvision-2.5.1/thingsvision/utils/checkpointing/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.846995 thingsvision-2.5.1/thingsvision/utils/data/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2013 2022-11-15 12:25:36.000000 thingsvision-2.5.1/thingsvision/utils/data/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     1778 2022-11-15 12:25:36.000000 thingsvision-2.5.1/thingsvision/utils/data/data_loader.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7808 2022-11-15 12:25:36.000000 thingsvision-2.5.1/thingsvision/utils/data/dataset.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2969 2022-08-25 08:25:51.000000 thingsvision-2.5.1/thingsvision/utils/data/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.847223 thingsvision-2.5.1/thingsvision/utils/imagenet/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2355 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/utils/imagenet/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.847493 thingsvision-2.5.1/thingsvision/utils/models/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)        0 2023-08-09 09:09:13.000000 thingsvision-2.5.1/thingsvision/utils/models/__init__.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.848175 thingsvision-2.5.1/thingsvision/utils/models/dino/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       62 2023-08-08 13:01:35.000000 thingsvision-2.5.1/thingsvision/utils/models/dino/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2396 2023-08-08 13:01:35.000000 thingsvision-2.5.1/thingsvision/utils/models/dino/utils.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    11168 2023-08-08 13:01:35.000000 thingsvision-2.5.1/thingsvision/utils/models/dino/vision_transformer.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.848879 thingsvision-2.5.1/thingsvision/utils/storing/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       67 2022-08-22 09:49:44.000000 thingsvision-2.5.1/thingsvision/utils/storing/__init__.py
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     7325 2023-02-22 09:56:38.000000 thingsvision-2.5.1/thingsvision/utils/storing/helpers.py
+drwxr-xr-x   0 lmuttenthaler   (501) staff       (20)        0 2024-04-04 09:43:35.836865 thingsvision-2.5.1/thingsvision.egg-info/
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)    15110 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/PKG-INFO
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)     2651 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/SOURCES.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       39 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/dependency_links.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       64 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/entry_points.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)      332 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/requires.txt
+-rw-r--r--   0 lmuttenthaler   (501) staff       (20)       19 2024-04-04 09:43:35.000000 thingsvision-2.5.1/thingsvision.egg-info/top_level.txt
```

### Comparing `thingsvision-2.5.0/LICENSE` & `thingsvision-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/PKG-INFO` & `thingsvision-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.0
+Version: 2.5.1
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -132,15 +132,15 @@
 
 If you want to extract features for [DreamSim](https://dreamsim-nights.github.io/) from the [DreamSim repo](https://github.com/ssundaram21/dreamsim), you have to additionally run the following `pip` command in your `thingsvision` environment,
 
 ```bash
 $ pip install dreamsim==0.1.2
 ```
 
-See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for which `DreamSim` models are available in `thingsvision`.
+See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for which `DreamSim` models are available in `thingsvision`.
 
 #### Google Colab.
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
@@ -188,15 +188,15 @@
   model_parameters=model_parameters,
 )
 ```
 
 As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
 
 ```python
-root='path/to/root/image/directory' # (e.g., './images/)
+root='path/to/your/image/directory' # (e.g., './images/)
 batch_size = 32
 
 dataset = ImageDataset(
     root=root,
     out_path='path/to/features',
     backend=extractor.get_backend(), # backend framework of model
     transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set the input dimensionality to whichever values are required for your pretrained model
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.0 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.5.1 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -81,15 +81,15 @@
 be working smoothly on Ubuntu only but not on macOS), ```bash $ pip install
 git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
 attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
 (https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
 github.com/ssundaram21/dreamsim), you have to additionally run the following
 `pip` command in your `thingsvision` environment, ```bash $ pip install
 dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
-AvailableModels.html) for which `DreamSim` models are available in
+AvailableModels.html#dreamsim) for which `DreamSim` models are available in
 `thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
 play around with `thingsvision` by uploading your image data to Google Drive
 (via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
 master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
 colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
 notebooks/tensorflow.ipynb).
@@ -118,15 +118,15 @@
 import ImageDataset, DataLoader model_name = 'clip' source = 'custom' device =
 'cuda' if torch.cuda.is_available() else 'cpu' model_parameters = { 'variant':
 'ViT-L/14' } extractor = get_extractor( model_name=model_name, source=source,
 device=device, pretrained=True, model_parameters=model_parameters, ) ``` As a
 next step, create both dataset and dataloader for your images. We assume that
 all of your images are in a single `root` directory which can contain
 subfolders (e.g., for individual classes). Therefore, we leverage the
-`ImageDataset` class. ```python root='path/to/root/image/directory' # (e.g.,
+`ImageDataset` class. ```python root='path/to/your/image/directory' # (e.g.,
 './images/) batch_size = 32 dataset = ImageDataset( root=root, out_path='path/
 to/features', backend=extractor.get_backend(), # backend framework of model
 transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set
 the input dimensionality to whichever values are required for your pretrained
 model ) batches = DataLoader( dataset=dataset, batch_size=batch_size,
 backend=extractor.get_backend() # backend framework of model ) ``` Now all that
 is left is to extract the image features and store them on disk! Here we're
```

### Comparing `thingsvision-2.5.0/README.md` & `thingsvision-2.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 If you want to extract features for [DreamSim](https://dreamsim-nights.github.io/) from the [DreamSim repo](https://github.com/ssundaram21/dreamsim), you have to additionally run the following `pip` command in your `thingsvision` environment,
 
 ```bash
 $ pip install dreamsim==0.1.2
 ```
 
-See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for which `DreamSim` models are available in `thingsvision`.
+See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for which `DreamSim` models are available in `thingsvision`.
 
 #### Google Colab.
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
@@ -171,15 +171,15 @@
   model_parameters=model_parameters,
 )
 ```
 
 As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
 
 ```python
-root='path/to/root/image/directory' # (e.g., './images/)
+root='path/to/your/image/directory' # (e.g., './images/)
 batch_size = 32
 
 dataset = ImageDataset(
     root=root,
     out_path='path/to/features',
     backend=extractor.get_backend(), # backend framework of model
     transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set the input dimensionality to whichever values are required for your pretrained model
```

#### html2text {}

```diff
@@ -73,15 +73,15 @@
 be working smoothly on Ubuntu only but not on macOS), ```bash $ pip install
 git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
 attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
 (https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
 github.com/ssundaram21/dreamsim), you have to additionally run the following
 `pip` command in your `thingsvision` environment, ```bash $ pip install
 dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
-AvailableModels.html) for which `DreamSim` models are available in
+AvailableModels.html#dreamsim) for which `DreamSim` models are available in
 `thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
 play around with `thingsvision` by uploading your image data to Google Drive
 (via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
 master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
 colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
 notebooks/tensorflow.ipynb).
@@ -110,15 +110,15 @@
 import ImageDataset, DataLoader model_name = 'clip' source = 'custom' device =
 'cuda' if torch.cuda.is_available() else 'cpu' model_parameters = { 'variant':
 'ViT-L/14' } extractor = get_extractor( model_name=model_name, source=source,
 device=device, pretrained=True, model_parameters=model_parameters, ) ``` As a
 next step, create both dataset and dataloader for your images. We assume that
 all of your images are in a single `root` directory which can contain
 subfolders (e.g., for individual classes). Therefore, we leverage the
-`ImageDataset` class. ```python root='path/to/root/image/directory' # (e.g.,
+`ImageDataset` class. ```python root='path/to/your/image/directory' # (e.g.,
 './images/) batch_size = 32 dataset = ImageDataset( root=root, out_path='path/
 to/features', backend=extractor.get_backend(), # backend framework of model
 transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set
 the input dimensionality to whichever values are required for your pretrained
 model ) batches = DataLoader( dataset=dataset, batch_size=batch_size,
 backend=extractor.get_backend() # backend framework of model ) ``` Now all that
 is left is to extract the image features and store them on disk! Here we're
```

### Comparing `thingsvision-2.5.0/setup.py` & `thingsvision-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/tests/extractor/extraction/test_custom_model.py` & `thingsvision-2.5.1/tests/extractor/extraction/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/tests/extractor/extraction/test_model_extractor.py` & `thingsvision-2.5.1/tests/extractor/extraction/test_model_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/tests/extractor/extraction/test_pretrained_model.py` & `thingsvision-2.5.1/tests/extractor/extraction/test_pretrained_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,15 @@
     def test_extraction_pretrained_models(self):
         """Tests basic feature extraction pipeline."""
         for (
             extractor,
             dataset,
             batches,
             module_names,
-            model_name,
-            clip
+            model_name
         ) in helper.iterate_through_all_model_combinations():
             self.assertEqual(len(dataset), len(batches) * helper.BATCH_SIZE)
             num_objects = len(dataset)
 
             for module_name in module_names:
                 features = extractor.extract_features(
                     batches=batches,
@@ -37,24 +36,14 @@
 
                 if module_name.startswith("classifier"):
                     self.assertEqual(
                         features.shape[1],
                         extractor.model.classifier[int(module_name[-1])].out_features,
                     )
 
-                if not clip:
-                    features = extractor.extract_features(
-                        batches=batches,
-                        module_name=module_name,
-                        flatten_acts=False,
-                    )
-
-                    self.assertTrue(isinstance(features, Array))
-                    self.assertEqual(features.shape[0], num_objects)
-
                 if extractor.get_backend() == "pt":
                     if model_name in helper.ALIGNED_MODELS:
                         if module_name == helper.ALIGNED_MODELS[model_name]:
                             print(f"\nAligning representations extracted from layer: {module_name} of model: {model_name}")
                             aligned_features = extractor.align(features=features, module_name=module_name)
                             print(f"Successfully aligned the representation space of model: {model_name}\n")
                             self.assertTrue(isinstance(aligned_features, Array))
```

### Comparing `thingsvision-2.5.0/tests/extractor/test_load_extractor.py` & `thingsvision-2.5.1/tests/extractor/test_load_extractor.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/tests/extractor/test_transformations.py` & `thingsvision-2.5.1/tests/extractor/test_transformations.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/tests/helper.py` & `thingsvision-2.5.1/tests/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         "modules": ["decoder.flatten"],
         "pretrained": True,
         "source": "custom",
     },
     "cornet_rt": {
         "model_name": "cornet_rt",
         "modules": ["decoder.flatten"],
-        "pretrained": False,
+        "pretrained": True,
         "source": "custom",
     },
     "cornet_s": {
         "model_name": "cornet_s",
         "modules": ["decoder.flatten"],
         "pretrained": False,
         "source": "custom",
@@ -66,22 +66,14 @@
     # Custom models
     "VGG16_ecoset": {
         "model_name": "VGG16_ecoset",
         "modules": ["classifier.3"],
         "pretrained": True,
         "source": "custom",
     },
-    "clip_vitl14": {
-        "model_name": "clip",
-        "modules": ["visual"],
-        "pretrained": True,
-        "source": "custom",
-        "clip": True,
-        "kwargs": {"variant": "ViT-L/14"},
-    },
     "clip_rn50": {
         "model_name": "clip",
         "modules": ["visual"],
         "pretrained": True,
         "source": "custom",
         "clip": True,
         "kwargs": {"variant": "RN50"},
@@ -231,21 +223,14 @@
     "DreamSim_mlp_dino_vitb16": {
         "model_name": "DreamSim",
         "modules": ["model.mlp"],
         "pretrained": True,
         "source": "custom",
         "kwargs": {"variant": "dino_vitb16"},
     },
-    "DreamSim_mlp_ensemble": {
-        "model_name": "DreamSim",
-        "modules": ["model.mlp"],
-        "pretrained": True,
-        "source": "custom",
-        "kwargs": {"variant": "ensemble"},
-    },
 }
 
 ALIGNED_MODELS = {
     "alexnet": "classifier.4",
     "vgg16": "classifier.3",
     "resnet18": "avgpool",
     "resnet50": "avgpool",
@@ -346,16 +331,15 @@
         source = model_config["source"]
         kwargs = model_config.get("kwargs", {})
         extractor, dataset, batches = create_extractor_and_dataloader(
             model_name, pretrained, source, kwargs
         )
 
         modules = model_config["modules"]
-        clip = model_config.get("clip", False)
-        yield extractor, dataset, batches, modules, model_name, clip
+        yield extractor, dataset, batches, modules, model_name
 
 
 def create_extractor_and_dataloader(
     model_name: str, pretrained: bool, source: str, kwargs: dict = {}
 ):
     """Iterate through models and create model, dataset and data loader."""
     extractor = get_extractor(
```

### Comparing `thingsvision-2.5.0/tests/test_features.py` & `thingsvision-2.5.1/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/tests/test_rest.py` & `thingsvision-2.5.1/tests/test_rest.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/core/cka/base.py` & `thingsvision-2.5.1/thingsvision/core/cka/base.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/core/extraction/base.py` & `thingsvision-2.5.1/thingsvision/core/extraction/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import abc
 import os
 import re
 import warnings
 from typing import Callable, Iterator, List, Optional, Union
 
 import numpy as np
+import torch
 from torchtyping import TensorType
 from tqdm.auto import tqdm
 
-import torch
-
 Array = np.ndarray
 
 
 class BaseExtractor(metaclass=abc.ABCMeta):
     def __init__(self, device, preprocess) -> None:
         self.device = device
         self._check_device()
@@ -68,14 +67,50 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def load_model(self) -> None:
         raise NotImplementedError
 
     @abc.abstractmethod
+    def extract_batch(
+        self,
+        batch: Union[TensorType["b", "c", "h", "w"], Array],
+        module_name: str,
+        flatten_acts: bool,
+        output_type: str,
+    ) -> Union[
+        Union[
+            TensorType["b", "num_maps", "h_prime", "w_prime"],
+            TensorType["b", "t", "d"],
+            TensorType["b", "p"],
+            TensorType["b", "d"],
+        ],
+        Array,
+    ]:
+        """Extract hidden unit activations (at specified layer) for every image in a mini-batch.
+
+        Parameters
+        ----------
+        batch : np.ndarray or torch.Tensor
+            mini-batch of three-dimensional image tensors.
+        module_name : str
+            Name of the module for which features should be extraced.
+        flatten_acts : bool
+            Whether the activation of a tensor should be flattened to a vector.
+        output_type : str {"ndarray", "tensor"}
+            Whether to return output features as torch.Tensor or np.ndarray.
+            Available options are "ndarray" or "tensor".
+        Returns
+        -------
+        output : np.ndarray or torch.Tensor
+            Returns the feature matrix (e.g., $X \in \mathbb{R}^{B \times d}$ if penultimate or logits layer or flatten_acts = True).
+        """
+        raise NotImplementedError
+
+    @abc.abstractmethod
     def _extract_batch(
         self,
         batch: Union[TensorType["b", "c", "h", "w"], Array],
         module_name: str,
         flatten_acts: bool,
     ) -> Union[
         Union[
@@ -87,20 +122,31 @@
         Array,
     ]:
         raise NotImplementedError
 
     def get_output_types(self) -> List[str]:
         return ["ndarray", "tensor"]
 
+    def _module_and_output_check(self, module_name: str, output_type: str) -> None:
+        """Checks whether the provided module name and output type are valid."""
+        valid_names = self.get_module_names()
+        if not module_name in valid_names:
+            raise ValueError(
+                f"\n{module_name} is not a valid module name. Please choose a name from the following set of modules: {valid_names}\n"
+            )
+        assert (
+            output_type in self.get_output_types()
+        ), f"\nData type of output feature matrix must be set to one of the following available data types: {self.get_output_types()}\n"
+
     def extract_features(
         self,
         batches: Iterator[Union[TensorType["b", "c", "h", "w"], Array]],
         module_name: str,
         flatten_acts: bool,
-        output_type: str = "ndarray",
+        output_type: Optional[str] = "ndarray",
         output_dir: Optional[str] = None,
         step_size: Optional[int] = None,
     ) -> Union[
         Union[
             TensorType["n", "num_maps", "h_prime", "w_prime"],
             TensorType["n", "t", "d"],
             TensorType["n", "p"],
@@ -142,22 +188,15 @@
             Only used if output_dir is defined.
 
         Returns
         -------
         output : np.ndarray or torch.Tensor
             Returns the feature matrix (e.g., $X \in \mathbb{R}^{n \times d}$ if penultimate or logits layer or flatten_acts = True).
         """
-        valid_names = self.get_module_names()
-        if not module_name in valid_names:
-            raise ValueError(
-                f"\n{module_name} is not a valid module name. Please choose a name from the following set of modules: {valid_names}\n"
-            )
-        assert (
-            output_type in self.get_output_types()
-        ), f"\nData type of output feature matrix must be set to one of the following available data types: {self.get_output_types()}\n"
+        self._module_and_output_check(module_name, output_type)
         if output_dir:
             os.makedirs(output_dir, exist_ok=True)
 
             if not step_size:
                 # if step size is not given, assume that features to every image consume 3MB of memory and that the user has at least 8GB of free RAM
                 step_size = 8000 // (len(next(iter(batches))) * 3) + 1
```

### Comparing `thingsvision-2.5.0/thingsvision/core/extraction/extractors.py` & `thingsvision-2.5.1/thingsvision/core/extraction/extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
-import timm
-import torchvision
-
 import tensorflow as tf
 import tensorflow.keras.applications as tensorflow_models
+import timm
 import torch
+import torchvision
 
 try:
     from torch.hub import load_state_dict_from_url
 except ImportError:
     from torch.utils.model_zoo import load_url as load_state_dict_from_url
 
 from thingsvision.utils.checkpointing import get_torch_home
```

### Comparing `thingsvision-2.5.0/thingsvision/core/extraction/helpers.py` & `thingsvision-2.5.1/thingsvision/core/extraction/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import warnings
 from typing import Any, Callable, Dict, Union
 
 import numpy as np
-from torchtyping import TensorType
-
 import torch
+from torchtyping import TensorType
 
 from .extractors import (
     KerasExtractor,
     SSLExtractor,
     TimmExtractor,
     TorchvisionExtractor,
 )
@@ -63,15 +62,15 @@
 
     Extractor = PyTorchExtractor if backend == "pt" else TensorFlowExtractor
 
     class CustomExtractor(Extractor):
         def __init__(self, *args, **kwargs) -> None:
             super().__init__(*args, **kwargs)
 
-    #TODO(lukasmut): this should probably be defined in the custom model itself
+    # TODO(lukasmut): this should probably be defined in the custom model itself
     if model_name.lower().startswith("clip"):
 
         def show_model(self):
             for l, (n, p) in enumerate(self.model.named_modules()):
                 if l > 1:
                     if n.startswith("visual"):
                         print(n)
```

### Comparing `thingsvision-2.5.0/thingsvision/core/extraction/tensorflow.py` & `thingsvision-2.5.1/thingsvision/core/extraction/tensorflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,26 +32,40 @@
         self.model = model
 
         if not self.model:
             self.load_model()
         self.prepare_inference()
 
     def _extract_batch(
-        self, batch: Array, module_name: str, flatten_acts: bool
+        self,
+        batch: Array,
+        module_name: str,
+        flatten_acts: bool,
     ) -> Array:
         layer_out = [self.model.get_layer(module_name).output]
         activation_model = keras.models.Model(
             inputs=self.model.input,
             outputs=layer_out,
         )
         activations = activation_model.predict(batch)
         if flatten_acts:
             activations = activations.reshape(activations.shape[0], -1)
         return activations
 
+    def extract_batch(
+        self,
+        batch: Array,
+        module_name: str,
+        flatten_acts: bool,
+        output_type: str = "ndarray",
+    ) -> Array:
+        self._module_and_output_check(module_name, output_type)
+        activations = self._extract_batch(batch, module_name, flatten_acts)
+        return activations
+
     def show_model(self) -> str:
         return self.model.summary()
 
     def load_model_from_source(self) -> None:
         raise NotImplementedError
 
     def load_model(self) -> None:
```

### Comparing `thingsvision-2.5.0/thingsvision/core/extraction/torch.py` & `thingsvision-2.5.1/thingsvision/core/extraction/torch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Callable, Dict, Iterator, List, Optional, Union
 
 import numpy as np
-from thingsvision.utils.alignment import gLocal
+import torch
 from torchtyping import TensorType
 from torchvision import transforms as T
 
-import torch
+from thingsvision.utils.alignment import gLocal
 
 from .base import BaseExtractor
 
 Array = np.ndarray
 Tensor = torch.Tensor
 
 
@@ -37,38 +37,14 @@
             if "extract_cls_token" in self.model_parameters:
                 self.extract_cls_token = self.model_parameters["extract_cls_token"]
 
         if not self.model:
             self.load_model()
         self.prepare_inference()
 
-    def extract_features(
-        self,
-        batches: Iterator,
-        module_name: str,
-        flatten_acts: bool,
-        output_type: str = "ndarray",
-        output_dir: Optional[str] = None,
-        step_size: Optional[int] = None,
-    ):
-        self.model = self.model.to(self.device)
-        self.activations = {}
-        self.register_hook(module_name=module_name)
-        features = super().extract_features(
-            batches=batches,
-            module_name=module_name,
-            flatten_acts=flatten_acts,
-            output_type=output_type,
-            output_dir=output_dir,
-            step_size=step_size,
-        )
-        if self.hook_handle:
-            self._unregister_hook()
-        return features
-
     def get_activation(self, name: str) -> Callable:
         """Store copy of activations for a specific layer of the model."""
 
         def hook(model, input, output) -> None:
             # store copy of tensor rather than tensor itself
             if isinstance(output, tuple):
                 act = output[0]
@@ -87,14 +63,34 @@
             if n == module_name:
                 self.hook_handle = m.register_forward_hook(self.get_activation(n))
                 break
 
     def _unregister_hook(self) -> None:
         self.hook_handle.remove()
 
+    def extract_batch(
+        self,
+        batch: TensorType["b", "c", "h", "w"],
+        module_name: str,
+        flatten_acts: bool,
+        output_type: str = "tensor",
+    ) -> Union[
+        TensorType["b", "num_maps", "h_prime", "w_prime"],
+        TensorType["b", "t", "d"],
+        TensorType["b", "p"],
+        TensorType["b", "d"],
+    ]:
+        self._module_and_output_check(module_name, output_type)
+        self.register_hook(module_name=module_name)
+        act = self._extract_batch(batch, module_name, flatten_acts)
+        if output_type == "ndarray":
+            act = self._to_numpy(act)
+        self._unregister_hook()
+        return act
+
     @torch.no_grad()
     def _extract_batch(
         self,
         batch: TensorType["b", "c", "h", "w"],
         module_name: str,
         flatten_acts: bool,
     ) -> Union[
@@ -104,26 +100,51 @@
         TensorType["b", "d"],
     ]:
         # move current batch to torch device
         batch = batch.to(self.device)
         _ = self.forward(batch)
         act = self.activations[module_name]
         if hasattr(self, "extract_cls_token"):
-            # we are only interested in the representations of the first token, i.e., [cls] token
-            act = act[:, 0, :].clone()
+            if self.extract_cls_token:
+                # we are only interested in the representations of the first token, i.e., [cls] token
+                act = act[:, 0, :].clone()
         if flatten_acts:
             if self.model_name.lower().startswith("clip"):
                 act = self.flatten_acts(act, batch, module_name)
             else:
                 act = self.flatten_acts(act)
         if act.is_cuda or act.get_device() >= 0:
             torch.cuda.empty_cache()
             act = act.cpu()
         return act
 
+    def extract_features(
+        self,
+        batches: Iterator,
+        module_name: str,
+        flatten_acts: bool,
+        output_type: str = "ndarray",
+        output_dir: Optional[str] = None,
+        step_size: Optional[int] = None,
+    ):
+        self.model = self.model.to(self.device)
+        self.activations = {}
+        self.register_hook(module_name=module_name)
+        features = super().extract_features(
+            batches=batches,
+            module_name=module_name,
+            flatten_acts=flatten_acts,
+            output_type=output_type,
+            output_dir=output_dir,
+            step_size=step_size,
+        )
+        if self.hook_handle:
+            self._unregister_hook()
+        return features
+
     def forward(
         self, batch: TensorType["b", "c", "h", "w"]
     ) -> TensorType["b", "num_cls"]:
         """Default forward pass."""
         return self.model(batch)
 
     @staticmethod
```

### Comparing `thingsvision-2.5.0/thingsvision/core/rsa/helpers.py` & `thingsvision-2.5.1/thingsvision/core/rsa/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/alexnet_ecoset.py` & `thingsvision-2.5.1/thingsvision/custom_models/alexnet_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/alexnet_salobjsub.py` & `thingsvision-2.5.1/thingsvision/custom_models/alexnet_salobjsub.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/cornet/__init__.py` & `thingsvision-2.5.1/thingsvision/custom_models/cornet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/cornet/cornet_r.py` & `thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_r.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/cornet/cornet_rt.py` & `thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_rt.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/cornet/cornet_s.py` & `thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_s.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/cornet/cornet_z.py` & `thingsvision-2.5.1/thingsvision/custom_models/cornet/cornet_z.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/dreamsim/dreamsim.py` & `thingsvision-2.5.1/thingsvision/custom_models/dreamsim/dreamsim.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/harmonization/harmonization.py` & `thingsvision-2.5.1/thingsvision/custom_models/harmonization/harmonization.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/inception_ecoset.py` & `thingsvision-2.5.1/thingsvision/custom_models/inception_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/openclip.py` & `thingsvision-2.5.1/thingsvision/custom_models/openclip.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/resnet50_ecoset.py` & `thingsvision-2.5.1/thingsvision/custom_models/resnet50_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/vgg16_ecoset.py` & `thingsvision-2.5.1/thingsvision/custom_models/vgg16_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/custom_models/vgg16bn_ecoset.py` & `thingsvision-2.5.1/thingsvision/custom_models/vgg16bn_ecoset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/thingsvision.py` & `thingsvision-2.5.1/thingsvision/thingsvision.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/alignment/transforms.py` & `thingsvision-2.5.1/thingsvision/utils/alignment/transforms.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/checkpointing/__init__.py` & `thingsvision-2.5.1/thingsvision/utils/checkpointing/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/data/__init__.py` & `thingsvision-2.5.1/thingsvision/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/data/data_loader.py` & `thingsvision-2.5.1/thingsvision/utils/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/data/dataset.py` & `thingsvision-2.5.1/thingsvision/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/data/helpers.py` & `thingsvision-2.5.1/thingsvision/utils/data/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/imagenet/__init__.py` & `thingsvision-2.5.1/thingsvision/utils/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/models/dino/utils.py` & `thingsvision-2.5.1/thingsvision/utils/models/dino/utils.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/models/dino/vision_transformer.py` & `thingsvision-2.5.1/thingsvision/utils/models/dino/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision/utils/storing/helpers.py` & `thingsvision-2.5.1/thingsvision/utils/storing/helpers.py`

 * *Files identical despite different names*

### Comparing `thingsvision-2.5.0/thingsvision.egg-info/PKG-INFO` & `thingsvision-2.5.1/thingsvision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thingsvision
-Version: 2.5.0
+Version: 2.5.1
 Summary: Extracting image features from state-of-the-art neural networks for Computer Vision made easy
 Home-page: https://github.com/ViCCo-Group/thingsvision
 Author: Lukas Muttenthaler
 Author-email: muttenthaler@cbs.mpg.de
 License: MIT License
 Keywords: feature extraction
 Classifier: Programming Language :: Python :: 3.8
@@ -132,15 +132,15 @@
 
 If you want to extract features for [DreamSim](https://dreamsim-nights.github.io/) from the [DreamSim repo](https://github.com/ssundaram21/dreamsim), you have to additionally run the following `pip` command in your `thingsvision` environment,
 
 ```bash
 $ pip install dreamsim==0.1.2
 ```
 
-See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html) for which `DreamSim` models are available in `thingsvision`.
+See the [docs](https://vicco-group.github.io/thingsvision/AvailableModels.html#dreamsim) for which `DreamSim` models are available in `thingsvision`.
 
 #### Google Colab.
 Alternatively, you can use Google Colab to play around with `thingsvision` by uploading your image data to Google Drive (via directory mounting).
 You can find the jupyter notebook using `PyTorch` [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/notebooks/tensorflow.ipynb).
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
@@ -188,15 +188,15 @@
   model_parameters=model_parameters,
 )
 ```
 
 As a next step, create both dataset and dataloader for your images. We assume that all of your images are in a single `root` directory which can contain subfolders (e.g., for individual classes). Therefore, we leverage the `ImageDataset` class. 
 
 ```python
-root='path/to/root/image/directory' # (e.g., './images/)
+root='path/to/your/image/directory' # (e.g., './images/)
 batch_size = 32
 
 dataset = ImageDataset(
     root=root,
     out_path='path/to/features',
     backend=extractor.get_backend(), # backend framework of model
     transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set the input dimensionality to whichever values are required for your pretrained model
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thingsvision Version: 2.5.0 Summary: Extracting
+Metadata-Version: 2.1 Name: thingsvision Version: 2.5.1 Summary: Extracting
 image features from state-of-the-art neural networks for Computer Vision made
 easy Home-page: https://github.com/ViCCo-Group/thingsvision Author: Lukas
 Muttenthaler Author-email: muttenthaler@cbs.mpg.de License: MIT License
 Keywords: feature extraction Classifier: Programming Language :: Python :: 3.8
 Classifier: Natural Language :: English Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
@@ -81,15 +81,15 @@
 be working smoothly on Ubuntu only but not on macOS), ```bash $ pip install
 git+https://github.com/serre-lab/Harmonization.git $ pip install keras-cv-
 attention-models>=1.3.5 ``` If you want to extract features for [DreamSim]
 (https://dreamsim-nights.github.io/) from the [DreamSim repo](https://
 github.com/ssundaram21/dreamsim), you have to additionally run the following
 `pip` command in your `thingsvision` environment, ```bash $ pip install
 dreamsim==0.1.2 ``` See the [docs](https://vicco-group.github.io/thingsvision/
-AvailableModels.html) for which `DreamSim` models are available in
+AvailableModels.html#dreamsim) for which `DreamSim` models are available in
 `thingsvision`. #### Google Colab. Alternatively, you can use Google Colab to
 play around with `thingsvision` by uploading your image data to Google Drive
 (via directory mounting). You can find the jupyter notebook using `PyTorch`
 [here](https://colab.research.google.com/github/ViCCo-Group/thingsvision/blob/
 master/notebooks/pytorch.ipynb) and the `TensorFlow` example [here](https://
 colab.research.google.com/github/ViCCo-Group/thingsvision/blob/master/
 notebooks/tensorflow.ipynb).
@@ -118,15 +118,15 @@
 import ImageDataset, DataLoader model_name = 'clip' source = 'custom' device =
 'cuda' if torch.cuda.is_available() else 'cpu' model_parameters = { 'variant':
 'ViT-L/14' } extractor = get_extractor( model_name=model_name, source=source,
 device=device, pretrained=True, model_parameters=model_parameters, ) ``` As a
 next step, create both dataset and dataloader for your images. We assume that
 all of your images are in a single `root` directory which can contain
 subfolders (e.g., for individual classes). Therefore, we leverage the
-`ImageDataset` class. ```python root='path/to/root/image/directory' # (e.g.,
+`ImageDataset` class. ```python root='path/to/your/image/directory' # (e.g.,
 './images/) batch_size = 32 dataset = ImageDataset( root=root, out_path='path/
 to/features', backend=extractor.get_backend(), # backend framework of model
 transforms=extractor.get_transformations(resize_dim=256, crop_dim=224) # set
 the input dimensionality to whichever values are required for your pretrained
 model ) batches = DataLoader( dataset=dataset, batch_size=batch_size,
 backend=extractor.get_backend() # backend framework of model ) ``` Now all that
 is left is to extract the image features and store them on disk! Here we're
```

### Comparing `thingsvision-2.5.0/thingsvision.egg-info/SOURCES.txt` & `thingsvision-2.5.1/thingsvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

