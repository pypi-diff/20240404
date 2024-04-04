# Comparing `tmp/gattlib-py-0.4.9.tar.gz` & `tmp/gattlib-py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattlib-py-0.4.9.tar", last modified: Sun Mar 17 23:42:52 2024, max compression
+gzip compressed data, was "gattlib-py-0.5.0.tar", last modified: Thu Apr  4 10:53:19 2024, max compression
```

## Comparing `gattlib-py-0.4.9.tar` & `gattlib-py-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 23:42:52.028149 gattlib-py-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-17 23:42:52.028149 gattlib-py-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 23:42:52.028149 gattlib-py-0.4.9/gattlib/
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/gattlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/gattlib/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/gattlib/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/gattlib/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/gattlib/gatt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/gattlib/mainloop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/gattlib/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 23:42:52.028149 gattlib-py-0.4.9/gattlib_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-17 23:42:52.000000 gattlib-py-0.4.9/gattlib_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-17 23:42:52.000000 gattlib-py-0.4.9/gattlib_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 23:42:52.000000 gattlib-py-0.4.9/gattlib_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-17 23:42:52.000000 gattlib-py-0.4.9/gattlib_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-17 23:42:52.000000 gattlib-py-0.4.9/gattlib_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 23:42:52.028149 gattlib-py-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-03-17 23:22:02.000000 gattlib-py-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/gattlib/
+-rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11167 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/gatt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/mainloop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/gattlib/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/gattlib_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 10:53:19.000000 gattlib-py-0.5.0/gattlib_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:53:19.333000 gattlib-py-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-04-04 10:35:39.000000 gattlib-py-0.5.0/setup.py
```

### Comparing `gattlib-py-0.4.9/PKG-INFO` & `gattlib-py-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.4.9/gattlib/__init__.py` & `gattlib-py-0.5.0/gattlib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 # Copyright (c) 2016-2024, Olivier Martin <olivier@labapart.org>
 #
 
 from ctypes import *
 import logging
 import pathlib
 
+try:
+    # '_version.py' is generated by 'setup.py'
+    from ._version import __version__
+except:
+    pass
+
 logger = logging.getLogger(__name__)
 
 try:
     gattlib = cdll.LoadLibrary(str(pathlib.Path(__file__).with_name('libgattlib.so')))
 except OSError:
     # While in development, we might not have 'libgattlib.so' into the python directory
     # We can define 'libgattlib.so' location using LD_LIBRARY_PATH
@@ -142,17 +148,17 @@
 gattlib_adapter_scan_eddystone = gattlib.gattlib_adapter_scan_eddystone
 gattlib_adapter_scan_eddystone.argtypes = [c_void_p, c_int16, c_uint32, py_object, c_size_t, py_object]
 
 # int gattlib_connect(void *adapter, const char *dst, unsigned long options, gatt_connect_cb_t connect_cb, void* user_data)
 gattlib_connect = gattlib.gattlib_connect
 gattlib_connect.argtypes = [c_void_p, c_char_p, c_ulong, c_void_p, c_void_p]
 
-# int gattlib_disconnect(gatt_connection_t* connection);
+# int gattlib_disconnect(gatt_connection_t* connection, bool wait_disconnection);
 gattlib_disconnect = gattlib.gattlib_disconnect
-gattlib_disconnect.argtypes = [c_void_p]
+gattlib_disconnect.argtypes = [c_void_p, c_bool]
 
 # int gattlib_discover_primary(gatt_connection_t* connection, gattlib_primary_service_t** services, int* services_count);
 gattlib_discover_primary = gattlib.gattlib_discover_primary
 gattlib_discover_primary.argtypes = [c_void_p, POINTER(POINTER(GattlibPrimaryService)), POINTER(c_int)]
 
 # int gattlib_discover_char(gatt_connection_t* connection, gattlib_characteristic_t** characteristics, int* characteristic_count);
 gattlib_discover_char = gattlib.gattlib_discover_char
```

### Comparing `gattlib-py-0.4.9/gattlib/adapter.py` & `gattlib-py-0.5.0/gattlib/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,34 +60,38 @@
         # TODO: Add support
         return []
 
     def open(self):
         self._lock.acquire()
         if self._is_opened:
             self._lock.release()
-            return 0
+            return
 
-        self._adapter = c_void_p(None)
-        ret = gattlib_adapter_open(self._name, byref(self._adapter))
-        if ret == 0:
-            self._is_opened = True
-            if self._name is None:
-                self._name = gattlib_adapter_get_name(self._adapter)
-        self._lock.release()
-        return ret
+        try:
+            self._adapter = c_void_p(None)
+            ret = gattlib_adapter_open(self._name, byref(self._adapter))
+            if ret == 0:
+                self._is_opened = True
+                if self._name is None:
+                    self._name = gattlib_adapter_get_name(self._adapter)
+            else:
+                handle_return(ret)
+        finally:
+            self._lock.release()
 
     def close(self):
         self._lock.acquire()
-        ret = 0
-        if self._adapter:
-            ret = gattlib.gattlib_adapter_close(self._adapter)
-        self._is_opened = False
-        self._adapter = None
-        self._lock.release()
-        return ret
+        try:
+            if self._adapter:
+                ret = gattlib.gattlib_adapter_close(self._adapter)
+                handle_return(ret)
+            self._is_opened = False
+            self._adapter = None
+        finally:
+            self._lock.release()
 
     # Use a closure to return a method that can be called by the C-library (see: https://stackoverflow.com/a/7261524/6267288)
     def get_on_discovered_device_callback(self):
         def on_discovered_device(adapter, addr, name, user_data):
             try:
                 device = Device(self, addr, name)
                 self.on_discovered_device_user_callback(device, user_data)
```

### Comparing `gattlib-py-0.4.9/gattlib/device.py` & `gattlib-py-0.5.0/gattlib/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,19 +134,19 @@
 
             self._disconnection_lock.release()
 
         gattlib_register_on_disconnect(self.connection,
                                        gattlib_disconnected_device_python_callback,
                                        gattlib_python_callback_args(on_disconnection, user_data))
 
-    def disconnect(self):
+    def disconnect(self, wait_disconnection: bool = False):
         self._connection_lock.acquire()
         try:
             if self._connection:
-                ret = gattlib_disconnect(self.connection)
+                ret = gattlib_disconnect(self.connection, wait_disconnection)
                 handle_return(ret)
             self._connection = None
         finally:
             self._connection_lock.release()
 
     def discover(self):
         #
```

### Comparing `gattlib-py-0.4.9/gattlib/exception.py` & `gattlib-py-0.5.0/gattlib/exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,33 +3,41 @@
 #
 # Copyright (c) 2016-2024, Olivier Martin <olivier@labapart.org>
 #
 
 GATTLIB_SUCCESS = 0
 GATTLIB_INVALID_PARAMETER = 1
 GATTLIB_NOT_FOUND = 2
-GATTLIB_ERROR_TIMEOUT = 3
+GATTLIB_TIMEOUT = 3
 GATTLIB_OUT_OF_MEMORY = 4
 GATTLIB_NOT_SUPPORTED = 5
 GATTLIB_DEVICE_ERROR = 6
 GATTLIB_DEVICE_NOT_CONNECTED = 7
 GATTLIB_NO_ADAPTER = 8
+GATTLIB_BUSY = 9
+GATTLIB_UNEXPECTED = 10
 
 GATTLIB_ERROR_MODULE_MASK      = 0xF0000000
 GATTLIB_ERROR_DBUS             = 0x10000000
 GATTLIB_ERROR_BLUEZ            = 0x20000000
 GATTLIB_ERROR_INTERNAL         = 0x80000000
 
 
 class GattlibException(Exception):
     pass
 
 class NoAdapter(GattlibException):
     pass
 
+class Busy(GattlibException):
+    pass
+
+class Unexpected(GattlibException):
+    pass
+
 class AdapterNotOpened(GattlibException):
     pass
 
 class InvalidParameter(GattlibException):
     pass
 
 class NotFound(GattlibException):
@@ -70,23 +78,27 @@
 def handle_return(ret):
     if ret == GATTLIB_INVALID_PARAMETER:
         raise InvalidParameter()
     elif ret == GATTLIB_NOT_FOUND:
         raise NotFound()
     elif ret == GATTLIB_OUT_OF_MEMORY:
         raise OutOfMemory()
-    elif ret == GATTLIB_ERROR_TIMEOUT:
+    elif ret == GATTLIB_TIMEOUT:
         raise TimeoutError()
     elif ret == GATTLIB_NOT_SUPPORTED:
         raise NotSupported()
     elif ret == GATTLIB_DEVICE_ERROR:
         raise DeviceError()
     elif ret == GATTLIB_DEVICE_NOT_CONNECTED:
         raise NotConnected()
     elif ret == GATTLIB_NO_ADAPTER:
         raise NoAdapter()
+    elif ret == GATTLIB_BUSY:
+        raise Busy()
+    elif ret == GATTLIB_UNEXPECTED:
+        raise Unexpected()
     elif (ret & GATTLIB_ERROR_MODULE_MASK) == GATTLIB_ERROR_DBUS:
         raise DBusError((ret >> 8) & 0xFFF, ret & 0xFFFF)
     elif ret == -22: # From '-EINVAL'
         raise ValueError("Gattlib value error")
     elif ret != 0:
         raise RuntimeError("Gattlib exception %d" % ret)
```

### Comparing `gattlib-py-0.4.9/gattlib/gatt.py` & `gattlib-py-0.5.0/gattlib/gatt.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.4.9/gattlib/mainloop.py` & `gattlib-py-0.5.0/gattlib/mainloop.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.4.9/gattlib/uuid.py` & `gattlib-py-0.5.0/gattlib/uuid.py`

 * *Files identical despite different names*

### Comparing `gattlib-py-0.4.9/gattlib_py.egg-info/PKG-INFO` & `gattlib-py-0.5.0/gattlib_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattlib-py
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python wrapper for gattlib library
 Home-page: https://github.com/labapart/gattlib/gattlib-py
 Author: Olivier Martin
 Author-email: olivier@labapart.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `gattlib-py-0.4.9/setup.py` & `gattlib-py-0.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,21 @@
 
 # Retrieve version from GIT
 git_version_command = subprocess.Popen(['git', 'describe', '--abbrev=7', '--dirty', '--always', '--tags'],
                                        stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 stdout, stderr = git_version_command.communicate()
 git_version = stdout.decode('utf-8').strip()
 
+#
+# Create '_version.py'
+#
+package_version = os.environ.get('GATTLIB_PY_VERSION', git_version)
+with open(os.path.join("gattlib", "_version.py"), "w") as f:
+    f.write(f"__version__ = \"{package_version}\"\n")
+
 
 class CMakeExtension(Extension):
     """Custom extension class that allows to specify the root folder of the CMake project."""
     def __init__(self, name, sourcedir='.', **kwa):
         Extension.__init__(self, name, sources=[], **kwa)
         self.sourcedir = os.path.abspath(sourcedir)
 
@@ -145,15 +152,15 @@
         )
         subprocess.run(
             ["cmake", "--build", ".", "--target", "gattlib", *build_args], cwd=build_temp, check=True
         )
 
 setup(
     name='gattlib-py',
-    version=os.environ.get('GATTLIB_PY_VERSION', git_version),
+    version=package_version,
     author="Olivier Martin",
     author_email="olivier@labapart.com",
     description="Python wrapper for gattlib library",
     url="https://github.com/labapart/gattlib/gattlib-py",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

