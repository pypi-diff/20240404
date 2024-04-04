# Comparing `tmp/atom-tools-0.5.1.tar.gz` & `tmp/atom-tools-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atom-tools-0.5.1.tar", last modified: Thu Apr  4 12:51:10 2024, max compression
+gzip compressed data, was "atom-tools-0.5.2.tar", last modified: Thu Apr  4 14:03:28 2024, max compression
```

## Comparing `atom-tools-0.5.1.tar` & `atom-tools-0.5.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:10.717129 atom-tools-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 12:51:05.000000 atom-tools-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 12:51:05.000000 atom-tools-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-04 12:51:10.717129 atom-tools-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-04 12:51:05.000000 atom-tools-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:10.709129 atom-tools-0.5.1/atom_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:10.713129 atom-tools-0.5.1/atom_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/command_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:10.713129 atom-tools-0.5.1/atom_tools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/commands/query_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/commands/validate_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/cli/logging_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:10.713129 atom-tools-0.5.1/atom_tools/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/lib/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/lib/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/lib/regex_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/lib/slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-04 12:51:05.000000 atom-tools-0.5.1/atom_tools/lib/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:10.717129 atom-tools-0.5.1/atom_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-04 12:51:10.000000 atom-tools-0.5.1/atom_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 12:51:10.000000 atom-tools-0.5.1/atom_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:51:10.000000 atom-tools-0.5.1/atom_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 12:51:10.000000 atom-tools-0.5.1/atom_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 12:51:10.000000 atom-tools-0.5.1/atom_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 12:51:10.000000 atom-tools-0.5.1/atom_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-04 12:51:05.000000 atom-tools-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:51:10.717129 atom-tools-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:51:10.717129 atom-tools-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)   831738 2024-04-04 12:51:05.000000 atom-tools-0.5.1/test/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-04 12:51:05.000000 atom-tools-0.5.1/test/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 12:51:05.000000 atom-tools-0.5.1/test/test_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 12:51:05.000000 atom-tools-0.5.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.398151 atom-tools-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 14:03:19.000000 atom-tools-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 14:03:19.000000 atom-tools-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-04 14:03:28.398151 atom-tools-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-04-04 14:03:19.000000 atom-tools-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.394151 atom-tools-0.5.2/atom_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.394151 atom-tools-0.5.2/atom_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4429 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/command_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.394151 atom-tools-0.5.2/atom_tools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/query_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/commands/validate_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/cli/logging_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.398151 atom-tools-0.5.2/atom_tools/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28204 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/regex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-04 14:03:19.000000 atom-tools-0.5.2/atom_tools/lib/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.398151 atom-tools-0.5.2/atom_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 14:03:28.000000 atom-tools-0.5.2/atom_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-04 14:03:19.000000 atom-tools-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:03:28.398151 atom-tools-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:03:28.398151 atom-tools-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)   831738 2024-04-04 14:03:19.000000 atom-tools-0.5.2/test/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-04 14:03:19.000000 atom-tools-0.5.2/test/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-04 14:03:19.000000 atom-tools-0.5.2/test/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6034 2024-04-04 14:03:19.000000 atom-tools-0.5.2/test/test_utils.py
```

### Comparing `atom-tools-0.5.1/LICENSE` & `atom-tools-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/PKG-INFO` & `atom-tools-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atom-tools
-Version: 0.5.1
+Version: 0.5.2
 Summary: Collection of tools for use with AppThreat/atom.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/atom-tools
 Project-URL: Bug Tracker, https://github.com/appthreat/atom-tools/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `atom-tools-0.5.1/README.md` & `atom-tools-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/cli/application.py` & `atom-tools-0.5.2/atom_tools/cli/application.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/cli/command_loader.py` & `atom-tools-0.5.2/atom_tools/cli/command_loader.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/cli/commands/convert.py` & `atom-tools-0.5.2/atom_tools/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/cli/commands/filter.py` & `atom-tools-0.5.2/atom_tools/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/cli/commands/query_endpoints.py` & `atom-tools-0.5.2/atom_tools/cli/commands/query_endpoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,8 +73,9 @@
             self.option('input-slice'),
         )
         if not (result := converter.endpoints_to_openapi('')):
             logging.warning('No results produced!')
         line_filter = ()
         if self.option('filter-lines'):
             line_filter = get_ln_range(self.option('filter-lines'))
-        output_endpoints(result, self.option('sparse'), line_filter)
+        output = output_endpoints(result, self.option('sparse'), line_filter)
+        print(output)
```

### Comparing `atom-tools-0.5.1/atom_tools/cli/commands/validate_lines.py` & `atom-tools-0.5.2/atom_tools/cli/commands/validate_lines.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/cli/logging_config.py` & `atom-tools-0.5.2/atom_tools/cli/logging_config.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/lib/converter.py` & `atom-tools-0.5.2/atom_tools/lib/converter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/lib/filtering.py` & `atom-tools-0.5.2/atom_tools/lib/filtering.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/lib/regex_utils.py` & `atom-tools-0.5.2/atom_tools/lib/regex_utils.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/lib/slices.py` & `atom-tools-0.5.2/atom_tools/lib/slices.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools/lib/utils.py` & `atom-tools-0.5.2/atom_tools/lib/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,30 +31,36 @@
 
 def export_json(data: Dict, outfile: str, indent: int | None = None) -> None:
     """Exports data to json"""
     with open(outfile, 'w', encoding='utf-8') as f:
         json.dump(data, f, indent=indent, sort_keys=True)
 
 
-def output_endpoints(data: Dict, names_only: bool, line_range: Tuple[int, int] | Tuple) -> None:
+def output_endpoints(data: Dict, sparse: bool, line_range: Tuple[int, int] | Tuple) -> str:
     """Outputs endpoints"""
     to_print = ''
     for endpoint, values in data.get('paths', {}).items():
-        to_print += f'{endpoint}'
-        usages = values.get("x-atom-usages", {}).get('call', {})
-        if names_only:
-            to_print += '\n'
-            continue
-        for k, v in usages.items():
-            for i in v:
-                if not line_range or line_range[0] <= i <= line_range[1]:
-                    to_print += f':{k}:{i}'
-                    break
-            to_print += '\n'
-    print(to_print)
+        if result := filter_endpoint_ln(endpoint, values, sparse, line_range):
+            to_print += f'{result}\n'
+    return to_print
+
+
+def filter_endpoint_ln(ep: str, values: Dict, sparse: bool, ln_range: Tuple[int, int]) -> str:
+    """Filters endpoint line numbers"""
+    to_print = ''
+    usages = values.get("x-atom-usages", {}).get('call', {})
+    for k, v in usages.items():
+        for i in v:
+            if not ln_range or ln_range[0] <= i <= ln_range[1]:
+                if sparse:
+                    return f'{ep}'
+                to_print += f':{k}:{i}'
+    if to_print:
+        to_print = f'{ep}{to_print}'
+    return to_print
 
 
 def remove_duplicates_list(obj: List[Dict]) -> List[Dict]:
     """Removes duplicates from a list of dictionaries."""
     if not obj:
         return obj
     unique_objs = []
```

### Comparing `atom-tools-0.5.1/atom_tools/lib/validator.py` & `atom-tools-0.5.2/atom_tools/lib/validator.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/atom_tools.egg-info/PKG-INFO` & `atom-tools-0.5.2/atom_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atom-tools
-Version: 0.5.1
+Version: 0.5.2
 Summary: Collection of tools for use with AppThreat/atom.
 Author-email: Caroline Russell <caroline@appthreat.dev>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/appthreat/atom-tools
 Project-URL: Bug Tracker, https://github.com/appthreat/atom-tools/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `atom-tools-0.5.1/atom_tools.egg-info/SOURCES.txt` & `atom-tools-0.5.2/atom_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/pyproject.toml` & `atom-tools-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atom-tools"
-version = "0.5.1"
+version = "0.5.2"
 description = "Collection of tools for use with AppThreat/atom."
 authors = [
   { name = "Caroline Russell", email = "caroline@appthreat.dev" },
 ]
 dependencies = ["cleo>=1.0.0", "jmespath>=1.0.0", "thefuzz>=0.22.1", "json-flatten>=0.3"]
 license = { text = "Apache-2.0" }
 readme = "README.md"
```

### Comparing `atom-tools-0.5.1/test/test_converter.py` & `atom-tools-0.5.2/test/test_converter.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/test/test_filtering.py` & `atom-tools-0.5.2/test/test_filtering.py`

 * *Files identical despite different names*

### Comparing `atom-tools-0.5.1/test/test_slices.py` & `atom-tools-0.5.2/test/test_slices.py`

 * *Files identical despite different names*

