# Comparing `tmp/copasi-petab-importer-1.0.6.tar.gz` & `tmp/copasi-petab-importer-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copasi-petab-importer-1.0.6.tar", last modified: Mon Sep 25 11:22:19 2023, max compression
+gzip compressed data, was "copasi-petab-importer-1.0.7.tar", last modified: Thu Apr  4 21:06:13 2024, max compression
```

## Comparing `copasi-petab-importer-1.0.6.tar` & `copasi-petab-importer-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-09-25 11:22:19.587223 copasi-petab-importer-1.0.6/
--rw-r--r--   0 frank      (501) staff       (20)       64 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.6/MANIFEST.in
--rw-r--r--   0 frank      (501) staff       (20)      279 2023-09-25 11:22:19.587264 copasi-petab-importer-1.0.6/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)     3714 2023-05-03 06:40:46.000000 copasi-petab-importer-1.0.6/README.md
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-09-25 11:22:19.587529 copasi-petab-importer-1.0.6/copasi_petab_importer/
--rw-r--r--   0 frank      (501) staff       (20)     9163 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.6/copasi_petab_importer/PEtab.py
--rw-r--r--   0 frank      (501) staff       (20)      351 2023-05-16 13:46:05.000000 copasi-petab-importer-1.0.6/copasi_petab_importer/__init__.py
--rw-r--r--   0 frank      (501) staff       (20)      497 2023-09-25 11:22:19.587554 copasi-petab-importer-1.0.6/copasi_petab_importer/_version.py
--rw-r--r--   0 frank      (501) staff       (20)     1899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.6/copasi_petab_importer/convert_all_petab.py
--rw-r--r--   0 frank      (501) staff       (20)     4579 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.6/copasi_petab_importer/convert_benchmark.py
--rw-r--r--   0 frank      (501) staff       (20)    39765 2023-09-25 11:18:26.000000 copasi-petab-importer-1.0.6/copasi_petab_importer/convert_petab.py
--rw-r--r--   0 frank      (501) staff       (20)    12270 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.6/copasi_petab_importer/petab.ui
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-09-25 11:22:19.586886 copasi-petab-importer-1.0.6/copasi_petab_importer.egg-info/
--rw-r--r--   0 frank      (501) staff       (20)      279 2023-09-25 11:22:19.000000 copasi-petab-importer-1.0.6/copasi_petab_importer.egg-info/PKG-INFO
--rw-r--r--   0 frank      (501) staff       (20)      603 2023-09-25 11:22:19.000000 copasi-petab-importer-1.0.6/copasi_petab_importer.egg-info/SOURCES.txt
--rw-r--r--   0 frank      (501) staff       (20)        1 2023-09-25 11:22:19.000000 copasi-petab-importer-1.0.6/copasi_petab_importer.egg-info/dependency_links.txt
--rw-r--r--   0 frank      (501) staff       (20)      138 2023-09-25 11:22:19.000000 copasi-petab-importer-1.0.6/copasi_petab_importer.egg-info/entry_points.txt
--rw-r--r--   0 frank      (501) staff       (20)       62 2023-09-25 11:22:19.000000 copasi-petab-importer-1.0.6/copasi_petab_importer.egg-info/requires.txt
--rw-r--r--   0 frank      (501) staff       (20)       22 2023-09-25 11:22:19.000000 copasi-petab-importer-1.0.6/copasi_petab_importer.egg-info/top_level.txt
--rw-r--r--   0 frank      (501) staff       (20)      243 2023-09-25 11:22:19.587430 copasi-petab-importer-1.0.6/setup.cfg
--rw-r--r--   0 frank      (501) staff       (20)      899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.6/setup.py
-drwxr-xr-x   0 frank      (501) staff       (20)        0 2023-09-25 11:22:19.587010 copasi-petab-importer-1.0.6/test/
--rw-r--r--   0 frank      (501) staff       (20)     2940 2023-05-25 08:44:48.000000 copasi-petab-importer-1.0.6/test/test_importer.py
--rw-r--r--   0 frank      (501) staff       (20)    78254 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.6/versioneer.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-04-04 21:06:13.194181 copasi-petab-importer-1.0.7/
+-rw-r--r--   0 frank      (501) staff       (20)      138 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/.flake8
+-rw-r--r--   0 frank      (501) staff       (20)       47 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/.gitattributes
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-04-04 21:06:13.184718 copasi-petab-importer-1.0.7/.github/
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-04-04 21:06:13.187215 copasi-petab-importer-1.0.7/.github/workflows/
+-rw-r--r--   0 frank      (501) staff       (20)     1083 2023-05-26 07:42:40.000000 copasi-petab-importer-1.0.7/.github/workflows/build.yml
+-rw-r--r--   0 frank      (501) staff       (20)      145 2023-05-25 14:28:10.000000 copasi-petab-importer-1.0.7/.gitignore
+-rw-r--r--   0 frank      (501) staff       (20)      105 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/.gitmodules
+-rw-r--r--   0 frank      (501) staff       (20)       64 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/MANIFEST.in
+-rw-r--r--   0 frank      (501) staff       (20)      279 2024-04-04 21:06:13.194253 copasi-petab-importer-1.0.7/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)     3714 2023-05-03 06:40:46.000000 copasi-petab-importer-1.0.7/README.md
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-04-04 21:06:13.194653 copasi-petab-importer-1.0.7/copasi_petab_importer/
+-rw-r--r--   0 frank      (501) staff       (20)     9163 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/copasi_petab_importer/PEtab.py
+-rw-r--r--   0 frank      (501) staff       (20)      351 2023-05-16 13:46:05.000000 copasi-petab-importer-1.0.7/copasi_petab_importer/__init__.py
+-rw-r--r--   0 frank      (501) staff       (20)      497 2024-04-04 21:06:13.194685 copasi-petab-importer-1.0.7/copasi_petab_importer/_version.py
+-rw-r--r--   0 frank      (501) staff       (20)     1899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/copasi_petab_importer/convert_all_petab.py
+-rw-r--r--   0 frank      (501) staff       (20)     4599 2024-04-04 20:52:29.000000 copasi-petab-importer-1.0.7/copasi_petab_importer/convert_benchmark.py
+-rw-r--r--   0 frank      (501) staff       (20)    39805 2024-04-04 20:52:40.000000 copasi-petab-importer-1.0.7/copasi_petab_importer/convert_petab.py
+-rw-r--r--   0 frank      (501) staff       (20)    12270 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/copasi_petab_importer/petab.ui
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-04-04 21:06:13.189737 copasi-petab-importer-1.0.7/copasi_petab_importer.egg-info/
+-rw-r--r--   0 frank      (501) staff       (20)      279 2024-04-04 21:06:13.000000 copasi-petab-importer-1.0.7/copasi_petab_importer.egg-info/PKG-INFO
+-rw-r--r--   0 frank      (501) staff       (20)      719 2024-04-04 21:06:13.000000 copasi-petab-importer-1.0.7/copasi_petab_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 frank      (501) staff       (20)        1 2024-04-04 21:06:13.000000 copasi-petab-importer-1.0.7/copasi_petab_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 frank      (501) staff       (20)      138 2024-04-04 21:06:13.000000 copasi-petab-importer-1.0.7/copasi_petab_importer.egg-info/entry_points.txt
+-rw-r--r--   0 frank      (501) staff       (20)       62 2024-04-04 21:06:13.000000 copasi-petab-importer-1.0.7/copasi_petab_importer.egg-info/requires.txt
+-rw-r--r--   0 frank      (501) staff       (20)       22 2024-04-04 21:06:13.000000 copasi-petab-importer-1.0.7/copasi_petab_importer.egg-info/top_level.txt
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-04-04 21:06:13.189850 copasi-petab-importer-1.0.7/doc/
+-rw-r--r--   0 frank      (501) staff       (20)  4604148 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/doc/demo.gif
+-rw-r--r--   0 frank      (501) staff       (20)     9093 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/license.txt
+-rw-r--r--   0 frank      (501) staff       (20)       54 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/requirements.txt
+-rw-r--r--   0 frank      (501) staff       (20)      243 2024-04-04 21:06:13.194497 copasi-petab-importer-1.0.7/setup.cfg
+-rw-r--r--   0 frank      (501) staff       (20)      899 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/setup.py
+drwxr-xr-x   0 frank      (501) staff       (20)        0 2024-04-04 21:06:13.193904 copasi-petab-importer-1.0.7/test/
+-rw-r--r--   0 frank      (501) staff       (20)     2940 2023-05-25 08:44:48.000000 copasi-petab-importer-1.0.7/test/test_importer.py
+-rw-r--r--   0 frank      (501) staff       (20)    78254 2023-04-17 21:22:23.000000 copasi-petab-importer-1.0.7/versioneer.py
```

### Comparing `copasi-petab-importer-1.0.6/README.md` & `copasi-petab-importer-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.6/copasi_petab_importer/PEtab.py` & `copasi-petab-importer-1.0.7/copasi_petab_importer/PEtab.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.6/copasi_petab_importer/convert_all_petab.py` & `copasi-petab-importer-1.0.7/copasi_petab_importer/convert_all_petab.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.6/copasi_petab_importer/convert_benchmark.py` & `copasi-petab-importer-1.0.7/copasi_petab_importer/convert_benchmark.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 
         lower = pow(10.0, float(current['lower boundary']))
         upper = pow(10.0, float(current['upper boundary']))
         value = pow(10.0, float(current['value']))
 
         # if we found it, get its internal identifier and create the item
         item = problem.addOptItem(cn)
-        item.setLowerBound(COPASI.CCommonName(str(lower)))   # set the lower
-        item.setUpperBound(COPASI.CCommonName(str(upper)))   # and upper bound
+        item.setLowerBound(COPASI.CRegisteredCommonName(str(lower)))   # set the lower
+        item.setUpperBound(COPASI.CRegisteredCommonName(str(upper)))   # and upper bound
         item.setStartValue(value)                # as well as the initial value
 
 
 def convert_benchmark(sbml_file, data_file, info_file, output_dir, out_name):
     parameters = get_parameters_from_info_file(info_file)
     data = get_experimental_data(data_file)
     exp_file_name = os.path.join(output_dir,
```

### Comparing `copasi-petab-importer-1.0.6/copasi_petab_importer/convert_petab.py` & `copasi-petab-importer-1.0.7/copasi_petab_importer/convert_petab.py`

 * *Files 2% similar despite different names*

```diff
@@ -746,18 +746,18 @@
             cn = obj.getInitialValueReference().getCN()
 
             # if we found it, we can get its internal identifier and create
             # the item
             item = problem.addOptItem(cn)
             if np.isnan(lower):
                 lower = math.pow(10, -6)
-            item.setLowerBound(COPASI.CCommonName(str(lower)))
+            item.setLowerBound(COPASI.CRegisteredCommonName(str(lower)))
             if np.isnan(upper):
                 upper = math.pow(10, 6)
-            item.setUpperBound(COPASI.CCommonName(str(upper)))
+            item.setUpperBound(COPASI.CRegisteredCommonName(str(upper)))
             item.setStartValue(value)  # as well as the initial value
 
         # create experiment specific fit items
         for condition in self.ignore_independent:
             for name in self.ignore_independent[condition]:
                 parameterId = self.ignore_independent[condition][name]
                 obj = dm.findObjectByDisplayName(str('Values[' + name + ']'))
@@ -795,18 +795,18 @@
                     cn = obj.getInitialValueReference().getCN()
 
                 # if we found it, we can get its internal identifier and create
                 # the item
                 item = problem.addFitItem(cn)
                 if np.isnan(lower):
                     lower = math.pow(10, -6)
-                item.setLowerBound(COPASI.CCommonName(str(lower)))
+                item.setLowerBound(COPASI.CRegisteredCommonName(str(lower)))
                 if np.isnan(upper):
                     upper = math.pow(10, 6)
-                item.setUpperBound(COPASI.CCommonName(str(upper)))
+                item.setUpperBound(COPASI.CRegisteredCommonName(str(upper)))
                 item.setStartValue(value)  # as well as the initial value
                 item.addExperiment(self.experiment_to_key[condition])
 
     def convert_petab_fromdir(self, petab_dir, model_name, out_dir, out_name):
         petab = PEtabProblem(petab_dir, model_name)
         self.generate_copasi_file(petab, out_dir, out_name)
```

### Comparing `copasi-petab-importer-1.0.6/copasi_petab_importer/petab.ui` & `copasi-petab-importer-1.0.7/copasi_petab_importer/petab.ui`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.6/setup.py` & `copasi-petab-importer-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.6/test/test_importer.py` & `copasi-petab-importer-1.0.7/test/test_importer.py`

 * *Files identical despite different names*

### Comparing `copasi-petab-importer-1.0.6/versioneer.py` & `copasi-petab-importer-1.0.7/versioneer.py`

 * *Files identical despite different names*

