# Comparing `tmp/lockhart-serial-0.0.1.tar.gz` & `tmp/lockhart-serial-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockhart-serial-0.0.1.tar", last modified: Wed Feb 28 22:02:40 2024, max compression
+gzip compressed data, was "lockhart-serial-1.0.0.tar", last modified: Wed Apr  3 23:19:50 2024, max compression
```

## Comparing `lockhart-serial-0.0.1.tar` & `lockhart-serial-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 22:02:40.373039 lockhart-serial-0.0.1/
--rw-rw-rw-   0        0        0      510 2024-02-28 22:02:40.372066 lockhart-serial-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-28 21:58:53.000000 lockhart-serial-0.0.1/README.md
--rw-rw-rw-   0        0        0      611 2024-02-28 22:02:34.000000 lockhart-serial-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-28 22:02:40.373039 lockhart-serial-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-28 22:02:40.356036 lockhart-serial-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-28 22:02:40.359036 lockhart-serial-0.0.1/src/lockhart-serial/
--rw-rw-rw-   0        0        0        0 2024-02-28 21:55:36.000000 lockhart-serial-0.0.1/src/lockhart-serial/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-28 21:56:01.000000 lockhart-serial-0.0.1/src/lockhart-serial/lockhart_serial.py
-drwxrwxrwx   0        0        0        0 2024-02-28 22:02:40.371039 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/
--rw-rw-rw-   0        0        0      510 2024-02-28 22:02:40.000000 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-02-28 22:02:40.000000 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 22:02:40.000000 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-28 22:02:40.000000 lockhart-serial-0.0.1/src/lockhart_serial.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:19:50.586606 lockhart-serial-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 23:19:46.000000 lockhart-serial-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-03 23:19:50.586606 lockhart-serial-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:19:46.000000 lockhart-serial-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:19:50.582606 lockhart-serial-1.0.0/lockhart_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:19:50.000000 lockhart-serial-1.0.0/lockhart_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-03 23:19:46.000000 lockhart-serial-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:19:50.586606 lockhart-serial-1.0.0/setup.cfg
```

### Comparing `lockhart-serial-0.0.1/pyproject.toml` & `lockhart-serial-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,14 @@
-[project]
-name = "lockhart-serial"
-version = "0.0.1"
-authors = [
-  { name="NinjaBunny", email="xxninjabunnyxx@gmail.com" },
-]
-description = "Serial communication for Lockhart devices"
-readme = "README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-Homepage = "https://github.com/pypa/sampleproject"
-Issues = "https://github.com/pypa/sampleproject/issues"
-
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+Metadata-Version: 2.1
+Name: lockhart-serial
+Version: 1.0.0
+Summary: Serial communication for Lockhart devices
+Author-email: NinjaBunny <xxninjabunnyxx@gmail.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Issues, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyserial
```

