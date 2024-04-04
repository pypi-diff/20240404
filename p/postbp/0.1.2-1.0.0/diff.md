# Comparing `tmp/postbp-0.1.2.tar.gz` & `tmp/postbp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postbp-0.1.2.tar", last modified: Wed Apr  3 12:56:02 2024, max compression
+gzip compressed data, was "postbp-1.0.0.tar", last modified: Thu Apr  4 15:43:54 2024, max compression
```

## Comparing `postbp-0.1.2.tar` & `postbp-1.0.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.549768 postbp-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 12:55:50.000000 postbp-0.1.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.537768 postbp-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.541768 postbp-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.541768 postbp-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 12:55:50.000000 postbp-0.1.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-03 12:55:50.000000 postbp-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 12:55:50.000000 postbp-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 12:55:50.000000 postbp-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 12:56:02.549768 postbp-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 12:55:50.000000 postbp-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.545768 postbp-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/dailyfirevectors.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/dataloader.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.545768 postbp-0.1.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/finalfirevectors.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.545768 postbp-0.1.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/postbp.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/spreadrose.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/tessellation.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 12:55:50.000000 postbp-0.1.2/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-03 12:55:50.000000 postbp-0.1.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.545768 postbp-0.1.2/postbp/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/dailyfirevectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/finalfirevectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/postbp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/spreadrose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5274 2024-04-03 12:55:50.000000 postbp-0.1.2/postbp/tessellation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.549768 postbp-0.1.2/postbp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 12:56:02.000000 postbp-0.1.2/postbp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-03 12:55:50.000000 postbp-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 12:55:50.000000 postbp-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 12:55:50.000000 postbp-0.1.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:56:02.549768 postbp-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:56:02.549768 postbp-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 12:55:50.000000 postbp-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 12:55:50.000000 postbp-0.1.2/tests/test_postbp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.340013 postbp-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 15:43:44.000000 postbp-1.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.328013 postbp-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.332013 postbp-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.332013 postbp-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-04 15:43:44.000000 postbp-1.0.0/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-04 15:43:44.000000 postbp-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-04 15:43:44.000000 postbp-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 15:43:44.000000 postbp-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 15:43:54.340013 postbp-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-04 15:43:44.000000 postbp-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.336013 postbp-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/dailyfirevectors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/dataloader.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.336013 postbp-1.0.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/finalfirevectors.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.336013 postbp-1.0.0/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/postbp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/spreadrose.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/tessellation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-04 15:43:44.000000 postbp-1.0.0/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-04 15:43:44.000000 postbp-1.0.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.336013 postbp-1.0.0/postbp/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-04 15:43:44.000000 postbp-1.0.0/postbp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 15:43:44.000000 postbp-1.0.0/postbp/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-04 15:43:44.000000 postbp-1.0.0/postbp/dailyfirevectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-04 15:43:44.000000 postbp-1.0.0/postbp/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-04 15:43:44.000000 postbp-1.0.0/postbp/finalfirevectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-04 15:43:44.000000 postbp-1.0.0/postbp/postbp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-04 15:43:44.000000 postbp-1.0.0/postbp/spreadrose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-04 15:43:44.000000 postbp-1.0.0/postbp/tessellation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.340013 postbp-1.0.0/postbp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 15:43:54.000000 postbp-1.0.0/postbp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-04 15:43:54.000000 postbp-1.0.0/postbp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:43:54.000000 postbp-1.0.0/postbp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 15:43:54.000000 postbp-1.0.0/postbp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-04 15:43:54.000000 postbp-1.0.0/postbp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 15:43:54.000000 postbp-1.0.0/postbp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-04 15:43:44.000000 postbp-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 15:43:44.000000 postbp-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 15:43:44.000000 postbp-1.0.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:43:54.340013 postbp-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:43:54.340013 postbp-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 15:43:44.000000 postbp-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 15:43:44.000000 postbp-1.0.0/tests/test_postbp.py
```

### Comparing `postbp-0.1.2/.github/workflows/docs-build.yml` & `postbp-1.0.0/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/.github/workflows/docs.yml` & `postbp-1.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/.github/workflows/installation.yml` & `postbp-1.0.0/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/.github/workflows/macos.yml` & `postbp-1.0.0/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/.github/workflows/pypi.yml` & `postbp-1.0.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/.github/workflows/ubuntu.yml` & `postbp-1.0.0/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/.github/workflows/windows.yml` & `postbp-1.0.0/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/.gitignore` & `postbp-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/LICENSE` & `postbp-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/PKG-INFO` & `postbp-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postbp
-Version: 0.1.2
+Version: 1.0.0
 Summary: A Python Library
 Author-email: Ning Liu <ning.liu@nrcan-rncan.gc.ca>
 License: MIT License
 Project-URL: Homepage, https://github.com/nliu-cfs/postbp
 Keywords: postbp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `postbp-0.1.2/docs/contributing.md` & `postbp-1.0.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/docs/examples/intro.ipynb` & `postbp-1.0.0/docs/examples/intro.ipynb`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/docs/installation.md` & `postbp-1.0.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/mkdocs.yml` & `postbp-1.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/postbp/__init__.py` & `postbp-1.0.0/postbp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for postbp."""
 
 __author__ = """Ning Liu"""
 __email__ = "ning.liu@nrcan-rncan.gc.ca"
-__version__ = "0.1.2"
+__version__ = "1.0.0"
 
 from .common import (
     prj2hex,  #noqa
     pij_to_shp, #noqa
 )
 from .dataloader import(
     read_fireshp,  #noqa
```

### Comparing `postbp-0.1.2/postbp/common.py` & `postbp-1.0.0/postbp/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,9 +43,9 @@
         pij.rename(columns={kwargs["column_j"]: 'column_j'}, inplace=True)           
 
     SRID = node.crs
     pij = node.merge(pij, left_on='Node_ID', right_on='column_i', how='right')
     pij = pij.merge(node, left_on='column_j', right_on='Node_ID', how='left')
     pijLine = [LineString(xy) for xy in zip(pij['geometry_x'], pij['geometry_y'])]
     pijshp = gpd.GeoDataFrame(pij, crs = SRID, geometry = pijLine )
-    pijshp.drop(labels = ['geometry_x', 'geometry_y'], axis = 1, inplace = True)
+    pijshp.drop(labels = ['geometry_x', 'geometry_y', 'Node_ID_x', 'Node_ID_y'], axis = 1, inplace = True)
     return pijshp
```

### Comparing `postbp-0.1.2/postbp/dailyfirevectors.py` & `postbp-1.0.0/postbp/dailyfirevectors.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import pandas as pd
 import itertools
 from math import atan2, degrees
 from .common import prj2hex
 import warnings
 warnings.filterwarnings("ignore")
-import tqdm
+from tqdm import tqdm
 
 def angle(record):
     """Calculate angle from three points: ignition point and the points where fire spread from and to.  
 
     Args:
         record (_type_): _description_
 
@@ -48,15 +48,14 @@
     if 'Node_ID' in kwargs:
         hexagon = hexagon.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
     
     threshold = 3.1415926*bufferFactor**2 - 1 
     SRID = fireshp.crs
     df = pd.DataFrame()
     dfMore = pd.DataFrame()
-    errorlog = []
     
     for i in tqdm(np.unique(fireshp['fire'])):
         try: 
             fire_i = fireshp.loc[fireshp['fire'] == i]
             pts_i = ignition.loc[ignition['fire'] == i]
             pts_ni = gpd.sjoin(pts_i, hexagon, how = 'inner', op = 'within')
             ##### ignition point to all hexes
@@ -98,18 +97,16 @@
                     pass
             dfMore = dfMore.reset_index(drop = True)
             dfMore.drop_duplicates(subset = ['column_i', 'column_j', 'day'], keep = 'first', inplace = True)
             dfMore['fire'] = i
             dfMore['ignPt'] = pts_ni['Node_ID'].item()
             df = pd.concat([df, dfMore], sort = True)
         except Exception as e:
-                errorlog.append(f'{e} occurs for fire ID # {i} \n')
-        # output errorlog to a txt
-    with open("errorlog_dailyfire.txt", "w+") as f:
-        f.write(errorlog)
+            with open("errorlog_dailyfire.txt", "w+") as f:
+                f.write(f'{e} occurs for fire ID # {i} \n')    
     return df
 
 def calc_angles(vectors, nodes, **kwargs):
     """_summary_
 
     Args:
         vectors (_type_): _description_
```

### Comparing `postbp-0.1.2/postbp/dataloader.py` & `postbp-1.0.0/postbp/dataloader.py`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/postbp/finalfirevectors.py` & `postbp-1.0.0/postbp/finalfirevectors.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import geopandas as gpd
 import pandas as pd
 from .common import prj2hex
 import warnings
 warnings.filterwarnings("ignore")
 from shapely.errors import ShapelyDeprecationWarning
 warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
-import tqdm
+from tqdm import tqdm
 
 def spatial_join(fireshp, ignition, hexagon, threshold=0, iteration=False):
     """_summary_
 
     Args:
         fireshp (_type_): _description_
         ignition (_type_): _description_
@@ -31,15 +31,14 @@
     """    
 
     # make sure hexagons, fireShp and ignition point shapefile are in the same projection
     ignition = ignition.to_crs(fireshp.crs)
     hexagon = hexagon.to_crs(fireshp.crs)
 
     fire_vectors = pd.DataFrame()
-    errorlog = []
 
     if not iteration:
         for i in tqdm(fireshp['fire']):
             try:
                 fire_i = fireshp.loc[fireshp['fire'] == i]
                 fire_ni = prj2hex(fire_i, hexagon, threshold)                        
                 pts_i = ignition.loc[ignition['fire'] == i]
@@ -49,18 +48,16 @@
                 
                 dfTemp = fire_ni.merge(pts_ni, on = 'fire', how = 'left')
                 dfTemp = dfTemp.drop(dfTemp[dfTemp['Node_ID_x'] == dfTemp['Node_ID_y']].index)
                 dfTemp.drop(labels = ['geometry'], axis = 1, inplace = True)
                 fire_vectors = pd.concat([fire_vectors, dfTemp], sort = True)
                 
             except Exception as e:
-                errorlog.append(f'{e} occurs for fire ID # {i} \n')
-        # output errorlog to a txt
-        with open("errorlog_finalfire.txt", "w+") as f:
-            f.write(errorlog)
+                with open("errorlog_finalfire.txt", "w+") as f:
+                    f.write(f'{e} occurs for fire ID # {i} \n')   
         return fire_vectors
 
 
     if iteration:
         for j in tqdm(set(fireshp['iteration'])):
             fire_j = fireshp.loc[fireshp['iteration'] == j]
             pts_j = ignition.loc[ignition['iteration'] == j]
@@ -76,18 +73,16 @@
                     
                     dfTemp = fire_ni.merge(pts_ni, on = 'fire', how = 'left')
                     dfTemp = dfTemp.drop(dfTemp[dfTemp['Node_ID_x'] == dfTemp['Node_ID_y']].index)
                     dfTemp.drop(labels = ['geometry'], axis = 1, inplace = True)
                     fire_vectors = pd.concat([fire_vectors, dfTemp], sort = True)
                 
                 except Exception as e:
-                    errorlog.append(f'{e} occurs for fire ID # {i} \n')
-        # output errorlog to a txt
-        with open("errorlog_finalfire.txt", "w+") as f:
-            f.write(errorlog)                  
+                    with open("errorlog_finalfire.txt", "w+") as f:
+                        f.write(f'{e} occurs for fire ID # {i} \n')                         
         return fire_vectors
             
 def generate_fire_vectors(fireshp, ignition, hexagons, threshold = 0, loopBy = "fire", **kwargs):
     """_summary_
 
     Args:
         fireshp (_type_): _description_
@@ -132,9 +127,11 @@
 
     fire_pij = vectors.groupby(['column_j', 'column_i'])[['fire']].count()
     fire_pij.reset_index(inplace = True)
     fire_pij = fire_pij.drop(fire_pij[fire_pij['column_j'] == fire_pij['column_i']].index)
     fire_pij['pij'] = fire_pij['fire'] / iterations
     fire_pij['pij'] = fire_pij['pij'].round(5)
     fire_pij['pij'] = fire_pij['pij'].apply(lambda x: '%.5f' % x)
-    
+    fire_pij.rename(columns={'fire':'firecounts'},inplace=True)
+    fire_pij.sort_values(by = ['firecounts'], inplace = True)
+    fire_pij.reset_index(drop=True, inplace=True)
     return fire_pij
```

### Comparing `postbp-0.1.2/postbp/postbp.py` & `postbp-1.0.0/postbp/postbp.py`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/postbp/spreadrose.py` & `postbp-1.0.0/postbp/spreadrose.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from windrose import WindroseAxes
 import matplotlib.cm as cm
 import geopandas as gpd
 from math import atan2, degrees
 from shapely.geometry import LineString 
 from matplotlib import pyplot as plt
-import tqdm
+from tqdm import tqdm
 
 def angle_from_pij(record):
     """_summary_
 
     Args:
         record (_type_): _description_
 
@@ -52,38 +52,41 @@
         pijVectors (_type_): _description_
         nodes (_type_): _description_
 
     Returns:
         _type_: _description_
     """    
     node = nodes.copy()
+    pij = pijVectors.copy() 
     if 'Node_ID' in kwargs:
         node = node.rename(columns={kwargs["Node_ID"]: 'Node_ID'})
-    pij = pijVectors.copy()  
+    if 'column_i' in kwargs:
+        pij.rename(columns={kwargs["column_i"]: 'column_i'}, inplace=True)    
+    if 'column_j' in kwargs:
+        pij.rename(columns={kwargs["column_j"]: 'column_j'}, inplace=True)     
 
     pij = node.merge(pij, left_on = 'Node_ID', right_on = 'column_i', how = 'right')
     pij = pij.merge(node, left_on = 'column_j', right_on = 'Node_ID', how = 'left')    
     pij.drop(labels = ['Node_ID_x', 'Node_ID_y'], axis = 1, inplace = True)
     for index, row in tqdm(pij.iterrows()):
         pij.at[index, 'angle'] = angle_from_pij(row)
     dffLine = [LineString(xy) for xy in zip(pij['geometry_x'], pij['geometry_y'])]
     pij = gpd.GeoDataFrame(pij, crs = node.crs, geometry = dffLine )
     pij.drop(labels = ['geometry_x', 'geometry_y'], axis = 1, inplace = True)
     pij['len'] = pij.geometry.length
     pij['pij'] = pij['pij'].astype(float)
-    pij['pij_len'] = pij['pij']*pij['len']
     return pij
 
 def plot_rose(pijRose, column='pij', save = False):
     if save:
-        plt.rcParams.update({'font.size': 20})
+        plt.rcParams.update({'font.size': 20,"legend.frameon":False})
         ax = WindroseAxes.from_ax()
         ax.bar(pijRose['angle'], pijRose[column], normed=True, blowto=False, cmap=cm.Set2, opening=0.8, edgecolor='white')
-        ax.set_legend(fontsize="20",loc=(1.01, 0.01),frameon=False)
+        ax.set_legend(fontsize="20",loc=(1.01, 0.01))
         plt.savefig(column + 'Rose.png', bbox_inches='tight', pad_inches=.1, transparent=False)
         plt.close()
     else:
-        plt.rcParams.update({'font.size': 20})
+        plt.rcParams.update({'font.size': 20,"legend.frameon":False})
         ax = WindroseAxes.from_ax()
         ax.bar(pijRose['angle'], pijRose[column], normed=True, blowto=False, cmap=cm.Set2, opening=0.8, edgecolor='white')
-        ax.set_legend(fontsize="20",loc=(1.01, 0.01),frameon=False)
+        ax.set_legend(fontsize="20",loc=(1.01, 0.01))
         plt.show()
```

### Comparing `postbp-0.1.2/postbp/tessellation.py` & `postbp-1.0.0/postbp/tessellation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 '''
 
 import geopandas as gpd
 from shapely.geometry import Polygon, Point, LineString
 import warnings
 warnings.filterwarnings("ignore")
 import math
-import tqdm
+from tqdm import tqdm
 
 def create_hexnodes(area, xmin, ymin, xmax, ymax):
     nodes = []
     
     side = 3**0.25 * math.sqrt(2 * area / 9)
     v_step = math.sqrt(3) * side
     h_step = 1.5 * side
```

### Comparing `postbp-0.1.2/postbp.egg-info/PKG-INFO` & `postbp-1.0.0/postbp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postbp
-Version: 0.1.2
+Version: 1.0.0
 Summary: A Python Library
 Author-email: Ning Liu <ning.liu@nrcan-rncan.gc.ca>
 License: MIT License
 Project-URL: Homepage, https://github.com/nliu-cfs/postbp
 Keywords: postbp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `postbp-0.1.2/postbp.egg-info/SOURCES.txt` & `postbp-1.0.0/postbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postbp-0.1.2/pyproject.toml` & `postbp-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "postbp"
-version = "0.1.2"
+version = "1.0.0"
 dynamic = [
     "dependencies",
 ]
 description = "A Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.1.2"
+current_version = "1.0.0"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

