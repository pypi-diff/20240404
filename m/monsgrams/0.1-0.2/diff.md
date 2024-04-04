# Comparing `tmp/monsgrams-0.1.tar.gz` & `tmp/monsgrams-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsgrams-0.1.tar", last modified: Thu Apr  4 17:06:41 2024, max compression
+gzip compressed data, was "monsgrams-0.2.tar", last modified: Thu Apr  4 17:11:07 2024, max compression
```

## Comparing `monsgrams-0.1.tar` & `monsgrams-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:06:41.974598 monsgrams-0.1/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      146 2024-04-04 17:06:41.970598 monsgrams-0.1/PKG-INFO
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:06:41.962598 monsgrams-0.1/monsgrams/
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:06:12.000000 monsgrams-0.1/monsgrams/__init__.py
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      596 2024-04-04 17:06:18.000000 monsgrams-0.1/monsgrams/main.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:06:41.970598 monsgrams-0.1/monsgrams.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      146 2024-04-04 17:06:41.000000 monsgrams-0.1/monsgrams.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      180 2024-04-04 17:06:41.000000 monsgrams-0.1/monsgrams.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 17:06:41.000000 monsgrams-0.1/monsgrams.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 17:06:41.000000 monsgrams-0.1/monsgrams.egg-info/top_level.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 17:06:41.974598 monsgrams-0.1/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      235 2024-04-04 17:05:40.000000 monsgrams-0.1/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:11:07.806598 monsgrams-0.2/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      127 2024-04-04 17:11:07.806598 monsgrams-0.2/PKG-INFO
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:11:07.794598 monsgrams-0.2/monsgrams/
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       30 2024-04-04 17:10:22.000000 monsgrams-0.2/monsgrams/__init__.py
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      596 2024-04-04 17:06:18.000000 monsgrams-0.2/monsgrams/main.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 17:11:07.802598 monsgrams-0.2/monsgrams.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      127 2024-04-04 17:11:07.000000 monsgrams-0.2/monsgrams.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      180 2024-04-04 17:11:07.000000 monsgrams-0.2/monsgrams.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 17:11:07.000000 monsgrams-0.2/monsgrams.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       10 2024-04-04 17:11:07.000000 monsgrams-0.2/monsgrams.egg-info/top_level.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 17:11:07.810598 monsgrams-0.2/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      216 2024-04-04 17:10:52.000000 monsgrams-0.2/setup.py
```

### Comparing `monsgrams-0.1/monsgrams/main.py` & `monsgrams-0.2/monsgrams/main.py`

 * *Files identical despite different names*

