# Comparing `tmp/naapc-2.1.1.tar.gz` & `tmp/naapc-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naapc-2.1.1.tar", last modified: Wed Sep 27 12:31:28 2023, max compression
+gzip compressed data, was "naapc-2.1.2.tar", last modified: Thu Apr  4 12:54:29 2024, max compression
```

## Comparing `naapc-2.1.1.tar` & `naapc-2.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2023-09-27 12:31:28.799075 naapc-2.1.1/
--rw-r--r--   0 ei        (1000) ei        (1000)     1067 2023-09-24 12:01:55.000000 naapc-2.1.1/LICENSE
--rw-r--r--   0 ei        (1000) ei        (1000)     4224 2023-09-27 12:31:28.799075 naapc-2.1.1/PKG-INFO
--rw-r--r--   0 ei        (1000) ei        (1000)     2444 2023-09-24 12:01:55.000000 naapc-2.1.1/README.md
--rw-r--r--   0 ei        (1000) ei        (1000)     1003 2023-09-27 12:30:40.000000 naapc-2.1.1/pyproject.toml
--rw-r--r--   0 ei        (1000) ei        (1000)       38 2023-09-27 12:31:28.799075 naapc-2.1.1/setup.cfg
-drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2023-09-27 12:31:28.799075 naapc-2.1.1/src/
-drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2023-09-27 12:31:28.799075 naapc-2.1.1/src/naapc/
--rw-r--r--   0 ei        (1000) ei        (1000)      130 2023-09-27 12:30:40.000000 naapc-2.1.1/src/naapc/__init__.py
--rw-r--r--   0 ei        (1000) ei        (1000)     8780 2023-09-27 12:27:29.000000 naapc-2.1.1/src/naapc/base.py
--rw-r--r--   0 ei        (1000) ei        (1000)     4084 2023-09-26 13:27:14.000000 naapc-2.1.1/src/naapc/dict_traverse.py
--rw-r--r--   0 ei        (1000) ei        (1000)     7046 2023-09-27 12:29:52.000000 naapc-2.1.1/src/naapc/ndict.py
--rw-r--r--   0 ei        (1000) ei        (1000)      561 2023-09-26 13:27:14.000000 naapc-2.1.1/src/naapc/snd.py
--rw-r--r--   0 ei        (1000) ei        (1000)      505 2023-09-24 12:01:55.000000 naapc-2.1.1/src/naapc/stop_conditions.py
-drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2023-09-27 12:31:28.799075 naapc-2.1.1/src/naapc.egg-info/
--rw-r--r--   0 ei        (1000) ei        (1000)     4224 2023-09-27 12:31:28.000000 naapc-2.1.1/src/naapc.egg-info/PKG-INFO
--rw-r--r--   0 ei        (1000) ei        (1000)      364 2023-09-27 12:31:28.000000 naapc-2.1.1/src/naapc.egg-info/SOURCES.txt
--rw-r--r--   0 ei        (1000) ei        (1000)        1 2023-09-27 12:31:28.000000 naapc-2.1.1/src/naapc.egg-info/dependency_links.txt
--rw-r--r--   0 ei        (1000) ei        (1000)        7 2023-09-27 12:31:28.000000 naapc-2.1.1/src/naapc.egg-info/requires.txt
--rw-r--r--   0 ei        (1000) ei        (1000)        6 2023-09-27 12:31:28.000000 naapc-2.1.1/src/naapc.egg-info/top_level.txt
-drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2023-09-27 12:31:28.799075 naapc-2.1.1/test/
--rw-r--r--   0 ei        (1000) ei        (1000)    15297 2023-09-27 12:28:53.000000 naapc-2.1.1/test/test_ndict.py
--rw-r--r--   0 ei        (1000) ei        (1000)    15290 2023-09-27 12:30:25.000000 naapc-2.1.1/test/test_snd.py
+drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2024-04-04 12:54:29.201875 naapc-2.1.2/
+-rw-r--r--   0 ei        (1000) ei        (1000)     1067 2024-04-04 12:51:41.000000 naapc-2.1.2/LICENSE
+-rw-r--r--   0 ei        (1000) ei        (1000)     4222 2024-04-04 12:54:29.201875 naapc-2.1.2/PKG-INFO
+-rw-r--r--   0 ei        (1000) ei        (1000)     2444 2024-04-04 12:51:41.000000 naapc-2.1.2/README.md
+-rw-r--r--   0 ei        (1000) ei        (1000)     1001 2024-04-04 12:51:59.000000 naapc-2.1.2/pyproject.toml
+-rw-r--r--   0 ei        (1000) ei        (1000)       38 2024-04-04 12:54:29.201875 naapc-2.1.2/setup.cfg
+drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2024-04-04 12:54:29.201875 naapc-2.1.2/src/
+drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2024-04-04 12:54:29.201875 naapc-2.1.2/src/naapc/
+-rw-r--r--   0 ei        (1000) ei        (1000)      130 2024-04-04 12:52:11.000000 naapc-2.1.2/src/naapc/__init__.py
+-rw-r--r--   0 ei        (1000) ei        (1000)     8780 2024-04-04 12:51:41.000000 naapc-2.1.2/src/naapc/base.py
+-rw-r--r--   0 ei        (1000) ei        (1000)     4084 2024-04-04 12:51:41.000000 naapc-2.1.2/src/naapc/dict_traverse.py
+-rw-r--r--   0 ei        (1000) ei        (1000)     7046 2024-04-04 12:51:41.000000 naapc-2.1.2/src/naapc/ndict.py
+-rw-r--r--   0 ei        (1000) ei        (1000)      561 2024-04-04 12:51:41.000000 naapc-2.1.2/src/naapc/snd.py
+-rw-r--r--   0 ei        (1000) ei        (1000)      505 2024-04-04 12:51:41.000000 naapc-2.1.2/src/naapc/stop_conditions.py
+drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2024-04-04 12:54:29.201875 naapc-2.1.2/src/naapc.egg-info/
+-rw-r--r--   0 ei        (1000) ei        (1000)     4222 2024-04-04 12:54:29.000000 naapc-2.1.2/src/naapc.egg-info/PKG-INFO
+-rw-r--r--   0 ei        (1000) ei        (1000)      364 2024-04-04 12:54:29.000000 naapc-2.1.2/src/naapc.egg-info/SOURCES.txt
+-rw-r--r--   0 ei        (1000) ei        (1000)        1 2024-04-04 12:54:29.000000 naapc-2.1.2/src/naapc.egg-info/dependency_links.txt
+-rw-r--r--   0 ei        (1000) ei        (1000)        7 2024-04-04 12:54:29.000000 naapc-2.1.2/src/naapc.egg-info/requires.txt
+-rw-r--r--   0 ei        (1000) ei        (1000)        6 2024-04-04 12:54:29.000000 naapc-2.1.2/src/naapc.egg-info/top_level.txt
+drwxr-xr-x   0 ei        (1000) ei        (1000)        0 2024-04-04 12:54:29.201875 naapc-2.1.2/test/
+-rw-r--r--   0 ei        (1000) ei        (1000)    15297 2024-04-04 12:51:41.000000 naapc-2.1.2/test/test_ndict.py
+-rw-r--r--   0 ei        (1000) ei        (1000)    15290 2024-04-04 12:51:41.000000 naapc-2.1.2/test/test_snd.py
```

### Comparing `naapc-2.1.1/LICENSE` & `naapc-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `naapc-2.1.1/PKG-INFO` & `naapc-2.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 2.1.1
+Version: 2.1.2
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: repository, https://github.com/eiphy/naapc
 Keywords: configuration,config,dictionary,nested,argument parsing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: ==3.10.*
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 
 # Nested Automated Argument Parsing Configuration (NAAPC)
 [NAAPC](https://pypi.org/project/naapc/) contains two classes: NConfig and NDict.
 NDict provides method to easily manipulate nested dictionaries.
```

### Comparing `naapc-2.1.1/README.md` & `naapc-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `naapc-2.1.1/pyproject.toml` & `naapc-2.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["wheel", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naapc"
-version = "2.1.1"
+version = "2.1.2"
 description = "Nested Automated Argument Parsing Configuration (NAAPC)."
 readme = "README.md"
 authors = [{name = "Bai Huanyu", email = "eiphnix@gmail.com"}]
 license = {file = "LICENSE"}
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["configuration", "config", "dictionary", "nested", "argument parsing"]
 dependencies = ["pyyaml"]
-requires-python = "==3.10.*"
+requires-python = ">=3.10"
 
 [project.urls]
 repository = "https://github.com/eiphy/naapc"
 
 [tool.bumpver]
-current_version = "2.1.1"
+current_version = "2.1.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `naapc-2.1.1/src/naapc/base.py` & `naapc-2.1.2/src/naapc/base.py`

 * *Files identical despite different names*

### Comparing `naapc-2.1.1/src/naapc/dict_traverse.py` & `naapc-2.1.2/src/naapc/dict_traverse.py`

 * *Files identical despite different names*

### Comparing `naapc-2.1.1/src/naapc/ndict.py` & `naapc-2.1.2/src/naapc/ndict.py`

 * *Files identical despite different names*

### Comparing `naapc-2.1.1/src/naapc/snd.py` & `naapc-2.1.2/src/naapc/snd.py`

 * *Files identical despite different names*

### Comparing `naapc-2.1.1/src/naapc.egg-info/PKG-INFO` & `naapc-2.1.2/src/naapc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 2.1.1
+Version: 2.1.2
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: repository, https://github.com/eiphy/naapc
 Keywords: configuration,config,dictionary,nested,argument parsing
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: ==3.10.*
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 
 # Nested Automated Argument Parsing Configuration (NAAPC)
 [NAAPC](https://pypi.org/project/naapc/) contains two classes: NConfig and NDict.
 NDict provides method to easily manipulate nested dictionaries.
```

### Comparing `naapc-2.1.1/test/test_ndict.py` & `naapc-2.1.2/test/test_ndict.py`

 * *Files identical despite different names*

### Comparing `naapc-2.1.1/test/test_snd.py` & `naapc-2.1.2/test/test_snd.py`

 * *Files identical despite different names*

