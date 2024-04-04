# Comparing `tmp/gramps-ql-0.0.1rc0.tar.gz` & `tmp/gramps-ql-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramps-ql-0.0.1rc0.tar", last modified: Sun Mar 31 20:52:28 2024, max compression
+gzip compressed data, was "gramps-ql-0.1.tar", last modified: Thu Apr  4 19:40:38 2024, max compression
```

## Comparing `gramps-ql-0.0.1rc0.tar` & `gramps-ql-0.1.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-31 20:52:28.090758 gramps-ql-0.0.1rc0/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-31 20:52:28.086758 gramps-ql-0.0.1rc0/.github/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-31 20:52:28.090758 gramps-ql-0.0.1rc0/.github/workflows/
--rw-rw-r--   0 david     (1000) david     (1000)     1084 2024-01-18 20:48:28.000000 gramps-ql-0.0.1rc0/.github/workflows/python-publish.yml
--rw-rw-r--   0 david     (1000) david     (1000)      151 2024-01-13 20:37:22.000000 gramps-ql-0.0.1rc0/.gitignore
--rw-r--r--   0 david     (1000) david     (1000)      465 2024-03-31 20:52:28.090758 gramps-ql-0.0.1rc0/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)       98 2024-03-31 20:39:50.000000 gramps-ql-0.0.1rc0/README.md
--rw-rw-r--   0 david     (1000) david     (1000)       21 2024-01-13 20:37:22.000000 gramps-ql-0.0.1rc0/mypy.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      717 2024-03-31 20:41:14.000000 gramps-ql-0.0.1rc0/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       38 2024-03-31 20:52:28.090758 gramps-ql-0.0.1rc0/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      102 2024-01-13 20:37:22.000000 gramps-ql-0.0.1rc0/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-31 20:52:28.086758 gramps-ql-0.0.1rc0/src/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-31 20:52:28.090758 gramps-ql-0.0.1rc0/src/gramps_ql/
--rw-rw-r--   0 david     (1000) david     (1000)       69 2024-01-13 20:37:22.000000 gramps-ql-0.0.1rc0/src/gramps_ql/.gitignore
--rw-rw-r--   0 david     (1000) david     (1000)      374 2024-03-31 20:43:18.000000 gramps-ql-0.0.1rc0/src/gramps_ql/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      414 2024-03-31 20:52:27.000000 gramps-ql-0.0.1rc0/src/gramps_ql/_version.py
--rw-rw-r--   0 david     (1000) david     (1000)       27 2024-03-31 20:43:36.000000 gramps-ql-0.0.1rc0/src/gramps_ql/gql.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-31 20:52:28.090758 gramps-ql-0.0.1rc0/src/gramps_ql.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      465 2024-03-31 20:52:28.000000 gramps-ql-0.0.1rc0/src/gramps_ql.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      365 2024-03-31 20:52:28.000000 gramps-ql-0.0.1rc0/src/gramps_ql.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2024-03-31 20:52:28.000000 gramps-ql-0.0.1rc0/src/gramps_ql.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       10 2024-03-31 20:52:28.000000 gramps-ql-0.0.1rc0/src/gramps_ql.egg-info/top_level.txt
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-31 20:52:28.086758 gramps-ql-0.0.1rc0/tests/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-03-31 20:52:28.090758 gramps-ql-0.0.1rc0/tests/gramps_ql/
--rw-rw-r--   0 david     (1000) david     (1000)       72 2024-01-13 20:37:22.000000 gramps-ql-0.0.1rc0/tests/gramps_ql/test_todo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.335069 gramps-ql-0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.331069 gramps-ql-0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.331069 gramps-ql-0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-04 19:40:33.000000 gramps-ql-0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-04 19:40:33.000000 gramps-ql-0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-04 19:40:33.000000 gramps-ql-0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 19:40:33.000000 gramps-ql-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 19:40:38.335069 gramps-ql-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-04 19:40:33.000000 gramps-ql-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 19:40:33.000000 gramps-ql-0.1/mypy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 19:40:33.000000 gramps-ql-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:40:38.335069 gramps-ql-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-04 19:40:33.000000 gramps-ql-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.331069 gramps-ql-0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.335069 gramps-ql-0.1/src/gramps_ql/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 19:40:33.000000 gramps-ql-0.1/src/gramps_ql/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-04 19:40:33.000000 gramps-ql-0.1/src/gramps_ql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-04 19:40:33.000000 gramps-ql-0.1/src/gramps_ql/gql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.335069 gramps-ql-0.1/src/gramps_ql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 19:40:38.000000 gramps-ql-0.1/src/gramps_ql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.331069 gramps-ql-0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:40:38.335069 gramps-ql-0.1/tests/gramps_ql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-04 19:40:33.000000 gramps-ql-0.1/tests/gramps_ql/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 19:40:33.000000 gramps-ql-0.1/tests/gramps_ql/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-04 19:40:33.000000 gramps-ql-0.1/tests/gramps_ql/test_parse.py
```

### Comparing `gramps-ql-0.0.1rc0/.github/workflows/python-publish.yml` & `gramps-ql-0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gramps-ql-0.0.1rc0/pyproject.toml` & `gramps-ql-0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "A Python library to filter Gramps objects by a query syntax"
 authors = [
   { name = "David M. Straub", email = "straub@protonmail.com" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 dynamic = ["version"]
-dependencies = []
+dependencies = ["pyparsing"]
 
 [project.urls]
 homepage = "https://github.com/DavidMStraub/gramps-ql"
 repository = "https://github.com/DavidMStraub/gramps-ql"
 
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
```

