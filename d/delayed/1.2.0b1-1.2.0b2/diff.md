# Comparing `tmp/delayed-1.2.0b1.tar.gz` & `tmp/delayed-1.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delayed-1.2.0b1.tar", last modified: Tue Apr  2 08:31:18 2024, max compression
+gzip compressed data, was "delayed-1.2.0b2.tar", last modified: Thu Apr  4 04:40:23 2024, max compression
```

## Comparing `delayed-1.2.0b1.tar` & `delayed-1.2.0b2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-02 08:31:18.624708 delayed-1.2.0b1/
--rw-r--r--   0 keakon     (501) staff       (20)     1063 2024-03-27 06:18:19.000000 delayed-1.2.0b1/LICENSE
--rw-r--r--   0 keakon     (501) staff       (20)       16 2024-03-27 06:18:19.000000 delayed-1.2.0b1/MANIFEST.in
--rw-r--r--   0 keakon     (501) staff       (20)     9537 2024-04-02 08:31:18.624583 delayed-1.2.0b1/PKG-INFO
--rw-r--r--   0 keakon     (501) staff       (20)     8701 2024-04-02 08:30:03.000000 delayed-1.2.0b1/README.md
-drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-02 08:31:18.621639 delayed-1.2.0b1/delayed/
--rw-r--r--   0 keakon     (501) staff       (20)       49 2024-04-02 08:30:34.000000 delayed-1.2.0b1/delayed/__init__.py
--rw-r--r--   0 keakon     (501) staff       (20)      169 2024-03-29 02:03:21.000000 delayed-1.2.0b1/delayed/constants.py
--rw-r--r--   0 keakon     (501) staff       (20)     1120 2024-04-02 07:53:33.000000 delayed-1.2.0b1/delayed/delay.py
--rw-r--r--   0 keakon     (501) staff       (20)      837 2024-03-29 07:45:55.000000 delayed-1.2.0b1/delayed/keep_alive.py
--rw-r--r--   0 keakon     (501) staff       (20)     1767 2024-03-29 03:24:55.000000 delayed-1.2.0b1/delayed/logger.py
--rw-r--r--   0 keakon     (501) staff       (20)     5538 2024-04-02 08:16:56.000000 delayed-1.2.0b1/delayed/queue.py
--rw-r--r--   0 keakon     (501) staff       (20)     1306 2024-03-27 09:39:19.000000 delayed-1.2.0b1/delayed/sweeper.py
--rw-r--r--   0 keakon     (501) staff       (20)     3706 2024-04-02 08:26:28.000000 delayed-1.2.0b1/delayed/task.py
--rw-r--r--   0 keakon     (501) staff       (20)     5107 2024-04-02 08:24:26.000000 delayed-1.2.0b1/delayed/worker.py
-drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-02 08:31:18.624266 delayed-1.2.0b1/delayed.egg-info/
--rw-r--r--   0 keakon     (501) staff       (20)     9537 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/PKG-INFO
--rw-r--r--   0 keakon     (501) staff       (20)      518 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/SOURCES.txt
--rw-r--r--   0 keakon     (501) staff       (20)        1 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/dependency_links.txt
--rw-r--r--   0 keakon     (501) staff       (20)       22 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/requires.txt
--rw-r--r--   0 keakon     (501) staff       (20)        8 2024-04-02 08:31:18.000000 delayed-1.2.0b1/delayed.egg-info/top_level.txt
--rw-r--r--   0 keakon     (501) staff       (20)      191 2024-04-02 08:31:18.624961 delayed-1.2.0b1/setup.cfg
--rw-r--r--   0 keakon     (501) staff       (20)     1092 2024-03-27 08:23:52.000000 delayed-1.2.0b1/setup.py
-drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-02 08:31:18.623979 delayed-1.2.0b1/tests/
--rw-r--r--   0 keakon     (501) staff       (20)     1555 2024-04-02 08:07:47.000000 delayed-1.2.0b1/tests/test_delay.py
--rw-r--r--   0 keakon     (501) staff       (20)      415 2024-03-27 06:18:19.000000 delayed-1.2.0b1/tests/test_keep_alive.py
--rw-r--r--   0 keakon     (501) staff       (20)      687 2024-03-27 06:18:19.000000 delayed-1.2.0b1/tests/test_logger.py
--rw-r--r--   0 keakon     (501) staff       (20)     4435 2024-03-29 08:23:53.000000 delayed-1.2.0b1/tests/test_queue.py
--rw-r--r--   0 keakon     (501) staff       (20)     1396 2024-03-29 07:35:04.000000 delayed-1.2.0b1/tests/test_sweeper.py
--rw-r--r--   0 keakon     (501) staff       (20)     3384 2024-04-02 05:30:19.000000 delayed-1.2.0b1/tests/test_task.py
--rw-r--r--   0 keakon     (501) staff       (20)     1198 2024-04-02 08:27:47.000000 delayed-1.2.0b1/tests/test_worker.py
+drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-04 04:40:23.680765 delayed-1.2.0b2/
+-rw-r--r--   0 keakon     (501) staff       (20)     1063 2024-03-27 06:18:19.000000 delayed-1.2.0b2/LICENSE
+-rw-r--r--   0 keakon     (501) staff       (20)       16 2024-03-27 06:18:19.000000 delayed-1.2.0b2/MANIFEST.in
+-rw-r--r--   0 keakon     (501) staff       (20)     9537 2024-04-04 04:40:23.680650 delayed-1.2.0b2/PKG-INFO
+-rw-r--r--   0 keakon     (501) staff       (20)     8701 2024-04-02 08:36:06.000000 delayed-1.2.0b2/README.md
+drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-04 04:40:23.677602 delayed-1.2.0b2/delayed/
+-rw-r--r--   0 keakon     (501) staff       (20)       49 2024-04-04 03:53:14.000000 delayed-1.2.0b2/delayed/__init__.py
+-rw-r--r--   0 keakon     (501) staff       (20)      169 2024-03-29 02:03:21.000000 delayed-1.2.0b2/delayed/constants.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1120 2024-04-02 08:36:06.000000 delayed-1.2.0b2/delayed/delay.py
+-rw-r--r--   0 keakon     (501) staff       (20)      837 2024-03-29 07:45:55.000000 delayed-1.2.0b2/delayed/keep_alive.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1767 2024-03-29 03:24:55.000000 delayed-1.2.0b2/delayed/logger.py
+-rw-r--r--   0 keakon     (501) staff       (20)     5538 2024-04-02 08:36:06.000000 delayed-1.2.0b2/delayed/queue.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1306 2024-03-27 09:39:19.000000 delayed-1.2.0b2/delayed/sweeper.py
+-rw-r--r--   0 keakon     (501) staff       (20)     3706 2024-04-04 04:03:39.000000 delayed-1.2.0b2/delayed/task.py
+-rw-r--r--   0 keakon     (501) staff       (20)     5107 2024-04-02 08:36:06.000000 delayed-1.2.0b2/delayed/worker.py
+drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-04 04:40:23.680196 delayed-1.2.0b2/delayed.egg-info/
+-rw-r--r--   0 keakon     (501) staff       (20)     9537 2024-04-04 04:40:23.000000 delayed-1.2.0b2/delayed.egg-info/PKG-INFO
+-rw-r--r--   0 keakon     (501) staff       (20)      518 2024-04-04 04:40:23.000000 delayed-1.2.0b2/delayed.egg-info/SOURCES.txt
+-rw-r--r--   0 keakon     (501) staff       (20)        1 2024-04-04 04:40:23.000000 delayed-1.2.0b2/delayed.egg-info/dependency_links.txt
+-rw-r--r--   0 keakon     (501) staff       (20)       22 2024-04-04 04:40:23.000000 delayed-1.2.0b2/delayed.egg-info/requires.txt
+-rw-r--r--   0 keakon     (501) staff       (20)        8 2024-04-04 04:40:23.000000 delayed-1.2.0b2/delayed.egg-info/top_level.txt
+-rw-r--r--   0 keakon     (501) staff       (20)      191 2024-04-04 04:40:23.681035 delayed-1.2.0b2/setup.cfg
+-rw-r--r--   0 keakon     (501) staff       (20)     1092 2024-03-27 08:23:52.000000 delayed-1.2.0b2/setup.py
+drwxr-xr-x   0 keakon     (501) staff       (20)        0 2024-04-04 04:40:23.679979 delayed-1.2.0b2/tests/
+-rw-r--r--   0 keakon     (501) staff       (20)     1555 2024-04-02 08:36:06.000000 delayed-1.2.0b2/tests/test_delay.py
+-rw-r--r--   0 keakon     (501) staff       (20)      415 2024-03-27 06:18:19.000000 delayed-1.2.0b2/tests/test_keep_alive.py
+-rw-r--r--   0 keakon     (501) staff       (20)      687 2024-03-27 06:18:19.000000 delayed-1.2.0b2/tests/test_logger.py
+-rw-r--r--   0 keakon     (501) staff       (20)     4435 2024-03-29 08:23:53.000000 delayed-1.2.0b2/tests/test_queue.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1396 2024-04-04 04:02:33.000000 delayed-1.2.0b2/tests/test_sweeper.py
+-rw-r--r--   0 keakon     (501) staff       (20)     3384 2024-04-02 08:36:06.000000 delayed-1.2.0b2/tests/test_task.py
+-rw-r--r--   0 keakon     (501) staff       (20)     1113 2024-04-04 04:02:47.000000 delayed-1.2.0b2/tests/test_worker.py
```

### Comparing `delayed-1.2.0b1/LICENSE` & `delayed-1.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/PKG-INFO` & `delayed-1.2.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delayed
-Version: 1.2.0b1
+Version: 1.2.0b2
 Summary: a simple but robust task queue
 Home-page: https://github.com/keakon/delayed
 Author: keakon
 Author-email: keakon@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `delayed-1.2.0b1/README.md` & `delayed-1.2.0b2/README.md`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/delayed/delay.py` & `delayed-1.2.0b2/delayed/delay.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/delayed/keep_alive.py` & `delayed-1.2.0b2/delayed/keep_alive.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/delayed/logger.py` & `delayed-1.2.0b2/delayed/logger.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/delayed/queue.py` & `delayed-1.2.0b2/delayed/queue.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/delayed/sweeper.py` & `delayed-1.2.0b2/delayed/sweeper.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/delayed/task.py` & `delayed-1.2.0b2/delayed/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         Returns:
             bytes: The serialized data.
         """
         if self._data is None:
             data = self._func_path, self._args, self._kwargs, self._retry
 
             i = 0
-            if self._retry <= 0:
+            if self._retry == 0:
                 i -= 1
                 if not self._kwargs:
                     i -= 1
                     if not self._args:
                         i -= 1
             if i < 0:
                 data = data[:i]
```

### Comparing `delayed-1.2.0b1/delayed/worker.py` & `delayed-1.2.0b2/delayed/worker.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/delayed.egg-info/PKG-INFO` & `delayed-1.2.0b2/delayed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delayed
-Version: 1.2.0b1
+Version: 1.2.0b2
 Summary: a simple but robust task queue
 Home-page: https://github.com/keakon/delayed
 Author: keakon
 Author-email: keakon@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `delayed-1.2.0b1/delayed.egg-info/SOURCES.txt` & `delayed-1.2.0b2/delayed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/setup.py` & `delayed-1.2.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/tests/test_delay.py` & `delayed-1.2.0b2/tests/test_delay.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/tests/test_logger.py` & `delayed-1.2.0b2/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/tests/test_queue.py` & `delayed-1.2.0b2/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/tests/test_sweeper.py` & `delayed-1.2.0b2/tests/test_sweeper.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/tests/test_task.py` & `delayed-1.2.0b2/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `delayed-1.2.0b1/tests/test_worker.py` & `delayed-1.2.0b2/tests/test_worker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 # -*- coding: utf-8 -*-
 
-import os
-import signal
-
 from delayed.task import PyTask
 from delayed.queue import Queue
 from delayed.worker import Worker
 
 from .common import CONN, func3, NOTI_KEY, PROCESSING_KEY, QUEUE, QUEUE_NAME, WORKER
 
 
-def stop(pid: int):
-    os.kill(pid, signal.SIGHUP)
-
-
 class TestWorker:
     def test_generate_id(self):
         QUEUE.go_offline()  # make sure no worker ids are used
 
         queue1 = Queue(QUEUE_NAME, conn=CONN)
         worker1 = Worker(queue1, id_bits=1)
         worker1.generate_id()
@@ -35,14 +28,13 @@
         queue2.go_offline()
 
     def test_run(self):
         CONN.delete(QUEUE_NAME, NOTI_KEY, PROCESSING_KEY)
 
         task = PyTask(func3, retry=1)
         QUEUE.enqueue(task)
-
-        task = PyTask(stop, (os.getpid(),))
+        task = PyTask(func3, retry=-1)
         QUEUE.enqueue(task)
 
         WORKER.run()
 
         CONN.delete(QUEUE_NAME, NOTI_KEY, PROCESSING_KEY)
```

