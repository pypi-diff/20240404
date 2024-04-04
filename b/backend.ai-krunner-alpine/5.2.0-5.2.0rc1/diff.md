# Comparing `tmp/backend.ai-krunner-alpine-5.2.0.tar.gz` & `tmp/backend.ai-krunner-alpine-5.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-krunner-alpine-5.2.0.tar", last modified: Thu Apr  4 12:08:13 2024, max compression
+gzip compressed data, was "backend.ai-krunner-alpine-5.2.0rc1.tar", last modified: Thu Apr  4 11:59:59 2024, max compression
```

## Comparing `backend.ai-krunner-alpine-5.2.0.tar` & `backend.ai-krunner-alpine-5.2.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:08:13.254665 backend.ai-krunner-alpine-5.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-04 12:08:13.254665 backend.ai-krunner-alpine-5.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-04 12:08:13.254665 backend.ai-krunner-alpine-5.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:08:13.242665 backend.ai-krunner-alpine-5.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:08:13.242665 backend.ai-krunner-alpine-5.2.0/src/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:08:13.242665 backend.ai-krunner-alpine-5.2.0/src/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:08:13.242665 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:08:13.250665 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/krunner-env.musllinux_1_2.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/krunner-python.musllinux_1_2.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/krunner-python.musllinux_1_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/krunner-version.musllinux_1_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/krunner-wheels.musllinux_1_2.dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)  1163360 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/ttyd_linux.aarch64.bin
--rwxr-xr-x   0 runner    (1001) docker     (127)  1155360 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/ttyd_linux.x86_64.bin
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 12:08:06.000000 backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/versions.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:08:13.250665 backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-04 12:08:13.000000 backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-04 12:08:13.000000 backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:08:13.000000 backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-04 12:08:13.000000 backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:08:13.000000 backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 12:08:13.000000 backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-04 12:08:13.000000 backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:59:59.481243 backend.ai-krunner-alpine-5.2.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-04 11:59:59.481243 backend.ai-krunner-alpine-5.2.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-04 11:59:59.481243 backend.ai-krunner-alpine-5.2.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:59:59.473242 backend.ai-krunner-alpine-5.2.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:59:59.473242 backend.ai-krunner-alpine-5.2.0rc1/src/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:59:59.473242 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:59:59.473242 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:59:59.477242 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/krunner-env.musllinux_1_2.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/krunner-python.musllinux_1_2.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/krunner-python.musllinux_1_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/krunner-version.musllinux_1_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/krunner-wheels.musllinux_1_2.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1163360 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/ttyd_linux.aarch64.bin
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1155360 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/ttyd_linux.x86_64.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 11:59:56.000000 backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/versions.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:59:59.481243 backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-04 11:59:59.000000 backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-04 11:59:59.000000 backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:59:59.000000 backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-04 11:59:59.000000 backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:59:59.000000 backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 11:59:59.000000 backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-04 11:59:59.000000 backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/top_level.txt
```

### Comparing `backend.ai-krunner-alpine-5.2.0/LICENSE` & `backend.ai-krunner-alpine-5.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-alpine-5.2.0/PKG-INFO` & `backend.ai-krunner-alpine-5.2.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-krunner-alpine
-Version: 5.2.0
+Version: 5.2.0rc1
 Summary: Backend.AI Kernel Runner for Alpine
 Home-page: https://backend.ai
 Author: Lablup Inc.
 Author-email: devops@lablup.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `backend.ai-krunner-alpine-5.2.0/README.md` & `backend.ai-krunner-alpine-5.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-alpine-5.2.0/setup.cfg` & `backend.ai-krunner-alpine-5.2.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/krunner-env.musllinux_1_2.dockerfile` & `backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/krunner-env.musllinux_1_2.dockerfile`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/krunner-python.musllinux_1_2.dockerfile` & `backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/krunner-python.musllinux_1_2.dockerfile`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/ttyd_linux.aarch64.bin` & `backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/ttyd_linux.aarch64.bin`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-alpine-5.2.0/src/ai/backend/krunner/alpine/ttyd_linux.x86_64.bin` & `backend.ai-krunner-alpine-5.2.0rc1/src/ai/backend/krunner/alpine/ttyd_linux.x86_64.bin`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/PKG-INFO` & `backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-krunner-alpine
-Version: 5.2.0
+Version: 5.2.0rc1
 Summary: Backend.AI Kernel Runner for Alpine
 Home-page: https://backend.ai
 Author: Lablup Inc.
 Author-email: devops@lablup.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `backend.ai-krunner-alpine-5.2.0/src/backend.ai_krunner_alpine.egg-info/SOURCES.txt` & `backend.ai-krunner-alpine-5.2.0rc1/src/backend.ai_krunner_alpine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

