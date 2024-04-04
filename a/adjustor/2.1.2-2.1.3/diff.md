# Comparing `tmp/adjustor-2.1.2.tar.gz` & `tmp/adjustor-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adjustor-2.1.2.tar", last modified: Mon Mar 25 22:27:43 2024, max compression
+gzip compressed data, was "adjustor-2.1.3.tar", last modified: Thu Apr  4 16:58:01 2024, max compression
```

## Comparing `adjustor-2.1.2.tar` & `adjustor-2.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.061985 adjustor-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-25 22:27:37.000000 adjustor-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-25 22:27:37.000000 adjustor-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-25 22:27:43.061985 adjustor-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-25 22:27:37.000000 adjustor-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-03-25 22:27:37.000000 adjustor-2.1.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 22:27:43.061985 adjustor-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.053985 adjustor-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.057985 adjustor-2.1.2/src/adjustor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.061985 adjustor-2.1.2/src/adjustor/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/core/acpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/core/alib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/core/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/core/lenovo.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/core/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.061985 adjustor-2.1.2/src/adjustor/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.061985 adjustor-2.1.2/src/adjustor/drivers/asus/
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/drivers/asus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/drivers/asus/settings.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.061985 adjustor-2.1.2/src/adjustor/drivers/lenovo/
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/drivers/lenovo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/drivers/lenovo/settings.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.061985 adjustor-2.1.2/src/adjustor/drivers/smu/
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/drivers/smu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/drivers/smu/qam.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/drivers/smu/smu.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/hhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-25 22:27:37.000000 adjustor-2.1.2/src/adjustor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 22:27:43.061985 adjustor-2.1.2/src/adjustor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-25 22:27:43.000000 adjustor-2.1.2/src/adjustor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-25 22:27:43.000000 adjustor-2.1.2/src/adjustor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 22:27:43.000000 adjustor-2.1.2/src/adjustor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-25 22:27:43.000000 adjustor-2.1.2/src/adjustor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-25 22:27:43.000000 adjustor-2.1.2/src/adjustor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-25 22:27:43.000000 adjustor-2.1.2/src/adjustor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 16:57:55.000000 adjustor-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 16:57:55.000000 adjustor-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-04 16:58:01.269585 adjustor-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 16:57:55.000000 adjustor-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-04 16:57:55.000000 adjustor-2.1.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:58:01.269585 adjustor-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.261585 adjustor-2.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.265585 adjustor-2.1.3/src/adjustor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/acpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/alib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/lenovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/drivers/asus/
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/asus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/asus/settings.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/drivers/lenovo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/lenovo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/lenovo/settings.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/drivers/smu/
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/smu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/smu/qam.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/smu/smu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/hhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/top_level.txt
```

### Comparing `adjustor-2.1.2/LICENSE` & `adjustor-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/PKG-INFO` & `adjustor-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adjustor
-Version: 2.1.2
+Version: 2.1.3
 Summary: Adjustor, a userspace program for managing the TDP of handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/adjustor
 Project-URL: Bug Tracker, https://github.com/hhd-dev/adjustor/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `adjustor-2.1.2/pyproject.toml` & `adjustor-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "adjustor"
-version = "2.1.2"
+version = "2.1.3"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Adjustor, a userspace program for managing the TDP of handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `adjustor-2.1.2/readme.md` & `adjustor-2.1.3/readme.md`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/core/acpi.py` & `adjustor-2.1.3/src/adjustor/core/acpi.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/core/alib.py` & `adjustor-2.1.3/src/adjustor/core/alib.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/core/const.py` & `adjustor-2.1.3/src/adjustor/core/const.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/core/lenovo.py` & `adjustor-2.1.3/src/adjustor/core/lenovo.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/core/platform.py` & `adjustor-2.1.3/src/adjustor/core/platform.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/drivers/asus/__init__.py` & `adjustor-2.1.3/src/adjustor/drivers/asus/__init__.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/drivers/asus/settings.yml` & `adjustor-2.1.3/src/adjustor/drivers/asus/settings.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/drivers/lenovo/__init__.py` & `adjustor-2.1.3/src/adjustor/drivers/lenovo/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 
 from hhd.plugins import Context, HHDPlugin, HHDSettings, load_relative_yaml
 from hhd.plugins.conf import Config
 
 from adjustor.core.lenovo import (
     MIN_CURVE,
     TdpMode,
-    get_fan_curve,
-    get_fast_tdp,
     get_full_fan_speed,
     get_power_light,
-    get_steady_tdp,
     get_tdp_mode,
     set_fan_curve,
     set_fast_tdp,
     set_full_fan_speed,
     set_power_light,
     set_slow_tdp,
     set_steady_tdp,
@@ -137,14 +134,22 @@
                 tdp_reset = True
 
         # In custom mode, re-apply settings with debounce
         if new_mode == "custom":
             # Check user changed values
             steady = conf["tdp.lenovo.tdp.custom.tdp"].to(int)
 
+            old_steady = steady
+            if self.enforce_limits:
+                steady = min(max(steady, 4), 30)
+            else:
+                steady = min(max(steady, 0), 50)
+            if old_steady != steady:
+                conf["tdp.lenovo.tdp.custom.tdp"] = steady
+
             steady_updated = steady and steady != self.old_conf["tdp.custom.tdp"].to(
                 int
             )
 
             if self.startup and (steady > 30 or steady < 7):
                 logger.warning(
                     f"TDP ({steady}) outside the device spec. Resetting for stability reasons."
@@ -185,18 +190,23 @@
         # Handle fan curve resets
         if conf["tdp.lenovo.fan.manual.reset"].to(bool):
             conf["tdp.lenovo.fan.manual.reset"] = False
             for i, v in enumerate(MIN_CURVE):
                 conf[f"tdp.lenovo.fan.manual.st{(i + 1)*10}"] = v
 
         # Handle fan curve limits
-        if conf["tdp.lenovo.fan.manual.enforce_limits"].to(bool):
-            for i, v in enumerate(MIN_CURVE):
-                if conf[f"tdp.lenovo.fan.manual.st{(i + 1)*10}"].to(int) < v:
-                    conf[f"tdp.lenovo.fan.manual.st{(i + 1)*10}"] = v
+        for i, v in enumerate(MIN_CURVE):
+            val = conf[f"tdp.lenovo.fan.manual.st{(i + 1)*10}"].to(int)
+            old_val = val
+            if conf["tdp.lenovo.fan.manual.enforce_limits"].to(bool) and val < v:
+                val = v
+
+            val = max(min(val, 115), 0)
+            if old_val != val:
+                conf[f"tdp.lenovo.fan.manual.st{(i + 1)*10}"] = val
 
         # Check if fan curve has changed
         # Use debounce logic on these changes
         for i in (10, 20, 30, 40, 50, 60, 70, 80, 90, 100):
             if conf[f"tdp.lenovo.fan.manual.st{i}"].to(int) != self.old_conf[
                 f"fan.manual.st{i}"
             ].to(int):
```

### Comparing `adjustor-2.1.2/src/adjustor/drivers/lenovo/settings.yml` & `adjustor-2.1.3/src/adjustor/drivers/lenovo/settings.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/drivers/smu/__init__.py` & `adjustor-2.1.3/src/adjustor/drivers/smu/__init__.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/drivers/smu/smu.yml` & `adjustor-2.1.3/src/adjustor/drivers/smu/smu.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/events.py` & `adjustor-2.1.3/src/adjustor/events.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/hhd.py` & `adjustor-2.1.3/src/adjustor/hhd.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/settings.yml` & `adjustor-2.1.3/src/adjustor/settings.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor/utils.py` & `adjustor-2.1.3/src/adjustor/utils.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.2/src/adjustor.egg-info/PKG-INFO` & `adjustor-2.1.3/src/adjustor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adjustor
-Version: 2.1.2
+Version: 2.1.3
 Summary: Adjustor, a userspace program for managing the TDP of handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/adjustor
 Project-URL: Bug Tracker, https://github.com/hhd-dev/adjustor/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `adjustor-2.1.2/src/adjustor.egg-info/SOURCES.txt` & `adjustor-2.1.3/src/adjustor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

