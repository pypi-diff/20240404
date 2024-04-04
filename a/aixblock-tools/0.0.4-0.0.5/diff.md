# Comparing `tmp/aixblock_tools-0.0.4.tar.gz` & `tmp/aixblock_tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_tools-0.0.4.tar", max compression
+gzip compressed data, was "aixblock_tools-0.0.5.tar", max compression
```

## Comparing `aixblock_tools-0.0.4.tar` & `aixblock_tools-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       14 2024-04-02 11:26:35.487186 aixblock_tools-0.0.4/README.md
--rw-r--r--   0        0        0     6148 2024-04-03 05:20:29.911723 aixblock_tools-0.0.4/aixblock_tools/.DS_Store
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.157031 aixblock_tools-0.0.4/aixblock_tools/__init__.py
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.157393 aixblock_tools-0.0.4/aixblock_tools/core/__init__.py
--rw-r--r--   0        0        0      204 2023-08-31 04:15:47.167875 aixblock_tools-0.0.4/aixblock_tools/core/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4302 2023-08-31 04:15:47.169561 aixblock_tools-0.0.4/aixblock_tools/core/__pycache__/label_config.cpython-39.pyc
--rw-r--r--   0        0        0     5753 2024-04-03 07:24:15.704627 aixblock_tools-0.0.4/aixblock_tools/core/label_config.py
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.158189 aixblock_tools-0.0.4/aixblock_tools/core/utils/__init__.py
--rw-r--r--   0        0        0      210 2023-08-31 04:15:47.170281 aixblock_tools-0.0.4/aixblock_tools/core/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      405 2023-08-31 04:15:47.170884 aixblock_tools-0.0.4/aixblock_tools/core/utils/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0        0        0     3489 2023-08-31 04:15:47.172503 aixblock_tools-0.0.4/aixblock_tools/core/utils/__pycache__/io.cpython-39.pyc
--rw-r--r--   0        0        0     1362 2023-08-31 04:15:47.173662 aixblock_tools-0.0.4/aixblock_tools/core/utils/__pycache__/params.cpython-39.pyc
--rw-r--r--   0        0        0       66 2023-08-31 04:15:47.158548 aixblock_tools-0.0.4/aixblock_tools/core/utils/exceptions.py
--rw-r--r--   0        0        0     3981 2024-04-04 02:14:25.160292 aixblock_tools-0.0.4/aixblock_tools/core/utils/io.py
--rw-r--r--   0        0        0     1241 2024-04-03 08:23:43.577921 aixblock_tools-0.0.4/aixblock_tools/core/utils/params.py
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.159877 aixblock_tools-0.0.4/aixblock_tools/postprocessing/__init__.py
--rw-r--r--   0        0        0      214 2023-08-31 04:15:47.174550 aixblock_tools-0.0.4/aixblock_tools/postprocessing/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2584 2023-08-31 04:15:47.175963 aixblock_tools-0.0.4/aixblock_tools/postprocessing/__pycache__/video.cpython-39.pyc
--rw-r--r--   0        0        0     3486 2024-04-03 07:24:15.704467 aixblock_tools-0.0.4/aixblock_tools/postprocessing/video.py
--rw-r--r--   0        0        0        0 2023-08-31 04:15:47.160904 aixblock_tools-0.0.4/aixblock_tools/tests/__init__.py
--rw-r--r--   0        0        0      205 2023-08-31 04:15:47.176686 aixblock_tools-0.0.4/aixblock_tools/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     4193 2023-08-31 04:15:47.177862 aixblock_tools-0.0.4/aixblock_tools/tests/__pycache__/test_core_label_config.cpython-39.pyc
--rw-r--r--   0        0        0     6811 2023-08-31 04:15:47.180967 aixblock_tools-0.0.4/aixblock_tools/tests/__pycache__/test_postprocessing_video.cpython-39.pyc
--rw-r--r--   0        0        0     4349 2024-04-03 07:24:15.766177 aixblock_tools-0.0.4/aixblock_tools/tests/test_core_label_config.py
--rw-r--r--   0        0        0    14387 2024-04-03 07:24:15.765793 aixblock_tools-0.0.4/aixblock_tools/tests/test_postprocessing_video.py
--rw-r--r--   0        0        0      266 2024-04-04 02:14:34.206410 aixblock_tools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 aixblock_tools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       14 2024-04-02 11:26:35.487186 aixblock_tools-0.0.5/README.md
+-rw-r--r--   0        0        0     6148 2024-04-03 05:20:29.911723 aixblock_tools-0.0.5/aixblock_tools/.DS_Store
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.157031 aixblock_tools-0.0.5/aixblock_tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.157393 aixblock_tools-0.0.5/aixblock_tools/core/__init__.py
+-rw-r--r--   0        0        0      204 2023-08-31 04:15:47.167875 aixblock_tools-0.0.5/aixblock_tools/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4302 2023-08-31 04:15:47.169561 aixblock_tools-0.0.5/aixblock_tools/core/__pycache__/label_config.cpython-39.pyc
+-rw-r--r--   0        0        0     5724 2024-04-04 03:08:16.488954 aixblock_tools-0.0.5/aixblock_tools/core/label_config.py
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.158189 aixblock_tools-0.0.5/aixblock_tools/core/utils/__init__.py
+-rw-r--r--   0        0        0      210 2023-08-31 04:15:47.170281 aixblock_tools-0.0.5/aixblock_tools/core/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      405 2023-08-31 04:15:47.170884 aixblock_tools-0.0.5/aixblock_tools/core/utils/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0        0        0     3489 2023-08-31 04:15:47.172503 aixblock_tools-0.0.5/aixblock_tools/core/utils/__pycache__/io.cpython-39.pyc
+-rw-r--r--   0        0        0     1362 2023-08-31 04:15:47.173662 aixblock_tools-0.0.5/aixblock_tools/core/utils/__pycache__/params.cpython-39.pyc
+-rw-r--r--   0        0        0       63 2024-04-04 03:08:23.013269 aixblock_tools-0.0.5/aixblock_tools/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3981 2024-04-04 02:14:25.160292 aixblock_tools-0.0.5/aixblock_tools/core/utils/io.py
+-rw-r--r--   0        0        0     1241 2024-04-03 08:23:43.577921 aixblock_tools-0.0.5/aixblock_tools/core/utils/params.py
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.159877 aixblock_tools-0.0.5/aixblock_tools/postprocessing/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-31 04:15:47.174550 aixblock_tools-0.0.5/aixblock_tools/postprocessing/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2584 2023-08-31 04:15:47.175963 aixblock_tools-0.0.5/aixblock_tools/postprocessing/__pycache__/video.cpython-39.pyc
+-rw-r--r--   0        0        0     3486 2024-04-04 03:07:45.794761 aixblock_tools-0.0.5/aixblock_tools/postprocessing/video.py
+-rw-r--r--   0        0        0        0 2023-08-31 04:15:47.160904 aixblock_tools-0.0.5/aixblock_tools/tests/__init__.py
+-rw-r--r--   0        0        0      205 2023-08-31 04:15:47.176686 aixblock_tools-0.0.5/aixblock_tools/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4193 2023-08-31 04:15:47.177862 aixblock_tools-0.0.5/aixblock_tools/tests/__pycache__/test_core_label_config.cpython-39.pyc
+-rw-r--r--   0        0        0     6811 2023-08-31 04:15:47.180967 aixblock_tools-0.0.5/aixblock_tools/tests/__pycache__/test_postprocessing_video.cpython-39.pyc
+-rw-r--r--   0        0        0     4349 2024-04-03 07:24:15.766177 aixblock_tools-0.0.5/aixblock_tools/tests/test_core_label_config.py
+-rw-r--r--   0        0        0    14387 2024-04-03 07:24:15.765793 aixblock_tools-0.0.5/aixblock_tools/tests/test_postprocessing_video.py
+-rw-r--r--   0        0        0      266 2024-04-04 03:45:21.286669 aixblock_tools-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 aixblock_tools-0.0.5/PKG-INFO
```

### Comparing `aixblock_tools-0.0.4/aixblock_tools/.DS_Store` & `aixblock_tools-0.0.5/aixblock_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/core/__pycache__/label_config.cpython-39.pyc` & `aixblock_tools-0.0.5/aixblock_tools/core/__pycache__/label_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/core/label_config.py` & `aixblock_tools-0.0.5/aixblock_tools/core/label_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 import re
 
 from collections import defaultdict
 from lxml import etree
 
-from aixblock_tools.core.utils.exceptions import (
-    LabelStudioXMLSyntaxErrorSentryIgnored,
+from .utils.exceptions import (
+    AIxBlockXMLSyntaxErrorSentryIgnored,
 )
 
 logger = logging.getLogger(__name__)
 
 _LABEL_TAGS = {'Label', 'Choice', 'Relation'}
 _NOT_CONTROL_TAGS = {
     'Filter',
 }
-_DIR_APP_NAME = 'label-studio'
+_DIR_APP_NAME = 'aixblock'
 _VIDEO_TRACKING_TAGS = {'videorectangle'}
 
 
 def parse_config(config_string):
     """Parse a given Label Studio labeling configuration and return a structured version of the configuration.
     Useful for formatting results for predicted annotations and determining the type(s) of ML models that might
     be relevant to the labeling project.
@@ -38,15 +38,15 @@
     """
     if not config_string:
         return {}
 
     try:
         xml_tree = etree.fromstring(config_string)
     except etree.XMLSyntaxError as e:
-        raise LabelStudioXMLSyntaxErrorSentryIgnored(str(e))
+        raise AIxBlockXMLSyntaxErrorSentryIgnored(str(e))
     inputs, outputs, labels = {}, {}, defaultdict(dict)
     # Add variables to config (e.g. {{idx}} for index in Repeater
     variables = []
     for tag in xml_tree.iter():
         if tag.attrib and 'indexFlag' in tag.attrib:
             variables.append(tag.attrib['indexFlag'])
         if _is_output_tag(tag):
```

### Comparing `aixblock_tools-0.0.4/aixblock_tools/core/utils/__pycache__/io.cpython-39.pyc` & `aixblock_tools-0.0.5/aixblock_tools/core/utils/__pycache__/io.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/core/utils/__pycache__/params.cpython-39.pyc` & `aixblock_tools-0.0.5/aixblock_tools/core/utils/__pycache__/params.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/core/utils/io.py` & `aixblock_tools-0.0.5/aixblock_tools/core/utils/io.py`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/core/utils/params.py` & `aixblock_tools-0.0.5/aixblock_tools/core/utils/params.py`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/postprocessing/__pycache__/video.cpython-39.pyc` & `aixblock_tools-0.0.5/aixblock_tools/postprocessing/__pycache__/video.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/postprocessing/video.py` & `aixblock_tools-0.0.5/aixblock_tools/postprocessing/video.py`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/tests/__pycache__/test_core_label_config.cpython-39.pyc` & `aixblock_tools-0.0.5/aixblock_tools/tests/__pycache__/test_core_label_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/tests/__pycache__/test_postprocessing_video.cpython-39.pyc` & `aixblock_tools-0.0.5/aixblock_tools/tests/__pycache__/test_postprocessing_video.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/tests/test_core_label_config.py` & `aixblock_tools-0.0.5/aixblock_tools/tests/test_core_label_config.py`

 * *Files identical despite different names*

### Comparing `aixblock_tools-0.0.4/aixblock_tools/tests/test_postprocessing_video.py` & `aixblock_tools-0.0.5/aixblock_tools/tests/test_postprocessing_video.py`

 * *Files identical despite different names*

