# Comparing `tmp/foursight_smaht-0.8.5.tar.gz` & `tmp/foursight_smaht-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_smaht-0.8.5.tar", max compression
+gzip compressed data, was "foursight_smaht-0.8.6.tar", max compression
```

## Comparing `foursight_smaht-0.8.5.tar` & `foursight_smaht-0.8.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/LICENSE.txt
--rw-r--r--   0        0        0        0 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/app_utils.py
--rw-r--r--   0        0        0      873 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/buckets.py
--rw-r--r--   0        0        0     4960 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/check_schedules.py
--rw-r--r--   0        0        0    14108 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/check_setup.json
--rw-r--r--   0        0        0     6530 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/check_setup.json-local
--rw-r--r--   0        0        0    13660 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/check_setup.json-smaht-wolf
--rw-r--r--   0        0        0      249 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/__init__.py
--rw-r--r--   0        0        0     5682 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/audit_checks.py
--rw-r--r--   0        0        0     2883 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/es_checks.py
--rw-r--r--   0        0        0      262 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/constants.py
--rw-r--r--   0        0        0    12321 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     3993 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/utils.py
--rw-r--r--   0        0        0     1598 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2572 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    22420 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/system_checks.py
--rw-r--r--   0        0        0    34795 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/wfr_checks.py
--rw-r--r--   0        0        0     2595 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/checks/wrangler_checks.py
--rw-r--r--   0        0        0      773 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/deploy.py
--rw-r--r--   0        0        0      131 2024-04-03 18:41:58.990258 foursight_smaht-0.8.5/chalicelib_smaht/gitinfo.json
--rw-r--r--   0        0        0      601 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/package.py
--rw-r--r--   0        0        0      323 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/scripts/local_check_execution.py
--rw-r--r--   0        0        0      253 2024-04-03 18:41:45.514211 foursight_smaht-0.8.5/chalicelib_smaht/vars.py
--rw-r--r--   0        0        0     1566 2024-04-03 18:41:45.518211 foursight_smaht-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 foursight_smaht-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/LICENSE.txt
+-rw-r--r--   0        0        0        0 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/app_utils.py
+-rw-r--r--   0        0        0      873 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/buckets.py
+-rw-r--r--   0        0        0     4960 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/check_schedules.py
+-rw-r--r--   0        0        0    14108 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/check_setup.json
+-rw-r--r--   0        0        0     6530 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/check_setup.json-local
+-rw-r--r--   0        0        0    13660 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/check_setup.json-smaht-wolf
+-rw-r--r--   0        0        0      249 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/__init__.py
+-rw-r--r--   0        0        0     5682 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/audit_checks.py
+-rw-r--r--   0        0        0     2883 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/es_checks.py
+-rw-r--r--   0        0        0      262 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/constants.py
+-rw-r--r--   0        0        0    12321 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     3993 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/utils.py
+-rw-r--r--   0        0        0     1598 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2572 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    22420 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/system_checks.py
+-rw-r--r--   0        0        0    34795 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/wfr_checks.py
+-rw-r--r--   0        0        0     2595 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      773 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/deploy.py
+-rw-r--r--   0        0        0      131 2024-04-04 17:07:46.096125 foursight_smaht-0.8.6/chalicelib_smaht/gitinfo.json
+-rw-r--r--   0        0        0      601 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/package.py
+-rw-r--r--   0        0        0      323 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/scripts/local_check_execution.py
+-rw-r--r--   0        0        0      253 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/chalicelib_smaht/vars.py
+-rw-r--r--   0        0        0     1566 2024-04-04 17:07:35.356135 foursight_smaht-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 foursight_smaht-0.8.6/PKG-INFO
```

### Comparing `foursight_smaht-0.8.5/LICENSE.txt` & `foursight_smaht-0.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/app_utils.py` & `foursight_smaht-0.8.6/chalicelib_smaht/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/buckets.py` & `foursight_smaht-0.8.6/chalicelib_smaht/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/check_schedules.py` & `foursight_smaht-0.8.6/chalicelib_smaht/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/check_setup.json` & `foursight_smaht-0.8.6/chalicelib_smaht/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/check_setup.json-local` & `foursight_smaht-0.8.6/chalicelib_smaht/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/check_setup.json-smaht-wolf` & `foursight_smaht-0.8.6/chalicelib_smaht/check_setup.json-smaht-wolf`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/audit_checks.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/ecs_checks.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/es_checks.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/lifecycle_utils.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/linecount_dicts.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/utils.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/wfr_utils.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/helpers/wfrset_utils.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/lifecycle_checks.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/system_checks.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/wfr_checks.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/checks/wrangler_checks.py` & `foursight_smaht-0.8.6/chalicelib_smaht/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/deploy.py` & `foursight_smaht-0.8.6/chalicelib_smaht/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/chalicelib_smaht/package.py` & `foursight_smaht-0.8.6/chalicelib_smaht/package.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.5/pyproject.toml` & `foursight_smaht-0.8.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-smaht"
-version = "0.8.5"
+version = "0.8.6"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_smaht" }
 ]
 
@@ -21,15 +21,15 @@
 # Error: "The client noticed that the server is not Elasticsearch and we do not support this unknown product"
 # https://stackoverflow.com/questions/68802324/elasticsearch-in-go-err-the-client-noticed-that-the-server-is-not-elasticsear
 elasticsearch = "7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 packaging = "^23.0"
-magma-suite = "^3.1.0"
+magma-suite = "^3.2.1"
 tibanna-ff = "^3.2.0"
 MarkupSafe = "^2.1.3"
 foursight-core = "^5.4.0"
 # use below for tests but not for deployment
 #foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="core2" }
 #portal-pipeline-utils = "2.1.0.1b1"
 # Need pytest-redis 3.0.2 or higher for pytest 7.4.2 (or higher).
```

### Comparing `foursight_smaht-0.8.5/PKG-INFO` & `foursight_smaht-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-smaht
-Version: 0.8.5
+Version: 0.8.6
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,14 @@
 Requires-Dist: dcicutils (>=8.0.0,<9.0.0)
 Requires-Dist: elasticsearch (==7.13.4)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
 Requires-Dist: foursight-core (>=5.4.0,<6.0.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
-Requires-Dist: magma-suite (>=3.1.0,<4.0.0)
+Requires-Dist: magma-suite (>=3.2.1,<4.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: pytest (>=7.4.2,<8.0.0)
 Requires-Dist: pytest-redis (>=3.0.2,<4.0.0)
 Requires-Dist: pytz (>=2020.1,<2021.0)
 Requires-Dist: tibanna-ff (>=3.2.0,<4.0.0)
 Requires-Dist: tzlocal (>=5.1,<6.0)
```

