# Comparing `tmp/jobbergate_cli-5.0.0a0.tar.gz` & `tmp/jobbergate_cli-5.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_cli-5.0.0a0.tar", max compression
+gzip compressed data, was "jobbergate_cli-5.0.0a1.tar", max compression
```

## Comparing `jobbergate_cli-5.0.0a0.tar` & `jobbergate_cli-5.0.0a1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1082 2024-03-26 18:59:26.558591 jobbergate_cli-5.0.0a0/LICENSE
--rw-r--r--   0        0        0      980 2024-03-26 18:59:26.558591 jobbergate_cli-5.0.0a0/README.md
--rw-r--r--   0        0        0      709 2024-03-26 18:59:26.558591 jobbergate_cli-5.0.0a0/jobbergate_cli/__init__.py
--rw-r--r--   0        0        0     1111 2024-03-26 18:59:26.558591 jobbergate_cli-5.0.0a0/jobbergate_cli/application_base.py
--rw-r--r--   0        0        0    14152 2024-03-26 18:59:26.558591 jobbergate_cli-5.0.0a0/jobbergate_cli/auth.py
--rw-r--r--   0        0        0     4413 2024-03-26 18:59:26.558591 jobbergate_cli-5.0.0a0/jobbergate_cli/compat.py
--rw-r--r--   0        0        0     4908 2024-03-26 18:59:26.558591 jobbergate_cli-5.0.0a0/jobbergate_cli/config.py
--rw-r--r--   0        0        0     1601 2024-03-26 18:59:26.558591 jobbergate_cli-5.0.0a0/jobbergate_cli/constants.py
--rw-r--r--   0        0        0     3111 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/exceptions.py
--rw-r--r--   0        0        0     1133 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/jobberappslib.py
--rw-r--r--   0        0        0     1095 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/logging.py
--rw-r--r--   0        0        0     6888 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/main.py
--rw-r--r--   0        0        0     9126 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/render.py
--rw-r--r--   0        0        0     9618 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/requests.py
--rw-r--r--   0        0        0     8244 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/schemas.py
--rw-r--r--   0        0        0       66 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/__init__.py
--rw-r--r--   0        0        0       66 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/__init__.py
--rw-r--r--   0        0        0    14749 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/app.py
--rw-r--r--   0        0        0     1725 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/application_base.py
--rw-r--r--   0        0        0     1556 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/application_helpers.py
--rw-r--r--   0        0        0    11114 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/questions.py
--rw-r--r--   0        0        0    21590 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/tools.py
--rw-r--r--   0        0        0       61 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/clusters/__init__.py
--rw-r--r--   0        0        0      728 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/clusters/app.py
--rw-r--r--   0        0        0     3282 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/clusters/tools.py
--rw-r--r--   0        0        0       64 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_scripts/__init__.py
--rw-r--r--   0        0        0    17325 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_scripts/app.py
--rw-r--r--   0        0        0    19016 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_scripts/tools.py
--rw-r--r--   0        0        0       68 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_submissions/__init__.py
--rw-r--r--   0        0        0     7498 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_submissions/app.py
--rw-r--r--   0        0        0    10161 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_submissions/tools.py
--rw-r--r--   0        0        0     3754 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/pagination.py
--rw-r--r--   0        0        0     1474 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/text_tools.py
--rw-r--r--   0        0        0     3810 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/jobbergate_cli/time_loop.py
--rw-r--r--   0        0        0     2904 2024-03-26 18:59:26.562591 jobbergate_cli-5.0.0a0/pyproject.toml
--rw-r--r--   0        0        0     2356 1970-01-01 00:00:00.000000 jobbergate_cli-5.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/LICENSE
+-rw-r--r--   0        0        0      980 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/README.md
+-rw-r--r--   0        0        0      709 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/__init__.py
+-rw-r--r--   0        0        0     1111 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/application_base.py
+-rw-r--r--   0        0        0    14152 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/auth.py
+-rw-r--r--   0        0        0     4413 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/compat.py
+-rw-r--r--   0        0        0     4908 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/config.py
+-rw-r--r--   0        0        0     1601 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/constants.py
+-rw-r--r--   0        0        0     3111 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/exceptions.py
+-rw-r--r--   0        0        0     1133 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/jobberappslib.py
+-rw-r--r--   0        0        0     1095 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/logging.py
+-rw-r--r--   0        0        0     6888 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/main.py
+-rw-r--r--   0        0        0     9126 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/render.py
+-rw-r--r--   0        0        0     9618 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/requests.py
+-rw-r--r--   0        0        0     8244 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/schemas.py
+-rw-r--r--   0        0        0       66 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/__init__.py
+-rw-r--r--   0        0        0    14749 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/app.py
+-rw-r--r--   0        0        0     1725 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/application_base.py
+-rw-r--r--   0        0        0     1556 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/application_helpers.py
+-rw-r--r--   0        0        0    11114 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/questions.py
+-rw-r--r--   0        0        0    21590 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/tools.py
+-rw-r--r--   0        0        0       61 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/clusters/__init__.py
+-rw-r--r--   0        0        0      728 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/clusters/app.py
+-rw-r--r--   0        0        0     3282 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/clusters/tools.py
+-rw-r--r--   0        0        0       64 2024-04-04 21:27:36.027893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    17325 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_scripts/app.py
+-rw-r--r--   0        0        0    19016 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_scripts/tools.py
+-rw-r--r--   0        0        0       68 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_submissions/__init__.py
+-rw-r--r--   0        0        0     7498 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_submissions/app.py
+-rw-r--r--   0        0        0    10161 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_submissions/tools.py
+-rw-r--r--   0        0        0     3754 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/pagination.py
+-rw-r--r--   0        0        0     1474 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/jobbergate_cli/text_tools.py
+-rw-r--r--   0        0        0     3810 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/jobbergate_cli/time_loop.py
+-rw-r--r--   0        0        0     2904 2024-04-04 21:27:36.031893 jobbergate_cli-5.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2356 1970-01-01 00:00:00.000000 jobbergate_cli-5.0.0a1/PKG-INFO
```

### Comparing `jobbergate_cli-5.0.0a0/LICENSE` & `jobbergate_cli-5.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/README.md` & `jobbergate_cli-5.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/__init__.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/application_base.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/auth.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/auth.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/compat.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/compat.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/config.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/constants.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/exceptions.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/jobberappslib.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/jobberappslib.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/logging.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/main.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/render.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/render.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/requests.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/requests.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/schemas.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/app.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/application_base.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/application_base.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/application_helpers.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/application_helpers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/questions.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/questions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/applications/tools.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/applications/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/clusters/app.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/clusters/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/clusters/tools.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/clusters/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_scripts/app.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_scripts/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_scripts/tools.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_scripts/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_submissions/app.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_submissions/app.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/job_submissions/tools.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/job_submissions/tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/subapps/pagination.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/subapps/pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/text_tools.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/text_tools.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/jobbergate_cli/time_loop.py` & `jobbergate_cli-5.0.0a1/jobbergate_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `jobbergate_cli-5.0.0a0/pyproject.toml` & `jobbergate_cli-5.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-cli"
-version = "5.0.0a0"
+version = "5.0.0a1"
 description = "Jobbergate CLI Client"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 packages = [{ include = "jobbergate_cli" }]
 classifiers = [
```

### Comparing `jobbergate_cli-5.0.0a0/PKG-INFO` & `jobbergate_cli-5.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-cli
-Version: 5.0.0a0
+Version: 5.0.0a1
 Summary: Jobbergate CLI Client
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (==6.*)
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: importlib-metadata (>=4.2,<5.0)
 Requires-Dist: inquirer (>=3.1.0,<4.0.0)
-Requires-Dist: jobbergate-core (==5.0.0a0)
+Requires-Dist: jobbergate-core (==5.0.0a1)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: rich (>=11.2.0,<12.0.0)
 Requires-Dist: sentry-sdk (>=1.29.2,<2.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/omnivector-solutions/jobbergate/issues
 Project-URL: Changelog, https://github.com/omnivector-solutions/jobbergate/blob/main/jobbergate-cli/CHANGELOG.rst
```

