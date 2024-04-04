# Comparing `tmp/google-cloud-storage-control-0.1.1.tar.gz` & `tmp/google-cloud-storage-control-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-storage-control-0.1.1.tar", last modified: Wed Apr  3 01:22:09 2024, max compression
+gzip compressed data, was "google-cloud-storage-control-0.1.2.tar", last modified: Thu Apr  4 18:15:48 2024, max compression
```

## Comparing `google-cloud-storage-control-0.1.1.tar` & `google-cloud-storage-control-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5200 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3812 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.262756 google-cloud-storage-control-0.1.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.262756 google-cloud-storage-control-0.1.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.266756 google-cloud-storage-control-0.1.1/google/cloud/storage_control/
--rw-rw-r--   0 root         (0)     1003     2064 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/
--rw-rw-r--   0 root         (0)     1003     1899 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3061 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/
--rw-rw-r--   0 root         (0)     1003      769 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/__init__.py
--rw-rw-r--   0 root         (0)     1003    58574 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/async_client.py
--rw-rw-r--   0 root         (0)     1003    78950 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/client.py
--rw-rw-r--   0 root         (0)     1003    11060 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    14186 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/base.py
--rw-rw-r--   0 root         (0)     1003    22977 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    23517 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/
--rw-rw-r--   0 root         (0)     1003     1624 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    27732 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/storage_control.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/
--rw-r--r--   0 root         (0)     1003     5200 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1590 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3201 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/
--rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   194411 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/test_storage_control.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5526 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4138 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.522830 google-cloud-storage-control-0.1.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.522830 google-cloud-storage-control-0.1.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.526831 google-cloud-storage-control-0.1.2/google/cloud/storage_control/
+-rw-rw-r--   0 root         (0)     1003     2064 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.526831 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/
+-rw-rw-r--   0 root         (0)     1003     1899 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3061 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.526831 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.530833 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/
+-rw-rw-r--   0 root         (0)     1003      769 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/__init__.py
+-rw-rw-r--   0 root         (0)     1003    58574 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/async_client.py
+-rw-rw-r--   0 root         (0)     1003    78950 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/client.py
+-rw-rw-r--   0 root         (0)     1003    11060 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.530833 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14186 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22977 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23517 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.530833 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1624 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27732 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/storage_control.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.530833 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/
+-rw-r--r--   0 root         (0)     1003     5526 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1590 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-04 18:15:48.000000 google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3201 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-04 18:15:48.534834 google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   194411 2024-04-04 18:12:11.000000 google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/test_storage_control.py
```

### Comparing `google-cloud-storage-control-0.1.1/LICENSE` & `google-cloud-storage-control-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/MANIFEST.in` & `google-cloud-storage-control-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/PKG-INFO` & `google-cloud-storage-control-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-control
-Version: 0.1.1
+Version: 0.1.2
 Summary: Google Cloud Storage Control API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -23,47 +23,47 @@
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.1
 Requires-Dist: google-auth!=2.24.0,!=2.25.0,<3.0.0dev,>=2.14.1
 Requires-Dist: proto-plus<2.0.0dev,>=1.22.3
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 
-Python Client for Cloud Storage
-===============================
+Python Client for Storage Control API
+=====================================
 
 |preview| |pypi| |versions|
 
-`Cloud Storage`_: Lets you store and retrieve potentially-large, immutable data objects.
+`Storage Control API`_: Lets you perform metadata-specific, control plane, and long-running operations apart from the Storage API. Separating these operations from the Storage API improves API standardization and lets you run faster releases.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-storage-control.svg
    :target: https://pypi.org/project/google-cloud-storage-control/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-storage-control.svg
    :target: https://pypi.org/project/google-cloud-storage-control/
-.. _Cloud Storage: https://cloud.google.com/storage/docs/overview
+.. _Storage Control API: https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/google-cloud-storage-control/latest
-.. _Product Documentation:  https://cloud.google.com/storage/docs/overview
+.. _Product Documentation:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Storage.`_
+3. `Enable the Storage Control API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Storage.:  https://cloud.google.com/storage/docs/overview
+.. _Enable the Storage Control API.:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
 creates isolated Python environments. These isolated environments can have separate
@@ -122,16 +122,16 @@
     py -m venv <your-env>
     .\<your-env>\Scripts\activate
     pip install google-cloud-storage-control
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Storage
+-  Read the `Client Library Documentation`_ for Storage Control API
    to see other available methods on the client.
--  Read the `Cloud Storage Product documentation`_ to learn
+-  Read the `Storage Control API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Storage Product documentation:  https://cloud.google.com/storage/docs/overview
+.. _Storage Control API Product documentation:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-storage-control-0.1.1/README.rst` & `google-cloud-storage-control-0.1.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Cloud Storage
-===============================
+Python Client for Storage Control API
+=====================================
 
 |preview| |pypi| |versions|
 
-`Cloud Storage`_: Lets you store and retrieve potentially-large, immutable data objects.
+`Storage Control API`_: Lets you perform metadata-specific, control plane, and long-running operations apart from the Storage API. Separating these operations from the Storage API improves API standardization and lets you run faster releases.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-storage-control.svg
    :target: https://pypi.org/project/google-cloud-storage-control/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-storage-control.svg
    :target: https://pypi.org/project/google-cloud-storage-control/
-.. _Cloud Storage: https://cloud.google.com/storage/docs/overview
+.. _Storage Control API: https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/google-cloud-storage-control/latest
-.. _Product Documentation:  https://cloud.google.com/storage/docs/overview
+.. _Product Documentation:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Storage.`_
+3. `Enable the Storage Control API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Storage.:  https://cloud.google.com/storage/docs/overview
+.. _Enable the Storage Control API.:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
 creates isolated Python environments. These isolated environments can have separate
@@ -93,16 +93,16 @@
     py -m venv <your-env>
     .\<your-env>\Scripts\activate
     pip install google-cloud-storage-control
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Storage
+-  Read the `Client Library Documentation`_ for Storage Control API
    to see other available methods on the client.
--  Read the `Cloud Storage Product documentation`_ to learn
+-  Read the `Storage Control API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Storage Product documentation:  https://cloud.google.com/storage/docs/overview
+.. _Storage Control API Product documentation:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control/__init__.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control/gapic_version.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.1"  # {x-release-please-version}
+__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/__init__.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/gapic_metadata.json` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/gapic_version.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.1"  # {x-release-please-version}
+__version__ = "0.1.2"  # {x-release-please-version}
```

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/__init__.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/__init__.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/async_client.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/client.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/pagers.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/base.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/__init__.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/storage_control.py` & `google-cloud-storage-control-0.1.2/google/cloud/storage_control_v2/types/storage_control.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/PKG-INFO` & `google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-control
-Version: 0.1.1
+Version: 0.1.2
 Summary: Google Cloud Storage Control API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
@@ -23,47 +23,47 @@
 Requires-Python: >=3.7
 License-File: LICENSE
 Requires-Dist: google-api-core[grpc]!=2.0.*,!=2.1.*,!=2.10.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,<3.0.0dev,>=1.34.1
 Requires-Dist: google-auth!=2.24.0,!=2.25.0,<3.0.0dev,>=2.14.1
 Requires-Dist: proto-plus<2.0.0dev,>=1.22.3
 Requires-Dist: protobuf!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5,<5.0.0dev,>=3.19.5
 
-Python Client for Cloud Storage
-===============================
+Python Client for Storage Control API
+=====================================
 
 |preview| |pypi| |versions|
 
-`Cloud Storage`_: Lets you store and retrieve potentially-large, immutable data objects.
+`Storage Control API`_: Lets you perform metadata-specific, control plane, and long-running operations apart from the Storage API. Separating these operations from the Storage API improves API standardization and lets you run faster releases.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-storage-control.svg
    :target: https://pypi.org/project/google-cloud-storage-control/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-storage-control.svg
    :target: https://pypi.org/project/google-cloud-storage-control/
-.. _Cloud Storage: https://cloud.google.com/storage/docs/overview
+.. _Storage Control API: https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/google-cloud-storage-control/latest
-.. _Product Documentation:  https://cloud.google.com/storage/docs/overview
+.. _Product Documentation:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Cloud Storage.`_
+3. `Enable the Storage Control API.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Cloud Storage.:  https://cloud.google.com/storage/docs/overview
+.. _Enable the Storage Control API.:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a virtual environment using `venv`_. `venv`_ is a tool that
 creates isolated Python environments. These isolated environments can have separate
@@ -122,16 +122,16 @@
     py -m venv <your-env>
     .\<your-env>\Scripts\activate
     pip install google-cloud-storage-control
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Cloud Storage
+-  Read the `Client Library Documentation`_ for Storage Control API
    to see other available methods on the client.
--  Read the `Cloud Storage Product documentation`_ to learn
+-  Read the `Storage Control API Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Cloud Storage Product documentation:  https://cloud.google.com/storage/docs/overview
+.. _Storage Control API Product documentation:  https://cloud.google.com/storage/docs/reference/rpc/google.storage.control.v2
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/SOURCES.txt` & `google-cloud-storage-control-0.1.2/google_cloud_storage_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/setup.py` & `google-cloud-storage-control-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/tests/__init__.py` & `google-cloud-storage-control-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/tests/unit/__init__.py` & `google-cloud-storage-control-0.1.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/tests/unit/gapic/__init__.py` & `google-cloud-storage-control-0.1.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/__init__.py` & `google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/test_storage_control.py` & `google-cloud-storage-control-0.1.2/tests/unit/gapic/storage_control_v2/test_storage_control.py`

 * *Files identical despite different names*

