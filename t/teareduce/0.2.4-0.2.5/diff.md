# Comparing `tmp/teareduce-0.2.4.tar.gz` & `tmp/teareduce-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teareduce-0.2.4.tar", last modified: Thu Mar 14 06:47:03 2024, max compression
+gzip compressed data, was "teareduce-0.2.5.tar", last modified: Thu Apr  4 14:34:39 2024, max compression
```

## Comparing `teareduce-0.2.4.tar` & `teareduce-0.2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-03-14 06:47:03.985967 teareduce-0.2.4/
--rw-r--r--   0 cardiel    (501) staff       (20)    35149 2023-12-18 07:38:30.000000 teareduce-0.2.4/LICENSE.txt
--rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-03-14 06:47:03.985522 teareduce-0.2.4/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)     1109 2024-01-12 07:35:44.000000 teareduce-0.2.4/README.md
--rw-r--r--   0 cardiel    (501) staff       (20)     1624 2024-01-12 07:48:48.000000 teareduce-0.2.4/pyproject.toml
--rw-r--r--   0 cardiel    (501) staff       (20)       38 2024-03-14 06:47:03.986046 teareduce-0.2.4/setup.cfg
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-03-14 06:47:03.939313 teareduce-0.2.4/src/
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-03-14 06:47:03.982615 teareduce-0.2.4/src/teareduce/
--rw-r--r--   0 cardiel    (501) staff       (20)      909 2024-01-24 16:46:28.000000 teareduce-0.2.4/src/teareduce/__init__.py
--rw-r--r--   0 cardiel    (501) staff       (20)      648 2024-01-10 07:02:03.000000 teareduce-0.2.4/src/teareduce/avoid_astropy_warnings.py
--rw-r--r--   0 cardiel    (501) staff       (20)    24209 2024-01-10 09:37:14.000000 teareduce-0.2.4/src/teareduce/cosmicrays.py
--rw-r--r--   0 cardiel    (501) staff       (20)     2084 2024-03-13 08:16:34.000000 teareduce-0.2.4/src/teareduce/ctext.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1922 2024-01-10 09:15:12.000000 teareduce-0.2.4/src/teareduce/draw_rectangle.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1045 2024-03-14 06:42:00.000000 teareduce-0.2.4/src/teareduce/elapsed_time.py
--rw-r--r--   0 cardiel    (501) staff       (20)     3852 2024-01-10 09:15:40.000000 teareduce-0.2.4/src/teareduce/imshow.py
--rw-r--r--   0 cardiel    (501) staff       (20)     9890 2024-01-10 12:36:53.000000 teareduce-0.2.4/src/teareduce/peaks_spectrum.py
--rw-r--r--   0 cardiel    (501) staff       (20)    14281 2024-01-10 12:36:53.000000 teareduce-0.2.4/src/teareduce/polfit.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1084 2024-01-10 09:16:27.000000 teareduce-0.2.4/src/teareduce/robust_std.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5797 2024-01-11 08:06:41.000000 teareduce-0.2.4/src/teareduce/sdistortion.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5104 2024-01-10 07:18:01.000000 teareduce-0.2.4/src/teareduce/sliceregion.py
--rw-r--r--   0 cardiel    (501) staff       (20)     5417 2024-01-11 08:06:41.000000 teareduce-0.2.4/src/teareduce/statsummary.py
--rw-r--r--   0 cardiel    (501) staff       (20)      303 2024-03-14 06:42:17.000000 teareduce-0.2.4/src/teareduce/version.py
--rw-r--r--   0 cardiel    (501) staff       (20)    68697 2024-01-11 08:06:08.000000 teareduce-0.2.4/src/teareduce/wavecal.py
--rw-r--r--   0 cardiel    (501) staff       (20)     1161 2024-01-10 09:10:38.000000 teareduce-0.2.4/src/teareduce/zscale.py
-drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-03-14 06:47:03.984899 teareduce-0.2.4/src/teareduce.egg-info/
--rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-03-14 06:47:03.000000 teareduce-0.2.4/src/teareduce.egg-info/PKG-INFO
--rw-r--r--   0 cardiel    (501) staff       (20)      668 2024-03-14 06:47:03.000000 teareduce-0.2.4/src/teareduce.egg-info/SOURCES.txt
--rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-03-14 06:47:03.000000 teareduce-0.2.4/src/teareduce.egg-info/dependency_links.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       77 2024-03-14 06:47:03.000000 teareduce-0.2.4/src/teareduce.egg-info/requires.txt
--rw-r--r--   0 cardiel    (501) staff       (20)       10 2024-03-14 06:47:03.000000 teareduce-0.2.4/src/teareduce.egg-info/top_level.txt
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-04 14:34:39.194696 teareduce-0.2.5/
+-rw-r--r--   0 cardiel    (501) staff       (20)    35149 2023-12-18 07:38:30.000000 teareduce-0.2.5/LICENSE.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-04-04 14:34:39.194434 teareduce-0.2.5/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)     1109 2024-01-12 07:35:44.000000 teareduce-0.2.5/README.md
+-rw-r--r--   0 cardiel    (501) staff       (20)     1624 2024-01-12 07:48:48.000000 teareduce-0.2.5/pyproject.toml
+-rw-r--r--   0 cardiel    (501) staff       (20)       38 2024-04-04 14:34:39.194746 teareduce-0.2.5/setup.cfg
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-04 14:34:39.184920 teareduce-0.2.5/src/
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-04 14:34:39.193036 teareduce-0.2.5/src/teareduce/
+-rw-r--r--   0 cardiel    (501) staff       (20)      909 2024-01-24 16:46:28.000000 teareduce-0.2.5/src/teareduce/__init__.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      648 2024-01-10 07:02:03.000000 teareduce-0.2.5/src/teareduce/avoid_astropy_warnings.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    24209 2024-01-10 09:37:14.000000 teareduce-0.2.5/src/teareduce/cosmicrays.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     2084 2024-03-13 08:16:34.000000 teareduce-0.2.5/src/teareduce/ctext.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1922 2024-01-10 09:15:12.000000 teareduce-0.2.5/src/teareduce/draw_rectangle.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1045 2024-03-14 06:42:00.000000 teareduce-0.2.5/src/teareduce/elapsed_time.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     3852 2024-01-10 09:15:40.000000 teareduce-0.2.5/src/teareduce/imshow.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     9890 2024-01-10 12:36:53.000000 teareduce-0.2.5/src/teareduce/peaks_spectrum.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    14281 2024-01-10 12:36:53.000000 teareduce-0.2.5/src/teareduce/polfit.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1084 2024-01-10 09:16:27.000000 teareduce-0.2.5/src/teareduce/robust_std.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5806 2024-04-04 14:31:24.000000 teareduce-0.2.5/src/teareduce/sdistortion.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5104 2024-01-10 07:18:01.000000 teareduce-0.2.5/src/teareduce/sliceregion.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     5426 2024-04-04 14:31:46.000000 teareduce-0.2.5/src/teareduce/statsummary.py
+-rw-r--r--   0 cardiel    (501) staff       (20)      303 2024-04-04 14:32:39.000000 teareduce-0.2.5/src/teareduce/version.py
+-rw-r--r--   0 cardiel    (501) staff       (20)    68706 2024-04-04 14:24:28.000000 teareduce-0.2.5/src/teareduce/wavecal.py
+-rw-r--r--   0 cardiel    (501) staff       (20)     1161 2024-01-10 09:10:38.000000 teareduce-0.2.5/src/teareduce/zscale.py
+drwxr-xr-x   0 cardiel    (501) staff       (20)        0 2024-04-04 14:34:39.194128 teareduce-0.2.5/src/teareduce.egg-info/
+-rw-r--r--   0 cardiel    (501) staff       (20)     2281 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/PKG-INFO
+-rw-r--r--   0 cardiel    (501) staff       (20)      668 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/SOURCES.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)        1 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/dependency_links.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       77 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/requires.txt
+-rw-r--r--   0 cardiel    (501) staff       (20)       10 2024-04-04 14:34:39.000000 teareduce-0.2.5/src/teareduce.egg-info/top_level.txt
```

### Comparing `teareduce-0.2.4/LICENSE.txt` & `teareduce-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/PKG-INFO` & `teareduce-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teareduce
-Version: 0.2.4
+Version: 0.2.5
 Summary: Utilities for astronomical data reduction
 Author-email: Nicolás Cardiel <cardiel@ucm.es>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/nicocardiel/teareduce
 Project-URL: Repository, https://github.com/nicocardiel/teareduce.git
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `teareduce-0.2.4/README.md` & `teareduce-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/pyproject.toml` & `teareduce-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/__init__.py` & `teareduce-0.2.5/src/teareduce/__init__.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/avoid_astropy_warnings.py` & `teareduce-0.2.5/src/teareduce/avoid_astropy_warnings.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/cosmicrays.py` & `teareduce-0.2.5/src/teareduce/cosmicrays.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/ctext.py` & `teareduce-0.2.5/src/teareduce/ctext.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/draw_rectangle.py` & `teareduce-0.2.5/src/teareduce/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/elapsed_time.py` & `teareduce-0.2.5/src/teareduce/elapsed_time.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/imshow.py` & `teareduce-0.2.5/src/teareduce/imshow.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/peaks_spectrum.py` & `teareduce-0.2.5/src/teareduce/peaks_spectrum.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/polfit.py` & `teareduce-0.2.5/src/teareduce/polfit.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/robust_std.py` & `teareduce-0.2.5/src/teareduce/robust_std.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/sdistortion.py` & `teareduce-0.2.5/src/teareduce/sdistortion.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # License-Filename: LICENSE.txt
 #
 
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.polynomial import Polynomial
 from scipy import ndimage
-from tqdm import tqdm
+from tqdm.notebook import tqdm
 
 from .imshow import imshow
 from .polfit import polfit_residuals_with_sigma_rejection
 
 
 def fit_sdistortion(data, ns_min, ns_max, nc_min, nc_max,
                     median_size=None,
```

### Comparing `teareduce-0.2.4/src/teareduce/sliceregion.py` & `teareduce-0.2.5/src/teareduce/sliceregion.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce/statsummary.py` & `teareduce-0.2.5/src/teareduce/statsummary.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # SPDX-License-Identifier: GPL-3.0+
 # License-Filename: LICENSE.txt
 #
 
 from astropy.io import fits
 import numpy as np
 from pathlib import Path
-from tqdm import tqdm
+from tqdm.notebook import tqdm
 
 from .robust_std import robust_std
 from .sliceregion import SliceRegion2D
 
 
 def statsummary(x=None, rm_nan=False, show=True):
     """Compute basic statistical parameters.
```

### Comparing `teareduce-0.2.4/src/teareduce/wavecal.py` & `teareduce-0.2.5/src/teareduce/wavecal.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from datetime import datetime
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 import numpy as np
 from numpy.polynomial import Polynomial
 from pathlib import Path
 from scipy.ndimage import gaussian_filter1d
-from tqdm import tqdm
+from tqdm.notebook import tqdm
 
 from .ctext import ctext
 from .imshow import imshow
 from .peaks_spectrum import find_peaks_spectrum, refine_peaks_spectrum
 from .polfit import polfit_residuals_with_sigma_rejection
 from .sliceregion import SliceRegion1D
```

### Comparing `teareduce-0.2.4/src/teareduce/zscale.py` & `teareduce-0.2.5/src/teareduce/zscale.py`

 * *Files identical despite different names*

### Comparing `teareduce-0.2.4/src/teareduce.egg-info/PKG-INFO` & `teareduce-0.2.5/src/teareduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teareduce
-Version: 0.2.4
+Version: 0.2.5
 Summary: Utilities for astronomical data reduction
 Author-email: Nicolás Cardiel <cardiel@ucm.es>
 License: GPL-3.0-or-later
 Project-URL: Homepage, https://github.com/nicocardiel/teareduce
 Project-URL: Repository, https://github.com/nicocardiel/teareduce.git
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `teareduce-0.2.4/src/teareduce.egg-info/SOURCES.txt` & `teareduce-0.2.5/src/teareduce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

