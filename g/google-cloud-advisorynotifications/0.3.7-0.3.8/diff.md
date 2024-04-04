# Comparing `tmp/google-cloud-advisorynotifications-0.3.7.tar.gz` & `tmp/google-cloud-advisorynotifications-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-advisorynotifications-0.3.7.tar", last modified: Tue Mar  5 18:49:40 2024, max compression
+gzip compressed data, was "google-cloud-advisorynotifications-0.3.8.tar", last modified: Thu Apr  4 18:15:16 2024, max compression
```

## Comparing `google-cloud-advisorynotifications-0.3.7.tar` & `google-cloud-advisorynotifications-0.3.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.039673 google-cloud-advisorynotifications-0.3.7/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5506 2024-03-05 18:49:40.039673 google-cloud-advisorynotifications-0.3.7/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4100 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.027668 google-cloud-advisorynotifications-0.3.7/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.027668 google-cloud-advisorynotifications-0.3.7/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.031670 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications/
--rw-rw-r--   0 root         (0)     1003     1874 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.031670 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/
--rw-rw-r--   0 root         (0)     1003     1689 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     2234 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       95 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.031670 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.035672 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/
--rw-rw-r--   0 root         (0)     1003      825 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    30114 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    47020 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py
--rw-rw-r--   0 root         (0)     1003     5956 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.035672 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/
--rw-rw-r--   0 root         (0)     1003     1617 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8184 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15231 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15537 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    27493 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.035672 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/types/
--rw-rw-r--   0 root         (0)     1003     1324 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    15892 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.035672 google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/
--rw-r--r--   0 root         (0)     1003     5506 2024-03-05 18:49:39.000000 google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1970 2024-03-05 18:49:39.000000 google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:49:39.000000 google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:49:39.000000 google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-05 18:49:39.000000 google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 18:49:39.000000 google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 18:49:40.039673 google-cloud-advisorynotifications-0.3.7/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3225 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.035672 google-cloud-advisorynotifications-0.3.7/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.035672 google-cloud-advisorynotifications-0.3.7/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.035672 google-cloud-advisorynotifications-0.3.7/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:49:40.039673 google-cloud-advisorynotifications-0.3.7/tests/unit/gapic/advisorynotifications_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/tests/unit/gapic/advisorynotifications_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   162234 2024-03-05 18:46:00.000000 google-cloud-advisorynotifications-0.3.7/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.004214 google-cloud-advisorynotifications-0.3.8/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5506 2024-04-04 18:15:16.004214 google-cloud-advisorynotifications-0.3.8/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4100 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:15.992210 google-cloud-advisorynotifications-0.3.8/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:15.992210 google-cloud-advisorynotifications-0.3.8/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:15.996211 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications/
+-rw-rw-r--   0 root         (0)     1003     1874 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:15.996211 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/
+-rw-rw-r--   0 root         (0)     1003     1689 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2234 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       95 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.000213 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.000213 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/
+-rw-rw-r--   0 root         (0)     1003      825 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30200 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    47106 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5956 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.000213 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1617 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8184 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15231 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15537 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    27838 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.000213 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1324 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16045 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.004214 google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/
+-rw-r--r--   0 root         (0)     1003     5506 2024-04-04 18:15:15.000000 google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1970 2024-04-04 18:15:15.000000 google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-04 18:15:15.000000 google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-04 18:15:15.000000 google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-04-04 18:15:15.000000 google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-04 18:15:15.000000 google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-04 18:15:16.004214 google-cloud-advisorynotifications-0.3.8/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3225 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.004214 google-cloud-advisorynotifications-0.3.8/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.004214 google-cloud-advisorynotifications-0.3.8/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.004214 google-cloud-advisorynotifications-0.3.8/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:16.004214 google-cloud-advisorynotifications-0.3.8/tests/unit/gapic/advisorynotifications_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/tests/unit/gapic/advisorynotifications_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   170659 2024-04-04 18:12:09.000000 google-cloud-advisorynotifications-0.3.8/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py
```

### Comparing `google-cloud-advisorynotifications-0.3.7/LICENSE` & `google-cloud-advisorynotifications-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.3.7/MANIFEST.in` & `google-cloud-advisorynotifications-0.3.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.3.7/PKG-INFO` & `google-cloud-advisorynotifications-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-advisorynotifications
-Version: 0.3.7
+Version: 0.3.8
 Summary: Google Cloud Advisorynotifications API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-advisorynotifications
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-advisorynotifications-0.3.7/README.rst` & `google-cloud-advisorynotifications-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications/__init__.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications/gapic_version.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.3.7"  # {x-release-please-version}
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/__init__.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/gapic_metadata.json` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/gapic_version.py` & `google-cloud-advisorynotifications-0.3.8/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.3.7"  # {x-release-please-version}
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/__init__.py` & `google-cloud-advisorynotifications-0.3.8/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -317,15 +317,15 @@
                 notifications for a given parent.
             parent (:class:`str`):
                 Required. The parent, which owns this
                 collection of notifications. Must be of
                 the form
                 "organizations/{organization}/locations/{location}"
                 or
-                "projects/{project}/locations/{location}"
+                "projects/{project}/locations/{location}".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -562,15 +562,17 @@
         Args:
             request (Optional[Union[google.cloud.advisorynotifications_v1.types.GetSettingsRequest, dict]]):
                 The request object. Request of GetSettings endpoint.
             name (:class:`str`):
                 Required. The resource name of the
                 settings to retrieve. Format:
 
-                organizations/{organization}/locations/{location}/settings.
+                organizations/{organization}/locations/{location}/settings
+                or
+                projects/{projects}/locations/{location}/settings.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -743,15 +743,15 @@
                 notifications for a given parent.
             parent (str):
                 Required. The parent, which owns this
                 collection of notifications. Must be of
                 the form
                 "organizations/{organization}/locations/{location}"
                 or
-                "projects/{project}/locations/{location}"
+                "projects/{project}/locations/{location}".
 
                 This corresponds to the ``parent`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -970,15 +970,17 @@
         Args:
             request (Union[google.cloud.advisorynotifications_v1.types.GetSettingsRequest, dict]):
                 The request object. Request of GetSettings endpoint.
             name (str):
                 Required. The resource name of the
                 settings to retrieve. Format:
 
-                organizations/{organization}/locations/{location}/settings.
+                organizations/{organization}/locations/{location}/settings
+                or
+                projects/{projects}/locations/{location}/settings.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/pagers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/services/advisory_notifications_service/transports/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -417,14 +417,18 @@
             """
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "get",
                     "uri": "/v1/{name=organizations/*/locations/*/settings}",
                 },
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*/settings}",
+                },
             ]
             request, metadata = self._interceptor.pre_get_settings(request, metadata)
             pb_request = service.GetSettingsRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             uri = transcoded_request["uri"]
             method = transcoded_request["method"]
@@ -597,14 +601,19 @@
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "patch",
                     "uri": "/v1/{settings.name=organizations/*/locations/*/settings}",
                     "body": "settings",
                 },
+                {
+                    "method": "patch",
+                    "uri": "/v1/{settings.name=projects/*/locations/*/settings}",
+                    "body": "settings",
+                },
             ]
             request, metadata = self._interceptor.pre_update_settings(request, metadata)
             pb_request = service.UpdateSettingsRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
 
             # Jsonify the request body
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/types/__init__.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google/cloud/advisorynotifications_v1/types/service.py` & `google-cloud-advisorynotifications-0.3.8/google/cloud/advisorynotifications_v1/types/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -445,18 +445,20 @@
 
 
 class Settings(proto.Message):
     r"""Settings for Advisory Notifications.
 
     Attributes:
         name (str):
-            Output only. The resource name of the
-            settings to retrieve. Format:
+            Identifier. The resource name of the settings
+            to retrieve. Format:
 
-            organizations/{organization}/locations/{location}/settings.
+            organizations/{organization}/locations/{location}/settings
+            or
+            projects/{projects}/locations/{location}/settings.
         notification_settings (MutableMapping[str, google.cloud.advisorynotifications_v1.types.NotificationSettings]):
             Required. Map of each notification type and
             its settings to get/set all settings at once.
             The server will validate the value for each
             notification type.
         etag (str):
             Required. Fingerprint for optimistic
@@ -502,15 +504,17 @@
     r"""Request of GetSettings endpoint.
 
     Attributes:
         name (str):
             Required. The resource name of the settings
             to retrieve. Format:
 
-            organizations/{organization}/locations/{location}/settings.
+            organizations/{organization}/locations/{location}/settings
+            or
+            projects/{projects}/locations/{location}/settings.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/PKG-INFO` & `google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-advisorynotifications
-Version: 0.3.7
+Version: 0.3.8
 Summary: Google Cloud Advisorynotifications API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-advisorynotifications
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-advisorynotifications-0.3.7/google_cloud_advisorynotifications.egg-info/SOURCES.txt` & `google-cloud-advisorynotifications-0.3.8/google_cloud_advisorynotifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-advisorynotifications-0.3.7/setup.py` & `google-cloud-advisorynotifications-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/tests/__init__.py` & `google-cloud-advisorynotifications-0.3.8/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/tests/unit/__init__.py` & `google-cloud-advisorynotifications-0.3.8/tests/unit/gapic/advisorynotifications_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-cloud-advisorynotifications-0.3.7/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py` & `google-cloud-advisorynotifications-0.3.8/tests/unit/gapic/advisorynotifications_v1/test_advisory_notifications_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1236,15 +1236,16 @@
             total_size=1086,
         )
         response = client.list_notifications(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == service.ListNotificationsRequest()
+        request = service.ListNotificationsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListNotificationsPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
@@ -1262,14 +1263,71 @@
     ) as call:
         client.list_notifications()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.ListNotificationsRequest()
 
 
+def test_list_notifications_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = AdvisoryNotificationsServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = service.ListNotificationsRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        language_code="language_code_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_notifications), "__call__"
+    ) as call:
+        client.list_notifications(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.ListNotificationsRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            language_code="language_code_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_notifications_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = AdvisoryNotificationsServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_notifications), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            service.ListNotificationsResponse(
+                next_page_token="next_page_token_value",
+                total_size=1086,
+            )
+        )
+        response = await client.list_notifications()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.ListNotificationsRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_notifications_async(
     transport: str = "grpc_asyncio", request_type=service.ListNotificationsRequest
 ):
     client = AdvisoryNotificationsServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1291,15 +1349,16 @@
             )
         )
         response = await client.list_notifications(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == service.ListNotificationsRequest()
+        request = service.ListNotificationsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListNotificationsAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.total_size == 1086
 
 
@@ -1682,15 +1741,16 @@
             notification_type=service.NotificationType.NOTIFICATION_TYPE_SECURITY_PRIVACY_ADVISORY,
         )
         response = client.get_notification(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == service.GetNotificationRequest()
+        request = service.GetNotificationRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Notification)
     assert response.name == "name_value"
     assert (
         response.notification_type
         == service.NotificationType.NOTIFICATION_TYPE_SECURITY_PRIVACY_ADVISORY
@@ -1709,14 +1769,65 @@
     with mock.patch.object(type(client.transport.get_notification), "__call__") as call:
         client.get_notification()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetNotificationRequest()
 
 
+def test_get_notification_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = AdvisoryNotificationsServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = service.GetNotificationRequest(
+        name="name_value",
+        language_code="language_code_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_notification), "__call__") as call:
+        client.get_notification(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.GetNotificationRequest(
+            name="name_value",
+            language_code="language_code_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_notification_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = AdvisoryNotificationsServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_notification), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            service.Notification(
+                name="name_value",
+                notification_type=service.NotificationType.NOTIFICATION_TYPE_SECURITY_PRIVACY_ADVISORY,
+            )
+        )
+        response = await client.get_notification()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.GetNotificationRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_notification_async(
     transport: str = "grpc_asyncio", request_type=service.GetNotificationRequest
 ):
     client = AdvisoryNotificationsServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1736,15 +1847,16 @@
             )
         )
         response = await client.get_notification(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == service.GetNotificationRequest()
+        request = service.GetNotificationRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Notification)
     assert response.name == "name_value"
     assert (
         response.notification_type
         == service.NotificationType.NOTIFICATION_TYPE_SECURITY_PRIVACY_ADVISORY
@@ -1924,15 +2036,16 @@
             etag="etag_value",
         )
         response = client.get_settings(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == service.GetSettingsRequest()
+        request = service.GetSettingsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Settings)
     assert response.name == "name_value"
     assert response.etag == "etag_value"
 
 
@@ -1948,14 +2061,63 @@
     with mock.patch.object(type(client.transport.get_settings), "__call__") as call:
         client.get_settings()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.GetSettingsRequest()
 
 
+def test_get_settings_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = AdvisoryNotificationsServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = service.GetSettingsRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_settings), "__call__") as call:
+        client.get_settings(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.GetSettingsRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_settings_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = AdvisoryNotificationsServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_settings), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            service.Settings(
+                name="name_value",
+                etag="etag_value",
+            )
+        )
+        response = await client.get_settings()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.GetSettingsRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_settings_async(
     transport: str = "grpc_asyncio", request_type=service.GetSettingsRequest
 ):
     client = AdvisoryNotificationsServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1975,15 +2137,16 @@
             )
         )
         response = await client.get_settings(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == service.GetSettingsRequest()
+        request = service.GetSettingsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Settings)
     assert response.name == "name_value"
     assert response.etag == "etag_value"
 
 
@@ -2156,15 +2319,16 @@
             etag="etag_value",
         )
         response = client.update_settings(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == service.UpdateSettingsRequest()
+        request = service.UpdateSettingsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Settings)
     assert response.name == "name_value"
     assert response.etag == "etag_value"
 
 
@@ -2180,14 +2344,59 @@
     with mock.patch.object(type(client.transport.update_settings), "__call__") as call:
         client.update_settings()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == service.UpdateSettingsRequest()
 
 
+def test_update_settings_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = AdvisoryNotificationsServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = service.UpdateSettingsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_settings), "__call__") as call:
+        client.update_settings(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.UpdateSettingsRequest()
+
+
+@pytest.mark.asyncio
+async def test_update_settings_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = AdvisoryNotificationsServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.update_settings), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            service.Settings(
+                name="name_value",
+                etag="etag_value",
+            )
+        )
+        response = await client.update_settings()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == service.UpdateSettingsRequest()
+
+
 @pytest.mark.asyncio
 async def test_update_settings_async(
     transport: str = "grpc_asyncio", request_type=service.UpdateSettingsRequest
 ):
     client = AdvisoryNotificationsServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2207,15 +2416,16 @@
             )
         )
         response = await client.update_settings(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == service.UpdateSettingsRequest()
+        request = service.UpdateSettingsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, service.Settings)
     assert response.name == "name_value"
     assert response.etag == "etag_value"
```

