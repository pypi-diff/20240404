# Comparing `tmp/processing-pypelines-0.0.44.tar.gz` & `tmp/processing-pypelines-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.44.tar", last modified: Thu Mar 28 22:59:28 2024, max compression
+gzip compressed data, was "processing-pypelines-0.0.45.tar", last modified: Thu Apr  4 13:41:53 2024, max compression
```

## Comparing `processing-pypelines-0.0.44.tar` & `processing-pypelines-0.0.45.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 22:59:28.327132 processing-pypelines-0.0.44/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1605 2024-03-28 22:59:28.323132 processing-pypelines-0.0.44/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       36 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 22:59:28.327132 processing-pypelines-0.0.44/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 22:59:28.315132 processing-pypelines-0.0.44/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 22:59:28.323132 processing-pypelines-0.0.44/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1605 2024-03-28 22:59:28.000000 processing-pypelines-0.0.44/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-03-28 22:59:28.000000 processing-pypelines-0.0.44/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 22:59:28.000000 processing-pypelines-0.0.44/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      307 2024-03-28 22:59:28.000000 processing-pypelines-0.0.44/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-28 22:59:28.000000 processing-pypelines-0.0.44/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 22:59:28.323132 processing-pypelines-0.0.44/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    13513 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 22:59:28.323132 processing-pypelines-0.0.44/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-03-28 22:59:17.000000 processing-pypelines-0.0.44/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.947867 processing-pypelines-0.0.45/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 13:41:53.947867 processing-pypelines-0.0.45/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/requirements-celery.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 13:41:53.947867 processing-pypelines-0.0.45/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.939867 processing-pypelines-0.0.45/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.943867 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 13:41:53.000000 processing-pypelines-0.0.45/src/processing_pypelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.943867 processing-pypelines-0.0.45/src/pypelines/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    17819 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/celery_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/disk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/loggs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/multisession.py
+-rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/pickle_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/pipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/src/pypelines/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 13:41:53.943867 processing-pypelines-0.0.45/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 13:41:43.000000 processing-pypelines-0.0.45/tests/tests.py
```

### Comparing `processing-pypelines-0.0.44/LICENSE` & `processing-pypelines-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/PKG-INFO` & `processing-pypelines-0.0.45/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.44
+Version: 0.0.45
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
@@ -25,13 +25,13 @@
 Requires-Dist: matplotlib>=3.8.0; extra == "celery"
 Requires-Dist: natsort>=8.4.0; extra == "celery"
 Requires-Dist: networkx>=3.1; extra == "celery"
 Requires-Dist: numpy>=1.25.2; extra == "celery"
 Requires-Dist: pandas>=2.1.4; extra == "celery"
 Requires-Dist: setuptools>=68.0.0; extra == "celery"
 Requires-Dist: celery>=5.3.5; extra == "celery"
-Requires-Dist: alyx_connector>=0.0.10; extra == "celery"
+Requires-Dist: alyx_connector>=2.1.5; extra == "celery"
 
 # Pypelines
 
 
 ![coverage](https://gitlab.example.com/<namespace>/<project>/badges/<branch>/coverage.svg?job=coverage)
```

### Comparing `processing-pypelines-0.0.44/pyproject.toml` & `processing-pypelines-0.0.45/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/processing_pypelines.egg-info/PKG-INFO` & `processing-pypelines-0.0.45/src/processing_pypelines.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.44
+Version: 0.0.45
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
@@ -25,13 +25,13 @@
 Requires-Dist: matplotlib>=3.8.0; extra == "celery"
 Requires-Dist: natsort>=8.4.0; extra == "celery"
 Requires-Dist: networkx>=3.1; extra == "celery"
 Requires-Dist: numpy>=1.25.2; extra == "celery"
 Requires-Dist: pandas>=2.1.4; extra == "celery"
 Requires-Dist: setuptools>=68.0.0; extra == "celery"
 Requires-Dist: celery>=5.3.5; extra == "celery"
-Requires-Dist: alyx_connector>=0.0.10; extra == "celery"
+Requires-Dist: alyx_connector>=2.1.5; extra == "celery"
 
 # Pypelines
 
 
 ![coverage](https://gitlab.example.com/<namespace>/<project>/badges/<branch>/coverage.svg?job=coverage)
```

### Comparing `processing-pypelines-0.0.44/src/processing_pypelines.egg-info/SOURCES.txt` & `processing-pypelines-0.0.45/src/processing_pypelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/accessors.py` & `processing-pypelines-0.0.45/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/arguments.py` & `processing-pypelines-0.0.45/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/celery_tasks.py` & `processing-pypelines-0.0.45/src/pypelines/celery_tasks.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,97 +2,95 @@
 from .pipelines import Pipeline
 from .loggs import FileFormatter
 from pathlib import Path
 from traceback import format_exc as format_traceback_exc
 import logging
 import coloredlogs
 from logging import getLogger
-from functools import wraps
 from platform import node
 from pandas import Series
 
 from typing import TYPE_CHECKING, List
 
 if TYPE_CHECKING:
     from celery import Celery
     from .steps import BaseStep
 
 
 APPLICATIONS_STORE = {}
 
 
-def get_runner(task_name: str):
-    from celery import Task
-
-    class CeleryRunner(Task):
-        name = task_name
-
-        def run(self, task_id, extra=None):
-
-            task = CeleryTaskRecord(task_id)
-
-            try:
-                session = task.get_session()
-                application = task.get_application()
-                arguments = task.arguments
-
-                with LogTask(task) as log_object:
-                    logger = log_object.logger
-                    task["log"] = log_object.filename
-                    task["status"] = "Started"
-                    task.partial_update()
-
-                    try:
-                        step: "BaseStep" = (
-                            application.pipelines[task.pipeline_name].pipes[task.pipe_name].steps[task.step_name]
-                        )
-                        if arguments.get("refresh", False) or arguments.get("refresh_requirements", []):
-                            skip = False
-                        else:
-                            skip = True
-                        arguments.pop(skip)
-
-                        step.generate(session, extra=extra, skip=skip, check_requirements=True, **task.arguments)
-                        task.status_from_logs(log_object)
-                    except Exception as e:
-                        traceback_msg = format_traceback_exc()
-                        logger.critical(f"Fatal Error : {e}")
-                        logger.critical("Traceback :\n" + traceback_msg)
-                        task["status"] = "Failed"
-
-            except Exception as e:
-                # if it fails outside of the nested try statement, we can't store logs files,
-                # and we mention the failure through alyx directly.
-                task["status"] = "Uncatched_Fail"
-                task["log"] = str(e)
-
-            task.partial_update()
-
-    return CeleryRunner
-
-
 class CeleryAlyxTaskManager(BaseStepTaskManager):
 
     backend: "CeleryTaskBackend"
     step: "BaseStep"
 
     def register_step(self):
         if self.backend:
             # self.backend.app.task(CeleryRunner, name=self.step.complete_name)
-            self.backend.app.register_task(get_runner(self.step.complete_name))
+            self.backend.app.register_task(self.get_runner())
 
     def start(self, session, extra=None, **kwargs):
 
         if not self.backend:
             raise NotImplementedError(
                 "Cannot start a task on a celery cluster as this pipeline " "doesn't have a working celery backend"
             )
 
         return CeleryTaskRecord.create(self, session, extra, **kwargs)
 
+    def get_runner(superself):  # type: ignore
+        from celery import Task
+
+        class CeleryRunner(Task):
+            name = superself.step.complete_name
+
+            def run(self, task_id, extra=None):
+
+                task = CeleryTaskRecord(task_id)
+
+                try:
+                    session = task.get_session()
+                    application = task.get_application()
+                    arguments = task.arguments
+
+                    with LogTask(task) as log_object:
+                        logger = log_object.logger
+                        task["log"] = log_object.filename
+                        task["status"] = "Started"
+                        task.partial_update()
+
+                        try:
+                            step: "BaseStep" = (
+                                application.pipelines[task.pipeline_name].pipes[task.pipe_name].steps[task.step_name]
+                            )
+                            if arguments.get("refresh", False) or arguments.get("refresh_requirements", []):
+                                skip = False
+                            else:
+                                skip = True
+                            arguments.pop(skip)
+
+                            step.generate(session, extra=extra, skip=skip, check_requirements=True, **task.arguments)
+                            task.status_from_logs(log_object)
+                        except Exception as e:
+                            traceback_msg = format_traceback_exc()
+                            logger.critical(f"Fatal Error : {e}")
+                            logger.critical("Traceback :\n" + traceback_msg)
+                            task["status"] = "Failed"
+
+                except Exception as e:
+                    # if it fails outside of the nested try statement, we can't store logs files,
+                    # and we mention the failure through alyx directly.
+                    task["status"] = "Uncatched_Fail"
+                    task["log"] = str(e)
+
+                task.partial_update()
+
+        return CeleryRunner
+
 
 class CeleryTaskRecord(dict):
     session: Series
 
     # a class to make dictionnary keys accessible with attribute syntax
     def __init__(self, task_id, task_infos_dict={}, response_handle=None, session=None):
 
@@ -192,14 +190,36 @@
         worker = task_manager.backend.app.tasks[task_manager.step.complete_name]
         response_handle = worker.delay(task_dict["id"], extra=extra)
 
         return CeleryTaskRecord(
             task_dict["id"], task_infos_dict=task_dict, response_handle=response_handle, session=session
         )
 
+    @staticmethod
+    def create_from_task_name(app: "Celery", task_name: str, pipeline_name: str, session, extra=None, **kwargs):
+        from one import ONE
+
+        connector = ONE(mode="remote", data_access_mode="remote")
+
+        data = {
+            "session": session.name if isinstance(session, Series) else session,
+            "name": task_name,
+            "arguments": kwargs,
+            "status": "Waiting",
+            "executable": pipeline_name,
+        }
+
+        task_dict = connector.alyx.rest("tasks", "create", data=data)
+
+        response_handle = app.send_task(name=task_name, kwargs={"task_id": task_dict["id"], "extra": extra})
+
+        return CeleryTaskRecord(
+            task_dict["id"], task_infos_dict=task_dict, response_handle=response_handle, session=session
+        )
+
 
 class CeleryTaskBackend(BaseTaskBackend):
     app: "Celery"
     task_manager_class = CeleryAlyxTaskManager
 
     def __init__(self, parent: Pipeline, app: "Celery | None" = None):
         super().__init__(parent)
@@ -222,26 +242,14 @@
         return task_manager
 
 
 class CeleryPipeline(Pipeline):
     runner_backend_class = CeleryTaskBackend
 
 
-def get_setting_files_path(conf_path, app_name) -> List[Path]:
-    conf_path = Path(conf_path)
-    if conf_path.is_file():
-        conf_path = conf_path.parent
-    files = []
-    for prefix, suffix in zip(["", "."], ["", "_secrets"]):
-        file_loc = conf_path / f"{prefix}celery_{app_name}{suffix}.toml"
-        if file_loc.is_file():
-            files.append(file_loc)
-    return files
-
-
 class LogTask:
     def __init__(self, task_record: CeleryTaskRecord, username=None, level="LOAD"):
         self.path = Path(task_record.session_path) / "logs"
         self.username = username if username is not None else (node() if node() else "unknown")
         self.worker_pk = task_record.task_id
         self.task_name = task_record["name"]
         self.level = getattr(logging, level.upper())
@@ -284,28 +292,141 @@
         self.logger.addHandler(fh)
 
     def remove_handler(self):
         self.logger.removeHandler(self.logger.handlers[-1])
 
 
 def create_celery_app(conf_path, app_name="pypelines", v_host=None) -> "Celery | None":
+    from types import MethodType
+    from celery import Task
+
+    def get_setting_files_path(conf_path) -> List[Path]:
+        conf_path = Path(conf_path)
+        if conf_path.is_file():
+            conf_path = conf_path.parent
+        files = []
+        for prefix, suffix in zip(["", "."], ["", "_secrets"]):
+            file_loc = conf_path / f"{prefix}celery_{app_name}{suffix}.toml"
+            if file_loc.is_file():
+                files.append(file_loc)
+        return files
+
+    def get_signature_string(signature):
+        params = [
+            param_value for param_name, param_value in signature.parameters.items() if param_name not in ["session"]
+        ]
+        return str(signature.replace(parameters=params))[1:-1].replace(" *,", "")
+
+    class Handshake(Task):
+        name = f"{app_name}.handshake"
+
+        def run(self):
+            return f"{node()} is happy to shake your hand and says hello !"
+
+    class TasksInfos(Task):
+        name = f"{app_name}.tasks_infos"
+
+        def run(self, app_name, selfish=False):
+            app = APPLICATIONS_STORE[app_name]
+            tasks_dynamic_data = {}
+            pipelines = getattr(app, "pipelines", {})
+            if len(pipelines) == 0:
+                logger.warning(
+                    "No pipeline is registered on this app instance. "
+                    "Are you trying to read tasks infos from a non worker app ? (web server side ?)"
+                )
+                return {}
+            for pipeline in pipelines.values():
+                pipeline.resolve()
+                for pipe in pipeline.pipes.values():
+                    for step in pipe.steps.values():
+                        if step.complete_name in app.tasks.keys():
+                            sig = get_signature_string(step.generate.__signature__)
+                            doc = step.generate.__doc__
+                            task_data = {
+                                "signature": sig,
+                                "docstring": doc,
+                                "step_name": step.step_name,
+                                "pipe_name": step.pipe_name,
+                                "pipeline_name": step.pipeline_name,
+                                "requires": [item.complete_name for item in step.requires],
+                                "step_level_in_pipe": step.get_level(selfish=selfish),
+                            }
+                            tasks_dynamic_data[step.complete_name] = task_data
+            return tasks_dynamic_data
+
+    def get_remote_tasks(self):
+        registered_tasks = self.control.inspect().registered_tasks()
+        workers = []
+        task_names = []
+        for worker, tasks in registered_tasks.items():
+            workers.append(worker)
+            for task in tasks:
+                task_names.append(task)
+
+    def get_celery_app_tasks(self, refresh=False):
+
+        from datetime import datetime, timedelta
+
+        auto_refresh_time = timedelta(0, (20 * 1))  # a full day (24 hours of 3600 seconds)
+        failed_refresh_retry_time = timedelta(0, (30 * 1))  # try to refresh after an hour
+
+        app_task_data = getattr(self, "task_data", None)
+
+        if app_task_data is None:
+            try:
+                task_data = self.tasks[f"{app_name}.tasks_infos"].delay(app_name).get(timeout=2)
+                app_task_data = {"task_data": task_data, "refresh_time": datetime.now() + auto_refresh_time}
+                setattr(self, "task_data", app_task_data)
+                logger.warning("Got tasks data for the first time since django server relaunched")
+            except Exception as e:
+                logger.warning(f"Could not get tasks from app. {e}")
+                # logger.warning(f"Remote tasks are : {self.get_remote_tasks()}")
+                # logger.warning(f"Local tasks are : {self.tasks}")
+
+        else:
+            if datetime.now() > app_task_data["refresh_time"]:  # we refresh if refresh time is elapsed
+                refresh = True
+
+            if refresh:
+                try:
+                    task_data = self.tasks[f"{app_name}.tasks_infos"].delay(app_name).get(timeout=2)
+                    app_task_data = {"task_data": task_data, "refresh_time": datetime.now() + auto_refresh_time}
+                    logger.warning("Refreshed celery tasks data sucessfully")
+                except Exception as e:
+                    logger.warning(
+                        "Could not refresh tasks data from remote celery worker. All workers are is probably running. "
+                        f"{e}"
+                    )
+                    app_task_data["refresh_time"] = datetime.now() + failed_refresh_retry_time
+                setattr(self, "task_data", app_task_data)
+            else:
+                delta = (app_task_data["refresh_time"] - datetime.now()).total_seconds()
+                logger.warning(f"Returned cached task_data. Next refresh will happen in at least {delta} seconds")
+        return app_task_data["task_data"] if app_task_data is not None else None
+
+    def launch_named_task_remotely(self, session_id, task_name, extra=None, kwargs={}):
+        task_record = CeleryTaskRecord.create_from_task_name(
+            self, task_name, app_name, session_id, extra=extra, **kwargs
+        )
+        return task_record
 
     failure_message = (
         f"Celery app : {app_name} failed to be created."
         "Don't worry, about this alert, "
         "this is not be an issue if you didn't explicitely planned on using celery. Issue was : "
     )
 
     logger = getLogger("pypelines.create_celery_app")
 
     if app_name in APPLICATIONS_STORE.keys():
         logger.warning(f"Tried to create a celery app named {app_name}, but it already exists. Returning it instead.")
         return APPLICATIONS_STORE[app_name]
 
-    settings_files = get_setting_files_path(conf_path, app_name)
+    settings_files = get_setting_files_path(conf_path)
 
     if len(settings_files) == 0:
         logger.warning(f"{failure_message} Could not find celery toml config files.")
         return None
 
     try:
         from dynaconf import Dynaconf
@@ -351,55 +472,19 @@
     for key, value in conf_data.items():
         try:
             setattr(app.conf, key, value)
         except Exception as e:
             logger.warning(f"{failure_message} Could assign extra attribute {key} to celery app. {e}")
             return None
 
-    APPLICATIONS_STORE[app_name] = app
-
-    from celery import Task
-
-    class handshake(Task):
-        name = f"{app_name}.handshake"
-
-        def run(self):
-            return f"{node()} is happy to shake your hand and says hello !"
-
-    def get_signature_string(signature):
-        params = [
-            param_value for param_name, param_value in signature.parameters.items() if param_name not in ["session"]
-        ]
-        return str(signature.replace(parameters=params))[1:-1].replace(" *,", "")
-
-    class tasks_infos(Task):
-        name = f"{app_name}.tasks_infos"
-
-        def run(self, app_name, selfish=False):
-            app = APPLICATIONS_STORE[app_name]
-            tasks_dynamic_data = {}
-            pipelines = getattr(app, "pipelines", {})
-            for pipeline in pipelines.values():
-                pipeline.resolve()
-                for pipe in pipeline.pipes.values():
-                    for step in pipe.steps.values():
-                        if step.complete_name in app.tasks.keys():
-                            sig = get_signature_string(step.generate.__signature__)
-                            doc = step.generate.__doc__
-                            task_data = {
-                                "signature": sig,
-                                "docstring": doc,
-                                "step_name": step.step_name,
-                                "pipe_name": step.pipe_name,
-                                "pipeline_name": step.pipeline_name,
-                                "requires": [item.complete_name for item in step.requires],
-                                "step_level_in_pipe": step.get_level(selfish=selfish),
-                            }
-                            tasks_dynamic_data[step.complete_name] = task_data
-            return tasks_dynamic_data
+    app.register_task(Handshake)
+    app.register_task(TasksInfos)
 
-    app.register_task(handshake)
-    app.register_task(tasks_infos)
+    app.get_remote_tasks = MethodType(get_remote_tasks, app)  # type: ignore
+    app.get_celery_app_tasks = MethodType(get_celery_app_tasks, app)  # type: ignore
+    app.launch_named_task_remotely = MethodType(launch_named_task_remotely, app)  # type: ignore
 
     logger.info(f"The celery app {app_name} was created successfully.")
 
+    APPLICATIONS_STORE[app_name] = app
+
     return app
```

### Comparing `processing-pypelines-0.0.44/src/pypelines/disk.py` & `processing-pypelines-0.0.45/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/examples.py` & `processing-pypelines-0.0.45/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/graphs.py` & `processing-pypelines-0.0.45/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/loggs.py` & `processing-pypelines-0.0.45/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/multisession.py` & `processing-pypelines-0.0.45/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/pickle_backend.py` & `processing-pypelines-0.0.45/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/pipelines.py` & `processing-pypelines-0.0.45/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/pipes.py` & `processing-pypelines-0.0.45/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/sessions.py` & `processing-pypelines-0.0.45/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/steps.py` & `processing-pypelines-0.0.45/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/tasks.py` & `processing-pypelines-0.0.45/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/src/pypelines/versions.py` & `processing-pypelines-0.0.45/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.44/tests/tests.py` & `processing-pypelines-0.0.45/tests/tests.py`

 * *Files identical despite different names*

