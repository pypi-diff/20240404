# Comparing `tmp/envass-0.1.0.tar.gz` & `tmp/envass-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/envass-0.1.0.tar", last modified: Wed Nov 30 09:36:39 2022, max compression
+gzip compressed data, was "envass-1.0.0.tar", last modified: Thu Apr  4 14:50:25 2024, max compression
```

## Comparing `envass-0.1.0.tar` & `envass-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxr-x   0 jamesrunnalls  (1000) jamesrunnalls  (1000)        0 2022-11-30 09:36:39.000000 envass-0.1.0/
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)      998 2022-11-30 09:36:39.000000 envass-0.1.0/PKG-INFO
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)      450 2022-11-30 09:28:46.000000 envass-0.1.0/README.md
-drwxrwxr-x   0 jamesrunnalls  (1000) jamesrunnalls  (1000)        0 2022-11-30 09:36:39.000000 envass-0.1.0/envass/
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)       34 2022-11-30 09:28:46.000000 envass-0.1.0/envass/__init__.py
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)     3494 2022-11-30 09:28:46.000000 envass-0.1.0/envass/functions.py
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)     2147 2022-11-30 09:28:46.000000 envass-0.1.0/envass/main.py
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)    13184 2022-11-30 09:28:46.000000 envass-0.1.0/envass/methods.py
-drwxrwxr-x   0 jamesrunnalls  (1000) jamesrunnalls  (1000)        0 2022-11-30 09:36:39.000000 envass-0.1.0/envass.egg-info/
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)      998 2022-11-30 09:36:38.000000 envass-0.1.0/envass.egg-info/PKG-INFO
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)      239 2022-11-30 09:36:39.000000 envass-0.1.0/envass.egg-info/SOURCES.txt
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)        1 2022-11-30 09:36:38.000000 envass-0.1.0/envass.egg-info/dependency_links.txt
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)       94 2022-11-30 09:36:38.000000 envass-0.1.0/envass.egg-info/requires.txt
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)        7 2022-11-30 09:36:38.000000 envass-0.1.0/envass.egg-info/top_level.txt
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)       38 2022-11-30 09:36:39.000000 envass-0.1.0/setup.cfg
--rw-rw-r--   0 jamesrunnalls  (1000) jamesrunnalls  (1000)      792 2022-11-30 09:29:47.000000 envass-0.1.0/setup.py
+drwxrwxr-x   0 runnalja  (1000) runnalja  (1000)        0 2024-04-04 14:50:25.290656 envass-1.0.0/
+-rw-r--r--   0 runnalja  (1000) runnalja  (1000)      983 2024-04-04 14:50:25.290656 envass-1.0.0/PKG-INFO
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)      450 2024-04-04 14:09:23.000000 envass-1.0.0/README.md
+drwxrwxr-x   0 runnalja  (1000) runnalja  (1000)        0 2024-04-04 14:50:25.290656 envass-1.0.0/envass/
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)       34 2024-04-04 14:35:55.000000 envass-1.0.0/envass/__init__.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)     3494 2024-04-04 14:09:23.000000 envass-1.0.0/envass/functions.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)     2234 2024-04-04 14:38:04.000000 envass-1.0.0/envass/main.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)    13434 2024-04-04 14:45:50.000000 envass-1.0.0/envass/methods.py
+drwxrwxr-x   0 runnalja  (1000) runnalja  (1000)        0 2024-04-04 14:50:25.290656 envass-1.0.0/envass.egg-info/
+-rw-r--r--   0 runnalja  (1000) runnalja  (1000)      983 2024-04-04 14:50:25.000000 envass-1.0.0/envass.egg-info/PKG-INFO
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)      293 2024-04-04 14:50:25.000000 envass-1.0.0/envass.egg-info/SOURCES.txt
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)        1 2024-04-04 14:50:25.000000 envass-1.0.0/envass.egg-info/dependency_links.txt
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)       94 2024-04-04 14:50:25.000000 envass-1.0.0/envass.egg-info/requires.txt
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)       13 2024-04-04 14:50:25.000000 envass-1.0.0/envass.egg-info/top_level.txt
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)       38 2024-04-04 14:50:25.290656 envass-1.0.0/setup.cfg
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)      792 2024-04-04 14:49:29.000000 envass-1.0.0/setup.py
+drwxrwxr-x   0 runnalja  (1000) runnalja  (1000)        0 2024-04-04 14:50:25.290656 envass-1.0.0/tests/
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)        0 2024-04-04 14:43:24.000000 envass-1.0.0/tests/__init__.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)      144 2024-04-04 14:42:12.000000 envass-1.0.0/tests/context.py
+-rw-rw-r--   0 runnalja  (1000) runnalja  (1000)      376 2024-04-04 14:49:10.000000 envass-1.0.0/tests/test_main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `envass-0.1.0/PKG-INFO` & `envass-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: envass
-Version: 0.1.0
+Version: 1.0.0
 Summary: ENVASS ENVironmental data quality ASSurance.
 Home-page: https://github.com/eawag-surface-waters-research/envass
 Author: James Runnalls
 Author-email: <james.runnalls@eawag.ch>
 License: MIT
-Description: # ENVironmental data quality ASSurance
-        
-        ENVironmental data quality ASSurance for generating high quality data products.
-        
-        ## Installation
-        
-        `pip install envass`
-        
-        ## Usage
-        
-        ```python
-        
-        import numpy as np
-        from envass import qualityassurance
-        
-        variable = np.array([1, "g", 16, 12.0, False, 0, 22.12, 5.77])
-        time = np.array(range(len(variable)))
-        checks={"numeric":{}, "IQR":{"factor":4}, "IQR_window":{}}
-        
-        qa = qualityassurance(variable, time, **checks)
-        ```
-        
 Keywords: python,ENVASS,quality assurance,environmental data
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: ipywidgets>=7.6.5
+Requires-Dist: numpy>=1.19.5
+Requires-Dist: pandas>=1.1.5
+Requires-Dist: plotly>=5.6.0
+Requires-Dist: scikit-learn>=0.24.2
+Requires-Dist: scipy>=1.5.4
+
+# ENVironmental data quality ASSurance
+
+ENVironmental data quality ASSurance for generating high quality data products.
+
+## Installation
+
+`pip install envass`
+
+## Usage
+
+```python
+
+import numpy as np
+from envass import qualityassurance
+
+variable = np.array([1, "g", 16, 12.0, False, 0, 22.12, 5.77])
+time = np.array(range(len(variable)))
+checks={"numeric":{}, "IQR":{"factor":4}, "IQR_window":{}}
+
+qa = qualityassurance(variable, time, **checks)
+```
```

### Comparing `envass-0.1.0/envass/functions.py` & `envass-1.0.0/envass/functions.py`

 * *Files identical despite different names*

### Comparing `envass-0.1.0/envass/main.py` & `envass-1.0.0/envass/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from .methods import *
-from .functions import check_data, to_dict
+from . import methods
+from . import functions
 
 
 def qualityassurance(variable, time, **kwargs):
     """
         Quality assurance for timeseries data.
 
         Parameters:
@@ -14,50 +14,49 @@
             type of test supported: numeric, bounds, edges, IQR, variation_rate, IQR_moving, IQR_window, convolution, kmeans, kmeans_threshold, maintenance, 
             parameters examples: window_size, window_type,semiwindow, ncluster, threshold
             e.g. {"numeric":True,"IQR":{"factor":3}}
         Returns:
             qa (np.array): An array of ints where > 0 means non-trusted data.
         """
     
-    check_data(variable, time)
+    functions.check_data(variable, time)
     qa = np.zeros(variable.shape, dtype=int)
-    kwargs = to_dict(kwargs)
+    kwargs = functions.to_dict(kwargs)
 
     if "numeric" in kwargs:
-        qa[qa_numeric(variable)] = 1
+        qa[methods.qa_numeric(variable)] = 1
 
     if "bounds" in kwargs:
-        qa[qa_bounds(variable, **kwargs["bounds"])] = 1
+        qa[methods.qa_bounds(variable, **kwargs["bounds"])] = 1
 
     if "edges" in kwargs:
-        qa[qa_edges(variable, time, **kwargs["edges"])] = 1
+        qa[methods.qa_edges(variable, time, **kwargs["edges"])] = 1
 
     if "monotonic" in kwargs:
-        qa[qa_monotonic(time, **kwargs["monotonic"])] = 1
+        qa[methods.qa_monotonic(time, **kwargs["monotonic"])] = 1
         
     if "IQR" in kwargs:
-        qa[qa_iqr(variable, time, **kwargs["IQR"])] = 1
+        qa[methods.qa_iqr(variable, time, **kwargs["IQR"])] = 1
 
     if "variation_rate" in kwargs:
-        qa[qa_variation_rate(variable, time, **kwargs["variation_rate"])] = 1
+        qa[methods.qa_variation_rate(variable, time, **kwargs["variation_rate"])] = 1
     
     if "IQR_moving" in kwargs:
-        qa[qa_iqr_moving(variable, time, **kwargs["IQR_moving"])] = 1
+        qa[methods.qa_iqr_moving(variable, time, **kwargs["IQR_moving"])] = 1
 
     if "IQR_window" in kwargs:
-        qa[qa_max(variable, time, **kwargs["IQR_window"])] = 1
+        qa[methods.qa_max(variable, time, **kwargs["IQR_window"])] = 1
 
     if "kmeans" in kwargs:
-        qa[qa_kmeans(variable, time, **kwargs["kmeans"])] = 1
+        qa[methods.qa_kmeans(variable, time, **kwargs["kmeans"])] = 1
     
     if "kmeans_threshold" in kwargs:
-        qa[qa_kmeans_threshold(variable, time, **kwargs["kmeans_threshold"])] = 1
+        qa[methods.qa_kmeans_threshold(variable, time, **kwargs["kmeans_threshold"])] = 1
     
     if "maintenance" in kwargs:
-        qa[qa_maintenance(time, **kwargs["maintenance"])] = 1
+        qa[methods.qa_maintenance(time, **kwargs["maintenance"])] = 1
 
     if "individual_check" in kwargs:
-        qa[qa_individual(time, **kwargs["individual_check"])] = 1
+        qa[methods.qa_individual(time, **kwargs["individual_check"])] = 1
 
-        
     return qa
```

### Comparing `envass-0.1.0/envass/methods.py` & `envass-1.0.0/envass/methods.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,97 +1,102 @@
 import numpy as np
-from .functions import isnt_number, interp_nan, init_flag, nan_helper
+from . import functions
 import pandas as pd
 from sklearn.cluster import KMeans
 from datetime import datetime
 
 
 def qa_numeric(variable, prior_flags=False):
     """
     Indicate values that are not considered numerical 
 
     Parameters:
         variable (np.array): Data array to which to apply the quality assurance
     Returns:
         flag (np.array): An array of bools where True means non-trusted data for this outlier dectection
     """
-    
-    flags = init_flag(variable, prior_flags)
-    isnt_numeric = np.vectorize(isnt_number, otypes=[bool])
+
+    flags = functions.init_flag(variable, prior_flags)
+    isnt_numeric = np.vectorize(functions.isnt_number, otypes=[bool])
     flags[isnt_numeric(variable)] = True
     return flags
 
+
 def qa_bounds(variable, bounds, prior_flags=False):
     """¨
     Indicate values which are not in the range specified by the bounds
 
     Parameters:
         variable (np.array): Data array to which to apply the quality assurance
     Returns:
         flag (np.array): An array of bools where True means non-trusted data for this outlier dectection
     """
-    data = np.squeeze(np.array(pd.DataFrame(variable).apply(pd.to_numeric, errors='coerce').astype(np.float)))
+    data = np.squeeze(np.array(pd.DataFrame(variable).apply(pd.to_numeric, errors='coerce').astype(np.float64)))
     data[qa_numeric(data)] = np.nan
-    flags = init_flag(variable, prior_flags)
-    flags[~np.isnan(data)] = np.logical_or(data[~np.isnan(data)] < float(bounds[0]), data[~np.isnan(data)] > float(bounds[1]))
+    flags = functions.init_flag(variable, prior_flags)
+    flags[~np.isnan(data)] = np.logical_or(data[~np.isnan(data)] < float(bounds[0]),
+                                           data[~np.isnan(data)] > float(bounds[1]))
     return flags
 
+
 def qa_edges(variable, time, edges, prior_flags=False):
     """
     Indicate values on the edges of the data set
 
     Parameters:
     variable (np.array): Data array to which to apply the quality assurance
         time (np.array): Time array corresponding to the Data array, time should be in seconds
         edges (int): time (s) in which the data will be cutted on the edges
         prior_flags (np.array): An array of bools where True means non-trusted data
     Returns:
         flag (np.array): An array of bools where True means non-trusted data for this outlier dectection
     """
-    flags = np.atleast_2d(init_flag(variable, prior_flags))
-    flags[:,time > time[-1] - edges] = True
-    flags[:,time < time[0] + edges] = True
+    flags = np.atleast_2d(functions.init_flag(variable, prior_flags))
+    flags[:, time > time[-1] - edges] = True
+    flags[:, time < time[0] + edges] = True
     return np.squeeze(flags)
 
+
 def qa_monotonic(time, monotonic, prior_flags=False):
     '''
     Indicate values which are not (strictly) increasing/decreasing
 
     Parameters:
         time (np.array): Time array corresponding to the Data array, time should be in seconds
         monotonic (str): Indicate if the vector should be: strictly_increasing, increasing, strictly decreasing or decreasing
         prior_flags (np.array): An array of bools where True means non-trusted data
     Returns:
         flag (np.array): An array of bools where True means non-trusted data for this outlier dectection
     '''
-    flags = init_flag(time, prior_flags)
-    if 'strictly_increasing'in monotonic:
-        flags[np.where(np.diff(time)<=0)[0]+1] = 1
-    if 'strictly_decreasing'in monotonic:
-        flags[np.where(np.diff(time)>=0)[0]+1] = 1
-    if 'increasing'in monotonic:
-        flags[np.where(np.diff(time)<0)[0]+1] = 1
-    if 'decreasing'in monotonic:
-        flags[np.where(np.diff(time)>0)[0]+1] = 1
+    flags = functions.init_flag(time, prior_flags)
+    if 'strictly_increasing' in monotonic:
+        flags[np.where(np.diff(time) <= 0)[0] + 1] = 1
+    if 'strictly_decreasing' in monotonic:
+        flags[np.where(np.diff(time) >= 0)[0] + 1] = 1
+    if 'increasing' in monotonic:
+        flags[np.where(np.diff(time) < 0)[0] + 1] = 1
+    if 'decreasing' in monotonic:
+        flags[np.where(np.diff(time) > 0)[0] + 1] = 1
     return flags
 
+
 def qa_iqr(variable, time, factor=3, prior_flags=False):
     """
     Indicate values outside interquartile Range (IQR) for timeseries data.
 
     Parameters:
         variable (np.array): Data array to which to apply the quality assurance
         factor (int): threshold for outlier labelling rule
         prior_flags (np.array): An array of bools where True means non-trusted data
 
     Returns:
         flag (np.array): An array of bools where True means non-trusted data after this outlier detection
     """
-    data = interp_nan(time, np.copy(variable))
-    flags = init_flag(time, prior_flags)
+    data = functions.interp_nan(time, np.copy(variable))
+    flags = functions.init_flag(time, prior_flags)
 
     q75 = np.quantile(data, 0.75)
     q25 = np.quantile(data, 0.25)
     iqr = q75 - q25
     if iqr != 0:
         sup = q75 + factor * iqr
         inf = q25 - factor * iqr
@@ -100,28 +105,29 @@
         idx0 = np.r_[idx1, idx2]
     else:
         idx0 = np.array([])
 
     flags[idx0] = True
     return flags
 
+
 def qa_variation_rate(variable, time, prior_flags=False):
     """
     Indicate the trustability of the  values if variation rate exceed a defined threshold.
 
     Parameters:
         variable (np.array): Data array to which to apply the quality assurance 
         time (np.array): Time array corresponding to the Data array  
         prior_flags (np.array): An array of bools where True means non-trusted data
     Returns:
         flag (np.array): An array of bools where True means non-trusted data for this outlier dectection
     """
-    
-    data = interp_nan(time, np.copy(variable))
-    flags = init_flag(time, prior_flags)
+
+    data = functions.interp_nan(time, np.copy(variable))
+    flags = functions.init_flag(time, prior_flags)
 
     vec_diff = abs(np.diff(data))
     if len(vec_diff) > 0:
         vecdiff_quan = np.quantile(vec_diff, 0.999)
         idx_vecdiff = np.where(vec_diff >= vecdiff_quan)[0]
 
         vec_max = np.max(data)
@@ -132,36 +138,37 @@
         elif vec_max / np.quantile(data, 0.9999) < 2:
             quantile_threshold = 0.9999
         elif vec_max / np.quantile(data, 0.99999) < 2:
             quantile_threshold = 0.99999
 
         vec_quan = np.quantile(data, quantile_threshold)
         idx_vec = np.where(data >= vec_quan)[0]
-        idx = list(set(idx_vecdiff) & set(idx_vec)) 
+        idx = list(set(idx_vecdiff) & set(idx_vec))
     else:
         idx = []
     flags = np.array(flags, dtype=bool)
     flags[idx] = True
     return flags
 
+
 def qa_iqr_moving(variable, time, window_size=15, factor=3, prior_flags=False):
     """
    Indicate outliers values based on Interquartile Range (IQR) for a window of time series data
 
    Parameters:
        variable (np.array): Data array to which to apply the quality assurance
        windowsize (np.int): window size of data
        prior_flags (np.array): An array of bools where True means non-trusted data
 
    Returns:
        flags (np.array): An array of bools where True means non-trusted data for this outlier dectection
    """
-    data = interp_nan(time, np.copy(variable))
+    data = functions.interp_nan(time, np.copy(variable))
 
-    flags = init_flag(time, prior_flags)
+    flags = functions.init_flag(time, prior_flags)
 
     if len(data) < window_size:
         print("ERROR! Window size is larger than array length.")
     else:
         for i in range(0, (len(data) - window_size + 1)):
             data_sub = np.copy(data[i:i + window_size])
             q75 = np.quantile(data_sub, 0.75)
@@ -173,67 +180,69 @@
             idx1 = np.where(data_sub >= outsup)[0]
             idx2 = np.where(data_sub <= outinf)[0]
 
             idx0 = np.r_[idx1, idx2]
 
             if len(idx0) != 0:
                 flags[i + idx0] = flags[i + idx0] + 1
-    flags[flags>1]=1
+    flags[flags > 1] = 1
     flags = np.array(flags, dtype=bool)
     return flags
 
+
 def qa_max(variable, time, factor=3, semiwindow=1000, prior_flags=False):
     """
         Indicate outliers values based on Interquartile Range (IQR) for a window of time series data
 
        Parameters:
            variable (np.array): Data array to which to apply the quality assurance
            semiwindow (int): window size of data
            factor (int): threshold for outlier labelling rule
            prior_flags (np.array): An array of bools where True means non-trusted data
 
        Returns:
            flags (np.array): An array of bools where True means non-trusted data for this outlier detection
    """
-    data = interp_nan(time, np.copy(variable))
-    flags = init_flag(time, prior_flags)
+    data = functions.interp_nan(time, np.copy(variable))
+    flags = functions.init_flag(time, prior_flags)
 
     maxy = np.nanmax(data)
 
     n0 = np.where(data == maxy)[0][0] - semiwindow
     n1 = np.where(data == maxy)[0][0] + semiwindow
 
     if n0 < 0:
         n0 = 0  # maybe not ! check for the last dataset
     if n1 > (len(data) - 1):
-        n1 = len(data) - 1 #Yes but add the non evaluated dataset to the next bin
+        n1 = len(data) - 1  # Yes but add the non evaluated dataset to the next bin
 
     vec_sub = data[n0:n1]
     vec_qual = np.zeros(len(vec_sub))
     vec_time = time[n0:n1]
-    flags99 = qa_iqr(vec_sub,vec_time,factor)
+    flags99 = qa_iqr(vec_sub, vec_time, factor)
     if sum(flags99) > 0:
         flags[n0:n1] = flags[n0:n1] + flags99  # update vec_qual
 
     flags = np.array(flags, dtype=bool)
     return flags
 
-def qa_kmeans(variable, time, ncluster=2, prior_flags = False):
+
+def qa_kmeans(variable, time, ncluster=2, prior_flags=False):
     """
         Indicate outliers based on kmean clustering.
 
         Parameters:
             variable (np.array): Data array to which to apply the quality assurance
             ncluster (int) : number of cluster (>=2)
             prior_flags (np.array): An array of bools where True means non-trusted data
         Returns:
             flags (np.array): An array of bools where True means non-trusted data for this outlier detection
     """
-    data = interp_nan(time, np.copy(variable))
-    flags = init_flag(time, prior_flags)
+    data = functions.interp_nan(time, np.copy(variable))
+    flags = functions.init_flag(time, prior_flags)
 
     clusterer = KMeans(n_clusters=ncluster)
     clusterer.fit(data.reshape(-1, 1))
 
     nearest_centroid_idx = clusterer.predict(data.reshape(-1, 1))
 
     igr1 = np.where(nearest_centroid_idx == 0)[0]
@@ -244,27 +253,28 @@
     if val_thresh >= 5:  # if there is no 2 clearly seperated groups
         flags[igr2] = True
 
     flags = np.array(flags, dtype=bool)
 
     return flags
 
+
 def qa_kmeans_threshold(variable, time, ncluster=2, threshold=1.2, prior_flags=False):
     """
         Indicate outliers based on kmean clustering and threshold value.
 
         Parameters:
             variable (np.array): Data array to which to apply the quality assurance
             ncluster : number of cluster (>=2)
             prior_flags (np.array): An array of bools where True means non-trusted data
         Returns:
             flags (np.array): An array of bools where True means non-trusted data for this outlier detection
     """
-    data = interp_nan(time, np.copy(variable))
-    flags = init_flag(time, prior_flags)
+    data = functions.interp_nan(time, np.copy(variable))
+    flags = functions.init_flag(time, prior_flags)
 
     clusterer = KMeans(n_clusters=ncluster)
     clusterer.fit(data.reshape(-1, 1))
 
     nearest_centroid_idx = clusterer.predict(data.reshape(-1, 1))
 
     igr1 = np.where(nearest_centroid_idx == 0)[0]
@@ -280,56 +290,57 @@
     if val_thresh < threshold:  # if there is no 2 clearly seperated groups
         igrfin = []
     else:
         flags[igrfin] = True
     flags = np.array(flags, dtype=bool)
     return flags
 
-def qa_maintenance(time,path='maintenance_log.csv', prior_flags=False):
+
+def qa_maintenance(time, path='maintenance_log.csv', prior_flags=False):
     """
         Indicate the trustability of values based on the maintenance logbook
 
         Parameters:
             time (np.array): Time array to which to apply the quality assurance
             prior_flags (np.array): An array of bools where True means non-trusted data
             additional comments: The maintenance_log.csv should have a date format '%Y-%m-%d %H:%M:%S.%f'
         Returns:
             flags (np.array): An array of bools where True means non-trusted data
     """
-    maintenance_log=pd.read_csv(path, sep=';')
+    maintenance_log = pd.read_csv(path, sep=';')
 
-    flags = init_flag(time, prior_flags)
-    
-    start=maintenance_log.start.apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S.%f'))
-    end=maintenance_log.end.apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S.%f'))
-    maintenance_end=[datetime.timestamp(s) for s in end]
-    maintenance_start=[datetime.timestamp(s) for s in start]
-    
-    mask=[]
-    for i in  range(0,len(maintenance_end)):
-        mask=(time>maintenance_start[i]) & (time<maintenance_end[i])
-        flags[mask]=True
+    flags = functions.init_flag(time, prior_flags)
+
+    start = maintenance_log.start.apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S.%f'))
+    end = maintenance_log.end.apply(lambda x: datetime.strptime(x, '%Y-%m-%d %H:%M:%S.%f'))
+    maintenance_end = [datetime.timestamp(s) for s in end]
+    maintenance_start = [datetime.timestamp(s) for s in start]
+
+    mask = []
+    for i in range(0, len(maintenance_end)):
+        mask = (time > maintenance_start[i]) & (time < maintenance_end[i])
+        flags[mask] = True
 
     return flags
 
 
-def qa_individual(time, individual_check, prior_flags = False):
+def qa_individual(time, individual_check, prior_flags=False):
     """ 
         Read individual checks and flag 
         
         Parameters: 
             time (np.array): Time array to which to apply the quality assurance
             individual_check (list): List with points in time having to be removed 
             prior_flags (np.array): An array of bools where True means non-trusted data
         Returns:
             flags (np.array): An array of bools where True means non-trusted data
             """
-    flags = init_flag(time, prior_flags)
+    flags = functions.init_flag(time, prior_flags)
     for i in individual_check:
-        flag_idx = np.where(i==time)[0]
+        flag_idx = np.where(i == time)[0]
         flags[flag_idx] = True
     return flags
 
 
 def qa_moving_average_limit(variable, window=100, limit=5, prior_flags=False):
     """
     Indicate values on the edges of the data set
@@ -337,14 +348,13 @@
         variable (np.array): Data array to which to apply the quality assurance
         window (int): Size of window for moving average
         limit (flaot): Allowable distance from the moving average
         prior_flags (np.array): An array of bools where True means non-trusted data
     Returns:
         flag (np.array): An array of bools where True means non-trusted data for this outlier dectection
     """
-    flags = init_flag(variable, prior_flags)
+    flags = functions.init_flag(variable, prior_flags)
     ma = np.convolve(variable, np.ones(window), 'same') / window
-    nans, xx = nan_helper(ma)
+    nans, xx = functions.nan_helper(ma)
     ma[nans] = np.interp(xx(nans), xx(~nans), ma[~nans])
     flags[np.abs(ma - variable) > limit] = True
     return flags
-
```

### Comparing `envass-0.1.0/envass.egg-info/PKG-INFO` & `envass-1.0.0/envass.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 Metadata-Version: 2.1
 Name: envass
-Version: 0.1.0
+Version: 1.0.0
 Summary: ENVASS ENVironmental data quality ASSurance.
 Home-page: https://github.com/eawag-surface-waters-research/envass
 Author: James Runnalls
 Author-email: <james.runnalls@eawag.ch>
 License: MIT
-Description: # ENVironmental data quality ASSurance
-        
-        ENVironmental data quality ASSurance for generating high quality data products.
-        
-        ## Installation
-        
-        `pip install envass`
-        
-        ## Usage
-        
-        ```python
-        
-        import numpy as np
-        from envass import qualityassurance
-        
-        variable = np.array([1, "g", 16, 12.0, False, 0, 22.12, 5.77])
-        time = np.array(range(len(variable)))
-        checks={"numeric":{}, "IQR":{"factor":4}, "IQR_window":{}}
-        
-        qa = qualityassurance(variable, time, **checks)
-        ```
-        
 Keywords: python,ENVASS,quality assurance,environmental data
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: ipywidgets>=7.6.5
+Requires-Dist: numpy>=1.19.5
+Requires-Dist: pandas>=1.1.5
+Requires-Dist: plotly>=5.6.0
+Requires-Dist: scikit-learn>=0.24.2
+Requires-Dist: scipy>=1.5.4
+
+# ENVironmental data quality ASSurance
+
+ENVironmental data quality ASSurance for generating high quality data products.
+
+## Installation
+
+`pip install envass`
+
+## Usage
+
+```python
+
+import numpy as np
+from envass import qualityassurance
+
+variable = np.array([1, "g", 16, 12.0, False, 0, 22.12, 5.77])
+time = np.array(range(len(variable)))
+checks={"numeric":{}, "IQR":{"factor":4}, "IQR_window":{}}
+
+qa = qualityassurance(variable, time, **checks)
+```
```

### Comparing `envass-0.1.0/setup.py` & `envass-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     README = f.read()
 
-VERSION = '0.1.0'
+VERSION = '1.0.0'
 DESCRIPTION = 'ENVASS ENVironmental data quality ASSurance.'
 
 setup(
     name="envass",
     version=VERSION,
     author="James Runnalls",
     author_email="<james.runnalls@eawag.ch>",
```

