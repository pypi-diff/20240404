# Comparing `tmp/custom_cytomine_client-0.0.4.tar.gz` & `tmp/custom_cytomine_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_cytomine_client-0.0.4.tar", max compression
+gzip compressed data, was "custom_cytomine_client-0.0.5.tar", max compression
```

## Comparing `custom_cytomine_client-0.0.4.tar` & `custom_cytomine_client-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.4/README.md
--rw-r--r--   0        0        0       82 2024-04-04 00:40:37.901042 custom_cytomine_client-0.0.4/custom_cytomine_client/__init__.py
--rw-r--r--   0        0        0     7053 2024-04-04 01:11:32.512718 custom_cytomine_client-0.0.4/custom_cytomine_client/converter.py
--rw-r--r--   0        0        0      181 2024-04-04 01:11:32.504278 custom_cytomine_client-0.0.4/custom_cytomine_client/custom_types/__init__.py
--rw-r--r--   0        0        0     1169 2024-04-04 00:37:03.211426 custom_cytomine_client-0.0.4/custom_cytomine_client/custom_types/converter.py
--rw-r--r--   0        0        0        0 2024-04-03 08:59:25.449721 custom_cytomine_client-0.0.4/custom_cytomine_client/util/__init__.py
--rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.4/custom_cytomine_client/util/custom_exception.py
--rw-r--r--   0        0        0     2226 2024-04-04 01:11:32.507625 custom_cytomine_client-0.0.4/custom_cytomine_client/util/fit_util.py
--rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.4/custom_cytomine_client/util/normal_util.py
--rw-r--r--   0        0        0      726 2024-04-04 01:11:32.509851 custom_cytomine_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.5/README.md
+-rw-r--r--   0        0        0       82 2024-04-04 00:40:37.901042 custom_cytomine_client-0.0.5/custom_cytomine_client/__init__.py
+-rw-r--r--   0        0        0     7053 2024-04-04 01:11:32.512718 custom_cytomine_client-0.0.5/custom_cytomine_client/converter.py
+-rw-r--r--   0        0        0      181 2024-04-04 01:11:32.504278 custom_cytomine_client-0.0.5/custom_cytomine_client/custom_types/__init__.py
+-rw-r--r--   0        0        0     1169 2024-04-04 00:37:03.211426 custom_cytomine_client-0.0.5/custom_cytomine_client/custom_types/converter.py
+-rw-r--r--   0        0        0      162 2024-04-04 01:14:08.987014 custom_cytomine_client-0.0.5/custom_cytomine_client/util/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.5/custom_cytomine_client/util/custom_exception.py
+-rw-r--r--   0        0        0     2232 2024-04-04 01:14:08.982867 custom_cytomine_client-0.0.5/custom_cytomine_client/util/fit_util.py
+-rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.5/custom_cytomine_client/util/normal_util.py
+-rw-r--r--   0        0        0      726 2024-04-04 01:14:23.265671 custom_cytomine_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.5/PKG-INFO
```

### Comparing `custom_cytomine_client-0.0.4/custom_cytomine_client/converter.py` & `custom_cytomine_client-0.0.5/custom_cytomine_client/converter.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.0.4/custom_cytomine_client/custom_types/converter.py` & `custom_cytomine_client-0.0.5/custom_cytomine_client/custom_types/converter.py`

 * *Files identical despite different names*

### Comparing `custom_cytomine_client-0.0.4/custom_cytomine_client/util/fit_util.py` & `custom_cytomine_client-0.0.5/custom_cytomine_client/util/fit_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Any, List
 
-from object.converter import CytomineAnnotationInfo
+from custom_types.converter import CytomineAnnotationInfo
 
 
 class FitUtil:
     @classmethod
     def parse_xml_to_cytomine_annotation_info(cls, xml_dict_data: Dict[str, Any]) -> CytomineAnnotationInfo:
         annotations_data = xml_dict_data["custom_types-stream"]["Annotations"]
         image_name = annotations_data["@image"]
```

### Comparing `custom_cytomine_client-0.0.4/pyproject.toml` & `custom_cytomine_client-0.0.5/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "custom-cytomine-client"
-version = "0.0.4"
+version = "0.0.5"
 description = "Custom Cytomine Client for Python"
 authors = ["punrabbit <tjdmsch2201@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 annotated-types = "0.6.0"
```

### Comparing `custom_cytomine_client-0.0.4/PKG-INFO` & `custom_cytomine_client-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custom-cytomine-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Custom Cytomine Client for Python
 Author: punrabbit
 Author-email: tjdmsch2201@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

