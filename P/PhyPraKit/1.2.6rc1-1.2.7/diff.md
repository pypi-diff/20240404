# Comparing `tmp/PhyPraKit-1.2.6rc1.tar.gz` & `tmp/PhyPraKit-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PhyPraKit-1.2.6rc1.tar", last modified: Wed Sep 13 12:15:34 2023, max compression
+gzip compressed data, was "PhyPraKit-1.2.7.tar", last modified: Thu Apr  4 12:51:20 2024, max compression
```

## Comparing `PhyPraKit-1.2.6rc1.tar` & `PhyPraKit-1.2.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-09-13 12:15:34.889423 PhyPraKit-1.2.6rc1/
--rw-r--r--   0 quast     (1000) users      (100)      194 2021-03-15 10:06:09.000000 PhyPraKit-1.2.6rc1/AUTHORS
--rw-r--r--   0 quast     (1000) users      (100)    35141 2020-10-27 14:31:54.000000 PhyPraKit-1.2.6rc1/LICENSE
--rw-r--r--   0 quast     (1000) users      (100)     2490 2023-09-13 12:15:34.889423 PhyPraKit-1.2.6rc1/PKG-INFO
-drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-09-13 12:15:34.881424 PhyPraKit-1.2.6rc1/PhyPraKit/
--rw-r--r--   0 quast     (1000) users      (100)      814 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/PhyPraKit/__init__.py
--rw-r--r--   0 quast     (1000) users      (100)      413 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/PhyPraKit/_version_info.py
--rwxr-xr-x   0 quast     (1000) users      (100)     2965 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/PhyPraKit/csv2yml.py
--rwxr-xr-x   0 quast     (1000) users      (100)   162304 2023-08-30 08:17:23.000000 PhyPraKit-1.2.6rc1/PhyPraKit/phyFit.py
--rw-r--r--   0 quast     (1000) users      (100)    84060 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/PhyPraKit/phyTools.py
--rwxr-xr-x   0 quast     (1000) users      (100)     3223 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/PhyPraKit/plotCSV.py
--rwxr-xr-x   0 quast     (1000) users      (100)     4921 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/PhyPraKit/plotData.py
--rwxr-xr-x   0 quast     (1000) users      (100)     9239 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/PhyPraKit/run_phyFit.py
--rwxr-xr-x   0 quast     (1000) users      (100)     4691 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/PhyPraKit/smoothCSV.py
-drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-09-13 12:15:34.881424 PhyPraKit-1.2.6rc1/PhyPraKit.egg-info/
--rw-r--r--   0 quast     (1000) users      (100)     2490 2023-09-13 12:15:34.000000 PhyPraKit-1.2.6rc1/PhyPraKit.egg-info/PKG-INFO
--rw-r--r--   0 quast     (1000) users      (100)      853 2023-09-13 12:15:34.000000 PhyPraKit-1.2.6rc1/PhyPraKit.egg-info/SOURCES.txt
--rw-r--r--   0 quast     (1000) users      (100)        1 2023-09-13 12:15:34.000000 PhyPraKit-1.2.6rc1/PhyPraKit.egg-info/dependency_links.txt
--rw-r--r--   0 quast     (1000) users      (100)       61 2023-09-13 12:15:34.000000 PhyPraKit-1.2.6rc1/PhyPraKit.egg-info/requires.txt
--rw-r--r--   0 quast     (1000) users      (100)       10 2023-09-13 12:15:34.000000 PhyPraKit-1.2.6rc1/PhyPraKit.egg-info/top_level.txt
--rw-r--r--   0 quast     (1000) users      (100)     1777 2022-12-21 15:18:59.000000 PhyPraKit-1.2.6rc1/README.md
--rw-r--r--   0 quast     (1000) users      (100)       38 2023-09-13 12:15:34.889423 PhyPraKit-1.2.6rc1/setup.cfg
--rw-r--r--   0 quast     (1000) users      (100)     1542 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/setup.py
-drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-09-13 12:15:34.885424 PhyPraKit-1.2.6rc1/tests/
--rwxrwxr-x   0 quast     (1000) users      (100)     3078 2021-02-12 22:53:00.000000 PhyPraKit-1.2.6rc1/tests/test.py
--rw-r--r--   0 quast     (1000) users      (100)      856 2020-03-23 23:18:35.000000 PhyPraKit-1.2.6rc1/tests/testAveCor_kafe1.py
--rw-r--r--   0 quast     (1000) users      (100)      582 2020-11-08 09:15:44.000000 PhyPraKit-1.2.6rc1/tests/testKafe2.py
--rwxr-xr-x   0 quast     (1000) users      (100)     5090 2021-03-13 10:07:42.000000 PhyPraKit-1.2.6rc1/tests/test_Diodenkennlinie.py
--rwxr-xr-x   0 quast     (1000) users      (100)     2312 2021-05-13 06:55:27.000000 PhyPraKit-1.2.6rc1/tests/test_histFit.py
--rwxr-xr-x   0 quast     (1000) users      (100)    18327 2021-01-09 14:30:46.000000 PhyPraKit-1.2.6rc1/tests/test_iminuit.py
--rwxr-xr-x   0 quast     (1000) users      (100)     1933 2020-12-31 16:54:50.000000 PhyPraKit-1.2.6rc1/tests/test_iminuit2.py
--rwxr-xr-x   0 quast     (1000) users      (100)     2431 2021-01-10 14:03:26.000000 PhyPraKit-1.2.6rc1/tests/test_iminuitFit.py
--rwxr-xr-x   0 quast     (1000) users      (100)     2293 2021-01-01 14:22:22.000000 PhyPraKit-1.2.6rc1/tests/test_iminuit_bak.py
--rwxr-xr-x   0 quast     (1000) users      (100)    17943 2021-01-06 08:34:04.000000 PhyPraKit-1.2.6rc1/tests/test_iminuit_old.py
--rw-r--r--   0 quast     (1000) users      (100)     3431 2022-05-22 14:30:52.000000 PhyPraKit-1.2.6rc1/tests/test_k2Fit_2.py
--rwxr-xr-x   0 quast     (1000) users      (100)     3220 2021-05-16 17:05:53.000000 PhyPraKit-1.2.6rc1/tests/test_k2_hFit.py
--rwxr--r--   0 quast     (1000) users      (100)     2880 2021-02-27 10:06:07.000000 PhyPraKit-1.2.6rc1/tests/test_kafe2.py
--rw-r--r--   0 quast     (1000) users      (100)     2367 2021-03-13 09:59:10.000000 PhyPraKit-1.2.6rc1/tests/test_mFit2.py
--rwxr-xr-x   0 quast     (1000) users      (100)     1449 2021-05-26 20:41:57.000000 PhyPraKit-1.2.6rc1/tests/test_mnFit.py
--rw-r--r--   0 quast     (1000) users      (100)     1159 2021-03-02 08:31:08.000000 PhyPraKit-1.2.6rc1/tests/test_simplemFit.py
-drwxr-xr-x   0 quast     (1000) users      (100)        0 2023-09-13 12:15:34.889423 PhyPraKit-1.2.6rc1/tools/
--rwxr-xr-x   0 quast     (1000) users      (100)      485 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/tools/csv2yml.py
--rwxr-xr-x   0 quast     (1000) users      (100)      533 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/tools/plotCSV.py
--rwxr-xr-x   0 quast     (1000) users      (100)     2003 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/tools/plotData.py
--rwxr-xr-x   0 quast     (1000) users      (100)     3050 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/tools/run_phyFit.py
--rwxr-xr-x   0 quast     (1000) users      (100)      620 2023-08-13 22:06:05.000000 PhyPraKit-1.2.6rc1/tools/smoothCSV.py
+drwxr-xr-x   0 quast     (1000) users      (100)        0 2024-04-04 12:51:20.310706 PhyPraKit-1.2.7/
+-rw-r--r--   0 quast     (1000) users      (100)      194 2021-03-15 10:06:09.000000 PhyPraKit-1.2.7/AUTHORS
+-rw-r--r--   0 quast     (1000) users      (100)    35141 2020-10-27 14:31:54.000000 PhyPraKit-1.2.7/LICENSE
+-rw-r--r--   0 quast     (1000) users      (100)     2487 2024-04-04 12:51:20.310706 PhyPraKit-1.2.7/PKG-INFO
+drwxr-xr-x   0 quast     (1000) users      (100)        0 2024-04-04 12:51:20.306706 PhyPraKit-1.2.7/PhyPraKit/
+-rw-r--r--   0 quast     (1000) users      (100)      811 2023-10-11 13:16:42.000000 PhyPraKit-1.2.7/PhyPraKit/__init__.py
+-rw-r--r--   0 quast     (1000) users      (100)      413 2024-04-04 12:47:22.000000 PhyPraKit-1.2.7/PhyPraKit/_version_info.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     2965 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/PhyPraKit/csv2yml.py
+-rwxr-xr-x   0 quast     (1000) users      (100)   162311 2023-12-19 16:25:36.000000 PhyPraKit-1.2.7/PhyPraKit/phyFit.py
+-rw-r--r--   0 quast     (1000) users      (100)    84060 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/PhyPraKit/phyTools.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     3223 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/PhyPraKit/plotCSV.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     4921 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/PhyPraKit/plotData.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     9239 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/PhyPraKit/run_phyFit.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     4691 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/PhyPraKit/smoothCSV.py
+drwxr-xr-x   0 quast     (1000) users      (100)        0 2024-04-04 12:51:20.306706 PhyPraKit-1.2.7/PhyPraKit.egg-info/
+-rw-r--r--   0 quast     (1000) users      (100)     2487 2024-04-04 12:51:20.000000 PhyPraKit-1.2.7/PhyPraKit.egg-info/PKG-INFO
+-rw-r--r--   0 quast     (1000) users      (100)      853 2024-04-04 12:51:20.000000 PhyPraKit-1.2.7/PhyPraKit.egg-info/SOURCES.txt
+-rw-r--r--   0 quast     (1000) users      (100)        1 2024-04-04 12:51:20.000000 PhyPraKit-1.2.7/PhyPraKit.egg-info/dependency_links.txt
+-rw-r--r--   0 quast     (1000) users      (100)       61 2024-04-04 12:51:20.000000 PhyPraKit-1.2.7/PhyPraKit.egg-info/requires.txt
+-rw-r--r--   0 quast     (1000) users      (100)       10 2024-04-04 12:51:20.000000 PhyPraKit-1.2.7/PhyPraKit.egg-info/top_level.txt
+-rw-r--r--   0 quast     (1000) users      (100)     1777 2022-12-21 15:18:59.000000 PhyPraKit-1.2.7/README.md
+-rw-r--r--   0 quast     (1000) users      (100)       38 2024-04-04 12:51:20.310706 PhyPraKit-1.2.7/setup.cfg
+-rw-r--r--   0 quast     (1000) users      (100)     1542 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/setup.py
+drwxr-xr-x   0 quast     (1000) users      (100)        0 2024-04-04 12:51:20.310706 PhyPraKit-1.2.7/tests/
+-rwxrwxr-x   0 quast     (1000) users      (100)     3078 2021-02-12 22:53:00.000000 PhyPraKit-1.2.7/tests/test.py
+-rw-r--r--   0 quast     (1000) users      (100)      856 2020-03-23 23:18:35.000000 PhyPraKit-1.2.7/tests/testAveCor_kafe1.py
+-rw-r--r--   0 quast     (1000) users      (100)      582 2020-11-08 09:15:44.000000 PhyPraKit-1.2.7/tests/testKafe2.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     5090 2021-03-13 10:07:42.000000 PhyPraKit-1.2.7/tests/test_Diodenkennlinie.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     2312 2021-05-13 06:55:27.000000 PhyPraKit-1.2.7/tests/test_histFit.py
+-rwxr-xr-x   0 quast     (1000) users      (100)    18327 2021-01-09 14:30:46.000000 PhyPraKit-1.2.7/tests/test_iminuit.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     1933 2020-12-31 16:54:50.000000 PhyPraKit-1.2.7/tests/test_iminuit2.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     2431 2021-01-10 14:03:26.000000 PhyPraKit-1.2.7/tests/test_iminuitFit.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     2293 2021-01-01 14:22:22.000000 PhyPraKit-1.2.7/tests/test_iminuit_bak.py
+-rwxr-xr-x   0 quast     (1000) users      (100)    17943 2021-01-06 08:34:04.000000 PhyPraKit-1.2.7/tests/test_iminuit_old.py
+-rw-r--r--   0 quast     (1000) users      (100)     3431 2022-05-22 14:30:52.000000 PhyPraKit-1.2.7/tests/test_k2Fit_2.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     3220 2021-05-16 17:05:53.000000 PhyPraKit-1.2.7/tests/test_k2_hFit.py
+-rwxr--r--   0 quast     (1000) users      (100)     2880 2021-02-27 10:06:07.000000 PhyPraKit-1.2.7/tests/test_kafe2.py
+-rw-r--r--   0 quast     (1000) users      (100)     2367 2021-03-13 09:59:10.000000 PhyPraKit-1.2.7/tests/test_mFit2.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     1449 2021-05-26 20:41:57.000000 PhyPraKit-1.2.7/tests/test_mnFit.py
+-rw-r--r--   0 quast     (1000) users      (100)     1159 2021-03-02 08:31:08.000000 PhyPraKit-1.2.7/tests/test_simplemFit.py
+drwxr-xr-x   0 quast     (1000) users      (100)        0 2024-04-04 12:51:20.310706 PhyPraKit-1.2.7/tools/
+-rwxr-xr-x   0 quast     (1000) users      (100)      485 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/tools/csv2yml.py
+-rwxr-xr-x   0 quast     (1000) users      (100)      533 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/tools/plotCSV.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     2003 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/tools/plotData.py
+-rwxr-xr-x   0 quast     (1000) users      (100)     3050 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/tools/run_phyFit.py
+-rwxr-xr-x   0 quast     (1000) users      (100)      620 2023-08-13 22:06:05.000000 PhyPraKit-1.2.7/tools/smoothCSV.py
```

### Comparing `PhyPraKit-1.2.6rc1/LICENSE` & `PhyPraKit-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/PKG-INFO` & `PhyPraKit-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PhyPraKit
-Version: 1.2.6rc1
+Version: 1.2.7
 Summary: Tools for data visualisation and analysis in Physics Lab Courses
 Home-page: http://www.etp.kit.edu/~quast/
 Author: Guenter Quast
 Author-email: Guenter.Quast@online.de
 License: GNU Public Licence
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit/__init__.py` & `PhyPraKit-1.2.7/PhyPraKit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 # Import version info
 from . import _version_info
 
 # Import main components
 from .phyTools import *
 from .phyFit import *
 
-_version_suffix = "rc1"  # for suffixes such as 'rc' or 'beta' or 'alpha'
+_version_suffix = ""  # for suffixes such as 'rc' or 'beta' or 'alpha'
 __version__ = _version_info._get_version_string()
 __version__ += _version_suffix
 
 __all__ = ["phyTools", "phyFit"]
```

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit/csv2yml.py` & `PhyPraKit-1.2.7/PhyPraKit/csv2yml.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit/phyFit.py` & `PhyPraKit-1.2.7/PhyPraKit/phyFit.py`

 * *Files 0% similar despite different names*

```diff
@@ -3171,6974 +3171,6975 @@
 0000c620: 206c 6f67 2d6c 696b 656c 6968 6f6f 6422   log-likelihood"
 0000c630: 2c0a 2020 2020 2020 2020 5d0a 0a20 2020  ,.        ]..   
 0000c640: 2020 2020 2073 656c 662e 6f70 7469 6f6e       self.option
 0000c650: 735b 2275 7365 5f47 6175 7373 4170 7072  s["use_GaussAppr
 0000c660: 6f78 225d 203d 205b 0a20 2020 2020 2020  ox"] = [.       
 0000c670: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
 0000c680: 2020 2020 2268 6973 7422 2c0a 2020 2020      "hist",.    
-0000c690: 2020 2020 2020 2020 2275 7369 6e67 2050          "using P
-0000c6a0: 6f69 7373 6f6e 206c 696b 656c 6968 6f6f  oisson likelihoo
-0000c6b0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-0000c6c0: 2275 7369 6e67 2047 6175 7373 6961 6e20  "using Gaussian 
-0000c6d0: 6170 7072 6f78 696d 6174 696f 6e20 6f66  approximation of
-0000c6e0: 2050 6f69 7373 6f6e 2064 6973 7469 6275   Poisson distibu
-0000c6f0: 7469 6f6e 222c 0a20 2020 2020 2020 205d  tion",.        ]
-0000c700: 0a20 2020 2020 2020 2073 656c 662e 6f70  .        self.op
-0000c710: 7469 6f6e 735b 2266 6974 5f64 656e 7369  tions["fit_densi
-0000c720: 7479 225d 203d 205b 0a20 2020 2020 2020  ty"] = [.       
-0000c730: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
-0000c740: 2020 2020 2268 6973 7422 2c0a 2020 2020      "hist",.    
-0000c750: 2020 2020 2020 2020 2266 6974 2066 6f72          "fit for
-0000c760: 206e 756d 6265 7220 6f66 2065 6e74 7269   number of entri
-0000c770: 6573 2f62 696e 222c 0a20 2020 2020 2020  es/bin",.       
-0000c780: 2020 2020 2022 6669 7420 6465 6e73 6974       "fit densit
-0000c790: 7920 6469 7374 7269 6275 7469 6f6e 222c  y distribution",
-0000c7a0: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-0000c7b0: 2020 2073 656c 662e 6f70 7469 6f6e 735b     self.options[
-0000c7c0: 226e 6567 326c 6f67 4c22 5d20 3d20 5b0a  "neg2logL"] = [.
-0000c7d0: 2020 2020 2020 2020 2020 2020 312c 0a20              1,. 
-0000c7e0: 2020 2020 2020 2020 2020 205b 2275 7365             ["use
-0000c7f0: 7222 2c20 226d 6c22 5d2c 0a20 2020 2020  r", "ml"],.     
-0000c800: 2020 2020 2020 2022 7573 696e 6720 7374         "using st
-0000c810: 616e 6461 7264 206c 696b 656c 6968 6f6f  andard likelihoo
-0000c820: 6420 2d3e 2065 7272 6465 6620 3d20 302e  d -> errdef = 0.
-0000c830: 3522 2c0a 2020 2020 2020 2020 2020 2020  5",.            
-0000c840: 2275 7369 6e67 202d 3220 2a20 6e65 672e  "using -2 * neg.
-0000c850: 206c 6f67 2e20 6c69 6b65 6c69 686f 6f64   log. likelihood
-0000c860: 202d 3e20 6572 7264 6566 3d31 2e22 2c0a   -> errdef=1.",.
-0000c870: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
-0000c880: 2020 2023 2073 6574 206f 7074 696f 6e73     # set options
-0000c890: 2066 6f72 2028 6e69 6365 7229 2070 6c6f   for (nicer) plo
-0000c8a0: 7474 696e 670a 2020 2020 2020 2020 7365  tting.        se
-0000c8b0: 6c66 2e73 6574 506c 6f74 4f70 7469 6f6e  lf.setPlotOption
-0000c8c0: 7328 290a 0a20 2020 2064 6566 2069 6e69  s()..    def ini
-0000c8d0: 745f 6461 7461 2873 656c 662c 202a 6172  t_data(self, *ar
-0000c8e0: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
-0000c8f0: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
-0000c900: 6974 5f74 7970 6520 3d3d 2022 7879 223a  it_type == "xy":
-0000c910: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000c920: 662e 696e 6974 5f78 7944 6174 6128 2a61  f.init_xyData(*a
-0000c930: 7267 732c 202a 2a6b 7761 7267 7329 0a20  rgs, **kwargs). 
-0000c940: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-0000c950: 2e66 6974 5f74 7970 6520 3d3d 2022 696e  .fit_type == "in
-0000c960: 6465 7865 6422 3a0a 2020 2020 2020 2020  dexed":.        
-0000c970: 2020 2020 7365 6c66 2e69 6e69 745f 7844      self.init_xD
-0000c980: 6174 6128 2a61 7267 732c 202a 2a6b 7761  ata(*args, **kwa
-0000c990: 7267 7329 0a20 2020 2020 2020 2065 6c69  rgs).        eli
-0000c9a0: 6620 7365 6c66 2e66 6974 5f74 7970 6520  f self.fit_type 
-0000c9b0: 3d3d 2022 6869 7374 223a 0a20 2020 2020  == "hist":.     
-0000c9c0: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
-0000c9d0: 5f68 4461 7461 282a 6172 6773 2c20 2a2a  _hData(*args, **
-0000c9e0: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-0000c9f0: 656c 6966 2073 656c 662e 6669 745f 7479  elif self.fit_ty
-0000ca00: 7065 203d 3d20 226d 6c22 3a0a 2020 2020  pe == "ml":.    
-0000ca10: 2020 2020 2020 2020 7365 6c66 2e69 6e69          self.ini
-0000ca20: 745f 6d6c 4461 7461 282a 6172 6773 2c20  t_mlData(*args, 
-0000ca30: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-0000ca40: 2020 656c 6966 2073 656c 662e 6669 745f    elif self.fit_
-0000ca50: 7479 7065 203d 3d20 2275 7365 7222 3a0a  type == "user":.
-0000ca60: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000ca70: 7428 2221 2a2a 2120 6d6e 4669 743a 206e  t("!**! mnFit: n
-0000ca80: 6f74 2064 6174 6120 6f62 6a65 6374 2074  ot data object t
-0000ca90: 6f20 6265 2064 6566 696e 6465 6420 666f  o be definded fo
-0000caa0: 7220 6669 745f 7479 7065 2027 7573 6572  r fit_type 'user
-0000cab0: 2722 290a 2020 2020 2020 2020 656c 7365  '").        else
-0000cac0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0000cad0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-0000cae0: 212a 2a21 2075 6e6b 6e6f 776e 2074 7970  !**! unknown typ
-0000caf0: 6520 6f66 2046 6974 2022 202b 2073 656c  e of Fit " + sel
-0000cb00: 662e 6669 745f 7479 7065 290a 0a20 2020  f.fit_type)..   
-0000cb10: 2064 6566 2073 6574 4f70 7469 6f6e 7328   def setOptions(
-0000cb20: 7365 6c66 2c20 2a61 7267 732c 202a 2a6b  self, *args, **k
-0000cb30: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-0000cb40: 6966 2073 656c 662e 6669 745f 7479 7065  if self.fit_type
-0000cb50: 203d 3d20 2278 7922 3a0a 2020 2020 2020   == "xy":.      
-0000cb60: 2020 2020 2020 7365 6c66 2e73 6574 5f78        self.set_x
-0000cb70: 794f 7074 696f 6e73 282a 6172 6773 2c20  yOptions(*args, 
-0000cb80: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-0000cb90: 2020 656c 6966 2073 656c 662e 6669 745f    elif self.fit_
-0000cba0: 7479 7065 203d 3d20 2269 6e64 6578 6564  type == "indexed
-0000cbb0: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
-0000cbc0: 656c 662e 7365 745f 784f 7074 696f 6e73  elf.set_xOptions
-0000cbd0: 282a 6172 6773 2c20 2a2a 6b77 6172 6773  (*args, **kwargs
-0000cbe0: 290a 2020 2020 2020 2020 656c 6966 2073  ).        elif s
-0000cbf0: 656c 662e 6669 745f 7479 7065 203d 3d20  elf.fit_type == 
-0000cc00: 2268 6973 7422 3a0a 2020 2020 2020 2020  "hist":.        
-0000cc10: 2020 2020 7365 6c66 2e73 6574 5f68 4f70      self.set_hOp
-0000cc20: 7469 6f6e 7328 2a61 7267 732c 202a 2a6b  tions(*args, **k
-0000cc30: 7761 7267 7329 0a20 2020 2020 2020 2065  wargs).        e
-0000cc40: 6c69 6620 7365 6c66 2e66 6974 5f74 7970  lif self.fit_typ
-0000cc50: 6520 3d3d 2022 7573 6572 2220 6f72 2073  e == "user" or s
-0000cc60: 656c 662e 6669 745f 7479 7065 203d 3d20  elf.fit_type == 
-0000cc70: 226d 6c22 3a0a 2020 2020 2020 2020 2020  "ml":.          
-0000cc80: 2020 7365 6c66 2e73 6574 5f6d 6e4f 7074    self.set_mnOpt
-0000cc90: 696f 6e73 282a 6172 6773 2c20 2a2a 6b77  ions(*args, **kw
-0000cca0: 6172 6773 290a 2020 2020 2020 2020 656c  args).        el
-0000ccb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000ccc0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-0000ccd0: 2822 212a 2a21 2075 6e6b 6e6f 776e 2074  ("!**! unknown t
-0000cce0: 7970 6520 6f66 2046 6974 2022 202b 2073  ype of Fit " + s
-0000ccf0: 656c 662e 6669 745f 7479 7065 290a 0a20  elf.fit_type).. 
-0000cd00: 2020 2064 6566 2069 6e69 745f 6669 7428     def init_fit(
-0000cd10: 7365 6c66 2c20 2a61 7267 732c 202a 2a6b  self, *args, **k
-0000cd20: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-0000cd30: 6966 2073 656c 662e 6669 745f 7479 7065  if self.fit_type
-0000cd40: 203d 3d20 2278 7922 3a0a 2020 2020 2020   == "xy":.      
-0000cd50: 2020 2020 2020 7365 6c66 2e69 6e69 745f        self.init_
-0000cd60: 7879 4669 7428 2a61 7267 732c 202a 2a6b  xyFit(*args, **k
-0000cd70: 7761 7267 7329 0a20 2020 2020 2020 2065  wargs).        e
-0000cd80: 6c69 6620 7365 6c66 2e66 6974 5f74 7970  lif self.fit_typ
-0000cd90: 6520 3d3d 2022 696e 6465 7865 6422 3a0a  e == "indexed":.
-0000cda0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000cdb0: 2e69 6e69 745f 7846 6974 282a 6172 6773  .init_xFit(*args
-0000cdc0: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
-0000cdd0: 2020 2020 656c 6966 2073 656c 662e 6669      elif self.fi
-0000cde0: 745f 7479 7065 203d 3d20 2268 6973 7422  t_type == "hist"
-0000cdf0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000ce00: 6c66 2e69 6e69 745f 6846 6974 282a 6172  lf.init_hFit(*ar
-0000ce10: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
-0000ce20: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
-0000ce30: 6669 745f 7479 7065 203d 3d20 2275 7365  fit_type == "use
-0000ce40: 7222 206f 7220 7365 6c66 2e66 6974 5f74  r" or self.fit_t
-0000ce50: 7970 6520 3d3d 2022 6d6c 223a 0a20 2020  ype == "ml":.   
-0000ce60: 2020 2020 2020 2020 2073 656c 662e 696e           self.in
-0000ce70: 6974 5f6d 6e46 6974 282a 6172 6773 2c20  it_mnFit(*args, 
-0000ce80: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
-0000ce90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000cea0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000ceb0: 7272 6f72 2822 212a 2a21 2075 6e6b 6e6f  rror("!**! unkno
-0000cec0: 776e 2074 7970 6520 6f66 2046 6974 2022  wn type of Fit "
-0000ced0: 202b 2073 656c 662e 6669 745f 7479 7065   + self.fit_type
-0000cee0: 290a 0a20 2020 2023 0a20 2020 2023 202d  )..    #.    # -
-0000cef0: 2d2d 2073 7065 6369 616c 2063 6f64 6520  -- special code 
-0000cf00: 666f 7220 7879 2046 6974 0a20 2020 2023  for xy Fit.    #
-0000cf10: 0a0a 2020 2020 6465 6620 7365 745f 7879  ..    def set_xy
-0000cf20: 4f70 7469 6f6e 7328 0a20 2020 2020 2020  Options(.       
-0000cf30: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-0000cf40: 656c 6174 6976 655f 7265 6665 7273 5f74  elative_refers_t
-0000cf50: 6f5f 6d6f 6465 6c3d 4e6f 6e65 2c0a 2020  o_model=None,.  
-0000cf60: 2020 2020 2020 7275 6e5f 6d69 6e6f 733d        run_minos=
-0000cf70: 4e6f 6e65 2c0a 2020 2020 2020 2020 7573  None,.        us
-0000cf80: 655f 6e65 674c 6f67 4c3d 4e6f 6e65 2c0a  e_negLogL=None,.
-0000cf90: 2020 2020 2020 2020 7175 6965 743d 4e6f          quiet=No
-0000cfa0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0000cfb0: 2020 2022 2222 4465 6669 6e65 206f 7074     """Define opt
-0000cfc0: 696f 6e73 2066 6f72 2078 7920 6669 740a  ions for xy fit.
-0000cfd0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000cfe0: 2020 2020 2020 2020 2d20 7265 6c2e 2065          - rel. e
-0000cff0: 7272 6f72 7320 7265 6665 7220 746f 206d  rrors refer to m
-0000d000: 6f64 656c 2065 6c73 6520 6461 7461 0a20  odel else data. 
-0000d010: 2020 2020 2020 2020 2d20 7275 6e20 6d69          - run mi
-0000d020: 6e6f 7320 656c 7365 2064 6f6e 2a74 2072  nos else don*t r
-0000d030: 756e 206d 696e 6f73 0a20 2020 2020 2020  un minos.       
-0000d040: 2020 2d20 7573 6520 6675 6c6c 206e 6567    - use full neg
-0000d050: 326c 6f67 4c0a 2020 2020 2020 2020 202d  2logL.         -
-0000d060: 2064 6f6e 2a74 2070 726f 7669 6465 2070   don*t provide p
-0000d070: 7269 6e74 6f75 7420 656c 7365 2076 6572  rintout else ver
-0000d080: 626f 7365 2070 7269 6e74 6f75 740a 2020  bose printout.  
-0000d090: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000d0a0: 2020 6966 2072 656c 6174 6976 655f 7265    if relative_re
-0000d0b0: 6665 7273 5f74 6f5f 6d6f 6465 6c20 6973  fers_to_model is
-0000d0c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000d0d0: 2020 2020 2020 2073 656c 662e 7265 664d         self.refM
-0000d0e0: 6f64 656c 203d 2072 656c 6174 6976 655f  odel = relative_
-0000d0f0: 7265 6665 7273 5f74 6f5f 6d6f 6465 6c0a  refers_to_model.
-0000d100: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d110: 2e6f 7074 696f 6e73 5b22 7265 664d 6f64  .options["refMod
-0000d120: 656c 225d 5b30 5d20 3d20 696e 7428 7265  el"][0] = int(re
-0000d130: 6c61 7469 7665 5f72 6566 6572 735f 746f  lative_refers_to
-0000d140: 5f6d 6f64 656c 290a 2020 2020 2020 2020  _model).        
-0000d150: 6966 2072 756e 5f6d 696e 6f73 2069 7320  if run_minos is 
-0000d160: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0000d170: 2020 2020 2020 7365 6c66 2e72 756e 5f6d        self.run_m
-0000d180: 696e 6f73 203d 2072 756e 5f6d 696e 6f73  inos = run_minos
-0000d190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000d1a0: 662e 6f70 7469 6f6e 735b 2272 756e 5f6d  f.options["run_m
-0000d1b0: 696e 6f73 225d 5b30 5d20 3d20 696e 7428  inos"][0] = int(
-0000d1c0: 7275 6e5f 6d69 6e6f 7329 0a20 2020 2020  run_minos).     
-0000d1d0: 2020 2069 6620 7573 655f 6e65 674c 6f67     if use_negLog
-0000d1e0: 4c20 6973 206e 6f74 204e 6f6e 653a 0a20  L is not None:. 
-0000d1f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000d200: 7573 655f 6e65 674c 6f67 4c20 3d20 7573  use_negLogL = us
-0000d210: 655f 6e65 674c 6f67 4c0a 2020 2020 2020  e_negLogL.      
-0000d220: 2020 2020 2020 7365 6c66 2e6f 7074 696f        self.optio
-0000d230: 6e73 5b22 7573 655f 6e65 674c 6f67 4c22  ns["use_negLogL"
-0000d240: 5d5b 305d 203d 2069 6e74 2875 7365 5f6e  ][0] = int(use_n
-0000d250: 6567 4c6f 674c 290a 2020 2020 2020 2020  egLogL).        
-0000d260: 6966 2071 7569 6574 2069 7320 6e6f 7420  if quiet is not 
-0000d270: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000d280: 2020 7365 6c66 2e71 7569 6574 203d 2071    self.quiet = q
-0000d290: 7569 6574 0a0a 2020 2020 6465 6620 696e  uiet..    def in
-0000d2a0: 6974 5f78 7944 6174 6128 0a20 2020 2020  it_xyData(.     
-0000d2b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000d2c0: 2078 2c0a 2020 2020 2020 2020 792c 0a20   x,.        y,. 
-0000d2d0: 2020 2020 2020 2065 783d 4e6f 6e65 2c0a         ex=None,.
-0000d2e0: 2020 2020 2020 2020 6579 3d31 2e30 2c0a          ey=1.0,.
-0000d2f0: 2020 2020 2020 2020 6572 656c 783d 4e6f          erelx=No
-0000d300: 6e65 2c0a 2020 2020 2020 2020 6572 656c  ne,.        erel
-0000d310: 793d 4e6f 6e65 2c0a 2020 2020 2020 2020  y=None,.        
-0000d320: 6361 6273 783d 4e6f 6e65 2c0a 2020 2020  cabsx=None,.    
-0000d330: 2020 2020 6372 656c 783d 4e6f 6e65 2c0a      crelx=None,.
-0000d340: 2020 2020 2020 2020 6361 6273 793d 4e6f          cabsy=No
-0000d350: 6e65 2c0a 2020 2020 2020 2020 6372 656c  ne,.        crel
-0000d360: 793d 4e6f 6e65 2c0a 2020 2020 293a 0a20  y=None,.    ):. 
-0000d370: 2020 2020 2020 2022 2222 696e 6974 6961         """initia
-0000d380: 6c69 7a65 2064 6174 6120 6f62 6a65 6374  lize data object
-0000d390: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000d3a0: 2020 2020 2020 2020 2020 2d20 2078 3a20            -  x: 
-0000d3b0: 2020 2020 2020 6162 7363 6973 7361 206f        abscissa o
-0000d3c0: 6620 6461 7461 2070 6f69 6e74 7320 2822  f data points ("
-0000d3d0: 7820 7661 6c75 6573 2229 0a20 2020 2020  x values").     
-0000d3e0: 2020 2020 202d 2020 793a 2020 2020 2020       -  y:      
-0000d3f0: 206f 7264 696e 6174 6520 6f66 2064 6174   ordinate of dat
-0000d400: 6120 706f 696e 7473 2028 2279 2076 616c  a points ("y val
-0000d410: 7565 7322 290a 2020 2020 2020 2020 2020  ues").          
-0000d420: 2d20 2065 783a 2020 2020 2020 696e 6465  -  ex:      inde
-0000d430: 7065 6e64 656e 7420 756e 6365 7274 6169  pendent uncertai
-0000d440: 6e74 6965 7320 780a 2020 2020 2020 2020  nties x.        
-0000d450: 2020 2d20 2065 793a 2020 2020 2020 696e    -  ey:      in
-0000d460: 6465 7065 6e64 656e 7420 756e 6365 7274  dependent uncert
-0000d470: 6169 6e74 6965 7320 790a 2020 2020 2020  ainties y.      
-0000d480: 2020 2020 2d20 2065 7265 6c78 3a20 2020      -  erelx:   
-0000d490: 696e 6465 7065 6e64 656e 7420 7265 6c61  independent rela
-0000d4a0: 7469 7665 2075 6e63 6572 7461 696e 7469  tive uncertainti
-0000d4b0: 6573 2078 0a20 2020 2020 2020 2020 202d  es x.          -
-0000d4c0: 2020 6572 656c 793a 2020 2069 6e64 6570    erely:   indep
-0000d4d0: 656e 6465 6e74 2072 656c 6174 6976 6520  endent relative 
-0000d4e0: 756e 6365 7274 6169 6e74 6965 7320 790a  uncertainties y.
-0000d4f0: 2020 2020 2020 2020 2020 2d20 2063 6162            -  cab
-0000d500: 7378 3a20 2020 636f 7272 656c 6174 6564  sx:   correlated
-0000d510: 2061 626f 6c75 7465 2075 6e63 6572 7461   abolute uncerta
-0000d520: 696e 7469 6573 2078 0a20 2020 2020 2020  inties x.       
-0000d530: 2020 202d 2020 6372 656c 783a 2020 2063     -  crelx:   c
-0000d540: 6f72 7265 6c61 7465 6420 7265 6c61 7469  orrelated relati
-0000d550: 7665 2075 6e63 6572 7461 696e 7469 6573  ve uncertainties
-0000d560: 2078 0a20 2020 2020 2020 2020 202d 2020   x.          -  
-0000d570: 6361 6273 793a 2020 2063 6f72 7265 6c61  cabsy:   correla
-0000d580: 7465 6420 6162 736f 6c75 7465 2075 6e63  ted absolute unc
-0000d590: 6572 7461 696e 7469 6573 2079 0a20 2020  ertainties y.   
-0000d5a0: 2020 2020 2020 202d 2020 6372 656c 793a         -  crely:
-0000d5b0: 2020 2063 6f72 7265 6c61 7465 6420 7265     correlated re
-0000d5c0: 6c61 7469 7665 2075 6e63 6572 7461 696e  lative uncertain
-0000d5d0: 7469 6573 2079 0a20 2020 2020 2020 2020  ties y.         
-0000d5e0: 202d 2020 7175 6965 743a 2020 206e 6f20   -  quiet:   no 
-0000d5f0: 696e 666f 726d 6174 6976 6520 7072 696e  informative prin
-0000d600: 746f 7574 2069 6620 5472 7565 0a20 2020  tout if True.   
-0000d610: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000d620: 2020 2320 6372 6561 7465 2064 6174 6120    # create data 
-0000d630: 6f62 6a65 6374 2061 6e64 2070 6173 7320  object and pass 
-0000d640: 616c 6c20 696e 7075 7420 6172 6775 6d65  all input argume
-0000d650: 6e74 730a 2020 2020 2020 2020 7365 6c66  nts.        self
-0000d660: 2e78 7944 6174 6120 3d20 7365 6c66 2e78  .xyData = self.x
-0000d670: 7944 6174 6143 6f6e 7461 696e 6572 280a  yDataContainer(.
-0000d680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000d690: 2c0a 2020 2020 2020 2020 2020 2020 782c  ,.            x,
-0000d6a0: 0a20 2020 2020 2020 2020 2020 2079 2c0a  .            y,.
-0000d6b0: 2020 2020 2020 2020 2020 2020 6578 2c0a              ex,.
-0000d6c0: 2020 2020 2020 2020 2020 2020 6579 2c0a              ey,.
-0000d6d0: 2020 2020 2020 2020 2020 2020 6572 656c              erel
-0000d6e0: 782c 0a20 2020 2020 2020 2020 2020 2065  x,.            e
-0000d6f0: 7265 6c79 2c0a 2020 2020 2020 2020 2020  rely,.          
-0000d700: 2020 6361 6273 782c 0a20 2020 2020 2020    cabsx,.       
-0000d710: 2020 2020 2063 7265 6c78 2c0a 2020 2020       crelx,.    
-0000d720: 2020 2020 2020 2020 6361 6273 792c 0a20          cabsy,. 
-0000d730: 2020 2020 2020 2020 2020 2063 7265 6c79             crely
-0000d740: 2c0a 2020 2020 2020 2020 2020 2020 7175  ,.            qu
-0000d750: 6965 743d 7365 6c66 2e71 7569 6574 2c0a  iet=self.quiet,.
-0000d760: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d770: 2020 7365 6c66 2e64 6174 6120 3d20 7365    self.data = se
-0000d780: 6c66 2e78 7944 6174 610a 2020 2020 2020  lf.xyData.      
-0000d790: 2020 2320 7365 7420 666c 6167 7320 666f    # set flags fo
-0000d7a0: 7220 7374 6565 7269 6e67 206f 6620 6669  r steering of fi
-0000d7b0: 7420 7072 6f63 6573 7320 696e 2064 6f5f  t process in do_
-0000d7c0: 6669 7428 290a 2020 2020 2020 2020 7365  fit().        se
-0000d7d0: 6c66 2e69 7465 7261 7465 4669 7420 3d20  lf.iterateFit = 
-0000d7e0: 7365 6c66 2e78 7944 6174 612e 6861 735f  self.xyData.has_
-0000d7f0: 7845 7272 6f72 7320 6f72 2028 0a20 2020  xErrors or (.   
-0000d800: 2020 2020 2020 2020 2073 656c 662e 7879           self.xy
-0000d810: 4461 7461 2e68 6173 5f72 656c 5f79 4572  Data.has_rel_yEr
-0000d820: 726f 7273 2061 6e64 2073 656c 662e 7265  rors and self.re
-0000d830: 664d 6f64 656c 0a20 2020 2020 2020 2029  fModel.        )
-0000d840: 0a0a 2020 2020 6465 6620 696e 6974 5f78  ..    def init_x
-0000d850: 7946 6974 280a 2020 2020 2020 2020 7365  yFit(.        se
-0000d860: 6c66 2c0a 2020 2020 2020 2020 6d6f 6465  lf,.        mode
-0000d870: 6c2c 0a20 2020 2020 2020 206d 6f64 656c  l,.        model
-0000d880: 5f6b 7761 7267 733d 4e6f 6e65 2c0a 2020  _kwargs=None,.  
-0000d890: 2020 2020 2020 7030 3d4e 6f6e 652c 0a20        p0=None,. 
-0000d8a0: 2020 2020 2020 2064 7030 3d4e 6f6e 652c         dp0=None,
-0000d8b0: 0a20 2020 2020 2020 2063 6f6e 7374 7261  .        constra
-0000d8c0: 696e 7473 3d4e 6f6e 652c 0a20 2020 2020  ints=None,.     
-0000d8d0: 2020 2066 6978 5061 7273 3d4e 6f6e 652c     fixPars=None,
-0000d8e0: 0a20 2020 2020 2020 206c 696d 6974 733d  .        limits=
-0000d8f0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0000d900: 2020 2020 2022 2222 696e 6974 6961 6c69       """initiali
-0000d910: 7a65 2066 6974 206f 626a 6563 740a 0a20  ze fit object.. 
-0000d920: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000d930: 2020 2020 2020 202d 206d 6f64 656c 3a20         - model: 
-0000d940: 6d6f 6465 6c20 6675 6e63 7469 6f6e 2066  model function f
-0000d950: 2878 3b20 5c2a 7061 7229 0a20 2020 2020  (x; \*par).     
-0000d960: 2020 2020 202d 206d 6f64 656c 5f6b 7761       - model_kwa
-0000d970: 7267 733a 206f 7074 696f 6e61 6c2c 2066  rgs: optional, f
-0000d980: 6974 2070 6172 616d 6574 6572 7320 6966  it parameters if
-0000d990: 206e 6f74 2066 726f 6d20 6d6f 6465 6c20   not from model 
-0000d9a0: 7369 676e 6174 7572 650a 2020 2020 2020  signature.      
-0000d9b0: 2020 2020 2d20 7030 3a20 6e70 2d61 7272      - p0: np-arr
-0000d9c0: 6179 206f 6620 666c 6f61 7473 2c20 696e  ay of floats, in
-0000d9d0: 6974 6961 6c20 7061 7261 6d65 7465 7220  itial parameter 
-0000d9e0: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
-0000d9f0: 202d 2064 7030 3a20 6172 7261 792d 6c69   - dp0: array-li
-0000da00: 6b65 2c20 696e 6974 6961 6c20 6775 6573  ke, initial gues
-0000da10: 7320 6f66 2070 6172 616d 6574 6572 2075  s of parameter u
-0000da20: 6e63 6572 7461 696e 7469 6573 2028 6f70  ncertainties (op
-0000da30: 7469 6f6e 616c 290a 2020 2020 2020 2020  tional).        
-0000da40: 2020 2d20 636f 6e73 7472 6169 6e74 733a    - constraints:
-0000da50: 2028 6e65 7374 6564 2920 6c69 7374 2873   (nested) list(s
-0000da60: 293a 205b 7061 7261 6d65 7465 7220 6e61  ): [parameter na
-0000da70: 6d65 2c20 7661 6c75 652c 2075 6e63 6572  me, value, uncer
-0000da80: 7461 696e 7479 5d0a 2020 2020 2020 2020  tainty].        
-0000da90: 2020 2020 6f72 205b 7061 7261 6d65 7465      or [paramete
-0000daa0: 7220 696e 6465 782c 2076 616c 7565 2c20  r index, value, 
-0000dab0: 756e 6365 7274 6169 6e74 795d 0a20 2020  uncertainty].   
-0000dac0: 2020 2020 2020 202d 206c 696d 6974 733a         - limits:
-0000dad0: 2028 6e65 7374 6564 2920 6c69 7374 2873   (nested) list(s
-0000dae0: 293a 205b 7061 7261 6d65 7465 7220 6e61  ): [parameter na
-0000daf0: 6d65 2c20 6d69 6e2c 206d 6178 5d0a 2020  me, min, max].  
-0000db00: 2020 2020 2020 2020 2020 6f72 205b 7061            or [pa
-0000db10: 7261 6d65 7465 7220 696e 6465 782c 206d  rameter index, m
-0000db20: 696e 2c20 6d61 785d 0a20 2020 2020 2020  in, max].       
-0000db30: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
-0000db40: 2073 656c 662e 7879 4461 7461 2069 7320   self.xyData is 
-0000db50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000db60: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-0000db70: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-0000db80: 2020 2020 2220 2121 2120 6d6e 4669 742e      " !!! mnFit.
-0000db90: 696e 6974 5f78 7946 6974 3a20 6e6f 2064  init_xyFit: no d
-0000dba0: 6174 6120 6f62 6a65 6374 2064 6566 696e  ata object defin
-0000dbb0: 6564 202d 2063 616c 6c20 696e 6974 5f64  ed - call init_d
-0000dbc0: 6174 6128 2922 0a20 2020 2020 2020 2020  ata()".         
-0000dbd0: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-0000dbe0: 6765 7420 7061 7261 6d65 7465 7273 206f  get parameters o
-0000dbf0: 6620 6d6f 6465 6c20 6675 6e63 7469 6f6e  f model function
-0000dc00: 2074 6f20 7365 7420 7374 6172 7420 7661   to set start va
-0000dc10: 6c75 6573 2066 6f72 2066 6974 0a20 2020  lues for fit.   
-0000dc20: 2020 2020 2069 6620 6d6f 6465 6c5f 6b77       if model_kw
-0000dc30: 6172 6773 2069 7320 4e6f 6e65 3a0a 2020  args is None:.  
-0000dc40: 2020 2020 2020 2020 2020 6172 6773 2c20            args, 
-0000dc50: 6d6f 6465 6c5f 6b77 6172 6773 203d 2067  model_kwargs = g
-0000dc60: 6574 5f66 756e 6374 696f 6e53 6967 6e61  et_functionSigna
-0000dc70: 7475 7265 286d 6f64 656c 290a 0a20 2020  ture(model)..   
-0000dc80: 2020 2020 2070 6172 203d 2028 6d6f 6465       par = (mode
-0000dc90: 6c5f 6b77 6172 6773 2c20 7030 2c20 6470  l_kwargs, p0, dp
-0000dca0: 302c 2063 6f6e 7374 7261 696e 7473 2c20  0, constraints, 
-0000dcb0: 6669 7850 6172 732c 206c 696d 6974 7329  fixPars, limits)
-0000dcc0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-0000dcd0: 6574 7570 4669 7450 6172 616d 6574 6572  etupFitParameter
-0000dce0: 7328 2a70 6172 290a 0a20 2020 2020 2020  s(*par)..       
-0000dcf0: 2023 2063 7265 6174 6520 636f 7374 2066   # create cost f
-0000dd00: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
-0000dd10: 7365 6c66 2e63 6f73 7466 203d 2073 656c  self.costf = sel
-0000dd20: 662e 784c 5371 436f 7374 2873 656c 662c  f.xLSqCost(self,
-0000dd30: 206d 6f64 656c 2c20 7573 655f 6e65 6732   model, use_neg2
-0000dd40: 6c6f 674c 3d73 656c 662e 7573 655f 6e65  logL=self.use_ne
-0000dd50: 674c 6f67 4c29 0a20 2020 2020 2020 2073  gLogL).        s
-0000dd60: 656c 662e 5f73 6574 7570 4d69 6e75 6974  elf._setupMinuit
-0000dd70: 286d 6f64 656c 5f6b 7761 7267 7329 0a0a  (model_kwargs)..
-0000dd80: 2020 2020 636c 6173 7320 7879 4461 7461      class xyData
-0000dd90: 436f 6e74 6169 6e65 723a 0a20 2020 2020  Container:.     
-0000dda0: 2020 2022 2222 0a20 2020 2020 2020 2048     """.        H
-0000ddb0: 616e 646c 6520 6461 7461 2061 6e64 2075  andle data and u
-0000ddc0: 6e63 6572 7461 696e 7469 6573 2061 6e64  ncertainties and
-0000ddd0: 0a20 2020 2020 2020 2062 7569 6c64 2063  .        build c
-0000dde0: 6f76 6172 6961 6e63 6520 6d61 7472 6963  ovariance matric
-0000ddf0: 6573 2066 726f 6d20 636f 6d70 6f6e 656e  es from componen
-0000de00: 7473 0a0a 2020 2020 2020 2020 4172 6773  ts..        Args
-0000de10: 3a0a 2020 2020 2020 2020 2020 2d20 6f75  :.          - ou
-0000de20: 7465 723a 2020 2070 6f69 6e74 6572 2074  ter:   pointer t
-0000de30: 6f20 696e 7374 616e 6365 206f 6620 6361  o instance of ca
-0000de40: 6c6c 696e 6720 6f62 6a65 6374 0a20 2020  lling object.   
-0000de50: 2020 2020 2020 202d 2078 3a20 2020 2020         - x:     
-0000de60: 2020 6162 7363 6973 7361 206f 6620 6461    abscissa of da
-0000de70: 7461 2070 6f69 6e74 7320 2822 7820 7661  ta points ("x va
-0000de80: 6c75 6573 2229 0a20 2020 2020 2020 2020  lues").         
-0000de90: 202d 2079 3a20 2020 2020 2020 6f72 6469   - y:       ordi
-0000dea0: 6e61 7465 206f 6620 6461 7461 2070 6f69  nate of data poi
-0000deb0: 6e74 7320 2822 7920 7661 6c75 6573 2229  nts ("y values")
-0000dec0: 0a20 2020 2020 2020 2020 202d 2065 783a  .          - ex:
-0000ded0: 2020 2020 2020 696e 6465 7065 6e64 656e        independen
-0000dee0: 7420 756e 6365 7274 6169 6e74 6965 7320  t uncertainties 
-0000def0: 780a 2020 2020 2020 2020 2020 2d20 6579  x.          - ey
-0000df00: 3a20 2020 2020 2069 6e64 6570 656e 6465  :      independe
-0000df10: 6e74 2075 6e63 6572 7461 696e 7469 6573  nt uncertainties
-0000df20: 2079 0a20 2020 2020 2020 2020 202d 2065   y.          - e
-0000df30: 7265 6c78 3a20 2020 696e 6465 7065 6e64  relx:   independ
-0000df40: 656e 7420 7265 6c61 7469 7665 2075 6e63  ent relative unc
-0000df50: 6572 7461 696e 7469 6573 2078 0a20 2020  ertainties x.   
-0000df60: 2020 2020 2020 202d 2065 7265 6c79 3a20         - erely: 
-0000df70: 2020 696e 6465 7065 6e64 656e 7420 7265    independent re
-0000df80: 6c61 7469 7665 2075 6e63 6572 7461 696e  lative uncertain
-0000df90: 7469 6573 2079 0a20 2020 2020 2020 2020  ties y.         
-0000dfa0: 202d 2063 6162 7378 3a20 2020 636f 7272   - cabsx:   corr
-0000dfb0: 656c 6174 6564 2061 626f 6c75 7465 2075  elated abolute u
-0000dfc0: 6e63 6572 7461 696e 7469 6573 2078 0a20  ncertainties x. 
-0000dfd0: 2020 2020 2020 2020 202d 2063 7265 6c78           - crelx
-0000dfe0: 3a20 2020 636f 7272 656c 6174 6564 2072  :   correlated r
-0000dff0: 656c 6174 6976 6520 756e 6365 7274 6169  elative uncertai
-0000e000: 6e74 6965 7320 780a 2020 2020 2020 2020  nties x.        
-0000e010: 2020 2d20 6361 6273 793a 2020 2063 6f72    - cabsy:   cor
-0000e020: 7265 6c61 7465 6420 6162 736f 6c75 7465  related absolute
-0000e030: 2075 6e63 6572 7461 696e 7469 6573 2079   uncertainties y
-0000e040: 0a20 2020 2020 2020 2020 202d 2063 7265  .          - cre
-0000e050: 6c79 3a20 2020 636f 7272 656c 6174 6564  ly:   correlated
-0000e060: 2072 656c 6174 6976 6520 756e 6365 7274   relative uncert
-0000e070: 6169 6e74 6965 7320 790a 2020 2020 2020  ainties y.      
-0000e080: 2020 2020 2d20 7175 6965 743a 2020 206e      - quiet:   n
-0000e090: 6f20 696e 666f 726d 6174 6976 6520 7072  o informative pr
-0000e0a0: 696e 746f 7574 2069 6620 5472 7565 0a0a  intout if True..
-0000e0b0: 2020 2020 2020 2020 5075 626c 6963 206d          Public m
-0000e0c0: 6574 686f 6473 3a0a 2020 2020 2020 2020  ethods:.        
-0000e0d0: 2020 2d20 696e 6974 5f64 796e 616d 6963    - init_dynamic
-0000e0e0: 4572 726f 7273 2829 3a0a 2020 2020 2020  Errors():.      
-0000e0f0: 2020 2020 2d20 6765 745f 436f 7628 293a      - get_Cov():
-0000e100: 2066 696e 616c 2063 6f76 6172 6961 6e63   final covarianc
-0000e110: 6520 6d61 7472 6978 2028 696e 636c 2e20  e matrix (incl. 
-0000e120: 7072 6f6a 2e20 7829 0a20 2020 2020 2020  proj. x).       
-0000e130: 2020 202d 2067 6574 5f78 436f 7628 293a     - get_xCov():
-0000e140: 2063 6f76 6172 6961 6e63 6520 6f66 2078   covariance of x
-0000e150: 2d76 616c 7565 730a 2020 2020 2020 2020  -values.        
-0000e160: 2020 2d20 6765 745f 7943 6f76 2829 3a20    - get_yCov(): 
-0000e170: 636f 7661 7269 616e 6365 206f 6620 792d  covariance of y-
-0000e180: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
-0000e190: 202d 2067 6574 5f69 436f 7628 293a 2069   - get_iCov(): i
-0000e1a0: 6e76 6572 7365 2063 6f76 6172 6961 6e63  nverse covarianc
-0000e1b0: 6520 6d61 7472 6978 0a20 2020 2020 2020  e matrix.       
-0000e1c0: 2020 202d 2070 6c6f 7428 293a 2070 726f     - plot(): pro
-0000e1d0: 7669 6465 2061 2066 6967 7572 6520 7769  vide a figure wi
-0000e1e0: 7468 2072 6570 7265 7365 6e74 6174 696f  th representatio
-0000e1f0: 6e20 6f66 2064 6174 610a 0a20 2020 2020  n of data..     
-0000e200: 2020 2044 6174 6120 6d65 6d62 6572 733a     Data members:
-0000e210: 0a20 2020 2020 2020 2020 202a 2063 6f70  .          * cop
-0000e220: 7920 6f66 2061 6c6c 2069 6e70 7574 2061  y of all input a
-0000e230: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
-0000e240: 2020 202a 2063 6f76 783a 2063 6f76 6172     * covx: covar
-0000e250: 6961 6e63 6520 6d61 7472 6978 206f 6620  iance matrix of 
-0000e260: 780a 2020 2020 2020 2020 2020 2a20 636f  x.          * co
-0000e270: 7679 3a20 636f 7661 7269 616e 6365 206d  vy: covariance m
-0000e280: 6174 7269 7820 6f66 2079 2075 6e63 6572  atrix of y uncer
-0000e290: 7461 696e 7469 6573 0a20 2020 2020 2020  tainties.       
-0000e2a0: 2020 202a 2063 6f76 3a20 6675 6c6c 2063     * cov: full c
-0000e2b0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-0000e2c0: 2069 6e63 6c2e 2070 726f 6a65 6374 6564   incl. projected
-0000e2d0: 2078 0a20 2020 2020 2020 2020 202a 2069   x.          * i
-0000e2e0: 436f 763a 2069 6e76 6572 7365 206f 6620  Cov: inverse of 
-0000e2f0: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-0000e300: 780a 2020 2020 2020 2020 2222 220a 0a20  x.        """.. 
-0000e310: 2020 2020 2020 2064 6566 205f 5f69 6e69         def __ini
-0000e320: 745f 5f28 0a20 2020 2020 2020 2020 2020  t__(.           
-0000e330: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
-0000e340: 2020 206f 7574 6572 2c0a 2020 2020 2020     outer,.      
-0000e350: 2020 2020 2020 782c 0a20 2020 2020 2020        x,.       
-0000e360: 2020 2020 2079 2c0a 2020 2020 2020 2020       y,.        
-0000e370: 2020 2020 6578 2c0a 2020 2020 2020 2020      ex,.        
-0000e380: 2020 2020 6579 2c0a 2020 2020 2020 2020      ey,.        
-0000e390: 2020 2020 6572 656c 782c 0a20 2020 2020      erelx,.     
-0000e3a0: 2020 2020 2020 2065 7265 6c79 2c0a 2020         erely,.  
-0000e3b0: 2020 2020 2020 2020 2020 6361 6273 782c            cabsx,
-0000e3c0: 0a20 2020 2020 2020 2020 2020 2063 7265  .            cre
-0000e3d0: 6c78 2c0a 2020 2020 2020 2020 2020 2020  lx,.            
-0000e3e0: 6361 6273 792c 0a20 2020 2020 2020 2020  cabsy,.         
-0000e3f0: 2020 2063 7265 6c79 2c0a 2020 2020 2020     crely,.      
-0000e400: 2020 2020 2020 7175 6965 743d 5472 7565        quiet=True
-0000e410: 2c0a 2020 2020 2020 2020 293a 0a20 2020  ,.        ):.   
-0000e420: 2020 2020 2020 2020 2023 2073 6176 6520           # save 
-0000e430: 706f 696e 6572 2074 6f20 6361 6c6c 696e  poiner to callin
-0000e440: 6720 636c 6173 730a 2020 2020 2020 2020  g class.        
-0000e450: 2020 2020 7365 6c66 2e6f 7574 6572 203d      self.outer =
-0000e460: 206f 7574 6572 0a0a 2020 2020 2020 2020   outer..        
-0000e470: 2020 2020 2320 6173 7375 6d65 2073 696d      # assume sim
-0000e480: 706c 6520 6361 7365 2077 2e6f 2e20 636f  ple case w.o. co
-0000e490: 762e 6d61 742e 0a20 2020 2020 2020 2020  v.mat..         
-0000e4a0: 2020 2073 656c 662e 6e65 6564 735f 636f     self.needs_co
-0000e4b0: 7661 7269 616e 6365 203d 2046 616c 7365  variance = False
-0000e4c0: 0a0a 2020 2020 2020 2020 2020 2020 6e64  ..            nd
-0000e4d0: 203d 206c 656e 2878 290a 2020 2020 2020   = len(x).      
-0000e4e0: 2020 2020 2020 2320 7374 6f72 6520 696e        # store in
-0000e4f0: 7075 7420 6461 7461 2061 7320 6e75 6d70  put data as nump
-0000e500: 7920 666c 6f61 7420 6172 7261 7973 2c20  y float arrays, 
-0000e510: 656e 7375 7265 206c 656e 6774 6820 6e64  ensure length nd
-0000e520: 2069 6620 6e65 6564 6564 0a20 2020 2020   if needed.     
-0000e530: 2020 2020 2020 2073 656c 662e 646c 656e         self.dlen
-0000e540: 6774 6820 3d20 6e64 0a20 2020 2020 2020  gth = nd.       
-0000e550: 2020 2020 2073 656c 662e 7820 3d20 6e70       self.x = np
-0000e560: 2e61 7366 6172 7261 7928 7829 2020 2320  .asfarray(x)  # 
-0000e570: 6162 7363 6973 7361 202d 2022 7820 7661  abscissa - "x va
-0000e580: 6c75 6573 220a 2020 2020 2020 2020 2020  lues".          
-0000e590: 2020 7365 6c66 2e79 203d 206e 702e 6173    self.y = np.as
-0000e5a0: 6661 7272 6179 2879 2920 2023 206f 7264  farray(y)  # ord
-0000e5b0: 696e 6174 6520 2d20 2279 2076 616c 7565  inate - "y value
-0000e5c0: 7322 0a20 2020 2020 2020 2020 2020 2069  s".            i
-0000e5d0: 6620 6578 2069 7320 6e6f 7420 4e6f 6e65  f ex is not None
-0000e5e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e5f0: 2020 7365 6c66 2e65 7820 3d20 6e70 2e61    self.ex = np.a
-0000e600: 7366 6172 7261 7928 6578 2920 2023 2069  sfarray(ex)  # i
-0000e610: 6e64 6570 656e 6465 6e74 2075 6e63 6572  ndependent uncer
-0000e620: 7461 696e 7469 6573 2078 0a20 2020 2020  tainties x.     
-0000e630: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000e640: 6c66 2e65 782e 6e64 696d 203d 3d20 303a  lf.ex.ndim == 0:
-0000e650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e660: 2020 2020 2073 656c 662e 6578 203d 2073       self.ex = s
-0000e670: 656c 662e 6578 202a 206e 702e 6f6e 6573  elf.ex * np.ones
-0000e680: 286e 6429 0a20 2020 2020 2020 2020 2020  (nd).           
-0000e690: 2020 2020 2065 6c69 6620 7365 6c66 2e65       elif self.e
-0000e6a0: 782e 6e64 696d 203d 3d20 323a 0a20 2020  x.ndim == 2:.   
-0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6c0: 2073 656c 662e 6e65 6564 735f 636f 7661   self.needs_cova
-0000e6d0: 7269 616e 6365 203d 2054 7275 650a 2020  riance = True.  
-0000e6e0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e700: 7365 6c66 2e65 7820 3d20 4e6f 6e65 0a20  self.ex = None. 
-0000e710: 2020 2020 2020 2020 2020 2069 6620 6579             if ey
-0000e720: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e730: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000e740: 6c66 2e65 7920 3d20 6e70 2e61 7366 6172  lf.ey = np.asfar
-0000e750: 7261 7928 6579 2920 2023 2069 6e64 6570  ray(ey)  # indep
-0000e760: 656e 6465 6e74 2075 6e63 6572 7461 696e  endent uncertain
-0000e770: 7469 6573 2079 0a20 2020 2020 2020 2020  ties y.         
-0000e780: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-0000e790: 792e 6e64 696d 203d 3d20 303a 0a20 2020  y.ndim == 0:.   
-0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e7b0: 2073 656c 662e 6579 203d 2073 656c 662e   self.ey = self.
-0000e7c0: 6579 202a 206e 702e 6f6e 6573 286e 6429  ey * np.ones(nd)
-0000e7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e7e0: 2065 6c69 6620 7365 6c66 2e65 792e 6e64   elif self.ey.nd
-0000e7f0: 696d 203d 3d20 323a 0a20 2020 2020 2020  im == 2:.       
-0000e800: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e810: 662e 6e65 6564 735f 636f 7661 7269 616e  f.needs_covarian
-0000e820: 6365 203d 2054 7275 650a 2020 2020 2020  ce = True.      
-0000e830: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000e840: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000e850: 2e65 7920 3d20 4e6f 6e65 0a20 2020 2020  .ey = None.     
-0000e860: 2020 2020 2020 2069 6620 6572 656c 7820         if erelx 
-0000e870: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000e880: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000e890: 662e 6572 656c 7820 3d20 6e70 2e61 7366  f.erelx = np.asf
-0000e8a0: 6172 7261 7928 6572 656c 7829 2020 2320  array(erelx)  # 
-0000e8b0: 696e 6465 7065 6e64 656e 7420 7265 6c61  independent rela
-0000e8c0: 7469 7665 2075 6e63 6572 7461 696e 7469  tive uncertainti
-0000e8d0: 6573 2078 0a20 2020 2020 2020 2020 2020  es x.           
-0000e8e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000e8f0: 2020 2020 2020 2073 656c 662e 6572 656c         self.erel
-0000e900: 7820 3d20 4e6f 6e65 0a20 2020 2020 2020  x = None.       
-0000e910: 2020 2020 2069 6620 6572 656c 7920 6973       if erely is
-0000e920: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000e930: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000e940: 6572 656c 7920 3d20 6e70 2e61 7366 6172  erely = np.asfar
-0000e950: 7261 7928 6572 656c 7929 2020 2320 696e  ray(erely)  # in
-0000e960: 6465 7065 6e64 656e 7420 7265 6c61 7469  dependent relati
-0000e970: 7665 2075 6e63 6572 7461 696e 7469 6573  ve uncertainties
-0000e980: 2079 0a20 2020 2020 2020 2020 2020 2065   y.            e
-0000e990: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000e9a0: 2020 2020 2073 656c 662e 6572 656c 7920       self.erely 
-0000e9b0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0000e9c0: 2020 2069 6620 6361 6273 7820 6973 206e     if cabsx is n
-0000e9d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000e9e0: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
-0000e9f0: 6273 7820 3d20 6e70 2e61 7366 6172 7261  bsx = np.asfarra
-0000ea00: 7928 6361 6273 7829 2020 2320 636f 7272  y(cabsx)  # corr
-0000ea10: 656c 6174 6564 2061 626f 6c75 7465 2075  elated abolute u
-0000ea20: 6e63 6572 7461 696e 7469 6573 2078 0a20  ncertainties x. 
-0000ea30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000ea40: 6620 7365 6c66 2e63 6162 7378 2e6e 6469  f self.cabsx.ndi
-0000ea50: 6d20 3d3d 2030 3a0a 2020 2020 2020 2020  m == 0:.        
-0000ea60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ea70: 2e63 6162 7378 203d 2073 656c 662e 6361  .cabsx = self.ca
-0000ea80: 6273 7820 2a20 6e70 2e6f 6e65 7328 6e64  bsx * np.ones(nd
-0000ea90: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-0000eaa0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000eab0: 2020 2020 7365 6c66 2e63 6162 7378 203d      self.cabsx =
-0000eac0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000ead0: 2020 6966 2063 7265 6c78 2069 7320 6e6f    if crelx is no
-0000eae0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0000eaf0: 2020 2020 2020 2020 7365 6c66 2e63 7265          self.cre
-0000eb00: 6c78 203d 206e 702e 6173 6661 7272 6179  lx = np.asfarray
-0000eb10: 2863 7265 6c78 2920 2023 2063 6f72 7265  (crelx)  # corre
-0000eb20: 6c61 7465 6420 7265 6c61 7469 7665 2075  lated relative u
-0000eb30: 6e63 6572 7461 696e 7469 6573 2078 0a20  ncertainties x. 
-0000eb40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000eb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eb60: 2073 656c 662e 6372 656c 7820 3d20 4e6f   self.crelx = No
-0000eb70: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
-0000eb80: 6620 6361 6273 7920 6973 206e 6f74 204e  f cabsy is not N
-0000eb90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000eba0: 2020 2020 2073 656c 662e 6361 6273 7920       self.cabsy 
-0000ebb0: 3d20 6e70 2e61 7366 6172 7261 7928 6361  = np.asfarray(ca
-0000ebc0: 6273 7929 2020 2320 636f 7272 656c 6174  bsy)  # correlat
-0000ebd0: 6564 2061 6273 6f6c 7574 6520 756e 6365  ed absolute unce
-0000ebe0: 7274 6169 6e74 6965 7320 790a 2020 2020  rtainties y.    
-0000ebf0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000ec00: 656c 662e 6361 6273 792e 6e64 696d 203d  elf.cabsy.ndim =
-0000ec10: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0000ec20: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
-0000ec30: 6273 7920 3d20 7365 6c66 2e63 6162 7379  bsy = self.cabsy
-0000ec40: 202a 206e 702e 6f6e 6573 286e 6429 0a20   * np.ones(nd). 
-0000ec50: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000ec60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec70: 2073 656c 662e 6361 6273 7920 3d20 4e6f   self.cabsy = No
-0000ec80: 6e65 0a20 2020 2020 2020 2020 2020 2069  ne.            i
-0000ec90: 6620 6372 656c 7920 6973 206e 6f74 204e  f crely is not N
-0000eca0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000ecb0: 2020 2020 2073 656c 662e 6372 656c 7920       self.crely 
-0000ecc0: 3d20 6e70 2e61 7366 6172 7261 7928 6372  = np.asfarray(cr
-0000ecd0: 656c 7929 2020 2320 636f 7272 656c 6174  ely)  # correlat
-0000ece0: 6564 2072 656c 6174 6976 6520 756e 6365  ed relative unce
-0000ecf0: 7274 6169 6e74 6965 7320 790a 2020 2020  rtainties y.    
-0000ed00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ed10: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ed20: 6c66 2e63 7265 6c79 203d 204e 6f6e 650a  lf.crely = None.
-0000ed30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ed40: 2e71 7569 6574 203d 2071 7569 6574 2020  .quiet = quiet  
-0000ed50: 2320 6e6f 2069 6e66 6f72 6d61 7469 7665  # no informative
-0000ed60: 2070 7269 6e74 6f75 7420 6966 2054 7275   printout if Tru
-0000ed70: 650a 0a20 2020 2020 2020 2020 2020 2073  e..            s
-0000ed80: 656c 662e 6e64 203d 206e 640a 2020 2020  elf.nd = nd.    
-0000ed90: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
-0000eda0: 656c 203d 204e 6f6e 6520 2023 206e 6f20  el = None  # no 
-0000edb0: 6d6f 6465 6c20 6465 6669 6e65 6420 7965  model defined ye
-0000edc0: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
-0000edd0: 6c66 2e6d 6f64 656c 5f76 616c 7565 7320  lf.model_values 
-0000ede0: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-0000edf0: 2020 2020 2320 7365 7420 666c 6167 7320      # set flags 
-0000ee00: 666f 7220 7374 6565 7269 6e67 206f 6620  for steering of 
-0000ee10: 6669 7420 7072 6f63 6573 7320 696e 2064  fit process in d
-0000ee20: 6f5f 6669 7428 290a 2020 2020 2020 2020  o_fit().        
-0000ee30: 2020 2020 7365 6c66 2e72 6562 756c 696c      self.rebulil
-0000ee40: 6443 6f76 203d 204e 6f6e 650a 2020 2020  dCov = None.    
-0000ee50: 2020 2020 2020 2020 7365 6c66 2e68 6173          self.has
-0000ee60: 5f78 4572 726f 7273 203d 2028 0a20 2020  _xErrors = (.   
-0000ee70: 2020 2020 2020 2020 2020 2020 2065 7820               ex 
-0000ee80: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
-0000ee90: 2020 2020 2020 2020 2020 2020 6f72 2065              or e
-0000eea0: 7265 6c78 2069 7320 6e6f 7420 4e6f 6e65  relx is not None
-0000eeb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eec0: 206f 7220 6361 6273 7820 6973 206e 6f74   or cabsx is not
-0000eed0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0000eee0: 2020 2020 2020 6f72 2063 7265 6c78 2069        or crelx i
-0000eef0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
-0000ef00: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000ef10: 2020 2020 2073 656c 662e 6861 735f 7265       self.has_re
-0000ef20: 6c5f 7945 7272 6f72 7320 3d20 6572 656c  l_yErrors = erel
-0000ef30: 7920 6973 206e 6f74 204e 6f6e 6520 6f72  y is not None or
-0000ef40: 2063 7265 6c79 2069 7320 6e6f 7420 4e6f   crely is not No
-0000ef50: 6e65 0a20 2020 2020 2020 2020 2020 2073  ne.            s
-0000ef60: 656c 662e 6e65 6564 735f 636f 7661 7269  elf.needs_covari
-0000ef70: 616e 6365 203d 2028 0a20 2020 2020 2020  ance = (.       
-0000ef80: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
-0000ef90: 6564 735f 636f 7661 7269 616e 6365 0a20  eds_covariance. 
-0000efa0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000efb0: 7220 7365 6c66 2e63 6162 7378 2069 7320  r self.cabsx is 
-0000efc0: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
-0000efd0: 2020 2020 2020 2020 206f 7220 7365 6c66           or self
-0000efe0: 2e63 7265 6c78 2069 7320 6e6f 7420 4e6f  .crelx is not No
-0000eff0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000f000: 2020 206f 7220 7365 6c66 2e63 6162 7379     or self.cabsy
-0000f010: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-0000f020: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-0000f030: 7365 6c66 2e63 7265 6c79 2069 7320 6e6f  self.crely is no
-0000f040: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-0000f050: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0000f060: 2020 2320 6275 696c 6420 2869 6e69 7469    # build (initi
-0000f070: 616c 2920 636f 7661 7269 616e 6365 206d  al) covariance m
-0000f080: 6174 7269 7820 2877 6974 686f 7574 2078  atrix (without x
-0000f090: 2d65 7272 6f72 7329 0a20 2020 2020 2020  -errors).       
-0000f0a0: 2020 2020 2069 6620 7365 6c66 2e6e 6565       if self.nee
-0000f0b0: 6473 5f63 6f76 6172 6961 6e63 653a 0a20  ds_covariance:. 
-0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000f0d0: 7272 3220 3d20 5f62 7569 6c64 5f43 6f76  rr2 = _build_Cov
-0000f0e0: 4d61 7428 0a20 2020 2020 2020 2020 2020  Mat(.           
-0000f0f0: 2020 2020 2020 2020 2073 656c 662e 6e64           self.nd
-0000f100: 2c20 7365 6c66 2e65 792c 2073 656c 662e  , self.ey, self.
-0000f110: 6572 656c 792c 2073 656c 662e 6361 6273  erely, self.cabs
-0000f120: 792c 2073 656c 662e 6372 656c 792c 2073  y, self.crely, s
-0000f130: 656c 662e 790a 2020 2020 2020 2020 2020  elf.y.          
-0000f140: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000f150: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000f160: 2020 2020 2020 2020 2020 6572 7232 203d            err2 =
-0000f170: 205f 6275 696c 645f 4572 7232 2873 656c   _build_Err2(sel
-0000f180: 662e 6579 2c20 7365 6c66 2e65 7265 6c79  f.ey, self.erely
-0000f190: 2c20 7365 6c66 2e79 290a 0a20 2020 2020  , self.y)..     
-0000f1a0: 2020 2020 2020 2023 2069 6e69 7469 616c         # initial
-0000f1b0: 697a 6520 756e 6365 7274 6169 6e74 6965  ize uncertaintie
-0000f1c0: 7320 616e 6420 636f 7661 7269 616e 6365  s and covariance
-0000f1d0: 206d 6174 7269 782c 0a20 2020 2020 2020   matrix,.       
-0000f1e0: 2020 2020 2073 656c 662e 5f69 6e69 7469       self._initi
-0000f1f0: 616c 436f 7628 6572 7232 290a 2020 2020  alCov(err2).    
-0000f200: 2020 2020 2020 2020 2320 7365 7473 3a0a          # sets:.
-0000f210: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000f220: 7365 6c66 2e63 6f76 783a 2063 6f76 6172  self.covx: covar
-0000f230: 6961 6e63 6520 6d61 7472 6978 206f 6620  iance matrix of 
-0000f240: 780a 2020 2020 2020 2020 2020 2020 2320  x.            # 
-0000f250: 2020 7365 6c66 2e63 6f76 793a 2063 6f76    self.covy: cov
-0000f260: 6172 6961 6e63 6520 6d61 7472 6978 206f  ariance matrix o
-0000f270: 6620 7920 756e 6365 7274 6169 6e74 6965  f y uncertaintie
-0000f280: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-0000f290: 2020 7365 6c66 2e63 6f76 3a20 6675 6c6c    self.cov: full
-0000f2a0: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-0000f2b0: 6978 2069 6e63 6c2e 2070 726f 6a65 6374  ix incl. project
-0000f2c0: 6564 2078 0a20 2020 2020 2020 2020 2020  ed x.           
-0000f2d0: 2023 2020 2073 656c 662e 6943 6f76 3a20   #   self.iCov: 
-0000f2e0: 696e 7665 7273 6520 6f66 2063 6f76 6172  inverse of covar
-0000f2f0: 6961 6e63 6520 6d61 7472 6978 0a20 2020  iance matrix.   
-0000f300: 2020 2020 2020 2020 2023 2020 2073 656c           #   sel
-0000f310: 662e 6572 7232 3a20 6172 7261 7920 6f66  f.err2: array of
-0000f320: 2073 7175 6172 6564 2075 6e63 6572 7461   squared uncerta
-0000f330: 696e 7469 6573 0a20 2020 2020 2020 2020  inties.         
-0000f340: 2020 2023 2020 2073 656c 662e 6945 7272     #   self.iErr
-0000f350: 323a 2031 2e2f 7365 6c66 2e65 7272 320a  2: 1./self.err2.
-0000f360: 0a20 2020 2020 2020 2064 6566 205f 696e  .        def _in
-0000f370: 6974 6961 6c43 6f76 2873 656c 662c 2065  itialCov(self, e
-0000f380: 7272 3229 3a0a 2020 2020 2020 2020 2020  rr2):.          
-0000f390: 2020 2222 2242 7569 6c64 2069 6e69 7469    """Build initi
-0000f3a0: 616c 2028 7374 6174 6963 2920 636f 7661  al (static) cova
-0000f3b0: 7269 616e 6365 206d 6174 7269 7820 666f  riance matrix fo
-0000f3c0: 7220 792d 6572 726f 7273 0a20 2020 2020  r y-errors.     
-0000f3d0: 2020 2020 2020 2028 666f 7220 7072 652d         (for pre-
-0000f3e0: 6669 7429 2061 6e64 2063 616c 6375 6c61  fit) and calcula
-0000f3f0: 7465 2069 6e76 6572 7365 206d 6174 7269  te inverse matri
-0000f400: 780a 2020 2020 2020 2020 2020 2020 2222  x.            ""
-0000f410: 220a 2020 2020 2020 2020 2020 2020 6966  ".            if
-0000f420: 2065 7272 322e 6e64 696d 203d 3d20 323a   err2.ndim == 2:
-0000f430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f440: 2023 2067 6f74 2061 2063 6f76 6172 6961   # got a covaria
-0000f450: 6e63 6520 6d61 7472 6978 2c20 6e65 6564  nce matrix, need
-0000f460: 2069 6e76 6572 7365 0a20 2020 2020 2020   inverse.       
-0000f470: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
-0000f480: 6564 735f 636f 7661 7269 616e 6365 203d  eds_covariance =
-0000f490: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
-0000f4a0: 2020 2020 2020 7365 6c66 2e63 6f76 7920        self.covy 
-0000f4b0: 3d20 6572 7232 0a20 2020 2020 2020 2020  = err2.         
-0000f4c0: 2020 2020 2020 2073 656c 662e 6943 6f76         self.iCov
-0000f4d0: 203d 206c 696e 616c 672e 696e 7628 6572   = linalg.inv(er
-0000f4e0: 7232 290a 2020 2020 2020 2020 2020 2020  r2).            
-0000f4f0: 2020 2020 7365 6c66 2e65 7272 3220 3d20      self.err2 = 
-0000f500: 6e70 2e64 6961 676f 6e61 6c28 6572 7232  np.diagonal(err2
-0000f510: 2920 2023 2073 7175 6172 6564 2064 6961  )  # squared dia
-0000f520: 676f 6e61 6c20 656c 656d 656e 7473 0a20  gonal elements. 
-0000f530: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000f540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f550: 2023 2067 6f74 2069 6e64 6570 656e 6465   # got independe
-0000f560: 6e74 2075 6e63 6572 7461 696e 7469 6573  nt uncertainties
-0000f570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f580: 2073 656c 662e 6572 7232 203d 2065 7272   self.err2 = err
-0000f590: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
-0000f5a0: 2020 7365 6c66 2e65 7272 3279 203d 2065    self.err2y = e
-0000f5b0: 7272 320a 2020 2020 2020 2020 2020 2020  rr2.            
-0000f5c0: 2020 2020 7365 6c66 2e69 4572 7232 203d      self.iErr2 =
-0000f5d0: 2031 2e30 202f 2065 7272 320a 2020 2020   1.0 / err2.    
-0000f5e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f5f0: 2e63 6f76 7920 3d20 6e70 2e64 6961 6728  .covy = np.diag(
-0000f600: 6572 7232 290a 2020 2020 2020 2020 2020  err2).          
-0000f610: 2020 2020 2020 7365 6c66 2e69 436f 7620        self.iCov 
-0000f620: 3d20 6e70 2e64 6961 6728 312e 3020 2f20  = np.diag(1.0 / 
-0000f630: 7365 6c66 2e65 7272 3229 0a20 2020 2020  self.err2).     
-0000f640: 2020 2020 2020 2023 2064 6f20 6e6f 7420         # do not 
-0000f650: 7265 6275 696c 6420 636f 7661 7269 616e  rebuild covarian
-0000f660: 6365 206d 6174 7269 7820 696e 2063 6f73  ce matrix in cos
-0000f670: 7420 6675 6e63 7469 6f6e 0a20 2020 2020  t function.     
-0000f680: 2020 2020 2020 2073 656c 662e 6e65 6564         self.need
-0000f690: 735f 6479 6e61 6d69 6345 7272 6f72 7320  s_dynamicErrors 
-0000f6a0: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
-0000f6b0: 2020 2020 2023 206e 6f20 636f 7661 7269       # no covari
-0000f6c0: 616e 6365 206f 6620 782d 6572 726f 7273  ance of x-errors
-0000f6d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f6e0: 662e 636f 7678 203d 204e 6f6e 650a 2020  f.covx = None.  
-0000f6f0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-0000f700: 7272 3278 203d 204e 6f6e 650a 2020 2020  rr2x = None.    
-0000f710: 2020 2020 2020 2020 2320 746f 7461 6c20          # total 
-0000f720: 636f 7661 7269 616e 6365 2069 7320 7468  covariance is th
-0000f730: 6174 206f 6620 792d 6572 726f 7273 0a20  at of y-errors. 
-0000f740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000f750: 636f 7620 3d20 7365 6c66 2e63 6f76 790a  cov = self.covy.
-0000f760: 0a20 2020 2020 2020 2064 6566 2069 6e69  .        def ini
-0000f770: 745f 6479 6e61 6d69 6345 7272 6f72 7328  t_dynamicErrors(
-0000f780: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
-0000f790: 2020 2023 206d 6574 686f 6420 746f 2073     # method to s
-0000f7a0: 7769 7463 6820 6f6e 2064 796e 616d 6963  witch on dynamic
-0000f7b0: 2072 652d 6361 6c63 756c 6174 696f 6e20   re-calculation 
-0000f7c0: 6f66 2063 6f76 6172 6961 6e63 6520 6d61  of covariance ma
-0000f7d0: 7472 6978 0a20 2020 2020 2020 2020 2020  trix.           
-0000f7e0: 2073 656c 662e 7265 665f 746f 4d6f 6465   self.ref_toMode
-0000f7f0: 6c20 3d20 7365 6c66 2e6f 7574 6572 2e72  l = self.outer.r
-0000f800: 6566 4d6f 6465 6c0a 2020 2020 2020 2020  efModel.        
-0000f810: 2020 2020 7365 6c66 2e6d 6f64 656c 203d      self.model =
-0000f820: 2073 656c 662e 6f75 7465 722e 636f 7374   self.outer.cost
-0000f830: 662e 6d6f 6465 6c0a 0a20 2020 2020 2020  f.model..       
-0000f840: 2020 2020 2073 656c 662e 5f73 7461 7469       self._stati
-0000f850: 6343 6f76 203d 204e 6f6e 650a 2020 2020  cCov = None.    
-0000f860: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
-0000f870: 6174 6963 4572 7232 203d 204e 6f6e 650a  aticErr2 = None.
-0000f880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000f890: 2e69 436f 7620 3d20 4e6f 6e65 0a20 2020  .iCov = None.   
-0000f8a0: 2020 2020 2020 2020 2073 656c 662e 6945           self.iE
-0000f8b0: 7272 3220 3d20 4e6f 6e65 0a0a 2020 2020  rr2 = None..    
-0000f8c0: 2020 2020 2020 2020 2320 7265 6275 696c          # rebuil
-0000f8d0: 6420 636f 7661 7269 616e 6365 206d 6174  d covariance mat
-0000f8e0: 7269 7820 6475 7269 6e67 2066 6974 7469  rix during fitti
-0000f8f0: 6e67 2070 726f 6365 6475 7265 0a20 2020  ng procedure.   
-0000f900: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
-0000f910: 6564 735f 6479 6e61 6d69 6345 7272 6f72  eds_dynamicError
-0000f920: 7320 3d20 5472 7565 2020 2320 666c 6167  s = True  # flag
-0000f930: 2066 6f72 2063 6f73 7420 6675 6e63 7469   for cost functi
-0000f940: 6f6e 0a20 2020 2020 2020 2020 2020 2073  on.            s
-0000f950: 656c 662e 6669 6e61 6c5f 6361 6c6c 203d  elf.final_call =
-0000f960: 2046 616c 7365 2020 2320 666c 6167 2066   False  # flag f
-0000f970: 6f72 205f 7265 6275 696c 645f 436f 763a  or _rebuild_Cov:
-0000f980: 206e 6f20 7374 6f72 6167 6520 6f66 2079   no storage of y
-0000f990: 636f 760a 0a20 2020 2020 2020 2020 2020  cov..           
-0000f9a0: 2069 6620 7365 6c66 2e6e 6565 6473 5f63   if self.needs_c
-0000f9b0: 6f76 6172 6961 6e63 653a 0a20 2020 2020  ovariance:.     
-0000f9c0: 2020 2020 2020 2020 2020 2023 2062 7569             # bui
-0000f9d0: 6c64 2073 7461 7469 6320 283d 7061 7261  ld static (=para
-0000f9e0: 6d65 7465 722d 696e 6465 7065 6e64 656e  meter-independen
-0000f9f0: 7429 2070 6172 7420 6f66 2063 6f76 6172  t) part of covar
-0000fa00: 6961 6e63 6520 6d61 7472 6978 0a20 2020  iance matrix.   
-0000fa10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000fa20: 7365 6c66 2e68 6173 5f72 656c 5f79 4572  self.has_rel_yEr
-0000fa30: 726f 7273 2061 6e64 2073 656c 662e 7265  rors and self.re
-0000fa40: 665f 746f 4d6f 6465 6c3a 0a20 2020 2020  f_toModel:.     
-0000fa50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000fa60: 2073 6f6d 6520 792d 6572 726f 7273 2061   some y-errors a
-0000fa70: 7265 2070 6172 616d 6574 6572 2d69 6e64  re parameter-ind
-0000fa80: 6570 656e 6465 6e74 0a20 2020 2020 2020  ependent.       
-0000fa90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000faa0: 662e 5f73 7461 7469 6343 6f76 203d 205f  f._staticCov = _
-0000fab0: 6275 696c 645f 436f 764d 6174 280a 2020  build_CovMat(.  
-0000fac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fad0: 2020 2020 2020 7365 6c66 2e6e 642c 2073        self.nd, s
-0000fae0: 656c 662e 6579 2c20 6561 6273 636f 723d  elf.ey, eabscor=
-0000faf0: 7365 6c66 2e63 6162 7379 0a20 2020 2020  self.cabsy.     
-0000fb00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000fb10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fb20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000fb30: 2020 2020 2020 2020 2020 2023 2061 6c6c             # all
-0000fb40: 2079 2d65 7272 6f72 7320 6172 6520 7061   y-errors are pa
-0000fb50: 7261 6d65 7465 722d 696e 6465 7065 6e64  rameter-independ
-0000fb60: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-0000fb70: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
-0000fb80: 6174 6963 436f 7620 3d20 5f62 7569 6c64  aticCov = _build
-0000fb90: 5f43 6f76 4d61 7428 0a20 2020 2020 2020  _CovMat(.       
+0000c690: 2020 2020 2020 2020 2275 7369 6e67 202d          "using -
+0000c6a0: 322a 6c6e 2050 6f69 7373 6f6e 206c 696b  2*ln Poisson lik
+0000c6b0: 656c 6968 6f6f 6422 2c0a 2020 2020 2020  elihood",.      
+0000c6c0: 2020 2020 2020 2275 7369 6e67 2047 6175        "using Gau
+0000c6d0: 7373 6961 6e20 6170 7072 6f78 696d 6174  ssian approximat
+0000c6e0: 696f 6e20 6f66 2050 6f69 7373 6f6e 2064  ion of Poisson d
+0000c6f0: 6973 7472 6962 7574 696f 6e22 2c0a 2020  istribution",.  
+0000c700: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0000c710: 7365 6c66 2e6f 7074 696f 6e73 5b22 6669  self.options["fi
+0000c720: 745f 6465 6e73 6974 7922 5d20 3d20 5b0a  t_density"] = [.
+0000c730: 2020 2020 2020 2020 2020 2020 312c 0a20              1,. 
+0000c740: 2020 2020 2020 2020 2020 2022 6869 7374             "hist
+0000c750: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+0000c760: 6669 7420 666f 7220 6e75 6d62 6572 206f  fit for number o
+0000c770: 6620 656e 7472 6965 732f 6269 6e22 2c0a  f entries/bin",.
+0000c780: 2020 2020 2020 2020 2020 2020 2266 6974              "fit
+0000c790: 2064 656e 7369 7479 2064 6973 7472 6962   density distrib
+0000c7a0: 7574 696f 6e22 2c0a 2020 2020 2020 2020  ution",.        
+0000c7b0: 5d0a 2020 2020 2020 2020 7365 6c66 2e6f  ].        self.o
+0000c7c0: 7074 696f 6e73 5b22 6e65 6732 6c6f 674c  ptions["neg2logL
+0000c7d0: 225d 203d 205b 0a20 2020 2020 2020 2020  "] = [.         
+0000c7e0: 2020 2031 2c0a 2020 2020 2020 2020 2020     1,.          
+0000c7f0: 2020 5b22 7573 6572 222c 2022 6d6c 225d    ["user", "ml"]
+0000c800: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
+0000c810: 7369 6e67 2073 7461 6e64 6172 6420 6c69  sing standard li
+0000c820: 6b65 6c69 686f 6f64 202d 3e20 6572 7264  kelihood -> errd
+0000c830: 6566 203d 2030 2e35 222c 0a20 2020 2020  ef = 0.5",.     
+0000c840: 2020 2020 2020 2022 7573 696e 6720 2d32         "using -2
+0000c850: 202a 206e 6567 2e20 6c6f 672e 206c 696b   * neg. log. lik
+0000c860: 656c 6968 6f6f 6420 2d3e 2065 7272 6465  elihood -> errde
+0000c870: 663d 312e 222c 0a20 2020 2020 2020 205d  f=1.",.        ]
+0000c880: 0a0a 2020 2020 2020 2020 2320 7365 7420  ..        # set 
+0000c890: 6f70 7469 6f6e 7320 666f 7220 286e 6963  options for (nic
+0000c8a0: 6572 2920 706c 6f74 7469 6e67 0a20 2020  er) plotting.   
+0000c8b0: 2020 2020 2073 656c 662e 7365 7450 6c6f       self.setPlo
+0000c8c0: 744f 7074 696f 6e73 2829 0a0a 2020 2020  tOptions()..    
+0000c8d0: 6465 6620 696e 6974 5f64 6174 6128 7365  def init_data(se
+0000c8e0: 6c66 2c20 2a61 7267 732c 202a 2a6b 7761  lf, *args, **kwa
+0000c8f0: 7267 7329 3a0a 2020 2020 2020 2020 6966  rgs):.        if
+0000c900: 2073 656c 662e 6669 745f 7479 7065 203d   self.fit_type =
+0000c910: 3d20 2278 7922 3a0a 2020 2020 2020 2020  = "xy":.        
+0000c920: 2020 2020 7365 6c66 2e69 6e69 745f 7879      self.init_xy
+0000c930: 4461 7461 282a 6172 6773 2c20 2a2a 6b77  Data(*args, **kw
+0000c940: 6172 6773 290a 2020 2020 2020 2020 656c  args).        el
+0000c950: 6966 2073 656c 662e 6669 745f 7479 7065  if self.fit_type
+0000c960: 203d 3d20 2269 6e64 6578 6564 223a 0a20   == "indexed":. 
+0000c970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000c980: 696e 6974 5f78 4461 7461 282a 6172 6773  init_xData(*args
+0000c990: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+0000c9a0: 2020 2020 656c 6966 2073 656c 662e 6669      elif self.fi
+0000c9b0: 745f 7479 7065 203d 3d20 2268 6973 7422  t_type == "hist"
+0000c9c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000c9d0: 6c66 2e69 6e69 745f 6844 6174 6128 2a61  lf.init_hData(*a
+0000c9e0: 7267 732c 202a 2a6b 7761 7267 7329 0a20  rgs, **kwargs). 
+0000c9f0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+0000ca00: 2e66 6974 5f74 7970 6520 3d3d 2022 6d6c  .fit_type == "ml
+0000ca10: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
+0000ca20: 656c 662e 696e 6974 5f6d 6c44 6174 6128  elf.init_mlData(
+0000ca30: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+0000ca40: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+0000ca50: 6c66 2e66 6974 5f74 7970 6520 3d3d 2022  lf.fit_type == "
+0000ca60: 7573 6572 223a 0a20 2020 2020 2020 2020  user":.         
+0000ca70: 2020 2070 7269 6e74 2822 212a 2a21 206d     print("!**! m
+0000ca80: 6e46 6974 3a20 6e6f 7420 6461 7461 206f  nFit: not data o
+0000ca90: 626a 6563 7420 746f 2062 6520 6465 6669  bject to be defi
+0000caa0: 6e64 6564 2066 6f72 2066 6974 5f74 7970  nded for fit_typ
+0000cab0: 6520 2775 7365 7227 2229 0a20 2020 2020  e 'user'").     
+0000cac0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000cad0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0000cae0: 4572 726f 7228 2221 2a2a 2120 756e 6b6e  Error("!**! unkn
+0000caf0: 6f77 6e20 7479 7065 206f 6620 4669 7420  own type of Fit 
+0000cb00: 2220 2b20 7365 6c66 2e66 6974 5f74 7970  " + self.fit_typ
+0000cb10: 6529 0a0a 2020 2020 6465 6620 7365 744f  e)..    def setO
+0000cb20: 7074 696f 6e73 2873 656c 662c 202a 6172  ptions(self, *ar
+0000cb30: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
+0000cb40: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+0000cb50: 6974 5f74 7970 6520 3d3d 2022 7879 223a  it_type == "xy":
+0000cb60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cb70: 662e 7365 745f 7879 4f70 7469 6f6e 7328  f.set_xyOptions(
+0000cb80: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+0000cb90: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+0000cba0: 6c66 2e66 6974 5f74 7970 6520 3d3d 2022  lf.fit_type == "
+0000cbb0: 696e 6465 7865 6422 3a0a 2020 2020 2020  indexed":.      
+0000cbc0: 2020 2020 2020 7365 6c66 2e73 6574 5f78        self.set_x
+0000cbd0: 4f70 7469 6f6e 7328 2a61 7267 732c 202a  Options(*args, *
+0000cbe0: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
+0000cbf0: 2065 6c69 6620 7365 6c66 2e66 6974 5f74   elif self.fit_t
+0000cc00: 7970 6520 3d3d 2022 6869 7374 223a 0a20  ype == "hist":. 
+0000cc10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000cc20: 7365 745f 684f 7074 696f 6e73 282a 6172  set_hOptions(*ar
+0000cc30: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
+0000cc40: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+0000cc50: 6669 745f 7479 7065 203d 3d20 2275 7365  fit_type == "use
+0000cc60: 7222 206f 7220 7365 6c66 2e66 6974 5f74  r" or self.fit_t
+0000cc70: 7970 6520 3d3d 2022 6d6c 223a 0a20 2020  ype == "ml":.   
+0000cc80: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+0000cc90: 745f 6d6e 4f70 7469 6f6e 7328 2a61 7267  t_mnOptions(*arg
+0000cca0: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
+0000ccb0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000ccc0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0000ccd0: 7565 4572 726f 7228 2221 2a2a 2120 756e  ueError("!**! un
+0000cce0: 6b6e 6f77 6e20 7479 7065 206f 6620 4669  known type of Fi
+0000ccf0: 7420 2220 2b20 7365 6c66 2e66 6974 5f74  t " + self.fit_t
+0000cd00: 7970 6529 0a0a 2020 2020 6465 6620 696e  ype)..    def in
+0000cd10: 6974 5f66 6974 2873 656c 662c 202a 6172  it_fit(self, *ar
+0000cd20: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
+0000cd30: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+0000cd40: 6974 5f74 7970 6520 3d3d 2022 7879 223a  it_type == "xy":
+0000cd50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000cd60: 662e 696e 6974 5f78 7946 6974 282a 6172  f.init_xyFit(*ar
+0000cd70: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
+0000cd80: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+0000cd90: 6669 745f 7479 7065 203d 3d20 2269 6e64  fit_type == "ind
+0000cda0: 6578 6564 223a 0a20 2020 2020 2020 2020  exed":.         
+0000cdb0: 2020 2073 656c 662e 696e 6974 5f78 4669     self.init_xFi
+0000cdc0: 7428 2a61 7267 732c 202a 2a6b 7761 7267  t(*args, **kwarg
+0000cdd0: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
+0000cde0: 7365 6c66 2e66 6974 5f74 7970 6520 3d3d  self.fit_type ==
+0000cdf0: 2022 6869 7374 223a 0a20 2020 2020 2020   "hist":.       
+0000ce00: 2020 2020 2073 656c 662e 696e 6974 5f68       self.init_h
+0000ce10: 4669 7428 2a61 7267 732c 202a 2a6b 7761  Fit(*args, **kwa
+0000ce20: 7267 7329 0a20 2020 2020 2020 2065 6c69  rgs).        eli
+0000ce30: 6620 7365 6c66 2e66 6974 5f74 7970 6520  f self.fit_type 
+0000ce40: 3d3d 2022 7573 6572 2220 6f72 2073 656c  == "user" or sel
+0000ce50: 662e 6669 745f 7479 7065 203d 3d20 226d  f.fit_type == "m
+0000ce60: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+0000ce70: 7365 6c66 2e69 6e69 745f 6d6e 4669 7428  self.init_mnFit(
+0000ce80: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+0000ce90: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000cea0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000ceb0: 2056 616c 7565 4572 726f 7228 2221 2a2a   ValueError("!**
+0000cec0: 2120 756e 6b6e 6f77 6e20 7479 7065 206f  ! unknown type o
+0000ced0: 6620 4669 7420 2220 2b20 7365 6c66 2e66  f Fit " + self.f
+0000cee0: 6974 5f74 7970 6529 0a0a 2020 2020 230a  it_type)..    #.
+0000cef0: 2020 2020 2320 2d2d 2d20 7370 6563 6961      # --- specia
+0000cf00: 6c20 636f 6465 2066 6f72 2078 7920 4669  l code for xy Fi
+0000cf10: 740a 2020 2020 230a 0a20 2020 2064 6566  t.    #..    def
+0000cf20: 2073 6574 5f78 794f 7074 696f 6e73 280a   set_xyOptions(.
+0000cf30: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000cf40: 2020 2020 2020 7265 6c61 7469 7665 5f72        relative_r
+0000cf50: 6566 6572 735f 746f 5f6d 6f64 656c 3d4e  efers_to_model=N
+0000cf60: 6f6e 652c 0a20 2020 2020 2020 2072 756e  one,.        run
+0000cf70: 5f6d 696e 6f73 3d4e 6f6e 652c 0a20 2020  _minos=None,.   
+0000cf80: 2020 2020 2075 7365 5f6e 6567 4c6f 674c       use_negLogL
+0000cf90: 3d4e 6f6e 652c 0a20 2020 2020 2020 2071  =None,.        q
+0000cfa0: 7569 6574 3d4e 6f6e 652c 0a20 2020 2029  uiet=None,.    )
+0000cfb0: 3a0a 2020 2020 2020 2020 2222 2244 6566  :.        """Def
+0000cfc0: 696e 6520 6f70 7469 6f6e 7320 666f 7220  ine options for 
+0000cfd0: 7879 2066 6974 0a0a 2020 2020 2020 2020  xy fit..        
+0000cfe0: 4172 6773 3a0a 2020 2020 2020 2020 202d  Args:.         -
+0000cff0: 2072 656c 2e20 6572 726f 7273 2072 6566   rel. errors ref
+0000d000: 6572 2074 6f20 6d6f 6465 6c20 656c 7365  er to model else
+0000d010: 2064 6174 610a 2020 2020 2020 2020 202d   data.         -
+0000d020: 2072 756e 206d 696e 6f73 2065 6c73 6520   run minos else 
+0000d030: 646f 6e2a 7420 7275 6e20 6d69 6e6f 730a  don*t run minos.
+0000d040: 2020 2020 2020 2020 202d 2075 7365 2066           - use f
+0000d050: 756c 6c20 6e65 6732 6c6f 674c 0a20 2020  ull neg2logL.   
+0000d060: 2020 2020 2020 2d20 646f 6e2a 7420 7072        - don*t pr
+0000d070: 6f76 6964 6520 7072 696e 746f 7574 2065  ovide printout e
+0000d080: 6c73 6520 7665 7262 6f73 6520 7072 696e  lse verbose prin
+0000d090: 746f 7574 0a20 2020 2020 2020 2022 2222  tout.        """
+0000d0a0: 0a20 2020 2020 2020 2069 6620 7265 6c61  .        if rela
+0000d0b0: 7469 7665 5f72 6566 6572 735f 746f 5f6d  tive_refers_to_m
+0000d0c0: 6f64 656c 2069 7320 6e6f 7420 4e6f 6e65  odel is not None
+0000d0d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0000d0e0: 6c66 2e72 6566 4d6f 6465 6c20 3d20 7265  lf.refModel = re
+0000d0f0: 6c61 7469 7665 5f72 6566 6572 735f 746f  lative_refers_to
+0000d100: 5f6d 6f64 656c 0a20 2020 2020 2020 2020  _model.         
+0000d110: 2020 2073 656c 662e 6f70 7469 6f6e 735b     self.options[
+0000d120: 2272 6566 4d6f 6465 6c22 5d5b 305d 203d  "refModel"][0] =
+0000d130: 2069 6e74 2872 656c 6174 6976 655f 7265   int(relative_re
+0000d140: 6665 7273 5f74 6f5f 6d6f 6465 6c29 0a20  fers_to_model). 
+0000d150: 2020 2020 2020 2069 6620 7275 6e5f 6d69         if run_mi
+0000d160: 6e6f 7320 6973 206e 6f74 204e 6f6e 653a  nos is not None:
+0000d170: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d180: 662e 7275 6e5f 6d69 6e6f 7320 3d20 7275  f.run_minos = ru
+0000d190: 6e5f 6d69 6e6f 730a 2020 2020 2020 2020  n_minos.        
+0000d1a0: 2020 2020 7365 6c66 2e6f 7074 696f 6e73      self.options
+0000d1b0: 5b22 7275 6e5f 6d69 6e6f 7322 5d5b 305d  ["run_minos"][0]
+0000d1c0: 203d 2069 6e74 2872 756e 5f6d 696e 6f73   = int(run_minos
+0000d1d0: 290a 2020 2020 2020 2020 6966 2075 7365  ).        if use
+0000d1e0: 5f6e 6567 4c6f 674c 2069 7320 6e6f 7420  _negLogL is not 
+0000d1f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000d200: 2020 7365 6c66 2e75 7365 5f6e 6567 4c6f    self.use_negLo
+0000d210: 674c 203d 2075 7365 5f6e 6567 4c6f 674c  gL = use_negLogL
+0000d220: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000d230: 662e 6f70 7469 6f6e 735b 2275 7365 5f6e  f.options["use_n
+0000d240: 6567 4c6f 674c 225d 5b30 5d20 3d20 696e  egLogL"][0] = in
+0000d250: 7428 7573 655f 6e65 674c 6f67 4c29 0a20  t(use_negLogL). 
+0000d260: 2020 2020 2020 2069 6620 7175 6965 7420         if quiet 
+0000d270: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000d280: 2020 2020 2020 2020 2073 656c 662e 7175           self.qu
+0000d290: 6965 7420 3d20 7175 6965 740a 0a20 2020  iet = quiet..   
+0000d2a0: 2064 6566 2069 6e69 745f 7879 4461 7461   def init_xyData
+0000d2b0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0000d2c0: 2020 2020 2020 2020 782c 0a20 2020 2020          x,.     
+0000d2d0: 2020 2079 2c0a 2020 2020 2020 2020 6578     y,.        ex
+0000d2e0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2065  =None,.        e
+0000d2f0: 793d 312e 302c 0a20 2020 2020 2020 2065  y=1.0,.        e
+0000d300: 7265 6c78 3d4e 6f6e 652c 0a20 2020 2020  relx=None,.     
+0000d310: 2020 2065 7265 6c79 3d4e 6f6e 652c 0a20     erely=None,. 
+0000d320: 2020 2020 2020 2063 6162 7378 3d4e 6f6e         cabsx=Non
+0000d330: 652c 0a20 2020 2020 2020 2063 7265 6c78  e,.        crelx
+0000d340: 3d4e 6f6e 652c 0a20 2020 2020 2020 2063  =None,.        c
+0000d350: 6162 7379 3d4e 6f6e 652c 0a20 2020 2020  absy=None,.     
+0000d360: 2020 2063 7265 6c79 3d4e 6f6e 652c 0a20     crely=None,. 
+0000d370: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000d380: 2269 6e69 7469 616c 697a 6520 6461 7461  "initialize data
+0000d390: 206f 626a 6563 740a 0a20 2020 2020 2020   object..       
+0000d3a0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000d3b0: 202d 2020 783a 2020 2020 2020 2061 6273   -  x:       abs
+0000d3c0: 6369 7373 6120 6f66 2064 6174 6120 706f  cissa of data po
+0000d3d0: 696e 7473 2028 2278 2076 616c 7565 7322  ints ("x values"
+0000d3e0: 290a 2020 2020 2020 2020 2020 2d20 2079  ).          -  y
+0000d3f0: 3a20 2020 2020 2020 6f72 6469 6e61 7465  :       ordinate
+0000d400: 206f 6620 6461 7461 2070 6f69 6e74 7320   of data points 
+0000d410: 2822 7920 7661 6c75 6573 2229 0a20 2020  ("y values").   
+0000d420: 2020 2020 2020 202d 2020 6578 3a20 2020         -  ex:   
+0000d430: 2020 2069 6e64 6570 656e 6465 6e74 2075     independent u
+0000d440: 6e63 6572 7461 696e 7469 6573 2078 0a20  ncertainties x. 
+0000d450: 2020 2020 2020 2020 202d 2020 6579 3a20           -  ey: 
+0000d460: 2020 2020 2069 6e64 6570 656e 6465 6e74       independent
+0000d470: 2075 6e63 6572 7461 696e 7469 6573 2079   uncertainties y
+0000d480: 0a20 2020 2020 2020 2020 202d 2020 6572  .          -  er
+0000d490: 656c 783a 2020 2069 6e64 6570 656e 6465  elx:   independe
+0000d4a0: 6e74 2072 656c 6174 6976 6520 756e 6365  nt relative unce
+0000d4b0: 7274 6169 6e74 6965 7320 780a 2020 2020  rtainties x.    
+0000d4c0: 2020 2020 2020 2d20 2065 7265 6c79 3a20        -  erely: 
+0000d4d0: 2020 696e 6465 7065 6e64 656e 7420 7265    independent re
+0000d4e0: 6c61 7469 7665 2075 6e63 6572 7461 696e  lative uncertain
+0000d4f0: 7469 6573 2079 0a20 2020 2020 2020 2020  ties y.         
+0000d500: 202d 2020 6361 6273 783a 2020 2063 6f72   -  cabsx:   cor
+0000d510: 7265 6c61 7465 6420 6162 6f6c 7574 6520  related abolute 
+0000d520: 756e 6365 7274 6169 6e74 6965 7320 780a  uncertainties x.
+0000d530: 2020 2020 2020 2020 2020 2d20 2063 7265            -  cre
+0000d540: 6c78 3a20 2020 636f 7272 656c 6174 6564  lx:   correlated
+0000d550: 2072 656c 6174 6976 6520 756e 6365 7274   relative uncert
+0000d560: 6169 6e74 6965 7320 780a 2020 2020 2020  ainties x.      
+0000d570: 2020 2020 2d20 2063 6162 7379 3a20 2020      -  cabsy:   
+0000d580: 636f 7272 656c 6174 6564 2061 6273 6f6c  correlated absol
+0000d590: 7574 6520 756e 6365 7274 6169 6e74 6965  ute uncertaintie
+0000d5a0: 7320 790a 2020 2020 2020 2020 2020 2d20  s y.          - 
+0000d5b0: 2063 7265 6c79 3a20 2020 636f 7272 656c   crely:   correl
+0000d5c0: 6174 6564 2072 656c 6174 6976 6520 756e  ated relative un
+0000d5d0: 6365 7274 6169 6e74 6965 7320 790a 2020  certainties y.  
+0000d5e0: 2020 2020 2020 2020 2d20 2071 7569 6574          -  quiet
+0000d5f0: 3a20 2020 6e6f 2069 6e66 6f72 6d61 7469  :   no informati
+0000d600: 7665 2070 7269 6e74 6f75 7420 6966 2054  ve printout if T
+0000d610: 7275 650a 2020 2020 2020 2020 2222 220a  rue.        """.
+0000d620: 0a20 2020 2020 2020 2023 2063 7265 6174  .        # creat
+0000d630: 6520 6461 7461 206f 626a 6563 7420 616e  e data object an
+0000d640: 6420 7061 7373 2061 6c6c 2069 6e70 7574  d pass all input
+0000d650: 2061 7267 756d 656e 7473 0a20 2020 2020   arguments.     
+0000d660: 2020 2073 656c 662e 7879 4461 7461 203d     self.xyData =
+0000d670: 2073 656c 662e 7879 4461 7461 436f 6e74   self.xyDataCont
+0000d680: 6169 6e65 7228 0a20 2020 2020 2020 2020  ainer(.         
+0000d690: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0000d6a0: 2020 2020 2078 2c0a 2020 2020 2020 2020       x,.        
+0000d6b0: 2020 2020 792c 0a20 2020 2020 2020 2020      y,.         
+0000d6c0: 2020 2065 782c 0a20 2020 2020 2020 2020     ex,.         
+0000d6d0: 2020 2065 792c 0a20 2020 2020 2020 2020     ey,.         
+0000d6e0: 2020 2065 7265 6c78 2c0a 2020 2020 2020     erelx,.      
+0000d6f0: 2020 2020 2020 6572 656c 792c 0a20 2020        erely,.   
+0000d700: 2020 2020 2020 2020 2063 6162 7378 2c0a           cabsx,.
+0000d710: 2020 2020 2020 2020 2020 2020 6372 656c              crel
+0000d720: 782c 0a20 2020 2020 2020 2020 2020 2063  x,.            c
+0000d730: 6162 7379 2c0a 2020 2020 2020 2020 2020  absy,.          
+0000d740: 2020 6372 656c 792c 0a20 2020 2020 2020    crely,.       
+0000d750: 2020 2020 2071 7569 6574 3d73 656c 662e       quiet=self.
+0000d760: 7175 6965 742c 0a20 2020 2020 2020 2029  quiet,.        )
+0000d770: 0a20 2020 2020 2020 2073 656c 662e 6461  .        self.da
+0000d780: 7461 203d 2073 656c 662e 7879 4461 7461  ta = self.xyData
+0000d790: 0a20 2020 2020 2020 2023 2073 6574 2066  .        # set f
+0000d7a0: 6c61 6773 2066 6f72 2073 7465 6572 696e  lags for steerin
+0000d7b0: 6720 6f66 2066 6974 2070 726f 6365 7373  g of fit process
+0000d7c0: 2069 6e20 646f 5f66 6974 2829 0a20 2020   in do_fit().   
+0000d7d0: 2020 2020 2073 656c 662e 6974 6572 6174       self.iterat
+0000d7e0: 6546 6974 203d 2073 656c 662e 7879 4461  eFit = self.xyDa
+0000d7f0: 7461 2e68 6173 5f78 4572 726f 7273 206f  ta.has_xErrors o
+0000d800: 7220 280a 2020 2020 2020 2020 2020 2020  r (.            
+0000d810: 7365 6c66 2e78 7944 6174 612e 6861 735f  self.xyData.has_
+0000d820: 7265 6c5f 7945 7272 6f72 7320 616e 6420  rel_yErrors and 
+0000d830: 7365 6c66 2e72 6566 4d6f 6465 6c0a 2020  self.refModel.  
+0000d840: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+0000d850: 2069 6e69 745f 7879 4669 7428 0a20 2020   init_xyFit(.   
+0000d860: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000d870: 2020 206d 6f64 656c 2c0a 2020 2020 2020     model,.      
+0000d880: 2020 6d6f 6465 6c5f 6b77 6172 6773 3d4e    model_kwargs=N
+0000d890: 6f6e 652c 0a20 2020 2020 2020 2070 303d  one,.        p0=
+0000d8a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6470  None,.        dp
+0000d8b0: 303d 4e6f 6e65 2c0a 2020 2020 2020 2020  0=None,.        
+0000d8c0: 636f 6e73 7472 6169 6e74 733d 4e6f 6e65  constraints=None
+0000d8d0: 2c0a 2020 2020 2020 2020 6669 7850 6172  ,.        fixPar
+0000d8e0: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+0000d8f0: 6c69 6d69 7473 3d4e 6f6e 652c 0a20 2020  limits=None,.   
+0000d900: 2029 3a0a 2020 2020 2020 2020 2222 2269   ):.        """i
+0000d910: 6e69 7469 616c 697a 6520 6669 7420 6f62  nitialize fit ob
+0000d920: 6a65 6374 0a0a 2020 2020 2020 2020 4172  ject..        Ar
+0000d930: 6773 3a0a 2020 2020 2020 2020 2020 2d20  gs:.          - 
+0000d940: 6d6f 6465 6c3a 206d 6f64 656c 2066 756e  model: model fun
+0000d950: 6374 696f 6e20 6628 783b 205c 2a70 6172  ction f(x; \*par
+0000d960: 290a 2020 2020 2020 2020 2020 2d20 6d6f  ).          - mo
+0000d970: 6465 6c5f 6b77 6172 6773 3a20 6f70 7469  del_kwargs: opti
+0000d980: 6f6e 616c 2c20 6669 7420 7061 7261 6d65  onal, fit parame
+0000d990: 7465 7273 2069 6620 6e6f 7420 6672 6f6d  ters if not from
+0000d9a0: 206d 6f64 656c 2073 6967 6e61 7475 7265   model signature
+0000d9b0: 0a20 2020 2020 2020 2020 202d 2070 303a  .          - p0:
+0000d9c0: 206e 702d 6172 7261 7920 6f66 2066 6c6f   np-array of flo
+0000d9d0: 6174 732c 2069 6e69 7469 616c 2070 6172  ats, initial par
+0000d9e0: 616d 6574 6572 2076 616c 7565 730a 2020  ameter values.  
+0000d9f0: 2020 2020 2020 2020 2d20 6470 303a 2061          - dp0: a
+0000da00: 7272 6179 2d6c 696b 652c 2069 6e69 7469  rray-like, initi
+0000da10: 616c 2067 7565 7373 206f 6620 7061 7261  al guess of para
+0000da20: 6d65 7465 7220 756e 6365 7274 6169 6e74  meter uncertaint
+0000da30: 6965 7320 286f 7074 696f 6e61 6c29 0a20  ies (optional). 
+0000da40: 2020 2020 2020 2020 202d 2063 6f6e 7374           - const
+0000da50: 7261 696e 7473 3a20 286e 6573 7465 6429  raints: (nested)
+0000da60: 206c 6973 7428 7329 3a20 5b70 6172 616d   list(s): [param
+0000da70: 6574 6572 206e 616d 652c 2076 616c 7565  eter name, value
+0000da80: 2c20 756e 6365 7274 6169 6e74 795d 0a20  , uncertainty]. 
+0000da90: 2020 2020 2020 2020 2020 206f 7220 5b70             or [p
+0000daa0: 6172 616d 6574 6572 2069 6e64 6578 2c20  arameter index, 
+0000dab0: 7661 6c75 652c 2075 6e63 6572 7461 696e  value, uncertain
+0000dac0: 7479 5d0a 2020 2020 2020 2020 2020 2d20  ty].          - 
+0000dad0: 6c69 6d69 7473 3a20 286e 6573 7465 6429  limits: (nested)
+0000dae0: 206c 6973 7428 7329 3a20 5b70 6172 616d   list(s): [param
+0000daf0: 6574 6572 206e 616d 652c 206d 696e 2c20  eter name, min, 
+0000db00: 6d61 785d 0a20 2020 2020 2020 2020 2020  max].           
+0000db10: 206f 7220 5b70 6172 616d 6574 6572 2069   or [parameter i
+0000db20: 6e64 6578 2c20 6d69 6e2c 206d 6178 5d0a  ndex, min, max].
+0000db30: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0000db40: 2020 2020 2069 6620 7365 6c66 2e78 7944       if self.xyD
+0000db50: 6174 6120 6973 204e 6f6e 653a 0a20 2020  ata is None:.   
+0000db60: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000db70: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+0000db80: 2020 2020 2020 2020 2020 2022 2021 2121             " !!!
+0000db90: 206d 6e46 6974 2e69 6e69 745f 7879 4669   mnFit.init_xyFi
+0000dba0: 743a 206e 6f20 6461 7461 206f 626a 6563  t: no data objec
+0000dbb0: 7420 6465 6669 6e65 6420 2d20 6361 6c6c  t defined - call
+0000dbc0: 2069 6e69 745f 6461 7461 2829 220a 2020   init_data()".  
+0000dbd0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000dbe0: 2020 2020 2023 2067 6574 2070 6172 616d       # get param
+0000dbf0: 6574 6572 7320 6f66 206d 6f64 656c 2066  eters of model f
+0000dc00: 756e 6374 696f 6e20 746f 2073 6574 2073  unction to set s
+0000dc10: 7461 7274 2076 616c 7565 7320 666f 7220  tart values for 
+0000dc20: 6669 740a 2020 2020 2020 2020 6966 206d  fit.        if m
+0000dc30: 6f64 656c 5f6b 7761 7267 7320 6973 204e  odel_kwargs is N
+0000dc40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000dc50: 2061 7267 732c 206d 6f64 656c 5f6b 7761   args, model_kwa
+0000dc60: 7267 7320 3d20 6765 745f 6675 6e63 7469  rgs = get_functi
+0000dc70: 6f6e 5369 676e 6174 7572 6528 6d6f 6465  onSignature(mode
+0000dc80: 6c29 0a0a 2020 2020 2020 2020 7061 7220  l)..        par 
+0000dc90: 3d20 286d 6f64 656c 5f6b 7761 7267 732c  = (model_kwargs,
+0000dca0: 2070 302c 2064 7030 2c20 636f 6e73 7472   p0, dp0, constr
+0000dcb0: 6169 6e74 732c 2066 6978 5061 7273 2c20  aints, fixPars, 
+0000dcc0: 6c69 6d69 7473 290a 2020 2020 2020 2020  limits).        
+0000dcd0: 7365 6c66 2e5f 7365 7475 7046 6974 5061  self._setupFitPa
+0000dce0: 7261 6d65 7465 7273 282a 7061 7229 0a0a  rameters(*par)..
+0000dcf0: 2020 2020 2020 2020 2320 6372 6561 7465          # create
+0000dd00: 2063 6f73 7420 6675 6e63 7469 6f6e 0a20   cost function. 
+0000dd10: 2020 2020 2020 2073 656c 662e 636f 7374         self.cost
+0000dd20: 6620 3d20 7365 6c66 2e78 4c53 7143 6f73  f = self.xLSqCos
+0000dd30: 7428 7365 6c66 2c20 6d6f 6465 6c2c 2075  t(self, model, u
+0000dd40: 7365 5f6e 6567 326c 6f67 4c3d 7365 6c66  se_neg2logL=self
+0000dd50: 2e75 7365 5f6e 6567 4c6f 674c 290a 2020  .use_negLogL).  
+0000dd60: 2020 2020 2020 7365 6c66 2e5f 7365 7475        self._setu
+0000dd70: 704d 696e 7569 7428 6d6f 6465 6c5f 6b77  pMinuit(model_kw
+0000dd80: 6172 6773 290a 0a20 2020 2063 6c61 7373  args)..    class
+0000dd90: 2078 7944 6174 6143 6f6e 7461 696e 6572   xyDataContainer
+0000dda0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000ddb0: 2020 2020 2020 4861 6e64 6c65 2064 6174        Handle dat
+0000ddc0: 6120 616e 6420 756e 6365 7274 6169 6e74  a and uncertaint
+0000ddd0: 6965 7320 616e 640a 2020 2020 2020 2020  ies and.        
+0000dde0: 6275 696c 6420 636f 7661 7269 616e 6365  build covariance
+0000ddf0: 206d 6174 7269 6365 7320 6672 6f6d 2063   matrices from c
+0000de00: 6f6d 706f 6e65 6e74 730a 0a20 2020 2020  omponents..     
+0000de10: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000de20: 2020 202d 206f 7574 6572 3a20 2020 706f     - outer:   po
+0000de30: 696e 7465 7220 746f 2069 6e73 7461 6e63  inter to instanc
+0000de40: 6520 6f66 2063 616c 6c69 6e67 206f 626a  e of calling obj
+0000de50: 6563 740a 2020 2020 2020 2020 2020 2d20  ect.          - 
+0000de60: 783a 2020 2020 2020 2061 6273 6369 7373  x:       absciss
+0000de70: 6120 6f66 2064 6174 6120 706f 696e 7473  a of data points
+0000de80: 2028 2278 2076 616c 7565 7322 290a 2020   ("x values").  
+0000de90: 2020 2020 2020 2020 2d20 793a 2020 2020          - y:    
+0000dea0: 2020 206f 7264 696e 6174 6520 6f66 2064     ordinate of d
+0000deb0: 6174 6120 706f 696e 7473 2028 2279 2076  ata points ("y v
+0000dec0: 616c 7565 7322 290a 2020 2020 2020 2020  alues").        
+0000ded0: 2020 2d20 6578 3a20 2020 2020 2069 6e64    - ex:      ind
+0000dee0: 6570 656e 6465 6e74 2075 6e63 6572 7461  ependent uncerta
+0000def0: 696e 7469 6573 2078 0a20 2020 2020 2020  inties x.       
+0000df00: 2020 202d 2065 793a 2020 2020 2020 696e     - ey:      in
+0000df10: 6465 7065 6e64 656e 7420 756e 6365 7274  dependent uncert
+0000df20: 6169 6e74 6965 7320 790a 2020 2020 2020  ainties y.      
+0000df30: 2020 2020 2d20 6572 656c 783a 2020 2069      - erelx:   i
+0000df40: 6e64 6570 656e 6465 6e74 2072 656c 6174  ndependent relat
+0000df50: 6976 6520 756e 6365 7274 6169 6e74 6965  ive uncertaintie
+0000df60: 7320 780a 2020 2020 2020 2020 2020 2d20  s x.          - 
+0000df70: 6572 656c 793a 2020 2069 6e64 6570 656e  erely:   indepen
+0000df80: 6465 6e74 2072 656c 6174 6976 6520 756e  dent relative un
+0000df90: 6365 7274 6169 6e74 6965 7320 790a 2020  certainties y.  
+0000dfa0: 2020 2020 2020 2020 2d20 6361 6273 783a          - cabsx:
+0000dfb0: 2020 2063 6f72 7265 6c61 7465 6420 6162     correlated ab
+0000dfc0: 6f6c 7574 6520 756e 6365 7274 6169 6e74  olute uncertaint
+0000dfd0: 6965 7320 780a 2020 2020 2020 2020 2020  ies x.          
+0000dfe0: 2d20 6372 656c 783a 2020 2063 6f72 7265  - crelx:   corre
+0000dff0: 6c61 7465 6420 7265 6c61 7469 7665 2075  lated relative u
+0000e000: 6e63 6572 7461 696e 7469 6573 2078 0a20  ncertainties x. 
+0000e010: 2020 2020 2020 2020 202d 2063 6162 7379           - cabsy
+0000e020: 3a20 2020 636f 7272 656c 6174 6564 2061  :   correlated a
+0000e030: 6273 6f6c 7574 6520 756e 6365 7274 6169  bsolute uncertai
+0000e040: 6e74 6965 7320 790a 2020 2020 2020 2020  nties y.        
+0000e050: 2020 2d20 6372 656c 793a 2020 2063 6f72    - crely:   cor
+0000e060: 7265 6c61 7465 6420 7265 6c61 7469 7665  related relative
+0000e070: 2075 6e63 6572 7461 696e 7469 6573 2079   uncertainties y
+0000e080: 0a20 2020 2020 2020 2020 202d 2071 7569  .          - qui
+0000e090: 6574 3a20 2020 6e6f 2069 6e66 6f72 6d61  et:   no informa
+0000e0a0: 7469 7665 2070 7269 6e74 6f75 7420 6966  tive printout if
+0000e0b0: 2054 7275 650a 0a20 2020 2020 2020 2050   True..        P
+0000e0c0: 7562 6c69 6320 6d65 7468 6f64 733a 0a20  ublic methods:. 
+0000e0d0: 2020 2020 2020 2020 202d 2069 6e69 745f           - init_
+0000e0e0: 6479 6e61 6d69 6345 7272 6f72 7328 293a  dynamicErrors():
+0000e0f0: 0a20 2020 2020 2020 2020 202d 2067 6574  .          - get
+0000e100: 5f43 6f76 2829 3a20 6669 6e61 6c20 636f  _Cov(): final co
+0000e110: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
+0000e120: 2869 6e63 6c2e 2070 726f 6a2e 2078 290a  (incl. proj. x).
+0000e130: 2020 2020 2020 2020 2020 2d20 6765 745f            - get_
+0000e140: 7843 6f76 2829 3a20 636f 7661 7269 616e  xCov(): covarian
+0000e150: 6365 206f 6620 782d 7661 6c75 6573 0a20  ce of x-values. 
+0000e160: 2020 2020 2020 2020 202d 2067 6574 5f79           - get_y
+0000e170: 436f 7628 293a 2063 6f76 6172 6961 6e63  Cov(): covarianc
+0000e180: 6520 6f66 2079 2d76 616c 7565 730a 2020  e of y-values.  
+0000e190: 2020 2020 2020 2020 2d20 6765 745f 6943          - get_iC
+0000e1a0: 6f76 2829 3a20 696e 7665 7273 6520 636f  ov(): inverse co
+0000e1b0: 7661 7269 616e 6365 206d 6174 7269 780a  variance matrix.
+0000e1c0: 2020 2020 2020 2020 2020 2d20 706c 6f74            - plot
+0000e1d0: 2829 3a20 7072 6f76 6964 6520 6120 6669  (): provide a fi
+0000e1e0: 6775 7265 2077 6974 6820 7265 7072 6573  gure with repres
+0000e1f0: 656e 7461 7469 6f6e 206f 6620 6461 7461  entation of data
+0000e200: 0a0a 2020 2020 2020 2020 4461 7461 206d  ..        Data m
+0000e210: 656d 6265 7273 3a0a 2020 2020 2020 2020  embers:.        
+0000e220: 2020 2a20 636f 7079 206f 6620 616c 6c20    * copy of all 
+0000e230: 696e 7075 7420 6172 6775 6d65 6e74 730a  input arguments.
+0000e240: 2020 2020 2020 2020 2020 2a20 636f 7678            * covx
+0000e250: 3a20 636f 7661 7269 616e 6365 206d 6174  : covariance mat
+0000e260: 7269 7820 6f66 2078 0a20 2020 2020 2020  rix of x.       
+0000e270: 2020 202a 2063 6f76 793a 2063 6f76 6172     * covy: covar
+0000e280: 6961 6e63 6520 6d61 7472 6978 206f 6620  iance matrix of 
+0000e290: 7920 756e 6365 7274 6169 6e74 6965 730a  y uncertainties.
+0000e2a0: 2020 2020 2020 2020 2020 2a20 636f 763a            * cov:
+0000e2b0: 2066 756c 6c20 636f 7661 7269 616e 6365   full covariance
+0000e2c0: 206d 6174 7269 7820 696e 636c 2e20 7072   matrix incl. pr
+0000e2d0: 6f6a 6563 7465 6420 780a 2020 2020 2020  ojected x.      
+0000e2e0: 2020 2020 2a20 6943 6f76 3a20 696e 7665      * iCov: inve
+0000e2f0: 7273 6520 6f66 2063 6f76 6172 6961 6e63  rse of covarianc
+0000e300: 6520 6d61 7472 6978 0a20 2020 2020 2020  e matrix.       
+0000e310: 2022 2222 0a0a 2020 2020 2020 2020 6465   """..        de
+0000e320: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+0000e330: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000e340: 2020 2020 2020 2020 2020 6f75 7465 722c            outer,
+0000e350: 0a20 2020 2020 2020 2020 2020 2078 2c0a  .            x,.
+0000e360: 2020 2020 2020 2020 2020 2020 792c 0a20              y,. 
+0000e370: 2020 2020 2020 2020 2020 2065 782c 0a20             ex,. 
+0000e380: 2020 2020 2020 2020 2020 2065 792c 0a20             ey,. 
+0000e390: 2020 2020 2020 2020 2020 2065 7265 6c78             erelx
+0000e3a0: 2c0a 2020 2020 2020 2020 2020 2020 6572  ,.            er
+0000e3b0: 656c 792c 0a20 2020 2020 2020 2020 2020  ely,.           
+0000e3c0: 2063 6162 7378 2c0a 2020 2020 2020 2020   cabsx,.        
+0000e3d0: 2020 2020 6372 656c 782c 0a20 2020 2020      crelx,.     
+0000e3e0: 2020 2020 2020 2063 6162 7379 2c0a 2020         cabsy,.  
+0000e3f0: 2020 2020 2020 2020 2020 6372 656c 792c            crely,
+0000e400: 0a20 2020 2020 2020 2020 2020 2071 7569  .            qui
+0000e410: 6574 3d54 7275 652c 0a20 2020 2020 2020  et=True,.       
+0000e420: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000e430: 2320 7361 7665 2070 6f69 6e65 7220 746f  # save poiner to
+0000e440: 2063 616c 6c69 6e67 2063 6c61 7373 0a20   calling class. 
+0000e450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000e460: 6f75 7465 7220 3d20 6f75 7465 720a 0a20  outer = outer.. 
+0000e470: 2020 2020 2020 2020 2020 2023 2061 7373             # ass
+0000e480: 756d 6520 7369 6d70 6c65 2063 6173 6520  ume simple case 
+0000e490: 772e 6f2e 2063 6f76 2e6d 6174 2e0a 2020  w.o. cov.mat..  
+0000e4a0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+0000e4b0: 6565 6473 5f63 6f76 6172 6961 6e63 6520  eeds_covariance 
+0000e4c0: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
+0000e4d0: 2020 2020 206e 6420 3d20 6c65 6e28 7829       nd = len(x)
+0000e4e0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
+0000e4f0: 746f 7265 2069 6e70 7574 2064 6174 6120  tore input data 
+0000e500: 6173 206e 756d 7079 2066 6c6f 6174 2061  as numpy float a
+0000e510: 7272 6179 732c 2065 6e73 7572 6520 6c65  rrays, ensure le
+0000e520: 6e67 7468 206e 6420 6966 206e 6565 6465  ngth nd if neede
+0000e530: 640a 2020 2020 2020 2020 2020 2020 7365  d.            se
+0000e540: 6c66 2e64 6c65 6e67 7468 203d 206e 640a  lf.dlength = nd.
+0000e550: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e560: 2e78 203d 206e 702e 6173 6661 7272 6179  .x = np.asfarray
+0000e570: 2878 2920 2023 2061 6273 6369 7373 6120  (x)  # abscissa 
+0000e580: 2d20 2278 2076 616c 7565 7322 0a20 2020  - "x values".   
+0000e590: 2020 2020 2020 2020 2073 656c 662e 7920           self.y 
+0000e5a0: 3d20 6e70 2e61 7366 6172 7261 7928 7929  = np.asfarray(y)
+0000e5b0: 2020 2320 6f72 6469 6e61 7465 202d 2022    # ordinate - "
+0000e5c0: 7920 7661 6c75 6573 220a 2020 2020 2020  y values".      
+0000e5d0: 2020 2020 2020 6966 2065 7820 6973 206e        if ex is n
+0000e5e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0000e5f0: 2020 2020 2020 2020 2073 656c 662e 6578           self.ex
+0000e600: 203d 206e 702e 6173 6661 7272 6179 2865   = np.asfarray(e
+0000e610: 7829 2020 2320 696e 6465 7065 6e64 656e  x)  # independen
+0000e620: 7420 756e 6365 7274 6169 6e74 6965 7320  t uncertainties 
+0000e630: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+0000e640: 2020 6966 2073 656c 662e 6578 2e6e 6469    if self.ex.ndi
+0000e650: 6d20 3d3d 2030 3a0a 2020 2020 2020 2020  m == 0:.        
+0000e660: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e670: 2e65 7820 3d20 7365 6c66 2e65 7820 2a20  .ex = self.ex * 
+0000e680: 6e70 2e6f 6e65 7328 6e64 290a 2020 2020  np.ones(nd).    
+0000e690: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000e6a0: 2073 656c 662e 6578 2e6e 6469 6d20 3d3d   self.ex.ndim ==
+0000e6b0: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+0000e6c0: 2020 2020 2020 2020 7365 6c66 2e6e 6565          self.nee
+0000e6d0: 6473 5f63 6f76 6172 6961 6e63 6520 3d20  ds_covariance = 
+0000e6e0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0000e6f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000e700: 2020 2020 2020 2073 656c 662e 6578 203d         self.ex =
+0000e710: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+0000e720: 2020 6966 2065 7920 6973 206e 6f74 204e    if ey is not N
+0000e730: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000e740: 2020 2020 2073 656c 662e 6579 203d 206e       self.ey = n
+0000e750: 702e 6173 6661 7272 6179 2865 7929 2020  p.asfarray(ey)  
+0000e760: 2320 696e 6465 7065 6e64 656e 7420 756e  # independent un
+0000e770: 6365 7274 6169 6e74 6965 7320 790a 2020  certainties y.  
+0000e780: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000e790: 2073 656c 662e 6579 2e6e 6469 6d20 3d3d   self.ey.ndim ==
+0000e7a0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000e7b0: 2020 2020 2020 2020 7365 6c66 2e65 7920          self.ey 
+0000e7c0: 3d20 7365 6c66 2e65 7920 2a20 6e70 2e6f  = self.ey * np.o
+0000e7d0: 6e65 7328 6e64 290a 2020 2020 2020 2020  nes(nd).        
+0000e7e0: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+0000e7f0: 662e 6579 2e6e 6469 6d20 3d3d 2032 3a0a  f.ey.ndim == 2:.
+0000e800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e810: 2020 2020 7365 6c66 2e6e 6565 6473 5f63      self.needs_c
+0000e820: 6f76 6172 6961 6e63 6520 3d20 5472 7565  ovariance = True
+0000e830: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000e840: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000e850: 2020 2073 656c 662e 6579 203d 204e 6f6e     self.ey = Non
+0000e860: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+0000e870: 2065 7265 6c78 2069 7320 6e6f 7420 4e6f   erelx is not No
+0000e880: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000e890: 2020 2020 7365 6c66 2e65 7265 6c78 203d      self.erelx =
+0000e8a0: 206e 702e 6173 6661 7272 6179 2865 7265   np.asfarray(ere
+0000e8b0: 6c78 2920 2023 2069 6e64 6570 656e 6465  lx)  # independe
+0000e8c0: 6e74 2072 656c 6174 6976 6520 756e 6365  nt relative unce
+0000e8d0: 7274 6169 6e74 6965 7320 780a 2020 2020  rtainties x.    
+0000e8e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000e8f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000e900: 6c66 2e65 7265 6c78 203d 204e 6f6e 650a  lf.erelx = None.
+0000e910: 2020 2020 2020 2020 2020 2020 6966 2065              if e
+0000e920: 7265 6c79 2069 7320 6e6f 7420 4e6f 6e65  rely is not None
+0000e930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e940: 2020 7365 6c66 2e65 7265 6c79 203d 206e    self.erely = n
+0000e950: 702e 6173 6661 7272 6179 2865 7265 6c79  p.asfarray(erely
+0000e960: 2920 2023 2069 6e64 6570 656e 6465 6e74  )  # independent
+0000e970: 2072 656c 6174 6976 6520 756e 6365 7274   relative uncert
+0000e980: 6169 6e74 6965 7320 790a 2020 2020 2020  ainties y.      
+0000e990: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000e9a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000e9b0: 2e65 7265 6c79 203d 204e 6f6e 650a 2020  .erely = None.  
+0000e9c0: 2020 2020 2020 2020 2020 6966 2063 6162            if cab
+0000e9d0: 7378 2069 7320 6e6f 7420 4e6f 6e65 3a0a  sx is not None:.
+0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9f0: 7365 6c66 2e63 6162 7378 203d 206e 702e  self.cabsx = np.
+0000ea00: 6173 6661 7272 6179 2863 6162 7378 2920  asfarray(cabsx) 
+0000ea10: 2023 2063 6f72 7265 6c61 7465 6420 6162   # correlated ab
+0000ea20: 6f6c 7574 6520 756e 6365 7274 6169 6e74  olute uncertaint
+0000ea30: 6965 7320 780a 2020 2020 2020 2020 2020  ies x.          
+0000ea40: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
+0000ea50: 6273 782e 6e64 696d 203d 3d20 303a 0a20  bsx.ndim == 0:. 
+0000ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea70: 2020 2073 656c 662e 6361 6273 7820 3d20     self.cabsx = 
+0000ea80: 7365 6c66 2e63 6162 7378 202a 206e 702e  self.cabsx * np.
+0000ea90: 6f6e 6573 286e 6429 0a20 2020 2020 2020  ones(nd).       
+0000eaa0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000eab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000eac0: 6361 6273 7820 3d20 4e6f 6e65 0a20 2020  cabsx = None.   
+0000ead0: 2020 2020 2020 2020 2069 6620 6372 656c           if crel
+0000eae0: 7820 6973 206e 6f74 204e 6f6e 653a 0a20  x is not None:. 
+0000eaf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000eb00: 656c 662e 6372 656c 7820 3d20 6e70 2e61  elf.crelx = np.a
+0000eb10: 7366 6172 7261 7928 6372 656c 7829 2020  sfarray(crelx)  
+0000eb20: 2320 636f 7272 656c 6174 6564 2072 656c  # correlated rel
+0000eb30: 6174 6976 6520 756e 6365 7274 6169 6e74  ative uncertaint
+0000eb40: 6965 7320 780a 2020 2020 2020 2020 2020  ies x.          
+0000eb50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000eb60: 2020 2020 2020 2020 7365 6c66 2e63 7265          self.cre
+0000eb70: 6c78 203d 204e 6f6e 650a 2020 2020 2020  lx = None.      
+0000eb80: 2020 2020 2020 6966 2063 6162 7379 2069        if cabsy i
+0000eb90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000eba0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ebb0: 2e63 6162 7379 203d 206e 702e 6173 6661  .cabsy = np.asfa
+0000ebc0: 7272 6179 2863 6162 7379 2920 2023 2063  rray(cabsy)  # c
+0000ebd0: 6f72 7265 6c61 7465 6420 6162 736f 6c75  orrelated absolu
+0000ebe0: 7465 2075 6e63 6572 7461 696e 7469 6573  te uncertainties
+0000ebf0: 2079 0a20 2020 2020 2020 2020 2020 2020   y.             
+0000ec00: 2020 2069 6620 7365 6c66 2e63 6162 7379     if self.cabsy
+0000ec10: 2e6e 6469 6d20 3d3d 2030 3a0a 2020 2020  .ndim == 0:.    
+0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec30: 7365 6c66 2e63 6162 7379 203d 2073 656c  self.cabsy = sel
+0000ec40: 662e 6361 6273 7920 2a20 6e70 2e6f 6e65  f.cabsy * np.one
+0000ec50: 7328 6e64 290a 2020 2020 2020 2020 2020  s(nd).          
+0000ec60: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000ec70: 2020 2020 2020 2020 7365 6c66 2e63 6162          self.cab
+0000ec80: 7379 203d 204e 6f6e 650a 2020 2020 2020  sy = None.      
+0000ec90: 2020 2020 2020 6966 2063 7265 6c79 2069        if crely i
+0000eca0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0000ecb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ecc0: 2e63 7265 6c79 203d 206e 702e 6173 6661  .crely = np.asfa
+0000ecd0: 7272 6179 2863 7265 6c79 2920 2023 2063  rray(crely)  # c
+0000ece0: 6f72 7265 6c61 7465 6420 7265 6c61 7469  orrelated relati
+0000ecf0: 7665 2075 6e63 6572 7461 696e 7469 6573  ve uncertainties
+0000ed00: 2079 0a20 2020 2020 2020 2020 2020 2065   y.            e
+0000ed10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000ed20: 2020 2020 2073 656c 662e 6372 656c 7920       self.crely 
+0000ed30: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000ed40: 2020 2073 656c 662e 7175 6965 7420 3d20     self.quiet = 
+0000ed50: 7175 6965 7420 2023 206e 6f20 696e 666f  quiet  # no info
+0000ed60: 726d 6174 6976 6520 7072 696e 746f 7574  rmative printout
+0000ed70: 2069 6620 5472 7565 0a0a 2020 2020 2020   if True..      
+0000ed80: 2020 2020 2020 7365 6c66 2e6e 6420 3d20        self.nd = 
+0000ed90: 6e64 0a20 2020 2020 2020 2020 2020 2073  nd.            s
+0000eda0: 656c 662e 6d6f 6465 6c20 3d20 4e6f 6e65  elf.model = None
+0000edb0: 2020 2320 6e6f 206d 6f64 656c 2064 6566    # no model def
+0000edc0: 696e 6564 2079 6574 0a20 2020 2020 2020  ined yet.       
+0000edd0: 2020 2020 2073 656c 662e 6d6f 6465 6c5f       self.model_
+0000ede0: 7661 6c75 6573 203d 204e 6f6e 650a 0a20  values = None.. 
+0000edf0: 2020 2020 2020 2020 2020 2023 2073 6574             # set
+0000ee00: 2066 6c61 6773 2066 6f72 2073 7465 6572   flags for steer
+0000ee10: 696e 6720 6f66 2066 6974 2070 726f 6365  ing of fit proce
+0000ee20: 7373 2069 6e20 646f 5f66 6974 2829 0a20  ss in do_fit(). 
+0000ee30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000ee40: 7265 6275 6c69 6c64 436f 7620 3d20 4e6f  rebulildCov = No
+0000ee50: 6e65 0a20 2020 2020 2020 2020 2020 2073  ne.            s
+0000ee60: 656c 662e 6861 735f 7845 7272 6f72 7320  elf.has_xErrors 
+0000ee70: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0000ee80: 2020 2020 6578 2069 7320 6e6f 7420 4e6f      ex is not No
+0000ee90: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+0000eea0: 2020 206f 7220 6572 656c 7820 6973 206e     or erelx is n
+0000eeb0: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+0000eec0: 2020 2020 2020 2020 6f72 2063 6162 7378          or cabsx
+0000eed0: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+0000eee0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
+0000eef0: 6372 656c 7820 6973 206e 6f74 204e 6f6e  crelx is not Non
+0000ef00: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
+0000ef10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ef20: 2e68 6173 5f72 656c 5f79 4572 726f 7273  .has_rel_yErrors
+0000ef30: 203d 2065 7265 6c79 2069 7320 6e6f 7420   = erely is not 
+0000ef40: 4e6f 6e65 206f 7220 6372 656c 7920 6973  None or crely is
+0000ef50: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+0000ef60: 2020 2020 2020 7365 6c66 2e6e 6565 6473        self.needs
+0000ef70: 5f63 6f76 6172 6961 6e63 6520 3d20 280a  _covariance = (.
+0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef90: 7365 6c66 2e6e 6565 6473 5f63 6f76 6172  self.needs_covar
+0000efa0: 6961 6e63 650a 2020 2020 2020 2020 2020  iance.          
+0000efb0: 2020 2020 2020 6f72 2073 656c 662e 6361        or self.ca
+0000efc0: 6273 7820 6973 206e 6f74 204e 6f6e 650a  bsx is not None.
+0000efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efe0: 6f72 2073 656c 662e 6372 656c 7820 6973  or self.crelx is
+0000eff0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+0000f000: 2020 2020 2020 2020 2020 6f72 2073 656c            or sel
+0000f010: 662e 6361 6273 7920 6973 206e 6f74 204e  f.cabsy is not N
+0000f020: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000f030: 2020 2020 6f72 2073 656c 662e 6372 656c      or self.crel
+0000f040: 7920 6973 206e 6f74 204e 6f6e 650a 2020  y is not None.  
+0000f050: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000f060: 2020 2020 2020 2020 2023 2062 7569 6c64           # build
+0000f070: 2028 696e 6974 6961 6c29 2063 6f76 6172   (initial) covar
+0000f080: 6961 6e63 6520 6d61 7472 6978 2028 7769  iance matrix (wi
+0000f090: 7468 6f75 7420 782d 6572 726f 7273 290a  thout x-errors).
+0000f0a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000f0b0: 656c 662e 6e65 6564 735f 636f 7661 7269  elf.needs_covari
+0000f0c0: 616e 6365 3a0a 2020 2020 2020 2020 2020  ance:.          
+0000f0d0: 2020 2020 2020 6572 7232 203d 205f 6275        err2 = _bu
+0000f0e0: 696c 645f 436f 764d 6174 280a 2020 2020  ild_CovMat(.    
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f100: 7365 6c66 2e6e 642c 2073 656c 662e 6579  self.nd, self.ey
+0000f110: 2c20 7365 6c66 2e65 7265 6c79 2c20 7365  , self.erely, se
+0000f120: 6c66 2e63 6162 7379 2c20 7365 6c66 2e63  lf.cabsy, self.c
+0000f130: 7265 6c79 2c20 7365 6c66 2e79 0a20 2020  rely, self.y.   
+0000f140: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000f150: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000f160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f170: 2065 7272 3220 3d20 5f62 7569 6c64 5f45   err2 = _build_E
+0000f180: 7272 3228 7365 6c66 2e65 792c 2073 656c  rr2(self.ey, sel
+0000f190: 662e 6572 656c 792c 2073 656c 662e 7929  f.erely, self.y)
+0000f1a0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000f1b0: 696e 6974 6961 6c69 7a65 2075 6e63 6572  initialize uncer
+0000f1c0: 7461 696e 7469 6573 2061 6e64 2063 6f76  tainties and cov
+0000f1d0: 6172 6961 6e63 6520 6d61 7472 6978 2c0a  ariance matrix,.
+0000f1e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f1f0: 2e5f 696e 6974 6961 6c43 6f76 2865 7272  ._initialCov(err
+0000f200: 3229 0a20 2020 2020 2020 2020 2020 2023  2).            #
+0000f210: 2073 6574 733a 0a20 2020 2020 2020 2020   sets:.         
+0000f220: 2020 2023 2020 2073 656c 662e 636f 7678     #   self.covx
+0000f230: 3a20 636f 7661 7269 616e 6365 206d 6174  : covariance mat
+0000f240: 7269 7820 6f66 2078 0a20 2020 2020 2020  rix of x.       
+0000f250: 2020 2020 2023 2020 2073 656c 662e 636f       #   self.co
+0000f260: 7679 3a20 636f 7661 7269 616e 6365 206d  vy: covariance m
+0000f270: 6174 7269 7820 6f66 2079 2075 6e63 6572  atrix of y uncer
+0000f280: 7461 696e 7469 6573 0a20 2020 2020 2020  tainties.       
+0000f290: 2020 2020 2023 2020 2073 656c 662e 636f       #   self.co
+0000f2a0: 763a 2066 756c 6c20 636f 7661 7269 616e  v: full covarian
+0000f2b0: 6365 206d 6174 7269 7820 696e 636c 2e20  ce matrix incl. 
+0000f2c0: 7072 6f6a 6563 7465 6420 780a 2020 2020  projected x.    
+0000f2d0: 2020 2020 2020 2020 2320 2020 7365 6c66          #   self
+0000f2e0: 2e69 436f 763a 2069 6e76 6572 7365 206f  .iCov: inverse o
+0000f2f0: 6620 636f 7661 7269 616e 6365 206d 6174  f covariance mat
+0000f300: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
+0000f310: 2320 2020 7365 6c66 2e65 7272 323a 2061  #   self.err2: a
+0000f320: 7272 6179 206f 6620 7371 7561 7265 6420  rray of squared 
+0000f330: 756e 6365 7274 6169 6e74 6965 730a 2020  uncertainties.  
+0000f340: 2020 2020 2020 2020 2020 2320 2020 7365            #   se
+0000f350: 6c66 2e69 4572 7232 3a20 312e 2f73 656c  lf.iErr2: 1./sel
+0000f360: 662e 6572 7232 0a0a 2020 2020 2020 2020  f.err2..        
+0000f370: 6465 6620 5f69 6e69 7469 616c 436f 7628  def _initialCov(
+0000f380: 7365 6c66 2c20 6572 7232 293a 0a20 2020  self, err2):.   
+0000f390: 2020 2020 2020 2020 2022 2222 4275 696c           """Buil
+0000f3a0: 6420 696e 6974 6961 6c20 2873 7461 7469  d initial (stati
+0000f3b0: 6329 2063 6f76 6172 6961 6e63 6520 6d61  c) covariance ma
+0000f3c0: 7472 6978 2066 6f72 2079 2d65 7272 6f72  trix for y-error
+0000f3d0: 730a 2020 2020 2020 2020 2020 2020 2866  s.            (f
+0000f3e0: 6f72 2070 7265 2d66 6974 2920 616e 6420  or pre-fit) and 
+0000f3f0: 6361 6c63 756c 6174 6520 696e 7665 7273  calculate invers
+0000f400: 6520 6d61 7472 6978 0a20 2020 2020 2020  e matrix.       
+0000f410: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f420: 2020 2020 2069 6620 6572 7232 2e6e 6469       if err2.ndi
+0000f430: 6d20 3d3d 2032 3a0a 2020 2020 2020 2020  m == 2:.        
+0000f440: 2020 2020 2020 2020 2320 676f 7420 6120          # got a 
+0000f450: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+0000f460: 782c 206e 6565 6420 696e 7665 7273 650a  x, need inverse.
+0000f470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f480: 7365 6c66 2e6e 6565 6473 5f63 6f76 6172  self.needs_covar
+0000f490: 6961 6e63 6520 3d20 5472 7565 0a20 2020  iance = True.   
+0000f4a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f4b0: 662e 636f 7679 203d 2065 7272 320a 2020  f.covy = err2.  
+0000f4c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f4d0: 6c66 2e69 436f 7620 3d20 6c69 6e61 6c67  lf.iCov = linalg
+0000f4e0: 2e69 6e76 2865 7272 3229 0a20 2020 2020  .inv(err2).     
+0000f4f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f500: 6572 7232 203d 206e 702e 6469 6167 6f6e  err2 = np.diagon
+0000f510: 616c 2865 7272 3229 2020 2320 7371 7561  al(err2)  # squa
+0000f520: 7265 6420 6469 6167 6f6e 616c 2065 6c65  red diagonal ele
+0000f530: 6d65 6e74 730a 2020 2020 2020 2020 2020  ments.          
+0000f540: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000f550: 2020 2020 2020 2020 2320 676f 7420 696e          # got in
+0000f560: 6465 7065 6e64 656e 7420 756e 6365 7274  dependent uncert
+0000f570: 6169 6e74 6965 730a 2020 2020 2020 2020  ainties.        
+0000f580: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+0000f590: 3220 3d20 6572 7232 0a20 2020 2020 2020  2 = err2.       
+0000f5a0: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
+0000f5b0: 7232 7920 3d20 6572 7232 0a20 2020 2020  r2y = err2.     
+0000f5c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f5d0: 6945 7272 3220 3d20 312e 3020 2f20 6572  iErr2 = 1.0 / er
+0000f5e0: 7232 0a20 2020 2020 2020 2020 2020 2020  r2.             
+0000f5f0: 2020 2073 656c 662e 636f 7679 203d 206e     self.covy = n
+0000f600: 702e 6469 6167 2865 7272 3229 0a20 2020  p.diag(err2).   
+0000f610: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000f620: 662e 6943 6f76 203d 206e 702e 6469 6167  f.iCov = np.diag
+0000f630: 2831 2e30 202f 2073 656c 662e 6572 7232  (1.0 / self.err2
+0000f640: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
+0000f650: 646f 206e 6f74 2072 6562 7569 6c64 2063  do not rebuild c
+0000f660: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+0000f670: 2069 6e20 636f 7374 2066 756e 6374 696f   in cost functio
+0000f680: 6e0a 2020 2020 2020 2020 2020 2020 7365  n.            se
+0000f690: 6c66 2e6e 6565 6473 5f64 796e 616d 6963  lf.needs_dynamic
+0000f6a0: 4572 726f 7273 203d 2046 616c 7365 0a0a  Errors = False..
+0000f6b0: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
+0000f6c0: 2063 6f76 6172 6961 6e63 6520 6f66 2078   covariance of x
+0000f6d0: 2d65 7272 6f72 730a 2020 2020 2020 2020  -errors.        
+0000f6e0: 2020 2020 7365 6c66 2e63 6f76 7820 3d20      self.covx = 
+0000f6f0: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+0000f700: 2073 656c 662e 6572 7232 7820 3d20 4e6f   self.err2x = No
+0000f710: 6e65 0a20 2020 2020 2020 2020 2020 2023  ne.            #
+0000f720: 2074 6f74 616c 2063 6f76 6172 6961 6e63   total covarianc
+0000f730: 6520 6973 2074 6861 7420 6f66 2079 2d65  e is that of y-e
+0000f740: 7272 6f72 730a 2020 2020 2020 2020 2020  rrors.          
+0000f750: 2020 7365 6c66 2e63 6f76 203d 2073 656c    self.cov = sel
+0000f760: 662e 636f 7679 0a0a 2020 2020 2020 2020  f.covy..        
+0000f770: 6465 6620 696e 6974 5f64 796e 616d 6963  def init_dynamic
+0000f780: 4572 726f 7273 2873 656c 6629 3a0a 2020  Errors(self):.  
+0000f790: 2020 2020 2020 2020 2020 2320 6d65 7468            # meth
+0000f7a0: 6f64 2074 6f20 7377 6974 6368 206f 6e20  od to switch on 
+0000f7b0: 6479 6e61 6d69 6320 7265 2d63 616c 6375  dynamic re-calcu
+0000f7c0: 6c61 7469 6f6e 206f 6620 636f 7661 7269  lation of covari
+0000f7d0: 616e 6365 206d 6174 7269 780a 2020 2020  ance matrix.    
+0000f7e0: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+0000f7f0: 5f74 6f4d 6f64 656c 203d 2073 656c 662e  _toModel = self.
+0000f800: 6f75 7465 722e 7265 664d 6f64 656c 0a20  outer.refModel. 
+0000f810: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000f820: 6d6f 6465 6c20 3d20 7365 6c66 2e6f 7574  model = self.out
+0000f830: 6572 2e63 6f73 7466 2e6d 6f64 656c 0a0a  er.costf.model..
+0000f840: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f850: 2e5f 7374 6174 6963 436f 7620 3d20 4e6f  ._staticCov = No
+0000f860: 6e65 0a20 2020 2020 2020 2020 2020 2073  ne.            s
+0000f870: 656c 662e 5f73 7461 7469 6345 7272 3220  elf._staticErr2 
+0000f880: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000f890: 2020 2073 656c 662e 6943 6f76 203d 204e     self.iCov = N
+0000f8a0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+0000f8b0: 7365 6c66 2e69 4572 7232 203d 204e 6f6e  self.iErr2 = Non
+0000f8c0: 650a 0a20 2020 2020 2020 2020 2020 2023  e..            #
+0000f8d0: 2072 6562 7569 6c64 2063 6f76 6172 6961   rebuild covaria
+0000f8e0: 6e63 6520 6d61 7472 6978 2064 7572 696e  nce matrix durin
+0000f8f0: 6720 6669 7474 696e 6720 7072 6f63 6564  g fitting proced
+0000f900: 7572 650a 2020 2020 2020 2020 2020 2020  ure.            
+0000f910: 7365 6c66 2e6e 6565 6473 5f64 796e 616d  self.needs_dynam
+0000f920: 6963 4572 726f 7273 203d 2054 7275 6520  icErrors = True 
+0000f930: 2023 2066 6c61 6720 666f 7220 636f 7374   # flag for cost
+0000f940: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
+0000f950: 2020 2020 2020 7365 6c66 2e66 696e 616c        self.final
+0000f960: 5f63 616c 6c20 3d20 4661 6c73 6520 2023  _call = False  #
+0000f970: 2066 6c61 6720 666f 7220 5f72 6562 7569   flag for _rebui
+0000f980: 6c64 5f43 6f76 3a20 6e6f 2073 746f 7261  ld_Cov: no stora
+0000f990: 6765 206f 6620 7963 6f76 0a0a 2020 2020  ge of ycov..    
+0000f9a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000f9b0: 6e65 6564 735f 636f 7661 7269 616e 6365  needs_covariance
+0000f9c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f9d0: 2020 2320 6275 696c 6420 7374 6174 6963    # build static
+0000f9e0: 2028 3d70 6172 616d 6574 6572 2d69 6e64   (=parameter-ind
+0000f9f0: 6570 656e 6465 6e74 2920 7061 7274 206f  ependent) part o
+0000fa00: 6620 636f 7661 7269 616e 6365 206d 6174  f covariance mat
+0000fa10: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
+0000fa20: 2020 2020 6966 2073 656c 662e 6861 735f      if self.has_
+0000fa30: 7265 6c5f 7945 7272 6f72 7320 616e 6420  rel_yErrors and 
+0000fa40: 7365 6c66 2e72 6566 5f74 6f4d 6f64 656c  self.ref_toModel
+0000fa50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fa60: 2020 2020 2020 2320 736f 6d65 2079 2d65        # some y-e
+0000fa70: 7272 6f72 7320 6172 6520 7061 7261 6d65  rrors are parame
+0000fa80: 7465 722d 696e 6465 7065 6e64 656e 740a  ter-independent.
+0000fa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000faa0: 2020 2020 7365 6c66 2e5f 7374 6174 6963      self._static
+0000fab0: 436f 7620 3d20 5f62 7569 6c64 5f43 6f76  Cov = _build_Cov
+0000fac0: 4d61 7428 0a20 2020 2020 2020 2020 2020  Mat(.           
+0000fad0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0000fae0: 662e 6e64 2c20 7365 6c66 2e65 792c 2065  f.nd, self.ey, e
+0000faf0: 6162 7363 6f72 3d73 656c 662e 6361 6273  abscor=self.cabs
+0000fb00: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
+0000fb10: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000fb20: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb40: 2020 2320 616c 6c20 792d 6572 726f 7273    # all y-errors
+0000fb50: 2061 7265 2070 6172 616d 6574 6572 2d69   are parameter-i
+0000fb60: 6e64 6570 656e 6465 6e74 0a20 2020 2020  ndependent.     
+0000fb70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000fb80: 656c 662e 5f73 7461 7469 6343 6f76 203d  elf._staticCov =
+0000fb90: 205f 6275 696c 645f 436f 764d 6174 280a   _build_CovMat(.
 0000fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbb0: 2073 656c 662e 6e64 2c0a 2020 2020 2020   self.nd,.      
-0000fbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbd0: 2020 7365 6c66 2e65 792c 0a20 2020 2020    self.ey,.     
-0000fbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fbf0: 2020 2065 7265 6c3d 7365 6c66 2e65 7265     erel=self.ere
-0000fc00: 6c79 2c0a 2020 2020 2020 2020 2020 2020  ly,.            
-0000fc10: 2020 2020 2020 2020 2020 2020 6561 6273              eabs
-0000fc20: 636f 723d 7365 6c66 2e63 6162 7379 2c0a  cor=self.cabsy,.
-0000fc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc40: 2020 2020 2020 2020 6572 656c 636f 723d          erelcor=
-0000fc50: 7365 6c66 2e63 7265 6c79 2c0a 2020 2020  self.crely,.    
-0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fc70: 2020 2020 6461 7461 3d73 656c 662e 792c      data=self.y,
-0000fc80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc90: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000fca0: 2020 2020 2020 2023 2062 7569 6c64 206d         # build m
-0000fcb0: 6174 7269 7820 6f66 2072 656c 6174 6976  atrix of relativ
-0000fcc0: 6520 6572 726f 7273 0a20 2020 2020 2020  e errors.       
-0000fcd0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000fce0: 2e72 6566 5f74 6f4d 6f64 656c 2061 6e64  .ref_toModel and
-0000fcf0: 2073 656c 662e 6861 735f 7265 6c5f 7945   self.has_rel_yE
-0000fd00: 7272 6f72 733a 0a20 2020 2020 2020 2020  rrors:.         
-0000fd10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0000fd20: 5f63 6f76 7930 203d 205f 6275 696c 645f  _covy0 = _build_
-0000fd30: 436f 764d 6174 280a 2020 2020 2020 2020  CovMat(.        
+0000fbb0: 2020 2020 2020 2020 7365 6c66 2e6e 642c          self.nd,
+0000fbc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fbd0: 2020 2020 2020 2020 2073 656c 662e 6579           self.ey
+0000fbe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000fbf0: 2020 2020 2020 2020 2020 6572 656c 3d73            erel=s
+0000fc00: 656c 662e 6572 656c 792c 0a20 2020 2020  elf.erely,.     
+0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc20: 2020 2065 6162 7363 6f72 3d73 656c 662e     eabscor=self.
+0000fc30: 6361 6273 792c 0a20 2020 2020 2020 2020  cabsy,.         
+0000fc40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000fc50: 7265 6c63 6f72 3d73 656c 662e 6372 656c  relcor=self.crel
+0000fc60: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
+0000fc70: 2020 2020 2020 2020 2020 2064 6174 613d             data=
+0000fc80: 7365 6c66 2e79 2c0a 2020 2020 2020 2020  self.y,.        
+0000fc90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000fca0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000fcb0: 6275 696c 6420 6d61 7472 6978 206f 6620  build matrix of 
+0000fcc0: 7265 6c61 7469 7665 2065 7272 6f72 730a  relative errors.
+0000fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fce0: 6966 2073 656c 662e 7265 665f 746f 4d6f  if self.ref_toMo
+0000fcf0: 6465 6c20 616e 6420 7365 6c66 2e68 6173  del and self.has
+0000fd00: 5f72 656c 5f79 4572 726f 7273 3a0a 2020  _rel_yErrors:.  
+0000fd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd20: 2020 7365 6c66 2e5f 636f 7679 3020 3d20    self._covy0 = 
+0000fd30: 5f62 7569 6c64 5f43 6f76 4d61 7428 0a20  _build_CovMat(. 
 0000fd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd50: 7365 6c66 2e6e 642c 0a20 2020 2020 2020  self.nd,.       
+0000fd50: 2020 2020 2020 2073 656c 662e 6e64 2c0a         self.nd,.
 0000fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd70: 2065 7265 6c3d 7365 6c66 2e65 7265 6c79   erel=self.erely
-0000fd80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000fd90: 2020 2020 2020 2020 2020 6572 656c 636f            erelco
-0000fda0: 723d 7365 6c66 2e63 7265 6c79 2c0a 2020  r=self.crely,.  
-0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdc0: 2020 2020 2020 6461 7461 3d6e 702e 6f6e        data=np.on
-0000fdd0: 6573 2873 656c 662e 6e64 292c 0a20 2020  es(self.nd),.   
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fdf0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000fe00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000fe10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000fe20: 662e 5f63 6f76 7930 203d 204e 6f6e 650a  f._covy0 = None.
-0000fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fe40: 2320 636f 7661 7269 616e 6365 206d 6174  # covariance mat
-0000fe50: 7269 7820 6f66 2078 2d75 6e63 6572 7461  rix of x-uncerta
-0000fe60: 696e 7469 6573 2028 616c 6c20 6172 6520  inties (all are 
-0000fe70: 7061 7261 6d65 7465 722d 6465 7065 6e64  parameter-depend
-0000fe80: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
-0000fe90: 2020 2020 2069 6620 7365 6c66 2e68 6173       if self.has
-0000fea0: 5f78 4572 726f 7273 3a0a 2020 2020 2020  _xErrors:.      
-0000feb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000fec0: 6c66 2e63 6f76 7820 3d20 5f62 7569 6c64  lf.covx = _build
-0000fed0: 5f43 6f76 4d61 7428 0a20 2020 2020 2020  _CovMat(.       
+0000fd70: 2020 2020 2020 2020 6572 656c 3d73 656c          erel=sel
+0000fd80: 662e 6572 656c 792c 0a20 2020 2020 2020  f.erely,.       
+0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fda0: 2065 7265 6c63 6f72 3d73 656c 662e 6372   erelcor=self.cr
+0000fdb0: 656c 792c 0a20 2020 2020 2020 2020 2020  ely,.           
+0000fdc0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+0000fdd0: 613d 6e70 2e6f 6e65 7328 7365 6c66 2e6e  a=np.ones(self.n
+0000fde0: 6429 2c0a 2020 2020 2020 2020 2020 2020  d),.            
+0000fdf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000fe00: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe20: 2020 2020 7365 6c66 2e5f 636f 7679 3020      self._covy0 
+0000fe30: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000fe40: 2020 2020 2020 2023 2063 6f76 6172 6961         # covaria
+0000fe50: 6e63 6520 6d61 7472 6978 206f 6620 782d  nce matrix of x-
+0000fe60: 756e 6365 7274 6169 6e74 6965 7320 2861  uncertainties (a
+0000fe70: 6c6c 2061 7265 2070 6172 616d 6574 6572  ll are parameter
+0000fe80: 2d64 6570 656e 6465 6e74 290a 2020 2020  -dependent).    
+0000fe90: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0000fea0: 656c 662e 6861 735f 7845 7272 6f72 733a  elf.has_xErrors:
+0000feb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fec0: 2020 2020 2073 656c 662e 636f 7678 203d       self.covx =
+0000fed0: 205f 6275 696c 645f 436f 764d 6174 280a   _build_CovMat(.
 0000fee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fef0: 2073 656c 662e 6e64 2c20 7365 6c66 2e65   self.nd, self.e
-0000ff00: 782c 2073 656c 662e 6572 656c 782c 2073  x, self.erelx, s
-0000ff10: 656c 662e 6361 6273 782c 2073 656c 662e  elf.cabsx, self.
-0000ff20: 6372 656c 782c 2073 656c 662e 780a 2020  crelx, self.x.  
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ff40: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000ff50: 2020 2020 2020 2020 2320 2064 6574 6572          #  deter
-0000ff60: 6d69 6e65 2064 7820 666f 7220 6465 7269  mine dx for deri
-0000ff70: 7661 7469 7665 2066 726f 6d20 736d 616c  vative from smal
-0000ff80: 6c65 7374 2078 2d75 6e63 6572 7461 696e  lest x-uncertain
-0000ff90: 7479 0a20 2020 2020 2020 2020 2020 2020  ty.             
-0000ffa0: 2020 2020 2020 2073 656c 662e 5f64 7820         self._dx 
-0000ffb0: 3d20 6e70 2e73 7172 7428 6d69 6e28 6e70  = np.sqrt(min(np
-0000ffc0: 2e64 6961 676f 6e61 6c28 7365 6c66 2e63  .diagonal(self.c
-0000ffd0: 6f76 7829 2929 202f 2031 302e 300a 2020  ovx))) / 10.0.  
-0000ffe0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000fff0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00010000: 2020 2020 2020 2020 7365 6c66 2e63 6f76          self.cov
-00010010: 7820 3d20 4e6f 6e65 0a0a 2020 2020 2020  x = None..      
-00010020: 2020 2020 2020 656c 7365 3a20 2023 206e        else:  # n
-00010030: 6f20 636f 7661 7269 616e 6365 206e 6565  o covariance nee
-00010040: 6465 642c 2075 7365 2073 696d 706c 6520  ded, use simple 
-00010050: 6d61 7468 0a20 2020 2020 2020 2020 2020  math.           
-00010060: 2020 2020 2023 2062 7569 6c64 2073 7461       # build sta
-00010070: 7469 6320 283d 7061 7261 6d65 7465 722d  tic (=parameter-
-00010080: 696e 6465 7065 6e64 656e 7429 2070 6172  independent) par
-00010090: 7420 6f66 2063 6f76 6172 6961 6e63 6520  t of covariance 
-000100a0: 6d61 7472 6978 0a20 2020 2020 2020 2020  matrix.         
-000100b0: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-000100c0: 6173 5f72 656c 5f79 4572 726f 7273 2061  as_rel_yErrors a
-000100d0: 6e64 2073 656c 662e 7265 665f 746f 4d6f  nd self.ref_toMo
-000100e0: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
-000100f0: 2020 2020 2020 2020 2023 206f 6e6c 7920           # only 
-00010100: 696e 6465 7065 6e64 656e 7420 792d 6572  independent y-er
-00010110: 726f 7273 2064 6f20 6e6f 7420 6465 7065  rors do not depe
-00010120: 6e64 206f 6e20 7061 7261 6d65 7465 7273  nd on parameters
-00010130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010140: 2020 2020 2073 656c 662e 5f73 7461 7469       self._stati
-00010150: 6345 7272 3220 3d20 5f62 7569 6c64 5f45  cErr2 = _build_E
-00010160: 7272 3228 7365 6c66 2e65 7929 0a20 2020  rr2(self.ey).   
-00010170: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00010180: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00010190: 2020 2020 2020 2023 2061 6c6c 2079 2d65         # all y-e
-000101a0: 7272 6f72 7320 6172 6520 7061 7261 6d65  rrors are parame
-000101b0: 7465 722d 696e 6465 7065 6e64 656e 740a  ter-independent.
-000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 2020 2020 7365 6c66 2e5f 7374 6174 6963      self._static
-000101e0: 4572 7232 203d 205f 6275 696c 645f 4572  Err2 = _build_Er
-000101f0: 7232 2873 656c 662e 6579 2c20 7365 6c66  r2(self.ey, self
-00010200: 2e65 7265 6c79 2c20 7365 6c66 2e79 290a  .erely, self.y).
-00010210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010220: 2069 6620 7365 6c66 2e68 6173 5f78 4572   if self.has_xEr
-00010230: 726f 7273 3a0a 2020 2020 2020 2020 2020  rors:.          
-00010240: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00010250: 7272 3278 203d 205f 6275 696c 645f 4572  rr2x = _build_Er
-00010260: 7232 2873 656c 662e 6578 2c20 7365 6c66  r2(self.ex, self
-00010270: 2e65 7265 6c78 2c20 7365 6c66 2e78 290a  .erelx, self.x).
-00010280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010290: 2020 2020 2320 2064 6574 6572 6d69 6e65      #  determine
-000102a0: 2064 7820 666f 7220 6465 7269 7661 7469   dx for derivati
-000102b0: 7665 2066 726f 6d20 736d 616c 6c65 7374  ve from smallest
-000102c0: 2078 2d75 6e63 6572 7461 696e 7479 0a20   x-uncertainty. 
-000102d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102e0: 2020 2073 656c 662e 5f64 7820 3d20 6e70     self._dx = np
-000102f0: 2e73 7172 7428 6d69 6e28 7365 6c66 2e65  .sqrt(min(self.e
-00010300: 7272 3278 2929 202f 2031 302e 300a 2020  rr2x)) / 10.0.  
-00010310: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00010320: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00010330: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-00010340: 3278 203d 204e 6f6e 650a 0a20 2020 2020  2x = None..     
-00010350: 2020 2064 6566 205f 7265 6275 696c 645f     def _rebuild_
-00010360: 4572 7232 2873 656c 662c 206d 7061 7229  Err2(self, mpar)
-00010370: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
-00010380: 220a 2020 2020 2020 2020 2020 2020 2852  ".            (R
-00010390: 652d 2963 616c 6375 6c61 7465 2075 6e63  e-)calculate unc
-000103a0: 6572 7461 696e 6769 6573 0a20 2020 2020  ertaingies.     
-000103b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000103c0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
-000103d0: 7374 6174 6963 4572 7232 2069 7320 6e6f  staticErr2 is no
-000103e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000103f0: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-00010400: 3220 3d20 6e70 2e61 7272 6179 2873 656c  2 = np.array(sel
-00010410: 662e 5f73 7461 7469 6345 7272 322c 2063  f._staticErr2, c
-00010420: 6f70 793d 5472 7565 290a 2020 2020 2020  opy=True).      
-00010430: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00010440: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00010450: 2e65 7272 3220 3d20 6e70 2e7a 6572 6f73  .err2 = np.zeros
-00010460: 2873 656c 662e 6e64 290a 2020 2020 2020  (self.nd).      
-00010470: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-00010480: 665f 746f 4d6f 6465 6c20 616e 6420 7365  f_toModel and se
-00010490: 6c66 2e68 6173 5f72 656c 5f79 4572 726f  lf.has_rel_yErro
-000104a0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-000104b0: 2020 2020 5f65 7220 3d20 7365 6c66 2e65      _er = self.e
-000104c0: 7265 6c79 202a 2073 656c 662e 6d6f 6465  rely * self.mode
-000104d0: 6c28 7365 6c66 2e78 2c20 2a6d 7061 7229  l(self.x, *mpar)
-000104e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000104f0: 2073 656c 662e 6572 7232 202b 3d20 5f65   self.err2 += _e
-00010500: 7220 2a20 5f65 720a 2020 2020 2020 2020  r * _er.        
-00010510: 2020 2020 2320 7265 6d65 6d62 6572 2079      # remember y
-00010520: 2d65 7272 6f72 730a 2020 2020 2020 2020  -errors.        
-00010530: 2020 2020 7365 6c66 2e65 7272 3279 203d      self.err2y =
-00010540: 206e 702e 6172 7261 7928 7365 6c66 2e65   np.array(self.e
-00010550: 7272 322c 2063 6f70 793d 5472 7565 290a  rr2, copy=True).
-00010560: 2020 2020 2020 2020 2020 2020 2320 6164              # ad
-00010570: 6420 7072 6f6a 6563 7465 6420 7820 6572  d projected x er
-00010580: 726f 7273 0a20 2020 2020 2020 2020 2020  rors.           
-00010590: 2069 6620 7365 6c66 2e65 7272 3278 2069   if self.err2x i
-000105a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000105b0: 2020 2020 2020 2020 2020 2020 2320 6465              # de
-000105c0: 7465 726d 696e 6520 6465 7269 7661 7469  termine derivati
-000105d0: 7665 7320 6f66 206d 6f64 656c 2066 756e  ves of model fun
-000105e0: 6374 696f 6e20 772e 722e 742e 2078 2c0a  ction w.r.t. x,.
-000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 5f6d 7072 696d 6520 3d20 280a 2020 2020  _mprime = (.    
-00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010620: 302e 350a 2020 2020 2020 2020 2020 2020  0.5.            
-00010630: 2020 2020 2020 2020 2f20 7365 6c66 2e5f          / self._
-00010640: 6478 0a20 2020 2020 2020 2020 2020 2020  dx.             
-00010650: 2020 2020 2020 202a 2028 0a20 2020 2020         * (.     
-00010660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010670: 2020 2073 656c 662e 6d6f 6465 6c28 7365     self.model(se
-00010680: 6c66 2e78 202b 2073 656c 662e 5f64 782c  lf.x + self._dx,
-00010690: 202a 6d70 6172 290a 2020 2020 2020 2020   *mpar).        
+0000fef0: 2020 2020 2020 2020 7365 6c66 2e6e 642c          self.nd,
+0000ff00: 2073 656c 662e 6578 2c20 7365 6c66 2e65   self.ex, self.e
+0000ff10: 7265 6c78 2c20 7365 6c66 2e63 6162 7378  relx, self.cabsx
+0000ff20: 2c20 7365 6c66 2e63 7265 6c78 2c20 7365  , self.crelx, se
+0000ff30: 6c66 2e78 0a20 2020 2020 2020 2020 2020  lf.x.           
+0000ff40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000ff50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000ff60: 2020 6465 7465 726d 696e 6520 6478 2066    determine dx f
+0000ff70: 6f72 2064 6572 6976 6174 6976 6520 6672  or derivative fr
+0000ff80: 6f6d 2073 6d61 6c6c 6573 7420 782d 756e  om smallest x-un
+0000ff90: 6365 7274 6169 6e74 790a 2020 2020 2020  certainty.      
+0000ffa0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000ffb0: 6c66 2e5f 6478 203d 206e 702e 7371 7274  lf._dx = np.sqrt
+0000ffc0: 286d 696e 286e 702e 6469 6167 6f6e 616c  (min(np.diagonal
+0000ffd0: 2873 656c 662e 636f 7678 2929 2920 2f20  (self.covx))) / 
+0000ffe0: 3130 2e30 0a20 2020 2020 2020 2020 2020  10.0.           
+0000fff0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010000: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010010: 656c 662e 636f 7678 203d 204e 6f6e 650a  elf.covx = None.
+00010020: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00010030: 653a 2020 2320 6e6f 2063 6f76 6172 6961  e:  # no covaria
+00010040: 6e63 6520 6e65 6564 6564 2c20 7573 6520  nce needed, use 
+00010050: 7369 6d70 6c65 206d 6174 680a 2020 2020  simple math.    
+00010060: 2020 2020 2020 2020 2020 2020 2320 6275              # bu
+00010070: 696c 6420 7374 6174 6963 2028 3d70 6172  ild static (=par
+00010080: 616d 6574 6572 2d69 6e64 6570 656e 6465  ameter-independe
+00010090: 6e74 2920 7061 7274 206f 6620 636f 7661  nt) part of cova
+000100a0: 7269 616e 6365 206d 6174 7269 780a 2020  riance matrix.  
+000100b0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000100c0: 2073 656c 662e 6861 735f 7265 6c5f 7945   self.has_rel_yE
+000100d0: 7272 6f72 7320 616e 6420 7365 6c66 2e72  rrors and self.r
+000100e0: 6566 5f74 6f4d 6f64 656c 3a0a 2020 2020  ef_toModel:.    
+000100f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010100: 2320 6f6e 6c79 2069 6e64 6570 656e 6465  # only independe
+00010110: 6e74 2079 2d65 7272 6f72 7320 646f 206e  nt y-errors do n
+00010120: 6f74 2064 6570 656e 6420 6f6e 2070 6172  ot depend on par
+00010130: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00010140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010150: 2e5f 7374 6174 6963 4572 7232 203d 205f  ._staticErr2 = _
+00010160: 6275 696c 645f 4572 7232 2873 656c 662e  build_Err2(self.
+00010170: 6579 290a 2020 2020 2020 2020 2020 2020  ey).            
+00010180: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00010190: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+000101a0: 616c 6c20 792d 6572 726f 7273 2061 7265  all y-errors are
+000101b0: 2070 6172 616d 6574 6572 2d69 6e64 6570   parameter-indep
+000101c0: 656e 6465 6e74 0a20 2020 2020 2020 2020  endent.         
+000101d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000101e0: 5f73 7461 7469 6345 7272 3220 3d20 5f62  _staticErr2 = _b
+000101f0: 7569 6c64 5f45 7272 3228 7365 6c66 2e65  uild_Err2(self.e
+00010200: 792c 2073 656c 662e 6572 656c 792c 2073  y, self.erely, s
+00010210: 656c 662e 7929 0a0a 2020 2020 2020 2020  elf.y)..        
+00010220: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00010230: 6861 735f 7845 7272 6f72 733a 0a20 2020  has_xErrors:.   
+00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010250: 2073 656c 662e 6572 7232 7820 3d20 5f62   self.err2x = _b
+00010260: 7569 6c64 5f45 7272 3228 7365 6c66 2e65  uild_Err2(self.e
+00010270: 782c 2073 656c 662e 6572 656c 782c 2073  x, self.erelx, s
+00010280: 656c 662e 7829 0a20 2020 2020 2020 2020  elf.x).         
+00010290: 2020 2020 2020 2020 2020 2023 2020 6465             #  de
+000102a0: 7465 726d 696e 6520 6478 2066 6f72 2064  termine dx for d
+000102b0: 6572 6976 6174 6976 6520 6672 6f6d 2073  erivative from s
+000102c0: 6d61 6c6c 6573 7420 782d 756e 6365 7274  mallest x-uncert
+000102d0: 6169 6e74 790a 2020 2020 2020 2020 2020  ainty.          
+000102e0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+000102f0: 6478 203d 206e 702e 7371 7274 286d 696e  dx = np.sqrt(min
+00010300: 2873 656c 662e 6572 7232 7829 2920 2f20  (self.err2x)) / 
+00010310: 3130 2e30 0a20 2020 2020 2020 2020 2020  10.0.           
+00010320: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010330: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010340: 656c 662e 6572 7232 7820 3d20 4e6f 6e65  elf.err2x = None
+00010350: 0a0a 2020 2020 2020 2020 6465 6620 5f72  ..        def _r
+00010360: 6562 7569 6c64 5f45 7272 3228 7365 6c66  ebuild_Err2(self
+00010370: 2c20 6d70 6172 293a 0a20 2020 2020 2020  , mpar):.       
+00010380: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00010390: 2020 2020 2028 5265 2d29 6361 6c63 756c       (Re-)calcul
+000103a0: 6174 6520 756e 6365 7274 6169 6e67 6965  ate uncertaingie
+000103b0: 730a 2020 2020 2020 2020 2020 2020 2222  s.            ""
+000103c0: 220a 2020 2020 2020 2020 2020 2020 6966  ".            if
+000103d0: 2073 656c 662e 5f73 7461 7469 6345 7272   self._staticErr
+000103e0: 3220 6973 206e 6f74 204e 6f6e 653a 0a20  2 is not None:. 
+000103f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010400: 656c 662e 6572 7232 203d 206e 702e 6172  elf.err2 = np.ar
+00010410: 7261 7928 7365 6c66 2e5f 7374 6174 6963  ray(self._static
+00010420: 4572 7232 2c20 636f 7079 3d54 7275 6529  Err2, copy=True)
+00010430: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00010440: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00010450: 2020 2073 656c 662e 6572 7232 203d 206e     self.err2 = n
+00010460: 702e 7a65 726f 7328 7365 6c66 2e6e 6429  p.zeros(self.nd)
+00010470: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00010480: 7365 6c66 2e72 6566 5f74 6f4d 6f64 656c  self.ref_toModel
+00010490: 2061 6e64 2073 656c 662e 6861 735f 7265   and self.has_re
+000104a0: 6c5f 7945 7272 6f72 733a 0a20 2020 2020  l_yErrors:.     
+000104b0: 2020 2020 2020 2020 2020 205f 6572 203d             _er =
+000104c0: 2073 656c 662e 6572 656c 7920 2a20 7365   self.erely * se
+000104d0: 6c66 2e6d 6f64 656c 2873 656c 662e 782c  lf.model(self.x,
+000104e0: 202a 6d70 6172 290a 2020 2020 2020 2020   *mpar).        
+000104f0: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
+00010500: 3220 2b3d 205f 6572 202a 205f 6572 0a20  2 += _er * _er. 
+00010510: 2020 2020 2020 2020 2020 2023 2072 656d             # rem
+00010520: 656d 6265 7220 792d 6572 726f 7273 0a20  ember y-errors. 
+00010530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010540: 6572 7232 7920 3d20 6e70 2e61 7272 6179  err2y = np.array
+00010550: 2873 656c 662e 6572 7232 2c20 636f 7079  (self.err2, copy
+00010560: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+00010570: 2020 2023 2061 6464 2070 726f 6a65 6374     # add project
+00010580: 6564 2078 2065 7272 6f72 730a 2020 2020  ed x errors.    
+00010590: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000105a0: 6572 7232 7820 6973 206e 6f74 204e 6f6e  err2x is not Non
+000105b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000105c0: 2020 2023 2064 6574 6572 6d69 6e65 2064     # determine d
+000105d0: 6572 6976 6174 6976 6573 206f 6620 6d6f  erivatives of mo
+000105e0: 6465 6c20 6675 6e63 7469 6f6e 2077 2e72  del function w.r
+000105f0: 2e74 2e20 782c 0a20 2020 2020 2020 2020  .t. x,.         
+00010600: 2020 2020 2020 205f 6d70 7269 6d65 203d         _mprime =
+00010610: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00010620: 2020 2020 2020 2030 2e35 0a20 2020 2020         0.5.     
+00010630: 2020 2020 2020 2020 2020 2020 2020 202f                 /
+00010640: 2073 656c 662e 5f64 780a 2020 2020 2020   self._dx.      
+00010650: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+00010660: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00010670: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00010680: 6f64 656c 2873 656c 662e 7820 2b20 7365  odel(self.x + se
+00010690: 6c66 2e5f 6478 2c20 2a6d 7061 7229 0a20  lf._dx, *mpar). 
 000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106b0: 2d20 7365 6c66 2e6d 6f64 656c 2873 656c  - self.model(sel
-000106c0: 662e 7820 2d20 7365 6c66 2e5f 6478 2c20  f.x - self._dx, 
-000106d0: 2a6d 7061 7229 0a20 2020 2020 2020 2020  *mpar).         
-000106e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000106f0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00010700: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00010710: 2070 726f 6a65 6374 206f 6e20 7920 616e   project on y an
-00010720: 6420 6164 6420 746f 2063 6f76 6172 6961  d add to covaria
-00010730: 6e63 6520 6d61 7472 6978 0a20 2020 2020  nce matrix.     
-00010740: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00010750: 6572 7232 202b 3d20 5f6d 7072 696d 6520  err2 += _mprime 
-00010760: 2a20 5f6d 7072 696d 6520 2a20 7365 6c66  * _mprime * self
-00010770: 2e65 7272 3278 0a0a 2020 2020 2020 2020  .err2x..        
-00010780: 6465 6620 5f72 6562 7569 6c64 5f43 6f76  def _rebuild_Cov
-00010790: 2873 656c 662c 206d 7061 7229 3a0a 2020  (self, mpar):.  
-000107a0: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
-000107b0: 2020 2020 2020 2020 2020 2852 652d 2942            (Re-)B
-000107c0: 7569 6c64 2074 6865 2063 6f76 6172 6961  uild the covaria
-000107d0: 6e63 6520 6d61 7472 6978 2066 726f 6d20  nce matrix from 
-000107e0: 636f 6d70 6f6e 656e 7473 0a20 2020 2020  components.     
-000107f0: 2020 2020 2020 2061 6e64 2063 6163 6c75         and caclu
-00010800: 6c61 7465 2069 7473 2069 6e76 6572 7365  late its inverse
-00010810: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-00010820: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00010830: 7461 7274 2066 726f 6d20 7072 652d 6275  tart from pre-bu
-00010840: 696c 7420 7061 7261 6d65 7465 722d 696e  ilt parameter-in
-00010850: 6465 7065 6e64 656e 7420 7061 7274 206f  dependent part o
-00010860: 6620 436f 7661 7269 616e 6365 204d 6174  f Covariance Mat
-00010870: 7269 780a 2020 2020 2020 2020 2020 2020  rix.            
-00010880: 7365 6c66 2e63 6f76 203d 206e 702e 6172  self.cov = np.ar
-00010890: 7261 7928 7365 6c66 2e5f 7374 6174 6963  ray(self._static
-000108a0: 436f 762c 2063 6f70 793d 5472 7565 290a  Cov, copy=True).
-000108b0: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
-000108c0: 6464 206d 6174 7269 7820 6f66 2070 6172  dd matrix of par
-000108d0: 616d 6574 6572 2d64 6570 656e 6465 6e74  ameter-dependent
-000108e0: 2079 2d75 6e63 6572 7461 696e 7469 6573   y-uncertainties
-000108f0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-00010900: 2020 2020 6966 2073 656c 662e 7265 665f      if self.ref_
-00010910: 746f 4d6f 6465 6c20 616e 6420 7365 6c66  toModel and self
-00010920: 2e68 6173 5f72 656c 5f79 4572 726f 7273  .has_rel_yErrors
-00010930: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00010940: 2073 656c 662e 5f63 6f76 7930 2069 7320   self._covy0 is 
-00010950: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00010960: 2020 2020 2020 2020 2020 5f79 6461 7420            _ydat 
-00010970: 3d20 7365 6c66 2e6d 6f64 656c 2873 656c  = self.model(sel
-00010980: 662e 782c 202a 6d70 6172 290a 2020 2020  f.x, *mpar).    
-00010990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000109a0: 2e63 6f76 202b 3d20 7365 6c66 2e5f 636f  .cov += self._co
-000109b0: 7679 3020 2a20 6e70 2e6f 7574 6572 285f  vy0 * np.outer(_
-000109c0: 7964 6174 2c20 5f79 6461 7429 0a20 2020  ydat, _ydat).   
-000109d0: 2020 2020 2020 2020 2023 2061 6464 2070           # add p
-000109e0: 726f 6a65 6374 6564 2078 2065 7272 6f72  rojected x error
-000109f0: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
-00010a00: 2073 656c 662e 6861 735f 7845 7272 6f72   self.has_xError
-00010a10: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00010a20: 2020 2023 2073 746f 7265 2063 6f76 6172     # store covar
-00010a30: 6961 6e63 6520 6d61 7472 6978 206f 6620  iance matrix of 
-00010a40: 792d 756e 6365 7274 6169 6e74 6965 730a  y-uncertainties.
-00010a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a60: 6966 2073 656c 662e 6669 6e61 6c5f 6361  if self.final_ca
-00010a70: 6c6c 3a0a 2020 2020 2020 2020 2020 2020  ll:.            
-00010a80: 2020 2020 2020 2020 7365 6c66 2e63 6f76          self.cov
-00010a90: 7920 3d20 6e70 2e61 7272 6179 2873 656c  y = np.array(sel
-00010aa0: 662e 636f 762c 2063 6f70 793d 5472 7565  f.cov, copy=True
-00010ab0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00010ac0: 2020 2023 2064 6574 6572 6d69 6e65 2064     # determine d
-00010ad0: 6572 6976 6174 6976 6573 206f 6620 6d6f  erivatives of mo
-00010ae0: 6465 6c20 6675 6e63 7469 6f6e 2077 2e72  del function w.r
-00010af0: 2e74 2e20 782c 0a20 2020 2020 2020 2020  .t. x,.         
-00010b00: 2020 2020 2020 205f 6d70 7269 6d65 203d         _mprime =
-00010b10: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00010b20: 2020 2020 2020 2030 2e35 0a20 2020 2020         0.5.     
-00010b30: 2020 2020 2020 2020 2020 2020 2020 202f                 /
-00010b40: 2073 656c 662e 5f64 780a 2020 2020 2020   self._dx.      
-00010b50: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
-00010b60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010b70: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00010b80: 6f64 656c 2873 656c 662e 7820 2b20 7365  odel(self.x + se
-00010b90: 6c66 2e5f 6478 2c20 2a6d 7061 7229 0a20  lf._dx, *mpar). 
-00010ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bb0: 2020 2020 2020 202d 2073 656c 662e 6d6f         - self.mo
-00010bc0: 6465 6c28 7365 6c66 2e78 202d 2073 656c  del(self.x - sel
-00010bd0: 662e 5f64 782c 202a 6d70 6172 290a 2020  f._dx, *mpar).  
-00010be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bf0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00010c00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00010c10: 2020 2020 2020 2320 7072 6f6a 6563 7420        # project 
-00010c20: 6f6e 2079 2061 6e64 2061 6464 2074 6f20  on y and add to 
-00010c30: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-00010c40: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
-00010c50: 2020 7365 6c66 2e63 6f76 202b 3d20 6e70    self.cov += np
-00010c60: 2e6f 7574 6572 285f 6d70 7269 6d65 2c20  .outer(_mprime, 
-00010c70: 5f6d 7072 696d 6529 202a 2073 656c 662e  _mprime) * self.
-00010c80: 636f 7678 0a20 2020 2020 2020 2020 2020  covx.           
-00010c90: 2065 6c73 653a 2020 2320 6e6f 2078 2d65   else:  # no x-e
-00010ca0: 7272 6f72 732c 2079 2d63 6f76 6d61 7420  rrors, y-covmat 
-00010cb0: 3d20 636f 766d 6174 0a20 2020 2020 2020  = covmat.       
-00010cc0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00010cd0: 7679 203d 2073 656c 662e 636f 760a 0a20  vy = self.cov.. 
-00010ce0: 2020 2020 2020 2064 6566 2067 6574 5f43         def get_C
-00010cf0: 6f76 2873 656c 6629 3a0a 2020 2020 2020  ov(self):.      
-00010d00: 2020 2020 2020 2222 2272 6574 7572 6e20        """return 
-00010d10: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-00010d20: 7820 6f66 2064 6174 6122 2222 0a20 2020  x of data""".   
-00010d30: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00010d40: 2e6e 6565 6473 5f63 6f76 6172 6961 6e63  .needs_covarianc
-00010d50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00010d60: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
-00010d70: 6f76 0a20 2020 2020 2020 2020 2020 2065  ov.            e
-00010d80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00010d90: 2020 2020 2069 6620 7365 6c66 2e65 7272       if self.err
-00010da0: 3220 6973 204e 6f6e 653a 0a20 2020 2020  2 is None:.     
-00010db0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00010dc0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-00010dd0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00010de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010df0: 2020 2020 2072 6574 7572 6e20 6e70 2e64       return np.d
-00010e00: 6961 6728 7365 6c66 2e65 7272 3229 0a0a  iag(self.err2)..
-00010e10: 2020 2020 2020 2020 6465 6620 6765 745f          def get_
-00010e20: 7843 6f76 2873 656c 6629 3a0a 2020 2020  xCov(self):.    
-00010e30: 2020 2020 2020 2020 2222 2272 6574 7572          """retur
-00010e40: 6e20 636f 7661 7269 616e 6365 206d 6174  n covariance mat
-00010e50: 7269 7820 6f66 2078 2d64 6174 6122 2222  rix of x-data"""
-00010e60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00010e70: 7365 6c66 2e6e 6565 6473 5f63 6f76 6172  self.needs_covar
-00010e80: 6961 6e63 653a 0a20 2020 2020 2020 2020  iance:.         
-00010e90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00010ea0: 6c66 2e63 6f76 780a 2020 2020 2020 2020  lf.covx.        
-00010eb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00010ec0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00010ed0: 662e 6572 7232 7820 6973 204e 6f6e 653a  f.err2x is None:
-00010ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ef0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00010f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010f10: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00010f20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010f30: 6e20 6e70 2e64 6961 6728 7365 6c66 2e65  n np.diag(self.e
-00010f40: 7272 3278 290a 0a20 2020 2020 2020 2064  rr2x)..        d
-00010f50: 6566 2067 6574 5f79 436f 7628 7365 6c66  ef get_yCov(self
-00010f60: 293a 0a20 2020 2020 2020 2020 2020 2022  ):.            "
-00010f70: 2222 7265 7475 726e 2063 6f76 6172 6961  ""return covaria
-00010f80: 6e63 6520 6d61 7472 6978 206f 6620 792d  nce matrix of y-
-00010f90: 6461 7461 2222 220a 2020 2020 2020 2020  data""".        
-00010fa0: 2020 2020 6966 2073 656c 662e 6e65 6564      if self.need
-00010fb0: 735f 636f 7661 7269 616e 6365 3a0a 2020  s_covariance:.  
-00010fc0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00010fd0: 7475 726e 2073 656c 662e 636f 7679 0a20  turn self.covy. 
-00010fe0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00010ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011000: 2069 6620 7365 6c66 2e65 7272 3279 2069   if self.err2y i
-00011010: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00011020: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011030: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
-00011040: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011060: 2020 7265 7475 726e 206e 702e 6469 6167    return np.diag
-00011070: 2873 656c 662e 6572 7232 7929 0a0a 2020  (self.err2y)..  
-00011080: 2020 2020 2020 6465 6620 6765 745f 6943        def get_iC
-00011090: 6f76 2873 656c 6629 3a0a 2020 2020 2020  ov(self):.      
-000110a0: 2020 2020 2020 2222 2272 6574 7572 6e20        """return 
-000110b0: 696e 7665 7273 6520 6f66 2063 6f76 6172  inverse of covar
-000110c0: 6961 6e63 6520 6d61 7472 6978 2c20 6173  iance matrix, as
-000110d0: 2075 7365 6420 696e 2063 6f73 7420 6675   used in cost fu
-000110e0: 6e63 7469 6f6e 2222 220a 2020 2020 2020  nction""".      
-000110f0: 2020 2020 2020 6966 2073 656c 662e 6e65        if self.ne
-00011100: 6564 735f 636f 7661 7269 616e 6365 3a0a  eds_covariance:.
-00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 7265 7475 726e 2073 656c 662e 6943 6f76  return self.iCov
-00011130: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00011140: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011150: 2020 2072 6574 7572 6e20 6e70 2e64 6961     return np.dia
-00011160: 6728 312e 3020 2f20 7365 6c66 2e65 7272  g(1.0 / self.err
-00011170: 3229 0a0a 2020 2020 2020 2020 6465 6620  2)..        def 
-00011180: 706c 6f74 280a 2020 2020 2020 2020 2020  plot(.          
-00011190: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000111a0: 2020 2020 6e75 6d3d 2278 7944 6174 6120      num="xyData 
-000111b0: 616e 6420 4d6f 6465 6c22 2c0a 2020 2020  and Model",.    
-000111c0: 2020 2020 2020 2020 6669 6773 697a 653d          figsize=
-000111d0: 2837 2e35 2c20 362e 3529 2c0a 2020 2020  (7.5, 6.5),.    
-000111e0: 2020 2020 2020 2020 6461 7461 5f6c 6162          data_lab
-000111f0: 656c 3d22 6461 7461 222c 0a20 2020 2020  el="data",.     
-00011200: 2020 2020 2020 2070 6c6f 745f 7265 7369         plot_resi
-00011210: 6475 616c 3d46 616c 7365 2c0a 2020 2020  dual=False,.    
-00011220: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-00011230: 2020 2022 2222 7265 7475 726e 2066 6967     """return fig
-00011240: 7572 6520 7769 7468 2078 7920 6461 7461  ure with xy data
-00011250: 2061 6e64 2075 6e63 6572 7461 696e 7469   and uncertainti
-00011260: 6573 2222 220a 2020 2020 2020 2020 2020  es""".          
-00011270: 2020 2320 2020 2023 2067 6574 2064 6174    #    # get dat
-00011280: 610a 2020 2020 2020 2020 2020 2020 7820  a.            x 
-00011290: 3d20 7365 6c66 2e78 0a20 2020 2020 2020  = self.x.       
-000112a0: 2020 2020 2069 6620 706c 6f74 5f72 6573       if plot_res
-000112b0: 6964 7561 6c20 616e 6420 7365 6c66 2e6d  idual and self.m
-000112c0: 6f64 656c 5f76 616c 7565 7320 6973 206e  odel_values is n
-000112d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000112e0: 2020 2020 2020 2020 2079 203d 2073 656c           y = sel
-000112f0: 662e 7920 2d20 7365 6c66 2e6d 6f64 656c  f.y - self.model
-00011300: 5f76 616c 7565 730a 2020 2020 2020 2020  _values.        
-00011310: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00011320: 2020 2020 2020 2020 2020 7920 3d20 7365            y = se
-00011330: 6c66 2e79 0a20 2020 2020 2020 2020 2020  lf.y.           
-00011340: 2065 7920 3d20 7365 6c66 2e67 6574 5f79   ey = self.get_y
-00011350: 436f 7628 290a 2020 2020 2020 2020 2020  Cov().          
-00011360: 2020 6966 2065 792e 6e64 696d 203d 3d20    if ey.ndim == 
-00011370: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
-00011380: 2020 2065 7920 3d20 6e70 2e73 7172 7428     ey = np.sqrt(
-00011390: 6e70 2e64 6961 676f 6e61 6c28 6579 2929  np.diagonal(ey))
-000113a0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-000113b0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000113c0: 2020 2065 7920 3d20 6e70 2e73 7172 7428     ey = np.sqrt(
-000113d0: 6579 290a 2020 2020 2020 2020 2020 2020  ey).            
-000113e0: 6578 203d 2073 656c 662e 6765 745f 7843  ex = self.get_xC
-000113f0: 6f76 2829 0a20 2020 2020 2020 2020 2020  ov().           
-00011400: 2069 6620 6578 2069 7320 6e6f 7420 4e6f   if ex is not No
-00011410: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011420: 2020 2020 6966 2065 782e 6e64 696d 203d      if ex.ndim =
-00011430: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-00011440: 2020 2020 2020 2020 2065 7820 3d20 6e70           ex = np
-00011450: 2e73 7172 7428 6e70 2e64 6961 676f 6e61  .sqrt(np.diagona
-00011460: 6c28 6578 2929 0a20 2020 2020 2020 2020  l(ex)).         
-00011470: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00011480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011490: 2065 7820 3d20 6e70 2e73 7172 7428 6578   ex = np.sqrt(ex
-000114a0: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-000114b0: 6472 6177 2064 6174 610a 2020 2020 2020  draw data.      
-000114c0: 2020 2020 2020 6669 6720 3d20 706c 742e        fig = plt.
-000114d0: 6669 6775 7265 286e 756d 3d6e 756d 2c20  figure(num=num, 
-000114e0: 6669 6773 697a 653d 6669 6773 697a 6529  figsize=figsize)
-000114f0: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
-00011500: 2e70 6c6f 7428 782c 2079 2c20 6d61 726b  .plot(x, y, mark
-00011510: 6572 3d22 7822 2c20 6c69 6e65 7374 796c  er="x", linestyl
-00011520: 653d 2222 2c20 636f 6c6f 723d 2267 7265  e="", color="gre
-00011530: 7922 2c20 616c 7068 613d 302e 3529 0a20  y", alpha=0.5). 
-00011540: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
-00011550: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00011560: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00011570: 742e 6572 726f 7262 6172 2878 2c20 792c  t.errorbar(x, y,
-00011580: 2078 6572 723d 6578 2c20 7965 7272 3d65   xerr=ex, yerr=e
-00011590: 792c 2066 6d74 3d22 2e22 2c20 6c61 6265  y, fmt=".", labe
-000115a0: 6c3d 6461 7461 5f6c 6162 656c 290a 2020  l=data_label).  
-000115b0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000115c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115d0: 706c 742e 6572 726f 7262 6172 2878 2c20  plt.errorbar(x, 
-000115e0: 792c 2065 792c 2066 6d74 3d22 2e22 2c20  y, ey, fmt=".", 
-000115f0: 6c61 6265 6c3d 6461 7461 5f6c 6162 656c  label=data_label
-00011600: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00011610: 7475 726e 2066 6967 0a0a 2020 2020 2320  turn fig..    # 
-00011620: 6465 6669 6e65 2063 7573 746f 6d20 636f  define custom co
-00011630: 7374 2066 756e 6374 696f 6e20 666f 7220  st function for 
-00011640: 696d 696e 7569 740a 2020 2020 636c 6173  iminuit.    clas
-00011650: 7320 784c 5371 436f 7374 3a0a 2020 2020  s xLSqCost:.    
-00011660: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011670: 2043 7573 746f 6d20 655f 785f 7465 6e64   Custom e_x_tend
-00011680: 6564 204c 6561 7374 2d53 5175 6172 6573  ed Least-SQuares
-00011690: 2063 6f73 7420 6675 6e63 7469 6f6e 2077   cost function w
-000116a0: 6974 680a 2020 2020 2020 2020 2064 796e  ith.         dyn
-000116b0: 616d 6963 616c 6c79 2075 7064 6174 6564  amically updated
-000116c0: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-000116d0: 6978 2061 6e64 202d 326c 6f67 284c 290a  ix and -2log(L).
-000116e0: 2020 2020 2020 2020 2063 6f72 7265 6374           correct
-000116f0: 696f 6e20 7465 726d 2066 6f72 2070 6172  ion term for par
-00011700: 616d 6574 6572 2d64 6570 656e 6465 6e74  ameter-dependent
-00011710: 2075 6e63 6572 7461 696e 7469 6573 2e0a   uncertainties..
-00011720: 0a20 2020 2020 2020 2020 5468 6520 6465  .         The de
-00011730: 6661 756c 7420 636f 7374 2066 756e 6374  fault cost funct
-00011740: 696f 6e20 6973 2074 7769 6365 2074 6865  ion is twice the
-00011750: 206e 6567 6174 6976 6520 6c6f 6761 7269   negative logari
-00011760: 7468 6d0a 2020 2020 2020 2020 206f 6620  thm.         of 
-00011770: 7468 6520 6c69 6b65 6c69 686f 6f64 206f  the likelihood o
-00011780: 6620 6120 4761 7573 7369 616e 2064 6973  f a Gaussian dis
-00011790: 7472 6962 7574 696f 6e20 666f 7220 6461  tribution for da
-000117a0: 7461 2070 6f69 6e74 730a 2020 2020 2020  ta points.      
-000117b0: 2020 203a 6d61 7468 3a60 2878 2c20 7929     :math:`(x, y)
-000117c0: 6020 7769 7468 2061 206d 6f64 656c 2066  ` with a model f
-000117d0: 756e 6374 696f 6e20 3a6d 6174 683a 6079  unction :math:`y
-000117e0: 3d66 2878 2c20 2a70 2960 2064 6570 656e  =f(x, *p)` depen
-000117f0: 6469 6e67 0a20 2020 2020 2020 2020 6f6e  ding.         on
-00011800: 2061 2073 6574 206f 6620 7061 7261 6d65   a set of parame
-00011810: 7465 7273 203a 6d61 7468 3a60 2a70 6020  ters :math:`*p` 
-00011820: 616e 6420 6120 706f 7373 6962 6c79 2070  and a possibly p
-00011830: 6172 616d 6574 6572 2d64 6570 656e 6465  arameter-depende
-00011840: 6e74 0a20 2020 2020 2020 2020 636f 7661  nt.         cova
-00011850: 7269 616e 6365 206d 6174 7269 7820 3a6d  riance matrix :m
-00011860: 6174 683a 6056 2878 2c20 6628 782c 202a  ath:`V(x, f(x, *
-00011870: 7029 2960 206f 6620 7468 6520 7820 616e  p))` of the x an
-00011880: 6420 7920 6461 7461 3a0a 0a20 2020 2020  d y data:..     
-00011890: 2020 2020 2e2e 206d 6174 683a 3a0a 2020      .. math::.  
-000118a0: 2020 2020 2020 2020 202d 325c 6c6e 207b           -2\ln {
-000118b0: 5c63 616c 204c 7d20 3d20 5c63 6869 5e32  \cal L} = \chi^2
-000118c0: 2879 2c20 565e 7b2d 317d 2c20 6628 782c  (y, V^{-1}, f(x,
-000118d0: 202a 7029 205c 2c29 0a20 2020 2020 2020   *p) \,).       
-000118e0: 2020 2020 2b20 5c6c 6e28 5c2c 205c 6465      + \ln(\, \de
-000118f0: 7428 2056 2878 2c20 6628 782c 202a 7029  t( V(x, f(x, *p)
-00011900: 2029 205c 2c29 0a0a 2020 2020 2020 2020   ) \,)..        
-00011910: 2049 6e20 7468 6520 6162 7365 6e63 6520   In the absence 
-00011920: 6f66 2070 6172 616d 6574 6572 2d64 6570  of parameter-dep
-00011930: 656e 6465 6e74 2063 6f6d 706f 6e65 6e74  endent component
-00011940: 7320 6f66 2074 6865 2063 6f76 6172 6961  s of the covaria
-00011950: 6e63 650a 2020 2020 2020 2020 206d 6174  nce.         mat
-00011960: 7269 782c 2074 6865 206c 6173 7420 7465  rix, the last te
-00011970: 726d 2069 7320 6f6d 6974 7465 6420 616e  rm is omitted an
-00011980: 6420 7468 6520 636f 7374 2066 756e 6374  d the cost funct
-00011990: 696f 6e20 6973 2069 6465 6e74 6963 616c  ion is identical
-000119a0: 0a20 2020 2020 2020 2020 746f 2074 6865  .         to the
-000119b0: 2063 6c61 7373 6963 616c 203a 6d61 7468   classical :math
-000119c0: 3a60 5c63 6869 5e32 602e 0a20 2020 2020  :`\chi^2`..     
-000119d0: 2020 2020 466f 7220 7468 6520 6576 616c      For the eval
-000119e0: 7561 7469 6f6e 206f 6620 7468 6520 636f  uation of the co
-000119f0: 7374 2066 756e 6374 696f 6e20 616e 2065  st function an e
-00011a00: 6666 6963 6965 6e74 2061 7070 726f 6163  fficient approac
-00011a10: 6820 6261 7365 640a 2020 2020 2020 2020  h based.        
-00011a20: 206f 6e20 7468 6520 2243 686f 6c65 736b   on the "Cholesk
-00011a30: 7920 6465 636f 6d70 6f73 6974 696f 6e22  y decomposition"
-00011a40: 206f 6620 7468 6520 636f 7661 7269 616e   of the covarian
-00011a50: 6365 206d 6174 7269 7820 696e 0a20 2020  ce matrix in.   
-00011a60: 2020 2020 2020 6120 7072 6f64 7563 7420        a product 
-00011a70: 6f66 2061 2074 7269 616e 6775 6c61 7220  of a triangular 
-00011a80: 6d61 7472 6978 2061 6e64 2069 7473 2074  matrix and its t
-00011a90: 7261 6e73 706f 7365 6420 6973 2075 7365  ransposed is use
-00011aa0: 643a 0a0a 2020 2020 2020 2020 202e 2e20  d:..         .. 
-00011ab0: 6d61 7468 3a3a 0a20 2020 2020 2020 2020  math::.         
-00011ac0: 2020 2056 203d 204c 204c 5e54 2e0a 0a20     V = L L^T... 
-00011ad0: 2020 2020 2020 2020 5468 6520 7661 6c75          The valu
-00011ae0: 6520 6f66 2074 6865 2063 6f73 7420 6675  e of the cost fu
-00011af0: 6e63 7469 6f6e 0a0a 2020 2020 2020 2020  nction..        
-00011b00: 202e 2e20 6d61 7468 3a3a 0a20 2020 2020   .. math::.     
-00011b10: 2020 2020 2020 5c63 6869 5e32 203d 207b        \chi^2 = {
-00011b20: 727d 5c63 646f 7420 2856 5e7b 2d31 7d7b  r}\cdot (V^{-1}{
-00011b30: 727d 2920 7e7e 7769 7468 7e7e 2072 203d  r}) ~~with~~ r =
-00011b40: 2079 202d 2066 2878 2c2a 7029 0a0a 2020   y - f(x,*p)..  
-00011b50: 2020 2020 2020 2069 7320 7468 656e 2063         is then c
-00011b60: 616c 6375 6c61 7465 6420 6279 2073 6f6c  alculated by sol
-00011b70: 7669 6e67 2074 6865 206c 696e 6561 7220  ving the linear 
-00011b80: 6571 7561 7469 6f6e 0a0a 2020 2020 2020  equation..      
-00011b90: 2020 2e2e 206d 6174 683a 3a0a 2020 2020    .. math::.    
-00011ba0: 2020 2020 2020 2056 2058 203d 2072 2c20         V X = r, 
-00011bb0: 7e69 2e65 2e7e 2058 3d56 5e7b 2d31 7d20  ~i.e.~ X=V^{-1} 
-00011bc0: 7220 7e61 6e64 7e20 5c63 6869 5e32 3d20  r ~and~ \chi^2= 
-00011bd0: 7220 5c63 646f 7420 580a 0a20 2020 2020  r \cdot X..     
-00011be0: 2020 2077 6974 6820 7468 6520 6c69 6e65     with the line
-00011bf0: 6172 2d65 7175 6174 696f 6e20 736f 6c76  ar-equation solv
-00011c00: 6572 202a 7363 6970 792e 6c69 6e61 6c67  er *scipy.linalg
-00011c10: 2e63 686f 5f73 6f6c 7665 284c 2c78 292a  .cho_solve(L,x)*
-00011c20: 0a20 2020 2020 2020 2066 6f72 2043 686f  .        for Cho
-00011c30: 6c65 736b 792d 6465 636f 6d70 6f73 6564  lesky-decomposed
-00011c40: 206d 6174 7269 6365 732c 2074 6875 7320   matrices, thus 
-00011c50: 6176 6f69 6469 6e67 2074 6865 2063 6f73  avoiding the cos
-00011c60: 7479 0a20 2020 2020 2020 2063 616c 6375  ty.        calcu
-00011c70: 6c61 7469 6f6e 206f 6620 7468 6520 696e  lation of the in
-00011c80: 7665 7273 6520 6d61 7472 6978 2e0a 0a0a  verse matrix....
-00011c90: 2020 2020 2020 2020 5468 6520 6465 7465          The dete
-00011ca0: 726d 696e 616e 742c 2069 6620 6e65 6564  rminant, if need
-00011cb0: 6564 2c20 6973 2065 6666 6963 6965 6e74  ed, is efficient
-00011cc0: 6c79 2063 616c 6375 6c61 7465 6420 6279  ly calculated by
-00011cd0: 2074 616b 696e 670a 2020 2020 2020 2020   taking.        
-00011ce0: 7468 6520 7072 6f64 7563 7420 6f66 2074  the product of t
-00011cf0: 6865 2064 6961 676f 6e61 6c20 656c 656d  he diagonal elem
-00011d00: 656e 7473 206f 6620 7468 6520 6d61 7472  ents of the matr
-00011d10: 6978 204c 2c0a 0a20 2020 2020 2020 2020  ix L,..         
-00011d20: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
-00011d30: 2020 2020 205c 6465 7428 5629 203d 2032       \det(V) = 2
-00011d40: 205c 2c20 5c70 726f 6420 4c5f 7b69 2c69   \, \prod L_{i,i
-00011d50: 7d0a 0a20 2020 2020 2020 2020 496e 7075  }..         Inpu
-00011d60: 743a 0a0a 2020 2020 2020 2020 202d 206f  t:..         - o
-00011d70: 7574 6572 3a20 706f 696e 7465 7220 746f  uter: pointer to
-00011d80: 2069 6e73 7461 6e63 6520 6f66 2063 616c   instance of cal
-00011d90: 6c69 6e67 2063 6c61 7373 0a20 2020 2020  ling class.     
-00011da0: 2020 2020 2d20 6d6f 6465 6c3a 206d 6f64      - model: mod
-00011db0: 656c 2066 756e 6374 696f 6e20 6628 782c  el function f(x,
-00011dc0: 205c 2a70 6172 290a 2020 2020 2020 2020   \*par).        
-00011dd0: 202d 2075 7365 5f6e 6567 326c 6f67 4c3a   - use_neg2logL:
-00011de0: 2075 7365 2066 756c 6c20 2d32 6c6f 6728   use full -2log(
-00011df0: 4c29 2069 6e73 7465 6164 206f 6620 6368  L) instead of ch
-00011e00: 6932 2069 6620 5472 7565 0a0a 2020 2020  i2 if True..    
-00011e10: 2020 2020 205f 5f63 616c 6c5f 5f20 6d65       __call__ me
-00011e20: 7468 6f64 206f 6620 7468 6973 2063 6c61  thod of this cla
-00011e30: 7373 2069 7320 6361 6c6c 6564 2062 7920  ss is called by 
-00011e40: 696d 696e 7569 740a 0a20 2020 2020 2020  iminuit..       
-00011e50: 2020 4461 7461 206d 656d 6265 7273 3a0a    Data members:.
-00011e60: 0a20 2020 2020 2020 2020 2d20 6e64 6f66  .         - ndof
-00011e70: 3a20 6465 6772 6565 7320 6f66 2066 7265  : degrees of fre
-00011e80: 6564 6f6d 0a20 2020 2020 2020 2020 2d20  edom.         - 
-00011e90: 6e63 6f6e 7374 7261 696e 7473 3a20 6e75  nconstraints: nu
-00011ea0: 6d62 6572 206f 6620 7061 7261 6d65 7465  mber of paramete
-00011eb0: 7220 636f 6e73 7472 6169 6e74 730a 2020  r constraints.  
-00011ec0: 2020 2020 2020 202d 2067 6f66 3a20 6368         - gof: ch
-00011ed0: 6932 2d76 616c 7565 2028 676f 6f64 6e65  i2-value (goodne
-00011ee0: 7373 206f 6620 6669 7429 0a20 2020 2020  ss of fit).     
-00011ef0: 2020 2020 2d20 7573 655f 6e65 6732 6c6f      - use_neg2lo
-00011f00: 674c 3a20 7573 6167 6520 6f66 2066 756c  gL: usage of ful
-00011f10: 6c20 322a 6e65 6720 4c6f 6720 4c69 6b65  l 2*neg Log Like
-00011f20: 6c69 686f 6f64 0a20 2020 2020 2020 2020  lihood.         
-00011f30: 2d20 7175 6965 743a 206e 6f20 7072 696e  - quiet: no prin
-00011f40: 746f 7574 2069 6620 5472 7565 0a0a 2020  tout if True..  
-00011f50: 2020 2020 2020 204d 6574 686f 6473 3a0a         Methods:.
-00011f60: 0a20 2020 2020 2020 2020 2d20 6d6f 6465  .         - mode
-00011f70: 6c28 782c 205c 2a70 6172 290a 2020 2020  l(x, \*par).    
-00011f80: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00011f90: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00011fa0: 6c66 2c20 6f75 7465 722c 206d 6f64 656c  lf, outer, model
-00011fb0: 2c20 7573 655f 6e65 6732 6c6f 674c 3d46  , use_neg2logL=F
-00011fc0: 616c 7365 293a 0a20 2020 2020 2020 2020  alse):.         
-00011fd0: 2020 2023 2064 6174 6120 6f62 6a65 6374     # data object
-00011fe0: 206f 6620 7479 7065 2078 7944 6174 6143   of type xyDataC
-00011ff0: 6f6e 7461 696e 6572 0a20 2020 2020 2020  ontainer.       
-00012000: 2020 2020 2073 656c 662e 6461 7461 203d       self.data =
-00012010: 206f 7574 6572 2e64 6174 610a 2020 2020   outer.data.    
-00012020: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00012030: 7369 6e73 7461 6e63 6528 7365 6c66 2e64  sinstance(self.d
-00012040: 6174 612c 206d 6e46 6974 2e78 7944 6174  ata, mnFit.xyDat
-00012050: 6143 6f6e 7461 696e 6572 293a 0a20 2020  aContainer):.   
-00012060: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00012070: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012090: 2020 2022 2021 2121 206d 6e46 6974 2e78     " !!! mnFit.x
-000120a0: 4c53 7143 6f73 743a 2065 7870 6563 7469  LSqCost: expecti
-000120b0: 6e67 2064 6174 6120 636f 6e74 6169 6e65  ng data containe
-000120c0: 7220 6f66 2074 7970 6520 276d 6e46 6974  r of type 'mnFit
-000120d0: 2e78 7944 6174 6143 6f6e 7461 696e 6572  .xyDataContainer
-000120e0: 2722 0a20 2020 2020 2020 2020 2020 2020  '".             
-000120f0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00012100: 2073 656c 662e 6d6f 6465 6c20 3d20 6d6f   self.model = mo
-00012110: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
-00012120: 7365 6c66 2e71 7569 6574 203d 206f 7574  self.quiet = out
-00012130: 6572 2e71 7569 6574 0a20 2020 2020 2020  er.quiet.       
-00012140: 2020 2020 2023 2075 7365 202d 3220 2a20       # use -2 * 
-00012150: 6c6f 6728 4c29 206f 6620 4761 7573 7369  log(L) of Gaussi
-00012160: 616e 2069 6e73 7465 6164 206f 6620 4368  an instead of Ch
-00012170: 6932 0a20 2020 2020 2020 2020 2020 2023  i2.            #
-00012180: 2020 286f 6e6c 7920 6469 6666 6572 656e    (only differen
-00012190: 7420 6672 6f6d 2043 6869 3220 666f 7220  t from Chi2 for 
-000121a0: 7061 7261 6d65 7465 722d 6465 7065 6e64  parameter-depend
-000121b0: 656e 7420 756e 6365 7274 6169 6e74 6965  ent uncertaintie
-000121c0: 7329 0a20 2020 2020 2020 2020 2020 2073  s).            s
-000121d0: 656c 662e 7573 655f 6e65 6732 6c6f 674c  elf.use_neg2logL
-000121e0: 203d 2075 7365 5f6e 6567 326c 6f67 4c0a   = use_neg2logL.
-000121f0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00012200: 6574 2070 726f 7065 7220 7369 676e 6174  et proper signat
-00012210: 7572 6520 6f66 206d 6f64 656c 2066 756e  ure of model fun
-00012220: 6374 696f 6e20 666f 7220 696d 696e 7569  ction for iminui
-00012230: 740a 2020 2020 2020 2020 2020 2020 7365  t.            se
-00012240: 6c66 2e70 6e61 6d73 203d 206f 7574 6572  lf.pnams = outer
-00012250: 2e70 6e61 6d73 0a20 2020 2020 2020 2020  .pnams.         
-00012260: 2020 2073 656c 662e 6e70 6172 203d 206f     self.npar = o
-00012270: 7574 6572 2e6e 7061 720a 0a20 2020 2020  uter.npar..     
-00012280: 2020 2020 2020 2023 2074 616b 6520 6163         # take ac
-00012290: 636f 756e 7420 6f66 2063 6f6e 7374 7261  count of constra
-000122a0: 696e 7473 0a20 2020 2020 2020 2020 2020  ints.           
-000122b0: 2073 656c 662e 636f 6e73 7472 6169 6e74   self.constraint
-000122c0: 7320 3d20 6f75 7465 722e 636f 6e73 7472  s = outer.constr
-000122d0: 6169 6e74 730a 2020 2020 2020 2020 2020  aints.          
-000122e0: 2020 7365 6c66 2e6e 636f 6e73 7472 6169    self.nconstrai
-000122f0: 6e74 7320 3d20 6c65 6e28 7365 6c66 2e63  nts = len(self.c
-00012300: 6f6e 7374 7261 696e 7473 290a 2020 2020  onstraints).    
-00012310: 2020 2020 2020 2020 7365 6c66 2e6e 646f          self.ndo
-00012320: 6620 3d20 6c65 6e28 7365 6c66 2e64 6174  f = len(self.dat
-00012330: 612e 7929 202d 2073 656c 662e 6e70 6172  a.y) - self.npar
-00012340: 202b 2073 656c 662e 6e63 6f6e 7374 7261   + self.nconstra
-00012350: 696e 7473 202b 206f 7574 6572 2e6e 6669  ints + outer.nfi
-00012360: 7865 640a 0a20 2020 2020 2020 2020 2020  xed..           
-00012370: 2023 2066 6c61 6720 746f 2063 6f6e 7472   # flag to contr
-00012380: 6f6c 2066 696e 616c 2061 6374 696f 6e73  ol final actions
-00012390: 2069 6e20 636f 7374 2066 756e 6374 696f   in cost functio
-000123a0: 6e0a 2020 2020 2020 2020 2020 2020 7365  n.            se
-000123b0: 6c66 2e66 696e 616c 5f63 616c 6c20 3d20  lf.final_call = 
-000123c0: 4661 6c73 650a 0a20 2020 2020 2020 2064  False..        d
-000123d0: 6566 205f 5f63 616c 6c5f 5f28 7365 6c66  ef __call__(self
-000123e0: 2c20 2a70 6172 293a 0a20 2020 2020 2020  , *par):.       
-000123f0: 2020 2020 2023 2063 616c 6c65 6420 6974       # called it
-00012400: 6572 6174 6976 656c 7920 6279 206d 696e  eratively by min
-00012410: 7569 740a 0a20 2020 2020 2020 2020 2020  uit..           
-00012420: 2023 2063 6f73 7420 6675 6e63 7469 6f6e   # cost function
-00012430: 2069 7320 6578 7465 6e64 6564 2063 6869   is extended chi
-00012440: 323a 0a20 2020 2020 2020 2020 2020 2023  2:.            #
-00012450: 2020 2061 6464 206e 6f72 6d61 6c69 7a61     add normaliza
-00012460: 7469 6f6e 2074 6572 6d20 6966 2075 6e63  tion term if unc
-00012470: 6572 7461 696e 7469 6573 2064 6570 656e  ertainties depen
-00012480: 6420 6f6e 206d 6f64 656c 0a0a 2020 2020  d on model..    
-00012490: 2020 2020 2020 2020 6e6c 4c32 203d 2030          nlL2 = 0
-000124a0: 2e30 2020 2320 696e 6974 6961 6c69 7a65  .0  # initialize
-000124b0: 202d 322a 6c6e 284c 290a 2020 2020 2020   -2*ln(L).      
-000124c0: 2020 2020 2020 2320 2066 6972 7374 2c20        #  first, 
-000124d0: 7461 6b65 2069 6e74 6f20 6163 636f 756e  take into accoun
-000124e0: 7420 706f 7373 6962 6c65 2070 6172 616d  t possible param
-000124f0: 6574 6572 2063 6f6e 7374 7261 696e 7473  eter constraints
-00012500: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00012510: 7365 6c66 2e6e 636f 6e73 7472 6169 6e74  self.nconstraint
-00012520: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00012530: 2020 2066 6f72 2063 2069 6e20 7365 6c66     for c in self
-00012540: 2e63 6f6e 7374 7261 696e 7473 3a0a 2020  .constraints:.  
-00012550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012560: 2020 705f 6964 203d 2063 5b30 5d0a 2020    p_id = c[0].  
-00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012580: 2020 7220 3d20 2870 6172 5b70 5f69 645d    r = (par[p_id]
-00012590: 202d 2063 5b31 5d29 202f 2063 5b32 5d0a   - c[1]) / c[2].
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 2020 2020 6e6c 4c32 202b 3d20 7220 2a20      nlL2 += r * 
-000125c0: 720a 0a20 2020 2020 2020 2020 2020 2023  r..            #
-000125d0: 2063 616c 6375 6c61 7465 2072 6573 6964   calculate resid
-000125e0: 7561 6c20 6f66 2064 6174 6120 7772 742e  ual of data wrt.
-000125f0: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
-00012600: 2020 206d 6f64 656c 5f76 616c 7565 7320     model_values 
-00012610: 3d20 7365 6c66 2e6d 6f64 656c 2873 656c  = self.model(sel
-00012620: 662e 6461 7461 2e78 2c20 2a70 6172 290a  f.data.x, *par).
-00012630: 2020 2020 2020 2020 2020 2020 5f72 203d              _r =
-00012640: 2073 656c 662e 6461 7461 2e79 202d 206d   self.data.y - m
-00012650: 6f64 656c 5f76 616c 7565 730a 0a20 2020  odel_values..   
-00012660: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00012670: 2e64 6174 612e 6e65 6564 735f 636f 7661  .data.needs_cova
-00012680: 7269 616e 6365 3a0a 2020 2020 2020 2020  riance:.        
-00012690: 2020 2020 2020 2020 2320 2063 6865 636b          #  check
-000126a0: 2069 6620 6d61 7472 6978 206e 6565 6473   if matrix needs
-000126b0: 2072 6562 7569 6c64 696e 670a 2020 2020   rebuilding.    
-000126c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000126d0: 6f74 2073 656c 662e 6461 7461 2e6e 6565  ot self.data.nee
-000126e0: 6473 5f64 796e 616d 6963 4572 726f 7273  ds_dynamicErrors
-000126f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012700: 2020 2020 2020 2320 7374 6174 6963 2063        # static c
-00012710: 6f76 6172 6961 6e63 652c 2075 7365 2069  ovariance, use i
-00012720: 7473 2069 6e76 6572 7365 0a20 2020 2020  ts inverse.     
-00012730: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00012740: 6c4c 3220 2b3d 2066 6c6f 6174 286e 702e  lL2 += float(np.
-00012750: 696e 6e65 7228 6e70 2e6d 6174 6d75 6c28  inner(np.matmul(
-00012760: 5f72 2c20 7365 6c66 2e64 6174 612e 6943  _r, self.data.iC
-00012770: 6f76 292c 205f 7229 290a 2020 2020 2020  ov), _r)).      
-00012780: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00012790: 6964 656e 7469 6361 6c20 746f 2063 6c61  identical to cla
-000127a0: 7373 6963 616c 2043 6869 320a 2020 2020  ssical Chi2.    
-000127b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127c0: 7365 6c66 2e67 6f66 203d 206e 6c4c 320a  self.gof = nlL2.
-000127d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000127e0: 2065 6c73 653a 2020 2320 6479 6e61 6d69   else:  # dynami
-000127f0: 6361 6c6c 7920 7265 6275 696c 6420 636f  cally rebuild co
-00012800: 7661 7269 616e 6365 206d 6174 7269 780a  variance matrix.
-00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012820: 2020 2020 7365 6c66 2e64 6174 612e 5f72      self.data._r
-00012830: 6562 7569 6c64 5f43 6f76 2870 6172 290a  ebuild_Cov(par).
-00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012850: 2020 2020 2320 7573 6520 4368 6f6c 6573      # use Choles
-00012860: 6b79 2064 6563 6f6d 706f 7369 746f 6e20  ky decompositon 
-00012870: 746f 2063 6f6d 7075 7465 2063 6869 3220  to compute chi2 
-00012880: 3d20 5f72 2e54 2028 565e 2d31 2920 5f72  = _r.T (V^-1) _r
-00012890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000128a0: 2020 2020 204c 2c20 6973 5f6c 6f77 6572       L, is_lower
-000128b0: 203d 206c 696e 616c 672e 6368 6f5f 6661   = linalg.cho_fa
-000128c0: 6374 6f72 2873 656c 662e 6461 7461 2e63  ctor(self.data.c
-000128d0: 6f76 2c20 6368 6563 6b5f 6669 6e69 7465  ov, check_finite
-000128e0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-000128f0: 2020 2020 2020 2020 2020 2020 6e6c 4c32              nlL2
-00012900: 202b 3d20 6e70 2e69 6e6e 6572 285f 722c   += np.inner(_r,
-00012910: 206c 696e 616c 672e 6368 6f5f 736f 6c76   linalg.cho_solv
-00012920: 6528 284c 2c20 6973 5f6c 6f77 6572 292c  e((L, is_lower),
-00012930: 205f 7229 290a 2020 2020 2020 2020 2020   _r)).          
-00012940: 2020 2020 2020 2020 2020 2320 7570 2074            # up t
-00012950: 6f20 6865 7265 2c20 6964 656e 7469 6361  o here, identica
-00012960: 6c20 746f 2063 6c61 7373 6963 616c 2043  l to classical C
-00012970: 6869 320a 2020 2020 2020 2020 2020 2020  hi2.            
-00012980: 2020 2020 2020 2020 7365 6c66 2e67 6f66          self.gof
-00012990: 203d 206e 6c4c 320a 2020 2020 2020 2020   = nlL2.        
-000129a0: 2020 2020 2020 2020 2020 2020 2320 7461              # ta
-000129b0: 6b65 2069 6e74 6f20 6163 636f 756e 7420  ke into account 
-000129c0: 7061 7261 6d65 7465 722d 6465 7065 6e64  parameter-depend
-000129d0: 656e 7420 6e6f 726d 616c 6973 6174 696f  ent normalisatio
-000129e0: 6e20 7465 726d 0a20 2020 2020 2020 2020  n term.         
-000129f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00012a00: 6c66 2e75 7365 5f6e 6567 326c 6f67 4c3a  lf.use_neg2logL:
-00012a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012a20: 2020 2020 2020 2020 2023 2020 6661 7374           #  fast
-00012a30: 2063 616c 6375 6c61 7469 6f6e 206f 6620   calculation of 
-00012a40: 6465 7465 726d 696e 616e 7420 6465 7428  determinant det(
-00012a50: 5629 2066 726f 6d20 4368 6f6c 6573 6b79  V) from Cholesky
-00012a60: 2066 6163 746f 720a 2020 2020 2020 2020   factor.        
+000106b0: 2020 2020 2020 202d 2073 656c 662e 6d6f         - self.mo
+000106c0: 6465 6c28 7365 6c66 2e78 202d 2073 656c  del(self.x - sel
+000106d0: 662e 5f64 782c 202a 6d70 6172 290a 2020  f._dx, *mpar).  
+000106e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106f0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00010700: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00010710: 2020 2020 2020 2320 7072 6f6a 6563 7420        # project 
+00010720: 6f6e 2079 2061 6e64 2061 6464 2074 6f20  on y and add to 
+00010730: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+00010740: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+00010750: 2020 7365 6c66 2e65 7272 3220 2b3d 205f    self.err2 += _
+00010760: 6d70 7269 6d65 202a 205f 6d70 7269 6d65  mprime * _mprime
+00010770: 202a 2073 656c 662e 6572 7232 780a 0a20   * self.err2x.. 
+00010780: 2020 2020 2020 2064 6566 205f 7265 6275         def _rebu
+00010790: 696c 645f 436f 7628 7365 6c66 2c20 6d70  ild_Cov(self, mp
+000107a0: 6172 293a 0a20 2020 2020 2020 2020 2020  ar):.           
+000107b0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
+000107c0: 2028 5265 2d29 4275 696c 6420 7468 6520   (Re-)Build the 
+000107d0: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+000107e0: 7820 6672 6f6d 2063 6f6d 706f 6e65 6e74  x from component
+000107f0: 730a 2020 2020 2020 2020 2020 2020 616e  s.            an
+00010800: 6420 6361 636c 756c 6174 6520 6974 7320  d caclulate its 
+00010810: 696e 7665 7273 650a 2020 2020 2020 2020  inverse.        
+00010820: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010830: 2020 2020 2320 7374 6172 7420 6672 6f6d      # start from
+00010840: 2070 7265 2d62 7569 6c74 2070 6172 616d   pre-built param
+00010850: 6574 6572 2d69 6e64 6570 656e 6465 6e74  eter-independent
+00010860: 2070 6172 7420 6f66 2043 6f76 6172 6961   part of Covaria
+00010870: 6e63 6520 4d61 7472 6978 0a20 2020 2020  nce Matrix.     
+00010880: 2020 2020 2020 2073 656c 662e 636f 7620         self.cov 
+00010890: 3d20 6e70 2e61 7272 6179 2873 656c 662e  = np.array(self.
+000108a0: 5f73 7461 7469 6343 6f76 2c20 636f 7079  _staticCov, copy
+000108b0: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
+000108c0: 2020 2020 2320 6164 6420 6d61 7472 6978      # add matrix
+000108d0: 206f 6620 7061 7261 6d65 7465 722d 6465   of parameter-de
+000108e0: 7065 6e64 656e 7420 792d 756e 6365 7274  pendent y-uncert
+000108f0: 6169 6e74 6965 730a 2020 2020 2020 2020  ainties.        
+00010900: 2020 2020 2320 2020 2020 2069 6620 7365      #      if se
+00010910: 6c66 2e72 6566 5f74 6f4d 6f64 656c 2061  lf.ref_toModel a
+00010920: 6e64 2073 656c 662e 6861 735f 7265 6c5f  nd self.has_rel_
+00010930: 7945 7272 6f72 733a 0a20 2020 2020 2020  yErrors:.       
+00010940: 2020 2020 2069 6620 7365 6c66 2e5f 636f       if self._co
+00010950: 7679 3020 6973 206e 6f74 204e 6f6e 653a  vy0 is not None:
+00010960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010970: 205f 7964 6174 203d 2073 656c 662e 6d6f   _ydat = self.mo
+00010980: 6465 6c28 7365 6c66 2e78 2c20 2a6d 7061  del(self.x, *mpa
+00010990: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+000109a0: 2020 2073 656c 662e 636f 7620 2b3d 2073     self.cov += s
+000109b0: 656c 662e 5f63 6f76 7930 202a 206e 702e  elf._covy0 * np.
+000109c0: 6f75 7465 7228 5f79 6461 742c 205f 7964  outer(_ydat, _yd
+000109d0: 6174 290a 2020 2020 2020 2020 2020 2020  at).            
+000109e0: 2320 6164 6420 7072 6f6a 6563 7465 6420  # add projected 
+000109f0: 7820 6572 726f 7273 0a20 2020 2020 2020  x errors.       
+00010a00: 2020 2020 2069 6620 7365 6c66 2e68 6173       if self.has
+00010a10: 5f78 4572 726f 7273 3a0a 2020 2020 2020  _xErrors:.      
+00010a20: 2020 2020 2020 2020 2020 2320 7374 6f72            # stor
+00010a30: 6520 636f 7661 7269 616e 6365 206d 6174  e covariance mat
+00010a40: 7269 7820 6f66 2079 2d75 6e63 6572 7461  rix of y-uncerta
+00010a50: 696e 7469 6573 0a20 2020 2020 2020 2020  inties.         
+00010a60: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+00010a70: 696e 616c 5f63 616c 6c3a 0a20 2020 2020  inal_call:.     
+00010a80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00010a90: 656c 662e 636f 7679 203d 206e 702e 6172  elf.covy = np.ar
+00010aa0: 7261 7928 7365 6c66 2e63 6f76 2c20 636f  ray(self.cov, co
+00010ab0: 7079 3d54 7275 6529 0a0a 2020 2020 2020  py=True)..      
+00010ac0: 2020 2020 2020 2020 2020 2320 6465 7465            # dete
+00010ad0: 726d 696e 6520 6465 7269 7661 7469 7665  rmine derivative
+00010ae0: 7320 6f66 206d 6f64 656c 2066 756e 6374  s of model funct
+00010af0: 696f 6e20 772e 722e 742e 2078 2c0a 2020  ion w.r.t. x,.  
+00010b00: 2020 2020 2020 2020 2020 2020 2020 5f6d                _m
+00010b10: 7072 696d 6520 3d20 280a 2020 2020 2020  prime = (.      
+00010b20: 2020 2020 2020 2020 2020 2020 2020 302e                0.
+00010b30: 350a 2020 2020 2020 2020 2020 2020 2020  5.              
+00010b40: 2020 2020 2020 2f20 7365 6c66 2e5f 6478        / self._dx
+00010b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010b60: 2020 2020 202a 2028 0a20 2020 2020 2020       * (.       
+00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b80: 2073 656c 662e 6d6f 6465 6c28 7365 6c66   self.model(self
+00010b90: 2e78 202b 2073 656c 662e 5f64 782c 202a  .x + self._dx, *
+00010ba0: 6d70 6172 290a 2020 2020 2020 2020 2020  mpar).          
+00010bb0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00010bc0: 7365 6c66 2e6d 6f64 656c 2873 656c 662e  self.model(self.
+00010bd0: 7820 2d20 7365 6c66 2e5f 6478 2c20 2a6d  x - self._dx, *m
+00010be0: 7061 7229 0a20 2020 2020 2020 2020 2020  par).           
+00010bf0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00010c00: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010c10: 2020 2020 2020 2020 2020 2020 2023 2070               # p
+00010c20: 726f 6a65 6374 206f 6e20 7920 616e 6420  roject on y and 
+00010c30: 6164 6420 746f 2063 6f76 6172 6961 6e63  add to covarianc
+00010c40: 6520 6d61 7472 6978 0a20 2020 2020 2020  e matrix.       
+00010c50: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00010c60: 7620 2b3d 206e 702e 6f75 7465 7228 5f6d  v += np.outer(_m
+00010c70: 7072 696d 652c 205f 6d70 7269 6d65 2920  prime, _mprime) 
+00010c80: 2a20 7365 6c66 2e63 6f76 780a 2020 2020  * self.covx.    
+00010c90: 2020 2020 2020 2020 656c 7365 3a20 2023          else:  #
+00010ca0: 206e 6f20 782d 6572 726f 7273 2c20 792d   no x-errors, y-
+00010cb0: 636f 766d 6174 203d 2063 6f76 6d61 740a  covmat = covmat.
+00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010cd0: 7365 6c66 2e63 6f76 7920 3d20 7365 6c66  self.covy = self
+00010ce0: 2e63 6f76 0a0a 2020 2020 2020 2020 6465  .cov..        de
+00010cf0: 6620 6765 745f 436f 7628 7365 6c66 293a  f get_Cov(self):
+00010d00: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+00010d10: 7265 7475 726e 2063 6f76 6172 6961 6e63  return covarianc
+00010d20: 6520 6d61 7472 6978 206f 6620 6461 7461  e matrix of data
+00010d30: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
+00010d40: 6966 2073 656c 662e 6e65 6564 735f 636f  if self.needs_co
+00010d50: 7661 7269 616e 6365 3a0a 2020 2020 2020  variance:.      
+00010d60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010d70: 2073 656c 662e 636f 760a 2020 2020 2020   self.cov.      
+00010d80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00010d90: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00010da0: 656c 662e 6572 7232 2069 7320 4e6f 6e65  elf.err2 is None
+00010db0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010dc0: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00010dd0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00010de0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010df0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00010e00: 726e 206e 702e 6469 6167 2873 656c 662e  rn np.diag(self.
+00010e10: 6572 7232 290a 0a20 2020 2020 2020 2064  err2)..        d
+00010e20: 6566 2067 6574 5f78 436f 7628 7365 6c66  ef get_xCov(self
+00010e30: 293a 0a20 2020 2020 2020 2020 2020 2022  ):.            "
+00010e40: 2222 7265 7475 726e 2063 6f76 6172 6961  ""return covaria
+00010e50: 6e63 6520 6d61 7472 6978 206f 6620 782d  nce matrix of x-
+00010e60: 6461 7461 2222 220a 2020 2020 2020 2020  data""".        
+00010e70: 2020 2020 6966 2073 656c 662e 6e65 6564      if self.need
+00010e80: 735f 636f 7661 7269 616e 6365 3a0a 2020  s_covariance:.  
+00010e90: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00010ea0: 7475 726e 2073 656c 662e 636f 7678 0a20  turn self.covx. 
+00010eb0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00010ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ed0: 2069 6620 7365 6c66 2e65 7272 3278 2069   if self.err2x i
+00010ee0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00010ef0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00010f00: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+00010f10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 2020 7265 7475 726e 206e 702e 6469 6167    return np.diag
+00010f40: 2873 656c 662e 6572 7232 7829 0a0a 2020  (self.err2x)..  
+00010f50: 2020 2020 2020 6465 6620 6765 745f 7943        def get_yC
+00010f60: 6f76 2873 656c 6629 3a0a 2020 2020 2020  ov(self):.      
+00010f70: 2020 2020 2020 2222 2272 6574 7572 6e20        """return 
+00010f80: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+00010f90: 7820 6f66 2079 2d64 6174 6122 2222 0a20  x of y-data""". 
+00010fa0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00010fb0: 6c66 2e6e 6565 6473 5f63 6f76 6172 6961  lf.needs_covaria
+00010fc0: 6e63 653a 0a20 2020 2020 2020 2020 2020  nce:.           
+00010fd0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00010fe0: 2e63 6f76 790a 2020 2020 2020 2020 2020  .covy.          
+00010ff0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00011000: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00011010: 6572 7232 7920 6973 204e 6f6e 653a 0a20  err2y is None:. 
+00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011030: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+00011040: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011050: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00011060: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011070: 6e70 2e64 6961 6728 7365 6c66 2e65 7272  np.diag(self.err
+00011080: 3279 290a 0a20 2020 2020 2020 2064 6566  2y)..        def
+00011090: 2067 6574 5f69 436f 7628 7365 6c66 293a   get_iCov(self):
+000110a0: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
+000110b0: 7265 7475 726e 2069 6e76 6572 7365 206f  return inverse o
+000110c0: 6620 636f 7661 7269 616e 6365 206d 6174  f covariance mat
+000110d0: 7269 782c 2061 7320 7573 6564 2069 6e20  rix, as used in 
+000110e0: 636f 7374 2066 756e 6374 696f 6e22 2222  cost function"""
+000110f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011100: 7365 6c66 2e6e 6565 6473 5f63 6f76 6172  self.needs_covar
+00011110: 6961 6e63 653a 0a20 2020 2020 2020 2020  iance:.         
+00011120: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011130: 6c66 2e69 436f 760a 2020 2020 2020 2020  lf.iCov.        
+00011140: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00011150: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011160: 206e 702e 6469 6167 2831 2e30 202f 2073   np.diag(1.0 / s
+00011170: 656c 662e 6572 7232 290a 0a20 2020 2020  elf.err2)..     
+00011180: 2020 2064 6566 2070 6c6f 7428 0a20 2020     def plot(.   
+00011190: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+000111a0: 2020 2020 2020 2020 2020 206e 756d 3d22             num="
+000111b0: 7879 4461 7461 2061 6e64 204d 6f64 656c  xyData and Model
+000111c0: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
+000111d0: 6967 7369 7a65 3d28 372e 352c 2036 2e35  igsize=(7.5, 6.5
+000111e0: 292c 0a20 2020 2020 2020 2020 2020 2064  ),.            d
+000111f0: 6174 615f 6c61 6265 6c3d 2264 6174 6122  ata_label="data"
+00011200: 2c0a 2020 2020 2020 2020 2020 2020 706c  ,.            pl
+00011210: 6f74 5f72 6573 6964 7561 6c3d 4661 6c73  ot_residual=Fals
+00011220: 652c 0a20 2020 2020 2020 2029 3a0a 2020  e,.        ):.  
+00011230: 2020 2020 2020 2020 2020 2222 2272 6574            """ret
+00011240: 7572 6e20 6669 6775 7265 2077 6974 6820  urn figure with 
+00011250: 7879 2064 6174 6120 616e 6420 756e 6365  xy data and unce
+00011260: 7274 6169 6e74 6965 7322 2222 0a20 2020  rtainties""".   
+00011270: 2020 2020 2020 2020 2023 2020 2020 2320           #    # 
+00011280: 6765 7420 6461 7461 0a20 2020 2020 2020  get data.       
+00011290: 2020 2020 2078 203d 2073 656c 662e 780a       x = self.x.
+000112a0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+000112b0: 6c6f 745f 7265 7369 6475 616c 2061 6e64  lot_residual and
+000112c0: 2073 656c 662e 6d6f 6465 6c5f 7661 6c75   self.model_valu
+000112d0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+000112e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112f0: 7920 3d20 7365 6c66 2e79 202d 2073 656c  y = self.y - sel
+00011300: 662e 6d6f 6465 6c5f 7661 6c75 6573 0a20  f.model_values. 
+00011310: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00011320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011330: 2079 203d 2073 656c 662e 790a 2020 2020   y = self.y.    
+00011340: 2020 2020 2020 2020 6579 203d 2073 656c          ey = sel
+00011350: 662e 6765 745f 7943 6f76 2829 0a20 2020  f.get_yCov().   
+00011360: 2020 2020 2020 2020 2069 6620 6579 2e6e           if ey.n
+00011370: 6469 6d20 3d3d 2032 3a0a 2020 2020 2020  dim == 2:.      
+00011380: 2020 2020 2020 2020 2020 6579 203d 206e            ey = n
+00011390: 702e 7371 7274 286e 702e 6469 6167 6f6e  p.sqrt(np.diagon
+000113a0: 616c 2865 7929 290a 2020 2020 2020 2020  al(ey)).        
+000113b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000113c0: 2020 2020 2020 2020 2020 6579 203d 206e            ey = n
+000113d0: 702e 7371 7274 2865 7929 0a20 2020 2020  p.sqrt(ey).     
+000113e0: 2020 2020 2020 2065 7820 3d20 7365 6c66         ex = self
+000113f0: 2e67 6574 5f78 436f 7628 290a 2020 2020  .get_xCov().    
+00011400: 2020 2020 2020 2020 6966 2065 7820 6973          if ex is
+00011410: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00011420: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
+00011430: 2e6e 6469 6d20 3d3d 2032 3a0a 2020 2020  .ndim == 2:.    
+00011440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011450: 6578 203d 206e 702e 7371 7274 286e 702e  ex = np.sqrt(np.
+00011460: 6469 6167 6f6e 616c 2865 7829 290a 2020  diagonal(ex)).  
+00011470: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00011480: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00011490: 2020 2020 2020 2020 6578 203d 206e 702e          ex = np.
+000114a0: 7371 7274 2865 7829 0a20 2020 2020 2020  sqrt(ex).       
+000114b0: 2020 2020 2023 2064 7261 7720 6461 7461       # draw data
+000114c0: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
+000114d0: 203d 2070 6c74 2e66 6967 7572 6528 6e75   = plt.figure(nu
+000114e0: 6d3d 6e75 6d2c 2066 6967 7369 7a65 3d66  m=num, figsize=f
+000114f0: 6967 7369 7a65 290a 2020 2020 2020 2020  igsize).        
+00011500: 2020 2020 706c 742e 706c 6f74 2878 2c20      plt.plot(x, 
+00011510: 792c 206d 6172 6b65 723d 2278 222c 206c  y, marker="x", l
+00011520: 696e 6573 7479 6c65 3d22 222c 2063 6f6c  inestyle="", col
+00011530: 6f72 3d22 6772 6579 222c 2061 6c70 6861  or="grey", alpha
+00011540: 3d30 2e35 290a 2020 2020 2020 2020 2020  =0.5).          
+00011550: 2020 6966 2065 7820 6973 206e 6f74 204e    if ex is not N
+00011560: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00011570: 2020 2020 2070 6c74 2e65 7272 6f72 6261       plt.errorba
+00011580: 7228 782c 2079 2c20 7865 7272 3d65 782c  r(x, y, xerr=ex,
+00011590: 2079 6572 723d 6579 2c20 666d 743d 222e   yerr=ey, fmt=".
+000115a0: 222c 206c 6162 656c 3d64 6174 615f 6c61  ", label=data_la
+000115b0: 6265 6c29 0a20 2020 2020 2020 2020 2020  bel).           
+000115c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000115d0: 2020 2020 2020 2070 6c74 2e65 7272 6f72         plt.error
+000115e0: 6261 7228 782c 2079 2c20 6579 2c20 666d  bar(x, y, ey, fm
+000115f0: 743d 222e 222c 206c 6162 656c 3d64 6174  t=".", label=dat
+00011600: 615f 6c61 6265 6c29 0a20 2020 2020 2020  a_label).       
+00011610: 2020 2020 2072 6574 7572 6e20 6669 670a       return fig.
+00011620: 0a20 2020 2023 2064 6566 696e 6520 6375  .    # define cu
+00011630: 7374 6f6d 2063 6f73 7420 6675 6e63 7469  stom cost functi
+00011640: 6f6e 2066 6f72 2069 6d69 6e75 6974 0a20  on for iminuit. 
+00011650: 2020 2063 6c61 7373 2078 4c53 7143 6f73     class xLSqCos
+00011660: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+00011670: 2020 2020 2020 2020 4375 7374 6f6d 2065          Custom e
+00011680: 5f78 5f74 656e 6465 6420 4c65 6173 742d  _x_tended Least-
+00011690: 5351 7561 7265 7320 636f 7374 2066 756e  SQuares cost fun
+000116a0: 6374 696f 6e20 7769 7468 0a20 2020 2020  ction with.     
+000116b0: 2020 2020 6479 6e61 6d69 6361 6c6c 7920      dynamically 
+000116c0: 7570 6461 7465 6420 636f 7661 7269 616e  updated covarian
+000116d0: 6365 206d 6174 7269 7820 616e 6420 2d32  ce matrix and -2
+000116e0: 6c6f 6728 4c29 0a20 2020 2020 2020 2020  log(L).         
+000116f0: 636f 7272 6563 7469 6f6e 2074 6572 6d20  correction term 
+00011700: 666f 7220 7061 7261 6d65 7465 722d 6465  for parameter-de
+00011710: 7065 6e64 656e 7420 756e 6365 7274 6169  pendent uncertai
+00011720: 6e74 6965 732e 0a0a 2020 2020 2020 2020  nties...        
+00011730: 2054 6865 2064 6566 6175 6c74 2063 6f73   The default cos
+00011740: 7420 6675 6e63 7469 6f6e 2069 7320 7477  t function is tw
+00011750: 6963 6520 7468 6520 6e65 6761 7469 7665  ice the negative
+00011760: 206c 6f67 6172 6974 686d 0a20 2020 2020   logarithm.     
+00011770: 2020 2020 6f66 2074 6865 206c 696b 656c      of the likel
+00011780: 6968 6f6f 6420 6f66 2061 2047 6175 7373  ihood of a Gauss
+00011790: 6961 6e20 6469 7374 7269 6275 7469 6f6e  ian distribution
+000117a0: 2066 6f72 2064 6174 6120 706f 696e 7473   for data points
+000117b0: 0a20 2020 2020 2020 2020 3a6d 6174 683a  .         :math:
+000117c0: 6028 782c 2079 2960 2077 6974 6820 6120  `(x, y)` with a 
+000117d0: 6d6f 6465 6c20 6675 6e63 7469 6f6e 203a  model function :
+000117e0: 6d61 7468 3a60 793d 6628 782c 202a 7029  math:`y=f(x, *p)
+000117f0: 6020 6465 7065 6e64 696e 670a 2020 2020  ` depending.    
+00011800: 2020 2020 206f 6e20 6120 7365 7420 6f66       on a set of
+00011810: 2070 6172 616d 6574 6572 7320 3a6d 6174   parameters :mat
+00011820: 683a 602a 7060 2061 6e64 2061 2070 6f73  h:`*p` and a pos
+00011830: 7369 626c 7920 7061 7261 6d65 7465 722d  sibly parameter-
+00011840: 6465 7065 6e64 656e 740a 2020 2020 2020  dependent.      
+00011850: 2020 2063 6f76 6172 6961 6e63 6520 6d61     covariance ma
+00011860: 7472 6978 203a 6d61 7468 3a60 5628 782c  trix :math:`V(x,
+00011870: 2066 2878 2c20 2a70 2929 6020 6f66 2074   f(x, *p))` of t
+00011880: 6865 2078 2061 6e64 2079 2064 6174 613a  he x and y data:
+00011890: 0a0a 2020 2020 2020 2020 202e 2e20 6d61  ..         .. ma
+000118a0: 7468 3a3a 0a20 2020 2020 2020 2020 2020  th::.           
+000118b0: 2d32 5c6c 6e20 7b5c 6361 6c20 4c7d 203d  -2\ln {\cal L} =
+000118c0: 205c 6368 695e 3228 792c 2056 5e7b 2d31   \chi^2(y, V^{-1
+000118d0: 7d2c 2066 2878 2c20 2a70 2920 5c2c 290a  }, f(x, *p) \,).
+000118e0: 2020 2020 2020 2020 2020 202b 205c 6c6e             + \ln
+000118f0: 285c 2c20 5c64 6574 2820 5628 782c 2066  (\, \det( V(x, f
+00011900: 2878 2c20 2a70 2920 2920 5c2c 290a 0a20  (x, *p) ) \,).. 
+00011910: 2020 2020 2020 2020 496e 2074 6865 2061          In the a
+00011920: 6273 656e 6365 206f 6620 7061 7261 6d65  bsence of parame
+00011930: 7465 722d 6465 7065 6e64 656e 7420 636f  ter-dependent co
+00011940: 6d70 6f6e 656e 7473 206f 6620 7468 6520  mponents of the 
+00011950: 636f 7661 7269 616e 6365 0a20 2020 2020  covariance.     
+00011960: 2020 2020 6d61 7472 6978 2c20 7468 6520      matrix, the 
+00011970: 6c61 7374 2074 6572 6d20 6973 206f 6d69  last term is omi
+00011980: 7474 6564 2061 6e64 2074 6865 2063 6f73  tted and the cos
+00011990: 7420 6675 6e63 7469 6f6e 2069 7320 6964  t function is id
+000119a0: 656e 7469 6361 6c0a 2020 2020 2020 2020  entical.        
+000119b0: 2074 6f20 7468 6520 636c 6173 7369 6361   to the classica
+000119c0: 6c20 3a6d 6174 683a 605c 6368 695e 3260  l :math:`\chi^2`
+000119d0: 2e0a 2020 2020 2020 2020 2046 6f72 2074  ..         For t
+000119e0: 6865 2065 7661 6c75 6174 696f 6e20 6f66  he evaluation of
+000119f0: 2074 6865 2063 6f73 7420 6675 6e63 7469   the cost functi
+00011a00: 6f6e 2061 6e20 6566 6669 6369 656e 7420  on an efficient 
+00011a10: 6170 7072 6f61 6368 2062 6173 6564 0a20  approach based. 
+00011a20: 2020 2020 2020 2020 6f6e 2074 6865 2022          on the "
+00011a30: 4368 6f6c 6573 6b79 2064 6563 6f6d 706f  Cholesky decompo
+00011a40: 7369 7469 6f6e 2220 6f66 2074 6865 2063  sition" of the c
+00011a50: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+00011a60: 2069 6e0a 2020 2020 2020 2020 2061 2070   in.         a p
+00011a70: 726f 6475 6374 206f 6620 6120 7472 6961  roduct of a tria
+00011a80: 6e67 756c 6172 206d 6174 7269 7820 616e  ngular matrix an
+00011a90: 6420 6974 7320 7472 616e 7370 6f73 6564  d its transposed
+00011aa0: 2069 7320 7573 6564 3a0a 0a20 2020 2020   is used:..     
+00011ab0: 2020 2020 2e2e 206d 6174 683a 3a0a 2020      .. math::.  
+00011ac0: 2020 2020 2020 2020 2020 5620 3d20 4c20            V = L 
+00011ad0: 4c5e 542e 0a0a 2020 2020 2020 2020 2054  L^T...         T
+00011ae0: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00011af0: 636f 7374 2066 756e 6374 696f 6e0a 0a20  cost function.. 
+00011b00: 2020 2020 2020 2020 2e2e 206d 6174 683a          .. math:
+00011b10: 3a0a 2020 2020 2020 2020 2020 205c 6368  :.           \ch
+00011b20: 695e 3220 3d20 7b72 7d5c 6364 6f74 2028  i^2 = {r}\cdot (
+00011b30: 565e 7b2d 317d 7b72 7d29 207e 7e77 6974  V^{-1}{r}) ~~wit
+00011b40: 687e 7e20 7220 3d20 7920 2d20 6628 782c  h~~ r = y - f(x,
+00011b50: 2a70 290a 0a20 2020 2020 2020 2020 6973  *p)..         is
+00011b60: 2074 6865 6e20 6361 6c63 756c 6174 6564   then calculated
+00011b70: 2062 7920 736f 6c76 696e 6720 7468 6520   by solving the 
+00011b80: 6c69 6e65 6172 2065 7175 6174 696f 6e0a  linear equation.
+00011b90: 0a20 2020 2020 2020 202e 2e20 6d61 7468  .        .. math
+00011ba0: 3a3a 0a20 2020 2020 2020 2020 2020 5620  ::.           V 
+00011bb0: 5820 3d20 722c 207e 692e 652e 7e20 583d  X = r, ~i.e.~ X=
+00011bc0: 565e 7b2d 317d 2072 207e 616e 647e 205c  V^{-1} r ~and~ \
+00011bd0: 6368 695e 323d 2072 205c 6364 6f74 2058  chi^2= r \cdot X
+00011be0: 0a0a 2020 2020 2020 2020 7769 7468 2074  ..        with t
+00011bf0: 6865 206c 696e 6561 722d 6571 7561 7469  he linear-equati
+00011c00: 6f6e 2073 6f6c 7665 7220 2a73 6369 7079  on solver *scipy
+00011c10: 2e6c 696e 616c 672e 6368 6f5f 736f 6c76  .linalg.cho_solv
+00011c20: 6528 4c2c 7829 2a0a 2020 2020 2020 2020  e(L,x)*.        
+00011c30: 666f 7220 4368 6f6c 6573 6b79 2d64 6563  for Cholesky-dec
+00011c40: 6f6d 706f 7365 6420 6d61 7472 6963 6573  omposed matrices
+00011c50: 2c20 7468 7573 2061 766f 6964 696e 6720  , thus avoiding 
+00011c60: 7468 6520 636f 7374 790a 2020 2020 2020  the costy.      
+00011c70: 2020 6361 6c63 756c 6174 696f 6e20 6f66    calculation of
+00011c80: 2074 6865 2069 6e76 6572 7365 206d 6174   the inverse mat
+00011c90: 7269 782e 0a0a 0a20 2020 2020 2020 2054  rix....        T
+00011ca0: 6865 2064 6574 6572 6d69 6e61 6e74 2c20  he determinant, 
+00011cb0: 6966 206e 6565 6465 642c 2069 7320 6566  if needed, is ef
+00011cc0: 6669 6369 656e 746c 7920 6361 6c63 756c  ficiently calcul
+00011cd0: 6174 6564 2062 7920 7461 6b69 6e67 0a20  ated by taking. 
+00011ce0: 2020 2020 2020 2074 6865 2070 726f 6475         the produ
+00011cf0: 6374 206f 6620 7468 6520 6469 6167 6f6e  ct of the diagon
+00011d00: 616c 2065 6c65 6d65 6e74 7320 6f66 2074  al elements of t
+00011d10: 6865 206d 6174 7269 7820 4c2c 0a0a 2020  he matrix L,..  
+00011d20: 2020 2020 2020 202e 2e20 6d61 7468 3a3a         .. math::
+00011d30: 0a20 2020 2020 2020 2020 2020 5c64 6574  .           \det
+00011d40: 2856 2920 3d20 3220 5c2c 205c 7072 6f64  (V) = 2 \, \prod
+00011d50: 204c 5f7b 692c 697d 0a0a 2020 2020 2020   L_{i,i}..      
+00011d60: 2020 2049 6e70 7574 3a0a 0a20 2020 2020     Input:..     
+00011d70: 2020 2020 2d20 6f75 7465 723a 2070 6f69      - outer: poi
+00011d80: 6e74 6572 2074 6f20 696e 7374 616e 6365  nter to instance
+00011d90: 206f 6620 6361 6c6c 696e 6720 636c 6173   of calling clas
+00011da0: 730a 2020 2020 2020 2020 202d 206d 6f64  s.         - mod
+00011db0: 656c 3a20 6d6f 6465 6c20 6675 6e63 7469  el: model functi
+00011dc0: 6f6e 2066 2878 2c20 5c2a 7061 7229 0a20  on f(x, \*par). 
+00011dd0: 2020 2020 2020 2020 2d20 7573 655f 6e65          - use_ne
+00011de0: 6732 6c6f 674c 3a20 7573 6520 6675 6c6c  g2logL: use full
+00011df0: 202d 326c 6f67 284c 2920 696e 7374 6561   -2log(L) instea
+00011e00: 6420 6f66 2063 6869 3220 6966 2054 7275  d of chi2 if Tru
+00011e10: 650a 0a20 2020 2020 2020 2020 5f5f 6361  e..         __ca
+00011e20: 6c6c 5f5f 206d 6574 686f 6420 6f66 2074  ll__ method of t
+00011e30: 6869 7320 636c 6173 7320 6973 2063 616c  his class is cal
+00011e40: 6c65 6420 6279 2069 6d69 6e75 6974 0a0a  led by iminuit..
+00011e50: 2020 2020 2020 2020 2044 6174 6120 6d65           Data me
+00011e60: 6d62 6572 733a 0a0a 2020 2020 2020 2020  mbers:..        
+00011e70: 202d 206e 646f 663a 2064 6567 7265 6573   - ndof: degrees
+00011e80: 206f 6620 6672 6565 646f 6d0a 2020 2020   of freedom.    
+00011e90: 2020 2020 202d 206e 636f 6e73 7472 6169       - nconstrai
+00011ea0: 6e74 733a 206e 756d 6265 7220 6f66 2070  nts: number of p
+00011eb0: 6172 616d 6574 6572 2063 6f6e 7374 7261  arameter constra
+00011ec0: 696e 7473 0a20 2020 2020 2020 2020 2d20  ints.         - 
+00011ed0: 676f 663a 2063 6869 322d 7661 6c75 6520  gof: chi2-value 
+00011ee0: 2867 6f6f 646e 6573 7320 6f66 2066 6974  (goodness of fit
+00011ef0: 290a 2020 2020 2020 2020 202d 2075 7365  ).         - use
+00011f00: 5f6e 6567 326c 6f67 4c3a 2075 7361 6765  _neg2logL: usage
+00011f10: 206f 6620 6675 6c6c 2032 2a6e 6567 204c   of full 2*neg L
+00011f20: 6f67 204c 696b 656c 6968 6f6f 640a 2020  og Likelihood.  
+00011f30: 2020 2020 2020 202d 2071 7569 6574 3a20         - quiet: 
+00011f40: 6e6f 2070 7269 6e74 6f75 7420 6966 2054  no printout if T
+00011f50: 7275 650a 0a20 2020 2020 2020 2020 4d65  rue..         Me
+00011f60: 7468 6f64 733a 0a0a 2020 2020 2020 2020  thods:..        
+00011f70: 202d 206d 6f64 656c 2878 2c20 5c2a 7061   - model(x, \*pa
+00011f80: 7229 0a20 2020 2020 2020 2022 2222 0a0a  r).        """..
+00011f90: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
+00011fa0: 6974 5f5f 2873 656c 662c 206f 7574 6572  it__(self, outer
+00011fb0: 2c20 6d6f 6465 6c2c 2075 7365 5f6e 6567  , model, use_neg
+00011fc0: 326c 6f67 4c3d 4661 6c73 6529 3a0a 2020  2logL=False):.  
+00011fd0: 2020 2020 2020 2020 2020 2320 6461 7461            # data
+00011fe0: 206f 626a 6563 7420 6f66 2074 7970 6520   object of type 
+00011ff0: 7879 4461 7461 436f 6e74 6169 6e65 720a  xyDataContainer.
+00012000: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012010: 2e64 6174 6120 3d20 6f75 7465 722e 6461  .data = outer.da
+00012020: 7461 0a20 2020 2020 2020 2020 2020 2069  ta.            i
+00012030: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00012040: 2873 656c 662e 6461 7461 2c20 6d6e 4669  (self.data, mnFi
+00012050: 742e 7879 4461 7461 436f 6e74 6169 6e65  t.xyDataContaine
+00012060: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+00012070: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00012080: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00012090: 2020 2020 2020 2020 2020 2220 2121 2120            " !!! 
+000120a0: 6d6e 4669 742e 784c 5371 436f 7374 3a20  mnFit.xLSqCost: 
+000120b0: 6578 7065 6374 696e 6720 6461 7461 2063  expecting data c
+000120c0: 6f6e 7461 696e 6572 206f 6620 7479 7065  ontainer of type
+000120d0: 2027 6d6e 4669 742e 7879 4461 7461 436f   'mnFit.xyDataCo
+000120e0: 6e74 6169 6e65 7227 220a 2020 2020 2020  ntainer'".      
+000120f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00012100: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
+00012110: 656c 203d 206d 6f64 656c 0a20 2020 2020  el = model.     
+00012120: 2020 2020 2020 2073 656c 662e 7175 6965         self.quie
+00012130: 7420 3d20 6f75 7465 722e 7175 6965 740a  t = outer.quiet.
+00012140: 2020 2020 2020 2020 2020 2020 2320 7573              # us
+00012150: 6520 2d32 202a 206c 6f67 284c 2920 6f66  e -2 * log(L) of
+00012160: 2047 6175 7373 6961 6e20 696e 7374 6561   Gaussian instea
+00012170: 6420 6f66 2043 6869 320a 2020 2020 2020  d of Chi2.      
+00012180: 2020 2020 2020 2320 2028 6f6e 6c79 2064        #  (only d
+00012190: 6966 6665 7265 6e74 2066 726f 6d20 4368  ifferent from Ch
+000121a0: 6932 2066 6f72 2070 6172 616d 6574 6572  i2 for parameter
+000121b0: 2d64 6570 656e 6465 6e74 2075 6e63 6572  -dependent uncer
+000121c0: 7461 696e 7469 6573 290a 2020 2020 2020  tainties).      
+000121d0: 2020 2020 2020 7365 6c66 2e75 7365 5f6e        self.use_n
+000121e0: 6567 326c 6f67 4c20 3d20 7573 655f 6e65  eg2logL = use_ne
+000121f0: 6732 6c6f 674c 0a0a 2020 2020 2020 2020  g2logL..        
+00012200: 2020 2020 2320 7365 7420 7072 6f70 6572      # set proper
+00012210: 2073 6967 6e61 7475 7265 206f 6620 6d6f   signature of mo
+00012220: 6465 6c20 6675 6e63 7469 6f6e 2066 6f72  del function for
+00012230: 2069 6d69 6e75 6974 0a20 2020 2020 2020   iminuit.       
+00012240: 2020 2020 2073 656c 662e 706e 616d 7320       self.pnams 
+00012250: 3d20 6f75 7465 722e 706e 616d 730a 2020  = outer.pnams.  
+00012260: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+00012270: 7061 7220 3d20 6f75 7465 722e 6e70 6172  par = outer.npar
+00012280: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00012290: 7461 6b65 2061 6363 6f75 6e74 206f 6620  take account of 
+000122a0: 636f 6e73 7472 6169 6e74 730a 2020 2020  constraints.    
+000122b0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+000122c0: 7374 7261 696e 7473 203d 206f 7574 6572  straints = outer
+000122d0: 2e63 6f6e 7374 7261 696e 7473 0a20 2020  .constraints.   
+000122e0: 2020 2020 2020 2020 2073 656c 662e 6e63           self.nc
+000122f0: 6f6e 7374 7261 696e 7473 203d 206c 656e  onstraints = len
+00012300: 2873 656c 662e 636f 6e73 7472 6169 6e74  (self.constraint
+00012310: 7329 0a20 2020 2020 2020 2020 2020 2073  s).            s
+00012320: 656c 662e 6e64 6f66 203d 206c 656e 2873  elf.ndof = len(s
+00012330: 656c 662e 6461 7461 2e79 2920 2d20 7365  elf.data.y) - se
+00012340: 6c66 2e6e 7061 7220 2b20 7365 6c66 2e6e  lf.npar + self.n
+00012350: 636f 6e73 7472 6169 6e74 7320 2b20 6f75  constraints + ou
+00012360: 7465 722e 6e66 6978 6564 0a0a 2020 2020  ter.nfixed..    
+00012370: 2020 2020 2020 2020 2320 666c 6167 2074          # flag t
+00012380: 6f20 636f 6e74 726f 6c20 6669 6e61 6c20  o control final 
+00012390: 6163 7469 6f6e 7320 696e 2063 6f73 7420  actions in cost 
+000123a0: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
+000123b0: 2020 2020 2073 656c 662e 6669 6e61 6c5f       self.final_
+000123c0: 6361 6c6c 203d 2046 616c 7365 0a0a 2020  call = False..  
+000123d0: 2020 2020 2020 6465 6620 5f5f 6361 6c6c        def __call
+000123e0: 5f5f 2873 656c 662c 202a 7061 7229 3a0a  __(self, *par):.
+000123f0: 2020 2020 2020 2020 2020 2020 2320 6361              # ca
+00012400: 6c6c 6564 2069 7465 7261 7469 7665 6c79  lled iteratively
+00012410: 2062 7920 6d69 6e75 6974 0a0a 2020 2020   by minuit..    
+00012420: 2020 2020 2020 2020 2320 636f 7374 2066          # cost f
+00012430: 756e 6374 696f 6e20 6973 2065 7874 656e  unction is exten
+00012440: 6465 6420 6368 6932 3a0a 2020 2020 2020  ded chi2:.      
+00012450: 2020 2020 2020 2320 2020 6164 6420 6e6f        #   add no
+00012460: 726d 616c 697a 6174 696f 6e20 7465 726d  rmalization term
+00012470: 2069 6620 756e 6365 7274 6169 6e74 6965   if uncertaintie
+00012480: 7320 6465 7065 6e64 206f 6e20 6d6f 6465  s depend on mode
+00012490: 6c0a 0a20 2020 2020 2020 2020 2020 206e  l..            n
+000124a0: 6c4c 3220 3d20 302e 3020 2023 2069 6e69  lL2 = 0.0  # ini
+000124b0: 7469 616c 697a 6520 2d32 2a6c 6e28 4c29  tialize -2*ln(L)
+000124c0: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+000124d0: 6669 7273 742c 2074 616b 6520 696e 746f  first, take into
+000124e0: 2061 6363 6f75 6e74 2070 6f73 7369 626c   account possibl
+000124f0: 6520 7061 7261 6d65 7465 7220 636f 6e73  e parameter cons
+00012500: 7472 6169 6e74 730a 2020 2020 2020 2020  traints.        
+00012510: 2020 2020 6966 2073 656c 662e 6e63 6f6e      if self.ncon
+00012520: 7374 7261 696e 7473 3a0a 2020 2020 2020  straints:.      
+00012530: 2020 2020 2020 2020 2020 666f 7220 6320            for c 
+00012540: 696e 2073 656c 662e 636f 6e73 7472 6169  in self.constrai
+00012550: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+00012560: 2020 2020 2020 2020 2070 5f69 6420 3d20           p_id = 
+00012570: 635b 305d 0a20 2020 2020 2020 2020 2020  c[0].           
+00012580: 2020 2020 2020 2020 2072 203d 2028 7061           r = (pa
+00012590: 725b 705f 6964 5d20 2d20 635b 315d 2920  r[p_id] - c[1]) 
+000125a0: 2f20 635b 325d 0a20 2020 2020 2020 2020  / c[2].         
+000125b0: 2020 2020 2020 2020 2020 206e 6c4c 3220             nlL2 
+000125c0: 2b3d 2072 202a 2072 0a0a 2020 2020 2020  += r * r..      
+000125d0: 2020 2020 2020 2320 6361 6c63 756c 6174        # calculat
+000125e0: 6520 7265 7369 6475 616c 206f 6620 6461  e residual of da
+000125f0: 7461 2077 7274 2e20 6d6f 6465 6c0a 2020  ta wrt. model.  
+00012600: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+00012610: 7661 6c75 6573 203d 2073 656c 662e 6d6f  values = self.mo
+00012620: 6465 6c28 7365 6c66 2e64 6174 612e 782c  del(self.data.x,
+00012630: 202a 7061 7229 0a20 2020 2020 2020 2020   *par).         
+00012640: 2020 205f 7220 3d20 7365 6c66 2e64 6174     _r = self.dat
+00012650: 612e 7920 2d20 6d6f 6465 6c5f 7661 6c75  a.y - model_valu
+00012660: 6573 0a0a 2020 2020 2020 2020 2020 2020  es..            
+00012670: 6966 2073 656c 662e 6461 7461 2e6e 6565  if self.data.nee
+00012680: 6473 5f63 6f76 6172 6961 6e63 653a 0a20  ds_covariance:. 
+00012690: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000126a0: 2020 6368 6563 6b20 6966 206d 6174 7269    check if matri
+000126b0: 7820 6e65 6564 7320 7265 6275 696c 6469  x needs rebuildi
+000126c0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+000126d0: 2020 2069 6620 6e6f 7420 7365 6c66 2e64     if not self.d
+000126e0: 6174 612e 6e65 6564 735f 6479 6e61 6d69  ata.needs_dynami
+000126f0: 6345 7272 6f72 733a 0a20 2020 2020 2020  cErrors:.       
+00012700: 2020 2020 2020 2020 2020 2020 2023 2073               # s
+00012710: 7461 7469 6320 636f 7661 7269 616e 6365  tatic covariance
+00012720: 2c20 7573 6520 6974 7320 696e 7665 7273  , use its invers
+00012730: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00012740: 2020 2020 2020 6e6c 4c32 202b 3d20 666c        nlL2 += fl
+00012750: 6f61 7428 6e70 2e69 6e6e 6572 286e 702e  oat(np.inner(np.
+00012760: 6d61 746d 756c 285f 722c 2073 656c 662e  matmul(_r, self.
+00012770: 6461 7461 2e69 436f 7629 2c20 5f72 2929  data.iCov), _r))
+00012780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012790: 2020 2020 2023 2069 6465 6e74 6963 616c       # identical
+000127a0: 2074 6f20 636c 6173 7369 6361 6c20 4368   to classical Ch
+000127b0: 6932 0a20 2020 2020 2020 2020 2020 2020  i2.             
+000127c0: 2020 2020 2020 2073 656c 662e 676f 6620         self.gof 
+000127d0: 3d20 6e6c 4c32 0a0a 2020 2020 2020 2020  = nlL2..        
+000127e0: 2020 2020 2020 2020 656c 7365 3a20 2023          else:  #
+000127f0: 2064 796e 616d 6963 616c 6c79 2072 6562   dynamically reb
+00012800: 7569 6c64 2063 6f76 6172 6961 6e63 6520  uild covariance 
+00012810: 6d61 7472 6978 0a20 2020 2020 2020 2020  matrix.         
+00012820: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012830: 6461 7461 2e5f 7265 6275 696c 645f 436f  data._rebuild_Co
+00012840: 7628 7061 7229 0a20 2020 2020 2020 2020  v(par).         
+00012850: 2020 2020 2020 2020 2020 2023 2075 7365             # use
+00012860: 2043 686f 6c65 736b 7920 6465 636f 6d70   Cholesky decomp
+00012870: 6f73 6974 6f6e 2074 6f20 636f 6d70 7574  ositon to comput
+00012880: 6520 6368 6932 203d 205f 722e 5420 2856  e chi2 = _r.T (V
+00012890: 5e2d 3129 205f 720a 2020 2020 2020 2020  ^-1) _r.        
+000128a0: 2020 2020 2020 2020 2020 2020 4c2c 2069              L, i
+000128b0: 735f 6c6f 7765 7220 3d20 6c69 6e61 6c67  s_lower = linalg
+000128c0: 2e63 686f 5f66 6163 746f 7228 7365 6c66  .cho_factor(self
+000128d0: 2e64 6174 612e 636f 762c 2063 6865 636b  .data.cov, check
+000128e0: 5f66 696e 6974 653d 4661 6c73 6529 0a20  _finite=False). 
+000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012900: 2020 206e 6c4c 3220 2b3d 206e 702e 696e     nlL2 += np.in
+00012910: 6e65 7228 5f72 2c20 6c69 6e61 6c67 2e63  ner(_r, linalg.c
+00012920: 686f 5f73 6f6c 7665 2828 4c2c 2069 735f  ho_solve((L, is_
+00012930: 6c6f 7765 7229 2c20 5f72 2929 0a20 2020  lower), _r)).   
+00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012950: 2023 2075 7020 746f 2068 6572 652c 2069   # up to here, i
+00012960: 6465 6e74 6963 616c 2074 6f20 636c 6173  dentical to clas
+00012970: 7369 6361 6c20 4368 6932 0a20 2020 2020  sical Chi2.     
+00012980: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012990: 656c 662e 676f 6620 3d20 6e6c 4c32 0a20  elf.gof = nlL2. 
+000129a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000129b0: 2020 2023 2074 616b 6520 696e 746f 2061     # take into a
+000129c0: 6363 6f75 6e74 2070 6172 616d 6574 6572  ccount parameter
+000129d0: 2d64 6570 656e 6465 6e74 206e 6f72 6d61  -dependent norma
+000129e0: 6c69 7361 7469 6f6e 2074 6572 6d0a 2020  lisation term.  
+000129f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a00: 2020 6966 2073 656c 662e 7573 655f 6e65    if self.use_ne
+00012a10: 6732 6c6f 674c 3a0a 2020 2020 2020 2020  g2logL:.        
+00012a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a30: 2320 2066 6173 7420 6361 6c63 756c 6174  #  fast calculat
+00012a40: 696f 6e20 6f66 2064 6574 6572 6d69 6e61  ion of determina
+00012a50: 6e74 2064 6574 2856 2920 6672 6f6d 2043  nt det(V) from C
+00012a60: 686f 6c65 736b 7920 6661 6374 6f72 0a20  holesky factor. 
 00012a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a80: 6e6c 4c32 202b 3d20 322e 3020 2a20 6e70  nlL2 += 2.0 * np
-00012a90: 2e73 756d 286e 702e 6c6f 6728 6e70 2e64  .sum(np.log(np.d
-00012aa0: 6961 676f 6e61 6c28 4c29 2929 0a0a 2020  iagonal(L)))..  
-00012ab0: 2020 2020 2020 2020 2020 656c 7365 3a20            else: 
-00012ac0: 2023 2066 6173 7420 6361 6c63 756c 6174   # fast calculat
-00012ad0: 696f 6e20 666f 7220 7369 6d70 6c65 2065  ion for simple e
-00012ae0: 7272 6f72 730a 2020 2020 2020 2020 2020  rrors.          
-00012af0: 2020 2020 2020 2320 6368 6563 6b20 6966        # check if
-00012b00: 2065 7272 6f72 7320 6e65 6564 7320 7265   errors needs re
-00012b10: 6361 6c63 756c 6174 696e 670a 2020 2020  calculating.    
-00012b20: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00012b30: 656c 662e 6461 7461 2e6e 6565 6473 5f64  elf.data.needs_d
-00012b40: 796e 616d 6963 4572 726f 7273 3a0a 2020  ynamicErrors:.  
-00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b60: 2020 7365 6c66 2e64 6174 612e 5f72 6562    self.data._reb
-00012b70: 7569 6c64 5f45 7272 3228 7061 7229 0a20  uild_Err2(par). 
-00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b90: 2020 206e 6c4c 3220 2b3d 206e 702e 7375     nlL2 += np.su
-00012ba0: 6d28 5f72 202a 205f 7220 2f20 7365 6c66  m(_r * _r / self
-00012bb0: 2e64 6174 612e 6572 7232 290a 2020 2020  .data.err2).    
-00012bc0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00012bd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012be0: 2020 2020 2020 6e6c 4c32 202b 3d20 6e70        nlL2 += np
-00012bf0: 2e73 756d 285f 7220 2a20 5f72 202a 2073  .sum(_r * _r * s
-00012c00: 656c 662e 6461 7461 2e69 4572 7232 290a  elf.data.iErr2).
-00012c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012c20: 2023 2074 6869 7320 6973 2069 6465 6e74   # this is ident
-00012c30: 6963 616c 2074 6f20 636c 6173 7369 6361  ical to classica
-00012c40: 6c20 4368 6932 0a20 2020 2020 2020 2020  l Chi2.         
-00012c50: 2020 2020 2020 2073 656c 662e 676f 6620         self.gof 
-00012c60: 3d20 6e6c 4c32 0a0a 2020 2020 2020 2020  = nlL2..        
-00012c70: 2020 2020 2020 2020 2320 6164 6420 7061          # add pa
-00012c80: 7261 6d65 7465 722d 6465 7065 6e64 656e  rameter-dependen
-00012c90: 7420 6e6f 726d 616c 697a 6174 696f 6e20  t normalization 
-00012ca0: 7465 726d 2069 6620 6e65 6564 6564 2061  term if needed a
-00012cb0: 6e64 2077 616e 7465 640a 2020 2020 2020  nd wanted.      
-00012cc0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00012cd0: 662e 6461 7461 2e6e 6565 6473 5f64 796e  f.data.needs_dyn
-00012ce0: 616d 6963 4572 726f 7273 2061 6e64 2073  amicErrors and s
-00012cf0: 656c 662e 7573 655f 6e65 6732 6c6f 674c  elf.use_neg2logL
-00012d00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012d10: 2020 2020 2020 6e6c 4c32 202b 3d20 6e70        nlL2 += np
-00012d20: 2e73 756d 286e 702e 6c6f 6728 7365 6c66  .sum(np.log(self
-00012d30: 2e64 6174 612e 6572 7232 2929 0a0a 2020  .data.err2))..  
-00012d40: 2020 2020 2020 2020 2020 2320 7072 6f76            # prov
-00012d50: 6964 6520 6d6f 6465 6c20 7661 6c75 6573  ide model values
-00012d60: 2074 6f20 6461 7461 206f 626a 6563 740a   to data object.
-00012d70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012d80: 2e64 6174 612e 6d6f 6465 6c5f 7661 6c75  .data.model_valu
-00012d90: 6573 203d 206d 6f64 656c 5f76 616c 7565  es = model_value
-00012da0: 730a 0a20 2020 2020 2020 2020 2020 2072  s..            r
-00012db0: 6574 7572 6e20 6e6c 4c32 0a0a 2020 2020  eturn nlL2..    
-00012dc0: 2320 2d2d 2d20 656e 6420 6465 6669 6e69  # --- end defini
-00012dd0: 7469 6f6e 206f 6620 636c 6173 7320 784c  tion of class xL
-00012de0: 5371 436f 7374 202d 2d2d 2d0a 0a20 2020  SqCost ----..   
-00012df0: 2023 0a20 2020 2023 202d 2d2d 2073 7065   #.    # --- spe
-00012e00: 6369 616c 2063 6f64 6520 666f 7220 696e  cial code for in
-00012e10: 6465 7865 6420 4669 7420 2878 4669 7429  dexed Fit (xFit)
-00012e20: 0a20 2020 2023 0a0a 2020 2020 6465 6620  .    #..    def 
-00012e30: 7365 745f 784f 7074 696f 6e73 280a 2020  set_xOptions(.  
-00012e40: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00012e50: 2020 2020 7265 6c61 7469 7665 5f72 6566      relative_ref
-00012e60: 6572 735f 746f 5f6d 6f64 656c 3d4e 6f6e  ers_to_model=Non
-00012e70: 652c 0a20 2020 2020 2020 2072 756e 5f6d  e,.        run_m
-00012e80: 696e 6f73 3d4e 6f6e 652c 0a20 2020 2020  inos=None,.     
-00012e90: 2020 2075 7365 5f6e 6567 4c6f 674c 3d4e     use_negLogL=N
-00012ea0: 6f6e 652c 0a20 2020 2020 2020 2071 7569  one,.        qui
-00012eb0: 6574 3d4e 6f6e 652c 0a20 2020 2029 3a0a  et=None,.    ):.
-00012ec0: 2020 2020 2020 2020 2222 2244 6566 696e          """Defin
-00012ed0: 6520 6f70 7469 6f6e 7320 666f 7220 696e  e options for in
-00012ee0: 6465 7865 6420 6669 740a 0a20 2020 2020  dexed fit..     
-00012ef0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00012f00: 2020 2d20 7265 6c2e 2065 7272 6f72 7320    - rel. errors 
-00012f10: 7265 6665 7220 746f 206d 6f64 656c 2065  refer to model e
-00012f20: 6c73 6520 6461 7461 0a20 2020 2020 2020  lse data.       
-00012f30: 2020 2d20 7275 6e20 6d69 6e6f 7320 656c    - run minos el
-00012f40: 7365 2064 6f6e 2a74 2072 756e 206d 696e  se don*t run min
-00012f50: 6f73 0a20 2020 2020 2020 2020 2d20 7573  os.         - us
-00012f60: 6520 6675 6c6c 206e 6567 326c 6f67 4c0a  e full neg2logL.
-00012f70: 2020 2020 2020 2020 202d 2064 6f6e 2a74           - don*t
-00012f80: 2070 726f 7669 6465 2070 7269 6e74 6f75   provide printou
-00012f90: 7420 656c 7365 2076 6572 626f 7365 2070  t else verbose p
-00012fa0: 7269 6e74 6f75 740a 2020 2020 2020 2020  rintout.        
-00012fb0: 2222 220a 2020 2020 2020 2020 6966 2072  """.        if r
-00012fc0: 656c 6174 6976 655f 7265 6665 7273 5f74  elative_refers_t
-00012fd0: 6f5f 6d6f 6465 6c20 6973 206e 6f74 204e  o_model is not N
-00012fe0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00012ff0: 2073 656c 662e 7265 664d 6f64 656c 203d   self.refModel =
-00013000: 2072 656c 6174 6976 655f 7265 6665 7273   relative_refers
-00013010: 5f74 6f5f 6d6f 6465 6c0a 2020 2020 2020  _to_model.      
-00013020: 2020 2020 2020 7365 6c66 2e6f 7074 696f        self.optio
-00013030: 6e73 5b22 7265 664d 6f64 656c 225d 5b30  ns["refModel"][0
-00013040: 5d20 3d20 696e 7428 7265 6c61 7469 7665  ] = int(relative
-00013050: 5f72 6566 6572 735f 746f 5f6d 6f64 656c  _refers_to_model
-00013060: 290a 2020 2020 2020 2020 6966 2072 756e  ).        if run
-00013070: 5f6d 696e 6f73 2069 7320 6e6f 7420 4e6f  _minos is not No
-00013080: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00013090: 7365 6c66 2e72 756e 5f6d 696e 6f73 203d  self.run_minos =
-000130a0: 2072 756e 5f6d 696e 6f73 0a20 2020 2020   run_minos.     
-000130b0: 2020 2020 2020 2073 656c 662e 6f70 7469         self.opti
-000130c0: 6f6e 735b 2272 756e 5f6d 696e 6f73 225d  ons["run_minos"]
-000130d0: 5b30 5d20 3d20 696e 7428 7275 6e5f 6d69  [0] = int(run_mi
-000130e0: 6e6f 7329 0a20 2020 2020 2020 2069 6620  nos).        if 
-000130f0: 7573 655f 6e65 674c 6f67 4c20 6973 206e  use_negLogL is n
-00013100: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00013110: 2020 2020 2073 656c 662e 7573 655f 6e65       self.use_ne
-00013120: 674c 6f67 4c20 3d20 7573 655f 6e65 674c  gLogL = use_negL
-00013130: 6f67 4c0a 2020 2020 2020 2020 2020 2020  ogL.            
-00013140: 7365 6c66 2e6f 7074 696f 6e73 5b22 7573  self.options["us
-00013150: 655f 6e65 674c 6f67 4c22 5d5b 305d 203d  e_negLogL"][0] =
-00013160: 2069 6e74 2875 7365 5f6e 6567 4c6f 674c   int(use_negLogL
-00013170: 290a 2020 2020 2020 2020 6966 2071 7569  ).        if qui
-00013180: 6574 2069 7320 6e6f 7420 4e6f 6e65 3a0a  et is not None:.
-00013190: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000131a0: 2e71 7569 6574 203d 2071 7569 6574 0a0a  .quiet = quiet..
-000131b0: 2020 2020 6465 6620 696e 6974 5f78 4461      def init_xDa
-000131c0: 7461 2873 656c 662c 2078 2c20 653d 4e6f  ta(self, x, e=No
-000131d0: 6e65 2c20 6572 656c 3d4e 6f6e 652c 2063  ne, erel=None, c
-000131e0: 6162 733d 4e6f 6e65 2c20 6372 656c 3d4e  abs=None, crel=N
-000131f0: 6f6e 652c 206e 616d 6573 3d4e 6f6e 6529  one, names=None)
-00013200: 3a0a 2020 2020 2020 2020 2222 2269 6e69  :.        """ini
-00013210: 7469 616c 697a 6520 6461 7461 206f 626a  tialize data obj
-00013220: 6563 740a 0a20 2020 2020 2020 2041 7267  ect..        Arg
-00013230: 733a 0a20 2020 2020 2020 2020 202d 2020  s:.          -  
-00013240: 783a 2020 2020 2020 6461 7461 2076 616c  x:      data val
-00013250: 7565 730a 2020 2020 2020 2020 2020 2d20  ues.          - 
-00013260: 2073 3a20 2020 2020 2069 6e64 6570 656e   s:      indepen
-00013270: 6465 6e74 2075 6e63 6572 7461 696e 7469  dent uncertainti
-00013280: 6573 2078 0a20 2020 2020 2020 2020 202d  es x.          -
-00013290: 2020 7372 656c 3a20 2020 696e 6465 7065    srel:   indepe
-000132a0: 6e64 656e 7420 7265 6c61 7469 7665 2075  ndent relative u
-000132b0: 6e63 6572 7461 696e 7469 6573 2078 0a20  ncertainties x. 
-000132c0: 2020 2020 2020 2020 202d 2020 6361 6273           -  cabs
-000132d0: 3a20 2020 636f 7272 656c 6174 6564 2061  :   correlated a
-000132e0: 626f 6c75 7465 2075 6e63 6572 7461 696e  bolute uncertain
-000132f0: 7469 6573 2078 0a20 2020 2020 2020 2020  ties x.         
-00013300: 202d 2020 6372 656c 3a20 2020 636f 7272   -  crel:   corr
-00013310: 656c 6174 6564 2072 656c 6174 6976 6520  elated relative 
-00013320: 756e 6365 7274 6169 6e74 6965 7320 780a  uncertainties x.
-00013330: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00013340: 2020 2020 2023 2063 7265 6174 6520 6461       # create da
-00013350: 7461 206f 626a 6563 7420 616e 6420 7061  ta object and pa
-00013360: 7373 2061 6c6c 2069 6e70 7574 2061 7267  ss all input arg
-00013370: 756d 656e 7473 0a20 2020 2020 2020 2073  uments.        s
-00013380: 656c 662e 7844 6174 6120 3d20 7365 6c66  elf.xData = self
-00013390: 2e78 4461 7461 436f 6e74 6169 6e65 7228  .xDataContainer(
-000133a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000133b0: 662c 2078 2c20 652c 2065 7265 6c2c 2063  f, x, e, erel, c
-000133c0: 6162 732c 2063 7265 6c2c 206e 616d 6573  abs, crel, names
-000133d0: 3d6e 616d 6573 2c20 7175 6965 743d 7365  =names, quiet=se
-000133e0: 6c66 2e71 7569 6574 0a20 2020 2020 2020  lf.quiet.       
-000133f0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00013400: 6461 7461 203d 2073 656c 662e 7844 6174  data = self.xDat
-00013410: 610a 2020 2020 2020 2020 2320 7365 7420  a.        # set 
-00013420: 666c 6167 7320 666f 7220 7374 6565 7269  flags for steeri
-00013430: 6e67 206f 6620 6669 7420 7072 6f63 6573  ng of fit proces
-00013440: 7320 696e 2064 6f5f 6669 7428 290a 2020  s in do_fit().  
-00013450: 2020 2020 2020 7365 6c66 2e69 7465 7261        self.itera
-00013460: 7465 4669 7420 3d20 7365 6c66 2e78 4461  teFit = self.xDa
-00013470: 7461 2e68 6173 5f72 656c 5f45 7272 6f72  ta.has_rel_Error
-00013480: 7320 616e 6420 7365 6c66 2e72 6566 4d6f  s and self.refMo
-00013490: 6465 6c0a 0a20 2020 2064 6566 2069 6e69  del..    def ini
-000134a0: 745f 7846 6974 280a 2020 2020 2020 2020  t_xFit(.        
-000134b0: 7365 6c66 2c0a 2020 2020 2020 2020 6d6f  self,.        mo
-000134c0: 6465 6c2c 0a20 2020 2020 2020 206d 6f64  del,.        mod
-000134d0: 656c 5f6b 7761 7267 733d 4e6f 6e65 2c0a  el_kwargs=None,.
-000134e0: 2020 2020 2020 2020 7030 3d4e 6f6e 652c          p0=None,
-000134f0: 0a20 2020 2020 2020 2064 7030 3d4e 6f6e  .        dp0=Non
-00013500: 652c 0a20 2020 2020 2020 2063 6f6e 7374  e,.        const
-00013510: 7261 696e 7473 3d4e 6f6e 652c 0a20 2020  raints=None,.   
-00013520: 2020 2020 2066 6978 5061 7273 3d4e 6f6e       fixPars=Non
-00013530: 652c 0a20 2020 2020 2020 206c 696d 6974  e,.        limit
-00013540: 733d 4e6f 6e65 2c0a 2020 2020 293a 0a20  s=None,.    ):. 
-00013550: 2020 2020 2020 2022 2222 696e 6974 6961         """initia
-00013560: 6c69 7a65 2066 6974 206f 626a 6563 740a  lize fit object.
-00013570: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00013580: 2020 2020 2020 2020 202d 206d 6f64 656c           - model
-00013590: 3a20 6d6f 6465 6c20 6675 6e63 7469 6f6e  : model function
-000135a0: 2066 2878 3b20 5c2a 7061 7229 0a20 2020   f(x; \*par).   
-000135b0: 2020 2020 2020 202d 206d 6f64 656c 5f6b         - model_k
-000135c0: 7761 7267 733a 206f 7074 696f 6e61 6c2c  wargs: optional,
-000135d0: 2066 6974 2070 6172 616d 6574 6572 7320   fit parameters 
-000135e0: 6966 206e 6f74 2066 726f 6d20 6d6f 6465  if not from mode
-000135f0: 6c20 7369 676e 6174 7572 650a 2020 2020  l signature.    
-00013600: 2020 2020 2020 2d20 7030 3a20 6e70 2d61        - p0: np-a
-00013610: 7272 6179 206f 6620 666c 6f61 7473 2c20  rray of floats, 
-00013620: 696e 6974 6961 6c20 7061 7261 6d65 7465  initial paramete
-00013630: 7220 7661 6c75 6573 0a20 2020 2020 2020  r values.       
-00013640: 2020 202d 2064 7030 3a20 6172 7261 792d     - dp0: array-
-00013650: 6c69 6b65 2c20 696e 6974 6961 6c20 6775  like, initial gu
-00013660: 6573 7320 6f66 2070 6172 616d 6574 6572  ess of parameter
-00013670: 2075 6e63 6572 7461 696e 7469 6573 2028   uncertainties (
-00013680: 6f70 7469 6f6e 616c 290a 2020 2020 2020  optional).      
-00013690: 2020 2020 2d20 636f 6e73 7472 6169 6e74      - constraint
-000136a0: 733a 2028 6e65 7374 6564 2920 6c69 7374  s: (nested) list
-000136b0: 2873 293a 205b 7061 7261 6d65 7465 7220  (s): [parameter 
-000136c0: 6e61 6d65 2c20 7661 6c75 652c 2075 6e63  name, value, unc
-000136d0: 6572 7461 696e 7479 5d0a 2020 2020 2020  ertainty].      
-000136e0: 2020 2020 2020 6f72 205b 7061 7261 6d65        or [parame
-000136f0: 7465 7220 696e 6465 782c 2076 616c 7565  ter index, value
-00013700: 2c20 756e 6365 7274 6169 6e74 795d 0a20  , uncertainty]. 
-00013710: 2020 2020 2020 2020 202d 206c 696d 6974           - limit
-00013720: 733a 2028 6e65 7374 6564 2920 6c69 7374  s: (nested) list
-00013730: 2873 293a 205b 7061 7261 6d65 7465 7220  (s): [parameter 
-00013740: 6e61 6d65 2c20 6d69 6e2c 206d 6178 5d0a  name, min, max].
-00013750: 2020 2020 2020 2020 2020 2020 6f72 205b              or [
-00013760: 7061 7261 6d65 7465 7220 696e 6465 782c  parameter index,
-00013770: 206d 696e 2c20 6d61 785d 0a20 2020 2020   min, max].     
-00013780: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00013790: 6966 2073 656c 662e 7844 6174 6120 6973  if self.xData is
-000137a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000137b0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-000137c0: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-000137d0: 2020 2020 2022 2021 2121 206d 6e46 6974       " !!! mnFit
-000137e0: 2e69 6e69 745f 7846 6974 3a20 6e6f 2064  .init_xFit: no d
-000137f0: 6174 6120 6f62 6a65 6374 2064 6566 696e  ata object defin
-00013800: 6564 202d 2063 616c 6c20 696e 6974 5f64  ed - call init_d
-00013810: 6174 6128 2922 0a20 2020 2020 2020 2020  ata()".         
-00013820: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-00013830: 6765 7420 7061 7261 6d65 7465 7273 206f  get parameters o
-00013840: 6620 6d6f 6465 6c20 6675 6e63 7469 6f6e  f model function
-00013850: 2074 6f20 7365 7420 7374 6172 7420 7661   to set start va
-00013860: 6c75 6573 2066 6f72 2066 6974 0a20 2020  lues for fit.   
-00013870: 2020 2020 2069 6620 6d6f 6465 6c5f 6b77       if model_kw
-00013880: 6172 6773 2069 7320 4e6f 6e65 3a0a 2020  args is None:.  
-00013890: 2020 2020 2020 2020 2020 6172 6773 2c20            args, 
-000138a0: 6d6f 6465 6c5f 6b77 6172 6773 203d 2067  model_kwargs = g
-000138b0: 6574 5f66 756e 6374 696f 6e53 6967 6e61  et_functionSigna
-000138c0: 7475 7265 286d 6f64 656c 290a 0a20 2020  ture(model)..   
-000138d0: 2020 2020 2070 6172 203d 2028 6d6f 6465       par = (mode
-000138e0: 6c5f 6b77 6172 6773 2c20 7030 2c20 6470  l_kwargs, p0, dp
-000138f0: 302c 2063 6f6e 7374 7261 696e 7473 2c20  0, constraints, 
-00013900: 6669 7850 6172 732c 206c 696d 6974 7329  fixPars, limits)
-00013910: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-00013920: 6574 7570 4669 7450 6172 616d 6574 6572  etupFitParameter
-00013930: 7328 2a70 6172 290a 0a20 2020 2020 2020  s(*par)..       
-00013940: 2023 2063 7265 6174 6520 636f 7374 2066   # create cost f
-00013950: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
-00013960: 7365 6c66 2e63 6f73 7466 203d 2073 656c  self.costf = sel
-00013970: 662e 696e 6465 7865 6443 6f73 7428 7365  f.indexedCost(se
-00013980: 6c66 2c20 6d6f 6465 6c2c 2075 7365 5f6e  lf, model, use_n
-00013990: 6567 326c 6f67 4c3d 7365 6c66 2e75 7365  eg2logL=self.use
-000139a0: 5f6e 6567 4c6f 674c 290a 2020 2020 2020  _negLogL).      
-000139b0: 2020 7365 6c66 2e5f 7365 7475 704d 696e    self._setupMin
-000139c0: 7569 7428 6d6f 6465 6c5f 6b77 6172 6773  uit(model_kwargs
-000139d0: 290a 0a20 2020 2063 6c61 7373 2078 4461  )..    class xDa
-000139e0: 7461 436f 6e74 6169 6e65 723a 0a20 2020  taContainer:.   
-000139f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013a00: 2048 616e 646c 6520 6461 7461 2061 6e64   Handle data and
-00013a10: 2075 6e63 6572 7461 696e 7469 6573 2061   uncertainties a
-00013a20: 6e64 0a20 2020 2020 2020 2062 7569 6c64  nd.        build
-00013a30: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-00013a40: 6963 6573 2066 726f 6d20 636f 6d70 6f6e  ices from compon
-00013a50: 656e 7473 0a0a 2020 2020 2020 2020 4172  ents..        Ar
-00013a60: 6773 3a0a 2020 2020 2020 2020 2020 2d20  gs:.          - 
-00013a70: 6f75 7465 723a 2020 2070 6f69 6e74 6572  outer:   pointer
-00013a80: 2074 6f20 696e 7374 616e 6365 206f 6620   to instance of 
-00013a90: 6361 6c6c 696e 6720 6f62 6a65 6374 0a20  calling object. 
-00013aa0: 2020 2020 2020 2020 202d 2078 3a20 2020           - x:   
-00013ab0: 2020 2020 6162 7363 6973 7361 206f 6620      abscissa of 
-00013ac0: 6461 7461 2070 6f69 6e74 7320 2822 7820  data points ("x 
-00013ad0: 7661 6c75 6573 2229 0a20 2020 2020 2020  values").       
-00013ae0: 2020 202d 2065 3a20 2020 2020 2020 696e     - e:       in
-00013af0: 6465 7065 6e64 656e 7420 756e 6365 7274  dependent uncert
-00013b00: 6169 6e74 6965 730a 2020 2020 2020 2020  ainties.        
-00013b10: 2020 2d20 6572 656c 3a20 2020 696e 6465    - erel:   inde
-00013b20: 7065 6e64 656e 7420 7265 6c61 7469 7665  pendent relative
-00013b30: 2075 6e63 6572 7461 696e 7469 6573 2078   uncertainties x
-00013b40: 0a20 2020 2020 2020 2020 202d 2063 6162  .          - cab
-00013b50: 733a 2020 2063 6f72 7265 6c61 7465 6420  s:   correlated 
-00013b60: 6162 6f6c 7574 6520 756e 6365 7274 6169  abolute uncertai
-00013b70: 6e74 6965 7320 780a 2020 2020 2020 2020  nties x.        
-00013b80: 2020 2d20 6372 656c 3a20 2020 636f 7272    - crel:   corr
-00013b90: 656c 6174 6564 2072 656c 6174 6976 6520  elated relative 
-00013ba0: 756e 6365 7274 6169 6e74 6965 7320 780a  uncertainties x.
-00013bb0: 2020 2020 2020 2020 2020 2d20 7175 6965            - quie
-00013bc0: 743a 2020 206e 6f20 696e 666f 726d 6174  t:   no informat
-00013bd0: 6976 6520 7072 696e 746f 7574 2069 6620  ive printout if 
-00013be0: 5472 7565 0a0a 2020 2020 2020 2020 5075  True..        Pu
-00013bf0: 626c 6963 206d 6574 686f 6473 3a0a 2020  blic methods:.  
-00013c00: 2020 2020 2020 2020 2d20 696e 6974 5f64          - init_d
-00013c10: 796e 616d 6963 4572 726f 7273 2829 3a0a  ynamicErrors():.
-00013c20: 2020 2020 2020 2020 2020 2d20 6765 745f            - get_
-00013c30: 436f 7628 293a 2066 696e 616c 2063 6f76  Cov(): final cov
-00013c40: 6172 6961 6e63 6520 6d61 7472 6978 2028  ariance matrix (
-00013c50: 696e 636c 2e20 7072 6f6a 2e20 7829 0a20  incl. proj. x). 
-00013c60: 2020 2020 2020 2020 202d 2067 6574 5f69           - get_i
-00013c70: 436f 7628 293a 2069 6e76 6572 7365 2063  Cov(): inverse c
-00013c80: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-00013c90: 0a20 2020 2020 2020 2020 202d 2070 6c6f  .          - plo
-00013ca0: 7428 293a 2070 726f 7669 6465 2061 2066  t(): provide a f
-00013cb0: 6967 7572 6520 7769 7468 2072 6570 7265  igure with repre
-00013cc0: 7365 6e74 6174 696f 6e20 6f66 2064 6174  sentation of dat
-00013cd0: 610a 0a20 2020 2020 2020 2044 6174 6120  a..        Data 
-00013ce0: 6d65 6d62 6572 733a 0a20 2020 2020 2020  members:.       
-00013cf0: 2020 202a 2063 6f70 7920 6f66 2061 6c6c     * copy of all
-00013d00: 2069 6e70 7574 2061 7267 756d 656e 7473   input arguments
-00013d10: 0a20 2020 2020 2020 2020 202a 2063 6f76  .          * cov
-00013d20: 3a20 636f 7661 7269 616e 6365 206d 6174  : covariance mat
-00013d30: 7269 780a 2020 2020 2020 2020 2020 2a20  rix.          * 
-00013d40: 6943 6f76 3a20 696e 7665 7273 6520 6f66  iCov: inverse of
-00013d50: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-00013d60: 6978 0a20 2020 2020 2020 2022 2222 0a0a  ix.        """..
-00013d70: 2020 2020 2020 2020 6465 6620 5f5f 696e          def __in
-00013d80: 6974 5f5f 2873 656c 662c 206f 7574 6572  it__(self, outer
-00013d90: 2c20 782c 2065 2c20 6572 656c 2c20 6361  , x, e, erel, ca
-00013da0: 6273 2c20 6372 656c 2c20 6e61 6d65 733d  bs, crel, names=
-00013db0: 4e6f 6e65 2c20 7175 6965 743d 5472 7565  None, quiet=True
-00013dc0: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-00013dd0: 2073 6176 6520 706f 696e 6572 2074 6f20   save poiner to 
-00013de0: 6361 6c6c 696e 6720 636c 6173 730a 2020  calling class.  
-00013df0: 2020 2020 2020 2020 2020 7365 6c66 2e6f            self.o
-00013e00: 7574 6572 203d 206f 7574 6572 0a0a 2020  uter = outer..  
-00013e10: 2020 2020 2020 2020 2020 2320 6173 7375            # assu
-00013e20: 6d65 2073 696d 706c 6520 6361 7365 2077  me simple case w
-00013e30: 2e6f 2e20 636f 762e 6d61 742e 0a20 2020  .o. cov.mat..   
-00013e40: 2020 2020 2020 2020 2073 656c 662e 6e65           self.ne
-00013e50: 6564 735f 636f 7661 7269 616e 6365 203d  eds_covariance =
-00013e60: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
-00013e70: 2020 2020 7365 6c66 2e78 4e61 6d65 7320      self.xNames 
-00013e80: 3d20 6e61 6d65 7320 2023 2073 6574 2070  = names  # set p
-00013e90: 6172 616d 6574 6572 206e 616d 6573 0a0a  arameter names..
-00013ea0: 2020 2020 2020 2020 2020 2020 6e64 203d              nd =
-00013eb0: 206c 656e 2878 290a 2020 2020 2020 2020   len(x).        
-00013ec0: 2020 2020 2320 7374 6f72 6520 696e 7075      # store inpu
-00013ed0: 7420 6461 7461 2061 7320 6e75 6d70 7920  t data as numpy 
-00013ee0: 666c 6f61 7420 6172 7261 7973 2c20 656e  float arrays, en
-00013ef0: 7375 7265 206c 656e 6774 6820 6e64 2069  sure length nd i
-00013f00: 6620 6e65 6564 6564 0a20 2020 2020 2020  f needed.       
-00013f10: 2020 2020 2073 656c 662e 7820 3d20 6e70       self.x = np
-00013f20: 2e61 7366 6172 7261 7928 7829 2020 2320  .asfarray(x)  # 
-00013f30: 6162 7363 6973 7361 202d 2022 7820 7661  abscissa - "x va
-00013f40: 6c75 6573 220a 2020 2020 2020 2020 2020  lues".          
-00013f50: 2020 7365 6c66 2e65 203d 206e 702e 6173    self.e = np.as
-00013f60: 6661 7272 6179 2865 2920 2023 2069 6e64  farray(e)  # ind
-00013f70: 6570 656e 6465 6e74 2075 6e63 6572 7461  ependent uncerta
-00013f80: 696e 7469 6573 2079 0a20 2020 2020 2020  inties y.       
-00013f90: 2020 2020 2069 6620 7365 6c66 2e65 2e6e       if self.e.n
-00013fa0: 6469 6d20 3d3d 2030 3a0a 2020 2020 2020  dim == 0:.      
-00013fb0: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
-00013fc0: 203d 2073 656c 662e 6520 2a20 6e70 2e6f   = self.e * np.o
-00013fd0: 6e65 7328 6e64 290a 2020 2020 2020 2020  nes(nd).        
-00013fe0: 2020 2020 656c 6966 2073 656c 662e 652e      elif self.e.
-00013ff0: 6e64 696d 203d 3d20 323a 0a20 2020 2020  ndim == 2:.     
-00014000: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014010: 6e65 6564 735f 636f 7661 7269 616e 6365  needs_covariance
-00014020: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-00014030: 2020 2020 6966 2065 7265 6c20 6973 206e      if erel is n
-00014040: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00014050: 2020 2020 2020 2020 2073 656c 662e 6572           self.er
-00014060: 656c 203d 206e 702e 6173 6661 7272 6179  el = np.asfarray
-00014070: 2865 7265 6c29 2020 2320 696e 6465 7065  (erel)  # indepe
-00014080: 6e64 656e 7420 7265 6c61 7469 7665 2075  ndent relative u
-00014090: 6e63 6572 7461 696e 7469 6573 2078 0a20  ncertainties x. 
-000140a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000140b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000140c0: 2073 656c 662e 6572 656c 203d 204e 6f6e   self.erel = Non
-000140d0: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-000140e0: 2063 6162 7320 6973 206e 6f74 204e 6f6e   cabs is not Non
-000140f0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00014100: 2020 2073 656c 662e 6361 6273 203d 206e     self.cabs = n
-00014110: 702e 6173 6661 7272 6179 2863 6162 7329  p.asfarray(cabs)
-00014120: 2020 2320 636f 7272 656c 6174 6564 2061    # correlated a
-00014130: 626f 6c75 7465 2075 6e63 6572 7461 696e  bolute uncertain
-00014140: 7469 6573 2078 0a20 2020 2020 2020 2020  ties x.         
-00014150: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-00014160: 6162 732e 6e64 696d 203d 3d20 303a 0a20  abs.ndim == 0:. 
-00014170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014180: 2020 2073 656c 662e 6361 6273 203d 2073     self.cabs = s
-00014190: 656c 662e 6361 6273 202a 206e 702e 6f6e  elf.cabs * np.on
-000141a0: 6573 286e 6429 0a20 2020 2020 2020 2020  es(nd).         
-000141b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000141c0: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
-000141d0: 6273 203d 204e 6f6e 650a 2020 2020 2020  bs = None.      
-000141e0: 2020 2020 2020 6966 2063 7265 6c20 6973        if crel is
-000141f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00014200: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014210: 6372 656c 203d 206e 702e 6173 6661 7272  crel = np.asfarr
-00014220: 6179 2863 7265 6c29 2020 2320 636f 7272  ay(crel)  # corr
-00014230: 656c 6174 6564 2072 656c 6174 6976 6520  elated relative 
-00014240: 756e 6365 7274 6169 6e74 6965 7320 780a  uncertainties x.
-00014250: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00014260: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014270: 2020 7365 6c66 2e63 7265 6c20 3d20 4e6f    self.crel = No
-00014280: 6e65 0a20 2020 2020 2020 2020 2020 2073  ne.            s
-00014290: 656c 662e 7175 6965 7420 3d20 7175 6965  elf.quiet = quie
-000142a0: 7420 2023 206e 6f20 696e 666f 726d 6174  t  # no informat
-000142b0: 6976 6520 7072 696e 746f 7574 2069 6620  ive printout if 
-000142c0: 5472 7565 0a0a 2020 2020 2020 2020 2020  True..          
-000142d0: 2020 7365 6c66 2e6e 6420 3d20 6e64 0a20    self.nd = nd. 
-000142e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000142f0: 646c 656e 6774 6820 3d20 6e64 0a20 2020  dlength = nd.   
-00014300: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
-00014310: 6465 6c20 3d20 4e6f 6e65 2020 2320 6e6f  del = None  # no
-00014320: 206d 6f64 656c 2064 6566 696e 6564 2079   model defined y
-00014330: 6574 0a20 2020 2020 2020 2020 2020 2073  et.            s
-00014340: 656c 662e 6d6f 6465 6c5f 7661 6c75 6573  elf.model_values
-00014350: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
-00014360: 2020 2020 2023 2073 6574 2066 6c61 6773       # set flags
-00014370: 2066 6f72 2073 7465 6572 696e 6720 6f66   for steering of
-00014380: 2066 6974 2070 726f 6365 7373 2069 6e20   fit process in 
-00014390: 646f 5f66 6974 2829 0a20 2020 2020 2020  do_fit().       
-000143a0: 2020 2020 2073 656c 662e 7265 6275 6c69       self.rebuli
-000143b0: 6c64 436f 7620 3d20 4e6f 6e65 0a20 2020  ldCov = None.   
-000143c0: 2020 2020 2020 2020 2073 656c 662e 6861           self.ha
-000143d0: 735f 7265 6c5f 4572 726f 7273 203d 2065  s_rel_Errors = e
-000143e0: 7265 6c20 6973 206e 6f74 204e 6f6e 6520  rel is not None 
-000143f0: 6f72 2063 7265 6c20 6973 206e 6f74 204e  or crel is not N
-00014400: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00014410: 7365 6c66 2e6e 6565 6473 5f63 6f76 6172  self.needs_covar
-00014420: 6961 6e63 6520 3d20 280a 2020 2020 2020  iance = (.      
-00014430: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00014440: 6565 6473 5f63 6f76 6172 6961 6e63 6520  eeds_covariance 
-00014450: 6f72 2073 656c 662e 6361 6273 2069 7320  or self.cabs is 
-00014460: 6e6f 7420 4e6f 6e65 206f 7220 7365 6c66  not None or self
-00014470: 2e63 7265 6c20 6973 206e 6f74 204e 6f6e  .crel is not Non
-00014480: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
-00014490: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
-000144a0: 7569 6c64 2028 696e 6974 6961 6c29 2063  uild (initial) c
-000144b0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-000144c0: 2028 7769 7468 6f75 7420 782d 6572 726f   (without x-erro
-000144d0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
-000144e0: 6966 2073 656c 662e 6e65 6564 735f 636f  if self.needs_co
-000144f0: 7661 7269 616e 6365 3a0a 2020 2020 2020  variance:.      
-00014500: 2020 2020 2020 2020 2020 6572 7232 203d            err2 =
-00014510: 205f 6275 696c 645f 436f 764d 6174 280a   _build_CovMat(.
-00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014530: 2020 2020 7365 6c66 2e6e 642c 2073 656c      self.nd, sel
-00014540: 662e 652c 2073 656c 662e 6572 656c 2c20  f.e, self.erel, 
-00014550: 7365 6c66 2e63 6162 732c 2073 656c 662e  self.cabs, self.
-00014560: 6372 656c 2c20 7365 6c66 2e78 0a20 2020  crel, self.x.   
-00014570: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00014580: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00014590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000145a0: 2065 7272 3220 3d20 5f62 7569 6c64 5f45   err2 = _build_E
-000145b0: 7272 3228 7365 6c66 2e65 2c20 7365 6c66  rr2(self.e, self
-000145c0: 2e65 7265 6c2c 2073 656c 662e 7829 0a0a  .erel, self.x)..
-000145d0: 2020 2020 2020 2020 2020 2020 2320 696e              # in
-000145e0: 6974 6961 6c69 7a65 2075 6e63 6572 7461  itialize uncerta
-000145f0: 696e 7469 6573 2061 6e64 2063 6f76 6172  inties and covar
-00014600: 6961 6e63 6520 6d61 7472 6978 2c0a 2020  iance matrix,.  
-00014610: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00014620: 696e 6974 6961 6c43 6f76 2865 7272 3229  initialCov(err2)
-00014630: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00014640: 6574 733a 0a20 2020 2020 2020 2020 2020  ets:.           
-00014650: 2023 2020 2073 656c 662e 636f 7678 3a20   #   self.covx: 
-00014660: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-00014670: 7820 6f66 2078 0a20 2020 2020 2020 2020  x of x.         
-00014680: 2020 2023 2020 2073 656c 662e 636f 7679     #   self.covy
-00014690: 3a20 636f 7661 7269 616e 6365 206d 6174  : covariance mat
-000146a0: 7269 7820 6f66 2079 2075 6e63 6572 7461  rix of y uncerta
-000146b0: 696e 7469 6573 0a20 2020 2020 2020 2020  inties.         
-000146c0: 2020 2023 2020 2073 656c 662e 636f 763a     #   self.cov:
-000146d0: 2066 756c 6c20 636f 7661 7269 616e 6365   full covariance
-000146e0: 206d 6174 7269 7820 696e 636c 2e20 7072   matrix incl. pr
-000146f0: 6f6a 6563 7465 6420 780a 2020 2020 2020  ojected x.      
-00014700: 2020 2020 2020 2320 2020 7365 6c66 2e69        #   self.i
-00014710: 436f 763a 2069 6e76 6572 7365 206f 6620  Cov: inverse of 
-00014720: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
-00014730: 780a 2020 2020 2020 2020 2020 2020 2320  x.            # 
-00014740: 2020 7365 6c66 2e65 7272 323a 2061 7272    self.err2: arr
-00014750: 6179 206f 6620 7371 7561 7265 6420 756e  ay of squared un
-00014760: 6365 7274 6169 6e74 6965 730a 2020 2020  certainties.    
-00014770: 2020 2020 2020 2020 2320 2020 7365 6c66          #   self
-00014780: 2e69 4572 7232 3a20 312e 2f73 656c 662e  .iErr2: 1./self.
-00014790: 6572 7232 0a0a 2020 2020 2020 2020 6465  err2..        de
-000147a0: 6620 5f69 6e69 7469 616c 436f 7628 7365  f _initialCov(se
-000147b0: 6c66 2c20 6572 7232 293a 0a20 2020 2020  lf, err2):.     
-000147c0: 2020 2020 2020 2022 2222 4275 696c 6420         """Build 
-000147d0: 696e 6974 6961 6c20 2873 7461 7469 6329  initial (static)
-000147e0: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-000147f0: 6978 2066 6f72 2079 2d65 7272 6f72 730a  ix for y-errors.
-00014800: 2020 2020 2020 2020 2020 2020 2866 6f72              (for
-00014810: 2070 7265 2d66 6974 2920 616e 6420 6361   pre-fit) and ca
-00014820: 6c63 756c 6174 6520 696e 7665 7273 6520  lculate inverse 
-00014830: 6d61 7472 6978 0a20 2020 2020 2020 2020  matrix.         
-00014840: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
-00014850: 2020 2069 6620 6572 7232 2e6e 6469 6d20     if err2.ndim 
-00014860: 3d3d 2032 3a0a 2020 2020 2020 2020 2020  == 2:.          
-00014870: 2020 2020 2020 2320 676f 7420 6120 636f        # got a co
-00014880: 7661 7269 616e 6365 206d 6174 7269 782c  variance matrix,
-00014890: 206e 6565 6420 696e 7665 7273 650a 2020   need inverse.  
-000148a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000148b0: 6c66 2e6e 6565 6473 5f63 6f76 6172 6961  lf.needs_covaria
-000148c0: 6e63 6520 3d20 5472 7565 0a20 2020 2020  nce = True.     
-000148d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000148e0: 636f 7620 3d20 6572 7232 0a20 2020 2020  cov = err2.     
-000148f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014900: 6943 6f76 203d 206c 696e 616c 672e 696e  iCov = linalg.in
-00014910: 7628 6572 7232 290a 2020 2020 2020 2020  v(err2).        
-00014920: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-00014930: 3220 3d20 6e70 2e64 6961 676f 6e61 6c28  2 = np.diagonal(
-00014940: 6572 7232 2920 2023 2073 7175 6172 6564  err2)  # squared
-00014950: 2064 6961 676f 6e61 6c20 656c 656d 656e   diagonal elemen
-00014960: 7473 0a20 2020 2020 2020 2020 2020 2065  ts.            e
-00014970: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00014980: 2020 2020 2023 2067 6f74 2069 6e64 6570       # got indep
-00014990: 656e 6465 6e74 2075 6e63 6572 7461 696e  endent uncertain
-000149a0: 7469 6573 0a20 2020 2020 2020 2020 2020  ties.           
-000149b0: 2020 2020 2073 656c 662e 6572 7232 203d       self.err2 =
-000149c0: 2065 7272 320a 2020 2020 2020 2020 2020   err2.          
-000149d0: 2020 2020 2020 7365 6c66 2e65 7272 3279        self.err2y
-000149e0: 203d 2065 7272 320a 2020 2020 2020 2020   = err2.        
-000149f0: 2020 2020 2020 2020 7365 6c66 2e69 4572          self.iEr
-00014a00: 7232 203d 2031 2e30 202f 2065 7272 320a  r2 = 1.0 / err2.
-00014a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a20: 7365 6c66 2e63 6f76 203d 206e 702e 6469  self.cov = np.di
-00014a30: 6167 2865 7272 3229 0a20 2020 2020 2020  ag(err2).       
-00014a40: 2020 2020 2020 2020 2073 656c 662e 6943           self.iC
-00014a50: 6f76 203d 206e 702e 6469 6167 2831 2e30  ov = np.diag(1.0
-00014a60: 202f 2073 656c 662e 6572 7232 290a 2020   / self.err2).  
-00014a70: 2020 2020 2020 2020 2020 2320 646f 206e            # do n
-00014a80: 6f74 2072 6562 7569 6c64 2063 6f76 6172  ot rebuild covar
-00014a90: 6961 6e63 6520 6d61 7472 6978 2069 6e20  iance matrix in 
-00014aa0: 636f 7374 2066 756e 6374 696f 6e0a 2020  cost function.  
-00014ab0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00014ac0: 6565 6473 5f64 796e 616d 6963 4572 726f  eeds_dynamicErro
-00014ad0: 7273 203d 2046 616c 7365 0a0a 2020 2020  rs = False..    
-00014ae0: 2020 2020 6465 6620 696e 6974 5f64 796e      def init_dyn
-00014af0: 616d 6963 4572 726f 7273 2873 656c 6629  amicErrors(self)
-00014b00: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00014b10: 6d65 7468 6f64 2074 6f20 7377 6974 6368  method to switch
-00014b20: 206f 6e20 6479 6e61 6d69 6320 7265 2d63   on dynamic re-c
-00014b30: 616c 6375 6c61 7469 6f6e 206f 6620 636f  alculation of co
-00014b40: 7661 7269 616e 6365 206d 6174 7269 780a  variance matrix.
-00014b50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014b60: 2e72 6566 5f74 6f4d 6f64 656c 203d 2073  .ref_toModel = s
-00014b70: 656c 662e 6f75 7465 722e 7265 664d 6f64  elf.outer.refMod
-00014b80: 656c 0a20 2020 2020 2020 2020 2020 2073  el.            s
-00014b90: 656c 662e 6d6f 6465 6c20 3d20 7365 6c66  elf.model = self
-00014ba0: 2e6f 7574 6572 2e63 6f73 7466 2e6d 6f64  .outer.costf.mod
-00014bb0: 656c 0a0a 2020 2020 2020 2020 2020 2020  el..            
-00014bc0: 7365 6c66 2e5f 7374 6174 6963 436f 7620  self._staticCov 
-00014bd0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00014be0: 2020 2073 656c 662e 5f73 7461 7469 6345     self._staticE
-00014bf0: 7272 3220 3d20 4e6f 6e65 0a20 2020 2020  rr2 = None.     
-00014c00: 2020 2020 2020 2073 656c 662e 6943 6f76         self.iCov
-00014c10: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00014c20: 2020 2020 7365 6c66 2e69 4572 7232 203d      self.iErr2 =
-00014c30: 204e 6f6e 650a 0a20 2020 2020 2020 2020   None..         
-00014c40: 2020 2023 2072 6562 7569 6c64 2063 6f76     # rebuild cov
-00014c50: 6172 6961 6e63 6520 6d61 7472 6978 2064  ariance matrix d
-00014c60: 7572 696e 6720 6669 7474 696e 6720 7072  uring fitting pr
-00014c70: 6f63 6564 7572 650a 2020 2020 2020 2020  ocedure.        
-00014c80: 2020 2020 7365 6c66 2e6e 6565 6473 5f64      self.needs_d
-00014c90: 796e 616d 6963 4572 726f 7273 203d 2054  ynamicErrors = T
-00014ca0: 7275 6520 2023 2066 6c61 6720 666f 7220  rue  # flag for 
-00014cb0: 636f 7374 2066 756e 6374 696f 6e0a 2020  cost function.  
-00014cc0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-00014cd0: 696e 616c 5f63 616c 6c20 3d20 4661 6c73  inal_call = Fals
-00014ce0: 6520 2023 2066 6c61 6720 666f 7220 5f72  e  # flag for _r
-00014cf0: 6562 7569 6c64 5f43 6f76 3a20 6e6f 2073  ebuild_Cov: no s
-00014d00: 746f 7261 6765 206f 6620 7963 6f76 0a0a  torage of ycov..
-00014d10: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00014d20: 656c 662e 6e65 6564 735f 636f 7661 7269  elf.needs_covari
-00014d30: 616e 6365 3a0a 2020 2020 2020 2020 2020  ance:.          
-00014d40: 2020 2020 2020 2320 6275 696c 6420 7374        # build st
-00014d50: 6174 6963 2028 3d70 6172 616d 6574 6572  atic (=parameter
-00014d60: 2d69 6e64 6570 656e 6465 6e74 2920 7061  -independent) pa
-00014d70: 7274 206f 6620 636f 7661 7269 616e 6365  rt of covariance
-00014d80: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
-00014d90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00014da0: 6861 735f 7265 6c5f 4572 726f 7273 2061  has_rel_Errors a
-00014db0: 6e64 2073 656c 662e 7265 665f 746f 4d6f  nd self.ref_toMo
-00014dc0: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
-00014dd0: 2020 2020 2020 2020 2023 2073 6f6d 6520           # some 
-00014de0: 792d 6572 726f 7273 2061 7265 2070 6172  y-errors are par
-00014df0: 616d 6574 6572 2d69 6e64 6570 656e 6465  ameter-independe
-00014e00: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-00014e10: 2020 2020 2020 2073 656c 662e 5f73 7461         self._sta
-00014e20: 7469 6343 6f76 203d 205f 6275 696c 645f  ticCov = _build_
-00014e30: 436f 764d 6174 2873 656c 662e 6e64 2c20  CovMat(self.nd, 
-00014e40: 7365 6c66 2e65 2c20 6561 6273 636f 723d  self.e, eabscor=
-00014e50: 7365 6c66 2e63 6162 7329 0a20 2020 2020  self.cabs).     
-00014e60: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00014e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014e80: 2020 2020 2023 2061 6c6c 2079 2d65 7272       # all y-err
-00014e90: 6f72 7320 6172 6520 7061 7261 6d65 7465  ors are paramete
-00014ea0: 722d 696e 6465 7065 6e64 656e 740a 2020  r-independent.  
-00014eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ec0: 2020 7365 6c66 2e5f 7374 6174 6963 436f    self._staticCo
-00014ed0: 7620 3d20 5f62 7569 6c64 5f43 6f76 4d61  v = _build_CovMa
-00014ee0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00014ef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00014f00: 6e64 2c0a 2020 2020 2020 2020 2020 2020  nd,.            
-00014f10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00014f20: 2e65 2c0a 2020 2020 2020 2020 2020 2020  .e,.            
-00014f30: 2020 2020 2020 2020 2020 2020 6572 656c              erel
-00014f40: 3d73 656c 662e 6572 656c 2c0a 2020 2020  =self.erel,.    
-00014f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f60: 2020 2020 6561 6273 636f 723d 7365 6c66      eabscor=self
-00014f70: 2e63 6162 732c 0a20 2020 2020 2020 2020  .cabs,.         
-00014f80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00014f90: 7265 6c63 6f72 3d73 656c 662e 6372 656c  relcor=self.crel
-00014fa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014fb0: 2020 2020 2020 2020 2020 6461 7461 3d73            data=s
-00014fc0: 656c 662e 782c 0a20 2020 2020 2020 2020  elf.x,.         
-00014fd0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00014fe0: 2020 2020 2020 2020 2020 2020 2023 2062               # b
-00014ff0: 7569 6c64 206d 6174 7269 7820 6f66 2072  uild matrix of r
-00015000: 656c 6174 6976 6520 6572 726f 7273 0a20  elative errors. 
-00015010: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015020: 6620 7365 6c66 2e72 6566 5f74 6f4d 6f64  f self.ref_toMod
-00015030: 656c 2061 6e64 2073 656c 662e 6861 735f  el and self.has_
-00015040: 7265 6c5f 4572 726f 7273 3a0a 2020 2020  rel_Errors:.    
-00015050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015060: 7365 6c66 2e5f 636f 7679 3020 3d20 5f62  self._covy0 = _b
-00015070: 7569 6c64 5f43 6f76 4d61 7428 0a20 2020  uild_CovMat(.   
-00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015090: 2020 2020 2073 656c 662e 6e64 2c0a 2020       self.nd,.  
-000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150b0: 2020 2020 2020 6572 656c 3d73 656c 662e        erel=self.
-000150c0: 6572 656c 2c0a 2020 2020 2020 2020 2020  erel,.          
-000150d0: 2020 2020 2020 2020 2020 2020 2020 6572                er
-000150e0: 656c 636f 723d 7365 6c66 2e63 7265 6c2c  elcor=self.crel,
-000150f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015100: 2020 2020 2020 2020 2064 6174 613d 6e70           data=np
-00015110: 2e6f 6e65 7328 7365 6c66 2e6e 6429 2c0a  .ones(self.nd),.
-00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015130: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00015140: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015160: 7365 6c66 2e5f 636f 7679 3020 3d20 4e6f  self._covy0 = No
-00015170: 6e65 0a0a 2020 2020 2020 2020 2020 2020  ne..            
-00015180: 656c 7365 3a20 2023 206e 6f20 636f 7661  else:  # no cova
-00015190: 7269 616e 6365 206e 6565 6465 642c 2075  riance needed, u
-000151a0: 7365 2073 696d 706c 6520 6d61 7468 0a20  se simple math. 
-000151b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000151c0: 2062 7569 6c64 2073 7461 7469 6320 283d   build static (=
-000151d0: 7061 7261 6d65 7465 722d 696e 6465 7065  parameter-indepe
-000151e0: 6e64 656e 7429 2070 6172 7420 6f66 2063  ndent) part of c
-000151f0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-00015200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015210: 2069 6620 7365 6c66 2e68 6173 5f72 656c   if self.has_rel
-00015220: 5f45 7272 6f72 7320 616e 6420 7365 6c66  _Errors and self
-00015230: 2e72 6566 5f74 6f4d 6f64 656c 3a0a 2020  .ref_toModel:.  
-00015240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015250: 2020 2320 6f6e 6c79 2069 6e64 6570 656e    # only indepen
-00015260: 6465 6e74 2079 2d65 7272 6f72 7320 646f  dent y-errors do
-00015270: 206e 6f74 2064 6570 656e 6420 6f6e 2070   not depend on p
-00015280: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-00015290: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000152a0: 6c66 2e5f 7374 6174 6963 4572 7232 203d  lf._staticErr2 =
-000152b0: 205f 6275 696c 645f 4572 7232 2873 656c   _build_Err2(sel
-000152c0: 662e 6529 0a20 2020 2020 2020 2020 2020  f.e).           
-000152d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000152e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000152f0: 2061 6c6c 2079 2d65 7272 6f72 7320 6172   all y-errors ar
-00015300: 6520 7061 7261 6d65 7465 722d 696e 6465  e parameter-inde
-00015310: 7065 6e64 656e 740a 2020 2020 2020 2020  pendent.        
-00015320: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015330: 2e5f 7374 6174 6963 4572 7232 203d 205f  ._staticErr2 = _
-00015340: 6275 696c 645f 4572 7232 2873 656c 662e  build_Err2(self.
-00015350: 652c 2073 656c 662e 6572 656c 2c20 7365  e, self.erel, se
-00015360: 6c66 2e78 290a 0a20 2020 2020 2020 2064  lf.x)..        d
-00015370: 6566 205f 7265 6275 696c 645f 4572 7232  ef _rebuild_Err2
-00015380: 2873 656c 662c 206d 7061 7229 3a0a 2020  (self, mpar):.  
-00015390: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
-000153a0: 2020 2020 2020 2020 2020 2852 652d 2963            (Re-)c
-000153b0: 616c 6375 6c61 7465 2075 6e63 6572 7461  alculate uncerta
-000153c0: 696e 6769 6573 0a20 2020 2020 2020 2020  ingies.         
-000153d0: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
-000153e0: 2020 2069 6620 7365 6c66 2e5f 7374 6174     if self._stat
-000153f0: 6963 4572 7232 2069 7320 6e6f 7420 4e6f  icErr2 is not No
-00015400: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00015410: 2020 2020 7365 6c66 2e65 7272 3220 3d20      self.err2 = 
-00015420: 6e70 2e61 7272 6179 2873 656c 662e 5f73  np.array(self._s
-00015430: 7461 7469 6345 7272 322c 2063 6f70 793d  taticErr2, copy=
-00015440: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00015450: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00015460: 2020 2020 2020 2020 7365 6c66 2e65 7272          self.err
-00015470: 3220 3d20 6e70 2e7a 6572 6f73 2873 656c  2 = np.zeros(sel
-00015480: 662e 6e64 290a 2020 2020 2020 2020 2020  f.nd).          
-00015490: 2020 6966 2073 656c 662e 7265 665f 746f    if self.ref_to
-000154a0: 4d6f 6465 6c20 616e 6420 7365 6c66 2e68  Model and self.h
-000154b0: 6173 5f72 656c 5f45 7272 6f72 733a 0a20  as_rel_Errors:. 
-000154c0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-000154d0: 6572 203d 2073 656c 662e 6572 656c 202a  er = self.erel *
-000154e0: 2073 656c 662e 6d6f 6465 6c28 7365 6c66   self.model(self
-000154f0: 2e78 2c20 2a6d 7061 7229 0a20 2020 2020  .x, *mpar).     
-00015500: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015510: 6572 7232 202b 3d20 5f65 7220 2a20 5f65  err2 += _er * _e
-00015520: 720a 0a20 2020 2020 2020 2064 6566 205f  r..        def _
-00015530: 7265 6275 696c 645f 436f 7628 7365 6c66  rebuild_Cov(self
-00015540: 2c20 6d70 6172 293a 0a20 2020 2020 2020  , mpar):.       
-00015550: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015560: 2020 2020 2028 5265 2d29 4275 696c 6420       (Re-)Build 
-00015570: 7468 6520 636f 7661 7269 616e 6365 206d  the covariance m
-00015580: 6174 7269 7820 6672 6f6d 2063 6f6d 706f  atrix from compo
-00015590: 6e65 6e74 730a 2020 2020 2020 2020 2020  nents.          
-000155a0: 2020 616e 6420 6361 636c 756c 6174 6520    and caclulate 
-000155b0: 6974 7320 696e 7665 7273 650a 2020 2020  its inverse.    
-000155c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000155d0: 2020 2020 2020 2020 2320 7374 6172 7420          # start 
-000155e0: 6672 6f6d 2070 7265 2d62 7569 6c74 2070  from pre-built p
-000155f0: 6172 616d 6574 6572 2d69 6e64 6570 656e  arameter-indepen
-00015600: 6465 6e74 2070 6172 7420 6f66 2043 6f76  dent part of Cov
-00015610: 6172 6961 6e63 6520 4d61 7472 6978 0a20  ariance Matrix. 
-00015620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00015630: 636f 7620 3d20 6e70 2e61 7272 6179 2873  cov = np.array(s
-00015640: 656c 662e 5f73 7461 7469 6343 6f76 2c20  elf._staticCov, 
-00015650: 636f 7079 3d54 7275 6529 0a0a 2020 2020  copy=True)..    
-00015660: 2020 2020 2020 2020 2320 6164 6420 6d61          # add ma
-00015670: 7472 6978 206f 6620 7061 7261 6d65 7465  trix of paramete
-00015680: 722d 6465 7065 6e64 656e 7420 792d 756e  r-dependent y-un
-00015690: 6365 7274 6169 6e74 6965 730a 2020 2020  certainties.    
-000156a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000156b0: 5f63 6f76 7930 2069 7320 6e6f 7420 4e6f  _covy0 is not No
-000156c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000156d0: 2020 2020 5f64 6174 203d 2073 656c 662e      _dat = self.
-000156e0: 6d6f 6465 6c28 7365 6c66 2e78 2c20 2a6d  model(self.x, *m
-000156f0: 7061 7229 0a20 2020 2020 2020 2020 2020  par).           
-00015700: 2020 2020 2073 656c 662e 636f 7620 2b3d       self.cov +=
-00015710: 2073 656c 662e 5f63 6f76 7930 202a 206e   self._covy0 * n
-00015720: 702e 6f75 7465 7228 5f64 6174 2c20 5f64  p.outer(_dat, _d
-00015730: 6174 290a 0a20 2020 2020 2020 2064 6566  at)..        def
-00015740: 2067 6574 5f43 6f76 2873 656c 6629 3a0a   get_Cov(self):.
-00015750: 2020 2020 2020 2020 2020 2020 2222 2272              """r
-00015760: 6574 7572 6e20 636f 7661 7269 616e 6365  eturn covariance
-00015770: 206d 6174 7269 7820 6f66 2064 6174 6122   matrix of data"
-00015780: 2222 0a20 2020 2020 2020 2020 2020 2069  "".            i
-00015790: 6620 7365 6c66 2e6e 6565 6473 5f63 6f76  f self.needs_cov
-000157a0: 6172 6961 6e63 653a 0a20 2020 2020 2020  ariance:.       
-000157b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000157c0: 7365 6c66 2e63 6f76 0a20 2020 2020 2020  self.cov.       
-000157d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000157e0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000157f0: 6c66 2e65 7272 3220 6973 204e 6f6e 653a  lf.err2 is None:
-00015800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015810: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00015820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015830: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00015840: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015850: 6e20 6e70 2e64 6961 6728 7365 6c66 2e65  n np.diag(self.e
-00015860: 7272 3229 0a0a 2020 2020 2020 2020 6465  rr2)..        de
-00015870: 6620 6765 745f 6943 6f76 2873 656c 6629  f get_iCov(self)
-00015880: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
-00015890: 2272 6574 7572 6e20 696e 7665 7273 6520  "return inverse 
-000158a0: 6f66 2063 6f76 6172 6961 6e63 6520 6d61  of covariance ma
-000158b0: 7472 6978 2c20 6173 2075 7365 6420 696e  trix, as used in
-000158c0: 2063 6f73 7420 6675 6e63 7469 6f6e 2222   cost function""
-000158d0: 220a 2020 2020 2020 2020 2020 2020 6966  ".            if
-000158e0: 2073 656c 662e 6e65 6564 735f 636f 7661   self.needs_cova
-000158f0: 7269 616e 6365 3a0a 2020 2020 2020 2020  riance:.        
-00015900: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00015910: 656c 662e 6943 6f76 0a20 2020 2020 2020  elf.iCov.       
-00015920: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00015930: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015940: 6e20 6e70 2e64 6961 6728 312e 3020 2f20  n np.diag(1.0 / 
-00015950: 7365 6c66 2e65 7272 3229 0a0a 2020 2020  self.err2)..    
-00015960: 2020 2020 6465 6620 706c 6f74 280a 2020      def plot(.  
-00015970: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
-00015980: 2020 2020 2020 2020 2020 2020 6e75 6d3d              num=
-00015990: 2244 6174 6120 616e 6420 4d6f 6465 6c22  "Data and Model"
-000159a0: 2c0a 2020 2020 2020 2020 2020 2020 6669  ,.            fi
-000159b0: 6773 697a 653d 2837 2e35 2c20 362e 3529  gsize=(7.5, 6.5)
-000159c0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-000159d0: 7461 5f6c 6162 656c 3d22 6461 7461 222c  ta_label="data",
-000159e0: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
-000159f0: 745f 7265 7369 6475 616c 3d46 616c 7365  t_residual=False
-00015a00: 2c0a 2020 2020 2020 2020 293a 0a20 2020  ,.        ):.   
-00015a10: 2020 2020 2020 2020 2022 2222 7265 7475           """retu
-00015a20: 726e 2066 6967 7572 6520 7769 7468 2064  rn figure with d
-00015a30: 6174 6120 616e 6420 756e 6365 7274 6169  ata and uncertai
-00015a40: 6e74 6965 7322 2222 0a20 2020 2020 2020  nties""".       
-00015a50: 2020 2020 2023 2020 2020 2320 6765 7420       #    # get 
-00015a60: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
-00015a70: 2069 6620 706c 6f74 5f72 6573 6964 7561   if plot_residua
-00015a80: 6c20 616e 6420 7365 6c66 2e6d 6f64 656c  l and self.model
-00015a90: 5f76 616c 7565 7320 6973 206e 6f74 204e  _values is not N
-00015aa0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00015ab0: 2020 2020 2078 203d 2073 656c 662e 7820       x = self.x 
-00015ac0: 2d20 7365 6c66 2e6d 6f64 656c 5f76 616c  - self.model_val
-00015ad0: 7565 730a 2020 2020 2020 2020 2020 2020  ues.            
-00015ae0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00015af0: 2020 2020 2020 7820 3d20 7365 6c66 2e78        x = self.x
-00015b00: 0a20 2020 2020 2020 2020 2020 2065 203d  .            e =
-00015b10: 2073 656c 662e 6765 745f 436f 7628 290a   self.get_Cov().
-00015b20: 2020 2020 2020 2020 2020 2020 6966 2065              if e
-00015b30: 2e6e 6469 6d20 3d3d 2032 3a0a 2020 2020  .ndim == 2:.    
-00015b40: 2020 2020 2020 2020 2020 2020 6520 3d20              e = 
-00015b50: 6e70 2e73 7172 7428 6e70 2e64 6961 676f  np.sqrt(np.diago
-00015b60: 6e61 6c28 6529 290a 2020 2020 2020 2020  nal(e)).        
-00015b70: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015b80: 2020 2020 2020 2020 2020 6520 3d20 6e70            e = np
-00015b90: 2e73 7172 7428 6529 0a20 2020 2020 2020  .sqrt(e).       
-00015ba0: 2020 2020 2023 2064 7261 7720 6461 7461       # draw data
-00015bb0: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
-00015bc0: 203d 2070 6c74 2e66 6967 7572 6528 6e75   = plt.figure(nu
-00015bd0: 6d3d 6e75 6d2c 2066 6967 7369 7a65 3d66  m=num, figsize=f
-00015be0: 6967 7369 7a65 290a 2020 2020 2020 2020  igsize).        
-00015bf0: 2020 2020 6964 7820 3d20 6e70 2e6c 696e      idx = np.lin
-00015c00: 7370 6163 6528 302e 352c 206c 656e 2878  space(0.5, len(x
-00015c10: 2920 2d20 302e 352c 206c 656e 2878 2929  ) - 0.5, len(x))
-00015c20: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
-00015c30: 2e70 6c6f 7428 6964 782c 2078 2c20 6d61  .plot(idx, x, ma
-00015c40: 726b 6572 3d22 7822 2c20 6c69 6e65 7374  rker="x", linest
-00015c50: 796c 653d 2222 2c20 636f 6c6f 723d 2267  yle="", color="g
-00015c60: 7265 7922 2c20 616c 7068 613d 302e 3529  rey", alpha=0.5)
-00015c70: 0a20 2020 2020 2020 2020 2020 2070 6c74  .            plt
-00015c80: 2e65 7272 6f72 6261 7228 6964 782c 2078  .errorbar(idx, x
-00015c90: 2c20 652c 2066 6d74 3d22 2e22 2c20 6361  , e, fmt=".", ca
-00015ca0: 7073 697a 653d 332e 302c 206c 6162 656c  psize=3.0, label
-00015cb0: 3d64 6174 615f 6c61 6265 6c29 0a20 2020  =data_label).   
-00015cc0: 2020 2020 2020 2020 2070 6c74 2e78 6c69           plt.xli
-00015cd0: 6d28 302e 302c 206c 656e 2869 6478 2929  m(0.0, len(idx))
-00015ce0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015cf0: 7365 6c66 2e78 4e61 6d65 7320 6973 206e  self.xNames is n
-00015d00: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00015d10: 2020 2020 2020 2020 2070 6c74 2e78 7469           plt.xti
-00015d20: 636b 7328 7469 636b 733d 6964 782c 206c  cks(ticks=idx, l
-00015d30: 6162 656c 733d 7365 6c66 2e78 4e61 6d65  abels=self.xName
-00015d40: 7329 0a20 2020 2020 2020 2020 2020 2065  s).            e
-00015d50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00015d60: 2020 2020 2070 6c74 2e78 7469 636b 7328       plt.xticks(
-00015d70: 7469 636b 733d 6964 782c 206c 6162 656c  ticks=idx, label
-00015d80: 733d 7261 6e67 6528 6c65 6e28 6964 7829  s=range(len(idx)
-00015d90: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
-00015da0: 7265 7475 726e 2066 6967 0a0a 2020 2020  return fig..    
-00015db0: 2320 6465 6669 6e65 2063 7573 746f 6d20  # define custom 
-00015dc0: 636f 7374 2066 756e 6374 696f 6e20 666f  cost function fo
-00015dd0: 7220 696d 696e 7569 740a 2020 2020 636c  r iminuit.    cl
-00015de0: 6173 7320 696e 6465 7865 6443 6f73 743a  ass indexedCost:
-00015df0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00015e00: 2020 2020 2020 4375 7374 6f6d 2065 5f78        Custom e_x
-00015e10: 5f74 656e 6465 6420 4c65 6173 742d 5351  _tended Least-SQ
-00015e20: 7561 7265 7320 636f 7374 2066 756e 6374  uares cost funct
-00015e30: 696f 6e20 7769 7468 0a20 2020 2020 2020  ion with.       
-00015e40: 2020 6479 6e61 6d69 6361 6c6c 7920 7570    dynamically up
-00015e50: 6461 7465 6420 636f 7661 7269 616e 6365  dated covariance
-00015e60: 206d 6174 7269 7820 616e 6420 2d32 6c6f   matrix and -2lo
-00015e70: 6728 4c29 0a20 2020 2020 2020 2020 636f  g(L).         co
-00015e80: 7272 6563 7469 6f6e 2074 6572 6d20 666f  rrection term fo
-00015e90: 7220 7061 7261 6d65 7465 722d 6465 7065  r parameter-depe
-00015ea0: 6e64 656e 7420 756e 6365 7274 6169 6e74  ndent uncertaint
-00015eb0: 6965 732e 0a0a 2020 2020 2020 2020 2054  ies...         T
-00015ec0: 6865 2064 6566 6175 6c74 2063 6f73 7420  he default cost 
-00015ed0: 6675 6e63 7469 6f6e 2069 7320 7477 6963  function is twic
-00015ee0: 6520 7468 6520 6e65 6761 7469 7665 206c  e the negative l
-00015ef0: 6f67 6172 6974 686d 0a20 2020 2020 2020  ogarithm.       
-00015f00: 2020 6f66 2074 6865 206c 696b 656c 6968    of the likelih
-00015f10: 6f6f 6420 6f66 2061 2047 6175 7373 6961  ood of a Gaussia
-00015f20: 6e20 6469 7374 7269 6275 7469 6f6e 2066  n distribution f
-00015f30: 6f72 2064 6174 6120 706f 696e 7473 0a20  or data points. 
-00015f40: 2020 2020 2020 2020 3a6d 6174 683a 6028          :math:`(
-00015f50: 782c 2079 2960 2077 6974 6820 6120 6d6f  x, y)` with a mo
-00015f60: 6465 6c20 6675 6e63 7469 6f6e 203a 6d61  del function :ma
-00015f70: 7468 3a60 793d 6628 782c 202a 7029 6020  th:`y=f(x, *p)` 
-00015f80: 6465 7065 6e64 696e 670a 2020 2020 2020  depending.      
-00015f90: 2020 206f 6e20 6120 7365 7420 6f66 2070     on a set of p
-00015fa0: 6172 616d 6574 6572 7320 3a6d 6174 683a  arameters :math:
-00015fb0: 602a 7060 2061 6e64 2061 2070 6f73 7369  `*p` and a possi
-00015fc0: 626c 7920 7061 7261 6d65 7465 722d 6465  bly parameter-de
-00015fd0: 7065 6e64 656e 740a 2020 2020 2020 2020  pendent.        
-00015fe0: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-00015ff0: 6978 203a 6d61 7468 3a60 5628 782c 2066  ix :math:`V(x, f
-00016000: 2878 2c20 2a70 2929 6020 6f66 2074 6865  (x, *p))` of the
-00016010: 2078 2061 6e64 2079 2064 6174 613a 0a0a   x and y data:..
-00016020: 2020 2020 2020 2020 202e 2e20 6d61 7468           .. math
-00016030: 3a3a 0a20 2020 2020 2020 2020 2020 2d32  ::.           -2
-00016040: 5c6c 6e20 7b5c 6361 6c20 4c7d 203d 205c  \ln {\cal L} = \
-00016050: 6368 695e 3228 782c 2056 5e7b 2d31 7d2c  chi^2(x, V^{-1},
-00016060: 2078 282a 7029 205c 2c29 0a20 2020 2020   x(*p) \,).     
-00016070: 2020 2020 2020 2b20 5c6c 6e28 5c2c 205c        + \ln(\, \
-00016080: 6465 7428 2056 2878 2c20 7828 2a70 2920  det( V(x, x(*p) 
-00016090: 2920 5c2c 290a 0a20 2020 2020 2020 2020  ) \,)..         
-000160a0: 496e 2074 6865 2061 6273 656e 6365 206f  In the absence o
-000160b0: 6620 7061 7261 6d65 7465 722d 6465 7065  f parameter-depe
-000160c0: 6e64 656e 7420 636f 6d70 6f6e 656e 7473  ndent components
-000160d0: 206f 6620 7468 6520 636f 7661 7269 616e   of the covarian
-000160e0: 6365 0a20 2020 2020 2020 2020 6d61 7472  ce.         matr
-000160f0: 6978 2c20 7468 6520 6c61 7374 2074 6572  ix, the last ter
-00016100: 6d20 6973 206f 6d69 7474 6564 2061 6e64  m is omitted and
-00016110: 2074 6865 2063 6f73 7420 6675 6e63 7469   the cost functi
-00016120: 6f6e 2069 7320 6964 656e 7469 6361 6c0a  on is identical.
-00016130: 2020 2020 2020 2020 2074 6f20 7468 6520           to the 
-00016140: 636c 6173 7369 6361 6c20 3a6d 6174 683a  classical :math:
-00016150: 605c 6368 695e 3260 2e0a 2020 2020 2020  `\chi^2`..      
-00016160: 2020 2046 6f72 2074 6865 2065 7661 6c75     For the evalu
-00016170: 6174 696f 6e20 6f66 2074 6865 2063 6f73  ation of the cos
-00016180: 7420 6675 6e63 7469 6f6e 2061 6e20 6566  t function an ef
-00016190: 6669 6369 656e 7420 6170 7072 6f61 6368  ficient approach
-000161a0: 2062 6173 6564 0a20 2020 2020 2020 2020   based.         
-000161b0: 6f6e 2074 6865 2022 4368 6f6c 6573 6b79  on the "Cholesky
-000161c0: 2064 6563 6f6d 706f 7369 7469 6f6e 2220   decomposition" 
-000161d0: 6f66 2074 6865 2063 6f76 6172 6961 6e63  of the covarianc
-000161e0: 6520 6d61 7472 6978 2069 6e0a 2020 2020  e matrix in.    
-000161f0: 2020 2020 2061 2070 726f 6475 6374 206f       a product o
-00016200: 6620 6120 7472 6961 6e67 756c 6172 206d  f a triangular m
-00016210: 6174 7269 7820 616e 6420 6974 7320 7472  atrix and its tr
-00016220: 616e 7370 6f73 6564 2069 7320 7573 6564  ansposed is used
-00016230: 3a0a 0a20 2020 2020 2020 2020 2e2e 206d  :..         .. m
-00016240: 6174 683a 3a0a 2020 2020 2020 2020 2020  ath::.          
-00016250: 2020 5620 3d20 4c20 4c5e 542e 0a0a 2020    V = L L^T...  
-00016260: 2020 2020 2020 2054 6865 2076 616c 7565         The value
-00016270: 206f 6620 7468 6520 636f 7374 2066 756e   of the cost fun
-00016280: 6374 696f 6e0a 0a20 2020 2020 2020 2020  ction..         
-00016290: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
-000162a0: 2020 2020 205c 6368 695e 3220 3d20 7b72       \chi^2 = {r
-000162b0: 7d5c 6364 6f74 2028 565e 7b2d 317d 7b72  }\cdot (V^{-1}{r
-000162c0: 7d29 207e 7e77 6974 687e 7e20 7220 3d20  }) ~~with~~ r = 
-000162d0: 7820 2d20 7828 2a70 290a 0a20 2020 2020  x - x(*p)..     
-000162e0: 2020 2020 6973 2074 6865 6e20 6361 6c63      is then calc
-000162f0: 756c 6174 6564 2062 7920 736f 6c76 696e  ulated by solvin
-00016300: 6720 7468 6520 6c69 6e65 6172 2065 7175  g the linear equ
-00016310: 6174 696f 6e0a 0a20 2020 2020 2020 202e  ation..        .
-00016320: 2e20 6d61 7468 3a3a 0a20 2020 2020 2020  . math::.       
-00016330: 2020 2020 5620 5820 3d20 722c 207e 692e      V X = r, ~i.
-00016340: 652e 7e20 583d 565e 7b2d 317d 2072 207e  e.~ X=V^{-1} r ~
-00016350: 616e 647e 205c 6368 695e 323d 2072 205c  and~ \chi^2= r \
-00016360: 6364 6f74 2058 0a0a 2020 2020 2020 2020  cdot X..        
-00016370: 7769 7468 2074 6865 206c 696e 6561 722d  with the linear-
-00016380: 6571 7561 7469 6f6e 2073 6f6c 7665 7220  equation solver 
-00016390: 2a73 6369 7079 2e6c 696e 616c 672e 6368  *scipy.linalg.ch
-000163a0: 6f5f 736f 6c76 6528 4c2c 7829 2a0a 2020  o_solve(L,x)*.  
-000163b0: 2020 2020 2020 666f 7220 4368 6f6c 6573        for Choles
-000163c0: 6b79 2d64 6563 6f6d 706f 7365 6420 6d61  ky-decomposed ma
-000163d0: 7472 6963 6573 2c20 7468 7573 2061 766f  trices, thus avo
-000163e0: 6964 696e 6720 7468 6520 636f 7374 790a  iding the costy.
-000163f0: 2020 2020 2020 2020 6361 6c63 756c 6174          calculat
-00016400: 696f 6e20 6f66 2074 6865 2069 6e76 6572  ion of the inver
-00016410: 7365 206d 6174 7269 782e 0a0a 0a20 2020  se matrix....   
-00016420: 2020 2020 2054 6865 2064 6574 6572 6d69       The determi
-00016430: 6e61 6e74 2c20 6966 206e 6565 6465 642c  nant, if needed,
-00016440: 2069 7320 6566 6669 6369 656e 746c 7920   is efficiently 
-00016450: 6361 6c63 756c 6174 6564 2062 7920 7461  calculated by ta
-00016460: 6b69 6e67 0a20 2020 2020 2020 2074 6865  king.        the
-00016470: 2070 726f 6475 6374 206f 6620 7468 6520   product of the 
-00016480: 6469 6167 6f6e 616c 2065 6c65 6d65 6e74  diagonal element
-00016490: 7320 6f66 2074 6865 206d 6174 7269 7820  s of the matrix 
-000164a0: 4c2c 0a0a 2020 2020 2020 2020 202e 2e20  L,..         .. 
-000164b0: 6d61 7468 3a3a 0a20 2020 2020 2020 2020  math::.         
-000164c0: 2020 5c64 6574 2856 2920 3d20 3220 5c2c    \det(V) = 2 \,
-000164d0: 205c 7072 6f64 204c 5f7b 692c 697d 0a0a   \prod L_{i,i}..
-000164e0: 2020 2020 2020 2020 2049 6e70 7574 3a0a           Input:.
-000164f0: 0a20 2020 2020 2020 2020 2d20 6f75 7465  .         - oute
-00016500: 723a 2070 6f69 6e74 6572 2074 6f20 696e  r: pointer to in
-00016510: 7374 616e 6365 206f 6620 6361 6c6c 696e  stance of callin
-00016520: 6720 636c 6173 730a 2020 2020 2020 2020  g class.        
-00016530: 202d 206d 6f64 656c 3a20 6d6f 6465 6c20   - model: model 
-00016540: 6675 6e63 7469 6f6e 2063 616c 756c 6174  function calulat
-00016550: 696e 6720 7468 6520 6461 7461 2078 285c  ing the data x(\
-00016560: 2a70 6172 290a 2020 2020 2020 2020 202d  *par).         -
-00016570: 2075 7365 5f6e 6567 326c 6f67 4c3a 2075   use_neg2logL: u
-00016580: 7365 2066 756c 6c20 2d32 6c6f 6728 4c29  se full -2log(L)
-00016590: 2069 6e73 7465 6164 206f 6620 6368 6932   instead of chi2
-000165a0: 2069 6620 5472 7565 0a0a 2020 2020 2020   if True..      
-000165b0: 2020 205f 5f63 616c 6c5f 5f20 6d65 7468     __call__ meth
-000165c0: 6f64 206f 6620 7468 6973 2063 6c61 7373  od of this class
-000165d0: 2069 7320 6361 6c6c 6564 2062 7920 696d   is called by im
-000165e0: 696e 7569 740a 0a20 2020 2020 2020 2020  inuit..         
-000165f0: 4461 7461 206d 656d 6265 7273 3a0a 0a20  Data members:.. 
-00016600: 2020 2020 2020 2020 2d20 6e64 6f66 3a20          - ndof: 
-00016610: 6465 6772 6565 7320 6f66 2066 7265 6564  degrees of freed
-00016620: 6f6d 0a20 2020 2020 2020 2020 2d20 6e63  om.         - nc
-00016630: 6f6e 7374 7261 696e 7473 3a20 6e75 6d62  onstraints: numb
-00016640: 6572 206f 6620 7061 7261 6d65 7465 7220  er of parameter 
-00016650: 636f 6e73 7472 6169 6e74 730a 2020 2020  constraints.    
-00016660: 2020 2020 202d 2067 6f66 3a20 6368 6932       - gof: chi2
-00016670: 2d76 616c 7565 2028 676f 6f64 6e65 7373  -value (goodness
-00016680: 206f 6620 6669 7429 0a20 2020 2020 2020   of fit).       
-00016690: 2020 2d20 7573 655f 6e65 6732 6c6f 674c    - use_neg2logL
-000166a0: 3a20 7573 6167 6520 6f66 2066 756c 6c20  : usage of full 
-000166b0: 322a 6e65 6720 4c6f 6720 4c69 6b65 6c69  2*neg Log Likeli
-000166c0: 686f 6f64 0a20 2020 2020 2020 2020 2d20  hood.         - 
-000166d0: 7175 6965 743a 206e 6f20 7072 696e 746f  quiet: no printo
-000166e0: 7574 2069 6620 5472 7565 0a0a 2020 2020  ut if True..    
-000166f0: 2020 2020 204d 6574 686f 6473 3a0a 0a20       Methods:.. 
-00016700: 2020 2020 2020 2020 2d20 6d6f 6465 6c28          - model(
-00016710: 782c 205c 2a70 6172 290a 2020 2020 2020  x, \*par).      
-00016720: 2020 2222 220a 0a20 2020 2020 2020 2064    """..        d
-00016730: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00016740: 2c20 6f75 7465 722c 206d 6f64 656c 2c20  , outer, model, 
-00016750: 7573 655f 6e65 6732 6c6f 674c 3d46 616c  use_neg2logL=Fal
-00016760: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
-00016770: 2023 2064 6174 6120 6f62 6a65 6374 206f   # data object o
-00016780: 6620 7479 7065 2078 7944 6174 6143 6f6e  f type xyDataCon
-00016790: 7461 696e 6572 0a20 2020 2020 2020 2020  tainer.         
-000167a0: 2020 2073 656c 662e 6461 7461 203d 206f     self.data = o
-000167b0: 7574 6572 2e64 6174 610a 2020 2020 2020  uter.data.      
-000167c0: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-000167d0: 6e73 7461 6e63 6528 7365 6c66 2e64 6174  nstance(self.dat
-000167e0: 612c 206d 6e46 6974 2e78 4461 7461 436f  a, mnFit.xDataCo
-000167f0: 6e74 6169 6e65 7229 3a0a 2020 2020 2020  ntainer):.      
-00016800: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00016810: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016830: 2220 2121 2120 6d6e 4669 742e 696e 6465  " !!! mnFit.inde
-00016840: 7865 6443 6f73 743a 2065 7870 6563 7469  xedCost: expecti
-00016850: 6e67 2064 6174 6120 636f 6e74 6169 6e65  ng data containe
-00016860: 7220 6f66 2074 7970 6520 276d 6e46 6974  r of type 'mnFit
-00016870: 2e78 4461 7461 436f 6e74 6169 6e65 7227  .xDataContainer'
-00016880: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00016890: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-000168a0: 7365 6c66 2e6d 6f64 656c 203d 206d 6f64  self.model = mod
-000168b0: 656c 0a20 2020 2020 2020 2020 2020 2073  el.            s
-000168c0: 656c 662e 7175 6965 7420 3d20 6f75 7465  elf.quiet = oute
-000168d0: 722e 7175 6965 740a 2020 2020 2020 2020  r.quiet.        
-000168e0: 2020 2020 2320 7573 6520 2d32 202a 206c      # use -2 * l
-000168f0: 6f67 284c 2920 6f66 2047 6175 7373 6961  og(L) of Gaussia
-00016900: 6e20 696e 7374 6561 6420 6f66 2043 6869  n instead of Chi
-00016910: 320a 2020 2020 2020 2020 2020 2020 2320  2.            # 
-00016920: 2028 6f6e 6c79 2064 6966 6665 7265 6e74   (only different
-00016930: 2066 726f 6d20 4368 6932 2066 6f72 2070   from Chi2 for p
-00016940: 6172 616d 6574 6572 2d64 6570 656e 6465  arameter-depende
-00016950: 6e74 2075 6e63 6572 7461 696e 7469 6573  nt uncertainties
-00016960: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00016970: 6c66 2e75 7365 5f6e 6567 326c 6f67 4c20  lf.use_neg2logL 
-00016980: 3d20 7573 655f 6e65 6732 6c6f 674c 0a0a  = use_neg2logL..
-00016990: 2020 2020 2020 2020 2020 2020 2320 7365              # se
-000169a0: 7420 7072 6f70 6572 2073 6967 6e61 7475  t proper signatu
-000169b0: 7265 206f 6620 6d6f 6465 6c20 6675 6e63  re of model func
-000169c0: 7469 6f6e 2066 6f72 2069 6d69 6e75 6974  tion for iminuit
-000169d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000169e0: 662e 706e 616d 7320 3d20 6f75 7465 722e  f.pnams = outer.
-000169f0: 706e 616d 730a 2020 2020 2020 2020 2020  pnams.          
-00016a00: 2020 7365 6c66 2e6e 7061 7220 3d20 6f75    self.npar = ou
-00016a10: 7465 722e 6e70 6172 0a0a 2020 2020 2020  ter.npar..      
-00016a20: 2020 2020 2020 2320 7461 6b65 2061 6363        # take acc
-00016a30: 6f75 6e74 206f 6620 636f 6e73 7472 6169  ount of constrai
-00016a40: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-00016a50: 7365 6c66 2e63 6f6e 7374 7261 696e 7473  self.constraints
-00016a60: 203d 206f 7574 6572 2e63 6f6e 7374 7261   = outer.constra
-00016a70: 696e 7473 0a20 2020 2020 2020 2020 2020  ints.           
-00016a80: 2073 656c 662e 6e63 6f6e 7374 7261 696e   self.nconstrain
-00016a90: 7473 203d 206c 656e 2873 656c 662e 636f  ts = len(self.co
-00016aa0: 6e73 7472 6169 6e74 7329 0a20 2020 2020  nstraints).     
-00016ab0: 2020 2020 2020 2073 656c 662e 6e64 6f66         self.ndof
-00016ac0: 203d 206c 656e 2873 656c 662e 6461 7461   = len(self.data
-00016ad0: 2e78 2920 2d20 7365 6c66 2e6e 7061 7220  .x) - self.npar 
-00016ae0: 2b20 7365 6c66 2e6e 636f 6e73 7472 6169  + self.nconstrai
-00016af0: 6e74 7320 2b20 6f75 7465 722e 6e66 6978  nts + outer.nfix
-00016b00: 6564 0a0a 2020 2020 2020 2020 2020 2020  ed..            
-00016b10: 2320 666c 6167 2074 6f20 636f 6e74 726f  # flag to contro
-00016b20: 6c20 6669 6e61 6c20 6163 7469 6f6e 7320  l final actions 
-00016b30: 696e 2063 6f73 7420 6675 6e63 7469 6f6e  in cost function
-00016b40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00016b50: 662e 6669 6e61 6c5f 6361 6c6c 203d 2046  f.final_call = F
-00016b60: 616c 7365 0a0a 2020 2020 2020 2020 6465  alse..        de
-00016b70: 6620 5f5f 6361 6c6c 5f5f 2873 656c 662c  f __call__(self,
-00016b80: 202a 7061 7229 3a0a 2020 2020 2020 2020   *par):.        
-00016b90: 2020 2020 2320 6361 6c6c 6564 2069 7465      # called ite
-00016ba0: 7261 7469 7665 6c79 2062 7920 6d69 6e75  ratively by minu
-00016bb0: 6974 0a0a 2020 2020 2020 2020 2020 2020  it..            
-00016bc0: 2320 636f 7374 2066 756e 6374 696f 6e20  # cost function 
-00016bd0: 6973 2065 7874 656e 6465 6420 6368 6932  is extended chi2
-00016be0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00016bf0: 2020 6164 6420 6e6f 726d 616c 697a 6174    add normalizat
-00016c00: 696f 6e20 7465 726d 2069 6620 756e 6365  ion term if unce
-00016c10: 7274 6169 6e74 6965 7320 6465 7065 6e64  rtainties depend
-00016c20: 206f 6e20 6d6f 6465 6c0a 0a20 2020 2020   on model..     
-00016c30: 2020 2020 2020 206e 6c4c 3220 3d20 302e         nlL2 = 0.
-00016c40: 3020 2023 2069 6e69 7469 616c 697a 6520  0  # initialize 
-00016c50: 2d32 2a6c 6e28 4c29 0a20 2020 2020 2020  -2*ln(L).       
-00016c60: 2020 2020 2023 2020 6669 7273 742c 2074       #  first, t
-00016c70: 616b 6520 696e 746f 2061 6363 6f75 6e74  ake into account
-00016c80: 2070 6f73 7369 626c 6520 7061 7261 6d65   possible parame
-00016c90: 7465 7220 636f 6e73 7472 6169 6e74 730a  ter constraints.
-00016ca0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00016cb0: 656c 662e 6e63 6f6e 7374 7261 696e 7473  elf.nconstraints
-00016cc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016cd0: 2020 666f 7220 6320 696e 2073 656c 662e    for c in self.
-00016ce0: 636f 6e73 7472 6169 6e74 733a 0a20 2020  constraints:.   
-00016cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d00: 2070 5f69 6420 3d20 635b 305d 0a20 2020   p_id = c[0].   
-00016d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d20: 2072 203d 2028 7061 725b 705f 6964 5d20   r = (par[p_id] 
-00016d30: 2d20 635b 315d 2920 2f20 635b 325d 0a20  - c[1]) / c[2]. 
-00016d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016d50: 2020 206e 6c4c 3220 2b3d 2072 202a 2072     nlL2 += r * r
-00016d60: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00016d70: 6361 6c63 756c 6174 6520 7265 7369 6475  calculate residu
-00016d80: 616c 206f 6620 6461 7461 2077 7274 2e20  al of data wrt. 
-00016d90: 6d6f 6465 6c0a 2020 2020 2020 2020 2020  model.          
-00016da0: 2020 6d6f 6465 6c5f 7661 6c75 6573 203d    model_values =
-00016db0: 2073 656c 662e 6d6f 6465 6c28 7365 6c66   self.model(self
-00016dc0: 2e64 6174 612e 782c 202a 7061 7229 0a20  .data.x, *par). 
-00016dd0: 2020 2020 2020 2020 2020 205f 7220 3d20             _r = 
-00016de0: 7365 6c66 2e64 6174 612e 7820 2d20 6d6f  self.data.x - mo
-00016df0: 6465 6c5f 7661 6c75 6573 0a0a 2020 2020  del_values..    
-00016e00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00016e10: 6461 7461 2e6e 6565 6473 5f63 6f76 6172  data.needs_covar
-00016e20: 6961 6e63 653a 0a20 2020 2020 2020 2020  iance:.         
-00016e30: 2020 2020 2020 2023 2020 6368 6563 6b20         #  check 
-00016e40: 6966 206d 6174 7269 7820 6e65 6564 7320  if matrix needs 
-00016e50: 7265 6275 696c 6469 6e67 0a20 2020 2020  rebuilding.     
-00016e60: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00016e70: 7420 7365 6c66 2e64 6174 612e 6e65 6564  t self.data.need
-00016e80: 735f 6479 6e61 6d69 6345 7272 6f72 733a  s_dynamicErrors:
-00016e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ea0: 2020 2020 2023 2073 7461 7469 6320 636f       # static co
-00016eb0: 7661 7269 616e 6365 2c20 7573 6520 6974  variance, use it
-00016ec0: 7320 696e 7665 7273 650a 2020 2020 2020  s inverse.      
-00016ed0: 2020 2020 2020 2020 2020 2020 2020 6e6c                nl
-00016ee0: 4c32 202b 3d20 666c 6f61 7428 6e70 2e69  L2 += float(np.i
-00016ef0: 6e6e 6572 286e 702e 6d61 746d 756c 285f  nner(np.matmul(_
-00016f00: 722c 2073 656c 662e 6461 7461 2e69 436f  r, self.data.iCo
-00016f10: 7629 2c20 5f72 2929 0a20 2020 2020 2020  v), _r)).       
-00016f20: 2020 2020 2020 2020 2020 2020 2023 2069               # i
-00016f30: 6465 6e74 6963 616c 2074 6f20 636c 6173  dentical to clas
-00016f40: 7369 6361 6c20 4368 6932 0a20 2020 2020  sical Chi2.     
-00016f50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016f60: 656c 662e 676f 6620 3d20 6e6c 4c32 0a0a  elf.gof = nlL2..
-00016f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f80: 656c 7365 3a20 2023 2064 796e 616d 6963  else:  # dynamic
-00016f90: 616c 6c79 2072 6562 7569 6c64 2063 6f76  ally rebuild cov
-00016fa0: 6172 6961 6e63 6520 6d61 7472 6978 0a20  ariance matrix. 
-00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016fc0: 2020 2073 656c 662e 6461 7461 2e5f 7265     self.data._re
-00016fd0: 6275 696c 645f 436f 7628 7061 7229 0a20  build_Cov(par). 
-00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ff0: 2020 2023 2075 7365 2043 686f 6c65 736b     # use Cholesk
-00017000: 7920 6465 636f 6d70 6f73 6974 6f6e 2074  y decompositon t
-00017010: 6f20 636f 6d70 7574 6520 6368 6932 203d  o compute chi2 =
-00017020: 205f 722e 5420 2856 5e2d 3129 205f 720a   _r.T (V^-1) _r.
-00017030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017040: 2020 2020 4c2c 2069 735f 6c6f 7765 7220      L, is_lower 
-00017050: 3d20 6c69 6e61 6c67 2e63 686f 5f66 6163  = linalg.cho_fac
-00017060: 746f 7228 7365 6c66 2e64 6174 612e 636f  tor(self.data.co
-00017070: 762c 2063 6865 636b 5f66 696e 6974 653d  v, check_finite=
-00017080: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-00017090: 2020 2020 2020 2020 2020 206e 6c4c 3220             nlL2 
-000170a0: 2b3d 206e 702e 696e 6e65 7228 5f72 2c20  += np.inner(_r, 
-000170b0: 6c69 6e61 6c67 2e63 686f 5f73 6f6c 7665  linalg.cho_solve
-000170c0: 2828 4c2c 2069 735f 6c6f 7765 7229 2c20  ((L, is_lower), 
-000170d0: 5f72 2929 0a20 2020 2020 2020 2020 2020  _r)).           
-000170e0: 2020 2020 2020 2020 2023 2075 7020 746f           # up to
-000170f0: 2068 6572 652c 2069 6465 6e74 6963 616c   here, identical
-00017100: 2074 6f20 636c 6173 7369 6361 6c20 4368   to classical Ch
-00017110: 6932 0a20 2020 2020 2020 2020 2020 2020  i2.             
-00017120: 2020 2020 2020 2073 656c 662e 676f 6620         self.gof 
-00017130: 3d20 6e6c 4c32 0a20 2020 2020 2020 2020  = nlL2.         
-00017140: 2020 2020 2020 2020 2020 2023 2074 616b             # tak
-00017150: 6520 696e 746f 2061 6363 6f75 6e74 2070  e into account p
-00017160: 6172 616d 6574 6572 2d64 6570 656e 6465  arameter-depende
-00017170: 6e74 206e 6f72 6d61 6c69 7361 7469 6f6e  nt normalisation
-00017180: 2074 6572 6d0a 2020 2020 2020 2020 2020   term.          
-00017190: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-000171a0: 662e 7573 655f 6e65 6732 6c6f 674c 3a0a  f.use_neg2logL:.
-000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171c0: 2020 2020 2020 2020 2320 2066 6173 7420          #  fast 
-000171d0: 6361 6c63 756c 6174 696f 6e20 6f66 2064  calculation of d
-000171e0: 6574 6572 6d69 6e61 6e74 2064 6574 2856  eterminant det(V
-000171f0: 2920 6672 6f6d 2043 686f 6c65 736b 7920  ) from Cholesky 
-00017200: 6661 6374 6f72 0a20 2020 2020 2020 2020  factor.         
-00017210: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00017220: 6c4c 3220 2b3d 2032 2e30 202a 206e 702e  lL2 += 2.0 * np.
-00017230: 7375 6d28 6e70 2e6c 6f67 286e 702e 6469  sum(np.log(np.di
-00017240: 6167 6f6e 616c 284c 2929 290a 0a20 2020  agonal(L)))..   
-00017250: 2020 2020 2020 2020 2065 6c73 653a 2020           else:  
-00017260: 2320 6661 7374 2063 616c 6375 6c61 7469  # fast calculati
-00017270: 6f6e 2066 6f72 2073 696d 706c 6520 6572  on for simple er
-00017280: 726f 7273 0a20 2020 2020 2020 2020 2020  rors.           
-00017290: 2020 2020 2023 2063 6865 636b 2069 6620       # check if 
-000172a0: 6572 726f 7273 206e 6565 6473 2072 6563  errors needs rec
-000172b0: 616c 6375 6c61 7469 6e67 0a20 2020 2020  alculating.     
-000172c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000172d0: 6c66 2e64 6174 612e 6e65 6564 735f 6479  lf.data.needs_dy
-000172e0: 6e61 6d69 6345 7272 6f72 733a 0a20 2020  namicErrors:.   
-000172f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017300: 2073 656c 662e 6461 7461 2e5f 7265 6275   self.data._rebu
-00017310: 696c 645f 4572 7232 2870 6172 290a 2020  ild_Err2(par).  
-00017320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017330: 2020 6e6c 4c32 202b 3d20 6e70 2e73 756d    nlL2 += np.sum
-00017340: 285f 7220 2a20 5f72 202f 2073 656c 662e  (_r * _r / self.
-00017350: 6461 7461 2e65 7272 3229 0a20 2020 2020  data.err2).     
-00017360: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00017370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017380: 2020 2020 206e 6c4c 3220 2b3d 206e 702e       nlL2 += np.
-00017390: 7375 6d28 5f72 202a 205f 7220 2a20 7365  sum(_r * _r * se
-000173a0: 6c66 2e64 6174 612e 6945 7272 3229 0a0a  lf.data.iErr2)..
-000173b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173c0: 2320 7468 6973 2069 7320 6964 656e 7469  # this is identi
-000173d0: 6361 6c20 746f 2063 6c61 7373 6963 616c  cal to classical
-000173e0: 2043 6869 320a 2020 2020 2020 2020 2020   Chi2.          
-000173f0: 2020 2020 2020 7365 6c66 2e67 6f66 203d        self.gof =
-00017400: 206e 6c4c 320a 0a20 2020 2020 2020 2020   nlL2..         
-00017410: 2020 2020 2020 2023 2061 6464 2070 6172         # add par
-00017420: 616d 6574 6572 2d64 6570 656e 6465 6e74  ameter-dependent
-00017430: 206e 6f72 6d61 6c69 7a61 7469 6f6e 2074   normalization t
-00017440: 6572 6d20 6966 206e 6565 6465 6420 616e  erm if needed an
-00017450: 6420 7761 6e74 6564 0a20 2020 2020 2020  d wanted.       
-00017460: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00017470: 2e64 6174 612e 6e65 6564 735f 6479 6e61  .data.needs_dyna
-00017480: 6d69 6345 7272 6f72 7320 616e 6420 7365  micErrors and se
-00017490: 6c66 2e75 7365 5f6e 6567 326c 6f67 4c3a  lf.use_neg2logL:
-000174a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000174b0: 2020 2020 206e 6c4c 3220 2b3d 206e 702e       nlL2 += np.
-000174c0: 7375 6d28 6e70 2e6c 6f67 2873 656c 662e  sum(np.log(self.
-000174d0: 6461 7461 2e65 7272 3229 290a 0a20 2020  data.err2))..   
-000174e0: 2020 2020 2020 2020 2023 2070 726f 7669           # provi
-000174f0: 6465 206d 6f64 656c 2076 616c 7565 7320  de model values 
-00017500: 746f 2064 6174 6120 6f62 6a65 6374 0a20  to data object. 
-00017510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00017520: 6461 7461 2e6d 6f64 656c 5f76 616c 7565  data.model_value
-00017530: 7320 3d20 6d6f 6465 6c5f 7661 6c75 6573  s = model_values
-00017540: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00017550: 7475 726e 206e 6c4c 320a 0a20 2020 2023  turn nlL2..    #
-00017560: 0a20 2020 2023 202d 2d2d 2073 7065 6369  .    # --- speci
-00017570: 616c 2063 6f64 6520 666f 7220 6869 7374  al code for hist
-00017580: 6f67 7261 6d20 4669 740a 2020 2020 230a  ogram Fit.    #.
-00017590: 0a20 2020 2064 6566 2073 6574 5f68 4f70  .    def set_hOp
-000175a0: 7469 6f6e 7328 0a20 2020 2020 2020 2073  tions(.        s
-000175b0: 656c 662c 2072 756e 5f6d 696e 6f73 3d4e  elf, run_minos=N
-000175c0: 6f6e 652c 2075 7365 5f47 6175 7373 4170  one, use_GaussAp
-000175d0: 7072 6f78 3d4e 6f6e 652c 2066 6974 5f64  prox=None, fit_d
-000175e0: 656e 7369 7479 3d4e 6f6e 652c 2071 7569  ensity=None, qui
-000175f0: 6574 3d4e 6f6e 650a 2020 2020 293a 0a20  et=None.    ):. 
-00017600: 2020 2020 2020 2022 2222 4465 6669 6e65         """Define
-00017610: 206d 6e46 6974 206f 7074 696f 6e73 0a0a   mnFit options..
-00017620: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00017630: 2020 2020 2020 202d 2072 756e 206d 696e         - run min
-00017640: 6f73 2065 6c73 6520 646f 6e2a 7420 7275  os else don*t ru
-00017650: 6e20 6d69 6e6f 730a 2020 2020 2020 2020  n minos.        
-00017660: 202d 2075 7365 2047 6175 7373 6961 6e20   - use Gaussian 
-00017670: 4170 7072 6f78 696d 6174 696f 6e20 6f66  Approximation of
-00017680: 2050 6f69 7373 6f6e 2064 6973 7472 6962   Poisson distrib
-00017690: 7574 696f 6e0a 2020 2020 2020 2020 202d  ution.         -
-000176a0: 2064 6f6e 2a74 2070 726f 7669 6465 2070   don*t provide p
-000176b0: 7269 6e74 6f75 7420 656c 7365 2076 6572  rintout else ver
-000176c0: 626f 7365 2070 7269 6e74 6f75 740a 2020  bose printout.  
-000176d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000176e0: 2020 6966 2072 756e 5f6d 696e 6f73 2069    if run_minos i
-000176f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00017700: 2020 2020 2020 2020 7365 6c66 2e72 756e          self.run
-00017710: 5f6d 696e 6f73 203d 2072 756e 5f6d 696e  _minos = run_min
-00017720: 6f73 0a20 2020 2020 2020 2020 2020 2073  os.            s
-00017730: 656c 662e 6f70 7469 6f6e 735b 2272 756e  elf.options["run
-00017740: 5f6d 696e 6f73 225d 5b30 5d20 3d20 696e  _minos"][0] = in
-00017750: 7428 7275 6e5f 6d69 6e6f 7329 0a20 2020  t(run_minos).   
-00017760: 2020 2020 2069 6620 7573 655f 4761 7573       if use_Gaus
-00017770: 7341 7070 726f 7820 6973 206e 6f74 204e  sApprox is not N
-00017780: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00017790: 2073 656c 662e 7573 655f 4761 7573 7341   self.use_GaussA
-000177a0: 7070 726f 7820 3d20 7573 655f 4761 7573  pprox = use_Gaus
-000177b0: 7341 7070 726f 780a 2020 2020 2020 2020  sApprox.        
-000177c0: 2020 2020 7365 6c66 2e6f 7074 696f 6e73      self.options
-000177d0: 5b22 7573 655f 4761 7573 7341 7070 726f  ["use_GaussAppro
-000177e0: 7822 5d5b 305d 203d 2069 6e74 2875 7365  x"][0] = int(use
-000177f0: 5f47 6175 7373 4170 7072 6f78 290a 2020  _GaussApprox).  
-00017800: 2020 2020 2020 6966 2066 6974 5f64 656e        if fit_den
-00017810: 7369 7479 2069 7320 6e6f 7420 4e6f 6e65  sity is not None
-00017820: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00017830: 6c66 2e66 6974 5f64 656e 7369 7479 203d  lf.fit_density =
-00017840: 2066 6974 5f64 656e 7369 7479 0a20 2020   fit_density.   
-00017850: 2020 2020 2020 2020 2073 656c 662e 6f70           self.op
-00017860: 7469 6f6e 735b 2266 6974 5f64 656e 7369  tions["fit_densi
-00017870: 7479 225d 5b30 5d20 3d20 696e 7428 6669  ty"][0] = int(fi
-00017880: 745f 6465 6e73 6974 7929 0a20 2020 2020  t_density).     
-00017890: 2020 2069 6620 7175 6965 7420 6973 206e     if quiet is n
-000178a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000178b0: 2020 2020 2073 656c 662e 7175 6965 7420       self.quiet 
-000178c0: 3d20 7175 6965 740a 0a20 2020 2064 6566  = quiet..    def
-000178d0: 2069 6e69 745f 6844 6174 6128 7365 6c66   init_hData(self
-000178e0: 2c20 6269 6e5f 636f 6e74 656e 7473 2c20  , bin_contents, 
-000178f0: 6269 6e5f 6564 6765 732c 2044 656c 7461  bin_edges, Delta
-00017900: 4d75 3d4e 6f6e 6529 3a0a 2020 2020 2020  Mu=None):.      
-00017910: 2020 2222 220a 2020 2020 2020 2020 696e    """.        in
-00017920: 6974 6961 6c69 7a65 2068 6973 746f 6772  itialize histogr
-00017930: 616d 2064 6174 6120 6f62 6a65 6374 0a0a  am data object..
-00017940: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00017950: 2020 2020 2020 2d20 6269 6e5f 636f 6e74        - bin_cont
-00017960: 656e 7473 3a20 6172 7261 7920 6f66 2066  ents: array of f
-00017970: 6c6f 6174 730a 2020 2020 2020 2020 2d20  loats.        - 
-00017980: 6269 6e5f 6564 6765 733a 2061 7272 6179  bin_edges: array
-00017990: 206f 6620 6c65 6e67 7468 206c 656e 2862   of length len(b
-000179a0: 696e 5f63 6f6e 7465 6e74 7329 2a31 0a20  in_contents)*1. 
-000179b0: 2020 2020 2020 202d 2044 656c 7461 4d75         - DeltaMu
-000179c0: 3a20 7368 6966 7420 696e 206d 6561 6e20  : shift in mean 
-000179d0: 2844 656c 7461 206d 7529 2076 6572 7375  (Delta mu) versu
-000179e0: 7320 6c61 6d62 6461 0a20 2020 2020 2020  s lambda.       
-000179f0: 206f 6620 506f 6973 736f 6e20 6469 7374   of Poisson dist
-00017a00: 7269 6275 7469 6f6e 0a20 2020 2020 2020  ribution.       
-00017a10: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
-00017a20: 6372 6561 7465 2064 6174 6120 6f62 6a65  create data obje
-00017a30: 6374 2061 6e64 2070 6173 7320 616c 6c20  ct and pass all 
-00017a40: 696e 7075 7420 6172 6775 6d65 6e74 730a  input arguments.
-00017a50: 2020 2020 2020 2020 7365 6c66 2e68 4461          self.hDa
-00017a60: 7461 203d 2073 656c 662e 6869 7374 4461  ta = self.histDa
-00017a70: 7461 436f 6e74 6169 6e65 7228 0a20 2020  taContainer(.   
-00017a80: 2020 2020 2020 2020 2073 656c 662c 2062           self, b
-00017a90: 696e 5f63 6f6e 7465 6e74 732c 2062 696e  in_contents, bin
-00017aa0: 5f65 6467 6573 2c20 4465 6c74 614d 752c  _edges, DeltaMu,
-00017ab0: 2071 7569 6574 3d73 656c 662e 7175 6965   quiet=self.quie
-00017ac0: 740a 2020 2020 2020 2020 290a 2020 2020  t.        ).    
-00017ad0: 2020 2020 7365 6c66 2e64 6174 6120 3d20      self.data = 
-00017ae0: 7365 6c66 2e68 4461 7461 0a0a 2020 2020  self.hData..    
-00017af0: 6465 6620 696e 6974 5f68 4669 7428 0a20  def init_hFit(. 
-00017b00: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00017b10: 2020 2020 206d 6f64 656c 2c0a 2020 2020       model,.    
-00017b20: 2020 2020 6d6f 6465 6c5f 6b77 6172 6773      model_kwargs
-00017b30: 3d4e 6f6e 652c 0a20 2020 2020 2020 2070  =None,.        p
-00017b40: 303d 4e6f 6e65 2c0a 2020 2020 2020 2020  0=None,.        
-00017b50: 6470 303d 4e6f 6e65 2c0a 2020 2020 2020  dp0=None,.      
-00017b60: 2020 636f 6e73 7472 6169 6e74 733d 4e6f    constraints=No
-00017b70: 6e65 2c0a 2020 2020 2020 2020 6669 7850  ne,.        fixP
-00017b80: 6172 733d 4e6f 6e65 2c0a 2020 2020 2020  ars=None,.      
-00017b90: 2020 6c69 6d69 7473 3d4e 6f6e 652c 0a20    limits=None,. 
-00017ba0: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
-00017bb0: 2269 6e69 7469 616c 697a 6520 6669 7420  "initialize fit 
-00017bc0: 6f62 6a65 6374 0a0a 2020 2020 2020 2020  object..        
-00017bd0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00017be0: 2d20 6d6f 6465 6c3a 206d 6f64 656c 2064  - model: model d
-00017bf0: 656e 7369 7479 2066 756e 6374 696f 6e20  ensity function 
-00017c00: 6628 783b 205c 2a70 6172 290a 2020 2020  f(x; \*par).    
-00017c10: 2020 2020 2020 2d20 6d6f 6465 6c5f 6b77        - model_kw
-00017c20: 6172 6773 3a20 6f70 7469 6f6e 616c 2c20  args: optional, 
-00017c30: 6669 7420 7061 7261 6d65 7465 7273 2069  fit parameters i
-00017c40: 6620 6e6f 7420 6672 6f6d 206d 6f64 656c  f not from model
-00017c50: 2073 6967 6e61 7475 7265 0a20 2020 2020   signature.     
-00017c60: 2020 2020 202d 2070 303a 206e 702d 6172       - p0: np-ar
-00017c70: 7261 7920 6f66 2066 6c6f 6174 732c 2069  ray of floats, i
-00017c80: 6e69 7469 616c 2070 6172 616d 6574 6572  nitial parameter
-00017c90: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-00017ca0: 2020 2d20 6470 303a 2061 7272 6179 2d6c    - dp0: array-l
-00017cb0: 696b 652c 2069 6e69 7469 616c 2067 7565  ike, initial gue
-00017cc0: 7373 206f 6620 7061 7261 6d65 7465 7220  ss of parameter 
-00017cd0: 756e 6365 7274 6169 6e74 6965 7320 286f  uncertainties (o
-00017ce0: 7074 696f 6e61 6c29 0a20 2020 2020 2020  ptional).       
-00017cf0: 2020 202d 2063 6f6e 7374 7261 696e 7473     - constraints
-00017d00: 3a20 286e 6573 7465 6429 206c 6973 7428  : (nested) list(
-00017d10: 7329 3a20 5b70 6172 616d 6574 6572 206e  s): [parameter n
-00017d20: 616d 652c 2076 616c 7565 2c20 756e 6365  ame, value, unce
-00017d30: 7274 6169 6e74 795d 0a20 2020 2020 2020  rtainty].       
-00017d40: 2020 2020 206f 7220 5b70 6172 616d 6574       or [paramet
-00017d50: 6572 2069 6e64 6578 2c20 7661 6c75 652c  er index, value,
-00017d60: 2075 6e63 6572 7461 696e 7479 5d0a 2020   uncertainty].  
-00017d70: 2020 2020 2020 2020 2d20 6669 7820 7061          - fix pa
-00017d80: 7261 6d65 7465 7228 7329 2069 6e20 6669  rameter(s) in fi
-00017d90: 743a 206c 6973 7420 6f66 2070 6172 616d  t: list of param
-00017da0: 6574 6572 206e 616d 6573 206f 7220 696e  eter names or in
-00017db0: 6469 6365 730a 2020 2020 2020 2020 2020  dices.          
-00017dc0: 2d20 6c69 6d69 7473 3a20 286e 6573 7465  - limits: (neste
-00017dd0: 6429 206c 6973 7428 7329 3a20 5b70 6172  d) list(s): [par
-00017de0: 616d 6574 6572 206e 616d 652c 206d 696e  ameter name, min
-00017df0: 2c20 6d61 785d 0a20 2020 2020 2020 2020  , max].         
-00017e00: 2020 206f 7220 5b70 6172 616d 6574 6572     or [parameter
-00017e10: 2069 6e64 6578 2c20 6d69 6e2c 206d 6178   index, min, max
-00017e20: 5d0a 2020 2020 2020 2020 2222 220a 0a20  ].        """.. 
-00017e30: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
-00017e40: 4461 7461 2069 7320 4e6f 6e65 3a0a 2020  Data is None:.  
-00017e50: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00017e60: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-00017e70: 2020 2020 2020 2020 2020 2020 2220 2121              " !!
-00017e80: 2120 6d6e 4669 742e 696e 6974 5f68 4669  ! mnFit.init_hFi
-00017e90: 743a 206e 6f20 6461 7461 206f 626a 6563  t: no data objec
-00017ea0: 7420 6465 6669 6e65 6420 2d20 6361 6c6c  t defined - call
-00017eb0: 2069 6e69 745f 6461 7461 2829 220a 2020   init_data()".  
-00017ec0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
-00017ed0: 2020 2020 2023 2067 6574 2070 6172 616d       # get param
-00017ee0: 6574 6572 7320 6f66 206d 6f64 656c 2066  eters of model f
-00017ef0: 756e 6374 696f 6e20 746f 2073 6574 2073  unction to set s
-00017f00: 7461 7274 2076 616c 7565 7320 666f 7220  tart values for 
-00017f10: 6669 740a 2020 2020 2020 2020 6966 206d  fit.        if m
-00017f20: 6f64 656c 5f6b 7761 7267 7320 6973 204e  odel_kwargs is N
-00017f30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00017f40: 2061 7267 732c 206d 6f64 656c 5f6b 7761   args, model_kwa
-00017f50: 7267 7320 3d20 6765 745f 6675 6e63 7469  rgs = get_functi
-00017f60: 6f6e 5369 676e 6174 7572 6528 6d6f 6465  onSignature(mode
-00017f70: 6c29 0a0a 2020 2020 2020 2020 7061 7220  l)..        par 
-00017f80: 3d20 286d 6f64 656c 5f6b 7761 7267 732c  = (model_kwargs,
-00017f90: 2070 302c 2064 7030 2c20 636f 6e73 7472   p0, dp0, constr
-00017fa0: 6169 6e74 732c 2066 6978 5061 7273 2c20  aints, fixPars, 
-00017fb0: 6c69 6d69 7473 290a 2020 2020 2020 2020  limits).        
-00017fc0: 7365 6c66 2e5f 7365 7475 7046 6974 5061  self._setupFitPa
-00017fd0: 7261 6d65 7465 7273 282a 7061 7229 0a0a  rameters(*par)..
-00017fe0: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-00017ff0: 2063 6f73 7420 6675 6e63 7469 6f6e 0a20   cost function. 
-00018000: 2020 2020 2020 2073 656c 662e 636f 7374         self.cost
-00018010: 6620 3d20 7365 6c66 2e68 436f 7374 280a  f = self.hCost(.
-00018020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018030: 2c20 6d6f 6465 6c2c 2075 7365 5f47 6175  , model, use_Gau
-00018040: 7373 4170 7072 6f78 3d73 656c 662e 7573  ssApprox=self.us
-00018050: 655f 4761 7573 7341 7070 726f 782c 2064  e_GaussApprox, d
-00018060: 656e 7369 7479 3d73 656c 662e 6669 745f  ensity=self.fit_
-00018070: 6465 6e73 6974 790a 2020 2020 2020 2020  density.        
-00018080: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00018090: 7365 7475 704d 696e 7569 7428 6d6f 6465  setupMinuit(mode
-000180a0: 6c5f 6b77 6172 6773 290a 0a20 2020 2063  l_kwargs)..    c
-000180b0: 6c61 7373 2068 6973 7444 6174 6143 6f6e  lass histDataCon
-000180c0: 7461 696e 6572 3a0a 2020 2020 2020 2020  tainer:.        
-000180d0: 2222 220a 2020 2020 2020 2020 436f 6e74  """.        Cont
-000180e0: 6169 6e65 7220 666f 7220 4869 7374 6f67  ainer for Histog
-000180f0: 7261 6d20 6461 7461 0a0a 2020 2020 2020  ram data..      
-00018100: 2020 4461 7461 204d 656d 6265 7273 3a0a    Data Members:.
-00018110: 0a20 2020 2020 2020 202d 2063 6f6e 7465  .        - conte
-00018120: 6e74 732c 2061 7272 6179 206f 6620 666c  nts, array of fl
-00018130: 6f61 7473 3a20 6269 6e20 636f 6e74 656e  oats: bin conten
-00018140: 7473 0a20 2020 2020 2020 202d 2065 6467  ts.        - edg
-00018150: 6573 2c20 6172 7261 7920 6f66 2066 6c6f  es, array of flo
-00018160: 6174 733a 2062 696e 2065 6467 6573 2028  ats: bin edges (
-00018170: 6e62 696e 732b 3120 7661 6c75 6573 290a  nbins+1 values).
-00018180: 0a20 2020 2020 2020 2063 616c 6375 6c61  .        calcula
-00018190: 7465 6420 6672 6f6d 2069 6e70 7574 3a0a  ted from input:.
-000181a0: 0a20 2020 2020 2020 202d 206e 6269 6e73  .        - nbins
-000181b0: 3a20 6e75 6d62 6572 206f 6620 6269 6e73  : number of bins
-000181c0: 0a20 2020 2020 2020 202d 206c 6566 7473  .        - lefts
-000181d0: 3a20 6c65 6674 2065 6467 6573 0a20 2020  : left edges.   
-000181e0: 2020 2020 202d 2072 6967 6874 733a 2072       - rights: r
-000181f0: 6967 6874 2065 6467 6573 0a20 2020 2020  ight edges.     
-00018200: 2020 202d 2063 656e 7465 7273 3a20 6269     - centers: bi
-00018210: 6e20 6365 6e74 6572 730a 2020 2020 2020  n centers.      
-00018220: 2020 2d20 7769 6474 6873 3a20 6269 6e20    - widths: bin 
-00018230: 7769 6474 6873 0a20 2020 2020 2020 202d  widths.        -
-00018240: 204e 746f 743a 2074 6f74 616c 206e 756d   Ntot: total num
-00018250: 6265 7220 6f66 2065 6e74 7269 6573 2c20  ber of entries, 
-00018260: 7573 6564 2074 6f20 6e6f 726d 616c 697a  used to normaliz
-00018270: 6520 7072 6f62 6174 696c 6974 7920 6465  e probatility de
-00018280: 6e73 6974 790a 0a20 2020 2020 2020 2061  nsity..        a
-00018290: 7661 696c 6162 6c65 2061 6674 6572 2063  vailable after c
-000182a0: 6f6d 706c 6574 696f 6e20 6f66 2066 6974  ompletion of fit
-000182b0: 3a0a 0a20 2020 2020 2020 202d 206d 6f64  :..        - mod
-000182c0: 656c 5f76 616c 7565 733a 2062 696e 2063  el_values: bin c
-000182d0: 6f6e 7465 6e74 7320 6672 6f6d 2062 6573  ontents from bes
-000182e0: 742d 6669 7420 6d6f 6465 6c0a 0a20 2020  t-fit model..   
-000182f0: 2020 2020 204d 6574 686f 6473 3a0a 0a20       Methods:.. 
-00018300: 2020 2020 2020 202d 2070 6c6f 7428 293a         - plot():
-00018310: 2072 6574 7572 6e20 6669 6775 7265 2077   return figure w
-00018320: 6974 6820 6869 7374 6f67 7261 6d20 6f66  ith histogram of
-00018330: 2064 6174 6120 616e 6420 756e 6365 7274   data and uncert
-00018340: 6169 6e74 6965 730a 2020 2020 2020 2020  ainties.        
-00018350: 2222 220a 0a20 2020 2020 2020 2064 6566  """..        def
-00018360: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00018370: 6f75 7465 722c 2062 696e 5f63 6f6e 7465  outer, bin_conte
-00018380: 6e74 732c 2062 696e 5f65 6467 6573 2c20  nts, bin_edges, 
-00018390: 4465 6c74 614d 753d 4e6f 6e65 2c20 7175  DeltaMu=None, qu
-000183a0: 6965 743d 5472 7565 293a 0a20 2020 2020  iet=True):.     
-000183b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000183c0: 2020 2020 2020 2069 6e69 7469 616c 697a         initializ
-000183d0: 6520 6869 7374 6f67 7261 6d20 4461 7461  e histogram Data
-000183e0: 0a0a 2020 2020 2020 2020 2020 2020 4172  ..            Ar
-000183f0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00018400: 2d20 6269 6e5f 636f 6e74 656e 7473 3a20  - bin_contents: 
-00018410: 6172 7261 7920 6f66 2066 6c6f 6174 730a  array of floats.
-00018420: 2020 2020 2020 2020 2020 2020 2d20 6269              - bi
-00018430: 6e5f 6564 6765 733a 2061 7272 6179 206f  n_edges: array o
-00018440: 6620 6c65 6e67 7468 206c 656e 2862 696e  f length len(bin
-00018450: 5f63 6f6e 7465 6e74 7329 2a31 0a20 2020  _contents)*1.   
-00018460: 2020 2020 2020 2020 202d 2044 656c 7461           - Delta
-00018470: 4d75 3a20 6172 7261 7920 6f66 2066 6c6f  Mu: array of flo
-00018480: 6174 732c 2073 6869 6674 206f 6620 6d65  ats, shift of me
-00018490: 616e 206d 7520 7673 2e0a 2020 2020 2020  an mu vs..      
-000184a0: 2020 2020 2020 2020 2020 6c61 6d62 6461            lambda
-000184b0: 206f 6620 506f 6973 736f 6e20 6469 7374   of Poisson dist
-000184c0: 7269 6275 7469 6f6e 2c20 4465 6c74 614d  ribution, DeltaM
-000184d0: 7520 3d20 6d75 2d6c 616d 6264 610a 2020  u = mu-lambda.  
-000184e0: 2020 2020 2020 2020 2020 2d20 7175 6965            - quie
-000184f0: 743a 2062 6f6f 6c65 616e 2c20 636f 6e74  t: boolean, cont
-00018500: 726f 6c73 2070 7269 6e74 6564 206f 7574  rols printed out
-00018510: 7075 740a 0a20 2020 2020 2020 2020 2020  put..           
-00018520: 2022 2222 0a0a 2020 2020 2020 2020 2020   """..          
-00018530: 2020 7365 6c66 2e6f 7574 6572 203d 206f    self.outer = o
-00018540: 7574 6572 0a20 2020 2020 2020 2020 2020  uter.           
-00018550: 2073 656c 662e 636f 6e74 656e 7473 203d   self.contents =
-00018560: 2062 696e 5f63 6f6e 7465 6e74 730a 2020   bin_contents.  
-00018570: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018580: 6269 6e73 203d 206c 656e 2862 696e 5f63  bins = len(bin_c
-00018590: 6f6e 7465 6e74 7329 0a20 2020 2020 2020  ontents).       
-000185a0: 2020 2020 2073 656c 662e 646c 656e 6774       self.dlengt
-000185b0: 6820 3d20 7365 6c66 2e6e 6269 6e73 0a20  h = self.nbins. 
-000185c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000185d0: 4e74 6f74 203d 206e 702e 7375 6d28 6269  Ntot = np.sum(bi
-000185e0: 6e5f 636f 6e74 656e 7473 290a 2020 2020  n_contents).    
-000185f0: 2020 2020 2020 2020 7365 6c66 2e65 6467          self.edg
-00018600: 6573 203d 2062 696e 5f65 6467 6573 0a20  es = bin_edges. 
-00018610: 2020 2020 2020 2020 2020 2069 6620 4465             if De
-00018620: 6c74 614d 7520 6973 204e 6f6e 653a 0a20  ltaMu is None:. 
-00018630: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018640: 656c 662e 4465 6c74 614d 7520 3d20 6e70  elf.DeltaMu = np
-00018650: 2e7a 6572 6f73 286c 656e 2862 696e 5f63  .zeros(len(bin_c
-00018660: 6f6e 7465 6e74 7329 290a 2020 2020 2020  ontents)).      
-00018670: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00018680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018690: 2e44 656c 7461 203d 2044 656c 7461 4d75  .Delta = DeltaMu
-000186a0: 0a20 2020 2020 2020 2020 2020 2023 0a20  .            #. 
-000186b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000186c0: 6c65 6674 7320 3d20 7365 6c66 2e65 6467  lefts = self.edg
-000186d0: 6573 5b3a 2d31 5d0a 2020 2020 2020 2020  es[:-1].        
-000186e0: 2020 2020 7365 6c66 2e72 6967 6874 7320      self.rights 
-000186f0: 3d20 7365 6c66 2e65 6467 6573 5b31 3a5d  = self.edges[1:]
-00018700: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00018710: 662e 6365 6e74 6572 7320 3d20 2873 656c  f.centers = (sel
-00018720: 662e 7269 6768 7473 202b 2073 656c 662e  f.rights + self.
-00018730: 6c65 6674 7329 202f 2032 2e30 0a20 2020  lefts) / 2.0.   
-00018740: 2020 2020 2020 2020 2073 656c 662e 7769           self.wi
-00018750: 6474 6873 203d 2073 656c 662e 7269 6768  dths = self.righ
-00018760: 7473 202d 2073 656c 662e 6c65 6674 730a  ts - self.lefts.
-00018770: 2020 2020 2020 2020 2020 2020 2320 666c              # fl
-00018780: 6167 2074 6f20 636f 6e74 726f 6c20 6669  ag to control fi
-00018790: 6e61 6c20 6163 7469 6f6e 7320 696e 2063  nal actions in c
-000187a0: 6f73 7420 6675 6e63 7469 6f6e 0a20 2020  ost function.   
-000187b0: 2020 2020 2020 2020 2073 656c 662e 6669           self.fi
-000187c0: 6e61 6c5f 6361 6c6c 203d 2046 616c 7365  nal_call = False
-000187d0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000187e0: 662e 6d6f 6465 6c5f 7661 6c75 6573 203d  f.model_values =
-000187f0: 204e 6f6e 650a 0a20 2020 2020 2020 2064   None..        d
-00018800: 6566 2070 6c6f 7428 0a20 2020 2020 2020  ef plot(.       
-00018810: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-00018820: 2020 2020 2020 206e 756d 3d22 6869 7374         num="hist
-00018830: 4461 7461 2061 6e64 204d 6f64 656c 222c  Data and Model",
-00018840: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
-00018850: 7369 7a65 3d28 372e 352c 2036 2e35 292c  size=(7.5, 6.5),
-00018860: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00018870: 615f 6c61 6265 6c3d 2242 696e 6e65 6420  a_label="Binned 
-00018880: 6461 7461 222c 0a20 2020 2020 2020 2020  data",.         
-00018890: 2020 2070 6c6f 745f 7265 7369 6475 616c     plot_residual
-000188a0: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-000188b0: 293a 0a20 2020 2020 2020 2020 2020 2022  ):.            "
-000188c0: 2222 7265 7475 726e 2066 6967 7572 6520  ""return figure 
-000188d0: 7769 7468 2068 6973 746f 6772 616d 2064  with histogram d
-000188e0: 6174 6120 616e 6420 756e 6365 7274 6169  ata and uncertai
-000188f0: 6e74 6965 7322 2222 0a0a 2020 2020 2020  nties"""..      
-00018900: 2020 2020 2020 7720 3d20 7365 6c66 2e65        w = self.e
-00018910: 6467 6573 5b31 3a5d 202d 2073 656c 662e  dges[1:] - self.
-00018920: 6564 6765 735b 3a2d 315d 0a20 2020 2020  edges[:-1].     
-00018930: 2020 2020 2020 2066 6967 203d 2070 6c74         fig = plt
-00018940: 2e66 6967 7572 6528 6e75 6d3d 6e75 6d2c  .figure(num=num,
-00018950: 2066 6967 7369 7a65 3d66 6967 7369 7a65   figsize=figsize
-00018960: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00018970: 2073 656c 662e 6d6f 6465 6c5f 7661 6c75   self.model_valu
-00018980: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-00018990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189a0: 6966 2070 6c6f 745f 7265 7369 6475 616c  if plot_residual
-000189b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000189c0: 2020 2020 2020 6d63 6f6e 7473 203d 206e        mconts = n
-000189d0: 702e 7a65 726f 7328 7365 6c66 2e6e 6269  p.zeros(self.nbi
-000189e0: 6e73 290a 2020 2020 2020 2020 2020 2020  ns).            
-000189f0: 2020 2020 2020 2020 6263 6f6e 7473 203d          bconts =
-00018a00: 2073 656c 662e 636f 6e74 656e 7473 202d   self.contents -
-00018a10: 2073 656c 662e 6d6f 6465 6c5f 7661 6c75   self.model_valu
-00018a20: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
-00018a30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00018a40: 2020 2020 2020 2020 2020 2020 206d 636f               mco
-00018a50: 6e74 7320 3d20 7365 6c66 2e6d 6f64 656c  nts = self.model
-00018a60: 5f76 616c 7565 730a 2020 2020 2020 2020  _values.        
-00018a70: 2020 2020 2020 2020 2020 2020 6263 6f6e              bcon
-00018a80: 7473 203d 2073 656c 662e 636f 6e74 656e  ts = self.conten
-00018a90: 7473 0a20 2020 2020 2020 2020 2020 2070  ts.            p
-00018aa0: 6c74 2e62 6172 280a 2020 2020 2020 2020  lt.bar(.        
-00018ab0: 2020 2020 2020 2020 7365 6c66 2e63 656e          self.cen
-00018ac0: 7465 7273 2c0a 2020 2020 2020 2020 2020  ters,.          
-00018ad0: 2020 2020 2020 6263 6f6e 7473 2c0a 2020        bconts,.  
-00018ae0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00018af0: 6967 6e3d 2263 656e 7465 7222 2c0a 2020  ign="center",.  
-00018b00: 2020 2020 2020 2020 2020 2020 2020 7769                wi
-00018b10: 6474 683d 772c 0a20 2020 2020 2020 2020  dth=w,.         
-00018b20: 2020 2020 2020 2066 6163 6563 6f6c 6f72         facecolor
-00018b30: 3d22 6361 6465 7462 6c75 6522 2c0a 2020  ="cadetblue",.  
-00018b40: 2020 2020 2020 2020 2020 2020 2020 6564                ed
-00018b50: 6765 636f 6c6f 723d 2264 6172 6b62 6c75  gecolor="darkblu
-00018b60: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00018b70: 2020 2020 616c 7068 613d 302e 3636 2c0a      alpha=0.66,.
-00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b90: 6c61 6265 6c3d 6461 7461 5f6c 6162 656c  label=data_label
-00018ba0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00018bb0: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00018bc0: 6574 2061 6e64 2070 6c6f 7420 6572 726f  et and plot erro
-00018bd0: 7220 6261 7273 0a20 2020 2020 2020 2020  r bars.         
-00018be0: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
-00018bf0: 5f76 616c 7565 7320 6973 206e 6f74 204e  _values is not N
-00018c00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00018c10: 2020 2020 2023 2062 6573 742d 6669 7420       # best-fit 
-00018c20: 6d6f 6465 6c20 7661 6c75 6573 2061 7661  model values ava
-00018c30: 6961 626c 650a 2020 2020 2020 2020 2020  iable.          
-00018c40: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00018c50: 662e 6f75 7465 722e 7573 655f 4761 7573  f.outer.use_Gaus
-00018c60: 7341 7070 726f 783a 0a20 2020 2020 2020  sApprox:.       
-00018c70: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00018c80: 686f 7720 506f 6973 736f 6e20 436f 6e66  how Poisson Conf
-00018c90: 6964 656e 6365 2049 6e74 6572 7661 6c73  idence Intervals
-00018ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018cb0: 2020 2020 2065 7020 3d20 5b5d 0a20 2020       ep = [].   
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cd0: 2065 6d20 3d20 5b5d 0a20 2020 2020 2020   em = [].       
-00018ce0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00018cf0: 2069 2069 6e20 7261 6e67 6528 7365 6c66   i in range(self
-00018d00: 2e6e 6269 6e73 293a 0a20 2020 2020 2020  .nbins):.       
+00012a80: 2020 2020 2020 206e 6c4c 3220 2b3d 2032         nlL2 += 2
+00012a90: 2e30 202a 206e 702e 7375 6d28 6e70 2e6c  .0 * np.sum(np.l
+00012aa0: 6f67 286e 702e 6469 6167 6f6e 616c 284c  og(np.diagonal(L
+00012ab0: 2929 290a 0a20 2020 2020 2020 2020 2020  )))..           
+00012ac0: 2065 6c73 653a 2020 2320 6661 7374 2063   else:  # fast c
+00012ad0: 616c 6375 6c61 7469 6f6e 2066 6f72 2073  alculation for s
+00012ae0: 696d 706c 6520 6572 726f 7273 0a20 2020  imple errors.   
+00012af0: 2020 2020 2020 2020 2020 2020 2023 2063               # c
+00012b00: 6865 636b 2069 6620 6572 726f 7273 206e  heck if errors n
+00012b10: 6565 6473 2072 6563 616c 6375 6c61 7469  eeds recalculati
+00012b20: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00012b30: 2020 2069 6620 7365 6c66 2e64 6174 612e     if self.data.
+00012b40: 6e65 6564 735f 6479 6e61 6d69 6345 7272  needs_dynamicErr
+00012b50: 6f72 733a 0a20 2020 2020 2020 2020 2020  ors:.           
+00012b60: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
+00012b70: 7461 2e5f 7265 6275 696c 645f 4572 7232  ta._rebuild_Err2
+00012b80: 2870 6172 290a 2020 2020 2020 2020 2020  (par).          
+00012b90: 2020 2020 2020 2020 2020 6e6c 4c32 202b            nlL2 +
+00012ba0: 3d20 6e70 2e73 756d 285f 7220 2a20 5f72  = np.sum(_r * _r
+00012bb0: 202f 2073 656c 662e 6461 7461 2e65 7272   / self.data.err
+00012bc0: 3229 0a20 2020 2020 2020 2020 2020 2020  2).             
+00012bd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00012be0: 2020 2020 2020 2020 2020 2020 206e 6c4c               nlL
+00012bf0: 3220 2b3d 206e 702e 7375 6d28 5f72 202a  2 += np.sum(_r *
+00012c00: 205f 7220 2a20 7365 6c66 2e64 6174 612e   _r * self.data.
+00012c10: 6945 7272 3229 0a0a 2020 2020 2020 2020  iErr2)..        
+00012c20: 2020 2020 2020 2020 2320 7468 6973 2069          # this i
+00012c30: 7320 6964 656e 7469 6361 6c20 746f 2063  s identical to c
+00012c40: 6c61 7373 6963 616c 2043 6869 320a 2020  lassical Chi2.  
+00012c50: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00012c60: 6c66 2e67 6f66 203d 206e 6c4c 320a 0a20  lf.gof = nlL2.. 
+00012c70: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00012c80: 2061 6464 2070 6172 616d 6574 6572 2d64   add parameter-d
+00012c90: 6570 656e 6465 6e74 206e 6f72 6d61 6c69  ependent normali
+00012ca0: 7a61 7469 6f6e 2074 6572 6d20 6966 206e  zation term if n
+00012cb0: 6565 6465 6420 616e 6420 7761 6e74 6564  eeded and wanted
+00012cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012cd0: 2069 6620 7365 6c66 2e64 6174 612e 6e65   if self.data.ne
+00012ce0: 6564 735f 6479 6e61 6d69 6345 7272 6f72  eds_dynamicError
+00012cf0: 7320 616e 6420 7365 6c66 2e75 7365 5f6e  s and self.use_n
+00012d00: 6567 326c 6f67 4c3a 0a20 2020 2020 2020  eg2logL:.       
+00012d10: 2020 2020 2020 2020 2020 2020 206e 6c4c               nlL
+00012d20: 3220 2b3d 206e 702e 7375 6d28 6e70 2e6c  2 += np.sum(np.l
+00012d30: 6f67 2873 656c 662e 6461 7461 2e65 7272  og(self.data.err
+00012d40: 3229 290a 0a20 2020 2020 2020 2020 2020  2))..           
+00012d50: 2023 2070 726f 7669 6465 206d 6f64 656c   # provide model
+00012d60: 2076 616c 7565 7320 746f 2064 6174 6120   values to data 
+00012d70: 6f62 6a65 6374 0a20 2020 2020 2020 2020  object.         
+00012d80: 2020 2073 656c 662e 6461 7461 2e6d 6f64     self.data.mod
+00012d90: 656c 5f76 616c 7565 7320 3d20 6d6f 6465  el_values = mode
+00012da0: 6c5f 7661 6c75 6573 0a0a 2020 2020 2020  l_values..      
+00012db0: 2020 2020 2020 7265 7475 726e 206e 6c4c        return nlL
+00012dc0: 320a 0a20 2020 2023 202d 2d2d 2065 6e64  2..    # --- end
+00012dd0: 2064 6566 696e 6974 696f 6e20 6f66 2063   definition of c
+00012de0: 6c61 7373 2078 4c53 7143 6f73 7420 2d2d  lass xLSqCost --
+00012df0: 2d2d 0a0a 2020 2020 230a 2020 2020 2320  --..    #.    # 
+00012e00: 2d2d 2d20 7370 6563 6961 6c20 636f 6465  --- special code
+00012e10: 2066 6f72 2069 6e64 6578 6564 2046 6974   for indexed Fit
+00012e20: 2028 7846 6974 290a 2020 2020 230a 0a20   (xFit).    #.. 
+00012e30: 2020 2064 6566 2073 6574 5f78 4f70 7469     def set_xOpti
+00012e40: 6f6e 7328 0a20 2020 2020 2020 2073 656c  ons(.        sel
+00012e50: 662c 0a20 2020 2020 2020 2072 656c 6174  f,.        relat
+00012e60: 6976 655f 7265 6665 7273 5f74 6f5f 6d6f  ive_refers_to_mo
+00012e70: 6465 6c3d 4e6f 6e65 2c0a 2020 2020 2020  del=None,.      
+00012e80: 2020 7275 6e5f 6d69 6e6f 733d 4e6f 6e65    run_minos=None
+00012e90: 2c0a 2020 2020 2020 2020 7573 655f 6e65  ,.        use_ne
+00012ea0: 674c 6f67 4c3d 4e6f 6e65 2c0a 2020 2020  gLogL=None,.    
+00012eb0: 2020 2020 7175 6965 743d 4e6f 6e65 2c0a      quiet=None,.
+00012ec0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+00012ed0: 2222 4465 6669 6e65 206f 7074 696f 6e73  ""Define options
+00012ee0: 2066 6f72 2069 6e64 6578 6564 2066 6974   for indexed fit
+00012ef0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00012f00: 2020 2020 2020 2020 202d 2072 656c 2e20           - rel. 
+00012f10: 6572 726f 7273 2072 6566 6572 2074 6f20  errors refer to 
+00012f20: 6d6f 6465 6c20 656c 7365 2064 6174 610a  model else data.
+00012f30: 2020 2020 2020 2020 202d 2072 756e 206d           - run m
+00012f40: 696e 6f73 2065 6c73 6520 646f 6e2a 7420  inos else don*t 
+00012f50: 7275 6e20 6d69 6e6f 730a 2020 2020 2020  run minos.      
+00012f60: 2020 202d 2075 7365 2066 756c 6c20 6e65     - use full ne
+00012f70: 6732 6c6f 674c 0a20 2020 2020 2020 2020  g2logL.         
+00012f80: 2d20 646f 6e2a 7420 7072 6f76 6964 6520  - don*t provide 
+00012f90: 7072 696e 746f 7574 2065 6c73 6520 7665  printout else ve
+00012fa0: 7262 6f73 6520 7072 696e 746f 7574 0a20  rbose printout. 
+00012fb0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012fc0: 2020 2069 6620 7265 6c61 7469 7665 5f72     if relative_r
+00012fd0: 6566 6572 735f 746f 5f6d 6f64 656c 2069  efers_to_model i
+00012fe0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00012ff0: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+00013000: 4d6f 6465 6c20 3d20 7265 6c61 7469 7665  Model = relative
+00013010: 5f72 6566 6572 735f 746f 5f6d 6f64 656c  _refers_to_model
+00013020: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013030: 662e 6f70 7469 6f6e 735b 2272 6566 4d6f  f.options["refMo
+00013040: 6465 6c22 5d5b 305d 203d 2069 6e74 2872  del"][0] = int(r
+00013050: 656c 6174 6976 655f 7265 6665 7273 5f74  elative_refers_t
+00013060: 6f5f 6d6f 6465 6c29 0a20 2020 2020 2020  o_model).       
+00013070: 2069 6620 7275 6e5f 6d69 6e6f 7320 6973   if run_minos is
+00013080: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00013090: 2020 2020 2020 2073 656c 662e 7275 6e5f         self.run_
+000130a0: 6d69 6e6f 7320 3d20 7275 6e5f 6d69 6e6f  minos = run_mino
+000130b0: 730a 2020 2020 2020 2020 2020 2020 7365  s.            se
+000130c0: 6c66 2e6f 7074 696f 6e73 5b22 7275 6e5f  lf.options["run_
+000130d0: 6d69 6e6f 7322 5d5b 305d 203d 2069 6e74  minos"][0] = int
+000130e0: 2872 756e 5f6d 696e 6f73 290a 2020 2020  (run_minos).    
+000130f0: 2020 2020 6966 2075 7365 5f6e 6567 4c6f      if use_negLo
+00013100: 674c 2069 7320 6e6f 7420 4e6f 6e65 3a0a  gL is not None:.
+00013110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013120: 2e75 7365 5f6e 6567 4c6f 674c 203d 2075  .use_negLogL = u
+00013130: 7365 5f6e 6567 4c6f 674c 0a20 2020 2020  se_negLogL.     
+00013140: 2020 2020 2020 2073 656c 662e 6f70 7469         self.opti
+00013150: 6f6e 735b 2275 7365 5f6e 6567 4c6f 674c  ons["use_negLogL
+00013160: 225d 5b30 5d20 3d20 696e 7428 7573 655f  "][0] = int(use_
+00013170: 6e65 674c 6f67 4c29 0a20 2020 2020 2020  negLogL).       
+00013180: 2069 6620 7175 6965 7420 6973 206e 6f74   if quiet is not
+00013190: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000131a0: 2020 2073 656c 662e 7175 6965 7420 3d20     self.quiet = 
+000131b0: 7175 6965 740a 0a20 2020 2064 6566 2069  quiet..    def i
+000131c0: 6e69 745f 7844 6174 6128 7365 6c66 2c20  nit_xData(self, 
+000131d0: 782c 2065 3d4e 6f6e 652c 2065 7265 6c3d  x, e=None, erel=
+000131e0: 4e6f 6e65 2c20 6361 6273 3d4e 6f6e 652c  None, cabs=None,
+000131f0: 2063 7265 6c3d 4e6f 6e65 2c20 6e61 6d65   crel=None, name
+00013200: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
+00013210: 2022 2222 696e 6974 6961 6c69 7a65 2064   """initialize d
+00013220: 6174 6120 6f62 6a65 6374 0a0a 2020 2020  ata object..    
+00013230: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00013240: 2020 2020 2d20 2078 3a20 2020 2020 2064      -  x:      d
+00013250: 6174 6120 7661 6c75 6573 0a20 2020 2020  ata values.     
+00013260: 2020 2020 202d 2020 733a 2020 2020 2020       -  s:      
+00013270: 696e 6465 7065 6e64 656e 7420 756e 6365  independent unce
+00013280: 7274 6169 6e74 6965 7320 780a 2020 2020  rtainties x.    
+00013290: 2020 2020 2020 2d20 2073 7265 6c3a 2020        -  srel:  
+000132a0: 2069 6e64 6570 656e 6465 6e74 2072 656c   independent rel
+000132b0: 6174 6976 6520 756e 6365 7274 6169 6e74  ative uncertaint
+000132c0: 6965 7320 780a 2020 2020 2020 2020 2020  ies x.          
+000132d0: 2d20 2063 6162 733a 2020 2063 6f72 7265  -  cabs:   corre
+000132e0: 6c61 7465 6420 6162 6f6c 7574 6520 756e  lated abolute un
+000132f0: 6365 7274 6169 6e74 6965 7320 780a 2020  certainties x.  
+00013300: 2020 2020 2020 2020 2d20 2063 7265 6c3a          -  crel:
+00013310: 2020 2063 6f72 7265 6c61 7465 6420 7265     correlated re
+00013320: 6c61 7469 7665 2075 6e63 6572 7461 696e  lative uncertain
+00013330: 7469 6573 2078 0a20 2020 2020 2020 2022  ties x.        "
+00013340: 2222 0a0a 2020 2020 2020 2020 2320 6372  ""..        # cr
+00013350: 6561 7465 2064 6174 6120 6f62 6a65 6374  eate data object
+00013360: 2061 6e64 2070 6173 7320 616c 6c20 696e   and pass all in
+00013370: 7075 7420 6172 6775 6d65 6e74 730a 2020  put arguments.  
+00013380: 2020 2020 2020 7365 6c66 2e78 4461 7461        self.xData
+00013390: 203d 2073 656c 662e 7844 6174 6143 6f6e   = self.xDataCon
+000133a0: 7461 696e 6572 280a 2020 2020 2020 2020  tainer(.        
+000133b0: 2020 2020 7365 6c66 2c20 782c 2065 2c20      self, x, e, 
+000133c0: 6572 656c 2c20 6361 6273 2c20 6372 656c  erel, cabs, crel
+000133d0: 2c20 6e61 6d65 733d 6e61 6d65 732c 2071  , names=names, q
+000133e0: 7569 6574 3d73 656c 662e 7175 6965 740a  uiet=self.quiet.
+000133f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00013400: 2020 7365 6c66 2e64 6174 6120 3d20 7365    self.data = se
+00013410: 6c66 2e78 4461 7461 0a20 2020 2020 2020  lf.xData.       
+00013420: 2023 2073 6574 2066 6c61 6773 2066 6f72   # set flags for
+00013430: 2073 7465 6572 696e 6720 6f66 2066 6974   steering of fit
+00013440: 2070 726f 6365 7373 2069 6e20 646f 5f66   process in do_f
+00013450: 6974 2829 0a20 2020 2020 2020 2073 656c  it().        sel
+00013460: 662e 6974 6572 6174 6546 6974 203d 2073  f.iterateFit = s
+00013470: 656c 662e 7844 6174 612e 6861 735f 7265  elf.xData.has_re
+00013480: 6c5f 4572 726f 7273 2061 6e64 2073 656c  l_Errors and sel
+00013490: 662e 7265 664d 6f64 656c 0a0a 2020 2020  f.refModel..    
+000134a0: 6465 6620 696e 6974 5f78 4669 7428 0a20  def init_xFit(. 
+000134b0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+000134c0: 2020 2020 206d 6f64 656c 2c0a 2020 2020       model,.    
+000134d0: 2020 2020 6d6f 6465 6c5f 6b77 6172 6773      model_kwargs
+000134e0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2070  =None,.        p
+000134f0: 303d 4e6f 6e65 2c0a 2020 2020 2020 2020  0=None,.        
+00013500: 6470 303d 4e6f 6e65 2c0a 2020 2020 2020  dp0=None,.      
+00013510: 2020 636f 6e73 7472 6169 6e74 733d 4e6f    constraints=No
+00013520: 6e65 2c0a 2020 2020 2020 2020 6669 7850  ne,.        fixP
+00013530: 6172 733d 4e6f 6e65 2c0a 2020 2020 2020  ars=None,.      
+00013540: 2020 6c69 6d69 7473 3d4e 6f6e 652c 0a20    limits=None,. 
+00013550: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00013560: 2269 6e69 7469 616c 697a 6520 6669 7420  "initialize fit 
+00013570: 6f62 6a65 6374 0a0a 2020 2020 2020 2020  object..        
+00013580: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00013590: 2d20 6d6f 6465 6c3a 206d 6f64 656c 2066  - model: model f
+000135a0: 756e 6374 696f 6e20 6628 783b 205c 2a70  unction f(x; \*p
+000135b0: 6172 290a 2020 2020 2020 2020 2020 2d20  ar).          - 
+000135c0: 6d6f 6465 6c5f 6b77 6172 6773 3a20 6f70  model_kwargs: op
+000135d0: 7469 6f6e 616c 2c20 6669 7420 7061 7261  tional, fit para
+000135e0: 6d65 7465 7273 2069 6620 6e6f 7420 6672  meters if not fr
+000135f0: 6f6d 206d 6f64 656c 2073 6967 6e61 7475  om model signatu
+00013600: 7265 0a20 2020 2020 2020 2020 202d 2070  re.          - p
+00013610: 303a 206e 702d 6172 7261 7920 6f66 2066  0: np-array of f
+00013620: 6c6f 6174 732c 2069 6e69 7469 616c 2070  loats, initial p
+00013630: 6172 616d 6574 6572 2076 616c 7565 730a  arameter values.
+00013640: 2020 2020 2020 2020 2020 2d20 6470 303a            - dp0:
+00013650: 2061 7272 6179 2d6c 696b 652c 2069 6e69   array-like, ini
+00013660: 7469 616c 2067 7565 7373 206f 6620 7061  tial guess of pa
+00013670: 7261 6d65 7465 7220 756e 6365 7274 6169  rameter uncertai
+00013680: 6e74 6965 7320 286f 7074 696f 6e61 6c29  nties (optional)
+00013690: 0a20 2020 2020 2020 2020 202d 2063 6f6e  .          - con
+000136a0: 7374 7261 696e 7473 3a20 286e 6573 7465  straints: (neste
+000136b0: 6429 206c 6973 7428 7329 3a20 5b70 6172  d) list(s): [par
+000136c0: 616d 6574 6572 206e 616d 652c 2076 616c  ameter name, val
+000136d0: 7565 2c20 756e 6365 7274 6169 6e74 795d  ue, uncertainty]
+000136e0: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
+000136f0: 5b70 6172 616d 6574 6572 2069 6e64 6578  [parameter index
+00013700: 2c20 7661 6c75 652c 2075 6e63 6572 7461  , value, uncerta
+00013710: 696e 7479 5d0a 2020 2020 2020 2020 2020  inty].          
+00013720: 2d20 6c69 6d69 7473 3a20 286e 6573 7465  - limits: (neste
+00013730: 6429 206c 6973 7428 7329 3a20 5b70 6172  d) list(s): [par
+00013740: 616d 6574 6572 206e 616d 652c 206d 696e  ameter name, min
+00013750: 2c20 6d61 785d 0a20 2020 2020 2020 2020  , max].         
+00013760: 2020 206f 7220 5b70 6172 616d 6574 6572     or [parameter
+00013770: 2069 6e64 6578 2c20 6d69 6e2c 206d 6178   index, min, max
+00013780: 5d0a 2020 2020 2020 2020 2222 220a 0a20  ].        """.. 
+00013790: 2020 2020 2020 2069 6620 7365 6c66 2e78         if self.x
+000137a0: 4461 7461 2069 7320 4e6f 6e65 3a0a 2020  Data is None:.  
+000137b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000137c0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+000137d0: 2020 2020 2020 2020 2020 2020 2220 2121              " !!
+000137e0: 2120 6d6e 4669 742e 696e 6974 5f78 4669  ! mnFit.init_xFi
+000137f0: 743a 206e 6f20 6461 7461 206f 626a 6563  t: no data objec
+00013800: 7420 6465 6669 6e65 6420 2d20 6361 6c6c  t defined - call
+00013810: 2069 6e69 745f 6461 7461 2829 220a 2020   init_data()".  
+00013820: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00013830: 2020 2020 2023 2067 6574 2070 6172 616d       # get param
+00013840: 6574 6572 7320 6f66 206d 6f64 656c 2066  eters of model f
+00013850: 756e 6374 696f 6e20 746f 2073 6574 2073  unction to set s
+00013860: 7461 7274 2076 616c 7565 7320 666f 7220  tart values for 
+00013870: 6669 740a 2020 2020 2020 2020 6966 206d  fit.        if m
+00013880: 6f64 656c 5f6b 7761 7267 7320 6973 204e  odel_kwargs is N
+00013890: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000138a0: 2061 7267 732c 206d 6f64 656c 5f6b 7761   args, model_kwa
+000138b0: 7267 7320 3d20 6765 745f 6675 6e63 7469  rgs = get_functi
+000138c0: 6f6e 5369 676e 6174 7572 6528 6d6f 6465  onSignature(mode
+000138d0: 6c29 0a0a 2020 2020 2020 2020 7061 7220  l)..        par 
+000138e0: 3d20 286d 6f64 656c 5f6b 7761 7267 732c  = (model_kwargs,
+000138f0: 2070 302c 2064 7030 2c20 636f 6e73 7472   p0, dp0, constr
+00013900: 6169 6e74 732c 2066 6978 5061 7273 2c20  aints, fixPars, 
+00013910: 6c69 6d69 7473 290a 2020 2020 2020 2020  limits).        
+00013920: 7365 6c66 2e5f 7365 7475 7046 6974 5061  self._setupFitPa
+00013930: 7261 6d65 7465 7273 282a 7061 7229 0a0a  rameters(*par)..
+00013940: 2020 2020 2020 2020 2320 6372 6561 7465          # create
+00013950: 2063 6f73 7420 6675 6e63 7469 6f6e 0a20   cost function. 
+00013960: 2020 2020 2020 2073 656c 662e 636f 7374         self.cost
+00013970: 6620 3d20 7365 6c66 2e69 6e64 6578 6564  f = self.indexed
+00013980: 436f 7374 2873 656c 662c 206d 6f64 656c  Cost(self, model
+00013990: 2c20 7573 655f 6e65 6732 6c6f 674c 3d73  , use_neg2logL=s
+000139a0: 656c 662e 7573 655f 6e65 674c 6f67 4c29  elf.use_negLogL)
+000139b0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
+000139c0: 6574 7570 4d69 6e75 6974 286d 6f64 656c  etupMinuit(model
+000139d0: 5f6b 7761 7267 7329 0a0a 2020 2020 636c  _kwargs)..    cl
+000139e0: 6173 7320 7844 6174 6143 6f6e 7461 696e  ass xDataContain
+000139f0: 6572 3a0a 2020 2020 2020 2020 2222 220a  er:.        """.
+00013a00: 2020 2020 2020 2020 4861 6e64 6c65 2064          Handle d
+00013a10: 6174 6120 616e 6420 756e 6365 7274 6169  ata and uncertai
+00013a20: 6e74 6965 7320 616e 640a 2020 2020 2020  nties and.      
+00013a30: 2020 6275 696c 6420 636f 7661 7269 616e    build covarian
+00013a40: 6365 206d 6174 7269 6365 7320 6672 6f6d  ce matrices from
+00013a50: 2063 6f6d 706f 6e65 6e74 730a 0a20 2020   components..   
+00013a60: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00013a70: 2020 2020 202d 206f 7574 6572 3a20 2020       - outer:   
+00013a80: 706f 696e 7465 7220 746f 2069 6e73 7461  pointer to insta
+00013a90: 6e63 6520 6f66 2063 616c 6c69 6e67 206f  nce of calling o
+00013aa0: 626a 6563 740a 2020 2020 2020 2020 2020  bject.          
+00013ab0: 2d20 783a 2020 2020 2020 2061 6273 6369  - x:       absci
+00013ac0: 7373 6120 6f66 2064 6174 6120 706f 696e  ssa of data poin
+00013ad0: 7473 2028 2278 2076 616c 7565 7322 290a  ts ("x values").
+00013ae0: 2020 2020 2020 2020 2020 2d20 653a 2020            - e:  
+00013af0: 2020 2020 2069 6e64 6570 656e 6465 6e74       independent
+00013b00: 2075 6e63 6572 7461 696e 7469 6573 0a20   uncertainties. 
+00013b10: 2020 2020 2020 2020 202d 2065 7265 6c3a           - erel:
+00013b20: 2020 2069 6e64 6570 656e 6465 6e74 2072     independent r
+00013b30: 656c 6174 6976 6520 756e 6365 7274 6169  elative uncertai
+00013b40: 6e74 6965 7320 780a 2020 2020 2020 2020  nties x.        
+00013b50: 2020 2d20 6361 6273 3a20 2020 636f 7272    - cabs:   corr
+00013b60: 656c 6174 6564 2061 626f 6c75 7465 2075  elated abolute u
+00013b70: 6e63 6572 7461 696e 7469 6573 2078 0a20  ncertainties x. 
+00013b80: 2020 2020 2020 2020 202d 2063 7265 6c3a           - crel:
+00013b90: 2020 2063 6f72 7265 6c61 7465 6420 7265     correlated re
+00013ba0: 6c61 7469 7665 2075 6e63 6572 7461 696e  lative uncertain
+00013bb0: 7469 6573 2078 0a20 2020 2020 2020 2020  ties x.         
+00013bc0: 202d 2071 7569 6574 3a20 2020 6e6f 2069   - quiet:   no i
+00013bd0: 6e66 6f72 6d61 7469 7665 2070 7269 6e74  nformative print
+00013be0: 6f75 7420 6966 2054 7275 650a 0a20 2020  out if True..   
+00013bf0: 2020 2020 2050 7562 6c69 6320 6d65 7468       Public meth
+00013c00: 6f64 733a 0a20 2020 2020 2020 2020 202d  ods:.          -
+00013c10: 2069 6e69 745f 6479 6e61 6d69 6345 7272   init_dynamicErr
+00013c20: 6f72 7328 293a 0a20 2020 2020 2020 2020  ors():.         
+00013c30: 202d 2067 6574 5f43 6f76 2829 3a20 6669   - get_Cov(): fi
+00013c40: 6e61 6c20 636f 7661 7269 616e 6365 206d  nal covariance m
+00013c50: 6174 7269 7820 2869 6e63 6c2e 2070 726f  atrix (incl. pro
+00013c60: 6a2e 2078 290a 2020 2020 2020 2020 2020  j. x).          
+00013c70: 2d20 6765 745f 6943 6f76 2829 3a20 696e  - get_iCov(): in
+00013c80: 7665 7273 6520 636f 7661 7269 616e 6365  verse covariance
+00013c90: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
+00013ca0: 2020 2d20 706c 6f74 2829 3a20 7072 6f76    - plot(): prov
+00013cb0: 6964 6520 6120 6669 6775 7265 2077 6974  ide a figure wit
+00013cc0: 6820 7265 7072 6573 656e 7461 7469 6f6e  h representation
+00013cd0: 206f 6620 6461 7461 0a0a 2020 2020 2020   of data..      
+00013ce0: 2020 4461 7461 206d 656d 6265 7273 3a0a    Data members:.
+00013cf0: 2020 2020 2020 2020 2020 2a20 636f 7079            * copy
+00013d00: 206f 6620 616c 6c20 696e 7075 7420 6172   of all input ar
+00013d10: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
+00013d20: 2020 2a20 636f 763a 2063 6f76 6172 6961    * cov: covaria
+00013d30: 6e63 6520 6d61 7472 6978 0a20 2020 2020  nce matrix.     
+00013d40: 2020 2020 202a 2069 436f 763a 2069 6e76       * iCov: inv
+00013d50: 6572 7365 206f 6620 636f 7661 7269 616e  erse of covarian
+00013d60: 6365 206d 6174 7269 780a 2020 2020 2020  ce matrix.      
+00013d70: 2020 2222 220a 0a20 2020 2020 2020 2064    """..        d
+00013d80: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00013d90: 2c20 6f75 7465 722c 2078 2c20 652c 2065  , outer, x, e, e
+00013da0: 7265 6c2c 2063 6162 732c 2063 7265 6c2c  rel, cabs, crel,
+00013db0: 206e 616d 6573 3d4e 6f6e 652c 2071 7569   names=None, qui
+00013dc0: 6574 3d54 7275 6529 3a0a 2020 2020 2020  et=True):.      
+00013dd0: 2020 2020 2020 2320 7361 7665 2070 6f69        # save poi
+00013de0: 6e65 7220 746f 2063 616c 6c69 6e67 2063  ner to calling c
+00013df0: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
+00013e00: 2073 656c 662e 6f75 7465 7220 3d20 6f75   self.outer = ou
+00013e10: 7465 720a 0a20 2020 2020 2020 2020 2020  ter..           
+00013e20: 2023 2061 7373 756d 6520 7369 6d70 6c65   # assume simple
+00013e30: 2063 6173 6520 772e 6f2e 2063 6f76 2e6d   case w.o. cov.m
+00013e40: 6174 2e0a 2020 2020 2020 2020 2020 2020  at..            
+00013e50: 7365 6c66 2e6e 6565 6473 5f63 6f76 6172  self.needs_covar
+00013e60: 6961 6e63 6520 3d20 4661 6c73 650a 0a20  iance = False.. 
+00013e70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00013e80: 784e 616d 6573 203d 206e 616d 6573 2020  xNames = names  
+00013e90: 2320 7365 7420 7061 7261 6d65 7465 7220  # set parameter 
+00013ea0: 6e61 6d65 730a 0a20 2020 2020 2020 2020  names..         
+00013eb0: 2020 206e 6420 3d20 6c65 6e28 7829 0a20     nd = len(x). 
+00013ec0: 2020 2020 2020 2020 2020 2023 2073 746f             # sto
+00013ed0: 7265 2069 6e70 7574 2064 6174 6120 6173  re input data as
+00013ee0: 206e 756d 7079 2066 6c6f 6174 2061 7272   numpy float arr
+00013ef0: 6179 732c 2065 6e73 7572 6520 6c65 6e67  ays, ensure leng
+00013f00: 7468 206e 6420 6966 206e 6565 6465 640a  th nd if needed.
+00013f10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013f20: 2e78 203d 206e 702e 6173 6661 7272 6179  .x = np.asfarray
+00013f30: 2878 2920 2023 2061 6273 6369 7373 6120  (x)  # abscissa 
+00013f40: 2d20 2278 2076 616c 7565 7322 0a20 2020  - "x values".   
+00013f50: 2020 2020 2020 2020 2073 656c 662e 6520           self.e 
+00013f60: 3d20 6e70 2e61 7366 6172 7261 7928 6529  = np.asfarray(e)
+00013f70: 2020 2320 696e 6465 7065 6e64 656e 7420    # independent 
+00013f80: 756e 6365 7274 6169 6e74 6965 7320 790a  uncertainties y.
+00013f90: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00013fa0: 656c 662e 652e 6e64 696d 203d 3d20 303a  elf.e.ndim == 0:
+00013fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013fc0: 2073 656c 662e 6520 3d20 7365 6c66 2e65   self.e = self.e
+00013fd0: 202a 206e 702e 6f6e 6573 286e 6429 0a20   * np.ones(nd). 
+00013fe0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00013ff0: 7365 6c66 2e65 2e6e 6469 6d20 3d3d 2032  self.e.ndim == 2
+00014000: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014010: 2020 7365 6c66 2e6e 6565 6473 5f63 6f76    self.needs_cov
+00014020: 6172 6961 6e63 6520 3d20 5472 7565 0a20  ariance = True. 
+00014030: 2020 2020 2020 2020 2020 2069 6620 6572             if er
+00014040: 656c 2069 7320 6e6f 7420 4e6f 6e65 3a0a  el is not None:.
+00014050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014060: 7365 6c66 2e65 7265 6c20 3d20 6e70 2e61  self.erel = np.a
+00014070: 7366 6172 7261 7928 6572 656c 2920 2023  sfarray(erel)  #
+00014080: 2069 6e64 6570 656e 6465 6e74 2072 656c   independent rel
+00014090: 6174 6976 6520 756e 6365 7274 6169 6e74  ative uncertaint
+000140a0: 6965 7320 780a 2020 2020 2020 2020 2020  ies x.          
+000140b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000140c0: 2020 2020 2020 2020 7365 6c66 2e65 7265          self.ere
+000140d0: 6c20 3d20 4e6f 6e65 0a20 2020 2020 2020  l = None.       
+000140e0: 2020 2020 2069 6620 6361 6273 2069 7320       if cabs is 
+000140f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00014100: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00014110: 6162 7320 3d20 6e70 2e61 7366 6172 7261  abs = np.asfarra
+00014120: 7928 6361 6273 2920 2023 2063 6f72 7265  y(cabs)  # corre
+00014130: 6c61 7465 6420 6162 6f6c 7574 6520 756e  lated abolute un
+00014140: 6365 7274 6169 6e74 6965 7320 780a 2020  certainties x.  
+00014150: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00014160: 2073 656c 662e 6361 6273 2e6e 6469 6d20   self.cabs.ndim 
+00014170: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00014180: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00014190: 6162 7320 3d20 7365 6c66 2e63 6162 7320  abs = self.cabs 
+000141a0: 2a20 6e70 2e6f 6e65 7328 6e64 290a 2020  * np.ones(nd).  
+000141b0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+000141c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000141d0: 7365 6c66 2e63 6162 7320 3d20 4e6f 6e65  self.cabs = None
+000141e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000141f0: 6372 656c 2069 7320 6e6f 7420 4e6f 6e65  crel is not None
+00014200: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014210: 2020 7365 6c66 2e63 7265 6c20 3d20 6e70    self.crel = np
+00014220: 2e61 7366 6172 7261 7928 6372 656c 2920  .asfarray(crel) 
+00014230: 2023 2063 6f72 7265 6c61 7465 6420 7265   # correlated re
+00014240: 6c61 7469 7665 2075 6e63 6572 7461 696e  lative uncertain
+00014250: 7469 6573 2078 0a20 2020 2020 2020 2020  ties x.         
+00014260: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00014270: 2020 2020 2020 2020 2073 656c 662e 6372           self.cr
+00014280: 656c 203d 204e 6f6e 650a 2020 2020 2020  el = None.      
+00014290: 2020 2020 2020 7365 6c66 2e71 7569 6574        self.quiet
+000142a0: 203d 2071 7569 6574 2020 2320 6e6f 2069   = quiet  # no i
+000142b0: 6e66 6f72 6d61 7469 7665 2070 7269 6e74  nformative print
+000142c0: 6f75 7420 6966 2054 7275 650a 0a20 2020  out if True..   
+000142d0: 2020 2020 2020 2020 2073 656c 662e 6e64           self.nd
+000142e0: 203d 206e 640a 2020 2020 2020 2020 2020   = nd.          
+000142f0: 2020 7365 6c66 2e64 6c65 6e67 7468 203d    self.dlength =
+00014300: 206e 640a 2020 2020 2020 2020 2020 2020   nd.            
+00014310: 7365 6c66 2e6d 6f64 656c 203d 204e 6f6e  self.model = Non
+00014320: 6520 2023 206e 6f20 6d6f 6465 6c20 6465  e  # no model de
+00014330: 6669 6e65 6420 7965 740a 2020 2020 2020  fined yet.      
+00014340: 2020 2020 2020 7365 6c66 2e6d 6f64 656c        self.model
+00014350: 5f76 616c 7565 7320 3d20 4e6f 6e65 0a0a  _values = None..
+00014360: 2020 2020 2020 2020 2020 2020 2320 7365              # se
+00014370: 7420 666c 6167 7320 666f 7220 7374 6565  t flags for stee
+00014380: 7269 6e67 206f 6620 6669 7420 7072 6f63  ring of fit proc
+00014390: 6573 7320 696e 2064 6f5f 6669 7428 290a  ess in do_fit().
+000143a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000143b0: 2e72 6562 756c 696c 6443 6f76 203d 204e  .rebulildCov = N
+000143c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000143d0: 7365 6c66 2e68 6173 5f72 656c 5f45 7272  self.has_rel_Err
+000143e0: 6f72 7320 3d20 6572 656c 2069 7320 6e6f  ors = erel is no
+000143f0: 7420 4e6f 6e65 206f 7220 6372 656c 2069  t None or crel i
+00014400: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
+00014410: 2020 2020 2020 2073 656c 662e 6e65 6564         self.need
+00014420: 735f 636f 7661 7269 616e 6365 203d 2028  s_covariance = (
+00014430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014440: 2073 656c 662e 6e65 6564 735f 636f 7661   self.needs_cova
+00014450: 7269 616e 6365 206f 7220 7365 6c66 2e63  riance or self.c
+00014460: 6162 7320 6973 206e 6f74 204e 6f6e 6520  abs is not None 
+00014470: 6f72 2073 656c 662e 6372 656c 2069 7320  or self.crel is 
+00014480: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+00014490: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000144a0: 2020 2020 2320 6275 696c 6420 2869 6e69      # build (ini
+000144b0: 7469 616c 2920 636f 7661 7269 616e 6365  tial) covariance
+000144c0: 206d 6174 7269 7820 2877 6974 686f 7574   matrix (without
+000144d0: 2078 2d65 7272 6f72 7329 0a20 2020 2020   x-errors).     
+000144e0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
+000144f0: 6565 6473 5f63 6f76 6172 6961 6e63 653a  eeds_covariance:
+00014500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014510: 2065 7272 3220 3d20 5f62 7569 6c64 5f43   err2 = _build_C
+00014520: 6f76 4d61 7428 0a20 2020 2020 2020 2020  ovMat(.         
+00014530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014540: 6e64 2c20 7365 6c66 2e65 2c20 7365 6c66  nd, self.e, self
+00014550: 2e65 7265 6c2c 2073 656c 662e 6361 6273  .erel, self.cabs
+00014560: 2c20 7365 6c66 2e63 7265 6c2c 2073 656c  , self.crel, sel
+00014570: 662e 780a 2020 2020 2020 2020 2020 2020  f.x.            
+00014580: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00014590: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000145a0: 2020 2020 2020 2020 6572 7232 203d 205f          err2 = _
+000145b0: 6275 696c 645f 4572 7232 2873 656c 662e  build_Err2(self.
+000145c0: 652c 2073 656c 662e 6572 656c 2c20 7365  e, self.erel, se
+000145d0: 6c66 2e78 290a 0a20 2020 2020 2020 2020  lf.x)..         
+000145e0: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
+000145f0: 756e 6365 7274 6169 6e74 6965 7320 616e  uncertainties an
+00014600: 6420 636f 7661 7269 616e 6365 206d 6174  d covariance mat
+00014610: 7269 782c 0a20 2020 2020 2020 2020 2020  rix,.           
+00014620: 2073 656c 662e 5f69 6e69 7469 616c 436f   self._initialCo
+00014630: 7628 6572 7232 290a 2020 2020 2020 2020  v(err2).        
+00014640: 2020 2020 2320 7365 7473 3a0a 2020 2020      # sets:.    
+00014650: 2020 2020 2020 2020 2320 2020 7365 6c66          #   self
+00014660: 2e63 6f76 783a 2063 6f76 6172 6961 6e63  .covx: covarianc
+00014670: 6520 6d61 7472 6978 206f 6620 780a 2020  e matrix of x.  
+00014680: 2020 2020 2020 2020 2020 2320 2020 7365            #   se
+00014690: 6c66 2e63 6f76 793a 2063 6f76 6172 6961  lf.covy: covaria
+000146a0: 6e63 6520 6d61 7472 6978 206f 6620 7920  nce matrix of y 
+000146b0: 756e 6365 7274 6169 6e74 6965 730a 2020  uncertainties.  
+000146c0: 2020 2020 2020 2020 2020 2320 2020 7365            #   se
+000146d0: 6c66 2e63 6f76 3a20 6675 6c6c 2063 6f76  lf.cov: full cov
+000146e0: 6172 6961 6e63 6520 6d61 7472 6978 2069  ariance matrix i
+000146f0: 6e63 6c2e 2070 726f 6a65 6374 6564 2078  ncl. projected x
+00014700: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+00014710: 2073 656c 662e 6943 6f76 3a20 696e 7665   self.iCov: inve
+00014720: 7273 6520 6f66 2063 6f76 6172 6961 6e63  rse of covarianc
+00014730: 6520 6d61 7472 6978 0a20 2020 2020 2020  e matrix.       
+00014740: 2020 2020 2023 2020 2073 656c 662e 6572       #   self.er
+00014750: 7232 3a20 6172 7261 7920 6f66 2073 7175  r2: array of squ
+00014760: 6172 6564 2075 6e63 6572 7461 696e 7469  ared uncertainti
+00014770: 6573 0a20 2020 2020 2020 2020 2020 2023  es.            #
+00014780: 2020 2073 656c 662e 6945 7272 323a 2031     self.iErr2: 1
+00014790: 2e2f 7365 6c66 2e65 7272 320a 0a20 2020  ./self.err2..   
+000147a0: 2020 2020 2064 6566 205f 696e 6974 6961       def _initia
+000147b0: 6c43 6f76 2873 656c 662c 2065 7272 3229  lCov(self, err2)
+000147c0: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
+000147d0: 2242 7569 6c64 2069 6e69 7469 616c 2028  "Build initial (
+000147e0: 7374 6174 6963 2920 636f 7661 7269 616e  static) covarian
+000147f0: 6365 206d 6174 7269 7820 666f 7220 792d  ce matrix for y-
+00014800: 6572 726f 7273 0a20 2020 2020 2020 2020  errors.         
+00014810: 2020 2028 666f 7220 7072 652d 6669 7429     (for pre-fit)
+00014820: 2061 6e64 2063 616c 6375 6c61 7465 2069   and calculate i
+00014830: 6e76 6572 7365 206d 6174 7269 780a 2020  nverse matrix.  
+00014840: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
+00014850: 2020 2020 2020 2020 2020 6966 2065 7272            if err
+00014860: 322e 6e64 696d 203d 3d20 323a 0a20 2020  2.ndim == 2:.   
+00014870: 2020 2020 2020 2020 2020 2020 2023 2067               # g
+00014880: 6f74 2061 2063 6f76 6172 6961 6e63 6520  ot a covariance 
+00014890: 6d61 7472 6978 2c20 6e65 6564 2069 6e76  matrix, need inv
+000148a0: 6572 7365 0a20 2020 2020 2020 2020 2020  erse.           
+000148b0: 2020 2020 2073 656c 662e 6e65 6564 735f       self.needs_
+000148c0: 636f 7661 7269 616e 6365 203d 2054 7275  covariance = Tru
+000148d0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000148e0: 2020 7365 6c66 2e63 6f76 203d 2065 7272    self.cov = err
+000148f0: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
+00014900: 2020 7365 6c66 2e69 436f 7620 3d20 6c69    self.iCov = li
+00014910: 6e61 6c67 2e69 6e76 2865 7272 3229 0a20  nalg.inv(err2). 
+00014920: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014930: 656c 662e 6572 7232 203d 206e 702e 6469  elf.err2 = np.di
+00014940: 6167 6f6e 616c 2865 7272 3229 2020 2320  agonal(err2)  # 
+00014950: 7371 7561 7265 6420 6469 6167 6f6e 616c  squared diagonal
+00014960: 2065 6c65 6d65 6e74 730a 2020 2020 2020   elements.      
+00014970: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00014980: 2020 2020 2020 2020 2020 2020 2320 676f              # go
+00014990: 7420 696e 6465 7065 6e64 656e 7420 756e  t independent un
+000149a0: 6365 7274 6169 6e74 6965 730a 2020 2020  certainties.    
+000149b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000149c0: 2e65 7272 3220 3d20 6572 7232 0a20 2020  .err2 = err2.   
+000149d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000149e0: 662e 6572 7232 7920 3d20 6572 7232 0a20  f.err2y = err2. 
+000149f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00014a00: 656c 662e 6945 7272 3220 3d20 312e 3020  elf.iErr2 = 1.0 
+00014a10: 2f20 6572 7232 0a20 2020 2020 2020 2020  / err2.         
+00014a20: 2020 2020 2020 2073 656c 662e 636f 7620         self.cov 
+00014a30: 3d20 6e70 2e64 6961 6728 6572 7232 290a  = np.diag(err2).
+00014a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a50: 7365 6c66 2e69 436f 7620 3d20 6e70 2e64  self.iCov = np.d
+00014a60: 6961 6728 312e 3020 2f20 7365 6c66 2e65  iag(1.0 / self.e
+00014a70: 7272 3229 0a20 2020 2020 2020 2020 2020  rr2).           
+00014a80: 2023 2064 6f20 6e6f 7420 7265 6275 696c   # do not rebuil
+00014a90: 6420 636f 7661 7269 616e 6365 206d 6174  d covariance mat
+00014aa0: 7269 7820 696e 2063 6f73 7420 6675 6e63  rix in cost func
+00014ab0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00014ac0: 2073 656c 662e 6e65 6564 735f 6479 6e61   self.needs_dyna
+00014ad0: 6d69 6345 7272 6f72 7320 3d20 4661 6c73  micErrors = Fals
+00014ae0: 650a 0a20 2020 2020 2020 2064 6566 2069  e..        def i
+00014af0: 6e69 745f 6479 6e61 6d69 6345 7272 6f72  nit_dynamicError
+00014b00: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00014b10: 2020 2020 2023 206d 6574 686f 6420 746f       # method to
+00014b20: 2073 7769 7463 6820 6f6e 2064 796e 616d   switch on dynam
+00014b30: 6963 2072 652d 6361 6c63 756c 6174 696f  ic re-calculatio
+00014b40: 6e20 6f66 2063 6f76 6172 6961 6e63 6520  n of covariance 
+00014b50: 6d61 7472 6978 0a20 2020 2020 2020 2020  matrix.         
+00014b60: 2020 2073 656c 662e 7265 665f 746f 4d6f     self.ref_toMo
+00014b70: 6465 6c20 3d20 7365 6c66 2e6f 7574 6572  del = self.outer
+00014b80: 2e72 6566 4d6f 6465 6c0a 2020 2020 2020  .refModel.      
+00014b90: 2020 2020 2020 7365 6c66 2e6d 6f64 656c        self.model
+00014ba0: 203d 2073 656c 662e 6f75 7465 722e 636f   = self.outer.co
+00014bb0: 7374 662e 6d6f 6465 6c0a 0a20 2020 2020  stf.model..     
+00014bc0: 2020 2020 2020 2073 656c 662e 5f73 7461         self._sta
+00014bd0: 7469 6343 6f76 203d 204e 6f6e 650a 2020  ticCov = None.  
+00014be0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00014bf0: 7374 6174 6963 4572 7232 203d 204e 6f6e  staticErr2 = Non
+00014c00: 650a 2020 2020 2020 2020 2020 2020 7365  e.            se
+00014c10: 6c66 2e69 436f 7620 3d20 4e6f 6e65 0a20  lf.iCov = None. 
+00014c20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014c30: 6945 7272 3220 3d20 4e6f 6e65 0a0a 2020  iErr2 = None..  
+00014c40: 2020 2020 2020 2020 2020 2320 7265 6275            # rebu
+00014c50: 696c 6420 636f 7661 7269 616e 6365 206d  ild covariance m
+00014c60: 6174 7269 7820 6475 7269 6e67 2066 6974  atrix during fit
+00014c70: 7469 6e67 2070 726f 6365 6475 7265 0a20  ting procedure. 
+00014c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00014c90: 6e65 6564 735f 6479 6e61 6d69 6345 7272  needs_dynamicErr
+00014ca0: 6f72 7320 3d20 5472 7565 2020 2320 666c  ors = True  # fl
+00014cb0: 6167 2066 6f72 2063 6f73 7420 6675 6e63  ag for cost func
+00014cc0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
+00014cd0: 2073 656c 662e 6669 6e61 6c5f 6361 6c6c   self.final_call
+00014ce0: 203d 2046 616c 7365 2020 2320 666c 6167   = False  # flag
+00014cf0: 2066 6f72 205f 7265 6275 696c 645f 436f   for _rebuild_Co
+00014d00: 763a 206e 6f20 7374 6f72 6167 6520 6f66  v: no storage of
+00014d10: 2079 636f 760a 0a20 2020 2020 2020 2020   ycov..         
+00014d20: 2020 2069 6620 7365 6c66 2e6e 6565 6473     if self.needs
+00014d30: 5f63 6f76 6172 6961 6e63 653a 0a20 2020  _covariance:.   
+00014d40: 2020 2020 2020 2020 2020 2020 2023 2062               # b
+00014d50: 7569 6c64 2073 7461 7469 6320 283d 7061  uild static (=pa
+00014d60: 7261 6d65 7465 722d 696e 6465 7065 6e64  rameter-independ
+00014d70: 656e 7429 2070 6172 7420 6f66 2063 6f76  ent) part of cov
+00014d80: 6172 6961 6e63 6520 6d61 7472 6978 0a20  ariance matrix. 
+00014d90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014da0: 6620 7365 6c66 2e68 6173 5f72 656c 5f45  f self.has_rel_E
+00014db0: 7272 6f72 7320 616e 6420 7365 6c66 2e72  rrors and self.r
+00014dc0: 6566 5f74 6f4d 6f64 656c 3a0a 2020 2020  ef_toModel:.    
+00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014de0: 2320 736f 6d65 2079 2d65 7272 6f72 7320  # some y-errors 
+00014df0: 6172 6520 7061 7261 6d65 7465 722d 696e  are parameter-in
+00014e00: 6465 7065 6e64 656e 740a 2020 2020 2020  dependent.      
+00014e10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014e20: 6c66 2e5f 7374 6174 6963 436f 7620 3d20  lf._staticCov = 
+00014e30: 5f62 7569 6c64 5f43 6f76 4d61 7428 7365  _build_CovMat(se
+00014e40: 6c66 2e6e 642c 2073 656c 662e 652c 2065  lf.nd, self.e, e
+00014e50: 6162 7363 6f72 3d73 656c 662e 6361 6273  abscor=self.cabs
+00014e60: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014e70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00014e80: 2020 2020 2020 2020 2020 2020 2320 616c              # al
+00014e90: 6c20 792d 6572 726f 7273 2061 7265 2070  l y-errors are p
+00014ea0: 6172 616d 6574 6572 2d69 6e64 6570 656e  arameter-indepen
+00014eb0: 6465 6e74 0a20 2020 2020 2020 2020 2020  dent.           
+00014ec0: 2020 2020 2020 2020 2073 656c 662e 5f73           self._s
+00014ed0: 7461 7469 6343 6f76 203d 205f 6275 696c  taticCov = _buil
+00014ee0: 645f 436f 764d 6174 280a 2020 2020 2020  d_CovMat(.      
+00014ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f00: 2020 7365 6c66 2e6e 642c 0a20 2020 2020    self.nd,.     
+00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f20: 2020 2073 656c 662e 652c 0a20 2020 2020     self.e,.     
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f40: 2020 2065 7265 6c3d 7365 6c66 2e65 7265     erel=self.ere
+00014f50: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00014f60: 2020 2020 2020 2020 2020 2065 6162 7363             eabsc
+00014f70: 6f72 3d73 656c 662e 6361 6273 2c0a 2020  or=self.cabs,.  
+00014f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f90: 2020 2020 2020 6572 656c 636f 723d 7365        erelcor=se
+00014fa0: 6c66 2e63 7265 6c2c 0a20 2020 2020 2020  lf.crel,.       
+00014fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fc0: 2064 6174 613d 7365 6c66 2e78 2c0a 2020   data=self.x,.  
+00014fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014fe0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00014ff0: 2020 2020 2320 6275 696c 6420 6d61 7472      # build matr
+00015000: 6978 206f 6620 7265 6c61 7469 7665 2065  ix of relative e
+00015010: 7272 6f72 730a 2020 2020 2020 2020 2020  rrors.          
+00015020: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+00015030: 665f 746f 4d6f 6465 6c20 616e 6420 7365  f_toModel and se
+00015040: 6c66 2e68 6173 5f72 656c 5f45 7272 6f72  lf.has_rel_Error
+00015050: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00015060: 2020 2020 2020 2073 656c 662e 5f63 6f76         self._cov
+00015070: 7930 203d 205f 6275 696c 645f 436f 764d  y0 = _build_CovM
+00015080: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00015090: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000150a0: 2e6e 642c 0a20 2020 2020 2020 2020 2020  .nd,.           
+000150b0: 2020 2020 2020 2020 2020 2020 2065 7265               ere
+000150c0: 6c3d 7365 6c66 2e65 7265 6c2c 0a20 2020  l=self.erel,.   
+000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150e0: 2020 2020 2065 7265 6c63 6f72 3d73 656c       erelcor=sel
+000150f0: 662e 6372 656c 2c0a 2020 2020 2020 2020  f.crel,.        
+00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015110: 6461 7461 3d6e 702e 6f6e 6573 2873 656c  data=np.ones(sel
+00015120: 662e 6e64 292c 0a20 2020 2020 2020 2020  f.nd),.         
+00015130: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00015140: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00015150: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00015160: 2020 2020 2020 2073 656c 662e 5f63 6f76         self._cov
+00015170: 7930 203d 204e 6f6e 650a 0a20 2020 2020  y0 = None..     
+00015180: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
+00015190: 6e6f 2063 6f76 6172 6961 6e63 6520 6e65  no covariance ne
+000151a0: 6564 6564 2c20 7573 6520 7369 6d70 6c65  eded, use simple
+000151b0: 206d 6174 680a 2020 2020 2020 2020 2020   math.          
+000151c0: 2020 2020 2020 2320 6275 696c 6420 7374        # build st
+000151d0: 6174 6963 2028 3d70 6172 616d 6574 6572  atic (=parameter
+000151e0: 2d69 6e64 6570 656e 6465 6e74 2920 7061  -independent) pa
+000151f0: 7274 206f 6620 636f 7661 7269 616e 6365  rt of covariance
+00015200: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
+00015210: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00015220: 6861 735f 7265 6c5f 4572 726f 7273 2061  has_rel_Errors a
+00015230: 6e64 2073 656c 662e 7265 665f 746f 4d6f  nd self.ref_toMo
+00015240: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
+00015250: 2020 2020 2020 2020 2023 206f 6e6c 7920           # only 
+00015260: 696e 6465 7065 6e64 656e 7420 792d 6572  independent y-er
+00015270: 726f 7273 2064 6f20 6e6f 7420 6465 7065  rors do not depe
+00015280: 6e64 206f 6e20 7061 7261 6d65 7465 7273  nd on parameters
+00015290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000152a0: 2020 2020 2073 656c 662e 5f73 7461 7469       self._stati
+000152b0: 6345 7272 3220 3d20 5f62 7569 6c64 5f45  cErr2 = _build_E
+000152c0: 7272 3228 7365 6c66 2e65 290a 2020 2020  rr2(self.e).    
+000152d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000152e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000152f0: 2020 2020 2020 2320 616c 6c20 792d 6572        # all y-er
+00015300: 726f 7273 2061 7265 2070 6172 616d 6574  rors are paramet
+00015310: 6572 2d69 6e64 6570 656e 6465 6e74 0a20  er-independent. 
+00015320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015330: 2020 2073 656c 662e 5f73 7461 7469 6345     self._staticE
+00015340: 7272 3220 3d20 5f62 7569 6c64 5f45 7272  rr2 = _build_Err
+00015350: 3228 7365 6c66 2e65 2c20 7365 6c66 2e65  2(self.e, self.e
+00015360: 7265 6c2c 2073 656c 662e 7829 0a0a 2020  rel, self.x)..  
+00015370: 2020 2020 2020 6465 6620 5f72 6562 7569        def _rebui
+00015380: 6c64 5f45 7272 3228 7365 6c66 2c20 6d70  ld_Err2(self, mp
+00015390: 6172 293a 0a20 2020 2020 2020 2020 2020  ar):.           
+000153a0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
+000153b0: 2028 5265 2d29 6361 6c63 756c 6174 6520   (Re-)calculate 
+000153c0: 756e 6365 7274 6169 6e67 6965 730a 2020  uncertaingies.  
+000153d0: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
+000153e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+000153f0: 662e 5f73 7461 7469 6345 7272 3220 6973  f._staticErr2 is
+00015400: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00015410: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015420: 6572 7232 203d 206e 702e 6172 7261 7928  err2 = np.array(
+00015430: 7365 6c66 2e5f 7374 6174 6963 4572 7232  self._staticErr2
+00015440: 2c20 636f 7079 3d54 7275 6529 0a20 2020  , copy=True).   
+00015450: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00015460: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015470: 656c 662e 6572 7232 203d 206e 702e 7a65  elf.err2 = np.ze
+00015480: 726f 7328 7365 6c66 2e6e 6429 0a20 2020  ros(self.nd).   
+00015490: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000154a0: 2e72 6566 5f74 6f4d 6f64 656c 2061 6e64  .ref_toModel and
+000154b0: 2073 656c 662e 6861 735f 7265 6c5f 4572   self.has_rel_Er
+000154c0: 726f 7273 3a0a 2020 2020 2020 2020 2020  rors:.          
+000154d0: 2020 2020 2020 5f65 7220 3d20 7365 6c66        _er = self
+000154e0: 2e65 7265 6c20 2a20 7365 6c66 2e6d 6f64  .erel * self.mod
+000154f0: 656c 2873 656c 662e 782c 202a 6d70 6172  el(self.x, *mpar
+00015500: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00015510: 2020 7365 6c66 2e65 7272 3220 2b3d 205f    self.err2 += _
+00015520: 6572 202a 205f 6572 0a0a 2020 2020 2020  er * _er..      
+00015530: 2020 6465 6620 5f72 6562 7569 6c64 5f43    def _rebuild_C
+00015540: 6f76 2873 656c 662c 206d 7061 7229 3a0a  ov(self, mpar):.
+00015550: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00015560: 2020 2020 2020 2020 2020 2020 2852 652d              (Re-
+00015570: 2942 7569 6c64 2074 6865 2063 6f76 6172  )Build the covar
+00015580: 6961 6e63 6520 6d61 7472 6978 2066 726f  iance matrix fro
+00015590: 6d20 636f 6d70 6f6e 656e 7473 0a20 2020  m components.   
+000155a0: 2020 2020 2020 2020 2061 6e64 2063 6163           and cac
+000155b0: 6c75 6c61 7465 2069 7473 2069 6e76 6572  lulate its inver
+000155c0: 7365 0a20 2020 2020 2020 2020 2020 2022  se.            "
+000155d0: 2222 0a20 2020 2020 2020 2020 2020 2023  "".            #
+000155e0: 2073 7461 7274 2066 726f 6d20 7072 652d   start from pre-
+000155f0: 6275 696c 7420 7061 7261 6d65 7465 722d  built parameter-
+00015600: 696e 6465 7065 6e64 656e 7420 7061 7274  independent part
+00015610: 206f 6620 436f 7661 7269 616e 6365 204d   of Covariance M
+00015620: 6174 7269 780a 2020 2020 2020 2020 2020  atrix.          
+00015630: 2020 7365 6c66 2e63 6f76 203d 206e 702e    self.cov = np.
+00015640: 6172 7261 7928 7365 6c66 2e5f 7374 6174  array(self._stat
+00015650: 6963 436f 762c 2063 6f70 793d 5472 7565  icCov, copy=True
+00015660: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00015670: 2061 6464 206d 6174 7269 7820 6f66 2070   add matrix of p
+00015680: 6172 616d 6574 6572 2d64 6570 656e 6465  arameter-depende
+00015690: 6e74 2079 2d75 6e63 6572 7461 696e 7469  nt y-uncertainti
+000156a0: 6573 0a20 2020 2020 2020 2020 2020 2069  es.            i
+000156b0: 6620 7365 6c66 2e5f 636f 7679 3020 6973  f self._covy0 is
+000156c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000156d0: 2020 2020 2020 2020 2020 205f 6461 7420             _dat 
+000156e0: 3d20 7365 6c66 2e6d 6f64 656c 2873 656c  = self.model(sel
+000156f0: 662e 782c 202a 6d70 6172 290a 2020 2020  f.x, *mpar).    
+00015700: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015710: 2e63 6f76 202b 3d20 7365 6c66 2e5f 636f  .cov += self._co
+00015720: 7679 3020 2a20 6e70 2e6f 7574 6572 285f  vy0 * np.outer(_
+00015730: 6461 742c 205f 6461 7429 0a0a 2020 2020  dat, _dat)..    
+00015740: 2020 2020 6465 6620 6765 745f 436f 7628      def get_Cov(
+00015750: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
+00015760: 2020 2022 2222 7265 7475 726e 2063 6f76     """return cov
+00015770: 6172 6961 6e63 6520 6d61 7472 6978 206f  ariance matrix o
+00015780: 6620 6461 7461 2222 220a 2020 2020 2020  f data""".      
+00015790: 2020 2020 2020 6966 2073 656c 662e 6e65        if self.ne
+000157a0: 6564 735f 636f 7661 7269 616e 6365 3a0a  eds_covariance:.
+000157b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157c0: 7265 7475 726e 2073 656c 662e 636f 760a  return self.cov.
+000157d0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000157e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000157f0: 2020 6966 2073 656c 662e 6572 7232 2069    if self.err2 i
+00015800: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00015810: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00015820: 726e 204e 6f6e 650a 2020 2020 2020 2020  rn None.        
+00015830: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00015840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015850: 2020 7265 7475 726e 206e 702e 6469 6167    return np.diag
+00015860: 2873 656c 662e 6572 7232 290a 0a20 2020  (self.err2)..   
+00015870: 2020 2020 2064 6566 2067 6574 5f69 436f       def get_iCo
+00015880: 7628 7365 6c66 293a 0a20 2020 2020 2020  v(self):.       
+00015890: 2020 2020 2022 2222 7265 7475 726e 2069       """return i
+000158a0: 6e76 6572 7365 206f 6620 636f 7661 7269  nverse of covari
+000158b0: 616e 6365 206d 6174 7269 782c 2061 7320  ance matrix, as 
+000158c0: 7573 6564 2069 6e20 636f 7374 2066 756e  used in cost fun
+000158d0: 6374 696f 6e22 2222 0a20 2020 2020 2020  ction""".       
+000158e0: 2020 2020 2069 6620 7365 6c66 2e6e 6565       if self.nee
+000158f0: 6473 5f63 6f76 6172 6961 6e63 653a 0a20  ds_covariance:. 
+00015900: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00015910: 6574 7572 6e20 7365 6c66 2e69 436f 760a  eturn self.iCov.
+00015920: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00015930: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015940: 2020 7265 7475 726e 206e 702e 6469 6167    return np.diag
+00015950: 2831 2e30 202f 2073 656c 662e 6572 7232  (1.0 / self.err2
+00015960: 290a 0a20 2020 2020 2020 2064 6566 2070  )..        def p
+00015970: 6c6f 7428 0a20 2020 2020 2020 2020 2020  lot(.           
+00015980: 2073 656c 662c 0a20 2020 2020 2020 2020   self,.         
+00015990: 2020 206e 756d 3d22 4461 7461 2061 6e64     num="Data and
+000159a0: 204d 6f64 656c 222c 0a20 2020 2020 2020   Model",.       
+000159b0: 2020 2020 2066 6967 7369 7a65 3d28 372e       figsize=(7.
+000159c0: 352c 2036 2e35 292c 0a20 2020 2020 2020  5, 6.5),.       
+000159d0: 2020 2020 2064 6174 615f 6c61 6265 6c3d       data_label=
+000159e0: 2264 6174 6122 2c0a 2020 2020 2020 2020  "data",.        
+000159f0: 2020 2020 706c 6f74 5f72 6573 6964 7561      plot_residua
+00015a00: 6c3d 4661 6c73 652c 0a20 2020 2020 2020  l=False,.       
+00015a10: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00015a20: 2222 2272 6574 7572 6e20 6669 6775 7265  """return figure
+00015a30: 2077 6974 6820 6461 7461 2061 6e64 2075   with data and u
+00015a40: 6e63 6572 7461 696e 7469 6573 2222 220a  ncertainties""".
+00015a50: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00015a60: 2023 2067 6574 2064 6174 610a 2020 2020   # get data.    
+00015a70: 2020 2020 2020 2020 6966 2070 6c6f 745f          if plot_
+00015a80: 7265 7369 6475 616c 2061 6e64 2073 656c  residual and sel
+00015a90: 662e 6d6f 6465 6c5f 7661 6c75 6573 2069  f.model_values i
+00015aa0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00015ab0: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+00015ac0: 7365 6c66 2e78 202d 2073 656c 662e 6d6f  self.x - self.mo
+00015ad0: 6465 6c5f 7661 6c75 6573 0a20 2020 2020  del_values.     
+00015ae0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00015af0: 2020 2020 2020 2020 2020 2020 2078 203d               x =
+00015b00: 2073 656c 662e 780a 2020 2020 2020 2020   self.x.        
+00015b10: 2020 2020 6520 3d20 7365 6c66 2e67 6574      e = self.get
+00015b20: 5f43 6f76 2829 0a20 2020 2020 2020 2020  _Cov().         
+00015b30: 2020 2069 6620 652e 6e64 696d 203d 3d20     if e.ndim == 
+00015b40: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+00015b50: 2020 2065 203d 206e 702e 7371 7274 286e     e = np.sqrt(n
+00015b60: 702e 6469 6167 6f6e 616c 2865 2929 0a20  p.diagonal(e)). 
+00015b70: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00015b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015b90: 2065 203d 206e 702e 7371 7274 2865 290a   e = np.sqrt(e).
+00015ba0: 2020 2020 2020 2020 2020 2020 2320 6472              # dr
+00015bb0: 6177 2064 6174 610a 2020 2020 2020 2020  aw data.        
+00015bc0: 2020 2020 6669 6720 3d20 706c 742e 6669      fig = plt.fi
+00015bd0: 6775 7265 286e 756d 3d6e 756d 2c20 6669  gure(num=num, fi
+00015be0: 6773 697a 653d 6669 6773 697a 6529 0a20  gsize=figsize). 
+00015bf0: 2020 2020 2020 2020 2020 2069 6478 203d             idx =
+00015c00: 206e 702e 6c69 6e73 7061 6365 2830 2e35   np.linspace(0.5
+00015c10: 2c20 6c65 6e28 7829 202d 2030 2e35 2c20  , len(x) - 0.5, 
+00015c20: 6c65 6e28 7829 290a 2020 2020 2020 2020  len(x)).        
+00015c30: 2020 2020 706c 742e 706c 6f74 2869 6478      plt.plot(idx
+00015c40: 2c20 782c 206d 6172 6b65 723d 2278 222c  , x, marker="x",
+00015c50: 206c 696e 6573 7479 6c65 3d22 222c 2063   linestyle="", c
+00015c60: 6f6c 6f72 3d22 6772 6579 222c 2061 6c70  olor="grey", alp
+00015c70: 6861 3d30 2e35 290a 2020 2020 2020 2020  ha=0.5).        
+00015c80: 2020 2020 706c 742e 6572 726f 7262 6172      plt.errorbar
+00015c90: 2869 6478 2c20 782c 2065 2c20 666d 743d  (idx, x, e, fmt=
+00015ca0: 222e 222c 2063 6170 7369 7a65 3d33 2e30  ".", capsize=3.0
+00015cb0: 2c20 6c61 6265 6c3d 6461 7461 5f6c 6162  , label=data_lab
+00015cc0: 656c 290a 2020 2020 2020 2020 2020 2020  el).            
+00015cd0: 706c 742e 786c 696d 2830 2e30 2c20 6c65  plt.xlim(0.0, le
+00015ce0: 6e28 6964 7829 290a 2020 2020 2020 2020  n(idx)).        
+00015cf0: 2020 2020 6966 2073 656c 662e 784e 616d      if self.xNam
+00015d00: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+00015d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d20: 706c 742e 7874 6963 6b73 2874 6963 6b73  plt.xticks(ticks
+00015d30: 3d69 6478 2c20 6c61 6265 6c73 3d73 656c  =idx, labels=sel
+00015d40: 662e 784e 616d 6573 290a 2020 2020 2020  f.xNames).      
+00015d50: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00015d60: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+00015d70: 7874 6963 6b73 2874 6963 6b73 3d69 6478  xticks(ticks=idx
+00015d80: 2c20 6c61 6265 6c73 3d72 616e 6765 286c  , labels=range(l
+00015d90: 656e 2869 6478 2929 290a 0a20 2020 2020  en(idx)))..     
+00015da0: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
+00015db0: 670a 0a20 2020 2023 2064 6566 696e 6520  g..    # define 
+00015dc0: 6375 7374 6f6d 2063 6f73 7420 6675 6e63  custom cost func
+00015dd0: 7469 6f6e 2066 6f72 2069 6d69 6e75 6974  tion for iminuit
+00015de0: 0a20 2020 2063 6c61 7373 2069 6e64 6578  .    class index
+00015df0: 6564 436f 7374 3a0a 2020 2020 2020 2020  edCost:.        
+00015e00: 2222 220a 2020 2020 2020 2020 2043 7573  """.         Cus
+00015e10: 746f 6d20 655f 785f 7465 6e64 6564 204c  tom e_x_tended L
+00015e20: 6561 7374 2d53 5175 6172 6573 2063 6f73  east-SQuares cos
+00015e30: 7420 6675 6e63 7469 6f6e 2077 6974 680a  t function with.
+00015e40: 2020 2020 2020 2020 2064 796e 616d 6963           dynamic
+00015e50: 616c 6c79 2075 7064 6174 6564 2063 6f76  ally updated cov
+00015e60: 6172 6961 6e63 6520 6d61 7472 6978 2061  ariance matrix a
+00015e70: 6e64 202d 326c 6f67 284c 290a 2020 2020  nd -2log(L).    
+00015e80: 2020 2020 2063 6f72 7265 6374 696f 6e20       correction 
+00015e90: 7465 726d 2066 6f72 2070 6172 616d 6574  term for paramet
+00015ea0: 6572 2d64 6570 656e 6465 6e74 2075 6e63  er-dependent unc
+00015eb0: 6572 7461 696e 7469 6573 2e0a 0a20 2020  ertainties...   
+00015ec0: 2020 2020 2020 5468 6520 6465 6661 756c        The defaul
+00015ed0: 7420 636f 7374 2066 756e 6374 696f 6e20  t cost function 
+00015ee0: 6973 2074 7769 6365 2074 6865 206e 6567  is twice the neg
+00015ef0: 6174 6976 6520 6c6f 6761 7269 7468 6d0a  ative logarithm.
+00015f00: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
+00015f10: 6c69 6b65 6c69 686f 6f64 206f 6620 6120  likelihood of a 
+00015f20: 4761 7573 7369 616e 2064 6973 7472 6962  Gaussian distrib
+00015f30: 7574 696f 6e20 666f 7220 6461 7461 2070  ution for data p
+00015f40: 6f69 6e74 730a 2020 2020 2020 2020 203a  oints.         :
+00015f50: 6d61 7468 3a60 2878 2c20 7929 6020 7769  math:`(x, y)` wi
+00015f60: 7468 2061 206d 6f64 656c 2066 756e 6374  th a model funct
+00015f70: 696f 6e20 3a6d 6174 683a 6079 3d66 2878  ion :math:`y=f(x
+00015f80: 2c20 2a70 2960 2064 6570 656e 6469 6e67  , *p)` depending
+00015f90: 0a20 2020 2020 2020 2020 6f6e 2061 2073  .         on a s
+00015fa0: 6574 206f 6620 7061 7261 6d65 7465 7273  et of parameters
+00015fb0: 203a 6d61 7468 3a60 2a70 6020 616e 6420   :math:`*p` and 
+00015fc0: 6120 706f 7373 6962 6c79 2070 6172 616d  a possibly param
+00015fd0: 6574 6572 2d64 6570 656e 6465 6e74 0a20  eter-dependent. 
+00015fe0: 2020 2020 2020 2020 636f 7661 7269 616e          covarian
+00015ff0: 6365 206d 6174 7269 7820 3a6d 6174 683a  ce matrix :math:
+00016000: 6056 2878 2c20 6628 782c 202a 7029 2960  `V(x, f(x, *p))`
+00016010: 206f 6620 7468 6520 7820 616e 6420 7920   of the x and y 
+00016020: 6461 7461 3a0a 0a20 2020 2020 2020 2020  data:..         
+00016030: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
+00016040: 2020 2020 202d 325c 6c6e 207b 5c63 616c       -2\ln {\cal
+00016050: 204c 7d20 3d20 5c63 6869 5e32 2878 2c20   L} = \chi^2(x, 
+00016060: 565e 7b2d 317d 2c20 7828 2a70 2920 5c2c  V^{-1}, x(*p) \,
+00016070: 290a 2020 2020 2020 2020 2020 202b 205c  ).           + \
+00016080: 6c6e 285c 2c20 5c64 6574 2820 5628 782c  ln(\, \det( V(x,
+00016090: 2078 282a 7029 2029 205c 2c29 0a0a 2020   x(*p) ) \,)..  
+000160a0: 2020 2020 2020 2049 6e20 7468 6520 6162         In the ab
+000160b0: 7365 6e63 6520 6f66 2070 6172 616d 6574  sence of paramet
+000160c0: 6572 2d64 6570 656e 6465 6e74 2063 6f6d  er-dependent com
+000160d0: 706f 6e65 6e74 7320 6f66 2074 6865 2063  ponents of the c
+000160e0: 6f76 6172 6961 6e63 650a 2020 2020 2020  ovariance.      
+000160f0: 2020 206d 6174 7269 782c 2074 6865 206c     matrix, the l
+00016100: 6173 7420 7465 726d 2069 7320 6f6d 6974  ast term is omit
+00016110: 7465 6420 616e 6420 7468 6520 636f 7374  ted and the cost
+00016120: 2066 756e 6374 696f 6e20 6973 2069 6465   function is ide
+00016130: 6e74 6963 616c 0a20 2020 2020 2020 2020  ntical.         
+00016140: 746f 2074 6865 2063 6c61 7373 6963 616c  to the classical
+00016150: 203a 6d61 7468 3a60 5c63 6869 5e32 602e   :math:`\chi^2`.
+00016160: 0a20 2020 2020 2020 2020 466f 7220 7468  .         For th
+00016170: 6520 6576 616c 7561 7469 6f6e 206f 6620  e evaluation of 
+00016180: 7468 6520 636f 7374 2066 756e 6374 696f  the cost functio
+00016190: 6e20 616e 2065 6666 6963 6965 6e74 2061  n an efficient a
+000161a0: 7070 726f 6163 6820 6261 7365 640a 2020  pproach based.  
+000161b0: 2020 2020 2020 206f 6e20 7468 6520 2243         on the "C
+000161c0: 686f 6c65 736b 7920 6465 636f 6d70 6f73  holesky decompos
+000161d0: 6974 696f 6e22 206f 6620 7468 6520 636f  ition" of the co
+000161e0: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
+000161f0: 696e 0a20 2020 2020 2020 2020 6120 7072  in.         a pr
+00016200: 6f64 7563 7420 6f66 2061 2074 7269 616e  oduct of a trian
+00016210: 6775 6c61 7220 6d61 7472 6978 2061 6e64  gular matrix and
+00016220: 2069 7473 2074 7261 6e73 706f 7365 6420   its transposed 
+00016230: 6973 2075 7365 643a 0a0a 2020 2020 2020  is used:..      
+00016240: 2020 202e 2e20 6d61 7468 3a3a 0a20 2020     .. math::.   
+00016250: 2020 2020 2020 2020 2056 203d 204c 204c           V = L L
+00016260: 5e54 2e0a 0a20 2020 2020 2020 2020 5468  ^T...         Th
+00016270: 6520 7661 6c75 6520 6f66 2074 6865 2063  e value of the c
+00016280: 6f73 7420 6675 6e63 7469 6f6e 0a0a 2020  ost function..  
+00016290: 2020 2020 2020 202e 2e20 6d61 7468 3a3a         .. math::
+000162a0: 0a20 2020 2020 2020 2020 2020 5c63 6869  .           \chi
+000162b0: 5e32 203d 207b 727d 5c63 646f 7420 2856  ^2 = {r}\cdot (V
+000162c0: 5e7b 2d31 7d7b 727d 2920 7e7e 7769 7468  ^{-1}{r}) ~~with
+000162d0: 7e7e 2072 203d 2078 202d 2078 282a 7029  ~~ r = x - x(*p)
+000162e0: 0a0a 2020 2020 2020 2020 2069 7320 7468  ..         is th
+000162f0: 656e 2063 616c 6375 6c61 7465 6420 6279  en calculated by
+00016300: 2073 6f6c 7669 6e67 2074 6865 206c 696e   solving the lin
+00016310: 6561 7220 6571 7561 7469 6f6e 0a0a 2020  ear equation..  
+00016320: 2020 2020 2020 2e2e 206d 6174 683a 3a0a        .. math::.
+00016330: 2020 2020 2020 2020 2020 2056 2058 203d             V X =
+00016340: 2072 2c20 7e69 2e65 2e7e 2058 3d56 5e7b   r, ~i.e.~ X=V^{
+00016350: 2d31 7d20 7220 7e61 6e64 7e20 5c63 6869  -1} r ~and~ \chi
+00016360: 5e32 3d20 7220 5c63 646f 7420 580a 0a20  ^2= r \cdot X.. 
+00016370: 2020 2020 2020 2077 6974 6820 7468 6520         with the 
+00016380: 6c69 6e65 6172 2d65 7175 6174 696f 6e20  linear-equation 
+00016390: 736f 6c76 6572 202a 7363 6970 792e 6c69  solver *scipy.li
+000163a0: 6e61 6c67 2e63 686f 5f73 6f6c 7665 284c  nalg.cho_solve(L
+000163b0: 2c78 292a 0a20 2020 2020 2020 2066 6f72  ,x)*.        for
+000163c0: 2043 686f 6c65 736b 792d 6465 636f 6d70   Cholesky-decomp
+000163d0: 6f73 6564 206d 6174 7269 6365 732c 2074  osed matrices, t
+000163e0: 6875 7320 6176 6f69 6469 6e67 2074 6865  hus avoiding the
+000163f0: 2063 6f73 7479 0a20 2020 2020 2020 2063   costy.        c
+00016400: 616c 6375 6c61 7469 6f6e 206f 6620 7468  alculation of th
+00016410: 6520 696e 7665 7273 6520 6d61 7472 6978  e inverse matrix
+00016420: 2e0a 0a0a 2020 2020 2020 2020 5468 6520  ....        The 
+00016430: 6465 7465 726d 696e 616e 742c 2069 6620  determinant, if 
+00016440: 6e65 6564 6564 2c20 6973 2065 6666 6963  needed, is effic
+00016450: 6965 6e74 6c79 2063 616c 6375 6c61 7465  iently calculate
+00016460: 6420 6279 2074 616b 696e 670a 2020 2020  d by taking.    
+00016470: 2020 2020 7468 6520 7072 6f64 7563 7420      the product 
+00016480: 6f66 2074 6865 2064 6961 676f 6e61 6c20  of the diagonal 
+00016490: 656c 656d 656e 7473 206f 6620 7468 6520  elements of the 
+000164a0: 6d61 7472 6978 204c 2c0a 0a20 2020 2020  matrix L,..     
+000164b0: 2020 2020 2e2e 206d 6174 683a 3a0a 2020      .. math::.  
+000164c0: 2020 2020 2020 2020 205c 6465 7428 5629           \det(V)
+000164d0: 203d 2032 205c 2c20 5c70 726f 6420 4c5f   = 2 \, \prod L_
+000164e0: 7b69 2c69 7d0a 0a20 2020 2020 2020 2020  {i,i}..         
+000164f0: 496e 7075 743a 0a0a 2020 2020 2020 2020  Input:..        
+00016500: 202d 206f 7574 6572 3a20 706f 696e 7465   - outer: pointe
+00016510: 7220 746f 2069 6e73 7461 6e63 6520 6f66  r to instance of
+00016520: 2063 616c 6c69 6e67 2063 6c61 7373 0a20   calling class. 
+00016530: 2020 2020 2020 2020 2d20 6d6f 6465 6c3a          - model:
+00016540: 206d 6f64 656c 2066 756e 6374 696f 6e20   model function 
+00016550: 6361 6c75 6c61 7469 6e67 2074 6865 2064  calulating the d
+00016560: 6174 6120 7828 5c2a 7061 7229 0a20 2020  ata x(\*par).   
+00016570: 2020 2020 2020 2d20 7573 655f 6e65 6732        - use_neg2
+00016580: 6c6f 674c 3a20 7573 6520 6675 6c6c 202d  logL: use full -
+00016590: 326c 6f67 284c 2920 696e 7374 6561 6420  2log(L) instead 
+000165a0: 6f66 2063 6869 3220 6966 2054 7275 650a  of chi2 if True.
+000165b0: 0a20 2020 2020 2020 2020 5f5f 6361 6c6c  .         __call
+000165c0: 5f5f 206d 6574 686f 6420 6f66 2074 6869  __ method of thi
+000165d0: 7320 636c 6173 7320 6973 2063 616c 6c65  s class is calle
+000165e0: 6420 6279 2069 6d69 6e75 6974 0a0a 2020  d by iminuit..  
+000165f0: 2020 2020 2020 2044 6174 6120 6d65 6d62         Data memb
+00016600: 6572 733a 0a0a 2020 2020 2020 2020 202d  ers:..         -
+00016610: 206e 646f 663a 2064 6567 7265 6573 206f   ndof: degrees o
+00016620: 6620 6672 6565 646f 6d0a 2020 2020 2020  f freedom.      
+00016630: 2020 202d 206e 636f 6e73 7472 6169 6e74     - nconstraint
+00016640: 733a 206e 756d 6265 7220 6f66 2070 6172  s: number of par
+00016650: 616d 6574 6572 2063 6f6e 7374 7261 696e  ameter constrain
+00016660: 7473 0a20 2020 2020 2020 2020 2d20 676f  ts.         - go
+00016670: 663a 2063 6869 322d 7661 6c75 6520 2867  f: chi2-value (g
+00016680: 6f6f 646e 6573 7320 6f66 2066 6974 290a  oodness of fit).
+00016690: 2020 2020 2020 2020 202d 2075 7365 5f6e           - use_n
+000166a0: 6567 326c 6f67 4c3a 2075 7361 6765 206f  eg2logL: usage o
+000166b0: 6620 6675 6c6c 2032 2a6e 6567 204c 6f67  f full 2*neg Log
+000166c0: 204c 696b 656c 6968 6f6f 640a 2020 2020   Likelihood.    
+000166d0: 2020 2020 202d 2071 7569 6574 3a20 6e6f       - quiet: no
+000166e0: 2070 7269 6e74 6f75 7420 6966 2054 7275   printout if Tru
+000166f0: 650a 0a20 2020 2020 2020 2020 4d65 7468  e..         Meth
+00016700: 6f64 733a 0a0a 2020 2020 2020 2020 202d  ods:..         -
+00016710: 206d 6f64 656c 2878 2c20 5c2a 7061 7229   model(x, \*par)
+00016720: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
+00016730: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
+00016740: 5f5f 2873 656c 662c 206f 7574 6572 2c20  __(self, outer, 
+00016750: 6d6f 6465 6c2c 2075 7365 5f6e 6567 326c  model, use_neg2l
+00016760: 6f67 4c3d 4661 6c73 6529 3a0a 2020 2020  ogL=False):.    
+00016770: 2020 2020 2020 2020 2320 6461 7461 206f          # data o
+00016780: 626a 6563 7420 6f66 2074 7970 6520 7879  bject of type xy
+00016790: 4461 7461 436f 6e74 6169 6e65 720a 2020  DataContainer.  
+000167a0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000167b0: 6174 6120 3d20 6f75 7465 722e 6461 7461  ata = outer.data
+000167c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000167d0: 6e6f 7420 6973 696e 7374 616e 6365 2873  not isinstance(s
+000167e0: 656c 662e 6461 7461 2c20 6d6e 4669 742e  elf.data, mnFit.
+000167f0: 7844 6174 6143 6f6e 7461 696e 6572 293a  xDataContainer):
+00016800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016810: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00016820: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00016830: 2020 2020 2020 2022 2021 2121 206d 6e46         " !!! mnF
+00016840: 6974 2e69 6e64 6578 6564 436f 7374 3a20  it.indexedCost: 
+00016850: 6578 7065 6374 696e 6720 6461 7461 2063  expecting data c
+00016860: 6f6e 7461 696e 6572 206f 6620 7479 7065  ontainer of type
+00016870: 2027 6d6e 4669 742e 7844 6174 6143 6f6e   'mnFit.xDataCon
+00016880: 7461 696e 6572 2722 0a20 2020 2020 2020  tainer'".       
+00016890: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000168a0: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+000168b0: 6c20 3d20 6d6f 6465 6c0a 2020 2020 2020  l = model.      
+000168c0: 2020 2020 2020 7365 6c66 2e71 7569 6574        self.quiet
+000168d0: 203d 206f 7574 6572 2e71 7569 6574 0a20   = outer.quiet. 
+000168e0: 2020 2020 2020 2020 2020 2023 2075 7365             # use
+000168f0: 202d 3220 2a20 6c6f 6728 4c29 206f 6620   -2 * log(L) of 
+00016900: 4761 7573 7369 616e 2069 6e73 7465 6164  Gaussian instead
+00016910: 206f 6620 4368 6932 0a20 2020 2020 2020   of Chi2.       
+00016920: 2020 2020 2023 2020 286f 6e6c 7920 6469       #  (only di
+00016930: 6666 6572 656e 7420 6672 6f6d 2043 6869  fferent from Chi
+00016940: 3220 666f 7220 7061 7261 6d65 7465 722d  2 for parameter-
+00016950: 6465 7065 6e64 656e 7420 756e 6365 7274  dependent uncert
+00016960: 6169 6e74 6965 7329 0a20 2020 2020 2020  ainties).       
+00016970: 2020 2020 2073 656c 662e 7573 655f 6e65       self.use_ne
+00016980: 6732 6c6f 674c 203d 2075 7365 5f6e 6567  g2logL = use_neg
+00016990: 326c 6f67 4c0a 0a20 2020 2020 2020 2020  2logL..         
+000169a0: 2020 2023 2073 6574 2070 726f 7065 7220     # set proper 
+000169b0: 7369 676e 6174 7572 6520 6f66 206d 6f64  signature of mod
+000169c0: 656c 2066 756e 6374 696f 6e20 666f 7220  el function for 
+000169d0: 696d 696e 7569 740a 2020 2020 2020 2020  iminuit.        
+000169e0: 2020 2020 7365 6c66 2e70 6e61 6d73 203d      self.pnams =
+000169f0: 206f 7574 6572 2e70 6e61 6d73 0a20 2020   outer.pnams.   
+00016a00: 2020 2020 2020 2020 2073 656c 662e 6e70           self.np
+00016a10: 6172 203d 206f 7574 6572 2e6e 7061 720a  ar = outer.npar.
+00016a20: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
+00016a30: 616b 6520 6163 636f 756e 7420 6f66 2063  ake account of c
+00016a40: 6f6e 7374 7261 696e 7473 0a20 2020 2020  onstraints.     
+00016a50: 2020 2020 2020 2073 656c 662e 636f 6e73         self.cons
+00016a60: 7472 6169 6e74 7320 3d20 6f75 7465 722e  traints = outer.
+00016a70: 636f 6e73 7472 6169 6e74 730a 2020 2020  constraints.    
+00016a80: 2020 2020 2020 2020 7365 6c66 2e6e 636f          self.nco
+00016a90: 6e73 7472 6169 6e74 7320 3d20 6c65 6e28  nstraints = len(
+00016aa0: 7365 6c66 2e63 6f6e 7374 7261 696e 7473  self.constraints
+00016ab0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00016ac0: 6c66 2e6e 646f 6620 3d20 6c65 6e28 7365  lf.ndof = len(se
+00016ad0: 6c66 2e64 6174 612e 7829 202d 2073 656c  lf.data.x) - sel
+00016ae0: 662e 6e70 6172 202b 2073 656c 662e 6e63  f.npar + self.nc
+00016af0: 6f6e 7374 7261 696e 7473 202b 206f 7574  onstraints + out
+00016b00: 6572 2e6e 6669 7865 640a 0a20 2020 2020  er.nfixed..     
+00016b10: 2020 2020 2020 2023 2066 6c61 6720 746f         # flag to
+00016b20: 2063 6f6e 7472 6f6c 2066 696e 616c 2061   control final a
+00016b30: 6374 696f 6e73 2069 6e20 636f 7374 2066  ctions in cost f
+00016b40: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
+00016b50: 2020 2020 7365 6c66 2e66 696e 616c 5f63      self.final_c
+00016b60: 616c 6c20 3d20 4661 6c73 650a 0a20 2020  all = False..   
+00016b70: 2020 2020 2064 6566 205f 5f63 616c 6c5f       def __call_
+00016b80: 5f28 7365 6c66 2c20 2a70 6172 293a 0a20  _(self, *par):. 
+00016b90: 2020 2020 2020 2020 2020 2023 2063 616c             # cal
+00016ba0: 6c65 6420 6974 6572 6174 6976 656c 7920  led iteratively 
+00016bb0: 6279 206d 696e 7569 740a 0a20 2020 2020  by minuit..     
+00016bc0: 2020 2020 2020 2023 2063 6f73 7420 6675         # cost fu
+00016bd0: 6e63 7469 6f6e 2069 7320 6578 7465 6e64  nction is extend
+00016be0: 6564 2063 6869 323a 0a20 2020 2020 2020  ed chi2:.       
+00016bf0: 2020 2020 2023 2020 2061 6464 206e 6f72       #   add nor
+00016c00: 6d61 6c69 7a61 7469 6f6e 2074 6572 6d20  malization term 
+00016c10: 6966 2075 6e63 6572 7461 696e 7469 6573  if uncertainties
+00016c20: 2064 6570 656e 6420 6f6e 206d 6f64 656c   depend on model
+00016c30: 0a0a 2020 2020 2020 2020 2020 2020 6e6c  ..            nl
+00016c40: 4c32 203d 2030 2e30 2020 2320 696e 6974  L2 = 0.0  # init
+00016c50: 6961 6c69 7a65 202d 322a 6c6e 284c 290a  ialize -2*ln(L).
+00016c60: 2020 2020 2020 2020 2020 2020 2320 2066              #  f
+00016c70: 6972 7374 2c20 7461 6b65 2069 6e74 6f20  irst, take into 
+00016c80: 6163 636f 756e 7420 706f 7373 6962 6c65  account possible
+00016c90: 2070 6172 616d 6574 6572 2063 6f6e 7374   parameter const
+00016ca0: 7261 696e 7473 0a20 2020 2020 2020 2020  raints.         
+00016cb0: 2020 2069 6620 7365 6c66 2e6e 636f 6e73     if self.ncons
+00016cc0: 7472 6169 6e74 733a 0a20 2020 2020 2020  traints:.       
+00016cd0: 2020 2020 2020 2020 2066 6f72 2063 2069           for c i
+00016ce0: 6e20 7365 6c66 2e63 6f6e 7374 7261 696e  n self.constrain
+00016cf0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00016d00: 2020 2020 2020 2020 705f 6964 203d 2063          p_id = c
+00016d10: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00016d20: 2020 2020 2020 2020 7220 3d20 2870 6172          r = (par
+00016d30: 5b70 5f69 645d 202d 2063 5b31 5d29 202f  [p_id] - c[1]) /
+00016d40: 2063 5b32 5d0a 2020 2020 2020 2020 2020   c[2].          
+00016d50: 2020 2020 2020 2020 2020 6e6c 4c32 202b            nlL2 +
+00016d60: 3d20 7220 2a20 720a 0a20 2020 2020 2020  = r * r..       
+00016d70: 2020 2020 2023 2063 616c 6375 6c61 7465       # calculate
+00016d80: 2072 6573 6964 7561 6c20 6f66 2064 6174   residual of dat
+00016d90: 6120 7772 742e 206d 6f64 656c 0a20 2020  a wrt. model.   
+00016da0: 2020 2020 2020 2020 206d 6f64 656c 5f76           model_v
+00016db0: 616c 7565 7320 3d20 7365 6c66 2e6d 6f64  alues = self.mod
+00016dc0: 656c 2873 656c 662e 6461 7461 2e78 2c20  el(self.data.x, 
+00016dd0: 2a70 6172 290a 2020 2020 2020 2020 2020  *par).          
+00016de0: 2020 5f72 203d 2073 656c 662e 6461 7461    _r = self.data
+00016df0: 2e78 202d 206d 6f64 656c 5f76 616c 7565  .x - model_value
+00016e00: 730a 0a20 2020 2020 2020 2020 2020 2069  s..            i
+00016e10: 6620 7365 6c66 2e64 6174 612e 6e65 6564  f self.data.need
+00016e20: 735f 636f 7661 7269 616e 6365 3a0a 2020  s_covariance:.  
+00016e30: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00016e40: 2063 6865 636b 2069 6620 6d61 7472 6978   check if matrix
+00016e50: 206e 6565 6473 2072 6562 7569 6c64 696e   needs rebuildin
+00016e60: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+00016e70: 2020 6966 206e 6f74 2073 656c 662e 6461    if not self.da
+00016e80: 7461 2e6e 6565 6473 5f64 796e 616d 6963  ta.needs_dynamic
+00016e90: 4572 726f 7273 3a0a 2020 2020 2020 2020  Errors:.        
+00016ea0: 2020 2020 2020 2020 2020 2020 2320 7374              # st
+00016eb0: 6174 6963 2063 6f76 6172 6961 6e63 652c  atic covariance,
+00016ec0: 2075 7365 2069 7473 2069 6e76 6572 7365   use its inverse
+00016ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016ee0: 2020 2020 206e 6c4c 3220 2b3d 2066 6c6f       nlL2 += flo
+00016ef0: 6174 286e 702e 696e 6e65 7228 6e70 2e6d  at(np.inner(np.m
+00016f00: 6174 6d75 6c28 5f72 2c20 7365 6c66 2e64  atmul(_r, self.d
+00016f10: 6174 612e 6943 6f76 292c 205f 7229 290a  ata.iCov), _r)).
+00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f30: 2020 2020 2320 6964 656e 7469 6361 6c20      # identical 
+00016f40: 746f 2063 6c61 7373 6963 616c 2043 6869  to classical Chi
+00016f50: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
+00016f60: 2020 2020 2020 7365 6c66 2e67 6f66 203d        self.gof =
+00016f70: 206e 6c4c 320a 0a20 2020 2020 2020 2020   nlL2..         
+00016f80: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
+00016f90: 6479 6e61 6d69 6361 6c6c 7920 7265 6275  dynamically rebu
+00016fa0: 696c 6420 636f 7661 7269 616e 6365 206d  ild covariance m
+00016fb0: 6174 7269 780a 2020 2020 2020 2020 2020  atrix.          
+00016fc0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00016fd0: 6174 612e 5f72 6562 7569 6c64 5f43 6f76  ata._rebuild_Cov
+00016fe0: 2870 6172 290a 2020 2020 2020 2020 2020  (par).          
+00016ff0: 2020 2020 2020 2020 2020 2320 7573 6520            # use 
+00017000: 4368 6f6c 6573 6b79 2064 6563 6f6d 706f  Cholesky decompo
+00017010: 7369 746f 6e20 746f 2063 6f6d 7075 7465  siton to compute
+00017020: 2063 6869 3220 3d20 5f72 2e54 2028 565e   chi2 = _r.T (V^
+00017030: 2d31 2920 5f72 0a20 2020 2020 2020 2020  -1) _r.         
+00017040: 2020 2020 2020 2020 2020 204c 2c20 6973             L, is
+00017050: 5f6c 6f77 6572 203d 206c 696e 616c 672e  _lower = linalg.
+00017060: 6368 6f5f 6661 6374 6f72 2873 656c 662e  cho_factor(self.
+00017070: 6461 7461 2e63 6f76 2c20 6368 6563 6b5f  data.cov, check_
+00017080: 6669 6e69 7465 3d46 616c 7365 290a 2020  finite=False).  
+00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170a0: 2020 6e6c 4c32 202b 3d20 6e70 2e69 6e6e    nlL2 += np.inn
+000170b0: 6572 285f 722c 206c 696e 616c 672e 6368  er(_r, linalg.ch
+000170c0: 6f5f 736f 6c76 6528 284c 2c20 6973 5f6c  o_solve((L, is_l
+000170d0: 6f77 6572 292c 205f 7229 290a 2020 2020  ower), _r)).    
+000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170f0: 2320 7570 2074 6f20 6865 7265 2c20 6964  # up to here, id
+00017100: 656e 7469 6361 6c20 746f 2063 6c61 7373  entical to class
+00017110: 6963 616c 2043 6869 320a 2020 2020 2020  ical Chi2.      
+00017120: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00017130: 6c66 2e67 6f66 203d 206e 6c4c 320a 2020  lf.gof = nlL2.  
+00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017150: 2020 2320 7461 6b65 2069 6e74 6f20 6163    # take into ac
+00017160: 636f 756e 7420 7061 7261 6d65 7465 722d  count parameter-
+00017170: 6465 7065 6e64 656e 7420 6e6f 726d 616c  dependent normal
+00017180: 6973 6174 696f 6e20 7465 726d 0a20 2020  isation term.   
+00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171a0: 2069 6620 7365 6c66 2e75 7365 5f6e 6567   if self.use_neg
+000171b0: 326c 6f67 4c3a 0a20 2020 2020 2020 2020  2logL:.         
+000171c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000171d0: 2020 6661 7374 2063 616c 6375 6c61 7469    fast calculati
+000171e0: 6f6e 206f 6620 6465 7465 726d 696e 616e  on of determinan
+000171f0: 7420 6465 7428 5629 2066 726f 6d20 4368  t det(V) from Ch
+00017200: 6f6c 6573 6b79 2066 6163 746f 720a 2020  olesky factor.  
+00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017220: 2020 2020 2020 6e6c 4c32 202b 3d20 322e        nlL2 += 2.
+00017230: 3020 2a20 6e70 2e73 756d 286e 702e 6c6f  0 * np.sum(np.lo
+00017240: 6728 6e70 2e64 6961 676f 6e61 6c28 4c29  g(np.diagonal(L)
+00017250: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+00017260: 656c 7365 3a20 2023 2066 6173 7420 6361  else:  # fast ca
+00017270: 6c63 756c 6174 696f 6e20 666f 7220 7369  lculation for si
+00017280: 6d70 6c65 2065 7272 6f72 730a 2020 2020  mple errors.    
+00017290: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
+000172a0: 6563 6b20 6966 2065 7272 6f72 7320 6e65  eck if errors ne
+000172b0: 6564 7320 7265 6361 6c63 756c 6174 696e  eds recalculatin
+000172c0: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+000172d0: 2020 6966 2073 656c 662e 6461 7461 2e6e    if self.data.n
+000172e0: 6565 6473 5f64 796e 616d 6963 4572 726f  eeds_dynamicErro
+000172f0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
+00017300: 2020 2020 2020 2020 7365 6c66 2e64 6174          self.dat
+00017310: 612e 5f72 6562 7569 6c64 5f45 7272 3228  a._rebuild_Err2(
+00017320: 7061 7229 0a20 2020 2020 2020 2020 2020  par).           
+00017330: 2020 2020 2020 2020 206e 6c4c 3220 2b3d           nlL2 +=
+00017340: 206e 702e 7375 6d28 5f72 202a 205f 7220   np.sum(_r * _r 
+00017350: 2f20 7365 6c66 2e64 6174 612e 6572 7232  / self.data.err2
+00017360: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017370: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00017380: 2020 2020 2020 2020 2020 2020 6e6c 4c32              nlL2
+00017390: 202b 3d20 6e70 2e73 756d 285f 7220 2a20   += np.sum(_r * 
+000173a0: 5f72 202a 2073 656c 662e 6461 7461 2e69  _r * self.data.i
+000173b0: 4572 7232 290a 0a20 2020 2020 2020 2020  Err2)..         
+000173c0: 2020 2020 2020 2023 2074 6869 7320 6973         # this is
+000173d0: 2069 6465 6e74 6963 616c 2074 6f20 636c   identical to cl
+000173e0: 6173 7369 6361 6c20 4368 6932 0a20 2020  assical Chi2.   
+000173f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00017400: 662e 676f 6620 3d20 6e6c 4c32 0a0a 2020  f.gof = nlL2..  
+00017410: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00017420: 6164 6420 7061 7261 6d65 7465 722d 6465  add parameter-de
+00017430: 7065 6e64 656e 7420 6e6f 726d 616c 697a  pendent normaliz
+00017440: 6174 696f 6e20 7465 726d 2069 6620 6e65  ation term if ne
+00017450: 6564 6564 2061 6e64 2077 616e 7465 640a  eded and wanted.
+00017460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017470: 6966 2073 656c 662e 6461 7461 2e6e 6565  if self.data.nee
+00017480: 6473 5f64 796e 616d 6963 4572 726f 7273  ds_dynamicErrors
+00017490: 2061 6e64 2073 656c 662e 7573 655f 6e65   and self.use_ne
+000174a0: 6732 6c6f 674c 3a0a 2020 2020 2020 2020  g2logL:.        
+000174b0: 2020 2020 2020 2020 2020 2020 6e6c 4c32              nlL2
+000174c0: 202b 3d20 6e70 2e73 756d 286e 702e 6c6f   += np.sum(np.lo
+000174d0: 6728 7365 6c66 2e64 6174 612e 6572 7232  g(self.data.err2
+000174e0: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+000174f0: 2320 7072 6f76 6964 6520 6d6f 6465 6c20  # provide model 
+00017500: 7661 6c75 6573 2074 6f20 6461 7461 206f  values to data o
+00017510: 626a 6563 740a 2020 2020 2020 2020 2020  bject.          
+00017520: 2020 7365 6c66 2e64 6174 612e 6d6f 6465    self.data.mode
+00017530: 6c5f 7661 6c75 6573 203d 206d 6f64 656c  l_values = model
+00017540: 5f76 616c 7565 730a 0a20 2020 2020 2020  _values..       
+00017550: 2020 2020 2072 6574 7572 6e20 6e6c 4c32       return nlL2
+00017560: 0a0a 2020 2020 230a 2020 2020 2320 2d2d  ..    #.    # --
+00017570: 2d20 7370 6563 6961 6c20 636f 6465 2066  - special code f
+00017580: 6f72 2068 6973 746f 6772 616d 2046 6974  or histogram Fit
+00017590: 0a20 2020 2023 0a0a 2020 2020 6465 6620  .    #..    def 
+000175a0: 7365 745f 684f 7074 696f 6e73 280a 2020  set_hOptions(.  
+000175b0: 2020 2020 2020 7365 6c66 2c20 7275 6e5f        self, run_
+000175c0: 6d69 6e6f 733d 4e6f 6e65 2c20 7573 655f  minos=None, use_
+000175d0: 4761 7573 7341 7070 726f 783d 4e6f 6e65  GaussApprox=None
+000175e0: 2c20 6669 745f 6465 6e73 6974 793d 4e6f  , fit_density=No
+000175f0: 6e65 2c20 7175 6965 743d 4e6f 6e65 0a20  ne, quiet=None. 
+00017600: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+00017610: 2244 6566 696e 6520 6d6e 4669 7420 6f70  "Define mnFit op
+00017620: 7469 6f6e 730a 0a20 2020 2020 2020 2041  tions..        A
+00017630: 7267 733a 0a20 2020 2020 2020 2020 2d20  rgs:.         - 
+00017640: 7275 6e20 6d69 6e6f 7320 656c 7365 2064  run minos else d
+00017650: 6f6e 2a74 2072 756e 206d 696e 6f73 0a20  on*t run minos. 
+00017660: 2020 2020 2020 2020 2d20 7573 6520 4761          - use Ga
+00017670: 7573 7369 616e 2041 7070 726f 7869 6d61  ussian Approxima
+00017680: 7469 6f6e 206f 6620 506f 6973 736f 6e20  tion of Poisson 
+00017690: 6469 7374 7269 6275 7469 6f6e 0a20 2020  distribution.   
+000176a0: 2020 2020 2020 2d20 646f 6e2a 7420 7072        - don*t pr
+000176b0: 6f76 6964 6520 7072 696e 746f 7574 2065  ovide printout e
+000176c0: 6c73 6520 7665 7262 6f73 6520 7072 696e  lse verbose prin
+000176d0: 746f 7574 0a20 2020 2020 2020 2022 2222  tout.        """
+000176e0: 0a20 2020 2020 2020 2069 6620 7275 6e5f  .        if run_
+000176f0: 6d69 6e6f 7320 6973 206e 6f74 204e 6f6e  minos is not Non
+00017700: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00017710: 656c 662e 7275 6e5f 6d69 6e6f 7320 3d20  elf.run_minos = 
+00017720: 7275 6e5f 6d69 6e6f 730a 2020 2020 2020  run_minos.      
+00017730: 2020 2020 2020 7365 6c66 2e6f 7074 696f        self.optio
+00017740: 6e73 5b22 7275 6e5f 6d69 6e6f 7322 5d5b  ns["run_minos"][
+00017750: 305d 203d 2069 6e74 2872 756e 5f6d 696e  0] = int(run_min
+00017760: 6f73 290a 2020 2020 2020 2020 6966 2075  os).        if u
+00017770: 7365 5f47 6175 7373 4170 7072 6f78 2069  se_GaussApprox i
+00017780: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00017790: 2020 2020 2020 2020 7365 6c66 2e75 7365          self.use
+000177a0: 5f47 6175 7373 4170 7072 6f78 203d 2075  _GaussApprox = u
+000177b0: 7365 5f47 6175 7373 4170 7072 6f78 0a20  se_GaussApprox. 
+000177c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000177d0: 6f70 7469 6f6e 735b 2275 7365 5f47 6175  options["use_Gau
+000177e0: 7373 4170 7072 6f78 225d 5b30 5d20 3d20  ssApprox"][0] = 
+000177f0: 696e 7428 7573 655f 4761 7573 7341 7070  int(use_GaussApp
+00017800: 726f 7829 0a20 2020 2020 2020 2069 6620  rox).        if 
+00017810: 6669 745f 6465 6e73 6974 7920 6973 206e  fit_density is n
+00017820: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00017830: 2020 2020 2073 656c 662e 6669 745f 6465       self.fit_de
+00017840: 6e73 6974 7920 3d20 6669 745f 6465 6e73  nsity = fit_dens
+00017850: 6974 790a 2020 2020 2020 2020 2020 2020  ity.            
+00017860: 7365 6c66 2e6f 7074 696f 6e73 5b22 6669  self.options["fi
+00017870: 745f 6465 6e73 6974 7922 5d5b 305d 203d  t_density"][0] =
+00017880: 2069 6e74 2866 6974 5f64 656e 7369 7479   int(fit_density
+00017890: 290a 2020 2020 2020 2020 6966 2071 7569  ).        if qui
+000178a0: 6574 2069 7320 6e6f 7420 4e6f 6e65 3a0a  et is not None:.
+000178b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000178c0: 2e71 7569 6574 203d 2071 7569 6574 0a0a  .quiet = quiet..
+000178d0: 2020 2020 6465 6620 696e 6974 5f68 4461      def init_hDa
+000178e0: 7461 2873 656c 662c 2062 696e 5f63 6f6e  ta(self, bin_con
+000178f0: 7465 6e74 732c 2062 696e 5f65 6467 6573  tents, bin_edges
+00017900: 2c20 4465 6c74 614d 753d 4e6f 6e65 293a  , DeltaMu=None):
+00017910: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00017920: 2020 2020 2069 6e69 7469 616c 697a 6520       initialize 
+00017930: 6869 7374 6f67 7261 6d20 6461 7461 206f  histogram data o
+00017940: 626a 6563 740a 0a20 2020 2020 2020 2041  bject..        A
+00017950: 7267 733a 0a20 2020 2020 2020 202d 2062  rgs:.        - b
+00017960: 696e 5f63 6f6e 7465 6e74 733a 2061 7272  in_contents: arr
+00017970: 6179 206f 6620 666c 6f61 7473 0a20 2020  ay of floats.   
+00017980: 2020 2020 202d 2062 696e 5f65 6467 6573       - bin_edges
+00017990: 3a20 6172 7261 7920 6f66 206c 656e 6774  : array of lengt
+000179a0: 6820 6c65 6e28 6269 6e5f 636f 6e74 656e  h len(bin_conten
+000179b0: 7473 292a 310a 2020 2020 2020 2020 2d20  ts)*1.        - 
+000179c0: 4465 6c74 614d 753a 2073 6869 6674 2069  DeltaMu: shift i
+000179d0: 6e20 6d65 616e 2028 4465 6c74 6120 6d75  n mean (Delta mu
+000179e0: 2920 7665 7273 7573 206c 616d 6264 610a  ) versus lambda.
+000179f0: 2020 2020 2020 2020 6f66 2050 6f69 7373          of Poiss
+00017a00: 6f6e 2064 6973 7472 6962 7574 696f 6e0a  on distribution.
+00017a10: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00017a20: 2020 2020 2023 2063 7265 6174 6520 6461       # create da
+00017a30: 7461 206f 626a 6563 7420 616e 6420 7061  ta object and pa
+00017a40: 7373 2061 6c6c 2069 6e70 7574 2061 7267  ss all input arg
+00017a50: 756d 656e 7473 0a20 2020 2020 2020 2073  uments.        s
+00017a60: 656c 662e 6844 6174 6120 3d20 7365 6c66  elf.hData = self
+00017a70: 2e68 6973 7444 6174 6143 6f6e 7461 696e  .histDataContain
+00017a80: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
+00017a90: 7365 6c66 2c20 6269 6e5f 636f 6e74 656e  self, bin_conten
+00017aa0: 7473 2c20 6269 6e5f 6564 6765 732c 2044  ts, bin_edges, D
+00017ab0: 656c 7461 4d75 2c20 7175 6965 743d 7365  eltaMu, quiet=se
+00017ac0: 6c66 2e71 7569 6574 0a20 2020 2020 2020  lf.quiet.       
+00017ad0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+00017ae0: 6461 7461 203d 2073 656c 662e 6844 6174  data = self.hDat
+00017af0: 610a 0a20 2020 2064 6566 2069 6e69 745f  a..    def init_
+00017b00: 6846 6974 280a 2020 2020 2020 2020 7365  hFit(.        se
+00017b10: 6c66 2c0a 2020 2020 2020 2020 6d6f 6465  lf,.        mode
+00017b20: 6c2c 0a20 2020 2020 2020 206d 6f64 656c  l,.        model
+00017b30: 5f6b 7761 7267 733d 4e6f 6e65 2c0a 2020  _kwargs=None,.  
+00017b40: 2020 2020 2020 7030 3d4e 6f6e 652c 0a20        p0=None,. 
+00017b50: 2020 2020 2020 2064 7030 3d4e 6f6e 652c         dp0=None,
+00017b60: 0a20 2020 2020 2020 2063 6f6e 7374 7261  .        constra
+00017b70: 696e 7473 3d4e 6f6e 652c 0a20 2020 2020  ints=None,.     
+00017b80: 2020 2066 6978 5061 7273 3d4e 6f6e 652c     fixPars=None,
+00017b90: 0a20 2020 2020 2020 206c 696d 6974 733d  .        limits=
+00017ba0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00017bb0: 2020 2020 2022 2222 696e 6974 6961 6c69       """initiali
+00017bc0: 7a65 2066 6974 206f 626a 6563 740a 0a20  ze fit object.. 
+00017bd0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00017be0: 2020 2020 2020 202d 206d 6f64 656c 3a20         - model: 
+00017bf0: 6d6f 6465 6c20 6465 6e73 6974 7920 6675  model density fu
+00017c00: 6e63 7469 6f6e 2066 2878 3b20 5c2a 7061  nction f(x; \*pa
+00017c10: 7229 0a20 2020 2020 2020 2020 202d 206d  r).          - m
+00017c20: 6f64 656c 5f6b 7761 7267 733a 206f 7074  odel_kwargs: opt
+00017c30: 696f 6e61 6c2c 2066 6974 2070 6172 616d  ional, fit param
+00017c40: 6574 6572 7320 6966 206e 6f74 2066 726f  eters if not fro
+00017c50: 6d20 6d6f 6465 6c20 7369 676e 6174 7572  m model signatur
+00017c60: 650a 2020 2020 2020 2020 2020 2d20 7030  e.          - p0
+00017c70: 3a20 6e70 2d61 7272 6179 206f 6620 666c  : np-array of fl
+00017c80: 6f61 7473 2c20 696e 6974 6961 6c20 7061  oats, initial pa
+00017c90: 7261 6d65 7465 7220 7661 6c75 6573 0a20  rameter values. 
+00017ca0: 2020 2020 2020 2020 202d 2064 7030 3a20           - dp0: 
+00017cb0: 6172 7261 792d 6c69 6b65 2c20 696e 6974  array-like, init
+00017cc0: 6961 6c20 6775 6573 7320 6f66 2070 6172  ial guess of par
+00017cd0: 616d 6574 6572 2075 6e63 6572 7461 696e  ameter uncertain
+00017ce0: 7469 6573 2028 6f70 7469 6f6e 616c 290a  ties (optional).
+00017cf0: 2020 2020 2020 2020 2020 2d20 636f 6e73            - cons
+00017d00: 7472 6169 6e74 733a 2028 6e65 7374 6564  traints: (nested
+00017d10: 2920 6c69 7374 2873 293a 205b 7061 7261  ) list(s): [para
+00017d20: 6d65 7465 7220 6e61 6d65 2c20 7661 6c75  meter name, valu
+00017d30: 652c 2075 6e63 6572 7461 696e 7479 5d0a  e, uncertainty].
+00017d40: 2020 2020 2020 2020 2020 2020 6f72 205b              or [
+00017d50: 7061 7261 6d65 7465 7220 696e 6465 782c  parameter index,
+00017d60: 2076 616c 7565 2c20 756e 6365 7274 6169   value, uncertai
+00017d70: 6e74 795d 0a20 2020 2020 2020 2020 202d  nty].          -
+00017d80: 2066 6978 2070 6172 616d 6574 6572 2873   fix parameter(s
+00017d90: 2920 696e 2066 6974 3a20 6c69 7374 206f  ) in fit: list o
+00017da0: 6620 7061 7261 6d65 7465 7220 6e61 6d65  f parameter name
+00017db0: 7320 6f72 2069 6e64 6963 6573 0a20 2020  s or indices.   
+00017dc0: 2020 2020 2020 202d 206c 696d 6974 733a         - limits:
+00017dd0: 2028 6e65 7374 6564 2920 6c69 7374 2873   (nested) list(s
+00017de0: 293a 205b 7061 7261 6d65 7465 7220 6e61  ): [parameter na
+00017df0: 6d65 2c20 6d69 6e2c 206d 6178 5d0a 2020  me, min, max].  
+00017e00: 2020 2020 2020 2020 2020 6f72 205b 7061            or [pa
+00017e10: 7261 6d65 7465 7220 696e 6465 782c 206d  rameter index, m
+00017e20: 696e 2c20 6d61 785d 0a20 2020 2020 2020  in, max].       
+00017e30: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+00017e40: 2073 656c 662e 6844 6174 6120 6973 204e   self.hData is N
+00017e50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00017e60: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00017e70: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00017e80: 2020 2022 2021 2121 206d 6e46 6974 2e69     " !!! mnFit.i
+00017e90: 6e69 745f 6846 6974 3a20 6e6f 2064 6174  nit_hFit: no dat
+00017ea0: 6120 6f62 6a65 6374 2064 6566 696e 6564  a object defined
+00017eb0: 202d 2063 616c 6c20 696e 6974 5f64 6174   - call init_dat
+00017ec0: 6128 2922 0a20 2020 2020 2020 2020 2020  a()".           
+00017ed0: 2029 0a0a 2020 2020 2020 2020 2320 6765   )..        # ge
+00017ee0: 7420 7061 7261 6d65 7465 7273 206f 6620  t parameters of 
+00017ef0: 6d6f 6465 6c20 6675 6e63 7469 6f6e 2074  model function t
+00017f00: 6f20 7365 7420 7374 6172 7420 7661 6c75  o set start valu
+00017f10: 6573 2066 6f72 2066 6974 0a20 2020 2020  es for fit.     
+00017f20: 2020 2069 6620 6d6f 6465 6c5f 6b77 6172     if model_kwar
+00017f30: 6773 2069 7320 4e6f 6e65 3a0a 2020 2020  gs is None:.    
+00017f40: 2020 2020 2020 2020 6172 6773 2c20 6d6f          args, mo
+00017f50: 6465 6c5f 6b77 6172 6773 203d 2067 6574  del_kwargs = get
+00017f60: 5f66 756e 6374 696f 6e53 6967 6e61 7475  _functionSignatu
+00017f70: 7265 286d 6f64 656c 290a 0a20 2020 2020  re(model)..     
+00017f80: 2020 2070 6172 203d 2028 6d6f 6465 6c5f     par = (model_
+00017f90: 6b77 6172 6773 2c20 7030 2c20 6470 302c  kwargs, p0, dp0,
+00017fa0: 2063 6f6e 7374 7261 696e 7473 2c20 6669   constraints, fi
+00017fb0: 7850 6172 732c 206c 696d 6974 7329 0a20  xPars, limits). 
+00017fc0: 2020 2020 2020 2073 656c 662e 5f73 6574         self._set
+00017fd0: 7570 4669 7450 6172 616d 6574 6572 7328  upFitParameters(
+00017fe0: 2a70 6172 290a 0a20 2020 2020 2020 2023  *par)..        #
+00017ff0: 2063 7265 6174 6520 636f 7374 2066 756e   create cost fun
+00018000: 6374 696f 6e0a 2020 2020 2020 2020 7365  ction.        se
+00018010: 6c66 2e63 6f73 7466 203d 2073 656c 662e  lf.costf = self.
+00018020: 6843 6f73 7428 0a20 2020 2020 2020 2020  hCost(.         
+00018030: 2020 2073 656c 662c 206d 6f64 656c 2c20     self, model, 
+00018040: 7573 655f 4761 7573 7341 7070 726f 783d  use_GaussApprox=
+00018050: 7365 6c66 2e75 7365 5f47 6175 7373 4170  self.use_GaussAp
+00018060: 7072 6f78 2c20 6465 6e73 6974 793d 7365  prox, density=se
+00018070: 6c66 2e66 6974 5f64 656e 7369 7479 0a20  lf.fit_density. 
+00018080: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00018090: 2073 656c 662e 5f73 6574 7570 4d69 6e75   self._setupMinu
+000180a0: 6974 286d 6f64 656c 5f6b 7761 7267 7329  it(model_kwargs)
+000180b0: 0a0a 2020 2020 636c 6173 7320 6869 7374  ..    class hist
+000180c0: 4461 7461 436f 6e74 6169 6e65 723a 0a20  DataContainer:. 
+000180d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000180e0: 2020 2043 6f6e 7461 696e 6572 2066 6f72     Container for
+000180f0: 2048 6973 746f 6772 616d 2064 6174 610a   Histogram data.
+00018100: 0a20 2020 2020 2020 2044 6174 6120 4d65  .        Data Me
+00018110: 6d62 6572 733a 0a0a 2020 2020 2020 2020  mbers:..        
+00018120: 2d20 636f 6e74 656e 7473 2c20 6172 7261  - contents, arra
+00018130: 7920 6f66 2066 6c6f 6174 733a 2062 696e  y of floats: bin
+00018140: 2063 6f6e 7465 6e74 730a 2020 2020 2020   contents.      
+00018150: 2020 2d20 6564 6765 732c 2061 7272 6179    - edges, array
+00018160: 206f 6620 666c 6f61 7473 3a20 6269 6e20   of floats: bin 
+00018170: 6564 6765 7320 286e 6269 6e73 2b31 2076  edges (nbins+1 v
+00018180: 616c 7565 7329 0a0a 2020 2020 2020 2020  alues)..        
+00018190: 6361 6c63 756c 6174 6564 2066 726f 6d20  calculated from 
+000181a0: 696e 7075 743a 0a0a 2020 2020 2020 2020  input:..        
+000181b0: 2d20 6e62 696e 733a 206e 756d 6265 7220  - nbins: number 
+000181c0: 6f66 2062 696e 730a 2020 2020 2020 2020  of bins.        
+000181d0: 2d20 6c65 6674 733a 206c 6566 7420 6564  - lefts: left ed
+000181e0: 6765 730a 2020 2020 2020 2020 2d20 7269  ges.        - ri
+000181f0: 6768 7473 3a20 7269 6768 7420 6564 6765  ghts: right edge
+00018200: 730a 2020 2020 2020 2020 2d20 6365 6e74  s.        - cent
+00018210: 6572 733a 2062 696e 2063 656e 7465 7273  ers: bin centers
+00018220: 0a20 2020 2020 2020 202d 2077 6964 7468  .        - width
+00018230: 733a 2062 696e 2077 6964 7468 730a 2020  s: bin widths.  
+00018240: 2020 2020 2020 2d20 4e74 6f74 3a20 746f        - Ntot: to
+00018250: 7461 6c20 6e75 6d62 6572 206f 6620 656e  tal number of en
+00018260: 7472 6965 732c 2075 7365 6420 746f 206e  tries, used to n
+00018270: 6f72 6d61 6c69 7a65 2070 726f 6261 7469  ormalize probati
+00018280: 6c69 7479 2064 656e 7369 7479 0a0a 2020  lity density..  
+00018290: 2020 2020 2020 6176 6169 6c61 626c 6520        available 
+000182a0: 6166 7465 7220 636f 6d70 6c65 7469 6f6e  after completion
+000182b0: 206f 6620 6669 743a 0a0a 2020 2020 2020   of fit:..      
+000182c0: 2020 2d20 6d6f 6465 6c5f 7661 6c75 6573    - model_values
+000182d0: 3a20 6269 6e20 636f 6e74 656e 7473 2066  : bin contents f
+000182e0: 726f 6d20 6265 7374 2d66 6974 206d 6f64  rom best-fit mod
+000182f0: 656c 0a0a 2020 2020 2020 2020 4d65 7468  el..        Meth
+00018300: 6f64 733a 0a0a 2020 2020 2020 2020 2d20  ods:..        - 
+00018310: 706c 6f74 2829 3a20 7265 7475 726e 2066  plot(): return f
+00018320: 6967 7572 6520 7769 7468 2068 6973 746f  igure with histo
+00018330: 6772 616d 206f 6620 6461 7461 2061 6e64  gram of data and
+00018340: 2075 6e63 6572 7461 696e 7469 6573 0a20   uncertainties. 
+00018350: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00018360: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00018370: 2873 656c 662c 206f 7574 6572 2c20 6269  (self, outer, bi
+00018380: 6e5f 636f 6e74 656e 7473 2c20 6269 6e5f  n_contents, bin_
+00018390: 6564 6765 732c 2044 656c 7461 4d75 3d4e  edges, DeltaMu=N
+000183a0: 6f6e 652c 2071 7569 6574 3d54 7275 6529  one, quiet=True)
+000183b0: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
+000183c0: 220a 2020 2020 2020 2020 2020 2020 696e  ".            in
+000183d0: 6974 6961 6c69 7a65 2068 6973 746f 6772  itialize histogr
+000183e0: 616d 2044 6174 610a 0a20 2020 2020 2020  am Data..       
+000183f0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00018400: 2020 2020 2020 202d 2062 696e 5f63 6f6e         - bin_con
+00018410: 7465 6e74 733a 2061 7272 6179 206f 6620  tents: array of 
+00018420: 666c 6f61 7473 0a20 2020 2020 2020 2020  floats.         
+00018430: 2020 202d 2062 696e 5f65 6467 6573 3a20     - bin_edges: 
+00018440: 6172 7261 7920 6f66 206c 656e 6774 6820  array of length 
+00018450: 6c65 6e28 6269 6e5f 636f 6e74 656e 7473  len(bin_contents
+00018460: 292a 310a 2020 2020 2020 2020 2020 2020  )*1.            
+00018470: 2d20 4465 6c74 614d 753a 2061 7272 6179  - DeltaMu: array
+00018480: 206f 6620 666c 6f61 7473 2c20 7368 6966   of floats, shif
+00018490: 7420 6f66 206d 6561 6e20 6d75 2076 732e  t of mean mu vs.
+000184a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000184b0: 206c 616d 6264 6120 6f66 2050 6f69 7373   lambda of Poiss
+000184c0: 6f6e 2064 6973 7472 6962 7574 696f 6e2c  on distribution,
+000184d0: 2044 656c 7461 4d75 203d 206d 752d 6c61   DeltaMu = mu-la
+000184e0: 6d62 6461 0a20 2020 2020 2020 2020 2020  mbda.           
+000184f0: 202d 2071 7569 6574 3a20 626f 6f6c 6561   - quiet: boolea
+00018500: 6e2c 2063 6f6e 7472 6f6c 7320 7072 696e  n, controls prin
+00018510: 7465 6420 6f75 7470 7574 0a0a 2020 2020  ted output..    
+00018520: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+00018530: 2020 2020 2020 2020 2073 656c 662e 6f75           self.ou
+00018540: 7465 7220 3d20 6f75 7465 720a 2020 2020  ter = outer.    
+00018550: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00018560: 7465 6e74 7320 3d20 6269 6e5f 636f 6e74  tents = bin_cont
+00018570: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
+00018580: 2073 656c 662e 6e62 696e 7320 3d20 6c65   self.nbins = le
+00018590: 6e28 6269 6e5f 636f 6e74 656e 7473 290a  n(bin_contents).
+000185a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000185b0: 2e64 6c65 6e67 7468 203d 2073 656c 662e  .dlength = self.
+000185c0: 6e62 696e 730a 2020 2020 2020 2020 2020  nbins.          
+000185d0: 2020 7365 6c66 2e4e 746f 7420 3d20 6e70    self.Ntot = np
+000185e0: 2e73 756d 2862 696e 5f63 6f6e 7465 6e74  .sum(bin_content
+000185f0: 7329 0a20 2020 2020 2020 2020 2020 2073  s).            s
+00018600: 656c 662e 6564 6765 7320 3d20 6269 6e5f  elf.edges = bin_
+00018610: 6564 6765 730a 2020 2020 2020 2020 2020  edges.          
+00018620: 2020 6966 2044 656c 7461 4d75 2069 7320    if DeltaMu is 
+00018630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00018640: 2020 2020 2020 7365 6c66 2e44 656c 7461        self.Delta
+00018650: 4d75 203d 206e 702e 7a65 726f 7328 6c65  Mu = np.zeros(le
+00018660: 6e28 6269 6e5f 636f 6e74 656e 7473 2929  n(bin_contents))
+00018670: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00018680: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00018690: 2020 2073 656c 662e 4465 6c74 6120 3d20     self.Delta = 
+000186a0: 4465 6c74 614d 750a 2020 2020 2020 2020  DeltaMu.        
+000186b0: 2020 2020 230a 2020 2020 2020 2020 2020      #.          
+000186c0: 2020 7365 6c66 2e6c 6566 7473 203d 2073    self.lefts = s
+000186d0: 656c 662e 6564 6765 735b 3a2d 315d 0a20  elf.edges[:-1]. 
+000186e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000186f0: 7269 6768 7473 203d 2073 656c 662e 6564  rights = self.ed
+00018700: 6765 735b 313a 5d0a 2020 2020 2020 2020  ges[1:].        
+00018710: 2020 2020 7365 6c66 2e63 656e 7465 7273      self.centers
+00018720: 203d 2028 7365 6c66 2e72 6967 6874 7320   = (self.rights 
+00018730: 2b20 7365 6c66 2e6c 6566 7473 2920 2f20  + self.lefts) / 
+00018740: 322e 300a 2020 2020 2020 2020 2020 2020  2.0.            
+00018750: 7365 6c66 2e77 6964 7468 7320 3d20 7365  self.widths = se
+00018760: 6c66 2e72 6967 6874 7320 2d20 7365 6c66  lf.rights - self
+00018770: 2e6c 6566 7473 0a20 2020 2020 2020 2020  .lefts.         
+00018780: 2020 2023 2066 6c61 6720 746f 2063 6f6e     # flag to con
+00018790: 7472 6f6c 2066 696e 616c 2061 6374 696f  trol final actio
+000187a0: 6e73 2069 6e20 636f 7374 2066 756e 6374  ns in cost funct
+000187b0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000187c0: 7365 6c66 2e66 696e 616c 5f63 616c 6c20  self.final_call 
+000187d0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+000187e0: 2020 2020 7365 6c66 2e6d 6f64 656c 5f76      self.model_v
+000187f0: 616c 7565 7320 3d20 4e6f 6e65 0a0a 2020  alues = None..  
+00018800: 2020 2020 2020 6465 6620 706c 6f74 280a        def plot(.
+00018810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018820: 2c0a 2020 2020 2020 2020 2020 2020 6e75  ,.            nu
+00018830: 6d3d 2268 6973 7444 6174 6120 616e 6420  m="histData and 
+00018840: 4d6f 6465 6c22 2c0a 2020 2020 2020 2020  Model",.        
+00018850: 2020 2020 6669 6773 697a 653d 2837 2e35      figsize=(7.5
+00018860: 2c20 362e 3529 2c0a 2020 2020 2020 2020  , 6.5),.        
+00018870: 2020 2020 6461 7461 5f6c 6162 656c 3d22      data_label="
+00018880: 4269 6e6e 6564 2064 6174 6122 2c0a 2020  Binned data",.  
+00018890: 2020 2020 2020 2020 2020 706c 6f74 5f72            plot_r
+000188a0: 6573 6964 7561 6c3d 4661 6c73 652c 0a20  esidual=False,. 
+000188b0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+000188c0: 2020 2020 2020 2222 2272 6574 7572 6e20        """return 
+000188d0: 6669 6775 7265 2077 6974 6820 6869 7374  figure with hist
+000188e0: 6f67 7261 6d20 6461 7461 2061 6e64 2075  ogram data and u
+000188f0: 6e63 6572 7461 696e 7469 6573 2222 220a  ncertainties""".
+00018900: 0a20 2020 2020 2020 2020 2020 2077 203d  .            w =
+00018910: 2073 656c 662e 6564 6765 735b 313a 5d20   self.edges[1:] 
+00018920: 2d20 7365 6c66 2e65 6467 6573 5b3a 2d31  - self.edges[:-1
+00018930: 5d0a 2020 2020 2020 2020 2020 2020 6669  ].            fi
+00018940: 6720 3d20 706c 742e 6669 6775 7265 286e  g = plt.figure(n
+00018950: 756d 3d6e 756d 2c20 6669 6773 697a 653d  um=num, figsize=
+00018960: 6669 6773 697a 6529 0a20 2020 2020 2020  figsize).       
+00018970: 2020 2020 2069 6620 7365 6c66 2e6d 6f64       if self.mod
+00018980: 656c 5f76 616c 7565 7320 6973 206e 6f74  el_values is not
+00018990: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000189a0: 2020 2020 2020 2069 6620 706c 6f74 5f72         if plot_r
+000189b0: 6573 6964 7561 6c3a 0a20 2020 2020 2020  esidual:.       
+000189c0: 2020 2020 2020 2020 2020 2020 206d 636f               mco
+000189d0: 6e74 7320 3d20 6e70 2e7a 6572 6f73 2873  nts = np.zeros(s
+000189e0: 656c 662e 6e62 696e 7329 0a20 2020 2020  elf.nbins).     
+000189f0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00018a00: 636f 6e74 7320 3d20 7365 6c66 2e63 6f6e  conts = self.con
+00018a10: 7465 6e74 7320 2d20 7365 6c66 2e6d 6f64  tents - self.mod
+00018a20: 656c 5f76 616c 7565 730a 2020 2020 2020  el_values.      
+00018a30: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00018a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a50: 2020 2020 6d63 6f6e 7473 203d 2073 656c      mconts = sel
+00018a60: 662e 6d6f 6465 6c5f 7661 6c75 6573 0a20  f.model_values. 
+00018a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a80: 2020 2062 636f 6e74 7320 3d20 7365 6c66     bconts = self
+00018a90: 2e63 6f6e 7465 6e74 730a 2020 2020 2020  .contents.      
+00018aa0: 2020 2020 2020 706c 742e 6261 7228 0a20        plt.bar(. 
+00018ab0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018ac0: 656c 662e 6365 6e74 6572 732c 0a20 2020  elf.centers,.   
+00018ad0: 2020 2020 2020 2020 2020 2020 2062 636f               bco
+00018ae0: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
+00018af0: 2020 2020 2061 6c69 676e 3d22 6365 6e74       align="cent
+00018b00: 6572 222c 0a20 2020 2020 2020 2020 2020  er",.           
+00018b10: 2020 2020 2077 6964 7468 3d77 2c0a 2020       width=w,.  
+00018b20: 2020 2020 2020 2020 2020 2020 2020 6661                fa
+00018b30: 6365 636f 6c6f 723d 2263 6164 6574 626c  cecolor="cadetbl
+00018b40: 7565 222c 0a20 2020 2020 2020 2020 2020  ue",.           
+00018b50: 2020 2020 2065 6467 6563 6f6c 6f72 3d22       edgecolor="
+00018b60: 6461 726b 626c 7565 222c 0a20 2020 2020  darkblue",.     
+00018b70: 2020 2020 2020 2020 2020 2061 6c70 6861             alpha
+00018b80: 3d30 2e36 362c 0a20 2020 2020 2020 2020  =0.66,.         
+00018b90: 2020 2020 2020 206c 6162 656c 3d64 6174         label=dat
+00018ba0: 615f 6c61 6265 6c2c 0a20 2020 2020 2020  a_label,.       
+00018bb0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00018bc0: 2020 2020 2320 7365 7420 616e 6420 706c      # set and pl
+00018bd0: 6f74 2065 7272 6f72 2062 6172 730a 2020  ot error bars.  
+00018be0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00018bf0: 662e 6d6f 6465 6c5f 7661 6c75 6573 2069  f.model_values i
+00018c00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00018c10: 2020 2020 2020 2020 2020 2020 2320 6265              # be
+00018c20: 7374 2d66 6974 206d 6f64 656c 2076 616c  st-fit model val
+00018c30: 7565 7320 6176 6169 6162 6c65 0a20 2020  ues avaiable.   
+00018c40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018c50: 6e6f 7420 7365 6c66 2e6f 7574 6572 2e75  not self.outer.u
+00018c60: 7365 5f47 6175 7373 4170 7072 6f78 3a0a  se_GaussApprox:.
+00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c80: 2020 2020 2320 7368 6f77 2050 6f69 7373      # show Poiss
+00018c90: 6f6e 2043 6f6e 6669 6465 6e63 6520 496e  on Confidence In
+00018ca0: 7465 7276 616c 730a 2020 2020 2020 2020  tervals.        
+00018cb0: 2020 2020 2020 2020 2020 2020 6570 203d              ep =
+00018cc0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+00018cd0: 2020 2020 2020 2020 656d 203d 205b 5d0a          em = [].
+00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018cf0: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+00018d00: 6765 2873 656c 662e 6e62 696e 7329 3a0a  ge(self.nbins):.
 00018d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d20: 206c 203d 2073 656c 662e 6d6f 6465 6c5f   l = self.model_
-00018d30: 7661 6c75 6573 5b69 5d20 2b20 6e70 2e61  values[i] + np.a
-00018d40: 6273 2873 656c 662e 4465 6c74 614d 755b  bs(self.DeltaMu[
-00018d50: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-00018d60: 2020 2020 2020 2020 2020 2020 6d2c 2070              m, p
-00018d70: 203d 2073 656c 662e 506f 6973 736f 6e5f   = self.Poisson_
-00018d80: 4349 286c 2c20 7369 676d 613d 312e 3029  CI(l, sigma=1.0)
-00018d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018da0: 2020 2020 2020 2020 2065 702e 6170 7065           ep.appe
-00018db0: 6e64 2870 202d 206c 290a 2020 2020 2020  nd(p - l).      
-00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dd0: 2020 656d 2e61 7070 656e 6428 6c20 2d20    em.append(l - 
-00018de0: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
-00018df0: 2020 2020 2020 2070 6c74 2e65 7272 6f72         plt.error
-00018e00: 6261 7228 0a20 2020 2020 2020 2020 2020  bar(.           
-00018e10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018e20: 662e 6365 6e74 6572 732c 0a20 2020 2020  f.centers,.     
-00018e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e40: 2020 206d 636f 6e74 732c 0a20 2020 2020     mconts,.     
-00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e60: 2020 2079 6572 723d 2865 6d2c 2065 7029     yerr=(em, ep)
-00018e70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018e80: 2020 2020 2020 2020 2020 666d 743d 2220            fmt=" 
-00018e90: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00018ea0: 2020 2020 2020 2020 2020 2065 636f 6c6f             ecolo
-00018eb0: 723d 226f 6c69 7665 222c 0a20 2020 2020  r="olive",.     
-00018ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ed0: 2020 2063 6170 7369 7a65 3d33 2c0a 2020     capsize=3,.  
-00018ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ef0: 2020 2020 2020 616c 7068 613d 302e 382c        alpha=0.8,
-00018f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018f10: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00018f20: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
-00018f30: 7368 6f77 2073 796d 6d65 7472 6963 2065  show symmetric e
-00018f40: 7272 6f72 2062 6172 730a 2020 2020 2020  rror bars.      
-00018f50: 2020 2020 2020 2020 2020 2020 2020 6570                ep
-00018f60: 203d 206e 702e 7371 7274 2873 656c 662e   = np.sqrt(self.
-00018f70: 6d6f 6465 6c5f 7661 6c75 6573 202b 206e  model_values + n
-00018f80: 702e 6162 7328 7365 6c66 2e44 656c 7461  p.abs(self.Delta
-00018f90: 4d75 2929 0a20 2020 2020 2020 2020 2020  Mu)).           
-00018fa0: 2020 2020 2020 2020 2065 6d20 3d20 5b0a           em = [.
-00018fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fc0: 2020 2020 2020 2020 6570 5b69 5d0a 2020          ep[i].  
-00018fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fe0: 2020 2020 2020 6966 2073 656c 662e 6d6f        if self.mo
-00018ff0: 6465 6c5f 7661 6c75 6573 5b69 5d20 2d20  del_values[i] - 
-00019000: 6570 5b69 5d20 3e20 302e 300a 2020 2020  ep[i] > 0.0.    
-00019010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019020: 2020 2020 656c 7365 2073 656c 662e 6d6f      else self.mo
-00019030: 6465 6c5f 7661 6c75 6573 5b69 5d0a 2020  del_values[i].  
-00019040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019050: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00019060: 616e 6765 286c 656e 2865 7029 290a 2020  ange(len(ep)).  
-00019070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019080: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-00019090: 2020 2020 2020 2020 706c 742e 6572 726f          plt.erro
-000190a0: 7262 6172 280a 2020 2020 2020 2020 2020  rbar(.          
-000190b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000190c0: 6c66 2e63 656e 7465 7273 2c0a 2020 2020  lf.centers,.    
-000190d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190e0: 2020 2020 7365 6c66 2e6d 6f64 656c 5f76      self.model_v
-000190f0: 616c 7565 732c 0a20 2020 2020 2020 2020  alues,.         
-00019100: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00019110: 6572 723d 2865 6d2c 2065 7029 2c0a 2020  err=(em, ep),.  
-00019120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019130: 2020 2020 2020 666d 743d 2220 222c 0a20        fmt=" ",. 
-00019140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019150: 2020 2020 2020 2065 636f 6c6f 723d 226f         ecolor="o
-00019160: 6c69 7665 222c 0a20 2020 2020 2020 2020  live",.         
-00019170: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00019180: 6c69 6e65 7769 6474 683d 322c 0a20 2020  linewidth=2,.   
-00019190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191a0: 2020 2020 2061 6c70 6861 3d30 2e38 2c0a       alpha=0.8,.
-000191b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191c0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000191d0: 2020 656c 7365 3a20 2023 206e 6f20 6d6f    else:  # no mo
-000191e0: 6465 6c20 7661 6c75 6573 2061 7661 696c  del values avail
-000191f0: 6162 6c65 2028 7965 7429 2c20 7368 6f77  able (yet), show
-00019200: 2065 7272 6f72 2062 6172 7320 7265 6c61   error bars rela
-00019210: 7465 6420 746f 2064 6174 610a 2020 2020  ted to data.    
-00019220: 2020 2020 2020 2020 2020 2020 6570 203d              ep =
-00019230: 206e 702e 7371 7274 2873 656c 662e 636f   np.sqrt(self.co
-00019240: 6e74 656e 7473 202b 206e 702e 6162 7328  ntents + np.abs(
-00019250: 7365 6c66 2e44 656c 7461 4d75 2929 0a20  self.DeltaMu)). 
-00019260: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00019270: 6d20 3d20 5b0a 2020 2020 2020 2020 2020  m = [.          
-00019280: 2020 2020 2020 2020 2020 6570 5b69 5d20            ep[i] 
-00019290: 6966 2073 656c 662e 636f 6e74 656e 7473  if self.contents
-000192a0: 5b69 5d20 2d20 6570 5b69 5d20 3e20 302e  [i] - ep[i] > 0.
-000192b0: 3020 656c 7365 2073 656c 662e 636f 6e74  0 else self.cont
-000192c0: 656e 7473 5b69 5d0a 2020 2020 2020 2020  ents[i].        
-000192d0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000192e0: 6920 696e 2072 616e 6765 286c 656e 2865  i in range(len(e
-000192f0: 7029 290a 2020 2020 2020 2020 2020 2020  p)).            
-00019300: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00019310: 2020 2020 2020 706c 742e 6572 726f 7262        plt.errorb
-00019320: 6172 280a 2020 2020 2020 2020 2020 2020  ar(.            
-00019330: 2020 2020 2020 2020 7365 6c66 2e63 656e          self.cen
-00019340: 7465 7273 2c0a 2020 2020 2020 2020 2020  ters,.          
-00019350: 2020 2020 2020 2020 2020 6263 6f6e 7473            bconts
-00019360: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019370: 2020 2020 2020 7965 7272 3d28 656d 2c20        yerr=(em, 
-00019380: 6570 292c 0a20 2020 2020 2020 2020 2020  ep),.           
-00019390: 2020 2020 2020 2020 2066 6d74 3d22 5f22           fmt="_"
-000193a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000193b0: 2020 2020 2020 636f 6c6f 723d 2264 6172        color="dar
-000193c0: 6b62 6c75 6522 2c0a 2020 2020 2020 2020  kblue",.        
-000193d0: 2020 2020 2020 2020 2020 2020 6d61 726b              mark
-000193e0: 6572 7369 7a65 3d31 352c 0a20 2020 2020  ersize=15,.     
-000193f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00019400: 636f 6c6f 723d 2264 6172 6b62 6c75 6522  color="darkblue"
-00019410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019420: 2020 2020 2020 616c 7068 613d 302e 382c        alpha=0.8,
-00019430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019440: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-00019450: 6574 7572 6e20 6669 670a 0a20 2020 2020  eturn fig..     
-00019460: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00019470: 0a20 2020 2020 2020 2064 6566 2050 6f69  .        def Poi
-00019480: 7373 6f6e 5f43 4928 6c61 6d2c 2073 6967  sson_CI(lam, sig
-00019490: 6d61 3d31 2e30 293a 0a20 2020 2020 2020  ma=1.0):.       
-000194a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000194b0: 2020 2020 2064 6574 6572 6d69 6e65 206f       determine o
-000194c0: 6e65 2d73 6967 6d61 2043 6f6e 6669 6465  ne-sigma Confide
-000194d0: 6e63 6520 496e 7465 7276 616c 2061 726f  nce Interval aro
-000194e0: 756e 6420 7468 650a 2020 2020 2020 2020  und the.        
-000194f0: 2020 2020 6d65 616e 206c 616d 6264 6120      mean lambda 
-00019500: 6f66 2061 2050 6f69 7373 6f6e 2064 6973  of a Poisson dis
-00019510: 7472 6962 7574 696f 6e2c 2050 6f69 7373  tribution, Poiss
-00019520: 2878 2c20 6c61 6d62 6461 292e 0a0a 2020  (x, lambda)...  
-00019530: 2020 2020 2020 2020 2020 5468 6520 6d65            The me
-00019540: 7468 6f64 2069 7320 6261 7365 6420 6f6e  thod is based on
-00019550: 2064 656c 7461 2d6c 6f67 2d4c 696b 656c   delta-log-Likel
-00019560: 6968 6f6f 6420 2864 6c4c 290a 2020 2020  ihood (dlL).    
-00019570: 2020 2020 2020 2020 6f66 2074 6865 2050          of the P
-00019580: 6f69 7373 696f 6e20 6c69 6b65 6c69 686f  oission likeliho
-00019590: 6f64 0a0a 2020 2020 2020 2020 2020 2020  od..            
-000195a0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-000195b0: 2020 202d 206c 616d 3a20 6d65 616e 206f     - lam: mean o
-000195c0: 6620 506f 6973 7369 6f6e 2064 6973 7472  f Poission distr
-000195d0: 6962 7574 696f 6e0a 2020 2020 2020 2020  ibution.        
-000195e0: 2020 2020 202d 2063 6c3a 2064 6573 6972       - cl: desir
-000195f0: 6564 2063 6f6e 6669 6465 6e63 6520 6c65  ed confidence le
-00019600: 7665 6c0a 2020 2020 2020 2020 2020 2020  vel.            
-00019610: 202d 2073 6967 6d61 3a20 616c 7465 726e   - sigma: altern
-00019620: 6174 6976 656c 7920 7370 6563 6966 7920  atively specify 
-00019630: 616e 206e 2d73 6967 6d61 2069 6e74 6572  an n-sigma inter
-00019640: 7661 6c0a 2020 2020 2020 2020 2020 2020  val.            
-00019650: 2222 220a 0a20 2020 2020 2020 2020 2020  """..           
-00019660: 2023 2066 756e 6374 696f 6e73 0a20 2020   # functions.   
-00019670: 2020 2020 2020 2020 2064 6566 206e 6c4c           def nlL
-00019680: 506f 6973 736f 6e28 782c 206c 616d 293a  Poisson(x, lam):
-00019690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000196a0: 2022 2222 6e65 6761 7469 7665 206c 6f67   """negative log
-000196b0: 2d6c 696b 656c 6968 6f6f 6420 6f66 2050  -likelihood of P
-000196c0: 6f69 7373 6f69 6e20 6469 7374 7262 7574  oissoin distrbut
-000196d0: 696f 6e22 2222 0a20 2020 2020 2020 2020  ion""".         
-000196e0: 2020 2020 2020 2072 6574 7572 6e20 6c61         return la
-000196f0: 6d20 2d20 7820 2a20 6e70 2e6c 6f67 286c  m - x * np.log(l
-00019700: 616d 2920 2b20 6c6f 6767 616d 6d61 2878  am) + loggamma(x
-00019710: 202b 2031 2e30 290a 0a20 2020 2020 2020   + 1.0)..       
-00019720: 2020 2020 2064 6566 2066 2878 2c20 6c61       def f(x, la
-00019730: 6d2c 2064 6c4c 293a 0a20 2020 2020 2020  m, dlL):.       
-00019740: 2020 2020 2020 2020 2022 2222 4465 6c74           """Delt
-00019750: 6120 6c6f 672d 4c20 2d20 6f66 6673 6574  a log-L - offset
-00019760: 2c20 696e 7075 7420 746f 204e 6577 746f  , input to Newto
-00019770: 6e20 6d65 7468 6f64 2222 220a 2020 2020  n method""".    
-00019780: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00019790: 726e 206e 6c4c 506f 6973 736f 6e28 782c  rn nlLPoisson(x,
-000197a0: 206c 616d 2920 2d20 6e6c 4c50 6f69 7373   lam) - nlLPoiss
-000197b0: 6f6e 286c 616d 2c20 6c61 6d29 202d 2064  on(lam, lam) - d
-000197c0: 6c4c 0a0a 2020 2020 2020 2020 2020 2020  lL..            
-000197d0: 646c 4c20 3d20 302e 3520 2a20 7369 676d  dlL = 0.5 * sigm
-000197e0: 6120 2a20 7369 676d 610a 0a20 2020 2020  a * sigma..     
-000197f0: 2020 2020 2020 2023 2066 6f72 2064 6c4c         # for dlL
-00019800: 3d30 2e35 2c20 7468 6572 6520 6973 206f  =0.5, there is o
-00019810: 6e6c 7920 6f6e 6520 696e 7465 7273 6563  nly one intersec
-00019820: 7469 6f6e 2077 6974 6820 7a65 726f 2066  tion with zero f
-00019830: 6f72 206c 616d 3c31 2e38 0a20 2020 2020  or lam<1.8.     
-00019840: 2020 2020 2020 2064 6c20 3d20 312e 3220         dl = 1.2 
-00019850: 2a20 6e70 2e73 7172 7428 6c61 6d29 0a20  * np.sqrt(lam). 
-00019860: 2020 2020 2020 2020 2020 2064 6c6d 203d             dlm =
-00019870: 206d 696e 2864 6c2c 206c 616d 290a 2020   min(dl, lam).  
-00019880: 2020 2020 2020 2020 2020 6370 203d 206e            cp = n
-00019890: 6577 746f 6e28 662c 2078 303d 6c61 6d20  ewton(f, x0=lam 
-000198a0: 2b20 646c 2c20 7831 3d6c 616d 2c20 6172  + dl, x1=lam, ar
-000198b0: 6773 3d28 6c61 6d2c 2064 6c4c 2929 0a20  gs=(lam, dlL)). 
-000198c0: 2020 2020 2020 2020 2020 2074 7279 3a20             try: 
-000198d0: 2023 206d 6179 206e 6f74 2063 6f6e 7665   # may not conve
-000198e0: 7267 6520 666f 7220 736d 616c 6c20 6c61  rge for small la
-000198f0: 6d62 6461 2c20 6173 2074 6865 7265 2069  mbda, as there i
-00019900: 7320 6e6f 2069 6e74 6572 7365 6374 696f  s no intersectio
-00019910: 6e20 3c20 6c61 6d0a 2020 2020 2020 2020  n < lam.        
-00019920: 2020 2020 2020 2020 636d 203d 206e 6577          cm = new
-00019930: 746f 6e28 662c 2078 303d 6c61 6d20 2d20  ton(f, x0=lam - 
-00019940: 646c 6d2c 2078 313d 6c61 6d2c 2061 7267  dlm, x1=lam, arg
-00019950: 733d 286c 616d 2c20 646c 4c29 290a 2020  s=(lam, dlL)).  
-00019960: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00019970: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019980: 2020 636d 203d 2030 2e30 0a20 2020 2020    cm = 0.0.     
-00019990: 2020 2020 2020 2069 6620 2863 7020 2d20         if (cp - 
-000199a0: 636d 2920 3c20 6c61 6d20 2f20 3130 302e  cm) < lam / 100.
-000199b0: 303a 2020 2320 666f 756e 6420 7361 6d65  0:  # found same
-000199c0: 2069 6e74 6572 7365 6374 696f 6e2c 0a20   intersection,. 
-000199d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000199e0: 6d20 3d20 302e 3020 2023 2020 7365 7420  m = 0.0  #  set 
-000199f0: 3173 7420 6f6e 6520 746f 2030 2e0a 0a20  1st one to 0... 
-00019a00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00019a10: 6e20 636d 2c20 6370 0a0a 2020 2020 2320  n cm, cp..    # 
-00019a20: 2d2d 2d20 636f 7374 2066 756e 6374 696f  --- cost functio
-00019a30: 6e20 666f 7220 6869 7374 6f67 7261 6d20  n for histogram 
-00019a40: 6461 7461 0a20 2020 2063 6c61 7373 2068  data.    class h
-00019a50: 436f 7374 3a0a 2020 2020 2020 2020 2222  Cost:.        ""
-00019a60: 2243 6f73 7420 6675 6e63 7469 6f6e 2066  "Cost function f
-00019a70: 6f72 2062 696e 6e65 6420 6461 7461 0a0a  or binned data..
-00019a80: 2020 2020 2020 2020 5468 6520 5f5f 6361          The __ca
-00019a90: 6c6c 5f5f 206d 6574 686f 6420 6f66 2074  ll__ method of t
-00019aa0: 6869 7320 636c 6173 7320 6973 2063 616c  his class is cal
-00019ab0: 6c65 6420 6279 2069 6d69 6e75 6974 2e0a  led by iminuit..
-00019ac0: 0a20 2020 2020 2020 2054 6865 2064 6566  .        The def
-00019ad0: 6175 6c74 2063 6f73 7420 6675 6e63 7469  ault cost functi
-00019ae0: 6f6e 2074 6f20 6d69 6e69 6d6f 7a65 2069  on to minimoze i
-00019af0: 7320 7477 6963 6520 7468 6520 6e65 6761  s twice the nega
-00019b00: 7469 7665 0a20 2020 2020 2020 206c 6f67  tive.        log
-00019b10: 2d6c 696b 656c 6968 6f6f 6420 6f66 2074  -likelihood of t
-00019b20: 6865 2050 6f69 7373 6f6e 2064 6973 7472  he Poisson distr
-00019b30: 6962 7574 696f 6e20 6765 6e65 7261 6c69  ibution generali
-00019b40: 7a65 6420 746f 0a20 2020 2020 2020 2063  zed to.        c
-00019b50: 6f6e 7469 6e75 6f75 7320 6f62 7365 7276  ontinuous observ
-00019b60: 6174 696f 6e73 2078 2062 7920 7265 706c  ations x by repl
-00019b70: 6163 696e 6720 6b21 2062 7920 7468 6520  acing k! by the 
-00019b80: 6761 6d6d 6120 6675 6e63 7469 6f6e 3a0a  gamma function:.
-00019b90: 0a20 2020 2020 2020 202e 2e20 6d61 7468  .        .. math
-00019ba0: 3a3a 0a20 2020 2020 2020 2020 2020 2063  ::.            c
-00019bb0: 6f73 7428 783b 5c6c 616d 6264 6129 203d  ost(x;\lambda) =
-00019bc0: 2032 205c 6c61 6d62 6461 2028 5c6c 616d   2 \lambda (\lam
-00019bd0: 6264 6120 2d20 782a 5c6c 6e28 5c6c 616d  bda - x*\ln(\lam
-00019be0: 6264 6129 202b 205c 6c6e 5c47 616d 6d61  bda) + \ln\Gamma
-00019bf0: 2878 2b31 2e29 290a 0a20 2020 2020 2020  (x+1.))..       
-00019c00: 2041 6c74 6572 6e61 7469 7665 6c79 2c20   Alternatively, 
-00019c10: 7468 6520 4761 7573 7369 616e 2061 7070  the Gaussian app
-00019c20: 726f 7869 6d61 7469 6f6e 2069 7320 6176  roximation is av
-00019c30: 6169 6c61 626c 653a 0a0a 2020 2020 2020  ailable:..      
-00019c40: 2020 2e2e 206d 6174 683a 3a0a 2020 2020    .. math::.    
-00019c50: 2020 2020 2020 2020 636f 7374 2878 3b5c          cost(x;\
-00019c60: 6c61 6d62 6461 2920 3d20 2878 202d 205c  lambda) = (x - \
-00019c70: 6c61 6d62 6461 295e 3220 2f20 5c6c 616d  lambda)^2 / \lam
-00019c80: 6264 6120 2b20 5c6c 6e28 5c6c 616d 6264  bda + \ln(\lambd
-00019c90: 6129 0a0a 2020 2020 2020 2020 5468 6520  a)..        The 
-00019ca0: 696d 706c 656d 656e 7461 7469 6f6e 2061  implementation a
-00019cb0: 6c73 6f20 7065 726d 6974 7320 746f 2073  lso permits to s
-00019cc0: 6869 6674 2074 6865 206f 6273 6572 7661  hift the observa
-00019cd0: 7469 6f6e 2078 2062 7920 616e 0a20 2020  tion x by an.   
-00019ce0: 2020 2020 206f 6666 7365 7420 746f 2074       offset to t
-00019cf0: 616b 6520 696e 746f 2061 6363 6f75 6e74  ake into account
-00019d00: 2063 6f72 7265 6374 696f 6e73 2074 6f20   corrections to 
-00019d10: 7468 6520 6e75 6d62 6572 206f 6620 6f62  the number of ob
-00019d20: 7365 7276 6564 0a20 2020 2020 2020 2062  served.        b
-00019d30: 696e 2065 6e74 7269 6573 2028 652e 672e  in entries (e.g.
-00019d40: 2064 7565 2074 6f20 6261 636b 6772 6f75   due to backgrou
-00019d50: 6e64 206f 7220 6566 6669 6369 656e 6379  nd or efficiency
-00019d60: 2063 6f72 7265 6374 696f 6e73 293a 0a20   corrections):. 
-00019d70: 2020 2020 2020 2078 202d 3e20 782d 6465         x -> x-de
-00019d80: 6c74 614d 7520 7769 7468 2064 656c 7461  ltaMu with delta
-00019d90: 4d75 203d 206d 7520 2d20 6c61 6d62 6461  Mu = mu - lambda
-00019da0: 2c20 7768 6572 6520 6d75 2069 7320 7468  , where mu is th
-00019db0: 6520 6d65 616e 0a20 2020 2020 2020 206f  e mean.        o
-00019dc0: 6620 7468 6520 7368 6966 7465 6420 506f  f the shifted Po
-00019dd0: 6973 736f 6e20 6f72 2047 6175 c39f 2064  isson or Gau.. d
-00019de0: 6973 7472 6962 7574 696f 6e2e 0a0a 2020  istribution...  
-00019df0: 2020 2020 2020 5468 6520 6e75 6d62 6572        The number
-00019e00: 206f 6620 6269 6e20 656e 7472 6965 7320   of bin entries 
-00019e10: 7072 6564 6963 7465 6420 6279 2074 6865  predicted by the
-00019e20: 206d 6f64 656c 2064 656e 7369 7479 2069   model density i
-00019e30: 7320 6361 6c63 756c 6174 6564 0a20 2020  s calculated.   
-00019e40: 2020 2020 2062 7920 616e 2061 7070 726f       by an appro
-00019e50: 7869 6d61 7465 2069 6e74 6567 7261 6c20  ximate integral 
-00019e60: 6f76 6572 2074 6865 2072 6573 7065 6374  over the respect
-00019e70: 6976 6520 6269 6e20 7261 6e67 6573 2075  ive bin ranges u
-00019e80: 7369 6e67 2074 6865 0a20 2020 2020 2020  sing the.       
-00019e90: 2053 696d 7073 6f6e 2072 756c 652e 0a0a   Simpson rule...
-00019ea0: 2020 2020 2020 2020 546f 206a 7564 6765          To judge
-00019eb0: 2074 6865 206c 6576 656c 206f 6620 6167   the level of ag
-00019ec0: 7265 656d 656e 7420 6f66 206d 6f64 656c  reement of model
-00019ed0: 2064 656e 7369 7479 2061 6e64 2068 6973   density and his
-00019ee0: 746f 6772 616d 2064 6174 612c 0a20 2020  togram data,.   
-00019ef0: 2020 2020 2061 2022 676f 6f64 6e65 7373       a "goodness
-00019f00: 2d6f 662d 6669 7422 2028 2a67 6f66 2a29  -of-fit" (*gof*)
-00019f10: 2076 616c 7565 2069 7320 6361 6c75 6c61   value is calula
-00019f20: 7465 6420 6173 2074 6865 206c 696b 656c  ted as the likel
-00019f30: 6968 6f6f 642d 7261 7469 6f20 6f66 0a20  ihood-ratio of. 
-00019f40: 2020 2020 2020 2074 6865 206d 6f64 656c         the model
-00019f50: 2077 2e72 2e74 2e20 7468 6520 6461 7461   w.r.t. the data
-00019f60: 2061 6e64 2074 6865 2073 6f2d 6361 6c6c   and the so-call
-00019f70: 6564 2022 7361 7475 7261 7465 6420 6d6f  ed "saturated mo
-00019f80: 6465 6c22 2064 6573 6372 6962 696e 670a  del" describing.
-00019f90: 2020 2020 2020 2020 7468 6520 6461 7461          the data
-00019fa0: 2070 6572 6665 6374 6c79 2c20 692e 652e   perfectly, i.e.
-00019fb0: 2020 3a6d 6174 683a 6063 6f73 745f 7b73    :math:`cost_{s
-00019fc0: 6174 7d28 7829 203d 2063 6f73 7428 783b  at}(x) = cost(x;
-00019fd0: 205c 6c61 6d62 6461 3d78 2960 2e0a 2020   \lambda=x)`..  
-00019fe0: 2020 2020 2020 4966 2074 6865 2062 696e        If the bin
-00019ff0: 2065 6e74 7269 6573 2061 7265 2073 7566   entries are suf
-0001a000: 6669 6369 656e 746c 7920 6c61 7267 652c  ficiently large,
-0001a010: 202a 676f 662a 2063 6f6e 7665 7267 6573   *gof* converges
-0001a020: 2074 6f20 7468 6520 7374 616e 6461 7264   to the standard
-0001a030: 0a20 2020 2020 2020 202a 6368 6932 2a20  .        *chi2* 
-0001a040: 7661 6c75 652e 0a0a 2020 2020 2020 2020  value...        
-0001a050: 496e 7075 743a 0a0a 2020 2020 2020 2020  Input:..        
-0001a060: 2d20 6f75 7465 723a 2070 6f69 6e74 6572  - outer: pointer
-0001a070: 2074 6f20 696e 7374 616e 6365 206f 6620   to instance of 
-0001a080: 6361 6c6c 696e 6720 636c 6173 730a 2020  calling class.  
-0001a090: 2020 2020 2020 2d20 6d6f 6465 6c3a 206d        - model: m
-0001a0a0: 6f64 656c 2066 756e 6374 696f 6e20 6628  odel function f(
-0001a0b0: 782c 205c 2a70 6172 290a 2020 2020 2020  x, \*par).      
-0001a0c0: 2020 2d20 7573 655f 4761 7573 7341 7070    - use_GaussApp
-0001a0d0: 726f 782c 2062 6f6f 6c3a 2075 7365 2047  rox, bool: use G
-0001a0e0: 6175 7373 6961 6e20 6170 7072 6f78 696d  aussian approxim
-0001a0f0: 6174 696f 6e0a 2020 2020 2020 2020 2d20  ation.        - 
-0001a100: 6465 6e73 6974 792c 2062 6f6f 6c3a 2066  density, bool: f
-0001a110: 6974 2061 206e 6f72 6d61 6c69 7365 6420  it a normalised 
-0001a120: 6465 6e73 6974 793b 2069 6620 4661 6c73  density; if Fals
-0001a130: 652c 2061 6e20 6f76 6572 616c 6c0a 2020  e, an overall.  
-0001a140: 2020 2020 2020 2020 6e6f 726d 616c 6973          normalis
-0001a150: 6174 696f 6e20 6d75 7374 2062 6520 7072  ation must be pr
-0001a160: 6f76 6964 6564 2069 6e20 7468 6520 6d6f  ovided in the mo
-0001a170: 6465 6c20 6675 6e63 7469 6f6e 0a0a 2020  del function..  
-0001a180: 2020 2020 2020 4461 7461 206d 656d 6265        Data membe
-0001a190: 7273 3a0a 0a20 2020 2020 2020 202d 206e  rs:..        - n
-0001a1a0: 646f 663a 2064 6567 7265 6573 206f 6620  dof: degrees of 
-0001a1b0: 6672 6565 646f 6d0a 2020 2020 2020 2020  freedom.        
-0001a1c0: 2d20 6e63 6f6e 7374 7261 696e 7473 3a20  - nconstraints: 
-0001a1d0: 6e75 6d62 6572 206f 6620 7061 7261 6d65  number of parame
-0001a1e0: 7465 7220 636f 6e73 7472 6169 6e74 730a  ter constraints.
-0001a1f0: 2020 2020 2020 2020 2d20 676f 663a 2067          - gof: g
-0001a200: 6f6f 646e 6573 732d 6f66 2d66 6974 2061  oodness-of-fit a
-0001a210: 7320 6c69 6b65 6c69 686f 6f64 2072 6174  s likelihood rat
-0001a220: 696f 2077 2e72 2e74 2e20 7468 6520 2773  io w.r.t. the 's
-0001a230: 6174 7572 6174 6564 206d 6f64 656c 270a  aturated model'.
-0001a240: 0a20 2020 2020 2020 2045 7874 6572 6e61  .        Externa
-0001a250: 6c20 7265 6665 7265 6e63 6573 3a0a 0a20  l references:.. 
-0001a260: 2020 2020 2020 202d 206d 6f64 656c 2878         - model(x
-0001a270: 2c20 5c2a 7061 7229 3a20 7468 6520 6d6f  , \*par): the mo
-0001a280: 6465 6c20 6675 6e63 7469 6f6e 0a20 2020  del function.   
-0001a290: 2020 2020 202d 2064 6174 613a 2070 6f69       - data: poi
-0001a2a0: 6e74 6572 2074 6f20 696e 7374 616e 6365  nter to instance
-0001a2b0: 206f 6620 636c 6173 7320 6869 7374 4461   of class histDa
-0001a2c0: 7461 0a20 2020 2020 2020 202d 2064 6174  ta.        - dat
-0001a2d0: 612e 6d6f 6465 6c5f 7661 6c75 6573 3a20  a.model_values: 
-0001a2e0: 6269 6e20 656e 7472 6965 7320 6361 6c63  bin entries calc
-0001a2f0: 756c 6174 6564 2062 7920 7468 6520 6265  ulated by the be
-0001a300: 7374 2d66 6974 206d 6f64 656c 0a20 2020  st-fit model.   
-0001a310: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0001a320: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0001a330: 656c 662c 206f 7574 6572 2c20 6d6f 6465  elf, outer, mode
-0001a340: 6c2c 2075 7365 5f47 6175 7373 4170 7072  l, use_GaussAppr
-0001a350: 6f78 3d46 616c 7365 2c20 6465 6e73 6974  ox=False, densit
-0001a360: 793d 5472 7565 293a 0a20 2020 2020 2020  y=True):.       
-0001a370: 2020 2020 2023 2064 6174 6120 6f62 6a65       # data obje
-0001a380: 6374 206f 6620 7479 7065 2068 6973 7444  ct of type histD
-0001a390: 6174 6143 6f6e 7461 696e 7465 720a 2020  ataContainter.  
-0001a3a0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0001a3b0: 6174 6120 3d20 6f75 7465 722e 6844 6174  ata = outer.hDat
-0001a3c0: 610a 2020 2020 2020 2020 2020 2020 6966  a.            if
-0001a3d0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-0001a3e0: 7365 6c66 2e64 6174 612c 206d 6e46 6974  self.data, mnFit
-0001a3f0: 2e68 6973 7444 6174 6143 6f6e 7461 696e  .histDataContain
-0001a400: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
-0001a410: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0001a420: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0001a430: 2020 2020 2020 2020 2020 2022 2021 2121             " !!!
-0001a440: 206d 6e46 6974 2e68 436f 7374 3a20 6578   mnFit.hCost: ex
-0001a450: 7065 6374 696e 6720 6461 7461 2063 6f6e  pecting data con
-0001a460: 7461 696e 6572 206f 6620 7479 7065 2027  tainer of type '
-0001a470: 6869 7374 4461 7461 436f 6e74 6169 6e65  histDataContaine
-0001a480: 7227 220a 2020 2020 2020 2020 2020 2020  r'".            
-0001a490: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0001a4a0: 2020 2073 656c 662e 6d6f 6465 6c20 3d20     self.model = 
-0001a4b0: 6d6f 6465 6c0a 2020 2020 2020 2020 2020  model.          
-0001a4c0: 2020 7365 6c66 2e64 656e 7369 7479 203d    self.density =
-0001a4d0: 2064 656e 7369 7479 0a20 2020 2020 2020   density.       
-0001a4e0: 2020 2020 2073 656c 662e 4761 7573 7341       self.GaussA
-0001a4f0: 7070 726f 7820 3d20 7573 655f 4761 7573  pprox = use_Gaus
-0001a500: 7341 7070 726f 780a 2020 2020 2020 2020  sApprox.        
-0001a510: 2020 2020 7365 6c66 2e71 7569 6574 203d      self.quiet =
-0001a520: 206f 7574 6572 2e71 7569 6574 0a0a 2020   outer.quiet..  
-0001a530: 2020 2020 2020 2020 2020 2320 7365 7420            # set 
-0001a540: 7072 6f70 6572 2073 6967 6e61 7475 7265  proper signature
-0001a550: 206f 6620 6d6f 6465 6c20 6675 6e63 7469   of model functi
-0001a560: 6f6e 2066 6f72 2069 6d69 6e75 6974 0a20  on for iminuit. 
-0001a570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a580: 706e 616d 7320 3d20 6f75 7465 722e 706e  pnams = outer.pn
-0001a590: 616d 730a 2020 2020 2020 2020 2020 2020  ams.            
-0001a5a0: 7365 6c66 2e6e 7061 7220 3d20 6f75 7465  self.npar = oute
-0001a5b0: 722e 6e70 6172 0a0a 2020 2020 2020 2020  r.npar..        
-0001a5c0: 2020 2020 7365 6c66 2e63 6f6e 7374 7261      self.constra
-0001a5d0: 696e 7473 203d 206f 7574 6572 2e63 6f6e  ints = outer.con
-0001a5e0: 7374 7261 696e 7473 0a20 2020 2020 2020  straints.       
-0001a5f0: 2020 2020 2073 656c 662e 6e63 6f6e 7374       self.nconst
-0001a600: 7261 696e 7473 203d 206c 656e 2873 656c  raints = len(sel
-0001a610: 662e 636f 6e73 7472 6169 6e74 7329 0a20  f.constraints). 
-0001a620: 2020 2020 2020 2020 2020 2023 2074 616b             # tak
-0001a630: 6520 6163 636f 756e 7420 6f66 2063 6f6e  e account of con
-0001a640: 7374 7261 696e 7473 2069 6e20 6465 6772  straints in degr
-0001a650: 6565 7320 6f66 2066 7265 6564 6f6d 0a20  ees of freedom. 
-0001a660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a670: 6e64 6f66 203d 2073 656c 662e 6461 7461  ndof = self.data
-0001a680: 2e6e 6269 6e73 202d 2073 656c 662e 6e70  .nbins - self.np
-0001a690: 6172 202b 2073 656c 662e 6e63 6f6e 7374  ar + self.nconst
-0001a6a0: 7261 696e 7473 202b 206f 7574 6572 2e6e  raints + outer.n
-0001a6b0: 6669 7865 640a 0a20 2020 2020 2020 2020  fixed..         
-0001a6c0: 2020 2023 2066 6c61 6720 746f 2063 6f6e     # flag to con
-0001a6d0: 7472 6f6c 2066 696e 616c 2061 6374 696f  trol final actio
-0001a6e0: 6e73 2069 6e20 636f 7374 2066 756e 6374  ns in cost funct
-0001a6f0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0001a700: 7365 6c66 2e66 696e 616c 5f63 616c 6c20  self.final_call 
-0001a710: 3d20 4661 6c73 650a 0a20 2020 2020 2020  = False..       
-0001a720: 2020 2020 2069 6620 7365 6c66 2e47 6175       if self.Gau
-0001a730: 7373 4170 7072 6f78 3a0a 2020 2020 2020  ssApprox:.      
-0001a740: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0001a750: 326c 4c63 6f73 7420 3d20 7365 6c66 2e6e  2lLcost = self.n
-0001a760: 326c 4c47 6175 7373 0a20 2020 2020 2020  2lLGauss.       
-0001a770: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001a780: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001a790: 6e32 6c4c 636f 7374 203d 2073 656c 662e  n2lLcost = self.
-0001a7a0: 6e32 6c4c 506f 6973 736f 6e0a 0a20 2020  n2lLPoisson..   
-0001a7b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0001a7c0: 2e64 656e 7369 7479 3a0a 2020 2020 2020  .density:.      
-0001a7d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0001a7e0: 6f72 6d20 3d20 7365 6c66 2e64 6174 612e  orm = self.data.
-0001a7f0: 4e74 6f74 0a20 2020 2020 2020 2020 2020  Ntot.           
-0001a800: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001a810: 2020 2020 2020 2073 656c 662e 6e6f 726d         self.norm
-0001a820: 203d 2031 2e30 0a0a 2020 2020 2020 2020   = 1.0..        
-0001a830: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-0001a840: 662c 202a 7061 7229 3a0a 2020 2020 2020  f, *par):.      
-0001a850: 2020 2020 2020 2320 6361 6c6c 6564 2069        # called i
-0001a860: 7465 7261 7469 7665 6c79 2062 7920 6d69  teratively by mi
-0001a870: 6e75 6974 0a0a 2020 2020 2020 2020 2020  nuit..          
-0001a880: 2020 2320 636f 7374 2066 756e 6374 696f    # cost functio
-0001a890: 6e20 6973 206c 696b 656c 6968 6f6f 6420  n is likelihood 
-0001a8a0: 6f66 2073 6869 6674 6564 2050 6f69 7373  of shifted Poiss
-0001a8b0: 6f6e 206f 7220 4761 7573 7320 6170 7072  on or Gauss appr
-0001a8c0: 6f78 696d 6174 696f 6e0a 0a20 2020 2020  oximation..     
-0001a8d0: 2020 2020 2020 2023 202d 2066 6972 7374         # - first
-0001a8e0: 2c20 7461 6b65 2069 6e74 6f20 6163 636f  , take into acco
-0001a8f0: 756e 7420 706f 7373 6962 6c65 2070 6172  unt possible par
-0001a900: 616d 6574 6572 2063 6f6e 7374 7261 696e  ameter constrain
-0001a910: 7473 0a20 2020 2020 2020 2020 2020 206e  ts.            n
-0001a920: 326c 4c20 3d20 302e 300a 2020 2020 2020  2lL = 0.0.      
-0001a930: 2020 2020 2020 6966 2073 656c 662e 6e63        if self.nc
-0001a940: 6f6e 7374 7261 696e 7473 3a0a 2020 2020  onstraints:.    
-0001a950: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001a960: 6320 696e 2073 656c 662e 636f 6e73 7472  c in self.constr
-0001a970: 6169 6e74 733a 0a20 2020 2020 2020 2020  aints:.         
-0001a980: 2020 2020 2020 2020 2020 2070 5f69 6420             p_id 
-0001a990: 3d20 635b 305d 0a20 2020 2020 2020 2020  = c[0].         
-0001a9a0: 2020 2020 2020 2020 2020 2072 203d 2028             r = (
-0001a9b0: 7061 725b 705f 6964 5d20 2d20 635b 315d  par[p_id] - c[1]
-0001a9c0: 2920 2f20 635b 325d 0a20 2020 2020 2020  ) / c[2].       
-0001a9d0: 2020 2020 2020 2020 2020 2020 206e 326c               n2l
-0001a9e0: 4c20 2b3d 2072 202a 2072 0a0a 2020 2020  L += r * r..    
-0001a9f0: 2020 2020 2020 2020 2320 2d20 6361 6c63          # - calc
-0001aa00: 756c 6174 6520 322a 6e65 674c 6f67 4c20  ulate 2*negLogL 
-0001aa10: 506f 6973 736f 6e3b 0a20 2020 2020 2020  Poisson;.       
-0001aa20: 2020 2020 2023 2020 6d6f 6465 6c20 7072       #  model pr
-0001aa30: 6564 6963 7469 6f6e 2061 7320 6170 7072  ediction as appr
-0001aa40: 6f78 696d 6174 6520 696e 7465 6772 616c  oximate integral
-0001aa50: 206f 7665 7220 6269 6e0a 2020 2020 2020   over bin.      
-0001aa60: 2020 2020 2020 6d6f 6465 6c5f 7661 6c75        model_valu
-0001aa70: 6573 203d 2073 656c 662e 6e6f 726d 202a  es = self.norm *
-0001aa80: 2073 656c 662e 696e 7465 6772 616c 5f6f   self.integral_o
-0001aa90: 7665 7242 696e 7328 0a20 2020 2020 2020  verBins(.       
-0001aaa0: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
-0001aab0: 7461 2e6c 6566 7473 2c20 7365 6c66 2e64  ta.lefts, self.d
-0001aac0: 6174 612e 7269 6768 7473 2c20 7365 6c66  ata.rights, self
-0001aad0: 2e6d 6f64 656c 2c20 2a70 6172 0a20 2020  .model, *par.   
-0001aae0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0001aaf0: 2020 2020 2020 2023 0a0a 2020 2020 2020         #..      
-0001ab00: 2020 2020 2020 6e32 6c4c 202b 3d20 6e70        n2lL += np
-0001ab10: 2e73 756d 280a 2020 2020 2020 2020 2020  .sum(.          
-0001ab20: 2020 2020 2020 7365 6c66 2e6e 326c 4c63        self.n2lLc
-0001ab30: 6f73 7428 0a20 2020 2020 2020 2020 2020  ost(.           
-0001ab40: 2020 2020 2020 2020 2073 656c 662e 6461           self.da
-0001ab50: 7461 2e63 6f6e 7465 6e74 7320 2d20 7365  ta.contents - se
-0001ab60: 6c66 2e64 6174 612e 4465 6c74 614d 752c  lf.data.DeltaMu,
-0001ab70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ab80: 2020 2020 206d 6f64 656c 5f76 616c 7565       model_value
-0001ab90: 7320 2b20 6e70 2e61 6273 2873 656c 662e  s + np.abs(self.
-0001aba0: 6461 7461 2e44 656c 7461 4d75 292c 0a20  data.DeltaMu),. 
-0001abb0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001abc0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-0001abd0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001abe0: 656c 662e 6669 6e61 6c5f 6361 6c6c 3a0a  elf.final_call:.
-0001abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac00: 6966 2073 656c 662e 4761 7573 7341 7070  if self.GaussApp
-0001ac10: 726f 783a 0a20 2020 2020 2020 2020 2020  rox:.           
-0001ac20: 2020 2020 2020 2020 2023 2072 6574 7572           # retur
-0001ac30: 6e20 7374 616e 6461 7264 2063 6869 5e32  n standard chi^2
-0001ac40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ac50: 2020 2020 2073 656c 662e 676f 6620 3d20       self.gof = 
-0001ac60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001ac70: 2020 2020 2020 2020 2020 6e32 6c4c 202d            n2lL -
-0001ac80: 206e 702e 6c6f 6728 6d6f 6465 6c5f 7661   np.log(model_va
-0001ac90: 6c75 6573 202b 206e 702e 6162 7328 7365  lues + np.abs(se
-0001aca0: 6c66 2e64 6174 612e 4465 6c74 614d 7529  lf.data.DeltaMu)
-0001acb0: 292e 7375 6d28 290a 2020 2020 2020 2020  ).sum().        
-0001acc0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001acd0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0001ace0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001acf0: 2020 2020 2020 2020 2320 7374 6f72 6520          # store 
-0001ad00: 676f 6f64 6e65 7373 2d6f 662d 6669 7420  goodness-of-fit 
-0001ad10: 2864 6966 6665 7265 6e63 6520 6f66 206e  (difference of n
-0001ad20: 6c4c 3220 772e 722e 742e 2073 6174 7572  lL2 w.r.t. satur
-0001ad30: 6174 6564 206d 6f64 656c 290a 2020 2020  ated model).    
-0001ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad50: 6e32 6c4c 5f73 6174 7572 6174 6564 203d  n2lL_saturated =
-0001ad60: 206e 702e 7375 6d28 0a20 2020 2020 2020   np.sum(.       
+00018d20: 2020 2020 2020 2020 6c20 3d20 7365 6c66          l = self
+00018d30: 2e6d 6f64 656c 5f76 616c 7565 735b 695d  .model_values[i]
+00018d40: 202b 206e 702e 6162 7328 7365 6c66 2e44   + np.abs(self.D
+00018d50: 656c 7461 4d75 5b69 5d29 0a20 2020 2020  eltaMu[i]).     
+00018d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d70: 2020 206d 2c20 7020 3d20 7365 6c66 2e50     m, p = self.P
+00018d80: 6f69 7373 6f6e 5f43 4928 6c2c 2073 6967  oisson_CI(l, sig
+00018d90: 6d61 3d31 2e30 290a 2020 2020 2020 2020  ma=1.0).        
+00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018db0: 6570 2e61 7070 656e 6428 7020 2d20 6c29  ep.append(p - l)
+00018dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018dd0: 2020 2020 2020 2020 2065 6d2e 6170 7065           em.appe
+00018de0: 6e64 286c 202d 206d 290a 2020 2020 2020  nd(l - m).      
+00018df0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00018e00: 742e 6572 726f 7262 6172 280a 2020 2020  t.errorbar(.    
+00018e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e20: 2020 2020 7365 6c66 2e63 656e 7465 7273      self.centers
+00018e30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00018e40: 2020 2020 2020 2020 2020 6d63 6f6e 7473            mconts
+00018e50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00018e60: 2020 2020 2020 2020 2020 7965 7272 3d28            yerr=(
+00018e70: 656d 2c20 6570 292c 0a20 2020 2020 2020  em, ep),.       
+00018e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e90: 2066 6d74 3d22 2022 2c0a 2020 2020 2020   fmt=" ",.      
+00018ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018eb0: 2020 6563 6f6c 6f72 3d22 6f6c 6976 6522    ecolor="olive"
+00018ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00018ed0: 2020 2020 2020 2020 2020 6361 7073 697a            capsiz
+00018ee0: 653d 332c 0a20 2020 2020 2020 2020 2020  e=3,.           
+00018ef0: 2020 2020 2020 2020 2020 2020 2061 6c70               alp
+00018f00: 6861 3d30 2e38 2c0a 2020 2020 2020 2020  ha=0.8,.        
+00018f10: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00018f20: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00018f30: 7365 3a20 2023 2073 686f 7720 7379 6d6d  se:  # show symm
+00018f40: 6574 7269 6320 6572 726f 7220 6261 7273  etric error bars
+00018f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018f60: 2020 2020 2065 7020 3d20 6e70 2e73 7172       ep = np.sqr
+00018f70: 7428 7365 6c66 2e6d 6f64 656c 5f76 616c  t(self.model_val
+00018f80: 7565 7320 2b20 6e70 2e61 6273 2873 656c  ues + np.abs(sel
+00018f90: 662e 4465 6c74 614d 7529 290a 2020 2020  f.DeltaMu)).    
+00018fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fb0: 656d 203d 205b 0a20 2020 2020 2020 2020  em = [.         
+00018fc0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00018fd0: 705b 695d 0a20 2020 2020 2020 2020 2020  p[i].           
+00018fe0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018ff0: 7365 6c66 2e6d 6f64 656c 5f76 616c 7565  self.model_value
+00019000: 735b 695d 202d 2065 705b 695d 203e 2030  s[i] - ep[i] > 0
+00019010: 2e30 0a20 2020 2020 2020 2020 2020 2020  .0.             
+00019020: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+00019030: 7365 6c66 2e6d 6f64 656c 5f76 616c 7565  self.model_value
+00019040: 735b 695d 0a20 2020 2020 2020 2020 2020  s[i].           
+00019050: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00019060: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00019070: 6570 2929 0a20 2020 2020 2020 2020 2020  ep)).           
+00019080: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00019090: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000190a0: 6c74 2e65 7272 6f72 6261 7228 0a20 2020  lt.errorbar(.   
+000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190c0: 2020 2020 2073 656c 662e 6365 6e74 6572       self.center
+000190d0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000190e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000190f0: 6d6f 6465 6c5f 7661 6c75 6573 2c0a 2020  model_values,.  
+00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019110: 2020 2020 2020 7965 7272 3d28 656d 2c20        yerr=(em, 
+00019120: 6570 292c 0a20 2020 2020 2020 2020 2020  ep),.           
+00019130: 2020 2020 2020 2020 2020 2020 2066 6d74               fmt
+00019140: 3d22 2022 2c0a 2020 2020 2020 2020 2020  =" ",.          
+00019150: 2020 2020 2020 2020 2020 2020 2020 6563                ec
+00019160: 6f6c 6f72 3d22 6f6c 6976 6522 2c0a 2020  olor="olive",.  
+00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019180: 2020 2020 2020 656c 696e 6577 6964 7468        elinewidth
+00019190: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
+000191a0: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+000191b0: 613d 302e 382c 0a20 2020 2020 2020 2020  a=0.8,.         
+000191c0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000191d0: 2020 2020 2020 2020 2065 6c73 653a 2020           else:  
+000191e0: 2320 6e6f 206d 6f64 656c 2076 616c 7565  # no model value
+000191f0: 7320 6176 6169 6c61 626c 6520 2879 6574  s available (yet
+00019200: 292c 2073 686f 7720 6572 726f 7220 6261  ), show error ba
+00019210: 7273 2072 656c 6174 6564 2074 6f20 6461  rs related to da
+00019220: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
+00019230: 2020 2065 7020 3d20 6e70 2e73 7172 7428     ep = np.sqrt(
+00019240: 7365 6c66 2e63 6f6e 7465 6e74 7320 2b20  self.contents + 
+00019250: 6e70 2e61 6273 2873 656c 662e 4465 6c74  np.abs(self.Delt
+00019260: 614d 7529 290a 2020 2020 2020 2020 2020  aMu)).          
+00019270: 2020 2020 2020 656d 203d 205b 0a20 2020        em = [.   
+00019280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019290: 2065 705b 695d 2069 6620 7365 6c66 2e63   ep[i] if self.c
+000192a0: 6f6e 7465 6e74 735b 695d 202d 2065 705b  ontents[i] - ep[
+000192b0: 695d 203e 2030 2e30 2065 6c73 6520 7365  i] > 0.0 else se
+000192c0: 6c66 2e63 6f6e 7465 6e74 735b 695d 0a20  lf.contents[i]. 
+000192d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192e0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+000192f0: 6528 6c65 6e28 6570 2929 0a20 2020 2020  e(len(ep)).     
+00019300: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00019310: 2020 2020 2020 2020 2020 2020 2070 6c74               plt
+00019320: 2e65 7272 6f72 6261 7228 0a20 2020 2020  .errorbar(.     
+00019330: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019340: 656c 662e 6365 6e74 6572 732c 0a20 2020  elf.centers,.   
+00019350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019360: 2062 636f 6e74 732c 0a20 2020 2020 2020   bconts,.       
+00019370: 2020 2020 2020 2020 2020 2020 2079 6572               yer
+00019380: 723d 2865 6d2c 2065 7029 2c0a 2020 2020  r=(em, ep),.    
+00019390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193a0: 666d 743d 225f 222c 0a20 2020 2020 2020  fmt="_",.       
+000193b0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+000193c0: 6f72 3d22 6461 726b 626c 7565 222c 0a20  or="darkblue",. 
+000193d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193e0: 2020 206d 6172 6b65 7273 697a 653d 3135     markersize=15
+000193f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00019400: 2020 2020 2020 6563 6f6c 6f72 3d22 6461        ecolor="da
+00019410: 726b 626c 7565 222c 0a20 2020 2020 2020  rkblue",.       
+00019420: 2020 2020 2020 2020 2020 2020 2061 6c70               alp
+00019430: 6861 3d30 2e38 2c0a 2020 2020 2020 2020  ha=0.8,.        
+00019440: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00019450: 2020 2020 2020 7265 7475 726e 2066 6967        return fig
+00019460: 0a0a 2020 2020 2020 2020 4073 7461 7469  ..        @stati
+00019470: 636d 6574 686f 640a 2020 2020 2020 2020  cmethod.        
+00019480: 6465 6620 506f 6973 736f 6e5f 4349 286c  def Poisson_CI(l
+00019490: 616d 2c20 7369 676d 613d 312e 3029 3a0a  am, sigma=1.0):.
+000194a0: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+000194b0: 2020 2020 2020 2020 2020 2020 6465 7465              dete
+000194c0: 726d 696e 6520 6f6e 652d 7369 676d 6120  rmine one-sigma 
+000194d0: 436f 6e66 6964 656e 6365 2049 6e74 6572  Confidence Inter
+000194e0: 7661 6c20 6172 6f75 6e64 2074 6865 0a20  val around the. 
+000194f0: 2020 2020 2020 2020 2020 206d 6561 6e20             mean 
+00019500: 6c61 6d62 6461 206f 6620 6120 506f 6973  lambda of a Pois
+00019510: 736f 6e20 6469 7374 7269 6275 7469 6f6e  son distribution
+00019520: 2c20 506f 6973 7328 782c 206c 616d 6264  , Poiss(x, lambd
+00019530: 6129 2e0a 0a20 2020 2020 2020 2020 2020  a)...           
+00019540: 2054 6865 206d 6574 686f 6420 6973 2062   The method is b
+00019550: 6173 6564 206f 6e20 6465 6c74 612d 6c6f  ased on delta-lo
+00019560: 672d 4c69 6b65 6c69 686f 6f64 2028 646c  g-Likelihood (dl
+00019570: 4c29 0a20 2020 2020 2020 2020 2020 206f  L).            o
+00019580: 6620 7468 6520 506f 6973 7369 6f6e 206c  f the Poission l
+00019590: 696b 656c 6968 6f6f 640a 0a20 2020 2020  ikelihood..     
+000195a0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000195b0: 2020 2020 2020 2020 2020 2d20 6c61 6d3a            - lam:
+000195c0: 206d 6561 6e20 6f66 2050 6f69 7373 696f   mean of Poissio
+000195d0: 6e20 6469 7374 7269 6275 7469 6f6e 0a20  n distribution. 
+000195e0: 2020 2020 2020 2020 2020 2020 2d20 636c              - cl
+000195f0: 3a20 6465 7369 7265 6420 636f 6e66 6964  : desired confid
+00019600: 656e 6365 206c 6576 656c 0a20 2020 2020  ence level.     
+00019610: 2020 2020 2020 2020 2d20 7369 676d 613a          - sigma:
+00019620: 2061 6c74 6572 6e61 7469 7665 6c79 2073   alternatively s
+00019630: 7065 6369 6679 2061 6e20 6e2d 7369 676d  pecify an n-sigm
+00019640: 6120 696e 7465 7276 616c 0a20 2020 2020  a interval.     
+00019650: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+00019660: 2020 2020 2020 2020 2320 6675 6e63 7469          # functi
+00019670: 6f6e 730a 2020 2020 2020 2020 2020 2020  ons.            
+00019680: 6465 6620 6e6c 4c50 6f69 7373 6f6e 2878  def nlLPoisson(x
+00019690: 2c20 6c61 6d29 3a0a 2020 2020 2020 2020  , lam):.        
+000196a0: 2020 2020 2020 2020 2222 226e 6567 6174          """negat
+000196b0: 6976 6520 6c6f 672d 6c69 6b65 6c69 686f  ive log-likeliho
+000196c0: 6f64 206f 6620 506f 6973 736f 696e 2064  od of Poissoin d
+000196d0: 6973 7472 6275 7469 6f6e 2222 220a 2020  istrbution""".  
+000196e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000196f0: 7475 726e 206c 616d 202d 2078 202a 206e  turn lam - x * n
+00019700: 702e 6c6f 6728 6c61 6d29 202b 206c 6f67  p.log(lam) + log
+00019710: 6761 6d6d 6128 7820 2b20 312e 3029 0a0a  gamma(x + 1.0)..
+00019720: 2020 2020 2020 2020 2020 2020 6465 6620              def 
+00019730: 6628 782c 206c 616d 2c20 646c 4c29 3a0a  f(x, lam, dlL):.
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 2222 2244 656c 7461 206c 6f67 2d4c 202d  """Delta log-L -
+00019760: 206f 6666 7365 742c 2069 6e70 7574 2074   offset, input t
+00019770: 6f20 4e65 7774 6f6e 206d 6574 686f 6422  o Newton method"
+00019780: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+00019790: 2020 2072 6574 7572 6e20 6e6c 4c50 6f69     return nlLPoi
+000197a0: 7373 6f6e 2878 2c20 6c61 6d29 202d 206e  sson(x, lam) - n
+000197b0: 6c4c 506f 6973 736f 6e28 6c61 6d2c 206c  lLPoisson(lam, l
+000197c0: 616d 2920 2d20 646c 4c0a 0a20 2020 2020  am) - dlL..     
+000197d0: 2020 2020 2020 2064 6c4c 203d 2030 2e35         dlL = 0.5
+000197e0: 202a 2073 6967 6d61 202a 2073 6967 6d61   * sigma * sigma
+000197f0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00019800: 666f 7220 646c 4c3d 302e 352c 2074 6865  for dlL=0.5, the
+00019810: 7265 2069 7320 6f6e 6c79 206f 6e65 2069  re is only one i
+00019820: 6e74 6572 7365 6374 696f 6e20 7769 7468  ntersection with
+00019830: 207a 6572 6f20 666f 7220 6c61 6d3c 312e   zero for lam<1.
+00019840: 380a 2020 2020 2020 2020 2020 2020 646c  8.            dl
+00019850: 203d 2031 2e32 202a 206e 702e 7371 7274   = 1.2 * np.sqrt
+00019860: 286c 616d 290a 2020 2020 2020 2020 2020  (lam).          
+00019870: 2020 646c 6d20 3d20 6d69 6e28 646c 2c20    dlm = min(dl, 
+00019880: 6c61 6d29 0a20 2020 2020 2020 2020 2020  lam).           
+00019890: 2063 7020 3d20 6e65 7774 6f6e 2866 2c20   cp = newton(f, 
+000198a0: 7830 3d6c 616d 202b 2064 6c2c 2078 313d  x0=lam + dl, x1=
+000198b0: 6c61 6d2c 2061 7267 733d 286c 616d 2c20  lam, args=(lam, 
+000198c0: 646c 4c29 290a 2020 2020 2020 2020 2020  dlL)).          
+000198d0: 2020 7472 793a 2020 2320 6d61 7920 6e6f    try:  # may no
+000198e0: 7420 636f 6e76 6572 6765 2066 6f72 2073  t converge for s
+000198f0: 6d61 6c6c 206c 616d 6264 612c 2061 7320  mall lambda, as 
+00019900: 7468 6572 6520 6973 206e 6f20 696e 7465  there is no inte
+00019910: 7273 6563 7469 6f6e 203c 206c 616d 0a20  rsection < lam. 
+00019920: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00019930: 6d20 3d20 6e65 7774 6f6e 2866 2c20 7830  m = newton(f, x0
+00019940: 3d6c 616d 202d 2064 6c6d 2c20 7831 3d6c  =lam - dlm, x1=l
+00019950: 616d 2c20 6172 6773 3d28 6c61 6d2c 2064  am, args=(lam, d
+00019960: 6c4c 2929 0a20 2020 2020 2020 2020 2020  lL)).           
+00019970: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+00019980: 2020 2020 2020 2020 2063 6d20 3d20 302e           cm = 0.
+00019990: 300a 2020 2020 2020 2020 2020 2020 6966  0.            if
+000199a0: 2028 6370 202d 2063 6d29 203c 206c 616d   (cp - cm) < lam
+000199b0: 202f 2031 3030 2e30 3a20 2023 2066 6f75   / 100.0:  # fou
+000199c0: 6e64 2073 616d 6520 696e 7465 7273 6563  nd same intersec
+000199d0: 7469 6f6e 2c0a 2020 2020 2020 2020 2020  tion,.          
+000199e0: 2020 2020 2020 636d 203d 2030 2e30 2020        cm = 0.0  
+000199f0: 2320 2073 6574 2031 7374 206f 6e65 2074  #  set 1st one t
+00019a00: 6f20 302e 0a0a 2020 2020 2020 2020 2020  o 0...          
+00019a10: 2020 7265 7475 726e 2063 6d2c 2063 700a    return cm, cp.
+00019a20: 0a20 2020 2023 202d 2d2d 2063 6f73 7420  .    # --- cost 
+00019a30: 6675 6e63 7469 6f6e 2066 6f72 2068 6973  function for his
+00019a40: 746f 6772 616d 2064 6174 610a 2020 2020  togram data.    
+00019a50: 636c 6173 7320 6843 6f73 743a 0a20 2020  class hCost:.   
+00019a60: 2020 2020 2022 2222 436f 7374 2066 756e       """Cost fun
+00019a70: 6374 696f 6e20 666f 7220 6269 6e6e 6564  ction for binned
+00019a80: 2064 6174 610a 0a20 2020 2020 2020 2054   data..        T
+00019a90: 6865 205f 5f63 616c 6c5f 5f20 6d65 7468  he __call__ meth
+00019aa0: 6f64 206f 6620 7468 6973 2063 6c61 7373  od of this class
+00019ab0: 2069 7320 6361 6c6c 6564 2062 7920 696d   is called by im
+00019ac0: 696e 7569 742e 0a0a 2020 2020 2020 2020  inuit...        
+00019ad0: 5468 6520 6465 6661 756c 7420 636f 7374  The default cost
+00019ae0: 2066 756e 6374 696f 6e20 746f 206d 696e   function to min
+00019af0: 696d 6f7a 6520 6973 2074 7769 6365 2074  imoze is twice t
+00019b00: 6865 206e 6567 6174 6976 650a 2020 2020  he negative.    
+00019b10: 2020 2020 6c6f 672d 6c69 6b65 6c69 686f      log-likeliho
+00019b20: 6f64 206f 6620 7468 6520 506f 6973 736f  od of the Poisso
+00019b30: 6e20 6469 7374 7269 6275 7469 6f6e 2067  n distribution g
+00019b40: 656e 6572 616c 697a 6564 2074 6f0a 2020  eneralized to.  
+00019b50: 2020 2020 2020 636f 6e74 696e 756f 7573        continuous
+00019b60: 206f 6273 6572 7661 7469 6f6e 7320 7820   observations x 
+00019b70: 6279 2072 6570 6c61 6369 6e67 206b 2120  by replacing k! 
+00019b80: 6279 2074 6865 2067 616d 6d61 2066 756e  by the gamma fun
+00019b90: 6374 696f 6e3a 0a0a 2020 2020 2020 2020  ction:..        
+00019ba0: 2e2e 206d 6174 683a 3a0a 2020 2020 2020  .. math::.      
+00019bb0: 2020 2020 2020 636f 7374 2878 3b5c 6c61        cost(x;\la
+00019bc0: 6d62 6461 2920 3d20 3220 5c6c 616d 6264  mbda) = 2 \lambd
+00019bd0: 6120 285c 6c61 6d62 6461 202d 2078 2a5c  a (\lambda - x*\
+00019be0: 6c6e 285c 6c61 6d62 6461 2920 2b20 5c6c  ln(\lambda) + \l
+00019bf0: 6e5c 4761 6d6d 6128 782b 312e 2929 0a0a  n\Gamma(x+1.))..
+00019c00: 2020 2020 2020 2020 416c 7465 726e 6174          Alternat
+00019c10: 6976 656c 792c 2074 6865 2047 6175 7373  ively, the Gauss
+00019c20: 6961 6e20 6170 7072 6f78 696d 6174 696f  ian approximatio
+00019c30: 6e20 6973 2061 7661 696c 6162 6c65 3a0a  n is available:.
+00019c40: 0a20 2020 2020 2020 202e 2e20 6d61 7468  .        .. math
+00019c50: 3a3a 0a20 2020 2020 2020 2020 2020 2063  ::.            c
+00019c60: 6f73 7428 783b 5c6c 616d 6264 6129 203d  ost(x;\lambda) =
+00019c70: 2028 7820 2d20 5c6c 616d 6264 6129 5e32   (x - \lambda)^2
+00019c80: 202f 205c 6c61 6d62 6461 202b 205c 6c6e   / \lambda + \ln
+00019c90: 285c 6c61 6d62 6461 290a 0a20 2020 2020  (\lambda)..     
+00019ca0: 2020 2054 6865 2069 6d70 6c65 6d65 6e74     The implement
+00019cb0: 6174 696f 6e20 616c 736f 2070 6572 6d69  ation also permi
+00019cc0: 7473 2074 6f20 7368 6966 7420 7468 6520  ts to shift the 
+00019cd0: 6f62 7365 7276 6174 696f 6e20 7820 6279  observation x by
+00019ce0: 2061 6e0a 2020 2020 2020 2020 6f66 6673   an.        offs
+00019cf0: 6574 2074 6f20 7461 6b65 2069 6e74 6f20  et to take into 
+00019d00: 6163 636f 756e 7420 636f 7272 6563 7469  account correcti
+00019d10: 6f6e 7320 746f 2074 6865 206e 756d 6265  ons to the numbe
+00019d20: 7220 6f66 206f 6273 6572 7665 640a 2020  r of observed.  
+00019d30: 2020 2020 2020 6269 6e20 656e 7472 6965        bin entrie
+00019d40: 7320 2865 2e67 2e20 6475 6520 746f 2062  s (e.g. due to b
+00019d50: 6163 6b67 726f 756e 6420 6f72 2065 6666  ackground or eff
+00019d60: 6963 6965 6e63 7920 636f 7272 6563 7469  iciency correcti
+00019d70: 6f6e 7329 3a0a 2020 2020 2020 2020 7820  ons):.        x 
+00019d80: 2d3e 2078 2d64 656c 7461 4d75 2077 6974  -> x-deltaMu wit
+00019d90: 6820 6465 6c74 614d 7520 3d20 6d75 202d  h deltaMu = mu -
+00019da0: 206c 616d 6264 612c 2077 6865 7265 206d   lambda, where m
+00019db0: 7520 6973 2074 6865 206d 6561 6e0a 2020  u is the mean.  
+00019dc0: 2020 2020 2020 6f66 2074 6865 2073 6869        of the shi
+00019dd0: 6674 6564 2050 6f69 7373 6f6e 206f 7220  fted Poisson or 
+00019de0: 4761 75c3 9f20 6469 7374 7269 6275 7469  Gau.. distributi
+00019df0: 6f6e 2e0a 0a20 2020 2020 2020 2054 6865  on...        The
+00019e00: 206e 756d 6265 7220 6f66 2062 696e 2065   number of bin e
+00019e10: 6e74 7269 6573 2070 7265 6469 6374 6564  ntries predicted
+00019e20: 2062 7920 7468 6520 6d6f 6465 6c20 6465   by the model de
+00019e30: 6e73 6974 7920 6973 2063 616c 6375 6c61  nsity is calcula
+00019e40: 7465 640a 2020 2020 2020 2020 6279 2061  ted.        by a
+00019e50: 6e20 6170 7072 6f78 696d 6174 6520 696e  n approximate in
+00019e60: 7465 6772 616c 206f 7665 7220 7468 6520  tegral over the 
+00019e70: 7265 7370 6563 7469 7665 2062 696e 2072  respective bin r
+00019e80: 616e 6765 7320 7573 696e 6720 7468 650a  anges using the.
+00019e90: 2020 2020 2020 2020 5369 6d70 736f 6e20          Simpson 
+00019ea0: 7275 6c65 2e0a 0a20 2020 2020 2020 2054  rule...        T
+00019eb0: 6f20 6a75 6467 6520 7468 6520 6c65 7665  o judge the leve
+00019ec0: 6c20 6f66 2061 6772 6565 6d65 6e74 206f  l of agreement o
+00019ed0: 6620 6d6f 6465 6c20 6465 6e73 6974 7920  f model density 
+00019ee0: 616e 6420 6869 7374 6f67 7261 6d20 6461  and histogram da
+00019ef0: 7461 2c0a 2020 2020 2020 2020 6120 2267  ta,.        a "g
+00019f00: 6f6f 646e 6573 732d 6f66 2d66 6974 2220  oodness-of-fit" 
+00019f10: 282a 676f 662a 2920 7661 6c75 6520 6973  (*gof*) value is
+00019f20: 2063 616c 756c 6174 6564 2061 7320 7468   calulated as th
+00019f30: 6520 6c69 6b65 6c69 686f 6f64 2d72 6174  e likelihood-rat
+00019f40: 696f 206f 660a 2020 2020 2020 2020 7468  io of.        th
+00019f50: 6520 6d6f 6465 6c20 772e 722e 742e 2074  e model w.r.t. t
+00019f60: 6865 2064 6174 6120 616e 6420 7468 6520  he data and the 
+00019f70: 736f 2d63 616c 6c65 6420 2273 6174 7572  so-called "satur
+00019f80: 6174 6564 206d 6f64 656c 2220 6465 7363  ated model" desc
+00019f90: 7269 6269 6e67 0a20 2020 2020 2020 2074  ribing.        t
+00019fa0: 6865 2064 6174 6120 7065 7266 6563 746c  he data perfectl
+00019fb0: 792c 2069 2e65 2e20 203a 6d61 7468 3a60  y, i.e.  :math:`
+00019fc0: 636f 7374 5f7b 7361 747d 2878 2920 3d20  cost_{sat}(x) = 
+00019fd0: 636f 7374 2878 3b20 5c6c 616d 6264 613d  cost(x; \lambda=
+00019fe0: 7829 602e 0a20 2020 2020 2020 2049 6620  x)`..        If 
+00019ff0: 7468 6520 6269 6e20 656e 7472 6965 7320  the bin entries 
+0001a000: 6172 6520 7375 6666 6963 6965 6e74 6c79  are sufficiently
+0001a010: 206c 6172 6765 2c20 2a67 6f66 2a20 636f   large, *gof* co
+0001a020: 6e76 6572 6765 7320 746f 2074 6865 2073  nverges to the s
+0001a030: 7461 6e64 6172 640a 2020 2020 2020 2020  tandard.        
+0001a040: 2a63 6869 322a 2076 616c 7565 2e0a 0a20  *chi2* value... 
+0001a050: 2020 2020 2020 2049 6e70 7574 3a0a 0a20         Input:.. 
+0001a060: 2020 2020 2020 202d 206f 7574 6572 3a20         - outer: 
+0001a070: 706f 696e 7465 7220 746f 2069 6e73 7461  pointer to insta
+0001a080: 6e63 6520 6f66 2063 616c 6c69 6e67 2063  nce of calling c
+0001a090: 6c61 7373 0a20 2020 2020 2020 202d 206d  lass.        - m
+0001a0a0: 6f64 656c 3a20 6d6f 6465 6c20 6675 6e63  odel: model func
+0001a0b0: 7469 6f6e 2066 2878 2c20 5c2a 7061 7229  tion f(x, \*par)
+0001a0c0: 0a20 2020 2020 2020 202d 2075 7365 5f47  .        - use_G
+0001a0d0: 6175 7373 4170 7072 6f78 2c20 626f 6f6c  aussApprox, bool
+0001a0e0: 3a20 7573 6520 4761 7573 7369 616e 2061  : use Gaussian a
+0001a0f0: 7070 726f 7869 6d61 7469 6f6e 0a20 2020  pproximation.   
+0001a100: 2020 2020 202d 2064 656e 7369 7479 2c20       - density, 
+0001a110: 626f 6f6c 3a20 6669 7420 6120 6e6f 726d  bool: fit a norm
+0001a120: 616c 6973 6564 2064 656e 7369 7479 3b20  alised density; 
+0001a130: 6966 2046 616c 7365 2c20 616e 206f 7665  if False, an ove
+0001a140: 7261 6c6c 0a20 2020 2020 2020 2020 206e  rall.          n
+0001a150: 6f72 6d61 6c69 7361 7469 6f6e 206d 7573  ormalisation mus
+0001a160: 7420 6265 2070 726f 7669 6465 6420 696e  t be provided in
+0001a170: 2074 6865 206d 6f64 656c 2066 756e 6374   the model funct
+0001a180: 696f 6e0a 0a20 2020 2020 2020 2044 6174  ion..        Dat
+0001a190: 6120 6d65 6d62 6572 733a 0a0a 2020 2020  a members:..    
+0001a1a0: 2020 2020 2d20 6e64 6f66 3a20 6465 6772      - ndof: degr
+0001a1b0: 6565 7320 6f66 2066 7265 6564 6f6d 0a20  ees of freedom. 
+0001a1c0: 2020 2020 2020 202d 206e 636f 6e73 7472         - nconstr
+0001a1d0: 6169 6e74 733a 206e 756d 6265 7220 6f66  aints: number of
+0001a1e0: 2070 6172 616d 6574 6572 2063 6f6e 7374   parameter const
+0001a1f0: 7261 696e 7473 0a20 2020 2020 2020 202d  raints.        -
+0001a200: 2067 6f66 3a20 676f 6f64 6e65 7373 2d6f   gof: goodness-o
+0001a210: 662d 6669 7420 6173 206c 696b 656c 6968  f-fit as likelih
+0001a220: 6f6f 6420 7261 7469 6f20 772e 722e 742e  ood ratio w.r.t.
+0001a230: 2074 6865 2027 7361 7475 7261 7465 6420   the 'saturated 
+0001a240: 6d6f 6465 6c27 0a0a 2020 2020 2020 2020  model'..        
+0001a250: 4578 7465 726e 616c 2072 6566 6572 656e  External referen
+0001a260: 6365 733a 0a0a 2020 2020 2020 2020 2d20  ces:..        - 
+0001a270: 6d6f 6465 6c28 782c 205c 2a70 6172 293a  model(x, \*par):
+0001a280: 2074 6865 206d 6f64 656c 2066 756e 6374   the model funct
+0001a290: 696f 6e0a 2020 2020 2020 2020 2d20 6461  ion.        - da
+0001a2a0: 7461 3a20 706f 696e 7465 7220 746f 2069  ta: pointer to i
+0001a2b0: 6e73 7461 6e63 6520 6f66 2063 6c61 7373  nstance of class
+0001a2c0: 2068 6973 7444 6174 610a 2020 2020 2020   histData.      
+0001a2d0: 2020 2d20 6461 7461 2e6d 6f64 656c 5f76    - data.model_v
+0001a2e0: 616c 7565 733a 2062 696e 2065 6e74 7269  alues: bin entri
+0001a2f0: 6573 2063 616c 6375 6c61 7465 6420 6279  es calculated by
+0001a300: 2074 6865 2062 6573 742d 6669 7420 6d6f   the best-fit mo
+0001a310: 6465 6c0a 2020 2020 2020 2020 2222 220a  del.        """.
+0001a320: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
+0001a330: 6e69 745f 5f28 7365 6c66 2c20 6f75 7465  nit__(self, oute
+0001a340: 722c 206d 6f64 656c 2c20 7573 655f 4761  r, model, use_Ga
+0001a350: 7573 7341 7070 726f 783d 4661 6c73 652c  ussApprox=False,
+0001a360: 2064 656e 7369 7479 3d54 7275 6529 3a0a   density=True):.
+0001a370: 2020 2020 2020 2020 2020 2020 2320 6461              # da
+0001a380: 7461 206f 626a 6563 7420 6f66 2074 7970  ta object of typ
+0001a390: 6520 6869 7374 4461 7461 436f 6e74 6169  e histDataContai
+0001a3a0: 6e74 6572 0a20 2020 2020 2020 2020 2020  nter.           
+0001a3b0: 2073 656c 662e 6461 7461 203d 206f 7574   self.data = out
+0001a3c0: 6572 2e68 4461 7461 0a20 2020 2020 2020  er.hData.       
+0001a3d0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
+0001a3e0: 7374 616e 6365 2873 656c 662e 6461 7461  stance(self.data
+0001a3f0: 2c20 6d6e 4669 742e 6869 7374 4461 7461  , mnFit.histData
+0001a400: 436f 6e74 6169 6e65 7229 3a0a 2020 2020  Container):.    
+0001a410: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0001a420: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
+0001a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a440: 2020 2220 2121 2120 6d6e 4669 742e 6843    " !!! mnFit.hC
+0001a450: 6f73 743a 2065 7870 6563 7469 6e67 2064  ost: expecting d
+0001a460: 6174 6120 636f 6e74 6169 6e65 7220 6f66  ata container of
+0001a470: 2074 7970 6520 2768 6973 7444 6174 6143   type 'histDataC
+0001a480: 6f6e 7461 696e 6572 2722 0a20 2020 2020  ontainer'".     
+0001a490: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0001a4a0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+0001a4b0: 6f64 656c 203d 206d 6f64 656c 0a20 2020  odel = model.   
+0001a4c0: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+0001a4d0: 6e73 6974 7920 3d20 6465 6e73 6974 790a  nsity = density.
+0001a4e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a4f0: 2e47 6175 7373 4170 7072 6f78 203d 2075  .GaussApprox = u
+0001a500: 7365 5f47 6175 7373 4170 7072 6f78 0a20  se_GaussApprox. 
+0001a510: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a520: 7175 6965 7420 3d20 6f75 7465 722e 7175  quiet = outer.qu
+0001a530: 6965 740a 0a20 2020 2020 2020 2020 2020  iet..           
+0001a540: 2023 2073 6574 2070 726f 7065 7220 7369   # set proper si
+0001a550: 676e 6174 7572 6520 6f66 206d 6f64 656c  gnature of model
+0001a560: 2066 756e 6374 696f 6e20 666f 7220 696d   function for im
+0001a570: 696e 7569 740a 2020 2020 2020 2020 2020  inuit.          
+0001a580: 2020 7365 6c66 2e70 6e61 6d73 203d 206f    self.pnams = o
+0001a590: 7574 6572 2e70 6e61 6d73 0a20 2020 2020  uter.pnams.     
+0001a5a0: 2020 2020 2020 2073 656c 662e 6e70 6172         self.npar
+0001a5b0: 203d 206f 7574 6572 2e6e 7061 720a 0a20   = outer.npar.. 
+0001a5c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a5d0: 636f 6e73 7472 6169 6e74 7320 3d20 6f75  constraints = ou
+0001a5e0: 7465 722e 636f 6e73 7472 6169 6e74 730a  ter.constraints.
+0001a5f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a600: 2e6e 636f 6e73 7472 6169 6e74 7320 3d20  .nconstraints = 
+0001a610: 6c65 6e28 7365 6c66 2e63 6f6e 7374 7261  len(self.constra
+0001a620: 696e 7473 290a 2020 2020 2020 2020 2020  ints).          
+0001a630: 2020 2320 7461 6b65 2061 6363 6f75 6e74    # take account
+0001a640: 206f 6620 636f 6e73 7472 6169 6e74 7320   of constraints 
+0001a650: 696e 2064 6567 7265 6573 206f 6620 6672  in degrees of fr
+0001a660: 6565 646f 6d0a 2020 2020 2020 2020 2020  eedom.          
+0001a670: 2020 7365 6c66 2e6e 646f 6620 3d20 7365    self.ndof = se
+0001a680: 6c66 2e64 6174 612e 6e62 696e 7320 2d20  lf.data.nbins - 
+0001a690: 7365 6c66 2e6e 7061 7220 2b20 7365 6c66  self.npar + self
+0001a6a0: 2e6e 636f 6e73 7472 6169 6e74 7320 2b20  .nconstraints + 
+0001a6b0: 6f75 7465 722e 6e66 6978 6564 0a0a 2020  outer.nfixed..  
+0001a6c0: 2020 2020 2020 2020 2020 2320 666c 6167            # flag
+0001a6d0: 2074 6f20 636f 6e74 726f 6c20 6669 6e61   to control fina
+0001a6e0: 6c20 6163 7469 6f6e 7320 696e 2063 6f73  l actions in cos
+0001a6f0: 7420 6675 6e63 7469 6f6e 0a20 2020 2020  t function.     
+0001a700: 2020 2020 2020 2073 656c 662e 6669 6e61         self.fina
+0001a710: 6c5f 6361 6c6c 203d 2046 616c 7365 0a0a  l_call = False..
+0001a720: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0001a730: 656c 662e 4761 7573 7341 7070 726f 783a  elf.GaussApprox:
+0001a740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a750: 2073 656c 662e 6e32 6c4c 636f 7374 203d   self.n2lLcost =
+0001a760: 2073 656c 662e 6e32 6c4c 4761 7573 730a   self.n2lLGauss.
+0001a770: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001a780: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001a790: 2020 7365 6c66 2e6e 326c 4c63 6f73 7420    self.n2lLcost 
+0001a7a0: 3d20 7365 6c66 2e6e 326c 4c50 6f69 7373  = self.n2lLPoiss
+0001a7b0: 6f6e 0a0a 2020 2020 2020 2020 2020 2020  on..            
+0001a7c0: 6966 2073 656c 662e 6465 6e73 6974 793a  if self.density:
+0001a7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a7e0: 2073 656c 662e 6e6f 726d 203d 2073 656c   self.norm = sel
+0001a7f0: 662e 6461 7461 2e4e 746f 740a 2020 2020  f.data.Ntot.    
+0001a800: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001a810: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001a820: 6c66 2e6e 6f72 6d20 3d20 312e 300a 0a20  lf.norm = 1.0.. 
+0001a830: 2020 2020 2020 2064 6566 205f 5f63 616c         def __cal
+0001a840: 6c5f 5f28 7365 6c66 2c20 2a70 6172 293a  l__(self, *par):
+0001a850: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+0001a860: 616c 6c65 6420 6974 6572 6174 6976 656c  alled iterativel
+0001a870: 7920 6279 206d 696e 7569 740a 0a20 2020  y by minuit..   
+0001a880: 2020 2020 2020 2020 2023 2063 6f73 7420           # cost 
+0001a890: 6675 6e63 7469 6f6e 2069 7320 6c69 6b65  function is like
+0001a8a0: 6c69 686f 6f64 206f 6620 7368 6966 7465  lihood of shifte
+0001a8b0: 6420 506f 6973 736f 6e20 6f72 2047 6175  d Poisson or Gau
+0001a8c0: 7373 2061 7070 726f 7869 6d61 7469 6f6e  ss approximation
+0001a8d0: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001a8e0: 2d20 6669 7273 742c 2074 616b 6520 696e  - first, take in
+0001a8f0: 746f 2061 6363 6f75 6e74 2070 6f73 7369  to account possi
+0001a900: 626c 6520 7061 7261 6d65 7465 7220 636f  ble parameter co
+0001a910: 6e73 7472 6169 6e74 730a 2020 2020 2020  nstraints.      
+0001a920: 2020 2020 2020 6e32 6c4c 203d 2030 2e30        n2lL = 0.0
+0001a930: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a940: 7365 6c66 2e6e 636f 6e73 7472 6169 6e74  self.nconstraint
+0001a950: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0001a960: 2020 2066 6f72 2063 2069 6e20 7365 6c66     for c in self
+0001a970: 2e63 6f6e 7374 7261 696e 7473 3a0a 2020  .constraints:.  
+0001a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a990: 2020 705f 6964 203d 2063 5b30 5d0a 2020    p_id = c[0].  
+0001a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9b0: 2020 7220 3d20 2870 6172 5b70 5f69 645d    r = (par[p_id]
+0001a9c0: 202d 2063 5b31 5d29 202f 2063 5b32 5d0a   - c[1]) / c[2].
+0001a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9e0: 2020 2020 6e32 6c4c 202b 3d20 7220 2a20      n2lL += r * 
+0001a9f0: 720a 0a20 2020 2020 2020 2020 2020 2023  r..            #
+0001aa00: 202d 2063 616c 6375 6c61 7465 2032 2a6e   - calculate 2*n
+0001aa10: 6567 4c6f 674c 2050 6f69 7373 6f6e 3b0a  egLogL Poisson;.
+0001aa20: 2020 2020 2020 2020 2020 2020 2320 206d              #  m
+0001aa30: 6f64 656c 2070 7265 6469 6374 696f 6e20  odel prediction 
+0001aa40: 6173 2061 7070 726f 7869 6d61 7465 2069  as approximate i
+0001aa50: 6e74 6567 7261 6c20 6f76 6572 2062 696e  ntegral over bin
+0001aa60: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+0001aa70: 656c 5f76 616c 7565 7320 3d20 7365 6c66  el_values = self
+0001aa80: 2e6e 6f72 6d20 2a20 7365 6c66 2e69 6e74  .norm * self.int
+0001aa90: 6567 7261 6c5f 6f76 6572 4269 6e73 280a  egral_overBins(.
+0001aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aab0: 7365 6c66 2e64 6174 612e 6c65 6674 732c  self.data.lefts,
+0001aac0: 2073 656c 662e 6461 7461 2e72 6967 6874   self.data.right
+0001aad0: 732c 2073 656c 662e 6d6f 6465 6c2c 202a  s, self.model, *
+0001aae0: 7061 720a 2020 2020 2020 2020 2020 2020  par.            
+0001aaf0: 290a 2020 2020 2020 2020 2020 2020 230a  ).            #.
+0001ab00: 0a20 2020 2020 2020 2020 2020 206e 326c  .            n2l
+0001ab10: 4c20 2b3d 206e 702e 7375 6d28 0a20 2020  L += np.sum(.   
+0001ab20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001ab30: 662e 6e32 6c4c 636f 7374 280a 2020 2020  f.n2lLcost(.    
+0001ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab50: 7365 6c66 2e64 6174 612e 636f 6e74 656e  self.data.conten
+0001ab60: 7473 202d 2073 656c 662e 6461 7461 2e44  ts - self.data.D
+0001ab70: 656c 7461 4d75 2c0a 2020 2020 2020 2020  eltaMu,.        
+0001ab80: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+0001ab90: 6c5f 7661 6c75 6573 202b 206e 702e 6162  l_values + np.ab
+0001aba0: 7328 7365 6c66 2e64 6174 612e 4465 6c74  s(self.data.Delt
+0001abb0: 614d 7529 2c0a 2020 2020 2020 2020 2020  aMu),.          
+0001abc0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001abd0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+0001abe0: 2020 2069 6620 7365 6c66 2e66 696e 616c     if self.final
+0001abf0: 5f63 616c 6c3a 0a20 2020 2020 2020 2020  _call:.         
+0001ac00: 2020 2020 2020 2069 6620 7365 6c66 2e47         if self.G
+0001ac10: 6175 7373 4170 7072 6f78 3a0a 2020 2020  aussApprox:.    
+0001ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac30: 2320 7265 7475 726e 2073 7461 6e64 6172  # return standar
+0001ac40: 6420 6368 695e 320a 2020 2020 2020 2020  d chi^2.        
+0001ac50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ac60: 2e67 6f66 203d 2028 0a20 2020 2020 2020  .gof = (.       
+0001ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac80: 206e 326c 4c20 2d20 6e70 2e6c 6f67 286d   n2lL - np.log(m
+0001ac90: 6f64 656c 5f76 616c 7565 7320 2b20 6e70  odel_values + np
+0001aca0: 2e61 6273 2873 656c 662e 6461 7461 2e44  .abs(self.data.D
+0001acb0: 656c 7461 4d75 2929 2e73 756d 2829 0a20  eltaMu)).sum(). 
+0001acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acd0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001ace0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001acf0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001ad00: 2073 746f 7265 2067 6f6f 646e 6573 732d   store goodness-
+0001ad10: 6f66 2d66 6974 2028 6469 6666 6572 656e  of-fit (differen
+0001ad20: 6365 206f 6620 6e6c 4c32 2077 2e72 2e74  ce of nlL2 w.r.t
+0001ad30: 2e20 7361 7475 7261 7465 6420 6d6f 6465  . saturated mode
+0001ad40: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
+0001ad50: 2020 2020 2020 206e 326c 4c5f 7361 7475         n2lL_satu
+0001ad60: 7261 7465 6420 3d20 6e70 2e73 756d 280a  rated = np.sum(.
 0001ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad80: 2073 656c 662e 6e32 6c4c 636f 7374 280a   self.n2lLcost(.
-0001ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ada0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001adb0: 2e64 6174 612e 636f 6e74 656e 7473 202d  .data.contents -
-0001adc0: 2073 656c 662e 6461 7461 2e44 656c 7461   self.data.Delta
-0001add0: 4d75 2c0a 2020 2020 2020 2020 2020 2020  Mu,.            
+0001ad80: 2020 2020 2020 2020 7365 6c66 2e6e 326c          self.n2l
+0001ad90: 4c63 6f73 7428 0a20 2020 2020 2020 2020  Lcost(.         
+0001ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001adb0: 2020 2073 656c 662e 6461 7461 2e63 6f6e     self.data.con
+0001adc0: 7465 6e74 7320 2d20 7365 6c66 2e64 6174  tents - self.dat
+0001add0: 612e 4465 6c74 614d 752c 0a20 2020 2020  a.DeltaMu,.     
 0001ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adf0: 7365 6c66 2e64 6174 612e 636f 6e74 656e  self.data.conten
-0001ae00: 7473 202b 206e 702e 6162 7328 7365 6c66  ts + np.abs(self
-0001ae10: 2e64 6174 612e 4465 6c74 614d 7529 202b  .data.DeltaMu) +
-0001ae20: 2030 2e30 3035 2c0a 2020 2020 2020 2020   0.005,.        
+0001adf0: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
+0001ae00: 2e63 6f6e 7465 6e74 7320 2b20 6e70 2e61  .contents + np.a
+0001ae10: 6273 2873 656c 662e 6461 7461 2e44 656c  bs(self.data.Del
+0001ae20: 7461 4d75 2920 2b20 302e 3030 352c 0a20  taMu) + 0.005,. 
 0001ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001ae50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0001ae60: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0001ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae80: 2020 2020 2020 2020 2020 2020 2021 2121               !!!
-0001ae90: 2063 6f6e 7374 2e20 302e 3030 3520 746f   const. 0.005 to
-0001aea0: 2061 766f 6964 206c 6f67 2830 2e29 0a20   avoid log(0.). 
-0001aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aec0: 2020 2073 656c 662e 676f 6620 3d20 6e32     self.gof = n2
-0001aed0: 6c4c 202d 206e 326c 4c5f 7361 7475 7261  lL - n2lL_satura
-0001aee0: 7465 640a 0a20 2020 2020 2020 2020 2020  ted..           
-0001aef0: 2020 2020 2023 2070 726f 7669 6465 206d       # provide m
-0001af00: 6f64 656c 2076 616c 7565 7320 616e 6420  odel values and 
-0001af10: 6d6f 6465 6c2d 7265 6c61 7465 6420 756e  model-related un
-0001af20: 6365 7274 6169 6e74 6965 7320 746f 2064  certainties to d
-0001af30: 6174 6120 6f62 6a65 6374 0a20 2020 2020  ata object.     
-0001af40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001af50: 6461 7461 2e6d 6f64 656c 5f76 616c 7565  data.model_value
-0001af60: 7320 3d20 6d6f 6465 6c5f 7661 6c75 6573  s = model_values
-0001af70: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0001af80: 7265 7475 726e 2032 202a 206e 6567 2e20  return 2 * neg. 
-0001af90: 6c6f 674c 0a20 2020 2020 2020 2020 2020  logL.           
-0001afa0: 2072 6574 7572 6e20 6e32 6c4c 0a0a 2020   return n2lL..  
-0001afb0: 2020 2020 2020 4073 7461 7469 636d 6574        @staticmet
-0001afc0: 686f 640a 2020 2020 2020 2020 6465 6620  hod.        def 
-0001afd0: 6e32 6c4c 506f 6973 736f 6e28 782c 206c  n2lLPoisson(x, l
-0001afe0: 616d 293a 0a20 2020 2020 2020 2020 2020  am):.           
-0001aff0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
-0001b000: 206e 6567 2e20 6c6f 6761 7269 7468 6d20   neg. logarithm 
-0001b010: 6f66 2050 6f69 7373 6f6e 2064 6973 7472  of Poisson distr
-0001b020: 6962 7574 696f 6e20 666f 7220 7265 616c  ibution for real
-0001b030: 2d76 616c 7565 6420 780a 0a20 2020 2020  -valued x..     
-0001b040: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001b050: 2020 2020 2020 2072 6574 7572 6e20 322e         return 2.
-0001b060: 3020 2a20 286c 616d 202d 2078 202a 206e  0 * (lam - x * n
-0001b070: 702e 6c6f 6728 6c61 6d29 202b 206c 6f67  p.log(lam) + log
-0001b080: 6761 6d6d 6128 7820 2b20 312e 3029 290a  gamma(x + 1.0)).
-0001b090: 0a20 2020 2020 2020 2040 7374 6174 6963  .        @static
-0001b0a0: 6d65 7468 6f64 0a20 2020 2020 2020 2064  method.        d
-0001b0b0: 6566 206e 326c 4c73 506f 6973 736f 6e28  ef n2lLsPoisson(
-0001b0c0: 786b 2c20 6c61 6d2c 206d 7529 3a0a 2020  xk, lam, mu):.  
-0001b0d0: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
-0001b0e0: 2020 2020 2020 2020 2020 322a 206e 6567            2* neg
-0001b0f0: 2e20 6c6f 6761 7269 7468 6d20 6f66 2067  . logarithm of g
-0001b100: 656e 6572 616c 697a 6564 2050 6f69 7373  eneralized Poiss
-0001b110: 6f6e 2064 6973 7472 6962 7574 696f 6e3a  on distribution:
-0001b120: 0a20 2020 2020 2020 2020 2020 2073 6869  .            shi
-0001b130: 6674 6564 2074 6f20 6e65 7720 6d65 616e  fted to new mean
-0001b140: 206d 7520 666f 7220 7265 616c 2d76 616c   mu for real-val
-0001b150: 7565 6420 786b 0a20 2020 2020 2020 2020  ued xk.         
-0001b160: 2020 2066 6f72 206c 616d 3d6d 752c 2074     for lam=mu, t
-0001b170: 6865 2073 7461 6e64 6172 6420 506f 6973  he standard Pois
-0001b180: 736f 6e20 6469 7374 7269 6275 7469 6f6e  son distribution
-0001b190: 2069 7320 7265 636f 7665 7265 640a 2020   is recovered.  
-0001b1a0: 2020 2020 2020 2020 2020 6c61 6d3d 7369            lam=si
-0001b1b0: 676d 612a 3220 6973 2074 6865 2076 6172  gma*2 is the var
-0001b1c0: 6961 6e63 6520 6f66 2074 6865 2073 6869  iance of the shi
-0001b1d0: 6674 6564 2050 6f69 7373 6f6e 2064 6973  fted Poisson dis
-0001b1e0: 7472 6962 7574 696f 6e2e 0a20 2020 2020  tribution..     
-0001b1f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001b200: 2020 2020 2020 2078 7320 3d20 786b 202b         xs = xk +
-0001b210: 206c 616d 202d 206d 750a 2020 2020 2020   lam - mu.      
-0001b220: 2020 2020 2020 7265 7475 726e 2032 2e30        return 2.0
-0001b230: 202a 2028 6c61 6d20 2d20 7873 202a 206e   * (lam - xs * n
-0001b240: 702e 6c6f 6728 6c61 6d29 202b 206c 6f67  p.log(lam) + log
-0001b250: 6761 6d6d 6128 7873 202b 2031 2e30 2929  gamma(xs + 1.0))
-0001b260: 0a0a 2020 2020 2020 2020 4073 7461 7469  ..        @stati
-0001b270: 636d 6574 686f 640a 2020 2020 2020 2020  cmethod.        
-0001b280: 6465 6620 6e32 6c4c 4761 7573 7328 782c  def n2lLGauss(x,
-0001b290: 206c 616d 293a 0a20 2020 2020 2020 2020   lam):.         
-0001b2a0: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
-0001b2b0: 2020 206e 6567 6174 6976 6520 6c6f 672d     negative log-
-0001b2c0: 6c69 6b65 6c69 686f 6f64 206f 6620 4761  likelihood of Ga
-0001b2d0: 7573 7369 616e 2061 7070 726f 7869 6d61  ussian approxima
-0001b2e0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0001b2f0: 2050 6f69 7328 782c 206c 616d 2920 5c73   Pois(x, lam) \s
-0001b300: 696d 6571 2047 6175 7373 2878 2c20 6d75  imeq Gauss(x, mu
-0001b310: 3d6c 616d 2c20 7369 676d 615e 323d 6c61  =lam, sigma^2=la
-0001b320: 6d29 0a20 2020 2020 2020 2020 2020 2022  m).            "
-0001b330: 2222 0a20 2020 2020 2020 2020 2020 2072  "".            r
-0001b340: 203d 2078 202d 206c 616d 0a20 2020 2020   = x - lam.     
-0001b350: 2020 2020 2020 2072 6574 7572 6e20 7220         return r 
-0001b360: 2a20 7220 2f20 6c61 6d20 2b20 6e70 2e6c  * r / lam + np.l
-0001b370: 6f67 286c 616d 290a 0a20 2020 2020 2020  og(lam)..       
-0001b380: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-0001b390: 2020 2020 2020 2064 6566 2069 6e74 6567         def integ
-0001b3a0: 7261 6c5f 6f76 6572 4269 6e73 286c 6564  ral_overBins(led
-0001b3b0: 6765 732c 2072 6564 6765 732c 2066 2c20  ges, redges, f, 
-0001b3c0: 2a70 6172 293a 0a20 2020 2020 2020 2020  *par):.         
-0001b3d0: 2020 2022 2222 4361 6c63 756c 6174 6520     """Calculate 
-0001b3e0: 6170 7072 6f78 2e20 696e 7465 6772 616c  approx. integral
-0001b3f0: 206f 6620 6d6f 6465 6c20 6f76 6572 2062   of model over b
-0001b400: 696e 7320 7573 696e 6720 5369 6d70 736f  ins using Simpso
-0001b410: 6e27 7320 7275 6c65 2222 220a 2020 2020  n's rule""".    
-0001b420: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-0001b430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b440: 2028 7265 6467 6573 202d 206c 6564 6765   (redges - ledge
-0001b450: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-0001b460: 2020 202f 2036 2e30 0a20 2020 2020 2020     / 6.0.       
-0001b470: 2020 2020 2020 2020 202a 2028 0a20 2020           * (.   
-0001b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b490: 2066 286c 6564 6765 732c 202a 7061 7229   f(ledges, *par)
-0001b4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b4b0: 2020 2020 202b 2034 2e30 202a 2066 2828       + 4.0 * f((
-0001b4c0: 6c65 6467 6573 202b 2072 6564 6765 7329  ledges + redges)
-0001b4d0: 202f 2032 2e30 2c20 2a70 6172 290a 2020   / 2.0, *par).  
-0001b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4f0: 2020 2b20 6628 7265 6467 6573 2c20 2a70    + f(redges, *p
-0001b500: 6172 290a 2020 2020 2020 2020 2020 2020  ar).            
-0001b510: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0001b520: 2020 290a 0a20 2020 2023 202d 2d2d 2065    )..    # --- e
-0001b530: 6e64 2064 6566 696e 6974 696f 6e20 6f66  nd definition of
-0001b540: 2063 6c61 7373 2068 436f 7374 202d 2d2d   class hCost ---
-0001b550: 2d0a 0a20 2020 2023 0a20 2020 2023 202d  -..    #.    # -
-0001b560: 2d2d 2073 7065 6369 616c 2063 6f64 6520  -- special code 
-0001b570: 666f 7220 6669 7420 7769 7468 2075 7365  for fit with use
-0001b580: 722d 7375 7070 6c69 6564 2063 6f73 7420  r-supplied cost 
-0001b590: 6675 6e63 7469 6f6e 0a20 2020 2023 2020  function.    #  
-0001b5a0: 2020 206f 7220 7064 6620 666f 7220 6e65     or pdf for ne
-0001b5b0: 672e 206c 6f67 2d6c 696b 656c 6968 6f6f  g. log-likelihoo
-0001b5c0: 6420 6669 740a 2020 2020 230a 0a20 2020  d fit.    #..   
-0001b5d0: 2064 6566 2069 6e69 745f 6d6c 4461 7461   def init_mlData
-0001b5e0: 2873 656c 662c 2078 293a 0a20 2020 2020  (self, x):.     
-0001b5f0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0001b600: 6e69 7469 616c 697a 6520 6461 7461 206f  nitialize data o
-0001b610: 626a 6563 740a 0a20 2020 2020 2020 2041  bject..        A
-0001b620: 7267 733a 0a20 2020 2020 2020 202d 2078  rgs:.        - x
-0001b630: 2c20 6172 7261 7920 6f66 2066 6c6f 6174  , array of float
-0001b640: 730a 2020 2020 2020 2020 2222 220a 0a20  s.        """.. 
-0001b650: 2020 2020 2020 2023 2063 7265 6174 6520         # create 
-0001b660: 6461 7461 206f 626a 6563 7420 616e 6420  data object and 
-0001b670: 7061 7373 2061 6c6c 2069 6e70 7574 2061  pass all input a
-0001b680: 7267 756d 656e 7473 0a20 2020 2020 2020  rguments.       
-0001b690: 2073 656c 662e 6d6c 4461 7461 203d 2073   self.mlData = s
-0001b6a0: 656c 662e 6d6c 4461 7461 436f 6e74 6169  elf.mlDataContai
-0001b6b0: 6e65 7228 7365 6c66 2c20 7829 0a20 2020  ner(self, x).   
-0001b6c0: 2020 2020 2073 656c 662e 6461 7461 203d       self.data =
-0001b6d0: 2073 656c 662e 6d6c 4461 7461 0a0a 2020   self.mlData..  
-0001b6e0: 2020 6465 6620 696e 6974 5f6d 6e46 6974    def init_mnFit
-0001b6f0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0001b700: 2020 2020 2020 2020 7573 6572 4675 6e63          userFunc
-0001b710: 7469 6f6e 2c0a 2020 2020 2020 2020 6d6f  tion,.        mo
-0001b720: 6465 6c5f 6b77 6172 6773 3d4e 6f6e 652c  del_kwargs=None,
-0001b730: 0a20 2020 2020 2020 2070 303d 4e6f 6e65  .        p0=None
-0001b740: 2c0a 2020 2020 2020 2020 6470 303d 4e6f  ,.        dp0=No
-0001b750: 6e65 2c0a 2020 2020 2020 2020 636f 6e73  ne,.        cons
-0001b760: 7472 6169 6e74 733d 4e6f 6e65 2c0a 2020  traints=None,.  
-0001b770: 2020 2020 2020 6669 7850 6172 733d 4e6f        fixPars=No
-0001b780: 6e65 2c0a 2020 2020 2020 2020 6c69 6d69  ne,.        limi
-0001b790: 7473 3d4e 6f6e 652c 0a20 2020 2029 3a0a  ts=None,.    ):.
-0001b7a0: 2020 2020 2020 2020 2222 2269 6e69 7469          """initi
-0001b7b0: 616c 697a 6520 6669 7420 6f62 6a65 6374  alize fit object
-0001b7c0: 2066 6f72 2073 696d 706c 6520 6d69 6e75   for simple minu
-0001b7d0: 6974 2066 6974 2077 6974 680a 2020 2020  it fit with.    
-0001b7e0: 2020 2020 2a20 7769 7468 2075 7365 722d      * with user-
-0001b7f0: 7375 7070 6c69 6564 2063 6f73 7420 6675  supplied cost fu
-0001b800: 6e63 7469 6f6e 206f 720a 2020 2020 2020  nction or.      
-0001b810: 2020 2a20 6120 7072 6f62 6162 696c 6974    * a probabilit
-0001b820: 7920 6465 6e73 6974 7920 6675 6e63 7469  y density functi
-0001b830: 6f6e 2066 6f72 2061 6e20 756e 6269 6e6e  on for an unbinn
-0001b840: 6564 206e 6567 2e20 6c6f 672d 4c20 6669  ed neg. log-L fi
-0001b850: 740a 0a20 2020 2020 2020 2041 7267 733a  t..        Args:
-0001b860: 0a20 2020 2020 2020 2020 202d 2063 6f73  .          - cos
-0001b870: 7446 756e 6374 696f 6e3a 2063 6f73 7420  tFunction: cost 
-0001b880: 6675 6e63 7469 6f6e 206f 7220 7064 660a  function or pdf.
-0001b890: 2020 2020 2020 2020 2020 2d20 7030 3a20            - p0: 
-0001b8a0: 6e70 2d61 7272 6179 206f 6620 666c 6f61  np-array of floa
-0001b8b0: 7473 2c20 696e 6974 6961 6c20 7061 7261  ts, initial para
-0001b8c0: 6d65 7465 7220 7661 6c75 6573 0a20 2020  meter values.   
-0001b8d0: 2020 2020 2020 202d 206d 6f64 656c 5f6b         - model_k
-0001b8e0: 7761 7267 733a 206f 7074 696f 6e61 6c2c  wargs: optional,
-0001b8f0: 2066 6974 2070 6172 616d 6574 6572 7320   fit parameters 
-0001b900: 6966 206e 6f74 2066 726f 6d20 6d6f 6465  if not from mode
-0001b910: 6c20 7369 676e 6174 7572 650a 2020 2020  l signature.    
-0001b920: 2020 2020 2020 2d20 6470 303a 2061 7272        - dp0: arr
-0001b930: 6179 2d6c 696b 652c 2069 6e69 7469 616c  ay-like, initial
-0001b940: 2067 7565 7373 206f 6620 7061 7261 6d65   guess of parame
-0001b950: 7465 7220 756e 6365 7274 6169 6e74 6965  ter uncertaintie
-0001b960: 7320 286f 7074 696f 6e61 6c29 0a20 2020  s (optional).   
-0001b970: 2020 2020 2020 202d 2070 6172 616d 6574         - paramet
-0001b980: 6572 2063 6f6e 7374 7261 696e 7473 3a20  er constraints: 
-0001b990: 286e 6573 7465 6429 206c 6973 7428 7329  (nested) list(s)
-0001b9a0: 3a20 5b70 6172 616d 6574 6572 206e 616d  : [parameter nam
-0001b9b0: 652c 2076 616c 7565 2c20 756e 6365 7274  e, value, uncert
-0001b9c0: 6169 6e74 795d 0a20 2020 2020 2020 2020  ainty].         
-0001b9d0: 202d 2066 6978 2070 6172 616d 6574 6572   - fix parameter
-0001b9e0: 2873 2920 696e 2066 6974 3a20 6c69 7374  (s) in fit: list
-0001b9f0: 206f 6620 7061 7261 6d65 7465 7220 6e61   of parameter na
-0001ba00: 6d65 7320 6f72 2069 6e64 6963 6573 0a20  mes or indices. 
-0001ba10: 2020 2020 2020 2020 202d 206c 696d 6974           - limit
-0001ba20: 733a 2028 6e65 7374 6564 2920 6c69 7374  s: (nested) list
-0001ba30: 2873 293a 205b 7061 7261 6d65 7465 7220  (s): [parameter 
-0001ba40: 6e61 6d65 2c20 6d69 6e2c 206d 6178 5d20  name, min, max] 
-0001ba50: 6f72 0a20 2020 2020 2020 2020 2020 205b  or.            [
-0001ba60: 7061 7261 6d65 7465 7220 696e 6465 782c  parameter index,
-0001ba70: 206d 696e 2c20 6d61 785d 0a20 2020 2020   min, max].     
-0001ba80: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0001ba90: 6620 7365 6c66 2e64 6174 6120 6973 204e  f self.data is N
-0001baa0: 6f6e 6520 616e 6420 7365 6c66 2e66 6974  one and self.fit
-0001bab0: 5f74 7970 6520 213d 2022 7573 6572 223a  _type != "user":
-0001bac0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001bad0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
-0001bae0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001baf0: 2021 2121 206d 6e46 6974 2e69 6e69 745f   !!! mnFit.init_
-0001bb00: 6d6e 4669 743a 206e 6f20 6461 7461 206f  mnFit: no data o
-0001bb10: 626a 6563 7420 6465 6669 6e65 6420 2d20  bject defined - 
-0001bb20: 6361 6c6c 2069 6e69 745f 6461 7461 2829  call init_data()
-0001bb30: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-0001bb40: 0a20 2020 2020 2020 2023 2067 6574 2070  .        # get p
-0001bb50: 6172 616d 6574 6572 7320 6f66 206d 6f64  arameters of mod
-0001bb60: 656c 2066 756e 6374 696f 6e20 746f 2073  el function to s
-0001bb70: 6574 2073 7461 7274 2076 616c 7565 7320  et start values 
-0001bb80: 666f 7220 6669 740a 2020 2020 2020 2020  for fit.        
-0001bb90: 6966 206d 6f64 656c 5f6b 7761 7267 7320  if model_kwargs 
-0001bba0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0001bbb0: 2020 2020 2061 7267 732c 206d 6f64 656c       args, model
-0001bbc0: 5f6b 7761 7267 7320 3d20 6765 745f 6675  _kwargs = get_fu
-0001bbd0: 6e63 7469 6f6e 5369 676e 6174 7572 6528  nctionSignature(
-0001bbe0: 7573 6572 4675 6e63 7469 6f6e 290a 0a20  userFunction).. 
-0001bbf0: 2020 2020 2020 2070 6172 203d 2028 6d6f         par = (mo
-0001bc00: 6465 6c5f 6b77 6172 6773 2c20 7030 2c20  del_kwargs, p0, 
-0001bc10: 6470 302c 2063 6f6e 7374 7261 696e 7473  dp0, constraints
-0001bc20: 2c20 6669 7850 6172 732c 206c 696d 6974  , fixPars, limit
-0001bc30: 7329 0a20 2020 2020 2020 2073 656c 662e  s).        self.
-0001bc40: 5f73 6574 7570 4669 7450 6172 616d 6574  _setupFitParamet
-0001bc50: 6572 7328 2a70 6172 290a 0a20 2020 2020  ers(*par)..     
-0001bc60: 2020 2023 2073 6574 2075 7020 636f 7374     # set up cost
-0001bc70: 2066 756e 6374 696f 6e20 666f 7220 696d   function for im
-0001bc80: 696e 7569 740a 2020 2020 2020 2020 7365  inuit.        se
-0001bc90: 6c66 2e63 6f73 7466 203d 2073 656c 662e  lf.costf = self.
-0001bca0: 6d6e 436f 7374 2873 656c 662c 2075 7365  mnCost(self, use
-0001bcb0: 7246 756e 6374 696f 6e29 0a20 2020 2020  rFunction).     
-0001bcc0: 2020 2073 656c 662e 5f73 6574 7570 4d69     self._setupMi
-0001bcd0: 6e75 6974 286d 6f64 656c 5f6b 7761 7267  nuit(model_kwarg
-0001bce0: 7329 0a0a 2020 2020 6465 6620 7365 745f  s)..    def set_
-0001bcf0: 6d6e 4f70 7469 6f6e 7328 7365 6c66 2c20  mnOptions(self, 
-0001bd00: 7275 6e5f 6d69 6e6f 733d 4e6f 6e65 2c20  run_minos=None, 
-0001bd10: 6e65 6732 6c6f 674c 3d4e 6f6e 652c 2071  neg2logL=None, q
-0001bd20: 7569 6574 3d4e 6f6e 6529 3a0a 2020 2020  uiet=None):.    
-0001bd30: 2020 2020 2222 2244 6566 696e 6520 6f70      """Define op
-0001bd40: 7469 6f6e 7320 666f 7220 6d69 6e75 6974  tions for minuit
-0001bd50: 2066 6974 2077 6974 6820 7573 6572 2063   fit with user c
-0001bd60: 6f73 7420 6675 6e63 7469 6f6e 0a0a 2020  ost function..  
-0001bd70: 2020 2020 2020 4172 6773 3a0a 0a20 2020        Args:..   
-0001bd80: 2020 2020 202d 2072 756e 5f6d 696e 6f73       - run_minos
-0001bd90: 3a20 7275 6e20 6d69 6e6f 7320 7072 6f66  : run minos prof
-0001bda0: 696c 6520 6c69 6b65 6c69 686f 6f64 2073  ile likelihood s
-0001bdb0: 6361 6e0a 2020 2020 2020 2020 2d20 6e65  can.        - ne
-0001bdc0: 6732 6c6f 674c 3a20 636f 7374 2066 756e  g2logL: cost fun
-0001bdd0: 6374 696f 6e20 6973 202d 3220 6e65 674c  ction is -2 negL
-0001bde0: 6f67 4c0a 2020 2020 2020 2020 2222 220a  ogL.        """.
-0001bdf0: 2020 2020 2020 2020 6966 2072 756e 5f6d          if run_m
-0001be00: 696e 6f73 2069 7320 6e6f 7420 4e6f 6e65  inos is not None
-0001be10: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001be20: 6c66 2e72 756e 5f6d 696e 6f73 203d 2072  lf.run_minos = r
-0001be30: 756e 5f6d 696e 6f73 0a20 2020 2020 2020  un_minos.       
-0001be40: 2020 2020 2073 656c 662e 6f70 7469 6f6e       self.option
-0001be50: 735b 2272 756e 5f6d 696e 6f73 225d 5b30  s["run_minos"][0
-0001be60: 5d20 3d20 696e 7428 7275 6e5f 6d69 6e6f  ] = int(run_mino
-0001be70: 7329 0a20 2020 2020 2020 2069 6620 6e65  s).        if ne
-0001be80: 6732 6c6f 674c 2069 7320 6e6f 7420 4e6f  g2logL is not No
-0001be90: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0001bea0: 7365 6c66 2e6e 6567 326c 6f67 4c20 3d20  self.neg2logL = 
-0001beb0: 6e65 6732 6c6f 674c 0a20 2020 2020 2020  neg2logL.       
-0001bec0: 2020 2020 2073 656c 662e 6f70 7469 6f6e       self.option
-0001bed0: 735b 226e 6567 326c 6f67 4c22 5d5b 305d  s["neg2logL"][0]
-0001bee0: 203d 2069 6e74 286e 6567 326c 6f67 4c29   = int(neg2logL)
-0001bef0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001bf00: 7365 6c66 2e6e 6567 326c 6f67 4c3a 0a20  self.neg2logL:. 
-0001bf10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001bf20: 656c 662e 4572 7244 6566 203d 2031 2e30  elf.ErrDef = 1.0
-0001bf30: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001bf40: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001bf50: 2020 2073 656c 662e 4572 7244 6566 203d     self.ErrDef =
-0001bf60: 2030 2e35 0a20 2020 2020 2020 2069 6620   0.5.        if 
-0001bf70: 7175 6965 7420 6973 206e 6f74 204e 6f6e  quiet is not Non
-0001bf80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0001bf90: 656c 662e 7175 6965 7420 3d20 7175 6965  elf.quiet = quie
-0001bfa0: 740a 0a20 2020 2063 6c61 7373 206d 6c44  t..    class mlD
-0001bfb0: 6174 6143 6f6e 7461 696e 6572 3a0a 2020  ataContainer:.  
-0001bfc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001bfd0: 2020 436f 6e74 6169 6e65 7220 666f 7220    Container for 
-0001bfe0: 6765 6e65 7261 6c20 2869 6e64 6578 6564  general (indexed
-0001bff0: 2920 6461 7461 0a0a 2020 2020 2020 2020  ) data..        
-0001c000: 4461 7461 204d 656d 6265 7273 3a0a 0a20  Data Members:.. 
-0001c010: 2020 2020 2020 202d 2078 2c20 6172 7261         - x, arra
-0001c020: 7920 6f66 2066 6c6f 6174 733a 2064 6174  y of floats: dat
-0001c030: 610a 0a0a 2020 2020 2020 2020 4d65 7468  a...        Meth
-0001c040: 6f64 733a 0a0a 2020 2020 2020 2020 2d70  ods:..        -p
-0001c050: 6c6f 7428 293a 2072 6574 7572 6e20 6669  lot(): return fi
-0001c060: 6775 7265 2077 6974 6820 7265 7072 6573  gure with repres
-0001c070: 656e 7461 7469 6f6e 206f 6620 6461 7461  entation of data
-0001c080: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-0001c090: 2020 2020 2020 6465 6620 5f5f 696e 6974        def __init
-0001c0a0: 5f5f 2873 656c 662c 206f 7574 6572 2c20  __(self, outer, 
-0001c0b0: 7829 3a0a 2020 2020 2020 2020 2020 2020  x):.            
-0001c0c0: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
-0001c0d0: 7374 6f72 6520 6461 7461 0a0a 2020 2020  store data..    
-0001c0e0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0001c0f0: 2020 2020 2020 2020 2020 2d20 782c 2061            - x, a
-0001c100: 7272 6179 206f 6620 666c 6f61 7473 0a20  rray of floats. 
-0001c110: 2020 2020 2020 2020 2020 202d 2071 7569             - qui
-0001c120: 6574 3a20 626f 6f6c 6561 6e2c 2063 6f6e  et: boolean, con
-0001c130: 7472 6f6c 7320 7072 696e 7465 6420 6f75  trols printed ou
-0001c140: 7470 7574 0a0a 2020 2020 2020 2020 2020  tput..          
-0001c150: 2020 2222 220a 0a20 2020 2020 2020 2020    """..         
-0001c160: 2020 2073 656c 662e 7820 3d20 6e70 2e61     self.x = np.a
-0001c170: 7361 7272 6179 2878 290a 2020 2020 2020  sarray(x).      
-0001c180: 2020 2020 2020 7365 6c66 2e64 6c65 6e67        self.dleng
-0001c190: 7468 203d 206c 656e 2873 656c 662e 7829  th = len(self.x)
-0001c1a0: 0a0a 2020 2020 2020 2020 6465 6620 706c  ..        def pl
-0001c1b0: 6f74 280a 2020 2020 2020 2020 2020 2020  ot(.            
-0001c1c0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0001c1d0: 2020 6e75 6d3d 2269 6e64 6578 6564 2064    num="indexed d
-0001c1e0: 6174 6122 2c0a 2020 2020 2020 2020 2020  ata",.          
-0001c1f0: 2020 6669 6773 697a 653d 2837 2e35 2c20    figsize=(7.5, 
-0001c200: 362e 3529 2c0a 2020 2020 2020 2020 2020  6.5),.          
-0001c210: 2020 6461 7461 5f6c 6162 656c 3d22 4461    data_label="Da
-0001c220: 7461 222c 0a20 2020 2020 2020 2020 2020  ta",.           
-0001c230: 2070 6c6f 745f 7265 7369 6475 616c 3d46   plot_residual=F
-0001c240: 616c 7365 2c0a 2020 2020 2020 2020 293a  alse,.        ):
-0001c250: 0a20 2020 2020 2020 2020 2020 2022 2222  .            """
-0001c260: 7265 7475 726e 2066 6967 7572 6520 7769  return figure wi
-0001c270: 7468 2068 6973 746f 6772 616d 2064 6174  th histogram dat
-0001c280: 6120 616e 6420 756e 6365 7274 6169 6e74  a and uncertaint
-0001c290: 6965 7322 2222 0a0a 2020 2020 2020 2020  ies"""..        
-0001c2a0: 2020 2020 6669 6720 3d20 706c 742e 6669      fig = plt.fi
-0001c2b0: 6775 7265 286e 756d 3d6e 756d 2c20 6669  gure(num=num, fi
-0001c2c0: 6773 697a 653d 6669 6773 697a 6529 0a0a  gsize=figsize)..
-0001c2d0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-0001c2e0: 6c6f 745f 7265 7369 6475 616c 3a0a 2020  lot_residual:.  
-0001c2f0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0001c300: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
-0001c310: 2020 2020 2020 2020 2022 2021 2121 206d           " !!! m
-0001c320: 6e46 6974 2e6d 6c44 6174 612e 706c 6f74  nFit.mlData.plot
-0001c330: 3a20 706c 6f74 7469 6e67 2072 6573 6964  : plotting resid
-0001c340: 7561 6c73 206e 6f74 2070 6f73 7369 626c  uals not possibl
-0001c350: 6520 666f 7220 7573 6572 204d 4c20 6669  e for user ML fi
-0001c360: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
-0001c370: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0001c380: 2020 6966 2073 656c 662e 7820 6973 204e    if self.x is N
-0001c390: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001c3a0: 2020 2020 2070 7269 6e74 2822 2021 2121       print(" !!!
-0001c3b0: 206d 6e46 6974 2e6d 6c44 6174 612e 706c   mnFit.mlData.pl
-0001c3c0: 6f74 3a20 6e6f 2064 6174 6120 6f62 6a65  ot: no data obje
-0001c3d0: 6374 2064 6566 696e 6564 2229 0a20 2020  ct defined").   
-0001c3e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001c3f0: 7572 6e20 6669 670a 0a20 2020 2020 2020  urn fig..       
-0001c400: 2020 2020 206d 6e20 3d20 6d69 6e28 7365       mn = min(se
-0001c410: 6c66 2e78 290a 2020 2020 2020 2020 2020  lf.x).          
-0001c420: 2020 6d78 203d 206d 6178 2873 656c 662e    mx = max(self.
-0001c430: 7829 0a20 2020 2020 2020 2020 2020 2079  x).            y
-0001c440: 6d6e 203d 2030 2e30 0a20 2020 2020 2020  mn = 0.0.       
-0001c450: 2020 2020 2079 6d78 203d 2030 2e32 3520       ymx = 0.25 
-0001c460: 2f20 286d 7820 2d20 6d6e 290a 2020 2020  / (mx - mn).    
-0001c470: 2020 2020 2020 2020 706c 742e 766c 696e          plt.vlin
-0001c480: 6573 280a 2020 2020 2020 2020 2020 2020  es(.            
-0001c490: 2020 2020 7365 6c66 2e78 2c20 796d 6e2c      self.x, ymn,
-0001c4a0: 2079 6d78 2c20 6c77 3d31 2c20 636f 6c6f   ymx, lw=1, colo
-0001c4b0: 723d 2267 7265 7922 2c20 616c 7068 613d  r="grey", alpha=
-0001c4c0: 302e 352c 206c 6162 656c 3d64 6174 615f  0.5, label=data_
-0001c4d0: 6c61 6265 6c0a 2020 2020 2020 2020 2020  label.          
-0001c4e0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-0001c4f0: 2072 6574 7572 6e20 6669 670a 0a20 2020   return fig..   
-0001c500: 2023 202d 2d2d 2063 6c61 7373 2065 6e63   # --- class enc
-0001c510: 6170 7375 6c61 7469 6e67 2075 7365 722d  apsulating user-
-0001c520: 6465 6669 6e65 6420 636f 7374 2066 756e  defined cost fun
-0001c530: 6374 696f 6e0a 2020 2020 636c 6173 7320  ction.    class 
-0001c540: 6d6e 436f 7374 3a0a 2020 2020 2020 2020  mnCost:.        
-0001c550: 2222 220a 2020 2020 2020 2020 496e 7465  """.        Inte
-0001c560: 7266 6163 6520 666f 7220 7369 6d70 6c65  rface for simple
-0001c570: 206d 696e 7569 7420 6669 7420 7769 7468   minuit fit with
-0001c580: 2075 7365 722d 7375 7070 6c69 6564 2063   user-supplied c
-0001c590: 6f73 7420 6675 6e63 7469 6f6e 2e0a 0a20  ost function... 
-0001c5a0: 2020 2020 2020 2054 6865 205f 5f63 616c         The __cal
-0001c5b0: 6c5f 5f20 6d65 7468 6f64 206f 6620 7468  l__ method of th
-0001c5c0: 6973 2063 6c61 7373 2069 7320 6361 6c6c  is class is call
-0001c5d0: 6564 2062 7920 696d 696e 7569 742e 0a0a  ed by iminuit...
-0001c5e0: 2020 2020 2020 2020 4172 6773 3a0a 0a20          Args:.. 
-0001c5f0: 2020 2020 2020 2020 202d 2075 7365 7243           - userC
-0001c600: 6f73 7446 756e 6374 696f 6e3a 2075 7365  ostFunction: use
-0001c610: 722d 7375 7070 6c69 6564 2063 6f73 7420  r-supplied cost 
-0001c620: 6675 6e63 7469 6f6e 2066 6f72 206d 696e  function for min
-0001c630: 7569 743b 0a20 2020 2020 2020 2020 2020  uit;.           
-0001c640: 2020 6d75 7374 2062 6520 6120 6e65 6761    must be a nega
-0001c650: 7469 7665 206c 6f67 2d6c 696b 656c 6968  tive log-likelih
-0001c660: 6f6f 640a 2020 2020 2020 2020 2222 220a  ood.        """.
-0001c670: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
-0001c680: 6e69 745f 5f28 7365 6c66 2c20 6f75 7465  nit__(self, oute
-0001c690: 722c 2075 7365 7246 756e 6374 696f 6e29  r, userFunction)
-0001c6a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001c6b0: 6c66 2e71 7569 6574 203d 206f 7574 6572  lf.quiet = outer
-0001c6c0: 2e71 7569 6574 0a20 2020 2020 2020 2020  .quiet.         
-0001c6d0: 2020 2073 656c 662e 6461 7461 203d 206f     self.data = o
-0001c6e0: 7574 6572 2e64 6174 610a 2020 2020 2020  uter.data.      
-0001c6f0: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
-0001c700: 7461 2069 7320 4e6f 6e65 3a0a 2020 2020  ta is None:.    
-0001c710: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001c720: 2e63 6f73 7420 3d20 7573 6572 4675 6e63  .cost = userFunc
-0001c730: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0001c740: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-0001c750: 2e71 7569 6574 3a0a 2020 2020 2020 2020  .quiet:.        
-0001c760: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0001c770: 7428 222a 3d3d 2a20 6d6e 4669 742e 6d6e  t("*==* mnFit.mn
-0001c780: 436f 7374 3a20 6669 7420 7769 7468 2075  Cost: fit with u
-0001c790: 7365 722d 7375 7070 6c69 6564 2063 6f73  ser-supplied cos
-0001c7a0: 7420 6675 6e63 7469 6f6e 2722 290a 2020  t function'").  
-0001c7b0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0001c7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c7d0: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-0001c7e0: 6528 7365 6c66 2e64 6174 612c 206d 6e46  e(self.data, mnF
-0001c7f0: 6974 2e6d 6c44 6174 6143 6f6e 7461 696e  it.mlDataContain
-0001c800: 6572 293a 0a20 2020 2020 2020 2020 2020  er):.           
-0001c810: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0001c820: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-0001c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c840: 2020 2022 2021 2121 206d 6e46 6974 2e6d     " !!! mnFit.m
-0001c850: 6e43 6f73 743a 2065 7870 6563 7469 6e67  nCost: expecting
-0001c860: 2064 6174 6120 636f 6e74 6169 6e65 7220   data container 
-0001c870: 6f66 2074 7970 6520 276d 6c44 6174 6143  of type 'mlDataC
-0001c880: 6f6e 7461 696e 6572 2722 0a20 2020 2020  ontainer'".     
-0001c890: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001c8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c8b0: 2073 656c 662e 6d6f 6465 6c20 3d20 7573   self.model = us
-0001c8c0: 6572 4675 6e63 7469 6f6e 0a20 2020 2020  erFunction.     
-0001c8d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c8e0: 636f 7374 203d 2073 656c 662e 6e6c 4c63  cost = self.nlLc
-0001c8f0: 6f73 740a 2020 2020 2020 2020 2020 2020  ost.            
-0001c900: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0001c910: 7175 6965 743a 0a20 2020 2020 2020 2020  quiet:.         
-0001c920: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0001c930: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001c940: 2020 2020 2020 2020 2020 222a 3d3d 2a20            "*==* 
-0001c950: 6d6e 4669 742e 6d6e 436f 7374 3a20 6e65  mnFit.mnCost: ne
-0001c960: 674c 6f67 4c20 6669 7420 7769 7468 2075  gLogL fit with u
-0001c970: 7365 722d 6465 6669 6e65 6420 6465 6e73  ser-defined dens
-0001c980: 6974 7920 6675 6e63 7469 6f6e 2722 0a20  ity function'". 
-0001c990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9a0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0001c9b0: 2020 2320 7461 6b65 2061 6363 6f75 6e74    # take account
-0001c9c0: 206f 6620 706f 7373 6962 6c65 2070 6172   of possible par
-0001c9d0: 616d 6574 6572 2063 6f6e 7374 7261 696e  ameter constrain
-0001c9e0: 7473 0a20 2020 2020 2020 2020 2020 2073  ts.            s
-0001c9f0: 656c 662e 636f 6e73 7472 6169 6e74 7320  elf.constraints 
-0001ca00: 3d20 6f75 7465 722e 636f 6e73 7472 6169  = outer.constrai
-0001ca10: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
-0001ca20: 7365 6c66 2e6e 636f 6e73 7472 6169 6e74  self.nconstraint
-0001ca30: 7320 3d20 6c65 6e28 7365 6c66 2e63 6f6e  s = len(self.con
-0001ca40: 7374 7261 696e 7473 290a 2020 2020 2020  straints).      
-0001ca50: 2020 2020 2020 7365 6c66 2e45 7272 4465        self.ErrDe
-0001ca60: 6620 3d20 6f75 7465 722e 4572 7244 6566  f = outer.ErrDef
-0001ca70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001ca80: 662e 7366 5f6c 4c20 3d20 2d32 2e30 202a  f.sf_lL = -2.0 *
-0001ca90: 2073 656c 662e 4572 7244 6566 0a0a 2020   self.ErrDef..  
-0001caa0: 2020 2020 2020 2020 2020 2320 7365 7420            # set 
-0001cab0: 7072 6f70 6572 2073 6967 6e61 7475 7265  proper signature
-0001cac0: 206f 6620 6d6f 6465 6c20 6675 6e63 7469   of model functi
-0001cad0: 6f6e 2066 6f72 2069 6d69 6e75 6974 0a20  on for iminuit. 
-0001cae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001caf0: 706e 616d 7320 3d20 6f75 7465 722e 706e  pnams = outer.pn
-0001cb00: 616d 730a 2020 2020 2020 2020 2020 2020  ams.            
-0001cb10: 7365 6c66 2e6e 7061 7220 3d20 6f75 7465  self.npar = oute
-0001cb20: 722e 6e70 6172 0a0a 2020 2020 2020 2020  r.npar..        
-0001cb30: 2020 2020 2320 666f 7220 7468 6973 206b      # for this k
-0001cb40: 696e 6420 6f66 2066 6974 2c20 736f 6d65  ind of fit, some
-0001cb50: 2069 6e70 7574 2061 6e64 206f 7570 7574   input and ouput
-0001cb60: 2071 7561 6e74 6974 6965 7320 6172 6520   quantities are 
-0001cb70: 6e6f 7420 6b6e 6f77 6e0a 2020 2020 2020  not known.      
-0001cb80: 2020 2020 2020 7365 6c66 2e67 6f66 203d        self.gof =
-0001cb90: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-0001cba0: 2020 7365 6c66 2e6e 646f 6620 3d20 4e6f    self.ndof = No
-0001cbb0: 6e65 0a0a 2020 2020 2020 2020 6465 6620  ne..        def 
-0001cbc0: 5f5f 6361 6c6c 5f5f 2873 656c 662c 202a  __call__(self, *
-0001cbd0: 7061 7229 3a0a 2020 2020 2020 2020 2020  par):.          
-0001cbe0: 2020 636f 7374 203d 2030 2e30 0a20 2020    cost = 0.0.   
-0001cbf0: 2020 2020 2020 2020 2023 2061 6464 2063           # add c
-0001cc00: 6f6e 7374 7261 696e 7473 2074 6f20 636f  onstraints to co
-0001cc10: 7374 0a20 2020 2020 2020 2020 2020 2069  st.            i
-0001cc20: 6620 7365 6c66 2e6e 636f 6e73 7472 6169  f self.nconstrai
-0001cc30: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
-0001cc40: 2020 2020 2066 6f72 2063 2069 6e20 7365       for c in se
-0001cc50: 6c66 2e63 6f6e 7374 7261 696e 7473 3a0a  lf.constraints:.
-0001cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc70: 2020 2020 705f 6964 203d 2063 5b30 5d0a      p_id = c[0].
-0001cc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc90: 2020 2020 7220 3d20 2870 6172 5b70 5f69      r = (par[p_i
-0001cca0: 645d 202d 2063 5b31 5d29 202f 2063 5b32  d] - c[1]) / c[2
-0001ccb0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001ccc0: 2020 2020 2020 636f 7374 202b 3d20 7220        cost += r 
-0001ccd0: 2a20 720a 2020 2020 2020 2020 2020 2020  * r.            
-0001cce0: 2020 2020 636f 7374 202a 3d20 7365 6c66      cost *= self
-0001ccf0: 2e45 7272 4465 660a 2020 2020 2020 2020  .ErrDef.        
-0001cd00: 2020 2020 2320 6361 6c6c 6564 2069 7465      # called ite
-0001cd10: 7261 7469 7665 6c79 2062 7920 6d69 6e75  ratively by minu
-0001cd20: 6974 0a20 2020 2020 2020 2020 2020 2072  it.            r
-0001cd30: 6574 7572 6e20 636f 7374 202b 2073 656c  eturn cost + sel
-0001cd40: 662e 636f 7374 282a 7061 7229 0a0a 2020  f.cost(*par)..  
-0001cd50: 2020 2020 2020 6465 6620 6e6c 4c63 6f73        def nlLcos
-0001cd60: 7428 7365 6c66 2c20 2a70 6172 293a 0a20  t(self, *par):. 
-0001cd70: 2020 2020 2020 2020 2020 2022 2222 6e65             """ne
-0001cd80: 6761 7469 7665 206c 6f67 206c 696b 656c  gative log likel
-0001cd90: 6968 6f6f 6420 6f66 2064 6174 6120 616e  ihood of data an
-0001cda0: 6420 7573 6572 2d64 6566 696e 6564 2050  d user-defined P
-0001cdb0: 4446 2061 6e64 2222 220a 2020 2020 2020  DF and""".      
-0001cdc0: 2020 2020 2020 2320 6368 6563 6b20 6966        # check if
-0001cdd0: 2050 4446 2069 7320 6e6f 6d61 6c69 7a65   PDF is nomalize
-0001cde0: 6420 746f 2031 0a20 2020 2020 2020 2020  d to 1.         
-0001cdf0: 2020 2023 202e 2e2e 0a0a 2020 2020 2020     # .....      
-0001ce00: 2020 2020 2020 6c4c 203d 206e 702e 7375        lL = np.su
-0001ce10: 6d28 6e70 2e6c 6f67 2873 656c 662e 6d6f  m(np.log(self.mo
-0001ce20: 6465 6c28 7365 6c66 2e64 6174 612e 782c  del(self.data.x,
-0001ce30: 202a 7061 7229 2929 0a20 2020 2020 2020   *par))).       
-0001ce40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001ce50: 2e73 665f 6c4c 202a 206c 4c0a 0a20 2020  .sf_lL * lL..   
-0001ce60: 2023 202d 2d2d 2065 6e64 2064 6566 696e   # --- end defin
-0001ce70: 6974 696f 6e20 6f66 2063 6c61 7373 206d  ition of class m
-0001ce80: 6e43 6f73 7420 2d2d 2d2d 0a0a 2020 2020  nCost ----..    
-0001ce90: 230a 2020 2020 2320 2d2d 2d20 636f 6d6d  #.    # --- comm
-0001cea0: 6f6e 2063 6f64 6520 666f 7220 616c 6c20  on code for all 
-0001ceb0: 6669 7420 7479 7065 730a 2020 2020 230a  fit types.    #.
-0001cec0: 0a20 2020 2064 6566 205f 7365 7475 7046  .    def _setupF
-0001ced0: 6974 5061 7261 6d65 7465 7273 2873 656c  itParameters(sel
-0001cee0: 662c 206d 6f64 656c 5f6b 7761 7267 732c  f, model_kwargs,
-0001cef0: 2070 302c 2064 7030 2c20 636f 6e73 7472   p0, dp0, constr
-0001cf00: 6169 6e74 732c 2066 6978 5061 7273 2c20  aints, fixPars, 
-0001cf10: 6c69 6d69 7473 293a 0a20 2020 2020 2020  limits):.       
-0001cf20: 2022 2222 7365 7420 7570 2070 6172 616d   """set up param
-0001cf30: 6574 6572 7320 6e65 6564 6564 2066 6f72  eters needed for
-0001cf40: 204d 696e 7569 7420 616e 6420 636f 7374   Minuit and cost
-0001cf50: 2066 756e 6374 696f 6e22 2222 0a0a 2020   function"""..  
-0001cf60: 2020 2020 2020 2320 6765 7420 7061 7261        # get para
-0001cf70: 6d65 7465 7220 6e61 6d65 7320 6672 6f6d  meter names from
-0001cf80: 206b 7761 7267 7320 6f66 206d 6f64 656c   kwargs of model
-0001cf90: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
-0001cfa0: 2020 7365 6c66 2e70 6e61 6d73 203d 206c    self.pnams = l
-0001cfb0: 6973 742e 636f 7079 286c 6973 7428 6d6f  ist.copy(list(mo
-0001cfc0: 6465 6c5f 6b77 6172 6773 2e6b 6579 7328  del_kwargs.keys(
-0001cfd0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-0001cfe0: 2e6e 7061 7220 3d20 6c65 6e28 7365 6c66  .npar = len(self
-0001cff0: 2e70 6e61 6d73 290a 2020 2020 2020 2020  .pnams).        
-0001d000: 2320 6469 6374 696f 6e61 7279 2061 7373  # dictionary ass
-0001d010: 6967 6e69 6e67 2070 6172 616d 6574 6572  igning parameter
-0001d020: 206e 616d 6520 746f 2069 6e64 6578 0a20   name to index. 
-0001d030: 2020 2020 2020 2073 656c 662e 706e 616d         self.pnam
-0001d040: 3269 6420 3d20 7b73 656c 662e 706e 616d  2id = {self.pnam
-0001d050: 735b 695d 3a20 6920 666f 7220 6920 696e  s[i]: i for i in
-0001d060: 2072 616e 6765 2830 2c20 7365 6c66 2e6e   range(0, self.n
-0001d070: 7061 7229 7d0a 0a20 2020 2020 2020 2023  par)}..        #
-0001d080: 2070 726f 6365 7373 2061 6e64 2073 746f   process and sto
-0001d090: 7265 2070 6172 616d 6574 6572 2063 6f6e  re parameter con
-0001d0a0: 7374 7261 696e 7473 2028 7573 6564 2069  straints (used i
-0001d0b0: 6e20 636f 7374 2066 756e 6374 696f 6e29  n cost function)
-0001d0c0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-0001d0d0: 7443 6f6e 7374 7261 696e 7473 203d 2063  tConstraints = c
-0001d0e0: 6f6e 7374 7261 696e 7473 0a20 2020 2020  onstraints.     
-0001d0f0: 2020 2073 656c 662e 636f 6e73 7472 6169     self.constrai
-0001d100: 6e74 7320 3d20 5b5d 0a20 2020 2020 2020  nts = [].       
-0001d110: 2069 6620 636f 6e73 7472 6169 6e74 7320   if constraints 
-0001d120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0001d130: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0001d140: 6e70 2e73 6861 7065 2863 6f6e 7374 7261  np.shape(constra
-0001d150: 696e 7473 2929 203d 3d20 323a 0a20 2020  ints)) == 2:.   
-0001d160: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0001d170: 2063 2069 6e20 636f 6e73 7472 6169 6e74   c in constraint
-0001d180: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0001d190: 2020 2020 2020 2023 206e 616d 6520 746f         # name to
-0001d1a0: 2070 6172 616d 6574 6572 2069 640a 2020   parameter id.  
-0001d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1c0: 2020 6966 2074 7970 6528 635b 305d 2920    if type(c[0]) 
-0001d1d0: 3d3d 2074 7970 6528 2220 2229 3a0a 2020  == type(" "):.  
-0001d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1f0: 2020 2020 2020 635b 305d 203d 2073 656c        c[0] = sel
-0001d200: 662e 706e 616d 3269 645b 635b 305d 5d0a  f.pnam2id[c[0]].
-0001d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d220: 2020 2020 7365 6c66 2e63 6f6e 7374 7261      self.constra
-0001d230: 696e 7473 2e61 7070 656e 6428 6329 0a20  ints.append(c). 
-0001d240: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001d250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d260: 2023 206e 616d 6520 746f 2070 6172 616d   # name to param
-0001d270: 6574 6572 2069 640a 2020 2020 2020 2020  eter id.        
-0001d280: 2020 2020 2020 2020 6966 2074 7970 6528          if type(
-0001d290: 636f 6e73 7472 6169 6e74 735b 305d 2920  constraints[0]) 
-0001d2a0: 3d3d 2074 7970 6528 2220 2229 3a0a 2020  == type(" "):.  
-0001d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d2c0: 2020 636f 6e73 7472 6169 6e74 735b 305d    constraints[0]
-0001d2d0: 203d 2073 656c 662e 706e 616d 3269 645b   = self.pnam2id[
-0001d2e0: 636f 6e73 7472 6169 6e74 735b 305d 5d0a  constraints[0]].
-0001d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d300: 7365 6c66 2e63 6f6e 7374 7261 696e 7473  self.constraints
-0001d310: 2e61 7070 656e 6428 636f 6e73 7472 6169  .append(constrai
-0001d320: 6e74 7329 0a20 2020 2020 2020 2073 656c  nts).        sel
-0001d330: 662e 6e63 6f6e 7374 7261 696e 7473 203d  f.nconstraints =
-0001d340: 206c 656e 2873 656c 662e 636f 6e73 7472   len(self.constr
-0001d350: 6169 6e74 7329 0a0a 2020 2020 2020 2020  aints)..        
-0001d360: 2320 7365 7420 696e 6974 6961 6c20 7061  # set initial pa
-0001d370: 7261 6d65 7465 7273 2066 6f72 2066 6974  rameters for fit
-0001d380: 2028 7573 6564 2062 7920 6d69 6e75 6974   (used by minuit
-0001d390: 290a 2020 2020 2020 2020 6966 2070 3020  ).        if p0 
-0001d3a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0001d3b0: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
-0001d3c0: 706e 616d 2069 6e20 656e 756d 6572 6174  pnam in enumerat
-0001d3d0: 6528 7365 6c66 2e70 6e61 6d73 293a 0a20  e(self.pnams):. 
-0001d3e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001d3f0: 6f64 656c 5f6b 7761 7267 735b 706e 616d  odel_kwargs[pnam
-0001d400: 5d20 3d20 7030 5b69 5d0a 0a20 2020 2020  ] = p0[i]..     
-0001d410: 2020 2023 2073 6574 2069 6e69 7469 616c     # set initial
-0001d420: 2075 6e63 6572 7461 696e 7469 6573 2028   uncertainties (
-0001d430: 6f70 7469 6f6e 616c 290a 2020 2020 2020  optional).      
-0001d440: 2020 7365 6c66 2e64 7030 203d 2064 7030    self.dp0 = dp0
-0001d450: 0a0a 2020 2020 2020 2020 2320 7374 6f72  ..        # stor
-0001d460: 6520 696e 666f 726d 6174 696f 6e73 206f  e informations o
-0001d470: 6e20 7061 7261 6d65 7465 7220 6c69 6d69  n parameter limi
-0001d480: 7473 2028 7573 6564 2062 7920 6d69 6e75  ts (used by minu
-0001d490: 6974 290a 2020 2020 2020 2020 7365 6c66  it).        self
-0001d4a0: 2e73 6574 4c69 6d69 7473 203d 206c 696d  .setLimits = lim
-0001d4b0: 6974 730a 2020 2020 2020 2020 7365 6c66  its.        self
-0001d4c0: 2e6c 696d 6974 7320 3d20 5b5d 0a20 2020  .limits = [].   
-0001d4d0: 2020 2020 2069 6620 6c69 6d69 7473 2069       if limits i
-0001d4e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001d4f0: 2020 2020 2020 2020 7365 6c66 2e6c 696d          self.lim
-0001d500: 6974 7320 3d20 5b5b 4e6f 6e65 2c20 4e6f  its = [[None, No
-0001d510: 6e65 5d5d 202a 206c 656e 2873 656c 662e  ne]] * len(self.
-0001d520: 706e 616d 7329 0a20 2020 2020 2020 2020  pnams).         
-0001d530: 2020 2069 6620 6c65 6e28 6e70 2e73 6861     if len(np.sha
-0001d540: 7065 286c 696d 6974 7329 2920 3d3d 2032  pe(limits)) == 2
-0001d550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d560: 2020 666f 7220 6c20 696e 206c 696d 6974    for l in limit
-0001d570: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0001d580: 2020 2020 2020 2069 6620 7479 7065 286c         if type(l
-0001d590: 5b30 5d29 203d 3d20 7479 7065 2822 2022  [0]) == type(" "
-0001d5a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001d5b0: 2020 2020 2020 2020 2020 2070 5f69 6420             p_id 
-0001d5c0: 3d20 7365 6c66 2e70 6e61 6d32 6964 5b6c  = self.pnam2id[l
-0001d5d0: 5b30 5d5d 0a20 2020 2020 2020 2020 2020  [0]].           
-0001d5e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0001d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d600: 2020 2020 2020 2070 5f69 6420 3d20 6c5b         p_id = l[
-0001d610: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-0001d620: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
-0001d630: 7473 5b70 5f69 645d 203d 205b 6c5b 315d  ts[p_id] = [l[1]
-0001d640: 2c20 6c5b 325d 5d0a 2020 2020 2020 2020  , l[2]].        
-0001d650: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001d660: 2020 2020 2020 2020 2020 6966 2074 7970            if typ
-0001d670: 6528 6c69 6d69 7473 5b30 5d29 203d 3d20  e(limits[0]) == 
-0001d680: 7479 7065 2822 2022 293a 0a20 2020 2020  type(" "):.     
-0001d690: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001d6a0: 5f69 6420 3d20 7365 6c66 2e70 6e61 6d32  _id = self.pnam2
-0001d6b0: 6964 5b6c 696d 6974 735b 305d 5d0a 2020  id[limits[0]].  
-0001d6c0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0001d6d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001d6e0: 2020 2020 2020 2020 705f 6964 203d 206c          p_id = l
-0001d6f0: 696d 6974 735b 305d 0a20 2020 2020 2020  imits[0].       
-0001d700: 2020 2020 2020 2020 2073 656c 662e 6c69           self.li
-0001d710: 6d69 7473 5b70 5f69 645d 203d 205b 6c69  mits[p_id] = [li
-0001d720: 6d69 7473 5b31 5d2c 206c 696d 6974 735b  mits[1], limits[
-0001d730: 325d 5d0a 0a20 2020 2020 2020 2023 2073  2]]..        # s
-0001d740: 746f 7265 2069 6e66 6f72 6d61 7469 6f6e  tore information
-0001d750: 206f 6e20 6669 7865 6420 7061 7261 6d65   on fixed parame
-0001d760: 7465 7273 0a20 2020 2020 2020 2073 656c  ters.        sel
-0001d770: 662e 6669 7850 6172 7320 3d20 6669 7850  f.fixPars = fixP
-0001d780: 6172 730a 2020 2020 2020 2020 7365 6c66  ars.        self
-0001d790: 2e66 6978 6564 5061 7273 203d 205b 4661  .fixedPars = [Fa
-0001d7a0: 6c73 655d 202a 2073 656c 662e 6e70 6172  lse] * self.npar
-0001d7b0: 0a20 2020 2020 2020 2069 6620 6669 7850  .        if fixP
-0001d7c0: 6172 7320 6973 206e 6f74 204e 6f6e 653a  ars is not None:
-0001d7d0: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
-0001d7e0: 6574 2070 6172 616d 6574 6572 206e 616d  et parameter nam
-0001d7f0: 6573 206f 7220 696e 6469 6365 7320 746f  es or indices to
-0001d800: 2066 6978 0a20 2020 2020 2020 2020 2020   fix.           
-0001d810: 2069 6620 6c65 6e28 6e70 2e73 6861 7065   if len(np.shape
-0001d820: 2866 6978 5061 7273 2929 203d 3d20 313a  (fixPars)) == 1:
-0001d830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d840: 2066 6f72 2066 2069 6e20 6669 7850 6172   for f in fixPar
-0001d850: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0001d860: 2020 2020 2020 2069 6620 7479 7065 2866         if type(f
-0001d870: 2920 3d3d 2074 7970 6528 2220 2229 3a0a  ) == type(" "):.
-0001d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d890: 2020 2020 2020 2020 705f 6964 203d 2073          p_id = s
-0001d8a0: 656c 662e 706e 616d 3269 645b 665d 0a20  elf.pnam2id[f]. 
-0001d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001ae40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001ae50: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0001ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae70: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0001ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae90: 2020 2020 2121 2120 636f 6e73 742e 2030      !!! const. 0
+0001aea0: 2e30 3035 2074 6f20 6176 6f69 6420 6c6f  .005 to avoid lo
+0001aeb0: 6728 302e 290a 2020 2020 2020 2020 2020  g(0.).          
+0001aec0: 2020 2020 2020 2020 2020 7365 6c66 2e67            self.g
+0001aed0: 6f66 203d 206e 326c 4c20 2d20 6e32 6c4c  of = n2lL - n2lL
+0001aee0: 5f73 6174 7572 6174 6564 0a0a 2020 2020  _saturated..    
+0001aef0: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+0001af00: 6f76 6964 6520 6d6f 6465 6c20 7661 6c75  ovide model valu
+0001af10: 6573 2061 6e64 206d 6f64 656c 2d72 656c  es and model-rel
+0001af20: 6174 6564 2075 6e63 6572 7461 696e 7469  ated uncertainti
+0001af30: 6573 2074 6f20 6461 7461 206f 626a 6563  es to data objec
+0001af40: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0001af50: 2020 7365 6c66 2e64 6174 612e 6d6f 6465    self.data.mode
+0001af60: 6c5f 7661 6c75 6573 203d 206d 6f64 656c  l_values = model
+0001af70: 5f76 616c 7565 730a 0a20 2020 2020 2020  _values..       
+0001af80: 2020 2020 2023 2072 6574 7572 6e20 3220       # return 2 
+0001af90: 2a20 6e65 672e 206c 6f67 4c0a 2020 2020  * neg. logL.    
+0001afa0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+0001afb0: 326c 4c0a 0a20 2020 2020 2020 2040 7374  2lL..        @st
+0001afc0: 6174 6963 6d65 7468 6f64 0a20 2020 2020  aticmethod.     
+0001afd0: 2020 2064 6566 206e 326c 4c50 6f69 7373     def n2lLPoiss
+0001afe0: 6f6e 2878 2c20 6c61 6d29 3a0a 2020 2020  on(x, lam):.    
+0001aff0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001b000: 2020 2020 2020 2020 6e65 672e 206c 6f67          neg. log
+0001b010: 6172 6974 686d 206f 6620 506f 6973 736f  arithm of Poisso
+0001b020: 6e20 6469 7374 7269 6275 7469 6f6e 2066  n distribution f
+0001b030: 6f72 2072 6561 6c2d 7661 6c75 6564 2078  or real-valued x
+0001b040: 0a0a 2020 2020 2020 2020 2020 2020 2222  ..            ""
+0001b050: 220a 2020 2020 2020 2020 2020 2020 7265  ".            re
+0001b060: 7475 726e 2032 2e30 202a 2028 6c61 6d20  turn 2.0 * (lam 
+0001b070: 2d20 7820 2a20 6e70 2e6c 6f67 286c 616d  - x * np.log(lam
+0001b080: 2920 2b20 6c6f 6767 616d 6d61 2878 202b  ) + loggamma(x +
+0001b090: 2031 2e30 2929 0a0a 2020 2020 2020 2020   1.0))..        
+0001b0a0: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+0001b0b0: 2020 2020 2020 6465 6620 6e32 6c4c 7350        def n2lLsP
+0001b0c0: 6f69 7373 6f6e 2878 6b2c 206c 616d 2c20  oisson(xk, lam, 
+0001b0d0: 6d75 293a 0a20 2020 2020 2020 2020 2020  mu):.           
+0001b0e0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
+0001b0f0: 2032 2a20 6e65 672e 206c 6f67 6172 6974   2* neg. logarit
+0001b100: 686d 206f 6620 6765 6e65 7261 6c69 7a65  hm of generalize
+0001b110: 6420 506f 6973 736f 6e20 6469 7374 7269  d Poisson distri
+0001b120: 6275 7469 6f6e 3a0a 2020 2020 2020 2020  bution:.        
+0001b130: 2020 2020 7368 6966 7465 6420 746f 206e      shifted to n
+0001b140: 6577 206d 6561 6e20 6d75 2066 6f72 2072  ew mean mu for r
+0001b150: 6561 6c2d 7661 6c75 6564 2078 6b0a 2020  eal-valued xk.  
+0001b160: 2020 2020 2020 2020 2020 666f 7220 6c61            for la
+0001b170: 6d3d 6d75 2c20 7468 6520 7374 616e 6461  m=mu, the standa
+0001b180: 7264 2050 6f69 7373 6f6e 2064 6973 7472  rd Poisson distr
+0001b190: 6962 7574 696f 6e20 6973 2072 6563 6f76  ibution is recov
+0001b1a0: 6572 6564 0a20 2020 2020 2020 2020 2020  ered.           
+0001b1b0: 206c 616d 3d73 6967 6d61 2a32 2069 7320   lam=sigma*2 is 
+0001b1c0: 7468 6520 7661 7269 616e 6365 206f 6620  the variance of 
+0001b1d0: 7468 6520 7368 6966 7465 6420 506f 6973  the shifted Pois
+0001b1e0: 736f 6e20 6469 7374 7269 6275 7469 6f6e  son distribution
+0001b1f0: 2e0a 2020 2020 2020 2020 2020 2020 2222  ..            ""
+0001b200: 220a 2020 2020 2020 2020 2020 2020 7873  ".            xs
+0001b210: 203d 2078 6b20 2b20 6c61 6d20 2d20 6d75   = xk + lam - mu
+0001b220: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001b230: 7572 6e20 322e 3020 2a20 286c 616d 202d  urn 2.0 * (lam -
+0001b240: 2078 7320 2a20 6e70 2e6c 6f67 286c 616d   xs * np.log(lam
+0001b250: 2920 2b20 6c6f 6767 616d 6d61 2878 7320  ) + loggamma(xs 
+0001b260: 2b20 312e 3029 290a 0a20 2020 2020 2020  + 1.0))..       
+0001b270: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+0001b280: 2020 2020 2020 2064 6566 206e 326c 4c47         def n2lLG
+0001b290: 6175 7373 2878 2c20 6c61 6d29 3a0a 2020  auss(x, lam):.  
+0001b2a0: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
+0001b2b0: 2020 2020 2020 2020 2020 6e65 6761 7469            negati
+0001b2c0: 7665 206c 6f67 2d6c 696b 656c 6968 6f6f  ve log-likelihoo
+0001b2d0: 6420 6f66 2047 6175 7373 6961 6e20 6170  d of Gaussian ap
+0001b2e0: 7072 6f78 696d 6174 696f 6e0a 2020 2020  proximation.    
+0001b2f0: 2020 2020 2020 2020 506f 6973 2878 2c20          Pois(x, 
+0001b300: 6c61 6d29 205c 7369 6d65 7120 4761 7573  lam) \simeq Gaus
+0001b310: 7328 782c 206d 753d 6c61 6d2c 2073 6967  s(x, mu=lam, sig
+0001b320: 6d61 5e32 3d6c 616d 290a 2020 2020 2020  ma^2=lam).      
+0001b330: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0001b340: 2020 2020 2020 7220 3d20 7820 2d20 6c61        r = x - la
+0001b350: 6d0a 2020 2020 2020 2020 2020 2020 7265  m.            re
+0001b360: 7475 726e 2072 202a 2072 202f 206c 616d  turn r * r / lam
+0001b370: 202b 206e 702e 6c6f 6728 6c61 6d29 0a0a   + np.log(lam)..
+0001b380: 2020 2020 2020 2020 4073 7461 7469 636d          @staticm
+0001b390: 6574 686f 640a 2020 2020 2020 2020 6465  ethod.        de
+0001b3a0: 6620 696e 7465 6772 616c 5f6f 7665 7242  f integral_overB
+0001b3b0: 696e 7328 6c65 6467 6573 2c20 7265 6467  ins(ledges, redg
+0001b3c0: 6573 2c20 662c 202a 7061 7229 3a0a 2020  es, f, *par):.  
+0001b3d0: 2020 2020 2020 2020 2020 2222 2243 616c            """Cal
+0001b3e0: 6375 6c61 7465 2061 7070 726f 782e 2069  culate approx. i
+0001b3f0: 6e74 6567 7261 6c20 6f66 206d 6f64 656c  ntegral of model
+0001b400: 206f 7665 7220 6269 6e73 2075 7369 6e67   over bins using
+0001b410: 2053 696d 7073 6f6e 2773 2072 756c 6522   Simpson's rule"
+0001b420: 2222 0a20 2020 2020 2020 2020 2020 2072  "".            r
+0001b430: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
+0001b440: 2020 2020 2020 2020 2872 6564 6765 7320          (redges 
+0001b450: 2d20 6c65 6467 6573 290a 2020 2020 2020  - ledges).      
+0001b460: 2020 2020 2020 2020 2020 2f20 362e 300a            / 6.0.
+0001b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b480: 2a20 280a 2020 2020 2020 2020 2020 2020  * (.            
+0001b490: 2020 2020 2020 2020 6628 6c65 6467 6573          f(ledges
+0001b4a0: 2c20 2a70 6172 290a 2020 2020 2020 2020  , *par).        
+0001b4b0: 2020 2020 2020 2020 2020 2020 2b20 342e              + 4.
+0001b4c0: 3020 2a20 6628 286c 6564 6765 7320 2b20  0 * f((ledges + 
+0001b4d0: 7265 6467 6573 2920 2f20 322e 302c 202a  redges) / 2.0, *
+0001b4e0: 7061 7229 0a20 2020 2020 2020 2020 2020  par).           
+0001b4f0: 2020 2020 2020 2020 202b 2066 2872 6564           + f(red
+0001b500: 6765 732c 202a 7061 7229 0a20 2020 2020  ges, *par).     
+0001b510: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001b520: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0001b530: 2320 2d2d 2d20 656e 6420 6465 6669 6e69  # --- end defini
+0001b540: 7469 6f6e 206f 6620 636c 6173 7320 6843  tion of class hC
+0001b550: 6f73 7420 2d2d 2d2d 0a0a 2020 2020 230a  ost ----..    #.
+0001b560: 2020 2020 2320 2d2d 2d20 7370 6563 6961      # --- specia
+0001b570: 6c20 636f 6465 2066 6f72 2066 6974 2077  l code for fit w
+0001b580: 6974 6820 7573 6572 2d73 7570 706c 6965  ith user-supplie
+0001b590: 6420 636f 7374 2066 756e 6374 696f 6e0a  d cost function.
+0001b5a0: 2020 2020 2320 2020 2020 6f72 2070 6466      #     or pdf
+0001b5b0: 2066 6f72 206e 6567 2e20 6c6f 672d 6c69   for neg. log-li
+0001b5c0: 6b65 6c69 686f 6f64 2066 6974 0a20 2020  kelihood fit.   
+0001b5d0: 2023 0a0a 2020 2020 6465 6620 696e 6974   #..    def init
+0001b5e0: 5f6d 6c44 6174 6128 7365 6c66 2c20 7829  _mlData(self, x)
+0001b5f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0001b600: 2020 2020 2020 696e 6974 6961 6c69 7a65        initialize
+0001b610: 2064 6174 6120 6f62 6a65 6374 0a0a 2020   data object..  
+0001b620: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0001b630: 2020 2020 2d20 782c 2061 7272 6179 206f      - x, array o
+0001b640: 6620 666c 6f61 7473 0a20 2020 2020 2020  f floats.       
+0001b650: 2022 2222 0a0a 2020 2020 2020 2020 2320   """..        # 
+0001b660: 6372 6561 7465 2064 6174 6120 6f62 6a65  create data obje
+0001b670: 6374 2061 6e64 2070 6173 7320 616c 6c20  ct and pass all 
+0001b680: 696e 7075 7420 6172 6775 6d65 6e74 730a  input arguments.
+0001b690: 2020 2020 2020 2020 7365 6c66 2e6d 6c44          self.mlD
+0001b6a0: 6174 6120 3d20 7365 6c66 2e6d 6c44 6174  ata = self.mlDat
+0001b6b0: 6143 6f6e 7461 696e 6572 2873 656c 662c  aContainer(self,
+0001b6c0: 2078 290a 2020 2020 2020 2020 7365 6c66   x).        self
+0001b6d0: 2e64 6174 6120 3d20 7365 6c66 2e6d 6c44  .data = self.mlD
+0001b6e0: 6174 610a 0a20 2020 2064 6566 2069 6e69  ata..    def ini
+0001b6f0: 745f 6d6e 4669 7428 0a20 2020 2020 2020  t_mnFit(.       
+0001b700: 2073 656c 662c 0a20 2020 2020 2020 2075   self,.        u
+0001b710: 7365 7246 756e 6374 696f 6e2c 0a20 2020  serFunction,.   
+0001b720: 2020 2020 206d 6f64 656c 5f6b 7761 7267       model_kwarg
+0001b730: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+0001b740: 7030 3d4e 6f6e 652c 0a20 2020 2020 2020  p0=None,.       
+0001b750: 2064 7030 3d4e 6f6e 652c 0a20 2020 2020   dp0=None,.     
+0001b760: 2020 2063 6f6e 7374 7261 696e 7473 3d4e     constraints=N
+0001b770: 6f6e 652c 0a20 2020 2020 2020 2066 6978  one,.        fix
+0001b780: 5061 7273 3d4e 6f6e 652c 0a20 2020 2020  Pars=None,.     
+0001b790: 2020 206c 696d 6974 733d 4e6f 6e65 2c0a     limits=None,.
+0001b7a0: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+0001b7b0: 2222 696e 6974 6961 6c69 7a65 2066 6974  ""initialize fit
+0001b7c0: 206f 626a 6563 7420 666f 7220 7369 6d70   object for simp
+0001b7d0: 6c65 206d 696e 7569 7420 6669 7420 7769  le minuit fit wi
+0001b7e0: 7468 0a20 2020 2020 2020 202a 2077 6974  th.        * wit
+0001b7f0: 6820 7573 6572 2d73 7570 706c 6965 6420  h user-supplied 
+0001b800: 636f 7374 2066 756e 6374 696f 6e20 6f72  cost function or
+0001b810: 0a20 2020 2020 2020 202a 2061 2070 726f  .        * a pro
+0001b820: 6261 6269 6c69 7479 2064 656e 7369 7479  bability density
+0001b830: 2066 756e 6374 696f 6e20 666f 7220 616e   function for an
+0001b840: 2075 6e62 696e 6e65 6420 6e65 672e 206c   unbinned neg. l
+0001b850: 6f67 2d4c 2066 6974 0a0a 2020 2020 2020  og-L fit..      
+0001b860: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0001b870: 2020 2d20 636f 7374 4675 6e63 7469 6f6e    - costFunction
+0001b880: 3a20 636f 7374 2066 756e 6374 696f 6e20  : cost function 
+0001b890: 6f72 2070 6466 0a20 2020 2020 2020 2020  or pdf.         
+0001b8a0: 202d 2070 303a 206e 702d 6172 7261 7920   - p0: np-array 
+0001b8b0: 6f66 2066 6c6f 6174 732c 2069 6e69 7469  of floats, initi
+0001b8c0: 616c 2070 6172 616d 6574 6572 2076 616c  al parameter val
+0001b8d0: 7565 730a 2020 2020 2020 2020 2020 2d20  ues.          - 
+0001b8e0: 6d6f 6465 6c5f 6b77 6172 6773 3a20 6f70  model_kwargs: op
+0001b8f0: 7469 6f6e 616c 2c20 6669 7420 7061 7261  tional, fit para
+0001b900: 6d65 7465 7273 2069 6620 6e6f 7420 6672  meters if not fr
+0001b910: 6f6d 206d 6f64 656c 2073 6967 6e61 7475  om model signatu
+0001b920: 7265 0a20 2020 2020 2020 2020 202d 2064  re.          - d
+0001b930: 7030 3a20 6172 7261 792d 6c69 6b65 2c20  p0: array-like, 
+0001b940: 696e 6974 6961 6c20 6775 6573 7320 6f66  initial guess of
+0001b950: 2070 6172 616d 6574 6572 2075 6e63 6572   parameter uncer
+0001b960: 7461 696e 7469 6573 2028 6f70 7469 6f6e  tainties (option
+0001b970: 616c 290a 2020 2020 2020 2020 2020 2d20  al).          - 
+0001b980: 7061 7261 6d65 7465 7220 636f 6e73 7472  parameter constr
+0001b990: 6169 6e74 733a 2028 6e65 7374 6564 2920  aints: (nested) 
+0001b9a0: 6c69 7374 2873 293a 205b 7061 7261 6d65  list(s): [parame
+0001b9b0: 7465 7220 6e61 6d65 2c20 7661 6c75 652c  ter name, value,
+0001b9c0: 2075 6e63 6572 7461 696e 7479 5d0a 2020   uncertainty].  
+0001b9d0: 2020 2020 2020 2020 2d20 6669 7820 7061          - fix pa
+0001b9e0: 7261 6d65 7465 7228 7329 2069 6e20 6669  rameter(s) in fi
+0001b9f0: 743a 206c 6973 7420 6f66 2070 6172 616d  t: list of param
+0001ba00: 6574 6572 206e 616d 6573 206f 7220 696e  eter names or in
+0001ba10: 6469 6365 730a 2020 2020 2020 2020 2020  dices.          
+0001ba20: 2d20 6c69 6d69 7473 3a20 286e 6573 7465  - limits: (neste
+0001ba30: 6429 206c 6973 7428 7329 3a20 5b70 6172  d) list(s): [par
+0001ba40: 616d 6574 6572 206e 616d 652c 206d 696e  ameter name, min
+0001ba50: 2c20 6d61 785d 206f 720a 2020 2020 2020  , max] or.      
+0001ba60: 2020 2020 2020 5b70 6172 616d 6574 6572        [parameter
+0001ba70: 2069 6e64 6578 2c20 6d69 6e2c 206d 6178   index, min, max
+0001ba80: 5d0a 2020 2020 2020 2020 2222 220a 2020  ].        """.  
+0001ba90: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
+0001baa0: 7461 2069 7320 4e6f 6e65 2061 6e64 2073  ta is None and s
+0001bab0: 656c 662e 6669 745f 7479 7065 2021 3d20  elf.fit_type != 
+0001bac0: 2275 7365 7222 3a0a 2020 2020 2020 2020  "user":.        
+0001bad0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0001bae0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0001baf0: 2020 2020 2020 2220 2121 2120 6d6e 4669        " !!! mnFi
+0001bb00: 742e 696e 6974 5f6d 6e46 6974 3a20 6e6f  t.init_mnFit: no
+0001bb10: 2064 6174 6120 6f62 6a65 6374 2064 6566   data object def
+0001bb20: 696e 6564 202d 2063 616c 6c20 696e 6974  ined - call init
+0001bb30: 5f64 6174 6128 2922 0a20 2020 2020 2020  _data()".       
+0001bb40: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0001bb50: 2320 6765 7420 7061 7261 6d65 7465 7273  # get parameters
+0001bb60: 206f 6620 6d6f 6465 6c20 6675 6e63 7469   of model functi
+0001bb70: 6f6e 2074 6f20 7365 7420 7374 6172 7420  on to set start 
+0001bb80: 7661 6c75 6573 2066 6f72 2066 6974 0a20  values for fit. 
+0001bb90: 2020 2020 2020 2069 6620 6d6f 6465 6c5f         if model_
+0001bba0: 6b77 6172 6773 2069 7320 4e6f 6e65 3a0a  kwargs is None:.
+0001bbb0: 2020 2020 2020 2020 2020 2020 6172 6773              args
+0001bbc0: 2c20 6d6f 6465 6c5f 6b77 6172 6773 203d  , model_kwargs =
+0001bbd0: 2067 6574 5f66 756e 6374 696f 6e53 6967   get_functionSig
+0001bbe0: 6e61 7475 7265 2875 7365 7246 756e 6374  nature(userFunct
+0001bbf0: 696f 6e29 0a0a 2020 2020 2020 2020 7061  ion)..        pa
+0001bc00: 7220 3d20 286d 6f64 656c 5f6b 7761 7267  r = (model_kwarg
+0001bc10: 732c 2070 302c 2064 7030 2c20 636f 6e73  s, p0, dp0, cons
+0001bc20: 7472 6169 6e74 732c 2066 6978 5061 7273  traints, fixPars
+0001bc30: 2c20 6c69 6d69 7473 290a 2020 2020 2020  , limits).      
+0001bc40: 2020 7365 6c66 2e5f 7365 7475 7046 6974    self._setupFit
+0001bc50: 5061 7261 6d65 7465 7273 282a 7061 7229  Parameters(*par)
+0001bc60: 0a0a 2020 2020 2020 2020 2320 7365 7420  ..        # set 
+0001bc70: 7570 2063 6f73 7420 6675 6e63 7469 6f6e  up cost function
+0001bc80: 2066 6f72 2069 6d69 6e75 6974 0a20 2020   for iminuit.   
+0001bc90: 2020 2020 2073 656c 662e 636f 7374 6620       self.costf 
+0001bca0: 3d20 7365 6c66 2e6d 6e43 6f73 7428 7365  = self.mnCost(se
+0001bcb0: 6c66 2c20 7573 6572 4675 6e63 7469 6f6e  lf, userFunction
+0001bcc0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+0001bcd0: 7365 7475 704d 696e 7569 7428 6d6f 6465  setupMinuit(mode
+0001bce0: 6c5f 6b77 6172 6773 290a 0a20 2020 2064  l_kwargs)..    d
+0001bcf0: 6566 2073 6574 5f6d 6e4f 7074 696f 6e73  ef set_mnOptions
+0001bd00: 2873 656c 662c 2072 756e 5f6d 696e 6f73  (self, run_minos
+0001bd10: 3d4e 6f6e 652c 206e 6567 326c 6f67 4c3d  =None, neg2logL=
+0001bd20: 4e6f 6e65 2c20 7175 6965 743d 4e6f 6e65  None, quiet=None
+0001bd30: 293a 0a20 2020 2020 2020 2022 2222 4465  ):.        """De
+0001bd40: 6669 6e65 206f 7074 696f 6e73 2066 6f72  fine options for
+0001bd50: 206d 696e 7569 7420 6669 7420 7769 7468   minuit fit with
+0001bd60: 2075 7365 7220 636f 7374 2066 756e 6374   user cost funct
+0001bd70: 696f 6e0a 0a20 2020 2020 2020 2041 7267  ion..        Arg
+0001bd80: 733a 0a0a 2020 2020 2020 2020 2d20 7275  s:..        - ru
+0001bd90: 6e5f 6d69 6e6f 733a 2072 756e 206d 696e  n_minos: run min
+0001bda0: 6f73 2070 726f 6669 6c65 206c 696b 656c  os profile likel
+0001bdb0: 6968 6f6f 6420 7363 616e 0a20 2020 2020  ihood scan.     
+0001bdc0: 2020 202d 206e 6567 326c 6f67 4c3a 2063     - neg2logL: c
+0001bdd0: 6f73 7420 6675 6e63 7469 6f6e 2069 7320  ost function is 
+0001bde0: 2d32 206e 6567 4c6f 674c 0a20 2020 2020  -2 negLogL.     
+0001bdf0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0001be00: 6620 7275 6e5f 6d69 6e6f 7320 6973 206e  f run_minos is n
+0001be10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0001be20: 2020 2020 2073 656c 662e 7275 6e5f 6d69       self.run_mi
+0001be30: 6e6f 7320 3d20 7275 6e5f 6d69 6e6f 730a  nos = run_minos.
+0001be40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001be50: 2e6f 7074 696f 6e73 5b22 7275 6e5f 6d69  .options["run_mi
+0001be60: 6e6f 7322 5d5b 305d 203d 2069 6e74 2872  nos"][0] = int(r
+0001be70: 756e 5f6d 696e 6f73 290a 2020 2020 2020  un_minos).      
+0001be80: 2020 6966 206e 6567 326c 6f67 4c20 6973    if neg2logL is
+0001be90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001bea0: 2020 2020 2020 2073 656c 662e 6e65 6732         self.neg2
+0001beb0: 6c6f 674c 203d 206e 6567 326c 6f67 4c0a  logL = neg2logL.
+0001bec0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001bed0: 2e6f 7074 696f 6e73 5b22 6e65 6732 6c6f  .options["neg2lo
+0001bee0: 674c 225d 5b30 5d20 3d20 696e 7428 6e65  gL"][0] = int(ne
+0001bef0: 6732 6c6f 674c 290a 2020 2020 2020 2020  g2logL).        
+0001bf00: 2020 2020 6966 2073 656c 662e 6e65 6732      if self.neg2
+0001bf10: 6c6f 674c 3a0a 2020 2020 2020 2020 2020  logL:.          
+0001bf20: 2020 2020 2020 7365 6c66 2e45 7272 4465        self.ErrDe
+0001bf30: 6620 3d20 312e 300a 2020 2020 2020 2020  f = 1.0.        
+0001bf40: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001bf50: 2020 2020 2020 2020 2020 7365 6c66 2e45            self.E
+0001bf60: 7272 4465 6620 3d20 302e 350a 2020 2020  rrDef = 0.5.    
+0001bf70: 2020 2020 6966 2071 7569 6574 2069 7320      if quiet is 
+0001bf80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001bf90: 2020 2020 2020 7365 6c66 2e71 7569 6574        self.quiet
+0001bfa0: 203d 2071 7569 6574 0a0a 2020 2020 636c   = quiet..    cl
+0001bfb0: 6173 7320 6d6c 4461 7461 436f 6e74 6169  ass mlDataContai
+0001bfc0: 6e65 723a 0a20 2020 2020 2020 2022 2222  ner:.        """
+0001bfd0: 0a20 2020 2020 2020 2043 6f6e 7461 696e  .        Contain
+0001bfe0: 6572 2066 6f72 2067 656e 6572 616c 2028  er for general (
+0001bff0: 696e 6465 7865 6429 2064 6174 610a 0a20  indexed) data.. 
+0001c000: 2020 2020 2020 2044 6174 6120 4d65 6d62         Data Memb
+0001c010: 6572 733a 0a0a 2020 2020 2020 2020 2d20  ers:..        - 
+0001c020: 782c 2061 7272 6179 206f 6620 666c 6f61  x, array of floa
+0001c030: 7473 3a20 6461 7461 0a0a 0a20 2020 2020  ts: data...     
+0001c040: 2020 204d 6574 686f 6473 3a0a 0a20 2020     Methods:..   
+0001c050: 2020 2020 202d 706c 6f74 2829 3a20 7265       -plot(): re
+0001c060: 7475 726e 2066 6967 7572 6520 7769 7468  turn figure with
+0001c070: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
+0001c080: 6f66 2064 6174 610a 2020 2020 2020 2020  of data.        
+0001c090: 2222 220a 0a20 2020 2020 2020 2064 6566  """..        def
+0001c0a0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0001c0b0: 6f75 7465 722c 2078 293a 0a20 2020 2020  outer, x):.     
+0001c0c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001c0d0: 2020 2020 2020 2073 746f 7265 2064 6174         store dat
+0001c0e0: 610a 0a20 2020 2020 2020 2020 2020 2041  a..            A
+0001c0f0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0001c100: 202d 2078 2c20 6172 7261 7920 6f66 2066   - x, array of f
+0001c110: 6c6f 6174 730a 2020 2020 2020 2020 2020  loats.          
+0001c120: 2020 2d20 7175 6965 743a 2062 6f6f 6c65    - quiet: boole
+0001c130: 616e 2c20 636f 6e74 726f 6c73 2070 7269  an, controls pri
+0001c140: 6e74 6564 206f 7574 7075 740a 0a20 2020  nted output..   
+0001c150: 2020 2020 2020 2020 2022 2222 0a0a 2020           """..  
+0001c160: 2020 2020 2020 2020 2020 7365 6c66 2e78            self.x
+0001c170: 203d 206e 702e 6173 6172 7261 7928 7829   = np.asarray(x)
+0001c180: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001c190: 662e 646c 656e 6774 6820 3d20 6c65 6e28  f.dlength = len(
+0001c1a0: 7365 6c66 2e78 290a 0a20 2020 2020 2020  self.x)..       
+0001c1b0: 2064 6566 2070 6c6f 7428 0a20 2020 2020   def plot(.     
+0001c1c0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
+0001c1d0: 2020 2020 2020 2020 206e 756d 3d22 696e           num="in
+0001c1e0: 6465 7865 6420 6461 7461 222c 0a20 2020  dexed data",.   
+0001c1f0: 2020 2020 2020 2020 2066 6967 7369 7a65           figsize
+0001c200: 3d28 372e 352c 2036 2e35 292c 0a20 2020  =(7.5, 6.5),.   
+0001c210: 2020 2020 2020 2020 2064 6174 615f 6c61           data_la
+0001c220: 6265 6c3d 2244 6174 6122 2c0a 2020 2020  bel="Data",.    
+0001c230: 2020 2020 2020 2020 706c 6f74 5f72 6573          plot_res
+0001c240: 6964 7561 6c3d 4661 6c73 652c 0a20 2020  idual=False,.   
+0001c250: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+0001c260: 2020 2020 2222 2272 6574 7572 6e20 6669      """return fi
+0001c270: 6775 7265 2077 6974 6820 6869 7374 6f67  gure with histog
+0001c280: 7261 6d20 6461 7461 2061 6e64 2075 6e63  ram data and unc
+0001c290: 6572 7461 696e 7469 6573 2222 220a 0a20  ertainties""".. 
+0001c2a0: 2020 2020 2020 2020 2020 2066 6967 203d             fig =
+0001c2b0: 2070 6c74 2e66 6967 7572 6528 6e75 6d3d   plt.figure(num=
+0001c2c0: 6e75 6d2c 2066 6967 7369 7a65 3d66 6967  num, figsize=fig
+0001c2d0: 7369 7a65 290a 0a20 2020 2020 2020 2020  size)..         
+0001c2e0: 2020 2069 6620 706c 6f74 5f72 6573 6964     if plot_resid
+0001c2f0: 7561 6c3a 0a20 2020 2020 2020 2020 2020  ual:.           
+0001c300: 2020 2020 2070 7269 6e74 280a 2020 2020       print(.    
+0001c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c320: 2220 2121 2120 6d6e 4669 742e 6d6c 4461  " !!! mnFit.mlDa
+0001c330: 7461 2e70 6c6f 743a 2070 6c6f 7474 696e  ta.plot: plottin
+0001c340: 6720 7265 7369 6475 616c 7320 6e6f 7420  g residuals not 
+0001c350: 706f 7373 6962 6c65 2066 6f72 2075 7365  possible for use
+0001c360: 7220 4d4c 2066 6974 220a 2020 2020 2020  r ML fit".      
+0001c370: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0001c380: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0001c390: 2e78 2069 7320 4e6f 6e65 3a0a 2020 2020  .x is None:.    
+0001c3a0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0001c3b0: 7428 2220 2121 2120 6d6e 4669 742e 6d6c  t(" !!! mnFit.ml
+0001c3c0: 4461 7461 2e70 6c6f 743a 206e 6f20 6461  Data.plot: no da
+0001c3d0: 7461 206f 626a 6563 7420 6465 6669 6e65  ta object define
+0001c3e0: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
+0001c3f0: 2020 2020 7265 7475 726e 2066 6967 0a0a      return fig..
+0001c400: 2020 2020 2020 2020 2020 2020 6d6e 203d              mn =
+0001c410: 206d 696e 2873 656c 662e 7829 0a20 2020   min(self.x).   
+0001c420: 2020 2020 2020 2020 206d 7820 3d20 6d61           mx = ma
+0001c430: 7828 7365 6c66 2e78 290a 2020 2020 2020  x(self.x).      
+0001c440: 2020 2020 2020 796d 6e20 3d20 302e 300a        ymn = 0.0.
+0001c450: 2020 2020 2020 2020 2020 2020 796d 7820              ymx 
+0001c460: 3d20 302e 3235 202f 2028 6d78 202d 206d  = 0.25 / (mx - m
+0001c470: 6e29 0a20 2020 2020 2020 2020 2020 2070  n).            p
+0001c480: 6c74 2e76 6c69 6e65 7328 0a20 2020 2020  lt.vlines(.     
+0001c490: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001c4a0: 782c 2079 6d6e 2c20 796d 782c 206c 773d  x, ymn, ymx, lw=
+0001c4b0: 312c 2063 6f6c 6f72 3d22 6772 6579 222c  1, color="grey",
+0001c4c0: 2061 6c70 6861 3d30 2e35 2c20 6c61 6265   alpha=0.5, labe
+0001c4d0: 6c3d 6461 7461 5f6c 6162 656c 0a20 2020  l=data_label.   
+0001c4e0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0001c4f0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+0001c500: 6967 0a0a 2020 2020 2320 2d2d 2d20 636c  ig..    # --- cl
+0001c510: 6173 7320 656e 6361 7073 756c 6174 696e  ass encapsulatin
+0001c520: 6720 7573 6572 2d64 6566 696e 6564 2063  g user-defined c
+0001c530: 6f73 7420 6675 6e63 7469 6f6e 0a20 2020  ost function.   
+0001c540: 2063 6c61 7373 206d 6e43 6f73 743a 0a20   class mnCost:. 
+0001c550: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001c560: 2020 2049 6e74 6572 6661 6365 2066 6f72     Interface for
+0001c570: 2073 696d 706c 6520 6d69 6e75 6974 2066   simple minuit f
+0001c580: 6974 2077 6974 6820 7573 6572 2d73 7570  it with user-sup
+0001c590: 706c 6965 6420 636f 7374 2066 756e 6374  plied cost funct
+0001c5a0: 696f 6e2e 0a0a 2020 2020 2020 2020 5468  ion...        Th
+0001c5b0: 6520 5f5f 6361 6c6c 5f5f 206d 6574 686f  e __call__ metho
+0001c5c0: 6420 6f66 2074 6869 7320 636c 6173 7320  d of this class 
+0001c5d0: 6973 2063 616c 6c65 6420 6279 2069 6d69  is called by imi
+0001c5e0: 6e75 6974 2e0a 0a20 2020 2020 2020 2041  nuit...        A
+0001c5f0: 7267 733a 0a0a 2020 2020 2020 2020 2020  rgs:..          
+0001c600: 2d20 7573 6572 436f 7374 4675 6e63 7469  - userCostFuncti
+0001c610: 6f6e 3a20 7573 6572 2d73 7570 706c 6965  on: user-supplie
+0001c620: 6420 636f 7374 2066 756e 6374 696f 6e20  d cost function 
+0001c630: 666f 7220 6d69 6e75 6974 3b0a 2020 2020  for minuit;.    
+0001c640: 2020 2020 2020 2020 206d 7573 7420 6265           must be
+0001c650: 2061 206e 6567 6174 6976 6520 6c6f 672d   a negative log-
+0001c660: 6c69 6b65 6c69 686f 6f64 0a20 2020 2020  likelihood.     
+0001c670: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0001c680: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0001c690: 662c 206f 7574 6572 2c20 7573 6572 4675  f, outer, userFu
+0001c6a0: 6e63 7469 6f6e 293a 0a20 2020 2020 2020  nction):.       
+0001c6b0: 2020 2020 2073 656c 662e 7175 6965 7420       self.quiet 
+0001c6c0: 3d20 6f75 7465 722e 7175 6965 740a 2020  = outer.quiet.  
+0001c6d0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0001c6e0: 6174 6120 3d20 6f75 7465 722e 6461 7461  ata = outer.data
+0001c6f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001c700: 7365 6c66 2e64 6174 6120 6973 204e 6f6e  self.data is Non
+0001c710: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001c720: 2020 2073 656c 662e 636f 7374 203d 2075     self.cost = u
+0001c730: 7365 7246 756e 6374 696f 6e0a 2020 2020  serFunction.    
+0001c740: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0001c750: 6f74 2073 656c 662e 7175 6965 743a 0a20  ot self.quiet:. 
+0001c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c770: 2020 2070 7269 6e74 2822 2a3d 3d2a 206d     print("*==* m
+0001c780: 6e46 6974 2e6d 6e43 6f73 743a 2066 6974  nFit.mnCost: fit
+0001c790: 2077 6974 6820 7573 6572 2d73 7570 706c   with user-suppl
+0001c7a0: 6965 6420 636f 7374 2066 756e 6374 696f  ied cost functio
+0001c7b0: 6e27 2229 0a20 2020 2020 2020 2020 2020  n'").           
+0001c7c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001c7d0: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+0001c7e0: 696e 7374 616e 6365 2873 656c 662e 6461  instance(self.da
+0001c7f0: 7461 2c20 6d6e 4669 742e 6d6c 4461 7461  ta, mnFit.mlData
+0001c800: 436f 6e74 6169 6e65 7229 3a0a 2020 2020  Container):.    
+0001c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c820: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0001c830: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001c840: 2020 2020 2020 2020 2020 2220 2121 2120            " !!! 
+0001c850: 6d6e 4669 742e 6d6e 436f 7374 3a20 6578  mnFit.mnCost: ex
+0001c860: 7065 6374 696e 6720 6461 7461 2063 6f6e  pecting data con
+0001c870: 7461 696e 6572 206f 6620 7479 7065 2027  tainer of type '
+0001c880: 6d6c 4461 7461 436f 6e74 6169 6e65 7227  mlDataContainer'
+0001c890: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0001c8a0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001c8b0: 2020 2020 2020 2020 7365 6c66 2e6d 6f64          self.mod
+0001c8c0: 656c 203d 2075 7365 7246 756e 6374 696f  el = userFunctio
+0001c8d0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+0001c8e0: 2020 7365 6c66 2e63 6f73 7420 3d20 7365    self.cost = se
+0001c8f0: 6c66 2e6e 6c4c 636f 7374 0a20 2020 2020  lf.nlLcost.     
+0001c900: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0001c910: 7420 7365 6c66 2e71 7569 6574 3a0a 2020  t self.quiet:.  
+0001c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c930: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
+0001c940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c950: 2022 2a3d 3d2a 206d 6e46 6974 2e6d 6e43   "*==* mnFit.mnC
+0001c960: 6f73 743a 206e 6567 4c6f 674c 2066 6974  ost: negLogL fit
+0001c970: 2077 6974 6820 7573 6572 2d64 6566 696e   with user-defin
+0001c980: 6564 2064 656e 7369 7479 2066 756e 6374  ed density funct
+0001c990: 696f 6e27 220a 2020 2020 2020 2020 2020  ion'".          
+0001c9a0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0001c9b0: 2020 2020 2020 2020 2023 2074 616b 6520           # take 
+0001c9c0: 6163 636f 756e 7420 6f66 2070 6f73 7369  account of possi
+0001c9d0: 626c 6520 7061 7261 6d65 7465 7220 636f  ble parameter co
+0001c9e0: 6e73 7472 6169 6e74 730a 2020 2020 2020  nstraints.      
+0001c9f0: 2020 2020 2020 7365 6c66 2e63 6f6e 7374        self.const
+0001ca00: 7261 696e 7473 203d 206f 7574 6572 2e63  raints = outer.c
+0001ca10: 6f6e 7374 7261 696e 7473 0a20 2020 2020  onstraints.     
+0001ca20: 2020 2020 2020 2073 656c 662e 6e63 6f6e         self.ncon
+0001ca30: 7374 7261 696e 7473 203d 206c 656e 2873  straints = len(s
+0001ca40: 656c 662e 636f 6e73 7472 6169 6e74 7329  elf.constraints)
+0001ca50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001ca60: 662e 4572 7244 6566 203d 206f 7574 6572  f.ErrDef = outer
+0001ca70: 2e45 7272 4465 660a 2020 2020 2020 2020  .ErrDef.        
+0001ca80: 2020 2020 7365 6c66 2e73 665f 6c4c 203d      self.sf_lL =
+0001ca90: 202d 322e 3020 2a20 7365 6c66 2e45 7272   -2.0 * self.Err
+0001caa0: 4465 660a 0a20 2020 2020 2020 2020 2020  Def..           
+0001cab0: 2023 2073 6574 2070 726f 7065 7220 7369   # set proper si
+0001cac0: 676e 6174 7572 6520 6f66 206d 6f64 656c  gnature of model
+0001cad0: 2066 756e 6374 696f 6e20 666f 7220 696d   function for im
+0001cae0: 696e 7569 740a 2020 2020 2020 2020 2020  inuit.          
+0001caf0: 2020 7365 6c66 2e70 6e61 6d73 203d 206f    self.pnams = o
+0001cb00: 7574 6572 2e70 6e61 6d73 0a20 2020 2020  uter.pnams.     
+0001cb10: 2020 2020 2020 2073 656c 662e 6e70 6172         self.npar
+0001cb20: 203d 206f 7574 6572 2e6e 7061 720a 0a20   = outer.npar.. 
+0001cb30: 2020 2020 2020 2020 2020 2023 2066 6f72             # for
+0001cb40: 2074 6869 7320 6b69 6e64 206f 6620 6669   this kind of fi
+0001cb50: 742c 2073 6f6d 6520 696e 7075 7420 616e  t, some input an
+0001cb60: 6420 6f75 7075 7420 7175 616e 7469 7469  d ouput quantiti
+0001cb70: 6573 2061 7265 206e 6f74 206b 6e6f 776e  es are not known
+0001cb80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001cb90: 662e 676f 6620 3d20 4e6f 6e65 0a20 2020  f.gof = None.   
+0001cba0: 2020 2020 2020 2020 2073 656c 662e 6e64           self.nd
+0001cbb0: 6f66 203d 204e 6f6e 650a 0a20 2020 2020  of = None..     
+0001cbc0: 2020 2064 6566 205f 5f63 616c 6c5f 5f28     def __call__(
+0001cbd0: 7365 6c66 2c20 2a70 6172 293a 0a20 2020  self, *par):.   
+0001cbe0: 2020 2020 2020 2020 2063 6f73 7420 3d20           cost = 
+0001cbf0: 302e 300a 2020 2020 2020 2020 2020 2020  0.0.            
+0001cc00: 2320 6164 6420 636f 6e73 7472 6169 6e74  # add constraint
+0001cc10: 7320 746f 2063 6f73 740a 2020 2020 2020  s to cost.      
+0001cc20: 2020 2020 2020 6966 2073 656c 662e 6e63        if self.nc
+0001cc30: 6f6e 7374 7261 696e 7473 3a0a 2020 2020  onstraints:.    
+0001cc40: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001cc50: 6320 696e 2073 656c 662e 636f 6e73 7472  c in self.constr
+0001cc60: 6169 6e74 733a 0a20 2020 2020 2020 2020  aints:.         
+0001cc70: 2020 2020 2020 2020 2020 2070 5f69 6420             p_id 
+0001cc80: 3d20 635b 305d 0a20 2020 2020 2020 2020  = c[0].         
+0001cc90: 2020 2020 2020 2020 2020 2072 203d 2028             r = (
+0001cca0: 7061 725b 705f 6964 5d20 2d20 635b 315d  par[p_id] - c[1]
+0001ccb0: 2920 2f20 635b 325d 0a20 2020 2020 2020  ) / c[2].       
+0001ccc0: 2020 2020 2020 2020 2020 2020 2063 6f73               cos
+0001ccd0: 7420 2b3d 2072 202a 2072 0a20 2020 2020  t += r * r.     
+0001cce0: 2020 2020 2020 2020 2020 2063 6f73 7420             cost 
+0001ccf0: 2a3d 2073 656c 662e 4572 7244 6566 0a20  *= self.ErrDef. 
+0001cd00: 2020 2020 2020 2020 2020 2023 2063 616c             # cal
+0001cd10: 6c65 6420 6974 6572 6174 6976 656c 7920  led iteratively 
+0001cd20: 6279 206d 696e 7569 740a 2020 2020 2020  by minuit.      
+0001cd30: 2020 2020 2020 7265 7475 726e 2063 6f73        return cos
+0001cd40: 7420 2b20 7365 6c66 2e63 6f73 7428 2a70  t + self.cost(*p
+0001cd50: 6172 290a 0a20 2020 2020 2020 2064 6566  ar)..        def
+0001cd60: 206e 6c4c 636f 7374 2873 656c 662c 202a   nlLcost(self, *
+0001cd70: 7061 7229 3a0a 2020 2020 2020 2020 2020  par):.          
+0001cd80: 2020 2222 226e 6567 6174 6976 6520 6c6f    """negative lo
+0001cd90: 6720 6c69 6b65 6c69 686f 6f64 206f 6620  g likelihood of 
+0001cda0: 6461 7461 2061 6e64 2075 7365 722d 6465  data and user-de
+0001cdb0: 6669 6e65 6420 5044 4620 616e 6422 2222  fined PDF and"""
+0001cdc0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+0001cdd0: 6865 636b 2069 6620 5044 4620 6973 206e  heck if PDF is n
+0001cde0: 6f6d 616c 697a 6564 2074 6f20 310a 2020  omalized to 1.  
+0001cdf0: 2020 2020 2020 2020 2020 2320 2e2e 2e0a            # ....
+0001ce00: 0a20 2020 2020 2020 2020 2020 206c 4c20  .            lL 
+0001ce10: 3d20 6e70 2e73 756d 286e 702e 6c6f 6728  = np.sum(np.log(
+0001ce20: 7365 6c66 2e6d 6f64 656c 2873 656c 662e  self.model(self.
+0001ce30: 6461 7461 2e78 2c20 2a70 6172 2929 290a  data.x, *par))).
+0001ce40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001ce50: 726e 2073 656c 662e 7366 5f6c 4c20 2a20  rn self.sf_lL * 
+0001ce60: 6c4c 0a0a 2020 2020 2320 2d2d 2d20 656e  lL..    # --- en
+0001ce70: 6420 6465 6669 6e69 7469 6f6e 206f 6620  d definition of 
+0001ce80: 636c 6173 7320 6d6e 436f 7374 202d 2d2d  class mnCost ---
+0001ce90: 2d0a 0a20 2020 2023 0a20 2020 2023 202d  -..    #.    # -
+0001cea0: 2d2d 2063 6f6d 6d6f 6e20 636f 6465 2066  -- common code f
+0001ceb0: 6f72 2061 6c6c 2066 6974 2074 7970 6573  or all fit types
+0001cec0: 0a20 2020 2023 0a0a 2020 2020 6465 6620  .    #..    def 
+0001ced0: 5f73 6574 7570 4669 7450 6172 616d 6574  _setupFitParamet
+0001cee0: 6572 7328 7365 6c66 2c20 6d6f 6465 6c5f  ers(self, model_
+0001cef0: 6b77 6172 6773 2c20 7030 2c20 6470 302c  kwargs, p0, dp0,
+0001cf00: 2063 6f6e 7374 7261 696e 7473 2c20 6669   constraints, fi
+0001cf10: 7850 6172 732c 206c 696d 6974 7329 3a0a  xPars, limits):.
+0001cf20: 2020 2020 2020 2020 2222 2273 6574 2075          """set u
+0001cf30: 7020 7061 7261 6d65 7465 7273 206e 6565  p parameters nee
+0001cf40: 6465 6420 666f 7220 4d69 6e75 6974 2061  ded for Minuit a
+0001cf50: 6e64 2063 6f73 7420 6675 6e63 7469 6f6e  nd cost function
+0001cf60: 2222 220a 0a20 2020 2020 2020 2023 2067  """..        # g
+0001cf70: 6574 2070 6172 616d 6574 6572 206e 616d  et parameter nam
+0001cf80: 6573 2066 726f 6d20 6b77 6172 6773 206f  es from kwargs o
+0001cf90: 6620 6d6f 6465 6c20 6675 6e63 7469 6f6e  f model function
+0001cfa0: 0a20 2020 2020 2020 2073 656c 662e 706e  .        self.pn
+0001cfb0: 616d 7320 3d20 6c69 7374 2e63 6f70 7928  ams = list.copy(
+0001cfc0: 6c69 7374 286d 6f64 656c 5f6b 7761 7267  list(model_kwarg
+0001cfd0: 732e 6b65 7973 2829 2929 0a20 2020 2020  s.keys())).     
+0001cfe0: 2020 2073 656c 662e 6e70 6172 203d 206c     self.npar = l
+0001cff0: 656e 2873 656c 662e 706e 616d 7329 0a20  en(self.pnams). 
+0001d000: 2020 2020 2020 2023 2064 6963 7469 6f6e         # diction
+0001d010: 6172 7920 6173 7369 676e 696e 6720 7061  ary assigning pa
+0001d020: 7261 6d65 7465 7220 6e61 6d65 2074 6f20  rameter name to 
+0001d030: 696e 6465 780a 2020 2020 2020 2020 7365  index.        se
+0001d040: 6c66 2e70 6e61 6d32 6964 203d 207b 7365  lf.pnam2id = {se
+0001d050: 6c66 2e70 6e61 6d73 5b69 5d3a 2069 2066  lf.pnams[i]: i f
+0001d060: 6f72 2069 2069 6e20 7261 6e67 6528 302c  or i in range(0,
+0001d070: 2073 656c 662e 6e70 6172 297d 0a0a 2020   self.npar)}..  
+0001d080: 2020 2020 2020 2320 7072 6f63 6573 7320        # process 
+0001d090: 616e 6420 7374 6f72 6520 7061 7261 6d65  and store parame
+0001d0a0: 7465 7220 636f 6e73 7472 6169 6e74 7320  ter constraints 
+0001d0b0: 2875 7365 6420 696e 2063 6f73 7420 6675  (used in cost fu
+0001d0c0: 6e63 7469 6f6e 290a 2020 2020 2020 2020  nction).        
+0001d0d0: 7365 6c66 2e73 6574 436f 6e73 7472 6169  self.setConstrai
+0001d0e0: 6e74 7320 3d20 636f 6e73 7472 6169 6e74  nts = constraint
+0001d0f0: 730a 2020 2020 2020 2020 7365 6c66 2e63  s.        self.c
+0001d100: 6f6e 7374 7261 696e 7473 203d 205b 5d0a  onstraints = [].
+0001d110: 2020 2020 2020 2020 6966 2063 6f6e 7374          if const
+0001d120: 7261 696e 7473 2069 7320 6e6f 7420 4e6f  raints is not No
+0001d130: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001d140: 6966 206c 656e 286e 702e 7368 6170 6528  if len(np.shape(
+0001d150: 636f 6e73 7472 6169 6e74 7329 2920 3d3d  constraints)) ==
+0001d160: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+0001d170: 2020 2020 666f 7220 6320 696e 2063 6f6e      for c in con
+0001d180: 7374 7261 696e 7473 3a0a 2020 2020 2020  straints:.      
+0001d190: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001d1a0: 6e61 6d65 2074 6f20 7061 7261 6d65 7465  name to paramete
+0001d1b0: 7220 6964 0a20 2020 2020 2020 2020 2020  r id.           
+0001d1c0: 2020 2020 2020 2020 2069 6620 7479 7065           if type
+0001d1d0: 2863 5b30 5d29 203d 3d20 7479 7065 2822  (c[0]) == type("
+0001d1e0: 2022 293a 0a20 2020 2020 2020 2020 2020   "):.           
+0001d1f0: 2020 2020 2020 2020 2020 2020 2063 5b30               c[0
+0001d200: 5d20 3d20 7365 6c66 2e70 6e61 6d32 6964  ] = self.pnam2id
+0001d210: 5b63 5b30 5d5d 0a20 2020 2020 2020 2020  [c[0]].         
+0001d220: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001d230: 636f 6e73 7472 6169 6e74 732e 6170 7065  constraints.appe
+0001d240: 6e64 2863 290a 2020 2020 2020 2020 2020  nd(c).          
+0001d250: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001d260: 2020 2020 2020 2020 2320 6e61 6d65 2074          # name t
+0001d270: 6f20 7061 7261 6d65 7465 7220 6964 0a20  o parameter id. 
+0001d280: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001d290: 6620 7479 7065 2863 6f6e 7374 7261 696e  f type(constrain
+0001d2a0: 7473 5b30 5d29 203d 3d20 7479 7065 2822  ts[0]) == type("
+0001d2b0: 2022 293a 0a20 2020 2020 2020 2020 2020   "):.           
+0001d2c0: 2020 2020 2020 2020 2063 6f6e 7374 7261           constra
+0001d2d0: 696e 7473 5b30 5d20 3d20 7365 6c66 2e70  ints[0] = self.p
+0001d2e0: 6e61 6d32 6964 5b63 6f6e 7374 7261 696e  nam2id[constrain
+0001d2f0: 7473 5b30 5d5d 0a20 2020 2020 2020 2020  ts[0]].         
+0001d300: 2020 2020 2020 2073 656c 662e 636f 6e73         self.cons
+0001d310: 7472 6169 6e74 732e 6170 7065 6e64 2863  traints.append(c
+0001d320: 6f6e 7374 7261 696e 7473 290a 2020 2020  onstraints).    
+0001d330: 2020 2020 7365 6c66 2e6e 636f 6e73 7472      self.nconstr
+0001d340: 6169 6e74 7320 3d20 6c65 6e28 7365 6c66  aints = len(self
+0001d350: 2e63 6f6e 7374 7261 696e 7473 290a 0a20  .constraints).. 
+0001d360: 2020 2020 2020 2023 2073 6574 2069 6e69         # set ini
+0001d370: 7469 616c 2070 6172 616d 6574 6572 7320  tial parameters 
+0001d380: 666f 7220 6669 7420 2875 7365 6420 6279  for fit (used by
+0001d390: 206d 696e 7569 7429 0a20 2020 2020 2020   minuit).       
+0001d3a0: 2069 6620 7030 2069 7320 6e6f 7420 4e6f   if p0 is not No
+0001d3b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001d3c0: 666f 7220 692c 2070 6e61 6d20 696e 2065  for i, pnam in e
+0001d3d0: 6e75 6d65 7261 7465 2873 656c 662e 706e  numerate(self.pn
+0001d3e0: 616d 7329 3a0a 2020 2020 2020 2020 2020  ams):.          
+0001d3f0: 2020 2020 2020 6d6f 6465 6c5f 6b77 6172        model_kwar
+0001d400: 6773 5b70 6e61 6d5d 203d 2070 305b 695d  gs[pnam] = p0[i]
+0001d410: 0a0a 2020 2020 2020 2020 2320 7365 7420  ..        # set 
+0001d420: 696e 6974 6961 6c20 756e 6365 7274 6169  initial uncertai
+0001d430: 6e74 6965 7320 286f 7074 696f 6e61 6c29  nties (optional)
+0001d440: 0a20 2020 2020 2020 2073 656c 662e 6470  .        self.dp
+0001d450: 3020 3d20 6470 300a 0a20 2020 2020 2020  0 = dp0..       
+0001d460: 2023 2073 746f 7265 2069 6e66 6f72 6d61   # store informa
+0001d470: 7469 6f6e 7320 6f6e 2070 6172 616d 6574  tions on paramet
+0001d480: 6572 206c 696d 6974 7320 2875 7365 6420  er limits (used 
+0001d490: 6279 206d 696e 7569 7429 0a20 2020 2020  by minuit).     
+0001d4a0: 2020 2073 656c 662e 7365 744c 696d 6974     self.setLimit
+0001d4b0: 7320 3d20 6c69 6d69 7473 0a20 2020 2020  s = limits.     
+0001d4c0: 2020 2073 656c 662e 6c69 6d69 7473 203d     self.limits =
+0001d4d0: 205b 5d0a 2020 2020 2020 2020 6966 206c   [].        if l
+0001d4e0: 696d 6974 7320 6973 206e 6f74 204e 6f6e  imits is not Non
+0001d4f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001d500: 656c 662e 6c69 6d69 7473 203d 205b 5b4e  elf.limits = [[N
+0001d510: 6f6e 652c 204e 6f6e 655d 5d20 2a20 6c65  one, None]] * le
+0001d520: 6e28 7365 6c66 2e70 6e61 6d73 290a 2020  n(self.pnams).  
+0001d530: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+0001d540: 286e 702e 7368 6170 6528 6c69 6d69 7473  (np.shape(limits
+0001d550: 2929 203d 3d20 323a 0a20 2020 2020 2020  )) == 2:.       
+0001d560: 2020 2020 2020 2020 2066 6f72 206c 2069           for l i
+0001d570: 6e20 6c69 6d69 7473 3a0a 2020 2020 2020  n limits:.      
+0001d580: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001d590: 2074 7970 6528 6c5b 305d 2920 3d3d 2074   type(l[0]) == t
+0001d5a0: 7970 6528 2220 2229 3a0a 2020 2020 2020  ype(" "):.      
+0001d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5c0: 2020 705f 6964 203d 2073 656c 662e 706e    p_id = self.pn
+0001d5d0: 616d 3269 645b 6c5b 305d 5d0a 2020 2020  am2id[l[0]].    
+0001d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001d600: 2020 2020 2020 2020 2020 2020 2020 705f                p_
+0001d610: 6964 203d 206c 5b30 5d0a 2020 2020 2020  id = l[0].      
+0001d620: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001d630: 6c66 2e6c 696d 6974 735b 705f 6964 5d20  lf.limits[p_id] 
+0001d640: 3d20 5b6c 5b31 5d2c 206c 5b32 5d5d 0a20  = [l[1], l[2]]. 
+0001d650: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001d660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d670: 2069 6620 7479 7065 286c 696d 6974 735b   if type(limits[
+0001d680: 305d 2920 3d3d 2074 7970 6528 2220 2229  0]) == type(" ")
+0001d690: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001d6a0: 2020 2020 2020 705f 6964 203d 2073 656c        p_id = sel
+0001d6b0: 662e 706e 616d 3269 645b 6c69 6d69 7473  f.pnam2id[limits
+0001d6c0: 5b30 5d5d 0a20 2020 2020 2020 2020 2020  [0]].           
+0001d6d0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001d6e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001d6f0: 5f69 6420 3d20 6c69 6d69 7473 5b30 5d0a  _id = limits[0].
+0001d700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d710: 7365 6c66 2e6c 696d 6974 735b 705f 6964  self.limits[p_id
+0001d720: 5d20 3d20 5b6c 696d 6974 735b 315d 2c20  ] = [limits[1], 
+0001d730: 6c69 6d69 7473 5b32 5d5d 0a0a 2020 2020  limits[2]]..    
+0001d740: 2020 2020 2320 7374 6f72 6520 696e 666f      # store info
+0001d750: 726d 6174 696f 6e20 6f6e 2066 6978 6564  rmation on fixed
+0001d760: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
+0001d770: 2020 2020 7365 6c66 2e66 6978 5061 7273      self.fixPars
+0001d780: 203d 2066 6978 5061 7273 0a20 2020 2020   = fixPars.     
+0001d790: 2020 2073 656c 662e 6669 7865 6450 6172     self.fixedPar
+0001d7a0: 7320 3d20 5b46 616c 7365 5d20 2a20 7365  s = [False] * se
+0001d7b0: 6c66 2e6e 7061 720a 2020 2020 2020 2020  lf.npar.        
+0001d7c0: 6966 2066 6978 5061 7273 2069 7320 6e6f  if fixPars is no
+0001d7d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0001d7e0: 2020 2020 2320 6765 7420 7061 7261 6d65      # get parame
+0001d7f0: 7465 7220 6e61 6d65 7320 6f72 2069 6e64  ter names or ind
+0001d800: 6963 6573 2074 6f20 6669 780a 2020 2020  ices to fix.    
+0001d810: 2020 2020 2020 2020 6966 206c 656e 286e          if len(n
+0001d820: 702e 7368 6170 6528 6669 7850 6172 7329  p.shape(fixPars)
+0001d830: 2920 3d3d 2031 3a0a 2020 2020 2020 2020  ) == 1:.        
+0001d840: 2020 2020 2020 2020 666f 7220 6620 696e          for f in
+0001d850: 2066 6978 5061 7273 3a0a 2020 2020 2020   fixPars:.      
+0001d860: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001d870: 2074 7970 6528 6629 203d 3d20 7479 7065   type(f) == type
+0001d880: 2822 2022 293a 0a20 2020 2020 2020 2020  (" "):.         
+0001d890: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001d8a0: 5f69 6420 3d20 7365 6c66 2e70 6e61 6d32  _id = self.pnam2
+0001d8b0: 6964 5b66 5d0a 2020 2020 2020 2020 2020  id[f].          
+0001d8c0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
 0001d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8e0: 2070 5f69 6420 3d20 660a 2020 2020 2020   p_id = f.      
-0001d8f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001d900: 6c66 2e66 6978 6564 5061 7273 5b70 5f69  lf.fixedPars[p_i
-0001d910: 645d 203d 2054 7275 650a 2020 2020 2020  d] = True.      
-0001d920: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-0001d930: 6669 7865 6420 3d20 6c65 6e28 6669 7850  fixed = len(fixP
-0001d940: 6172 7329 0a20 2020 2020 2020 2020 2020  ars).           
-0001d950: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001d960: 2020 2020 2020 2069 6620 7479 7065 2866         if type(f
-0001d970: 6978 5061 7273 2920 3d3d 2074 7970 6528  ixPars) == type(
-0001d980: 2220 2229 3a0a 2020 2020 2020 2020 2020  " "):.          
-0001d990: 2020 2020 2020 2020 2020 705f 6964 203d            p_id =
-0001d9a0: 2073 656c 662e 706e 616d 3269 645b 6669   self.pnam2id[fi
-0001d9b0: 7850 6172 735d 0a20 2020 2020 2020 2020  xPars].         
-0001d9c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9e0: 2070 5f69 6420 3d20 6669 7850 6172 730a   p_id = fixPars.
-0001d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da00: 7365 6c66 2e66 6978 6564 5061 7273 5b70  self.fixedPars[p
-0001da10: 5f69 645d 203d 2054 7275 650a 2020 2020  _id] = True.    
-0001da20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001da30: 2e6e 6669 7865 6420 3d20 310a 2020 2020  .nfixed = 1.    
-0001da40: 2020 2020 2020 2020 2320 6765 7420 7061          # get pa
-0001da50: 7261 6d65 7465 7220 6e61 6d65 7320 6f72  rameter names or
-0001da60: 2069 6e64 6963 6573 206f 6620 6669 7865   indices of fixe
-0001da70: 6420 7061 7261 6d65 7465 7273 0a20 2020  d parameters.   
-0001da80: 2020 2020 2020 2020 2073 656c 662e 6672           self.fr
-0001da90: 6565 5061 724e 616d 7320 3d20 5b5d 0a20  eeParNams = []. 
-0001daa0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001dab0: 6669 7865 6450 6172 4e61 6d73 203d 205b  fixedParNams = [
-0001dac0: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
-0001dad0: 7220 692c 2066 6978 6564 2069 6e20 656e  r i, fixed in en
-0001dae0: 756d 6572 6174 6528 7365 6c66 2e66 6978  umerate(self.fix
-0001daf0: 6564 5061 7273 293a 0a20 2020 2020 2020  edPars):.       
-0001db00: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0001db10: 6669 7865 643a 0a20 2020 2020 2020 2020  fixed:.         
-0001db20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001db30: 6672 6565 5061 724e 616d 732e 6170 7065  freeParNams.appe
-0001db40: 6e64 2873 656c 662e 706e 616d 735b 695d  nd(self.pnams[i]
-0001db50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001db60: 2020 6966 2066 6978 6564 3a0a 2020 2020    if fixed:.    
-0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db80: 7365 6c66 2e66 6978 6564 5061 724e 616d  self.fixedParNam
-0001db90: 732e 6170 7065 6e64 2873 656c 662e 706e  s.append(self.pn
-0001dba0: 616d 735b 695d 290a 2020 2020 2020 2020  ams[i]).        
-0001dbb0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001dbc0: 2020 7365 6c66 2e66 7265 6550 6172 4e61    self.freeParNa
-0001dbd0: 6d73 203d 2073 656c 662e 706e 616d 730a  ms = self.pnams.
-0001dbe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001dbf0: 2e66 6978 6564 5061 724e 616d 7320 3d20  .fixedParNams = 
-0001dc00: 5b5d 0a0a 2020 2020 6465 6620 5f73 6574  []..    def _set
-0001dc10: 7570 4d69 6e75 6974 2873 656c 662c 206d  upMinuit(self, m
-0001dc20: 6f64 656c 5f6b 7761 7267 7329 3a0a 2020  odel_kwargs):.  
-0001dc30: 2020 2020 2020 2222 2263 7265 6174 6520        """create 
-0001dc40: 4d69 6e75 6974 206f 626a 6563 7420 2864  Minuit object (d
-0001dc50: 6570 656e 6473 206f 6e20 4d69 6e75 6974  epends on Minuit
-0001dc60: 2076 6572 7369 6f6e 2922 2222 0a20 2020   version)""".   
-0001dc70: 2020 2020 2069 6620 7365 6c66 2e69 6d69       if self.imi
-0001dc80: 6e75 6974 5f76 6572 7369 6f6e 203c 2022  nuit_version < "
-0001dc90: 3222 3a0a 2020 2020 2020 2020 2020 2020  2":.            
-0001dca0: 6966 2073 656c 662e 7175 6965 743a 0a20  if self.quiet:. 
-0001dcb0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001dcc0: 7269 6e74 5f6c 6576 656c 203d 2030 0a20  rint_level = 0. 
-0001dcd0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001dce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001dcf0: 2070 7269 6e74 5f6c 6576 656c 203d 2031   print_level = 1
-0001dd00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001dd10: 7365 6c66 2e64 7030 2069 7320 6e6f 7420  self.dp0 is not 
-0001dd20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001dd30: 2020 2020 2020 666f 7220 692c 2070 6e61        for i, pna
-0001dd40: 6d20 696e 2065 6e75 6d65 7261 7465 2873  m in enumerate(s
-0001dd50: 656c 662e 706e 616d 7329 3a0a 2020 2020  elf.pnams):.    
-0001dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd70: 6d6f 6465 6c5f 6b77 6172 6773 5b22 6572  model_kwargs["er
-0001dd80: 726f 725f 2220 2b20 706e 616d 5d20 3d20  ror_" + pnam] = 
-0001dd90: 7365 6c66 2e64 7030 5b69 5d0a 2020 2020  self.dp0[i].    
-0001dda0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001ddb0: 7365 744c 696d 6974 7320 6973 206e 6f74  setLimits is not
-0001ddc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001ddd0: 2020 2020 2020 2066 6f72 2069 2c20 706e         for i, pn
-0001dde0: 616d 2069 6e20 656e 756d 6572 6174 6528  am in enumerate(
-0001ddf0: 7365 6c66 2e70 6e61 6d73 293a 0a20 2020  self.pnams):.   
-0001de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de10: 206d 6f64 656c 5f6b 7761 7267 735b 226c   model_kwargs["l
-0001de20: 696d 6974 5f22 202b 2070 6e61 6d5d 203d  imit_" + pnam] =
-0001de30: 2073 656c 662e 6c69 6d69 7473 5b69 5d0a   self.limits[i].
-0001de40: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001de50: 656c 662e 6669 7850 6172 7320 6973 206e  elf.fixPars is n
-0001de60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0001de70: 2020 2020 2020 2020 2066 6f72 2069 2c20           for i, 
-0001de80: 706e 616d 2069 6e20 656e 756d 6572 6174  pnam in enumerat
-0001de90: 6528 7365 6c66 2e70 6e61 6d73 293a 0a20  e(self.pnams):. 
-0001dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001deb0: 2020 206d 6f64 656c 5f6b 7761 7267 735b     model_kwargs[
-0001dec0: 2266 6978 5f22 202b 2070 6e61 6d5d 203d  "fix_" + pnam] =
-0001ded0: 2073 656c 662e 6669 7865 6450 6172 735b   self.fixedPars[
-0001dee0: 695d 0a20 2020 2020 2020 2020 2020 2073  i].            s
-0001def0: 656c 662e 6d69 6e75 6974 203d 204d 696e  elf.minuit = Min
-0001df00: 7569 7428 0a20 2020 2020 2020 2020 2020  uit(.           
-0001df10: 2020 2020 2073 656c 662e 636f 7374 662c       self.costf,
-0001df20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001df30: 2065 7272 6f72 6465 663d 7365 6c66 2e45   errordef=self.E
-0001df40: 7272 4465 662c 0a20 2020 2020 2020 2020  rrDef,.         
-0001df50: 2020 2020 2020 2070 7269 6e74 5f6c 6576         print_lev
-0001df60: 656c 3d70 7269 6e74 5f6c 6576 656c 2c0a  el=print_level,.
-0001df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df80: 2a2a 6d6f 6465 6c5f 6b77 6172 6773 2c0a  **model_kwargs,.
-0001df90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0001dfa0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001dfb0: 2020 2020 2020 2020 7365 6c66 2e6d 696e          self.min
-0001dfc0: 7569 7420 3d20 4d69 6e75 6974 2873 656c  uit = Minuit(sel
-0001dfd0: 662e 636f 7374 662c 202a 6d6f 6465 6c5f  f.costf, *model_
-0001dfe0: 6b77 6172 6773 2e76 616c 7565 7328 292c  kwargs.values(),
-0001dff0: 206e 616d 653d 7365 6c66 2e70 6e61 6d73   name=self.pnams
-0001e000: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0001e010: 6c66 2e6d 696e 7569 742e 6572 726f 7264  lf.minuit.errord
-0001e020: 6566 203d 2073 656c 662e 4572 7244 6566  ef = self.ErrDef
-0001e030: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001e040: 7365 6c66 2e71 7569 6574 3a0a 2020 2020  self.quiet:.    
-0001e050: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001e060: 2e6d 696e 7569 742e 7072 696e 745f 6c65  .minuit.print_le
-0001e070: 7665 6c20 3d20 300a 2020 2020 2020 2020  vel = 0.        
-0001e080: 2020 2020 6966 2073 656c 662e 6470 3020      if self.dp0 
-0001e090: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0001e0a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001e0b0: 662e 6d69 6e75 6974 2e65 7272 6f72 7320  f.minuit.errors 
-0001e0c0: 3d20 7365 6c66 2e64 7030 0a20 2020 2020  = self.dp0.     
-0001e0d0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0001e0e0: 6574 4c69 6d69 7473 2069 7320 6e6f 7420  etLimits is not 
-0001e0f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001e100: 2020 2020 2020 7365 6c66 2e6d 696e 7569        self.minui
-0001e110: 742e 6c69 6d69 7473 203d 2073 656c 662e  t.limits = self.
-0001e120: 6c69 6d69 7473 0a20 2020 2020 2020 2020  limits.         
-0001e130: 2020 2069 6620 7365 6c66 2e66 6978 5061     if self.fixPa
-0001e140: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-0001e150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e160: 666f 7220 692c 2070 6e61 6d20 696e 2065  for i, pnam in e
-0001e170: 6e75 6d65 7261 7465 2873 656c 662e 706e  numerate(self.pn
-0001e180: 616d 7329 3a0a 2020 2020 2020 2020 2020  ams):.          
-0001e190: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-0001e1a0: 662e 6669 7865 6450 6172 735b 695d 3a0a  f.fixedPars[i]:.
-0001e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1c0: 2020 2020 2020 2020 7365 6c66 2e6d 696e          self.min
-0001e1d0: 7569 742e 6669 7865 645b 706e 616d 5d20  uit.fixed[pnam] 
-0001e1e0: 3d20 5472 7565 0a0a 2020 2020 6465 6620  = True..    def 
-0001e1f0: 5f73 746f 7265 5265 7375 6c74 2873 656c  _storeResult(sel
-0001e200: 6629 3a0a 2020 2020 2020 2020 2320 636f  f):.        # co
-0001e210: 6c6c 6563 7420 7265 7375 6c74 7320 6173  llect results as
-0001e220: 206e 756d 7079 2061 7272 6179 730a 2020   numpy arrays.  
-0001e230: 2020 2020 2020 2320 2121 2120 7468 6973        # !!! this
-0001e240: 2070 6172 7420 6465 7065 6e64 7320 6f6e   part depends on
-0001e250: 2069 6d69 6e75 6974 2076 6572 7369 6f6e   iminuit version
-0001e260: 2021 2121 0a20 2020 2020 2020 206d 203d   !!!.        m =
-0001e270: 2073 656c 662e 6d69 6e75 6974 0a20 2020   self.minuit.   
-0001e280: 2020 2020 206d 696e 436f 7374 203d 206d       minCost = m
-0001e290: 2e66 7661 6c20 2023 206d 696e 696d 756d  .fval  # minimum
-0001e2a0: 2076 616c 7565 206f 6620 636f 7374 2066   value of cost f
-0001e2b0: 756e 6374 696f 6e0a 2020 2020 2020 2020  unction.        
-0001e2c0: 6e66 7061 7220 3d20 6d2e 6e66 6974 2020  nfpar = m.nfit  
-0001e2d0: 2320 6e75 6d65 7220 6f66 2066 7265 6520  # numer of free 
-0001e2e0: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
-0001e2f0: 2020 206e 646f 6620 3d20 7365 6c66 2e63     ndof = self.c
-0001e300: 6f73 7466 2e6e 646f 6620 2023 2064 6567  ostf.ndof  # deg
-0001e310: 7265 6573 206f 6620 6672 6565 646f 6d0a  rees of freedom.
-0001e320: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0001e330: 696d 696e 7569 745f 7665 7273 696f 6e20  iminuit_version 
-0001e340: 3c20 2232 223a 0a20 2020 2020 2020 2020  < "2":.         
-0001e350: 2020 2070 6172 6e61 6d65 7320 3d20 6d2e     parnames = m.
-0001e360: 7661 6c75 6573 2e6b 6579 7328 2920 2023  values.keys()  #
-0001e370: 2070 6172 616d 6574 6572 206e 616d 6573   parameter names
-0001e380: 0a20 2020 2020 2020 2020 2020 2070 6172  .            par
-0001e390: 7661 6c73 203d 206e 702e 6173 6172 7261  vals = np.asarra
-0001e3a0: 7928 6d2e 7661 6c75 6573 2e76 616c 7565  y(m.values.value
-0001e3b0: 7328 2929 2020 2320 6265 7374 2d66 6974  s())  # best-fit
-0001e3c0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-0001e3d0: 2020 2020 7061 7265 7272 7320 3d20 6e70      parerrs = np
-0001e3e0: 2e61 7361 7272 6179 286d 2e65 7272 6f72  .asarray(m.error
-0001e3f0: 732e 7661 6c75 6573 2829 2920 2023 2070  s.values())  # p
-0001e400: 6172 616d 6574 6572 2075 6e63 6572 7461  arameter uncerta
-0001e410: 696e 7469 6573 0a20 2020 2020 2020 2020  inties.         
-0001e420: 2020 2063 6f76 203d 206e 702e 6172 7261     cov = np.arra
-0001e430: 7928 6d2e 6d61 7472 6978 2829 2920 2023  y(m.matrix())  #
-0001e440: 2063 6f76 2e20 6d61 7472 6978 206f 6620   cov. matrix of 
-0001e450: 6672 6565 2070 6172 616d 6574 6572 730a  free parameters.
-0001e460: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001e470: 2020 2020 2020 2020 2020 2320 7665 7273            # vers
-0001e480: 2e20 3e3d 322e 300a 2020 2020 2020 2020  . >=2.0.        
-0001e490: 2020 2020 7061 726e 616d 6573 203d 206d      parnames = m
-0001e4a0: 2e70 6172 616d 6574 6572 7320 2023 2070  .parameters  # p
-0001e4b0: 6172 616d 6574 6572 206e 616d 6573 0a20  arameter names. 
-0001e4c0: 2020 2020 2020 2020 2020 2070 6172 7661             parva
-0001e4d0: 6c73 203d 206e 702e 6173 6172 7261 7928  ls = np.asarray(
-0001e4e0: 6d2e 7661 6c75 6573 2920 2023 2062 6573  m.values)  # bes
-0001e4f0: 742d 6669 7420 7661 6c75 6573 0a20 2020  t-fit values.   
-0001e500: 2020 2020 2020 2020 2070 6172 6572 7273           parerrs
-0001e510: 203d 206e 702e 6173 6172 7261 7928 6d2e   = np.asarray(m.
-0001e520: 6572 726f 7273 2920 2023 2070 6172 616d  errors)  # param
-0001e530: 6574 6572 2075 6e63 6572 7461 696e 7469  eter uncertainti
-0001e540: 6573 0a20 2020 2020 2020 2020 2020 2063  es.            c
-0001e550: 6f76 203d 206e 702e 6173 6172 7261 7928  ov = np.asarray(
-0001e560: 6d2e 636f 7661 7269 616e 6365 2920 2023  m.covariance)  #
-0001e570: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-0001e580: 6978 206f 6620 616c 6c28 2129 2070 6172  ix of all(!) par
-0001e590: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0001e5a0: 2020 2020 2320 7072 6f64 7563 6520 7265      # produce re
-0001e5b0: 6475 6365 6420 636f 7661 7269 616e 6365  duced covariance
-0001e5c0: 206d 6174 7269 7820 666f 7220 6672 6565   matrix for free
-0001e5d0: 2070 6172 616d 6574 6572 7320 6f6e 6c79   parameters only
-0001e5e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001e5f0: 7365 6c66 2e6e 6669 7865 6420 213d 2030  self.nfixed != 0
-0001e600: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e610: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0001e620: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001e630: 2020 2020 2020 6c65 6e28 7061 726e 616d        len(parnam
-0001e640: 6573 2920 2d20 312c 202d 312c 202d 310a  es) - 1, -1, -1.
-0001e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e660: 293a 2020 2320 7374 6172 7420 6672 6f6d  ):  # start from
-0001e670: 206c 6172 6765 7374 2069 6e64 6578 2061   largest index a
-0001e680: 6e64 2077 6f72 6b20 6261 636b 0a20 2020  nd work back.   
-0001e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e6a0: 2069 6620 7365 6c66 2e66 6978 6564 5061   if self.fixedPa
-0001e6b0: 7273 5b69 5d3a 0a20 2020 2020 2020 2020  rs[i]:.         
-0001e6c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001e6d0: 6f76 203d 206e 702e 6465 6c65 7465 286e  ov = np.delete(n
-0001e6e0: 702e 6465 6c65 7465 2863 6f76 2c20 692c  p.delete(cov, i,
-0001e6f0: 2030 292c 2069 2c20 3129 0a20 2020 2020   0), i, 1).     
-0001e700: 2020 206e 7061 7220 3d20 6c65 6e28 7061     npar = len(pa
-0001e710: 726e 616d 6573 2920 2023 206e 756d 6265  rnames)  # numbe
-0001e720: 7220 6f66 2070 6172 616d 6574 6572 730a  r of parameters.
-0001e730: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0001e740: 2e6d 696e 6f73 5265 7375 6c74 2069 7320  .minosResult is 
-0001e750: 6e6f 7420 4e6f 6e65 2061 6e64 2073 656c  not None and sel
-0001e760: 662e 6d69 6e6f 735f 6f6b 3a0a 2020 2020  f.minos_ok:.    
-0001e770: 2020 2020 2020 2020 706d 6572 7273 203d          pmerrs =
-0001e780: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-0001e790: 2320 2070 7269 6e74 2822 4d49 4e4f 5320  #  print("MINOS 
-0001e7a0: 6572 726f 7273 3a22 290a 2020 2020 2020  errors:").      
-0001e7b0: 2020 2020 2020 6966 2073 656c 662e 696d        if self.im
-0001e7c0: 696e 7569 745f 7665 7273 696f 6e20 3c20  inuit_version < 
-0001e7d0: 2232 223a 0a20 2020 2020 2020 2020 2020  "2":.           
-0001e7e0: 2020 2020 2066 6f72 2070 6e61 6d20 696e       for pnam in
-0001e7f0: 206d 2e6d 6572 726f 7273 2e6b 6579 7328   m.merrors.keys(
-0001e800: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001e810: 2020 2020 2020 2070 6d65 7272 732e 6170         pmerrs.ap
-0001e820: 7065 6e64 285b 6d2e 6d65 7272 6f72 735b  pend([m.merrors[
-0001e830: 706e 616d 5d5b 325d 2c20 6d2e 6d65 7272  pnam][2], m.merr
-0001e840: 6f72 735b 706e 616d 5d5b 335d 5d29 0a20  ors[pnam][3]]). 
-0001e850: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001e860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e870: 2066 6f72 2070 6e61 6d20 696e 206d 2e6d   for pnam in m.m
-0001e880: 6572 726f 7273 2e6b 6579 7328 293a 0a20  errors.keys():. 
-0001e890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8a0: 2020 2070 6d65 7272 732e 6170 7065 6e64     pmerrs.append
-0001e8b0: 285b 6d2e 6d65 7272 6f72 735b 706e 616d  ([m.merrors[pnam
-0001e8c0: 5d2e 6c6f 7765 722c 206d 2e6d 6572 726f  ].lower, m.merro
-0001e8d0: 7273 5b70 6e61 6d5d 2e75 7070 6572 5d29  rs[pnam].upper])
-0001e8e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001e8f0: 662e 4f6e 6553 6967 496e 7465 7276 616c  f.OneSigInterval
-0001e900: 203d 206e 702e 6172 7261 7928 706d 6572   = np.array(pmer
-0001e910: 7273 290a 2020 2020 2020 2020 656c 7365  rs).        else
-0001e920: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0001e930: 6c66 2e4f 6e65 5369 6749 6e74 6572 7661  lf.OneSigInterva
-0001e940: 6c20 3d20 6e70 2e61 7272 6179 286c 6973  l = np.array(lis
-0001e950: 7428 7a69 7028 2d70 6172 6572 7273 2c20  t(zip(-parerrs, 
-0001e960: 7061 7265 7272 7329 2929 0a0a 2020 2020  parerrs)))..    
-0001e970: 2020 2020 2320 6669 6e61 6c20 6361 6c6c      # final call
-0001e980: 206f 6620 636f 7374 2066 756e 6374 696f   of cost functio
-0001e990: 6e20 6174 206d 696d 696e 756d 2074 6f20  n at miminum to 
-0001e9a0: 7570 6461 7465 2061 6c6c 2072 6573 756c  update all resul
-0001e9b0: 7473 0a20 2020 2020 2020 2023 202d 2020  ts.        # -  
-0001e9c0: 7369 676e 616c 7320 6461 7461 206f 626a  signals data obj
-0001e9d0: 6563 7420 746f 2073 746f 7265 206d 6f64  ect to store mod
-0001e9e0: 656c 2d64 656e 6465 6e74 2075 6e63 6572  el-dendent uncer
-0001e9f0: 7461 696e 7469 6573 0a20 2020 2020 2020  tainties.       
-0001ea00: 2069 6620 7365 6c66 2e64 6174 6120 6973   if self.data is
-0001ea10: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0001ea20: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-0001ea30: 2e66 696e 616c 5f63 616c 6c20 3d20 5472  .final_call = Tr
-0001ea40: 7565 0a20 2020 2020 2020 2023 202d 2020  ue.        # -  
-0001ea50: 616e 6420 636f 7374 2066 756e 6374 696f  and cost functio
-0001ea60: 6e20 746f 2073 746f 7265 2067 6f6f 646e  n to store goodn
-0001ea70: 6573 732d 6f66 2d66 6974 0a20 2020 2020  ess-of-fit.     
-0001ea80: 2020 2073 656c 662e 636f 7374 662e 6669     self.costf.fi
-0001ea90: 6e61 6c5f 6361 6c6c 203d 2054 7275 650a  nal_call = True.
-0001eaa0: 2020 2020 2020 2020 6676 616c 203d 2073          fval = s
-0001eab0: 656c 662e 636f 7374 6628 2a70 6172 7661  elf.costf(*parva
-0001eac0: 6c73 290a 0a20 2020 2020 2020 2023 2073  ls)..        # s
-0001ead0: 746f 7265 2072 6573 756c 7473 2061 7320  tore results as 
-0001eae0: 636c 6173 7320 6d65 6d62 6572 730a 2020  class members.  
-0001eaf0: 2020 2020 2020 2320 2020 7061 7261 6d65        #   parame
-0001eb00: 7465 7220 6e61 6d65 730a 2020 2020 2020  ter names.      
-0001eb10: 2020 7365 6c66 2e50 6172 616d 6574 6572    self.Parameter
-0001eb20: 4e61 6d65 7320 3d20 7061 726e 616d 6573  Names = parnames
-0001eb30: 0a20 2020 2020 2020 2023 202a 2066 6c61  .        # * fla
-0001eb40: 6720 666f 7220 6669 7865 6420 7061 7261  g for fixed para
-0001eb50: 6d65 7465 7273 2069 6e20 7365 6c66 2e66  meters in self.f
-0001eb60: 6978 6564 5061 7273 0a20 2020 2020 2020  ixedPars.       
-0001eb70: 2023 202a 206e 616d 6573 206f 6620 6672   # * names of fr
-0001eb80: 6565 2070 6172 616d 6574 6572 7320 696e  ee parameters in
-0001eb90: 2073 656c 662e 6672 6565 5061 724e 616d   self.freeParNam
-0001eba0: 730a 2020 2020 2020 2020 2320 2020 6368  s.        #   ch
-0001ebb0: 6932 2061 7420 6265 7374 2d66 6974 2070  i2 at best-fit p
-0001ebc0: 6f69 6e74 2028 706f 7373 6962 6c79 2064  oint (possibly d
-0001ebd0: 6966 6665 7265 6e74 2066 726f 6d20 6d69  ifferent from mi
-0001ebe0: 6e43 6f73 7429 0a20 2020 2020 2020 2073  nCost).        s
-0001ebf0: 656c 662e 476f 4620 3d20 7365 6c66 2e63  elf.GoF = self.c
-0001ec00: 6f73 7466 2e67 6f66 0a20 2020 2020 2020  ostf.gof.       
-0001ec10: 2023 2020 2070 6172 616d 6574 6572 2076   #   parameter v
-0001ec20: 616c 7565 7320 6174 2062 6573 742d 6669  alues at best-fi
-0001ec30: 7420 706f 696e 740a 2020 2020 2020 2020  t point.        
-0001ec40: 7365 6c66 2e50 6172 616d 6574 6572 5661  self.ParameterVa
-0001ec50: 6c75 6573 203d 206e 702e 6172 7261 7928  lues = np.array(
-0001ec60: 7061 7276 616c 732c 2063 6f70 793d 5472  parvals, copy=Tr
-0001ec70: 7565 290a 2020 2020 2020 2020 7365 6c66  ue).        self
-0001ec80: 2e66 7265 6550 6172 5661 6c73 203d 206e  .freeParVals = n
-0001ec90: 702e 6172 7261 7928 0a20 2020 2020 2020  p.array(.       
-0001eca0: 2020 2020 205b 7061 7276 616c 735b 695d       [parvals[i]
-0001ecb0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-0001ecc0: 6e70 6172 2920 6966 206e 6f74 2073 656c  npar) if not sel
-0001ecd0: 662e 6669 7865 6450 6172 735b 695d 5d0a  f.fixedPars[i]].
-0001ece0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001ecf0: 2020 7365 6c66 2e66 7265 6550 6172 4572    self.freeParEr
-0001ed00: 7273 203d 206e 702e 6172 7261 7928 0a20  rs = np.array(. 
-0001ed10: 2020 2020 2020 2020 2020 205b 7061 7265             [pare
-0001ed20: 7272 735b 695d 2066 6f72 2069 2069 6e20  rrs[i] for i in 
-0001ed30: 7261 6e67 6528 6e70 6172 2920 6966 206e  range(npar) if n
-0001ed40: 6f74 2073 656c 662e 6669 7865 6450 6172  ot self.fixedPar
-0001ed50: 735b 695d 5d0a 2020 2020 2020 2020 290a  s[i]].        ).
-0001ed60: 2020 2020 2020 2020 2320 6669 7865 6420          # fixed 
-0001ed70: 7061 7261 6d65 7465 7220 6e61 6d65 7320  parameter names 
-0001ed80: 616e 6420 7661 6c75 6573 0a20 2020 2020  and values.     
-0001ed90: 2020 2073 656c 662e 6669 7865 6450 6172     self.fixedPar
-0001eda0: 5661 6c73 203d 206e 702e 6172 7261 7928  Vals = np.array(
-0001edb0: 0a20 2020 2020 2020 2020 2020 205b 7061  .            [pa
-0001edc0: 7276 616c 735b 695d 2066 6f72 2069 2069  rvals[i] for i i
-0001edd0: 6e20 7261 6e67 6528 6e70 6172 2920 6966  n range(npar) if
-0001ede0: 2073 656c 662e 6669 7865 6450 6172 735b   self.fixedPars[
-0001edf0: 695d 5d0a 2020 2020 2020 2020 290a 2020  i]].        ).  
-0001ee00: 2020 2020 2020 2320 2a20 6e61 6d65 7320        # * names 
-0001ee10: 6f66 2066 6978 6564 2070 6172 616d 6574  of fixed paramet
-0001ee20: 6572 7320 696e 2073 656c 662e 6669 7865  ers in self.fixe
-0001ee30: 6450 6172 4e61 6d73 0a20 2020 2020 2020  dParNams.       
-0001ee40: 2023 2020 206e 756d 6265 7220 6f66 2064   #   number of d
-0001ee50: 6567 7265 6573 206f 6620 6672 6565 646f  egrees of freedo
-0001ee60: 6d0a 2020 2020 2020 2020 7365 6c66 2e4e  m.        self.N
-0001ee70: 446f 4620 3d20 6e64 6f66 0a20 2020 2020  DoF = ndof.     
-0001ee80: 2020 2023 2020 2073 796d 6d65 7472 6963     #   symmetric
-0001ee90: 2075 6e63 6572 7461 696e 7469 6573 0a20   uncertainties. 
-0001eea0: 2020 2020 2020 2073 656c 662e 4d69 6772         self.Migr
-0001eeb0: 6164 4572 726f 7273 203d 206e 702e 6172  adErrors = np.ar
-0001eec0: 7261 7928 7061 7265 7272 732c 2063 6f70  ray(parerrs, cop
-0001eed0: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
-0001eee0: 2320 2020 636f 7661 7269 616e 6365 2061  #   covariance a
-0001eef0: 6e64 2063 6f72 7265 6c61 7469 6f6e 206d  nd correlation m
-0001ef00: 6174 7269 6365 730a 2020 2020 2020 2020  atrices.        
-0001ef10: 7365 6c66 2e43 6f76 6172 6961 6e63 654d  self.CovarianceM
-0001ef20: 6174 7269 7820 3d20 6e70 2e61 7272 6179  atrix = np.array
-0001ef30: 2863 6f76 2c20 636f 7079 3d54 7275 6529  (cov, copy=True)
-0001ef40: 0a20 2020 2020 2020 2070 6572 7273 203d  .        perrs =
-0001ef50: 206e 702e 7371 7274 286e 702e 6469 6167   np.sqrt(np.diag
-0001ef60: 6f6e 616c 2863 6f76 2929 0a20 2020 2020  onal(cov)).     
-0001ef70: 2020 2073 656c 662e 436f 7272 656c 6174     self.Correlat
-0001ef80: 696f 6e4d 6174 7269 7820 3d20 636f 7620  ionMatrix = cov 
-0001ef90: 2f20 6e70 2e6f 7574 6572 2870 6572 7273  / np.outer(perrs
-0001efa0: 2c20 7065 7272 7329 0a20 2020 2020 2020  , perrs).       
-0001efb0: 2023 2020 2031 2d73 6967 6d61 2028 3638   #   1-sigma (68
-0001efc0: 2520 434c 2920 7261 6e67 6520 696e 2073  % CL) range in s
-0001efd0: 656c 662e 4f6e 6553 6967 496e 7465 7276  elf.OneSigInterv
-0001efe0: 616c 0a0a 2020 2020 2020 2020 2320 6275  al..        # bu
-0001eff0: 696c 6420 6120 636f 6e76 656e 6965 6e74  ild a convenient
-0001f000: 2072 6573 756c 7420 6469 6374 696f 6e61   result dictiona
-0001f010: 7279 0a20 2020 2020 2020 2069 6620 7365  ry.        if se
-0001f020: 6c66 2e6e 6669 7865 6420 3d3d 2030 3a0a  lf.nfixed == 0:.
-0001f030: 2020 2020 2020 2020 2020 2020 7274 7570              rtup
-0001f040: 6c65 203d 2028 0a20 2020 2020 2020 2020  le = (.         
-0001f050: 2020 2020 2020 2073 656c 662e 5061 7261         self.Para
-0001f060: 6d65 7465 7256 616c 7565 732c 0a20 2020  meterValues,.   
-0001f070: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001f080: 662e 4f6e 6553 6967 496e 7465 7276 616c  f.OneSigInterval
-0001f090: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001f0a0: 2020 7365 6c66 2e43 6f72 7265 6c61 7469    self.Correlati
-0001f0b0: 6f6e 4d61 7472 6978 2c0a 2020 2020 2020  onMatrix,.      
-0001f0c0: 2020 2020 2020 2020 2020 7365 6c66 2e47            self.G
-0001f0d0: 6f46 2c0a 2020 2020 2020 2020 2020 2020  oF,.            
-0001f0e0: 2020 2020 7365 6c66 2e50 6172 616d 6574      self.Paramet
-0001f0f0: 6572 4e61 6d65 732c 0a20 2020 2020 2020  erNames,.       
-0001f100: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-0001f110: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001f120: 2072 7475 706c 6520 3d20 280a 2020 2020   rtuple = (.    
-0001f130: 2020 2020 2020 2020 2020 2020 6e70 2e63              np.c
-0001f140: 6f6e 6361 7465 6e61 7465 2828 7365 6c66  oncatenate((self
-0001f150: 2e66 7265 6550 6172 5661 6c73 2c20 7365  .freeParVals, se
-0001f160: 6c66 2e66 6978 6564 5061 7256 616c 7329  lf.fixedParVals)
-0001f170: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0001f180: 2020 2073 656c 662e 4f6e 6553 6967 496e     self.OneSigIn
-0001f190: 7465 7276 616c 2c0a 2020 2020 2020 2020  terval,.        
-0001f1a0: 2020 2020 2020 2020 7365 6c66 2e43 6f72          self.Cor
-0001f1b0: 7265 6c61 7469 6f6e 4d61 7472 6978 2c0a  relationMatrix,.
-0001f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f1d0: 7365 6c66 2e47 6f46 2c0a 2020 2020 2020  self.GoF,.      
-0001f1e0: 2020 2020 2020 2020 2020 6e70 2e63 6f6e            np.con
-0001f1f0: 6361 7465 6e61 7465 2828 7365 6c66 2e66  catenate((self.f
-0001f200: 7265 6550 6172 4e61 6d73 2c20 7365 6c66  reeParNams, self
-0001f210: 2e66 6978 6564 5061 724e 616d 7329 292c  .fixedParNams)),
-0001f220: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0001f230: 2020 2020 2020 206b 6579 7320 3d20 280a         keys = (.
-0001f240: 2020 2020 2020 2020 2020 2020 2270 6172              "par
-0001f250: 616d 6574 6572 2076 616c 7565 7322 2c0a  ameter values",.
-0001f260: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-0001f270: 6669 6465 6e63 6520 696e 7465 7276 616c  fidence interval
-0001f280: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-0001f290: 2263 6f72 7265 6c61 7469 6f6e 206d 6174  "correlation mat
-0001f2a0: 7269 7822 2c0a 2020 2020 2020 2020 2020  rix",.          
-0001f2b0: 2020 2267 6f6f 646e 6573 732d 6f66 2d66    "goodness-of-f
-0001f2c0: 6974 222c 0a20 2020 2020 2020 2020 2020  it",.           
-0001f2d0: 2022 7061 7261 6d65 7465 7220 6e61 6d65   "parameter name
-0001f2e0: 7322 2c0a 2020 2020 2020 2020 290a 2020  s",.        ).  
-0001f2f0: 2020 2020 2020 2320 6275 696c 6420 6469        # build di
-0001f300: 6374 696f 6e61 7279 0a20 2020 2020 2020  ctionary.       
-0001f310: 2073 656c 662e 5265 7375 6c74 4469 6374   self.ResultDict
-0001f320: 696f 6e61 7279 203d 207b 6b3a 2072 7475  ionary = {k: rtu
-0001f330: 706c 655b 695d 2066 6f72 2028 692c 206b  ple[i] for (i, k
-0001f340: 2920 696e 2065 6e75 6d65 7261 7465 286b  ) in enumerate(k
-0001f350: 6579 7329 7d0a 0a20 2020 2064 6566 2067  eys)}..    def g
-0001f360: 6574 5265 7375 6c74 2873 656c 6629 3a0a  etResult(self):.
-0001f370: 2020 2020 2020 2020 2222 2272 6574 7572          """retur
-0001f380: 6e20 7265 7375 6c74 2064 6963 7469 6f6e  n result diction
-0001f390: 6172 7922 2222 0a20 2020 2020 2020 2069  ary""".        i
-0001f3a0: 6620 7365 6c66 2e52 6573 756c 7444 6963  f self.ResultDic
-0001f3b0: 7469 6f6e 6172 7920 6973 206e 6f74 204e  tionary is not N
-0001f3c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0001f3d0: 2072 6574 7572 6e20 7365 6c66 2e52 6573   return self.Res
-0001f3e0: 756c 7444 6963 7469 6f6e 6172 790a 2020  ultDictionary.  
-0001f3f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0001f400: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
-0001f410: 6e74 696d 6545 7272 6f72 280a 2020 2020  ntimeError(.    
-0001f420: 2020 2020 2020 2020 2020 2020 2220 2121              " !!
-0001f430: 2120 6d6e 4669 742e 6765 7452 6573 756c  ! mnFit.getResul
-0001f440: 743a 206e 6f20 7265 7375 6c74 7320 6176  t: no results av
-0001f450: 6169 6c61 626c 6520 2d20 7275 6e20 6669  ailable - run fi
-0001f460: 7420 6669 7273 7422 0a20 2020 2020 2020  t first".       
-0001f470: 2020 2020 2029 0a0a 2020 2020 4073 7461       )..    @sta
-0001f480: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-0001f490: 6620 6765 7446 756e 6374 696f 6e45 7272  f getFunctionErr
-0001f4a0: 6f72 2878 2c20 6d6f 6465 6c2c 2070 7661  or(x, model, pva
-0001f4b0: 6c73 2c20 636f 7670 2c20 6669 7865 6450  ls, covp, fixedP
-0001f4c0: 6172 7329 3a0a 2020 2020 2020 2020 2222  ars):.        ""
-0001f4d0: 2264 6574 6572 6d69 6e65 2065 7272 6f72  "determine error
-0001f4e0: 206f 6620 6d6f 6465 6c20 6174 2078 0a0a   of model at x..
-0001f4f0: 2020 2020 2020 2020 466f 726d 756c 613a          Formula:
-0001f500: 0a20 2020 2020 2020 2020 2044 656c 7461  .          Delta
-0001f510: 2878 2920 3d20 7371 7274 2820 7375 6d5f  (x) = sqrt( sum_
-0001f520: 692c 6a20 2864 662f 6470 5f69 2878 2920  i,j (df/dp_i(x) 
-0001f530: 6466 2f64 705f 6a28 7829 2056 705f 692c  df/dp_j(x) Vp_i,
-0001f540: 6a29 2029 0a0a 2020 2020 2020 2020 4172  j) )..        Ar
-0001f550: 6773 3a0a 2020 2020 2020 2020 2020 2a20  gs:.          * 
-0001f560: 783a 2073 6361 6c61 7220 6f72 206e 702d  x: scalar or np-
-0001f570: 6172 7261 7920 6f66 2078 2076 616c 7565  array of x value
-0001f580: 730a 2020 2020 2020 2020 2020 2a20 6d6f  s.          * mo
-0001f590: 6465 6c3a 206d 6f64 656c 2066 756e 6374  del: model funct
-0001f5a0: 696f 6e0a 2020 2020 2020 2020 2020 2a20  ion.          * 
-0001f5b0: 7076 6c61 733a 2070 6172 616d 6574 6572  pvlas: parameter
-0001f5c0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
-0001f5d0: 2020 2a20 636f 7670 3a20 636f 7661 7269    * covp: covari
-0001f5e0: 616e 6365 206d 6174 7269 7820 6f66 2070  ance matrix of p
-0001f5f0: 6172 616d 6574 6572 730a 0a20 2020 2020  arameters..     
-0001f600: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0001f610: 2020 2020 2020 2a20 6d6f 6465 6c20 756e        * model un
-0001f620: 6365 7274 6169 6e74 792c 2073 616d 6520  certainty, same 
-0001f630: 6c65 6e67 7468 2061 7320 780a 2020 2020  length as x.    
-0001f640: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0001f650: 2023 2063 616c 6375 6c61 7465 2070 6172   # calculate par
-0001f660: 7469 616c 2064 6572 6976 6174 6976 6573  tial derivatives
-0001f670: 206f 6620 6d6f 6465 6c20 772e 722e 7420   of model w.r.t 
-0001f680: 7061 7261 6d65 7465 7273 0a0a 2020 2020  parameters..    
-0001f690: 2020 2020 2320 2020 7061 7261 6d65 7465      #   paramete
-0001f6a0: 7220 7374 6570 2073 697a 650a 2020 2020  r step size.    
-0001f6b0: 2020 2020 6470 203d 2030 2e30 3120 2a20      dp = 0.01 * 
-0001f6c0: 6e70 2e73 7172 7428 6e70 2e64 6961 676f  np.sqrt(np.diago
-0001f6d0: 6e61 6c28 636f 7670 2929 0a20 2020 2020  nal(covp)).     
-0001f6e0: 2020 2023 206e 756d 6265 7220 6f66 2076     # number of v
-0001f6f0: 6172 6961 626c 6520 7061 7261 6d65 7465  ariable paramete
-0001f700: 7273 0a20 2020 2020 2020 206e 7670 6172  rs.        nvpar
-0001f710: 203d 206c 656e 2864 7029 0a20 2020 2020   = len(dp).     
-0001f720: 2020 2023 2020 2064 6572 6976 6174 6976     #   derivativ
-0001f730: 6520 6466 2f64 705f 6a20 6174 2065 6163  e df/dp_j at eac
-0001f740: 6820 785f 690a 2020 2020 2020 2020 6466  h x_i.        df
-0001f750: 6470 203d 206e 702e 656d 7074 7928 286e  dp = np.empty((n
-0001f760: 7670 6172 2c20 6c65 6e28 7829 2929 0a20  vpar, len(x))). 
-0001f770: 2020 2020 2020 2070 5f70 6c75 7320 3d20         p_plus = 
-0001f780: 6e70 2e61 7272 6179 2870 7661 6c73 2c20  np.array(pvals, 
-0001f790: 636f 7079 3d54 7275 6529 0a20 2020 2020  copy=True).     
-0001f7a0: 2020 2070 5f6d 696e 7573 203d 206e 702e     p_minus = np.
-0001f7b0: 6172 7261 7928 7076 616c 732c 2063 6f70  array(pvals, cop
-0001f7c0: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
-0001f7d0: 6b20 3d20 300a 2020 2020 2020 2020 666f  k = 0.        fo
-0001f7e0: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
-0001f7f0: 2870 7661 6c73 2929 3a0a 2020 2020 2020  (pvals)):.      
-0001f800: 2020 2020 2020 6966 206e 6f74 2066 6978        if not fix
-0001f810: 6564 5061 7273 5b6a 5d3a 0a20 2020 2020  edPars[j]:.     
-0001f820: 2020 2020 2020 2020 2020 2070 5f70 6c75             p_plu
-0001f830: 735b 6a5d 203d 2070 7661 6c73 5b6a 5d20  s[j] = pvals[j] 
-0001f840: 2b20 6470 5b6b 5d0a 2020 2020 2020 2020  + dp[k].        
-0001f850: 2020 2020 2020 2020 705f 6d69 6e75 735b          p_minus[
-0001f860: 6a5d 203d 2070 7661 6c73 5b6a 5d20 2d20  j] = pvals[j] - 
-0001f870: 6470 5b6b 5d0a 2020 2020 2020 2020 2020  dp[k].          
-0001f880: 2020 2020 2020 6466 6470 5b6b 5d20 3d20        dfdp[k] = 
-0001f890: 302e 3520 2f20 6470 5b6b 5d20 2a20 286d  0.5 / dp[k] * (m
-0001f8a0: 6f64 656c 2878 2c20 2a70 5f70 6c75 7329  odel(x, *p_plus)
-0001f8b0: 202d 206d 6f64 656c 2878 2c20 2a70 5f6d   - model(x, *p_m
-0001f8c0: 696e 7573 2929 0a20 2020 2020 2020 2020  inus)).         
-0001f8d0: 2020 2020 2020 2070 5f70 6c75 735b 6a5d         p_plus[j]
-0001f8e0: 203d 2070 7661 6c73 5b6a 5d0a 2020 2020   = pvals[j].    
-0001f8f0: 2020 2020 2020 2020 2020 2020 705f 6d69              p_mi
-0001f900: 6e75 735b 6a5d 203d 2070 7661 6c73 5b6a  nus[j] = pvals[j
-0001f910: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0001f920: 2020 6b20 2b3d 2031 0a20 2020 2020 2020    k += 1.       
-0001f930: 2023 2020 2073 7175 6172 6520 6f66 2075   #   square of u
-0001f940: 6e63 6572 7461 696e 7469 6573 206f 6e20  ncertainties on 
-0001f950: 6675 6e63 7469 6f6e 2076 616c 7565 730a  function values.
-0001f960: 2020 2020 2020 2020 4465 6c74 6120 3d20          Delta = 
-0001f970: 6e70 2e65 6d70 7479 286c 656e 2878 2929  np.empty(len(x))
-0001f980: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-0001f990: 6e20 7261 6e67 6528 6c65 6e28 7829 293a  n range(len(x)):
-0001f9a0: 0a20 2020 2020 2020 2020 2020 2044 656c  .            Del
-0001f9b0: 7461 5b69 5d20 3d20 6e70 2e73 756d 286e  ta[i] = np.sum(n
-0001f9c0: 702e 6f75 7465 7228 6466 6470 5b3a 2c20  p.outer(dfdp[:, 
-0001f9d0: 695d 2c20 6466 6470 5b3a 2c20 695d 2920  i], dfdp[:, i]) 
-0001f9e0: 2a20 636f 7670 290a 2020 2020 2020 2020  * covp).        
-0001f9f0: 7265 7475 726e 206e 702e 7371 7274 2844  return np.sqrt(D
-0001fa00: 656c 7461 290a 0a20 2020 2064 6566 2064  elta)..    def d
-0001fa10: 6f5f 6669 7428 7365 6c66 293a 0a20 2020  o_fit(self):.   
-0001fa20: 2020 2020 2022 2222 7065 7266 6f72 6d20       """perform 
-0001fa30: 616c 6c20 6e65 6365 7373 6172 7920 7374  all necessary st
-0001fa40: 6570 7320 6f66 2066 6974 2073 6571 7565  eps of fit seque
-0001fa50: 6e63 6522 2222 0a20 2020 2020 2020 2069  nce""".        i
-0001fa60: 6620 7365 6c66 2e64 6174 6120 6973 204e  f self.data is N
-0001fa70: 6f6e 6520 616e 6420 7365 6c66 2e66 6974  one and self.fit
-0001fa80: 5f74 7970 6520 213d 2022 7573 6572 223a  _type != "user":
-0001fa90: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001faa0: 7365 2056 616c 7565 4572 726f 7228 2220  se ValueError(" 
-0001fab0: 2121 2120 6d6e 4669 743a 206e 6f20 6461  !!! mnFit: no da
-0001fac0: 7461 206f 626a 6563 7420 6465 6669 6e65  ta object define
-0001fad0: 6420 2d20 6361 6c6c 2069 6e69 745f 6461  d - call init_da
-0001fae0: 7461 2829 2229 0a20 2020 2020 2020 2069  ta()").        i
-0001faf0: 6620 7365 6c66 2e63 6f73 7466 2069 7320  f self.costf is 
-0001fb00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001fb10: 2020 7261 6973 6520 5275 6e74 696d 6545    raise RuntimeE
-0001fb20: 7272 6f72 2822 2121 2120 6d6e 4669 743a  rror("!!! mnFit:
-0001fb30: 206e 6f20 6669 7420 6f62 6a65 6374 2064   no fit object d
-0001fb40: 6566 696e 6564 202d 2063 616c 6c20 696e  efined - call in
-0001fb50: 6974 5f66 6974 2829 2229 0a0a 2020 2020  it_fit()")..    
-0001fb60: 2020 2020 2320 7375 6d6d 6172 697a 6520      # summarize 
-0001fb70: 6f70 7469 6f6e 730a 2020 2020 2020 2020  options.        
-0001fb80: 6966 206e 6f74 2073 656c 662e 7175 6965  if not self.quie
-0001fb90: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
-0001fba0: 6620 7365 6c66 2e69 7465 7261 7465 4669  f self.iterateFi
-0001fbb0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0001fbc0: 2020 2070 7269 6e74 2822 2a3d 3d2a 206d     print("*==* m
-0001fbd0: 6e46 6974 2073 7461 7274 696e 6720 7072  nFit starting pr
-0001fbe0: 652d 6669 7422 290a 2020 2020 2020 2020  e-fit").        
-0001fbf0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001fc00: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0001fc10: 222a 3d3d 2a20 6d6e 4669 7420 7374 6172  "*==* mnFit star
-0001fc20: 7469 6e67 2066 6974 2229 0a20 2020 2020  ting fit").     
-0001fc30: 2020 2020 2020 2070 7269 6e74 2822 2020         print("  
-0001fc40: 4f70 7469 6f6e 733a 2229 0a20 2020 2020  Options:").     
-0001fc50: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
-0001fc60: 6e20 7365 6c66 2e6f 7074 696f 6e73 2e6b  n self.options.k
-0001fc70: 6579 7328 293a 0a20 2020 2020 2020 2020  eys():.         
-0001fc80: 2020 2020 2020 2072 656c 6576 616e 7420         relevant 
-0001fc90: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0001fca0: 2020 2020 2020 2020 7365 6c66 2e6f 7074          self.opt
-0001fcb0: 696f 6e73 5b6b 6579 5d5b 315d 203d 3d20  ions[key][1] == 
-0001fcc0: 2261 6c6c 220a 2020 2020 2020 2020 2020  "all".          
-0001fcd0: 2020 2020 2020 2020 2020 6f72 2073 656c            or sel
-0001fce0: 662e 6669 745f 7479 7065 2069 6e20 7365  f.fit_type in se
-0001fcf0: 6c66 2e6f 7074 696f 6e73 5b6b 6579 5d5b  lf.options[key][
-0001fd00: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
-0001fd10: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001fd20: 2020 2020 2069 6620 7265 6c65 7661 6e74       if relevant
-0001fd30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001fd40: 2020 2020 2020 696f 7074 203d 2073 656c        iopt = sel
-0001fd50: 662e 6f70 7469 6f6e 735b 6b65 795d 5b30  f.options[key][0
-0001fd60: 5d20 2b20 320a 2020 2020 2020 2020 2020  ] + 2.          
-0001fd70: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-0001fd80: 3520 2a20 2220 2220 2b20 222d 2022 2c20  5 * " " + "- ", 
-0001fd90: 7365 6c66 2e6f 7074 696f 6e73 5b6b 6579  self.options[key
-0001fda0: 5d5b 696f 7074 5d29 0a20 2020 2020 2020  ][iopt]).       
-0001fdb0: 2020 2020 2070 7269 6e74 2822 5c6e 2229       print("\n")
-0001fdc0: 0a0a 2020 2020 2020 2020 2320 7065 7266  ..        # perf
-0001fdd0: 6f72 6d20 2869 6e69 7469 616c 2920 6669  orm (initial) fi
-0001fde0: 740a 2020 2020 2020 2020 7472 793a 0a20  t.        try:. 
-0001fdf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001fe00: 6d69 6772 6164 5265 7375 6c74 203d 2073  migradResult = s
-0001fe10: 656c 662e 6d69 6e75 6974 2e6d 6967 7261  elf.minuit.migra
-0001fe20: 6428 2920 2023 2066 696e 6420 6d69 6e69  d()  # find mini
-0001fe30: 6d75 6d20 6f66 2063 6f73 7420 6675 6e63  mum of cost func
-0001fe40: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-0001fe50: 2073 656c 662e 6d69 6772 6164 5f6f 6b20   self.migrad_ok 
-0001fe60: 3d20 5472 7565 0a20 2020 2020 2020 2065  = True.        e
-0001fe70: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0001fe80: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-0001fe90: 2020 7365 6c66 2e6d 6967 7261 645f 6f6b    self.migrad_ok
-0001fea0: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-0001feb0: 2020 2020 2070 7269 6e74 2865 290a 2020       print(e).  
-0001fec0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001fed0: 5275 6e74 696d 6545 7272 6f72 2822 2a3d  RuntimeError("*=
-0001fee0: 3d2a 2021 2121 2066 6974 2077 6974 6820  =* !!! fit with 
-0001fef0: 6d69 6772 6164 2066 6169 6c65 6422 290a  migrad failed").
-0001ff00: 0a20 2020 2020 2020 2023 2070 6f73 7369  .        # possi
-0001ff10: 626c 792c 206e 6565 6420 746f 2069 7465  bly, need to ite
-0001ff20: 7261 7465 0a20 2020 2020 2020 2069 6620  rate.        if 
-0001ff30: 7365 6c66 2e69 7465 7261 7465 4669 743a  self.iterateFit:
-0001ff40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001ff50: 6e6f 7420 7365 6c66 2e71 7569 6574 3a0a  not self.quiet:.
-0001ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff70: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-0001ff80: 2020 2020 2020 2020 2020 2022 2a3d 3d2a             "*==*
-0001ff90: 206d 6e46 6974 2069 7465 7261 7469 6e67   mnFit iterating
-0001ffa0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0001ffb0: 2020 2020 2020 2022 746f 2061 6363 6f75         "to accou
-0001ffc0: 6e74 2066 6f72 2070 6172 616d 6574 6572  nt for parameter
-0001ffd0: 2d64 6570 656e 6465 6e74 2075 6e63 6572  -dependent uncer
-0001ffe0: 7461 696e 7469 6573 222c 0a20 2020 2020  tainties",.     
-0001fff0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00020000: 2020 2020 2020 2020 2023 2065 6e61 626c           # enabl
-00020010: 6520 6479 6e61 6d69 6320 6361 6c63 756c  e dynamic calcul
-00020020: 6174 696f 6e20 6f66 2063 6f76 6172 6961  ation of covaria
-00020030: 6e63 6520 6d61 7472 6978 0a20 2020 2020  nce matrix.     
-00020040: 2020 2020 2020 2073 656c 662e 6461 7461         self.data
-00020050: 2e69 6e69 745f 6479 6e61 6d69 6345 7272  .init_dynamicErr
-00020060: 6f72 7328 290a 0a20 2020 2020 2020 2020  ors()..         
-00020070: 2020 2023 2066 6974 2077 6974 6820 6479     # fit with dy
-00020080: 6e61 6d69 6320 7265 6361 6c63 756c 6174  namic recalculat
-00020090: 696f 6e20 6f66 2063 6f76 6172 6961 6e63  ion of covarianc
-000200a0: 6520 6d61 7472 6978 0a20 2020 2020 2020  e matrix.       
-000200b0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000200c0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-000200d0: 6967 7261 6452 6573 756c 7420 3d20 7365  igradResult = se
-000200e0: 6c66 2e6d 696e 7569 742e 6d69 6772 6164  lf.minuit.migrad
-000200f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00020100: 2020 2073 656c 662e 6d69 6772 6164 5f6f     self.migrad_o
-00020110: 6b20 3d20 5472 7565 0a20 2020 2020 2020  k = True.       
-00020120: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00020130: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
-00020140: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00020150: 2e6d 6967 7261 645f 6f6b 203d 2046 616c  .migrad_ok = Fal
-00020160: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-00020170: 2020 2070 7269 6e74 2865 290a 2020 2020     print(e).    
-00020180: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00020190: 6520 5275 6e74 696d 6545 7272 6f72 2822  e RuntimeError("
-000201a0: 2a3d 3d2a 2021 2121 2069 7465 7261 7469  *==* !!! iterati
-000201b0: 6f6e 206f 6620 6669 7420 7769 7468 206d  on of fit with m
-000201c0: 6967 7261 6420 6661 696c 6564 2229 0a0a  igrad failed")..
-000201d0: 2020 2020 2020 2020 2320 7275 6e20 7072          # run pr
-000201e0: 6f66 696c 6520 6c69 6b65 6c69 686f 6f64  ofile likelihood
-000201f0: 2073 6361 6e20 746f 2063 6865 636b 2066   scan to check f
-00020200: 6f72 2061 7379 6d6d 6574 7269 6320 6572  or asymmetric er
-00020210: 726f 7273 0a20 2020 2020 2020 2069 6620  rors.        if 
-00020220: 7365 6c66 2e72 756e 5f6d 696e 6f73 3a0a  self.run_minos:.
-00020230: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00020240: 6f74 2073 656c 662e 7175 6965 743a 0a20  ot self.quiet:. 
-00020250: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00020260: 7269 6e74 2822 2a3d 3d2a 206d 6e46 6974  rint("*==* mnFit
-00020270: 2073 7461 7274 696e 6720 6d69 6e6f 7320   starting minos 
-00020280: 7363 616e 2229 0a20 2020 2020 2020 2020  scan").         
-00020290: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000202a0: 2020 2020 2020 2020 7365 6c66 2e6d 696e          self.min
-000202b0: 6f73 5265 7375 6c74 203d 2073 656c 662e  osResult = self.
-000202c0: 6d69 6e75 6974 2e6d 696e 6f73 2829 0a20  minuit.minos(). 
-000202d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000202e0: 656c 662e 6d69 6e6f 735f 6f6b 203d 2054  elf.minos_ok = T
-000202f0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00020300: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00020310: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00020320: 2020 2020 2020 2073 656c 662e 6d69 6e6f         self.mino
-00020330: 735f 6f6b 203d 2046 616c 7365 0a20 2020  s_ok = False.   
-00020340: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00020350: 6e6f 7420 7365 6c66 2e71 7569 6574 3a0a  not self.quiet:.
-00020360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020370: 2020 2020 7072 696e 7428 222a 3d3d 2a20      print("*==* 
-00020380: 6d6e 4669 743a 2021 2121 206d 696e 6f73  mnFit: !!! minos
-00020390: 2066 6169 6c65 6420 5c6e 222c 2065 290a   failed \n", e).
-000203a0: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
-000203b0: 6f72 6552 6573 756c 7428 290a 2020 2020  oreResult().    
-000203c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000203d0: 6d69 6772 6164 5265 7375 6c74 2c20 7365  migradResult, se
-000203e0: 6c66 2e6d 696e 6f73 5265 7375 6c74 0a0a  lf.minosResult..
-000203f0: 2020 2020 6465 6620 7365 7450 6c6f 744f      def setPlotO
-00020400: 7074 696f 6e73 2873 656c 6629 3a0a 2020  ptions(self):.  
-00020410: 2020 2020 2020 2222 2253 6574 206f 7074        """Set opt
-00020420: 696f 6e73 2066 6f72 206e 6963 6572 2070  ions for nicer p
-00020430: 6c6f 7474 696e 6722 2222 0a0a 2020 2020  lotting"""..    
-00020440: 2020 2020 2320 746f 2062 6520 696d 706c      # to be impl
-00020450: 656d 656e 7465 640a 2020 2020 2020 2020  emented.        
-00020460: 7061 7373 0a0a 2020 2020 6465 6620 706c  pass..    def pl
-00020470: 6f74 4d6f 6465 6c28 0a20 2020 2020 2020  otModel(.       
-00020480: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
-00020490: 7869 735f 6c61 6265 6c73 3d5b 2278 222c  xis_labels=["x",
-000204a0: 2022 7920 3d20 6628 782c 202a 7061 7229   "y = f(x, *par)
-000204b0: 225d 2c0a 2020 2020 2020 2020 6461 7461  "],.        data
-000204c0: 5f6c 6567 656e 643d 2264 6174 6122 2c0a  _legend="data",.
-000204d0: 2020 2020 2020 2020 6d6f 6465 6c5f 6c65          model_le
-000204e0: 6765 6e64 3d22 6669 7422 2c0a 2020 2020  gend="fit",.    
-000204f0: 2020 2020 706c 6f74 5f62 616e 643d 5472      plot_band=Tr
-00020500: 7565 2c0a 2020 2020 2020 2020 7361 6d65  ue,.        same
-00020510: 5f70 6c6f 743d 4661 6c73 652c 0a20 2020  _plot=False,.   
-00020520: 2020 2020 2070 6c6f 745f 7265 7369 6475       plot_residu
-00020530: 616c 3d46 616c 7365 2c0a 2020 2020 293a  al=False,.    ):
-00020540: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00020550: 2020 2020 2050 6c6f 7420 6d6f 6465 6c20       Plot model 
-00020560: 6675 6e63 7469 6f6e 2061 6e64 2064 6174  function and dat
-00020570: 610a 0a20 2020 2020 2020 2055 7365 7320  a..        Uses 
-00020580: 696d 696e 7569 744f 626a 6563 742c 2063  iminuitObject, c
-00020590: 6f73 7420 4675 6e63 7469 6f6e 2028 616e  ost Function (an
-000205a0: 6420 6461 7461 206f 626a 6563 7429 0a0a  d data object)..
-000205b0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-000205c0: 2020 2020 2020 2020 2a20 6c69 7374 206f          * list o
-000205d0: 6620 7374 723a 2061 7869 7320 6c61 6265  f str: axis labe
-000205e0: 6c73 0a20 2020 2020 2020 2020 202a 2073  ls.          * s
-000205f0: 7472 3a20 6c65 6765 6e64 2066 6f72 2064  tr: legend for d
-00020600: 6174 610a 2020 2020 2020 2020 2020 2a20  ata.          * 
-00020610: 7374 723a 206c 6567 656e 6420 666f 7220  str: legend for 
-00020620: 6d6f 6465 6c0a 2020 2020 2020 2020 2020  model.          
-00020630: 2a20 706c 6f74 5f62 616e 643a 2070 6c6f  * plot_band: plo
-00020640: 7420 6d6f 6465 6c20 636f 6e66 6964 656e  t model confiden
-00020650: 6365 2062 616e 6420 6966 2054 7275 650a  ce band if True.
-00020660: 2020 2020 2020 2020 2020 2a20 7361 6d65            * same
-00020670: 5f70 6c6f 743a 2061 6363 756d 756c 6174  _plot: accumulat
-00020680: 6520 6669 7420 7265 7375 6c74 7320 6672  e fit results fr
-00020690: 6f6d 2070 7265 7669 6f75 7320 6361 6c6c  om previous call
-000206a0: 2069 6620 5472 7565 0a20 2020 2020 2020   if True.       
-000206b0: 2020 202a 2070 6c6f 745f 7265 7369 6475     * plot_residu
-000206c0: 616c 3a20 706c 6f74 2072 6573 6964 7561  al: plot residua
-000206d0: 6c20 772e 722e 742e 206d 6f64 656c 2069  l w.r.t. model i
-000206e0: 6620 5472 7565 0a0a 2020 2020 2020 2020  f True..        
-000206f0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00020700: 2020 202a 206d 6174 706c 6f74 6c69 6220     * matplotlib 
-00020710: 6669 6775 7265 0a20 2020 2020 2020 2022  figure.        "
-00020720: 2222 0a0a 2020 2020 2020 2020 2320 6163  ""..        # ac
-00020730: 6365 7373 206f 626a 6563 7473 0a20 2020  cess objects.   
-00020740: 2020 2020 206d 203d 2073 656c 662e 6d69       m = self.mi
-00020750: 6e75 6974 2020 2320 6d69 6e75 6974 206f  nuit  # minuit o
-00020760: 626a 6563 740a 2020 2020 2020 2020 6366  bject.        cf
-00020770: 203d 2073 656c 662e 636f 7374 6620 2023   = self.costf  #
-00020780: 2063 6f73 7420 6675 6e63 7469 6f6e 206f   cost function o
-00020790: 626a 6563 740a 2020 2020 2020 2020 6420  bject.        d 
-000207a0: 3d20 6366 2e64 6174 610a 2020 2020 2020  = cf.data.      
-000207b0: 2020 6e70 7473 203d 206d 6178 2831 3930    npts = max(190
-000207c0: 2c20 3520 2a20 642e 646c 656e 6774 6829  , 5 * d.dlength)
-000207d0: 2020 2320 6e75 6d62 6572 206f 6620 706f    # number of po
-000207e0: 696e 7473 2066 6f72 206d 6f64 656c 2066  ints for model f
-000207f0: 756e 6374 696f 6e0a 0a20 2020 2020 2020  unction..       
-00020800: 2023 2072 6574 7269 6576 6520 6669 7420   # retrieve fit 
-00020810: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
-00020820: 706e 616d 7320 3d20 7365 6c66 2e50 6172  pnams = self.Par
-00020830: 616d 6574 6572 4e61 6d65 730a 2020 2020  ameterNames.    
-00020840: 2020 2020 7076 616c 7320 3d20 7365 6c66      pvals = self
-00020850: 2e50 6172 616d 6574 6572 5661 6c75 6573  .ParameterValues
-00020860: 0a20 2020 2020 2020 2070 6d65 7272 7320  .        pmerrs 
-00020870: 3d20 7365 6c66 2e4f 6e65 5369 6749 6e74  = self.OneSigInt
-00020880: 6572 7661 6c0a 2020 2020 2020 2020 2320  erval.        # 
-00020890: 2073 796d 6d65 7472 6963 2065 7272 6f72   symmetric error
-000208a0: 730a 2020 2020 2020 2020 7065 7272 7320  s.        perrs 
-000208b0: 3d20 2870 6d65 7272 735b 3a2c 2031 5d20  = (pmerrs[:, 1] 
-000208c0: 2d20 706d 6572 7273 5b3a 2c20 305d 2920  - pmerrs[:, 0]) 
-000208d0: 2f20 322e 300a 2020 2020 2020 2020 636f  / 2.0.        co
-000208e0: 7220 3d20 7365 6c66 2e43 6f72 7265 6c61  r = self.Correla
-000208f0: 7469 6f6e 4d61 7472 6978 0a20 2020 2020  tionMatrix.     
-00020900: 2020 2023 2020 636f 7661 7269 616e 6365     #  covariance
-00020910: 206d 6174 7269 7820 6672 6f6d 2063 6f72   matrix from cor
-00020920: 7265 6c61 7469 6f6e 730a 2020 2020 2020  relations.      
-00020930: 2020 7063 6f76 203d 2063 6f72 202a 206e    pcov = cor * n
-00020940: 702e 6f75 7465 7228 7065 7272 732c 2070  p.outer(perrs, p
-00020950: 6572 7273 290a 2020 2020 2020 2020 676f  errs).        go
-00020960: 6620 3d20 7365 6c66 2e47 6f46 0a20 2020  f = self.GoF.   
-00020970: 2020 2020 206e 646f 6620 3d20 6366 2e6e       ndof = cf.n
-00020980: 646f 660a 2020 2020 2020 2020 2320 2063  dof.        #  c
-00020990: 6869 3270 7262 0a20 2020 2020 2020 2069  hi2prb.        i
-000209a0: 6620 676f 6620 6973 206e 6f74 204e 6f6e  f gof is not Non
-000209b0: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
-000209c0: 6869 3270 7262 203d 2073 656c 662e 6368  hi2prb = self.ch
-000209d0: 6932 7072 6228 676f 662c 206e 646f 6629  i2prb(gof, ndof)
-000209e0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000209f0: 2020 2020 2020 2020 2020 2063 6869 3270             chi2p
-00020a00: 7262 203d 204e 6f6e 650a 2020 2020 2020  rb = None.      
-00020a10: 2020 2320 7661 6c75 6573 206f 6620 6672    # values of fr
-00020a20: 6565 2061 6e64 2066 6978 6564 2070 6172  ee and fixed par
-00020a30: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00020a40: 6669 7865 6450 6172 7320 3d20 7365 6c66  fixedPars = self
-00020a50: 2e66 6978 6564 5061 7273 0a20 2020 2020  .fixedPars.     
-00020a60: 2020 2066 7265 655f 7076 616c 7320 3d20     free_pvals = 
-00020a70: 7365 6c66 2e66 7265 6550 6172 5661 6c73  self.freeParVals
-00020a80: 0a20 2020 2020 2020 2066 7265 655f 706e  .        free_pn
-00020a90: 616d 7320 3d20 7365 6c66 2e66 7265 6550  ams = self.freeP
-00020aa0: 6172 4e61 6d73 0a20 2020 2020 2020 2066  arNams.        f
-00020ab0: 6978 6564 5f70 6e61 6d73 203d 2073 656c  ixed_pnams = sel
-00020ac0: 662e 6669 7865 6450 6172 4e61 6d73 0a20  f.fixedParNams. 
-00020ad0: 2020 2020 2020 2066 6978 6564 5f70 7661         fixed_pva
-00020ae0: 6c73 203d 2073 656c 662e 6669 7865 6450  ls = self.fixedP
-00020af0: 6172 5661 6c73 0a20 2020 2020 2020 206e  arVals.        n
-00020b00: 6669 7865 6420 3d20 6c65 6e28 6669 7865  fixed = len(fixe
-00020b10: 645f 7076 616c 7329 0a0a 2020 2020 2020  d_pvals)..      
-00020b20: 2020 2320 706c 6f74 2064 6174 610a 2020    # plot data.  
-00020b30: 2020 2020 2020 6669 675f 6d6f 6465 6c20        fig_model 
-00020b40: 3d20 642e 706c 6f74 280a 2020 2020 2020  = d.plot(.      
-00020b50: 2020 2020 2020 6669 6773 697a 653d 2837        figsize=(7
-00020b60: 2e35 2c20 362e 3529 2c20 6461 7461 5f6c  .5, 6.5), data_l
-00020b70: 6162 656c 3d64 6174 615f 6c65 6765 6e64  abel=data_legend
-00020b80: 2c20 706c 6f74 5f72 6573 6964 7561 6c3d  , plot_residual=
-00020b90: 706c 6f74 5f72 6573 6964 7561 6c0a 2020  plot_residual.  
-00020ba0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00020bb0: 2023 206f 7665 726c 6179 206d 6f64 656c   # overlay model
-00020bc0: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
-00020bd0: 2020 2320 6869 7374 6f67 7261 6d20 6669    # histogram fi
-00020be0: 7420 7072 6f76 6964 6573 206e 6f72 6d61  t provides norma
-00020bf0: 6c69 7365 6420 6469 7374 7269 6275 7469  lised distributi
-00020c00: 6f6e 2c0a 2020 2020 2020 2020 2320 2020  on,.        #   
-00020c10: 2064 6574 6572 6d69 6e65 2062 696e 2077   determine bin w
-00020c20: 6964 7468 7320 616e 6420 7363 616c 6520  idths and scale 
-00020c30: 6661 6374 6f72 0a20 2020 2020 2020 2078  factor.        x
-00020c40: 6d69 6e2c 2078 6d61 7820 3d20 706c 742e  min, xmax = plt.
-00020c50: 786c 696d 2829 0a20 2020 2020 2020 2078  xlim().        x
-00020c60: 706c 7420 3d20 6e70 2e6c 696e 7370 6163  plt = np.linspac
-00020c70: 6528 786d 696e 2c20 786d 6178 2c20 6e70  e(xmin, xmax, np
-00020c80: 7473 290a 2020 2020 2020 2020 7876 616c  ts).        xval
-00020c90: 7320 3d20 7870 6c74 0a20 2020 2020 2020  s = xplt.       
-00020ca0: 2069 6620 7365 6c66 2e66 6974 5f74 7970   if self.fit_typ
-00020cb0: 6520 3d3d 2022 6869 7374 223a 0a20 2020  e == "hist":.   
-00020cc0: 2020 2020 2020 2020 2023 2064 6574 656d           # detem
-00020cd0: 696e 6520 6c6f 6361 6c20 6269 6e20 7769  ine local bin wi
-00020ce0: 6474 680a 2020 2020 2020 2020 2020 2020  dth.            
-00020cf0: 6277 6964 7468 7320 3d20 6e70 2e7a 6572  bwidths = np.zer
-00020d00: 6f73 286c 656e 2878 706c 7429 290a 2020  os(len(xplt)).  
-00020d10: 2020 2020 2020 2020 2020 6920 3d20 300a            i = 0.
-00020d20: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00020d30: 6a2c 2078 2069 6e20 656e 756d 6572 6174  j, x in enumerat
-00020d40: 6528 7870 6c74 293a 0a20 2020 2020 2020  e(xplt):.       
-00020d50: 2020 2020 2020 2020 2069 6620 7820 3e3d           if x >=
-00020d60: 2063 662e 6461 7461 2e72 6967 6874 735b   cf.data.rights[
-00020d70: 6d69 6e28 692c 2063 662e 6461 7461 2e6e  min(i, cf.data.n
-00020d80: 6269 6e73 202d 2031 295d 3a0a 2020 2020  bins - 1)]:.    
-00020d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020da0: 6920 2b3d 2031 0a20 2020 2020 2020 2020  i += 1.         
-00020db0: 2020 2020 2020 2062 7769 6474 6873 5b6a         bwidths[j
-00020dc0: 5d20 3d20 6366 2e64 6174 612e 7769 6474  ] = cf.data.widt
-00020dd0: 6873 5b6d 696e 2869 2c20 6366 2e64 6174  hs[min(i, cf.dat
-00020de0: 612e 6e62 696e 7320 2d20 3129 5d0a 2020  a.nbins - 1)].  
-00020df0: 2020 2020 2020 2020 2020 7366 6163 203d            sfac =
-00020e00: 2063 662e 6e6f 726d 202a 2062 7769 6474   cf.norm * bwidt
-00020e10: 6873 0a20 2020 2020 2020 2065 6c69 6620  hs.        elif 
-00020e20: 7365 6c66 2e66 6974 5f74 7970 6520 3d3d  self.fit_type ==
-00020e30: 2022 7879 2220 6f72 2073 656c 662e 6669   "xy" or self.fi
-00020e40: 745f 7479 7065 203d 3d20 226d 6c22 3a0a  t_type == "ml":.
-00020e50: 2020 2020 2020 2020 2020 2020 7366 6163              sfac
-00020e60: 203d 2031 2e30 0a20 2020 2020 2020 2065   = 1.0.        e
-00020e70: 6c69 6620 7365 6c66 2e66 6974 5f74 7970  lif self.fit_typ
-00020e80: 6520 3d3d 2022 696e 6465 7865 6422 3a0a  e == "indexed":.
-00020e90: 2020 2020 2020 2020 2020 2020 7366 6163              sfac
-00020ea0: 203d 2031 2e30 0a20 2020 2020 2020 2020   = 1.0.         
-00020eb0: 2020 2078 7661 6c73 203d 2063 662e 6461     xvals = cf.da
-00020ec0: 7461 2e78 0a20 2020 2020 2020 2020 2020  ta.x.           
-00020ed0: 2078 706c 7420 3d20 6e70 2e6c 696e 7370   xplt = np.linsp
-00020ee0: 6163 6528 302e 352c 206c 656e 2878 7661  ace(0.5, len(xva
-00020ef0: 6c73 2920 2d20 302e 352c 206c 656e 2878  ls) - 0.5, len(x
-00020f00: 7661 6c73 2929 0a20 2020 2020 2020 2065  vals)).        e
-00020f10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00020f20: 2070 7269 6e74 2822 212a 2a21 206d 6e46   print("!**! mnF
-00020f30: 6974 2e70 6c6f 744d 6f64 656c 3a20 756e  it.plotModel: un
-00020f40: 6b6e 6f77 6e20 6669 7420 7479 7065 3a20  known fit type: 
-00020f50: 222c 2073 656c 662e 6669 745f 7479 7065  ", self.fit_type
-00020f60: 290a 2020 2020 2020 2020 2020 2020 7366  ).            sf
-00020f70: 6163 203d 2031 2e30 0a20 2020 2020 2020  ac = 1.0.       
-00020f80: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-00020f90: 2020 2020 2023 2064 6f20 7765 2077 616e       # do we wan
-00020fa0: 7420 6d6f 6465 6c20 6f72 2072 6573 6964  t model or resid
-00020fb0: 7561 6c73 203f 0a20 2020 2020 2020 2069  uals ?.        i
-00020fc0: 6620 706c 6f74 5f72 6573 6964 7561 6c3a  f plot_residual:
-00020fd0: 0a20 2020 2020 2020 2020 2020 2079 706c  .            ypl
-00020fe0: 7420 3d20 6e70 2e7a 6572 6f73 286c 656e  t = np.zeros(len
-00020ff0: 2878 706c 7429 290a 2020 2020 2020 2020  (xplt)).        
-00021000: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00021010: 2020 7970 6c74 203d 2063 662e 6d6f 6465    yplt = cf.mode
-00021020: 6c28 7876 616c 732c 202a 7076 616c 7329  l(xvals, *pvals)
-00021030: 0a0a 2020 2020 2020 2020 2320 2070 6c6f  ..        #  plo
-00021040: 7420 6d6f 6465 6c20 6c69 6e65 0a20 2020  t model line.   
-00021050: 2020 2020 2069 6620 7365 6c66 2e66 6974       if self.fit
-00021060: 5f74 7970 6520 3d3d 2022 696e 6465 7865  _type == "indexe
-00021070: 6422 3a0a 2020 2020 2020 2020 2020 2020  d":.            
-00021080: 706c 742e 6572 726f 7262 6172 280a 2020  plt.errorbar(.  
-00021090: 2020 2020 2020 2020 2020 2020 2020 7870                xp
-000210a0: 6c74 2c0a 2020 2020 2020 2020 2020 2020  lt,.            
-000210b0: 2020 2020 7970 6c74 2c0a 2020 2020 2020      yplt,.      
-000210c0: 2020 2020 2020 2020 2020 666d 743d 2220            fmt=" 
-000210d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000210e0: 2020 2078 6572 723d 302e 342c 0a20 2020     xerr=0.4,.   
-000210f0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-00021100: 656c 3d6d 6f64 656c 5f6c 6567 656e 642c  el=model_legend,
-00021110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021120: 2061 6c70 6861 3d30 2e37 2c0a 2020 2020   alpha=0.7,.    
-00021130: 2020 2020 2020 2020 2020 2020 656c 696e              elin
-00021140: 6577 6964 7468 3d32 2e35 2c0a 2020 2020  ewidth=2.5,.    
-00021150: 2020 2020 2020 2020 2020 2020 636f 6c6f              colo
-00021160: 723d 2264 6172 6b6f 7261 6e67 6522 2c0a  r="darkorange",.
-00021170: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00021180: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00021190: 2020 2020 2020 2020 706c 742e 706c 6f74          plt.plot
-000211a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000211b0: 2020 7870 6c74 2c0a 2020 2020 2020 2020    xplt,.        
-000211c0: 2020 2020 2020 2020 7970 6c74 202a 2073          yplt * s
-000211d0: 6661 632c 0a20 2020 2020 2020 2020 2020  fac,.           
-000211e0: 2020 2020 206c 6162 656c 3d6d 6f64 656c       label=model
-000211f0: 5f6c 6567 656e 642c 0a20 2020 2020 2020  _legend,.       
-00021200: 2020 2020 2020 2020 206c 696e 6573 7479           linesty
-00021210: 6c65 3d22 6461 7368 6564 222c 0a20 2020  le="dashed",.   
-00021220: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-00021230: 6577 6964 7468 3d32 2e35 2c0a 2020 2020  ewidth=2.5,.    
-00021240: 2020 2020 2020 2020 2020 2020 616c 7068              alph
-00021250: 613d 302e 372c 0a20 2020 2020 2020 2020  a=0.7,.         
-00021260: 2020 2029 0a20 2020 2020 2020 2023 2320     ).        ## 
-00021270: 2020 2020 2020 2020 2063 6f6c 6f72 3d27           color='
-00021280: 6461 726b 6f72 616e 6765 2729 0a20 2020  darkorange').   
-00021290: 2020 2020 2070 6c74 2e78 6c61 6265 6c28       plt.xlabel(
-000212a0: 6178 6973 5f6c 6162 656c 735b 305d 2c20  axis_labels[0], 
-000212b0: 7369 7a65 3d22 782d 6c61 7267 6522 290a  size="x-large").
-000212c0: 2020 2020 2020 2020 706c 742e 796c 6162          plt.ylab
-000212d0: 656c 2861 7869 735f 6c61 6265 6c73 5b31  el(axis_labels[1
-000212e0: 5d2c 2073 697a 653d 2278 2d6c 6172 6765  ], size="x-large
-000212f0: 2229 0a20 2020 2020 2020 2070 6c74 2e67  ").        plt.g
-00021300: 7269 6428 290a 0a20 2020 2020 2020 2023  rid()..        #
-00021310: 2064 7261 7720 6572 726f 7220 6261 6e64   draw error band
-00021320: 2061 726f 756e 6420 6d6f 6465 6c20 6675   around model fu
-00021330: 6e63 7469 6f6e 0a20 2020 2020 2020 2069  nction.        i
-00021340: 6620 706c 6f74 5f62 616e 643a 0a20 2020  f plot_band:.   
-00021350: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00021360: 2e66 6974 5f74 7970 6520 213d 2022 696e  .fit_type != "in
-00021370: 6465 7865 6422 3a0a 2020 2020 2020 2020  dexed":.        
-00021380: 2020 2020 2020 2020 4465 6c74 6146 203d          DeltaF =
-00021390: 2073 656c 662e 6765 7446 756e 6374 696f   self.getFunctio
-000213a0: 6e45 7272 6f72 2878 706c 742c 2063 662e  nError(xplt, cf.
-000213b0: 6d6f 6465 6c2c 2070 7661 6c73 2c20 7063  model, pvals, pc
-000213c0: 6f76 2c20 6669 7865 6450 6172 7329 0a20  ov, fixedPars). 
-000213d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000213e0: 6c74 2e66 696c 6c5f 6265 7477 6565 6e28  lt.fill_between(
-000213f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021400: 2020 2020 2078 706c 742c 0a20 2020 2020       xplt,.     
-00021410: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00021420: 6661 6320 2a20 2879 706c 7420 2b20 4465  fac * (yplt + De
-00021430: 6c74 6146 292c 0a20 2020 2020 2020 2020  ltaF),.         
-00021440: 2020 2020 2020 2020 2020 2073 6661 6320             sfac 
-00021450: 2a20 2879 706c 7420 2d20 4465 6c74 6146  * (yplt - DeltaF
-00021460: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00021470: 2020 2020 2020 2061 6c70 6861 3d30 2e33         alpha=0.3
-00021480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021490: 2020 2020 2020 636f 6c6f 723d 2264 6172        color="dar
-000214a0: 6b6b 6861 6b69 222c 0a20 2020 2020 2020  kkhaki",.       
-000214b0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-000214c0: 656c 3d22 2020 245c 706d 2031 205c 7369  el="  $\pm 1 \si
-000214d0: 676d 6124 222c 0a20 2020 2020 2020 2020  gma$",.         
-000214e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000214f0: 2020 2020 2020 2020 2070 6c74 2e70 6c6f           plt.plo
-00021500: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00021510: 2020 2020 2020 2078 706c 742c 0a20 2020         xplt,.   
-00021520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021530: 2073 6661 6320 2a20 2879 706c 7420 2b20   sfac * (yplt + 
-00021540: 4465 6c74 6146 292c 0a20 2020 2020 2020  DeltaF),.       
-00021550: 2020 2020 2020 2020 2020 2020 206c 696e               lin
-00021560: 6577 6964 7468 3d31 2c0a 2020 2020 2020  ewidth=1,.      
-00021570: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00021580: 7068 613d 302e 342c 0a20 2020 2020 2020  pha=0.4,.       
-00021590: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-000215a0: 6f72 3d22 6461 726b 6772 6565 6e22 2c0a  or="darkgreen",.
-000215b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000215c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000215d0: 2020 706c 742e 706c 6f74 280a 2020 2020    plt.plot(.    
-000215e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000215f0: 7870 6c74 2c0a 2020 2020 2020 2020 2020  xplt,.          
-00021600: 2020 2020 2020 2020 2020 7366 6163 202a            sfac *
-00021610: 2028 7970 6c74 202d 2044 656c 7461 4629   (yplt - DeltaF)
-00021620: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021630: 2020 2020 2020 6c69 6e65 7769 6474 683d        linewidth=
-00021640: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00021650: 2020 2020 2020 2061 6c70 6861 3d30 2e34         alpha=0.4
-00021660: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021670: 2020 2020 2020 636f 6c6f 723d 2264 6172        color="dar
-00021680: 6b67 7265 656e 222c 0a20 2020 2020 2020  kgreen",.       
-00021690: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000216a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000216b0: 2020 2020 2020 2020 2020 2020 2044 656c               Del
-000216c0: 7461 203d 2073 656c 662e 6765 7446 756e  ta = self.getFun
-000216d0: 6374 696f 6e45 7272 6f72 2878 7661 6c73  ctionError(xvals
-000216e0: 2c20 6366 2e6d 6f64 656c 2c20 7076 616c  , cf.model, pval
-000216f0: 732c 2070 636f 762c 2066 6978 6564 5061  s, pcov, fixedPa
-00021700: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
-00021710: 2020 2020 706c 742e 6572 726f 7262 6172      plt.errorbar
-00021720: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00021730: 2020 2020 2020 7870 6c74 2c0a 2020 2020        xplt,.    
-00021740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021750: 7970 6c74 202b 2044 656c 7461 2c0a 2020  yplt + Delta,.  
-00021760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021770: 2020 666d 743d 2220 222c 0a20 2020 2020    fmt=" ",.     
-00021780: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00021790: 6572 723d 302e 342c 0a20 2020 2020 2020  err=0.4,.       
-000217a0: 2020 2020 2020 2020 2020 2020 2061 6c70               alp
-000217b0: 6861 3d30 2e37 2c0a 2020 2020 2020 2020  ha=0.7,.        
-000217c0: 2020 2020 2020 2020 2020 2020 656c 696e              elin
-000217d0: 6577 6964 7468 3d31 2e30 2c0a 2020 2020  ewidth=1.0,.    
-000217e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000217f0: 636f 6c6f 723d 2264 6172 6b67 7265 656e  color="darkgreen
-00021800: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00021810: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00021820: 2020 2020 2070 6c74 2e65 7272 6f72 6261       plt.errorba
-00021830: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00021840: 2020 2020 2020 2078 706c 742c 0a20 2020         xplt,.   
-00021850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021860: 2079 706c 7420 2d20 4465 6c74 612c 0a20   yplt - Delta,. 
-00021870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021880: 2020 2066 6d74 3d22 2022 2c0a 2020 2020     fmt=" ",.    
-00021890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000218a0: 7865 7272 3d30 2e34 2c0a 2020 2020 2020  xerr=0.4,.      
-000218b0: 2020 2020 2020 2020 2020 2020 2020 616c                al
-000218c0: 7068 613d 302e 372c 0a20 2020 2020 2020  pha=0.7,.       
-000218d0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-000218e0: 6e65 7769 6474 683d 312e 302c 0a20 2020  newidth=1.0,.   
-000218f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021900: 2063 6f6c 6f72 3d22 6461 726b 6772 6565   color="darkgree
-00021910: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00021920: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00021930: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00021940: 616e 6765 286c 656e 2878 706c 7429 293a  ange(len(xplt)):
-00021950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021960: 2020 2020 206c 626c 203d 2022 245c 706d       lbl = "$\pm
-00021970: 2031 205c 7369 676d 6124 2220 6966 2069   1 \sigma$" if i
-00021980: 203d 3d20 3020 656c 7365 2022 220a 2020   == 0 else "".  
-00021990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000219a0: 2020 706c 742e 6178 6873 7061 6e28 0a20    plt.axhspan(. 
-000219b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000219c0: 2020 2020 2020 2079 706c 745b 695d 202d         yplt[i] -
-000219d0: 2044 656c 7461 5b69 5d2c 0a20 2020 2020   Delta[i],.     
-000219e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000219f0: 2020 2079 706c 745b 695d 202b 2044 656c     yplt[i] + Del
-00021a00: 7461 5b69 5d2c 0a20 2020 2020 2020 2020  ta[i],.         
-00021a10: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00021a20: 6d69 6e3d 2878 706c 745b 695d 202d 2030  min=(xplt[i] - 0
-00021a30: 2e34 2920 2f20 6c65 6e28 7870 6c74 292c  .4) / len(xplt),
-00021a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021a50: 2020 2020 2020 2020 2078 6d61 783d 2878           xmax=(x
-00021a60: 706c 745b 695d 202b 2030 2e34 2920 2f20  plt[i] + 0.4) / 
-00021a70: 6c65 6e28 7870 6c74 292c 0a20 2020 2020  len(xplt),.     
-00021a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021a90: 2020 2061 6c70 6861 3d30 2e33 2c0a 2020     alpha=0.3,.  
-00021aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ab0: 2020 2020 2020 636f 6c6f 723d 2264 6172        color="dar
-00021ac0: 6b6b 6861 6b69 222c 0a20 2020 2020 2020  kkhaki",.       
+0001d8e0: 2020 2020 2020 2020 705f 6964 203d 2066          p_id = f
+0001d8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d900: 2020 2020 2073 656c 662e 6669 7865 6450       self.fixedP
+0001d910: 6172 735b 705f 6964 5d20 3d20 5472 7565  ars[p_id] = True
+0001d920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d930: 2073 656c 662e 6e66 6978 6564 203d 206c   self.nfixed = l
+0001d940: 656e 2866 6978 5061 7273 290a 2020 2020  en(fixPars).    
+0001d950: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001d960: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001d970: 2074 7970 6528 6669 7850 6172 7329 203d   type(fixPars) =
+0001d980: 3d20 7479 7065 2822 2022 293a 0a20 2020  = type(" "):.   
+0001d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9a0: 2070 5f69 6420 3d20 7365 6c66 2e70 6e61   p_id = self.pna
+0001d9b0: 6d32 6964 5b66 6978 5061 7273 5d0a 2020  m2id[fixPars].  
+0001d9c0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0001d9d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001d9e0: 2020 2020 2020 2020 705f 6964 203d 2066          p_id = f
+0001d9f0: 6978 5061 7273 0a20 2020 2020 2020 2020  ixPars.         
+0001da00: 2020 2020 2020 2073 656c 662e 6669 7865         self.fixe
+0001da10: 6450 6172 735b 705f 6964 5d20 3d20 5472  dPars[p_id] = Tr
+0001da20: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+0001da30: 2020 2073 656c 662e 6e66 6978 6564 203d     self.nfixed =
+0001da40: 2031 0a20 2020 2020 2020 2020 2020 2023   1.            #
+0001da50: 2067 6574 2070 6172 616d 6574 6572 206e   get parameter n
+0001da60: 616d 6573 206f 7220 696e 6469 6365 7320  ames or indices 
+0001da70: 6f66 2066 6978 6564 2070 6172 616d 6574  of fixed paramet
+0001da80: 6572 730a 2020 2020 2020 2020 2020 2020  ers.            
+0001da90: 7365 6c66 2e66 7265 6550 6172 4e61 6d73  self.freeParNams
+0001daa0: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+0001dab0: 2020 7365 6c66 2e66 6978 6564 5061 724e    self.fixedParN
+0001dac0: 616d 7320 3d20 5b5d 0a20 2020 2020 2020  ams = [].       
+0001dad0: 2020 2020 2066 6f72 2069 2c20 6669 7865       for i, fixe
+0001dae0: 6420 696e 2065 6e75 6d65 7261 7465 2873  d in enumerate(s
+0001daf0: 656c 662e 6669 7865 6450 6172 7329 3a0a  elf.fixedPars):.
+0001db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db10: 6966 206e 6f74 2066 6978 6564 3a0a 2020  if not fixed:.  
+0001db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db30: 2020 7365 6c66 2e66 7265 6550 6172 4e61    self.freeParNa
+0001db40: 6d73 2e61 7070 656e 6428 7365 6c66 2e70  ms.append(self.p
+0001db50: 6e61 6d73 5b69 5d29 0a20 2020 2020 2020  nams[i]).       
+0001db60: 2020 2020 2020 2020 2069 6620 6669 7865           if fixe
+0001db70: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
+0001db80: 2020 2020 2020 2073 656c 662e 6669 7865         self.fixe
+0001db90: 6450 6172 4e61 6d73 2e61 7070 656e 6428  dParNams.append(
+0001dba0: 7365 6c66 2e70 6e61 6d73 5b69 5d29 0a20  self.pnams[i]). 
+0001dbb0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001dbc0: 2020 2020 2020 2020 2073 656c 662e 6672           self.fr
+0001dbd0: 6565 5061 724e 616d 7320 3d20 7365 6c66  eeParNams = self
+0001dbe0: 2e70 6e61 6d73 0a20 2020 2020 2020 2020  .pnams.         
+0001dbf0: 2020 2073 656c 662e 6669 7865 6450 6172     self.fixedPar
+0001dc00: 4e61 6d73 203d 205b 5d0a 0a20 2020 2064  Nams = []..    d
+0001dc10: 6566 205f 7365 7475 704d 696e 7569 7428  ef _setupMinuit(
+0001dc20: 7365 6c66 2c20 6d6f 6465 6c5f 6b77 6172  self, model_kwar
+0001dc30: 6773 293a 0a20 2020 2020 2020 2022 2222  gs):.        """
+0001dc40: 6372 6561 7465 204d 696e 7569 7420 6f62  create Minuit ob
+0001dc50: 6a65 6374 2028 6465 7065 6e64 7320 6f6e  ject (depends on
+0001dc60: 204d 696e 7569 7420 7665 7273 696f 6e29   Minuit version)
+0001dc70: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+0001dc80: 656c 662e 696d 696e 7569 745f 7665 7273  elf.iminuit_vers
+0001dc90: 696f 6e20 3c20 2232 223a 0a20 2020 2020  ion < "2":.     
+0001dca0: 2020 2020 2020 2069 6620 7365 6c66 2e71         if self.q
+0001dcb0: 7569 6574 3a0a 2020 2020 2020 2020 2020  uiet:.          
+0001dcc0: 2020 2020 2020 7072 696e 745f 6c65 7665        print_leve
+0001dcd0: 6c20 3d20 300a 2020 2020 2020 2020 2020  l = 0.          
+0001dce0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001dcf0: 2020 2020 2020 2020 7072 696e 745f 6c65          print_le
+0001dd00: 7665 6c20 3d20 310a 2020 2020 2020 2020  vel = 1.        
+0001dd10: 2020 2020 6966 2073 656c 662e 6470 3020      if self.dp0 
+0001dd20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0001dd30: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001dd40: 2069 2c20 706e 616d 2069 6e20 656e 756d   i, pnam in enum
+0001dd50: 6572 6174 6528 7365 6c66 2e70 6e61 6d73  erate(self.pnams
+0001dd60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001dd70: 2020 2020 2020 206d 6f64 656c 5f6b 7761         model_kwa
+0001dd80: 7267 735b 2265 7272 6f72 5f22 202b 2070  rgs["error_" + p
+0001dd90: 6e61 6d5d 203d 2073 656c 662e 6470 305b  nam] = self.dp0[
+0001dda0: 695d 0a20 2020 2020 2020 2020 2020 2069  i].            i
+0001ddb0: 6620 7365 6c66 2e73 6574 4c69 6d69 7473  f self.setLimits
+0001ddc0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0001ddd0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0001dde0: 7220 692c 2070 6e61 6d20 696e 2065 6e75  r i, pnam in enu
+0001ddf0: 6d65 7261 7465 2873 656c 662e 706e 616d  merate(self.pnam
+0001de00: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0001de10: 2020 2020 2020 2020 6d6f 6465 6c5f 6b77          model_kw
+0001de20: 6172 6773 5b22 6c69 6d69 745f 2220 2b20  args["limit_" + 
+0001de30: 706e 616d 5d20 3d20 7365 6c66 2e6c 696d  pnam] = self.lim
+0001de40: 6974 735b 695d 0a20 2020 2020 2020 2020  its[i].         
+0001de50: 2020 2069 6620 7365 6c66 2e66 6978 5061     if self.fixPa
+0001de60: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
+0001de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de80: 666f 7220 692c 2070 6e61 6d20 696e 2065  for i, pnam in e
+0001de90: 6e75 6d65 7261 7465 2873 656c 662e 706e  numerate(self.pn
+0001dea0: 616d 7329 3a0a 2020 2020 2020 2020 2020  ams):.          
+0001deb0: 2020 2020 2020 2020 2020 6d6f 6465 6c5f            model_
+0001dec0: 6b77 6172 6773 5b22 6669 785f 2220 2b20  kwargs["fix_" + 
+0001ded0: 706e 616d 5d20 3d20 7365 6c66 2e66 6978  pnam] = self.fix
+0001dee0: 6564 5061 7273 5b69 5d0a 2020 2020 2020  edPars[i].      
+0001def0: 2020 2020 2020 7365 6c66 2e6d 696e 7569        self.minui
+0001df00: 7420 3d20 4d69 6e75 6974 280a 2020 2020  t = Minuit(.    
+0001df10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001df20: 2e63 6f73 7466 2c0a 2020 2020 2020 2020  .costf,.        
+0001df30: 2020 2020 2020 2020 6572 726f 7264 6566          errordef
+0001df40: 3d73 656c 662e 4572 7244 6566 2c0a 2020  =self.ErrDef,.  
+0001df50: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0001df60: 696e 745f 6c65 7665 6c3d 7072 696e 745f  int_level=print_
+0001df70: 6c65 7665 6c2c 0a20 2020 2020 2020 2020  level,.         
+0001df80: 2020 2020 2020 202a 2a6d 6f64 656c 5f6b         **model_k
+0001df90: 7761 7267 732c 0a20 2020 2020 2020 2020  wargs,.         
+0001dfa0: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
+0001dfb0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0001dfc0: 656c 662e 6d69 6e75 6974 203d 204d 696e  elf.minuit = Min
+0001dfd0: 7569 7428 7365 6c66 2e63 6f73 7466 2c20  uit(self.costf, 
+0001dfe0: 2a6d 6f64 656c 5f6b 7761 7267 732e 7661  *model_kwargs.va
+0001dff0: 6c75 6573 2829 2c20 6e61 6d65 3d73 656c  lues(), name=sel
+0001e000: 662e 706e 616d 7329 0a20 2020 2020 2020  f.pnams).       
+0001e010: 2020 2020 2073 656c 662e 6d69 6e75 6974       self.minuit
+0001e020: 2e65 7272 6f72 6465 6620 3d20 7365 6c66  .errordef = self
+0001e030: 2e45 7272 4465 660a 2020 2020 2020 2020  .ErrDef.        
+0001e040: 2020 2020 6966 2073 656c 662e 7175 6965      if self.quie
+0001e050: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0001e060: 2020 2073 656c 662e 6d69 6e75 6974 2e70     self.minuit.p
+0001e070: 7269 6e74 5f6c 6576 656c 203d 2030 0a20  rint_level = 0. 
+0001e080: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0001e090: 6c66 2e64 7030 2069 7320 6e6f 7420 4e6f  lf.dp0 is not No
+0001e0a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001e0b0: 2020 2020 7365 6c66 2e6d 696e 7569 742e      self.minuit.
+0001e0c0: 6572 726f 7273 203d 2073 656c 662e 6470  errors = self.dp
+0001e0d0: 300a 2020 2020 2020 2020 2020 2020 6966  0.            if
+0001e0e0: 2073 656c 662e 7365 744c 696d 6974 7320   self.setLimits 
+0001e0f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0001e100: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001e110: 662e 6d69 6e75 6974 2e6c 696d 6974 7320  f.minuit.limits 
+0001e120: 3d20 7365 6c66 2e6c 696d 6974 730a 2020  = self.limits.  
+0001e130: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0001e140: 662e 6669 7850 6172 7320 6973 206e 6f74  f.fixPars is not
+0001e150: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001e160: 2020 2020 2020 2066 6f72 2069 2c20 706e         for i, pn
+0001e170: 616d 2069 6e20 656e 756d 6572 6174 6528  am in enumerate(
+0001e180: 7365 6c66 2e70 6e61 6d73 293a 0a20 2020  self.pnams):.   
+0001e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1a0: 2069 6620 7365 6c66 2e66 6978 6564 5061   if self.fixedPa
+0001e1b0: 7273 5b69 5d3a 0a20 2020 2020 2020 2020  rs[i]:.         
+0001e1c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001e1d0: 656c 662e 6d69 6e75 6974 2e66 6978 6564  elf.minuit.fixed
+0001e1e0: 5b70 6e61 6d5d 203d 2054 7275 650a 0a20  [pnam] = True.. 
+0001e1f0: 2020 2064 6566 205f 7374 6f72 6552 6573     def _storeRes
+0001e200: 756c 7428 7365 6c66 293a 0a20 2020 2020  ult(self):.     
+0001e210: 2020 2023 2063 6f6c 6c65 6374 2072 6573     # collect res
+0001e220: 756c 7473 2061 7320 6e75 6d70 7920 6172  ults as numpy ar
+0001e230: 7261 7973 0a20 2020 2020 2020 2023 2021  rays.        # !
+0001e240: 2121 2074 6869 7320 7061 7274 2064 6570  !! this part dep
+0001e250: 656e 6473 206f 6e20 696d 696e 7569 7420  ends on iminuit 
+0001e260: 7665 7273 696f 6e20 2121 210a 2020 2020  version !!!.    
+0001e270: 2020 2020 6d20 3d20 7365 6c66 2e6d 696e      m = self.min
+0001e280: 7569 740a 2020 2020 2020 2020 6d69 6e43  uit.        minC
+0001e290: 6f73 7420 3d20 6d2e 6676 616c 2020 2320  ost = m.fval  # 
+0001e2a0: 6d69 6e69 6d75 6d20 7661 6c75 6520 6f66  minimum value of
+0001e2b0: 2063 6f73 7420 6675 6e63 7469 6f6e 0a20   cost function. 
+0001e2c0: 2020 2020 2020 206e 6670 6172 203d 206d         nfpar = m
+0001e2d0: 2e6e 6669 7420 2023 206e 756d 6572 206f  .nfit  # numer o
+0001e2e0: 6620 6672 6565 2070 6172 616d 6574 6572  f free parameter
+0001e2f0: 730a 2020 2020 2020 2020 6e64 6f66 203d  s.        ndof =
+0001e300: 2073 656c 662e 636f 7374 662e 6e64 6f66   self.costf.ndof
+0001e310: 2020 2320 6465 6772 6565 7320 6f66 2066    # degrees of f
+0001e320: 7265 6564 6f6d 0a20 2020 2020 2020 2069  reedom.        i
+0001e330: 6620 7365 6c66 2e69 6d69 6e75 6974 5f76  f self.iminuit_v
+0001e340: 6572 7369 6f6e 203c 2022 3222 3a0a 2020  ersion < "2":.  
+0001e350: 2020 2020 2020 2020 2020 7061 726e 616d            parnam
+0001e360: 6573 203d 206d 2e76 616c 7565 732e 6b65  es = m.values.ke
+0001e370: 7973 2829 2020 2320 7061 7261 6d65 7465  ys()  # paramete
+0001e380: 7220 6e61 6d65 730a 2020 2020 2020 2020  r names.        
+0001e390: 2020 2020 7061 7276 616c 7320 3d20 6e70      parvals = np
+0001e3a0: 2e61 7361 7272 6179 286d 2e76 616c 7565  .asarray(m.value
+0001e3b0: 732e 7661 6c75 6573 2829 2920 2023 2062  s.values())  # b
+0001e3c0: 6573 742d 6669 7420 7661 6c75 6573 0a20  est-fit values. 
+0001e3d0: 2020 2020 2020 2020 2020 2070 6172 6572             parer
+0001e3e0: 7273 203d 206e 702e 6173 6172 7261 7928  rs = np.asarray(
+0001e3f0: 6d2e 6572 726f 7273 2e76 616c 7565 7328  m.errors.values(
+0001e400: 2929 2020 2320 7061 7261 6d65 7465 7220  ))  # parameter 
+0001e410: 756e 6365 7274 6169 6e74 6965 730a 2020  uncertainties.  
+0001e420: 2020 2020 2020 2020 2020 636f 7620 3d20            cov = 
+0001e430: 6e70 2e61 7272 6179 286d 2e6d 6174 7269  np.array(m.matri
+0001e440: 7828 2929 2020 2320 636f 762e 206d 6174  x())  # cov. mat
+0001e450: 7269 7820 6f66 2066 7265 6520 7061 7261  rix of free para
+0001e460: 6d65 7465 7273 0a20 2020 2020 2020 2065  meters.        e
+0001e470: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001e480: 2023 2076 6572 732e 203e 3d32 2e30 0a20   # vers. >=2.0. 
+0001e490: 2020 2020 2020 2020 2020 2070 6172 6e61             parna
+0001e4a0: 6d65 7320 3d20 6d2e 7061 7261 6d65 7465  mes = m.paramete
+0001e4b0: 7273 2020 2320 7061 7261 6d65 7465 7220  rs  # parameter 
+0001e4c0: 6e61 6d65 730a 2020 2020 2020 2020 2020  names.          
+0001e4d0: 2020 7061 7276 616c 7320 3d20 6e70 2e61    parvals = np.a
+0001e4e0: 7361 7272 6179 286d 2e76 616c 7565 7329  sarray(m.values)
+0001e4f0: 2020 2320 6265 7374 2d66 6974 2076 616c    # best-fit val
+0001e500: 7565 730a 2020 2020 2020 2020 2020 2020  ues.            
+0001e510: 7061 7265 7272 7320 3d20 6e70 2e61 7361  parerrs = np.asa
+0001e520: 7272 6179 286d 2e65 7272 6f72 7329 2020  rray(m.errors)  
+0001e530: 2320 7061 7261 6d65 7465 7220 756e 6365  # parameter unce
+0001e540: 7274 6169 6e74 6965 730a 2020 2020 2020  rtainties.      
+0001e550: 2020 2020 2020 636f 7620 3d20 6e70 2e61        cov = np.a
+0001e560: 7361 7272 6179 286d 2e63 6f76 6172 6961  sarray(m.covaria
+0001e570: 6e63 6529 2020 2320 636f 7661 7269 616e  nce)  # covarian
+0001e580: 6365 206d 6174 7269 7820 6f66 2061 6c6c  ce matrix of all
+0001e590: 2821 2920 7061 7261 6d65 7465 7273 0a20  (!) parameters. 
+0001e5a0: 2020 2020 2020 2020 2020 2023 2070 726f             # pro
+0001e5b0: 6475 6365 2072 6564 7563 6564 2063 6f76  duce reduced cov
+0001e5c0: 6172 6961 6e63 6520 6d61 7472 6978 2066  ariance matrix f
+0001e5d0: 6f72 2066 7265 6520 7061 7261 6d65 7465  or free paramete
+0001e5e0: 7273 206f 6e6c 790a 2020 2020 2020 2020  rs only.        
+0001e5f0: 2020 2020 6966 2073 656c 662e 6e66 6978      if self.nfix
+0001e600: 6564 2021 3d20 303a 0a20 2020 2020 2020  ed != 0:.       
+0001e610: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+0001e620: 6e20 7261 6e67 6528 0a20 2020 2020 2020  n range(.       
+0001e630: 2020 2020 2020 2020 2020 2020 206c 656e               len
+0001e640: 2870 6172 6e61 6d65 7329 202d 2031 2c20  (parnames) - 1, 
+0001e650: 2d31 2c20 2d31 0a20 2020 2020 2020 2020  -1, -1.         
+0001e660: 2020 2020 2020 2029 3a20 2023 2073 7461         ):  # sta
+0001e670: 7274 2066 726f 6d20 6c61 7267 6573 7420  rt from largest 
+0001e680: 696e 6465 7820 616e 6420 776f 726b 2062  index and work b
+0001e690: 6163 6b0a 2020 2020 2020 2020 2020 2020  ack.            
+0001e6a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001e6b0: 6669 7865 6450 6172 735b 695d 3a0a 2020  fixedPars[i]:.  
+0001e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6d0: 2020 2020 2020 636f 7620 3d20 6e70 2e64        cov = np.d
+0001e6e0: 656c 6574 6528 6e70 2e64 656c 6574 6528  elete(np.delete(
+0001e6f0: 636f 762c 2069 2c20 3029 2c20 692c 2031  cov, i, 0), i, 1
+0001e700: 290a 2020 2020 2020 2020 6e70 6172 203d  ).        npar =
+0001e710: 206c 656e 2870 6172 6e61 6d65 7329 2020   len(parnames)  
+0001e720: 2320 6e75 6d62 6572 206f 6620 7061 7261  # number of para
+0001e730: 6d65 7465 7273 0a0a 2020 2020 2020 2020  meters..        
+0001e740: 6966 2073 656c 662e 6d69 6e6f 7352 6573  if self.minosRes
+0001e750: 756c 7420 6973 206e 6f74 204e 6f6e 6520  ult is not None 
+0001e760: 616e 6420 7365 6c66 2e6d 696e 6f73 5f6f  and self.minos_o
+0001e770: 6b3a 0a20 2020 2020 2020 2020 2020 2070  k:.            p
+0001e780: 6d65 7272 7320 3d20 5b5d 0a20 2020 2020  merrs = [].     
+0001e790: 2020 2020 2020 2023 2020 7072 696e 7428         #  print(
+0001e7a0: 224d 494e 4f53 2065 7272 6f72 733a 2229  "MINOS errors:")
+0001e7b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001e7c0: 7365 6c66 2e69 6d69 6e75 6974 5f76 6572  self.iminuit_ver
+0001e7d0: 7369 6f6e 203c 2022 3222 3a0a 2020 2020  sion < "2":.    
+0001e7e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001e7f0: 706e 616d 2069 6e20 6d2e 6d65 7272 6f72  pnam in m.merror
+0001e800: 732e 6b65 7973 2829 3a0a 2020 2020 2020  s.keys():.      
+0001e810: 2020 2020 2020 2020 2020 2020 2020 706d                pm
+0001e820: 6572 7273 2e61 7070 656e 6428 5b6d 2e6d  errs.append([m.m
+0001e830: 6572 726f 7273 5b70 6e61 6d5d 5b32 5d2c  errors[pnam][2],
+0001e840: 206d 2e6d 6572 726f 7273 5b70 6e61 6d5d   m.merrors[pnam]
+0001e850: 5b33 5d5d 290a 2020 2020 2020 2020 2020  [3]]).          
+0001e860: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001e870: 2020 2020 2020 2020 666f 7220 706e 616d          for pnam
+0001e880: 2069 6e20 6d2e 6d65 7272 6f72 732e 6b65   in m.merrors.ke
+0001e890: 7973 2829 3a0a 2020 2020 2020 2020 2020  ys():.          
+0001e8a0: 2020 2020 2020 2020 2020 706d 6572 7273            pmerrs
+0001e8b0: 2e61 7070 656e 6428 5b6d 2e6d 6572 726f  .append([m.merro
+0001e8c0: 7273 5b70 6e61 6d5d 2e6c 6f77 6572 2c20  rs[pnam].lower, 
+0001e8d0: 6d2e 6d65 7272 6f72 735b 706e 616d 5d2e  m.merrors[pnam].
+0001e8e0: 7570 7065 725d 290a 2020 2020 2020 2020  upper]).        
+0001e8f0: 2020 2020 7365 6c66 2e4f 6e65 5369 6749      self.OneSigI
+0001e900: 6e74 6572 7661 6c20 3d20 6e70 2e61 7272  nterval = np.arr
+0001e910: 6179 2870 6d65 7272 7329 0a20 2020 2020  ay(pmerrs).     
+0001e920: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001e930: 2020 2020 2073 656c 662e 4f6e 6553 6967       self.OneSig
+0001e940: 496e 7465 7276 616c 203d 206e 702e 6172  Interval = np.ar
+0001e950: 7261 7928 6c69 7374 287a 6970 282d 7061  ray(list(zip(-pa
+0001e960: 7265 7272 732c 2070 6172 6572 7273 2929  rerrs, parerrs))
+0001e970: 290a 0a20 2020 2020 2020 2023 2066 696e  )..        # fin
+0001e980: 616c 2063 616c 6c20 6f66 2063 6f73 7420  al call of cost 
+0001e990: 6675 6e63 7469 6f6e 2061 7420 6d69 6d69  function at mimi
+0001e9a0: 6e75 6d20 746f 2075 7064 6174 6520 616c  num to update al
+0001e9b0: 6c20 7265 7375 6c74 730a 2020 2020 2020  l results.      
+0001e9c0: 2020 2320 2d20 2073 6967 6e61 6c73 2064    # -  signals d
+0001e9d0: 6174 6120 6f62 6a65 6374 2074 6f20 7374  ata object to st
+0001e9e0: 6f72 6520 6d6f 6465 6c2d 6465 6e64 656e  ore model-denden
+0001e9f0: 7420 756e 6365 7274 6169 6e74 6965 730a  t uncertainties.
+0001ea00: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001ea10: 6461 7461 2069 7320 6e6f 7420 4e6f 6e65  data is not None
+0001ea20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0001ea30: 6c66 2e64 6174 612e 6669 6e61 6c5f 6361  lf.data.final_ca
+0001ea40: 6c6c 203d 2054 7275 650a 2020 2020 2020  ll = True.      
+0001ea50: 2020 2320 2d20 2061 6e64 2063 6f73 7420    # -  and cost 
+0001ea60: 6675 6e63 7469 6f6e 2074 6f20 7374 6f72  function to stor
+0001ea70: 6520 676f 6f64 6e65 7373 2d6f 662d 6669  e goodness-of-fi
+0001ea80: 740a 2020 2020 2020 2020 7365 6c66 2e63  t.        self.c
+0001ea90: 6f73 7466 2e66 696e 616c 5f63 616c 6c20  ostf.final_call 
+0001eaa0: 3d20 5472 7565 0a20 2020 2020 2020 2066  = True.        f
+0001eab0: 7661 6c20 3d20 7365 6c66 2e63 6f73 7466  val = self.costf
+0001eac0: 282a 7061 7276 616c 7329 0a0a 2020 2020  (*parvals)..    
+0001ead0: 2020 2020 2320 7374 6f72 6520 7265 7375      # store resu
+0001eae0: 6c74 7320 6173 2063 6c61 7373 206d 656d  lts as class mem
+0001eaf0: 6265 7273 0a20 2020 2020 2020 2023 2020  bers.        #  
+0001eb00: 2070 6172 616d 6574 6572 206e 616d 6573   parameter names
+0001eb10: 0a20 2020 2020 2020 2073 656c 662e 5061  .        self.Pa
+0001eb20: 7261 6d65 7465 724e 616d 6573 203d 2070  rameterNames = p
+0001eb30: 6172 6e61 6d65 730a 2020 2020 2020 2020  arnames.        
+0001eb40: 2320 2a20 666c 6167 2066 6f72 2066 6978  # * flag for fix
+0001eb50: 6564 2070 6172 616d 6574 6572 7320 696e  ed parameters in
+0001eb60: 2073 656c 662e 6669 7865 6450 6172 730a   self.fixedPars.
+0001eb70: 2020 2020 2020 2020 2320 2a20 6e61 6d65          # * name
+0001eb80: 7320 6f66 2066 7265 6520 7061 7261 6d65  s of free parame
+0001eb90: 7465 7273 2069 6e20 7365 6c66 2e66 7265  ters in self.fre
+0001eba0: 6550 6172 4e61 6d73 0a20 2020 2020 2020  eParNams.       
+0001ebb0: 2023 2020 2063 6869 3220 6174 2062 6573   #   chi2 at bes
+0001ebc0: 742d 6669 7420 706f 696e 7420 2870 6f73  t-fit point (pos
+0001ebd0: 7369 626c 7920 6469 6666 6572 656e 7420  sibly different 
+0001ebe0: 6672 6f6d 206d 696e 436f 7374 290a 2020  from minCost).  
+0001ebf0: 2020 2020 2020 7365 6c66 2e47 6f46 203d        self.GoF =
+0001ec00: 2073 656c 662e 636f 7374 662e 676f 660a   self.costf.gof.
+0001ec10: 2020 2020 2020 2020 2320 2020 7061 7261          #   para
+0001ec20: 6d65 7465 7220 7661 6c75 6573 2061 7420  meter values at 
+0001ec30: 6265 7374 2d66 6974 2070 6f69 6e74 0a20  best-fit point. 
+0001ec40: 2020 2020 2020 2073 656c 662e 5061 7261         self.Para
+0001ec50: 6d65 7465 7256 616c 7565 7320 3d20 6e70  meterValues = np
+0001ec60: 2e61 7272 6179 2870 6172 7661 6c73 2c20  .array(parvals, 
+0001ec70: 636f 7079 3d54 7275 6529 0a20 2020 2020  copy=True).     
+0001ec80: 2020 2073 656c 662e 6672 6565 5061 7256     self.freeParV
+0001ec90: 616c 7320 3d20 6e70 2e61 7272 6179 280a  als = np.array(.
+0001eca0: 2020 2020 2020 2020 2020 2020 5b70 6172              [par
+0001ecb0: 7661 6c73 5b69 5d20 666f 7220 6920 696e  vals[i] for i in
+0001ecc0: 2072 616e 6765 286e 7061 7229 2069 6620   range(npar) if 
+0001ecd0: 6e6f 7420 7365 6c66 2e66 6978 6564 5061  not self.fixedPa
+0001ece0: 7273 5b69 5d5d 0a20 2020 2020 2020 2029  rs[i]].        )
+0001ecf0: 0a20 2020 2020 2020 2073 656c 662e 6672  .        self.fr
+0001ed00: 6565 5061 7245 7272 7320 3d20 6e70 2e61  eeParErrs = np.a
+0001ed10: 7272 6179 280a 2020 2020 2020 2020 2020  rray(.          
+0001ed20: 2020 5b70 6172 6572 7273 5b69 5d20 666f    [parerrs[i] fo
+0001ed30: 7220 6920 696e 2072 616e 6765 286e 7061  r i in range(npa
+0001ed40: 7229 2069 6620 6e6f 7420 7365 6c66 2e66  r) if not self.f
+0001ed50: 6978 6564 5061 7273 5b69 5d5d 0a20 2020  ixedPars[i]].   
+0001ed60: 2020 2020 2029 0a20 2020 2020 2020 2023       ).        #
+0001ed70: 2066 6978 6564 2070 6172 616d 6574 6572   fixed parameter
+0001ed80: 206e 616d 6573 2061 6e64 2076 616c 7565   names and value
+0001ed90: 730a 2020 2020 2020 2020 7365 6c66 2e66  s.        self.f
+0001eda0: 6978 6564 5061 7256 616c 7320 3d20 6e70  ixedParVals = np
+0001edb0: 2e61 7272 6179 280a 2020 2020 2020 2020  .array(.        
+0001edc0: 2020 2020 5b70 6172 7661 6c73 5b69 5d20      [parvals[i] 
+0001edd0: 666f 7220 6920 696e 2072 616e 6765 286e  for i in range(n
+0001ede0: 7061 7229 2069 6620 7365 6c66 2e66 6978  par) if self.fix
+0001edf0: 6564 5061 7273 5b69 5d5d 0a20 2020 2020  edPars[i]].     
+0001ee00: 2020 2029 0a20 2020 2020 2020 2023 202a     ).        # *
+0001ee10: 206e 616d 6573 206f 6620 6669 7865 6420   names of fixed 
+0001ee20: 7061 7261 6d65 7465 7273 2069 6e20 7365  parameters in se
+0001ee30: 6c66 2e66 6978 6564 5061 724e 616d 730a  lf.fixedParNams.
+0001ee40: 2020 2020 2020 2020 2320 2020 6e75 6d62          #   numb
+0001ee50: 6572 206f 6620 6465 6772 6565 7320 6f66  er of degrees of
+0001ee60: 2066 7265 6564 6f6d 0a20 2020 2020 2020   freedom.       
+0001ee70: 2073 656c 662e 4e44 6f46 203d 206e 646f   self.NDoF = ndo
+0001ee80: 660a 2020 2020 2020 2020 2320 2020 7379  f.        #   sy
+0001ee90: 6d6d 6574 7269 6320 756e 6365 7274 6169  mmetric uncertai
+0001eea0: 6e74 6965 730a 2020 2020 2020 2020 7365  nties.        se
+0001eeb0: 6c66 2e4d 6967 7261 6445 7272 6f72 7320  lf.MigradErrors 
+0001eec0: 3d20 6e70 2e61 7272 6179 2870 6172 6572  = np.array(parer
+0001eed0: 7273 2c20 636f 7079 3d54 7275 6529 0a20  rs, copy=True). 
+0001eee0: 2020 2020 2020 2023 2020 2063 6f76 6172         #   covar
+0001eef0: 6961 6e63 6520 616e 6420 636f 7272 656c  iance and correl
+0001ef00: 6174 696f 6e20 6d61 7472 6963 6573 0a20  ation matrices. 
+0001ef10: 2020 2020 2020 2073 656c 662e 436f 7661         self.Cova
+0001ef20: 7269 616e 6365 4d61 7472 6978 203d 206e  rianceMatrix = n
+0001ef30: 702e 6172 7261 7928 636f 762c 2063 6f70  p.array(cov, cop
+0001ef40: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
+0001ef50: 7065 7272 7320 3d20 6e70 2e73 7172 7428  perrs = np.sqrt(
+0001ef60: 6e70 2e64 6961 676f 6e61 6c28 636f 7629  np.diagonal(cov)
+0001ef70: 290a 2020 2020 2020 2020 7365 6c66 2e43  ).        self.C
+0001ef80: 6f72 7265 6c61 7469 6f6e 4d61 7472 6978  orrelationMatrix
+0001ef90: 203d 2063 6f76 202f 206e 702e 6f75 7465   = cov / np.oute
+0001efa0: 7228 7065 7272 732c 2070 6572 7273 290a  r(perrs, perrs).
+0001efb0: 2020 2020 2020 2020 2320 2020 312d 7369          #   1-si
+0001efc0: 676d 6120 2836 3825 2043 4c29 2072 616e  gma (68% CL) ran
+0001efd0: 6765 2069 6e20 7365 6c66 2e4f 6e65 5369  ge in self.OneSi
+0001efe0: 6749 6e74 6572 7661 6c0a 0a20 2020 2020  gInterval..     
+0001eff0: 2020 2023 2062 7569 6c64 2061 2063 6f6e     # build a con
+0001f000: 7665 6e69 656e 7420 7265 7375 6c74 2064  venient result d
+0001f010: 6963 7469 6f6e 6172 790a 2020 2020 2020  ictionary.      
+0001f020: 2020 6966 2073 656c 662e 6e66 6978 6564    if self.nfixed
+0001f030: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+0001f040: 2020 2072 7475 706c 6520 3d20 280a 2020     rtuple = (.  
+0001f050: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001f060: 6c66 2e50 6172 616d 6574 6572 5661 6c75  lf.ParameterValu
+0001f070: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0001f080: 2020 2020 7365 6c66 2e4f 6e65 5369 6749      self.OneSigI
+0001f090: 6e74 6572 7661 6c2c 0a20 2020 2020 2020  nterval,.       
+0001f0a0: 2020 2020 2020 2020 2073 656c 662e 436f           self.Co
+0001f0b0: 7272 656c 6174 696f 6e4d 6174 7269 782c  rrelationMatrix,
+0001f0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f0d0: 2073 656c 662e 476f 462c 0a20 2020 2020   self.GoF,.     
+0001f0e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001f0f0: 5061 7261 6d65 7465 724e 616d 6573 2c0a  ParameterNames,.
+0001f100: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001f110: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001f120: 2020 2020 2020 2020 7274 7570 6c65 203d          rtuple =
+0001f130: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0001f140: 2020 206e 702e 636f 6e63 6174 656e 6174     np.concatenat
+0001f150: 6528 2873 656c 662e 6672 6565 5061 7256  e((self.freeParV
+0001f160: 616c 732c 2073 656c 662e 6669 7865 6450  als, self.fixedP
+0001f170: 6172 5661 6c73 2929 2c0a 2020 2020 2020  arVals)),.      
+0001f180: 2020 2020 2020 2020 2020 7365 6c66 2e4f            self.O
+0001f190: 6e65 5369 6749 6e74 6572 7661 6c2c 0a20  neSigInterval,. 
+0001f1a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001f1b0: 656c 662e 436f 7272 656c 6174 696f 6e4d  elf.CorrelationM
+0001f1c0: 6174 7269 782c 0a20 2020 2020 2020 2020  atrix,.         
+0001f1d0: 2020 2020 2020 2073 656c 662e 476f 462c         self.GoF,
+0001f1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f1f0: 206e 702e 636f 6e63 6174 656e 6174 6528   np.concatenate(
+0001f200: 2873 656c 662e 6672 6565 5061 724e 616d  (self.freeParNam
+0001f210: 732c 2073 656c 662e 6669 7865 6450 6172  s, self.fixedPar
+0001f220: 4e61 6d73 2929 2c0a 2020 2020 2020 2020  Nams)),.        
+0001f230: 2020 2020 290a 2020 2020 2020 2020 6b65      ).        ke
+0001f240: 7973 203d 2028 0a20 2020 2020 2020 2020  ys = (.         
+0001f250: 2020 2022 7061 7261 6d65 7465 7220 7661     "parameter va
+0001f260: 6c75 6573 222c 0a20 2020 2020 2020 2020  lues",.         
+0001f270: 2020 2022 636f 6e66 6964 656e 6365 2069     "confidence i
+0001f280: 6e74 6572 7661 6c73 222c 0a20 2020 2020  ntervals",.     
+0001f290: 2020 2020 2020 2022 636f 7272 656c 6174         "correlat
+0001f2a0: 696f 6e20 6d61 7472 6978 222c 0a20 2020  ion matrix",.   
+0001f2b0: 2020 2020 2020 2020 2022 676f 6f64 6e65           "goodne
+0001f2c0: 7373 2d6f 662d 6669 7422 2c0a 2020 2020  ss-of-fit",.    
+0001f2d0: 2020 2020 2020 2020 2270 6172 616d 6574          "paramet
+0001f2e0: 6572 206e 616d 6573 222c 0a20 2020 2020  er names",.     
+0001f2f0: 2020 2029 0a20 2020 2020 2020 2023 2062     ).        # b
+0001f300: 7569 6c64 2064 6963 7469 6f6e 6172 790a  uild dictionary.
+0001f310: 2020 2020 2020 2020 7365 6c66 2e52 6573          self.Res
+0001f320: 756c 7444 6963 7469 6f6e 6172 7920 3d20  ultDictionary = 
+0001f330: 7b6b 3a20 7274 7570 6c65 5b69 5d20 666f  {k: rtuple[i] fo
+0001f340: 7220 2869 2c20 6b29 2069 6e20 656e 756d  r (i, k) in enum
+0001f350: 6572 6174 6528 6b65 7973 297d 0a0a 2020  erate(keys)}..  
+0001f360: 2020 6465 6620 6765 7452 6573 756c 7428    def getResult(
+0001f370: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+0001f380: 2222 7265 7475 726e 2072 6573 756c 7420  ""return result 
+0001f390: 6469 6374 696f 6e61 7279 2222 220a 2020  dictionary""".  
+0001f3a0: 2020 2020 2020 6966 2073 656c 662e 5265        if self.Re
+0001f3b0: 7375 6c74 4469 6374 696f 6e61 7279 2069  sultDictionary i
+0001f3c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0001f3d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0001f3e0: 656c 662e 5265 7375 6c74 4469 6374 696f  elf.ResultDictio
+0001f3f0: 6e61 7279 0a20 2020 2020 2020 2065 6c73  nary.        els
+0001f400: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0001f410: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
+0001f420: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+0001f430: 2020 2022 2021 2121 206d 6e46 6974 2e67     " !!! mnFit.g
+0001f440: 6574 5265 7375 6c74 3a20 6e6f 2072 6573  etResult: no res
+0001f450: 756c 7473 2061 7661 696c 6162 6c65 202d  ults available -
+0001f460: 2072 756e 2066 6974 2066 6972 7374 220a   run fit first".
+0001f470: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0001f480: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+0001f490: 0a20 2020 2064 6566 2067 6574 4675 6e63  .    def getFunc
+0001f4a0: 7469 6f6e 4572 726f 7228 782c 206d 6f64  tionError(x, mod
+0001f4b0: 656c 2c20 7076 616c 732c 2063 6f76 702c  el, pvals, covp,
+0001f4c0: 2066 6978 6564 5061 7273 293a 0a20 2020   fixedPars):.   
+0001f4d0: 2020 2020 2022 2222 6465 7465 726d 696e       """determin
+0001f4e0: 6520 6572 726f 7220 6f66 206d 6f64 656c  e error of model
+0001f4f0: 2061 7420 780a 0a20 2020 2020 2020 2046   at x..        F
+0001f500: 6f72 6d75 6c61 3a0a 2020 2020 2020 2020  ormula:.        
+0001f510: 2020 4465 6c74 6128 7829 203d 2073 7172    Delta(x) = sqr
+0001f520: 7428 2073 756d 5f69 2c6a 2028 6466 2f64  t( sum_i,j (df/d
+0001f530: 705f 6928 7829 2064 662f 6470 5f6a 2878  p_i(x) df/dp_j(x
+0001f540: 2920 5670 5f69 2c6a 2920 290a 0a20 2020  ) Vp_i,j) )..   
+0001f550: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0001f560: 2020 2020 202a 2078 3a20 7363 616c 6172       * x: scalar
+0001f570: 206f 7220 6e70 2d61 7272 6179 206f 6620   or np-array of 
+0001f580: 7820 7661 6c75 6573 0a20 2020 2020 2020  x values.       
+0001f590: 2020 202a 206d 6f64 656c 3a20 6d6f 6465     * model: mode
+0001f5a0: 6c20 6675 6e63 7469 6f6e 0a20 2020 2020  l function.     
+0001f5b0: 2020 2020 202a 2070 766c 6173 3a20 7061       * pvlas: pa
+0001f5c0: 7261 6d65 7465 7220 7661 6c75 6573 0a20  rameter values. 
+0001f5d0: 2020 2020 2020 2020 202a 2063 6f76 703a           * covp:
+0001f5e0: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
+0001f5f0: 6978 206f 6620 7061 7261 6d65 7465 7273  ix of parameters
+0001f600: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0001f610: 733a 0a20 2020 2020 2020 2020 202a 206d  s:.          * m
+0001f620: 6f64 656c 2075 6e63 6572 7461 696e 7479  odel uncertainty
+0001f630: 2c20 7361 6d65 206c 656e 6774 6820 6173  , same length as
+0001f640: 2078 0a20 2020 2020 2020 2022 2222 0a0a   x.        """..
+0001f650: 2020 2020 2020 2020 2320 6361 6c63 756c          # calcul
+0001f660: 6174 6520 7061 7274 6961 6c20 6465 7269  ate partial deri
+0001f670: 7661 7469 7665 7320 6f66 206d 6f64 656c  vatives of model
+0001f680: 2077 2e72 2e74 2070 6172 616d 6574 6572   w.r.t parameter
+0001f690: 730a 0a20 2020 2020 2020 2023 2020 2070  s..        #   p
+0001f6a0: 6172 616d 6574 6572 2073 7465 7020 7369  arameter step si
+0001f6b0: 7a65 0a20 2020 2020 2020 2064 7020 3d20  ze.        dp = 
+0001f6c0: 302e 3031 202a 206e 702e 7371 7274 286e  0.01 * np.sqrt(n
+0001f6d0: 702e 6469 6167 6f6e 616c 2863 6f76 7029  p.diagonal(covp)
+0001f6e0: 290a 2020 2020 2020 2020 2320 6e75 6d62  ).        # numb
+0001f6f0: 6572 206f 6620 7661 7269 6162 6c65 2070  er of variable p
+0001f700: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+0001f710: 2020 6e76 7061 7220 3d20 6c65 6e28 6470    nvpar = len(dp
+0001f720: 290a 2020 2020 2020 2020 2320 2020 6465  ).        #   de
+0001f730: 7269 7661 7469 7665 2064 662f 6470 5f6a  rivative df/dp_j
+0001f740: 2061 7420 6561 6368 2078 5f69 0a20 2020   at each x_i.   
+0001f750: 2020 2020 2064 6664 7020 3d20 6e70 2e65       dfdp = np.e
+0001f760: 6d70 7479 2828 6e76 7061 722c 206c 656e  mpty((nvpar, len
+0001f770: 2878 2929 290a 2020 2020 2020 2020 705f  (x))).        p_
+0001f780: 706c 7573 203d 206e 702e 6172 7261 7928  plus = np.array(
+0001f790: 7076 616c 732c 2063 6f70 793d 5472 7565  pvals, copy=True
+0001f7a0: 290a 2020 2020 2020 2020 705f 6d69 6e75  ).        p_minu
+0001f7b0: 7320 3d20 6e70 2e61 7272 6179 2870 7661  s = np.array(pva
+0001f7c0: 6c73 2c20 636f 7079 3d54 7275 6529 0a20  ls, copy=True). 
+0001f7d0: 2020 2020 2020 206b 203d 2030 0a20 2020         k = 0.   
+0001f7e0: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
+0001f7f0: 6e67 6528 6c65 6e28 7076 616c 7329 293a  nge(len(pvals)):
+0001f800: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001f810: 6e6f 7420 6669 7865 6450 6172 735b 6a5d  not fixedPars[j]
+0001f820: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001f830: 2020 705f 706c 7573 5b6a 5d20 3d20 7076    p_plus[j] = pv
+0001f840: 616c 735b 6a5d 202b 2064 705b 6b5d 0a20  als[j] + dp[k]. 
+0001f850: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001f860: 5f6d 696e 7573 5b6a 5d20 3d20 7076 616c  _minus[j] = pval
+0001f870: 735b 6a5d 202d 2064 705b 6b5d 0a20 2020  s[j] - dp[k].   
+0001f880: 2020 2020 2020 2020 2020 2020 2064 6664               dfd
+0001f890: 705b 6b5d 203d 2030 2e35 202f 2064 705b  p[k] = 0.5 / dp[
+0001f8a0: 6b5d 202a 2028 6d6f 6465 6c28 782c 202a  k] * (model(x, *
+0001f8b0: 705f 706c 7573 2920 2d20 6d6f 6465 6c28  p_plus) - model(
+0001f8c0: 782c 202a 705f 6d69 6e75 7329 290a 2020  x, *p_minus)).  
+0001f8d0: 2020 2020 2020 2020 2020 2020 2020 705f                p_
+0001f8e0: 706c 7573 5b6a 5d20 3d20 7076 616c 735b  plus[j] = pvals[
+0001f8f0: 6a5d 0a20 2020 2020 2020 2020 2020 2020  j].             
+0001f900: 2020 2070 5f6d 696e 7573 5b6a 5d20 3d20     p_minus[j] = 
+0001f910: 7076 616c 735b 6a5d 0a20 2020 2020 2020  pvals[j].       
+0001f920: 2020 2020 2020 2020 206b 202b 3d20 310a           k += 1.
+0001f930: 2020 2020 2020 2020 2320 2020 7371 7561          #   squa
+0001f940: 7265 206f 6620 756e 6365 7274 6169 6e74  re of uncertaint
+0001f950: 6965 7320 6f6e 2066 756e 6374 696f 6e20  ies on function 
+0001f960: 7661 6c75 6573 0a20 2020 2020 2020 2044  values.        D
+0001f970: 656c 7461 203d 206e 702e 656d 7074 7928  elta = np.empty(
+0001f980: 6c65 6e28 7829 290a 2020 2020 2020 2020  len(x)).        
+0001f990: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+0001f9a0: 656e 2878 2929 3a0a 2020 2020 2020 2020  en(x)):.        
+0001f9b0: 2020 2020 4465 6c74 615b 695d 203d 206e      Delta[i] = n
+0001f9c0: 702e 7375 6d28 6e70 2e6f 7574 6572 2864  p.sum(np.outer(d
+0001f9d0: 6664 705b 3a2c 2069 5d2c 2064 6664 705b  fdp[:, i], dfdp[
+0001f9e0: 3a2c 2069 5d29 202a 2063 6f76 7029 0a20  :, i]) * covp). 
+0001f9f0: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
+0001fa00: 2e73 7172 7428 4465 6c74 6129 0a0a 2020  .sqrt(Delta)..  
+0001fa10: 2020 6465 6620 646f 5f66 6974 2873 656c    def do_fit(sel
+0001fa20: 6629 3a0a 2020 2020 2020 2020 2222 2270  f):.        """p
+0001fa30: 6572 666f 726d 2061 6c6c 206e 6563 6573  erform all neces
+0001fa40: 7361 7279 2073 7465 7073 206f 6620 6669  sary steps of fi
+0001fa50: 7420 7365 7175 656e 6365 2222 220a 2020  t sequence""".  
+0001fa60: 2020 2020 2020 6966 2073 656c 662e 6461        if self.da
+0001fa70: 7461 2069 7320 4e6f 6e65 2061 6e64 2073  ta is None and s
+0001fa80: 656c 662e 6669 745f 7479 7065 2021 3d20  elf.fit_type != 
+0001fa90: 2275 7365 7222 3a0a 2020 2020 2020 2020  "user":.        
+0001faa0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0001fab0: 7272 6f72 2822 2021 2121 206d 6e46 6974  rror(" !!! mnFit
+0001fac0: 3a20 6e6f 2064 6174 6120 6f62 6a65 6374  : no data object
+0001fad0: 2064 6566 696e 6564 202d 2063 616c 6c20   defined - call 
+0001fae0: 696e 6974 5f64 6174 6128 2922 290a 2020  init_data()").  
+0001faf0: 2020 2020 2020 6966 2073 656c 662e 636f        if self.co
+0001fb00: 7374 6620 6973 204e 6f6e 653a 0a20 2020  stf is None:.   
+0001fb10: 2020 2020 2020 2020 2072 6169 7365 2052           raise R
+0001fb20: 756e 7469 6d65 4572 726f 7228 2221 2121  untimeError("!!!
+0001fb30: 206d 6e46 6974 3a20 6e6f 2066 6974 206f   mnFit: no fit o
+0001fb40: 626a 6563 7420 6465 6669 6e65 6420 2d20  bject defined - 
+0001fb50: 6361 6c6c 2069 6e69 745f 6669 7428 2922  call init_fit()"
+0001fb60: 290a 0a20 2020 2020 2020 2023 2073 756d  )..        # sum
+0001fb70: 6d61 7269 7a65 206f 7074 696f 6e73 0a20  marize options. 
+0001fb80: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0001fb90: 6c66 2e71 7569 6574 3a0a 2020 2020 2020  lf.quiet:.      
+0001fba0: 2020 2020 2020 6966 2073 656c 662e 6974        if self.it
+0001fbb0: 6572 6174 6546 6974 3a0a 2020 2020 2020  erateFit:.      
+0001fbc0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0001fbd0: 222a 3d3d 2a20 6d6e 4669 7420 7374 6172  "*==* mnFit star
+0001fbe0: 7469 6e67 2070 7265 2d66 6974 2229 0a20  ting pre-fit"). 
+0001fbf0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001fc00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001fc10: 2070 7269 6e74 2822 2a3d 3d2a 206d 6e46   print("*==* mnF
+0001fc20: 6974 2073 7461 7274 696e 6720 6669 7422  it starting fit"
+0001fc30: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+0001fc40: 696e 7428 2220 204f 7074 696f 6e73 3a22  int("  Options:"
+0001fc50: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0001fc60: 7220 6b65 7920 696e 2073 656c 662e 6f70  r key in self.op
+0001fc70: 7469 6f6e 732e 6b65 7973 2829 3a0a 2020  tions.keys():.  
+0001fc80: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0001fc90: 6c65 7661 6e74 203d 2028 0a20 2020 2020  levant = (.     
+0001fca0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001fcb0: 656c 662e 6f70 7469 6f6e 735b 6b65 795d  elf.options[key]
+0001fcc0: 5b31 5d20 3d3d 2022 616c 6c22 0a20 2020  [1] == "all".   
+0001fcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fce0: 206f 7220 7365 6c66 2e66 6974 5f74 7970   or self.fit_typ
+0001fcf0: 6520 696e 2073 656c 662e 6f70 7469 6f6e  e in self.option
+0001fd00: 735b 6b65 795d 5b31 5d0a 2020 2020 2020  s[key][1].      
+0001fd10: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001fd20: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+0001fd30: 656c 6576 616e 743a 0a20 2020 2020 2020  elevant:.       
+0001fd40: 2020 2020 2020 2020 2020 2020 2069 6f70               iop
+0001fd50: 7420 3d20 7365 6c66 2e6f 7074 696f 6e73  t = self.options
+0001fd60: 5b6b 6579 5d5b 305d 202b 2032 0a20 2020  [key][0] + 2.   
+0001fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fd80: 2070 7269 6e74 2835 202a 2022 2022 202b   print(5 * " " +
+0001fd90: 2022 2d20 222c 2073 656c 662e 6f70 7469   "- ", self.opti
+0001fda0: 6f6e 735b 6b65 795d 5b69 6f70 745d 290a  ons[key][iopt]).
+0001fdb0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0001fdc0: 7428 225c 6e22 290a 0a20 2020 2020 2020  t("\n")..       
+0001fdd0: 2023 2070 6572 666f 726d 2028 696e 6974   # perform (init
+0001fde0: 6961 6c29 2066 6974 0a20 2020 2020 2020  ial) fit.       
+0001fdf0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0001fe00: 2020 7365 6c66 2e6d 6967 7261 6452 6573    self.migradRes
+0001fe10: 756c 7420 3d20 7365 6c66 2e6d 696e 7569  ult = self.minui
+0001fe20: 742e 6d69 6772 6164 2829 2020 2320 6669  t.migrad()  # fi
+0001fe30: 6e64 206d 696e 696d 756d 206f 6620 636f  nd minimum of co
+0001fe40: 7374 2066 756e 6374 696f 6e0a 2020 2020  st function.    
+0001fe50: 2020 2020 2020 2020 7365 6c66 2e6d 6967          self.mig
+0001fe60: 7261 645f 6f6b 203d 2054 7275 650a 2020  rad_ok = True.  
+0001fe70: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+0001fe80: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
+0001fe90: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
+0001fea0: 6772 6164 5f6f 6b20 3d20 4661 6c73 650a  grad_ok = False.
+0001feb0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+0001fec0: 7428 6529 0a20 2020 2020 2020 2020 2020  t(e).           
+0001fed0: 2072 6169 7365 2052 756e 7469 6d65 4572   raise RuntimeEr
+0001fee0: 726f 7228 222a 3d3d 2a20 2121 2120 6669  ror("*==* !!! fi
+0001fef0: 7420 7769 7468 206d 6967 7261 6420 6661  t with migrad fa
+0001ff00: 696c 6564 2229 0a0a 2020 2020 2020 2020  iled")..        
+0001ff10: 2320 706f 7373 6962 6c79 2c20 6e65 6564  # possibly, need
+0001ff20: 2074 6f20 6974 6572 6174 650a 2020 2020   to iterate.    
+0001ff30: 2020 2020 6966 2073 656c 662e 6974 6572      if self.iter
+0001ff40: 6174 6546 6974 3a0a 2020 2020 2020 2020  ateFit:.        
+0001ff50: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+0001ff60: 7175 6965 743a 0a20 2020 2020 2020 2020  quiet:.         
+0001ff70: 2020 2020 2020 2070 7269 6e74 280a 2020         print(.  
+0001ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff90: 2020 222a 3d3d 2a20 6d6e 4669 7420 6974    "*==* mnFit it
+0001ffa0: 6572 6174 696e 6722 2c0a 2020 2020 2020  erating",.      
+0001ffb0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+0001ffc0: 6f20 6163 636f 756e 7420 666f 7220 7061  o account for pa
+0001ffd0: 7261 6d65 7465 722d 6465 7065 6e64 656e  rameter-dependen
+0001ffe0: 7420 756e 6365 7274 6169 6e74 6965 7322  t uncertainties"
+0001fff0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00020000: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00020010: 2320 656e 6162 6c65 2064 796e 616d 6963  # enable dynamic
+00020020: 2063 616c 6375 6c61 7469 6f6e 206f 6620   calculation of 
+00020030: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+00020040: 780a 2020 2020 2020 2020 2020 2020 7365  x.            se
+00020050: 6c66 2e64 6174 612e 696e 6974 5f64 796e  lf.data.init_dyn
+00020060: 616d 6963 4572 726f 7273 2829 0a0a 2020  amicErrors()..  
+00020070: 2020 2020 2020 2020 2020 2320 6669 7420            # fit 
+00020080: 7769 7468 2064 796e 616d 6963 2072 6563  with dynamic rec
+00020090: 616c 6375 6c61 7469 6f6e 206f 6620 636f  alculation of co
+000200a0: 7661 7269 616e 6365 206d 6174 7269 780a  variance matrix.
+000200b0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+000200c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000200d0: 2073 656c 662e 6d69 6772 6164 5265 7375   self.migradResu
+000200e0: 6c74 203d 2073 656c 662e 6d69 6e75 6974  lt = self.minuit
+000200f0: 2e6d 6967 7261 6428 290a 2020 2020 2020  .migrad().      
+00020100: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00020110: 6967 7261 645f 6f6b 203d 2054 7275 650a  igrad_ok = True.
+00020120: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00020130: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00020140: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00020150: 2020 2073 656c 662e 6d69 6772 6164 5f6f     self.migrad_o
+00020160: 6b20 3d20 4661 6c73 650a 2020 2020 2020  k = False.      
+00020170: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00020180: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00020190: 2020 2072 6169 7365 2052 756e 7469 6d65     raise Runtime
+000201a0: 4572 726f 7228 222a 3d3d 2a20 2121 2120  Error("*==* !!! 
+000201b0: 6974 6572 6174 696f 6e20 6f66 2066 6974  iteration of fit
+000201c0: 2077 6974 6820 6d69 6772 6164 2066 6169   with migrad fai
+000201d0: 6c65 6422 290a 0a20 2020 2020 2020 2023  led")..        #
+000201e0: 2072 756e 2070 726f 6669 6c65 206c 696b   run profile lik
+000201f0: 656c 6968 6f6f 6420 7363 616e 2074 6f20  elihood scan to 
+00020200: 6368 6563 6b20 666f 7220 6173 796d 6d65  check for asymme
+00020210: 7472 6963 2065 7272 6f72 730a 2020 2020  tric errors.    
+00020220: 2020 2020 6966 2073 656c 662e 7275 6e5f      if self.run_
+00020230: 6d69 6e6f 733a 0a20 2020 2020 2020 2020  minos:.         
+00020240: 2020 2069 6620 6e6f 7420 7365 6c66 2e71     if not self.q
+00020250: 7569 6574 3a0a 2020 2020 2020 2020 2020  uiet:.          
+00020260: 2020 2020 2020 7072 696e 7428 222a 3d3d        print("*==
+00020270: 2a20 6d6e 4669 7420 7374 6172 7469 6e67  * mnFit starting
+00020280: 206d 696e 6f73 2073 6361 6e22 290a 2020   minos scan").  
+00020290: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+000202a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000202b0: 656c 662e 6d69 6e6f 7352 6573 756c 7420  elf.minosResult 
+000202c0: 3d20 7365 6c66 2e6d 696e 7569 742e 6d69  = self.minuit.mi
+000202d0: 6e6f 7328 290a 2020 2020 2020 2020 2020  nos().          
+000202e0: 2020 2020 2020 7365 6c66 2e6d 696e 6f73        self.minos
+000202f0: 5f6f 6b20 3d20 5472 7565 0a20 2020 2020  _ok = True.     
+00020300: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00020310: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00020320: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00020330: 6c66 2e6d 696e 6f73 5f6f 6b20 3d20 4661  lf.minos_ok = Fa
+00020340: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00020350: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00020360: 7175 6965 743a 0a20 2020 2020 2020 2020  quiet:.         
+00020370: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00020380: 2822 2a3d 3d2a 206d 6e46 6974 3a20 2121  ("*==* mnFit: !!
+00020390: 2120 6d69 6e6f 7320 6661 696c 6564 205c  ! minos failed \
+000203a0: 6e22 2c20 6529 0a20 2020 2020 2020 2073  n", e).        s
+000203b0: 656c 662e 5f73 746f 7265 5265 7375 6c74  elf._storeResult
+000203c0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+000203d0: 6e20 7365 6c66 2e6d 6967 7261 6452 6573  n self.migradRes
+000203e0: 756c 742c 2073 656c 662e 6d69 6e6f 7352  ult, self.minosR
+000203f0: 6573 756c 740a 0a20 2020 2064 6566 2073  esult..    def s
+00020400: 6574 506c 6f74 4f70 7469 6f6e 7328 7365  etPlotOptions(se
+00020410: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+00020420: 5365 7420 6f70 7469 6f6e 7320 666f 7220  Set options for 
+00020430: 6e69 6365 7220 706c 6f74 7469 6e67 2222  nicer plotting""
+00020440: 220a 0a20 2020 2020 2020 2023 2074 6f20  "..        # to 
+00020450: 6265 2069 6d70 6c65 6d65 6e74 6564 0a20  be implemented. 
+00020460: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00020470: 2064 6566 2070 6c6f 744d 6f64 656c 280a   def plotModel(.
+00020480: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00020490: 2020 2020 2020 6178 6973 5f6c 6162 656c        axis_label
+000204a0: 733d 5b22 7822 2c20 2279 203d 2066 2878  s=["x", "y = f(x
+000204b0: 2c20 2a70 6172 2922 5d2c 0a20 2020 2020  , *par)"],.     
+000204c0: 2020 2064 6174 615f 6c65 6765 6e64 3d22     data_legend="
+000204d0: 6461 7461 222c 0a20 2020 2020 2020 206d  data",.        m
+000204e0: 6f64 656c 5f6c 6567 656e 643d 2266 6974  odel_legend="fit
+000204f0: 222c 0a20 2020 2020 2020 2070 6c6f 745f  ",.        plot_
+00020500: 6261 6e64 3d54 7275 652c 0a20 2020 2020  band=True,.     
+00020510: 2020 2073 616d 655f 706c 6f74 3d46 616c     same_plot=Fal
+00020520: 7365 2c0a 2020 2020 2020 2020 706c 6f74  se,.        plot
+00020530: 5f72 6573 6964 7561 6c3d 4661 6c73 652c  _residual=False,
+00020540: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00020550: 2222 220a 2020 2020 2020 2020 506c 6f74  """.        Plot
+00020560: 206d 6f64 656c 2066 756e 6374 696f 6e20   model function 
+00020570: 616e 6420 6461 7461 0a0a 2020 2020 2020  and data..      
+00020580: 2020 5573 6573 2069 6d69 6e75 6974 4f62    Uses iminuitOb
+00020590: 6a65 6374 2c20 636f 7374 2046 756e 6374  ject, cost Funct
+000205a0: 696f 6e20 2861 6e64 2064 6174 6120 6f62  ion (and data ob
+000205b0: 6a65 6374 290a 0a20 2020 2020 2020 2041  ject)..        A
+000205c0: 7267 733a 0a20 2020 2020 2020 2020 202a  rgs:.          *
+000205d0: 206c 6973 7420 6f66 2073 7472 3a20 6178   list of str: ax
+000205e0: 6973 206c 6162 656c 730a 2020 2020 2020  is labels.      
+000205f0: 2020 2020 2a20 7374 723a 206c 6567 656e      * str: legen
+00020600: 6420 666f 7220 6461 7461 0a20 2020 2020  d for data.     
+00020610: 2020 2020 202a 2073 7472 3a20 6c65 6765       * str: lege
+00020620: 6e64 2066 6f72 206d 6f64 656c 0a20 2020  nd for model.   
+00020630: 2020 2020 2020 202a 2070 6c6f 745f 6261         * plot_ba
+00020640: 6e64 3a20 706c 6f74 206d 6f64 656c 2063  nd: plot model c
+00020650: 6f6e 6669 6465 6e63 6520 6261 6e64 2069  onfidence band i
+00020660: 6620 5472 7565 0a20 2020 2020 2020 2020  f True.         
+00020670: 202a 2073 616d 655f 706c 6f74 3a20 6163   * same_plot: ac
+00020680: 6375 6d75 6c61 7465 2066 6974 2072 6573  cumulate fit res
+00020690: 756c 7473 2066 726f 6d20 7072 6576 696f  ults from previo
+000206a0: 7573 2063 616c 6c20 6966 2054 7275 650a  us call if True.
+000206b0: 2020 2020 2020 2020 2020 2a20 706c 6f74            * plot
+000206c0: 5f72 6573 6964 7561 6c3a 2070 6c6f 7420  _residual: plot 
+000206d0: 7265 7369 6475 616c 2077 2e72 2e74 2e20  residual w.r.t. 
+000206e0: 6d6f 6465 6c20 6966 2054 7275 650a 0a20  model if True.. 
+000206f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00020700: 2020 2020 2020 2020 2020 2a20 6d61 7470            * matp
+00020710: 6c6f 746c 6962 2066 6967 7572 650a 2020  lotlib figure.  
+00020720: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00020730: 2020 2023 2061 6363 6573 7320 6f62 6a65     # access obje
+00020740: 6374 730a 2020 2020 2020 2020 6d20 3d20  cts.        m = 
+00020750: 7365 6c66 2e6d 696e 7569 7420 2023 206d  self.minuit  # m
+00020760: 696e 7569 7420 6f62 6a65 6374 0a20 2020  inuit object.   
+00020770: 2020 2020 2063 6620 3d20 7365 6c66 2e63       cf = self.c
+00020780: 6f73 7466 2020 2320 636f 7374 2066 756e  ostf  # cost fun
+00020790: 6374 696f 6e20 6f62 6a65 6374 0a20 2020  ction object.   
+000207a0: 2020 2020 2064 203d 2063 662e 6461 7461       d = cf.data
+000207b0: 0a20 2020 2020 2020 206e 7074 7320 3d20  .        npts = 
+000207c0: 6d61 7828 3139 302c 2035 202a 2064 2e64  max(190, 5 * d.d
+000207d0: 6c65 6e67 7468 2920 2023 206e 756d 6265  length)  # numbe
+000207e0: 7220 6f66 2070 6f69 6e74 7320 666f 7220  r of points for 
+000207f0: 6d6f 6465 6c20 6675 6e63 7469 6f6e 0a0a  model function..
+00020800: 2020 2020 2020 2020 2320 7265 7472 6965          # retrie
+00020810: 7665 2066 6974 2072 6573 756c 7473 0a20  ve fit results. 
+00020820: 2020 2020 2020 2070 6e61 6d73 203d 2073         pnams = s
+00020830: 656c 662e 5061 7261 6d65 7465 724e 616d  elf.ParameterNam
+00020840: 6573 0a20 2020 2020 2020 2070 7661 6c73  es.        pvals
+00020850: 203d 2073 656c 662e 5061 7261 6d65 7465   = self.Paramete
+00020860: 7256 616c 7565 730a 2020 2020 2020 2020  rValues.        
+00020870: 706d 6572 7273 203d 2073 656c 662e 4f6e  pmerrs = self.On
+00020880: 6553 6967 496e 7465 7276 616c 0a20 2020  eSigInterval.   
+00020890: 2020 2020 2023 2020 7379 6d6d 6574 7269       #  symmetri
+000208a0: 6320 6572 726f 7273 0a20 2020 2020 2020  c errors.       
+000208b0: 2070 6572 7273 203d 2028 706d 6572 7273   perrs = (pmerrs
+000208c0: 5b3a 2c20 315d 202d 2070 6d65 7272 735b  [:, 1] - pmerrs[
+000208d0: 3a2c 2030 5d29 202f 2032 2e30 0a20 2020  :, 0]) / 2.0.   
+000208e0: 2020 2020 2063 6f72 203d 2073 656c 662e       cor = self.
+000208f0: 436f 7272 656c 6174 696f 6e4d 6174 7269  CorrelationMatri
+00020900: 780a 2020 2020 2020 2020 2320 2063 6f76  x.        #  cov
+00020910: 6172 6961 6e63 6520 6d61 7472 6978 2066  ariance matrix f
+00020920: 726f 6d20 636f 7272 656c 6174 696f 6e73  rom correlations
+00020930: 0a20 2020 2020 2020 2070 636f 7620 3d20  .        pcov = 
+00020940: 636f 7220 2a20 6e70 2e6f 7574 6572 2870  cor * np.outer(p
+00020950: 6572 7273 2c20 7065 7272 7329 0a20 2020  errs, perrs).   
+00020960: 2020 2020 2067 6f66 203d 2073 656c 662e       gof = self.
+00020970: 476f 460a 2020 2020 2020 2020 6e64 6f66  GoF.        ndof
+00020980: 203d 2063 662e 6e64 6f66 0a20 2020 2020   = cf.ndof.     
+00020990: 2020 2023 2020 6368 6932 7072 620a 2020     #  chi2prb.  
+000209a0: 2020 2020 2020 6966 2067 6f66 2069 7320        if gof is 
+000209b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000209c0: 2020 2020 2020 6368 6932 7072 6220 3d20        chi2prb = 
+000209d0: 7365 6c66 2e63 6869 3270 7262 2867 6f66  self.chi2prb(gof
+000209e0: 2c20 6e64 6f66 290a 2020 2020 2020 2020  , ndof).        
+000209f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00020a00: 2020 6368 6932 7072 6220 3d20 4e6f 6e65    chi2prb = None
+00020a10: 0a20 2020 2020 2020 2023 2076 616c 7565  .        # value
+00020a20: 7320 6f66 2066 7265 6520 616e 6420 6669  s of free and fi
+00020a30: 7865 6420 7061 7261 6d65 7465 7273 0a20  xed parameters. 
+00020a40: 2020 2020 2020 2066 6978 6564 5061 7273         fixedPars
+00020a50: 203d 2073 656c 662e 6669 7865 6450 6172   = self.fixedPar
+00020a60: 730a 2020 2020 2020 2020 6672 6565 5f70  s.        free_p
+00020a70: 7661 6c73 203d 2073 656c 662e 6672 6565  vals = self.free
+00020a80: 5061 7256 616c 730a 2020 2020 2020 2020  ParVals.        
+00020a90: 6672 6565 5f70 6e61 6d73 203d 2073 656c  free_pnams = sel
+00020aa0: 662e 6672 6565 5061 724e 616d 730a 2020  f.freeParNams.  
+00020ab0: 2020 2020 2020 6669 7865 645f 706e 616d        fixed_pnam
+00020ac0: 7320 3d20 7365 6c66 2e66 6978 6564 5061  s = self.fixedPa
+00020ad0: 724e 616d 730a 2020 2020 2020 2020 6669  rNams.        fi
+00020ae0: 7865 645f 7076 616c 7320 3d20 7365 6c66  xed_pvals = self
+00020af0: 2e66 6978 6564 5061 7256 616c 730a 2020  .fixedParVals.  
+00020b00: 2020 2020 2020 6e66 6978 6564 203d 206c        nfixed = l
+00020b10: 656e 2866 6978 6564 5f70 7661 6c73 290a  en(fixed_pvals).
+00020b20: 0a20 2020 2020 2020 2023 2070 6c6f 7420  .        # plot 
+00020b30: 6461 7461 0a20 2020 2020 2020 2066 6967  data.        fig
+00020b40: 5f6d 6f64 656c 203d 2064 2e70 6c6f 7428  _model = d.plot(
+00020b50: 0a20 2020 2020 2020 2020 2020 2066 6967  .            fig
+00020b60: 7369 7a65 3d28 372e 352c 2036 2e35 292c  size=(7.5, 6.5),
+00020b70: 2064 6174 615f 6c61 6265 6c3d 6461 7461   data_label=data
+00020b80: 5f6c 6567 656e 642c 2070 6c6f 745f 7265  _legend, plot_re
+00020b90: 7369 6475 616c 3d70 6c6f 745f 7265 7369  sidual=plot_resi
+00020ba0: 6475 616c 0a20 2020 2020 2020 2029 0a0a  dual.        )..
+00020bb0: 2020 2020 2020 2020 2320 6f76 6572 6c61          # overla
+00020bc0: 7920 6d6f 6465 6c20 6675 6e63 7469 6f6e  y model function
+00020bd0: 0a20 2020 2020 2020 2023 2068 6973 746f  .        # histo
+00020be0: 6772 616d 2066 6974 2070 726f 7669 6465  gram fit provide
+00020bf0: 7320 6e6f 726d 616c 6973 6564 2064 6973  s normalised dis
+00020c00: 7472 6962 7574 696f 6e2c 0a20 2020 2020  tribution,.     
+00020c10: 2020 2023 2020 2020 6465 7465 726d 696e     #    determin
+00020c20: 6520 6269 6e20 7769 6474 6873 2061 6e64  e bin widths and
+00020c30: 2073 6361 6c65 2066 6163 746f 720a 2020   scale factor.  
+00020c40: 2020 2020 2020 786d 696e 2c20 786d 6178        xmin, xmax
+00020c50: 203d 2070 6c74 2e78 6c69 6d28 290a 2020   = plt.xlim().  
+00020c60: 2020 2020 2020 7870 6c74 203d 206e 702e        xplt = np.
+00020c70: 6c69 6e73 7061 6365 2878 6d69 6e2c 2078  linspace(xmin, x
+00020c80: 6d61 782c 206e 7074 7329 0a20 2020 2020  max, npts).     
+00020c90: 2020 2078 7661 6c73 203d 2078 706c 740a     xvals = xplt.
+00020ca0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00020cb0: 6669 745f 7479 7065 203d 3d20 2268 6973  fit_type == "his
+00020cc0: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
+00020cd0: 2320 6465 7465 6d69 6e65 206c 6f63 616c  # detemine local
+00020ce0: 2062 696e 2077 6964 7468 0a20 2020 2020   bin width.     
+00020cf0: 2020 2020 2020 2062 7769 6474 6873 203d         bwidths =
+00020d00: 206e 702e 7a65 726f 7328 6c65 6e28 7870   np.zeros(len(xp
+00020d10: 6c74 2929 0a20 2020 2020 2020 2020 2020  lt)).           
+00020d20: 2069 203d 2030 0a20 2020 2020 2020 2020   i = 0.         
+00020d30: 2020 2066 6f72 206a 2c20 7820 696e 2065     for j, x in e
+00020d40: 6e75 6d65 7261 7465 2878 706c 7429 3a0a  numerate(xplt):.
+00020d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d60: 6966 2078 203e 3d20 6366 2e64 6174 612e  if x >= cf.data.
+00020d70: 7269 6768 7473 5b6d 696e 2869 2c20 6366  rights[min(i, cf
+00020d80: 2e64 6174 612e 6e62 696e 7320 2d20 3129  .data.nbins - 1)
+00020d90: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00020da0: 2020 2020 2020 2069 202b 3d20 310a 2020         i += 1.  
+00020db0: 2020 2020 2020 2020 2020 2020 2020 6277                bw
+00020dc0: 6964 7468 735b 6a5d 203d 2063 662e 6461  idths[j] = cf.da
+00020dd0: 7461 2e77 6964 7468 735b 6d69 6e28 692c  ta.widths[min(i,
+00020de0: 2063 662e 6461 7461 2e6e 6269 6e73 202d   cf.data.nbins -
+00020df0: 2031 295d 0a20 2020 2020 2020 2020 2020   1)].           
+00020e00: 2073 6661 6320 3d20 6366 2e6e 6f72 6d20   sfac = cf.norm 
+00020e10: 2a20 6277 6964 7468 730a 2020 2020 2020  * bwidths.      
+00020e20: 2020 656c 6966 2073 656c 662e 6669 745f    elif self.fit_
+00020e30: 7479 7065 203d 3d20 2278 7922 206f 7220  type == "xy" or 
+00020e40: 7365 6c66 2e66 6974 5f74 7970 6520 3d3d  self.fit_type ==
+00020e50: 2022 6d6c 223a 0a20 2020 2020 2020 2020   "ml":.         
+00020e60: 2020 2073 6661 6320 3d20 312e 300a 2020     sfac = 1.0.  
+00020e70: 2020 2020 2020 656c 6966 2073 656c 662e        elif self.
+00020e80: 6669 745f 7479 7065 203d 3d20 2269 6e64  fit_type == "ind
+00020e90: 6578 6564 223a 0a20 2020 2020 2020 2020  exed":.         
+00020ea0: 2020 2073 6661 6320 3d20 312e 300a 2020     sfac = 1.0.  
+00020eb0: 2020 2020 2020 2020 2020 7876 616c 7320            xvals 
+00020ec0: 3d20 6366 2e64 6174 612e 780a 2020 2020  = cf.data.x.    
+00020ed0: 2020 2020 2020 2020 7870 6c74 203d 206e          xplt = n
+00020ee0: 702e 6c69 6e73 7061 6365 2830 2e35 2c20  p.linspace(0.5, 
+00020ef0: 6c65 6e28 7876 616c 7329 202d 2030 2e35  len(xvals) - 0.5
+00020f00: 2c20 6c65 6e28 7876 616c 7329 290a 2020  , len(xvals)).  
+00020f10: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00020f20: 2020 2020 2020 2020 7072 696e 7428 2221          print("!
+00020f30: 2a2a 2120 6d6e 4669 742e 706c 6f74 4d6f  **! mnFit.plotMo
+00020f40: 6465 6c3a 2075 6e6b 6e6f 776e 2066 6974  del: unknown fit
+00020f50: 2074 7970 653a 2022 2c20 7365 6c66 2e66   type: ", self.f
+00020f60: 6974 5f74 7970 6529 0a20 2020 2020 2020  it_type).       
+00020f70: 2020 2020 2073 6661 6320 3d20 312e 300a       sfac = 1.0.
+00020f80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00020f90: 726e 0a0a 2020 2020 2020 2020 2320 646f  rn..        # do
+00020fa0: 2077 6520 7761 6e74 206d 6f64 656c 206f   we want model o
+00020fb0: 7220 7265 7369 6475 616c 7320 3f0a 2020  r residuals ?.  
+00020fc0: 2020 2020 2020 6966 2070 6c6f 745f 7265        if plot_re
+00020fd0: 7369 6475 616c 3a0a 2020 2020 2020 2020  sidual:.        
+00020fe0: 2020 2020 7970 6c74 203d 206e 702e 7a65      yplt = np.ze
+00020ff0: 726f 7328 6c65 6e28 7870 6c74 2929 0a20  ros(len(xplt)). 
+00021000: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00021010: 2020 2020 2020 2020 2079 706c 7420 3d20           yplt = 
+00021020: 6366 2e6d 6f64 656c 2878 7661 6c73 2c20  cf.model(xvals, 
+00021030: 2a70 7661 6c73 290a 0a20 2020 2020 2020  *pvals)..       
+00021040: 2023 2020 706c 6f74 206d 6f64 656c 206c   #  plot model l
+00021050: 696e 650a 2020 2020 2020 2020 6966 2073  ine.        if s
+00021060: 656c 662e 6669 745f 7479 7065 203d 3d20  elf.fit_type == 
+00021070: 2269 6e64 6578 6564 223a 0a20 2020 2020  "indexed":.     
+00021080: 2020 2020 2020 2070 6c74 2e65 7272 6f72         plt.error
+00021090: 6261 7228 0a20 2020 2020 2020 2020 2020  bar(.           
+000210a0: 2020 2020 2078 706c 742c 0a20 2020 2020       xplt,.     
+000210b0: 2020 2020 2020 2020 2020 2079 706c 742c             yplt,
+000210c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000210d0: 2066 6d74 3d22 2022 2c0a 2020 2020 2020   fmt=" ",.      
+000210e0: 2020 2020 2020 2020 2020 7865 7272 3d30            xerr=0
+000210f0: 2e34 2c0a 2020 2020 2020 2020 2020 2020  .4,.            
+00021100: 2020 2020 6c61 6265 6c3d 6d6f 6465 6c5f      label=model_
+00021110: 6c65 6765 6e64 2c0a 2020 2020 2020 2020  legend,.        
+00021120: 2020 2020 2020 2020 616c 7068 613d 302e          alpha=0.
+00021130: 372c 0a20 2020 2020 2020 2020 2020 2020  7,.             
+00021140: 2020 2065 6c69 6e65 7769 6474 683d 322e     elinewidth=2.
+00021150: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
+00021160: 2020 2063 6f6c 6f72 3d22 6461 726b 6f72     color="darkor
+00021170: 616e 6765 222c 0a20 2020 2020 2020 2020  ange",.         
+00021180: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
+00021190: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+000211a0: 6c74 2e70 6c6f 7428 0a20 2020 2020 2020  lt.plot(.       
+000211b0: 2020 2020 2020 2020 2078 706c 742c 0a20           xplt,. 
+000211c0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+000211d0: 706c 7420 2a20 7366 6163 2c0a 2020 2020  plt * sfac,.    
+000211e0: 2020 2020 2020 2020 2020 2020 6c61 6265              labe
+000211f0: 6c3d 6d6f 6465 6c5f 6c65 6765 6e64 2c0a  l=model_legend,.
+00021200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021210: 6c69 6e65 7374 796c 653d 2264 6173 6865  linestyle="dashe
+00021220: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+00021230: 2020 2020 6c69 6e65 7769 6474 683d 322e      linewidth=2.
+00021240: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
+00021250: 2020 2061 6c70 6861 3d30 2e37 2c0a 2020     alpha=0.7,.  
+00021260: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00021270: 2020 2020 2323 2020 2020 2020 2020 2020      ##          
+00021280: 636f 6c6f 723d 2764 6172 6b6f 7261 6e67  color='darkorang
+00021290: 6527 290a 2020 2020 2020 2020 706c 742e  e').        plt.
+000212a0: 786c 6162 656c 2861 7869 735f 6c61 6265  xlabel(axis_labe
+000212b0: 6c73 5b30 5d2c 2073 697a 653d 2278 2d6c  ls[0], size="x-l
+000212c0: 6172 6765 2229 0a20 2020 2020 2020 2070  arge").        p
+000212d0: 6c74 2e79 6c61 6265 6c28 6178 6973 5f6c  lt.ylabel(axis_l
+000212e0: 6162 656c 735b 315d 2c20 7369 7a65 3d22  abels[1], size="
+000212f0: 782d 6c61 7267 6522 290a 2020 2020 2020  x-large").      
+00021300: 2020 706c 742e 6772 6964 2829 0a0a 2020    plt.grid()..  
+00021310: 2020 2020 2020 2320 6472 6177 2065 7272        # draw err
+00021320: 6f72 2062 616e 6420 6172 6f75 6e64 206d  or band around m
+00021330: 6f64 656c 2066 756e 6374 696f 6e0a 2020  odel function.  
+00021340: 2020 2020 2020 6966 2070 6c6f 745f 6261        if plot_ba
+00021350: 6e64 3a0a 2020 2020 2020 2020 2020 2020  nd:.            
+00021360: 6966 2073 656c 662e 6669 745f 7479 7065  if self.fit_type
+00021370: 2021 3d20 2269 6e64 6578 6564 223a 0a20   != "indexed":. 
+00021380: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+00021390: 656c 7461 4620 3d20 7365 6c66 2e67 6574  eltaF = self.get
+000213a0: 4675 6e63 7469 6f6e 4572 726f 7228 7870  FunctionError(xp
+000213b0: 6c74 2c20 6366 2e6d 6f64 656c 2c20 7076  lt, cf.model, pv
+000213c0: 616c 732c 2070 636f 762c 2066 6978 6564  als, pcov, fixed
+000213d0: 5061 7273 290a 2020 2020 2020 2020 2020  Pars).          
+000213e0: 2020 2020 2020 706c 742e 6669 6c6c 5f62        plt.fill_b
+000213f0: 6574 7765 656e 280a 2020 2020 2020 2020  etween(.        
+00021400: 2020 2020 2020 2020 2020 2020 7870 6c74              xplt
+00021410: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021420: 2020 2020 2020 7366 6163 202a 2028 7970        sfac * (yp
+00021430: 6c74 202b 2044 656c 7461 4629 2c0a 2020  lt + DeltaF),.  
+00021440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021450: 2020 7366 6163 202a 2028 7970 6c74 202d    sfac * (yplt -
+00021460: 2044 656c 7461 4629 2c0a 2020 2020 2020   DeltaF),.      
+00021470: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00021480: 7068 613d 302e 332c 0a20 2020 2020 2020  pha=0.3,.       
+00021490: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+000214a0: 6f72 3d22 6461 726b 6b68 616b 6922 2c0a  or="darkkhaki",.
+000214b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000214c0: 2020 2020 6c61 6265 6c3d 2220 2024 5c70      label="  $\p
+000214d0: 6d20 3120 5c73 6967 6d61 2422 2c0a 2020  m 1 \sigma$",.  
+000214e0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000214f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021500: 706c 742e 706c 6f74 280a 2020 2020 2020  plt.plot(.      
+00021510: 2020 2020 2020 2020 2020 2020 2020 7870                xp
+00021520: 6c74 2c0a 2020 2020 2020 2020 2020 2020  lt,.            
+00021530: 2020 2020 2020 2020 7366 6163 202a 2028          sfac * (
+00021540: 7970 6c74 202b 2044 656c 7461 4629 2c0a  yplt + DeltaF),.
+00021550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021560: 2020 2020 6c69 6e65 7769 6474 683d 312c      linewidth=1,
+00021570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021580: 2020 2020 2061 6c70 6861 3d30 2e34 2c0a       alpha=0.4,.
+00021590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000215a0: 2020 2020 636f 6c6f 723d 2264 6172 6b67      color="darkg
+000215b0: 7265 656e 222c 0a20 2020 2020 2020 2020  reen",.         
+000215c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000215d0: 2020 2020 2020 2020 2070 6c74 2e70 6c6f           plt.plo
+000215e0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+000215f0: 2020 2020 2020 2078 706c 742c 0a20 2020         xplt,.   
+00021600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021610: 2073 6661 6320 2a20 2879 706c 7420 2d20   sfac * (yplt - 
+00021620: 4465 6c74 6146 292c 0a20 2020 2020 2020  DeltaF),.       
+00021630: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+00021640: 6577 6964 7468 3d31 2c0a 2020 2020 2020  ewidth=1,.      
+00021650: 2020 2020 2020 2020 2020 2020 2020 616c                al
+00021660: 7068 613d 302e 342c 0a20 2020 2020 2020  pha=0.4,.       
+00021670: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00021680: 6f72 3d22 6461 726b 6772 6565 6e22 2c0a  or="darkgreen",.
+00021690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000216a0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+000216b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+000216c0: 2020 2020 4465 6c74 6120 3d20 7365 6c66      Delta = self
+000216d0: 2e67 6574 4675 6e63 7469 6f6e 4572 726f  .getFunctionErro
+000216e0: 7228 7876 616c 732c 2063 662e 6d6f 6465  r(xvals, cf.mode
+000216f0: 6c2c 2070 7661 6c73 2c20 7063 6f76 2c20  l, pvals, pcov, 
+00021700: 6669 7865 6450 6172 7329 0a20 2020 2020  fixedPars).     
+00021710: 2020 2020 2020 2020 2020 2070 6c74 2e65             plt.e
+00021720: 7272 6f72 6261 7228 0a20 2020 2020 2020  rrorbar(.       
+00021730: 2020 2020 2020 2020 2020 2020 2078 706c               xpl
+00021740: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00021750: 2020 2020 2020 2079 706c 7420 2b20 4465         yplt + De
+00021760: 6c74 612c 0a20 2020 2020 2020 2020 2020  lta,.           
+00021770: 2020 2020 2020 2020 2066 6d74 3d22 2022           fmt=" "
+00021780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021790: 2020 2020 2020 7865 7272 3d30 2e34 2c0a        xerr=0.4,.
+000217a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000217b0: 2020 2020 616c 7068 613d 302e 372c 0a20      alpha=0.7,. 
+000217c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000217d0: 2020 2065 6c69 6e65 7769 6474 683d 312e     elinewidth=1.
+000217e0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+000217f0: 2020 2020 2020 2063 6f6c 6f72 3d22 6461         color="da
+00021800: 726b 6772 6565 6e22 2c0a 2020 2020 2020  rkgreen",.      
+00021810: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00021820: 2020 2020 2020 2020 2020 2020 706c 742e              plt.
+00021830: 6572 726f 7262 6172 280a 2020 2020 2020  errorbar(.      
+00021840: 2020 2020 2020 2020 2020 2020 2020 7870                xp
+00021850: 6c74 2c0a 2020 2020 2020 2020 2020 2020  lt,.            
+00021860: 2020 2020 2020 2020 7970 6c74 202d 2044          yplt - D
+00021870: 656c 7461 2c0a 2020 2020 2020 2020 2020  elta,.          
+00021880: 2020 2020 2020 2020 2020 666d 743d 2220            fmt=" 
+00021890: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000218a0: 2020 2020 2020 2078 6572 723d 302e 342c         xerr=0.4,
+000218b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000218c0: 2020 2020 2061 6c70 6861 3d30 2e37 2c0a       alpha=0.7,.
+000218d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000218e0: 2020 2020 656c 696e 6577 6964 7468 3d31      elinewidth=1
+000218f0: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
+00021900: 2020 2020 2020 2020 636f 6c6f 723d 2264          color="d
+00021910: 6172 6b67 7265 656e 222c 0a20 2020 2020  arkgreen",.     
+00021920: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00021930: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00021940: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+00021950: 7870 6c74 2929 3a0a 2020 2020 2020 2020  xplt)):.        
+00021960: 2020 2020 2020 2020 2020 2020 6c62 6c20              lbl 
+00021970: 3d20 2224 5c70 6d20 3120 5c73 6967 6d61  = "$\pm 1 \sigma
+00021980: 2422 2069 6620 6920 3d3d 2030 2065 6c73  $" if i == 0 els
+00021990: 6520 2222 0a20 2020 2020 2020 2020 2020  e "".           
+000219a0: 2020 2020 2020 2020 2070 6c74 2e61 7868           plt.axh
+000219b0: 7370 616e 280a 2020 2020 2020 2020 2020  span(.          
+000219c0: 2020 2020 2020 2020 2020 2020 2020 7970                yp
+000219d0: 6c74 5b69 5d20 2d20 4465 6c74 615b 695d  lt[i] - Delta[i]
+000219e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000219f0: 2020 2020 2020 2020 2020 7970 6c74 5b69            yplt[i
+00021a00: 5d20 2b20 4465 6c74 615b 695d 2c0a 2020  ] + Delta[i],.  
+00021a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021a20: 2020 2020 2020 786d 696e 3d28 7870 6c74        xmin=(xplt
+00021a30: 5b69 5d20 2d20 302e 3429 202f 206c 656e  [i] - 0.4) / len
+00021a40: 2878 706c 7429 2c0a 2020 2020 2020 2020  (xplt),.        
+00021a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021a60: 786d 6178 3d28 7870 6c74 5b69 5d20 2b20  xmax=(xplt[i] + 
+00021a70: 302e 3429 202f 206c 656e 2878 706c 7429  0.4) / len(xplt)
+00021a80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00021a90: 2020 2020 2020 2020 2020 616c 7068 613d            alpha=
+00021aa0: 302e 332c 0a20 2020 2020 2020 2020 2020  0.3,.           
+00021ab0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+00021ac0: 6f72 3d22 6461 726b 6b68 616b 6922 2c0a  or="darkkhaki",.
 00021ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021ae0: 206c 6162 656c 3d6c 626c 2c0a 2020 2020   label=lbl,.    
-00021af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b00: 290a 0a20 2020 2020 2020 2023 2064 6973  )..        # dis
-00021b10: 706c 6179 206c 6567 656e 6420 7769 7468  play legend with
-00021b20: 2066 6974 2069 6e66 6f0a 2020 2020 2020   fit info.      
-00021b30: 2020 676c 6f62 616c 2066 6974 5f69 6e66    global fit_inf
-00021b40: 6f0a 2020 2020 2020 2020 6966 2073 616d  o.        if sam
-00021b50: 655f 706c 6f74 3a0a 2020 2020 2020 2020  e_plot:.        
-00021b60: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00021b70: 2020 2020 2020 2020 2066 6974 5f69 6e66           fit_inf
-00021b80: 6f0a 2020 2020 2020 2020 2020 2020 6578  o.            ex
-00021b90: 6365 7074 204e 616d 6545 7272 6f72 3a0a  cept NameError:.
-00021ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021bb0: 6669 745f 696e 666f 203d 205b 5d0a 2020  fit_info = [].  
-00021bc0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00021bd0: 2020 2020 2020 2020 6669 745f 696e 666f          fit_info
-00021be0: 203d 205b 5d0a 0a20 2020 2020 2020 2023   = []..        #
-00021bf0: 2020 312e 2070 6172 616d 6574 6572 2076    1. parameter v
-00021c00: 616c 7565 7320 616e 6420 756e 6365 7274  alues and uncert
-00021c10: 6169 6e74 6965 730a 2020 2020 2020 2020  ainties.        
-00021c20: 7065 203d 2032 2020 2320 6e75 6d62 6572  pe = 2  # number
-00021c30: 206f 6620 7369 676e 6966 6963 616e 7420   of significant 
-00021c40: 6469 6769 7473 206f 6620 756e 6365 7274  digits of uncert
-00021c50: 6169 6e74 790a 2020 2020 2020 2020 6966  ainty.        if
-00021c60: 2073 656c 662e 6d69 6e6f 7352 6573 756c   self.minosResul
-00021c70: 7420 6973 206e 6f74 204e 6f6e 6520 616e  t is not None an
-00021c80: 6420 7365 6c66 2e6d 696e 6f73 5f6f 6b3a  d self.minos_ok:
-00021c90: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00021ca0: 2070 6e2c 2076 2c20 6520 696e 207a 6970   pn, v, e in zip
-00021cb0: 2866 7265 655f 706e 616d 732c 2066 7265  (free_pnams, fre
-00021cc0: 655f 7076 616c 732c 2070 6d65 7272 7329  e_pvals, pmerrs)
-00021cd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00021ce0: 2020 6e64 2c20 5f76 2c20 5f65 203d 2072    nd, _v, _e = r
-00021cf0: 6f75 6e64 5f74 6f5f 6572 726f 7228 762c  ound_to_error(v,
-00021d00: 206d 696e 2861 6273 2865 5b30 5d29 2c20   min(abs(e[0]), 
-00021d10: 6162 7328 655b 315d 2929 2c20 6e73 645f  abs(e[1])), nsd_
-00021d20: 653d 7065 290a 2020 2020 2020 2020 2020  e=pe).          
-00021d30: 2020 2020 2020 7478 7420 3d20 227b 7d20        txt = "{} 
-00021d40: 3d20 247b 3a23 2e7b 7076 7d67 7d5e 7b7b  = ${:#.{pv}g}^{{
-00021d50: 2b7b 3a23 2e7b 7065 7d67 7d7d 7d5f 7b7b  +{:#.{pe}g}}}_{{
-00021d60: 7b3a 232e 7b70 657d 677d 7d7d 2422 0a20  {:#.{pe}g}}}$". 
-00021d70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00021d80: 6974 5f69 6e66 6f2e 6170 7065 6e64 2874  it_info.append(t
-00021d90: 7874 2e66 6f72 6d61 7428 706e 2c20 5f76  xt.format(pn, _v
-00021da0: 2c20 655b 315d 2c20 655b 305d 2c20 7076  , e[1], e[0], pv
-00021db0: 3d6e 642c 2070 653d 7065 2929 0a20 2020  =nd, pe=pe)).   
-00021dc0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00021dd0: 2020 2020 2020 2066 6f72 2070 6e2c 2076         for pn, v
-00021de0: 2c20 6520 696e 207a 6970 2866 7265 655f  , e in zip(free_
-00021df0: 706e 616d 732c 2066 7265 655f 7076 616c  pnams, free_pval
-00021e00: 732c 2070 6d65 7272 7329 3a0a 2020 2020  s, pmerrs):.    
-00021e10: 2020 2020 2020 2020 2020 2020 6e64 2c20              nd, 
-00021e20: 5f76 2c20 5f65 203d 2072 6f75 6e64 5f74  _v, _e = round_t
-00021e30: 6f5f 6572 726f 7228 762c 2065 5b31 5d2c  o_error(v, e[1],
-00021e40: 206e 7364 5f65 3d70 6529 0a20 2020 2020   nsd_e=pe).     
-00021e50: 2020 2020 2020 2020 2020 2074 7874 203d             txt =
-00021e60: 2022 7b7d 203d 2024 7b3a 232e 7b70 767d   "{} = ${:#.{pv}
-00021e70: 677d 5c70 6d7b 3a23 2e7b 7065 7d67 7d24  g}\pm{:#.{pe}g}$
-00021e80: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00021e90: 2020 6669 745f 696e 666f 2e61 7070 656e    fit_info.appen
-00021ea0: 6428 7478 742e 666f 726d 6174 2870 6e2c  d(txt.format(pn,
-00021eb0: 205f 762c 205f 652c 2070 763d 6e64 2c20   _v, _e, pv=nd, 
-00021ec0: 7065 3d70 6529 290a 2020 2020 2020 2020  pe=pe)).        
-00021ed0: 6966 206e 6669 7865 643a 0a20 2020 2020  if nfixed:.     
-00021ee0: 2020 2020 2020 2066 6f72 2070 6e2c 2076         for pn, v
-00021ef0: 2069 6e20 7a69 7028 6669 7865 645f 706e   in zip(fixed_pn
-00021f00: 616d 732c 2066 6978 6564 5f70 7661 6c73  ams, fixed_pvals
-00021f10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00021f20: 2020 2074 7874 203d 2022 7b7d 203d 207b     txt = "{} = {
-00021f30: 3a67 7d20 2028 6669 7865 6429 220a 2020  :g}  (fixed)".  
-00021f40: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00021f50: 745f 696e 666f 2e61 7070 656e 6428 7478  t_info.append(tx
-00021f60: 742e 666f 726d 6174 2870 6e2c 2076 2929  t.format(pn, v))
-00021f70: 0a0a 2020 2020 2020 2020 2320 2032 2e20  ..        #  2. 
-00021f80: 676f 6f64 6e65 7373 2d6f 662d 6669 740a  goodness-of-fit.
-00021f90: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00021fa0: 6669 745f 7479 7065 2069 6e20 5b22 7879  fit_type in ["xy
-00021fb0: 222c 2022 696e 6465 7865 6422 5d3a 0a20  ", "indexed"]:. 
-00021fc0: 2020 2020 2020 2020 2020 2066 6974 5f69             fit_i
-00021fd0: 6e66 6f2e 6170 7065 6e64 280a 2020 2020  nfo.append(.    
-00021fe0: 2020 2020 2020 2020 2020 2020 2224 5c5c              "$\\
-00021ff0: 6368 695e 3224 2f24 6e5f 5c5c 6d61 7468  chi^2$/$n_\\math
-00022000: 726d 7b7b 646f 667d 7d24 3d7b 3a2e 3166  rm{{dof}}$={:.1f
-00022010: 7d2f 7b7d 222e 666f 726d 6174 2867 6f66  }/{}".format(gof
-00022020: 2c20 6e64 6f66 290a 2020 2020 2020 2020  , ndof).        
-00022030: 2020 2020 2020 2020 2b20 222c 2070 3d7b          + ", p={
-00022040: 3a2e 3166 7d25 222e 666f 726d 6174 2831  :.1f}%".format(1
-00022050: 3030 202a 2063 6869 3270 7262 290a 2020  00 * chi2prb).  
-00022060: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00022070: 2020 2020 656c 6966 2073 656c 662e 6669      elif self.fi
-00022080: 745f 7479 7065 203d 3d20 2268 6973 7422  t_type == "hist"
-00022090: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
-000220a0: 745f 696e 666f 2e61 7070 656e 6428 2267  t_info.append("g
-000220b0: 2e6f 2e66 2e2f 246e 5f5c 5c6d 6174 6872  .o.f./$n_\\mathr
-000220c0: 6d7b 7b64 6f66 7d7d 2420 3d20 7b3a 2e31  m{{dof}}$ = {:.1
-000220d0: 667d 2f7b 7d22 2e66 6f72 6d61 7428 676f  f}/{}".format(go
-000220e0: 662c 206e 646f 6629 290a 2020 2020 2020  f, ndof)).      
-000220f0: 2020 2320 2061 6464 206c 6567 656e 6420    #  add legend 
-00022100: 746f 2070 6c6f 740a 2020 2020 2020 2020  to plot.        
-00022110: 706c 742e 6c65 6765 6e64 286c 6f63 3d22  plt.legend(loc="
-00022120: 6265 7374 222c 2074 6974 6c65 3d22 5c6e  best", title="\n
-00022130: 222e 6a6f 696e 2866 6974 5f69 6e66 6f29  ".join(fit_info)
-00022140: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00022150: 6e20 6669 675f 6d6f 6465 6c0a 0a20 2020  n fig_model..   
-00022160: 2023 2070 6c6f 7420 6172 7261 7920 6f66   # plot array of
-00022170: 2070 726f 6669 6c65 7320 616e 6420 636f   profiles and co
-00022180: 6e74 6f75 7273 0a20 2020 2064 6566 2070  ntours.    def p
-00022190: 6c6f 7443 6f6e 746f 7572 7328 7365 6c66  lotContours(self
-000221a0: 2c20 6669 676e 616d 653d 2250 726f 6669  , figname="Profi
-000221b0: 6c65 7320 616e 6420 436f 6e74 6f75 7273  les and Contours
-000221c0: 2229 3a0a 2020 2020 2020 2020 2222 220a  "):.        """.
-000221d0: 2020 2020 2020 2020 506c 6f74 2067 7269          Plot gri
-000221e0: 6420 6f66 2070 726f 6669 6c65 2063 7572  d of profile cur
-000221f0: 7665 7320 616e 6420 6f6e 652d 2061 6e64  ves and one- and
-00022200: 2074 776f 2d73 6967 6d61 0a20 2020 2020   two-sigma.     
-00022210: 2020 2063 6f6e 746f 7572 206c 696e 6573     contour lines
-00022220: 2066 726f 6d20 696d 696e 7569 7420 6f62   from iminuit ob
-00022230: 6a65 6374 0a0a 2020 2020 2020 2020 4172  ject..        Ar
-00022240: 673a 0a20 2020 2020 2020 2020 202a 2069  g:.          * i
-00022250: 6d69 6e75 6974 4f62 6a65 6374 0a0a 2020  minuitObject..  
-00022260: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00022270: 2020 2020 2020 2020 202a 206d 6174 706c           * matpl
-00022280: 6f74 6c69 6220 6669 6775 7265 0a20 2020  otlib figure.   
-00022290: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-000222a0: 2020 6966 206e 6f74 2073 656c 662e 7175    if not self.qu
-000222b0: 6965 743a 0a20 2020 2020 2020 2020 2020  iet:.           
-000222c0: 2070 7269 6e74 2822 2a3d 3d2a 206d 6e46   print("*==* mnF
-000222d0: 6974 3a20 7363 616e 6e69 6e67 2063 6f6e  it: scanning con
-000222e0: 746f 7572 7322 290a 0a20 2020 2020 2020  tours")..       
-000222f0: 2023 2073 6176 6520 636f 6c6f 7220 6d61   # save color ma
-00022300: 7020 616e 6420 7365 7420 6e65 7720 6f6e  p and set new on
-00022310: 6520 2d20 6166 6665 6374 7320 696d 696e  e - affects imin
-00022320: 7569 742e 6472 6177 5f6d 6e63 6f6e 746f  uit.draw_mnconto
-00022330: 7572 2829 0a20 2020 2020 2020 206f 7269  ur().        ori
-00022340: 675f 636d 203d 2070 6c74 2e67 6574 5f63  g_cm = plt.get_c
-00022350: 6d61 7028 290a 2020 2020 2020 2020 706c  map().        pl
-00022360: 742e 7365 745f 636d 6170 2822 7461 6232  t.set_cmap("tab2
-00022370: 3062 2229 0a0a 2020 2020 2020 2020 6d20  0b")..        m 
-00022380: 3d20 7365 6c66 2e6d 696e 7569 740a 2020  = self.minuit.  
-00022390: 2020 2020 2020 6670 6e61 6d73 203d 2073        fpnams = s
-000223a0: 656c 662e 6672 6565 5061 724e 616d 730a  elf.freeParNams.
-000223b0: 2020 2020 2020 2020 6670 7661 6c73 203d          fpvals =
-000223c0: 2073 656c 662e 6672 6565 5061 7256 616c   self.freeParVal
-000223d0: 730a 2020 2020 2020 2020 6670 6572 7273  s.        fperrs
-000223e0: 203d 2073 656c 662e 6672 6565 5061 7245   = self.freeParE
-000223f0: 7272 730a 2020 2020 2020 2020 6e70 6172  rrs.        npar
-00022400: 203d 206c 656e 2866 706e 616d 7329 0a0a   = len(fpnams)..
-00022410: 2020 2020 2020 2020 6673 697a 6520 3d20          fsize = 
-00022420: 332e 3520 6966 206e 7061 7220 3c3d 2033  3.5 if npar <= 3
-00022430: 2065 6c73 6520 322e 350a 2020 2020 2020   else 2.5.      
-00022440: 2020 636f 725f 6669 672c 2061 7861 7272    cor_fig, axarr
-00022450: 203d 2070 6c74 2e73 7562 706c 6f74 7328   = plt.subplots(
-00022460: 0a20 2020 2020 2020 2020 2020 206e 7061  .            npa
-00022470: 722c 0a20 2020 2020 2020 2020 2020 206e  r,.            n
-00022480: 7061 722c 0a20 2020 2020 2020 2020 2020  par,.           
-00022490: 206e 756d 3d66 6967 6e61 6d65 2c0a 2020   num=figname,.  
-000224a0: 2020 2020 2020 2020 2020 6669 6773 697a            figsiz
-000224b0: 653d 2866 7369 7a65 202a 206e 7061 722c  e=(fsize * npar,
-000224c0: 2066 7369 7a65 202a 206e 7061 7229 2c0a   fsize * npar),.
-000224d0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-000224e0: 7472 6169 6e65 645f 6c61 796f 7574 3d54  trained_layout=T
-000224f0: 7275 652c 0a20 2020 2020 2020 2029 0a0a  rue,.        )..
-00022500: 2020 2020 2020 2020 2320 7072 6f74 6563          # protec
-00022510: 7420 7468 6520 666f 6c6c 6f77 696e 672c  t the following,
-00022520: 206d 6179 2066 6169 6c0a 2020 2020 2020   may fail.      
-00022530: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-00022540: 2020 2069 7020 3d20 2d31 0a20 2020 2020     ip = -1.     
-00022550: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00022560: 7261 6e67 6528 302c 206e 7061 7229 3a0a  range(0, npar):.
-00022570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022580: 6970 202b 3d20 310a 2020 2020 2020 2020  ip += 1.        
-00022590: 2020 2020 2020 2020 6a70 203d 202d 310a          jp = -1.
-000225a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000225b0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
-000225c0: 2c20 6e70 6172 293a 0a20 2020 2020 2020  , npar):.       
-000225d0: 2020 2020 2020 2020 2020 2020 206a 7020               jp 
-000225e0: 2b3d 2031 0a20 2020 2020 2020 2020 2020  += 1.           
-000225f0: 2020 2020 2020 2020 2069 6620 6970 203e           if ip >
-00022600: 206a 703a 0a20 2020 2020 2020 2020 2020   jp:.           
-00022610: 2020 2020 2020 2020 2020 2020 2023 2065               # e
-00022620: 6d70 7479 2073 7061 6365 0a20 2020 2020  mpty space.     
-00022630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022640: 2020 2061 7861 7272 5b6a 702c 2069 705d     axarr[jp, ip]
-00022650: 2e61 7869 7328 226f 6666 2229 0a20 2020  .axis("off").   
-00022660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022670: 2065 6c69 6620 6970 203d 3d20 6a70 3a0a   elif ip == jp:.
-00022680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022690: 2020 2020 2020 2020 2320 706c 6f74 2070          # plot p
-000226a0: 726f 6669 6c65 0a20 2020 2020 2020 2020  rofile.         
-000226b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000226c0: 6c74 2e73 6361 2861 7861 7272 5b69 702c  lt.sca(axarr[ip,
-000226d0: 2069 705d 2920 6966 206e 7061 7220 213d   ip]) if npar !=
-000226e0: 2031 2065 6c73 6520 706c 742e 7363 6128   1 else plt.sca(
-000226f0: 6178 6172 7229 0a20 2020 2020 2020 2020  axarr).         
-00022700: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00022710: 2e64 7261 775f 6d6e 7072 6f66 696c 6528  .draw_mnprofile(
-00022720: 6670 6e61 6d73 5b69 5d2c 2073 7562 7472  fpnams[i], subtr
-00022730: 6163 745f 6d69 6e3d 5472 7565 290a 2020  act_min=True).  
-00022740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022750: 2020 2020 2020 6966 2073 656c 662e 4572        if self.Er
-00022760: 7244 6566 203d 3d20 313a 0a20 2020 2020  rDef == 1:.     
-00022770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022780: 2020 2020 2020 2079 6c61 6265 6c20 3d20         ylabel = 
-00022790: 2224 5c44 656c 7461 2028 2d32 5c6c 6e5c  "$\Delta (-2\ln\
-000227a0: 6361 6c7b 4c7d 2924 220a 2020 2020 2020  cal{L})$".      
-000227b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000227c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00021ae0: 2020 2020 2020 2020 6c61 6265 6c3d 6c62          label=lb
+00021af0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+00021b00: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00021b10: 2020 2320 6469 7370 6c61 7920 6c65 6765    # display lege
+00021b20: 6e64 2077 6974 6820 6669 7420 696e 666f  nd with fit info
+00021b30: 0a20 2020 2020 2020 2067 6c6f 6261 6c20  .        global 
+00021b40: 6669 745f 696e 666f 0a20 2020 2020 2020  fit_info.       
+00021b50: 2069 6620 7361 6d65 5f70 6c6f 743a 0a20   if same_plot:. 
+00021b60: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00021b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021b80: 6669 745f 696e 666f 0a20 2020 2020 2020  fit_info.       
+00021b90: 2020 2020 2065 7863 6570 7420 4e61 6d65       except Name
+00021ba0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+00021bb0: 2020 2020 2020 2066 6974 5f69 6e66 6f20         fit_info 
+00021bc0: 3d20 5b5d 0a20 2020 2020 2020 2065 6c73  = [].        els
+00021bd0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+00021be0: 6974 5f69 6e66 6f20 3d20 5b5d 0a0a 2020  it_info = []..  
+00021bf0: 2020 2020 2020 2320 2031 2e20 7061 7261        #  1. para
+00021c00: 6d65 7465 7220 7661 6c75 6573 2061 6e64  meter values and
+00021c10: 2075 6e63 6572 7461 696e 7469 6573 0a20   uncertainties. 
+00021c20: 2020 2020 2020 2070 6520 3d20 3220 2023         pe = 2  #
+00021c30: 206e 756d 6265 7220 6f66 2073 6967 6e69   number of signi
+00021c40: 6669 6361 6e74 2064 6967 6974 7320 6f66  ficant digits of
+00021c50: 2075 6e63 6572 7461 696e 7479 0a20 2020   uncertainty.   
+00021c60: 2020 2020 2069 6620 7365 6c66 2e6d 696e       if self.min
+00021c70: 6f73 5265 7375 6c74 2069 7320 6e6f 7420  osResult is not 
+00021c80: 4e6f 6e65 2061 6e64 2073 656c 662e 6d69  None and self.mi
+00021c90: 6e6f 735f 6f6b 3a0a 2020 2020 2020 2020  nos_ok:.        
+00021ca0: 2020 2020 666f 7220 706e 2c20 762c 2065      for pn, v, e
+00021cb0: 2069 6e20 7a69 7028 6672 6565 5f70 6e61   in zip(free_pna
+00021cc0: 6d73 2c20 6672 6565 5f70 7661 6c73 2c20  ms, free_pvals, 
+00021cd0: 706d 6572 7273 293a 0a20 2020 2020 2020  pmerrs):.       
+00021ce0: 2020 2020 2020 2020 206e 642c 205f 762c           nd, _v,
+00021cf0: 205f 6520 3d20 726f 756e 645f 746f 5f65   _e = round_to_e
+00021d00: 7272 6f72 2876 2c20 6d69 6e28 6162 7328  rror(v, min(abs(
+00021d10: 655b 305d 292c 2061 6273 2865 5b31 5d29  e[0]), abs(e[1])
+00021d20: 292c 206e 7364 5f65 3d70 6529 0a20 2020  ), nsd_e=pe).   
+00021d30: 2020 2020 2020 2020 2020 2020 2074 7874               txt
+00021d40: 203d 2022 7b7d 203d 2024 7b3a 232e 7b70   = "{} = ${:#.{p
+00021d50: 767d 677d 5e7b 7b2b 7b3a 232e 7b70 657d  v}g}^{{+{:#.{pe}
+00021d60: 677d 7d7d 5f7b 7b7b 3a23 2e7b 7065 7d67  g}}}_{{{:#.{pe}g
+00021d70: 7d7d 7d24 220a 2020 2020 2020 2020 2020  }}}$".          
+00021d80: 2020 2020 2020 6669 745f 696e 666f 2e61        fit_info.a
+00021d90: 7070 656e 6428 7478 742e 666f 726d 6174  ppend(txt.format
+00021da0: 2870 6e2c 205f 762c 2065 5b31 5d2c 2065  (pn, _v, e[1], e
+00021db0: 5b30 5d2c 2070 763d 6e64 2c20 7065 3d70  [0], pv=nd, pe=p
+00021dc0: 6529 290a 2020 2020 2020 2020 656c 7365  e)).        else
+00021dd0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00021de0: 7220 706e 2c20 762c 2065 2069 6e20 7a69  r pn, v, e in zi
+00021df0: 7028 6672 6565 5f70 6e61 6d73 2c20 6672  p(free_pnams, fr
+00021e00: 6565 5f70 7661 6c73 2c20 706d 6572 7273  ee_pvals, pmerrs
+00021e10: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00021e20: 2020 206e 642c 205f 762c 205f 6520 3d20     nd, _v, _e = 
+00021e30: 726f 756e 645f 746f 5f65 7272 6f72 2876  round_to_error(v
+00021e40: 2c20 655b 315d 2c20 6e73 645f 653d 7065  , e[1], nsd_e=pe
+00021e50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00021e60: 2020 7478 7420 3d20 227b 7d20 3d20 247b    txt = "{} = ${
+00021e70: 3a23 2e7b 7076 7d67 7d5c 706d 7b3a 232e  :#.{pv}g}\pm{:#.
+00021e80: 7b70 657d 677d 2422 0a20 2020 2020 2020  {pe}g}$".       
+00021e90: 2020 2020 2020 2020 2066 6974 5f69 6e66           fit_inf
+00021ea0: 6f2e 6170 7065 6e64 2874 7874 2e66 6f72  o.append(txt.for
+00021eb0: 6d61 7428 706e 2c20 5f76 2c20 5f65 2c20  mat(pn, _v, _e, 
+00021ec0: 7076 3d6e 642c 2070 653d 7065 2929 0a20  pv=nd, pe=pe)). 
+00021ed0: 2020 2020 2020 2069 6620 6e66 6978 6564         if nfixed
+00021ee0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00021ef0: 7220 706e 2c20 7620 696e 207a 6970 2866  r pn, v in zip(f
+00021f00: 6978 6564 5f70 6e61 6d73 2c20 6669 7865  ixed_pnams, fixe
+00021f10: 645f 7076 616c 7329 3a0a 2020 2020 2020  d_pvals):.      
+00021f20: 2020 2020 2020 2020 2020 7478 7420 3d20            txt = 
+00021f30: 227b 7d20 3d20 7b3a 677d 2020 2866 6978  "{} = {:g}  (fix
+00021f40: 6564 2922 0a20 2020 2020 2020 2020 2020  ed)".           
+00021f50: 2020 2020 2066 6974 5f69 6e66 6f2e 6170       fit_info.ap
+00021f60: 7065 6e64 2874 7874 2e66 6f72 6d61 7428  pend(txt.format(
+00021f70: 706e 2c20 7629 290a 0a20 2020 2020 2020  pn, v))..       
+00021f80: 2023 2020 322e 2067 6f6f 646e 6573 732d   #  2. goodness-
+00021f90: 6f66 2d66 6974 0a20 2020 2020 2020 2069  of-fit.        i
+00021fa0: 6620 7365 6c66 2e66 6974 5f74 7970 6520  f self.fit_type 
+00021fb0: 696e 205b 2278 7922 2c20 2269 6e64 6578  in ["xy", "index
+00021fc0: 6564 225d 3a0a 2020 2020 2020 2020 2020  ed"]:.          
+00021fd0: 2020 6669 745f 696e 666f 2e61 7070 656e    fit_info.appen
+00021fe0: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00021ff0: 2020 2022 245c 5c63 6869 5e32 242f 246e     "$\\chi^2$/$n
+00022000: 5f5c 5c6d 6174 6872 6d7b 7b64 6f66 7d7d  _\\mathrm{{dof}}
+00022010: 243d 7b3a 2e31 667d 2f7b 7d22 2e66 6f72  $={:.1f}/{}".for
+00022020: 6d61 7428 676f 662c 206e 646f 6629 0a20  mat(gof, ndof). 
+00022030: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+00022040: 2022 2c20 703d 7b3a 2e31 667d 2522 2e66   ", p={:.1f}%".f
+00022050: 6f72 6d61 7428 3130 3020 2a20 6368 6932  ormat(100 * chi2
+00022060: 7072 6229 0a20 2020 2020 2020 2020 2020  prb).           
+00022070: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
+00022080: 7365 6c66 2e66 6974 5f74 7970 6520 3d3d  self.fit_type ==
+00022090: 2022 6869 7374 223a 0a20 2020 2020 2020   "hist":.       
+000220a0: 2020 2020 2066 6974 5f69 6e66 6f2e 6170       fit_info.ap
+000220b0: 7065 6e64 2822 672e 6f2e 662e 2f24 6e5f  pend("g.o.f./$n_
+000220c0: 5c5c 6d61 7468 726d 7b7b 646f 667d 7d24  \\mathrm{{dof}}$
+000220d0: 203d 207b 3a2e 3166 7d2f 7b7d 222e 666f   = {:.1f}/{}".fo
+000220e0: 726d 6174 2867 6f66 2c20 6e64 6f66 2929  rmat(gof, ndof))
+000220f0: 0a20 2020 2020 2020 2023 2020 6164 6420  .        #  add 
+00022100: 6c65 6765 6e64 2074 6f20 706c 6f74 0a20  legend to plot. 
+00022110: 2020 2020 2020 2070 6c74 2e6c 6567 656e         plt.legen
+00022120: 6428 6c6f 633d 2262 6573 7422 2c20 7469  d(loc="best", ti
+00022130: 746c 653d 225c 6e22 2e6a 6f69 6e28 6669  tle="\n".join(fi
+00022140: 745f 696e 666f 2929 0a0a 2020 2020 2020  t_info))..      
+00022150: 2020 7265 7475 726e 2066 6967 5f6d 6f64    return fig_mod
+00022160: 656c 0a0a 2020 2020 2320 706c 6f74 2061  el..    # plot a
+00022170: 7272 6179 206f 6620 7072 6f66 696c 6573  rray of profiles
+00022180: 2061 6e64 2063 6f6e 746f 7572 730a 2020   and contours.  
+00022190: 2020 6465 6620 706c 6f74 436f 6e74 6f75    def plotContou
+000221a0: 7273 2873 656c 662c 2066 6967 6e61 6d65  rs(self, figname
+000221b0: 3d22 5072 6f66 696c 6573 2061 6e64 2043  ="Profiles and C
+000221c0: 6f6e 746f 7572 7322 293a 0a20 2020 2020  ontours"):.     
+000221d0: 2020 2022 2222 0a20 2020 2020 2020 2050     """.        P
+000221e0: 6c6f 7420 6772 6964 206f 6620 7072 6f66  lot grid of prof
+000221f0: 696c 6520 6375 7276 6573 2061 6e64 206f  ile curves and o
+00022200: 6e65 2d20 616e 6420 7477 6f2d 7369 676d  ne- and two-sigm
+00022210: 610a 2020 2020 2020 2020 636f 6e74 6f75  a.        contou
+00022220: 7220 6c69 6e65 7320 6672 6f6d 2069 6d69  r lines from imi
+00022230: 6e75 6974 206f 626a 6563 740a 0a20 2020  nuit object..   
+00022240: 2020 2020 2041 7267 3a0a 2020 2020 2020       Arg:.      
+00022250: 2020 2020 2a20 696d 696e 7569 744f 626a      * iminuitObj
+00022260: 6563 740a 0a20 2020 2020 2020 2052 6574  ect..        Ret
+00022270: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00022280: 2a20 6d61 7470 6c6f 746c 6962 2066 6967  * matplotlib fig
+00022290: 7572 650a 2020 2020 2020 2020 2222 220a  ure.        """.
+000222a0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000222b0: 7365 6c66 2e71 7569 6574 3a0a 2020 2020  self.quiet:.    
+000222c0: 2020 2020 2020 2020 7072 696e 7428 222a          print("*
+000222d0: 3d3d 2a20 6d6e 4669 743a 2073 6361 6e6e  ==* mnFit: scann
+000222e0: 696e 6720 636f 6e74 6f75 7273 2229 0a0a  ing contours")..
+000222f0: 2020 2020 2020 2020 2320 7361 7665 2063          # save c
+00022300: 6f6c 6f72 206d 6170 2061 6e64 2073 6574  olor map and set
+00022310: 206e 6577 206f 6e65 202d 2061 6666 6563   new one - affec
+00022320: 7473 2069 6d69 6e75 6974 2e64 7261 775f  ts iminuit.draw_
+00022330: 6d6e 636f 6e74 6f75 7228 290a 2020 2020  mncontour().    
+00022340: 2020 2020 6f72 6967 5f63 6d20 3d20 706c      orig_cm = pl
+00022350: 742e 6765 745f 636d 6170 2829 0a20 2020  t.get_cmap().   
+00022360: 2020 2020 2070 6c74 2e73 6574 5f63 6d61       plt.set_cma
+00022370: 7028 2274 6162 3230 6222 290a 0a20 2020  p("tab20b")..   
+00022380: 2020 2020 206d 203d 2073 656c 662e 6d69       m = self.mi
+00022390: 6e75 6974 0a20 2020 2020 2020 2066 706e  nuit.        fpn
+000223a0: 616d 7320 3d20 7365 6c66 2e66 7265 6550  ams = self.freeP
+000223b0: 6172 4e61 6d73 0a20 2020 2020 2020 2066  arNams.        f
+000223c0: 7076 616c 7320 3d20 7365 6c66 2e66 7265  pvals = self.fre
+000223d0: 6550 6172 5661 6c73 0a20 2020 2020 2020  eParVals.       
+000223e0: 2066 7065 7272 7320 3d20 7365 6c66 2e66   fperrs = self.f
+000223f0: 7265 6550 6172 4572 7273 0a20 2020 2020  reeParErrs.     
+00022400: 2020 206e 7061 7220 3d20 6c65 6e28 6670     npar = len(fp
+00022410: 6e61 6d73 290a 0a20 2020 2020 2020 2066  nams)..        f
+00022420: 7369 7a65 203d 2033 2e35 2069 6620 6e70  size = 3.5 if np
+00022430: 6172 203c 3d20 3320 656c 7365 2032 2e35  ar <= 3 else 2.5
+00022440: 0a20 2020 2020 2020 2063 6f72 5f66 6967  .        cor_fig
+00022450: 2c20 6178 6172 7220 3d20 706c 742e 7375  , axarr = plt.su
+00022460: 6270 6c6f 7473 280a 2020 2020 2020 2020  bplots(.        
+00022470: 2020 2020 6e70 6172 2c0a 2020 2020 2020      npar,.      
+00022480: 2020 2020 2020 6e70 6172 2c0a 2020 2020        npar,.    
+00022490: 2020 2020 2020 2020 6e75 6d3d 6669 676e          num=fign
+000224a0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+000224b0: 2066 6967 7369 7a65 3d28 6673 697a 6520   figsize=(fsize 
+000224c0: 2a20 6e70 6172 2c20 6673 697a 6520 2a20  * npar, fsize * 
+000224d0: 6e70 6172 292c 0a20 2020 2020 2020 2020  npar),.         
+000224e0: 2020 2063 6f6e 7374 7261 696e 6564 5f6c     constrained_l
+000224f0: 6179 6f75 743d 5472 7565 2c0a 2020 2020  ayout=True,.    
+00022500: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+00022510: 2070 726f 7465 6374 2074 6865 2066 6f6c   protect the fol
+00022520: 6c6f 7769 6e67 2c20 6d61 7920 6661 696c  lowing, may fail
+00022530: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00022540: 2020 2020 2020 2020 2020 6970 203d 202d            ip = -
+00022550: 310a 2020 2020 2020 2020 2020 2020 666f  1.            fo
+00022560: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
+00022570: 6e70 6172 293a 0a20 2020 2020 2020 2020  npar):.         
+00022580: 2020 2020 2020 2069 7020 2b3d 2031 0a20         ip += 1. 
+00022590: 2020 2020 2020 2020 2020 2020 2020 206a                 j
+000225a0: 7020 3d20 2d31 0a20 2020 2020 2020 2020  p = -1.         
+000225b0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+000225c0: 7261 6e67 6528 302c 206e 7061 7229 3a0a  range(0, npar):.
+000225d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000225e0: 2020 2020 6a70 202b 3d20 310a 2020 2020      jp += 1.    
+000225f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022600: 6966 2069 7020 3e20 6a70 3a0a 2020 2020  if ip > jp:.    
+00022610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022620: 2020 2020 2320 656d 7074 7920 7370 6163      # empty spac
+00022630: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00022640: 2020 2020 2020 2020 2020 6178 6172 725b            axarr[
+00022650: 6a70 2c20 6970 5d2e 6178 6973 2822 6f66  jp, ip].axis("of
+00022660: 6622 290a 2020 2020 2020 2020 2020 2020  f").            
+00022670: 2020 2020 2020 2020 656c 6966 2069 7020          elif ip 
+00022680: 3d3d 206a 703a 0a20 2020 2020 2020 2020  == jp:.         
+00022690: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000226a0: 2070 6c6f 7420 7072 6f66 696c 650a 2020   plot profile.  
+000226b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000226c0: 2020 2020 2020 706c 742e 7363 6128 6178        plt.sca(ax
+000226d0: 6172 725b 6970 2c20 6970 5d29 2069 6620  arr[ip, ip]) if 
+000226e0: 6e70 6172 2021 3d20 3120 656c 7365 2070  npar != 1 else p
+000226f0: 6c74 2e73 6361 2861 7861 7272 290a 2020  lt.sca(axarr).  
+00022700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022710: 2020 2020 2020 6d2e 6472 6177 5f6d 6e70        m.draw_mnp
+00022720: 726f 6669 6c65 2866 706e 616d 735b 695d  rofile(fpnams[i]
+00022730: 2c20 7375 6274 7261 6374 5f6d 696e 3d54  , subtract_min=T
+00022740: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00022750: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00022760: 7365 6c66 2e45 7272 4465 6620 3d3d 2031  self.ErrDef == 1
+00022770: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00022780: 2020 2020 2020 2020 2020 2020 2020 796c                yl
+00022790: 6162 656c 203d 2022 245c 4465 6c74 6120  abel = "$\Delta 
+000227a0: 282d 325c 6c6e 5c63 616c 7b4c 7d29 2422  (-2\ln\cal{L})$"
+000227b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000227c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 000227d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000227e0: 2020 2020 796c 6162 656c 203d 2022 245c      ylabel = "$\
-000227f0: 4465 6c74 6120 282d 5c6c 6e5c 6361 6c7b  Delta (-\ln\cal{
-00022800: 4c7d 2924 220a 2020 2020 2020 2020 2020  L})$".          
-00022810: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00022820: 742e 796c 6162 656c 2879 6c61 6265 6c29  t.ylabel(ylabel)
-00022830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022840: 2020 2020 2020 2020 2078 6d6e 2c20 786d           xmn, xm
-00022850: 7820 3d20 706c 742e 6763 6128 292e 6765  x = plt.gca().ge
-00022860: 745f 786c 696d 2829 0a20 2020 2020 2020  t_xlim().       
+000227e0: 2020 2020 2020 2020 2020 2079 6c61 6265             ylabe
+000227f0: 6c20 3d20 2224 5c44 656c 7461 2028 2d5c  l = "$\Delta (-\
+00022800: 6c6e 5c63 616c 7b4c 7d29 2422 0a20 2020  ln\cal{L})$".   
+00022810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022820: 2020 2020 2070 6c74 2e79 6c61 6265 6c28       plt.ylabel(
+00022830: 796c 6162 656c 290a 2020 2020 2020 2020  ylabel).        
+00022840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022850: 786d 6e2c 2078 6d78 203d 2070 6c74 2e67  xmn, xmx = plt.g
+00022860: 6361 2829 2e67 6574 5f78 6c69 6d28 290a  ca().get_xlim().
 00022870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022880: 2023 2073 686f 7720 686f 7269 7a6f 6e74   # show horizont
-00022890: 616c 206c 696e 6520 6174 2073 656c 662e  al line at self.
-000228a0: 4572 7244 6566 0a20 2020 2020 2020 2020  ErrDef.         
-000228b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000228c0: 6c74 2e68 6c69 6e65 7328 0a20 2020 2020  lt.hlines(.     
-000228d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000228e0: 2020 2020 2020 2073 656c 662e 4572 7244         self.ErrD
-000228f0: 6566 2c20 786d 6e2c 2078 6d78 2c20 636f  ef, xmn, xmx, co
-00022900: 6c6f 723d 226f 7261 6e67 6522 2c20 6c69  lor="orange", li
-00022910: 6e65 7374 796c 653d 222d 2d22 0a20 2020  nestyle="--".   
-00022920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022930: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00022940: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00022950: 6c74 2e65 7272 6f72 6261 7228 0a20 2020  lt.errorbar(.   
-00022960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022970: 2020 2020 2020 2020 2066 7076 616c 735b           fpvals[
-00022980: 695d 2c0a 2020 2020 2020 2020 2020 2020  i],.            
+00022880: 2020 2020 2020 2020 2320 7368 6f77 2068          # show h
+00022890: 6f72 697a 6f6e 7461 6c20 6c69 6e65 2061  orizontal line a
+000228a0: 7420 7365 6c66 2e45 7272 4465 660a 2020  t self.ErrDef.  
+000228b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000228c0: 2020 2020 2020 706c 742e 686c 696e 6573        plt.hlines
+000228d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000228e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000228f0: 6c66 2e45 7272 4465 662c 2078 6d6e 2c20  lf.ErrDef, xmn, 
+00022900: 786d 782c 2063 6f6c 6f72 3d22 6f72 616e  xmx, color="oran
+00022910: 6765 222c 206c 696e 6573 7479 6c65 3d22  ge", linestyle="
+00022920: 2d2d 220a 2020 2020 2020 2020 2020 2020  --".            
+00022930: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00022940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022950: 2020 2020 2020 706c 742e 6572 726f 7262        plt.errorb
+00022960: 6172 280a 2020 2020 2020 2020 2020 2020  ar(.            
+00022970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022980: 6670 7661 6c73 5b69 5d2c 0a20 2020 2020  fpvals[i],.     
 00022990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229a0: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
+000229a0: 2020 2020 2020 2030 2e30 2c0a 2020 2020         0.0,.    
 000229b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229c0: 2078 6572 723d 6670 6572 7273 5b69 5d2c   xerr=fperrs[i],
-000229d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000229e0: 2020 2020 2020 2020 2020 2020 2066 6d74               fmt
-000229f0: 3d22 7822 2c0a 2020 2020 2020 2020 2020  ="x",.          
+000229c0: 2020 2020 2020 2020 7865 7272 3d66 7065          xerr=fpe
+000229d0: 7272 735b 695d 2c0a 2020 2020 2020 2020  rrs[i],.        
+000229e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229f0: 2020 2020 666d 743d 2278 222c 0a20 2020      fmt="x",.   
 00022a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a10: 2020 636f 6c6f 723d 2262 6c75 6522 2c0a    color="blue",.
-00022a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a30: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-00022a40: 7374 796c 653d 222d 222c 0a20 2020 2020  style="-",.     
-00022a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a60: 2020 2020 2020 2063 6170 7369 7a65 3d33         capsize=3
-00022a70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00022a80: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00022a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022aa0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00022ab0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00022ac0: 742e 7363 6128 6178 6172 725b 6a70 2c20  t.sca(axarr[jp, 
-00022ad0: 6970 5d29 0a20 2020 2020 2020 2020 2020  ip]).           
-00022ae0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00022af0: 7365 6c66 2e69 6d69 6e75 6974 5f76 6572  self.iminuit_ver
-00022b00: 7369 6f6e 203c 2022 3222 3a0a 2020 2020  sion < "2":.    
-00022b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b20: 2020 2020 2020 2020 6d2e 6472 6177 5f6d          m.draw_m
-00022b30: 6e63 6f6e 746f 7572 2866 706e 616d 735b  ncontour(fpnams[
-00022b40: 695d 2c20 6670 6e61 6d73 5b6a 5d29 0a20  i], fpnams[j]). 
-00022b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00022b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022b80: 2020 2020 2020 2020 206d 2e64 7261 775f           m.draw_
-00022b90: 6d6e 636f 6e74 6f75 7228 0a20 2020 2020  mncontour(.     
-00022ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022bb0: 2020 2020 2020 2020 2020 2066 706e 616d             fpnam
-00022bc0: 735b 695d 2c0a 2020 2020 2020 2020 2020  s[i],.          
+00022a10: 2020 2020 2020 2020 2063 6f6c 6f72 3d22           color="
+00022a20: 626c 7565 222c 0a20 2020 2020 2020 2020  blue",.         
+00022a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a40: 2020 206c 696e 6573 7479 6c65 3d22 2d22     linestyle="-"
+00022a50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00022a60: 2020 2020 2020 2020 2020 2020 2020 6361                ca
+00022a70: 7073 697a 653d 332c 0a20 2020 2020 2020  psize=3,.       
+00022a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a90: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00022aa0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00022ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022ac0: 2020 2020 2070 6c74 2e73 6361 2861 7861       plt.sca(axa
+00022ad0: 7272 5b6a 702c 2069 705d 290a 2020 2020  rr[jp, ip]).    
+00022ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022af0: 2020 2020 6966 2073 656c 662e 696d 696e      if self.imin
+00022b00: 7569 745f 7665 7273 696f 6e20 3c20 2232  uit_version < "2
+00022b10: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00022b20: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00022b30: 2e64 7261 775f 6d6e 636f 6e74 6f75 7228  .draw_mncontour(
+00022b40: 6670 6e61 6d73 5b69 5d2c 2066 706e 616d  fpnams[i], fpnam
+00022b50: 735b 6a5d 290a 2020 2020 2020 2020 2020  s[j]).          
+00022b60: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00022b70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00022b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b90: 6d2e 6472 6177 5f6d 6e63 6f6e 746f 7572  m.draw_mncontour
+00022ba0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00022bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022bc0: 2020 6670 6e61 6d73 5b69 5d2c 0a20 2020    fpnams[i],.   
 00022bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022be0: 2020 2020 2020 6670 6e61 6d73 5b6a 5d2c        fpnams[j],
-00022bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022be0: 2020 2020 2020 2020 2020 2020 2066 706e               fpn
+00022bf0: 616d 735b 6a5d 2c0a 2020 2020 2020 2020  ams[j],.        
 00022c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c10: 2063 6c3d 2873 656c 662e 4368 6932 3243   cl=(self.Chi22C
-00022c20: 4c28 312e 3029 2c20 7365 6c66 2e43 6869  L(1.0), self.Chi
-00022c30: 3232 434c 2834 2e30 2929 2c0a 2020 2020  22CL(4.0)),.    
-00022c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c50: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00022c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022c70: 2020 2320 706c 6f74 2062 6573 742d 6669    # plot best-fi
-00022c80: 7420 7661 6c75 6573 2061 6e64 206d 6967  t values and mig
-00022c90: 7261 6420 6572 726f 7273 0a20 2020 2020  rad errors.     
-00022ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022cb0: 2020 2070 6c74 2e65 7272 6f72 6261 7228     plt.errorbar(
-00022cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022cd0: 2020 2020 2020 2020 2020 2020 2066 7076               fpv
-00022ce0: 616c 735b 695d 2c0a 2020 2020 2020 2020  als[i],.        
+00022c10: 2020 2020 2020 2020 636c 3d28 7365 6c66          cl=(self
+00022c20: 2e43 6869 3232 434c 2831 2e30 292c 2073  .Chi22CL(1.0), s
+00022c30: 656c 662e 4368 6932 3243 4c28 342e 3029  elf.Chi22CL(4.0)
+00022c40: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00022c50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00022c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022c70: 2020 2020 2020 2020 2023 2070 6c6f 7420           # plot 
+00022c80: 6265 7374 2d66 6974 2076 616c 7565 7320  best-fit values 
+00022c90: 616e 6420 6d69 6772 6164 2065 7272 6f72  and migrad error
+00022ca0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00022cb0: 2020 2020 2020 2020 2020 706c 742e 6572            plt.er
+00022cc0: 726f 7262 6172 280a 2020 2020 2020 2020  rorbar(.        
+00022cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022ce0: 2020 2020 6670 7661 6c73 5b69 5d2c 0a20      fpvals[i],. 
 00022cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d00: 2020 2020 6670 7661 6c73 5b6a 5d2c 0a20      fpvals[j],. 
-00022d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d20: 2020 2020 2020 2020 2020 2078 6572 723d             xerr=
-00022d30: 6670 6572 7273 5b69 5d2c 0a20 2020 2020  fperrs[i],.     
-00022d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d50: 2020 2020 2020 2079 6572 723d 6670 6572         yerr=fper
-00022d60: 7273 5b6a 5d2c 0a20 2020 2020 2020 2020  rs[j],.         
+00022d00: 2020 2020 2020 2020 2020 2066 7076 616c             fpval
+00022d10: 735b 6a5d 2c0a 2020 2020 2020 2020 2020  s[j],.          
+00022d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022d30: 2020 7865 7272 3d66 7065 7272 735b 695d    xerr=fperrs[i]
+00022d40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00022d50: 2020 2020 2020 2020 2020 2020 2020 7965                ye
+00022d60: 7272 3d66 7065 7272 735b 6a5d 2c0a 2020  rr=fperrs[j],.  
 00022d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d80: 2020 2066 6d74 3d22 7822 2c0a 2020 2020     fmt="x",.    
-00022d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022da0: 2020 2020 2020 2020 636f 6c6f 723d 2264          color="d
-00022db0: 6172 6b62 6c75 6522 2c0a 2020 2020 2020  arkblue",.      
-00022dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022dd0: 2020 2020 2020 6563 6f6c 6f72 3d22 626c        ecolor="bl
-00022de0: 7565 222c 0a20 2020 2020 2020 2020 2020  ue",.           
+00022d80: 2020 2020 2020 2020 2020 666d 743d 2278            fmt="x
+00022d90: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00022da0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00022db0: 6f6c 6f72 3d22 6461 726b 626c 7565 222c  olor="darkblue",
+00022dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00022dd0: 2020 2020 2020 2020 2020 2020 2065 636f               eco
+00022de0: 6c6f 723d 2262 6c75 6522 2c0a 2020 2020  lor="blue",.    
 00022df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e00: 2063 6170 7369 7a65 3d33 2c0a 2020 2020   capsize=3,.    
-00022e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e20: 2020 2020 2020 2020 616c 7068 613d 302e          alpha=0.
-00022e30: 3636 2c0a 2020 2020 2020 2020 2020 2020  66,.            
-00022e40: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00022e50: 2020 2020 2020 2020 2020 2320 7265 7374            # rest
-00022e60: 6f72 6520 636f 6c6f 7220 6d61 700a 2020  ore color map.  
-00022e70: 2020 2020 2020 2020 2020 706c 742e 7365            plt.se
-00022e80: 745f 636d 6170 286f 7269 675f 636d 290a  t_cmap(orig_cm).
-00022e90: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00022ea0: 7572 6e20 636f 725f 6669 670a 0a20 2020  urn cor_fig..   
-00022eb0: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
-00022ec0: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
-00022ed0: 2020 2020 2020 2020 7072 696e 7428 222a          print("*
-00022ee0: 3d3d 2a20 2121 2120 7072 6f66 696c 6520  ==* !!! profile 
-00022ef0: 616e 6420 636f 6e74 6f75 7220 7363 616e  and contour scan
-00022f00: 2066 6169 6c65 6422 290a 2020 2020 2020   failed").      
-00022f10: 2020 2020 2020 7072 696e 7428 6529 0a20        print(e). 
-00022f20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00022f30: 6e20 4e6f 6e65 0a0a 2020 2020 6465 6620  n None..    def 
-00022f40: 6765 7450 726f 6669 6c65 2873 656c 662c  getProfile(self,
-00022f50: 2070 6e61 6d2c 2072 616e 6765 3d33 2e30   pnam, range=3.0
-00022f60: 2c20 6e70 6f69 6e74 733d 3330 293a 0a20  , npoints=30):. 
-00022f70: 2020 2020 2020 2022 2222 7265 7475 726e         """return
-00022f80: 2070 726f 6669 6c65 206c 696b 656c 6968   profile likelih
-00022f90: 6f6f 6420 6f66 2070 6172 616d 6574 6572  ood of parameter
-00022fa0: 2070 6e61 6d0a 0a20 2020 2020 2020 2041   pnam..        A
-00022fb0: 7267 733a 0a20 2020 2020 2020 2020 202d  rgs:.          -
-00022fc0: 2070 6172 616d 6574 6572 206e 616d 650a   parameter name.
-00022fd0: 2020 2020 2020 2020 2020 2d20 7363 616e            - scan
-00022fe0: 2072 616e 6765 2069 6e20 7369 676d 612c   range in sigma,
-00022ff0: 2061 7265 2074 7570 6c65 2077 6974 6820   are tuple with 
-00023000: 6c6f 7765 7220 616e 6420 7570 7065 7220  lower and upper 
-00023010: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
-00023020: 2d20 6e75 6d62 6572 206f 6620 706f 696e  - number of poin
-00023030: 7473 0a20 2020 2020 2020 2022 2222 0a20  ts.        """. 
-00023040: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00023050: 6d69 6e75 6974 5f76 6572 7369 6f6e 203c  minuit_version <
-00023060: 2022 3222 3a0a 2020 2020 2020 2020 2020   "2":.          
-00023070: 2020 7072 696e 7428 2221 2121 2067 6574    print("!!! get
-00023080: 5072 6f66 696c 6520 6e6f 7420 696d 706c  Profile not impl
-00023090: 656d 656e 7465 6420 766f 7220 696d 696e  emented vor imin
-000230a0: 7569 7420 7665 7273 2e3c 3222 290a 2020  uit vers.<2").  
-000230b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000230c0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000230d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000230e0: 6e20 7365 6c66 2e6d 696e 7569 742e 6d6e  n self.minuit.mn
-000230f0: 7072 6f66 696c 6528 0a20 2020 2020 2020  profile(.       
-00023100: 2020 2020 2020 2020 2070 6e61 6d2c 2062           pnam, b
-00023110: 6f75 6e64 3d72 616e 6765 2c20 7369 7a65  ound=range, size
-00023120: 3d6e 706f 696e 7473 2c20 7375 6274 7261  =npoints, subtra
-00023130: 6374 5f6d 696e 3d54 7275 650a 2020 2020  ct_min=True.    
-00023140: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00023150: 6566 2067 6574 436f 6e74 6f75 7228 7365  ef getContour(se
-00023160: 6c66 2c20 706e 616d 312c 2070 6e61 6d32  lf, pnam1, pnam2
-00023170: 2c20 636c 3d4e 6f6e 652c 206e 706f 696e  , cl=None, npoin
-00023180: 7473 3d31 3030 293a 0a20 2020 2020 2020  ts=100):.       
-00023190: 2022 2222 7265 7475 726e 2070 726f 6669   """return profi
-000231a0: 6c65 206c 696b 656c 6968 6f6f 6420 636f  le likelihood co
-000231b0: 6e74 6f75 7220 6f66 2070 6172 616d 6574  ntour of paramet
-000231c0: 6572 7320 706e 616d 3120 616e 6420 706e  ers pnam1 and pn
-000231d0: 616d 320a 0a20 2020 2020 2020 2041 7267  am2..        Arg
-000231e0: 733a 0a20 2020 2020 2020 2020 202d 2031  s:.          - 1
-000231f0: 7374 2070 6172 616d 6574 6572 206e 616d  st parameter nam
-00023200: 650a 2020 2020 2020 2020 2020 2d20 326e  e.          - 2n
-00023210: 6420 7061 7261 6d65 7465 7220 6e61 6d65  d parameter name
-00023220: 0a20 2020 2020 2020 2020 202d 2063 6f6e  .          - con
-00023230: 6669 6465 6e63 6520 6c65 7665 6c0a 2020  fidence level.  
-00023240: 2020 2020 2020 2020 2d20 6e75 6d62 6572          - number
-00023250: 206f 6620 706f 696e 7473 0a0a 2020 2020   of points..    
-00023260: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00023270: 2020 2020 2020 202d 2061 7272 6179 206f         - array o
-00023280: 6620 666c 6f61 7420 286e 706f 696e 7473  f float (npoints
-00023290: 202a 2032 2920 636f 6e74 6f75 7220 706f   * 2) contour po
-000232a0: 696e 7473 0a20 2020 2020 2020 2022 2222  ints.        """
-000232b0: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-000232c0: 662e 696d 696e 7569 745f 7665 7273 696f  f.iminuit_versio
-000232d0: 6e20 3c20 2232 223a 0a20 2020 2020 2020  n < "2":.       
-000232e0: 2020 2020 2070 7269 6e74 2822 2121 2120       print("!!! 
-000232f0: 6765 7443 6f6e 746f 7572 206e 6f74 2069  getContour not i
-00023300: 6d70 6c65 6d65 6e74 6564 2076 6f72 2069  mplemented vor i
-00023310: 6d69 6e75 6974 2076 6572 732e 3c32 2229  minuit vers.<2")
-00023320: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00023330: 7572 6e0a 2020 2020 2020 2020 7265 7475  urn.        retu
-00023340: 726e 2073 656c 662e 6d69 6e75 6974 2e6d  rn self.minuit.m
-00023350: 6e63 6f6e 746f 7572 2870 6e61 6d31 2c20  ncontour(pnam1, 
-00023360: 706e 616d 322c 2063 6c3d 636c 2c20 7369  pnam2, cl=cl, si
-00023370: 7a65 3d6e 706f 696e 7473 290a 0a20 2020  ze=npoints)..   
-00023380: 2064 6566 2070 6c6f 745f 5072 6f66 696c   def plot_Profil
-00023390: 6528 7365 6c66 2c20 706e 616d 2c20 7261  e(self, pnam, ra
-000233a0: 6e67 653d 322e 302c 206e 706f 696e 7473  nge=2.0, npoints
-000233b0: 3d33 3029 3a0a 2020 2020 2020 2020 2222  =30):.        ""
-000233c0: 2270 6c6f 7420 7072 6f66 696c 6520 6c69  "plot profile li
-000233d0: 6b65 6c69 686f 6f64 206f 6620 7061 7261  kelihood of para
-000233e0: 6d65 7465 7220 706e 616d 0a0a 2020 2020  meter pnam..    
-000233f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00023400: 2020 2020 2d20 7061 7261 6d65 7465 7220      - parameter 
-00023410: 6e61 6d65 0a20 2020 2020 2020 2020 202d  name.          -
-00023420: 2073 6361 6e20 7261 6e67 6520 696e 2073   scan range in s
-00023430: 6967 6d61 2c20 6172 6520 7475 706c 6520  igma, are tuple 
-00023440: 7769 7468 206c 6f77 6572 2061 6e64 2075  with lower and u
-00023450: 7070 6572 2076 616c 7565 0a20 2020 2020  pper value.     
-00023460: 2020 2020 202d 206e 756d 6265 7220 6f66       - number of
-00023470: 2070 6f69 6e74 730a 0a20 2020 2020 2020   points..       
-00023480: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00023490: 2020 2020 2d20 6d61 7470 6c6f 746c 6962      - matplotlib
-000234a0: 2066 6967 7572 650a 2020 2020 2020 2020   figure.        
-000234b0: 2222 220a 0a20 2020 2020 2020 2066 6967  """..        fig
-000234c0: 203d 2070 6c74 2e66 6967 7572 6528 6e75   = plt.figure(nu
-000234d0: 6d3d 224c 696b 656c 6968 6f6f 6420 7072  m="Likelihood pr
-000234e0: 6f66 696c 6520 2220 2b20 706e 616d 2c20  ofile " + pnam, 
-000234f0: 6669 6773 697a 653d 2835 2e30 2c20 352e  figsize=(5.0, 5.
-00023500: 3029 290a 2020 2020 2020 2020 7365 6c66  0)).        self
-00023510: 2e6d 696e 7569 742e 6472 6177 5f6d 6e70  .minuit.draw_mnp
-00023520: 726f 6669 6c65 2870 6e61 6d2c 2062 6f75  rofile(pnam, bou
-00023530: 6e64 3d72 616e 6765 2c20 7369 7a65 3d6e  nd=range, size=n
-00023540: 706f 696e 7473 2c20 7375 6274 7261 6374  points, subtract
-00023550: 5f6d 696e 3d54 7275 6529 0a0a 2020 2020  _min=True)..    
-00023560: 2020 2020 6966 2073 656c 662e 4572 7244      if self.ErrD
-00023570: 6566 203d 3d20 313a 0a20 2020 2020 2020  ef == 1:.       
-00023580: 2020 2020 2079 6c61 6265 6c20 3d20 2224       ylabel = "$
-00023590: 5c44 656c 7461 2028 2d32 5c6c 6e5c 6361  \Delta (-2\ln\ca
-000235a0: 6c7b 4c7d 2924 220a 2020 2020 2020 2020  l{L})$".        
-000235b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000235c0: 2020 796c 6162 656c 203d 2022 245c 4465    ylabel = "$\De
-000235d0: 6c74 6120 282d 5c6c 6e5c 6361 6c7b 4c7d  lta (-\ln\cal{L}
-000235e0: 2924 220a 2020 2020 2020 2020 706c 742e  )$".        plt.
-000235f0: 796c 6162 656c 2879 6c61 6265 6c29 0a20  ylabel(ylabel). 
-00023600: 2020 2020 2020 2072 6574 7572 6e20 6669         return fi
-00023610: 670a 0a20 2020 2064 6566 2070 6c6f 745f  g..    def plot_
-00023620: 636c 436f 6e74 6f75 7228 7365 6c66 2c20  clContour(self, 
-00023630: 706e 616d 312c 2070 6e61 6d32 2c20 636c  pnam1, pnam2, cl
-00023640: 293a 0a20 2020 2020 2020 2022 2222 706c  ):.        """pl
-00023650: 6f74 2061 2063 6f6e 746f 7572 206f 6620  ot a contour of 
-00023660: 7061 7261 6d65 7465 7273 2070 6e61 6d31  parameters pnam1
-00023670: 2061 6e64 2070 6e61 6d32 0a20 2020 2020   and pnam2.     
-00023680: 2020 2077 6974 6820 636f 6e66 6964 656e     with confiden
-00023690: 6365 206c 6576 656c 2873 2920 636c 0a20  ce level(s) cl. 
-000236a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000236b0: 2020 2069 6620 7365 6c66 2e69 6d69 6e75     if self.iminu
-000236c0: 6974 5f76 6572 7369 6f6e 203c 2022 3222  it_version < "2"
-000236d0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-000236e0: 696e 7428 2221 2121 2070 6c6f 745f 636c  int("!!! plot_cl
-000236f0: 436f 6e74 6f75 7220 6e6f 7420 696d 706c  Contour not impl
-00023700: 656d 656e 7465 6420 766f 7220 696d 696e  emented vor imin
-00023710: 7569 7420 7665 7273 2e3c 3222 290a 2020  uit vers.<2").  
-00023720: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00023730: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00023740: 2020 2020 2020 2020 2020 2066 6967 203d             fig =
-00023750: 2070 6c74 2e66 6967 7572 6528 0a20 2020   plt.figure(.   
-00023760: 2020 2020 2020 2020 2020 2020 206e 756d               num
-00023770: 3d22 436f 6e74 6f75 7228 7329 2022 202b  ="Contour(s) " +
-00023780: 2070 6e61 6d31 202b 2022 2076 732e 2022   pnam1 + " vs. "
-00023790: 202b 2070 6e61 6d32 2c20 6669 6773 697a   + pnam2, figsiz
-000237a0: 653d 2835 2e30 2c20 352e 3029 0a20 2020  e=(5.0, 5.0).   
-000237b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000237c0: 2020 2020 2020 2073 656c 662e 6d69 6e75         self.minu
-000237d0: 6974 2e64 7261 775f 6d6e 636f 6e74 6f75  it.draw_mncontou
-000237e0: 7228 706e 616d 312c 2070 6e61 6d32 2c20  r(pnam1, pnam2, 
-000237f0: 636c 3d63 6c29 0a20 2020 2020 2020 2020  cl=cl).         
-00023800: 2020 2072 6574 7572 6e20 6669 670a 0a20     return fig.. 
-00023810: 2020 2064 6566 2070 6c6f 745f 6e73 6967     def plot_nsig
-00023820: 436f 6e74 6f75 7228 7365 6c66 2c20 706e  Contour(self, pn
-00023830: 616d 312c 2070 6e61 6d32 2c20 6e73 6967  am1, pnam2, nsig
-00023840: 293a 0a20 2020 2020 2020 2022 2222 706c  ):.        """pl
-00023850: 6f74 206e 7369 6720 636f 6e74 6f75 7273  ot nsig contours
-00023860: 206f 6620 7061 7261 6d65 7465 7273 2070   of parameters p
-00023870: 6e61 6d31 2061 6e64 2070 6e61 6d32 2222  nam1 and pnam2""
-00023880: 220a 2020 2020 2020 2020 6669 6720 3d20  ".        fig = 
-00023890: 706c 742e 6669 6775 7265 280a 2020 2020  plt.figure(.    
-000238a0: 2020 2020 2020 2020 6e75 6d3d 2243 6f6e          num="Con
-000238b0: 746f 7572 2873 2920 2220 2b20 706e 616d  tour(s) " + pnam
-000238c0: 3120 2b20 2220 7673 2e20 2220 2b20 706e  1 + " vs. " + pn
-000238d0: 616d 322c 2066 6967 7369 7a65 3d28 352e  am2, figsize=(5.
-000238e0: 302c 2035 2e30 290a 2020 2020 2020 2020  0, 5.0).        
-000238f0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00023900: 662e 696d 696e 7569 745f 7665 7273 696f  f.iminuit_versio
-00023910: 6e20 3c20 2232 223a 0a20 2020 2020 2020  n < "2":.       
-00023920: 2020 2020 2073 656c 662e 6d69 6e75 6974       self.minuit
-00023930: 2e64 7261 775f 6d6e 636f 6e74 6f75 7228  .draw_mncontour(
-00023940: 706e 616d 312c 2070 6e61 6d32 2c20 6e73  pnam1, pnam2, ns
-00023950: 6967 6d61 3d6e 7369 6729 0a20 2020 2020  igma=nsig).     
-00023960: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00023970: 2020 2020 206e 7320 3d20 7261 6e67 6528       ns = range(
-00023980: 312c 206e 7369 6720 2b20 3129 0a20 2020  1, nsig + 1).   
-00023990: 2020 2020 2020 2020 2064 6368 6932 203d           dchi2 =
-000239a0: 206e 702e 6172 7261 7928 6e73 2920 2a2a   np.array(ns) **
-000239b0: 2032 0a20 2020 2020 2020 2020 2020 2063   2.            c
-000239c0: 6c20 3d20 7365 6c66 2e43 6869 3232 434c  l = self.Chi22CL
-000239d0: 2864 6368 6932 290a 2020 2020 2020 2020  (dchi2).        
-000239e0: 2020 2020 7365 6c66 2e6d 696e 7569 742e      self.minuit.
-000239f0: 6472 6177 5f6d 6e63 6f6e 746f 7572 2870  draw_mncontour(p
-00023a00: 6e61 6d31 2c20 706e 616d 322c 2063 6c3d  nam1, pnam2, cl=
-00023a10: 636c 290a 2020 2020 2020 2020 7265 7475  cl).        retu
-00023a20: 726e 2066 6967 0a0a 2020 2020 4073 7461  rn fig..    @sta
-00023a30: 7469 636d 6574 686f 640a 2020 2020 6465  ticmethod.    de
-00023a40: 6620 6368 6932 7072 6228 6368 6932 2c20  f chi2prb(chi2, 
-00023a50: 6e64 6f66 293a 0a20 2020 2020 2020 2022  ndof):.        "
-00023a60: 2222 4361 6c63 756c 6174 6520 6368 6932  ""Calculate chi2
-00023a70: 2d70 726f 6261 6269 6c69 7479 2066 726f  -probability fro
-00023a80: 6d20 6368 6932 2061 6e64 2064 6567 7265  m chi2 and degre
-00023a90: 6573 206f 6620 6672 6565 646f 6d22 2222  es of freedom"""
-00023aa0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00023ab0: 312e 3020 2d20 7374 6174 732e 6368 6932  1.0 - stats.chi2
-00023ac0: 2e63 6466 2863 6869 322c 206e 646f 6629  .cdf(chi2, ndof)
-00023ad0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00023ae0: 686f 640a 2020 2020 6465 6620 434c 3243  hod.    def CL2C
-00023af0: 6869 3228 434c 293a 0a20 2020 2020 2020  hi2(CL):.       
-00023b00: 2022 2222 6361 6c63 756c 6174 6520 4465   """calculate De
-00023b10: 6c74 6143 6869 3220 6672 6f6d 2063 6f6e  ltaChi2 from con
-00023b20: 6669 6465 6e63 6520 6c65 7665 6c20 434c  fidence level CL
-00023b30: 2066 6f72 2032 2d64 696d 2063 6f6e 746f   for 2-dim conto
-00023b40: 7572 7322 2222 0a20 2020 2020 2020 2072  urs""".        r
-00023b50: 6574 7572 6e20 2d32 2e30 202a 206e 702e  eturn -2.0 * np.
-00023b60: 6c6f 6728 312e 3020 2d20 434c 290a 0a20  log(1.0 - CL).. 
-00023b70: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
-00023b80: 0a20 2020 2064 6566 2043 6869 3232 434c  .    def Chi22CL
-00023b90: 2864 6332 293a 0a20 2020 2020 2020 2022  (dc2):.        "
-00023ba0: 2222 6361 6c63 756c 6174 6520 636f 6e66  ""calculate conf
-00023bb0: 6964 656e 6365 206c 6576 656c 2043 4c20  idence level CL 
-00023bc0: 6672 6f6d 2044 656c 7461 4368 6932 2066  from DeltaChi2 f
-00023bd0: 6f72 2032 2d64 696d 2063 6f6e 746f 7572  or 2-dim contour
-00023be0: 7322 2222 0a20 2020 2020 2020 2072 6574  s""".        ret
-00023bf0: 7572 6e20 312e 3020 2d20 6e70 2e65 7870  urn 1.0 - np.exp
-00023c00: 282d 6463 3220 2f20 322e 3029 0a0a 0a69  (-dc2 / 2.0)...i
-00023c10: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
-00023c20: 5f6d 6169 6e5f 5f22 3a20 2023 202d 2d2d  _main__":  # ---
-00023c30: 2069 6e74 6572 6661 6365 2061 6e64 2065   interface and e
-00023c40: 7861 6d70 6c65 0a0a 2020 2020 6465 6620  xample..    def 
-00023c50: 6578 616d 706c 655f 7879 4669 7428 293a  example_xyFit():
-00023c60: 0a20 2020 2020 2020 2023 0a20 2020 2020  .        #.     
-00023c70: 2020 2023 202a 2a2a 2045 7861 6d70 6c65     # *** Example
-00023c80: 206f 6620 616e 2061 7070 6c69 6361 7469   of an applicati
-00023c90: 6f6e 206f 6620 7068 7946 6974 2e78 7946  on of phyFit.xyF
-00023ca0: 6974 2829 0a20 2020 2020 2020 2023 0a20  it().        #. 
-00023cb0: 2020 2020 2020 2023 2064 6566 696e 6520         # define 
-00023cc0: 7468 6520 6d6f 6465 6c20 6675 6e63 7469  the model functi
-00023cd0: 6f6e 2074 6f20 6669 740a 2020 2020 2020  on to fit.      
-00023ce0: 2020 6465 6620 6578 705f 6d6f 6465 6c28    def exp_model(
-00023cf0: 782c 2041 3d31 2e30 2c20 7830 3d31 2e30  x, A=1.0, x0=1.0
-00023d00: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00023d10: 6574 7572 6e20 4120 2a20 6e70 2e65 7870  eturn A * np.exp
-00023d20: 282d 7820 2f20 7830 290a 0a20 2020 2020  (-x / x0)..     
-00023d30: 2020 2023 2061 6e6f 7468 6572 206d 6f64     # another mod
-00023d40: 656c 2066 756e 6374 696f 6e0a 2020 2020  el function.    
-00023d50: 2020 2020 6465 6620 706f 6c79 325f 6d6f      def poly2_mo
-00023d60: 6465 6c28 782c 2061 3d30 2e31 2c20 623d  del(x, a=0.1, b=
-00023d70: 312e 302c 2063 3d31 2e30 293a 0a20 2020  1.0, c=1.0):.   
-00023d80: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00023d90: 6120 2a20 782a 2a32 202b 2062 202a 2078  a * x**2 + b * x
-00023da0: 202b 2063 0a0a 2020 2020 2020 2020 2320   + c..        # 
-00023db0: 7365 7420 6d6f 6465 6c20 746f 2075 7365  set model to use
-00023dc0: 2069 6e20 6669 740a 2020 2020 2020 2020   in fit.        
-00023dd0: 6669 746d 6f64 656c 203d 2065 7870 5f6d  fitmodel = exp_m
-00023de0: 6f64 656c 2020 2320 616c 736f 2074 7279  odel  # also try
-00023df0: 2070 6f6c 7932 5f6d 6f64 656c 2021 0a0a   poly2_model !..
-00023e00: 2020 2020 2020 2020 2320 7468 6520 6461          # the da
-00023e10: 7461 202e 2e2e 0a20 2020 2020 2020 2064  ta ....        d
-00023e20: 6174 615f 7820 3d20 5b30 2e30 2c20 302e  ata_x = [0.0, 0.
-00023e30: 322c 2030 2e34 2c20 302e 362c 2030 2e38  2, 0.4, 0.6, 0.8
-00023e40: 2c20 312e 302c 2031 2e32 2c20 312e 342c  , 1.0, 1.2, 1.4,
-00023e50: 2031 2e36 2c20 312e 382c 2032 2e30 2c20   1.6, 1.8, 2.0, 
-00023e60: 322e 322c 2032 2e34 2c20 322e 365d 0a20  2.2, 2.4, 2.6]. 
-00023e70: 2020 2020 2020 2064 6174 615f 7920 3d20         data_y = 
-00023e80: 5b0a 2020 2020 2020 2020 2020 2020 312e  [.            1.
-00023e90: 3134 392c 0a20 2020 2020 2020 2020 2020  149,.           
-00023ea0: 2030 2e37 3132 2c0a 2020 2020 2020 2020   0.712,.        
-00023eb0: 2020 2020 302e 3830 332c 0a20 2020 2020      0.803,.     
-00023ec0: 2020 2020 2020 2030 2e34 3634 2c0a 2020         0.464,.  
-00023ed0: 2020 2020 2020 2020 2020 302e 3339 382c            0.398,
-00023ee0: 0a20 2020 2020 2020 2020 2020 2030 2e33  .            0.3
-00023ef0: 3534 2c0a 2020 2020 2020 2020 2020 2020  54,.            
-00023f00: 302e 3134 382c 0a20 2020 2020 2020 2020  0.148,.         
-00023f10: 2020 2030 2e33 3238 2c0a 2020 2020 2020     0.328,.      
-00023f20: 2020 2020 2020 302e 3138 312c 0a20 2020        0.181,.   
-00023f30: 2020 2020 2020 2020 2030 2e31 3430 2c0a           0.140,.
-00023f40: 2020 2020 2020 2020 2020 2020 302e 3036              0.06
-00023f50: 352c 0a20 2020 2020 2020 2020 2020 2030  5,.            0
-00023f60: 2e30 3035 2c0a 2020 2020 2020 2020 2020  .005,.          
-00023f70: 2020 2d30 2e30 3035 2c0a 2020 2020 2020    -0.005,.      
-00023f80: 2020 2020 2020 302e 3131 362c 0a20 2020        0.116,.   
-00023f90: 2020 2020 205d 0a20 2020 2020 2020 2023       ].        #
-00023fa0: 202e 2e2e 2061 6e64 2075 6e63 6572 7461   ... and uncerta
-00023fb0: 6974 6965 730a 2020 2020 2020 2020 7361  ities.        sa
-00023fc0: 6273 7920 3d20 302e 3037 2020 2320 696e  bsy = 0.07  # in
-00023fd0: 6465 7065 6e64 656e 7420 790a 2020 2020  dependent y.    
-00023fe0: 2020 2020 7372 656c 7920 3d20 302e 3035      srely = 0.05
-00023ff0: 2020 2320 3525 206f 6620 6d6f 6465 6c20    # 5% of model 
-00024000: 7661 6c75 650a 2020 2020 2020 2020 6361  value.        ca
-00024010: 6273 7920 3d20 302e 3034 2020 2320 636f  bsy = 0.04  # co
-00024020: 7272 656c 6174 6564 0a20 2020 2020 2020  rrelated.       
-00024030: 2063 7265 6c79 203d 2030 2e30 3320 2023   crely = 0.03  #
-00024040: 2033 2520 6f66 206d 6f64 656c 2076 616c   3% of model val
-00024050: 7565 2063 6f72 7265 6c61 7465 640a 2020  ue correlated.  
-00024060: 2020 2020 2020 7361 6273 7820 3d20 302e        sabsx = 0.
-00024070: 3035 2020 2320 696e 6465 7065 6e64 656e  05  # independen
-00024080: 7420 780a 2020 2020 2020 2020 7372 656c  t x.        srel
-00024090: 7820 3d20 302e 3034 2020 2320 3425 206f  x = 0.04  # 4% o
-000240a0: 6620 780a 2020 2020 2020 2020 6361 6273  f x.        cabs
-000240b0: 7820 3d20 302e 3033 2020 2320 636f 7272  x = 0.03  # corr
-000240c0: 656c 6174 6564 2078 0a20 2020 2020 2020  elated x.       
-000240d0: 2063 7265 6c78 203d 2030 2e30 3220 2023   crelx = 0.02  #
-000240e0: 2032 2520 6f66 2078 2063 6f72 7265 6c61   2% of x correla
-000240f0: 7465 640a 0a20 2020 2020 2020 2023 2070  ted..        # p
-00024100: 6572 666f 726d 2066 6974 2074 6f20 6461  erform fit to da
-00024110: 7461 2077 6974 6820 6675 6e63 7469 6f6e  ta with function
-00024120: 2078 7946 6974 2075 7369 6e67 2063 6c61   xyFit using cla
-00024130: 7373 206d 6e46 6974 0a20 2020 2020 2020  ss mnFit.       
-00024140: 2072 6573 756c 7444 6963 7420 3d20 7879   resultDict = xy
-00024150: 4669 7428 0a20 2020 2020 2020 2020 2020  Fit(.           
-00024160: 2066 6974 6d6f 6465 6c2c 0a20 2020 2020   fitmodel,.     
-00024170: 2020 2020 2020 2064 6174 615f 782c 0a20         data_x,. 
-00024180: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00024190: 792c 0a20 2020 2020 2020 2020 2020 2073  y,.            s
-000241a0: 783d 7361 6273 782c 0a20 2020 2020 2020  x=sabsx,.       
-000241b0: 2020 2020 2073 793d 7361 6273 792c 0a20       sy=sabsy,. 
-000241c0: 2020 2020 2020 2020 2020 2073 7265 6c78             srelx
-000241d0: 3d73 7265 6c78 2c0a 2020 2020 2020 2020  =srelx,.        
-000241e0: 2020 2020 7372 656c 793d 7372 656c 792c      srely=srely,
-000241f0: 0a20 2020 2020 2020 2020 2020 2078 6162  .            xab
-00024200: 7363 6f72 3d63 6162 7378 2c0a 2020 2020  scor=cabsx,.    
-00024210: 2020 2020 2020 2020 7872 656c 636f 723d          xrelcor=
-00024220: 6372 656c 782c 0a20 2020 2020 2020 2020  crelx,.         
-00024230: 2020 2079 6162 7363 6f72 3d63 6162 7379     yabscor=cabsy
-00024240: 2c0a 2020 2020 2020 2020 2020 2020 7972  ,.            yr
-00024250: 656c 636f 723d 6372 656c 792c 0a20 2020  elcor=crely,.   
-00024260: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-00024270: 2020 2020 2020 2020 2020 2020 7030 3d28              p0=(
-00024280: 312e 2c20 302e 3529 2c0a 2020 2020 2020  1., 0.5),.      
-00024290: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-000242a0: 2020 2020 2020 2020 2063 6f6e 7374 7261           constra
-000242b0: 696e 7473 3d5b 2741 272c 2031 2e2c 2030  ints=['A', 1., 0
-000242c0: 2e30 335d 2c0a 2020 2020 2020 2020 2020  .03],.          
-000242d0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-000242e0: 2020 2020 2063 6f6e 7374 7261 696e 7473       constraints
-000242f0: 3d5b 302c 2031 2e2c 2030 2e30 335d 2028  =[0, 1., 0.03] (
-00024300: 616c 7465 726e 6174 6976 6529 0a20 2020  alternative).   
-00024310: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-00024320: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
-00024330: 7473 3d28 2741 272c 2030 2e2c 204e 6f6e  ts=('A', 0., Non
-00024340: 6529 2c20 2023 2070 6172 616d 6574 6572  e),  # parameter
-00024350: 206c 696d 6974 730a 2020 2020 2020 2020   limits.        
-00024360: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00024370: 2020 2020 2020 2066 6978 5061 7273 203d         fixPars =
-00024380: 205b 2741 275d 2c20 2020 2020 2020 2020   ['A'],         
-00024390: 2320 6669 7820 7061 7261 6d65 7465 7228  # fix parameter(
-000243a0: 7329 0a20 2020 2020 2020 2020 2020 2075  s).            u
-000243b0: 7365 5f6e 6567 4c6f 674c 3d54 7275 652c  se_negLogL=True,
-000243c0: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
-000243d0: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
-000243e0: 2020 2020 706c 6f74 5f62 616e 643d 5472      plot_band=Tr
-000243f0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00024400: 706c 6f74 5f63 6f72 3d46 616c 7365 2c0a  plot_cor=False,.
-00024410: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-00024420: 706c 6f74 733d 4661 6c73 652c 0a20 2020  plots=False,.   
-00024430: 2020 2020 2020 2020 2071 7569 6574 3d46           quiet=F
-00024440: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00024450: 2020 6178 6973 5f6c 6162 656c 733d 5b22    axis_labels=["
-00024460: 7822 2c20 2279 2020 205c 2020 6628 782c  x", "y   \  f(x,
-00024470: 202a 7061 7229 225d 2c0a 2020 2020 2020   *par)"],.      
-00024480: 2020 2020 2020 6461 7461 5f6c 6567 656e        data_legen
-00024490: 643d 2272 616e 646f 6d20 6461 7461 222c  d="random data",
-000244a0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-000244b0: 656c 5f6c 6567 656e 643d 226d 6f64 656c  el_legend="model
-000244c0: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
-000244d0: 2020 2020 2070 6c74 2e73 7570 7469 746c       plt.suptitl
-000244e0: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-000244f0: 6d6e 4669 7420 6578 616d 706c 653a 2066  mnFit example: f
-00024500: 6974 2074 6f20 782d 7920 6461 7461 222c  it to x-y data",
-00024510: 2073 697a 653d 2278 782d 6c61 7267 6522   size="xx-large"
-00024520: 2c20 636f 6c6f 723d 2264 6172 6b62 6c75  , color="darkblu
-00024530: 6522 0a20 2020 2020 2020 2029 0a0a 2020  e".        )..  
-00024540: 2020 2020 2020 2320 5072 696e 7420 7265        # Print re
-00024550: 7375 6c74 730a 2020 2020 2020 2020 7076  sults.        pv
-00024560: 616c 732c 2070 6572 7273 2c20 636f 722c  als, perrs, cor,
-00024570: 2063 6869 322c 2070 6e61 6d73 203d 2072   chi2, pnams = r
-00024580: 6573 756c 7444 6963 742e 7661 6c75 6573  esultDict.values
-00024590: 2829 0a20 2020 2020 2020 2070 7269 6e74  ().        print
-000245a0: 2822 5c6e 2a3d 3d2a 2078 7946 6974 2052  ("\n*==* xyFit R
-000245b0: 6573 756c 743a 2229 0a20 2020 2020 2020  esult:").       
-000245c0: 2070 7269 6e74 2822 2070 6172 616d 6574   print(" paramet
-000245d0: 6572 206e 616d 6573 3a20 2020 2020 2020  er names:       
-000245e0: 222c 2070 6e61 6d73 290a 2020 2020 2020  ", pnams).      
-000245f0: 2020 7072 696e 7428 2220 6368 6932 3a20    print(" chi2: 
-00024600: 7b3a 2e33 677d 222e 666f 726d 6174 2863  {:.3g}".format(c
-00024610: 6869 3229 290a 2020 2020 2020 2020 7072  hi2)).        pr
-00024620: 696e 7428 2220 7061 7261 6d65 7465 7220  int(" parameter 
-00024630: 7661 6c75 6573 3a20 2020 2020 2022 2c20  values:      ", 
-00024640: 7076 616c 7329 0a20 2020 2020 2020 2070  pvals).        p
-00024650: 7269 6e74 2822 206e 6567 2e20 7061 7261  rint(" neg. para
-00024660: 6d65 7465 7220 6572 726f 7273 3a20 222c  meter errors: ",
-00024670: 2070 6572 7273 5b3a 2c20 305d 290a 2020   perrs[:, 0]).  
-00024680: 2020 2020 2020 7072 696e 7428 2220 706f        print(" po
-00024690: 732e 2070 6172 616d 6574 6572 2065 7272  s. parameter err
-000246a0: 6f72 733a 2022 2c20 7065 7272 735b 3a2c  ors: ", perrs[:,
-000246b0: 2031 5d29 0a20 2020 2020 2020 2070 7269   1]).        pri
-000246c0: 6e74 2822 2063 6f72 7265 6c61 7469 6f6e  nt(" correlation
-000246d0: 7320 3a20 5c6e 222c 2063 6f72 290a 0a20  s : \n", cor).. 
-000246e0: 2020 2064 6566 2065 7861 6d70 6c65 5f69     def example_i
-000246f0: 6e64 6578 6564 4669 7428 293a 0a20 2020  ndexedFit():.   
-00024700: 2020 2020 2023 0a20 2020 2020 2020 2023       #.        #
-00024710: 202a 2a2a 2045 7861 6d70 6c65 206f 6620   *** Example of 
-00024720: 616e 2061 7070 6c69 6361 7469 6f6e 206f  an application o
-00024730: 6620 7068 7946 6974 2e78 4669 7428 2920  f phyFit.xFit() 
-00024740: 746f 2066 6974 2069 6e64 6578 6564 2064  to fit indexed d
-00024750: 6174 610a 2020 2020 2020 2020 230a 2020  ata.        #.  
-00024760: 2020 2020 2020 2320 2020 2020 436f 6f72        #     Coor
-00024770: 6469 6e61 7465 7320 696e 2072 2d70 6869  dinates in r-phi
-00024780: 2061 7265 2061 7665 7261 6765 6420 616e   are averaged an
-00024790: 6420 7472 616e 7366 6f72 6d65 6420 746f  d transformed to
-000247a0: 2063 6172 7465 7369 616e 0a0a 2020 2020   cartesian..    
-000247b0: 2020 2020 6465 6620 6361 7274 6573 6961      def cartesia
-000247c0: 6e5f 746f 5f70 6f6c 6172 2864 6174 612c  n_to_polar(data,
-000247d0: 2078 3d31 2e30 2c20 793d 312e 3029 3a0a   x=1.0, y=1.0):.
-000247e0: 2020 2020 2020 2020 2020 2020 2320 6465              # de
-000247f0: 7465 726d 696e 6520 706f 6c61 7220 636f  termine polar co
-00024800: 6f72 6469 6e61 7473 2066 726f 6d20 6361  ordinats from ca
-00024810: 7274 6573 6961 6e20 2878 2c79 290a 2020  rtesian (x,y).  
-00024820: 2020 2020 2020 2020 2020 6e6d 203d 206c            nm = l
-00024830: 656e 2864 6174 6129 202f 2f20 3220 2023  en(data) // 2  #
-00024840: 2065 7870 6563 7420 7477 6f20 6172 7261   expect two arra
-00024850: 7973 2077 6974 6820 6d65 6173 7572 656d  ys with measurem
-00024860: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00024870: 2072 203d 206e 702e 7371 7274 2878 202a   r = np.sqrt(x *
-00024880: 2078 202b 2079 202a 2079 2920 2a20 6e70   x + y * y) * np
-00024890: 2e6f 6e65 7328 6e6d 290a 2020 2020 2020  .ones(nm).      
-000248a0: 2020 2020 2020 7068 6920 3d20 6e70 2e61        phi = np.a
-000248b0: 7263 7461 6e32 2879 2c20 7829 202a 206e  rctan2(y, x) * n
-000248c0: 702e 6f6e 6573 286e 6d29 0a20 2020 2020  p.ones(nm).     
-000248d0: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
-000248e0: 2e63 6f6e 6361 7465 6e61 7465 2828 722c  .concatenate((r,
-000248f0: 2070 6869 2929 0a0a 2020 2020 2020 2020   phi))..        
-00024900: 2320 6578 616d 706c 653a 2028 722c 2070  # example: (r, p
-00024910: 6869 2920 6f66 2074 776f 2073 7061 6365  hi) of two space
-00024920: 2070 6f69 6e74 7320 696e 2070 6f6c 6172   points in polar
-00024930: 2063 6f6f 7264 696e 6174 6573 0a20 2020   coordinates.   
-00024940: 2020 2020 2070 6172 7320 3d20 6e70 2e61       pars = np.a
-00024950: 7272 6179 285b 302e 392c 2030 2e38 372c  rray([0.9, 0.87,
-00024960: 2030 2e37 3535 2c20 302e 3739 305d 290a   0.755, 0.790]).
-00024970: 2020 2020 2020 2020 7075 6e63 7320 3d20          puncs = 
-00024980: 6e70 2e61 7272 6179 285b 302e 3032 372c  np.array([0.027,
-00024990: 2030 2e30 3233 2c20 302e 3136 2c20 302e   0.023, 0.16, 0.
-000249a0: 3133 5d29 0a0a 2020 2020 2020 2020 2320  13])..        # 
-000249b0: 7065 7266 6f72 6d20 6669 7420 746f 2064  perform fit to d
-000249c0: 6174 6120 7769 7468 2066 756e 6374 696f  ata with functio
-000249d0: 6e20 7846 6974 2075 7369 6e67 2063 6c61  n xFit using cla
-000249e0: 7373 206d 6e46 6974 0a20 2020 2020 2020  ss mnFit.       
-000249f0: 2072 6573 756c 7444 6963 7420 3d20 7846   resultDict = xF
-00024a00: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
-00024a10: 6361 7274 6573 6961 6e5f 746f 5f70 6f6c  cartesian_to_pol
-00024a20: 6172 2c0a 2020 2020 2020 2020 2020 2020  ar,.            
-00024a30: 7061 7273 2c0a 2020 2020 2020 2020 2020  pars,.          
-00024a40: 2020 733d 7075 6e63 732c 0a20 2020 2020    s=puncs,.     
-00024a50: 2020 2020 2020 2073 7265 6c3d 4e6f 6e65         srel=None
-00024a60: 2c0a 2020 2020 2020 2020 2020 2020 7361  ,.            sa
-00024a70: 6273 636f 723d 4e6f 6e65 2c0a 2020 2020  bscor=None,.    
-00024a80: 2020 2020 2020 2020 7372 656c 636f 723d          srelcor=
-00024a90: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00024aa0: 2020 6e61 6d65 733d 5b22 7222 2c20 2272    names=["r", "r
-00024ab0: 222c 2072 2224 5c76 6172 7068 6924 222c  ", r"$\varphi$",
-00024ac0: 2072 2224 5c76 6172 7068 6924 225d 2c0a   r"$\varphi$"],.
-00024ad0: 2020 2020 2020 2020 2020 2020 2320 7030              # p0
-00024ae0: 3d28 312e 2c20 312e 292c 0a20 2020 2020  =(1., 1.),.     
-00024af0: 2020 2020 2020 2075 7365 5f6e 6567 4c6f         use_negLo
-00024b00: 674c 3d54 7275 652c 0a20 2020 2020 2020  gL=True,.       
-00024b10: 2020 2020 2070 6c6f 743d 5472 7565 2c0a       plot=True,.
-00024b20: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
-00024b30: 5f62 616e 643d 5472 7565 2c0a 2020 2020  _band=True,.    
-00024b40: 2020 2020 2020 2020 706c 6f74 5f63 6f72          plot_cor
-00024b50: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-00024b60: 2020 2073 686f 7770 6c6f 7473 3d46 616c     showplots=Fal
-00024b70: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00024b80: 7175 6965 743d 4661 6c73 652c 0a20 2020  quiet=False,.   
-00024b90: 2020 2020 2020 2020 2061 7869 735f 6c61           axis_la
-00024ba0: 6265 6c73 3d5b 2249 6e64 6578 222c 2022  bels=["Index", "
-00024bb0: 7820 2020 5c20 2078 282a 7061 7229 225d  x   \  x(*par)"]
-00024bc0: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00024bd0: 7461 5f6c 6567 656e 643d 2250 6f6c 6172  ta_legend="Polar
-00024be0: 2044 6174 6122 2c0a 2020 2020 2020 2020   Data",.        
-00024bf0: 2020 2020 6d6f 6465 6c5f 6c65 6765 6e64      model_legend
-00024c00: 3d22 722d 7068 6920 6672 6f6d 2078 2d79  ="r-phi from x-y
-00024c10: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
-00024c20: 2020 2020 2070 6c74 2e73 7570 7469 746c       plt.suptitl
-00024c30: 6528 0a20 2020 2020 2020 2020 2020 2022  e(.            "
-00024c40: 6d6e 4669 7420 6578 616d 706c 653a 2066  mnFit example: f
-00024c50: 6974 2074 6f20 696e 6465 7865 6420 6461  it to indexed da
-00024c60: 7461 222c 2073 697a 653d 2278 782d 6c61  ta", size="xx-la
-00024c70: 7267 6522 2c20 636f 6c6f 723d 2264 6172  rge", color="dar
-00024c80: 6b62 6c75 6522 0a20 2020 2020 2020 2029  kblue".        )
-00024c90: 0a0a 2020 2020 2020 2020 2320 5072 696e  ..        # Prin
-00024ca0: 7420 7265 7375 6c74 730a 2020 2020 2020  t results.      
-00024cb0: 2020 7076 616c 732c 2070 6572 7273 2c20    pvals, perrs, 
-00024cc0: 636f 722c 2063 6869 322c 2070 6e61 6d73  cor, chi2, pnams
-00024cd0: 203d 2072 6573 756c 7444 6963 742e 7661   = resultDict.va
-00024ce0: 6c75 6573 2829 0a20 2020 2020 2020 2070  lues().        p
-00024cf0: 7269 6e74 2822 5c6e 2a3d 3d2a 2078 7946  rint("\n*==* xyF
-00024d00: 6974 2052 6573 756c 743a 2229 0a20 2020  it Result:").   
-00024d10: 2020 2020 2070 7269 6e74 2822 2070 6172       print(" par
-00024d20: 616d 6574 6572 206e 616d 6573 3a20 2020  ameter names:   
-00024d30: 2020 2020 222c 2070 6e61 6d73 290a 2020      ", pnams).  
-00024d40: 2020 2020 2020 7072 696e 7428 2220 6368        print(" ch
-00024d50: 6932 3a20 7b3a 2e33 677d 222e 666f 726d  i2: {:.3g}".form
-00024d60: 6174 2863 6869 3229 290a 2020 2020 2020  at(chi2)).      
-00024d70: 2020 7072 696e 7428 2220 7061 7261 6d65    print(" parame
-00024d80: 7465 7220 7661 6c75 6573 3a20 2020 2020  ter values:     
-00024d90: 2022 2c20 7076 616c 7329 0a20 2020 2020   ", pvals).     
-00024da0: 2020 2070 7269 6e74 2822 206e 6567 2e20     print(" neg. 
-00024db0: 7061 7261 6d65 7465 7220 6572 726f 7273  parameter errors
-00024dc0: 3a20 222c 2070 6572 7273 5b3a 2c20 305d  : ", perrs[:, 0]
-00024dd0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
-00024de0: 2220 706f 732e 2070 6172 616d 6574 6572  " pos. parameter
-00024df0: 2065 7272 6f72 733a 2022 2c20 7065 7272   errors: ", perr
-00024e00: 735b 3a2c 2031 5d29 0a20 2020 2020 2020  s[:, 1]).       
-00024e10: 2070 7269 6e74 2822 2063 6f72 7265 6c61   print(" correla
-00024e20: 7469 6f6e 7320 3a20 5c6e 222c 2063 6f72  tions : \n", cor
-00024e30: 290a 0a20 2020 2064 6566 2065 7861 6d70  )..    def examp
-00024e40: 6c65 5f68 6973 746f 6772 616d 4669 7428  le_histogramFit(
-00024e50: 293a 0a20 2020 2020 2020 2023 0a20 2020  ):.        #.   
-00024e60: 2020 2020 2023 202a 2a2a 2048 6973 746f       # *** Histo
-00024e70: 6772 616d 2046 6974 3a20 4578 616d 706c  gram Fit: Exampl
-00024e80: 6520 6f66 2061 6e20 6170 706c 6963 6174  e of an applicat
-00024e90: 696f 6e20 6f66 2070 6879 4669 742e 6846  ion of phyFit.hF
-00024ea0: 6974 2829 0a20 2020 2020 2020 2023 0a0a  it().        #..
-00024eb0: 2020 2020 2020 2020 2320 2020 2023 2064          #    # d
-00024ec0: 6566 696e 6520 7468 6520 6d6f 6465 6c20  efine the model 
-00024ed0: 6675 6e63 7469 6f6e 2074 6f20 6669 740a  function to fit.
-00024ee0: 2020 2020 2020 2020 6465 6620 5370 6c75          def Splu
-00024ef0: 7342 5f6d 6f64 656c 2878 2c20 6d75 3d36  sB_model(x, mu=6
-00024f00: 2e39 3837 2c20 7369 676d 613d 302e 352c  .987, sigma=0.5,
-00024f10: 2061 3d30 2e30 2c20 733d 302e 3229 3a0a   a=0.0, s=0.2):.
-00024f20: 2020 2020 2020 2020 2020 2020 2222 2270              """p
-00024f30: 6466 206f 6620 6120 4761 7573 7369 616e  df of a Gaussian
-00024f40: 2073 6967 6e61 6c20 6f6e 2074 6f70 206f   signal on top o
-00024f50: 6620 666c 6174 2062 6163 6b67 726f 756e  f flat backgroun
-00024f60: 6422 2222 0a20 2020 2020 2020 2020 2020  d""".           
-00024f70: 206e 6f72 6d61 6c20 3d20 6e70 2e65 7870   normal = np.exp
-00024f80: 282d 302e 3520 2a20 2828 7820 2d20 6d75  (-0.5 * ((x - mu
-00024f90: 2920 2f20 7369 676d 6129 202a 2a20 3229  ) / sigma) ** 2)
-00024fa0: 202f 206e 702e 7371 7274 280a 2020 2020   / np.sqrt(.    
-00024fb0: 2020 2020 2020 2020 2020 2020 322e 3020              2.0 
-00024fc0: 2a20 6e70 2e70 6920 2a20 7369 676d 612a  * np.pi * sigma*
-00024fd0: 2a32 0a20 2020 2020 2020 2020 2020 2029  *2.            )
-00024fe0: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
-00024ff0: 6561 7220 3d20 2861 202a 2028 786d 7820  ear = (a * (xmx 
-00025000: 2b20 786d 6e29 202f 2032 202b 2031 2e30  + xmn) / 2 + 1.0
-00025010: 2920 2f20 2878 6d78 202d 2078 6d6e 290a  ) / (xmx - xmn).
-00025020: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00025030: 726e 2073 202a 206e 6f72 6d61 6c20 2b20  rn s * normal + 
-00025040: 2831 202d 2073 2920 2a20 6c69 6e65 6172  (1 - s) * linear
-00025050: 0a0a 2020 2020 2020 2020 6e62 696e 7320  ..        nbins 
-00025060: 3d20 3430 0a20 2020 2020 2020 2078 6d6e  = 40.        xmn
-00025070: 203d 2031 0a20 2020 2020 2020 2078 6d78   = 1.        xmx
-00025080: 203d 2031 300a 2020 2020 2020 2020 6265   = 10.        be
-00025090: 6467 6573 203d 206e 702e 6c69 6e73 7061  dges = np.linspa
-000250a0: 6365 2878 6d6e 2c20 786d 782c 206e 6269  ce(xmn, xmx, nbi
-000250b0: 6e73 202b 2031 290a 2020 2020 2020 2020  ns + 1).        
-000250c0: 6263 6f6e 7465 6e74 7320 3d20 6e70 2e61  bcontents = np.a
-000250d0: 7272 6179 280a 2020 2020 2020 2020 2020  rray(.          
-000250e0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000250f0: 2020 2020 312c 0a20 2020 2020 2020 2020      1,.         
-00025100: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00025110: 2020 2020 2020 2020 2020 312c 0a20 2020            1,.   
-00025120: 2020 2020 2020 2020 2020 2020 2032 2c0a               2,.
-00025130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025140: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-00025150: 2020 2032 2c0a 2020 2020 2020 2020 2020     2,.          
-00025160: 2020 2020 2020 342c 0a20 2020 2020 2020        4,.       
-00025170: 2020 2020 2020 2020 2031 2c0a 2020 2020           1,.    
-00025180: 2020 2020 2020 2020 2020 2020 302c 0a20              0,. 
-00025190: 2020 2020 2020 2020 2020 2020 2020 2033                 3
-000251a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000251b0: 2020 312c 0a20 2020 2020 2020 2020 2020    1,.           
-000251c0: 2020 2020 2031 2c0a 2020 2020 2020 2020       1,.        
-000251d0: 2020 2020 2020 2020 302c 0a20 2020 2020          0,.     
-000251e0: 2020 2020 2020 2020 2020 2032 2c0a 2020             2,.  
-000251f0: 2020 2020 2020 2020 2020 2020 2020 332c                3,
-00025200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025210: 2033 2c0a 2020 2020 2020 2020 2020 2020   3,.            
-00025220: 2020 2020 312c 0a20 2020 2020 2020 2020      1,.         
-00025230: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00025240: 2020 2020 2020 2020 2020 302c 0a20 2020            0,.   
-00025250: 2020 2020 2020 2020 2020 2020 2032 2c0a               2,.
-00025260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025270: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
-00025280: 2020 2032 2c0a 2020 2020 2020 2020 2020     2,.          
-00025290: 2020 2020 2020 332c 0a20 2020 2020 2020        3,.       
-000252a0: 2020 2020 2020 2020 2031 2c0a 2020 2020           1,.    
-000252b0: 2020 2020 2020 2020 2020 2020 312c 0a20              1,. 
-000252c0: 2020 2020 2020 2020 2020 2020 2020 2038                 8
-000252d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000252e0: 2020 362c 0a20 2020 2020 2020 2020 2020    6,.           
-000252f0: 2020 2020 2037 2c0a 2020 2020 2020 2020       7,.        
-00025300: 2020 2020 2020 2020 392c 0a20 2020 2020          9,.     
-00025310: 2020 2020 2020 2020 2020 2031 2c0a 2020             1,.  
-00025320: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-00025330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00025340: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
-00025350: 2020 2020 322c 0a20 2020 2020 2020 2020      2,.         
-00025360: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
-00025370: 2020 2020 2020 2020 2020 332c 0a20 2020            3,.   
-00025380: 2020 2020 2020 2020 2020 2020 2032 2c0a               2,.
-00025390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000253a0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-000253b0: 2020 2033 2c0a 2020 2020 2020 2020 2020     3,.          
-000253c0: 2020 2020 2020 322c 0a20 2020 2020 2020        2,.       
-000253d0: 2020 2020 2020 2020 2034 2c0a 2020 2020           4,.    
-000253e0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000253f0: 2020 290a 2020 2020 2020 2020 230a 2020    ).        #.  
-00025400: 2020 2020 2020 2320 2d2d 2d20 2070 6572        # ---  per
-00025410: 666f 726d 2066 6974 0a20 2020 2020 2020  form fit.       
-00025420: 2023 0a20 2020 2020 2020 2072 6573 756c   #.        resul
-00025430: 7444 6963 7420 3d20 6846 6974 280a 2020  tDict = hFit(.  
-00025440: 2020 2020 2020 2020 2020 5370 6c75 7342            SplusB
-00025450: 5f6d 6f64 656c 2c0a 2020 2020 2020 2020  _model,.        
-00025460: 2020 2020 6263 6f6e 7465 6e74 732c 0a20      bcontents,. 
-00025470: 2020 2020 2020 2020 2020 2062 6564 6765             bedge
-00025480: 732c 2020 2320 6269 6e20 656e 7472 6965  s,  # bin entrie
-00025490: 7320 616e 6420 6269 6e20 6564 6765 730a  s and bin edges.
-000254a0: 2020 2020 2020 2020 2020 2020 7030 3d4e              p0=N
-000254b0: 6f6e 652c 2020 2320 696e 6974 6961 6c20  one,  # initial 
-000254c0: 6775 6573 7320 666f 7220 7061 7261 6d65  guess for parame
-000254d0: 7465 7220 7661 6c75 6573 0a20 2020 2020  ter values.     
-000254e0: 2020 2020 2020 2023 2020 2020 2063 6f6e         #     con
-000254f0: 7374 7261 696e 7473 3d5b 2773 272c 2076  straints=['s', v
-00025500: 616c 202c 2065 7272 205d 2c20 2020 2320  al , err ],   # 
-00025510: 636f 6e73 7472 6169 6e74 7320 7769 7468  constraints with
-00025520: 696e 2065 7272 6f72 730a 2020 2020 2020  in errors.      
-00025530: 2020 2020 2020 6669 7850 6172 733d 5b22        fixPars=["
-00025540: 6122 5d2c 2020 2320 6669 7820 7061 7261  a"],  # fix para
-00025550: 6d65 7465 7228 7329 0a20 2020 2020 2020  meter(s).       
-00025560: 2020 2020 206c 696d 6974 733d 2822 7322       limits=("s"
-00025570: 2c20 302e 302c 204e 6f6e 6529 2c20 2023  , 0.0, None),  #
-00025580: 206c 696d 6974 730a 2020 2020 2020 2020   limits.        
-00025590: 2020 2020 7573 655f 4761 7573 7341 7070      use_GaussApp
-000255a0: 726f 783d 4661 6c73 652c 2020 2320 4761  rox=False,  # Ga
-000255b0: 7573 7369 616e 2061 7070 726f 7869 6d61  ussian approxima
-000255c0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-000255d0: 2066 6974 5f64 656e 7369 7479 3d54 7275   fit_density=Tru
-000255e0: 652c 2020 2320 6669 7420 6465 6e73 6974  e,  # fit densit
-000255f0: 790a 2020 2020 2020 2020 2020 2020 706c  y.            pl
-00025600: 6f74 3d54 7275 652c 2020 2320 706c 6f74  ot=True,  # plot
-00025610: 2064 6174 6120 616e 6420 6d6f 6465 6c0a   data and model.
-00025620: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
-00025630: 5f62 616e 643d 5472 7565 2c20 2023 2070  _band=True,  # p
-00025640: 6c6f 7420 6d6f 6465 6c20 636f 6e66 6964  lot model confid
-00025650: 656e 6365 2d62 616e 640a 2020 2020 2020  ence-band.      
-00025660: 2020 2020 2020 706c 6f74 5f63 6f72 3d54        plot_cor=T
-00025670: 7275 652c 2020 2320 706c 6f74 2070 726f  rue,  # plot pro
-00025680: 6669 6c65 7320 6c69 6b65 6c69 686f 6f64  files likelihood
-00025690: 2061 6e64 2063 6f6e 746f 7572 730a 2020   and contours.  
-000256a0: 2020 2020 2020 2020 2020 7368 6f77 706c            showpl
-000256b0: 6f74 733d 4661 6c73 652c 2020 2320 7368  ots=False,  # sh
-000256c0: 6f77 202f 2064 6f6e 2774 2073 686f 7720  ow / don't show 
-000256d0: 706c 6f74 730a 2020 2020 2020 2020 2020  plots.          
-000256e0: 2020 7175 6965 743d 4661 6c73 652c 2020    quiet=False,  
-000256f0: 2320 7375 7070 7265 7373 2069 6e66 6f72  # suppress infor
-00025700: 6d61 7469 7665 2070 7269 6e74 6f75 740a  mative printout.
-00025710: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-00025720: 5f6c 6162 656c 733d 5b22 7822 2c20 2279  _labels=["x", "y
-00025730: 2020 205c 2020 6628 782c 202a 7061 7229     \  f(x, *par)
-00025740: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-00025750: 6461 7461 5f6c 6567 656e 643d 2272 616e  data_legend="ran
-00025760: 646f 6d20 6461 7461 222c 0a20 2020 2020  dom data",.     
-00025770: 2020 2020 2020 206d 6f64 656c 5f6c 6567         model_leg
-00025780: 656e 643d 2273 6967 6e61 6c20 2b20 6261  end="signal + ba
-00025790: 636b 6772 6f75 6e64 206d 6f64 656c 222c  ckground model",
-000257a0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000257b0: 2020 2020 706c 742e 7375 7074 6974 6c65      plt.suptitle
-000257c0: 280a 2020 2020 2020 2020 2020 2020 226d  (.            "m
-000257d0: 6e46 6974 2065 7861 6d70 6c65 3a20 6669  nFit example: fi
-000257e0: 7420 746f 2068 6973 746f 6772 616d 2064  t to histogram d
-000257f0: 6174 6122 2c20 7369 7a65 3d22 7878 2d6c  ata", size="xx-l
-00025800: 6172 6765 222c 2063 6f6c 6f72 3d22 6461  arge", color="da
-00025810: 726b 626c 7565 220a 2020 2020 2020 2020  rkblue".        
-00025820: 290a 0a20 2020 2020 2020 2023 2050 7269  )..        # Pri
-00025830: 6e74 2072 6573 756c 7473 0a20 2020 2020  nt results.     
-00025840: 2020 2070 7269 6e74 2822 5c6e 2a3d 3d2a     print("\n*==*
-00025850: 2068 6973 746f 6772 616d 2066 6974 2052   histogram fit R
-00025860: 6573 756c 743a 2229 0a20 2020 2020 2020  esult:").       
-00025870: 2070 7661 6c73 2c20 7065 7272 732c 2063   pvals, perrs, c
-00025880: 6f72 2c20 676f 662c 2070 6e61 6d73 203d  or, gof, pnams =
-00025890: 2072 6573 756c 7444 6963 742e 7661 6c75   resultDict.valu
-000258a0: 6573 2829 0a20 2020 2020 2020 2070 7269  es().        pri
-000258b0: 6e74 2822 2070 6172 616d 6574 6572 206e  nt(" parameter n
-000258c0: 616d 6573 3a20 2020 2020 2020 222c 2070  ames:       ", p
-000258d0: 6e61 6d73 290a 2020 2020 2020 2020 7072  nams).        pr
-000258e0: 696e 7428 2220 676f 6f64 6e65 7373 2d6f  int(" goodness-o
-000258f0: 662d 6669 743a 207b 3a2e 3367 7d22 2e66  f-fit: {:.3g}".f
-00025900: 6f72 6d61 7428 676f 6629 290a 2020 2020  ormat(gof)).    
-00025910: 2020 2020 7072 696e 7428 2220 7061 7261      print(" para
-00025920: 6d65 7465 7220 7661 6c75 6573 3a20 2020  meter values:   
-00025930: 2020 2022 2c20 7076 616c 7329 0a20 2020     ", pvals).   
-00025940: 2020 2020 2070 7269 6e74 2822 206e 6567       print(" neg
-00025950: 2e20 7061 7261 6d65 7465 7220 6572 726f  . parameter erro
-00025960: 7273 3a20 222c 2070 6572 7273 5b3a 2c20  rs: ", perrs[:, 
-00025970: 305d 290a 2020 2020 2020 2020 7072 696e  0]).        prin
-00025980: 7428 2220 706f 732e 2070 6172 616d 6574  t(" pos. paramet
-00025990: 6572 2065 7272 6f72 733a 2022 2c20 7065  er errors: ", pe
-000259a0: 7272 735b 3a2c 2031 5d29 0a20 2020 2020  rrs[:, 1]).     
-000259b0: 2020 2070 7269 6e74 2822 2063 6f72 7265     print(" corre
-000259c0: 6c61 7469 6f6e 7320 3a20 5c6e 222c 2063  lations : \n", c
-000259d0: 6f72 290a 0a20 2020 2064 6566 2065 7861  or)..    def exa
-000259e0: 6d70 6c65 5f75 7365 7246 6974 2829 3a0a  mple_userFit():.
-000259f0: 2020 2020 2020 2020 2222 222a 2a75 6e62          """**unb
-00025a00: 696e 6e65 6420 4d4c 2066 6974 2a2a 2077  inned ML fit** w
-00025a10: 6974 6820 7573 6572 2d64 6566 696e 6564  ith user-defined
-00025a20: 2063 6f73 7420 6675 6e63 7469 6f6e 0a0a   cost function..
-00025a30: 2020 2020 2020 2020 5468 6973 2063 6f64          This cod
-00025a40: 6520 696c 6c75 7374 7261 7465 7320 7573  e illustrates us
-00025a50: 6167 6520 6f66 2074 6865 2077 7261 7070  age of the wrapp
-00025a60: 6572 2066 756e 6374 696f 6e20 6d46 6974  er function mFit
-00025a70: 2829 0a20 2020 2020 2020 2066 6f72 2020  ().        for  
-00025a80: 636c 6173 7320 2a2a 6d6e 4669 742a 2a20  class **mnFit** 
-00025a90: 7573 6572 2d64 6566 696e 6564 2063 6f73  user-defined cos
-00025aa0: 7420 6675 6e63 7469 6f6e 0a20 2020 2020  t function.     
-00025ab0: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00025ac0: 2320 6765 6e65 7261 7465 2047 6175 7373  # generate Gauss
-00025ad0: 6961 6e2d 6469 7374 7269 6275 7465 6420  ian-distributed 
-00025ae0: 6461 7461 0a20 2020 2020 2020 206d 7530  data.        mu0
-00025af0: 203d 2032 2e30 0a20 2020 2020 2020 2073   = 2.0.        s
-00025b00: 6967 3020 3d20 302e 350a 2020 2020 2020  ig0 = 0.5.      
-00025b10: 2020 6e70 2e72 616e 646f 6d2e 7365 6564    np.random.seed
-00025b20: 2833 3134 3135 3929 2020 2320 696e 6974  (314159)  # init
-00025b30: 6961 6c69 7a65 2072 616e 646f 6d20 6765  ialize random ge
-00025b40: 6e65 7261 746f 720a 2020 2020 2020 2020  nerator.        
-00025b50: 6461 7461 203d 206d 7530 202b 2073 6967  data = mu0 + sig
-00025b60: 3020 2a20 6e70 2e72 616e 646f 6d2e 7261  0 * np.random.ra
-00025b70: 6e64 6e28 3130 3029 0a0a 2020 2020 2020  ndn(100)..      
-00025b80: 2020 2320 6465 6669 6e65 2063 6f73 7420    # define cost 
-00025b90: 6675 6e63 7469 6f6e 3a20 3220 2a20 6e65  function: 2 * ne
-00025ba0: 6761 7469 7665 206c 6f67 206c 696b 656c  gative log likel
-00025bb0: 6968 6f6f 6420 6f66 2047 6175 c39f 3b0a  ihood of Gau..;.
-00025bc0: 2020 2020 2020 2020 6465 6620 6d79 436f          def myCo
-00025bd0: 7374 286d 753d 312e 302c 2073 6967 6d61  st(mu=1.0, sigma
-00025be0: 3d31 2e30 293a 0a20 2020 2020 2020 2020  =1.0):.         
-00025bf0: 2020 2023 2073 696d 706c 6520 2d32 2a6c     # simple -2*l
-00025c00: 6f67 2d6c 696b 656c 6968 6f6f 6420 6f66  og-likelihood of
-00025c10: 2061 2031 2d64 2047 6175 7373 2064 6973   a 1-d Gauss dis
-00025c20: 7472 6962 7574 696f 6e0a 2020 2020 2020  tribution.      
-00025c30: 2020 2020 2020 7220 3d20 2864 6174 6120        r = (data 
-00025c40: 2d20 6d75 2920 2f20 7369 676d 610a 2020  - mu) / sigma.  
-00025c50: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00025c60: 206e 702e 7375 6d28 7220 2a20 7220 2b20   np.sum(r * r + 
-00025c70: 322e 3020 2a20 6e70 2e6c 6f67 2873 6967  2.0 * np.log(sig
-00025c80: 6d61 2929 0a0a 2020 2020 2020 2020 7265  ma))..        re
-00025c90: 7375 6c74 4469 6374 203d 206d 4669 7428  sultDict = mFit(
-00025ca0: 0a20 2020 2020 2020 2020 2020 206d 7943  .            myC
-00025cb0: 6f73 742c 0a20 2020 2020 2020 2020 2020  ost,.           
-00025cc0: 2070 303d 4e6f 6e65 2c20 2023 2069 6e69   p0=None,  # ini
-00025cd0: 7469 616c 2067 7565 7373 2066 6f72 2070  tial guess for p
-00025ce0: 6172 616d 6574 6572 2076 616c 7565 730a  arameter values.
-00025cf0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00025d00: 7472 6169 6e74 733d 5b5b 226d 7522 2c20  traints=[["mu", 
-00025d10: 322e 302c 2030 2e30 315d 5d2c 2020 2320  2.0, 0.01]],  # 
-00025d20: 4761 7573 7369 616e 2070 6172 616d 6574  Gaussian paramet
-00025d30: 6572 2063 6f6e 7374 7261 696e 7473 0a20  er constraints. 
-00025d40: 2020 2020 2020 2020 2020 2023 2020 6c69             #  li
-00025d50: 6d69 7473 3d28 2773 6967 6d61 272c 204e  mits=('sigma', N
-00025d60: 6f6e 652c 204e 6f6e 6529 2c20 2023 6c69  one, None),  #li
-00025d70: 6d69 7473 0a20 2020 2020 2020 2020 2020  mits.           
-00025d80: 2023 2020 6669 7850 6172 7320 3d20 5b27   #  fixPars = ['
-00025d90: 6d75 275d 2c20 2020 2020 2020 2023 2066  mu'],        # f
-00025da0: 6978 2070 6172 616d 6574 6572 2873 290a  ix parameter(s).
-00025db0: 2020 2020 2020 2020 2020 2020 6e65 6732              neg2
-00025dc0: 6c6f 674c 3d54 7275 652c 2020 2320 636f  logL=True,  # co
-00025dd0: 7374 2069 7320 2d32 202a 206c 6e28 4c29  st is -2 * ln(L)
-00025de0: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
-00025df0: 745f 636f 723d 5472 7565 2c20 2023 2070  t_cor=True,  # p
-00025e00: 6c6f 7420 7072 6f66 696c 6573 206c 696b  lot profiles lik
-00025e10: 656c 6968 6f6f 6420 616e 6420 636f 6e74  elihood and cont
-00025e20: 6f75 7273 0a20 2020 2020 2020 2020 2020  ours.           
-00025e30: 2073 686f 7770 6c6f 7473 3d46 616c 7365   showplots=False
-00025e40: 2c20 2023 2073 686f 7720 2f20 646f 6e27  ,  # show / don'
-00025e50: 7420 7368 6f77 2070 6c6f 7473 0a20 2020  t show plots.   
-00025e60: 2020 2020 2020 2020 2071 7569 6574 3d46           quiet=F
-00025e70: 616c 7365 2c20 2023 2073 7570 7072 6573  alse,  # suppres
-00025e80: 7320 696e 666f 726d 6174 6976 6520 7072  s informative pr
-00025e90: 696e 746f 7574 0a20 2020 2020 2020 2029  intout.        )
-00025ea0: 0a0a 2020 2020 2020 2020 706c 742e 7375  ..        plt.su
-00025eb0: 7074 6974 6c65 280a 2020 2020 2020 2020  ptitle(.        
-00025ec0: 2020 2020 224d 6178 696d 756d 2d6c 696b      "Maximum-lik
-00025ed0: 656c 6968 6f6f 6420 6669 743a 2070 726f  elihood fit: pro
-00025ee0: 6669 6c65 7320 616e 6420 636f 6e74 6f75  files and contou
-00025ef0: 7273 222c 0a20 2020 2020 2020 2020 2020  rs",.           
-00025f00: 2073 697a 653d 2278 782d 6c61 7267 6522   size="xx-large"
-00025f10: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
-00025f20: 6c6f 723d 2264 6172 6b62 6c75 6522 2c0a  lor="darkblue",.
-00025f30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00025f40: 2020 2320 5072 696e 7420 7265 7375 6c74    # Print result
-00025f50: 730a 2020 2020 2020 2020 7076 616c 732c  s.        pvals,
-00025f60: 2070 6572 7273 2c20 636f 722c 2067 6f66   perrs, cor, gof
-00025f70: 2c20 706e 616d 7320 3d20 7265 7375 6c74  , pnams = result
-00025f80: 4469 6374 2e76 616c 7565 7328 290a 2020  Dict.values().  
-00025f90: 2020 2020 2020 7072 696e 7428 225c 6e2a        print("\n*
-00025fa0: 3d3d 2a20 7573 6572 2d64 6566 696e 6564  ==* user-defined
-00025fb0: 2063 6f73 743a 2046 6974 2052 6573 756c   cost: Fit Resul
-00025fc0: 743a 2229 0a20 2020 2020 2020 2070 7269  t:").        pri
-00025fd0: 6e74 2822 2070 6172 616d 6574 6572 206e  nt(" parameter n
-00025fe0: 616d 6573 3a20 2020 2020 2020 222c 2070  ames:       ", p
-00025ff0: 6e61 6d73 290a 2020 2020 2020 2020 7072  nams).        pr
-00026000: 696e 7428 2220 7061 7261 6d65 7465 7220  int(" parameter 
-00026010: 7661 6c75 6573 3a20 2020 2020 2022 2c20  values:      ", 
-00026020: 7076 616c 7329 0a20 2020 2020 2020 2070  pvals).        p
-00026030: 7269 6e74 2822 206e 6567 2e20 7061 7261  rint(" neg. para
-00026040: 6d65 7465 7220 6572 726f 7273 3a20 222c  meter errors: ",
-00026050: 2070 6572 7273 5b3a 2c20 305d 290a 2020   perrs[:, 0]).  
-00026060: 2020 2020 2020 7072 696e 7428 2220 706f        print(" po
-00026070: 732e 2070 6172 616d 6574 6572 2065 7272  s. parameter err
-00026080: 6f72 733a 2022 2c20 7065 7272 735b 3a2c  ors: ", perrs[:,
-00026090: 2031 5d29 0a20 2020 2020 2020 2070 7269   1]).        pri
-000260a0: 6e74 2822 2063 6f72 7265 6c61 7469 6f6e  nt(" correlation
-000260b0: 7320 3a20 5c6e 222c 2063 6f72 290a 0a20  s : \n", cor).. 
-000260c0: 2020 2064 6566 2065 7861 6d70 6c65 5f75     def example_u
-000260d0: 6e62 696e 6e65 644d 4c46 6974 2829 3a0a  nbinnedMLFit():.
-000260e0: 2020 2020 2020 2020 2222 222a 2a75 6e62          """**unb
-000260f0: 696e 6e65 6420 4d4c 2066 6974 2a2a 206f  inned ML fit** o
-00026100: 6620 7064 6620 746f 2075 6e62 696e 6e65  f pdf to unbinne
-00026110: 6420 6461 7461 0a0a 2020 2020 2020 2020  d data..        
-00026120: 7265 616c 2064 6174 6120 6672 6f6d 206d  real data from m
-00026130: 6561 7375 7265 6d65 6e74 2077 6974 6820  easurement with 
-00026140: 6120 5761 7465 7220 4368 6572 656e 6b6f  a Water Cherenko
-00026150: 7620 6465 7465 6374 6f72 2028 224b 616d  v detector ("Kam
-00026160: 696f 6b61 6e6e 6522 290a 0a20 2020 2020  iokanne")..     
-00026170: 2020 206e 756d 6265 7273 2072 6570 7265     numbers repre
-00026180: 7365 6e74 2074 696d 6520 6469 6666 6572  sent time differ
-00026190: 656e 6365 7320 2869 6e20 c2b5 7329 2062  ences (in ..s) b
-000261a0: 6574 7765 656e 2074 6865 2070 6173 7361  etween the passa
-000261b0: 6765 206f 6620 6120 6d75 6f6e 0a20 2020  ge of a muon.   
-000261c0: 2020 2020 2061 6e64 2074 6865 2072 6567       and the reg
-000261d0: 6973 7472 6174 696f 6e20 6f66 2061 2073  istration of a s
-000261e0: 6563 6f6e 6420 7075 6c73 652c 206f 6674  econd pulse, oft
-000261f0: 656e 2063 6175 7365 6420 6279 2061 6e20  en caused by an 
-00026200: 656c 6563 7472 6f6e 2066 726f 6d0a 2020  electron from.  
-00026210: 2020 2020 2020 7468 6520 6465 6361 7920        the decay 
-00026220: 6f66 2074 6865 2073 746f 7070 6564 206d  of the stopped m
-00026230: 756f 6e2e 2041 7320 7375 6368 2065 7665  uon. As such eve
-00026240: 6e74 7320 6172 6520 7261 7265 2c20 6869  nts are rare, hi
-00026250: 7374 6f67 7261 6d6d 696e 6720 7468 650a  stogramming the.
-00026260: 2020 2020 2020 2020 6461 7461 2070 7269          data pri
-00026270: 6f72 2074 6f20 6669 7474 696e 6720 776f  or to fitting wo
-00026280: 756c 6420 696e 7472 6f64 7563 6520 7368  uld introduce sh
-00026290: 6966 7473 2061 6e64 2062 6961 7365 732c  ifts and biases,
-000262a0: 2061 6e64 2074 6865 7265 666f 7265 2074   and therefore t
-000262b0: 6865 0a20 2020 2020 2020 2075 6e62 696e  he.        unbin
-000262c0: 6e65 6420 6669 7420 6973 2074 6865 206f  ned fit is the o
-000262d0: 7074 696d 616c 206d 6574 686f 6420 666f  ptimal method fo
-000262e0: 7220 7468 6973 2061 6e64 2073 696d 756c  r this and simul
-000262f0: 6172 2075 7365 2063 6173 6573 2e0a 2020  ar use cases..  
-00026300: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00026310: 2020 6454 203d 205b 0a20 2020 2020 2020    dT = [.       
-00026320: 2020 2020 2037 2e34 322c 0a20 2020 2020       7.42,.     
-00026330: 2020 2020 2020 2033 2e37 3733 2c0a 2020         3.773,.  
-00026340: 2020 2020 2020 2020 2020 352e 3936 382c            5.968,
-00026350: 0a20 2020 2020 2020 2020 2020 2034 2e39  .            4.9
-00026360: 3234 2c0a 2020 2020 2020 2020 2020 2020  24,.            
-00026370: 312e 3436 382c 0a20 2020 2020 2020 2020  1.468,.         
-00026380: 2020 2034 2e36 3634 2c0a 2020 2020 2020     4.664,.      
-00026390: 2020 2020 2020 312e 3734 352c 0a20 2020        1.745,.   
-000263a0: 2020 2020 2020 2020 2032 2e31 3434 2c0a           2.144,.
-000263b0: 2020 2020 2020 2020 2020 2020 332e 3833              3.83
-000263c0: 362c 0a20 2020 2020 2020 2020 2020 2033  6,.            3
-000263d0: 2e31 3332 2c0a 2020 2020 2020 2020 2020  .132,.          
-000263e0: 2020 312e 3536 382c 0a20 2020 2020 2020    1.568,.       
-000263f0: 2020 2020 2032 2e33 3532 2c0a 2020 2020       2.352,.    
-00026400: 2020 2020 2020 2020 322e 3133 322c 0a20          2.132,. 
-00026410: 2020 2020 2020 2020 2020 2039 2e33 3831             9.381
-00026420: 2c0a 2020 2020 2020 2020 2020 2020 312e  ,.            1.
-00026430: 3438 342c 0a20 2020 2020 2020 2020 2020  484,.           
-00026440: 2031 2e31 3831 2c0a 2020 2020 2020 2020   1.181,.        
-00026450: 2020 2020 352e 3030 342c 0a20 2020 2020      5.004,.     
-00026460: 2020 2020 2020 2033 2e30 362c 0a20 2020         3.06,.   
-00026470: 2020 2020 2020 2020 2034 2e35 3832 2c0a           4.582,.
-00026480: 2020 2020 2020 2020 2020 2020 322e 3037              2.07
-00026490: 362c 0a20 2020 2020 2020 2020 2020 2031  6,.            1
-000264a0: 2e38 382c 0a20 2020 2020 2020 2020 2020  .88,.           
-000264b0: 2031 2e33 3337 2c0a 2020 2020 2020 2020   1.337,.        
-000264c0: 2020 2020 332e 3039 322c 0a20 2020 2020      3.092,.     
-000264d0: 2020 2020 2020 2032 2e32 3635 2c0a 2020         2.265,.  
-000264e0: 2020 2020 2020 2020 2020 312e 3230 382c            1.208,
-000264f0: 0a20 2020 2020 2020 2020 2020 2032 2e37  .            2.7
-00026500: 3533 2c0a 2020 2020 2020 2020 2020 2020  53,.            
-00026510: 342e 3435 372c 0a20 2020 2020 2020 2020  4.457,.         
-00026520: 2020 2033 2e34 3939 2c0a 2020 2020 2020     3.499,.      
-00026530: 2020 2020 2020 382e 3139 322c 0a20 2020        8.192,.   
-00026540: 2020 2020 2020 2020 2035 2e31 3031 2c0a           5.101,.
-00026550: 2020 2020 2020 2020 2020 2020 312e 3537              1.57
-00026560: 322c 0a20 2020 2020 2020 2020 2020 2035  2,.            5
-00026570: 2e31 3532 2c0a 2020 2020 2020 2020 2020  .152,.          
-00026580: 2020 342e 3138 312c 0a20 2020 2020 2020    4.181,.       
-00026590: 2020 2020 2033 2e35 322c 0a20 2020 2020       3.52,.     
-000265a0: 2020 2020 2020 2031 2e33 3434 2c0a 2020         1.344,.  
-000265b0: 2020 2020 2020 2020 2020 3130 2e32 392c            10.29,
-000265c0: 0a20 2020 2020 2020 2020 2020 2031 2e31  .            1.1
-000265d0: 3532 2c0a 2020 2020 2020 2020 2020 2020  52,.            
-000265e0: 322e 3334 382c 0a20 2020 2020 2020 2020  2.348,.         
-000265f0: 2020 2032 2e32 3238 2c0a 2020 2020 2020     2.228,.      
-00026600: 2020 2020 2020 322e 3137 322c 0a20 2020        2.172,.   
-00026610: 2020 2020 2020 2020 2037 2e34 3438 2c0a           7.448,.
-00026620: 2020 2020 2020 2020 2020 2020 312e 3130              1.10
-00026630: 382c 0a20 2020 2020 2020 2020 2020 2034  8,.            4
-00026640: 2e33 3434 2c0a 2020 2020 2020 2020 2020  .344,.          
-00026650: 2020 322e 3034 322c 0a20 2020 2020 2020    2.042,.       
-00026660: 2020 2020 2035 2e30 3838 2c0a 2020 2020       5.088,.    
-00026670: 2020 2020 2020 2020 312e 3032 2c0a 2020          1.02,.  
-00026680: 2020 2020 2020 2020 2020 312e 3035 312c            1.051,
-00026690: 0a20 2020 2020 2020 2020 2020 2031 2e39  .            1.9
-000266a0: 3837 2c0a 2020 2020 2020 2020 2020 2020  87,.            
-000266b0: 312e 3933 352c 0a20 2020 2020 2020 2020  1.935,.         
-000266c0: 2020 2033 2e37 3733 2c0a 2020 2020 2020     3.773,.      
-000266d0: 2020 2020 2020 342e 3039 322c 0a20 2020        4.092,.   
-000266e0: 2020 2020 2020 2020 2031 2e36 3238 2c0a           1.628,.
-000266f0: 2020 2020 2020 2020 2020 2020 312e 3638              1.68
-00026700: 382c 0a20 2020 2020 2020 2020 2020 2034  8,.            4
-00026710: 2e35 3032 2c0a 2020 2020 2020 2020 2020  .502,.          
-00026720: 2020 342e 3638 372c 0a20 2020 2020 2020    4.687,.       
-00026730: 2020 2020 2036 2e37 3535 2c0a 2020 2020       6.755,.    
-00026740: 2020 2020 2020 2020 322e 3536 2c0a 2020          2.56,.  
-00026750: 2020 2020 2020 2020 2020 312e 3230 382c            1.208,
-00026760: 0a20 2020 2020 2020 2020 2020 2032 2e36  .            2.6
-00026770: 3439 2c0a 2020 2020 2020 2020 2020 2020  49,.            
-00026780: 312e 3031 322c 0a20 2020 2020 2020 2020  1.012,.         
-00026790: 2020 2031 2e37 332c 0a20 2020 2020 2020     1.73,.       
-000267a0: 2020 2020 2032 2e31 3634 2c0a 2020 2020       2.164,.    
-000267b0: 2020 2020 2020 2020 312e 3732 382c 0a20          1.728,. 
-000267c0: 2020 2020 2020 2020 2020 2034 2e36 3436             4.646
-000267d0: 2c0a 2020 2020 2020 2020 2020 2020 322e  ,.            2.
-000267e0: 3931 362c 0a20 2020 2020 2020 2020 2020  916,.           
-000267f0: 2031 2e31 3031 2c0a 2020 2020 2020 2020   1.101,.        
-00026800: 2020 2020 322e 3534 2c0a 2020 2020 2020      2.54,.      
-00026810: 2020 2020 2020 312e 3032 2c0a 2020 2020        1.02,.    
-00026820: 2020 2020 2020 2020 312e 3137 362c 0a20          1.176,. 
-00026830: 2020 2020 2020 2020 2020 2034 2e37 3136             4.716
-00026840: 2c0a 2020 2020 2020 2020 2020 2020 392e  ,.            9.
-00026850: 3637 312c 0a20 2020 2020 2020 2020 2020  671,.           
-00026860: 2031 2e36 3932 2c0a 2020 2020 2020 2020   1.692,.        
-00026870: 2020 2020 392e 3239 322c 0a20 2020 2020      9.292,.     
-00026880: 2020 2020 2020 2031 302e 3732 2c0a 2020         10.72,.  
-00026890: 2020 2020 2020 2020 2020 322e 3136 342c            2.164,
-000268a0: 0a20 2020 2020 2020 2020 2020 2032 2e30  .            2.0
-000268b0: 3834 2c0a 2020 2020 2020 2020 2020 2020  84,.            
-000268c0: 322e 3631 362c 0a20 2020 2020 2020 2020  2.616,.         
-000268d0: 2020 2031 2e35 3834 2c0a 2020 2020 2020     1.584,.      
-000268e0: 2020 2020 2020 352e 3233 362c 0a20 2020        5.236,.   
-000268f0: 2020 2020 2020 2020 2033 2e36 3633 2c0a           3.663,.
-00026900: 2020 2020 2020 2020 2020 2020 332e 3632              3.62
-00026910: 342c 0a20 2020 2020 2020 2020 2020 2031  4,.            1
-00026920: 2e30 3531 2c0a 2020 2020 2020 2020 2020  .051,.          
-00026930: 2020 312e 3534 342c 0a20 2020 2020 2020    1.544,.       
-00026940: 2020 2020 2031 2e34 3936 2c0a 2020 2020       1.496,.    
-00026950: 2020 2020 2020 2020 312e 3838 332c 0a20          1.883,. 
-00026960: 2020 2020 2020 2020 2020 2031 2e39 322c             1.92,
-00026970: 0a20 2020 2020 2020 2020 2020 2035 2e39  .            5.9
-00026980: 3638 2c0a 2020 2020 2020 2020 2020 2020  68,.            
-00026990: 352e 3839 2c0a 2020 2020 2020 2020 2020  5.89,.          
-000269a0: 2020 322e 3839 362c 0a20 2020 2020 2020    2.896,.       
-000269b0: 2020 2020 2032 2e37 362c 0a20 2020 2020       2.76,.     
-000269c0: 2020 2020 2020 2031 2e34 3735 2c0a 2020         1.475,.  
-000269d0: 2020 2020 2020 2020 2020 322e 3634 342c            2.644,
-000269e0: 0a20 2020 2020 2020 2020 2020 2033 2e36  .            3.6
-000269f0: 2c0a 2020 2020 2020 2020 2020 2020 352e  ,.            5.
-00026a00: 3332 342c 0a20 2020 2020 2020 2020 2020  324,.           
-00026a10: 2038 2e33 3631 2c0a 2020 2020 2020 2020   8.361,.        
-00026a20: 2020 2020 332e 3035 322c 0a20 2020 2020      3.052,.     
-00026a30: 2020 2020 2020 2037 2e37 3033 2c0a 2020         7.703,.  
-00026a40: 2020 2020 2020 2020 2020 332e 3833 2c0a            3.83,.
-00026a50: 2020 2020 2020 2020 2020 2020 312e 3434              1.44
-00026a60: 342c 0a20 2020 2020 2020 2020 2020 2031  4,.            1
-00026a70: 2e33 3433 2c0a 2020 2020 2020 2020 2020  .343,.          
-00026a80: 2020 342e 3733 362c 0a20 2020 2020 2020    4.736,.       
-00026a90: 2020 2020 2038 2e37 2c0a 2020 2020 2020       8.7,.      
-00026aa0: 2020 2020 2020 362e 3139 322c 0a20 2020        6.192,.   
-00026ab0: 2020 2020 2020 2020 2035 2e37 3936 2c0a           5.796,.
-00026ac0: 2020 2020 2020 2020 2020 2020 312e 342c              1.4,
-00026ad0: 0a20 2020 2020 2020 2020 2020 2033 2e33  .            3.3
-00026ae0: 3932 2c0a 2020 2020 2020 2020 2020 2020  92,.            
-00026af0: 372e 3830 382c 0a20 2020 2020 2020 2020  7.808,.         
-00026b00: 2020 2036 2e33 3434 2c0a 2020 2020 2020     6.344,.      
-00026b10: 2020 2020 2020 312e 3838 342c 0a20 2020        1.884,.   
-00026b20: 2020 2020 2020 2020 2032 2e33 3332 2c0a           2.332,.
-00026b30: 2020 2020 2020 2020 2020 2020 312e 3736              1.76
-00026b40: 2c0a 2020 2020 2020 2020 2020 2020 342e  ,.            4.
-00026b50: 3334 342c 0a20 2020 2020 2020 2020 2020  344,.           
-00026b60: 2032 2e39 3838 2c0a 2020 2020 2020 2020   2.988,.        
-00026b70: 2020 2020 372e 3434 2c0a 2020 2020 2020      7.44,.      
-00026b80: 2020 2020 2020 352e 3830 342c 0a20 2020        5.804,.   
-00026b90: 2020 2020 2020 2020 2039 2e35 2c0a 2020           9.5,.  
-00026ba0: 2020 2020 2020 2020 2020 392e 3930 342c            9.904,
-00026bb0: 0a20 2020 2020 2020 2020 2020 2033 2e31  .            3.1
-00026bc0: 3936 2c0a 2020 2020 2020 2020 2020 2020  96,.            
-00026bd0: 332e 3031 322c 0a20 2020 2020 2020 2020  3.012,.         
-00026be0: 2020 2036 2e30 3536 2c0a 2020 2020 2020     6.056,.      
-00026bf0: 2020 2020 2020 362e 3332 382c 0a20 2020        6.328,.   
-00026c00: 2020 2020 2020 2020 2039 2e30 3634 2c0a           9.064,.
-00026c10: 2020 2020 2020 2020 2020 2020 332e 3036              3.06
-00026c20: 382c 0a20 2020 2020 2020 2020 2020 2039  8,.            9
-00026c30: 2e33 3532 2c0a 2020 2020 2020 2020 2020  .352,.          
-00026c40: 2020 312e 3933 362c 0a20 2020 2020 2020    1.936,.       
-00026c50: 2020 2020 2031 2e30 382c 0a20 2020 2020       1.08,.     
-00026c60: 2020 2020 2020 2031 2e39 3834 2c0a 2020         1.984,.  
-00026c70: 2020 2020 2020 2020 2020 312e 3739 322c            1.792,
-00026c80: 0a20 2020 2020 2020 2020 2020 2039 2e33  .            9.3
-00026c90: 3834 2c0a 2020 2020 2020 2020 2020 2020  84,.            
-00026ca0: 3130 2e31 352c 0a20 2020 2020 2020 2020  10.15,.         
-00026cb0: 2020 2034 2e37 3536 2c0a 2020 2020 2020     4.756,.      
-00026cc0: 2020 2020 2020 312e 3532 2c0a 2020 2020        1.52,.    
-00026cd0: 2020 2020 2020 2020 332e 3931 322c 0a20          3.912,. 
-00026ce0: 2020 2020 2020 2020 2020 2031 2e37 3132             1.712
-00026cf0: 2c0a 2020 2020 2020 2020 2020 2020 3130  ,.            10
-00026d00: 2e35 372c 0a20 2020 2020 2020 2020 2020  .57,.           
-00026d10: 2035 2e33 3034 2c0a 2020 2020 2020 2020   5.304,.        
-00026d20: 2020 2020 322e 3936 382c 0a20 2020 2020      2.968,.     
-00026d30: 2020 2020 2020 2039 2e36 3332 2c0a 2020         9.632,.  
-00026d40: 2020 2020 2020 2020 2020 372e 3131 362c            7.116,
-00026d50: 0a20 2020 2020 2020 2020 2020 2031 2e32  .            1.2
-00026d60: 3132 2c0a 2020 2020 2020 2020 2020 2020  12,.            
-00026d70: 382e 3533 322c 0a20 2020 2020 2020 2020  8.532,.         
-00026d80: 2020 2033 2e30 3030 2c0a 2020 2020 2020     3.000,.      
-00026d90: 2020 2020 2020 342e 3739 322c 0a20 2020        4.792,.   
-00026da0: 2020 2020 2020 2020 2032 2e35 3132 2c0a           2.512,.
-00026db0: 2020 2020 2020 2020 2020 2020 312e 3335              1.35
-00026dc0: 322c 0a20 2020 2020 2020 2020 2020 2032  2,.            2
-00026dd0: 2e31 3638 2c0a 2020 2020 2020 2020 2020  .168,.          
-00026de0: 2020 342e 3334 342c 0a20 2020 2020 2020    4.344,.       
-00026df0: 2020 2020 2031 2e33 3136 2c0a 2020 2020       1.316,.    
-00026e00: 2020 2020 2020 2020 312e 3436 382c 0a20          1.468,. 
-00026e10: 2020 2020 2020 2020 2020 2031 2e31 3532             1.152
-00026e20: 2c0a 2020 2020 2020 2020 2020 2020 362e  ,.            6.
-00026e30: 3032 342c 0a20 2020 2020 2020 2020 2020  024,.           
-00026e40: 2033 2e32 3732 2c0a 2020 2020 2020 2020   3.272,.        
-00026e50: 2020 2020 342e 3936 2c0a 2020 2020 2020      4.96,.      
-00026e60: 2020 2020 2020 3130 2e31 362c 0a20 2020        10.16,.   
-00026e70: 2020 2020 2020 2020 2032 2e31 342c 0a20           2.14,. 
-00026e80: 2020 2020 2020 2020 2020 2032 2e38 3536             2.856
-00026e90: 2c0a 2020 2020 2020 2020 2020 2020 3130  ,.            10
-00026ea0: 2e30 312c 0a20 2020 2020 2020 2020 2020  .01,.           
-00026eb0: 2031 2e32 3332 2c0a 2020 2020 2020 2020   1.232,.        
-00026ec0: 2020 2020 322e 3636 382c 0a20 2020 2020      2.668,.     
-00026ed0: 2020 2020 2020 2039 2e31 3736 2c0a 2020         9.176,.  
-00026ee0: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
-00026ef0: 2064 6566 2065 7870 6f6e 656e 7469 616c   def exponential
-00026f00: 4465 6361 7950 4446 2874 2c20 7461 753d  DecayPDF(t, tau=
-00026f10: 322e 302c 2066 6267 3d30 2e32 2c20 613d  2.0, fbg=0.2, a=
-00026f20: 312e 302c 2062 3d31 312e 3529 3a0a 2020  1.0, b=11.5):.  
-00026f30: 2020 2020 2020 2020 2020 2222 2250 726f            """Pro
-00026f40: 6261 6269 6c69 7479 2064 656e 7369 7479  bability density
-00026f50: 2066 756e 6374 696f 6e0a 0a20 2020 2020   function..     
-00026f60: 2020 2020 2020 2066 6f72 2061 6e20 6578         for an ex
-00026f70: 706f 6e65 6e74 6961 6c20 6465 6361 7920  ponential decay 
-00026f80: 7769 7468 2066 6c61 7420 6261 636b 6772  with flat backgr
-00026f90: 6f75 6e64 2e20 5468 6520 7064 6620 6973  ound. The pdf is
-00026fa0: 206e 6f72 6d65 6420 666f 720a 2020 2020   normed for.    
-00026fb0: 2020 2020 2020 2020 7468 6520 696e 7465          the inte
-00026fc0: 7276 616c 205b 613d 31c2 b573 2c20 2062  rval [a=1..s,  b
-00026fd0: 3d31 312e 35c2 b573 293b 2074 6865 7365  =11.5..s); these
-00026fe0: 2070 6172 616d 6574 6572 7320 6120 616e   parameters a an
-00026ff0: 6420 6220 6d75 7374 2062 650a 2020 2020  d b must be.    
-00027000: 2020 2020 2020 2020 6669 7865 6420 696e          fixed in
-00027010: 2074 6865 2066 6974 210a 0a20 2020 2020   the fit!..     
-00027020: 2020 2020 2020 203a 7061 7261 6d20 743a         :param t:
-00027030: 2064 6563 6179 2074 696d 650a 2020 2020   decay time.    
-00027040: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00027050: 6267 3a20 6261 636b 6772 6f75 6e64 0a20  bg: background. 
-00027060: 2020 2020 2020 2020 2020 203a 7061 7261             :para
-00027070: 6d20 7461 753a 2065 7870 6563 7465 6420  m tau: expected 
-00027080: 6d65 616e 206f 6620 7468 6520 6465 6361  mean of the deca
-00027090: 7920 7469 6d65 0a20 2020 2020 2020 2020  y time.         
-000270a0: 2020 203a 7061 7261 6d20 613a 2074 6865     :param a: the
-000270b0: 206d 696e 696d 756d 2064 6563 6179 2074   minimum decay t
-000270c0: 696d 6520 7768 6963 6820 6361 6e20 6265  ime which can be
-000270d0: 206d 6561 7375 7265 640a 2020 2020 2020   measured.      
-000270e0: 2020 2020 2020 3a70 6172 616d 2062 3a20        :param b: 
-000270f0: 7468 6520 6d61 7869 6d75 6d20 6465 6361  the maximum deca
-00027100: 7920 7469 6d65 2077 6869 6368 2063 616e  y time which can
-00027110: 2062 6520 6d65 6173 7572 6564 0a20 2020   be measured.   
-00027120: 2020 2020 2020 2020 203a 7265 7475 726e           :return
-00027130: 3a20 7072 6f62 6162 696c 6974 7920 666f  : probability fo
-00027140: 7220 6465 6361 7920 7469 6d65 2078 0a20  r decay time x. 
-00027150: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
-00027160: 2020 2020 2020 2020 2020 2070 6466 3120             pdf1 
-00027170: 3d20 6e70 2e65 7870 282d 7420 2f20 7461  = np.exp(-t / ta
-00027180: 7529 202f 2074 6175 202f 2028 6e70 2e65  u) / tau / (np.e
-00027190: 7870 282d 6120 2f20 7461 7529 202d 206e  xp(-a / tau) - n
-000271a0: 702e 6578 7028 2d62 202f 2074 6175 2929  p.exp(-b / tau))
-000271b0: 0a20 2020 2020 2020 2020 2020 2070 6466  .            pdf
-000271c0: 3220 3d20 312e 3020 2f20 2862 202d 2061  2 = 1.0 / (b - a
-000271d0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000271e0: 7475 726e 2028 3120 2d20 6662 6729 202a  turn (1 - fbg) *
-000271f0: 2070 6466 3120 2b20 6662 6720 2a20 7064   pdf1 + fbg * pd
-00027200: 6632 0a0a 2020 2020 2020 2020 7265 7375  f2..        resu
-00027210: 6c74 4469 6374 203d 206d 4669 7428 0a20  ltDict = mFit(. 
-00027220: 2020 2020 2020 2020 2020 2065 7870 6f6e             expon
-00027230: 656e 7469 616c 4465 6361 7950 4446 2c0a  entialDecayPDF,.
-00027240: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00027250: 3d64 542c 2020 2320 6461 7461 202d 2069  =dT,  # data - i
-00027260: 6620 6e6f 7420 4e6f 6e65 2c20 6120 6e6f  f not None, a no
-00027270: 726d 616c 6973 6564 2050 4446 2069 7320  rmalised PDF is 
-00027280: 6173 7375 6d65 6420 6173 206d 6f64 656c  assumed as model
-00027290: 0a20 2020 2020 2020 2020 2020 2070 303d  .            p0=
-000272a0: 4e6f 6e65 2c20 2023 2069 6e69 7469 616c  None,  # initial
-000272b0: 2067 7565 7373 2066 6f72 2070 6172 616d   guess for param
-000272c0: 6574 6572 2076 616c 7565 730a 2020 2020  eter values.    
-000272d0: 2020 2020 2020 2020 2320 2063 6f6e 7374          #  const
-000272e0: 7261 696e 7473 3d5b 5b27 7461 7527 2c20  raints=[['tau', 
-000272f0: 322e 322c 2030 2e30 315d 2c20 2320 4761  2.2, 0.01], # Ga
-00027300: 7573 7369 616e 2070 6172 616d 6574 6572  ussian parameter
-00027310: 2063 6f6e 7374 7261 696e 7473 0a20 2020   constraints.   
-00027320: 2020 2020 2020 2020 206c 696d 6974 733d           limits=
-00027330: 2822 6662 6722 2c20 302e 302c 2031 2e30  ("fbg", 0.0, 1.0
-00027340: 292c 2020 2320 7061 7261 6d65 7465 7220  ),  # parameter 
-00027350: 6c69 6d69 7473 0a20 2020 2020 2020 2020  limits.         
-00027360: 2020 2066 6978 5061 7273 3d5b 2261 222c     fixPars=["a",
-00027370: 2022 6222 5d2c 2020 2320 6669 7820 7061   "b"],  # fix pa
-00027380: 7261 6d65 7465 7228 7329 0a20 2020 2020  rameter(s).     
-00027390: 2020 2020 2020 206e 6567 326c 6f67 4c3d         neg2logL=
-000273a0: 5472 7565 2c20 2023 2075 7365 2020 2d32  True,  # use  -2
-000273b0: 202a 206c 6e28 4c29 0a20 2020 2020 2020   * ln(L).       
-000273c0: 2020 2020 2070 6c6f 743d 5472 7565 2c20       plot=True, 
-000273d0: 2023 2070 6c6f 7420 6461 7461 2061 6e64   # plot data and
-000273e0: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
-000273f0: 2020 2070 6c6f 745f 6261 6e64 3d54 7275     plot_band=Tru
-00027400: 652c 2020 2320 706c 6f74 206d 6f64 656c  e,  # plot model
-00027410: 2063 6f6e 6669 6465 6e63 652d 6261 6e64   confidence-band
-00027420: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
-00027430: 745f 636f 723d 4661 6c73 652c 2020 2320  t_cor=False,  # 
-00027440: 706c 6f74 2070 726f 6669 6c65 7320 6c69  plot profiles li
-00027450: 6b65 6c69 686f 6f64 2061 6e64 2063 6f6e  kelihood and con
-00027460: 746f 7572 730a 2020 2020 2020 2020 2020  tours.          
-00027470: 2020 7368 6f77 706c 6f74 733d 4661 6c73    showplots=Fals
-00027480: 652c 2020 2320 7368 6f77 202f 2064 6f6e  e,  # show / don
-00027490: 2774 2073 686f 7720 706c 6f74 730a 2020  't show plots.  
-000274a0: 2020 2020 2020 2020 2020 7175 6965 743d            quiet=
-000274b0: 4661 6c73 652c 2020 2320 7375 7070 7265  False,  # suppre
-000274c0: 7373 2069 6e66 6f72 6d61 7469 7665 2070  ss informative p
-000274d0: 7269 6e74 6f75 7420 6966 2054 7275 650a  rintout if True.
-000274e0: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-000274f0: 5f6c 6162 656c 733d 5b0a 2020 2020 2020  _labels=[.      
-00027500: 2020 2020 2020 2020 2020 226c 6966 6520            "life 
-00027510: 7469 6d65 2020 2220 2b20 2224 5c44 656c  time  " + "$\Del
-00027520: 7461 2474 2028 245c 6d75 2473 2922 2c0a  ta$t ($\mu$s)",.
-00027530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027540: 2250 726f 6261 6269 6c69 7479 2044 656e  "Probability Den
-00027550: 7369 7479 2020 7064 6628 245c 4465 6c74  sity  pdf($\Delt
-00027560: 6124 743b 202a 7029 222c 0a20 2020 2020  a$t; *p)",.     
-00027570: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00027580: 2020 2020 2020 6461 7461 5f6c 6567 656e        data_legen
-00027590: 643d 2224 5c6d 7524 206c 6966 6574 696d  d="$\mu$ lifetim
-000275a0: 6520 6461 7461 222c 0a20 2020 2020 2020  e data",.       
-000275b0: 2020 2020 206d 6f64 656c 5f6c 6567 656e       model_legen
-000275c0: 643d 2265 7870 6f6e 656e 7469 616c 2064  d="exponential d
-000275d0: 6563 6179 202b 2066 6c61 7420 6261 636b  ecay + flat back
-000275e0: 6772 6f75 6e64 222c 0a20 2020 2020 2020  ground",.       
-000275f0: 2029 0a0a 2020 2020 2020 2020 706c 742e   )..        plt.
-00027600: 7375 7074 6974 6c65 280a 2020 2020 2020  suptitle(.      
-00027610: 2020 2020 2020 2255 6e62 696e 6e65 6420        "Unbinned 
-00027620: 4d4c 2066 6974 206f 6620 616e 2065 7870  ML fit of an exp
-00027630: 6f6e 656e 7469 616c 202b 2066 6c61 7420  onential + flat 
-00027640: 6469 7374 7269 6275 7469 6f6e 222c 0a20  distribution",. 
-00027650: 2020 2020 2020 2020 2020 2073 697a 653d             size=
-00027660: 2278 782d 6c61 7267 6522 2c0a 2020 2020  "xx-large",.    
-00027670: 2020 2020 2020 2020 636f 6c6f 723d 2264          color="d
-00027680: 6172 6b62 6c75 6522 2c0a 2020 2020 2020  arkblue",.      
-00027690: 2020 290a 2020 2020 2020 2020 2320 5072    ).        # Pr
-000276a0: 696e 7420 7265 7375 6c74 730a 2020 2020  int results.    
-000276b0: 2020 2020 7076 616c 732c 2070 6572 7273      pvals, perrs
-000276c0: 2c20 636f 722c 2067 6f66 2c20 706e 616d  , cor, gof, pnam
-000276d0: 7320 3d20 7265 7375 6c74 4469 6374 2e76  s = resultDict.v
-000276e0: 616c 7565 7328 290a 2020 2020 2020 2020  alues().        
-000276f0: 7072 696e 7428 225c 6e2a 3d3d 2a20 756e  print("\n*==* un
-00027700: 6269 6e6e 6564 204d 4c20 4669 7420 5265  binned ML Fit Re
-00027710: 7375 6c74 3a22 290a 2020 2020 2020 2020  sult:").        
-00027720: 7072 696e 7428 2220 7061 7261 6d65 7465  print(" paramete
-00027730: 7220 6e61 6d65 733a 2020 2020 2020 2022  r names:       "
-00027740: 2c20 706e 616d 7329 0a20 2020 2020 2020  , pnams).       
-00027750: 2070 7269 6e74 2822 2070 6172 616d 6574   print(" paramet
-00027760: 6572 2076 616c 7565 733a 2020 2020 2020  er values:      
-00027770: 222c 2070 7661 6c73 290a 2020 2020 2020  ", pvals).      
-00027780: 2020 7072 696e 7428 2220 6e65 672e 2070    print(" neg. p
-00027790: 6172 616d 6574 6572 2065 7272 6f72 733a  arameter errors:
-000277a0: 2022 2c20 7065 7272 735b 3a2c 2030 5d29   ", perrs[:, 0])
-000277b0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-000277c0: 2070 6f73 2e20 7061 7261 6d65 7465 7220   pos. parameter 
-000277d0: 6572 726f 7273 3a20 222c 2070 6572 7273  errors: ", perrs
-000277e0: 5b3a 2c20 315d 290a 2020 2020 2020 2020  [:, 1]).        
-000277f0: 7072 696e 7428 2220 636f 7272 656c 6174  print(" correlat
-00027800: 696f 6e73 203a 205c 6e22 2c20 636f 7229  ions : \n", cor)
-00027810: 0a0a 2020 2020 230a 2020 2020 2320 2d2d  ..    #.    # --
-00027820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00022e00: 2020 2020 2020 2020 6361 7073 697a 653d          capsize=
+00022e10: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
+00022e20: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00022e30: 6c70 6861 3d30 2e36 362c 0a20 2020 2020  lpha=0.66,.     
+00022e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022e50: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00022e60: 2023 2072 6573 746f 7265 2063 6f6c 6f72   # restore color
+00022e70: 206d 6170 0a20 2020 2020 2020 2020 2020   map.           
+00022e80: 2070 6c74 2e73 6574 5f63 6d61 7028 6f72   plt.set_cmap(or
+00022e90: 6967 5f63 6d29 0a0a 2020 2020 2020 2020  ig_cm)..        
+00022ea0: 2020 2020 7265 7475 726e 2063 6f72 5f66      return cor_f
+00022eb0: 6967 0a0a 2020 2020 2020 2020 6578 6365  ig..        exce
+00022ec0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00022ed0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00022ee0: 7269 6e74 2822 2a3d 3d2a 2021 2121 2070  rint("*==* !!! p
+00022ef0: 726f 6669 6c65 2061 6e64 2063 6f6e 746f  rofile and conto
+00022f00: 7572 2073 6361 6e20 6661 696c 6564 2229  ur scan failed")
+00022f10: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00022f20: 6e74 2865 290a 2020 2020 2020 2020 2020  nt(e).          
+00022f30: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+00022f40: 2020 2064 6566 2067 6574 5072 6f66 696c     def getProfil
+00022f50: 6528 7365 6c66 2c20 706e 616d 2c20 7261  e(self, pnam, ra
+00022f60: 6e67 653d 332e 302c 206e 706f 696e 7473  nge=3.0, npoints
+00022f70: 3d33 3029 3a0a 2020 2020 2020 2020 2222  =30):.        ""
+00022f80: 2272 6574 7572 6e20 7072 6f66 696c 6520  "return profile 
+00022f90: 6c69 6b65 6c69 686f 6f64 206f 6620 7061  likelihood of pa
+00022fa0: 7261 6d65 7465 7220 706e 616d 0a0a 2020  rameter pnam..  
+00022fb0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00022fc0: 2020 2020 2020 2d20 7061 7261 6d65 7465        - paramete
+00022fd0: 7220 6e61 6d65 0a20 2020 2020 2020 2020  r name.         
+00022fe0: 202d 2073 6361 6e20 7261 6e67 6520 696e   - scan range in
+00022ff0: 2073 6967 6d61 2c20 6172 6520 7475 706c   sigma, are tupl
+00023000: 6520 7769 7468 206c 6f77 6572 2061 6e64  e with lower and
+00023010: 2075 7070 6572 2076 616c 7565 0a20 2020   upper value.   
+00023020: 2020 2020 2020 202d 206e 756d 6265 7220         - number 
+00023030: 6f66 2070 6f69 6e74 730a 2020 2020 2020  of points.      
+00023040: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00023050: 2073 656c 662e 696d 696e 7569 745f 7665   self.iminuit_ve
+00023060: 7273 696f 6e20 3c20 2232 223a 0a20 2020  rsion < "2":.   
+00023070: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00023080: 2121 2120 6765 7450 726f 6669 6c65 206e  !!! getProfile n
+00023090: 6f74 2069 6d70 6c65 6d65 6e74 6564 2076  ot implemented v
+000230a0: 6f72 2069 6d69 6e75 6974 2076 6572 732e  or iminuit vers.
+000230b0: 3c32 2229 0a20 2020 2020 2020 2020 2020  <2").           
+000230c0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+000230d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000230e0: 2020 7265 7475 726e 2073 656c 662e 6d69    return self.mi
+000230f0: 6e75 6974 2e6d 6e70 726f 6669 6c65 280a  nuit.mnprofile(.
+00023100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023110: 706e 616d 2c20 626f 756e 643d 7261 6e67  pnam, bound=rang
+00023120: 652c 2073 697a 653d 6e70 6f69 6e74 732c  e, size=npoints,
+00023130: 2073 7562 7472 6163 745f 6d69 6e3d 5472   subtract_min=Tr
+00023140: 7565 0a20 2020 2020 2020 2020 2020 2029  ue.            )
+00023150: 0a0a 2020 2020 6465 6620 6765 7443 6f6e  ..    def getCon
+00023160: 746f 7572 2873 656c 662c 2070 6e61 6d31  tour(self, pnam1
+00023170: 2c20 706e 616d 322c 2063 6c3d 4e6f 6e65  , pnam2, cl=None
+00023180: 2c20 6e70 6f69 6e74 733d 3130 3029 3a0a  , npoints=100):.
+00023190: 2020 2020 2020 2020 2222 2272 6574 7572          """retur
+000231a0: 6e20 7072 6f66 696c 6520 6c69 6b65 6c69  n profile likeli
+000231b0: 686f 6f64 2063 6f6e 746f 7572 206f 6620  hood contour of 
+000231c0: 7061 7261 6d65 7465 7273 2070 6e61 6d31  parameters pnam1
+000231d0: 2061 6e64 2070 6e61 6d32 0a0a 2020 2020   and pnam2..    
+000231e0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000231f0: 2020 2020 2d20 3173 7420 7061 7261 6d65      - 1st parame
+00023200: 7465 7220 6e61 6d65 0a20 2020 2020 2020  ter name.       
+00023210: 2020 202d 2032 6e64 2070 6172 616d 6574     - 2nd paramet
+00023220: 6572 206e 616d 650a 2020 2020 2020 2020  er name.        
+00023230: 2020 2d20 636f 6e66 6964 656e 6365 206c    - confidence l
+00023240: 6576 656c 0a20 2020 2020 2020 2020 202d  evel.          -
+00023250: 206e 756d 6265 7220 6f66 2070 6f69 6e74   number of point
+00023260: 730a 0a20 2020 2020 2020 2052 6574 7572  s..        Retur
+00023270: 6e73 3a0a 2020 2020 2020 2020 2020 2d20  ns:.          - 
+00023280: 6172 7261 7920 6f66 2066 6c6f 6174 2028  array of float (
+00023290: 6e70 6f69 6e74 7320 2a20 3229 2063 6f6e  npoints * 2) con
+000232a0: 746f 7572 2070 6f69 6e74 730a 2020 2020  tour points.    
+000232b0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+000232c0: 2069 6620 7365 6c66 2e69 6d69 6e75 6974   if self.iminuit
+000232d0: 5f76 6572 7369 6f6e 203c 2022 3222 3a0a  _version < "2":.
+000232e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000232f0: 7428 2221 2121 2067 6574 436f 6e74 6f75  t("!!! getContou
+00023300: 7220 6e6f 7420 696d 706c 656d 656e 7465  r not implemente
+00023310: 6420 766f 7220 696d 696e 7569 7420 7665  d vor iminuit ve
+00023320: 7273 2e3c 3222 290a 2020 2020 2020 2020  rs.<2").        
+00023330: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00023340: 2020 2072 6574 7572 6e20 7365 6c66 2e6d     return self.m
+00023350: 696e 7569 742e 6d6e 636f 6e74 6f75 7228  inuit.mncontour(
+00023360: 706e 616d 312c 2070 6e61 6d32 2c20 636c  pnam1, pnam2, cl
+00023370: 3d63 6c2c 2073 697a 653d 6e70 6f69 6e74  =cl, size=npoint
+00023380: 7329 0a0a 2020 2020 6465 6620 706c 6f74  s)..    def plot
+00023390: 5f50 726f 6669 6c65 2873 656c 662c 2070  _Profile(self, p
+000233a0: 6e61 6d2c 2072 616e 6765 3d32 2e30 2c20  nam, range=2.0, 
+000233b0: 6e70 6f69 6e74 733d 3330 293a 0a20 2020  npoints=30):.   
+000233c0: 2020 2020 2022 2222 706c 6f74 2070 726f       """plot pro
+000233d0: 6669 6c65 206c 696b 656c 6968 6f6f 6420  file likelihood 
+000233e0: 6f66 2070 6172 616d 6574 6572 2070 6e61  of parameter pna
+000233f0: 6d0a 0a20 2020 2020 2020 2041 7267 733a  m..        Args:
+00023400: 0a20 2020 2020 2020 2020 202d 2070 6172  .          - par
+00023410: 616d 6574 6572 206e 616d 650a 2020 2020  ameter name.    
+00023420: 2020 2020 2020 2d20 7363 616e 2072 616e        - scan ran
+00023430: 6765 2069 6e20 7369 676d 612c 2061 7265  ge in sigma, are
+00023440: 2074 7570 6c65 2077 6974 6820 6c6f 7765   tuple with lowe
+00023450: 7220 616e 6420 7570 7065 7220 7661 6c75  r and upper valu
+00023460: 650a 2020 2020 2020 2020 2020 2d20 6e75  e.          - nu
+00023470: 6d62 6572 206f 6620 706f 696e 7473 0a0a  mber of points..
+00023480: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00023490: 0a20 2020 2020 2020 2020 202d 206d 6174  .          - mat
+000234a0: 706c 6f74 6c69 6220 6669 6775 7265 0a20  plotlib figure. 
+000234b0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+000234c0: 2020 2020 6669 6720 3d20 706c 742e 6669      fig = plt.fi
+000234d0: 6775 7265 286e 756d 3d22 4c69 6b65 6c69  gure(num="Likeli
+000234e0: 686f 6f64 2070 726f 6669 6c65 2022 202b  hood profile " +
+000234f0: 2070 6e61 6d2c 2066 6967 7369 7a65 3d28   pnam, figsize=(
+00023500: 352e 302c 2035 2e30 2929 0a20 2020 2020  5.0, 5.0)).     
+00023510: 2020 2073 656c 662e 6d69 6e75 6974 2e64     self.minuit.d
+00023520: 7261 775f 6d6e 7072 6f66 696c 6528 706e  raw_mnprofile(pn
+00023530: 616d 2c20 626f 756e 643d 7261 6e67 652c  am, bound=range,
+00023540: 2073 697a 653d 6e70 6f69 6e74 732c 2073   size=npoints, s
+00023550: 7562 7472 6163 745f 6d69 6e3d 5472 7565  ubtract_min=True
+00023560: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00023570: 6c66 2e45 7272 4465 6620 3d3d 2031 3a0a  lf.ErrDef == 1:.
+00023580: 2020 2020 2020 2020 2020 2020 796c 6162              ylab
+00023590: 656c 203d 2022 245c 4465 6c74 6120 282d  el = "$\Delta (-
+000235a0: 325c 6c6e 5c63 616c 7b4c 7d29 2422 0a20  2\ln\cal{L})$". 
+000235b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000235c0: 2020 2020 2020 2020 2079 6c61 6265 6c20           ylabel 
+000235d0: 3d20 2224 5c44 656c 7461 2028 2d5c 6c6e  = "$\Delta (-\ln
+000235e0: 5c63 616c 7b4c 7d29 2422 0a20 2020 2020  \cal{L})$".     
+000235f0: 2020 2070 6c74 2e79 6c61 6265 6c28 796c     plt.ylabel(yl
+00023600: 6162 656c 290a 2020 2020 2020 2020 7265  abel).        re
+00023610: 7475 726e 2066 6967 0a0a 2020 2020 6465  turn fig..    de
+00023620: 6620 706c 6f74 5f63 6c43 6f6e 746f 7572  f plot_clContour
+00023630: 2873 656c 662c 2070 6e61 6d31 2c20 706e  (self, pnam1, pn
+00023640: 616d 322c 2063 6c29 3a0a 2020 2020 2020  am2, cl):.      
+00023650: 2020 2222 2270 6c6f 7420 6120 636f 6e74    """plot a cont
+00023660: 6f75 7220 6f66 2070 6172 616d 6574 6572  our of parameter
+00023670: 7320 706e 616d 3120 616e 6420 706e 616d  s pnam1 and pnam
+00023680: 320a 2020 2020 2020 2020 7769 7468 2063  2.        with c
+00023690: 6f6e 6669 6465 6e63 6520 6c65 7665 6c28  onfidence level(
+000236a0: 7329 2063 6c0a 2020 2020 2020 2020 2222  s) cl.        ""
+000236b0: 220a 2020 2020 2020 2020 6966 2073 656c  ".        if sel
+000236c0: 662e 696d 696e 7569 745f 7665 7273 696f  f.iminuit_versio
+000236d0: 6e20 3c20 2232 223a 0a20 2020 2020 2020  n < "2":.       
+000236e0: 2020 2020 2070 7269 6e74 2822 2121 2120       print("!!! 
+000236f0: 706c 6f74 5f63 6c43 6f6e 746f 7572 206e  plot_clContour n
+00023700: 6f74 2069 6d70 6c65 6d65 6e74 6564 2076  ot implemented v
+00023710: 6f72 2069 6d69 6e75 6974 2076 6572 732e  or iminuit vers.
+00023720: 3c32 2229 0a20 2020 2020 2020 2020 2020  <2").           
+00023730: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00023740: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00023750: 2020 6669 6720 3d20 706c 742e 6669 6775    fig = plt.figu
+00023760: 7265 280a 2020 2020 2020 2020 2020 2020  re(.            
+00023770: 2020 2020 6e75 6d3d 2243 6f6e 746f 7572      num="Contour
+00023780: 2873 2920 2220 2b20 706e 616d 3120 2b20  (s) " + pnam1 + 
+00023790: 2220 7673 2e20 2220 2b20 706e 616d 322c  " vs. " + pnam2,
+000237a0: 2066 6967 7369 7a65 3d28 352e 302c 2035   figsize=(5.0, 5
+000237b0: 2e30 290a 2020 2020 2020 2020 2020 2020  .0).            
+000237c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000237d0: 6c66 2e6d 696e 7569 742e 6472 6177 5f6d  lf.minuit.draw_m
+000237e0: 6e63 6f6e 746f 7572 2870 6e61 6d31 2c20  ncontour(pnam1, 
+000237f0: 706e 616d 322c 2063 6c3d 636c 290a 2020  pnam2, cl=cl).  
+00023800: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00023810: 2066 6967 0a0a 2020 2020 6465 6620 706c   fig..    def pl
+00023820: 6f74 5f6e 7369 6743 6f6e 746f 7572 2873  ot_nsigContour(s
+00023830: 656c 662c 2070 6e61 6d31 2c20 706e 616d  elf, pnam1, pnam
+00023840: 322c 206e 7369 6729 3a0a 2020 2020 2020  2, nsig):.      
+00023850: 2020 2222 2270 6c6f 7420 6e73 6967 2063    """plot nsig c
+00023860: 6f6e 746f 7572 7320 6f66 2070 6172 616d  ontours of param
+00023870: 6574 6572 7320 706e 616d 3120 616e 6420  eters pnam1 and 
+00023880: 706e 616d 3222 2222 0a20 2020 2020 2020  pnam2""".       
+00023890: 2066 6967 203d 2070 6c74 2e66 6967 7572   fig = plt.figur
+000238a0: 6528 0a20 2020 2020 2020 2020 2020 206e  e(.            n
+000238b0: 756d 3d22 436f 6e74 6f75 7228 7329 2022  um="Contour(s) "
+000238c0: 202b 2070 6e61 6d31 202b 2022 2076 732e   + pnam1 + " vs.
+000238d0: 2022 202b 2070 6e61 6d32 2c20 6669 6773   " + pnam2, figs
+000238e0: 697a 653d 2835 2e30 2c20 352e 3029 0a20  ize=(5.0, 5.0). 
+000238f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00023900: 2069 6620 7365 6c66 2e69 6d69 6e75 6974   if self.iminuit
+00023910: 5f76 6572 7369 6f6e 203c 2022 3222 3a0a  _version < "2":.
+00023920: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00023930: 2e6d 696e 7569 742e 6472 6177 5f6d 6e63  .minuit.draw_mnc
+00023940: 6f6e 746f 7572 2870 6e61 6d31 2c20 706e  ontour(pnam1, pn
+00023950: 616d 322c 206e 7369 676d 613d 6e73 6967  am2, nsigma=nsig
+00023960: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00023970: 2020 2020 2020 2020 2020 2020 6e73 203d              ns =
+00023980: 2072 616e 6765 2831 2c20 6e73 6967 202b   range(1, nsig +
+00023990: 2031 290a 2020 2020 2020 2020 2020 2020   1).            
+000239a0: 6463 6869 3220 3d20 6e70 2e61 7272 6179  dchi2 = np.array
+000239b0: 286e 7329 202a 2a20 320a 2020 2020 2020  (ns) ** 2.      
+000239c0: 2020 2020 2020 636c 203d 2073 656c 662e        cl = self.
+000239d0: 4368 6932 3243 4c28 6463 6869 3229 0a20  Chi22CL(dchi2). 
+000239e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000239f0: 6d69 6e75 6974 2e64 7261 775f 6d6e 636f  minuit.draw_mnco
+00023a00: 6e74 6f75 7228 706e 616d 312c 2070 6e61  ntour(pnam1, pna
+00023a10: 6d32 2c20 636c 3d63 6c29 0a20 2020 2020  m2, cl=cl).     
+00023a20: 2020 2072 6574 7572 6e20 6669 670a 0a20     return fig.. 
+00023a30: 2020 2040 7374 6174 6963 6d65 7468 6f64     @staticmethod
+00023a40: 0a20 2020 2064 6566 2063 6869 3270 7262  .    def chi2prb
+00023a50: 2863 6869 322c 206e 646f 6629 3a0a 2020  (chi2, ndof):.  
+00023a60: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+00023a70: 7465 2063 6869 322d 7072 6f62 6162 696c  te chi2-probabil
+00023a80: 6974 7920 6672 6f6d 2063 6869 3220 616e  ity from chi2 an
+00023a90: 6420 6465 6772 6565 7320 6f66 2066 7265  d degrees of fre
+00023aa0: 6564 6f6d 2222 220a 2020 2020 2020 2020  edom""".        
+00023ab0: 7265 7475 726e 2031 2e30 202d 2073 7461  return 1.0 - sta
+00023ac0: 7473 2e63 6869 322e 6364 6628 6368 6932  ts.chi2.cdf(chi2
+00023ad0: 2c20 6e64 6f66 290a 0a20 2020 2040 7374  , ndof)..    @st
+00023ae0: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00023af0: 6566 2043 4c32 4368 6932 2843 4c29 3a0a  ef CL2Chi2(CL):.
+00023b00: 2020 2020 2020 2020 2222 2263 616c 6375          """calcu
+00023b10: 6c61 7465 2044 656c 7461 4368 6932 2066  late DeltaChi2 f
+00023b20: 726f 6d20 636f 6e66 6964 656e 6365 206c  rom confidence l
+00023b30: 6576 656c 2043 4c20 666f 7220 322d 6469  evel CL for 2-di
+00023b40: 6d20 636f 6e74 6f75 7273 2222 220a 2020  m contours""".  
+00023b50: 2020 2020 2020 7265 7475 726e 202d 322e        return -2.
+00023b60: 3020 2a20 6e70 2e6c 6f67 2831 2e30 202d  0 * np.log(1.0 -
+00023b70: 2043 4c29 0a0a 2020 2020 4073 7461 7469   CL)..    @stati
+00023b80: 636d 6574 686f 640a 2020 2020 6465 6620  cmethod.    def 
+00023b90: 4368 6932 3243 4c28 6463 3229 3a0a 2020  Chi22CL(dc2):.  
+00023ba0: 2020 2020 2020 2222 2263 616c 6375 6c61        """calcula
+00023bb0: 7465 2063 6f6e 6669 6465 6e63 6520 6c65  te confidence le
+00023bc0: 7665 6c20 434c 2066 726f 6d20 4465 6c74  vel CL from Delt
+00023bd0: 6143 6869 3220 666f 7220 322d 6469 6d20  aChi2 for 2-dim 
+00023be0: 636f 6e74 6f75 7273 2222 220a 2020 2020  contours""".    
+00023bf0: 2020 2020 7265 7475 726e 2031 2e30 202d      return 1.0 -
+00023c00: 206e 702e 6578 7028 2d64 6332 202f 2032   np.exp(-dc2 / 2
+00023c10: 2e30 290a 0a0a 6966 205f 5f6e 616d 655f  .0)...if __name_
+00023c20: 5f20 3d3d 2022 5f5f 6d61 696e 5f5f 223a  _ == "__main__":
+00023c30: 2020 2320 2d2d 2d20 696e 7465 7266 6163    # --- interfac
+00023c40: 6520 616e 6420 6578 616d 706c 650a 0a20  e and example.. 
+00023c50: 2020 2064 6566 2065 7861 6d70 6c65 5f78     def example_x
+00023c60: 7946 6974 2829 3a0a 2020 2020 2020 2020  yFit():.        
+00023c70: 230a 2020 2020 2020 2020 2320 2a2a 2a20  #.        # *** 
+00023c80: 4578 616d 706c 6520 6f66 2061 6e20 6170  Example of an ap
+00023c90: 706c 6963 6174 696f 6e20 6f66 2070 6879  plication of phy
+00023ca0: 4669 742e 7879 4669 7428 290a 2020 2020  Fit.xyFit().    
+00023cb0: 2020 2020 230a 2020 2020 2020 2020 2320      #.        # 
+00023cc0: 6465 6669 6e65 2074 6865 206d 6f64 656c  define the model
+00023cd0: 2066 756e 6374 696f 6e20 746f 2066 6974   function to fit
+00023ce0: 0a20 2020 2020 2020 2064 6566 2065 7870  .        def exp
+00023cf0: 5f6d 6f64 656c 2878 2c20 413d 312e 302c  _model(x, A=1.0,
+00023d00: 2078 303d 312e 3029 3a0a 2020 2020 2020   x0=1.0):.      
+00023d10: 2020 2020 2020 7265 7475 726e 2041 202a        return A *
+00023d20: 206e 702e 6578 7028 2d78 202f 2078 3029   np.exp(-x / x0)
+00023d30: 0a0a 2020 2020 2020 2020 2320 616e 6f74  ..        # anot
+00023d40: 6865 7220 6d6f 6465 6c20 6675 6e63 7469  her model functi
+00023d50: 6f6e 0a20 2020 2020 2020 2064 6566 2070  on.        def p
+00023d60: 6f6c 7932 5f6d 6f64 656c 2878 2c20 613d  oly2_model(x, a=
+00023d70: 302e 312c 2062 3d31 2e30 2c20 633d 312e  0.1, b=1.0, c=1.
+00023d80: 3029 3a0a 2020 2020 2020 2020 2020 2020  0):.            
+00023d90: 7265 7475 726e 2061 202a 2078 2a2a 3220  return a * x**2 
+00023da0: 2b20 6220 2a20 7820 2b20 630a 0a20 2020  + b * x + c..   
+00023db0: 2020 2020 2023 2073 6574 206d 6f64 656c       # set model
+00023dc0: 2074 6f20 7573 6520 696e 2066 6974 0a20   to use in fit. 
+00023dd0: 2020 2020 2020 2066 6974 6d6f 6465 6c20         fitmodel 
+00023de0: 3d20 6578 705f 6d6f 6465 6c20 2023 2061  = exp_model  # a
+00023df0: 6c73 6f20 7472 7920 706f 6c79 325f 6d6f  lso try poly2_mo
+00023e00: 6465 6c20 210a 0a20 2020 2020 2020 2023  del !..        #
+00023e10: 2074 6865 2064 6174 6120 2e2e 2e0a 2020   the data ....  
+00023e20: 2020 2020 2020 6461 7461 5f78 203d 205b        data_x = [
+00023e30: 302e 302c 2030 2e32 2c20 302e 342c 2030  0.0, 0.2, 0.4, 0
+00023e40: 2e36 2c20 302e 382c 2031 2e30 2c20 312e  .6, 0.8, 1.0, 1.
+00023e50: 322c 2031 2e34 2c20 312e 362c 2031 2e38  2, 1.4, 1.6, 1.8
+00023e60: 2c20 322e 302c 2032 2e32 2c20 322e 342c  , 2.0, 2.2, 2.4,
+00023e70: 2032 2e36 5d0a 2020 2020 2020 2020 6461   2.6].        da
+00023e80: 7461 5f79 203d 205b 0a20 2020 2020 2020  ta_y = [.       
+00023e90: 2020 2020 2031 2e31 3439 2c0a 2020 2020       1.149,.    
+00023ea0: 2020 2020 2020 2020 302e 3731 322c 0a20          0.712,. 
+00023eb0: 2020 2020 2020 2020 2020 2030 2e38 3033             0.803
+00023ec0: 2c0a 2020 2020 2020 2020 2020 2020 302e  ,.            0.
+00023ed0: 3436 342c 0a20 2020 2020 2020 2020 2020  464,.           
+00023ee0: 2030 2e33 3938 2c0a 2020 2020 2020 2020   0.398,.        
+00023ef0: 2020 2020 302e 3335 342c 0a20 2020 2020      0.354,.     
+00023f00: 2020 2020 2020 2030 2e31 3438 2c0a 2020         0.148,.  
+00023f10: 2020 2020 2020 2020 2020 302e 3332 382c            0.328,
+00023f20: 0a20 2020 2020 2020 2020 2020 2030 2e31  .            0.1
+00023f30: 3831 2c0a 2020 2020 2020 2020 2020 2020  81,.            
+00023f40: 302e 3134 302c 0a20 2020 2020 2020 2020  0.140,.         
+00023f50: 2020 2030 2e30 3635 2c0a 2020 2020 2020     0.065,.      
+00023f60: 2020 2020 2020 302e 3030 352c 0a20 2020        0.005,.   
+00023f70: 2020 2020 2020 2020 202d 302e 3030 352c           -0.005,
+00023f80: 0a20 2020 2020 2020 2020 2020 2030 2e31  .            0.1
+00023f90: 3136 2c0a 2020 2020 2020 2020 5d0a 2020  16,.        ].  
+00023fa0: 2020 2020 2020 2320 2e2e 2e20 616e 6420        # ... and 
+00023fb0: 756e 6365 7274 6169 7469 6573 0a20 2020  uncertaities.   
+00023fc0: 2020 2020 2073 6162 7379 203d 2030 2e30       sabsy = 0.0
+00023fd0: 3720 2023 2069 6e64 6570 656e 6465 6e74  7  # independent
+00023fe0: 2079 0a20 2020 2020 2020 2073 7265 6c79   y.        srely
+00023ff0: 203d 2030 2e30 3520 2023 2035 2520 6f66   = 0.05  # 5% of
+00024000: 206d 6f64 656c 2076 616c 7565 0a20 2020   model value.   
+00024010: 2020 2020 2063 6162 7379 203d 2030 2e30       cabsy = 0.0
+00024020: 3420 2023 2063 6f72 7265 6c61 7465 640a  4  # correlated.
+00024030: 2020 2020 2020 2020 6372 656c 7920 3d20          crely = 
+00024040: 302e 3033 2020 2320 3325 206f 6620 6d6f  0.03  # 3% of mo
+00024050: 6465 6c20 7661 6c75 6520 636f 7272 656c  del value correl
+00024060: 6174 6564 0a20 2020 2020 2020 2073 6162  ated.        sab
+00024070: 7378 203d 2030 2e30 3520 2023 2069 6e64  sx = 0.05  # ind
+00024080: 6570 656e 6465 6e74 2078 0a20 2020 2020  ependent x.     
+00024090: 2020 2073 7265 6c78 203d 2030 2e30 3420     srelx = 0.04 
+000240a0: 2023 2034 2520 6f66 2078 0a20 2020 2020   # 4% of x.     
+000240b0: 2020 2063 6162 7378 203d 2030 2e30 3320     cabsx = 0.03 
+000240c0: 2023 2063 6f72 7265 6c61 7465 6420 780a   # correlated x.
+000240d0: 2020 2020 2020 2020 6372 656c 7820 3d20          crelx = 
+000240e0: 302e 3032 2020 2320 3225 206f 6620 7820  0.02  # 2% of x 
+000240f0: 636f 7272 656c 6174 6564 0a0a 2020 2020  correlated..    
+00024100: 2020 2020 2320 7065 7266 6f72 6d20 6669      # perform fi
+00024110: 7420 746f 2064 6174 6120 7769 7468 2066  t to data with f
+00024120: 756e 6374 696f 6e20 7879 4669 7420 7573  unction xyFit us
+00024130: 696e 6720 636c 6173 7320 6d6e 4669 740a  ing class mnFit.
+00024140: 2020 2020 2020 2020 7265 7375 6c74 4469          resultDi
+00024150: 6374 203d 2078 7946 6974 280a 2020 2020  ct = xyFit(.    
+00024160: 2020 2020 2020 2020 6669 746d 6f64 656c          fitmodel
+00024170: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00024180: 7461 5f78 2c0a 2020 2020 2020 2020 2020  ta_x,.          
+00024190: 2020 6461 7461 5f79 2c0a 2020 2020 2020    data_y,.      
+000241a0: 2020 2020 2020 7378 3d73 6162 7378 2c0a        sx=sabsx,.
+000241b0: 2020 2020 2020 2020 2020 2020 7379 3d73              sy=s
+000241c0: 6162 7379 2c0a 2020 2020 2020 2020 2020  absy,.          
+000241d0: 2020 7372 656c 783d 7372 656c 782c 0a20    srelx=srelx,. 
+000241e0: 2020 2020 2020 2020 2020 2073 7265 6c79             srely
+000241f0: 3d73 7265 6c79 2c0a 2020 2020 2020 2020  =srely,.        
+00024200: 2020 2020 7861 6273 636f 723d 6361 6273      xabscor=cabs
+00024210: 782c 0a20 2020 2020 2020 2020 2020 2078  x,.            x
+00024220: 7265 6c63 6f72 3d63 7265 6c78 2c0a 2020  relcor=crelx,.  
+00024230: 2020 2020 2020 2020 2020 7961 6273 636f            yabsco
+00024240: 723d 6361 6273 792c 0a20 2020 2020 2020  r=cabsy,.       
+00024250: 2020 2020 2079 7265 6c63 6f72 3d63 7265       yrelcor=cre
+00024260: 6c79 2c0a 2020 2020 2020 2020 2020 2020  ly,.            
+00024270: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00024280: 2020 2070 303d 2831 2e2c 2030 2e35 292c     p0=(1., 0.5),
+00024290: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
+000242a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000242b0: 636f 6e73 7472 6169 6e74 733d 5b27 4127  constraints=['A'
+000242c0: 2c20 312e 2c20 302e 3033 5d2c 0a20 2020  , 1., 0.03],.   
+000242d0: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+000242e0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+000242f0: 7472 6169 6e74 733d 5b30 2c20 312e 2c20  traints=[0, 1., 
+00024300: 302e 3033 5d20 2861 6c74 6572 6e61 7469  0.03] (alternati
+00024310: 7665 290a 2020 2020 2020 2020 2020 2020  ve).            
+00024320: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+00024330: 2020 206c 696d 6974 733d 2827 4127 2c20     limits=('A', 
+00024340: 302e 2c20 4e6f 6e65 292c 2020 2320 7061  0., None),  # pa
+00024350: 7261 6d65 7465 7220 6c69 6d69 7473 0a20  rameter limits. 
+00024360: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00024370: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00024380: 7850 6172 7320 3d20 5b27 4127 5d2c 2020  xPars = ['A'],  
+00024390: 2020 2020 2020 2023 2066 6978 2070 6172         # fix par
+000243a0: 616d 6574 6572 2873 290a 2020 2020 2020  ameter(s).      
+000243b0: 2020 2020 2020 7573 655f 6e65 674c 6f67        use_negLog
+000243c0: 4c3d 5472 7565 2c0a 2020 2020 2020 2020  L=True,.        
+000243d0: 2020 2020 706c 6f74 3d54 7275 652c 0a20      plot=True,. 
+000243e0: 2020 2020 2020 2020 2020 2070 6c6f 745f             plot_
+000243f0: 6261 6e64 3d54 7275 652c 0a20 2020 2020  band=True,.     
+00024400: 2020 2020 2020 2070 6c6f 745f 636f 723d         plot_cor=
+00024410: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+00024420: 2020 2073 686f 7770 6c6f 7473 3d46 616c     showplots=Fal
+00024430: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00024440: 7175 6965 743d 4661 6c73 652c 0a20 2020  quiet=False,.   
+00024450: 2020 2020 2020 2020 2061 7869 735f 6c61           axis_la
+00024460: 6265 6c73 3d5b 2278 222c 2022 7920 2020  bels=["x", "y   
+00024470: 5c20 2066 2878 2c20 2a70 6172 2922 5d2c  \  f(x, *par)"],
+00024480: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00024490: 615f 6c65 6765 6e64 3d22 7261 6e64 6f6d  a_legend="random
+000244a0: 2064 6174 6122 2c0a 2020 2020 2020 2020   data",.        
+000244b0: 2020 2020 6d6f 6465 6c5f 6c65 6765 6e64      model_legend
+000244c0: 3d22 6d6f 6465 6c22 2c0a 2020 2020 2020  ="model",.      
+000244d0: 2020 290a 2020 2020 2020 2020 706c 742e    ).        plt.
+000244e0: 7375 7074 6974 6c65 280a 2020 2020 2020  suptitle(.      
+000244f0: 2020 2020 2020 226d 6e46 6974 2065 7861        "mnFit exa
+00024500: 6d70 6c65 3a20 6669 7420 746f 2078 2d79  mple: fit to x-y
+00024510: 2064 6174 6122 2c20 7369 7a65 3d22 7878   data", size="xx
+00024520: 2d6c 6172 6765 222c 2063 6f6c 6f72 3d22  -large", color="
+00024530: 6461 726b 626c 7565 220a 2020 2020 2020  darkblue".      
+00024540: 2020 290a 0a20 2020 2020 2020 2023 2050    )..        # P
+00024550: 7269 6e74 2072 6573 756c 7473 0a20 2020  rint results.   
+00024560: 2020 2020 2070 7661 6c73 2c20 7065 7272       pvals, perr
+00024570: 732c 2063 6f72 2c20 6368 6932 2c20 706e  s, cor, chi2, pn
+00024580: 616d 7320 3d20 7265 7375 6c74 4469 6374  ams = resultDict
+00024590: 2e76 616c 7565 7328 290a 2020 2020 2020  .values().      
+000245a0: 2020 7072 696e 7428 225c 6e2a 3d3d 2a20    print("\n*==* 
+000245b0: 7879 4669 7420 5265 7375 6c74 3a22 290a  xyFit Result:").
+000245c0: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+000245d0: 7061 7261 6d65 7465 7220 6e61 6d65 733a  parameter names:
+000245e0: 2020 2020 2020 2022 2c20 706e 616d 7329         ", pnams)
+000245f0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00024600: 2063 6869 323a 207b 3a2e 3367 7d22 2e66   chi2: {:.3g}".f
+00024610: 6f72 6d61 7428 6368 6932 2929 0a20 2020  ormat(chi2)).   
+00024620: 2020 2020 2070 7269 6e74 2822 2070 6172       print(" par
+00024630: 616d 6574 6572 2076 616c 7565 733a 2020  ameter values:  
+00024640: 2020 2020 222c 2070 7661 6c73 290a 2020      ", pvals).  
+00024650: 2020 2020 2020 7072 696e 7428 2220 6e65        print(" ne
+00024660: 672e 2070 6172 616d 6574 6572 2065 7272  g. parameter err
+00024670: 6f72 733a 2022 2c20 7065 7272 735b 3a2c  ors: ", perrs[:,
+00024680: 2030 5d29 0a20 2020 2020 2020 2070 7269   0]).        pri
+00024690: 6e74 2822 2070 6f73 2e20 7061 7261 6d65  nt(" pos. parame
+000246a0: 7465 7220 6572 726f 7273 3a20 222c 2070  ter errors: ", p
+000246b0: 6572 7273 5b3a 2c20 315d 290a 2020 2020  errs[:, 1]).    
+000246c0: 2020 2020 7072 696e 7428 2220 636f 7272      print(" corr
+000246d0: 656c 6174 696f 6e73 203a 205c 6e22 2c20  elations : \n", 
+000246e0: 636f 7229 0a0a 2020 2020 6465 6620 6578  cor)..    def ex
+000246f0: 616d 706c 655f 696e 6465 7865 6446 6974  ample_indexedFit
+00024700: 2829 3a0a 2020 2020 2020 2020 230a 2020  ():.        #.  
+00024710: 2020 2020 2020 2320 2a2a 2a20 4578 616d        # *** Exam
+00024720: 706c 6520 6f66 2061 6e20 6170 706c 6963  ple of an applic
+00024730: 6174 696f 6e20 6f66 2070 6879 4669 742e  ation of phyFit.
+00024740: 7846 6974 2829 2074 6f20 6669 7420 696e  xFit() to fit in
+00024750: 6465 7865 6420 6461 7461 0a20 2020 2020  dexed data.     
+00024760: 2020 2023 0a20 2020 2020 2020 2023 2020     #.        #  
+00024770: 2020 2043 6f6f 7264 696e 6174 6573 2069     Coordinates i
+00024780: 6e20 722d 7068 6920 6172 6520 6176 6572  n r-phi are aver
+00024790: 6167 6564 2061 6e64 2074 7261 6e73 666f  aged and transfo
+000247a0: 726d 6564 2074 6f20 6361 7274 6573 6961  rmed to cartesia
+000247b0: 6e0a 0a20 2020 2020 2020 2064 6566 2063  n..        def c
+000247c0: 6172 7465 7369 616e 5f74 6f5f 706f 6c61  artesian_to_pola
+000247d0: 7228 6461 7461 2c20 783d 312e 302c 2079  r(data, x=1.0, y
+000247e0: 3d31 2e30 293a 0a20 2020 2020 2020 2020  =1.0):.         
+000247f0: 2020 2023 2064 6574 6572 6d69 6e65 2070     # determine p
+00024800: 6f6c 6172 2063 6f6f 7264 696e 6174 7320  olar coordinats 
+00024810: 6672 6f6d 2063 6172 7465 7369 616e 2028  from cartesian (
+00024820: 782c 7929 0a20 2020 2020 2020 2020 2020  x,y).           
+00024830: 206e 6d20 3d20 6c65 6e28 6461 7461 2920   nm = len(data) 
+00024840: 2f2f 2032 2020 2320 6578 7065 6374 2074  // 2  # expect t
+00024850: 776f 2061 7272 6179 7320 7769 7468 206d  wo arrays with m
+00024860: 6561 7375 7265 6d65 6e74 730a 2020 2020  easurements.    
+00024870: 2020 2020 2020 2020 7220 3d20 6e70 2e73          r = np.s
+00024880: 7172 7428 7820 2a20 7820 2b20 7920 2a20  qrt(x * x + y * 
+00024890: 7929 202a 206e 702e 6f6e 6573 286e 6d29  y) * np.ones(nm)
+000248a0: 0a20 2020 2020 2020 2020 2020 2070 6869  .            phi
+000248b0: 203d 206e 702e 6172 6374 616e 3228 792c   = np.arctan2(y,
+000248c0: 2078 2920 2a20 6e70 2e6f 6e65 7328 6e6d   x) * np.ones(nm
+000248d0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+000248e0: 7475 726e 206e 702e 636f 6e63 6174 656e  turn np.concaten
+000248f0: 6174 6528 2872 2c20 7068 6929 290a 0a20  ate((r, phi)).. 
+00024900: 2020 2020 2020 2023 2065 7861 6d70 6c65         # example
+00024910: 3a20 2872 2c20 7068 6929 206f 6620 7477  : (r, phi) of tw
+00024920: 6f20 7370 6163 6520 706f 696e 7473 2069  o space points i
+00024930: 6e20 706f 6c61 7220 636f 6f72 6469 6e61  n polar coordina
+00024940: 7465 730a 2020 2020 2020 2020 7061 7273  tes.        pars
+00024950: 203d 206e 702e 6172 7261 7928 5b30 2e39   = np.array([0.9
+00024960: 2c20 302e 3837 2c20 302e 3735 352c 2030  , 0.87, 0.755, 0
+00024970: 2e37 3930 5d29 0a20 2020 2020 2020 2070  .790]).        p
+00024980: 756e 6373 203d 206e 702e 6172 7261 7928  uncs = np.array(
+00024990: 5b30 2e30 3237 2c20 302e 3032 332c 2030  [0.027, 0.023, 0
+000249a0: 2e31 362c 2030 2e31 335d 290a 0a20 2020  .16, 0.13])..   
+000249b0: 2020 2020 2023 2070 6572 666f 726d 2066       # perform f
+000249c0: 6974 2074 6f20 6461 7461 2077 6974 6820  it to data with 
+000249d0: 6675 6e63 7469 6f6e 2078 4669 7420 7573  function xFit us
+000249e0: 696e 6720 636c 6173 7320 6d6e 4669 740a  ing class mnFit.
+000249f0: 2020 2020 2020 2020 7265 7375 6c74 4469          resultDi
+00024a00: 6374 203d 2078 4669 7428 0a20 2020 2020  ct = xFit(.     
+00024a10: 2020 2020 2020 2063 6172 7465 7369 616e         cartesian
+00024a20: 5f74 6f5f 706f 6c61 722c 0a20 2020 2020  _to_polar,.     
+00024a30: 2020 2020 2020 2070 6172 732c 0a20 2020         pars,.   
+00024a40: 2020 2020 2020 2020 2073 3d70 756e 6373           s=puncs
+00024a50: 2c0a 2020 2020 2020 2020 2020 2020 7372  ,.            sr
+00024a60: 656c 3d4e 6f6e 652c 0a20 2020 2020 2020  el=None,.       
+00024a70: 2020 2020 2073 6162 7363 6f72 3d4e 6f6e       sabscor=Non
+00024a80: 652c 0a20 2020 2020 2020 2020 2020 2073  e,.            s
+00024a90: 7265 6c63 6f72 3d4e 6f6e 652c 0a20 2020  relcor=None,.   
+00024aa0: 2020 2020 2020 2020 206e 616d 6573 3d5b           names=[
+00024ab0: 2272 222c 2022 7222 2c20 7222 245c 7661  "r", "r", r"$\va
+00024ac0: 7270 6869 2422 2c20 7222 245c 7661 7270  rphi$", r"$\varp
+00024ad0: 6869 2422 5d2c 0a20 2020 2020 2020 2020  hi$"],.         
+00024ae0: 2020 2023 2070 303d 2831 2e2c 2031 2e29     # p0=(1., 1.)
+00024af0: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
+00024b00: 655f 6e65 674c 6f67 4c3d 5472 7565 2c0a  e_negLogL=True,.
+00024b10: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
+00024b20: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00024b30: 2020 2070 6c6f 745f 6261 6e64 3d54 7275     plot_band=Tru
+00024b40: 652c 0a20 2020 2020 2020 2020 2020 2070  e,.            p
+00024b50: 6c6f 745f 636f 723d 5472 7565 2c0a 2020  lot_cor=True,.  
+00024b60: 2020 2020 2020 2020 2020 7368 6f77 706c            showpl
+00024b70: 6f74 733d 4661 6c73 652c 0a20 2020 2020  ots=False,.     
+00024b80: 2020 2020 2020 2071 7569 6574 3d46 616c         quiet=Fal
+00024b90: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00024ba0: 6178 6973 5f6c 6162 656c 733d 5b22 496e  axis_labels=["In
+00024bb0: 6465 7822 2c20 2278 2020 205c 2020 7828  dex", "x   \  x(
+00024bc0: 2a70 6172 2922 5d2c 0a20 2020 2020 2020  *par)"],.       
+00024bd0: 2020 2020 2064 6174 615f 6c65 6765 6e64       data_legend
+00024be0: 3d22 506f 6c61 7220 4461 7461 222c 0a20  ="Polar Data",. 
+00024bf0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+00024c00: 5f6c 6567 656e 643d 2272 2d70 6869 2066  _legend="r-phi f
+00024c10: 726f 6d20 782d 7922 2c0a 2020 2020 2020  rom x-y",.      
+00024c20: 2020 290a 2020 2020 2020 2020 706c 742e    ).        plt.
+00024c30: 7375 7074 6974 6c65 280a 2020 2020 2020  suptitle(.      
+00024c40: 2020 2020 2020 226d 6e46 6974 2065 7861        "mnFit exa
+00024c50: 6d70 6c65 3a20 6669 7420 746f 2069 6e64  mple: fit to ind
+00024c60: 6578 6564 2064 6174 6122 2c20 7369 7a65  exed data", size
+00024c70: 3d22 7878 2d6c 6172 6765 222c 2063 6f6c  ="xx-large", col
+00024c80: 6f72 3d22 6461 726b 626c 7565 220a 2020  or="darkblue".  
+00024c90: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00024ca0: 2023 2050 7269 6e74 2072 6573 756c 7473   # Print results
+00024cb0: 0a20 2020 2020 2020 2070 7661 6c73 2c20  .        pvals, 
+00024cc0: 7065 7272 732c 2063 6f72 2c20 6368 6932  perrs, cor, chi2
+00024cd0: 2c20 706e 616d 7320 3d20 7265 7375 6c74  , pnams = result
+00024ce0: 4469 6374 2e76 616c 7565 7328 290a 2020  Dict.values().  
+00024cf0: 2020 2020 2020 7072 696e 7428 225c 6e2a        print("\n*
+00024d00: 3d3d 2a20 7879 4669 7420 5265 7375 6c74  ==* xyFit Result
+00024d10: 3a22 290a 2020 2020 2020 2020 7072 696e  :").        prin
+00024d20: 7428 2220 7061 7261 6d65 7465 7220 6e61  t(" parameter na
+00024d30: 6d65 733a 2020 2020 2020 2022 2c20 706e  mes:       ", pn
+00024d40: 616d 7329 0a20 2020 2020 2020 2070 7269  ams).        pri
+00024d50: 6e74 2822 2063 6869 323a 207b 3a2e 3367  nt(" chi2: {:.3g
+00024d60: 7d22 2e66 6f72 6d61 7428 6368 6932 2929  }".format(chi2))
+00024d70: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00024d80: 2070 6172 616d 6574 6572 2076 616c 7565   parameter value
+00024d90: 733a 2020 2020 2020 222c 2070 7661 6c73  s:      ", pvals
+00024da0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00024db0: 2220 6e65 672e 2070 6172 616d 6574 6572  " neg. parameter
+00024dc0: 2065 7272 6f72 733a 2022 2c20 7065 7272   errors: ", perr
+00024dd0: 735b 3a2c 2030 5d29 0a20 2020 2020 2020  s[:, 0]).       
+00024de0: 2070 7269 6e74 2822 2070 6f73 2e20 7061   print(" pos. pa
+00024df0: 7261 6d65 7465 7220 6572 726f 7273 3a20  rameter errors: 
+00024e00: 222c 2070 6572 7273 5b3a 2c20 315d 290a  ", perrs[:, 1]).
+00024e10: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+00024e20: 636f 7272 656c 6174 696f 6e73 203a 205c  correlations : \
+00024e30: 6e22 2c20 636f 7229 0a0a 2020 2020 6465  n", cor)..    de
+00024e40: 6620 6578 616d 706c 655f 6869 7374 6f67  f example_histog
+00024e50: 7261 6d46 6974 2829 3a0a 2020 2020 2020  ramFit():.      
+00024e60: 2020 230a 2020 2020 2020 2020 2320 2a2a    #.        # **
+00024e70: 2a20 4869 7374 6f67 7261 6d20 4669 743a  * Histogram Fit:
+00024e80: 2045 7861 6d70 6c65 206f 6620 616e 2061   Example of an a
+00024e90: 7070 6c69 6361 7469 6f6e 206f 6620 7068  pplication of ph
+00024ea0: 7946 6974 2e68 4669 7428 290a 2020 2020  yFit.hFit().    
+00024eb0: 2020 2020 230a 0a20 2020 2020 2020 2023      #..        #
+00024ec0: 2020 2020 2320 6465 6669 6e65 2074 6865      # define the
+00024ed0: 206d 6f64 656c 2066 756e 6374 696f 6e20   model function 
+00024ee0: 746f 2066 6974 0a20 2020 2020 2020 2064  to fit.        d
+00024ef0: 6566 2053 706c 7573 425f 6d6f 6465 6c28  ef SplusB_model(
+00024f00: 782c 206d 753d 362e 3938 372c 2073 6967  x, mu=6.987, sig
+00024f10: 6d61 3d30 2e35 2c20 613d 302e 302c 2073  ma=0.5, a=0.0, s
+00024f20: 3d30 2e32 293a 0a20 2020 2020 2020 2020  =0.2):.         
+00024f30: 2020 2022 2222 7064 6620 6f66 2061 2047     """pdf of a G
+00024f40: 6175 7373 6961 6e20 7369 676e 616c 206f  aussian signal o
+00024f50: 6e20 746f 7020 6f66 2066 6c61 7420 6261  n top of flat ba
+00024f60: 636b 6772 6f75 6e64 2222 220a 2020 2020  ckground""".    
+00024f70: 2020 2020 2020 2020 6e6f 726d 616c 203d          normal =
+00024f80: 206e 702e 6578 7028 2d30 2e35 202a 2028   np.exp(-0.5 * (
+00024f90: 2878 202d 206d 7529 202f 2073 6967 6d61  (x - mu) / sigma
+00024fa0: 2920 2a2a 2032 2920 2f20 6e70 2e73 7172  ) ** 2) / np.sqr
+00024fb0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00024fc0: 2020 2032 2e30 202a 206e 702e 7069 202a     2.0 * np.pi *
+00024fd0: 2073 6967 6d61 2a2a 320a 2020 2020 2020   sigma**2.      
+00024fe0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00024ff0: 2020 2020 6c69 6e65 6172 203d 2028 6120      linear = (a 
+00025000: 2a20 2878 6d78 202b 2078 6d6e 2920 2f20  * (xmx + xmn) / 
+00025010: 3220 2b20 312e 3029 202f 2028 786d 7820  2 + 1.0) / (xmx 
+00025020: 2d20 786d 6e29 0a20 2020 2020 2020 2020  - xmn).         
+00025030: 2020 2072 6574 7572 6e20 7320 2a20 6e6f     return s * no
+00025040: 726d 616c 202b 2028 3120 2d20 7329 202a  rmal + (1 - s) *
+00025050: 206c 696e 6561 720a 0a20 2020 2020 2020   linear..       
+00025060: 206e 6269 6e73 203d 2034 300a 2020 2020   nbins = 40.    
+00025070: 2020 2020 786d 6e20 3d20 310a 2020 2020      xmn = 1.    
+00025080: 2020 2020 786d 7820 3d20 3130 0a20 2020      xmx = 10.   
+00025090: 2020 2020 2062 6564 6765 7320 3d20 6e70       bedges = np
+000250a0: 2e6c 696e 7370 6163 6528 786d 6e2c 2078  .linspace(xmn, x
+000250b0: 6d78 2c20 6e62 696e 7320 2b20 3129 0a20  mx, nbins + 1). 
+000250c0: 2020 2020 2020 2062 636f 6e74 656e 7473         bcontents
+000250d0: 203d 206e 702e 6172 7261 7928 0a20 2020   = np.array(.   
+000250e0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
+000250f0: 2020 2020 2020 2020 2020 2031 2c0a 2020             1,.  
+00025100: 2020 2020 2020 2020 2020 2020 2020 312c                1,
+00025110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025120: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+00025130: 2020 2020 322c 0a20 2020 2020 2020 2020      2,.         
+00025140: 2020 2020 2020 2032 2c0a 2020 2020 2020         2,.      
+00025150: 2020 2020 2020 2020 2020 322c 0a20 2020            2,.   
+00025160: 2020 2020 2020 2020 2020 2020 2034 2c0a               4,.
+00025170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025180: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+00025190: 2020 2030 2c0a 2020 2020 2020 2020 2020     0,.          
+000251a0: 2020 2020 2020 332c 0a20 2020 2020 2020        3,.       
+000251b0: 2020 2020 2020 2020 2031 2c0a 2020 2020           1,.    
+000251c0: 2020 2020 2020 2020 2020 2020 312c 0a20              1,. 
+000251d0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+000251e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000251f0: 2020 322c 0a20 2020 2020 2020 2020 2020    2,.           
+00025200: 2020 2020 2033 2c0a 2020 2020 2020 2020       3,.        
+00025210: 2020 2020 2020 2020 332c 0a20 2020 2020          3,.     
+00025220: 2020 2020 2020 2020 2020 2031 2c0a 2020             1,.  
+00025230: 2020 2020 2020 2020 2020 2020 2020 312c                1,
+00025240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025250: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
+00025260: 2020 2020 322c 0a20 2020 2020 2020 2020      2,.         
+00025270: 2020 2020 2020 2033 2c0a 2020 2020 2020         3,.      
+00025280: 2020 2020 2020 2020 2020 322c 0a20 2020            2,.   
+00025290: 2020 2020 2020 2020 2020 2020 2033 2c0a               3,.
+000252a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000252b0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+000252c0: 2020 2031 2c0a 2020 2020 2020 2020 2020     1,.          
+000252d0: 2020 2020 2020 382c 0a20 2020 2020 2020        8,.       
+000252e0: 2020 2020 2020 2020 2036 2c0a 2020 2020           6,.    
+000252f0: 2020 2020 2020 2020 2020 2020 372c 0a20              7,. 
+00025300: 2020 2020 2020 2020 2020 2020 2020 2039                 9
+00025310: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00025320: 2020 312c 0a20 2020 2020 2020 2020 2020    1,.           
+00025330: 2020 2020 2030 2c0a 2020 2020 2020 2020       0,.        
+00025340: 2020 2020 2020 2020 312c 0a20 2020 2020          1,.     
+00025350: 2020 2020 2020 2020 2020 2032 2c0a 2020             2,.  
+00025360: 2020 2020 2020 2020 2020 2020 2020 312c                1,
+00025370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025380: 2033 2c0a 2020 2020 2020 2020 2020 2020   3,.            
+00025390: 2020 2020 322c 0a20 2020 2020 2020 2020      2,.         
+000253a0: 2020 2020 2020 2031 2c0a 2020 2020 2020         1,.      
+000253b0: 2020 2020 2020 2020 2020 332c 0a20 2020            3,.   
+000253c0: 2020 2020 2020 2020 2020 2020 2032 2c0a               2,.
+000253d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000253e0: 342c 0a20 2020 2020 2020 2020 2020 205d  4,.            ]
+000253f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00025400: 2020 2023 0a20 2020 2020 2020 2023 202d     #.        # -
+00025410: 2d2d 2020 7065 7266 6f72 6d20 6669 740a  --  perform fit.
+00025420: 2020 2020 2020 2020 230a 2020 2020 2020          #.      
+00025430: 2020 7265 7375 6c74 4469 6374 203d 2068    resultDict = h
+00025440: 4669 7428 0a20 2020 2020 2020 2020 2020  Fit(.           
+00025450: 2053 706c 7573 425f 6d6f 6465 6c2c 0a20   SplusB_model,. 
+00025460: 2020 2020 2020 2020 2020 2062 636f 6e74             bcont
+00025470: 656e 7473 2c0a 2020 2020 2020 2020 2020  ents,.          
+00025480: 2020 6265 6467 6573 2c20 2023 2062 696e    bedges,  # bin
+00025490: 2065 6e74 7269 6573 2061 6e64 2062 696e   entries and bin
+000254a0: 2065 6467 6573 0a20 2020 2020 2020 2020   edges.         
+000254b0: 2020 2070 303d 4e6f 6e65 2c20 2023 2069     p0=None,  # i
+000254c0: 6e69 7469 616c 2067 7565 7373 2066 6f72  nitial guess for
+000254d0: 2070 6172 616d 6574 6572 2076 616c 7565   parameter value
+000254e0: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
+000254f0: 2020 2020 636f 6e73 7472 6169 6e74 733d      constraints=
+00025500: 5b27 7327 2c20 7661 6c20 2c20 6572 7220  ['s', val , err 
+00025510: 5d2c 2020 2023 2063 6f6e 7374 7261 696e  ],   # constrain
+00025520: 7473 2077 6974 6869 6e20 6572 726f 7273  ts within errors
+00025530: 0a20 2020 2020 2020 2020 2020 2066 6978  .            fix
+00025540: 5061 7273 3d5b 2261 225d 2c20 2023 2066  Pars=["a"],  # f
+00025550: 6978 2070 6172 616d 6574 6572 2873 290a  ix parameter(s).
+00025560: 2020 2020 2020 2020 2020 2020 6c69 6d69              limi
+00025570: 7473 3d28 2273 222c 2030 2e30 2c20 4e6f  ts=("s", 0.0, No
+00025580: 6e65 292c 2020 2320 6c69 6d69 7473 0a20  ne),  # limits. 
+00025590: 2020 2020 2020 2020 2020 2075 7365 5f47             use_G
+000255a0: 6175 7373 4170 7072 6f78 3d46 616c 7365  aussApprox=False
+000255b0: 2c20 2023 2047 6175 7373 6961 6e20 6170  ,  # Gaussian ap
+000255c0: 7072 6f78 696d 6174 696f 6e0a 2020 2020  proximation.    
+000255d0: 2020 2020 2020 2020 6669 745f 6465 6e73          fit_dens
+000255e0: 6974 793d 5472 7565 2c20 2023 2066 6974  ity=True,  # fit
+000255f0: 2064 656e 7369 7479 0a20 2020 2020 2020   density.       
+00025600: 2020 2020 2070 6c6f 743d 5472 7565 2c20       plot=True, 
+00025610: 2023 2070 6c6f 7420 6461 7461 2061 6e64   # plot data and
+00025620: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
+00025630: 2020 2070 6c6f 745f 6261 6e64 3d54 7275     plot_band=Tru
+00025640: 652c 2020 2320 706c 6f74 206d 6f64 656c  e,  # plot model
+00025650: 2063 6f6e 6669 6465 6e63 652d 6261 6e64   confidence-band
+00025660: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
+00025670: 745f 636f 723d 5472 7565 2c20 2023 2070  t_cor=True,  # p
+00025680: 6c6f 7420 7072 6f66 696c 6573 206c 696b  lot profiles lik
+00025690: 656c 6968 6f6f 6420 616e 6420 636f 6e74  elihood and cont
+000256a0: 6f75 7273 0a20 2020 2020 2020 2020 2020  ours.           
+000256b0: 2073 686f 7770 6c6f 7473 3d46 616c 7365   showplots=False
+000256c0: 2c20 2023 2073 686f 7720 2f20 646f 6e27  ,  # show / don'
+000256d0: 7420 7368 6f77 2070 6c6f 7473 0a20 2020  t show plots.   
+000256e0: 2020 2020 2020 2020 2071 7569 6574 3d46           quiet=F
+000256f0: 616c 7365 2c20 2023 2073 7570 7072 6573  alse,  # suppres
+00025700: 7320 696e 666f 726d 6174 6976 6520 7072  s informative pr
+00025710: 696e 746f 7574 0a20 2020 2020 2020 2020  intout.         
+00025720: 2020 2061 7869 735f 6c61 6265 6c73 3d5b     axis_labels=[
+00025730: 2278 222c 2022 7920 2020 5c20 2066 2878  "x", "y   \  f(x
+00025740: 2c20 2a70 6172 2922 5d2c 0a20 2020 2020  , *par)"],.     
+00025750: 2020 2020 2020 2064 6174 615f 6c65 6765         data_lege
+00025760: 6e64 3d22 7261 6e64 6f6d 2064 6174 6122  nd="random data"
+00025770: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
+00025780: 6465 6c5f 6c65 6765 6e64 3d22 7369 676e  del_legend="sign
+00025790: 616c 202b 2062 6163 6b67 726f 756e 6420  al + background 
+000257a0: 6d6f 6465 6c22 2c0a 2020 2020 2020 2020  model",.        
+000257b0: 290a 0a20 2020 2020 2020 2070 6c74 2e73  )..        plt.s
+000257c0: 7570 7469 746c 6528 0a20 2020 2020 2020  uptitle(.       
+000257d0: 2020 2020 2022 6d6e 4669 7420 6578 616d       "mnFit exam
+000257e0: 706c 653a 2066 6974 2074 6f20 6869 7374  ple: fit to hist
+000257f0: 6f67 7261 6d20 6461 7461 222c 2073 697a  ogram data", siz
+00025800: 653d 2278 782d 6c61 7267 6522 2c20 636f  e="xx-large", co
+00025810: 6c6f 723d 2264 6172 6b62 6c75 6522 0a20  lor="darkblue". 
+00025820: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00025830: 2020 2320 5072 696e 7420 7265 7375 6c74    # Print result
+00025840: 730a 2020 2020 2020 2020 7072 696e 7428  s.        print(
+00025850: 225c 6e2a 3d3d 2a20 6869 7374 6f67 7261  "\n*==* histogra
+00025860: 6d20 6669 7420 5265 7375 6c74 3a22 290a  m fit Result:").
+00025870: 2020 2020 2020 2020 7076 616c 732c 2070          pvals, p
+00025880: 6572 7273 2c20 636f 722c 2067 6f66 2c20  errs, cor, gof, 
+00025890: 706e 616d 7320 3d20 7265 7375 6c74 4469  pnams = resultDi
+000258a0: 6374 2e76 616c 7565 7328 290a 2020 2020  ct.values().    
+000258b0: 2020 2020 7072 696e 7428 2220 7061 7261      print(" para
+000258c0: 6d65 7465 7220 6e61 6d65 733a 2020 2020  meter names:    
+000258d0: 2020 2022 2c20 706e 616d 7329 0a20 2020     ", pnams).   
+000258e0: 2020 2020 2070 7269 6e74 2822 2067 6f6f       print(" goo
+000258f0: 646e 6573 732d 6f66 2d66 6974 3a20 7b3a  dness-of-fit: {:
+00025900: 2e33 677d 222e 666f 726d 6174 2867 6f66  .3g}".format(gof
+00025910: 2929 0a20 2020 2020 2020 2070 7269 6e74  )).        print
+00025920: 2822 2070 6172 616d 6574 6572 2076 616c  (" parameter val
+00025930: 7565 733a 2020 2020 2020 222c 2070 7661  ues:      ", pva
+00025940: 6c73 290a 2020 2020 2020 2020 7072 696e  ls).        prin
+00025950: 7428 2220 6e65 672e 2070 6172 616d 6574  t(" neg. paramet
+00025960: 6572 2065 7272 6f72 733a 2022 2c20 7065  er errors: ", pe
+00025970: 7272 735b 3a2c 2030 5d29 0a20 2020 2020  rrs[:, 0]).     
+00025980: 2020 2070 7269 6e74 2822 2070 6f73 2e20     print(" pos. 
+00025990: 7061 7261 6d65 7465 7220 6572 726f 7273  parameter errors
+000259a0: 3a20 222c 2070 6572 7273 5b3a 2c20 315d  : ", perrs[:, 1]
+000259b0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+000259c0: 2220 636f 7272 656c 6174 696f 6e73 203a  " correlations :
+000259d0: 205c 6e22 2c20 636f 7229 0a0a 2020 2020   \n", cor)..    
+000259e0: 6465 6620 6578 616d 706c 655f 7573 6572  def example_user
+000259f0: 4669 7428 293a 0a20 2020 2020 2020 2022  Fit():.        "
+00025a00: 2222 2a2a 756e 6269 6e6e 6564 204d 4c20  ""**unbinned ML 
+00025a10: 6669 742a 2a20 7769 7468 2075 7365 722d  fit** with user-
+00025a20: 6465 6669 6e65 6420 636f 7374 2066 756e  defined cost fun
+00025a30: 6374 696f 6e0a 0a20 2020 2020 2020 2054  ction..        T
+00025a40: 6869 7320 636f 6465 2069 6c6c 7573 7472  his code illustr
+00025a50: 6174 6573 2075 7361 6765 206f 6620 7468  ates usage of th
+00025a60: 6520 7772 6170 7065 7220 6675 6e63 7469  e wrapper functi
+00025a70: 6f6e 206d 4669 7428 290a 2020 2020 2020  on mFit().      
+00025a80: 2020 666f 7220 2063 6c61 7373 202a 2a6d    for  class **m
+00025a90: 6e46 6974 2a2a 2075 7365 722d 6465 6669  nFit** user-defi
+00025aa0: 6e65 6420 636f 7374 2066 756e 6374 696f  ned cost functio
+00025ab0: 6e0a 2020 2020 2020 2020 2222 220a 0a20  n.        """.. 
+00025ac0: 2020 2020 2020 2023 2067 656e 6572 6174         # generat
+00025ad0: 6520 4761 7573 7369 616e 2d64 6973 7472  e Gaussian-distr
+00025ae0: 6962 7574 6564 2064 6174 610a 2020 2020  ibuted data.    
+00025af0: 2020 2020 6d75 3020 3d20 322e 300a 2020      mu0 = 2.0.  
+00025b00: 2020 2020 2020 7369 6730 203d 2030 2e35        sig0 = 0.5
+00025b10: 0a20 2020 2020 2020 206e 702e 7261 6e64  .        np.rand
+00025b20: 6f6d 2e73 6565 6428 3331 3431 3539 2920  om.seed(314159) 
+00025b30: 2023 2069 6e69 7469 616c 697a 6520 7261   # initialize ra
+00025b40: 6e64 6f6d 2067 656e 6572 6174 6f72 0a20  ndom generator. 
+00025b50: 2020 2020 2020 2064 6174 6120 3d20 6d75         data = mu
+00025b60: 3020 2b20 7369 6730 202a 206e 702e 7261  0 + sig0 * np.ra
+00025b70: 6e64 6f6d 2e72 616e 646e 2831 3030 290a  ndom.randn(100).
+00025b80: 0a20 2020 2020 2020 2023 2064 6566 696e  .        # defin
+00025b90: 6520 636f 7374 2066 756e 6374 696f 6e3a  e cost function:
+00025ba0: 2032 202a 206e 6567 6174 6976 6520 6c6f   2 * negative lo
+00025bb0: 6720 6c69 6b65 6c69 686f 6f64 206f 6620  g likelihood of 
+00025bc0: 4761 75c3 9f3b 0a20 2020 2020 2020 2064  Gau..;.        d
+00025bd0: 6566 206d 7943 6f73 7428 6d75 3d31 2e30  ef myCost(mu=1.0
+00025be0: 2c20 7369 676d 613d 312e 3029 3a0a 2020  , sigma=1.0):.  
+00025bf0: 2020 2020 2020 2020 2020 2320 7369 6d70            # simp
+00025c00: 6c65 202d 322a 6c6f 672d 6c69 6b65 6c69  le -2*log-likeli
+00025c10: 686f 6f64 206f 6620 6120 312d 6420 4761  hood of a 1-d Ga
+00025c20: 7573 7320 6469 7374 7269 6275 7469 6f6e  uss distribution
+00025c30: 0a20 2020 2020 2020 2020 2020 2072 203d  .            r =
+00025c40: 2028 6461 7461 202d 206d 7529 202f 2073   (data - mu) / s
+00025c50: 6967 6d61 0a20 2020 2020 2020 2020 2020  igma.           
+00025c60: 2072 6574 7572 6e20 6e70 2e73 756d 2872   return np.sum(r
+00025c70: 202a 2072 202b 2032 2e30 202a 206e 702e   * r + 2.0 * np.
+00025c80: 6c6f 6728 7369 676d 6129 290a 0a20 2020  log(sigma))..   
+00025c90: 2020 2020 2072 6573 756c 7444 6963 7420       resultDict 
+00025ca0: 3d20 6d46 6974 280a 2020 2020 2020 2020  = mFit(.        
+00025cb0: 2020 2020 6d79 436f 7374 2c0a 2020 2020      myCost,.    
+00025cc0: 2020 2020 2020 2020 7030 3d4e 6f6e 652c          p0=None,
+00025cd0: 2020 2320 696e 6974 6961 6c20 6775 6573    # initial gues
+00025ce0: 7320 666f 7220 7061 7261 6d65 7465 7220  s for parameter 
+00025cf0: 7661 6c75 6573 0a20 2020 2020 2020 2020  values.         
+00025d00: 2020 2063 6f6e 7374 7261 696e 7473 3d5b     constraints=[
+00025d10: 5b22 6d75 222c 2032 2e30 2c20 302e 3031  ["mu", 2.0, 0.01
+00025d20: 5d5d 2c20 2023 2047 6175 7373 6961 6e20  ]],  # Gaussian 
+00025d30: 7061 7261 6d65 7465 7220 636f 6e73 7472  parameter constr
+00025d40: 6169 6e74 730a 2020 2020 2020 2020 2020  aints.          
+00025d50: 2020 2320 206c 696d 6974 733d 2827 7369    #  limits=('si
+00025d60: 676d 6127 2c20 4e6f 6e65 2c20 4e6f 6e65  gma', None, None
+00025d70: 292c 2020 236c 696d 6974 730a 2020 2020  ),  #limits.    
+00025d80: 2020 2020 2020 2020 2320 2066 6978 5061          #  fixPa
+00025d90: 7273 203d 205b 276d 7527 5d2c 2020 2020  rs = ['mu'],    
+00025da0: 2020 2020 2320 6669 7820 7061 7261 6d65      # fix parame
+00025db0: 7465 7228 7329 0a20 2020 2020 2020 2020  ter(s).         
+00025dc0: 2020 206e 6567 326c 6f67 4c3d 5472 7565     neg2logL=True
+00025dd0: 2c20 2023 2063 6f73 7420 6973 202d 3220  ,  # cost is -2 
+00025de0: 2a20 6c6e 284c 290a 2020 2020 2020 2020  * ln(L).        
+00025df0: 2020 2020 706c 6f74 5f63 6f72 3d54 7275      plot_cor=Tru
+00025e00: 652c 2020 2320 706c 6f74 2070 726f 6669  e,  # plot profi
+00025e10: 6c65 7320 6c69 6b65 6c69 686f 6f64 2061  les likelihood a
+00025e20: 6e64 2063 6f6e 746f 7572 730a 2020 2020  nd contours.    
+00025e30: 2020 2020 2020 2020 7368 6f77 706c 6f74          showplot
+00025e40: 733d 4661 6c73 652c 2020 2320 7368 6f77  s=False,  # show
+00025e50: 202f 2064 6f6e 2774 2073 686f 7720 706c   / don't show pl
+00025e60: 6f74 730a 2020 2020 2020 2020 2020 2020  ots.            
+00025e70: 7175 6965 743d 4661 6c73 652c 2020 2320  quiet=False,  # 
+00025e80: 7375 7070 7265 7373 2069 6e66 6f72 6d61  suppress informa
+00025e90: 7469 7665 2070 7269 6e74 6f75 740a 2020  tive printout.  
+00025ea0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00025eb0: 2070 6c74 2e73 7570 7469 746c 6528 0a20   plt.suptitle(. 
+00025ec0: 2020 2020 2020 2020 2020 2022 4d61 7869             "Maxi
+00025ed0: 6d75 6d2d 6c69 6b65 6c69 686f 6f64 2066  mum-likelihood f
+00025ee0: 6974 3a20 7072 6f66 696c 6573 2061 6e64  it: profiles and
+00025ef0: 2063 6f6e 746f 7572 7322 2c0a 2020 2020   contours",.    
+00025f00: 2020 2020 2020 2020 7369 7a65 3d22 7878          size="xx
+00025f10: 2d6c 6172 6765 222c 0a20 2020 2020 2020  -large",.       
+00025f20: 2020 2020 2063 6f6c 6f72 3d22 6461 726b       color="dark
+00025f30: 626c 7565 222c 0a20 2020 2020 2020 2029  blue",.        )
+00025f40: 0a20 2020 2020 2020 2023 2050 7269 6e74  .        # Print
+00025f50: 2072 6573 756c 7473 0a20 2020 2020 2020   results.       
+00025f60: 2070 7661 6c73 2c20 7065 7272 732c 2063   pvals, perrs, c
+00025f70: 6f72 2c20 676f 662c 2070 6e61 6d73 203d  or, gof, pnams =
+00025f80: 2072 6573 756c 7444 6963 742e 7661 6c75   resultDict.valu
+00025f90: 6573 2829 0a20 2020 2020 2020 2070 7269  es().        pri
+00025fa0: 6e74 2822 5c6e 2a3d 3d2a 2075 7365 722d  nt("\n*==* user-
+00025fb0: 6465 6669 6e65 6420 636f 7374 3a20 4669  defined cost: Fi
+00025fc0: 7420 5265 7375 6c74 3a22 290a 2020 2020  t Result:").    
+00025fd0: 2020 2020 7072 696e 7428 2220 7061 7261      print(" para
+00025fe0: 6d65 7465 7220 6e61 6d65 733a 2020 2020  meter names:    
+00025ff0: 2020 2022 2c20 706e 616d 7329 0a20 2020     ", pnams).   
+00026000: 2020 2020 2070 7269 6e74 2822 2070 6172       print(" par
+00026010: 616d 6574 6572 2076 616c 7565 733a 2020  ameter values:  
+00026020: 2020 2020 222c 2070 7661 6c73 290a 2020      ", pvals).  
+00026030: 2020 2020 2020 7072 696e 7428 2220 6e65        print(" ne
+00026040: 672e 2070 6172 616d 6574 6572 2065 7272  g. parameter err
+00026050: 6f72 733a 2022 2c20 7065 7272 735b 3a2c  ors: ", perrs[:,
+00026060: 2030 5d29 0a20 2020 2020 2020 2070 7269   0]).        pri
+00026070: 6e74 2822 2070 6f73 2e20 7061 7261 6d65  nt(" pos. parame
+00026080: 7465 7220 6572 726f 7273 3a20 222c 2070  ter errors: ", p
+00026090: 6572 7273 5b3a 2c20 315d 290a 2020 2020  errs[:, 1]).    
+000260a0: 2020 2020 7072 696e 7428 2220 636f 7272      print(" corr
+000260b0: 656c 6174 696f 6e73 203a 205c 6e22 2c20  elations : \n", 
+000260c0: 636f 7229 0a0a 2020 2020 6465 6620 6578  cor)..    def ex
+000260d0: 616d 706c 655f 756e 6269 6e6e 6564 4d4c  ample_unbinnedML
+000260e0: 4669 7428 293a 0a20 2020 2020 2020 2022  Fit():.        "
+000260f0: 2222 2a2a 756e 6269 6e6e 6564 204d 4c20  ""**unbinned ML 
+00026100: 6669 742a 2a20 6f66 2070 6466 2074 6f20  fit** of pdf to 
+00026110: 756e 6269 6e6e 6564 2064 6174 610a 0a20  unbinned data.. 
+00026120: 2020 2020 2020 2072 6561 6c20 6461 7461         real data
+00026130: 2066 726f 6d20 6d65 6173 7572 656d 656e   from measuremen
+00026140: 7420 7769 7468 2061 2057 6174 6572 2043  t with a Water C
+00026150: 6865 7265 6e6b 6f76 2064 6574 6563 746f  herenkov detecto
+00026160: 7220 2822 4b61 6d69 6f6b 616e 6e65 2229  r ("Kamiokanne")
+00026170: 0a0a 2020 2020 2020 2020 6e75 6d62 6572  ..        number
+00026180: 7320 7265 7072 6573 656e 7420 7469 6d65  s represent time
+00026190: 2064 6966 6665 7265 6e63 6573 2028 696e   differences (in
+000261a0: 20c2 b573 2920 6265 7477 6565 6e20 7468   ..s) between th
+000261b0: 6520 7061 7373 6167 6520 6f66 2061 206d  e passage of a m
+000261c0: 756f 6e0a 2020 2020 2020 2020 616e 6420  uon.        and 
+000261d0: 7468 6520 7265 6769 7374 7261 7469 6f6e  the registration
+000261e0: 206f 6620 6120 7365 636f 6e64 2070 756c   of a second pul
+000261f0: 7365 2c20 6f66 7465 6e20 6361 7573 6564  se, often caused
+00026200: 2062 7920 616e 2065 6c65 6374 726f 6e20   by an electron 
+00026210: 6672 6f6d 0a20 2020 2020 2020 2074 6865  from.        the
+00026220: 2064 6563 6179 206f 6620 7468 6520 7374   decay of the st
+00026230: 6f70 7065 6420 6d75 6f6e 2e20 4173 2073  opped muon. As s
+00026240: 7563 6820 6576 656e 7473 2061 7265 2072  uch events are r
+00026250: 6172 652c 2068 6973 746f 6772 616d 6d69  are, histogrammi
+00026260: 6e67 2074 6865 0a20 2020 2020 2020 2064  ng the.        d
+00026270: 6174 6120 7072 696f 7220 746f 2066 6974  ata prior to fit
+00026280: 7469 6e67 2077 6f75 6c64 2069 6e74 726f  ting would intro
+00026290: 6475 6365 2073 6869 6674 7320 616e 6420  duce shifts and 
+000262a0: 6269 6173 6573 2c20 616e 6420 7468 6572  biases, and ther
+000262b0: 6566 6f72 6520 7468 650a 2020 2020 2020  efore the.      
+000262c0: 2020 756e 6269 6e6e 6564 2066 6974 2069    unbinned fit i
+000262d0: 7320 7468 6520 6f70 7469 6d61 6c20 6d65  s the optimal me
+000262e0: 7468 6f64 2066 6f72 2074 6869 7320 616e  thod for this an
+000262f0: 6420 7369 6d75 6c61 7220 7573 6520 6361  d simular use ca
+00026300: 7365 732e 0a20 2020 2020 2020 2022 2222  ses..        """
+00026310: 0a20 2020 2020 2020 2064 5420 3d20 5b0a  .        dT = [.
+00026320: 2020 2020 2020 2020 2020 2020 372e 3432              7.42
+00026330: 2c0a 2020 2020 2020 2020 2020 2020 332e  ,.            3.
+00026340: 3737 332c 0a20 2020 2020 2020 2020 2020  773,.           
+00026350: 2035 2e39 3638 2c0a 2020 2020 2020 2020   5.968,.        
+00026360: 2020 2020 342e 3932 342c 0a20 2020 2020      4.924,.     
+00026370: 2020 2020 2020 2031 2e34 3638 2c0a 2020         1.468,.  
+00026380: 2020 2020 2020 2020 2020 342e 3636 342c            4.664,
+00026390: 0a20 2020 2020 2020 2020 2020 2031 2e37  .            1.7
+000263a0: 3435 2c0a 2020 2020 2020 2020 2020 2020  45,.            
+000263b0: 322e 3134 342c 0a20 2020 2020 2020 2020  2.144,.         
+000263c0: 2020 2033 2e38 3336 2c0a 2020 2020 2020     3.836,.      
+000263d0: 2020 2020 2020 332e 3133 322c 0a20 2020        3.132,.   
+000263e0: 2020 2020 2020 2020 2031 2e35 3638 2c0a           1.568,.
+000263f0: 2020 2020 2020 2020 2020 2020 322e 3335              2.35
+00026400: 322c 0a20 2020 2020 2020 2020 2020 2032  2,.            2
+00026410: 2e31 3332 2c0a 2020 2020 2020 2020 2020  .132,.          
+00026420: 2020 392e 3338 312c 0a20 2020 2020 2020    9.381,.       
+00026430: 2020 2020 2031 2e34 3834 2c0a 2020 2020       1.484,.    
+00026440: 2020 2020 2020 2020 312e 3138 312c 0a20          1.181,. 
+00026450: 2020 2020 2020 2020 2020 2035 2e30 3034             5.004
+00026460: 2c0a 2020 2020 2020 2020 2020 2020 332e  ,.            3.
+00026470: 3036 2c0a 2020 2020 2020 2020 2020 2020  06,.            
+00026480: 342e 3538 322c 0a20 2020 2020 2020 2020  4.582,.         
+00026490: 2020 2032 2e30 3736 2c0a 2020 2020 2020     2.076,.      
+000264a0: 2020 2020 2020 312e 3838 2c0a 2020 2020        1.88,.    
+000264b0: 2020 2020 2020 2020 312e 3333 372c 0a20          1.337,. 
+000264c0: 2020 2020 2020 2020 2020 2033 2e30 3932             3.092
+000264d0: 2c0a 2020 2020 2020 2020 2020 2020 322e  ,.            2.
+000264e0: 3236 352c 0a20 2020 2020 2020 2020 2020  265,.           
+000264f0: 2031 2e32 3038 2c0a 2020 2020 2020 2020   1.208,.        
+00026500: 2020 2020 322e 3735 332c 0a20 2020 2020      2.753,.     
+00026510: 2020 2020 2020 2034 2e34 3537 2c0a 2020         4.457,.  
+00026520: 2020 2020 2020 2020 2020 332e 3439 392c            3.499,
+00026530: 0a20 2020 2020 2020 2020 2020 2038 2e31  .            8.1
+00026540: 3932 2c0a 2020 2020 2020 2020 2020 2020  92,.            
+00026550: 352e 3130 312c 0a20 2020 2020 2020 2020  5.101,.         
+00026560: 2020 2031 2e35 3732 2c0a 2020 2020 2020     1.572,.      
+00026570: 2020 2020 2020 352e 3135 322c 0a20 2020        5.152,.   
+00026580: 2020 2020 2020 2020 2034 2e31 3831 2c0a           4.181,.
+00026590: 2020 2020 2020 2020 2020 2020 332e 3532              3.52
+000265a0: 2c0a 2020 2020 2020 2020 2020 2020 312e  ,.            1.
+000265b0: 3334 342c 0a20 2020 2020 2020 2020 2020  344,.           
+000265c0: 2031 302e 3239 2c0a 2020 2020 2020 2020   10.29,.        
+000265d0: 2020 2020 312e 3135 322c 0a20 2020 2020      1.152,.     
+000265e0: 2020 2020 2020 2032 2e33 3438 2c0a 2020         2.348,.  
+000265f0: 2020 2020 2020 2020 2020 322e 3232 382c            2.228,
+00026600: 0a20 2020 2020 2020 2020 2020 2032 2e31  .            2.1
+00026610: 3732 2c0a 2020 2020 2020 2020 2020 2020  72,.            
+00026620: 372e 3434 382c 0a20 2020 2020 2020 2020  7.448,.         
+00026630: 2020 2031 2e31 3038 2c0a 2020 2020 2020     1.108,.      
+00026640: 2020 2020 2020 342e 3334 342c 0a20 2020        4.344,.   
+00026650: 2020 2020 2020 2020 2032 2e30 3432 2c0a           2.042,.
+00026660: 2020 2020 2020 2020 2020 2020 352e 3038              5.08
+00026670: 382c 0a20 2020 2020 2020 2020 2020 2031  8,.            1
+00026680: 2e30 322c 0a20 2020 2020 2020 2020 2020  .02,.           
+00026690: 2031 2e30 3531 2c0a 2020 2020 2020 2020   1.051,.        
+000266a0: 2020 2020 312e 3938 372c 0a20 2020 2020      1.987,.     
+000266b0: 2020 2020 2020 2031 2e39 3335 2c0a 2020         1.935,.  
+000266c0: 2020 2020 2020 2020 2020 332e 3737 332c            3.773,
+000266d0: 0a20 2020 2020 2020 2020 2020 2034 2e30  .            4.0
+000266e0: 3932 2c0a 2020 2020 2020 2020 2020 2020  92,.            
+000266f0: 312e 3632 382c 0a20 2020 2020 2020 2020  1.628,.         
+00026700: 2020 2031 2e36 3838 2c0a 2020 2020 2020     1.688,.      
+00026710: 2020 2020 2020 342e 3530 322c 0a20 2020        4.502,.   
+00026720: 2020 2020 2020 2020 2034 2e36 3837 2c0a           4.687,.
+00026730: 2020 2020 2020 2020 2020 2020 362e 3735              6.75
+00026740: 352c 0a20 2020 2020 2020 2020 2020 2032  5,.            2
+00026750: 2e35 362c 0a20 2020 2020 2020 2020 2020  .56,.           
+00026760: 2031 2e32 3038 2c0a 2020 2020 2020 2020   1.208,.        
+00026770: 2020 2020 322e 3634 392c 0a20 2020 2020      2.649,.     
+00026780: 2020 2020 2020 2031 2e30 3132 2c0a 2020         1.012,.  
+00026790: 2020 2020 2020 2020 2020 312e 3733 2c0a            1.73,.
+000267a0: 2020 2020 2020 2020 2020 2020 322e 3136              2.16
+000267b0: 342c 0a20 2020 2020 2020 2020 2020 2031  4,.            1
+000267c0: 2e37 3238 2c0a 2020 2020 2020 2020 2020  .728,.          
+000267d0: 2020 342e 3634 362c 0a20 2020 2020 2020    4.646,.       
+000267e0: 2020 2020 2032 2e39 3136 2c0a 2020 2020       2.916,.    
+000267f0: 2020 2020 2020 2020 312e 3130 312c 0a20          1.101,. 
+00026800: 2020 2020 2020 2020 2020 2032 2e35 342c             2.54,
+00026810: 0a20 2020 2020 2020 2020 2020 2031 2e30  .            1.0
+00026820: 322c 0a20 2020 2020 2020 2020 2020 2031  2,.            1
+00026830: 2e31 3736 2c0a 2020 2020 2020 2020 2020  .176,.          
+00026840: 2020 342e 3731 362c 0a20 2020 2020 2020    4.716,.       
+00026850: 2020 2020 2039 2e36 3731 2c0a 2020 2020       9.671,.    
+00026860: 2020 2020 2020 2020 312e 3639 322c 0a20          1.692,. 
+00026870: 2020 2020 2020 2020 2020 2039 2e32 3932             9.292
+00026880: 2c0a 2020 2020 2020 2020 2020 2020 3130  ,.            10
+00026890: 2e37 322c 0a20 2020 2020 2020 2020 2020  .72,.           
+000268a0: 2032 2e31 3634 2c0a 2020 2020 2020 2020   2.164,.        
+000268b0: 2020 2020 322e 3038 342c 0a20 2020 2020      2.084,.     
+000268c0: 2020 2020 2020 2032 2e36 3136 2c0a 2020         2.616,.  
+000268d0: 2020 2020 2020 2020 2020 312e 3538 342c            1.584,
+000268e0: 0a20 2020 2020 2020 2020 2020 2035 2e32  .            5.2
+000268f0: 3336 2c0a 2020 2020 2020 2020 2020 2020  36,.            
+00026900: 332e 3636 332c 0a20 2020 2020 2020 2020  3.663,.         
+00026910: 2020 2033 2e36 3234 2c0a 2020 2020 2020     3.624,.      
+00026920: 2020 2020 2020 312e 3035 312c 0a20 2020        1.051,.   
+00026930: 2020 2020 2020 2020 2031 2e35 3434 2c0a           1.544,.
+00026940: 2020 2020 2020 2020 2020 2020 312e 3439              1.49
+00026950: 362c 0a20 2020 2020 2020 2020 2020 2031  6,.            1
+00026960: 2e38 3833 2c0a 2020 2020 2020 2020 2020  .883,.          
+00026970: 2020 312e 3932 2c0a 2020 2020 2020 2020    1.92,.        
+00026980: 2020 2020 352e 3936 382c 0a20 2020 2020      5.968,.     
+00026990: 2020 2020 2020 2035 2e38 392c 0a20 2020         5.89,.   
+000269a0: 2020 2020 2020 2020 2032 2e38 3936 2c0a           2.896,.
+000269b0: 2020 2020 2020 2020 2020 2020 322e 3736              2.76
+000269c0: 2c0a 2020 2020 2020 2020 2020 2020 312e  ,.            1.
+000269d0: 3437 352c 0a20 2020 2020 2020 2020 2020  475,.           
+000269e0: 2032 2e36 3434 2c0a 2020 2020 2020 2020   2.644,.        
+000269f0: 2020 2020 332e 362c 0a20 2020 2020 2020      3.6,.       
+00026a00: 2020 2020 2035 2e33 3234 2c0a 2020 2020       5.324,.    
+00026a10: 2020 2020 2020 2020 382e 3336 312c 0a20          8.361,. 
+00026a20: 2020 2020 2020 2020 2020 2033 2e30 3532             3.052
+00026a30: 2c0a 2020 2020 2020 2020 2020 2020 372e  ,.            7.
+00026a40: 3730 332c 0a20 2020 2020 2020 2020 2020  703,.           
+00026a50: 2033 2e38 332c 0a20 2020 2020 2020 2020   3.83,.         
+00026a60: 2020 2031 2e34 3434 2c0a 2020 2020 2020     1.444,.      
+00026a70: 2020 2020 2020 312e 3334 332c 0a20 2020        1.343,.   
+00026a80: 2020 2020 2020 2020 2034 2e37 3336 2c0a           4.736,.
+00026a90: 2020 2020 2020 2020 2020 2020 382e 372c              8.7,
+00026aa0: 0a20 2020 2020 2020 2020 2020 2036 2e31  .            6.1
+00026ab0: 3932 2c0a 2020 2020 2020 2020 2020 2020  92,.            
+00026ac0: 352e 3739 362c 0a20 2020 2020 2020 2020  5.796,.         
+00026ad0: 2020 2031 2e34 2c0a 2020 2020 2020 2020     1.4,.        
+00026ae0: 2020 2020 332e 3339 322c 0a20 2020 2020      3.392,.     
+00026af0: 2020 2020 2020 2037 2e38 3038 2c0a 2020         7.808,.  
+00026b00: 2020 2020 2020 2020 2020 362e 3334 342c            6.344,
+00026b10: 0a20 2020 2020 2020 2020 2020 2031 2e38  .            1.8
+00026b20: 3834 2c0a 2020 2020 2020 2020 2020 2020  84,.            
+00026b30: 322e 3333 322c 0a20 2020 2020 2020 2020  2.332,.         
+00026b40: 2020 2031 2e37 362c 0a20 2020 2020 2020     1.76,.       
+00026b50: 2020 2020 2034 2e33 3434 2c0a 2020 2020       4.344,.    
+00026b60: 2020 2020 2020 2020 322e 3938 382c 0a20          2.988,. 
+00026b70: 2020 2020 2020 2020 2020 2037 2e34 342c             7.44,
+00026b80: 0a20 2020 2020 2020 2020 2020 2035 2e38  .            5.8
+00026b90: 3034 2c0a 2020 2020 2020 2020 2020 2020  04,.            
+00026ba0: 392e 352c 0a20 2020 2020 2020 2020 2020  9.5,.           
+00026bb0: 2039 2e39 3034 2c0a 2020 2020 2020 2020   9.904,.        
+00026bc0: 2020 2020 332e 3139 362c 0a20 2020 2020      3.196,.     
+00026bd0: 2020 2020 2020 2033 2e30 3132 2c0a 2020         3.012,.  
+00026be0: 2020 2020 2020 2020 2020 362e 3035 362c            6.056,
+00026bf0: 0a20 2020 2020 2020 2020 2020 2036 2e33  .            6.3
+00026c00: 3238 2c0a 2020 2020 2020 2020 2020 2020  28,.            
+00026c10: 392e 3036 342c 0a20 2020 2020 2020 2020  9.064,.         
+00026c20: 2020 2033 2e30 3638 2c0a 2020 2020 2020     3.068,.      
+00026c30: 2020 2020 2020 392e 3335 322c 0a20 2020        9.352,.   
+00026c40: 2020 2020 2020 2020 2031 2e39 3336 2c0a           1.936,.
+00026c50: 2020 2020 2020 2020 2020 2020 312e 3038              1.08
+00026c60: 2c0a 2020 2020 2020 2020 2020 2020 312e  ,.            1.
+00026c70: 3938 342c 0a20 2020 2020 2020 2020 2020  984,.           
+00026c80: 2031 2e37 3932 2c0a 2020 2020 2020 2020   1.792,.        
+00026c90: 2020 2020 392e 3338 342c 0a20 2020 2020      9.384,.     
+00026ca0: 2020 2020 2020 2031 302e 3135 2c0a 2020         10.15,.  
+00026cb0: 2020 2020 2020 2020 2020 342e 3735 362c            4.756,
+00026cc0: 0a20 2020 2020 2020 2020 2020 2031 2e35  .            1.5
+00026cd0: 322c 0a20 2020 2020 2020 2020 2020 2033  2,.            3
+00026ce0: 2e39 3132 2c0a 2020 2020 2020 2020 2020  .912,.          
+00026cf0: 2020 312e 3731 322c 0a20 2020 2020 2020    1.712,.       
+00026d00: 2020 2020 2031 302e 3537 2c0a 2020 2020       10.57,.    
+00026d10: 2020 2020 2020 2020 352e 3330 342c 0a20          5.304,. 
+00026d20: 2020 2020 2020 2020 2020 2032 2e39 3638             2.968
+00026d30: 2c0a 2020 2020 2020 2020 2020 2020 392e  ,.            9.
+00026d40: 3633 322c 0a20 2020 2020 2020 2020 2020  632,.           
+00026d50: 2037 2e31 3136 2c0a 2020 2020 2020 2020   7.116,.        
+00026d60: 2020 2020 312e 3231 322c 0a20 2020 2020      1.212,.     
+00026d70: 2020 2020 2020 2038 2e35 3332 2c0a 2020         8.532,.  
+00026d80: 2020 2020 2020 2020 2020 332e 3030 302c            3.000,
+00026d90: 0a20 2020 2020 2020 2020 2020 2034 2e37  .            4.7
+00026da0: 3932 2c0a 2020 2020 2020 2020 2020 2020  92,.            
+00026db0: 322e 3531 322c 0a20 2020 2020 2020 2020  2.512,.         
+00026dc0: 2020 2031 2e33 3532 2c0a 2020 2020 2020     1.352,.      
+00026dd0: 2020 2020 2020 322e 3136 382c 0a20 2020        2.168,.   
+00026de0: 2020 2020 2020 2020 2034 2e33 3434 2c0a           4.344,.
+00026df0: 2020 2020 2020 2020 2020 2020 312e 3331              1.31
+00026e00: 362c 0a20 2020 2020 2020 2020 2020 2031  6,.            1
+00026e10: 2e34 3638 2c0a 2020 2020 2020 2020 2020  .468,.          
+00026e20: 2020 312e 3135 322c 0a20 2020 2020 2020    1.152,.       
+00026e30: 2020 2020 2036 2e30 3234 2c0a 2020 2020       6.024,.    
+00026e40: 2020 2020 2020 2020 332e 3237 322c 0a20          3.272,. 
+00026e50: 2020 2020 2020 2020 2020 2034 2e39 362c             4.96,
+00026e60: 0a20 2020 2020 2020 2020 2020 2031 302e  .            10.
+00026e70: 3136 2c0a 2020 2020 2020 2020 2020 2020  16,.            
+00026e80: 322e 3134 2c0a 2020 2020 2020 2020 2020  2.14,.          
+00026e90: 2020 322e 3835 362c 0a20 2020 2020 2020    2.856,.       
+00026ea0: 2020 2020 2031 302e 3031 2c0a 2020 2020       10.01,.    
+00026eb0: 2020 2020 2020 2020 312e 3233 322c 0a20          1.232,. 
+00026ec0: 2020 2020 2020 2020 2020 2032 2e36 3638             2.668
+00026ed0: 2c0a 2020 2020 2020 2020 2020 2020 392e  ,.            9.
+00026ee0: 3137 362c 0a20 2020 2020 2020 205d 0a0a  176,.        ]..
+00026ef0: 2020 2020 2020 2020 6465 6620 6578 706f          def expo
+00026f00: 6e65 6e74 6961 6c44 6563 6179 5044 4628  nentialDecayPDF(
+00026f10: 742c 2074 6175 3d32 2e30 2c20 6662 673d  t, tau=2.0, fbg=
+00026f20: 302e 322c 2061 3d31 2e30 2c20 623d 3131  0.2, a=1.0, b=11
+00026f30: 2e35 293a 0a20 2020 2020 2020 2020 2020  .5):.           
+00026f40: 2022 2222 5072 6f62 6162 696c 6974 7920   """Probability 
+00026f50: 6465 6e73 6974 7920 6675 6e63 7469 6f6e  density function
+00026f60: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00026f70: 7220 616e 2065 7870 6f6e 656e 7469 616c  r an exponential
+00026f80: 2064 6563 6179 2077 6974 6820 666c 6174   decay with flat
+00026f90: 2062 6163 6b67 726f 756e 642e 2054 6865   background. The
+00026fa0: 2070 6466 2069 7320 6e6f 726d 6564 2066   pdf is normed f
+00026fb0: 6f72 0a20 2020 2020 2020 2020 2020 2074  or.            t
+00026fc0: 6865 2069 6e74 6572 7661 6c20 5b61 3d31  he interval [a=1
+00026fd0: c2b5 732c 2020 623d 3131 2e35 c2b5 7329  ..s,  b=11.5..s)
+00026fe0: 3b20 7468 6573 6520 7061 7261 6d65 7465  ; these paramete
+00026ff0: 7273 2061 2061 6e64 2062 206d 7573 7420  rs a and b must 
+00027000: 6265 0a20 2020 2020 2020 2020 2020 2066  be.            f
+00027010: 6978 6564 2069 6e20 7468 6520 6669 7421  ixed in the fit!
+00027020: 0a0a 2020 2020 2020 2020 2020 2020 3a70  ..            :p
+00027030: 6172 616d 2074 3a20 6465 6361 7920 7469  aram t: decay ti
+00027040: 6d65 0a20 2020 2020 2020 2020 2020 203a  me.            :
+00027050: 7061 7261 6d20 6662 673a 2062 6163 6b67  param fbg: backg
+00027060: 726f 756e 640a 2020 2020 2020 2020 2020  round.          
+00027070: 2020 3a70 6172 616d 2074 6175 3a20 6578    :param tau: ex
+00027080: 7065 6374 6564 206d 6561 6e20 6f66 2074  pected mean of t
+00027090: 6865 2064 6563 6179 2074 696d 650a 2020  he decay time.  
+000270a0: 2020 2020 2020 2020 2020 3a70 6172 616d            :param
+000270b0: 2061 3a20 7468 6520 6d69 6e69 6d75 6d20   a: the minimum 
+000270c0: 6465 6361 7920 7469 6d65 2077 6869 6368  decay time which
+000270d0: 2063 616e 2062 6520 6d65 6173 7572 6564   can be measured
+000270e0: 0a20 2020 2020 2020 2020 2020 203a 7061  .            :pa
+000270f0: 7261 6d20 623a 2074 6865 206d 6178 696d  ram b: the maxim
+00027100: 756d 2064 6563 6179 2074 696d 6520 7768  um decay time wh
+00027110: 6963 6820 6361 6e20 6265 206d 6561 7375  ich can be measu
+00027120: 7265 640a 2020 2020 2020 2020 2020 2020  red.            
+00027130: 3a72 6574 7572 6e3a 2070 726f 6261 6269  :return: probabi
+00027140: 6c69 7479 2066 6f72 2064 6563 6179 2074  lity for decay t
+00027150: 696d 6520 780a 2020 2020 2020 2020 2020  ime x.          
+00027160: 2020 2222 220a 2020 2020 2020 2020 2020    """.          
+00027170: 2020 7064 6631 203d 206e 702e 6578 7028    pdf1 = np.exp(
+00027180: 2d74 202f 2074 6175 2920 2f20 7461 7520  -t / tau) / tau 
+00027190: 2f20 286e 702e 6578 7028 2d61 202f 2074  / (np.exp(-a / t
+000271a0: 6175 2920 2d20 6e70 2e65 7870 282d 6220  au) - np.exp(-b 
+000271b0: 2f20 7461 7529 290a 2020 2020 2020 2020  / tau)).        
+000271c0: 2020 2020 7064 6632 203d 2031 2e30 202f      pdf2 = 1.0 /
+000271d0: 2028 6220 2d20 6129 0a20 2020 2020 2020   (b - a).       
+000271e0: 2020 2020 2072 6574 7572 6e20 2831 202d       return (1 -
+000271f0: 2066 6267 2920 2a20 7064 6631 202b 2066   fbg) * pdf1 + f
+00027200: 6267 202a 2070 6466 320a 0a20 2020 2020  bg * pdf2..     
+00027210: 2020 2072 6573 756c 7444 6963 7420 3d20     resultDict = 
+00027220: 6d46 6974 280a 2020 2020 2020 2020 2020  mFit(.          
+00027230: 2020 6578 706f 6e65 6e74 6961 6c44 6563    exponentialDec
+00027240: 6179 5044 462c 0a20 2020 2020 2020 2020  ayPDF,.         
+00027250: 2020 2064 6174 613d 6454 2c20 2023 2064     data=dT,  # d
+00027260: 6174 6120 2d20 6966 206e 6f74 204e 6f6e  ata - if not Non
+00027270: 652c 2061 206e 6f72 6d61 6c69 7365 6420  e, a normalised 
+00027280: 5044 4620 6973 2061 7373 756d 6564 2061  PDF is assumed a
+00027290: 7320 6d6f 6465 6c0a 2020 2020 2020 2020  s model.        
+000272a0: 2020 2020 7030 3d4e 6f6e 652c 2020 2320      p0=None,  # 
+000272b0: 696e 6974 6961 6c20 6775 6573 7320 666f  initial guess fo
+000272c0: 7220 7061 7261 6d65 7465 7220 7661 6c75  r parameter valu
+000272d0: 6573 0a20 2020 2020 2020 2020 2020 2023  es.            #
+000272e0: 2020 636f 6e73 7472 6169 6e74 733d 5b5b    constraints=[[
+000272f0: 2774 6175 272c 2032 2e32 2c20 302e 3031  'tau', 2.2, 0.01
+00027300: 5d2c 2023 2047 6175 7373 6961 6e20 7061  ], # Gaussian pa
+00027310: 7261 6d65 7465 7220 636f 6e73 7472 6169  rameter constrai
+00027320: 6e74 730a 2020 2020 2020 2020 2020 2020  nts.            
+00027330: 6c69 6d69 7473 3d28 2266 6267 222c 2030  limits=("fbg", 0
+00027340: 2e30 2c20 312e 3029 2c20 2023 2070 6172  .0, 1.0),  # par
+00027350: 616d 6574 6572 206c 696d 6974 730a 2020  ameter limits.  
+00027360: 2020 2020 2020 2020 2020 6669 7850 6172            fixPar
+00027370: 733d 5b22 6122 2c20 2262 225d 2c20 2023  s=["a", "b"],  #
+00027380: 2066 6978 2070 6172 616d 6574 6572 2873   fix parameter(s
+00027390: 290a 2020 2020 2020 2020 2020 2020 6e65  ).            ne
+000273a0: 6732 6c6f 674c 3d54 7275 652c 2020 2320  g2logL=True,  # 
+000273b0: 7573 6520 202d 3220 2a20 6c6e 284c 290a  use  -2 * ln(L).
+000273c0: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
+000273d0: 3d54 7275 652c 2020 2320 706c 6f74 2064  =True,  # plot d
+000273e0: 6174 6120 616e 6420 6d6f 6465 6c0a 2020  ata and model.  
+000273f0: 2020 2020 2020 2020 2020 706c 6f74 5f62            plot_b
+00027400: 616e 643d 5472 7565 2c20 2023 2070 6c6f  and=True,  # plo
+00027410: 7420 6d6f 6465 6c20 636f 6e66 6964 656e  t model confiden
+00027420: 6365 2d62 616e 640a 2020 2020 2020 2020  ce-band.        
+00027430: 2020 2020 706c 6f74 5f63 6f72 3d46 616c      plot_cor=Fal
+00027440: 7365 2c20 2023 2070 6c6f 7420 7072 6f66  se,  # plot prof
+00027450: 696c 6573 206c 696b 656c 6968 6f6f 6420  iles likelihood 
+00027460: 616e 6420 636f 6e74 6f75 7273 0a20 2020  and contours.   
+00027470: 2020 2020 2020 2020 2073 686f 7770 6c6f           showplo
+00027480: 7473 3d46 616c 7365 2c20 2023 2073 686f  ts=False,  # sho
+00027490: 7720 2f20 646f 6e27 7420 7368 6f77 2070  w / don't show p
+000274a0: 6c6f 7473 0a20 2020 2020 2020 2020 2020  lots.           
+000274b0: 2071 7569 6574 3d46 616c 7365 2c20 2023   quiet=False,  #
+000274c0: 2073 7570 7072 6573 7320 696e 666f 726d   suppress inform
+000274d0: 6174 6976 6520 7072 696e 746f 7574 2069  ative printout i
+000274e0: 6620 5472 7565 0a20 2020 2020 2020 2020  f True.         
+000274f0: 2020 2061 7869 735f 6c61 6265 6c73 3d5b     axis_labels=[
+00027500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027510: 2022 6c69 6665 2074 696d 6520 2022 202b   "life time  " +
+00027520: 2022 245c 4465 6c74 6124 7420 2824 5c6d   "$\Delta$t ($\m
+00027530: 7524 7329 222c 0a20 2020 2020 2020 2020  u$s)",.         
+00027540: 2020 2020 2020 2022 5072 6f62 6162 696c         "Probabil
+00027550: 6974 7920 4465 6e73 6974 7920 2070 6466  ity Density  pdf
+00027560: 2824 5c44 656c 7461 2474 3b20 2a70 2922  ($\Delta$t; *p)"
+00027570: 2c0a 2020 2020 2020 2020 2020 2020 5d2c  ,.            ],
+00027580: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00027590: 615f 6c65 6765 6e64 3d22 245c 6d75 2420  a_legend="$\mu$ 
+000275a0: 6c69 6665 7469 6d65 2064 6174 6122 2c0a  lifetime data",.
+000275b0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+000275c0: 6c5f 6c65 6765 6e64 3d22 6578 706f 6e65  l_legend="expone
+000275d0: 6e74 6961 6c20 6465 6361 7920 2b20 666c  ntial decay + fl
+000275e0: 6174 2062 6163 6b67 726f 756e 6422 2c0a  at background",.
+000275f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00027600: 2020 2070 6c74 2e73 7570 7469 746c 6528     plt.suptitle(
+00027610: 0a20 2020 2020 2020 2020 2020 2022 556e  .            "Un
+00027620: 6269 6e6e 6564 204d 4c20 6669 7420 6f66  binned ML fit of
+00027630: 2061 6e20 6578 706f 6e65 6e74 6961 6c20   an exponential 
+00027640: 2b20 666c 6174 2064 6973 7472 6962 7574  + flat distribut
+00027650: 696f 6e22 2c0a 2020 2020 2020 2020 2020  ion",.          
+00027660: 2020 7369 7a65 3d22 7878 2d6c 6172 6765    size="xx-large
+00027670: 222c 0a20 2020 2020 2020 2020 2020 2063  ",.            c
+00027680: 6f6c 6f72 3d22 6461 726b 626c 7565 222c  olor="darkblue",
+00027690: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000276a0: 2020 2023 2050 7269 6e74 2072 6573 756c     # Print resul
+000276b0: 7473 0a20 2020 2020 2020 2070 7661 6c73  ts.        pvals
+000276c0: 2c20 7065 7272 732c 2063 6f72 2c20 676f  , perrs, cor, go
+000276d0: 662c 2070 6e61 6d73 203d 2072 6573 756c  f, pnams = resul
+000276e0: 7444 6963 742e 7661 6c75 6573 2829 0a20  tDict.values(). 
+000276f0: 2020 2020 2020 2070 7269 6e74 2822 5c6e         print("\n
+00027700: 2a3d 3d2a 2075 6e62 696e 6e65 6420 4d4c  *==* unbinned ML
+00027710: 2046 6974 2052 6573 756c 743a 2229 0a20   Fit Result:"). 
+00027720: 2020 2020 2020 2070 7269 6e74 2822 2070         print(" p
+00027730: 6172 616d 6574 6572 206e 616d 6573 3a20  arameter names: 
+00027740: 2020 2020 2020 222c 2070 6e61 6d73 290a        ", pnams).
+00027750: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+00027760: 7061 7261 6d65 7465 7220 7661 6c75 6573  parameter values
+00027770: 3a20 2020 2020 2022 2c20 7076 616c 7329  :      ", pvals)
+00027780: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00027790: 206e 6567 2e20 7061 7261 6d65 7465 7220   neg. parameter 
+000277a0: 6572 726f 7273 3a20 222c 2070 6572 7273  errors: ", perrs
+000277b0: 5b3a 2c20 305d 290a 2020 2020 2020 2020  [:, 0]).        
+000277c0: 7072 696e 7428 2220 706f 732e 2070 6172  print(" pos. par
+000277d0: 616d 6574 6572 2065 7272 6f72 733a 2022  ameter errors: "
+000277e0: 2c20 7065 7272 735b 3a2c 2031 5d29 0a20  , perrs[:, 1]). 
+000277f0: 2020 2020 2020 2070 7269 6e74 2822 2063         print(" c
+00027800: 6f72 7265 6c61 7469 6f6e 7320 3a20 5c6e  orrelations : \n
+00027810: 222c 2063 6f72 290a 0a20 2020 2023 0a20  ", cor)..    #. 
+00027820: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
 00027830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00027840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00027850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027860: 2d2d 2d2d 2d2d 2d0a 2020 2020 230a 2020  -------.    #.  
-00027870: 2020 2320 2d2d 2d20 7275 6e20 6162 6f76    # --- run abov
-00027880: 6520 6578 616d 706c 6573 0a0a 2020 2020  e examples..    
-00027890: 7072 696e 7428 222a 2a2a 2078 7920 6669  print("*** xy fi
-000278a0: 7420 6578 616d 706c 6522 290a 2020 2020  t example").    
-000278b0: 6578 616d 706c 655f 7879 4669 7428 290a  example_xyFit().
-000278c0: 0a20 2020 2070 7269 6e74 2822 2a2a 2a20  .    print("*** 
-000278d0: 696e 6465 7865 6420 6669 7420 6578 616d  indexed fit exam
-000278e0: 706c 6522 290a 2020 2020 6578 616d 706c  ple").    exampl
-000278f0: 655f 696e 6465 7865 6446 6974 2829 0a0a  e_indexedFit()..
-00027900: 2020 2020 7072 696e 7428 225c 6e5c 6e2a      print("\n\n*
-00027910: 2a2a 2068 6973 746f 6772 616d 2066 6974  ** histogram fit
-00027920: 2065 7861 6d70 6c65 2229 0a20 2020 2065   example").    e
-00027930: 7861 6d70 6c65 5f68 6973 746f 6772 616d  xample_histogram
-00027940: 4669 7428 290a 0a20 2020 2070 7269 6e74  Fit()..    print
-00027950: 2822 5c6e 5c6e 2a2a 2a20 6d69 6e75 6974  ("\n\n*** minuit
-00027960: 2066 6974 2077 6974 6820 6578 7465 726e   fit with extern
-00027970: 616c 2063 6f73 7420 6675 6e63 7469 6f6e  al cost function
-00027980: 2229 0a20 2020 2065 7861 6d70 6c65 5f75  ").    example_u
-00027990: 7365 7246 6974 2829 0a0a 2020 2020 7072  serFit()..    pr
-000279a0: 696e 7428 225c 6e5c 6e2a 2a2a 204d 4c20  int("\n\n*** ML 
-000279b0: 6d69 6e75 6974 2046 6974 2229 0a20 2020  minuit Fit").   
-000279c0: 2065 7861 6d70 6c65 5f75 6e62 696e 6e65   example_unbinne
-000279d0: 644d 4c46 6974 2829 0a0a 2020 2020 2320  dMLFit()..    # 
-000279e0: 7368 6f77 2061 6c6c 2066 6967 7572 6573  show all figures
-000279f0: 0a20 2020 2070 6c74 2e73 686f 7728 290a  .    plt.show().
+00027860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00027870: 2020 2023 0a20 2020 2023 202d 2d2d 2072     #.    # --- r
+00027880: 756e 2061 626f 7665 2065 7861 6d70 6c65  un above example
+00027890: 730a 0a20 2020 2070 7269 6e74 2822 2a2a  s..    print("**
+000278a0: 2a20 7879 2066 6974 2065 7861 6d70 6c65  * xy fit example
+000278b0: 2229 0a20 2020 2065 7861 6d70 6c65 5f78  ").    example_x
+000278c0: 7946 6974 2829 0a0a 2020 2020 7072 696e  yFit()..    prin
+000278d0: 7428 222a 2a2a 2069 6e64 6578 6564 2066  t("*** indexed f
+000278e0: 6974 2065 7861 6d70 6c65 2229 0a20 2020  it example").   
+000278f0: 2065 7861 6d70 6c65 5f69 6e64 6578 6564   example_indexed
+00027900: 4669 7428 290a 0a20 2020 2070 7269 6e74  Fit()..    print
+00027910: 2822 5c6e 5c6e 2a2a 2a20 6869 7374 6f67  ("\n\n*** histog
+00027920: 7261 6d20 6669 7420 6578 616d 706c 6522  ram fit example"
+00027930: 290a 2020 2020 6578 616d 706c 655f 6869  ).    example_hi
+00027940: 7374 6f67 7261 6d46 6974 2829 0a0a 2020  stogramFit()..  
+00027950: 2020 7072 696e 7428 225c 6e5c 6e2a 2a2a    print("\n\n***
+00027960: 206d 696e 7569 7420 6669 7420 7769 7468   minuit fit with
+00027970: 2065 7874 6572 6e61 6c20 636f 7374 2066   external cost f
+00027980: 756e 6374 696f 6e22 290a 2020 2020 6578  unction").    ex
+00027990: 616d 706c 655f 7573 6572 4669 7428 290a  ample_userFit().
+000279a0: 0a20 2020 2070 7269 6e74 2822 5c6e 5c6e  .    print("\n\n
+000279b0: 2a2a 2a20 4d4c 206d 696e 7569 7420 4669  *** ML minuit Fi
+000279c0: 7422 290a 2020 2020 6578 616d 706c 655f  t").    example_
+000279d0: 756e 6269 6e6e 6564 4d4c 4669 7428 290a  unbinnedMLFit().
+000279e0: 0a20 2020 2023 2073 686f 7720 616c 6c20  .    # show all 
+000279f0: 6669 6775 7265 730a 2020 2020 706c 742e  figures.    plt.
+00027a00: 7368 6f77 2829 0a                        show().
```

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit/phyTools.py` & `PhyPraKit-1.2.7/PhyPraKit/phyTools.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit/plotCSV.py` & `PhyPraKit-1.2.7/PhyPraKit/plotCSV.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit/plotData.py` & `PhyPraKit-1.2.7/PhyPraKit/plotData.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit/run_phyFit.py` & `PhyPraKit-1.2.7/PhyPraKit/run_phyFit.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit/smoothCSV.py` & `PhyPraKit-1.2.7/PhyPraKit/smoothCSV.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit.egg-info/PKG-INFO` & `PhyPraKit-1.2.7/PhyPraKit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PhyPraKit
-Version: 1.2.6rc1
+Version: 1.2.7
 Summary: Tools for data visualisation and analysis in Physics Lab Courses
 Home-page: http://www.etp.kit.edu/~quast/
 Author: Guenter Quast
 Author-email: Guenter.Quast@online.de
 License: GNU Public Licence
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `PhyPraKit-1.2.6rc1/PhyPraKit.egg-info/SOURCES.txt` & `PhyPraKit-1.2.7/PhyPraKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/README.md` & `PhyPraKit-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/setup.py` & `PhyPraKit-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test.py` & `PhyPraKit-1.2.7/tests/test.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/testAveCor_kafe1.py` & `PhyPraKit-1.2.7/tests/testAveCor_kafe1.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/testKafe2.py` & `PhyPraKit-1.2.7/tests/testKafe2.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_Diodenkennlinie.py` & `PhyPraKit-1.2.7/tests/test_Diodenkennlinie.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_histFit.py` & `PhyPraKit-1.2.7/tests/test_histFit.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_iminuit.py` & `PhyPraKit-1.2.7/tests/test_iminuit.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_iminuit2.py` & `PhyPraKit-1.2.7/tests/test_iminuit2.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_iminuitFit.py` & `PhyPraKit-1.2.7/tests/test_iminuitFit.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_iminuit_bak.py` & `PhyPraKit-1.2.7/tests/test_iminuit_bak.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_iminuit_old.py` & `PhyPraKit-1.2.7/tests/test_iminuit_old.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_k2Fit_2.py` & `PhyPraKit-1.2.7/tests/test_k2Fit_2.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_k2_hFit.py` & `PhyPraKit-1.2.7/tests/test_k2_hFit.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_kafe2.py` & `PhyPraKit-1.2.7/tests/test_kafe2.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_mFit2.py` & `PhyPraKit-1.2.7/tests/test_mFit2.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_mnFit.py` & `PhyPraKit-1.2.7/tests/test_mnFit.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tests/test_simplemFit.py` & `PhyPraKit-1.2.7/tests/test_simplemFit.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tools/plotCSV.py` & `PhyPraKit-1.2.7/tools/plotCSV.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tools/plotData.py` & `PhyPraKit-1.2.7/tools/plotData.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tools/run_phyFit.py` & `PhyPraKit-1.2.7/tools/run_phyFit.py`

 * *Files identical despite different names*

### Comparing `PhyPraKit-1.2.6rc1/tools/smoothCSV.py` & `PhyPraKit-1.2.7/tools/smoothCSV.py`

 * *Files identical despite different names*

