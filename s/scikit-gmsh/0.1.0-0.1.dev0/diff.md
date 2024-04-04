# Comparing `tmp/scikit-gmsh-0.1.0.tar.gz` & `tmp/scikit-gmsh-0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-gmsh-0.1.0.tar", last modified: Thu Apr  4 05:13:00 2024, max compression
+gzip compressed data, was "scikit-gmsh-0.1.dev0.tar", last modified: Thu Apr  4 05:09:42 2024, max compression
```

## Comparing `scikit-gmsh-0.1.0.tar` & `scikit-gmsh-0.1.dev0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:13:00.382687 scikit-gmsh-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 05:12:24.000000 scikit-gmsh-0.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 05:12:24.000000 scikit-gmsh-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-04 05:13:00.382687 scikit-gmsh-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-04 05:12:24.000000 scikit-gmsh-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-04 05:12:24.000000 scikit-gmsh-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:13:00.382687 scikit-gmsh-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-04 05:12:24.000000 scikit-gmsh-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:13:00.378687 scikit-gmsh-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:13:00.382687 scikit-gmsh-0.1.0/src/scikit_gmsh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-04 05:13:00.000000 scikit-gmsh-0.1.0/src/scikit_gmsh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-04 05:13:00.000000 scikit-gmsh-0.1.0/src/scikit_gmsh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:13:00.000000 scikit-gmsh-0.1.0/src/scikit_gmsh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 05:13:00.000000 scikit-gmsh-0.1.0/src/scikit_gmsh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 05:13:00.000000 scikit-gmsh-0.1.0/src/scikit_gmsh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:13:00.382687 scikit-gmsh-0.1.0/src/skgmsh/
--rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-04-04 05:12:24.000000 scikit-gmsh-0.1.0/src/skgmsh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:13:00.382687 scikit-gmsh-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-04 05:12:24.000000 scikit-gmsh-0.1.0/tests/test_skgmsh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:09:42.729515 scikit-gmsh-0.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 05:08:44.000000 scikit-gmsh-0.1.dev0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 05:08:44.000000 scikit-gmsh-0.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-04 05:09:42.729515 scikit-gmsh-0.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-04 05:08:44.000000 scikit-gmsh-0.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-04 05:08:44.000000 scikit-gmsh-0.1.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:09:42.729515 scikit-gmsh-0.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-04 05:08:44.000000 scikit-gmsh-0.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:09:42.725515 scikit-gmsh-0.1.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:09:42.729515 scikit-gmsh-0.1.dev0/src/scikit_gmsh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-04 05:09:42.000000 scikit-gmsh-0.1.dev0/src/scikit_gmsh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-04 05:09:42.000000 scikit-gmsh-0.1.dev0/src/scikit_gmsh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:09:42.000000 scikit-gmsh-0.1.dev0/src/scikit_gmsh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 05:09:42.000000 scikit-gmsh-0.1.dev0/src/scikit_gmsh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 05:09:42.000000 scikit-gmsh-0.1.dev0/src/scikit_gmsh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:09:42.729515 scikit-gmsh-0.1.dev0/src/skgmsh/
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-04-04 05:08:44.000000 scikit-gmsh-0.1.dev0/src/skgmsh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:09:42.729515 scikit-gmsh-0.1.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-04 05:08:44.000000 scikit-gmsh-0.1.dev0/tests/test_skgmsh.py
```

### Comparing `scikit-gmsh-0.1.0/AUTHORS.md` & `scikit-gmsh-0.1.dev0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `scikit-gmsh-0.1.0/LICENSE` & `scikit-gmsh-0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-gmsh-0.1.0/PKG-INFO` & `scikit-gmsh-0.1.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-gmsh
-Version: 0.1.0
+Version: 0.1.dev0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: gmsh<4.12.3
 Requires-Dist: meshio<5.3.6
 Requires-Dist: pygmsh<7.1.18
```

### Comparing `scikit-gmsh-0.1.0/README.md` & `scikit-gmsh-0.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `scikit-gmsh-0.1.0/pyproject.toml` & `scikit-gmsh-0.1.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit-gmsh-0.1.0/src/scikit_gmsh.egg-info/PKG-INFO` & `scikit-gmsh-0.1.dev0/src/scikit_gmsh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-gmsh
-Version: 0.1.0
+Version: 0.1.dev0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: gmsh<4.12.3
 Requires-Dist: meshio<5.3.6
 Requires-Dist: pygmsh<7.1.18
```

### Comparing `scikit-gmsh-0.1.0/src/skgmsh/__init__.py` & `scikit-gmsh-0.1.dev0/src/skgmsh/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 FRONTAL_DELAUNAY_2D = 6
 DELAUNAY_3D = 1
 
 now = datetime.datetime.now(tz=datetime.timezone.utc)
 
 # major, minor, patch
-version_info = 0, 1, 0
+version_info = 0, 1, "dev0"
 
 # Nice string for the version
 __version__ = ".".join(map(str, version_info))
 
 
 def frontal_delaunay_2d(
     edge_source: pv.PolyData,
```

### Comparing `scikit-gmsh-0.1.0/tests/test_skgmsh.py` & `scikit-gmsh-0.1.dev0/tests/test_skgmsh.py`

 * *Files identical despite different names*

