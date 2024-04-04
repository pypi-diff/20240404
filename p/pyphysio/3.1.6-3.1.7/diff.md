# Comparing `tmp/pyphysio-3.1.6.tar.gz` & `tmp/pyphysio-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphysio-3.1.6.tar", last modified: Wed Sep 27 08:34:54 2023, max compression
+gzip compressed data, was "pyphysio-3.1.7.tar", last modified: Thu Apr  4 09:46:57 2024, max compression
```

## Comparing `pyphysio-3.1.6.tar` & `pyphysio-3.1.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.433244 pyphysio-3.1.6/
--rwx------   0 bizzego   (1002) bizzego   (1002)    35142 2019-02-28 14:12:28.000000 pyphysio-3.1.6/LICENSE
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)      879 2023-09-27 08:34:54.433244 pyphysio-3.1.6/PKG-INFO
--rwx------   0 bizzego   (1002) bizzego   (1002)      730 2023-03-24 15:13:33.000000 pyphysio-3.1.6/README.md
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.137243 pyphysio-3.1.6/pyphysio/
--rwx------   0 bizzego   (1002) bizzego   (1002)     1468 2023-03-27 13:38:27.000000 pyphysio-3.1.6/pyphysio/__init__.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    15550 2023-06-06 12:20:24.000000 pyphysio-3.1.6/pyphysio/_base_algorithm.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    18955 2023-07-20 14:01:36.000000 pyphysio-3.1.6/pyphysio/artefacts.py
--rwxrwxr-x   0 bizzego   (1002) bizzego   (1002)    23474 2023-06-06 12:20:24.000000 pyphysio-3.1.6/pyphysio/filters.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.137243 pyphysio-3.1.6/pyphysio/generators/
--rwx------   0 bizzego   (1002) bizzego   (1002)     3714 2023-03-24 10:35:17.000000 pyphysio-3.1.6/pyphysio/generators/__init__.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.181244 pyphysio-3.1.6/pyphysio/indicators/
--rwx------   0 bizzego   (1002) bizzego   (1002)      374 2023-04-05 14:15:39.000000 pyphysio-3.1.6/pyphysio/indicators/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     2676 2023-03-24 10:35:17.000000 pyphysio-3.1.6/pyphysio/indicators/frequencydomain.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    11155 2023-04-05 14:15:40.000000 pyphysio-3.1.6/pyphysio/indicators/nonlinear.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    13092 2023-06-22 09:53:20.000000 pyphysio-3.1.6/pyphysio/indicators/peaks.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     6892 2023-04-05 14:15:40.000000 pyphysio-3.1.6/pyphysio/indicators/timedomain.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     9328 2023-09-21 10:02:51.000000 pyphysio-3.1.6/pyphysio/interactive.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.201243 pyphysio-3.1.6/pyphysio/loaders/
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)      146 2023-07-10 08:17:19.000000 pyphysio-3.1.6/pyphysio/loaders/__init__.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    19203 2023-07-10 08:16:45.000000 pyphysio-3.1.6/pyphysio/loaders/_load_nirs.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    18669 2023-06-22 08:20:18.000000 pyphysio-3.1.6/pyphysio/segmenters.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    23569 2023-09-21 10:00:06.000000 pyphysio-3.1.6/pyphysio/signal.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.077243 pyphysio-3.1.6/pyphysio/specialized/
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.201243 pyphysio-3.1.6/pyphysio/specialized/activity/
--rwx------   0 bizzego   (1002) bizzego   (1002)      632 2023-03-24 10:35:17.000000 pyphysio-3.1.6/pyphysio/specialized/activity/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.229244 pyphysio-3.1.6/pyphysio/specialized/eda/
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8888 2023-06-19 10:19:09.000000 pyphysio-3.1.6/pyphysio/specialized/eda/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1026 2023-03-27 13:38:27.000000 pyphysio-3.1.6/pyphysio/specialized/eda/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.249244 pyphysio-3.1.6/pyphysio/specialized/eeg/
--rwx------   0 bizzego   (1002) bizzego   (1002)      768 2023-03-24 10:35:17.000000 pyphysio-3.1.6/pyphysio/specialized/eeg/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.249244 pyphysio-3.1.6/pyphysio/specialized/emg/
--rwx------   0 bizzego   (1002) bizzego   (1002)      628 2023-03-24 10:35:17.000000 pyphysio-3.1.6/pyphysio/specialized/emg/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.265244 pyphysio-3.1.6/pyphysio/specialized/fnirs/
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    12983 2023-07-24 13:29:08.000000 pyphysio-3.1.6/pyphysio/specialized/fnirs/__init__.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    10632 2023-09-13 08:41:47.000000 pyphysio-3.1.6/pyphysio/specialized/fnirs/_convert.py
--rwx------   0 bizzego   (1002) bizzego   (1002)    24210 2023-03-24 10:35:17.000000 pyphysio-3.1.6/pyphysio/specialized/fnirs/_data.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     2718 2023-03-24 10:35:17.000000 pyphysio-3.1.6/pyphysio/specialized/fnirs/_dl_sqi.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.265244 pyphysio-3.1.6/pyphysio/specialized/heart/
--rwx------   0 bizzego   (1002) bizzego   (1002)    27246 2023-09-20 14:17:14.000000 pyphysio-3.1.6/pyphysio/specialized/heart/__init__.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1957 2023-04-05 14:15:40.000000 pyphysio-3.1.6/pyphysio/specialized/heart/_presets.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.269244 pyphysio-3.1.6/pyphysio/specialized/resp/
--rwx------   0 bizzego   (1002) bizzego   (1002)      630 2023-03-24 10:35:18.000000 pyphysio-3.1.6/pyphysio/specialized/resp/_presets.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     6272 2023-03-24 10:35:18.000000 pyphysio-3.1.6/pyphysio/sqi.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.289244 pyphysio-3.1.6/pyphysio/test_data/
--rwx------   0 bizzego   (1002) bizzego   (1002)       64 2023-03-27 13:38:27.000000 pyphysio-3.1.6/pyphysio/test_data/info_medical
--rwx------   0 bizzego   (1002) bizzego   (1002)  1097515 2023-03-27 13:38:27.000000 pyphysio-3.1.6/pyphysio/test_data/medical.txt.bz2
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    34358 2023-06-22 08:07:50.000000 pyphysio-3.1.6/pyphysio/utils.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.137243 pyphysio-3.1.6/pyphysio.egg-info/
--rwx------   0 bizzego   (1002) bizzego   (1002)      879 2023-09-27 08:34:53.000000 pyphysio-3.1.6/pyphysio.egg-info/PKG-INFO
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     1355 2023-09-27 08:34:54.000000 pyphysio-3.1.6/pyphysio.egg-info/SOURCES.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)        1 2023-09-27 08:34:53.000000 pyphysio-3.1.6/pyphysio.egg-info/dependency_links.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)       65 2023-09-27 08:34:53.000000 pyphysio-3.1.6/pyphysio.egg-info/requires.txt
--rwx------   0 bizzego   (1002) bizzego   (1002)        9 2023-09-27 08:34:53.000000 pyphysio-3.1.6/pyphysio.egg-info/top_level.txt
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)       38 2023-09-27 08:34:54.433244 pyphysio-3.1.6/setup.cfg
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     2311 2023-09-27 08:34:37.000000 pyphysio-3.1.6/setup.py
-drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2023-09-27 08:34:54.421244 pyphysio-3.1.6/tests/
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8726 2023-06-06 14:17:39.000000 pyphysio-3.1.6/tests/test_eda_methods.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1201 2023-03-27 13:38:27.000000 pyphysio-3.1.6/tests/test_filters.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     1587 2023-06-22 12:35:51.000000 pyphysio-3.1.6/tests/test_fnirs.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      547 2023-03-27 13:38:27.000000 pyphysio-3.1.6/tests/test_get_sampling_freq.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      600 2023-04-19 07:37:36.000000 pyphysio-3.1.6/tests/test_ibi_estimators.py
--rwx------   0 bizzego   (1002) bizzego   (1002)     1016 2023-03-24 10:35:18.000000 pyphysio-3.1.6/tests/test_segmenters.py
--rwx------   0 bizzego   (1002) bizzego   (1002)      959 2023-03-27 13:38:27.000000 pyphysio-3.1.6/tests/test_signal.py
--rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     4554 2023-06-22 08:09:42.000000 pyphysio-3.1.6/tests/test_tools.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.413048 pyphysio-3.1.7/
+-rwx------   0 bizzego   (1002) bizzego   (1002)    35142 2019-02-28 14:12:28.000000 pyphysio-3.1.7/LICENSE
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)      879 2024-04-04 09:46:57.413048 pyphysio-3.1.7/PKG-INFO
+-rwx------   0 bizzego   (1002) bizzego   (1002)      730 2023-03-24 15:13:33.000000 pyphysio-3.1.7/README.md
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.165042 pyphysio-3.1.7/pyphysio/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1468 2024-03-05 08:52:37.000000 pyphysio-3.1.7/pyphysio/__init__.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    15550 2023-06-06 12:20:24.000000 pyphysio-3.1.7/pyphysio/_base_algorithm.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    18882 2023-11-09 15:51:26.000000 pyphysio-3.1.7/pyphysio/artefacts.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    24555 2023-12-18 10:44:49.000000 pyphysio-3.1.7/pyphysio/filters.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.169042 pyphysio-3.1.7/pyphysio/generators/
+-rwx------   0 bizzego   (1002) bizzego   (1002)     3714 2023-03-24 10:35:17.000000 pyphysio-3.1.7/pyphysio/generators/__init__.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.193043 pyphysio-3.1.7/pyphysio/indicators/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      374 2023-04-05 14:15:39.000000 pyphysio-3.1.7/pyphysio/indicators/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2676 2023-03-24 10:35:17.000000 pyphysio-3.1.7/pyphysio/indicators/frequencydomain.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    11155 2023-04-05 14:15:40.000000 pyphysio-3.1.7/pyphysio/indicators/nonlinear.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    13092 2023-06-22 09:53:20.000000 pyphysio-3.1.7/pyphysio/indicators/peaks.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     6892 2023-04-05 14:15:40.000000 pyphysio-3.1.7/pyphysio/indicators/timedomain.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     9372 2023-10-19 12:54:30.000000 pyphysio-3.1.7/pyphysio/interactive.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.213043 pyphysio-3.1.7/pyphysio/loaders/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     1644 2024-03-19 13:05:45.000000 pyphysio-3.1.7/pyphysio/loaders/__init__.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    19202 2024-02-06 11:12:58.000000 pyphysio-3.1.7/pyphysio/loaders/_load_nirs.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    18786 2024-02-15 13:50:39.000000 pyphysio-3.1.7/pyphysio/segmenters.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    23569 2023-09-21 10:00:06.000000 pyphysio-3.1.7/pyphysio/signal.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.129042 pyphysio-3.1.7/pyphysio/specialized/
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.213043 pyphysio-3.1.7/pyphysio/specialized/activity/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      632 2023-03-24 10:35:17.000000 pyphysio-3.1.7/pyphysio/specialized/activity/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.225044 pyphysio-3.1.7/pyphysio/specialized/eda/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8888 2023-06-19 10:19:09.000000 pyphysio-3.1.7/pyphysio/specialized/eda/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1026 2023-03-27 13:38:27.000000 pyphysio-3.1.7/pyphysio/specialized/eda/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.233044 pyphysio-3.1.7/pyphysio/specialized/eeg/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      768 2023-03-24 10:35:17.000000 pyphysio-3.1.7/pyphysio/specialized/eeg/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.241044 pyphysio-3.1.7/pyphysio/specialized/emg/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      628 2023-03-24 10:35:17.000000 pyphysio-3.1.7/pyphysio/specialized/emg/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.277045 pyphysio-3.1.7/pyphysio/specialized/fnirs/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    12983 2023-07-24 13:29:08.000000 pyphysio-3.1.7/pyphysio/specialized/fnirs/__init__.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    10632 2024-02-06 10:09:10.000000 pyphysio-3.1.7/pyphysio/specialized/fnirs/_convert.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)    24210 2023-03-24 10:35:17.000000 pyphysio-3.1.7/pyphysio/specialized/fnirs/_data.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     2718 2023-03-24 10:35:17.000000 pyphysio-3.1.7/pyphysio/specialized/fnirs/_dl_sqi.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.277045 pyphysio-3.1.7/pyphysio/specialized/heart/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    27543 2023-10-20 08:05:22.000000 pyphysio-3.1.7/pyphysio/specialized/heart/__init__.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1957 2023-04-05 14:15:40.000000 pyphysio-3.1.7/pyphysio/specialized/heart/_presets.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.277045 pyphysio-3.1.7/pyphysio/specialized/resp/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      630 2023-03-24 10:35:18.000000 pyphysio-3.1.7/pyphysio/specialized/resp/_presets.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     6272 2023-03-24 10:35:18.000000 pyphysio-3.1.7/pyphysio/sqi.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.297045 pyphysio-3.1.7/pyphysio/test_data/
+-rwx------   0 bizzego   (1002) bizzego   (1002)       64 2023-03-27 13:38:27.000000 pyphysio-3.1.7/pyphysio/test_data/info_medical
+-rwx------   0 bizzego   (1002) bizzego   (1002)  1097515 2023-03-27 13:38:27.000000 pyphysio-3.1.7/pyphysio/test_data/medical.txt.bz2
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)    34478 2023-10-17 08:33:46.000000 pyphysio-3.1.7/pyphysio/utils.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.165042 pyphysio-3.1.7/pyphysio.egg-info/
+-rwx------   0 bizzego   (1002) bizzego   (1002)      879 2024-04-04 09:46:57.000000 pyphysio-3.1.7/pyphysio.egg-info/PKG-INFO
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     1355 2024-04-04 09:46:57.000000 pyphysio-3.1.7/pyphysio.egg-info/SOURCES.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)        1 2024-04-04 09:46:57.000000 pyphysio-3.1.7/pyphysio.egg-info/dependency_links.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)       65 2024-04-04 09:46:57.000000 pyphysio-3.1.7/pyphysio.egg-info/requires.txt
+-rwx------   0 bizzego   (1002) bizzego   (1002)        9 2024-04-04 09:46:57.000000 pyphysio-3.1.7/pyphysio.egg-info/top_level.txt
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)       38 2024-04-04 09:46:57.413048 pyphysio-3.1.7/setup.cfg
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     2311 2024-04-04 09:44:19.000000 pyphysio-3.1.7/setup.py
+drwxrwxr-x   0 bizzego   (1002) bizzego   (1002)        0 2024-04-04 09:46:57.397048 pyphysio-3.1.7/tests/
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     8726 2023-06-06 14:17:39.000000 pyphysio-3.1.7/tests/test_eda_methods.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1201 2023-03-27 13:38:27.000000 pyphysio-3.1.7/tests/test_filters.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     1587 2023-06-22 12:35:51.000000 pyphysio-3.1.7/tests/test_fnirs.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      547 2023-03-27 13:38:27.000000 pyphysio-3.1.7/tests/test_get_sampling_freq.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      600 2023-04-19 07:37:36.000000 pyphysio-3.1.7/tests/test_ibi_estimators.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)     1016 2023-03-24 10:35:18.000000 pyphysio-3.1.7/tests/test_segmenters.py
+-rwx------   0 bizzego   (1002) bizzego   (1002)      959 2023-03-27 13:38:27.000000 pyphysio-3.1.7/tests/test_signal.py
+-rw-rw-r--   0 bizzego   (1002) bizzego   (1002)     4554 2023-06-22 08:09:42.000000 pyphysio-3.1.7/tests/test_tools.py
```

### Comparing `pyphysio-3.1.6/LICENSE` & `pyphysio-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/PKG-INFO` & `pyphysio-3.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphysio
-Version: 3.1.6
+Version: 3.1.7
 Summary: Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)
 Home-page: https://gitlab.com/a.bizzego/pyphysio
 Author: a.bizzego
 Author-email: andrea.bizzego@unitn.it
 Keywords: eda,gsr,ecg,bvp,fnirs,signal,analysis,physiological,psychopysiology,neuroscience
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
```

### Comparing `pyphysio-3.1.6/README.md` & `pyphysio-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/__init__.py` & `pyphysio-3.1.7/pyphysio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/_base_algorithm.py` & `pyphysio-3.1.7/pyphysio/_base_algorithm.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/artefacts.py` & `pyphysio-3.1.7/pyphysio/artefacts.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,16 @@
         # MSD = MSD - _np.median(MSD) #TODO: needed for method = 'mad'?
         MSD = (MSD >= th_MSD)
         AMP = (AMP > th_AMP)
         
         MA = (AMP | MSD).astype(int)
         
         idxlen_smooth = int(win_mask*fsamp)
-        MA = _np.convolve(MA, _np.ones(idxlen_smooth)/idxlen_smooth, 'same')
+        if idxlen_smooth > 0:
+            MA = _np.convolve(MA, _np.ones(idxlen_smooth)/idxlen_smooth, 'same')
         
         signal_out = _np.zeros(len(signal_values))
         idx_MA = _np.where(MA>0)[0] + half
         signal_out[idx_MA] = 1
         return(signal_out)
         
 class DetectMA_AR(_Algorithm):
@@ -151,16 +152,14 @@
     Motion Artifact Detection Algorithm based on AR models
 
     Parameters
     ----------
     order : int, default 0
         Order of the AR model. 
         Set order = 0  to use the order that minimizes the BIC.
-    th_std_coeff : float, optional, default 2
-        Standard deviation threshold when method is 'fixed'.
     fuse : bool, optional
         Flag indicating whether to detect motion artifacts by channel or globally.
     **kwargs : dict, optional
         Additional keyword arguments.
 
     """
```

### Comparing `pyphysio-3.1.6/pyphysio/filters.py` & `pyphysio-3.1.7/pyphysio/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,14 +517,52 @@
             out = _np.ones(len(signal))*out_dec[-1]
             out[:len(out_dec)] = out_dec
         else:
             print('Deconvolution method not implemented. Returning original signal.')
             out = s
         return out
 
+
+
+
+class Prewhitening(_Algorithm):
+    """
+    """
+
+    def __init__(self, order=50, optimize=True, **kwargs):
+        _Algorithm.__init__(self, order=order, optimize=optimize, **kwargs)
+        self.dimensions = {'time' : 0}
+
+    def algorithm(self, signal, **kwargs):
+        from statsmodels.tsa.ar_model import AutoReg as _AutoReg
+        
+        params = self._params
+        order = params['order']
+        optimize = params['optimize']
+        
+        signal_values = signal.p.get_values().ravel()
+        
+        if optimize:
+            bic_ = []
+            for i in _np.arange(1, order+1):
+                model = _AutoReg(signal_values, lags=i)
+                model_fit = model.fit()
+                bic_.append(model_fit.bic)
+            order_final = _np.argmin(bic_)+1
+        else:
+            order_final = order
+            
+        model = _AutoReg(signal_values, lags=order_final)
+        model_fit = model.fit()
+        
+        prewhit_signal = signal_values
+        prewhit_signal[order_final:] = model_fit.resid
+        
+        return(prewhit_signal)
+
 '''
 # TODO: check and convert to xarray
 
 class DenoiseEDA(_Algorithm):
     """
     Remove noise due to sensor displacement from the EDA signal.
```

### Comparing `pyphysio-3.1.6/pyphysio/generators/__init__.py` & `pyphysio-3.1.7/pyphysio/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/indicators/frequencydomain.py` & `pyphysio-3.1.7/pyphysio/indicators/frequencydomain.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/indicators/nonlinear.py` & `pyphysio-3.1.7/pyphysio/indicators/nonlinear.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/indicators/peaks.py` & `pyphysio-3.1.7/pyphysio/indicators/peaks.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/indicators/timedomain.py` & `pyphysio-3.1.7/pyphysio/indicators/timedomain.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/interactive.py` & `pyphysio-3.1.7/pyphysio/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self.ibi_plot = None
         self.done = False
         
         self.ecg = ecg
         self.ibi = ibi
         
         self.t_ibi = ibi.p.get_times()
+        self.t0 = self.t_ibi[0]
         self.v_ibi = ibi.p.get_values().ravel()
         self.idx_beats = _np.where(~_np.isnan(self.v_ibi))[0]
         self.idx_outliers = _np.array([self.idx_beats[0]])
         self.idx_beats_good = [i for i in self.idx_beats if i not in self.idx_outliers]
         
         self.min = _np.min(ecg.p.get_values())
         self.max = _np.max(ecg.p.get_values())
@@ -174,15 +175,15 @@
 #                    print("unselect: %d" % item)
                     Selector.selector.remove()
 
         # it is correct that the computation of the values is done at the end (line 186)
         def add(time, y, pos):
             fsamp = self.ecg.p.get_sampling_freq()
             
-            self.idx_beats = _np.insert(self.idx_beats, pos, time*fsamp)
+            self.idx_beats = _np.insert(self.idx_beats, pos, (time - self.t0)*fsamp)
             self.replot()
 
         def delete(item):
             self.idx_beats = _np.delete(self.idx_beats, item)
             self.replot()
             
         def switch_outlier(item):
```

### Comparing `pyphysio-3.1.6/pyphysio/loaders/_load_nirs.py` & `pyphysio-3.1.7/pyphysio/loaders/_load_nirs.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         nirs[k].p.main_signal.attrs = SD
         
     return(nirs)
 
 def load_snirf(datafile):
     from snirf import Snirf
     
-    snirf = Snirf(datafile, 'r+')
+    snirf = Snirf(datafile, 'r')
 
     nirs = snirf.nirs[0]
     data = nirs.data[0]
     probe = nirs.probe
 
     nirs_values = data.dataTimeSeries
     n_ch = nirs_values.shape[1]//2
```

### Comparing `pyphysio-3.1.6/pyphysio/segmenters.py` & `pyphysio-3.1.7/pyphysio/segmenters.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,29 +269,37 @@
     Raises
     ------
     AssertionError
         If the length of begins is not equal to the length of ends.
 
     """
 
-    def __init__(self, begins, ends, timeline=None, drop_mixed=True, drop_cut=True, **kwargs):
+    def __init__(self, begins, ends, labels=None, drop_mixed=True, drop_cut=True, **kwargs):
         #TODO: timeline can also be a list with labels of each segment
-        super(CustomSegments, self).__init__(timeline=timeline, drop_cut=drop_cut, drop_mixed=drop_mixed, **kwargs)
+        super(CustomSegments, self).__init__(labels=labels, drop_cut=drop_cut, drop_mixed=drop_mixed, **kwargs)
         
         assert len(begins) == len(ends), "The number of begins has to be equal to the number of ends :)"
+        if (labels is not None):
+            assert len(labels) == len(begins)
         self._i = -1
         self._b = begins
         self._e = ends
+        self._labels = labels
 
     def _next_segment(self):
         self._i += 1
         if self._i < len(self._b):
             b = self._b[self._i]
             e = self._e[self._i]
-            return self.manage_drops(b, e)
+            l = self._labels[self._i]
+            # b, e, _ = self.manage_drops(b, e)
+            # if (self._labels is not None):
+            #     l = self._labels[self._i]
+            return(b, e, l)
+                
         else:
             raise StopIteration()
 
 class LabelSegments(_Segmenter):
     """
     Segmenter class for creating custom segments frmo a signal.
 
@@ -466,54 +474,49 @@
             result_algorithm.append(res_out)
 
         result.append(_xr.concat(result_algorithm, dim='time'))
 
     result = _xr.merge(result,compat='override')
     return result
 
-#TODO: needed? if yes, fix--->
-'''
 def indicators2df(fmap_results):
     import pandas as _pd
 
-    k = list(fmap_results.keys())[0]
-    
-    for k,v in fmap_results.items():
-        assert isinstance(v, _Signal), 'Provided fmap_results should be all Signals'
+    k = list(fmap_results.keys())
+
         
-    ind_sample = fmap_results[k]
+    ind_sample = fmap_results[k[0]]
     assert ind_sample.ndim <=3, "computed results have more than three dimensions"
-    n_channels = ind_sample.get_nchannels()
-    n_components = ind_sample.get_ncomponents()
+    n_channels = ind_sample.p.get_nchannels()
+    n_components = ind_sample.p.get_ncomponents()
     
-    t = ind_sample.get_times()
-    label = ind_sample.get_info()['label'].get_values().ravel()
+    t = ind_sample.p.get_times()
+    label = ind_sample['label'].p.get_values().ravel()
     
     df_all = []
     for i_comp in range(n_components):
         for i_chan in range(n_channels):
             
             indicator_df = {}
             indicator_df['time'] = t
             indicator_df['label'] = label
     
             for key in list(fmap_results.keys()):
                 result_key = fmap_results[key]
                 
                 if ind_sample.ndim == 3:
-                    indicator_df[key] = result_key.get_values()[:, i_chan, i_comp].ravel()
+                    indicator_df[key] = result_key.p.get_values()[:, i_chan, i_comp].ravel()
                     indicator_df['component'] = _np.repeat(i_comp+1, len(t))
                     indicator_df['channel'] = _np.repeat(i_chan+1, len(t))
                     
                 else:
                     if ind_sample.ndim == 2:
-                        indicator_df[key] = result_key[:, i_chan].get_values().ravel()
+                        indicator_df[key] = result_key[:, i_chan].p.get_values().ravel()
                         indicator_df['channel'] = _np.repeat(i_chan+1, len(t))
                     else:
                         indicator_df[key] =  result_key
             
             df_all.append(_pd.DataFrame(indicator_df))
     
     
     df_all = _pd.concat(df_all, axis = 0)
     return(df_all)
-'''
```

### Comparing `pyphysio-3.1.6/pyphysio/signal.py` & `pyphysio-3.1.7/pyphysio/signal.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/activity/_presets.py` & `pyphysio-3.1.7/pyphysio/specialized/activity/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/eda/__init__.py` & `pyphysio-3.1.7/pyphysio/specialized/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/eda/_presets.py` & `pyphysio-3.1.7/pyphysio/specialized/eda/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/eeg/_presets.py` & `pyphysio-3.1.7/pyphysio/specialized/eeg/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/emg/_presets.py` & `pyphysio-3.1.7/pyphysio/specialized/emg/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/fnirs/__init__.py` & `pyphysio-3.1.7/pyphysio/specialized/fnirs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/fnirs/_convert.py` & `pyphysio-3.1.7/pyphysio/specialized/fnirs/_convert.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/fnirs/_data.py` & `pyphysio-3.1.7/pyphysio/specialized/fnirs/_data.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/fnirs/_dl_sqi.py` & `pyphysio-3.1.7/pyphysio/specialized/fnirs/_dl_sqi.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/heart/__init__.py` & `pyphysio-3.1.7/pyphysio/specialized/heart/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,53 +209,59 @@
         
         # STAGE 1 - EXTRACT BEAT POSITION SIGNAL
         # filtering
         signal_f =  _IIRFilter(fp=[0.5*fmax, 1.5*fmax], btype='bandpass')(signal)
         
         # find range for the adaptive peak detection
         delta = 0.5 * _SignalRange(win_len=1.5 / fmax, win_step=1 / fmax)(signal_f)
-
         delta = delta.values.ravel()
 
         # adjust for delta values equal to 0
         idx_delta_zeros = _np.where(delta == 0)[0]
         idx_delta_nozeros = _np.where(delta > 0)[0]
         delta[idx_delta_zeros] = _np.min(delta[idx_delta_nozeros])
 
         # detection of candidate peaks
         maxima = _PeakDetection(
-            delta=delta, refractory=ibi_min, start_max=True, return_peaks=True)(signal_f)
+            delta=delta, refractory=ibi_min, return_peaks=True)(signal_f)
         maxp = _np.where(~_np.isnan(maxima.values))[0].ravel()
         
+        if len(maxp) == 0:
+            return(_np.nan * _np.zeros(len(signal.p.main_signal.values)))
+        
         if maxp[0] == 0:
             maxp = maxp[1:]
 
         # STAGE 2 - IDENTIFY PEAKS using the signal derivative
         # compute the signal derivative
         dxdt = _Diff()(signal).values
-
+        
+        import matplotlib.pyplot as plt
         true_peaks = []
         # for each candidate peak find the correct peak
         for idx_beat in maxp:
             start_ = int(idx_beat - win_pre)
             if start_ < 0:
                 start_ = 0
 
             stop_ = int(idx_beat + win_post)
             if stop_ > len(dxdt):
                 stop_ = -1
-
+            
             # select portion of derivative where to search
             obs = dxdt[start_:stop_]
             peak_obs = _np.argmax(obs)
+                
             i_end = 1
-            while peak_obs == (len(obs) - i_end):
+            
+            while (peak_obs == (len(obs) - i_end)) and (i_end < len(obs)):
                 peak_obs = _np.argmax(obs[:-i_end])
                 i_end += 1
-
+            
+            
             true_obs = dxdt[start_ + peak_obs: stop_]
 
             true_obs = create_signal(abs(true_obs),
                                      sampling_freq=fsamp,
                                      start_time=times[start_ + peak_obs])
 
             # find the 'first minimum' (zero) the derivative (peak)
@@ -269,20 +275,23 @@
                 true_peaks.append(start_ + peak_obs + peak + 1)
             # else:
             #     print('Peak not found; idx_beat: ' + str(idx_beat))
             #     pass
         true_peaks = _np.array(true_peaks)
         
         # STAGE 3 - FINALIZE computing IBI
-        t_ibi = true_peaks / fsamp
-        v_ibi = _np.diff(t_ibi)
-        v_ibi = _np.insert(v_ibi, 0, v_ibi[0])
-
         ibi_scaffold = _np.nan * _np.zeros(len(signal.values))
-        ibi_scaffold[true_peaks] = v_ibi
+        
+        if len(true_peaks)>1:
+            t_ibi = true_peaks / fsamp
+            v_ibi = _np.diff(t_ibi)
+        
+            v_ibi = _np.insert(v_ibi, 0, v_ibi[0])
+
+            ibi_scaffold[true_peaks] = v_ibi
 
         return ibi_scaffold
 
 class BeatFromECG(_Algorithm):
     """
     Identify the beats in an ECG signal and compute the IBIs.
```

### Comparing `pyphysio-3.1.6/pyphysio/specialized/heart/_presets.py` & `pyphysio-3.1.7/pyphysio/specialized/heart/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/specialized/resp/_presets.py` & `pyphysio-3.1.7/pyphysio/specialized/resp/_presets.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/sqi.py` & `pyphysio-3.1.7/pyphysio/sqi.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/test_data/medical.txt.bz2` & `pyphysio-3.1.7/pyphysio/test_data/medical.txt.bz2`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/pyphysio/utils.py` & `pyphysio-3.1.7/pyphysio/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,35 +219,40 @@
         smooth = params['smooth']
 
         fsamp = signal.p.get_sampling_freq()
         idx_len = int(win_len * fsamp)
         idx_step = int(win_step * fsamp)
         
         signal_values = signal.values
+
         # print('>>> signalrange')
+        deltas = _np.zeros(len(signal_values))
+        
         if len(signal) < idx_len:
             print("Input signal is shorter than the window length.")
-            return _np.max(signal) - _np.min(signal)
+            deltas = deltas + (_np.max(signal_values) - _np.min(signal_values))
         else:
             windows = _np.arange(0, len(signal_values) - idx_len + 1, idx_step)
-            deltas = _np.zeros(len(signal_values))
+            
 
             curr_delta = 0
             for start in windows:
                 portion_curr = signal_values[start: start + idx_len]
                 curr_delta = _np.max(portion_curr) - _np.min(portion_curr)
                 deltas[start:start + idx_len] = curr_delta
 
             deltas[windows[-1] + idx_len:] = curr_delta
-
+            
             if smooth:
                 win_len = int(win_len*2*fsamp)
                 deltas = _np.convolve(deltas, _np.ones(win_len)/win_len, mode='same')
+                deltas = deltas[:len(signal_values)]
             # print('<<< signalrange')
-            return deltas
+            
+        return deltas
 
 class PSD(_Algorithm): #xarray done
     """
     Estimate the power spectral density (PSD) of the signal.
 
     Parameters
     ----------
```

### Comparing `pyphysio-3.1.6/pyphysio.egg-info/PKG-INFO` & `pyphysio-3.1.7/pyphysio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphysio
-Version: 3.1.6
+Version: 3.1.7
 Summary: Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)
 Home-page: https://gitlab.com/a.bizzego/pyphysio
 Author: a.bizzego
 Author-email: andrea.bizzego@unitn.it
 Keywords: eda,gsr,ecg,bvp,fnirs,signal,analysis,physiological,psychopysiology,neuroscience
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
```

### Comparing `pyphysio-3.1.6/pyphysio.egg-info/SOURCES.txt` & `pyphysio-3.1.7/pyphysio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/setup.py` & `pyphysio-3.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
               'pyphysio.specialized.fnirs',
               'pyphysio.specialized.heart',
               'pyphysio.specialized.resp',
               'pyphysio.indicators',
               'pyphysio.generators'],
     package_data={'pyphysio': ['test_data/*']},
     # data_files={'test_data_out': ['info_medical', 'medical.txt.bz2']},
-    version='3.1.6',
+    version='3.1.7',
     description='Python library for physiological signals analysis (IBI & HRV, ECG, BVP, EDA, RESP, fNIRS, ...)',
     author='a.bizzego',
     author_email='andrea.bizzego@unitn.it',
     url='https://gitlab.com/a.bizzego/pyphysio',
     keywords=['eda', 'gsr', 'ecg', 'bvp', 'fnirs', 'signal', 
               'analysis', 'physiological', 'psychopysiology', 'neuroscience'],
     classifiers=[
```

### Comparing `pyphysio-3.1.6/tests/test_eda_methods.py` & `pyphysio-3.1.7/tests/test_eda_methods.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/tests/test_filters.py` & `pyphysio-3.1.7/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/tests/test_fnirs.py` & `pyphysio-3.1.7/tests/test_fnirs.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/tests/test_get_sampling_freq.py` & `pyphysio-3.1.7/tests/test_get_sampling_freq.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/tests/test_ibi_estimators.py` & `pyphysio-3.1.7/tests/test_ibi_estimators.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/tests/test_segmenters.py` & `pyphysio-3.1.7/tests/test_segmenters.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/tests/test_signal.py` & `pyphysio-3.1.7/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pyphysio-3.1.6/tests/test_tools.py` & `pyphysio-3.1.7/tests/test_tools.py`

 * *Files identical despite different names*

