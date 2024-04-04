# Comparing `tmp/pygt3x-0.5.2.tar.gz` & `tmp/pygt3x-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygt3x-0.5.2.tar", max compression
+gzip compressed data, was "pygt3x-0.6.0.tar", max compression
```

## Comparing `pygt3x-0.5.2.tar` & `pygt3x-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2024-01-09 10:18:00.918637 pygt3x-0.5.2/LICENSE
--rw-r--r--   0        0        0      765 2024-01-09 10:18:00.918637 pygt3x-0.5.2/README.md
--rw-r--r--   0        0        0      688 2024-01-09 10:18:00.922637 pygt3x-0.5.2/pygt3x/__init__.py
--rw-r--r--   0        0        0     4675 2024-01-09 10:18:00.922637 pygt3x-0.5.2/pygt3x/activity_payload.py
--rw-r--r--   0        0        0     2696 2024-01-09 10:18:00.922637 pygt3x-0.5.2/pygt3x/calibration.py
--rw-r--r--   0        0        0     4887 2024-01-09 10:18:00.922637 pygt3x-0.5.2/pygt3x/components.py
--rw-r--r--   0        0        0    16428 2024-01-09 10:18:00.922637 pygt3x-0.5.2/pygt3x/reader.py
--rw-r--r--   0        0        0      763 2024-01-09 10:18:00.922637 pygt3x-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 pygt3x-0.5.2/setup.py
--rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 pygt3x-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-04 07:01:45.283421 pygt3x-0.6.0/LICENSE
+-rw-r--r--   0        0        0      765 2024-04-04 07:01:45.283421 pygt3x-0.6.0/README.md
+-rw-r--r--   0        0        0      689 2024-04-04 07:01:45.283421 pygt3x-0.6.0/pygt3x/__init__.py
+-rw-r--r--   0        0        0     4676 2024-04-04 07:01:45.283421 pygt3x-0.6.0/pygt3x/activity_payload.py
+-rw-r--r--   0        0        0     2697 2024-04-04 07:01:45.283421 pygt3x-0.6.0/pygt3x/calibration.py
+-rw-r--r--   0        0        0     4766 2024-04-04 07:01:45.283421 pygt3x-0.6.0/pygt3x/components.py
+-rw-r--r--   0        0        0    17478 2024-04-04 07:01:45.283421 pygt3x-0.6.0/pygt3x/reader.py
+-rw-r--r--   0        0        0      789 2024-04-04 07:01:45.283421 pygt3x-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 pygt3x-0.6.0/setup.py
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 pygt3x-0.6.0/PKG-INFO
```

### Comparing `pygt3x-0.5.2/LICENSE` & `pygt3x-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygt3x-0.5.2/README.md` & `pygt3x-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pygt3x-0.5.2/pygt3x/__init__.py` & `pygt3x-0.6.0/pygt3x/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """GT3x python module."""
+
 from enum import Enum, unique
 
 
 @unique
 class Types(Enum):
     """Enum of event types."""
```

### Comparing `pygt3x-0.5.2/pygt3x/activity_payload.py` & `pygt3x-0.6.0/pygt3x/activity_payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Binary payload parsing."""
+
 import struct
 
 import numpy as np
 
 NHANES_SCALE = 341
```

### Comparing `pygt3x-0.5.2/pygt3x/calibration.py` & `pygt3x-0.6.0/pygt3x/calibration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Calibrate accelerometer values."""
+
 from typing import Dict
 
 import numpy as np
 from numpy import typing as npt
 
 
 class CalibrationV2Service:
```

### Comparing `pygt3x-0.5.2/pygt3x/components.py` & `pygt3x-0.6.0/pygt3x/components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """GT3x header structure."""
+
 import io
-import logging
 import struct
-from dataclasses import InitVar, dataclass
+from dataclasses import dataclass, field
 from typing import Optional, Union
 
 import numpy as np
 
 
 @dataclass
 class Header:
@@ -37,15 +37,15 @@
         )
         self.separator = separator
         self.timestamp = timestamp
         self.event_type = event_type
         self.payload_size = payload_size
 
 
-@dataclass(frozen=True)
+@dataclass
 class RawEvent:
     """
     Gt3xRawEvent class.
 
     Attributes:
     -----------
     header:
@@ -54,34 +54,33 @@
         Log event payload as byte array
     checksum:
         Log event checksum
     """
 
     header: Header
     payload: bytes
-    checksum: InitVar[bytes]
+    checksum: bytes
+    is_checksum_valid: bool = field(init=False)
 
-    def __post_init__(self, checksum: bytes):
+    def __post_init__(self):
         """Verify event's checksum."""
         new_checksum = self.header.separator ^ self.header.event_type
         timestamp = self.header.timestamp.to_bytes(4, "little")
         new_checksum = np.bitwise_xor.reduce(
             np.frombuffer(timestamp, dtype=np.uint8), initial=new_checksum
         )
         payload_size = self.header.payload_size.to_bytes(4, "little")
         new_checksum = np.bitwise_xor.reduce(
             np.frombuffer(payload_size, dtype=np.uint8), initial=new_checksum
         )
         new_checksum = np.bitwise_xor.reduce(
             np.frombuffer(self.payload, dtype=np.uint8), initial=new_checksum
         )
         new_checksum = int(~new_checksum & 0xFF)
-        if new_checksum.to_bytes(1, "little") != checksum:
-            logging.warning("Corrupted event at %s.", self.header.timestamp)
-            raise ValueError("Event checksum does not match.")
+        self.is_checksum_valid = new_checksum.to_bytes(1, "little") == self.checksum
 
 
 @dataclass
 class Info:
     """Metadata class."""
 
     acceleration_max: float
```

### Comparing `pygt3x-0.5.2/pygt3x/reader.py` & `pygt3x-0.6.0/pygt3x/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,28 @@
     read_activity3_payload,
     read_nhanes_payload,
     read_temperature_payload,
 )
 from pygt3x.calibration import CalibrationV2Service
 from pygt3x.components import Header, Info, RawEvent
 
+logger = logging.getLogger(__name__)
+
 
 class FileReader:
     """Read GT3X/AGDC files.
 
     Parameters:
     -----------
     file_name:
         Input file name
     """
 
     def __init__(self, file_name: str, num_rows: Optional[int] = None):
         """Initialise."""
-        self.logger = logging.getLogger(__name__)
         self.file_name = file_name
         self.acceleration = np.empty((0, 4))
         self.temperature = np.empty((0, 3))
         self.idle_sleep_mode_activated = None
         self.num_rows = num_rows
         self.nhanes = None
 
@@ -92,15 +93,15 @@
         )
         return result
 
     def _validate_payload(self, payload):
         shape = payload.shape
         expected_shape = (self.info.sample_rate, 4)
         if shape[1:] != expected_shape and shape != expected_shape:
-            self.logger.warning(f"Unexpected payload shape {shape}")
+            logger.warning("Unexpected payload shape %s", shape)
         return payload
 
     def read_events(self, num_rows=None):
         """Read events from file.
 
         Parameters:
         -----------
@@ -139,18 +140,25 @@
         idle_sleep_mode_started = None
         # This is used for filling in gaps created by idle sleep mode
         last_values = None
         last_idsm_ts = 0
         # Initialize evt in case there are no events in the GT3x file
         evt = None
         for evt in self.read_events(num_rows):
+
+            if not evt.is_checksum_valid:
+                logger.warning(
+                    "Event checksum does not match at %s .", evt.header.timestamp
+                )
+                continue
+
             try:
                 type = Types(evt.header.event_type)
             except ValueError:
-                self.logger.warning(f"Unsupported event type {evt.header.event_type}")
+                logger.warning("Unsupported event type %s", evt.header.event_type)
                 continue
 
             if type == Types.Params:
                 params = np.frombuffer(evt.payload, dtype="<u8")
                 for param in params:
                     buffer = param.tobytes()
                     address = np.frombuffer(buffer, dtype="<u1")
@@ -168,37 +176,40 @@
                 dt = evt.header.timestamp - last_second
 
             # Time travel dt is relative to last event,
             # no matter whether it had valid data
             # or was e.g. ISM start/end
             time_travel_dt = last_idsm_ts - evt.header.timestamp
             if time_travel_dt > 0:
-                self.logger.debug(
-                    f"{evt.header.timestamp} --> {dt} time drift by {time_travel_dt}s"
+                logger.debug(
+                    "%s --> %s time drift by %s s",
+                    evt.header.timestamp,
+                    dt,
+                    time_travel_dt,
                 )
 
             # Idle sleep mode is encoded as an event with payload 8 when entering
             # and 09 when leaving.
             if type == Types.Event and evt.payload == b"\x08":
                 if not self.idle_sleep_mode_activated:
-                    self.logger.error(
+                    logger.error(
                         "Found activation of idle sleep mode in the data, but idle "
                         "sleep mode was not activated in the device. This is probably a"
                         "bug in the parser."
                     )
                 last_idsm_ts = evt.header.timestamp
                 dt_idm = dt
                 if dt >= 2:
                     ts = pd.to_datetime(evt.header.timestamp, unit="s")
-                    self.logger.debug(f"Missed {dt}s before {ts}")
+                    logger.debug("Missed %s s before %s", dt, ts)
 
                 if idle_sleep_mode_started is not None:
-                    self.logger.warning(
-                        f"Idle sleep mode was already active at"
-                        f" {idle_sleep_mode_started}"
+                    logger.warning(
+                        "Idle sleep mode was already active at %s",
+                        idle_sleep_mode_started,
                     )
                 idle_sleep_mode_started = evt.header.timestamp
                 continue
             if type == Types.Event and evt.payload == b"\x09":
                 if idle_sleep_mode_started is not None and last_values is not None:
                     last_idsm_ts = evt.header.timestamp
                     # Fill in missing data for dt past payloads
@@ -207,16 +218,16 @@
                     payload = self._validate_payload(
                         self._fill_ism(fill_start, evt.header.timestamp, last_values)
                     )
                     idle_sleep_mode_started = None
                     acceleration.extend(payload)
                     continue
                 else:
-                    self.logger.warning(
-                        f"Idle sleep mode was not active at {evt.header.timestamp}"
+                    logger.warning(
+                        "Idle sleep mode was not active at %s", evt.header.timestamp
                     )
                     continue
 
             # An 'Activity' (id: 0x00) log record type with a 1-byte payload is
             # captured on a USB connection event (and does not represent a reading
             # from the activity monitor's accelerometer). This event is captured
             # upon docking the activity monitor (via USB) to a PC or CentrePoint
@@ -248,19 +259,22 @@
             if payload.shape[0] > 0:
                 last_values = payload[-1, 1:]
                 # Without the next line, if we miss an ISM stop event, we would
                 # think we are in ISM even when receiving accelerometer data.
                 idle_sleep_mode_started = None
             if payload.shape[0] != 0:
                 if time_travel_dt > 0:
-                    self.logger.debug(
-                        f"{evt.header.timestamp}>{dt} time drift by {time_travel_dt}s"
+                    logger.debug(
+                        "%s>%s time drift by %s s",
+                        evt.header.timestamp,
+                        dt,
+                        time_travel_dt,
                     )
-                    self.logger.debug(f"Last valid second: {acceleration[-1][0, 0]}")
-                    acceleration[-1 + dt] = self._validate_payload(payload)
+                    logger.debug("Last valid second: %s", acceleration[-1][0, 0])
+                    acceleration[-1 + int(dt)] = self._validate_payload(payload)
                 else:
                     acceleration.append(self._validate_payload(payload))
 
         if idle_sleep_mode_started is not None:
             # Idle sleep mode was started but not finished before the recording
             # ended. This means that we might be missing some records at the end of
             # the file.
@@ -271,15 +285,15 @@
                     idle_sleep_mode_started - (dt_idm - 1),
                     idle_sleep_mode_ended,
                     last_values,
                 )
             )
             acceleration.extend(payload)
         if evt is not None:
-            self.logger.debug(f"last ts {evt.header.timestamp}")
+            logger.debug("last ts %s", evt.header.timestamp)
         return acceleration, temperature
 
     def _get_data(self, num_rows=None):
         """Yield acceleration data.
 
         Parameters:
         -----------
@@ -287,24 +301,46 @@
             Number of events to read.
         """
         if not self.logreader:
             acceleration, temperature = self._get_data_nhanes()
         else:
             acceleration, temperature = self._get_data_default(num_rows=num_rows)
 
+        # Check for and remove identical samples
+        if len(acceleration) > 1:
+            assert len(acceleration[0].shape) == 2
+            acceleration, counts = np.unique(acceleration, axis=0, return_counts=True)
+            duplicates_removed = acceleration[counts > 1]
+            if duplicates_removed.size > 0:
+                logger.warning(
+                    "%s duplicate accelerometer records removed.",
+                    duplicates_removed.shape[0],
+                )
+                for d in duplicates_removed:
+                    logger.debug(
+                        "Duplicate accelerometer record removed: %s", d.tolist()
+                    )
+
         if len(acceleration) > 0:
             self.acceleration = np.concatenate(acceleration)
         if len(temperature) > 0:
             self.temperature = np.concatenate(temperature)
 
         # Make sure each second appears sample rate times
         counter = Counter(self.acceleration[:, 0].astype(int))
-        wrong_freq_cases = [c for c in counter.values() if c != self.info.sample_rate]
-        if len(wrong_freq_cases) > 0:
-            self.logger.warning(f"Wrong freq cases: {wrong_freq_cases}")
+        wrong_freq_cases = [
+            (k, v) for k, v in counter.items() if v != self.info.sample_rate
+        ]
+        for w in wrong_freq_cases:
+            logger.warning(
+                "Timestamp (second) %s has %s samples instead of %s.",
+                w[0],
+                w[1],
+                self.info.sample_rate,
+            )
 
     def calibrate_acceleration(self):
         """Calibrates acceleration samples."""
         calibration = self.calibration
         info = self.info
         acceleration = self.acceleration
 
@@ -417,12 +453,9 @@
         header = Header(header_bytes)
         payload_bytes = self.source.read(header.payload_size)
         if len(payload_bytes) != header.payload_size:
             return None
         checksum = self.source.read(1)
         if not checksum:
             return None
-        try:
-            raw_event = RawEvent(header, payload_bytes, checksum)
-        except ValueError:
-            return None
+        raw_event = RawEvent(header, payload_bytes, checksum)
         return raw_event
```

### Comparing `pygt3x-0.5.2/pyproject.toml` & `pygt3x-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygt3x"
-version = "0.5.2"
+version = "0.6.0"
 description = "Python module for reading GT3X/AGDC file format data"
 authors = ["Mark Fogle <mark.fogle@theactigraph.com>"]
 maintainers = ["Ali Neishabouri <ali.neishabouri@theactigraph.com>"]
 license = "GPL-3.0-or-later"
 repository = "https://github.com/actigraph/pygt3x"
 readme = "README.md"
 
@@ -16,14 +16,15 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 mypy = "^0.991"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
 pydocstyle = "^6.1.1"
 types-setuptools = "^65.7.0.3"
+flake8-logging = "^1.6.0"
 
 [[tool.mypy.overrides]]
 module = ["pandas"]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pygt3x-0.5.2/setup.py` & `pygt3x-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.21.2', 'pandas>=1.2.5']
 
 setup_kwargs = {
     'name': 'pygt3x',
-    'version': '0.5.2',
+    'version': '0.6.0',
     'description': 'Python module for reading GT3X/AGDC file format data',
     'long_description': '# pygt3x\n![Tests](https://github.com/actigraph/pygt3x/actions/workflows/tests.yml/badge.svg)\n\nPython module for reading GT3X/AGDC file format data generated by ActiGraph devices.\n\n## Example Usage\n\nTo read calibrated accelerometer data, you can use the code snippet below:\n\n```python\nfrom pygt3x.reader import FileReader\n\n# Read raw data and calibrate, then export to pandas data frame\nwith FileReader("FILENAME") as reader:\n    was_idle_sleep_mode_used = reader.idle_sleep_mode_activated\n    df = reader.to_pandas()\n    print(df.head(5))\n```\n\nIf your AGDC file contains temperature data, you can read it using:\n\n```python\nfrom pygt3x.reader import FileReader\n\nwith FileReader("FILENAME") as reader:\n    df = reader.temperature_to_pandas()\n    print(df.head(5))\n```',
     'author': 'Mark Fogle',
     'author_email': 'mark.fogle@theactigraph.com',
     'maintainer': 'Ali Neishabouri',
     'maintainer_email': 'ali.neishabouri@theactigraph.com',
     'url': 'https://github.com/actigraph/pygt3x',
```

### Comparing `pygt3x-0.5.2/PKG-INFO` & `pygt3x-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygt3x
-Version: 0.5.2
+Version: 0.6.0
 Summary: Python module for reading GT3X/AGDC file format data
 Home-page: https://github.com/actigraph/pygt3x
 License: GPL-3.0-or-later
 Author: Mark Fogle
 Author-email: mark.fogle@theactigraph.com
 Maintainer: Ali Neishabouri
 Maintainer-email: ali.neishabouri@theactigraph.com
```

