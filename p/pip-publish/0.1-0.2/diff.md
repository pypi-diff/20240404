# Comparing `tmp/pip_publish-0.1.tar.gz` & `tmp/pip_publish-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_publish-0.1.tar", last modified: Thu Apr  4 17:44:51 2024, max compression
+gzip compressed data, was "pip_publish-0.2.tar", last modified: Thu Apr  4 17:45:04 2024, max compression
```

## Comparing `pip_publish-0.1.tar` & `pip_publish-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 shukur    (1000) shukur    (1000)        0 2024-04-04 17:44:51.581967 pip_publish-0.1/
--rw-r--r--   0 shukur    (1000) shukur    (1000)       53 2024-04-04 17:44:51.581967 pip_publish-0.1/PKG-INFO
--rw-rw-r--   0 shukur    (1000) shukur    (1000)        0 2024-04-04 17:32:02.000000 pip_publish-0.1/README.md
-drwxrwxr-x   0 shukur    (1000) shukur    (1000)        0 2024-04-04 17:44:51.577967 pip_publish-0.1/pip_publish/
--rw-rw-r--   0 shukur    (1000) shukur    (1000)       23 2024-04-04 17:33:24.000000 pip_publish-0.1/pip_publish/__init__.py
--rw-rw-r--   0 shukur    (1000) shukur    (1000)       39 2024-04-04 17:32:53.000000 pip_publish-0.1/pip_publish/main.py
-drwxrwxr-x   0 shukur    (1000) shukur    (1000)        0 2024-04-04 17:44:51.577967 pip_publish-0.1/pip_publish.egg-info/
--rw-r--r--   0 shukur    (1000) shukur    (1000)       53 2024-04-04 17:44:51.000000 pip_publish-0.1/pip_publish.egg-info/PKG-INFO
--rw-rw-r--   0 shukur    (1000) shukur    (1000)      240 2024-04-04 17:44:51.000000 pip_publish-0.1/pip_publish.egg-info/SOURCES.txt
--rw-rw-r--   0 shukur    (1000) shukur    (1000)        1 2024-04-04 17:44:51.000000 pip_publish-0.1/pip_publish.egg-info/dependency_links.txt
--rw-rw-r--   0 shukur    (1000) shukur    (1000)       49 2024-04-04 17:44:51.000000 pip_publish-0.1/pip_publish.egg-info/entry_points.txt
--rw-rw-r--   0 shukur    (1000) shukur    (1000)       12 2024-04-04 17:44:51.000000 pip_publish-0.1/pip_publish.egg-info/top_level.txt
--rw-rw-r--   0 shukur    (1000) shukur    (1000)       38 2024-04-04 17:44:51.581967 pip_publish-0.1/setup.cfg
--rw-rw-r--   0 shukur    (1000) shukur    (1000)      334 2024-04-04 17:44:22.000000 pip_publish-0.1/setup.py
+drwxrwxr-x   0 shukur    (1000) shukur    (1000)        0 2024-04-04 17:45:04.394097 pip_publish-0.2/
+-rw-r--r--   0 shukur    (1000) shukur    (1000)       53 2024-04-04 17:45:04.394097 pip_publish-0.2/PKG-INFO
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)        0 2024-04-04 17:32:02.000000 pip_publish-0.2/README.md
+drwxrwxr-x   0 shukur    (1000) shukur    (1000)        0 2024-04-04 17:45:04.394097 pip_publish-0.2/pip_publish/
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)       23 2024-04-04 17:33:24.000000 pip_publish-0.2/pip_publish/__init__.py
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)       39 2024-04-04 17:32:53.000000 pip_publish-0.2/pip_publish/main.py
+drwxrwxr-x   0 shukur    (1000) shukur    (1000)        0 2024-04-04 17:45:04.394097 pip_publish-0.2/pip_publish.egg-info/
+-rw-r--r--   0 shukur    (1000) shukur    (1000)       53 2024-04-04 17:45:04.000000 pip_publish-0.2/pip_publish.egg-info/PKG-INFO
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)      240 2024-04-04 17:45:04.000000 pip_publish-0.2/pip_publish.egg-info/SOURCES.txt
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)        1 2024-04-04 17:45:04.000000 pip_publish-0.2/pip_publish.egg-info/dependency_links.txt
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)       49 2024-04-04 17:45:04.000000 pip_publish-0.2/pip_publish.egg-info/entry_points.txt
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)       12 2024-04-04 17:45:04.000000 pip_publish-0.2/pip_publish.egg-info/top_level.txt
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)       38 2024-04-04 17:45:04.394097 pip_publish-0.2/setup.cfg
+-rw-rw-r--   0 shukur    (1000) shukur    (1000)      334 2024-04-04 17:45:01.000000 pip_publish-0.2/setup.py
```

