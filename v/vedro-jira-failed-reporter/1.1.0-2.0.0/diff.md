# Comparing `tmp/vedro-jira-failed-reporter-1.1.0.tar.gz` & `tmp/vedro-jira-failed-reporter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-jira-failed-reporter-1.1.0.tar", last modified: Mon Apr  1 03:41:36 2024, max compression
+gzip compressed data, was "vedro-jira-failed-reporter-2.0.0.tar", last modified: Thu Apr  4 15:46:30 2024, max compression
```

## Comparing `vedro-jira-failed-reporter-1.1.0.tar` & `vedro-jira-failed-reporter-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:41:36.834245 vedro-jira-failed-reporter-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-01 03:41:36.834245 vedro-jira-failed-reporter-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-01 03:41:36.834245 vedro-jira-failed-reporter-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:41:36.834245 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/_failed_reporter_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/_jira_stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/_traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/version
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-01 03:41:27.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:41:36.834245 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-01 03:41:36.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-01 03:41:36.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 03:41:36.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-01 03:41:36.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-01 03:41:36.000000 vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_failed_reporter_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_jira_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/version
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-04 15:46:19.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:30.814412 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 15:46:30.000000 vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/top_level.txt
```

### Comparing `vedro-jira-failed-reporter-1.1.0/LICENSE` & `vedro-jira-failed-reporter-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-1.1.0/PKG-INFO` & `vedro-jira-failed-reporter-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-jira-failed-reporter
-Version: 1.1.0
+Version: 2.0.0
 Summary: vedro.io plugin for reporting about flaky tests into jira (with plugin enabled in flaky check runs)
 Home-page: https://github.com/ko10ok/vedro-jira-failed-reporter
 Author: Yuriy Sagitov
 Author-email: pro100.ko10ok@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vedro-jira-failed-reporter-1.1.0/README.md` & `vedro-jira-failed-reporter-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-1.1.0/setup.py` & `vedro-jira-failed-reporter-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/_failed_reporter_plugin.py` & `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_failed_reporter_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 
     jira_server: str = 'https://NOT_SET'
     jira_user: str = 'NOT_SET'
     jira_password: str = 'NOT_SET'
     jira_project: str = 'NOT_SET'
     jira_components: list[str] = []
     jira_labels: list[str] = []
-    jira_flaky_label: str = 'flaky'
+    jira_flaky_label: str = 'auto_flaky'
 
     jira_search_statuses: list[str] = ['Взят в бэклог', 'Open', 'Reopened', 'In Progress']
     jira_search_forbidden_symbols: list[str] = ['[', ']', '"']
     report_project_name: str = 'NOT_SET'
     job_path = '{job_id}'
     job_id: str = 'NOT_SET'
```

### Comparing `vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/_jira_stdout.py` & `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_jira_stdout.py`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/_messages.py` & `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_messages.py`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter/_traceback.py` & `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter/_traceback.py`

 * *Files identical despite different names*

### Comparing `vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter.egg-info/PKG-INFO` & `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vedro-jira-failed-reporter
-Version: 1.1.0
+Version: 2.0.0
 Summary: vedro.io plugin for reporting about flaky tests into jira (with plugin enabled in flaky check runs)
 Home-page: https://github.com/ko10ok/vedro-jira-failed-reporter
 Author: Yuriy Sagitov
 Author-email: pro100.ko10ok@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `vedro-jira-failed-reporter-1.1.0/vedro_jira_failed_reporter.egg-info/SOURCES.txt` & `vedro-jira-failed-reporter-2.0.0/vedro_jira_failed_reporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

