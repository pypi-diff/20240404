# Comparing `tmp/monsgrams-0.3.tar.gz` & `tmp/monsgrams-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.3.tar", last modified: Thu Apr  4 18:09:52 2024, max compression
+gzip compressed data, was "monsgrams-0.3.1.tar", last modified: Thu Apr  4 18:11:14 2024, max compression
```

## Comparing `monsgrams-0.3.tar` & `monsgrams-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:09:52.080426 monsgrams-0.3/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      127 2024-04-04 18:09:52.076426 monsgrams-0.3/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      311 2024-04-04 18:09:27.000000 monsgrams-0.3/README.md
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:09:52.068426 monsgrams-0.3/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       22 2024-04-04 18:09:05.000000 monsgrams-0.3/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)     1219 2024-04-04 18:04:40.000000 monsgrams-0.3/monsgrams/main.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:09:52.076426 monsgrams-0.3/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      127 2024-04-04 18:09:51.000000 monsgrams-0.3/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      190 2024-04-04 18:09:51.000000 monsgrams-0.3/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 18:09:51.000000 monsgrams-0.3/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 18:09:51.000000 monsgrams-0.3/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 18:09:52.080426 monsgrams-0.3/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      216 2024-04-04 18:09:44.000000 monsgrams-0.3/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:11:14.844426 monsgrams-0.3.1/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      129 2024-04-04 18:11:14.840426 monsgrams-0.3.1/PKG-INFO
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:11:14.820426 monsgrams-0.3.1/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       22 2024-04-04 18:09:05.000000 monsgrams-0.3.1/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)     1219 2024-04-04 18:04:40.000000 monsgrams-0.3.1/monsgrams/main.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 18:11:14.836426 monsgrams-0.3.1/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      129 2024-04-04 18:11:14.000000 monsgrams-0.3.1/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      180 2024-04-04 18:11:14.000000 monsgrams-0.3.1/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 18:11:14.000000 monsgrams-0.3.1/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 18:11:14.000000 monsgrams-0.3.1/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 18:11:14.844426 monsgrams-0.3.1/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      218 2024-04-04 18:11:02.000000 monsgrams-0.3.1/setup.py
```

### Comparing `monsgrams-0.3/monsgrams/main.py` & `monsgrams-0.3.1/monsgrams/main.py`

 * *Files identical despite different names*

