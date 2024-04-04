# Comparing `tmp/jaraco.zstd-1.1.0.tar.gz` & `tmp/jaraco.zstd-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.zstd-1.1.0.tar", last modified: Tue Jun 27 23:59:53 2023, max compression
+gzip compressed data, was "jaraco.zstd-1.1.1.tar", last modified: Thu Apr  4 19:04:44 2024, max compression
```

## Comparing `jaraco.zstd-1.1.0.tar` & `jaraco.zstd-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:59:53.885017 jaraco.zstd-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:59:53.877017 jaraco.zstd-1.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:59:53.877017 jaraco.zstd-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-27 23:59:53.885017 jaraco.zstd-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:59:53.881017 jaraco.zstd-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:59:53.881017 jaraco.zstd-1.1.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/jaraco/zstd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 23:59:53.881017 jaraco.zstd-1.1.0/jaraco.zstd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-27 23:59:53.000000 jaraco.zstd-1.1.0/jaraco.zstd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-27 23:59:53.000000 jaraco.zstd-1.1.0/jaraco.zstd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 23:59:53.000000 jaraco.zstd-1.1.0/jaraco.zstd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-27 23:59:53.000000 jaraco.zstd-1.1.0/jaraco.zstd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 23:59:53.000000 jaraco.zstd-1.1.0/jaraco.zstd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-27 23:59:53.885017 jaraco.zstd-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-27 23:59:31.000000 jaraco.zstd-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:04:44.391260 jaraco.zstd-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:04:44.387260 jaraco.zstd-1.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:04:44.387260 jaraco.zstd-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-04 19:04:44.391260 jaraco.zstd-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:04:44.387260 jaraco.zstd-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:04:44.387260 jaraco.zstd-1.1.1/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/jaraco/zstd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:04:44.387260 jaraco.zstd-1.1.1/jaraco.zstd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-04 19:04:44.000000 jaraco.zstd-1.1.1/jaraco.zstd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 19:04:44.000000 jaraco.zstd-1.1.1/jaraco.zstd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:04:44.000000 jaraco.zstd-1.1.1/jaraco.zstd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 19:04:44.000000 jaraco.zstd-1.1.1/jaraco.zstd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 19:04:44.000000 jaraco.zstd-1.1.1/jaraco.zstd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-04 19:04:44.391260 jaraco.zstd-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:04:44.387260 jaraco.zstd-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/tests/sample.tar.zst
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 19:04:21.000000 jaraco.zstd-1.1.1/tox.ini
```

### Comparing `jaraco.zstd-1.1.0/.github/workflows/main.yml` & `jaraco.zstd-1.1.1/.github/workflows/main.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,98 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
 
 permissions:
   contents: read
 
 env:
-  # Environment variables to support color support (jaraco/skeleton#66):
-  # Request colored output from CLI tools supporting it. Different tools
-  # interpret the value differently. For some, just being set is sufficient.
-  # For others, it must be a non-zero integer. For yet others, being set
-  # to a non-empty value is sufficient. For tox, it must be one of
-  # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
-  # in common is "1".
+  # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
-  # MyPy's color enforcement (must be a non-zero number)
-  MYPY_FORCE_COLOR: -42
-  # Recognized by the `py` package, dependency of `pytest` (must be "1")
-  PY_COLORS: 1
-  # Make tox-wrapped tools see color requests
-  TOX_TESTENV_PASSENV: >-
-    FORCE_COLOR
-    MYPY_FORCE_COLOR
-    NO_COLOR
-    PY_COLORS
-    PYTEST_THEME
-    PYTEST_THEME_MODE
 
   # Suppress noisy pip warnings
   PIP_DISABLE_PIP_VERSION_CHECK: 'true'
   PIP_NO_PYTHON_VERSION_WARNING: 'true'
   PIP_NO_WARN_SCRIPT_LOCATION: 'true'
 
-  # Disable the spinner, noise in GHA; TODO(webknjaz): Fix this upstream
-  # Must be "1".
-  TOX_PARALLEL_NO_SPINNER: 1
+  # Ensure tests can sense settings about the environment
+  TOX_OVERRIDE: >-
+    testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
-        - python: pypy3.9
+        - python: "3.11"
+          platform: ubuntu-latest
+        - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.12' }}
+    continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run tests
+        run: python -m pip install tox
+      - name: Run
         run: tox
 
-  docs:
+  collateral:
+    strategy:
+      fail-fast: false
+      matrix:
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
-    env:
-      TOXENV: docs
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
+        with:
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Run tests
-        run: tox
+        run: python -m pip install tox
+      - name: Eval ${{ matrix.job }}
+        run: tox -e ${{ matrix.job }}
 
   check:  # This job does nothing and is only used for the branch protection
     if: always()
 
     needs:
     - test
-    - docs
+    - collateral
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
@@ -105,20 +103,19 @@
       contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: 3.11-dev
+          python-version: 3.x
       - name: Install tox
-        run: |
-          python -m pip install tox
-      - name: Release
+        run: python -m pip install tox
+      - name: Run
         run: tox -e release
         env:
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `jaraco.zstd-1.1.0/LICENSE` & `jaraco.zstd-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.zstd-1.1.0/README.rst` & `jaraco.zstd-1.1.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 .. image:: https://img.shields.io/pypi/v/jaraco.zstd.svg
    :target: https://pypi.org/project/jaraco.zstd
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.zstd.svg
 
-.. image:: https://github.com/jaraco/jaraco.zstd/workflows/tests/badge.svg
+.. image:: https://github.com/jaraco/jaraco.zstd/actions/workflows/main.yml/badge.svg
    :target: https://github.com/jaraco/jaraco.zstd/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
 ..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 Extract files from a ``.tar.zstd``::
 
     python -m jaraco.zstd --extract filename.tar.zstd
 
 Usage::
```

### Comparing `jaraco.zstd-1.1.0/docs/conf.py` & `jaraco.zstd-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.zstd-1.1.0/jaraco/zstd.py` & `jaraco.zstd-1.1.1/jaraco/zstd.py`

 * *Files identical despite different names*

### Comparing `jaraco.zstd-1.1.0/setup.cfg` & `jaraco.zstd-1.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -9,41 +9,30 @@
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find_namespace:
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
 	zstandard
 
-[options.packages.find]
-exclude = 
-	build*
-	dist*
-	docs*
-	tests*
-
 [options.extras_require]
 testing = 
-	pytest >= 6
+	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
-	pytest-black >= 0.3.7; \
-	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy >= 0.9.1; \
-	python_implementation != "PyPy"
+	pytest-mypy
 	pytest-enabler >= 2.2
-	pytest-ruff
+	pytest-ruff >= 0.2.1
 docs = 
 	sphinx >= 3.5
-	jaraco.packaging >= 9
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 
 [options.entry_points]
 
 [egg_info]
```

