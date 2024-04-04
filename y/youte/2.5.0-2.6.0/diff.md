# Comparing `tmp/youte-2.5.0.tar.gz` & `tmp/youte-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youte-2.5.0.tar", last modified: Wed Mar 27 03:06:45 2024, max compression
+gzip compressed data, was "youte-2.6.0.tar", last modified: Thu Apr  4 04:55:16 2024, max compression
```

## Comparing `youte-2.5.0.tar` & `youte-2.6.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-03-27 03:06:45.988499 youte-2.5.0/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1858 2023-02-16 01:17:30.000000 youte-2.5.0/.gitignore
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      198 2023-08-28 04:10:23.000000 youte-2.5.0/.readthedocs.yaml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     5832 2023-05-22 01:08:56.000000 youte-2.5.0/CHANGELOG.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1081 2022-06-06 05:38:09.000000 youte-2.5.0/LICENCE
--rw-r--r--   0 boyd      (1000) boyd      (1000)    17163 2024-03-27 03:06:45.988499 youte-2.5.0/PKG-INFO
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    16257 2023-05-16 23:00:47.000000 youte-2.5.0/README.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-03-27 03:06:45.980499 youte-2.5.0/docs/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    37494 2023-08-28 06:19:58.000000 youte-2.5.0/docs/documentation.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-03-27 03:06:45.988499 youte-2.5.0/docs/images/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    23688 2023-02-16 01:17:30.000000 youte-2.5.0/docs/images/youte-logo-black-transparent.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     7979 2023-02-16 01:17:30.000000 youte-2.5.0/docs/images/youte-logo-white-transparent-1x.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    24570 2023-02-16 01:17:30.000000 youte-2.5.0/docs/images/youte-logo-white-transparent.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    82963 2023-03-14 23:29:14.000000 youte-2.5.0/docs/images/youte_save_progress.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)   762396 2023-03-17 03:28:46.000000 youte-2.5.0/docs/images/youte_search_results.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)   183270 2023-03-17 03:37:54.000000 youte-2.5.0/docs/images/youte_search_results_pretty.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    67111 2023-05-15 01:12:17.000000 youte-2.5.0/docs/images/youte_thumbnail.png
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     4122 2023-05-16 23:00:47.000000 youte-2.5.0/docs/index.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       56 2023-03-17 06:57:11.000000 youte-2.5.0/docs/reference.md
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-03-27 03:06:45.988499 youte-2.5.0/docs/stylesheets/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      163 2023-02-16 01:17:30.000000 youte-2.5.0/docs/stylesheets/extra.css
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    14669 2023-03-17 05:20:49.000000 youte-2.5.0/docs/tutorial.md
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1243 2023-08-28 06:36:29.000000 youte-2.5.0/mkdocs.yml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      479 2023-08-28 06:19:58.000000 youte-2.5.0/noxfile.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      231 2023-04-14 05:35:56.000000 youte-2.5.0/pyproject.toml
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      572 2023-03-20 05:22:46.000000 youte-2.5.0/requirements-mkdocs.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1027 2024-03-27 03:06:45.992499 youte-2.5.0/setup.cfg
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1363 2024-03-27 03:05:15.000000 youte-2.5.0/setup.py
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-03-27 03:06:45.980499 youte-2.5.0/src/
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-03-27 03:06:45.988499 youte-2.5.0/src/youte/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        0 2023-04-27 05:21:18.000000 youte-2.5.0/src/youte/__init__.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1253 2023-04-14 05:35:56.000000 youte-2.5.0/src/youte/_logging.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      967 2023-05-16 23:00:47.000000 youte-2.5.0/src/youte/_typing.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    37451 2024-03-27 03:04:07.000000 youte-2.5.0/src/youte/cli.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    28835 2023-05-16 23:00:47.000000 youte-2.5.0/src/youte/collector.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1804 2024-03-27 03:04:07.000000 youte-2.5.0/src/youte/common.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1269 2023-03-16 07:04:20.000000 youte-2.5.0/src/youte/config.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    12937 2023-04-14 05:35:56.000000 youte-2.5.0/src/youte/database.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      359 2023-05-16 23:00:47.000000 youte-2.5.0/src/youte/exceptions.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)    15153 2024-03-27 03:04:07.000000 youte-2.5.0/src/youte/parser.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3274 2023-10-24 05:18:36.000000 youte-2.5.0/src/youte/resources.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3911 2023-08-28 06:19:58.000000 youte-2.5.0/src/youte/utilities.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      189 2024-03-27 03:05:08.000000 youte-2.5.0/src/youte/version.py
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-03-27 03:06:45.988499 youte-2.5.0/src/youte.egg-info/
--rw-r--r--   0 boyd      (1000) boyd      (1000)    17163 2024-03-27 03:06:45.000000 youte-2.5.0/src/youte.egg-info/PKG-INFO
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     1087 2024-03-27 03:06:45.000000 youte-2.5.0/src/youte.egg-info/SOURCES.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        1 2024-03-27 03:06:45.000000 youte-2.5.0/src/youte.egg-info/dependency_links.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)       42 2024-03-27 03:06:45.000000 youte-2.5.0/src/youte.egg-info/entry_points.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)      147 2024-03-27 03:06:45.000000 youte-2.5.0/src/youte.egg-info/requires.txt
--rw-rw-r--   0 boyd      (1000) boyd      (1000)        6 2024-03-27 03:06:45.000000 youte-2.5.0/src/youte.egg-info/top_level.txt
-drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-03-27 03:06:45.988499 youte-2.5.0/tests/
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     2817 2023-05-22 01:08:56.000000 youte-2.5.0/tests/test_archive.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     9741 2023-08-28 06:19:58.000000 youte-2.5.0/tests/test_cli.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3184 2023-08-28 06:19:58.000000 youte-2.5.0/tests/test_collector.py
--rw-rw-r--   0 boyd      (1000) boyd      (1000)     3051 2023-08-28 06:19:58.000000 youte-2.5.0/tests/test_parser.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-04-04 04:55:16.218936 youte-2.6.0/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1866 2024-03-27 03:16:48.000000 youte-2.6.0/.gitignore
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      198 2023-08-28 04:10:23.000000 youte-2.6.0/.readthedocs.yaml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     5832 2023-05-22 01:08:56.000000 youte-2.6.0/CHANGELOG.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1081 2022-06-06 05:38:09.000000 youte-2.6.0/LICENCE
+-rw-r--r--   0 boyd      (1000) boyd      (1000)    17491 2024-04-04 04:55:16.218936 youte-2.6.0/PKG-INFO
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    16584 2024-04-04 04:55:03.000000 youte-2.6.0/README.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-04-04 04:55:16.210936 youte-2.6.0/docs/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    38355 2024-04-04 04:55:03.000000 youte-2.6.0/docs/documentation.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-04-04 04:55:16.218936 youte-2.6.0/docs/images/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    23688 2023-02-16 01:17:30.000000 youte-2.6.0/docs/images/youte-logo-black-transparent.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     7979 2023-02-16 01:17:30.000000 youte-2.6.0/docs/images/youte-logo-white-transparent-1x.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    24570 2023-02-16 01:17:30.000000 youte-2.6.0/docs/images/youte-logo-white-transparent.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    82963 2023-03-14 23:29:14.000000 youte-2.6.0/docs/images/youte_save_progress.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)   762396 2023-03-17 03:28:46.000000 youte-2.6.0/docs/images/youte_search_results.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)   183270 2023-03-17 03:37:54.000000 youte-2.6.0/docs/images/youte_search_results_pretty.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    67111 2023-05-15 01:12:17.000000 youte-2.6.0/docs/images/youte_thumbnail.png
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     4122 2023-05-16 23:00:47.000000 youte-2.6.0/docs/index.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)       56 2023-03-17 06:57:11.000000 youte-2.6.0/docs/reference.md
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-04-04 04:55:16.218936 youte-2.6.0/docs/stylesheets/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      163 2023-02-16 01:17:30.000000 youte-2.6.0/docs/stylesheets/extra.css
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    14669 2023-03-17 05:20:49.000000 youte-2.6.0/docs/tutorial.md
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1243 2023-08-28 06:36:29.000000 youte-2.6.0/mkdocs.yml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      479 2023-08-28 06:19:58.000000 youte-2.6.0/noxfile.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      231 2023-04-14 05:35:56.000000 youte-2.6.0/pyproject.toml
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      572 2023-03-20 05:22:46.000000 youte-2.6.0/requirements-mkdocs.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1027 2024-04-04 04:55:16.218936 youte-2.6.0/setup.cfg
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1363 2024-04-04 04:55:03.000000 youte-2.6.0/setup.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-04-04 04:55:16.210936 youte-2.6.0/src/
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-04-04 04:55:16.218936 youte-2.6.0/src/youte/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        0 2023-04-27 05:21:18.000000 youte-2.6.0/src/youte/__init__.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1253 2023-04-14 05:35:56.000000 youte-2.6.0/src/youte/_logging.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      967 2023-05-16 23:00:47.000000 youte-2.6.0/src/youte/_typing.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    37934 2024-04-04 04:55:03.000000 youte-2.6.0/src/youte/cli.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    29776 2024-04-04 04:55:03.000000 youte-2.6.0/src/youte/collector.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1804 2024-03-27 03:04:07.000000 youte-2.6.0/src/youte/common.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1269 2023-03-16 07:04:20.000000 youte-2.6.0/src/youte/config.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    12937 2023-04-14 05:35:56.000000 youte-2.6.0/src/youte/database.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      359 2023-05-16 23:00:47.000000 youte-2.6.0/src/youte/exceptions.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    15153 2024-03-27 03:04:07.000000 youte-2.6.0/src/youte/parser.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3274 2023-10-24 05:18:36.000000 youte-2.6.0/src/youte/resources.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3911 2023-08-28 06:19:58.000000 youte-2.6.0/src/youte/utilities.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      189 2024-04-04 04:55:03.000000 youte-2.6.0/src/youte/version.py
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-04-04 04:55:16.218936 youte-2.6.0/src/youte.egg-info/
+-rw-r--r--   0 boyd      (1000) boyd      (1000)    17491 2024-04-04 04:55:16.000000 youte-2.6.0/src/youte.egg-info/PKG-INFO
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     1087 2024-04-04 04:55:16.000000 youte-2.6.0/src/youte.egg-info/SOURCES.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        1 2024-04-04 04:55:16.000000 youte-2.6.0/src/youte.egg-info/dependency_links.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)       42 2024-04-04 04:55:16.000000 youte-2.6.0/src/youte.egg-info/entry_points.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)      147 2024-04-04 04:55:16.000000 youte-2.6.0/src/youte.egg-info/requires.txt
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)        6 2024-04-04 04:55:16.000000 youte-2.6.0/src/youte.egg-info/top_level.txt
+drwxrwxr-x   0 boyd      (1000) boyd      (1000)        0 2024-04-04 04:55:16.218936 youte-2.6.0/tests/
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     2817 2023-05-22 01:08:56.000000 youte-2.6.0/tests/test_archive.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)    12107 2024-04-04 04:55:03.000000 youte-2.6.0/tests/test_cli.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3640 2024-04-04 04:55:03.000000 youte-2.6.0/tests/test_collector.py
+-rw-rw-r--   0 boyd      (1000) boyd      (1000)     3051 2023-08-28 06:19:58.000000 youte-2.6.0/tests/test_parser.py
```

### Comparing `youte-2.5.0/.gitignore` & `youte-2.6.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+.pypirc
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
```

### Comparing `youte-2.5.0/CHANGELOG.md` & `youte-2.6.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/LICENCE` & `youte-2.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/PKG-INFO` & `youte-2.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youte
-Version: 2.5.0
+Version: 2.6.0
 Summary: Command-line tool to collect video metadata and comments from Youtube API
 Home-page: https://github.com/QUT-Digital-Observatory/youte
 Author: Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -29,30 +29,15 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/youte?period=month&units=international_system&left_color=black&right_color=orange&left_text=Monthly%20PyPI%20downloads)](https://pepy.tech/project/youte)
 [![Licence](https://img.shields.io/github/license/QUT-Digital-Observatory/youte)](LICENCE)
 ![Supported Versions](https://img.shields.io/pypi/pyversions/youte)
 ![Development Status](https://img.shields.io/pypi/status/youte)
 
 ![](docs/images/youte_thumbnail.png)
 
-## Changes from youte 1.3.0
-
-Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion, some commands have been changed.
-
-- `youte hydrate` is now broken down to `youte videos` and `youte channels`.
-- `youte get-comments` is now `youte comments` and `youte replies`.
-- `youte most-popular` is now `youte chart`.
-- `youte get-related` is now `youte related-to`.
-
-Furthermore:
-
-- Resuming search is no longer available. Instead, you can set a limit on the number of search pages returned to avoid exhausting your API quota.
-- All youte commands that retrieve data from YouTube API now won't print results to the shell, but store them in a specified json or jsonl file. This is to avoid clogging up the shell.
-- You can now tidy data into a CSV or a flat JSON array.
-
-Big thanks to @Lingomat (Mat Bettinson) for code review and suggestions.
+Big thanks to [@Lingomat](https://github.com/Lingomat) (Mat Bettinson) for code review and suggestions.
 
 ## Installation
 
 ```bash
 python -m pip install youte
 ```  
 
@@ -146,14 +131,20 @@
 
 Raw JSONs from YouTube API contain request metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
 
 ```bash
 youte search <search-terms> --tidy-to <file.csv>
 ```
 
+You can specify the encoding for the CSV. By default, `youte` uses `utf-8-sig` for compatibility with Excel readers. To change this, use the `--encoding` argument.
+
+```bash
+youte search <search-terms> --tidy-to <file.csv> --encoding "utf-8"
+```
+
 Specify `--format json` if you want to tidy raw data into an array of flat JSON objects.
 
 ```bash
 youte search <search-terms> --tidy-to <file-name.json> --format json
 ```
 
 `--tidy-to` option is available for all `youte` commands that retrieve data, and works the same way.
@@ -258,15 +249,31 @@
 youte hydrate -f <id-file.csv>
 ```
 
 This option is often used in combination with `youte dehydrate`, which retrieves the ids from raw JSON returned by `youte search` and stores them in a text file.
 
 ## channels
 
-`youte channels` works the same as `youte videos`, except it retrieves channel metadata given channel ids.
+`youte channels` works the same as `youte videos`, except it retrieves channel metadata from channel ids.
+
+You can either hydrate channels by channel IDs, or *handles*, i.e. @stanfordgsb. To pass handles, use the option `--handles` followed by a comma separated list of handles, each prefererably prepended by `@`. For example:
+
+```shell
+youte channels --handles @stanfordgsb,@TED,@TEDEd -o <file.json>
+```
+
+To use a file containing handles, pass `--handle-file`.
+
+You can hydrate both channel IDs and handles in one command:
+
+```shell
+youte channels -f <id-file.csv> --handles @stanfordgsb,@TED,@TEDEd -o <file.json>
+```
+
+This will hydrate both the channel IDs in the file and the handles specified in the terminal.
 
 ## comments
 
 `youte comments` retrieves top-level comments (comment threads) on one or multiple videos or channels. It takes in a list of ids and a flag indicating which type these ids are (i.e. videos or channels).
 
 To retrieve comments on videos, specify the video ids and pass the `--by-video-id` or `-v` flag.
 
@@ -296,36 +303,14 @@
 
 While `youte comments` only retrieve top-level comment threads, if those threads have replies, they can be retrieved using `youte replies`. `youte replies` takes a list of thread ids and return the replies to those threads.
 
 ```shell
 youte replies <ids>... --outfile <file.json>
 ```
 
-## related-to
-
-`related-to` retrieves videos related to a video.
-
-```shell
-youte related-to <video-ids>... -o <file.json>
-```
-
-If multiple video IDs are inputted, youte will iterate through each video ID separately, retrieving all related videos to each video, one by one.
-
-Other options include:
-
-```{.bash .no-copy}
-  --safe-search [none|moderate|strict]
-                                  Include or exclude restricted content
-                                  [default: none]
-  --region TEXT                   Specify region the videos can be viewed in
-                                  (ISO 3166-1 alpha-2 country code)
-  --lang TEXT                     Return results most relevant to a language
-                                  (ISO 639-1 two-letter code)
-```
-
 ## chart
 
 `youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
 
 For example:
 
 ```shell
@@ -360,20 +345,43 @@
 ```
 
 ```{.shell .no-copy}
 Options:
   -o, --output FILENAME  Output text file to store IDs in
 ```
 
+## related-to (deprecated)
+
+*Note.* **From August 7, 2023, this endpoint was deprecated by YouTube. This command is no longer usable.**
+
+`youte related-to` retrieves a list of videos related to a video.
+
+```shell
+youte related-to <video-ids>... -o <file.json>
+```
+
+You can pass one or many video IDs. If multiple video IDs are inputted, youte will iterate through those video IDs, retrieving all related videos to each video separately. The end result contains both the related videos and the id of the video that they are related to.
+
+Other options include:
+
+```{.bash .no-copy}
+  --safe-search [none|moderate|strict]
+                                  Include or exclude restricted content
+                                  [default: none]
+  --region TEXT                   Specify region the videos can be viewed in
+                                  (ISO 3166-1 alpha-2 country code)
+  --lang TEXT                     Return results most relevant to a language
+                                  (ISO 639-1 two-letter code)
+```
+
 ## YouTube API Quota system and youte handling of quota 
 
 Most often, there is a limit to how many requests you can make to YouTube API per day. YouTube Data API uses a quota system, whereby each request costs a number of units depending on the endpoint the request is made to.
 
 For example:  
 
 - search endpoint costs 100 units per request  
 - video, channel, commentThread, and comment endpoints each costs 1 unit per request  
 
 Free accounts get an API quota cap of 10,000 units per project per day, which resets at midnight Pacific Time.
 
 At present, you can only check your quota usage on the [Quotas](https://console.developers.google.com/iam-admin/quotas) page in the API Console. It is not possible to monitor quota usage via metadata returned in the API response. `youte` does not monitor quota usage.
-
```

### Comparing `youte-2.5.0/README.md` & `youte-2.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,15 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/youte?period=month&units=international_system&left_color=black&right_color=orange&left_text=Monthly%20PyPI%20downloads)](https://pepy.tech/project/youte)
 [![Licence](https://img.shields.io/github/license/QUT-Digital-Observatory/youte)](LICENCE)
 ![Supported Versions](https://img.shields.io/pypi/pyversions/youte)
 ![Development Status](https://img.shields.io/pypi/status/youte)
 
 ![](docs/images/youte_thumbnail.png)
 
-## Changes from youte 1.3.0
-
-Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion, some commands have been changed.
-
-- `youte hydrate` is now broken down to `youte videos` and `youte channels`.
-- `youte get-comments` is now `youte comments` and `youte replies`.
-- `youte most-popular` is now `youte chart`.
-- `youte get-related` is now `youte related-to`.
-
-Furthermore:
-
-- Resuming search is no longer available. Instead, you can set a limit on the number of search pages returned to avoid exhausting your API quota.
-- All youte commands that retrieve data from YouTube API now won't print results to the shell, but store them in a specified json or jsonl file. This is to avoid clogging up the shell.
-- You can now tidy data into a CSV or a flat JSON array.
-
-Big thanks to @Lingomat (Mat Bettinson) for code review and suggestions.
+Big thanks to [@Lingomat](https://github.com/Lingomat) (Mat Bettinson) for code review and suggestions.
 
 ## Installation
 
 ```bash
 python -m pip install youte
 ```  
 
@@ -122,14 +107,20 @@
 
 Raw JSONs from YouTube API contain request metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
 
 ```bash
 youte search <search-terms> --tidy-to <file.csv>
 ```
 
+You can specify the encoding for the CSV. By default, `youte` uses `utf-8-sig` for compatibility with Excel readers. To change this, use the `--encoding` argument.
+
+```bash
+youte search <search-terms> --tidy-to <file.csv> --encoding "utf-8"
+```
+
 Specify `--format json` if you want to tidy raw data into an array of flat JSON objects.
 
 ```bash
 youte search <search-terms> --tidy-to <file-name.json> --format json
 ```
 
 `--tidy-to` option is available for all `youte` commands that retrieve data, and works the same way.
@@ -234,15 +225,31 @@
 youte hydrate -f <id-file.csv>
 ```
 
 This option is often used in combination with `youte dehydrate`, which retrieves the ids from raw JSON returned by `youte search` and stores them in a text file.
 
 ## channels
 
-`youte channels` works the same as `youte videos`, except it retrieves channel metadata given channel ids.
+`youte channels` works the same as `youte videos`, except it retrieves channel metadata from channel ids.
+
+You can either hydrate channels by channel IDs, or *handles*, i.e. @stanfordgsb. To pass handles, use the option `--handles` followed by a comma separated list of handles, each prefererably prepended by `@`. For example:
+
+```shell
+youte channels --handles @stanfordgsb,@TED,@TEDEd -o <file.json>
+```
+
+To use a file containing handles, pass `--handle-file`.
+
+You can hydrate both channel IDs and handles in one command:
+
+```shell
+youte channels -f <id-file.csv> --handles @stanfordgsb,@TED,@TEDEd -o <file.json>
+```
+
+This will hydrate both the channel IDs in the file and the handles specified in the terminal.
 
 ## comments
 
 `youte comments` retrieves top-level comments (comment threads) on one or multiple videos or channels. It takes in a list of ids and a flag indicating which type these ids are (i.e. videos or channels).
 
 To retrieve comments on videos, specify the video ids and pass the `--by-video-id` or `-v` flag.
 
@@ -272,36 +279,14 @@
 
 While `youte comments` only retrieve top-level comment threads, if those threads have replies, they can be retrieved using `youte replies`. `youte replies` takes a list of thread ids and return the replies to those threads.
 
 ```shell
 youte replies <ids>... --outfile <file.json>
 ```
 
-## related-to
-
-`related-to` retrieves videos related to a video.
-
-```shell
-youte related-to <video-ids>... -o <file.json>
-```
-
-If multiple video IDs are inputted, youte will iterate through each video ID separately, retrieving all related videos to each video, one by one.
-
-Other options include:
-
-```{.bash .no-copy}
-  --safe-search [none|moderate|strict]
-                                  Include or exclude restricted content
-                                  [default: none]
-  --region TEXT                   Specify region the videos can be viewed in
-                                  (ISO 3166-1 alpha-2 country code)
-  --lang TEXT                     Return results most relevant to a language
-                                  (ISO 639-1 two-letter code)
-```
-
 ## chart
 
 `youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
 
 For example:
 
 ```shell
@@ -336,20 +321,43 @@
 ```
 
 ```{.shell .no-copy}
 Options:
   -o, --output FILENAME  Output text file to store IDs in
 ```
 
+## related-to (deprecated)
+
+*Note.* **From August 7, 2023, this endpoint was deprecated by YouTube. This command is no longer usable.**
+
+`youte related-to` retrieves a list of videos related to a video.
+
+```shell
+youte related-to <video-ids>... -o <file.json>
+```
+
+You can pass one or many video IDs. If multiple video IDs are inputted, youte will iterate through those video IDs, retrieving all related videos to each video separately. The end result contains both the related videos and the id of the video that they are related to.
+
+Other options include:
+
+```{.bash .no-copy}
+  --safe-search [none|moderate|strict]
+                                  Include or exclude restricted content
+                                  [default: none]
+  --region TEXT                   Specify region the videos can be viewed in
+                                  (ISO 3166-1 alpha-2 country code)
+  --lang TEXT                     Return results most relevant to a language
+                                  (ISO 639-1 two-letter code)
+```
+
 ## YouTube API Quota system and youte handling of quota 
 
 Most often, there is a limit to how many requests you can make to YouTube API per day. YouTube Data API uses a quota system, whereby each request costs a number of units depending on the endpoint the request is made to.
 
 For example:  
 
 - search endpoint costs 100 units per request  
 - video, channel, commentThread, and comment endpoints each costs 1 unit per request  
 
 Free accounts get an API quota cap of 10,000 units per project per day, which resets at midnight Pacific Time.
 
-At present, you can only check your quota usage on the [Quotas](https://console.developers.google.com/iam-admin/quotas) page in the API Console. It is not possible to monitor quota usage via metadata returned in the API response. `youte` does not monitor quota usage.
-
+At present, you can only check your quota usage on the [Quotas](https://console.developers.google.com/iam-admin/quotas) page in the API Console. It is not possible to monitor quota usage via metadata returned in the API response. `youte` does not monitor quota usage.
```

### Comparing `youte-2.5.0/docs/documentation.md` & `youte-2.6.0/docs/documentation.md`

 * *Files 3% similar despite different names*

```diff
@@ -116,27 +116,33 @@
 youte search <search-terms> --max-pages 5
 # OR
 youte search <search-terms> -m 5
 ```
 
 ### Tidy data
 
-Raw JSONs from YouTube API contain query metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy data into will be CSV.
+Raw JSONs from YouTube API contain request metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
 
 ```bash
 youte search <search-terms> --tidy-to <file.csv>
 ```
 
+You can specify the encoding for the CSV. By default, `youte` uses `utf-8-sig` for compatibility with Excel readers. To change this, use the `--encoding` argument.
+
+```bash
+youte search <search-terms> --tidy-to <file.csv> --encoding "utf-8"
+```
+
 Specify `--format json` if you want to tidy raw data into an array of flat JSON objects.
 
 ```bash
 youte search <search-terms> --tidy-to <file-name.json> --format json
 ```
 
-`--tidy-to` option is available for and works the same across all `youte` commands that retrieve data.
+`--tidy-to` option is available for all `youte` commands that retrieve data, and works the same way.
 
 ### Advanced search
 
 There are multiple filters to refine your search. A full list of these are provided below:
 
 ``` {.bash .no-copy}
 Options:
@@ -236,14 +242,30 @@
 
 This option is often used in combination with `youte dehydrate`, which retrieves the ids from results returned by `youte search` and stores them in a text file.
 
 ## channels
 
 `youte channels` works the same as `youte videos`, except it retrieves channel metadata from channel ids.
 
+You can either hydrate channels by channel IDs, or *handles*, i.e. @stanfordgsb. To pass handles, use the option `--handles` followed by a comma separated list of handles, each prefererably prepended by `@`. For example:
+
+```shell
+youte channels --handles @stanfordgsb,@TED,@TEDEd -o <file.json>
+```
+
+To use a file containing handles, pass `--handle-file`.
+
+You can hydrate both channel IDs and handles in one command:
+
+```shell
+youte channels -f <id-file.csv> --handles @stanfordgsb,@TED,@TEDEd -o <file.json>
+```
+
+This will hydrate both the channel IDs in the file and the handles specified in the terminal.
+
 ## comments
 
 `youte comments` retrieves top-level comments (comment threads) on videos or channels. It takes in a list of video or channel ids, followed by a flag indicating the type of these ids (i.e. videos or channels). Only one type of ids should be specified.
 
 To retrieve comments on videos, specify the video ids and pass the `--by-video-id` or `-v` flag.
 
 ```shell
@@ -437,15 +459,15 @@
 ### Parsing
 
 Results returned from the `search()` are standard Python dictionaries, so you can extract the attributes and tidy them as you want. A better way of processing these dictionaries is to use `youte.parser`, which processes these results and returns a Resources object. A Resources object can be a `Searches`, `Videos`, `Channels`, or `Comments` object.
 
 Each resource type has its corresponding parser function. (A potential improvement in the future is to have one all-encompassing parser function that detects resource type and parses data accordingly.) The table below lists out the resulting resource type from each `Youte` methods and its corresponding parser function.
 
 | `Youte` method         | Resulting resource type | Parser function | Object returned from parser function |
-|------------------------|-------------------------|-----------------|--------------------------------------|
+| ---------------------- | ----------------------- | --------------- | ------------------------------------ |
 | search()               | search                  | parse_searches  | `Searches`                           |
 | get_video_metadata()   | video                   | parse_videos    | `Videos`                             |
 | get_channel_metadata() | channel                 | parse_channels  | `Channels`                           |
 | get_comment_threads()  | comment                 | parse_comments  | `Comments`                           |
 | get_thread_replies()   | comment                 | parse_comments  | `Comments`                           |
 | get_most_popular()     | video                   | parse_videos    | `Videos`                             |
 | get_related_videos()   | search                  | parse_searches  | `Searches`                           |
```

### Comparing `youte-2.5.0/docs/images/youte-logo-black-transparent.png` & `youte-2.6.0/docs/images/youte-logo-black-transparent.png`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/docs/images/youte-logo-white-transparent-1x.png` & `youte-2.6.0/docs/images/youte-logo-white-transparent-1x.png`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/docs/images/youte-logo-white-transparent.png` & `youte-2.6.0/docs/images/youte-logo-white-transparent.png`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/docs/images/youte_save_progress.png` & `youte-2.6.0/docs/images/youte_save_progress.png`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/docs/images/youte_search_results.png` & `youte-2.6.0/docs/images/youte_search_results.png`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/docs/images/youte_search_results_pretty.png` & `youte-2.6.0/docs/images/youte_search_results_pretty.png`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/docs/images/youte_thumbnail.png` & `youte-2.6.0/docs/images/youte_thumbnail.png`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/docs/index.md` & `youte-2.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/docs/tutorial.md` & `youte-2.6.0/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/mkdocs.yml` & `youte-2.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/requirements-mkdocs.txt` & `youte-2.6.0/requirements-mkdocs.txt`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/setup.cfg` & `youte-2.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/setup.py` & `youte-2.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "2.5.0"
+__version__ = "2.6.0"
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 if __name__ == "__main__":
     setup(
         name="youte",
```

### Comparing `youte-2.5.0/src/youte/_logging.py` & `youte-2.6.0/src/youte/_logging.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/src/youte/_typing.py` & `youte-2.6.0/src/youte/_typing.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/src/youte/cli.py` & `youte-2.6.0/src/youte/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import youte.parser as parser
 from youte._logging import MultiFormatter
 from youte.collector import Youte
 from youte.common import Resources
 from youte.config import YouteConfig
 from youte.exceptions import ValueAlreadyExists
 from youte.utilities import export_file, retrieve_ids_from_file, validate_date_string
+from youte.version import user_agent, version
 
 # Logging
 
 logger = logging.getLogger()
 logging.getLogger("sqlalchemy.engine").setLevel(logging.WARNING)
 
 console_handler = logging.StreamHandler()
@@ -139,15 +140,15 @@
             raise click.Abort
     else:
         return path_value
 
 
 # CLI argument set up:
 @click.group()
-@click.version_option()
+@click.version_option(version=user_agent)
 def youte():
     """
     Utility to collect and tidy YouTube meta-data and comments via YouTube API.
     Run `youte --help` to get started.
     """
     pass
 
@@ -618,27 +619,36 @@
 @youte.command()
 @click.argument("items", nargs=-1, required=False)
 @output_options
 @tidy_options
 @default_options
 @click.option("-f", "--file-path", help="Get IDs from file", default=None)
 @click.option(
+    "--handles",
+    required=False,
+    default=None,
+    help="A comma-separated list of handles, each prepended by '@'",
+)
+@click.option("--handle-file", help="Get handles from file", default=None)
+@click.option(
     "--max-results",
     type=click.IntRange(0, 50),
     help="Maximum number of results returned per page",
     default=50,
     show_default=True,
 )
 @click_log.simple_verbosity_option(logger, "--verbosity")
 def channels(
     items: list[str],
+    handles: list[str],
     outfile: Path,
     output_format: Literal["json", "jsonl"],
     pretty: bool,
     file_path: Path,
+    handle_file: Path,
     name: str,
     key: str,
     tidy_to: Path,
     format_: Literal["json", "csv"],
     max_results: int,
     metadata: bool,
     encoding: str,
@@ -652,19 +662,20 @@
     You can use ids stored in a text file by using --file-path <FILENAME>. The file
     has to contain a line-separated list of ids, with no header.
     """
     api_key = key if key else _get_api_key(name=name)
     yob = Youte(api_key=api_key)
 
     ids = _read_ids(string=items, file=file_path)
+    handles = _read_ids(string=handles, file=handle_file)
 
     results = [
         result
         for result in yob.get_channel_metadata(
-            ids=ids, max_results=max_results, include_meta=metadata
+            ids=ids, handles=handles, max_results=max_results, include_meta=metadata
         )
     ]
 
     export_file(
         results, outfile, file_format=output_format, pretty=pretty, ensure_ascii=True
     )
 
@@ -1198,19 +1209,24 @@
 
 
 def _set_up_config(filename=_get_config_path()) -> YouteConfig:
     config_file = YouteConfig(filename=filename)
     return config_file
 
 
-def _read_ids(string: list[str] = None, file: str | Path = None) -> list[str]:
-    if not (string or file):
-        raise click.BadParameter("No ids are specified.")
+def _read_ids(
+    string: list[str] | str | None = None,
+    file: str | Path | None = None,
+) -> list[str] | None:
+    ids = None
     if string:
-        ids = list(string)
+        if isinstance(string, list):
+            ids = list(string)
+        elif isinstance(string, str):
+            ids = string.split(",")
     if file:
         with open(file, mode="r") as f:
             ids = [row.rstrip() for row in f.readlines()]
     return ids
 
 
 def _get_api_key(name=None, filename="config"):
```

### Comparing `youte-2.5.0/src/youte/collector.py` & `youte-2.6.0/src/youte/collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -216,15 +216,16 @@
             total_batches -= 1
             yield from _paginate_results(
                 url=url, include_meta=include_meta, meta=kwargs, **params
             )
 
     def get_channel_metadata(
         self,
-        ids: list[str],
+        ids: Optional[list[str]] = None,
+        handles: Optional[list[str]] = None,
         part: Optional[list[str]] = None,
         max_results: int = 50,
         include_meta: bool = True,
         **kwargs,
     ) -> Iterator[APIResponse]:
         """Retrieve full metadata for channels using their IDs.
         Currently, do not work with usernames. Channel IDs can be obtained in API
@@ -247,15 +248,26 @@
         Yields:
             Dict mappings containing API response.
 
         Raises:
             TypeError: If the value passed to ids is not a list,
                 a TypeError will be raised.
         """
+
+        if not (ids or handles):
+            raise ValueError("ids or handles must be specified")
+
+        if ids and not isinstance(ids, list):
+            raise TypeError(f"ids must be a list, got type {type(ids)}")
+
+        if handles and not isinstance(handles, list):
+            raise TypeError(f"handles must be a list, got type {type(handles)}")
+
         url: str = r"https://www.googleapis.com/youtube/v3/channels"
+
         if part is None:
             part = [
                 "snippet",
                 "statistics",
                 "topicDetails",
                 "status",
                 "contentDetails",
@@ -264,37 +276,53 @@
             ]
         params: dict = {
             "part": ",".join(part),
             "maxResults": max_results,
             "key": self.api_key,
         }
 
-        if ids and not isinstance(ids, list):
-            raise TypeError("ids and username must be a list")
-
-        total_batches: int = int(len(ids) / 50)  # logging purpose only
+        if ids:
+            total_batches: int = int(len(ids) / 50)  # logging purpose only
 
-        while ids:
-            ids = list(set(ids))
-            if len(ids) <= 50:
-                ids_string = ",".join(ids)
-                ids = []
-            else:
-                batch = random.sample(ids, k=50)
-                ids_string = ",".join(batch)
-                for elm in batch:
-                    ids.remove(elm)
-
-            params["id"] = ids_string
-            logger.info(f"Retrieving channel metadata: {total_batches} pages remaining")
-            logger.debug(f"Retrieving metadata for channels: {params['id']}")
-            total_batches -= 1
-            yield from _paginate_results(
-                url=url, include_meta=include_meta, meta=kwargs, **params
-            )
+            while ids:
+                ids = list(set(ids))
+                if len(ids) <= 50:
+                    ids_string = ",".join(ids)
+                    ids = []
+                else:
+                    batch = random.sample(ids, k=50)
+                    ids_string = ",".join(batch)
+                    for elm in batch:
+                        ids.remove(elm)
+
+                params["id"] = ids_string
+                logger.info(
+                    f"Retrieving channel metadata: {total_batches} pages remaining"
+                )
+                logger.debug(f"Retrieving metadata for channels: {params['id']}")
+                total_batches -= 1
+                yield from _paginate_results(
+                    url=url, include_meta=include_meta, meta=kwargs, **params
+                )
+
+        if handles:
+            params.pop("id", None)
+
+            i = 1
+            for handle in handles:
+
+                params["forHandle"] = handle
+                logger.info(
+                    f"{i}/{len(handles)}: Retrieving metadata for handle {handle}"
+                )
+                logger.debug(f"Query {url}: {params}")
+                i += 1
+                yield from _paginate_results(
+                    url=url, include_meta=include_meta, meta=kwargs, **params
+                )
 
     def get_comment_threads(
         self,
         video_ids: Optional[list[str]] = None,
         related_channel_ids: Optional[list[str]] = None,
         comment_ids: Optional[list[str]] = None,
         order: Literal["time", "relevance"] = "time",
```

### Comparing `youte-2.5.0/src/youte/common.py` & `youte-2.6.0/src/youte/common.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/src/youte/config.py` & `youte-2.6.0/src/youte/config.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/src/youte/database.py` & `youte-2.6.0/src/youte/database.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/src/youte/parser.py` & `youte-2.6.0/src/youte/parser.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/src/youte/resources.py` & `youte-2.6.0/src/youte/resources.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/src/youte/utilities.py` & `youte-2.6.0/src/youte/utilities.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/src/youte.egg-info/PKG-INFO` & `youte-2.6.0/src/youte.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youte
-Version: 2.5.0
+Version: 2.6.0
 Summary: Command-line tool to collect video metadata and comments from Youtube API
 Home-page: https://github.com/QUT-Digital-Observatory/youte
 Author: Digital Observatory
 Author-email: digitalobservatory@qut.edu.au
 Project-URL: Bug Tracker, https://github.com/QUT-Digital-Observatory/youte/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -29,30 +29,15 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/youte?period=month&units=international_system&left_color=black&right_color=orange&left_text=Monthly%20PyPI%20downloads)](https://pepy.tech/project/youte)
 [![Licence](https://img.shields.io/github/license/QUT-Digital-Observatory/youte)](LICENCE)
 ![Supported Versions](https://img.shields.io/pypi/pyversions/youte)
 ![Development Status](https://img.shields.io/pypi/status/youte)
 
 ![](docs/images/youte_thumbnail.png)
 
-## Changes from youte 1.3.0
-
-Several major changes are made in youte 2.0. To better correspond with YouTube API endpoints and avoid confusion, some commands have been changed.
-
-- `youte hydrate` is now broken down to `youte videos` and `youte channels`.
-- `youte get-comments` is now `youte comments` and `youte replies`.
-- `youte most-popular` is now `youte chart`.
-- `youte get-related` is now `youte related-to`.
-
-Furthermore:
-
-- Resuming search is no longer available. Instead, you can set a limit on the number of search pages returned to avoid exhausting your API quota.
-- All youte commands that retrieve data from YouTube API now won't print results to the shell, but store them in a specified json or jsonl file. This is to avoid clogging up the shell.
-- You can now tidy data into a CSV or a flat JSON array.
-
-Big thanks to @Lingomat (Mat Bettinson) for code review and suggestions.
+Big thanks to [@Lingomat](https://github.com/Lingomat) (Mat Bettinson) for code review and suggestions.
 
 ## Installation
 
 ```bash
 python -m pip install youte
 ```  
 
@@ -146,14 +131,20 @@
 
 Raw JSONs from YouTube API contain request metadata and nested fields. You can tidy these data into a CSV or a flat JSON using `--tidy-to`. The default format that youte will tidy raw JSON into will be CSV.
 
 ```bash
 youte search <search-terms> --tidy-to <file.csv>
 ```
 
+You can specify the encoding for the CSV. By default, `youte` uses `utf-8-sig` for compatibility with Excel readers. To change this, use the `--encoding` argument.
+
+```bash
+youte search <search-terms> --tidy-to <file.csv> --encoding "utf-8"
+```
+
 Specify `--format json` if you want to tidy raw data into an array of flat JSON objects.
 
 ```bash
 youte search <search-terms> --tidy-to <file-name.json> --format json
 ```
 
 `--tidy-to` option is available for all `youte` commands that retrieve data, and works the same way.
@@ -258,15 +249,31 @@
 youte hydrate -f <id-file.csv>
 ```
 
 This option is often used in combination with `youte dehydrate`, which retrieves the ids from raw JSON returned by `youte search` and stores them in a text file.
 
 ## channels
 
-`youte channels` works the same as `youte videos`, except it retrieves channel metadata given channel ids.
+`youte channels` works the same as `youte videos`, except it retrieves channel metadata from channel ids.
+
+You can either hydrate channels by channel IDs, or *handles*, i.e. @stanfordgsb. To pass handles, use the option `--handles` followed by a comma separated list of handles, each prefererably prepended by `@`. For example:
+
+```shell
+youte channels --handles @stanfordgsb,@TED,@TEDEd -o <file.json>
+```
+
+To use a file containing handles, pass `--handle-file`.
+
+You can hydrate both channel IDs and handles in one command:
+
+```shell
+youte channels -f <id-file.csv> --handles @stanfordgsb,@TED,@TEDEd -o <file.json>
+```
+
+This will hydrate both the channel IDs in the file and the handles specified in the terminal.
 
 ## comments
 
 `youte comments` retrieves top-level comments (comment threads) on one or multiple videos or channels. It takes in a list of ids and a flag indicating which type these ids are (i.e. videos or channels).
 
 To retrieve comments on videos, specify the video ids and pass the `--by-video-id` or `-v` flag.
 
@@ -296,36 +303,14 @@
 
 While `youte comments` only retrieve top-level comment threads, if those threads have replies, they can be retrieved using `youte replies`. `youte replies` takes a list of thread ids and return the replies to those threads.
 
 ```shell
 youte replies <ids>... --outfile <file.json>
 ```
 
-## related-to
-
-`related-to` retrieves videos related to a video.
-
-```shell
-youte related-to <video-ids>... -o <file.json>
-```
-
-If multiple video IDs are inputted, youte will iterate through each video ID separately, retrieving all related videos to each video, one by one.
-
-Other options include:
-
-```{.bash .no-copy}
-  --safe-search [none|moderate|strict]
-                                  Include or exclude restricted content
-                                  [default: none]
-  --region TEXT                   Specify region the videos can be viewed in
-                                  (ISO 3166-1 alpha-2 country code)
-  --lang TEXT                     Return results most relevant to a language
-                                  (ISO 639-1 two-letter code)
-```
-
 ## chart
 
 `youte chart` retrieves the most popular videos in a region, specified by [ISO 3166-1 alpha-2 country codes](https://www.iso.org/obp/ui/#search). If no argument or option is given, it retrieves the most popular videos in the United States.
 
 For example:
 
 ```shell
@@ -360,20 +345,43 @@
 ```
 
 ```{.shell .no-copy}
 Options:
   -o, --output FILENAME  Output text file to store IDs in
 ```
 
+## related-to (deprecated)
+
+*Note.* **From August 7, 2023, this endpoint was deprecated by YouTube. This command is no longer usable.**
+
+`youte related-to` retrieves a list of videos related to a video.
+
+```shell
+youte related-to <video-ids>... -o <file.json>
+```
+
+You can pass one or many video IDs. If multiple video IDs are inputted, youte will iterate through those video IDs, retrieving all related videos to each video separately. The end result contains both the related videos and the id of the video that they are related to.
+
+Other options include:
+
+```{.bash .no-copy}
+  --safe-search [none|moderate|strict]
+                                  Include or exclude restricted content
+                                  [default: none]
+  --region TEXT                   Specify region the videos can be viewed in
+                                  (ISO 3166-1 alpha-2 country code)
+  --lang TEXT                     Return results most relevant to a language
+                                  (ISO 639-1 two-letter code)
+```
+
 ## YouTube API Quota system and youte handling of quota 
 
 Most often, there is a limit to how many requests you can make to YouTube API per day. YouTube Data API uses a quota system, whereby each request costs a number of units depending on the endpoint the request is made to.
 
 For example:  
 
 - search endpoint costs 100 units per request  
 - video, channel, commentThread, and comment endpoints each costs 1 unit per request  
 
 Free accounts get an API quota cap of 10,000 units per project per day, which resets at midnight Pacific Time.
 
 At present, you can only check your quota usage on the [Quotas](https://console.developers.google.com/iam-admin/quotas) page in the API Console. It is not possible to monitor quota usage via metadata returned in the API response. `youte` does not monitor quota usage.
-
```

### Comparing `youte-2.5.0/src/youte.egg-info/SOURCES.txt` & `youte-2.6.0/src/youte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/tests/test_archive.py` & `youte-2.6.0/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `youte-2.5.0/tests/test_cli.py` & `youte-2.6.0/tests/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -292,14 +292,112 @@
     )
     assert os.path.exists(outfile_csv)
     assert _check_csv(outfile_csv)
 
     os.remove(outfile_json)
 
 
+def test_cli_channels_handle(runner, outfile_json, outfile_csv):
+    results = runner.invoke(
+        youte,
+        [
+            "channels",
+            "--handles",
+            "@NextNewsNetwork",
+            "-o",
+            outfile_json,
+            "--key",
+            API_KEY,
+        ],
+    )
+    assert results.exit_code == 0
+
+    with open(outfile_json, "r") as file:
+        r: list[dict] = json.loads(file.read())
+        assert len(r) == 1
+        for i in r:
+            assert i["items"]
+        assert r[0]["_youte"]
+
+    runner.invoke(
+        youte,
+        ["parse", outfile_json, "--output", outfile_csv],
+    )
+    assert os.path.exists(outfile_csv)
+    assert _check_csv(outfile_csv)
+
+    os.remove(outfile_json)
+
+
+def test_cli_channels_handles(runner, outfile_json, outfile_csv):
+    results = runner.invoke(
+        youte,
+        [
+            "channels",
+            "--handles",
+            "@NextNewsNetwork,@TurningPointUSA,@BlazeTV,@msnbc,@CNN,@Vox",
+            "-o",
+            outfile_json,
+            "--key",
+            API_KEY,
+        ],
+    )
+    assert results.exit_code == 0
+
+    with open(outfile_json, "r") as file:
+        r: list[dict] = json.loads(file.read())
+        assert len(r) == 6
+        for i in r:
+            assert i["items"]
+        assert r[0]["_youte"]
+
+    runner.invoke(
+        youte,
+        ["parse", outfile_json, "--output", outfile_csv],
+    )
+    assert os.path.exists(outfile_csv)
+    assert _check_csv(outfile_csv)
+
+    os.remove(outfile_json)
+
+
+def test_cli_channels_both(runner, outfile_json, outfile_csv):
+    results = runner.invoke(
+        youte,
+        [
+            "channels",
+            "-f",
+            Path("tests") / "channel_ids.csv",
+            "--handles",
+            "@NextNewsNetwork,@TurningPointUSA,@BlazeTV,@msnbc,@CNN,@Vox",
+            "-o",
+            outfile_json,
+            "--key",
+            API_KEY,
+        ],
+    )
+    assert results.exit_code == 0
+
+    with open(outfile_json, "r") as file:
+        r: list[dict] = json.loads(file.read())
+        assert len(r) > 6
+        for i in r:
+            assert i["items"]
+        assert r[0]["_youte"]
+
+    runner.invoke(
+        youte,
+        ["parse", outfile_json, "--output", outfile_csv],
+    )
+    assert os.path.exists(outfile_csv)
+    assert _check_csv(outfile_csv)
+
+    os.remove(outfile_json)
+
+
 # TEST comments COMMAND
 
 
 @pytest.fixture()
 def comment_args(outfile_json) -> list:
     return ["comments", "--key", API_KEY, "-o", outfile_json]
```

### Comparing `youte-2.5.0/tests/test_collector.py` & `youte-2.6.0/tests/test_collector.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,22 +32,43 @@
 def test_channel_hydrate_ids(yob):
     ids = ["UC_NN7u1HKTQR6vurmS9iQ1A", "UCMhRG26kBpMp3GAZv5Iv7sw"]
     channels = [ch for ch in yob.get_channel_metadata(ids=ids)]
     assert len(channels)
     assert len(channels[0]["items"]) == 2
 
 
-# def test_channel_hydrate_username(yob):
-#     usernames = ["@brilliantclassics", "@TED"]
-#     channels = [ch
-#                 for ch in
-#                 yob.get_channel_metadata(usernames=usernames)]
-#     print(channels)
-#     assert len(channels)
-#     assert len(channels[0]["items"]) == 2
+def test_channel_hydrate_handles(yob):
+    handles = [
+        "@NextNewsNetwork",
+        "@TurningPointUSA",
+        "@BlazeTV",
+        "@msnbc",
+        "@CNN",
+        "@Vox",
+    ]
+    channels = [ch for ch in yob.get_channel_metadata(handles=handles)]
+    assert len(channels) > 4
+    for el in channels:
+        assert el["items"]
+
+
+def test_channel_hydrate_both(yob):
+    ids = ["UC_NN7u1HKTQR6vurmS9iQ1A", "UCMhRG26kBpMp3GAZv5Iv7sw"]
+    handles = [
+        "@NextNewsNetwork",
+        "@TurningPointUSA",
+        "@BlazeTV",
+        "@msnbc",
+        "@CNN",
+        "@Vox",
+    ]
+    channels = [ch for ch in yob.get_channel_metadata(ids=ids, handles=handles)]
+    assert len(channels) == 7
+    for el in channels:
+        assert el["items"]
 
 
 def test_comments_by_videos(yob):
     vid_ids = ["4MQyV7Wluhs", "6m0qaN2sGDg"]
     channel_ids = ["UC_NN7u1HKTQR6vurmS9iQ1A", "UCMhRG26kBpMp3GAZv5Iv7sw"]
     comments = [cmt for cmt in yob.get_comment_threads(video_ids=vid_ids)]
     assert len(comments) > 2
```

### Comparing `youte-2.5.0/tests/test_parser.py` & `youte-2.6.0/tests/test_parser.py`

 * *Files identical despite different names*

