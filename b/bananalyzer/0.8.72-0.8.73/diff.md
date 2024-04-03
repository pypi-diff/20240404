# Comparing `tmp/bananalyzer-0.8.72.tar.gz` & `tmp/bananalyzer-0.8.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bananalyzer-0.8.72.tar", max compression
+gzip compressed data, was "bananalyzer-0.8.73.tar", max compression
```

## Comparing `bananalyzer-0.8.72.tar` & `bananalyzer-0.8.73.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2023-11-23 23:05:17.895386 bananalyzer-0.8.72/LICENSE
--rw-r--r--   0        0        0     7149 2024-01-29 23:48:01.270146 bananalyzer-0.8.72/README.md
--rw-r--r--   0        0        0      380 2024-01-29 23:31:29.206701 bananalyzer-0.8.72/bananalyzer/__init__.py
--rw-r--r--   0        0        0    10925 2024-02-20 00:23:21.187131 bananalyzer-0.8.72/bananalyzer/__main__.py
--rw-r--r--   0        0        0       79 2024-01-18 00:36:02.748184 bananalyzer-0.8.72/bananalyzer/__version.py
--rw-r--r--   0        0        0        0 2023-11-23 23:05:17.898081 bananalyzer-0.8.72/bananalyzer/data/__init__.py
--rw-r--r--   0        0        0     1416 2024-02-14 05:15:51.767051 bananalyzer-0.8.72/bananalyzer/data/banana_seeds.py
--rw-r--r--   0        0        0     4583 2024-01-29 23:31:29.208551 bananalyzer-0.8.72/bananalyzer/data/examples.py
--rw-r--r--   0        0        0    13341 2024-03-19 05:36:25.357129 bananalyzer-0.8.72/bananalyzer/data/fetch_schemas.py
--rw-r--r--   0        0        0     5356 2024-02-15 22:53:28.228334 bananalyzer-0.8.72/bananalyzer/data/generate_examples.py
--rw-r--r--   0        0        0     6273 2024-03-19 05:36:25.358014 bananalyzer-0.8.72/bananalyzer/data/schemas.py
--rw-r--r--   0        0        0     6703 2024-01-29 23:31:29.209682 bananalyzer-0.8.72/bananalyzer/hooks.py
--rw-r--r--   0        0        0     1249 2024-01-29 23:31:29.209995 bananalyzer-0.8.72/bananalyzer/junit.py
--rw-r--r--   0        0        0        0 2023-11-23 23:05:17.900777 bananalyzer-0.8.72/bananalyzer/runner/__init__.py
--rw-r--r--   0        0        0      501 2023-11-28 00:11:43.853844 bananalyzer-0.8.72/bananalyzer/runner/agent_runner.py
--rw-r--r--   0        0        0     4404 2024-02-16 01:47:21.342805 bananalyzer-0.8.72/bananalyzer/runner/evals.py
--rw-r--r--   0        0        0     2402 2024-03-19 05:36:28.376065 bananalyzer-0.8.72/bananalyzer/runner/generator.py
--rw-r--r--   0        0        0     1306 2024-02-16 05:41:25.422171 bananalyzer-0.8.72/bananalyzer/runner/null_agent_wrapper.py
--rw-r--r--   0        0        0     4392 2024-03-19 05:36:28.376276 bananalyzer-0.8.72/bananalyzer/runner/runner.py
--rw-r--r--   0        0        0     1566 2023-11-23 23:05:17.903092 bananalyzer-0.8.72/bananalyzer/runner/website_responder.py
--rw-r--r--   0        0        0     1366 2024-02-19 05:54:13.593386 bananalyzer-0.8.72/bananalyzer/schema.py
--rw-r--r--   0        0        0     1320 2024-03-19 05:37:21.196837 bananalyzer-0.8.72/pyproject.toml
--rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 bananalyzer-0.8.72/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-23 23:05:17.895386 bananalyzer-0.8.73/LICENSE
+-rw-r--r--   0        0        0     7149 2024-01-29 23:48:01.270146 bananalyzer-0.8.73/README.md
+-rw-r--r--   0        0        0      380 2024-01-29 23:31:29.206701 bananalyzer-0.8.73/bananalyzer/__init__.py
+-rw-r--r--   0        0        0    10925 2024-04-02 18:46:06.321568 bananalyzer-0.8.73/bananalyzer/__main__.py
+-rw-r--r--   0        0        0       79 2024-01-18 00:36:02.748184 bananalyzer-0.8.73/bananalyzer/__version.py
+-rw-r--r--   0        0        0        0 2023-11-23 23:05:17.898081 bananalyzer-0.8.73/bananalyzer/data/__init__.py
+-rw-r--r--   0        0        0     1500 2024-04-02 18:44:14.621000 bananalyzer-0.8.73/bananalyzer/data/banana_seeds.py
+-rw-r--r--   0        0        0     4583 2024-01-29 23:31:29.208551 bananalyzer-0.8.73/bananalyzer/data/examples.py
+-rw-r--r--   0        0        0    13341 2024-03-19 05:36:25.357129 bananalyzer-0.8.73/bananalyzer/data/fetch_schemas.py
+-rw-r--r--   0        0        0     5356 2024-02-15 22:53:28.228334 bananalyzer-0.8.73/bananalyzer/data/generate_examples.py
+-rw-r--r--   0        0        0     6273 2024-03-19 05:36:25.358014 bananalyzer-0.8.73/bananalyzer/data/schemas.py
+-rw-r--r--   0        0        0     6703 2024-01-29 23:31:29.209682 bananalyzer-0.8.73/bananalyzer/hooks.py
+-rw-r--r--   0        0        0     1249 2024-01-29 23:31:29.209995 bananalyzer-0.8.73/bananalyzer/junit.py
+-rw-r--r--   0        0        0        0 2023-11-23 23:05:17.900777 bananalyzer-0.8.73/bananalyzer/runner/__init__.py
+-rw-r--r--   0        0        0      501 2023-11-28 00:11:43.853844 bananalyzer-0.8.73/bananalyzer/runner/agent_runner.py
+-rw-r--r--   0        0        0     5006 2024-04-03 21:50:56.706436 bananalyzer-0.8.73/bananalyzer/runner/evals.py
+-rw-r--r--   0        0        0     2402 2024-03-19 05:36:28.376065 bananalyzer-0.8.73/bananalyzer/runner/generator.py
+-rw-r--r--   0        0        0     1306 2024-02-16 05:41:25.422171 bananalyzer-0.8.73/bananalyzer/runner/null_agent_wrapper.py
+-rw-r--r--   0        0        0     4392 2024-03-19 05:36:28.376276 bananalyzer-0.8.73/bananalyzer/runner/runner.py
+-rw-r--r--   0        0        0     1566 2023-11-23 23:05:17.903092 bananalyzer-0.8.73/bananalyzer/runner/website_responder.py
+-rw-r--r--   0        0        0     1366 2024-02-19 05:54:13.593386 bananalyzer-0.8.73/bananalyzer/schema.py
+-rw-r--r--   0        0        0     1320 2024-04-03 21:55:57.989313 bananalyzer-0.8.73/pyproject.toml
+-rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 bananalyzer-0.8.73/PKG-INFO
```

### Comparing `bananalyzer-0.8.72/LICENSE` & `bananalyzer-0.8.73/LICENSE`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/README.md` & `bananalyzer-0.8.73/README.md`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/__main__.py` & `bananalyzer-0.8.73/bananalyzer/__main__.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/data/banana_seeds.py` & `bananalyzer-0.8.73/bananalyzer/data/banana_seeds.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from typing import Any, Dict, List
 
-import boto3
 
-s3 = boto3.client("s3", region_name="us-east-1")
+def download_examples_from_s3(examples_bucket: str) -> List[Dict[str, Any]]:
+    import boto3
 
+    s3 = boto3.client("s3", region_name="us-east-1")
 
-def download_examples_from_s3(examples_bucket: str) -> List[Dict[str, Any]]:
     examples = []
     response = s3.list_objects(Bucket=examples_bucket)
     for file in response["Contents"]:
         key = file["Key"]
 
         if key.startswith("example-") and key.endswith(".json"):
             response = s3.get_object(Bucket=examples_bucket, Key=key)
@@ -29,14 +29,18 @@
 
             examples.append(example)
 
     return examples
 
 
 def download_mhtml(url: str) -> str:
+    import boto3
+
+    s3 = boto3.client("s3", region_name="us-east-1")
+    
     if url.startswith("s3://"):
         bucket_name = url.split("/")[2]
         key = "/".join(url.split("/")[3:])
 
         response = s3.get_object(Bucket=bucket_name, Key=key)
         mhtml = response["Body"].read().decode("utf-8")
```

### Comparing `bananalyzer-0.8.72/bananalyzer/data/examples.py` & `bananalyzer-0.8.73/bananalyzer/data/examples.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/data/fetch_schemas.py` & `bananalyzer-0.8.73/bananalyzer/data/fetch_schemas.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/data/generate_examples.py` & `bananalyzer-0.8.73/bananalyzer/data/generate_examples.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/data/schemas.py` & `bananalyzer-0.8.73/bananalyzer/data/schemas.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/hooks.py` & `bananalyzer-0.8.73/bananalyzer/hooks.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/junit.py` & `bananalyzer-0.8.73/bananalyzer/junit.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/runner/evals.py` & `bananalyzer-0.8.73/bananalyzer/runner/evals.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,20 +35,34 @@
         return [trim_strings(elem) for elem in value]
     elif isinstance(value, str):
         return value.strip()
     else:
         return value
 
 
+def replace_empty_strings_with_none(value: AllowedJSON) -> AllowedJSON | None:
+    """Recursively replace empty strings with None in the given JSON structure."""
+    if isinstance(value, dict):
+        return {k: replace_empty_strings_with_none(v) for k, v in value.items()}
+    elif isinstance(value, list):
+        return [replace_empty_strings_with_none(elem) for elem in value]
+    elif isinstance(value, str) and value == "":
+        return None
+    else:
+        return value
+
+
 def validate_json_match(expected: AllowedJSON, actual: AllowedJSON) -> None:
     if isinstance(expected, Dict) and isinstance(actual, Dict):
         expected = format_new_lines(expected)
         expected = trim_strings(expected)
+        expected = replace_empty_strings_with_none(expected)
         actual = format_new_lines(actual)
         actual = trim_strings(actual)
+        actual = replace_empty_strings_with_none(actual)
 
         # TODO: Pass in schema in the backend and handle this OUTSIDE of tests
         # Adding missing keys in actual with None if they are expected to be None
         for key, value in expected.items():
             if value is None and key not in actual:
                 actual[key] = None
```

### Comparing `bananalyzer-0.8.72/bananalyzer/runner/generator.py` & `bananalyzer-0.8.73/bananalyzer/runner/generator.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/runner/null_agent_wrapper.py` & `bananalyzer-0.8.73/bananalyzer/runner/null_agent_wrapper.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/runner/runner.py` & `bananalyzer-0.8.73/bananalyzer/runner/runner.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/runner/website_responder.py` & `bananalyzer-0.8.73/bananalyzer/runner/website_responder.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/bananalyzer/schema.py` & `bananalyzer-0.8.73/bananalyzer/schema.py`

 * *Files identical despite different names*

### Comparing `bananalyzer-0.8.72/pyproject.toml` & `bananalyzer-0.8.73/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bananalyzer"
-version = "0.8.72"
+version = "0.8.73"
 
 description = "Open source AI Agent evaluation framework for web tasks 🐒🍌"
 authors = ["asim-shrestha <asim.shrestha@hotmail.com>", "awtkns <hello@awtkns.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 bananalyze = "bananalyzer.__main__:main"
```

### Comparing `bananalyzer-0.8.72/PKG-INFO` & `bananalyzer-0.8.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bananalyzer
-Version: 0.8.72
+Version: 0.8.73
 Summary: Open source AI Agent evaluation framework for web tasks 🐒🍌
 Author: asim-shrestha
 Author-email: asim.shrestha@hotmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

