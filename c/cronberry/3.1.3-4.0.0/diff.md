# Comparing `tmp/cronberry-3.1.3.tar.gz` & `tmp/cronberry-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cronberry-3.1.3.tar", last modified: Thu Feb 15 16:10:34 2024, max compression
+gzip compressed data, was "cronberry-4.0.0.tar", last modified: Thu Apr  4 19:31:58 2024, max compression
```

## Comparing `cronberry-3.1.3.tar` & `cronberry-4.0.0.tar`

### file list

```diff
@@ -1,58 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.654783 cronberry-3.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.646783 cronberry-3.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-15 16:10:19.000000 cronberry-3.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.646783 cronberry-3.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-15 16:10:19.000000 cronberry-3.1.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-02-15 16:10:19.000000 cronberry-3.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-02-15 16:10:19.000000 cronberry-3.1.3/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-15 16:10:19.000000 cronberry-3.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-15 16:10:19.000000 cronberry-3.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-15 16:10:19.000000 cronberry-3.1.3/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.646783 cronberry-3.1.3/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-15 16:10:19.000000 cronberry-3.1.3/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-15 16:10:19.000000 cronberry-3.1.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.646783 cronberry-3.1.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-15 16:10:19.000000 cronberry-3.1.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-15 16:10:19.000000 cronberry-3.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-02-15 16:10:34.654783 cronberry-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-02-15 16:10:19.000000 cronberry-3.1.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-15 16:10:19.000000 cronberry-3.1.3/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-15 16:10:27.000000 cronberry-3.1.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.646783 cronberry-3.1.3/cronberry/
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-02-15 16:10:19.000000 cronberry-3.1.3/cronberry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-02-15 16:10:19.000000 cronberry-3.1.3/cronberry/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-02-15 16:10:19.000000 cronberry-3.1.3/cronberry/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-15 16:10:19.000000 cronberry-3.1.3/cronberry/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.650783 cronberry-3.1.3/cronberry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-02-15 16:10:34.000000 cronberry-3.1.3/cronberry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-15 16:10:34.000000 cronberry-3.1.3/cronberry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 16:10:34.000000 cronberry-3.1.3/cronberry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-15 16:10:34.000000 cronberry-3.1.3/cronberry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-15 16:10:34.000000 cronberry-3.1.3/cronberry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-15 16:10:34.000000 cronberry-3.1.3/cronberry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.650783 cronberry-3.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/api_app.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/api_app.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/api_fields.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-15 16:10:19.000000 cronberry-3.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.650783 cronberry-3.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-15 16:10:19.000000 cronberry-3.1.3/examples/example.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-15 16:10:19.000000 cronberry-3.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-15 16:10:19.000000 cronberry-3.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-15 16:10:19.000000 cronberry-3.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 16:10:34.654783 cronberry-3.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.650783 cronberry-3.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-02-15 16:10:19.000000 cronberry-3.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 16:10:34.650783 cronberry-3.1.3/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-15 16:10:19.000000 cronberry-3.1.3/tests/tables/bad.tab
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-15 16:10:19.000000 cronberry-3.1.3/tests/tables/combined.tab
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-15 16:10:19.000000 cronberry-3.1.3/tests/tables/new.tab
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-15 16:10:19.000000 cronberry-3.1.3/tests/tables/src.tab
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-02-15 16:10:19.000000 cronberry-3.1.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-02-15 16:10:19.000000 cronberry-3.1.3/tests/test_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.707365 cronberry-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.699365 cronberry-4.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-04 19:31:53.000000 cronberry-4.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.699365 cronberry-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-04 19:31:53.000000 cronberry-4.0.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-04 19:31:53.000000 cronberry-4.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-04 19:31:53.000000 cronberry-4.0.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-04 19:31:53.000000 cronberry-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-04 19:31:53.000000 cronberry-4.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 19:31:53.000000 cronberry-4.0.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.699365 cronberry-4.0.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-04 19:31:53.000000 cronberry-4.0.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 19:31:53.000000 cronberry-4.0.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.699365 cronberry-4.0.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 19:31:53.000000 cronberry-4.0.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 19:31:53.000000 cronberry-4.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-04 19:31:58.707365 cronberry-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-04 19:31:53.000000 cronberry-4.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 19:31:55.000000 cronberry-4.0.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 19:31:53.000000 cronberry-4.0.0/VERSION.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.703364 cronberry-4.0.0/cronberry/
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-04-04 19:31:53.000000 cronberry-4.0.0/cronberry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-04 19:31:53.000000 cronberry-4.0.0/cronberry/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-04 19:31:53.000000 cronberry-4.0.0/cronberry/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-04 19:31:53.000000 cronberry-4.0.0/cronberry/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.707365 cronberry-4.0.0/cronberry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-04 19:31:58.000000 cronberry-4.0.0/cronberry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-04 19:31:58.000000 cronberry-4.0.0/cronberry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:31:58.000000 cronberry-4.0.0/cronberry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 19:31:58.000000 cronberry-4.0.0/cronberry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-04 19:31:58.000000 cronberry-4.0.0/cronberry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 19:31:58.000000 cronberry-4.0.0/cronberry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.703364 cronberry-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-04 19:31:53.000000 cronberry-4.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-04 19:31:53.000000 cronberry-4.0.0/docs/api_app.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-04 19:31:53.000000 cronberry-4.0.0/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-04 19:31:53.000000 cronberry-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-04 19:31:53.000000 cronberry-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-04 19:31:53.000000 cronberry-4.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.703364 cronberry-4.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-04 19:31:53.000000 cronberry-4.0.0/examples/example.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-04 19:31:53.000000 cronberry-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-04 19:31:53.000000 cronberry-4.0.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-04 19:31:53.000000 cronberry-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:31:58.707365 cronberry-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.703364 cronberry-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-04 19:31:53.000000 cronberry-4.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:31:58.707365 cronberry-4.0.0/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 19:31:53.000000 cronberry-4.0.0/tests/tables/bad.tab
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-04 19:31:53.000000 cronberry-4.0.0/tests/tables/combined.tab
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-04 19:31:53.000000 cronberry-4.0.0/tests/tables/new.tab
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-04 19:31:53.000000 cronberry-4.0.0/tests/tables/src.tab
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-04 19:31:53.000000 cronberry-4.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-04 19:31:53.000000 cronberry-4.0.0/tests/test_library.py
```

### Comparing `cronberry-3.1.3/.github/workflows/codeql.yml` & `cronberry-4.0.0/.github/workflows/codeql.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 name: "CodeQL Analysis"
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
```

### Comparing `cronberry-3.1.3/.github/workflows/publish.yml` & `cronberry-4.0.0/.github/workflows/publish.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 name: Run publish-specific workflows
 
 on:
   release:
     types: [published]
```

### Comparing `cronberry-3.1.3/.github/workflows/push.yml` & `cronberry-4.0.0/.github/workflows/push.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 name: Run push-specific workflows
 
 on:
   [push, pull_request]
 
 jobs:
```

### Comparing `cronberry-3.1.3/.gitignore` & `cronberry-4.0.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
```

### Comparing `cronberry-3.1.3/.pre-commit-config.yaml` & `cronberry-4.0.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 repos:
   - repo: https://github.com/fsfe/reuse-tool
     rev: v3.0.1
     hooks:
       - id: reuse
         name: Check REUSE compatibility
@@ -13,14 +13,14 @@
       - id: check-yaml
         name: Check YAML
       - id: end-of-file-fixer
         name: Fix end of files
       - id: trailing-whitespace
         name: Trim trailing whitespace
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.0
+    rev: v0.3.5
     hooks:
       - id: ruff
         name: Lint via ruff
         args: [--fix]
       - id: ruff-format
         name: Format via ruff
```

### Comparing `cronberry-3.1.3/Makefile` & `cronberry-4.0.0/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 .PHONY: lint
 lint:
 	pre-commit run ruff --all-files
 
 .PHONY: format
 format:
```

### Comparing `cronberry-3.1.3/PKG-INFO` & `cronberry-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cronberry
-Version: 3.1.3
+Version: 4.0.0
 Summary: Library and CLI for working with multiple cron jobs within a single cron table
 Author-email: Alec Delaney <tekktrik@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/tekktrik/cronberry
 Project-URL: Repository, https://github.com/tekktrik/cronberry
 Project-URL: Documentation, https://cronberry.readthedocs.io/en/latest/
 Keywords: cron,crontab,tools,scheduler
@@ -29,14 +29,18 @@
 Requires-Dist: click~=8.1
 Requires-Dist: typing-extensions~=4.0
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: coverage~=7.4; extra == "dev"
 
+..
+   SPDX-FileCopyrightText: 2024 Alec Delaney
+   SPDX-License-Identifier: GPL-3.0-or-later
+
 cronberry
 ---------
 
 .. image:: https://img.shields.io/pypi/pyversions/cronberry
    :target: https://pypi.org/project/cronberry/
    :alt: PyPI - Python Version
```

### Comparing `cronberry-3.1.3/README.rst` & `cronberry-4.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+..
+   SPDX-FileCopyrightText: 2024 Alec Delaney
+   SPDX-License-Identifier: GPL-3.0-or-later
+
 cronberry
 ---------
 
 .. image:: https://img.shields.io/pypi/pyversions/cronberry
    :target: https://pypi.org/project/cronberry/
    :alt: PyPI - Python Version
```

### Comparing `cronberry-3.1.3/cronberry/__init__.py` & `cronberry-4.0.0/cronberry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Library for working with multiple cron jobs within a single cron table."""
 
 import functools
 import getpass
 import os
 import re
```

### Comparing `cronberry-3.1.3/cronberry/app.py` & `cronberry-4.0.0/cronberry/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """CLI for working with cronberry library."""
 
 from typing import Optional, Tuple
 
 import click
```

### Comparing `cronberry-3.1.3/cronberry/fields.py` & `cronberry-4.0.0/cronberry/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Classes and type annotations for cronjob fields."""
 
 from enum import Enum
 from typing import Any, NamedTuple, Tuple, Union
 
 from typing_extensions import TypeAlias
```

### Comparing `cronberry-3.1.3/cronberry.egg-info/PKG-INFO` & `cronberry-4.0.0/cronberry.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cronberry
-Version: 3.1.3
+Version: 4.0.0
 Summary: Library and CLI for working with multiple cron jobs within a single cron table
 Author-email: Alec Delaney <tekktrik@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/tekktrik/cronberry
 Project-URL: Repository, https://github.com/tekktrik/cronberry
 Project-URL: Documentation, https://cronberry.readthedocs.io/en/latest/
 Keywords: cron,crontab,tools,scheduler
@@ -29,14 +29,18 @@
 Requires-Dist: click~=8.1
 Requires-Dist: typing-extensions~=4.0
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: coverage~=7.4; extra == "dev"
 
+..
+   SPDX-FileCopyrightText: 2024 Alec Delaney
+   SPDX-License-Identifier: GPL-3.0-or-later
+
 cronberry
 ---------
 
 .. image:: https://img.shields.io/pypi/pyversions/cronberry
    :target: https://pypi.org/project/cronberry/
    :alt: PyPI - Python Version
```

### Comparing `cronberry-3.1.3/docs/conf.py` & `cronberry-4.0.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Configuration settings for sphinx."""
 
 import sphinx_rtd_theme
 
 project = "cronberry"
 copyright = "2024 Alec Delaney"
```

### Comparing `cronberry-3.1.3/examples/example.sh` & `cronberry-4.0.0/examples/example.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 #
 # The following examples assume you have the following example
 # crontab file jobs.tab.  Note that due to the way the examples
 # are laid out, they will not run in the order shown below.
 #
 # jobs.tab contents:
 # # [Frequent Job]
```

### Comparing `cronberry-3.1.3/pyproject.toml` & `cronberry-4.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 [build-system]
 requires = [
     "setuptools",
     "setuptools-scm",
     "wheel",
 ]
```

### Comparing `cronberry-3.1.3/tests/conftest.py` & `cronberry-4.0.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Pytest configuration file."""
 
 import pathlib
 import subprocess
 from typing import Union
```

### Comparing `cronberry-3.1.3/tests/tables/combined.tab` & `cronberry-4.0.0/tests/tables/combined.tab`

 * *Files identical despite different names*

### Comparing `cronberry-3.1.3/tests/test_cli.py` & `cronberry-4.0.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for functionality related to cli functionality."""
 
 import os
 import subprocess
 from typing import Tuple
```

### Comparing `cronberry-3.1.3/tests/test_library.py` & `cronberry-4.0.0/tests/test_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2024 Alec Delaney
-# SPDX-License-Identifier: MIT
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 """Tests for functionality related to library functionality."""
 
 import copy
 import os
 import tempfile
 from typing import List
```

