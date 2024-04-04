# Comparing `tmp/taskara-0.1.6.tar.gz` & `tmp/taskara-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.6.tar", max compression
+gzip compressed data, was "taskara-0.1.7.tar", max compression
```

## Comparing `taskara-0.1.6.tar` & `taskara-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.6/LICENSE
--rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.6/README.md
--rw-r--r--   0        0        0      392 2024-04-04 16:39:23.904286 taskara-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.6/taskara/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.6/taskara/db/conn.py
--rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.6/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.6/taskara/env.py
--rw-r--r--   0        0        0     1513 2024-04-04 16:36:43.488474 taskara-0.1.6/taskara/models.py
--rw-r--r--   0        0        0    18774 2024-04-04 16:39:10.464672 taskara-0.1.6/taskara/task.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.7/LICENSE
+-rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.7/README.md
+-rw-r--r--   0        0        0      392 2024-04-04 17:21:39.608405 taskara-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.7/taskara/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.7/taskara/db/conn.py
+-rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.7/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.7/taskara/env.py
+-rw-r--r--   0        0        0     1513 2024-04-04 16:36:43.488474 taskara-0.1.7/taskara/models.py
+-rw-r--r--   0        0        0    18410 2024-04-04 17:21:05.365064 taskara-0.1.7/taskara/task.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.7/PKG-INFO
```

### Comparing `taskara-0.1.6/LICENSE` & `taskara-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.6/README.md` & `taskara-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.6/taskara/db/conn.py` & `taskara-0.1.7/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.6/taskara/db/models.py` & `taskara-0.1.7/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.6/taskara/models.py` & `taskara-0.1.7/taskara/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.6/taskara/task.py` & `taskara-0.1.7/taskara/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,30 +133,14 @@
         return self._completed
 
     @completed.setter
     def completed(self, value: float):
         self._completed = value
 
     @property
-    def feed(self) -> RoleThread:
-        return self._feed
-
-    @feed.setter
-    def feed(self, value: RoleThread):
-        self._feed = value
-
-    @property
-    def thread(self) -> RoleThread:
-        return self._thread
-
-    @thread.setter
-    def thread(self, value: RoleThread):
-        self._thread = value
-
-    @property
     def threads(self) -> List[RoleThread]:
         return self._threads
 
     @threads.setter
     def threads(self, value: List[RoleThread]):
         self._threads = value
 
@@ -196,15 +180,14 @@
             description=self._description,
             url=self._url,
             status=self._status,
             created=self._created,
             started=self._started,
             completed=self._completed,
             assigned_to=self._assigned_to,
-            feed_id=self._feed._id,
             error=self._error,
             output=self._output,
             threads=json.dumps([t._id for t in self._threads]),
             version=self._version,
         )
 
     @classmethod
```

### Comparing `taskara-0.1.6/PKG-INFO` & `taskara-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.6
+Version: 0.1.7
 Summary: Task management for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

