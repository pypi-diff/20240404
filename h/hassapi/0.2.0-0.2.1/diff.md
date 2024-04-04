# Comparing `tmp/hassapi-0.2.0.tar.gz` & `tmp/hassapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassapi-0.2.0.tar", last modified: Mon Sep 18 21:07:38 2023, max compression
+gzip compressed data, was "hassapi-0.2.1.tar", last modified: Thu Apr  4 21:07:58 2024, max compression
```

## Comparing `hassapi-0.2.0.tar` & `hassapi-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 21:07:38.297320 hassapi-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-09-18 21:07:20.000000 hassapi-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-09-18 21:07:38.297320 hassapi-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-09-18 21:07:20.000000 hassapi-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-09-18 21:07:20.000000 hassapi-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-09-18 21:07:38.297320 hassapi-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-09-18 21:07:20.000000 hassapi-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 21:07:38.293320 hassapi-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 21:07:38.293320 hassapi-0.2.0/src/hassapi/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 21:07:38.293320 hassapi-0.2.0/src/hassapi/client/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/client/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/client/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/client/services.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/client/states.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/client/template.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 21:07:38.297320 hassapi-0.2.0/src/hassapi/models/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/models/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2023-09-18 21:07:20.000000 hassapi-0.2.0/src/hassapi/models/state.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-18 21:07:37.000000 hassapi-0.2.0/src/hassapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 21:07:38.293320 hassapi-0.2.0/src/hassapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-09-18 21:07:38.000000 hassapi-0.2.0/src/hassapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-09-18 21:07:38.000000 hassapi-0.2.0/src/hassapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 21:07:38.000000 hassapi-0.2.0/src/hassapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-18 21:07:38.000000 hassapi-0.2.0/src/hassapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-18 21:07:38.000000 hassapi-0.2.0/src/hassapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:07:58.567534 hassapi-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 21:07:49.000000 hassapi-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-04 21:07:58.567534 hassapi-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-04 21:07:49.000000 hassapi-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-04 21:07:49.000000 hassapi-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 21:07:58.571534 hassapi-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 21:07:49.000000 hassapi-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:07:58.563534 hassapi-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:07:58.563534 hassapi-0.2.1/src/hassapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:07:58.567534 hassapi-0.2.1/src/hassapi/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/client/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/client/states.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/client/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:07:58.567534 hassapi-0.2.1/src/hassapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/models/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-04 21:07:49.000000 hassapi-0.2.1/src/hassapi/models/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-04 21:07:58.000000 hassapi-0.2.1/src/hassapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:07:58.567534 hassapi-0.2.1/src/hassapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-04 21:07:58.000000 hassapi-0.2.1/src/hassapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 21:07:58.000000 hassapi-0.2.1/src/hassapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:07:58.000000 hassapi-0.2.1/src/hassapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 21:07:58.000000 hassapi-0.2.1/src/hassapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 21:07:58.000000 hassapi-0.2.1/src/hassapi.egg-info/top_level.txt
```

### Comparing `hassapi-0.2.0/LICENSE` & `hassapi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/PKG-INFO` & `hassapi-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Home Assistant Python API
 Home-page: https://github.com/hass-api/hassapi
 Author: Vadim Titov
 Author-email: titov.hse@gmail.com
 Project-URL: Bug Tracker, https://github.com/hass-api/hassapi/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,16 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: requests
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 ## [Home Assistant](https://www.home-assistant.io/) Web API Client for Python
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/hassapi?style=flat-square)](https://pypistats.org/packages/hassapi)
 
 ## Examples
 ```python
 from hassapi import Hass
```

### Comparing `hassapi-0.2.0/README.md` & `hassapi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/pyproject.toml` & `hassapi-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/setup.cfg` & `hassapi-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/setup.py` & `hassapi-0.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """Handle module packaging."""
 
+import re
 import subprocess
 import textwrap
 
 from setuptools import setup
 
+RE_VERSION = re.compile(r"(\d+\.\d+\.\d+)")
 
-def _get_release_version() -> None:
+
+def _get_release_version() -> str:
     """Get git release tag version."""
-    version = (
+    version_match = RE_VERSION.search(
         subprocess.run(["git", "describe", "--tags"], stdout=subprocess.PIPE)
         .stdout.decode("utf-8")
         .strip()
     )
-    print("VERSION: ", version)
+    version = version_match[0] if version_match else "0.0.0"
+    print("Release version: ", version)
     return version
 
 
 def _write_version(version: str) -> None:
     """Write version to version.py."""
     with open("src/hassapi/version.py", "w") as file:
         file.write(
@@ -27,10 +31,9 @@
                 __version__ = "{version}"
                 '''
             ).lstrip()
         )
 
 
 version = _get_release_version()
-
 _write_version(version)
-setup(version=version)
+setup(version=version)
```

### Comparing `hassapi-0.2.0/src/hassapi/client/auth.py` & `hassapi-0.2.1/src/hassapi/client/auth.py`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/src/hassapi/client/base.py` & `hassapi-0.2.1/src/hassapi/client/base.py`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/src/hassapi/client/events.py` & `hassapi-0.2.1/src/hassapi/client/events.py`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/src/hassapi/client/services.py` & `hassapi-0.2.1/src/hassapi/client/services.py`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/src/hassapi/client/states.py` & `hassapi-0.2.1/src/hassapi/client/states.py`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/src/hassapi/exceptions.py` & `hassapi-0.2.1/src/hassapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/src/hassapi/models/base.py` & `hassapi-0.2.1/src/hassapi/models/base.py`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/src/hassapi/models/service.py` & `hassapi-0.2.1/src/hassapi/models/service.py`

 * *Files identical despite different names*

### Comparing `hassapi-0.2.0/src/hassapi/models/state.py` & `hassapi-0.2.1/src/hassapi/models/state.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,21 +24,24 @@
 
     entity_id: str
     state: str
     attributes: Dict
     context: Context
     last_changed: datetime
     last_updated: Optional[datetime] = field(default=None)
+    last_reported: Optional[datetime] = field(default=None)
 
     def __post_init__(self) -> None:
         """Cast some attributes into more convenient types."""
         self.context = Context(**self.context)  # type: ignore
         self.last_changed = datetime.strptime(self.last_changed, DATE_FORMAT)  # type: ignore
         if self.last_updated:
             self.last_updated = datetime.strptime(self.last_updated, DATE_FORMAT)  # type: ignore
+        if self.last_reported:
+            self.last_reported = datetime.strptime(self.last_reported, DATE_FORMAT)  # type: ignore
 
 
 class StateList(ModelList):
     """List of HASS State objects."""
 
     def __init__(self, states: Iterable = ()):
         """Init StateList."""
```

### Comparing `hassapi-0.2.0/src/hassapi.egg-info/PKG-INFO` & `hassapi-0.2.1/src/hassapi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassapi
-Version: 0.2.0
+Version: 0.2.1
 Summary: Home Assistant Python API
 Home-page: https://github.com/hass-api/hassapi
 Author: Vadim Titov
 Author-email: titov.hse@gmail.com
 Project-URL: Bug Tracker, https://github.com/hass-api/hassapi/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,16 +15,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: requests
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 ## [Home Assistant](https://www.home-assistant.io/) Web API Client for Python
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/hassapi?style=flat-square)](https://pypistats.org/packages/hassapi)
 
 ## Examples
 ```python
 from hassapi import Hass
```

### Comparing `hassapi-0.2.0/src/hassapi.egg-info/SOURCES.txt` & `hassapi-0.2.1/src/hassapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

