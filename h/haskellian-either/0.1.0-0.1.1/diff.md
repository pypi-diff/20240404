# Comparing `tmp/haskellian-either-0.1.0.tar.gz` & `tmp/haskellian-either-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-either-0.1.0.tar", last modified: Tue Apr  2 06:01:04 2024, max compression
+gzip compressed data, was "haskellian-either-0.1.1.tar", last modified: Thu Apr  4 06:20:54 2024, max compression
```

## Comparing `haskellian-either-0.1.0.tar` & `haskellian-either-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 06:01:04.491958 haskellian-either-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      270 2024-04-02 06:01:04.491958 haskellian-either-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      503 2024-04-02 05:45:18.000000 haskellian-either-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-02 06:01:04.491958 haskellian-either-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 06:01:04.491958 haskellian-either-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 06:01:04.491958 haskellian-either-0.1.0/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 06:01:04.491958 haskellian-either-0.1.0/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      150 2024-04-02 06:00:24.000000 haskellian-either-0.1.0/src/haskellian/either/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1028 2024-04-02 06:00:50.000000 haskellian-either-0.1.0/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      396 2024-04-02 05:44:02.000000 haskellian-either-0.1.0/src/haskellian/either/type.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-02 06:01:04.491958 haskellian-either-0.1.0/src/haskellian_either.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      270 2024-04-02 06:01:04.000000 haskellian-either-0.1.0/src/haskellian_either.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      343 2024-04-02 06:01:04.000000 haskellian-either-0.1.0/src/haskellian_either.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-02 06:01:04.000000 haskellian-either-0.1.0/src/haskellian_either.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-02 06:01:04.000000 haskellian-either-0.1.0/src/haskellian_either.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-02 06:01:04.000000 haskellian-either-0.1.0/src/haskellian_either.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       41 2024-04-02 05:31:14.000000 haskellian-either-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      492 2024-04-04 06:20:50.000000 haskellian-either-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-04-02 10:45:11.000000 haskellian-either-0.1.1/src/haskellian/either/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1911 2024-04-02 17:04:36.000000 haskellian-either-0.1.1/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2257 2024-04-03 05:57:59.000000 haskellian-either-0.1.1/src/haskellian/either/type.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 06:20:54.458645 haskellian-either-0.1.1/src/haskellian_either.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      249 2024-04-04 06:20:54.000000 haskellian-either-0.1.1/src/haskellian_either.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-04-04 06:20:54.000000 haskellian-either-0.1.1/src/haskellian_either.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 06:20:54.000000 haskellian-either-0.1.1/src/haskellian_either.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-04 06:20:54.000000 haskellian-either-0.1.1/src/haskellian_either.egg-info/top_level.txt
```

