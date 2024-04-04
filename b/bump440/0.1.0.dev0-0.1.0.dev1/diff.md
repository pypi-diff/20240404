# Comparing `tmp/bump440-0.1.0.dev0.tar.gz` & `tmp/bump440-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bump440-0.1.0.dev0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bump440-0.1.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bump440-0.1.0.dev0.tar` & `bump440-0.1.0.dev1.tar`

### file list

```diff
@@ -1,14 +1,20 @@
--rw-r--r--   0        0        0     3078 2024-04-04 12:53:40.622107 bump440-0.1.0.dev0/.gitignore
--rw-r--r--   0        0        0      916 2024-04-04 13:04:50.014182 bump440-0.1.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    35149 2024-04-04 13:21:26.521425 bump440-0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0     1459 2024-04-04 13:09:39.067040 bump440-0.1.0.dev0/Makefile
--rw-r--r--   0        0        0       10 2024-04-04 13:05:17.075901 bump440-0.1.0.dev0/README.md
--rw-r--r--   0        0        0       40 2024-04-04 13:09:29.364812 bump440-0.1.0.dev0/dev-requirements.in
--rw-r--r--   0        0        0      583 2024-04-04 13:10:36.439306 bump440-0.1.0.dev0/dev-requirements.txt
--rw-r--r--   0        0        0      512 2024-04-04 13:02:11.011707 bump440-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0        6 2024-04-04 13:09:29.364677 bump440-0.1.0.dev0/requirements.in
--rw-r--r--   0        0        0      543 2024-04-04 13:09:56.928354 bump440-0.1.0.dev0/requirements.txt
--rw-r--r--   0        0        0      115 2024-04-04 13:18:16.946730 bump440-0.1.0.dev0/src/bump440/__init__.py
--rw-r--r--   0        0        0      161 2024-04-04 13:12:59.363743 bump440-0.1.0.dev0/src/bump440/main.py
--rw-r--r--   0        0        0       20 2024-04-04 12:57:13.427698 bump440-0.1.0.dev0/tests/__init__.py
--rw-r--r--   0        0        0      458 1970-01-01 00:00:00.000000 bump440-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-04-04 12:53:40.622107 bump440-0.1.0.dev1/.gitignore
+-rw-r--r--   0        0        0      916 2024-04-04 13:04:50.014182 bump440-0.1.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1086 2024-04-04 15:24:51.760493 bump440-0.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0     1753 2024-04-04 15:31:09.575603 bump440-0.1.0.dev1/Makefile
+-rw-r--r--   0        0        0       94 2024-04-04 15:30:31.927495 bump440-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0       40 2024-04-04 13:09:29.364812 bump440-0.1.0.dev1/dev-requirements.in
+-rw-r--r--   0        0        0      583 2024-04-04 13:10:36.439306 bump440-0.1.0.dev1/dev-requirements.txt
+-rw-r--r--   0        0        0      574 2024-04-04 15:30:27.210258 bump440-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0       11 2024-04-04 15:23:34.664751 bump440-0.1.0.dev1/requirements.in
+-rw-r--r--   0        0        0      585 2024-04-04 15:23:34.664806 bump440-0.1.0.dev1/requirements.txt
+-rw-r--r--   0        0        0      215 2024-04-04 15:30:21.394988 bump440-0.1.0.dev1/src/bump440/__init__.py
+-rw-r--r--   0        0        0      578 2024-04-04 14:29:05.748920 bump440-0.1.0.dev1/src/bump440/bump.py
+-rw-r--r--   0        0        0     1057 2024-04-04 15:30:32.295696 bump440-0.1.0.dev1/src/bump440/cli.py
+-rw-r--r--   0        0        0      602 2024-04-04 15:26:04.872856 bump440-0.1.0.dev1/src/bump440/exceptions.py
+-rw-r--r--   0        0        0     1185 2024-04-04 15:22:48.921924 bump440-0.1.0.dev1/src/bump440/io.py
+-rw-r--r--   0        0        0      500 2024-04-04 15:21:31.978624 bump440-0.1.0.dev1/src/bump440/logger.py
+-rw-r--r--   0        0        0      281 2024-04-04 15:21:31.978681 bump440-0.1.0.dev1/src/bump440/parts.py
+-rw-r--r--   0        0        0     2670 2024-04-04 15:21:31.978894 bump440-0.1.0.dev1/src/bump440/versions.py
+-rw-r--r--   0        0        0       20 2024-04-04 12:57:13.427698 bump440-0.1.0.dev1/tests/__init__.py
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 bump440-0.1.0.dev1/PKG-INFO
```

### Comparing `bump440-0.1.0.dev0/.gitignore` & `bump440-0.1.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `bump440-0.1.0.dev0/.pre-commit-config.yaml` & `bump440-0.1.0.dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bump440-0.1.0.dev0/Makefile` & `bump440-0.1.0.dev1/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -44,7 +44,22 @@
 	@python -m piptools compile  --strip-extras dev-requirements.in
 
 # -- Git and Commit --
 ## Run pre-commit
 pre-commit:
 	@echo "Running pre-commit"
 	@pre-commit run --all-files
+
+
+# -- Development --
+## Install Locally for Development
+install:
+	@echo "Uninstalling old version:"
+	@pip uninstall -y bump440
+	@echo "Installing locally for development"
+	@flit install --symlink
+
+
+## Publish the package to PyPi
+publish:
+	@echo "Publishing the package to PyPi"
+	@flit publish
```

### Comparing `bump440-0.1.0.dev0/dev-requirements.txt` & `bump440-0.1.0.dev1/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `bump440-0.1.0.dev0/requirements.txt` & `bump440-0.1.0.dev1/requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     # via markdown-it-py
 pygments==2.17.2
     # via rich
 rich==13.7.1
     # via typer-slim
 shellingham==1.5.4
     # via typer-slim
+toml==0.10.2
+    # via -r requirements.in
 typer==0.12.0
     # via -r requirements.in
 typer-cli==0.12.0
     # via typer
 typer-slim==0.12.0
     # via
     #   typer
```

