# Comparing `tmp/autobmt-0.1.9.tar.gz` & `tmp/autobmt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autobmt-0.1.9.tar", last modified: Sun Dec 10 13:41:57 2023, max compression
+gzip compressed data, was "dist/autobmt-0.2.0.tar", last modified: Thu Apr  4 10:06:38 2024, max compression
```

## Comparing `autobmt-0.1.9.tar` & `autobmt-0.2.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      292 2023-10-26 07:00:35.000000 autobmt-0.1.9/.editorconfig
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/.github/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      318 2023-10-26 07:00:35.000000 autobmt-0.1.9/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1204 2023-10-26 07:00:35.000000 autobmt-0.1.9/.gitignore
--rw-r--r--   0 ryanzheng   (501) staff       (20)      687 2023-10-26 07:00:35.000000 autobmt-0.1.9/.travis.yml
--rw-r--r--   0 ryanzheng   (501) staff       (20)     3527 2023-10-26 07:00:35.000000 autobmt-0.1.9/CONTRIBUTING.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-10-26 07:00:35.000000 autobmt-0.1.9/LICENSE
--rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-10-26 07:00:35.000000 autobmt-0.1.9/MANIFEST.in
--rw-r--r--   0 ryanzheng   (501) staff       (20)     2295 2023-10-26 07:00:35.000000 autobmt-0.1.9/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)     5009 2023-12-10 13:41:57.000000 autobmt-0.1.9/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)     3588 2023-11-14 06:53:15.000000 autobmt-0.1.9/README.md
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/autobmt/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      981 2023-12-10 13:25:40.000000 autobmt-0.1.9/autobmt/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    18328 2023-12-10 13:16:40.000000 autobmt-0.1.9/autobmt/auto_build_scorecard.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    10581 2023-11-23 01:58:14.000000 autobmt-0.1.9/autobmt/auto_build_tree_model.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    11025 2023-11-23 01:20:50.000000 autobmt-0.1.9/autobmt/auto_build_tree_model_lgb.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    13566 2023-11-18 13:03:19.000000 autobmt-0.1.9/autobmt/bayes_opt_tuner.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     3734 2023-11-14 07:57:11.000000 autobmt-0.1.9/autobmt/category_label_encoder.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     5735 2023-11-14 07:58:57.000000 autobmt-0.1.9/autobmt/category_woe_encoder.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     4234 2023-11-12 02:56:01.000000 autobmt-0.1.9/autobmt/detector.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    17099 2023-12-10 13:00:31.000000 autobmt-0.1.9/autobmt/feature_binning.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    31163 2023-12-10 13:03:05.000000 autobmt-0.1.9/autobmt/feature_selection.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)      728 2022-07-10 05:37:33.000000 autobmt-0.1.9/autobmt/logger_utils.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     6847 2023-12-07 03:47:31.000000 autobmt-0.1.9/autobmt/metrics.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    16016 2023-12-07 12:43:16.000000 autobmt-0.1.9/autobmt/plot.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    28367 2023-11-14 08:02:57.000000 autobmt-0.1.9/autobmt/report2excel.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    13959 2023-11-19 07:45:06.000000 autobmt-0.1.9/autobmt/scorecard.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    33658 2023-12-09 09:40:18.000000 autobmt-0.1.9/autobmt/statistics.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    24181 2023-11-07 06:08:47.000000 autobmt-0.1.9/autobmt/stepwise.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    22583 2023-12-10 12:51:53.000000 autobmt-0.1.9/autobmt/transformer.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    21055 2023-12-10 12:58:57.000000 autobmt-0.1.9/autobmt/utils.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/autobmt.egg-info/
--rw-r--r--   0 ryanzheng   (501) staff       (20)     5009 2023-12-10 13:41:57.000000 autobmt-0.1.9/autobmt.egg-info/PKG-INFO
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1658 2023-12-10 13:41:57.000000 autobmt-0.1.9/autobmt.egg-info/SOURCES.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-12-10 13:41:57.000000 autobmt-0.1.9/autobmt.egg-info/dependency_links.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2023-12-10 13:41:57.000000 autobmt-0.1.9/autobmt.egg-info/not-zip-safe
--rw-r--r--   0 ryanzheng   (501) staff       (20)      208 2023-12-10 13:41:57.000000 autobmt-0.1.9/autobmt.egg-info/requires.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)        8 2023-12-10 13:41:57.000000 autobmt-0.1.9/autobmt.egg-info/top_level.txt
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/docs/
--rw-r--r--   0 ryanzheng   (501) staff       (20)      608 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/Makefile
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/authors.rst
--rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4769 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/conf.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/contributing.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/history.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      304 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/index.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1118 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/installation.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)      805 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/make.bat
--rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/readme.rst
--rw-r--r--   0 ryanzheng   (501) staff       (20)       69 2023-10-26 07:00:35.000000 autobmt-0.1.9/docs/usage.rst
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/examples/
--rw-r--r--   0 ryanzheng   (501) staff       (20)     4345 2023-11-19 07:15:17.000000 autobmt-0.1.9/examples/autobmt_lr_tutorial_code.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     4574 2023-11-26 01:46:48.000000 autobmt-0.1.9/examples/autobmt_treemodel_tutorial_code.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     4591 2023-11-26 01:46:55.000000 autobmt-0.1.9/examples/autobmt_treemodel_tutorial_code_LGB.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)   687290 2023-12-07 13:48:29.000000 autobmt-0.1.9/examples/tutorial_code.ipynb
--rw-r--r--   0 ryanzheng   (501) staff       (20)      210 2023-12-07 06:45:34.000000 autobmt-0.1.9/requirements.txt
--rw-r--r--   0 ryanzheng   (501) staff       (20)      132 2023-12-10 13:41:57.000000 autobmt-0.1.9/setup.cfg
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1729 2023-11-12 11:03:04.000000 autobmt-0.1.9/setup.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/tests/
--rw-r--r--   0 ryanzheng   (501) staff       (20)     8196 2023-12-06 06:54:17.000000 autobmt-0.1.9/tests/.DS_Store
--rw-r--r--   0 ryanzheng   (501) staff       (20)       37 2023-10-26 07:00:35.000000 autobmt-0.1.9/tests/__init__.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    13520 2023-11-12 02:26:28.000000 autobmt-0.1.9/tests/feature_binning_test.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)    13279 2023-12-10 13:22:28.000000 autobmt-0.1.9/tests/feature_selection_test.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1462 2023-11-12 02:26:17.000000 autobmt-0.1.9/tests/metrics_test.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1733 2023-11-12 02:26:13.000000 autobmt-0.1.9/tests/plot_test.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     6638 2023-12-08 04:13:50.000000 autobmt-0.1.9/tests/scorecard_test.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     1044 2023-12-10 13:22:21.000000 autobmt-0.1.9/tests/statistics_mr_auc_ks_test.py
--rw-r--r--   0 ryanzheng   (501) staff       (20)     2943 2023-11-12 02:31:20.000000 autobmt-0.1.9/tests/statistics_test.py
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/tests/tests/
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/tests/tests/polt_bin_summary/
--rw-r--r--   0 ryanzheng   (501) staff       (20)  1125124 2023-12-09 10:24:35.000000 autobmt-0.1.9/tests/tests/polt_bin_summary/plot_var_bin_summary.xlsx
-drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2023-12-10 13:41:57.000000 autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/
--rw-r--r--   0 ryanzheng   (501) staff       (20)   347395 2023-12-09 10:24:25.000000 autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/A.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)   300146 2023-12-09 10:24:27.000000 autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/B.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)   118153 2023-12-09 10:24:29.000000 autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/C.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)   396276 2023-12-09 10:24:32.000000 autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/D.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)   125695 2023-12-09 10:24:34.000000 autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/type.png
--rw-r--r--   0 ryanzheng   (501) staff       (20)     5277 2023-12-10 13:01:45.000000 autobmt-0.1.9/tests/transformer_test.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      292 2023-10-26 07:00:35.000000 autobmt-0.2.0/.editorconfig
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/.github/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      318 2023-10-26 07:00:35.000000 autobmt-0.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1204 2023-10-26 07:00:35.000000 autobmt-0.2.0/.gitignore
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      687 2023-10-26 07:00:35.000000 autobmt-0.2.0/.travis.yml
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     3527 2023-10-26 07:00:35.000000 autobmt-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1068 2023-10-26 07:00:35.000000 autobmt-0.2.0/LICENSE
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      262 2023-10-26 07:00:35.000000 autobmt-0.2.0/MANIFEST.in
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     2295 2023-10-26 07:00:35.000000 autobmt-0.2.0/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     5009 2024-04-04 10:06:38.000000 autobmt-0.2.0/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     3588 2024-04-04 07:27:08.000000 autobmt-0.2.0/README.md
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/autobmt/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      981 2024-04-04 07:30:30.000000 autobmt-0.2.0/autobmt/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    18328 2023-12-10 13:16:40.000000 autobmt-0.2.0/autobmt/auto_build_scorecard.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    10581 2023-11-23 01:58:14.000000 autobmt-0.2.0/autobmt/auto_build_tree_model.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    11025 2023-11-23 01:20:50.000000 autobmt-0.2.0/autobmt/auto_build_tree_model_lgb.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    13566 2023-11-18 13:03:19.000000 autobmt-0.2.0/autobmt/bayes_opt_tuner.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     3734 2023-11-14 07:57:11.000000 autobmt-0.2.0/autobmt/category_label_encoder.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     5735 2023-11-14 07:58:57.000000 autobmt-0.2.0/autobmt/category_woe_encoder.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     4234 2023-11-12 02:56:01.000000 autobmt-0.2.0/autobmt/detector.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    17099 2023-12-10 13:00:31.000000 autobmt-0.2.0/autobmt/feature_binning.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    31163 2023-12-10 13:03:05.000000 autobmt-0.2.0/autobmt/feature_selection.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      728 2022-07-10 05:37:33.000000 autobmt-0.2.0/autobmt/logger_utils.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     6847 2023-12-07 03:47:31.000000 autobmt-0.2.0/autobmt/metrics.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    16016 2023-12-07 12:43:16.000000 autobmt-0.2.0/autobmt/plot.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    28367 2023-11-14 08:02:57.000000 autobmt-0.2.0/autobmt/report2excel.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    13959 2023-11-19 07:45:06.000000 autobmt-0.2.0/autobmt/scorecard.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    33519 2024-04-04 07:16:58.000000 autobmt-0.2.0/autobmt/statistics.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    24138 2024-04-04 07:17:26.000000 autobmt-0.2.0/autobmt/stepwise.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    22583 2023-12-10 12:51:53.000000 autobmt-0.2.0/autobmt/transformer.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    21055 2023-12-10 12:58:57.000000 autobmt-0.2.0/autobmt/utils.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/autobmt.egg-info/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     5009 2024-04-04 10:06:38.000000 autobmt-0.2.0/autobmt.egg-info/PKG-INFO
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1658 2024-04-04 10:06:38.000000 autobmt-0.2.0/autobmt.egg-info/SOURCES.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2024-04-04 10:06:38.000000 autobmt-0.2.0/autobmt.egg-info/dependency_links.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        1 2024-04-04 10:06:38.000000 autobmt-0.2.0/autobmt.egg-info/not-zip-safe
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      208 2024-04-04 10:06:38.000000 autobmt-0.2.0/autobmt.egg-info/requires.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)        8 2024-04-04 10:06:38.000000 autobmt-0.2.0/autobmt.egg-info/top_level.txt
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/docs/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      608 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/Makefile
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/authors.rst
+-rwxr-xr-x   0 ryanzheng   (501) staff       (20)     4769 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/conf.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       33 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/contributing.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       28 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/history.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      304 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/index.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1118 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/installation.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      805 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/make.bat
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       27 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/readme.rst
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       69 2023-10-26 07:00:35.000000 autobmt-0.2.0/docs/usage.rst
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/examples/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     4345 2023-11-19 07:15:17.000000 autobmt-0.2.0/examples/autobmt_lr_tutorial_code.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     4574 2023-11-26 01:46:48.000000 autobmt-0.2.0/examples/autobmt_treemodel_tutorial_code.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     4591 2023-11-26 01:46:55.000000 autobmt-0.2.0/examples/autobmt_treemodel_tutorial_code_LGB.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   687290 2023-12-07 13:48:29.000000 autobmt-0.2.0/examples/tutorial_code.ipynb
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      210 2023-12-07 06:45:34.000000 autobmt-0.2.0/requirements.txt
+-rw-r--r--   0 ryanzheng   (501) staff       (20)      132 2024-04-04 10:06:38.000000 autobmt-0.2.0/setup.cfg
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1729 2023-11-12 11:03:04.000000 autobmt-0.2.0/setup.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/tests/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     8196 2023-12-06 06:54:17.000000 autobmt-0.2.0/tests/.DS_Store
+-rw-r--r--   0 ryanzheng   (501) staff       (20)       37 2023-10-26 07:00:35.000000 autobmt-0.2.0/tests/__init__.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    13520 2023-11-12 02:26:28.000000 autobmt-0.2.0/tests/feature_binning_test.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)    13279 2023-12-10 13:22:28.000000 autobmt-0.2.0/tests/feature_selection_test.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1462 2023-11-12 02:26:17.000000 autobmt-0.2.0/tests/metrics_test.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1733 2023-11-12 02:26:13.000000 autobmt-0.2.0/tests/plot_test.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     6638 2023-12-08 04:13:50.000000 autobmt-0.2.0/tests/scorecard_test.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     1044 2023-12-10 13:22:21.000000 autobmt-0.2.0/tests/statistics_mr_auc_ks_test.py
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     2943 2023-11-12 02:31:20.000000 autobmt-0.2.0/tests/statistics_test.py
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/tests/tests/
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/tests/tests/polt_bin_summary/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)  1125124 2023-12-09 10:24:35.000000 autobmt-0.2.0/tests/tests/polt_bin_summary/plot_var_bin_summary.xlsx
+drwxr-xr-x   0 ryanzheng   (501) staff       (20)        0 2024-04-04 10:06:38.000000 autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   347395 2023-12-09 10:24:25.000000 autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/A.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   300146 2023-12-09 10:24:27.000000 autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/B.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   118153 2023-12-09 10:24:29.000000 autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/C.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   396276 2023-12-09 10:24:32.000000 autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/D.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)   125695 2023-12-09 10:24:34.000000 autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/type.png
+-rw-r--r--   0 ryanzheng   (501) staff       (20)     5277 2023-12-10 13:01:45.000000 autobmt-0.2.0/tests/transformer_test.py
```

### Comparing `autobmt-0.1.9/.gitignore` & `autobmt-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/.travis.yml` & `autobmt-0.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/CONTRIBUTING.rst` & `autobmt-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/LICENSE` & `autobmt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/Makefile` & `autobmt-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/PKG-INFO` & `autobmt-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: autobmt
-Version: 0.1.9
+Version: 0.2.0
 Summary: a modeling tool that automatically builds scorecards and tree models.
 Home-page: https://github.com/ZhengRyan/autobmt
 Author: RyanZheng
 Author-email: zhengruiping000@163.com
 License: MIT license
 Description: ##自动构建评分卡
         
@@ -14,15 +14,15 @@
         | :---: | :----: |
         | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
         |  干饭人  | 魔都数据干饭人 |
         
         
         > 仓库地址：https://github.com/ZhengRyan/autobmt
         > 
-        > 微信公众号文章：https://mp.weixin.qq.com/s/u8Nsp5M93WIGL2M0tU4U_g
+        > 微信公众号文章：https://mp.weixin.qq.com/s/30-V0p30p1rKSBtcBgLTRA
         > 
         > pipy包：https://pypi.org/project/autobmt/
         > 
         > 实验数据：链接: https://pan.baidu.com/s/1BRIHH9Wcwy2EZaO5xSgH9w?pwd=tdq5 提取码: tdq5
         
         ## 一、环境准备
         可以不用单独创建虚拟环境，都是日常常用的python依赖包。需要创建虚拟环境，请参考"五、依赖包安装"
```

### Comparing `autobmt-0.1.9/README.md` & `autobmt-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 | :---: | :----: |
 | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
 |  干饭人  | 魔都数据干饭人 |
 
 
 > 仓库地址：https://github.com/ZhengRyan/autobmt
 > 
-> 微信公众号文章：https://mp.weixin.qq.com/s/u8Nsp5M93WIGL2M0tU4U_g
+> 微信公众号文章：https://mp.weixin.qq.com/s/30-V0p30p1rKSBtcBgLTRA
 > 
 > pipy包：https://pypi.org/project/autobmt/
 > 
 > 实验数据：链接: https://pan.baidu.com/s/1BRIHH9Wcwy2EZaO5xSgH9w?pwd=tdq5 提取码: tdq5
 
 ## 一、环境准备
 可以不用单独创建虚拟环境，都是日常常用的python依赖包。需要创建虚拟环境，请参考"五、依赖包安装"
```

### Comparing `autobmt-0.1.9/autobmt/__init__.py` & `autobmt-0.2.0/autobmt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 from .metrics import psi, get_auc_ks_psi, get_auc, get_ks
 from .utils import del_df, dump_to_pkl, load_from_pkl, fea_woe_dict_format, to_score
 from .logger_utils import Logger
 from .scorecard import ScoreCard
 from .bayes_opt_tuner import classifiers_model_auto_tune_params
 from .plot import plot_var_bin_summary
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
 VERSION = __version__
```

### Comparing `autobmt-0.1.9/autobmt/auto_build_scorecard.py` & `autobmt-0.2.0/autobmt/auto_build_scorecard.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/auto_build_tree_model.py` & `autobmt-0.2.0/autobmt/auto_build_tree_model.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/auto_build_tree_model_lgb.py` & `autobmt-0.2.0/autobmt/auto_build_tree_model_lgb.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/bayes_opt_tuner.py` & `autobmt-0.2.0/autobmt/bayes_opt_tuner.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/category_label_encoder.py` & `autobmt-0.2.0/autobmt/category_label_encoder.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/category_woe_encoder.py` & `autobmt-0.2.0/autobmt/category_woe_encoder.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/detector.py` & `autobmt-0.2.0/autobmt/detector.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/feature_binning.py` & `autobmt-0.2.0/autobmt/feature_binning.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/feature_selection.py` & `autobmt-0.2.0/autobmt/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/logger_utils.py` & `autobmt-0.2.0/autobmt/logger_utils.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/metrics.py` & `autobmt-0.2.0/autobmt/metrics.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/plot.py` & `autobmt-0.2.0/autobmt/plot.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/report2excel.py` & `autobmt-0.2.0/autobmt/report2excel.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/scorecard.py` & `autobmt-0.2.0/autobmt/scorecard.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/statistics.py` & `autobmt-0.2.0/autobmt/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -554,16 +554,14 @@
 from pandas.core.groupby import Grouper
 from pandas.core.indexes.api import Index
 import warnings
 
 is_scalar = lib.is_scalar
 
 warnings.filterwarnings('ignore')
-pd.set_option('display.max_rows', None)  # 设置行数为无限制
-pd.set_option('display.max_columns', None)  # 设置列数为无限制
 
 
 def _convert_by(by):
     if by is None:
         by = []
     elif (
         is_scalar(by)
```

### Comparing `autobmt-0.1.9/autobmt/stepwise.py` & `autobmt-0.2.0/autobmt/stepwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from .metrics import get_auc, get_ks, AIC, BIC, MSE
 from .utils import split_target, unpack_tuple, step_evaluate_models, \
     get_max_corr_feature, model_predict_evaluate
 
 INTERCEPT_COLS = 'intercept'
 
 warnings.filterwarnings(action='ignore')
-pd.set_option('display.max_columns', None)
 log = Logger(level="info", name=__name__).logger
 
 
 class StatsModel:
     def __init__(self, estimator='ols', criterion='aic', intercept=False):
         if isinstance(estimator, str):
             Est = self.get_estimator(estimator)
```

### Comparing `autobmt-0.1.9/autobmt/transformer.py` & `autobmt-0.2.0/autobmt/transformer.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt/utils.py` & `autobmt-0.2.0/autobmt/utils.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/autobmt.egg-info/PKG-INFO` & `autobmt-0.2.0/autobmt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: autobmt
-Version: 0.1.9
+Version: 0.2.0
 Summary: a modeling tool that automatically builds scorecards and tree models.
 Home-page: https://github.com/ZhengRyan/autobmt
 Author: RyanZheng
 Author-email: zhengruiping000@163.com
 License: MIT license
 Description: ##自动构建评分卡
         
@@ -14,15 +14,15 @@
         | :---: | :----: |
         | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="RyanZheng.png" width="50%" border=0/> | <img src="https://github.com/ZhengRyan/autotreemodel/blob/master/images/%E9%AD%94%E9%83%BD%E6%95%B0%E6%8D%AE%E5%B9%B2%E9%A5%AD%E4%BA%BA.png" alt="魔都数据干饭人.png" width="50%" border=0/> |
         |  干饭人  | 魔都数据干饭人 |
         
         
         > 仓库地址：https://github.com/ZhengRyan/autobmt
         > 
-        > 微信公众号文章：https://mp.weixin.qq.com/s/u8Nsp5M93WIGL2M0tU4U_g
+        > 微信公众号文章：https://mp.weixin.qq.com/s/30-V0p30p1rKSBtcBgLTRA
         > 
         > pipy包：https://pypi.org/project/autobmt/
         > 
         > 实验数据：链接: https://pan.baidu.com/s/1BRIHH9Wcwy2EZaO5xSgH9w?pwd=tdq5 提取码: tdq5
         
         ## 一、环境准备
         可以不用单独创建虚拟环境，都是日常常用的python依赖包。需要创建虚拟环境，请参考"五、依赖包安装"
```

### Comparing `autobmt-0.1.9/autobmt.egg-info/SOURCES.txt` & `autobmt-0.2.0/autobmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/docs/Makefile` & `autobmt-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/docs/conf.py` & `autobmt-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/docs/installation.rst` & `autobmt-0.2.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/docs/make.bat` & `autobmt-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/examples/autobmt_lr_tutorial_code.py` & `autobmt-0.2.0/examples/autobmt_lr_tutorial_code.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/examples/autobmt_treemodel_tutorial_code.py` & `autobmt-0.2.0/examples/autobmt_treemodel_tutorial_code.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/examples/autobmt_treemodel_tutorial_code_LGB.py` & `autobmt-0.2.0/examples/autobmt_treemodel_tutorial_code_LGB.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/examples/tutorial_code.ipynb` & `autobmt-0.2.0/examples/tutorial_code.ipynb`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/setup.py` & `autobmt-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/.DS_Store` & `autobmt-0.2.0/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/feature_binning_test.py` & `autobmt-0.2.0/tests/feature_binning_test.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/feature_selection_test.py` & `autobmt-0.2.0/tests/feature_selection_test.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/metrics_test.py` & `autobmt-0.2.0/tests/metrics_test.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/plot_test.py` & `autobmt-0.2.0/tests/plot_test.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/scorecard_test.py` & `autobmt-0.2.0/tests/scorecard_test.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/statistics_mr_auc_ks_test.py` & `autobmt-0.2.0/tests/statistics_mr_auc_ks_test.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/statistics_test.py` & `autobmt-0.2.0/tests/statistics_test.py`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/tests/polt_bin_summary/plot_var_bin_summary.xlsx` & `autobmt-0.2.0/tests/tests/polt_bin_summary/plot_var_bin_summary.xlsx`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/A.png` & `autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/A.png`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/B.png` & `autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/B.png`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/C.png` & `autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/C.png`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/D.png` & `autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/D.png`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/tests/polt_bin_summary/var_jpg/type.png` & `autobmt-0.2.0/tests/tests/polt_bin_summary/var_jpg/type.png`

 * *Files identical despite different names*

### Comparing `autobmt-0.1.9/tests/transformer_test.py` & `autobmt-0.2.0/tests/transformer_test.py`

 * *Files identical despite different names*

