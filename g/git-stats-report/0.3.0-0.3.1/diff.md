# Comparing `tmp/git-stats-report-0.3.0.tar.gz` & `tmp/git-stats-report-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-stats-report-0.3.0.tar", last modified: Thu Apr  4 04:35:15 2024, max compression
+gzip compressed data, was "git-stats-report-0.3.1.tar", last modified: Thu Apr  4 05:22:59 2024, max compression
```

## Comparing `git-stats-report-0.3.0.tar` & `git-stats-report-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:35:15.074833 git-stats-report-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-04 04:35:15.074833 git-stats-report-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:35:15.070833 git-stats-report-0.3.0/git_stats_report/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/git_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:35:15.074833 git-stats-report-0.3.0/git_stats_report/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/strategy/from_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/strategy/from_latest_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/strategy/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/git_stats_report/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:35:15.074833 git-stats-report-0.3.0/git_stats_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-04 04:35:15.000000 git-stats-report-0.3.0/git_stats_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 04:35:15.000000 git-stats-report-0.3.0/git_stats_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:35:15.000000 git-stats-report-0.3.0/git_stats_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 04:35:15.000000 git-stats-report-0.3.0/git_stats_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 04:35:15.000000 git-stats-report-0.3.0/git_stats_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 04:35:15.000000 git-stats-report-0.3.0/git_stats_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-04 04:35:04.000000 git-stats-report-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:35:15.074833 git-stats-report-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:59.126883 git-stats-report-0.3.1/git_stats_report/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/git_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/git_stats_report/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/strategy/from_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/strategy/from_latest_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/strategy/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/git_stats_report/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/git_stats_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 05:22:59.000000 git-stats-report-0.3.1/git_stats_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-04 05:22:48.000000 git-stats-report-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 05:22:59.130883 git-stats-report-0.3.1/setup.cfg
```

### Comparing `git-stats-report-0.3.0/LICENSE` & `git-stats-report-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/PKG-INFO` & `git-stats-report-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.3.0
+Version: 0.3.1
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `git-stats-report-0.3.0/Pipfile` & `git-stats-report-0.3.1/Pipfile`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/README.md` & `git-stats-report-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/git_stats_report/__main__.py` & `git-stats-report-0.3.1/git_stats_report/__main__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/git_stats_report/entrypoint.py` & `git-stats-report-0.3.1/git_stats_report/entrypoint.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/git_stats_report/git_stats.py` & `git-stats-report-0.3.1/git_stats_report/git_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,16 @@
 
 def get_reports(
     git_stats: GitStatsRawOutput, since: datetime, total_commits: int
 ) -> list[AuthorReport]:
     reports: list[AuthorReport] = []
 
     for author in git_stats["authors"]:
+        if not author["value"]:
+            continue
         author_report = get_author_info(author, since, total_commits)
         reports.append(author_report)
     return reports
 
 
 def format_author_name(author: str) -> str:
     name_as_list = author.split(".")
```

### Comparing `git-stats-report-0.3.0/git_stats_report/strategy/__init__.py` & `git-stats-report-0.3.1/git_stats_report/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/git_stats_report/strategy/from_latest_tag.py` & `git-stats-report-0.3.1/git_stats_report/strategy/from_latest_tag.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/git_stats_report/utils.py` & `git-stats-report-0.3.1/git_stats_report/utils.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/git_stats_report.egg-info/PKG-INFO` & `git-stats-report-0.3.1/git_stats_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.3.0
+Version: 0.3.1
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `git-stats-report-0.3.0/git_stats_report.egg-info/SOURCES.txt` & `git-stats-report-0.3.1/git_stats_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.3.0/pyproject.toml` & `git-stats-report-0.3.1/pyproject.toml`

 * *Files identical despite different names*

