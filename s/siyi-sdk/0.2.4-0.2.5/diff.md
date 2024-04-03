# Comparing `tmp/siyi_sdk-0.2.4.tar.gz` & `tmp/siyi_sdk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siyi_sdk-0.2.4.tar", max compression
+gzip compressed data, was "siyi_sdk-0.2.5.tar", max compression
```

## Comparing `siyi_sdk-0.2.4.tar` & `siyi_sdk-0.2.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       51 2024-03-25 23:21:52.454164 siyi_sdk-0.2.4/README.md
--rw-r--r--   0        0        0      335 2024-04-03 23:42:01.387343 siyi_sdk-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       33 2024-03-25 23:25:34.330901 siyi_sdk-0.2.4/siyi_sdk/.git
--rw-r--r--   0        0        0     3078 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/.gitignore
--rw-r--r--   0        0        0     1082 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/LICENSE
--rw-r--r--   0        0        0     4034 2024-03-25 23:25:44.550383 siyi_sdk-0.2.4/siyi_sdk/README.md
--rw-r--r--   0        0        0       58 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/__init__.py
--rw-r--r--   0        0        0     4353 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/crc16_python.py
--rw-r--r--   0        0        0  8385675 2024-03-25 23:25:44.562382 siyi_sdk-0.2.4/siyi_sdk/gui/demo.mp4
--rw-r--r--   0        0        0    16665 2024-03-25 23:25:44.562382 siyi_sdk-0.2.4/siyi_sdk/gui/gui_tkinter.png
--rw-r--r--   0        0        0     3994 2024-03-28 21:15:20.435565 siyi_sdk-0.2.4/siyi_sdk/gui/tkgui.py
--rw-r--r--   0        0        0    12921 2024-04-03 23:41:01.858916 siyi_sdk-0.2.4/siyi_sdk/siyi_message.py
--rw-r--r--   0        0        0    30536 2024-04-03 23:41:25.317516 siyi_sdk-0.2.4/siyi_sdk/siyi_sdk.py
--rw-r--r--   0        0        0     9360 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/stream.py
--rw-r--r--   0        0        0        0 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/__init__.py
--rw-r--r--   0        0        0      878 2024-03-28 21:04:24.903711 siyi_sdk-0.2.4/siyi_sdk/tests/serial/test_center_gimbal.py
--rw-r--r--   0        0        0      787 2024-03-28 21:04:24.903711 siyi_sdk-0.2.4/siyi_sdk/tests/serial/test_get_fw_ver.py
--rw-r--r--   0        0        0      820 2024-03-28 21:04:24.903711 siyi_sdk-0.2.4/siyi_sdk/tests/serial/test_gimbal_position.py
--rw-r--r--   0        0        0      790 2024-03-28 21:04:24.903711 siyi_sdk-0.2.4/siyi_sdk/tests/serial/test_gimbal_rotation.py
--rw-r--r--   0        0        0      844 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_center_gimbal.py
--rw-r--r--   0        0        0      746 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_follow_mode.py
--rw-r--r--   0        0        0      737 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_fpv_mode.py
--rw-r--r--   0        0        0      924 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_from_rtsp_to_rtmp.py
--rw-r--r--   0        0        0      753 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_get_fw_ver.py
--rw-r--r--   0        0        0      881 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_get_gimbal_info.py
--rw-r--r--   0        0        0      734 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_get_hw_id.py
--rw-r--r--   0        0        0      774 2024-03-28 21:14:01.390679 siyi_sdk-0.2.4/siyi_sdk/tests/test_gimbal_position.py
--rw-r--r--   0        0        0      756 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_gimbal_rotation.py
--rw-r--r--   0        0        0      740 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_lock_mode.py
--rw-r--r--   0        0        0     1088 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_record_video.py
--rw-r--r--   0        0        0     1213 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_rtmp_stream.py
--rw-r--r--   0        0        0      582 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_rtsp.py
--rw-r--r--   0        0        0      918 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/test_zoom.py
--rw-r--r--   0        0        0      541 2024-03-25 23:25:34.334901 siyi_sdk-0.2.4/siyi_sdk/tests/udp_server.py
--rw-r--r--   0        0        0     1209 2024-03-28 21:04:24.903711 siyi_sdk-0.2.4/siyi_sdk/utils.py
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 siyi_sdk-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       51 2024-03-25 23:21:52.454164 siyi_sdk-0.2.5/README.md
+-rw-r--r--   0        0        0      335 2024-04-03 23:45:44.657436 siyi_sdk-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       33 2024-03-25 23:25:34.330901 siyi_sdk-0.2.5/siyi_sdk/.git
+-rw-r--r--   0        0        0     3078 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/.gitignore
+-rw-r--r--   0        0        0     1082 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/LICENSE
+-rw-r--r--   0        0        0     4034 2024-03-25 23:25:44.550383 siyi_sdk-0.2.5/siyi_sdk/README.md
+-rw-r--r--   0        0        0       58 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/__init__.py
+-rw-r--r--   0        0        0     4353 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/crc16_python.py
+-rw-r--r--   0        0        0  8385675 2024-03-25 23:25:44.562382 siyi_sdk-0.2.5/siyi_sdk/gui/demo.mp4
+-rw-r--r--   0        0        0    16665 2024-03-25 23:25:44.562382 siyi_sdk-0.2.5/siyi_sdk/gui/gui_tkinter.png
+-rw-r--r--   0        0        0     3994 2024-03-28 21:15:20.435565 siyi_sdk-0.2.5/siyi_sdk/gui/tkgui.py
+-rw-r--r--   0        0        0    12931 2024-04-03 23:45:36.129980 siyi_sdk-0.2.5/siyi_sdk/siyi_message.py
+-rw-r--r--   0        0        0    30479 2024-04-03 23:45:19.023067 siyi_sdk-0.2.5/siyi_sdk/siyi_sdk.py
+-rw-r--r--   0        0        0     9360 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/stream.py
+-rw-r--r--   0        0        0        0 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/__init__.py
+-rw-r--r--   0        0        0      878 2024-03-28 21:04:24.903711 siyi_sdk-0.2.5/siyi_sdk/tests/serial/test_center_gimbal.py
+-rw-r--r--   0        0        0      787 2024-03-28 21:04:24.903711 siyi_sdk-0.2.5/siyi_sdk/tests/serial/test_get_fw_ver.py
+-rw-r--r--   0        0        0      820 2024-03-28 21:04:24.903711 siyi_sdk-0.2.5/siyi_sdk/tests/serial/test_gimbal_position.py
+-rw-r--r--   0        0        0      790 2024-03-28 21:04:24.903711 siyi_sdk-0.2.5/siyi_sdk/tests/serial/test_gimbal_rotation.py
+-rw-r--r--   0        0        0      844 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_center_gimbal.py
+-rw-r--r--   0        0        0      746 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_follow_mode.py
+-rw-r--r--   0        0        0      737 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_fpv_mode.py
+-rw-r--r--   0        0        0      924 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_from_rtsp_to_rtmp.py
+-rw-r--r--   0        0        0      753 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_get_fw_ver.py
+-rw-r--r--   0        0        0      881 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_get_gimbal_info.py
+-rw-r--r--   0        0        0      734 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_get_hw_id.py
+-rw-r--r--   0        0        0      774 2024-03-28 21:14:01.390679 siyi_sdk-0.2.5/siyi_sdk/tests/test_gimbal_position.py
+-rw-r--r--   0        0        0      756 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_gimbal_rotation.py
+-rw-r--r--   0        0        0      740 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_lock_mode.py
+-rw-r--r--   0        0        0     1088 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_record_video.py
+-rw-r--r--   0        0        0     1213 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_rtmp_stream.py
+-rw-r--r--   0        0        0      582 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_rtsp.py
+-rw-r--r--   0        0        0      918 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/test_zoom.py
+-rw-r--r--   0        0        0      541 2024-03-25 23:25:34.334901 siyi_sdk-0.2.5/siyi_sdk/tests/udp_server.py
+-rw-r--r--   0        0        0     1209 2024-03-28 21:04:24.903711 siyi_sdk-0.2.5/siyi_sdk/utils.py
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 siyi_sdk-0.2.5/PKG-INFO
```

### Comparing `siyi_sdk-0.2.4/siyi_sdk/.gitignore` & `siyi_sdk-0.2.5/siyi_sdk/.gitignore`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/LICENSE` & `siyi_sdk-0.2.5/siyi_sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/README.md` & `siyi_sdk-0.2.5/siyi_sdk/README.md`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/crc16_python.py` & `siyi_sdk-0.2.5/siyi_sdk/crc16_python.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/gui/demo.mp4` & `siyi_sdk-0.2.5/siyi_sdk/gui/demo.mp4`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/gui/gui_tkinter.png` & `siyi_sdk-0.2.5/siyi_sdk/gui/gui_tkinter.png`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/gui/tkgui.py` & `siyi_sdk-0.2.5/siyi_sdk/gui/tkgui.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/siyi_message.py` & `siyi_sdk-0.2.5/siyi_sdk/siyi_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,16 +491,16 @@
             yaw=-160
 
         if pitch>45:
             pitch=45
         if pitch<-90:
             pitch=-90
 
-        data1=format_hex(10*yaw)
-        data2=format_hex(10*pitch)
+        data1=format_hex(int(10*yaw))
+        data2=format_hex(int(10*pitch))
         
         self._logger.debug("data1 %s", data1)
         self._logger.debug("data2 %s", data2)
         data=data1[2:4]+data1[0:2]+data2[2:4]+data2[0:2]
         self._logger.debug("data %s", data)
         cmd_id = COMMAND.SET_GIMBAL_ANGLE
         return self.encodeMsg(data, cmd_id)
```

### Comparing `siyi_sdk-0.2.4/siyi_sdk/siyi_sdk.py` & `siyi_sdk-0.2.5/siyi_sdk/siyi_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,25 +545,22 @@
 
     def requestGimbalPosition(self, yaw:float, pitch:float):
         """
         Sends request for to set gimbal angles 
 
         Params
         --
-        yaw [int] -160~0~160. away from zero -> fast, close to zero -> slow. Sign is for direction
-        pitch [int] -90~0~45
+        yaw [float] -160~0~160. away from zero -> fast, close to zero -> slow. Sign is for direction
+        pitch [float] -90~0~45
         
         Returns
         --
         [bool] True: success. False: fail
         """
-        
-        yaw = round(yaw, 1)
-        pitch = round(pitch, 1)
-        
+                
         msg = self._out_msg.gimbalPositionMsg(yaw, pitch)
         if not self.sendMsg(msg):
             return False
         return True
 
     def requestPhoto(self):
         """
```

### Comparing `siyi_sdk-0.2.4/siyi_sdk/stream.py` & `siyi_sdk-0.2.5/siyi_sdk/stream.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/serial/test_center_gimbal.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/serial/test_center_gimbal.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/serial/test_get_fw_ver.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/serial/test_get_fw_ver.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/serial/test_gimbal_position.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/serial/test_gimbal_position.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/serial/test_gimbal_rotation.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/serial/test_gimbal_rotation.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_center_gimbal.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_center_gimbal.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_follow_mode.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_follow_mode.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_fpv_mode.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_fpv_mode.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_from_rtsp_to_rtmp.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_from_rtsp_to_rtmp.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_get_fw_ver.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_get_fw_ver.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_get_gimbal_info.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_get_gimbal_info.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_get_hw_id.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_get_hw_id.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_gimbal_position.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_gimbal_position.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_gimbal_rotation.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_gimbal_rotation.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_lock_mode.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_lock_mode.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_record_video.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_record_video.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_rtmp_stream.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_rtmp_stream.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_rtsp.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_rtsp.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/test_zoom.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/tests/udp_server.py` & `siyi_sdk-0.2.5/siyi_sdk/tests/udp_server.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/siyi_sdk/utils.py` & `siyi_sdk-0.2.5/siyi_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.4/PKG-INFO` & `siyi_sdk-0.2.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siyi-sdk
-Version: 0.2.4
+Version: 0.2.5
 Summary: SIYI gimbal camera SDK
 Author: Soter Technology
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

