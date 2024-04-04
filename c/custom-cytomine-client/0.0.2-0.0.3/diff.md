# Comparing `tmp/custom_cytomine_client-0.0.2.tar.gz` & `tmp/custom_cytomine_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_cytomine_client-0.0.2.tar", max compression
+gzip compressed data, was "custom_cytomine_client-0.0.3.tar", max compression
```

## Comparing `custom_cytomine_client-0.0.2.tar` & `custom_cytomine_client-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,11 @@
--rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.2/README.md
--rw-r--r--   0        0        0      105 2024-04-03 09:55:25.277416 custom_cytomine_client-0.0.2/custom_cytomine_client/__init__.py
--rw-r--r--   0        0        0     7084 2024-04-03 09:45:13.244491 custom_cytomine_client-0.0.2/custom_cytomine_client/converter.py
--rw-r--r--   0        0        0        0 2024-04-03 08:59:25.424661 custom_cytomine_client-0.0.2/custom_cytomine_client/interface/__init__.py
--rw-r--r--   0        0        0      667 2024-04-03 09:45:13.249640 custom_cytomine_client-0.0.2/custom_cytomine_client/interface/converter.py
--rw-r--r--   0        0        0        0 2024-04-03 08:59:25.440198 custom_cytomine_client-0.0.2/custom_cytomine_client/object/__init__.py
--rw-r--r--   0        0        0      594 2024-04-03 03:17:44.790948 custom_cytomine_client-0.0.2/custom_cytomine_client/object/converter.py
--rw-r--r--   0        0        0        0 2024-04-03 08:59:25.449721 custom_cytomine_client-0.0.2/custom_cytomine_client/util/__init__.py
--rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.2/custom_cytomine_client/util/custom_exception.py
--rw-r--r--   0        0        0     2220 2024-04-03 03:31:00.559389 custom_cytomine_client-0.0.2/custom_cytomine_client/util/fit_util.py
--rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.2/custom_cytomine_client/util/normal_util.py
--rw-r--r--   0        0        0      726 2024-04-03 09:55:25.281338 custom_cytomine_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.3/README.md
+-rw-r--r--   0        0        0       82 2024-04-04 00:40:37.901042 custom_cytomine_client-0.0.3/custom_cytomine_client/__init__.py
+-rw-r--r--   0        0        0     7079 2024-04-04 00:37:03.214145 custom_cytomine_client-0.0.3/custom_cytomine_client/converter.py
+-rw-r--r--   0        0        0      180 2024-04-04 00:39:22.534385 custom_cytomine_client-0.0.3/custom_cytomine_client/types/__init__.py
+-rw-r--r--   0        0        0     1169 2024-04-04 00:37:03.211426 custom_cytomine_client-0.0.3/custom_cytomine_client/types/converter.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:59:25.449721 custom_cytomine_client-0.0.3/custom_cytomine_client/util/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.3/custom_cytomine_client/util/custom_exception.py
+-rw-r--r--   0        0        0     2219 2024-04-04 00:30:03.481393 custom_cytomine_client-0.0.3/custom_cytomine_client/util/fit_util.py
+-rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.3/custom_cytomine_client/util/normal_util.py
+-rw-r--r--   0        0        0      726 2024-04-04 00:40:47.679962 custom_cytomine_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.3/PKG-INFO
```

### Comparing `custom_cytomine_client-0.0.2/custom_cytomine_client/converter.py` & `custom_cytomine_client-0.0.3/custom_cytomine_client/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     TermCollection,
     Annotation,
     AnnotationTerm,
 )
 from typing import List, Union, Optional
 from overrides import override
 
-from interface.converter import CustomCytomineClientInterface
+from types.converter import CustomCytomineClientInterface
 from util.normal_util import NormalUtil
 from util.fit_util import FitUtil
 from util.custom_exception import XMLImageNameNotFoundError
-from object.converter import (
+from types.converter import (
     CytomineAnnotationInfo,
     CytomineTermInfo,
     CytomineImageInfo,
     CytomineProjectInfo,
 )
```

### Comparing `custom_cytomine_client-0.0.2/custom_cytomine_client/util/fit_util.py` & `custom_cytomine_client-0.0.3/custom_cytomine_client/util/fit_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from object.converter import CytomineAnnotationInfo
 
 
 class FitUtil:
     @classmethod
     def parse_xml_to_cytomine_annotation_info(cls, xml_dict_data: Dict[str, Any]) -> CytomineAnnotationInfo:
-        annotations_data = xml_dict_data["object-stream"]["Annotations"]
+        annotations_data = xml_dict_data["types-stream"]["Annotations"]
         image_name = annotations_data["@image"]
         annotation_infos = []
         if type(annotations_data["Annotation"]) == dict:
             annotation_info = annotations_data["Annotation"]
             class_name = annotation_info["@class"]
             polygon_points = [
                 CytomineAnnotationInfo.AnnotationInfo.PolygonInfo(x=float(coord["@x"]), y=float(coord["@y"]))
```

### Comparing `custom_cytomine_client-0.0.2/pyproject.toml` & `custom_cytomine_client-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "custom-cytomine-client"
-version = "0.0.2"
-description = "Custom Cytomine client for Python"
+version = "0.0.3"
+description = "Custom Cytomine Client for Python"
 authors = ["punrabbit <tjdmsch2201@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 annotated-types = "0.6.0"
 black = "24.3.0"
```

### Comparing `custom_cytomine_client-0.0.2/PKG-INFO` & `custom_cytomine_client-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: custom-cytomine-client
-Version: 0.0.2
-Summary: Custom Cytomine client for Python
+Version: 0.0.3
+Summary: Custom Cytomine Client for Python
 Author: punrabbit
 Author-email: tjdmsch2201@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

