# Comparing `tmp/pulumi-runpod-1.1.8.tar.gz` & `tmp/pulumi-runpod-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi-runpod-1.1.8.tar", last modified: Sat Mar 30 00:18:21 2024, max compression
+gzip compressed data, was "pulumi-runpod-1.2.4.tar", last modified: Thu Apr  4 01:43:35 2024, max compression
```

## Comparing `pulumi-runpod-1.1.8.tar` & `pulumi-runpod-1.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:18:21.693687 pulumi-runpod-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-30 00:18:21.693687 pulumi-runpod-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:18:21.689687 pulumi-runpod-1.1.8/pulumi-runpod/
--rw-------   0 runner    (1001) docker     (127)      929 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1918 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9279 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:18:21.689687 pulumi-runpod-1.1.8/pulumi-runpod/config/
--rw-------   0 runner    (1001) docker     (127)      267 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      564 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/config/vars.py
--rw-------   0 runner    (1001) docker     (127)     6351 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/network_storage.py
--rw-------   0 runner    (1001) docker     (127)    18526 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/outputs.py
--rw-------   0 runner    (1001) docker     (127)    31793 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/pod.py
--rw-------   0 runner    (1001) docker     (127)     3631 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/provider.py
--rw-------   0 runner    (1001) docker     (127)      110 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi-runpod/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 00:18:21.693687 pulumi-runpod-1.1.8/pulumi_runpod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi_runpod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi_runpod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi_runpod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi_runpod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi_runpod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/pulumi_runpod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 00:18:21.693687 pulumi-runpod-1.1.8/setup.cfg
--rw-------   0 runner    (1001) docker     (127)     1311 2024-03-30 00:18:21.000000 pulumi-runpod-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:43:35.544618 pulumi-runpod-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-04 01:43:35.544618 pulumi-runpod-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:43:35.544618 pulumi-runpod-1.2.4/pulumi-runpod/
+-rw-------   0 runner    (1001) docker     (127)      929 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1918 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9279 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:43:35.544618 pulumi-runpod-1.2.4/pulumi-runpod/config/
+-rw-------   0 runner    (1001) docker     (127)      267 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      564 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/config/vars.py
+-rw-------   0 runner    (1001) docker     (127)     6351 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/network_storage.py
+-rw-------   0 runner    (1001) docker     (127)    18526 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    31793 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/pod.py
+-rw-------   0 runner    (1001) docker     (127)     3631 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/provider.py
+-rw-------   0 runner    (1001) docker     (127)      110 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi-runpod/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:43:35.544618 pulumi-runpod-1.2.4/pulumi_runpod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi_runpod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi_runpod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi_runpod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi_runpod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi_runpod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/pulumi_runpod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:43:35.544618 pulumi-runpod-1.2.4/setup.cfg
+-rw-------   0 runner    (1001) docker     (127)     1311 2024-04-04 01:43:35.000000 pulumi-runpod-1.2.4/setup.py
```

### Comparing `pulumi-runpod-1.1.8/PKG-INFO` & `pulumi-runpod-1.2.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-runpod
-Version: 1.1.8
+Version: 1.2.4
 Summary: The Runpod Pulumi provider provides resources to interact with Runpod's native APIs.
 Home-page: https://runpod.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/runpod/pulumi-runpod-native
 Keywords: pulumi runpod gpus ml ai
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -25,18 +25,33 @@
 
 ```bash
   pulumi config set --secret runpod:token
 ```
 
 ## Example
 
-This is an example of how to deploy over typescript. We also serve pulumi over Python and Go. For more examples, please go through the examples folder or the documents inside
-docs. 
+This is an example of how to deploy it over Golang. We also serve pulumi over Typescript and Python. For more examples, please navigate to the examples directory
+or the documents inside docs. If you have any problems in doing so, please contact support@runpod.io.
 
-Filename must be index.ts.
+1. Create a new Pulumi Go example:
+```
+    pulumi new
+```
+Select either the Go template or Runpod's Go template.
+
+2. Set your API keys using the config shown above. 
+
+3. Install the official Go package:
+
+```
+    go get github.com/runpod/pulumi-runpod-native/sdk/go/runpod@v1.1.8
+```
+Replace the version above to any that you want. We advise you to pin a certain version as there will be fewer breaking changes.
+
+4. Use this example as a simple building guide for your example project:
 
 ```typescript
     import * as pulumi from "@pulumi/pulumi";
     import * as runpod from "@runpod-infra/pulumi";
 
     const testNetworkStorage = new runpod.NetworkStorage("testNetworkStorage", {
         name: "testStorage1",
@@ -66,9 +81,25 @@
         value: myRandomPod.pod,
     };
     export const networkStorage = {
         value: testNetworkStorage.networkStorage,
     };
 ```
 
+5. PULUMI UP
+Create your resources using the command below:
+
+```
+    pulumi up
+```
+
+6. PULUMI DOWN
+If you want to remove your resources, you can use the command below:
+
+```
+    pulumi down
+```
+
+If you have any issues, please feel free to create an issue or reach out to us directly at support@runpod.io.
+
 > **Note:** For examples in Go and Python, please visit the documentation inside the docs directory or click [here](https://github.com/runpod/pulumi-runpod-native/tree/main/docs).
```

### Comparing `pulumi-runpod-1.1.8/pulumi-runpod/__init__.py` & `pulumi-runpod-1.2.4/pulumi-runpod/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/pulumi-runpod/_inputs.py` & `pulumi-runpod-1.2.4/pulumi-runpod/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/pulumi-runpod/_utilities.py` & `pulumi-runpod-1.2.4/pulumi-runpod/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/pulumi-runpod/config/vars.py` & `pulumi-runpod-1.2.4/pulumi-runpod/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/pulumi-runpod/network_storage.py` & `pulumi-runpod-1.2.4/pulumi-runpod/network_storage.py`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/pulumi-runpod/outputs.py` & `pulumi-runpod-1.2.4/pulumi-runpod/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/pulumi-runpod/pod.py` & `pulumi-runpod-1.2.4/pulumi-runpod/pod.py`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/pulumi-runpod/provider.py` & `pulumi-runpod-1.2.4/pulumi-runpod/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/pulumi_runpod.egg-info/PKG-INFO` & `pulumi-runpod-1.2.4/pulumi_runpod.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-runpod
-Version: 1.1.8
+Version: 1.2.4
 Summary: The Runpod Pulumi provider provides resources to interact with Runpod's native APIs.
 Home-page: https://runpod.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/runpod/pulumi-runpod-native
 Keywords: pulumi runpod gpus ml ai
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -25,18 +25,33 @@
 
 ```bash
   pulumi config set --secret runpod:token
 ```
 
 ## Example
 
-This is an example of how to deploy over typescript. We also serve pulumi over Python and Go. For more examples, please go through the examples folder or the documents inside
-docs. 
+This is an example of how to deploy it over Golang. We also serve pulumi over Typescript and Python. For more examples, please navigate to the examples directory
+or the documents inside docs. If you have any problems in doing so, please contact support@runpod.io.
 
-Filename must be index.ts.
+1. Create a new Pulumi Go example:
+```
+    pulumi new
+```
+Select either the Go template or Runpod's Go template.
+
+2. Set your API keys using the config shown above. 
+
+3. Install the official Go package:
+
+```
+    go get github.com/runpod/pulumi-runpod-native/sdk/go/runpod@v1.1.8
+```
+Replace the version above to any that you want. We advise you to pin a certain version as there will be fewer breaking changes.
+
+4. Use this example as a simple building guide for your example project:
 
 ```typescript
     import * as pulumi from "@pulumi/pulumi";
     import * as runpod from "@runpod-infra/pulumi";
 
     const testNetworkStorage = new runpod.NetworkStorage("testNetworkStorage", {
         name: "testStorage1",
@@ -66,9 +81,25 @@
         value: myRandomPod.pod,
     };
     export const networkStorage = {
         value: testNetworkStorage.networkStorage,
     };
 ```
 
+5. PULUMI UP
+Create your resources using the command below:
+
+```
+    pulumi up
+```
+
+6. PULUMI DOWN
+If you want to remove your resources, you can use the command below:
+
+```
+    pulumi down
+```
+
+If you have any issues, please feel free to create an issue or reach out to us directly at support@runpod.io.
+
 > **Note:** For examples in Go and Python, please visit the documentation inside the docs directory or click [here](https://github.com/runpod/pulumi-runpod-native/tree/main/docs).
```

### Comparing `pulumi-runpod-1.1.8/pulumi_runpod.egg-info/SOURCES.txt` & `pulumi-runpod-1.2.4/pulumi_runpod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi-runpod-1.1.8/setup.py` & `pulumi-runpod-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.1.8"
+VERSION = "1.2.4"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "runpod Pulumi Package - Development Version"
```

