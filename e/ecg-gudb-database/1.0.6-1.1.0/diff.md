# Comparing `tmp/ecg_gudb_database-1.0.6.tar.gz` & `tmp/ecg_gudb_database-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ecg_gudb_database-1.0.6.tar", last modified: Mon Jun  8 11:28:38 2020, max compression
+gzip compressed data, was "ecg_gudb_database-1.1.0.tar", last modified: Thu Apr  4 09:18:51 2024, max compression
```

## Comparing `ecg_gudb_database-1.0.6.tar` & `ecg_gudb_database-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bp1       (1000) bp1       (1000)        0 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/
--rw-r--r--   0 bp1       (1000) bp1       (1000)     3658 2020-06-08 11:26:23.000000 ecg_gudb_database-1.0.6/README.md
--rw-r--r--   0 bp1       (1000) bp1       (1000)     2927 2020-06-08 10:34:49.000000 ecg_gudb_database-1.0.6/ecg_gudb_database.py
-drwxr-xr-x   0 bp1       (1000) bp1       (1000)        0 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/ecg_gudb_database.egg-info/
--rw-r--r--   0 bp1       (1000) bp1       (1000)       18 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/ecg_gudb_database.egg-info/top_level.txt
--rw-r--r--   0 bp1       (1000) bp1       (1000)     5565 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/ecg_gudb_database.egg-info/PKG-INFO
--rw-r--r--   0 bp1       (1000) bp1       (1000)        1 2020-06-06 13:29:54.000000 ecg_gudb_database-1.0.6/ecg_gudb_database.egg-info/not-zip-safe
--rw-r--r--   0 bp1       (1000) bp1       (1000)       12 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/ecg_gudb_database.egg-info/requires.txt
--rw-r--r--   0 bp1       (1000) bp1       (1000)      294 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/ecg_gudb_database.egg-info/SOURCES.txt
--rw-r--r--   0 bp1       (1000) bp1       (1000)        1 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/ecg_gudb_database.egg-info/dependency_links.txt
--rw-r--r--   0 bp1       (1000) bp1       (1000)     5565 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/PKG-INFO
--rwxr-xr-x   0 bp1       (1000) bp1       (1000)      771 2020-06-08 11:28:27.000000 ecg_gudb_database-1.0.6/setup.py
--rw-r--r--   0 bp1       (1000) bp1       (1000)       38 2020-06-08 11:28:38.000000 ecg_gudb_database-1.0.6/setup.cfg
--rw-r--r--   0 bp1       (1000) bp1       (1000)     4087 2020-06-08 11:27:23.000000 ecg_gudb_database-1.0.6/README.rst
+drwxrwxr-x   0 bp1       (1000) bp1       (1000)        0 2024-04-04 09:18:51.793501 ecg_gudb_database-1.1.0/
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)    19776 2024-04-04 09:13:48.000000 ecg_gudb_database-1.1.0/LICENSE
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     4512 2024-04-04 09:18:51.793501 ecg_gudb_database-1.1.0/PKG-INFO
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     4031 2024-04-04 09:17:48.000000 ecg_gudb_database-1.1.0/README.rst
+drwxrwxr-x   0 bp1       (1000) bp1       (1000)        0 2024-04-04 09:18:51.793501 ecg_gudb_database-1.1.0/ecg_gudb_database.egg-info/
+-rw-r--r--   0 bp1       (1000) bp1       (1000)     4512 2024-04-04 09:18:51.000000 ecg_gudb_database-1.1.0/ecg_gudb_database.egg-info/PKG-INFO
+-rw-r--r--   0 bp1       (1000) bp1       (1000)      292 2024-04-04 09:18:51.000000 ecg_gudb_database-1.1.0/ecg_gudb_database.egg-info/SOURCES.txt
+-rw-r--r--   0 bp1       (1000) bp1       (1000)        1 2024-04-04 09:18:51.000000 ecg_gudb_database-1.1.0/ecg_gudb_database.egg-info/dependency_links.txt
+-rw-r--r--   0 bp1       (1000) bp1       (1000)        1 2020-06-07 00:58:25.000000 ecg_gudb_database-1.1.0/ecg_gudb_database.egg-info/not-zip-safe
+-rw-r--r--   0 bp1       (1000) bp1       (1000)       12 2024-04-04 09:18:51.000000 ecg_gudb_database-1.1.0/ecg_gudb_database.egg-info/requires.txt
+-rw-r--r--   0 bp1       (1000) bp1       (1000)       18 2024-04-04 09:18:51.000000 ecg_gudb_database-1.1.0/ecg_gudb_database.egg-info/top_level.txt
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)     2927 2024-04-04 08:44:52.000000 ecg_gudb_database-1.1.0/ecg_gudb_database.py
+-rw-rw-r--   0 bp1       (1000) bp1       (1000)       38 2024-04-04 09:18:51.793501 ecg_gudb_database-1.1.0/setup.cfg
+-rwxrwxr-x   0 bp1       (1000) bp1       (1000)      771 2024-04-04 09:18:33.000000 ecg_gudb_database-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ecg_gudb_database-1.0.6/README.md` & `ecg_gudb_database-1.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,31 @@
-# High precision ECG Database with annotated R peaks, recorded and filmed under realistic conditions
+Metadata-Version: 2.1
+Name: ecg_gudb_database
+Version: 1.1.0
+Summary: API for a high precision ECG Database with annotated R peaks (GUDB)
+Home-page: https://github.com/berndporr/ECG-GUDB
+Author: Bernd Porr
+Author-email: bernd.porr@glasgow.ac.uk
+License: GPL 3.0
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==================================================================================================
+High precision ECG Database with annotated R peaks
+==================================================================================================
+
+This is a mirror of the ECG GUDB
+http://researchdata.gla.ac.uk/716/ and provides transparent online access via
+a python API.
 
-This is an API which provides transparent online access to the ECG GUDB
-http://researchdata.gla.ac.uk/716/ without the need of downloading it.
-
-DOI: 10.5525/gla.researchdata.716
-
-![Example of a dataset](https://berndporr.github.io/ECG-GUDB/dataplot.jpg)
+DOI: https://doi.org/10.5281/zenodo.10925419
 
 It contains ECGs from 25 subjects. Each subject was recorded performing 5 different tasks for two minutes:
    * sitting
    * a maths test on a tablet
    * walking on a treadmill
    * running on a treadmill
    * using a hand bike
@@ -25,100 +41,103 @@
 DC-coupled signals as originally recorded. In order to be able to link
 the ECG artefacts to the behaviour of the subject all but one subject
 gave permission to be filmed and the videos are also part of the
 database.
 
 
 
-## Installation
+Installation
+============
 
-Simply install via pip or pip3
+Simply install via pip or pip3::
+
+   pip install ecg_gudb_database
+   pip3 install ecg_gudb_database
 
-```
-pip install ecg_gudb_database
-pip3 install ecg_gudb_database
-```
 
    
-## Usage
+Usage
+=====
 
 Check out `usage_example.py` on github which plots the ECG and the heartrate of one subject.
 
 
-### Module
+Module
+------
+
+The module is called `ecg_gudb_database`::
 
-The module is called `ecg_gudb_database`:
+    from ecg_gudb_database import GUDb
 
-```
-from ecg_gudb_database import GUDb
-```
 
-The constructor loads the ECG data of one subject/experiment from github:
+The constructor loads the ECG data of one subject/experiment from github::
 
-```
-ecg_class = GUDb(subject_number, experiment)
-```
+    ecg_class = GUDb(subject_number, experiment)
 
 where `subject_number` is from 0..24 and `experiment` is 'sitting', 'maths', 'walking', 'hand_bike' or 'jogging'.
 The array `ecg_class.experiments` is an array of all experiments so that one can loop through the different experiments.
 
 Optionally, in case you decide later to download the whole dataset from http://researchdata.gla.ac.uk/716/ then
-specify the absolute path to the dataset with the optional parameter url without the "file:" specifier:
+specify the absolute path to the dataset with the optional parameter url without the "file:" specifier::
 
-```
-ecg_class = GUDb(subject_number, experiment, url = "/home/bp1/dataset_dataset_716/experiment_data/")
-```
+    ecg_class = GUDb(subject_number, experiment, url = "/home/bp1/dataset_dataset_716/experiment_data/")
 
-### Retrieve the ECG data
 
+Retrieve the ECG data
+---------------------
 
 The data is available as numpy arrays. The sampling rate is 250Hz for all experiments (`ecg_class.fs`).
 We have recorded Einthoven and from a chest strap.
 
-#### Einthoven
+Einthoven::
+
+    ecg_class.einthoven_I, ecg_class.einthoven_I_filt
+    ecg_class.einthoven_II, ecg_class.einthoven_II_filt
+    ecg_class.einthoven_III, ecg_class.einthoven_III_filt
+
+
+Chest strap::
 
-```
-ecg_class.einthoven_I, ecg_class.einthoven_I_filt
-ecg_class.einthoven_II, ecg_class.einthoven_II_filt
-ecg_class.einthoven_III, ecg_class.einthoven_III_filt
-```
-
-#### Chest strap
-
-```
-ecg_class.cs_V2_V1, ecg_class.cs_V2_V1_filt
-```
+    ecg_class.cs_V2_V1, ecg_class.cs_V2_V1_filt
 
 where the filtered versions have 50Hz mains and DC removed.
 
 
 
-#### R peak annotations
+R peak annotations
+------------------
 
 The two boolean variables `ecg_class.anno_cs_exists` and `ecg_class.anno_cables_exists`
-tell the user if annotations exist. If yes they can be obtained.
+tell the user if annotations exist. If yes they can be obtained::
 
-```
-ecg_class.anno_cs
-ecg_class.anno_cables
-```
 
-#### Accelerometer data
+    if ecg_class.anno_cs_exists:
+        chest_strap_anno = ecg_class.anno_cs
+    else:
+        print('No chest strap annotations')
+    if ecg_class.anno_cables_exists:
+        cables_anno = ecg_class.anno_cables
+    else:
+        print("No cables annotations")
 
-The accelerometer was worn on a standard belt around the subject's waist.
 
-```
-ecg_class.acc_x
-ecg_class.acc_y
-ecg_class.acc_z
-```
+Accelerometer data
+------------------
 
-## Videos and full dataset for offline use
+The accelerometer was worn on a standard belt around the subject's waist::
 
-Where the participant has consented, there is a video for each of the tasks. Here is an example: 
+    ecg_class.acc_x
+    ecg_class.acc_y
+    ecg_class.acc_z
 
-https://berndporr.github.io/ECG-GUDB/
 
+Videos and full dataset for offline use
+=======================================
+
+Where the participant has consented, there is a video for each of the tasks. Here is an example: 
+https://berndporr.github.io/ECG-GUDB/
 The video and ECG data have been synchronised so they start and end at the same time. The full dataset with the
 videos can be requested here:
 
 http://researchdata.gla.ac.uk/716/
+
+
```

### Comparing `ecg_gudb_database-1.0.6/ecg_gudb_database.py` & `ecg_gudb_database-1.1.0/ecg_gudb_database.py`

 * *Files identical despite different names*

### Comparing `ecg_gudb_database-1.0.6/setup.py` & `ecg_gudb_database-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='ecg_gudb_database',
-    version='1.0.6',
+    version='1.1.0',
     description="API for a high precision ECG Database with annotated R peaks (GUDB)",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     author='Bernd Porr',
     author_email='bernd.porr@glasgow.ac.uk',
     py_modules=['ecg_gudb_database'],
     install_requires=['numpy',
```

### Comparing `ecg_gudb_database-1.0.6/README.rst` & `ecg_gudb_database-1.1.0/ecg_gudb_database.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,31 @@
+Metadata-Version: 2.1
+Name: ecg-gudb-database
+Version: 1.1.0
+Summary: API for a high precision ECG Database with annotated R peaks (GUDB)
+Home-page: https://github.com/berndporr/ECG-GUDB
+Author: Bernd Porr
+Author-email: bernd.porr@glasgow.ac.uk
+License: GPL 3.0
+Platform: UNKNOWN
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ==================================================================================================
-High precision ECG Database with annotated R peaks, recorded and filmed under realistic conditions
+High precision ECG Database with annotated R peaks
 ==================================================================================================
 
-This is an API which provides transparent online access to the ECG GUDB
-http://researchdata.gla.ac.uk/716/ without the need of downloading it.
+This is a mirror of the ECG GUDB
+http://researchdata.gla.ac.uk/716/ and provides transparent online access via
+a python API.
 
-DOI: 10.5525/gla.researchdata.716
+DOI: https://doi.org/10.5281/zenodo.10925419
 
 It contains ECGs from 25 subjects. Each subject was recorded performing 5 different tasks for two minutes:
    * sitting
    * a maths test on a tablet
    * walking on a treadmill
    * running on a treadmill
    * using a hand bike
@@ -120,7 +136,8 @@
 Where the participant has consented, there is a video for each of the tasks. Here is an example: 
 https://berndporr.github.io/ECG-GUDB/
 The video and ECG data have been synchronised so they start and end at the same time. The full dataset with the
 videos can be requested here:
 
 http://researchdata.gla.ac.uk/716/
 
+
```

