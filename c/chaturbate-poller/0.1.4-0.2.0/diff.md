# Comparing `tmp/chaturbate_poller-0.1.4.tar.gz` & `tmp/chaturbate_poller-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaturbate_poller-0.1.4.tar", max compression
+gzip compressed data, was "chaturbate_poller-0.2.0.tar", max compression
```

## Comparing `chaturbate_poller-0.1.4.tar` & `chaturbate_poller-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2024-04-03 00:32:31.464864 chaturbate_poller-0.1.4/LICENSE
--rw-r--r--   0        0        0     2251 2024-04-03 00:32:31.464864 chaturbate_poller-0.1.4/README.md
--rw-r--r--   0        0        0     3080 2024-04-03 00:32:44.356931 chaturbate_poller-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      818 2024-04-03 00:32:31.468864 chaturbate_poller-0.1.4/src/chaturbate_poller/__init__.py
--rw-r--r--   0        0        0     1572 2024-04-03 00:32:31.468864 chaturbate_poller-0.1.4/src/chaturbate_poller/__main__.py
--rw-r--r--   0        0        0     4272 2024-04-03 00:32:31.468864 chaturbate_poller-0.1.4/src/chaturbate_poller/chaturbate_poller.py
--rw-r--r--   0        0        0      724 2024-04-03 00:32:31.468864 chaturbate_poller-0.1.4/src/chaturbate_poller/constants.py
--rw-r--r--   0        0        0     1429 2024-04-03 00:32:31.468864 chaturbate_poller-0.1.4/src/chaturbate_poller/logging_config.py
--rw-r--r--   0        0        0     3480 2024-04-03 00:32:31.468864 chaturbate_poller-0.1.4/src/chaturbate_poller/models.py
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 chaturbate_poller-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2251 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/README.md
+-rw-r--r--   0        0        0     3080 2024-04-04 01:21:00.383548 chaturbate_poller-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      818 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/__init__.py
+-rw-r--r--   0        0        0     1572 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/__main__.py
+-rw-r--r--   0        0        0     2800 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/chaturbate_poller.py
+-rw-r--r--   0        0        0      724 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/constants.py
+-rw-r--r--   0        0        0     1429 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/logging_config.py
+-rw-r--r--   0        0        0     3480 2024-04-04 01:20:43.291489 chaturbate_poller-0.2.0/src/chaturbate_poller/models.py
+-rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 chaturbate_poller-0.2.0/PKG-INFO
```

### Comparing `chaturbate_poller-0.1.4/LICENSE` & `chaturbate_poller-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.4/README.md` & `chaturbate_poller-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.4/pyproject.toml` & `chaturbate_poller-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chaturbate-poller"
-version = "0.1.4"
+version = "0.2.0"
 description = "Poller for the Chaturbate events API."
 authors = ["MountainGod2"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/MountainGod2/chaturbate_poller"
 documentation = "https://mountaingod2.github.io/chaturbate_poller/"
```

### Comparing `chaturbate_poller-0.1.4/src/chaturbate_poller/__init__.py` & `chaturbate_poller-0.2.0/src/chaturbate_poller/__init__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.4/src/chaturbate_poller/__main__.py` & `chaturbate_poller-0.2.0/src/chaturbate_poller/__main__.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.4/src/chaturbate_poller/constants.py` & `chaturbate_poller-0.2.0/src/chaturbate_poller/constants.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.4/src/chaturbate_poller/logging_config.py` & `chaturbate_poller-0.2.0/src/chaturbate_poller/logging_config.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.4/src/chaturbate_poller/models.py` & `chaturbate_poller-0.2.0/src/chaturbate_poller/models.py`

 * *Files identical despite different names*

### Comparing `chaturbate_poller-0.1.4/PKG-INFO` & `chaturbate_poller-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chaturbate-poller
-Version: 0.1.4
+Version: 0.2.0
 Summary: Poller for the Chaturbate events API.
 Home-page: https://github.com/MountainGod2/chaturbate_poller
 License: MIT
 Author: MountainGod2
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

