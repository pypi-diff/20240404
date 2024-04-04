# Comparing `tmp/processing-pypelines-0.0.48.tar.gz` & `tmp/processing-pypelines-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.48.tar", last modified: Thu Apr  4 17:53:19 2024, max compression
+gzip compressed data, was "processing-pypelines-0.0.49.tar", last modified: Thu Apr  4 19:25:45 2024, max compression
```

## Comparing `processing-pypelines-0.0.48.tar` & `processing-pypelines-0.0.49.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.950630 processing-pypelines-0.0.48/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 17:53:19.000000 processing-pypelines-0.0.48/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    20400 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 17:53:19.954630 processing-pypelines-0.0.48/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 17:53:08.000000 processing-pypelines-0.0.48/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:25:45.694859 processing-pypelines-0.0.49/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 19:25:45.694859 processing-pypelines-0.0.49/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/requirements-celery.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 19:25:45.694859 processing-pypelines-0.0.49/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:25:45.690859 processing-pypelines-0.0.49/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:25:45.694859 processing-pypelines-0.0.49/src/processing_pypelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 19:25:45.000000 processing-pypelines-0.0.49/src/processing_pypelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 19:25:45.000000 processing-pypelines-0.0.49/src/processing_pypelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:25:45.000000 processing-pypelines-0.0.49/src/processing_pypelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 19:25:45.000000 processing-pypelines-0.0.49/src/processing_pypelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 19:25:45.000000 processing-pypelines-0.0.49/src/processing_pypelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:25:45.694859 processing-pypelines-0.0.49/src/pypelines/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    20542 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/celery_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/disk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/loggs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/multisession.py
+-rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/pickle_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/pipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/src/pypelines/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:25:45.694859 processing-pypelines-0.0.49/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 19:25:34.000000 processing-pypelines-0.0.49/tests/tests.py
```

### Comparing `processing-pypelines-0.0.48/LICENSE` & `processing-pypelines-0.0.49/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/PKG-INFO` & `processing-pypelines-0.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.48
+Version: 0.0.49
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.48/pyproject.toml` & `processing-pypelines-0.0.49/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/processing_pypelines.egg-info/PKG-INFO` & `processing-pypelines-0.0.49/src/processing_pypelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.48
+Version: 0.0.49
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.48/src/processing_pypelines.egg-info/SOURCES.txt` & `processing-pypelines-0.0.49/src/processing_pypelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/accessors.py` & `processing-pypelines-0.0.49/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/arguments.py` & `processing-pypelines-0.0.49/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/celery_tasks.py` & `processing-pypelines-0.0.49/src/pypelines/celery_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,16 +312,34 @@
         self.logger.addHandler(fh)
 
     def remove_handler(self):
         self.logger.removeHandler(self.logger.handlers[-1])
 
 
 def create_celery_app(conf_path, app_name="pypelines", v_host=None) -> "Celery | None":
+
+    failure_message = (
+        f"Celery app : {app_name} failed to be created."
+        "Don't worry, about this alert, "
+        "this is not be an issue if you didn't explicitely planned on using celery. Issue was : "
+    )
+
+    logger = getLogger("pypelines.create_celery_app")
+
+    if app_name in APPLICATIONS_STORE.keys():
+        logger.warning(f"Tried to create a celery app named {app_name}, but it already exists. Returning it instead.")
+        return APPLICATIONS_STORE[app_name]
+
+    try:
+        from celery import Task
+    except ImportError as e:
+        logger.warning(f"{failure_message} Could not import celery app. {e}")
+        return None
+
     from types import MethodType
-    from celery import Task
 
     def get_setting_files_path(conf_path) -> List[Path]:
         conf_path = Path(conf_path)
         if conf_path.is_file():
             conf_path = conf_path.parent
         files = []
         for prefix, suffix in zip(["", "."], ["", "_secrets"]):
@@ -476,26 +494,14 @@
 
     def launch_named_task_remotely(self, session_id, task_name, extra=None, kwargs={}):
         task_record = CeleryTaskRecord.create_from_task_name(
             self, task_name, app_name, session_id, extra=extra, **kwargs
         )
         return task_record
 
-    failure_message = (
-        f"Celery app : {app_name} failed to be created."
-        "Don't worry, about this alert, "
-        "this is not be an issue if you didn't explicitely planned on using celery. Issue was : "
-    )
-
-    logger = getLogger("pypelines.create_celery_app")
-
-    if app_name in APPLICATIONS_STORE.keys():
-        logger.warning(f"Tried to create a celery app named {app_name}, but it already exists. Returning it instead.")
-        return APPLICATIONS_STORE[app_name]
-
     settings_files = get_setting_files_path(conf_path)
 
     if len(settings_files) == 0:
         logger.warning(f"{failure_message} Could not find celery toml config files.")
         return None
 
     try:
```

### Comparing `processing-pypelines-0.0.48/src/pypelines/disk.py` & `processing-pypelines-0.0.49/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/examples.py` & `processing-pypelines-0.0.49/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/graphs.py` & `processing-pypelines-0.0.49/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/loggs.py` & `processing-pypelines-0.0.49/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/multisession.py` & `processing-pypelines-0.0.49/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/pickle_backend.py` & `processing-pypelines-0.0.49/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/pipelines.py` & `processing-pypelines-0.0.49/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/pipes.py` & `processing-pypelines-0.0.49/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/sessions.py` & `processing-pypelines-0.0.49/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/steps.py` & `processing-pypelines-0.0.49/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/tasks.py` & `processing-pypelines-0.0.49/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/src/pypelines/versions.py` & `processing-pypelines-0.0.49/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.48/tests/tests.py` & `processing-pypelines-0.0.49/tests/tests.py`

 * *Files identical despite different names*

