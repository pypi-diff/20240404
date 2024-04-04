# Comparing `tmp/pyscail-0.0.8.tar.gz` & `tmp/pyscail-0.0.9.tar.gz`

## Comparing `pyscail-0.0.8.tar` & `pyscail-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pyscail-0.0.8/Makefile
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pyscail-0.0.8/demos/ant.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pyscail-0.0.8/demos/belusov-zhabotinsky.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pyscail-0.0.8/demos/game-of-life.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyscail-0.0.8/demos/julia.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 pyscail-0.0.8/demos/wireworld.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyscail-0.0.8/src/pyscail/__init__.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 pyscail-0.0.8/src/pyscail/graphics.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pyscail-0.0.8/src/pyscail/grid.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyscail-0.0.8/src/pyscail/kernels.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pyscail-0.0.8/src/pyscail/pyscail.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 pyscail-0.0.8/src/pyscail/settings.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pyscail-0.0.8/tests/tests.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pyscail-0.0.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyscail-0.0.8/LICENSE
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 pyscail-0.0.8/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 pyscail-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pyscail-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 pyscail-0.0.9/Makefile
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 pyscail-0.0.9/demos/ant.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pyscail-0.0.9/demos/belusov-zhabotinsky.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 pyscail-0.0.9/demos/game-of-life.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyscail-0.0.9/demos/julia.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 pyscail-0.0.9/demos/wireworld.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyscail-0.0.9/src/pyscail/__init__.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 pyscail-0.0.9/src/pyscail/graphics.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pyscail-0.0.9/src/pyscail/grid.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 pyscail-0.0.9/src/pyscail/kernels.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 pyscail-0.0.9/src/pyscail/pyscail.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 pyscail-0.0.9/src/pyscail/settings.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 pyscail-0.0.9/tests/tests.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pyscail-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pyscail-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 pyscail-0.0.9/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 pyscail-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pyscail-0.0.9/PKG-INFO
```

### Comparing `pyscail-0.0.8/demos/ant.py` & `pyscail-0.0.9/demos/ant.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/demos/belusov-zhabotinsky.py` & `pyscail-0.0.9/demos/belusov-zhabotinsky.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/demos/game-of-life.py` & `pyscail-0.0.9/demos/game-of-life.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/demos/julia.py` & `pyscail-0.0.9/demos/julia.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/demos/wireworld.py` & `pyscail-0.0.9/demos/wireworld.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/src/pyscail/graphics.py` & `pyscail-0.0.9/src/pyscail/graphics.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/src/pyscail/grid.py` & `pyscail-0.0.9/src/pyscail/grid.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/src/pyscail/kernels.py` & `pyscail-0.0.9/src/pyscail/kernels.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/src/pyscail/pyscail.py` & `pyscail-0.0.9/src/pyscail/pyscail.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import pygame
 
-from settings import Settings
-from graphics import Graphics
-from grid import Grid
-import kernels
+from pyscail.settings import Settings
+from pyscail.graphics import Graphics
+from pyscail.grid import Grid
 
 
 class Scail:
     grid: Grid | None = None
 
 
 def mainLoop(initialize, update, settings: Settings):
```

### Comparing `pyscail-0.0.8/src/pyscail/settings.py` & `pyscail-0.0.9/src/pyscail/settings.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/tests/tests.py` & `pyscail-0.0.9/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/LICENSE` & `pyscail-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/README.md` & `pyscail-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyscail-0.0.8/pyproject.toml` & `pyscail-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyscail"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = ["pygame"]
 authors = [{ name = "Ribhu Hooja", email = "ribhu.hooja.27@dartmouth.edu" }]
 description = "A package that helps build cellular automata"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `pyscail-0.0.8/PKG-INFO` & `pyscail-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyscail
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package that helps build cellular automata
 Project-URL: Homepage, https://github.com/ribhuhooja/pyscail
 Project-URL: Issues, https://github.com/ribhuhooja/pyscail/issues
 Author-email: Ribhu Hooja <ribhu.hooja.27@dartmouth.edu>
 License-File: LICENSE
 Keywords: cellular automata,game of life
 Classifier: License :: OSI Approved :: MIT License
```

