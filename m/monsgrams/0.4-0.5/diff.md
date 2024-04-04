# Comparing `tmp/monsgrams-0.4.tar.gz` & `tmp/monsgrams-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.4.tar", last modified: Thu Apr  4 18:19:02 2024, max compression
+gzip compressed data, was "monsgrams-0.5.tar", last modified: Thu Apr  4 19:03:46 2024, max compression
```

## Comparing `monsgrams-0.4.tar` & `monsgrams-0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:19:02.396426 monsgrams-0.4/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      492 2024-04-04 18:19:02.392426 monsgrams-0.4/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      311 2024-04-04 18:16:29.000000 monsgrams-0.4/README.md
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:19:02.380426 monsgrams-0.4/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       22 2024-04-04 18:09:05.000000 monsgrams-0.4/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     1219 2024-04-04 18:04:40.000000 monsgrams-0.4/monsgrams/main.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:19:02.392426 monsgrams-0.4/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      492 2024-04-04 18:19:01.000000 monsgrams-0.4/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      190 2024-04-04 18:19:02.000000 monsgrams-0.4/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 18:19:01.000000 monsgrams-0.4/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 18:19:01.000000 monsgrams-0.4/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 18:19:02.396426 monsgrams-0.4/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      333 2024-04-04 18:18:48.000000 monsgrams-0.4/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:03:46.488426 monsgrams-0.5/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      627 2024-04-04 19:03:46.484426 monsgrams-0.5/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      446 2024-04-04 19:03:35.000000 monsgrams-0.5/README.md
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:03:46.472426 monsgrams-0.5/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       22 2024-04-04 18:09:05.000000 monsgrams-0.5/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      412 2024-04-04 18:43:28.000000 monsgrams-0.5/monsgrams/api.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     1139 2024-04-04 18:58:08.000000 monsgrams-0.5/monsgrams/main.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 19:03:46.484426 monsgrams-0.5/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      627 2024-04-04 19:03:45.000000 monsgrams-0.5/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      207 2024-04-04 19:03:46.000000 monsgrams-0.5/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 19:03:46.000000 monsgrams-0.5/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 19:03:46.000000 monsgrams-0.5/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 19:03:46.492426 monsgrams-0.5/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      333 2024-04-04 19:02:38.000000 monsgrams-0.5/setup.py
```

