# Comparing `tmp/botocore-a-la-carte-chime-sdk-voice-1.34.8.tar.gz` & `tmp/botocore-a-la-carte-chime-sdk-voice-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-chime-sdk-voice-1.34.8.tar", last modified: Wed Dec 27 01:06:32 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-chime-sdk-voice-1.34.9.tar", last modified: Thu Dec 28 01:06:33 2023, max compression
```

## Comparing `botocore-a-la-carte-chime-sdk-voice-1.34.8.tar` & `botocore-a-la-carte-chime-sdk-voice-1.34.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:32.451296 botocore-a-la-carte-chime-sdk-voice-1.34.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-27 01:06:32.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-27 01:06:32.451296 botocore-a-la-carte-chime-sdk-voice-1.34.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:32.447296 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:32.447296 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:32.447296 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/data/chime-sdk-voice/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:32.451296 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/data/chime-sdk-voice/2022-08-03/
--rw-r--r--   0 runner    (1001) docker     (127)    17644 2023-12-27 01:06:28.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/data/chime-sdk-voice/2022-08-03/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-27 01:06:28.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/data/chime-sdk-voice/2022-08-03/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   217018 2023-12-27 01:06:28.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/data/chime-sdk-voice/2022-08-03/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:32.451296 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore_a_la_carte_chime_sdk_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-27 01:06:32.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore_a_la_carte_chime_sdk_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-27 01:06:32.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore_a_la_carte_chime_sdk_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 01:06:32.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore_a_la_carte_chime_sdk_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 01:06:32.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore_a_la_carte_chime_sdk_voice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 01:06:32.451296 botocore-a-la-carte-chime-sdk-voice-1.34.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-12-27 01:06:32.000000 botocore-a-la-carte-chime-sdk-voice-1.34.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:33.890218 botocore-a-la-carte-chime-sdk-voice-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:33.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-28 01:06:33.890218 botocore-a-la-carte-chime-sdk-voice-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:33.886218 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:33.886218 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:33.886218 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/data/chime-sdk-voice/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:33.890218 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/data/chime-sdk-voice/2022-08-03/
+-rw-r--r--   0 runner    (1001) docker     (127)    17644 2023-12-28 01:06:26.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/data/chime-sdk-voice/2022-08-03/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-28 01:06:26.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/data/chime-sdk-voice/2022-08-03/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   217018 2023-12-28 01:06:26.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/data/chime-sdk-voice/2022-08-03/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:33.890218 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore_a_la_carte_chime_sdk_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2023-12-28 01:06:33.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore_a_la_carte_chime_sdk_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-12-28 01:06:33.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore_a_la_carte_chime_sdk_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:33.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore_a_la_carte_chime_sdk_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:33.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore_a_la_carte_chime_sdk_voice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:33.890218 botocore-a-la-carte-chime-sdk-voice-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-12-28 01:06:33.000000 botocore-a-la-carte-chime-sdk-voice-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-chime-sdk-voice-1.34.8/LICENSE.txt` & `botocore-a-la-carte-chime-sdk-voice-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-chime-sdk-voice-1.34.8/PKG-INFO` & `botocore-a-la-carte-chime-sdk-voice-1.34.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-chime-sdk-voice
-Version: 1.34.8
+Version: 1.34.9
 Summary: chime-sdk-voice data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/data/chime-sdk-voice/2022-08-03/endpoint-rule-set-1.json` & `botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/data/chime-sdk-voice/2022-08-03/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore/data/chime-sdk-voice/2022-08-03/service-2.json` & `botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore/data/chime-sdk-voice/2022-08-03/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-chime-sdk-voice-1.34.8/botocore_a_la_carte_chime_sdk_voice.egg-info/PKG-INFO` & `botocore-a-la-carte-chime-sdk-voice-1.34.9/botocore_a_la_carte_chime_sdk_voice.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-chime-sdk-voice
-Version: 1.34.8
+Version: 1.34.9
 Summary: chime-sdk-voice data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-chime-sdk-voice-1.34.8/setup.py` & `botocore-a-la-carte-chime-sdk-voice-1.34.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-chime-sdk-voice',
-    version="1.34.8",
+    version="1.34.9",
     description='chime-sdk-voice data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/chime-sdk-voice/*/*.json'],
```

