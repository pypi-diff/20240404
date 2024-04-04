# Comparing `tmp/eppo_metrics_sync-0.0.0.tar.gz` & `tmp/eppo_metrics_sync-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eppo_metrics_sync-0.0.0.tar", last modified: Thu Dec 21 19:31:38 2023, max compression
+gzip compressed data, was "eppo_metrics_sync-0.0.1.tar", last modified: Thu Apr  4 05:08:41 2024, max compression
```

## Comparing `eppo_metrics_sync-0.0.0.tar` & `eppo_metrics_sync-0.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-12-21 19:31:38.233033 eppo_metrics_sync-0.0.0/
--rw-r--r--   0 lukas      (501) staff       (20)     1061 2023-12-07 04:26:58.000000 eppo_metrics_sync-0.0.0/LICENSE
--rw-r--r--   0 lukas      (501) staff       (20)       56 2023-11-11 23:16:23.000000 eppo_metrics_sync-0.0.0/MANIFEST.in
--rw-r--r--   0 lukas      (501) staff       (20)      155 2023-12-21 19:31:38.232694 eppo_metrics_sync-0.0.0/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)        0 2023-11-11 00:59:21.000000 eppo_metrics_sync-0.0.0/README.md
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-12-21 19:31:38.227552 eppo_metrics_sync-0.0.0/eppo_metrics_sync/
--rw-r--r--   0 lukas      (501) staff       (20)       46 2023-11-11 19:14:32.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)      673 2023-12-06 16:41:37.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync/__main__.py
--rw-r--r--   0 lukas      (501) staff       (20)     3973 2023-12-07 15:00:45.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync/eppo_metrics_sync.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-12-21 19:31:38.229428 eppo_metrics_sync-0.0.0/eppo_metrics_sync/schema/
--rw-r--r--   0 lukas      (501) staff       (20)    16445 2023-11-29 13:41:09.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync/schema/eppo_metric_schema.json
--rw-r--r--   0 lukas      (501) staff       (20)     5761 2023-11-16 15:36:27.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync/validation.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-12-21 19:31:38.232308 eppo_metrics_sync-0.0.0/eppo_metrics_sync.egg-info/
--rw-r--r--   0 lukas      (501) staff       (20)      155 2023-12-21 19:31:38.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync.egg-info/PKG-INFO
--rw-r--r--   0 lukas      (501) staff       (20)      515 2023-12-21 19:31:38.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync.egg-info/SOURCES.txt
--rw-r--r--   0 lukas      (501) staff       (20)        1 2023-12-21 19:31:38.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync.egg-info/dependency_links.txt
--rw-r--r--   0 lukas      (501) staff       (20)       27 2023-12-21 19:31:38.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync.egg-info/requires.txt
--rw-r--r--   0 lukas      (501) staff       (20)       24 2023-12-21 19:31:38.000000 eppo_metrics_sync-0.0.0/eppo_metrics_sync.egg-info/top_level.txt
--rw-r--r--   0 lukas      (501) staff       (20)       87 2023-12-07 03:11:53.000000 eppo_metrics_sync-0.0.0/pyproject.toml
--rw-r--r--   0 lukas      (501) staff       (20)       38 2023-12-21 19:31:38.233095 eppo_metrics_sync-0.0.0/setup.cfg
--rw-r--r--   0 lukas      (501) staff       (20)      237 2023-12-21 19:29:42.000000 eppo_metrics_sync-0.0.0/setup.py
-drwxr-xr-x   0 lukas      (501) staff       (20)        0 2023-12-21 19:31:38.231648 eppo_metrics_sync-0.0.0/tests/
--rw-r--r--   0 lukas      (501) staff       (20)        0 2023-11-11 01:22:16.000000 eppo_metrics_sync-0.0.0/tests/__init__.py
--rw-r--r--   0 lukas      (501) staff       (20)      306 2023-11-11 01:36:28.000000 eppo_metrics_sync-0.0.0/tests/context.py
--rw-r--r--   0 lukas      (501) staff       (20)      770 2023-12-07 04:04:32.000000 eppo_metrics_sync-0.0.0/tests/test_cli.py
--rw-r--r--   0 lukas      (501) staff       (20)     3752 2023-12-07 04:05:24.000000 eppo_metrics_sync-0.0.0/tests/test_validation.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-04 05:08:41.646856 eppo_metrics_sync-0.0.1/
+-rw-r--r--   0 tyler      (501) staff       (20)     1061 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)       56 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/MANIFEST.in
+-rw-r--r--   0 tyler      (501) staff       (20)      155 2024-04-04 05:08:41.646627 eppo_metrics_sync-0.0.1/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/README.md
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-04 05:08:41.643604 eppo_metrics_sync-0.0.1/eppo_metrics_sync/
+-rw-r--r--   0 tyler      (501) staff       (20)       46 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)      673 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync/__main__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3922 2024-04-03 23:54:28.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync/eppo_metrics_sync.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-04 05:08:41.644768 eppo_metrics_sync-0.0.1/eppo_metrics_sync/schema/
+-rw-r--r--   0 tyler      (501) staff       (20)    16463 2024-04-03 23:54:28.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync/schema/eppo_metric_schema.json
+-rw-r--r--   0 tyler      (501) staff       (20)     5761 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync/validation.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-04 05:08:41.646331 eppo_metrics_sync-0.0.1/eppo_metrics_sync.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)      155 2024-04-04 05:08:41.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      515 2024-04-04 05:08:41.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2024-04-04 05:08:41.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       27 2024-04-04 05:08:41.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       24 2024-04-04 05:08:41.000000 eppo_metrics_sync-0.0.1/eppo_metrics_sync.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       87 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/pyproject.toml
+-rw-r--r--   0 tyler      (501) staff       (20)       38 2024-04-04 05:08:41.646893 eppo_metrics_sync-0.0.1/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)      237 2024-04-04 05:07:06.000000 eppo_metrics_sync-0.0.1/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2024-04-04 05:08:41.646038 eppo_metrics_sync-0.0.1/tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)      306 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/tests/context.py
+-rw-r--r--   0 tyler      (501) staff       (20)      770 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/tests/test_cli.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3752 2024-04-03 00:01:25.000000 eppo_metrics_sync-0.0.1/tests/test_validation.py
```

### Comparing `eppo_metrics_sync-0.0.0/LICENSE` & `eppo_metrics_sync-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eppo_metrics_sync-0.0.0/eppo_metrics_sync/__main__.py` & `eppo_metrics_sync-0.0.1/eppo_metrics_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `eppo_metrics_sync-0.0.0/eppo_metrics_sync/eppo_metrics_sync.py` & `eppo_metrics_sync-0.0.1/eppo_metrics_sync/eppo_metrics_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,112 @@
-import json, yaml, jsonschema, os, logging, requests
+import json
+import jsonschema
+import os
+import requests
+import yaml
 
 from eppo_metrics_sync.validation import (
-    unique_names, 
-    valid_fact_references, 
-    aggregation_is_valid,
+    unique_names,
+    valid_fact_references,
     metric_aggregation_is_valid
 )
 
 API_ENDPOINT = 'https://eppo.cloud/api/v1/metrics/sync'
 
+
 class EppoMetricsSync:
     def __init__(
-        self,
-        directory
+            self,
+            directory
     ):
         self.directory = directory
         self.fact_sources = []
         self.metrics = []
         self.validation_errors = []
 
         # temporary: ideally would pull this from Eppo API
         package_root = os.path.dirname(os.path.abspath(__file__))
         schema_path = os.path.join(package_root, 'schema', 'eppo_metric_schema.json')
         with open(schema_path) as schema_file:
             self.schema = json.load(schema_file)
-    
 
     def load_yaml(self, path):
         with open(path, 'r') as yaml_file:
             yaml_data = yaml.safe_load(yaml_file)
             if 'fact_sources' in yaml_data:
                 self.fact_sources.extend(yaml_data['fact_sources'])
             if 'metrics' in yaml_data:
                 self.metrics.extend(yaml_data['metrics'])
-        
-
-    def read_yaml_files(self):
 
-        # Validate a single YAML file against the schema
-        def yaml_is_valid(yaml_path):
-            with open(yaml_path, 'r') as yaml_file:
-                data = yaml.safe_load(yaml_file)
-                try:
-                    jsonschema.validate(data, self.schema)
-                    return {"passed": True}
-                except jsonschema.exceptions.ValidationError as e:
-                    return {"passed": False, "error_message": e}
+    def yaml_is_valid(self, yaml_path):
+        """
+        Validate a single YAML file against the schema
+
+        """
+        with open(yaml_path, 'r') as yaml_file:
+            data = yaml.safe_load(yaml_file)
+            try:
+                jsonschema.validate(data, self.schema)
+                return {"passed": True}
+            except jsonschema.exceptions.ValidationError as e:
+                return {"passed": False, "error_message": e}
 
+    def read_yaml_files(self):
         # Recursively scan the directory for YAML files and load valid ones
         for root, _, files in os.walk(self.directory):
             for file in files:
                 if file.endswith(".yaml") or file.endswith(".yml"):
                     yaml_path = os.path.join(root, file)
-                    valid = yaml_is_valid(yaml_path)
+                    valid = self.yaml_is_valid(yaml_path)
                     if valid['passed']:
                         self.load_yaml(yaml_path)
                     else:
                         self.validation_errors.append(
-                            f"Schema violation in {yaml_path}: \n{valid.error_message}"
+                            f"Schema violation in {yaml_path}: \n{valid['error_message']}"
                         )
-        
+
         if len(self.fact_sources) == 0 and len(self.metrics) == 0:
             raise ValueError(
                 'No valid yaml files found. ' + ', '.join(self.validation_errors)
             )
 
-
     def validate(self):
 
-        if(len(self.fact_sources) == 0 and len(self.metrics) == 0):
+        if len(self.fact_sources) == 0 and len(self.metrics) == 0:
             raise ValueError('No fact sources or metrics found, did you call eppo_metrics.read_yaml_files()?')
-        
+
         unique_names(self)
         valid_fact_references(self)
         metric_aggregation_is_valid(self)
 
         if self.validation_errors:
             error_count = len(self.validation_errors)
             error_message = f"Validation failed with {error_count} error(s): \n"
             error_message += '\n'.join(self.validation_errors)
             raise ValueError(error_message)
 
         return True
 
-
     def sync(self):
         self.read_yaml_files()
         self.validate()
 
         api_key = os.getenv('EPPO_API_KEY')
         if not api_key:
             raise Exception('EPPO_API_KEY not set in environment variables. Please set and try again')
-        
+
         sync_tag = os.getenv('EPPO_SYNC_TAG')
         if not api_key:
             raise Exception('EPPO_SYNC_TAG not set in environment variables. Please set and try again')
-        
+
         headers = {"X-Eppo-Token": api_key}
         payload = {
             "sync_tag": sync_tag,
-            "fact_sources" : self.fact_sources,
-            "metrics" : self.metrics
+            "fact_sources": self.fact_sources,
+            "metrics": self.metrics
         }
 
         response = requests.post(API_ENDPOINT, json=payload, headers=headers)
 
         if response.status_code < 400:
             print('Metrics synced')
         else:
```

### Comparing `eppo_metrics_sync-0.0.0/eppo_metrics_sync/schema/eppo_metric_schema.json` & `eppo_metrics_sync-0.0.1/eppo_metrics_sync/schema/eppo_metric_schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999904314864%*

 * *Differences: {"'properties'": "{'metrics': {'items': {'properties': {'numerator': {'properties': {'operation': "*

 * *                 "{'enum': {insert: [(6, 'count_distinct')]}}, 'threshold_metric_settings': "*

 * *                 "{'required': {insert: [(0, 'comparison_operator')], delete: [0]}, 'properties': "*

 * *                 "{'comparison_operator': OrderedDict([('description', 'One of gt or gte'), "*

 * *                 "('enum', ['gt', 'gte'])]), delete: ['comparions_operator']}}}}}}}}"}*

```diff
@@ -286,15 +286,16 @@
                                 "description": "Which aggregation to apply to the fact",
                                 "enum": [
                                     "sum",
                                     "count",
                                     "distinct_entity",
                                     "threshold",
                                     "conversion",
-                                    "retention"
+                                    "retention",
+                                    "count_distinct"
                                 ]
                             },
                             "retention_threshold_days": {
                                 "description": "Only used if operation = retention",
                                 "type": "number"
                             },
                             "threshold_metric_settings": {
@@ -308,15 +309,15 @@
                                             "count"
                                         ]
                                     },
                                     "breach_value": {
                                         "description": "At what value is the threshold breached?",
                                         "type": "number"
                                     },
-                                    "comparions_operator": {
+                                    "comparison_operator": {
                                         "description": "One of gt or gte",
                                         "enum": [
                                             "gt",
                                             "gte"
                                         ]
                                     },
                                     "timeframe_unit": {
@@ -330,15 +331,15 @@
                                     },
                                     "timeframe_value": {
                                         "description": "How many timeframe units since assignment to include (optional)",
                                         "value": "number"
                                     }
                                 },
                                 "required": [
-                                    "comparions_operator",
+                                    "comparison_operator",
                                     "aggregation_type",
                                     "breach_value"
                                 ],
                                 "type": "object"
                             },
                             "winsorization_lower_percentile": {
                                 "description": "Percentile at which to clip aggregated metrics (optional)",
```

### Comparing `eppo_metrics_sync-0.0.0/eppo_metrics_sync/validation.py` & `eppo_metrics_sync-0.0.1/eppo_metrics_sync/validation.py`

 * *Files identical despite different names*

### Comparing `eppo_metrics_sync-0.0.0/eppo_metrics_sync.egg-info/SOURCES.txt` & `eppo_metrics_sync-0.0.1/eppo_metrics_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eppo_metrics_sync-0.0.0/tests/test_cli.py` & `eppo_metrics_sync-0.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `eppo_metrics_sync-0.0.0/tests/test_validation.py` & `eppo_metrics_sync-0.0.1/tests/test_validation.py`

 * *Files identical despite different names*

