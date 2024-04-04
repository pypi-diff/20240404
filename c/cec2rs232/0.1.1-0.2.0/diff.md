# Comparing `tmp/cec2rs232-0.1.1.tar.gz` & `tmp/cec2rs232-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cec2rs232-0.1.1.tar", last modified: Mon Jan  2 04:55:21 2023, max compression
+gzip compressed data, was "cec2rs232-0.2.0.tar", last modified: Thu Apr  4 03:18:09 2024, max compression
```

## Comparing `cec2rs232-0.1.1.tar` & `cec2rs232-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 04:55:21.210071 cec2rs232-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-01-02 04:55:21.210071 cec2rs232-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 04:55:21.210071 cec2rs232-0.1.1/cec2rs232/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/cec2rs232/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 04:55:21.210071 cec2rs232-0.1.1/cec2rs232/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/cec2rs232/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/cec2rs232/driver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/cec2rs232/driver/base_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/cec2rs232/driver/base_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/cec2rs232/driver/cambridge_cxa61.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/cec2rs232/driver/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/cec2rs232/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-02 04:55:21.210071 cec2rs232-0.1.1/cec2rs232.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-01-02 04:55:21.000000 cec2rs232-0.1.1/cec2rs232.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-01-02 04:55:21.000000 cec2rs232-0.1.1/cec2rs232.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-02 04:55:21.000000 cec2rs232-0.1.1/cec2rs232.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-01-02 04:55:21.000000 cec2rs232-0.1.1/cec2rs232.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-02 04:55:21.000000 cec2rs232-0.1.1/cec2rs232.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-02 04:55:21.000000 cec2rs232-0.1.1/cec2rs232.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-02 04:55:21.210071 cec2rs232-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-01-02 04:55:11.000000 cec2rs232-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:18:09.364567 cec2rs232-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-04 03:18:09.364567 cec2rs232-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:18:09.360567 cec2rs232-0.2.0/cec2rs232/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/cec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:18:09.364567 cec2rs232-0.2.0/cec2rs232/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/driver/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/driver/base_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/driver/base_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/driver/cambridge_cxa61.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/driver/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/cec2rs232/mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:18:09.364567 cec2rs232-0.2.0/cec2rs232.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-04 03:18:09.000000 cec2rs232-0.2.0/cec2rs232.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-04 03:18:09.000000 cec2rs232-0.2.0/cec2rs232.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:18:09.000000 cec2rs232-0.2.0/cec2rs232.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 03:18:09.000000 cec2rs232-0.2.0/cec2rs232.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 03:18:09.000000 cec2rs232-0.2.0/cec2rs232.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 03:18:09.000000 cec2rs232-0.2.0/cec2rs232.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:18:09.364567 cec2rs232-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-04 03:18:05.000000 cec2rs232-0.2.0/setup.py
```

### Comparing `cec2rs232-0.1.1/LICENSE.md` & `cec2rs232-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cec2rs232-0.1.1/PKG-INFO` & `cec2rs232-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cec2rs232
-Version: 0.1.1
-Summary: Enables a Raspberry Pi to act as a bridge between CEC and RS-232 or IR
-Home-page: https://github.com/tmick0/cec2rs232
-Author: travis mick
-Author-email: root@lo.calho.st
-License: MIT
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # cec2rs232
 
 ## Overview
 
 This project aims to turn a Raspberry Pi into a bridge between the HDMI CEC standard
 and arbitrary control protocols for audio systems.
 
@@ -75,14 +63,38 @@
 | `ir_gpio_pin` | integer            | GPIO pin number driving the IR transmitter                          |
 | `tv_source`   | string (optional)  | Source to activate when TV turns on, e.g. "D2". Omit to not change. |
 
 ### Others
 
 Please feel free to make a pull request to add support for other devices.
 
+## MQTT
+
+The controls for the connected audio device can also be exposed over MQTT, with the intention
+of being controlled from Home Assistant.
+
+To enable this functionality, add an `"mqtt"` section to the configuration file:
+
+```
+"mqtt": {
+    "server": "homeassistant.local",
+    "port": 1883,
+    "username": "mqtt",
+    "password": "password",
+    "name": "cxa61",
+    "topic": "homeassistant/button/cxa61",
+    "discovery": true
+}
+```
+
+Each supported input (e.g., power_on, power_off, volume_up, volume_down, etc...) is exposed as a separate button entity, and
+when pressed will execute that command as if it were pressed on a remote control.
+
+If not using Home Assistant, disable `discovery`. Then, you can manually send commands to the chosen topic.
+
 ## Dependencies
 
 Bindings for libCEC are required: `sudo apt install python3-cec`.
 
 If using a virtual environment, specify `--system-site-packages` so the native libcec can be used.
 
 Pigpiod is required: `sudo apt install pigpiod && sudo systemctl enable pigpiod && sudo systemctl start pigpiod`.
```

### Comparing `cec2rs232-0.1.1/README.md` & `cec2rs232-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: cec2rs232
+Version: 0.2.0
+Summary: Enables a Raspberry Pi to act as a bridge between CEC and RS-232 or IR
+Home-page: https://github.com/tmick0/cec2rs232
+Author: travis mick
+Author-email: root@lo.calho.st
+License: MIT
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: pycec
+Requires-Dist: pyserial
+Requires-Dist: piir
+Requires-Dist: aiomqtt
+
 # cec2rs232
 
 ## Overview
 
 This project aims to turn a Raspberry Pi into a bridge between the HDMI CEC standard
 and arbitrary control protocols for audio systems.
 
@@ -63,14 +79,38 @@
 | `ir_gpio_pin` | integer            | GPIO pin number driving the IR transmitter                          |
 | `tv_source`   | string (optional)  | Source to activate when TV turns on, e.g. "D2". Omit to not change. |
 
 ### Others
 
 Please feel free to make a pull request to add support for other devices.
 
+## MQTT
+
+The controls for the connected audio device can also be exposed over MQTT, with the intention
+of being controlled from Home Assistant.
+
+To enable this functionality, add an `"mqtt"` section to the configuration file:
+
+```
+"mqtt": {
+    "server": "homeassistant.local",
+    "port": 1883,
+    "username": "mqtt",
+    "password": "password",
+    "name": "cxa61",
+    "topic": "homeassistant/button/cxa61",
+    "discovery": true
+}
+```
+
+Each supported input (e.g., power_on, power_off, volume_up, volume_down, etc...) is exposed as a separate button entity, and
+when pressed will execute that command as if it were pressed on a remote control.
+
+If not using Home Assistant, disable `discovery`. Then, you can manually send commands to the chosen topic.
+
 ## Dependencies
 
 Bindings for libCEC are required: `sudo apt install python3-cec`.
 
 If using a virtual environment, specify `--system-site-packages` so the native libcec can be used.
 
 Pigpiod is required: `sudo apt install pigpiod && sudo systemctl enable pigpiod && sudo systemctl start pigpiod`.
```

### Comparing `cec2rs232-0.1.1/cec2rs232/driver/base.py` & `cec2rs232-0.2.0/cec2rs232/driver/base.py`

 * *Files identical despite different names*

### Comparing `cec2rs232-0.1.1/cec2rs232/driver/cambridge_cxa61.py` & `cec2rs232-0.2.0/cec2rs232/driver/cambridge_cxa61.py`

 * *Files identical despite different names*

### Comparing `cec2rs232-0.1.1/cec2rs232/main.py` & `cec2rs232-0.2.0/cec2rs232/cec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-import argparse
 import logging
-import asyncio
-import json
 from pycec import cec, const, commands
-from .driver.cambridge_cxa61 import cambridge_cxa61
-from .driver.registry import driver_registry
 
-logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 SYSTEM_AUDIO_MODE_REQUEST = 0x70
 SET_SYSTEM_AUDIO_MODE = 0x72
 
 CMD_AUDIO_MODE_STATUS_REQ, CMD_AUDIO_MODE_STATUS_REP = const.CMD_AUDIO_MODE_STATUS
 
-class cec2rs232:
 
-    def __init__(self, driver):
-        self._loop = asyncio.new_event_loop()
+class cec_interface (object):
+
+    def __init__(self, driver, loop):
         self._driver = driver
         self._adapter = cec.CecAdapter(driver.get_name(), device_type=const.TYPE_AUDIO, activate_source=False)
-        self._adapter.set_event_loop(self._loop)
+        self._adapter.set_event_loop(loop)
         self._adapter.set_command_callback(self._handle_command)
         self._address = None
         self._power = False
-        
+    
+    def init(self):
+        return self._adapter.init(self._init_callback)
+
     def _init_callback(self, *args, **kwargs):
         self._address = self._adapter.get_logical_address()
         logger.info("ready")
 
     def _handle_keypress(self, att):
         if att == const.KEY_VOLUME_DOWN:
             self._driver.volume_down()
@@ -73,26 +70,7 @@
                         logger.info('cmd_standby')
                         self._driver.power_off()
                     else:
                         logger.debug(f"unhandled command: {raw} - 0x{cmd.cmd:02x} att: {cmd.att}")
         except Exception as e:
             logger.error("error in handle_command:")
             logger.exception(e)
-    
-    def run(self):
-        task = self._adapter.init(self._init_callback)
-        try:
-            self._loop.run_forever()
-        except Exception as e:
-            logger.exception(e)
-        self._loop.close()
-
-def main():
-    parser = argparse.ArgumentParser()
-    parser.add_argument('config_file', default='/etc/cec2rs232/cec2rs232.json')
-    args = parser.parse_args()
-
-    with open(args.config_file, 'r') as fh:
-        config = json.load(fh)
-    
-    driver = driver_registry[config["device"]](**config["parameters"])
-    cec2rs232(driver).run()
```

### Comparing `cec2rs232-0.1.1/cec2rs232.egg-info/PKG-INFO` & `cec2rs232-0.2.0/cec2rs232.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: cec2rs232
-Version: 0.1.1
+Version: 0.2.0
 Summary: Enables a Raspberry Pi to act as a bridge between CEC and RS-232 or IR
 Home-page: https://github.com/tmick0/cec2rs232
 Author: travis mick
 Author-email: root@lo.calho.st
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: pycec
+Requires-Dist: pyserial
+Requires-Dist: piir
+Requires-Dist: aiomqtt
 
 # cec2rs232
 
 ## Overview
 
 This project aims to turn a Raspberry Pi into a bridge between the HDMI CEC standard
 and arbitrary control protocols for audio systems.
@@ -75,14 +79,38 @@
 | `ir_gpio_pin` | integer            | GPIO pin number driving the IR transmitter                          |
 | `tv_source`   | string (optional)  | Source to activate when TV turns on, e.g. "D2". Omit to not change. |
 
 ### Others
 
 Please feel free to make a pull request to add support for other devices.
 
+## MQTT
+
+The controls for the connected audio device can also be exposed over MQTT, with the intention
+of being controlled from Home Assistant.
+
+To enable this functionality, add an `"mqtt"` section to the configuration file:
+
+```
+"mqtt": {
+    "server": "homeassistant.local",
+    "port": 1883,
+    "username": "mqtt",
+    "password": "password",
+    "name": "cxa61",
+    "topic": "homeassistant/button/cxa61",
+    "discovery": true
+}
+```
+
+Each supported input (e.g., power_on, power_off, volume_up, volume_down, etc...) is exposed as a separate button entity, and
+when pressed will execute that command as if it were pressed on a remote control.
+
+If not using Home Assistant, disable `discovery`. Then, you can manually send commands to the chosen topic.
+
 ## Dependencies
 
 Bindings for libCEC are required: `sudo apt install python3-cec`.
 
 If using a virtual environment, specify `--system-site-packages` so the native libcec can be used.
 
 Pigpiod is required: `sudo apt install pigpiod && sudo systemctl enable pigpiod && sudo systemctl start pigpiod`.
```

### Comparing `cec2rs232-0.1.1/setup.py` & `cec2rs232-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name="cec2rs232",
-    version="0.1.1",
+    version="0.2.0",
     author="travis mick",
     author_email="root@lo.calho.st",
     description="Enables a Raspberry Pi to act as a bridge between CEC and RS-232 or IR",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/tmick0/cec2rs232",
     python_requires='>=3.9',
-    install_requires=["pycec", "pyserial", "piir"],
+    install_requires=["pycec", "pyserial", "piir", "aiomqtt"],
     packages=find_packages(),
     entry_points={
         'console_scripts': ['cec2rs232=cec2rs232.main:main'],
     }
 )
```

