# Comparing `tmp/pycanha_core-0.0.3.tar.gz` & `tmp/pycanha_core-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycanha_core-0.0.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "pycanha_core-0.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pycanha_core-0.0.3.tar` & `pycanha_core-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,31 @@
--rw-r--r--   0        0        0     3217 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/.github/workflows/build-publish-wheels.yml
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/.gitignore
--rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/.gitmodules
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/.pytest_cache/README.md
--rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/LICENSE
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/README.md
--rw-r--r--   0        0        0     4134 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      560 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/CMakeLists.txt
--rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/__init__.py
--rw-r--r--   0        0        0     3776 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/geometry.hpp
--rw-r--r--   0        0        0      982 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/geometrymodel.hpp
--rw-r--r--   0        0        0     8431 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/primitives.hpp
--rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/thermalmesh.hpp
--rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/transformations.hpp
--rw-r--r--   0        0        0     7877 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/trimesh.hpp
--rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/conanfile.txt.in
--rw-r--r--   0        0        0     4817 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/prepare-build-backend.py
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/pycanha-core-conan-profile
--rw-r--r--   0        0        0     1004 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/pycanha-core-wrapper.cpp
--rw-r--r--   0        0        0     7438 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/src/pycanha_core/pycanha_core.pyi
--rw-r--r--   0        0        0     2229 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/test/primitives/test_triangle.py
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 pycanha_core-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3242 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.github/workflows/build-publish-wheels.yml
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.gitignore
+-rw-r--r--   0        0        0      156 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.gitmodules
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0      885 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1027 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/LICENSE
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/README.md
+-rw-r--r--   0        0        0     1317 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/docs/index.md
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/docs/installation.md
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     4185 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      560 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/CMakeLists.txt
+-rw-r--r--   0        0        0      806 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/__init__.py
+-rw-r--r--   0        0        0     3776 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/geometry.hpp
+-rw-r--r--   0        0        0      982 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/geometrymodel.hpp
+-rw-r--r--   0        0        0     8431 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/primitives.hpp
+-rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/thermalmesh.hpp
+-rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/transformations.hpp
+-rw-r--r--   0        0        0     7877 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/trimesh.hpp
+-rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/conanfile.txt.in
+-rw-r--r--   0        0        0     4859 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/prepare-build-backend.py
+-rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/pycanha-core-conan-profile
+-rw-r--r--   0        0        0     1004 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/pycanha-core-wrapper.cpp
+-rw-r--r--   0        0        0     7438 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/src/pycanha_core/pycanha_core.pyi
+-rw-r--r--   0        0        0     2229 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/test/primitives/test_triangle.py
+-rw-r--r--   0        0        0      920 2022-11-09 12:37:21.000000 pycanha_core-0.1.0/PKG-INFO
```

### Comparing `pycanha_core-0.0.3/.github/workflows/build-publish-wheels.yml` & `pycanha_core-0.1.0/.github/workflows/build-publish-wheels.yml`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         with:
           path: pycanha-project/pycanha-core-python
 
       - name: Get version from pyproject.toml and Set Environment Variable
         run: |
           import toml
           pyproject = toml.load('pycanha-project/pycanha-core-python/pyproject.toml')
-          version = pyproject['project']['version']
+          version = ".".join(pyproject['project']['version'].split(".")[:2])
           print(f"::set-output name=version::{version}")
         shell: python
         id: get_version
 
       - name: Check out pycanha-core repo at version
         uses: actions/checkout@v3
         with:
```

### Comparing `pycanha_core-0.0.3/.pytest_cache/v/cache/nodeids` & `pycanha_core-0.1.0/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/LICENSE` & `pycanha_core-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/pyproject.toml` & `pycanha_core-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "prepare-build-backend" # Custom wrapper around scikit_build_core.build See comments in prepare-build-backend.py.
 backend-path = [
     "src/pycanha_core",
 ] #For in-tree builds, we need to add the directory to the path. See: https://peps.python.org/pep-0517/#in-tree-build-backends
 
 [project]
 name = "pycanha-core"
-version = "0.0.3"
+version = "0.1.0"
 description = "Python bindings for pycanha-core with Pybind11"
 readme = "README.md"
 authors = [{ name = "Javier Piqueras Carreño", email = "javier.piqueras@upm.es" }]
 requires-python = ">=3.11"
 classifiers = [
     #Add licence classifiers
     #Add development status classifiers
@@ -26,14 +26,15 @@
 [project.urls]
 "Homepage" = "https://github.com/pycanha-project/pycanha-core-python"
 "Bug Tracker" = "https://github.com/pycanha-project/pycanha-core-python/issues"
 
 [project.optional-dependencies]
 test = ["pytest"]
 build = ["build"]
+docs = ["sphinx", "myst-parser", "sphinx-autoapi"]
 
 [tool.scikit-build]
 cmake.version = ">=3.25"
 ninja.version = ">=1.5"
 
 # Fallback on gmake/make if available and ninja is missing (Unix). Will only
 # fallback on platforms without a known ninja wheel.
```

### Comparing `pycanha_core-0.0.3/src/pycanha_core/CMakeLists.txt` & `pycanha_core-0.1.0/src/pycanha_core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/__init__.py` & `pycanha_core-0.1.0/src/pycanha_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/geometry.hpp` & `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/geometry.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/geometrymodel.hpp` & `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/geometrymodel.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/primitives.hpp` & `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/primitives.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/thermalmesh.hpp` & `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/thermalmesh.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/transformations.hpp` & `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/transformations.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/bindings/gmm/trimesh.hpp` & `pycanha_core-0.1.0/src/pycanha_core/bindings/gmm/trimesh.hpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/conanfile.txt.in` & `pycanha_core-0.1.0/src/pycanha_core/conanfile.txt.in`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/prepare-build-backend.py` & `pycanha_core-0.1.0/src/pycanha_core/prepare-build-backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 # Import the hooks from scikit-build-core that will be called by pip
 from scikit_build_core.build import *
 import subprocess
 
 # Get version of the bindings from pyproject.toml
 import toml
 
-bindings_version_str = toml.load("pyproject.toml")["project"]["version"]
+pyproject = toml.load("pyproject.toml")
+bindings_version_str = ".".join(pyproject["project"]["version"].split(".")[:2])
 
 # Configure the binding version in conanfile.txt (of the bindings)
 with open("src/pycanha_core/conanfile.txt.in", "r") as file:
     conanfile_txt_in = file.read()
     conanfile_txt = conanfile_txt_in.replace(
         "@CONFIG_PYCANHA_CORE_VERSION@", bindings_version_str
     )
@@ -35,15 +36,15 @@
 # Read ../pycanha-core/conanfile.py
 import re
 
 try:
     with open("../pycanha-core/conanfile.py", "r") as file:
         conanfile_content = file.read()
         pycanha_core_version = re.search(
-            r'version\s*=\s*"(\d+\.\d+\.\d+)"', conanfile_content
+            r'version\s*=\s*"(\d+\.\d+)"', conanfile_content
         )
 
         # Check binding version is the same as pycanha-core version
         if pycanha_core_version is None:
             raise RuntimeError(
                 f"Could not find version in pycanha-core/conanfile.py. Required version is {bindings_version_str}"
             )
```

### Comparing `pycanha_core-0.0.3/src/pycanha_core/pycanha-core-conan-profile` & `pycanha_core-0.1.0/src/pycanha_core/pycanha-core-conan-profile`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/pycanha-core-wrapper.cpp` & `pycanha_core-0.1.0/src/pycanha_core/pycanha-core-wrapper.cpp`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/src/pycanha_core/pycanha_core.pyi` & `pycanha_core-0.1.0/src/pycanha_core/pycanha_core.pyi`

 * *Files identical despite different names*

### Comparing `pycanha_core-0.0.3/test/primitives/test_triangle.py` & `pycanha_core-0.1.0/test/primitives/test_triangle.py`

 * *Files identical despite different names*

