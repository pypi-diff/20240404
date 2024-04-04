# Comparing `tmp/taskara-0.1.5.tar.gz` & `tmp/taskara-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.5.tar", max compression
+gzip compressed data, was "taskara-0.1.6.tar", max compression
```

## Comparing `taskara-0.1.5.tar` & `taskara-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.5/LICENSE
--rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.5/README.md
--rw-r--r--   0        0        0      392 2024-04-03 04:11:38.811051 taskara-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.5/taskara/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.5/taskara/db/conn.py
--rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.5/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.5/taskara/env.py
--rw-r--r--   0        0        0     1513 2024-04-03 02:25:02.082624 taskara-0.1.5/taskara/models.py
--rw-r--r--   0        0        0    18840 2024-04-03 02:34:10.525445 taskara-0.1.5/taskara/task.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.6/LICENSE
+-rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.6/README.md
+-rw-r--r--   0        0        0      392 2024-04-04 16:39:23.904286 taskara-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.6/taskara/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.6/taskara/db/conn.py
+-rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.6/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.6/taskara/env.py
+-rw-r--r--   0        0        0     1513 2024-04-04 16:36:43.488474 taskara-0.1.6/taskara/models.py
+-rw-r--r--   0        0        0    18774 2024-04-04 16:39:10.464672 taskara-0.1.6/taskara/task.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.6/PKG-INFO
```

### Comparing `taskara-0.1.5/LICENSE` & `taskara-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.5/README.md` & `taskara-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.5/taskara/db/conn.py` & `taskara-0.1.6/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.5/taskara/db/models.py` & `taskara-0.1.6/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.5/taskara/models.py` & `taskara-0.1.6/taskara/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.5/taskara/task.py` & `taskara-0.1.6/taskara/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,14 @@
             owner_id=self._owner_id,
             description=self._description,
             url=self._url,
             status=self._status,
             created=self._created,
             started=self._started,
             completed=self._completed,
-            thread_id=self._thread._id,
             assigned_to=self._assigned_to,
             feed_id=self._feed._id,
             error=self._error,
             output=self._output,
             threads=json.dumps([t._id for t in self._threads]),
             version=self._version,
         )
@@ -275,29 +274,29 @@
         self,
         name: Optional[str] = None,
         public: bool = False,
         metadata: Optional[dict] = None,
         id: Optional[str] = None,
     ) -> None:
         if hasattr(self, "_remote") and self._remote:
-            print("creting remote work thread")
+            print("creting remote thread")
             self._remote_request(
                 self._remote,
                 "POST",
                 f"/v1/tasks/{self._id}/threads",
                 {"name": name, "public": public, "metadata": metadata, "id": id},
             )
-            print("removed remote work thread")
+            print("removed remote thread")
             return
 
-        print("creating local work thread")
+        print("creating thread")
         thread = RoleThread(self.owner_id, public, name, metadata)
         self._threads.append(thread)
         self.save()
-        print("created local work thread")
+        print("created local thread")
         return
 
     def remove_thread(self, thread_id: str) -> None:
         if hasattr(self, "_remote") and self._remote:
             print("removing remote thread")
             self._remote_request(
                 self._remote,
```

### Comparing `taskara-0.1.5/PKG-INFO` & `taskara-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.5
+Version: 0.1.6
 Summary: Task management for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

