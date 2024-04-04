# Comparing `tmp/casioplot-3.1.5.tar.gz` & `tmp/casioplot-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casioplot-3.1.5.tar", last modified: Thu Apr  4 06:48:01 2024, max compression
+gzip compressed data, was "casioplot-3.1.6.tar", last modified: Thu Apr  4 06:58:04 2024, max compression
```

## Comparing `casioplot-3.1.5.tar` & `casioplot-3.1.6.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:48:01.363855 casioplot-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 06:47:56.000000 casioplot-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 06:47:56.000000 casioplot-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-04 06:48:01.363855 casioplot-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-04 06:47:56.000000 casioplot-3.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-04 06:47:56.000000 casioplot-3.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 06:48:01.363855 casioplot-3.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:48:01.359854 casioplot-3.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:48:01.363855 casioplot-3.1.5/src/casioplot/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 06:47:56.000000 casioplot-3.1.5/src/casioplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-04-04 06:47:56.000000 casioplot-3.1.5/src/casioplot/casioplot.py
--rw-r--r--   0 runner    (1001) docker     (127)   127297 2024-04-04 06:47:56.000000 casioplot-3.1.5/src/casioplot/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-04 06:47:56.000000 casioplot-3.1.5/src/casioplot/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-04 06:47:56.000000 casioplot-3.1.5/src/casioplot/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:48:01.363855 casioplot-3.1.5/src/casioplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-04 06:48:01.000000 casioplot-3.1.5/src/casioplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-04 06:48:01.000000 casioplot-3.1.5/src/casioplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 06:48:01.000000 casioplot-3.1.5/src/casioplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 06:48:01.000000 casioplot-3.1.5/src/casioplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 06:48:01.000000 casioplot-3.1.5/src/casioplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:58:04.633456 casioplot-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 06:57:59.000000 casioplot-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-04 06:57:59.000000 casioplot-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-04 06:58:04.633456 casioplot-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-04 06:57:59.000000 casioplot-3.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-04 06:57:59.000000 casioplot-3.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 06:58:04.633456 casioplot-3.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:58:04.629456 casioplot-3.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:58:04.629456 casioplot-3.1.6/src/casioplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/casioplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127297 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/characters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:58:04.633456 casioplot-3.1.6/src/casioplot/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/presets/default.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/presets/fx-CG50.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/presets/fx-CG50_AU.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/presets/graph_90+e.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-04 06:57:59.000000 casioplot-3.1.6/src/casioplot/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 06:58:04.633456 casioplot-3.1.6/src/casioplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-04 06:58:04.000000 casioplot-3.1.6/src/casioplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-04 06:58:04.000000 casioplot-3.1.6/src/casioplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 06:58:04.000000 casioplot-3.1.6/src/casioplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 06:58:04.000000 casioplot-3.1.6/src/casioplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 06:58:04.000000 casioplot-3.1.6/src/casioplot.egg-info/top_level.txt
```

### Comparing `casioplot-3.1.5/LICENSE` & `casioplot-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.5/PKG-INFO` & `casioplot-3.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 3.1.5
+Version: 3.1.6
 Summary: Use casioplot module on a computer
 Author-email: Uniwix <uniwixu@gmail.com>, Miguel Torrinha Pereira <miguel.torrinha.pereira+pypi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -124,8 +124,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.5 - Uniwix - MiguelTorrinhaPereira
+v 3.1.6 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.1.5/README.rst` & `casioplot-3.1.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -83,8 +83,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.5 - Uniwix - MiguelTorrinhaPereira
+v 3.1.6 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.1.5/pyproject.toml` & `casioplot-3.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "Pillow"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "casioplot"
-version = "3.1.5"
+version = "3.1.6"
 description = "Use casioplot module on a computer"
 readme = "README.rst"
 authors = [
     { name = "Uniwix", email = "uniwixu@gmail.com" },
     { name = "Miguel Torrinha Pereira", email = "miguel.torrinha.pereira+pypi@gmail.com" }
 ]
 license = { file = "LICENSE" }
```

### Comparing `casioplot-3.1.5/src/casioplot/casioplot.py` & `casioplot-3.1.6/src/casioplot/casioplot.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.5/src/casioplot/characters.py` & `casioplot-3.1.6/src/casioplot/characters.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.5/src/casioplot/settings.py` & `casioplot-3.1.6/src/casioplot/settings.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.5/src/casioplot/types.py` & `casioplot-3.1.6/src/casioplot/types.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.5/src/casioplot.egg-info/PKG-INFO` & `casioplot-3.1.6/src/casioplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 3.1.5
+Version: 3.1.6
 Summary: Use casioplot module on a computer
 Author-email: Uniwix <uniwixu@gmail.com>, Miguel Torrinha Pereira <miguel.torrinha.pereira+pypi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -124,8 +124,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.5 - Uniwix - MiguelTorrinhaPereira
+v 3.1.6 - Uniwix - MiguelTorrinhaPereira
```

