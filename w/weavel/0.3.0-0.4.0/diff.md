# Comparing `tmp/weavel-0.3.0.tar.gz` & `tmp/weavel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weavel-0.3.0.tar", last modified: Thu Mar 21 11:41:37 2024, max compression
+gzip compressed data, was "weavel-0.4.0.tar", last modified: Thu Apr  4 12:08:44 2024, max compression
```

## Comparing `weavel-0.3.0.tar` & `weavel-0.4.0.tar`

### file list

```diff
@@ -1,55 +1,29 @@
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.008838 weavel-0.3.0/
--rw-r--r--   0 jypark     (501) staff       (20)        0 2024-01-15 02:29:57.000000 weavel-0.3.0/LICENSE
--rw-r--r--   0 jypark     (501) staff       (20)      406 2024-03-21 11:41:37.008696 weavel-0.3.0/PKG-INFO
--rw-r--r--   0 jypark     (501) staff       (20)       15 2024-02-08 04:16:27.000000 weavel-0.3.0/README.md
--rw-r--r--   0 jypark     (501) staff       (20)       38 2024-03-21 11:41:37.008884 weavel-0.3.0/setup.cfg
--rw-r--r--   0 jypark     (501) staff       (20)     1248 2024-03-21 11:40:58.000000 weavel-0.3.0/setup.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.002670 weavel-0.3.0/testapp/
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.003066 weavel-0.3.0/testapp/daily_dialog/
--rw-r--r--   0 jypark     (501) staff       (20)     9480 2024-02-06 10:50:36.000000 weavel-0.3.0/testapp/daily_dialog/run_qa_extractor.py
--rw-r--r--   0 jypark     (501) staff       (20)     8672 2024-02-06 10:50:37.000000 weavel-0.3.0/testapp/daily_dialog/run_qa_extractor_on_chatalpaca.py
--rw-r--r--   0 jypark     (501) staff       (20)     4110 2024-02-06 12:05:08.000000 weavel-0.3.0/testapp/daily_dialog/save_to_db.py
--rw-r--r--   0 jypark     (501) staff       (20)     1298 2024-03-21 06:59:25.000000 weavel-0.3.0/testapp/demo.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.003531 weavel-0.3.0/testapp/py_files/
--rw-r--r--   0 jypark     (501) staff       (20)     1065 2024-01-24 05:01:55.000000 weavel-0.3.0/testapp/py_files/duplicate_log_test.py
--rw-r--r--   0 jypark     (501) staff       (20)     1892 2024-01-30 03:05:12.000000 weavel-0.3.0/testapp/py_files/poe_test.py
--rw-r--r--   0 jypark     (501) staff       (20)     1068 2024-01-24 07:27:52.000000 weavel-0.3.0/testapp/py_files/save_mock_data.py
--rw-r--r--   0 jypark     (501) staff       (20)     1160 2024-01-24 11:29:54.000000 weavel-0.3.0/testapp/py_files/save_mock_retention_data.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.001984 weavel-0.3.0/venv/
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.006169 weavel-0.3.0/venv/bin/
--rwxr-xr-x   0 jypark     (501) staff       (20)     8236 2024-02-02 10:25:14.000000 weavel-0.3.0/venv/bin/pwiz.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      648 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2html.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      770 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 jypark     (501) staff       (20)     1105 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      847 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      670 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2man.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      836 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      642 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      655 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      691 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      927 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      656 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 jypark     (501) staff       (20)      724 2024-01-15 02:43:20.000000 weavel-0.3.0/venv/bin/rstpep2html.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.007043 weavel-0.3.0/weavel/
--rw-r--r--   0 jypark     (501) staff       (20)      106 2024-03-21 11:41:03.000000 weavel-0.3.0/weavel/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     6063 2024-02-08 04:18:02.000000 weavel-0.3.0/weavel/_api_client.py
--rw-r--r--   0 jypark     (501) staff       (20)     1645 2024-03-21 11:07:52.000000 weavel-0.3.0/weavel/_buffer_storage.py
--rw-r--r--   0 jypark     (501) staff       (20)      211 2024-03-21 09:39:03.000000 weavel-0.3.0/weavel/_constants.py
--rw-r--r--   0 jypark     (501) staff       (20)     8464 2024-03-21 11:10:05.000000 weavel-0.3.0/weavel/_worker.py
--rw-r--r--   0 jypark     (501) staff       (20)     3638 2024-03-21 10:56:32.000000 weavel-0.3.0/weavel/client.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.008149 weavel-0.3.0/weavel/poe/
--rw-r--r--   0 jypark     (501) staff       (20)       58 2024-01-30 04:23:45.000000 weavel-0.3.0/weavel/poe/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     1749 2024-03-21 10:51:40.000000 weavel-0.3.0/weavel/poe/_poe_buffer_storage.py
--rw-r--r--   0 jypark     (501) staff       (20)     4756 2024-03-21 10:51:40.000000 weavel-0.3.0/weavel/poe/_poe_worker.py
--rw-r--r--   0 jypark     (501) staff       (20)     1278 2024-03-21 10:56:32.000000 weavel-0.3.0/weavel/poe/poe_client.py
--rw-r--r--   0 jypark     (501) staff       (20)     2471 2024-03-21 10:55:55.000000 weavel-0.3.0/weavel/types.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.008497 weavel-0.3.0/weavel/utils/
--rw-r--r--   0 jypark     (501) staff       (20)       43 2024-01-15 06:20:46.000000 weavel-0.3.0/weavel/utils/__init__.py
--rw-r--r--   0 jypark     (501) staff       (20)     1134 2024-01-15 05:54:15.000000 weavel-0.3.0/weavel/utils/crypto.py
--rw-r--r--   0 jypark     (501) staff       (20)      679 2024-01-15 11:33:18.000000 weavel-0.3.0/weavel/utils/logger.py
-drwxr-xr-x   0 jypark     (501) staff       (20)        0 2024-03-21 11:41:37.007683 weavel-0.3.0/weavel.egg-info/
--rw-r--r--   0 jypark     (501) staff       (20)      406 2024-03-21 11:41:36.000000 weavel-0.3.0/weavel.egg-info/PKG-INFO
--rw-r--r--   0 jypark     (501) staff       (20)     1074 2024-03-21 11:41:36.000000 weavel-0.3.0/weavel.egg-info/SOURCES.txt
--rw-r--r--   0 jypark     (501) staff       (20)        1 2024-03-21 11:41:36.000000 weavel-0.3.0/weavel.egg-info/dependency_links.txt
--rw-r--r--   0 jypark     (501) staff       (20)      184 2024-03-21 11:41:36.000000 weavel-0.3.0/weavel.egg-info/requires.txt
--rw-r--r--   0 jypark     (501) staff       (20)       20 2024-03-21 11:41:36.000000 weavel-0.3.0/weavel.egg-info/top_level.txt
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.313794 weavel-0.4.0/
+-rw-r--r--   0 aschung    (501) staff       (20)        0 2024-01-18 05:08:39.000000 weavel-0.4.0/LICENSE
+-rw-r--r--   0 aschung    (501) staff       (20)      830 2024-04-04 12:08:44.313587 weavel-0.4.0/PKG-INFO
+-rw-r--r--   0 aschung    (501) staff       (20)       15 2024-01-18 05:08:39.000000 weavel-0.4.0/README.md
+-rw-r--r--   0 aschung    (501) staff       (20)       38 2024-04-04 12:08:44.313952 weavel-0.4.0/setup.cfg
+-rw-r--r--   0 aschung    (501) staff       (20)     1244 2024-04-04 12:08:16.000000 weavel-0.4.0/setup.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.310125 weavel-0.4.0/weavel/
+-rw-r--r--   0 aschung    (501) staff       (20)      107 2024-04-04 12:08:29.000000 weavel-0.4.0/weavel/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     6063 2024-01-18 05:08:39.000000 weavel-0.4.0/weavel/_api_client.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1692 2024-04-04 11:41:46.000000 weavel-0.4.0/weavel/_buffer_storage.py
+-rw-r--r--   0 aschung    (501) staff       (20)      211 2024-03-12 07:47:26.000000 weavel-0.4.0/weavel/_constants.py
+-rw-r--r--   0 aschung    (501) staff       (20)     9433 2024-04-04 11:46:25.000000 weavel-0.4.0/weavel/_worker.py
+-rw-r--r--   0 aschung    (501) staff       (20)     5404 2024-04-04 11:47:30.000000 weavel-0.4.0/weavel/client.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.312078 weavel-0.4.0/weavel/poe/
+-rw-r--r--   0 aschung    (501) staff       (20)       58 2024-03-12 07:47:26.000000 weavel-0.4.0/weavel/poe/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1749 2024-03-23 13:27:30.000000 weavel-0.4.0/weavel/poe/_poe_buffer_storage.py
+-rw-r--r--   0 aschung    (501) staff       (20)     4756 2024-03-23 13:27:30.000000 weavel-0.4.0/weavel/poe/_poe_worker.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1278 2024-03-23 13:27:30.000000 weavel-0.4.0/weavel/poe/poe_client.py
+-rw-r--r--   0 aschung    (501) staff       (20)     2431 2024-04-04 11:42:13.000000 weavel-0.4.0/weavel/types.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.312909 weavel-0.4.0/weavel/utils/
+-rw-r--r--   0 aschung    (501) staff       (20)       43 2024-01-18 05:08:39.000000 weavel-0.4.0/weavel/utils/__init__.py
+-rw-r--r--   0 aschung    (501) staff       (20)     1134 2024-01-18 05:08:39.000000 weavel-0.4.0/weavel/utils/crypto.py
+-rw-r--r--   0 aschung    (501) staff       (20)      679 2024-01-18 05:08:39.000000 weavel-0.4.0/weavel/utils/logger.py
+drwxr-xr-x   0 aschung    (501) staff       (20)        0 2024-04-04 12:08:44.313255 weavel-0.4.0/weavel.egg-info/
+-rw-r--r--   0 aschung    (501) staff       (20)      830 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/PKG-INFO
+-rw-r--r--   0 aschung    (501) staff       (20)      493 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/SOURCES.txt
+-rw-r--r--   0 aschung    (501) staff       (20)        1 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/dependency_links.txt
+-rw-r--r--   0 aschung    (501) staff       (20)      184 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/requires.txt
+-rw-r--r--   0 aschung    (501) staff       (20)        7 2024-04-04 12:08:44.000000 weavel-0.4.0/weavel.egg-info/top_level.txt
```

### Comparing `weavel-0.3.0/setup.py` & `weavel-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Weavel, natural language analysis Dashboard for LLM Agent
 """
+
 from setuptools import setup, find_namespace_packages
 
 # Read README.md for the long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="weavel",
-    version="0.3.0",
+    version="0.4.0",
     packages=find_namespace_packages(),
-    entry_points={
-    },
+    entry_points={},
     description="Weavel, natural language analysis Dashboard for LLM Agent",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="weavel",
     url="https://github.com/weavel-ai/weavel-python",
     install_requires=[
         "httpx[http2]",
```

### Comparing `weavel-0.3.0/weavel/_api_client.py` & `weavel-0.4.0/weavel/_api_client.py`

 * *Files identical despite different names*

### Comparing `weavel-0.3.0/weavel/_buffer_storage.py` & `weavel-0.4.0/weavel/_buffer_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 from threading import Condition, Lock
 from typing import Dict, List, Union
 
 from weavel.types import (
     OpenTraceBody,
-    CaptureActionEventBody,
+    CaptureTrackEventBody,
     CaptureTraceDataBody,
 )
 
 
 class BufferStorage:
     def __init__(self, max_buffer_size: int):
         self.max_buffer_size = max_buffer_size
-        self.buffer: List[Union[OpenTraceBody, CaptureActionEventBody, CaptureTraceDataBody]] = []
+        self.buffer: List[
+            Union[OpenTraceBody, CaptureTrackEventBody, CaptureTraceDataBody]
+        ] = []
         self.buffer_lock = Lock()
         self.not_full_cv = Condition(self.buffer_lock)
         self.not_empty_cv = Condition(self.buffer_lock)
 
     @property
     def buffer_size(self) -> int:
         return len(self.buffer)
@@ -27,21 +29,25 @@
             while self.buffer_size >= self.max_buffer_size:
                 self.not_empty_cv.notify()  # immediately wake up possibly sleeping consumer
                 self.not_full_cv.wait()
             self.buffer.append(event)
             if self.buffer_size >= self.max_buffer_size:
                 self.not_empty_cv.notify()
 
-    def pull(self, batch_size: int) -> List[Union[OpenTraceBody, CaptureActionEventBody, CaptureTraceDataBody]]:
+    def pull(
+        self, batch_size: int
+    ) -> List[Union[OpenTraceBody, CaptureTrackEventBody, CaptureTraceDataBody]]:
         while not self.buffer_size:
             self.not_empty_cv.wait()
         pull_size = min(batch_size, self.buffer_size)
         out = self.buffer[:pull_size]
         self.buffer = self.buffer[pull_size:]
         self.not_full_cv.notify()
         return out
 
-    def pull_all(self) -> List[Union[OpenTraceBody, CaptureActionEventBody, CaptureTraceDataBody]]:
+    def pull_all(
+        self,
+    ) -> List[Union[OpenTraceBody, CaptureTrackEventBody, CaptureTraceDataBody]]:
         out = self.buffer[:]
         self.buffer = []
         self.not_full_cv.notify()
         return out
```

### Comparing `weavel-0.3.0/weavel/_worker.py` & `weavel-0.4.0/weavel/_worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,94 +5,110 @@
 from datetime import datetime
 from typing import Dict, List, Optional, Union
 from threading import Thread
 from concurrent.futures import Future, ThreadPoolExecutor
 
 from weavel.types import (
     TraceDataRole,
-    BackgroundTaskType,
     OpenTraceBody,
     CaptureTraceDataBody,
-    CaptureActionEventBody,
+    CaptureTrackEventBody,
 )
 from weavel._constants import BACKEND_SERVER_URL
 from weavel._buffer_storage import BufferStorage
 from weavel._api_client import APIClient
 from weavel.utils import logger
 
+
 class Worker:
     _instance = None
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = super(Worker, cls).__new__(cls)
         return cls._instance
-    
+
     def __init__(
         self,
         api_key: str,
     ) -> None:
-        if not hasattr(self, 'is_initialized'):
+        if not hasattr(self, "is_initialized"):
             self.api_key = api_key
             self.endpoint = BACKEND_SERVER_URL
-            
+
             self.max_retry = 3
             self.flush_interval = 60
             self.flush_batch_size = 20
-            
+
             self.api_client = APIClient()
-            
+
             self.api_pool = ThreadPoolExecutor(max_workers=1)
             self.buffer_storage = BufferStorage(max_buffer_size=1000)
             self._running = True
             self._thread = Thread(target=self.consume_buffer, daemon=True)
             self._thread.start()
             self.is_initialized = True
-        
-    def _open_trace(self, trace_id: str, user_id: str, timestamp: Optional[datetime] = None, metadata: Optional[Dict[str, str]] = None) -> str:
+
+    def open_trace(
+        self,
+        trace_id: str,
+        user_id: str,
+        timestamp: Optional[datetime] = None,
+        metadata: Optional[Dict[str, str]] = None,
+    ) -> str:
         """Start the new trace for user_id.
-        
+
         Returns:
             The trace id.
         """
         # add task to buffer
         request = OpenTraceBody(
             user_id=user_id,
             trace_id=trace_id,
             timestamp=str(timestamp or datetime.now().isoformat()),
             metadata=metadata,
         )
 
         self.buffer_storage.push(request)
-        
+
         return trace_id
-    
-    def _track_users(self, user_id: str, name: str, properties: Dict) -> None:
-        """Save the user event"""
-        request = CaptureActionEventBody(
+
+    def log_track_event(self, user_id: str, name: str, properties: Dict) -> None:
+        """
+        Logs a track event for a user.
+
+        Args:
+            user_id (str): The ID of the user.
+            name (str): The name of the track event.
+            properties (Dict): Additional properties associated with the track event.
+
+        Returns:
+            None
+        """
+        request = CaptureTrackEventBody(
             user_id=user_id,
-            action_event_name=name,
+            track_event_name=name,
             properties=properties,
             timestamp=str(datetime.now().isoformat()),
         )
         self.buffer_storage.push(request)
-        
+
         return
-        
-    def user_message(
+
+    def log_user_message(
         self,
         user_id: str,
         trace_id: str,
         content: str,
         unit_name: Optional[str] = None,
         timestamp: Optional[datetime] = None,
-        metadata: Optional[Dict[str, str]] = None, 
+        metadata: Optional[Dict[str, str]] = None,
     ):
         """Log the "user_message" type data to the trace.
-        
+
         Args:
             trace_id: The trace identifier.
             content: The data content.
             unit_name: The unit name.
             timestamp: The timestamp.
             metadata: The metadata.
         """
@@ -103,26 +119,26 @@
             content=content,
             unit_name=unit_name,
             metadata=metadata,
             timestamp=str(timestamp or datetime.now().isoformat()),
         )
         self.buffer_storage.push(request)
         return
-    
-    def assistant_message(
+
+    def log_assistant_message(
         self,
         user_id: str,
         trace_id: str,
         content: str,
         unit_name: Optional[str] = None,
         timestamp: Optional[datetime] = None,
         metadata: Optional[Dict[str, str]] = None,
     ):
         """Log the "llm_background_message" type data to the trace.
-        
+
         Args:
             trace_id: The trace identifier.
             content: The data content.
             unit_name: The unit name.
             timestamp: The timestamp.
             metadata: The metadata.
         """
@@ -133,77 +149,65 @@
             content=content,
             unit_name=unit_name,
             metadata=metadata,
             timestamp=str(timestamp or datetime.now().isoformat()),
         )
         self.buffer_storage.push(request)
         return
-    
-    def system_message(
+
+    def log_inner_step(
         self,
         user_id: str,
         trace_id: str,
         content: str,
         unit_name: Optional[str] = None,
         timestamp: Optional[datetime] = None,
         metadata: Optional[Dict[str, str]] = None,
     ):
-        """Log the "system_message" type data to the trace.
-        
+        """Log the "inner_step" type data to the trace.
+
         Args:
             trace_id: The trace identifier.
             content: The data content.
             unit_name: The unit name.
             timestamp: The timestamp.
             metadata: The metadata.
         """
         request = CaptureTraceDataBody(
             user_id=user_id,
             trace_id=trace_id,
-            role=TraceDataRole.system,
+            role=TraceDataRole.inner_step,
             content=content,
             unit_name=unit_name,
             metadata=metadata,
             timestamp=str(timestamp or datetime.now().isoformat()),
         )
-
         self.buffer_storage.push(request)
         return
-    
-    def inner_step(
+
+    def send_requests(
         self,
-        user_id: str,
-        trace_id: str,
-        content: str,
-        unit_name: Optional[str] = None,
-        timestamp: Optional[datetime] = None,
-        metadata: Optional[Dict[str, str]] = None,
+        requests: List[
+            Union[OpenTraceBody, CaptureTrackEventBody, CaptureTraceDataBody]
+        ],
     ):
-        """Log the "inner_step" type data to the trace.
-        
+        """
+        Sends a batch of requests to the API endpoint.
+
         Args:
-            trace_id: The trace identifier.
-            content: The data content.
-            unit_name: The unit name.
-            timestamp: The timestamp.
-            metadata: The metadata.
+            requests (List[Union[OpenTraceBody, CaptureTrackEventBody, CaptureTraceDataBody]]):
+                A list of requests to be sent to the API endpoint.
+
+        Returns:
+            None: This method does not return any value.
+
+        Raises:
+            Exception: If an error occurs while sending the requests.
+
         """
-        request = CaptureTraceDataBody(
-            user_id=user_id,
-            trace_id=trace_id,
-            role=TraceDataRole.inner_step,
-            content=content,
-            unit_name=unit_name,
-            metadata=metadata,
-            timestamp=str(timestamp or datetime.now().isoformat()),
-        )
-        self.buffer_storage.push(request)
-        return
-            
-    def send_requests(self, requests: List[Union[OpenTraceBody, CaptureActionEventBody, CaptureTraceDataBody]]):
         # logger.info(requests)
         for attempt in range(self.max_retry):
             logger.info(requests)
             try:
                 response = self.api_client.execute(
                     self.api_key,
                     self.endpoint,
@@ -214,47 +218,78 @@
                 )
                 if response.status_code == 200:
                     return
             except Exception as e:
                 print(e)
                 time.sleep(2**attempt)
                 continue
-        
+
     def consume_buffer(self) -> None:
+        """
+        Continuously consumes the buffer and sends requests to the API.
+
+        This method runs in a loop until the `_running` flag is set to False. It checks the buffer size and waits for
+        the specified flush interval if the buffer is empty. If the buffer has data, it pulls a batch of data from
+        the buffer and sends requests to the API using the `send_requests` method. The completion of the API task is
+        handled by the `_handle_api_task_completion` method.
+
+        Raises:
+            Exception: If an error occurs while consuming the buffer.
+
+        """
         while self._running:
             try:
                 with self.buffer_storage.buffer_lock:
                     if self.buffer_storage.buffer_size == 0:
                         self.buffer_storage.not_empty_cv.wait(self.flush_interval)
                         continue
                     out = self.buffer_storage.pull(self.flush_batch_size)
                     future = self.api_pool.submit(self.send_requests, out)
                     future.add_done_callback(self._handle_api_task_completion)
                     self.buffer_storage.not_empty_cv.wait(self.flush_interval)
             except Exception as e:
                 print(e)
 
     def flush(self) -> None:
+        """
+        Flushes the buffer by sending the buffered requests.
+
+        This method pulls all the requests from the buffer and sends them in batches
+        of size `self.flush_batch_size` to the `send_requests` method.
+
+        Raises:
+            Exception: If an error occurs while flushing the buffer.
+        """
         try:
             with self.buffer_storage.buffer_lock:
                 if self.buffer_storage.buffer_size == 0:
                     return
                 out = self.buffer_storage.pull_all()
                 # for request chunks size of self.flush_batch_size
                 for i in range(0, len(out), self.flush_batch_size):
-                    request = out[i:i+self.flush_batch_size]
+                    request = out[i : i + self.flush_batch_size]
                     self.send_requests(request)
         except Exception as e:
             print(e)
-            
+
     def stop(self) -> None:
+        """
+        Stops the worker thread and flushes any remaining data in the buffer.
+
+        This method sets the `_running` flag to False, notifies the buffer storage
+        that it is not empty, joins the worker thread, and then calls the `flush`
+        method to ensure any remaining data in the buffer is processed.
+
+        Returns:
+            None
+        """
         self._running = False
         with self.buffer_storage.buffer_lock:
             self.buffer_storage.not_empty_cv.notify()
         self._thread.join()
         self.flush()
-                                     
+
     def _handle_api_task_completion(self, future: Future) -> None:
         try:
             future.result()
         except Exception as e:
-            print(e)
+            print(e)
```

### Comparing `weavel-0.3.0/weavel/poe/_poe_buffer_storage.py` & `weavel-0.4.0/weavel/poe/_poe_buffer_storage.py`

 * *Files identical despite different names*

### Comparing `weavel-0.3.0/weavel/poe/_poe_worker.py` & `weavel-0.4.0/weavel/poe/_poe_worker.py`

 * *Files identical despite different names*

### Comparing `weavel-0.3.0/weavel/poe/poe_client.py` & `weavel-0.4.0/weavel/poe/poe_client.py`

 * *Files identical despite different names*

### Comparing `weavel-0.3.0/weavel/types.py` & `weavel-0.4.0/weavel/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,85 @@
 from pydantic import BaseModel, validator
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, Literal
 from enum import Enum
 from uuid import UUID
 from datetime import datetime, date
 
+
 class WeavelObject(BaseModel):
     """Weavel Object. Extended Pydantic BaseModel with support for UUID and datetime."""
+
     def __init__(self, **data: Any):
         for key, value in data.items():
-            if key in self.__annotations__ and (self.__annotations__[key] == str or self.__annotations__[key] == Optional[str]):
+            if key in self.__annotations__ and (
+                self.__annotations__[key] == str
+                or self.__annotations__[key] == Optional[str]
+            ):
                 if (
                     isinstance(value, UUID)
                     or isinstance(value, datetime)
                     or isinstance(value, date)
                 ):
                     try:
                         data[key] = str(value)
                     except:
                         data[key] = value
         super().__init__(**data)
-        
-        
+
+
 class TraceDataRole(str, Enum):
     system = "system"
     user = "user"
     assisatant = "assistant"
     inner_step = "inner_step"
     # retrieved_content = "retrieved_content"
 
+
 class BackgroundTaskType(str, Enum):
     open_trace = "open_trace"
     capture_trace_data = "capture_trace_data"
-    capture_action_event = "capture_action_event"
+    capture_track_event = "capture_track_event"
     create_semantic_event = "create_semantic_event"
     extract_keywords = "extract_keywords"
-    
+
+
 class OpenTraceBody(WeavelObject):
     """Start Trace body."""
+
     type: Literal["open_trace"] = "open_trace"
     user_id: str
     trace_id: str
     timestamp: Optional[str] = None
     metadata: Optional[Dict[str, str]] = None
 
-class CaptureActionEventBody(WeavelObject):
-    """Capture action_event body."""
 
-    type: Literal["capture_action_event"] = "capture_action_event"
+class CaptureTrackEventBody(WeavelObject):
+    """Capture track_event body."""
+
+    type: Literal["capture_track_event"] = "capture_track_event"
     user_id: str
-    action_event_name: str
+    track_event_name: str
     properties: Dict[str, Any]
     timestamp: Optional[str] = None
-    
+
+
 class CaptureTraceDataBody(WeavelObject):
     """Capture Trace Data body."""
 
     type: Literal["capture_trace_data"] = "capture_trace_data"
     user_id: str
     trace_id: str
     role: str
     content: str
     unit_name: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
     timestamp: Optional[str] = None
-    
+
+
 # class SaveMetadataTraceBody(WeavelObject):
 #     """Save metadata body."""
 #     trace_id: str
 #     metadata: Dict[str, str]
 
+
 class BatchRequest(WeavelObject):
-    batch: List[
-        Union[
-            OpenTraceBody,
-            CaptureActionEventBody,
-            CaptureTraceDataBody
-        ]
-    ]
+    batch: List[Union[OpenTraceBody, CaptureTrackEventBody, CaptureTraceDataBody]]
```

### Comparing `weavel-0.3.0/weavel/utils/crypto.py` & `weavel-0.4.0/weavel/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `weavel-0.3.0/weavel/utils/logger.py` & `weavel-0.4.0/weavel/utils/logger.py`

 * *Files identical despite different names*

