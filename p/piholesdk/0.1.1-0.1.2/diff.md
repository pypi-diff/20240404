# Comparing `tmp/piholesdk-0.1.1.tar.gz` & `tmp/piholesdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piholesdk-0.1.1.tar", last modified: Thu Apr  4 18:32:39 2024, max compression
+gzip compressed data, was "piholesdk-0.1.2.tar", last modified: Thu Apr  4 19:29:33 2024, max compression
```

## Comparing `piholesdk-0.1.1.tar` & `piholesdk-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:39.708562 piholesdk-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 18:32:39.708562 piholesdk-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 18:32:35.000000 piholesdk-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:39.708562 piholesdk-0.1.1/piholesdk/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 18:32:35.000000 piholesdk-0.1.1/piholesdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 18:32:35.000000 piholesdk-0.1.1/piholesdk/piholesdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:39.708562 piholesdk-0.1.1/piholesdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 18:32:39.000000 piholesdk-0.1.1/piholesdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:32:39.708562 piholesdk-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-04 18:32:35.000000 piholesdk-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:39.708562 piholesdk-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:35.000000 piholesdk-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:35.000000 piholesdk-0.1.1/tests/test_piholesdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:29:33.971101 piholesdk-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-04 19:29:33.971101 piholesdk-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-04 19:29:27.000000 piholesdk-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:29:33.967101 piholesdk-0.1.2/piholesdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 19:29:27.000000 piholesdk-0.1.2/piholesdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-04 19:29:27.000000 piholesdk-0.1.2/piholesdk/piholesdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:29:33.971101 piholesdk-0.1.2/piholesdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-04-04 19:29:33.000000 piholesdk-0.1.2/piholesdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 19:29:33.000000 piholesdk-0.1.2/piholesdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:29:33.000000 piholesdk-0.1.2/piholesdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 19:29:33.000000 piholesdk-0.1.2/piholesdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 19:29:33.000000 piholesdk-0.1.2/piholesdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:29:33.971101 piholesdk-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-04 19:29:27.000000 piholesdk-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:29:33.971101 piholesdk-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:29:27.000000 piholesdk-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:29:27.000000 piholesdk-0.1.2/tests/test_piholesdk.py
```

### Comparing `piholesdk-0.1.1/piholesdk/piholesdk.py` & `piholesdk-0.1.2/piholesdk/piholesdk.py`

 * *Files identical despite different names*

