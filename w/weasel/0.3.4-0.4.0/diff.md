# Comparing `tmp/weasel-0.3.4.tar.gz` & `tmp/weasel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weasel-0.3.4.tar", last modified: Mon Nov  6 16:07:56 2023, max compression
+gzip compressed data, was "weasel-0.4.0.tar", last modified: Thu Apr  4 09:40:16 2024, max compression
```

## Comparing `weasel-0.3.4.tar` & `weasel-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:56.827650 weasel-0.3.4/
--rw-r--r--   0 vsts      (1001) docker     (127)     1083 2023-11-06 16:07:42.000000 weasel-0.3.4/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     4656 2023-11-06 16:07:56.827650 weasel-0.3.4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3099 2023-11-06 16:07:42.000000 weasel-0.3.4/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      403 2023-11-06 16:07:42.000000 weasel-0.3.4/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1531 2023-11-06 16:07:56.827650 weasel-0.3.4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      136 2023-11-06 16:07:42.000000 weasel-0.3.4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:56.819650 weasel-0.3.4/weasel/
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       59 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       82 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/about.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:56.823650 weasel-0.3.4/weasel/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)      272 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8231 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/assets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5025 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/clone.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5747 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/document.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8452 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/dvc.py
--rw-r--r--   0 vsts      (1001) docker     (127)      793 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2934 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/pull.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2764 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/push.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8118 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/remote_storage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13248 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/cli/run.py
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1171 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/errors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4268 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:56.823650 weasel-0.3.4/weasel/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:56.823650 weasel-0.3.4/weasel/tests/cli/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5673 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/cli/test_cli.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5972 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/cli/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3628 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/cli/test_document.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2156 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/cli/test_remote.py
--rw-r--r--   0 vsts      (1001) docker     (127)      831 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/test_schemas.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5222 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/test_validation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      600 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:56.823650 weasel-0.3.4/weasel/util/
--rw-r--r--   0 vsts      (1001) docker     (127)      841 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2960 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/commands.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5778 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1058 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/environment.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2965 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/filesystem.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2232 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/frozen.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6419 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/git.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1380 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/hashing.py
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/logging.py
--rw-r--r--   0 vsts      (1001) docker     (127)      587 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/modules.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1301 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/remote.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3218 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/validation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2098 2023-11-06 16:07:42.000000 weasel-0.3.4/weasel/util/versions.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2023-11-06 16:07:56.823650 weasel-0.3.4/weasel.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     4656 2023-11-06 16:07:56.000000 weasel-0.3.4/weasel.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1117 2023-11-06 16:07:56.000000 weasel-0.3.4/weasel.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2023-11-06 16:07:56.000000 weasel-0.3.4/weasel.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       42 2023-11-06 16:07:56.000000 weasel-0.3.4/weasel.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      217 2023-11-06 16:07:56.000000 weasel-0.3.4/weasel.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        7 2023-11-06 16:07:56.000000 weasel-0.3.4/weasel.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:16.016612 weasel-0.4.0/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1083 2024-04-04 09:40:05.000000 weasel-0.4.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     4605 2024-04-04 09:40:16.016612 weasel-0.4.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3099 2024-04-04 09:40:05.000000 weasel-0.4.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      403 2024-04-04 09:40:05.000000 weasel-0.4.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1551 2024-04-04 09:40:16.016612 weasel-0.4.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      136 2024-04-04 09:40:05.000000 weasel-0.4.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:16.008612 weasel-0.4.0/weasel/
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       59 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       82 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/about.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:16.012612 weasel-0.4.0/weasel/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)      272 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8231 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/assets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5025 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/clone.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5747 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/document.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8452 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/dvc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      793 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2934 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/pull.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2764 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/push.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8118 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/remote_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13248 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/cli/run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1171 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4268 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:16.012612 weasel-0.4.0/weasel/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:16.012612 weasel-0.4.0/weasel/tests/cli/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6352 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/cli/test_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5972 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/cli/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3628 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/cli/test_document.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2156 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/cli/test_remote.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      831 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/test_schemas.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5222 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/test_validation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      600 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:16.016612 weasel-0.4.0/weasel/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)      841 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2960 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5778 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1058 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2965 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/filesystem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2232 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/frozen.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6535 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/git.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1380 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/hashing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      587 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/modules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1301 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/remote.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3218 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/validation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2098 2024-04-04 09:40:05.000000 weasel-0.4.0/weasel/util/versions.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-04 09:40:16.016612 weasel-0.4.0/weasel.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4605 2024-04-04 09:40:15.000000 weasel-0.4.0/weasel.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1117 2024-04-04 09:40:16.000000 weasel-0.4.0/weasel.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-04 09:40:15.000000 weasel-0.4.0/weasel.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       42 2024-04-04 09:40:15.000000 weasel-0.4.0/weasel.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      216 2024-04-04 09:40:16.000000 weasel-0.4.0/weasel.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        7 2024-04-04 09:40:16.000000 weasel-0.4.0/weasel.egg-info/top_level.txt
```

### Comparing `weasel-0.3.4/LICENSE` & `weasel-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/PKG-INFO` & `weasel-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasel
-Version: 0.3.4
+Version: 0.4.0
 Summary: Weasel: A small and easy workflow system
 Home-page: https://github.com/explosion/weasel/
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/weasel/releases
 Project-URL: Source, https://github.com/explosion/weasel/
@@ -12,32 +12,31 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: confection<0.2.0,>=0.0.4
 Requires-Dist: packaging>=20.0
 Requires-Dist: wasabi<1.2.0,>=0.9.1
 Requires-Dist: srsly<3.0.0,>=2.4.3
 Requires-Dist: typer<0.10.0,>=0.3.0
-Requires-Dist: cloudpathlib<0.17.0,>=0.7.0
-Requires-Dist: smart-open<7.0.0,>=5.2.1
+Requires-Dist: cloudpathlib<1.0.0,>=0.7.0
+Requires-Dist: smart-open<8.0.0,>=5.2.1
 Requires-Dist: requests<3.0.0,>=2.13.0
 Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Weasel: A small and easy workflow system
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: weasel Version: 0.3.4 Summary: Weasel: A small and
+Metadata-Version: 2.1 Name: weasel Version: 0.4.0 Summary: Weasel: A small and
 easy workflow system Home-page: https://github.com/explosion/weasel/ Author:
 Explosion Author-email: contact@explosion.ai License: MIT Project-URL: Release
 notes, https://github.com/explosion/weasel/releases Project-URL: Source, https:
 //github.com/explosion/weasel/ Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Topic :: Scientific/Engineering Requires-Python:
->=3.6 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: confection<0.2.0,>=0.0.4 Requires-Dist: packaging>=20.0 Requires-Dist:
-wasabi<1.2.0,>=0.9.1 Requires-Dist: srsly<3.0.0,>=2.4.3 Requires-Dist:
-typer<0.10.0,>=0.3.0 Requires-Dist: cloudpathlib<0.17.0,>=0.7.0 Requires-Dist:
-smart-open<7.0.0,>=5.2.1 Requires-Dist: requests<3.0.0,>=2.13.0 Requires-Dist:
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
+Engineering Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: confection<0.2.0,>=0.0.4 Requires-Dist:
+packaging>=20.0 Requires-Dist: wasabi<1.2.0,>=0.9.1 Requires-Dist:
+srsly<3.0.0,>=2.4.3 Requires-Dist: typer<0.10.0,>=0.3.0 Requires-Dist:
+cloudpathlib<1.0.0,>=0.7.0 Requires-Dist: smart-open<8.0.0,>=5.2.1 Requires-
+Dist: requests<3.0.0,>=2.13.0 Requires-Dist:
 pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4 _[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/
 _l_o_g_o_._s_v_g_]# Weasel: A small and easy workflow system Weasel lets you manage and
 share **end-to-end workflows** for different **use cases and domains**, and
 orchestrate training, packaging and serving your custom pipelines. You can
 start off by cloning a pre-defined project template, adjust it to fit your
 needs, load in your data, train a pipeline, export it as a Python package,
 upload your outputs to a remote storage and share your results with your team.
```

### Comparing `weasel-0.3.4/README.md` & `weasel-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/setup.cfg` & `weasel-0.4.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weasel
-version = 0.3.4
+version = 0.4.0
 description = Weasel: A small and easy workflow system
 url = https://github.com/explosion/weasel/
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -13,43 +13,46 @@
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 project_urls = 
 	Release notes = https://github.com/explosion/weasel/releases
 	Source = https://github.com/explosion/weasel/
 
 [options]
-python_requires = >=3.6
+python_requires = >=3.7
 install_requires = 
 	confection>=0.0.4,<0.2.0
 	packaging>=20.0
 	wasabi>=0.9.1,<1.2.0
 	srsly>=2.4.3,<3.0.0
 	typer>=0.3.0,<0.10.0
-	cloudpathlib>=0.7.0,<0.17.0
-	smart-open>=5.2.1,<7.0.0
+	cloudpathlib>=0.7.0,<1.0.0
+	smart-open>=5.2.1,<8.0.0
 	requests>=2.13.0,<3.0.0
 	pydantic>=1.7.4,!=1.8,!=1.8.1,<3.0.0
 
 [options.entry_points]
 console_scripts = 
 	weasel = weasel.cli:app
 
+[tool:pytest]
+markers = 
+	issue: references specific issue
+
 [mypy]
 ignore_missing_imports = True
 no_implicit_optional = True
 plugins = pydantic.mypy
 allow_redefinition = True
 
 [egg_info]
```

### Comparing `weasel-0.3.4/weasel/cli/assets.py` & `weasel-0.4.0/weasel/cli/assets.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/cli/clone.py` & `weasel-0.4.0/weasel/cli/clone.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/cli/document.py` & `weasel-0.4.0/weasel/cli/document.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/cli/dvc.py` & `weasel-0.4.0/weasel/cli/dvc.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/cli/main.py` & `weasel-0.4.0/weasel/cli/main.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/cli/pull.py` & `weasel-0.4.0/weasel/cli/pull.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # fmt: off
     remote: str = Arg("default", help="Name or path of remote storage"),
     project_dir: Path = Arg(Path.cwd(), help="Location of project directory. Defaults to current working directory.", exists=True, file_okay=False),
     # fmt: on
 ):
     """Retrieve available precomputed outputs from a remote storage.
     You can alias remotes in your project.yml by mapping them to storage paths.
-    A storage can be anything that the smart-open library can upload to, e.g.
+    A storage can be anything that the smart_open library can upload to, e.g.
     AWS, Google Cloud Storage, SSH, local directories etc.
 
     DOCS: https://github.com/explosion/weasel/tree/main/docs/cli.md#arrow_down-push
     """
     for url, output_path in project_pull(project_dir, remote):
         if url is not None:
             msg.good(f"Pulled {output_path} from {url}")
```

### Comparing `weasel-0.3.4/weasel/cli/push.py` & `weasel-0.4.0/weasel/cli/push.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,29 +12,29 @@
     # fmt: off
     remote: str = Arg("default", help="Name or path of remote storage"),
     project_dir: Path = Arg(Path.cwd(), help="Location of project directory. Defaults to current working directory.", exists=True, file_okay=False),
     # fmt: on
 ):
     """Persist outputs to a remote storage. You can alias remotes in your
     project.yml by mapping them to storage paths. A storage can be anything that
-    the smart-open library can upload to, e.g. AWS, Google Cloud Storage, SSH,
+    the smart_open library can upload to, e.g. AWS, Google Cloud Storage, SSH,
     local directories etc.
 
     DOCS: https://github.com/explosion/weasel/tree/main/docs/cli.md#arrow_up-push
     """
     for output_path, url in project_push(project_dir, remote):
         if url is None:
             msg.info(f"Skipping {output_path}")
         else:
             msg.good(f"Pushed {output_path} to {url}")
 
 
 def project_push(project_dir: Path, remote: str):
     """Persist outputs to a remote storage. You can alias remotes in your project.yml
-    by mapping them to storage paths. A storage can be anything that the smart-open
+    by mapping them to storage paths. A storage can be anything that the smart_open
     library can upload to, e.g. gcs, aws, ssh, local directories etc
     """
     config = load_project_config(project_dir)
     if remote in config.get("remotes", {}):
         remote = config["remotes"][remote]
     storage = RemoteStorage(project_dir, remote)
     for cmd in config.get("commands", []):
```

### Comparing `weasel-0.3.4/weasel/cli/remote_storage.py` & `weasel-0.4.0/weasel/cli/remote_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 if TYPE_CHECKING:
     from cloudpathlib import CloudPath
 
 
 class RemoteStorage:
     """Push and pull outputs to and from a remote file storage.
 
-    Remotes can be anything that `smart-open` can support: AWS, GCS, file system,
+    Remotes can be anything that `smart_open` can support: AWS, GCS, file system,
     ssh, etc.
     """
 
     def __init__(self, project_root: Path, url: str, *, compression="gz"):
         self.root = project_root
         self.url = ensure_pathy(url)
         self.compression = compression
```

### Comparing `weasel-0.3.4/weasel/cli/run.py` & `weasel-0.4.0/weasel/cli/run.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/errors.py` & `weasel-0.4.0/weasel/errors.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/schemas.py` & `weasel-0.4.0/weasel/schemas.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/tests/cli/test_cli.py` & `weasel-0.4.0/weasel/tests/cli/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 
 import pytest
 import srsly
 
 from weasel.cli.remote_storage import RemoteStorage
 from weasel.schemas import ProjectConfigSchema, validate
-from weasel.util import is_subpath_of, load_project_config, make_tempdir
+from weasel.util import git_checkout, is_subpath_of, load_project_config, make_tempdir
 from weasel.util import validate_project_commands
 
 
 def test_issue11235():
     """
     Test that the cli handles interpolation in the directory names correctly when loading project config.
     """
@@ -161,7 +161,32 @@
 def test_local_remote_storage_pull_missing():
     # pulling from a non-existent remote pulls nothing gracefully
     with make_tempdir() as d:
         filename = "a.txt"
         remote = RemoteStorage(d / "root", str(d / "remote"))
         assert remote.pull(filename, command_hash="aaaa") is None
         assert remote.pull(filename) is None
+
+
+def test_project_git_dir_asset():
+    with make_tempdir() as d:
+        # Use a very small repo.
+        git_checkout(
+            "https://github.com/explosion/os-signpost.git",
+            "os_signpost",
+            d / "signpost",
+            branch="v0.0.3",
+        )
+        assert os.path.isdir(d / "signpost")
+
+
+@pytest.mark.issue(66)
+def test_project_git_file_asset():
+    with make_tempdir() as d:
+        # Use a very small repo.
+        git_checkout(
+            "https://github.com/explosion/os-signpost.git",
+            "README.md",
+            d / "readme.md",
+            branch="v0.0.3",
+        )
+        assert os.path.isfile(d / "readme.md")
```

### Comparing `weasel-0.3.4/weasel/tests/cli/test_cli_app.py` & `weasel-0.4.0/weasel/tests/cli/test_cli_app.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/tests/cli/test_document.py` & `weasel-0.4.0/weasel/tests/cli/test_document.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/tests/cli/test_remote.py` & `weasel-0.4.0/weasel/tests/cli/test_remote.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/tests/test_schemas.py` & `weasel-0.4.0/weasel/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/tests/test_validation.py` & `weasel-0.4.0/weasel/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/tests/util.py` & `weasel-0.4.0/weasel/tests/util.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/__init__.py` & `weasel-0.4.0/weasel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/commands.py` & `weasel-0.4.0/weasel/util/commands.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/config.py` & `weasel-0.4.0/weasel/util/config.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/environment.py` & `weasel-0.4.0/weasel/util/environment.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/filesystem.py` & `weasel-0.4.0/weasel/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/frozen.py` & `weasel-0.4.0/weasel/util/frozen.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/git.py` & `weasel-0.4.0/weasel/util/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import shutil
 from pathlib import Path
 from typing import Tuple
 
 from wasabi import msg
 
 from .commands import run_command
@@ -37,15 +38,18 @@
         run_command(cmd, capture=True)
         # We need Path(name) to make sure we also support subdirectories
         try:
             source_path = tmp_dir / Path(subpath)
             if not is_subpath_of(tmp_dir, source_path):
                 err = f"'{subpath}' is a path outside of the cloned repository."
                 msg.fail(err, repo, exits=1)
-            shutil.copytree(str(source_path), str(dest))
+            if os.path.isdir(source_path):
+                shutil.copytree(source_path, dest)
+            else:
+                shutil.copyfile(source_path, dest)
         except FileNotFoundError:
             err = f"Can't clone {subpath}. Make sure the directory exists in the repo (branch '{branch}')"
             msg.fail(err, repo, exits=1)
 
 
 def git_sparse_checkout(repo, subpath, dest, branch):
     # We're using Git, partial clone and sparse checkout to
```

### Comparing `weasel-0.3.4/weasel/util/hashing.py` & `weasel-0.4.0/weasel/util/hashing.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/modules.py` & `weasel-0.4.0/weasel/util/modules.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/remote.py` & `weasel-0.4.0/weasel/util/remote.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/validation.py` & `weasel-0.4.0/weasel/util/validation.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel/util/versions.py` & `weasel-0.4.0/weasel/util/versions.py`

 * *Files identical despite different names*

### Comparing `weasel-0.3.4/weasel.egg-info/PKG-INFO` & `weasel-0.4.0/weasel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasel
-Version: 0.3.4
+Version: 0.4.0
 Summary: Weasel: A small and easy workflow system
 Home-page: https://github.com/explosion/weasel/
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/weasel/releases
 Project-URL: Source, https://github.com/explosion/weasel/
@@ -12,32 +12,31 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: confection<0.2.0,>=0.0.4
 Requires-Dist: packaging>=20.0
 Requires-Dist: wasabi<1.2.0,>=0.9.1
 Requires-Dist: srsly<3.0.0,>=2.4.3
 Requires-Dist: typer<0.10.0,>=0.3.0
-Requires-Dist: cloudpathlib<0.17.0,>=0.7.0
-Requires-Dist: smart-open<7.0.0,>=5.2.1
+Requires-Dist: cloudpathlib<1.0.0,>=0.7.0
+Requires-Dist: smart-open<8.0.0,>=5.2.1
 Requires-Dist: requests<3.0.0,>=2.13.0
 Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Weasel: A small and easy workflow system
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: weasel Version: 0.3.4 Summary: Weasel: A small and
+Metadata-Version: 2.1 Name: weasel Version: 0.4.0 Summary: Weasel: A small and
 easy workflow system Home-page: https://github.com/explosion/weasel/ Author:
 Explosion Author-email: contact@explosion.ai License: MIT Project-URL: Release
 notes, https://github.com/explosion/weasel/releases Project-URL: Source, https:
 //github.com/explosion/weasel/ Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.12 Classifier: Topic :: Scientific/Engineering Requires-Python:
->=3.6 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: confection<0.2.0,>=0.0.4 Requires-Dist: packaging>=20.0 Requires-Dist:
-wasabi<1.2.0,>=0.9.1 Requires-Dist: srsly<3.0.0,>=2.4.3 Requires-Dist:
-typer<0.10.0,>=0.3.0 Requires-Dist: cloudpathlib<0.17.0,>=0.7.0 Requires-Dist:
-smart-open<7.0.0,>=5.2.1 Requires-Dist: requests<3.0.0,>=2.13.0 Requires-Dist:
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
+Engineering Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: confection<0.2.0,>=0.0.4 Requires-Dist:
+packaging>=20.0 Requires-Dist: wasabi<1.2.0,>=0.9.1 Requires-Dist:
+srsly<3.0.0,>=2.4.3 Requires-Dist: typer<0.10.0,>=0.3.0 Requires-Dist:
+cloudpathlib<1.0.0,>=0.7.0 Requires-Dist: smart-open<8.0.0,>=5.2.1 Requires-
+Dist: requests<3.0.0,>=2.13.0 Requires-Dist:
 pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4 _[_h_t_t_p_s_:_/_/_e_x_p_l_o_s_i_o_n_._a_i_/_a_s_s_e_t_s_/_i_m_g_/
 _l_o_g_o_._s_v_g_]# Weasel: A small and easy workflow system Weasel lets you manage and
 share **end-to-end workflows** for different **use cases and domains**, and
 orchestrate training, packaging and serving your custom pipelines. You can
 start off by cloning a pre-defined project template, adjust it to fit your
 needs, load in your data, train a pipeline, export it as a Python package,
 upload your outputs to a remote storage and share your results with your team.
```

### Comparing `weasel-0.3.4/weasel.egg-info/SOURCES.txt` & `weasel-0.4.0/weasel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

