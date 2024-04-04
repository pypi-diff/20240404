# Comparing `tmp/ionbench-0.4.0.tar.gz` & `tmp/ionbench-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ionbench-0.4.0.tar", last modified: Thu Mar 28 15:12:47 2024, max compression
+gzip compressed data, was "ionbench-0.4.1.tar", last modified: Thu Apr  4 15:23:52 2024, max compression
```

## Comparing `ionbench-0.4.0.tar` & `ionbench-0.4.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.701542 ionbench-0.4.0/
--rw-rw-rw-   0        0        0     1491 2023-09-15 08:58:40.000000 ionbench-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5369 2024-03-28 15:12:47.692819 ionbench-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4404 2024-03-04 14:35:22.000000 ionbench-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.211034 ionbench-0.4.0/ionbench/
--rw-rw-rw-   0        0        0     2060 2024-02-19 17:13:07.000000 ionbench-0.4.0/ionbench/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.322962 ionbench-0.4.0/ionbench/benchmarker/
--rw-rw-rw-   0        0        0       48 2024-02-19 17:32:13.000000 ionbench-0.4.0/ionbench/benchmarker/__init__.py
--rw-rw-rw-   0        0        0    37534 2024-03-28 14:07:15.000000 ionbench-0.4.0/ionbench/benchmarker/benchmarker.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.136296 ionbench-0.4.0/ionbench/data/
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.376698 ionbench-0.4.0/ionbench/data/loewe2016/
--rw-rw-rw-   0        0        0     1902 2024-03-26 11:30:58.000000 ionbench-0.4.0/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt
--rw-rw-rw-   0        0        0     2929 2024-03-25 13:04:48.000000 ionbench-0.4.0/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt
--rw-rw-rw-   0        0        0   468578 2024-03-26 11:58:01.000000 ionbench-0.4.0/ionbench/data/loewe2016/ikr.csv
--rw-rw-rw-   0        0        0   483972 2024-03-26 10:27:20.000000 ionbench-0.4.0/ionbench/data/loewe2016/ikur.csv
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.406752 ionbench-0.4.0/ionbench/data/moreno2016/
--rw-rw-rw-   0        0        0      947 2024-01-31 11:58:14.000000 ionbench-0.4.0/ionbench/data/moreno2016/ina.csv
--rw-rw-rw-   0        0        0     2786 2024-02-20 17:22:01.000000 ionbench-0.4.0/ionbench/data/moreno2016/moreno2016.mmt
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.475098 ionbench-0.4.0/ionbench/data/staircase/
--rw-rw-rw-   0        0        0      838 2024-03-06 13:55:41.000000 ionbench-0.4.0/ionbench/data/staircase/beattie-2017-ikr-hh.mmt
--rw-rw-rw-   0        0        0   647878 2024-03-06 14:25:28.000000 ionbench-0.4.0/ionbench/data/staircase/dataHH.csv
--rw-rw-rw-   0        0        0   658551 2024-03-06 14:30:35.000000 ionbench-0.4.0/ionbench/data/staircase/dataMM.csv
--rw-rw-rw-   0        0        0     2254 2024-03-06 14:29:18.000000 ionbench-0.4.0/ionbench/data/staircase/fink-2008-ikr-mm.mmt
--rw-rw-rw-   0        0        0     1142 2024-03-06 14:06:01.000000 ionbench-0.4.0/ionbench/data/staircase/staircase-pace.mmt
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.486830 ionbench-0.4.0/ionbench/data/test/
--rw-rw-rw-   0        0        0      440 2023-11-23 15:28:16.000000 ionbench-0.4.0/ionbench/data/test/data.csv
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.538860 ionbench-0.4.0/ionbench/modification/
--rw-rw-rw-   0        0        0       50 2023-10-17 16:49:57.000000 ionbench-0.4.0/ionbench/modification/__init__.py
--rw-rw-rw-   0        0        0    16367 2024-03-21 12:50:48.000000 ionbench-0.4.0/ionbench/modification/modification.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:46.553162 ionbench-0.4.0/ionbench/optimisers/
--rw-rw-rw-   0        0        0      153 2023-10-26 10:28:33.000000 ionbench-0.4.0/ionbench/optimisers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.035361 ionbench-0.4.0/ionbench/optimisers/external_optimisers/
--rw-rw-rw-   0        0        0     5624 2024-03-21 12:57:10.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/DE_Zhou2009.py
--rw-rw-rw-   0        0        0     2932 2024-03-21 12:57:09.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Bot2012.py
--rw-rw-rw-   0        0        0     5153 2024-03-21 12:57:09.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Cairns2017.py
--rw-rw-rw-   0        0        0     3726 2024-03-21 12:57:09.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py
--rw-rw-rw-   0        0        0     3385 2024-03-21 12:57:09.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py
--rw-rw-rw-   0        0        0     3223 2024-03-21 15:12:02.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py
--rw-rw-rw-   0        0        0     2267 2024-03-25 15:28:47.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py
--rw-rw-rw-   0        0        0    10669 2024-03-26 10:17:05.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py
--rw-rw-rw-   0        0        0     7970 2024-03-25 15:17:59.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     5530 2024-03-25 15:17:58.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py
--rw-rw-rw-   0        0        0    10097 2024-03-21 13:12:06.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/SA_Vanier1999.py
--rw-rw-rw-   0        0        0     4293 2024-03-21 13:12:06.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py
--rw-rw-rw-   0        0        0     1491 2023-11-14 17:57:37.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/__init__.py
--rw-rw-rw-   0        0        0    15056 2024-03-28 15:05:33.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py
--rw-rw-rw-   0        0        0     8595 2024-03-25 15:17:59.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     7612 2024-03-25 15:17:58.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py
--rw-rw-rw-   0        0        0     5125 2024-03-21 13:03:27.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py
--rw-rw-rw-   0        0        0     9131 2024-03-25 15:33:26.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/ppso_Chen2012.py
--rw-rw-rw-   0        0        0     6752 2024-03-25 15:52:04.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/pso_Cabo2022.py
--rw-rw-rw-   0        0        0     4418 2024-03-26 10:13:34.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/pso_Seemann2009.py
--rw-rw-rw-   0        0        0     2183 2024-03-21 15:19:01.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
--rw-rw-rw-   0        0        0     2685 2024-03-21 13:11:58.000000 ionbench-0.4.0/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.189825 ionbench-0.4.0/ionbench/optimisers/pints_optimisers/
--rw-rw-rw-   0        0        0      311 2023-08-23 14:25:17.000000 ionbench-0.4.0/ionbench/optimisers/pints_optimisers/__init__.py
--rw-rw-rw-   0        0        0     1937 2024-03-21 16:56:40.000000 ionbench-0.4.0/ionbench/optimisers/pints_optimisers/cmaes_pints.py
--rw-rw-rw-   0        0        0     1638 2024-03-21 16:56:40.000000 ionbench-0.4.0/ionbench/optimisers/pints_optimisers/nelderMead_pints.py
--rw-rw-rw-   0        0        0     1611 2024-03-21 16:56:40.000000 ionbench-0.4.0/ionbench/optimisers/pints_optimisers/pso_pints.py
--rw-rw-rw-   0        0        0     1623 2024-03-21 16:56:40.000000 ionbench-0.4.0/ionbench/optimisers/pints_optimisers/snes_pints.py
--rw-rw-rw-   0        0        0     1625 2024-03-21 16:56:40.000000 ionbench-0.4.0/ionbench/optimisers/pints_optimisers/xnes_pints.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.304200 ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/
--rw-rw-rw-   0        0        0      397 2023-11-14 13:29:40.000000 ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/__init__.py
--rw-rw-rw-   0        0        0     2312 2024-03-21 13:11:58.000000 ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
--rw-rw-rw-   0        0        0     1770 2024-03-28 14:52:14.000000 ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/lm_scipy.py
--rw-rw-rw-   0        0        0     2900 2024-03-21 16:55:00.000000 ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
--rw-rw-rw-   0        0        0     2905 2024-03-21 16:55:01.000000 ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/powell_scipy.py
--rw-rw-rw-   0        0        0     2320 2024-03-21 16:55:01.000000 ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py
--rw-rw-rw-   0        0        0     2009 2024-03-28 14:52:14.000000 ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.388895 ionbench-0.4.0/ionbench/problems/
--rw-rw-rw-   0        0        0      160 2023-11-23 15:25:37.000000 ionbench-0.4.0/ionbench/problems/__init__.py
--rw-rw-rw-   0        0        0     8195 2024-03-28 13:37:02.000000 ionbench-0.4.0/ionbench/problems/loewe2016.py
--rw-rw-rw-   0        0        0    17417 2024-03-28 13:37:02.000000 ionbench-0.4.0/ionbench/problems/moreno2016.py
--rw-rw-rw-   0        0        0     9604 2024-03-28 13:37:02.000000 ionbench-0.4.0/ionbench/problems/staircase.py
--rw-rw-rw-   0        0        0     5839 2024-03-21 12:50:42.000000 ionbench-0.4.0/ionbench/problems/test.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.421275 ionbench-0.4.0/ionbench/tracker/
--rw-rw-rw-   0        0        0       40 2024-02-19 17:33:47.000000 ionbench-0.4.0/ionbench/tracker/__init__.py
--rw-rw-rw-   0        0        0    16857 2024-03-28 13:43:43.000000 ionbench-0.4.0/ionbench/tracker/tracker.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.478765 ionbench-0.4.0/ionbench/uncertainty/
--rw-rw-rw-   0        0        0       91 2023-09-08 12:44:51.000000 ionbench-0.4.0/ionbench/uncertainty/__init__.py
--rw-rw-rw-   0        0        0     7060 2024-03-21 12:36:02.000000 ionbench-0.4.0/ionbench/uncertainty/fim.py
--rw-rw-rw-   0        0        0    12104 2024-03-27 11:54:37.000000 ionbench-0.4.0/ionbench/uncertainty/profile_likelihood.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.621122 ionbench-0.4.0/ionbench/utils/
--rw-rw-rw-   0        0        0      259 2024-03-22 14:22:36.000000 ionbench-0.4.0/ionbench/utils/__init__.py
--rw-rw-rw-   0        0        0     7768 2024-03-21 12:50:42.000000 ionbench-0.4.0/ionbench/utils/autodiff.py
--rw-rw-rw-   0        0        0     1590 2024-03-20 15:36:43.000000 ionbench-0.4.0/ionbench/utils/cache.py
--rw-rw-rw-   0        0        0     4805 2024-03-28 13:55:01.000000 ionbench-0.4.0/ionbench/utils/classes_pints.py
--rw-rw-rw-   0        0        0     1516 2024-02-12 13:34:30.000000 ionbench-0.4.0/ionbench/utils/multistart.py
--rw-rw-rw-   0        0        0     2544 2024-03-26 09:47:49.000000 ionbench-0.4.0/ionbench/utils/particle_optimisers.py
--rw-rw-rw-   0        0        0     7625 2024-03-25 15:28:47.000000 ionbench-0.4.0/ionbench/utils/population_optimisers.py
--rw-rw-rw-   0        0        0     2460 2024-03-28 14:52:19.000000 ionbench-0.4.0/ionbench/utils/scipy_setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.685437 ionbench-0.4.0/ionbench.egg-info/
--rw-rw-rw-   0        0        0     5369 2024-03-28 15:12:45.000000 ionbench-0.4.0/ionbench.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3565 2024-03-28 15:12:46.000000 ionbench-0.4.0/ionbench.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 15:12:45.000000 ionbench-0.4.0/ionbench.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2024-03-28 15:12:45.000000 ionbench-0.4.0/ionbench.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-28 15:12:45.000000 ionbench-0.4.0/ionbench.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 15:12:47.703508 ionbench-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     8469 2024-03-28 14:30:43.000000 ionbench-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-28 15:12:47.670267 ionbench-0.4.0/test/
--rw-rw-rw-   0        0        0     5403 2024-03-08 13:55:46.000000 ionbench-0.4.0/test/test_modifications.py
--rw-rw-rw-   0        0        0      542 2024-03-05 15:24:03.000000 ionbench-0.4.0/test/test_multistart.py
--rw-rw-rw-   0        0        0     2052 2024-03-26 10:22:59.000000 ionbench-0.4.0/test/test_optimisers.py
--rw-rw-rw-   0        0        0    29511 2024-03-28 14:36:40.000000 ionbench-0.4.0/test/test_problems.py
--rw-rw-rw-   0        0        0      773 2024-02-20 17:03:12.000000 ionbench-0.4.0/test/test_uncertainty.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.557291 ionbench-0.4.1/
+-rw-rw-rw-   0        0        0     1491 2023-09-15 08:58:40.000000 ionbench-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5369 2024-04-04 15:23:52.551955 ionbench-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4404 2024-03-04 14:35:22.000000 ionbench-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.208842 ionbench-0.4.1/ionbench/
+-rw-rw-rw-   0        0        0     2060 2024-02-19 17:13:07.000000 ionbench-0.4.1/ionbench/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.305537 ionbench-0.4.1/ionbench/benchmarker/
+-rw-rw-rw-   0        0        0       48 2024-02-19 17:32:13.000000 ionbench-0.4.1/ionbench/benchmarker/__init__.py
+-rw-rw-rw-   0        0        0    38265 2024-04-04 14:59:14.000000 ionbench-0.4.1/ionbench/benchmarker/benchmarker.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.139294 ionbench-0.4.1/ionbench/data/
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.378336 ionbench-0.4.1/ionbench/data/loewe2016/
+-rw-rw-rw-   0        0        0     1902 2024-03-26 11:30:58.000000 ionbench-0.4.1/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt
+-rw-rw-rw-   0        0        0     2929 2024-03-25 13:04:48.000000 ionbench-0.4.1/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt
+-rw-rw-rw-   0        0        0   468578 2024-03-26 11:58:01.000000 ionbench-0.4.1/ionbench/data/loewe2016/ikr.csv
+-rw-rw-rw-   0        0        0   483972 2024-03-26 10:27:20.000000 ionbench-0.4.1/ionbench/data/loewe2016/ikur.csv
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.401142 ionbench-0.4.1/ionbench/data/moreno2016/
+-rw-rw-rw-   0        0        0      947 2024-01-31 11:58:14.000000 ionbench-0.4.1/ionbench/data/moreno2016/ina.csv
+-rw-rw-rw-   0        0        0     2786 2024-02-20 17:22:01.000000 ionbench-0.4.1/ionbench/data/moreno2016/moreno2016.mmt
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.471706 ionbench-0.4.1/ionbench/data/staircase/
+-rw-rw-rw-   0        0        0      838 2024-03-06 13:55:41.000000 ionbench-0.4.1/ionbench/data/staircase/beattie-2017-ikr-hh.mmt
+-rw-rw-rw-   0        0        0   647878 2024-03-06 14:25:28.000000 ionbench-0.4.1/ionbench/data/staircase/dataHH.csv
+-rw-rw-rw-   0        0        0   658551 2024-03-06 14:30:35.000000 ionbench-0.4.1/ionbench/data/staircase/dataMM.csv
+-rw-rw-rw-   0        0        0     2254 2024-03-06 14:29:18.000000 ionbench-0.4.1/ionbench/data/staircase/fink-2008-ikr-mm.mmt
+-rw-rw-rw-   0        0        0     1142 2024-03-06 14:06:01.000000 ionbench-0.4.1/ionbench/data/staircase/staircase-pace.mmt
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.492538 ionbench-0.4.1/ionbench/data/test/
+-rw-rw-rw-   0        0        0      440 2023-11-23 15:28:16.000000 ionbench-0.4.1/ionbench/data/test/data.csv
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.528603 ionbench-0.4.1/ionbench/modification/
+-rw-rw-rw-   0        0        0       50 2023-10-17 16:49:57.000000 ionbench-0.4.1/ionbench/modification/__init__.py
+-rw-rw-rw-   0        0        0    16367 2024-03-21 12:50:48.000000 ionbench-0.4.1/ionbench/modification/modification.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.543301 ionbench-0.4.1/ionbench/optimisers/
+-rw-rw-rw-   0        0        0      153 2023-10-26 10:28:33.000000 ionbench-0.4.1/ionbench/optimisers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:51.930328 ionbench-0.4.1/ionbench/optimisers/external_optimisers/
+-rw-rw-rw-   0        0        0     5624 2024-03-21 12:57:10.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/DE_Zhou2009.py
+-rw-rw-rw-   0        0        0     2932 2024-03-21 12:57:09.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Bot2012.py
+-rw-rw-rw-   0        0        0     5153 2024-03-21 12:57:09.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Cairns2017.py
+-rw-rw-rw-   0        0        0     3726 2024-03-21 12:57:09.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py
+-rw-rw-rw-   0        0        0     3385 2024-03-21 12:57:09.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py
+-rw-rw-rw-   0        0        0     3223 2024-03-21 15:12:02.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py
+-rw-rw-rw-   0        0        0     2267 2024-03-25 15:28:47.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py
+-rw-rw-rw-   0        0        0    10669 2024-03-26 10:17:05.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py
+-rw-rw-rw-   0        0        0     7970 2024-03-25 15:17:59.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     5530 2024-03-25 15:17:58.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py
+-rw-rw-rw-   0        0        0    10097 2024-03-21 13:12:06.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/SA_Vanier1999.py
+-rw-rw-rw-   0        0        0     4293 2024-03-21 13:12:06.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py
+-rw-rw-rw-   0        0        0     1491 2023-11-14 17:57:37.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/__init__.py
+-rw-rw-rw-   0        0        0    15056 2024-03-28 15:05:33.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py
+-rw-rw-rw-   0        0        0     8595 2024-03-25 15:17:59.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     7612 2024-03-25 15:17:58.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py
+-rw-rw-rw-   0        0        0     5125 2024-03-21 13:03:27.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py
+-rw-rw-rw-   0        0        0     9131 2024-03-25 15:33:26.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/ppso_Chen2012.py
+-rw-rw-rw-   0        0        0     6752 2024-03-25 15:52:04.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/pso_Cabo2022.py
+-rw-rw-rw-   0        0        0     4418 2024-03-26 10:13:34.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/pso_Seemann2009.py
+-rw-rw-rw-   0        0        0     2183 2024-03-21 15:19:01.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py
+-rw-rw-rw-   0        0        0     2685 2024-03-21 13:11:58.000000 ionbench-0.4.1/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.020763 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/
+-rw-rw-rw-   0        0        0      311 2023-08-23 14:25:17.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/__init__.py
+-rw-rw-rw-   0        0        0     1937 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/cmaes_pints.py
+-rw-rw-rw-   0        0        0     1638 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/nelderMead_pints.py
+-rw-rw-rw-   0        0        0     1611 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/pso_pints.py
+-rw-rw-rw-   0        0        0     1623 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/snes_pints.py
+-rw-rw-rw-   0        0        0     1625 2024-03-21 16:56:40.000000 ionbench-0.4.1/ionbench/optimisers/pints_optimisers/xnes_pints.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.120826 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/
+-rw-rw-rw-   0        0        0      397 2023-11-14 13:29:40.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/__init__.py
+-rw-rw-rw-   0        0        0     2312 2024-03-21 13:11:58.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py
+-rw-rw-rw-   0        0        0     1770 2024-03-28 14:52:14.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/lm_scipy.py
+-rw-rw-rw-   0        0        0     2900 2024-03-21 16:55:00.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py
+-rw-rw-rw-   0        0        0     2905 2024-03-21 16:55:01.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/powell_scipy.py
+-rw-rw-rw-   0        0        0     2320 2024-03-21 16:55:01.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py
+-rw-rw-rw-   0        0        0     2009 2024-03-28 14:52:14.000000 ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.187777 ionbench-0.4.1/ionbench/problems/
+-rw-rw-rw-   0        0        0      160 2023-11-23 15:25:37.000000 ionbench-0.4.1/ionbench/problems/__init__.py
+-rw-rw-rw-   0        0        0     8195 2024-03-28 13:37:02.000000 ionbench-0.4.1/ionbench/problems/loewe2016.py
+-rw-rw-rw-   0        0        0    17417 2024-03-28 13:37:02.000000 ionbench-0.4.1/ionbench/problems/moreno2016.py
+-rw-rw-rw-   0        0        0     9604 2024-03-28 13:37:02.000000 ionbench-0.4.1/ionbench/problems/staircase.py
+-rw-rw-rw-   0        0        0     5839 2024-03-21 12:50:42.000000 ionbench-0.4.1/ionbench/problems/test.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.212627 ionbench-0.4.1/ionbench/tracker/
+-rw-rw-rw-   0        0        0       40 2024-02-19 17:33:47.000000 ionbench-0.4.1/ionbench/tracker/__init__.py
+-rw-rw-rw-   0        0        0    16857 2024-03-28 13:43:43.000000 ionbench-0.4.1/ionbench/tracker/tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.259804 ionbench-0.4.1/ionbench/uncertainty/
+-rw-rw-rw-   0        0        0       91 2023-09-08 12:44:51.000000 ionbench-0.4.1/ionbench/uncertainty/__init__.py
+-rw-rw-rw-   0        0        0     7060 2024-03-21 12:36:02.000000 ionbench-0.4.1/ionbench/uncertainty/fim.py
+-rw-rw-rw-   0        0        0    12104 2024-03-27 11:54:37.000000 ionbench-0.4.1/ionbench/uncertainty/profile_likelihood.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.456807 ionbench-0.4.1/ionbench/utils/
+-rw-rw-rw-   0        0        0      259 2024-03-22 14:22:36.000000 ionbench-0.4.1/ionbench/utils/__init__.py
+-rw-rw-rw-   0        0        0     7768 2024-03-21 12:50:42.000000 ionbench-0.4.1/ionbench/utils/autodiff.py
+-rw-rw-rw-   0        0        0     1590 2024-03-20 15:36:43.000000 ionbench-0.4.1/ionbench/utils/cache.py
+-rw-rw-rw-   0        0        0     4805 2024-03-28 13:55:01.000000 ionbench-0.4.1/ionbench/utils/classes_pints.py
+-rw-rw-rw-   0        0        0     1516 2024-02-12 13:34:30.000000 ionbench-0.4.1/ionbench/utils/multistart.py
+-rw-rw-rw-   0        0        0     2544 2024-03-26 09:47:49.000000 ionbench-0.4.1/ionbench/utils/particle_optimisers.py
+-rw-rw-rw-   0        0        0     7625 2024-03-25 15:28:47.000000 ionbench-0.4.1/ionbench/utils/population_optimisers.py
+-rw-rw-rw-   0        0        0     2460 2024-04-04 08:48:53.000000 ionbench-0.4.1/ionbench/utils/scipy_setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.543711 ionbench-0.4.1/ionbench.egg-info/
+-rw-rw-rw-   0        0        0     5369 2024-04-04 15:23:50.000000 ionbench-0.4.1/ionbench.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3565 2024-04-04 15:23:51.000000 ionbench-0.4.1/ionbench.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 15:23:50.000000 ionbench-0.4.1/ionbench.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2024-04-04 15:23:50.000000 ionbench-0.4.1/ionbench.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-04 15:23:50.000000 ionbench-0.4.1/ionbench.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 15:23:52.558336 ionbench-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     8469 2024-04-04 15:02:07.000000 ionbench-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 15:23:52.533715 ionbench-0.4.1/test/
+-rw-rw-rw-   0        0        0     5403 2024-03-08 13:55:46.000000 ionbench-0.4.1/test/test_modifications.py
+-rw-rw-rw-   0        0        0      542 2024-03-05 15:24:03.000000 ionbench-0.4.1/test/test_multistart.py
+-rw-rw-rw-   0        0        0     2052 2024-03-26 10:22:59.000000 ionbench-0.4.1/test/test_optimisers.py
+-rw-rw-rw-   0        0        0    29511 2024-03-28 14:36:40.000000 ionbench-0.4.1/test/test_problems.py
+-rw-rw-rw-   0        0        0      773 2024-02-20 17:03:12.000000 ionbench-0.4.1/test/test_uncertainty.py
```

### Comparing `ionbench-0.4.0/LICENSE.txt` & `ionbench-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/PKG-INFO` & `ionbench-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionbench
-Version: 0.4.0
+Version: 0.4.1
 Summary: A benchmarking tool for comparing different parameter optimization algorithms for ion channel models
 Home-page: https://github.com/CardiacModelling/ionbench
 Author: Matt J. Owen
 Author-email: matt.owen@nottingham.ac.uk
 Project-URL: Bug Reports, https://github.com/CardiacModelling/ionbench/issues
 Project-URL: Source, https://github.com/CardiacModelling/ionbench
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ionbench-0.4.0/README.md` & `ionbench-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/__init__.py` & `ionbench-0.4.1/ionbench/__init__.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/benchmarker/benchmarker.py` & `ionbench-0.4.1/ionbench/benchmarker/benchmarker.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,15 +331,16 @@
         Returns
         -------
         cost : float
             The RMSE cost of the parameters.
 
         """
         testOutput = np.array(
-            self.simulate(parameters, np.arange(0, self.T_MAX, self.TIMESTEP), incrementSolveCounter=incrementSolveCounter))
+            self.simulate(parameters, np.arange(0, self.T_MAX, self.TIMESTEP),
+                          incrementSolveCounter=incrementSolveCounter))
         cost = self.rmse(testOutput, self.DATA)
         return cost
 
     def signed_error(self, parameters):
         """
         Similar to the cost method, but instead returns the vector of residuals/errors in the model output.
 
@@ -434,15 +435,15 @@
             penalty = self.parameter_penalty(parametersMG) + self.rate_penalty(parametersMG)
             assert penalty.data > 0
             penalty.backward()
             grad = np.zeros(self.n_parameters())
             for i in range(self.n_parameters()):
                 grad[i] = parametersMG[i].grad if parametersMG[i].grad is not None else 0
             cost = float(penalty.data)
-            error = cost*np.array(len(self.DATA))
+            error = cost * np.array(len(self.DATA))
             J = np.zeros((len(self.DATA), self.n_parameters()))
             for i in range(len(self.DATA)):
                 J[i,] = grad
             self.tracker.update(parameters, incrementSolveCounter=False, solveType='grad', cost=cost,
                                 solveTime=0)
         else:
             # Inside any bounds, so we can get sensitivities
@@ -541,15 +542,15 @@
         parameters : list or numpy array
             Vector of parameters to use for the calculation of the steady state.
         """
         if 'moreno' in self.NAME:
             V = -120
         else:
             V = -80
-
+        At = np.zeros(self.n_parameters())
         if 'hh' in str(type(self._ANALYTICAL_MODEL)):
             t = [mg.tensor(a, dtype=np.double) for a in parameters]
             state = self._ANALYTICAL_MODEL._steady_state_function(V, *t)
             s_state = np.zeros((len(parameters), len(state)))
             for j in range(len(state)):
                 state[j].backward()
                 sens = [float(t[i].grad) if t[i].grad is not None else 0 for i in range(self.n_parameters())]
@@ -597,15 +598,26 @@
         if state is not None:
             if np.any(np.array(state) < 0):
                 npstate = np.array(state)
                 if np.all(np.abs(npstate[npstate < 0]) < 1e-12):
                     # If the negative values are very close to zero, then we can assume they are zero
                     state = [max(0, s) / np.sum(npstate) for s in npstate]
                 else:
-                    raise ValueError('Steady state contains significant (>1e-12) negative values. This needs fixing.')
+                    # Some parameter combinations lead to negative steady state values (not just rounding errors). We don't set the state in this case as a positive steady state doesn't exist.
+                    if np.any(At < 0):
+                        warnings.warn(
+                            'The parameters give negative transition probabilities which leads to an invalid steady state. Will use states defined in the problem instead.')
+                        state = None
+                    else:
+                        print(parameters)
+                        print(At)
+                        raise ValueError(
+                            'Steady state contains significant (>1e-12) negative values. This needs fixing.')
+
+        if state is not None:
             self.sim.set_state(state)
             if self.sensitivityCalc:
                 self.simSens.set_state(state)
                 self.simSens._s_state = s_state
 
     def solve_with_sensitivities(self, times):
         """
@@ -744,15 +756,15 @@
         penalty = 0
         for i, rateFunc in enumerate(self._RATE_FUNCTIONS):
             k = max(rateFunc(parameters, self.V_HIGH), rateFunc(parameters, self.V_LOW))
             if 'moreno' in self.NAME:
                 if k < self.RATE_MIN:
                     penalty += 1e5
                     penalty += 1e5 * np.log(1 + np.abs(k - self.RATE_MIN))
-                elif (k > self.RATE_MAX and i not in [3, 5]) or (k > self.RATE_MAX*10000 and i in [3, 5]):
+                elif (k > self.RATE_MAX and i not in [3, 5]) or (k > self.RATE_MAX * 10000 and i in [3, 5]):
                     penalty += 1e5
                     penalty += 1e5 * np.log(1 + np.abs(k - self.RATE_MAX))
             else:
                 if k < self.RATE_MIN:
                     penalty += 1e5
                     penalty += 1e5 * np.log(1 + np.abs(k - self.RATE_MIN))
                 elif k > self.RATE_MAX:
```

### Comparing `ionbench-0.4.0/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt` & `ionbench-0.4.1/ionbench/data/loewe2016/courtemanche-1998-ikr.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt` & `ionbench-0.4.1/ionbench/data/loewe2016/courtemanche-1998-ikur.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/loewe2016/ikr.csv` & `ionbench-0.4.1/ionbench/data/loewe2016/ikr.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/loewe2016/ikur.csv` & `ionbench-0.4.1/ionbench/data/loewe2016/ikur.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/moreno2016/ina.csv` & `ionbench-0.4.1/ionbench/data/moreno2016/ina.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/moreno2016/moreno2016.mmt` & `ionbench-0.4.1/ionbench/data/moreno2016/moreno2016.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/staircase/beattie-2017-ikr-hh.mmt` & `ionbench-0.4.1/ionbench/data/staircase/beattie-2017-ikr-hh.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/staircase/dataHH.csv` & `ionbench-0.4.1/ionbench/data/staircase/dataHH.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/staircase/dataMM.csv` & `ionbench-0.4.1/ionbench/data/staircase/dataMM.csv`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/staircase/fink-2008-ikr-mm.mmt` & `ionbench-0.4.1/ionbench/data/staircase/fink-2008-ikr-mm.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/data/staircase/staircase-pace.mmt` & `ionbench-0.4.1/ionbench/data/staircase/staircase-pace.mmt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/modification/modification.py` & `ionbench-0.4.1/ionbench/modification/modification.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/DE_Zhou2009.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/DE_Zhou2009.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Bot2012.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Bot2012.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Cairns2017.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Cairns2017.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007a.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Gurkiewicz2007b.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/GA_Smirnov2020.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/NMPSO_Clausen2020.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/NMPSO_Liu2011.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/PSOTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/PSO_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/SA_Vanier1999.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/SA_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/SPSA_Spall1998.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/__init__.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/__init__.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/curvilinearGD_Dokos2004.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/hybridPSOTRRTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/hybridPSOTRR_Loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/patternSearch_Kohjitani2022.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/ppso_Chen2012.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/ppso_Chen2012.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/pso_Cabo2022.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/pso_Cabo2022.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/pso_Seemann2009.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/pso_Seemann2009.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/randomSearch_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py` & `ionbench-0.4.1/ionbench/optimisers/external_optimisers/stochasticSearch_Vanier1999.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/pints_optimisers/cmaes_pints.py` & `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/cmaes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/pints_optimisers/nelderMead_pints.py` & `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/nelderMead_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/pints_optimisers/pso_pints.py` & `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/pso_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/pints_optimisers/snes_pints.py` & `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/snes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/pints_optimisers/xnes_pints.py` & `ionbench-0.4.1/ionbench/optimisers/pints_optimisers/xnes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py` & `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/conjugateGD_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/lm_scipy.py` & `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/lm_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py` & `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/nelderMead_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/powell_scipy.py` & `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/powell_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py` & `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/slsqp_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py` & `ionbench-0.4.1/ionbench/optimisers/scipy_optimisers/trustRegionReflective_scipy.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/problems/loewe2016.py` & `ionbench-0.4.1/ionbench/problems/loewe2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/problems/moreno2016.py` & `ionbench-0.4.1/ionbench/problems/moreno2016.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/problems/staircase.py` & `ionbench-0.4.1/ionbench/problems/staircase.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/problems/test.py` & `ionbench-0.4.1/ionbench/problems/test.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/tracker/tracker.py` & `ionbench-0.4.1/ionbench/tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/uncertainty/fim.py` & `ionbench-0.4.1/ionbench/uncertainty/fim.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/uncertainty/profile_likelihood.py` & `ionbench-0.4.1/ionbench/uncertainty/profile_likelihood.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/utils/autodiff.py` & `ionbench-0.4.1/ionbench/utils/autodiff.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/utils/cache.py` & `ionbench-0.4.1/ionbench/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/utils/classes_pints.py` & `ionbench-0.4.1/ionbench/utils/classes_pints.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/utils/multistart.py` & `ionbench-0.4.1/ionbench/utils/multistart.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/utils/particle_optimisers.py` & `ionbench-0.4.1/ionbench/utils/particle_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/utils/population_optimisers.py` & `ionbench-0.4.1/ionbench/utils/population_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench/utils/scipy_setup.py` & `ionbench-0.4.1/ionbench/utils/scipy_setup.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/ionbench.egg-info/PKG-INFO` & `ionbench-0.4.1/ionbench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ionbench
-Version: 0.4.0
+Version: 0.4.1
 Summary: A benchmarking tool for comparing different parameter optimization algorithms for ion channel models
 Home-page: https://github.com/CardiacModelling/ionbench
 Author: Matt J. Owen
 Author-email: matt.owen@nottingham.ac.uk
 Project-URL: Bug Reports, https://github.com/CardiacModelling/ionbench/issues
 Project-URL: Source, https://github.com/CardiacModelling/ionbench
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ionbench-0.4.0/ionbench.egg-info/SOURCES.txt` & `ionbench-0.4.1/ionbench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/setup.py` & `ionbench-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     name="ionbench",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.0",  # Required
+    version="0.4.1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A benchmarking tool for comparing different parameter optimization algorithms for ion channel models",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ionbench-0.4.0/test/test_modifications.py` & `ionbench-0.4.1/test/test_modifications.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/test/test_multistart.py` & `ionbench-0.4.1/test/test_multistart.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/test/test_optimisers.py` & `ionbench-0.4.1/test/test_optimisers.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/test/test_problems.py` & `ionbench-0.4.1/test/test_problems.py`

 * *Files identical despite different names*

### Comparing `ionbench-0.4.0/test/test_uncertainty.py` & `ionbench-0.4.1/test/test_uncertainty.py`

 * *Files identical despite different names*

