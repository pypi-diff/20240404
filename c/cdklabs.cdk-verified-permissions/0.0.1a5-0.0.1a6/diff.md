# Comparing `tmp/cdklabs.cdk-verified-permissions-0.0.1a5.tar.gz` & `tmp/cdklabs.cdk-verified-permissions-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-verified-permissions-0.0.1a5.tar", last modified: Wed Apr  3 06:51:06 2024, max compression
+gzip compressed data, was "cdklabs.cdk-verified-permissions-0.0.1a6.tar", last modified: Thu Apr  4 16:17:03 2024, max compression
```

## Comparing `cdklabs.cdk-verified-permissions-0.0.1a5.tar` & `cdklabs.cdk-verified-permissions-0.0.1a6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:51:06.709061 cdklabs.cdk-verified-permissions-0.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-03 06:51:06.709061 cdklabs.cdk-verified-permissions-0.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:51:06.709061 cdklabs.cdk-verified-permissions-0.0.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:51:06.705061 cdklabs.cdk-verified-permissions-0.0.1a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:51:06.705061 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:51:06.709061 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/cdk_verified_permissions/
--rw-r--r--   0 runner    (1001) docker     (127)   107624 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/cdk_verified_permissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:51:06.709061 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/cdk_verified_permissions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55489 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.5.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:50:52.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/cdk_verified_permissions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:51:06.705061 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs.cdk_verified_permissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-03 06:51:06.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 06:51:06.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:51:06.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 06:51:06.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 06:51:06.000000 cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:03.748558 cdklabs.cdk-verified-permissions-0.0.1a6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-04 16:17:03.748558 cdklabs.cdk-verified-permissions-0.0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:17:03.748558 cdklabs.cdk-verified-permissions-0.0.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:03.748558 cdklabs.cdk-verified-permissions-0.0.1a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:03.748558 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:03.748558 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/cdk_verified_permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)   107624 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/cdk_verified_permissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:03.748558 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/cdk_verified_permissions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55514 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.6.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:16:53.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/cdk_verified_permissions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:03.748558 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs.cdk_verified_permissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-04 16:17:03.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 16:17:03.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:17:03.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 16:17:03.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 16:17:03.000000 cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a5/LICENSE` & `cdklabs.cdk-verified-permissions-0.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a5/PKG-INFO` & `cdklabs.cdk-verified-permissions-0.0.1a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-verified-permissions
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: L2 AWS CDK Constructs for Amazon Verified Permissions
 Home-page: https://github.com/cdklabs/cdk-verified-permissions.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-verified-permissions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a5/README.md` & `cdklabs.cdk-verified-permissions-0.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a5/setup.py` & `cdklabs.cdk-verified-permissions-0.0.1a6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-verified-permissions",
-    "version": "0.0.1.a5",
+    "version": "0.0.1.a6",
     "description": "L2 AWS CDK Constructs for Amazon Verified Permissions",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-verified-permissions.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "cdklabs.cdk_verified_permissions",
         "cdklabs.cdk_verified_permissions._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_verified_permissions._jsii": [
-            "cdk-verified-permissions@0.0.1-alpha.5.jsii.tgz"
+            "cdk-verified-permissions@0.0.1-alpha.6.jsii.tgz"
         ],
         "cdklabs.cdk_verified_permissions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.134.0, <3.0.0",
+        "aws-cdk-lib>=2.135.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/cdk_verified_permissions/__init__.py` & `cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/cdk_verified_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py` & `cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs/cdk_verified_permissions/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdklabs/cdk-verified-permissions",
-    "0.0.1-alpha.5",
+    "0.0.1-alpha.6",
     __name__[0:-6],
-    "cdk-verified-permissions@0.0.1-alpha.5.jsii.tgz",
+    "cdk-verified-permissions@0.0.1-alpha.6.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO` & `cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs.cdk_verified_permissions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-verified-permissions
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: L2 AWS CDK Constructs for Amazon Verified Permissions
 Home-page: https://github.com/cdklabs/cdk-verified-permissions.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-verified-permissions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-verified-permissions-0.0.1a5/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt` & `cdklabs.cdk-verified-permissions-0.0.1a6/src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdklabs.cdk_verified_permissions.egg-info/SOURCES.txt
 src/cdklabs.cdk_verified_permissions.egg-info/dependency_links.txt
 src/cdklabs.cdk_verified_permissions.egg-info/requires.txt
 src/cdklabs.cdk_verified_permissions.egg-info/top_level.txt
 src/cdklabs/cdk_verified_permissions/__init__.py
 src/cdklabs/cdk_verified_permissions/py.typed
 src/cdklabs/cdk_verified_permissions/_jsii/__init__.py
-src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.5.jsii.tgz
+src/cdklabs/cdk_verified_permissions/_jsii/cdk-verified-permissions@0.0.1-alpha.6.jsii.tgz
```

