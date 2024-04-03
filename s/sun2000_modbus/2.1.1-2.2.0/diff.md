# Comparing `tmp/sun2000_modbus-2.1.1.tar.gz` & `tmp/sun2000_modbus-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sun2000_modbus-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sun2000_modbus-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sun2000_modbus-2.1.1.tar` & `sun2000_modbus-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      231 2024-03-19 22:44:30.917898 sun2000_modbus-2.1.1/.editorconfig
--rw-r--r--   0        0        0       21 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      570 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1136 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      444 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/.gitignore
--rw-r--r--   0        0        0      385 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/LEGAL
--rw-r--r--   0        0        0     1073 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/LICENSE
--rw-r--r--   0        0        0    36038 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/README.md
--rw-r--r--   0        0        0      689 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/pyproject.toml
--rw-r--r--   0        0        0       16 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/requirements.txt
--rw-r--r--   0        0        0       96 2024-03-19 22:44:31.133896 sun2000_modbus-2.1.1/sun2000_modbus/__init__.py
--rw-r--r--   0        0        0     1144 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/sun2000_modbus/datatypes.py
--rw-r--r--   0        0        0     3695 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/sun2000_modbus/inverter.py
--rw-r--r--   0        0        0     2783 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/sun2000_modbus/mappings.py
--rw-r--r--   0        0        0    31787 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/sun2000_modbus/registers.py
--rw-r--r--   0        0        0        0 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1512 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/tests/sun2000mock.py
--rw-r--r--   0        0        0    14153 2024-03-19 22:44:30.921898 sun2000_modbus-2.1.1/tests/test_sun2000_modbus.py
--rw-r--r--   0        0        0    36648 1970-01-01 00:00:00.000000 sun2000_modbus-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      231 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/.editorconfig
+-rw-r--r--   0        0        0       21 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      570 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1136 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      444 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/.gitignore
+-rw-r--r--   0        0        0      385 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/LEGAL
+-rw-r--r--   0        0        0     1073 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/LICENSE
+-rw-r--r--   0        0        0    36038 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/README.md
+-rw-r--r--   0        0        0      689 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       16 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/requirements.txt
+-rw-r--r--   0        0        0       96 2024-04-03 22:13:06.927630 sun2000_modbus-2.2.0/sun2000_modbus/__init__.py
+-rw-r--r--   0        0        0     1178 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/sun2000_modbus/datatypes.py
+-rw-r--r--   0        0        0     4078 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/sun2000_modbus/inverter.py
+-rw-r--r--   0        0        0     2783 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/sun2000_modbus/mappings.py
+-rw-r--r--   0        0        0    31787 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/sun2000_modbus/registers.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1512 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/tests/sun2000mock.py
+-rw-r--r--   0        0        0    14153 2024-04-03 22:13:06.711630 sun2000_modbus-2.2.0/tests/test_sun2000_modbus.py
+-rw-r--r--   0        0        0    36648 1970-01-01 00:00:00.000000 sun2000_modbus-2.2.0/PKG-INFO
```

### Comparing `sun2000_modbus-2.1.1/.github/workflows/build.yml` & `sun2000_modbus-2.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/.github/workflows/publish.yml` & `sun2000_modbus-2.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/LICENSE` & `sun2000_modbus-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/README.md` & `sun2000_modbus-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/pyproject.toml` & `sun2000_modbus-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/sun2000_modbus/inverter.py` & `sun2000_modbus-2.2.0/sun2000_modbus/inverter.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,73 +2,85 @@
 import time
 
 from pymodbus.client.sync import ModbusTcpClient
 from pymodbus.exceptions import ModbusIOException, ConnectionException
 
 from . import datatypes
 
-logging.basicConfig(level=logging.INFO)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+log_format = logging.Formatter('%(levelname)s:%(name)s:%(message)s')
+handler = logging.StreamHandler()
+handler.setFormatter(log_format)
+logger.addHandler(handler)
 
 
 class Sun2000:
     def __init__(self, host, port=502, timeout=5, wait=2, unit=0): # some models need unit=1
         self.wait = wait
         self.unit = unit
         self.inverter = ModbusTcpClient(host, port, timeout=timeout)
 
     def connect(self):
         if not self.isConnected():
             self.inverter.connect()
             time.sleep(self.wait)
             if self.isConnected():
-                logging.info('Successfully connected to inverter')
+                logger.info('Successfully connected to inverter')
                 return True
             else:
-                logging.error('Connection to inverter failed')
+                logger.error('Connection to inverter failed')
                 return False
 
     def disconnect(self):
         """Close the underlying tcp socket"""
         # Some Sun2000 models with the SDongle WLAN-FE require the TCP connection to be closed
         # as soon as possible. Leaving the TCP connection open for an extended time may cause 
         # dongle reboots and/or FusionSolar portal updates to be delayed or even paused. 
         self.inverter.close()
 
     def isConnected(self):
         """Check if underlying tcp socket is open"""
         return self.inverter.is_socket_open()
 
+    @property
+    def connected(self):
+        return self.isConnected()
+
     def read_raw_value(self, register):
         if not self.isConnected():
             raise ValueError('Inverter is not connected')
 
         try:
             register_value = self.inverter.read_holding_registers(register.value.address, register.value.quantity, unit=self.unit)
             if type(register_value) == ModbusIOException:
-                logging.error("Inverter unit did not respond")
+                logger.error("Inverter unit did not respond")
                 raise register_value
         except ConnectionException:
-            logging.error("A connection error occurred")
+            logger.error("A connection error occurred")
             raise
 
         return datatypes.decode(register_value.encode()[1:], register.value.data_type)
 
     def read(self, register):
         raw_value = self.read_raw_value(register)
 
         if register.value.gain is None:
             return raw_value
         else:
             return raw_value / register.value.gain
 
-    def read_formatted(self, register):
+    def read_formatted(self, register, use_locale=False):
         value = self.read(register)
 
         if register.value.unit is not None:
-            return f'{value} {register.value.unit}'
+            if use_locale:
+                return f'{value:n} {register.value.unit}'
+            else:
+                return f'{value} {register.value.unit}'
         elif register.value.mapping is not None:
             return register.value.mapping.get(value, 'undefined')
         else:
             return value
 
     def read_range(self, start_address, quantity=0, end_address=0):
         if quantity == 0 and end_address == 0:
@@ -82,14 +94,14 @@
             raise ValueError('Inverter is not connected')
 
         if end_address != 0:
             quantity = end_address - start_address + 1
         try:
             register_range_value = self.inverter.read_holding_registers(start_address, quantity, unit=self.unit)
             if type(register_range_value) == ModbusIOException:
-                logging.error("Inverter unit did not respond")
+                logger.error("Inverter unit did not respond")
                 raise register_range_value
         except ConnectionException:
-            logging.error("A connection error occurred")
+            logger.error("A connection error occurred")
             raise
 
         return datatypes.decode(register_range_value.encode()[1:], datatypes.DataType.MULTIDATA)
```

### Comparing `sun2000_modbus-2.1.1/sun2000_modbus/mappings.py` & `sun2000_modbus-2.2.0/sun2000_modbus/mappings.py`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/sun2000_modbus/registers.py` & `sun2000_modbus-2.2.0/sun2000_modbus/registers.py`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/tests/sun2000mock.py` & `sun2000_modbus-2.2.0/tests/sun2000mock.py`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/tests/test_sun2000_modbus.py` & `sun2000_modbus-2.2.0/tests/test_sun2000_modbus.py`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-2.1.1/PKG-INFO` & `sun2000_modbus-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sun2000_modbus
-Version: 2.1.1
+Version: 2.2.0
 Summary: Library for reading Huawei Sun2000 inverter metrics via Modbus TCP
 Keywords: sun2000,modbus,photovoltaic
 Author-email: Oliver Gregorius <oliver@gregorius.dev>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

