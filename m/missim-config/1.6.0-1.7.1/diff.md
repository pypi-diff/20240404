# Comparing `tmp/missim_config-1.6.0.tar.gz` & `tmp/missim_config-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missim_config-1.6.0.tar", last modified: Thu Mar 21 02:47:06 2024, max compression
+gzip compressed data, was "missim_config-1.7.1.tar", last modified: Thu Apr  4 03:06:29 2024, max compression
```

## Comparing `missim_config-1.6.0.tar` & `missim_config-1.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:06.762467 missim_config-1.6.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1263 2024-03-21 02:47:06.762467 missim_config-1.6.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      521 2024-03-21 02:46:44.000000 missim_config-1.6.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:06.758466 missim_config-1.6.0/missim_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2701 2024-03-21 02:46:44.000000 missim_config-1.6.0/missim_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      432 2024-03-21 02:46:44.000000 missim_config-1.6.0/missim_config/generate_schemas.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:06.758466 missim_config-1.6.0/missim_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)      970 2024-03-21 02:46:44.000000 missim_config-1.6.0/missim_config/schemas/missim.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:06.758466 missim_config-1.6.0/missim_config/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-03-21 02:46:44.000000 missim_config-1.6.0/missim_config/test/missim_config_test.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:06.762467 missim_config-1.6.0/missim_config.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1263 2024-03-21 02:47:06.000000 missim_config-1.6.0/missim_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      386 2024-03-21 02:47:06.000000 missim_config-1.6.0/missim_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-03-21 02:47:06.000000 missim_config-1.6.0/missim_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       35 2024-03-21 02:47:06.000000 missim_config-1.6.0/missim_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       14 2024-03-21 02:47:06.000000 missim_config-1.6.0/missim_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-03-21 02:46:56.000000 missim_config-1.6.0/missim_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      871 2024-03-21 02:47:06.762467 missim_config-1.6.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-03-21 02:46:44.000000 missim_config-1.6.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.180287 missim_config-1.7.1/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1263 2024-04-04 03:06:29.180287 missim_config-1.7.1/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      521 2024-04-04 03:05:59.000000 missim_config-1.7.1/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.180287 missim_config-1.7.1/missim_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2701 2024-04-04 03:05:59.000000 missim_config-1.7.1/missim_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      432 2024-04-04 03:05:59.000000 missim_config-1.7.1/missim_config/generate_schemas.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.180287 missim_config-1.7.1/missim_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      970 2024-04-04 03:05:59.000000 missim_config-1.7.1/missim_config/schemas/missim.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.180287 missim_config-1.7.1/missim_config/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-04 03:05:59.000000 missim_config-1.7.1/missim_config/test/missim_config_test.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.180287 missim_config-1.7.1/missim_config.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1263 2024-04-04 03:06:29.000000 missim_config-1.7.1/missim_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      386 2024-04-04 03:06:29.000000 missim_config-1.7.1/missim_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-04 03:06:29.000000 missim_config-1.7.1/missim_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       35 2024-04-04 03:06:29.000000 missim_config-1.7.1/missim_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       14 2024-04-04 03:06:29.000000 missim_config-1.7.1/missim_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-04 03:06:15.000000 missim_config-1.7.1/missim_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      871 2024-04-04 03:06:29.180287 missim_config-1.7.1/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-04 03:05:59.000000 missim_config-1.7.1/setup.py
```

### Comparing `missim_config-1.6.0/PKG-INFO` & `missim_config-1.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missim_config
-Version: 1.6.0
+Version: 1.7.1
 Summary: A library for reading / writing Missim config files
 Home-page: https://github.com/Greenroom-Robotics/missim
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `missim_config-1.6.0/README.md` & `missim_config-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `missim_config-1.6.0/missim_config/__init__.py` & `missim_config-1.7.1/missim_config/__init__.py`

 * *Files identical despite different names*

### Comparing `missim_config-1.6.0/missim_config/schemas/missim.schema.json` & `missim_config-1.7.1/missim_config/schemas/missim.schema.json`

 * *Files identical despite different names*

### Comparing `missim_config-1.6.0/missim_config.egg-info/PKG-INFO` & `missim_config-1.7.1/missim_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missim_config
-Version: 1.6.0
+Version: 1.7.1
 Summary: A library for reading / writing Missim config files
 Home-page: https://github.com/Greenroom-Robotics/missim
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `missim_config-1.6.0/setup.cfg` & `missim_config-1.7.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = missim_config
-version = 1.6.0
+version = 1.7.1
 url = https://github.com/Greenroom-Robotics/missim
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

