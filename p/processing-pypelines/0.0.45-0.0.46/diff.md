# Comparing `tmp/processing-pypelines-0.0.45.tar.gz` & `tmp/processing-pypelines-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.45.tar", last modified: Thu Apr  4 13:41:53 2024, max compression
+gzip compressed data, was "processing-pypelines-0.0.46.tar", last modified: Thu Apr  4 14:09:23 2024, max compression
```

## Comparing `processing-pypelines-0.0.45.tar` & `processing-pypelines-0.0.46.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.947867 processing-pypelines-0.0.45/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 13:41:53.947867 processing-pypelines-0.0.45/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 13:41:53.947867 processing-pypelines-0.0.45/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.939867 processing-pypelines-0.0.45/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.943867 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.943867 processing-pypelines-0.0.45/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    17819 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.943867 processing-pypelines-0.0.45/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:09:23.251001 processing-pypelines-0.0.46/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 14:09:23.251001 processing-pypelines-0.0.46/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/requirements-celery.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 14:09:23.251001 processing-pypelines-0.0.46/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:09:23.243001 processing-pypelines-0.0.46/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:09:23.247001 processing-pypelines-0.0.46/src/processing_pypelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 14:09:23.000000 processing-pypelines-0.0.46/src/processing_pypelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 14:09:23.000000 processing-pypelines-0.0.46/src/processing_pypelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 14:09:23.000000 processing-pypelines-0.0.46/src/processing_pypelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 14:09:23.000000 processing-pypelines-0.0.46/src/processing_pypelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 14:09:23.000000 processing-pypelines-0.0.46/src/processing_pypelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:09:23.247001 processing-pypelines-0.0.46/src/pypelines/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    19023 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/celery_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/disk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/loggs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/multisession.py
+-rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/pickle_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/pipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/src/pypelines/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 14:09:23.247001 processing-pypelines-0.0.46/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 14:09:13.000000 processing-pypelines-0.0.46/tests/tests.py
```

### Comparing `processing-pypelines-0.0.45/LICENSE` & `processing-pypelines-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/PKG-INFO` & `processing-pypelines-0.0.46/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.45
+Version: 0.0.46
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.45/pyproject.toml` & `processing-pypelines-0.0.46/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/processing_pypelines.egg-info/PKG-INFO` & `processing-pypelines-0.0.46/src/processing_pypelines.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.45
+Version: 0.0.46
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.45/src/processing_pypelines.egg-info/SOURCES.txt` & `processing-pypelines-0.0.46/src/processing_pypelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/accessors.py` & `processing-pypelines-0.0.46/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/arguments.py` & `processing-pypelines-0.0.46/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/celery_tasks.py` & `processing-pypelines-0.0.46/src/pypelines/celery_tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,33 +47,27 @@
             def run(self, task_id, extra=None):
 
                 task = CeleryTaskRecord(task_id)
 
                 try:
                     session = task.get_session()
                     application = task.get_application()
-                    arguments = task.arguments
 
                     with LogTask(task) as log_object:
                         logger = log_object.logger
                         task["log"] = log_object.filename
                         task["status"] = "Started"
                         task.partial_update()
 
                         try:
                             step: "BaseStep" = (
                                 application.pipelines[task.pipeline_name].pipes[task.pipe_name].steps[task.step_name]
                             )
-                            if arguments.get("refresh", False) or arguments.get("refresh_requirements", []):
-                                skip = False
-                            else:
-                                skip = True
-                            arguments.pop(skip)
 
-                            step.generate(session, extra=extra, skip=skip, check_requirements=True, **task.arguments)
+                            step.generate(session, extra=extra, **task.arguments, **task.management_arguments)
                             task.status_from_logs(log_object)
                         except Exception as e:
                             traceback_msg = format_traceback_exc()
                             logger.critical(f"Fatal Error : {e}")
                             logger.critical("Traceback :\n" + traceback_msg)
                             task["status"] = "Failed"
 
@@ -153,16 +147,42 @@
 
     @property
     def step_name(self):
         return self["name"].split(".")[2]
 
     @property
     def arguments(self):
+        # once step arguments control will be done via file, these should take prio over the main step ran's file args
         args = self.get("arguments", {})
-        return args if args else {}
+        args = args if args else {}
+        management_args = self.management_arguments
+        filtered_args = {}
+        for key, value in args.items():
+            if key not in management_args.keys():
+                filtered_args[key] = value
+        return filtered_args
+
+    @property
+    def management_arguments(self):
+        default_management_args = {
+            "skip": True,
+            "refresh": False,
+            "refresh_requirements": False,
+            "check_requirements": True,
+            "save_output": True,
+        }
+        args = self.get("arguments", {})
+        management_args = {}
+        for key, default_value in default_management_args.items():
+            management_args[key] = args.get(key, default_value)
+
+        if management_args["refresh"] == True:
+            management_args["skip"] = False
+
+        return management_args
 
     @property
     def session_path(self) -> str:
         return self.session["path"]
 
     @property
     def task_id(self):
@@ -306,20 +326,32 @@
         files = []
         for prefix, suffix in zip(["", "."], ["", "_secrets"]):
             file_loc = conf_path / f"{prefix}celery_{app_name}{suffix}.toml"
             if file_loc.is_file():
                 files.append(file_loc)
         return files
 
-    def get_signature_string(signature):
+    def get_signature_as_string(signature):
         params = [
             param_value for param_name, param_value in signature.parameters.items() if param_name not in ["session"]
         ]
         return str(signature.replace(parameters=params))[1:-1].replace(" *,", "")
 
+    def get_signature_as_dict(signature_string):
+        from re import compile as re_compile
+        from ast import literal_eval
+
+        signature_pattern = re_compile(r" *(?P<key> *\w+) *= *(?P<value>.*?) *(?=(?:(?:, *\w+ *=)|(?:$)))")
+        patt = signature_pattern.findall(signature_string)
+        data = {}
+        for key, value in patt:
+            t_val = literal_eval(value)
+            data[key] = t_val
+        return data
+
     class Handshake(Task):
         name = f"{app_name}.handshake"
 
         def run(self):
             return f"{node()} is happy to shake your hand and says hello !"
 
     class TasksInfos(Task):
@@ -336,18 +368,20 @@
                 )
                 return {}
             for pipeline in pipelines.values():
                 pipeline.resolve()
                 for pipe in pipeline.pipes.values():
                     for step in pipe.steps.values():
                         if step.complete_name in app.tasks.keys():
-                            sig = get_signature_string(step.generate.__signature__)
+                            str_sig = get_signature_as_string(step.generate.__signature__)
+                            dict_sig = get_signature_as_dict(str_sig)
                             doc = step.generate.__doc__
                             task_data = {
-                                "signature": sig,
+                                "signature": str_sig,
+                                "signature_dict": dict_sig,
                                 "docstring": doc,
                                 "step_name": step.step_name,
                                 "pipe_name": step.pipe_name,
                                 "pipeline_name": step.pipeline_name,
                                 "requires": [item.complete_name for item in step.requires],
                                 "step_level_in_pipe": step.get_level(selfish=selfish),
                             }
```

### Comparing `processing-pypelines-0.0.45/src/pypelines/disk.py` & `processing-pypelines-0.0.46/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/examples.py` & `processing-pypelines-0.0.46/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/graphs.py` & `processing-pypelines-0.0.46/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/loggs.py` & `processing-pypelines-0.0.46/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/multisession.py` & `processing-pypelines-0.0.46/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/pickle_backend.py` & `processing-pypelines-0.0.46/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/pipelines.py` & `processing-pypelines-0.0.46/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/pipes.py` & `processing-pypelines-0.0.46/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/sessions.py` & `processing-pypelines-0.0.46/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/steps.py` & `processing-pypelines-0.0.46/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/tasks.py` & `processing-pypelines-0.0.46/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/src/pypelines/versions.py` & `processing-pypelines-0.0.46/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.45/tests/tests.py` & `processing-pypelines-0.0.46/tests/tests.py`

 * *Files identical despite different names*

