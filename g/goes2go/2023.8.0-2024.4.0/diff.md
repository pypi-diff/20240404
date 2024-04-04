# Comparing `tmp/goes2go-2023.8.0.tar.gz` & `tmp/goes2go-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goes2go-2023.8.0.tar", last modified: Wed Aug 23 05:22:17 2023, max compression
+gzip compressed data, was "goes2go-2024.4.0.tar", last modified: Thu Apr  4 15:06:39 2024, max compression
```

## Comparing `goes2go-2023.8.0.tar` & `goes2go-2024.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 05:22:17.348149 goes2go-2023.8.0/
--rw-r--r--   0 runner    (1001) docker     (999)       69 2023-08-23 05:21:48.000000 goes2go-2023.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 05:22:17.344149 goes2go-2023.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 05:22:17.348149 goes2go-2023.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      746 2023-08-23 05:21:48.000000 goes2go-2023.8.0/.github/workflows/release_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1496 2023-08-23 05:21:48.000000 goes2go-2023.8.0/.github/workflows/tests-python.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2027 2023-08-23 05:21:48.000000 goes2go-2023.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)     1079 2023-08-23 05:21:48.000000 goes2go-2023.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (999)      977 2023-08-23 05:21:48.000000 goes2go-2023.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (999)     1076 2023-08-23 05:21:48.000000 goes2go-2023.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      102 2023-08-23 05:21:48.000000 goes2go-2023.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)    12414 2023-08-23 05:22:17.348149 goes2go-2023.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     9789 2023-08-23 05:21:48.000000 goes2go-2023.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (999)     2393 2023-08-23 05:21:50.000000 goes2go-2023.8.0/environment-dev.yml
--rw-r--r--   0 runner    (1001) docker     (999)      747 2023-08-23 05:21:50.000000 goes2go-2023.8.0/environment-test-conda.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1038 2023-08-23 05:21:50.000000 goes2go-2023.8.0/environment-test.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1362 2023-08-23 05:21:50.000000 goes2go-2023.8.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 05:22:17.348149 goes2go-2023.8.0/goes2go/
--rw-r--r--   0 runner    (1001) docker     (999)     8426 2023-08-23 05:21:50.000000 goes2go-2023.8.0/goes2go/NEW.py
--rw-r--r--   0 runner    (1001) docker     (999)     3105 2023-08-23 05:21:50.000000 goes2go-2023.8.0/goes2go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      166 2023-08-23 05:22:15.000000 goes2go-2023.8.0/goes2go/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)    45030 2023-08-23 05:21:50.000000 goes2go-2023.8.0/goes2go/accessors.py
--rw-r--r--   0 runner    (1001) docker     (999)    21281 2023-08-23 05:21:50.000000 goes2go-2023.8.0/goes2go/data.py
--rw-r--r--   0 runner    (1001) docker     (999)     6710 2023-08-23 05:21:50.000000 goes2go-2023.8.0/goes2go/product_table.txt
--rw-r--r--   0 runner    (1001) docker     (999)    35082 2023-08-23 05:21:50.000000 goes2go-2023.8.0/goes2go/rgb.py
--rw-r--r--   0 runner    (1001) docker     (999)     6947 2023-08-23 05:21:50.000000 goes2go-2023.8.0/goes2go/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 05:22:17.348149 goes2go-2023.8.0/goes2go.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)    12414 2023-08-23 05:22:15.000000 goes2go-2023.8.0/goes2go.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      702 2023-08-23 05:22:17.000000 goes2go-2023.8.0/goes2go.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-23 05:22:15.000000 goes2go-2023.8.0/goes2go.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      302 2023-08-23 05:22:15.000000 goes2go-2023.8.0/goes2go.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        8 2023-08-23 05:22:15.000000 goes2go-2023.8.0/goes2go.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)     2372 2023-08-23 05:21:50.000000 goes2go-2023.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)        9 2023-08-23 05:21:50.000000 goes2go-2023.8.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (999)      139 2023-08-23 05:21:50.000000 goes2go-2023.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-23 05:22:17.348149 goes2go-2023.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 05:22:17.348149 goes2go-2023.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 05:21:50.000000 goes2go-2023.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1021 2023-08-23 05:21:50.000000 goes2go-2023.8.0/tests/test_GOES.py
--rw-r--r--   0 runner    (1001) docker     (999)      302 2023-08-23 05:21:50.000000 goes2go-2023.8.0/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (999)     2756 2023-08-23 05:21:50.000000 goes2go-2023.8.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (999)      332 2023-08-23 05:21:50.000000 goes2go-2023.8.0/tests/test_glm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:39.369245 goes2go-2024.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 15:06:20.000000 goes2go-2024.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:39.361245 goes2go-2024.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:39.365245 goes2go-2024.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-04 15:06:20.000000 goes2go-2024.4.0/.github/workflows/release_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 15:06:20.000000 goes2go-2024.4.0/.github/workflows/tests-python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-04 15:06:20.000000 goes2go-2024.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 15:06:20.000000 goes2go-2024.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-04 15:06:20.000000 goes2go-2024.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-04 15:06:20.000000 goes2go-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 15:06:20.000000 goes2go-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-04-04 15:06:39.369245 goes2go-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-04-04 15:06:20.000000 goes2go-2024.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-04 15:06:22.000000 goes2go-2024.4.0/environment-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-04 15:06:22.000000 goes2go-2024.4.0/environment-test-conda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-04 15:06:22.000000 goes2go-2024.4.0/environment-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-04 15:06:22.000000 goes2go-2024.4.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:39.365245 goes2go-2024.4.0/goes2go/
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-04-04 15:06:22.000000 goes2go-2024.4.0/goes2go/NEW.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-04 15:06:22.000000 goes2go-2024.4.0/goes2go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-04 15:06:37.000000 goes2go-2024.4.0/goes2go/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45042 2024-04-04 15:06:22.000000 goes2go-2024.4.0/goes2go/accessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21268 2024-04-04 15:06:22.000000 goes2go-2024.4.0/goes2go/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-04 15:06:22.000000 goes2go-2024.4.0/goes2go/product_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35323 2024-04-04 15:06:22.000000 goes2go-2024.4.0/goes2go/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-04 15:06:22.000000 goes2go-2024.4.0/goes2go/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:39.369245 goes2go-2024.4.0/goes2go.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13377 2024-04-04 15:06:37.000000 goes2go-2024.4.0/goes2go.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-04 15:06:39.000000 goes2go-2024.4.0/goes2go.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:06:37.000000 goes2go-2024.4.0/goes2go.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 15:06:37.000000 goes2go-2024.4.0/goes2go.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 15:06:37.000000 goes2go-2024.4.0/goes2go.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-04 15:06:22.000000 goes2go-2024.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 15:06:22.000000 goes2go-2024.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 15:06:22.000000 goes2go-2024.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:06:39.369245 goes2go-2024.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:39.369245 goes2go-2024.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:06:22.000000 goes2go-2024.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-04 15:06:22.000000 goes2go-2024.4.0/tests/test_GOES.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-04 15:06:22.000000 goes2go-2024.4.0/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-04 15:06:22.000000 goes2go-2024.4.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-04 15:06:22.000000 goes2go-2024.4.0/tests/test_glm.py
```

### Comparing `goes2go-2023.8.0/.github/workflows/release_to_pypi.yml` & `goes2go-2024.4.0/.github/workflows/release_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/.github/workflows/tests-python.yml` & `goes2go-2024.4.0/.github/workflows/tests-python.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: Tests (Python)
 
 on:
   push:
-    branches: [ main ]
+    branches: [main]
   pull_request:
-    branches: [ main ]
+    branches: [main]
 
   # Allow job to be triggered manually.
   workflow_dispatch:
 
 # Cancel in-progress jobs when pushing to the same branch.
 concurrency:
   cancel-in-progress: true
@@ -17,15 +17,15 @@
 jobs:
   tests:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: true
       matrix:
         os: ["ubuntu-latest"]
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
         # In order to save resources, only run particular
         # matrix slots on other OS than Linux.
         include:
           - os: "macos-latest"
             python-version: "3.11"
           - os: "windows-latest"
             python-version: "3.11"
@@ -36,31 +36,30 @@
 
     defaults:
       run:
         shell: bash -el {0}
 
     name: Python ${{ matrix.python-version }} on OS ${{ matrix.os }}
     steps:
-
-    - name: Acquire sources
-      uses: actions/checkout@v3
-      with:
-        fetch-depth: 2
-
-    - name: Setup Python
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
-        architecture: x64
-        cache: 'pip'
-        cache-dependency-path: 'setup.cfg'
-
-    - name: Install project
-      run: |
-        pip3 install --requirement=requirements-test.txt
-        pip3 install --editable=.
-
-    - name: Run tests
-      env:
-        TMPDIR: ${{ runner.temp }}
-      run: |
-        pytest
+      - name: Acquire sources
+        uses: actions/checkout@v4
+        with:
+          fetch-depth: 2
+
+      - name: Setup Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+          architecture: x64
+          cache: "pip"
+          cache-dependency-path: "setup.cfg"
+
+      - name: Install project
+        run: |
+          pip3 install --requirement=requirements-test.txt
+          pip3 install --editable=.
+
+      - name: Run tests
+        env:
+          TMPDIR: ${{ runner.temp }}
+        run: |
+          pytest
```

### Comparing `goes2go-2023.8.0/.gitignore` & `goes2go-2024.4.0/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Don't upload ANY NetCDF files
 *.nc
 
 goes2go/_version.py
 
 core.*
 
+.ruff_cache
+
 # Don't upload my sandbox notebooks
 sandbox*.ipynb
 
 # The GLM_FOV_edges.nc file isn't released.
 # I don't have permission to share.
 GLM_FOV_edges.nc
```

### Comparing `goes2go-2023.8.0/.readthedocs.yml` & `goes2go-2024.4.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/CITATION.cff` & `goes2go-2024.4.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/LICENSE` & `goes2go-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/PKG-INFO` & `goes2go-2024.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: goes2go
-Version: 2023.8.0
-Summary: Retrieve GOES-16/17 data from AWS. Also proves some RGB recipes.
+Version: 2024.4.0
+Summary: Retrieve GOES Satellite data from AWS. Also proves some RGB recipes.
 Author-email: "Brian K. Blaylock" <blaylockbk@gmail.com>
 Maintainer-email: "Brian K. Blaylock" <blaylockbk@gmail.com>
 License: MIT License
         
         Copyright (c) 2019-2022 Brian Blaylock
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,47 +30,71 @@
 Project-URL: Documentation, https://goes2go.readthedocs.io/
 Project-URL: Repository, https://github.com/blaylockbk/goes2go
 Project-URL: Changelog, https://github.com/blaylockbk/goes2go/releases
 Project-URL: Bug Tracker, https://github.com/blaylockbk/goes2go/issues
 Keywords: weather,meteorology,satellite,atmosphere,GOES,xarray,AWS,NOAA
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cartopy>=0.22.0
+Requires-Dist: h5netcdf
+Requires-Dist: matplotlib
+Requires-Dist: metpy
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: s3fs>=2023.6.0
+Requires-Dist: toml
+Requires-Dist: xarray
 Provides-Extra: docs
+Requires-Dist: autodocsumm; extra == "docs"
+Requires-Dist: linkify-it-py; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs"
+Requires-Dist: nbconvert; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: recommonmark; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autosummary-accessors; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
+Requires-Dist: sphinx-markdown-tables; extra == "docs"
+Requires-Dist: sphinxcontrib-mermaid; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: ruff; extra == "test"
 
 <div
   align="center"
 >
 
 ![](https://github.com/blaylockbk/goes2go/blob/main/docs/_static/goes2go_logo_100dpi.png?raw=true)
 
 # Download and display GOES-East and GOES-West data
 
 <!-- Badges -->
 
 [![](https://img.shields.io/pypi/v/goes2go)](https://pypi.python.org/pypi/goes2go/)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/goes2go.svg)](https://anaconday.org/conda-forge/goes2go)
 [![DOI](https://zenodo.org/badge/296737878.svg)](https://zenodo.org/badge/latestdoi/296737878)
 
 ![](https://img.shields.io/github/license/blaylockbk/goes2go)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Tests (Python)](https://github.com/blaylockbk/goes2g0/actions/workflows/tests-python.yml/badge.svg)](https://github.com/blaylockbk/goes2g0/actions/workflows/tests-python.yml)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Tests (Python)](https://github.com/blaylockbk/goes2go/actions/workflows/tests-python.yml/badge.svg)](https://github.com/blaylockbk/goes2go/actions/workflows/tests-python.yml)
 [![Documentation Status](https://readthedocs.org/projects/goes2go/badge/?version=latest)](https://goes2go.readthedocs.io/?badge=latest)
 [![Python](https://img.shields.io/pypi/pyversions/goes2go.svg)](https://pypi.org/project/goes2go/)
 [![Conda Recipe](https://img.shields.io/badge/recipe-goes2go-green.svg)](https://anaconda.org/conda-forge/goes2go)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
 [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
 
 <!--(Badges)-->
@@ -203,15 +227,15 @@
 
    # Download recent data for a specific interval
    G.timerange(recent='30min')
 ```
 
 ## RGB Recipes
 
-The `rgb` xarray accessor computes various RGB products from a GOES ABI ***ABI-L2-MCMIP*** (multi-channel cloud and moisture imagry products) `xarray.Dataset`. See the [demo](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/DEMO_rgb_recipes.html#) for more examples of RGB products.
+The `rgb` xarray accessor computes various RGB products from a GOES ABI **_ABI-L2-MCMIP_** (multi-channel cloud and moisture imagry products) `xarray.Dataset`. See the [demo](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/DEMO_rgb_recipes.html#) for more examples of RGB products.
 
 ```python
 import matplotlib.pyplot as plt
 ds = GOES().latest()
 ax = plt.subplot(projection=ds.rgb.crs)
 ax.imshow(ds.rgb.TrueColor(), **ds.rgb.imshow_kwargs)
 ax.coastlines()
@@ -263,14 +287,15 @@
 
 👨🏻‍💻 [Contributing Guidelines](https://goes2go.readthedocs.io/en/latest/user_guide/contribute.html)  
 💬 [GitHub Discussions](https://github.com/blaylockbk/goes2go/discussions)  
 🚑 [GitHub Issues](https://github.com/blaylockbk/goes2go/issues)  
 🌐 [Personal Webpage](http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/home.html)
 
 P.S. If you like GOES-2-go, check out my other python packages
+
 - [🏁 Herbie](https://github.com/blaylockbk/Herbie): download numerical weather model data
 - [🌡️ SynopticPy](https://github.com/blaylockbk/SynopticPy): retrieve mesonet data from the Synoptic API.
 - [🌹 Pandas-rose](https://github.com/blaylockbk/pandas-rose): easly wind rose from Pandas dataframe.
 
 # Related Content
 
 - [🙋🏻‍♂️ Brian's AWS GOES Web Downloader](https://home.chpc.utah.edu/~u0553130/Brian_Blaylock/cgi-bin/goes16_download.cgi)
```

### Comparing `goes2go-2023.8.0/README.md` & `goes2go-2024.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 ![](https://github.com/blaylockbk/goes2go/blob/main/docs/_static/goes2go_logo_100dpi.png?raw=true)
 
 # Download and display GOES-East and GOES-West data
 
 <!-- Badges -->
 
 [![](https://img.shields.io/pypi/v/goes2go)](https://pypi.python.org/pypi/goes2go/)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/goes2go.svg)](https://anaconday.org/conda-forge/goes2go)
 [![DOI](https://zenodo.org/badge/296737878.svg)](https://zenodo.org/badge/latestdoi/296737878)
 
 ![](https://img.shields.io/github/license/blaylockbk/goes2go)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Tests (Python)](https://github.com/blaylockbk/goes2g0/actions/workflows/tests-python.yml/badge.svg)](https://github.com/blaylockbk/goes2g0/actions/workflows/tests-python.yml)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Tests (Python)](https://github.com/blaylockbk/goes2go/actions/workflows/tests-python.yml/badge.svg)](https://github.com/blaylockbk/goes2go/actions/workflows/tests-python.yml)
 [![Documentation Status](https://readthedocs.org/projects/goes2go/badge/?version=latest)](https://goes2go.readthedocs.io/?badge=latest)
 [![Python](https://img.shields.io/pypi/pyversions/goes2go.svg)](https://pypi.org/project/goes2go/)
 [![Conda Recipe](https://img.shields.io/badge/recipe-goes2go-green.svg)](https://anaconda.org/conda-forge/goes2go)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
 [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
 
 <!--(Badges)-->
@@ -151,15 +151,15 @@
 
    # Download recent data for a specific interval
    G.timerange(recent='30min')
 ```
 
 ## RGB Recipes
 
-The `rgb` xarray accessor computes various RGB products from a GOES ABI ***ABI-L2-MCMIP*** (multi-channel cloud and moisture imagry products) `xarray.Dataset`. See the [demo](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/DEMO_rgb_recipes.html#) for more examples of RGB products.
+The `rgb` xarray accessor computes various RGB products from a GOES ABI **_ABI-L2-MCMIP_** (multi-channel cloud and moisture imagry products) `xarray.Dataset`. See the [demo](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/DEMO_rgb_recipes.html#) for more examples of RGB products.
 
 ```python
 import matplotlib.pyplot as plt
 ds = GOES().latest()
 ax = plt.subplot(projection=ds.rgb.crs)
 ax.imshow(ds.rgb.TrueColor(), **ds.rgb.imshow_kwargs)
 ax.coastlines()
@@ -211,14 +211,15 @@
 
 👨🏻‍💻 [Contributing Guidelines](https://goes2go.readthedocs.io/en/latest/user_guide/contribute.html)  
 💬 [GitHub Discussions](https://github.com/blaylockbk/goes2go/discussions)  
 🚑 [GitHub Issues](https://github.com/blaylockbk/goes2go/issues)  
 🌐 [Personal Webpage](http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/home.html)
 
 P.S. If you like GOES-2-go, check out my other python packages
+
 - [🏁 Herbie](https://github.com/blaylockbk/Herbie): download numerical weather model data
 - [🌡️ SynopticPy](https://github.com/blaylockbk/SynopticPy): retrieve mesonet data from the Synoptic API.
 - [🌹 Pandas-rose](https://github.com/blaylockbk/pandas-rose): easly wind rose from Pandas dataframe.
 
 # Related Content
 
 - [🙋🏻‍♂️ Brian's AWS GOES Web Downloader](https://home.chpc.utah.edu/~u0553130/Brian_Blaylock/cgi-bin/goes16_download.cgi)
```

### Comparing `goes2go-2023.8.0/environment-dev.yml` & `goes2go-2024.4.0/environment-dev.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/environment-test-conda.yml` & `goes2go-2024.4.0/environment-test-conda.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/environment-test.yml` & `goes2go-2024.4.0/environment-test.yml`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/environment.yml` & `goes2go-2024.4.0/environment.yml`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   - s3fs>=2023.6.0
   - toml
   - xarray
 
   # -------------------
   # Formatter & Testing
   # -------------------
+  - ruff
   - black
   - black-jupyter
   - isort
   - pytest
 
   - pip:
       # Borrow some tools from my garage
```

### Comparing `goes2go-2023.8.0/goes2go/NEW.py` & `goes2go-2024.4.0/goes2go/NEW.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,26 @@
 GOES Class
 ==========
 """
 
 import itertools
 import logging
 import re
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import s3fs
 import toml
 
 from goes2go import config
 from goes2go.data import _goes_file_df, goes_latest, goes_nearesttime, goes_timerange
 
 log = logging.getLogger(__name__)
 
-# Location of tables directory
-from pathlib import Path
-
 tables_dir = Path(__file__).parent
 
 # Connect to AWS public buckets
 fs = s3fs.S3FileSystem(anon=True)
 
 product_table = pd.read_csv(
     tables_dir / "product_table.txt",
@@ -36,24 +34,26 @@
     index_col=0,
 )
 product_table.index = product_table.index.str.strip()
 product_table["description"] = product_table.description.str.strip()
 
 
 # Assume goes17 and goes18 have same products as goes16
-_product = {i.split("/")[-1] for i in fs.ls(f"noaa-goes16")}
+_product = {i.split("/")[-1] for i in fs.ls("noaa-goes16")}
 _product = set(filter(lambda x: x.split(".")[-1] not in ["pdf", "html"], _product))
 _product
 
 # you can be unspecific and request any mesoscale domain (M),
 # or by number (M1, M2)
 _domains = {"F", "C", "M", "M1", "M2"}
 
 
 class GOES:
+    """The GOES satellite class."""
+
     def __init__(
         self,
         satellite=config["timerange"].get("satellite"),
         product=config["timerange"].get("product"),
         domain=config["timerange"].get("domain"),
         bands=None,
         channel=None,
@@ -156,23 +156,23 @@
         if self.product in _product:
             self.description = product_table.loc[self.product].description
         else:
             raise ValueError(f"{self.product} is not an available product.")
 
     def __repr__(self):
         msg = [
-            f"╭───────────────────────────────╌┄┈",
-            f"│ 🌎 GOES Object   ",
-            f"│ ───────────────",
+            "╭───────────────────────────────╌┄┈",
+            "│ 🌎 GOES Object   ",
+            "│ ───────────────",
             f"│  {self.satellite=}",
             f"│  {self.product=}",
             f"│  {self.domain=}",
             f"│  {self.bands=}",
             f"│  {self.description=}",
-            f"╰───────────────────────────────╌┄┈",
+            "╰───────────────────────────────╌┄┈",
         ]
         return "\n".join(msg)
 
     def latest(self, **kwargs):
         """Get the latest available GOES data."""
         return goes_latest(
             satellite=self.satellite,
```

### Comparing `goes2go-2023.8.0/goes2go/accessors.py` & `goes2go-2024.4.0/goes2go/accessors.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 from shapely.geometry import Point, Polygon
 
 
 ########################
 # Image Processing Tools
 def _gamma_correction(a, gamma, verbose=False):
     """
-    Darken or lighten an image with `gamma correction
+    Darken or lighten an image with `gamma correction.
+
     <https://en.wikipedia.org/wiki/_gamma_correction>`_.
 
     Parameters
     ----------
     a : array-like
         An array of values, typically the RGB array of values in
         an image.
@@ -137,22 +138,22 @@
             sweep_axis="x",
         )
 
         return crs
 
     @property
     def x(self):
-        """x sweep in crs units (m); x * sat_height"""
+        """The x sweep in crs units (m); x * sat_height."""
         if self._x is None:
             self._x = self._obj.x * self._sat_h
         return self._x
 
     @property
     def y(self):
-        """y sweep in crs units (m); x * sat_height"""
+        """The y sweep in crs units (m); x * sat_height."""
         if self._y is None:
             self._y = self._obj.y * self._sat_h
         return self._y
 
     @property
     def imshow_kwargs(self):
         """Key word arguments for plt.imshow for generating images.
@@ -170,15 +171,15 @@
                 transform=self._crs,
                 origin="upper",
                 interpolation="none",
             )
         return self._imshow_kwargs
 
     def get_latlon(self):
-        """Get lat/lon of all points"""
+        """Get lat/lon of all points."""
         X, Y = np.meshgrid(self.x, self.y)
         a = ccrs.PlateCarree().transform_points(self._crs, X, Y)
         lons, lats, _ = a[:, :, 0], a[:, :, 1], a[:, :, 2]
 
         self._obj.coords["longitude"] = (("y", "x"), lons)
         self._obj.coords["latitude"] = (("y", "x"), lats)
         return self._obj["latitude"], self._obj["longitude"]
@@ -271,43 +272,45 @@
         FOV_domain = Polygon(dom_border * sat_height)
         FOV_domain = FOV_domain.intersection(self.full_disk)
         return FOV_domain
 
 
 @xr.register_dataset_accessor("rgb")
 class rgbAccessor:
+    """An accessor to create RGB composites."""
+
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
         assert (
             self._obj.title == "ABI L2 Cloud and Moisture Imagery"
         ), "Dataset must be an ABI L2 Cloud and Moisture Imagery file."
         self._crs = None
         self._x = None
         self._y = None
         self._sat_h = self._obj.goes_imager_projection.perspective_point_height
         self._imshow_kwargs = None
 
     @property
     def crs(self):
-        """Cartopy coordinate reference system"""
+        """Cartopy coordinate reference system."""
         if self._crs is None:
             # Why am I doing this? To cache the values.
             self._crs = self._obj.FOV.crs
         return self._crs
 
     @property
     def x(self):
-        """x sweep in crs units (m); x * sat_height"""
+        """The x sweep in crs units (m); x * sat_height."""
         if self._x is None:
             self._x = self._obj.x * self._sat_h
         return self._x
 
     @property
     def y(self):
-        """y sweep in crs units (m); x * sat_height"""
+        """The y sweep in crs units (m); x * sat_height."""
         if self._y is None:
             self._y = self._obj.y * self._sat_h
         return self._y
 
     @property
     def imshow_kwargs(self):
         """Key word arguments for plt.imshow for generating images.
@@ -325,27 +328,28 @@
                 transform=self._crs,
                 origin="upper",
                 interpolation="none",
             )
         return self._imshow_kwargs
 
     def get_latlon(self):
-        """Get lat/lon of all points"""
+        """Get lat/lon of all points."""
         X, Y = np.meshgrid(self.x, self.y)
         a = ccrs.PlateCarree().transform_points(self._crs, X, Y)
         lons, lats, _ = a[:, :, 0], a[:, :, 1], a[:, :, 2]
 
         self._obj.coords["longitude"] = (("y", "x"), lons)
         self._obj.coords["latitude"] = (("y", "x"), lats)
         return self._obj["latitude"], self._obj["longitude"]
 
     ####################################################################
     # Helpers
     def _load_RGB_channels(self, channels):
-        """
+        """Load the specified RGB channels.
+
         Return the R, G, and B arrays for the three channels requested. This
         function will convert the data any units in Kelvin to Celsius.
 
         Parameters
         ----------
         channels : tuple of size 3
             A tuple of the channel number for each (R, G, B).
@@ -369,16 +373,16 @@
             else:
                 RGB.append(ds["CMI_C%02d" % c].data)
         return RGB
 
     ####################################################################
     # RGB Recipes
     def TrueColor(self, gamma=2.2, pseudoGreen=True, night_IR=True):
-        """
-        True Color RGB:
+        """Create a True Color RGB.
+
         (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
 
         This is similar to the NaturalColor RGB, but uses a different gamma
         correction and does not apply contrast stretching. I think these
         images look a little "washed out" when compared to the NaturalColor
         RGB. So, I would recommend using the NaturalColor RGB.
 
@@ -449,16 +453,17 @@
             "Quick Guide"
         ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf"
         ds["TrueColor"].attrs["long_name"] = "True Color"
 
         return ds["TrueColor"]
 
     def NaturalColor(self, gamma=0.8, pseudoGreen=True, night_IR=False):
-        """
-        Natural Color RGB based on CIMSS method. Thanks Rick Kohrs!
+        """Create a Natural Color RGB based on CIMSS method.
+
+        Thanks Rick Kohrs!
         (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf>`__ for reference)
 
         Check out Rick Kohrs `merged GOES images <https://www.ssec.wisc.edu/~rickk/local-noon.html>`_.
 
         This NaturalColor RGB is *very* similar to the TrueColor RGB but
         uses slightly different contrast stretches and ranges.
 
@@ -485,16 +490,17 @@
             so that cold clouds show up at night. (Be aware that some
             daytime clouds might appear brighter).
 
         """
         ds = self._obj
 
         def breakpoint_stretch(C, breakpoint):
-            """
-            Contrast stretching by break point (number provided by Rick Kohrs)
+            """Contrast stretching by break point.
+
+            (number provided by Rick Kohrs).
             """
             lower = _normalize(C, 0, 10)  # Low end
             upper = _normalize(C, 10, 255)  # High end
 
             # Combine the two datasets
             # This works because if upper=1 and lower==.7, then
             # that means the upper value was out of range and the
@@ -552,16 +558,16 @@
             "Quick Guide"
         ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_CIMSSRGB_v2.pdf"
         ds["NaturalColor"].attrs["long_name"] = "Natural Color"
 
         return ds["NaturalColor"]
 
     def FireTemperature(self):
-        """
-        Fire Temperature RGB:
+        """Create the Fire Temperature RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Fire_Temperature_RGB.pdf>`__ for reference)
 
         .. image:: /_static/FireTemperature.png
 
 
         """
         ds = self._obj
@@ -588,16 +594,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Fire_Temperature_RGB.pdf"
         ds["FireTemperature"].attrs["long_name"] = "Fire Temperature"
 
         return ds["FireTemperature"]
 
     def AirMass(self):
-        """
-        Air Mass RGB:
+        """Create the Air Mass RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_AirMassRGB_final.pdf>`__ for reference)
 
         .. image:: /_static/AirMass.png
 
 
         """
         ds = self._obj
@@ -622,18 +628,18 @@
         ds["rgb"] = ["R", "G", "B"]
         ds["AirMass"].attrs[
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_AirMassRGB_final.pdf"
         ds["AirMass"].attrs["long_name"] = "Air Mass"
 
         return ds["AirMass"]
-    
+
     def AirMassTropical(self):
-        """
-        Air Mass Tropical RGB:
+        """Create the Air Mass Tropical RGB.
+
         (See `Quick Guide <https://www.eumetsat.int/media/43301>`__ for reference)
 
         .. image:: /_static/AirMassTropical.png
 
 
         """
         ds = self._obj
@@ -643,53 +649,52 @@
         G = ds["CMI_C12"].data - ds["CMI_C13"].data
         B = ds["CMI_C08"].data - 273.15  # remember to convert to Celsius
 
         # _normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
         R = _normalize(R, -25, 5)
         G = _normalize(G, -30, 25)
         B = _normalize(B, -83, -30)
-            
-        # Invert B 
+
+        # Invert B
         B = 1 - B
-            
+
         # Apply the gamma correction to Red channel.
         #   corrected_value = value^(1/gamma)
-        gamma = .5
+        gamma = 0.5
         G = _gamma_correction(G, gamma)
-            
+
         # The final RGB array :)
-        RGB = np.dstack([R, G, B]) 
-        
+        RGB = np.dstack([R, G, B])
+
         ds["AirMassTropical"] = (("y", "x", "rgb"), RGB)
-        ds["rgb"] = ["R", "G", "B"] 
+        ds["rgb"] = ["R", "G", "B"]
         ds["AirMassTropical"].attrs[
             "Quick Guide"
         ] = "https://www.eumetsat.int/media/43301"
         ds["AirMassTropical"].attrs["long_name"] = "Air Mass Tropical"
-        
+
         return ds["AirMassTropical"]
-    
+
     def AirMassTropicalPac(self):
-        """
-        Air Mass Tropical Pac RGB:
+        """Create the Air Mass Tropical Pac RGB.
+
         (See `Blog Write-up <https://cimss.ssec.wisc.edu/satellite-blog/archives/51777>`__ for reference)
-        
+
         .. image:: /_static/AirMassTropicalPac.png
-        
 
         """
         ds = self._obj
-        
+
         # Load the three channels into appropriate R, G, and B variables
         R = ds["CMI_C08"].data - ds["CMI_C10"].data
         G = ds["CMI_C12"].data - ds["CMI_C13"].data
         B = ds["CMI_C08"].data - 273.15  # remember to convert to Celsius
-        
+
         # _normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
-        R = _normalize(R, -26.2, .6)
+        R = _normalize(R, -26.2, 0.6)
         G = _normalize(G, -26.2, 27.4)
         B = _normalize(B, -64.45, -29.25)
 
         # Invert B
         B = 1 - B
 
         # The final RGB array :)
@@ -701,16 +706,16 @@
             "Quick Guide"
         ] = "https://cimss.ssec.wisc.edu/satellite-blog/archives/51777"
         ds["AirMassTropicalPac"].attrs["long_name"] = "Air Mass Tropical Pac"
 
         return ds["AirMassTropicalPac"]
 
     def DayCloudPhase(self):
-        """
-        Day Cloud Phase Distinction RGB:
+        """Create the Day Cloud Phase Distinction RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Day_Cloud_Phase_Distinction.pdf>`__ for reference)
 
         .. image:: /_static/DayCloudPhase.png
 
 
         """
         ds = self._obj
@@ -735,16 +740,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Day_Cloud_Phase_Distinction.pdf"
         ds["DayCloudPhase"].attrs["long_name"] = "Day Cloud Phase"
 
         return ds["DayCloudPhase"]
 
     def DayConvection(self):
-        """
-        Day Convection RGB:
+        """Create the Day Convection RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayConvectionRGB_final.pdf>`__ for reference)
 
         .. image:: /_static/DayConvection.png
 
 
         """
         ds = self._obj
@@ -769,16 +774,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayConvectionRGB_final.pdf"
         ds["DayConvection"].attrs["long_name"] = "Day Convection"
 
         return ds["DayConvection"]
 
     def DayCloudConvection(self):
-        """
-        Day Cloud Convection RGB:
+        """Create the Day Cloud Convection RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DayCloudConvectionRGB_final.pdf>`__ for reference)
 
         .. image:: /_static/DayCloudConvection.png
 
         """
         ds = self._obj
 
@@ -808,16 +813,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DayCloudConvectionRGB_final.pdf"
         ds["DayCloudConvection"].attrs["long_name"] = "Day Cloud Convection"
 
         return ds["DayCloudConvection"]
 
     def DayLandCloud(self):
-        """
-        Day Land Cloud Fire RGB:
+        """Create the Day Land Cloud Fire RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_daylandcloudRGB_final.pdf>`__ for reference)
 
         .. image:: /_static/DayLandCloud.png
 
 
         """
         ds = self._obj
@@ -839,16 +844,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_daylandcloudRGB_final.pdf"
         ds["DayLandCloud"].attrs["long_name"] = "Day Land Cloud"
 
         return ds["DayLandCloud"]
 
     def DayLandCloudFire(self):
-        """
-        Day Land Cloud Fire RGB:
+        """Create the Day Land Cloud Fire RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayLandCloudFireRGB_final.pdf>`__ for reference)
 
         .. image:: /_static/DayLandCloudFire.png
 
 
         """
         ds = self._obj
@@ -870,16 +875,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DayLandCloudFireRGB_final.pdf"
         ds["DayLandCloudFire"].attrs["long_name"] = "Day Land Cloud Fire"
 
         return ds["DayLandCloudFire"]
 
     def WaterVapor(self):
-        """
-        Simple Water Vapor RGB:
+        """Create the Simple Water Vapor RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Simple_Water_Vapor_RGB.pdf>`__ for reference)
 
         .. image:: /_static/WaterVapor.png
 
 
         """
         ds = self._obj
@@ -906,16 +911,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Simple_Water_Vapor_RGB.pdf"
         ds["WaterVapor"].attrs["long_name"] = "Water Vapor"
 
         return ds["WaterVapor"]
 
     def DifferentialWaterVapor(self):
-        """
-        Differential Water Vapor RGB:
+        """Differential Water Vapor RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DifferentialWaterVaporRGB_final.pdf>`__ for reference)
 
         .. image:: /_static/DifferentialWaterVapor.png
 
 
         """
         ds = self._obj
@@ -949,16 +954,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_DifferentialWaterVaporRGB_final.pdf"
         ds["DifferentialWaterVapor"].attrs["long_name"] = "Differential Water Vapor"
 
         return ds["DifferentialWaterVapor"]
 
     def DaySnowFog(self):
-        """
-        Day Snow-Fog RGB:
+        """Day Snow-Fog RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DaySnowFog.pdf>`__ for reference)
 
         .. image:: /_static/DaySnowFog.png
 
 
         """
         ds = self._obj
@@ -988,16 +993,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_DaySnowFog.pdf"
         ds["DaySnowFog"].attrs["long_name"] = "Day Snow Fog"
 
         return ds["DaySnowFog"]
 
     def NighttimeMicrophysics(self):
-        """
-        Nighttime Microphysics RGB:
+        """Create the Nighttime Microphysics RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_NtMicroRGB_final.pdf>`__ for reference)
 
         .. image:: /_static/NighttimeMicrophysics.png
 
 
         """
         ds = self._obj
@@ -1021,16 +1026,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/QuickGuide_GOESR_NtMicroRGB_final.pdf"
         ds["NighttimeMicrophysics"].attrs["long_name"] = "Nighttime Microphysics"
 
         return ds["NighttimeMicrophysics"]
 
     def Dust(self):
-        """
-        SulfurDioxide RGB:
+        """Create the SulfurDioxide RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Dust_RGB_Quick_Guide.pdf>`__ for reference)
 
         .. image:: /_static/Dust.png
 
 
         """
         ds = self._obj
@@ -1058,16 +1063,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Dust_RGB_Quick_Guide.pdf"
         ds["Dust"].attrs["long_name"] = "Dust"
 
         return ds["Dust"]
 
     def SulfurDioxide(self):
-        """
-        SulfurDioxide RGB:
+        """Create the SulfurDioxide RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/Quick_Guide_SO2_RGB.pdf>`__ for reference)
 
         .. image:: /_static/SulfurDioxide.png
 
 
         """
         ds = self._obj
@@ -1091,16 +1096,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/Quick_Guide_SO2_RGB.pdf"
         ds["SulfurDioxide"].attrs["long_name"] = "Sulfur Dioxide"
 
         return ds["SulfurDioxide"]
 
     def Ash(self):
-        """
-        Ash RGB:
+        """Create the Ash RGB.
+
         (See `Quick Guide <http://rammb.cira.colostate.edu/training/visit/quick_guides/GOES_Ash_RGB.pdf>`__ for reference)
 
         .. image:: /_static/Ash.png
 
 
         """
         ds = self._obj
@@ -1124,16 +1129,16 @@
             "Quick Guide"
         ] = "http://rammb.cira.colostate.edu/training/visit/quick_guides/GOES_Ash_RGB.pdf"
         ds["Ash"].attrs["long_name"] = "Ash"
 
         return ds["Ash"]
 
     def SplitWindowDifference(self):
-        """
-        Split Window Difference RGB (greyscale):
+        """Split Window Difference RGB (greyscale).
+
         (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_SplitWindowDifference.pdf>`__ for reference)
 
         .. image:: /_static/SplitWindowDifference.png
 
 
         """
         ds = self._obj
@@ -1153,16 +1158,16 @@
             "Quick Guide"
         ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_SplitWindowDifference.pdf"
         ds["SplitWindowDifference"].attrs["long_name"] = "Split Window Difference"
 
         return ds["SplitWindowDifference"]
 
     def NightFogDifference(self):
-        """
-        Night Fog Difference RGB (greyscale):
+        """Night Fog Difference RGB (greyscale).
+
         (See `Quick Guide <http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_NightFogBTD.pdf>`__ for reference)
 
         .. image:: /_static/NightFogDifference.png
 
 
         """
         ds = self._obj
@@ -1185,16 +1190,15 @@
             "Quick Guide"
         ] = "http://cimss.ssec.wisc.edu/goes/OCLOFactSheetPDFs/ABIQuickGuide_NightFogBTD.pdf"
         ds["NightFogDifference"].attrs["long_name"] = "NightFogDifference"
 
         return ds["NightFogDifference"]
 
     def RocketPlume(self, night=False):
-        """
-        Rocket Plume RGB
+        """Create the  Rocket Plume RGB.
 
         For identifying rocket launches.
 
         See `this blog <https://cimss.ssec.wisc.edu/satellite-blog/archives/41335>`__ and
         the `Quick Guide <https://cimss.ssec.wisc.edu/satellite-blog/images/2021/06/QuickGuide_Template_GOESRBanner_Rocket_Plume.pdf>`__
         for reference
 
@@ -1232,20 +1236,19 @@
             "Quick Guide"
         ] = "https://cimss.ssec.wisc.edu/satellite-blog/images/2021/06/QuickGuide_Template_GOESRBanner_Rocket_Plume.pdf"
         ds["RocketPlume"].attrs["long_name"] = "Rocket Plume"
 
         return ds["RocketPlume"]
 
     def NormalizedBurnRatio(self):
-        """
-        Normalized Burn Ratio
+        """Create the Normalized Burn Ratio.
 
         **THIS FUNCTION IS NOT FULLY DEVELOPED. Need more info.**
 
-        NBR= (0.86 µm – 2.2 µm)/(0.86 um + 2.2 um)
+        NBR= (0.86 µm - 2.2 µm)/(0.86 um + 2.2 um)
 
 
         https://ntrs.nasa.gov/citations/20190030825
 
         """
         warnings.warn(
             "THE `NormalizedBurnRatio` FUNCTION IS NOT FULLY DEVELOPED. NEED MORE INFO."
@@ -1269,35 +1272,32 @@
             "Quick Guide"
         ] = "https://ntrs.nasa.gov/citations/20190030825"
         ds["NormalizedBurnRatio"].attrs["long_name"] = "Normalized Burn Ratio"
 
         return ds["NormalizedBurnRatio"]
 
     def SeaSpray(self, **kwargs):
-        """
-        Sea Spray RGB:
+        """Create the Sea Spray RGB.
+
         (See `Quick Guide <https://rammb.cira.colostate.edu/training/visit/quick_guides/VIIRS_Sea_Spray_RGB_Quick_Guide_v2.pdf>`__ for reference)
 
         .. image:: /_static/SeaSpray.png
 
-        Parameters
-        ----------
         """
-
         ds = self._obj
 
         # Load the three channels into appropriate R, G, and B variables
         R = ds["CMI_C07"].data - ds["CMI_C13"].data
         G = ds["CMI_C03"].data
         B = ds["CMI_C02"].data
 
         # Normalize each channel by the appropriate range of values. e.g. R = (R-minimum)/(maximum-minimum)
         R = _normalize(R, 0, 5)
-        G = _normalize(G, .01, .09) #values for this channel go from 0 to 1.
-        B = _normalize(B, .02, .12) #values for this channel go from o to 1.
+        G = _normalize(G, 0.01, 0.09)  # values for this channel go from 0 to 1.
+        B = _normalize(B, 0.02, 0.12)  # values for this channel go from o to 1.
 
         # Apply a gamma correction to each R, G, B channel
         R = _gamma_correction(R, 1.0)
         G = _gamma_correction(G, 1.67)
         B = _gamma_correction(B, 1.67)
 
         # The final RGB array :)
```

### Comparing `goes2go-2023.8.0/goes2go/data.py` & `goes2go-2024.4.0/goes2go/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,26 +45,25 @@
     "F": ["FULL", "FULLDISK", "FULL DISK"],
     "M": ["MESOSCALE", "M1", "M2"],
 }
 
 _product = {
     # Assume goes17 and goes18 have same products as goes16
     i.split("/")[-1]: []
-    for i in fs.ls(f"noaa-goes16")
+    for i in fs.ls("noaa-goes16")
 }
 _product.pop("index.html", None)
 _product["GLM-L2-LCFA"] = ["GLM"]
 _product["ABI-L2-MCMIPC"] = ["ABIC"]
 _product["ABI-L2-MCMIPF"] = ["ABIF"]
 _product["ABI-L2-MCMIPM"] = ["ABIM"]
 
 
 def _check_param_inputs(**params):
-    """
-    Checks the input parameters for correct name or alias.
+    """Check the input parameters for correct name or alias.
 
     Specifically, check the input for product, domain, and satellite are
     in the list of accepted values. If not, then look if it has an alias.
     """
     # Kinda messy, but gets the job done.
     params.setdefault("verbose", True)
     satellite = params["satellite"]
@@ -92,16 +91,16 @@
             if domain in ["M1", "M2"]:
                 product = product + "M"
             else:
                 for key, aliases in _domain.items():
                     if domain in aliases:
                         domain = key
                 product = product + domain
-        assert (domain in _domain) or (
-            domain in ["M1", "M2"]
+        assert (
+            (domain in _domain) or (domain in ["M1", "M2"])
         ), f"domain must be one of {list(_domain.keys())} or an alias {list(_domain.values())}"
     else:
         domain = None
 
     ## Determine the Product
     if product not in _product:
         for key, aliases in _product.items():
@@ -111,16 +110,15 @@
         product in _product
     ), f"product must be one of {list(_product .keys())} or an alias {list(_product .values())}"
 
     return satellite, product, domain
 
 
 def _goes_file_df(satellite, product, start, end, bands=None, refresh=True):
-    """
-    Get list of requested GOES files as pandas.DataFrame.
+    """Get list of requested GOES files as pandas.DataFrame.
 
     Parameters
     ----------
     satellite : str
     product : str
     start : datetime
     end : datetime
@@ -183,15 +181,15 @@
     for i in params:
         df.attrs[i] = params[i]
 
     return df
 
 
 def _download(df, save_dir, overwrite, max_threads=10, verbose=False):
-    """Download the files from a DataFrame listing with multithreading"""
+    """Download the files from a DataFrame listing with multithreading."""
 
     def do_download(src):
         dst = Path(save_dir) / src
         if not dst.parent.is_dir():
             dst.parent.mkdir(parents=True, exist_ok=True)
         if dst.is_file() and not overwrite:
             if verbose:
@@ -213,15 +211,15 @@
 
     print(
         f"📦 Finished downloading [{len(df)}] files to [{save_dir/Path(df.file[0]).parents[3]}]."
     )
 
 
 def _as_xarray_MP(src, save_dir, i=None, n=None, verbose=True):
-    """Open a file as a xarray.Dataset -- a multiprocessing helper"""
+    """Open a file as a xarray.Dataset -- a multiprocessing helper."""
 
     # File destination
     local_copy = Path(save_dir) / src
 
     if local_copy.is_file():
         if verbose:
             print(
@@ -252,16 +250,15 @@
 
     ds["filename"] = src
 
     return ds
 
 
 def _as_xarray(df, **params):
-    """
-    Download files in the list to the desired path.
+    """Download files in the list to the desired path.
 
     Use multiprocessing to speed up the download process.
 
     Parameters
     ----------
     df : pandas.DataFrame
         A list of files in the GOES s3 bucket.
```

### Comparing `goes2go-2023.8.0/goes2go/product_table.txt` & `goes2go-2024.4.0/goes2go/product_table.txt`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/goes2go/rgb.py` & `goes2go-2024.4.0/goes2go/rgb.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,37 +101,44 @@
       15            12.3 μm        "Dirty" Longwave Window Band                   IR
       16            13.3 μm        "CO2" Longwave infrared                        IR
 =============== ================== ============================================== ======================================
 
 
 """
 
-import numpy as np
-import matplotlib.pyplot as plt
+import warnings
+
 import cartopy.crs as ccrs
+import matplotlib.pyplot as plt
+import numpy as np
 import xarray as xr
 
 from goes2go.tools import field_of_view
 
+warnings.warn(
+    "The rgb module is deprecated. Use the rgb accessor instead. "
+    "See https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/DEMO_rgb_recipes.html for examples.",
+    DeprecationWarning,
+    stacklevel=2,
+)
+
 
 def get_imshow_kwargs(ds):
-    """
-    Help determine the ``plt.imshow`` arguments.
+    r"""Help determine the ``plt.imshow`` arguments.
 
     Parameters
     ----------
     ds : xarray.Dataset
 
     Returns
     -------
     kwargs for the ``plt.imshow`` with the correct image extent limits.
 
     Examples
     --------
-
     .. code:: python
 
         r = TrueColor(G)
         ax = common_features(r.crs)
         ax.imshow(r.TrueColor, *\*\get_imshow_kwargs(r))
 
     """
@@ -207,17 +214,17 @@
     #    )
     # ds.attrs['pcolormesh_kwargs'] = pcolormesh_kwargs
 
     return ds
 
 
 def load_RGB_channels(C, channels):
-    """
-    Return the R, G, and B arrays for the three channels requested. This
-    function will convert the data any units in Kelvin to Celsius.
+    """Return the R, G, and B arrays for the three channels requested.
+
+    This function will convert the data any units in Kelvin to Celsius.
 
     Parameters
     ----------
     C : xarray.Dataset
         The GOES multi-channel file opened with xarray.
     channels : tuple of size 3
         A tuple of the channel number for each (R, G, B).
@@ -238,16 +245,16 @@
             RGB.append(C["CMI_C%02d" % c].data - 273.15)
         else:
             RGB.append(C["CMI_C%02d" % c].data)
     return RGB
 
 
 def gamma_correction(a, gamma, verbose=False):
-    """
-    Darken or lighten an image with `gamma correction
+    """Darken or lighten an image with `gamma correction.
+
     <https://en.wikipedia.org/wiki/Gamma_correction>`_.
 
     Parameters
     ----------
     a : array-like
         An array of values, typically the RGB array of values in
         an image.
```

### Comparing `goes2go-2023.8.0/goes2go/tools.py` & `goes2go-2024.4.0/goes2go/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,18 +56,18 @@
     Returns
     -------
     pFOV_inst is a polygon of the instrument field of view.
     pFOV_dom is a polygon of the domain field of view
     crs is the cartopy coordinate reference system for the instrument
     """
     warnings.warn(
-            "Use the FOV accessor instead `G.FOV.full_disk` or `G.FOV.domain`",
-            DeprecationWarning,
-            stacklevel=2,
-        )
+        "Use the FOV accessor instead `G.FOV.full_disk` or `G.FOV.domain`",
+        DeprecationWarning,
+        stacklevel=2,
+    )
 
     if G.title.startswith("ABI"):
         globe_kwargs = dict(
             semimajor_axis=G.goes_imager_projection.semi_major_axis,
             semiminor_axis=G.goes_imager_projection.semi_minor_axis,
             inverse_flattening=G.goes_imager_projection.inverse_flattening,
         )
@@ -134,15 +134,15 @@
             np.linspace(FOV_radius, -FOV_radius, resolution),
             np.ones(resolution) * -FOV_radius,
         )
         x = np.hstack([side1x, side2x, side3x, side4x])
         y = np.hstack([side1y, side2y, side3y, side4y])
         square_FOV = Polygon(zip(x, y))
         pFOV_inst = pFOV_inst.intersection(square_FOV)
-        pFOV_dom = None # there is no "domain" for the GLM instrument
+        pFOV_dom = None  # there is no "domain" for the GLM instrument
 
     if G.title.startswith("ABI"):
         # We have the global field of view,
         # now we need the domain field of view
         dom_border = np.array(
             [(i, G.y.data[0]) for i in G.x.data]
             + [(G.x.data[-1], i) for i in G.y.data]
```

### Comparing `goes2go-2023.8.0/goes2go.egg-info/PKG-INFO` & `goes2go-2024.4.0/goes2go.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: goes2go
-Version: 2023.8.0
-Summary: Retrieve GOES-16/17 data from AWS. Also proves some RGB recipes.
+Version: 2024.4.0
+Summary: Retrieve GOES Satellite data from AWS. Also proves some RGB recipes.
 Author-email: "Brian K. Blaylock" <blaylockbk@gmail.com>
 Maintainer-email: "Brian K. Blaylock" <blaylockbk@gmail.com>
 License: MIT License
         
         Copyright (c) 2019-2022 Brian Blaylock
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,47 +30,71 @@
 Project-URL: Documentation, https://goes2go.readthedocs.io/
 Project-URL: Repository, https://github.com/blaylockbk/goes2go
 Project-URL: Changelog, https://github.com/blaylockbk/goes2go/releases
 Project-URL: Bug Tracker, https://github.com/blaylockbk/goes2go/issues
 Keywords: weather,meteorology,satellite,atmosphere,GOES,xarray,AWS,NOAA
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cartopy>=0.22.0
+Requires-Dist: h5netcdf
+Requires-Dist: matplotlib
+Requires-Dist: metpy
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: s3fs>=2023.6.0
+Requires-Dist: toml
+Requires-Dist: xarray
 Provides-Extra: docs
+Requires-Dist: autodocsumm; extra == "docs"
+Requires-Dist: linkify-it-py; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs"
+Requires-Dist: nbconvert; extra == "docs"
+Requires-Dist: nbsphinx; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: recommonmark; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinx-autosummary-accessors; extra == "docs"
+Requires-Dist: sphinx-design; extra == "docs"
+Requires-Dist: sphinx-markdown-tables; extra == "docs"
+Requires-Dist: sphinxcontrib-mermaid; extra == "docs"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: ruff; extra == "test"
 
 <div
   align="center"
 >
 
 ![](https://github.com/blaylockbk/goes2go/blob/main/docs/_static/goes2go_logo_100dpi.png?raw=true)
 
 # Download and display GOES-East and GOES-West data
 
 <!-- Badges -->
 
 [![](https://img.shields.io/pypi/v/goes2go)](https://pypi.python.org/pypi/goes2go/)
-[![Conda Version](https://img.shields.io/conda/vn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/goes2go.svg)](https://anaconday.org/conda-forge/goes2go)
 [![DOI](https://zenodo.org/badge/296737878.svg)](https://zenodo.org/badge/latestdoi/296737878)
 
 ![](https://img.shields.io/github/license/blaylockbk/goes2go)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![Tests (Python)](https://github.com/blaylockbk/goes2g0/actions/workflows/tests-python.yml/badge.svg)](https://github.com/blaylockbk/goes2g0/actions/workflows/tests-python.yml)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Tests (Python)](https://github.com/blaylockbk/goes2go/actions/workflows/tests-python.yml/badge.svg)](https://github.com/blaylockbk/goes2go/actions/workflows/tests-python.yml)
 [![Documentation Status](https://readthedocs.org/projects/goes2go/badge/?version=latest)](https://goes2go.readthedocs.io/?badge=latest)
 [![Python](https://img.shields.io/pypi/pyversions/goes2go.svg)](https://pypi.org/project/goes2go/)
 [![Conda Recipe](https://img.shields.io/badge/recipe-goes2go-green.svg)](https://anaconda.org/conda-forge/goes2go)
 [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
 [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/goes2go.svg)](https://anaconda.org/conda-forge/goes2go)
 
 <!--(Badges)-->
@@ -203,15 +227,15 @@
 
    # Download recent data for a specific interval
    G.timerange(recent='30min')
 ```
 
 ## RGB Recipes
 
-The `rgb` xarray accessor computes various RGB products from a GOES ABI ***ABI-L2-MCMIP*** (multi-channel cloud and moisture imagry products) `xarray.Dataset`. See the [demo](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/DEMO_rgb_recipes.html#) for more examples of RGB products.
+The `rgb` xarray accessor computes various RGB products from a GOES ABI **_ABI-L2-MCMIP_** (multi-channel cloud and moisture imagry products) `xarray.Dataset`. See the [demo](https://goes2go.readthedocs.io/en/latest/user_guide/notebooks/DEMO_rgb_recipes.html#) for more examples of RGB products.
 
 ```python
 import matplotlib.pyplot as plt
 ds = GOES().latest()
 ax = plt.subplot(projection=ds.rgb.crs)
 ax.imshow(ds.rgb.TrueColor(), **ds.rgb.imshow_kwargs)
 ax.coastlines()
@@ -263,14 +287,15 @@
 
 👨🏻‍💻 [Contributing Guidelines](https://goes2go.readthedocs.io/en/latest/user_guide/contribute.html)  
 💬 [GitHub Discussions](https://github.com/blaylockbk/goes2go/discussions)  
 🚑 [GitHub Issues](https://github.com/blaylockbk/goes2go/issues)  
 🌐 [Personal Webpage](http://home.chpc.utah.edu/~u0553130/Brian_Blaylock/home.html)
 
 P.S. If you like GOES-2-go, check out my other python packages
+
 - [🏁 Herbie](https://github.com/blaylockbk/Herbie): download numerical weather model data
 - [🌡️ SynopticPy](https://github.com/blaylockbk/SynopticPy): retrieve mesonet data from the Synoptic API.
 - [🌹 Pandas-rose](https://github.com/blaylockbk/pandas-rose): easly wind rose from Pandas dataframe.
 
 # Related Content
 
 - [🙋🏻‍♂️ Brian's AWS GOES Web Downloader](https://home.chpc.utah.edu/~u0553130/Brian_Blaylock/cgi-bin/goes16_download.cgi)
```

### Comparing `goes2go-2023.8.0/goes2go.egg-info/SOURCES.txt` & `goes2go-2024.4.0/goes2go.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/pyproject.toml` & `goes2go-2024.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [project]
 name = "goes2go"
-description = "Retrieve GOES-16/17 data from AWS. Also proves some RGB recipes."
+description = "Retrieve GOES Satellite data from AWS. Also proves some RGB recipes."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = { file = "LICENSE" }
 authors = [{ name = "Brian K. Blaylock", email = "blaylockbk@gmail.com" }]
 maintainers = [{ name = "Brian K. Blaylock", email = "blaylockbk@gmail.com" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
-
 ]
 keywords = [
     "weather",
     "meteorology",
     "satellite",
     "atmosphere",
     "GOES",
@@ -54,37 +53,51 @@
 [project.optional-dependencies]
 docs = [
     "autodocsumm",
     "linkify-it-py",
     "myst-parser",
     "nbconvert",
     "nbsphinx",
+    "sphinx-copybutton",
     "pydata-sphinx-theme",
     "recommonmark",
     "sphinx",
     "sphinx-autosummary-accessors",
     "sphinx-design",
     "sphinx-markdown-tables",
     "sphinxcontrib-mermaid",
 ]
-
-test = ["pytest", "black", "isort"]
+test = ["pytest", "ruff"]
 
 [build-system]
 requires = ["setuptools>=42", "wheel", "setuptools_scm[toml]>=3.4"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["goes2go"]
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
 local_scheme = "no-local-version"
 write_to = "goes2go/_version.py"
 
+[tool.ruff]
+target-version = "py311"
+extend-include = ["*.ipynb"]
+
+[tool.ruff.lint]
+extend-select = [
+    "UP", # pyupgrade
+    "D", # pydocstyle
+
+]
+
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
+
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 minversion = "2.0"
 addopts = "-rsfEX -p pytester --strict-markers --verbosity=3"
 log_level = "DEBUG"
```

### Comparing `goes2go-2023.8.0/tests/test_GOES.py` & `goes2go-2024.4.0/tests/test_GOES.py`

 * *Files identical despite different names*

### Comparing `goes2go-2023.8.0/tests/test_data.py` & `goes2go-2024.4.0/tests/test_data.py`

 * *Files identical despite different names*

