# Comparing `tmp/spiakid-drs-0.11.tar.gz` & `tmp/spiakid-drs-0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiakid-drs-0.11.tar", last modified: Tue Apr 18 13:50:55 2023, max compression
+gzip compressed data, was "spiakid-drs-0.20.tar", last modified: Thu Apr  4 14:08:14 2024, max compression
```

## Comparing `spiakid-drs-0.11.tar` & `spiakid-drs-0.20.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.471867 spiakid-drs-0.11/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    10173 2023-03-15 14:15:26.000000 spiakid-drs-0.11/LICENSE
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1676 2023-04-18 13:50:55.471867 spiakid-drs-0.11/PKG-INFO
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     2552 2023-03-15 14:15:26.000000 spiakid-drs-0.11/README.md
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1262 2023-03-15 14:15:26.000000 spiakid-drs-0.11/README_for_pip.md
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      580 2023-04-18 13:49:31.000000 spiakid-drs-0.11/pyproject.toml
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       38 2023-04-18 13:50:55.471867 spiakid-drs-0.11/setup.cfg
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.463867 spiakid-drs-0.11/src/
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.467867 spiakid-drs-0.11/src/Functions/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1926 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/Data.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     5329 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/IQCalibration.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     3105 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/Modelisation.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     9399 2023-04-18 13:48:18.000000 spiakid-drs-0.11/src/Functions/Pixel.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     4915 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/Plot.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     7577 2023-04-18 13:48:18.000000 spiakid-drs-0.11/src/Functions/Pulse_Timeline.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     3331 2023-04-18 13:48:18.000000 spiakid-drs-0.11/src/Functions/Pulse_average.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        0 2023-03-15 14:15:26.000000 spiakid-drs-0.11/src/Functions/__init__.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    11983 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/cmplxIQ.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    48462 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/resonator.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)    11933 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Functions/utility.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1906 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/Interface.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        0 2023-03-15 14:15:26.000000 spiakid-drs-0.11/src/__init__.py
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1466 2023-04-18 08:42:51.000000 spiakid-drs-0.11/src/prototype.py
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.471867 spiakid-drs-0.11/src/spiakid_drs.egg-info/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)     1676 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/PKG-INFO
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      612 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/SOURCES.txt
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)        1 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/dependency_links.txt
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       40 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/requires.txt
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)       39 2023-04-18 13:50:55.000000 spiakid-drs-0.11/src/spiakid_drs.egg-info/top_level.txt
-drwxrwxr-x   0 sfaes     (1000) sfaes     (1000)        0 2023-04-18 13:50:55.471867 spiakid-drs-0.11/tests/
--rw-rw-r--   0 sfaes     (1000) sfaes     (1000)      159 2023-03-15 14:15:26.000000 spiakid-drs-0.11/tests/test_prototype.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10173 2023-08-28 11:01:43.000000 spiakid-drs-0.20/LICENSE
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1788 2024-04-04 14:08:14.580998 spiakid-drs-0.20/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2552 2023-08-28 11:01:43.000000 spiakid-drs-0.20/README.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1262 2023-08-28 11:01:43.000000 spiakid-drs-0.20/README_for_pip.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      575 2024-04-04 14:07:10.000000 spiakid-drs-0.20/pyproject.toml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-04-04 14:08:14.580998 spiakid-drs-0.20/setup.cfg
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/spiakid_DRS/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      903 2024-03-28 13:08:26.000000 spiakid-drs-0.20/spiakid_DRS/Home.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/spiakid_DRS/SpectralRes/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      694 2024-03-25 15:07:20.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/Data.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12205 2024-04-04 14:03:28.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/Detect.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5343 2024-04-04 14:03:59.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/IQCalibration.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4293 2024-04-04 14:03:53.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/Plot.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-08-28 11:01:43.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/__init__.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    11983 2024-03-25 15:07:20.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/cmplxIQ.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10726 2024-04-04 14:03:45.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/fun.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    48462 2024-03-25 15:07:19.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/resonator.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    19391 2024-04-04 14:04:08.000000 spiakid-drs-0.20/spiakid_DRS/SpectralRes/utility.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-08-28 11:01:43.000000 spiakid-drs-0.20/spiakid_DRS/__init__.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1065 2024-03-28 13:07:57.000000 spiakid-drs-0.20/spiakid_DRS/inter.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/spiakid_DRS/pages/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2682 2024-04-04 14:04:24.000000 spiakid-drs-0.20/spiakid_DRS/pages/Recons_inter.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2826 2024-04-04 14:04:16.000000 spiakid-drs-0.20/spiakid_DRS/pages/SpecRes.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2392 2024-04-04 14:02:46.000000 spiakid-drs-0.20/spiakid_DRS/recons_inter.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/spiakid_drs.egg-info/
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1788 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      717 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/SOURCES.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/dependency_links.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       37 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/requires.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       12 2024-04-04 14:08:14.000000 spiakid-drs-0.20/spiakid_drs.egg-info/top_level.txt
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-04-04 14:08:14.580998 spiakid-drs-0.20/tests/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      159 2023-08-28 11:01:43.000000 spiakid-drs-0.20/tests/test_prototype.py
```

### Comparing `spiakid-drs-0.11/LICENSE` & `spiakid-drs-0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.11/PKG-INFO` & `spiakid-drs-0.20/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: spiakid-drs
-Version: 0.11
+Version: 0.20
 Summary: Data Reduction System of SPIAKID project
 Author-email: Pasquale Panuzzo <pasquale.panuzzo@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/DRS/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dynaconf
+Requires-Dist: h5py
+Requires-Dist: scraps
+Requires-Dist: lmfit
+Requires-Dist: streamlit
 
 # Data Reduction System of SPIAKID
 
 This project contains the **Data Reduction System** (DRS) of SPIAKID.
 
 The **SPIAKID** (SpectroPhotometric Imaging in Astronomy with Kinetic Inductance Detectors) project aims at designing, building and deploying on the sky a spectrophotometric imager based on Kinetic Inductance detectors. More information can be found on the [SPIAKID project homepage](https://www.observatoiredeparis.psl.eu/spiakid.html).
```

### Comparing `spiakid-drs-0.11/README.md` & `spiakid-drs-0.20/README.md`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.11/README_for_pip.md` & `spiakid-drs-0.20/README_for_pip.md`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.11/src/Functions/IQCalibration.py` & `spiakid-drs-0.20/spiakid_DRS/SpectralRes/IQCalibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.optimize import curve_fit
 import scipy.interpolate as interp;
-import Functions.utility as ut
+import spiakid_DRS.SpectralRes.utility as ut
 
 
 def IQ_binary_old(filename):
     
     data = np.fromfile(filename,dtype=float,count = -1,sep = '')
     data_len = int((len(data)-1)/2)
```

### Comparing `spiakid-drs-0.11/src/Functions/cmplxIQ.py` & `spiakid-drs-0.20/spiakid_DRS/SpectralRes/cmplxIQ.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.11/src/Functions/resonator.py` & `spiakid-drs-0.20/spiakid_DRS/SpectralRes/resonator.py`

 * *Files identical despite different names*

### Comparing `spiakid-drs-0.11/src/prototype.py` & `spiakid-drs-0.20/spiakid_DRS/inter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from Functions import Modelisation as mod
+from SpectralRes import Detect as D
 import os
 import argparse
 from pathlib import Path
 import pathlib
 
 """
 Link between Terminal and pipeline
@@ -19,28 +19,14 @@
 
 
 if __name__ == "__main__":
     args = parse()
 
     if args.init:
         try:
-            path = str(sorted(pathlib.Path('/').glob('**/Interface.py'))[0]) #Docker version
+            path = str(sorted(pathlib.Path('/').glob('**/Home.py'))[0]) #Docker version
         except:
-            path = str(sorted(pathlib.Path('').glob('**/Interface.py'))[0])  #Terminal version
+            path = str(sorted(pathlib.Path('').glob('**/Home.py'))[0])  #Terminal version
 
         os.system("streamlit run "+path)
     
-    if args.out_cfg!=None and args.in_cfg!=None:
-        mod.Data_read(args.in_cfg,args.out_cfg,args.form)
-        print('Done')
-
-    if args.dir:
-        output = Path('Output')
-        Input = Path('Data_location')
-        if output.exists():
-            pass
-        else:
-            output.mkdir()
-        if Input.exists():
-            pass
-        else:
-            Input.mkdir()
+
```

### Comparing `spiakid-drs-0.11/src/spiakid_drs.egg-info/PKG-INFO` & `spiakid-drs-0.20/spiakid_drs.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: spiakid-drs
-Version: 0.11
+Version: 0.20
 Summary: Data Reduction System of SPIAKID project
 Author-email: Pasquale Panuzzo <pasquale.panuzzo@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/DRS/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dynaconf
+Requires-Dist: h5py
+Requires-Dist: scraps
+Requires-Dist: lmfit
+Requires-Dist: streamlit
 
 # Data Reduction System of SPIAKID
 
 This project contains the **Data Reduction System** (DRS) of SPIAKID.
 
 The **SPIAKID** (SpectroPhotometric Imaging in Astronomy with Kinetic Inductance Detectors) project aims at designing, building and deploying on the sky a spectrophotometric imager based on Kinetic Inductance detectors. More information can be found on the [SPIAKID project homepage](https://www.observatoiredeparis.psl.eu/spiakid.html).
```

