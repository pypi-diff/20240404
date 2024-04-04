# Comparing `tmp/dagster-openai-0.22.9.tar.gz` & `tmp/dagster-openai-0.23.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-openai-0.22.9.tar", last modified: Fri Mar  8 00:31:30 2024, max compression
+gzip compressed data, was "dagster-openai-0.23.0.tar", last modified: Thu Apr  4 19:50:20 2024, max compression
```

## Comparing `dagster-openai-0.22.9.tar` & `dagster-openai-0.23.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:30.838586 dagster-openai-0.22.9/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-03-08 00:17:46.000000 dagster-openai-0.22.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-08 00:17:46.000000 dagster-openai-0.22.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      640 2024-03-08 00:31:30.838586 dagster-openai-0.22.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2024-03-08 00:17:46.000000 dagster-openai-0.22.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:30.838586 dagster-openai-0.22.9/dagster_openai/
--rw-r--r--   0 root         (0) root         (0)      270 2024-03-08 00:17:46.000000 dagster-openai-0.22.9/dagster_openai/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-08 00:17:46.000000 dagster-openai-0.22.9/dagster_openai/py.typed
--rw-r--r--   0 root         (0) root         (0)    14982 2024-03-08 00:17:46.000000 dagster-openai-0.22.9/dagster_openai/resources.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-08 00:17:46.000000 dagster-openai-0.22.9/dagster_openai/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 00:31:30.838586 dagster-openai-0.22.9/dagster_openai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      640 2024-03-08 00:31:30.000000 dagster-openai-0.22.9/dagster_openai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2024-03-08 00:31:30.000000 dagster-openai-0.22.9/dagster_openai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:31:30.000000 dagster-openai-0.22.9/dagster_openai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 00:31:30.000000 dagster-openai-0.22.9/dagster_openai.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-08 00:31:30.000000 dagster-openai-0.22.9/dagster_openai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-08 00:31:30.000000 dagster-openai-0.22.9/dagster_openai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      161 2024-03-08 00:31:30.842586 dagster-openai-0.22.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1207 2024-03-08 00:17:46.000000 dagster-openai-0.22.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:50:20.230005 dagster-openai-0.23.0/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-04 19:44:08.000000 dagster-openai-0.23.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-04 19:44:08.000000 dagster-openai-0.23.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      640 2024-04-04 19:50:20.230005 dagster-openai-0.23.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2024-04-04 19:44:08.000000 dagster-openai-0.23.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:50:20.230005 dagster-openai-0.23.0/dagster_openai/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-04 19:44:08.000000 dagster-openai-0.23.0/dagster_openai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-04 19:44:08.000000 dagster-openai-0.23.0/dagster_openai/py.typed
+-rw-r--r--   0 root         (0) root         (0)    15015 2024-04-04 19:44:08.000000 dagster-openai-0.23.0/dagster_openai/resources.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-04 19:44:08.000000 dagster-openai-0.23.0/dagster_openai/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:50:20.230005 dagster-openai-0.23.0/dagster_openai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      640 2024-04-04 19:50:20.000000 dagster-openai-0.23.0/dagster_openai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-04-04 19:50:20.000000 dagster-openai-0.23.0/dagster_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:50:20.000000 dagster-openai-0.23.0/dagster_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:50:20.000000 dagster-openai-0.23.0/dagster_openai.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-04 19:50:20.000000 dagster-openai-0.23.0/dagster_openai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-04 19:50:20.000000 dagster-openai-0.23.0/dagster_openai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-04 19:50:20.230005 dagster-openai-0.23.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1207 2024-04-04 19:44:08.000000 dagster-openai-0.23.0/setup.py
```

### Comparing `dagster-openai-0.22.9/LICENSE` & `dagster-openai-0.23.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-openai-0.22.9/PKG-INFO` & `dagster-openai-0.23.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-openai
-Version: 0.22.9
+Version: 0.23.0
 Summary: A Open AI client resource for interacting with Open AI API.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-openai
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-openai-0.22.9/dagster_openai/resources.py` & `dagster-openai-0.23.0/dagster_openai/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,17 @@
     for metadata_key, delta in usage_metadata.items():
         counters[metadata_key] += delta
     context.add_output_metadata(dict(counters), output_name)
 
 
 @public
 @experimental
-def with_usage_metadata(context: AssetExecutionContext, output_name: Optional[str], func):
+def with_usage_metadata(
+    context: Union[AssetExecutionContext, OpExecutionContext], output_name: Optional[str], func
+):
     """This wrapper can be used on any endpoint of the
     `openai library <https://github.com/openai/openai-python>`
     to log the OpenAI API usage metadata in the asset metadata.
 
     Examples:
         .. code-block:: python
```

### Comparing `dagster-openai-0.22.9/dagster_openai.egg-info/PKG-INFO` & `dagster-openai-0.23.0/dagster_openai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-openai
-Version: 0.22.9
+Version: 0.23.0
 Summary: A Open AI client resource for interacting with Open AI API.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-openai
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-openai-0.22.9/setup.py` & `dagster-openai-0.23.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,12 +28,12 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_openai_tests*"]),
     install_requires=[
-        "dagster==1.6.9",
+        "dagster==1.7.0",
         "openai",
     ],
     zip_safe=False,
 )
```

