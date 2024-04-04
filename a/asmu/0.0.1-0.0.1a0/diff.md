# Comparing `tmp/asmu-0.0.1.tar.gz` & `tmp/asmu-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmu-0.0.1.tar", last modified: Thu Apr  4 11:26:54 2024, max compression
+gzip compressed data, was "asmu-0.0.1a0.tar", last modified: Thu Apr  4 12:03:48 2024, max compression
```

## Comparing `asmu-0.0.1.tar` & `asmu-0.0.1a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 11:26:54.736963 asmu-0.0.1/
--rw-rw-rw-   0        0        0    35821 2024-04-04 08:35:45.000000 asmu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      691 2024-04-04 11:26:54.732923 asmu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       39 2024-04-04 11:24:23.000000 asmu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 11:26:54.655768 asmu-0.0.1/asmu/
--rw-rw-rw-   0        0        0      479 2024-04-04 09:04:11.000000 asmu-0.0.1/asmu/__init__.py
--rw-rw-rw-   0        0        0     1975 2024-04-04 08:51:58.000000 asmu-0.0.1/asmu/analysis.py
--rw-rw-rw-   0        0        0     5103 2024-04-04 08:51:56.000000 asmu-0.0.1/asmu/generator.py
--rw-rw-rw-   0        0        0     1893 2024-04-04 08:51:54.000000 asmu-0.0.1/asmu/inout.py
--rw-rw-rw-   0        0        0     3685 2024-04-04 08:51:53.000000 asmu-0.0.1/asmu/interface.py
--rw-rw-rw-   0        0        0     6361 2024-04-04 11:23:17.000000 asmu-0.0.1/asmu/recording.py
--rw-rw-rw-   0        0        0     2145 2024-04-04 11:23:15.000000 asmu-0.0.1/asmu/setup.py
--rw-rw-rw-   0        0        0     4249 2024-04-04 08:51:45.000000 asmu-0.0.1/asmu/view.py
-drwxrwxrwx   0        0        0        0 2024-04-04 11:26:54.729223 asmu-0.0.1/asmu.egg-info/
--rw-rw-rw-   0        0        0      691 2024-04-04 11:26:54.000000 asmu-0.0.1/asmu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-04-04 11:26:54.000000 asmu-0.0.1/asmu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 11:26:54.000000 asmu-0.0.1/asmu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-04 11:26:54.000000 asmu-0.0.1/asmu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-04 11:26:54.000000 asmu-0.0.1/asmu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      761 2024-04-04 11:24:26.000000 asmu-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 11:26:54.737963 asmu-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 12:03:48.920809 asmu-0.0.1a0/
+-rw-rw-rw-   0        0        0    35821 2024-04-04 08:35:45.000000 asmu-0.0.1a0/LICENSE
+-rw-rw-rw-   0        0        0     1654 2024-04-04 12:03:48.917820 asmu-0.0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0      957 2024-04-04 11:47:53.000000 asmu-0.0.1a0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 12:03:48.870078 asmu-0.0.1a0/asmu/
+-rw-rw-rw-   0        0        0      479 2024-04-04 09:04:11.000000 asmu-0.0.1a0/asmu/__init__.py
+-rw-rw-rw-   0        0        0     1975 2024-04-04 08:51:58.000000 asmu-0.0.1a0/asmu/analysis.py
+-rw-rw-rw-   0        0        0     5103 2024-04-04 08:51:56.000000 asmu-0.0.1a0/asmu/generator.py
+-rw-rw-rw-   0        0        0     1893 2024-04-04 08:51:54.000000 asmu-0.0.1a0/asmu/inout.py
+-rw-rw-rw-   0        0        0     3685 2024-04-04 08:51:53.000000 asmu-0.0.1a0/asmu/interface.py
+-rw-rw-rw-   0        0        0     6361 2024-04-04 11:23:17.000000 asmu-0.0.1a0/asmu/recording.py
+-rw-rw-rw-   0        0        0     2145 2024-04-04 11:23:15.000000 asmu-0.0.1a0/asmu/setup.py
+-rw-rw-rw-   0        0        0     4249 2024-04-04 08:51:45.000000 asmu-0.0.1a0/asmu/view.py
+drwxrwxrwx   0        0        0        0 2024-04-04 12:03:48.915743 asmu-0.0.1a0/asmu.egg-info/
+-rw-rw-rw-   0        0        0     1654 2024-04-04 12:03:48.000000 asmu-0.0.1a0/asmu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-04 12:03:48.000000 asmu-0.0.1a0/asmu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 12:03:48.000000 asmu-0.0.1a0/asmu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-04 12:03:48.000000 asmu-0.0.1a0/asmu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-04 12:03:48.000000 asmu-0.0.1a0/asmu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      765 2024-04-04 12:03:08.000000 asmu-0.0.1a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-04 12:03:48.920809 asmu-0.0.1a0/setup.cfg
```

### Comparing `asmu-0.0.1/LICENSE` & `asmu-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1/asmu/analysis.py` & `asmu-0.0.1a0/asmu/analysis.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1/asmu/generator.py` & `asmu-0.0.1a0/asmu/generator.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1/asmu/inout.py` & `asmu-0.0.1a0/asmu/inout.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1/asmu/interface.py` & `asmu-0.0.1a0/asmu/interface.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1/asmu/recording.py` & `asmu-0.0.1a0/asmu/recording.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1/asmu/setup.py` & `asmu-0.0.1a0/asmu/setup.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1/asmu/view.py` & `asmu-0.0.1a0/asmu/view.py`

 * *Files identical despite different names*

### Comparing `asmu-0.0.1/pyproject.toml` & `asmu-0.0.1a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=69.2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asmu"
-version = "0.0.1"
+version = "0.0.1a"
 authors = [
     {name = "felhub", email = "felhub@net4us.at"},
 ]
 description = "Acoustic Signal Measurement Utilities"
-readme = "REAMDME.md"
+readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Multimedia :: Sound/Audio"
@@ -22,8 +22,8 @@
     "numpy>=1.26.4",
     "scipy>=1.13.0",
     "sounddevice>=0.4.6",
     "soundfile>=0.12.1"
 ]
 
 [project.urls]
-Homepage = "https://github.com/felhub/asmu"
+Repository = "https://github.com/felhub/asmu"
```

