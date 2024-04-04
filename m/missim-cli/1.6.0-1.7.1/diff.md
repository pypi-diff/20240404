# Comparing `tmp/missim_cli-1.6.0.tar.gz` & `tmp/missim_cli-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "missim_cli-1.6.0.tar", last modified: Thu Mar 21 02:47:07 2024, max compression
+gzip compressed data, was "missim_cli-1.7.1.tar", last modified: Thu Apr  4 03:06:29 2024, max compression
```

## Comparing `missim_cli-1.6.0.tar` & `missim_cli-1.7.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:07.158543 missim_cli-1.6.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1892 2024-03-21 02:47:07.158543 missim_cli-1.6.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)     1072 2024-03-21 02:46:45.000000 missim_cli-1.6.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:07.158543 missim_cli-1.6.0/missim_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      411 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/banner.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     1313 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/cli.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:07.158543 missim_cli-1.6.0/missim_cli/docker/
--rw-rw-r--   0 runner    (1000) runner    (1001)     1894 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.dev.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       84 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.network-host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      241 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.network-shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       46 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.ue_editor.host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       52 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.ue_editor.shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)     1307 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.ue_editor.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       56 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.ue_standalone.host.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)       64 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.ue_standalone.shared.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      656 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.ue_standalone.yaml
--rw-rw-r--   0 runner    (1000) runner    (1001)      729 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/docker/docker-compose.yaml
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:07.158543 missim_cli-1.6.0/missim_cli/groups/
--rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/groups/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)    14488 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/groups/base.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      251 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/groups/git.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      831 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/groups/setup.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     4212 2024-03-21 02:46:45.000000 missim_cli-1.6.0/missim_cli/helpers.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-03-21 02:47:07.158543 missim_cli-1.6.0/missim_cli.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1892 2024-03-21 02:47:07.000000 missim_cli-1.6.0/missim_cli.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      963 2024-03-21 02:47:07.000000 missim_cli-1.6.0/missim_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-03-21 02:47:07.000000 missim_cli-1.6.0/missim_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       46 2024-03-21 02:47:07.000000 missim_cli-1.6.0/missim_cli.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       75 2024-03-21 02:47:07.000000 missim_cli-1.6.0/missim_cli.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       11 2024-03-21 02:47:07.000000 missim_cli-1.6.0/missim_cli.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-03-21 02:46:58.000000 missim_cli-1.6.0/missim_cli.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)     1002 2024-03-21 02:47:07.158543 missim_cli-1.6.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-03-21 02:46:45.000000 missim_cli-1.6.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.796282 missim_cli-1.7.1/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1892 2024-04-04 03:06:29.796282 missim_cli-1.7.1/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1072 2024-04-04 03:06:00.000000 missim_cli-1.7.1/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.792282 missim_cli-1.7.1/missim_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      411 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/banner.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1313 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/cli.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.796282 missim_cli-1.7.1/missim_cli/docker/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1894 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.dev.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       84 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.network-host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      241 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.network-shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       46 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.ue_editor.host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       52 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.ue_editor.shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1307 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.ue_editor.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       56 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.ue_standalone.host.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)       64 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.ue_standalone.shared.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      656 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.ue_standalone.yaml
+-rw-rw-r--   0 runner    (1000) runner    (1001)      729 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/docker/docker-compose.yaml
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.796282 missim_cli-1.7.1/missim_cli/groups/
+-rw-rw-r--   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/groups/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)    14488 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/groups/base.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      251 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/groups/git.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      831 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/groups/setup.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     4212 2024-04-04 03:06:00.000000 missim_cli-1.7.1/missim_cli/helpers.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-04 03:06:29.796282 missim_cli-1.7.1/missim_cli.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1892 2024-04-04 03:06:29.000000 missim_cli-1.7.1/missim_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      963 2024-04-04 03:06:29.000000 missim_cli-1.7.1/missim_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-04 03:06:29.000000 missim_cli-1.7.1/missim_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       46 2024-04-04 03:06:29.000000 missim_cli-1.7.1/missim_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       75 2024-04-04 03:06:29.000000 missim_cli-1.7.1/missim_cli.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       11 2024-04-04 03:06:29.000000 missim_cli-1.7.1/missim_cli.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-04 03:06:19.000000 missim_cli-1.7.1/missim_cli.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1002 2024-04-04 03:06:29.796282 missim_cli-1.7.1/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-04 03:06:00.000000 missim_cli-1.7.1/setup.py
```

### Comparing `missim_cli-1.6.0/PKG-INFO` & `missim_cli-1.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missim_cli
-Version: 1.6.0
+Version: 1.7.1
 Summary: A CLI for interacting with the MISSIM platform
 Home-page: https://github.com/Greenroom-Robotics/missim
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `missim_cli-1.6.0/README.md` & `missim_cli-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli/cli.py` & `missim_cli-1.7.1/missim_cli/cli.py`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli/docker/docker-compose.dev.yaml` & `missim_cli-1.7.1/missim_cli/docker/docker-compose.dev.yaml`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli/docker/docker-compose.ue_editor.yaml` & `missim_cli-1.7.1/missim_cli/docker/docker-compose.ue_editor.yaml`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli/docker/docker-compose.ue_standalone.yaml` & `missim_cli-1.7.1/missim_cli/docker/docker-compose.ue_standalone.yaml`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli/docker/docker-compose.yaml` & `missim_cli-1.7.1/missim_cli/docker/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli/groups/base.py` & `missim_cli-1.7.1/missim_cli/groups/base.py`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli/groups/setup.py` & `missim_cli-1.7.1/missim_cli/groups/setup.py`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli/helpers.py` & `missim_cli-1.7.1/missim_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/missim_cli.egg-info/PKG-INFO` & `missim_cli-1.7.1/missim_cli.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missim_cli
-Version: 1.6.0
+Version: 1.7.1
 Summary: A CLI for interacting with the MISSIM platform
 Home-page: https://github.com/Greenroom-Robotics/missim
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `missim_cli-1.6.0/missim_cli.egg-info/SOURCES.txt` & `missim_cli-1.7.1/missim_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `missim_cli-1.6.0/setup.cfg` & `missim_cli-1.7.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = missim_cli
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

