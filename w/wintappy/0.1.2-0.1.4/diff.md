# Comparing `tmp/wintappy-0.1.2.tar.gz` & `tmp/wintappy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wintappy-0.1.2.tar", last modified: Mon Oct 23 21:18:12 2023, max compression
+gzip compressed data, was "wintappy-0.1.4.tar", last modified: Thu Apr  4 19:08:48 2024, max compression
```

## Comparing `wintappy-0.1.2.tar` & `wintappy-0.1.4.tar`

### file list

```diff
@@ -1,95 +1,108 @@
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.072777 wintappy-0.1.2/
--rw-r--r--   0 johnson30  (5081)     5081     1095 2023-08-31 14:53:20.000000 wintappy-0.1.2/LICENSE
--rw-r--r--   0 johnson30  (5081)     5081     2055 2023-10-23 21:18:12.072608 wintappy-0.1.2/PKG-INFO
--rw-r--r--   0 johnson30  (5081)     5081     1222 2023-08-31 14:53:20.000000 wintappy-0.1.2/README.md
--rw-r--r--   0 johnson30  (5081)     5081     1212 2023-10-23 21:18:12.073520 wintappy-0.1.2/setup.cfg
--rw-r--r--   0 johnson30  (5081)     5081      461 2023-10-23 21:15:18.000000 wintappy-0.1.2/setup.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.001785 wintappy-0.1.2/wintappy/
--rw-r--r--   0 johnson30  (5081)     5081       18 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/__init__.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.006305 wintappy-0.1.2/wintappy/analytics/
--rw-r--r--   0 johnson30  (5081)     5081        0 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/__init__.py
--rw-r--r--   0 johnson30  (5081)     5081      873 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/constants.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.034587 wintappy-0.1.2/wintappy/analytics/mitre_car/
--rw-r--r--   0 johnson30  (5081)     5081      245 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2013-02-003.sql
--rw-r--r--   0 johnson30  (5081)     5081      702 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2013-03-001.sql
--rw-r--r--   0 johnson30  (5081)     5081      234 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2013-05-004.sql
--rw-r--r--   0 johnson30  (5081)     5081      294 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2013-07-002.sql
--rw-r--r--   0 johnson30  (5081)     5081      246 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2014-03-006.sql
--rw-r--r--   0 johnson30  (5081)     5081      441 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2014-04-003.sql
--rw-r--r--   0 johnson30  (5081)     5081      435 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2014-05-002.sql
--rw-r--r--   0 johnson30  (5081)     5081      454 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2014-11-004.sql
--rw-r--r--   0 johnson30  (5081)     5081      339 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2014-11-006.sql
--rw-r--r--   0 johnson30  (5081)     5081      443 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2014-11-008.sql
--rw-r--r--   0 johnson30  (5081)     5081      293 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2016-03-002.sql
--rw-r--r--   0 johnson30  (5081)     5081      447 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2019-04-002.sql
--rw-r--r--   0 johnson30  (5081)     5081      270 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2019-04-003.sql
--rw-r--r--   0 johnson30  (5081)     5081      287 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2019-07-002.sql
--rw-r--r--   0 johnson30  (5081)     5081      276 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-09-002.sql
--rw-r--r--   0 johnson30  (5081)     5081      286 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-09-003.sql
--rw-r--r--   0 johnson30  (5081)     5081      637 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-09-004.sql
--rw-r--r--   0 johnson30  (5081)     5081      442 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-09-005.sql
--rw-r--r--   0 johnson30  (5081)     5081     1650 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-004.sql
--rw-r--r--   0 johnson30  (5081)     5081      620 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-005.sql
--rw-r--r--   0 johnson30  (5081)     5081      472 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-006.sql
--rw-r--r--   0 johnson30  (5081)     5081      425 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-007.sql
--rw-r--r--   0 johnson30  (5081)     5081      387 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-008.sql
--rw-r--r--   0 johnson30  (5081)     5081      238 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-009.sql
--rw-r--r--   0 johnson30  (5081)     5081      345 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-011.sql
--rw-r--r--   0 johnson30  (5081)     5081      397 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-01-003.sql
--rw-r--r--   0 johnson30  (5081)     5081      483 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-01-004.sql
--rw-r--r--   0 johnson30  (5081)     5081      613 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-01-006.sql
--rw-r--r--   0 johnson30  (5081)     5081      464 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-01-007.sql
--rw-r--r--   0 johnson30  (5081)     5081      363 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-01-008.sql
--rw-r--r--   0 johnson30  (5081)     5081      764 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-02-001.sql
--rw-r--r--   0 johnson30  (5081)     5081      691 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-02-002.sql
--rw-r--r--   0 johnson30  (5081)     5081      584 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-04-001.sql
--rw-r--r--   0 johnson30  (5081)     5081      300 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-001.sql
--rw-r--r--   0 johnson30  (5081)     5081      298 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-003.sql
--rw-r--r--   0 johnson30  (5081)     5081      334 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-006.sql
--rw-r--r--   0 johnson30  (5081)     5081      336 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-007.sql
--rw-r--r--   0 johnson30  (5081)     5081      294 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-008.sql
--rw-r--r--   0 johnson30  (5081)     5081      282 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-009.sql
--rw-r--r--   0 johnson30  (5081)     5081      385 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-010.sql
--rw-r--r--   0 johnson30  (5081)     5081      587 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-012.sql
--rw-r--r--   0 johnson30  (5081)     5081        0 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/__init__.py
--rw-r--r--   0 johnson30  (5081)     5081      256 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/mitre_car/macros.sql
--rw-r--r--   0 johnson30  (5081)     5081      927 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/analytics/query_analytic.py
--rw-r--r--   0 johnson30  (5081)     5081     4064 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/analytics/utils.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.056026 wintappy-0.1.2/wintappy/database/
--rw-r--r--   0 johnson30  (5081)     5081        0 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/database/__init__.py
--rw-r--r--   0 johnson30  (5081)     5081      479 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/database/constants.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.058821 wintappy-0.1.2/wintappy/database/templates/
--rw-r--r--   0 johnson30  (5081)     5081        0 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/database/templates/__init__.py
--rw-r--r--   0 johnson30  (5081)     5081      307 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/database/templates/create_analytics.sql
--rw-r--r--   0 johnson30  (5081)     5081      353 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/database/templates/create_analytics_results.sql
--rw-r--r--   0 johnson30  (5081)     5081      258 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/database/templates/insert_analytics.sql
--rw-r--r--   0 johnson30  (5081)     5081      185 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/database/templates/insert_analytics_results.sql
--rw-r--r--   0 johnson30  (5081)     5081      325 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/database/wintap_database.py
--rw-r--r--   0 johnson30  (5081)     5081     6453 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/database/wintap_duckdb.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.064331 wintappy-0.1.2/wintappy/datautils/
--rw-r--r--   0 johnson30  (5081)     5081        0 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/datautils/__init__.py
--rw-r--r--   0 johnson30  (5081)     5081      367 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/datautils/initdb.sql
--rw-r--r--   0 johnson30  (5081)     5081    19948 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/datautils/rawtostdview.sql
--rw-r--r--   0 johnson30  (5081)     5081    12450 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/datautils/rawutil.py
--rw-r--r--   0 johnson30  (5081)     5081     6939 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/datautils/stdview_duckdb.py
--rw-r--r--   0 johnson30  (5081)     5081     7491 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/datautils/stdviewutil.py
--rw-r--r--   0 johnson30  (5081)     5081     8259 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/datautils/wintapgraph.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.070110 wintappy-0.1.2/wintappy/etlutils/
--rw-r--r--   0 johnson30  (5081)     5081        0 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/etlutils/__init__.py
--rw-r--r--   0 johnson30  (5081)     5081     5290 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/etlutils/collectbinaries.py
--rw-r--r--   0 johnson30  (5081)     5081    12919 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/etlutils/download_from_s3.py
--rw-r--r--   0 johnson30  (5081)     5081     1927 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/etlutils/rawtorolling.py
--rw-r--r--   0 johnson30  (5081)     5081     1353 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/etlutils/rawtostdview.py
--rw-r--r--   0 johnson30  (5081)     5081     5597 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/etlutils/run_enrichment.py
--rw-r--r--   0 johnson30  (5081)     5081     1065 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/etlutils/transformer_manager.py
--rw-r--r--   0 johnson30  (5081)     5081      195 2023-10-23 21:15:18.000000 wintappy-0.1.2/wintappy/etlutils/utils.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.071468 wintappy-0.1.2/wintappy/notebookutils/
--rw-r--r--   0 johnson30  (5081)     5081      399 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/notebookutils/__init__.py
--rw-r--r--   0 johnson30  (5081)     5081     1441 2023-08-31 14:53:20.000000 wintappy-0.1.2/wintappy/notebookutils/datasetchooser.py
-drwxr-xr-x   0 johnson30  (5081)     5081        0 2023-10-23 21:18:12.004333 wintappy-0.1.2/wintappy.egg-info/
--rw-r--r--   0 johnson30  (5081)     5081     2055 2023-10-23 21:18:11.000000 wintappy-0.1.2/wintappy.egg-info/PKG-INFO
--rw-r--r--   0 johnson30  (5081)     5081     3439 2023-10-23 21:18:11.000000 wintappy-0.1.2/wintappy.egg-info/SOURCES.txt
--rw-r--r--   0 johnson30  (5081)     5081        1 2023-10-23 21:18:11.000000 wintappy-0.1.2/wintappy.egg-info/dependency_links.txt
--rw-r--r--   0 johnson30  (5081)     5081      291 2023-10-23 21:18:11.000000 wintappy-0.1.2/wintappy.egg-info/entry_points.txt
--rw-r--r--   0 johnson30  (5081)     5081      212 2023-10-23 21:18:11.000000 wintappy-0.1.2/wintappy.egg-info/requires.txt
--rw-r--r--   0 johnson30  (5081)     5081        9 2023-10-23 21:18:11.000000 wintappy-0.1.2/wintappy.egg-info/top_level.txt
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.625769 wintappy-0.1.4/
+-rw-r--r--   0 johnson30  (5081)     5081     1095 2023-07-10 21:41:14.000000 wintappy-0.1.4/LICENSE
+-rw-r--r--   0 johnson30  (5081)     5081     2072 2024-04-04 19:08:48.625481 wintappy-0.1.4/PKG-INFO
+-rw-r--r--   0 johnson30  (5081)     5081     1222 2023-07-11 21:46:34.000000 wintappy-0.1.4/README.md
+-rw-r--r--   0 johnson30  (5081)     5081     1304 2024-04-04 19:08:48.627122 wintappy-0.1.4/setup.cfg
+-rw-r--r--   0 johnson30  (5081)     5081      470 2024-04-04 19:00:29.000000 wintappy-0.1.4/setup.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.557319 wintappy-0.1.4/tests/
+-rw-r--r--   0 johnson30  (5081)     5081     2042 2024-03-05 21:48:59.000000 wintappy-0.1.4/tests/test_config.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.558858 wintappy-0.1.4/wintappy/
+-rw-r--r--   0 johnson30  (5081)     5081       18 2024-04-04 19:04:56.000000 wintappy-0.1.4/wintappy/__init__.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.564637 wintappy-0.1.4/wintappy/analytics/
+-rw-r--r--   0 johnson30  (5081)     5081        0 2023-11-09 23:28:21.000000 wintappy-0.1.4/wintappy/analytics/__init__.py
+-rw-r--r--   0 johnson30  (5081)     5081     1035 2023-11-10 00:23:32.000000 wintappy-0.1.4/wintappy/analytics/constants.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.590951 wintappy-0.1.4/wintappy/analytics/mitre_car/
+-rw-r--r--   0 johnson30  (5081)     5081      233 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2013-02-003.sql
+-rw-r--r--   0 johnson30  (5081)     5081      790 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2013-03-001.sql
+-rw-r--r--   0 johnson30  (5081)     5081      222 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2013-05-004.sql
+-rw-r--r--   0 johnson30  (5081)     5081      282 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2013-07-002.sql
+-rw-r--r--   0 johnson30  (5081)     5081      234 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2014-03-006.sql
+-rw-r--r--   0 johnson30  (5081)     5081      464 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2014-04-003.sql
+-rw-r--r--   0 johnson30  (5081)     5081      458 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2014-05-002.sql
+-rw-r--r--   0 johnson30  (5081)     5081      469 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2014-11-004.sql
+-rw-r--r--   0 johnson30  (5081)     5081      327 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2014-11-006.sql
+-rw-r--r--   0 johnson30  (5081)     5081      466 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2014-11-008.sql
+-rw-r--r--   0 johnson30  (5081)     5081      281 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2016-03-002.sql
+-rw-r--r--   0 johnson30  (5081)     5081      470 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2019-04-002.sql
+-rw-r--r--   0 johnson30  (5081)     5081      258 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2019-04-003.sql
+-rw-r--r--   0 johnson30  (5081)     5081      275 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2019-07-002.sql
+-rw-r--r--   0 johnson30  (5081)     5081      264 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-09-002.sql
+-rw-r--r--   0 johnson30  (5081)     5081      274 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-09-003.sql
+-rw-r--r--   0 johnson30  (5081)     5081      625 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-09-004.sql
+-rw-r--r--   0 johnson30  (5081)     5081      430 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-09-005.sql
+-rw-r--r--   0 johnson30  (5081)     5081     1673 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-004.sql
+-rw-r--r--   0 johnson30  (5081)     5081      608 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-005.sql
+-rw-r--r--   0 johnson30  (5081)     5081      460 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-006.sql
+-rw-r--r--   0 johnson30  (5081)     5081      413 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-007.sql
+-rw-r--r--   0 johnson30  (5081)     5081      375 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-008.sql
+-rw-r--r--   0 johnson30  (5081)     5081      226 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-009.sql
+-rw-r--r--   0 johnson30  (5081)     5081      333 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-011.sql
+-rw-r--r--   0 johnson30  (5081)     5081      385 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-01-003.sql
+-rw-r--r--   0 johnson30  (5081)     5081      506 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-01-004.sql
+-rw-r--r--   0 johnson30  (5081)     5081      636 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-01-006.sql
+-rw-r--r--   0 johnson30  (5081)     5081      449 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-01-007.sql
+-rw-r--r--   0 johnson30  (5081)     5081      348 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-01-008.sql
+-rw-r--r--   0 johnson30  (5081)     5081      787 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-02-001.sql
+-rw-r--r--   0 johnson30  (5081)     5081      714 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-02-002.sql
+-rw-r--r--   0 johnson30  (5081)     5081      572 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-04-001.sql
+-rw-r--r--   0 johnson30  (5081)     5081      288 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-001.sql
+-rw-r--r--   0 johnson30  (5081)     5081      286 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-003.sql
+-rw-r--r--   0 johnson30  (5081)     5081      322 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-006.sql
+-rw-r--r--   0 johnson30  (5081)     5081      324 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-007.sql
+-rw-r--r--   0 johnson30  (5081)     5081      282 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-008.sql
+-rw-r--r--   0 johnson30  (5081)     5081      270 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-009.sql
+-rw-r--r--   0 johnson30  (5081)     5081      373 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-010.sql
+-rw-r--r--   0 johnson30  (5081)     5081      575 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-012.sql
+-rw-r--r--   0 johnson30  (5081)     5081        0 2023-11-09 23:28:21.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/__init__.py
+-rw-r--r--   0 johnson30  (5081)     5081      318 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/mitre_car/macros.sql
+-rw-r--r--   0 johnson30  (5081)     5081     2239 2023-12-13 04:29:38.000000 wintappy-0.1.4/wintappy/analytics/query_analytic.py
+-rw-r--r--   0 johnson30  (5081)     5081     6890 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/analytics/utils.py
+-rw-r--r--   0 johnson30  (5081)     5081     4940 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/config.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.594547 wintappy-0.1.4/wintappy/database/
+-rw-r--r--   0 johnson30  (5081)     5081        0 2023-11-09 23:28:21.000000 wintappy-0.1.4/wintappy/database/__init__.py
+-rw-r--r--   0 johnson30  (5081)     5081      450 2024-01-25 19:43:03.000000 wintappy-0.1.4/wintappy/database/constants.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.598611 wintappy-0.1.4/wintappy/database/templates/
+-rw-r--r--   0 johnson30  (5081)     5081        0 2023-11-09 23:28:21.000000 wintappy-0.1.4/wintappy/database/templates/__init__.py
+-rw-r--r--   0 johnson30  (5081)     5081      353 2023-11-09 23:28:21.000000 wintappy-0.1.4/wintappy/database/templates/create_analytics_results.sql
+-rw-r--r--   0 johnson30  (5081)     5081      353 2023-12-13 04:29:37.000000 wintappy-0.1.4/wintappy/database/templates/create_sigma_results.sql
+-rw-r--r--   0 johnson30  (5081)     5081      194 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/database/templates/insert_analytics_results.sql
+-rw-r--r--   0 johnson30  (5081)     5081      325 2023-11-09 23:28:21.000000 wintappy-0.1.4/wintappy/database/wintap_database.py
+-rw-r--r--   0 johnson30  (5081)     5081     5754 2024-01-25 19:43:03.000000 wintappy-0.1.4/wintappy/database/wintap_duckdb.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.612982 wintappy-0.1.4/wintappy/datautils/
+-rw-r--r--   0 johnson30  (5081)     5081        0 2023-07-11 21:46:34.000000 wintappy-0.1.4/wintappy/datautils/__init__.py
+-rw-r--r--   0 johnson30  (5081)     5081      367 2023-07-11 21:46:34.000000 wintappy-0.1.4/wintappy/datautils/initdb.sql
+-rw-r--r--   0 johnson30  (5081)     5081     1567 2024-02-28 17:18:51.000000 wintappy-0.1.4/wintappy/datautils/label_summary.sql
+-rw-r--r--   0 johnson30  (5081)     5081      697 2024-02-28 17:18:51.000000 wintappy-0.1.4/wintappy/datautils/lolbas_summary.sql
+-rw-r--r--   0 johnson30  (5081)     5081      600 2024-02-28 17:18:51.000000 wintappy-0.1.4/wintappy/datautils/mitre_summary.sql
+-rw-r--r--   0 johnson30  (5081)     5081     1936 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/datautils/process_path.sql
+-rw-r--r--   0 johnson30  (5081)     5081     6976 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/datautils/process_summary.sql
+-rw-r--r--   0 johnson30  (5081)     5081    17362 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/datautils/rawtostdview.sql
+-rw-r--r--   0 johnson30  (5081)     5081    18704 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/datautils/rawutil.py
+-rw-r--r--   0 johnson30  (5081)     5081     1025 2024-02-28 17:18:51.000000 wintappy-0.1.4/wintappy/datautils/sigma_summary.sql
+-rw-r--r--   0 johnson30  (5081)     5081     9219 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/datautils/stdview_duckdb.py
+-rw-r--r--   0 johnson30  (5081)     5081     7491 2023-07-11 21:46:34.000000 wintappy-0.1.4/wintappy/datautils/stdviewutil.py
+-rw-r--r--   0 johnson30  (5081)     5081     2830 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/datautils/summary_util.py
+-rw-r--r--   0 johnson30  (5081)     5081      757 2024-02-28 17:18:51.000000 wintappy-0.1.4/wintappy/datautils/uber_summary.sql
+-rw-r--r--   0 johnson30  (5081)     5081     8210 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/datautils/wintapgraph.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.622115 wintappy-0.1.4/wintappy/etlutils/
+-rw-r--r--   0 johnson30  (5081)     5081        0 2023-07-11 21:46:34.000000 wintappy-0.1.4/wintappy/etlutils/__init__.py
+-rw-r--r--   0 johnson30  (5081)     5081     5290 2023-07-11 21:46:34.000000 wintappy-0.1.4/wintappy/etlutils/collectbinaries.py
+-rw-r--r--   0 johnson30  (5081)     5081     3486 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/etlutils/dbhelpers.py
+-rw-r--r--   0 johnson30  (5081)     5081    13337 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/etlutils/downloadfroms3.py
+-rw-r--r--   0 johnson30  (5081)     5081     1633 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/etlutils/rawtorolling.py
+-rw-r--r--   0 johnson30  (5081)     5081     1406 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/etlutils/rawtostdview.py
+-rw-r--r--   0 johnson30  (5081)     5081     5337 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/etlutils/run_enrichment.py
+-rw-r--r--   0 johnson30  (5081)     5081     1657 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/etlutils/runone.py
+-rw-r--r--   0 johnson30  (5081)     5081     1288 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/etlutils/transformer_manager.py
+-rw-r--r--   0 johnson30  (5081)     5081     3897 2024-04-04 19:00:29.000000 wintappy-0.1.4/wintappy/etlutils/ubersummary.py
+-rw-r--r--   0 johnson30  (5081)     5081     2270 2024-03-05 21:48:59.000000 wintappy-0.1.4/wintappy/etlutils/utils.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.624092 wintappy-0.1.4/wintappy/notebookutils/
+-rw-r--r--   0 johnson30  (5081)     5081      399 2023-07-11 21:46:34.000000 wintappy-0.1.4/wintappy/notebookutils/__init__.py
+-rw-r--r--   0 johnson30  (5081)     5081     1441 2023-07-11 21:46:34.000000 wintappy-0.1.4/wintappy/notebookutils/datasetchooser.py
+drwxr-xr-x   0 johnson30  (5081)     5081        0 2024-04-04 19:08:48.562002 wintappy-0.1.4/wintappy.egg-info/
+-rw-r--r--   0 johnson30  (5081)     5081     2072 2024-04-04 19:08:48.000000 wintappy-0.1.4/wintappy.egg-info/PKG-INFO
+-rw-r--r--   0 johnson30  (5081)     5081     3819 2024-04-04 19:08:48.000000 wintappy-0.1.4/wintappy.egg-info/SOURCES.txt
+-rw-r--r--   0 johnson30  (5081)     5081        1 2024-04-04 19:08:48.000000 wintappy-0.1.4/wintappy.egg-info/dependency_links.txt
+-rw-r--r--   0 johnson30  (5081)     5081      381 2024-04-04 19:08:48.000000 wintappy-0.1.4/wintappy.egg-info/entry_points.txt
+-rw-r--r--   0 johnson30  (5081)     5081      214 2024-04-04 19:08:48.000000 wintappy-0.1.4/wintappy.egg-info/requires.txt
+-rw-r--r--   0 johnson30  (5081)     5081        9 2024-04-04 19:08:48.000000 wintappy-0.1.4/wintappy.egg-info/top_level.txt
```

### Comparing `wintappy-0.1.2/LICENSE` & `wintappy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wintappy-0.1.2/PKG-INFO` & `wintappy-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: wintappy
-Version: 0.1.2
+Version: 0.1.4
 Summary: Python utilities for working with Wintap data
 Home-page: https://github.com/LLNL/Wintap-PyUtil
 Author: LLNL
 Author-email: grantj@llnl.gov
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: altair
 Requires-Dist: boto3
 Requires-Dist: duckdb
+Requires-Dist: dynaconf
 Requires-Dist: fsspec
 Requires-Dist: gitpython
 Requires-Dist: humanfriendly
 Requires-Dist: importlib_resources
 Requires-Dist: ipyfilechooser
-Requires-Dist: jinja2==3.0.3
+Requires-Dist: jinja2
 Requires-Dist: jinjasql
 Requires-Dist: lxml
 Requires-Dist: magic_duckdb
 Requires-Dist: matplotlib
 Requires-Dist: mitreattack-python
 Requires-Dist: networkx
 Requires-Dist: pandas
```

### Comparing `wintappy-0.1.2/README.md` & `wintappy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `wintappy-0.1.2/setup.cfg` & `wintappy-0.1.4/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -21,18 +21,20 @@
 
 [options.package_data]
 * = *.sql
 
 [options.entry_points]
 console_scripts = 
 	collectbinaries = wintappy.etlutils.collectbinaries:main
-	download_from_s3 = wintappy.etlutils.download_from_s3:main
+	dbhelpers = wintappy.etlutils.dbhelpers:main
+	downloadfroms3 = wintappy.etlutils.downloadfroms3:main
 	run_enrichment = wintappy.etlutils.run_enrichment:main
 	rawtorolling = wintappy.etlutils.rawtorolling:main
 	rawtostdview = wintappy.etlutils.rawtostdview:main
+	ubersummary = wintappy.etlutils.ubersummary:main
 
 [black]
 line-length = 100
 target-version = ["py310"]
 disallow-untyped-defs = true
 ignore-missing-imports = true
 warn-unused-imports = true
```

### Comparing `wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-004.sql` & `wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-004.sql`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 -- Processes Started From Irregular Parent
 -- Tactic: Defense Evasion; Technique: Process Injection
 SELECT
-    child.pid_hash AS pid_hash,
-    COALESCE(child.first_seen, child.daypk) AS first_seen
+    child.pid_hash,
+    child.first_seen
 FROM process AS child,
     process AS parent
 WHERE
     parent.pid_hash = child.parent_pid_hash
     AND (
         (
             child.process_name = 'smss.exe'
@@ -41,9 +41,11 @@
             AND parent.process_name NOT IN ('services.exe', 'svchost.exe')
         )
         OR (
             child.process_name = 'userinit.exe'
             AND parent.process_name NOT IN ('dwm.exe', 'winlogon.exe')
         )
     )
+{% if search_day_pk is defined and search_day_pk != None %}
     AND parent.daypk = {{ search_day_pk|default(20230501, true) }}
     AND child.daypk = {{ search_day_pk|default(20230501, true) }}
+{% endif %}
```

### Comparing `wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2020-11-005.sql` & `wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2020-11-005.sql`

 * *Files 27% similar despite different names*

```diff
@@ -8,8 +8,8 @@
     (
         args LIKE '%rm (Get-PSReadlineOption).HistorySavePath%'
         OR args LIKE '%del (Get-PSReadlineOption).HistorySavePath%'
         OR args LIKE '%Set-PSReadlineOption –HistorySaveStyle SaveNothing%'
         OR args LIKE '%Remove-Item (Get-PSReadlineOption).HistorySavePath%'
         OR args LIKE '%del%Microsoft\Windows\Powershell\PSReadline\ConsoleHost_history.txt'
     )
-    AND daypk = {{ limit_search_days( search_day_pk ) }}
+    {{ limit_search_days( search_day_pk ) }}
```

### Comparing `wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-01-006.sql` & `wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-01-006.sql`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 -- Unusual Child Process spawned using DDE exploit
 SELECT
-    child.pid_hash AS pid_hash,
-    COALESCE(child.first_seen, child.daypk) AS first_seen
+    child.pid_hash,
+    child.first_seen
 FROM process AS child,
     process AS parent
 WHERE
     parent.pid_hash = child.parent_pid_hash
     AND (
         child.process_name LIKE '%.exe'
         AND (
             parent.process_name LIKE '%excel.exe'
             OR parent.process_name LIKE '%word.exe'
             OR parent.process_name LIKE '%outlook.exe'
         )
     )
+{% if search_day_pk is defined and search_day_pk != None %}
     AND parent.daypk = {{ search_day_pk|default(20230501, true) }}
     AND child.daypk = {{ search_day_pk|default(20230501, true) }}
+{% endif %}
```

### Comparing `wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-02-002.sql` & `wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-02-002.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 -- Get System Elevation
 
 SELECT
-    child.pid_hash AS pid_hash,
-    COALESCE(child.first_seen, child.daypk) AS first_seen
+    child.pid_hash,
+    child.first_seen
 FROM process AS child,
     process AS parent
 WHERE
     parent.pid_hash = child.parent_pid_hash
     AND
     (
         (
@@ -17,9 +17,11 @@
         )
         OR
         (
             parent.process_name = 'rundll32.exe'
             AND child.args LIKE '%,a /p:%'
         )
     )
-    AND child.daypk = {{ search_day_pk|default(20230501, true) }}
+{% if search_day_pk is defined and search_day_pk != None %}
     AND parent.daypk = {{ search_day_pk|default(20230501, true) }}
+    AND child.daypk = {{ search_day_pk|default(20230501, true) }}
+{% endif %}
```

### Comparing `wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-04-001.sql` & `wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-04-001.sql`

 * *Files 2% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 FROM process
 WHERE
     process_name IN ('smss.exe', 'wininit.exe', 'taskhost.exe', 'lasass.exe', 'winlogon.exe', 'csrss.exe', 'services.exe', )
     AND process_path NOT LIKE 'C:\Windows\System32\%.exe'
     AND process_path NOT LIKE 'c:\windows\system32\%.exe'
     AND process_path NOT LIKE 'systemroot\system32\%.exe'
     AND process_path NOT LIKE '%systemroot%\system32\%.exe'
-    AND daypk = {{ limit_search_days( search_day_pk ) }}
+    {{ limit_search_days( search_day_pk ) }}
```

### Comparing `wintappy-0.1.2/wintappy/analytics/mitre_car/CAR-2021-05-012.sql` & `wintappy-0.1.4/wintappy/analytics/mitre_car/CAR-2021-05-012.sql`

 * *Files 14% similar despite different names*

```diff
@@ -9,8 +9,8 @@
     AND process_path NOT LIKE 'C:\\Windows%'
     AND process_path NOT LIKE '%windir%'
     AND process_path NOT LIKE 'C:\\Program File%'
     AND process_path NOT LIKE 'C:\\Programdata%'
     AND process_path NOT LIKE 'c:\\windows%'
     AND process_path NOT LIKE 'c:\\Program File%'
     AND process_path NOT LIKE 'c:\\Programdata%'
-    AND daypk = {{ limit_search_days( search_day_pk ) }}
+    {{ limit_search_days( search_day_pk ) }}
```

### Comparing `wintappy-0.1.2/wintappy/database/wintap_duckdb.py` & `wintappy-0.1.4/wintappy/database/wintap_duckdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,20 +6,17 @@
 
 import duckdb
 from duckdb import DuckDBPyConnection
 from jinja2 import Environment, FileSystemLoader
 from pandas import DataFrame
 
 from .constants import (
-    ANALYTICS_RESULTS_TABLE,
-    ANALYTICS_TABLE,
+    CAR_ANALYTICS_RESULTS_TABLE,
     CREATE_ANALYTICS_RESULTS_TEMPLATE,
-    CREATE_ANALYTICS_TEMPLATE,
     INSERT_ANALYTICS_RESULTS_TEMPLATE,
-    INSERT_ANALYTICS_TEMPLATE,
     PID_HASH,
     TEMPLATE_DIR,
 )
 
 
 @dataclass
 class WintapDuckDBOptions:
@@ -42,29 +39,29 @@
         self._jinja_environment = Environment(
             loader=FileSystemLoader(os.path.join(cwd, TEMPLATE_DIR))
         )
         self._setup_tables()
 
     def _setup_tables(self) -> None:
         """Create extra tables that store analytics results"""
-        if self._is_table_or_view(ANALYTICS_RESULTS_TABLE):
+        if self._is_table_or_view(CAR_ANALYTICS_RESULTS_TABLE):
             if self._load_analytics:
                 return
         # Because we are generating analytics, we should drop any existing views
         # of our data, else we will run into errors
-        self.query(f"DROP VIEW IF EXISTS {ANALYTICS_RESULTS_TABLE}")
+        self.query(f"DROP VIEW IF EXISTS {CAR_ANALYTICS_RESULTS_TABLE}")
         self.query(
             self._jinja_environment.get_template(
                 CREATE_ANALYTICS_RESULTS_TEMPLATE
             ).render()
         )
-        # Create table for analytics metadata
-        self.query(f"DROP VIEW IF EXISTS {ANALYTICS_TABLE}")
+        # shim in for sigma
+        self.query(f"DROP VIEW IF EXISTS sigma_labels")
         self.query(
-            self._jinja_environment.get_template(CREATE_ANALYTICS_TEMPLATE).render()
+            self._jinja_environment.get_template("create_sigma_results.sql").render()
         )
 
     def _is_table_or_view(self, table_name: str):
         try:
             self.query(f"describe {table_name}")
             logging.debug(f"table or view ({table_name}) already exists")
         except duckdb.CatalogException as err:
@@ -148,32 +145,14 @@
             time=int(event_time.strftime("%s")),
             # for now, we will simply support pid_hash as entity types
             entity_type=entity_type,
         )
         logging.debug(f"generated insert analtyic: {sql}")
         self._connection.execute(sql)
 
-    def insert_analytics_table(
-        self,
-        analytic_id: str,
-        technique_id: str,
-        technique_stix_type: str,
-        tactic_id: str,
-        tactic_stix_type: str,
-    ) -> None:
-        sql = self._jinja_environment.get_template(INSERT_ANALYTICS_TEMPLATE).render(
-            analytic_id=analytic_id,
-            technique_id=technique_id,
-            technique_stix_type=technique_stix_type,
-            tactic_id=tactic_id,
-            tactic_stix_type=tactic_stix_type,
-        )
-        logging.debug(f"generated insert analtyic: {sql}")
-        self._connection.execute(sql)
-
     def clear_table(self, table: str) -> None:
         """clear contents of a table in the connection. Mainly used after writing out table to file."""
         logging.debug(f"Clearing {table}")
         try:
             sql = f"DELETE FROM {table}"
             logging.debug(f"generated delete sql: {sql}")
             self._connection.execute(sql)
```

### Comparing `wintappy-0.1.2/wintappy/datautils/rawutil.py` & `wintappy-0.1.4/wintappy/datautils/rawutil.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,50 @@
 import logging
 import os
 import re
+import tempfile
+import time
 from collections import defaultdict
-from datetime import datetime
+from dataclasses import dataclass
 from glob import glob
+from importlib.resources import files as resource_files
+from typing import List, Optional
 
 import duckdb
 import pyarrow.parquet as pq
 from duckdb import CatalogException
-from importlib_resources import files
 from pyarrow.lib import ArrowInvalid
 
 
+@dataclass
+class SqlStmt:
+    name: str
+    sql: str
+    required: bool
+    template: Optional[str]
+
+
+class InvalidSchema(Exception):
+    """
+    Use to signal that the base schema doesn't match what we expect.
+    """
+
+    pass
+
+
 def init_db(dataset=None, agg_level="rolling", database=":memory:", lookups=""):
     """
     Initialize an in memory db instance and configure with our custom sql.
     """
     con = duckdb.connect(database=database)
+    # set caching dir to a temp directory location
+    con.execute(f"SET temp_directory = '{tempfile.mkdtemp()}'")
+    logging.debug(f"Duckdb info: {con.sql('CALL pragma_database_size()').fetchall()}")
     # TODO fix reference to SQL scripts
-    run_sql_no_args(con, files("wintappy.datautils").joinpath("initdb.sql"))
+    run_sql_no_args(con, resource_files("wintappy.datautils").joinpath("initdb.sql"))
     if not dataset == None:
         globs = get_glob_paths_for_dataset(dataset, agg_level, lookups=lookups)
         create_views(con, globs)
     return con
 
 
 def get_glob_paths_for_dataset(dataset, subdir="raw_sensor", include=None, lookups=""):
@@ -39,39 +61,46 @@
     dataset_path = os.path.join(dataset, subdir)
     event_types = [
         os.path.join(dataset_path, fn)
         for fn in os.listdir(dataset_path)
         if include == None or fn.startswith(include)
     ]
     # optionally add lookup directory
-    if lookups != "":
-        for lookup in os.listdir(lookups):
-            event_types.append(os.path.join(lookups, lookup))
+    for path, _, files in os.walk(lookups):
+        for name in files:
+            if name.endswith(".parquet") or name.endswith(".csv"):
+                event_types.append(os.path.join(path, name))
     globs = defaultdict(set)
     for cur_event in event_types:
-        event_type = cur_event.split("/")[-1]
+        event_type = cur_event.split(os.sep)[-1]
         if os.path.isdir(cur_event):
             for dirpath, dirnames, filenames in os.walk(cur_event):
                 if not dirnames:
                     if dirpath == cur_event:
                         # No dir globs needed
-                        globs[event_type].add(f"{cur_event}/*.parquet")
+                        globs[event_type].add(f"{cur_event}{os.sep}*.parquet")
                     else:
-                        # Remove the pre-fix, including event_type. Convert that to a glob.
+                        # Remove the prefix, including event_type. Convert that to a glob.
                         subdir = dirpath.replace(cur_event, "")
-                        glob = "/".join(["*"] * subdir.count(os.path.sep))
-                        globs[event_type].add(f"{cur_event}/{glob}/*.parquet")
+                        glob = os.sep.join(["*"] * subdir.count(os.path.sep))
+                        globs[event_type].add(
+                            os.path.join(cur_event, glob, "*.parquet")
+                        )
                         logging.debug(
                             f"{event_type} {subdir} {glob} has 0 subdirectories and {len(filenames)} files"
                         )
         else:
             # Treat as a simple, single file.
             if event_type.lower().endswith("parquet"):
                 event = re.split(r"\.", event_type)[0]
-                logging.info(f"{datetime.now()} Found {event} file: {event_type}")
+                logging.info(f"Found {event} file: {event_type}")
+                globs[event].add(cur_event)
+            elif event_type.lower().endswith("csv"):
+                event = re.split(r"\.", event_type)[0]
+                logging.info(f"Found {event} file: {event_type}")
                 globs[event].add(cur_event)
     return validate_globs(globs)
 
 
 def validate_globs(raw_data):
     """
     raw_data is a map of event_type -> list of globs.
@@ -113,15 +142,17 @@
     First, get the full glob paths for raw_sensor.  Then, splice in the dayPK specification.
     Finally, confirm that specific path exists and has files.
     """
     globs_all = get_glob_paths_for_dataset(dataset)
     globs = {}
     for event_type, pathspec in globs_all.items():
         # Add in the daypk filter
-        pathspec = pathspec.replace("/*/", f"/dayPK={daypk}/", 1)
+        pathspec = pathspec.replace(
+            f"{os.sep}*{os.sep}", f"{os.sep}dayPK={daypk}{os.sep}", 1
+        )
         num_files = len(glob(pathspec))
         if num_files == 0:
             logging.info(f"Not found: {pathspec}  Skipping")
         else:
             logging.info(f"Found {num_files} parquet files in {pathspec}")
             # Check for empty files. These confuse duckdb and lead to schema errors.
             for file in glob(pathspec):
@@ -142,148 +173,248 @@
             if len(glob(pathspec)) > 0:
                 globs[event_type] = pathspec
             else:
                 logging.info(f"Skipping empty path: {pathspec}")
     return globs
 
 
-def loadSqlStatements(file):
+def loadSqlStatements(file) -> List[SqlStmt]:
     """
-    Read sql script into map keyed by table name.
+    Read sql script. Parse into individual statements.
+
+    Optional metadata can be set for each statement. Must be provided AFTER the first line of sql:
+    --# name: [friendly name]
+    --# required
+    --# template: [path]
+
+    Name - defaults to tablename for CREATE, all others default to the first line with line number.
+    Best practice: for SELECT statements, provide a friendly name.
+
+    Required - applies only to CREATEs. If present, and create fails, an empty table will be built using a
+        parquet file located in ./schema/[template]/[name].parquet. Any data in the parquet will be ignored.
+
+    Template - applies only to CREATEs. The subdirectory within "./schema" that has the template parquet file.
     """
     file = open(file, "r")
     lines = file.readlines()
 
-    statements = {}
-    count = 0
-    # Strips the newline character
-    curKey = ""
-    curStatement = ""
-    for count, line in enumerate(lines):
-        if line.lower().startswith("create "):
+    statements = []
+    linenumber = 0
+    inStmt = False
+    for linenumber, line in enumerate(lines):
+        keyword = line.split(" ")[0].strip().lower()
+        if not inStmt and keyword in [
+            "create",
+            "alter",
+            "update",
+            "insert",
+            "delete",
+            "select",
+        ]:
+            # start of a new statement
             # For tables and views, use the object name
-            curKey = line.strip().split()[-1]
-            curStatement = line
-        elif line.lower().startswith("update "):
-            # Add line number to be sure its unique
-            curKey = f"{line.strip()}-{count}"
-            curStatement = line
+            if keyword == "create":
+                name = line.strip().split()[-1]
+            else:
+                # Add line number to be sure its unique as there can be multiple of these per table
+                name = f"{line.strip()}-{linenumber}"
+            curStatement = SqlStmt(
+                name=name,
+                sql=line,
+                required=False,
+                template=None,
+            )
+            inStmt = True
+        elif line.lower().startswith("--# name:"):
+            # Override default name with provided one.
+            curStatement.name = line.split(":")[1].strip()
+        elif line.lower().startswith("--# required"):
+            # This object is required to exist, so if execution fails, an empty object will be created with a matching schema.
+            curStatement.required = True
+        elif line.lower().startswith("--# template:"):
+            # Template identifies where the corresponding parquet template is that will be used for creating empty objects.
+            curStatement.template = line.split(":")[1].strip()
         else:
             if line.strip() == ";":
                 # We done. Save the statement. Don't save the semi-colon.
-                statements[curKey] = curStatement
-                curStatement = "SKIP"
+                statements.append(curStatement)
+                inStmt = False
+                logging.debug(curStatement.sql)
             else:
-                if curStatement != "SKIP":
-                    curStatement += line
+                if inStmt:
+                    curStatement.sql += line
     return statements
 
 
 def generate_view_sql(event_map, start=None, end=None):
     """
     Create SQL for each of the event_types in the map.
     """
     # View Template
     stmts = []
     for event_type, pathspec in event_map.items():
+        if "raw_" in event_type and "/raw_sensor/" in pathspec:
+            # Raw files *may* have differing schemas, so enable union'ing of all schemas.
+            # FIX in Wintap(?): Found that exact dups are in the raw tables, so remove them here using the GROUP BY ALL.
+            # Only implement duplicate fix on 'raw_sensor' path. RAW tables in 'rolling' are already fixed.
+            view_sql = get_raw_view(event_type, pathspec)
+        elif pathspec.endswith(".csv"):
+            view_sql = f"""
+            create or replace view {event_type} as
+            select * from read_csv('{pathspec}', AUTO_DETECT=TRUE)
+            """
+        else:
+            view_sql = f"""
+            create or replace view {event_type} as
+            select * from parquet_scan('{pathspec}',hive_partitioning=1)
+            """
+            # Apply start/end filtering for rolling tables only.
+            if "/rolling/" in pathspec:
+                if start and end:
+                    view_sql += f"where dayPK between {start} and {end}"
+                if start is not None and end is None:
+                    view_sql += f"where dayPK = {start}"
+        if view_sql:
+            stmts.append(view_sql)
+            logging.debug(f"View for {event_type} using {pathspec}")
+            logging.debug(view_sql)
+    return stmts
+
+
+def get_raw_view(event_type: str, pathspec):
+    """
+    The introduction of agentid causes a ripple effect thru all ETL SQL.
+    For as long as is reasonable, auto-detect incoming parquet and add a null agentid when missing.
+    This allows for processing of older data sets.
+    At some point, a new, breaking schema change will happen and a different approach will be needed.
+    """
+
+    # Get the schema from the first parquet file
+    schema = pq.read_schema(glob(pathspec)[0])
+    if "agentid" in schema.names:
         view_sql = f"""
         create or replace view {event_type} as
-        select * from parquet_scan('{pathspec}',hive_partitioning=1)
+        select *, count(*) num_dups from parquet_scan('{pathspec}',hive_partitioning=1,union_by_name=true) group by all
         """
-        if start != None and end != None:
-            stmt += f"where dayPK between {start} and {end}"
-        if start != None and end == None:
-            stmt += f"where dayPK = {start}"
-        stmts.append(view_sql)
-        logging.debug(f"View for {event_type} using {pathspec}")
-        logging.debug(view_sql)
-    return stmts
+    else:
+        view_sql = f"""
+        create or replace view {event_type} as
+        select *, cast(null as varchar) agentid, count(*) num_dups from parquet_scan('{pathspec}',hive_partitioning=1,union_by_name=true) group by all
+        """
+    return view_sql
 
 
-def create_views(con, event_map):
-    stmts = generate_view_sql(event_map)
+def create_views(con, event_map, start=None, end=None):
+    stmts = generate_view_sql(event_map, start, end)
     for sql in stmts:
         cursor = con.cursor()
-        cursor.execute(sql)
-        cursor.close()
+        try:
+            cursor.execute(sql)
+        except duckdb.duckdb.IOException as e:
+            logging.error(f"SQL Failed: {sql}", e)
+            logging.error("If the error is too many files open, try this on OSX:")
+            logging.error("ulimit -Sn 524288; ulimit -Hn 10485760")
+            raise e
+        finally:
+            cursor.close()
+
+
+def validate_raw_views(con, raw_data, start=None, end=None):
+    """
+    Due to the variability in sensor configuration and collection issues, this hook is here to allow validating
+    and possibly fixing, known problems:
+    * In some cases, there are no raw_process_stop.parquet files which leads to all the unique fields defined in
+      it to be missing, causing downstream SQL errors. Fixed here by copying in an empty parquet file.
+    """
+
+    if "raw_process" in raw_data.keys():
+        # Validate existence of raw_process_stop fields. Shortcut by just checking for 1 for now.
+        col_sql = """
+            select table_catalog, table_name, column_name
+            from information_schema.columns
+            where table_name ilike 'raw_process'
+            and lower(column_name)=lower('CPUCycleCount')
+            """
+        if con.sql(col_sql).count("*").fetchone()[0] == 0:
+            # It's missing, create the empty file from the template
+            src_file = resource_files("wintappy.schema.raw_sensor").joinpath(
+                "raw_processstop.parquet"
+            )
+            # Destination will be the pathspec for raw_process, with a little tweaking:
+            pathspec = raw_data["raw_process"]
+            basepath = pathspec.split("*")[0]
+            dest_file = os.path.join(
+                basepath,
+                "hourPK=00",
+                f"EMPTY-raw_processstop-{int(time.time())}.parquet",
+            )
+            # Create the file by querying from template with the right schema
+            logging.info(f"Creating empty raw_processstop.parquet in {pathspec}")
+            con.execute(
+                f"copy (select * from '{src_file}' where false) to '{dest_file}'"
+            )
+            # Finally, recreate the raw_view.
+            create_views(con, {"raw_process": pathspec}, start, end)
 
 
 def create_raw_views(con, raw_data, start=None, end=None):
     """
     Create views in the db for each of the event_types.
     """
-    create_views(con, raw_data)
-
-    # For now, processing REQUIREs that RAW_PROCESS_STOP exist even if its empty. Create an empty table if needed.
-    create_empty_process_stop(con)
+    create_views(con, raw_data, start, end)
+    validate_raw_views(con, raw_data, start, end)
 
 
-def create_empty_process_stop(con):
-    """
-    The current processing expects there to always be a RAW_PROCESS_STOP table for the final step for PROCESS.
-    This function is used to create an empty table with the right structure for cases where there were no PROCESS_STOP events reported.
+def create_empty_table(con, sqlstmt: SqlStmt):
     """
-    db_objects = con.execute(
-        "select table_name, table_type from information_schema.tables where table_schema='main' and lower(table_name)='raw_process_stop'"
-    ).fetchall()
-    if len(db_objects) == 0:
-        logging.info("Creating empty RAW_PROCESS_STOP")
-        cursor = con.cursor()
-        cursor.execute(
-            """
-        CREATE TABLE raw_process_stop (
-            PidHash VARCHAR,
-            ParentPidHash VARCHAR,
-            CPUCycleCount BIGINT,
-            CPUUtilization INTEGER,
-            CommitCharge BIGINT,
-            CommitPeak BIGINT,
-            ReadOperationCount BIGINT,
-            WriteOperationCount BIGINT,
-            ReadTransferKiloBytes BIGINT,
-            WriteTransferKiloBytes BIGINT,
-            HardFaultCount INTEGER,
-            TokenElevationType INTEGER,
-            ExitCode BIGINT,
-            MessageType VARCHAR,
-            Hostname VARCHAR,
-            ActivityType VARCHAR,
-            EventTime BIGINT,
-            ReceiveTime BIGINT,
-            PID INTEGER,
-            IncrType VARCHAR,
-            EventCount INTEGER,
-            FirstSeenMs BIGINT,
-            LastSeenMs BIGINT
-        )
-        """
+    Create an empty table from a parquet used as the template for the schema.
+    This is useful when no data exists, but the structural element (table) is required for later SQL.
+
+    template
+    """
+    fqfn = resource_files(f"wintappy.schema.{sqlstmt.template}").joinpath(
+        f"{sqlstmt.name}.parquet"
+    )
+    logging.debug(f"Creating empty table from: {fqfn}")
+    sql = f"create table {sqlstmt.name} as select * from '{fqfn}' where False"
+    try:
+        con.execute(sql)
+    except CatalogException as e:
+        logging.warning(
+            f"Warning! Failed to create empty table for {sqlstmt.name} due to:\n{e}"
         )
-        cursor.close()
 
 
 def run_sql_no_args(con, sqlfile):
     """
     Execute all SQL statements in the file without binding any parameters.
-    Format should SQL delimited with semi-colons. Comments are allowed SQL
+    Format should be SQL statements (DDL) delimited with semi-colons. Comments are allowed SQL
     style:
        -- for single line
        /*
        Multi-line
        */
     """
     etl_sql = loadSqlStatements(sqlfile)
-    for key in etl_sql:
-        logging.info(f"Processing: {key}")
+    for sqlstmt in etl_sql:
+        logging.info(f"Processing: {sqlstmt.name}")
         try:
-            con.execute(etl_sql[key])
+            con.execute(sqlstmt.sql)
         except CatalogException as e:
-            logging.info(f"No raw data for {key}")
+            logging.info(f"Missing dependent table/view for {sqlstmt.name}")
+            logging.debug(f"Error: {e}\nSQL: {sqlstmt.sql}")
+            if sqlstmt.required:
+                logging.info(f"Creating empty object from {sqlstmt.template}")
+                create_empty_table(con, sqlstmt)
+        except duckdb.BinderException as e:
+            logging.error(f"Likely missing column: \n{e}")
+            raise InvalidSchema(f"Likely missing column: \n{e}")
         except Exception as e:
-            logging.info(f"  Failed: {e}")
-            logging.info(type(e))
+            logging.error(f"  Failed: {e}")
+            raise
 
 
 def get_db_objects(con, exclude=None):
     """
     Get all tables/views defined in the db.
     exclude should be a list of strings. If the strings appear in the object names, they'll be dropped from the result.
     """
@@ -295,32 +426,32 @@
         tables = [t for t, x in db_objects if not any(e in t for e in exclude)]
         logging.debug(f"Not Matches: {tables}")
     else:
         tables = [t for t, x in db_objects]
     return tables
 
 
-def write_parquet(con, datasetpath, db_objects, daypk=None):
+def write_parquet(con, datasetpath, db_objects, daypk=None, agg_level="stdview"):
     """
     Write tables/views from duckdb instance to parquet.
     If daypk is provided, write to corresponding path in rolling.
-    Otherwise, write to stdview.
+    Otherwise, write to agg_level.
     """
     for object_name in db_objects:
         logging.info(f"Writing {object_name}")
         try:
             if daypk == None:
-                pathspec = f"{datasetpath}/stdview"
+                pathspec = f"{datasetpath}{os.sep}{agg_level}"
                 filename = f"{object_name}.parquet"
             else:
-                pathspec = f"{datasetpath}/rolling/{object_name}/dayPK={daypk}"
+                pathspec = f"{datasetpath}{os.sep}rolling{os.sep}{object_name}{os.sep}dayPK={daypk}"
                 filename = f"{object_name}-{daypk}.parquet"
             if not os.path.exists(pathspec):
                 os.makedirs(pathspec)
                 logging.debug(f"created folder: {pathspec} ")
             else:
                 logging.debug(f"folder already exists: {pathspec}")
             # TODO Add test for file existence
-            sql = f"COPY {object_name} TO '{pathspec}/{filename}' (FORMAT 'parquet')"
+            sql = f"COPY {object_name} TO '{pathspec}{os.sep}{filename}' (FORMAT 'parquet')"
             con.execute(sql)
         except duckdb.IOException as e:
             logging.exception(f"Failed to write: {object_name}")
```

### Comparing `wintappy-0.1.2/wintappy/datautils/stdview_duckdb.py` & `wintappy-0.1.4/wintappy/datautils/stdview_duckdb.py`

 * *Files 24% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             "tb(EventTime)",
             "count(*)",
         )
     )
     return esm
 
 
-def create_event_summary_view(con):
+def create_event_summary_view(con, min_daypk, max_daypk):
     """
     Create a view for all known raw event types.
     To add a new type, define in the event_summary_metadata.
     """
     esms = event_summary_metadata()
     tablesDF = con.execute(
         "select table_name from information_schema.tables where table_name like 'raw_%'"
@@ -93,71 +93,99 @@
     logging.info(f"Missing: {set(db_tables) - set(esm.table for esm in esms)}")
 
     template = """
     CREATE OR replace VIEW event_summary_raw_v1
     AS
     {%- for esm in esms %}
     SELECT '{{esm.label}}' as Event,
-    {{esm.host_col}} as Hostname,
+    upper({{esm.host_col}}) as Hostname,
     {{esm.ts_func}} bin_date,
     {{esm.num_event_func}} NumRows
     FROM {{esm.table}}
+    WHERE dayPK between {{min_daypk}} and {{max_daypk}}
     GROUP BY ALL
     {% if not loop.last %}UNION{% endif %}
     {%- endfor %}
     """
 
-    sql = Template(template).render(esms=tables)
+    sql = Template(template).render(
+        esms=tables, min_daypk=min_daypk, max_daypk=max_daypk
+    )
     logging.debug(f"Generated summary view: {sql}")
     con.execute(sql)
 
 
-def init_db(con, bucket_size="30 minutes"):
+def init_db(con, min_dayPK, max_dayPK):
     # Create a macro (function) that will create the time bins.
     # To do: derive the intertotal_size based on the dataset time range and the desired target number of data points. The data points size directly affects performance of the chart. Too fine-grained isn't generally useful.
+
+    # Move this into stdview_duckdb and make behavior the default...
+
+    bucket_size = str((max_dayPK - min_dayPK) / 500)
+
+    # Once min/max are calc'd here, they can be passed into creating the view
     con.execute(
-        f"create or replace macro tb(wts) as time_bucket(interval '{bucket_size}', to_timestamp_micros(win32_to_epoch(wts)))"
+        f"create or replace macro tb(wts) as time_bucket(interval '{bucket_size}', cast(to_timestamp_micros(win32_to_epoch(wts)) as timestamp))"
+    )
+    # Convert from Timestamps to int
+    create_event_summary_view(
+        con, int(min_dayPK.strftime("%Y%m%d")), int(max_dayPK.strftime("%Y%m%d"))
     )
-    create_event_summary_view(con)
 
 
-def duckdb_table_metadata(con):
+def duckdb_table_metadata(con, include_paritioned_data=True):
     # Ignore objects ending in _v1 as they are likely complex view and can be expensive to count.
+    in_clause = "IN" if include_paritioned_data else "NOT IN"
     tablesDF = con.execute(
-        "select table_name from information_schema.tables where table_name not like '%_v1' order by all"
+        f"select table_name from information_schema.tables where table_name not like '%_v1' and table_name {in_clause} ( select table_name from information_schema.columns WHERE column_name = 'dayPK' ) order by all"
     ).df()
     tables = tablesDF["table_name"].tolist()
-    template = """
-    {%- for table in tables %}
-    SELECT '{{table}}' as Table_Name, min(daypk) Min_DayPK, max(daypk) Max_DayPK, count(*) as Num_Rows
-    FROM {{table}}
-    {% if not loop.last %}UNION{% endif %}
-    {%- endfor %}
-    ORDER BY table_name
-    """
-
-    sql = Template(template).render(tables=tables)
-    logging.debug(f"Generated sql: {sql}")
-    return con.execute(sql).df()
-
-
-def table_summary(con, dataset, agg_level="rolling"):
+    if include_paritioned_data:
+        template = """
+        {%- for table in tables %}
+        SELECT '{{table}}' as Table_Name, min(daypk) Min_DayPK, max(daypk) Max_DayPK, count(*) as Num_Rows
+        FROM {{table}}
+        {% if not loop.last %}UNION ALL{% endif %}
+        {%- endfor %}
+        ORDER BY table_name
+        """
+    else:
+        template = """
+        {%- for table in tables %}
+        SELECT '{{table}}' as Table_Name, count(*) as Num_Rows
+        FROM {{table}}
+        {% if not loop.last %}UNION ALL{% endif %}
+        {%- endfor %}
+        ORDER BY table_name
+        """
+
+    if not tablesDF.empty:
+        sql = Template(template).render(tables=tables)
+        logging.debug(f"Generated sql: {sql}")
+        return con.execute(sql).df()
+    else:
+        return tablesDF
+
+
+def table_summary(
+    con, dataset, lookups="", agg_level="rolling", include_paritioned_data=True
+):
     """
     Get the list of tables defined in duckdb, then add sizes for the associated parquet files.
     """
-    tablesDF = duckdb_table_metadata(con)
-
-    globs = ru.get_glob_paths_for_dataset(dataset, agg_level)
-    for event, glob in globs.items():
-        cur_size = cur_files = 0
-        for file in iglob(glob):
-            cur_size += os.path.getsize(file)
-            cur_files += 1
-        tablesDF.loc[tablesDF.Table_Name == event, "Size"] = format_size(cur_size)
-        tablesDF.loc[tablesDF.Table_Name == event, "Files"] = cur_files
+    tablesDF = duckdb_table_metadata(con, include_paritioned_data)
+    if not tablesDF.empty:
+        globs = ru.get_glob_paths_for_dataset(dataset, agg_level, lookups=lookups)
+        for event, glob in globs.items():
+            cur_size = cur_files = 0
+            for file in iglob(glob):
+                cur_size += os.path.getsize(file)
+                cur_files += 1
+            tablesDF.loc[tablesDF.Table_Name == event, "Size"] = format_size(cur_size)
+            tablesDF.loc[tablesDF.Table_Name == event, "Files"] = cur_files
     return tablesDF
 
 
 def fetch_summary_data(con):
     eventDF = con.execute(
         'select "Event", "Hostname",bin_date as BinDT,"NumRows" from event_summary_raw_v1 order by all'
     ).df()
@@ -178,35 +206,69 @@
         # Hmm, need positive total_size for a sensible marker size. Shift'em. Note: min is assumed to always be < 0.
         eventDF.loc[eventDF.Event == event, "NumRowsRobust"] = (
             eventDF["NumRowsRobust"] + eventDF["NumRowsRobust"].min() * -1 + 0.5
         ) * sizeMx
     return eventDF
 
 
-def display_event_chart(eventDF):
-    # Set jupyter options
-    pd.set_option("display.max_columns", None)
-    pd.set_option("display.max_colwidth", None)
-
+def create_event_chart(eventDF):
     # Set altair options
     alt.data_transformers.disable_max_rows()
 
-    allEvents = eventDF
-
     # Create a compound key for the Y. Can't seem to specify it in the altair syntax
-    allEvents["Hostname+Event"] = allEvents["Hostname"] + ": " + allEvents["Event"]
+    allEvents = eventDF.assign(Hostname_Event=lambda x: x.Hostname + ": " + x.Event)
 
     eventsChart = (
         alt.Chart(allEvents)
         .mark_circle()
         .encode(
-            x="BinDT",
-            y="Hostname+Event",
+            alt.X("BinDT"),
+            alt.Y("Hostname_Event"),
             # size=alt.Size('NumRowsRobust:N', scale=None),
+            alt.Size(
+                "NumRows:Q",
+                scale=alt.Scale(range=[0, 4000]),
+                legend=alt.Legend(title="Events per bucket"),
+            ),
             # size=20,
             color="Event",
             tooltip=["Hostname:N", "Event:N", "NumRows:Q", "BinDT"],
         )
-        .properties(width=1200, height=600, title="Raw Events over Time")
+        .properties(title="Raw Events over Time")
         .interactive()
     )
-    display(eventsChart)
+    return eventsChart
+
+
+def display_event_chart(eventDF, width=1200, height=600):
+    # Set jupyter options
+    pd.set_option("display.max_columns", None)
+    pd.set_option("display.max_colwidth", None)
+
+    display(create_event_chart(eventDF).properties(width=width, heigh=height))
+
+
+def create_data_summary(datasummaryDF):
+    # Create line charts for many features. Each chart will then have its own Y-Scale
+    # Set altair options
+    alt.data_transformers.disable_max_rows()
+
+    hostChart = (
+        alt.Chart(datasummaryDF)
+        .mark_line(interpolate="monotone")
+        .encode(
+            alt.X("bucket_day"),
+            alt.Y("hosts"),
+            tooltip=["bucket_day"],
+        )
+    )
+    uniqProcessChart = (
+        alt.Chart(datasummaryDF)
+        .mark_line(interpolate="monotone", stroke="grey")
+        .encode(
+            alt.X("bucket_day"),
+            alt.Y("uniq_processes"),
+            tooltip=["bucket_day"],
+        )
+    )
+
+    return (hostChart + uniqProcessChart).resolve_scale(y="independent").interactive()
```

### Comparing `wintappy-0.1.2/wintappy/datautils/stdviewutil.py` & `wintappy-0.1.4/wintappy/datautils/stdviewutil.py`

 * *Files identical despite different names*

### Comparing `wintappy-0.1.2/wintappy/datautils/wintapgraph.py` & `wintappy-0.1.4/wintappy/datautils/wintapgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Functions for creating graph data structures from wintap dataframes
 """
-import matplotlib
-import matplotlib.pyplot as plt
+
 import networkx as nx
 import pandas as pd
 
 
 def add_proc_node_for(g, pid_hashes, procdf):
     proc = procdf.loc[procdf["pid_hash"].isin(pid_hashes)]
     print(f"Adding {proc.shape[0]} process nodes")
```

### Comparing `wintappy-0.1.2/wintappy/etlutils/collectbinaries.py` & `wintappy-0.1.4/wintappy/etlutils/collectbinaries.py`

 * *Files identical despite different names*

### Comparing `wintappy-0.1.2/wintappy/etlutils/download_from_s3.py` & `wintappy-0.1.4/wintappy/etlutils/downloadfroms3.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,48 +15,48 @@
 import argparse
 import csv
 import logging
 import os
 import sys
 import traceback
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from functools import partial
-from typing import NamedTuple
 
 import boto3
 import botocore
 import tqdm
 
+from wintappy.config import EnvironmentConfig
+from wintappy.etlutils.utils import configure_basic_logging, get_date_range
+
 # Maximum number of open HTTP(s) connections
 MAX_POOL_CONNECTIONS = 50
 # Maximum S3 download threads
 MAX_WORKERS = 32
 # Maximum number of retries for failed downloads
 MAX_RETRIES = 3
 
 
-S3File = NamedTuple(
-    "S3File",
-    [
-        ("key", str),
-        ("filename", str),
-        ("s3_path", str),
-        ("hostname", str),
-        ("data_capture_ts", datetime),
-        ("uploadedDPK", str),
-        ("uploadedHPK", str),
-        ("dataDPK", str),
-        ("dataHPK", str),
-        ("local_file_path", str),
-        ("os", str),
-        ("sensor_version", str),
-        ("event_type", str),
-    ],
-)
+@dataclass
+class S3File:
+    key: str
+    filename: str
+    s3_path: str
+    hostname: str
+    data_capture_ts: datetime
+    uploadedDPK: str
+    uploadedHPK: str
+    dataDPK: str
+    dataHPK: str
+    local_file_path: str
+    os: str
+    sensor_version: str
+    event_type: str
 
 
 def list_files(s3_client, bucket, prefix):
     """
     Lists all files, at any folder level, under the given prefix.
     No folders (CommonPrefixes) are returned as there is no delimiter given.
     """
@@ -208,29 +208,40 @@
     else:
         hostname = filename.split("+")[0]
         # Drop the '.parquet' also
         data_capture_epoch = filename.split("+")[2].split(".")[0]
     return hostname, data_capture_epoch
 
 
-def parse_s3_metadata(files, local_path, uploadedDPK, uploadedHPK, event_type):
+def parse_s3_metadata(files, dataset, uploadedDPK, uploadedHPK, event_type):
     """
     Parse metadata from S3. This will be used for generating the correct path to write to.
     TODO: Write this data also to a parquet file for metadata analytics.
     """
     # Prefix all event_types with "raw_" TODO: fix this in Wintap
     if event_type.lower().startswith("raw_"):
         new_event_type = event_type
     else:
         new_event_type = "raw_" + event_type
+
+    # Modify some event names to what SQL expects
+    # To Do: Fix this in Wintap
+    if new_event_type == "raw_file":
+        new_event_type = "raw_process_file"
+    if new_event_type == "raw_registry":
+        new_event_type = "raw_process_registry"
+    if new_event_type == "raw_processstop":
+        # Put process_stop in with process.
+        new_event_type = "raw_process"
+
     files_metadata = []
     back_dated = {}
     for file in files:
         try:
-            (s3_path, delim, filename) = file.get("Key").rpartition("/")
+            (s3_path, _, filename) = file.get("Key").rpartition("/")
             hostname, data_capture_epoch = parse_filename(filename)
             data_capture_ts = datetime.fromtimestamp(
                 int(data_capture_epoch), timezone.utc
             )
             datadpk = data_capture_ts.strftime("%Y%m%d")
             datahpk = data_capture_ts.strftime("%H")
             # Data date can be different! Thats ok, it just means the host got delayed sending for some reason.
@@ -238,15 +249,15 @@
             if datadpk != uploadedDPK or datahpk != uploadedHPK:
                 # Key by data date.
                 back_dated[(datadpk, datahpk)] = (
                     back_dated.get((datadpk, datahpk), 0) + 1
                 )
 
             # Define fully-qualified local name
-            local_file_path = f"{local_path}/raw_sensor/{new_event_type}/dayPK={datadpk}/hourPK={datahpk}"
+            local_file_path = f"{dataset}/raw_sensor/{new_event_type}/dayPK={datadpk}/hourPK={datahpk}"
 
             s3File = S3File(
                 file.get("Key"),
                 filename,
                 s3_path,
                 hostname,
                 data_capture_ts,
@@ -264,93 +275,102 @@
             logging.error(f"Filename parse error on: s3_path: {s3_path} {filename}")
             logging.error(traceback.format_exc())
     if len(back_dated) > 0:
         logging.info(f"Back dated data: {back_dated}")
     return files_metadata
 
 
-def main():
+def main(argv=None) -> None:
+    configure_basic_logging()
     parser = argparse.ArgumentParser(
-        prog="downloadFromS3.py", description="Download Wintap files from S3"
-    )
-    parser.add_argument("--profile", help="AWS profile to use", required=False)
-    parser.add_argument("-b", "--bucket", help="The S3 bucket", required=True)
-    parser.add_argument(
-        "-p", "--prefix", help="S3 prefix within the bucket", required=True
-    )
-    parser.add_argument("-s", "--start", help="Start date (YYYYMMDD HH)", required=True)
-    parser.add_argument("-e", "--end", help="End date (YYYYMMDD HH)", required=True)
-    parser.add_argument(
-        "-l", "--localpath", help="Local path to write files", required=True
+        prog="downloadfromS3.py", description="Download Wintap files from S3"
     )
-    parser.add_argument(
-        "--log-level", default="INFO", help="Logging Level: INFO, WARN, ERROR, DEBUG"
-    )
-    args = parser.parse_args()
+    env_config = EnvironmentConfig(parser)
+    env_config.add_aws_settings(required=True)
+    env_config.add_start(required=True)
+    env_config.add_end(required=True)
 
-    try:
-        logging.basicConfig(
-            level=args.log_level,
-            format="%(asctime)s %(message)s",
-            datefmt="%m/%d/%Y %I:%M:%S %p",
-        )
-    except ValueError:
-        logging.error("Invalid log level: {}".format(args.log_level))
-        sys.exit(1)
+    # setup config based on env variables and config file
+    args = env_config.get_options(argv)
 
-    if args.profile:
-        session = boto3.Session(profile_name=args.profile)
+    if args.AWS_PROFILE:
+        session = boto3.Session(profile_name=args.AWS_PROFILE)
     else:
         session = boto3.Session()
-    s3 = session.client("s3", config=botocore.client.Config(max_pool_connections=50))
+    if args.AWS_REGION:
+        s3 = session.client(
+            "s3",
+            config=botocore.client.Config(max_pool_connections=50),
+            region_name=args.AWS_REGION,
+        )
+    else:
+        s3 = session.client(
+            "s3", config=botocore.client.Config(max_pool_connections=50)
+        )
 
-    files, folders = list_folders(s3, bucket=args.bucket, prefix=args.prefix)
+    top_level_prefix = (
+        args.AWS_S3_PREFIX
+        if args.AWS_S3_PREFIX.endswith("/")
+        else f"{args.AWS_S3_PREFIX}/"
+    )
+    files, folders = list_folders(
+        s3, bucket=args.AWS_S3_BUCKET, prefix=top_level_prefix
+    )
 
     # Top level is event types
     event_types = folders
+    start_date, end_date = get_date_range(
+        args.START, args.END, date_format="%Y%m%d %H", data_set_path=args.DATASET
+    )
 
-    start_date = datetime.strptime(args.start, "%Y%m%d %H")
-    end_date = datetime.strptime(args.end, "%Y%m%d %H")
-
+    logging.info(f"Using time range: {start_date} -> {end_date}")
     for event_type in event_types:
-        logging.info(event_type.get("Prefix"))
+        logging.info(f'S3 EventType Prefix: {event_type.get("Prefix")}')
         # Within an event type, iterate over date range by hour
         files_md = []
         for single_date in hour_range(start_date, end_date):
             daypk = single_date.strftime("%Y%m%d")
             hourpk = single_date.strftime("%H")
+            logging.debug(f"daypk={daypk}; hourpk={hourpk}")
+
+            # Note: 'Prefix' includes a trailing slash.
             prefix = (
                 f"{event_type.get('Prefix')}uploadedDPK={daypk}/uploadedHPK={hourpk}/"
             )
+
             # Optimization: many event types are sparsely populated, so enumerate the dayPK/hourPK structure, then just get files from the ones that exist.
             files_tmp, existing_S3_paths = list_folders(
                 s3,
-                bucket=args.bucket,
+                bucket=args.AWS_S3_BUCKET,
                 prefix=f"{event_type.get('Prefix')}uploadedDPK={daypk}/",
             )
             # list_folders returns a JSON list. Extract the paths as a simple string list
             existing_S3_paths = [x.get("Prefix") for x in existing_S3_paths]
             if prefix in existing_S3_paths:
-                files, folders = list_files(s3, bucket=args.bucket, prefix=prefix)
+                files, folders = list_files(
+                    s3, bucket=args.AWS_S3_BUCKET, prefix=prefix
+                )
                 if len(files) > 0 or len(folders) > 0:
                     logging.debug(f"  {prefix}")
                     logging.debug(f"    Files: {len(files)}  Folders: {len(folders)}")
                     files_md.extend(
                         parse_s3_metadata(
                             files,
-                            args.localpath,
+                            args.DATASET,
                             daypk,
                             hourpk,
                             event_type.get("Prefix").split("/")[2],
                         )
                     )
                 logging.info(
                     f"  {prefix}  Files: {len(files)}  Folders: {len(folders)}  Total: {len(files_md)}"
                 )
             else:
                 logging.debug(f"  {prefix} not in S3, skipping")
-        logging.info(f"   Downloading {len(files_md)}...")
-        download_files_threaded(args.bucket, s3, files_md)
+
+        if len(files_md) > 0:
+            logging.info(f"   Downloading {len(files_md)}...")
+            download_files_threaded(args.AWS_S3_BUCKET, s3, files_md)
 
 
 if __name__ == "__main__":
-    main()
+    main(argv=None)
```

### Comparing `wintappy-0.1.2/wintappy/etlutils/run_enrichment.py` & `wintappy-0.1.4/wintappy/etlutils/run_enrichment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 import argparse
+import dataclasses
 import json
 import logging
 import sys
 from datetime import datetime
 
 import fsspec
 
 from wintappy.analytics.constants import TACTIC_STIX_TYPE, TECHNIQUE_STIX_TYPE
 from wintappy.analytics.utils import load_attack_metadata, run_against_day
+from wintappy.config import EnvironmentConfig
 from wintappy.database.constants import (
-    ANALYTICS_RESULTS_TABLE,
-    ANALYTICS_TABLE,
-    LOOKUPS_DIR,
+    CAR_ANALYTIC_COVERAGE,
+    CAR_ANALYTICS_RESULTS_TABLE,
+    CAR_ANALYTICS_TABLE,
+    MITRE_DIR,
     TACTICS_TABLE,
     TECHNIQUES_TABLE,
 )
 from wintappy.etlutils.transformer_manager import TransformerManager
-from wintappy.etlutils.utils import daterange
+from wintappy.etlutils.utils import configure_basic_logging, daterange, get_date_range
 
 
 def add_enrichment_tables(
     manager: TransformerManager, enrichment_location: str
 ) -> None:
-    # first, load analytics metadata
-    for analytic_id in manager.analytics:
-        for entry in manager.analytics[analytic_id].coverage:
-            for t in entry.tactics:
-                manager.wintap_duckdb.insert_analytics_table(
-                    analytic_id=analytic_id,
-                    technique_id=entry.technique,
-                    technique_stix_type=TECHNIQUE_STIX_TYPE,
-                    tactic_id=t,
-                    tactic_stix_type=TACTIC_STIX_TYPE,
-                )
-    # write out the tables
-    manager.wintap_duckdb.write_table(
-        ANALYTICS_TABLE, location=f"{enrichment_location}/{LOOKUPS_DIR}"
-    )
-    # clear out results table that we just wrote out to the fs
-    manager.wintap_duckdb.clear_table(ANALYTICS_TABLE)
-
-    # Next, load tactic and technique metadata
+    # setup metadata tables
     mitre_attack_data = load_attack_metadata()
     metadata_tables = {
+        CAR_ANALYTICS_TABLE: list(
+            map(
+                lambda x: x.table_item(),
+                manager.analytics.values(),
+            )
+        ),
+        CAR_ANALYTIC_COVERAGE: [
+            item
+            for obj in manager.analytics.values()
+            for item in obj.coverage_table_items()
+        ],
         TECHNIQUES_TABLE: list(
             map(
                 lambda x: json.loads(x.serialize()),
                 mitre_attack_data.get_techniques(remove_revoked_deprecated=True),
             )
         ),
         TACTICS_TABLE: list(
@@ -61,94 +57,92 @@
         table_name_internal = f"{table_name}_internal"
         with fsspec.filesystem("memory").open(
             f"{table_name_internal}.json", "w"
         ) as file:
             file.write(json.dumps(table_data))
         # Register the memory filesystem and create the table
         manager.wintap_duckdb.register_filesystem(fsspec.filesystem("memory"))
-        manager.wintap_duckdb.query(
-            f"CREATE TABLE IF NOT EXISTS {table_name_internal} AS SELECT * FROM read_json_auto('memory://{table_name_internal}.json')"
-        )
-        # Insert the data into the table
-        manager.wintap_duckdb.query(
-            f"INSERT INTO {table_name_internal} SELECT * FROM read_json_auto('memory://{table_name_internal}.json')"
-        )
-        # Now we need to unnest the data
-        manager.wintap_duckdb.query(
-            f"CREATE OR REPLACE VIEW {table_name} as select unnest(external_references).external_id as external_id, * from {table_name_internal}"
-        )
+        if table_name in [TECHNIQUES_TABLE, TACTICS_TABLE]:
+            manager.wintap_duckdb.query(
+                f"CREATE TABLE IF NOT EXISTS {table_name_internal} AS SELECT * FROM read_json_auto('memory://{table_name_internal}.json')"
+            )
+            # Insert the data into the table
+            manager.wintap_duckdb.query(
+                f"INSERT INTO {table_name_internal} SELECT * FROM read_json_auto('memory://{table_name_internal}.json')"
+            )
+            # Now we need to unnest the data
+            manager.wintap_duckdb.query(
+                f"CREATE OR REPLACE VIEW {table_name} as select unnest(external_references).external_id as external_id, * from {table_name_internal}"
+            )
+        else:
+            manager.wintap_duckdb.query(f"DROP TABLE IF EXISTS {table_name}")
+            manager.wintap_duckdb.query(
+                f"CREATE TABLE IF NOT EXISTS {table_name} AS SELECT * FROM read_json_auto('memory://{table_name_internal}.json')"
+            )
         # finally, write out the tables
         manager.wintap_duckdb.write_table(
-            table_name, location=f"{enrichment_location}/{LOOKUPS_DIR}"
+            table_name, location=f"{enrichment_location}/{MITRE_DIR}"
         )
     return
 
 
 def process_range(
     manager: TransformerManager, start_date: datetime, end_date: datetime
 ) -> None:
     # run analytics against input range
     analytics_list = list(manager.analytics.values())
     for single_date in daterange(start_date, end_date):
         daypk = int(single_date.strftime("%Y%m%d"))
         logging.debug(f"running with daypk: {daypk}")
         # run analytics against this day
         run_against_day(
-            daypk, manager.jinja_environment, manager.wintap_duckdb, analytics_list
-        )
-        # write results out to the fs for this day
-        manager.wintap_duckdb.write_table(
-            ANALYTICS_RESULTS_TABLE, daypk, location=manager.dataset_path
+            manager.jinja_environment,
+            manager.wintap_duckdb,
+            analytics_list,
+            daypk=daypk,
         )
-        # clear out results table that we just wrote out to the fs
-        manager.wintap_duckdb.clear_table(ANALYTICS_RESULTS_TABLE)
     return
 
 
-def main():
+def process_table(manager: TransformerManager) -> None:
+    # run analytics against single table
+    analytics_list = list(manager.analytics.values())
+    logging.debug("running without daypk")
+    # run analytics against this day
+    run_against_day(manager.jinja_environment, manager.wintap_duckdb, analytics_list)
+    return
+
+
+def main(argv=None):
+    configure_basic_logging()
     parser = argparse.ArgumentParser(
         prog="run_enrichment.py",
         description="Run enrichements against wintap data, write out results partitioned by day",
     )
-    parser.add_argument(
-        "-d", "--dataset", help="Path to the dataset dir to process", required=True
-    )
-    parser.add_argument("-s", "--start", help="Start date (YYYYMMDD)", required=True)
-    parser.add_argument("-e", "--end", help="End date (YYYYMMDD)", required=True)
+    # option that is specific to this cli tool
     parser.add_argument(
         "-E",
         "--populate-enrichment-tables",
         help="Add enrichment tables to the specified path",
-        required=False,
-    )
-    parser.add_argument(
-        "-l",
-        "--log-level",
-        default="INFO",
-        help="Logging Level: INFO, WARN, ERROR, DEBUG",
+        default="",
     )
-    args = parser.parse_args()
-
-    try:
-        logging.getLogger().setLevel(args.log_level)
-        logging.getLogger().handlers[0].setFormatter(
-            logging.Formatter("%(asctime)s %(message)s", datefmt="%m/%d/%Y %I:%M:%S %p")
-        )
-    except ValueError:
-        logging.error(f"Invalid log level: {args.log_level}")
-        sys.exit(1)
-
-    cur_dataset = args.dataset
-
-    manager = TransformerManager(current_dataset=cur_dataset)
-
-    start_date = datetime.strptime(args.start, "%Y%m%d")
-    end_date = datetime.strptime(args.end, "%Y%m%d")
-
-    process_range(manager, start_date, end_date)
+    env_config = EnvironmentConfig(parser)
+    env_config.add_start(required=False)
+    env_config.add_end(required=False)
+    env_config.add_aggregation_level(required=False)
+    env_config.add_dataset_path(required=True)
+    args = env_config.get_options(argv)
+
+    manager = TransformerManager(current_dataset=args.DATASET, agg_level=args.AGGLEVEL)
+
+    start_date, end_date = get_date_range(args.START, args.END, agg_level=args.AGGLEVEL)
+    if start_date and end_date:
+        process_range(manager, start_date, end_date)
+    else:
+        process_table(manager)
 
-    if args.populate_enrichment_tables:
-        add_enrichment_tables(manager, args.populate_enrichment_tables)
+    if args.POPULATE_ENRICHMENT_TABLES:
+        add_enrichment_tables(manager, args.POPULATE_ENRICHMENT_TABLES)
 
 
 if __name__ == "__main__":
-    main()
+    main(argv=None)
```

### Comparing `wintappy-0.1.2/wintappy/etlutils/transformer_manager.py` & `wintappy-0.1.4/wintappy/etlutils/transformer_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from dataclasses import dataclass
 from typing import Dict
 
 from jinja2 import Environment, PackageLoader
 
-from wintappy.analytics.utils import QueryAnalytic, load_all
+from wintappy.analytics.utils import CARAnalytic, load_all
 from wintappy.database.wintap_duckdb import WintapDuckDB, WintapDuckDBOptions
 from wintappy.datautils import rawutil as ru
 
 
 # Just a wrapper class to hold some of the commonly used objects in etl utils
 @dataclass
 class TransformerManager:
-    analytics: Dict[str, QueryAnalytic]
+    analytics: Dict[str, CARAnalytic]
     dataset_path: str
     jinja_environment: Environment
     wintap_duckdb: WintapDuckDB
 
-    def __init__(self, current_dataset: str):
+    def __init__(self, current_dataset: str, agg_level: str = ""):
         self.dataset_path = current_dataset
-        con = ru.init_db(self.dataset_path)
+        con = None
+        if agg_level:
+            con = ru.init_db(self.dataset_path, agg_level=agg_level)
+            path = f"{self.dataset_path}/{agg_level}"
+        else:
+            con = ru.init_db(self.dataset_path)
+            path = self.dataset_path
         ## basic setup for what we will use to run analytics
-        options = WintapDuckDBOptions(con, self.dataset_path, load_analytics=False)
+        options = WintapDuckDBOptions(con, path, load_analytics=False)
         self.wintap_duckdb = WintapDuckDB(options)
         self.jinja_environment = Environment(
             loader=PackageLoader("wintappy", package_path="./analytics/mitre_car/")
         )
         self.analytics = load_all(self.jinja_environment)
```

### Comparing `wintappy-0.1.2/wintappy/notebookutils/datasetchooser.py` & `wintappy-0.1.4/wintappy/notebookutils/datasetchooser.py`

 * *Files identical despite different names*

### Comparing `wintappy-0.1.2/wintappy.egg-info/PKG-INFO` & `wintappy-0.1.4/wintappy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: wintappy
-Version: 0.1.2
+Version: 0.1.4
 Summary: Python utilities for working with Wintap data
 Home-page: https://github.com/LLNL/Wintap-PyUtil
 Author: LLNL
 Author-email: grantj@llnl.gov
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: altair
 Requires-Dist: boto3
 Requires-Dist: duckdb
+Requires-Dist: dynaconf
 Requires-Dist: fsspec
 Requires-Dist: gitpython
 Requires-Dist: humanfriendly
 Requires-Dist: importlib_resources
 Requires-Dist: ipyfilechooser
-Requires-Dist: jinja2==3.0.3
+Requires-Dist: jinja2
 Requires-Dist: jinjasql
 Requires-Dist: lxml
 Requires-Dist: magic_duckdb
 Requires-Dist: matplotlib
 Requires-Dist: mitreattack-python
 Requires-Dist: networkx
 Requires-Dist: pandas
```

### Comparing `wintappy-0.1.2/wintappy.egg-info/SOURCES.txt` & `wintappy-0.1.4/wintappy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
+tests/test_config.py
 wintappy/__init__.py
+wintappy/config.py
 wintappy.egg-info/PKG-INFO
 wintappy.egg-info/SOURCES.txt
 wintappy.egg-info/dependency_links.txt
 wintappy.egg-info/entry_points.txt
 wintappy.egg-info/requires.txt
 wintappy.egg-info/top_level.txt
 wintappy/analytics/__init__.py
@@ -57,28 +59,38 @@
 wintappy/analytics/mitre_car/__init__.py
 wintappy/analytics/mitre_car/macros.sql
 wintappy/database/__init__.py
 wintappy/database/constants.py
 wintappy/database/wintap_database.py
 wintappy/database/wintap_duckdb.py
 wintappy/database/templates/__init__.py
-wintappy/database/templates/create_analytics.sql
 wintappy/database/templates/create_analytics_results.sql
-wintappy/database/templates/insert_analytics.sql
+wintappy/database/templates/create_sigma_results.sql
 wintappy/database/templates/insert_analytics_results.sql
 wintappy/datautils/__init__.py
 wintappy/datautils/initdb.sql
+wintappy/datautils/label_summary.sql
+wintappy/datautils/lolbas_summary.sql
+wintappy/datautils/mitre_summary.sql
+wintappy/datautils/process_path.sql
+wintappy/datautils/process_summary.sql
 wintappy/datautils/rawtostdview.sql
 wintappy/datautils/rawutil.py
+wintappy/datautils/sigma_summary.sql
 wintappy/datautils/stdview_duckdb.py
 wintappy/datautils/stdviewutil.py
+wintappy/datautils/summary_util.py
+wintappy/datautils/uber_summary.sql
 wintappy/datautils/wintapgraph.py
 wintappy/etlutils/__init__.py
 wintappy/etlutils/collectbinaries.py
-wintappy/etlutils/download_from_s3.py
+wintappy/etlutils/dbhelpers.py
+wintappy/etlutils/downloadfroms3.py
 wintappy/etlutils/rawtorolling.py
 wintappy/etlutils/rawtostdview.py
 wintappy/etlutils/run_enrichment.py
+wintappy/etlutils/runone.py
 wintappy/etlutils/transformer_manager.py
+wintappy/etlutils/ubersummary.py
 wintappy/etlutils/utils.py
 wintappy/notebookutils/__init__.py
 wintappy/notebookutils/datasetchooser.py
```

