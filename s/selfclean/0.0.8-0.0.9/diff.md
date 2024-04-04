# Comparing `tmp/selfclean-0.0.8.tar.gz` & `tmp/selfclean-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfclean-0.0.8.tar", last modified: Thu Mar 21 11:45:20 2024, max compression
+gzip compressed data, was "selfclean-0.0.9.tar", last modified: Fri Mar 22 08:40:18 2024, max compression
```

## Comparing `selfclean-0.0.8.tar` & `selfclean-0.0.9.tar`

### file list

```diff
@@ -1,172 +1,173 @@
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.292811 selfclean-0.0.8/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1487 2024-03-21 11:45:20.292811 selfclean-0.0.8/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      993 2024-03-21 10:44:06.000000 selfclean-0.0.8/README.md
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      580 2024-03-19 13:10:56.000000 selfclean-0.0.8/pyproject.toml
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/selfclean.egg-info/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1487 2024-03-21 11:45:20.000000 selfclean-0.0.8/selfclean.egg-info/PKG-INFO
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     6107 2024-03-21 11:45:20.000000 selfclean-0.0.8/selfclean.egg-info/SOURCES.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-03-21 11:45:20.000000 selfclean-0.0.8/selfclean.egg-info/dependency_links.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      268 2024-03-21 11:45:20.000000 selfclean-0.0.8/selfclean.egg-info/requires.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       10 2024-03-21 11:45:20.000000 selfclean-0.0.8/selfclean.egg-info/top_level.txt
--rw-rw-r--   0 fabian    (1000) fabian    (1000)       38 2024-03-21 11:45:20.292811 selfclean-0.0.8/setup.cfg
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1578 2024-03-21 11:43:21.000000 selfclean-0.0.8/setup.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      221 2024-03-19 13:12:36.000000 selfclean-0.0.8/src/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/cleaner/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/cleaner/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     6744 2024-03-21 10:45:08.000000 selfclean-0.0.8/src/cleaner/auto_cleaning_mixin.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      498 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/cleaner/base_cleaner.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/cleaner/irrelevants/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/cleaner/irrelevants/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      222 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/cleaner/irrelevants/base_irrelevant_mixin.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1128 2024-03-19 12:43:27.000000 selfclean-0.0.8/src/cleaner/irrelevants/lad_mixin.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1394 2024-03-19 12:43:27.000000 selfclean-0.0.8/src/cleaner/irrelevants/quantile_irrelevant_mixin.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/cleaner/label_errors/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/cleaner/label_errors/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      243 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/cleaner/label_errors/base_label_error_mixin.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2760 2024-03-19 12:43:27.000000 selfclean-0.0.8/src/cleaner/label_errors/intra_extra_distance_mixin.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/cleaner/near_duplicates/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/cleaner/near_duplicates/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      229 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/cleaner/near_duplicates/base_near_duplicate_mixin.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2893 2024-03-21 10:08:10.000000 selfclean-0.0.8/src/cleaner/near_duplicates/embedding_distance_mixin.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    11131 2024-03-21 11:42:38.000000 selfclean-0.0.8/src/cleaner/selfclean.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     7523 2024-03-21 11:43:29.000000 selfclean-0.0.8/src/cleaner/selfclean_cleaner.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/distances/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/distances/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      863 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/distances/projective_distance.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/scoring/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/scoring/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    11629 2024-03-21 10:07:58.000000 selfclean-0.0.8/src/scoring/lad_scoring.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/ssl_library/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.280810 selfclean-0.0.8/src/ssl_library/src/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      217 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/augmentations/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/augmentations/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1131 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/augmentations/augmentations.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3069 2024-03-21 09:52:32.000000 selfclean-0.0.8/src/ssl_library/src/augmentations/dino.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     4484 2024-03-21 09:51:42.000000 selfclean-0.0.8/src/ssl_library/src/augmentations/ibot.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2407 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/augmentations/simclr.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/dataset_wrappers/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/dataset_wrappers/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      793 2024-03-21 09:07:23.000000 selfclean-0.0.8/src/ssl_library/src/dataset_wrappers/base_wrapper.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1220 2024-03-21 09:07:48.000000 selfclean-0.0.8/src/ssl_library/src/dataset_wrappers/colorme_wrapper.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     4739 2024-03-19 12:46:15.000000 selfclean-0.0.8/src/ssl_library/src/dataset_wrappers/ibot_wrapper.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/datasets/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/datasets/__init__.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4597 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/datasets/base_dataset.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/__init__.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     2052 2024-03-19 12:46:28.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/celeba_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3061 2024-03-19 12:46:40.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/chest_xray_covid_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     5606 2024-03-19 12:46:48.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/chexpert_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3867 2024-03-19 12:46:52.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/ddi_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4225 2024-03-21 10:45:08.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/derm7pt_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4143 2024-03-19 12:46:58.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/derma_compass_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     5317 2024-03-19 12:47:02.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/fitzpatrick17_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3137 2024-03-19 12:47:05.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/food101_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3893 2024-03-19 12:47:08.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/ham10000_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4525 2024-03-19 12:47:11.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/imagenet_1k_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3037 2024-03-19 12:47:15.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/imagenet_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4630 2024-03-19 12:47:42.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/isic_2018_task_1_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     2928 2024-03-19 12:47:42.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/isic_2019_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     1591 2024-03-19 12:47:42.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/med_node_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     2340 2024-03-19 12:47:42.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/oxford_flowers102_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4425 2024-03-21 10:45:08.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/pad_ufes_20_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3899 2024-03-19 12:47:42.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/passion_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3078 2024-03-19 12:47:42.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/pcam_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     2837 2024-03-19 12:47:42.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/ph2_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     5768 2024-03-19 12:47:42.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/ppp_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     6969 2024-03-21 10:45:08.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/sd_128_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     1112 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/stl_dataset.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     5283 2024-03-21 10:45:08.000000 selfclean-0.0.8/src/ssl_library/src/datasets/encrypted_image_dataset.py
--rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3410 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/datasets/generic_image_dataset.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     8765 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/datasets/helper.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2821 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/datasets/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/losses/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/losses/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2995 2024-03-19 16:49:00.000000 selfclean-0.0.8/src/ssl_library/src/losses/dino_loss.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      397 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/losses/distance_loss.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     5869 2024-02-27 09:14:07.000000 selfclean-0.0.8/src/ssl_library/src/losses/ibot_loss.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1172 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/losses/mae_loss.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2481 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/losses/nt_xent.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1025 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/losses/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/models/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/models/byol/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/byol/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1431 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/models/byol/model.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      433 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/byol/predictor.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/models/colorme/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/colorme/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1492 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/colorme/model.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.284810 selfclean-0.0.8/src/ssl_library/src/models/dino/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/dino/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1637 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/dino/head.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2291 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/dino/multi_crop_wrapper.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/models/encoders/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/encoders/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    36674 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/models/encoders/swin_transformer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1037 2024-03-19 12:52:07.000000 selfclean-0.0.8/src/ssl_library/src/models/encoders/utils.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    11283 2024-03-19 14:12:51.000000 selfclean-0.0.8/src/ssl_library/src/models/encoders/vision_transformer.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/models/fine_tuning/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/fine_tuning/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2104 2024-02-15 11:28:02.000000 selfclean-0.0.8/src/ssl_library/src/models/fine_tuning/classifiers.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    12386 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/fine_tuning/segmentation.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/models/ibot/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/ibot/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     2371 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/ibot/head.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/models/mae/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/mae/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     9486 2024-03-18 19:15:49.000000 selfclean-0.0.8/src/ssl_library/src/models/mae/model.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1804 2024-03-19 12:52:07.000000 selfclean-0.0.8/src/ssl_library/src/models/mae/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/models/simclr/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/simclr/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1090 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/simclr/model.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     7862 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/models/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/optimizers/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/optimizers/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3674 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/optimizers/lars.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1199 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/optimizers/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/pkg/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      108 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/pkg/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    23811 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/pkg/embedder.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     4033 2024-03-21 10:08:25.000000 selfclean-0.0.8/src/ssl_library/src/pkg/helper.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    10758 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/pkg/segmenter.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3463 2024-03-19 07:39:15.000000 selfclean-0.0.8/src/ssl_library/src/pkg/wrappers.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/trainers/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-16 07:42:07.000000 selfclean-0.0.8/src/ssl_library/src/trainers/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    13538 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/trainers/base_trainer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    10204 2024-03-21 10:08:51.000000 selfclean-0.0.8/src/ssl_library/src/trainers/byol_trainer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    10532 2024-03-21 10:09:03.000000 selfclean-0.0.8/src/ssl_library/src/trainers/colorme_trainer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    13494 2024-03-21 10:18:37.000000 selfclean-0.0.8/src/ssl_library/src/trainers/dino_trainer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    14347 2024-03-21 10:08:57.000000 selfclean-0.0.8/src/ssl_library/src/trainers/ibot_trainer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     8267 2024-03-21 10:08:44.000000 selfclean-0.0.8/src/ssl_library/src/trainers/mae_trainer.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     8079 2024-03-21 10:08:32.000000 selfclean-0.0.8/src/ssl_library/src/trainers/simclr_trainer.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/src/utils/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/utils/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      419 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/utils/loader.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    16513 2024-03-21 09:58:41.000000 selfclean-0.0.8/src/ssl_library/src/utils/logging.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1743 2024-02-15 06:34:51.000000 selfclean-0.0.8/src/ssl_library/src/utils/metrics.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)    14575 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/src/utils/prg.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     8677 2024-03-21 09:08:30.000000 selfclean-0.0.8/src/ssl_library/src/utils/utils.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/tests/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/tests/unittests/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/__init__.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/tests/unittests/augmentations/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/augmentations/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1333 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/augmentations/test_dino.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1368 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/augmentations/test_ibot.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1538 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/augmentations/test_simclr.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/tests/unittests/datasets/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/datasets/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     3801 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/datasets/test_encrypted_folder.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/ssl_library/tests/unittests/losses/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/losses/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      201 2024-02-14 09:58:40.000000 selfclean-0.0.8/src/ssl_library/tests/unittests/losses/test_dino_loss.py
-drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-21 11:45:20.288810 selfclean-0.0.8/src/utils/
--rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.8/src/utils/__init__.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)      197 2024-03-19 06:13:46.000000 selfclean-0.0.8/src/utils/paths.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     5236 2024-03-19 12:43:18.000000 selfclean-0.0.8/src/utils/plotting.py
--rw-rw-r--   0 fabian    (1000) fabian    (1000)     1670 2024-03-21 08:59:29.000000 selfclean-0.0.8/src/utils/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1487 2024-03-22 08:40:18.968561 selfclean-0.0.9/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      993 2024-03-21 10:44:06.000000 selfclean-0.0.9/README.md
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      580 2024-03-19 13:10:56.000000 selfclean-0.0.9/pyproject.toml
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.956561 selfclean-0.0.9/selfclean.egg-info/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1487 2024-03-22 08:40:18.000000 selfclean-0.0.9/selfclean.egg-info/PKG-INFO
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     6136 2024-03-22 08:40:18.000000 selfclean-0.0.9/selfclean.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-03-22 08:40:18.000000 selfclean-0.0.9/selfclean.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      242 2024-03-22 08:40:18.000000 selfclean-0.0.9/selfclean.egg-info/requires.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       10 2024-03-22 08:40:18.000000 selfclean-0.0.9/selfclean.egg-info/top_level.txt
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)       38 2024-03-22 08:40:18.968561 selfclean-0.0.9/setup.cfg
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1578 2024-03-22 08:40:08.000000 selfclean-0.0.9/setup.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.956561 selfclean-0.0.9/src/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      221 2024-03-19 13:12:36.000000 selfclean-0.0.9/src/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.956561 selfclean-0.0.9/src/cleaner/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.9/src/cleaner/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     6789 2024-03-22 06:27:16.000000 selfclean-0.0.9/src/cleaner/auto_cleaning_mixin.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      533 2024-03-22 07:38:10.000000 selfclean-0.0.9/src/cleaner/base_cleaner.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/cleaner/irrelevants/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.9/src/cleaner/irrelevants/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      242 2024-03-21 17:35:29.000000 selfclean-0.0.9/src/cleaner/irrelevants/base_irrelevant_mixin.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1271 2024-03-21 17:41:41.000000 selfclean-0.0.9/src/cleaner/irrelevants/lad_mixin.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1124 2024-03-22 05:34:51.000000 selfclean-0.0.9/src/cleaner/irrelevants/quantile_irrelevant_mixin.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2254 2024-03-22 08:23:50.000000 selfclean-0.0.9/src/cleaner/issue_manager.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/cleaner/label_errors/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.9/src/cleaner/label_errors/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      288 2024-03-21 17:35:29.000000 selfclean-0.0.9/src/cleaner/label_errors/base_label_error_mixin.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2933 2024-03-21 18:06:57.000000 selfclean-0.0.9/src/cleaner/label_errors/intra_extra_distance_mixin.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/cleaner/near_duplicates/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.9/src/cleaner/near_duplicates/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      249 2024-03-21 17:35:29.000000 selfclean-0.0.9/src/cleaner/near_duplicates/base_near_duplicate_mixin.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3011 2024-03-22 07:01:15.000000 selfclean-0.0.9/src/cleaner/near_duplicates/embedding_distance_mixin.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    11078 2024-03-22 07:38:34.000000 selfclean-0.0.9/src/cleaner/selfclean.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     7445 2024-03-22 08:29:30.000000 selfclean-0.0.9/src/cleaner/selfclean_cleaner.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/distances/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.9/src/distances/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      863 2024-02-14 14:17:25.000000 selfclean-0.0.9/src/distances/projective_distance.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/scoring/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.9/src/scoring/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    11629 2024-03-21 10:07:58.000000 selfclean-0.0.9/src/scoring/lad_scoring.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/ssl_library/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/ssl_library/src/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      217 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/ssl_library/src/augmentations/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/augmentations/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1131 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/augmentations/augmentations.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3069 2024-03-21 09:52:32.000000 selfclean-0.0.9/src/ssl_library/src/augmentations/dino.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     4484 2024-03-21 09:51:42.000000 selfclean-0.0.9/src/ssl_library/src/augmentations/ibot.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2407 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/augmentations/simclr.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/ssl_library/src/dataset_wrappers/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/dataset_wrappers/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      793 2024-03-21 09:07:23.000000 selfclean-0.0.9/src/ssl_library/src/dataset_wrappers/base_wrapper.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1220 2024-03-21 09:07:48.000000 selfclean-0.0.9/src/ssl_library/src/dataset_wrappers/colorme_wrapper.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     4739 2024-03-19 12:46:15.000000 selfclean-0.0.9/src/ssl_library/src/dataset_wrappers/ibot_wrapper.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.960561 selfclean-0.0.9/src/ssl_library/src/datasets/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/datasets/__init__.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4597 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/datasets/base_dataset.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/__init__.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     2052 2024-03-19 12:46:28.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/celeba_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3061 2024-03-19 12:46:40.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/chest_xray_covid_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     5606 2024-03-19 12:46:48.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/chexpert_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3867 2024-03-19 12:46:52.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/ddi_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4225 2024-03-21 11:47:37.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/derm7pt_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4143 2024-03-19 12:46:58.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/derma_compass_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     5317 2024-03-19 12:47:02.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/fitzpatrick17_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3137 2024-03-19 12:47:05.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/food101_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3893 2024-03-19 12:47:08.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/ham10000_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4525 2024-03-19 12:47:11.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/imagenet_1k_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3037 2024-03-19 12:47:15.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/imagenet_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4630 2024-03-19 12:47:42.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/isic_2018_task_1_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     2928 2024-03-19 12:47:42.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/isic_2019_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     1591 2024-03-19 12:47:42.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/med_node_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     2340 2024-03-19 12:47:42.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/oxford_flowers102_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     4425 2024-03-21 11:47:37.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/pad_ufes_20_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3899 2024-03-19 12:47:42.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/passion_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3078 2024-03-19 12:47:42.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/pcam_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     2837 2024-03-19 12:47:42.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/ph2_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     5768 2024-03-19 12:47:42.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/ppp_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     6969 2024-03-21 11:47:37.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/sd_128_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     1112 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/stl_dataset.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     5283 2024-03-21 11:47:37.000000 selfclean-0.0.9/src/ssl_library/src/datasets/encrypted_image_dataset.py
+-rwxrwxr-x   0 fabian    (1000) fabian    (1000)     3410 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/datasets/generic_image_dataset.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     8765 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/datasets/helper.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2821 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/datasets/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/losses/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/losses/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2995 2024-03-19 16:49:00.000000 selfclean-0.0.9/src/ssl_library/src/losses/dino_loss.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      397 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/losses/distance_loss.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     5869 2024-02-27 09:14:07.000000 selfclean-0.0.9/src/ssl_library/src/losses/ibot_loss.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1172 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/losses/mae_loss.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2481 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/losses/nt_xent.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1025 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/losses/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/byol/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/byol/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1431 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/models/byol/model.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      433 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/byol/predictor.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/colorme/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/colorme/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1492 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/colorme/model.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/dino/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/dino/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1637 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/dino/head.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2291 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/dino/multi_crop_wrapper.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/encoders/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/encoders/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    36674 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/models/encoders/swin_transformer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1037 2024-03-19 12:52:07.000000 selfclean-0.0.9/src/ssl_library/src/models/encoders/utils.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    11283 2024-03-19 14:12:51.000000 selfclean-0.0.9/src/ssl_library/src/models/encoders/vision_transformer.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/fine_tuning/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/fine_tuning/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2104 2024-02-15 11:28:02.000000 selfclean-0.0.9/src/ssl_library/src/models/fine_tuning/classifiers.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    12386 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/fine_tuning/segmentation.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/ibot/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/ibot/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     2371 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/ibot/head.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/mae/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/mae/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     9486 2024-03-18 19:15:49.000000 selfclean-0.0.9/src/ssl_library/src/models/mae/model.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1804 2024-03-19 12:52:07.000000 selfclean-0.0.9/src/ssl_library/src/models/mae/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/models/simclr/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        1 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/simclr/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1090 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/simclr/model.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     7862 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/models/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/optimizers/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/optimizers/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3674 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/optimizers/lars.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1199 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/optimizers/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.964561 selfclean-0.0.9/src/ssl_library/src/pkg/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      108 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/pkg/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    23811 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/pkg/embedder.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     4193 2024-03-22 07:45:04.000000 selfclean-0.0.9/src/ssl_library/src/pkg/helper.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    10758 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/pkg/segmenter.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3463 2024-03-19 07:39:15.000000 selfclean-0.0.9/src/ssl_library/src/pkg/wrappers.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/src/ssl_library/src/trainers/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-16 07:42:07.000000 selfclean-0.0.9/src/ssl_library/src/trainers/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    13538 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/trainers/base_trainer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    10204 2024-03-21 10:08:51.000000 selfclean-0.0.9/src/ssl_library/src/trainers/byol_trainer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    10532 2024-03-21 10:09:03.000000 selfclean-0.0.9/src/ssl_library/src/trainers/colorme_trainer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    13494 2024-03-21 10:18:37.000000 selfclean-0.0.9/src/ssl_library/src/trainers/dino_trainer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    14347 2024-03-21 10:08:57.000000 selfclean-0.0.9/src/ssl_library/src/trainers/ibot_trainer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     8267 2024-03-21 10:08:44.000000 selfclean-0.0.9/src/ssl_library/src/trainers/mae_trainer.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     8079 2024-03-21 10:08:32.000000 selfclean-0.0.9/src/ssl_library/src/trainers/simclr_trainer.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/src/ssl_library/src/utils/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/utils/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      419 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/utils/loader.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    16513 2024-03-21 09:58:41.000000 selfclean-0.0.9/src/ssl_library/src/utils/logging.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1743 2024-02-15 06:34:51.000000 selfclean-0.0.9/src/ssl_library/src/utils/metrics.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)    14575 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/src/utils/prg.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     8677 2024-03-21 09:08:30.000000 selfclean-0.0.9/src/ssl_library/src/utils/utils.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/src/ssl_library/tests/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/src/ssl_library/tests/unittests/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/__init__.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/src/ssl_library/tests/unittests/augmentations/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/augmentations/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1333 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/augmentations/test_dino.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1368 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/augmentations/test_ibot.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1538 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/augmentations/test_simclr.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/src/ssl_library/tests/unittests/datasets/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/datasets/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     3801 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/datasets/test_encrypted_folder.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/src/ssl_library/tests/unittests/losses/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/losses/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      201 2024-02-14 09:58:40.000000 selfclean-0.0.9/src/ssl_library/tests/unittests/losses/test_dino_loss.py
+drwxrwxr-x   0 fabian    (1000) fabian    (1000)        0 2024-03-22 08:40:18.968561 selfclean-0.0.9/src/utils/
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)        0 2024-02-14 14:17:25.000000 selfclean-0.0.9/src/utils/__init__.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)      197 2024-03-19 06:13:46.000000 selfclean-0.0.9/src/utils/paths.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     4912 2024-03-22 07:34:22.000000 selfclean-0.0.9/src/utils/plotting.py
+-rw-rw-r--   0 fabian    (1000) fabian    (1000)     1684 2024-03-21 18:06:32.000000 selfclean-0.0.9/src/utils/utils.py
```

### Comparing `selfclean-0.0.8/PKG-INFO` & `selfclean-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfclean
-Version: 0.0.8
+Version: 0.0.9
 Summary: A holistic self-supervised data cleaning strategy to detect irrelevant samples, near duplicates and label errors.
 Home-page: https://github.com/Digital-Dermatology/SelfClean
 Author: Fabian Groeger
 Author-email: fabian.groeger@unibas.ch
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `selfclean-0.0.8/README.md` & `selfclean-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/pyproject.toml` & `selfclean-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/selfclean.egg-info/PKG-INFO` & `selfclean-0.0.9/selfclean.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfclean
-Version: 0.0.8
+Version: 0.0.9
 Summary: A holistic self-supervised data cleaning strategy to detect irrelevant samples, near duplicates and label errors.
 Home-page: https://github.com/Digital-Dermatology/SelfClean
 Author: Fabian Groeger
 Author-email: fabian.groeger@unibas.ch
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `selfclean-0.0.8/selfclean.egg-info/SOURCES.txt` & `selfclean-0.0.9/selfclean.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 selfclean.egg-info/dependency_links.txt
 selfclean.egg-info/requires.txt
 selfclean.egg-info/top_level.txt
 src/__init__.py
 src/cleaner/__init__.py
 src/cleaner/auto_cleaning_mixin.py
 src/cleaner/base_cleaner.py
+src/cleaner/issue_manager.py
 src/cleaner/selfclean.py
 src/cleaner/selfclean_cleaner.py
 src/cleaner/irrelevants/__init__.py
 src/cleaner/irrelevants/base_irrelevant_mixin.py
 src/cleaner/irrelevants/lad_mixin.py
 src/cleaner/irrelevants/quantile_irrelevant_mixin.py
 src/cleaner/label_errors/__init__.py
```

### Comparing `selfclean-0.0.8/setup.py` & `selfclean-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     SOURCE_PACKAGE_REGEX.sub(PACKAGE_NAME, name) for name in source_packages
 ]
 
 setup(
     name=PACKAGE_NAME,
     packages=proj_packages,
     package_dir={PACKAGE_NAME: SOURCE_DIRECTORY},
-    version="0.0.8",
+    version="0.0.9",
     author="Fabian Groeger",
     author_email="fabian.groeger@unibas.ch",
     description="A holistic self-supervised data cleaning strategy to detect irrelevant samples, near duplicates and label errors.",
     long_description=README_MD,
     long_description_content_type="text/markdown",
     url="https://github.com/Digital-Dermatology/SelfClean",
     python_requires=">=3.6",
```

### Comparing `selfclean-0.0.8/src/cleaner/auto_cleaning_mixin.py` & `selfclean-0.0.9/src/cleaner/auto_cleaning_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Optional
+from pathlib import Path
+from typing import Optional, Union
 
 import numpy as np
 import scipy
 import scipy.stats
 from loguru import logger
 
 from ..utils.plotting import (
@@ -32,15 +33,15 @@
 
     def perform_auto_cleaning(
         self,
         return_dict: dict,
         pred_near_duplicate_scores: np.ndarray,
         pred_irrelevant_scores: np.ndarray,
         pred_label_error_scores: Optional[np.ndarray],
-        output_path: Optional[str] = None,
+        output_path: Optional[Union[str, Path]] = None,
     ):
         if self.auto_cleaning:
             # Near Duplicates
             if output_path is not None:
                 self.cleaner_kwargs[
                     "path"
                 ] = f"{output_path.stem}_auto_dups{output_path.suffix}"
```

### Comparing `selfclean-0.0.8/src/cleaner/irrelevants/lad_mixin.py` & `selfclean-0.0.9/src/cleaner/irrelevants/lad_mixin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from typing import List, Tuple
+from typing import Tuple
 
 import numpy as np
 from scipy.cluster.hierarchy import single
 
 from ...cleaner.irrelevants.base_irrelevant_mixin import BaseIrrelevantMixin
 from ...scoring.lad_scoring import LAD
 from ...ssl_library.src.utils.logging import plot_dist
 
 
 class LADIrrelevantMixin(BaseIrrelevantMixin):
     def __init__(self, global_leaves: bool = False, **kwargs):
         super().__init__(**kwargs)
         self.global_leaves = global_leaves
 
-    def get_irrelevant_ranking(self) -> List[Tuple[float, int]]:
+    def get_irrelevant_ranking(self) -> Tuple[np.ndarray, np.ndarray]:
         # linkage_matrix: [idx1, idx2, dist, sample_count]
         linkage_matrix = single(self.p_distances)
         lad = LAD()
-        irrelevant_score = lad.calc_scores(
+        irrelevants = lad.calc_scores(
             linkage_matrix=linkage_matrix,
             global_leaves=self.global_leaves,
         )
         # free up allocated memory
         del lad, linkage_matrix
 
-        if self.plot_distribution and irrelevant_score is not None:
+        if self.plot_distribution and irrelevants is not None:
             plot_dist(
-                scores=np.asarray([x[0] for x in irrelevant_score]),
+                scores=np.asarray([x[0] for x in irrelevants]),
                 title="Distribution of irrelevant samples",
             )
-        return irrelevant_score
+        irrelevant_scores = np.asarray([x[0] for x in irrelevants])
+        irrelevant_indices = np.asarray([x[1] for x in irrelevants])
+        return irrelevant_scores, irrelevant_indices
```

### Comparing `selfclean-0.0.8/src/cleaner/irrelevants/quantile_irrelevant_mixin.py` & `selfclean-0.0.9/src/cleaner/irrelevants/quantile_irrelevant_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-from typing import List, Tuple
+from typing import Tuple
 
 import numpy as np
 
 from ...cleaner.irrelevants.base_irrelevant_mixin import BaseIrrelevantMixin
 from ...ssl_library.src.utils.logging import plot_dist
-from ...utils.plotting import plot_irrelevant_samples
 
 
 class QuantileIrrelevantMixin(BaseIrrelevantMixin):
     def __init__(self, quantile: float = 0.01, **kwargs):
         super().__init__(**kwargs)
         self.quantile = quantile
 
-    def get_irrelevant_ranking(self) -> List[Tuple[float, int]]:
-        irrelevant_score = np.quantile(self.distance_matrix, self.quantile, axis=0)
-        irrelevant_score = [(irrelevant_score[i], i) for i in list(range(self.N))]
-        irrelevant_score = sorted(
-            irrelevant_score,
+    def get_irrelevant_ranking(self) -> Tuple[np.ndarray, np.ndarray]:
+        irrelevants = np.quantile(self.distance_matrix, self.quantile, axis=0)
+        irrelevants = [(irrelevants[i], i) for i in list(range(self.N))]
+        irrelevants = sorted(
+            irrelevants,
             key=lambda tup: tup[0],
             reverse=True,
         )
 
-        if self.plot_top_N is not None and self.images is not None:
-            plot_irrelevant_samples(
-                irrelevant_score=irrelevant_score,
-                images=self.images,
-                plot_top_N=self.plot_top_N,
-                plot_title=self.plot_title,
-                return_fig=self.return_fig,
-            )
-
-        if self.plot_distribution and irrelevant_score is not None:
+        if self.plot_distribution and irrelevants is not None:
             plot_dist(
-                scores=np.asarray([x[0] for x in irrelevant_score]),
+                scores=np.asarray([x[0] for x in irrelevants]),
                 title="Distribution of irrelevant samples",
             )
-        return irrelevant_score
+        irrelevant_scores = np.asarray([x[0] for x in irrelevants])
+        irrelevant_indices = np.asarray([x[1] for x in irrelevants])
+        return irrelevant_scores, irrelevant_indices
```

### Comparing `selfclean-0.0.8/src/cleaner/label_errors/intra_extra_distance_mixin.py` & `selfclean-0.0.9/src/cleaner/label_errors/intra_extra_distance_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import List, Optional, Tuple
+from typing import Optional, Tuple
 
 import numpy as np
 
 from ...cleaner.label_errors.base_label_error_mixin import BaseLabelErrorMixin
 from ...ssl_library.src.utils.logging import plot_dist
 from ...utils.utils import has_same_label
 
@@ -15,16 +15,16 @@
 
         The samples which have a smaller distance to a sample with an other label
         than to their own have a larger score.
         """
         assert self.labels is not None
         # create a int matrix of same label relation
         L = has_same_label(self.labels)
-        o_hot_same = L.astype(float)
-        o_hot_diff = (~L).astype(float)
+        o_hot_same = L.astype(np.float16)
+        o_hot_diff = (~L).astype(np.float16)
         # set non-equal values to inf for multiplication
         o_hot_same[o_hot_same == 0.0] = np.inf
         o_hot_diff[o_hot_diff == 0.0] = np.inf
         # ensure one can not choose it's own distance
         np.fill_diagonal(o_hot_same, np.inf)
         # calc. the matrices for same and other lbl dists.
         with np.errstate(all="ignore"):
@@ -38,29 +38,33 @@
             min_same[missing_same_indices] = (
                 np.ma.masked_invalid(val_missing).max(axis=-1).data
             )
         # calc. score matrix
         lbl_scores = (min_diff**2) / (min_same**2 + min_diff**2)
         return lbl_scores
 
-    def get_label_error_ranking(self) -> Optional[List[Tuple[float, int]]]:
+    def get_label_error_ranking(
+        self,
+    ) -> Tuple[Optional[np.ndarray], Optional[np.ndarray]]:
         if self.labels is None:
             warnings.warn("Can't find label errors without having access to labels.")
-            return None
+            return None, None
         if len(np.unique(self.labels)) == 1:
             warnings.warn("Can't detect label errors with only one label.")
-            return None
+            return None, None
 
-        label_error_scores = self.labels_calc_scores()
-        label_error_scores = [(label_error_scores[i], i) for i in list(range(self.N))]
-        label_error_scores = sorted(
-            label_error_scores,
+        label_errors = self.labels_calc_scores()
+        label_errors = [(label_errors[i], i) for i in list(range(self.N))]
+        label_errors = sorted(
+            label_errors,
             key=lambda tup: tup[0],
             reverse=False,
         )
 
         if self.plot_distribution:
             plot_dist(
-                scores=np.asarray([x[0] for x in label_error_scores]),
+                scores=np.asarray([x[0] for x in label_errors]),
                 title="Distribution of possible label errors",
             )
-        return label_error_scores
+        label_error_scores = np.asarray([x[0] for x in label_errors])
+        label_error_indices = np.asarray([x[1] for x in label_errors])
+        return label_error_scores, label_error_indices
```

### Comparing `selfclean-0.0.8/src/cleaner/near_duplicates/embedding_distance_mixin.py` & `selfclean-0.0.9/src/cleaner/near_duplicates/embedding_distance_mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import math
-from typing import List, Tuple
+from typing import Tuple
 
 import numpy as np
 from tqdm.auto import tqdm
 
 from ...cleaner.near_duplicates.base_near_duplicate_mixin import BaseNearDuplicateMixin
 from ...ssl_library.src.utils.logging import plot_dist
 from ...utils.utils import condensed_to_square
 
 
 class EmbeddingDistanceMixin(BaseNearDuplicateMixin):
-    def get_near_duplicate_ranking(self) -> List[Tuple[float, int]]:
+    def get_near_duplicate_ranking(self) -> Tuple[np.ndarray, np.ndarray]:
         if self.memmap:
             score_file = self.memmap_path / "near_duplicate_scores.dat"
             # make sure the files do not exist already
             if score_file.exists():
                 score_file.unlink()
             scores_near_dup = np.memmap(
                 str(score_file),
@@ -27,14 +27,16 @@
                 shape=(self.condensed_size,),
                 dtype=self.precision_type_distance,
             )
 
         # sort the values in the condensed matrix
         sorting = self.p_distances.argsort()
         scores_near_dup[:] = np.take(self.p_distances, indices=sorting, axis=0)
+        if self.memmap:
+            scores_near_dup.flush()
         # vectorize the mapping function
         vec_index_mapping = np.vectorize(condensed_to_square)
         # here the chunk size is x**2 since we have quadratically more
         chunk_size = self.chunk_size**2
         # chunk the sorted values for memory optimization
         n_chunks = math.ceil(self.condensed_size / chunk_size)
         if self.memmap:
@@ -61,15 +63,17 @@
             leave=True,
         ):
             chunk_slice = slice(i * chunk_size, (i + 1) * chunk_size, 1)
             chunk_sorting = sorting[chunk_slice]
             # map the indices from the condensed to the redundant distance matrix
             mapping_row = np.asarray(vec_index_mapping(chunk_sorting, self.N)).T
             indices_near_dup[chunk_slice, :] = mapping_row
+            if self.memmap:
+                indices_near_dup.flush()
             del mapping_row
 
         if self.plot_distribution:
             plot_dist(
                 scores=scores_near_dup,
                 title="Distribution of near-duplicates",
             )
-        return list(zip(scores_near_dup, indices_near_dup))
+        return scores_near_dup, indices_near_dup
```

### Comparing `selfclean-0.0.8/src/cleaner/selfclean.py` & `selfclean-0.0.9/src/cleaner/selfclean.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     "lr": 0.0005,
     "min_lr": "1e-6",
     "weight_decay": 0.04,
     "weight_decay_end": 0.4,
     "warmup_epochs": 10,
     "momentum_teacher": 0.996,
     "clip_grad": 3.0,
-    "apply_l2_norm": False,  # TODO: check influence of this
+    "apply_l2_norm": True,
     "save_every_n_epochs": 10,
     "model": {
         "out_dim": 4096,
         "emb_dim": 192,
         "base_model": "vit_tiny",
         "model_type": "VIT",
         "use_bn_in_head": False,
         "norm_last_layer": True,
         "student": {
-            "drop_path_rate": 0.1,  # TODO: check influence of this
+            "drop_path_rate": 0.1,
             "pretrained": True,
         },
         "teacher": {
-            "drop_path_rate": 0.1,  # TODO: check influence of this
+            "drop_path_rate": 0.1,
             "pretrained": True,
         },
         "eval": {"n_last_blocks": 4, "avgpool_patchtokens": False},
     },
     "dataset": {
         "augmentations": {
             "global_crops_scale": "(0.7, 1.)",
@@ -243,32 +243,34 @@
         set_dataset_transformation(dataset=dataset, transform=self.base_transform)
         torch_dataset = DataLoader(
             dataset,
             batch_size=batch_size,
             drop_last=False,
             shuffle=False,
         )
-        emb_space, labels, images, paths = embed_dataset(
+        emb_space, labels = embed_dataset(
             torch_dataset=torch_dataset,
             model=self.model,
             n_layers=n_layers,
             normalize=apply_l2_norm,
             memmap=self.memmap,
             memmap_path=self.memmap_path,
             tqdm_desc="Creating dataset representation",
+            return_only_embedding_and_labels=True,
         )
         # for default datasets we can set the paths manually
+        paths = None
         if hasattr(dataset, "_image_files") and paths is None:
             paths = dataset._image_files
 
         self.cleaner.fit(
             emb_space=np.asarray(emb_space),
-            images=np.asarray(images),
             labels=np.asarray(labels),
             paths=np.asarray(paths) if paths is not None else paths,
+            dataset=dataset,
             class_labels=dataset.classes if hasattr(dataset, "classes") else None,
         )
         return self.cleaner.predict()
 
     def train_dino(
         self,
         dataset: Dataset,
```

### Comparing `selfclean-0.0.8/src/cleaner/selfclean_cleaner.py` & `selfclean-0.0.9/src/cleaner/selfclean_cleaner.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 import tempfile
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 import numpy as np
 import scienceplots  # noqa: F401
 import sklearn  # noqa: F401
+from torch.utils.data import Dataset
 from tqdm.auto import tqdm
 
 from ..cleaner.auto_cleaning_mixin import AutoCleaningMixin
 from ..cleaner.base_cleaner import BaseCleaner
 from ..cleaner.irrelevants.lad_mixin import LADIrrelevantMixin
+from ..cleaner.issue_manager import IssueManager
 from ..cleaner.label_errors.intra_extra_distance_mixin import (
     IntraExtraDistanceLabelErrorMixin,
 )
 from ..cleaner.near_duplicates.embedding_distance_mixin import EmbeddingDistanceMixin
 from ..distances import *  # noqa: F401, F403
 from ..distances.projective_distance import *  # noqa: F401, F403
 from ..ssl_library.src.utils.logging import set_log_level
@@ -77,20 +79,20 @@
         self.figsize = figsize
         super().__init__(**kwargs)
 
     def fit(
         self,
         emb_space: np.ndarray,
         labels: Optional[np.ndarray] = None,
-        images: Optional[np.ndarray] = None,
         paths: Optional[np.ndarray] = None,
+        dataset: Optional[Dataset] = None,
         class_labels: Optional[list] = None,
     ):
         self.labels = labels
-        self.images = images
+        self.dataset = dataset
         self.paths = paths
         self.class_labels = class_labels
         self.N, self.D = emb_space.shape
         self.condensed_size = int(self.N * ((self.N - 1) / 2))
 
         if self.memmap:
             dist_file = self.memmap_path / "dist_matrix.dat"
@@ -149,63 +151,57 @@
                 dtype=self.precision_type_distance,
             )
         self.p_distances[:] = self.distance_matrix[
             ~np.tril(np.ones((self.N, self.N), dtype=bool))
         ]
         return self
 
-    def predict(self) -> dict:
-        pred_nd = self.get_near_duplicate_ranking()
-        pred_nd_scores = np.asarray([x[0] for x in pred_nd])
-        pred_nd_indices = np.asarray([x[1] for x in pred_nd])
-        del pred_nd
-
-        pred_oods = self.get_irrelevant_ranking()
-        pred_oods_scores = np.asarray([x[0] for x in pred_oods])
-        pred_oods_indices = np.asarray([x[1] for x in pred_oods])
-        del pred_oods
-
-        pred_lbl_errs = self.get_label_error_ranking()
-        if pred_lbl_errs is not None:
-            pred_lbl_errs_scores = np.asarray([x[0] for x in pred_lbl_errs])
-            pred_lbl_errs_indices = np.asarray([x[1] for x in pred_lbl_errs])
-        else:
-            pred_lbl_errs_scores = None
-            pred_lbl_errs_indices = None
-        del pred_lbl_errs
+    def predict(self) -> IssueManager:
+        pred_nd_scores, pred_nd_indices = self.get_near_duplicate_ranking()
+        pred_oods_scores, pred_oods_indices = self.get_irrelevant_ranking()
+        pred_lbl_errs_scores, pred_lbl_errs_indices = self.get_label_error_ranking()
+
+        # transform labels using class names if given
+        if self.labels is not None:
+            self.labels = [
+                self.class_labels[x] if self.class_labels is not None else x
+                for x in self.labels
+            ]
 
-        if self.plot_top_N is not None and self.images is not None:
+        if self.plot_top_N is not None and self.dataset is not None:
             plot_inspection_result(
                 pred_dups_indices=pred_nd_indices,
                 pred_oods_indices=pred_oods_indices,
                 pred_lbl_errs_indices=pred_lbl_errs_indices,
-                images=self.images,
+                dataset=self.dataset,
                 labels=self.labels,
-                class_labels=self.class_labels,
                 plot_top_N=self.plot_top_N,
                 output_path=self.output_path,
                 figsize=self.figsize,
             )
 
+        meta_data_dict = {
+            "path": self.paths,
+            "label": self.labels,
+        }
         return_dict = {
             "irrelevants": {
                 "indices": pred_oods_indices,
                 "scores": pred_oods_scores,
             },
             "near_duplicates": {
                 "indices": pred_nd_indices,
                 "scores": pred_nd_scores,
             },
             "label_errors": {
                 "indices": pred_lbl_errs_indices,
                 "scores": pred_lbl_errs_scores,
             },
         }
-
         return_dict = self.perform_auto_cleaning(
             return_dict=return_dict,
             pred_near_duplicate_scores=pred_nd_scores,
             pred_irrelevant_scores=pred_oods_scores,
             pred_label_error_scores=pred_lbl_errs_scores,
             output_path=self.output_path,
         )
-        return return_dict
+        return IssueManager(issue_dict=return_dict, meta_data_dict=meta_data_dict)
```

### Comparing `selfclean-0.0.8/src/distances/projective_distance.py` & `selfclean-0.0.9/src/distances/projective_distance.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/scoring/lad_scoring.py` & `selfclean-0.0.9/src/scoring/lad_scoring.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/augmentations/augmentations.py` & `selfclean-0.0.9/src/ssl_library/src/augmentations/augmentations.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/augmentations/dino.py` & `selfclean-0.0.9/src/ssl_library/src/augmentations/dino.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/augmentations/ibot.py` & `selfclean-0.0.9/src/ssl_library/src/augmentations/ibot.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/augmentations/simclr.py` & `selfclean-0.0.9/src/ssl_library/src/augmentations/simclr.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/dataset_wrappers/base_wrapper.py` & `selfclean-0.0.9/src/ssl_library/src/dataset_wrappers/base_wrapper.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/dataset_wrappers/colorme_wrapper.py` & `selfclean-0.0.9/src/ssl_library/src/dataset_wrappers/colorme_wrapper.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/dataset_wrappers/ibot_wrapper.py` & `selfclean-0.0.9/src/ssl_library/src/dataset_wrappers/ibot_wrapper.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/base_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/base_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/celeba_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/celeba_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/chest_xray_covid_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/chest_xray_covid_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/chexpert_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/chexpert_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/ddi_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/ddi_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/derm7pt_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/derm7pt_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/derma_compass_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/derma_compass_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/fitzpatrick17_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/fitzpatrick17_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/food101_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/food101_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/ham10000_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/ham10000_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/imagenet_1k_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/imagenet_1k_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/imagenet_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/imagenet_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/isic_2018_task_1_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/isic_2018_task_1_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/isic_2019_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/isic_2019_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/med_node_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/med_node_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/oxford_flowers102_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/oxford_flowers102_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/pad_ufes_20_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/pad_ufes_20_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/passion_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/passion_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/pcam_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/pcam_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/ph2_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/ph2_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/ppp_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/ppp_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/sd_128_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/sd_128_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/downstream_tasks/stl_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/downstream_tasks/stl_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/encrypted_image_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/encrypted_image_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/generic_image_dataset.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/generic_image_dataset.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/helper.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/helper.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/datasets/utils.py` & `selfclean-0.0.9/src/ssl_library/src/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/losses/dino_loss.py` & `selfclean-0.0.9/src/ssl_library/src/losses/dino_loss.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/losses/ibot_loss.py` & `selfclean-0.0.9/src/ssl_library/src/losses/ibot_loss.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/losses/mae_loss.py` & `selfclean-0.0.9/src/ssl_library/src/losses/mae_loss.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/losses/nt_xent.py` & `selfclean-0.0.9/src/ssl_library/src/losses/nt_xent.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/losses/utils.py` & `selfclean-0.0.9/src/ssl_library/src/losses/utils.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/byol/model.py` & `selfclean-0.0.9/src/ssl_library/src/models/byol/model.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/colorme/model.py` & `selfclean-0.0.9/src/ssl_library/src/models/colorme/model.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/dino/head.py` & `selfclean-0.0.9/src/ssl_library/src/models/dino/head.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/dino/multi_crop_wrapper.py` & `selfclean-0.0.9/src/ssl_library/src/models/dino/multi_crop_wrapper.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/encoders/swin_transformer.py` & `selfclean-0.0.9/src/ssl_library/src/models/encoders/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/encoders/utils.py` & `selfclean-0.0.9/src/ssl_library/src/models/encoders/utils.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/encoders/vision_transformer.py` & `selfclean-0.0.9/src/ssl_library/src/models/encoders/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/fine_tuning/classifiers.py` & `selfclean-0.0.9/src/ssl_library/src/models/fine_tuning/classifiers.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/fine_tuning/segmentation.py` & `selfclean-0.0.9/src/ssl_library/src/models/fine_tuning/segmentation.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/ibot/head.py` & `selfclean-0.0.9/src/ssl_library/src/models/ibot/head.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/mae/model.py` & `selfclean-0.0.9/src/ssl_library/src/models/mae/model.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/mae/utils.py` & `selfclean-0.0.9/src/ssl_library/src/models/mae/utils.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/simclr/model.py` & `selfclean-0.0.9/src/ssl_library/src/models/simclr/model.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/models/utils.py` & `selfclean-0.0.9/src/ssl_library/src/models/utils.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/optimizers/lars.py` & `selfclean-0.0.9/src/ssl_library/src/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/optimizers/utils.py` & `selfclean-0.0.9/src/ssl_library/src/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/pkg/embedder.py` & `selfclean-0.0.9/src/ssl_library/src/pkg/embedder.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/pkg/helper.py` & `selfclean-0.0.9/src/ssl_library/src/pkg/helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     model,
     n_layers: int,
     normalize: bool = False,
     memmap: bool = True,
     memmap_path: Union[Path, str, None] = None,
     return_only_embedding_and_labels: bool = False,
     tqdm_desc: Optional[str] = None,
-) -> Tuple[ARR_TYPE, ARR_TYPE, ARR_TYPE, ARR_TYPE]:
+) -> Union[Tuple[ARR_TYPE, ARR_TYPE, ARR_TYPE, ARR_TYPE], Tuple[ARR_TYPE, ARR_TYPE]]:
     labels = []
     paths = []
     batch_size = torch_dataset.batch_size
     iterator = tqdm(
         enumerate(torch_dataset),
         position=0,
         leave=True,
@@ -45,23 +45,25 @@
         memmap_path = create_memmap_path(memmap_path=memmap_path)
         emb_space = create_memmap(
             memmap_path,
             "embedding_space.dat",
             len(torch_dataset.dataset),
             *(emb_dim,),
         )
-        images = create_memmap(
-            memmap_path,
-            "images.dat",
-            len(torch_dataset.dataset),
-            *batch_dim,
-        )
+        if not return_only_embedding_and_labels:
+            images = create_memmap(
+                memmap_path,
+                "images.dat",
+                len(torch_dataset.dataset),
+                *batch_dim,
+            )
     else:
         emb_space = np.zeros(shape=(len(torch_dataset.dataset), emb_dim))
-        images = np.zeros(shape=(len(torch_dataset.dataset), *batch_dim))
+        if not return_only_embedding_and_labels:
+            images = np.zeros(shape=(len(torch_dataset.dataset), *batch_dim))
     del emb_dim, batch_dim, _batch
     # embed the dataset
     for i, batch_tup in iterator:
         if len(batch_tup) == 3:
             batch, path, label = batch_tup
         elif len(batch_tup) == 2:
             batch, label = batch_tup
```

### Comparing `selfclean-0.0.8/src/ssl_library/src/pkg/segmenter.py` & `selfclean-0.0.9/src/ssl_library/src/pkg/segmenter.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/pkg/wrappers.py` & `selfclean-0.0.9/src/ssl_library/src/pkg/wrappers.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/trainers/base_trainer.py` & `selfclean-0.0.9/src/ssl_library/src/trainers/base_trainer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/trainers/byol_trainer.py` & `selfclean-0.0.9/src/ssl_library/src/trainers/byol_trainer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/trainers/colorme_trainer.py` & `selfclean-0.0.9/src/ssl_library/src/trainers/colorme_trainer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/trainers/dino_trainer.py` & `selfclean-0.0.9/src/ssl_library/src/trainers/dino_trainer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/trainers/ibot_trainer.py` & `selfclean-0.0.9/src/ssl_library/src/trainers/ibot_trainer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/trainers/mae_trainer.py` & `selfclean-0.0.9/src/ssl_library/src/trainers/mae_trainer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/trainers/simclr_trainer.py` & `selfclean-0.0.9/src/ssl_library/src/trainers/simclr_trainer.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/utils/logging.py` & `selfclean-0.0.9/src/ssl_library/src/utils/logging.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/utils/metrics.py` & `selfclean-0.0.9/src/ssl_library/src/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/utils/prg.py` & `selfclean-0.0.9/src/ssl_library/src/utils/prg.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/src/utils/utils.py` & `selfclean-0.0.9/src/ssl_library/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/tests/unittests/augmentations/test_dino.py` & `selfclean-0.0.9/src/ssl_library/tests/unittests/augmentations/test_dino.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/tests/unittests/augmentations/test_ibot.py` & `selfclean-0.0.9/src/ssl_library/tests/unittests/augmentations/test_ibot.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/tests/unittests/augmentations/test_simclr.py` & `selfclean-0.0.9/src/ssl_library/tests/unittests/augmentations/test_simclr.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/ssl_library/tests/unittests/datasets/test_encrypted_folder.py` & `selfclean-0.0.9/src/ssl_library/tests/unittests/datasets/test_encrypted_folder.py`

 * *Files identical despite different names*

### Comparing `selfclean-0.0.8/src/utils/plotting.py` & `selfclean-0.0.9/src/utils/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,57 @@
 from pathlib import Path
 from typing import Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
+from torch.utils.data import Dataset
 from torchvision import transforms
 
 from ..ssl_library.src.utils.logging import create_subtitle, denormalize_image
 
 
 def plot_inspection_result(
     pred_dups_indices: np.ndarray,
     pred_oods_indices: np.ndarray,
-    images: np.ndarray,
+    dataset: Dataset,
     plot_top_N: int,
     pred_lbl_errs_indices: Optional[np.ndarray] = None,
     labels: Optional[np.ndarray] = None,
-    class_labels: Optional[list] = None,
     output_path: Optional[Union[str, Path]] = None,
     figsize: tuple = (10, 8),
 ):
     rows = 4 if pred_lbl_errs_indices is not None else 3
     fig, ax = plt.subplots(rows, plot_top_N, figsize=figsize)
     for i, (idx1, idx2) in enumerate(pred_dups_indices[:plot_top_N]):
-        ax[0, i].imshow(transforms.ToPILImage()(denormalize_image(images[int(idx1)])))
-        ax[1, i].imshow(transforms.ToPILImage()(denormalize_image(images[int(idx2)])))
+        ax[0, i].imshow(
+            transforms.ToPILImage()(denormalize_image(dataset[int(idx1)][0]))
+        )
+        ax[1, i].imshow(
+            transforms.ToPILImage()(denormalize_image(dataset[int(idx2)][0]))
+        )
         ax[0, i].set_xticks([])
         ax[0, i].set_yticks([])
         ax[1, i].set_xticks([])
         ax[1, i].set_yticks([])
         ax[0, i].set_title(f"Ranking: {i+1}, Idx: {int(idx1)}", fontsize=6)
         ax[1, i].set_title(f"Idx: {int(idx2)}", fontsize=6)
 
     for i, idx in enumerate(pred_oods_indices[:plot_top_N]):
-        ax[2, i].imshow(transforms.ToPILImage()(denormalize_image(images[int(idx)])))
+        ax[2, i].imshow(
+            transforms.ToPILImage()(denormalize_image(dataset[int(idx)][0]))
+        )
         ax[2, i].set_title(f"Ranking: {i+1}, Idx: {int(idx)}", fontsize=6)
         ax[2, i].set_xticks([])
         ax[2, i].set_yticks([])
 
     if pred_lbl_errs_indices is not None:
         for i, idx in enumerate(pred_lbl_errs_indices[:plot_top_N]):
-            class_label = get_label_from_index(
-                index=idx, labels=labels, class_labels=class_labels
-            )
+            class_label = labels[idx] if labels is not None else None
             ax[3, i].imshow(
-                transforms.ToPILImage()(denormalize_image(images[int(idx)]))
+                transforms.ToPILImage()(denormalize_image(dataset[int(idx)][0]))
             )
             ax[3, i].set_title(
                 f"Ranking: {i+1}\nIdx: {int(idx)}\nLbl: {class_label}",
                 fontsize=6,
             )
             ax[3, i].set_xticks([])
             ax[3, i].set_yticks([])
@@ -59,28 +63,14 @@
         create_subtitle(fig, grid[3, ::], "Label Error Ranking", fontsize=12)
     fig.tight_layout()
     if output_path is not None:
         plt.savefig(output_path, bbox_inches="tight")
     plt.show()
 
 
-def get_label_from_index(
-    index: int,
-    labels: Optional[np.ndarray] = None,
-    class_labels: Optional[list] = None,
-):
-    index = int(index)
-    if class_labels is not None and labels is not None:
-        return class_labels[labels[index]]
-    elif labels is not None:
-        return labels[index]
-    else:
-        return index
-
-
 def plot_frac_cut(dist, logit_scores, bins, q1, q2, cutoff, loc, scale, path):
     with plt.style.context(["science", "std-colors", "grid"]):
         dist_name = dist.__class__.__name__.split("_")[0]
         fig, ax = plt.subplots(1, 1, figsize=(4, 3))
         subplot_frac_cut(
             ax,
             logit_scores,
```

### Comparing `selfclean-0.0.8/src/utils/utils.py` & `selfclean-0.0.9/src/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     shifts = np.concatenate([[0], n_row_elems])
     jj = np.arange(1, n)[ii] + idx - shifts[ii]
     if np.sum(ii < 0) > 0 or np.sum(jj < 0) > 0:
         logger.error("Negative indices")
     return ii, jj
 
 
-def has_same_label(arr):
+def has_same_label(arr) -> np.ndarray:
     arr = np.array(arr)
     result = arr[:, None] == arr
     return result
 
 
 def set_dataset_transformation(dataset: Dataset, transform: torch.nn.Module):
     def _set_transform(d: Dataset, transform: torch.nn.Module):
```

