# Comparing `tmp/monsgrams-0.2.tar.gz` & `tmp/monsgrams-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.2.tar", last modified: Thu Apr  4 17:11:07 2024, max compression
+gzip compressed data, was "monsgrams-0.3.tar", last modified: Thu Apr  4 18:09:52 2024, max compression
```

## Comparing `monsgrams-0.2.tar` & `monsgrams-0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:11:07.806598 monsgrams-0.2/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      127 2024-04-04 17:11:07.806598 monsgrams-0.2/PKG-INFO
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:11:07.794598 monsgrams-0.2/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       30 2024-04-04 17:10:22.000000 monsgrams-0.2/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      596 2024-04-04 17:06:18.000000 monsgrams-0.2/monsgrams/main.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:11:07.802598 monsgrams-0.2/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      127 2024-04-04 17:11:07.000000 monsgrams-0.2/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      180 2024-04-04 17:11:07.000000 monsgrams-0.2/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 17:11:07.000000 monsgrams-0.2/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 17:11:07.000000 monsgrams-0.2/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 17:11:07.810598 monsgrams-0.2/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      216 2024-04-04 17:10:52.000000 monsgrams-0.2/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:09:52.080426 monsgrams-0.3/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      127 2024-04-04 18:09:52.076426 monsgrams-0.3/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      311 2024-04-04 18:09:27.000000 monsgrams-0.3/README.md
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:09:52.068426 monsgrams-0.3/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       22 2024-04-04 18:09:05.000000 monsgrams-0.3/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     1219 2024-04-04 18:04:40.000000 monsgrams-0.3/monsgrams/main.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:09:52.076426 monsgrams-0.3/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      127 2024-04-04 18:09:51.000000 monsgrams-0.3/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      190 2024-04-04 18:09:51.000000 monsgrams-0.3/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 18:09:51.000000 monsgrams-0.3/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 18:09:51.000000 monsgrams-0.3/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 18:09:52.080426 monsgrams-0.3/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      216 2024-04-04 18:09:44.000000 monsgrams-0.3/setup.py
```

