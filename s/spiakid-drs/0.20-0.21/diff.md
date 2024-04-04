# Comparing `tmp/spiakid-drs-0.20.tar.gz` & `tmp/spiakid-drs-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiakid-drs-0.20.tar", last modified: Thu Apr  4 14:08:14 2024, max compression
+gzip compressed data, was "spiakid-drs-0.21.tar", last modified: Thu Apr  4 14:27:55 2024, max compression
```

## Comparing `spiakid-drs-0.20.tar` & `spiakid-drs-0.21.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10173 2023-08-28 11:01:43.000000 spiakid-drs-0.20/LICENSE
--rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1788 2024-04-04 14:08:14.580998 spiakid-drs-0.20/PKG-INFO
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2552 2023-08-28 11:01:43.000000 spiakid-drs-0.20/README.md
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1262 2023-08-28 11:01:43.000000 spiakid-drs-0.20/README_for_pip.md
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      575 2024-04-04 14:07:10.000000 spiakid-drs-0.20/pyproject.toml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-04-04 14:08:14.580998 spiakid-drs-0.20/setup.cfg
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/spiakid_DRS/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      903 2024-03-28 13:08:26.000000 spiakid-drs-0.20/spiakid_DRS/Home.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/spiakid_DRS/SpectralRes/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      694 2024-03-25 15:07:20.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/Data.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12205 2024-04-04 14:03:28.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/Detect.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5343 2024-04-04 14:03:59.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/IQCalibration.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4293 2024-04-04 14:03:53.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/Plot.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-08-28 11:01:43.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/__init__.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    11983 2024-03-25 15:07:20.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/cmplxIQ.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10726 2024-04-04 14:03:45.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/fun.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    48462 2024-03-25 15:07:19.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/resonator.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    19391 2024-04-04 14:04:08.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/utility.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-08-28 11:01:43.000000 spiakid-drs-0.20/spiakid_DRS/__init__.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1065 2024-03-28 13:07:57.000000 spiakid-drs-0.20/spiakid_DRS/inter.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/spiakid_DRS/pages/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2682 2024-04-04 14:04:24.000000 spiakid-drs-0.20/spiakid_DRS/pages/Recons_inter.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2826 2024-04-04 14:04:16.000000 spiakid-drs-0.20/spiakid_DRS/pages/SpecRes.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2392 2024-04-04 14:02:46.000000 spiakid-drs-0.20/spiakid_DRS/recons_inter.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/spiakid_drs.egg-info/
--rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1788 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/PKG-INFO
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      717 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/SOURCES.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/dependency_links.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       37 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/requires.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       12 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/top_level.txt
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/tests/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      159 2023-08-28 11:01:43.000000 spiakid-drs-0.20/tests/test_prototype.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:27:55.864654 spiakid-drs-0.21/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10173 2023-08-28 11:01:43.000000 spiakid-drs-0.21/LICENSE
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1788 2024-04-04 14:27:55.864654 spiakid-drs-0.21/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2552 2023-08-28 11:01:43.000000 spiakid-drs-0.21/README.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1262 2023-08-28 11:01:43.000000 spiakid-drs-0.21/README_for_pip.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      575 2024-04-04 14:27:11.000000 spiakid-drs-0.21/pyproject.toml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-04-04 14:27:55.864654 spiakid-drs-0.21/setup.cfg
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:27:55.864654 spiakid-drs-0.21/spiakid_DRS/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      903 2024-03-28 13:08:26.000000 spiakid-drs-0.21/spiakid_DRS/Home.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:27:55.864654 spiakid-drs-0.21/spiakid_DRS/SpectralRes/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      694 2024-03-25 15:07:20.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/Data.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12205 2024-04-04 14:03:28.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/Detect.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5343 2024-04-04 14:03:59.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/IQCalibration.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4293 2024-04-04 14:03:53.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/Plot.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-08-28 11:01:43.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/__init__.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    11983 2024-03-25 15:07:20.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/cmplxIQ.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10726 2024-04-04 14:03:45.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/fun.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    48462 2024-03-25 15:07:19.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/resonator.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    19391 2024-04-04 14:04:08.000000 spiakid-drs-0.21/spiakid_DRS/SpectralRes/utility.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-08-28 11:01:43.000000 spiakid-drs-0.21/spiakid_DRS/__init__.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1077 2024-04-04 14:25:40.000000 spiakid-drs-0.21/spiakid_DRS/inter.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:27:55.864654 spiakid-drs-0.21/spiakid_DRS/pages/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2682 2024-04-04 14:04:24.000000 spiakid-drs-0.21/spiakid_DRS/pages/Recons_inter.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2826 2024-04-04 14:04:16.000000 spiakid-drs-0.21/spiakid_DRS/pages/SpecRes.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2264 2024-04-04 14:26:18.000000 spiakid-drs-0.21/spiakid_DRS/recons_inter.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:27:55.864654 spiakid-drs-0.21/spiakid_drs.egg-info/
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1788 2024-04-04 14:27:55.000000 spiakid-drs-0.21/spiakid_drs.egg-info/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      717 2024-04-04 14:27:55.000000 spiakid-drs-0.21/spiakid_drs.egg-info/SOURCES.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-04-04 14:27:55.000000 spiakid-drs-0.21/spiakid_drs.egg-info/dependency_links.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       37 2024-04-04 14:27:55.000000 spiakid-drs-0.21/spiakid_drs.egg-info/requires.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       12 2024-04-04 14:27:55.000000 spiakid-drs-0.21/spiakid_drs.egg-info/top_level.txt
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:27:55.864654 spiakid-drs-0.21/tests/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      159 2023-08-28 11:01:43.000000 spiakid-drs-0.21/tests/test_prototype.py
```

### Comparing `spiakid-drs-0.20/LICENSE` & `spiakid-drs-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/PKG-INFO` & `spiakid-drs-0.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-drs
-Version: 0.20
+Version: 0.21
 Summary: Data Reduction System of SPIAKID project
 Author-email: Pasquale Panuzzo <pasquale.panuzzo@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/DRS/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `spiakid-drs-0.20/README.md` & `spiakid-drs-0.21/README.md`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/README_for_pip.md` & `spiakid-drs-0.21/README_for_pip.md`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/pyproject.toml` & `spiakid-drs-0.21/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spiakid-drs"
-version = "0.20"
+version = "0.21"
 authors = [
   { name="Pasquale Panuzzo", email="pasquale.panuzzo@gmail.com" },
 ]
 description = "Data Reduction System of SPIAKID project"
 readme = "README_for_pip.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `spiakid-drs-0.20/spiakid_DRS/Home.py` & `spiakid-drs-0.21/spiakid_DRS/Home.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/SpectralRes/Data.py` & `spiakid-drs-0.21/spiakid_DRS/SpectralRes/Data.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/SpectralRes/Detect.py` & `spiakid-drs-0.21/spiakid_DRS/SpectralRes/Detect.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/SpectralRes/IQCalibration.py` & `spiakid-drs-0.21/spiakid_DRS/SpectralRes/IQCalibration.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/SpectralRes/Plot.py` & `spiakid-drs-0.21/spiakid_DRS/SpectralRes/Plot.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/SpectralRes/cmplxIQ.py` & `spiakid-drs-0.21/spiakid_DRS/SpectralRes/cmplxIQ.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/SpectralRes/fun.py` & `spiakid-drs-0.21/spiakid_DRS/SpectralRes/fun.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/SpectralRes/resonator.py` & `spiakid-drs-0.21/spiakid_DRS/SpectralRes/resonator.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/SpectralRes/utility.py` & `spiakid-drs-0.21/spiakid_DRS/SpectralRes/utility.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/inter.py` & `spiakid-drs-0.21/spiakid_DRS/inter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from SpectralRes import Detect as D
+from spiakid_DRS.SpectralRes import Detect as D
 import os
 import argparse
 from pathlib import Path
 import pathlib
 
 """
 Link between Terminal and pipeline
```

### Comparing `spiakid-drs-0.20/spiakid_DRS/pages/Recons_inter.py` & `spiakid-drs-0.21/spiakid_DRS/pages/Recons_inter.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/pages/SpecRes.py` & `spiakid-drs-0.21/spiakid_DRS/pages/SpecRes.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.20/spiakid_DRS/recons_inter.py` & `spiakid-drs-0.21/spiakid_DRS/recons_inter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import spiakid_DRS.SpectralRes.Data as Dt
 import numpy as np
 from tkinter import *
 from matplotlib.figure import Figure
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
-from matplotlib.backends.backend_tkagg import NavigationToolbar2Tk
+
 
 
 def interface(data_file):
 
     def plot_recons(event):
         time = int(var.get())
         Text['text'] = str(t[time]) + ' s'
@@ -34,16 +34,15 @@
         for j in range(num):
             pix = data['Photons'][str(i)+'_'+str(j)]
             if len(pix[0]) > 0:
                 mini.append(min(pix[1]))
                 maxi.append(max(pix[1]))
     maxi = max(maxi)
     mini = min(mini)
-    E_range = maxi-mini
-    E_bins = np.linspace(mini,maxi,10)
+
     time_bins = int(obs_time/time_step)
     t = np.arange(0,time_bins,time_step)
     ph = np.zeros(shape = (num,num), dtype=object)
     for i in range(num):
         for j in range(num):
             pix = data['Photons'][str(i)+'_'+str(j)]
             H,b = np.histogram(pix[0],bins = time_bins)
```

### Comparing `spiakid-drs-0.20/spiakid_drs.egg-info/PKG-INFO` & `spiakid-drs-0.21/spiakid_drs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-drs
-Version: 0.20
+Version: 0.21
 Summary: Data Reduction System of SPIAKID project
 Author-email: Pasquale Panuzzo <pasquale.panuzzo@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/DRS/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `spiakid-drs-0.20/spiakid_drs.egg-info/SOURCES.txt` & `spiakid-drs-0.21/spiakid_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

