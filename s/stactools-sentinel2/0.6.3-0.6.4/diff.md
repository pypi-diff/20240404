# Comparing `tmp/stactools-sentinel2-0.6.3.tar.gz` & `tmp/stactools-sentinel2-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-sentinel2-0.6.3.tar", last modified: Thu Feb  1 13:49:15 2024, max compression
+gzip compressed data, was "stactools-sentinel2-0.6.4.tar", last modified: Thu Apr  4 16:36:27 2024, max compression
```

## Comparing `stactools-sentinel2-0.6.3.tar` & `stactools-sentinel2-0.6.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:49:15.223528 stactools-sentinel2-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-01 13:49:15.223528 stactools-sentinel2-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-01 13:49:15.223528 stactools-sentinel2-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:49:15.219528 stactools-sentinel2-0.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:49:15.219528 stactools-sentinel2-0.6.3/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:49:15.219528 stactools-sentinel2-0.6.3/src/stactools/sentinel2/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/cog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/granule_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/mgrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/product_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/safe_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    24682 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/tileinfo_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/src/stactools/sentinel2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:49:15.223528 stactools-sentinel2-0.6.3/src/stactools_sentinel2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-01 13:49:15.000000 stactools-sentinel2-0.6.3/src/stactools_sentinel2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-01 13:49:15.000000 stactools-sentinel2-0.6.3/src/stactools_sentinel2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 13:49:15.000000 stactools-sentinel2-0.6.3/src/stactools_sentinel2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-01 13:49:15.000000 stactools-sentinel2-0.6.3/src/stactools_sentinel2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-01 13:49:15.000000 stactools-sentinel2-0.6.3/src/stactools_sentinel2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 13:49:15.223528 stactools-sentinel2-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-02-01 13:49:06.000000 stactools-sentinel2-0.6.3/tests/test_stac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:36:27.736215 stactools-sentinel2-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-04 16:36:27.736215 stactools-sentinel2-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-04 16:36:27.736215 stactools-sentinel2-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:36:27.728215 stactools-sentinel2-0.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:36:27.728215 stactools-sentinel2-0.6.4/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:36:27.732215 stactools-sentinel2-0.6.4/src/stactools/sentinel2/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/cog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/granule_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/mgrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/product_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/safe_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25195 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/tileinfo_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/src/stactools/sentinel2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:36:27.736215 stactools-sentinel2-0.6.4/src/stactools_sentinel2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-04 16:36:27.000000 stactools-sentinel2-0.6.4/src/stactools_sentinel2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 16:36:27.000000 stactools-sentinel2-0.6.4/src/stactools_sentinel2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:36:27.000000 stactools-sentinel2-0.6.4/src/stactools_sentinel2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-04 16:36:27.000000 stactools-sentinel2-0.6.4/src/stactools_sentinel2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 16:36:27.000000 stactools-sentinel2-0.6.4/src/stactools_sentinel2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:36:27.736215 stactools-sentinel2-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-04 16:36:17.000000 stactools-sentinel2-0.6.4/tests/test_stac.py
```

### Comparing `stactools-sentinel2-0.6.3/LICENSE` & `stactools-sentinel2-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/PKG-INFO` & `stactools-sentinel2-0.6.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel2
-Version: 0.6.3
+Version: 0.6.4
 Summary: Create STAC Items from Sentinel-2 metadata
 Home-page: https://github.com/stactools-sentinel2/stactools-sentinel2
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Issues, https://github.com/stactools-sentinel2s/stactools-sentinel2/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
@@ -21,16 +21,16 @@
 
 # stactools-sentinel2
 
 stactools package for Sentinel-2 data.
 
 ## Examples
 
-- [L1C item](./examples/sentinel2-l1c-example/S2A_MSIL1C_20200717T221941_R029_T01LAC_20200717T234135/S2A_MSIL1C_20200717T221941_R029_T01LAC_20200717T234135.json)
-- [L2A item](./examples/sentinel2-l2a-example/S2A_MSIL2A_20190212T192651_R013_T07HFE_20201007T160857/S2A_MSIL2A_20190212T192651_R013_T07HFE_20201007T160857.json)
+- [L1C item](./examples/sentinel2-l1c-example/S2A_T01LAC_20200717T221944_L1C/S2A_T01LAC_20200717T221944_L1C.json)
+- [L2A item](./examples/sentinel2-l2a-example/S2A_T07HFE_20190212T192646_L2A/S2A_T07HFE_20190212T192646_L2A.json)
 
 ## Running
 
 ```shell
 pip install stactools-sentinel2
 ````
```

### Comparing `stactools-sentinel2-0.6.3/README.md` & `stactools-sentinel2-0.6.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stactools-sentinel2
 
 stactools package for Sentinel-2 data.
 
 ## Examples
 
-- [L1C item](./examples/sentinel2-l1c-example/S2A_MSIL1C_20200717T221941_R029_T01LAC_20200717T234135/S2A_MSIL1C_20200717T221941_R029_T01LAC_20200717T234135.json)
-- [L2A item](./examples/sentinel2-l2a-example/S2A_MSIL2A_20190212T192651_R013_T07HFE_20201007T160857/S2A_MSIL2A_20190212T192651_R013_T07HFE_20201007T160857.json)
+- [L1C item](./examples/sentinel2-l1c-example/S2A_T01LAC_20200717T221944_L1C/S2A_T01LAC_20200717T221944_L1C.json)
+- [L2A item](./examples/sentinel2-l2a-example/S2A_T07HFE_20190212T192646_L2A/S2A_T07HFE_20190212T192646_L2A.json)
 
 ## Running
 
 ```shell
 pip install stactools-sentinel2
 ````
```

### Comparing `stactools-sentinel2-0.6.3/setup.cfg` & `stactools-sentinel2-0.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/cog.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/cog.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/commands.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/commands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/constants.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/constants.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/granule_metadata.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/granule_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/mgrs.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/mgrs.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/product_metadata.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/product_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/safe_manifest.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/safe_manifest.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/stac.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/stac.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,20 +374,39 @@
         # True color
         asset = pystac.Asset(
             href=asset_href,
             media_type=asset_media_type,
             title="True color image",
             roles=["visual"],
         )
-        asset_eo = EOExtension.ext(asset)
-        asset_eo.bands = RGB_BANDS
+
+        EOExtension.ext(asset).bands = RGB_BANDS
+
+        RasterExtension.ext(asset).bands = [
+            RasterBand.create(
+                nodata=0,
+                spatial_resolution=resolution,
+                data_type=DataType.UINT8,
+            ),
+            RasterBand.create(
+                nodata=0,
+                spatial_resolution=resolution,
+                data_type=DataType.UINT8,
+            ),
+            RasterBand.create(
+                nodata=0,
+                spatial_resolution=resolution,
+                data_type=DataType.UINT8,
+            ),
+        ]
 
         maybe_res = extract_gsd(asset_href)
         asset_id = f"visual_{maybe_res}m" if maybe_res and maybe_res != 10 else "visual"
         set_asset_properties(asset, maybe_res)
+
     elif AOT_PATTERN.search(asset_href):
         # Aerosol
         asset = pystac.Asset(
             href=asset_href,
             media_type=asset_media_type,
             title="Aerosol optical thickness (AOT)",
             roles=["data"],
```

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/tileinfo_metadata.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/tileinfo_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools/sentinel2/utils.py` & `stactools-sentinel2-0.6.4/src/stactools/sentinel2/utils.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/src/stactools_sentinel2.egg-info/PKG-INFO` & `stactools-sentinel2-0.6.4/src/stactools_sentinel2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-sentinel2
-Version: 0.6.3
+Version: 0.6.4
 Summary: Create STAC Items from Sentinel-2 metadata
 Home-page: https://github.com/stactools-sentinel2/stactools-sentinel2
 Author: stac-utils
 Author-email: stac@radiant.earth
 Project-URL: Issues, https://github.com/stactools-sentinel2s/stactools-sentinel2/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
@@ -21,16 +21,16 @@
 
 # stactools-sentinel2
 
 stactools package for Sentinel-2 data.
 
 ## Examples
 
-- [L1C item](./examples/sentinel2-l1c-example/S2A_MSIL1C_20200717T221941_R029_T01LAC_20200717T234135/S2A_MSIL1C_20200717T221941_R029_T01LAC_20200717T234135.json)
-- [L2A item](./examples/sentinel2-l2a-example/S2A_MSIL2A_20190212T192651_R013_T07HFE_20201007T160857/S2A_MSIL2A_20190212T192651_R013_T07HFE_20201007T160857.json)
+- [L1C item](./examples/sentinel2-l1c-example/S2A_T01LAC_20200717T221944_L1C/S2A_T01LAC_20200717T221944_L1C.json)
+- [L2A item](./examples/sentinel2-l2a-example/S2A_T07HFE_20190212T192646_L2A/S2A_T07HFE_20190212T192646_L2A.json)
 
 ## Running
 
 ```shell
 pip install stactools-sentinel2
 ````
```

### Comparing `stactools-sentinel2-0.6.3/src/stactools_sentinel2.egg-info/SOURCES.txt` & `stactools-sentinel2-0.6.4/src/stactools_sentinel2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/tests/test_commands.py` & `stactools-sentinel2-0.6.4/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/tests/test_metadata.py` & `stactools-sentinel2-0.6.4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `stactools-sentinel2-0.6.3/tests/test_stac.py` & `stactools-sentinel2-0.6.4/tests/test_stac.py`

 * *Files identical despite different names*

