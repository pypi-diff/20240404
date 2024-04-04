# Comparing `tmp/custom_cytomine_client-0.0.7.tar.gz` & `tmp/custom_cytomine_client-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_cytomine_client-0.0.7.tar", max compression
+gzip compressed data, was "custom_cytomine_client-0.0.8.tar", max compression
```

## Comparing `custom_cytomine_client-0.0.7.tar` & `custom_cytomine_client-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.7/README.md
--rw-r--r--   0        0        0      290 2024-04-04 08:20:03.608390 custom_cytomine_client-0.0.7/custom_cytomine_client/__init__.py
--rw-r--r--   0        0        0     6983 2024-04-04 01:15:57.625119 custom_cytomine_client-0.0.7/custom_cytomine_client/converter.py
--rw-r--r--   0        0        0      181 2024-04-04 01:11:32.504278 custom_cytomine_client-0.0.7/custom_cytomine_client/custom_types/__init__.py
--rw-r--r--   0        0        0     1169 2024-04-04 00:37:03.211426 custom_cytomine_client-0.0.7/custom_cytomine_client/custom_types/converter.py
--rw-r--r--   0        0        0      162 2024-04-04 01:14:08.987014 custom_cytomine_client-0.0.7/custom_cytomine_client/util/__init__.py
--rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.7/custom_cytomine_client/util/custom_exception.py
--rw-r--r--   0        0        0     2232 2024-04-04 01:14:08.982867 custom_cytomine_client-0.0.7/custom_cytomine_client/util/fit_util.py
--rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.7/custom_cytomine_client/util/normal_util.py
--rw-r--r--   0        0        0      726 2024-04-04 08:20:08.255591 custom_cytomine_client-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       70 2024-04-03 09:00:43.689977 custom_cytomine_client-0.0.8/README.md
+-rw-r--r--   0        0        0       82 2024-04-04 08:22:45.857833 custom_cytomine_client-0.0.8/custom_cytomine_client/__init__.py
+-rw-r--r--   0        0        0     7084 2024-04-04 08:21:59.692699 custom_cytomine_client-0.0.8/custom_cytomine_client/converter.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:21:59.692773 custom_cytomine_client-0.0.8/custom_cytomine_client/interface/__init__.py
+-rw-r--r--   0        0        0      667 2024-04-04 08:21:59.692900 custom_cytomine_client-0.0.8/custom_cytomine_client/interface/converter.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:21:59.693022 custom_cytomine_client-0.0.8/custom_cytomine_client/object/__init__.py
+-rw-r--r--   0        0        0      594 2024-04-04 08:21:59.693147 custom_cytomine_client-0.0.8/custom_cytomine_client/object/converter.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:21:59.693627 custom_cytomine_client-0.0.8/custom_cytomine_client/util/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-02 08:34:59.565119 custom_cytomine_client-0.0.8/custom_cytomine_client/util/custom_exception.py
+-rw-r--r--   0        0        0     2220 2024-04-04 08:21:59.693785 custom_cytomine_client-0.0.8/custom_cytomine_client/util/fit_util.py
+-rw-r--r--   0        0        0      485 2024-04-02 07:41:42.188210 custom_cytomine_client-0.0.8/custom_cytomine_client/util/normal_util.py
+-rw-r--r--   0        0        0      726 2024-04-04 08:22:45.854078 custom_cytomine_client-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 custom_cytomine_client-0.0.8/PKG-INFO
```

### Comparing `custom_cytomine_client-0.0.7/custom_cytomine_client/converter.py` & `custom_cytomine_client-0.0.8/custom_cytomine_client/converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,19 @@
     TermCollection,
     Annotation,
     AnnotationTerm,
 )
 from typing import List, Union, Optional
 from overrides import override
 
-from util import NormalUtil, FitUtil, XMLImageNameNotFoundError
-from custom_types import (
-    CustomCytomineClientInterface,
+from interface.converter import CustomCytomineClientInterface
+from util.normal_util import NormalUtil
+from util.fit_util import FitUtil
+from util.custom_exception import XMLImageNameNotFoundError
+from object.converter import (
     CytomineAnnotationInfo,
     CytomineTermInfo,
     CytomineImageInfo,
     CytomineProjectInfo,
 )
```

### Comparing `custom_cytomine_client-0.0.7/custom_cytomine_client/util/fit_util.py` & `custom_cytomine_client-0.0.8/custom_cytomine_client/util/fit_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Dict, Any, List
 
-from custom_types.converter import CytomineAnnotationInfo
+from object.converter import CytomineAnnotationInfo
 
 
 class FitUtil:
     @classmethod
     def parse_xml_to_cytomine_annotation_info(cls, xml_dict_data: Dict[str, Any]) -> CytomineAnnotationInfo:
-        annotations_data = xml_dict_data["custom_types-stream"]["Annotations"]
+        annotations_data = xml_dict_data["object-stream"]["Annotations"]
         image_name = annotations_data["@image"]
         annotation_infos = []
         if type(annotations_data["Annotation"]) == dict:
             annotation_info = annotations_data["Annotation"]
             class_name = annotation_info["@class"]
             polygon_points = [
                 CytomineAnnotationInfo.AnnotationInfo.PolygonInfo(x=float(coord["@x"]), y=float(coord["@y"]))
```

### Comparing `custom_cytomine_client-0.0.7/pyproject.toml` & `custom_cytomine_client-0.0.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "custom-cytomine-client"
-version = "0.0.7"
-description = "Custom Cytomine Client for Python"
+version = "0.0.8"
+description = "Custom Cytomine client for Python"
 authors = ["punrabbit <tjdmsch2201@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 annotated-types = "0.6.0"
 black = "24.3.0"
```

### Comparing `custom_cytomine_client-0.0.7/PKG-INFO` & `custom_cytomine_client-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: custom-cytomine-client
-Version: 0.0.7
-Summary: Custom Cytomine Client for Python
+Version: 0.0.8
+Summary: Custom Cytomine client for Python
 Author: punrabbit
 Author-email: tjdmsch2201@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

