# Comparing `tmp/countess-0.0.56.tar.gz` & `tmp/countess-0.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countess-0.0.56.tar", last modified: Wed Apr  3 05:26:15 2024, max compression
+gzip compressed data, was "countess-0.0.57.tar", last modified: Thu Apr  4 09:44:33 2024, max compression
```

## Comparing `countess-0.0.56.tar` & `countess-0.0.57.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/
--rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.56/LICENSE.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.56/MANIFEST.in
--rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-03 05:26:15.267245 countess-0.0.56/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-03 05:25:56.000000 countess-0.0.56/README.md
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.263245 countess-0.0.56/countess/
--rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-03 05:25:56.000000 countess-0.0.56/countess/__init__.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.263245 countess-0.0.56/countess/core/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.56/countess/core/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.56/countess/core/cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-03 00:27:43.000000 countess-0.0.56/countess/core/config.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.56/countess/core/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    19161 2024-04-03 00:27:43.000000 countess-0.0.56/countess/core/parameters.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-03 05:16:18.000000 countess-0.0.56/countess/core/pipeline.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-03 05:16:18.000000 countess-0.0.56/countess/core/plugins.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.263245 countess-0.0.56/countess/gui/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.56/countess/gui/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    18458 2024-04-03 05:18:33.000000 countess-0.0.56/countess/gui/config.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.263245 countess-0.0.56/countess/gui/icons/
--rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/add.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/check.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/del.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/hbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/info.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/redbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/sort_dn.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/sort_un.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/sort_up.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/uncheck.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/icons/vbar.gif
--rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/logger.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    20088 2024-04-03 05:16:18.000000 countess-0.0.56/countess/gui/main.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-03 00:27:43.000000 countess-0.0.56/countess/gui/mini_browser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    15188 2024-04-03 00:42:47.000000 countess-0.0.56/countess/gui/tabular.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-03 01:42:58.000000 countess-0.0.56/countess/gui/tree.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3565 2024-04-03 05:15:43.000000 countess-0.0.56/countess/gui/widgets.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/countess/plugins/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.56/countess/plugins/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/collate.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/column.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/correlation.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/csv.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/data_table.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/expression.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-03 00:27:43.000000 countess-0.0.56/countess/plugins/fastq.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/group_by.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/hgvs_parser.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/join.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.56/countess/plugins/mutagenize.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3660 2024-04-03 00:44:33.000000 countess-0.0.56/countess/plugins/pivot.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.56/countess/plugins/python.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/regex.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/sequence.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     3705 2024-04-03 05:16:18.000000 countess-0.0.56/countess/plugins/variant.py
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.56/countess/py.typed
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/countess/utils/
--rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.56/countess/utils/__init__.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.56/countess/utils/pandas.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.56/countess/utils/parallel.py
--rw-rw-r--   0 nick      (1000) nick      (1000)    17825 2024-04-03 00:27:43.000000 countess-0.0.56/countess/utils/variant.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/countess.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/PKG-INFO
--rw-rw-r--   0 nick      (1000) nick      (1000)     1619 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/SOURCES.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/dependency_links.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/entry_points.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/requires.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-03 05:26:15.000000 countess-0.0.56/countess.egg-info/top_level.txt
--rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-03 00:27:43.000000 countess-0.0.56/pyproject.toml
--rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-03 05:26:15.267245 countess-0.0.56/setup.cfg
--rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.56/setup.py
-drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-03 05:26:15.267245 countess-0.0.56/tests/
--rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-03 00:27:43.000000 countess-0.0.56/tests/test_cmd.py
--rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-03 00:27:43.000000 countess-0.0.56/tests/test_gui.py
--rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.56/tests/test_plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1470 2023-10-25 21:13:29.000000 countess-0.0.57/LICENSE.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)       59 2024-04-03 00:27:43.000000 countess-0.0.57/MANIFEST.in
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-04 09:44:33.957883 countess-0.0.57/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)      723 2024-04-04 09:42:41.000000 countess-0.0.57/README.md
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.949883 countess-0.0.57/countess/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       43 2024-04-04 09:42:41.000000 countess-0.0.57/countess/__init__.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.949883 countess-0.0.57/countess/core/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:48:22.000000 countess-0.0.57/countess/core/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      466 2024-04-03 00:27:43.000000 countess-0.0.57/countess/core/cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4764 2024-04-03 00:27:43.000000 countess-0.0.57/countess/core/config.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2799 2023-11-09 02:30:05.000000 countess-0.0.57/countess/core/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    19161 2024-04-03 00:27:43.000000 countess-0.0.57/countess/core/parameters.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    13908 2024-04-03 05:16:18.000000 countess-0.0.57/countess/core/pipeline.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    25925 2024-04-03 05:16:18.000000 countess-0.0.57/countess/core/plugins.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.953883 countess-0.0.57/countess/gui/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.57/countess/gui/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18458 2024-04-03 05:18:33.000000 countess-0.0.57/countess/gui/config.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.953883 countess-0.0.57/countess/gui/icons/
+-rw-rw-r--   0 nick      (1000) nick      (1000)       90 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/add.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/check.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       98 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/del.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       62 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/hbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/info.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/redbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       84 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/sort_dn.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       86 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/sort_un.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/sort_up.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       88 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/uncheck.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)       71 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/icons/vbar.gif
+-rw-rw-r--   0 nick      (1000) nick      (1000)     5105 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/logger.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    20088 2024-04-04 09:42:21.000000 countess-0.0.57/countess/gui/main.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1730 2024-04-03 00:27:43.000000 countess-0.0.57/countess/gui/mini_browser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    15188 2024-04-03 00:42:47.000000 countess-0.0.57/countess/gui/tabular.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    23070 2024-04-03 01:42:58.000000 countess-0.0.57/countess/gui/tree.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3565 2024-04-03 05:15:43.000000 countess-0.0.57/countess/gui/widgets.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/countess/plugins/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2023-05-25 01:44:18.000000 countess-0.0.57/countess/plugins/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2402 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/collate.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2116 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/column.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2245 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/correlation.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     7274 2024-04-03 23:13:30.000000 countess-0.0.57/countess/plugins/csv.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3844 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/data_table.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1842 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/expression.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2938 2024-04-03 00:27:43.000000 countess-0.0.57/countess/plugins/fastq.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4735 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/group_by.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3339 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/hgvs_parser.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     4541 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/join.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3348 2023-11-28 03:30:23.000000 countess-0.0.57/countess/plugins/mutagenize.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3660 2024-04-03 23:55:53.000000 countess-0.0.57/countess/plugins/pivot.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2977 2024-04-03 00:27:43.000000 countess-0.0.57/countess/plugins/python.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     6758 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/regex.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1902 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/sequence.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3705 2024-04-03 05:16:18.000000 countess-0.0.57/countess/plugins/variant.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-08-11 05:39:01.000000 countess-0.0.57/countess/py.typed
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/countess/utils/
+-rw-rw-r--   0 nick      (1000) nick      (1000)        0 2022-09-26 22:30:04.000000 countess-0.0.57/countess/utils/__init__.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2768 2024-03-14 02:50:26.000000 countess-0.0.57/countess/utils/pandas.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     2996 2024-04-03 00:27:43.000000 countess-0.0.57/countess/utils/parallel.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)    18145 2024-04-04 01:40:39.000000 countess-0.0.57/countess/utils/variant.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/countess.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     2050 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/PKG-INFO
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1619 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/SOURCES.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        1 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/dependency_links.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1056 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/entry_points.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)      310 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/requires.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)        9 2024-04-04 09:44:33.000000 countess-0.0.57/countess.egg-info/top_level.txt
+-rw-rw-r--   0 nick      (1000) nick      (1000)     3236 2024-04-03 00:27:43.000000 countess-0.0.57/pyproject.toml
+-rw-rw-r--   0 nick      (1000) nick      (1000)       38 2024-04-04 09:44:33.957883 countess-0.0.57/setup.cfg
+-rw-rw-r--   0 nick      (1000) nick      (1000)       39 2023-05-25 01:44:18.000000 countess-0.0.57/setup.py
+drwxrwxr-x   0 nick      (1000) nick      (1000)        0 2024-04-04 09:44:33.957883 countess-0.0.57/tests/
+-rw-rw-r--   0 nick      (1000) nick      (1000)      476 2024-04-03 00:27:43.000000 countess-0.0.57/tests/test_cmd.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)      498 2024-04-03 00:27:43.000000 countess-0.0.57/tests/test_gui.py
+-rw-rw-r--   0 nick      (1000) nick      (1000)     1060 2023-11-09 02:44:32.000000 countess-0.0.57/tests/test_plugins.py
```

### Comparing `countess-0.0.56/LICENSE.txt` & `countess-0.0.57/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/PKG-INFO` & `countess-0.0.57/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.56
+Version: 0.0.57
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.56
+# CountESS 0.0.57
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.56/README.md` & `countess-0.0.57/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# CountESS 0.0.56
+# CountESS 0.0.57
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.56/countess/core/config.py` & `countess-0.0.57/countess/core/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/core/logger.py` & `countess-0.0.57/countess/core/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/core/parameters.py` & `countess-0.0.57/countess/core/parameters.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/core/pipeline.py` & `countess-0.0.57/countess/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/core/plugins.py` & `countess-0.0.57/countess/core/plugins.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/gui/config.py` & `countess-0.0.57/countess/gui/config.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/gui/logger.py` & `countess-0.0.57/countess/gui/logger.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/gui/main.py` & `countess-0.0.57/countess/gui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             )
             if self.node.plugin.link:
                 info_button(self.frame, command=self.on_info_button_press).place(anchor=tk.NE, relx=1, y=50)
             # self.node.prepare(self.logger)
             # self.node.plugin.update()
             self.configurator = PluginConfigurator(self.config_canvas, self.node.plugin, self.config_change_callback)
             self.config_subframe = self.configurator.frame
-            self.frame.rowconfigure(3, weight=1, minsize=self.frame.winfo_height() / 2)
+            self.frame.rowconfigure(3, weight=1, minsize=self.frame.winfo_height() / 3)
 
         else:
             has_parents = len(self.node.parent_nodes) > 0
             has_children = len(self.node.child_nodes) > 0
             self.config_subframe = PluginChooserFrame(
                 self.config_canvas, "Choose Plugin", self.choose_plugin, has_parents, has_children
             )
```

### Comparing `countess-0.0.56/countess/gui/mini_browser.py` & `countess-0.0.57/countess/gui/mini_browser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/gui/tabular.py` & `countess-0.0.57/countess/gui/tabular.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/gui/tree.py` & `countess-0.0.57/countess/gui/tree.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/gui/widgets.py` & `countess-0.0.57/countess/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/collate.py` & `countess-0.0.57/countess/plugins/collate.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/column.py` & `countess-0.0.57/countess/plugins/column.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/correlation.py` & `countess-0.0.57/countess/plugins/correlation.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/csv.py` & `countess-0.0.57/countess/plugins/csv.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/data_table.py` & `countess-0.0.57/countess/plugins/data_table.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/expression.py` & `countess-0.0.57/countess/plugins/expression.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/fastq.py` & `countess-0.0.57/countess/plugins/fastq.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/group_by.py` & `countess-0.0.57/countess/plugins/group_by.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/hgvs_parser.py` & `countess-0.0.57/countess/plugins/hgvs_parser.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/join.py` & `countess-0.0.57/countess/plugins/join.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/mutagenize.py` & `countess-0.0.57/countess/plugins/mutagenize.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/pivot.py` & `countess-0.0.57/countess/plugins/pivot.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/python.py` & `countess-0.0.57/countess/plugins/python.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/regex.py` & `countess-0.0.57/countess/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/sequence.py` & `countess-0.0.57/countess/plugins/sequence.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/plugins/variant.py` & `countess-0.0.57/countess/plugins/variant.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/utils/pandas.py` & `countess-0.0.57/countess/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/utils/parallel.py` & `countess-0.0.57/countess/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess/utils/variant.py` & `countess-0.0.57/countess/utils/variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,14 +349,17 @@
     ['Ser4extLysGln']
 
     Protein calling should stop at the first Ter encountered:
 
     >>> list(find_variant_protein("ATGGTTGGTTCA", "ATGGTTTAGACA"))
     ['Gly3Ter']
 
+    >>> list(find_variant_protein("ATGGTTTGGTAG", "ATGGTTTAGTAG"))
+    ['Trp3Ter']
+
     Offset lets you set the frame offset (0, 1 or 2, practically)
 
     """
 
     ref_seq = ref_seq.strip().upper()
     var_seq = var_seq.strip().upper()
 
@@ -383,14 +386,19 @@
     for opcode in opcodes:
         src_start, src_end = opcode.src_start, opcode.src_end
         src_pro = ref_pro[src_start:src_end]
         dest_pro = var_pro[opcode.dest_start : opcode.dest_end]
 
         if opcode.tag == "delete":
             assert dest_pro == ""
+            if ref_pro[src_end] == '*':
+                # if the codon just after this deletion is a terminator,
+                # consider this an early termination.
+                yield f"{_ref(src_start)}Ter"
+                return
             if len(src_pro) == 1:
                 yield f"{_ref(src_start)}del"
             else:
                 yield f"{_ref(src_start)}_{_ref(src_end-1)}del"
 
         elif opcode.tag == "insert":
             assert src_pro == ""
```

### Comparing `countess-0.0.56/countess.egg-info/PKG-INFO` & `countess-0.0.57/countess.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: countess
-Version: 0.0.56
+Version: 0.0.57
 Summary: CountESS
 Author-email: Nick Moore <nick@zoic.org>, Alan Rubin <alan@rubin.id.au>
 Maintainer-email: Nick Moore <nick@zoic.org>
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,15 @@
 Requires-Dist: pylint~=2.17; extra == "dev"
 Requires-Dist: types-psutil~=5.9.5; extra == "dev"
 Requires-Dist: types-ttkthemes~=3.2; extra == "dev"
 Requires-Dist: twine==4.0.2; extra == "dev"
 Requires-Dist: pandas-stubs~=2.1.0; extra == "dev"
 Requires-Dist: pytest~=7.2; extra == "dev"
 
-# CountESS 0.0.56
+# CountESS 0.0.57
 
 This is CountESS, a modular, Python 3 reimplementation of Enrich2.
 
 ## License
 
 BSD 3-clause.  See [LICENSE.txt](LICENSE.txt)
```

### Comparing `countess-0.0.56/countess.egg-info/SOURCES.txt` & `countess-0.0.57/countess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/countess.egg-info/entry_points.txt` & `countess-0.0.57/countess.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/pyproject.toml` & `countess-0.0.57/pyproject.toml`

 * *Files identical despite different names*

### Comparing `countess-0.0.56/tests/test_plugins.py` & `countess-0.0.57/tests/test_plugins.py`

 * *Files identical despite different names*

