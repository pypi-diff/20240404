# Comparing `tmp/casioplot-3.1.3.tar.gz` & `tmp/casioplot-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casioplot-3.1.3.tar", last modified: Wed Apr  3 21:08:13 2024, max compression
+gzip compressed data, was "casioplot-3.1.4.tar", last modified: Wed Apr  3 22:11:20 2024, max compression
```

## Comparing `casioplot-3.1.3.tar` & `casioplot-3.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:08:13.839917 casioplot-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 21:08:05.000000 casioplot-3.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 21:08:05.000000 casioplot-3.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-03 21:08:13.839917 casioplot-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-03 21:08:05.000000 casioplot-3.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-03 21:08:05.000000 casioplot-3.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:08:13.839917 casioplot-3.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:08:13.835917 casioplot-3.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:08:13.835917 casioplot-3.1.3/src/casioplot/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 21:08:05.000000 casioplot-3.1.3/src/casioplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-04-03 21:08:05.000000 casioplot-3.1.3/src/casioplot/casioplot.py
--rw-r--r--   0 runner    (1001) docker     (127)   127297 2024-04-03 21:08:05.000000 casioplot-3.1.3/src/casioplot/characters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-03 21:08:05.000000 casioplot-3.1.3/src/casioplot/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 21:08:05.000000 casioplot-3.1.3/src/casioplot/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:08:13.839917 casioplot-3.1.3/src/casioplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-03 21:08:13.000000 casioplot-3.1.3/src/casioplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-03 21:08:13.000000 casioplot-3.1.3/src/casioplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:08:13.000000 casioplot-3.1.3/src/casioplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 21:08:13.000000 casioplot-3.1.3/src/casioplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 21:08:13.000000 casioplot-3.1.3/src/casioplot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:11:20.567046 casioplot-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 22:11:15.000000 casioplot-3.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 22:11:15.000000 casioplot-3.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-03 22:11:20.567046 casioplot-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-03 22:11:15.000000 casioplot-3.1.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-03 22:11:15.000000 casioplot-3.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:11:20.567046 casioplot-3.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:11:20.563046 casioplot-3.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:11:20.567046 casioplot-3.1.4/src/casioplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 22:11:15.000000 casioplot-3.1.4/src/casioplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-04-03 22:11:15.000000 casioplot-3.1.4/src/casioplot/casioplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127297 2024-04-03 22:11:15.000000 casioplot-3.1.4/src/casioplot/characters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-04-03 22:11:15.000000 casioplot-3.1.4/src/casioplot/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-03 22:11:15.000000 casioplot-3.1.4/src/casioplot/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:11:20.567046 casioplot-3.1.4/src/casioplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-03 22:11:20.000000 casioplot-3.1.4/src/casioplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-03 22:11:20.000000 casioplot-3.1.4/src/casioplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:11:20.000000 casioplot-3.1.4/src/casioplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 22:11:20.000000 casioplot-3.1.4/src/casioplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 22:11:20.000000 casioplot-3.1.4/src/casioplot.egg-info/top_level.txt
```

### Comparing `casioplot-3.1.3/LICENSE` & `casioplot-3.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.3/PKG-INFO` & `casioplot-3.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 3.1.3
+Version: 3.1.4
 Summary: Use casioplot module on a computer
 Author-email: Uniwix <uniwixu@gmail.com>, Miguel Torrinha Pereira <miguel.torrinha.pereira+pypi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Pillow
 
 Casioplot for computers
 =======================
 
-    Module ``casioplot`` from Casio calculator for Computers.
+Module ``casioplot`` from Casio calculator for Computers.
 
 This can help to develop python programs in your computer and run it before you put it in your calculator.
 Due to it's customization ability, this package can also be used as simple way to draw at a pixel level.
 
 .. image:: docs/source/images/colours.png
     :alt: A colorful image
 
@@ -124,8 +124,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.3 - Uniwix
+v 3.1.4 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.1.3/README.rst` & `casioplot-3.1.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Casioplot for computers
 =======================
 
-    Module ``casioplot`` from Casio calculator for Computers.
+Module ``casioplot`` from Casio calculator for Computers.
 
 This can help to develop python programs in your computer and run it before you put it in your calculator.
 Due to it's customization ability, this package can also be used as simple way to draw at a pixel level.
 
 .. image:: docs/source/images/colours.png
     :alt: A colorful image
 
@@ -83,8 +83,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.3 - Uniwix
+v 3.1.4 - Uniwix - MiguelTorrinhaPereira
```

### Comparing `casioplot-3.1.3/pyproject.toml` & `casioplot-3.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel",
     "Pillow"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "casioplot"
-version = "3.1.3"
+version = "3.1.4"
 description = "Use casioplot module on a computer"
 readme = "README.rst"
 authors = [
     { name = "Uniwix", email = "uniwixu@gmail.com" },
     { name = "Miguel Torrinha Pereira", email = "miguel.torrinha.pereira+pypi@gmail.com" }
 ]
 license = { file = "LICENSE" }
```

### Comparing `casioplot-3.1.3/src/casioplot/casioplot.py` & `casioplot-3.1.4/src/casioplot/casioplot.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.3/src/casioplot/characters.py` & `casioplot-3.1.4/src/casioplot/characters.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.3/src/casioplot/settings.py` & `casioplot-3.1.4/src/casioplot/settings.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.3/src/casioplot/types.py` & `casioplot-3.1.4/src/casioplot/types.py`

 * *Files identical despite different names*

### Comparing `casioplot-3.1.3/src/casioplot.egg-info/PKG-INFO` & `casioplot-3.1.4/src/casioplot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casioplot
-Version: 3.1.3
+Version: 3.1.4
 Summary: Use casioplot module on a computer
 Author-email: Uniwix <uniwixu@gmail.com>, Miguel Torrinha Pereira <miguel.torrinha.pereira+pypi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Uniwix
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,15 +38,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Pillow
 
 Casioplot for computers
 =======================
 
-    Module ``casioplot`` from Casio calculator for Computers.
+Module ``casioplot`` from Casio calculator for Computers.
 
 This can help to develop python programs in your computer and run it before you put it in your calculator.
 Due to it's customization ability, this package can also be used as simple way to draw at a pixel level.
 
 .. image:: docs/source/images/colours.png
     :alt: A colorful image
 
@@ -124,8 +124,8 @@
 1. Fork it (`<https://github.com/uniwix/casioplot/fork>`_)
 2. Create your feature branch (``git checkout -b feature/fooBar``)
 3. Commit your changes (``git commit -am 'Add some fooBar'``)
 4. Push to the branch (``git push origin feature/fooBar``)
 5. Create a new Pull Request
 
 
-v 3.1.3 - Uniwix
+v 3.1.4 - Uniwix - MiguelTorrinhaPereira
```

