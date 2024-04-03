# Comparing `tmp/pygo-tools-0.1.5.tar.gz` & `tmp/pygo-tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygo-tools-0.1.5.tar", last modified: Tue Apr  2 22:32:32 2024, max compression
+gzip compressed data, was "pygo-tools-0.1.6.tar", last modified: Wed Apr  3 22:29:45 2024, max compression
```

## Comparing `pygo-tools-0.1.5.tar` & `pygo-tools-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/pygo_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/build_ffi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/pygo_tools/util/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/util/monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pygo_tools/util/pathlib_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/pygo_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 22:32:32.000000 pygo-tools-0.1.5/pygo_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-02 22:32:11.000000 pygo-tools-0.1.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:32:32.342093 pygo-tools-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:29:45.185708 pygo-tools-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-03 22:29:45.185708 pygo-tools-0.1.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:29:45.185708 pygo-tools-0.1.6/pygo_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pygo_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pygo_tools/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pygo_tools/build_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pygo_tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pygo_tools/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:29:45.185708 pygo-tools-0.1.6/pygo_tools/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pygo_tools/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pygo_tools/util/monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pygo_tools/util/pathlib_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:29:45.185708 pygo-tools-0.1.6/pygo_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-03 22:29:45.000000 pygo-tools-0.1.6/pygo_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-03 22:29:45.000000 pygo-tools-0.1.6/pygo_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:29:45.000000 pygo-tools-0.1.6/pygo_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 22:29:45.000000 pygo-tools-0.1.6/pygo_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 22:29:45.000000 pygo-tools-0.1.6/pygo_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 22:29:45.000000 pygo-tools-0.1.6/pygo_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-03 22:29:09.000000 pygo-tools-0.1.6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:29:45.185708 pygo-tools-0.1.6/setup.cfg
```

### Comparing `pygo-tools-0.1.5/PKG-INFO` & `pygo-tools-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygo-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simplify Python-Go integration for Libraries with Precompiled Extensions
 Author-email: Rajan Khullar <rkhullar03@gmail.com>
 License: MIT NON-AI License
 Project-URL: Repository, https://github.com/rkhullar/python-libraries/tree/main/pygo-tools
 Keywords: python,golang,cffi
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pygo-tools-0.1.5/pygo_tools/backend.py` & `pygo-tools-0.1.6/pygo_tools/backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import tempfile
+from pathlib import Path
 
 from setuptools import build_meta as _build_meta
 from setuptools.build_meta import *
 from wheel.bdist_wheel import bdist_wheel
 
 from .config import Config
-from .setup import build_ffi, inject_file, patch_wheel_darwin, precompile
+from .setup import (build_ffi, find_wheel, inject_file, patch_wheel_darwin,
+                    precompile)
 from .util import monkey_patched
 
 
 class custom_bdist_wheel(bdist_wheel):
     def finalize_options(self):
         # NOTE: self.distribution -> setuptools.dist.Distribution
         self.root_is_pure = False
@@ -24,9 +26,12 @@
     with tempfile.TemporaryDirectory() as temp_dir:
         config = Config.from_toml()
         precompile(config)
         source_ffi_path = build_ffi(config, target=temp_dir)
         result = _build_meta.build_wheel(wheel_directory, config_settings, metadata_directory)
         inject_file(config, path=source_ffi_path)
         if config.platform == 'darwin':
-            patch_wheel_darwin(config)
+            wheel_path = find_wheel(config, dist_path=Path(wheel_directory))
+            if not wheel_path:
+                raise FileNotFoundError(f'could not find wheel to patch')
+            patch_wheel_darwin(config, wheel_path=wheel_path)
     return result
```

### Comparing `pygo-tools-0.1.5/pygo_tools/build_ffi.py` & `pygo-tools-0.1.6/pygo_tools/build_ffi.py`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.5/pygo_tools/config.py` & `pygo-tools-0.1.6/pygo_tools/config.py`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.5/pygo_tools/setup.py` & `pygo-tools-0.1.6/pygo_tools/setup.py`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.5/pygo_tools/util/monkey_patch.py` & `pygo-tools-0.1.6/pygo_tools/util/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.5/pygo_tools.egg-info/PKG-INFO` & `pygo-tools-0.1.6/pygo_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygo-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Simplify Python-Go integration for Libraries with Precompiled Extensions
 Author-email: Rajan Khullar <rkhullar03@gmail.com>
 License: MIT NON-AI License
 Project-URL: Repository, https://github.com/rkhullar/python-libraries/tree/main/pygo-tools
 Keywords: python,golang,cffi
 Requires-Python: <4.0,>=3.10
 Description-Content-Type: text/markdown
```

### Comparing `pygo-tools-0.1.5/pyproject.toml` & `pygo-tools-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygo-tools-0.1.5/readme.md` & `pygo-tools-0.1.6/readme.md`

 * *Files identical despite different names*

