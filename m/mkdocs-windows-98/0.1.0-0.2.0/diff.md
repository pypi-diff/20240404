# Comparing `tmp/mkdocs-windows-98-0.1.0.tar.gz` & `tmp/mkdocs-windows-98-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-windows-98-0.1.0.tar", last modified: Wed Apr  3 16:31:10 2024, max compression
+gzip compressed data, was "mkdocs-windows-98-0.2.0.tar", last modified: Thu Apr  4 10:48:52 2024, max compression
```

## Comparing `mkdocs-windows-98-0.1.0.tar` & `mkdocs-windows-98-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:10.871918 mkdocs-windows-98-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-03 16:30:58.000000 mkdocs-windows-98-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-03 16:31:10.871918 mkdocs-windows-98-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-03 16:30:58.000000 mkdocs-windows-98-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-03 16:30:58.000000 mkdocs-windows-98-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:31:10.871918 mkdocs-windows-98-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:10.871918 mkdocs-windows-98-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:10.871918 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:58.000000 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:10.871918 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-03 16:31:10.000000 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 16:31:10.000000 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:31:10.000000 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 16:31:10.000000 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 16:31:10.000000 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 16:31:10.000000 mkdocs-windows-98-0.1.0/src/mkdocs_windows_98.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:48:52.161441 mkdocs-windows-98-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 10:48:42.000000 mkdocs-windows-98-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-04 10:48:52.161441 mkdocs-windows-98-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-04 10:48:42.000000 mkdocs-windows-98-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-04 10:48:42.000000 mkdocs-windows-98-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 10:48:52.161441 mkdocs-windows-98-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:48:52.161441 mkdocs-windows-98-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:48:52.161441 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:48:42.000000 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:48:52.161441 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-04 10:48:52.000000 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-04 10:48:52.000000 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:48:52.000000 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 10:48:52.000000 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 10:48:52.000000 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 10:48:52.000000 mkdocs-windows-98-0.2.0/src/mkdocs_windows_98.egg-info/top_level.txt
```

### Comparing `mkdocs-windows-98-0.1.0/LICENSE` & `mkdocs-windows-98-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-windows-98-0.1.0/PKG-INFO` & `mkdocs-windows-98-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-windows-98
-Version: 0.1.0
+Version: 0.2.0
 Summary: Windows 98 MkDocs Theme
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `mkdocs-windows-98-0.1.0/README.md` & `mkdocs-windows-98-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-windows-98-0.1.0/pyproject.toml` & `mkdocs-windows-98-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-windows-98"
-version = "0.1.0"
+version = "0.2.0"
 description = "Windows 98 MkDocs Theme"
 readme = "README.md"
 authors = [
   {name = "Useless DevLab", email = "useless.devlab@gmail.com"}
 ]
 requires-python = ">=3.9"
```

### Comparing `mkdocs-windows-98-0.1.0/src/mkdocs_windows_98.egg-info/PKG-INFO` & `mkdocs-windows-98-0.2.0/src/mkdocs_windows_98.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-windows-98
-Version: 0.1.0
+Version: 0.2.0
 Summary: Windows 98 MkDocs Theme
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

