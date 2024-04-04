# Comparing `tmp/atomicds-0.0.4.tar.gz` & `tmp/atomicds-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomicds-0.0.4.tar", last modified: Sat Mar 30 21:01:09 2024, max compression
+gzip compressed data, was "atomicds-0.0.5.tar", last modified: Thu Apr  4 00:55:25 2024, max compression
```

## Comparing `atomicds-0.0.4.tar` & `atomicds-0.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.222355 atomicds-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.206355 atomicds-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.210355 atomicds-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-30 21:01:04.000000 atomicds-0.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-30 21:01:04.000000 atomicds-0.0.4/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-30 21:01:04.000000 atomicds-0.0.4/.github/workflows/upgrade_dependencies.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-30 21:01:04.000000 atomicds-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-30 21:01:04.000000 atomicds-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-30 21:01:04.000000 atomicds-0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-30 21:01:04.000000 atomicds-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-30 21:01:04.000000 atomicds-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-30 21:01:09.222355 atomicds-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 21:01:04.000000 atomicds-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-30 21:01:04.000000 atomicds-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.214355 atomicds-0.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-windows-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-windows-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-windows-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-windows-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-windows-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-30 21:01:04.000000 atomicds-0.0.4/requirements/requirements-windows-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 21:01:09.222355 atomicds-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.206355 atomicds-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.218355 atomicds-0.0.4/src/atomicds/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.218355 atomicds-0.0.4/src/atomicds/core/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.222355 atomicds-0.0.4/src/atomicds/results/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19360 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/results/rheed_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/results/rheed_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-30 21:01:04.000000 atomicds-0.0.4/src/atomicds/results/xps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.222355 atomicds-0.0.4/src/atomicds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-30 21:01:09.000000 atomicds-0.0.4/src/atomicds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-30 21:01:09.000000 atomicds-0.0.4/src/atomicds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:01:09.000000 atomicds-0.0.4/src/atomicds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-30 21:01:09.000000 atomicds-0.0.4/src/atomicds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 21:01:09.000000 atomicds-0.0.4/src/atomicds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:09.222355 atomicds-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 21:01:04.000000 atomicds-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-30 21:01:04.000000 atomicds-0.0.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-30 21:01:04.000000 atomicds-0.0.4/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.534187 atomicds-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.522187 atomicds-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.522187 atomicds-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-04 00:55:20.000000 atomicds-0.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-04 00:55:20.000000 atomicds-0.0.5/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-04 00:55:20.000000 atomicds-0.0.5/.github/workflows/upgrade_dependencies.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-04 00:55:20.000000 atomicds-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-04 00:55:20.000000 atomicds-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 00:55:20.000000 atomicds-0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 00:55:20.000000 atomicds-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 00:55:20.000000 atomicds-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-04 00:55:25.534187 atomicds-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:55:20.000000 atomicds-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-04 00:55:20.000000 atomicds-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.530187 atomicds-0.0.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-04 00:55:20.000000 atomicds-0.0.5/requirements/requirements-windows-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:55:25.534187 atomicds-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.522187 atomicds-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.530187 atomicds-0.0.5/src/atomicds/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.530187 atomicds-0.0.5/src/atomicds/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.534187 atomicds-0.0.5/src/atomicds/results/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25799 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/results/rheed_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/results/rheed_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-04 00:55:20.000000 atomicds-0.0.5/src/atomicds/results/xps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.534187 atomicds-0.0.5/src/atomicds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 00:55:25.000000 atomicds-0.0.5/src/atomicds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:25.534187 atomicds-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:55:20.000000 atomicds-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-04 00:55:20.000000 atomicds-0.0.5/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-04 00:55:20.000000 atomicds-0.0.5/tests/test_core.py
```

### Comparing `atomicds-0.0.4/.github/workflows/release.yml` & `atomicds-0.0.5/.github/workflows/release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
       working-directory: ./
 
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_TOKEN }}
-        packages_dir: ./dist/
+        packages-dir: ./dist/
 
   #  docs:
   #    runs-on: ubuntu-latest
   #    needs:
   #      - deploy
   #
   #    steps:
```

### Comparing `atomicds-0.0.4/.github/workflows/testing.yml` & `atomicds-0.0.5/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/.github/workflows/upgrade_dependencies.yml` & `atomicds-0.0.5/.github/workflows/upgrade_dependencies.yml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/.gitignore` & `atomicds-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/.pre-commit-config.yaml` & `atomicds-0.0.5/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       - id: check-yaml
       - id: destroyed-symlinks
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.292
+    rev: v0.3.4
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
```

### Comparing `atomicds-0.0.4/LICENSE` & `atomicds-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/PKG-INFO` & `atomicds-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomicds
-Version: 0.0.4
+Version: 0.0.5
 Summary: API client for Atomic Data Sciences.
 Author-email: Atomic Data Sciences <info@atomicdatasciences.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atomicds-0.0.4/pyproject.toml` & `atomicds-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-macos-latest_py3.10.txt` & `atomicds-0.0.5/requirements/requirements-macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-macos-latest_py3.10_extras.txt` & `atomicds-0.0.5/requirements/requirements-macos-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-macos-latest_py3.11.txt` & `atomicds-0.0.5/requirements/requirements-macos-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-macos-latest_py3.11_extras.txt` & `atomicds-0.0.5/requirements/requirements-macos-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-macos-latest_py3.9.txt` & `atomicds-0.0.5/requirements/requirements-macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-macos-latest_py3.9_extras.txt` & `atomicds-0.0.5/requirements/requirements-macos-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.10.txt` & `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.10_extras.txt` & `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.11.txt` & `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.11_extras.txt` & `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.9.txt` & `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-ubuntu-latest_py3.9_extras.txt` & `atomicds-0.0.5/requirements/requirements-ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-windows-latest_py3.10.txt` & `atomicds-0.0.5/requirements/requirements-windows-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-windows-latest_py3.10_extras.txt` & `atomicds-0.0.5/requirements/requirements-windows-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-windows-latest_py3.11.txt` & `atomicds-0.0.5/requirements/requirements-windows-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-windows-latest_py3.11_extras.txt` & `atomicds-0.0.5/requirements/requirements-windows-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-windows-latest_py3.9.txt` & `atomicds-0.0.5/requirements/requirements-windows-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/requirements/requirements-windows-latest_py3.9_extras.txt` & `atomicds-0.0.5/requirements/requirements-windows-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/src/atomicds/client.py` & `atomicds-0.0.5/src/atomicds/client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/src/atomicds/core/client.py` & `atomicds-0.0.5/src/atomicds/core/client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/src/atomicds/results/rheed_image.py` & `atomicds-0.0.5/src/atomicds/results/rheed_image.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from monty.json import MSONable
 from networkx import Graph
 from PIL import Image as PILImage
 from PIL import ImageDraw
 from PIL.Image import Image
 from pycocotools import mask
 
-from atomicds.core import ClientError, boxes_overlap
+from atomicds.core import boxes_overlap, generate_graph_from_nodes
 
 tp.quiet()
 
 
 class RHEEDImageResult(MSONable):
     def __init__(
         self,
@@ -47,30 +47,44 @@
 
         self.data_id = data_id
         self.processed_image = processed_image
         self.pattern_graph = pattern_graph
         self.processed_data_id = processed_data_id
         self.metadata = metadata
 
-    def get_plot(self, show_mask: bool = True, show_spot_nodes: bool = True) -> Image:
+    def get_plot(
+        self,
+        show_mask: bool = True,
+        show_spot_nodes: bool = True,
+        symmetrize: bool = False,
+    ) -> Image:
         """Get diffraction pattern image with optional overlays
 
         Args:
             show_mask (bool): Whether to show mask overlay of identified pattern. Defaults to True.
             show_spot_nodes (bool): Whether to show identified diffraction node overlays. Defaults to True.
 
         Returns:
             (Image): PIL Image object with optional overlays
 
         """
         image = self.processed_image.copy().convert("RGBA")
         draw = ImageDraw.Draw(image)
-        if self.pattern_graph:
+
+        if symmetrize:
+            node_df = pd.DataFrame.from_dict(
+                dict(self.pattern_graph.nodes(data=True)), orient="index"
+            )
+            _, pattern_graph = self._symmetrize(node_df)
+        else:
+            pattern_graph = self.pattern_graph
+
+        if pattern_graph:
             masks = []
-            for _, node_data in self.pattern_graph.nodes.data():
+            for _, node_data in pattern_graph.nodes.data():
                 if show_mask:
                     mask_rle = node_data.get("mask_rle")
                     mask_width = node_data.get("mask_width")
                     mask_height = node_data.get("mask_height")
 
                     if mask_rle and mask_width and mask_height:
                         mask_dict = {
@@ -123,28 +137,34 @@
             node_data.append(
                 pd.DataFrame.from_dict(
                     dict(self.pattern_graph.nodes(data=True)), orient="index"
                 )
             )
 
         node_df = pd.concat(node_data, axis=0).reset_index(drop=True)
-        node_df = self._symmetrize(node_df)
+        node_df, _ = self._symmetrize(node_df)
 
         image_array = np.array(self.processed_image)
 
         thetas = np.linspace(0, 2 * np.pi, 1440)
-        radiis = np.linspace(100, 1000, 100)
+        radiis = np.linspace(100, 1400, 2000)
 
         intersection_point = (
             node_df.loc[node_df["node_id"] == node_df["node_id"].min()][
-                ["centroid_0", "centroid_1"]
+                ["intensity_centroid_0", "intensity_centroid_1"]
+            ]
+            .to_numpy()
+            .squeeze()
+            + node_df.loc[node_df["node_id"] == node_df["node_id"].min()][
+                ["specular_origin_0", "specular_origin_1"]
             ]
             .to_numpy()
             .squeeze()
         )
+
         result_matrix = []
 
         for r0 in radiis:
             x_center, y_center = intersection_point[1], intersection_point[0] - r0
             x_points = r0 * np.cos(thetas) + x_center
             y_points = r0 * np.sin(thetas) + y_center
             int_x_points = np.round(x_points).astype(int)
@@ -157,22 +177,23 @@
             coords = coords[coords[:, 1] < image_array.shape[0]]
             coords = coords[coords[:, 0] < image_array.shape[1]]
             if len(coords) == 0:
                 continue
             intensities = image_array[coords[:, 1], coords[:, 0]]
             result_matrix.append(np.quantile(intensities, 0.9))
 
-        best_fit_radius = np.mean(radiis[np.argsort(result_matrix)][-3:])
+        best_fit_radius = np.mean(radiis[np.argsort(result_matrix)][-30:])
 
-        return best_fit_radius, (intersection_point[0] - best_fit_radius, x_center)  # type: ignore  # noqa: PGH003
+        return best_fit_radius, [intersection_point[0] - best_fit_radius, x_center]  # type: ignore  # noqa: PGH003
 
     def get_pattern_dataframe(
         self,
         extra_data: dict | None = None,
         symmetrize: bool = False,
+        return_as_features: bool = False,
     ) -> pd.DataFrame:
         """Featurize the RHEED image collection into a dataframe of node features and edge features.
 
         Args:
             extra_data (dict | None): Dictionary containing field names and values of extra data to be included in the DataFrame object.
                 Defaults to None.
             fields_to_retain (list[str] | None): Fields to ensure are kept in the DataFrame object. Defaults to None which
@@ -212,19 +233,20 @@
                     dict(self.pattern_graph.nodes(data=True)), orient="index"
                 )
             )
 
         node_df = pd.concat(node_data, axis=0).reset_index(drop=True)
 
         if symmetrize:
-            node_df = self._symmetrize(node_df)
+            node_df, _ = self._symmetrize(node_df)
 
         extra_data_df = pd.DataFrame.from_records(
-            [{"data_id": self.data_id} | extra_data]
+            [{"data_id": self.processed_data_id} | extra_data]
         )
+
         feature_df: pd.DataFrame = node_df.pivot_table(
             index="uuid", columns="node_id", values=node_feature_cols
         )
 
         feature_df.columns = feature_df.columns.to_flat_index()
 
         feature_df = feature_df.merge(
@@ -233,138 +255,221 @@
         feature_df = feature_df.rename(
             columns={col: (col, "") for col in extra_data_df.columns}
         )
         feature_df.columns = pd.MultiIndex.from_tuples(feature_df.columns)
 
         keep_cols = node_feature_cols + list(extra_data.keys())
 
-        return feature_df[keep_cols]  # type: ignore  # noqa: PGH003
+        if return_as_features:
+            return feature_df[keep_cols]
+
+        return node_df  # , feature_df[keep_cols]  # type: ignore  # noqa: PGH003
 
     @staticmethod
     def _symmetrize(node_df: pd.DataFrame):
         """Symmetrize a DataFrame object containing RHEED image node data"""
 
+        # def reflect_mask(mask_obj: str, height, width) -> str:
+        #     """Reflect a list of RLE masks across the vertical axis"""
+        #     mask_obj = mask.decode({"counts": mask_obj, "size": (height, width)})
+        #     reflected_mask = np.asfortranarray(np.fliplr(mask_obj))
+        #     return mask.encode(reflected_mask)['counts']
+
+        def reflect_mask(mask_obj: str, height: int, width: int, origin: float) -> str:
+            """Reflect a list of RLE masks across the vertical axis"""
+
+            mask_array: np.ndarray = mask.decode(
+                {"counts": mask_obj, "size": (height, width)}
+            )
+            origin = int(np.round(origin, 0))
+            num_cols_to_mirror = mask_array.shape[1] - origin
+
+            reflected_array = mask_array.copy()
+
+            # For columns before the origin position, swap them with their mirrored counterparts
+            for i in range(origin, origin - num_cols_to_mirror, -1):
+                swap_index = origin + (origin - i)
+                if swap_index < mask_array.shape[1]:
+                    reflected_array[:, i], reflected_array[:, swap_index] = (
+                        mask_array[:, swap_index].copy(),
+                        mask_array[:, i].copy(),
+                    )
+
+            return mask.encode(np.asfortranarray(reflected_array))["counts"]
+
+        def merge_masks(masks: list[str], height, width) -> str:
+            """Merge a list of RLE masks using logical OR"""
+            mask_objs = [
+                mask.decode({"counts": mm, "size": (height, width)}) for mm in masks
+            ]
+            merged_mask = np.asfortranarray(np.logical_or.reduce(mask_objs))
+            return mask.encode(merged_mask)
+
+        def merge_overlaps(node_df):
+            """Merge overlapping nodes in a DataFrame object. Use recursively until no overlaps remain."""
+
+            first_row = node_df.iloc[[0]]
+            original_dtypes = first_row.dtypes
+
+            agg_dict = {
+                "centroid_0": "mean",
+                "centroid_1": "mean",
+                "intensity_centroid_0": "mean",
+                "intensity_centroid_1": "mean",
+                "relative_centroid_0": "mean",
+                "relative_centroid_1": "mean",
+                "bbox_minc": "mean",
+                "bbox_minr": "mean",
+                "bbox_maxc": "mean",
+                "bbox_maxr": "mean",
+                "area": "mean",
+                "node_id": "min",
+                "pattern_id": lambda x: x.iloc[0],
+                "specular_origin_0": "mean",
+                "specular_origin_1": "mean",
+                "center_distance": "mean",
+                "fwhm_0": "mean",
+                "fwhm_1": "mean",
+                "mask_rle": lambda x: x.tolist(),
+                "mask_width": lambda x: x.iloc[0],
+                "mask_height": lambda x: x.iloc[0],
+                "uuid": lambda x: x.iloc[0],
+                "oscillation_period_seconds": "mean",
+                "eccentricity": "mean",
+                "axis_major_length": "mean",
+                "axis_minor_length": "mean",
+                "bbox_intensity": "mean",
+                "spot_area": "mean",
+                "streak_area": "mean",
+            }
+
+            new_df = pd.DataFrame()
+            for i in range(len(node_df)):
+                current_bbox = node_df.iloc[i][
+                    ["bbox_minc", "bbox_minr", "bbox_maxc", "bbox_maxr"]
+                ]
+                overlapping_nodes = node_df[
+                    node_df.apply(
+                        lambda row, current_bbox=current_bbox: boxes_overlap(
+                            current_bbox,
+                            row[["bbox_minc", "bbox_minr", "bbox_maxc", "bbox_maxr"]],
+                        ),
+                        axis=1,
+                    )
+                ]
+
+                merged_row = overlapping_nodes.agg(agg_dict)
+
+                new_mask = merge_masks(
+                    merged_row["mask_rle"],
+                    merged_row["mask_height"],
+                    merged_row["mask_width"],
+                )["counts"]
+                merged_row["mask_rle"] = new_mask
+
+                new_df = pd.concat([new_df, merged_row], axis=1)
+
+            new_df = new_df.T.astype(original_dtypes).reset_index(drop=True)
+            agg_dict["mask_rle"] = lambda x: merge_masks(
+                x, new_df["mask_height"].iloc[0], new_df["mask_width"].iloc[0]
+            )["counts"]
+            new_df = new_df.groupby("node_id").agg(agg_dict).reset_index(drop=True)
+
+            # relabel node_id > 1000 to monotonically increase from the largest ID < 1000
+            while new_df["node_id"].max() > 1000:
+                max_id = new_df.loc[new_df["node_id"] < 1000]["node_id"].max()
+                new_df.loc[new_df["node_id"] == new_df["node_id"].max(), "node_id"] = (
+                    max_id + 1
+                )
+
+            return new_df
+
         reflection_plane = node_df["specular_origin_1"].mean()
 
         left_nodes = node_df.loc[node_df["centroid_1"] < reflection_plane]
         right_nodes = node_df.loc[node_df["centroid_1"] > reflection_plane]
 
-        # Left to right
         left_to_right = left_nodes.copy()
         left_to_right["centroid_1"] = reflection_plane + (
             reflection_plane - left_to_right["centroid_1"]
         )
         left_to_right["intensity_centroid_1"] = -left_to_right["intensity_centroid_1"]
         left_to_right["relative_centroid_1"] = -left_to_right["relative_centroid_1"]
+        left_to_right["mask_rle"] = left_to_right["mask_rle"].apply(
+            lambda x: reflect_mask(
+                x,
+                left_to_right["mask_height"].iloc[0],
+                left_to_right["mask_width"].iloc[0],
+                left_to_right["specular_origin_1"].iloc[0],
+            )
+        )
 
-        left_to_right["bbox_maxc"] = (
+        new_max = (
             reflection_plane + (reflection_plane - left_to_right["bbox_minc"])
         ).astype(int)
-        left_to_right["bbox_minc"] = (
+        new_min = (
             reflection_plane + (reflection_plane - left_to_right["bbox_maxc"])
         ).astype(int)
+        left_to_right["bbox_maxc"] = new_max
+        left_to_right["bbox_minc"] = new_min
+
+        left_to_right["node_id"] = left_to_right["node_id"] + 1000
 
-        # Right to left
         right_to_left = right_nodes.copy()
         right_to_left["centroid_1"] = reflection_plane - (
             right_to_left["centroid_1"] - reflection_plane
         )
         right_to_left["intensity_centroid_1"] = -right_to_left["intensity_centroid_1"]
         right_to_left["relative_centroid_1"] = -right_to_left["relative_centroid_1"]
+        right_to_left["mask_rle"] = right_to_left["mask_rle"].apply(
+            lambda x: reflect_mask(
+                x,
+                right_to_left["mask_height"].iloc[0],
+                right_to_left["mask_width"].iloc[0],
+                right_to_left["specular_origin_1"].iloc[0],
+            )
+        )
 
-        right_to_left["bbox_minc"] = (
+        new_max = (
             reflection_plane - (right_to_left["bbox_minc"] - reflection_plane)
         ).astype(int)
-        right_to_left["bbox_maxc"] = (
+        new_min = (
             reflection_plane - (right_to_left["bbox_maxc"] - reflection_plane)
         ).astype(int)
 
+        right_to_left["bbox_minc"] = new_min
+        right_to_left["bbox_maxc"] = new_max
+        right_to_left["node_id"] = right_to_left["node_id"] + 2000
+
         node_df = pd.concat(
             [node_df, left_to_right, right_to_left], axis=0
         ).reset_index(drop=True)
 
         if node_df.empty:
             return node_df
 
-        first_row = node_df.iloc[[0]].pop("last_updated")
-        original_dtypes = first_row.dtypes
+        node_df = node_df.drop(columns=["last_updated", "version"])
 
-        # merge rows with overlapping bounding boxes into one row
-        drop_rows = []
-        add_rows = []
-        for i in range(
-            len(node_df) - 1
-        ):  # -1 so we don't try to pair the last row with anything
-            for j in range(
-                i + 1, len(node_df)
-            ):  # Start from i+1 to avoid repeats and self-pairing
-                row1 = node_df.iloc[[i]]
-                row2 = node_df.iloc[[j]]
-                if boxes_overlap(
-                    row1[["bbox_minc", "bbox_minr", "bbox_maxc", "bbox_maxr"]]
-                    .to_numpy()
-                    .squeeze()
-                    .tolist(),
-                    row2[["bbox_minc", "bbox_minr", "bbox_maxc", "bbox_maxr"]]
-                    .to_numpy()
-                    .squeeze()
-                    .tolist(),
-                ):
-                    merged_row = (
-                        pd.concat([row1, row2], axis=0)
-                        .sort_values("node_id")
-                        .reset_index(drop=True)
-                    )
-                    merged_row = merged_row.agg(
-                        {
-                            "centroid_0": "mean",
-                            "centroid_1": "mean",
-                            "intensity_centroid_0": "mean",
-                            "intensity_centroid_1": "mean",
-                            "relative_centroid_0": "mean",
-                            "relative_centroid_1": "mean",
-                            "bbox_minc": "mean",
-                            "bbox_minr": "mean",
-                            "bbox_maxc": "mean",
-                            "bbox_maxr": "mean",
-                            "area": "mean",
-                            "node_id": "min",
-                            "pattern_id": lambda x: x.iloc[0],
-                            "specular_origin_0": "mean",
-                            "specular_origin_1": "mean",
-                            "center_distance": "mean",
-                            "fwhm_0": "mean",
-                            "fwhm_1": "mean",
-                            "mask_rle": lambda x: x.iloc[0],
-                            "mask_width": lambda x: x.iloc[0],
-                            "mask_height": lambda x: x.iloc[0],
-                            "uuid": lambda x: x.iloc[0],
-                            "oscillation_period_seconds": "mean",
-                            "eccentricity": "mean",
-                            "axis_major_length": "mean",
-                            "axis_minor_length": "mean",
-                            "bbox_intensity": "mean",
-                            "spot_area": "mean",
-                            "streak_area": "mean",
-                        }
-                    )
+        new_df = merge_overlaps(node_df)
+        while len(new_df) != len(node_df):
+            node_df = new_df.copy(deep=True)
+            new_df = merge_overlaps(node_df)
+
+        new_pattern_graph = generate_graph_from_nodes(new_df)
 
-                    drop_rows.append(i)
-                    drop_rows.append(j)
-                    add_rows.append(merged_row)
-
-        node_df = node_df.drop(drop_rows, axis=0)
-        merged_df = pd.concat(add_rows, axis=1).T.astype(original_dtypes)
-        return pd.concat([node_df, merged_df], axis=0).reset_index(drop=True)
+        return new_df, new_pattern_graph
 
 
 # TODO: Add tests for RHEEDImageCollection
 class RHEEDImageCollection(MSONable):
     def __init__(
-        self, rheed_images: list[RHEEDImageResult], extra_data: list[dict] | None = None
+        self,
+        rheed_images: list[RHEEDImageResult],
+        extra_data: list[dict] | None = None,
+        sort_key: str | None = None,
     ):
         """Collection of RHEED images
 
         Args:
             rheed_images (list[RHEEDImageResult]): List of RHEEDImageResult objects.
             extra_data (list[dict] | None): List of dictionaries containing field names and values of extra data to be included in the DataFrame object.
                 Defaults to None.
@@ -380,80 +485,98 @@
         for idx, rheed_image in enumerate(rheed_images):
             if rheed_image.pattern_graph:
                 for node in rheed_image.pattern_graph.nodes:
                     rheed_image.pattern_graph.nodes[node]["pattern_id"] = idx
 
         self._rheed_images = rheed_images
         self._extra_data = extra_data
+        self._sort_key = sort_key
+        if self._sort_key is None:
+            self._sort_key = next(iter(self._extra_data[0].keys()))
+        self._sort_by_extra_data_key(self._sort_key)
 
     @property
     def rheed_images(self):
         return self._rheed_images
 
     @property
     def extra_data(self):
         return self._extra_data
 
-    def align_fingerprints(self) -> tuple[pd.DataFrame, list[RHEEDImageResult]]:
+    @property
+    def sort_key(self):
+        return self._sort_key
+
+    def align_fingerprints(
+        self, node_df: pd.DataFrame | None = None, inplace: bool = False
+    ) -> RHEEDImageCollection:
         """
         Align a collection of RHEED fingerprints by relabeling the nodes to connect the same scattering
         features across RHEED patterns, based on relative position to the center feature.
 
         Returns:
             (tuple[DataFrame, list[RHEEDImageResult]): Pandas DataFrame object with aligned RHEED fingerprint data
         """
+
         image_scales = [
             rheed_image.processed_image.size for rheed_image in self.rheed_images
         ]
         image_scale = np.amax(image_scales, axis=0)
-        data_ids = [rheed_image.data_id for rheed_image in self.rheed_images]
+        # data_ids = [rheed_image.data_id for rheed_image in self.rheed_images]
 
-        node_data = []
-        for ind, rheed_image in enumerate(self.rheed_images):
-            if rheed_image.pattern_graph is None:
-                raise ClientError(
-                    f"Unable to align fingerprints as rheed image {ind} has no graph data."
+        if node_df is None:
+            node_dfs = [
+                rheed_image.get_pattern_dataframe(
+                    extra_data=extra_data, symmetrize=False, return_as_features=False
                 )
-            node_data.append(
-                pd.DataFrame.from_dict(
-                    dict(rheed_image.pattern_graph.nodes(data=True)), orient="index"
-                )
-            )
+                for rheed_image, extra_data in zip(self.rheed_images, self.extra_data)
+            ]
 
-        node_df = pd.concat(
-            node_data,
-            axis=0,
-        ).reset_index(drop=True)
+            node_df = pd.concat(node_dfs, axis=0).reset_index(drop=True)
 
         labels, _ = pd.factorize(node_df["uuid"])
         node_df["pattern_id"] = labels
 
         linked_df = tp.link(
             f=node_df,
-            search_range=np.sqrt(np.sum(np.square(image_scale))) * 0.05,
-            memory=len(data_ids),
+            search_range=np.sqrt(np.sum(np.square(image_scale))) * 0.1,
+            memory=1,
             t_column="pattern_id",
             pos_columns=["relative_centroid_1", "relative_centroid_0"],
         )
 
         rheed_images: list[RHEEDImageResult] = []
         splits = [group for _, group in linked_df.groupby("pattern_id")]
         for split, rheed_image in zip(splits, self.rheed_images):
             mapping = dict(zip(split["node_id"], split["particle"]))
+            # don't relabel the specular 0 node.
+            if 0 in mapping:
+                mapping.pop(0)
+
             rheed_image.pattern_graph = nx.relabel_nodes(  # type: ignore  # noqa: PGH003
                 rheed_image.pattern_graph,  # type: ignore  # noqa: PGH003
                 mapping,
             )
+            for node in rheed_image.pattern_graph.nodes:
+                rheed_image.pattern_graph.nodes[node]["node_id"] = node
+
             rheed_images.append(rheed_image)
 
-        return linked_df, rheed_images
+        if inplace:
+            self._rheed_images = rheed_images
+
+        return self.__class__(rheed_images, self.extra_data, self.sort_key)  # linked_df
 
     def get_pattern_dataframe(
-        self, streamline: bool = True, normalize: bool = True
-    ) -> pd.DataFrame:
+        self,
+        streamline: bool = True,
+        normalize: bool = True,
+        symmetrize: bool = False,
+        return_as_features: bool = True,
+    ) -> tuple[pd.DataFrame, pd.DataFrame]:
         """Featurize the RHEED image collection into a dataframe of node features and edge features.
 
         Args:
             streamline (bool): Whether to remove streamline the DataFrame object and remove null values. Defaults to True.
             normalize (bool): Whether to min/max normalize the feature data across all images. Defaults to True.
 
         Returns:
@@ -478,34 +601,93 @@
             "axis_minor_length",
         ]
 
         # TODO: add edge features
         # edge_feature_cols = ["weight", "horizontal_weight", "vertical_weight", "horizontal_overlap"]
 
         if self.extra_data:
+            node_dfs = [
+                rheed_image.get_pattern_dataframe(
+                    extra_data=extra_data,
+                    symmetrize=symmetrize,
+                    return_as_features=False,
+                )
+                for rheed_image, extra_data in zip(self.rheed_images, self.extra_data)
+            ]
             feature_dfs = [
-                rheed_image.get_pattern_dataframe(extra_data=extra_data)
+                rheed_image.get_pattern_dataframe(
+                    extra_data=extra_data,
+                    symmetrize=symmetrize,
+                    return_as_features=True,
+                )
                 for rheed_image, extra_data in zip(self.rheed_images, self.extra_data)
             ]
         else:
+            node_dfs = [
+                rheed_image.get_pattern_dataframe(
+                    symmetrize=symmetrize, return_as_features=False
+                )
+                for rheed_image in self.rheed_images
+            ]
             feature_dfs = [
-                rheed_image.get_pattern_dataframe() for rheed_image in self.rheed_images
+                rheed_image.get_pattern_dataframe(
+                    symmetrize=symmetrize, return_as_features=True
+                )
+                for rheed_image in self.rheed_images
             ]
 
+        node_df = pd.concat(node_dfs, axis=0).reset_index(drop=True)
         feature_df = pd.concat(feature_dfs, axis=0).reset_index(drop=True)
 
         keep_cols = node_feature_cols + list(
             {key for extra_data in self.extra_data for key in extra_data}
         )
 
         feature_df = feature_df[keep_cols]
 
         if streamline:
             feature_df = feature_df.dropna(axis=1)
 
         if normalize:
+            for col in node_feature_cols:
+                feature_df[col] = (feature_df[col] - feature_df[col].mean()) / (
+                    feature_df[col].std()
+                )
+
             # min max normalization
-            feature_df = (feature_df - feature_df.min()) / (
-                feature_df.max() - feature_df.min()
+            # feature_df[node_feature_cols].apply(
+            #     lambda x: (x - x.min()) / (x.max() - x.min()), inp
+            # )
+
+        if return_as_features:
+            return feature_df
+
+        return node_df  # , feature_df  # type: ignore  # noqa: PGH003
+
+    def _sort_by_extra_data_key(self, key: str):
+        """Sort the RHEEDImageCollection by an extra data key"""
+        if key not in self.extra_data[0]:
+            raise ValueError(
+                f"Extra data key {key} not found in the extra data dictionary."
             )
 
-        return feature_df  # type: ignore  # noqa: PGH003
+        sort_order = [extra_data[key] for extra_data in self.extra_data]
+        sorted_indices = np.argsort(sort_order)
+
+        self._rheed_images = [self.rheed_images[idx] for idx in sorted_indices]
+        self._extra_data = [self.extra_data[idx] for idx in sorted_indices]
+
+    def __getitem__(self, key: int | slice) -> RHEEDImageResult | RHEEDImageCollection:
+        if isinstance(key, int):
+            return self.rheed_images[key]
+
+        if isinstance(key, slice):
+            return self.__class__(
+                self.rheed_images[key], self.extra_data[key], self.sort_key
+            )
+
+        return self.__class__(
+            self.rheed_images[key], self.extra_data[key], self.sort_key
+        )
+
+    def __len__(self) -> int:
+        return len(self.rheed_images)
```

### Comparing `atomicds-0.0.4/src/atomicds/results/rheed_video.py` & `atomicds-0.0.5/src/atomicds/results/rheed_video.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/src/atomicds/results/xps.py` & `atomicds-0.0.5/src/atomicds/results/xps.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/src/atomicds.egg-info/PKG-INFO` & `atomicds-0.0.5/src/atomicds.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomicds
-Version: 0.0.4
+Version: 0.0.5
 Summary: API client for Atomic Data Sciences.
 Author-email: Atomic Data Sciences <info@atomicdatasciences.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `atomicds-0.0.4/src/atomicds.egg-info/SOURCES.txt` & `atomicds-0.0.5/src/atomicds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/tests/test_client.py` & `atomicds-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `atomicds-0.0.4/tests/test_core.py` & `atomicds-0.0.5/tests/test_core.py`

 * *Files identical despite different names*

