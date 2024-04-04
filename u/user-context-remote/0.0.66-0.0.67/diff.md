# Comparing `tmp/user-context-remote-0.0.66.tar.gz` & `tmp/user-context-remote-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-context-remote-0.0.66.tar", last modified: Mon Apr  1 19:58:19 2024, max compression
+gzip compressed data, was "user-context-remote-0.0.67.tar", last modified: Thu Apr  4 21:02:29 2024, max compression
```

## Comparing `user-context-remote-0.0.66.tar` & `user-context-remote-0.0.67.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:19.990881 user-context-remote-0.0.66/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-01 19:58:07.000000 user-context-remote-0.0.66/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 19:58:19.994881 user-context-remote-0.0.66/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 19:58:19.000000 user-context-remote-0.0.66/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:29.686457 user-context-remote-0.0.67/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 21:02:29.686457 user-context-remote-0.0.67/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-04 21:02:18.000000 user-context-remote-0.0.67/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-04 21:02:18.000000 user-context-remote-0.0.67/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:02:29.686457 user-context-remote-0.0.67/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-04 21:02:18.000000 user-context-remote-0.0.67/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:29.682457 user-context-remote-0.0.67/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:29.682457 user-context-remote-0.0.67/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:18.000000 user-context-remote-0.0.67/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-04 21:02:18.000000 user-context-remote-0.0.67/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:02:29.686457 user-context-remote-0.0.67/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 21:02:29.000000 user-context-remote-0.0.67/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-04 21:02:29.000000 user-context-remote-0.0.67/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:02:29.000000 user-context-remote-0.0.67/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 21:02:29.000000 user-context-remote-0.0.67/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 21:02:29.000000 user-context-remote-0.0.67/user_context_remote.egg-info/top_level.txt
```

### Comparing `user-context-remote-0.0.66/PKG-INFO` & `user-context-remote-0.0.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.66
+Version: 0.0.67
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `user-context-remote-0.0.66/README.md` & `user-context-remote-0.0.67/README.md`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.66/pyproject.toml` & `user-context-remote-0.0.67/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.66/setup.py` & `user-context-remote-0.0.67/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.66',  # https://pypi.org/project/user-context-remote/
+    version='0.0.67',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `user-context-remote-0.0.66/user_context_remote/src/user_context.py` & `user-context-remote-0.0.67/user_context_remote/src/user_context.py`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.66/user_context_remote.egg-info/PKG-INFO` & `user-context-remote-0.0.67/user_context_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.66
+Version: 0.0.67
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

