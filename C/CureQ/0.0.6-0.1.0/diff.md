# Comparing `tmp/CureQ-0.0.6.tar.gz` & `tmp/CureQ-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CureQ-0.0.6.tar", last modified: Tue Apr  2 10:36:21 2024, max compression
+gzip compressed data, was "CureQ-0.1.0.tar", last modified: Thu Apr  4 10:25:38 2024, max compression
```

## Comparing `CureQ-0.0.6.tar` & `CureQ-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:36:21.614630 CureQ-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-04-02 10:36:21.583380 CureQ-0.0.6/CureQ/
--rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.0.6/CureQ/__init__.py
--rw-rw-rw-   0        0        0    41237 2024-04-02 09:31:40.000000 CureQ-0.0.6/CureQ/mea.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:36:21.614630 CureQ-0.0.6/CureQ.egg-info/
--rw-rw-rw-   0        0        0     1430 2024-04-02 10:36:20.000000 CureQ-0.0.6/CureQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-04-02 10:36:21.000000 CureQ-0.0.6/CureQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:36:20.000000 CureQ-0.0.6/CureQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-02 10:36:20.000000 CureQ-0.0.6/CureQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 10:36:20.000000 CureQ-0.0.6/CureQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1430 2024-04-02 10:36:21.614630 CureQ-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      708 2024-03-19 15:09:22.000000 CureQ-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 10:36:21.614630 CureQ-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1366 2024-04-02 10:35:38.000000 CureQ-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:38.475905 CureQ-0.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:38.444243 CureQ-0.1.0/CureQ/
+-rw-rw-rw-   0        0        0      293 2024-03-14 12:47:34.000000 CureQ-0.1.0/CureQ/__init__.py
+-rw-rw-rw-   0        0        0    62828 2024-04-04 10:16:10.000000 CureQ-0.1.0/CureQ/mea.py
+-rw-rw-rw-   0        0        0    41237 2024-04-02 11:23:38.000000 CureQ-0.1.0/CureQ/mea_02_04.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:25:38.475905 CureQ-0.1.0/CureQ.egg-info/
+-rw-rw-rw-   0        0        0     1529 2024-04-04 10:25:37.000000 CureQ-0.1.0/CureQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-04-04 10:25:38.000000 CureQ-0.1.0/CureQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:25:37.000000 CureQ-0.1.0/CureQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2024-04-04 10:25:37.000000 CureQ-0.1.0/CureQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-04 10:25:37.000000 CureQ-0.1.0/CureQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2024-03-19 15:09:22.000000 CureQ-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1529 2024-04-04 10:25:38.475905 CureQ-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      708 2024-03-19 15:09:22.000000 CureQ-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:25:38.475905 CureQ-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1631 2024-04-04 08:45:28.000000 CureQ-0.1.0/setup.py
```

### Comparing `CureQ-0.0.6/CureQ/mea.py` & `CureQ-0.1.0/CureQ/mea_02_04.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Version 0.0.5
+# Version 0.0.6
 
 '''This file contains the entire MEA_analyzer pipeline, contained in functions'''
 # Imports
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.signal import butter, lfilter
 from scipy.stats import norm
```

### Comparing `CureQ-0.0.6/CureQ.egg-info/PKG-INFO` & `CureQ-0.1.0/CureQ.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CureQ
-Version: 0.0.6
+Version: 0.1.0
 Summary: Library for analyzing MEA files.
 Home-page: https://github.com/CureQ/CureQ.git
 Author: CureQ
 Author-email: cureq-ft@hva.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,17 @@
 Requires-Dist: matplotlib>=3.7.3
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: h5py>=3.9.0
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: seaborn>=0.12.2
+Requires-Dist: statsmodels>=0.14.0
+Requires-Dist: skimage>=0.22.0
+Requires-Dist: plotly>=5.14.0
 
 ### CureQ - HvA
 
 This is the repository of the CureQ consortium.<br>
 This repository contains a library with functions for analyzing a MEA file.<br>
 This repository is maintained by the Amsterdam University of Applied Sciences.<br>
 More information: https://cureq.nl/
```

### Comparing `CureQ-0.0.6/LICENSE` & `CureQ-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CureQ-0.0.6/PKG-INFO` & `CureQ-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CureQ
-Version: 0.0.6
+Version: 0.1.0
 Summary: Library for analyzing MEA files.
 Home-page: https://github.com/CureQ/CureQ.git
 Author: CureQ
 Author-email: cureq-ft@hva.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,17 @@
 Requires-Dist: matplotlib>=3.7.3
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: h5py>=3.9.0
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: seaborn>=0.12.2
+Requires-Dist: statsmodels>=0.14.0
+Requires-Dist: skimage>=0.22.0
+Requires-Dist: plotly>=5.14.0
 
 ### CureQ - HvA
 
 This is the repository of the CureQ consortium.<br>
 This repository contains a library with functions for analyzing a MEA file.<br>
 This repository is maintained by the Amsterdam University of Applied Sciences.<br>
 More information: https://cureq.nl/
```

### Comparing `CureQ-0.0.6/README.md` & `CureQ-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `CureQ-0.0.6/setup.py` & `CureQ-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,33 @@
 # Use the text in the README file for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # Setup metadata for initializing the library
 setuptools.setup(
     name="CureQ",
-    version="0.0.6",
+    version="0.1.0",
     author="CureQ",
     author_email="cureq-ft@hva.nl",
     description="Library for analyzing MEA files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CureQ/CureQ.git",
     packages=setuptools.find_packages(),
     install_requires=[          # Installs all required libraries to run the pipeline analysis correctly
         "matplotlib>=3.7.3",    # For visualisation plots of the data
         "numpy>=1.26.4",        # For array computing in python
         "h5py>=3.9.0",          # For reading the HDF5 file in python
         "pandas>=2.1.4",        # For creating and using a 2D Dataframe
         "scipy>=1.11.4",        # For scientific functions in Python
         "scikit-learn>=1.3.0",  # For basic Machine Learning modules
-        "seaborn>=0.12.2"       # For statistical data visualization
+        "seaborn>=0.12.2",      # For statistical data visualization
+        "statsmodels>=0.14.0",  # For calculating the partial autocorrelation function
+        "skimage>=0.22.0",      # For determining the threshold of the network bursts
+        "plotly>=5.14.0"        # For creating an interactive 3D view of a single well
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
-)
+)
```

