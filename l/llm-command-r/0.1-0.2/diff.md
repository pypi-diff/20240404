# Comparing `tmp/llm-command-r-0.1.tar.gz` & `tmp/llm-command-r-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-command-r-0.1.tar", last modified: Thu Apr  4 14:32:57 2024, max compression
+gzip compressed data, was "llm-command-r-0.2.tar", last modified: Thu Apr  4 16:14:56 2024, max compression
```

## Comparing `llm-command-r-0.1.tar` & `llm-command-r-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:57.952197 llm-command-r-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 14:32:44.000000 llm-command-r-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-04 14:32:57.952197 llm-command-r-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-04 14:32:44.000000 llm-command-r-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:57.952197 llm-command-r-0.1/llm_command_r.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-04 14:32:57.000000 llm-command-r-0.1/llm_command_r.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-04 14:32:57.000000 llm-command-r-0.1/llm_command_r.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:32:57.000000 llm-command-r-0.1/llm_command_r.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 14:32:57.000000 llm-command-r-0.1/llm_command_r.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 14:32:57.000000 llm-command-r-0.1/llm_command_r.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 14:32:57.000000 llm-command-r-0.1/llm_command_r.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-04 14:32:44.000000 llm-command-r-0.1/llm_command_r.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 14:32:44.000000 llm-command-r-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:32:57.952197 llm-command-r-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:32:57.952197 llm-command-r-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 14:32:44.000000 llm-command-r-0.1/tests/test_command_r.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:56.522025 llm-command-r-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 16:14:47.000000 llm-command-r-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-04 16:14:56.522025 llm-command-r-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-04 16:14:47.000000 llm-command-r-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:56.522025 llm-command-r-0.2/llm_command_r.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-04 16:14:56.000000 llm-command-r-0.2/llm_command_r.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-04 16:14:56.000000 llm-command-r-0.2/llm_command_r.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:14:56.000000 llm-command-r-0.2/llm_command_r.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-04 16:14:56.000000 llm-command-r-0.2/llm_command_r.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-04 16:14:56.000000 llm-command-r-0.2/llm_command_r.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 16:14:56.000000 llm-command-r-0.2/llm_command_r.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-04 16:14:47.000000 llm-command-r-0.2/llm_command_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-04 16:14:47.000000 llm-command-r-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:14:56.522025 llm-command-r-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:14:56.522025 llm-command-r-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 16:14:47.000000 llm-command-r-0.2/tests/test_command_r.py
```

### Comparing `llm-command-r-0.1/LICENSE` & `llm-command-r-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-command-r-0.1/pyproject.toml` & `llm-command-r-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm-command-r"
-version = "0.1"
+version = "0.2"
 description = "Access the Cohere Command R family of models"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

