# Comparing `tmp/romy-0.0.8.tar.gz` & `tmp/romy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romy-0.0.8.tar", last modified: Sun Mar 10 09:12:30 2024, max compression
+gzip compressed data, was "romy-0.0.9.tar", last modified: Wed Mar 13 19:41:06 2024, max compression
```

## Comparing `romy-0.0.8.tar` & `romy-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 09:12:30.535619 romy-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-10 09:12:25.000000 romy-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-10 09:12:30.535619 romy-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-10 09:12:25.000000 romy-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-10 09:12:25.000000 romy-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 09:12:30.535619 romy-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 09:12:30.535619 romy-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 09:12:30.535619 romy-0.0.8/src/romy/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-10 09:12:25.000000 romy-0.0.8/src/romy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 09:12:25.000000 romy-0.0.8/src/romy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-03-10 09:12:25.000000 romy-0.0.8/src/romy/romy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-10 09:12:25.000000 romy-0.0.8/src/romy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 09:12:30.535619 romy-0.0.8/src/romy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-10 09:12:30.000000 romy-0.0.8/src/romy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-10 09:12:30.000000 romy-0.0.8/src/romy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 09:12:30.000000 romy-0.0.8/src/romy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-10 09:12:30.000000 romy-0.0.8/src/romy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-10 09:12:30.000000 romy-0.0.8/src/romy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-10 09:12:25.000000 romy-0.0.8/src/usage_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:41:06.566128 romy-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-13 19:40:58.000000 romy-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-13 19:41:06.566128 romy-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-13 19:40:58.000000 romy-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-13 19:40:58.000000 romy-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 19:41:06.566128 romy-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:41:06.562128 romy-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:41:06.562128 romy-0.0.9/src/romy/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-13 19:40:58.000000 romy-0.0.9/src/romy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 19:40:58.000000 romy-0.0.9/src/romy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-03-13 19:40:58.000000 romy-0.0.9/src/romy/romy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-13 19:40:58.000000 romy-0.0.9/src/romy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:41:06.566128 romy-0.0.9/src/romy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-13 19:41:06.000000 romy-0.0.9/src/romy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-13 19:41:06.000000 romy-0.0.9/src/romy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:41:06.000000 romy-0.0.9/src/romy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-13 19:41:06.000000 romy-0.0.9/src/romy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-13 19:41:06.000000 romy-0.0.9/src/romy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-13 19:40:58.000000 romy-0.0.9/src/usage_example.py
```

### Comparing `romy-0.0.8/LICENSE` & `romy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `romy-0.0.8/PKG-INFO` & `romy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python program and library to control Wi-Fi enabled ROMY vacuum cleaners
 Author-email: Manuel Dipolt <manuel.dipolt@robart.cc>
 Project-URL: Homepage, https://github.com/xeniter/romy
 Project-URL: Bug Tracker, https://github.com/xeniter/romy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `romy-0.0.8/README.md` & `romy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `romy-0.0.8/pyproject.toml` & `romy-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "romy"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Manuel Dipolt", email="manuel.dipolt@robart.cc" },
 ]
 description = "Python program and library to control Wi-Fi enabled ROMY vacuum cleaners"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies    = [
```

### Comparing `romy-0.0.8/src/romy/romy.py` & `romy-0.0.9/src/romy/romy.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,16 @@
         self._model : str = ""
         self._firmware : str = ""
 
         self._battery_level : None | int = None
         self._fan_speed : int = 0
         self._status : None | str = None
 
-        self._sensors : dict[str, bool] = {}
+        self._sensors : dict[str, int] = {}
         self._binary_sensors : dict[str, bool] = {}
-        self._adc_sensors : dict[str, bool] = {}
-
 
     async def _init(self):
 
         self._initialized = False
         # check all ports and if local http interface is locked
         for port in self._ports:            
             _, _, http_status = await async_query_with_http_status(self._host, port, "ishttpinterfacelocked")
@@ -180,29 +178,23 @@
     @property
     def status(self) -> str | None:
         """Return the status of your ROMY."""
         return self._status
 
 
     @property
-    def sensors(self) -> dict[str, bool]:
+    def sensors(self) -> dict[str, int]:
         """Return the available sensors of your ROMY."""
         return self._sensors
 
     @property
     def binary_sensors(self) -> dict[str, bool]:
         """Return the available sensors of your ROMY."""
         return self._binary_sensors
 
-    @property
-    def adc_sensors(self) -> dict[str, bool]:
-        """Return the available sensors of your ROMY."""
-        return self._adc_sensors
-
-
     async def get_protocol_version(self, **kwargs: Any) -> str:
         """Get http api version."""
         ret, json_resp = await self.romy_async_query(f"get/protocol_version")
         version = json.loads(json_resp)
         return f"{version['version_major']}.{version['version_minor']}.{version['patch_level']}"
```

### Comparing `romy-0.0.8/src/romy/utils.py` & `romy-0.0.9/src/romy/utils.py`

 * *Files identical despite different names*

### Comparing `romy-0.0.8/src/romy.egg-info/PKG-INFO` & `romy-0.0.9/src/romy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python program and library to control Wi-Fi enabled ROMY vacuum cleaners
 Author-email: Manuel Dipolt <manuel.dipolt@robart.cc>
 Project-URL: Homepage, https://github.com/xeniter/romy
 Project-URL: Bug Tracker, https://github.com/xeniter/romy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `romy-0.0.8/src/usage_example.py` & `romy-0.0.9/src/usage_example.py`

 * *Files identical despite different names*

