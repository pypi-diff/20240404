# Comparing `tmp/frogml-1.0.0rc1.tar.gz` & `tmp/frogml-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogml-1.0.0rc1.tar", last modified: Thu Apr  4 12:35:39 2024, max compression
+gzip compressed data, was "frogml-1.0.0rc2.tar", last modified: Thu Apr  4 14:11:08 2024, max compression
```

## Comparing `frogml-1.0.0rc1.tar` & `frogml-1.0.0rc2.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.952657 frogml-1.0.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/src/frogml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-04 12:35:39.000000 frogml-1.0.0rc1/src/frogml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-04 12:35:39.000000 frogml-1.0.0rc1/src/frogml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:35:39.000000 frogml-1.0.0rc1/src/frogml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 12:35:39.000000 frogml-1.0.0rc1/src/frogml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 12:35:39.000000 frogml-1.0.0rc1/src/frogml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.956657 frogml-1.0.0rc1/src/jfrog_ml/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/_artifactory_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/_log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.956657 frogml-1.0.0rc1/src/jfrog_ml/authentication/
--rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/authentication/_authentication_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/src/jfrog_ml/authentication/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/authentication/models/_auth_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/src/jfrog_ml/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/cli/_frogml_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/cli/_login_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/src/jfrog_ml/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/cli/commands/_login_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/src/jfrog_ml/cli/models/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/cli/models/_cli_login_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/src/jfrog_ml/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/cli/utils/_cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/cli/utils/_login_checks_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/frog_ml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/src/jfrog_ml/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/model_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/src/jfrog_ml/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:35:39.960657 frogml-1.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 12:35:33.000000 frogml-1.0.0rc1/tests/test_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.240143 frogml-1.0.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/frogml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-04-04 14:11:08.000000 frogml-1.0.0rc2/src/frogml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-04 14:11:08.000000 frogml-1.0.0rc2/src/frogml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:11:08.000000 frogml-1.0.0rc2/src/frogml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 14:11:08.000000 frogml-1.0.0rc2/src/frogml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 14:11:08.000000 frogml-1.0.0rc2/src/frogml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 14:11:08.000000 frogml-1.0.0rc2/src/frogml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/jfrog_ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/_artifactory_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/_log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/jfrog_ml/authentication/
+-rw-r--r--   0 runner    (1001) docker     (127)     7554 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/authentication/_authentication_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/jfrog_ml/authentication/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/authentication/models/_auth_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/jfrog_ml/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/cli/_frogml_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7259 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/cli/_login_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/jfrog_ml/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/cli/commands/_login_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/jfrog_ml/cli/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/cli/models/_cli_login_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/jfrog_ml/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/cli/utils/_cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/cli/utils/_login_checks_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/frog_ml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/src/jfrog_ml/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/model_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/src/jfrog_ml/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:11:08.248143 frogml-1.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-04 14:11:01.000000 frogml-1.0.0rc2/tests/test_environment.py
```

### Comparing `frogml-1.0.0rc1/LICENSE` & `frogml-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/PKG-INFO` & `frogml-1.0.0rc2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
 Name: frogml
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: JFrog ML package
 Author: "Shay Bagants"
 Author-email: JFrog <Shayb@jfrog.com>
 Project-URL: Homepage, https://github.com/jfrog/frogml
 Project-URL: Issues, https://github.com/jfrog/frogml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pytest==7.4.3
+Requires-Dist: requests==2.31.0
+Requires-Dist: urllib3==2.1.0
+Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: tensorflow==2.15.0
+Requires-Dist: pydantic==2.5.3
+Requires-Dist: typer==0.9.0
+Requires-Dist: tqdm==4.66.2
 
 # JFrog ML (frogML)
 
 ## Table of contents:
 
 - [Overview](#Overview)
 - [Build](#Build)
```

### Comparing `frogml-1.0.0rc1/README.md` & `frogml-1.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/pyproject.toml` & `frogml-1.0.0rc2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
+dynamic = ["dependencies"]
 name = "frogml"
-version = "1.0.0rc1"
+version = "1.0.0rc2"
 authors = [
     { name = "JFrog", email = "Shayb@jfrog.com" },
 ]
 description = "JFrog ML package"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -17,8 +18,11 @@
 ]
 
 [project.scripts]
 frogml = "jfrog_ml.cli._frogml_cli:main"
 
 [project.urls]
 Homepage = "https://github.com/jfrog/frogml"
-Issues = "https://github.com/jfrog/frogml/issues"
+Issues = "https://github.com/jfrog/frogml/issues"
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
```

### Comparing `frogml-1.0.0rc1/src/frogml.egg-info/PKG-INFO` & `frogml-1.0.0rc2/src/frogml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
 Name: frogml
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: JFrog ML package
 Author: "Shay Bagants"
 Author-email: JFrog <Shayb@jfrog.com>
 Project-URL: Homepage, https://github.com/jfrog/frogml
 Project-URL: Issues, https://github.com/jfrog/frogml/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pytest==7.4.3
+Requires-Dist: requests==2.31.0
+Requires-Dist: urllib3==2.1.0
+Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: tensorflow==2.15.0
+Requires-Dist: pydantic==2.5.3
+Requires-Dist: typer==0.9.0
+Requires-Dist: tqdm==4.66.2
 
 # JFrog ML (frogML)
 
 ## Table of contents:
 
 - [Overview](#Overview)
 - [Build](#Build)
```

### Comparing `frogml-1.0.0rc1/src/frogml.egg-info/SOURCES.txt` & `frogml-1.0.0rc2/src/frogml.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 src/frogml.egg-info/PKG-INFO
 src/frogml.egg-info/SOURCES.txt
 src/frogml.egg-info/dependency_links.txt
 src/frogml.egg-info/entry_points.txt
+src/frogml.egg-info/requires.txt
 src/frogml.egg-info/top_level.txt
 src/jfrog_ml/__init__.py
 src/jfrog_ml/_artifactory_api.py
 src/jfrog_ml/_environment.py
 src/jfrog_ml/_log_config.py
 src/jfrog_ml/_storage_utils.py
 src/jfrog_ml/_utils.py
```

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/_artifactory_api.py` & `frogml-1.0.0rc2/src/jfrog_ml/_artifactory_api.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/_environment.py` & `frogml-1.0.0rc2/src/jfrog_ml/_environment.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/_log_config.py` & `frogml-1.0.0rc2/src/jfrog_ml/_log_config.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/_utils.py` & `frogml-1.0.0rc2/src/jfrog_ml/_utils.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/authentication/_authentication_utils.py` & `frogml-1.0.0rc2/src/jfrog_ml/authentication/_authentication_utils.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/authentication/models/_auth_config.py` & `frogml-1.0.0rc2/src/jfrog_ml/authentication/models/_auth_config.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/cli/_frogml_cli.py` & `frogml-1.0.0rc2/src/jfrog_ml/cli/_frogml_cli.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/cli/_login_cli.py` & `frogml-1.0.0rc2/src/jfrog_ml/cli/_login_cli.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/cli/commands/_login_command.py` & `frogml-1.0.0rc2/src/jfrog_ml/cli/commands/_login_command.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/cli/utils/_cli_utils.py` & `frogml-1.0.0rc2/src/jfrog_ml/cli/utils/_cli_utils.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/cli/utils/_login_checks_utility.py` & `frogml-1.0.0rc2/src/jfrog_ml/cli/utils/_login_checks_utility.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/constants.py` & `frogml-1.0.0rc2/src/jfrog_ml/constants.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/frog_ml.py` & `frogml-1.0.0rc2/src/jfrog_ml/frog_ml.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/http/http_client.py` & `frogml-1.0.0rc2/src/jfrog_ml/http/http_client.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/model_info.py` & `frogml-1.0.0rc2/src/jfrog_ml/model_info.py`

 * *Files identical despite different names*

### Comparing `frogml-1.0.0rc1/src/jfrog_ml/storage.py` & `frogml-1.0.0rc2/src/jfrog_ml/storage.py`

 * *Files identical despite different names*

