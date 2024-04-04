# Comparing `tmp/eodc-2024.2.6.tar.gz` & `tmp/eodc-2024.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2024.2.6.tar", max compression
+gzip compressed data, was "eodc-2024.3.1.tar", max compression
```

## Comparing `eodc-2024.2.6.tar` & `eodc-2024.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      513 2024-02-23 13:17:58.151390 eodc-2024.2.6/README.md
--rw-r--r--   0        0        0      195 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/__init__.py
--rw-r--r--   0        0        0     1794 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/auth.py
--rw-r--r--   0        0        0     1311 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/dask.py
--rw-r--r--   0        0        0    13711 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/faas.py
--rw-r--r--   0        0        0     1183 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/settings.py
--rw-r--r--   0        0        0     2240 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/storage.py
--rw-r--r--   0        0        0        0 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/visualisation/vessel_detection/__init__.py
--rwxr-xr-x   0        0        0    15080 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/visualisation/vessel_detection/app.py
--rw-r--r--   0        0        0      261 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/visualisation/vessel_detection/assets/app.css
--rw-r--r--   0        0        0     2539 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/visualisation/vessel_detection/cards.py
--rw-r--r--   0        0        0     8522 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/visualisation/vessel_detection/navbar.py
--rw-r--r--   0        0        0     2867 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/visualisation/vessel_detection/utils.py
--rw-r--r--   0        0        0    19104 2024-02-23 13:17:58.151390 eodc-2024.2.6/eodc/workspace.py
--rw-r--r--   0        0        0     1725 2024-02-23 13:17:58.155390 eodc-2024.2.6/pyproject.toml
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 eodc-2024.2.6/PKG-INFO
+-rw-r--r--   0        0        0      513 2024-04-04 11:59:07.217675 eodc-2024.3.1/README.md
+-rw-r--r--   0        0        0      195 2024-04-04 11:59:07.217675 eodc-2024.3.1/eodc/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-04 11:59:07.217675 eodc-2024.3.1/eodc/auth.py
+-rw-r--r--   0        0        0     1311 2024-04-04 11:59:07.217675 eodc-2024.3.1/eodc/dask.py
+-rw-r--r--   0        0        0    13711 2024-04-04 11:59:07.217675 eodc-2024.3.1/eodc/faas.py
+-rw-r--r--   0        0        0     1183 2024-04-04 11:59:07.217675 eodc-2024.3.1/eodc/settings.py
+-rw-r--r--   0        0        0     2240 2024-04-04 11:59:07.217675 eodc-2024.3.1/eodc/storage.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:07.217675 eodc-2024.3.1/eodc/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 11:59:07.217675 eodc-2024.3.1/eodc/visualisation/vessel_detection/__init__.py
+-rwxr-xr-x   0        0        0    15080 2024-04-04 11:59:07.221675 eodc-2024.3.1/eodc/visualisation/vessel_detection/app.py
+-rw-r--r--   0        0        0      261 2024-04-04 11:59:07.221675 eodc-2024.3.1/eodc/visualisation/vessel_detection/assets/app.css
+-rw-r--r--   0        0        0     2539 2024-04-04 11:59:07.221675 eodc-2024.3.1/eodc/visualisation/vessel_detection/cards.py
+-rw-r--r--   0        0        0     8522 2024-04-04 11:59:07.221675 eodc-2024.3.1/eodc/visualisation/vessel_detection/navbar.py
+-rw-r--r--   0        0        0     2867 2024-04-04 11:59:07.221675 eodc-2024.3.1/eodc/visualisation/vessel_detection/utils.py
+-rw-r--r--   0        0        0    28244 2024-04-04 11:59:07.221675 eodc-2024.3.1/eodc/workspace.py
+-rw-r--r--   0        0        0     1913 2024-04-04 11:59:07.221675 eodc-2024.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 eodc-2024.3.1/PKG-INFO
```

### Comparing `eodc-2024.2.6/README.md` & `eodc-2024.3.1/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/auth.py` & `eodc-2024.3.1/eodc/auth.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/dask.py` & `eodc-2024.3.1/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/faas.py` & `eodc-2024.3.1/eodc/faas.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/settings.py` & `eodc-2024.3.1/eodc/settings.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/storage.py` & `eodc-2024.3.1/eodc/storage.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/visualisation/vessel_detection/app.py` & `eodc-2024.3.1/eodc/visualisation/vessel_detection/app.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/visualisation/vessel_detection/cards.py` & `eodc-2024.3.1/eodc/visualisation/vessel_detection/cards.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/visualisation/vessel_detection/navbar.py` & `eodc-2024.3.1/eodc/visualisation/vessel_detection/navbar.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/eodc/visualisation/vessel_detection/utils.py` & `eodc-2024.3.1/eodc/visualisation/vessel_detection/utils.py`

 * *Files identical despite different names*

### Comparing `eodc-2024.2.6/pyproject.toml` & `eodc-2024.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "eodc"
 
-version = "2024.2.6"
+version = "2024.3.1"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>", "Christoph Reimer <christoph.reimer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -45,17 +45,24 @@
 dash-bootstrap-components="1.5.0"
 dash_daq="0.5.0"
 dash-extensions="1.0.11"
 jsbeautifier="1.14.11"
 OWSLib = "^0.29.3"
 geopandas = "0.14.3"
 httpx = "^0.27.0"
+boto3 = "^1.34.56"
+pystac-client = "^0.7.6"
+odc-stac = ">=0.3.3,<1"
+rasterio = {extras = ["session"], version = "*"}
+datacube = "*"
+openeo-pg-parser-networkx = "2024.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ipykernel = "^6.22.0"
+matplotlib = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eodc-2024.2.6/PKG-INFO` & `eodc-2024.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2024.2.6
+Version: 2024.3.1
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
@@ -15,37 +15,43 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: OWSLib (>=0.29.3,<0.30.0)
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.18.3,<13.0.0)
+Requires-Dist: boto3 (>=1.34.56,<2.0.0)
 Requires-Dist: dash (==2.15.0)
 Requires-Dist: dash-bootstrap-components (==1.5.0)
 Requires-Dist: dash-extensions (==1.0.11)
 Requires-Dist: dash_daq (==0.5.0)
 Requires-Dist: dash_leaflet (==1.0.15)
 Requires-Dist: dask-gateway (>=2023.1.1)
+Requires-Dist: datacube
 Requires-Dist: eodc-faas-force (>=2023.7.1)
 Requires-Dist: eodc-faas-openeo (>=2023.6.8)
 Requires-Dist: eodc-faas-sen2like (>=2023.6.2)
 Requires-Dist: eodc-faas-snap (>=2023.6.2)
 Requires-Dist: eodc-faas-vessel-detection (>=2023.11.4)
 Requires-Dist: geopandas (==0.14.3)
 Requires-Dist: hera (>=5.5.2,<5.10)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: jsbeautifier (==1.14.11)
 Requires-Dist: minio (==7.1.16)
 Requires-Dist: nbformat (>4.2.0)
+Requires-Dist: odc-stac (>=0.3.3,<1)
 Requires-Dist: openeo (>=0.13.0,<1)
+Requires-Dist: openeo-pg-parser-networkx (==2024.1.1)
 Requires-Dist: plotly (>=5.18.0,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyjwt[crypto] (>=2.8.0,<3.0.0)
 Requires-Dist: pyproj (>=3.6.0,<4.0.0)
 Requires-Dist: pystac (>=1.7.3,<2.0.0)
+Requires-Dist: pystac-client (>=0.7.6,<0.8.0)
+Requires-Dist: rasterio[session]
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/eodcgmbh/eodc-sdk
 Description-Content-Type: text/markdown
 
 # EODC SDK
 ![PyPI - Status](https://img.shields.io/pypi/status/eodc)
 ![PyPI](https://img.shields.io/pypi/v/eodc)
```

