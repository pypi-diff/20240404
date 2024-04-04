# Comparing `tmp/ju-0.1.8.tar.gz` & `tmp/ju-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ju-0.1.8.tar", last modified: Fri Mar 22 13:46:04 2024, max compression
+gzip compressed data, was "ju-0.1.9.tar", last modified: Fri Mar 22 14:17:33 2024, max compression
```

## Comparing `ju-0.1.8.tar` & `ju-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:46:04.666086 ju-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 13:45:36.000000 ju-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-22 13:46:04.670086 ju-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-03-22 13:45:36.000000 ju-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:46:04.666086 ju-0.1.8/ju/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-22 13:45:41.000000 ju-0.1.8/ju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-03-22 13:45:41.000000 ju-0.1.8/ju/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-03-22 13:45:41.000000 ju-0.1.8/ju/oas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-03-22 13:45:41.000000 ju-0.1.8/ju/rjsf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:46:04.666086 ju-0.1.8/ju/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 13:45:36.000000 ju-0.1.8/ju/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-03-22 13:45:36.000000 ju-0.1.8/ju/tests/oas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-22 13:45:36.000000 ju-0.1.8/ju/tests/rjsf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-03-22 13:45:41.000000 ju-0.1.8/ju/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:46:04.666086 ju-0.1.8/ju.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-22 13:46:04.000000 ju-0.1.8/ju.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-22 13:46:04.000000 ju-0.1.8/ju.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 13:46:04.000000 ju-0.1.8/ju.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 13:46:04.000000 ju-0.1.8/ju.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 13:46:04.000000 ju-0.1.8/ju.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-22 13:46:04.000000 ju-0.1.8/ju.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-22 13:46:04.670086 ju-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 13:45:36.000000 ju-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:17:33.737154 ju-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 14:16:53.000000 ju-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-22 14:17:33.737154 ju-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-03-22 14:16:53.000000 ju-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:17:33.737154 ju-0.1.9/ju/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-22 14:16:58.000000 ju-0.1.9/ju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-03-22 14:16:58.000000 ju-0.1.9/ju/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-03-22 14:16:58.000000 ju-0.1.9/ju/oas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-03-22 14:16:58.000000 ju-0.1.9/ju/rjsf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:17:33.737154 ju-0.1.9/ju/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 14:16:53.000000 ju-0.1.9/ju/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-03-22 14:16:53.000000 ju-0.1.9/ju/tests/oas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-22 14:16:53.000000 ju-0.1.9/ju/tests/rjsf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 2024-03-22 14:16:58.000000 ju-0.1.9/ju/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:17:33.737154 ju-0.1.9/ju.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-03-22 14:17:33.000000 ju-0.1.9/ju.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-22 14:17:33.000000 ju-0.1.9/ju.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:17:33.000000 ju-0.1.9/ju.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:17:33.000000 ju-0.1.9/ju.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 14:17:33.000000 ju-0.1.9/ju.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-22 14:17:33.000000 ju-0.1.9/ju.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-22 14:17:33.737154 ju-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 14:16:53.000000 ju-0.1.9/setup.py
```

### Comparing `ju-0.1.8/LICENSE` & `ju-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ju-0.1.8/PKG-INFO` & `ju-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ju
-Version: 0.1.8
+Version: 0.1.9
 Summary: JSON schema Utils
 Author: OtoSense
 License: apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ju-0.1.8/README.md` & `ju-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ju-0.1.8/ju/json_schema.py` & `ju-0.1.9/ju/json_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,19 @@
         # Add the field to the schema
         schema['properties'][name] = field
 
     return schema
 
 
 def json_schema_to_signature(
-    json_schema: dict, *, type_mapper: Mapper = DFLT_JSON_PY_TYPE_PAIRS
+    json_schema: dict,
+    *,
+    type_mapper: Mapper = DFLT_JSON_PY_TYPE_PAIRS,
+    default_default=Parameter.empty,
+    default_annotation=Parameter.empty,
 ):
     """
     Transforms a JSON schema to a Python function signature.
 
     param schema: The JSON schema to transform
     return: The Python function signature
 
@@ -229,29 +233,29 @@
     >>> sig.name
     'earth'
     >>> sig.docs
     'Earth docs'
 
 
     """
-    type_mapper = ensure_callable_mapper(type_mapper)
+    type_mapper = ensure_callable_mapper(type_mapper, default=default_annotation)
     properties = json_schema['properties']
 
     def _params():
         for name, field in properties.items():
             if (json_type := field.get('type', None)) is not None:
                 if not isinstance(json_type, list):
                     py_type = type_mapper(json_type)
                 else:
                     json_types = map(type_mapper, json_type)
                     # Make a typing.Union of the json_types
                     py_type = Union[tuple(json_types)]
             else:
                 py_type = Parameter.empty
-            default = field.get('default', Parameter.empty)
+            default = field.get('default', default_default)
             yield Parameter(
                 name=name,
                 annotation=py_type,
                 default=default,
                 kind=Parameter.POSITIONAL_OR_KEYWORD,
             )
```

### Comparing `ju-0.1.8/ju/oas.py` & `ju-0.1.9/ju/oas.py`

 * *Files identical despite different names*

### Comparing `ju-0.1.8/ju/rjsf.py` & `ju-0.1.9/ju/rjsf.py`

 * *Files identical despite different names*

### Comparing `ju-0.1.8/ju/tests/oas_test.py` & `ju-0.1.9/ju/tests/oas_test.py`

 * *Files identical despite different names*

### Comparing `ju-0.1.8/ju/tests/rjsf_test.py` & `ju-0.1.9/ju/tests/rjsf_test.py`

 * *Files identical despite different names*

### Comparing `ju-0.1.8/ju/util.py` & `ju-0.1.9/ju/util.py`

 * *Files identical despite different names*

### Comparing `ju-0.1.8/ju.egg-info/PKG-INFO` & `ju-0.1.9/ju.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ju
-Version: 0.1.8
+Version: 0.1.9
 Summary: JSON schema Utils
 Author: OtoSense
 License: apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

