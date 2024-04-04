# Comparing `tmp/spaceweather-0.2.4.tar.gz` & `tmp/spaceweather-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceweather-0.2.4.tar", last modified: Wed Feb 14 16:18:54 2024, max compression
+gzip compressed data, was "spaceweather-0.3.0.tar", last modified: Thu Apr  4 17:19:24 2024, max compression
```

## Comparing `spaceweather-0.2.4.tar` & `spaceweather-0.3.0.tar`

### file list

```diff
@@ -1,47 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.493412 spaceweather-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-14 16:18:39.000000 spaceweather-0.2.4/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-14 16:18:39.000000 spaceweather-0.2.4/COPYING.GPLv2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-14 16:18:39.000000 spaceweather-0.2.4/COPYING.data
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-14 16:18:39.000000 spaceweather-0.2.4/COPYING.omni
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-14 16:18:39.000000 spaceweather-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-02-14 16:18:54.493412 spaceweather-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-02-14 16:18:39.000000 spaceweather-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.485412 spaceweather-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/COPYING.GPLv2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/COPYING.data
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/COPYING.omni
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/file_format.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/omni_format.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/omnie_format.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.485412 spaceweather-0.2.4/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-14 16:18:39.000000 spaceweather-0.2.4/docs/reference/spaceweather.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-14 16:18:54.493412 spaceweather-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-02-14 16:18:39.000000 spaceweather-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.481412 spaceweather-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.485412 spaceweather-0.2.4/src/spaceweather/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-14 16:18:39.000000 spaceweather-0.2.4/src/spaceweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-02-14 16:18:39.000000 spaceweather-0.2.4/src/spaceweather/celestrak.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-14 16:18:39.000000 spaceweather-0.2.4/src/spaceweather/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.489412 spaceweather-0.2.4/src/spaceweather/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:39.000000 spaceweather-0.2.4/src/spaceweather/data/.cache
--rw-r--r--   0 runner    (1001) docker     (127)  3046273 2024-02-14 16:18:39.000000 spaceweather-0.2.4/src/spaceweather/data/SW-All.txt
--rw-r--r--   0 runner    (1001) docker     (127)   281917 2024-02-14 16:18:39.000000 spaceweather-0.2.4/src/spaceweather/data/SW-Last5Years.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.489412 spaceweather-0.2.4/src/spaceweather/data/omni_extended/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:39.000000 spaceweather-0.2.4/src/spaceweather/data/omni_extended/.cache
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-02-14 16:18:39.000000 spaceweather-0.2.4/src/spaceweather/omni.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.493412 spaceweather-0.2.4/src/spaceweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-02-14 16:18:54.000000 spaceweather-0.2.4/src/spaceweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-14 16:18:54.000000 spaceweather-0.2.4/src/spaceweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 16:18:54.000000 spaceweather-0.2.4/src/spaceweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 16:18:54.000000 spaceweather-0.2.4/src/spaceweather.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-14 16:18:54.000000 spaceweather-0.2.4/src/spaceweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-14 16:18:54.000000 spaceweather-0.2.4/src/spaceweather.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 16:18:54.493412 spaceweather-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-02-14 16:18:39.000000 spaceweather-0.2.4/tests/omni2t_2000.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-02-14 16:18:39.000000 spaceweather-0.2.4/tests/test_omni.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-02-14 16:18:39.000000 spaceweather-0.2.4/tests/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.779957 spaceweather-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-04 17:19:12.000000 spaceweather-0.3.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-04-04 17:19:12.000000 spaceweather-0.3.0/COPYING.CCby4.0
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-04 17:19:12.000000 spaceweather-0.3.0/COPYING.GPLv2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-04 17:19:12.000000 spaceweather-0.3.0/COPYING.data
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-04 17:19:12.000000 spaceweather-0.3.0/COPYING.gfz
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-04 17:19:12.000000 spaceweather-0.3.0/COPYING.omni
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-04 17:19:12.000000 spaceweather-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-04-04 17:19:24.779957 spaceweather-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-04 17:19:12.000000 spaceweather-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.767957 spaceweather-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    18657 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/COPYING.CCby4.0
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/COPYING.GPLv2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/COPYING.data
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/COPYING.gfz
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/COPYING.omni
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/file_format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/gfz_Kp_ap_Ap_SN_F107_format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/gfz_wdc_fmt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17696 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/omni_format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/omnie_format.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.767957 spaceweather-0.3.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-04 17:19:12.000000 spaceweather-0.3.0/docs/reference/spaceweather.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 17:19:24.779957 spaceweather-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-04 17:19:12.000000 spaceweather-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.763957 spaceweather-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.771957 spaceweather-0.3.0/src/spaceweather/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/celestrak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.775957 spaceweather-0.3.0/src/spaceweather/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/data/.cache
+-rw-r--r--   0 runner    (1001) docker     (127)  3046273 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/data/SW-All.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   287989 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/data/SW-Last5Years.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.775957 spaceweather-0.3.0/src/spaceweather/data/omni_extended/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/data/omni_extended/.cache
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/gfz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-04-04 17:19:12.000000 spaceweather-0.3.0/src/spaceweather/omni.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.779957 spaceweather-0.3.0/src/spaceweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11442 2024-04-04 17:19:24.000000 spaceweather-0.3.0/src/spaceweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-04 17:19:24.000000 spaceweather-0.3.0/src/spaceweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:19:24.000000 spaceweather-0.3.0/src/spaceweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:19:24.000000 spaceweather-0.3.0/src/spaceweather.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 17:19:24.000000 spaceweather-0.3.0/src/spaceweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-04 17:19:24.000000 spaceweather-0.3.0/src/spaceweather.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:19:24.775957 spaceweather-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-04-04 17:19:12.000000 spaceweather-0.3.0/tests/Kp_ap_Ap_SN_F107_nowcast.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-04 17:19:12.000000 spaceweather-0.3.0/tests/Kp_ap_Ap_SN_F107_since_2024.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-04 17:19:12.000000 spaceweather-0.3.0/tests/omni2t_2000.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-04 17:19:12.000000 spaceweather-0.3.0/tests/test_gfz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-04 17:19:12.000000 spaceweather-0.3.0/tests/test_omni.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-04 17:19:12.000000 spaceweather-0.3.0/tests/test_read.py
```

### Comparing `spaceweather-0.2.4/CHANGES.md` & `spaceweather-0.3.0/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,27 @@
 Changelog
 =========
 
+v0.3.0 (2024-04-04)
+-------------------
+
+### New
+
+- Supports space weather index data from GFZ Potsdam
+  https://kp.gfz-potsdam.de/en/
+
+### Fixes
+
+- Fixes downloading OMNI2 on Windows (https://github.com/st-bender/pyspaceweather/issues/2)
+
+### Changes
+
+- Updates space weather indices from celestrak (observed until 2024-04-01)
+
+
 v0.2.4 (2024-02-14)
 -------------------
 
 ### Changes
 
 - Updates space weather indices from celestrak (observed until 2024-02-13)
 - CI updates
```

### Comparing `spaceweather-0.2.4/COPYING.GPLv2` & `spaceweather-0.3.0/COPYING.GPLv2`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/COPYING.data` & `spaceweather-0.3.0/COPYING.data`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/COPYING.omni` & `spaceweather-0.3.0/COPYING.omni`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/PKG-INFO` & `spaceweather-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,24 @@
-Metadata-Version: 2.1
-Name: spaceweather
-Version: 0.2.4
-Summary: Python interface for space weather indices
-Home-page: https://github.com/st-bender/pyspaceweather
-Author: Stefan Bender
-Author-email: stefan.bender@ntnu.no
-License: GPLv2
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: COPYING.GPLv2
-License-File: COPYING.data
-License-File: COPYING.omni
-Requires-Dist: numpy>=1.13.0
-Requires-Dist: pandas
-Requires-Dist: requests
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
-Requires-Dist: pytest-mock; extra == "tests"
-Provides-Extra: all
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: pytest-mock; extra == "all"
-
 # PySpaceWeather
 
 **Python interface for space weather indices**
 
 [![builds](https://github.com/st-bender/pyspaceweather/actions/workflows/ci_build_and_test.yml/badge.svg?branch=master)](https://github.com/st-bender/pyspaceweather/actions/workflows/ci_build_and_test.yml)
 [![docs](https://readthedocs.org/projects/pyspaceweather/badge/?version=latest)](https://pyspaceweather.readthedocs.io/en/latest/?badge=latest)
 [![package](https://img.shields.io/pypi/v/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![wheel](https://img.shields.io/pypi/wheel/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![pyversions](https://img.shields.io/pypi/pyversions/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![codecov](https://codecov.io/gh/st-bender/pyspaceweather/badge.svg)](https://codecov.io/gh/st-bender/pyspaceweather)
 [![coveralls](https://coveralls.io/repos/github/st-bender/pyspaceweather/badge.svg)](https://coveralls.io/github/st-bender/pyspaceweather)
 [![scrutinizer](https://scrutinizer-ci.com/g/st-bender/pyspaceweather/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/st-bender/pyspaceweather/?branch=master)
 
 This python module interfaces the space weather data available at
-<https://celestrak.com/SpaceData/> and <https://omniweb.gsfc.nasa.gov/ow.html>.
+<https://celestrak.com/SpaceData/>,
+<https://kp.gfz-potsdam.de/en/data>,
+and <https://omniweb.gsfc.nasa.gov/ow.html>.
 It includes the geomagnetic Ap and Kp indices, both the 3h values and
 the daily sum/averages.
 The data also include the solar f10.7 cm radio fluxes,
 the observed values as well as the 1 AU adjusted values,
 daily values and the 81-day running means.
 See [Data sources](#data-sources) below.
 
@@ -154,14 +125,51 @@
 2000-01-01 13:30:00  32  4.3
 2000-01-01 16:30:00  15  3.0
 2000-01-01 19:30:00  32  4.3
 2000-01-01 22:30:00  22  3.7
 
 ```
 
+### GFZ
+
+The "GFZ" module supports the ascii and WDC files as offered by the
+[GFZ German Research Centre for Geosciences](https://www.gfz-potsdam.de/en/)
+on their [data page](https://kp.gfz-potsdam.de/en/data).
+In contrast to the official python client, this module reads the data
+from the (downloaded) files and does not access the web service API.
+The interface is mostly the same as for the "Celestrak" data:
+
+```python
+>>> import spaceweather as sw
+>>> df_d = sw.gfz_daily()
+>>> df_d.loc["2000-01-01"].Apavg
+30.0
+>>> df_3h = sw.gfz_3h()
+>>> df_3h.loc["2000-01-01 01:30:00"]
+Ap    56.000
+Kp     5.333
+Name: 2000-01-01 01:30:00, dtype: float64
+
+```
+
+Currently, the data are not included in the package, downloads can be triggered
+by passing `update=True` to `sw.gfz_daily()` or by running `sw.update_gfz()`.
+The lower-level interface functions are called `read_gfz(<filename>)`
+for the ascii `.txt` files, and `read_gfz_wdc(<filename>)` for the WDC format.
+They can also be used directly for reading already downloaded data files
+outside of the package's data directory.
+
+```python
+>>> import spaceweather as sw
+>>> df_d = sw.read_gfz("./tests/Kp_ap_Ap_SN_F107_since_2024.txt")
+>>> df_d.loc["2024-01-01"].Apavg
+10.0
+
+```
+
 ### OMNI
 
 The [OMNI](https://omniweb.gsfc.nasa.gov/ow.html) 1-hour yearly data
 are accessible via `omnie_hourly(<year>)` or `read_omnie(<file>)`.
 Both functions should work with the OMNI2 standard and extended text files.
 If the data are not already available locally, they can be cached by passing
 `cache=True` to that function or by calling `cache_omnie(<year>)` explicitly.
@@ -196,14 +204,15 @@
 ### Reference
 
 Basic class and method documentation is accessible via `pydoc`:
 
 ```sh
 $ pydoc spaceweather
 $ pydoc spaceweather.celestrak
+$ pydoc spaceweather.gfz
 $ pydoc spaceweather.omni
 ```
 
 ## License
 
 This python interface is free software: you can redistribute it or modify
 it under the terms of the GNU General Public License as published by
@@ -219,14 +228,30 @@
 [celestrak](https://celestrak.com),
 for details see the included [COPYING.data](COPYING.data) file.
 
 The data sources and file format are described at
 <http://celestrak.com/SpaceData/SpaceWx-format.php>
 (see [file_format.txt](file_format.txt) for a local copy of the format description).
 
+### GFZ
+
+The "GFZ" data are provided as tabulated ascii files
+([format description](https://kp.gfz-potsdam.de/app/format/Kp_ap_Ap_SN_F107_format.txt),
+[local copy](gfz_Kp_ap_Ap_SN_F107_format.txt))
+and in [WDC format](https://kp.gfz-potsdam.de/app/format/wdc_fmt.txt)
+([local copy](gfz_wdc_fmt.txt))
+by the
+[GFZ German Research Centre for Geosciences](https://www.gfz-potsdam.de/en/)
+on their official [data webpage](https://kp.gfz-potsdam.de/en/data).
+The data have the doi: [10.5880/Kp.0001](https://doi.org/10.5880/Kp.0001),
+and they are provided under the "Creative Commons attribution license"
+[CC-by 4.0](https://creativecommons.org/licenses/by/4.0/)
+(local copy [COPYING.CCby4.0](COPYING.CCby4.0)).
+See also [COPYING.gfz](COPYING.gfz) for details.
+
 ### OMNI
 
 This package includes part of the hourly-resolved OMNI data,
 accessible through <https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/>,
 and it enables easy downloading of it.
 The file format is described at
 <https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/omni2.text>
```

### Comparing `spaceweather-0.2.4/README.md` & `spaceweather-0.3.0/docs/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 [![wheel](https://img.shields.io/pypi/wheel/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![pyversions](https://img.shields.io/pypi/pyversions/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![codecov](https://codecov.io/gh/st-bender/pyspaceweather/badge.svg)](https://codecov.io/gh/st-bender/pyspaceweather)
 [![coveralls](https://coveralls.io/repos/github/st-bender/pyspaceweather/badge.svg)](https://coveralls.io/github/st-bender/pyspaceweather)
 [![scrutinizer](https://scrutinizer-ci.com/g/st-bender/pyspaceweather/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/st-bender/pyspaceweather/?branch=master)
 
 This python module interfaces the space weather data available at
-<https://celestrak.com/SpaceData/> and <https://omniweb.gsfc.nasa.gov/ow.html>.
+<https://celestrak.com/SpaceData/>,
+<https://kp.gfz-potsdam.de/en/data>,
+and <https://omniweb.gsfc.nasa.gov/ow.html>.
 It includes the geomagnetic Ap and Kp indices, both the 3h values and
 the daily sum/averages.
 The data also include the solar f10.7 cm radio fluxes,
 the observed values as well as the 1 AU adjusted values,
 daily values and the 81-day running means.
 See [Data sources](#data-sources) below.
 
@@ -123,14 +125,51 @@
 2000-01-01 13:30:00  32  4.3
 2000-01-01 16:30:00  15  3.0
 2000-01-01 19:30:00  32  4.3
 2000-01-01 22:30:00  22  3.7
 
 ```
 
+### GFZ
+
+The "GFZ" module supports the ascii and WDC files as offered by the
+[GFZ German Research Centre for Geosciences](https://www.gfz-potsdam.de/en/)
+on their [data page](https://kp.gfz-potsdam.de/en/data).
+In contrast to the official python client, this module reads the data
+from the (downloaded) files and does not access the web service API.
+The interface is mostly the same as for the "Celestrak" data:
+
+```python
+>>> import spaceweather as sw
+>>> df_d = sw.gfz_daily()
+>>> df_d.loc["2000-01-01"].Apavg
+30.0
+>>> df_3h = sw.gfz_3h()
+>>> df_3h.loc["2000-01-01 01:30:00"]
+Ap    56.000
+Kp     5.333
+Name: 2000-01-01 01:30:00, dtype: float64
+
+```
+
+Currently, the data are not included in the package, downloads can be triggered
+by passing `update=True` to `sw.gfz_daily()` or by running `sw.update_gfz()`.
+The lower-level interface functions are called `read_gfz(<filename>)`
+for the ascii `.txt` files, and `read_gfz_wdc(<filename>)` for the WDC format.
+They can also be used directly for reading already downloaded data files
+outside of the package's data directory.
+
+```python
+>>> import spaceweather as sw
+>>> df_d = sw.read_gfz("./tests/Kp_ap_Ap_SN_F107_since_2024.txt")
+>>> df_d.loc["2024-01-01"].Apavg
+10.0
+
+```
+
 ### OMNI
 
 The [OMNI](https://omniweb.gsfc.nasa.gov/ow.html) 1-hour yearly data
 are accessible via `omnie_hourly(<year>)` or `read_omnie(<file>)`.
 Both functions should work with the OMNI2 standard and extended text files.
 If the data are not already available locally, they can be cached by passing
 `cache=True` to that function or by calling `cache_omnie(<year>)` explicitly.
@@ -165,14 +204,15 @@
 ### Reference
 
 Basic class and method documentation is accessible via `pydoc`:
 
 ```sh
 $ pydoc spaceweather
 $ pydoc spaceweather.celestrak
+$ pydoc spaceweather.gfz
 $ pydoc spaceweather.omni
 ```
 
 ## License
 
 This python interface is free software: you can redistribute it or modify
 it under the terms of the GNU General Public License as published by
@@ -188,14 +228,30 @@
 [celestrak](https://celestrak.com),
 for details see the included [COPYING.data](COPYING.data) file.
 
 The data sources and file format are described at
 <http://celestrak.com/SpaceData/SpaceWx-format.php>
 (see [file_format.txt](file_format.txt) for a local copy of the format description).
 
+### GFZ
+
+The "GFZ" data are provided as tabulated ascii files
+([format description](https://kp.gfz-potsdam.de/app/format/Kp_ap_Ap_SN_F107_format.txt),
+[local copy](gfz_Kp_ap_Ap_SN_F107_format.txt))
+and in [WDC format](https://kp.gfz-potsdam.de/app/format/wdc_fmt.txt)
+([local copy](gfz_wdc_fmt.txt))
+by the
+[GFZ German Research Centre for Geosciences](https://www.gfz-potsdam.de/en/)
+on their official [data webpage](https://kp.gfz-potsdam.de/en/data).
+The data have the doi: [10.5880/Kp.0001](https://doi.org/10.5880/Kp.0001),
+and they are provided under the "Creative Commons attribution license"
+[CC-by 4.0](https://creativecommons.org/licenses/by/4.0/)
+(local copy [COPYING.CCby4.0](COPYING.CCby4.0)).
+See also [COPYING.gfz](COPYING.gfz) for details.
+
 ### OMNI
 
 This package includes part of the hourly-resolved OMNI data,
 accessible through <https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/>,
 and it enables easy downloading of it.
 The file format is described at
 <https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/omni2.text>
```

### Comparing `spaceweather-0.2.4/docs/COPYING.GPLv2` & `spaceweather-0.3.0/docs/COPYING.GPLv2`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/docs/COPYING.data` & `spaceweather-0.3.0/docs/COPYING.data`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/docs/COPYING.omni` & `spaceweather-0.3.0/docs/COPYING.omni`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/docs/Makefile` & `spaceweather-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/docs/README.md` & `spaceweather-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,57 @@
+Metadata-Version: 2.1
+Name: spaceweather
+Version: 0.3.0
+Summary: Python interface for space weather indices
+Home-page: https://github.com/st-bender/pyspaceweather
+Author: Stefan Bender
+Author-email: stefan.bender@ntnu.no
+License: GPLv2
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: COPYING.CCby4.0
+License-File: COPYING.GPLv2
+License-File: COPYING.data
+License-File: COPYING.gfz
+License-File: COPYING.omni
+Requires-Dist: numpy>=1.13.0
+Requires-Dist: pandas
+Requires-Dist: requests
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-mock; extra == "tests"
+Provides-Extra: all
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: pytest-mock; extra == "all"
+
 # PySpaceWeather
 
 **Python interface for space weather indices**
 
 [![builds](https://github.com/st-bender/pyspaceweather/actions/workflows/ci_build_and_test.yml/badge.svg?branch=master)](https://github.com/st-bender/pyspaceweather/actions/workflows/ci_build_and_test.yml)
 [![docs](https://readthedocs.org/projects/pyspaceweather/badge/?version=latest)](https://pyspaceweather.readthedocs.io/en/latest/?badge=latest)
 [![package](https://img.shields.io/pypi/v/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![wheel](https://img.shields.io/pypi/wheel/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![pyversions](https://img.shields.io/pypi/pyversions/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![codecov](https://codecov.io/gh/st-bender/pyspaceweather/badge.svg)](https://codecov.io/gh/st-bender/pyspaceweather)
 [![coveralls](https://coveralls.io/repos/github/st-bender/pyspaceweather/badge.svg)](https://coveralls.io/github/st-bender/pyspaceweather)
 [![scrutinizer](https://scrutinizer-ci.com/g/st-bender/pyspaceweather/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/st-bender/pyspaceweather/?branch=master)
 
 This python module interfaces the space weather data available at
-<https://celestrak.com/SpaceData/> and <https://omniweb.gsfc.nasa.gov/ow.html>.
+<https://celestrak.com/SpaceData/>,
+<https://kp.gfz-potsdam.de/en/data>,
+and <https://omniweb.gsfc.nasa.gov/ow.html>.
 It includes the geomagnetic Ap and Kp indices, both the 3h values and
 the daily sum/averages.
 The data also include the solar f10.7 cm radio fluxes,
 the observed values as well as the 1 AU adjusted values,
 daily values and the 81-day running means.
 See [Data sources](#data-sources) below.
 
@@ -123,14 +158,51 @@
 2000-01-01 13:30:00  32  4.3
 2000-01-01 16:30:00  15  3.0
 2000-01-01 19:30:00  32  4.3
 2000-01-01 22:30:00  22  3.7
 
 ```
 
+### GFZ
+
+The "GFZ" module supports the ascii and WDC files as offered by the
+[GFZ German Research Centre for Geosciences](https://www.gfz-potsdam.de/en/)
+on their [data page](https://kp.gfz-potsdam.de/en/data).
+In contrast to the official python client, this module reads the data
+from the (downloaded) files and does not access the web service API.
+The interface is mostly the same as for the "Celestrak" data:
+
+```python
+>>> import spaceweather as sw
+>>> df_d = sw.gfz_daily()
+>>> df_d.loc["2000-01-01"].Apavg
+30.0
+>>> df_3h = sw.gfz_3h()
+>>> df_3h.loc["2000-01-01 01:30:00"]
+Ap    56.000
+Kp     5.333
+Name: 2000-01-01 01:30:00, dtype: float64
+
+```
+
+Currently, the data are not included in the package, downloads can be triggered
+by passing `update=True` to `sw.gfz_daily()` or by running `sw.update_gfz()`.
+The lower-level interface functions are called `read_gfz(<filename>)`
+for the ascii `.txt` files, and `read_gfz_wdc(<filename>)` for the WDC format.
+They can also be used directly for reading already downloaded data files
+outside of the package's data directory.
+
+```python
+>>> import spaceweather as sw
+>>> df_d = sw.read_gfz("./tests/Kp_ap_Ap_SN_F107_since_2024.txt")
+>>> df_d.loc["2024-01-01"].Apavg
+10.0
+
+```
+
 ### OMNI
 
 The [OMNI](https://omniweb.gsfc.nasa.gov/ow.html) 1-hour yearly data
 are accessible via `omnie_hourly(<year>)` or `read_omnie(<file>)`.
 Both functions should work with the OMNI2 standard and extended text files.
 If the data are not already available locally, they can be cached by passing
 `cache=True` to that function or by calling `cache_omnie(<year>)` explicitly.
@@ -165,14 +237,15 @@
 ### Reference
 
 Basic class and method documentation is accessible via `pydoc`:
 
 ```sh
 $ pydoc spaceweather
 $ pydoc spaceweather.celestrak
+$ pydoc spaceweather.gfz
 $ pydoc spaceweather.omni
 ```
 
 ## License
 
 This python interface is free software: you can redistribute it or modify
 it under the terms of the GNU General Public License as published by
@@ -188,14 +261,30 @@
 [celestrak](https://celestrak.com),
 for details see the included [COPYING.data](COPYING.data) file.
 
 The data sources and file format are described at
 <http://celestrak.com/SpaceData/SpaceWx-format.php>
 (see [file_format.txt](file_format.txt) for a local copy of the format description).
 
+### GFZ
+
+The "GFZ" data are provided as tabulated ascii files
+([format description](https://kp.gfz-potsdam.de/app/format/Kp_ap_Ap_SN_F107_format.txt),
+[local copy](gfz_Kp_ap_Ap_SN_F107_format.txt))
+and in [WDC format](https://kp.gfz-potsdam.de/app/format/wdc_fmt.txt)
+([local copy](gfz_wdc_fmt.txt))
+by the
+[GFZ German Research Centre for Geosciences](https://www.gfz-potsdam.de/en/)
+on their official [data webpage](https://kp.gfz-potsdam.de/en/data).
+The data have the doi: [10.5880/Kp.0001](https://doi.org/10.5880/Kp.0001),
+and they are provided under the "Creative Commons attribution license"
+[CC-by 4.0](https://creativecommons.org/licenses/by/4.0/)
+(local copy [COPYING.CCby4.0](COPYING.CCby4.0)).
+See also [COPYING.gfz](COPYING.gfz) for details.
+
 ### OMNI
 
 This package includes part of the hourly-resolved OMNI data,
 accessible through <https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/>,
 and it enables easy downloading of it.
 The file format is described at
 <https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/omni2.text>
```

### Comparing `spaceweather-0.2.4/docs/conf.py` & `spaceweather-0.3.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 if getenv('SPELLCHECK'):
     extensions += 'sphinxcontrib.spelling',
     spelling_show_suggestions = True
     spelling_lang = 'en_GB'
 
 master_doc = 'index'
 
-language = None
+language = "en"
 
 htmlhelp_basename = 'pyspaceweatherdoc'
 
 # autodoc_docstring_signature = False
 # autodoc_dumb_docstring = True
 autosummary_generate = True
 
@@ -66,14 +66,16 @@
 #  dir menu entry, description, category)
 texinfo_documents = [
     (master_doc, 'pyspaceweather', u'pyspaceweather Documentation',
      author, 'pyspaceweather', 'Space weather indices for python.',
      'Miscellaneous'),
 ]
 
+napoleon_use_admonition_for_notes = True
+
 html_theme = "sphinx_rtd_theme"
 
 # on_rtd is whether we are on readthedocs.org
 on_rtd = getenv("READTHEDOCS", None) == "True"
 if not on_rtd:
     import sphinx_rtd_theme
     html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
@@ -92,15 +94,16 @@
 html_context = dict(
     display_github=True,
     github_user="st-bender",
     github_repo="pyspaceweather",
     github_version="master",
     conf_py_path="/docs/",
 )
-html_static_path = ["_static"]
+html_extra_path = ["."]
+exclude_patterns = ["Makefile", "conf*"]
 # Switch to old behavior with html4, for a good display of references,
 # as described in https://github.com/sphinx-doc/sphinx/issues/6705
 # html4_writer = True
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 # Example configuration for intersphinx: refer to the Python standard library.
```

### Comparing `spaceweather-0.2.4/docs/file_format.txt` & `spaceweather-0.3.0/docs/file_format.txt`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/docs/index.rst` & `spaceweather-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/docs/omni_format.txt` & `spaceweather-0.3.0/docs/omni_format.txt`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/docs/omnie_format.txt` & `spaceweather-0.3.0/docs/omnie_format.txt`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/docs/reference/spaceweather.rst` & `spaceweather-0.3.0/docs/reference/spaceweather.rst`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,24 @@
 .. currentmodule:: spaceweather
 
 .. automodule:: spaceweather.celestrak
    :members:
    :undoc-members:
    :show-inheritance:
 
+spaceweather.gfz
+----------------
+
+.. currentmodule:: spaceweather
+
+.. automodule:: spaceweather.gfz
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 spaceweather.omni
 -----------------
 
 .. automodule:: spaceweather.omni
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `spaceweather-0.2.4/setup.py` & `spaceweather-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/src/spaceweather/celestrak.py` & `spaceweather-0.3.0/src/spaceweather/celestrak.py`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/src/spaceweather/core.py` & `spaceweather-0.3.0/src/spaceweather/core.py`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/src/spaceweather/data/SW-All.txt` & `spaceweather-0.3.0/src/spaceweather/data/SW-All.txt`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/src/spaceweather/data/SW-Last5Years.txt` & `spaceweather-0.3.0/src/spaceweather/data/SW-Last5Years.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 DATATYPE CssiSpaceWeather
 VERSION 1.2
-UPDATED 2024 Feb 14 15:31:33 UTC
+UPDATED 2024 Apr 02 18:31:47 UTC
 # --------------------------------------------------------------------------------------------------------------------------------
 #                              SPACE WEATHER DATA
 # --------------------------------------------------------------------------------------------------------------------------------
 #
 # See http://celestrak.com/SpaceData/SpaceWx-format.asp for format details.
 #
 # FORMAT(I4,I3,I3,I5,I3,8I3,I4,8I4,I4,F4.1,I2,I4,F6.1,I2,5F6.1)
 # --------------------------------------------------------------------------------------------------------------------------------
 #                                                                                             Adj     Adj   Adj   Obs   Obs   Obs 
 # yy mm dd BSRN ND Kp Kp Kp Kp Kp Kp Kp Kp Sum Ap  Ap  Ap  Ap  Ap  Ap  Ap  Ap  Avg Cp C9 ISN F10.7 Q Ctr81 Lst81 F10.7 Ctr81 Lst81
 # --------------------------------------------------------------------------------------------------------------------------------
 #
-NUM_OBSERVED_POINTS 1870
+NUM_OBSERVED_POINTS 1918
 BEGIN OBSERVED
 2019 01 01 2529  8 10 13 27 17 20  3  0  7  97   4   5  12   6   7   2   0   3   5 0.2 1  12  69.5 0  68.4  68.0  71.9  70.5  69.6
 2019 01 02 2529  9  0  0  0  0  3  3  0  0   7   0   0   0   0   2   2   0   0   0 0.0 0  15  72.7 0  68.4  68.0  75.2  70.5  69.6
 2019 01 03 2529 10 10  0  0  3  3  0  0  3  20   4   0   0   2   2   0   0   2   1 0.0 0  15  70.2 0  68.4  68.0  72.6  70.6  69.6
 2019 01 04 2529 11 13  3 10 17 20 30 27 33 153   5   2   4   6   7  15  12  18   9 0.5 2  13  69.1 0  68.4  68.0  71.5  70.6  69.6
 2019 01 05 2529 12 50 40 23 23 17 23 20 30 227  48  27   9   9   6   9   7  15  16 0.9 4  11  68.8 0  68.4  68.0  71.1  70.6  69.7
 2019 01 06 2529 13 17 27 23 17 20 27 30 20 180   6  12   9   6   7  12  15   7   9 0.5 2   0  69.6 0  68.5  68.0  72.0  70.6  69.7
@@ -1841,190 +1841,236 @@
 2023 12 29 2596 22 13 10 13 20 17  7 17 23 120   5   4   5   7   6   3   6   9   6 0.3 1  82 138.2 0 156.8 146.1 142.9 161.7 149.4
 2023 12 30 2596 23 10 23 13  3  7 10 10  0  77   4   9   5   2   3   4   4   0   4 0.1 0  65 135.1 0 157.3 145.7 139.7 162.2 149.1
 2023 12 31 2596 24  0  7  3  3  3  7 10 13  47   0   3   2   2   2   3   4   5   3 0.0 0  53 141.4 0 157.6 145.5 146.2 162.5 148.9
 2024 01 01 2596 25  7  3  7 13 20 30 33 40 153   3   2   3   5   7  15  18  27  10 0.6 3  54 131.2 0 157.9 145.2 135.7 162.8 148.6
 2024 01 02 2596 26 27 23  7 20 23 27 20  7 153  12   9   3   7   9  12   7   3   8 0.4 2  66 137.4 0 157.8 145.1 142.1 162.7 148.6
 2024 01 03 2596 27 27 27 10 17 17 27 33 30 187  12  12   4   6   6  12  18  15  11 0.6 3  57 135.5 0 157.9 144.9 140.2 162.9 148.5
 2024 01 04 2597  1 13  7 17  7  7 13 10 27 100   5   3   6   3   3   5   4  12   5 0.2 1  98 121.6 0 158.1 144.7 125.8 163.1 148.2
-2024 01 05 2597  2 20 17  3 10 13 17  3  3  87   7   6   2   4   5   6   2   2   4 0.1 0 117 147.6 0 158.4 144.7 152.7 163.3 148.3
-2024 01 06 2597  3  3 10  0  0  0  0  7 10  30   2   4   0   0   0   0   3   4   2 0.0 0 144 154.1 0 158.6 144.9 159.4 163.5 148.6
-2024 01 07 2597  4  0  0  0  3  3  3  0  0  10   0   0   0   2   2   2   0   0   1 0.0 0 164 161.6 0 158.7 145.3 167.1 163.7 149.0
-2024 01 08 2597  5  0  0  0  3 10  7 13 20  53   0   0   0   2   4   3   5   7   3 0.0 0 162 170.4 0 158.0 145.8 176.2 162.9 149.6
-2024 01 09 2597  6 23 10 23  7  7 13  3 10  97   9   4   9   3   3   5   2   4   5 0.2 1 148 170.1 0 158.1 146.4 175.9 163.1 150.2
-2024 01 10 2597  7 13 17 13 20 23 17 20 17 140   5   6   5   7   9   6   7   6   6 0.3 1 164 179.9 0 158.3 147.1 186.0 163.2 151.0
-2024 01 11 2597  8  7 13 17 13 20 13  7 17 107   3   5   6   5   7   5   3   6   5 0.2 1 179 186.2 0 158.5 147.9 192.5 163.4 151.9
-2024 01 12 2597  9  0 13  3 10 13 13  7 10  70   0   5   2   4   5   5   3   4   4 0.1 0 179 180.3 0 158.7 148.7 186.4 163.6 152.7
-2024 01 13 2597 10  3  0  3  7  7  7  3  7  37   2   0   2   3   3   3   2   3   2 0.0 0 186 179.4 0 159.0 149.4 185.4 163.9 153.5
-2024 01 14 2597 11  7 13 17 20 17 20 20 20 133   3   5   6   7   6   7   7   7   6 0.3 1 157 181.7 0 159.3 150.1 187.9 164.2 154.3
-2024 01 15 2597 12 10  7 17 17 23  3 13 17 107   4   3   6   6   9   2   5   6   5 0.2 1 140 176.6 0 159.5 150.7 182.5 164.4 154.9
-2024 01 16 2597 13 27 20  7  7  7 10 10  3  90  12   7   3   3   3   4   4   2   5 0.2 1 131 173.8 0 159.8 151.3 179.6 164.7 155.6
-2024 01 17 2597 14  7  3 13  7  7  7  7 10  60   3   2   5   3   3   3   3   4   3 0.1 0 146 168.5 0 160.0 151.9 174.1 164.9 156.2
-2024 01 18 2597 15 10 10 10 17 13 13 23 23 120   4   4   4   6   5   5   9   9   6 0.3 1 129 157.1 0 160.3 152.1 162.3 165.2 156.5
-2024 01 19 2597 16 13 27 17 13 17 17 13 23 140   5  12   6   5   6   6   5   9   7 0.3 1 141 152.4 0 160.6 152.3 157.4 165.5 156.7
-2024 01 20 2597 17 17 23 13 10 20 17 13 13 127   6   9   5   4   7   6   5   5   6 0.3 1 132 161.0 0 161.0 152.5 166.3 165.9 156.9
-2024 01 21 2597 18  0 13 13 20 17 10  7 10  90   0   5   5   7   6   4   3   4   4 0.1 0 154 172.9 0 161.5 152.7 178.5 166.3 157.2
-2024 01 22 2597 19  7  3 10 13 17 20 30 33 133   3   2   4   5   6   7  15  18   8 0.4 2 164 189.9 0 162.0 153.2 196.1 166.8 157.7
-2024 01 23 2597 20 20 27 17 10 13 10 10 20 127   7  12   6   4   5   4   4   7   6 0.3 1 144 174.7 0 162.5 153.4 180.3 167.3 158.0
-2024 01 24 2597 21 33 30 30 17 13  3  3  3 133  18  15  15   6   5   2   2   2   8 0.4 2 122 166.6 0 162.7 153.6 172.0 167.5 158.2
-2024 01 25 2597 22  3  7  7 13 17 17 13 23 100   2   3   3   5   6   6   5   9   5 0.2 1  92 155.6 0 163.1 153.6 160.5 167.9 158.2
-2024 01 26 2597 23  3 13  3  7 20 17 13 17  93   2   5   2   3   7   6   5   6   4 0.2 1  79 151.9 0 163.4 153.7 156.7 168.2 158.4
-2024 01 27 2597 24 23 13 10 10  7  7  7  7  83   9   5   4   4   3   3   3   3   4 0.1 0  63 143.6 0 163.7 153.7 148.1 168.4 158.4
-2024 01 28 2597 25  7 10 10 20 13 17 30 30 137   3   4   4   7   5   6  15  15   7 0.4 2  68 136.8 0 163.8 153.7 141.1 168.5 158.3
-2024 01 29 2597 26 27 20 10  7 23 20 23 20 150  12   7   4   3   9   7   9   7   7 0.4 2  70 136.1 0 163.8 153.7 140.3 168.4 158.4
-2024 01 30 2597 27 20 23 17 17 10 10 23 20 140   7   9   6   6   4   4   9   7   6 0.3 1  70 131.0 0 163.6 153.5 135.0 168.2 158.2
-2024 01 31 2598  1 20 23 13 13 13 20 20 10 133   7   9   5   5   5   7   7   4   6 0.3 1  94 132.2 0 163.3 153.5 136.2 167.8 158.2
-2024 02 01 2598  2 10 10 17 20  7 13 17  7 100   4   4   6   7   3   5   6   3   5 0.2 1 114 132.9 0 163.1 153.4 136.9 167.6 158.2
-2024 02 02 2598  3  3  3 10  7  3  0  0  0  27   2   2   4   3   2   0   0   0   2 0.0 0 118 138.5 0 163.1 153.5 142.6 167.5 158.3
-2024 02 03 2598  4  0  7  3  3  0  3  0  3  20   0   3   2   2   0   2   0   2   1 0.0 0 117 152.0 0 163.0 153.9 156.4 167.4 158.7
-2024 02 04 2598  5 10 13 10 17  7 10 17 30 113   4   5   4   6   3   4   6  15   6 0.3 1 131 165.6 0 162.9 154.5 170.4 167.3 159.3
-2024 02 05 2598  6  3  7 13 13 17 20 17 23 113   2   3   5   5   6   7   6   9   5 0.2 1 162 168.6 0 163.1 155.2 173.4 167.4 160.0
-2024 02 06 2598  7 30 23 13 17 17 13 17  7 137  15   9   5   6   6   5   6   3   7 0.3 1 161 185.1 0 163.3 156.0 190.3 167.5 160.9
-2024 02 07 2598  8  0  7 13 17 13 10  7 13  80   0   3   5   6   5   4   3   5   4 0.1 0 154 183.3 0 163.5 156.8 188.4 167.7 161.7
-2024 02 08 2598  9  7 10  7 17 17 17 17  3  93   3   4   3   6   6   6   6   2   4 0.2 1 163 180.0 0 163.8 157.3 185.0 168.0 162.2
-2024 02 09 2598 10 10  0  7 13 17  3  7 30  87   4   0   3   5   6   2   3  15   5 0.2 1 128 178.6 0 164.1 157.6 183.4 168.3 162.5
-2024 02 10 2598 11 10 10 13 20 17  7  3 10  90   4   4   5   7   6   3   2   4   4 0.2 1 150 188.7 0 164.4 157.9 193.8 168.5 162.8
-2024 02 11 2598 12 43 33 33 30 17 23 13 20 213  32  18  18  15   6   9   5   7  14 0.8 4 151 175.7 0 164.6 157.8 180.4 168.7 162.7
-2024 02 12 2598 13 17 20 20  3  3  0  0  3  67   6   7   7   2   2   0   0   2   3 0.1 0 161 203.0 0 164.8 157.9 208.3 168.8 162.9
-2024 02 13 2598 14 17 23 13 23 20 40 20 20 177   6   9   5   9   7  27   7   7  10 0.5 2 133 189.9 0 164.9 158.1 194.8 168.9 163.1
+2024 01 05 2597  2 20 17  3 10 13 17  3  3  87   7   6   2   4   5   6   2   2   4 0.1 0 117 147.6 0 158.2 144.7 152.7 163.2 148.3
+2024 01 06 2597  3  3 10  0  0  0  0  7 10  30   2   4   0   0   0   0   3   4   2 0.0 0 144 154.1 0 158.2 144.9 159.4 163.2 148.6
+2024 01 07 2597  4  0  0  0  3  3  3  0  0  10   0   0   0   2   2   2   0   0   1 0.0 0 164 161.6 0 158.0 145.3 167.1 162.9 149.0
+2024 01 08 2597  5  0  0  0  3 10  7 13 20  53   0   0   0   2   4   3   5   7   3 0.0 0 162 170.4 0 157.0 145.8 176.2 161.9 149.6
+2024 01 09 2597  6 23 10 23  7  7 13  3 10  97   9   4   9   3   3   5   2   4   5 0.2 1 148 170.1 0 156.8 146.4 175.9 161.7 150.2
+2024 01 10 2597  7 13 17 13 20 23 17 20 17 140   5   6   5   7   9   6   7   6   6 0.3 1 164 179.9 0 156.7 147.1 186.0 161.5 151.0
+2024 01 11 2597  8  7 13 17 13 20 13  7 17 107   3   5   6   5   7   5   3   6   5 0.2 1 179 186.2 0 156.6 147.9 192.5 161.4 151.9
+2024 01 12 2597  9  0 13  3 10 13 13  7 10  70   0   5   2   4   5   5   3   4   4 0.1 0 179 180.3 0 156.8 148.7 186.4 161.7 152.7
+2024 01 13 2597 10  3  0  3  7  7  7  3  7  37   2   0   2   3   3   3   2   3   2 0.0 0 186 179.4 0 157.3 149.4 185.4 162.1 153.5
+2024 01 14 2597 11  7 13 17 20 17 20 20 20 133   3   5   6   7   6   7   7   7   6 0.3 1 157 181.7 0 157.7 150.1 187.9 162.5 154.3
+2024 01 15 2597 12 10  7 17 17 23  3 13 17 107   4   3   6   6   9   2   5   6   5 0.2 1 140 176.6 0 158.2 150.7 182.5 163.0 154.9
+2024 01 16 2597 13 27 20  7  7  7 10 10  3  90  12   7   3   3   3   4   4   2   5 0.2 1 131 173.8 0 158.8 151.3 179.6 163.6 155.6
+2024 01 17 2597 14  7  3 13  7  7  7  7 10  60   3   2   5   3   3   3   3   4   3 0.1 0 146 168.5 0 159.3 151.9 174.1 164.1 156.2
+2024 01 18 2597 15 10 10 10 17 13 13 23 23 120   4   4   4   6   5   5   9   9   6 0.3 1 129 157.1 0 159.7 152.1 162.3 164.5 156.5
+2024 01 19 2597 16 13 27 17 13 17 17 13 23 140   5  12   6   5   6   6   5   9   7 0.3 1 141 152.4 0 160.3 152.3 157.4 165.2 156.7
+2024 01 20 2597 17 17 23 13 10 20 17 13 13 127   6   9   5   4   7   6   5   5   6 0.3 1 132 161.0 0 160.8 152.5 166.3 165.6 156.9
+2024 01 21 2597 18  0 13 13 20 17 10  7 10  90   0   5   5   7   6   4   3   4   4 0.1 0 154 172.9 0 161.2 152.7 178.5 166.0 157.2
+2024 01 22 2597 19  7  3 10 13 17 20 30 33 133   3   2   4   5   6   7  15  18   8 0.4 2 164 189.9 0 161.5 153.2 196.1 166.3 157.7
+2024 01 23 2597 20 20 27 17 10 13 10 10 20 127   7  12   6   4   5   4   4   7   6 0.3 1 144 174.7 0 161.6 153.4 180.3 166.4 158.0
+2024 01 24 2597 21 33 30 30 17 13  3  3  3 133  18  15  15   6   5   2   2   2   8 0.4 2 122 166.6 0 161.5 153.6 172.0 166.2 158.2
+2024 01 25 2597 22  3  7  7 13 17 17 13 23 100   2   3   3   5   6   6   5   9   5 0.2 1  92 155.6 0 161.5 153.6 160.5 166.2 158.2
+2024 01 26 2597 23  3 13  3  7 20 17 13 17  93   2   5   2   3   7   6   5   6   4 0.2 1  79 151.9 0 161.4 153.7 156.7 166.0 158.4
+2024 01 27 2597 24 23 13 10 10  7  7  7  7  83   9   5   4   4   3   3   3   3   4 0.1 0  63 143.6 0 161.2 153.7 148.1 165.8 158.4
+2024 01 28 2597 25  7 10 10 20 13 17 30 30 137   3   4   4   7   5   6  15  15   7 0.4 2  68 136.8 0 160.8 153.7 141.1 165.4 158.3
+2024 01 29 2597 26 27 20 10  7 23 20 23 20 150  12   7   4   3   9   7   9   7   7 0.4 2  70 136.1 0 160.3 153.7 140.3 164.9 158.4
+2024 01 30 2597 27 20 23 17 17 10 10 23 20 140   7   9   6   6   4   4   9   7   6 0.3 1  70 131.0 0 159.5 153.5 135.0 164.0 158.2
+2024 01 31 2598  1 20 23 13 13 13 20 20 10 133   7   9   5   5   5   7   7   4   6 0.3 1  94 132.2 0 158.7 153.5 136.2 163.2 158.2
+2024 02 01 2598  2 10 10 20 20 10 20 20  3 113   4   4   7   7   4   7   7   2   5 0.2 1 118 132.9 0 158.1 153.4 136.9 162.5 158.2
+2024 02 02 2598  3  3  3 10  7  7  7  3  0  40   2   2   4   3   3   3   2   0   2 0.0 0 123 138.5 0 157.6 153.5 142.6 161.9 158.3
+2024 02 03 2598  4  0  7  3  3  0  7  0  3  23   0   3   2   2   0   3   0   2   2 0.0 0 127 152.0 0 157.0 153.9 156.4 161.2 158.7
+2024 02 04 2598  5  7 13  7 13  7 13 20 30 110   3   5   3   5   3   5   7  15   6 0.3 1 137 165.6 0 156.5 154.5 170.4 160.8 159.3
+2024 02 05 2598  6  0  3 13 10 20 23 17 27 113   0   2   5   4   7   9   6  12   6 0.3 1 157 168.6 0 156.5 155.2 173.4 160.6 160.0
+2024 02 06 2598  7 30 20 13 17 17 17 20  7 140  15   7   5   6   6   6   7   3   7 0.3 1 157 185.1 0 156.5 156.0 190.3 160.7 160.9
+2024 02 07 2598  8  0  3 13 13 13  7  7  7  63   0   2   5   5   5   3   3   3   3 0.1 0 150 183.3 0 156.9 156.8 188.4 161.0 161.7
+2024 02 08 2598  9  7 10  7 13 17 17 17  3  90   3   4   3   5   6   6   6   2   4 0.2 1 165 180.0 0 157.3 157.3 185.0 161.4 162.2
+2024 02 09 2598 10  7  0  3 13 20  3 10 30  87   3   0   2   5   7   2   4  15   5 0.2 1 129 178.6 0 157.8 157.6 183.4 161.8 162.5
+2024 02 10 2598 11  7  7 13 23 17  7  3  7  83   3   3   5   9   6   3   2   3   4 0.1 0 150 188.7 0 158.5 157.9 193.8 162.4 162.8
+2024 02 11 2598 12 43 33 33 30 17 23 17 17 213  32  18  18  15   6   9   6   6  14 0.8 4 167 175.7 0 159.3 157.8 180.4 163.2 162.7
+2024 02 12 2598 13 17 23 20  3  3  3  3  3  77   6   9   7   2   2   2   2   2   4 0.1 0 157 203.0 0 160.1 157.9 208.3 164.0 162.9
+2024 02 13 2598 14 13 20 10 20 20 37 20 27 167   5   7   4   7   7  22   7  12   9 0.5 2 138 189.9 0 160.9 158.1 194.8 164.7 163.1
+2024 02 14 2598 15 30 23  7 10  7  7  3 10  97  15   9   3   4   3   3   2   4   5 0.2 1 143 179.5 0 161.7 158.2 184.1 165.5 163.2
+2024 02 15 2598 16 10  3  7  7  7  7 13  7  60   4   2   3   3   3   3   5   3   3 0.1 0 147 173.9 0 162.1 158.2 178.3 165.8 163.2
+2024 02 16 2598 17 10  0  7 13 20 13  0  7  70   4   0   3   5   7   5   0   3   3 0.1 0 145 164.8 0 162.3 158.0 168.8 166.0 162.9
+2024 02 17 2598 18 10  3  0 13 17  7 13 20  83   4   2   0   5   6   3   5   7   4 0.1 0 120 165.9 0 162.4 157.0 169.9 166.1 161.9
+2024 02 18 2598 19 33 17 10 13 10  3  3  0  90  18   6   4   5   4   2   2   0   5 0.2 1 102 152.9 0 162.4 156.8 156.5 166.0 161.7
+2024 02 19 2598 20  0  0  0  0  3  0  3  3  10   0   0   0   0   2   0   2   2   1 0.0 0  73 148.6 0 162.0 156.7 152.1 165.5 161.5
+2024 02 20 2598 21  3  7 20 17 20 13 10 23 113   2   3   7   6   7   5   4   9   5 0.2 1  54 149.2 0 161.4 156.6 152.6 164.9 161.4
+2024 02 21 2598 22  7  0  7  7  7 13 13  3  57   3   0   3   3   3   5   5   2   3 0.1 0  51 166.2 0 160.6 156.8 169.9 164.0 161.7
+2024 02 22 2598 23 17 13 17 17 10 10 13 10 107   6   5   6   6   4   4   5   4   5 0.2 1  58 169.6 0 159.9 157.3 173.3 163.2 162.1
+2024 02 23 2598 24  0  0  3 10 13  7  3  7  43   0   0   2   4   5   3   2   3   2 0.0 0 106 169.2 0 159.3 157.7 172.9 162.5 162.5
+2024 02 24 2598 25  7  3  7 10 20 23 20 23 113   3   2   3   4   7   9   7   9   6 0.2 1 111 175.5 0 158.6 158.2 179.2 161.8 163.0
+2024 02 25 2598 26 23 30 20 20 30 17 27 27 193   9  15   7   7  15   6  12  12  10 0.6 3 115 177.1 0 158.1 158.8 180.8 161.1 163.6
+2024 02 26 2598 27 30 30 23 27 23 13 13 20 180  15  15   9  12   9   5   5   7  10 0.5 2 137 168.3 0 157.5 159.3 171.7 160.5 164.1
+2024 02 27 2599  1 37 43 30  7 10 10 30 10 177  22  32  15   3   4   4  15   4  12 0.7 3 120 165.1 0 157.0 159.7 168.3 159.9 164.5
+2024 02 28 2599  2 10 13 17 20  7  7 10 10  93   4   5   6   7   3   3   4   4   4 0.2 1 131 175.7 0 156.6 160.3 179.1 159.5 165.2
+2024 02 29 2599  3  3  0 10 13 17 10  3  7  63   2   0   4   5   6   4   2   3   3 0.1 0 128 161.1 0 156.5 160.8 164.1 159.3 165.6
+2024 03 01 2599  4 27 27 27 13 13 17 13 10 147  12  12  12   5   5   6   5   4   8 0.4 2 119 150.1 0 156.2 161.2 152.8 158.9 166.0
+2024 03 02 2599  5 23 13  7  7 13  0  3  7  73   9   5   3   3   5   0   2   3   4 0.1 0  97 149.7 0 155.8 161.5 152.3 158.4 166.3
+2024 03 03 2599  6 27  7  7 33 47 57 57 37 270  12   3   3  18  39  67  67  22  29 1.3 6 101 143.1 0 155.2 161.6 145.5 157.7 166.4
+2024 03 04 2599  7 37 23 20 10 13 10  7 23 143  22   9   7   4   5   4   3   9   8 0.4 2 109 137.6 0 154.8 161.5 139.9 157.2 166.2
+2024 03 05 2599  8 30  7 20 17 20 13 20  7 133  15   3   7   6   7   5   7   3   7 0.3 1 111 139.2 0 154.6 161.5 141.5 157.0 166.2
+2024 03 06 2599  9 10 30 13 17 17 10  0  3 100   4  15   5   6   6   4   0   2   5 0.2 1 101 133.9 0 154.5 161.4 136.0 156.8 166.0
+2024 03 07 2599 10 27 17 20 23 20 27 40 33 207  12   6   7   9   7  12  27  18  12 0.7 3  97 134.5 0 154.5 161.2 136.6 156.7 165.8
+2024 03 08 2599 11 30 33 20  3 17  7 17 37 163  15  18   7   2   6   3   6  22  10 0.6 3 102 127.2 0 154.7 160.8 129.0 156.9 165.4
+2024 03 09 2599 12 40 33 23 20 17 10 27 17 187  27  18   9   7   6   4  12   6  11 0.6 3  95 132.6 0 155.0 160.3 134.5 157.1 164.9
+2024 03 10 2599 13 13 10 17 27 13 20 20 10 130   5   4   6  12   5   7   7   4   6 0.3 1  77 125.3 0 155.4 159.5 127.0 157.4 164.0
+2024 03 11 2599 14 13 13 20 10  3  7  0 10  77   5   5   7   4   2   3   0   4   4 0.1 0  75 125.1 0 155.9 158.7 126.7 157.8 163.2
+2024 03 12 2599 15 23  3 10 17 13 17  3  3  90   9   2   4   6   5   6   2   2   4 0.2 1  84 128.9 0 156.3 158.1 130.5 158.2 162.5
+2024 03 13 2599 16 13  7 37 20 23 30 17  7 153   5   3  22   7   9  15   6   3   9 0.5 2  81 126.8 0 156.8 157.6 128.3 158.6 161.9
+2024 03 14 2599 17 10 23 17 17 10 13 17 33 140   4   9   6   6   4   5   6  18   7 0.4 2  70 125.7 0 157.2 157.0 127.1 158.9 161.2
+2024 03 15 2599 18 33 23 20 13 13  7  3  7 120  18   9   7   5   5   3   2   3   6 0.3 1  53 127.7 0 157.4 156.5 129.0 159.1 160.8
+2024 03 16 2599 19  3  0  3  0  3  3  0  3  17   2   0   2   0   2   2   0   2   1 0.0 0  63 142.6 0 157.3 156.5 144.1 158.9 160.6
+2024 03 17 2599 20  0  0  3  0  0  0  0  0   3   0   0   2   0   0   0   0   0   0 0.0 0  74 149.8 0 157.1 156.5 151.3 158.6 160.7
+2024 03 18 2599 21  3  3  7  0  7  3 20 27  70   2   2   3   0   3   2   7  12   4 0.1 0 119 175.8 0 156.5 156.9 177.4 158.0 161.0
+2024 03 19 2599 22 27 20 20 20 10  7 13 13 130  12   7   7   7   4   3   5   5   6 0.3 1 134 167.5 0 155.9 157.3 168.9 157.2 161.4
+2024 03 20 2599 23 20  3 13  7  3  0  7 23  77   7   2   5   3   2   0   3   9   4 0.1 0 124 174.1 0 155.3 157.8 175.5 156.5 161.8
+2024 03 21 2599 24 27 23 30 23 43 50 43 40 280  12   9  15   9  32  48  32  27  23 1.1 5 162 195.5 0 154.7 158.5 196.9 155.8 162.4
+2024 03 22 2599 25 33 30 27 33 10 13  3  3 153  18  15  12  18   4   5   2   2  10 0.5 2 164 196.2 0 153.9 159.3 197.6 155.0 163.2
+2024 03 23 2599 26 27 47 40 37 40 40 47 57 333  12  39  27  22  27  27  39  67  32 1.3 6 157 209.3 0 153.4 160.1 210.7 154.4 164.0
+2024 03 24 2599 27 47 33 37 37 63 83 63 40 403  39  18  22  22  94 236  94  27  69 1.7 7 166 194.0 0 152.5 160.9 195.1 153.4 164.7
+2024 03 25 2600  1 43 50 37 40 40 30 20 20 280  32  48  22  27  27  15   7   7  23 1.1 5 167 189.1 0 151.7 161.7 190.1 152.6 165.5
+2024 03 26 2600  2 33 27  7 30 23 20 30 30 200  18  12   3  15   9   7  15  15  12 0.7 3 141 177.4 0 151.3 162.1 178.2 152.0 165.8
+2024 03 27 2600  3 30 10 23 10  7  7  7 13 107  15   4   9   4   3   3   3   5   6 0.3 1 114 173.9 0 150.8 162.3 174.6 151.5 166.0
+2024 03 28 2600  4 20 13 13 13 23 13 17 23 137   7   5   5   5   9   5   6   9   6 0.3 1  98 172.1 0 150.5 162.4 172.7 151.1 166.1
+2024 03 29 2600  5 20 17 17 17 17  7  3  7 103   7   6   6   6   6   3   2   3   5 0.2 1  81 166.8 0 150.2 162.4 167.3 150.7 166.0
+2024 03 30 2600  6  3  3  3  7 10 13  7 20  67   2   2   2   3   4   5   3   7   4 0.1 0  50 139.3 0 150.1 162.0 139.6 150.5 165.5
+2024 03 31 2600  7 40 20 23 13 10 13  7 23 150  27   7   9   5   4   5   3   9   9 0.5 2  66 133.4 0 149.9 161.4 133.6 150.3 164.9
+2024 04 01 2600  8 20 33 37 17 17 13 23 13 173   7  18  22   6   6   5   9   5  10 0.5 2  31 120.3 0 150.0 160.6 120.4 150.2 164.0
 END OBSERVED
 
 NUM_DAILY_PREDICTED_POINTS 45
 BEGIN DAILY_PREDICTED
-2024 02 14 2598 15 30 27 13 10  7 39 30 47 202  15  12   5   4   3  25  15  39  14 0.8 4 147 192.0   165.3 158.4 197.0 169.2 163.3
-2024 02 15 2598 16 30 27 23 27 20 13 20 23 183  15  12   9  12   7   5   7   9   9 0.5 2 129 192.0   165.3 158.6 196.9 169.2 163.5
-2024 02 16 2598 17 17 13 13 13 13 13 17 17 117   6   5   5   5   5   5   6   6   5 0.2 1 129 195.0   165.3 158.7 199.9 169.1 163.7
-2024 02 17 2598 18 17 13 13 13 13 13 13 13 110   6   5   5   5   5   5   5   5   5 0.2 1 129 185.0   165.3 158.0 189.5 169.1 162.9
-2024 02 18 2598 19 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 180.0   165.2 158.1 184.3 168.9 163.1
-2024 02 19 2598 20 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 175.0   165.1 158.3 179.2 168.7 163.2
-2024 02 20 2598 21 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   164.8 158.5 174.0 168.3 163.4
-2024 02 21 2598 22 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   164.4 158.7 163.7 167.9 163.6
-2024 02 22 2598 23 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 165.0   164.1 159.0 168.7 167.5 163.9
-2024 02 23 2598 24 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   163.8 159.3 163.5 167.1 164.2
-2024 02 24 2598 25 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   163.5 159.5 153.2 166.7 164.4
-2024 02 25 2598 26 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   163.2 159.8 153.2 166.4 164.7
-2024 02 26 2598 27 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 150.0   163.0 160.0 153.1 166.1 164.9
-2024 02 27 2599  1 20 20 20 20 20 20 20 20 160   7   7   7   7   7   7   7   7   7 0.4 2 129 150.0   162.8 160.3 153.0 165.8 165.2
-2024 02 28 2599  2 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   162.8 160.6 152.9 165.8 165.5
-2024 02 29 2599  3 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 155.0   162.8 161.0 158.0 165.7 165.9
-2024 03 01 2599  4 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   162.8 161.5 163.0 165.6 166.3
-2024 03 02 2599  5 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 165.0   162.6 162.0 168.0 165.3 166.8
-2024 03 03 2599  6 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   162.1 162.5 173.0 164.8 167.3
-2024 03 04 2599  7 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   161.9 162.7 172.9 164.5 167.5
-2024 03 05 2599  8 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   161.8 163.1 172.8 164.3 167.9
-2024 03 06 2599  9 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   161.8 163.4 172.7 164.2 168.2
-2024 03 07 2599 10 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   161.8 163.7 172.6 164.1 168.4
-2024 03 08 2599 11 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   161.9 163.8 172.5 164.2 168.5
-2024 03 09 2599 12 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   162.2 163.8 172.5 164.4 168.4
-2024 03 10 2599 13 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   162.4 163.6 172.4 164.6 168.2
-2024 03 11 2599 14 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 165.0   162.7 163.3 167.2 164.8 167.8
-2024 03 12 2599 15 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 165.0   163.0 163.1 167.1 165.0 167.6
-2024 03 13 2599 16 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 165.0   163.3 163.1 167.0 165.2 167.5
-2024 03 14 2599 17 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   163.5 163.0 172.0 165.4 167.4
-2024 03 15 2599 18 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   163.5 162.9 161.8 165.3 167.3
-2024 03 16 2599 19 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   163.4 163.1 161.7 165.1 167.4
-2024 03 17 2599 20 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   163.2 163.3 161.6 164.9 167.5
-2024 03 18 2599 21 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   162.9 163.5 161.5 164.4 167.7
-2024 03 19 2599 22 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   162.5 163.8 161.4 164.0 168.0
-2024 03 20 2599 23 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 165.0   162.2 164.1 166.4 163.6 168.3
-2024 03 21 2599 24 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   162.0 164.4 161.2 163.2 168.5
-2024 03 22 2599 25 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   161.5 164.6 151.1 162.7 168.7
-2024 03 23 2599 26 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   161.3 164.8 151.0 162.4 168.8
-2024 03 24 2599 27 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 150.0   160.7 164.9 150.9 161.7 168.9
-2024 03 25 2600  1 20 20 20 20 20 20 20 20 160   7   7   7   7   7   7   7   7   7 0.4 2 129 150.0   160.3 165.3 150.8 161.2 169.2
-2024 03 26 2600  2 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   159.8 165.3 150.7 160.7 169.2
-2024 03 27 2600  3 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 155.0   159.4 165.3 155.7 160.1 169.1
-2024 03 28 2600  4 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   158.9 165.3 160.6 159.5 169.1
-2024 03 29 2600  5 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 165.0   158.5 165.2 165.5 159.1 168.9
+2024 04 02 2600  9 10 17 17 23 20 13 22 20 142   4   6   6   9   7   5   8   7   6 0.3 1  43 124.0   149.8 159.9 124.1 149.9 163.2
+2024 04 03 2600 10 30 20 20 20 23 23 27 40 203  15   7   7   7   9   9  12  27  11 0.7 3 129 126.0   149.5 159.3 126.0 149.6 162.5
+2024 04 04 2600 11 40 37 27 23 23 27 30 47 253  27  22  12   9   9  12  15  39  18 1.0 5 129 130.0   149.4 158.6 130.0 149.4 161.8
+2024 04 05 2600 12 47 33 33 33 33 33 33 33 280  39  18  18  18  18  18  18  18  20 1.1 5 129 130.0   149.2 158.1 129.9 149.1 161.1
+2024 04 06 2600 13 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 128.0   149.1 157.5 127.8 148.9 160.5
+2024 04 07 2600 14 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 128.0   149.0 157.0 127.7 148.7 159.9
+2024 04 08 2600 15 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 128.0   148.8 156.6 127.7 148.5 159.5
+2024 04 09 2600 16 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 140.0   148.6 156.5 139.6 148.1 159.3
+2024 04 10 2600 17 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 140.0   148.5 156.2 139.5 148.0 158.9
+2024 04 11 2600 18 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 140.0   148.6 155.8 139.4 148.0 158.4
+2024 04 12 2600 19 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 140.0   148.6 155.2 139.3 148.0 157.7
+2024 04 13 2600 20 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 140.0   148.8 154.8 139.2 148.0 157.2
+2024 04 14 2600 21 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   149.0 154.6 149.1 148.2 157.0
+2024 04 15 2600 22 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   149.2 154.5 149.0 148.3 156.8
+2024 04 16 2600 23 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   149.4 154.5 148.9 148.5 156.7
+2024 04 17 2600 24 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   149.7 154.7 158.8 148.6 156.9
+2024 04 18 2600 25 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   150.0 155.0 158.7 148.9 157.1
+2024 04 19 2600 26 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 170.0   150.3 155.4 168.5 149.1 157.4
+2024 04 20 2600 27 24 24 24 24 24 24 24 24 192  10  10  10  10  10  10  10  10  10 0.6 3 129 170.0   150.7 155.9 168.4 149.4 157.8
+2024 04 21 2601  1 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 170.0   151.0 156.3 168.3 149.7 158.2
+2024 04 22 2601  2 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 170.0   151.4 156.8 168.2 149.9 158.6
+2024 04 23 2601  3 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 170.0   151.7 157.2 168.2 150.2 158.9
+2024 04 24 2601  4 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 170.0   152.1 157.4 168.1 150.5 159.1
+2024 04 25 2601  5 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 160.0   152.4 157.3 158.1 150.8 158.9
+2024 04 26 2601  6 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 129 150.0   152.6 157.1 148.1 150.9 158.6
+2024 04 27 2601  7 24 24 24 24 24 24 24 24 192  10  10  10  10  10  10  10  10  10 0.6 3 129 140.0   152.6 156.5 138.2 150.9 158.0
+2024 04 28 2601  8 24 24 24 24 24 24 24 24 192  10  10  10  10  10  10  10  10  10 0.6 3 129 130.0   152.4 155.9 128.3 150.5 157.2
+2024 04 29 2601  9 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 129 130.0   152.2 155.3 128.2 150.3 156.5
+2024 04 30 2601 10 27 27 27 27 27 27 27 27 216  12  12  12  12  12  12  12  12  12 0.7 3 129 130.0   152.0 154.7 128.1 150.0 155.8
+2024 05 01 2601 11 27 27 27 27 27 27 27 27 216  12  12  12  12  12  12  12  12  12 0.7 3 130 130.0   151.5 153.9 128.1 149.4 155.0
+2024 05 02 2601 12 27 27 27 27 27 27 27 27 216  12  12  12  12  12  12  12  12  12 0.7 3 130 130.0   151.0 153.4 128.0 148.8 154.4
+2024 05 03 2601 13 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 130 130.0   150.3 152.5 127.9 148.1 153.4
+2024 05 04 2601 14 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 130.0   149.8 151.7 127.9 147.5 152.6
+2024 05 05 2601 15 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 140.0   149.4 151.3 137.6 147.0 152.0
+2024 05 06 2601 16 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 130 140.0   149.1 150.8 137.6 146.7 151.5
+2024 05 07 2601 17 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 130 140.0   148.9 150.5 137.5 146.4 151.1
+2024 05 08 2601 18 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 130 140.0   148.7 150.2 137.4 146.1 150.7
+2024 05 09 2601 19 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 140.0   148.5 150.1 137.4 145.9 150.5
+2024 05 10 2601 20 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 140.0   148.7 149.9 137.3 146.0 150.3
+2024 05 11 2601 21 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 150.0   149.0 150.0 147.0 146.2 150.2
+2024 05 12 2601 22 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 150.0   149.4 149.8 147.0 146.6 149.9
+2024 05 13 2601 23 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 150.0   149.8 149.5 146.9 146.9 149.6
+2024 05 14 2601 24 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 160.0   150.2 149.4 156.6 147.2 149.4
+2024 05 15 2601 25 13 13 13 13 13 13 13 13 104   5   5   5   5   5   5   5   5   5 0.2 1 130 160.0   150.5 149.2 156.6 147.5 149.1
+2024 05 16 2601 26 22 22 22 22 22 22 22 22 176   8   8   8   8   8   8   8   8   8 0.4 2 130 170.0   150.8 149.1 166.3 147.7 148.9
 END DAILY_PREDICTED
 
-NUM_MONTHLY_PREDICTED_POINTS 211
+NUM_MONTHLY_PREDICTED_POINTS 209
 BEGIN MONTHLY_PREDICTED
-2024 04 01 2600  8                                                                       130 155.5   157.8 164.4 155.7 158.1 167.9
-2024 05 01 2601 11                                                                       131 155.6   155.4 161.5 153.3 153.3 162.7
-2024 06 01 2602 15                                                                       132 155.8   155.7 156.1 151.5 151.7 154.7
-2024 07 01 2603 18                                                                       131 155.6   155.6 155.7 150.5 150.9 152.2
-2024 08 01 2604 22                                                                       132 155.3   155.4 155.7 150.7 151.2 151.1
-2024 09 01 2605 26                                                                       132 154.9   155.1 155.5 152.1 152.5 151.0
-2024 10 01 2607  2                                                                       132 154.4   154.7 155.2 154.0 154.3 152.0
-2024 11 01 2608  6                                                                       131 154.1   154.2 154.8 156.4 156.4 153.7
-2024 12 01 2609  9                                                                       130 153.7   153.8 154.4 158.1 157.8 155.8
-2025 01 01 2610 13                                                                       130 152.8   153.1 154.0 158.0 157.9 157.6
-2025 02 01 2611 17                                                                       128 151.5   152.0 153.4 156.0 156.1 158.1
-2025 03 01 2612 18                                                                       126 149.7   150.6 152.5 152.5 153.2 157.1
-2025 04 01 2613 22                                                                       124 147.9   148.8 151.1 148.1 149.0 154.3
-2025 05 01 2614 25                                                                       122 146.3   147.1 149.4 144.1 145.2 150.5
-2025 06 01 2616  2                                                                       121 144.9   145.5 147.7 140.9 141.9 146.3
-2025 07 01 2617  5                                                                       119 143.2   144.0 146.1 138.5 139.6 142.9
-2025 08 01 2618  9                                                                       117 141.2   142.1 144.5 137.1 138.2 140.3
-2025 09 01 2619 13                                                                       115 138.9   140.0 142.8 136.4 137.6 138.6
-2025 10 01 2620 16                                                                       114 136.9   138.0 140.8 136.6 137.6 137.8
-2025 11 01 2621 20                                                                       112 135.2   136.1 138.6 137.2 137.9 137.7
-2025 12 01 2622 23                                                                       110 133.7   134.4 136.7 137.5 137.9 137.9
-2026 01 01 2623 27                                                                       107 131.8   132.7 135.0 136.3 136.8 138.1
-2026 02 01 2625  4                                                                       105 129.8   130.8 133.3 133.7 134.4 137.4
-2026 03 01 2626  5                                                                       103 128.4   129.2 131.6 130.8 131.5 135.5
-2026 04 01 2627  9                                                                       102 127.2   127.7 129.8 127.4 128.0 132.5
-2026 05 01 2628 12                                                                       100 125.7   126.4 128.3 123.9 124.7 129.2
-2026 06 01 2629 16                                                                        98 123.9   124.7 126.9 120.5 121.5 125.7
-2026 07 01 2630 19                                                                        96 121.9   122.9 125.3 117.9 119.2 122.6
-2026 08 01 2631 23                                                                        93 119.8   120.8 123.5 116.3 117.5 119.9
-2026 09 01 2632 27                                                                        91 117.9   118.8 121.5 115.7 116.8 118.0
-2026 10 01 2634  3                                                                        88 115.9   116.9 119.5 115.6 116.6 117.0
-2026 11 01 2635  7                                                                        85 113.8   114.8 117.5 115.5 116.4 116.7
-2026 12 01 2636 10                                                                        82 112.1   113.0 115.5 115.3 115.9 116.5
-2027 01 01 2637 14                                                                        80 110.5   111.3 113.6 114.3 114.7 116.2
-2027 02 01 2638 18                                                                        78 108.7   109.5 111.8 112.0 112.5 115.3
-2027 03 01 2639 19                                                                        76 106.9   107.9 110.2 108.9 109.8 113.6
-2027 04 01 2640 23                                                                        74 105.4   106.1 108.4 105.6 106.3 110.8
-2027 05 01 2641 26                                                                        71 103.7   104.5 106.7 102.2 103.1 107.5
-2027 06 01 2643  3                                                                        69 101.9   102.7 105.1  99.1 100.2 104.1
-2027 07 01 2644  6                                                                        67 100.2   101.1 103.4  96.9  98.1 101.1
-2027 08 01 2645 10                                                                        64  99.0    99.6 101.6  96.1  96.9  98.7
-2027 09 01 2646 14                                                                        62  97.7    98.3 100.1  95.9  96.6  97.2
-2027 10 01 2647 17                                                                        60  96.6    97.2  98.8  96.3  96.9  96.7
-2027 11 01 2648 21                                                                        58  95.7    96.1  97.6  97.1  97.4  96.9
-2027 12 01 2649 24                                                                        56  94.7    95.2  96.5  97.4  97.6  97.3
-2028 01 01 2651  1                                                                        54  93.5    94.1  95.5  96.7  97.0  97.7
-2028 02 01 2652  5                                                                        52  92.3    92.9  94.4  95.1  95.5  97.3
-2028 03 01 2653  7                                                                        51  91.2    91.8  93.3  92.9  93.4  96.1
-2028 04 01 2654 11                                                                        49  90.0    90.5  92.1  90.1  90.7  94.1
-2028 05 01 2655 14                                                                        47  88.7    89.4  91.0  87.4  88.1  91.6
-2028 06 01 2656 18                                                                        45  87.6    88.2  89.8  85.2  86.0  88.9
-2028 07 01 2657 21                                                                        44  86.8    87.2  88.6  84.0  84.6  86.6
-2028 08 01 2658 25                                                                        43  85.8    86.3  87.5  83.3  83.9  85.0
-2028 09 01 2660  2                                                                        41  84.8    85.2  86.6  83.3  83.8  84.1
-2028 10 01 2661  5                                                                        39  83.6    84.2  85.6  83.4  84.0  83.9
-2028 11 01 2662  9                                                                        37  82.6    83.1  84.5  83.8  84.3  84.0
-2028 12 01 2663 12                                                                        36  81.8    82.2  83.5  84.1  84.4  84.2
+2024 06 01 2602 15                                                                       130 155.1   152.2 151.4 150.8 148.4 149.9
+2024 07 01 2603 18                                                                       130 155.0   155.0 152.4 150.0 150.3 149.0
+2024 08 01 2604 22                                                                       131 154.6   154.8 155.3 150.1 150.6 150.7
+2024 09 01 2605 26                                                                       131 154.2   154.4 154.9 151.4 151.8 150.4
+2024 10 01 2607  2                                                                       131 153.7   154.0 154.5 153.3 153.6 151.3
+2024 11 01 2608  6                                                                       130 153.4   153.6 154.1 155.7 155.7 153.1
+2024 12 01 2609  9                                                                       130 153.1   153.2 153.7 157.5 157.2 155.1
+2025 01 01 2610 13                                                                       129 152.2   152.5 153.3 157.4 157.3 156.9
+2025 02 01 2611 17                                                                       128 150.8   151.3 152.8 155.3 155.5 157.5
+2025 03 01 2612 18                                                                       125 149.1   149.9 151.9 151.9 152.5 156.5
+2025 04 01 2613 22                                                                       123 147.3   148.2 150.5 147.5 148.4 153.7
+2025 05 01 2614 25                                                                       122 145.7   146.6 148.8 143.5 144.6 149.8
+2025 06 01 2616  2                                                                       120 144.4   145.0 147.1 140.4 141.3 145.7
+2025 07 01 2617  5                                                                       118 142.7   143.5 145.6 138.1 139.1 142.3
+2025 08 01 2618  9                                                                       116 140.7   141.6 144.0 136.6 137.7 139.8
+2025 09 01 2619 13                                                                       115 138.4   139.5 142.3 135.9 137.1 138.2
+2025 10 01 2620 16                                                                       113 136.4   137.5 140.3 136.1 137.2 137.3
+2025 11 01 2621 20                                                                       112 134.8   135.6 138.1 136.8 137.5 137.2
+2025 12 01 2622 23                                                                       109 133.3   134.0 136.2 137.1 137.5 137.4
+2026 01 01 2623 27                                                                       107 131.4   132.3 134.6 135.9 136.4 137.6
+2026 02 01 2625  4                                                                       104 129.4   130.4 132.9 133.3 134.0 136.9
+2026 03 01 2626  5                                                                       103 128.1   128.9 131.2 130.5 131.1 135.1
+2026 04 01 2627  9                                                                       101 126.8   127.4 129.4 127.0 127.6 132.2
+2026 05 01 2628 12                                                                        99 125.3   126.0 127.9 123.5 124.3 128.8
+2026 06 01 2629 16                                                                        97 123.6   124.3 126.5 120.2 121.2 125.4
+2026 07 01 2630 19                                                                        95 121.6   122.5 125.0 117.6 118.8 122.2
+2026 08 01 2631 23                                                                        93 119.5   120.5 123.2 116.0 117.2 119.6
+2026 09 01 2632 27                                                                        90 117.7   118.6 121.2 115.5 116.5 117.7
+2026 10 01 2634  3                                                                        87 115.7   116.7 119.3 115.4 116.4 116.8
+2026 11 01 2635  7                                                                        84 113.6   114.6 117.3 115.3 116.2 116.5
+2026 12 01 2636 10                                                                        81 111.9   112.8 115.3 115.1 115.7 116.3
+2027 01 01 2637 14                                                                        79 110.3   111.1 113.4 114.1 114.5 116.0
+2027 02 01 2638 18                                                                        77 108.5   109.3 111.6 111.8 112.3 115.0
+2027 03 01 2639 19                                                                        75 106.8   107.7 110.0 108.8 109.6 113.4
+2027 04 01 2640 23                                                                        73 105.2   105.9 108.3 105.4 106.2 110.6
+2027 05 01 2641 26                                                                        71 103.5   104.3 106.6 102.0 102.9 107.4
+2027 06 01 2643  3                                                                        69 101.7   102.6 104.9  98.9 100.0 104.0
+2027 07 01 2644  6                                                                        66 100.1   101.0 103.2  96.8  97.9 100.9
+2027 08 01 2645 10                                                                        64  98.9    99.5 101.5  96.0  96.8  98.5
+2027 09 01 2646 14                                                                        62  97.6    98.2 100.0  95.8  96.5  97.1
+2027 10 01 2647 17                                                                        60  96.5    97.1  98.7  96.2  96.9  96.6
+2027 11 01 2648 21                                                                        58  95.7    96.1  97.5  97.1  97.4  96.8
+2027 12 01 2649 24                                                                        55  94.6    95.1  96.4  97.3  97.6  97.3
+2028 01 01 2651  1                                                                        53  93.4    94.0  95.4  96.6  96.9  97.6
+2028 02 01 2652  5                                                                        52  92.2    92.8  94.4  95.0  95.3  97.2
+2028 03 01 2653  7                                                                        50  91.1    91.7  93.2  92.8  93.3  96.0
+2028 04 01 2654 11                                                                        49  90.0    90.5  92.0  90.1  90.6  94.0
+2028 05 01 2655 14                                                                        47  88.7    89.3  90.9  87.4  88.1  91.6
+2028 06 01 2656 18                                                                        45  87.6    88.2  89.7  85.2  85.9  88.9
+2028 07 01 2657 21                                                                        44  86.7    87.2  88.6  83.9  84.6  86.6
+2028 08 01 2658 25                                                                        42  85.8    86.2  87.5  83.3  83.9  84.9
+2028 09 01 2660  2                                                                        40  84.7    85.2  86.5  83.2  83.8  84.0
+2028 10 01 2661  5                                                                        38  83.6    84.1  85.6  83.4  84.0  83.8
+2028 11 01 2662  9                                                                        37  82.5    83.1  84.5  83.7  84.2  83.9
+2028 12 01 2663 12                                                                        36  81.8    82.2  83.4  84.1  84.3  84.2
 2029 01 01 2664 16                                                                        34  81.1    81.4  82.5  83.9  84.0  84.4
-2029 02 01 2665 20                                                                        33  80.4    80.7  81.7  82.8  82.9  84.2
-2029 03 01 2666 21                                                                        31  79.7    80.1  81.0  81.2  81.5  83.5
-2029 04 01 2667 25                                                                        29  79.0    79.3  80.3  79.1  79.5  82.0
-2029 05 01 2669  1                                                                        28  78.3    78.7  79.6  77.1  77.6  80.1
-2029 06 01 2670  5                                                                        26  77.7    78.0  78.9  75.6  76.0  78.2
-2029 07 01 2671  8                                                                        25  77.1    77.4  78.2  74.6  75.1  76.5
-2029 08 01 2672 12                                                                        24  76.5    76.8  77.6  74.3  74.7  75.3
-2029 09 01 2673 16                                                                        22  76.0    76.2  77.0  74.6  75.0  74.8
+2029 02 01 2665 20                                                                        32  80.4    80.7  81.7  82.8  82.9  84.2
+2029 03 01 2666 21                                                                        31  79.6    80.0  81.0  81.1  81.4  83.5
+2029 04 01 2667 25                                                                        29  78.9    79.3  80.3  79.0  79.4  82.0
+2029 05 01 2669  1                                                                        27  78.3    78.6  79.5  77.1  77.5  80.1
+2029 06 01 2670  5                                                                        26  77.6    77.9  78.8  75.5  76.0  78.1
+2029 07 01 2671  8                                                                        25  77.0    77.3  78.2  74.5  75.0  76.4
+2029 08 01 2672 12                                                                        23  76.5    76.8  77.5  74.3  74.7  75.2
+2029 09 01 2673 16                                                                        22  76.0    76.2  76.9  74.6  74.9  74.7
 2029 10 01 2674 19                                                                        21  75.5    75.7  76.4  75.3  75.6  74.8
-2029 11 01 2675 23                                                                        20  75.0    75.2  75.9  76.1  76.2  75.4
-2029 12 01 2676 26                                                                        18  74.3    74.6  75.4  76.4  76.6  76.1
-2030 01 01 2678  3                                                                        17  73.6    73.9  74.8  76.1  76.3  76.5
-2030 02 01 2679  7                                                                        15  72.9    73.2  74.2  75.1  75.3  76.4
+2029 11 01 2675 23                                                                        20  74.9    75.2  75.9  76.0  76.2  75.4
+2029 12 01 2676 26                                                                        18  74.3    74.6  75.4  76.4  76.5  76.0
+2030 01 01 2678  3                                                                        17  73.6    73.9  74.8  76.1  76.2  76.5
+2030 02 01 2679  7                                                                        15  72.9    73.2  74.1  75.1  75.3  76.4
 2030 03 01 2680  8                                                                        14  72.4    72.7  73.5  73.8  74.0  75.7
-2030 04 01 2681 12                                                                        13  72.1    72.2  72.9  72.2  72.4  74.4
-2030 05 01 2682 15                                                                        12  71.7    71.9  72.4  70.6  70.9  72.9
-2030 06 01 2683 19                                                                        12  71.4    71.5  72.0  69.4  69.7  71.4
-2030 07 01 2684 22                                                                        11  71.0    71.2  71.7  68.7  69.1  70.1
-2030 08 01 2685 26                                                                        10  70.7    70.9  71.3  68.6  68.9  69.2
-2030 09 01 2687  3                                                                         9  70.4    70.6  71.0  69.1  69.4  68.9
-2030 10 01 2688  6                                                                         9  70.3    70.4  70.7  70.1  70.2  69.2
-2030 11 01 2689 10                                                                         8  70.1    70.2  70.4  71.1  71.2  69.9
-2030 12 01 2690 13                                                                         8  70.0    70.1  70.2  72.0  71.9  70.9
-2031 01 01 2691 17                                                                         9  70.1    70.1  70.1  72.5  72.3  71.7
-2031 02 01 2692 21                                                                        10  70.4    70.3  70.1  72.5  72.3  72.2
+2030 04 01 2681 12                                                                        13  72.0    72.2  72.9  72.1  72.3  74.4
+2030 05 01 2682 15                                                                        12  71.7    71.8  72.4  70.6  70.9  72.9
+2030 06 01 2683 19                                                                        12  71.3    71.5  72.0  69.4  69.7  71.3
+2030 07 01 2684 22                                                                        11  71.0    71.2  71.6  68.7  69.0  70.0
+2030 08 01 2685 26                                                                        10  70.7    70.8  71.3  68.6  68.9  69.2
+2030 09 01 2687  3                                                                         9  70.4    70.6  70.9  69.1  69.4  68.9
+2030 10 01 2688  6                                                                         9  70.2    70.3  70.7  70.0  70.1  69.2
+2030 11 01 2689 10                                                                         8  70.0    70.1  70.4  71.0  71.1  69.9
+2030 12 01 2690 13                                                                         8  70.0    70.0  70.2  72.0  71.9  70.8
+2031 01 01 2691 17                                                                         9  70.1    70.1  70.0  72.5  72.3  71.7
+2031 02 01 2692 21                                                                        10  70.4    70.3  70.0  72.5  72.3  72.2
 2031 03 01 2693 22                                                                        11  70.8    70.6  70.2  72.1  71.8  72.3
 2031 04 01 2694 26                                                                        12  71.1    71.0  70.5  71.2  71.1  72.0
 2031 05 01 2696  2                                                                        14  71.5    71.3  70.8  70.5  70.4  71.3
 2031 06 01 2697  6                                                                        15  72.1    71.9  71.2  70.1  70.0  70.6
 2031 07 01 2698  9                                                                        17  72.8    72.5  71.6  70.4  70.3  70.1
 2031 08 01 2699 13                                                                        19  73.5    73.2  72.2  71.3  71.2  70.1
 2031 09 01 2700 17                                                                        21  74.3    74.0  72.9  72.9  72.7  70.8
```

### Comparing `spaceweather-0.2.4/src/spaceweather/omni.py` & `spaceweather-0.3.0/src/spaceweather/omni.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 .. [#] https://omniweb.gsfc.nasa.gov/ow.html
 """
 import os
 from pkg_resources import resource_filename
 import logging
 from warnings import warn
 
+from posixpath import join as urljoin
+
 import numpy as np
 import pandas as pd
 
 from .core import _assert_file_exists, _dl_file
 
 __all__ = [
 	"cache_omnie",
@@ -136,38 +138,38 @@
 	basename = "{0}_{1:04d}.{2}".format(prefix, year, ext)
 
 	if not os.path.exists(local_path):
 		os.makedirs(local_path)
 
 	omnie_file = os.path.join(local_path, basename)
 	if not os.path.exists(omnie_file):
-		url = os.path.join(url_base, basename)
+		url = urljoin(url_base, basename)
 		logging.info("%s not found, downloading from %s.", omnie_file, url)
 		_dl_file(omnie_file, url)
 
 
 def omnie_mask_missing(df):
 	"""Mask missing values with NaN
 
 	Marks missing values in the OMNI2 data set by NaN.
 	The missing value indicating numbers are taken from the file format description
 	https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/extended/aareadme_extended
 
 	Parameters
 	----------
 	df: pandas.DataFrame
-		The OMNI2 data set, e.g. from ``omnie_hourly()`` or ``read_omnie()``.
+		The OMNI2 data set, e.g. from :func:`omnie_hourly()` or :func:`read_omnie()`.
 
 	Returns
 	-------
 	df: pandas.DataFrame
-		The same dataframe with the missing values masked with numpy.nan.
+		The same dataframe with the missing values masked with ``numpy.nan``.
 
-	Note
-	----
+	Notes
+	-----
 	This function returns a copy of the dataframe, and all the integer columns
 	will be converted to float to support NaN.
 	"""
 	res = df.copy()
 	for _c in df.columns:
 		_m = _OMNI_MISSING.get(_c, None)
 		if _m is None:
```

### Comparing `spaceweather-0.2.4/src/spaceweather.egg-info/PKG-INFO` & `spaceweather-0.3.0/src/spaceweather.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaceweather
-Version: 0.2.4
+Version: 0.3.0
 Summary: Python interface for space weather indices
 Home-page: https://github.com/st-bender/pyspaceweather
 Author: Stefan Bender
 Author-email: stefan.bender@ntnu.no
 License: GPLv2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,16 +12,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: COPYING.CCby4.0
 License-File: COPYING.GPLv2
 License-File: COPYING.data
+License-File: COPYING.gfz
 License-File: COPYING.omni
 Requires-Dist: numpy>=1.13.0
 Requires-Dist: pandas
 Requires-Dist: requests
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
@@ -39,15 +41,17 @@
 [![wheel](https://img.shields.io/pypi/wheel/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![pyversions](https://img.shields.io/pypi/pyversions/spaceweather.svg?style=flat)](https://pypi.org/project/spaceweather)
 [![codecov](https://codecov.io/gh/st-bender/pyspaceweather/badge.svg)](https://codecov.io/gh/st-bender/pyspaceweather)
 [![coveralls](https://coveralls.io/repos/github/st-bender/pyspaceweather/badge.svg)](https://coveralls.io/github/st-bender/pyspaceweather)
 [![scrutinizer](https://scrutinizer-ci.com/g/st-bender/pyspaceweather/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/st-bender/pyspaceweather/?branch=master)
 
 This python module interfaces the space weather data available at
-<https://celestrak.com/SpaceData/> and <https://omniweb.gsfc.nasa.gov/ow.html>.
+<https://celestrak.com/SpaceData/>,
+<https://kp.gfz-potsdam.de/en/data>,
+and <https://omniweb.gsfc.nasa.gov/ow.html>.
 It includes the geomagnetic Ap and Kp indices, both the 3h values and
 the daily sum/averages.
 The data also include the solar f10.7 cm radio fluxes,
 the observed values as well as the 1 AU adjusted values,
 daily values and the 81-day running means.
 See [Data sources](#data-sources) below.
 
@@ -154,14 +158,51 @@
 2000-01-01 13:30:00  32  4.3
 2000-01-01 16:30:00  15  3.0
 2000-01-01 19:30:00  32  4.3
 2000-01-01 22:30:00  22  3.7
 
 ```
 
+### GFZ
+
+The "GFZ" module supports the ascii and WDC files as offered by the
+[GFZ German Research Centre for Geosciences](https://www.gfz-potsdam.de/en/)
+on their [data page](https://kp.gfz-potsdam.de/en/data).
+In contrast to the official python client, this module reads the data
+from the (downloaded) files and does not access the web service API.
+The interface is mostly the same as for the "Celestrak" data:
+
+```python
+>>> import spaceweather as sw
+>>> df_d = sw.gfz_daily()
+>>> df_d.loc["2000-01-01"].Apavg
+30.0
+>>> df_3h = sw.gfz_3h()
+>>> df_3h.loc["2000-01-01 01:30:00"]
+Ap    56.000
+Kp     5.333
+Name: 2000-01-01 01:30:00, dtype: float64
+
+```
+
+Currently, the data are not included in the package, downloads can be triggered
+by passing `update=True` to `sw.gfz_daily()` or by running `sw.update_gfz()`.
+The lower-level interface functions are called `read_gfz(<filename>)`
+for the ascii `.txt` files, and `read_gfz_wdc(<filename>)` for the WDC format.
+They can also be used directly for reading already downloaded data files
+outside of the package's data directory.
+
+```python
+>>> import spaceweather as sw
+>>> df_d = sw.read_gfz("./tests/Kp_ap_Ap_SN_F107_since_2024.txt")
+>>> df_d.loc["2024-01-01"].Apavg
+10.0
+
+```
+
 ### OMNI
 
 The [OMNI](https://omniweb.gsfc.nasa.gov/ow.html) 1-hour yearly data
 are accessible via `omnie_hourly(<year>)` or `read_omnie(<file>)`.
 Both functions should work with the OMNI2 standard and extended text files.
 If the data are not already available locally, they can be cached by passing
 `cache=True` to that function or by calling `cache_omnie(<year>)` explicitly.
@@ -196,14 +237,15 @@
 ### Reference
 
 Basic class and method documentation is accessible via `pydoc`:
 
 ```sh
 $ pydoc spaceweather
 $ pydoc spaceweather.celestrak
+$ pydoc spaceweather.gfz
 $ pydoc spaceweather.omni
 ```
 
 ## License
 
 This python interface is free software: you can redistribute it or modify
 it under the terms of the GNU General Public License as published by
@@ -219,14 +261,30 @@
 [celestrak](https://celestrak.com),
 for details see the included [COPYING.data](COPYING.data) file.
 
 The data sources and file format are described at
 <http://celestrak.com/SpaceData/SpaceWx-format.php>
 (see [file_format.txt](file_format.txt) for a local copy of the format description).
 
+### GFZ
+
+The "GFZ" data are provided as tabulated ascii files
+([format description](https://kp.gfz-potsdam.de/app/format/Kp_ap_Ap_SN_F107_format.txt),
+[local copy](gfz_Kp_ap_Ap_SN_F107_format.txt))
+and in [WDC format](https://kp.gfz-potsdam.de/app/format/wdc_fmt.txt)
+([local copy](gfz_wdc_fmt.txt))
+by the
+[GFZ German Research Centre for Geosciences](https://www.gfz-potsdam.de/en/)
+on their official [data webpage](https://kp.gfz-potsdam.de/en/data).
+The data have the doi: [10.5880/Kp.0001](https://doi.org/10.5880/Kp.0001),
+and they are provided under the "Creative Commons attribution license"
+[CC-by 4.0](https://creativecommons.org/licenses/by/4.0/)
+(local copy [COPYING.CCby4.0](COPYING.CCby4.0)).
+See also [COPYING.gfz](COPYING.gfz) for details.
+
 ### OMNI
 
 This package includes part of the hourly-resolved OMNI data,
 accessible through <https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/>,
 and it enables easy downloading of it.
 The file format is described at
 <https://spdf.gsfc.nasa.gov/pub/data/omni/low_res_omni/omni2.text>
```

### Comparing `spaceweather-0.2.4/src/spaceweather.egg-info/SOURCES.txt` & `spaceweather-0.3.0/src/spaceweather.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 CHANGES.md
+COPYING.CCby4.0
 COPYING.GPLv2
 COPYING.data
+COPYING.gfz
 COPYING.omni
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+docs/COPYING.CCby4.0
 docs/COPYING.GPLv2
 docs/COPYING.data
+docs/COPYING.gfz
 docs/COPYING.omni
 docs/Makefile
 docs/README.md
 docs/conf.py
 docs/file_format.txt
+docs/gfz_Kp_ap_Ap_SN_F107_format.txt
+docs/gfz_wdc_fmt.txt
 docs/index.rst
 docs/omni_format.txt
 docs/omnie_format.txt
 docs/reference/index.rst
 docs/reference/spaceweather.rst
 src/spaceweather/__init__.py
 src/spaceweather/celestrak.py
 src/spaceweather/core.py
+src/spaceweather/gfz.py
 src/spaceweather/omni.py
 src/spaceweather.egg-info/PKG-INFO
 src/spaceweather.egg-info/SOURCES.txt
 src/spaceweather.egg-info/dependency_links.txt
 src/spaceweather.egg-info/not-zip-safe
 src/spaceweather.egg-info/requires.txt
 src/spaceweather.egg-info/top_level.txt
 src/spaceweather/data/.cache
 src/spaceweather/data/SW-All.txt
 src/spaceweather/data/SW-Last5Years.txt
 src/spaceweather/data/omni_extended/.cache
+tests/Kp_ap_Ap_SN_F107_nowcast.txt
+tests/Kp_ap_Ap_SN_F107_since_2024.txt
 tests/omni2t_2000.dat
+tests/test_gfz.py
 tests/test_omni.py
 tests/test_read.py
```

### Comparing `spaceweather-0.2.4/tests/omni2t_2000.dat` & `spaceweather-0.3.0/tests/omni2t_2000.dat`

 * *Files identical despite different names*

### Comparing `spaceweather-0.2.4/tests/test_omni.py` & `spaceweather-0.3.0/tests/test_omni.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 # it under the terms of the GNU General Public License as published
 # by the Free Software Foundation, version 2.
 # See accompanying COPYING.GPLv2 file or http://www.gnu.org/licenses/gpl-2.0.html.
 """OMNI data read tests
 """
 import os
 import requests
+from posixpath import join as urljoin
 
 import numpy as np
 import pandas as pd
 
 import pytest
 
 from spaceweather import cache_omnie, omnie_hourly, omnie_mask_missing, sw_daily
 from spaceweather.omni import OMNI_URL_BASE, OMNI_PREFIX, OMNI_EXT
 
 _TEST_YEAR = 2012
 _TEST_FILE = "{0}_{1:04d}.{2}".format(OMNI_PREFIX, _TEST_YEAR, OMNI_EXT)
-_TEST_URL = os.path.join(OMNI_URL_BASE, _TEST_FILE)
+_TEST_URL = urljoin(OMNI_URL_BASE, _TEST_FILE)
 _TEST_PATH = os.path.join(".", "tests")
 
 
 @pytest.fixture(scope="module")
 def df_d():
 	return sw_daily()
```

### Comparing `spaceweather-0.2.4/tests/test_read.py` & `spaceweather-0.3.0/tests/test_read.py`

 * *Files identical despite different names*

