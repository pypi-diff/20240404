# Comparing `tmp/mypy-boto3-ivs-1.34.45.tar.gz` & `tmp/mypy-boto3-ivs-1.34.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-1.34.45.tar", last modified: Mon Feb 19 20:21:46 2024, max compression
+gzip compressed data, was "mypy-boto3-ivs-1.34.78.tar", last modified: Thu Apr  4 19:33:17 2024, max compression
```

## Comparing `mypy-boto3-ivs-1.34.45.tar` & `mypy-boto3-ivs-1.34.78.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:46.026640 mypy-boto3-ivs-1.34.45/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-02-19 20:21:46.022640 mypy-boto3-ivs-1.34.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:46.022640 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26395 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    26392 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10160 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-02-19 20:21:32.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:46.022640 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-02-19 20:21:45.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-19 20:21:45.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 20:21:45.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 20:21:45.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-19 20:21:45.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-19 20:21:45.000000 mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 20:21:46.026640 mypy-boto3-ivs-1.34.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-02-19 20:21:31.000000 mypy-boto3-ivs-1.34.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.792019 mypy-boto3-ivs-1.34.78/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-04 19:33:17.792019 mypy-boto3-ivs-1.34.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11480 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.788019 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26395 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26392 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-04-04 19:33:03.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:17.788019 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 19:33:17.000000 mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:17.792019 mypy-boto3-ivs-1.34.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-04 19:33:02.000000 mypy-boto3-ivs-1.34.78/setup.py
```

### Comparing `mypy-boto3-ivs-1.34.45/LICENSE` & `mypy-boto3-ivs-1.34.78/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.45/PKG-INFO` & `mypy-boto3-ivs-1.34.78/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.34.45
-Summary: Type annotations for boto3.IVS 1.34.45 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.78
+Summary: Type annotations for boto3.IVS 1.34.78 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.34.45/README.md` & `mypy-boto3-ivs-1.34.78/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/__init__.py` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/__init__.pyi` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/__main__.py` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IVS 1.34.45\n"
-        "Version:         1.34.45\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.IVS 1.34.78\n"
+        "Version:         1.34.78\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.45")
+    print("1.34.78")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/client.py` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/client.pyi` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/literals.py` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -157,14 +158,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -225,15 +227,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -413,14 +414,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/literals.pyi` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -157,14 +158,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -225,15 +227,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -413,14 +414,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/paginator.py` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/paginator.pyi` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/type_defs.py` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
-    "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
     "BatchStartViewerSessionRevocationErrorTypeDef",
     "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
+    "SrtTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "CreatePlaybackRestrictionPolicyRequestRequestTypeDef",
     "PlaybackRestrictionPolicyTypeDef",
     "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
@@ -91,26 +91,23 @@
     "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdatePlaybackRestrictionPolicyRequestRequestTypeDef",
-    "BatchGetChannelResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "GetChannelResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
-    "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
+    "ChannelTypeDef",
     "CreatePlaybackRestrictionPolicyResponseTypeDef",
     "GetPlaybackRestrictionPolicyResponseTypeDef",
     "UpdatePlaybackRestrictionPolicyResponseTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
@@ -122,14 +119,18 @@
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListPlaybackRestrictionPoliciesResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
+    "BatchGetChannelResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "GetChannelResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
     "ListRecordingConfigurationsResponseTypeDef",
     "CreateRecordingConfigurationResponseTypeDef",
     "GetRecordingConfigurationResponseTypeDef",
     "StreamSessionTypeDef",
@@ -155,39 +156,22 @@
 )
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
-ChannelTypeDef = TypedDict(
-    "ChannelTypeDef",
-    {
-        "arn": NotRequired[str],
-        "authorized": NotRequired[bool],
-        "ingestEndpoint": NotRequired[str],
-        "insecureIngest": NotRequired[bool],
-        "latencyMode": NotRequired[ChannelLatencyModeType],
-        "name": NotRequired[str],
-        "playbackRestrictionPolicyArn": NotRequired[str],
-        "playbackUrl": NotRequired[str],
-        "preset": NotRequired[TranscodePresetType],
-        "recordingConfigurationArn": NotRequired[str],
-        "tags": NotRequired[Dict[str, str]],
-        "type": NotRequired[ChannelTypeType],
-    },
-)
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 BatchGetStreamKeyRequestRequestTypeDef = TypedDict(
     "BatchGetStreamKeyRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -229,14 +213,21 @@
         "playbackRestrictionPolicyArn": NotRequired[str],
         "preset": NotRequired[TranscodePresetType],
         "recordingConfigurationArn": NotRequired[str],
         "tags": NotRequired[Dict[str, str]],
         "type": NotRequired[ChannelTypeType],
     },
 )
+SrtTypeDef = TypedDict(
+    "SrtTypeDef",
+    {
+        "endpoint": NotRequired[str],
+        "passphrase": NotRequired[str],
+    },
+)
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": NotRequired[bool],
         "insecureIngest": NotRequired[bool],
         "latencyMode": NotRequired[ChannelLatencyModeType],
         "name": NotRequired[str],
@@ -589,65 +580,35 @@
         "arn": str,
         "allowedCountries": NotRequired[Sequence[str]],
         "allowedOrigins": NotRequired[Sequence[str]],
         "enableStrictOriginEnforcement": NotRequired[bool],
         "name": NotRequired[str],
     },
 )
-BatchGetChannelResponseTypeDef = TypedDict(
-    "BatchGetChannelResponseTypeDef",
-    {
-        "channels": List[ChannelTypeDef],
-        "errors": List[BatchErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetChannelResponseTypeDef = TypedDict(
-    "GetChannelResponseTypeDef",
-    {
-        "channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 BatchGetStreamKeyResponseTypeDef = TypedDict(
     "BatchGetStreamKeyResponseTypeDef",
     {
         "errors": List[BatchErrorTypeDef],
         "streamKeys": List[StreamKeyTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "channel": ChannelTypeDef,
-        "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateStreamKeyResponseTypeDef = TypedDict(
     "CreateStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -675,14 +636,32 @@
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ChannelTypeDef = TypedDict(
+    "ChannelTypeDef",
+    {
+        "arn": NotRequired[str],
+        "authorized": NotRequired[bool],
+        "ingestEndpoint": NotRequired[str],
+        "insecureIngest": NotRequired[bool],
+        "latencyMode": NotRequired[ChannelLatencyModeType],
+        "name": NotRequired[str],
+        "playbackRestrictionPolicyArn": NotRequired[str],
+        "playbackUrl": NotRequired[str],
+        "preset": NotRequired[TranscodePresetType],
+        "recordingConfigurationArn": NotRequired[str],
+        "srt": NotRequired[SrtTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+        "type": NotRequired[ChannelTypeType],
+    },
+)
 CreatePlaybackRestrictionPolicyResponseTypeDef = TypedDict(
     "CreatePlaybackRestrictionPolicyResponseTypeDef",
     {
         "playbackRestrictionPolicy": PlaybackRestrictionPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -813,14 +792,44 @@
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchGetChannelResponseTypeDef = TypedDict(
+    "BatchGetChannelResponseTypeDef",
+    {
+        "channels": List[ChannelTypeDef],
+        "errors": List[BatchErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "streamKey": StreamKeyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetChannelResponseTypeDef = TypedDict(
+    "GetChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecordingConfigurationRequestRequestTypeDef",
     {
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "name": NotRequired[str],
         "recordingReconnectWindowSeconds": NotRequired[int],
         "renditionConfiguration": NotRequired[RenditionConfigurationTypeDef],
```

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs/type_defs.pyi` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AudioConfigurationTypeDef",
     "BatchErrorTypeDef",
     "BatchGetChannelRequestRequestTypeDef",
-    "ChannelTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetStreamKeyRequestRequestTypeDef",
     "StreamKeyTypeDef",
     "BatchStartViewerSessionRevocationErrorTypeDef",
     "BatchStartViewerSessionRevocationViewerSessionTypeDef",
     "ChannelSummaryTypeDef",
+    "SrtTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "CreatePlaybackRestrictionPolicyRequestRequestTypeDef",
     "PlaybackRestrictionPolicyTypeDef",
     "RenditionConfigurationTypeDef",
     "ThumbnailConfigurationTypeDef",
     "CreateStreamKeyRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
@@ -91,26 +91,23 @@
     "StartViewerSessionRevocationRequestRequestTypeDef",
     "StopStreamRequestRequestTypeDef",
     "StreamEventTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdatePlaybackRestrictionPolicyRequestRequestTypeDef",
-    "BatchGetChannelResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "GetChannelResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "UpdateChannelResponseTypeDef",
     "BatchGetStreamKeyResponseTypeDef",
-    "CreateChannelResponseTypeDef",
     "CreateStreamKeyResponseTypeDef",
     "GetStreamKeyResponseTypeDef",
     "BatchStartViewerSessionRevocationResponseTypeDef",
     "BatchStartViewerSessionRevocationRequestRequestTypeDef",
     "ListChannelsResponseTypeDef",
+    "ChannelTypeDef",
     "CreatePlaybackRestrictionPolicyResponseTypeDef",
     "GetPlaybackRestrictionPolicyResponseTypeDef",
     "UpdatePlaybackRestrictionPolicyResponseTypeDef",
     "DestinationConfigurationTypeDef",
     "GetPlaybackKeyPairResponseTypeDef",
     "ImportPlaybackKeyPairResponseTypeDef",
     "GetStreamResponseTypeDef",
@@ -122,14 +119,18 @@
     "ListPlaybackKeyPairsResponseTypeDef",
     "ListPlaybackRestrictionPoliciesResponseTypeDef",
     "ListStreamKeysResponseTypeDef",
     "ListStreamSessionsResponseTypeDef",
     "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "ListStreamsResponseTypeDef",
+    "BatchGetChannelResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "GetChannelResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "CreateRecordingConfigurationRequestRequestTypeDef",
     "RecordingConfigurationSummaryTypeDef",
     "RecordingConfigurationTypeDef",
     "ListRecordingConfigurationsResponseTypeDef",
     "CreateRecordingConfigurationResponseTypeDef",
     "GetRecordingConfigurationResponseTypeDef",
     "StreamSessionTypeDef",
@@ -155,39 +156,22 @@
 )
 BatchGetChannelRequestRequestTypeDef = TypedDict(
     "BatchGetChannelRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
-ChannelTypeDef = TypedDict(
-    "ChannelTypeDef",
-    {
-        "arn": NotRequired[str],
-        "authorized": NotRequired[bool],
-        "ingestEndpoint": NotRequired[str],
-        "insecureIngest": NotRequired[bool],
-        "latencyMode": NotRequired[ChannelLatencyModeType],
-        "name": NotRequired[str],
-        "playbackRestrictionPolicyArn": NotRequired[str],
-        "playbackUrl": NotRequired[str],
-        "preset": NotRequired[TranscodePresetType],
-        "recordingConfigurationArn": NotRequired[str],
-        "tags": NotRequired[Dict[str, str]],
-        "type": NotRequired[ChannelTypeType],
-    },
-)
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 BatchGetStreamKeyRequestRequestTypeDef = TypedDict(
     "BatchGetStreamKeyRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
@@ -229,14 +213,21 @@
         "playbackRestrictionPolicyArn": NotRequired[str],
         "preset": NotRequired[TranscodePresetType],
         "recordingConfigurationArn": NotRequired[str],
         "tags": NotRequired[Dict[str, str]],
         "type": NotRequired[ChannelTypeType],
     },
 )
+SrtTypeDef = TypedDict(
+    "SrtTypeDef",
+    {
+        "endpoint": NotRequired[str],
+        "passphrase": NotRequired[str],
+    },
+)
 CreateChannelRequestRequestTypeDef = TypedDict(
     "CreateChannelRequestRequestTypeDef",
     {
         "authorized": NotRequired[bool],
         "insecureIngest": NotRequired[bool],
         "latencyMode": NotRequired[ChannelLatencyModeType],
         "name": NotRequired[str],
@@ -589,65 +580,35 @@
         "arn": str,
         "allowedCountries": NotRequired[Sequence[str]],
         "allowedOrigins": NotRequired[Sequence[str]],
         "enableStrictOriginEnforcement": NotRequired[bool],
         "name": NotRequired[str],
     },
 )
-BatchGetChannelResponseTypeDef = TypedDict(
-    "BatchGetChannelResponseTypeDef",
-    {
-        "channels": List[ChannelTypeDef],
-        "errors": List[BatchErrorTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-GetChannelResponseTypeDef = TypedDict(
-    "GetChannelResponseTypeDef",
-    {
-        "channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "channel": ChannelTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 BatchGetStreamKeyResponseTypeDef = TypedDict(
     "BatchGetStreamKeyResponseTypeDef",
     {
         "errors": List[BatchErrorTypeDef],
         "streamKeys": List[StreamKeyTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "channel": ChannelTypeDef,
-        "streamKey": StreamKeyTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CreateStreamKeyResponseTypeDef = TypedDict(
     "CreateStreamKeyResponseTypeDef",
     {
         "streamKey": StreamKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -675,14 +636,32 @@
     "ListChannelsResponseTypeDef",
     {
         "channels": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ChannelTypeDef = TypedDict(
+    "ChannelTypeDef",
+    {
+        "arn": NotRequired[str],
+        "authorized": NotRequired[bool],
+        "ingestEndpoint": NotRequired[str],
+        "insecureIngest": NotRequired[bool],
+        "latencyMode": NotRequired[ChannelLatencyModeType],
+        "name": NotRequired[str],
+        "playbackRestrictionPolicyArn": NotRequired[str],
+        "playbackUrl": NotRequired[str],
+        "preset": NotRequired[TranscodePresetType],
+        "recordingConfigurationArn": NotRequired[str],
+        "srt": NotRequired[SrtTypeDef],
+        "tags": NotRequired[Dict[str, str]],
+        "type": NotRequired[ChannelTypeType],
+    },
+)
 CreatePlaybackRestrictionPolicyResponseTypeDef = TypedDict(
     "CreatePlaybackRestrictionPolicyResponseTypeDef",
     {
         "playbackRestrictionPolicy": PlaybackRestrictionPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -813,14 +792,44 @@
     "ListStreamsResponseTypeDef",
     {
         "nextToken": str,
         "streams": List[StreamSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+BatchGetChannelResponseTypeDef = TypedDict(
+    "BatchGetChannelResponseTypeDef",
+    {
+        "channels": List[ChannelTypeDef],
+        "errors": List[BatchErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "streamKey": StreamKeyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+GetChannelResponseTypeDef = TypedDict(
+    "GetChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreateRecordingConfigurationRequestRequestTypeDef = TypedDict(
     "CreateRecordingConfigurationRequestRequestTypeDef",
     {
         "destinationConfiguration": DestinationConfigurationTypeDef,
         "name": NotRequired[str],
         "recordingReconnectWindowSeconds": NotRequired[int],
         "renditionConfiguration": NotRequired[RenditionConfigurationTypeDef],
```

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/PKG-INFO` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs
-Version: 1.34.45
-Summary: Type annotations for boto3.IVS 1.34.45 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.78
+Summary: Type annotations for boto3.IVS 1.34.78 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs)](https://pepy.tech/project/mypy-boto3-ivs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IVS 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
+[boto3.IVS 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ivs docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ivs-1.34.45/mypy_boto3_ivs.egg-info/SOURCES.txt` & `mypy-boto3-ivs-1.34.78/mypy_boto3_ivs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-1.34.45/setup.py` & `mypy-boto3-ivs-1.34.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs",
-    version="1.34.45",
+    version="1.34.78",
     packages=["mypy_boto3_ivs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.IVS 1.34.45 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.IVS 1.34.78 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

