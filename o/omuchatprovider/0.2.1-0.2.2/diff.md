# Comparing `tmp/omuchatprovider-0.2.1.tar.gz` & `tmp/omuchatprovider-0.2.2.tar.gz`

## Comparing `omuchatprovider-0.2.1.tar` & `omuchatprovider-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/.python-version
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/run.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/.vscode/launch.json
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/.vscode/settings.json
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/__main__.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/chatprovider.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/errors.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/helper.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/services/__init__.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/services/service.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/services/youtube/__init__.py
--rw-r--r--   0        0        0    29120 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/services/youtube/youtube.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/services/youtube/types/__init__.py
--rw-r--r--   0        0        0    14367 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/services/youtube/types/api.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/tasks/__init__.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/src/omuchatprovider/tasks/taskprofiler.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/.python-version
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/run.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/.vscode/launch.json
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/__main__.py
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/chatprovider.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/errors.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/helper.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/services/__init__.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/services/service.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/services/youtube/__init__.py
+-rw-r--r--   0        0        0    29120 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/services/youtube/youtube.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/services/youtube/types/__init__.py
+-rw-r--r--   0        0        0    14367 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/services/youtube/types/api.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/tasks/__init__.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/src/omuchatprovider/tasks/taskprofiler.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.2.2/PKG-INFO
```

### Comparing `omuchatprovider-0.2.1/src/omuchatprovider/chatprovider.py` & `omuchatprovider-0.2.2/src/omuchatprovider/chatprovider.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.1/src/omuchatprovider/helper.py` & `omuchatprovider-0.2.2/src/omuchatprovider/helper.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.1/src/omuchatprovider/services/service.py` & `omuchatprovider-0.2.2/src/omuchatprovider/services/service.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.1/src/omuchatprovider/services/youtube/youtube.py` & `omuchatprovider-0.2.2/src/omuchatprovider/services/youtube/youtube.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.1/src/omuchatprovider/services/youtube/types/api.py` & `omuchatprovider-0.2.2/src/omuchatprovider/services/youtube/types/api.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.1/src/omuchatprovider/tasks/taskprofiler.py` & `omuchatprovider-0.2.2/src/omuchatprovider/tasks/taskprofiler.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.1/pyproject.toml` & `omuchatprovider-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuchatprovider"
-version = "0.2.1"
+version = "0.2.2"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "aiohttp>=3.9.1",
     "beautifulsoup4>=4.12.2",
```

