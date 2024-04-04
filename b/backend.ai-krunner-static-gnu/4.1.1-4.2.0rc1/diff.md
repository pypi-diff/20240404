# Comparing `tmp/backend.ai-krunner-static-gnu-4.1.1.tar.gz` & `tmp/backend.ai-krunner-static-gnu-4.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-krunner-static-gnu-4.1.1.tar", last modified: Sat Feb  3 14:56:43 2024, max compression
+gzip compressed data, was "backend.ai-krunner-static-gnu-4.2.0rc1.tar", last modified: Thu Apr  4 11:25:13 2024, max compression
```

## Comparing `backend.ai-krunner-static-gnu-4.1.1.tar` & `backend.ai-krunner-static-gnu-4.2.0rc1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/src/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/src/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/src/ai/backend/krunner/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/src/ai/backend/krunner/static_gnu/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/src/ai/backend/krunner/static_gnu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/src/ai/backend/krunner/static_gnu/krunner-python.static-gnu.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/src/ai/backend/krunner/static_gnu/krunner-version.static-gnu.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/src/ai/backend/krunner/static_gnu/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-03 14:56:40.000000 backend.ai-krunner-static-gnu-4.1.1/src/ai/backend/krunner/static_gnu/versions.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 14:56:43.399797 backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-02-03 14:56:43.000000 backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-03 14:56:43.000000 backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 14:56:43.000000 backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-03 14:56:43.000000 backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 14:56:43.000000 backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-03 14:56:43.000000 backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-03 14:56:43.000000 backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/top_level.txt
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

### Comparing `backend.ai-krunner-static-gnu-4.1.1/LICENSE` & `backend.ai-krunner-static-gnu-4.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-static-gnu-4.1.1/PKG-INFO` & `backend.ai-krunner-static-gnu-4.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-krunner-static-gnu
-Version: 4.1.1
+Version: 4.2.0rc1
 Summary: Backend.AI Kernel Runner based on GNU libc
 Home-page: https://backend.ai
 Author: Lablup Inc.
 Author-email: devops@lablup.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -62,18 +62,19 @@
   package names and paths. (e.g., `static_gnu`, `alpine`)
 
 ## Development
 
 ```console
 $ git clone https://github.com/lablup/backend.ai-krunner-{distro} krunner-{distro}
 $ cd krunner-{distro}
-$ pyenv virtualenv 3.11.2 venv-krunner  # you may share the same venv with other krunner projects
+$ pyenv virtualenv 3.12.2 venv-krunner  # you may share the same venv with other krunner projects
 $ pyenv local venv-krunner
 $ pip install -U pip setuptools
-$ pip install -U click -e .
+$ pip install -U -r build/requirements.txt
+$ pip install -U -e .
 ```
 
 ## How to update
 
 1. Modify Dockerfile and/or other contents.
   - To update the Python version, update `src/ai/backend/krunner/{distro_}/krunner-python.{distro}.txt`
     and the dockerfiles (both python and wheels) accordingly, including the
```

### Comparing `backend.ai-krunner-static-gnu-4.1.1/README.md` & `backend.ai-krunner-static-gnu-4.2.0rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,18 +41,19 @@
   package names and paths. (e.g., `static_gnu`, `alpine`)
 
 ## Development
 
 ```console
 $ git clone https://github.com/lablup/backend.ai-krunner-{distro} krunner-{distro}
 $ cd krunner-{distro}
-$ pyenv virtualenv 3.11.2 venv-krunner  # you may share the same venv with other krunner projects
+$ pyenv virtualenv 3.12.2 venv-krunner  # you may share the same venv with other krunner projects
 $ pyenv local venv-krunner
 $ pip install -U pip setuptools
-$ pip install -U click -e .
+$ pip install -U -r build/requirements.txt
+$ pip install -U -e .
 ```
 
 ## How to update
 
 1. Modify Dockerfile and/or other contents.
   - To update the Python version, update `src/ai/backend/krunner/{distro_}/krunner-python.{distro}.txt`
     and the dockerfiles (both python and wheels) accordingly, including the
```

### Comparing `backend.ai-krunner-static-gnu-4.1.1/setup.cfg` & `backend.ai-krunner-static-gnu-4.2.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/PKG-INFO` & `backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-krunner-static-gnu
-Version: 4.1.1
+Version: 4.2.0rc1
 Summary: Backend.AI Kernel Runner based on GNU libc
 Home-page: https://backend.ai
 Author: Lablup Inc.
 Author-email: devops@lablup.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -62,18 +62,19 @@
   package names and paths. (e.g., `static_gnu`, `alpine`)
 
 ## Development
 
 ```console
 $ git clone https://github.com/lablup/backend.ai-krunner-{distro} krunner-{distro}
 $ cd krunner-{distro}
-$ pyenv virtualenv 3.11.2 venv-krunner  # you may share the same venv with other krunner projects
+$ pyenv virtualenv 3.12.2 venv-krunner  # you may share the same venv with other krunner projects
 $ pyenv local venv-krunner
 $ pip install -U pip setuptools
-$ pip install -U click -e .
+$ pip install -U -r build/requirements.txt
+$ pip install -U -e .
 ```
 
 ## How to update
 
 1. Modify Dockerfile and/or other contents.
   - To update the Python version, update `src/ai/backend/krunner/{distro_}/krunner-python.{distro}.txt`
     and the dockerfiles (both python and wheels) accordingly, including the
```

### Comparing `backend.ai-krunner-static-gnu-4.1.1/src/backend.ai_krunner_static_gnu.egg-info/SOURCES.txt` & `backend.ai-krunner-static-gnu-4.2.0rc1/src/backend.ai_krunner_static_gnu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

