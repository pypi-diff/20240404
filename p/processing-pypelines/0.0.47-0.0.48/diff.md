# Comparing `tmp/processing-pypelines-0.0.47.tar.gz` & `tmp/processing-pypelines-0.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.47.tar", last modified: Thu Apr  4 14:24:16 2024, max compression
+gzip compressed data, was "processing-pypelines-0.0.48.tar", last modified: Thu Apr  4 17:53:19 2024, max compression
```

## Comparing `processing-pypelines-0.0.47.tar` & `processing-pypelines-0.0.48.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:24:16.610083 processing-pypelines-0.0.47/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 14:24:16.610083 processing-pypelines-0.0.47/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 14:24:16.610083 processing-pypelines-0.0.47/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:24:16.606083 processing-pypelines-0.0.47/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:24:16.610083 processing-pypelines-0.0.47/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 14:24:16.000000 processing-pypelines-0.0.47/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 14:24:16.000000 processing-pypelines-0.0.47/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 14:24:16.000000 processing-pypelines-0.0.47/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 14:24:16.000000 processing-pypelines-0.0.47/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 14:24:16.000000 processing-pypelines-0.0.47/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:24:16.610083 processing-pypelines-0.0.47/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    19332 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:24:16.610083 processing-pypelines-0.0.47/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 14:24:06.000000 processing-pypelines-0.0.47/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/requirements-celery.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.950630 processing-pypelines-0.0.48/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/src/pypelines/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    20400 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/celery_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/disk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/loggs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/multisession.py
+-rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/pickle_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/pipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/tests/tests.py
```

### Comparing `processing-pypelines-0.0.47/LICENSE` & `processing-pypelines-0.0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/PKG-INFO` & `processing-pypelines-0.0.48/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.47
+Version: 0.0.48
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.47/pyproject.toml` & `processing-pypelines-0.0.48/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/processing_pypelines.egg-info/PKG-INFO` & `processing-pypelines-0.0.48/src/processing_pypelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.47
+Version: 0.0.48
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.47/src/processing_pypelines.egg-info/SOURCES.txt` & `processing-pypelines-0.0.48/src/processing_pypelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/accessors.py` & `processing-pypelines-0.0.48/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/arguments.py` & `processing-pypelines-0.0.48/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/celery_tasks.py` & `processing-pypelines-0.0.48/src/pypelines/celery_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -332,25 +332,58 @@
 
     def get_signature_as_string(signature):
         params = [
             param_value for param_name, param_value in signature.parameters.items() if param_name not in ["session"]
         ]
         return str(signature.replace(parameters=params))[1:-1].replace(" *,", "")
 
-    def get_signature_as_dict(signature_string):
-        from re import compile as re_compile
-        from ast import literal_eval
-
-        signature_pattern = re_compile(r" *(?P<key> *\w+) *= *(?P<value>.*?) *(?=(?:(?:, *\w+ *=)|(?:$)))")
-        patt = signature_pattern.findall(signature_string)
-        data = {}
-        for key, value in patt:
-            t_val = literal_eval(value)
-            data[key] = t_val
-        return data
+    def get_type_name(annotation):
+        from inspect import Parameter
+        from typing import get_args, get_origin
+        from types import UnionType
+
+        if isinstance(annotation, str):
+            annotation = string_to_typehint(annotation, globals(), locals())
+
+        if isinstance(annotation, UnionType):
+            typ = get_args(annotation)[0]
+        elif hasattr(annotation, "__origin__"):  # For types from 'typing' like List, Dict, etc.
+            typ = get_origin(annotation)
+        else:
+            typ = annotation
+
+        if isinstance(typ, type):
+            if typ is Parameter.empty:
+                return "__unknown__"
+            else:
+                return typ.__name__
+        return "__unknown__"
+
+    def string_to_typehint(string_hint, globalns=None, localns=None):
+        from typing import ForwardRef, _eval_type
+
+        try:
+            return _eval_type(ForwardRef(string_hint), globalns, localns)
+        except NameError:
+            return "__unknown__"
+
+    def get_signature_as_dict(signature):
+        from inspect import Parameter
+
+        parameters = signature.parameters
+        parsed_args = {}
+        for name, param in parameters.items():
+
+            parsed_args[name] = {
+                "typehint": get_type_name(param.annotation),
+                "default_value": param.default if param.default is not Parameter.empty else "__empty__",
+                "kind": param.kind.name,
+            }
+
+        return parsed_args
 
     class Handshake(Task):
         name = f"{app_name}.handshake"
 
         def run(self):
             return f"{node()} is happy to shake your hand and says hello !"
 
@@ -369,15 +402,15 @@
                 return {}
             for pipeline in pipelines.values():
                 pipeline.resolve()
                 for pipe in pipeline.pipes.values():
                     for step in pipe.steps.values():
                         if step.complete_name in app.tasks.keys():
                             str_sig = get_signature_as_string(step.generate.__signature__)
-                            dict_sig = get_signature_as_dict(str_sig)
+                            dict_sig = get_signature_as_dict(step.generate.__signature__)
                             doc = step.generate.__doc__
                             task_data = {
                                 "signature": str_sig,
                                 "signature_dict": dict_sig,
                                 "docstring": doc,
                                 "step_name": step.step_name,
                                 "pipe_name": step.pipe_name,
```

### Comparing `processing-pypelines-0.0.47/src/pypelines/disk.py` & `processing-pypelines-0.0.48/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/examples.py` & `processing-pypelines-0.0.48/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/graphs.py` & `processing-pypelines-0.0.48/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/loggs.py` & `processing-pypelines-0.0.48/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/multisession.py` & `processing-pypelines-0.0.48/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/pickle_backend.py` & `processing-pypelines-0.0.48/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/pipelines.py` & `processing-pypelines-0.0.48/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/pipes.py` & `processing-pypelines-0.0.48/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/sessions.py` & `processing-pypelines-0.0.48/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/steps.py` & `processing-pypelines-0.0.48/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/tasks.py` & `processing-pypelines-0.0.48/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/src/pypelines/versions.py` & `processing-pypelines-0.0.48/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.47/tests/tests.py` & `processing-pypelines-0.0.48/tests/tests.py`

 * *Files identical despite different names*

