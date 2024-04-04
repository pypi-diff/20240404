# Comparing `tmp/encommon-0.7.2.tar.gz` & `tmp/encommon-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encommon-0.7.2.tar", last modified: Sun Mar 31 14:53:53 2024, max compression
+gzip compressed data, was "encommon-0.7.3.tar", last modified: Thu Apr  4 05:11:00 2024, max compression
```

## Comparing `encommon-0.7.2.tar` & `encommon-0.7.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.119778 encommon-0.7.2/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.7.2/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.7.2/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-03-31 14:53:53.119778 encommon-0.7.2/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2177 2024-03-31 14:52:08.000000 encommon-0.7.2/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.117778 encommon-0.7.2/encommon/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.117778 encommon-0.7.2/encommon/config/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2023-12-31 23:46:50.000000 encommon-0.7.2/encommon/config/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2041 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/config/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4853 2024-03-29 04:32:48.000000 encommon-0.7.2/encommon/config/config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2313 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/config/files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13662 2024-03-31 04:43:35.000000 encommon-0.7.2/encommon/config/logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1810 2024-03-31 06:53:30.000000 encommon-0.7.2/encommon/config/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/config/paths.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.118778 encommon-0.7.2/encommon/config/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-03-31 14:51:50.000000 encommon-0.7.2/encommon/config/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      731 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/config/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3247 2024-03-31 14:51:50.000000 encommon-0.7.2/encommon/config/test/test_config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2253 2024-03-31 14:51:50.000000 encommon-0.7.2/encommon/config/test/test_files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4740 2024-03-31 04:43:35.000000 encommon-0.7.2/encommon/config/test/test_logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2062 2024-03-31 14:51:50.000000 encommon-0.7.2/encommon/config/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      880 2024-03-29 04:32:48.000000 encommon-0.7.2/encommon/conftest.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.118778 encommon-0.7.2/encommon/crypts/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2023-12-31 23:46:50.000000 encommon-0.7.2/encommon/crypts/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3158 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/crypts/crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3145 2024-02-24 03:44:32.000000 encommon-0.7.2/encommon/crypts/hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-03-31 06:53:30.000000 encommon-0.7.2/encommon/crypts/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.118778 encommon-0.7.2/encommon/crypts/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/crypts/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-01-01 00:31:04.000000 encommon-0.7.2/encommon/crypts/test/test_crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1206 2024-02-24 03:44:32.000000 encommon-0.7.2/encommon/crypts/test/test_hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.118778 encommon-0.7.2/encommon/times/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      597 2024-02-24 04:11:08.000000 encommon-0.7.2/encommon/times/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2506 2024-03-29 10:21:00.000000 encommon-0.7.2/encommon/times/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9872 2024-03-02 07:24:59.000000 encommon-0.7.2/encommon/times/duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6411 2024-03-29 10:21:11.000000 encommon-0.7.2/encommon/times/parse.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.118778 encommon-0.7.2/encommon/times/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/times/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1477 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/times/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3901 2024-03-02 07:24:59.000000 encommon-0.7.2/encommon/times/test/test_duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4308 2024-02-24 04:11:08.000000 encommon-0.7.2/encommon/times/test/test_parse.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2314 2024-03-29 04:37:46.000000 encommon-0.7.2/encommon/times/test/test_timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2023 2024-03-31 14:51:50.000000 encommon-0.7.2/encommon/times/test/test_times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4735 2024-01-01 00:31:04.000000 encommon-0.7.2/encommon/times/test/test_window.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6312 2024-03-29 10:21:22.000000 encommon-0.7.2/encommon/times/timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9694 2024-03-31 14:51:50.000000 encommon-0.7.2/encommon/times/times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     8023 2024-03-29 10:21:32.000000 encommon-0.7.2/encommon/times/window.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.119778 encommon-0.7.2/encommon/types/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-03-29 08:35:51.000000 encommon-0.7.2/encommon/types/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2208 2024-03-27 03:36:15.000000 encommon-0.7.2/encommon/types/dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2675 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/types/empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      560 2024-03-27 03:47:38.000000 encommon-0.7.2/encommon/types/strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.119778 encommon-0.7.2/encommon/types/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/types/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2673 2024-03-27 03:36:15.000000 encommon-0.7.2/encommon/types/test/test_dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      981 2023-12-31 23:41:33.000000 encommon-0.7.2/encommon/types/test/test_empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      407 2024-03-27 03:47:38.000000 encommon-0.7.2/encommon/types/test/test_strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.119778 encommon-0.7.2/encommon/utils/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      833 2024-03-29 10:55:04.000000 encommon-0.7.2/encommon/utils/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      466 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/utils/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2462 2024-02-24 04:04:57.000000 encommon-0.7.2/encommon/utils/match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3236 2024-02-24 04:04:57.000000 encommon-0.7.2/encommon/utils/paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3169 2024-03-20 05:52:00.000000 encommon-0.7.2/encommon/utils/sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7360 2024-03-31 06:53:30.000000 encommon-0.7.2/encommon/utils/stdout.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.119778 encommon-0.7.2/encommon/utils/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2023-12-31 23:18:53.000000 encommon-0.7.2/encommon/utils/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-02-24 04:04:57.000000 encommon-0.7.2/encommon/utils/test/test_match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1892 2024-02-24 04:04:57.000000 encommon-0.7.2/encommon/utils/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1464 2024-01-01 00:31:04.000000 encommon-0.7.2/encommon/utils/test/test_sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-03-31 04:43:35.000000 encommon-0.7.2/encommon/utils/test/test_stdout.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-03-31 14:52:33.000000 encommon-0.7.2/encommon/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-03-31 14:53:53.119778 encommon-0.7.2/encommon.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-03-31 14:53:53.000000 encommon-0.7.2/encommon.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1891 2024-03-31 14:53:53.000000 encommon-0.7.2/encommon.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-03-31 14:53:53.000000 encommon-0.7.2/encommon.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-03-31 14:53:53.000000 encommon-0.7.2/encommon.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-03-31 14:53:53.000000 encommon-0.7.2/encommon.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.7.2/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.7.2/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      422 2024-03-31 14:53:53.120778 encommon-0.7.2/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.050277 encommon-0.7.3/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.7.3/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.7.3/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-04 05:11:00.050277 encommon-0.7.3/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2177 2024-03-31 14:52:08.000000 encommon-0.7.3/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.047277 encommon-0.7.3/encommon/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-02 23:01:55.000000 encommon-0.7.3/encommon/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.047277 encommon-0.7.3/encommon/config/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/config/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2041 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/config/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4743 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2313 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/config/files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13973 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1816 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/config/paths.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.048277 encommon-0.7.3/encommon/config/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-02 23:01:55.000000 encommon-0.7.3/encommon/config/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      731 2024-04-02 23:01:55.000000 encommon-0.7.3/encommon/config/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3327 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/test/test_config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2292 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/test/test_files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4740 2024-04-02 23:01:55.000000 encommon-0.7.3/encommon/config/test/test_logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2101 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/config/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      880 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/conftest.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.048277 encommon-0.7.3/encommon/crypts/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/crypts/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3500 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/crypts/crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3103 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/crypts/hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-04 05:02:38.000000 encommon-0.7.3/encommon/crypts/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.048277 encommon-0.7.3/encommon/crypts/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/crypts/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/crypts/test/test_crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1206 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/crypts/test/test_hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.7.3/encommon/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.048277 encommon-0.7.3/encommon/times/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      597 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2506 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9854 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6411 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/parse.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/times/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1477 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3901 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4308 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_parse.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2314 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2023 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4735 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/times/test/test_window.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6287 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9688 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-04 05:08:51.000000 encommon-0.7.3/encommon/times/window.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/types/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2208 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2675 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      560 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/types/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2673 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/test/test_dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      981 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/test/test_empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      407 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/types/test/test_strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/utils/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      833 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      466 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2462 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3236 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3169 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7360 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/stdout.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.049276 encommon-0.7.3/encommon/utils/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/test_match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1892 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1464 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/test_sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-02 23:01:56.000000 encommon-0.7.3/encommon/utils/test/test_stdout.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-04 05:09:53.000000 encommon-0.7.3/encommon/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-04 05:11:00.050277 encommon-0.7.3/encommon.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1891 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-04 05:11:00.000000 encommon-0.7.3/encommon.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.7.3/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.7.3/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      422 2024-04-04 05:11:00.050277 encommon-0.7.3/setup.cfg
```

### Comparing `encommon-0.7.2/LICENSE` & `encommon-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/PKG-INFO` & `encommon-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.7.2
+Version: 0.7.3
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `encommon-0.7.2/README.md` & `encommon-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/__init__.py` & `encommon-0.7.3/encommon/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/config/__init__.py` & `encommon-0.7.3/encommon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/config/common.py` & `encommon-0.7.3/encommon/config/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/config/config.py` & `encommon-0.7.3/encommon/config/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,43 +86,43 @@
 
 
     @property
     def files(
         self,
     ) -> ConfigFiles:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__files
 
 
     @property
     def paths(
         self,
     ) -> ConfigPaths:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__paths
 
 
     @property
     def cargs(
         self,
     ) -> dict[str, Any]:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__cargs
 
 
     @property
     def config(
@@ -138,17 +138,17 @@
 
 
     @property
     def model(
         self,
     ) -> Callable:  # type: ignore
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__model
 
 
     @property
     def params(
@@ -187,18 +187,16 @@
 
         if self.__logger is not None:
             return self.__logger
 
         enlogger = (
             self.params.enlogger)
 
-        assert enlogger is not None
-
-        self.__logger = Logger(
-            **enlogger.model_dump())
+        self.__logger = (
+            Logger(params=enlogger))
 
         return self.__logger
 
 
     @property
     def crypts(
         self,
@@ -209,13 +207,11 @@
 
         if self.__crypts is not None:
             return self.__crypts
 
         encrypts = (
             self.params.encrypts)
 
-        assert encrypts is not None
-
-        self.__crypts = Crypts(
-            **encrypts.model_dump())
+        self.__crypts = (
+            Crypts(params=encrypts))
 
         return self.__crypts
```

### Comparing `encommon-0.7.2/encommon/config/files.py` & `encommon-0.7.3/encommon/config/files.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/config/logger.py` & `encommon-0.7.3/encommon/config/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,26 @@
 from logging import StreamHandler
 from logging import WARNING
 from logging import getLogger
 from pathlib import Path
 from typing import Any
 from typing import Literal
 from typing import Optional
+from typing import TYPE_CHECKING
 
 from .common import LOGLEVELS
 from .common import config_path
 from ..times.common import PARSABLE
 from ..times.times import Times
 from ..types.empty import Empty
 from ..utils.stdout import kvpair_ansi
 
+if TYPE_CHECKING:
+    from .params import LoggerParams
+
 
 
 LOGGER_FILE = 'encommon.logger.file'
 LOGGER_STDO = 'encommon.logger.stdo'
 
 LOGSEVERS = {
     'critical': int(CRITICAL),
@@ -139,43 +143,43 @@
 
 
     @property
     def level(
         self,
     ) -> LOGLEVELS:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__level
 
 
     @property
     def time(
         self,
     ) -> Times:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return Times(self.__time)
 
 
     @property
     def fields(
         self,
     ) -> dict[str, str]:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return dict(self.__fields)
 
 
     @property
     def stdo_output(
@@ -279,17 +283,18 @@
 
     Example
     -------
     >>> logger = Logger(stdo_level='info')
     >>> logger.start()
     >>> logger.log_i(message='testing')
 
-    :param stdo_level: Minimum log message severity level.
-    :param file_level: Minimum log message severity level.
+    :param stdo_level: Minimum level for the message to pass.
+    :param file_level: Minimum level for the message to pass.
     :param file_path: Enables writing to the filesystem path.
+    :param params: Parameters for instantiating the instance.
     """
 
     __stdo_level: Optional[LOGLEVELS]
     __file_level: Optional[LOGLEVELS]
     __file_path: Optional[Path]
 
     __started: bool
@@ -300,19 +305,25 @@
 
     def __init__(
         self,
         *,
         stdo_level: Optional[LOGLEVELS] = None,
         file_level: Optional[LOGLEVELS] = None,
         file_path: Optional[str | Path] = None,
+        params: Optional['LoggerParams'] = None,
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
+        if params is not None:
+            stdo_level = params.stdo_level
+            file_level = params.file_level
+            file_path = params.file_path
+
         if file_path is not None:
             file_path = config_path(file_path)
 
         self.__stdo_level = stdo_level
         self.__file_level = file_level
         self.__file_path = file_path
 
@@ -323,82 +334,82 @@
 
 
     @property
     def stdo_level(
         self,
     ) -> Optional[LOGLEVELS]:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__stdo_level
 
 
     @property
     def file_level(
         self,
     ) -> Optional[LOGLEVELS]:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__file_level
 
 
     @property
     def file_path(
         self,
     ) -> Optional[Path]:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__file_path
 
 
     @property
     def started(
         self,
     ) -> bool:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__started
 
 
     @property
     def logger_stdo(
         self,
     ) -> _Logger:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__logger_stdo
 
 
     @property
     def logger_file(
         self,
     ) -> _Logger:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__logger_file
 
 
     def start(
         self,
```

### Comparing `encommon-0.7.2/encommon/config/params.py` & `encommon-0.7.3/encommon/config/params.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 
 
 class LoggerParams(BaseModel, extra='forbid'):
     """
     Process and validate the common configuration parameters.
 
-    :param stdo_level: Minimum log message severity level.
-    :param file_level: Minimum log message severity level.
+    :param stdo_level: Minimum level for the message to pass.
+    :param file_level: Minimum level for the message to pass.
     :param file_path: Enables writing to the filesystem path.
     :param data: Keyword arguments passed to Pydantic model.
         Parameter is picked up by autodoc, please ignore.
     """
 
     stdo_level: Optional[LOGLEVELS] = None
     file_level: Optional[LOGLEVELS] = None
```

### Comparing `encommon-0.7.2/encommon/config/paths.py` & `encommon-0.7.3/encommon/config/paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/config/test/test_common.py` & `encommon-0.7.3/encommon/config/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/config/test/test_config.py` & `encommon-0.7.3/encommon/config/test/test_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,16 +84,20 @@
 
 
     _config1 = config.config
     _config2 = config.config
 
     assert _config1 is not _config2
 
+
+    sample_path = Path(
+        f'{SAMPLES}/config.json')
+
     sample = load_sample(
-        path=SAMPLES.joinpath('config.json'),
+        path=sample_path,
         update=ENPYRWS,
         content=_config1,
         replace={
             'config_path': str(config_path)})
 
     expect = prep_sample(
         content=_config2,
@@ -104,16 +108,20 @@
 
 
     _params1 = config.params
     _params2 = config.params
 
     assert _params1 is _params2
 
+
+    sample_path = Path(
+        f'{SAMPLES}/params.json')
+
     sample = load_sample(
-        path=SAMPLES.joinpath('params.json'),
+        path=sample_path,
         update=ENPYRWS,
         content=_params1.model_dump(),
         replace={
             'config_path': str(config_path)})
 
     expect = prep_sample(
         content=_params2.model_dump(),
```

### Comparing `encommon-0.7.2/encommon/config/test/test_files.py` & `encommon-0.7.3/encommon/config/test/test_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -83,16 +83,19 @@
 
 
     _merged1 = files.merged
     _merged2 = files.merged
 
     assert _merged1 is not _merged2
 
+    sample_path = Path(
+        f'{SAMPLES}/files.json')
+
     sample = load_sample(
-        path=SAMPLES.joinpath('files.json'),
+        path=sample_path,
         update=ENPYRWS,
         content=_merged1,
         replace={
             'config_path': str(config_path)})
 
     expect = prep_sample(
         content=_merged2,
```

### Comparing `encommon-0.7.2/encommon/config/test/test_logger.py` & `encommon-0.7.3/encommon/config/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/config/test/test_paths.py` & `encommon-0.7.3/encommon/config/test/test_paths.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,19 @@
 
 
     _merged1 = paths.merged
     _merged2 = paths.merged
 
     assert _merged1 is not _merged2
 
+    sample_path = Path(
+        f'{SAMPLES}/paths.json')
+
     sample = load_sample(
-        path=SAMPLES.joinpath('paths.json'),
+        path=sample_path,
         update=ENPYRWS,
         content=_merged1,
         replace={
             'config_path': str(config_path)})
 
     expect = prep_sample(
         content=_merged2,
```

### Comparing `encommon-0.7.2/encommon/conftest.py` & `encommon-0.7.3/encommon/conftest.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/crypts/crypts.py` & `encommon-0.7.3/encommon/crypts/crypts.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,22 @@
 """
 
 
 
 from re import compile
 from re import match as re_match
 from re import sub as re_sub
+from typing import Optional
+from typing import TYPE_CHECKING
 
 from cryptography.fernet import Fernet
 
+if TYPE_CHECKING:
+    from .params import CryptsParams
+
 
 
 ENCRYPT = compile(
     r'^\$ENCRYPT;1\.\d;\S+\;.+?$')
 
 
 
@@ -29,41 +34,48 @@
     >>> phrase = Crypts.keygen()
     >>> crypts = Crypts({'default': phrase})
     >>> encrypt = crypts.encrypt('example')
     >>> crypts.decrypt(encrypt)
     'example'
 
     :param phrases: Passphrases that are used in operations.
+    :param params: Parameters for instantiating the instance.
     """
 
     __phrases: dict[str, str]
 
 
     def __init__(
         self,
-        phrases: dict[str, str],
+        phrases: Optional[dict[str, str]] = None,
+        params: Optional['CryptsParams'] = None,
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
+        phrases = phrases or {}
+
+        if params is not None:
+            phrases |= params.phrases
+
         if 'default' not in phrases:
             raise ValueError('default')
 
         self.__phrases = dict(phrases)
 
 
     @property
     def phrases(
         self,
     ) -> dict[str, str]:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return dict(self.__phrases)
 
 
     def encrypt(
         self,
```

### Comparing `encommon-0.7.2/encommon/crypts/params.py` & `encommon-0.7.3/encommon/crypts/params.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/crypts/test/test_crypts.py` & `encommon-0.7.3/encommon/crypts/test/test_crypts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/crypts/test/test_hashes.py` & `encommon-0.7.3/encommon/crypts/test/test_hashes.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/__init__.py` & `encommon-0.7.3/encommon/times/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/common.py` & `encommon-0.7.3/encommon/times/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/duration.py` & `encommon-0.7.3/encommon/times/duration.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,43 +274,43 @@
 
 
     @property
     def source(
         self,
     ) -> float:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__source
 
 
     @property
     def smart(
         self,
     ) -> bool:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__smart
 
 
     @property
     def groups(
         self,
     ) -> int:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__groups
 
 
     def units(
         self,
```

### Comparing `encommon-0.7.2/encommon/times/parse.py` & `encommon-0.7.3/encommon/times/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     Example
     -------
     >>> parse_time(0)
     datetime.datetime(1970, 1, 1, 0...
 
     :param source: Time in various forms that will be parsed.
     :param anchor: Optional relative time; for snap notation.
-    :param format: Optional format for the timestamp string.
+    :param format: Optional format when source is timestamp.
     :param tzname: Name of the timezone associated to source.
         This is not relevant in timezone included in source.
     :returns: Python datetime object containing related time.
     """
 
     if (source is not None
             and hasattr(source, 'source')):
```

### Comparing `encommon-0.7.2/encommon/times/test/test_common.py` & `encommon-0.7.3/encommon/times/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/test/test_duration.py` & `encommon-0.7.3/encommon/times/test/test_duration.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/test/test_parse.py` & `encommon-0.7.3/encommon/times/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/test/test_timers.py` & `encommon-0.7.3/encommon/times/test/test_timers.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/test/test_times.py` & `encommon-0.7.3/encommon/times/test/test_times.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/test/test_window.py` & `encommon-0.7.3/encommon/times/test/test_window.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/times/timers.py` & `encommon-0.7.3/encommon/times/timers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .common import PARSABLE
 from .times import Times
 
 if TYPE_CHECKING:
     from sqlite3 import Connection
 
 
+
 TABLE = (
     """
     create table
      if not exists
      {0} (
       "unique" text not null,
       "update" text not null,
@@ -155,56 +156,56 @@
 
 
     @property
     def timers(
         self,
     ) -> dict[str, float]:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return dict(self.__timers)
 
 
     @property
     def cache_file(
         self,
     ) -> 'Connection':
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__cache_file
 
 
     @property
     def cache_dict(
         self,
     ) -> dict[str, Times]:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return dict(self.__cache_dict)
 
 
     @property
     def cache_name(
         self,
     ) -> str:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__cache_name
 
 
     def ready(
         self,
@@ -227,15 +228,15 @@
 
         if unique not in caches:
             raise ValueError('unique')
 
         cache = caches[unique]
         timer = timers[unique]
 
-        ready = cache.elapsed >= timer
+        ready = cache.since >= timer
 
         if ready and update:
             self.update(unique)
 
         return ready
 
 
@@ -274,14 +275,14 @@
         :param minimum: Determines minimum seconds that must pass.
         :param started: Determines when the time starts for timer.
         """
 
         timers = self.__timers
         caches = self.__cache_dict
 
-        if unique in caches:
+        if unique in timers:
             raise ValueError('unique')
 
         timers[unique] = float(minimum)
         caches[unique] = Times(started)
 
         self.save_cache()
```

### Comparing `encommon-0.7.2/encommon/times/times.py` & `encommon-0.7.3/encommon/times/times.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Example
     -------
     >>> Times('1/1/2000 12:00am')
     Times('2000-01-01T00:00:00.000000+0000')
 
     :param source: Time in various forms that will be parsed.
     :param anchor: Optional relative time; for snap notation.
-    :param format: Optional format for the timestamp string.
+    :param format: Optional format when source is timestamp.
     :param tzname: Name of the timezone associated to source.
         This is not relevant in timezone included in source.
     """
 
     __source: datetime
 
 
@@ -256,17 +256,17 @@
 
 
     @property
     def source(
         self,
     ) -> datetime:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__source
 
 
     @property
     def epoch(
@@ -399,15 +399,15 @@
         self,
         format: str = STAMP_SUBSEC,
         tzname: Optional[str] = None,
     ) -> str:
         """
         Return the timestamp using provided format for instance.
 
-        :param format: Optional format for the timestamp string.
+        :param format: Optional format when source is timestamp.
         :param tzname: Name of the timezone associated to source.
             This is not relevant in timezone included in source.
         :returns: Timestamp using provided format for instance.
         """
 
         parsed = self.__source
```

### Comparing `encommon-0.7.2/encommon/times/window.py` & `encommon-0.7.3/encommon/times/window.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,108 +105,108 @@
 
 
     @property
     def schedule(
         self,
     ) -> SCHEDULE:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return copy(self.__schedule)
 
 
     @property
     def start(
         self,
     ) -> Times:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return Times(self.__start)
 
 
     @property
     def stop(
         self,
     ) -> Times:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return Times(self.__stop)
 
 
     @property
     def anchor(
         self,
     ) -> Times:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return Times(self.__anchor)
 
 
     @property
     def delay(
         self,
     ) -> float:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__delay
 
 
     @property
     def next(
         self,
     ) -> Times:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return Times(self.__winext)
 
 
     @property
     def last(
         self,
     ) -> Times:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return Times(self.__wilast)
 
 
     @property
     def walked(
         self,
     ) -> bool:
         """
-        Return the property for attribute from the class instance.
+        Return the value for the attribute from class instance.
 
-        :returns: Property for attribute from the class instance.
+        :returns: Value for the attribute from class instance.
         """
 
         return self.__walked
 
 
     def __wifunc(
         self,
```

### Comparing `encommon-0.7.2/encommon/types/dicts.py` & `encommon-0.7.3/encommon/types/dicts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/types/empty.py` & `encommon-0.7.3/encommon/types/empty.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/types/strings.py` & `encommon-0.7.3/encommon/types/strings.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/types/test/test_dicts.py` & `encommon-0.7.3/encommon/types/test/test_dicts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/types/test/test_empty.py` & `encommon-0.7.3/encommon/types/test/test_empty.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/__init__.py` & `encommon-0.7.3/encommon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/match.py` & `encommon-0.7.3/encommon/utils/match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/paths.py` & `encommon-0.7.3/encommon/utils/paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/sample.py` & `encommon-0.7.3/encommon/utils/sample.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/stdout.py` & `encommon-0.7.3/encommon/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/test/test_match.py` & `encommon-0.7.3/encommon/utils/test/test_match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/test/test_paths.py` & `encommon-0.7.3/encommon/utils/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/test/test_sample.py` & `encommon-0.7.3/encommon/utils/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon/utils/test/test_stdout.py` & `encommon-0.7.3/encommon/utils/test/test_stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/encommon.egg-info/PKG-INFO` & `encommon-0.7.3/encommon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.7.2
+Version: 0.7.3
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `encommon-0.7.2/encommon.egg-info/SOURCES.txt` & `encommon-0.7.3/encommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `encommon-0.7.2/pyproject.toml` & `encommon-0.7.3/pyproject.toml`

 * *Files identical despite different names*

