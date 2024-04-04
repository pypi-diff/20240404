# Comparing `tmp/sliderule-4.3.1.tar.gz` & `tmp/sliderule-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-4.3.1.tar", last modified: Fri Mar  8 15:17:43 2024, max compression
+gzip compressed data, was "sliderule-4.3.2.tar", last modified: Thu Apr  4 20:23:45 2024, max compression
```

## Comparing `sliderule-4.3.1.tar` & `sliderule-4.3.2.tar`

### file list

```diff
@@ -1,56 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:17:43.039077 sliderule-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-08 15:17:35.000000 sliderule-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-08 15:17:35.000000 sliderule-4.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-08 15:17:43.039077 sliderule-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-08 15:17:35.000000 sliderule-4.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-08 15:17:35.000000 sliderule-4.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 15:17:43.039077 sliderule-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-08 15:17:35.000000 sliderule-4.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:17:43.035077 sliderule-4.3.1/sliderule/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    36770 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16231 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (127)    30789 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (127)    38833 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (127)   117488 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)    50023 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/swot.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-08 15:17:35.000000 sliderule-4.3.1/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:17:43.039077 sliderule-4.3.1/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-08 15:17:42.000000 sliderule-4.3.1/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-08 15:17:43.000000 sliderule-4.3.1/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 15:17:42.000000 sliderule-4.3.1/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-08 15:17:42.000000 sliderule-4.3.1/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-08 15:17:42.000000 sliderule-4.3.1/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:17:43.039077 sliderule-4.3.1/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/build_3dep_DEM_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/create_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/lpdaac_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/opendata_worldcover.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-03-08 15:17:35.000000 sliderule-4.3.1/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-08 15:17:35.000000 sliderule-4.3.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:23:45.794572 sliderule-4.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-04 20:23:36.000000 sliderule-4.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 20:23:36.000000 sliderule-4.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 20:23:45.794572 sliderule-4.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-04 20:23:36.000000 sliderule-4.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-04 20:23:36.000000 sliderule-4.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:23:45.794572 sliderule-4.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-04 20:23:36.000000 sliderule-4.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:23:45.786572 sliderule-4.3.2/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/bathy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36904 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16231 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9779 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36298 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38833 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118505 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50316 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/swot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-04 20:23:36.000000 sliderule-4.3.2/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:23:45.794572 sliderule-4.3.2/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 20:23:45.000000 sliderule-4.3.2/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:23:45.790572 sliderule-4.3.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/bathy_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/build_3dep_DEM_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/container_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/lpdaac_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/opendata_worldcover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-04 20:23:36.000000 sliderule-4.3.2/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 20:23:36.000000 sliderule-4.3.2/version.txt
```

### Comparing `sliderule-4.3.1/LICENSE` & `sliderule-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/PKG-INFO` & `sliderule-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 4.3.1
+Version: 4.3.2
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-4.3.1/README.md` & `sliderule-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/setup.py` & `sliderule-4.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/sliderule/container.py` & `sliderule-4.3.2/sliderule/container.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/sliderule/earthdata.py` & `sliderule-4.3.2/sliderule/earthdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 import time
 import itertools
 import copy
 import json
 import ssl
 import urllib.request
+import http
 import requests
 import numpy
 import geopandas
 from datetime import datetime
 from shapely.geometry.multipolygon import MultiPolygon
 from shapely.geometry import Polygon
 from sliderule import logger
@@ -322,14 +323,16 @@
 
             # call into NSIDC routines to make CMR request
             try:
                 urls,metadata = __cmr_query(provider, short_name, version, time_start, time_end, polygon=polystr, return_metadata=return_metadata, name_filter=name_filter)
                 break # exit loop because cmr search was successful
             except urllib.error.HTTPError as e:
                 logger.error('HTTP Request Error: {}'.format(e.reason))
+            except http.client.HTTPException as e:
+                logger.error('HTTP Client Error: {}'.format(e.reason))
             except RuntimeError as e:
                 logger.error("Runtime Error:", e)
 
             # simplify polygon
             if polygon and tolerance:
                 raw_multi_polygon = [[(tuple([(c['lon'], c['lat']) for c in polygon]), [])]]
                 shape = MultiPolygon(*raw_multi_polygon)
```

### Comparing `sliderule-4.3.1/sliderule/gedi.py` & `sliderule-4.3.2/sliderule/gedi.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/sliderule/h5.py` & `sliderule-4.3.2/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/sliderule/icesat2.py` & `sliderule-4.3.2/sliderule/icesat2.py`

 * *Files 10% similar despite different names*

```diff
@@ -735,7 +735,140 @@
     except RuntimeError as e:
         logger.critical(e)
         if rethrow_exceptions:
             raise
     
     # Error Case
     return sliderule.emptyframe()
+
+#
+# ATL24 Gold Standard
+#
+def atl24g (parm, resource):
+    '''
+    Produces gold standard bathymetry photon classification of ATL03 data
+
+    Parameters
+    ----------
+        parms:      dict
+                    parameters used to configure ATL03 subsetting (see `Parameters </web/rtd/user_guide/ICESat-2.html#parameters>`_)
+        resource:   str
+                    ATL03 HDF5 filename
+
+    Returns
+    -------
+    GeoDataFrame
+        ATL03 extents (see `Photon Segments </web/rtd/user_guide/ICESat-2.html#segmented-photon-data>`_)
+    '''
+    return atl03sp(parm, resources=[resource])
+
+#
+#  Parallel  Gold Standard
+#
+def atl24gp(parm, callbacks={}, resources=None, keep_id=False, height_key=None):
+    '''
+    Performs ATL24 gold standard generation in parallel on ATL03 data. Unlike the `atl03s <#atl03s>`_ function,
+    this function does not take a resource as a parameter; instead it is expected that the **parm** argument includes a polygon which
+    is used to fetch all available resources from the CMR system automatically.
+
+    Parameters
+    ----------
+        parms:          dict
+                        parameters used to configure ATL03 subsetting (see `Parameters </web/rtd/user_guide/ICESat-2.html#parameters>`_)
+        callbacks:      dictionary
+                        a callback function that is called for each result record
+        resources:      list
+                        a list of granules to process (e.g. ["ATL03_20181019065445_03150111_005_01.h5", ...])
+        keep_id:        bool
+                        whether to retain the "extent_id" column in the GeoDataFrame for future merges
+        height_key:     str
+                        identifies the name of the column provided for the 3D CRS transformation
+
+    Returns
+    -------
+    GeoDataFrame
+        ATL03 segments (see `Photon Segments </web/rtd/user_guide/ICESat-2.html#photon-segments>`_)
+    '''
+    try:
+        tstart = time.perf_counter()
+
+        # Build Request
+        rqst = __build_request(parm, resources)
+
+        # Make Request
+        rsps = sliderule.source("atl24gp", rqst, stream=True, callbacks=callbacks)
+
+        # Check for Output Options
+        if "output" in parm:
+            profiles[atl24gp.__name__] = time.perf_counter() - tstart
+            return sliderule.procoutputfile(parm, rsps)
+        else: # Native Output
+            # Flatten Responses
+            tstart_flatten = time.perf_counter()
+            columns = {}
+            sample_photon_record = None
+            photon_records = []
+            num_photons = 0
+            if len(rsps) > 0:
+                # Sort Records
+                for rsp in rsps:
+                    if 'bathyrec' in rsp['__rectype']:
+                        photon_records += rsp,
+                        num_photons += len(rsp['photons'])
+                        if sample_photon_record == None and len(rsp['photons']) > 0:
+                            sample_photon_record = rsp
+                # Build Elevation Columns
+                if num_photons > 0:
+                    # Initialize Columns
+                    for field in sample_photon_record.keys():
+                        fielddef = sliderule.get_definition("bathyrec", field)
+                        if len(fielddef) > 0 and field != "photons":
+                            columns[field] = numpy.empty(num_photons, fielddef["nptype"])
+                    for field in sample_photon_record["photons"][0].keys():
+                        fielddef = sliderule.get_definition("bathyrec.photons", field)
+                        if len(fielddef) > 0:
+                            columns[field] = numpy.empty(num_photons, fielddef["nptype"])
+                    # Populate Columns
+                    ph_cnt = 0
+                    for record in photon_records:
+                        # For Each Photon in Extent
+                        for photon in record["photons"]:
+                            # Add per Extent Fields
+                            for field in record.keys():
+                                if field in columns:
+                                    columns[field][ph_cnt] = record[field]
+                            # Add per Photon Fields
+                            for field in photon.keys():
+                                if field in columns:
+                                    columns[field][ph_cnt] = photon[field]
+                            # Goto Next Photon
+                            ph_cnt += 1
+
+                    # Delete Extent ID Column
+                    if "extent_id" in columns and not keep_id:
+                        del columns["extent_id"]
+
+                    # Capture Time to Flatten
+                    profiles["flatten"] = time.perf_counter() - tstart_flatten
+
+                    # Create DataFrame
+                    gdf = sliderule.todataframe(columns, height_key=height_key)
+
+                    # Calculate Spot Column
+                    gdf['spot'] = gdf.apply(lambda row: __calcspot(row["sc_orient"], row["track"], row["pair"]), axis=1)
+
+                    # Return Response
+                    profiles[atl24gp.__name__] = time.perf_counter() - tstart
+                    return gdf
+                else:
+                    logger.debug("No photons returned")
+            else:
+                logger.debug("No response returned")
+
+    # Handle Runtime Errors
+    except RuntimeError as e:
+        logger.critical(e)
+        if rethrow_exceptions:
+            raise
+
+    # Error Case
+    return sliderule.emptyframe()
```

### Comparing `sliderule-4.3.1/sliderule/io.py` & `sliderule-4.3.2/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/sliderule/ipxapi.py` & `sliderule-4.3.2/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/sliderule/ipysliderule.py` & `sliderule-4.3.2/sliderule/ipysliderule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1487,16 +1487,16 @@
                 # reduce ATL03 data frame to RGT, ground track and cycle
                 atl03 = kwargs['atl03'][(kwargs['atl03']['rgt'] == RGT) &
                     (kwargs['atl03']['track'] == PT) &
                     (kwargs['atl03']['pair'] == LR) &
                     (kwargs['atl03']['cycle'] == cycle)]
             if (kwargs['classification'] == 'atl08'):
                 # noise, ground, canopy, top of canopy, unclassified
-                colormap = np.array(['c','b','g','g','y'])
-                classes = ['noise','ground','canopy','toc','unclassified']
+                colormap = np.array(['c','b','limegreen','g','y'])
+                classes = ['noise','ground','canopy','top of canopy','unclassified']
                 sc = ax.scatter(atl03.index.values, atl03["height"].values,
                     c=colormap[atl03["atl08_class"].values.astype('i')],
                     s=1.5, rasterized=True)
                 for i,lab in enumerate(classes):
                     element = matplotlib.lines.Line2D([0], [0],
                         color=colormap[i], lw=6, label=lab)
                     legend_elements.append(element)
@@ -2688,41 +2688,46 @@
         Parameters
         ----------
         ax : obj, matplotlib axes object
         kind : str, kind of plot to produce
 
             - 'scatter' : scatter plot of along-track heights
             - 'cycles' : time series plot for each orbital cycle
+        data_type: str, GeoDataFrame data format for 'scatter' plot
+
+            - 'atl03' : ATL03 geolocated photons
+            - 'atl06' : ATL06 segment heights
         cmap : str, matplotlib colormap
         title: str, title to use for the plot
         legend: bool, title to use for the plot
         legend_label: str, legend label type for 'cycles' plot
         legend_frameon: bool, use a background patch for legend
         column_name: str, GeoDataFrame column for 'cycles' plot
-        atl03: obj, ATL03 GeoDataFrame for 'scatter' plot
+
         classification: str, ATL03 photon classification for scatter plot
 
             - 'atl03' : ATL03 photon confidence
             - 'atl08' : ATL08 photon-level land classification
             - 'yapc' : Yet Another Photon Classification photon-density
             - 'none' : no classification of photons
+        x_offset: float, offset for along-track distance
         cycle_start: int, beginning cycle for 'cycles' plot
         """
         # default keyword arguments
         kwargs.setdefault('ax', None)
         kwargs.setdefault('kind', 'cycles')
+        kwargs.setdefault('data_type', 'atl06')
         kwargs.setdefault('cmap', 'viridis')
         kwargs.setdefault('title', None)
         kwargs.setdefault('legend', False)
         kwargs.setdefault('legend_label','date')
         kwargs.setdefault('legend_frameon',True)
         kwargs.setdefault('column_name', 'h_mean')
-        kwargs.setdefault('atl03', None)
         kwargs.setdefault('classification', None)
-        kwargs.setdefault('segments', True)
+        kwargs.setdefault('x_offset', 0.0)
         kwargs.setdefault('cycle_start', 3)
         kwargs.setdefault('cycle', 0)
         kwargs.setdefault('RGT', 0)
         kwargs.setdefault('GT', 0)
         # variable to plot
         column = kwargs['column_name']
         RGT = int(kwargs['RGT'])
@@ -2731,128 +2736,148 @@
         if (RGT == 0) or (GT == 0):
             return
         # create figure axis
         if kwargs['ax'] is None:
             fig,ax = plt.subplots(num=1, figsize=(8,6))
             fig.set_facecolor('white')
             fig.canvas.header_visible = False
+            # list of legend elements
+            legend_handles = []
         else:
+            # use existing axis
             ax = kwargs['ax']
-        # list of legend elements
-        legend_elements = []
+            # get existing legend elements
+            try:
+                legend_handles = ax.get_legend().legendHandles
+            except AttributeError:
+                legend_handles = []
+
         # different plot types
         # cycles: along-track plot showing all available cycles
-        # scatter: plot showing a single cycle possibly with ATL03
+        # scatter: plot showing a single cycle
         if (kwargs['kind'] == 'cycles'):
             # for each unique cycles
             for cycle in self._gdf['cycle'].unique():
                 # skip cycles with significant off pointing
                 if (cycle < kwargs['cycle_start']):
                     continue
                 # reduce data frame to RGT, ground track and cycle
-                geodataframe = self._gdf[
+                atl06 = self._gdf[
                     (self._gdf['rgt'] == RGT) &
                     (self._gdf['gt'] == GT) &
                     (self._gdf['cycle'] == cycle)]
-                if not any(geodataframe[column].values):
+                if not any(atl06[column].values):
                     continue
+                # set index to along-track distance
+                atl06['x_atc'] -= kwargs['x_offset']
+                atl06.set_index('x_atc', inplace=True)
                 # plot reduced data frame
-                l, = ax.plot(geodataframe['x_atc'].values,
-                    geodataframe[column].values,
+                l, = ax.plot(atl06.index.values,
+                    atl06[column].values,
                     marker='.', lw=0, ms=1.5)
                 # create legend element for cycle
                 if (kwargs['legend_label'] == 'date'):
-                    label = geodataframe.index[0].strftime('%Y-%m-%d')
+                    label = atl06.index[0].strftime('%Y-%m-%d')
                 elif (kwargs['legend_label'] == 'cycle'):
                     label = f'Cycle {cycle:0.0f}'
-                legend_elements.append(matplotlib.lines.Line2D([0], [0],
-                    color=l.get_color(), lw=6, label=label))
+                # append handle to legend
+                handle = matplotlib.lines.Line2D([0], [0],
+                    color=l.get_color(), lw=6, label=label)
+                legend_handles.append(handle)
             # add axes labels
             ax.set_xlabel('Along-Track Distance [m]')
             ax.set_ylabel(f'SlideRule {column}')
         elif (kwargs['kind'] == 'scatter'):
             # extract orbital cycle parameters
             cycle = int(kwargs['cycle'])
-            if (kwargs['atl03'] == 'dataframe'):
+            if (kwargs['data_type'] == 'atl03'):
                 # reduce entered data frame to RGT, ground track and cycle
                 atl03 = self._gdf[(self._gdf['rgt'] == RGT) &
                     (self._gdf['track'] == self.PT(GT)) &
                     (self._gdf['pair'] == self.LR(GT)) &
                     (self._gdf['cycle'] == cycle)]
-            elif (kwargs['atl03'] is not None):
-                # reduce ATL03 data frame to RGT, ground track and cycle
-                atl03 = kwargs['atl03'][(kwargs['atl03']['rgt'] == RGT) &
-                    (kwargs['atl03']['track'] == self.PT(GT)) &
-                    (kwargs['atl03']['pair'] == self.LR(GT)) &
-                    (kwargs['atl03']['cycle'] == cycle)]
-            if (kwargs['classification'] == 'atl08'):
+                # set index to along-track distance
+                atl03['segment_dist'] += atl03['x_atc']
+                atl03['segment_dist'] -= kwargs['x_offset']
+                atl03.set_index('segment_dist', inplace=True)
+            if (kwargs['data_type'] == 'atl03') and (kwargs['classification'] == 'atl08'):
                 # noise, ground, canopy, top of canopy, unclassified
-                colormap = np.array(['c','b','g','g','y'])
-                classes = ['noise','ground','canopy','toc','unclassified']
+                colormap = np.array(['c','b','limegreen','g','y'])
+                classes = ['noise','ground','canopy','top of canopy','unclassified']
                 sc = ax.scatter(atl03.index.values, atl03["height"].values,
                     c=colormap[atl03["atl08_class"].values.astype('i')],
                     s=1.5, rasterized=True)
+                # append handles to legend
                 for i,lab in enumerate(classes):
-                    element = matplotlib.lines.Line2D([0], [0],
+                    handle = matplotlib.lines.Line2D([0], [0],
                         color=colormap[i], lw=6, label=lab)
-                    legend_elements.append(element)
-            elif (kwargs['classification'] == 'yapc'):
+                    legend_handles.append(handle)
+            elif (kwargs['data_type'] == 'atl03') and (kwargs['classification'] == 'yapc'):
                 sc = ax.scatter(atl03.index.values,
                     atl03["height"].values,
                     c=atl03["yapc_score"],
                     cmap=kwargs['cmap'],
                     s=1.5, rasterized=True)
                 plt.colorbar(sc)
-            elif (kwargs['classification'] == 'atl03'):
+            elif (kwargs['data_type'] == 'atl03') and (kwargs['classification'] == 'atl03'):
                 # background, buffer, low, medium, high
                 colormap = np.array(['y','c','b','g','m'])
                 confidences = ['background','buffer','low','medium','high']
                 # reduce data frame to photon classified for surface
                 atl03 = atl03[atl03["atl03_cnf"] >= 0]
                 sc = ax.scatter(atl03.index.values, atl03["height"].values,
                     c=colormap[atl03["atl03_cnf"].values.astype('i')],
                     s=1.5, rasterized=True)
+                # append handles to legend
                 for i,lab in enumerate(confidences):
-                    element = matplotlib.lines.Line2D([0], [0],
+                    handle = matplotlib.lines.Line2D([0], [0],
                         color=colormap[i], lw=6, label=lab)
-                    legend_elements.append(element)
-            elif (kwargs['atl03'] is not None):
+                    legend_handles.append(handle)
+            elif (kwargs['data_type'] == 'atl03'):
                 # plot all available ATL03 points as gray
                 sc = ax.scatter(atl03.index.values, atl03["height"].values,
                     c='0.4', s=0.5, rasterized=True)
-                legend_elements.append(matplotlib.lines.Line2D([0], [0],
-                    color='0.4', lw=6, label='ATL03'))
-            if kwargs['segments']:
-                geodataframe = self._gdf[
+                # append handle to legend
+                handle = matplotlib.lines.Line2D([0], [0],
+                    color='0.4', lw=6, label='ATL03')
+                legend_handles.append(handle)
+            # plot ATL06-SR segments for cycle and track
+            if (kwargs['data_type'] == 'atl06'):
+                atl06 = self._gdf[
                     (self._gdf['rgt'] == RGT) &
                     (self._gdf['gt'] == GT) &
                     (self._gdf['cycle'] == cycle)]
+                # set index to along-track distance
+                atl06['x_atc'] -= kwargs['x_offset']
+                atl06.set_index('x_atc', inplace=True)
                 # plot reduced data frame
-                sc = ax.scatter(geodataframe.index.values,
-                    geodataframe["h_mean"].values,
+                sc = ax.scatter(atl06.index.values,
+                    atl06["h_mean"].values,
                     c='red', s=2.5, rasterized=True)
-                legend_elements.append(matplotlib.lines.Line2D([0], [0],
-                    color='red', lw=6, label='ATL06-SR'))
+                handle = matplotlib.lines.Line2D([0], [0],
+                    color='red', lw=6, label='ATL06-SR')
+                legend_handles.append(handle)
             # add axes labels
-            ax.set_xlabel('UTC')
+            ax.set_xlabel('Along-Track Distance [m]')
             ax.set_ylabel('Height (m)')
         # add title
         if kwargs['title']:
             ax.set_title(kwargs['title'])
         # create legend
         if kwargs['legend']:
-            lgd = ax.legend(handles=legend_elements, loc=3,
+            lgd = ax.legend(handles=legend_handles, loc=3,
                 frameon=kwargs['legend_frameon'])
         # set legend frame to solid white
         if kwargs['legend'] and kwargs['legend_frameon']:
             lgd.get_frame().set_alpha(1.0)
             lgd.get_frame().set_edgecolor('white')
         if kwargs['ax'] is None:
             # show the figure
             plt.tight_layout()
+            plt.draw()
 
     def ground_track(self, GT):
         """extract the ground track name for a given Ground Track (GT) index
         """
         ground_track_list = ['gt1l', 'gt1r', 'gt2l', 'gt2r', 'gt3l', 'gt3r']
         return ground_track_list[GT//10 - 1]
```

### Comparing `sliderule-4.3.1/sliderule/raster.py` & `sliderule-4.3.2/sliderule/raster.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/sliderule/sliderule.py` & `sliderule-4.3.2/sliderule/sliderule.py`

 * *Files 1% similar despite different names*

```diff
@@ -553,20 +553,26 @@
     # Check If Remote Record Is In Responses
     for rsp in rsps:
         if 'arrowrec.remote' == rsp['__rectype']:
             path = rsp['url']
             break
     # Handle Local Files
     if "open_on_complete" in output and output["open_on_complete"]:
-        if "as_geo" in output and not output["as_geo"]:
-            # Return Parquet File as DataFrame
-            return geopandas.pd.read_parquet(path)
+        if output["format"] == "parquet":
+            if "as_geo" in output and not output["as_geo"]:
+                # Return Parquet File as DataFrame
+                return geopandas.pd.read_parquet(path)
+            else:
+                # Return GeoParquet File as GeoDataFrame
+                return geopandas.read_parquet(path)
+        elif output["format"] == "csv":
+            # Return CSV File as DataFrame
+            return geopandas.pd.read_csv(path)
         else:
-            # Return GeoParquet File as GeoDataFrame
-            return geopandas.read_parquet(path)
+            raise FatalError('unsupported output format: %s' % (output["format"]))
     else:
         # Return Parquet Filename
         return path
 
 #
 #  Get Values from Raw Buffer
 #
```

### Comparing `sliderule-4.3.1/sliderule/swot.py` & `sliderule-4.3.2/sliderule/swot.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/sliderule.egg-info/PKG-INFO` & `sliderule-4.3.2/sliderule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 4.3.1
+Version: 4.3.2
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-4.3.1/sliderule.egg-info/SOURCES.txt` & `sliderule-4.3.2/sliderule.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 version.txt
 sliderule/__init__.py
+sliderule/bathy.py
 sliderule/container.py
 sliderule/earthdata.py
 sliderule/gedi.py
 sliderule/h5.py
 sliderule/icesat2.py
 sliderule/io.py
 sliderule/ipxapi.py
@@ -18,20 +19,22 @@
 sliderule/swot.py
 sliderule/version.py
 sliderule.egg-info/PKG-INFO
 sliderule.egg-info/SOURCES.txt
 sliderule.egg-info/dependency_links.txt
 sliderule.egg-info/requires.txt
 sliderule.egg-info/top_level.txt
+utils/bathy_runner.py
 utils/benchmark.py
 utils/big_query.py
 utils/build_3dep_DEM_geojson.py
 utils/build_arctic_dem_mosaics_index.py
 utils/build_arctic_dem_mosaics_vrt_list.py
 utils/build_arctic_dem_strips_vrt.py
+utils/container_runner.py
 utils/create_geojson.py
 utils/extract_h5_dataset.py
 utils/icepyx_region.py
 utils/lpdaac_download.py
 utils/lpdaac_list.py
 utils/monitor.py
 utils/opendata_worldcover.py
@@ -42,9 +45,8 @@
 utils/query_stac.py
 utils/query_version.py
 utils/region_of_interest.py
 utils/results_to_s3.py
 utils/stac.py
 utils/stream_events.py
 utils/tail_events.py
-utils/test.py
 utils/utils.py
```

### Comparing `sliderule-4.3.1/utils/benchmark.py` & `sliderule-4.3.2/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/big_query.py` & `sliderule-4.3.2/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/build_3dep_DEM_geojson.py` & `sliderule-4.3.2/utils/build_3dep_DEM_geojson.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/build_arctic_dem_mosaics_index.py` & `sliderule-4.3.2/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-4.3.2/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/build_arctic_dem_strips_vrt.py` & `sliderule-4.3.2/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/create_geojson.py` & `sliderule-4.3.2/utils/create_geojson.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/extract_h5_dataset.py` & `sliderule-4.3.2/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/icepyx_region.py` & `sliderule-4.3.2/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/lpdaac_download.py` & `sliderule-4.3.2/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/monitor.py` & `sliderule-4.3.2/utils/monitor.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/opendata_worldcover.py` & `sliderule-4.3.2/utils/opendata_worldcover.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/query_cmr.py` & `sliderule-4.3.2/utils/query_cmr.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/query_elevations.py` & `sliderule-4.3.2/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/query_metrics.py` & `sliderule-4.3.2/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/query_photons.py` & `sliderule-4.3.2/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/query_stac.py` & `sliderule-4.3.2/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/query_version.py` & `sliderule-4.3.2/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/region_of_interest.py` & `sliderule-4.3.2/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/results_to_s3.py` & `sliderule-4.3.2/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/stac.py` & `sliderule-4.3.2/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/stream_events.py` & `sliderule-4.3.2/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/tail_events.py` & `sliderule-4.3.2/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-4.3.1/utils/utils.py` & `sliderule-4.3.2/utils/utils.py`

 * *Files identical despite different names*

