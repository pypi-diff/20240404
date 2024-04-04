# Comparing `tmp/TheBeans-0.0.6.tar.gz` & `tmp/TheBeans-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheBeans-0.0.6.tar", last modified: Thu Mar 28 18:16:21 2024, max compression
+gzip compressed data, was "TheBeans-0.0.7.tar", last modified: Thu Apr  4 01:12:38 2024, max compression
```

## Comparing `TheBeans-0.0.6.tar` & `TheBeans-0.0.7.tar`

### file list

```diff
@@ -1,65 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.506928 TheBeans-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.494928 TheBeans-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.498928 TheBeans-0.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.498928 TheBeans-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-28 18:16:06.000000 TheBeans-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:16:06.000000 TheBeans-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-28 18:16:06.000000 TheBeans-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-28 18:16:21.506928 TheBeans-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-28 18:16:06.000000 TheBeans-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.506928 TheBeans-0.0.6/TheBeans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-28 18:16:21.000000 TheBeans-0.0.6/TheBeans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-28 18:16:21.000000 TheBeans-0.0.6/TheBeans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 18:16:21.000000 TheBeans-0.0.6/TheBeans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 18:16:21.000000 TheBeans-0.0.6/TheBeans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 18:16:21.000000 TheBeans-0.0.6/TheBeans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 18:16:21.000000 TheBeans-0.0.6/TheBeans.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.502928 TheBeans-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.502928 TheBeans-0.0.6/docs/Labs/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/_cats_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/_dogs_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/broken_dogs_.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/guestbook.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/lab4.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42912 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/lab5.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/learning_python.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/name.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/Labs/reasons.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.506928 TheBeans-0.0.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/examples/ExampleBeans.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/examples/europe_110.geo.json
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/examples/ipyleaflet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.506928 TheBeans-0.0.6/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/thebeans.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-28 18:16:06.000000 TheBeans-0.0.6/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-28 18:16:06.000000 TheBeans-0.0.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-28 18:16:06.000000 TheBeans-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 18:16:06.000000 TheBeans-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-28 18:16:06.000000 TheBeans-0.0.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:16:21.506928 TheBeans-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.506928 TheBeans-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 18:16:06.000000 TheBeans-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-28 18:16:06.000000 TheBeans-0.0.6/tests/test_thebeans.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 18:16:21.506928 TheBeans-0.0.6/thebeans/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-28 18:16:06.000000 TheBeans-0.0.6/thebeans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-28 18:16:06.000000 TheBeans-0.0.6/thebeans/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-03-28 18:16:06.000000 TheBeans-0.0.6/thebeans/thebeans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.345569 TheBeans-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.349570 TheBeans-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.349570 TheBeans-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-04 01:12:20.000000 TheBeans-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:12:20.000000 TheBeans-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 01:12:20.000000 TheBeans-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 01:12:38.357570 TheBeans-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-04 01:12:20.000000 TheBeans-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/TheBeans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 01:12:38.000000 TheBeans-0.0.7/TheBeans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.353570 TheBeans-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/CSVtoDF.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.353570 TheBeans-0.0.7/docs/Labs/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/_cats_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/_dogs_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/broken_dogs_.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/guestbook.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    33576 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42912 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/learning_python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/Labs/reasons.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/CedarCubMuck.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)   309152 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/CedarCubMuck.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/ExampleBeansLab7.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/StudyArea.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/classnotes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   207731 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/us_regions.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/thebeans.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-04 01:12:20.000000 TheBeans-0.0.7/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-04 01:12:20.000000 TheBeans-0.0.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-04 01:12:20.000000 TheBeans-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 01:12:20.000000 TheBeans-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-04 01:12:20.000000 TheBeans-0.0.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:12:38.357570 TheBeans-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:12:20.000000 TheBeans-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-04 01:12:20.000000 TheBeans-0.0.7/tests/test_thebeans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:12:38.357570 TheBeans-0.0.7/thebeans/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-04 01:12:20.000000 TheBeans-0.0.7/thebeans/CSVtoDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-04 01:12:20.000000 TheBeans-0.0.7/thebeans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-04 01:12:20.000000 TheBeans-0.0.7/thebeans/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-04 01:12:20.000000 TheBeans-0.0.7/thebeans/thebeans.py
```

### Comparing `TheBeans-0.0.6/.github/workflows/docs-build.yml` & `TheBeans-0.0.7/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/.github/workflows/docs.yml` & `TheBeans-0.0.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/.github/workflows/installation.yml` & `TheBeans-0.0.7/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/.github/workflows/macos.yml` & `TheBeans-0.0.7/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/.github/workflows/pypi.yml` & `TheBeans-0.0.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/.github/workflows/ubuntu.yml` & `TheBeans-0.0.7/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/.github/workflows/windows.yml` & `TheBeans-0.0.7/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/.gitignore` & `TheBeans-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/PKG-INFO` & `TheBeans-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheBeans
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package with the beans.
 Author-email: Lucas Phillips <lphill57@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/phillipslucas/TheBeans
 Keywords: TheBeans
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ipyleaflet
+Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: TheBeans[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # TheBeans
```

### Comparing `TheBeans-0.0.6/TheBeans.egg-info/PKG-INFO` & `TheBeans-0.0.7/TheBeans.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TheBeans
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package with the beans.
 Author-email: Lucas Phillips <lphill57@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/phillipslucas/TheBeans
 Keywords: TheBeans
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ipyleaflet
+Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: TheBeans[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # TheBeans
```

### Comparing `TheBeans-0.0.6/TheBeans.egg-info/SOURCES.txt` & `TheBeans-0.0.7/TheBeans.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .github/workflows/windows.yml
 TheBeans.egg-info/PKG-INFO
 TheBeans.egg-info/SOURCES.txt
 TheBeans.egg-info/dependency_links.txt
 TheBeans.egg-info/entry_points.txt
 TheBeans.egg-info/requires.txt
 TheBeans.egg-info/top_level.txt
+docs/CSVtoDF.md
 docs/changelog.md
 docs/common.md
 docs/contributing.md
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/thebeans.md
@@ -36,17 +37,26 @@
 docs/Labs/broken_dogs_.txt
 docs/Labs/guestbook.txt
 docs/Labs/lab4.ipynb
 docs/Labs/lab5.ipynb
 docs/Labs/learning_python.txt
 docs/Labs/name.txt
 docs/Labs/reasons.txt
-docs/examples/ExampleBeans.ipynb
+docs/examples/CedarCubMuck.dbf
+docs/examples/CedarCubMuck.shp
+docs/examples/ExampleBeansLab7.ipynb
+docs/examples/StudyArea.geojson
+docs/examples/classnotes.ipynb
+docs/examples/csv.ipynb
 docs/examples/europe_110.geo.json
 docs/examples/intro.ipynb
 docs/examples/ipyleaflet.ipynb
+docs/examples/raster.ipynb
+docs/examples/us_regions.geojson
+docs/examples/vector.ipynb
 docs/overrides/main.html
 tests/__init__.py
 tests/test_thebeans.py
+thebeans/CSVtoDF.py
 thebeans/__init__.py
 thebeans/common.py
 thebeans/thebeans.py
```

### Comparing `TheBeans-0.0.6/docs/Labs/lab4.ipynb` & `TheBeans-0.0.7/docs/Labs/lab4.ipynb`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/docs/Labs/lab5.ipynb` & `TheBeans-0.0.7/docs/Labs/lab5.ipynb`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/docs/contributing.md` & `TheBeans-0.0.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/docs/examples/europe_110.geo.json` & `TheBeans-0.0.7/docs/examples/europe_110.geo.json`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/docs/examples/ipyleaflet.ipynb` & `TheBeans-0.0.7/docs/examples/ipyleaflet.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9879687500000001%*

 * *Differences: {"'cells'": "{0: {'execution_count': 4, 'outputs': {0: {'traceback': {insert: [(2, 'Cell "*

 * *            '\\x1b[1;32mIn[4], line 9\\x1b[0m\\n\\x1b[0;32m      2\\x1b[0m '*

 * *            '\\x1b[38;5;28;01mfrom\\x1b[39;00m \\x1b[38;5;21;01mthebeans\\x1b[39;00m '*

 * *            '\\x1b[38;5;28;01mimport\\x1b[39;00m Map\\n\\x1b[0;32m      6\\x1b[0m m '*

 * *            '\\x1b[38;5;241m=\\x1b[39m '*

 * *            'Map(basemap\\x1b[38;5;241m=\\x1b[39mbasemaps\\x1b[38;5;241m.\\x1b[39mNASAGIBS\\x1b[38;5;241m.\\x1b[39mViirsTrueColorC […]*

```diff
@@ -1,74 +1,102 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "ename": "NameError",
                     "evalue": "name 'center' is not defined",
                     "output_type": "error",
                     "traceback": [
                         "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
                         "\u001b[1;31mNameError\u001b[0m                                 Traceback (most recent call last)",
-                        "Cell \u001b[1;32mIn[2], line 5\u001b[0m\n\u001b[0;32m      1\u001b[0m \u001b[38;5;28;01mimport\u001b[39;00m \u001b[38;5;21;01mthebeans\u001b[39;00m\n\u001b[0;32m      2\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mipyleaflet\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m Map, Marker, basemaps\n\u001b[1;32m----> 5\u001b[0m m \u001b[38;5;241m=\u001b[39m Map(basemap\u001b[38;5;241m=\u001b[39mbasemaps\u001b[38;5;241m.\u001b[39mNASAGIBS\u001b[38;5;241m.\u001b[39mViirsTrueColorCR, center\u001b[38;5;241m=\u001b[39m\u001b[43mcenter\u001b[49m, zoom\u001b[38;5;241m=\u001b[39m\u001b[38;5;241m8\u001b[39m)\n\u001b[0;32m      8\u001b[0m marker \u001b[38;5;241m=\u001b[39m Marker(location\u001b[38;5;241m=\u001b[39mcenter, draggable\u001b[38;5;241m=\u001b[39m\u001b[38;5;28;01mTrue\u001b[39;00m)\n\u001b[0;32m      9\u001b[0m m\u001b[38;5;241m.\u001b[39madd(marker);\n",
+                        "Cell \u001b[1;32mIn[4], line 9\u001b[0m\n\u001b[0;32m      2\u001b[0m \u001b[38;5;28;01mfrom\u001b[39;00m \u001b[38;5;21;01mthebeans\u001b[39;00m \u001b[38;5;28;01mimport\u001b[39;00m Map\n\u001b[0;32m      6\u001b[0m m \u001b[38;5;241m=\u001b[39m Map(basemap\u001b[38;5;241m=\u001b[39mbasemaps\u001b[38;5;241m.\u001b[39mNASAGIBS\u001b[38;5;241m.\u001b[39mViirsTrueColorCR)\n\u001b[1;32m----> 9\u001b[0m marker \u001b[38;5;241m=\u001b[39m Marker(location \u001b[38;5;241m=\u001b[39m \u001b[43mcenter\u001b[49m, draggable\u001b[38;5;241m=\u001b[39m\u001b[38;5;28;01mTrue\u001b[39;00m)\n\u001b[0;32m     10\u001b[0m m\u001b[38;5;241m.\u001b[39madd(marker);\n\u001b[0;32m     12\u001b[0m display(m)\n",
                         "\u001b[1;31mNameError\u001b[0m: name 'center' is not defined"
                     ]
                 }
             ],
             "source": [
-                "import ipyleaflet\n",
-                "from ipyleaflet import Map, Marker, basemaps\n",
+                "import thebeans\n",
+                "from thebeans import Map\n",
                 "\n",
                 "\n",
-                "m = Map(basemap=basemaps.NASAGIBS.ViirsTrueColorCR, center=center, zoom=8)\n",
                 "\n",
+                "m = Map(\n",
+                "    basemap=basemaps.NASAGIBS.ViirsTrueColorCR\n",
+                "    center =\n",
+                "    zoom =\n",
+                ")\n",
                 "\n",
-                "marker = Marker(location=center, draggable=True)\n",
+                "\n",
+                "marker = Marker(location = center, draggable=True)\n",
                 "m.add(marker);\n",
                 "\n",
                 "display(m)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 7,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'https://a.tile.opentopomap.org/{z}/{x}/{y}.png'"
+                        ]
+                    },
+                    "execution_count": 7,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "eval(\"basemaps.OpenTopoMap\").build_url() #gets URL to add to tile layer"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 8,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "ename": "AttributeError",
+                    "evalue": "'tuple' object has no attribute 'interact'",
+                    "output_type": "error",
+                    "traceback": [
+                        "\u001b[1;31m---------------------------------------------------------------------------\u001b[0m",
+                        "\u001b[1;31mAttributeError\u001b[0m                            Traceback (most recent call last)",
+                        "Cell \u001b[1;32mIn[8], line 2\u001b[0m\n\u001b[0;32m      1\u001b[0m m\u001b[38;5;241m.\u001b[39mlayers\n\u001b[1;32m----> 2\u001b[0m \u001b[43mm\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43mlayers\u001b[49m\u001b[38;5;241;43m.\u001b[39;49m\u001b[43minteract\u001b[49m(opacity\u001b[38;5;241m=\u001b[39m(\u001b[38;5;241m0.0\u001b[39m,\u001b[38;5;241m1.0\u001b[39m,\u001b[38;5;241m0.1\u001b[39m))\n",
+                        "\u001b[1;31mAttributeError\u001b[0m: 'tuple' object has no attribute 'interact'"
+                    ]
+                }
+            ],
             "source": [
                 "m.layers\n",
                 "m.layers.interact(opacity=(0.0,1.0,0.1))"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
                 "m  = thebeans.Map() # not sure what\n",
                 "\n",
                 "url = \"https://mt1.google.com/vt/lyrs=y&x={col}&y={row}&z={level}\"\n",
                 "Tile = ipyleaflet.TileLayer(url=url, name=\"Google Hyybrid\", opacity=1)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#removes data credits at bottom. Takes slice of tuple that map is referencing\n",
                 "m.controls = m.controls[:1]\n"
             ]
         },
```

### Comparing `TheBeans-0.0.6/docs/installation.md` & `TheBeans-0.0.7/docs/installation.md`

 * *Files identical despite different names*

### Comparing `TheBeans-0.0.6/mkdocs.yml` & `TheBeans-0.0.7/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -72,15 +72,18 @@
     - Installation: installation.md
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/phillipslucas/TheBeans/issues
     - Examples:
-        - examples/intro.ipynb
+        - examples/ExampleBeansLab7.ipynb
+        - examples/csv.ipynb
+        - examples/vector.ipynb
     - API Reference:
           - thebeans module: thebeans.md
           - common module: common.md
+          - CSVtoDF module: CSVtoDF.md
     - Labs:
         - Labs/lab4.ipynb
         - Labs/lab5.ipynb
```

### Comparing `TheBeans-0.0.6/pyproject.toml` & `TheBeans-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "TheBeans"
-version = "0.0.6"
+version = "0.0.7"
 dynamic = [
     "dependencies",
 ]
 description = "Python package with the beans."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.6"
+current_version = "0.0.7"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

