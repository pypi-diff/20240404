# Comparing `tmp/slcode-1.0.0.tar.gz` & `tmp/slcode-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcode-1.0.0.tar", last modified: Thu Apr  4 09:55:02 2024, max compression
+gzip compressed data, was "slcode-1.0.1.tar", last modified: Thu Apr  4 14:26:02 2024, max compression
```

## Comparing `slcode-1.0.0.tar` & `slcode-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:55:02.225880 slcode-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-04-04 09:54:58.000000 slcode-1.0.0/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-04 09:55:02.225880 slcode-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 09:54:58.000000 slcode-1.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:55:02.225880 slcode-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-04 09:54:58.000000 slcode-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:55:02.221880 slcode-1.0.0/slcode/
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-04 09:54:58.000000 slcode-1.0.0/slcode/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)    79351 2024-04-04 09:54:58.000000 slcode-1.0.0/slcode/SOLVER.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:54:58.000000 slcode-1.0.0/slcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79394 2024-04-04 09:54:59.000000 slcode-1.0.0/slcode/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    21466 2024-04-04 09:54:59.000000 slcode-1.0.0/slcode/love.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-04 09:54:59.000000 slcode-1.0.0/slcode/spharm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:55:02.225880 slcode-1.0.0/slcode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 09:55:02.000000 slcode-1.0.0/slcode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:55:02.225880 slcode-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 09:54:59.000000 slcode-1.0.0/tests/test_SL_C0de_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:26:02.619083 slcode-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35128 2024-04-04 14:25:59.000000 slcode-1.0.1/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-04 14:26:02.619083 slcode-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 14:25:59.000000 slcode-1.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:26:02.619083 slcode-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-04 14:25:59.000000 slcode-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:26:02.619083 slcode-1.0.1/slcode/
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-04 14:25:59.000000 slcode-1.0.1/slcode/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79351 2024-04-04 14:25:59.000000 slcode-1.0.1/slcode/SOLVER.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:25:59.000000 slcode-1.0.1/slcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79394 2024-04-04 14:25:59.000000 slcode-1.0.1/slcode/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21466 2024-04-04 14:25:59.000000 slcode-1.0.1/slcode/love.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-04 14:25:59.000000 slcode-1.0.1/slcode/spharm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:26:02.619083 slcode-1.0.1/slcode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-04 14:26:02.000000 slcode-1.0.1/slcode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 14:26:02.000000 slcode-1.0.1/slcode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:26:02.000000 slcode-1.0.1/slcode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 14:26:02.000000 slcode-1.0.1/slcode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 14:26:02.000000 slcode-1.0.1/slcode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:26:02.619083 slcode-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:25:59.000000 slcode-1.0.1/tests/test_SL_C0de_lib.py
```

### Comparing `slcode-1.0.0/LICENCE.md` & `slcode-1.0.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `slcode-1.0.0/README.rst` & `slcode-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `slcode-1.0.0/setup.py` & `slcode-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import setuptools
 
-VERSION = "1.0.0"  # PEP-440
+VERSION = "1.0.1"  # PEP-440
 
 NAME = "slcode"
 
 INSTALL_REQUIRES = [
-    "joblib==1.2.0",
-    "matplotlib==3.7.0",
-    "numpy==1.24.2",
-    "plotly==5.13.0",
-    "pyshtools==4.10.1",
-    "scipy==1.10.0",
-    "sphinx_rtd_theme==1.2.0",
-    "tomli==2.0.1",
-    "stripy==2.2",
-    "netcdf4==1.6.2",
-    "jupyter==1.0.0",
+    "joblib",
+    "matplotlib",
+    "numpy",
+    "plotly",
+    "pyshtools",
+    "scipy",
+    "stripy",
+    "netcdf4",
 ]
 
+# INSTALL_REQUIRES = [
+#     "joblib==1.2.0",
+#     "matplotlib==3.7.0",
+#     "numpy==1.24.2",
+#     "plotly==5.13.0",
+#     "pyshtools==4.10.1",
+#     "scipy==1.10.0",
+#     "stripy==2.2",
+#     "netcdf4==1.6.2",
+# ]
+
+
 
 setuptools.setup(
     name=NAME,
     version=VERSION,
     description="SL_C0de is a python library based on the matlab code SL_code. This module is used to calculate GIA over the world but alse the sediment isostasy. It include function to calculate radial symetric auto gravitational earth visco-elastic response. This module also include the possibility to resolve the Sea level equation based on the publication of Mitrovica and Austermann ... ajouter des refs. The aim of this library is to be easy to include new sources of load and link to other python library.",
     url="https://github.com/AHenryLarroze/Py_SL_C0de",
     project_urls={
@@ -32,14 +41,14 @@
     author_email="adrien_henry@orange.fr",
     license="GPL-3.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     # Snowpark requires Python 3.8
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     # Requirements
     install_requires=INSTALL_REQUIRES,
     packages=["slcode"],
-    long_description=open("README.rst").read(),
+    long_description=open("Readme.md").read(),
     long_description_content_type="text/markdown",
 )
```

### Comparing `slcode-1.0.0/slcode/Load.py` & `slcode-1.0.1/slcode/Load.py`

 * *Files identical despite different names*

### Comparing `slcode-1.0.0/slcode/SOLVER.py` & `slcode-1.0.1/slcode/SOLVER.py`

 * *Files identical despite different names*

### Comparing `slcode-1.0.0/slcode/grid.py` & `slcode-1.0.1/slcode/grid.py`

 * *Files identical despite different names*

### Comparing `slcode-1.0.0/slcode/love.py` & `slcode-1.0.1/slcode/love.py`

 * *Files identical despite different names*

### Comparing `slcode-1.0.0/slcode/spharm.py` & `slcode-1.0.1/slcode/spharm.py`

 * *Files identical despite different names*

