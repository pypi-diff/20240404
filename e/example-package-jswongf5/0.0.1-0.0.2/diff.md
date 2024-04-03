# Comparing `tmp/example_package_jswongf5-0.0.1.tar.gz` & `tmp/example_package_jswongf5-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_jswongf5-0.0.1.tar", last modified: Wed Apr  3 22:37:05 2024, max compression
+gzip compressed data, was "example_package_jswongf5-0.0.2.tar", last modified: Wed Apr  3 23:17:07 2024, max compression
```

## Comparing `example_package_jswongf5-0.0.1.tar` & `example_package_jswongf5-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 22:37:05.795595 example_package_jswongf5-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-03 22:31:26.000000 example_package_jswongf5-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      681 2024-04-03 22:37:05.793613 example_package_jswongf5-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      171 2024-04-03 22:32:57.000000 example_package_jswongf5-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      580 2024-04-03 22:31:11.000000 example_package_jswongf5-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 22:37:05.795891 example_package_jswongf5-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 22:37:05.779465 example_package_jswongf5-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 22:37:05.784517 example_package_jswongf5-0.0.1/src/example_package_jswongf5/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 22:29:09.000000 example_package_jswongf5-0.0.1/src/example_package_jswongf5/__init__.py
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-03 22:29:45.000000 example_package_jswongf5-0.0.1/src/example_package_jswongf5/example.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 22:37:05.792459 example_package_jswongf5-0.0.1/src/example_package_jswongf5.egg-info/
--rw-r--r--   0 root         (0) root         (0)      681 2024-04-03 22:37:05.000000 example_package_jswongf5-0.0.1/src/example_package_jswongf5.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      321 2024-04-03 22:37:05.000000 example_package_jswongf5-0.0.1/src/example_package_jswongf5.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 22:37:05.000000 example_package_jswongf5-0.0.1/src/example_package_jswongf5.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-03 22:37:05.000000 example_package_jswongf5-0.0.1/src/example_package_jswongf5.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 23:17:07.348092 example_package_jswongf5-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1074 2024-04-03 22:31:26.000000 example_package_jswongf5-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      681 2024-04-03 23:17:07.346717 example_package_jswongf5-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      171 2024-04-03 22:32:57.000000 example_package_jswongf5-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      580 2024-04-03 23:16:51.000000 example_package_jswongf5-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 23:17:07.348560 example_package_jswongf5-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 23:17:07.328865 example_package_jswongf5-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 23:17:07.334591 example_package_jswongf5-0.0.2/src/example_package_jswongf5/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 22:29:09.000000 example_package_jswongf5-0.0.2/src/example_package_jswongf5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-03 22:29:45.000000 example_package_jswongf5-0.0.2/src/example_package_jswongf5/example.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 23:17:07.345770 example_package_jswongf5-0.0.2/src/example_package_jswongf5.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      681 2024-04-03 23:17:07.000000 example_package_jswongf5-0.0.2/src/example_package_jswongf5.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      321 2024-04-03 23:17:07.000000 example_package_jswongf5-0.0.2/src/example_package_jswongf5.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 23:17:07.000000 example_package_jswongf5-0.0.2/src/example_package_jswongf5.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-03 23:17:07.000000 example_package_jswongf5-0.0.2/src/example_package_jswongf5.egg-info/top_level.txt
```

### Comparing `example_package_jswongf5-0.0.1/LICENSE` & `example_package_jswongf5-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_jswongf5-0.0.1/PKG-INFO` & `example_package_jswongf5-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_jswongf5
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `example_package_jswongf5-0.0.1/pyproject.toml` & `example_package_jswongf5-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "example_package_jswongf5"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `example_package_jswongf5-0.0.1/src/example_package_jswongf5.egg-info/PKG-INFO` & `example_package_jswongf5-0.0.2/src/example_package_jswongf5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_jswongf5
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

