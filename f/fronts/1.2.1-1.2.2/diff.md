# Comparing `tmp/fronts-1.2.1.tar.gz` & `tmp/fronts-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fronts-1.2.1.tar", last modified: Mon Feb 19 15:49:55 2024, max compression
+gzip compressed data, was "fronts-1.2.2.tar", last modified: Thu Apr  4 21:42:01 2024, max compression
```

## Comparing `fronts-1.2.1.tar` & `fronts-1.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:49:55.684744 fronts-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-19 15:49:47.000000 fronts-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-02-19 15:49:55.684744 fronts-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-02-19 15:49:47.000000 fronts-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:49:55.680745 fronts-1.2.1/fronts/
--rw-r--r--   0 runner    (1001) docker     (127)    33379 2024-02-19 15:49:47.000000 fronts-1.2.1/fronts/D.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-19 15:49:47.000000 fronts-1.2.1/fronts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-02-19 15:49:47.000000 fronts-1.2.1/fronts/_boltzmann.py
--rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-02-19 15:49:47.000000 fronts-1.2.1/fronts/_inverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-02-19 15:49:47.000000 fronts-1.2.1/fronts/_rootfinding.py
--rw-r--r--   0 runner    (1001) docker     (127)    46864 2024-02-19 15:49:47.000000 fronts-1.2.1/fronts/_semiinfinite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:49:55.684744 fronts-1.2.1/fronts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-02-19 15:49:55.000000 fronts-1.2.1/fronts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-19 15:49:55.000000 fronts-1.2.1/fronts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 15:49:55.000000 fronts-1.2.1/fronts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-19 15:49:55.000000 fronts-1.2.1/fronts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-19 15:49:55.000000 fronts-1.2.1/fronts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-02-19 15:49:47.000000 fronts-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 15:49:55.684744 fronts-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 15:49:55.684744 fronts-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-19 15:49:47.000000 fronts-1.2.1/tests/test_D.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-19 15:49:47.000000 fronts-1.2.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-19 15:49:47.000000 fronts-1.2.1/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-02-19 15:49:47.000000 fronts-1.2.1/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-19 15:49:47.000000 fronts-1.2.1/tests/test_solve_flowrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-19 15:49:47.000000 fronts-1.2.1/tests/test_solve_from_guess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:42:01.249475 fronts-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-04 21:41:56.000000 fronts-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-04 21:42:01.249475 fronts-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-04-04 21:41:56.000000 fronts-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:42:01.249475 fronts-1.2.2/fronts/
+-rw-r--r--   0 runner    (1001) docker     (127)    33379 2024-04-04 21:41:56.000000 fronts-1.2.2/fronts/D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-04 21:41:56.000000 fronts-1.2.2/fronts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17722 2024-04-04 21:41:56.000000 fronts-1.2.2/fronts/_boltzmann.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-04-04 21:41:56.000000 fronts-1.2.2/fronts/_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-04 21:41:56.000000 fronts-1.2.2/fronts/_rootfinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46864 2024-04-04 21:41:56.000000 fronts-1.2.2/fronts/_semiinfinite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:42:01.249475 fronts-1.2.2/fronts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-04 21:42:01.000000 fronts-1.2.2/fronts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-04 21:42:01.000000 fronts-1.2.2/fronts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:42:01.000000 fronts-1.2.2/fronts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-04 21:42:01.000000 fronts-1.2.2/fronts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 21:42:01.000000 fronts-1.2.2/fronts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-04 21:41:56.000000 fronts-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:42:01.249475 fronts-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:42:01.249475 fronts-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-04 21:41:56.000000 fronts-1.2.2/tests/test_D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-04 21:41:56.000000 fronts-1.2.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-04 21:41:56.000000 fronts-1.2.2/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-04 21:41:56.000000 fronts-1.2.2/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-04 21:41:56.000000 fronts-1.2.2/tests/test_solve_flowrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 21:41:56.000000 fronts-1.2.2/tests/test_solve_from_guess.py
```

### Comparing `fronts-1.2.1/LICENSE.txt` & `fronts-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/PKG-INFO` & `fronts-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fronts
-Version: 1.2.1
+Version: 1.2.2
 Summary: Numerical library for nonlinear diffusion problems in semi-infinite domains
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/fronts
 Project-URL: Repository, https://github.com/gerlero/fronts
 Project-URL: Documentation, https://fronts.readthedocs.io
 Project-URL: Changelog, https://github.com/gerlero/fronts/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,15 +31,15 @@
 Requires-Dist: matplotlib==3.*; extra == "examples"
 Provides-Extra: test
 Requires-Dist: pytest<9,>=7; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: autograd<2,>=1.3; extra == "test"
 Requires-Dist: fronts[examples]; extra == "test"
 Provides-Extra: doc
-Requires-Dist: sphinx<7,>=5; extra == "doc"
+Requires-Dist: sphinx<8,>=5; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: fronts[examples]; extra == "dev"
 Requires-Dist: fronts[test]; extra == "dev"
 Requires-Dist: fronts[doc]; extra == "dev"
 
 [<img alt="Fronts" src="https://raw.githubusercontent.com/gerlero/fronts/main/resources/logo.png" height="100">](https://github.com/gerlero/fronts)
```

### Comparing `fronts-1.2.1/README.md` & `fronts-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/fronts/D.py` & `fronts-1.2.2/fronts/D.py`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/fronts/_boltzmann.py` & `fronts-1.2.2/fronts/_boltzmann.py`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/fronts/_inverse.py` & `fronts-1.2.2/fronts/_inverse.py`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/fronts/_rootfinding.py` & `fronts-1.2.2/fronts/_rootfinding.py`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/fronts/_semiinfinite.py` & `fronts-1.2.2/fronts/_semiinfinite.py`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/fronts.egg-info/PKG-INFO` & `fronts-1.2.2/fronts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fronts
-Version: 1.2.1
+Version: 1.2.2
 Summary: Numerical library for nonlinear diffusion problems in semi-infinite domains
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/gerlero/fronts
 Project-URL: Repository, https://github.com/gerlero/fronts
 Project-URL: Documentation, https://fronts.readthedocs.io
 Project-URL: Changelog, https://github.com/gerlero/fronts/blob/main/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,15 +31,15 @@
 Requires-Dist: matplotlib==3.*; extra == "examples"
 Provides-Extra: test
 Requires-Dist: pytest<9,>=7; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: autograd<2,>=1.3; extra == "test"
 Requires-Dist: fronts[examples]; extra == "test"
 Provides-Extra: doc
-Requires-Dist: sphinx<7,>=5; extra == "doc"
+Requires-Dist: sphinx<8,>=5; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Provides-Extra: dev
 Requires-Dist: fronts[examples]; extra == "dev"
 Requires-Dist: fronts[test]; extra == "dev"
 Requires-Dist: fronts[doc]; extra == "dev"
 
 [<img alt="Fronts" src="https://raw.githubusercontent.com/gerlero/fronts/main/resources/logo.png" height="100">](https://github.com/gerlero/fronts)
```

### Comparing `fronts-1.2.1/pyproject.toml` & `fronts-1.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 test = [
     "pytest>=7,<9",
     "pytest-cov",
     "autograd>=1.3,<2",
     "fronts[examples]",
 ]
 doc = [
-    "sphinx>=5,<7",
+    "sphinx>=5,<8",
     "sphinx_rtd_theme",
 ]
 dev = [
     "fronts[examples]",
     "fronts[test]",
     "fronts[doc]",
 ]
```

### Comparing `fronts-1.2.1/tests/test_D.py` & `fronts-1.2.2/tests/test_D.py`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/tests/test_inverse.py` & `fronts-1.2.2/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/tests/test_solve.py` & `fronts-1.2.2/tests/test_solve.py`

 * *Files identical despite different names*

### Comparing `fronts-1.2.1/tests/test_solve_flowrate.py` & `fronts-1.2.2/tests/test_solve_flowrate.py`

 * *Files identical despite different names*

