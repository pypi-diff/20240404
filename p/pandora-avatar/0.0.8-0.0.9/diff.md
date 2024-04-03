# Comparing `tmp/pandora-avatar-0.0.8.tar.gz` & `tmp/pandora-avatar-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandora-avatar-0.0.8.tar", last modified: Thu Mar 14 21:03:28 2024, max compression
+gzip compressed data, was "pandora-avatar-0.0.9.tar", last modified: Wed Apr  3 22:10:48 2024, max compression
```

## Comparing `pandora-avatar-0.0.8.tar` & `pandora-avatar-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      965 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/README.md
--rw-r--r--   0        0        0    11139 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/__init__.py
--rw-r--r--   0        0        0     1561 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/aio.py
--rw-r--r--   0        0        0      575 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/cases/__init__.py
--rw-r--r--   0        0        0      376 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/cases/config.yml
--rw-r--r--   0        0        0     5620 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/cases/host_test.py
--rw-r--r--   0        0        0    10657 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/cases/le_host_test.py
--rw-r--r--   0        0        0    17759 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/cases/le_security_test.py
--rw-r--r--   0        0        0    20281 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/cases/security_test.py
--rw-r--r--   0        0        0      608 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/controllers/__init__.py
--rw-r--r--   0        0        0     1464 2024-03-14 21:03:21.940638 pandora-avatar-0.0.8/avatar/controllers/bumble_device.py
--rw-r--r--   0        0        0     1668 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/controllers/pandora_device.py
--rw-r--r--   0        0        0      383 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/metrics/README.md
--rw-r--r--   0        0        0      598 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/metrics/__init__.py
--rw-r--r--   0        0        0     9858 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/metrics/interceptors.py
--rw-r--r--   0        0        0     2042 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/metrics/trace.proto
--rw-r--r--   0        0        0     9765 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/metrics/trace.py
--rw-r--r--   0        0        0     3814 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/metrics/trace_pb2.py
--rw-r--r--   0        0        0     5552 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/metrics/trace_pb2.pyi
--rw-r--r--   0        0        0     7802 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/pandora_client.py
--rw-r--r--   0        0        0     5012 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/pandora_server.py
--rw-r--r--   0        0        0     2756 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/pandora_snippet.py
--rw-r--r--   0        0        0        0 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/py.typed
--rw-r--r--   0        0        0     5562 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/avatar/runner.py
--rw-r--r--   0        0        0     3737 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/doc/android-bumble-extensions.md
--rw-r--r--   0        0        0    12175 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/doc/android-guide.md
--rw-r--r--   0        0        0   196945 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/doc/images/avatar-android-bumble-virtual-architecture-simplified.svg
--rw-r--r--   0        0        0   255455 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/doc/images/avatar-extended-architecture-simplified.svg
--rw-r--r--   0        0        0     6901 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/doc/overview.md
--rw-r--r--   0        0        0     2012 2024-03-14 21:03:21.944638 pandora-avatar-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pandora-avatar-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      965 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/README.md
+-rw-r--r--   0        0        0    11195 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/__init__.py
+-rw-r--r--   0        0        0     1561 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/aio.py
+-rw-r--r--   0        0        0      575 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/cases/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/cases/config.yml
+-rw-r--r--   0        0        0     5620 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/cases/host_test.py
+-rw-r--r--   0        0        0    14229 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/cases/le_host_test.py
+-rw-r--r--   0        0        0    17759 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/cases/le_security_test.py
+-rw-r--r--   0        0        0    20281 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/cases/security_test.py
+-rw-r--r--   0        0        0      608 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/controllers/__init__.py
+-rw-r--r--   0        0        0     1464 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/controllers/bumble_device.py
+-rw-r--r--   0        0        0     1668 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/controllers/pandora_device.py
+-rw-r--r--   0        0        0     1254 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/controllers/usb_bumble_device.py
+-rw-r--r--   0        0        0      383 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/metrics/README.md
+-rw-r--r--   0        0        0      598 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/metrics/__init__.py
+-rw-r--r--   0        0        0     9858 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/metrics/interceptors.py
+-rw-r--r--   0        0        0     2042 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/metrics/trace.proto
+-rw-r--r--   0        0        0     9765 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/metrics/trace.py
+-rw-r--r--   0        0        0     3814 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/metrics/trace_pb2.py
+-rw-r--r--   0        0        0     5552 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/metrics/trace_pb2.pyi
+-rw-r--r--   0        0        0     7802 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/pandora_client.py
+-rw-r--r--   0        0        0     5162 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/pandora_server.py
+-rw-r--r--   0        0        0     2756 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/pandora_snippet.py
+-rw-r--r--   0        0        0        0 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/py.typed
+-rw-r--r--   0        0        0     5562 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/avatar/runner.py
+-rw-r--r--   0        0        0     3737 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/doc/android-bumble-extensions.md
+-rw-r--r--   0        0        0    12175 2024-04-03 22:10:42.353492 pandora-avatar-0.0.9/doc/android-guide.md
+-rw-r--r--   0        0        0   196945 2024-04-03 22:10:42.357492 pandora-avatar-0.0.9/doc/images/avatar-android-bumble-virtual-architecture-simplified.svg
+-rw-r--r--   0        0        0   255455 2024-04-03 22:10:42.357492 pandora-avatar-0.0.9/doc/images/avatar-extended-architecture-simplified.svg
+-rw-r--r--   0        0        0     6901 2024-04-03 22:10:42.357492 pandora-avatar-0.0.9/doc/overview.md
+-rw-r--r--   0        0        0     2017 2024-04-03 22:10:42.357492 pandora-avatar-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 pandora-avatar-0.0.9/PKG-INFO
```

### Comparing `pandora-avatar-0.0.8/README.md` & `pandora-avatar-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/__init__.py` & `pandora-avatar-0.0.9/avatar/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """
 Avatar is a scalable multi-platform Bluetooth testing tool capable of running
 any Bluetooth test cases virtually and physically.
 """
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 import argparse
 import enum
 import functools
 import grpc
 import grpc.aio
 import importlib
@@ -50,14 +50,15 @@
 ]
 
 
 PANDORA_COMMON_SERVER_CLASSES: Dict[str, Type[pandora_server.PandoraServer[Any]]] = {
     'PandoraDevice': pandora_server.PandoraServer,
     'AndroidDevice': pandora_server.AndroidPandoraServer,
     'BumbleDevice': pandora_server.BumblePandoraServer,
+    'UsbDevice': pandora_server.UsbBumblePandoraServer,
 }
 
 KEY_PANDORA_SERVER_CLASS = 'pandora_server_class'
 
 
 class PandoraDevices(Sized, Iterable[PandoraDevice]):
     """Utility for abstracting controller registration and Pandora setup."""
```

### Comparing `pandora-avatar-0.0.8/avatar/aio.py` & `pandora-avatar-0.0.9/avatar/aio.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/cases/__init__.py` & `pandora-avatar-0.0.9/avatar/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/cases/host_test.py` & `pandora-avatar-0.0.9/avatar/cases/host_test.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/cases/le_host_test.py` & `pandora-avatar-0.0.9/avatar/cases/le_host_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,19 +26,24 @@
 from mobly import base_test
 from mobly import test_runner
 from mobly.asserts import assert_equal  # type: ignore
 from mobly.asserts import assert_false  # type: ignore
 from mobly.asserts import assert_is_not_none  # type: ignore
 from mobly.asserts import assert_true  # type: ignore
 from mobly.asserts import explicit_pass  # type: ignore
+from pandora.host_pb2 import PRIMARY_1M
+from pandora.host_pb2 import PRIMARY_CODED
 from pandora.host_pb2 import PUBLIC
 from pandora.host_pb2 import RANDOM
+from pandora.host_pb2 import SECONDARY_1M
+from pandora.host_pb2 import SECONDARY_CODED
 from pandora.host_pb2 import Connection
 from pandora.host_pb2 import DataTypes
 from pandora.host_pb2 import OwnAddressType
+from pandora.host_pb2 import PrimaryPhy
 from typing import Any, Dict, Literal, Optional, Union
 
 
 class AdvertisingEventProperties(enum.IntEnum):
     ADV_IND = 0x13
     ADV_DIRECT_IND = 0x15
     ADV_SCAN_IND = 0x12
@@ -54,14 +59,16 @@
 class LeHostTest(base_test.BaseTestClass):  # type: ignore[misc]
     devices: Optional[PandoraDevices] = None
 
     # pandora devices.
     dut: PandoraDevice
     ref: PandoraDevice
 
+    scan_timeout: float
+
     def setup_class(self) -> None:
         self.devices = PandoraDevices(self)
         self.dut, self.ref, *_ = self.devices
         self.scan_timeout = float(self.user_params.get('scan_timeout') or 15.0)  # type: ignore
 
         # Enable BR/EDR mode for Bumble devices.
         for device in self.devices:
@@ -111,15 +118,14 @@
             data=data,  # type: ignore[arg-type]
             scan_response_data=scan_response_data,  # type: ignore[arg-type]
             public=target,
             own_address_type=PUBLIC,
         )
 
         scan = self.dut.host.Scan(legacy=False, passive=False, timeout=self.scan_timeout)
-        report = next((x for x in scan if x.public == self.ref.address))
         try:
             report = next((x for x in scan if x.public == self.ref.address))
 
             # TODO: scannable is not set by the android server
             # TODO: direct_address is not set by the android server
             assert_true(report.legacy, msg='expected legacy advertising report')
             assert_equal(report.connectable, is_connectable or directed == 'directed')
@@ -136,14 +142,93 @@
                 explicit_pass('')
             raise e
         finally:
             scan.cancel()
             advertise.cancel()
 
     @avatar.parameterized(
+        *itertools.product(
+            # The advertisement cannot be both connectable and scannable.
+            ('connectable', 'non_connectable', 'non_connectable_scannable'),
+            ('directed', 'undirected'),
+            # Bumble does not send multiple HCI commands, so it must also fit in
+            # 1 HCI command (max length 251 minus overhead).
+            (0, 150),
+            (PRIMARY_1M, PRIMARY_CODED),
+        ),
+    )  # type: ignore[misc]
+    def test_extended_scan(
+        self,
+        connectable_scannable: Union[
+            Literal['connectable'], Literal['non_connectable'], Literal['non_connectable_scannable']
+        ],
+        directed: Union[Literal['directed'], Literal['undirected']],
+        data_len: int,
+        primary_phy: PrimaryPhy,
+    ) -> None:
+        '''
+        Advertise from the REF device with the specified extended advertising
+        event properties. Use the manufacturer specific data to pad the advertising data to the
+        desired length. The scan response data must always be provided when
+        scannable.
+        '''
+        man_specific_data_length = max(0, data_len - 5)  # Flags (3) + LV (2)
+        man_specific_data = bytes([random.randint(1, 255) for _ in range(man_specific_data_length)])
+        data = DataTypes(manufacturer_specific_data=man_specific_data) if data_len > 0 else None
+        scan_response_data = None
+        # Extended advertisements with advertising data cannot also have
+        # scan response data.
+        if connectable_scannable == 'non_connectable_scannable':
+            scan_response_data = data
+            data = None
+
+        is_connectable = True if connectable_scannable == 'connectable' else False
+        target = self.dut.address if directed == 'directed' else None
+
+        # For a better test, make the secondary phy the same as the primary to
+        # avoid the scan just scanning the 1M advertisement when the primary
+        # phy is CODED.
+        secondary_phy = SECONDARY_1M
+        if primary_phy == PRIMARY_CODED:
+            secondary_phy = SECONDARY_CODED
+
+        advertise = self.ref.host.Advertise(
+            legacy=False,
+            connectable=is_connectable,
+            data=data,  # type: ignore[arg-type]
+            scan_response_data=scan_response_data,  # type: ignore[arg-type]
+            public=target,
+            own_address_type=PUBLIC,
+            primary_phy=primary_phy,
+            secondary_phy=secondary_phy,
+        )
+
+        scan = self.dut.host.Scan(
+            legacy=False,
+            passive=False,
+            timeout=self.scan_timeout,
+            phys=[primary_phy],
+        )
+        try:
+            report = next((x for x in scan if x.public == self.ref.address))
+
+            # TODO: scannable is not set by the android server
+            # TODO: direct_address is not set by the android server
+            assert_false(report.legacy, msg='expected extended advertising report')
+            assert_equal(report.connectable, is_connectable)
+            assert_equal(report.data.manufacturer_specific_data, man_specific_data)
+            assert_false(report.truncated, msg='expected non-truncated advertising report')
+            assert_equal(report.primary_phy, primary_phy)
+        except grpc.aio.AioRpcError as e:
+            raise e
+        finally:
+            scan.cancel()
+            advertise.cancel()
+
+    @avatar.parameterized(
         (dict(incomplete_service_class_uuids16=["183A", "181F"]),),
         (dict(incomplete_service_class_uuids32=["FFFF183A", "FFFF181F"]),),
         (dict(incomplete_service_class_uuids128=["FFFF181F-FFFF-1000-8000-00805F9B34FB"]),),
         (dict(shortened_local_name="avatar"),),
         (dict(complete_local_name="avatar_the_last_test_blender"),),
         (dict(tx_power_level=20),),
         (dict(class_of_device=0x40680),),
```

### Comparing `pandora-avatar-0.0.8/avatar/cases/le_security_test.py` & `pandora-avatar-0.0.9/avatar/cases/le_security_test.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/cases/security_test.py` & `pandora-avatar-0.0.9/avatar/cases/security_test.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/controllers/__init__.py` & `pandora-avatar-0.0.9/avatar/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/controllers/bumble_device.py` & `pandora-avatar-0.0.9/avatar/controllers/bumble_device.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/controllers/pandora_device.py` & `pandora-avatar-0.0.9/avatar/controllers/pandora_device.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/metrics/__init__.py` & `pandora-avatar-0.0.9/avatar/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/metrics/interceptors.py` & `pandora-avatar-0.0.9/avatar/metrics/interceptors.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/metrics/trace.proto` & `pandora-avatar-0.0.9/avatar/metrics/trace.proto`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/metrics/trace.py` & `pandora-avatar-0.0.9/avatar/metrics/trace.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/metrics/trace_pb2.py` & `pandora-avatar-0.0.9/avatar/metrics/trace_pb2.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/metrics/trace_pb2.pyi` & `pandora-avatar-0.0.9/avatar/metrics/trace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/pandora_client.py` & `pandora-avatar-0.0.9/avatar/pandora_client.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/pandora_server.py` & `pandora-avatar-0.0.9/avatar/pandora_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import grpc.aio
 import portpicker
 import threading
 import types
 
 from avatar.controllers import bumble_device
 from avatar.controllers import pandora_device
+from avatar.controllers import usb_bumble_device
 from avatar.pandora_client import BumblePandoraClient
 from avatar.pandora_client import PandoraClient
 from bumble import pandora as bumble_server
 from bumble.pandora.device import PandoraDevice as BumblePandoraDevice
 from contextlib import suppress
 from mobly.controllers import android_device
 from mobly.controllers.android_device import AndroidDevice
@@ -101,14 +102,18 @@
                 with suppress(asyncio.CancelledError):
                     await self._task
             self._task = None
 
         avatar.aio.run_until_complete(server_stop())
 
 
+class UsbBumblePandoraServer(BumblePandoraServer):
+    MOBLY_CONTROLLER_MODULE = usb_bumble_device
+
+
 class AndroidPandoraServer(PandoraServer[AndroidDevice]):
     """Manages the Pandora gRPC server on an AndroidDevice."""
 
     MOBLY_CONTROLLER_MODULE = android_device
 
     _instrumentation: Optional[threading.Thread] = None
     _port: int
```

### Comparing `pandora-avatar-0.0.8/avatar/pandora_snippet.py` & `pandora-avatar-0.0.9/avatar/pandora_snippet.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/avatar/runner.py` & `pandora-avatar-0.0.9/avatar/runner.py`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/doc/android-bumble-extensions.md` & `pandora-avatar-0.0.9/doc/android-bumble-extensions.md`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/doc/android-guide.md` & `pandora-avatar-0.0.9/doc/android-guide.md`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/doc/images/avatar-android-bumble-virtual-architecture-simplified.svg` & `pandora-avatar-0.0.9/doc/images/avatar-android-bumble-virtual-architecture-simplified.svg`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/doc/images/avatar-extended-architecture-simplified.svg` & `pandora-avatar-0.0.9/doc/images/avatar-extended-architecture-simplified.svg`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/doc/overview.md` & `pandora-avatar-0.0.9/doc/overview.md`

 * *Files identical despite different names*

### Comparing `pandora-avatar-0.0.8/pyproject.toml` & `pandora-avatar-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
-    "bt-test-interfaces>=0.0.4",
-    "bumble>=0.0.176",
+    "bt-test-interfaces>=0.0.6",
+    "bumble>=0.0.186",
     "protobuf==4.24.2",
-    "grpcio==1.57",
+    "grpcio>=1.62.1",
     "mobly==1.12.2",
     "portpicker>=1.5.2",
 ]
 
 [project.urls]
 Source = "https://github.com/google/avatar"
 
 [project.scripts]
 avatar = "avatar:main"
 
 [project.optional-dependencies]
 dev = [
-    "rootcanal>=1.3.0",
-    "grpcio-tools>=1.57",
+    "rootcanal>=1.10.0",
+    "grpcio-tools>=1.62.1",
     "pyright==1.1.298",
     "mypy==1.5.1",
     "black==23.7.0",
     "isort==5.12.0",
     "types-psutil==5.9.5.16",
     "types-setuptools==68.1.0.1",
     "types-protobuf==4.24.0.1"
```

### Comparing `pandora-avatar-0.0.8/PKG-INFO` & `pandora-avatar-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pandora-avatar
-Version: 0.0.8
+Version: 0.0.9
 Summary: Avatar is a scalable multi-platform Bluetooth testing tool capable of running
 Author-email: Pandora <pandora-core@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: bt-test-interfaces>=0.0.4
-Requires-Dist: bumble>=0.0.176
+Requires-Dist: bt-test-interfaces>=0.0.6
+Requires-Dist: bumble>=0.0.186
 Requires-Dist: protobuf==4.24.2
-Requires-Dist: grpcio==1.57
+Requires-Dist: grpcio>=1.62.1
 Requires-Dist: mobly==1.12.2
 Requires-Dist: portpicker>=1.5.2
-Requires-Dist: rootcanal>=1.3.0 ; extra == "dev"
-Requires-Dist: grpcio-tools>=1.57 ; extra == "dev"
+Requires-Dist: rootcanal>=1.10.0 ; extra == "dev"
+Requires-Dist: grpcio-tools>=1.62.1 ; extra == "dev"
 Requires-Dist: pyright==1.1.298 ; extra == "dev"
 Requires-Dist: mypy==1.5.1 ; extra == "dev"
 Requires-Dist: black==23.7.0 ; extra == "dev"
 Requires-Dist: isort==5.12.0 ; extra == "dev"
 Requires-Dist: types-psutil==5.9.5.16 ; extra == "dev"
 Requires-Dist: types-setuptools==68.1.0.1 ; extra == "dev"
 Requires-Dist: types-protobuf==4.24.0.1 ; extra == "dev"
```

