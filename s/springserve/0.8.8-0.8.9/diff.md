# Comparing `tmp/springserve-0.8.8.tar.gz` & `tmp/springserve-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "springserve-0.8.8.tar", last modified: Tue Sep 28 13:34:53 2021, max compression
+gzip compressed data, was "springserve-0.8.9.tar", last modified: Wed Oct  6 16:15:28 2021, max compression
```

## Comparing `springserve-0.8.8.tar` & `springserve-0.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2021-09-28 13:34:53.748818 springserve-0.8.8/
--rw-r--r--   0 dave       (501) staff       (20)      776 2021-08-19 17:51:42.000000 springserve-0.8.8/.gitignore
--rw-r--r--   0 dave       (501) staff       (20)      589 2021-09-28 13:34:53.748513 springserve-0.8.8/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)     7513 2021-09-27 21:30:36.000000 springserve-0.8.8/README.md
--rw-r--r--   0 dave       (501) staff       (20)       38 2021-09-28 13:34:53.748912 springserve-0.8.8/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1576 2021-09-28 13:32:42.000000 springserve-0.8.8/setup.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2021-09-28 13:34:53.744762 springserve-0.8.8/springserve/
--rw-r--r--   0 dave       (501) staff       (20)    23101 2021-09-28 13:32:52.000000 springserve-0.8.8/springserve/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)      148 2021-08-19 17:51:42.000000 springserve-0.8.8/springserve/_account.py
--rw-r--r--   0 dave       (501) staff       (20)    12281 2021-08-19 18:34:12.000000 springserve-0.8.8/springserve/_common.py
--rw-r--r--   0 dave       (501) staff       (20)     3420 2021-08-19 17:51:42.000000 springserve-0.8.8/springserve/_decorators.py
--rw-r--r--   0 dave       (501) staff       (20)     2101 2021-08-20 14:51:26.000000 springserve-0.8.8/springserve/_demand.py
--rw-r--r--   0 dave       (501) staff       (20)      109 2021-08-19 17:51:42.000000 springserve-0.8.8/springserve/_direct_connect.py
--rw-r--r--   0 dave       (501) staff       (20)      123 2021-08-19 17:51:42.000000 springserve-0.8.8/springserve/_object_change_messages.py
--rw-r--r--   0 dave       (501) staff       (20)     5621 2021-08-19 17:51:42.000000 springserve-0.8.8/springserve/_reporting.py
--rw-r--r--   0 dave       (501) staff       (20)      470 2021-08-19 17:51:42.000000 springserve-0.8.8/springserve/_supply.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2021-09-28 13:34:53.746457 springserve-0.8.8/springserve.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      589 2021-09-28 13:34:53.000000 springserve-0.8.8/springserve.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      508 2021-09-28 13:34:53.000000 springserve-0.8.8/springserve.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2021-09-28 13:34:53.000000 springserve-0.8.8/springserve.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)      105 2021-09-28 13:34:53.000000 springserve-0.8.8/springserve.egg-info/requires.txt
--rw-r--r--   0 dave       (501) staff       (20)       12 2021-09-28 13:34:53.000000 springserve-0.8.8/springserve.egg-info/top_level.txt
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2021-09-28 13:34:53.747913 springserve-0.8.8/tests/
--rw-r--r--   0 dave       (501) staff       (20)      844 2021-08-19 17:51:42.000000 springserve-0.8.8/tests/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)     4819 2021-08-19 17:51:42.000000 springserve-0.8.8/tests/test_responses.py
--rw-r--r--   0 dave       (501) staff       (20)     3871 2021-08-19 17:51:42.000000 springserve-0.8.8/tests/test_services.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2021-10-06 16:15:28.960155 springserve-0.8.9/
+-rw-r--r--   0 dave       (501) staff       (20)      776 2021-08-19 17:51:42.000000 springserve-0.8.9/.gitignore
+-rw-r--r--   0 dave       (501) staff       (20)      589 2021-10-06 16:15:28.959875 springserve-0.8.9/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)     7513 2021-09-27 21:30:36.000000 springserve-0.8.9/README.md
+-rw-r--r--   0 dave       (501) staff       (20)       38 2021-10-06 16:15:28.960247 springserve-0.8.9/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1576 2021-10-06 16:14:55.000000 springserve-0.8.9/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2021-10-06 16:15:28.956793 springserve-0.8.9/springserve/
+-rw-r--r--   0 dave       (501) staff       (20)    23158 2021-10-06 16:14:55.000000 springserve-0.8.9/springserve/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)      148 2021-08-19 17:51:42.000000 springserve-0.8.9/springserve/_account.py
+-rw-r--r--   0 dave       (501) staff       (20)    12520 2021-10-06 16:14:55.000000 springserve-0.8.9/springserve/_common.py
+-rw-r--r--   0 dave       (501) staff       (20)     3420 2021-08-19 17:51:42.000000 springserve-0.8.9/springserve/_decorators.py
+-rw-r--r--   0 dave       (501) staff       (20)     2101 2021-08-20 14:51:26.000000 springserve-0.8.9/springserve/_demand.py
+-rw-r--r--   0 dave       (501) staff       (20)      109 2021-08-19 17:51:42.000000 springserve-0.8.9/springserve/_direct_connect.py
+-rw-r--r--   0 dave       (501) staff       (20)      123 2021-08-19 17:51:42.000000 springserve-0.8.9/springserve/_object_change_messages.py
+-rw-r--r--   0 dave       (501) staff       (20)     5621 2021-08-19 17:51:42.000000 springserve-0.8.9/springserve/_reporting.py
+-rw-r--r--   0 dave       (501) staff       (20)      470 2021-08-19 17:51:42.000000 springserve-0.8.9/springserve/_supply.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2021-10-06 16:15:28.958282 springserve-0.8.9/springserve.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      589 2021-10-06 16:15:28.000000 springserve-0.8.9/springserve.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      508 2021-10-06 16:15:28.000000 springserve-0.8.9/springserve.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2021-10-06 16:15:28.000000 springserve-0.8.9/springserve.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)      105 2021-10-06 16:15:28.000000 springserve-0.8.9/springserve.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       12 2021-10-06 16:15:28.000000 springserve-0.8.9/springserve.egg-info/top_level.txt
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2021-10-06 16:15:28.959395 springserve-0.8.9/tests/
+-rw-r--r--   0 dave       (501) staff       (20)      844 2021-08-19 17:51:42.000000 springserve-0.8.9/tests/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     4819 2021-08-19 17:51:42.000000 springserve-0.8.9/tests/test_responses.py
+-rw-r--r--   0 dave       (501) staff       (20)     3871 2021-08-19 17:51:42.000000 springserve-0.8.9/tests/test_services.py
```

### Comparing `springserve-0.8.8/.gitignore` & `springserve-0.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `springserve-0.8.8/PKG-INFO` & `springserve-0.8.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: springserve
-Version: 0.8.8
+Version: 0.8.9
 Summary: API Library for console.springserve.com
 Home-page: http://www.springserve.com
 Maintainer: dave@springserve.com
 Maintainer-email: 
 License: Apache 2.0
 Description: Springserve is a video adserver, and this library allows you
         to interface with its api to do read/write and reporting requests
```

### Comparing `springserve-0.8.8/README.md` & `springserve-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `springserve-0.8.8/setup.py` & `springserve-0.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 import os
 
 # import all of this version information
-__version__ = '0.8.8'
+__version__ = '0.8.9'
 __author__ = 'dave@springserve.com'
 __license__ = 'Apache 2.0'
 __copyright__ = 'Copyright 2016 Springserve'
 __title__ = 'springserve'
 
 
 dir = os.path.split(os.path.abspath(__file__))[0]
```

### Comparing `springserve-0.8.8/springserve/__init__.py` & `springserve-0.8.9/springserve/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import six
 
 if six.PY3:
     from builtins import input
     from builtins import object
 
 
-__version__ = '0.8.8' #TODO: This is duplicated in the build.  Need to figure how to set this once 
+__version__ = '0.8.9' #TODO: This is duplicated in the build.  Need to figure how to set this once 
 
 import sys as _sys
 import json as _json
 import getpass
 
 from requests_toolbelt import MultipartEncoder
 
@@ -630,15 +630,15 @@
         return self.post(data, path_param, reauth, **query_params)
 
 
 from ._supply import _SupplyTagAPI, _SupplyPartnerAPI, _SupplyLabelAPI, _ConnectedSupplyAPI, _SupplyRouterAPI
 from ._demand import _DemandTagAPI, _DemandPartnerAPI, _DemandLabelAPI, _ConnectedDemandAPI, _CampaignAPI, _SpotxConnectAPI
 from ._demand import _CreativeAPI, _TagCreativeAPI, _VideoCreativeAPI, _AudioCreativeAPI
 from ._common import _DomainListAPI, _BillAPI, _KeyAPI, _AppBundleListAPI, _AppNameListAPI, _IpListAPI, _SegmentListAPI, _AdvertiserDomainListAPI
-from ._common import _ChannelIdListAPI, _DealIdListAPI, _PlacementIdListAPI, _PublisherIdListAPI
+from ._common import _ChannelIdListAPI, _DealIdListAPI, _PlacementIdListAPI, _PublisherIdListAPI, _ParameterListAPI
 from ._reporting import _ReportingAPI, _TrafficQualityReport
 from ._account import _AccountAPI, _UserAPI
 from ._direct_connect import _DirectConnectionAPI
 from ._object_change_messages import _ObjectChangeMessagesAPI
 
 accounts = _AccountAPI()
 app_bundles = _AppBundleListAPI()
@@ -667,14 +667,15 @@
 audio_creatives = _AudioCreativeAPI()
 
 keys = _KeyAPI()
 
 _object_change_messages = _ObjectChangeMessagesAPI()
 
 placement_id_lists = _PlacementIdListAPI()
+parameter_lists = _ParameterListAPI()
 publisher_id_lists = _PublisherIdListAPI()
 
 reports = _ReportingAPI()
 quality_reports = _TrafficQualityReport()
 
 spotx_connects = _SpotxConnectAPI()
 supply_labels = _SupplyLabelAPI()
```

### Comparing `springserve-0.8.8/springserve/_common.py` & `springserve-0.8.9/springserve/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,24 @@
     __LIST_PAYLOAD_ENTRY__="placement_ids"
 
 class _PlacementIdListAPI(_VDAPIService):
 
     __API__ =  "placement_id_lists"
     __RESPONSE_OBJECT__ = _PlacementIdListResponse
 
+class _ParameterListResponse(_BulkListResponse):
+
+    __LIST_API__ = "values"
+    __LIST_PAYLOAD_ENTRY__="values"
+
+class _ParameterListAPI(_VDAPIService):
+
+    __API__ =  "parameter_lists"
+    __RESPONSE_OBJECT__ = _ParameterListResponse
+
 class _PublisherIdListResponse(_BulkListResponse):
 
     __LIST_API__ = "publisher_ids"
     __LIST_PAYLOAD_ENTRY__="publisher_ids"
 
 class _PublisherIdListAPI(_VDAPIService):
```

### Comparing `springserve-0.8.8/springserve/_decorators.py` & `springserve-0.8.9/springserve/_decorators.py`

 * *Files identical despite different names*

### Comparing `springserve-0.8.8/springserve/_demand.py` & `springserve-0.8.9/springserve/_demand.py`

 * *Files identical despite different names*

### Comparing `springserve-0.8.8/springserve/_reporting.py` & `springserve-0.8.9/springserve/_reporting.py`

 * *Files identical despite different names*

### Comparing `springserve-0.8.8/springserve.egg-info/PKG-INFO` & `springserve-0.8.9/springserve.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: springserve
-Version: 0.8.8
+Version: 0.8.9
 Summary: API Library for console.springserve.com
 Home-page: http://www.springserve.com
 Maintainer: dave@springserve.com
 Maintainer-email: 
 License: Apache 2.0
 Description: Springserve is a video adserver, and this library allows you
         to interface with its api to do read/write and reporting requests
```

### Comparing `springserve-0.8.8/tests/__init__.py` & `springserve-0.8.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `springserve-0.8.8/tests/test_responses.py` & `springserve-0.8.9/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `springserve-0.8.8/tests/test_services.py` & `springserve-0.8.9/tests/test_services.py`

 * *Files identical despite different names*

