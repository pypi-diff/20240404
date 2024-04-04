# Comparing `tmp/PyQuantimClient-1.0.83.tar.gz` & `tmp/PyQuantimClient-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQuantimClient-1.0.83.tar", last modified: Thu Apr  4 16:33:58 2024, max compression
+gzip compressed data, was "PyQuantimClient-1.0.9.tar", last modified: Mon Dec 19 20:05:36 2022, max compression
```

## Comparing `PyQuantimClient-1.0.83.tar` & `PyQuantimClient-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:33:58.131884 PyQuantimClient-1.0.83/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 16:33:58.131884 PyQuantimClient-1.0.83/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:33:58.131884 PyQuantimClient-1.0.83/PyQuantimClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-04 16:33:58.000000 PyQuantimClient-1.0.83/PyQuantimClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-04 16:33:58.000000 PyQuantimClient-1.0.83/PyQuantimClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:33:58.000000 PyQuantimClient-1.0.83/PyQuantimClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 16:33:58.000000 PyQuantimClient-1.0.83/PyQuantimClient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:33:58.131884 PyQuantimClient-1.0.83/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:33:58.131884 PyQuantimClient-1.0.83/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/bi.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/portfolios.py
--rw-r--r--   0 runner    (1001) docker     (127)    19944 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/preprocess_co.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/risk.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-04 16:33:49.000000 PyQuantimClient-1.0.83/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-19 20:05:36.000000 PyQuantimClient-1.0.9/PyQuantimClient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:36.514548 PyQuantimClient-1.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/portfolios.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/preprocess_co.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2022-12-19 20:05:26.000000 PyQuantimClient-1.0.9/src/risk.py
```

### Comparing `PyQuantimClient-1.0.83/src/benchmarks.py` & `PyQuantimClient-1.0.9/src/benchmarks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import numpy as np
 import datetime as dt
 from .api import quantim
 
 class benchmarks(quantim):
-    def __init__(self, username, password, secretpool, env="pdn", api_url=None):
-        super().__init__(username, password, secretpool, env, api_url)
+    def __init__(self, username, password, secretpool, env="qa"):
+        super().__init__(username, password, secretpool, env)
 
     def load_constraints(self, file_name, sep=',', country='CO'):
         '''
         Load portfolio file to s3.
         '''
         if ~np.all(np.in1d(country, ['CO', 'CL', 'PE', 'MX', 'UY'])):
             raise ValueError('Country not supported.')
```

### Comparing `PyQuantimClient-1.0.83/src/data.py` & `PyQuantimClient-1.0.9/src/data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 import pandas as pd
 import numpy as np
 import datetime as dt
 from .api import quantim
 
 class time_series(quantim):
-    def __init__(self, username, password, secretpool, env="pdn", api_url=None):
-        super().__init__(username, password, secretpool, env, api_url)
+    def __init__(self, username, password, secretpool, env="qa"):
+        super().__init__(username, password, secretpool, env)
 
-    def get_series(self, tks, ref_curr='Origen', join='outer', verify=False):
+    def get_series(self, tks, ref_curr='Origen', join='outer'):
         '''
         Get series
         '''
         data = {'tks':list(tks), 'ref_curr':ref_curr, 'join':join}
-        resp = self.api_call('get_series', method="post", data=data, verify=verify)
-        ts, summ, tks_invalid = pd.DataFrame(resp['ts']).set_index("Date"), pd.DataFrame(resp['summ']), resp['tks_invalid']
-        return ts, summ, tks_invalid
+        resp = self.api_call('get_series', method="post", data=data, verify=False)
+        ref_curr, ts, summ = resp['ref_curr'], pd.DataFrame(resp['ts']).set_index("Date"), pd.DataFrame(resp['summ'])
+        return ref_curr, ts, summ
```

### Comparing `PyQuantimClient-1.0.83/src/energy.py` & `PyQuantimClient-1.0.9/src/energy.py`

 * *Files identical despite different names*

