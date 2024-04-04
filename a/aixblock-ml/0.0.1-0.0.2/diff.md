# Comparing `tmp/aixblock_ml-0.0.1.tar.gz` & `tmp/aixblock_ml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_ml-0.0.1.tar", max compression
+gzip compressed data, was "aixblock_ml-0.0.2.tar", max compression
```

## Comparing `aixblock_ml-0.0.1.tar` & `aixblock_ml-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6488 2024-04-02 09:32:28.849201 aixblock_ml-0.0.1/README.md
--rw-r--r--   0        0        0       84 2024-04-01 06:20:49.108490 aixblock_ml-0.0.1/aixblock_ml/__init__.py
--rw-r--r--   0        0        0     8940 2024-04-01 06:42:58.082943 aixblock_ml-0.0.1/aixblock_ml/api.py
--rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.1/aixblock_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2701 2024-04-01 06:20:49.119434 aixblock_ml-0.0.1/aixblock_ml/default_configs/README.md
--rw-r--r--   0        0        0     3861 2024-04-01 06:20:49.120057 aixblock_ml-0.0.1/aixblock_ml/default_configs/_wsgi.py
--rw-r--r--   0        0        0     3857 2024-04-03 06:08:47.124828 aixblock_ml-0.0.1/aixblock_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      563 2024-04-01 06:20:49.121558 aixblock_ml-0.0.1/aixblock_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0     2145 2024-04-03 06:08:47.125040 aixblock_ml-0.0.1/aixblock_ml/default_configs/model.py
--rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.1/aixblock_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.1/aixblock_ml/exceptions.py
--rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.1/aixblock_ml/helpers.py
--rw-r--r--   0        0        0    34780 2024-04-01 06:43:18.973363 aixblock_ml-0.0.1/aixblock_ml/model.py
--rw-r--r--   0        0        0     7515 2024-04-01 06:43:12.387687 aixblock_ml-0.0.1/aixblock_ml/server.py
--rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.1/aixblock_ml/templates/preview.html
--rw-r--r--   0        0        0     1999 2024-04-01 06:43:17.236638 aixblock_ml-0.0.1/aixblock_ml/utils.py
--rw-r--r--   0        0        0      264 2024-04-03 05:27:34.346403 aixblock_ml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6872 1970-01-01 00:00:00.000000 aixblock_ml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6488 2024-04-02 09:32:28.849201 aixblock_ml-0.0.2/README.md
+-rw-r--r--   0        0        0       84 2024-04-01 06:20:49.108490 aixblock_ml-0.0.2/aixblock_ml/__init__.py
+-rw-r--r--   0        0        0     8940 2024-04-01 06:42:58.082943 aixblock_ml-0.0.2/aixblock_ml/api.py
+-rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.0.2/aixblock_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2701 2024-04-01 06:20:49.119434 aixblock_ml-0.0.2/aixblock_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3861 2024-04-01 06:20:49.120057 aixblock_ml-0.0.2/aixblock_ml/default_configs/_wsgi.py
+-rw-r--r--   0        0        0     3857 2024-04-03 06:08:47.124828 aixblock_ml-0.0.2/aixblock_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      563 2024-04-01 06:20:49.121558 aixblock_ml-0.0.2/aixblock_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0     2145 2024-04-03 06:08:47.125040 aixblock_ml-0.0.2/aixblock_ml/default_configs/model.py
+-rw-r--r--   0        0        0       90 2024-04-01 06:20:49.122796 aixblock_ml-0.0.2/aixblock_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.0.2/aixblock_ml/exceptions.py
+-rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.0.2/aixblock_ml/helpers.py
+-rw-r--r--   0        0        0    34768 2024-04-03 07:24:15.793828 aixblock_ml-0.0.2/aixblock_ml/model.py
+-rw-r--r--   0        0        0     7515 2024-04-01 06:43:12.387687 aixblock_ml-0.0.2/aixblock_ml/server.py
+-rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.0.2/aixblock_ml/templates/preview.html
+-rw-r--r--   0        0        0     1991 2024-04-03 07:24:15.797590 aixblock_ml-0.0.2/aixblock_ml/utils.py
+-rw-r--r--   0        0        0      264 2024-04-03 07:25:12.648356 aixblock_ml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6872 1970-01-01 00:00:00.000000 aixblock_ml-0.0.2/PKG-INFO
```

### Comparing `aixblock_ml-0.0.1/README.md` & `aixblock_ml-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/api.py` & `aixblock_ml-0.0.2/aixblock_ml/api.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/default_configs/README.md` & `aixblock_ml-0.0.2/aixblock_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/default_configs/_wsgi.py` & `aixblock_ml-0.0.2/aixblock_ml/default_configs/_wsgi.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/default_configs/_wsgi.py.tmpl` & `aixblock_ml-0.0.2/aixblock_ml/default_configs/_wsgi.py.tmpl`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/default_configs/docker-compose.yml` & `aixblock_ml-0.0.2/aixblock_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/default_configs/model.py` & `aixblock_ml-0.0.2/aixblock_ml/default_configs/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/exceptions.py` & `aixblock_ml-0.0.2/aixblock_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/helpers.py` & `aixblock_ml-0.0.2/aixblock_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/model.py` & `aixblock_ml-0.0.2/aixblock_ml/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 from contextlib import contextmanager
 from redis import Redis
 from rq import Queue, get_current_job
 from rq.registry import StartedJobRegistry, FinishedJobRegistry, FailedJobRegistry
 from rq.job import Job
 from colorama import Fore
 
-from label_studio_tools.core.utils.params import get_bool_env
-from label_studio_tools.core.label_config import parse_config
-from label_studio_tools.core.utils.io import get_local_path
+from aixblock_tools.core.utils.params import get_bool_env
+from aixblock_tools.core.label_config import parse_config
+from aixblock_tools.core.utils.io import get_local_path
 
 logger = logging.getLogger(__name__)
 
 LABEL_STUDIO_ML_BACKEND_V2_DEFAULT = False
 
 @attr.s
 class ModelWrapper(object):
```

### Comparing `aixblock_ml-0.0.1/aixblock_ml/server.py` & `aixblock_ml-0.0.2/aixblock_ml/server.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.0.1/aixblock_ml/utils.py` & `aixblock_ml-0.0.2/aixblock_ml/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
 from PIL import Image
 
-from label_studio_tools.core.utils.params import get_env
-from label_studio_tools.core.utils.io import get_local_path
+from aixblock_tools.core.utils.params import get_env
+from aixblock_tools.core.utils.io import get_local_path
 
 DATA_UNDEFINED_NAME = '$undefined$'
 
 logger = logging.getLogger(__name__)
 
 
 def get_single_tag_keys(parsed_label_config, control_type, object_type):
```

### Comparing `aixblock_ml-0.0.1/PKG-INFO` & `aixblock_ml-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixblock_ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: AIxBlock
 Author-email: info@aixblock.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

