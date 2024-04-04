# Comparing `tmp/processing-pypelines-0.0.50.tar.gz` & `tmp/processing-pypelines-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.50.tar", last modified: Thu Apr  4 20:12:16 2024, max compression
+gzip compressed data, was "processing-pypelines-0.0.51.tar", last modified: Thu Apr  4 21:25:42 2024, max compression
```

## Comparing `processing-pypelines-0.0.50.tar` & `processing-pypelines-0.0.51.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:12:16.232669 processing-pypelines-0.0.50/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 20:12:16.228670 processing-pypelines-0.0.50/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 20:12:16.232669 processing-pypelines-0.0.50/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:12:16.220670 processing-pypelines-0.0.50/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:12:16.228670 processing-pypelines-0.0.50/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 20:12:16.000000 processing-pypelines-0.0.50/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 20:12:16.000000 processing-pypelines-0.0.50/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 20:12:16.000000 processing-pypelines-0.0.50/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 20:12:16.000000 processing-pypelines-0.0.50/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 20:12:16.000000 processing-pypelines-0.0.50/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:12:16.228670 processing-pypelines-0.0.50/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    20738 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:12:16.228670 processing-pypelines-0.0.50/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 20:12:04.000000 processing-pypelines-0.0.50/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.568300 processing-pypelines-0.0.51/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:25:42.568300 processing-pypelines-0.0.51/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/requirements-celery.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:25:42.568300 processing-pypelines-0.0.51/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.560300 processing-pypelines-0.0.51/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.564300 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.564300 processing-pypelines-0.0.51/src/pypelines/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    21258 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/celery_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/disk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/loggs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/multisession.py
+-rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/pickle_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/pipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.564300 processing-pypelines-0.0.51/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/tests/tests.py
```

### Comparing `processing-pypelines-0.0.50/LICENSE` & `processing-pypelines-0.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/PKG-INFO` & `processing-pypelines-0.0.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.50
+Version: 0.0.51
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.50/pyproject.toml` & `processing-pypelines-0.0.51/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/processing_pypelines.egg-info/PKG-INFO` & `processing-pypelines-0.0.51/src/processing_pypelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.50
+Version: 0.0.51
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.50/src/processing_pypelines.egg-info/SOURCES.txt` & `processing-pypelines-0.0.51/src/processing_pypelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/accessors.py` & `processing-pypelines-0.0.51/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/arguments.py` & `processing-pypelines-0.0.51/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/celery_tasks.py` & `processing-pypelines-0.0.51/src/pypelines/celery_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,18 +439,21 @@
                             tasks_dynamic_data[step.complete_name] = task_data
             return tasks_dynamic_data
 
     def get_remote_tasks(self):
         registered_tasks = self.control.inspect().registered_tasks()
         workers = []
         task_names = []
-        for worker, tasks in registered_tasks.items():
-            workers.append(worker)
-            for task in tasks:
-                task_names.append(task)
+        if registered_tasks:
+            for worker, tasks in registered_tasks.items():
+                workers.append(worker)
+                for task in tasks:
+                    task_names.append(task)
+
+        return {"workers": workers, "task_names": task_names}
 
     def get_celery_app_tasks(self, refresh=False):
 
         from datetime import datetime, timedelta
 
         auto_refresh_time = timedelta(0, (3600 * 24))  # a full day (24 hours of 3600 seconds)
         failed_refresh_retry_time = timedelta(0, (60 * 5))  # try to refresh after 5 minutes
@@ -499,14 +502,23 @@
 
     def launch_named_task_remotely(self, session_id, task_name, extra=None, kwargs={}):
         task_record = CeleryTaskRecord.create_from_task_name(
             self, task_name, app_name, session_id, extra=extra, **kwargs
         )
         return task_record
 
+    def is_hand_shaken(self):
+        try:
+            result = self.tasks[f"{app_name}.handshake"].delay(app_name).get(timeout=1)
+            logger.warning(f"Handshake result : {result}")
+            return True
+        except ValueError:
+            logger.error("No handshake result. All workers are busy ?")
+            return False
+
     settings_files = get_setting_files_path(conf_path)
 
     if len(settings_files) == 0:
         logger.warning(f"{failure_message} Could not find celery toml config files.")
         return None
 
     try:
@@ -559,13 +571,14 @@
 
     app.register_task(Handshake)
     app.register_task(TasksInfos)
 
     app.get_remote_tasks = MethodType(get_remote_tasks, app)  # type: ignore
     app.get_celery_app_tasks = MethodType(get_celery_app_tasks, app)  # type: ignore
     app.launch_named_task_remotely = MethodType(launch_named_task_remotely, app)  # type: ignore
+    app.is_hand_shaken = MethodType(is_hand_shaken, app)  # type: ignore
 
     logger.info(f"The celery app {app_name} was created successfully.")
 
     APPLICATIONS_STORE[app_name] = app
 
     return app
```

### Comparing `processing-pypelines-0.0.50/src/pypelines/disk.py` & `processing-pypelines-0.0.51/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/examples.py` & `processing-pypelines-0.0.51/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/graphs.py` & `processing-pypelines-0.0.51/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/loggs.py` & `processing-pypelines-0.0.51/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/multisession.py` & `processing-pypelines-0.0.51/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/pickle_backend.py` & `processing-pypelines-0.0.51/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/pipelines.py` & `processing-pypelines-0.0.51/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/pipes.py` & `processing-pypelines-0.0.51/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/sessions.py` & `processing-pypelines-0.0.51/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/steps.py` & `processing-pypelines-0.0.51/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/tasks.py` & `processing-pypelines-0.0.51/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/src/pypelines/versions.py` & `processing-pypelines-0.0.51/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.50/tests/tests.py` & `processing-pypelines-0.0.51/tests/tests.py`

 * *Files identical despite different names*

