# Comparing `tmp/curlquest-0.0.3.tar.gz` & `tmp/curlquest-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curlquest-0.0.3.tar", max compression
+gzip compressed data, was "curlquest-0.1.0.tar", max compression
```

## Comparing `curlquest-0.0.3.tar` & `curlquest-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2024-04-04 02:38:00.275545 curlquest-0.0.3/LICENSE
--rw-r--r--   0        0        0     4574 2024-04-04 02:38:00.275545 curlquest-0.0.3/README.md
--rw-r--r--   0        0        0      204 2024-04-04 02:38:00.278878 curlquest-0.0.3/curlquest/__init__.py
--rw-r--r--   0        0        0     2633 2024-04-04 02:38:00.278878 curlquest-0.0.3/curlquest/defaults.py
--rw-r--r--   0        0        0     1167 2024-04-04 02:38:00.278878 curlquest-0.0.3/curlquest/dict.py
--rw-r--r--   0        0        0     1765 2024-04-04 02:38:00.278878 curlquest-0.0.3/curlquest/helper.py
--rw-r--r--   0        0        0     6065 2024-04-04 02:44:00.134121 curlquest-0.0.3/curlquest/models.py
--rw-r--r--   0        0        0     9034 2024-04-04 02:42:56.525790 curlquest-0.0.3/curlquest/sessions.py
--rw-r--r--   0        0        0      822 2024-04-04 02:45:58.078169 curlquest-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5677 1970-01-01 00:00:00.000000 curlquest-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-04 02:38:00.275545 curlquest-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4574 2024-04-04 02:38:00.275545 curlquest-0.1.0/README.md
+-rw-r--r--   0        0        0      204 2024-04-04 02:38:00.278878 curlquest-0.1.0/curlquest/__init__.py
+-rw-r--r--   0        0        0     2633 2024-04-04 02:38:00.278878 curlquest-0.1.0/curlquest/defaults.py
+-rw-r--r--   0        0        0     1167 2024-04-04 02:38:00.278878 curlquest-0.1.0/curlquest/dict.py
+-rw-r--r--   0        0        0     1765 2024-04-04 02:38:00.278878 curlquest-0.1.0/curlquest/helper.py
+-rw-r--r--   0        0        0     6065 2024-04-04 02:44:00.134121 curlquest-0.1.0/curlquest/models.py
+-rw-r--r--   0        0        0     9034 2024-04-04 02:42:56.525790 curlquest-0.1.0/curlquest/sessions.py
+-rw-r--r--   0        0        0      864 2024-04-04 02:56:08.380505 curlquest-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 curlquest-0.1.0/PKG-INFO
```

### Comparing `curlquest-0.0.3/LICENSE` & `curlquest-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `curlquest-0.0.3/README.md` & `curlquest-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `curlquest-0.0.3/curlquest/defaults.py` & `curlquest-0.1.0/curlquest/defaults.py`

 * *Files identical despite different names*

### Comparing `curlquest-0.0.3/curlquest/dict.py` & `curlquest-0.1.0/curlquest/dict.py`

 * *Files identical despite different names*

### Comparing `curlquest-0.0.3/curlquest/helper.py` & `curlquest-0.1.0/curlquest/helper.py`

 * *Files identical despite different names*

### Comparing `curlquest-0.0.3/curlquest/models.py` & `curlquest-0.1.0/curlquest/models.py`

 * *Files identical despite different names*

### Comparing `curlquest-0.0.3/curlquest/sessions.py` & `curlquest-0.1.0/curlquest/sessions.py`

 * *Files identical despite different names*

### Comparing `curlquest-0.0.3/pyproject.toml` & `curlquest-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "curlquest"
-version = "0.0.3"
-description = "A user-friendly wrapper for pycurl that simplifies HTTP requests"
+version = "0.1.0"
+description = "A user-friendly wrapper for pycurl that simplifies HTTP requests (fork of curl_request with a few changes)"
 authors = [
     "Mauritz Uphoff <mauritz.uphoff@hs-osnabrueck.de>",
     "Ennis Blank <Ennis.Blank@fau.de>",
 ]
 readme = "README.md"
 license = "MIT"
 maintainers = ["Mauritz Uphoff", "Ennis Blank"]
```

### Comparing `curlquest-0.0.3/PKG-INFO` & `curlquest-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: curlquest
-Version: 0.0.3
-Summary: A user-friendly wrapper for pycurl that simplifies HTTP requests
+Version: 0.1.0
+Summary: A user-friendly wrapper for pycurl that simplifies HTTP requests (fork of curl_request with a few changes)
 Home-page: https://github.com/Notifysolutions/request_curl
 License: MIT
 Author: Mauritz Uphoff
 Author-email: mauritz.uphoff@hs-osnabrueck.de
 Maintainer: Mauritz Uphoff
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

