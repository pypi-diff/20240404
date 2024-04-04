# Comparing `tmp/robothub-2.5.5.tar.gz` & `tmp/robothub-2.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub-2.5.5.tar", last modified: Wed Mar 27 22:09:18 2024, max compression
+gzip compressed data, was "robothub-2.5.6.tar", last modified: Thu Apr  4 14:51:06 2024, max compression
```

## Comparing `robothub-2.5.5.tar` & `robothub-2.5.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:09:18.342525 robothub-2.5.5/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-03-27 22:08:59.000000 robothub-2.5.5/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-03-27 22:08:59.000000 robothub-2.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-27 22:09:18.338525 robothub-2.5.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-03-27 22:08:59.000000 robothub-2.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 22:09:18.342525 robothub-2.5.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-03-27 22:08:59.000000 robothub-2.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:09:18.334525 robothub-2.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:09:18.334525 robothub-2.5.5/src/robothub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/application.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/frame_buffer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/live_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/live_view_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23375 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/replay_camera.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:09:18.338525 robothub-2.5.5/src/robothub/robothub_core_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/_event_typechecks.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/_stop_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9335 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/robothub_core_wrapper/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-03-27 22:08:59.000000 robothub-2.5.5/src/robothub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:09:18.338525 robothub-2.5.5/src/robothub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-27 22:09:18.000000 robothub-2.5.5/src/robothub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-27 22:09:18.000000 robothub-2.5.5/src/robothub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 22:09:18.000000 robothub-2.5.5/src/robothub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 22:09:18.000000 robothub-2.5.5/src/robothub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:09:18.338525 robothub-2.5.5/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:08:59.000000 robothub-2.5.5/tests/test_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:08:59.000000 robothub-2.5.5/tests/test_hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:08:59.000000 robothub-2.5.5/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.213237 robothub-2.5.6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-04 14:50:43.000000 robothub-2.5.6/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-04 14:50:43.000000 robothub-2.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-04 14:51:06.213237 robothub-2.5.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-04-04 14:50:43.000000 robothub-2.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:51:06.213237 robothub-2.5.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-04-04 14:50:43.000000 robothub-2.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.205237 robothub-2.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.209237 robothub-2.5.6/src/robothub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12843 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/application.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/frame_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/live_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/live_view_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/replay_camera.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.209237 robothub-2.5.6/src/robothub/robothub_core_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_event_typechecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_stop_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9335 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/robothub_core_wrapper/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-04 14:50:43.000000 robothub-2.5.6/src/robothub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.213237 robothub-2.5.6/src/robothub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-04 14:51:06.000000 robothub-2.5.6/src/robothub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-04 14:51:06.000000 robothub-2.5.6/src/robothub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:51:06.000000 robothub-2.5.6/src/robothub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 14:51:06.000000 robothub-2.5.6/src/robothub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:51:06.213237 robothub-2.5.6/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:43.000000 robothub-2.5.6/tests/test_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:43.000000 robothub-2.5.6/tests/test_hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:50:43.000000 robothub-2.5.6/tests/test_manager.py
```

### Comparing `robothub-2.5.5/LICENSE` & `robothub-2.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/PKG-INFO` & `robothub-2.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.5
+Version: 2.5.6
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub-2.5.5/README.md` & `robothub-2.5.6/README.md`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/setup.py` & `robothub-2.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub',
-    version='2.5.5',
+    version='2.5.6',
     description='RobotHub integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub camera robot hub connect agent depthai sdk',
     author='Luxonis',
```

### Comparing `robothub-2.5.5/src/robothub/__init__.py` & `robothub-2.5.6/src/robothub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
 # Import symbols from robothub_core and make them available under the robothub namespace
 try:
     import robothub_core as robothub
 except ImportError:
     import robothub.robothub_core_wrapper as robothub
 
-__version__ = '2.5.5'
+__version__ = '2.5.6'
 
 # Setup logging for the module
 # setup_logger(__name__)
```

### Comparing `robothub-2.5.5/src/robothub/application.py` & `robothub-2.5.6/src/robothub/application.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/events.py` & `robothub-2.5.6/src/robothub/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/frame_buffer.py` & `robothub-2.5.6/src/robothub/frame_buffer.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/live_view.py` & `robothub-2.5.6/src/robothub/live_view.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/live_view_utils.py` & `robothub-2.5.6/src/robothub/live_view_utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/replay_camera.py` & `robothub-2.5.6/src/robothub/replay_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,17 @@
         self._preview_height: int = 720
         self._color_order: dai.ColorCameraProperties.ColorOrder = dai.ColorCameraProperties.ColorOrder.BGR
         self._interleaved = False
         self._run_in_loop = run_in_loop
         self._pipeline: dai.Pipeline = pipeline
         self._camera_socket: dai.CameraBoardSocket | None = None
 
+        self._stop_event = threading.Event()
+        self._thread: Optional[threading.Thread] = None
+
         self._init_cap(src)
         if self._cap is None:
             logging.error("Couldn't init the cap")
             return
 
         # NOTE(miha): Used for saving references to nodes if we want to set max
         # data size later (i.e. calling setPreviewSize also alter max data size).
@@ -251,15 +254,15 @@
                 if not next_frame_exists and self._run_in_loop:
                     self._reset_cap()
                     continue
                 break
 
             return frame
 
-        while rh.app_is_running:
+        while rh.app_is_running and self.replay_is_running:
             start = time.monotonic()
 
             # NOTE(miha): Returned frame is in BGR format
             frame = get_next_frame()
             if frame is None:
                 break
 
@@ -318,16 +321,25 @@
             time_to_sleep = max((1. / self._fps) - process_time, 0)
             logging.debug(f"process_time: {process_time}, time_to_sleep: {time_to_sleep}")
             time.sleep(time_to_sleep)
 
         self._cap.release()
 
     def start_polling(self, device: dai.Device):
-        thread = threading.Thread(target=self._send_video_frames, args=(device,))
-        thread.start()
+        self._thread = threading.Thread(target=self._send_video_frames, args=(device,))
+        self._thread.start()
+
+    def stop_polling(self):
+        if self._thread and self._thread.is_alive():
+            self._stop_event.set()
+            self._thread.join()
+
+    @property
+    def replay_is_running(self):
+        return not self._stop_event.is_set()
 
     # NOTE(miha): Below are methods for ColorCamera class:
 
     def getBoardSocket(self) -> dai.CameraBoardSocket:
         return self._camera_socket
 
     def getCamId(self) -> int:
```

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/__init__.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/_event_typechecks.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/_event_typechecks.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/app.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/app.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/client.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/communicator.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/communicator.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/device.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/device.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/events.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/globals.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/globals.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/robothub_core_wrapper/streams.py` & `robothub-2.5.6/src/robothub/robothub_core_wrapper/streams.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub/utils.py` & `robothub-2.5.6/src/robothub/utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.5/src/robothub.egg-info/PKG-INFO` & `robothub-2.5.6/src/robothub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.5
+Version: 2.5.6
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub-2.5.5/src/robothub.egg-info/SOURCES.txt` & `robothub-2.5.6/src/robothub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

