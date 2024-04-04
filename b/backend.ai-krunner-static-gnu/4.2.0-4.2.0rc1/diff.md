# Comparing `tmp/backend.ai-krunner-static-gnu-4.2.0.tar.gz` & `tmp/backend.ai-krunner-static-gnu-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-krunner-static-gnu-4.2.0.tar", last modified: Thu Apr  4 12:06:53 2024, max compression
+gzip compressed data, was "backend.ai-krunner-static-gnu-4.2.0rc1.tar", last modified: Thu Apr  4 11:25:13 2024, max compression
```

## Comparing `backend.ai-krunner-static-gnu-4.2.0.tar` & `backend.ai-krunner-static-gnu-4.2.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:06:53.334425 backend.ai-krunner-static-gnu-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-04-04 12:06:53.334425 backend.ai-krunner-static-gnu-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-04 12:06:53.334425 backend.ai-krunner-static-gnu-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:06:53.330424 backend.ai-krunner-static-gnu-4.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:06:53.330424 backend.ai-krunner-static-gnu-4.2.0/src/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:06:53.330424 backend.ai-krunner-static-gnu-4.2.0/src/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:06:53.330424 backend.ai-krunner-static-gnu-4.2.0/src/ai/backend/krunner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:06:53.330424 backend.ai-krunner-static-gnu-4.2.0/src/ai/backend/krunner/static_gnu/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/src/ai/backend/krunner/static_gnu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/src/ai/backend/krunner/static_gnu/krunner-python.static-gnu.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/src/ai/backend/krunner/static_gnu/krunner-version.static-gnu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/src/ai/backend/krunner/static_gnu/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 12:06:50.000000 backend.ai-krunner-static-gnu-4.2.0/src/ai/backend/krunner/static_gnu/versions.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:06:53.334425 backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2024-04-04 12:06:53.000000 backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-04 12:06:53.000000 backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:06:53.000000 backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 12:06:53.000000 backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:06:53.000000 backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 12:06:53.000000 backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-04 12:06:53.000000 backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:25:13.904471 backend.ai-krunner-static-gnu-4.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-04-04 11:25:13.904471 backend.ai-krunner-static-gnu-4.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-04 11:25:13.904471 backend.ai-krunner-static-gnu-4.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:25:13.900471 backend.ai-krunner-static-gnu-4.2.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:25:13.900471 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:25:13.900471 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:25:13.900471 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/backend/krunner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:25:13.900471 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/backend/krunner/static_gnu/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/backend/krunner/static_gnu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/backend/krunner/static_gnu/krunner-python.static-gnu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/backend/krunner/static_gnu/krunner-version.static-gnu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/backend/krunner/static_gnu/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 11:25:11.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/ai/backend/krunner/static_gnu/versions.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:25:13.904471 backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-04-04 11:25:13.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-04 11:25:13.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:25:13.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 11:25:13.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:25:13.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 11:25:13.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-04 11:25:13.000000 backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/top_level.txt
```

### Comparing `backend.ai-krunner-static-gnu-4.2.0/LICENSE` & `backend.ai-krunner-static-gnu-4.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-static-gnu-4.2.0/PKG-INFO` & `backend.ai-krunner-static-gnu-4.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-krunner-static-gnu
-Version: 4.2.0
+Version: 4.2.0rc1
 Summary: Backend.AI Kernel Runner based on GNU libc
 Home-page: https://backend.ai
 Author: Lablup Inc.
 Author-email: devops@lablup.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `backend.ai-krunner-static-gnu-4.2.0/README.md` & `backend.ai-krunner-static-gnu-4.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-static-gnu-4.2.0/setup.cfg` & `backend.ai-krunner-static-gnu-4.2.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/PKG-INFO` & `backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-krunner-static-gnu
-Version: 4.2.0
+Version: 4.2.0rc1
 Summary: Backend.AI Kernel Runner based on GNU libc
 Home-page: https://backend.ai
 Author: Lablup Inc.
 Author-email: devops@lablup.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `backend.ai-krunner-static-gnu-4.2.0/src/backend.ai_krunner_static_gnu.egg-info/SOURCES.txt` & `backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

