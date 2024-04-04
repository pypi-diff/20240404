# Comparing `tmp/mbapy-0.7.1.tar.gz` & `tmp/mbapy-0.7.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.7.1.tar", last modified: Thu Apr  4 11:05:23 2024, max compression
+gzip compressed data, was "mbapy-0.7.1b1.tar", last modified: Tue Mar 12 14:49:40 2024, max compression
```

## Comparing `mbapy-0.7.1.tar` & `mbapy-0.7.1b1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.579331 mbapy-0.7.1/
--rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.1/LICENSE
--rw-rw-rw-   0        0        0      163 2024-01-11 01:58:53.000000 mbapy-0.7.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7462 2024-04-04 11:05:23.578183 mbapy-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     5503 2024-02-23 13:27:31.000000 mbapy-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.366299 mbapy-0.7.1/mbapy/
--rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.1/mbapy/__init__.py
--rw-rw-rw-   0        0        0      402 2024-04-04 11:05:03.000000 mbapy-0.7.1/mbapy/__version__.py
--rw-rw-rw-   0        0        0    26515 2024-03-01 02:09:58.000000 mbapy-0.7.1/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.416525 mbapy-0.7.1/mbapy/bio/
--rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.1/mbapy/bio/__init__.py
--rw-rw-rw-   0        0        0    21232 2024-03-12 14:00:39.000000 mbapy-0.7.1/mbapy/bio/peptide.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.431660 mbapy-0.7.1/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.1/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.432659 mbapy-0.7.1/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.437657 mbapy-0.7.1/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.442798 mbapy-0.7.1/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.1/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.1/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.1/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.1/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.444797 mbapy-0.7.1/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.1/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0    22069 2024-03-09 11:28:49.000000 mbapy-0.7.1/mbapy/file.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.449796 mbapy-0.7.1/mbapy/file_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.1/mbapy/file_utils/__init__.py
--rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.1/mbapy/file_utils/image.py
--rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.1/mbapy/file_utils/video.py
--rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/game.py
--rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.1/mbapy/paper.py
--rw-rw-rw-   0        0        0    20352 2024-04-03 14:23:00.000000 mbapy-0.7.1/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.455915 mbapy-0.7.1/mbapy/sci_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.1/mbapy/sci_utils/__init__.py
--rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.1/mbapy/sci_utils/paper_download.py
--rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.1/mbapy/sci_utils/paper_parse.py
--rw-rw-rw-   0        0        0    16559 2024-01-20 12:03:17.000000 mbapy-0.7.1/mbapy/sci_utils/paper_search.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.489163 mbapy-0.7.1/mbapy/scripts/
--rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.1/mbapy/scripts/__init__.py
--rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.1/mbapy/scripts/__main__.py
--rw-rw-rw-   0        0        0     6954 2024-03-12 14:06:48.000000 mbapy-0.7.1/mbapy/scripts/_main_.py
--rw-rw-rw-   0        0        0      503 2024-01-25 04:33:05.000000 mbapy-0.7.1/mbapy/scripts/_script_utils_.py
--rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/scripts/avif.py
--rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.1/mbapy/scripts/cluster.py
--rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.1/mbapy/scripts/cnipa.py
--rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/scripts/cp.py
--rw-rw-rw-   0        0        0     4821 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/scripts/duitang.py
--rw-rw-rw-   0        0        0     2651 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/scripts/extract-dir.py
--rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.1/mbapy/scripts/extract_paper.py
--rw-rw-rw-   0        0        0    11285 2024-03-20 11:24:38.000000 mbapy-0.7.1/mbapy/scripts/mass.py
--rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/scripts/mv.py
--rw-rw-rw-   0        0        0    25827 2024-03-12 14:29:11.000000 mbapy-0.7.1/mbapy/scripts/peptide.py
--rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.1/mbapy/scripts/reviz.py
--rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/scripts/rm.py
--rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.1/mbapy/scripts/scihub.py
--rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.1/mbapy/scripts/scihub_selenium.py
--rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/scripts/splash_img.py
--rw-rw-rw-   0        0        0     9128 2024-03-14 08:21:47.000000 mbapy-0.7.1/mbapy/scripts/video.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.499158 mbapy-0.7.1/mbapy/stats/
--rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.1/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.1/mbapy/stats/cluster.py
--rw-rw-rw-   0        0        0    15721 2024-03-20 11:37:13.000000 mbapy-0.7.1/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.1/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     3784 2024-04-02 03:46:14.000000 mbapy-0.7.1/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0    13083 2024-04-03 09:43:58.000000 mbapy-0.7.1/mbapy/stats/test.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.563203 mbapy-0.7.1/mbapy/storage/
--rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.1/mbapy/storage/libsci.dll
--rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.1/mbapy/storage/libsci.so
--rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.1/mbapy/storage/libstats.dll
--rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.1/mbapy/storage/libstats.so
--rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.1/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.572185 mbapy-0.7.1/mbapy/web_utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.1/mbapy/web_utils/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.1/mbapy/web_utils/parse.py
--rw-rw-rw-   0        0        0    35766 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/web_utils/request.py
--rw-rw-rw-   0        0        0    28907 2024-02-23 13:27:31.000000 mbapy-0.7.1/mbapy/web_utils/spider.py
--rw-rw-rw-   0        0        0    11644 2024-02-23 13:30:29.000000 mbapy-0.7.1/mbapy/web_utils/task.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.413536 mbapy-0.7.1/mbapy.egg-info/
--rw-rw-rw-   0        0        0     7462 2024-04-04 11:05:23.000000 mbapy-0.7.1/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2016 2024-04-04 11:05:23.000000 mbapy-0.7.1/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:05:23.000000 mbapy-0.7.1/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-04 11:05:23.000000 mbapy-0.7.1/mbapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      908 2024-04-04 11:05:23.000000 mbapy-0.7.1/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-04 11:05:23.000000 mbapy-0.7.1/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      891 2024-02-23 13:27:31.000000 mbapy-0.7.1/requirements.json
--rw-rw-rw-   0        0        0       42 2024-04-04 11:05:23.579331 mbapy-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     3400 2024-04-04 11:05:15.000000 mbapy-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:05:23.576183 mbapy-0.7.1/test/
--rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.1/test/test_base.py
--rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.1/test/test_game.py
--rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.1/test/test_web.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.410085 mbapy-0.7.1b1/
+-rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/LICENSE
+-rw-rw-rw-   0        0        0      163 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7464 2024-03-12 14:49:40.409085 mbapy-0.7.1b1/PKG-INFO
+-rw-rw-rw-   0        0        0     5503 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/README.md
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.217236 mbapy-0.7.1b1/mbapy/
+-rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.1b1/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      404 2024-03-12 14:49:29.000000 mbapy-0.7.1b1/mbapy/__version__.py
+-rw-rw-rw-   0        0        0    26515 2024-03-01 02:09:58.000000 mbapy-0.7.1b1/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.257750 mbapy-0.7.1b1/mbapy/bio/
+-rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.1b1/mbapy/bio/__init__.py
+-rw-rw-rw-   0        0        0    21232 2024-03-12 14:00:39.000000 mbapy-0.7.1b1/mbapy/bio/peptide.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.276890 mbapy-0.7.1b1/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.278889 mbapy-0.7.1b1/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.288218 mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.293214 mbapy-0.7.1b1/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.1b1/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.1b1/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.297385 mbapy-0.7.1b1/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.1b1/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0    22069 2024-03-09 11:28:49.000000 mbapy-0.7.1b1/mbapy/file.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.305655 mbapy-0.7.1b1/mbapy/file_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.1b1/mbapy/file_utils/__init__.py
+-rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.1b1/mbapy/file_utils/image.py
+-rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.1b1/mbapy/file_utils/video.py
+-rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/game.py
+-rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.1b1/mbapy/paper.py
+-rw-rw-rw-   0        0        0    15911 2024-03-11 08:51:41.000000 mbapy-0.7.1b1/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.314816 mbapy-0.7.1b1/mbapy/sci_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.1b1/mbapy/sci_utils/__init__.py
+-rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.1b1/mbapy/sci_utils/paper_download.py
+-rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.1b1/mbapy/sci_utils/paper_parse.py
+-rw-rw-rw-   0        0        0    16559 2024-01-20 12:03:17.000000 mbapy-0.7.1b1/mbapy/sci_utils/paper_search.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.361477 mbapy-0.7.1b1/mbapy/scripts/
+-rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/__main__.py
+-rw-rw-rw-   0        0        0     6954 2024-03-12 14:06:48.000000 mbapy-0.7.1b1/mbapy/scripts/_main_.py
+-rw-rw-rw-   0        0        0      503 2024-01-25 04:33:05.000000 mbapy-0.7.1b1/mbapy/scripts/_script_utils_.py
+-rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/avif.py
+-rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.1b1/mbapy/scripts/cluster.py
+-rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/cnipa.py
+-rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/cp.py
+-rw-rw-rw-   0        0        0     4821 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/duitang.py
+-rw-rw-rw-   0        0        0     2651 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/extract-dir.py
+-rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/extract_paper.py
+-rw-rw-rw-   0        0        0     7628 2024-01-19 15:41:57.000000 mbapy-0.7.1b1/mbapy/scripts/mass.py
+-rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/mv.py
+-rw-rw-rw-   0        0        0    25827 2024-03-12 14:29:11.000000 mbapy-0.7.1b1/mbapy/scripts/peptide.py
+-rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.1b1/mbapy/scripts/reviz.py
+-rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/rm.py
+-rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/scihub.py
+-rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.1b1/mbapy/scripts/scihub_selenium.py
+-rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/scripts/splash_img.py
+-rw-rw-rw-   0        0        0     9126 2024-03-10 02:52:00.000000 mbapy-0.7.1b1/mbapy/scripts/video.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.375653 mbapy-0.7.1b1/mbapy/stats/
+-rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.1b1/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.1b1/mbapy/stats/cluster.py
+-rw-rw-rw-   0        0        0    15004 2023-12-11 09:26:16.000000 mbapy-0.7.1b1/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     1772 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    12718 2023-09-30 06:15:47.000000 mbapy-0.7.1b1/mbapy/stats/test.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.386913 mbapy-0.7.1b1/mbapy/storage/
+-rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/storage/libsci.dll
+-rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/storage/libsci.so
+-rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/storage/libstats.dll
+-rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/mbapy/storage/libstats.so
+-rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.1b1/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.399903 mbapy-0.7.1b1/mbapy/web_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.1b1/mbapy/web_utils/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.1b1/mbapy/web_utils/parse.py
+-rw-rw-rw-   0        0        0    35766 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/web_utils/request.py
+-rw-rw-rw-   0        0        0    28907 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/mbapy/web_utils/spider.py
+-rw-rw-rw-   0        0        0    11644 2024-02-23 13:30:29.000000 mbapy-0.7.1b1/mbapy/web_utils/task.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.254576 mbapy-0.7.1b1/mbapy.egg-info/
+-rw-rw-rw-   0        0        0     7464 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2016 2024-03-12 14:49:40.000000 mbapy-0.7.1b1/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      908 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-03-12 14:49:39.000000 mbapy-0.7.1b1/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      891 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/requirements.json
+-rw-rw-rw-   0        0        0       42 2024-03-12 14:49:40.410085 mbapy-0.7.1b1/setup.cfg
+-rw-rw-rw-   0        0        0     3400 2024-02-23 13:27:31.000000 mbapy-0.7.1b1/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-12 14:49:40.407086 mbapy-0.7.1b1/test/
+-rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/test/test_base.py
+-rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.1b1/test/test_game.py
+-rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.1b1/test/test_web.py
```

### Comparing `mbapy-0.7.1/LICENSE` & `mbapy-0.7.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/PKG-INFO` & `mbapy-0.7.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.7.1
+Version: 0.7.1b1
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Description: <!--
          * @Author: BHM-Bob 2262029386@qq.com
```

### Comparing `mbapy-0.7.1/README.md` & `mbapy-0.7.1b1/README.md`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/__init__.py` & `mbapy-0.7.1b1/mbapy/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/base.py` & `mbapy-0.7.1b1/mbapy/base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/bio/peptide.py` & `mbapy-0.7.1b1/mbapy/bio/peptide.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.7.1b1/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/bb.py` & `mbapy-0.7.1b1/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/data.py` & `mbapy-0.7.1b1/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/hyper_search.py` & `mbapy-0.7.1b1/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/loss.py` & `mbapy-0.7.1b1/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/m.py` & `mbapy-0.7.1b1/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/optim.py` & `mbapy-0.7.1b1/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/paper/bb.py` & `mbapy-0.7.1b1/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/dl_torch/utils.py` & `mbapy-0.7.1b1/mbapy/dl_torch/utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/file.py` & `mbapy-0.7.1b1/mbapy/file.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/file_utils/image.py` & `mbapy-0.7.1b1/mbapy/file_utils/image.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/file_utils/video.py` & `mbapy-0.7.1b1/mbapy/file_utils/video.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/game.py` & `mbapy-0.7.1b1/mbapy/game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/paper.py` & `mbapy-0.7.1b1/mbapy/paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/plot.py` & `mbapy-0.7.1b1/mbapy/plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import wraps
 from itertools import combinations
-from typing import Callable, Dict, List, Tuple, Union, Optional
+from typing import Dict, List, Tuple, Union
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
 import numpy as np
 import pandas as pd
 import seaborn as sns
@@ -63,150 +63,118 @@
         ret = ret[:n]
     return ret
     
 class AxisLable():
     def __init__(self, name:str, hold_space:int = 1) -> None:
         self.name = name
         self.hold_space = hold_space
-        self.father = None
-        self.child = set()
-        self._hash = id(self) # 固定hash值
-    def __eq__(self, other: 'AxisLable') -> bool:
-        return id(self) == id(other)
-    def __hash__(self) -> int:
-        return self._hash
     def add_space(self, space:int = 1):
         self.hold_space += space
-    def add_father(self, father: 'AxisLable'):
-        self.father = father
-        self.father.child.add(self)
 
-def pro_hue_pos(factors:List[str], df:pd.DataFrame, width:float,
-                hue_space:float, bar_space:float):
+def pro_hue_pos(factors:List[str], df:pd.DataFrame, width:float, bar_space:float):
     """
     Generate the position and labels for a grouped bar plot with multiple factors.
 
     Args:
-        - factors (List[str]): A list of strings representing the factors to group the bars by.
-        - df (pd.DataFrame): A pandas DataFrame containing the data for the bar plot.
-        - width (float): The width of each individual bar.
-        - hue_space (float): The space between each group of bars.
-        - bar_space (float): The space between each bar in a group.
+        factors (List[str]): A list of strings representing the factors to group the bars by.
+        df (pd.DataFrame): A pandas DataFrame containing the data for the bar plot.
+        width (float): The width of each individual bar.
+        bar_space (float): The space between each group of bars.
 
     Returns:
         Tuple[List[List[AxisLable]], List[List[float]]]: A tuple containing two lists. The first list contains the labels for each factor and each bar. The second list contains the x-positions for each bar.
 
-    Notes:
-        - `df` must be processed by `pro_bar_data` or `sort_df_factors`.
-        - The LAST factor will be the TOP level x-axis.
-    """
-    xlabels, fj_old, pos = [ [] for _ in range(len(factors))], None, []
-    xlabels_mat = df[factors].T.values.tolist()
-    # build relationships between each level sub-factors. build xlabels and allocte space for each level.
-    for i, fi in enumerate(factors[::-1]): # 从最高级开始
-        for j, fj in enumerate(df[fi]):
-            # 不同sub-factor 或 相同sub-factor但上级sub-factor不同
-            if (fi+fj) != fj_old or (i > 0 and xlabels_mat[i-1][j] != xlabels_mat[i-1][j-1]):
-                xlabels_mat[i][j] = AxisLable(fj)
-                xlabels[i].append(AxisLable(fj))
-                fj_old = fi+fj # 以防两个级别的factors中出现相同的sub-factors
-                if i > 0:
-                    xlabels_mat[i][j].add_father(xlabels_mat[i-1][j])
+    """
+    xlabels, fc_old, pos = [ [] for _ in range(len(factors))], '', []
+    for f_i, f in enumerate(factors):
+        for fc_i, fc in enumerate(df[f]):
+            if fc != fc_old:
+                xlabels[f_i].append(AxisLable(fc))
+                fc_old = fc
             else:
-                xlabels_mat[i][j] = xlabels_mat[i][j-1]
-                xlabels[i][-1].add_space()
-    xlabels = xlabels[::-1] # 倒序，使最高级在最后
+                xlabels[f_i][-1].add_space()
     xlabels.append([AxisLable(factors[-1], df.shape[0])])#master level has an extra total axis as x_title
     for axis_idx in range(len(xlabels)):
         pos.append([])
         if axis_idx == 0:
-            st_pos = hue_space
+            st_pos = bar_space
             for h_fc_idx in range(len(xlabels[axis_idx+1])):
                 sum_this_hue_bar = xlabels[axis_idx+1][h_fc_idx].hold_space
-                pos[axis_idx] += [st_pos+width*(i+0.5)+bar_space*i for i in range(sum_this_hue_bar)]
-                st_pos += (sum_this_hue_bar*width+(sum_this_hue_bar-1)*bar_space+hue_space)
+                pos[axis_idx] += [st_pos+width*(i+0.5) for i in range(sum_this_hue_bar)]
+                st_pos += (sum_this_hue_bar*width+bar_space)
         else:
             st_pos = 0
             for fc_idx in range(len(xlabels[axis_idx])):
                 this_hue_per = xlabels[axis_idx][fc_idx].hold_space / df.shape[0]
                 pos[axis_idx].append(st_pos+this_hue_per/2)
                 st_pos += this_hue_per
     return xlabels, pos
 
 def plot_bar(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     Stack bar plot with hue style
 
     Args:
-        - factors (List[str]): A list of factors. [low_lever_factor, medium_lever_factor, ...] or just one.
-        - tags (List[str]): A list of tags. [stack_low_y, stack_medium_y, ...] or just one.
-        - df (pd.DataFrame): A pandas DataFrame. From `pro_bar_data` or `sort_df_factors`.
-        - kwargs: Additional keyword arguments.
-            - width = 0.4
-            - bar_space = 0.2
-            - xrotations = [0]*len(factors)
-            - colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
-            - hatchs:['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
-            - font_size:None,
-            - labels:None,
-            - offset = [None] + [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors)-1)]
-            - edgecolor:['white'] * len(tags),
-            - linewidth: 0,
-            - err = None, will multiply 1.96 to yerr.
-            - err_kwargs = {'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k', 'ecolor':'black'}
+        factors (List[str]): A list of factors. [low_lever_factor, medium_lever_factor, ...] or just one.
+        tags (List[str]): A list of tags. [stack_low_y, stack_medium_y, ...] or just one.
+        df (pd.DataFrame): A pandas DataFrame. From pro_bar_data or sort_df_factors.
+        **kwargs: Additional keyword arguments.
+            width = 0.4\n
+            bar_space = 0.2\n
+            xrotations = [0]*len(factors)\n
+            colors = plt.rcParams['axes.prop_cycle'].by_key()['color']\n
+            hatchs:['-', '+', 'x', '\\', '*', 'o', 'O', '.'],\n
+            labels:None,\n
+            font_size:None, \n
+            offset = [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]\n
+            err = None\n
+            err_kwargs = {'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k'}
 
     Returns:
         np.array: An array of positions.
         ax1: An axis object.
     """
     ax1 = host_subplot(111, axes_class=axisartist.Axes)
     
     if len(tags) == 0:
-        # TODO: 可能存在'Unbond: 0'等其他情况
         tags = list(df.columns)[len(factors):]
-    args = get_wanted_args({'width':0.4, 'hue_space':0.2, 'bar_space':0.05,
-                            'xrotations':[0]*len(factors),
+    args = get_wanted_args({'width':0.4, 'bar_space':0.2, 'xrotations':[0]*len(factors),
                             'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
                             'hatchs':['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
                             'font_size':None,
                             'labels':None,
-                            'offset':[None] + [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))],
-                            'edgecolor':['white'] * len(tags),
-                            'linewidth': 0,
-                            'log': False,
+                            'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))],
+                            'edgecolor':'white',
                             'err':None,
-                            'err_kwargs':{'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k', 'ecolor':'black'}},
+                            'err_kwargs':{'capsize':5, 'capthick':2, 'elinewidth':2, 'fmt':' k'}},
                             kwargs)
     args.xrotations.append(0)
-    xlabels, pos = pro_hue_pos(factors, df, args.width, args.hue_space, args.bar_space)
+    xlabels, pos = pro_hue_pos(factors, df, args.width, args.bar_space)
     bottom = kwargs['bottom'] if 'bottom' in kwargs else np.zeros(len(pos[0]))
     
     for yIdx, yName in enumerate(tags):
         if args.labels is not None:
             label = args.labels[yIdx]
         else:
             label = yName
         ax1.bar(pos[0], df[yName], width = args.width, bottom = bottom, label=label,
-                edgecolor=args.edgecolor[yIdx], linewidth = args.linewidth,
-                color=args.colors[yIdx], log = args.log)
+                edgecolor=args.edgecolor, color=args.colors[yIdx])
         bottom += df[yName]
     ax1.set_xlim(0, pos[0][-1]+args.bar_space+args.width/2)
     ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
     plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=args.xrotations[0])
     if args.font_size is not None:
         plt.setp(ax1.axis["bottom"].major_ticklabels, fontsize=args.font_size[0])
-    if isinstance(args.offset[0], int) or isinstance(args.offset[0], float):
-        plt.setp(ax1.axis["bottom"].major_ticklabels, pad=args.offset[0])
     
     axs = []
     for idx, sub_pos in enumerate(pos[1:]):
         axs.append(ax1.twiny())
         axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
         new_axisline = axs[-1].get_grid_helper().new_fixed_axis
-        axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx+1]))
+        axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx]))
         plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=args.xrotations[idx+1])
         if args.font_size is not None:
             plt.setp(axs[-1].axis["bottom"].major_ticklabels, fontsize=args.font_size[idx+1])
         axs[-1].axis["top"].major_ticks.set_ticksize(0)
         # TODO : do not work
         axs[-1].axis["right"].major_ticks.set_ticksize(0)
         
@@ -256,45 +224,14 @@
                 axs[-1].axis["top"].major_ticks.set_ticksize(0)
                 # TODO : do not work
                 axs[-1].axis["right"].major_ticks.set_ticksize(0)            
             return np.array(pos[0]), ax1
         return core_wrapper
     return ret_wrapper
 
-def calcu_swarm_pos(x: float, y: np.ndarray, width: float, d: Optional[float] = None):
-    """
-   This function calculates the x-coordinates for the data points in a swarm plot.
-   The x-coordinates are calculated based on the given x-coordinate, y-coordinates,
-   and width of the swarm. If d is not None, it will be used as the distance between
-   the data points. Otherwise, it will be calculated based on the number of data points.
-   
-    Parameters:
-        - x: the x-coordinate of the center of the swarm.
-        - y: the y-coordinates of the data points.
-        - width: the width of the swarm.
-        - d: the distance between the data points. If None, it will be calculated based on the number of data points.
-        
-    Returns:
-        - A numpy array of x-coordinates for the data points.
-    """
-    def _calcu_arithmetic(x, n, w, d):
-        if isinstance(d, float) or isinstance(d, int):
-            a0 = x - (n-1)*d/2
-            return np.linspace(a0, a0+d*(n-1), n)
-        if n == 1:
-            return x
-        else:
-            a0, d = x-w/2, w/(n-1)
-            return np.linspace(a0, a0+d*(n-1), n)
-    ret = np.zeros(len(y))
-    for y_u in np.unique(y):
-        y_idx = np.where(y == y_u)[0]
-        ret[y_idx] = _calcu_arithmetic(x, len(y_idx), width, d)
-    return ret
-
 def qqplot(tags:List[str], df:pd.DataFrame, figsize = (12, 6), nrows = 1, ncols = 1, **kwargs):
     """
     Generate a QQ-plot for each column in the given DataFrame.
 
     Parameters:
         tags (List[str]): A list of column names to generate QQ-plots for.
         df (pd.DataFrame): The DataFrame containing the data.
@@ -337,34 +274,14 @@
     Returns:
         None
     """
     plt.tight_layout()
     plt.gcf().savefig(path, dpi=dpi, bbox_inches = bbox_inches)
     plt.show()
     
-def plot_stats_star(x1: float, x2: float, h: float, endpoint: float, p_value: float,
-                    ax = plt, p2star: Callable[[float], str] = p_value_to_stars):
-    """
-    Params
-        - x1: The x-coordinate of the left endpoint.
-        - x2: The x-coordinate of the right endpoint.
-        - h: The y-coordinate of the horizontal line.
-        - endpoint: The height of the endpoint.
-        - p_value: The p-value of the difference.
-        - ax: The `Axes` instance to plot on. Default is `plt`.
-        - p2star: A function that converts a p-value to a string of stars. Default is `p_value_to_stars`.
-
-    Returns:
-        None
-    """
-    ax.plot([x1, x2], [h, h], color='black')
-    ax.plot([x1, x1], [h, h-endpoint], color='black')
-    ax.plot([x2, x2], [h, h-endpoint], color='black')
-    ax.text((x1+x2)/2, h, p2star(p_value), ha='center')    
-    
 def plot_turkey(means, std_errs, tukey_results, min_star = 1):
     """
     Plot a bar chart showing the means of different groups along with the standard errors.
 
     Parameters:
         - means: A list of mean values for each group.
         - std_errs: A list of standard errors for each group.
@@ -393,23 +310,15 @@
                      p_value_to_stars(tukey_results.pvalues[i]), ha='center')
             height += min_height
 
     plt.xticks(x, tukey_results.groupsunique)
     return plt.gca()
 
 if __name__ == '__main__':
-    # dev code
-    df = pd.DataFrame({
-        'f1': ['a', 'b', 'b'],
-        'f2': ['M', 'M', 'N'],
-        'tag': [0.1, 0.2, 0.3]
-    })
-    pro_hue_pos(['f1', 'f2'], df, 0.4, 0.2, 0.1)
-    pos = calcu_swarm_pos(0.5, np.array([1, 2, 2, 1, 1, 1, 0, 0, 4]), 0.5)
-    # dev code
+    """dev code"""
     df = pd.read_excel('./data/plot.xlsx', sheet_name='MWM')
     df['Animal Type'] = df['Animal Type'].astype('str')
     model = mst.multicomp_turkeyHSD({'Animal Type':[]}, 'Duration', df)
     result = mst.turkey_to_table(model)
     print(result)
     sub_df = get_df_data({'Animal Type':[]}, ['Duration'], df)
     sub_df = pro_bar_data(['Animal Type'], ['Duration'], sub_df)
```

### Comparing `mbapy-0.7.1/mbapy/sci_utils/paper_download.py` & `mbapy-0.7.1b1/mbapy/sci_utils/paper_download.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/sci_utils/paper_parse.py` & `mbapy-0.7.1b1/mbapy/sci_utils/paper_parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/sci_utils/paper_search.py` & `mbapy-0.7.1b1/mbapy/sci_utils/paper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/_main_.py` & `mbapy-0.7.1b1/mbapy/scripts/_main_.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/avif.py` & `mbapy-0.7.1b1/mbapy/scripts/avif.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/cluster.py` & `mbapy-0.7.1b1/mbapy/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/cnipa.py` & `mbapy-0.7.1b1/mbapy/scripts/cnipa.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/cp.py` & `mbapy-0.7.1b1/mbapy/scripts/cp.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/duitang.py` & `mbapy-0.7.1b1/mbapy/scripts/duitang.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/extract-dir.py` & `mbapy-0.7.1b1/mbapy/scripts/extract-dir.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/extract_paper.py` & `mbapy-0.7.1b1/mbapy/scripts/extract_paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/mass.py` & `mbapy-0.7.1b1/mbapy/scripts/mass.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,212 +1,148 @@
 import argparse
 import glob
 import os
 from pathlib import Path
 from typing import Dict, List
 
-import scipy
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 os.environ['MBAPY_AUTO_IMPORT_TORCH'] = 'False'
 os.environ['MBAPY_FAST_LOAD'] = 'True'
-from mbapy.base import put_err
+from mbapy import base, file
 from mbapy.plot import get_palette, save_show
 
 if __name__ == '__main__':
-    from mbapy.scripts._script_utils_ import clean_path, show_args
+    from mbapy.scripts._script_utils_ import clean_path
 else:
-    from ._script_utils_ import clean_path, show_args
+    from ._script_utils_ import clean_path
 
 
 def plot_mass_load_file(path: Path):
     lines = path.read_text().splitlines()
     df = pd.DataFrame([line.split('\t') for line in lines[1:]],
                         columns = lines[0].split('\t'))
-    if df.shape[1] == 2 and df.columns[0] == 'Time' and df.columns[1] == 'Intensity':
-        # setattr(df, '_content_type', 'base peak') # NOTE: this does not work
-        df._attrs['content_type'] = 'base peak'
-        return df.astype(float)
-    elif df.shape[1] == 2 and df.columns[0] == 'Time' and df.columns[1] == 'Absorbance':
-        df._attrs['content_type'] = 'absorbance'
-        return df.astype(float)
-    elif df.shape[1] == 2 and df.columns[0] == 'Mass/Charge' and df.columns[1] == 'Intensity':
-        df._attrs['content_type'] = 'mass-charge'
+    if df.shape[1] == 2 and df.columns[0] == 'Time':
         return df.astype(float)
     elif df.shape[1] == 10:
-        df._attrs['content_type'] = 'peak list'
         return df.astype({'Mass/Charge':float, 'Height':float, 'Charge':int,
                             'Monoisotopic':str, 'Mass (charge)':str,
                             'Mass/charge (charge)':str})
-    else:
-        return put_err(f'Can not recognizable txt file: {path}, skip.')
 
 def plot_mass_plot_basepeak(name:str, base_peak: pd.DataFrame, args):
-    fig, ax = plt.subplots(figsize=(10, 6))
+    fig, ax = plt.subplots(figsize=(8, 6))
     ax.plot(base_peak['Time'], base_peak['Intensity'], color = args.color)
     plt.xticks(size = 20)
     plt.yticks(size = 20)
     plt.yscale('log')
     ax.set_title(f'{name} (TIC of TOF MS)', fontsize=25)
     ax.set_xlabel('Time (min)', fontsize=25)
     ax.set_ylabel('Intensity (cps)', fontsize=25)
-    save_show(os.path.join(args.output, f'{name} base peak.png'), dpi = 300)
-    
-def plot_mass_plot_absorbance(name:str, df: pd.DataFrame, args):
-    fig, ax = plt.subplots(figsize=(10, 6))
-    ax.plot(df['Time'], df['Absorbance'], color = args.color)
-    plt.xticks(size = 20)
-    plt.yticks(size = 20)
-    ax.set_title(f'{name} (Absorbance)', fontsize=25)
-    ax.set_xlabel('Time (min)', fontsize=25)
-    au_units = ('m' if df['Absorbance'].max() > 10 else '') + 'AU'
-    ax.set_ylabel(f'Absorbance ({au_units})', fontsize=25)
-    ax.set_xlim(0, df['Time'].max())
-    save_show(os.path.join(args.output, f'{name} absorbance.png'), dpi = 300)
-
-def _plot_vlines(x, y, col, label = None):
-    plt.vlines(x, 0, y, colors = [col] * len(x), label = label)
-    plt.scatter(x, y, c = col)
-    
-def plot_mass_plot_peaklist(name:str, df: pd.DataFrame, args):
+    save_show(os.path.join(args.output, f'{name}.png'), dpi = 300)
+
+def plot_mass_plot_peaklist(name:str, peak_list: pd.DataFrame, args):
+    def plot_vlines(x, y, col, label = ''):
+        plt.vlines(x, 0, y, colors = [col] * len(x), label = label)
+        plt.scatter(x, y, c = col)
     fig, ax = plt.subplots(figsize=(8, 6))
-    idx = df['Monoisotopic'] == 'Yes'
-    _plot_vlines(df['mass_data'], df['Height'], args.color)
+    idx = peak_list['Monoisotopic'] == 'Yes'
+    plot_vlines(peak_list['mass_data'], peak_list['Height'], args.color)
     labels_ms = np.array(list(args.labels.keys()))
-    for ms, h, c in zip(df['mass_data'][idx], df['Height'][idx],
-                        df['Charge'][idx]):
+    for ms, h, c in zip(peak_list['mass_data'][idx], peak_list['Height'][idx],
+                        peak_list['Charge'][idx]):
         matched = np.where(np.abs(labels_ms - ms) < args.labels_eps)[0]
         if matched.size > 0:
             label, color = args.labels.get(labels_ms[matched[0]])
-            _plot_vlines([ms], [h], color, label)
+            plot_vlines([ms], [h], color, label)
             ax.text(ms, h, f'* {ms:.2f}({c:d})', fontsize=15, color = color)
         else:
             ax.text(ms, h, f'* {ms:.2f}({c:d})', fontsize=15, color = args.color)
     plt.xticks(size = 20)
     plt.yticks(size = 20)
     plt.yscale('log')
     axis_lim = (1-args.expand, 1+args.expand)
-    plt.xlim(df['mass_data'].min() * axis_lim[0], df['mass_data'].max() * axis_lim[1])
-    plt.ylim(df['Height'].min() * axis_lim[0], df['Height'].max() * axis_lim[1])
+    plt.xlim(peak_list['mass_data'].min() * axis_lim[0], peak_list['mass_data'].max() * axis_lim[1])
+    plt.ylim(peak_list['Height'].min() * axis_lim[0], peak_list['Height'].max() * axis_lim[1])
     ax.set_title(f'{name} (Peak List of TOF MS)', fontsize=25)
     ax.set_xlabel(f'Mass{"" if args.mass else "/charge"}', fontsize=25)
     ax.set_ylabel('Intensity (cps)', fontsize=25)
     plt.legend(fontsize=15)
-    save_show(os.path.join(args.output, f'{name} peak list.png'), dpi = 300)
-    
-def plot_mass_plot_masscharge(name: str, df: pd.DataFrame, args):
-    # process data, filter data, then search peaks
-    print('searching peaks...')
-    min_height = df['Intensity'].max() * args.min_height_percent / 100
-    df = df[df['Intensity'] >= min_height] # save time in searching, widths should be small
-    peaks = scipy.signal.find_peaks_cwt(df['Intensity'], 3)
-    if peaks.any():
-        df = df.iloc[peaks, :]
-    print(f'searching done. {len(df)} peaks found.')
-    df.to_csv(os.path.join(args.output, f'{name} {df._attrs["content_type"]}.csv'))
-    # plot
-    fig, ax = plt.subplots(figsize=(8, 6))
-    _plot_vlines(df['Mass/Charge'], df['Intensity'], args.color)
-    labels_ms = np.array(list(args.labels.keys()))
-    for ms, h in zip(df['Mass/Charge'], df['Intensity']):
-        matched = np.where(np.abs(labels_ms - ms) < args.labels_eps)[0]
-        if matched.size > 0:
-            label, color = args.labels.get(labels_ms[matched[0]])
-            _plot_vlines([ms], [h], color, label)
-            ax.text(ms, h, f'* {ms:.2f}', fontsize=15, color = color)
-        else:
-            ax.text(ms, h, f'* {ms:.2f}', fontsize=15, color = args.color)
-    # fix style
-    plt.xticks(size = 20)
-    plt.yticks(size = 20)
-    plt.yscale('log')
-    axis_lim = (1-args.expand, 1+args.expand)
-    plt.xlim(df['Mass/Charge'].min() * axis_lim[0], df['Mass/Charge'].max() * axis_lim[1])
-    plt.ylim(df['Intensity'].min() * axis_lim[0], df['Intensity'].max() * axis_lim[1])
-    ax.set_title(f'{name} (Mass/Charge of TOF MS)', fontsize=25)
-    ax.set_xlabel(f'Mass/Charge', fontsize=25)
-    ax.set_ylabel('Intensity (cps)', fontsize=25)
-    plt.legend(fontsize=15)
-    save_show(os.path.join(args.output, f'{name} Mass-Charge.png'), dpi = 300)
+    save_show(os.path.join(args.output, f'{name}.png'), dpi = 300)
     
 def plot_mass(args):           
     # process args
     args.dir = clean_path(args.dir)
-    args.output = clean_path(args.output) if args.output else args.dir
+    print(f'get arg: dir: {args.dir}')
+    # find base peak file and peak list file
+    paths = glob.glob(os.path.join(args.dir, '*.txt'))
+    dfs = {path:plot_mass_load_file(Path(path)) for path in paths}
+    dfs = {k:v for k,v in dfs.items() if v is not None}
+    if not dfs:
+        raise FileNotFoundError(f'can not find two files in {args.dir}')
     if not os.path.isdir(args.output):
         print(f'given output {args.output} is a file, change it to parent dir')
         args.output = args.output.parent
+    print(f'get arg: output: {args.output}')
+    print(f'get arg: mass: {args.mass}')
     labels, colors = {}, get_palette(len(args.labels.split(';')), mode = 'hls')
     for idx, i in enumerate(args.labels.split(';')):
-        if i:
-            pack = i.split(',')
-            mass, label, color = pack[0], pack[1], pack[2] if len(pack) == 3 else colors[idx]
-            labels[float(mass)] = [label, color]
+        pack = i.split(',')
+        mass, label, color = pack[0], pack[1], pack[2] if len(pack) == 3 else colors[idx]
+        labels[float(mass)] = [label, color]
     args.labels = labels
-    # find base peak file and peak list file
-    paths = glob.glob(os.path.join(args.dir, '*.txt'))
-    dfs = {path:plot_mass_load_file(Path(path)) for path in paths}
-    dfs = {k:v for k,v in dfs.items() if v is not None}
-    if not dfs:
-        raise FileNotFoundError(f'can not find txt files in {args.dir}')
-    # show args
-    show_args(args, ['dir', 'output', 'labels', 'labels_eps', 'color','min_height','mass', 'expand'])
+    print(f'get arg: labels: {labels}')
     # show data general info and output peak list DataFrame
     for n,df in dfs.items():
         name = Path(n).resolve().stem
-        print(f'\n\n\n\n\n{name}: {df._attrs["content_type"]}:\n', df)
-        df.to_csv(os.path.join(args.output, f'{name} {df._attrs["content_type"]}.csv'))
+        print(f'\n\n\n\n\n{name}: peak list: signal(s):\n', df)
+        df.to_csv(os.path.join(args.output, f'{name}.csv'))
         # process Mass (charge) and identify mass
-        if df._attrs['content_type'] == 'peak list':
+        if df.shape[1] == 10:
             df['Mass (charge)'] = df['Mass (charge)'].str.extract(r'(\d+\.\d+)', expand=False).astype(float)
             df['Mass/charge (charge)'] = df['Mass/charge (charge)'].str.extract(r'(\d+\.\d+)', expand=False).astype(float)
             df['mass_data'] = df['Mass (charge)'] if args.mass else df['Mass/charge (charge)']
             drop_idx = df[df['Height'] < args.min_height].index
             if not drop_idx.empty:
                 print(f'drop data with min-height: {args.min_height} and only these data remained:\n',
                       df[df['Height'] >= args.min_height])
                 df.drop(drop_idx, axis = 0, inplace = True)
-        # plot each df
-        print(f'plotting {name}: {df._attrs["content_type"]}')
-        if df._attrs["content_type"] == 'base peak':
+    # plot each df
+    for n,df in dfs.items():
+        name = Path(n).resolve().stem
+        if df.shape[1] == 2:
+            # plot base peak
+            print(f'ploting base peak: {name}')
             plot_mass_plot_basepeak(name, df, args)
-        elif df._attrs["content_type"] == 'absorbance':
-            plot_mass_plot_absorbance(name, df, args)
-        elif df._attrs["content_type"] == 'peak list': # avoid drop all data but still draw
+        elif df.shape[0] > 0: # avoid drop all data but still draw
+            # plot peak list
+            print(f'ploting peak list: {name}')
             plot_mass_plot_peaklist(name, df, args)
-        elif df._attrs["content_type"] =='mass-charge':
-            plot_mass_plot_masscharge(name, df, args)
-        else:    
-            put_err(f'can not recognize data type: {df._attrs["content_type"]}, skip.')
-
 
 _str2func = {
     'plot-mass': plot_mass,
 }
 
 
 def main(sys_args: List[str] = None):
     args_paser = argparse.ArgumentParser()
     subparsers = args_paser.add_subparsers(title='subcommands', dest='sub_command')
     
     plot_mass_args = subparsers.add_parser('plot-mass', description='plot mass spectrum')
     # set dir argument
     plot_mass_args.add_argument("-d", "--dir", type = str, help="txt file directory")
     # set output file argument
-    plot_mass_args.add_argument("-o", "--output", type = str, default=None,
-                                help="output file dir or path, default is %(default)s, means same as input dir")
+    plot_mass_args.add_argument("-o", "--output", type = str, default='.',
+                                help="output file dir or path, default is %(default)s")
     # set draw argument
     plot_mass_args.add_argument('-m', '--mass', action='store_true', default=False,
                                 help='draw Mass instead of Mass/charge which is Mass+z, default is %(default)s')
     plot_mass_args.add_argument('-min', '--min-height', type = int, default=0,
-                                help='filter data with min height in peak list plot, default is %(default)s')
-    plot_mass_args.add_argument('-minp', '--min-height-percent', type = int, default=10,
-                                help='filter data with min height percent to hightest in mass/charge plot, default is %(default)s')
+                                help='filter data with min height, default is %(default)s')
     plot_mass_args.add_argument('-col', '--color', type = str, default='black',
                                 help='draw color, default is %(default)s')
     plot_mass_args.add_argument('-labels', '--labels', type = str, default='',
                                 help='labels, input as 1000,Pep1;1050,Pep2, default is %(default)s')
     plot_mass_args.add_argument('--labels-eps', type = float, default=0.5,
                                 help='eps to recognize labels, default is %(default)s')
     plot_mass_args.add_argument('-expand', '--expand', type = float, default=0.2,
@@ -215,14 +151,11 @@
     
     args = args_paser.parse_args(sys_args)
     
     if args.sub_command in _str2func:
         print(f'excuting command: {args.sub_command}')
         _str2func[args.sub_command](args)
     else:
-        put_err(f'no such sub commmand: {args.sub_command}')
+        base.put_err(f'no such sub commmand: {args.sub_command}')
 
 if __name__ == "__main__":
-    # dev code, MUST COMMENT OUT BEFORE RELEASE
-    # pass
-    
     main()
```

### Comparing `mbapy-0.7.1/mbapy/scripts/mv.py` & `mbapy-0.7.1b1/mbapy/scripts/mv.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/peptide.py` & `mbapy-0.7.1b1/mbapy/scripts/peptide.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/reviz.py` & `mbapy-0.7.1b1/mbapy/scripts/reviz.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/rm.py` & `mbapy-0.7.1b1/mbapy/scripts/rm.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/scihub.py` & `mbapy-0.7.1b1/mbapy/scripts/scihub.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/scihub_selenium.py` & `mbapy-0.7.1b1/mbapy/scripts/scihub_selenium.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/splash_img.py` & `mbapy-0.7.1b1/mbapy/scripts/splash_img.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/scripts/video.py` & `mbapy-0.7.1b1/mbapy/scripts/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Date: 2024-02-05 12:03:34
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-03-14 16:21:45
+LastEditTime: 2024-03-10 10:51:47
 Description: 
 '''
 import argparse
 import os
 from pathlib import Path
 from typing import Dict, List
 
@@ -170,11 +170,11 @@
     else:
         put_err(f'no such sub commmand: {args.sub_command}')
 
 
 if __name__ == "__main__":
     # dev code
     # comment the following line when release
-    # main(['extract', 'frames', '-i', './data_tmp/video.mp4'])
+    main(['extract', 'frames', '-i', './data_tmp/video.mp4'])
     
     # RELEASE CODE
     main()
```

### Comparing `mbapy-0.7.1/mbapy/stats/__init__.py` & `mbapy-0.7.1b1/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/stats/cluster.py` & `mbapy-0.7.1b1/mbapy/stats/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/stats/df.py` & `mbapy-0.7.1b1/mbapy/stats/df.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-04-10 20:59:26
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-03-20 19:36:03
+LastEditTime: 2023-07-10 16:42:29
 Description: pd.dataFrame utils
 '''
 import itertools
 from functools import wraps
 from typing import Dict, List
 
 import numpy as np
@@ -22,29 +22,30 @@
     from ..base import CDLL, get_dll_path_for_sys, put_err
     from ..file import update_excel
 
 def get_value(df:pd.DataFrame, column:str, mask:np.array)->list:
     return df.loc[mask, column].tolist()
 
 
+# TODO : not use itertools.product
 def pro_bar_data(factors:List[str], tags:List[str], df:pd.DataFrame, **kwargs):
     """
     cacu mean and SE for each combinations of facotors\n
     data should be like this:\n
     | factor1 | factor2 | y1 | y2 |...\n
     |  f1_1   |   f2_1  |2.1 |-2  |...\n
     after process\n
     | factor1 | factor2 | y1(mean) | y1_SE(SE) | y1_N(sum_data) |...\n
     |  f1_1   |   f2_1  |2.1       |   -2      |   32           |...\n
     kwargs:
         min_sample_N:int : min N threshold(>=)
     """
     # kwargs
-    min_sample_N = kwargs.get('min_sample_N', 1)
-    assert min_sample_N > 0, 'min_sample_N <= 0 !'
+    min_sample_N = 1 if 'min_sample_N' not in kwargs else kwargs['min_sample_N']
+    assert min_sample_N > 0, 'min_sample_N <= 0'
     # pro
     if len(tags) == 0:
         tags = list(df.columns)[len(factors):]
     factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
     ndf = [factors.copy()]
     for tag in tags:
         ndf[0] += [tag, tag+'_SE', tag+'_N']
@@ -63,50 +64,34 @@
                     line.append(np.NaN)
                 line.append(values.shape[0])
             ndf.append(list(factorCombi) + line)
     return pd.DataFrame(ndf[1:], columns=ndf[0])
 
 def pro_bar_data_R(factors:List[str], tags:List[str], df:pd.DataFrame, suffixs:List[str], **kwargs):
     """
-    Params:
-        - factors: list of factors to group by
-        - tags: list of tags to calculate mean and SE for
-        - df: input DataFrame
-        - suffixs: list of suffixes for each tag, used to distinguish different tags with same name
-        - kwargs:
-            - min_sample_N: int, min N threshold(>=)
-            
-    Return:
-        - pd.DataFrame, with each row representing a combination of factors and tags, and columns as follows:
-            - factors: the values of factors
-            - tags: the values of tags, with suffixes
-            - values: the values of tags, calculated by core_func
-            
-    Example
-    >>> @pro_bar_data_R(['solution', 'type'], ['root', 'leaf'], ndf)\n
-    >>> def plot_func(values, **kwargs):
-    >>>     return produced vars in list format whose length equal to len(suffix)
+    wrapper\n
+    @pro_bar_data_R(['solution', 'type'], ['root', 'leaf'], ndf)\n
+    def plot_func(values, **kwargs):
+        return produced vars in list format whose length equal to len(suffix)
     """
     def ret_wrapper(core_func):
         def core_wrapper(**kwargs):
-            min_sample_N = kwargs.get('min_sample_N', 1)
-            assert min_sample_N > 0, 'min_sample_N <= 0 !'
             nonlocal tags
             if len(tags) == 0:
                 tags = list(df.columns)[len(factors):]
             factor_contents:List[List[str]] = [ df[f].unique().tolist() for f in factors ]
             ndf = [factors.copy()]
             for tag in tags:
                 for suffix in suffixs:
                     ndf[0] += [tag+suffix]
             for factorCombi in itertools.product(*factor_contents):
                 factorMask = np.array(df[factors[0]] == factorCombi[0])
                 for i in range(1, len(factors)):
                     factorMask &= np.array(df[factors[i]] == factorCombi[i])
-                if factorMask.sum() > min_sample_N:
+                if(factorMask.sum() > 0):
                     line = []
                     for idx, tag in enumerate(tags):
                         values = np.array(df.loc[factorMask, [tag]])
                         ret_line = core_func(values)
                         assert len(ret_line) == len(suffixs), 'length of return value of core_func != len(suffixs)'
                         line += ret_line
                     ndf.append(list(factorCombi) + line)
```

### Comparing `mbapy-0.7.1/mbapy/stats/geography.py` & `mbapy-0.7.1b1/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/stats/test.py` & `mbapy-0.7.1b1/mbapy/stats/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-04-04 16:45:23
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-04-03 17:43:43
+LastEditTime: 2023-07-10 16:44:48
 Description: 
 '''
 from itertools import combinations
 from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
@@ -36,17 +36,17 @@
 
 def _get_x1_x2(x1 = None, x2 = None,
                factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None):
     """以同一列factors提取同一列tag的x1和x2，其余factors仅作筛选作用"""
     if factors is not None and tag is not None and df is not None:
         sub_df = msd.get_df_data(factors, [tag], df)
         fac_name = list(factors.keys())[0]
-        x1 = sub_df.loc[sub_df[fac_name] == factors[fac_name][0], [tag]].values.reshape(-1)
+        x1 = sub_df.loc[sub_df[fac_name] == factors[fac_name][0], [tag]].values
         if len(factors[fac_name]) == 2:
-            x2 = sub_df.loc[sub_df[fac_name] == factors[fac_name][1], [tag]].values.reshape(-1)
+            x2 = sub_df.loc[sub_df[fac_name] == factors[fac_name][1], [tag]].values
         elif len(factors[fac_name]) > 2:
             raise ValueError('Only support 1 or 2 value of factors')
     return x1, x2
 
 def _get_x1_x2_R(x1 = None, x2 = None,
                factors:Dict[str, List[str]] = None, tags:List[str] = None, df:pd.DataFrame = None):
     """
@@ -66,15 +66,15 @@
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     return scipy.stats.ttest_1samp(x1, x2, **kwargs)
 
 def ttest_ind(x1 = None, x2 = None,
                  factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
     独立样本t检验(双样本T检验):检验两组独立样本均值是否相等\n
-    要求正态分布，正态检验结果由scipy.stats.levene计算并返回\n
+    要求正太分布，正太检验结果由scipy.stats.levene计算并返回\n
     levene 检验P值 > 0.05，接受原假设，认为两组方差相等\n
     如不相等， scipy.stats.ttest_ind() 函数中的参数 equal_var 会设置成 False
     """
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     levene = scipy.stats.levene(x1, x2)
     return levene.pvalue, scipy.stats.ttest_ind(x1, x2, equal_var=levene.pvalue > 0.05)
 
@@ -91,22 +91,14 @@
     评估了两个抽样群体是否可能来自同一群体，这两个群体在数据方面是否具有相同的形状？\n
     证明这两个群体是否来自于具有不同水平的相关变量的人群。\n
     此包装函数同时支持直接输入和mbapy-style数据输入
     """
     x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
     return scipy.stats.mannwhitneyu(x1, x2, **kwargs)
 
-def wilcoxon(x1 = None, x2 = None,
-             factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
-    """
-    Wilcoxon signed-rank test, 样本不符合正态分布但配对时使用。
-    """
-    x1, x2 = _get_x1_x2(x1, x2, factors, tag, df)
-    return scipy.stats.ranksums(x1, x2, **kwargs)
-
 def shapiro(x1 = None,
             factors:Dict[str, List[str]] = None, tag:str = None, df:pd.DataFrame = None, **kwargs):
     """
     shapiro正态检验:\n
     p > 0.05 为正态分布
     """
     x1, _ = _get_x1_x2(x1, None, factors, tag, df)
```

### Comparing `mbapy-0.7.1/mbapy/storage/libsci.dll` & `mbapy-0.7.1b1/mbapy/storage/libsci.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/storage/libsci.so` & `mbapy-0.7.1b1/mbapy/storage/libsci.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/storage/libstats.dll` & `mbapy-0.7.1b1/mbapy/storage/libstats.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/storage/libstats.so` & `mbapy-0.7.1b1/mbapy/storage/libstats.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/web.py` & `mbapy-0.7.1b1/mbapy/web.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/web_utils/parse.py` & `mbapy-0.7.1b1/mbapy/web_utils/parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/web_utils/request.py` & `mbapy-0.7.1b1/mbapy/web_utils/request.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/web_utils/spider.py` & `mbapy-0.7.1b1/mbapy/web_utils/spider.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy/web_utils/task.py` & `mbapy-0.7.1b1/mbapy/web_utils/task.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy.egg-info/PKG-INFO` & `mbapy-0.7.1b1/mbapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.7.1
+Version: 0.7.1b1
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Description: <!--
          * @Author: BHM-Bob 2262029386@qq.com
```

### Comparing `mbapy-0.7.1/mbapy.egg-info/SOURCES.txt` & `mbapy-0.7.1b1/mbapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/mbapy.egg-info/requires.txt` & `mbapy-0.7.1b1/mbapy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/requirements.json` & `mbapy-0.7.1b1/requirements.json`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/setup.py` & `mbapy-0.7.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-04-04 19:05:15
+LastEditTime: 2024-02-20 17:12:04
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 thanks to https://github.com/gaogaotiantian/viztracer/blob/master/setup.py
 """
@@ -104,8 +104,8 @@
         'full': requirements['std'] + requirements['full'],
         },
 )
 
 # pip install .
 
 # python setup.py sdist
-# twine upload dist/mbapy-0.7.1.tar.gz
+# twine upload dist/mbapy-0.7.0.tar.gz
```

### Comparing `mbapy-0.7.1/test/test_base.py` & `mbapy-0.7.1b1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/test/test_game.py` & `mbapy-0.7.1b1/test/test_game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.1/test/test_web.py` & `mbapy-0.7.1b1/test/test_web.py`

 * *Files identical despite different names*

