# Comparing `tmp/DOLOST-1.0rc1.tar.gz` & `tmp/DOLOST-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DOLOST-1.0rc1.tar", last modified: Fri Mar 29 20:18:53 2024, max compression
+gzip compressed data, was "DOLOST-1.1.tar", last modified: Thu Apr  4 21:17:42 2024, max compression
```

## Comparing `DOLOST-1.0rc1.tar` & `DOLOST-1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:18:53.420472 DOLOST-1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-03-29 20:18:53.420472 DOLOST-1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 20:18:53.420472 DOLOST-1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:18:53.416472 DOLOST-1.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:18:53.416472 DOLOST-1.0rc1/src/DOLOST/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:18:53.420472 DOLOST-1.0rc1/src/DOLOST/blueprints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23974 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/blueprints/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/blueprints/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/blueprints/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:18:53.420472 DOLOST-1.0rc1/src/DOLOST/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/services/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/services/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/services/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-29 20:18:40.000000 DOLOST-1.0rc1/src/DOLOST/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:18:53.420472 DOLOST-1.0rc1/src/DOLOST.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-03-29 20:18:53.000000 DOLOST-1.0rc1/src/DOLOST.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-29 20:18:53.000000 DOLOST-1.0rc1/src/DOLOST.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 20:18:53.000000 DOLOST-1.0rc1/src/DOLOST.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 20:18:53.000000 DOLOST-1.0rc1/src/DOLOST.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-29 20:18:53.000000 DOLOST-1.0rc1/src/DOLOST.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 20:18:53.000000 DOLOST-1.0rc1/src/DOLOST.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:42.509534 DOLOST-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 21:17:22.000000 DOLOST-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-04 21:17:42.505534 DOLOST-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-04 21:17:22.000000 DOLOST-1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:17:42.509534 DOLOST-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-04 21:17:22.000000 DOLOST-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:42.501534 DOLOST-1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:42.505534 DOLOST-1.1/src/DOLOST/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:42.505534 DOLOST-1.1/src/DOLOST/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23974 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/blueprints/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/blueprints/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/blueprints/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:42.505534 DOLOST-1.1/src/DOLOST/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/services/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/services/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 21:17:22.000000 DOLOST-1.1/src/DOLOST/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:17:42.505534 DOLOST-1.1/src/DOLOST.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-04 21:17:42.000000 DOLOST-1.1/src/DOLOST.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-04 21:17:42.000000 DOLOST-1.1/src/DOLOST.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:17:42.000000 DOLOST-1.1/src/DOLOST.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 21:17:42.000000 DOLOST-1.1/src/DOLOST.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 21:17:42.000000 DOLOST-1.1/src/DOLOST.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 21:17:42.000000 DOLOST-1.1/src/DOLOST.egg-info/top_level.txt
```

### Comparing `DOLOST-1.0rc1/LICENSE` & `DOLOST-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/PKG-INFO` & `DOLOST-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DOLOST
-Version: 1.0rc1
+Version: 1.1
 Summary: Deceptive Operations: Lure, Observe, and Secure Tool
 Home-page: https://github.com/Base4Security/DOLOS-T/
 Author-email: idi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/DOLOS-T/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: DOLOST Version: 1.0rc1 Summary: Deceptive
-Operations: Lure, Observe, and Secure Tool Home-page: https://github.com/
-Base4Security/DOLOS-T/ Author-email: idi@base4sec.com Project-URL: Bug Tracker,
-https://github.com/Base4Security/DOLOS-T/issues Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
-Libraries :: Application Frameworks Classifier: Operating System :: OS
-Independent Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: flask Requires-Dist: docker Requires-Dist: flask-socketio
-Requires-Dist: gevent-websocket
+Metadata-Version: 2.1 Name: DOLOST Version: 1.1 Summary: Deceptive Operations:
+Lure, Observe, and Secure Tool Home-page: https://github.com/Base4Security/
+DOLOS-T/ Author-email: idi@base4sec.com Project-URL: Bug Tracker, https://
+github.com/Base4Security/DOLOS-T/issues Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+flask Requires-Dist: docker Requires-Dist: flask-socketio Requires-Dist:
+gevent-websocket
                                    _[_D_O_L_O_S_T_]
                                ******** DDOOLLOOSSTT ********
          ****** DDeecceeppttiivvee OOppeerraattiioonnss:: LLuurree,, OObbsseerrvvee,, aanndd SSeeccuurree TTooooll ******
 ===============================================================================
  [![Status](https://img.shields.io/badge/status-active-success.svg)]() [![PyPI
 version](https://badge.fury.io/py/dolost.svg)](https://badge.fury.io/py/dolost)
     [![Documentation Status](https://readthedocs.org/projects/dolost/badge/
```

### Comparing `DOLOST-1.0rc1/README.md` & `DOLOST-1.1/README.md`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/setup.py` & `DOLOST-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/src/DOLOST/app.py` & `DOLOST-1.1/src/DOLOST/app.py`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/src/DOLOST/blueprints/api.py` & `DOLOST-1.1/src/DOLOST/blueprints/api.py`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/src/DOLOST/blueprints/views.py` & `DOLOST-1.1/src/DOLOST/blueprints/views.py`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/src/DOLOST/blueprints/websocket.py` & `DOLOST-1.1/src/DOLOST/blueprints/websocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,29 +58,28 @@
     def send_activity_logs(self):
         """
         Send activity logs to clients.
 
         Continuously fetches and emits activity logs until stop event is set.
 
         """
-        auxcount = 0
         while not self.thread_stop_event.is_set():
             logs = ActivityViewer.review_logs()
             self.emit('activity_logs', {'logs': logs})
 
             observable_ips = ActivityViewer.review_observable_ips()
             self.emit('activity_observable_ips', {'observable_ips': observable_ips})
-            
-            self.thread_stop_event.wait(5)  # Wait for 5 second before sending next update
 
-            # Auxiliary function turn on crond every 60 seconds
-            if (auxcount == 0):
-                ActivityViewer.turn_on_crond()
-                auxcount = 60
-            auxcount = auxcount - 1
+            observable_usage = ActivityViewer.review_observable_usage()
+            self.emit('activity_observable_usage', {'observable_usage': observable_usage})
+
+            observable_interesting = ActivityViewer.review_interesting_observable()
+            self.emit('activity_observable_interesting', {'observable_interesting': observable_interesting})
+
+            self.thread_stop_event.wait(5)  # Wait for 5 second before sending next update
 
     def on_request_activity(self):
         """
         Callback function triggered on request for activity logs.
 
         Starts a new thread to continuously send activity logs to clients.
```

### Comparing `DOLOST-1.0rc1/src/DOLOST/cli.py` & `DOLOST-1.1/src/DOLOST/cli.py`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/src/DOLOST/context.py` & `DOLOST-1.1/src/DOLOST/context.py`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/src/DOLOST/services/docker_manager.py` & `DOLOST-1.1/src/DOLOST/services/docker_manager.py`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/src/DOLOST/services/logger.py` & `DOLOST-1.1/src/DOLOST/services/logger.py`

 * *Files identical despite different names*

### Comparing `DOLOST-1.0rc1/src/DOLOST.egg-info/PKG-INFO` & `DOLOST-1.1/src/DOLOST.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DOLOST
-Version: 1.0rc1
+Version: 1.1
 Summary: Deceptive Operations: Lure, Observe, and Secure Tool
 Home-page: https://github.com/Base4Security/DOLOS-T/
 Author-email: idi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/DOLOS-T/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: DOLOST Version: 1.0rc1 Summary: Deceptive
-Operations: Lure, Observe, and Secure Tool Home-page: https://github.com/
-Base4Security/DOLOS-T/ Author-email: idi@base4sec.com Project-URL: Bug Tracker,
-https://github.com/Base4Security/DOLOS-T/issues Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
-Libraries :: Application Frameworks Classifier: Operating System :: OS
-Independent Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: flask Requires-Dist: docker Requires-Dist: flask-socketio
-Requires-Dist: gevent-websocket
+Metadata-Version: 2.1 Name: DOLOST Version: 1.1 Summary: Deceptive Operations:
+Lure, Observe, and Secure Tool Home-page: https://github.com/Base4Security/
+DOLOS-T/ Author-email: idi@base4sec.com Project-URL: Bug Tracker, https://
+github.com/Base4Security/DOLOS-T/issues Classifier: Programming Language ::
+Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
+v3 (GPLv3) Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+flask Requires-Dist: docker Requires-Dist: flask-socketio Requires-Dist:
+gevent-websocket
                                    _[_D_O_L_O_S_T_]
                                ******** DDOOLLOOSSTT ********
          ****** DDeecceeppttiivvee OOppeerraattiioonnss:: LLuurree,, OObbsseerrvvee,, aanndd SSeeccuurree TTooooll ******
 ===============================================================================
  [![Status](https://img.shields.io/badge/status-active-success.svg)]() [![PyPI
 version](https://badge.fury.io/py/dolost.svg)](https://badge.fury.io/py/dolost)
     [![Documentation Status](https://readthedocs.org/projects/dolost/badge/
```

### Comparing `DOLOST-1.0rc1/src/DOLOST.egg-info/SOURCES.txt` & `DOLOST-1.1/src/DOLOST.egg-info/SOURCES.txt`

 * *Files identical despite different names*

