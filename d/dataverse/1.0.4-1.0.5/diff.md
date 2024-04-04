# Comparing `tmp/dataverse-1.0.4.tar.gz` & `tmp/dataverse-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-1.0.4.tar", last modified: Mon Mar 18 10:44:31 2024, max compression
+gzip compressed data, was "dataverse-1.0.5.tar", last modified: Thu Apr  4 08:18:45 2024, max compression
```

## Comparing `dataverse-1.0.4.tar` & `dataverse-1.0.5.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:31.497462 dataverse-1.0.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-06 12:20:27.000000 dataverse-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      718 2024-03-18 10:44:31.496869 dataverse-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10728 2024-03-18 10:20:08.000000 dataverse-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:25.745747 dataverse-1.0.4/dataverse/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:26.105872 dataverse-1.0.4/dataverse/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      413 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/api/cli.py
--rw-r--r--   0 root         (0) root         (0)     1350 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/api/emr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:26.117383 dataverse-1.0.4/dataverse/config/
--rw-r--r--   0 root         (0) root         (0)       30 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6923 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/config/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:26.172635 dataverse-1.0.4/dataverse/etl/
--rw-r--r--   0 root         (0) root         (0)      133 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:26.189380 dataverse-1.0.4/dataverse/etl/__sample/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/__sample/__init__.py
--rw-r--r--   0 root         (0) root         (0)      374 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/__sample/ducky.py
--rw-r--r--   0 root         (0) root         (0)     1437 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/__sample/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:26.195527 dataverse-1.0.4/dataverse/etl/bias/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/bias/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.196626 dataverse-1.0.4/dataverse/etl/cleaning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3759 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/char.py
--rw-r--r--   0 root         (0) root         (0)     2656 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/document.py
--rw-r--r--   0 root         (0) root         (0)     2421 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/html.py
--rw-r--r--   0 root         (0) root         (0)     9955 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/korean.py
--rw-r--r--   0 root         (0) root         (0)     2998 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/length.py
--rw-r--r--   0 root         (0) root         (0)     1816 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/number.py
--rw-r--r--   0 root         (0) root         (0)     2318 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/table.py
--rw-r--r--   0 root         (0) root         (0)     3415 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/cleaning/unicode.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.367770 dataverse-1.0.4/dataverse/etl/data_ingestion/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5615 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/arrow.py
--rw-r--r--   0 root         (0) root         (0)    15117 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/common_crawl.py
--rw-r--r--   0 root         (0) root         (0)     1051 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/csv.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/cultura_x.py
--rw-r--r--   0 root         (0) root         (0)     1590 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/huggingface.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/parquet.py
--rw-r--r--   0 root         (0) root         (0)     3535 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/red_pajama.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/slim_pajama.py
--rw-r--r--   0 root         (0) root         (0)     1506 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_ingestion/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.442544 dataverse-1.0.4/dataverse/etl/data_load/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_load/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_load/aws.py
--rw-r--r--   0 root         (0) root         (0)     2525 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_load/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/data_load/parquet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.502037 dataverse-1.0.4/dataverse/etl/decontamination/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/decontamination/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.761284 dataverse-1.0.4/dataverse/etl/deduplication/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/deduplication/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2586 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/deduplication/common_crawl.py
--rw-r--r--   0 root         (0) root         (0)      903 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/deduplication/exact.py
--rw-r--r--   0 root         (0) root         (0)    14139 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/deduplication/minhash.py
--rw-r--r--   0 root         (0) root         (0)     5331 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/deduplication/polyglot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.827286 dataverse-1.0.4/dataverse/etl/pii/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/pii/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3099 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/pii/card.py
--rw-r--r--   0 root         (0) root         (0)     3392 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/pii/nin.py
--rw-r--r--   0 root         (0) root         (0)    16553 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.862731 dataverse-1.0.4/dataverse/etl/quality/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/quality/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6078 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/quality/language.py
--rw-r--r--   0 root         (0) root         (0)    14568 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.870546 dataverse-1.0.4/dataverse/etl/toxicity/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/toxicity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:28.944282 dataverse-1.0.4/dataverse/etl/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      890 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/utils/log.py
--rw-r--r--   0 root         (0) root         (0)     1375 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/utils/sampling.py
--rw-r--r--   0 root         (0) root         (0)     2185 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/etl/utils/statistics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:29.041168 dataverse-1.0.4/dataverse/lab/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/lab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:29.161536 dataverse-1.0.4/dataverse/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:31.088341 dataverse-1.0.4/dataverse/utils/analyze/
--rw-r--r--   0 root         (0) root         (0)       86 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/analyze/__init__.py
--rw-r--r--   0 root         (0) root         (0)      296 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/analyze/pip.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/analyze/python.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:31.248007 dataverse-1.0.4/dataverse/utils/api/
--rw-r--r--   0 root         (0) root         (0)     1603 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68144 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/api/aws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:31.377376 dataverse-1.0.4/dataverse/utils/format/
--rw-r--r--   0 root         (0) root         (0)      151 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/format/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3319 2024-03-18 10:23:11.000000 dataverse-1.0.4/dataverse/utils/format/huggingface.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/format/ufl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:31.493025 dataverse-1.0.4/dataverse/utils/setting/
--rw-r--r--   0 root         (0) root         (0)      110 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/setting/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7283 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/setting/system.py
--rw-r--r--   0 root         (0) root         (0)     6019 2024-03-06 12:20:27.000000 dataverse-1.0.4/dataverse/utils/setting/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 10:44:26.038237 dataverse-1.0.4/dataverse.egg-info/
--rw-r--r--   0 root         (0) root         (0)      718 2024-03-18 10:44:21.000000 dataverse-1.0.4/dataverse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2402 2024-03-18 10:44:21.000000 dataverse-1.0.4/dataverse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 10:44:21.000000 dataverse-1.0.4/dataverse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-03-18 10:44:21.000000 dataverse-1.0.4/dataverse.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      182 2024-03-18 10:44:21.000000 dataverse-1.0.4/dataverse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-18 10:44:21.000000 dataverse-1.0.4/dataverse.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-18 10:44:31.500789 dataverse-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1275 2024-03-18 10:44:02.000000 dataverse-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.697984 dataverse-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-03-06 12:20:27.000000 dataverse-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-04 08:18:45.696857 dataverse-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11134 2024-04-04 06:53:09.000000 dataverse-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.432025 dataverse-1.0.5/dataverse/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.466034 dataverse-1.0.5/dataverse/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      413 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/api/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/api/emr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.470287 dataverse-1.0.5/dataverse/config/
+-rw-r--r--   0 root         (0) root         (0)       30 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8299 2024-04-01 01:17:56.000000 dataverse-1.0.5/dataverse/config/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.485024 dataverse-1.0.5/dataverse/etl/
+-rw-r--r--   0 root         (0) root         (0)      133 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.496772 dataverse-1.0.5/dataverse/etl/__sample/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/__sample/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      374 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/__sample/ducky.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/__sample/github.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.501024 dataverse-1.0.5/dataverse/etl/bias/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/bias/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.534032 dataverse-1.0.5/dataverse/etl/cleaning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/char.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/document.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/html.py
+-rw-r--r--   0 root         (0) root         (0)     9955 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/korean.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/length.py
+-rw-r--r--   0 root         (0) root         (0)     1816 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/number.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/table.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/cleaning/unicode.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.567253 dataverse-1.0.5/dataverse/etl/data_ingestion/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5615 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/arrow.py
+-rw-r--r--   0 root         (0) root         (0)    15117 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/common_crawl.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/csv.py
+-rw-r--r--   0 root         (0) root         (0)      991 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/cultura_x.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/parquet.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/red_pajama.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/slim_pajama.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/data_ingestion/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.582255 dataverse-1.0.5/dataverse/etl/data_save/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 01:17:56.000000 dataverse-1.0.5/dataverse/etl/data_save/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      139 2024-04-01 01:17:56.000000 dataverse-1.0.5/dataverse/etl/data_save/aws.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-04-01 01:17:56.000000 dataverse-1.0.5/dataverse/etl/data_save/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-04-01 01:17:56.000000 dataverse-1.0.5/dataverse/etl/data_save/parquet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.590032 dataverse-1.0.5/dataverse/etl/decontamination/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/decontamination/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.609255 dataverse-1.0.5/dataverse/etl/deduplication/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/deduplication/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/deduplication/common_crawl.py
+-rw-r--r--   0 root         (0) root         (0)      903 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/deduplication/exact.py
+-rw-r--r--   0 root         (0) root         (0)    14139 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/deduplication/minhash.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/deduplication/polyglot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.620504 dataverse-1.0.5/dataverse/etl/pii/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/pii/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/pii/card.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/pii/nin.py
+-rw-r--r--   0 root         (0) root         (0)    15812 2024-04-01 01:17:56.000000 dataverse-1.0.5/dataverse/etl/pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.625031 dataverse-1.0.5/dataverse/etl/quality/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/quality/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6078 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/quality/language.py
+-rw-r--r--   0 root         (0) root         (0)    14324 2024-04-01 01:17:56.000000 dataverse-1.0.5/dataverse/etl/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.633506 dataverse-1.0.5/dataverse/etl/toxicity/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/toxicity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.644531 dataverse-1.0.5/dataverse/etl/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      890 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/utils/sampling.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/etl/utils/statistics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.652531 dataverse-1.0.5/dataverse/lab/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/lab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.656031 dataverse-1.0.5/dataverse/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.667781 dataverse-1.0.5/dataverse/utils/analyze/
+-rw-r--r--   0 root         (0) root         (0)       86 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/analyze/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      296 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/analyze/pip.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/analyze/python.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.672030 dataverse-1.0.5/dataverse/utils/api/
+-rw-r--r--   0 root         (0) root         (0)     1603 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68144 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/api/aws.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.688280 dataverse-1.0.5/dataverse/utils/format/
+-rw-r--r--   0 root         (0) root         (0)      151 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/format/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3319 2024-04-01 01:17:56.000000 dataverse-1.0.5/dataverse/utils/format/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/format/ufl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.700031 dataverse-1.0.5/dataverse/utils/setting/
+-rw-r--r--   0 root         (0) root         (0)      110 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/setting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7283 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/setting/system.py
+-rw-r--r--   0 root         (0) root         (0)     6019 2024-03-06 12:20:27.000000 dataverse-1.0.5/dataverse/utils/setting/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 08:18:45.451034 dataverse-1.0.5/dataverse.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-04 08:18:45.000000 dataverse-1.0.5/dataverse.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2402 2024-04-04 08:18:45.000000 dataverse-1.0.5/dataverse.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 08:18:45.000000 dataverse-1.0.5/dataverse.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-04 08:18:45.000000 dataverse-1.0.5/dataverse.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      182 2024-04-04 08:18:45.000000 dataverse-1.0.5/dataverse.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 08:18:45.000000 dataverse-1.0.5/dataverse.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 08:18:45.700782 dataverse-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-04-04 08:18:08.000000 dataverse-1.0.5/setup.py
```

### Comparing `dataverse-1.0.4/LICENSE` & `dataverse-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/PKG-INFO` & `dataverse-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse
-Version: 1.0.4
+Version: 1.0.5
 Summary: An open-source simplifies ETL workflow with Python based on Spark
 Author: Dataverse Team
 Author-email: dataverse@upstage.ai
 License: Apache License 2.0
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
```

### Comparing `dataverse-1.0.4/README.md` & `dataverse-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,18 @@
   <source media="(prefers-color-scheme: light)" srcset="docs/images/dataverse_logo-color.png" width=300>
   <img alt="DATAVERSE" src="docs/images/dataverse_logo-color.png" width=300>
 </picture>
 
 <br>
 
 The Universe of Data. 
-All about Data, Data Science, and Data Engineering.
+All about Data, Data Science, and Data Engineering. </br>
+Upstage Solar is powered by Dataverse! Try at Upstage [Console](https://console.upstage.ai/)!
 
-[Docs](https://data-verse.gitbook.io/docs/) • [Examples](https://github.com/UpstageAI/dataverse/tree/main/examples) • [API Reference](https://data-verse.readthedocs.io/en/latest/) • [FAQ](https://data-verse.gitbook.io/docs/documents/faqs) • [Contribution Guide](https://github.com/UpstageAI/dataverse/blob/main/contribution/CONTRIBUTING.md)  • [Contact](mailto:dataverse@upstage.ai)  • [Discord](https://discord.gg/aAqF7pyq4h)
+[Docs](https://data-verse.gitbook.io/docs/) • [Examples](https://github.com/UpstageAI/dataverse/tree/main/examples) • [API Reference](https://data-verse.readthedocs.io/en/latest/) • [FAQ](https://data-verse.gitbook.io/docs/documents/faqs) • [Contribution Guide](https://github.com/UpstageAI/dataverse/blob/main/contribution/CONTRIBUTING.md)  • [Contact](mailto:dataverse@upstage.ai)  • [Discord](https://discord.gg/aAqF7pyq4h) • [Paper](https://arxiv.org/abs/2403.19340)
 <br><br>
 <div align="left">
 
 ## Welcome to Dataverse!
 Dataverse is a freely-accessible open-source project that supports your **ETL(Extract, Transform and Load) pipeline with Python**. We offer a simple, standardized and user-friendly solution for data processing and management, catering to the needs of data scientists, analysts, and developers in LLM era. Even though you don't know much about Spark, you can use it easily via _dataverse_.
 
 ### With Dataverse, you are empowered to
@@ -24,15 +25,15 @@
 - utilize a range of preprocessing functions without the need to install multiple libraries.
 - create high-quality data for analysis and training of Large Language Models (LLM).
 - leverage Spark with ease, regardless of your expertise level.
 - facilitate smoother collaboration among users with varying degress of Spark proficiency.
 - enjoy freedom from the limitations of local environments by harnessing the capabilities of AWS EMR.
 
 ### Architecture of Dataverse
-![Architecture of Dataverse](./docs/images/dataverse_system_architecture.jpg)
+![Architecture of Dataverse](./docs/images/dataverse_system_architecture_white.jpeg)
 
 ### Key Features of Dataverse
 - **Block-Based**: In Dataverse, a `block` means a `registered ETL function` which is running on Spark. You can build Spark code like putting together puzzle pieces. You can easily add, take away, or re-arrange pieces to get the results you want via configure.
 - **Configure-Based**: All the setups for Spark and steps of block can be defined with configure. You don't need to know all the code. Just set up the options, and you're good to go.
 - **Extensible**: It's designed to meet your specific demands, allowing for custom features that fit perfectly with your project.
 
 If you want to know more about Dataverse, please checkout our [docs](https://data-verse.gitbook.io/docs/).
@@ -78,15 +79,15 @@
         This will reduce the dataset to 1.29k rows. 
     </ul>
     <ul>
         <li style="line-height:250%;"> <b>deduplication___minhash___lsh_jaccard </b></li>
         Deduplicate by <code>question</code> column, 5-gram minhash jaccard similarity threshold of 0.1.
     </ul>
     <ul>
-        <li style="line-height:250%;"> <b>data_load___parquet___ufl2parquet </b></li>
+        <li style="line-height:250%;"> <b>data_save___parquet___ufl2parquet </b></li>
         Save the processed dataset as a Parquet file to <code>./guideline/etl/sample/quickstart.parquet</code>.<br/>
         The final dataset comprises around 1.14k rows.
     </ul>
 </details>
 
 ```python
 # 1. Set your ETL process as config.
@@ -115,15 +116,15 @@
           'name': 'deduplication___minhash___lsh_jaccard', 
           'args': {'threshold': 0.1,
                   'ngram_size': 5,
                   'subset': 'question'}
         },
         {
           # Load; Save the data
-          'name': 'data_load___parquet___ufl2parquet',
+          'name': 'data_save___parquet___ufl2parquet',
           'args': {'save_path': './guideline/etl/sample/quickstart.parquet'}
         }
       ]
   })
 ```
 Above code block is an example of an ETL process in Dataverse. In Dataverse, the available registered ETL functions are referred to as `blocks`, and this example is comprised of four blocks. You can freely combine these blocks using config to create the ETL processes for your needs. The list of available functions and args of them can be found in the [API Reference](https://data-verse.readthedocs.io/en/latest/). Each functions 'args' should be added in dictionary format.
 
@@ -152,20 +153,20 @@
 | Transform | bias            | (WIP) Reduce skewed or prejudiced data, particularly data that reinforce stereotypes.             |
 |           | cleaning        | Remove irrelevant, redundant, or noisy information, such as stop words or special characters.     |
 |           | decontamination | (WIP) Remove contaminated data including benchmark.                                               |
 |           | deduplication   | Remove duplicated data, targeting not only identical matches but also similar data.               |
 |           | pii             | PII stands for Personally Identifiable Information. Removing sensitive information from data.     |
 |           | quality         | Improving the data quality, in the perspective of accuracy, consistency, and reliability of data. |
 |           | toxicity        | (WIP) Removing harmful, offensive, or inappropriate content within the data.                      |
-| Load      | data_load       | Saving the processed data to a preferred source like data lake, database, etc.                    |
+| Load      | data_save       | Saving the processed data to a preferred source like data lake, database, etc.                    |
 | Utils     | utils           | Essential tools for data processing, including sampling, logging, statistics, etc.                |
 <br>
 
 ## 🌌 Dataverse supports AWS
-Dataverse supports AWS! Step by step guide to setting up is [here](https://data-verse.gitbook.io/docs/lets-start/aws-s3-support).
+Dataverse works with AWS S3 and EMR, enabling you to load and save data on S3 and execute ETL pipelines through EMR. Step by step guide to setting up is [here](https://data-verse.gitbook.io/docs/lets-start/aws-s3-support).
 </br>
 
 ## 🌌 Dataverse use-case
 > If you have any use-cases of your own, please feel free to let us know. </br>We would love to hear about them and possibly feature your case.
 
 
 *✨* [`Upstage`](https://www.upstage.ai/) is using Dataverse for preprocessing the data for the training of [Solar Mini](https://console.upstage.ai/services/solar?utm_source=upstage.ai&utm_medium=referral&utm_campaign=Main+hero+Solar+card&utm_term=Try+API+for+Free&utm_content=home). </br>
@@ -183,18 +184,19 @@
 Dataverse is an open-source project orchestrated by the **Data-Centric LLM Team** at [`Upstage`](https://www.upstage.ai/), designed as an data ecosystem for LLM(Large Language Model). Launched in March 2024, this initiative stands at the forefront of advancing data handling in the realm of LLM.
 
 ## 🌌 License
 Dataverse is completely freely-accessible open-source and licensed under the Apache-2.0 license.
 
 
 ## 🌌 Citation
-> If you want to cite our 🌌 Dataverse project, feel free to use the following bibtex
+If you want to cite our 🌌 Dataverse project, feel free to use the following bibtex. You can check our paper via [link](https://arxiv.org/abs/2403.19340).
 
 ```bibtex
-@misc{dataverse,
-  title = {Dataverse},
-  author = {Hyunbyung Park, Sukyung Lee, Gyoungjin Gim, Yungi Kim, Dahyun Kim, Chanjun Park},
-  year = {2024},
-  publisher = {GitHub, Upstage AI},
-  howpublished = {\url{https://github.com/UpstageAI/dataverse}},
+@misc{park2024dataverse,
+      title={Dataverse: Open-Source ETL (Extract, Transform, Load) Pipeline for Large Language Models}, 
+      author={Hyunbyung Park and Sukyung Lee and Gyoungjin Gim and Yungi Kim and Dahyun Kim and Chanjun Park},
+      year={2024},
+      eprint={2403.19340},
+      archivePrefix={arXiv},
+      primaryClass={cs.CL}
 }
 ```
```

### Comparing `dataverse-1.0.4/dataverse/api/emr.py` & `dataverse-1.0.5/dataverse/api/emr.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/config/interface.py` & `dataverse-1.0.5/dataverse/config/interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,31 +19,42 @@
 from pathlib import Path
 
 
 
 class Config:
     """
     Interface to check & load the configurations
-    lightweight wrapper for OmegaConf
+    
+    This class provides a lightweight wrapper for OmegaConf and allows checking and loading configurations.
+    It supports loading configurations from various sources such as files, AWS S3, and config strings.
+    The class also provides methods for saving configurations and setting default values for missing config arguments.
     """
     def __new__(cls, *args, **kwargs):
         raise NotImplementedError("Config is not allowed to be instantiated")
 
     @classmethod
     def load(cls, config: Union[str, dict, DictConfig, OmegaConf, Path]):
         """
-        config (Union[str, dict, OmegaConf]): config for the etl
-            - str or Path: (this could has several cases)
-                - path to the config file
-                - s3 path to the config file
-                - config string
-                    - this is like when you load `yaml` file with open()
-                        config = yaml.load(f)
-            - dict: config dict
-            - OmegaConf: config object
+        Load the configuration for the etl.
+
+        Args:
+            config (Union[str, dict, OmegaConf]): The configuration for the etl.
+                - str or Path: This could have several cases:
+                    - Path to the config file.
+                    - S3 path to the config file.
+                    - Config string. This is similar to loading a `yaml` file with `open()`.
+                - dict: Config dictionary.
+                - OmegaConf: Config object.
+
+        Returns:
+            The loaded configuration.
+
+        Raises:
+            ValueError: If the provided config is not a valid path or S3 path.
+            TypeError: If the provided config is not of type str, dict, or OmegaConf.
         """
         if isinstance(config, (str, Path)):
             if isinstance(config, Path):
                 config = str(config)
 
             # Local File
             if Path(config).is_file():
@@ -53,59 +64,75 @@
             elif config.startswith(('s3://', 's3a://', 's3n://')):
                 aws_s3_matched = re.match(r's3[a,n]?://([^/]+)/(.*)', config)
                 if aws_s3_matched:
                     bucket, key = aws_s3_matched.groups()
                     config_content = aws_s3_read(bucket, key)
                     config = OmegaConf.create(config_content)
                 else:
-                    # assume it's a config string that starts with s3
+                    # Assume it's a config string that starts with s3
                     config_str = config
                     config = OmegaConf.create(config_str)
 
-                    # check if it's config string or not
-                    # in case of config string it should create a config object
-                    # if not, it will create {'config': None}
+                    # Check if it's a config string or not
+                    # In case of a config string, it should create a config object
+                    # If not, it will create {'config': None}
                     if config_str in config and config[config_str] is None:
                         raise ValueError(f"config {config_str} is not a valid s3 path")
             
             # String Config
             else:
-                # assume it's a config string
+                # Assume it's a config string
                 config_str = config
                 config = OmegaConf.create(config_str)
 
-                # same as above, check if it's config string or not
+                # Same as above, check if it's a config string or not
                 if config_str in config and config[config_str] is None:
                     raise ValueError(f"config {config_str} is not a valid path")
 
         elif isinstance(config, dict):
             config = OmegaConf.create(config)
         elif isinstance(config, (OmegaConf, DictConfig)):
             pass
         else:
             raise TypeError(f"config should be str, dict, or OmegaConf but got {type(config)}")
 
         return config
 
     @classmethod
     def save(cls, config, path: Union[str, Path]):
+        """
+        Saves the configuration to a specified path.
+
+        Args:
+            config: The configuration to be saved.
+            path (Union[str, Path]): The path where the configuration should be saved.
+
+        Raises:
+            ValueError: If the provided path is not a valid S3 path.
+        """
         if path.startswith(('s3://', 's3a://', 's3n://')):
             aws_s3_matched = re.match(r's3[a,n]?://([^/]+)/(.*)', path)
             if aws_s3_matched:
                 bucket, key = aws_s3_matched.groups()
                 aws_s3_write(bucket, key, config)
             else:
                 raise ValueError(f"config path {path} is not a valid s3 path")
         else:
             OmegaConf.save(config, Path(path))
 
     @classmethod
     def default(cls, emr: bool = False):
         """
-        fill the missing config with default
+        Fill the missing config with default values.
+
+        Args:
+            emr (bool, optional): Flag indicating whether the config is for EMR. Defaults to False.
+
+        Returns:
+            dict: Default configuration dictionary.
         """
         local_dir = f"{SystemSetting().CACHE_DIR}/.cache/dataverse/tmp"
 
         default = OmegaConf.create({
             'spark': {
                 'master': 'local[10]',
                 'appname': 'default',
@@ -195,10 +222,18 @@
             })
 
         return default
 
     @classmethod
     def set_default(cls, config: OmegaConf, emr: bool = False):
         """
-        set the missing config args with default
+        Sets the missing config arguments with default values.
+
+        Args:
+            config (OmegaConf): The configuration object to merge with default values.
+            emr (bool, optional): Whether to use EMR configuration. Defaults to False.
+
+        Returns:
+            OmegaConf: The merged configuration object.
+
         """
         return OmegaConf.merge(cls.default(emr=emr), config)
```

### Comparing `dataverse-1.0.4/dataverse/etl/__sample/github.py` & `dataverse-1.0.5/dataverse/etl/__sample/github.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/cleaning/char.py` & `dataverse-1.0.5/dataverse/etl/cleaning/char.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/cleaning/document.py` & `dataverse-1.0.5/dataverse/etl/cleaning/document.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/cleaning/html.py` & `dataverse-1.0.5/dataverse/etl/cleaning/html.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/cleaning/korean.py` & `dataverse-1.0.5/dataverse/etl/cleaning/korean.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/cleaning/length.py` & `dataverse-1.0.5/dataverse/etl/cleaning/length.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/cleaning/number.py` & `dataverse-1.0.5/dataverse/etl/cleaning/number.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/cleaning/table.py` & `dataverse-1.0.5/dataverse/etl/cleaning/table.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/cleaning/unicode.py` & `dataverse-1.0.5/dataverse/etl/cleaning/unicode.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/arrow.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/arrow.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/common_crawl.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/common_crawl.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/csv.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/csv.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/cultura_x.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/cultura_x.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/huggingface.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/huggingface.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/parquet.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/parquet.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/red_pajama.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/red_pajama.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/slim_pajama.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/slim_pajama.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_ingestion/test.py` & `dataverse-1.0.5/dataverse/etl/data_ingestion/test.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/data_load/huggingface.py` & `dataverse-1.0.5/dataverse/etl/data_save/huggingface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Data loading to Huggingface Datasets
+Data saving to Huggingface Datasets
 
 Huggingface support spark natively!
 https://huggingface.co/docs/datasets/use_with_spark
 
 Copyright (c) 2024-present Upstage Co., Ltd.
 Apache-2.0 license
 """
@@ -15,24 +15,24 @@
 from pyspark.rdd import RDD
 from pyspark.sql import DataFrame
 
 from dataverse.etl import register_etl
 
 
 @register_etl
-def data_load___huggingface___ufl2hf_hub(spark, ufl, hub_path, repartition=1, *args, **kwargs):
+def data_save___huggingface___ufl2hf_hub(spark, ufl, hub_path, repartition=1, *args, **kwargs):
     """
     TODO: Save data to Hugging Face dataset and upload to hub.
     """
     NotImplementedError()
     return None
 
 
 @register_etl
-def data_load___huggingface___ufl2hf(
+def data_save___huggingface___ufl2hf(
     spark, ufl: Union[RDD, DataFrame], save_path: str, repartition: int = 1, *args, **kwargs
 ) -> str:
     """
     Save data to HuggingFace dataset and return the path.
 
     Args:
         spark(sparkSession): The Spark session.
@@ -60,15 +60,15 @@
     hf_dataset = Dataset.from_spark(ufl)
     hf_dataset.save_to_disk(save_path)
 
     return save_path
 
 
 @register_etl
-def data_load___huggingface___ufl2hf_obj(
+def data_save___huggingface___ufl2hf_obj(
     spark, ufl: Union[RDD, DataFrame], repartition: int = 1, *args, **kwargs
 ) -> Dataset:
     """
     Convert data to HuggingFace dataset object.
 
     Args:
         spark(sparkSession): The Spark session.
```

### Comparing `dataverse-1.0.4/dataverse/etl/data_load/parquet.py` & `dataverse-1.0.5/dataverse/etl/data_save/parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Data loading to Parquets
+Data saving to Parquets
 
 Copyright (c) 2024-present Upstage Co., Ltd.
 Apache-2.0 license
 """
 
 import os
 from typing import Union
@@ -11,15 +11,15 @@
 from pyspark.rdd import RDD
 from pyspark.sql import DataFrame
 
 from dataverse.etl import register_etl
 
 
 @register_etl
-def data_load___parquet___ufl2parquet(
+def data_save___parquet___ufl2parquet(
     spark,
     ufl: Union[RDD, DataFrame],
     save_path: str,
     repartition: int = 1,
     *args,
     **kwargs,
 ) -> str:
```

### Comparing `dataverse-1.0.4/dataverse/etl/deduplication/common_crawl.py` & `dataverse-1.0.5/dataverse/etl/deduplication/common_crawl.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/deduplication/exact.py` & `dataverse-1.0.5/dataverse/etl/deduplication/exact.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/deduplication/minhash.py` & `dataverse-1.0.5/dataverse/etl/deduplication/minhash.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/deduplication/polyglot.py` & `dataverse-1.0.5/dataverse/etl/deduplication/polyglot.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/pii/card.py` & `dataverse-1.0.5/dataverse/etl/pii/card.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/pii/nin.py` & `dataverse-1.0.5/dataverse/etl/pii/nin.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/pipeline.py` & `dataverse-1.0.5/dataverse/etl/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,14 @@
 
     This class represents an ETL (Extract, Transform, Load) pipeline.
     It provides methods for managing and executing ETL processes.
 
     Attributes:
         registry (ETLRegistry): The registry of ETL processes.
 
-    Methods:
-        __len__(): Returns the number of ETL processes in the registry.
-        status(): Prints the status of the registry.
-        search(category=None, sub_category=None): Searches the registry for ETL processes matching the specified
-            category and sub-category.
-        get(key): Retrieves an ETL class from the registry.
-        setup_spark_conf(config, verbose=False): Sets up the Spark configuration based on the provided config.
-        sample(n=100, config=None, sample_etl="data_ingestion___test___generate_fake_ufl", verbose=False):
-            Generates a sample dataset using the specified ETL process and Spark session.
-        run(config, verbose=False, cache=False, emr=False, *args, **kwargs): Runs the ETL process based on the
-            provided config.
-
     Examples:
         >>> etl_pipeline = ETLPipeline()
         >>> etl_pipeline.status()
         >>> etl_pipeline.search('data_ingestion', 'ufl')
         >>> spark, data = etl_pipeline.sample()
 
         >>> config = Config.default()
@@ -92,22 +80,25 @@
             category (str, optional): The category to filter the search results. Defaults to None.
             sub_category (str, optional): The sub-category to filter the search results. Defaults to None.
 
         Returns:
             list: A list of search results matching the specified category and sub-category.
 
         Examples:
-            # Return every ETL
-            >>> etl_pipeline.search()
-
-            # Only selected category
+            Return every ETL
+            
+            >>> etl_pipeline.search() 
+            
+            Only selected category
+            
             >>> etl_pipeline.search('data_ingestion')
             >>> etl_pipeline.search(category='data_ingestion')
-
-            # Only selected category & sub_category
+            
+            Only selected category & sub_category
+            
             >>> etl_pipeline.search('data_ingestion', 'ufl')
             >>> etl_pipeline.search(category='data_ingestion', sub_category='ufl')
         """
         return self.registry.search(category=category, sub_category=sub_category)
 
     def get(self, key):
         """get ETL class from registry"""
@@ -278,15 +269,15 @@
             print("[ Spark Final Configuration ]")
             print(OmegaConf.to_yaml(spark_conf.getAll()))
             print("=" * 50)
 
         # ================= [ Run ETL ] ====================
         # [ Load RDD/DataFrame ] - data ingestion
         # [ Preprocessing ]
-        # [ Save RDD/DataFrame ] - data load
+        # [ Save RDD/DataFrame ] - data save
         etl_configs = config.etl
         total_etl_n = len(etl_configs)
 
         # [switch] is the ETL process ended or not
         # if not, spark session & data will be returned to continue
         IS_ETL_FINISHED = True
 
@@ -300,25 +291,25 @@
             etl_category = etl_name.split("___")[0]
             etl_class = self.get(key=etl_name)
 
             # instantiate etl class
             etl_instance = etl_class()
 
             # this is middle creator mode
-            # if the last ETL process is not data load
-            if etl_i == total_etl_n - 1 and etl_category != "data_load":
+            # if the last ETL process is not data save
+            if etl_i == total_etl_n - 1 and etl_category != "data_save":
                 if verbose:
                     print(
                         (
                             f"{'=' * 50}\n"
                             "[ DEBUG MODE ]\n"
                             f"{'=' * 50}\n"
                             f"Last ETL process was assigned for [ {etl_category} ]\n"
                             "Spark session will not be stopped and will be returned\n"
-                            "If this is not intended, please assign [ data_load ] at the end.\n"
+                            "If this is not intended, please assign [ data_save ] at the end.\n"
                             f"{'=' * 50}\n"
                             "Example:\n"
                             "=> spark, data = etl_pipeline.run(config)\n"
                             "=> data = data.map(add awesome duck to column)\n"
                             f"{'=' * 50}\n"
                         )
                     )
```

### Comparing `dataverse-1.0.4/dataverse/etl/quality/language.py` & `dataverse-1.0.5/dataverse/etl/quality/language.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/registry.py` & `dataverse-1.0.5/dataverse/etl/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "decontamination",
     "deduplication",
     "bias",
     "toxicity",
     "cleaning",
     "pii",
     "quality",
-    "data_load",
+    "data_save",
     "utils",
 ]
 
 IGNORE_FILES = [
     "__init__.py",
 ]
 
@@ -86,21 +86,16 @@
 
     Methods:
         __new__(): Creates a new instance of the class if it doesn't exist.
         __init__(): Initializes the class and registers the ETL classes.
         __len__(): Returns the number of registered ETL classes.
         __repr__(): Returns a string representation of the registry.
         __str__(): Returns a string representation of the registry.
-        reset(): Resets the registry.
-        register(key, etl): Registers an ETL class with a given key.
         _update_status(key): Updates the status of the registry.
-        search(category, sub_category): Searches for ETL classes based on category and sub-category.
         _convert_to_report_format(status, print_sub_category, print_etl_name): Converts the status to a report format.
-        get(key): Retrieves an ETL class based on the key.
-        get_all(): Retrieves all the registered ETL classes.
     """
 
     _initialized = False
 
     def __new__(cls):
         if not hasattr(cls, "instance"):
             cls.instance = super(ETLRegistry, cls).__new__(cls)
@@ -143,18 +138,19 @@
 
         Raises:
             ValueError: If the key is not all lowercase, not separated by '___', or does not have 2 layers of category.
             TypeError: If the ETL class is not a subclass of ETLStructure.
             KeyError: If the key is already registered.
 
         Note:
-            The key should be in the format of:
-            - all lowercase
-            - separated by ___
-            - it should have 2 layers of category
+            - The key should be in the format of:
+                - all lowercase
+                - separated by ___
+                - it should have 2 layers of category
+            
             - Example: <etl_type>___<file_key>___<etl_key> or <category>___<sub_category>___<etl_key>.
         """
         if not key.islower():
             raise ValueError(f"The key [ {key} ] should be all lowercase")
         if "___" not in key:
             raise ValueError(f"The key [ {key} ] should be separated by ___")
         if len(key.split("___")) != 3:
@@ -293,18 +289,19 @@
             ETLStructure: The ETLStructure associated with the given key.
 
         Raises:
             ValueError: If the key is not all lowercase, not separated by '___', or does not have 2 layers of category.
             KeyError: If the key is not registered in the registry.
 
         Note:
-             The key should be in the format of:
-            - all lowercase
-            - separated by ___
-            - it should have 2 layers of category
+            - The key should be in the format of:
+                - all lowercase
+                - separated by ___
+                - it should have 2 layers of category
+            
             - Example: <etl_type>___<file_key>___<etl_key> or <category>___<sub_category>___<etl_key>.
         """
         if not key.islower():
             raise ValueError(f"The key [ {key} ] should be all lowercase")
         if "___" not in key:
             raise ValueError(f"The key [ {key} ] should be separated by ___")
         if len(key.split("___")) != 3:
@@ -314,14 +311,17 @@
             raise KeyError(f"The key {key} is not registered")
 
         return self._registry[key]
 
     def get_all(self):
         """
         get all the etls
+        
+        Returns:
+            list: list of all registered etls
         """
         return list(self._registry.values())
 
 
 class ETLAutoRegistry(abc.ABCMeta, type):
     def __new__(cls, name, bases, attrs):
         """
@@ -349,23 +349,20 @@
 class BaseETL(ETLStructure, metaclass=ETLAutoRegistry):
     """
     Base class for spark ETL.
 
     This class provides a base structure for implementing spark ETL processes.
     If you need to use `self` directly, inherit this class.
 
-    Attributes:
-        None
-
     Methods:
-        run(data: Union[RDD, DataFrame], *args, **kwargs):
+        run(self, data, *args, **kwargs):
             Run the preprocessing logic.
             This method should be implemented by subclasses.
 
-        __call__(*args, **kwargs):
+        __call__(self, *args, **kwargs):
             Call the `run` method to perform the preprocessing.
     """
 
     @abc.abstractmethod
     def run(self, data: Union[RDD, DataFrame], *args, **kwargs):
         """
         run the preprocessing
```

### Comparing `dataverse-1.0.4/dataverse/etl/utils/log.py` & `dataverse-1.0.5/dataverse/etl/utils/log.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/utils/sampling.py` & `dataverse-1.0.5/dataverse/etl/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/etl/utils/statistics.py` & `dataverse-1.0.5/dataverse/etl/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/utils/analyze/python.py` & `dataverse-1.0.5/dataverse/utils/analyze/python.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/utils/api/__init__.py` & `dataverse-1.0.5/dataverse/utils/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/utils/api/aws.py` & `dataverse-1.0.5/dataverse/utils/api/aws.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/utils/format/huggingface.py` & `dataverse-1.0.5/dataverse/utils/format/huggingface.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/utils/setting/system.py` & `dataverse-1.0.5/dataverse/utils/setting/system.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse/utils/setting/user.py` & `dataverse-1.0.5/dataverse/utils/setting/user.py`

 * *Files identical despite different names*

### Comparing `dataverse-1.0.4/dataverse.egg-info/PKG-INFO` & `dataverse-1.0.5/dataverse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse
-Version: 1.0.4
+Version: 1.0.5
 Summary: An open-source simplifies ETL workflow with Python based on Spark
 Author: Dataverse Team
 Author-email: dataverse@upstage.ai
 License: Apache License 2.0
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: numpy
```

### Comparing `dataverse-1.0.4/dataverse.egg-info/SOURCES.txt` & `dataverse-1.0.5/dataverse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 dataverse/etl/data_ingestion/csv.py
 dataverse/etl/data_ingestion/cultura_x.py
 dataverse/etl/data_ingestion/huggingface.py
 dataverse/etl/data_ingestion/parquet.py
 dataverse/etl/data_ingestion/red_pajama.py
 dataverse/etl/data_ingestion/slim_pajama.py
 dataverse/etl/data_ingestion/test.py
-dataverse/etl/data_load/__init__.py
-dataverse/etl/data_load/aws.py
-dataverse/etl/data_load/huggingface.py
-dataverse/etl/data_load/parquet.py
+dataverse/etl/data_save/__init__.py
+dataverse/etl/data_save/aws.py
+dataverse/etl/data_save/huggingface.py
+dataverse/etl/data_save/parquet.py
 dataverse/etl/decontamination/__init__.py
 dataverse/etl/deduplication/__init__.py
 dataverse/etl/deduplication/common_crawl.py
 dataverse/etl/deduplication/exact.py
 dataverse/etl/deduplication/minhash.py
 dataverse/etl/deduplication/polyglot.py
 dataverse/etl/pii/__init__.py
```

### Comparing `dataverse-1.0.4/setup.py` & `dataverse-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     extras_require.update({"all": [i[0] for i in extras_require.values()]})
     return extras_require
 
 
 setup(
     name="dataverse",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     author="Dataverse Team",
     author_email="dataverse@upstage.ai",
     description="An open-source simplifies ETL workflow with Python based on Spark",
     license="Apache License 2.0",
     include_package_data=True,
     install_requires=get_requirements(),
```

