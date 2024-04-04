# Comparing `tmp/tiegcmpy-1.2.5.tar.gz` & `tmp/tiegcmpy-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiegcmpy-1.2.5.tar", last modified: Fri Mar 22 21:37:19 2024, max compression
+gzip compressed data, was "tiegcmpy-1.2.6.tar", last modified: Thu Apr  4 15:16:39 2024, max compression
```

## Comparing `tiegcmpy-1.2.5.tar` & `tiegcmpy-1.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-03-22 21:37:18.039561 tiegcmpy-1.2.5/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-03-22 21:37:18.038675 tiegcmpy-1.2.5/PKG-INFO
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16164 2023-12-19 19:29:40.000000 tiegcmpy-1.2.5/README.md
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       38 2024-03-22 21:37:18.039658 tiegcmpy-1.2.5/setup.cfg
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      810 2024-03-20 14:29:17.000000 tiegcmpy-1.2.5/setup.py
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-03-22 21:37:17.717140 tiegcmpy-1.2.5/src/
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-03-22 21:37:18.033407 tiegcmpy-1.2.5/src/tiegcmpy/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      280 2023-12-19 18:21:34.000000 tiegcmpy-1.2.5/src/tiegcmpy/__init__.py
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)     1984 2023-10-18 21:02:51.000000 tiegcmpy-1.2.5/src/tiegcmpy/convert_units.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    42106 2023-12-06 02:37:57.000000 tiegcmpy-1.2.5/src/tiegcmpy/data_parse copy.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    50121 2024-03-22 14:36:32.000000 tiegcmpy-1.2.5/src/tiegcmpy/data_parse.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    43845 2023-12-04 20:38:48.000000 tiegcmpy-1.2.5/src/tiegcmpy/data_parse_old.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    16097 2023-12-19 20:29:36.000000 tiegcmpy-1.2.5/src/tiegcmpy/getoptions.py
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      683 2023-12-19 18:20:02.000000 tiegcmpy-1.2.5/src/tiegcmpy/io.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)     7391 2023-12-19 20:00:08.000000 tiegcmpy-1.2.5/src/tiegcmpy/main.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    35239 2023-12-05 15:26:08.000000 tiegcmpy-1.2.5/src/tiegcmpy/plot_gen copy.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    41528 2024-03-22 14:38:32.000000 tiegcmpy-1.2.5/src/tiegcmpy/plot_gen.py
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-03-22 21:37:18.037909 tiegcmpy-1.2.5/src/tiegcmpy.egg-info/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-03-22 21:37:14.000000 tiegcmpy-1.2.5/src/tiegcmpy.egg-info/PKG-INFO
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      503 2024-03-22 21:37:14.000000 tiegcmpy-1.2.5/src/tiegcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)        1 2024-03-22 21:37:14.000000 tiegcmpy-1.2.5/src/tiegcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       86 2024-03-22 21:37:14.000000 tiegcmpy-1.2.5/src/tiegcmpy.egg-info/entry_points.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       32 2024-03-22 21:37:14.000000 tiegcmpy-1.2.5/src/tiegcmpy.egg-info/requires.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)        9 2024-03-22 21:37:14.000000 tiegcmpy-1.2.5/src/tiegcmpy.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-04 15:16:39.242557 tiegcmpy-1.2.6/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-04-04 15:16:39.241600 tiegcmpy-1.2.6/PKG-INFO
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16164 2023-12-19 19:29:40.000000 tiegcmpy-1.2.6/README.md
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       38 2024-04-04 15:16:39.242705 tiegcmpy-1.2.6/setup.cfg
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      810 2024-04-04 15:12:35.000000 tiegcmpy-1.2.6/setup.py
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-04 15:16:39.165096 tiegcmpy-1.2.6/src/
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-04 15:16:39.233253 tiegcmpy-1.2.6/src/tiegcmpy/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      280 2023-12-19 18:21:34.000000 tiegcmpy-1.2.6/src/tiegcmpy/__init__.py
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)     1984 2023-10-18 21:02:51.000000 tiegcmpy-1.2.6/src/tiegcmpy/convert_units.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    42106 2023-12-06 02:37:57.000000 tiegcmpy-1.2.6/src/tiegcmpy/data_parse copy.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    50121 2024-03-22 14:36:32.000000 tiegcmpy-1.2.6/src/tiegcmpy/data_parse.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    43845 2023-12-04 20:38:48.000000 tiegcmpy-1.2.6/src/tiegcmpy/data_parse_old.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    16097 2023-12-19 20:29:36.000000 tiegcmpy-1.2.6/src/tiegcmpy/getoptions.py
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      683 2023-12-19 18:20:02.000000 tiegcmpy-1.2.6/src/tiegcmpy/io.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)     7391 2023-12-19 20:00:08.000000 tiegcmpy-1.2.6/src/tiegcmpy/main.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    35239 2023-12-05 15:26:08.000000 tiegcmpy-1.2.6/src/tiegcmpy/plot_gen copy.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    41531 2024-04-01 19:34:33.000000 tiegcmpy-1.2.6/src/tiegcmpy/plot_gen.py
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-04 15:16:39.240961 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      503 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)        1 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       86 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       32 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/requires.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)        9 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/top_level.txt
```

### Comparing `tiegcmpy-1.2.5/PKG-INFO` & `tiegcmpy-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiegcmpy
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python3 post processing tool for TIE-GCM
 Home-page: https://github.com/NCAR/tiegcm
 Author: Nikhil Rao
 Author-email: nikhilr@ucar.edu
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: cartopy
```

### Comparing `tiegcmpy-1.2.5/README.md` & `tiegcmpy-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/setup.py` & `tiegcmpy-1.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='tiegcmpy',
-    version='1.2.5',
+    version='1.2.6',
     author = "Nikhil Rao",
     author_email = "nikhilr@ucar.edu",
     description='A Python3 post processing tool for TIE-GCM',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NCAR/tiegcm', 
     python_requires='>=3.8',
```

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/convert_units.py` & `tiegcmpy-1.2.6/src/tiegcmpy/convert_units.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/data_parse copy.py` & `tiegcmpy-1.2.6/src/tiegcmpy/data_parse copy.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/data_parse.py` & `tiegcmpy-1.2.6/src/tiegcmpy/data_parse.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/data_parse_old.py` & `tiegcmpy-1.2.6/src/tiegcmpy/data_parse_old.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/getoptions.py` & `tiegcmpy-1.2.6/src/tiegcmpy/getoptions.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/io.py` & `tiegcmpy-1.2.6/src/tiegcmpy/io.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/main.py` & `tiegcmpy-1.2.6/src/tiegcmpy/main.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/plot_gen copy.py` & `tiegcmpy-1.2.6/src/tiegcmpy/plot_gen copy.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy/plot_gen.py` & `tiegcmpy-1.2.6/src/tiegcmpy/plot_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,17 +588,16 @@
 
     if mtime_minimum is not None and mtime_maximum is not None:
         new_mtime_values = []
         for t_mtime in mtime_values:
             mtime_total_minutes = t_mtime[0] * 24 * 60 *60 + t_mtime[1] * 60 *60+ t_mtime[2] *60+ t_mtime[3]
             mtime_min_total = mtime_minimum[0] * 24 * 60*60 + mtime_minimum[1] * 60 *60+ mtime_minimum[2]*60 + mtime_minimum[3]
             mtime_max_total = mtime_maximum[0] * 24 * 60*60 + mtime_maximum[1] * 60 *60+ mtime_maximum[2]*60 + mtime_minimum[3]
-        
-            if all(mtime_minimum[i] <= t <= mtime_maximum[i] for i, t in enumerate(t_mtime[:4])):
-                new_mtime_values.append(t_mtime)
+            if mtime_total_minutes >= mtime_min_total and mtime_total_minutes <= mtime_max_total:                
+                new_mtime_values.append(t_mtime)  
             else:
                 if mtime_total_minutes < mtime_min_total:
                     num_deleted_before += 1
                 elif mtime_total_minutes > mtime_max_total:
                     num_deleted_after += 1
         mtime_values = new_mtime_values
         mtime_values_sorted = sorted(mtime_values, key=lambda x: (x[0], x[1], x[2], x[3]))
@@ -711,17 +710,16 @@
 
     if mtime_minimum is not None and mtime_maximum is not None:
         new_mtime_values = []
         for t_mtime in mtime_values:
             mtime_total_minutes = t_mtime[0] * 24 * 60 *60 + t_mtime[1] * 60 *60+ t_mtime[2] *60+ t_mtime[3]
             mtime_min_total = mtime_minimum[0] * 24 * 60*60 + mtime_minimum[1] * 60 *60+ mtime_minimum[2]*60 + mtime_minimum[3]
             mtime_max_total = mtime_maximum[0] * 24 * 60*60 + mtime_maximum[1] * 60 *60+ mtime_maximum[2]*60 + mtime_minimum[3]
-        
-            if all(mtime_minimum[i] <= t <= mtime_maximum[i] for i, t in enumerate(t_mtime[:4])):
-                new_mtime_values.append(t_mtime)
+            if mtime_total_minutes >= mtime_min_total and mtime_total_minutes <= mtime_max_total:
+                new_mtime_values.append(t_mtime)   
             else:
                 if mtime_total_minutes < mtime_min_total:
                     num_deleted_before += 1
                 elif mtime_total_minutes > mtime_max_total:
                     num_deleted_after += 1
         mtime_values = new_mtime_values
         mtime_values_sorted = sorted(mtime_values, key=lambda x: (x[0], x[1], x[2], x[3]))
```

### Comparing `tiegcmpy-1.2.5/src/tiegcmpy.egg-info/PKG-INFO` & `tiegcmpy-1.2.6/src/tiegcmpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiegcmpy
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python3 post processing tool for TIE-GCM
 Home-page: https://github.com/NCAR/tiegcm
 Author: Nikhil Rao
 Author-email: nikhilr@ucar.edu
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: cartopy
```

