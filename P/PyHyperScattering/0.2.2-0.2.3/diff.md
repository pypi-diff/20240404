# Comparing `tmp/PyHyperScattering-0.2.2.tar.gz` & `tmp/PyHyperScattering-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyHyperScattering-0.2.2.tar", last modified: Mon Oct  2 21:05:58 2023, max compression
+gzip compressed data, was "PyHyperScattering-0.2.3.tar", last modified: Thu Apr  4 18:05:16 2024, max compression
```

## Comparing `PyHyperScattering-0.2.2.tar` & `PyHyperScattering-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:05:58.496233 PyHyperScattering-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2023-10-02 21:05:58.496233 PyHyperScattering-0.2.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3528 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-10-02 21:05:58.496233 PyHyperScattering-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:05:58.484233 PyHyperScattering-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:05:58.496233 PyHyperScattering-0.2.2/src/PyHyperScattering/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10030 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/ALS11012RSoXSLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/ESRFID2Loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12736 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/FileIO.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9282 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/FileLoader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12893 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/Fitting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4242 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/HDR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/IntegrationUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10147 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/Nexus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11762 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/PFEnergySeriesIntegrator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24799 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/PFGeneralIntegrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/PlotTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/RSoXS.py
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/SMIRSoXSLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    53511 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/SST1RSoXSDB.py
--rw-r--r--   0 runner    (1001) docker     (127)    14158 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/SST1RSoXSLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/WPIntegrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-02 21:05:58.496233 PyHyperScattering-0.2.2/src/PyHyperScattering/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    15279 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/cyrsoxsLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/src/PyHyperScattering/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:05:58.492233 PyHyperScattering-0.2.2/src/PyHyperScattering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2023-10-02 21:05:58.000000 PyHyperScattering-0.2.2/src/PyHyperScattering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-10-02 21:05:58.000000 PyHyperScattering-0.2.2/src/PyHyperScattering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-02 21:05:58.000000 PyHyperScattering-0.2.2/src/PyHyperScattering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-02 21:05:58.000000 PyHyperScattering-0.2.2/src/PyHyperScattering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-02 21:05:58.000000 PyHyperScattering-0.2.2/src/PyHyperScattering.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-02 21:05:58.496233 PyHyperScattering-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_11012Loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_PFIntegrators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_RSoXS.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_SMILoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_SST1DBLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_SST1Loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_WPintegrator.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_autoversioning.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_cyrsoxsLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    78254 2023-10-02 21:05:43.000000 PyHyperScattering-0.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:16.938150 PyHyperScattering-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-04 18:05:16.938150 PyHyperScattering-0.2.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3528 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-04 18:05:16.938150 PyHyperScattering-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:16.934150 PyHyperScattering-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:16.938150 PyHyperScattering-0.2.3/src/PyHyperScattering/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10030 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/ALS11012RSoXSLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/ESRFID2Loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/FileIO.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9282 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/FileLoader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12893 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/Fitting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4242 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/HDR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/IntegrationUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/Nexus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12014 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/PFEnergySeriesIntegrator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26477 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/PFGeneralIntegrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/PlotTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/RSoXS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/SMIRSoXSLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54636 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/SST1RSoXSDB.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/SST1RSoXSLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/WPIntegrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 18:05:16.938150 PyHyperScattering-0.2.3/src/PyHyperScattering/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15279 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/cyrsoxsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/src/PyHyperScattering/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:16.938150 PyHyperScattering-0.2.3/src/PyHyperScattering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-04 18:05:16.000000 PyHyperScattering-0.2.3/src/PyHyperScattering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-04 18:05:16.000000 PyHyperScattering-0.2.3/src/PyHyperScattering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:05:16.000000 PyHyperScattering-0.2.3/src/PyHyperScattering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 18:05:16.000000 PyHyperScattering-0.2.3/src/PyHyperScattering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 18:05:16.000000 PyHyperScattering-0.2.3/src/PyHyperScattering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:16.938150 PyHyperScattering-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_11012Loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_PFIntegrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_RSoXS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_SMILoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_SST1DBLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_SST1Loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_WPintegrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_autoversioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_cyrsoxsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78254 2024-04-04 18:05:12.000000 PyHyperScattering-0.2.3/versioneer.py
```

### Comparing `PyHyperScattering-0.2.2/LICENSE` & `PyHyperScattering-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/PKG-INFO` & `PyHyperScattering-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHyperScattering
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utilities for loading, reducing, fitting, and plotting hyperspectral x-ray and neutron scattering data.
 Home-page: https://github.com/usnistgov/pyhyperscattering
 Author: Peter Beaucage
 Author-email: peter.beaucage@nist.gov
 Project-URL: Github, https://github.com/usnistgov/pyhyperscattering
 Project-URL: Project Site, https://www.nist.gov/laboratories/tools-instruments/polarized-resonant-soft-x-ray-scattering-p-rsoxs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyHyperScattering-0.2.2/README.md` & `PyHyperScattering-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/setup.cfg` & `PyHyperScattering-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/ALS11012RSoXSLoader.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/ALS11012RSoXSLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/ESRFID2Loader.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/ESRFID2Loader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/FileIO.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/FileIO.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/FileLoader.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/FileLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/Fitting.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/Fitting.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/HDR.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/HDR.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/IntegrationUtils.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/IntegrationUtils.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/Nexus.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/Nexus.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/PFEnergySeriesIntegrator.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/PFEnergySeriesIntegrator.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 class PFEnergySeriesIntegrator(PFGeneralIntegrator):
 
     def integrateSingleImage(self,img):
         # for each image: 
         #    get the energy and locate the matching integrator
         #    use that integrator to reduce
         #    return single reduced frame
+
         #print(f'    img.energy is a {type(img.energy)}, len = {len(img.energy)} and is {img.energy}') 
         #print(f'    img.system is a {type(img.system)}, len = {len(img.energy)} and is {img.system}')
         #print(f'    img.system.levels: {img.indexes["system"].names}')
         #print(f'    img.indexes: {img.indexes}')
         #print(f'    type of system value: {type(getattr(img,"system").values)}')
         #print(f'    shape of system value: {getattr(img,"system").values.shape}')
         en = None
@@ -71,29 +72,31 @@
             try:
                 en = img.energy.values[0]
                 if len(img.energy.values)>1:
                     warnings.warn(f'Using the first energy value of {img.energy.values}, check that this is correct.',stacklevel=2)
             except IndexError:
                 en = float(img.energy)
             except AttributeError:
-                en = img.energy[0]
-                warnings.warn(f'Using the first energy value of {img.energy}, check that this is correct.',stacklevel=2)
+                try:
+                    en = img.energy[0]
+                    warnings.warn(f'Using the first energy value of {img.energy}, if this contains more than one energy, your data are likely wrong.',stacklevel=2)
+                except IndexError:
+                    en = float(img.energy)
             
-        
         try:
             self.integrator = self.integrator_stack[en]
         except KeyError:
             self.integrator = self.createIntegrator(en)
         res = super().integrateSingleImage(img)
         try:
             if len(self.dest_q)>0:
                 return res.interp(q=self.dest_q)
             else:
                 return res
-        except TypeError:
+        except (TypeError,AttributeError):
             return res
     def setupIntegrators(self,energies):
         '''
         Sets up the integrator stack as a function of energy.
 
         The final statement ensures that the integrator for the median of the set is created.  This integrator is used to set
         the output q-binning.
@@ -118,15 +121,15 @@
         indexes = list(img_stack.dims)
         indexes.remove('pix_x')
         indexes.remove('pix_y')
 
         # idx_name_to_use = 'energy'#indexes[0]
         # idx_val_to_use = img_stack.indexes[idx_name_to_use]
         
-        
+
         if 'energy' in indexes:
             dim_to_chunk = 'energy'
         else:
             dim_to_chunk = indexes[0]
             #this probably should check which is the longest?  Shortest?  and chunk that.
         print(f'chunking on {dim_to_chunk}')
         
@@ -192,14 +195,16 @@
         # paradigm; specifically, it needs one index that's not pixel x/y.  We either identify if that is the case, or we make it the
         # case.  however, there are probably edge cases not handled here
         
         if len(indexes) == 1:
             if img_stack.__getattr__(indexes[0]).to_pandas().drop_duplicates().shape[0] != img_stack.__getattr__(indexes[0]).shape[0]:
                 warnings.warn(f'Axis {indexes[0]} contains duplicate conditions.  This is not supported and may not work.  Try adding additional coords to separate image conditions',stacklevel=2)
             data_int = data.groupby(indexes[0],squeeze=False).progress_apply(self.integrateSingleImage)
+        elif len(indexes) == 0:
+            data_int = self.integrateSingleImage(data).isel(image_num=0)
         else:
             #some kinda logic to check for existing multiindexes and stack into them appropriately maybe
             data = data.stack({'pyhyper_internal_multiindex':indexes})
             if data.pyhyper_internal_multiindex.to_pandas().drop_duplicates().shape[0] != data.pyhyper_internal_multiindex.shape[0]:
                 warnings.warn('Your index set contains duplicate conditions.  This is not supported and may not work.  Try adding additional coords to separate image conditions',stacklevel=2)
         
             data_int = data.groupby('pyhyper_internal_multiindex',squeeze=False).progress_apply(self.integrateSingleImage).unstack('pyhyper_internal_multiindex')
```

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/PFGeneralIntegrator.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/PFGeneralIntegrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,120 +14,183 @@
 
 # tqdm.pandas()
 # the following block monkey-patches xarray to add tqdm support.  This will not be needed once tqdm v5 releases.
 from xarray.core.groupby import DataArrayGroupBy, DatasetGroupBy
 
 
 def inner_generator(df_function='apply'):
-    def inner(df,func,*args,**kwargs):
+    def inner(df, func, *args, **kwargs):
         t = tqdm(total=len(df))
-        def wrapper(*args,**kwargs):
-            t.update( n=1 if not t.total or t.n < t.total else 0)
-            return func(*args,**kwargs)
-        result = getattr(df,df_function)(wrapper, **kwargs)
-    
+
+        def wrapper(*args, **kwargs):
+            t.update(n=1 if not t.total or t.n < t.total else 0)
+            return func(*args, **kwargs)
+
+        result = getattr(df, df_function)(wrapper, **kwargs)
+
         t.close()
         return result
+
     return inner
 
+
 DataArrayGroupBy.progress_apply = inner_generator(df_function='apply')
 DatasetGroupBy.progress_apply = inner_generator(df_function='apply')
 
 DataArrayGroupBy.progress_map = inner_generator(df_function='map')
 DatasetGroupBy.progress_map = inner_generator(df_function='map')
 
 DataArrayGroupBy.progress_map_blocks = inner_generator(df_function='map_blocks')
 DatasetGroupBy.progress_map_blocks = inner_generator(df_function='map_blocks')
 
 # end monkey patch
 
-class PFGeneralIntegrator():
+
+class PFGeneralIntegrator:
 
     def integrateSingleImage(self, img):
         if type(img) == xr.Dataset:
             for key in img.keys():
-                target_key=key
-            img=img[key]
-        if(img.ndim>2):
-            
+                target_key = key
+            img = img[key]
+        if img.ndim > 2:
+
             img_to_integ = np.squeeze(img.values)
         else:
             img_to_integ = img.values
-        
+
         if self.mask is None:
-            warnings.warn('No mask defined.  Creating an empty mask with dimensions {img.shape}.',stacklevel=2)
+            warnings.warn(
+                'No mask defined.  Creating an empty mask with dimensions {img.shape}.',
+                stacklevel=2,
+            )
             self.mask = np.zeros_like(img).squeeze()
-        assert np.shape(self.mask)==np.shape(img_to_integ),f'Error!  Mask has shape {np.shape(self.mask)} but you are attempting to integrate data with shape {np.shape(img_to_integ)}.  Try changing mask orientation or updating mask.'
+        assert np.shape(self.mask) == np.shape(
+            img_to_integ
+        ), f'Error!  Mask has shape {np.shape(self.mask)} but you are attempting to integrate data with shape {np.shape(img_to_integ)}.  Try changing mask orientation or updating mask.'
         stacked_axis = list(img.dims)
         stacked_axis.remove('pix_x')
         stacked_axis.remove('pix_y')
-        if len(stacked_axis)>0:
-            assert len(stacked_axis)==1, f"More than one dimension left after removing pix_x and pix_y, I see {stacked_axis}, not sure how to handle"
+        if len(stacked_axis) > 0:
+            assert (
+                len(stacked_axis) == 1
+            ), f"More than one dimension left after removing pix_x and pix_y, I see {stacked_axis}, not sure how to handle"
             stacked_axis = stacked_axis[0]
-            #print(f'looking for {stacked_axis} in {img[0].indexes} (indexes), it has dims {img[0].dims} and looks like {img[0]}')
-            if(img.__getattr__(stacked_axis).shape[0]>1):
+            # print(f'looking for {stacked_axis} in {img[0].indexes} (indexes), it has dims {img[0].dims} and looks like {img[0]}')
+            if img.__getattr__(stacked_axis).shape[0] > 1:
                 system_to_integ = img[0].indexes[stacked_axis]
-                warnings.warn(f'There are two images for {img.__getattr__(stacked_axis)}, I am ONLY INTEGRATING THE FIRST.  This may cause the labels to be dropped and the result to need manual re-tagging in the index.',stacklevel=2)
+                warnings.warn(
+                    f'There are two images for {img.__getattr__(stacked_axis)}, I am ONLY INTEGRATING THE FIRST.  This may cause the labels to be dropped and the result to need manual re-tagging in the index.',
+                    stacklevel=2,
+                )
             else:
                 system_to_integ = img.indexes[stacked_axis]
-                
+
         else:
             stacked_axis = 'image_num'
             system_to_integ = [0]
         if self.do_1d_integration:
             integ_func = self.integrator.integrate1d
         else:
             integ_func = self.integrator.integrate2d
 
         try:
-            frame = integ_func(img_to_integ,
-                               self.npts,
-                               filename=None,
-                               correctSolidAngle=self.correctSolidAngle,
-                               error_model="azimuthal",
-                               dummy=-8675309 if self.maskToNan else 0,
-                               mask=self.mask,
-                               unit='arcsinh(q.µm)' if self.use_log_ish_binning else 'q_A^-1',
-                               method=self.integration_method
-                               )
+            frame = integ_func(
+                img_to_integ,
+                self.npts,
+                filename=None,
+                correctSolidAngle=self.correctSolidAngle,
+                error_model="azimuthal",
+                dummy=-8675309 if self.maskToNan else 0,
+                mask=self.mask,
+                unit='arcsinh(q.µm)' if self.use_log_ish_binning else 'q_A^-1',
+                method=self.integration_method,
+            )
         except TypeError as e:
             if 'diffSolidAngle() missing 2 required positional arguments: ' in str(e):
                 raise TypeError(
-                    'Geometry is incorrect, cannot integrate.\n \n - Do your mask dimensions match your image dimensions? \n - Do you have pixel sizes set that are not zero?\n - Is SDD, beamcenter/poni, and tilt set correctly?') from e
+                    'Geometry is incorrect, cannot integrate.\n \n - Do your mask dimensions match your image dimensions? \n - Do you have pixel sizes set that are not zero?\n - Is SDD, beamcenter/poni, and tilt set correctly?'
+                ) from e
             else:
                 raise e
 
         if self.maskToNan:
             # preexisting_nans = np.isnan(TwoD.intensity).sum()
             frame.intensity[frame.intensity == -8675309] = np.nan
             # print(f'Patched dummy flag to NaN, number of NaNs = {np.isnan(TwoD.intensity).sum()}, preexisting {preexisting_nans}')
         if self.use_log_ish_binning:
             radial_to_save = np.sinh(frame.radial) / 10000  # was 1000 for inverse nm
         else:
             radial_to_save = frame.radial
         if self.do_1d_integration:
             try:
-                res = xr.DataArray([frame.intensity],dims=[stacked_axis,'q'],coords={'q':('q',radial_to_save),stacked_axis:(stacked_axis,system_to_integ)},attrs=img.attrs)
+                res = xr.DataArray(
+                    [frame.intensity],
+                    dims=[stacked_axis, 'q'],
+                    coords={
+                        'q': ('q', radial_to_save),
+                        stacked_axis: (stacked_axis, system_to_integ),
+                    },
+                    attrs=img.attrs,
+                )
                 if self.return_sigma:
-                    sigma = xr.DataArray([frame.sigma],dims=[stacked_axis,'q'],coords={'q':('q',radial_to_save),stacked_axis:(stacked_axis,system_to_integ)},attrs=img.attrs)
+                    sigma = xr.DataArray(
+                        [frame.sigma],
+                        dims=[stacked_axis, 'q'],
+                        coords={
+                            'q': ('q', radial_to_save),
+                            stacked_axis: (stacked_axis, system_to_integ),
+                        },
+                        attrs=img.attrs,
+                    )
             except AttributeError:
-                res = xr.DataArray(frame.intensity, dims=['q'], coords={'q': radial_to_save}, attrs=img.attrs)
+                res = xr.DataArray(
+                    frame.intensity, dims=['q'], coords={'q': radial_to_save}, attrs=img.attrs
+                )
                 if self.return_sigma:
-                    sigma = xr.DataArray(frame.sigma, dims=['q'], coords={'q': radial_to_save}, attrs=img.attrs)
+                    sigma = xr.DataArray(
+                        frame.sigma, dims=['q'], coords={'q': radial_to_save}, attrs=img.attrs
+                    )
         else:
             try:
-                res = xr.DataArray([frame.intensity],dims=[stacked_axis,'chi','q'],coords={'q':('q',radial_to_save),'chi':('chi',frame.azimuthal),stacked_axis:(stacked_axis,system_to_integ)},attrs=img.attrs)#.transpose(['chi','q',stacked_axis])
+                res = xr.DataArray(
+                    [frame.intensity],
+                    dims=[stacked_axis, 'chi', 'q'],
+                    coords={
+                        'q': ('q', radial_to_save),
+                        'chi': ('chi', frame.azimuthal),
+                        stacked_axis: (stacked_axis, system_to_integ),
+                    },
+                    attrs=img.attrs,
+                )  # .transpose(['chi','q',stacked_axis])
                 if self.return_sigma:
-                    sigma = xr.DataArray([frame.sigma],dims=[stacked_axis,'chi','q'],coords={'q':('q',radial_to_save),'chi':('chi',frame.azimuthal),stacked_axis:(stacked_axis,system_to_integ)},attrs=img.attrs)#.transpose(['chi','q',stacked_axis])
+                    sigma = xr.DataArray(
+                        [frame.sigma],
+                        dims=[stacked_axis, 'chi', 'q'],
+                        coords={
+                            'q': ('q', radial_to_save),
+                            'chi': ('chi', frame.azimuthal),
+                            stacked_axis: (stacked_axis, system_to_integ),
+                        },
+                        attrs=img.attrs,
+                    )  # .transpose(['chi','q',stacked_axis])
             except AttributeError:
-                res = xr.DataArray(frame.intensity, dims=['chi', 'q'],
-                                   coords={'q': radial_to_save, 'chi': frame.azimuthal}, attrs=img.attrs)
+                res = xr.DataArray(
+                    frame.intensity,
+                    dims=['chi', 'q'],
+                    coords={'q': radial_to_save, 'chi': frame.azimuthal},
+                    attrs=img.attrs,
+                )
                 if self.return_sigma:
-                    sigma = xr.DataArray(frame.sigma, dims=['chi', 'q'],
-                                         coords={'q': radial_to_save, 'chi': frame.azimuthal}, attrs=img.attrs)
+                    sigma = xr.DataArray(
+                        frame.sigma,
+                        dims=['chi', 'q'],
+                        coords={'q': radial_to_save, 'chi': frame.azimuthal},
+                        attrs=img.attrs,
+                    )
         if self.return_sigma:
             res = res.to_dataset(name='I')
             res['dI'] = sigma
         return res
 
     '''
     legacy index ident code:
@@ -140,105 +203,113 @@
                 for level in data.indexes[idx].names:
                     try:
                         real_indexes.remove(level)
                     except ValueError:
                         pass
         indexes = real_indexes
     '''
-    
-    def integrateImageStack_legacy(self,data):
+
+    def integrateImageStack_legacy(self, data):
         indexes = list(data.dims)
         indexes.remove('pix_x')
         indexes.remove('pix_y')
-        
+
         if len(indexes) == 1:
             data_int = data.groupby(indexes[0],squeeze=False).progress_map(self.integrateSingleImage)
+        elif len(indexes) == 0:
+            data_int = self.integrateSingleImage(data).isel(image_num=0)
         else:
-            #some kinda logic to check for existing multiindexes and stack into them appropriately maybe
-            data = data.stack({'pyhyper_internal_multiindex':indexes})
-            data_int = data.groupby('pyhyper_internal_multiindex',squeeze=False)
+            # some kinda logic to check for existing multiindexes and stack into them appropriately maybe
+            data = data.stack({'pyhyper_internal_multiindex': indexes})
+            data_int = data.groupby('pyhyper_internal_multiindex', squeeze=False)
             data_int = data_int.progress_map(self.integrateSingleImage)
             data_int = data_int.unstack('pyhyper_internal_multiindex')
-            #this is a hack to fix the dimension order in case we are being called as an inner function of a Dask reduction
-            if getattr(self,'expected_dim_order',None) is not None:
+            # this is a hack to fix the dimension order in case we are being called as an inner function of a Dask reduction
+            if getattr(self, 'expected_dim_order', None) is not None:
                 orig_order = data_int.dims
                 data_int = data_int.transpose(*self.expected_dim_order)
-        
+
         return data_int
-        #int_stack = img_stack.groupby('system').map_progress(self.integrateSingleImage)
-        #PRSUtils.fix_unstacked_dims(int_stack,img_stack,'system',img_stack.attrs['dims_unpacked'])
-        #return int_stack
-        
-    def integrateImageStack_dask(self,data,chunksize=5):
-        #int_stack = img_stack.groupby('system').map(self.integrateSingleImage)   
-        #return int_stack
+        # int_stack = img_stack.groupby('system').map_progress(self.integrateSingleImage)
+        # PRSUtils.fix_unstacked_dims(int_stack,img_stack,'system',img_stack.attrs['dims_unpacked'])
+        # return int_stack
+
+    def integrateImageStack_dask(self, data, chunksize=5):
+        # int_stack = img_stack.groupby('system').map(self.integrateSingleImage)
+        # return int_stack
         indexes = list(data.dims)
         try:
             indexes.remove('pix_x')
             indexes.remove('pix_y')
         except ValueError:
             pass
         try:
             indexes.remove('qx')
             indexes.remove('qy')
         except ValueError:
             pass
 
         if len(indexes) == 1:
-            if data.__getattr__(indexes[0]).to_pandas().drop_duplicates().shape[0] != data.__getattr__(indexes[0]).shape[0]:
-                warnings.warn(f'Axis {indexes[0]} contains duplicate conditions.  This is not supported and may not work.  Try adding additional coords to separate image conditions',stacklevel=2)
-            
+            if (
+                data.__getattr__(indexes[0]).to_pandas().drop_duplicates().shape[0]
+                != data.__getattr__(indexes[0]).shape[0]
+            ):
+                warnings.warn(
+                    f'Axis {indexes[0]} contains duplicate conditions.  This is not supported and may not work.  Try adding additional coords to separate image conditions',
+                    stacklevel=2,
+                )
+
             dim_to_chunk = indexes[0]
         else:
-            #some kinda logic to check for existing multiindexes and stack into them appropriately maybe
+            # some kinda logic to check for existing multiindexes and stack into them appropriately maybe
             if 'energy' in indexes:
                 dim_to_chunk = 'energy'
             else:
                 dim_to_chunk = indexes[0]
-            #this probably should check which is the longest?  Shortest?  and chunk that.
+            # this probably should check which is the longest?  Shortest?  and chunk that.
         print(f'chunking on {dim_to_chunk}')
-        
+
         '''
             data = data.stack({'pyhyper_internal_multiindex':indexes})
             if data.pyhyper_internal_multiindex.to_pandas().drop_duplicates().shape[0] != data.pyhyper_internal_multiindex.shape[0]:
                 warnings.warn('Your index set contains duplicate conditions.  This is not supported and may not work.  Try adding additional coords to separate image conditions',stacklevel=2)
                 
             fake_image_to_process = data.isel(**{'pyhyper_internal_multiindex':0},drop=False)
             indexes=['pyhyper_internal_multiindex']
             dim_to_chunk = 'pyhyper_internal_multiindex'
         '''
-        
-        fake_image_to_process = data.isel(**{dim_to_chunk:0},drop=False)
-        data = data.chunk({dim_to_chunk:chunksize})
+
+        fake_image_to_process = data.isel(**{dim_to_chunk: 0}, drop=False)
+        data = data.chunk({dim_to_chunk: chunksize})
         coord_dict = {}
         shape = tuple([])
         demo_integration = self.integrateSingleImage(fake_image_to_process)
-        coord_dict.update({'chi':demo_integration.chi,'q':demo_integration.q})
+        coord_dict.update({'chi': demo_integration.chi, 'q': demo_integration.q})
         npts_q = len(demo_integration.q)
-              
+
         order_list = []
         for idx in indexes:
             order_list.append(idx)
             coord_dict[idx] = data.indexes[idx]
             shape = shape + tuple([len(data.indexes[idx])])
-        shape = shape + (360,npts_q)
-        
-        desired_order_list = order_list+['chi','q']
+        shape = shape + (360, npts_q)
+
+        desired_order_list = order_list + ['chi', 'q']
         coord_dict_sorted = {k: coord_dict[k] for k in desired_order_list}
-        
-        
-        
-        template = xr.DataArray(np.empty(shape),coords=coord_dict_sorted)  
-        
+
+        template = xr.DataArray(np.empty(shape), coords=coord_dict_sorted)
+
         print(demo_integration.dims)
         if 'image_num' in demo_integration.dims:
-            template = template.transpose(*[item if item != 'image_num' else dim_to_chunk for item in demo_integration.dims])
+            template = template.transpose(
+                *[item if item != 'image_num' else dim_to_chunk for item in demo_integration.dims]
+            )
         elif dim_to_chunk not in demo_integration.dims:
             template = template.transpose(dim_to_chunk, *demo_integration.dims)
-        template = template.chunk({indexes[0]:chunksize})
+        template = template.chunk({indexes[0]: chunksize})
         '''
         try:
             print(template)
             print(template.indexes)
             print(template.pyhyper_internal_multiindex)
             print(data)
             print(data.indexes)
@@ -246,45 +317,51 @@
             print(data.pyhyper_internal_multiindex==template.pyhyper_internal_multiindex)
         except AttributeError:
             pass
             
         '''
         self.expected_dim_order = template.dims
         print(f'set expected dim order to {self.expected_dim_order}')
-        integ_fly = data.map_blocks(self.integrateImageStack_legacy,template=template)
-        if dim_to_chunk=='pyhyper_internal_multiindex':
+        integ_fly = data.map_blocks(self.integrateImageStack_legacy, template=template)
+        if dim_to_chunk == 'pyhyper_internal_multiindex':
             integ_fly = integ_fly.unstack('pyhyper_internal_multiindex')
-        return integ_fly 
-    
-    
-    def __init__(self,
-                 maskmethod='none', 
-                 maskpath= '',
-                 maskrotate = True,
-                 geomethod = "none",
-                 NIdistance=0, NIbcx=0, NIbcy=0, NItiltx=0, NItilty=0,
-                 NIpixsizex=0, NIpixsizey=0,
-                 template_xr=None,
-                 energy=2000,
-                 integration_method='csr_ocl',
-                 correctSolidAngle=True,
-                 maskToNan=True,
-                 npts=500,
-                 use_log_ish_binning=False,
-                 do_1d_integration=False,
-                 return_sigma=False,
-                 use_chunked_processing=False,
-                 **kwargs):
+        return integ_fly
+
+    def __init__(
+        self,
+        maskmethod='none',
+        maskpath='',
+        maskrotate=True,
+        geomethod="none",
+        NIdistance=0,
+        NIbcx=0,
+        NIbcy=0,
+        NItiltx=0,
+        NItilty=0,
+        NIpixsizex=0,
+        NIpixsizey=0,
+        template_xr=None,
+        energy=2000,
+        integration_method='csr_ocl',
+        correctSolidAngle=True,
+        maskToNan=True,
+        npts=500,
+        use_log_ish_binning=False,
+        do_1d_integration=False,
+        return_sigma=False,
+        use_chunked_processing=False,
+        **kwargs,
+    ):
         # energy units eV
         if maskmethod == 'nika':
-            self.loadNikaMask(filetoload=maskpath,rotate_image =maskrotate,**kwargs) 
+            self.loadNikaMask(filetoload=maskpath, rotate_image=maskrotate, **kwargs)
         elif maskmethod == 'polygon':
             self.loadPolyMask(**kwargs)
         elif maskmethod == 'image':
-            self.loadImageMask(**kwargs)
+            self.loadImageMask(maskpath=maskpath, maskrotate=maskrotate, **kwargs)
         elif maskmethod == 'pyhyper':
             self.loadPyHyperSavedMask(**kwargs)
         elif maskmethod == 'none':
             self.mask = None
         else:
             raise ValueError(f'Invalid or unsupported maskmethod {maskmethod}.')
         self.dist = 0.1
@@ -298,18 +375,20 @@
         self.correctSolidAngle = correctSolidAngle
         self.integration_method = integration_method
         self._energy = energy
         self.npts = npts
         self.use_log_ish_binning = use_log_ish_binning
         self.do_1d_integration = do_1d_integration
         if self.use_log_ish_binning:
-            register_radial_unit("arcsinh(q.µm)",
-                                 scale=1.0,
-                                 label=r"arcsinh($q$.µm)",
-                                 formula="arcsinh(4.0e-6*π/λ*sin(arctan2(sqrt(x**2 + y**2), z)/2.0))")
+            register_radial_unit(
+                "arcsinh(q.µm)",
+                scale=1.0,
+                label=r"arcsinh($q$.µm)",
+                formula="arcsinh(4.0e-6*π/λ*sin(arctan2(sqrt(x**2 + y**2), z)/2.0))",
+            )
 
         self.maskToNan = maskToNan
         self.return_sigma = return_sigma
         self.use_chunked_processing = use_chunked_processing
         # self._energy = 0
         if geomethod == "nika":
             self.ni_pixel_x = NIpixsizex
@@ -318,52 +397,50 @@
             self.ni_beamcenter_x = NIbcx
             self.ni_beamcenter_y = NIbcy
             self.ni_tilt_x = NItiltx
             self.ni_tilt_y = NItilty
         elif geomethod == 'template_xr':
             self.calibrationFromTemplateXRParams(template_xr)
         elif geomethod == "none":
-            warnings.warn('Initializing geometry with default values.  This is probably NOT what you want.',
-                          stacklevel=2)
+            warnings.warn(
+                'Initializing geometry with default values.  This is probably NOT what you want.',
+                stacklevel=2,
+            )
 
         self.recreateIntegrator()
 
     def __str__(self):
         return f"PyFAI general integrator wrapper SDD = {self.dist} m, poni1 = {self.poni1} m, poni2 = {self.poni2} m, rot1 = {self.rot1} rad, rot2 = {self.rot2} rad"
 
+    def integrateImageStack(self, img_stack, method=None, chunksize=None):
+        ''' '''
 
-    def integrateImageStack(self,img_stack,method=None,chunksize=None):
-        '''
-        
-        '''
-
-        if (self.use_chunked_processing and method is None) or method=='dask':
+        if (self.use_chunked_processing and method is None) or method == 'dask':
             func_args = {}
             if chunksize is not None:
                 func_args['chunksize'] = chunksize
-            return self.integrateImageStack_dask(img_stack,**func_args)
+            return self.integrateImageStack_dask(img_stack, **func_args)
         elif (method is None) or method == 'legacy':
             return self.integrateImageStack_legacy(img_stack)
         else:
             raise NotImplementedError(f'unsupported integration method {method}')
 
-
-    def loadPolyMask(self,maskpoints = [], **kwargs):
+    def loadPolyMask(self, maskpoints=[], **kwargs):
         '''
         loads a polygon mask from a list of polygon points
-        
+
         Args:
         (list) maskpoints: a list of lists of points, e.g.
                 [
                     [ #begin polygon 1
                         [0,0],[0,10],[10,10],[10,0]
                     ],
                     [ #later polygons]
                 ]
-        (tuple) maskshape: (x,y) dimensions of mask to create 
+        (tuple) maskshape: (x,y) dimensions of mask to create
                 if not passed, will assume that the maximum point is included in the mask
         '''
         points = maskpoints
         xs = []
         ys = []
         for polygon in points:
             x, y = zip(*polygon)
@@ -371,40 +448,39 @@
             ys += y
             if 'maskshape' in kwargs:
                 shape = kwargs['maskshape']
             else:
                 shape = (math.ceil(max(xs)), math.ceil(max(ys)))
             image = np.zeros(shape)
             for polygon in points:
-                 image += draw.polygon2mask(shape, polygon)
+                image += draw.polygon2mask(shape, polygon)
             image[image > 1] = 1
         boolmask = np.invert(image.astype(bool))
         print(f"Created mask with dimensions {str(np.shape(boolmask))}")
         self.mask = boolmask
 
     def loadImageMask(self, **kwargs):
         '''
         loads a mask from a generic image
-        
+
         Args:
             (pathlib.Path or String) maskpath: path to load
             (bool) maskrotate: rotate mask using np.flipud(np.rot90(mask))
         '''
 
         im = Image.open(kwargs['maskpath'])
         image = np.array(im)
         if 'maskrotate' in kwargs:
             if kwargs['maskrotate']:
                 image = np.flipud(np.rot90(image))
         boolmask = np.invert(image.astype(bool))
         print(f"Imported mask with dimensions {str(np.shape(boolmask))}")
         self.mask = boolmask
 
-    def loadNikaMask(self, filetoload, rotate_image = True,**kwargs):
-
+    def loadNikaMask(self, filetoload, rotate_image=True, **kwargs):
         '''
         Loads a Nika-generated HDF5 or tiff mask and converts it to an array that matches the local conventions.
 
         Args:
             filetoload (pathlib.Path or string): path to hdf5/tiff format mask from Nika.
             rotate_image (bool, default True): rotate image as should work
         '''
@@ -432,31 +508,31 @@
         Loads a mask json file saved by PyHyper's drawMask routines.
 
         Args:
             (pathlib.Path or string) maskpath: path to load json file from
 
 
         '''
-        with open(kwargs['maskpath'],'r') as f:
+        with open(kwargs['maskpath'], 'r') as f:
             strlist = json.load(f)
-        #print(strlist)
+        # print(strlist)
         dflist = []
         for item in strlist:
             dflist.append(pd.read_json(item))
-        #print(dflist)
+        # print(dflist)
         pyhyperlist = []
         for shape in dflist:
             pyhyper_shape = []
-            for index,xval in enumerate(shape.x):
+            for index, xval in enumerate(shape.x):
                 yval = shape.y[index]
-                pyhyper_shape.append([xval,yval])
+                pyhyper_shape.append([xval, yval])
             pyhyperlist.append(pyhyper_shape)
-        self.loadPolyMask(maskpoints=pyhyperlist,**kwargs)
-    def calibrationFromTemplateXRParams(self, raw_xr):
+        self.loadPolyMask(maskpoints=pyhyperlist, **kwargs)
 
+    def calibrationFromTemplateXRParams(self, raw_xr):
         '''
         Sets calibration from a pyFAI values in a template xarray
 
         Args:
             raw_xr (raw format xarray): a raw_xr bearing the metadata in members
 
         '''
@@ -465,19 +541,32 @@
         self.poni2 = raw_xr.poni2
 
         self.rot1 = raw_xr.rot1
         self.rot2 = raw_xr.rot2
         self.rot3 = raw_xr.rot3
 
         self.pixel1 = raw_xr.pixel1
-        self.pixel2 = raw_xr.pixel2
-        
+        self.pixel2 = raw_xr.pixel2        
+        try:
+            self.energy = float(raw_xr.energy)
+        except TypeError:
+            pass
+
         if self.mask is None:
-            self.mask = np.zeros((len(raw_xr.pix_y),len(raw_xr.pix_x)))
-            warnings.warn(f'Since mask was none, creating an empty mask with shape {self.mask.shape}',stacklevel=2)
+            self.mask = np.zeros((len(raw_xr.pix_y), len(raw_xr.pix_x)))
+            warnings.warn(
+                f'Since mask was none, creating an empty mask with shape {self.mask.shape}',
+                stacklevel=2,
+            )
+
+        if hasattr(raw_xr.energy, '__iter__'):  # this is an iterable, not a single number
+            self.energy = raw_xr.energy[0]
+        else:
+            self.energy = raw_xr.energy
+
         self.recreateIntegrator()
 
     @property
     def wavelength(self):
         return 1.239842e-6 / self._energy  # = wl ; energy = 1.239842e-6 / wl
 
     @wavelength.setter
@@ -495,28 +584,32 @@
         self.recreateIntegrator()
 
     @property
     def ni_beamcenter_x(self):
         try:
             return self.poni2 / self.ni_pixel_x * 1000
         except ZeroDivisionError:
-            warnings.warn('x pixel size is 0, cannot set beam center, fix pixel size first', stacklevel=2)
+            warnings.warn(
+                'x pixel size is 0, cannot set beam center, fix pixel size first', stacklevel=2
+            )
             return 0
 
     @ni_beamcenter_x.setter
     def ni_beamcenter_x(self, value):
         self.poni2 = self.ni_pixel_x * value / 1000
         self.recreateIntegrator()
 
     @property
     def ni_beamcenter_y(self):
         try:
             return self.poni1 / self.ni_pixel_y * 1000
         except ZeroDivisionError:
-            warnings.warn('y pixel size is 0, cannot set beam center, fix pixel size first', stacklevel=2)
+            warnings.warn(
+                'y pixel size is 0, cannot set beam center, fix pixel size first', stacklevel=2
+            )
             return 0
 
     @ni_beamcenter_y.setter
     def ni_beamcenter_y(self, value):
         self.poni1 = self.ni_pixel_y * value / 1000
         self.recreateIntegrator()
 
@@ -568,33 +661,41 @@
         self.recreateIntegrator()
 
     def recreateIntegrator(self):
         '''
         recreate the integrator, after geometry change
         '''
         self.integrator = azimuthalIntegrator.AzimuthalIntegrator(
-            self.dist, self.poni1, self.poni2, self.rot1, self.rot2, self.rot3, pixel1=self.pixel1, pixel2=self.pixel2,
-            wavelength=self.wavelength)
+            self.dist,
+            self.poni1,
+            self.poni2,
+            self.rot1,
+            self.rot2,
+            self.rot3,
+            pixel1=self.pixel1,
+            pixel2=self.pixel2,
+            wavelength=self.wavelength,
+        )
 
     def calibrationFromNikaParams(self, distance, bcx, bcy, tiltx, tilty, pixsizex, pixsizey):
         '''
-        DEPRECATED as of 0.2
+         DEPRECATED as of 0.2
 
-       Set the local calibrations using Nika parameters.
-           this will probably only support rotations in the SAXS limit (i.e., where sin(x) ~ x, i.e., a couple degrees)
-           since it assumes the PyFAI and Nika rotations are about the same origin point (which I think isn't true).
-
-        Args:
-            distance: sample-detector distance in mm
-            bcx: beam center x in pixels
-            bcy: beam center y in pixels
-            tiltx: detector x tilt in deg, see note above
-            tilty: detector y tilt in deg, see note above
-            pixsizex: pixel size in x, microns
-            pixsizey: pixel size in y, microns
+        Set the local calibrations using Nika parameters.
+            this will probably only support rotations in the SAXS limit (i.e., where sin(x) ~ x, i.e., a couple degrees)
+            since it assumes the PyFAI and Nika rotations are about the same origin point (which I think isn't true).
+
+         Args:
+             distance: sample-detector distance in mm
+             bcx: beam center x in pixels
+             bcy: beam center y in pixels
+             tiltx: detector x tilt in deg, see note above
+             tilty: detector y tilt in deg, see note above
+             pixsizex: pixel size in x, microns
+             pixsizey: pixel size in y, microns
         '''
 
         self.ni_pixel_x = pixsizex
         self.ni_pixel_y = pixsizey
         self.ni_distance = distance
         self.ni_beamcenter_x = bcx
         self.ni_beamcenter_y = bcy
```

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/PlotTools.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/PlotTools.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/RSoXS.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/RSoXS.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/SMIRSoXSLoader.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/SMIRSoXSLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/SST1RSoXSDB.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/SST1RSoXSDB.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import scipy.ndimage
 import asyncio
 import time
 import copy
 
 try:
     os.environ["TILED_SITE_PROFILES"] = "/nsls2/software/etc/tiled/profiles"
-    from tiled.client import from_profile
+    from tiled.client import from_profile,from_uri
     from httpx import HTTPStatusError
     import tiled
     import dask
     from databroker.queries import RawMongo, Key, FullText, Contains, Regex
 except Exception:
     print(
         "Imports failed.  Are you running on a machine with proper libraries for databroker,"
@@ -62,25 +62,27 @@
         dark_subtract=True,
         dark_pedestal=0,
         exposure_offset=0,
         catalog=None,
         catalog_kwargs={},
         use_precise_positions=False,
         use_chunked_loading=False,
+        suppress_time_dimension=True,
     ):
         """
         Args:
             corr_mode (str): origin to use for the intensity correction.  Can be 'expt','i0','expt+i0','user_func','old',or 'none'
             user_corr_func (callable): takes the header dictionary and returns the value of the correction.
             dark_pedestal (numeric): value to add to the whole image before doing dark subtraction, to avoid non-negative values.
             exposure_offset (numeric): value to add to the exposure time.
             catalog (DataBroker Catalog): overrides the internally-set-up catalog with a version you provide
             catalog_kwargs (dict): kwargs to be passed to a from_profile catalog generation script.  For example, you can ask for Dask arrays here.
             use_precise_positions (bool): if False, rounds sam_x and sam_y to 1 digit.  If True, keeps default rounding (4 digits).  Needed for spiral scans to work with readback positions.
             use_chunked_loading (bool): if True, returns Dask backed arrays for further Dask processing.  if false, behaves in conventional Numpy-backed way
+            suppress_time_dimension (bool): if True, time is never a dimension that you want in your data and will be dropped (default).  if False, time will be a dimension in almost every scan.
         """
 
         if corr_mode == None:
             warnings.warn(
                 "Correction mode was not set, not performing *any* intensity corrections.  Are you"
                 " sure this is "
                 + "right? Set corr_mode to 'none' to suppress this warning.",
@@ -89,15 +91,19 @@
             self.corr_mode = "none"
         else:
             self.corr_mode = corr_mode
         if use_chunked_loading:
             catalog_kwargs["structure_clients"] = "dask"
         self.use_chunked_loading = use_chunked_loading
         if catalog is None:
-            self.c = from_profile("rsoxs", **catalog_kwargs)
+            try:
+                self.c = from_profile("rsoxs", **catalog_kwargs)
+            except tiled.profiles.ProfileNotFound:
+                print('could not directly connect to Tiled using a system profile.\n  Making network connection.\n  Enter your BNL credentials now or pass an api key like catalog_kwargs={"api_key":"..."}.')
+                self.c = from_uri('https://tiled.nsls2.bnl.gov',**catalog_kwargs)['rsoxs']['raw']
         else:
             self.c = catalog
             if use_chunked_loading:
                 raise SyntaxError(
                     "use_chunked_loading is incompatible with externally supplied catalog.  when"
                     ' creating the catalog, pass structure_clients = "dask" as a kwarg.'
                 )
@@ -106,14 +112,15 @@
                     "catalog_kwargs is incompatible with externally supplied catalog.  pass those"
                     " kwargs to whoever gave you the catalog you passed in."
                 )
         self.dark_subtract = dark_subtract
         self.dark_pedestal = dark_pedestal
         self.exposure_offset = exposure_offset
         self.use_precise_positions = use_precise_positions
+        self.suppress_time_dimension = suppress_time_dimension
 
     # def loadFileSeries(self,basepath):
     #     try:
     #         flist = list(basepath.glob('*primary*.tiff'))
     #     except AttributeError:
     #         basepath = pathlib.Path(basepath)
     #         flist = list(basepath.glob('*primary*.tiff'))
@@ -279,36 +286,36 @@
         reducedCatalog = bsCatalog
         for _, searchSeries in tqdm(
             df_SearchDet.iterrows(), total=df_SearchDet.shape[0], desc="Running catalog search..."
         ):
             # Skip arguments with value None, and quits if the catalog was reduced to 0 elements
             if (searchSeries[1] is not None) and (len(reducedCatalog) > 0):
                 # For numeric entries, do Key equality
-                if "numeric" in str(searchSeries[2]):
+                if "numeric" in str(searchSeries.iloc[2]):
                     reducedCatalog = reducedCatalog.search(
-                        Key(searchSeries[0]) == float(searchSeries[1])
+                        Key(searchSeries.iloc[0]) == float(searchSeries.iloc[1])
                     )
 
                 else:  # Build regex search string
                     reg_prefix = ""
                     reg_postfix = ""
 
                     # Regex cheatsheet:
                     # (?i) is case insensitive
                     # ^_$ forces exact match to _, ^ anchors the start, $ anchors the end
-                    if "case-insensitive" in str(searchSeries[2]):
+                    if "case-insensitive" in str(searchSeries.iloc[2]):
                         reg_prefix += "(?i)"
-                    if "exact" in searchSeries[2]:
+                    if "exact" in searchSeries.iloc[2]:
                         reg_prefix += "^"
                         reg_postfix += "$"
 
-                    regexString = reg_prefix + str(searchSeries[1]) + reg_postfix
+                    regexString = reg_prefix + str(searchSeries.iloc[1]) + reg_postfix
 
                     # Search/reduce the catalog
-                    reducedCatalog = reducedCatalog.search(Regex(searchSeries[0], regexString))
+                    reducedCatalog = reducedCatalog.search(Regex(searchSeries.iloc[0], regexString))
 
                 # If a match fails, notify the user which search parameter yielded 0 results
                 if len(reducedCatalog) == 0:
                     warnString = (
                         f"Catalog reduced to zero when attempting to match {searchSeries}\n"
                         + f"If this is a user-provided search parameter, check spelling/syntax."
                     )
@@ -560,19 +567,19 @@
             CHANGE: List of dimensions you'd like. If not set, will set all possibilities as dimensions (x, y, theta, energy, polarization)
             coords (dict): user-supplied dimensions, see syntax examples in documentation.
             return_dataset (bool,default False): return both the data and the monitors as a xr.dataset.  If false (default), just returns the data.
         Returns:
             raw (xarray): raw xarray containing your scan in PyHyper-compliant format
 
         """
-        if type(run) is int:
+        if isinstance(run,int):
             run = self.c[run]
-        elif type(run) is pd.DataFrame:
+        elif isinstance(run,pd.DataFrame):
             run = list(run.scan_id)
-        if type(run) is list:
+        if isinstance(run,list):
             return self.loadSeries(
                 run,
                 "sample_name",
                 loadrun_kwargs={
                     "dims": dims,
                     "coords": coords,
                     "return_dataset": return_dataset,
@@ -598,38 +605,47 @@
             elif "spiralsearch" in md["start"]["plan_name"] and dims is None:
                 dims = ["sam_x", "sam_y"]
             elif "count" in md["start"]["plan_name"] and dims is None:
                 dims = ["epoch"]
             else:
                 axes_to_include = []
                 rsd_cutoff = 0.005
-
+            
                 # begin with a list of the things that are primary streams
                 axis_list = list(run["primary"]["data"].keys())
+                
                 # next, knock out anything that has 'image', 'fullframe' in it - these aren't axes
                 axis_list = [x for x in axis_list if "image" not in x]
                 axis_list = [x for x in axis_list if "fullframe" not in x]
                 axis_list = [x for x in axis_list if "stats" not in x]
                 axis_list = [x for x in axis_list if "saturated" not in x]
                 axis_list = [x for x in axis_list if "under_exposed" not in x]
+                
                 # knock out any known names of scalar counters
                 axis_list = [x for x in axis_list if "Beamstop" not in x]
                 axis_list = [x for x in axis_list if "Current" not in x]
 
+                if self.suppress_time_dimension:
+                    axis_list = [x for x in axis_list if x != "time"]
+
                 # now, clean up duplicates.
                 axis_list = [x for x in axis_list if "setpoint" not in x]
                 # now, figure out what's actually moving.  we use a relative standard deviation to do this.
                 # arbitrary cutoff of 0.5% motion = it moved intentionally.
                 for axis in axis_list:
                     std = np.std(run["primary"]["data"][axis])
-                    mean = np.mean(run["primary"]["data"][axis])
-                    rsd = std / mean
-
+                    motion = np.abs(np.max(run["primary"]["data"][axis])-np.min(run["primary"]["data"][axis]))
+                    if motion == 0:
+                        rsd = 0
+                    else:
+                        rsd = std / motion
+                    #print(f'Evaluating {axis} for inclusion as a dimension with rsd {rsd}...')
                     if rsd > rsd_cutoff:
                         axes_to_include.append(axis)
+                        #print(f'    --> it was included')
 
                 # next, construct the reverse lookup table - best mapping we can make of key to pyhyper word
                 # we start with the lookup table used by loadMd()
                 reverse_lut = {v: k for k, v in self.md_lookup.items()}
                 reverse_lut_secondary = {v: k for k, v in self.md_secondary_lookup.items()}
                 reverse_lut.update(reverse_lut_secondary)
 
@@ -673,23 +689,19 @@
                 if dims[i] == 'energy':
                     dims[i] = 'en_energy'
             if len(dims) == 0:
                 raise NotImplementedError('You have not entered any dimensions; please enter at least one, or use None rather than an empty list')
         """
 
         data = run["primary"]["data"][md["detector"] + "_image"]
-        if (
-            type(data) == tiled.client.array.ArrayClient
-            or type(data) == tiled.client.array.DaskArrayClient
-        ):
+        if isinstance(data,tiled.client.array.ArrayClient):
+            data = run["primary"]["data"].read()[md["detector"] + "_image"]
+        elif isinstance(data,tiled.client.array.DaskArrayClient):
             data = run["primary"]["data"].read()[md["detector"] + "_image"]
-        elif type(data) == tiled.client.array.DaskArrayClient:
-            data = xr.DataArray(
-                data.read(), dims=data.dims
-            )  # xxx hack!  Really should use tiled structure_clients xarraydaskclient here.
+        
         data = data.astype(int)  # convert from uint to handle dark subtraction
 
         if self.dark_subtract:
             dark = run["dark"]["data"][md["detector"] + "_image"]
             if (
                 type(dark) == tiled.client.array.ArrayClient
                 or type(dark) == tiled.client.array.DaskArrayClient
@@ -699,15 +711,15 @@
             for n, time in enumerate(dark.time):
                 darkframe[(data.time - time) > 0] = int(n)
             data = data.assign_coords(dark_id=("time", darkframe))
 
             def subtract_dark(img, pedestal=100, darks=None):
                 return img + pedestal - darks[int(img.dark_id.values)]
 
-            data = data.groupby("time").map(subtract_dark, darks=dark, pedestal=self.dark_pedestal)
+            data = data.groupby("time",squeeze=False).map(subtract_dark, darks=dark, pedestal=self.dark_pedestal)
 
         dims_to_join = []
         dim_names_to_join = []
 
         for dim in dims:
             try:
                 test = len(md[dim])  # this will throw a typeerror if single value
@@ -725,19 +737,20 @@
             dim_names_to_join.append(key)
 
         index = pd.MultiIndex.from_arrays(dims_to_join, names=dim_names_to_join)
         # handle the edge case of a partly-finished scan
         if len(index) != len(data["time"]):
             index = index[: len(data["time"])]
         actual_exposure = md["exposure"] * len(data.dim_0)
+        mindex_coords = xr.Coordinates.from_pandas_multiindex(index, 'system')
         retxr = (
             data.sum("dim_0")
             .rename({"dim_1": "pix_y", "dim_2": "pix_x"})
             .rename({"time": "system"})
-            .assign_coords(system=index)
+            .assign_coords(mindex_coords)
         )  # ,md['detector']+'_image':'intensity'})
 
         # this is needed for holoviews compatibility, hopefully does not break other features.
         retxr = retxr.assign_coords(
             {
                 "pix_x": np.arange(0, len(retxr.pix_x)),
                 "pix_y": np.arange(0, len(retxr.pix_y)),
@@ -768,15 +781,15 @@
         )  # patch for multi exposures
         # now do corrections:
         frozen_attrs = retxr.attrs
         if self.corr_mode == "i0":
             retxr = retxr / monitors["RSoXS Au Mesh Current"]
         elif self.corr_mode != "none":
             warnings.warn(
-                "corrections other than none are not supported at the moment",
+                "corrections other than none or i0 are not supported at the moment",
                 stacklevel=2,
             )
 
         retxr.attrs.update(frozen_attrs)
 
         # deal with the edge case where the LAST energy of a run is repeated... this may need modification to make it correct (did the energies shift when this happened??)
         try:
```

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/SST1RSoXSLoader.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/SST1RSoXSLoader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,32 @@
 import xarray as xr
 import pandas as pd
 import datetime
 import warnings
 import json
 #from pyFAI import azimuthalIntegrator
 import numpy as np
+try:
+    import dask.array as da
+except ImportError:
+    print('Could not import Dask.  Chunked loading may not work.  Install Dask or pyhyperscattering[performance] if this is desired.')
+
 
 
 class SST1RSoXSLoader(FileLoader):
     '''
     Loader for TIFF files from NSLS-II SST1 RSoXS instrument
 
     '''
     file_ext = '(.*?)primary(.*?).tiff'
     md_loading_is_quick = True
     pix_size_1 = 0.06
     pix_size_2 = 0.06
 
-    def __init__(self,corr_mode=None,user_corr_func=None,dark_pedestal=100,exposure_offset=0,constant_md={},):
+    def __init__(self,corr_mode=None,user_corr_func=None,dark_pedestal=100,exposure_offset=0,constant_md={},use_chunked_loading=False):
         '''
         Args:
             corr_mode (str): origin to use for the intensity correction.  Can be 'expt','i0','expt+i0','user_func','old',or 'none'
             user_corr_func (callable): takes the header dictionary and returns the value of the correction.
             dark_pedestal (numeric): value to subtract(/add, if negative) to the whole image.  this should match the instrument setting for suitcased tiffs, typically 100.
             exposure_offset (numeric): value to add to the exposure time.  Measured at 2ms with the piezo shutter in Dec 2019 by Jacob Thelen, NIST
             constant_md (dict): values to insert into every metadata load. 
@@ -40,14 +45,15 @@
 
 
         self.constant_md = constant_md
 
         self.dark_pedestal = dark_pedestal
         self.user_corr_func = user_corr_func
         self.exposure_offset = exposure_offset
+        self.use_chunked_loading = use_chunked_loading
         # self.darks = {}
     # def loadFileSeries(self,basepath):
     #     try:
     #         flist = list(basepath.glob('*primary*.tiff'))
     #     except AttributeError:
     #         basepath = pathlib.Path(basepath)
     #         flist = list(basepath.glob('*primary*.tiff'))
@@ -76,15 +82,19 @@
         if len(kwargs.keys())>0:
             warnings.warn(f'Loader does not support features for kwargs: {kwargs.keys()}',stacklevel=2)
         
         if image_slice != None:
             raise NotImplementedError('Image slicing is not supported for SST1')
         if use_cached_md != False:
             raise NotImplementedError('Caching of metadata is not supported for SST1')
-        img = Image.open(filepath)
+            
+        img = np.array(Image.open(filepath))
+        
+        if self.use_chunked_loading:
+            img = da.from_array(img, chunks='auto')
 
         headerdict = self.loadMd(filepath)
         # two steps in this pre-processing stage:
         #     (1) get and apply the right scalar correction term to the image
         #     (2) find and subtract the right dark
         if coords != None:
             headerdict.update(coords)
@@ -108,19 +118,19 @@
         if(corr<0):
             warnings.warn(f'Correction value is negative: {corr} with headers {headerdict}.',stacklevel=2)
             corr = abs(corr)
 
 
         # # step 2: dark subtraction
         # this is already done in the suitcase, but we offer the option to add/subtract a pedestal.
-        image_data = (np.array(img)-self.dark_pedestal)/corr
+        image_data = (img-self.dark_pedestal)/corr
         if return_q:
             qpx = 2*np.pi*60e-6/(headerdict['sdd']/1000)/(headerdict['wavelength']*1e10)
-            qx = (np.arange(1,img.size[0]+1)-headerdict['beamcenter_y'])*qpx
-            qy = (np.arange(1,img.size[1]+1)-headerdict['beamcenter_x'])*qpx
+            qx = (np.arange(1,img.shape[1]+1)-headerdict['beamcenter_y'])*qpx
+            qy = (np.arange(1,img.shape[0]+1)-headerdict['beamcenter_x'])*qpx
             # now, match up the dims and coords
             return xr.DataArray(image_data,dims=['qy','qx'],coords={'qy':qy,'qx':qx},attrs=headerdict)
         else:
             # dim order changed by ktoth17 to reflect SST1RSoXSDB.py. See Issue #34 for more details. 
             return xr.DataArray(image_data,dims=['pix_y','pix_x'],attrs=headerdict)
 
     def read_json(self,jsonfile):
```

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/WPIntegrator.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/WPIntegrator.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering/cyrsoxsLoader.py` & `PyHyperScattering-0.2.3/src/PyHyperScattering/cyrsoxsLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering.egg-info/PKG-INFO` & `PyHyperScattering-0.2.3/src/PyHyperScattering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyHyperScattering
-Version: 0.2.2
+Version: 0.2.3
 Summary: Utilities for loading, reducing, fitting, and plotting hyperspectral x-ray and neutron scattering data.
 Home-page: https://github.com/usnistgov/pyhyperscattering
 Author: Peter Beaucage
 Author-email: peter.beaucage@nist.gov
 Project-URL: Github, https://github.com/usnistgov/pyhyperscattering
 Project-URL: Project Site, https://www.nist.gov/laboratories/tools-instruments/polarized-resonant-soft-x-ray-scattering-p-rsoxs
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyHyperScattering-0.2.2/src/PyHyperScattering.egg-info/SOURCES.txt` & `PyHyperScattering-0.2.3/src/PyHyperScattering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/tests/test_11012Loader.py` & `PyHyperScattering-0.2.3/tests/test_11012Loader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/tests/test_PFIntegrators.py` & `PyHyperScattering-0.2.3/tests/test_PFIntegrators.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/tests/test_RSoXS.py` & `PyHyperScattering-0.2.3/tests/test_RSoXS.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/tests/test_SMILoader.py` & `PyHyperScattering-0.2.3/tests/test_SMILoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/tests/test_SST1DBLoader.py` & `PyHyperScattering-0.2.3/tests/test_SST1DBLoader.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,32 +5,41 @@
     import tiled
     import tiled.client
     try:
         client = tiled.client.from_profile('rsoxs')
         from PyHyperScattering.load import SST1RSoXSDB
         SKIP_DB_TESTING=False
     except tiled.profiles.ProfileNotFound:
-        SKIP_DB_TESTING=True
+        try:
+            client = tiled.client.from_uri('https://tiled-demo.blueskyproject.io')
+            SKIP_DB_TESTING=True # waiting on test data to be posted to this server
+        except Exception:
+            SKIP_DB_TESTING=True
 except ImportError:
     SKIP_DB_TESTING=True
 
 
 
     
 import numpy as np
 import pandas as pd
 import xarray as xr
 import pytest
+from PyHyperScattering.load import SST1RSoXSDB
 
 must_have_tiled = pytest.mark.skipif(SKIP_DB_TESTING,reason='Connection to Tiled server not possible in this environment.')
 
 
 @pytest.fixture(autouse=True,scope='module')
 def sstdb():
-    sstdb = SST1RSoXSDB(corr_mode='none')
+    try:
+        catalog = tiled.client.from_profile('rsoxs')
+    except tiled.profiles.ProfileNotFound:
+        catalog = tiled.client.from_uri('https://tiled-demo.blueskyproject.io')['rsoxs']['raw']
+    sstdb = SST1RSoXSDB(catalog=catalog,corr_mode='none')
     return sstdb
 
 @must_have_tiled
 def test_SST1DB_load_single_scan_legacy_hinted_dims(sstdb):
     run = sstdb.loadRun(21792).unstack('system')
     assert 'energy' in run.indexes
```

### Comparing `PyHyperScattering-0.2.2/tests/test_SST1Loader.py` & `PyHyperScattering-0.2.3/tests/test_SST1Loader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/tests/test_WPintegrator.py` & `PyHyperScattering-0.2.3/tests/test_WPintegrator.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/tests/test_cyrsoxsLoader.py` & `PyHyperScattering-0.2.3/tests/test_cyrsoxsLoader.py`

 * *Files identical despite different names*

### Comparing `PyHyperScattering-0.2.2/versioneer.py` & `PyHyperScattering-0.2.3/versioneer.py`

 * *Files identical despite different names*

