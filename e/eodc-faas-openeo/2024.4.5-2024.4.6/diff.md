# Comparing `tmp/eodc_faas_openeo-2024.4.5.tar.gz` & `tmp/eodc_faas_openeo-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_openeo-2024.4.5.tar", max compression
+gzip compressed data, was "eodc_faas_openeo-2024.4.6.tar", max compression
```

## Comparing `eodc_faas_openeo-2024.4.5.tar` & `eodc_faas_openeo-2024.4.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       11 2024-04-04 07:20:32.236000 eodc_faas_openeo-2024.4.5/README.md
--rw-r--r--   0        0        0       76 2024-04-04 07:20:32.236000 eodc_faas_openeo-2024.4.5/openeo_executor_bindings/__init__.py
--rw-r--r--   0        0        0      901 2024-04-04 07:20:32.236000 eodc_faas_openeo-2024.4.5/openeo_executor_bindings/model.py
--rw-r--r--   0        0        0      659 2024-04-04 07:20:32.236000 eodc_faas_openeo-2024.4.5/pyproject.toml
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 eodc_faas_openeo-2024.4.5/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-04-04 11:52:30.000000 eodc_faas_openeo-2024.4.6/README.md
+-rw-r--r--   0        0        0       76 2024-04-04 11:52:30.000000 eodc_faas_openeo-2024.4.6/openeo_executor_bindings/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-04 11:52:30.000000 eodc_faas_openeo-2024.4.6/openeo_executor_bindings/model.py
+-rw-r--r--   0        0        0      659 2024-04-04 11:52:30.000000 eodc_faas_openeo-2024.4.6/pyproject.toml
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 eodc_faas_openeo-2024.4.6/PKG-INFO
```

### Comparing `eodc_faas_openeo-2024.4.5/openeo_executor_bindings/model.py` & `eodc_faas_openeo-2024.4.6/openeo_executor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_openeo-2024.4.5/pyproject.toml` & `eodc_faas_openeo-2024.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-openeo"
-version = "2024.4.5"
+version = "2024.4.6"
 description = "Bindings for the OpenEO processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>", "Gerald Irsiegler <gerald.irsiegler@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "openeo_executor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_openeo-2024.4.5/PKG-INFO` & `eodc_faas_openeo-2024.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-openeo
-Version: 2024.4.5
+Version: 2024.4.6
 Summary: Bindings for the OpenEO processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

