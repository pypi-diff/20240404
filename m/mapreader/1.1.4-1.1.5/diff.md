# Comparing `tmp/mapreader-1.1.4.tar.gz` & `tmp/mapreader-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapreader-1.1.4.tar", last modified: Fri Feb 23 09:57:51 2024, max compression
+gzip compressed data, was "mapreader-1.1.5.tar", last modified: Thu Apr  4 13:58:12 2024, max compression
```

## Comparing `mapreader-1.1.4.tar` & `mapreader-1.1.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.727676 mapreader-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-02-23 09:57:39.000000 mapreader-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15440 2024-02-23 09:57:51.723676 mapreader-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-02-23 09:57:39.000000 mapreader-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.727676 mapreader-1.1.4/mapreader/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-23 09:57:51.727676 mapreader-1.1.4/mapreader/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.719676 mapreader-1.1.4/mapreader/annotate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/annotate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34533 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/annotate/annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/annotate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.719676 mapreader-1.1.4/mapreader/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    75024 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/classify/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/classify/custom_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/classify/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/classify/load_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.719676 mapreader-1.1.4/mapreader/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/download/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/download/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44527 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/download/sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/download/tile_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/download/tile_merging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.723676 mapreader-1.1.4/mapreader/load/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/load/geo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    94714 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/load/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/load/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.723676 mapreader-1.1.4/mapreader/process/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/process/post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/process/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.723676 mapreader-1.1.4/mapreader/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/utils/compute_and_save_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-23 09:57:39.000000 mapreader-1.1.4/mapreader/utils/slice_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.723676 mapreader-1.1.4/mapreader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15440 2024-02-23 09:57:51.000000 mapreader-1.1.4/mapreader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-23 09:57:51.000000 mapreader-1.1.4/mapreader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 09:57:51.000000 mapreader-1.1.4/mapreader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-23 09:57:51.000000 mapreader-1.1.4/mapreader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 09:57:51.000000 mapreader-1.1.4/mapreader.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-23 09:57:51.000000 mapreader-1.1.4/mapreader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-23 09:57:51.000000 mapreader-1.1.4/mapreader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-23 09:57:51.727676 mapreader-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-02-23 09:57:39.000000 mapreader-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:57:51.723676 mapreader-1.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-02-23 09:57:40.000000 mapreader-1.1.4/tests/test_annotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-02-23 09:57:40.000000 mapreader-1.1.4/tests/test_geo_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-23 09:57:40.000000 mapreader-1.1.4/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-02-23 09:57:40.000000 mapreader-1.1.4/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    22537 2024-02-23 09:57:40.000000 mapreader-1.1.4/tests/test_sheet_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    83834 2024-02-23 09:57:40.000000 mapreader-1.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.739074 mapreader-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-04 13:58:06.000000 mapreader-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-04-04 13:58:12.739074 mapreader-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12791 2024-04-04 13:58:06.000000 mapreader-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.739074 mapreader-1.1.5/mapreader/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 13:58:12.739074 mapreader-1.1.5/mapreader/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.731074 mapreader-1.1.5/mapreader/annotate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/annotate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34533 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/annotate/annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26468 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/annotate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.731074 mapreader-1.1.5/mapreader/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75024 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/custom_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31931 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/classify/load_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46716 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/tile_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/download/tile_merging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/load/geo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98833 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/load/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/load/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader/process/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/process/post_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/process/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/utils/compute_and_save_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-04 13:58:06.000000 mapreader-1.1.5/mapreader/utils/slice_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/mapreader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15556 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 13:58:12.000000 mapreader-1.1.5/mapreader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 13:58:12.739074 mapreader-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-04-04 13:58:06.000000 mapreader-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:58:12.735074 mapreader-1.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_geo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22537 2024-04-04 13:58:06.000000 mapreader-1.1.5/tests/test_sheet_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83834 2024-04-04 13:58:06.000000 mapreader-1.1.5/versioneer.py
```

### Comparing `mapreader-1.1.4/LICENSE` & `mapreader-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/PKG-INFO` & `mapreader-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.1.4
+Version: 1.1.5
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
@@ -20,15 +20,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib<4.0.0,>=3.5.0
 Requires-Dist: numpy<2.0.0,>=1.21.5
 Requires-Dist: pandas<2.0.0,>=1.3.4
 Requires-Dist: pyproj<4.0.0,>=3.2.0
 Requires-Dist: azure-storage-blob<13.0.0,>=12.9.0
@@ -51,21 +51,24 @@
 Requires-Dist: rasterio<2.0.0,>=1.2.10
 Requires-Dist: simplekml<2.0.0,>=1.3.6
 Requires-Dist: versioneer>=0.28
 Requires-Dist: tqdm<5.0.0
 Requires-Dist: torchinfo<2.0.0
 Requires-Dist: openpyxl<4.0.0
 Requires-Dist: geopandas<1.0.0
+Requires-Dist: pyogrio>=0.7.2
 Provides-Extra: dev
 Requires-Dist: pytest<8.0.0; extra == "dev"
 Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == "dev"
 Requires-Dist: timm<1.0.0; extra == "dev"
 Requires-Dist: transformers<5.0.0; extra == "dev"
 Requires-Dist: black<24.0.0,>=23.7.0; extra == "dev"
 Requires-Dist: flake8<7.0.0,>=6.0.0; extra == "dev"
+Provides-Extra: geo
+Requires-Dist: cartopy>=0.20.0; extra == "geo"
 
 <div align="center">
     <br>
     <p align="center">
     <h1>MapReader</h1>
     <h2>A computer vision pipeline for exploring and analyzing images at scale</h2>
     </p>
@@ -128,15 +131,15 @@
 **New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for help with the initial set up of MapReader.
 
 **All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustrating use cases such as:
 
 - Geospatial images (i.e. maps)
 - Non-geospatial images
 
- **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
+ **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
 
 **Join our Slack workspace!**
 Please fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9) to receive an invitation to the Slack workspace.
 
 ## What is included in this repo?
 
 The MapReader package provides a set of tools to:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.1.4 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.1.5 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
@@ -10,34 +10,35 @@
 Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: Unix Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7, <3.11 Description-Content-Type: text/markdown License-
+Requires-Python: >=3.8, <3.11 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: matplotlib<4.0.0,>=3.5.0 Requires-Dist:
 numpy<2.0.0,>=1.21.5 Requires-Dist: pandas<2.0.0,>=1.3.4 Requires-Dist:
 pyproj<4.0.0,>=3.2.0 Requires-Dist: azure-storage-blob<13.0.0,>=12.9.0
 Requires-Dist: aiohttp<4.0.0,>=3.8.1 Requires-Dist: Shapely<3.0.0,>=2.0.0
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.1 Requires-Dist: scikit-image>=0.18.3
 Requires-Dist: scikit-learn<2.0.0,>=1.0.1 Requires-Dist: torch<2.0.0,>=1.10.0
 Requires-Dist: torchvision<0.12.1,>=0.11.1 Requires-Dist: jupyter<2.0.0,>=1.0.0
 Requires-Dist: ipykernel<7.0.0,>=6.5.1 Requires-Dist: ipywidgets<9.0.0,>=8.0.0
 Requires-Dist: ipyannotate==0.1.0-beta.0 Requires-Dist: Cython<0.30.0,>=0.29.24
 Requires-Dist: PyYAML<7.0,>=6.0 Requires-Dist: tensorboard<3.0.0,>=2.7.0
 Requires-Dist: parhugin<0.0.4,>=0.0.3 Requires-Dist: geopy==2.1.0 Requires-
 Dist: rasterio<2.0.0,>=1.2.10 Requires-Dist: simplekml<2.0.0,>=1.3.6 Requires-
 Dist: versioneer>=0.28 Requires-Dist: tqdm<5.0.0 Requires-Dist: torchinfo<2.0.0
-Requires-Dist: openpyxl<4.0.0 Requires-Dist: geopandas<1.0.0 Provides-Extra:
-dev Requires-Dist: pytest<8.0.0; extra == "dev" Requires-Dist: pytest-
-cov<5.0.0,>=4.1.0; extra == "dev" Requires-Dist: timm<1.0.0; extra == "dev"
-Requires-Dist: transformers<5.0.0; extra == "dev" Requires-Dist:
-black<24.0.0,>=23.7.0; extra == "dev" Requires-Dist: flake8<7.0.0,>=6.0.0;
-extra == "dev"
+Requires-Dist: openpyxl<4.0.0 Requires-Dist: geopandas<1.0.0 Requires-Dist:
+pyogrio>=0.7.2 Provides-Extra: dev Requires-Dist: pytest<8.0.0; extra == "dev"
+Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == "dev" Requires-Dist:
+timm<1.0.0; extra == "dev" Requires-Dist: transformers<5.0.0; extra == "dev"
+Requires-Dist: black<24.0.0,>=23.7.0; extra == "dev" Requires-Dist:
+flake8<7.0.0,>=6.0.0; extra == "dev" Provides-Extra: geo Requires-Dist:
+cartopy>=0.20.0; extra == "geo"
 
                             ************ MMaappRReeaaddeerr ************
  ********** AA ccoommppuutteerr vviissiioonn ppiippeelliinnee ffoorr eexxpplloorriinngg aanndd aannaallyyzziinngg iimmaaggeess aatt ssccaallee
                                      **********
                  _[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _b_a_d_g_e_]_[_D_O_I_]
        _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_L_i_v_i_n_g_-_w_i_t_h_-_m_a_c_h_i_n_e_s_/_M_a_p_R_e_a_d_e_r_/_g_r_a_p_h_/
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_8_G_Q_3_O_1_G_B_5_]
@@ -72,22 +73,22 @@
 users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/
 latest/User-guide/User-guide.html) for guidance on how to use MapReader. This
 contains end-to-end instructions on how to use the MapReader pipeline, plus a
 number of worked examples illustrating use cases such as: - Geospatial images
 (i.e. maps) - Non-geospatial images **Developers and contributors** may also
 want to refer to the [API documentation](https://mapreader.readthedocs.io/en/
 latest/api/index.html) and [Contribution guide](https://
-mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how
-to contribute to the MapReader package. **Join our Slack workspace!** Please
-fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9) to receive an
-invitation to the Slack workspace. ## What is included in this repo? The
-MapReader package provides a set of tools to: - **Download** images/maps and
-metadata stored on web-servers (e.g. tileservers which can be used to retrieve
-maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or
-elsewhere). - **Load** images/maps and metadata stored locally. - **Pre-
+mapreader.readthedocs.io/en/latest/Contribution-guide/Contribution-guide.html)
+for guidance on how to contribute to the MapReader package. **Join our Slack
+workspace!** Please fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9)
+to receive an invitation to the Slack workspace. ## What is included in this
+repo? The MapReader package provides a set of tools to: - **Download** images/
+maps and metadata stored on web-servers (e.g. tileservers which can be used to
+retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS),
+or elsewhere). - **Load** images/maps and metadata stored locally. - **Pre-
 process** images/maps: - patchify (create patches from a parent image), -
 resample (use image transformations to alter pixel-dimensions/resolution/
 orientation/etc.), - remove borders outside the neatline, - reproject between
 coordinate reference systems (CRS). - **Annotate** images/maps (or their
 patches) using an interactive annotation tool. - **Train or fine-tune**
 Computer Vision (CV) models and use these to **predict** labels (i.e. model
 inference) on large sets of images/maps. Various **plotting and analysis**
```

### Comparing `mapreader-1.1.4/README.md` & `mapreader-1.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 **New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for help with the initial set up of MapReader.
 
 **All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustrating use cases such as:
 
 - Geospatial images (i.e. maps)
 - Non-geospatial images
 
- **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
+ **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
 
 **Join our Slack workspace!**
 Please fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9) to receive an invitation to the Slack workspace.
 
 ## What is included in this repo?
 
 The MapReader package provides a set of tools to:
```

#### html2text {}

```diff
@@ -36,22 +36,22 @@
 users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/
 latest/User-guide/User-guide.html) for guidance on how to use MapReader. This
 contains end-to-end instructions on how to use the MapReader pipeline, plus a
 number of worked examples illustrating use cases such as: - Geospatial images
 (i.e. maps) - Non-geospatial images **Developers and contributors** may also
 want to refer to the [API documentation](https://mapreader.readthedocs.io/en/
 latest/api/index.html) and [Contribution guide](https://
-mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how
-to contribute to the MapReader package. **Join our Slack workspace!** Please
-fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9) to receive an
-invitation to the Slack workspace. ## What is included in this repo? The
-MapReader package provides a set of tools to: - **Download** images/maps and
-metadata stored on web-servers (e.g. tileservers which can be used to retrieve
-maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or
-elsewhere). - **Load** images/maps and metadata stored locally. - **Pre-
+mapreader.readthedocs.io/en/latest/Contribution-guide/Contribution-guide.html)
+for guidance on how to contribute to the MapReader package. **Join our Slack
+workspace!** Please fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9)
+to receive an invitation to the Slack workspace. ## What is included in this
+repo? The MapReader package provides a set of tools to: - **Download** images/
+maps and metadata stored on web-servers (e.g. tileservers which can be used to
+retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS),
+or elsewhere). - **Load** images/maps and metadata stored locally. - **Pre-
 process** images/maps: - patchify (create patches from a parent image), -
 resample (use image transformations to alter pixel-dimensions/resolution/
 orientation/etc.), - remove borders outside the neatline, - reproject between
 coordinate reference systems (CRS). - **Annotate** images/maps (or their
 patches) using an interactive annotation tool. - **Train or fine-tune**
 Computer Vision (CV) models and use these to **predict** labels (i.e. model
 inference) on large sets of images/maps. Various **plotting and analysis**
```

### Comparing `mapreader-1.1.4/mapreader/__init__.py` & `mapreader-1.1.5/mapreader/__init__.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/annotate/annotator.py` & `mapreader-1.1.5/mapreader/annotate/annotator.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/annotate/utils.py` & `mapreader-1.1.5/mapreader/annotate/utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/classify/classifier.py` & `mapreader-1.1.5/mapreader/classify/classifier.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/classify/custom_models.py` & `mapreader-1.1.5/mapreader/classify/custom_models.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/classify/datasets.py` & `mapreader-1.1.5/mapreader/classify/datasets.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/classify/load_annotations.py` & `mapreader-1.1.5/mapreader/classify/load_annotations.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/download/data_structures.py` & `mapreader-1.1.5/mapreader/download/data_structures.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/download/downloader.py` & `mapreader-1.1.5/mapreader/download/downloader.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,80 +57,91 @@
         Parameters
         ----------
         path_save : str
             Path to save merged items (i.e. whole map sheets)
         """
         self.merger = TileMerger(output_folder=path_save, show_progress=False)
 
-    def _check_map_exists(self, grid_bb: GridBoundingBox) -> bool:
+    def _check_map_exists(self, grid_bb: GridBoundingBox, map_name: str | None) -> bool:
         """
         Checks if a map is already saved.
 
         Parameters
         ----------
         grid_bb : GridBoundingBox
+            The grid bounding box of the map
+        map_name : str, optional
+            Name to use when saving the map, by default None
 
         Returns
         -------
         bool
             True if file exists, False if not.
         """
-        map_name = self.merger._get_output_name(grid_bb)
+        if map_name is None:
+            map_name = self.merger._get_output_name(grid_bb)
         path_save = self.merger.output_folder
         if os.path.exists(f"{path_save}{map_name}.png"):
             print(
                 f'[INFO] "{path_save}{map_name}.png" already exists. Skipping download.'
             )
             return True
         return False
 
-    def _download_map(self, grid_bb: GridBoundingBox) -> bool:
+    def _download_map(self, grid_bb: GridBoundingBox, map_name: str | None) -> bool:
         """
         Downloads a map contained within a grid bounding box.
 
         Parameters
         ----------
         grid_bb : GridBoundingBox
+            The grid bounding box of the map
+        map_name : str, optional
+            Name to use when saving the map, by default None
 
         Returns
         -------
         bool
             True if map was successfully downloaded, False if not.
         """
-        map_name = self.merger._get_output_name(grid_bb)
+        if map_name is None:
+            map_name = self.merger._get_output_name(grid_bb)
         self.downloader.download_tiles(grid_bb, download_in_parallel=False)
-        success = self.merger.merge(grid_bb)
+        success = self.merger.merge(grid_bb, map_name)
         if success:
             print(f'[INFO] Downloaded "{map_name}.png"')
         else:
             print(f'[WARNING] Download of "{map_name}.png" was unsuccessful.')
 
         shutil.rmtree(DEFAULT_TEMP_FOLDER)
         return success
 
     def download_map_by_polygon(
         self,
         polygon: Polygon,
         zoom_level: int | None = 14,
         path_save: str | None = "maps",
         overwrite: bool | None = False,
+        map_name: str | None = None,
     ) -> None:
         """
         Downloads a map contained within a polygon.
 
         Parameters
         ----------
         polygon : Polygon
             A polygon defining the boundaries of the map
         zoom_level : int, optional
             The zoom level to use, by default 14
         path_save : str, optional
             Path to save map sheets, by default "maps"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
+        map_name : str, optional
+            Name to use when saving the map, by default None
         """
 
         assert isinstance(
             polygon, Polygon
         ), "[ERROR] \
 Please pass polygon as shapely.geometry.Polygon object.\n\
 [HINT] Use ``create_polygon_from_latlons()`` to create polygon."
@@ -143,10 +154,10 @@
         start_idx = get_index_from_coordinate(start, zoom_level)
         end_idx = get_index_from_coordinate(end, zoom_level)
         grid_bb = GridBoundingBox(start_idx, end_idx)
 
         self._initialise_downloader()
         self._initialise_merger(f"{path_save}/")
         if not overwrite:
-            if self._check_map_exists(grid_bb):
+            if self._check_map_exists(grid_bb, map_name):
                 return
-        self._download_map(grid_bb)
+        self._download_map(grid_bb, map_name)
```

### Comparing `mapreader-1.1.4/mapreader/download/downloader_utils.py` & `mapreader-1.1.5/mapreader/download/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/download/sheet_downloader.py` & `mapreader-1.1.5/mapreader/download/sheet_downloader.py`

 * *Files 4% similar despite different names*

```diff
@@ -555,29 +555,31 @@
                     f'[INFO] "{path_save}{map_name}.png" already exists. Skipping download.'
                 )
                 return True
             except OSError:
                 return False
         return False
 
-    def _download_map(self, feature: dict) -> bool:
+    def _download_map(self, feature: dict, download_in_parallel: bool = True) -> bool:
         """
         Downloads a single map sheet and saves as png file.
 
         Parameters
         ----------
         feature : dict
 
         Returns
         -------
         bool
             True if map was downloaded successfully, False if not.
         """
         map_name = str("map_" + feature["properties"]["IMAGE"])
-        self.downloader.download_tiles(feature["grid_bb"])
+        self.downloader.download_tiles(
+            feature["grid_bb"], download_in_parallel=download_in_parallel
+        )
         success = self.merger.merge(feature["grid_bb"], map_name)
         if success:
             print(f'[INFO] Downloaded "{map_name}.png"')
         else:
             print(f'[WARNING] Download of "{map_name}.png" was unsuccessful.')
 
         shutil.rmtree(DEFAULT_TEMP_FOLDER)
@@ -677,81 +679,95 @@
 
     def _download_map_sheets(
         self,
         features: list,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         overwrite: bool | None = False,
+        download_in_parallel: bool = True,
         **kwargs: dict | None,
     ):
         """Download map sheets from a list of features.
 
         Parameters
         ----------
         features : list
             list of features to download
         path_save : str, optional
             Path to save map sheets, by default "maps"
         metadata_fname : str, optional
             Name to use for metadata file, by default "metadata.csv"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_save_metadata()`` method.
         """
 
         for feature in tqdm(features):
             if not overwrite:
                 if self._check_map_sheet_exists(feature):
                     continue
-            success = self._download_map(feature)
+            success = self._download_map(
+                feature, download_in_parallel=download_in_parallel
+            )
             if success:
                 metadata_path = f"{path_save}/{metadata_fname}"
                 self._save_metadata(
                     feature=feature, out_filepath=metadata_path, **kwargs
                 )
 
     def download_all_map_sheets(
         self,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         overwrite: bool | None = False,
+        download_in_parallel: bool = True,
         **kwargs: dict | None,
     ) -> None:
         """
         Downloads all map sheets in metadata.
 
         Parameters
         ----------
         path_save : str, optional
             Path to save map sheets, by default "maps"
         metadata_fname : str, optional
             Name to use for metadata file, by default "metadata.csv"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_download_map_sheets()`` method.
         """
         if not self.grid_bbs:
             raise ValueError("[ERROR] Please first run ``get_grid_bb()``")
 
         self._initialise_downloader()
         self._initialise_merger(path_save)
 
         features = self.features
         self._download_map_sheets(
-            features, path_save, metadata_fname, overwrite, **kwargs
+            features,
+            path_save,
+            metadata_fname,
+            overwrite,
+            download_in_parallel=download_in_parallel,
+            **kwargs,
         )
 
     def download_map_sheets_by_wfs_ids(
         self,
         wfs_ids: list | int,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         overwrite: bool | None = False,
+        download_in_parallel: bool = True,
         **kwargs: dict | None,
     ) -> None:
         """
         Downloads map sheets by WFS ID numbers.
 
         Parameters
         ----------
@@ -759,14 +775,16 @@
             The WFS ID numbers of the maps to download.
         path_save : str, optional
             Path to save map sheets, by default "maps"
         metadata_fname : str, optional
             Name to use for metadata file, by default "metadata.csv"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_download_map_sheets()`` method.
         """
 
         if not self.wfs_id_nos:
             self.extract_wfs_id_nos()
 
@@ -790,24 +808,30 @@
         features = []
         for feature in self.features:
             wfs_id_no = feature["wfs_id_no"]
             if wfs_id_no in requested_maps:
                 features.append(feature)
 
         self._download_map_sheets(
-            features, path_save, metadata_fname, overwrite, **kwargs
+            features,
+            path_save,
+            metadata_fname,
+            overwrite,
+            download_in_parallel=download_in_parallel,
+            **kwargs,
         )
 
     def download_map_sheets_by_polygon(
         self,
         polygon: Polygon,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         mode: str | None = "within",
         overwrite: bool | None = False,
+        download_in_parallel: bool = True,
         **kwargs: dict | None,
     ) -> None:
         """
         Downloads any map sheets which are found within or intersecting with a defined polygon.
 
         Parameters
         ----------
@@ -820,14 +844,16 @@
         mode : str, optional
             The mode to use when finding maps.
             Options of ``"within"``, which returns all map sheets which are completely within the defined polygon,
             and ``"intersects""``, which returns all map sheets which intersect/overlap with the defined polygon.
             By default "within".
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_download_map_sheets()`` method.
 
         Notes
         -----
         Use ``create_polygon_from_latlons()`` to create polygon.
         """
@@ -865,23 +891,29 @@
                 if map_polygon.within(polygon):
                     features.append(feature)
             elif mode == "intersects":
                 if map_polygon.intersects(polygon):
                     features.append(feature)
 
         self._download_map_sheets(
-            features, path_save, metadata_fname, overwrite, **kwargs
+            features,
+            path_save,
+            metadata_fname,
+            overwrite,
+            download_in_parallel=download_in_parallel,
+            **kwargs,
         )
 
     def download_map_sheets_by_coordinates(
         self,
         coords: tuple,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         overwrite: bool | None = False,
+        download_in_parallel: bool = True,
         **kwargs: dict | None,
     ) -> None:
         """
         Downloads any maps sheets which contain a defined set of coordinates.
         Coordinates are (x,y).
 
         Parameters
@@ -890,14 +922,16 @@
             Coordinates in ``(x,y)`` format.
         path_save : str, optional
             Path to save map sheets, by default "maps"
         metadata_fname : str, optional
             Name to use for metadata file, by default "metadata.csv"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_download_map_sheets()`` method.
         """
 
         if not isinstance(coords, tuple):
             raise ValueError("[ERROR] Please pass coords as a tuple in the form (x,y).")
 
@@ -918,23 +952,29 @@
         features = []
         for feature in self.features:
             map_polygon = feature["polygon"]
             if map_polygon.contains(coords):
                 features.append(feature)
 
         self._download_map_sheets(
-            features, path_save, metadata_fname, overwrite, **kwargs
+            features,
+            path_save,
+            metadata_fname,
+            overwrite,
+            download_in_parallel=download_in_parallel,
+            **kwargs,
         )
 
     def download_map_sheets_by_line(
         self,
         line: LineString,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         overwrite: bool | None = False,
+        download_in_parallel: bool = True,
         **kwargs: dict | None,
     ) -> None:
         """
         Downloads any maps sheets which intersect with a line.
 
         Parameters
         ----------
@@ -942,14 +982,16 @@
             shapely LineString
         path_save : str, optional
             Path to save map sheets, by default "maps"
         metadata_fname : str, optional
             Name to use for metadata file, by default "metadata.csv"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_download_map_sheets()`` method.
 
         Notes
         -----
         Use ``create_line_from_latlons()`` to create line.
         """
@@ -976,24 +1018,30 @@
         for feature in self.features:
             map_polygon = feature["polygon"]
 
             if map_polygon.intersects(line):
                 features.append(feature)
 
         self._download_map_sheets(
-            features, path_save, metadata_fname, overwrite, **kwargs
+            features,
+            path_save,
+            metadata_fname,
+            overwrite,
+            download_in_parallel=download_in_parallel,
+            **kwargs,
         )
 
     def download_map_sheets_by_string(
         self,
         string: str,
         keys: str | list = None,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         overwrite: bool | None = False,
+        download_in_parallel: bool = True,
         **kwargs: dict | None,
     ) -> None:
         """
         Download map sheets by searching for a string in a chosen metadata field.
 
         Parameters
         ----------
@@ -1009,14 +1057,16 @@
             If ``None``, will search in all metadata fields. By default ``None``.
         path_save : str, optional
             Path to save map sheets, by default "maps"
         metadata_fname : str, optional
             Name to use for metadata file, by default "metadata.csv"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_download_map_sheets()`` method.
 
         Notes
         -----
         ``string`` is case insensitive.
         """
@@ -1049,50 +1099,63 @@
 
             match = bool(re.search(string, str(field_to_search), re.IGNORECASE))
 
             if match:
                 features.append(feature)
 
         self._download_map_sheets(
-            features, path_save, metadata_fname, overwrite, **kwargs
+            features,
+            path_save,
+            metadata_fname,
+            overwrite,
+            download_in_parallel=download_in_parallel,
+            **kwargs,
         )
 
     def download_map_sheets_by_queries(
         self,
         path_save: str | None = "maps",
         metadata_fname: str | None = "metadata.csv",
         overwrite: bool | None = False,
+        download_in_parallel: bool = True,
         **kwargs: dict | None,
     ) -> None:
         """
         Downloads map sheets saved as query results.
 
         Parameters
         ----------
         path_save : str, optional
             Path to save map sheets, by default "maps"
         metadata_fname : str, optional
             Name to use for metadata file, by default "metadata.csv"
         overwrite : bool, optional
             Whether to overwrite existing maps, by default ``False``.
+        download_in_parallel : bool, optional
+            Whether to download tiles in parallel, by default ``True``.
         **kwargs : dict, optional
             Keyword arguments to pass to the ``_download_map_sheets()`` method.
         """
         if not self.grid_bbs:
             raise ValueError("[ERROR] Please first run ``get_grid_bb()``")
 
         self._initialise_downloader()
         self._initialise_merger(path_save)
 
         if len(self.found_queries) == 0:
             raise ValueError("[ERROR] No query results found/saved.")
 
         features = self.found_queries
         self._download_map_sheets(
-            features, path_save, metadata_fname, overwrite, **kwargs
+            features,
+            path_save,
+            metadata_fname,
+            overwrite,
+            download_in_parallel=download_in_parallel,
+            **kwargs,
         )
 
     def hist_published_dates(self, **kwargs) -> None:
         """
         Plots a histogram of the publication dates of maps in metadata.
 
         Parameters
```

### Comparing `mapreader-1.1.4/mapreader/download/tile_loading.py` & `mapreader-1.1.5/mapreader/download/tile_loading.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/download/tile_merging.py` & `mapreader-1.1.5/mapreader/download/tile_merging.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/load/geo_utils.py` & `mapreader-1.1.5/mapreader/load/geo_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,25 +55,23 @@
     -------
     list
         shape, old CRS, new CRS, reprojected coord, size in meters
     """
     tiff_shape, tiff_proj, tiff_coord = extractGeoInfo(image_path)
 
     # Coordinate transformation: proj1 ---> proj2
-    transformer = Transformer.from_crs(tiff_proj, target_crs)
-    ymin, xmin = transformer.transform(tiff_coord[0], tiff_coord[1])
-    ymax, xmax = transformer.transform(tiff_coord[2], tiff_coord[3])
-    coord = (xmin, ymin, xmax, ymax)
-
+    transformer = Transformer.from_crs(tiff_proj, target_crs, always_xy=True)
+    coord = transformer.transform_bounds(*tiff_coord)
     print(f"[INFO] New CRS: {target_crs}")
     print("[INFO] Reprojected coordinates: {:.4f} {:.4f} {:.4f} {:.4f}".format(*coord))
 
     height, width, _ = tiff_shape
 
     # Calculate the size of image in meters
+    xmin, ymin, xmax, ymax = coord
     if calc_size_in_m:
         if calc_size_in_m in ["geodesic", "gd"]:
             bottom = geodesic((ymin, xmin), (ymin, xmax)).meters
             right = geodesic((ymin, xmax), (ymax, xmax)).meters
             top = geodesic((ymax, xmax), (ymax, xmin)).meters
             left = geodesic((ymax, xmin), (ymin, xmin)).meters
```

### Comparing `mapreader-1.1.4/mapreader/load/images.py` & `mapreader-1.1.5/mapreader/load/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -981,14 +981,15 @@
     def patchify_all(
         self,
         method: str | None = "pixel",
         patch_size: int | None = 100,
         tree_level: str | None = "parent",
         path_save: str | None = None,
         add_to_parents: bool | None = True,
+        square_cuts: bool | None = False,
         resize_factor: bool | None = False,
         output_format: str | None = "png",
         rewrite: bool | None = False,
         verbose: bool | None = False,
     ) -> None:
         """
         Patchify all images in the specified ``tree_level`` and (if ``add_to_parents=True``) add the patches to the MapImages instance's ``images`` dictionary.
@@ -1007,14 +1008,17 @@
         path_save : str, optional
             Directory to save the patches.
             If None, will be set as f"patches_{patch_size}_{method}" (e.g. "patches_100_pixel").
             By default None.
         add_to_parents : bool, optional
             If True, patches will be added to the MapImages instance's
             ``images`` dictionary, by default ``True``.
+        square_cuts : bool, optional
+            If True, all patches will have the same number of pixels in
+            x and y, by default ``False``.
         resize_factor : bool, optional
             If True, resize the images before patchifying, by default ``False``.
         output_format : str, optional
             Format to use when writing image files, by default ``"png"``.
         rewrite : bool, optional
             If True, existing patches will be rewritten, by default ``False``.
         verbose : bool, optional
@@ -1054,24 +1058,41 @@
                     )
 
                 mean_pixel_height = self._calc_pixel_height_width(image_id)[1]
                 patch_size = int(
                     original_patch_size / mean_pixel_height
                 )  ## check this is correct - should patch be different size in x and y?
 
-            self._patchify_by_pixel(
-                image_id=image_id,
-                patch_size=patch_size,
-                path_save=path_save,
-                add_to_parents=add_to_parents,
-                resize_factor=resize_factor,
-                output_format=output_format,
-                rewrite=rewrite,
-                verbose=verbose,
-            )
+            if square_cuts:
+                print(
+                    "[WARNING] Square cuts is deprecated as of version 1.1.3 and will soon be removed."
+                )
+
+                self._patchify_by_pixel_square(
+                    image_id=image_id,
+                    patch_size=patch_size,
+                    path_save=path_save,
+                    add_to_parents=add_to_parents,
+                    resize_factor=resize_factor,
+                    output_format=output_format,
+                    rewrite=rewrite,
+                    verbose=verbose,
+                )
+
+            else:
+                self._patchify_by_pixel(
+                    image_id=image_id,
+                    patch_size=patch_size,
+                    path_save=path_save,
+                    add_to_parents=add_to_parents,
+                    resize_factor=resize_factor,
+                    output_format=output_format,
+                    rewrite=rewrite,
+                    verbose=verbose,
+                )
 
     def _patchify_by_pixel(
         self,
         image_id: str,
         patch_size: int,
         path_save: str,
         add_to_parents: bool | None = True,
@@ -1161,14 +1182,102 @@
                         parent_path=parent_path,
                         tree_level="patch",
                         pixel_bounds=(min_x, min_y, max_x, max_y),
                     )
                     self._add_patch_coords_id(patch_id)
                     self._add_patch_polygons_id(patch_id)
 
+    def _patchify_by_pixel_square(
+        self,
+        image_id: str,
+        patch_size: int,
+        path_save: str,
+        add_to_parents: bool | None = True,
+        resize_factor: bool | None = False,
+        output_format: str | None = "png",
+        rewrite: bool | None = False,
+        verbose: bool | None = False,
+    ):
+        """Patchify one image and (if ``add_to_parents=True``) add the patch to the MapImages instance's ``images`` dictionary.
+        Use square cuts for patches at edges.
+
+        Parameters
+        ----------
+        image_id : str
+            The ID of the image to patchify
+        patch_size : int
+            Number of pixels in both x and y to use for slicing
+        path_save : str
+            Directory to save the patches.
+        add_to_parents : bool, optional
+            If True, patches will be added to the MapImages instance's
+            ``images`` dictionary, by default ``True``.
+        resize_factor : bool, optional
+            If True, resize the images before patchifying, by default ``False``.
+        output_format : str, optional
+            Format to use when writing image files, by default ``"png"``.
+        rewrite : bool, optional
+            If True, existing patches will be rewritten, by default ``False``.
+        verbose : bool, optional
+            If True, progress updates will be printed throughout, by default
+            ``False``.
+        """
+        tree_level = self._get_tree_level(image_id)
+
+        parent_path = self.images[tree_level][image_id]["image_path"]
+        img = Image.open(parent_path)
+
+        if resize_factor:
+            original_height, original_width = img.height, img.width
+            img = img.resize(
+                (
+                    int(original_width / resize_factor),
+                    int(original_height / resize_factor),
+                )
+            )
+
+        height, width = img.height, img.width
+
+        for x in range(0, width, patch_size):
+            for y in range(0, height, patch_size):
+                max_x = min(x + patch_size, width)
+                max_y = min(y + patch_size, height)
+
+                # move min_x and min_y back a bit so the patch is square
+                min_x = x - (patch_size - (max_x - x))
+                min_y = y - (patch_size - (max_y - y))
+
+                patch_id = f"patch-{min_x}-{min_y}-{max_x}-{max_y}-#{image_id}#.{output_format}"
+                patch_path = os.path.join(path_save, patch_id)
+                patch_path = os.path.abspath(patch_path)
+
+                if os.path.isfile(patch_path) and not rewrite:
+                    self._print_if_verbose(
+                        f"[INFO] File already exists: {patch_path}.", verbose
+                    )
+
+                else:
+                    self._print_if_verbose(
+                        f'[INFO] Creating "{patch_id}". Number of pixels in x,y: {max_x - min_x},{max_y - min_y}.',
+                        verbose,
+                    )
+
+                    patch = img.crop((min_x, min_y, max_x, max_y))
+                    patch.save(patch_path, output_format)
+
+                if add_to_parents:
+                    self._images_constructor(
+                        image_path=patch_path,
+                        parent_path=parent_path,
+                        tree_level="patch",
+                        pixel_bounds=(min_x, min_y, max_x, max_y),
+                    )
+                    self._add_patch_coords_id(patch_id)
+                    self._add_patch_polygons_id(patch_id)
+
     def _add_patch_to_parent(self, patch_id: str) -> None:
         """
         Add patch to parent.
 
         Parameters
         ----------
         patch_id : str
@@ -2104,23 +2213,16 @@
             return
 
         else:
             # Get coordinates as string
             tiff_proj = tiff_src.crs.to_string()
             # Coordinate transformation: proj1 ---> proj2
             # tiff is "lat, lon" instead of "x, y"
-            transformer = Transformer.from_crs(tiff_proj, target_crs)
-            ymin, xmin = transformer.transform(
-                tiff_src.bounds.left, tiff_src.bounds.bottom
-            )
-            ymax, xmax = transformer.transform(
-                tiff_src.bounds.right, tiff_src.bounds.top
-            )
-            # New projected coordinates
-            coords = (xmin, ymin, xmax, ymax)
+            transformer = Transformer.from_crs(tiff_proj, target_crs, always_xy=True)
+            coords = transformer.transform_bounds(*tiff_src.bounds)
             self.parents[image_id]["coordinates"] = coords
             self.parents[image_id]["crs"] = target_crs
 
     @staticmethod
     def _print_if_verbose(msg: str, verbose: bool) -> None:
         """
         Print message if verbose is True.
```

### Comparing `mapreader-1.1.4/mapreader/load/loader.py` & `mapreader-1.1.5/mapreader/load/loader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/process/post_process.py` & `mapreader-1.1.5/mapreader/process/post_process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/process/process.py` & `mapreader-1.1.5/mapreader/process/process.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/utils/compute_and_save_stats.py` & `mapreader-1.1.5/mapreader/utils/compute_and_save_stats.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader/utils/slice_parallel.py` & `mapreader-1.1.5/mapreader/utils/slice_parallel.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader.egg-info/PKG-INFO` & `mapreader-1.1.5/mapreader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapreader
-Version: 1.1.4
+Version: 1.1.5
 Summary: A computer vision pipeline for the semantic exploration of maps/images at scale
 Home-page: https://github.com/Living-with-machines/MapReader
 Download-URL: https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip
 Author: MapReader team
 License: MIT License
 Keywords: Computer Vision,Classification,Deep Learning,living with machines
 Platform: OS Independent
@@ -20,15 +20,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib<4.0.0,>=3.5.0
 Requires-Dist: numpy<2.0.0,>=1.21.5
 Requires-Dist: pandas<2.0.0,>=1.3.4
 Requires-Dist: pyproj<4.0.0,>=3.2.0
 Requires-Dist: azure-storage-blob<13.0.0,>=12.9.0
@@ -51,21 +51,24 @@
 Requires-Dist: rasterio<2.0.0,>=1.2.10
 Requires-Dist: simplekml<2.0.0,>=1.3.6
 Requires-Dist: versioneer>=0.28
 Requires-Dist: tqdm<5.0.0
 Requires-Dist: torchinfo<2.0.0
 Requires-Dist: openpyxl<4.0.0
 Requires-Dist: geopandas<1.0.0
+Requires-Dist: pyogrio>=0.7.2
 Provides-Extra: dev
 Requires-Dist: pytest<8.0.0; extra == "dev"
 Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == "dev"
 Requires-Dist: timm<1.0.0; extra == "dev"
 Requires-Dist: transformers<5.0.0; extra == "dev"
 Requires-Dist: black<24.0.0,>=23.7.0; extra == "dev"
 Requires-Dist: flake8<7.0.0,>=6.0.0; extra == "dev"
+Provides-Extra: geo
+Requires-Dist: cartopy>=0.20.0; extra == "geo"
 
 <div align="center">
     <br>
     <p align="center">
     <h1>MapReader</h1>
     <h2>A computer vision pipeline for exploring and analyzing images at scale</h2>
     </p>
@@ -128,15 +131,15 @@
 **New users** should refer to the [Installation instructions](https://mapreader.readthedocs.io/en/latest/Install.html) and [Input guidance](https://mapreader.readthedocs.io/en/latest/Input-guidance.html) for help with the initial set up of MapReader.
 
 **All users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/latest/User-guide/User-guide.html) for guidance on how to use MapReader. This contains end-to-end instructions on how to use the MapReader pipeline, plus a number of worked examples illustrating use cases such as:
 
 - Geospatial images (i.e. maps)
 - Non-geospatial images
 
- **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
+ **Developers and contributors** may also want to refer to the [API documentation](https://mapreader.readthedocs.io/en/latest/api/index.html) and [Contribution guide](https://mapreader.readthedocs.io/en/latest/Contribution-guide/Contribution-guide.html) for guidance on how to contribute to the MapReader package.
 
 **Join our Slack workspace!**
 Please fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9) to receive an invitation to the Slack workspace.
 
 ## What is included in this repo?
 
 The MapReader package provides a set of tools to:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mapreader Version: 1.1.4 Summary: A computer vision
+Metadata-Version: 2.1 Name: mapreader Version: 1.1.5 Summary: A computer vision
 pipeline for the semantic exploration of maps/images at scale Home-page: https:
 //github.com/Living-with-machines/MapReader Download-URL: https://github.com/
 Living-with-machines/MapReader/archive/refs/heads/main.zip Author: MapReader
 team License: MIT License Keywords: Computer Vision,Classification,Deep
 Learning,living with machines Platform: OS Independent Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
@@ -10,34 +10,35 @@
 Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: Unix Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent Classifier: Topic :: Software
 Development Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7, <3.11 Description-Content-Type: text/markdown License-
+Requires-Python: >=3.8, <3.11 Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: matplotlib<4.0.0,>=3.5.0 Requires-Dist:
 numpy<2.0.0,>=1.21.5 Requires-Dist: pandas<2.0.0,>=1.3.4 Requires-Dist:
 pyproj<4.0.0,>=3.2.0 Requires-Dist: azure-storage-blob<13.0.0,>=12.9.0
 Requires-Dist: aiohttp<4.0.0,>=3.8.1 Requires-Dist: Shapely<3.0.0,>=2.0.0
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.1 Requires-Dist: scikit-image>=0.18.3
 Requires-Dist: scikit-learn<2.0.0,>=1.0.1 Requires-Dist: torch<2.0.0,>=1.10.0
 Requires-Dist: torchvision<0.12.1,>=0.11.1 Requires-Dist: jupyter<2.0.0,>=1.0.0
 Requires-Dist: ipykernel<7.0.0,>=6.5.1 Requires-Dist: ipywidgets<9.0.0,>=8.0.0
 Requires-Dist: ipyannotate==0.1.0-beta.0 Requires-Dist: Cython<0.30.0,>=0.29.24
 Requires-Dist: PyYAML<7.0,>=6.0 Requires-Dist: tensorboard<3.0.0,>=2.7.0
 Requires-Dist: parhugin<0.0.4,>=0.0.3 Requires-Dist: geopy==2.1.0 Requires-
 Dist: rasterio<2.0.0,>=1.2.10 Requires-Dist: simplekml<2.0.0,>=1.3.6 Requires-
 Dist: versioneer>=0.28 Requires-Dist: tqdm<5.0.0 Requires-Dist: torchinfo<2.0.0
-Requires-Dist: openpyxl<4.0.0 Requires-Dist: geopandas<1.0.0 Provides-Extra:
-dev Requires-Dist: pytest<8.0.0; extra == "dev" Requires-Dist: pytest-
-cov<5.0.0,>=4.1.0; extra == "dev" Requires-Dist: timm<1.0.0; extra == "dev"
-Requires-Dist: transformers<5.0.0; extra == "dev" Requires-Dist:
-black<24.0.0,>=23.7.0; extra == "dev" Requires-Dist: flake8<7.0.0,>=6.0.0;
-extra == "dev"
+Requires-Dist: openpyxl<4.0.0 Requires-Dist: geopandas<1.0.0 Requires-Dist:
+pyogrio>=0.7.2 Provides-Extra: dev Requires-Dist: pytest<8.0.0; extra == "dev"
+Requires-Dist: pytest-cov<5.0.0,>=4.1.0; extra == "dev" Requires-Dist:
+timm<1.0.0; extra == "dev" Requires-Dist: transformers<5.0.0; extra == "dev"
+Requires-Dist: black<24.0.0,>=23.7.0; extra == "dev" Requires-Dist:
+flake8<7.0.0,>=6.0.0; extra == "dev" Provides-Extra: geo Requires-Dist:
+cartopy>=0.20.0; extra == "geo"
 
                             ************ MMaappRReeaaddeerr ************
  ********** AA ccoommppuutteerr vviissiioonn ppiippeelliinnee ffoorr eexxpplloorriinngg aanndd aannaallyyzziinngg iimmaaggeess aatt ssccaallee
                                      **********
                  _[_P_y_P_I_]_[_L_i_c_e_n_s_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _b_a_d_g_e_]_[_D_O_I_]
        _[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_L_i_v_i_n_g_-_w_i_t_h_-_m_a_c_h_i_n_e_s_/_M_a_p_R_e_a_d_e_r_/_g_r_a_p_h_/
                           _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_3_8_G_Q_3_O_1_G_B_5_]
@@ -72,22 +73,22 @@
 users** should refer to our [User Guide](https://mapreader.readthedocs.io/en/
 latest/User-guide/User-guide.html) for guidance on how to use MapReader. This
 contains end-to-end instructions on how to use the MapReader pipeline, plus a
 number of worked examples illustrating use cases such as: - Geospatial images
 (i.e. maps) - Non-geospatial images **Developers and contributors** may also
 want to refer to the [API documentation](https://mapreader.readthedocs.io/en/
 latest/api/index.html) and [Contribution guide](https://
-mapreader.readthedocs.io/en/latest/Contribution-guide.html) for guidance on how
-to contribute to the MapReader package. **Join our Slack workspace!** Please
-fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9) to receive an
-invitation to the Slack workspace. ## What is included in this repo? The
-MapReader package provides a set of tools to: - **Download** images/maps and
-metadata stored on web-servers (e.g. tileservers which can be used to retrieve
-maps from OpenStreetMap (OSM), the National Library of Scotland (NLS), or
-elsewhere). - **Load** images/maps and metadata stored locally. - **Pre-
+mapreader.readthedocs.io/en/latest/Contribution-guide/Contribution-guide.html)
+for guidance on how to contribute to the MapReader package. **Join our Slack
+workspace!** Please fill out [this form](https://forms.gle/dXjECHZQkwrZ3Xpt9)
+to receive an invitation to the Slack workspace. ## What is included in this
+repo? The MapReader package provides a set of tools to: - **Download** images/
+maps and metadata stored on web-servers (e.g. tileservers which can be used to
+retrieve maps from OpenStreetMap (OSM), the National Library of Scotland (NLS),
+or elsewhere). - **Load** images/maps and metadata stored locally. - **Pre-
 process** images/maps: - patchify (create patches from a parent image), -
 resample (use image transformations to alter pixel-dimensions/resolution/
 orientation/etc.), - remove borders outside the neatline, - reproject between
 coordinate reference systems (CRS). - **Annotate** images/maps (or their
 patches) using an interactive annotation tool. - **Train or fine-tune**
 Computer Vision (CV) models and use these to **predict** labels (i.e. model
 inference) on large sets of images/maps. Various **plotting and analysis**
```

### Comparing `mapreader-1.1.4/mapreader.egg-info/SOURCES.txt` & `mapreader-1.1.5/mapreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/mapreader.egg-info/requires.txt` & `mapreader-1.1.5/mapreader.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 rasterio<2.0.0,>=1.2.10
 simplekml<2.0.0,>=1.3.6
 versioneer>=0.28
 tqdm<5.0.0
 torchinfo<2.0.0
 openpyxl<4.0.0
 geopandas<1.0.0
+pyogrio>=0.7.2
 
 [dev]
 pytest<8.0.0
 pytest-cov<5.0.0,>=4.1.0
 timm<1.0.0
 transformers<5.0.0
 black<24.0.0,>=23.7.0
 flake8<7.0.0,>=6.0.0
+
+[geo]
+cartopy>=0.20.0
```

### Comparing `mapreader-1.1.4/setup.py` & `mapreader-1.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     long_description_content_type="text/markdown",
     zip_safe=False,
     url="https://github.com/Living-with-machines/MapReader",
     download_url="https://github.com/Living-with-machines/MapReader/archive/refs/heads/main.zip",
     packages=setuptools.find_packages(),
     include_package_data=True,
     platforms="OS Independent",
-    python_requires=">=3.7, <3.11",
+    python_requires=">=3.8, <3.11",
     install_requires=[
         "matplotlib>=3.5.0,<4.0.0",
         "numpy>=1.21.5,<2.0.0",
         "pandas>=1.3.4,<2.0.0",
         "pyproj>=3.2.0,<4.0.0",
         "azure-storage-blob>=12.9.0,<13.0.0",
         "aiohttp>=3.8.1,<4.0.0",
@@ -53,25 +53,29 @@
         "rasterio>=1.2.10,<2.0.0",
         "simplekml>=1.3.6,<2.0.0",
         "versioneer>=0.28",
         "tqdm<5.0.0",
         "torchinfo<2.0.0",
         "openpyxl<4.0.0",
         "geopandas<1.0.0",
+        "pyogrio>=0.7.2",
     ],
     extras_require={
         "dev": [
             "pytest<8.0.0",
             "pytest-cov>=4.1.0,<5.0.0",
             "timm<1.0.0",
             "transformers<5.0.0",
             "black>=23.7.0,<24.0.0",
             "flake8>=6.0.0,<7.0.0",
-        ]
-    },
+        ],
+        "geo": [
+            "cartopy>=0.20.0"
+        ],
+    },  
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Intended Audience :: End Users/Desktop",
```

### Comparing `mapreader-1.1.4/tests/test_annotator.py` & `mapreader-1.1.5/tests/test_annotator.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/tests/test_geo_pipeline.py` & `mapreader-1.1.5/tests/test_geo_pipeline.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/tests/test_post_processing.py` & `mapreader-1.1.5/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/tests/test_sheet_downloader.py` & `mapreader-1.1.5/tests/test_sheet_downloader.py`

 * *Files identical despite different names*

### Comparing `mapreader-1.1.4/versioneer.py` & `mapreader-1.1.5/versioneer.py`

 * *Files identical despite different names*

