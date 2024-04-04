# Comparing `tmp/ding_api_client-3.4.0.tar.gz` & `tmp/ding_api_client-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ding_api_client-3.4.0.tar", last modified: Wed Apr  3 00:11:57 2024, max compression
+gzip compressed data, was "ding_api_client-3.4.1.tar", last modified: Thu Apr  4 00:12:36 2024, max compression
```

## Comparing `ding_api_client-3.4.0.tar` & `ding_api_client-3.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.745812 ding_api_client-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/createauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/createauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/createcheckrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/createcheckresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/feedbackrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/feedbackresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/lookupresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/retryauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/retryauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/errors/errorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/src/ding/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/create_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/src/ding/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/src/ding_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:12:36.864558 ding_api_client-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.856557 ding_api_client-3.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.856557 ding_api_client-3.4.1/src/ding/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.856557 ding_api_client-3.4.1/src/ding/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.856557 ding_api_client-3.4.1/src/ding/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/createauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/createauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/createcheckrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/createcheckresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/feedbackrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/feedbackresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/lookupresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/retryauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/retryauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/errors/errorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/create_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/top_level.txt
```

### Comparing `ding_api_client-3.4.0/PKG-INFO` & `ding_api_client-3.4.1/src/ding_api_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ding_api_client
-Version: 3.4.0
+Name: ding-api-client
+Version: 3.4.1
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
@@ -101,24 +101,24 @@
         
         ```
         <!-- End SDK Example Usage [usage] -->
         
         <!-- Start Available Resources and Operations [operations] -->
         ## Available Resources and Operations
         
-        ### [otp](docs/sdks/otp/README.md)
+        ### [otp](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md)
         
-        * [create_authentication](docs/sdks/otp/README.md#create_authentication) - Send a code
-        * [check](docs/sdks/otp/README.md#check) - Check a code
-        * [feedback](docs/sdks/otp/README.md#feedback) - Send feedback
-        * [retry](docs/sdks/otp/README.md#retry) - Perform a retry
+        * [create_authentication](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md#create_authentication) - Send a code
+        * [check](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md#check) - Check a code
+        * [feedback](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md#feedback) - Send feedback
+        * [retry](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md#retry) - Perform a retry
         
-        ### [lookup](docs/sdks/lookup/README.md)
+        ### [lookup](https://github.com/ding-live/ding-python/blob/master/docs/sdks/lookup/README.md)
         
-        * [lookup](docs/sdks/lookup/README.md#lookup) - Perform a phone number lookup
+        * [lookup](https://github.com/ding-live/ding-python/blob/master/docs/sdks/lookup/README.md#lookup) - Perform a phone number lookup
         <!-- End Available Resources and Operations [operations] -->
         
         <!-- Start Error Handling [errors] -->
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
```

### Comparing `ding_api_client-3.4.0/README.md` & `ding_api_client-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/setup.py` & `ding_api_client-3.4.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import setuptools
+import re
 
 try:
-    with open("README.md", "r") as fh:
+    with open('README.md', 'r') as fh:
         long_description = fh.read()
+        GITHUB_URL = 'https://github.com/ding-live/ding-python.git'
+        GITHUB_URL = GITHUB_URL[: -len('.git')] if GITHUB_URL.endswith('.git') else GITHUB_URL
+        # links on PyPI should have absolute URLs
+        long_description = re.sub(
+            r'(\[[^\]]+\]\()((?!https?:)[^\)]+)(\))',
+            lambda m: m.group(1) + GITHUB_URL + '/blob/master/' + m.group(2) + m.group(3),
+            long_description,
+        )
 except FileNotFoundError:
-    long_description = ""
+    long_description = ''
 
 setuptools.setup(
-    name="ding_api_client",
-    version="3.4.0",
-    author="Ding",
-    description="Python Client SDK",
-    url="https://github.com/ding-live/ding-python.git",
+    name='ding_api_client',
+    version='3.4.1',
+    author='Ding',
+    description='Python Client SDK',
+    url='https://github.com/ding-live/ding-python.git',
     long_description=long_description,
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(where="src"),
+    long_description_content_type='text/markdown',
+    packages=setuptools.find_packages(where='src'),
     install_requires=[
         "certifi>=2023.7.22",
         "charset-normalizer>=3.2.0",
         "dataclasses-json>=0.6.4",
         "idna>=3.4",
         "jsonpath-python>=1.0.6",
         "marshmallow>=3.19.0",
@@ -36,9 +45,9 @@
     extras_require={
         "dev": [
             "pylint==2.16.2",
         ],
     },
     package_dir={'': 'src'},
     python_requires='>=3.8',
-    package_data={"ding_api_client": ["py.typed"]},
+    package_data={'ding_api_client': ['py.typed']},
 )
```

### Comparing `ding_api_client-3.4.0/src/ding/_hooks/sdkhooks.py` & `ding_api_client-3.4.1/src/ding/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/_hooks/types.py` & `ding_api_client-3.4.1/src/ding/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/lookup.py` & `ding_api_client-3.4.1/src/ding/lookup.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/__init__.py` & `ding_api_client-3.4.1/src/ding/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/createauthenticationrequest.py` & `ding_api_client-3.4.1/src/ding/models/components/createauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/createauthenticationresponse.py` & `ding_api_client-3.4.1/src/ding/models/components/createauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/createcheckrequest.py` & `ding_api_client-3.4.1/src/ding/models/components/createcheckrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/createcheckresponse.py` & `ding_api_client-3.4.1/src/ding/models/components/createcheckresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/feedbackrequest.py` & `ding_api_client-3.4.1/src/ding/models/components/feedbackrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/feedbackresponse.py` & `ding_api_client-3.4.1/src/ding/models/components/feedbackresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/lookupresponse.py` & `ding_api_client-3.4.1/src/ding/models/components/lookupresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/retryauthenticationrequest.py` & `ding_api_client-3.4.1/src/ding/models/components/retryauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/components/retryauthenticationresponse.py` & `ding_api_client-3.4.1/src/ding/models/components/retryauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/errors/errorresponse.py` & `ding_api_client-3.4.1/src/ding/models/errors/errorresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/errors/sdkerror.py` & `ding_api_client-3.4.1/src/ding/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/operations/check.py` & `ding_api_client-3.4.1/src/ding/models/operations/check.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/operations/create_authentication.py` & `ding_api_client-3.4.1/src/ding/models/operations/create_authentication.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/operations/feedback.py` & `ding_api_client-3.4.1/src/ding/models/operations/feedback.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/operations/lookup.py` & `ding_api_client-3.4.1/src/ding/models/operations/lookup.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/models/operations/retry.py` & `ding_api_client-3.4.1/src/ding/models/operations/retry.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/otp.py` & `ding_api_client-3.4.1/src/ding/otp.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/sdk.py` & `ding_api_client-3.4.1/src/ding/sdk.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/sdkconfiguration.py` & `ding_api_client-3.4.1/src/ding/sdkconfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '3.4.0'
-    gen_version: str = '2.298.0'
-    user_agent: str = 'speakeasy-sdk/python 3.4.0 2.298.0 1.0.0 ding_api_client'
+    sdk_version: str = '3.4.1'
+    gen_version: str = '2.298.2'
+    user_agent: str = 'speakeasy-sdk/python 3.4.1 2.298.2 1.0.0 ding_api_client'
     retry_config: Optional[RetryConfig] = None
     _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
```

### Comparing `ding_api_client-3.4.0/src/ding/utils/retries.py` & `ding_api_client-3.4.1/src/ding/utils/retries.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding/utils/utils.py` & `ding_api_client-3.4.1/src/ding/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.0/src/ding_api_client.egg-info/PKG-INFO` & `ding_api_client-3.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ding-api-client
-Version: 3.4.0
+Name: ding_api_client
+Version: 3.4.1
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
@@ -101,24 +101,24 @@
         
         ```
         <!-- End SDK Example Usage [usage] -->
         
         <!-- Start Available Resources and Operations [operations] -->
         ## Available Resources and Operations
         
-        ### [otp](docs/sdks/otp/README.md)
+        ### [otp](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md)
         
-        * [create_authentication](docs/sdks/otp/README.md#create_authentication) - Send a code
-        * [check](docs/sdks/otp/README.md#check) - Check a code
-        * [feedback](docs/sdks/otp/README.md#feedback) - Send feedback
-        * [retry](docs/sdks/otp/README.md#retry) - Perform a retry
+        * [create_authentication](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md#create_authentication) - Send a code
+        * [check](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md#check) - Check a code
+        * [feedback](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md#feedback) - Send feedback
+        * [retry](https://github.com/ding-live/ding-python/blob/master/docs/sdks/otp/README.md#retry) - Perform a retry
         
-        ### [lookup](docs/sdks/lookup/README.md)
+        ### [lookup](https://github.com/ding-live/ding-python/blob/master/docs/sdks/lookup/README.md)
         
-        * [lookup](docs/sdks/lookup/README.md#lookup) - Perform a phone number lookup
+        * [lookup](https://github.com/ding-live/ding-python/blob/master/docs/sdks/lookup/README.md#lookup) - Perform a phone number lookup
         <!-- End Available Resources and Operations [operations] -->
         
         <!-- Start Error Handling [errors] -->
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
```

### Comparing `ding_api_client-3.4.0/src/ding_api_client.egg-info/SOURCES.txt` & `ding_api_client-3.4.1/src/ding_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

