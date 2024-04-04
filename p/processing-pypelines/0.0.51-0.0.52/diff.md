# Comparing `tmp/processing-pypelines-0.0.51.tar.gz` & `tmp/processing-pypelines-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processing-pypelines-0.0.51.tar", last modified: Thu Apr  4 21:25:42 2024, max compression
+gzip compressed data, was "processing-pypelines-0.0.52.tar", last modified: Thu Apr  4 21:28:55 2024, max compression
```

## Comparing `processing-pypelines-0.0.51.tar` & `processing-pypelines-0.0.52.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.568300 processing-pypelines-0.0.51/
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:25:42.568300 processing-pypelines-0.0.51/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/requirements-celery.txt
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:25:42.568300 processing-pypelines-0.0.51/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.560300 processing-pypelines-0.0.51/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.564300 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 21:25:42.000000 processing-pypelines-0.0.51/src/processing_pypelines.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.564300 processing-pypelines-0.0.51/src/pypelines/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/accessors.py
--rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/arguments.py
--rw-rw-rw-   0 root         (0) root         (0)    21258 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/celery_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/disk.py
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/examples.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/graphs.py
--rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/loggs.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/multisession.py
--rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/pickle_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/pipes.py
--rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/steps.py
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/src/pypelines/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:25:42.564300 processing-pypelines-0.0.51/tests/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 21:25:32.000000 processing-pypelines-0.0.51/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.686454 processing-pypelines-0.0.52/
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:28:55.682454 processing-pypelines-0.0.52/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/requirements-celery.txt
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 21:28:55.686454 processing-pypelines-0.0.52/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.678454 processing-pypelines-0.0.52/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.682454 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1604 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      742 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-04 21:28:55.000000 processing-pypelines-0.0.52/src/processing_pypelines.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.682454 processing-pypelines-0.0.52/src/pypelines/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2365 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/accessors.py
+-rw-rw-rw-   0 root         (0) root         (0)     3191 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/arguments.py
+-rw-rw-rw-   0 root         (0) root         (0)    21250 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/celery_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     7301 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/disk.py
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/graphs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15517 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/loggs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/multisession.py
+-rw-rw-rw-   0 root         (0) root         (0)    14910 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/pickle_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     5669 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/pipes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)    29008 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/steps.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/src/pypelines/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 21:28:55.682454 processing-pypelines-0.0.52/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-04 21:28:44.000000 processing-pypelines-0.0.52/tests/tests.py
```

### Comparing `processing-pypelines-0.0.51/LICENSE` & `processing-pypelines-0.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/PKG-INFO` & `processing-pypelines-0.0.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.51
+Version: 0.0.52
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.51/pyproject.toml` & `processing-pypelines-0.0.52/pyproject.toml`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/processing_pypelines.egg-info/PKG-INFO` & `processing-pypelines-0.0.52/src/processing_pypelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processing-pypelines
-Version: 0.0.51
+Version: 0.0.52
 Summary: Framework to organize processing code outputs to/from disk, processing chaining and versionning with a common easy to use api
 Author-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 Maintainer-email: Timothé Jost-Mousseau <timothe.jost-mousseau@pasteur.fr>
 License: MIT
 Project-URL: homepage, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: repository, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
 Project-URL: documentation, https://gitlab.pasteur.fr/haisslab/data-management/pypelines
```

### Comparing `processing-pypelines-0.0.51/src/processing_pypelines.egg-info/SOURCES.txt` & `processing-pypelines-0.0.52/src/processing_pypelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/accessors.py` & `processing-pypelines-0.0.52/src/pypelines/accessors.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/arguments.py` & `processing-pypelines-0.0.52/src/pypelines/arguments.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/celery_tasks.py` & `processing-pypelines-0.0.52/src/pypelines/celery_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,15 @@
         task_record = CeleryTaskRecord.create_from_task_name(
             self, task_name, app_name, session_id, extra=extra, **kwargs
         )
         return task_record
 
     def is_hand_shaken(self):
         try:
-            result = self.tasks[f"{app_name}.handshake"].delay(app_name).get(timeout=1)
+            result = self.tasks[f"{app_name}.handshake"].delay().get(timeout=1)
             logger.warning(f"Handshake result : {result}")
             return True
         except ValueError:
             logger.error("No handshake result. All workers are busy ?")
             return False
 
     settings_files = get_setting_files_path(conf_path)
```

### Comparing `processing-pypelines-0.0.51/src/pypelines/disk.py` & `processing-pypelines-0.0.52/src/pypelines/disk.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/examples.py` & `processing-pypelines-0.0.52/src/pypelines/examples.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/graphs.py` & `processing-pypelines-0.0.52/src/pypelines/graphs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/loggs.py` & `processing-pypelines-0.0.52/src/pypelines/loggs.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/multisession.py` & `processing-pypelines-0.0.52/src/pypelines/multisession.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/pickle_backend.py` & `processing-pypelines-0.0.52/src/pypelines/pickle_backend.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/pipelines.py` & `processing-pypelines-0.0.52/src/pypelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/pipes.py` & `processing-pypelines-0.0.52/src/pypelines/pipes.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/sessions.py` & `processing-pypelines-0.0.52/src/pypelines/sessions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/steps.py` & `processing-pypelines-0.0.52/src/pypelines/steps.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/tasks.py` & `processing-pypelines-0.0.52/src/pypelines/tasks.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/src/pypelines/versions.py` & `processing-pypelines-0.0.52/src/pypelines/versions.py`

 * *Files identical despite different names*

### Comparing `processing-pypelines-0.0.51/tests/tests.py` & `processing-pypelines-0.0.52/tests/tests.py`

 * *Files identical despite different names*

