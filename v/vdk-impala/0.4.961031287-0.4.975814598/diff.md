# Comparing `tmp/vdk-impala-0.4.961031287.tar.gz` & `tmp/vdk-impala-0.4.975814598.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-impala-0.4.961031287.tar", last modified: Wed Aug  9 16:26:02 2023, max compression
+gzip compressed data, was "vdk-impala-0.4.975814598.tar", last modified: Tue Aug 22 11:25:59 2023, max compression
```

## Comparing `vdk-impala-0.4.961031287.tar` & `vdk-impala-0.4.975814598.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.663979 vdk-impala-0.4.961031287/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6530 2023-08-09 16:26:02.663979 vdk-impala-0.4.961031287/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5936 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-09 16:26:02.663979 vdk-impala-0.4.961031287/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1223 2023-08-09 16:25:49.000000 vdk-impala-0.4.961031287/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.651979 vdk-impala-0.4.961031287/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.651979 vdk-impala-0.4.961031287/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.651979 vdk-impala-0.4.961031287/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/
--rw-rw-rw-   0 root         (0) root         (0)     7458 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4518 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)    21129 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     7846 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     7448 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_lineage_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     6850 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/data_quality_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     2703 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.655979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3373 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.659979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
--rw-rw-rw-   0 root         (0) root         (0)      309 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.659979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     3190 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.659979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.659979 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/
--rw-rw-rw-   0 root         (0) root         (0)     3032 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
--rw-rw-rw-   0 root         (0) root         (0)     4358 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
--rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/template_arguments_validator.py
--rw-rw-rw-   0 root         (0) root         (0)     2298 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.659979 vdk-impala-0.4.961031287/src/vdk_impala.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6530 2023-08-09 16:26:02.000000 vdk-impala-0.4.961031287/src/vdk_impala.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3918 2023-08-09 16:26:02.000000 vdk-impala-0.4.961031287/src/vdk_impala.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-09 16:26:02.000000 vdk-impala-0.4.961031287/src/vdk_impala.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-08-09 16:26:02.000000 vdk-impala-0.4.961031287/src/vdk_impala.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-08-09 16:26:02.000000 vdk-impala-0.4.961031287/src/vdk_impala.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-08-09 16:26:02.000000 vdk-impala-0.4.961031287/src/vdk_impala.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.659979 vdk-impala-0.4.961031287/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.651979 vdk-impala-0.4.961031287/tests/functional/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.651979 vdk-impala-0.4.961031287/tests/functional/jobs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.659979 vdk-impala-0.4.961031287/tests/functional/jobs/sql-job/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/tests/functional/jobs/sql-job/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/tests/functional/jobs/sql-job/20_populate_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.663979 vdk-impala-0.4.961031287/tests/functional/jobs/sql-job-non-lineage/
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-09 16:26:02.663979 vdk-impala-0.4.961031287/tests/functional/jobs/sql-job-syntax-error/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
--rw-rw-rw-   0 root         (0) root         (0)     3952 2023-08-09 16:25:44.000000 vdk-impala-0.4.961031287/tests/test_error_classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.755289 vdk-impala-0.4.975814598/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-08-22 11:25:59.755289 vdk-impala-0.4.975814598/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5936 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-22 11:25:59.755289 vdk-impala-0.4.975814598/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2023-08-22 11:25:48.000000 vdk-impala-0.4.975814598/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.739288 vdk-impala-0.4.975814598/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.735288 vdk-impala-0.4.975814598/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.735288 vdk-impala-0.4.975814598/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.739288 vdk-impala-0.4.975814598/src/vdk/plugin/impala/
+-rw-rw-rw-   0 root         (0) root         (0)     7458 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     4518 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    21129 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     7846 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     7448 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_lineage_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6850 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.743289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/data_quality_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.743289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.743289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.743289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     2774 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.743289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.743289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.743289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.747289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3444 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.747289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-create-consolidated-view.sql
+-rw-rw-rw-   0 root         (0) root         (0)      309 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/04-compute-stats.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.747289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3261 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.747289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-requisite-sql-scripts/02-overwrite-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.751289 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/
+-rw-rw-rw-   0 root         (0) root         (0)     3032 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/01-test-if-view-matches-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)     4358 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/03-refresh.sql
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/04-compute-stats.sql
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/template_arguments_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)     2298 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.751289 vdk-impala-0.4.975814598/src/vdk_impala.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-08-22 11:25:59.000000 vdk-impala-0.4.975814598/src/vdk_impala.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3918 2023-08-22 11:25:59.000000 vdk-impala-0.4.975814598/src/vdk_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-22 11:25:59.000000 vdk-impala-0.4.975814598/src/vdk_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-08-22 11:25:59.000000 vdk-impala-0.4.975814598/src/vdk_impala.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-08-22 11:25:59.000000 vdk-impala-0.4.975814598/src/vdk_impala.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-08-22 11:25:59.000000 vdk-impala-0.4.975814598/src/vdk_impala.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.751289 vdk-impala-0.4.975814598/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.739288 vdk-impala-0.4.975814598/tests/functional/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.739288 vdk-impala-0.4.975814598/tests/functional/jobs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.751289 vdk-impala-0.4.975814598/tests/functional/jobs/sql-job/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/tests/functional/jobs/sql-job/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/tests/functional/jobs/sql-job/20_populate_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.751289 vdk-impala-0.4.975814598/tests/functional/jobs/sql-job-non-lineage/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/tests/functional/jobs/sql-job-non-lineage/10_create_table.sql
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/tests/functional/jobs/sql-job-non-lineage/20_compute_table.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-22 11:25:59.755289 vdk-impala-0.4.975814598/tests/functional/jobs/sql-job-syntax-error/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/tests/functional/jobs/sql-job-syntax-error/10_bad_query.sql
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2023-08-22 11:25:44.000000 vdk-impala-0.4.975814598/tests/test_error_classifier.py
```

### Comparing `vdk-impala-0.4.961031287/PKG-INFO` & `vdk-impala-0.4.975814598/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.961031287
+Version: 0.4.975814598
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.961031287/README.md` & `vdk-impala-0.4.975814598/README.md`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/setup.py` & `vdk-impala-0.4.975814598/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.4.961031287"
+__version__ = "0.4.975814598"
 
 setuptools.setup(
     name="vdk-impala",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for Impala database.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_configuration.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_connection.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_error_classifier.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_error_handler.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_error_handler.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_helper.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_helper.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_lineage_plugin.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_lineage_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/impala_plugin.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/impala_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/data_quality_exception.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/data_quality_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/00-dimension-scd1-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-handle-quality-checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
             _vdk_template_insert_partition_clause=partition_clause,
             source_schema=source_schema,
             source_view=source_view,
         )
         job_input.execute_query(insert_into_staging)
 
         if check(staging_table):
+            job_input.execute_query(f"COMPUTE STATS {staging_table}")
+
             insert_into_target = insert_query.format(
                 source_schema=staging_schema,
                 source_view=staging_table_name,
                 _vdk_template_insert_partition_clause=partition_clause,
                 target_schema=target_schema,
                 target_table=target_table,
             )
```

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd1/02-requisite-sql-scripts/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/00-dimension-scd2-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/dimension/scd2/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/00-fact-snapshot-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/insert/02-handle-quality-checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
             staging_schema=staging_schema,
             staging_table_name=staging_table_name,
         )
         job_input.execute_query(create_view)
 
         view_full_name = f"{view_schema}.{view_name}"
         if check(view_full_name):
+            job_input.execute_query(f"COMPUTE STATS {staging_table}")
+
             insert_into_target = insert_query.format(
                 source_schema=staging_schema,
                 source_view=staging_table_name,
                 _vdk_template_insert_partition_clause=partition_clause,
                 target_schema=target_schema,
                 target_table=target_table,
             )
```

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/00-fact-snapshot-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/fact/snapshot/02-handle-quality-checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,16 @@
             source_schema=source_schema,
             source_view=source_view,
             last_arrival_ts=last_arrival_ts,
         )
         job_input.execute_query(insert_into_staging)
 
         if check(staging_table):
+            job_input.execute_query(f"COMPUTE STATS {staging_table}")
+
             insert_into_target = overwrite_target_query.format(
                 staging_schema=staging_schema,
                 staging_table_name=staging_table_name,
                 _vdk_template_insert_partition_clause=partition_clause,
                 target_schema=target_schema,
                 target_table=target_table,
             )
```

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/00-versioned-definition.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/load/versioned/02-insert-into-target.sql`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/template_arguments_validator.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/template_arguments_validator.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk/plugin/impala/templates/utility.py` & `vdk-impala-0.4.975814598/src/vdk/plugin/impala/templates/utility.py`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/src/vdk_impala.egg-info/PKG-INFO` & `vdk-impala-0.4.975814598/src/vdk_impala.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-impala
-Version: 0.4.961031287
+Version: 0.4.975814598
 Summary: Versatile Data Kit SDK plugin provides support for Impala database.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-impala-0.4.961031287/src/vdk_impala.egg-info/SOURCES.txt` & `vdk-impala-0.4.975814598/src/vdk_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vdk-impala-0.4.961031287/tests/test_error_classifier.py` & `vdk-impala-0.4.975814598/tests/test_error_classifier.py`

 * *Files identical despite different names*

