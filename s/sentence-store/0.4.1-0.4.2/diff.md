# Comparing `tmp/sentence_store-0.4.1.tar.gz` & `tmp/sentence_store-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentence_store-0.4.1.tar", last modified: Thu Apr  4 03:27:50 2024, max compression
+gzip compressed data, was "sentence_store-0.4.2.tar", last modified: Thu Apr  4 03:36:44 2024, max compression
```

## Comparing `sentence_store-0.4.1.tar` & `sentence_store-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:27:50.059726 sentence_store-0.4.1/
--rw-r--r--   0 tarau      (503) staff       (20)     1067 2024-03-22 00:56:36.000000 sentence_store-0.4.1/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)      929 2024-04-04 03:27:50.059450 sentence_store-0.4.1/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)      597 2024-03-22 02:11:02.000000 sentence_store-0.4.1/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:27:50.057275 sentence_store-0.4.1/sentence_store/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-04 03:27:31.000000 sentence_store-0.4.1/sentence_store/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     6661 2024-04-04 02:45:15.000000 sentence_store-0.4.1/sentence_store/main.py
--rw-r--r--   0 tarau      (503) staff       (20)       45 2024-03-22 21:22:17.000000 sentence_store-0.4.1/sentence_store/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1009 2024-04-04 02:08:24.000000 sentence_store-0.4.1/sentence_store/tools.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:27:50.059008 sentence_store-0.4.1/sentence_store.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)      929 2024-04-04 03:27:49.000000 sentence_store-0.4.1/sentence_store.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)      358 2024-04-04 03:27:50.000000 sentence_store-0.4.1/sentence_store.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:27:50.000000 sentence_store-0.4.1/sentence_store.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:27:50.000000 sentence_store-0.4.1/sentence_store.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       45 2024-04-04 03:27:50.000000 sentence_store-0.4.1/sentence_store.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)       15 2024-04-04 03:27:50.000000 sentence_store-0.4.1/sentence_store.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-04 03:27:50.059832 sentence_store-0.4.1/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      938 2024-03-22 02:06:24.000000 sentence_store-0.4.1/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:36:44.654421 sentence_store-0.4.2/
+-rw-r--r--   0 tarau      (503) staff       (20)     1067 2024-03-22 00:56:36.000000 sentence_store-0.4.2/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)      929 2024-04-04 03:36:44.654148 sentence_store-0.4.2/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)      597 2024-03-22 02:11:02.000000 sentence_store-0.4.2/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:36:44.652086 sentence_store-0.4.2/sentence_store/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-04 03:34:13.000000 sentence_store-0.4.2/sentence_store/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6661 2024-04-04 02:45:15.000000 sentence_store-0.4.2/sentence_store/main.py
+-rw-r--r--   0 tarau      (503) staff       (20)       45 2024-03-22 21:22:17.000000 sentence_store-0.4.2/sentence_store/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1009 2024-04-04 02:08:24.000000 sentence_store-0.4.2/sentence_store/tools.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:36:44.653744 sentence_store-0.4.2/sentence_store.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)      929 2024-04-04 03:36:44.000000 sentence_store-0.4.2/sentence_store.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)      358 2024-04-04 03:36:44.000000 sentence_store-0.4.2/sentence_store.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:36:44.000000 sentence_store-0.4.2/sentence_store.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:36:44.000000 sentence_store-0.4.2/sentence_store.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       45 2024-04-04 03:36:44.000000 sentence_store-0.4.2/sentence_store.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       15 2024-04-04 03:36:44.000000 sentence_store-0.4.2/sentence_store.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-04 03:36:44.654543 sentence_store-0.4.2/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      938 2024-03-22 02:06:24.000000 sentence_store-0.4.2/setup.py
```

### Comparing `sentence_store-0.4.1/LICENSE` & `sentence_store-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentence_store-0.4.1/PKG-INFO` & `sentence_store-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentence_store
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tool to extract and store sentence embeddings to a fast and scalable vector db
 Home-page: https://github.com/ptarau/sentence_store.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sentence_store-0.4.1/README.md` & `sentence_store-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sentence_store-0.4.1/sentence_store/main.py` & `sentence_store-0.4.2/sentence_store/main.py`

 * *Files identical despite different names*

### Comparing `sentence_store-0.4.1/sentence_store/tools.py` & `sentence_store-0.4.2/sentence_store/tools.py`

 * *Files identical despite different names*

### Comparing `sentence_store-0.4.1/sentence_store.egg-info/PKG-INFO` & `sentence_store-0.4.2/sentence_store.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentence-store
-Version: 0.4.1
+Version: 0.4.2
 Summary: Tool to extract and store sentence embeddings to a fast and scalable vector db
 Home-page: https://github.com/ptarau/sentence_store.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sentence_store-0.4.1/setup.py` & `sentence_store-0.4.2/setup.py`

 * *Files identical despite different names*

