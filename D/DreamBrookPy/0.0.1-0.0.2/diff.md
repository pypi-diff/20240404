# Comparing `tmp/DreamBrookPy-0.0.1.tar.gz` & `tmp/DreamBrookPy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DreamBrookPy-0.0.1.tar", last modified: Tue Feb 20 09:08:33 2024, max compression
+gzip compressed data, was "DreamBrookPy-0.0.2.tar", last modified: Thu Apr  4 04:56:22 2024, max compression
```

## Comparing `DreamBrookPy-0.0.1.tar` & `DreamBrookPy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-20 09:08:33.199161 DreamBrookPy-0.0.1/
-drwxrwxr-x   0 root         (0) root         (0)        0 2024-02-20 09:08:33.195161 DreamBrookPy-0.0.1/DreamBrookPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)      645 2024-02-20 09:08:33.000000 DreamBrookPy-0.0.1/DreamBrookPy.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      185 2024-02-20 09:08:33.000000 DreamBrookPy-0.0.1/DreamBrookPy.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-02-20 09:08:33.000000 DreamBrookPy-0.0.1/DreamBrookPy.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-02-20 09:08:33.000000 DreamBrookPy-0.0.1/DreamBrookPy.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)    35149 2024-02-11 13:40:09.000000 DreamBrookPy-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      645 2024-02-20 09:08:33.195161 DreamBrookPy-0.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)       73 2024-02-11 13:40:09.000000 DreamBrookPy-0.0.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      560 2024-02-20 09:07:08.000000 DreamBrookPy-0.0.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2024-02-20 09:08:33.199161 DreamBrookPy-0.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      458 2024-02-11 13:46:18.000000 DreamBrookPy-0.0.1/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-04 04:56:22.400622 DreamBrookPy-0.0.2/
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-04-04 04:56:22.396622 DreamBrookPy-0.0.2/DreamBrookPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-04 04:56:22.000000 DreamBrookPy-0.0.2/DreamBrookPy.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      185 2024-04-04 04:56:22.000000 DreamBrookPy-0.0.2/DreamBrookPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-04 04:56:22.000000 DreamBrookPy-0.0.2/DreamBrookPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-04 04:56:22.000000 DreamBrookPy-0.0.2/DreamBrookPy.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)    35149 2024-02-11 13:40:09.000000 DreamBrookPy-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-04 04:56:22.396622 DreamBrookPy-0.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       89 2024-04-04 04:56:05.000000 DreamBrookPy-0.0.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      560 2024-04-04 04:55:28.000000 DreamBrookPy-0.0.2/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2024-04-04 04:56:22.400622 DreamBrookPy-0.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      458 2024-04-04 04:50:28.000000 DreamBrookPy-0.0.2/setup.py
```

### Comparing `DreamBrookPy-0.0.1/DreamBrookPy.egg-info/PKG-INFO` & `DreamBrookPy-0.0.2/DreamBrookPy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DreamBrookPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Toolkit for DreamBrook Tech
 Home-page: https://github.com/DreamBrookTech/DreamBrookPy
 Author: DreamBrookTech
 Author-email: DreamBrook Tech Dev  <dev@dreambrook.tech>
 Project-URL: Homepage, https://docs.dreambrook.tech
 Project-URL: Issues, https://docs.dreambrook.tech
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,8 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DreamBrookPy
 Official Python Toolbox for the DreamBrook Tech Ecosystem
+Version = 0.0.2
```

### Comparing `DreamBrookPy-0.0.1/LICENSE` & `DreamBrookPy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `DreamBrookPy-0.0.1/PKG-INFO` & `DreamBrookPy-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DreamBrookPy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python Toolkit for DreamBrook Tech
 Home-page: https://github.com/DreamBrookTech/DreamBrookPy
 Author: DreamBrookTech
 Author-email: DreamBrook Tech Dev  <dev@dreambrook.tech>
 Project-URL: Homepage, https://docs.dreambrook.tech
 Project-URL: Issues, https://docs.dreambrook.tech
 Classifier: Programming Language :: Python :: 3
@@ -12,7 +12,8 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DreamBrookPy
 Official Python Toolbox for the DreamBrook Tech Ecosystem
+Version = 0.0.2
```

### Comparing `DreamBrookPy-0.0.1/pyproject.toml` & `DreamBrookPy-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "DreamBrookPy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="DreamBrook Tech Dev ", email="dev@dreambrook.tech" },
 ]
 description ="Python Toolkit for DreamBrook Tech"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

