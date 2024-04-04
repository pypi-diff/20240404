# Comparing `tmp/ficture-0.0.1.post3.tar.gz` & `tmp/ficture-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ficture-0.0.1.post3.tar", last modified: Wed Nov 15 01:21:10 2023, max compression
+gzip compressed data, was "ficture-0.0.2.tar", last modified: Thu Apr  4 13:58:05 2024, max compression
```

## Comparing `ficture-0.0.1.post3.tar` & `ficture-0.0.2.tar`

### file list

```diff
@@ -1,60 +1,71 @@
-drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-15 01:21:10.538207 ficture-0.0.1.post3/
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    19347 2023-09-11 21:49:40.000000 ficture-0.0.1.post3/LICENSE
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       57 2023-11-04 03:07:00.000000 ficture-0.0.1.post3/MANIFEST.in
--rwxrwxr--   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1705 2023-11-15 01:21:10.533696 ficture-0.0.1.post3/PKG-INFO
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      911 2023-11-15 01:19:24.000000 ficture-0.0.1.post3/README.md
-drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-15 01:21:10.148594 ficture-0.0.1.post3/ficture/
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      263 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/__init__.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1387 2023-11-06 05:22:28.000000 ficture-0.0.1.post3/ficture/cli.py
-drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-15 01:21:10.244842 ficture-0.0.1.post3/ficture/loaders/
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/loaders/__init__.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10709 2023-11-04 03:08:20.000000 ficture-0.0.1.post3/ficture/loaders/data_loader.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     3552 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/loaders/pixel_factor_loader.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    12509 2023-11-04 03:08:30.000000 ficture-0.0.1.post3/ficture/loaders/pixel_loader.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     8647 2023-11-04 03:08:41.000000 ficture-0.0.1.post3/ficture/loaders/pixel_to_unit_loader.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     6999 2023-11-04 03:08:47.000000 ficture-0.0.1.post3/ficture/loaders/read_chunk_fn.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     5361 2023-11-04 03:08:51.000000 ficture-0.0.1.post3/ficture/loaders/unit_loader.py
-drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-15 01:21:10.320834 ficture-0.0.1.post3/ficture/models/
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/models/__init__.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2442 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/models/lda_minibatch.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10183 2023-11-04 03:09:00.000000 ficture-0.0.1.post3/ficture/models/online_lda.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    13713 2023-11-04 03:09:03.000000 ficture-0.0.1.post3/ficture/models/online_penalized_lda.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10376 2023-11-04 03:09:10.000000 ficture-0.0.1.post3/ficture/models/online_slda.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2350 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/models/slda_minibatch.py
-drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-15 01:21:10.450530 ficture-0.0.1.post3/ficture/scripts/
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      212 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/scripts/__init__.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     5350 2023-11-04 03:09:19.000000 ficture-0.0.1.post3/ficture/scripts/choose_color.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     5150 2023-11-04 03:09:22.000000 ficture-0.0.1.post3/ficture/scripts/de_bulk.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     8446 2023-11-04 03:09:25.000000 ficture-0.0.1.post3/ficture/scripts/factor_report.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     2442 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/scripts/factor_report.template.html
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     4713 2023-11-04 03:09:30.000000 ficture-0.0.1.post3/ficture/scripts/filter_boundary.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     7201 2023-11-04 03:09:33.000000 ficture-0.0.1.post3/ficture/scripts/filter_density.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    19527 2023-11-06 06:13:39.000000 ficture-0.0.1.post3/ficture/scripts/lda_univ.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     7686 2023-11-06 05:37:38.000000 ficture-0.0.1.post3/ficture/scripts/make_dge_univ.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     6860 2023-11-15 00:47:49.000000 ficture-0.0.1.post3/ficture/scripts/make_spatial_minibatch.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    10949 2023-11-04 03:09:46.000000 ficture-0.0.1.post3/ficture/scripts/plot_base.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     3467 2023-11-06 03:27:43.000000 ficture-0.0.1.post3/ficture/scripts/plot_pixel_full.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     5642 2023-11-04 03:09:56.000000 ficture-0.0.1.post3/ficture/scripts/plot_pixel_multi.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     4124 2023-11-04 03:09:59.000000 ficture-0.0.1.post3/ficture/scripts/plot_pixel_single.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     7767 2023-11-04 03:10:02.000000 ficture-0.0.1.post3/ficture/scripts/slda_decode.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     5862 2023-11-04 03:10:11.000000 ficture-0.0.1.post3/ficture/scripts/transform_univ.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     6137 2023-11-04 03:10:05.000000 ficture-0.0.1.post3/ficture/scripts/transform_univ_unit.py
-drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-15 01:21:10.522057 ficture-0.0.1.post3/ficture/utils/
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/utils/__init__.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     3195 2023-11-04 03:10:28.000000 ficture-0.0.1.post3/ficture/utils/filter_fn.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1127 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/utils/hexagon_fn.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)    11956 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/utils/image_fn.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1447 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/utils/layout_fn.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     3647 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/utils/mds_color_circle.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     8794 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/utils/utilt.py
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     5580 2023-11-04 03:02:24.000000 ficture-0.0.1.post3/ficture/utils/visualize_factors.py
-drwxrws---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        0 2023-11-15 01:21:10.187916 ficture-0.0.1.post3/ficture.egg-info/
--rwxrwxr--   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1705 2023-11-15 01:21:09.000000 ficture-0.0.1.post3/ficture.egg-info/PKG-INFO
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)     1513 2023-11-15 01:21:10.000000 ficture-0.0.1.post3/ficture.egg-info/SOURCES.txt
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        1 2023-11-15 01:21:10.000000 ficture-0.0.1.post3/ficture.egg-info/dependency_links.txt
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       45 2023-11-15 01:21:10.000000 ficture-0.0.1.post3/ficture.egg-info/entry_points.txt
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      127 2023-11-15 01:21:10.000000 ficture-0.0.1.post3/ficture.egg-info/requires.txt
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)        8 2023-11-15 01:21:10.000000 ficture-0.0.1.post3/ficture.egg-info/top_level.txt
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      842 2023-11-15 01:20:56.000000 ficture-0.0.1.post3/pyproject.toml
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)      268 2023-11-15 01:21:10.544585 ficture-0.0.1.post3/setup.cfg
--rwxrwx---   0 ycsi     (99507095) sph-hmkang-turbo (2455996)       38 2023-11-04 04:37:40.000000 ficture-0.0.1.post3/setup.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.804289 ficture-0.0.2/
+-rw-r--r--   0 bluebear   (501) staff       (20)    19347 2024-04-04 10:02:06.000000 ficture-0.0.2/LICENSE
+-rw-r--r--   0 bluebear   (501) staff       (20)       57 2024-04-04 13:57:26.000000 ficture-0.0.2/MANIFEST.in
+-rw-r--r--   0 bluebear   (501) staff       (20)     1846 2024-04-04 13:58:05.804216 ficture-0.0.2/PKG-INFO
+-rw-r--r--   0 bluebear   (501) staff       (20)     1058 2024-04-04 07:30:11.000000 ficture-0.0.2/README.md
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.787746 ficture-0.0.2/ficture/
+-rw-r--r--   0 bluebear   (501) staff       (20)      263 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     1562 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/cli.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.789446 ficture-0.0.2/ficture/loaders/
+-rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10715 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/data_loader.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     4077 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/pixel_factor_loader.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    12685 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/pixel_loader.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10013 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/pixel_to_unit_loader.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     7907 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/loaders/unit_loader.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.790153 ficture-0.0.2/ficture/models/
+-rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2442 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/lda_minibatch.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    28506 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/online_lda.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10460 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/online_slda.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2350 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/models/slda_minibatch.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.792728 ficture-0.0.2/ficture/scripts/
+-rw-r--r--   0 bluebear   (501) staff       (20)      212 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     6411 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/choose_color.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     5394 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/de_bulk.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10343 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/factor_report.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2442 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/factor_report.template.html
+-rw-r--r--   0 bluebear   (501) staff       (20)     4738 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/filter_boundary.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     7726 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/filter_density.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    10560 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/filter_poly.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    11914 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/init_model_selection.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    12193 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/lda_univ.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     9058 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/make_dge_univ.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     7437 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/make_spatial_minibatch.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    11623 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_base.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    11866 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_hexagon.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     7246 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_pixel_full.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     6782 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_pixel_multi.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     4698 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/plot_pixel_single.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     9333 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/slda_decode.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     8932 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/scripts/transform_univ.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.793869 ficture-0.0.2/ficture/utils/
+-rw-r--r--   0 bluebear   (501) staff       (20)        0 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/__init__.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     4501 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/filter_fn.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     2123 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/hexagon_fn.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    11956 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/image_fn.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     1447 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/layout_fn.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     3767 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/mds_color_circle.py
+-rw-r--r--   0 bluebear   (501) staff       (20)    14775 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/utilt.py
+-rw-r--r--   0 bluebear   (501) staff       (20)     5885 2024-04-04 13:57:26.000000 ficture-0.0.2/ficture/utils/visualize_factors.py
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.803974 ficture-0.0.2/ficture.egg-info/
+-rw-r--r--   0 bluebear   (501) staff       (20)     1846 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/PKG-INFO
+-rw-r--r--   0 bluebear   (501) staff       (20)     1923 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/SOURCES.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)        1 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/dependency_links.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)       45 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/entry_points.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)      127 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/requires.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)        8 2024-04-04 13:58:05.000000 ficture-0.0.2/ficture.egg-info/top_level.txt
+drwxr-xr-x   0 bluebear   (501) staff       (20)        0 2024-04-04 13:58:05.803756 ficture-0.0.2/info/
+-rw-r--r--   0 bluebear   (501) staff       (20)   743896 2024-03-20 18:43:57.000000 ficture-0.0.2/info/Homo_sapiens.GRCh38.107.names.tsv.gz
+-rw-r--r--   0 bluebear   (501) staff       (20)   953535 2024-03-20 18:43:57.000000 ficture-0.0.2/info/Mus_musculus.GRCm38.102.names.tsv.gz
+-rw-r--r--   0 bluebear   (501) staff       (20)   957882 2024-03-20 18:43:57.000000 ficture-0.0.2/info/Mus_musculus.GRCm39.107.names.tsv.gz
+-rw-r--r--   0 bluebear   (501) staff       (20)   323108 2024-03-20 18:43:57.000000 ficture-0.0.2/info/gencode.human.mouse.combined.gene.types.tsv.gz
+-rw-r--r--   0 bluebear   (501) staff       (20)   356994 2024-03-20 18:43:57.000000 ficture-0.0.2/info/gencode.human.mouse.combined.gene_names.clean.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)       40 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.half_right.coordinate_minmax.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)       43 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.l1.half_right.coordinate_minmax.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)       40 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.l2.half_right.coordinate_minmax.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)     1518 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.layout.tsv
+-rw-r--r--   0 bluebear   (501) staff       (20)      320 2024-03-20 18:43:57.000000 ficture-0.0.2/info/hiseq.tile_list.txt
+-rw-r--r--   0 bluebear   (501) staff       (20)      840 2024-04-04 13:57:26.000000 ficture-0.0.2/pyproject.toml
+-rw-r--r--   0 bluebear   (501) staff       (20)      268 2024-04-04 13:58:05.804528 ficture-0.0.2/setup.cfg
+-rw-r--r--   0 bluebear   (501) staff       (20)       38 2024-04-04 13:57:26.000000 ficture-0.0.2/setup.py
```

### Comparing `ficture-0.0.1.post3/LICENSE` & `ficture-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ficture-0.0.1.post3/ficture/cli.py` & `ficture-0.0.2/ficture/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import sys, logging, importlib
 
 def main():
 
     # MAYBE.. should change legacy file names to match callable module names
     module_map = {\
-        "filter_by_density": "filter_density", \
+        "filter_by_density": "filter_poly", \
+        # "filter_by_density_v1": "filter_density", \
         "filter_by_boundary": "filter_boundary", \
         "make_spatial_minibatch": "make_spatial_minibatch",\
         "make_dge": "make_dge_univ", \
-        "lda": "lda_univ", \
+        "fit_model": "init_model_selection", \
+        # "lda": "lda_univ", \
         "transform": "transform_univ", \
         "choose_color": "choose_color", \
         "plot_base": "plot_base", \
         "de_bulk": "de_bulk", \
         "factor_report": "factor_report", \
         "slda_decode": "slda_decode", \
+
+        "plot_base": "plot_base", \
+        "plot_hexagon": "plot_hexagon", \
         "plot_pixel_multi": "plot_pixel_multi", \
         "plot_pixel_full": "plot_pixel_full", \
         "plot_pixel_single": "plot_pixel_single", \
-        }
+    }
 
     if len(sys.argv) < 2:
         print("Usage: ficture <command> <args>, ficture <command> -h to see arguments for each command")
         print("Available commands:\n"+"\t".join(list(module_map.keys()) ))
         return
     elif sys.argv[1] not in module_map:
         print("Unknown command: "+sys.argv[1])
```

### Comparing `ficture-0.0.1.post3/ficture/loaders/data_loader.py` & `ficture-0.0.2/ficture/loaders/data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,38 +206,38 @@
             chunk.rename(inplace=True, \
                          columns = {self._unit_id:'j', self._feature_id:'gene'})
             # Incomplete left over
             last_indx = chunk.j.iloc[-1]
             left = copy.copy(chunk[chunk.j.eq(last_indx)])
             chunk = chunk.loc[~chunk.j.eq(last_indx), :]
 
-            ct = chunk.groupby(by = ['j']).agg({self._key: sum}).reset_index()
+            ct = chunk.groupby(by = ['j']).agg({self._key: "sum"}).reset_index()
             kept_unit = set(ct.loc[ct[self._key] > self._min_c, "j"].values)
             self.df = pd.concat([self.df, chunk[chunk.j.isin(kept_unit)]])
             if len(self.df.j.unique()) < self._min_n: # Wait until more data
                 self.df = pd.concat([self.df, left])
                 continue
 
             # Total molecule count per unit
-            brc = self.df.groupby(by = ['j']).agg({self._key: sum}).reset_index()
+            brc = self.df.groupby(by = ['j']).agg({self._key: "sum"}).reset_index()
             brc = brc[brc[self._key] > self._min_c]
             brc.index = range(brc.shape[0])
             self.df = self.df[self.df.j.isin(brc.j.values)]
             # Make DGE
             barcode_kept = list(brc.j.values)
             bc_dict = {x:i for i,x in enumerate( barcode_kept ) }
             indx_row = [ bc_dict[x] for x in self.df['j']]
             indx_col = [ self.ft_dict[x] for x in self.df['gene']]
             N = len(barcode_kept)
             mtx = coo_array((self.df[self._key].values, (indx_row, indx_col)), shape=(N, self.M)).tocsr()
             yield mtx
             self.df = copy.copy(left)
 
         if len(self.df.j.unique()) > 1:
-            brc = self.df.groupby(by = ['j']).agg({self._key: sum}).reset_index()
+            brc = self.df.groupby(by = ['j']).agg({self._key: "sum"}).reset_index()
             brc = brc[brc[self._key] > self._min_c]
             brc.index = range(brc.shape[0])
             self.df = self.df[self.df.j.isin(brc.j.values)]
             # Make DGE
             barcode_kept = list(brc.j.values)
             bc_dict = {x:i for i,x in enumerate( barcode_kept ) }
             indx_row = [ bc_dict[x] for x in self.df['j']]
```

### Comparing `ficture-0.0.1.post3/ficture/loaders/pixel_factor_loader.py` & `ficture-0.0.2/ficture/loaders/pixel_factor_loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import sys, os, gzip, copy, re, logging, warnings
 import numpy as np
 import pandas as pd
 import subprocess as sp
 
 class BlockIndexedLoader:
 
-    def __init__(self, input, xmin = -np.inf, xmax = np.inf, ymin = -np.inf, ymax = np.inf, full = False) -> None:
+    def __init__(self, input, xmin = -np.inf, xmax = np.inf, ymin = -np.inf, ymax = np.inf, full = False, offseted = True, filter_cmd = "", idtype={}, chunksize=1000000) -> None:
         self.meta = {}
+        self.header = []
         nheader = 0
         with gzip.open(input, 'rt') as rf:
             for line in rf:
                 if line[0] != "#":
                     break
                 nheader += 1
                 if line[:2] == "##":
@@ -20,58 +21,67 @@
                         if v[1].lstrip('-+').isdigit():
                             self.meta[v[0]] = int(v[1])
                         elif v[1].replace('.','',1).lstrip('-+').isdigit():
                             self.meta[v[0]] = float(v[1])
                         else:
                             self.meta[v[0]] = v[1]
                 else:
-                    header = line[(line.rfind("#")+1):].strip().split('\t')
+                    self.header = line[(line.rfind("#")+1):].strip().split('\t')
+        logging.basicConfig(level= getattr(logging, "INFO", None), format='%(asctime)s %(message)s', datefmt='%I:%M:%S %p')
         logging.info("Read header %s", self.meta)
 
+        if np.isinf(xmin) and np.isinf(xmax) and np.isinf(ymin) and np.isinf(ymax):
+            full = True
+        self.xmin = xmin if offseted else xmin - self.meta['OFFSET_X']
+        self.xmax = xmax if offseted else xmax - self.meta['OFFSET_X']
+        self.ymin = ymin if offseted else ymin - self.meta['OFFSET_Y']
+        self.ymax = ymax if offseted else ymax - self.meta['OFFSET_Y']
         # Input reader
-        self.kheader = ['K'+str(k+1) for k in range(self.meta['TOPK'])]
-        self.pheader = ['P'+str(k+1) for k in range(self.meta['TOPK'])]
         dty={'BLOCK':str, 'X':int, 'Y':int}
-        dty.update({x : str for x in self.kheader})
-        dty.update({x : np.float16 for x in self.pheader})
+        if 'TOPK' in self.meta:
+            dty.update({f"K{k+1}" : str for k in range(self.meta['TOPK']) })
+            dty.update({f"P{k+1}" : float for k in range(self.meta['TOPK']) })
+        if len(idtype) > 0:
+            dty.update(idtype)
         self.file_is_open = True
-        if full or np.isfinite(xmin) or np.isfinite(xmax):
-            self.reader = pd.read_csv(input,sep='\t',skiprows=nheader,chunksize=1000000,names=header, dtype=dty)
+        self.xmin = max(xmin, 0)
+        self.xmax = min(xmax, self.meta["SIZE_X"])
+        self.ymin = max(ymin, 0)
+        self.ymax = min(ymax, self.meta["SIZE_Y"])
+        if full:
+            self.reader = pd.read_csv(input,sep='\t',skiprows=nheader,chunksize=chunksize,names=self.header, dtype=dty)
         else:
             # Translate target region to index
-            block = [int(x / self.meta['BLOCK_SIZE']) for x in [xmin, xmax - 1] ]
-            pos_range = [int((x - self.meta['OFFSET_Y'])*self.meta['SCALE']) for x in [ymin, ymax]]
+            block = [int(x / self.meta['BLOCK_SIZE']) for x in [self.xmin, self.xmax - 1] ]
+            pos_range = [int(x*self.meta['SCALE']) for x in [self.ymin, self.ymax]]
             if self.meta['BLOCK_AXIS'] == "Y":
-                block = [int(x / self.meta['BLOCK_SIZE']) for x in [ymin, ymax - 1] ]
-                pos_range = [int((x - self.meta['OFFSET_X'])*self.meta['SCALE']) for x in [xmin, xmax]]
+                block = [int(x / self.meta['BLOCK_SIZE']) for x in [self.ymin, self.ymax - 1] ]
+                pos_range = [int(x*self.meta['SCALE']) for x in [self.xmin, self.xmax]]
             block = np.arange(block[0], block[1]+1) * self.meta['BLOCK_SIZE']
             query = []
             pos_range = '-'.join([str(x) for x in pos_range])
             for i,b in enumerate(block):
                 query.append( str(b)+':'+pos_range )
 
-            cmd = ["tabix", input]+query
-            process = sp.Popen(cmd, stdout=sp.PIPE, stderr=sp.STDOUT)
-            self.reader = pd.read_csv(process.stdout,sep='\t',chunksize=1000000,names=header, dtype=dty)
-            logging.info(" ".join(cmd))
-
-        self.xmin = max(xmin, self.meta['OFFSET_X'])
-        self.xmax = min(xmax, self.meta['OFFSET_X'] + self.meta["SIZE_X"])
-        self.ymin = max(ymin, self.meta['OFFSET_Y'])
-        self.ymax = min(ymax, self.meta['OFFSET_Y'] + self.meta["SIZE_Y"])
+            cmd = " ".join( ["tabix", input] + query )
+            if filter_cmd != "":
+                cmd = cmd + " | " + filter_cmd
+            logging.info(cmd)
+            process = sp.Popen(cmd, stdout=sp.PIPE, stderr=sp.STDOUT, shell=True)
+            self.reader = pd.read_csv(process.stdout,sep='\t',chunksize=chunksize,names=self.header, dtype=dty)
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if not self.file_is_open:
             raise StopIteration
         try:
             chunk = next(self.reader)
         except StopIteration:
             self.file_is_open = False
             raise StopIteration
-        chunk['X']=chunk.X/self.meta['SCALE']+self.meta['OFFSET_X']
-        chunk['Y']=chunk.Y/self.meta['SCALE']+self.meta['OFFSET_Y']
+        chunk['X']=chunk.X/self.meta['SCALE']
+        chunk['Y']=chunk.Y/self.meta['SCALE']
         drop_index = chunk.index[(chunk.X<self.xmin)|(chunk.X>self.xmax)|\
                                  (chunk.Y<self.ymin)|(chunk.Y>self.ymax)]
         return chunk.drop(index=drop_index)
```

### Comparing `ficture-0.0.1.post3/ficture/loaders/pixel_loader.py` & `ficture-0.0.2/ficture/loaders/pixel_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ### Read a batched pixel file, construct slda minibatch
 
-import sys, os, gzip, copy, re
+import sys, os, gzip, copy, re, logging
 import numpy as np
 import pandas as pd
 
 from scipy.sparse import coo_array
 import sklearn.neighbors
 import sklearn.preprocessing
 from joblib.parallel import Parallel, delayed
+from sklearn.decomposition._online_lda_fast import _dirichlet_expectation_2d
 
-sys.path.append(os.path.dirname(os.path.abspath(__file__)))
 from ficture.utils import utilt
 from ficture.models.slda_minibatch import minibatch
 
 class PixelMinibatch:
 
     def __init__(self, reader, ft_dict, batch_id, key, mu_scale, radius, halflife, adj_penal=-1, precision=0.1, thread=1, verbose=0) -> None:
         self.df_full = pd.DataFrame()
@@ -66,15 +66,15 @@
             except StopIteration:
                 self.file_is_open = False
                 break
             chunk = chunk.loc[chunk.gene.isin(self.ft_dict) & \
                               (chunk[self.key] > 0), :]
             chunk.X = (chunk.X * self.mu_scale / self.precision).astype(int)
             chunk.Y = (chunk.Y * self.mu_scale / self.precision).astype(int)
-            chunk = chunk.groupby(by=[self.batch_id,"gene","X","Y"]).agg({self.key:np.sum}).reset_index()
+            chunk = chunk.groupby(by=[self.batch_id,"gene","X","Y"]).agg({self.key: "sum"}).reset_index()
             random_pref = chunk[self.batch_id].map(lambda x : x[-5:]).values
             chunk['j'] = random_pref + '_' + chunk.X.astype(str) + '_' + chunk.Y.astype(str)
             chunk.X *= self.precision
             chunk.Y *= self.precision
             # Keep pixels close enough to at least one anchor
             pts = chunk[["j", "X", "Y"]].drop_duplicates(subset="j")
             dist, indx = self.ref.query(X = np.array(pts[['X','Y']]), k = 1, return_distance = True)
@@ -82,29 +82,29 @@
 
             kept_pixel = dist < self.radius
             if np.sum(kept_pixel) == 0:
                 continue
             chunk = chunk.loc[chunk.j.isin(pts.loc[kept_pixel, 'j'].values), :]
             batch_ids.update(set(chunk[self.batch_id].unique()))
             self.df_full = pd.concat([self.df_full, chunk], axis=0)
-            # print(f"Read {len(batch_ids)} minibatches")
+            # logging.info(f"Read {len(batch_ids)} minibatches")
 
         left = pd.DataFrame()
         if self.file_is_open:
             last_indx = self.df_full[self.batch_id].iloc[-1]
             left = copy.copy(self.df_full.loc[self.df_full[self.batch_id].eq(last_indx), :])
             self.df_full = self.df_full.loc[~self.df_full[self.batch_id].eq(last_indx), :]
 
         ### Process chunk of data
         self.batch_index = list(self.df_full[self.batch_id].unique() )
         self.brc = self.df_full[[self.batch_id,"j","X","Y"]].drop_duplicates(subset=["j"])
         self.N0 = self.brc.shape[0]
         self.brc.index = range(self.N0)
-        self.df_full = self.df_full.groupby(by = [self.batch_id, "j", "gene"]).agg({self.key:sum}).reset_index()
-        print(f"Read {self.N0} pixels, forming {len(self.batch_index)} batches.")
+        self.df_full = self.df_full.groupby(by = [self.batch_id, "j", "gene"]).agg({self.key:"sum"}).reset_index()
+        logging.info(f"Read {self.N0} pixels, forming {len(self.batch_index)} batches.")
         self.bt = sklearn.neighbors.BallTree(np.asarray(self.brc[['X','Y']]))
         # Make DGE
         barcode_kept = list(self.brc['j'])
         bc_dict = {x:i for i,x in enumerate( barcode_kept ) }
         indx_row = [ bc_dict[x] for x in self.df_full['j']]
         indx_col = [ self.ft_dict[x] for x in self.df_full['gene']]
         self.dge_mtx = coo_array((self.df_full[self.key], (indx_row, indx_col)), shape=(self.N0, self.M)).tocsr()
@@ -127,16 +127,16 @@
         # Initilize anchor
         theta = np.array(self.grid_info.loc[grid_indx, self.factor_header])
         theta = sklearn.preprocessing.normalize(np.clip(theta, init_bound, 1.-init_bound), norm='l1', axis=1)
         n = theta.shape[0]
 
         # Pixel to anchor weight
         indx, dist = self.bt.query_radius(X = np.array(grid_pt), r = self.radius, return_distance = True)
-        r_indx = [i for i,x in enumerate(indx) for y in range(len(x))]
-        c_indx = [x for y in indx for x in y]
+        r_indx = [i for i,x in enumerate(indx) for y in range(len(x))] # anchor
+        c_indx = [x for y in indx for x in y] # pixel
         wij = np.array([x for y in dist for x in y])
         wij = 1-(wij / self.radius)**self.nu
         wij = coo_array((wij, (r_indx,c_indx)),shape=(n,self.N0)).tocsc().T
         wij.eliminate_zeros()
         nchoice=(wij != 0).sum(axis = 1)
         b_indx = np.arange(self.N0)[nchoice > 0]
         wij = wij[b_indx, :]
@@ -150,46 +150,48 @@
         post_count = np.zeros((self.K, self.M))
         for b in batch_index:
             b_indx, grid_pt, wij, theta = self._prepare_batch(b, init_bound)
             if b_indx is None:
                 continue
             N = len(b_indx)
             grid_pt = np.array(grid_pt)
+            x_min, y_min = grid_pt.min(axis = 0)
+            x_max, y_max = grid_pt.max(axis = 0)
             psi_org = sklearn.preprocessing.normalize(wij, norm='l1', axis=1)
             batch = minibatch()
             batch.init_from_matrix(self.dge_mtx[b_indx, :], grid_pt, wij, psi = psi_org, m_gamma = theta)
             _ = slda.do_e_step(batch)
 
-            tmp = self.brc.iloc[b_indx, :]
-            x_min, x_max = tmp.X.min(), tmp.X.max()
-            y_min, y_max = tmp.Y.min(), tmp.Y.max()
-            v = np.arange(N)[(tmp.X > x_min+self.out_buff) &\
-                             (tmp.X < x_max-self.out_buff) &\
-                             (tmp.Y > y_min+self.out_buff) &\
-                             (tmp.Y < y_max-self.out_buff)]
-            post_count += batch.phi[v, :].T @ batch.mtx[v, :]
-
             tmp = copy.copy(self.brc.loc[b_indx, ['j','X','Y']] )
             tmp.index = range(tmp.shape[0])
             tmp = pd.concat([tmp, pd.DataFrame(batch.phi, \
                              columns = self.factor_header)], axis = 1)
-            tmp = tmp.iloc[v, :]
+            if self.file_is_open:
+                v = np.arange(N)[(tmp.X > x_min+self.out_buff) &\
+                                (tmp.X < x_max-self.out_buff) &\
+                                (tmp.Y > y_min+self.out_buff) &\
+                                (tmp.Y < y_max-self.out_buff)]
+                post_count += batch.phi[v, :].T @ batch.mtx[v, :]
+                tmp = tmp.iloc[v, :]
+            else:
+                post_count += batch.phi.T @ batch.mtx
             pixel_result = pd.concat([pixel_result, tmp], axis = 0)
 
-            expElog_theta = np.exp(utilt.dirichlet_expectation(batch.gamma))
+            expElog_theta = np.exp(_dirichlet_expectation_2d(batch.gamma))
             expElog_theta/= expElog_theta.sum(axis = 1).reshape((-1, 1))
             tmp = pd.DataFrame({'minibatch':b,'X':grid_pt[:,0],'Y':grid_pt[:,1]})
             asum = batch.psi.T @ batch.mtx.sum(axis = 1).reshape((-1, 1))
             tmp['avg_size'] = np.array(asum).reshape(-1)
             for v in range(self.K):
                 tmp[str(v)] = expElog_theta[:, v]
-            tmp = tmp.loc[(tmp.X > x_min+self.out_buff) & \
-                          (tmp.X < x_max-self.out_buff) & \
-                          (tmp.Y > y_min+self.out_buff) & \
-                          (tmp.Y < y_max-self.out_buff), :]
+            if self.file_is_open:
+                tmp = tmp.loc[(tmp.X > x_min+self.out_buff) & \
+                            (tmp.X < x_max-self.out_buff) & \
+                            (tmp.Y > y_min+self.out_buff) & \
+                            (tmp.Y < y_max-self.out_buff), :]
             anchor_result = pd.concat([anchor_result, tmp], axis = 0)
         return post_count, pixel_result, anchor_result
 
     def run_chunk(self, slda, init_bound):
         if self.thread > 1:
             idx_slices = [[ self.batch_index[x] for x in y ] for y in utilt.gen_even_slices(len(self.batch_index), self.thread)]
             with Parallel( n_jobs=self.thread, backend='threading', verbose=self.verbose) as parallel:
@@ -239,15 +241,15 @@
             tmp = copy.copy(self.brc.loc[b_indx, ['j','X','Y']] )
             tmp.index = range(tmp.shape[0])
             tmp = pd.concat([tmp, pd.DataFrame(batch.phi, \
                              columns = self.factor_header)], axis = 1)
             tmp = tmp.iloc[v, :]
             pixel_result = pd.concat([pixel_result, tmp], axis = 0)
 
-            expElog_theta = np.exp(utilt.dirichlet_expectation(batch.gamma))
+            expElog_theta = np.exp(_dirichlet_expectation_2d(batch.gamma))
             expElog_theta/= expElog_theta.sum(axis = 1).reshape((-1, 1))
             tmp = pd.DataFrame({'minibatch':b,'X':grid_pt[:,0],'Y':grid_pt[:,1]})
             asum = batch.psi.T @ batch.mtx.sum(axis = 1).reshape((-1, 1))
             tmp['avg_size'] = np.array(asum).reshape(-1)
             for v in range(self.K):
                 tmp[str(v)] = expElog_theta[:, v]
             tmp = tmp.loc[(tmp.X > x_min+self.out_buff) & \
```

### Comparing `ficture-0.0.1.post3/ficture/loaders/pixel_to_unit_loader.py` & `ficture-0.0.2/ficture/loaders/pixel_to_unit_loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pandas as pd
 from scipy.sparse import coo_array, vstack
 
 from ficture.utils.hexagon_fn import *
 
 class PixelToUnit:
 
-    def __init__(self, reader, ft_dict, key, radius, scale=1, region_id=None, min_ct_per_unit=1, sliding_step=1, major_axis=None) -> None:
+    def __init__(self, reader, ft_dict, key, radius, scale=1, region_id=None, min_ct_per_unit=1, sliding_step=1, major_axis=None, xy_lattice=False) -> None:
         self.reader = reader
         self.ft_dict = ft_dict
         self.M = len(self.ft_dict)
         self.key = key
         self.radius = radius
         self.file_is_open = True
         self.min_ct_per_unit = min_ct_per_unit
@@ -26,14 +26,17 @@
         self.n_move = sliding_step
         self.Y = major_axis
         self.mj = self.Y if self.Y is not None else 'X'
         self.mi = 'X' if self.mj == 'Y' else 'Y'
         self.df = pd.DataFrame()
         self.brc = None
         self.mtx = None
+        self.lattice = xy_lattice
+        self.n_batch = 0
+        self.bound = self.radius * np.sqrt(3)/2
 
     def read_chunk(self, min_size = 200):
         if not self.file_is_open:
             return 0
         if self.region_id is None:
             return self._read_chunk_consecutive(min_size)
         else:
@@ -89,29 +92,38 @@
         self.df['hex_id'] = ''
         self.brc = pd.DataFrame()
         self.mtx = coo_array(([], ([], [])), shape = (0, self.M))
         for reg in region_list:
             indx = self.df[self.region_id].eq(reg)
             for offs_x in range(self.n_move):
                 for offs_y in range(self.n_move):
+                    offs_iden = str(offs_x) + '_' + str(offs_y)
                     x, y = pixel_to_hex(self.df.loc[indx, ['X', 'Y']].values, self.radius, offs_x/self.n_move, offs_y/self.n_move)
                     self.df.loc[indx, "hex_id"] = list(zip(x, y))
-                    ct = self.df[indx].groupby('hex_id').agg({self.key: sum}).reset_index()
-                    ct = ct[ct[self.key] >= self.min_ct_per_unit]
-                    kept_unit = ct.hex_id.values
-                    ct['hex_id'] = ct.hex_id.map(lambda x : '_'.join([str(u) for u in x]))
-                    if len(kept_unit) < 1:
+                    ct = self.df[indx].groupby('hex_id').agg({self.key: "sum"}).reset_index()
+                    ct.drop(index = ct.index[ct[self.key] < self.min_ct_per_unit], inplace=True)
+                    if len(ct) < 1:
                         continue
-                    bt_dict = {x:i for i,x in enumerate(kept_unit)}
+                    bt_dict = {x:i for i,x in enumerate(ct.hex_id.values)}
                     N = len(bt_dict)
-                    sub = self.df[indx & self.df.hex_id.isin(bt_dict)].groupby(by = ['hex_id', 'gene']).agg({self.key: sum}).reset_index()
-                    self.mtx = vstack([self.mtx, coo_array((sub[self.key].values, (sub.hex_id.map(bt_dict).values, sub.gene.map(self.ft_dict).values) ), shape = (N, self.M))])
-                    ct['x'], ct['y'] = hex_to_pixel([v[0] for v in kept_unit],\
-                                        [v[1] for v in kept_unit],\
-                                self.radius, offs_x/self.n_move, offs_y/self.n_move)
+                    brc = self.df[indx & self.df.hex_id.isin(bt_dict)].groupby(by = ['hex_id', 'gene']).agg({self.key: "sum"}).reset_index()
+                    self.mtx = vstack([self.mtx, coo_array((brc[self.key].values, (brc.hex_id.map(bt_dict).values, brc.gene.map(self.ft_dict).values) ), shape = (N, self.M))])
+                    if self.lattice:
+                        ct['x'], ct['y'] = \
+                            hex_to_pixel([v[0] for v in ct.hex_id.values],\
+                                         [v[1] for v in ct.hex_id.values],\
+                            self.radius, offs_x/self.n_move, offs_y/self.n_move)
+                    else:
+                        ct = brc.groupby(by = ['hex_id']).agg({self.key: sum,\
+                            'X': np.median, 'Y':np.median}).reset_index()
+                        ct.rename(columns = {'X':'x', 'Y':'y'}, inplace=True)
+                    ct.index = ct.hex_id.map(bt_dict)
+                    ct.sort_index(inplace=True)
+                    ct['hex_id'] = ct.hex_id.map(lambda x : '_'.join([str(u) for u in x]))
+                    ct.hex_id = offs_iden + '_' + ct.hex_id.values
                     ct[self.region_id] = reg
                     self.brc = pd.concat([self.brc, ct])
         self.mtx = self.mtx.tocsr()
         self.df = left
         self.brc.index = range(self.brc.shape[0])
         return self.brc.shape[0]
 
@@ -120,56 +132,65 @@
         if not self.file_is_open:
             return -1
         mj_range = [-np.inf, np.inf]
         mi_range = [-np.inf, np.inf]
         mj_size = 0
         mi_size = 0
         if len(self.df) > 0:
-            mj_range = [self.df[self.mj].max(), self.df[self.mj].min()]
+            mj_range = [self.df[self.mj].iloc[-1], self.df[self.mj].iloc[0]]
             mi_range = [self.df[self.mi].max(), self.df[self.mi].min()]
             mj_size = mj_range[0] - mj_range[1]
             mi_size = mi_range[0] - mi_range[1]
         while mj_size < min_size or mi_size < min_size:
             try:
                 chunk = next(self.reader)
             except StopIteration:
                 self.file_is_open = False
                 break
             chunk = chunk[chunk.gene.isin(self.ft_dict)]
             chunk.X = chunk.X.astype(float) * self.scale
             chunk.Y = chunk.Y.astype(float) * self.scale
-            mj_range[0] = max(mj_range[0], chunk[self.mj].max())
-            mj_range[1] = min(mj_range[1], chunk[self.mj].min())
+            mj_range[0] = chunk[self.mj].iloc[-1]
+            mj_range[1] = min(mj_range[1], chunk[self.mj].iloc[0])
             mi_range[0] = max(mi_range[0], chunk[self.mi].max())
             mi_range[1] = min(mi_range[1], chunk[self.mi].min())
             mj_size = mj_range[0] - mj_range[1]
             mi_size = mi_range[0] - mi_range[1]
             self.df = pd.concat([self.df, chunk])
         self.df['hex_id'] = ''
         self.brc = pd.DataFrame()
         self.mtx = coo_array(([], ([], [])), shape = (0, self.M))
         for offs_x in range(self.n_move):
             for offs_y in range(self.n_move):
+                offs_iden = str(offs_x) + '_' + str(offs_y)
                 x, y = pixel_to_hex(self.df[['X', 'Y']].values, self.radius, offs_x/self.n_move, offs_y/self.n_move)
                 self.df.hex_id = list(zip(x, y))
-                ct = self.df.groupby('hex_id').agg({self.key: sum}).reset_index()
-                ct = ct[ct[self.key] >= self.min_ct_per_unit]
-                kept_unit = ct.hex_id.values
-                ct['hex_id'] = ct.hex_id.map(lambda x : '_'.join([str(u) for u in x]))
-                if len(kept_unit) < 1:
+                ct = self.df.groupby('hex_id').agg({self.key: "sum"}).reset_index()
+                ct['X'], ct['Y'] = \
+                        hex_to_pixel([v[0] for v in ct.hex_id.values],\
+                                     [v[1] for v in ct.hex_id.values],\
+                        self.radius, offs_x/self.n_move, offs_y/self.n_move)
+                # Drop hexagons with centers within sqrt(3)*raidus/2 from each boundary
+                ct.drop(index = ct.index[\
+                    (ct[self.mj].lt(mj_range[1] + self.bound) ) | \
+                    (ct[self.mj].gt(mj_range[0] - self.bound) ) ], inplace=True)
+                ct.drop(index = ct.index[ct[self.key] < self.min_ct_per_unit], inplace=True)
+                if len(ct) < 1:
                     continue
-                bt_dict = {x:i for i,x in enumerate(kept_unit)}
+                bt_dict = {x:i for i,x in enumerate(ct.hex_id.values)}
                 N = len(bt_dict)
-                sub = self.df[self.df.hex_id.isin(bt_dict)].groupby(by = ['hex_id', 'gene']).agg({self.key: sum}).reset_index()
-                self.mtx = vstack([self.mtx, coo_array((sub[self.key].values, (sub.hex_id.map(bt_dict).values, sub.gene.map(self.ft_dict).values) ), shape = (N, self.M))])
-                ct['x'], ct['y'] = hex_to_pixel([v[0] for v in kept_unit],\
-                                    [v[1] for v in kept_unit],\
-                            self.radius, offs_x/self.n_move, offs_y/self.n_move)
+                brc = self.df[self.df.hex_id.isin(bt_dict)].groupby(by = ['hex_id', 'gene']).agg({self.key: "sum"}).reset_index()
+                self.mtx = vstack([self.mtx, coo_array((brc[self.key].values, (brc.hex_id.map(bt_dict).values, brc.gene.map(self.ft_dict).values) ), shape = (N, self.M))])
+                if not self.lattice:
+                    ct = brc.groupby(by = ['hex_id']).agg({self.key: sum, 'X': np.median, 'Y':np.median}).reset_index()
+                ct.rename(columns = {'X':'x', 'Y':'y'}, inplace=True)
+                ct.index = ct.hex_id.map(bt_dict)
+                ct.sort_index(inplace=True)
+                ct['hex_id'] = ct.hex_id.map(lambda x : '_'.join([str(u) for u in x]))
+                ct.hex_id = offs_iden + '_' + ct.hex_id.values
                 self.brc = pd.concat([self.brc, ct])
-        if self.Y is not None:
-            self.df = self.df[self.df[self.mj] >= mj_range[0] - self.radius]
-            self.df.drop(columns = ['hex_id'], inplace = True)
-        else:
-            self.df = pd.DataFrame()
+        self.df = self.df[self.df[self.mj] >= mj_range[0] - 2 * self.radius]
+        self.df.drop(columns = ['hex_id'], inplace = True)
         self.mtx = self.mtx.tocsr()
         self.brc.index = range(self.brc.shape[0])
+        self.n_batch += 1
         return self.brc.shape[0]
```

### Comparing `ficture-0.0.1.post3/ficture/models/lda_minibatch.py` & `ficture-0.0.2/ficture/models/lda_minibatch.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.1.post3/ficture/models/online_lda.py` & `ficture-0.0.2/ficture/models/online_slda.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,223 +1,217 @@
-# Functions for fitting Latent Dirichlet Allocation
-# with online variational Bayes (VB)
-# following Hoffman et al. 2010
+# Functions for fitting augmented Latent Dirichlet Allocation
+# with online variational Bayes (VB).
+
+import sys, io, os, re, time, copy, subprocess, logging
 
-import sys, io, os, re, time, copy, warnings
 import numpy as np
+from sklearn.utils import check_random_state
 from scipy.special import gammaln, psi, logsumexp, expit, logit
-from scipy.sparse import issparse
+from scipy.sparse import *
 from sklearn.preprocessing import normalize
-from joblib.parallel import Parallel, delayed
-
-# Add directory
-from ficture.utils import utilt
+from sklearn.decomposition._online_lda_fast import (
+    _dirichlet_expectation_1d, _dirichlet_expectation_2d,
+)
 
 class OnlineLDA:
     """
-    Implements online VB for LDA as described in Hoffman et al. 2010.
+    Implements online VB for LDA as described in (Hoffman et al. 2010).
     """
-    def __init__(self, vocab, K, N, alpha = None, eta = None, tau0=9, kappa=.7, iter_inner = 50, tol = 1e-4, verbose = 0, thread = 1):
+    def __init__(self, vocab, K, N, alpha = None, eta = None, tau0=9, kappa=.7, zeta = 0, iter_inner = 50, tol = 1e-4, iter_gamma = 10, verbose = 0, seed = None):
         """
         Arguments:
+        K: Number of topics
         vocab: A list of features
-        K:     Number of topics
-        N:     Estimated total number of units
-        alpha: Hyperparameter for the prior on theta
-        eta:   Hyperparameter for prior on beta
+        D:     Total number of pixels in the entire dataset.
+        alpha: Hyperparameter for the prior on weight vectors theta
+        eta:   Hyperparameter for prior on topics beta
         tau0:  A (non-negative) learning parameter that downweights earl iterations
         kappa: Learning rate (exponential decay), should be between
                (0.5, 1.0] to guarantee asymptotic convergence.
+        --- Experimental ---
+        zeta:  Weight of the proximal contamination penalty
+        iter_gamma: Maximum number of iterations when maximizing the "penalized ELBO" w.r.t. gamma (there is no analytical solution)
         """
         self._vocab = vocab
         self._K = K
         self._M = len(self._vocab)
         self._N = N
         self._tau0 = tau0 + 1
         self._kappa = kappa
+        self._zeta = zeta
         self._updatect = 0
         self._max_iter_inner = iter_inner
+        self._max_iter_gamma = iter_gamma
         self._tol = tol
-        self._eps = 1e-16
         self._verbose = verbose
-        self._thread = thread
         self._Elog_beta = None      # K x M
         self._lambda = None         # K x M
-        self._expElog_beta = None   # K x M
-        self._sstats = None         # K x M
+        self.rng_ = check_random_state(seed)
 
-        self._alpha = alpha # Factor weight prior
+        self._alpha = alpha # 1D array
         if self._alpha is None:
             self._alpha = np.ones(self._K)/self._K
         elif np.isscalar(self._alpha):
             self._alpha = np.ones(self._K)*self._alpha
-        elif len(self._alpha.shape) == 1:
-            assert self._alpha.shape[0] == self._K, "Invalid alpha"
         else:
-            warnings.warn("Invalid alpha, fall back to default uniform 1/K")
-            self._alpha = np.ones(self._K)/self._K
+            self._alpha = self._alpha.reshape(-1)
+            assert self._alpha.shape[0] == self._K, "Invalid alpha"
 
-        self._eta = eta  # Expression profile prior
+        self._eta = eta     # 1D array
         if self._eta is None:
             self._eta = (np.ones(self._M)/self._K).reshape((1,-1))
         elif np.isscalar(self._eta):
             self._eta = (np.ones(self._M)*self._eta).reshape((1,-1))
-        elif len(self._eta.shape) == 1:
-            self._eta = np.array(self._eta).reshape((1, -1))
-            assert self._eta.shape[1] == self._M, "Invalid eta"
-        elif len(self._eta.shape) == 2:
-            assert self._eta.shape == (self._K, self._M), "Invalid eta"
         else:
-            warnings.warn("Invalid eta, fall back to default uniform 1/K")
-            self._eta = (np.ones(self._M)/self._K).reshape((1,-1))
+            self._eta = self._eta.reshape((1, -1))
+            assert self._eta.shape[1] == self._M, "Invalid eta"
 
-    def init_global_parameter(self, _lambda=None):
+    def init_global_parameter(self, m_lambda=None):
         # Initialize the variational distribution q(beta|lambda)
-        if _lambda is None:
-            self._lambda = np.random.gamma(100., 1./100., (self._K, self._M))
+        if m_lambda is None:
+            self._lambda = self.rng_.gamma(100., 1./100., (self._K, self._M))
         else:
-            self._lambda = _lambda
-            assert self._lambda.shape == (self._K, self._M), "Invalid lambda"
-        if self._lambda.min() <= 0 :
-            warnings.warn("Parameters must be positive, will clip to 1/10 the min nonzero value")
-            pseudo = self._lambda[self._lambda > 0].min()/10
-            self._lambda = np.clip(self._lambda, pseudo, None)
-        self._Elog_beta = utilt.dirichlet_expectation(self._lambda)
-        self._expElog_beta = np.exp(self._Elog_beta)
-
-
-    def _update_gamma(self, X, _gamma, alpha):
-        gamma = copy.copy(_gamma)
-        sstats = np.zeros((self._K, self._M))
-        expElog_theta = np.exp(utilt.dirichlet_expectation(gamma))
-        for j in range(X.shape[0]):
-            maxchange = self._tol + 1
-            it = 0
-            while it < self._max_iter_inner and maxchange > self._tol:
-                old_gamma = copy.copy(gamma[j, :])
-                phi_norm = expElog_theta[j, :] @ self._expElog_beta + self._eps # 1 x M
-                gamma[j, :] = alpha[j, :] +\
-                    np.multiply(expElog_theta[j, :], \
-                                (X[[j], :].multiply(1./phi_norm)) @ self._expElog_beta.T) # 1 x K
-                expElog_theta[j, :] = np.exp(utilt.dirichlet_expectation(gamma[j, :]))
-                maxchange = np.abs(old_gamma/old_gamma.sum() - gamma[j, :]/gamma[j, :].sum()).max()
-                it += 1
-                if self._verbose > 2 or (self._verbose > 1 and it % 10 == 0):
-                    print(f"E-step, {j}-th unit, update gamma: {it}-th iteration, max change {maxchange:.4f}")
-            phi_norm = expElog_theta[j, :] @ self._expElog_beta + self._eps
-            phi = expElog_theta[j, :].reshape((-1, 1)) * self._expElog_beta / phi_norm.reshape((1, -1)) # K x M
-            sstats += np.multiply(X[[j], :].toarray(), phi)
-        return sstats, gamma
-
+            self._lambda = m_lambda
+        self._Elog_beta = _dirichlet_expectation_2d(self._lambda)
 
     def do_e_step(self, batch):
         """
         Update local parameters, compute sufficient stats for M step
         """
+        Xb = batch.mtx @ self._Elog_beta.T         # Dense, N x K
+        if issparse(Xb):
+            Xb = Xb.toarray()
+        c_indx, r_indx = batch.psi.nonzero()
         # Initialize the variational distribution q(theta|gamma)
         if batch.alpha is None:
             batch.alpha = np.broadcast_to(self._alpha, (batch.n, self._K))
         if batch.gamma is None:
-            batch.gamma = np.random.gamma(100., 1./100., (batch.n, self._K))
+            batch.gamma = copy.copy(batch.alpha)
+        gamma_old = copy.copy(batch.gamma)
+        Elog_theta = _dirichlet_expectation_2d(batch.gamma) # n x K
+        meanchange = self._tol + 1
+        it = 0
+
+        while it < self._max_iter_inner and meanchange > self._tol:
+
+            batch.phi = batch.psi @ Elog_theta + Xb
+            batch.phi = np.exp(batch.phi -\
+                               logsumexp(batch.phi, axis = 1).reshape((-1, 1)) )
+            psi_hat = batch.phi[c_indx, 0] * Elog_theta[r_indx, 0] # \sum_k phi_ik Elog[theta_jk]
+            for k in range(1, self._K):
+                psi_hat += batch.phi[c_indx, k] * Elog_theta[r_indx, k]
+            psi_hat += np.multiply(Xb, batch.phi).sum(axis = 1).reshape(-1)[c_indx] # \sum_k phi_ik log Pik
+            batch.psi.data = psi_hat
+            batch.psi += batch.ElogO
+            batch.psi.data = np.exp(batch.psi.data)
+            batch.psi = normalize(batch.psi, norm='l1', axis=1)
+            batch.gamma = batch.alpha + batch.psi.T @ batch.phi
+            Elog_theta = _dirichlet_expectation_2d(batch.gamma)
+
+            meanchange = np.abs(batch.gamma - gamma_old).max(axis=1).mean()
+            gamma_old = copy.copy(batch.gamma)
+            it += 1
+            # if self._verbose > 2: # debug
+            #     print( np.around([batch.psi.sum(axis = 1).min(),\
+            #                       batch.phi.sum(axis = 1).min()], 2) )
+            if self._verbose > 2 or (self._verbose > 1 and it % 10 == 0):
+                logging.info(f"E-step, update phi, psi, gamma: {it}-th iteration, mean change {meanchange:.4f}")
+
+        sstats = batch.phi.T @ batch.mtx # K x M
+        batch.ll = batch.psi.T @ batch.mtx @ self._Elog_beta.T
+        ll_norm = logsumexp(batch.ll, axis = 1)
+        ll_tot = 0
+        for k in range(self._K):
+            ll_tot += (batch.ll[:, k] - ll_norm).sum()
+        batch.ll = ll_tot / batch.n
+        return sstats
+
+    def update_lambda_penalized(self, batch):
+        assert self._zeta > 0 and self._zeta < 1, "zeta must be in (0, 1) for penalized update"
+        assert batch.anchor_adj is not None, "batch.anchor_adj must be provided for penalized update"
+        if issparse(batch.anchor_adj):
+            assert (batch.anchor_adj.diagonal() > 0).sum() >= batch.n, "anchor_adj must contain self-loops"
+        else:
+            assert (np.diag(batch.anchor_adj) > 0).sum() >= batch.n, "anchor_adj must contain self-loops"
+        # E step to update gamma, phi | lambda for mini-batch
+        lambda_org = self._eta + self.do_e_step(batch) # K X M
+        theta = normalize(batch.gamma, norm='l1', axis=1) # n x K, E[theta]
+        ckl = theta.T @ normalize(batch.anchor_adj, norm='l1', axis=1) @ theta
+        ckl /= theta.sum(axis = 0).reshape((-1, 1)) # K x K, factor spatial proximity
+        np.fill_diagonal(ckl, 0)
+        lam_sum = lambda_org.sum(axis = 1)
+        it = 0
+        meanchange = self._tol + 1
+        while it < self._max_iter_gamma and meanchange > self._tol:
+            lambda_new = np.zeros((self._K, self._M))
+            for k in range(self._K):
+                avg = ckl[[k], :] @ (normalize(lambda_org, norm='l1', axis=1)*lam_sum[k])
+                adj = np.clip(lambda_org[k, :] - self._zeta * avg, 0, None)
+                lambda_new[k, :] = adj / adj.sum() * lam_sum[k]
+            v = np.abs(lambda_new - lambda_org).max(axis = 1) / lambda_org.sum(axis = 1)
+            meanchange = v.mean()
+            if self._verbose > 2 or (self._verbose > 1 and it % 10 == 0) or (self._verbose > 1 and it == self._max_iter_gamma - 1):
+                logging.info(f"Penalized M-step, update lambda : {it}-th iteration, mean max change {meanchange:.4f}")
+            lambda_org = copy.copy(lambda_new)
+            it += 1
 
-        # Run E-step in parallel
-        if self._thread <= 1:
-            self._sstats, batch.gamma = self._update_gamma(batch.mtx, batch.gamma, batch.alpha)
-        else:
-            idx_slices = [idx for idx in utilt.gen_even_slices(batch.n, self._thread)]
-            with Parallel(n_jobs=self._thread, verbose=max(0, self._verbose - 1)) as parallel:
-                result = parallel(delayed(self._update_gamma)(batch.mtx[idx, :], batch.gamma[idx, :], batch.alpha[idx, :])
-                for idx in idx_slices)
-            # Collect sufficient statistics
-            self._sstats = np.zeros((self._K, self._M))
-            for i, v in enumerate(result):
-                self._sstats += v[0]
-                batch.gamma[idx_slices[i], :] = v[1]
-
-        batch.ll = np.multiply(normalize(batch.gamma, norm='l1', axis=1), batch.mtx @ self._Elog_beta.T).sum() / batch.n
-        return
+        if self._verbose > 0:
+            # Estimate likelihood for current values of lambda.
+            scores = self.approx_score(batch)
+            logging.info(f"{self._updatect}-th global update. Scores: " + ", ".join(['%.2e'%x for x in scores]))
 
+        rhot = pow(self._tau0 + self._updatect, -self._kappa)
+        self._lambda = (1-rhot) * self._lambda + \
+                       rhot * ((self._N / batch.N) * lambda_org)
+        self._Elog_beta = _dirichlet_expectation_2d(self._lambda)
+        self._updatect += 1
+        return 1
 
     def update_lambda(self, batch):
         """
         Process one minibatch
         """
         # rhot will be between 0 and 1, and says how much to weight
         # the information we got from this mini-batch.
 
-        # E step to update gamma | lambda for mini-batch
-        self.do_e_step(batch)
-
+        # E step to update gamma, phi | lambda for mini-batch
+        sstats = self.do_e_step(batch)
         # Estimate likelihood for current values of lambda.
         scores = self.approx_score(batch)
         if self._verbose > 0:
-            print(f"{self._updatect}-th global update. Scores: " + ", ".join(['%.2e'%x for x in scores]))
+            logging.info(f"{self._updatect}-th global update. Scores: " + ", ".join(['%.2e'%x for x in scores]))
 
-        # Update global parameters
         rhot = pow(self._tau0 + self._updatect, -self._kappa)
-        doc_ratio = float(self._N) / batch.n
         self._lambda = (1-rhot) * self._lambda + \
-                       rhot * (doc_ratio * (self._eta + self._sstats) )
-        self._Elog_beta = utilt.dirichlet_expectation(self._lambda)
-        self._expElog_beta = np.exp(self._Elog_beta)
+                       rhot * ((self._N / batch.N) * (self._eta + sstats) )
+        self._Elog_beta = _dirichlet_expectation_2d(self._lambda)
         self._updatect += 1
         return scores
 
-
-    def transform(self, X, gamma = None, alpha = None):
-        assert X.shape[1] == self._M
-        if issparse(X):
-            X = X.tocsr()
-        n = X.shape[0]
-        if gamma is None:
-            gamma = np.random.gamma(100., 1./100., (n, self._K))
-        if alpha is None:
-            alpha = np.broadcast_to(self._alpha, (n, self._K))
-        else:
-            if len(alpha.shape) == 1:
-                alpha = np.broadcast_to(alpha, (n, self._K))
-            else:
-                assert alpha.shape == (n, self._K), "Invalid alpha input"
-        # Run E-step in parallel
-        if self._thread <= 1:
-            _, gamma = self._update_gamma(X, gamma, alpha)
-        else:
-            idx_slices = [idx for idx in utilt.gen_even_slices(n, self._thread)]
-            with Parallel(n_jobs=self._thread, verbose=max(0, self._verbose - 1)) as parallel:
-                result = parallel(delayed(self._update_gamma)(X[idx, :], gamma[idx, :], alpha[idx, :])
-                for idx in idx_slices)
-            for i, v in enumerate(result):
-                gamma[idx_slices[i], :] = v[1]
-        gamma = normalize(gamma, norm='l1', axis=1)
-        return gamma
-
-
     def approx_score(self, batch):
-        """
-        ELBO
-        """
+
         score_gamma = 0
         score_beta  = 0
-        Elog_theta = utilt.dirichlet_expectation(batch.gamma)
-        E_theta = normalize(batch.gamma, norm='l1', axis=1)
+        Elog_theta = _dirichlet_expectation_2d(batch.gamma)
 
-        # E[log p(x | theta, beta)]
-        score_unit = batch.mtx @ self._Elog_beta.T
-        score_unit = np.multiply(E_theta, score_unit/batch.n).sum()
+        # E[log p(x | theta, phi, beta)]
+        score_pixel = batch.mtx @ self._Elog_beta.T
+        score_pixel = np.multiply(batch.phi, score_pixel/batch.N).sum()
+        score_patch = batch.ll
 
         # E[log p(theta | alpha) - log q(theta | gamma)]
         score_gamma += np.sum((batch.alpha - batch.gamma)*Elog_theta)
         score_gamma += np.sum(gammaln(batch.gamma)) - np.sum(gammaln(np.sum(batch.gamma, 1)))
         score_gamma /= batch.n
 
         # E[log p(beta | eta) - log q (beta | lambda)]
         score_beta += np.sum((self._eta-self._lambda)*self._Elog_beta)
         score_beta += np.sum(gammaln(self._lambda)) - np.sum(gammaln(np.sum(self._lambda, 1)))
 
-        return((score_unit, score_gamma, score_beta, self._N * (score_unit+score_gamma) + score_beta))
+        return((score_pixel, score_patch, score_gamma, score_beta, self._N * (score_patch+score_gamma) + score_beta))
 
     def coherence_pmi(self, pw, pseudo_ct = 200, top_gene_n = 100):
         """
         Topic coherence (pointwise mutual information)
         """
         topic_pmi = []
         top_gene_n = np.min([top_gene_n, self._M])
```

### Comparing `ficture-0.0.1.post3/ficture/models/slda_minibatch.py` & `ficture-0.0.2/ficture/models/slda_minibatch.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.1.post3/ficture/scripts/choose_color.py` & `ficture-0.0.2/ficture/scripts/choose_color.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,48 @@
 import sys, os, copy, gc, re, gzip, pickle, argparse, logging, warnings
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 import sklearn.neighbors
 from scipy.sparse import coo_array
+from datetime import datetime
 
 from ficture.utils.utilt import plot_colortable
 from ficture.utils.mds_color_circle import assign_color_mds_circle
 
 def choose_color(_args):
 
-    parser = argparse.ArgumentParser(prog="choose_color")
+    parser = argparse.ArgumentParser()
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', type=str, help='')
     parser.add_argument('--cmap_name', type=str, default="turbo", help="Name of Matplotlib colormap to use (better close to a circular colormap)")
     parser.add_argument('--top_color', type=str, default="#fcd217", help="HEX color code for the top factor")
     parser.add_argument('--even_space', action='store_true', help="Evenly space the factors on the circle")
+    parser.add_argument('--annotation', type=str, default = '', help='')
+    parser.add_argument('--seed', type=int, default=-1, help='')
     args = parser.parse_args(_args)
 
+    if len(_args) == 0:
+        parser.print_help()
+        return
+
+    ## obtain seed if not provided
+    seed = args.seed
+    if seed <= 0:
+        seed = int(datetime.now().timestamp()) % 2147483648
+    np.random.seed(seed)
+
+    factor_name = {}
+    if os.path.isfile(args.annotation):
+        with open(args.annotation) as f:
+            for line in f:
+                x = line.strip().split('\t')
+                factor_name[x[0]] = x[1]
+
     cmap_name = args.cmap_name
     if args.cmap_name not in plt.colormaps():
         cmap_name = "turbo"
 
     df = pd.read_csv(args.input, sep='\t', header=0)
     df.rename(columns = {"X":"x","Y":"y"},inplace=True)
     header = df.columns
@@ -37,14 +57,16 @@
     # Factor abundance (want top factors to have more distinct colors)
     if args.even_space:
         weight=None
     else:
         weight = df.loc[:, factor_header].sum(axis = 0).values
         weight = weight**(1/2)
         weight /= weight.sum()
+        weight = np.clip(weight, .2/K, 1)
+        weight /= weight.sum()
 
     # Find neearest neighbors
     bt = sklearn.neighbors.BallTree(df.loc[:, ["x", "y"]])
     dist, indx = bt.query(df.loc[:, ["x", "y"]], k = 7, return_distance=True)
     r_indx = np.array([i for i,v in enumerate(indx) for y in range(len(v))], dtype=int)
     c_indx = indx.reshape(-1)
     dist = dist.reshape(-1)
@@ -59,32 +81,40 @@
     # Translate into a symmetric dissimilarity measure
     # Large values in mtx indicate close proximity, to be mapped to distinct colors
     np.fill_diagonal(mtx, 0)
     mtx /= mtx.sum(axis = 1)
     mtx = mtx + mtx.T
 
     # Assign color using MDS with circular constraint
-    c_pos = assign_color_mds_circle(mtx, cmap_name, weight=weight, top_color=args.top_color)
+    c_pos = assign_color_mds_circle(mtx, cmap_name, weight=weight, top_color=args.top_color, seed=seed)
+    spectral_offset = .05 # avoid extremely dark colors
+    c_pos = (c_pos - c_pos.min()) / (c_pos.max() - c_pos.min()) * (1 - spectral_offset) + spectral_offset
 
     c_rank = np.argsort(np.argsort(c_pos))
     cmtx = plt.get_cmap(cmap_name)(c_pos) # K x 4
-    cdict = {k:cmtx[k,:] for k in range(K)}
-    df = pd.DataFrame({"Name":range(K), "Color_index":c_rank})
+    df = pd.DataFrame({"Name":np.arange(K).astype(str), "Color_index":c_rank})
     df = pd.concat([df, pd.DataFrame(cmtx[:, :3], columns=["R", "G", "B"])], axis=1)
+    cdict = {k:cmtx[k,:] for k in range(K)}
+    if len(factor_name) > 0:
+        df["Annotation"] = df.Name.map(factor_name)
+        cdict = {factor_name[str(k)]:cmtx[k,:] for k in range(K)}
 
     # Output RGB table
     f = args.output + ".rgb.tsv"
     df.to_csv(f, sep='\t', index=False)
 
     # Plot color bar
     fig = plot_colortable(cdict, "Factor label", sort_colors=False, ncols=4)
     f = args.output + ".cbar.png"
     fig.savefig(f, format="png", transparent=True)
 
 
+if __name__ == "__main__":
+    choose_color(sys.argv[1:])
+
 
 
 
 # ### zz - Previous approach
 
 # linear = MDS(n_components=1, dissimilarity="precomputed",normalized_stress='auto').fit_transform(mtx).squeeze()
 # c_order = np.argsort(linear)
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/de_bulk.py` & `ficture-0.0.2/ficture/scripts/de_bulk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ### Simple differential expression tests
 
-import sys, io, os, gzip, copy, re, time, pickle, argparse
+import sys, io, os, gzip, copy, re, time, argparse
 import numpy as np
 import pandas as pd
 import scipy.stats
 from scipy.sparse import *
 from joblib.parallel import Parallel, delayed
 
 from ficture.utils import utilt
@@ -17,56 +17,65 @@
     parser.add_argument('--feature', type=str, default='', help='')
     parser.add_argument('--feature_label', type=str, default = "gene", help='')
     parser.add_argument('--min_ct_per_feature', default=50, type=int, help='')
     parser.add_argument('--max_pval_output', default=1e-3, type=float, help='')
     parser.add_argument('--min_fold_output', default=1.5, type=float, help='')
     parser.add_argument('--min_output_per_factor', default=10, type=int, help='Even when there are no significant DE genes, output top genes for each factor')
     parser.add_argument('--thread', default=1, type=int, help='')
+    parser.add_argument('--use_input_header', action = 'store_true', help='')
     args = parser.parse_args(_args)
 
+    if len(_args) == 0:
+        parser.print_help()
+        return
+
     pcut=args.max_pval_output
     fcut=args.min_fold_output
     gene_kept = set()
     if os.path.exists(args.feature):
         feature = pd.read_csv(args.feature, sep='\t', header=0)
         gene_kept = set(feature[args.feature_label].values )
 
     # Read aggregated count table
     info = pd.read_csv(args.input,sep='\t',header=0)
     oheader = []
     header = []
-    for x in info.columns:
-        y = re.match('^[A-Za-z]*_*(\d+)$', x)
-        if y:
-            header.append(y.group(1))
-            oheader.append(x)
+    if args.use_input_header:
+        header = [x for x in info.columns if x != args.feature_label]
+        oheader = header
+    else:
+        for x in info.columns:
+            y = re.match('^[A-Za-z]*_*(\d+)$', x)
+            if y:
+                header.append(y.group(1))
+                oheader.append(x)
     K = len(header)
     M = info.shape[0]
     reheader = {oheader[k]:header[k] for k in range(K)}
     reheader[args.feature_label] = "gene"
     info.rename(columns = reheader, inplace=True)
     print(f"Read posterior count over {M} genes and {K} factors")
 
     if len(gene_kept) > 0:
         info = info.loc[info.gene.isin(gene_kept), :]
     info["gene_tot"] = info.loc[:, header].sum(axis=1).astype(int)
     info = info[info["gene_tot"] > args.min_ct_per_feature]
     info.index = info.gene.values
     total_umi = info.gene_tot.sum()
-    total_k = np.array(info.loc[:, [str(k) for k in range(K)]].sum(axis = 0) )
+    total_k = np.array(info.loc[:, header].sum(axis = 0) )
     M = info.shape[0]
 
     print(f"Testing {M} genes over {K} factors")
 
     def chisq(k,info,total_k,total_umi):
         res = []
         if total_k <= 0:
             return res
         for name, v in info.iterrows():
-            if v[str(k)] <= 0:
+            if v[k] <= 0:
                 continue
             tab=np.zeros((2,2))
             tab[0,0]=v[str(k)]
             tab[0,1]=v["gene_tot"]-tab[0,0]
             tab[1,0]=total_k-tab[0,0]
             tab[1,1]=total_umi-total_k-v["gene_tot"]+tab[0,0]
             fd=tab[0,0]/total_k/tab[0,1]*(total_umi-total_k)
@@ -75,47 +84,47 @@
             tab = np.around(tab, 0).astype(int) + 1
             chi2, p, dof, ex = scipy.stats.chi2_contingency(tab, correction=False)
             res.append([name,k,chi2,p,fd,v["gene_tot"]])
         return res
 
     res = []
     if args.thread > 1:
-        for k in range(K):
+        for k, kname in enumerate(header):
             idx_slices = [idx for idx in utilt.gen_even_slices(M, args.thread)]
             with Parallel(n_jobs=args.thread, verbose=0) as parallel:
-                result = parallel(delayed(chisq)(k, \
-                            info.iloc[idx, :].loc[:, [str(k), 'gene_tot']],\
+                result = parallel(delayed(chisq)(kname, \
+                            info.iloc[idx, :].loc[:, [kname, 'gene_tot']],\
                             total_k[k], total_umi) for idx in idx_slices)
             res += [item for sublist in result for item in sublist]
     else:
         for name, v in info.iterrows():
-            for k in range(K):
+            for k, kname in enumerate(header):
                 if total_k[k] <= 0 or v[str(k)] <= 0:
                     continue
                 tab=np.zeros((2,2))
-                tab[0,0]=v[str(k)]
+                tab[0,0]=v[kname]
                 tab[0,1]=v["gene_tot"]-tab[0,0]
                 tab[1,0]=total_k[k]-tab[0,0]
                 tab[1,1]=total_umi-total_k[k]-v["gene_tot"]+tab[0,0]
                 fd=tab[0,0]/total_k[k]/tab[0,1]*(total_umi-total_k[k])
                 if fd < 1:
                     continue
                 tab = np.around(tab, 0).astype(int) + 1
                 chi2, p, dof, ex = scipy.stats.chi2_contingency(tab, correction=False)
-                res.append([name,k,chi2,p,fd,v["gene_tot"]])
+                res.append([name,kname,chi2,p,fd,v["gene_tot"]])
 
     chidf=pd.DataFrame(res,columns=['gene','factor','Chi2','pval','FoldChange','gene_total'])
-    chidf.sort_values(by=['factor','Chi2'],ascending=[True,False],inplace=True)
-    chidf['Rank'] = 0
-    for k in range(K):
-        chidf.loc[chidf.factor.eq(k), 'Rank'] = np.arange((chidf.factor==k).sum())
+    chidf["Rank"] = chidf.groupby(by = "factor")["Chi2"].rank(ascending=False)
     chidf = chidf.loc[((chidf.pval<pcut)&(chidf.FoldChange>fcut)) | (chidf.Rank < args.min_output_per_factor), :]
-    chidf.sort_values(by=['factor','Chi2'],ascending=[True,False])
+    chidf.sort_values(by=['factor','Chi2'],ascending=[True,False],inplace=True)
     chidf.Chi2 = chidf.Chi2.map(lambda x : "{:.1f}".format(x) )
     chidf.FoldChange = chidf.FoldChange.map(lambda x : "{:.2f}".format(x) )
     chidf.gene_total = chidf.gene_total.astype(int)
     chidf.drop(columns = 'Rank', inplace=True)
 
     outpath=os.path.dirname(args.output)
     if not os.path.exists(outpath):
         os.makedirs(outpath)
     chidf.to_csv(args.output,sep='\t',float_format="%.2e",index=False)
+
+if __name__ == "__main__":
+    de_bulk(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/factor_report.py` & `ficture-0.0.2/ficture/scripts/factor_report.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,137 +1,178 @@
 import sys, os, copy, gc, re, gzip, pickle, argparse, logging, warnings
 import numpy as np
 import pandas as pd
 import matplotlib.colors
 from jinja2 import Environment, FileSystemLoader
+from importlib import resources as impresources
 
+import ficture.scripts
 from ficture.utils.visualize_factors import visual_hc, image_to_base64
 
 def factor_report(_args):
 
     parser = argparse.ArgumentParser(prog="factor_report")
     parser.add_argument('--path', type=str, help='')
     parser.add_argument('--pref', type=str, help='')
     parser.add_argument('--model_id', type=str, default='', help='')
     parser.add_argument('--color_table', type=str, default='', help='')
     parser.add_argument('--n_top_gene', type=int, default=20, help='')
     parser.add_argument('--min_top_gene', type=int, default=10, help='')
     parser.add_argument('--max_pval', type=float, default=0.001, help='')
     parser.add_argument('--min_fc', type=float, default=1.5, help='')
     parser.add_argument('--output_pref', type=str, default='', help='')
+    parser.add_argument('--annotation', type=str, default = '', help='')
 
     parser.add_argument('--hc_tree', action='store_true')
     parser.add_argument('--n_top_gene_on_tree', type=int, default=10, help='')
     parser.add_argument('--tree_figure', type=str, default='', help='')
     parser.add_argument('--cprob_cut', type=str, default='.99', help='Only visualize top factors with cumulative probability > cprob_cut')
     parser.add_argument('--model', type=str, default='', help='')
+    parser.add_argument('--anchor', type=str, default='', help='')
     parser.add_argument('--circle_if', type=int, default=24, help='')
     parser.add_argument('--remake_tree', action='store_true')
     parser.add_argument('--circle', action='store_true')
     parser.add_argument('--vertical', action='store_true')
     args = parser.parse_args(_args)
 
+    if len(_args) == 0:
+        parser.print_help()
+        return
+
     path=args.path
     pref=args.pref
     ntop = args.n_top_gene
     mtop = args.min_top_gene
     pval_max = args.max_pval
     fc_min = args.min_fc
-    ejs = os.path.join(os.path.dirname(__file__), "factor_report.template.html")
+    ejs = os.path.join(impresources.files(ficture.scripts), "factor_report.template.html")
     if not os.path.isfile(ejs):
         sys.exit(f"Template file {ejs} not found")
+
     if args.remake_tree or args.circle or args.vertical:
         args.hc_tree = True
 
     model_id = args.model_id
     if model_id == '':
         model_id = args.pref
 
     output_pref = args.output_pref
     if output_pref == '':
         output_pref = path+"/"+pref
 
     # Color code
     color_f = args.color_table
-    if os.path.isfile(args.color_table):
-        color_table = pd.read_csv(args.color_table, sep='\t')
-    else:
+    if not os.path.isfile(color_f):
         color_f = path+"/figure/"+model_id+".rgb.tsv"
-        color_table = pd.read_csv(color_f, sep='\t')
+    if not os.path.isfile(color_f):
+        sys.exit(f"Cannot find color table")
+    color_table = pd.read_csv(color_f, sep='\t')
     K = color_table.shape[0]
+    logging.info(f"Read color table from {color_f}")
+
     factor_header = np.arange(K).astype(str)
-    color_table.Name = color_table.Name.astype(int)
-    color_table.sort_values(by = 'Name', inplace=True)
-    color_table.index = color_table.Name.values
+    factor_name = {}
+    if os.path.isfile(args.annotation):
+        with open(args.annotation) as f:
+            for line in f:
+                x = line.strip().split('\t')
+                factor_name[x[0]] = x[1]
+                factor_header[int(x[0])] = x[1]
+
+    print(factor_header)
     color_table['RGB'] = [','.join(x) for x in np.clip((color_table.loc[:, ['R','G','B']].values * 255).astype(int), 0, 255).astype(str) ]
     color_table['HEX'] = [ matplotlib.colors.to_hex(v) for v in np.array(color_table.loc[:, ['R','G','B']]) ]
-    node_color = {str(i):v['HEX'] for i,v in color_table.iterrows() }
-
+    node_color = {factor_header[v['Name']]:v['HEX'] for i,v in color_table.iterrows() }
 
     # Posterior count
     f=path+"/"+pref+".posterior.count.tsv.gz"
     post = pd.read_csv(f, sep='\t')
+    logging.info(f"Read posterior count from {f}")
     recol = {}
     for u in post.columns:
         v = re.match('^[A-Za-z]*_*(\d+)$', u.strip())
         if v:
             recol[v.group(0)] = v.group(1)
-    post.rename(columns=recol, inplace=True)
+    if len(recol) == K:
+        post.rename(columns=recol, inplace=True)
+    for u in factor_header:
+        post[u] = post[u].astype(float)
     post_umi = post.loc[:, factor_header].sum(axis = 0).astype(int).values
-    post_weight = post.loc[:, factor_header].sum(axis = 0).values
+    post_weight = post.loc[:, factor_header].sum(axis = 0).values.astype(float)
     post_weight /= post_weight.sum()
 
     # DE genes
     f=path+"/DE/"+pref+".bulk_chisq.tsv"
-    de = pd.read_csv(f, sep='\t')
-    de.factor = de.factor.astype(int)
+    if not os.path.exists(f):
+        f=path+"/"+pref+".bulk_chisq.tsv"
+        if not os.path.exists(f):
+            sys.exit(f"Cannot find DE file")
+    de = pd.read_csv(f, sep='\t', dtype={'factor':str})
+    logging.info(f"Read DE genes from {f}")
+    # de.factor = de.factor.astype(int)
     top_gene = []
     top_gene_anno = []
     de['Rank'] = 0
     # Temporary: shorten unspliced gene names
     de.gene = de.gene.str.replace('unspl_', 'u_')
     # Top genes by Chi2
     de.sort_values(by=['factor','Chi2'],ascending=False,inplace=True)
-    for k in range(K):
-        v = de.loc[de.factor.eq(k), 'gene'].iloc[:args.n_top_gene_on_tree].values
+    de["Rank"] = de.groupby(by = "factor").Chi2.rank(ascending=False, method = "min").astype(int)
+    for k, kname in enumerate(factor_header):
+        indx = de.factor.eq(kname)
+        v = de.loc[indx, 'gene'].iloc[:args.n_top_gene_on_tree].values
         top_gene_anno.append(', '.join(v))
-        de.loc[de.factor.eq(k), 'Rank'] = np.arange(de.factor.eq(k).sum())
-        v = de.loc[de.factor.eq(k) & ( (de.Rank < mtop) | \
+        v = de.loc[indx & ( (de.Rank < mtop) | \
                 ((de.pval <= pval_max) & (de.FoldChange >= fc_min)) ), \
                 'gene'].iloc[:ntop].values
         if len(v) == 0:
-            top_gene.append([k, '.'])
+            top_gene.append([kname, '.'])
         else:
-            top_gene.append([k, ', '.join(v)])
+            top_gene.append([kname, ', '.join(v)])
     # Top genes by fold change
     de.sort_values(by=['factor','FoldChange'],ascending=False,inplace=True)
-    for k in range(K):
-        de.loc[de.factor.eq(k), 'Rank'] = np.arange(de.factor.eq(k).sum())
-        v = de.loc[de.factor.eq(k) & ( (de.Rank < mtop) | \
+    de["Rank"] = de.groupby(by = "factor").FoldChange.rank(ascending=False, method = "min").astype(int)
+    for k, kname in enumerate(factor_header):
+        indx = de.factor.eq(kname)
+        v = de.loc[indx & ( (de.Rank < mtop) | \
                 ((de.pval <= pval_max) & (de.FoldChange >= fc_min)) ), \
                 'gene'].iloc[:ntop].values
         if len(v) == 0:
             top_gene[k].append('.')
         else:
             top_gene[k].append(', '.join(v))
     # Top genes by absolute weight
-    for k in range(K):
-        v = post.gene.iloc[np.argsort(post.loc[:, str(k)].values)[::-1][:ntop] ].values
+    for k, kname in enumerate(factor_header):
+        if post_umi[k] < 10:
+            top_gene[k].append('.')
+            continue
+        v = post.gene.iloc[np.argsort(-post.loc[:, kname].values)[:ntop] ].values
         top_gene[k].append(', '.join(v))
 
     # Summary
-    table = pd.DataFrame({'Factor':np.arange(K), 'RGB':color_table.RGB.values,
+    table = pd.DataFrame({'Factor':factor_header, 'RGB':color_table.RGB.values,
                         'Weight':post_weight, 'PostUMI':post_umi,
                         'TopGene_pval':[x[1] for x in top_gene],
                         'TopGene_fc':[x[2] for x in top_gene],
                         'TopGene_weight':[x[3] for x in top_gene] })
+    oheader = ["Factor", "RGB", "Weight", "PostUMI", "TopGene_pval", "TopGene_fc", "TopGene_weight"]
+    # Anchor genes used for initialization if applicable
+    anchor_f = args.anchor
+    if not os.path.exists(anchor_f):
+        anchor_f = path + "/" + model_id + ".model_anchors.tsv"
+    if os.path.exists(anchor_f):
+        ak = pd.read_csv(anchor_f, sep='\t', names = ["Factor", "Anchors"], dtype={"Factor":str})
+        table = table.merge(ak, on = "Factor", how = "left")
+        oheader.insert(4, "Anchors")
+        logging.info(f"Read anchor genes from {anchor_f}")
+
     table.sort_values(by = 'Weight', ascending = False, inplace=True)
 
     f = output_pref+".factor.info.tsv"
-    table.to_csv(f, sep='\t', index=False, header=True, float_format="%.5f")
+    table.loc[table.PostUMI.ge(10), oheader].to_csv(f, sep='\t', index=False, header=True, float_format="%.5f")
 
     f = output_pref+".factor.info.tsv"
     with open(f, 'r') as rf:
         lines = rf.readlines()
     header = lines[0].strip().split('\t')
     rows = [ list(enumerate(row.strip().split('\t') )) for row in lines[1:]]
 
@@ -159,26 +200,27 @@
                 if not os.path.exists(args.model):
                     model_f = path + "/" + model_id + ".model_matrix.tsv.gz"
                 if not os.path.exists(model_f):
                     print("Cannot find model file, will cluster based on posterior count")
                     model = post
                 else:
                     model = pd.read_csv(model_f, sep='\t')
-                model_prob = np.array(model.iloc[:, 1:]).T + .1
+                # model_prob = np.array(model.iloc[:, 1:]).T + .1
+                model_prob = np.array(model.loc[:, factor_header]).T + .1
                 model_prob = model_prob / model_prob.sum(axis = 1).reshape((-1,1))
 
                 circle = args.circle
                 if not circle and args.circle_if > 0:
                     v = np.argsort(post_weight)[::-1]
                     w = np.cumsum(post_weight[v] )
                     k = np.arange(K)[w > cprob_cut][0]
                     if k > args.circle_if:
                         circle = True
                 tree = visual_hc(model_prob, post_weight, top_gene_anno, \
-                                node_color = node_color, circle = circle, \
+                                node_color = node_color, factor_name = factor_header, circle = circle, \
                                 output_f = tree_f, cprob_cut = cprob_cut)
         print(f"Tree figure path: {tree_f}")
         image_base64 = image_to_base64(tree_f)
 
         tree_alt = "Hierarchical clustering of factors based on pairwise coine distance"
         tree_caption = "Clustering of factors based on pairwise coine distance. Factors with high abundance jointly accounting for " + args.cprob_cut + " of observations are displayed."
 
@@ -186,7 +228,10 @@
     html_output = template.render(header=header, rows=rows, image_base64=image_base64, tree_image_alt=tree_alt, tree_image_caption=tree_caption)
 
     f=output_pref+".factor.info.html"
     with open(f, "w") as html_file:
         html_file.write(html_output)
 
     print(f)
+
+if __name__ == "__main__":
+    factor_report(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/factor_report.template.html` & `ficture-0.0.2/ficture/scripts/factor_report.template.html`

 * *Files identical despite different names*

### Comparing `ficture-0.0.1.post3/ficture/scripts/filter_boundary.py` & `ficture-0.0.2/ficture/scripts/filter_boundary.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     if os.path.exists(args.output):
         warnings.warn("Output file already exists")
     if not os.path.exists(args.input):
         sys.exit("Cannot find input file")
     if not os.path.exists(args.boundary):
         sys.exit("Cannot find input file")
 
-    # logging.basicConfig(level= getattr(logging, "INFO", None))
-    logger = logging.getLogger(__name__)
+    logging.basicConfig(level= getattr(logging, "INFO", None))
 
     if args.boundary.endswith('.geojson'):
         vertices = extract_polygons_from_json(args.boundary)
         vertices = [(x * args.boundary_unit_in_um + np.array([args.offset_x, args.offset_y])) for x in vertices]
         n_poly = len(vertices)
         poly_list = [shapely.polygons(x) for x in vertices]
         poly_list = [x if x.is_valid else x.buffer(0) for x in poly_list]
@@ -63,21 +62,21 @@
             print(verts.min(axis=0), verts.max(axis=0))
         n_poly = len(poly_list)
         poly_list = [x if x.is_valid else x.buffer(0) for x in poly_list]
         poly = shapely.unary_union(poly_list)
     else:
         sys.exit("Unknown boundary format")
 
-    logger.info(f"Read boundary info with {n_poly} polygons, total area {poly.area:.1f} um^2")
+    logging.info(f"Read boundary info with {n_poly} polygons, total area {poly.area:.1f} um^2")
 
     gene_kept = set()
     if os.path.exists(args.feature):
         feature = pd.read_csv(args.feature, sep='\t', header=0)
         gene_kept = set(feature.gene.values)
-        logger.info(f"Read feature info with {len(gene_kept)} genes")
+        logging.info(f"Read feature info with {len(gene_kept)} genes")
 
     with gzip.open(args.input, 'rt') as rf:
         header = rf.readline()
     if args.output.endswith('.gz'):
         with gzip.open(args.output, 'wt') as wf:
             _=wf.write(header)
     else:
@@ -97,11 +96,14 @@
         if args.transpose:
             pts = GeoSeries(map(Point, zip(chunk.Y.values / args.mu_scale,\
                                         chunk.X.values / args.mu_scale)))
         else:
             pts = GeoSeries(map(Point, zip(chunk.X.values / args.mu_scale,\
                                         chunk.Y.values / args.mu_scale)))
         chunk = chunk.loc[pts.within(poly).values, :]
-        logger.info(f"Output {chunk.shape[0]} rows ...")
+        logging.info(f"Output {chunk.shape[0]} rows ...")
         if chunk.shape[0] == 0:
             continue
         chunk.to_csv(args.output, mode='a', sep='\t', index=False, header=False)
+
+if __name__ == "__main__":
+    filter_by_boundary(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/filter_density.py` & `ficture-0.0.2/ficture/scripts/filter_density.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import sys, os, gzip, gc, argparse, warnings, logging
 import numpy as np
 import pandas as pd
 import sklearn.neighbors
 import sklearn.mixture
 
-# # Add parent directory
-# sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-# from hexagon_fn import *
-# from filter_fn import filter_by_density_mixture
-
 from ficture.utils.filter_fn import filter_by_density_mixture
 
-def filter_by_density(_args):
+def filter_by_density_v1(_args):
 
     parser = argparse.ArgumentParser(prog = "filter_by_density")
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', type=str, help='')
     parser.add_argument('--ref_pt', type=str, help='')
     parser.add_argument('--filter_based_on', type=str, default="Count", help='')
     parser.add_argument('--feature', type=str, default='', help='')
     parser.add_argument('--mu_scale', type=float, default=26.67, help='Coordinate to um translate')
-    parser.add_argument('--filter_batch_size', type=float, default=1000, help='In um, along the streaming axis')
-    parser.add_argument('--filter_batch_ncut', type=int, default=2, help='')
+    parser.add_argument('--filter_batch_size', type=float, default=5000, help='In um, along the streaming axis')
+    parser.add_argument('--filter_batch_ncut', type=int, default=1, help='')
     parser.add_argument('--major_axis', type=str, default="X", help='')
     parser.add_argument('--precision_um', type=float, default=2, help='')
+    parser.add_argument('--log', default = '', type=str, help='files to write log to')
     parser.add_argument('--max_npts_to_fit_model', type=float, default=1e6, help='')
+    parser.add_argument('--min_abs_mol_density_squm_dense', type=float, default=0.2, help='Lowerbound for dense tissue region')
     parser.add_argument('--min_abs_mol_density_squm', type=float, default=0.02, help='A safe lowerbound to remove very sparse technical noise')
     parser.add_argument('--hard_threshold', type=float, default=-1, help='If provided, filter by hard threshold (number of molecules per squared um)')
     parser.add_argument('--radius', type=float, default=7, help='')
     parser.add_argument('--hex_n_move', type=int, default=6, help='')
 
     parser.add_argument('--xmin', type=float, default=-1, help='In um')
     parser.add_argument('--xmax', type=float, default=np.inf, help='In um')
@@ -40,44 +37,50 @@
     parser.add_argument('--debug', action='store_true')
 
     args = parser.parse_args(_args)
     if len(_args) == 0:
         parser.print_help()
         return
 
-    logger = logging.getLogger(__name__)
-
     if os.path.exists(args.output):
         warnings.warn("Output file already exists")
     if not os.path.exists(args.input):
         sys.exit("Cannot find input file")
     major_axis = args.major_axis.upper()
     if major_axis not in ["X", "Y"]:
         sys.exit("Invalid --major_axis")
     minor_axis = "X" if major_axis == "Y" else "Y"
     if args.xmax <= 0:
         args.xmax = np.inf
     if args.ymax <= 0:
         args.ymax = np.inf
 
+    if args.log != '':
+        try:
+            logging.basicConfig(filename=args.log, filemode='a', encoding='utf-8', level=logging.INFO)
+        except:
+            logging.basicConfig(level= getattr(logging, "INFO", None))
+    else:
+        logging.basicConfig(level= getattr(logging, "INFO", None))
+
     key      = args.filter_based_on
     mu_scale = 1./args.mu_scale
     n_move   = args.hex_n_move
     radius   = args.radius
     hex_area = radius**2*3*np.sqrt(3)/2
     chunk_size = 1000000
 
     gene_kept = set()
     if os.path.exists(args.feature):
         feature = pd.read_csv(args.feature, sep='\t', header=0)
         gene_kept = set(feature.gene.values)
 
     if os.path.exists(args.ref_pt) and not args.redo_filter:
         pt = pd.read_csv(args.ref_pt, sep='\t')
-        logger.info(f"Read existing anchor points")
+        logging.info(f"Read existing anchor points")
     else:
         pt = pd.DataFrame()
         df=pd.DataFrame()
         for chunk in pd.read_csv(gzip.open(args.input, 'rb'),\
             sep='\t', usecols=["Y","X","gene",key], chunksize=chunk_size):
             full = chunk.shape[0] == chunk_size
             if len(gene_kept) != 0:
@@ -91,42 +94,44 @@
             if args.precision_um > 0:
                 chunk['X'] = np.around(chunk.X.values/args.precision_um,0).astype(int)*args.precision_um
                 chunk['Y'] = np.around(chunk.Y.values/args.precision_um,0).astype(int)*args.precision_um
             chunk = chunk.groupby(by = ["X", "Y"]).agg({key:sum}).reset_index()
             df = pd.concat([df, chunk])
             hst, hed = df[major_axis].iloc[0], df[major_axis].iloc[-1]
             wst, wed = df[minor_axis].min(), df[minor_axis].max()
-            logger.info(f"Current chunk size {hed-hst} x {wed-wst}, collapsed into {df.shape[0]} pts")
+            logging.info(f"Current chunk size {hed-hst} x {wed-wst}, collapsed into {df.shape[0]} pts")
 
             if hed - hst < args.filter_batch_size * .9 and full:
                 continue
 
             st = hst
             ed = st + args.filter_batch_size
             wstep = (wed - wst + 1) / args.filter_batch_ncut
             df['win'] = ((df[minor_axis] - wst)/wstep).astype(int).astype(str)
             ### Detect grid points falling inside dense tissue region
             for w in df.win.unique():
                 indx = df.win.eq(w)
+                xmin, ymin = df.loc[indx, ['X','Y']].min()
+                xmax, ymax = df.loc[indx, ['X','Y']].max()
                 sub, m0, m1 = filter_by_density_mixture(df.loc[indx, :], key, radius, n_move, args)
                 pt = pd.concat([pt, sub])
-                logger.info(f"Window {str(w)}:\t{m0:.3f} v.s. {m1:.3f}")
+                logging.info(f"Window {str(w)} ({xmax-xmin:.1f} X {ymax-ymin:.1f} ):\t{m0:.3f} v.s. {m1:.3f}")
             df=pd.DataFrame()
             if args.debug:
                 break
 
         if not args.debug:
             pt.x = np.around(np.clip(pt.x.values,0,np.inf)/args.precision_um,0).astype(int)
             pt.y = np.around(np.clip(pt.y.values,0,np.inf)/args.precision_um,0).astype(int)
             pt.drop_duplicates(inplace=True)
             pt.x = pt.x * args.precision_um
             pt.y = pt.y * args.precision_um
             pt.to_csv(args.ref_pt, sep='\t', index=False, header=True)
 
-        logger.info(f"Finished identifying anchor points in tissue region.")
+        logging.info(f"Finished identifying anchor points in tissue region.")
 
     if args.anchor_only:
         sys.exit()
 
 
     ref=sklearn.neighbors.BallTree(np.array(pt.loc[:, ['x','y']]))
     with gzip.open(args.input, 'rt') as rf:
@@ -152,11 +157,14 @@
             continue
         dv, iv = ref.query(X=np.array(chunk.loc[:, ["X","Y"]]) * mu_scale, \
                         k=1, return_distance=True, sort_results=False)
         dv = dv.squeeze()
         chunk = chunk.loc[dv < radius, :]
         if chunk.shape[0] == 0:
             continue
-        logger.info(f"Output {chunk.shape[0]} rows ...")
+        logging.info(f"Output {chunk.shape[0]} rows ...")
         chunk.to_csv(args.output, mode='a', sep='\t', index=False, header=False)
         if args.debug:
             break
+
+if __name__ == "__main__":
+    filter_by_density_v1(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/make_dge_univ.py` & `ficture-0.0.2/ficture/scripts/make_dge_univ.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 import sys, os, gzip, copy, gc, time, argparse, logging
 import numpy as np
 import pandas as pd
 from scipy.sparse import *
 import subprocess as sp
 import random as rng
+from collections import defaultdict
+import geojson
+import shapely.prepared, shapely.geometry
+from shapely.geometry import Point
 
 from ficture.utils.hexagon_fn import pixel_to_hex, hex_to_pixel
 
 def make_dge(_args):
 
     parser = argparse.ArgumentParser(prog = "make_dge")
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', type=str, help='')
+    parser.add_argument('--boundary', type=str, default = '', help='')
 
     parser.add_argument('--major_axis', type=str, default="Y", help='X or Y')
     parser.add_argument('--mu_scale', type=float, default=1, help='Coordinate to um translate')
 
     parser.add_argument('--count_header', nargs='*', type=str, default=["gn","gt", "spl","unspl","ambig"], help="Which columns correspond to UMI counts in the input")
     parser.add_argument('--group_within', nargs='*', type=str, default=[], help="Pixels are collapsed within each group. Separate by space if multiple identifier")
 
@@ -24,36 +29,41 @@
 
     parser.add_argument('--precision', type=int, default=1, help='Number of digits to store spatial location (in um), 0 for integer.')
 
     parser.add_argument('--n_move', type=int, default=3, help='')
     parser.add_argument('--hex_width', type=int, default=24, help='')
     parser.add_argument('--hex_radius', type=int, default=-1, help='')
     parser.add_argument('--min_ct_per_unit', type=int, default=20, help='')
+    parser.add_argument('--min_density_per_unit', type=float, default=0.2, help='')
 
     args = parser.parse_args(_args)
-    logger = logging.getLogger(__name__)
+    if len(_args) == 0:
+        parser.print_help()
+        return
 
     r_seed = time.time()
     rng.seed(r_seed)
-    logger.info(f"Random seed {r_seed}")
+    logging.basicConfig(level= getattr(logging, "INFO", None))
+    logging.info(f"Random seed {r_seed}")
     mj = args.major_axis
 
     # Input file and numerical columns to use as counts
     ct_header = args.count_header
     key = args.key
     if key not in ct_header:
         key = ct_header[0]
-        logger.warning(f"The designated major key is not one of the specified count columns, --key is ignored the first existing key is chosen")
-    if not os.path.exists(args.input):
+        logging.warning(f"The designated major key is not one of the specified count columns, --key is ignored the first existing key is chosen")
+    if not os.path.isfile(args.input):
         sys.exit(f"ERROR: cannot find input file \n {args.input}")
     with gzip.open(args.input, 'rt') as rf:
         input_header=rf.readline().strip().split('\t')
         ct_header = [v for v in input_header if v in ct_header]
         if len(ct_header) == 0:
             sys.exit("Input header does not contain the specified --count_header")
+    print(input_header)
     keep_header=['X','Y','j','Group'] + ct_header
     output_header = ["random_index",'X','Y','gene'] + ct_header + args.group_within
     with open(args.output,'w') as wf:
         _=wf.write('\t'.join(output_header)+'\n')
 
     # basic parameters
     random_index_max=sys.maxsize//100000
@@ -65,91 +75,110 @@
     if n_move > diam // 2:
         n_move = diam // 4
     ovlp_buffer = diam * 2
     if radius < 0:
         radius = diam / np.sqrt(3)
     else:
         diam = int(radius*np.sqrt(3))
+    area = radius * diam * 3 / 2
+    min_ct_per_unit = max(args.min_ct_per_unit, args.min_density_per_unit * area)
 
-    adt = {x:np.sum for x in ct_header}
+    adt = {x:"sum" for x in ct_header}
     dty = {x:int for x in ct_header}
     dty.update({x:str for x in ['X','Y','gene'] + args.group_within})
 
+    use_boundary = False
+    if os.path.isfile(args.boundary):
+        mpoly = shapely.geometry.shape(geojson.load(open(args.boundary, 'rb')))
+        mpoly = shapely.prepared.prep(mpoly)
+        use_boundary = True
+        logging.info(f"Load boundary from {args.boundary}")
+
     n_unit = 0
     df_full = pd.DataFrame()
+    last_batch = defaultdict(set)
     for chunk in pd.read_csv(args.input, sep='\t', chunksize=1000000, dtype=dty):
         if chunk.shape[0] == 0:
-            logger.info(f"Empty? Left over size {df_full.shape[0]}.")
+            logging.info(f"Empty? Left over size {df_full.shape[0]}.")
             continue
         chunk.rename(columns={args.feature_id:'gene'}, inplace=True)
         chunk['j'] = chunk.X + '_' + chunk.Y
         chunk.X = chunk.X.astype(float)
         chunk.Y = chunk.Y.astype(float)
         ed = chunk[mj].iloc[-1]
         chunk['Group'] = ''
         if len(args.group_within) > 0:
             chunk['Group'] = chunk[args.group_within].apply(lambda x: '_'.join(x), axis=1)
         df_full = pd.concat([df_full, chunk])
 
         if df_full[mj].iloc[-1] - df_full[mj].iloc[0] < ovlp_buffer * args.mu_scale:
             # This chunk is too narrow, leave to process together with neighbors
-            r = int(df_full[mj].iloc[-1]*args.mu_scale)
-            l = int(df_full[mj].iloc[0] *args.mu_scale)
-            logger.info(f"Left over size {df_full.shape[0]} ({l}, {r}).")
+            r = int(df_full[mj].iloc[-1]*mu_scale)
+            l = int(df_full[mj].iloc[0] *mu_scale)
+            logging.info(f"Not enough pixels, left over size {df_full.shape[0]} ({l}, {r}).")
             continue
 
         left = copy.copy(df_full.loc[df_full[mj] > ed - ovlp_buffer * args.mu_scale, keep_header])
 
         for l in df_full.Group.unique():
             df = df_full.loc[df_full.Group.eq(l)]
             brc = df.groupby(by = ['j']).agg(adt).reset_index()
             brc = brc.merge(right = df[['j','X','Y']].drop_duplicates(subset='j'), on = 'j', how='inner')
             brc.index = range(brc.shape[0])
             brc['X'] *= mu_scale
             brc['Y'] *= mu_scale
             st = brc[mj].min()
             ed = brc[mj].max()
             pts = np.asarray(brc[['X','Y']])
-            logger.info(f"Read {brc.shape[0]} pixels.")
+            logging.info(f"Processing {brc.shape[0]} pixels ({len(df)} {st}, {ed}).")
             brc["hex_id"] = ""
             brc["random_index"] = 0
             offs_x = 0
             offs_y = 0
             while offs_x < n_move:
                 while offs_y < n_move:
                     prefix  = str(offs_x)+str(offs_y)
                     x,y = pixel_to_hex(pts, radius, offs_x/n_move, offs_y/n_move)
                     hex_crd = list(zip(x,y))
-                    ct = pd.DataFrame({'hex_id':hex_crd, 'tot':brc[key].values, 'X':pts[:, 0], 'Y':pts[:,1]}).groupby(by = 'hex_id').agg({'tot': sum, 'X':np.min, 'Y':np.min}).reset_index()
-                    mid_ct = np.median(ct.loc[ct.tot >= args.min_ct_per_unit, 'tot'].values)
-                    ct = set(ct.loc[(ct.tot >= args.min_ct_per_unit) & (ct[mj] > st + diam/2) & (ct[mj] < ed - diam/2), 'hex_id'].values)
+                    ct = pd.DataFrame({'hex_id':hex_crd, 'tot':brc[key].values, 'X':pts[:, 0], 'Y':pts[:,1]}).groupby(by = 'hex_id').agg({'tot': "sum", 'X':"min", 'Y':"min"}).reset_index()
+                    mid_ct = np.median(ct.loc[ct.tot >= min_ct_per_unit, 'tot'].values)
+                    ct = set(ct.loc[(ct.tot >= min_ct_per_unit) & (ct[mj] > st + diam/2) & (ct[mj] < ed - diam/2), 'hex_id'].values)
+                    ct = ct - last_batch[(offs_x,offs_y,l)]
                     if len(ct) < 2:
                         offs_y += 1
                         continue
+                    last_batch[(offs_x,offs_y,l)] = ct
                     hex_list = list(ct)
                     suff = [str(x[0])[-1]+str(x[1])[-1] for x in hex_list]
                     hex_dict = {x: str(rng.randint(1, random_index_max)).zfill(random_index_length) + suff[i] for i,x in enumerate(hex_list)}
                     brc["hex_id"] = hex_crd
                     brc["random_index"] = brc.hex_id.map(hex_dict)
                     sub = copy.copy(brc[brc.hex_id.isin(ct)] )
 
                     cnt = sub[['hex_id', 'random_index']].drop_duplicates()
                     hx = cnt.hex_id.map(lambda x : x[0])
                     hy = cnt.hex_id.map(lambda x : x[1])
                     cnt['X'], cnt['Y'] = hex_to_pixel(hx, hy, radius, offs_x/n_move, offs_y/n_move)
+                    if use_boundary:
+                        kept = [mpoly.contains(Point(*p)) for p in cnt[['X','Y']].values]
+                        logging.info(f"Keep {sum(kept)}/{len(cnt)} units within boundary.")
+                        cnt = cnt.loc[kept, :]
 
                     sub = sub.loc[:,['j','random_index']].merge(right = df, on='j', how = 'inner')
                     sub = sub.groupby(by = ['random_index','gene']).agg(adt).reset_index()
                     sub = sub.merge(right = cnt, on = 'random_index', how = 'inner')
                     sub['X'] = [f"{x:.{args.precision}f}" for x in sub.X.values]
                     sub['Y'] = [f"{x:.{args.precision}f}" for x in sub.Y.values]
                     sub = sub.astype({x:int for x in ct_header})
                     # Add offset combination as prefix to random_index
                     sub.random_index = prefix + sub.random_index.values
                     sub.loc[:, output_header].to_csv(args.output, mode='a', sep='\t', index=False, header=False)
                     n_unit += len(ct)
-                    logger.info(f"Sliding offset {offs_x}, {offs_y}. Add {len(ct)} units, median count {mid_ct}, {n_unit} units so far.")
+                    logging.info(f"Sliding offset {offs_x}, {offs_y}. Add {len(ct)} units, median count {mid_ct}, {n_unit} units so far.")
                     offs_y += 1
                 offs_y = 0
                 offs_x += 1
         df_full = copy.copy(left)
-        logger.info(f"Left over size {df_full.shape[0]}.")
+        logging.info(f"Left over size {df_full.shape[0]} ({df_full[mj].iloc[0] * mu_scale :.0f}, {df_full[mj].iloc[-1] * mu_scale :.0f}).")
+
+if __name__ == "__main__":
+    make_dge(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/make_spatial_minibatch.py` & `ficture-0.0.2/ficture/scripts/make_spatial_minibatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ### Stream in pixel level data, assign minibatch label
 ### global-randomize-local-contiguous
 ### Output has the same columns as input with an extra column (1st) being the minibatch index
 
-import sys, os, argparse, gzip, logging, copy, time, warnings, pickle
+import sys, os, argparse, gzip, logging, copy, time
 import subprocess as sp
 import numpy as np
 import pandas as pd
 import random as rng
 
 def make_spatial_minibatch(_args):
 
@@ -14,14 +14,15 @@
 
     # Innput and output info
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', type=str, help='')
 
     # Basic parameter
     parser.add_argument('--major_axis', type=str, default="Y", help='X or Y')
+    parser.add_argument('--major_axis_max', type=float, default=-1, help='')
     parser.add_argument('--batch_size', type=float, default=500, help='Length of the side (um) of square minibatches')
     parser.add_argument('--batch_buff', type=float, default=50, help='Overlap between minibatches')
     parser.add_argument('--mu_scale', type=float, default=26.67, help='Coordinate to um translate')
     parser.add_argument('--min_pixel', type=int, default=100, help='Just to avoid non-tissue regions with isolated pixels')
     parser.add_argument('--seed', type=float, default=-1, help='')
 
     # Specify a region to work on
@@ -29,25 +30,25 @@
     parser.add_argument('--region', nargs='*', type=str, default=[], help='lane:Ystart-Yend (Y axis in barcode coordinate unit), separate by space if multiple regions')
     parser.add_argument('--region_um', nargs='*', type=str, default=[], help='lane:Ystart-Yend (Y axis in um), separate by space if multiple regions')
 
     args = parser.parse_args(_args)
     if len(_args) == 0:
         parser.print_help()
         return
-    logger = logging.getLogger(__name__)
+
+    logging.basicConfig(level= getattr(logging, "INFO", None))
 
     if not os.path.exists(args.input):
         sys.exit("ERROR: cannot find input file")
 
-
     r_seed = args.seed
     if r_seed <= 0:
         r_seed = time.time()
     rng.seed(r_seed)
-    logger.info(f"Random seed {r_seed}")
+    logging.info(f"Random seed {r_seed}")
 
     ### Basic parameterse
     batch_size = int(args.batch_size * args.mu_scale)
     batch_buff = int(args.batch_buff * args.mu_scale)
     batch_step = batch_size - batch_buff
 
     ### Input pixel info (input has to have correct header)
@@ -80,14 +81,15 @@
         process = sp.Popen(["tail", "-n", "+2"], stdin=p0.stdout, stdout=sp.PIPE)
     else:
         process = sp.Popen(cmd, stdout=sp.PIPE, stderr=sp.STDOUT)
 
     ### Group pixels into minibatches
     output_header = copy.copy(input_header)
     output_header.insert(1, "random_index")
+    print(output_header)
     if args.output.endswith(".gz"):
         with gzip.open(args.output, 'wt') as wf:
             _=wf.write('\t'.join(output_header) + '\n')
     else:
         with open(args.output, 'w') as wf:
             _=wf.write('\t'.join(output_header) + '\n')
 
@@ -103,22 +105,28 @@
             end_of_file = True
             if len(df) == 0:
                 break
         else:
             chunk["random_index"] = -1
             chunk.random_index = chunk.random_index.astype(int)
             df = pd.concat([df, chunk])
-        x_min, y_min = df.loc[:, ["X","Y"]].values.min(axis = 0)
-        x_max, y_max = df.loc[:, ["X","Y"]].values.max(axis = 0)
+        x_min, y_min = df[["X","Y"]].values.min(axis = 0)
+        x_max, y_max = df[["X","Y"]].values.max(axis = 0)
         x_range = x_max - x_min
         y_range = y_max - y_min
-        logger.info(f"Read blocks of pixels: {x_range/args.mu_scale:.2f} x {y_range/args.mu_scale:.2f}")
-        if not end_of_file and (x_range < batch_size or y_range < batch_size):
-            continue
-        else:
+        logging.info(f"Read blocks of pixels: {x_range/args.mu_scale:.2f} x {y_range/args.mu_scale:.2f}")
+        if not end_of_file:
+            if x_range < batch_size or y_range < batch_size:
+                continue
+            if args.major_axis_max > 0:
+                if args.major_axis == "X" and x_max > args.major_axis_max - batch_size / 2:
+                    continue
+                if args.major_axis == "Y" and y_max > args.major_axis_max - batch_size / 2:
+                    continue
+        else: # end of file, and the last batch is too small potentially caused by the batch size almost divides the axis lenght
             if (args.major_axis == "X" and x_range <= batch_buff) or (args.major_axis == "Y" and y_range <= batch_buff):
                 break
         x_grd_st = np.arange(x_min, x_max-batch_size/2+1, batch_step)
         if len(x_grd_st) == 0:
             x_grd_st = np.array([x_min-1])
         x_grd_ed = [x + batch_size for x in x_grd_st]
         y_grd_st = np.arange(y_min, y_max-batch_size/2+1, batch_step)
@@ -141,22 +149,26 @@
                     continue
                 df.loc[indx, "random_index"] = rng.randint(1, sys.maxsize//100)
                 ### Output
                 xst /= args.mu_scale
                 xed /= args.mu_scale
                 yst /= args.mu_scale
                 yed /= args.mu_scale
-                logger.info(f"Output region ({xed-xst:.2f}, {yed-yst:.2f}) ({xst:.1f}, {xed:.1f}) x ({yst:.1f}, {yed:.1f})")
+                logging.info(f"Output region ({xed-xst:.2f}, {yed-yst:.2f}) ({xst:.1f}, {xed:.1f}) x ({yst:.1f}, {yed:.1f})")
                 df.loc[indx, output_header].to_csv(args.output, mode='a', sep='\t', index=False, header=False, float_format='%.2f')
                 nbatch += 1
 
         ### Leftover
         if end_of_file:
             break
         mj_max = df.loc[:, args.major_axis].max()
         left_indx = (df.random_index < 0) |\
                     (df[args.major_axis] > mj_max-batch_buff)
         df = df.loc[left_indx, :]
         df["random_index"] = -1
         w  = df[args.major_axis].max() - df[args.major_axis].min()
         w0 = (df.random_index < 0).sum()
-        logger.info(f"Left over size {df.shape[0]} ({w0}, {w:.2f})")
+        logging.info(f"Left over size {df.shape[0]} ({w0}, {w:.2f})")
+
+
+if __name__ == "__main__":
+    make_spatial_minibatch(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/plot_base.py` & `ficture-0.0.2/ficture/scripts/plot_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,37 @@
 import pandas as pd
 from random import shuffle
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from PIL import Image
 
-from scipy.sparse import coo_array
+from scipy.sparse import *
 import sklearn.neighbors
 import sklearn.preprocessing
 
 from ficture.utils.hexagon_fn import *
 from ficture.utils.utilt import plot_colortable
 
 def plot_base(_args):
 
     parser = argparse.ArgumentParser(prog = "plot_base")
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', type=str, help='Output prefix')
     parser.add_argument('--fill_range', type=float, default=0, help="um")
-    parser.add_argument('--batch_size', type=float, default=100000, help="")
+    parser.add_argument('--batch_size', type=float, default=500, help="")
     parser.add_argument("--tif", action='store_true', help="Store as 16-bit tif instead of png")
     parser.add_argument('--scale', type=float, default=-1, help="")
     parser.add_argument('--origin', type=int, default=[0,0], help="{0, 1} x {0, 1}, specify how to orient the image w.r.t. the coordinates. (0, 0) means the lower left corner has the minimum x-value and the minimum y-value; (0, 1) means the lower left corner has the minimum x-value and the maximum y-value;")
     parser.add_argument('--category_column', type=str, default='', help='')
 
     parser.add_argument('--color_table_category_name', type=str, default='Name', help='When --category_column is provided, which column to use as the category name')
     parser.add_argument('--binary_cmap_name', type=str, default="plasma", help="Name of Matplotlib colormap to use for ploting individual factors")
     parser.add_argument('--color_table', type=str, default='', help='Pre-defined color map')
+    parser.add_argument('--input_rgb_uint8', action="store_true",help="If input rgb is from 0-255 instead of 0-1")
     parser.add_argument('--cmap_name', type=str, default="turbo", help="Name of Matplotlib colormap, only used when --color_table is not provided")
 
     parser.add_argument("--plot_fit", action='store_true', help="")
     parser.add_argument('--xmin', type=float, default=-np.inf, help="")
     parser.add_argument('--ymin', type=float, default=-np.inf, help="")
     parser.add_argument('--xmax', type=float, default=np.inf, help="")
     parser.add_argument('--ymax', type=float, default=np.inf, help="")
@@ -40,16 +41,19 @@
 
     parser.add_argument("--skip_mixture_plot", action='store_true', help="")
     parser.add_argument("--plot_discretized", action='store_true', help="")
     parser.add_argument("--plot_individual_factor", action='store_true', help="")
     parser.add_argument("--debug", action='store_true', help="")
 
     args = parser.parse_args(_args)
-    logger = logging.getLogger(__name__)
+    if len(_args) == 0:
+        parser.print_help()
+        return
 
+    logging.basicConfig(level= getattr(logging, "INFO", None))
     dt = np.uint16 if args.tif else np.uint8
     kcol = args.category_column
     ccol = args.color_table_category_name
 
     # Dangerous way to detect which columns to use as factor loadings
     with gzip.open(args.input, "rt") as rf:
         header = rf.readline().strip().split('\t')
@@ -62,31 +66,37 @@
     categorical = False
     if args.category_column != '':
         if args.category_column not in header:
             sys.exit(f"ERROR: {args.category_column} not found in header")
         categorical = True
         if not os.path.exists(args.color_table):
             sys.exit(f"ERROR: --color_table is required for categorical input")
-        color_info = pd.read_csv(args.color_table, sep='\t', header=0)
-        color_info[ccol] = color_info[ccol].astype(str)
-        color_idx = {x:i for i,x in enumerate(color_info[ccol])}
+        color_info = pd.read_csv(args.color_table, sep='\t', header=0, dtype={ccol:str})
+        if args.input_rgb_uint8 or color_info[["R","G","B"]].max().max() > 2:
+            for c in list("RGB"):
+                color_info[c] = color_info[c] / 255
+        color_info = color_info[~color_info[ccol].isna()]
+        color_idx = {x:i for i,x in enumerate(color_info[ccol].values)}
         cmtx = np.array(color_info.loc[:, ["R","G","B"]])
         K = len(color_idx)
         factor_header = [str(k) for k in range(K)]
-        print("Use categorical input")
+        logging.info(f"Use categorical input ({K} categories)")
     else:
         for x in header:
             y = re.match('^[A-Za-z]*_*(\d+)$', x)
             if y:
                 factor_header.append([y.group(0), int(y.group(1)) ])
         factor_header.sort(key = lambda x : x[1] )
         factor_header = [x[0] for x in factor_header]
         K = len(factor_header)
         if os.path.exists(args.color_table):
             color_info = pd.read_csv(args.color_table, sep='\t', header=0)
+            if args.input_rgb_uint8 or color_info[["R","G","B"]].max().max() > 2:
+                for c in list("RGB"):
+                    color_info[c] = color_info[c] / 255
             cmtx = np.array(color_info.loc[:, ["R","G","B"]])
         else:
             cmap_name = args.cmap_name
             if args.cmap_name not in plt.colormaps():
                 cmap_name = "turbo"
             cmap = plt.get_cmap(cmap_name, K)
             cmtx = np.array([cmap(i) for i in range(K)] )
@@ -95,15 +105,15 @@
             cmtx = cmtx[indx, ]
             cmtx = cmtx[:, :3]
             cdict = {k:cmtx[k,:] for k in range(K)}
             # Plot color bar separately
             fig = plot_colortable(cdict, "Factor label", sort_colors=False, ncols=4)
             f = args.output + ".cbar"
             fig.savefig(f, format="png")
-            logger.info(f"Set up color map for {K} factors")
+            logging.info(f"Set up color map for {K} factors")
 
     # Read data
     adt={x:float for x in ["x", "y"]+factor_header}
     adt[kcol] = str
     df = pd.DataFrame()
     for chunk in pd.read_csv(gzip.open(args.input, 'rt'), sep='\t', \
         chunksize=1000000, skiprows=1, names=header, dtype=adt):
@@ -118,49 +128,51 @@
             chunk[kcol] = chunk[kcol].map(color_idx).astype(int)
             for k in range(K):
                 chunk[str(k)] = chunk[kcol].eq(k).astype(int)
         chunk = chunk.groupby(by = ['x_indx', 'y_indx']).agg({ x:np.mean for x in factor_header }).reset_index()
         df = pd.concat([df, chunk])
 
     df = df.groupby(by = ['x_indx', 'y_indx']).agg({ x:np.mean for x in factor_header }).reset_index()
-    x_indx_min = int(args.xmin / args.plot_um_per_pixel )
-    y_indx_min = int(args.ymin / args.plot_um_per_pixel )
+    x_indx_min = args.xmin / args.plot_um_per_pixel
+    y_indx_min = args.ymin / args.plot_um_per_pixel
     if args.plot_fit or np.isinf(args.xmin):
-        df.x_indx = df.x_indx - np.max([x_indx_min, df.x_indx.min()])
+        df.x_indx = df.x_indx - int(np.max([x_indx_min, df.x_indx.min()]) )
     else:
-        df.x_indx -= x_indx_min
+        df.x_indx -= int(x_indx_min)
     if args.plot_fit or np.isinf(args.ymin):
-        df.y_indx = df.y_indx - np.max([y_indx_min, df.y_indx.min()])
+        df.y_indx = df.y_indx - int(np.max([y_indx_min, df.y_indx.min()]) )
     else:
-        df.y_indx -= y_indx_min
+        df.y_indx -= int(y_indx_min)
 
     N0 = df.shape[0]
     df.index = range(N0)
     hsize, wsize = df[['x_indx','y_indx']].max(axis = 0) + 1
     hsize_um = hsize * args.plot_um_per_pixel
     wsize_um = wsize * args.plot_um_per_pixel
-    logger.info(f"Read region {N0} pixels in region {hsize_um} x {wsize_um}")
+    logging.info(f"Read region {N0} pixels in region {hsize_um} x {wsize_um}")
 
 
     # Make images
     wst = df.y_indx.min()
     wed = df.y_indx.max()
-    wstep = np.max([10, int(args.batch_size / hsize)])
+    wstep = np.max([10, int(args.batch_size)])
     radius = args.fill_range/args.plot_um_per_pixel
+    print(wsize, wstep)
+
 
     if radius <= 0:
         pts = df[['x_indx', 'y_indx']].values
         pts_indx = df.index.values
     else:
         pts = np.zeros((0, 2), dtype=int)
         pts_indx = []
         st = wst
         while st < wed:
             ed = min([st + wstep, wed])
-            logger.info(f"Filling pixels {st} - {ed} / {wed}")
+            logging.info(f"Filling pixels {st} - {ed} / {wed}")
             if ((df.y_indx > st) & (df.y_indx < ed)).sum() < 10:
                 st = ed
                 continue
             block = df.index[(df.y_indx > st - 2*radius) & (df.y_indx < ed + 2*radius)]
             ref = sklearn.neighbors.BallTree(np.array(df.loc[block, ['x_indx', 'y_indx']]))
             mesh = np.meshgrid(np.arange(hsize), np.arange(st, ed))
             nodes = np.array(list(zip(*(dim.flat for dim in mesh))), dtype=int)
@@ -180,15 +192,15 @@
     pts[:,0] = np.clip(hsize - pts[:, 0], 0, hsize-1)
     pts[:,1] = np.clip(pts[:, 1], 0, wsize-1)
     if args.origin[0] > 0:
         pts[:,0] = hsize - 1 - pts[:, 0]
     if args.origin[1] > 0:
         pts[:,1] = wsize - 1 - pts[:, 1]
 
-    logger.info(f"Start constructing RGB image")
+    logging.info(f"Start constructing RGB image")
 
     if not args.skip_mixture_plot:
         rgb_mtx = np.clip(np.around(np.array(df.loc[pts_indx,factor_header]) @\
                                     cmtx * 255),0,255).astype(dt)
         img = np.zeros( (hsize, wsize, 3), dtype=dt)
         for r in range(3):
             img[:, :, r] = coo_array((rgb_mtx[:, r], (pts[:,0], pts[:,1])),\
@@ -197,15 +209,15 @@
             img = Image.fromarray(img, mode="I;16")
         else:
             img = Image.fromarray(img)
 
         outf = args.output
         outf += ".tif" if args.tif else ".png"
         img.save(outf)
-        logger.info(f"Made fractional image\n{outf}")
+        logging.info(f"Made fractional image\n{outf}")
 
     if args.plot_discretized:
         kvec = np.array(df.loc[pts_indx,factor_header]).argmax(axis = 1)
         cmtx = np.clip(np.around(cmtx * 255), 0, 255).astype(dt)
         img = np.zeros( (hsize, wsize, 3), dtype=dt)
         for r in range(3):
             img[:, :, r] = coo_array((cmtx[kvec, r], (pts[:,0], pts[:,1])),\
@@ -235,8 +247,11 @@
             if args.tif:
                 img = Image.fromarray(img, mode="I;16")
             else:
                 img = Image.fromarray(img)
             outf = args.output + ".F_"+str(k)
             outf += ".tif" if args.tif else ".png"
             img.save(outf)
-            logger.info(f"Made factor specific image - {k}\n{outf}")
+            logging.info(f"Made factor specific image - {k}\n{outf}")
+
+if __name__ == "__main__":
+    plot_base(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/plot_pixel_multi.py` & `ficture-0.0.2/ficture/scripts/plot_pixel_multi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,115 +1,138 @@
 # Visualize pixel level factor analysis results
 # <= 5 (preferably 3) factors at a time, with specified colors
 # Input file contains only top k factors and probabilities per pixel
 # Meant to make use of the indexed input to plot for specified regions quickly
 
-import sys, os, copy, gc, re, gzip, pickle, argparse, logging, warnings
+import sys, os, copy, re, gzip, argparse, logging, warnings
 import numpy as np
 import pandas as pd
 from scipy.sparse import *
-import subprocess as sp
-from joblib.parallel import Parallel, delayed
-import matplotlib as mpl
 import cv2
 
-from ficture.utils import utilt
 from ficture.loaders.pixel_factor_loader import BlockIndexedLoader
 
 def plot_pixel_multi(_args):
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', type=str, help='Output file full path')
     parser.add_argument('--channel_list', type=str, nargs='+', help="Select up to 3 channels/factors to visualize")
-    parser.add_argument('--color_list', type=str, nargs='*', default=["#144A74", "#FF9900", "#FFEC11", "#DD65E6"], help='')
+    parser.add_argument('--color_list', type=str, nargs='*', default=["144A74", "FF9900", "DD65E6", "FFEC11"], help='') # blue, orange, purple, yellow
     parser.add_argument('--color_table', type=str, default='', help='Pre-defined color map')
     parser.add_argument('--color_table_index_column', type=str, default='Name', help='')
+    parser.add_argument('--input_rgb_uint8', action="store_true",help="If input rgb is from 0-255 instead of 0-1")
+
     parser.add_argument('--xmin', type=float, default=-np.inf, help="")
     parser.add_argument('--ymin', type=float, default=-np.inf, help="")
     parser.add_argument('--xmax', type=float, default=np.inf, help="")
     parser.add_argument('--ymax', type=float, default=np.inf, help="")
+    parser.add_argument('--pcut', type=float, default=0.01, help="")
+    parser.add_argument('--spcut', type=float, default=0.1, help="")
+    parser.add_argument('--org_coord', action='store_true', help="If the input coordinates do not include the offset (if your coordinates are from an existing figure, the offset is already factored in)")
     parser.add_argument('--full', action='store_true', help="")
     parser.add_argument('--plot_um_per_pixel', type=float, default=1, help="Actual size (um) corresponding to each pixel in the output image")
     parser.add_argument('--categorical', action='store_true', help="Plot top factor for each pixel categorically, without probability or mixture")
     parser.add_argument('--debug', action='store_true', help="")
 
     args = parser.parse_args(_args)
-    logger =  logging.getLogger(__name__)
+    if len(_args) == 0:
+        parser.print_help()
+        return
+
+    logging.basicConfig(level= getattr(logging, "INFO", None), format='%(asctime)s %(message)s', datefmt='%I:%M:%S %p')
 
     rgb=list("RGB")
     bgr=list("BGR") # opencv default channel order
     bgra=list("BGRA") # opencv bgra
     pcut = 0.01
     spcut = 0.1
     if len(args.channel_list) > 5:
-        logger.error("Be colorblind friendly, visualize <=5 and preferably 3 channels at a time")
-        sys.exit(1)
+        logging.warning("Be colorblind friendly")
     channels = args.channel_list
     # Read color table
     if os.path.exists(args.color_table):
         color_info = pd.read_csv(args.color_table, sep='\t', header=0, index_col=args.color_table_index_column)
-        if color_info[rgb].max().max() > 1:
-            logger.warning("Color table should contain RGB values in 0-1 range, but found values > 1, will interpret as in 0-255 range")
+        if color_info[rgb].max().max() > 1.1 and not args.input_rgb_uint8:
+            logging.warning("Color table should contain RGB values in 0-1 range, but found values > 1, will assume unit8")
+            args.input_rgb_uint8 = True
+        if args.input_rgb_uint8:
             for c in rgb:
                 color_info[c] = np.clip(color_info[c]/255,0,1)
         color_info.index = color_info.index.astype(str)
         channels = [x for x in channels if x in color_info.index]
         if len(channels) != len(args.channel_list):
-            logger.error("Some channels are not found in the input color table")
+            logging.error("Some channels are not found in the input color table")
             sys.exit(1)
         color_info = {i: np.array(color_info.loc[i, rgb]) for i in channels}
     else:
         if len(args.color_list) < len(channels):
-            logger.error("Number of input colors and channels do not match")
+            logging.error("Number of input colors and channels do not match")
             sys.exit(1)
         color_list = [[int(x.strip('#')[i:i+2],16)/255 for i in (0,2,4)] for x in args.color_list]
         color_info = {x:np.array(color_list[i]) for i,x in enumerate(channels)}
+        ctab = pd.DataFrame(color_info, index=rgb).T
+        ctab['Name'] = ctab.index
+        if not args.output.endswith(".png"):
+            f = args.output + ".color_table.tsv"
+        else:
+            f = args.output.replace(".png", ".color_table.tsv")
+        ctab.to_csv(f, sep='\t', header=True, index=False)
 
-    logger.info(f"Read color map {color_info}")
+    logging.info(f"Set up color map {color_info}")
 
-    loader = BlockIndexedLoader(args.input, args.xmin, args.xmax, args.ymin, args.ymax, args.full)
+    loader = BlockIndexedLoader(args.input, args.xmin, args.xmax, args.ymin, args.ymax, args.full, not args.org_coord)
     width = int((loader.xmax - loader.xmin + 1)/args.plot_um_per_pixel)
     height= int((loader.ymax - loader.ymin + 1)/args.plot_um_per_pixel)
-    logger.info(f"Image size {height} x {width}")
+    logging.info(f"Image size {height} x {width}")
 
     # Read input file, fill the rgb matrix
     img = np.zeros((height,width,4), dtype=np.uint8)
     img[:,:,3] = 255
+    clps = {x:np.mean for x in rgb}
+    clps['A'] = np.max
     for df in loader:
         if df.shape[0] == 0:
             continue
-        logger.info(f"Reading pixels... {df.X.iloc[-1]}, {df.Y.iloc[-1]}, {df.shape[0]}")
         indx = np.zeros(df.shape[0], dtype=bool)
         if args.categorical:
             indx = df.K1.isin(channels)
         else:
             for k in range(1, loader.meta['TOPK']):
                 indx = indx | (df[f"K{k}"].isin(channels) & df[f"P{k}"].gt(pcut))
         df = df.loc[indx, :]
+        if args.debug:
+            print(df.shape[0])
         if df.shape[0] == 0:
             continue
         df['X'] = np.clip(((df.X - loader.xmin) / args.plot_um_per_pixel).astype(int),0,width-1)
         df['Y'] = np.clip(((df.Y - loader.ymin) / args.plot_um_per_pixel).astype(int),0,height-1)
         df[bgra] = 0
         if args.categorical:
             df.loc[:,rgb] = np.array(list(df.K1.map(color_info)) )
             df['A'] = 1
         else:
             for k in range(1, loader.meta['TOPK']):
                 indx = df[f"K{k}"].isin(channels)
                 if indx.sum() == 0:
                     continue
-                df.loc[indx, rgb] = np.array(list(df.loc[indx, f"K{k}"].map(color_info))) * df.loc[indx, f"P{k}"].values.reshape((-1,1))
+                df.loc[indx, rgb] += np.array(list(df.loc[indx, f"K{k}"].map(color_info))) * df.loc[indx, f"P{k}"].values.reshape((-1,1))
                 df.loc[indx, 'A'] += df.loc[indx, f"P{k}"]
-        df = df.groupby(by=['X','Y']).agg({c:np.mean for c in bgra}).reset_index()
+        if args.debug:
+            print(df.shape[0], np.median(df.A), np.mean(df.A), df.A.gt(spcut).sum())
+        df = df.groupby(by=['X','Y']).agg(clps).reset_index()
         df = df.loc[df.A.gt(spcut), :]
         df[bgra] = np.clip(np.around(df[bgra] * 255),0,255).astype(np.uint8)
+        logging.info(f"Reading pixels... {df.X.iloc[-1]}, {df.Y.iloc[-1]}, {df.shape[0]}")
         for i,c in enumerate(bgra):
             img[df.Y.values, df.X.values, [i]*df.shape[0]] = df[c].values
         if args.debug:
             break
 
     if not args.output.endswith(".png"):
         args.output += ".png"
     cv2.imwrite(args.output,img)
-    logger.info(f"Finished")
+    logging.info(f"Finished\n{args.output}")
+
+
+if __name__ == "__main__":
+    plot_pixel_multi(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/plot_pixel_single.py` & `ficture-0.0.2/ficture/scripts/plot_pixel_single.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,79 +3,89 @@
 # Meant to make use of the indexed input to plot for specified regions quickly
 # Would take a huge amount of memory if trying to plot many factors simultaneously in a large region
 
 import sys, os, copy, gc, re, gzip, pickle, argparse, logging, warnings
 import numpy as np
 import pandas as pd
 from scipy.sparse import *
-import subprocess as sp
-from joblib.parallel import Parallel, delayed
 import matplotlib as mpl
 import cv2
 
-from ficture.utils import utilt
 from ficture.loaders.pixel_factor_loader import BlockIndexedLoader
 
 def plot_pixel_single(_args):
 
     parser = argparse.ArgumentParser(prog="plot_pixel_single")
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--output', type=str, help="Output prefix")
     parser.add_argument('--id_list', type=str, nargs="+", help="List of IDs of the factors to plot")
-
     parser.add_argument('--pcut', type=float, default=1e-2, help="")
     parser.add_argument('--binary_cmap_name', type=str, default="plasma", help="Name of Matplotlib colormap to use for ploting individual factors")
 
     parser.add_argument('--xmin', type=float, default=-np.inf, help="")
     parser.add_argument('--ymin', type=float, default=-np.inf, help="")
     parser.add_argument('--xmax', type=float, default=np.inf, help="")
     parser.add_argument('--ymax', type=float, default=np.inf, help="")
+    parser.add_argument('--org_coord', action='store_true', help="If the input coordinates do not include the offset (if your coordinates are from an existing figure, the offset is already factored in)")
     parser.add_argument('--full', action='store_true', help="Read full input")
     parser.add_argument('--plot_um_per_pixel', type=float, default=1, help="Actual size (um) corresponding to each pixel in the output image")
     parser.add_argument('--all', action="store_true", help="Caution: when set, assume factors are named as 0, 1, ... K-1, where K is defined in the input header. Only use when plotting a small region.")
+    parser.add_argument('--debug', action='store_true', help="")
 
     args = parser.parse_args(_args)
-    logger = logging.getLogger(__name__)
+    if len(_args) == 0:
+        parser.print_help()
+        return
+
+    logging.basicConfig(level= getattr(logging, "INFO", None), format='%(asctime)s %(message)s', datefmt='%I:%M:%S %p')
     if not os.path.exists(os.path.dirname(args.output)):
         os.makedirs(os.path.dirname(args.output))
 
-    loader = BlockIndexedLoader(args.input, args.xmin, args.xmax, args.ymin, args.ymax, args.full)
+    loader = BlockIndexedLoader(args.input, args.xmin, args.xmax, args.ymin, args.ymax, args.full, not args.org_coord)
     width = int((loader.xmax - loader.xmin + 1)/args.plot_um_per_pixel)
     height= int((loader.ymax - loader.ymin + 1)/args.plot_um_per_pixel)
-    logger.info(f"Image size {height} x {width}")
+    logging.info(f"Image size {height} x {width}")
+    if args.debug:
+        logging.info(f"{loader.xmin}, {loader.xmax}, {loader.ymin}, {loader.ymax}")
 
     id_list = args.id_list
     if args.all:
         id_list = [str(k) for k in range(loader.meta['K'])]
 
     # Read input file
     df = pd.DataFrame()
     for chunk in loader:
         if chunk.shape[0] == 0:
             continue
-        logger.info(f"Reading pixels... {chunk.X.iloc[-1]}, {chunk.Y.iloc[-1]}, {df.shape[0]}")
         chunk['X'] = np.clip(((chunk.X - loader.xmin) / args.plot_um_per_pixel).astype(int),0,width-1)
         chunk['Y'] = np.clip(((chunk.Y - loader.ymin) / args.plot_um_per_pixel).astype(int),0,height-1)
         for k in id_list:
             chunk[k] = np.zeros(chunk.shape[0], dtype=np.float16)
             for i in range(1, loader.meta['TOPK']+1):
                 indx = chunk['K'+str(i)].eq(k) & chunk['P'+str(i)].gt(args.pcut)
                 chunk.loc[indx, k] = chunk.loc[indx, 'P'+str(i)]
         chunk = chunk.groupby(by=['X','Y']).agg({k:np.mean for k in id_list}).reset_index()
         pmax = chunk.loc[:, id_list].max(axis = 1)
         df = pd.concat([df, chunk.loc[pmax > args.pcut, :]])
+        logging.info(f"Reading pixels... {chunk.X.iloc[-1]}, {chunk.Y.iloc[-1]}, {df.shape[0]}")
     df.drop_duplicates(subset=['X','Y'], inplace=True)
-    logger.info(f"Read {df.shape[0]} pixels")
+    if df.shape[0] == 0:
+        sys.exit("ERROR: No pixels found")
+
+    logging.info(f"Read {df.shape[0]} pixels")
 
     for k in id_list:
         indx = df[k] > args.pcut
         if (df[k] > .5).sum() < 10 and indx.sum() < 100:
             continue
         rgb = np.clip(mpl.colormaps['plasma'](df.loc[indx, k].values)[:,:3]*255,0,255).astype(np.uint8)
         img = np.zeros((height,width,3), dtype=np.uint8)
         for i in range(3):
             img[:, :, i] = coo_array( ( rgb[:, i], (df.loc[indx, 'Y'], df.loc[indx, 'X']) ), shape=(height, width) ).toarray()
         img = cv2.cvtColor(img, cv2.COLOR_RGB2BGR)
         cv2.imwrite(args.output +".F_" +k+".png",img)
-        logger.info(f"Made image for {k}")
+        logging.info(f"Made image for {k}")
+
+    logging.info(f"Finished")
 
-    logger.info(f"Finished")
+if __name__ == "__main__":
+    plot_pixel_single(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/slda_decode.py` & `ficture-0.0.2/ficture/scripts/slda_decode.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,111 @@
 import sys, os, argparse, logging, gzip, copy, re, time, warnings, pickle
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import normalize
+from datetime import datetime
 
 from ficture.models.online_slda import OnlineLDA
 from ficture.loaders.pixel_loader import PixelMinibatch
 
 def slda_decode(_args):
 
     parser = argparse.ArgumentParser(prog="slda_decode")
     # Innput and output info
     parser.add_argument('--input', type=str, help='')
     parser.add_argument('--model', type=str, help='')
     parser.add_argument('--output', type=str, help='')
     parser.add_argument('--anchor', type=str, help='')
     parser.add_argument('--anchor_in_um', action='store_true')
+    parser.add_argument('--feature', type=str, default='', help='')
 
     # Data realted parameters
     parser.add_argument('--mu_scale', type=float, default=26.67, help='Coordinate to um translate')
     parser.add_argument('--key', type=str, default = 'gn', help='gt: genetotal, gn: gene, spl: velo-spliced, unspl: velo-unspliced')
     parser.add_argument('--batch_id', type=str, default = 'random_index', help='Input has to have a column with this name indicating the minibatch id')
     parser.add_argument('--precision', type=float, default=.25, help='If positive, collapse pixels within X um.')
 
     # Learning related parameters
     parser.add_argument('--thread', type=int, default=1, help='')
     parser.add_argument('--neighbor_radius', type=float, default=25, help='The radius (um) of each anchor point\'s territory')
     parser.add_argument('--halflife', type=float, default=0.7, help='Control the decay of distance-based weight')
     parser.add_argument('--theta_init_bound_multiplier', type=float, default=.2, help='')
     parser.add_argument('--inner_max_iter', type=int, default=30, help='')
     parser.add_argument('--model_scale', type=float, default=-1, help='')
+    parser.add_argument('--seed', type=int, default=-1, help='')
 
     # Other
     parser.add_argument('--lite_topk_output_pixel', type=int, default=-1)
     parser.add_argument('--lite_topk_output_anchor', type=int, default=-1)
+    parser.add_argument('--log', type=str, default = '', help='files to write log to')
     parser.add_argument('--debug', action='store_true')
 
     args = parser.parse_args(_args)
-    logger = logging.getLogger('slda_decode')
+    if len(_args) == 0:
+        parser.print_help()
+        return
+
+    if args.log != '':
+        try:
+            logging.basicConfig(filename=args.log, filemode='a', encoding='utf-8', level=logging.INFO)
+        except:
+            logging.basicConfig(level= getattr(logging, "INFO", None))
+    else:
+        logging.basicConfig(level= getattr(logging, "INFO", None))
+
     if not os.path.exists(args.model):
         sys.exit("ERROR: cannot find model file")
     if not os.path.exists(args.input):
         sys.exit("ERROR: cannot find input file")
     if not os.path.exists(args.anchor):
         sys.exit("ERROR: cannot find anchor file")
 
+    ## obtain seed if not provided
+    seed = int(args.seed)
+    if seed <= 0:
+        seed = int(datetime.now().timestamp()) % 2147483648
+
     ### Basic parameterse
     mu_scale = 1./args.mu_scale
     radius = args.neighbor_radius
     precision = args.precision
     key = args.key.lower()
     batch_id = args.batch_id.lower()
     chunk_size = 500000
 
     ### Load model
+    factor_names = []
     if args.model.endswith(".tsv.gz") or args.model.endswith(".tsv"):
         # If input is a gzip tsv file
         model = pd.read_csv(args.model, sep='\t')
-        gene_kept = list(model.gene)
+        factor_names = list(model.columns)[1:]
+        feature_kept = model.gene.values
         model = np.array(model.iloc[:,1:]).T
         model = np.clip(model, 0.5, None)
     else:
         # If input is a pickled model object
         try:
             model = pickle.load(open( args.model, "rb" ))
-            gene_kept = model.feature_names_in_
+            feature_kept = np.array(model.feature_names_in_)
             model = model.components_
         except:
             sys.exit("ERROR: --model input should be either a tsv file containing gene names and factor profiles, or a pickled model object with at least two attributes, feature_names_in_ and components_, like those defined in scikit-learn LDA model")
+    if os.path.isfile(args.feature):
+        feature = pd.read_csv(args.feature, sep='\t')
+        kept_idx = np.where(np.in1d(feature_kept, feature.gene.values))[0]
+        feature_kept = np.array(feature_kept)[kept_idx]
+        model = model[:, kept_idx]
 
     K, M = model.shape
-    ft_dict = {x:i for i,x in enumerate( gene_kept ) }
+    ft_dict = {x:i for i,x in enumerate( feature_kept ) }
     if args.model_scale > 0:
         model = normalize(model, norm='l1', axis=1) * args.model_scale
-    logger.info(f"{M} genes and {K} factors are read from input model")
+    logging.info(f"{M} genes and {K} factors are read from input model")
 
-    slda = OnlineLDA(vocab=gene_kept, K=K, N=1e6, iter_inner=args.inner_max_iter, verbose = 1)
+    slda = OnlineLDA(vocab=feature_kept, K=K, N=1e6, iter_inner=args.inner_max_iter, verbose = 1, seed = seed)
     slda.init_global_parameter(model)
     init_bound = 1./K * args.theta_init_bound_multiplier
 
     ### Input pixel info (input has to contain certain columns with correct header)
     with gzip.open(args.input, 'rt') as rf:
         oheader = rf.readline().strip().split('\t')
     oheader = [x.lower() if len(x) > 1 else x.upper() for x in oheader]
@@ -96,52 +123,63 @@
 
     pixel_obj = PixelMinibatch(pixel_reader, ft_dict, \
                             batch_id, key, mu_scale, \
                             radius=radius, halflife=args.halflife,\
                             precision=args.precision, thread=args.thread)
     ### anchor info
     pixel_obj.load_anchor(args.anchor, args.anchor_in_um)
-    logger.info(f"Read {pixel_obj.grid_info.shape[0]} grid points")
+    logging.info(f"Read {pixel_obj.grid_info.shape[0]} grid points")
     factor_header = pixel_obj.factor_header
 
     post_count = np.zeros((K, M))
     n_batch = 0
     while True:
         read_n_batch = pixel_obj.read_chunk(args.thread)
-        logger.info(f"Read {read_n_batch} batches ({pixel_obj.dge_mtx.shape})")
+        logging.info(f"Read {read_n_batch} batches ({pixel_obj.dge_mtx.shape})")
         pcount, pixel, anchor  = pixel_obj.run_chunk(slda, init_bound)
-        logger.info(f"Output {pixel.shape[0]} pixels and {anchor.shape[0]} anchors")
         pixel.X = pixel.X.map('{:.2f}'.format)
         pixel.Y = pixel.Y.map('{:.2f}'.format)
         if args.lite_topk_output_pixel > 0 and args.lite_topk_output_pixel < K:
-            part = np.argpartition(-pixel[factor_header].values, kth=np.arange(args.lite_topk_output_pixel), axis=1)[:, :args.lite_topk_output_pixel]
+            X = pixel[factor_header].values
+            partial_indices = np.argpartition(X, -args.lite_topk_output_pixel, axis=1)[:, -args.lite_topk_output_pixel:]
+            sorted_top_indices = np.argsort(X[np.arange(X.shape[0])[:, None], partial_indices], axis=1)[:, ::-1]
+            top_indices = partial_indices[np.arange(partial_indices.shape[0])[:, None], sorted_top_indices]
+            top_values = X[np.arange(X.shape[0])[:, None], top_indices]
             for k in range(args.lite_topk_output_pixel):
-                pixel[f"K{k}"] = part[:,k]
-            part = np.partition(-pixel[factor_header].values, kth=np.arange(args.lite_topk_output_pixel), axis=1)[:, :args.lite_topk_output_pixel]
+                pixel[f"K{k+1}"] = top_indices[:, k]
             for k in range(args.lite_topk_output_pixel):
-                pixel[f"P{k}"] = np.clip(-part[:,k], 0, 1)
+                pixel[f"P{k+1}"] = np.clip(top_values[:, k], 0, 1)
             pixel.drop(columns = factor_header, inplace=True)
         write_mode = 'w' if n_batch == 0 else 'a'
         header_include = True if n_batch == 0 else False
         pixel.to_csv(args.output+".pixel.tsv.gz", sep='\t', index=False, header=header_include, mode=write_mode, float_format="%.2e", compression={"method":"gzip"})
+        logging.info(f"Output {pixel.shape[0]} pixels and {anchor.shape[0]} anchors")
         anchor.X = anchor.X.map('{:.2f}'.format)
         anchor.Y = anchor.Y.map('{:.2f}'.format)
         if args.lite_topk_output_anchor > 0 and args.lite_topk_output_anchor < K:
-            part = np.argpartition(-anchor[factor_header].values, kth=np.arange(args.lite_topk_output_anchor), axis=1)[:, :args.lite_topk_output_anchor]
+            X = anchor[factor_header].values
+            partial_indices = np.argpartition(X, -args.lite_topk_output_anchor, axis=1)[:, -args.lite_topk_output_anchor:]
+            sorted_top_indices = np.argsort(X[np.arange(X.shape[0])[:, None], partial_indices], axis=1)[:, ::-1]
+            top_indices = partial_indices[np.arange(partial_indices.shape[0])[:, None], sorted_top_indices]
+            top_values = X[np.arange(X.shape[0])[:, None], top_indices]
             for k in range(args.lite_topk_output_anchor):
-                anchor[f"K{k}"] = part[:,k]
-            part = np.partition(-anchor[factor_header].values, kth=np.arange(args.lite_topk_output_anchor), axis=1)[:, :args.lite_topk_output_anchor]
+                anchor[f"K{k+1}"] = top_indices[:, k]
             for k in range(args.lite_topk_output_anchor):
-                anchor[f"P{k}"] = np.clip(-part[:,k], 0, 1)
+                anchor[f"P{k+1}"] = np.clip(top_values[:, k], 0, 1)
             anchor.drop(columns = factor_header, inplace=True)
         anchor.to_csv(args.output+".anchor.tsv.gz", sep='\t', index=False, header=header_include, mode=write_mode, float_format="%.2e", compression={"method":"gzip"})
         n_batch += read_n_batch
         post_count += pcount
         if not pixel_obj.file_is_open:
             break
 
     ### Output posterior summaries
+    if len(factor_names) == K:
+        factor_header = factor_names
     out_f = args.output + ".posterior.count.tsv.gz"
-    pd.concat([pd.DataFrame({'gene': gene_kept}),\
+    pd.concat([pd.DataFrame({'gene': feature_kept}),\
             pd.DataFrame(post_count.T, dtype='float64',\
                             columns = factor_header)],\
             axis = 1).to_csv(out_f, sep='\t', index=False, float_format='%.2f', compression={"method":"gzip"})
+
+if __name__ == "__main__":
+    slda_decode(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/scripts/transform_univ.py` & `ficture-0.0.2/ficture/scripts/transform_univ.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,47 +3,62 @@
 Model contains gene names and either Dirichlet parameters (or probabilities for more general use?)
 Input pixel level data will be grouped into (overlapping) hexagons
 '''
 import sys, os, copy, gzip, time, logging, pickle, argparse
 import numpy as np
 import pandas as pd
 import random as rng
+from sklearn.preprocessing import normalize
+from sklearn.decomposition import LatentDirichletAllocation as LDA
+sys.path.append(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+from sklearn.decomposition._online_lda_fast import _dirichlet_expectation_2d
 
 from ficture.loaders.pixel_to_unit_loader import PixelToUnit
-from ficture.models.online_lda import OnlineLDA
+from ficture.utils.utilt import init_latent_vars
 
 def transform(_args):
 
     parser = argparse.ArgumentParser(prog = "transform")
     parser.add_argument('--input', type=str, help='')
-    parser.add_argument('--output_pref', type=str, help='')
+    parser.add_argument('--output', '--output_pref', type=str, help='')
     parser.add_argument('--model', type=str, help='')
+    parser.add_argument('--feature', type=str, default='', help='')
 
     parser.add_argument('--key', type=str, default = 'gn', help='gt: genetotal, gn: gene, spl: velo-spliced, unspl: velo-unspliced')
     parser.add_argument('--major_axis', type=str, default=None, help='X or Y')
     parser.add_argument('--region_id', type=str, default=None, help='')
     parser.add_argument('--min_ct_per_unit', type=int, default=20, help='')
     parser.add_argument('--mu_scale', type=float, default=26.67, help='Coordinate to um translate')
     parser.add_argument('--thread', type=int, default=-1, help='')
     parser.add_argument('--n_move', type=int, default=3, help='')
-    parser.add_argument('--hex_width', type=int, default=24, help='')
-    parser.add_argument('--hex_radius', type=int, default=-1, help='')
+    parser.add_argument('--hex_width', type=float, default=24, help='')
+    parser.add_argument('--hex_radius', type=float, default=-1, help='')
     parser.add_argument('--precision', type=int, default=1, help='Number of digits to store spatial location (in um), 0 for integer.')
-    parser.add_argument('--chunksize', type=int, default=100000, help='Number of lines to read at a time')
+    parser.add_argument('--chunksize', type=int, default=1000000, help='Number of lines to read at a time')
+    parser.add_argument('--xy_median', action='store_true', help='Output the median of pixel cooredinates inside each hexagon, default is to output hexagon centers exactly as lattice points')
+    parser.add_argument('--log_norm', action='store_true', help='')
+    parser.add_argument('--log_norm_size_factor', action='store_true', help='')
+    parser.add_argument('--scale_const', type=float, default=-1, help='')
+    parser.add_argument('--unit_sum_mean', type=float, default=-1, help='')
+    parser.add_argument('--debug', type=int, default=0, help='')
 
     args = parser.parse_args(_args)
-    logger = logging.getLogger(__name__)
+    if len(_args) == 0:
+        parser.print_help()
+        return
+
     if not os.path.exists(args.input):
         sys.exit("ERROR: cannot find input file.")
     if not os.path.exists(args.model):
         sys.exit("ERROR: cannot find model file.")
     if args.hex_width <= 0 and args.hex_radius <= 0:
         sys.exit("ERROR: invalid hex_width or hex_radius")
-    if not os.path.exists(os.path.dirname(args.output_pref)):
-        os.makedirs(os.path.dirname(args.output_pref))
+    if not os.path.exists(os.path.dirname(args.output)):
+        os.makedirs(os.path.dirname(args.output))
+    logging.basicConfig(level= getattr(logging, "INFO", None))
 
     ### Input
     with gzip.open(args.input, 'rt') as rf:
         header=rf.readline().strip().split('\t')
     key = args.key.lower()
     header=[x.upper() if len(x) == 1 else x.lower() for x in header]
     usecol = ['X','Y','gene',key]
@@ -55,67 +70,112 @@
     if len(miss_header) > 0:
         sys.exit(f"ERROR: {miss_header} is not in the input file")
     reader = pd.read_csv(gzip.open(args.input, 'rt'), sep='\t',\
                         chunksize=args.chunksize, skiprows=1, names=header,\
                         usecols=usecol, dtype=adt)
 
     ### Model
+    factor_header = []
     if args.model.endswith('.tsv.gz') or args.model.endswith('tsv'):
-        model_mtx = pd.read_csv(args.model, sep='\t')
-        feature_kept=list(model_mtx.gene)
-        model_mtx = np.array(model_mtx.iloc[:, 1:])
+        model_mtx = pd.read_csv(args.model, sep='\t', index_col = 0)
+        factor_header = list(model_mtx.columns)
+        feature_kept =list(model_mtx.index)
         M, K = model_mtx.shape
-        model = OnlineLDA(vocab=feature_kept,K=K,N=1e4,thread=args.thread,tol=1e-3)
-        model.init_global_parameter(model_mtx.T)
+        model = LDA(n_components=K, learning_method='online', batch_size=512, n_jobs = args.thread, verbose = 0)
+        init_latent_vars(model, n_features = M, gamma = np.array(model_mtx).T)
     else:
         try:
             model = pickle.load(open(args.model, 'rb'))
             model.n_jobs = args.thread
             feature_kept = model.feature_names_in_
             K, M = model.components_.shape
             model.feature_names_in_ = None
+            factor_header = list(np.arange(K).astype(str) )
         except:
             sys.exit("ERROR: --model must be either a tsv file containing gene name and factor-gene loadings or a pickle model object from sklearn LDA")
+    if os.path.isfile(args.feature):
+        feature = pd.read_csv(args.feature, sep='\t')
+        kept_idx = np.where(np.in1d(feature_kept, feature.gene.values))[0]
+        feature_kept = np.array(feature_kept)[kept_idx]
+        model.components_ = model.components_[:, kept_idx]
+        model.exp_dirichlet_component_ = np.exp(
+            _dirichlet_expectation_2d(model.components_)
+        )
+        M = len(feature_kept)
+
     ft_dict = {x:i for i,x in enumerate(feature_kept)}
-    logger.info(f"Model loaded with {M} features and {K} factors")
+    logging.info(f"Model loaded with {M} features and {K} factors")
 
     ### Basic parameterse
-    factor_header = [str(x) for x in range(K)]
     radius = args.hex_radius
     if radius < 0:
         radius = args.hex_width / np.sqrt(3)
-    b_size = radius * 10
+    b_size = radius * 20
+    scale_const = args.scale_const
+    unit_sum_mean = args.unit_sum_mean
+    if args.log_norm_size_factor:
+        args.log_norm = True
+    if args.log_norm:
+        if hasattr(model, 'log_norm_scaling_const_'):
+            scale_const = model.log_norm_scaling_const_
+        if scale_const < 0:
+            sys.exit("ERROR: --log_norm is specified but the normalization constant used in model fitting is unknown.")
+        if args.log_norm_size_factor:
+            if hasattr(model, 'unit_sum_mean_'):
+                unit_sum_mean = model.unit_sum_mean_
+            if unit_sum_mean < 0:
+                sys.exit("ERROR: --log_norm_size_factor is specified but the size constant used in model fitting is unknown.")
 
     # Pixel reader
     batch_obj = PixelToUnit(reader, ft_dict, key, radius,\
                 scale=1./args.mu_scale, min_ct_per_unit=args.min_ct_per_unit,\
-                sliding_step=args.n_move, major_axis=args.major_axis)
+                sliding_step=args.n_move, major_axis=args.major_axis,\
+                xy_lattice=(not args.xy_median))
 
     # Transform
     post_count = np.zeros((K, M))
     n_unit = 0
     n_batch= 0
-    oheader = ["unit",key,"x","y","topK","topP"]+factor_header
-    out_f = args.output_pref + ".fit_result.tsv.gz"
+    oheader = ["unit",key,"x","y","topK","topP"]+[str(x) for x in range(K)]
+    out_f = args.output + ".fit_result.tsv.gz"
     with gzip.open(out_f, 'wt') as wf:
         wf.write('\t'.join(oheader) + '\n')
     t0 = time.time()
+    last_batch = set()
     while batch_obj.read_chunk(min_size=b_size):
-        theta = model.transform(batch_obj.mtx)
+        if args.log_norm_size_factor:
+            rsum = batch_obj.mtx.sum(axis=1) / unit_sum_mean
+            mtx = batch_obj.mtx / rsum.reshape((-1,1))
+            mtx.data = np.log(mtx.data + 1) / scale_const
+            mtx = mtx.tocsr()
+        elif args.log_norm:
+            mtx = normalize(batch_obj.mtx, norm='l1', axis=1)
+            mtx.data = np.log(mtx.data + 1) / scale_const
+        else:
+            mtx = batch_obj.mtx
+        theta = model.transform(mtx)
         post_count += np.array(theta.T @ batch_obj.mtx)
         n_batch += 1
         n_unit  += theta.shape[0]
         t1 = time.time() - t0
         batch_obj.brc['topK'] = np.argmax(theta, axis = 1)
         batch_obj.brc['topP'] = theta.max(axis = 1)
-        batch_obj.brc = pd.concat([batch_obj.brc, pd.DataFrame(theta, columns=factor_header)], axis=1)
+        batch_obj.brc = pd.concat([batch_obj.brc, pd.DataFrame(theta, columns=[str(x) for x in range(K)] )], axis=1)
         batch_obj.brc['x'] = batch_obj.brc.x.map(lambda x : f"{x:.{args.precision}f}")
         batch_obj.brc['y'] = batch_obj.brc.y.map(lambda x : f"{x:.{args.precision}f}")
         batch_obj.brc.rename(columns = {'hex_id':'unit'}, inplace=True)
+        if len(last_batch) > 0:
+            batch_obj.brc.drop(index = batch_obj.brc.index[batch_obj.brc.unit.isin(last_batch)], inplace=True)
+        last_batch = set(batch_obj.brc.unit.values)
         batch_obj.brc[oheader].to_csv(out_f, sep='\t', index=False, header=False, float_format='%.3e', mode='a', compression={"method":"gzip"})
-        logger.info(f"Transformed {n_batch} batches with total {n_unit} units, {t1/60:2f}min")
+        logging.info(f"Transformed {n_batch} batches with total {n_unit} units, {t1/60:2f}min")
+        if (args.debug > 0) and (n_unit >= args.debug):
+            break
 
-    out_f = args.output_pref + ".posterior.count.tsv.gz"
+    out_f = args.output + ".posterior.count.tsv.gz"
     pd.concat([pd.DataFrame({'gene': feature_kept}),\
             pd.DataFrame(post_count.T, dtype='float64',\
-                            columns = [str(k) for k in range(K)])],\
+                            columns = factor_header)],\
                 axis = 1).to_csv(out_f, sep='\t', index=False, float_format='%.2f', compression={"method":"gzip"})
+
+if __name__ is '__main__':
+    transform(sys.argv[1:])
```

### Comparing `ficture-0.0.1.post3/ficture/utils/image_fn.py` & `ficture-0.0.2/ficture/utils/image_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.1.post3/ficture/utils/layout_fn.py` & `ficture-0.0.2/ficture/utils/layout_fn.py`

 * *Files identical despite different names*

### Comparing `ficture-0.0.1.post3/ficture/utils/mds_color_circle.py` & `ficture-0.0.2/ficture/utils/mds_color_circle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
 import pymde
 import numpy as np
 import matplotlib.colors
 import matplotlib.pyplot as plt
 import re, os, sys
+sys.path.append(os.path.dirname(os.path.abspath(__file__)))
 
 # A constraint class that implements the unit circle constraint
 class circle(pymde.constraints.Constraint):
     def name(self):
         return "circle"
 
     def initialization(self, n_items, embedding_dim, device=None):
@@ -37,16 +38,17 @@
         if inplace:
             Z.div_(torch.norm(Z, dim=1).unsqueeze(-1))
             return Z
         else:
             return torch.div(Z, torch.norm(Z, dim=1).unsqueeze(-1))
 
 # Map pairwise factor proximity to an unit circle embedding then to RGB colors
-def assign_color_mds_circle(mtx, cmap_name, weight=None, top_color=None):
-
+def assign_color_mds_circle(mtx, cmap_name, weight=None, top_color=None, seed=None):
+    if seed is not None:
+        pymde.seed(seed)
     # mtx is a K by K similarity/proximity matrix
     assert mtx.shape[0] == mtx.shape[1], "mtx must be square"
     K = mtx.shape[0]
     # weight is a K vector of factor abundance
     if weight is None:
         weight = np.ones(K)
     weight /= weight.sum()
```

### Comparing `ficture-0.0.1.post3/ficture/utils/visualize_factors.py` & `ficture-0.0.2/ficture/utils/visualize_factors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys, io, os, gzip, glob, copy, re, time, pickle, warnings, importlib
 import numpy as np
 import pandas as pd
 import base64
 
 from sklearn.preprocessing import normalize
+# from sklearn.decomposition import TruncatedSVD, PCA
 import scipy.cluster
 import scipy.stats
 import scipy.spatial
 import scipy.linalg
 
 import ete3
 from ete3 import Tree, TreeStyle, NodeStyle
@@ -63,31 +64,34 @@
         node[K+s] = [lvs, orgmtx[lvs, :].mean(axis = 0)]
         active_node.remove(v1)
         active_node.remove(v2)
         active_node.append(K+s)
         Z.append([ v1, v2, 1-candi[0][1], len(lvs) ])
     return Z
 
-def visual_hc(model_prob, weight, top_gene, node_color=None, circle=False, vertical=False, output_f=None, cprob_cut=.99):
+def visual_hc(model_prob, weight, top_gene, node_color=None, factor_name=None, circle=False, vertical=False, output_f=None, cprob_cut=.99):
 
     K = model_prob.shape[0]
     assert len(weight) == K, "model_prob.shape[0] != len(weight)"
     assert len(top_gene) == K, "len(top_gene) != K"
+    if factor_name is None:
+        factor_name = [str(x) for x in range(K)]
 
     model_prob = normalize(np.array(model_prob), norm='l1', axis=1)
     weight = np.array(weight)
     weight /= weight.sum()
     weight_anno = ["%.2e" % x if x < 0.1 else "%.3f" % x for x in weight]
     v = np.argsort(weight)[::-1]
     w = np.cumsum(weight[v] )
     if sum(w > cprob_cut) == 0:
         k = K - 1
     else:
         k = np.arange(K)[w > cprob_cut][0]
-    kept_factor = v[:(k+1)].astype(str)
+    kept_factor = factor_name[v[:(k+1)]]
+    kept_idx = v[:(k+1)].astype(str)
 
     # # Hierarchical clustering
     # cd_dist = scipy.spatial.distance.pdist(model_prob, metric='cosine')
     # Z_hc = scipy.cluster.hierarchy.linkage(cd_dist, method="complete")
     # Z_hc = NJ_logrank(model_prob)
 
     corlogrank = cor_logrank(model_prob)
@@ -112,17 +116,21 @@
                 ch = Tree()
                 ch.dist = c_dist
                 ch.name = str(c.id)
                 _=node_dict[node.id].add_child(ch)
                 node_dict[c.id] = ch
                 stack.append(c)
 
-    node_list = [x for x in tr.traverse() if x.is_leaf() and x.name in kept_factor]
+    node_list = [x for x in tr.traverse() if x.is_leaf() and x.name in
+    kept_idx]
     subtr = tr.copy()
     subtr.prune( [x.name for x in node_list] )
+    for x in subtr.traverse():
+        if x.is_leaf():
+            x.name = factor_name[int(x.name)]
 
     if output_f is None:
         return subtr
 
     ### Visualize tree
     title=f"Hierarchical clustering of {len(node_list)} factors"
 
@@ -134,18 +142,18 @@
     if node_color is not None:
         for n in subtr.traverse():
             if n.is_leaf():
                 nstyle = NodeStyle()
                 nstyle["fgcolor"] = node_color[n.name]
                 nstyle['size'] = 10
                 n.set_style(nstyle)
-    node_anno = {k: " " + str(k) + " ("+weight_anno[k] + "): " + v  for k,v in enumerate(top_gene) }
+    node_anno = {factor_name[k]: " " + factor_name[k] + " ("+weight_anno[k] + "): " + v  for k,v in enumerate(top_gene) }
     def layout(node):
         if node.is_leaf():
-            ete3.faces.add_face_to_node(ete3.TextFace(node_anno[int(node.name)]), node, column=0)
+            ete3.faces.add_face_to_node(ete3.TextFace(node_anno[node.name]), node, column=0)
 
     # Tree style
     ts = TreeStyle()
     ts.layout_fn=layout
     ts.show_leaf_name = False
     ts.show_branch_length = False
     ts.show_scale = False
```

### Comparing `ficture-0.0.1.post3/pyproject.toml` & `ficture-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [project]
 name = "ficture"
 description = "Segmentation free factor analysis for sub-micron resolution spatial transcriptomics"
-version = "0.0.1-3"
+version = "0.0.2"
 authors = [{name = "Yichen Si", email = "ycsi@umich.edu"}]
 license = {text = "CC BY-NC 4.0"}
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
-    "numpy", "pandas", "geopandas",
+    "numpy", "pandas",
     "scipy", "scikit-learn",
     "joblib",
     "matplotlib", "Pillow", "Jinja2", "opencv-python",
-    "shapely", "geojson",
+    "shapely", "geojson", "geopandas",
     "torch", "pymde", "ete3", "PyQt5"
 ]
 
 [project.scripts]
 ficture = "ficture.cli:main"
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
 scripts = ["*.txt", "*.rst", "*.html"]
 
 [project.urls]
-"Homepage" = "https://github.com/seqscope/ficture"
+"Homepage" = "https://seqscope.github.io/ficture/"
 "Bug Tracker" = "https://github.com/seqscope/ficture/issues"
```

