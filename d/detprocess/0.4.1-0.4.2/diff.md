# Comparing `tmp/detprocess-0.4.1.tar.gz` & `tmp/detprocess-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detprocess-0.4.1.tar", last modified: Fri Mar 15 23:51:59 2024, max compression
+gzip compressed data, was "detprocess-0.4.2.tar", last modified: Thu Apr  4 17:09:06 2024, max compression
```

## Comparing `detprocess-0.4.1.tar` & `detprocess-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 23:51:59.667003 detprocess-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-15 23:51:55.000000 detprocess-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-03-15 23:51:59.667003 detprocess-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-03-15 23:51:55.000000 detprocess-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 23:51:59.663003 detprocess-0.4.1/detprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 23:51:59.667003 detprocess-0.4.1/detprocess/core/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29070 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    52506 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/didv.py
--rw-r--r--   0 runner    (1001) docker     (127)    15835 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/eventbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    30763 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/filterdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    59654 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/ivsweep.py
--rw-r--r--   0 runner    (1001) docker     (127)    22110 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    19125 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/oftrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/core/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 23:51:59.667003 detprocess-0.4.1/detprocess/process/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49449 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/process/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    35001 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/process/ivprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/process/processing_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    32572 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/process/randoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    37391 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/process/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 23:51:59.667003 detprocess-0.4.1/detprocess/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-03-15 23:51:55.000000 detprocess-0.4.1/detprocess/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 23:51:59.667003 detprocess-0.4.1/detprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-03-15 23:51:59.000000 detprocess-0.4.1/detprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-15 23:51:59.000000 detprocess-0.4.1/detprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 23:51:59.000000 detprocess-0.4.1/detprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 23:51:59.000000 detprocess-0.4.1/detprocess.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-15 23:51:59.000000 detprocess-0.4.1/detprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-15 23:51:59.000000 detprocess-0.4.1/detprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-15 23:51:55.000000 detprocess-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 23:51:59.667003 detprocess-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-03-15 23:51:55.000000 detprocess-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:09:06.658903 detprocess-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 17:09:02.000000 detprocess-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-04 17:09:06.658903 detprocess-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-04 17:09:02.000000 detprocess-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:09:06.650902 detprocess-0.4.2/detprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:09:06.654903 detprocess-0.4.2/detprocess/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29070 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52506 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/didv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15835 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/eventbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30763 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/filterdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59654 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/ivsweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22110 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19125 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/oftrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/core/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:09:06.654903 detprocess-0.4.2/detprocess/process/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/process/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35001 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/process/ivprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/process/processing_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32572 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/process/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37391 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/process/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:09:06.654903 detprocess-0.4.2/detprocess/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-04 17:09:02.000000 detprocess-0.4.2/detprocess/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:09:06.654903 detprocess-0.4.2/detprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7000 2024-04-04 17:09:06.000000 detprocess-0.4.2/detprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 17:09:06.000000 detprocess-0.4.2/detprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:09:06.000000 detprocess-0.4.2/detprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:09:06.000000 detprocess-0.4.2/detprocess.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-04 17:09:06.000000 detprocess-0.4.2/detprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 17:09:06.000000 detprocess-0.4.2/detprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 17:09:02.000000 detprocess-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:09:06.658903 detprocess-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-04 17:09:02.000000 detprocess-0.4.2/setup.py
```

### Comparing `detprocess-0.4.1/LICENSE` & `detprocess-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/PKG-INFO` & `detprocess-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: detprocess
-Version: 0.4.1
+Version: 0.4.2
 Summary: Detector Data Processing Package
 Home-page: https://github.com/spice-herald/detprocess
 Author: Bruno Serfass, Samuel Watkins
 Author-email: serfass@berkeley.edu, samwatkins@berkeley.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: pyyaml
-Requires-Dist: qetpy>=1.6.4
+Requires-Dist: qetpy>=1.6.8
 Requires-Dist: pandas
-Requires-Dist: pytesdaq>=0.3.7
+Requires-Dist: pytesdaq>=0.3.9
 Requires-Dist: scikit-image
 Requires-Dist: iminuit>=2
 Requires-Dist: seaborn
 Requires-Dist: humanfriendly
 Requires-Dist: vaex
 
 #  `detprocess`: Detector processing code for feature extraction
```

### Comparing `detprocess-0.4.1/README.md` & `detprocess-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/core/algorithms.py` & `detprocess-0.4.2/detprocess/core/algorithms.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/core/didv.py` & `detprocess-0.4.2/detprocess/core/didv.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/core/eventbuilder.py` & `detprocess-0.4.2/detprocess/core/eventbuilder.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/core/filterdata.py` & `detprocess-0.4.2/detprocess/core/filterdata.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/core/ivsweep.py` & `detprocess-0.4.2/detprocess/core/ivsweep.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/core/noise.py` & `detprocess-0.4.2/detprocess/core/noise.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/core/oftrigger.py` & `detprocess-0.4.2/detprocess/core/oftrigger.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/core/template.py` & `detprocess-0.4.2/detprocess/core/template.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/process/features.py` & `detprocess-0.4.2/detprocess/process/features.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 warnings.filterwarnings('ignore')
 
 
 __all__ = [
     'FeatureProcessing'
 ]
 
-
-
 class FeatureProcessing:
     """
     Class to manage data processing and 
     extract features, dataframe can be saved
     in hdf5 using vaex framework and returned
     as a pandas dataframe (not both)
 
@@ -104,45 +102,56 @@
 
         # processing id
         self._processing_id = processing_id
 
         # restricted data
         self._restricted = restricted
         
-        
         # display
         self._verbose = verbose
 
+        # series argument (FIXME: filter solely based raw data series?)
+        #  -> raw data series if no dataframe
+        #  -> dataframe series if trigger_dataframe_path
+        raw_series = None
+        dataframe_series = None
+        if trigger_dataframe_path is not None:
+            dataframe_series = series
+        else:
+            raw_series = series 
+             
         # Raw file list
         raw_files, raw_path, group_name = (
             self._get_file_list(raw_path,
-                                series=series,
+                                series=raw_series,
                                 restricted=restricted)
         )
+
         if not raw_files:
             raise ValueError('No raw data files were found! '
                              + 'Check configuration...')
         self._series_list = list(raw_files.keys())
         self._input_group_name = str(group_name)
-        
+      
         # Dataframe file list
         trigger_files = None
         trigger_path = None
         trigger_group_name = None
         
         if trigger_dataframe_path is not None:
-            
+                   
             trigger_files, trigger_path, trigger_group_name = (
                 self._get_file_list(trigger_dataframe_path,
+                                    series=dataframe_series,
                                     is_raw=False,
                                     restricted=restricted)
             )
             if not trigger_files:
-                raise ValueError('No dataframe files were found! '
-                                 + 'Check configuration...')
+                raise ValueError(f'No dataframe files were found! '
+                                 f'Check configuration...')
             
             self._series_list = list(trigger_files.keys())
 
 
         # get list of available channels in raw data
         available_channels = self._get_channel_list(raw_files)
             
@@ -304,15 +313,15 @@
                                       output_group_path,
                                       memory_limit)
 
         else:
             
             # split data
             series_list_split = self._split_series(ncores)
-            
+        
             # for multi-core processing, we need to decrease the
             # max memory so it fits in RAM
             memory_limit /= ncores
 
               
             # lauch pool processing
             if self._verbose:
@@ -392,24 +401,21 @@
    
         """
 
         # node string (for display)
         node_num_str = str()
         if node_num>-1:
             node_num_str = ' Node #' + str(node_num)
-        
-
+    
         # feature extractors
         FE = FeatureExtractors
         FE_ext = None
         if self._external_file is not None:
             FE_ext = self._load_external_extractors(self._external_file)
 
-
-
         # output file name base
         output_base_file = None
         if lgc_save:
             
             file_prefix = 'feature'
             if self._processing_id is not None:
                 file_prefix = self._processing_id + '_feature'
@@ -494,15 +500,15 @@
                     or memory_limit_reached):
                     
                     # save file if needed
                     if lgc_save:
                         
                         # build hdf5 file name
                         dump_str = str(dump_counter)
-                        dump_str ='_F' + dump_str.zfill(4)
+                        dump_str = '_F' + dump_str.zfill(4)
                         file_name =  output_base_file +  dump_str + '.hdf5'
                     
                         # convert to vaex
                         feature_vx = vx.from_pandas(feature_df,
                                                     copy_index=False)
 
 
@@ -702,17 +708,18 @@
                             feature_name = f'{feature_base_name}_{feature_channel}'
                             event_features.update(
                                 {feature_name: extracted_features[feature_base_name]}
                             )
 
                 # done processing event!
                 # append event dictionary to dataframe
-                feature_df = feature_df.append(event_features,
-                                               ignore_index=True)
-           
+                event_df = pd.DataFrame([event_features])
+                feature_df = pd.concat([feature_df, event_df],
+                                       ignore_index=True)
+                         
         # return features
         return feature_df
        
 
 
         
         
@@ -814,25 +821,37 @@
                             for it_series in series:
                                 if a_path.find(it_series) != -1:
                                     file_list.append(a_path)
                     else:
                         file_list.append(a_path)
 
             else:
-                raise ValueError('File or directory "' + a_path
-                                 + '" does not exist!')
+                raise ValueError(f'File or directory "{a_path}" '
+                                 f'does not exist!')
             
         if not file_list:
-            raise ValueError('ERROR: No raw input data found. Check arguments!')
+            if is_raw:
+                msg = ('No input raw data found. '
+                       'Check data path! ')
+                if series is not None:
+                    msg = msg + ' Or check "series" argument.'
+                raise ValueError(msg)
+            else:
+                msg = ('No input dataframe vaex files found. '
+                       'Check data path!')
+                if series is not None:
+                    msg = (msg
+                           + ' Or check "series" argument (it should be '
+                           + '"series" of dataframe files, not raw data)')
+                raise ValueError(msg)
+            
 
         # sort
         file_list.sort()
 
-
-        
       
         # convert to series dictionary so can be easily split
         # in multiple cores
         
         series_dict = dict()
         h5reader = h5io.H5Reader()
         series_name = None
@@ -1323,15 +1342,14 @@
         series_split = np.array_split(self._series_list, ncores)
 
         # remove empty array
         for series_sublist in series_split:
             if series_sublist.size == 0:
                 continue
             output_list.append(list(series_sublist))
-            
 
         return output_list
 
     
 
     
     def _get_channel_list(self, file_dict):
```

### Comparing `detprocess-0.4.1/detprocess/process/ivprocess.py` & `detprocess-0.4.2/detprocess/process/ivprocess.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/process/processing_data.py` & `detprocess-0.4.2/detprocess/process/processing_data.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/process/randoms.py` & `detprocess-0.4.2/detprocess/process/randoms.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/process/triggers.py` & `detprocess-0.4.2/detprocess/process/triggers.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess/utils/utils.py` & `detprocess-0.4.2/detprocess/utils/utils.py`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/detprocess.egg-info/PKG-INFO` & `detprocess-0.4.2/detprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: detprocess
-Version: 0.4.1
+Version: 0.4.2
 Summary: Detector Data Processing Package
 Home-page: https://github.com/spice-herald/detprocess
 Author: Bruno Serfass, Samuel Watkins
 Author-email: serfass@berkeley.edu, samwatkins@berkeley.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: pyyaml
-Requires-Dist: qetpy>=1.6.4
+Requires-Dist: qetpy>=1.6.8
 Requires-Dist: pandas
-Requires-Dist: pytesdaq>=0.3.7
+Requires-Dist: pytesdaq>=0.3.9
 Requires-Dist: scikit-image
 Requires-Dist: iminuit>=2
 Requires-Dist: seaborn
 Requires-Dist: humanfriendly
 Requires-Dist: vaex
 
 #  `detprocess`: Detector processing code for feature extraction
```

### Comparing `detprocess-0.4.1/detprocess.egg-info/SOURCES.txt` & `detprocess-0.4.2/detprocess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `detprocess-0.4.1/setup.py` & `detprocess-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                     # Die if path in CLEAN_FILES is absolute + outside this directory
                     raise ValueError("%s is not a path inside %s" % (path, here))
                 print('removing %s' % os.path.relpath(path))
                 shutil.rmtree(path)
 
 setup(
     name="detprocess",
-    version="0.4.1",
+    version="0.4.2",
     description="Detector Data Processing Package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Bruno Serfass, Samuel Watkins",
     author_email="serfass@berkeley.edu, samwatkins@berkeley.edu",
     url="https://github.com/spice-herald/detprocess",
     license_files = ('LICENSE', ),
@@ -50,17 +50,17 @@
         'clean': CleanCommand,
     },
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'pyyaml',
-        'qetpy>=1.6.4',
+        'qetpy>=1.6.8',
         'pandas',
-        'pytesdaq>=0.3.7',
+        'pytesdaq>=0.3.9',
         'scikit-image',
         'iminuit>=2',
         'seaborn',
         'humanfriendly',
         'vaex',
     ],
 )
```

