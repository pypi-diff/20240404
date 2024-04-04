# Comparing `tmp/chess-utils-0.1.6.tar.gz` & `tmp/chess-utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-utils-0.1.6.tar", last modified: Thu Apr  4 09:24:02 2024, max compression
+gzip compressed data, was "chess-utils-0.1.7.tar", last modified: Thu Apr  4 18:46:08 2024, max compression
```

## Comparing `chess-utils-0.1.6.tar` & `chess-utils-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:24:02.439819 chess-utils-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      377 2024-04-04 09:24:02.439819 chess-utils-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      520 2024-04-04 09:23:41.000000 chess-utils-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 09:24:02.439819 chess-utils-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:24:02.429819 chess-utils-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:24:02.429819 chess-utils-0.1.6/src/chess_utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-03-21 05:52:16.000000 chess-utils-0.1.6/src/chess_utils/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:24:02.429819 chess-utils-0.1.6/src/chess_utils/fens/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       42 2024-03-21 05:52:30.000000 chess-utils-0.1.6/src/chess_utils/fens/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-03-21 05:50:44.000000 chess-utils-0.1.6/src/chess_utils/fens/fens.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:24:02.429819 chess-utils-0.1.6/src/chess_utils/misc/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-03-21 05:50:11.000000 chess-utils-0.1.6/src/chess_utils/misc/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-03-21 05:50:11.000000 chess-utils-0.1.6/src/chess_utils/misc/misc.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:24:02.429819 chess-utils-0.1.6/src/chess_utils/parse/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-03-21 05:50:11.000000 chess-utils-0.1.6/src/chess_utils/parse/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      850 2024-03-29 09:29:50.000000 chess-utils-0.1.6/src/chess_utils/parse/parse.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-03-21 05:50:11.000000 chess-utils-0.1.6/src/chess_utils/parse/test_parsing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:24:02.439819 chess-utils-0.1.6/src/chess_utils/random/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-03-21 05:50:11.000000 chess-utils-0.1.6/src/chess_utils/random/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1041 2024-03-21 05:50:11.000000 chess-utils-0.1.6/src/chess_utils/random/random.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      254 2024-03-21 05:50:11.000000 chess-utils-0.1.6/src/chess_utils/test.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 09:24:02.439819 chess-utils-0.1.6/src/chess_utils.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      377 2024-04-04 09:24:02.000000 chess-utils-0.1.6/src/chess_utils.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      555 2024-04-04 09:24:02.000000 chess-utils-0.1.6/src/chess_utils.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 09:24:02.000000 chess-utils-0.1.6/src/chess_utils.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-04 09:24:02.000000 chess-utils-0.1.6/src/chess_utils.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-04-04 09:24:02.000000 chess-utils-0.1.6/src/chess_utils.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      410 2024-04-04 18:46:08.434860 chess-utils-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      541 2024-04-04 18:45:58.000000 chess-utils-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 18:46:08.434860 chess-utils-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-03-21 05:52:16.000000 chess-utils-0.1.7/src/chess_utils/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/fens/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       42 2024-03-21 05:52:30.000000 chess-utils-0.1.7/src/chess_utils/fens/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-03-21 05:50:44.000000 chess-utils-0.1.7/src/chess_utils/fens/fens.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/misc/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/misc/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/misc/misc.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/parse/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/parse/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      850 2024-03-29 09:29:50.000000 chess-utils-0.1.7/src/chess_utils/parse/parse.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/parse/test_parsing.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/pgns/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:42:54.000000 chess-utils-0.1.7/src/chess_utils/pgns/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      257 2024-04-04 18:45:41.000000 chess-utils-0.1.7/src/chess_utils/pgns/pgns.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/random/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/random/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1041 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/random/random.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      254 2024-04-04 18:45:50.000000 chess-utils-0.1.7/src/chess_utils/test.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      410 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      617 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/top_level.txt
```

### Comparing `chess-utils-0.1.6/pyproject.toml` & `chess-utils-0.1.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-utils"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Higher level utilities over the `chess` library"
 dependencies = [
-    "chess", "pydantic"
+    "chess", "pydantic", "haskellian-either"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.optional-dependencies]
 test = [
     "pytest", "hypothesis"
```

### Comparing `chess-utils-0.1.6/src/chess_utils/fens/fens.py` & `chess-utils-0.1.7/src/chess_utils/fens/fens.py`

 * *Files identical despite different names*

### Comparing `chess-utils-0.1.6/src/chess_utils/misc/misc.py` & `chess-utils-0.1.7/src/chess_utils/misc/misc.py`

 * *Files identical despite different names*

### Comparing `chess-utils-0.1.6/src/chess_utils/parse/parse.py` & `chess-utils-0.1.7/src/chess_utils/parse/parse.py`

 * *Files identical despite different names*

### Comparing `chess-utils-0.1.6/src/chess_utils/random/random.py` & `chess-utils-0.1.7/src/chess_utils/random/random.py`

 * *Files identical despite different names*

### Comparing `chess-utils-0.1.6/src/chess_utils.egg-info/SOURCES.txt` & `chess-utils-0.1.7/src/chess_utils.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,9 +9,11 @@
 src/chess_utils/fens/__init__.py
 src/chess_utils/fens/fens.py
 src/chess_utils/misc/__init__.py
 src/chess_utils/misc/misc.py
 src/chess_utils/parse/__init__.py
 src/chess_utils/parse/parse.py
 src/chess_utils/parse/test_parsing.py
+src/chess_utils/pgns/__init__.py
+src/chess_utils/pgns/pgns.py
 src/chess_utils/random/__init__.py
 src/chess_utils/random/random.py
```

