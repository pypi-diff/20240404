# Comparing `tmp/datagov_harvesting_logic-0.3.5.tar.gz` & `tmp/datagov_harvesting_logic-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datagov_harvesting_logic-0.3.5.tar", max compression
+gzip compressed data, was "datagov_harvesting_logic-0.3.6.tar", max compression
```

## Comparing `datagov_harvesting_logic-0.3.5.tar` & `datagov_harvesting_logic-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1878 2024-03-21 18:58:28.123889 datagov_harvesting_logic-0.3.5/LICENSE.md
--rw-r--r--   0        0        0     5031 2024-03-21 18:58:28.123889 datagov_harvesting_logic-0.3.5/README.md
--rw-r--r--   0        0        0      162 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/__init__.py
--rw-r--r--   0        0        0     4489 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/ckan_utils.py
--rw-r--r--   0        0        0     4464 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/arm.data.json
--rw-r--r--   0        0        0     7830 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
--rw-r--r--   0        0        0    14027 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
--rw-r--r--   0        0        0     7454 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/geospatial.data.json
--rw-r--r--   0        0        0   310979 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/large-spatial.data.json
--rw-r--r--   0        0        0      918 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/missing-catalog.data.json
--rw-r--r--   0        0        0     1059 2024-03-21 18:58:28.127889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
--rw-r--r--   0        0        0     3259 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/missing-identifier-title.data.json
--rw-r--r--   0        0        0     1292 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/numerical-title.data.json
--rw-r--r--   0        0        0     2520 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/ny.data.json
--rw-r--r--   0        0        0     1314 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/reserved-title.data.json
--rw-r--r--   0        0        0     9562 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/usda.gov.data.json
--rw-r--r--   0        0        0     1604 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/schemas/catalog.json
--rw-r--r--   0        0        0    23811 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/data/dcatus/schemas/dataset.json
--rw-r--r--   0        0        0     2200 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/exceptions.py
--rw-r--r--   0        0        0    25444 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/harvest.py
--rw-r--r--   0        0        0      589 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/logger_config.py
--rw-r--r--   0        0        0     2238 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/harvester/utils.py
--rw-r--r--   0        0        0     2180 2024-03-21 18:58:28.131889 datagov_harvesting_logic-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6243 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1878 2024-04-03 22:04:24.163847 datagov_harvesting_logic-0.3.6/LICENSE.md
+-rw-r--r--   0        0        0     5031 2024-04-03 22:04:24.163847 datagov_harvesting_logic-0.3.6/README.md
+-rw-r--r--   0        0        0      162 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/__init__.py
+-rw-r--r--   0        0        0     4489 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/ckan_utils.py
+-rw-r--r--   0        0        0     4464 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/arm.data.json
+-rw-r--r--   0        0        0     7830 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json
+-rw-r--r--   0        0        0    14027 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json
+-rw-r--r--   0        0        0     7454 2024-04-03 22:04:24.167847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/geospatial.data.json
+-rw-r--r--   0        0        0   310979 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/large-spatial.data.json
+-rw-r--r--   0        0        0      918 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-catalog.data.json
+-rw-r--r--   0        0        0     1059 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-dataset-fields.data.json
+-rw-r--r--   0        0        0     3259 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-identifier-title.data.json
+-rw-r--r--   0        0        0     1292 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/numerical-title.data.json
+-rw-r--r--   0        0        0     2520 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/ny.data.json
+-rw-r--r--   0        0        0     1314 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/reserved-title.data.json
+-rw-r--r--   0        0        0     9562 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/usda.gov.data.json
+-rw-r--r--   0        0        0     1604 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/schemas/catalog.json
+-rw-r--r--   0        0        0    23811 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/data/dcatus/schemas/dataset.json
+-rw-r--r--   0        0        0     2200 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/exceptions.py
+-rw-r--r--   0        0        0    25444 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/harvest.py
+-rw-r--r--   0        0        0      589 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/logger_config.py
+-rw-r--r--   0        0        0     3632 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/harvester/utils.py
+-rw-r--r--   0        0        0     2212 2024-04-03 22:04:24.171847 datagov_harvesting_logic-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6296 1970-01-01 00:00:00.000000 datagov_harvesting_logic-0.3.6/PKG-INFO
```

### Comparing `datagov_harvesting_logic-0.3.5/LICENSE.md` & `datagov_harvesting_logic-0.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/README.md` & `datagov_harvesting_logic-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/ckan_utils.py` & `datagov_harvesting_logic-0.3.6/harvester/ckan_utils.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/arm.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/arm.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/collection-1-parent-2-children.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/collection-2-parent-4-children.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/geospatial.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/geospatial.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/large-spatial.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/large-spatial.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/missing-catalog.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-catalog.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/missing-dataset-fields.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-dataset-fields.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/missing-identifier-title.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/missing-identifier-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/numerical-title.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/numerical-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/ny.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/ny.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/reserved-title.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/reserved-title.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/jsons/usda.gov.data.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/jsons/usda.gov.data.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/schemas/catalog.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/schemas/catalog.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/data/dcatus/schemas/dataset.json` & `datagov_harvesting_logic-0.3.6/harvester/data/dcatus/schemas/dataset.json`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/exceptions.py` & `datagov_harvesting_logic-0.3.6/harvester/exceptions.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/harvest.py` & `datagov_harvesting_logic-0.3.6/harvester/harvest.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/harvester/logger_config.py` & `datagov_harvesting_logic-0.3.6/harvester/logger_config.py`

 * *Files identical despite different names*

### Comparing `datagov_harvesting_logic-0.3.5/pyproject.toml` & `datagov_harvesting_logic-0.3.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datagov-harvesting-logic"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 # authors = [
 #     {name = "Jin Sun", email = "jin.sun@gsa.gov"},
 #     {name = "Tyler Burton", email = "tyler.burton@gsa.gov"},
 # ]
 authors = [
     "Datagov Team <datagov@gsa.gov>",
@@ -29,14 +29,15 @@
 boto3 = "^1.34.29"
 sqlalchemy = "^2.0.25"
 flask = "^3.0.2"
 psycopg2-binary = "^2.9.9"
 flask-sqlalchemy = "^3.1.1"
 flask-wtf = "^1.2.1"
 flask-migrate = "^4.0.7"
+cloudfoundry-client = "^1.36.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 ruff = "^0.0.261"
 pytest-cov = "^4.0.0"
 
 [tool.ruff]
```

### Comparing `datagov_harvesting_logic-0.3.5/PKG-INFO` & `datagov_harvesting_logic-0.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datagov-harvesting-logic
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Home-page: https://github.com/GSA/datagov-harvesting-logic
 License: LICENSE.md
 Author: Datagov Team
 Author-email: datagov@gsa.gov
 Maintainer: Datagov Team
 Maintainer-email: datagov@gsa.gov
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: boto3 (>=1.34.29,<2.0.0)
 Requires-Dist: ckanapi (>=4.7)
+Requires-Dist: cloudfoundry-client (>=1.36.0,<2.0.0)
 Requires-Dist: deepdiff (>=6)
 Requires-Dist: flask (>=3.0.2,<4.0.0)
 Requires-Dist: flask-migrate (>=4.0.7,<5.0.0)
 Requires-Dist: flask-sqlalchemy (>=3.1.1,<4.0.0)
 Requires-Dist: flask-wtf (>=1.2.1,<2.0.0)
 Requires-Dist: jsonschema (>=4)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
```

