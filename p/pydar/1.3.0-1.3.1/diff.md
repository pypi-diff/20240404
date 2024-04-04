# Comparing `tmp/pydar-1.3.0.tar.gz` & `tmp/pydar-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydar-1.3.0.tar", last modified: Mon Feb 26 01:20:29 2024, max compression
+gzip compressed data, was "pydar-1.3.1.tar", last modified: Thu Apr  4 07:28:03 2024, max compression
```

## Comparing `pydar-1.3.0.tar` & `pydar-1.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-26 01:20:29.553428 pydar-1.3.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1067 2024-01-24 02:24:32.000000 pydar-1.3.0/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       25 2024-01-24 02:24:32.000000 pydar-1.3.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)    44143 2024-02-26 01:20:29.549428 pydar-1.3.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    42664 2024-02-26 00:59:19.000000 pydar-1.3.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-26 01:20:29.541428 pydar-1.3.0/pydar/
--rw-rw-r--   0 user      (1000) user      (1000)     2345 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-26 01:20:29.549428 pydar-1.3.0/pydar/data/
--rw-rw-r--   0 user      (1000) user      (1000)     1218 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/data/cassini_flyby.csv
--rw-rw-r--   0 user      (1000) user      (1000)    15662 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/data/coradr_jpl_options.csv
--rw-rw-r--   0 user      (1000) user      (1000)    30062 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/data/feature_name_details.csv
--rw-rw-r--   0 user      (1000) user      (1000)    36144 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/data/sar_swath_details.csv
--rw-rw-r--   0 user      (1000) user      (1000)   545452 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/data/swath_coverage_by_time_position.csv
--rw-rw-r--   0 user      (1000) user      (1000)     1932 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/display_image.py
--rw-rw-r--   0 user      (1000) user      (1000)    17718 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)    15452 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/extract_flyby_parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)      259 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/pydar_testing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-26 01:20:29.549428 pydar-1.3.0/pydar/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     3185 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/pytests/test_display_image.py
--rw-rw-r--   0 user      (1000) user      (1000)    10469 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/pytests/test_extract_flyby_parameters.py
--rw-rw-r--   0 user      (1000) user      (1000)     7593 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/pytests/test_read_readme.py
--rw-rw-r--   0 user      (1000) user      (1000)    26633 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/pytests/test_retrieve_ids_by_time_position.py
--rw-rw-r--   0 user      (1000) user      (1000)    12390 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/read_readme.py
--rw-rw-r--   0 user      (1000) user      (1000)    14052 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/retrieve_ids_by_time_position.py
--rw-rw-r--   0 user      (1000) user      (1000)     4054 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/retrieve_supplementary_backplanes.py
--rw-rw-r--   0 user      (1000) user      (1000)    12254 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/sbdr_make_shapefile.py
--rw-rw-r--   0 user      (1000) user      (1000)      211 2024-02-26 01:14:21.000000 pydar-1.3.0/pydar/sbdr_tester_shapefile.py
--rw-rw-r--   0 user      (1000) user      (1000)      969 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/test_bearing_correction.py
--rw-rw-r--   0 user      (1000) user      (1000)     4011 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/updateCsvCORADARJPLOptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     5063 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/updateCsvFeatureNameDetails.py
--rw-rw-r--   0 user      (1000) user      (1000)     6596 2024-01-24 02:24:32.000000 pydar-1.3.0/pydar/updateCsvSwathCoverage.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-02-26 01:20:29.545428 pydar-1.3.0/pydar.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    44143 2024-02-26 01:20:29.000000 pydar-1.3.0/pydar.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      953 2024-02-26 01:20:29.000000 pydar-1.3.0/pydar.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-02-26 01:20:29.000000 pydar-1.3.0/pydar.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      127 2024-02-26 01:20:29.000000 pydar-1.3.0/pydar.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2024-02-26 01:20:29.000000 pydar-1.3.0/pydar.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-02-26 01:20:29.553428 pydar-1.3.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1710 2024-02-26 01:12:00.000000 pydar-1.3.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-04 07:28:03.650187 pydar-1.3.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     1067 2024-02-26 01:32:11.000000 pydar-1.3.1/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       25 2024-02-26 01:32:11.000000 pydar-1.3.1/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)    44897 2024-04-04 07:28:03.650187 pydar-1.3.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    43350 2024-04-02 07:14:48.000000 pydar-1.3.1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-04 07:28:03.646187 pydar-1.3.1/pydar/
+-rw-rw-r--   0 user      (1000) user      (1000)     2345 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-04 07:28:03.650187 pydar-1.3.1/pydar/data/
+-rw-rw-r--   0 user      (1000) user      (1000)     1218 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/data/cassini_flyby.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    15662 2024-04-02 06:47:09.000000 pydar-1.3.1/pydar/data/coradr_jpl_options.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    30150 2024-04-02 07:07:31.000000 pydar-1.3.1/pydar/data/feature_name_details.csv
+-rw-rw-r--   0 user      (1000) user      (1000)    36144 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/data/sar_swath_details.csv
+-rw-rw-r--   0 user      (1000) user      (1000)   545452 2024-04-02 07:04:46.000000 pydar-1.3.1/pydar/data/swath_coverage_by_time_position.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     1932 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/display_image.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17719 2024-03-19 07:13:59.000000 pydar-1.3.1/pydar/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15451 2024-03-19 07:14:50.000000 pydar-1.3.1/pydar/extract_flyby_parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)      259 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/pydar_testing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-04 07:28:03.650187 pydar-1.3.1/pydar/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     3185 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/pytests/test_error_display_image.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10469 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/pytests/test_error_extract_flyby_parameters.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7593 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/pytests/test_error_read_readme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    26641 2024-04-02 07:19:42.000000 pydar-1.3.1/pydar/pytests/test_error_retrieve_ids_by_time_position.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12394 2024-03-19 07:16:39.000000 pydar-1.3.1/pydar/read_readme.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13980 2024-03-01 06:37:58.000000 pydar-1.3.1/pydar/retrieve_ids_by_time_position.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4054 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/retrieve_supplementary_backplanes.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12254 2024-03-19 07:17:37.000000 pydar-1.3.1/pydar/sbdr_make_shapefile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      211 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/sbdr_tester_shapefile.py
+-rw-rw-r--   0 user      (1000) user      (1000)      969 2024-02-26 01:32:12.000000 pydar-1.3.1/pydar/test_bearing_correction.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4012 2024-03-19 07:18:22.000000 pydar-1.3.1/pydar/updateCsvCORADARJPLOptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5078 2024-03-19 07:18:38.000000 pydar-1.3.1/pydar/updateCsvFeatureNameDetails.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6597 2024-03-19 07:18:58.000000 pydar-1.3.1/pydar/updateCsvSwathCoverage.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-04-04 07:28:03.650187 pydar-1.3.1/pydar.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    44897 2024-04-04 07:28:03.000000 pydar-1.3.1/pydar.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      977 2024-04-04 07:28:03.000000 pydar-1.3.1/pydar.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-04-04 07:28:03.000000 pydar-1.3.1/pydar.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       68 2024-04-04 07:28:03.000000 pydar-1.3.1/pydar.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2024-04-04 07:28:03.000000 pydar-1.3.1/pydar.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-04-04 07:28:03.650187 pydar-1.3.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1774 2024-04-04 07:17:39.000000 pydar-1.3.1/setup.py
```

### Comparing `pydar-1.3.0/LICENSE` & `pydar-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/PKG-INFO` & `pydar-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: pydar
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python package to access, download, view, and manipulate Cassini RADAR images
 Home-page: https://github.com/unaschneck/pydar
-Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.3.0.tar.gz
+Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.3.1.tar.gz
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
+Keywords: geophysics,python,astronomy,nasa,radar,planetary-science,cassini,jpl
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beautifulsoup4>=4.11.1
-Requires-Dist: matplotlib>=3.1.0
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: pdr>=0.7.3
-Requires-Dist: pyproj>=3.4.1
-Requires-Dist: pytest>=7.2.2
-Requires-Dist: rasterio>=1.3.6
-Requires-Dist: urllib3>=1.26.18
+Requires-Dist: beautifulsoup4
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: pdr
+Requires-Dist: pyproj
+Requires-Dist: pytest
+Requires-Dist: rasterio
+Requires-Dist: urllib3
 
 # PYDAR
  <p align="center">
   <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
 </p>
 
 ![PyPi](https://img.shields.io/pypi/v/pydar)
 ![license](https://img.shields.io/pypi/l/pydar)
+[![repo-status](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
 ![PyPi-Versions](https://img.shields.io/pypi/pyversions/pydar)
 [![update-dynamic-csv-data-files](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml)
 [![pytests](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml)
 
 A Python package to access, download, view, and manipulate Cassini RADAR images in one place
 
@@ -75,15 +78,17 @@
 
 ```
 pip install pydar
 ```
 
 ## Quickstart: PYDAR
 
-All Cassini data for Titan is retrieved based on flyby observation numbers or IDs, so relevant flybys can be found based on time range, latitude/longitude position, or a known feature name
+Cassini-Huygens was an [orbiter around Saturn and its moons](https://science.nasa.gov/mission/cassini/), originally launched in 1997. Cassini ran successfully for years before it was purposefully burned up in Saturn's upper atmosphere to avoid potential contamination of Saturn's moons . As the orbiter passed over Titan in dozens of flybys gigabits of data were recorded and sent back
+
+All Cassini data for Titan is organized and retrieved based on [flyby observation numbers or ID numbers](https://solarsystem.nasa.gov/missions/cassini/mission/tour/flybys/?page=0&per_page=40&order=publish_date+desc%2Ccreated_at+desc&search=&tags=cassini%3Aflybys). Pydar makes it easy to find and view relevant flybys based on a time range, latitude/longitude position, or a feature name
 
 ```python
 import pydar
 feature_name_example = "ontario lacus"
 flyby_ids = pydar.retrieveIDSByFeatureName(feature_name=feature_name_example)
 ```
 Returns a dictionary of flyby IDs (and their relevant segments) that Ontario Lacus could be found from: `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
@@ -283,15 +288,15 @@
 
 **feature_name_details.csv**
 
 Contains all named features on Titan with their furthest latitude/longitude position and origin of name
 
 Collected from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
 
-Headers: ["Feature Name", "Northernmost Latitude", "Southernmost Latitude", "Easternmost Longitude", "Westernmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
+Headers: ["Feature Name", "Northmost Latitude", "Southmost Latitude", "Eastmost Longitude", "Westmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
 
 View data file: [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
 
 ### Static Data Files
 
 **cassini_flyby.csv**
 
@@ -344,15 +349,15 @@
 ```
 * **[REQUIRED]** feature_name (string): Feature name on Titan, not case-sensitive
 
 Feature names are retrieved from [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
 <details closed>
 <summary>List of Valid Feature Names (Click to view all)</summary>
 <br>
-['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
+['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihi', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
 </details>
 
 ```python
 import pydar
 pydar.retrieveIDSByFeatureName(feature_name="Ontario Lacus")
 ```
 Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
@@ -723,15 +728,15 @@
 ```
 
 ## Credits
 Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
 
 Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
 
-This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not neccessarily reflect the views of the National Science Foundation.
+This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
 ## Acknowledging Software 
 Please acknowledge the use of this software in any publications by citing:
 
 ```
 Cassini RADAR data extraction software was provided by C. Y. Schneck and U. G. Schneck and is available at URL: https://github.com/unaschneck/pydar
 ```
```

### Comparing `pydar-1.3.0/README.md` & `pydar-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # PYDAR
  <p align="center">
   <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
 </p>
 
 ![PyPi](https://img.shields.io/pypi/v/pydar)
 ![license](https://img.shields.io/pypi/l/pydar)
+[![repo-status](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
 ![PyPi-Versions](https://img.shields.io/pypi/pyversions/pydar)
 [![update-dynamic-csv-data-files](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml)
 [![pytests](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml)
 
 A Python package to access, download, view, and manipulate Cassini RADAR images in one place
 
@@ -39,15 +40,17 @@
 
 ```
 pip install pydar
 ```
 
 ## Quickstart: PYDAR
 
-All Cassini data for Titan is retrieved based on flyby observation numbers or IDs, so relevant flybys can be found based on time range, latitude/longitude position, or a known feature name
+Cassini-Huygens was an [orbiter around Saturn and its moons](https://science.nasa.gov/mission/cassini/), originally launched in 1997. Cassini ran successfully for years before it was purposefully burned up in Saturn's upper atmosphere to avoid potential contamination of Saturn's moons . As the orbiter passed over Titan in dozens of flybys gigabits of data were recorded and sent back
+
+All Cassini data for Titan is organized and retrieved based on [flyby observation numbers or ID numbers](https://solarsystem.nasa.gov/missions/cassini/mission/tour/flybys/?page=0&per_page=40&order=publish_date+desc%2Ccreated_at+desc&search=&tags=cassini%3Aflybys). Pydar makes it easy to find and view relevant flybys based on a time range, latitude/longitude position, or a feature name
 
 ```python
 import pydar
 feature_name_example = "ontario lacus"
 flyby_ids = pydar.retrieveIDSByFeatureName(feature_name=feature_name_example)
 ```
 Returns a dictionary of flyby IDs (and their relevant segments) that Ontario Lacus could be found from: `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
@@ -247,15 +250,15 @@
 
 **feature_name_details.csv**
 
 Contains all named features on Titan with their furthest latitude/longitude position and origin of name
 
 Collected from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
 
-Headers: ["Feature Name", "Northernmost Latitude", "Southernmost Latitude", "Easternmost Longitude", "Westernmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
+Headers: ["Feature Name", "Northmost Latitude", "Southmost Latitude", "Eastmost Longitude", "Westmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
 
 View data file: [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
 
 ### Static Data Files
 
 **cassini_flyby.csv**
 
@@ -308,15 +311,15 @@
 ```
 * **[REQUIRED]** feature_name (string): Feature name on Titan, not case-sensitive
 
 Feature names are retrieved from [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
 <details closed>
 <summary>List of Valid Feature Names (Click to view all)</summary>
 <br>
-['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
+['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihi', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
 </details>
 
 ```python
 import pydar
 pydar.retrieveIDSByFeatureName(feature_name="Ontario Lacus")
 ```
 Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
@@ -687,15 +690,15 @@
 ```
 
 ## Credits
 Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
 
 Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
 
-This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not neccessarily reflect the views of the National Science Foundation.
+This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
 ## Acknowledging Software 
 Please acknowledge the use of this software in any publications by citing:
 
 ```
 Cassini RADAR data extraction software was provided by C. Y. Schneck and U. G. Schneck and is available at URL: https://github.com/unaschneck/pydar
 ```
```

### Comparing `pydar-1.3.0/pydar/__init__.py` & `pydar-1.3.1/pydar/__init__.py`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/data/cassini_flyby.csv` & `pydar-1.3.1/pydar/data/cassini_flyby.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/data/coradr_jpl_options.csv` & `pydar-1.3.1/pydar/data/coradr_jpl_options.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/data/feature_name_details.csv` & `pydar-1.3.1/pydar/data/feature_name_details.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Feature Name,Northernmost Latitude,Southernmost Latitude,Easternmost Longitude,Westernmost Longitude,Center Latitude,Center Longitude,Origin of Name
+Feature Name,Northmost Latitude,Southmost Latitude,Eastmost Longitude,Westmost Longitude,Center Latitude,Center Longitude,Origin of Name
 Aaru,10.00,10.00,340.00,340.00,10.00,340.00,Egyptian abode of the blessed dead.
 Abaya Lacus,73.70,72.75,43.39,48.00,73.17,45.55,Lake in Ethiopia.
 Adiri,-10.00,-10.00,210.00,210.00,-10.00,210.00,Melanesian afterworld where life is easier than on Earth.
 Afekan,25.80,25.80,200.30,200.30,25.80,200.30,New Guinea goddess of creation and knowledge who teaches people how to live correctly.
 Akmena Lacus,85.40,84.70,53.00,58.80,85.10,55.60,Lake in Lithuania.
 Albano Lacus,66.00,65.90,236.20,236.50,65.90,236.40,Lake in Italy.
 Anbus Labyrinthus,40.40,38.00,213.30,216.60,39.20,215.00,"Planet from the Dune series; IV Anbus, home of Tibana, an apologist for Socratic Christianity."
@@ -104,14 +104,15 @@
 Hlawga Lacus,76.90,76.30,102.20,105.10,76.60,103.60,Lake in Myanmar.
 Hobal Virga,-33.00,-38.00,150.00,183.00,-35.00,166.00,Arabian rain god.
 Hotei Arcus,-23.00,-29.00,72.00,86.00,-28.00,79.00,"One of the seven gods of happiness in Japanese Buddhism. He is the god of contentment, good fortune, cheerfulness, and he is always smiling."
 Hotei Regio,-26.00,-26.00,78.00,78.00,-26.00,78.00,"One of the seven gods of happiness in Japanese Buddhism. He is the god of contentment, good fortune, and cheerfulness, and he is always smiling."
 Hubur Flumen,-69.79,-70.94,191.58,194.38,-70.24,192.85,The river that flows at the gates of the netherworld in Mesopotamian mythology.
 Hufaidh Insulae,67.80,65.90,316.80,324.00,67.00,320.30,Legendary island in the marshes of southern Iraq.
 Huygens Landing Site,-10.576,-10.576,167.547,167.547,-10.576,167.547,where the Huygens probe landed east Adiri
+Ihi,-7.40,-8.29,164.75,165.46,-7.82,165.12,"Tahitian goddess of wisdom, worshipped by the learned."
 Ihotry Lacus,76.50,75.70,136.20,138.20,76.10,137.20,Lake in Madagascar.
 Imogene Lacus,71.50,70.70,110.80,112.70,71.10,111.80,"Lake in Idaho, USA."
 Ipyr Labyrinthus,86.65,85.83,280.42,300.50,86.24,289.00,Planet from the Dune series; home of House Thorvald.
 Irensaga Montes,-5.00,-6.65,210.54,214.73,-5.68,212.71,
 Jerid Lacuna,67.20,66.10,220.20,221.70,66.70,221.00,Intermittent lake (shott) in Tunisia.
 Jingpo Lacus,76.00,71.00,333.00,346.00,73.00,336.00,Lake in China.
 Junction Labyrinthus,-42.50,-52.90,209.10,221.40,-47.70,215.30,"Planet from the Dune series; once controlled by the Spacing Guild, taken over by the Honored Matres as a stronghold for their leader."
```

### Comparing `pydar-1.3.0/pydar/data/sar_swath_details.csv` & `pydar-1.3.1/pydar/data/sar_swath_details.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/data/swath_coverage_by_time_position.csv` & `pydar-1.3.1/pydar/data/swath_coverage_by_time_position.csv`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/display_image.py` & `pydar-1.3.1/pydar/display_image.py`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/error_handling.py` & `pydar-1.3.1/pydar/error_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
 		if second < 0 or second > 59:
 			raise ValueError("[second]: second must be within range between 0 to 59")
 
 	if millisecond is not None:
 		if type(millisecond) != int:
 			raise ValueError(f"[millisecond]: Must be an int, current type = '{type(millisecond)}'")
 		if millisecond < 0 or millisecond > 999:
-			raise ValueError("[millisecond]: second must be a postive value from 0 to 999")
+			raise ValueError("[millisecond]: second must be a positive value from 0 to 999")
 
 def errorHandlingRetrieveIDSByTimeRange(start_year=None, 
 										start_doy=None,
 										start_hour=None, 
 										start_minute=None, 
 										start_second=None, 
 										start_millisecond=None,
```

### Comparing `pydar-1.3.0/pydar/extract_flyby_parameters.py` & `pydar-1.3.1/pydar/extract_flyby_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 		if txt.startswith('BI'):
 			filename = (txt.split('/')[0]).split(".")[0]
 			if 'LBL' in (txt.split('/')[0]).split(".")[1]:
 				filename += '.LBL'
 			if 'ZIP' in (txt.split('/')[0]).split(".")[1]:
 				filename += '.ZIP'
 			all_bidr_files.append(filename)
-			if segment_id in filename: # only save certain segements
+			if segment_id in filename: # only save certain segments
 				for resolution in resolution_px: # only save top x resolutions
 					bi_types = ["B", "E", "T", "N", "M", "L"] # BI<OPTION>Q<RESOLUTION>
 					for bi in bi_types:
 						if f"BI{bi}Q{resolution}" in filename:
 							url_filenames.append(filename)
 
 	logger.info(f"All BIDR files found with specified resolution, segment, and flyby identification: {url_filenames}\n")
```

### Comparing `pydar-1.3.0/pydar/pytests/test_display_image.py` & `pydar-1.3.1/pydar/pytests/test_error_display_image.py`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/pytests/test_extract_flyby_parameters.py` & `pydar-1.3.1/pydar/pytests/test_error_extract_flyby_parameters.py`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/pytests/test_read_readme.py` & `pydar-1.3.1/pydar/pytests/test_error_read_readme.py`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/pytests/test_retrieve_ids_by_time_position.py` & `pydar-1.3.1/pydar/pytests/test_error_retrieve_ids_by_time_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
 def test_retrieveIDSByFeatureName_featureNameInvalidTypes(invalid_input, error_output):
 	with pytest.raises(ValueError, match=re.escape(f"[feature_name]: Must be a str, current type = '{error_output}'")):
 		pydar.retrieveIDSByFeatureName(feature_name=invalid_input)
 
 def test_retrieveIDSByFeatureName_featureNameNotValid():
-	with pytest.raises(ValueError, match=re.escape("Feature Name 'Invalid/Unknown Feature Name' not in available in features list = ['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']")):
+	with pytest.raises(ValueError, match=re.escape("Feature Name 'Invalid/Unknown Feature Name' not in available in features list = ['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihi', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']")):
 		pydar.retrieveIDSByFeatureName(feature_name="Invalid/Unknown Feature Name")
 
 ## retrieveIDSByFeatureName() ##########################################
 
 ## retrieveIDSByLatitudeLongitude() ####################################
 def test_retrieveIDSByLatitudeLongitude_latitudeRequired():
 	with pytest.raises(ValueError, match=re.escape("[latitude]: latitude is required")):
@@ -282,15 +282,15 @@
 @pytest.mark.parametrize("second_invalid_range", [(-1), (60)])
 def test_retrieveIDSByTime_secondInvalidRange(second_invalid_range):
 	with pytest.raises(ValueError, match=re.escape("[second]: second must be within range between 0 to 59")):
 		pydar.retrieveIDSByTime(year=2005, doy=301, hour=3, minute=15, second=second_invalid_range)
 
 @pytest.mark.parametrize("millisecond_invalid_range", [(-1), (1000)])
 def test_retrieveIDSByTime_milliscondInvalidRange(millisecond_invalid_range):
-	with pytest.raises(ValueError, match=re.escape("[millisecond]: second must be a postive value from 0 to 999")):
+	with pytest.raises(ValueError, match=re.escape("[millisecond]: second must be a positive value from 0 to 999")):
 		pydar.retrieveIDSByTime(year=2005, doy=301, hour=3, minute=15, second=20, millisecond=millisecond_invalid_range)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_int_options)
 def test_retrieveIDSByTime_yearInvalidTypes(invalid_input, error_output):
 	with pytest.raises(ValueError, match=re.escape(f"[year]: Must be an int, current type = '{error_output}'")):
 		pydar.retrieveIDSByTime(year=invalid_input, doy=301)
```

### Comparing `pydar-1.3.0/pydar/read_readme.py` & `pydar-1.3.1/pydar/read_readme.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 	# Print AAREADME to console
 	pydar.errorHandlingREADME(coradr_results_directory=coradr_results_directory,
 							section_to_print=section_to_print,
 							print_to_console=print_to_console)
 
 	sectionList = determineSectionToPrint(section_to_print, "AAREADME")
 	if sectionList is None:
-		section_to_print = section_to_print.upper() # check if the section is case-senstive
+		section_to_print = section_to_print.upper() # check if the section is case-sensitive
 		sectionList = determineSectionToPrint(section_to_print, "AAREADME")
 		if sectionList is None:
-			section_to_print = section_to_print.title() # check if the section is case-senstive
+			section_to_print = section_to_print.title() # check if the section is case-sensitive
 			sectionList = determineSectionToPrint(section_to_print, "AAREADME")
 			if sectionList is None:
 				raise ValueError(f"[readAAREADME]: Cannot find a revelant section_to_print: Invalid '{section_to_print}'")
 
 	# Define position to start console print, default to 'All' if no section is specified
 	if section_to_print is None:
 		start_index = 0
@@ -213,25 +213,25 @@
 	logger.info(f"Section Header Options: {lblreadme_section_options}")
 
 def readLBLREADME(coradr_results_directory=None, section_to_print=None, print_to_console=True):
 	# Print .LBL to console
 	if section_to_print == "FILE_NAME" or section_to_print == "RECORD_TYPE":
 		# Same text used to reference both FILE_NAME and RECORD_TYPE, user needs to specify if UNCOMPRESSED or COMPRESSED file
 		raise ValueError(f"Specify {section_to_print} as either '{section_to_print} UNCOMPRESSED' or '{section_to_print} COMPRESSED'")
-	# Catch common mispelling: not including the ^ at the front of a line name
+	# Catch common misspelling: not including the ^ at the front of a line name
 	if section_to_print == "DESCRIPTION" or section_to_print == "IMAGE" or section_to_print == "DATA_SET_MAP_PROJECTION":
 		section_to_print = f"^{section_to_print}" # sets the user's option to include the easy to miss ^
 
 	pydar.errorHandlingREADME(coradr_results_directory=coradr_results_directory,
 							section_to_print=section_to_print,
 							print_to_console=print_to_console)
 
 	sectionList = determineSectionToPrint(section_to_print, "LBL")
 	if sectionList is None:
-		# check if the section is case-senstive
+		# check if the section is case-sensitive
 		section_to_print = section_to_print.upper()
 		sectionList = determineSectionToPrint(section_to_print, "LBL")
 		if sectionList is None:
 			raise ValueError(f"[readLBLREADME]: Cannot find a revelant section_to_print: Invalid '{section_to_print}'")
 
 	# Define position to start console print, default to 'All' if no section is specified
 	if section_to_print is None:
```

### Comparing `pydar-1.3.0/pydar/retrieve_ids_by_time_position.py` & `pydar-1.3.1/pydar/retrieve_ids_by_time_position.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 	#	Returns a Dictionary of Feature Name with feature details
 	feature_name_dict = {}
 
 	flyby_csv_file = os.path.join(os.path.dirname(__file__), 'data', 'feature_name_details.csv')  # get file's directory, up one level, /data/*.csv
 	flyby_dataframe = pd.read_csv(flyby_csv_file)
 
 	for index, row in flyby_dataframe.iterrows():
-			feature_name_dict[row["Feature Name"]] = {"Southernmost Latitude": row["Southernmost Latitude"],
-													"Northernmost Latitude": row["Northernmost Latitude"], 
-													"Easternmost Longitude": row["Easternmost Longitude"], 
-													"Westernmost Longitude": row["Westernmost Longitude"],
+			feature_name_dict[row["Feature Name"]] = {"Southmost Latitude": row["Southmost Latitude"],
+													"Northmost Latitude": row["Northmost Latitude"], 
+													"Eastmost Longitude": row["Eastmost Longitude"], 
+													"Westmost Longitude": row["Westmost Longitude"],
 													"Center Latitude": row["Center Latitude"],
 													"Center Longitude": row["Center Longitude"]}
 
 	return feature_name_dict
 
 ### RETURN FLYBY IDS FOR A GIVEN FEATURE NAME ##########################
 def retrieveIDSByFeatureName(feature_name=None):
@@ -46,18 +46,18 @@
 	feature_name_csv_dict = latitudeLongitudeWithFeatureNameFromCSV()
 	feature_name = feature_name.title() # convert 'ligeria mare' to 'Ligeria Mare' to make input not sensitive to case
 
 	if feature_name not in feature_name_csv_dict.keys():
 		raise ValueError(f"Feature Name '{feature_name}' not in available in features list = {list(feature_name_csv_dict.keys())}")
 
 	feature_dict = feature_name_csv_dict[feature_name]
-	min_feature_latitude = min([feature_dict["Northernmost Latitude"], feature_dict["Southernmost Latitude"]])
-	max_feature_latitude = max([feature_dict["Northernmost Latitude"], feature_dict["Southernmost Latitude"]])
-	min_feature_longtidue = min([feature_dict["Easternmost Longitude"], feature_dict["Westernmost Longitude"]])
-	max_feature_longtidue = max([feature_dict["Easternmost Longitude"], feature_dict["Westernmost Longitude"]])
+	min_feature_latitude = min([feature_dict["Northmost Latitude"], feature_dict["Southmost Latitude"]])
+	max_feature_latitude = max([feature_dict["Northmost Latitude"], feature_dict["Southmost Latitude"]])
+	min_feature_longtidue = min([feature_dict["Eastmost Longitude"], feature_dict["Westmost Longitude"]])
+	max_feature_longtidue = max([feature_dict["Eastmost Longitude"], feature_dict["Westmost Longitude"]])
 	flyby_ids = retrieveIDSByLatitudeLongitudeRange(min_latitude=min_feature_latitude,
 													max_latitude=max_feature_latitude,
 													min_longitude=min_feature_longtidue,
 													max_longitude=max_feature_longtidue)
 	return flyby_ids
 
 ### RETURN FLYBY IDS FOR A SPECIFIC LATITUDE/LONGITUDE###################
@@ -267,19 +267,19 @@
 		range1 = (min_feature <= max_user and min_feature >= min_user)
 		range2 = (max_feature >= min_user and max_feature <= max_user)
 		range3 = (min_feature <= min_user and max_feature >= max_user)
 		intersectionFound = (range1 or range2 or range3)
 		return intersectionFound
 
 	for feature_name, position_dict in feature_name_csv_dict.items():
-		min_feature_latitude = min([float(position_dict["Northernmost Latitude"]), float(position_dict["Southernmost Latitude"])])
-		max_feature_latitude = max([float(position_dict["Northernmost Latitude"]), float(position_dict["Southernmost Latitude"])])
+		min_feature_latitude = min([float(position_dict["Northmost Latitude"]), float(position_dict["Southmost Latitude"])])
+		max_feature_latitude = max([float(position_dict["Northmost Latitude"]), float(position_dict["Southmost Latitude"])])
 		if twoRangesIntersect(min_feature_latitude, max_feature_latitude, min_latitude, max_latitude):
-			min_feature_longitude = min([float(position_dict["Westernmost Longitude"]), float(position_dict["Easternmost Longitude"])])
-			max_feature_longitude = max([float(position_dict["Westernmost Longitude"]), float(position_dict["Easternmost Longitude"])])
+			min_feature_longitude = min([float(position_dict["Westmost Longitude"]), float(position_dict["Eastmost Longitude"])])
+			max_feature_longitude = max([float(position_dict["Westmost Longitude"]), float(position_dict["Eastmost Longitude"])])
 			if twoRangesIntersect(min_feature_longitude, max_feature_longitude, min_longitude, max_longitude):
 				feature_names_list.append(feature_name)
 
 	if len(feature_names_list) == 0:
 		logger.info(f"\n[WARNING]: No Features found at latitude from {min_latitude} to {max_latitude} and longitude from {min_longitude} to {max_longitude}\n")
 
 	return feature_names_list
```

### Comparing `pydar-1.3.0/pydar/retrieve_supplementary_backplanes.py` & `pydar-1.3.1/pydar/retrieve_supplementary_backplanes.py`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/sbdr_make_shapefile.py` & `pydar-1.3.1/pydar/sbdr_make_shapefile.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 				ind = ind[~ind.SAR_AZIMUTH_RES.isin([0])]
 			else:
 				# TODO: note: usepassive and not use the same functionality
 				ind = info[~info.PASS_ELLIPSE_PT1_LAT.isin([0])]
 				ind = ind[~ind.SAR_RANGE_RES.isin([0])]
 				ind = ind[~ind.SAR_AZIMUTH_RES.isin([0])]
 
-		if len(ind.index) == 0: # No data  satifies all conditions
+		if len(ind.index) == 0: # No data satisfies all conditions
 			ind = info[~info.ACT_AZIMUTH_ANGLE.isin([0])]
 			ind = ind[~ind.ACT_ELLIPSE_PT1_LAT.isin([0])]
 			logger.info("ERROR: No Active SAR Model")
 			struct = []
 			return
 		else:
 			logger.info("Found {0} Active Pulses".format(len(ind.index)))
```

### Comparing `pydar-1.3.0/pydar/test_bearing_correction.py` & `pydar-1.3.1/pydar/test_bearing_correction.py`

 * *Files identical despite different names*

### Comparing `pydar-1.3.0/pydar/updateCsvCORADARJPLOptions.py` & `pydar-1.3.1/pydar/updateCsvCORADARJPLOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 		for txt in table_text:
 			for i, data_type in enumerate(pydar.datafile_types_columns):
 				if data_type in txt:
 					coradr_id[i+2] = True
 				if coradr_id[0].split("_")[1] in flyby_radar_take_num:
 					coradr_id[1] = True # Is a Titan Flyby
 
-	# Wrte to CSV
+	# Write to CSV
 	header_options = ["CORADR ID",
 					"Is a Titan Flyby",
 					"Contains ABDR",
 					"Contains ASUM",
 					"Contains BIDR",
 					"Contains LBDR",
 					"Contains SBDR",
```

### Comparing `pydar-1.3.0/pydar/updateCsvFeatureNameDetails.py` & `pydar-1.3.1/pydar/updateCsvFeatureNameDetails.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,56 +57,56 @@
 
 	feature_options = []
 	base_url = "https://planetarynames.wr.usgs.gov"
 	for i, feature_ahref in enumerate(ahref_lst):
 		feature_html = request.urlopen(base_url + feature_ahref)
 		logger.info(f"[{i+1}/{len(ahref_lst)}] Retrieving: {base_url + feature_ahref}")
 		soup = BeautifulSoup(feature_html, 'html.parser')
-		table = soup.find("div", {"id":"layout_content_wrapper"})
-		tr = table.find_all("tr")
+		tables = soup.find_all('table', class_='usa-table')
 		feature_object = [None, None, None, None, None, None, None, None]
-		for i in tr:
-			feature_row = ((i.text).lstrip()).split("\n")
-			feature_row = [f.strip() for f in feature_row if f != '' and re.search('[a-zA-Z-?\d+]', f)]
-			if len(feature_row) == 2:
-				if feature_row[0] == "Feature Name":
-					feature_object[0] = feature_row[1]
-				if feature_row[0] == "Northernmost Latitude":
-					feature_object[1] = feature_row[1].split(" ")[0]
-				if feature_row[0] == "Southernmost Latitude":
-					feature_object[2] = feature_row[1].split(" ")[0]
-				if feature_row[0] == "Easternmost Longitude":
-					feature_object[3] = feature_row[1].split(" ")[0]
-				if feature_row[0] == "Westernmost Longitude":
-					feature_object[4] = feature_row[1].split(" ")[0]
-				if feature_row[0] == "Center Latitude":
-					feature_object[5] = feature_row[1].split(" ")[0]
-				if feature_row[0] == "Center Longitude":
-					feature_object[6] = feature_row[1].split(" ")[0]
-				if feature_row[0] == "Origin":
-					feature_object[7] = feature_row[1]
+		for table in tables:
+			for row in table.tbody.find_all("tr"):
+				feature_row = ((row.text).lstrip()).split("\n")
+				feature_row = [f.strip() for f in feature_row if f != '' and re.search(r'[a-zA-Z-?\d+]', f)]
+				if len(feature_row) == 2:
+					if feature_row[0] == "Feature Name":
+						feature_object[0] = feature_row[1]
+					if feature_row[0] == "Northmost Latitude":
+						feature_object[1] = feature_row[1].split(" ")[0]
+					if feature_row[0] == "Southmost Latitude":
+						feature_object[2] = feature_row[1].split(" ")[0]
+					if feature_row[0] == "Eastmost Longitude":
+						feature_object[3] = feature_row[1].split(" ")[0]
+					if feature_row[0] == "Westmost Longitude":
+						feature_object[4] = feature_row[1].split(" ")[0]
+					if feature_row[0] == "Center Latitude":
+						feature_object[5] = feature_row[1].split(" ")[0]
+					if feature_row[0] == "Center Longitude":
+						feature_object[6] = feature_row[1].split(" ")[0]
+					if feature_row[0] == "Origin":
+						feature_object[7] = feature_row[1]
 		feature_options.append(feature_object)
 
 	# Add Huygens landing site manually
 	huygens_landing_site = ["Huygens Landing Site", 
 							"-10.576",
 							"-10.576",
 							"167.547",
 							"167.547",
 							"-10.576",
 							"167.547",
 							"where the Huygens probe landed east Adiri"]
 	feature_options.append(huygens_landing_site)
 
-	# Wrte to CSV
+	# Write to CSV
 	header_options = ["Feature Name", 
-					"Northernmost Latitude",
-					"Southernmost Latitude",
-					"Easternmost Longitude",
-					"Westernmost Longitude",
+					"Northmost Latitude",
+					"Southmost Latitude",
+					"Eastmost Longitude",
+					"Westmost Longitude",
 					"Center Latitude",
 					"Center Longitude", 
 					"Origin of Name"]
 	df = pd.DataFrame(feature_options, columns=header_options)
 	df = df.sort_values(by=["Feature Name"])
 	df.to_csv(os.path.join(os.path.dirname(__file__), 'data', 'feature_name_details.csv'), header=header_options, index=False)
```

### Comparing `pydar-1.3.0/pydar/updateCsvSwathCoverage.py` & `pydar-1.3.1/pydar/updateCsvSwathCoverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 									lbl[11] = west_long
 								if "START_TIME" in line:
 									lbl[12] = line.split("=")[1].strip()
 								if "STOP_TIME" in line:
 									lbl[13] = line.split("=")[1].strip()
 							lbl_information.append(lbl)
 
-	# Wrte to CSV
+	# Write to CSV
 	header_options = ["CORADR ID",
 					"FLYBY ID",
 					"SEGMENT NUMBER",
 					"FILENAME",
 					"DATE TYPE SYMBOL",
 					"DATE TYPE",
 					"RESOLUTION (pixels/degrees)",
```

### Comparing `pydar-1.3.0/pydar.egg-info/PKG-INFO` & `pydar-1.3.1/pydar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: pydar
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Python package to access, download, view, and manipulate Cassini RADAR images
 Home-page: https://github.com/unaschneck/pydar
-Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.3.0.tar.gz
+Download-URL: https://github.com/unaschneck/pydar/archive/refs/tags/v1.3.1.tar.gz
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
+Keywords: geophysics,python,astronomy,nasa,radar,planetary-science,cassini,jpl
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: beautifulsoup4>=4.11.1
-Requires-Dist: matplotlib>=3.1.0
-Requires-Dist: pandas>=1.5.2
-Requires-Dist: pdr>=0.7.3
-Requires-Dist: pyproj>=3.4.1
-Requires-Dist: pytest>=7.2.2
-Requires-Dist: rasterio>=1.3.6
-Requires-Dist: urllib3>=1.26.18
+Requires-Dist: beautifulsoup4
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: pdr
+Requires-Dist: pyproj
+Requires-Dist: pytest
+Requires-Dist: rasterio
+Requires-Dist: urllib3
 
 # PYDAR
  <p align="center">
   <img src="https://raw.githubusercontent.com/unaschneck/pydar/main/assets/pydar_logo.jpg" />
 </p>
 
 ![PyPi](https://img.shields.io/pypi/v/pydar)
 ![license](https://img.shields.io/pypi/l/pydar)
+[![repo-status](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![NSF-2141064](https://img.shields.io/badge/NSF-2141064-blue)](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2141064&HistoricalAwards=false)
 ![PyPi-Versions](https://img.shields.io/pypi/pyversions/pydar)
 [![update-dynamic-csv-data-files](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/web_scrap_dynamic_csv_files.yml)
 [![pytests](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml/badge.svg)](https://github.com/unaschneck/pydar/actions/workflows/pytests.yml)
 
 A Python package to access, download, view, and manipulate Cassini RADAR images in one place
 
@@ -75,15 +78,17 @@
 
 ```
 pip install pydar
 ```
 
 ## Quickstart: PYDAR
 
-All Cassini data for Titan is retrieved based on flyby observation numbers or IDs, so relevant flybys can be found based on time range, latitude/longitude position, or a known feature name
+Cassini-Huygens was an [orbiter around Saturn and its moons](https://science.nasa.gov/mission/cassini/), originally launched in 1997. Cassini ran successfully for years before it was purposefully burned up in Saturn's upper atmosphere to avoid potential contamination of Saturn's moons . As the orbiter passed over Titan in dozens of flybys gigabits of data were recorded and sent back
+
+All Cassini data for Titan is organized and retrieved based on [flyby observation numbers or ID numbers](https://solarsystem.nasa.gov/missions/cassini/mission/tour/flybys/?page=0&per_page=40&order=publish_date+desc%2Ccreated_at+desc&search=&tags=cassini%3Aflybys). Pydar makes it easy to find and view relevant flybys based on a time range, latitude/longitude position, or a feature name
 
 ```python
 import pydar
 feature_name_example = "ontario lacus"
 flyby_ids = pydar.retrieveIDSByFeatureName(feature_name=feature_name_example)
 ```
 Returns a dictionary of flyby IDs (and their relevant segments) that Ontario Lacus could be found from: `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
@@ -283,15 +288,15 @@
 
 **feature_name_details.csv**
 
 Contains all named features on Titan with their furthest latitude/longitude position and origin of name
 
 Collected from the [planetarynames.wr.usgs.gov](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
 
-Headers: ["Feature Name", "Northernmost Latitude", "Southernmost Latitude", "Easternmost Longitude", "Westernmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
+Headers: ["Feature Name", "Northmost Latitude", "Southmost Latitude", "Eastmost Longitude", "Westmost Longitude", "Center Latitude", "Center Longitude", "Origin of Name"]
 
 View data file: [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
 
 ### Static Data Files
 
 **cassini_flyby.csv**
 
@@ -344,15 +349,15 @@
 ```
 * **[REQUIRED]** feature_name (string): Feature name on Titan, not case-sensitive
 
 Feature names are retrieved from [feature_name_details.csv](https://github.com/unaschneck/pydar/blob/main/pydar/data/feature_name_details.csv)
 <details closed>
 <summary>List of Valid Feature Names (Click to view all)</summary>
 <br>
-['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
+['Aaru', 'Abaya Lacus', 'Adiri', 'Afekan', 'Akmena Lacus', 'Albano Lacus', 'Anbus Labyrinthus', 'Angmar Montes', 'Annecy Lacus', 'Antilia Faculae', 'Apanohuaya Flumen', 'Ara Fluctus', 'Arala Lacus', 'Arnar Sinus', 'Arrakis Planitia', 'Arwen Colles', 'Atacama Lacuna', 'Atitlán Lacus', 'Aura Undae', 'Avacha Sinus', 'Aztlan', 'Bacab Virgae', 'Baffin Sinus', 'Balaton Lacus', 'Bayta Fretum', 'Bazaruto Facula', 'Beag', 'Belet', 'Bermoothes Insula', 'Bilbo Colles', 'Bimini Insula', 'Bolsena Lacus', 'Boni Sinus', 'Boreas Undae', 'Bralgu Insulae', 'Brienz Lacus', 'Buada Lacus', 'Buyan Insula', 'Buzzell Planitia', 'Caladan Planitia', 'Cardiel Lacus', 'Cayuga Lacus', 'Celadon Flumina', 'Cerknica Lacuna', 'Chilwa Lacus', 'Ching-tu', 'Chusuk Planitia', 'Coats Facula', 'Concordia Regio', 'Corrin Labyrinthus', 'Crete Facula', 'Crveno Lacus', 'Dilmun', 'Dilolo Lacus', 'Dingle Sinus', 'Dolmed Montes', 'Doom Mons', 'Dridzis Lacus', 'Ecaz Labyrinthus', 'Echoriath Montes', 'Eir Macula', 'Elba Facula', 'Elivagar Flumina', 'Elpis Macula', 'Enriquillo Lacus', 'Erebor Mons', 'Eurus Undae', 'Eyre Lacuna', 'Fagaloa Sinus', 'Faramir Colles', 'Feia Lacus', 'Fensal', 'Flensborg Sinus', 'Fogo Lacus', 'Forseti', 'Freeman Lacus', 'Fundy Sinus', 'Gabes Sinus', 'Gammu Labyrinthus', 'Gamont Labyrinthus', 'Gandalf Colles', 'Ganesa Macula', 'Gansireed Labyrinthus', 'Garotman Terra', 'Gatun Lacus', 'Genetaska Macula', 'Genova Sinus', 'Giedi Planitia', 'Gihon Flumen', 'Ginaz Labyrinthus', 'Gram Montes', 'Grasmere Lacus', 'Grumman Labyrinthus', 'Guabonito', 'Hagal Planitia', 'Hammar Lacus', 'Handir Colles', 'Hano', 'Hardin Fretum', 'Harmonthep Labyrinthus', 'Hawaiki Insulae', 'Hetpet Regio', 'Hlawga Lacus', 'Hobal Virga', 'Hotei Arcus', 'Hotei Regio', 'Hubur Flumen', 'Hufaidh Insulae', 'Huygens Landing Site', 'Ihi', 'Ihotry Lacus', 'Imogene Lacus', 'Ipyr Labyrinthus', 'Irensaga Montes', 'Jerid Lacuna', 'Jingpo Lacus', 'Junction Labyrinthus', 'Junín Lacus', 'Kaitain Labyrinthus', 'Kalseru Virga', 'Karakul Lacus', 'Karesos Flumen', 'Kayangan Lacus', 'Kerguelen Facula', 'Kivu Lacus', 'Koitere Lacus', 'Kokytos Flumina', 'Kraken Mare', 'Krocylea Insulae', 'Kronin Labyrinthus', 'Ksa', 'Kumbaru Sinus', 'Kutch Lacuna', 'Ladoga Lacus', 'Lagdo Lacus', 'Lampadas Labyrinthus', 'Lanao Lacus', 'Lankiveil Labyrinthus', 'Leilah Fluctus', 'Lernaeus Labyrinthus', 'Letas Lacus', 'Ligeia Mare', 'Lithui Montes', 'Logtak Lacus', 'Luin Montes', 'Lulworth Sinus', 'Mackay Lacus', 'Maizuru Sinus', 'Manza Sinus', 'Maracaibo Lacus', 'Mayda Insula', 'Melrhir Lacuna', 'Menrva', 'Merlock Montes', 'Meropis Insula', 'Mezzoramia', 'Mindanao Facula', 'Mindolluin Montes', 'Misty Montes', 'Mithrim Montes', 'Mohini Fluctus', 'Momoy', 'Montego Sinus', 'Moray Sinus', 'Moria Montes', 'Muritan Labyrinthus', 'Muzhwi Lacus', 'Mweru Lacus', 'Mystis', 'Müggel Lacus', 'Mývatn Lacus', 'Nakuru Lacuna', 'Naraj Labyrinthus', 'Nath', 'Neagh Lacus', 'Negra Lacus', 'Ngami Lacuna', 'Nicobar Faculae', 'Nicoya Sinus', 'Nimloth Colles', 'Niushe Labyrinthus', 'Notus Undae', 'Oahu Facula', 'Ochumare Regio', 'Ohrid Lacus', 'Okahu Sinus', 'Olomega Lacus', 'Omacatl Macula', 'Oneida Lacus', 'Onogoro Insula', 'Ontario Lacus', 'Orog Lacuna', 'Palma Labyrinthus', 'Patos Sinus', 'Paxsi', 'Penglai Insula', 'Perkunas Virgae', 'Phewa Lacus', 'Pielinen Lacus', 'Planctae Insulae', 'Polaznik Macula', 'Polelya Macula', 'Poritrin Planitia', 'Prespa Lacus', 'Puget Sinus', 'Punga Mare', 'Qinghai Lacus', 'Quilotoa Lacus', 'Quivira', 'Racetrack Lacuna', 'Rannoch Lacus', 'Rerir Montes', 'Richese Labyrinthus', 'Roca Lacus', 'Rohe Fluctus', 'Rombaken Sinus', 'Romo Planitia', 'Rossak Planitia', 'Royllo Insula', 'Rukwa Lacus', 'Rwegura Lacus', 'Saldanha Sinus', 'Salusa Labyrinthus', 'Sambation Flumina', 'Santorini Facula', 'Saraswati Flumen', 'Sarygamysh Lacus', 'Seldon Fretum', 'Selk', 'Senkyo', 'Sevan Lacus', 'Shangri-La', 'Shikoku Facula', 'Shiwanni Virgae', 'Shoji Lacus', 'Sikun Labyrinthus', 'Sinlap', 'Sionascaig Lacus', 'Skelton Sinus', 'Soi', 'Sotonera Lacus', 'Sotra Patera', 'Sparrow Lacus', 'Suwa Lacus', 'Synevyr Lacus', 'Taniquetil Montes', 'Tasmania Facula', 'Taupo Lacus', 'Tengiz Lacus', 'Texel Facula', 'Tishtrya Virgae', 'Tlaloc Virgae', 'Tleilax Labyrinthus', 'Toba Lacus', 'Tollan Terra', 'Tortola Facula', 'Totak Lacus', 'Towada Lacus', 'Trevize Fretum', 'Trichonida Lacus', 'Trold Sinus', 'Tsegihi', 'Tsiipiya Terra', 'Tsomgo Lacus', 'Tui Regio', 'Tumaco Sinus', 'Tunu Sinus', 'Tupile Labyrinthus', 'Uanui Virgae', 'Urmia Lacus', 'Uvs Lacus', 'Uyuni Lacuna', 'Van Lacus', 'Veles', 'Veliko Lacuna', 'Vid Flumina', 'Viedma Lacus', 'Vis Facula', 'Vänern Lacus', 'Waikare Lacus', 'Wakasa Sinus', 'Walvis Sinus', 'Weija Lacus', 'Winia Fluctus', 'Winnipeg Lacus', 'Woytchugga Lacuna', 'Xanadu', 'Xanthus Flumen', 'Xolotlán Lacus', 'Xuttah Planitia', 'Yalaing Terra', 'Yessey Lacus', 'Yojoa Lacus', 'Ypoa Lacus', 'Zaza Lacus', 'Zephyrus Undae', 'Zub Lacus']
 </details>
 
 ```python
 import pydar
 pydar.retrieveIDSByFeatureName(feature_name="Ontario Lacus")
 ```
 Output = `{'T7': ['S01'], 'T36': ['S03'], 'T39': ['S06', 'S05', 'S01', 'S04'], 'T48': ['S04'], 'T49': ['S01'], 'T50': ['S02'], 'T55': ['S01', 'S03'], 'T56': ['S01'], 'T57': ['S01', 'S02'], 'T58': ['S01'], 'T59': ['S01'], 'T65': ['S04', 'S01', 'S05', 'S02', 'S03'], 'T71': ['S01'], 'T95': ['S03'], 'T98': ['S01', 'S04']}`
@@ -723,15 +728,15 @@
 ```
 
 ## Credits
 Feature Names collected from [Gazetteer of Planetary Nomenclature](https://planetarynames.wr.usgs.gov/SearchResults?Target=74_Titan)
 
 Instrument information and naming conventions collected from the [Cassini Radar User Guide](https://pds-imaging.jpl.nasa.gov/documentation/Cassini_RADAR_Users_Guide_2nd_Ed_191004_cmp_200421.pdf)
 
-This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not neccessarily reflect the views of the National Science Foundation.
+This material is based upon work supported by the National Science Foundation Graduate Fellowship under Grant No. 2141064. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the authors and do not necessarily reflect the views of the National Science Foundation.
 
 ## Acknowledging Software 
 Please acknowledge the use of this software in any publications by citing:
 
 ```
 Cassini RADAR data extraction software was provided by C. Y. Schneck and U. G. Schneck and is available at URL: https://github.com/unaschneck/pydar
 ```
```

### Comparing `pydar-1.3.0/pydar.egg-info/SOURCES.txt` & `pydar-1.3.1/pydar.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 pydar.egg-info/requires.txt
 pydar.egg-info/top_level.txt
 pydar/data/cassini_flyby.csv
 pydar/data/coradr_jpl_options.csv
 pydar/data/feature_name_details.csv
 pydar/data/sar_swath_details.csv
 pydar/data/swath_coverage_by_time_position.csv
-pydar/pytests/test_display_image.py
-pydar/pytests/test_extract_flyby_parameters.py
-pydar/pytests/test_read_readme.py
-pydar/pytests/test_retrieve_ids_by_time_position.py
+pydar/pytests/test_error_display_image.py
+pydar/pytests/test_error_extract_flyby_parameters.py
+pydar/pytests/test_error_read_readme.py
+pydar/pytests/test_error_retrieve_ids_by_time_position.py
```

### Comparing `pydar-1.3.0/setup.py` & `pydar-1.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.3.0"
+VERSION="1.3.1"
 DESCRIPTION="A Python package to access, download, view, and manipulate Cassini RADAR images"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="pydar",
 	version=VERSION,
 	description=DESCRIPTION,
 	long_description=long_description_readme,
 	long_description_content_type='text/markdown',
 	url="https://github.com/unaschneck/pydar",
-	download_url="https://github.com/unaschneck/pydar/archive/refs/tags/v{0}.tar.gz".format(VERSION),
+	download_url=f"https://github.com/unaschneck/pydar/archive/refs/tags/v{VERSION}.tar.gz",
 	author="Una Schneck (unaschneck), Cora Schneck (cyschneck)",
-	keywords=[],
+	keywords=["geophysics", "python", "astronomy", "nasa", "radar", "planetary-science", "cassini", "jpl"],
 	license="MIT",
 	classifiers=[
 		"Development Status :: 4 - Beta",
 		"Intended Audience :: Developers",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
 		"License :: OSI Approved :: MIT License",
 		"Programming Language :: Python",
+		"Programming Language :: Python :: 3",
 		"Programming Language :: Python :: 3.9",
 		"Programming Language :: Python :: 3.10",
 		"Programming Language :: Python :: 3.11",
 		"Programming Language :: Python :: 3.12",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
 		"Topic :: Scientific/Engineering :: Physics",
 		"Topic :: Scientific/Engineering :: Image Processing",
 		"Topic :: Scientific/Engineering :: Visualization",
 		"Topic :: Scientific/Engineering :: Astronomy"
 	],
 	packages=find_namespace_packages(include=['pydar', 'pydar.*']),
 	include_package_data=True,
 	install_requires=[
-			"beautifulsoup4>=4.11.1",
-			"matplotlib>=3.1.0",
-			"pandas>=1.5.2",
-			"pdr>=0.7.3",
-			"pyproj>=3.4.1",
-			"pytest>=7.2.2",
-			"rasterio>=1.3.6",
-			"urllib3>=1.26.18"
+			"beautifulsoup4",
+			"matplotlib",
+			"pandas",
+			"pdr",
+			"pyproj",
+			"pytest",
+			"rasterio",
+			"urllib3"
 			],
 	python_requires='>=3.9'
 )
```

