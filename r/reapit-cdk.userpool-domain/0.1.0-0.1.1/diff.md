# Comparing `tmp/reapit-cdk.userpool-domain-0.1.0.tar.gz` & `tmp/reapit-cdk.userpool-domain-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reapit-cdk.userpool-domain-0.1.0.tar", last modified: Tue Apr  2 13:00:50 2024, max compression
+gzip compressed data, was "reapit-cdk.userpool-domain-0.1.1.tar", last modified: Thu Apr  4 15:05:18 2024, max compression
```

## Comparing `reapit-cdk.userpool-domain-0.1.0.tar` & `reapit-cdk.userpool-domain-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:50.995188 reapit-cdk.userpool-domain-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-02 13:00:50.995188 reapit-cdk.userpool-domain-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:00:50.995188 reapit-cdk.userpool-domain-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:50.991188 reapit-cdk.userpool-domain-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:50.991188 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:50.991188 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk/userpool_domain/
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk/userpool_domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:50.995188 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk/userpool_domain/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk/userpool_domain/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   105317 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk/userpool_domain/_jsii/userpool-domain@0.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:00:42.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk/userpool_domain/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:00:50.991188 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk.userpool_domain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-02 13:00:50.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk.userpool_domain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-02 13:00:50.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk.userpool_domain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:00:50.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk.userpool_domain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 13:00:50.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk.userpool_domain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:00:50.000000 reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk.userpool_domain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:05:18.522714 reapit-cdk.userpool-domain-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-04 15:05:18.522714 reapit-cdk.userpool-domain-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:05:18.522714 reapit-cdk.userpool-domain-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:05:18.518714 reapit-cdk.userpool-domain-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:05:18.518714 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:05:18.522714 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk/userpool_domain/
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk/userpool_domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:05:18.522714 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk/userpool_domain/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk/userpool_domain/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104851 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk/userpool_domain/_jsii/userpool-domain@0.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:05:10.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk/userpool_domain/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:05:18.522714 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk.userpool_domain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-04 15:05:18.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk.userpool_domain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-04 15:05:18.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk.userpool_domain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:05:18.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk.userpool_domain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 15:05:18.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk.userpool_domain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 15:05:18.000000 reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk.userpool_domain.egg-info/top_level.txt
```

### Comparing `reapit-cdk.userpool-domain-0.1.0/LICENSE` & `reapit-cdk.userpool-domain-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reapit-cdk.userpool-domain-0.1.0/PKG-INFO` & `reapit-cdk.userpool-domain-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.userpool-domain
-Version: 0.1.0
+Version: 0.1.1
 Summary: This construct returns the given Cognito UserPool's UserPoolDomain, or creates one. This resolves an issue with [AWS::Cognito::UserPoolDomain](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-cognito-userpooldomain.html), since that will fail if one already exists.
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/userpool-domain
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.userpool-domain-0.1.0/README.md` & `reapit-cdk.userpool-domain-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `reapit-cdk.userpool-domain-0.1.0/setup.py` & `reapit-cdk.userpool-domain-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "reapit-cdk.userpool-domain",
-    "version": "0.1.0",
+    "version": "0.1.1",
     "description": "This construct returns the given Cognito UserPool's UserPoolDomain, or creates one. This resolves an issue with [AWS::Cognito::UserPoolDomain](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-cognito-userpooldomain.html), since that will fail if one already exists.",
     "license": "MIT",
     "url": "https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/userpool-domain",
     "long_description_content_type": "text/markdown",
     "author": "Josh Balfour<jbalfour@reapit.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "reapit_cdk.userpool_domain",
         "reapit_cdk.userpool_domain._jsii"
     ],
     "package_data": {
         "reapit_cdk.userpool_domain._jsii": [
-            "userpool-domain@0.1.0.jsii.tgz"
+            "userpool-domain@0.1.1.jsii.tgz"
         ],
         "reapit_cdk.userpool_domain": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk/userpool_domain/__init__.py` & `reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk/userpool_domain/__init__.py`

 * *Files identical despite different names*

### Comparing `reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk.userpool_domain.egg-info/PKG-INFO` & `reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk.userpool_domain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reapit-cdk.userpool-domain
-Version: 0.1.0
+Version: 0.1.1
 Summary: This construct returns the given Cognito UserPool's UserPoolDomain, or creates one. This resolves an issue with [AWS::Cognito::UserPoolDomain](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-cognito-userpooldomain.html), since that will fail if one already exists.
 Home-page: https://github.com/reapit/ts-cdk-constructs/blob/main/packages/constructs/userpool-domain
 Author: Josh Balfour<jbalfour@reapit.com>
 License: MIT
 Project-URL: Source, https://github.com/reapit/ts-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `reapit-cdk.userpool-domain-0.1.0/src/reapit_cdk.userpool_domain.egg-info/SOURCES.txt` & `reapit-cdk.userpool-domain-0.1.1/src/reapit_cdk.userpool_domain.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/reapit_cdk.userpool_domain.egg-info/SOURCES.txt
 src/reapit_cdk.userpool_domain.egg-info/dependency_links.txt
 src/reapit_cdk.userpool_domain.egg-info/requires.txt
 src/reapit_cdk.userpool_domain.egg-info/top_level.txt
 src/reapit_cdk/userpool_domain/__init__.py
 src/reapit_cdk/userpool_domain/py.typed
 src/reapit_cdk/userpool_domain/_jsii/__init__.py
-src/reapit_cdk/userpool_domain/_jsii/userpool-domain@0.1.0.jsii.tgz
+src/reapit_cdk/userpool_domain/_jsii/userpool-domain@0.1.1.jsii.tgz
```

