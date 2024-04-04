# Comparing `tmp/rattail-wave-0.1.0.tar.gz` & `tmp/rattail-wave-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattail-wave-0.1.0.tar", last modified: Sat Nov 18 02:19:56 2023, max compression
+gzip compressed data, was "rattail-wave-0.1.1.tar", last modified: Thu Apr  4 01:45:23 2024, max compression
```

## Comparing `rattail-wave-0.1.0.tar` & `rattail-wave-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-18 02:19:56.872633 rattail-wave-0.1.0/
--rw-r--r--   0 lance     (1000) lance     (1000)      303 2023-11-18 02:19:13.000000 rattail-wave-0.1.0/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)       76 2022-09-02 18:18:12.000000 rattail-wave-0.1.0/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1058 2023-11-18 02:19:56.872633 rattail-wave-0.1.0/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      319 2022-09-02 18:18:38.000000 rattail-wave-0.1.0/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-18 02:19:56.868633 rattail-wave-0.1.0/rattail_wave/
--rw-r--r--   0 lance     (1000) lance     (1000)     1004 2022-09-02 18:29:51.000000 rattail-wave-0.1.0/rattail_wave/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2022-09-02 18:29:56.000000 rattail-wave-0.1.0/rattail_wave/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1207 2022-09-02 18:21:10.000000 rattail-wave-0.1.0/rattail_wave/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1611 2022-09-02 22:12:00.000000 rattail-wave-0.1.0/rattail_wave/config.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-18 02:19:56.868633 rattail-wave-0.1.0/rattail_wave/db/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2022-01-29 17:43:32.000000 rattail-wave-0.1.0/rattail_wave/db/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-18 02:19:56.868633 rattail-wave-0.1.0/rattail_wave/db/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     1070 2022-09-02 20:36:51.000000 rattail-wave-0.1.0/rattail_wave/db/model/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2045 2022-09-02 19:32:16.000000 rattail-wave-0.1.0/rattail_wave/db/model/customers.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3847 2022-09-02 21:03:00.000000 rattail-wave-0.1.0/rattail_wave/db/model/wave_cache.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-18 02:19:56.868633 rattail-wave-0.1.0/rattail_wave/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)      990 2022-01-29 19:45:18.000000 rattail-wave-0.1.0/rattail_wave/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1466 2022-09-02 22:03:21.000000 rattail-wave-0.1.0/rattail_wave/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1977 2022-09-02 22:03:49.000000 rattail-wave-0.1.0/rattail_wave/importing/rattail.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1759 2022-09-02 21:40:50.000000 rattail-wave-0.1.0/rattail_wave/importing/versions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7891 2023-05-05 06:59:55.000000 rattail-wave-0.1.0/rattail_wave/importing/wave.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-11-18 02:19:56.868633 rattail-wave-0.1.0/rattail_wave.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1058 2023-11-18 02:19:56.000000 rattail-wave-0.1.0/rattail_wave.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      670 2023-11-18 02:19:56.000000 rattail-wave-0.1.0/rattail_wave.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-11-18 02:19:56.000000 rattail-wave-0.1.0/rattail_wave.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      248 2023-11-18 02:19:56.000000 rattail-wave-0.1.0/rattail_wave.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       19 2023-11-18 02:19:56.000000 rattail-wave-0.1.0/rattail_wave.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       13 2023-11-18 02:19:56.000000 rattail-wave-0.1.0/rattail_wave.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1060 2023-11-18 02:19:56.872633 rattail-wave-0.1.0/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1008 2023-05-16 18:04:12.000000 rattail-wave-0.1.0/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-04 01:45:23.269626 rattail-wave-0.1.1/
+-rw-r--r--   0 lance     (1000) lance     (1000)      418 2024-04-04 01:44:49.000000 rattail-wave-0.1.1/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)       76 2022-09-02 18:18:12.000000 rattail-wave-0.1.1/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1058 2024-04-04 01:45:23.269626 rattail-wave-0.1.1/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      319 2022-09-02 18:18:38.000000 rattail-wave-0.1.1/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-04 01:45:23.269626 rattail-wave-0.1.1/rattail_wave/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1004 2022-09-02 18:29:51.000000 rattail-wave-0.1.1/rattail_wave/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2024-04-04 01:44:54.000000 rattail-wave-0.1.1/rattail_wave/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1207 2022-09-02 18:21:10.000000 rattail-wave-0.1.1/rattail_wave/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1611 2022-09-02 22:12:00.000000 rattail-wave-0.1.1/rattail_wave/config.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-04 01:45:23.269626 rattail-wave-0.1.1/rattail_wave/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2022-01-29 17:43:32.000000 rattail-wave-0.1.1/rattail_wave/db/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-04 01:45:23.269626 rattail-wave-0.1.1/rattail_wave/db/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1070 2022-09-02 20:36:51.000000 rattail-wave-0.1.1/rattail_wave/db/model/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2045 2022-09-02 19:32:16.000000 rattail-wave-0.1.1/rattail_wave/db/model/customers.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3847 2022-09-02 21:03:00.000000 rattail-wave-0.1.1/rattail_wave/db/model/wave_cache.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-04 01:45:23.269626 rattail-wave-0.1.1/rattail_wave/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      990 2022-01-29 19:45:18.000000 rattail-wave-0.1.1/rattail_wave/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1466 2022-09-02 22:03:21.000000 rattail-wave-0.1.1/rattail_wave/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1977 2022-09-02 22:03:49.000000 rattail-wave-0.1.1/rattail_wave/importing/rattail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1759 2022-09-02 21:40:50.000000 rattail-wave-0.1.1/rattail_wave/importing/versions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7891 2023-05-05 06:59:55.000000 rattail-wave-0.1.1/rattail_wave/importing/wave.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-04-04 01:45:23.269626 rattail-wave-0.1.1/rattail_wave.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1058 2024-04-04 01:45:23.000000 rattail-wave-0.1.1/rattail_wave.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      670 2024-04-04 01:45:23.000000 rattail-wave-0.1.1/rattail_wave.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-04-04 01:45:23.000000 rattail-wave-0.1.1/rattail_wave.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      251 2024-04-04 01:45:23.000000 rattail-wave-0.1.1/rattail_wave.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       19 2024-04-04 01:45:23.000000 rattail-wave-0.1.1/rattail_wave.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       13 2024-04-04 01:45:23.000000 rattail-wave-0.1.1/rattail_wave.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1063 2024-04-04 01:45:23.269626 rattail-wave-0.1.1/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1008 2023-05-16 18:04:12.000000 rattail-wave-0.1.1/setup.py
```

### Comparing `rattail-wave-0.1.0/PKG-INFO` & `rattail-wave-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-wave
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rattail integration package for Wave
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-wave-0.1.0/rattail_wave/__init__.py` & `rattail-wave-0.1.1/rattail_wave/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/commands.py` & `rattail-wave-0.1.1/rattail_wave/commands.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/config.py` & `rattail-wave-0.1.1/rattail_wave/config.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/db/model/__init__.py` & `rattail-wave-0.1.1/rattail_wave/db/model/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/db/model/customers.py` & `rattail-wave-0.1.1/rattail_wave/db/model/customers.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/db/model/wave_cache.py` & `rattail-wave-0.1.1/rattail_wave/db/model/wave_cache.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/importing/__init__.py` & `rattail-wave-0.1.1/rattail_wave/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/importing/model.py` & `rattail-wave-0.1.1/rattail_wave/importing/model.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/importing/rattail.py` & `rattail-wave-0.1.1/rattail_wave/importing/rattail.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/importing/versions.py` & `rattail-wave-0.1.1/rattail_wave/importing/versions.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave/importing/wave.py` & `rattail-wave-0.1.1/rattail_wave/importing/wave.py`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/rattail_wave.egg-info/PKG-INFO` & `rattail-wave-0.1.1/rattail_wave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-wave
-Version: 0.1.0
+Version: 0.1.1
 Summary: Rattail integration package for Wave
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-wave-0.1.0/rattail_wave.egg-info/SOURCES.txt` & `rattail-wave-0.1.1/rattail_wave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rattail-wave-0.1.0/setup.cfg` & `rattail-wave-0.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 install_requires = 
 	invoke
 	rattail[db]
 packages = find:
 include_package_data = True
 
 [options.entry_points]
-rattail.commands = 
+rattail.subcommands = 
 	import-wave = rattail_wave.commands:ImportWave
 rattail.config.extensions = 
 	rattail_wave = rattail_wave.config:RattailWaveExtension
 rattail.importing = 
 	to_rattail.from_wave.import = rattail_wave.importing.wave:FromWaveToRattail
 
 [egg_info]
```

### Comparing `rattail-wave-0.1.0/setup.py` & `rattail-wave-0.1.1/setup.py`

 * *Files identical despite different names*

