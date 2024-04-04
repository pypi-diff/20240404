# Comparing `tmp/smart_meter_to_openhab-0.3.2.tar.gz` & `tmp/smart_meter_to_openhab-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_meter_to_openhab-0.3.2.tar", max compression
+gzip compressed data, was "smart_meter_to_openhab-0.3.3.tar", max compression
```

## Comparing `smart_meter_to_openhab-0.3.2.tar` & `smart_meter_to_openhab-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1211 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/LICENSE
--rw-r--r--   0        0        0     4538 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/README.md
--rw-r--r--   0        0        0      793 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      543 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/.env.example
--rw-r--r--   0        0        0      154 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/__init__.py
--rw-r--r--   0        0        0     9261 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/interfaces.py
--rw-r--r--   0        0        0     5367 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/openhab.py
--rw-r--r--   0        0        0     3512 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/sml_iskra_mt175.py
--rw-r--r--   0        0        0     5623 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/sml_reader.py
--rw-r--r--   0        0        0      168 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/utils.py
--rw-r--r--   0        0        0     6331 2024-03-27 19:49:56.373400 smart_meter_to_openhab-0.3.2/smart_meter_to_openhab_scripts/main.py
--rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/LICENSE
+-rw-r--r--   0        0        0     4538 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/README.md
+-rw-r--r--   0        0        0      793 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      543 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/.env.example
+-rw-r--r--   0        0        0      154 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/__init__.py
+-rw-r--r--   0        0        0     9335 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/interfaces.py
+-rw-r--r--   0        0        0     5645 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/openhab.py
+-rw-r--r--   0        0        0     5694 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/sml_iskra_mt175.py
+-rw-r--r--   0        0        0     3531 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/sml_reader.py
+-rw-r--r--   0        0        0      168 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/utils.py
+-rw-r--r--   0        0        0     6492 2024-04-04 08:23:53.250580 smart_meter_to_openhab-0.3.3/smart_meter_to_openhab_scripts/main.py
+-rw-r--r--   0        0        0     5211 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.3.3/PKG-INFO
```

### Comparing `smart_meter_to_openhab-0.3.2/LICENSE` & `smart_meter_to_openhab-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.3.2/README.md` & `smart_meter_to_openhab-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.3.2/pyproject.toml` & `smart_meter_to_openhab-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smart_meter_to_openhab"
-version = "0.3.2"
+version = "0.3.3"
 description = "Pushing data of ISKRA MT175 smart meter to openhab"
 authors = ["Heiko Bauer <heiko_bauer@icloud.com>"]
 repository = "https://github.com/die-bauerei/smart-meter-to-openhab"
 readme = "README.md"
 packages = [
     {include = "smart_meter_to_openhab"},
     {include = "smart_meter_to_openhab_scripts"}
```

### Comparing `smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/.env.example` & `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/.env.example`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/interfaces.py` & `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,17 @@
     def __iter__(self) -> Iterator[OhItemAndValue]:
         return iter(self._oh_items_and_values)                
     
     def is_invalid(self) -> bool:
         # consider only the values that really will be used (oh_item name not empty)
         return all(oh_item_value.value is None for oh_item_value in self._oh_items_and_values if oh_item_value.oh_item)
     
+    def is_valid(self) -> bool:
+        return not self.is_invalid()
+    
     def value_list(self) -> List[Any]:
         # consider only the values that really will be used (oh_item name not empty)
         return [oh_item_value.value for oh_item_value in self._oh_items_and_values  if oh_item_value.oh_item]
     
     def __eq__(self, other) -> bool:
         if isinstance(other, OhItemAndValueContainer):
             return self._oh_items_and_values == other._oh_items_and_values
```

### Comparing `smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/openhab.py` & `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/openhab.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import http
 import datetime
 from logging import Logger
 from requests.auth import HTTPBasicAuth
 from requests.adapters import HTTPAdapter, Retry
-from typing import List, Tuple
+from typing import List, Tuple, Union
 from statistics import median
 from .interfaces import *
 
 # disable warnings about insecure requests because ssl verification is disabled
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
@@ -75,18 +75,21 @@
                         else:
                             values=[float(data['state']) for data in response.json()['data']]
                 except requests.exceptions.RequestException as e:
                     self._logger.warning("Caught Exception while getting persistence data from openHAB: " + str(e))
                 pers_values.append(values)
         return pers_values
 
-    def check_if_updated(self, oh_item_names : Tuple[str, ...], timedelta : datetime.timedelta) -> bool:
+    def check_if_updated(self, oh_item_names : Tuple[str, ...], timedelta : datetime.timedelta, 
+                         default : Union[SmartMeterValues, ExtendedSmartMeterValues, None] = None) -> bool:
         pers_values=self._get_persistence_values(oh_item_names, timedelta)
         for values in pers_values:
-            if any(i != values[0] for i in values):
+            if default is not None and default.is_valid() and any(i == default for i in values): # consider a valid default value as updated
+                return True
+            elif any(i != values[0] for i in values):
                 return True
         return False
 
     def get_median_from_items(self, oh_item_names : SmartMeterOhItemNames, timedelta : datetime.timedelta = datetime.timedelta(minutes=30)) -> SmartMeterValues:
         smart_meter_values : List[OhItemAndValue] = []
         pers_values=self._get_persistence_values(oh_item_names, timedelta)
         value_index=0
```

### Comparing `smart_meter_to_openhab-0.3.2/smart_meter_to_openhab/sml_reader.py` & `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab/sml_iskra_mt175.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,117 +1,127 @@
-from time import sleep
-from datetime import datetime
+import serial
+from datetime import timedelta, datetime
 from logging import Logger
-from typing import List, Any, Tuple, Callable
-from .interfaces import SmartMeterValues, ExtendedSmartMeterValues
-from .utils import compute_watt_h
+from typing import Protocol, List, Any
+from functools import cached_property
+from .interfaces import SmartMeterValues
 
 MIN_REF_VALUE_IN_WATT=50
 def _has_outlier(value_list : List[Any], ref_value_list : List[Any]) -> bool:
     for i in range(len(value_list)):
         if value_list[i] is not None and ref_value_list[i] is not None and value_list[i]*0.001 > max(ref_value_list[i], MIN_REF_VALUE_IN_WATT):
             return True
     return False
 
-class SmlReader():
-    SmlReadFunction = Callable[..., SmartMeterValues]
+class SmartMeterReader(Protocol):
+    @cached_property
+    def default(self) -> SmartMeterValues:
+        ...
+    
+    def read(self, ref_values : SmartMeterValues) -> SmartMeterValues:
+        ...
 
-    def __init__(self, logger : Logger) -> None:
+# The smart meter supports consumption only. No electricity feed-in support! (German: Zweirichtungszähler)
+class SmlIskraMt175OneWay():
+    def __init__(self, serial_port : str, logger : Logger) -> None:
+        self._port=serial.Serial(baudrate=9600, bytesize=serial.EIGHTBITS, parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE)
+        self._serial_port=serial_port
         self._logger=logger
-    
-    def read_from_sml(self, read_func : SmlReadFunction, max_read_count : int = 5, 
-                      ref_values : SmartMeterValues = SmartMeterValues()) -> SmartMeterValues:
+
+    @cached_property
+    def default(self) -> SmartMeterValues:
+        return SmartMeterValues(overall_consumption=0, phase_1_consumption=0, phase_2_consumption=0, phase_3_consumption=0)
+
+    def read(self, ref_values : SmartMeterValues) -> SmartMeterValues:
         """Read data from the smart meter via SML and try to validate them
 
         Parameters
         ----------
-        read_func : SmlReadFunction
-            Callable to get measurements. Could later on be used to read from other smart meters.
-        max_read_count : int
-            specifies the number of performed reads to get a valid read
         ref_values : SmartMeterValues
-            Values that are used as baseline. If a new read value is 1000 times higher as the given reference value, 
-            it is considered as outlier and will be ignored.
+            Values that are used as baseline to detect outliers
         
         Returns
         -------
         SmartMeterValues
             Contains the data read from the smart meter
         """
         ref_value_list=ref_values.value_list()
         values=SmartMeterValues()
-        for i in range(max_read_count):
-            values=read_func()
+        for i in range(4): # try n times to get a valid read
+            values=self._read_raw()
             if values.is_invalid():
                 self._logger.info(f"Detected invalid values during SML read. Trying again")
                 continue
             value_list=values.value_list()
             if _has_outlier(value_list, ref_value_list):
                 self._logger.info(f"Detected unrealistic values during SML read. Trying again")
                 continue
             break
 
         value_list=values.value_list()
         if values.is_invalid() or _has_outlier(value_list, ref_value_list):
-            self._logger.info(f"Unable to read and validate SML data. Ignoring following values: {values}")
+            self._logger.warning(f"Unable to read and validate SML data. Ignoring following values: {values}")
             values.reset()
 
-        return values
+        return values if values.is_valid() else self.default
 
-    def read_avg_from_sml(self, read_func : SmlReadFunction, read_count : int, 
-                          ref_values : SmartMeterValues = SmartMeterValues()) -> SmartMeterValues:
-        """Read average data from the smart meter via SML
+    def _read_raw(self, time_out : timedelta = timedelta(seconds=4)) -> SmartMeterValues:
+        """Read raw data from the smart meter via SML
 
         Parameters
         ----------
-        read_func : SmlReadFunction
-            Callable to get measurements. Could later on be used to read from other smart meters.
-        read_count : int
-            specifies the number of performed reads that are averaged. Between each read is a sleep of 1 sec
-        ref_values : SmartMeterValues
-            Values that are used as baseline. If a new read value is 100 times higher as the given reference value, 
-            it is considered as outlier and will be ignored.
-            
+        time_out : timedelta
+            Data reading will be canceled after this time period.
+            NOTE: Take care that this is longer then the specified transmission time of your smart meter.
+        
         Returns
         -------
         SmartMeterValues
             Contains the data read from the smart meter
         """
-        all_values : List[SmartMeterValues] = []
-        for i in range(read_count):
-            values=self.read_from_sml(read_func, 5, ref_values)
-            if not values.is_invalid():
-                 all_values.append(values)
-            sleep(1)
-        if len(all_values) < read_count:
-            self._logger.warning(f"Expected {read_count} valid SML values but only received {len(all_values)}. Returning average value anyway.")
-        return SmartMeterValues.create_avg(all_values)
-    
-    def read_avg_from_sml_and_compute_extended_values(self, read_func : SmlReadFunction, read_count : int, 
-                          ref_values : SmartMeterValues = SmartMeterValues()) -> Tuple[SmartMeterValues, ExtendedSmartMeterValues]:
-        """Read average data from the smart meter via SML and compute overall watt hours from overall watt
+        data = ''
+        smart_meter_values=SmartMeterValues()
+        try:
+            if not self._port.is_open:
+                self._port.port=self._serial_port
+                self._port.open()
+                
+            time_start=datetime.now()
+            while (datetime.now() - time_start) <= time_out:
+                input : bytes = self._port.read()
+                data += input.hex()          # Convert Bytes to Hex String to use find function for easy parsing
+
+                pos = data.find('1b1b1b1b01010101')        # find start of Frame
+
+                if (pos != -1):
+                    data = data[pos:]                      # cut trash before start delimiter
+
+                pos = data.find('1b1b1b1b1a')              # find end of Frame
+
+                if (pos != -1) and len(data) >= pos + 16:
+                    data = data[0:pos + 16]                # cut trash after end delimiter
+                    
+                    pos = data.find('070100010800ff') # looking for OBIS Code: 1-0:1.8.0*255 - Energy kWh
+                    smart_meter_values.electricity_meter.value = int(data[pos+36:pos + 52], 16) / 1e4 if pos != -1 else None
+
+                    pos = data.find('070100100700ff') # looking for OBIS Code: 1-0:16.7.0*255 - Sum Power L1,L2,L3
+                    smart_meter_values.overall_consumption.value = int(data[pos+28:pos+36], 16) if pos != -1 else None
+
+                    pos = data.find('070100240700ff') # looking for OBIS Code: 1-0:36.7.0*255 - current Power L1
+                    smart_meter_values.phase_1_consumption.value = int(data[pos+28:pos+36], 16) if pos != -1 else None
 
-        Parameters
-        ----------
-        read_func : SmlReadFunction
-            Callable to get measurements. Could later on be used to read from other smart meters.
-        read_count : int
-            specifies the number of performed reads that are averaged. Between each read is a sleep of 1 sec
-        ref_values : SmartMeterValues
-            Values that are used as baseline. If a new read value is 100 times higher as the given reference value, 
-            it is considered as outlier and will be ignored.
+                    pos = data.find('070100380700ff') # looking for OBIS Code: 1-0:56.7.0*255 - current Power L2
+                    smart_meter_values.phase_2_consumption.value = int(data[pos+28:pos+36], 16) if pos != -1 else None
+
+                    pos = data.find('0701004c0700ff') # looking for OBIS Code: 1-0:76.7.0*255 - current Power L3
+                    smart_meter_values.phase_3_consumption.value = int(data[pos+28:pos+36], 16) if pos != -1 else None
+
+                    break
             
-        Returns
-        -------
-        Tuple[SmartMeterValues, ExtendedSmartMeterValues]
-            SmartMeterValues: Contains the data read from the smart meter
-            ExtendedSmartMeterValues: Contains extended values like watt hours
-        """
-        time_start=datetime.now()
-        avg_values=self.read_avg_from_sml(read_func, read_count, ref_values)
-        extended_values=ExtendedSmartMeterValues()
-        if avg_values.overall_consumption.value is not None:
-            # TODO: in case of an error (service restart, ...) the computed time delta would not be realistic. 
-            # A possibility would be to take the timestamp of the last value from openHAB.
-            # Even better would be to resolve errors (checkout libsml)
-            extended_values.overall_consumption_wh.value=compute_watt_h(avg_values.overall_consumption.value, datetime.now() - time_start)
-        return (avg_values, extended_values)
+            if (datetime.now() - time_start) > time_out:
+                self._logger.warning(f"Exceeded time out of {time_out} while reading from smart meter.")
+        except serial.SerialException as e:
+            self._logger.info("Caught Exception: " + str(e))
+            #self._port.close() # TODO: is this needed? 
+            smart_meter_values.reset()
+        
+        return smart_meter_values
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `smart_meter_to_openhab-0.3.2/smart_meter_to_openhab_scripts/main.py` & `smart_meter_to_openhab-0.3.3/smart_meter_to_openhab_scripts/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,39 +50,40 @@
     result = subprocess.run(params, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     rc=result.returncode
     if rc != 0:
         raise Exception("Failed to execute command "+ ' '.join(params)+". Return code was: "+str(result.returncode))
 
 def _run(process_start_time : datetime, logger : logging.Logger, read_count : int, interval_in_sec : int, ping_in_min : int, use_uhubctl : bool) -> bool:
     from smart_meter_to_openhab.openhab import OpenhabConnection
-    from smart_meter_to_openhab.sml_iskra_mt175 import SmlIskraMt175
+    from smart_meter_to_openhab.sml_iskra_mt175 import SmlIskraMt175OneWay
     from smart_meter_to_openhab.sml_reader import SmlReader
     from smart_meter_to_openhab.interfaces import SmartMeterValues, ExtendedSmartMeterValues
 
     oh_user=os.getenv('OH_USER') if 'OH_USER' in os.environ else ''
     oh_passwd=os.getenv('OH_PASSWD') if 'OH_PASSWD' in os.environ else ''
     oh_connection = OpenhabConnection(os.getenv('OH_HOST'), oh_user, oh_passwd, logger) # type: ignore
-    sml_iskra = SmlIskraMt175('/dev/ttyUSB0', logger)
+    sml_iskra = SmlIskraMt175OneWay('/dev/ttyUSB0', logger)
     sml_reader = SmlReader(logger)
     logger.info("Connections established. Starting to transfer smart meter values to openhab.")
     ping_timedelta = timedelta(minutes=ping_in_min)
     ping_succeeded=False
     while True:
         logger.info("Reading SML data")
         ref_smart_meter_value=oh_connection.get_median_from_items(SmartMeterValues.oh_item_names())
-        values, extended_values=sml_reader.read_avg_from_sml_and_compute_extended_values(sml_iskra.read, read_count, ref_smart_meter_value)
+        values, extended_values=sml_reader.read_avg_from_sml_and_compute_extended_values(sml_iskra, read_count, 
+                                                                                         ref_values=ref_smart_meter_value)
         logger.info(f"current values: {values}")
         logger.info(f"current extended values: {extended_values}")
         oh_connection.post_to_items(values)
         oh_connection.post_to_items(extended_values)
         logger.info("Values posted to openHAB")
-        sleep(interval_in_sec)
+        sleep(interval_in_sec) # TODO: rm this variable?
         # start pinging after process is running for the specified time
         if (datetime.now() - process_start_time) > ping_timedelta:
-            if not (oh_connection.check_if_updated(SmartMeterValues.oh_item_names(), ping_timedelta) 
+            if not (oh_connection.check_if_updated(SmartMeterValues.oh_item_names(), ping_timedelta, default=sml_iskra.default) 
                     and oh_connection.check_if_updated(ExtendedSmartMeterValues.oh_item_names(), ping_timedelta)):
                 break
             ping_succeeded=True
             logger.info("openHAB items ping successful.")
     
     if use_uhubctl:
         logger.error("openHAB items seem to have not been updated - Power off and on usb ports and reinit process")
```

### Comparing `smart_meter_to_openhab-0.3.2/PKG-INFO` & `smart_meter_to_openhab-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_meter_to_openhab
-Version: 0.3.2
+Version: 0.3.3
 Summary: Pushing data of ISKRA MT175 smart meter to openhab
 Home-page: https://github.com/die-bauerei/smart-meter-to-openhab
 Author: Heiko Bauer
 Author-email: heiko_bauer@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

