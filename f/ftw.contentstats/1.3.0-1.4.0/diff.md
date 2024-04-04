# Comparing `tmp/ftw.contentstats-1.3.0.tar.gz` & `tmp/ftw.contentstats-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ftw.contentstats-1.3.0.tar", last modified: Tue Apr  4 12:51:12 2023, max compression
+gzip compressed data, was "ftw.contentstats-1.4.0.tar", last modified: Thu Apr  4 11:42:19 2024, max compression
```

## Comparing `ftw.contentstats-1.3.0.tar` & `ftw.contentstats-1.4.0.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/
--rw-r--r--   0 lukasgraf   (501) staff       (20)     7103 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/PKG-INFO
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/demo/
--rw-r--r--   0 lukasgraf   (501) staff       (20)      255 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/demo/configure.zcml
--rw-r--r--   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/demo/__init__.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      912 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/demo/filters.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1361 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/interfaces.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2328 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/console.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      852 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/configure.zcml
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/providers/
--rw-r--r--   0 lukasgraf   (501) staff       (20)      554 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/providers/configure.zcml
--rw-r--r--   0 lukasgraf   (501) staff       (20)     4395 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/providers/perf_metrics.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/providers/__init__.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1888 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/providers/review_states.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1683 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/providers/disk_usage.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1831 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/providers/portal_types.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1469 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_disk_usage_provider.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2946 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_dump_stats_view.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      290 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_uninstall.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2708 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_stats.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1746 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_review_state_provider.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     3064 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_content_stats_view.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1549 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_portal_types_provider.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1504 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/__init__.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2754 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_perf_metrics_provider.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     5542 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_disk_usage.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      409 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_profiles.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/assets/
--rw-r--r--   0 lukasgraf   (501) staff       (20)      308 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/assets/disk-usage.json
--rw-r--r--   0 lukasgraf   (501) staff       (20)      305 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/assets/__init__.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     8377 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/tests/test_logger.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      129 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/__init__.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     3162 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/logger.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/Extensions/
--rw-r--r--   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/Extensions/__init__.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      250 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/Extensions/install.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/
--rw-r--r--   0 lukasgraf   (501) staff       (20)      895 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/configure.zcml
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1834 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/content-stats.js
--rw-r--r--   0 lukasgraf   (501) staff       (20)   151725 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/d3.v3.min.js
--rw-r--r--   0 lukasgraf   (501) staff       (20)   180227 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/c3.min.js
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2043 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/c3.min.css
--rw-r--r--   0 lukasgraf   (501) staff       (20)      435 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/content-stats.css
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1051 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/dump_stats.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/__init__.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/templates/
--rw-r--r--   0 lukasgraf   (501) staff       (20)     3079 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/templates/content_stats.pt
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2056 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/browser/content_stats.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1891 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/utils.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     3094 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/stats.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)     6341 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/disk_usage.py
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/profiles/
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/profiles/default/
--rwxr-xr-x   0 lukasgraf   (501) staff       (20)       73 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/profiles/default/metadata.xml
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/profiles/uninstall/
--rw-r--r--   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/profiles/uninstall/.gitkeep
--rw-r--r--   0 lukasgraf   (501) staff       (20)     5841 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/contentstats/testing.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      244 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw/__init__.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)      137 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/MANIFEST.in
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/docs/
--rw-r--r--   0 lukasgraf   (501) staff       (20)    12282 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/docs/LICENSE.GPL
--rw-r--r--   0 lukasgraf   (501) staff       (20)     1297 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/docs/HISTORY.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)      744 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/docs/LICENSE.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)    60270 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/docs/content-stats-view.png
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2023 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/setup.py
--rw-r--r--   0 lukasgraf   (501) staff       (20)       38 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/setup.cfg
--rw-r--r--   0 lukasgraf   (501) staff       (20)     3552 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/README.rst
-drwxr-xr-x   0 lukasgraf   (501) staff       (20)        0 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/
--rw-r--r--   0 lukasgraf   (501) staff       (20)     7103 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/PKG-INFO
--rw-r--r--   0 lukasgraf   (501) staff       (20)        1 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/not-zip-safe
--rw-r--r--   0 lukasgraf   (501) staff       (20)        4 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/namespace_packages.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)     2323 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/SOURCES.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)      169 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/entry_points.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)      327 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/requires.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)        4 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/top_level.txt
--rw-r--r--   0 lukasgraf   (501) staff       (20)        1 2023-04-04 12:51:12.000000 ftw.contentstats-1.3.0/ftw.contentstats.egg-info/dependency_links.txt
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.091422 ftw.contentstats-1.4.0/
+-rw-r--r--   0 tbu       (1001) users      (100)      137 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/MANIFEST.in
+-rw-r--r--   0 tbu       (1001) users      (100)     6762 2024-04-04 11:42:19.090422 ftw.contentstats-1.4.0/PKG-INFO
+-rw-r--r--   0 tbu       (1001) users      (100)     3552 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/README.rst
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.084422 ftw.contentstats-1.4.0/docs/
+-rw-r--r--   0 tbu       (1001) users      (100)     1619 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/docs/HISTORY.txt
+-rw-r--r--   0 tbu       (1001) users      (100)    12282 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/docs/LICENSE.GPL
+-rw-r--r--   0 tbu       (1001) users      (100)      744 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/docs/LICENSE.txt
+-rw-r--r--   0 tbu       (1001) users      (100)    60270 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/docs/content-stats-view.png
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.084422 ftw.contentstats-1.4.0/ftw/
+-rw-r--r--   0 tbu       (1001) users      (100)      244 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/__init__.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.086422 ftw.contentstats-1.4.0/ftw/contentstats/
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.086422 ftw.contentstats-1.4.0/ftw/contentstats/Extensions/
+-rw-r--r--   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/Extensions/__init__.py
+-rw-r--r--   0 tbu       (1001) users      (100)      250 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/Extensions/install.py
+-rw-r--r--   0 tbu       (1001) users      (100)      129 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/__init__.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.086422 ftw.contentstats-1.4.0/ftw/contentstats/browser/
+-rw-r--r--   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/__init__.py
+-rw-r--r--   0 tbu       (1001) users      (100)      895 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/configure.zcml
+-rw-r--r--   0 tbu       (1001) users      (100)     2056 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/content_stats.py
+-rw-r--r--   0 tbu       (1001) users      (100)     1051 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/dump_stats.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.087422 ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/
+-rw-r--r--   0 tbu       (1001) users      (100)     2043 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/c3.min.css
+-rw-r--r--   0 tbu       (1001) users      (100)   180227 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/c3.min.js
+-rw-r--r--   0 tbu       (1001) users      (100)      435 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/content-stats.css
+-rw-r--r--   0 tbu       (1001) users      (100)     1834 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/content-stats.js
+-rw-r--r--   0 tbu       (1001) users      (100)   151725 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/d3.v3.min.js
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.087422 ftw.contentstats-1.4.0/ftw/contentstats/browser/templates/
+-rw-r--r--   0 tbu       (1001) users      (100)     3079 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/browser/templates/content_stats.pt
+-rw-r--r--   0 tbu       (1001) users      (100)     2609 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/command.py
+-rw-r--r--   0 tbu       (1001) users      (100)      852 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/configure.zcml
+-rw-r--r--   0 tbu       (1001) users      (100)     3160 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/console.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.087422 ftw.contentstats-1.4.0/ftw/contentstats/demo/
+-rw-r--r--   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/demo/__init__.py
+-rw-r--r--   0 tbu       (1001) users      (100)      255 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/demo/configure.zcml
+-rw-r--r--   0 tbu       (1001) users      (100)      912 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/demo/filters.py
+-rw-r--r--   0 tbu       (1001) users      (100)     9427 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/disk_usage.py
+-rw-r--r--   0 tbu       (1001) users      (100)     1361 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/interfaces.py
+-rw-r--r--   0 tbu       (1001) users      (100)     3162 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/logger.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.084422 ftw.contentstats-1.4.0/ftw/contentstats/profiles/
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.087422 ftw.contentstats-1.4.0/ftw/contentstats/profiles/default/
+-rwxr-xr-x   0 tbu       (1001) users      (100)       73 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/profiles/default/metadata.xml
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.087422 ftw.contentstats-1.4.0/ftw/contentstats/profiles/uninstall/
+-rw-r--r--   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/profiles/uninstall/.gitkeep
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.088422 ftw.contentstats-1.4.0/ftw/contentstats/providers/
+-rw-r--r--   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/providers/__init__.py
+-rw-r--r--   0 tbu       (1001) users      (100)      554 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/providers/configure.zcml
+-rw-r--r--   0 tbu       (1001) users      (100)     1494 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/providers/disk_usage.py
+-rw-r--r--   0 tbu       (1001) users      (100)     4395 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/providers/perf_metrics.py
+-rw-r--r--   0 tbu       (1001) users      (100)     1831 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/providers/portal_types.py
+-rw-r--r--   0 tbu       (1001) users      (100)     1888 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/providers/review_states.py
+-rw-r--r--   0 tbu       (1001) users      (100)     3094 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/stats.py
+-rw-r--r--   0 tbu       (1001) users      (100)     5841 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/testing.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.089422 ftw.contentstats-1.4.0/ftw/contentstats/tests/
+-rw-r--r--   0 tbu       (1001) users      (100)     1504 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/__init__.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.089422 ftw.contentstats-1.4.0/ftw/contentstats/tests/assets/
+-rw-r--r--   0 tbu       (1001) users      (100)      305 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/assets/__init__.py
+-rw-r--r--   0 tbu       (1001) users      (100)      354 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/assets/disk-usage.json
+-rw-r--r--   0 tbu       (1001) users      (100)     3064 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_content_stats_view.py
+-rw-r--r--   0 tbu       (1001) users      (100)     5632 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_disk_usage.py
+-rw-r--r--   0 tbu       (1001) users      (100)     1469 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_disk_usage_provider.py
+-rw-r--r--   0 tbu       (1001) users      (100)     2946 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_dump_stats_view.py
+-rw-r--r--   0 tbu       (1001) users      (100)     8377 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_logger.py
+-rw-r--r--   0 tbu       (1001) users      (100)     2754 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_perf_metrics_provider.py
+-rw-r--r--   0 tbu       (1001) users      (100)     1549 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_portal_types_provider.py
+-rw-r--r--   0 tbu       (1001) users      (100)      409 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_profiles.py
+-rw-r--r--   0 tbu       (1001) users      (100)     1746 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_review_state_provider.py
+-rw-r--r--   0 tbu       (1001) users      (100)     2708 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_stats.py
+-rw-r--r--   0 tbu       (1001) users      (100)      290 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/tests/test_uninstall.py
+-rw-r--r--   0 tbu       (1001) users      (100)     1891 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/ftw/contentstats/utils.py
+drwxr-xr-x   0 tbu       (1001) users      (100)        0 2024-04-04 11:42:19.089422 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/
+-rw-r--r--   0 tbu       (1001) users      (100)     6762 2024-04-04 11:42:19.000000 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/PKG-INFO
+-rw-r--r--   0 tbu       (1001) users      (100)     2351 2024-04-04 11:42:19.000000 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/SOURCES.txt
+-rw-r--r--   0 tbu       (1001) users      (100)        1 2024-04-04 11:42:19.000000 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/dependency_links.txt
+-rw-r--r--   0 tbu       (1001) users      (100)      204 2024-04-04 11:42:19.000000 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/entry_points.txt
+-rw-r--r--   0 tbu       (1001) users      (100)        4 2024-04-04 11:42:19.000000 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/namespace_packages.txt
+-rw-r--r--   0 tbu       (1001) users      (100)        1 2024-04-04 11:42:19.000000 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/not-zip-safe
+-rw-r--r--   0 tbu       (1001) users      (100)      346 2024-04-04 11:42:19.000000 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/requires.txt
+-rw-r--r--   0 tbu       (1001) users      (100)        4 2024-04-04 11:42:19.000000 ftw.contentstats-1.4.0/ftw.contentstats.egg-info/top_level.txt
+-rw-r--r--   0 tbu       (1001) users      (100)       38 2024-04-04 11:42:19.091422 ftw.contentstats-1.4.0/setup.cfg
+-rw-r--r--   0 tbu       (1001) users      (100)     2142 2024-04-04 11:42:18.000000 ftw.contentstats-1.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/demo/filters.py` & `ftw.contentstats-1.4.0/ftw/contentstats/demo/filters.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/interfaces.py` & `ftw.contentstats-1.4.0/ftw/contentstats/interfaces.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/configure.zcml` & `ftw.contentstats-1.4.0/ftw/contentstats/configure.zcml`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/providers/configure.zcml` & `ftw.contentstats-1.4.0/ftw/contentstats/providers/configure.zcml`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/providers/perf_metrics.py` & `ftw.contentstats-1.4.0/ftw/contentstats/providers/perf_metrics.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/providers/review_states.py` & `ftw.contentstats-1.4.0/ftw/contentstats/providers/review_states.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/providers/disk_usage.py` & `ftw.contentstats-1.4.0/ftw/contentstats/providers/disk_usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,18 +37,15 @@
         try:
             with open(path) as disk_usage_file:
                 disk_usage = json.load(disk_usage_file)
         except IOError:
             log.warn('Unable to read disk usage stats from %r' % path)
             return {}
 
-        # XXX: The paths to filestorage and blobstorage could eventually be
-        # determined dynamically (ZODB APIs should be able to tell us).
-
         stats = {}
         stats['total'] = disk_usage['total']
-        stats['filestorage'] = disk_usage['subtrees']['var/filestorage/Data.fs']
-        stats['blobstorage'] = disk_usage['subtrees']['var/blobstorage']
+        stats['filestorage'] = disk_usage['filestorage']
+        stats['blobstorage'] = disk_usage['blobstorage']
         return stats
 
     def get_display_names(self):
         return None
```

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/providers/portal_types.py` & `ftw.contentstats-1.4.0/ftw/contentstats/providers/portal_types.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_disk_usage_provider.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_disk_usage_provider.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_dump_stats_view.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_dump_stats_view.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_stats.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_review_state_provider.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_review_state_provider.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_content_stats_view.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_content_stats_view.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_portal_types_provider.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_portal_types_provider.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/__init__.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_perf_metrics_provider.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_perf_metrics_provider.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_disk_usage.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_disk_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,17 @@
         1024   /path/to/deployment
         """)
 
         with freeze(FROZEN_NOW):
             du_stats = calculator.calc_du_stats()
 
         # Should reduce subtree depth to 2 levels, except for var/filestorage/*
-        self.assertEqual({'deployment': '/path/to/deployment',
+        self.assertEqual({'blobstorage': 45,
+                          'deployment': '/path/to/deployment',
+                          'filestorage': 20,
                           'updated': FROZEN_NOW.isoformat(),
                           'total': 1024,
                           'subtrees': {'bin': 10,
                                        'bin/instance': 5,
                                        'var/blobstorage': 45,
                                        'var/filestorage/Data.fs': 20,
                                        'var/filestorage/Data.fs.index': 25,
```

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/tests/test_logger.py` & `ftw.contentstats-1.4.0/ftw/contentstats/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/logger.py` & `ftw.contentstats-1.4.0/ftw/contentstats/logger.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/browser/configure.zcml` & `ftw.contentstats-1.4.0/ftw/contentstats/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/content-stats.js` & `ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/content-stats.js`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/d3.v3.min.js` & `ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/d3.v3.min.js`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/c3.min.js` & `ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/c3.min.js`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/browser/resources/c3.min.css` & `ftw.contentstats-1.4.0/ftw/contentstats/browser/resources/c3.min.css`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/browser/dump_stats.py` & `ftw.contentstats-1.4.0/ftw/contentstats/browser/dump_stats.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/browser/templates/content_stats.pt` & `ftw.contentstats-1.4.0/ftw/contentstats/browser/templates/content_stats.pt`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/browser/content_stats.py` & `ftw.contentstats-1.4.0/ftw/contentstats/browser/content_stats.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/utils.py` & `ftw.contentstats-1.4.0/ftw/contentstats/utils.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/stats.py` & `ftw.contentstats-1.4.0/ftw/contentstats/stats.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw/contentstats/testing.py` & `ftw.contentstats-1.4.0/ftw/contentstats/testing.py`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/docs/LICENSE.GPL` & `ftw.contentstats-1.4.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/docs/HISTORY.txt` & `ftw.contentstats-1.4.0/docs/HISTORY.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 Changelog
 =========
 
 
+1.4.0 (2024-04-04)
+------------------
+
+- Add Python implementation for calculating disk usage. [buchi]
+
+- Add option to specify data path for disk usage calculation. [buchi]
+
+- Add zopectl command for dumping content stats. [buchi]
+
+- Make filestorage (Data.fs) and blobstorage path for disk usage configurable. [buchi]
+
+
 1.3.0 (2023-04-04)
 ------------------
 
 - Add support for logging to Fluentd. [lgraf]
 
 
 1.2.0 (2020-05-04)
```

### Comparing `ftw.contentstats-1.3.0/docs/LICENSE.txt` & `ftw.contentstats-1.4.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/docs/content-stats-view.png` & `ftw.contentstats-1.4.0/docs/content-stats-view.png`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/setup.py` & `ftw.contentstats-1.4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 import os
 
-version = '1.3.0'
+version = '1.4.0'
 
 tests_require = [
     'ftw.builder',
     'ftw.testbrowser',
     'ftw.testing',
     'mock',
     'plone.app.testing',
@@ -16,14 +16,15 @@
     'zope.configuration',
     'freezegun < 0.3.15',
     'requests_toolbelt',
 ]
 
 extras_require = {
     'tests': tests_require,
+    'scandir': ['scandir']
 }
 
 
 setup(
     name='ftw.contentstats',
     version=version,
     description='Collect and display content statistics for Plone sites',
@@ -72,11 +73,14 @@
     extras_require=extras_require,
 
     entry_points="""
     # -*- Entry points: -*-
     [z3c.autoinclude.plugin]
     target = plone
 
+    [zopectl.command]
+    dump_content_stats = ftw.contentstats.command:dump_content_stats
+
     [console_scripts]
     dump-content-stats = ftw.contentstats.console:dump_stats_cmd
     """,
 )
```

### Comparing `ftw.contentstats-1.3.0/README.rst` & `ftw.contentstats-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `ftw.contentstats-1.3.0/ftw.contentstats.egg-info/SOURCES.txt` & `ftw.contentstats-1.4.0/ftw.contentstats.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ftw.contentstats.egg-info/dependency_links.txt
 ftw.contentstats.egg-info/entry_points.txt
 ftw.contentstats.egg-info/namespace_packages.txt
 ftw.contentstats.egg-info/not-zip-safe
 ftw.contentstats.egg-info/requires.txt
 ftw.contentstats.egg-info/top_level.txt
 ftw/contentstats/__init__.py
+ftw/contentstats/command.py
 ftw/contentstats/configure.zcml
 ftw/contentstats/console.py
 ftw/contentstats/disk_usage.py
 ftw/contentstats/interfaces.py
 ftw/contentstats/logger.py
 ftw/contentstats/stats.py
 ftw/contentstats/testing.py
```

