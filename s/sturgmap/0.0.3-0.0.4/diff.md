# Comparing `tmp/sturgmap-0.0.3.tar.gz` & `tmp/sturgmap-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sturgmap-0.0.3.tar", last modified: Wed Mar 27 20:40:03 2024, max compression
+gzip compressed data, was "sturgmap-0.0.4.tar", last modified: Thu Apr  4 03:59:52 2024, max compression
```

## Comparing `sturgmap-0.0.3.tar` & `sturgmap-0.0.4.tar`

### file list

```diff
@@ -1,67 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.076080 sturgmap-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.064081 sturgmap-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.068081 sturgmap-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.068081 sturgmap-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-27 20:39:50.000000 sturgmap-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:39:50.000000 sturgmap-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-27 20:39:50.000000 sturgmap-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-27 20:40:03.076080 sturgmap-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-27 20:39:50.000000 sturgmap-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.068081 sturgmap-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.072080 sturgmap-0.0.3/docs/510labs/
--rw-r--r--   0 runner    (1001) docker     (127)    49445 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/GEOG510_lab5.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/GEOG_510_lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   613279 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/Huckleberry_Finn.txt
--rw-r--r--   0 runner    (1001) docker     (127)   483582 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/This_Side_of_Paradise.txt
--rw-r--r--   0 runner    (1001) docker     (127)   649853 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/Walden.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/cats.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/dogs.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/guest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/guest_book.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/learning_python.txt
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/510labs/programming.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.072080 sturgmap-0.0.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/examples/ipyleaflet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/examples/practice.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.072080 sturgmap-0.0.3/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/sturgmap.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-27 20:39:50.000000 sturgmap-0.0.3/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-27 20:39:50.000000 sturgmap-0.0.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-27 20:39:50.000000 sturgmap-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-27 20:39:50.000000 sturgmap-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-27 20:39:50.000000 sturgmap-0.0.3/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 20:40:03.076080 sturgmap-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.076080 sturgmap-0.0.3/sturgmap/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-27 20:39:50.000000 sturgmap-0.0.3/sturgmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-27 20:39:50.000000 sturgmap-0.0.3/sturgmap/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-27 20:39:50.000000 sturgmap-0.0.3/sturgmap/sturgmap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.076080 sturgmap-0.0.3/sturgmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-27 20:40:03.000000 sturgmap-0.0.3/sturgmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-27 20:40:03.000000 sturgmap-0.0.3/sturgmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:40:03.000000 sturgmap-0.0.3/sturgmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-27 20:40:03.000000 sturgmap-0.0.3/sturgmap.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-27 20:40:03.000000 sturgmap-0.0.3/sturgmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 20:40:03.000000 sturgmap-0.0.3/sturgmap.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:40:03.076080 sturgmap-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 20:39:50.000000 sturgmap-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-27 20:39:50.000000 sturgmap-0.0.3/tests/test_sturgmap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.605828 sturgmap-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.589828 sturgmap-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.593828 sturgmap-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.593828 sturgmap-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-04 03:59:42.000000 sturgmap-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:59:42.000000 sturgmap-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 03:59:42.000000 sturgmap-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-04 03:59:52.605828 sturgmap-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-04 03:59:42.000000 sturgmap-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.597828 sturgmap-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.601828 sturgmap-0.0.4/docs/510labs/
+-rw-r--r--   0 runner    (1001) docker     (127)    49445 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/GEOG510_lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/GEOG_510_lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   613279 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/Huckleberry_Finn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   483582 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/This_Side_of_Paradise.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   649853 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/Walden.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/cats.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/dogs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/guest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/guest_book.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/learning_python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/510labs/programming.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.601828 sturgmap-0.0.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (127)   241236 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/countries.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    91209 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/countries1.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)   171476 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/countries1.shp
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/practice.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/examples/vectordata.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.601828 sturgmap-0.0.4/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/sturgmap.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 03:59:42.000000 sturgmap-0.0.4/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-04 03:59:42.000000 sturgmap-0.0.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-04 03:59:42.000000 sturgmap-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 03:59:42.000000 sturgmap-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 03:59:42.000000 sturgmap-0.0.4/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:59:52.605828 sturgmap-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.601828 sturgmap-0.0.4/sturgmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-04 03:59:42.000000 sturgmap-0.0.4/sturgmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-04 03:59:42.000000 sturgmap-0.0.4/sturgmap/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-04 03:59:42.000000 sturgmap-0.0.4/sturgmap/sturgmap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.605828 sturgmap-0.0.4/sturgmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-04 03:59:52.000000 sturgmap-0.0.4/sturgmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-04 03:59:52.000000 sturgmap-0.0.4/sturgmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 03:59:52.000000 sturgmap-0.0.4/sturgmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 03:59:52.000000 sturgmap-0.0.4/sturgmap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-04 03:59:52.000000 sturgmap-0.0.4/sturgmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 03:59:52.000000 sturgmap-0.0.4/sturgmap.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 03:59:52.605828 sturgmap-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 03:59:42.000000 sturgmap-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-04 03:59:42.000000 sturgmap-0.0.4/tests/test_sturgmap.py
```

### Comparing `sturgmap-0.0.3/.DS_Store` & `sturgmap-0.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/.github/workflows/docs-build.yml` & `sturgmap-0.0.4/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/.github/workflows/docs.yml` & `sturgmap-0.0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/.github/workflows/installation.yml` & `sturgmap-0.0.4/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/.github/workflows/macos.yml` & `sturgmap-0.0.4/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/.github/workflows/pypi.yml` & `sturgmap-0.0.4/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/.github/workflows/ubuntu.yml` & `sturgmap-0.0.4/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/.github/workflows/windows.yml` & `sturgmap-0.0.4/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/.gitignore` & `sturgmap-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/PKG-INFO` & `sturgmap-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sturgmap
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for geospatial analysis
 Author-email: Nathan Sturgill <nsturgi1@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/nathansturgill/sturgmap
 Keywords: sturgmap
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sturgmap-0.0.3/docs/510labs/GEOG510_lab5.ipynb` & `sturgmap-0.0.4/docs/510labs/GEOG510_lab5.ipynb`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/docs/510labs/GEOG_510_lab4.ipynb` & `sturgmap-0.0.4/docs/510labs/GEOG_510_lab4.ipynb`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/docs/510labs/Huckleberry_Finn.txt` & `sturgmap-0.0.4/docs/510labs/Huckleberry_Finn.txt`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/docs/510labs/This_Side_of_Paradise.txt` & `sturgmap-0.0.4/docs/510labs/This_Side_of_Paradise.txt`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/docs/510labs/Walden.txt` & `sturgmap-0.0.4/docs/510labs/Walden.txt`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/docs/contributing.md` & `sturgmap-0.0.4/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/docs/examples/ipyleaflet.ipynb` & `sturgmap-0.0.4/docs/examples/ipyleaflet.ipynb`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/docs/installation.md` & `sturgmap-0.0.4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `sturgmap-0.0.3/mkdocs.yml` & `sturgmap-0.0.4/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
           execute: True
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["510labs/GEOG_510_lab4.ipynb", "510labs/GEOG510_lab5.ipynb", "ipyleaflet.ipynb"]
+          execute_ignore: ["510labs/GEOG_510_lab4.ipynb", "510labs/GEOG510_lab5.ipynb", "ipyleaflet.ipynb", "vectordata.ipynb"]
           
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -78,13 +78,14 @@
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/nathansturgill/sturgmap/issues
     - Examples:
         - examples/intro.ipynb
         - examples/ipyleaflet.ipynb
+        - examples/vectordata.ipynb
     - API Reference:
           - sturgmap module: sturgmap.md
           - common module: common.md
     - Lab:
           - 510labs/GEOG_510_lab4.ipynb
           - 510labs/GEOG510_lab5.ipynb
```

### Comparing `sturgmap-0.0.3/pyproject.toml` & `sturgmap-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sturgmap"
-version = "0.0.3"
+version = "0.0.4"
 dynamic = [
     "dependencies",
 ]
 description = "Python package for geospatial analysis"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.3"
+current_version = "0.0.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `sturgmap-0.0.3/sturgmap.egg-info/PKG-INFO` & `sturgmap-0.0.4/sturgmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sturgmap
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for geospatial analysis
 Author-email: Nathan Sturgill <nsturgi1@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/nathansturgill/sturgmap
 Keywords: sturgmap
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sturgmap-0.0.3/sturgmap.egg-info/SOURCES.txt` & `sturgmap-0.0.4/sturgmap.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -34,16 +34,23 @@
 docs/510labs/Walden.txt
 docs/510labs/cats.txt
 docs/510labs/dogs.txt
 docs/510labs/guest.txt
 docs/510labs/guest_book.txt
 docs/510labs/learning_python.txt
 docs/510labs/programming.txt
+docs/examples/.DS_Store
+docs/examples/countries.geojson
+docs/examples/countries1.dbf
+docs/examples/countries1.shp
+docs/examples/europe_110.geo.json
 docs/examples/ipyleaflet.ipynb
 docs/examples/practice.ipynb
+docs/examples/raster.ipynb
+docs/examples/vectordata.ipynb
 docs/overrides/main.html
 sturgmap/__init__.py
 sturgmap/common.py
 sturgmap/sturgmap.py
 sturgmap.egg-info/PKG-INFO
 sturgmap.egg-info/SOURCES.txt
 sturgmap.egg-info/dependency_links.txt
```

