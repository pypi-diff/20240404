# Comparing `tmp/varbose_gram-0.1.tar.gz` & `tmp/varbose_gram-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varbose_gram-0.1.tar", last modified: Thu Apr  4 14:54:07 2024, max compression
+gzip compressed data, was "varbose_gram-0.2.tar", last modified: Thu Apr  4 15:11:38 2024, max compression
```

## Comparing `varbose_gram-0.1.tar` & `varbose_gram-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 14:54:07.736557 varbose_gram-0.1/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      172 2024-04-04 14:54:07.736557 varbose_gram-0.1/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 14:54:07.740557 varbose_gram-0.1/setup.cfg
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      268 2024-04-04 14:53:50.000000 varbose_gram-0.1/setup.py
-drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 14:54:07.728557 varbose_gram-0.1/varbose_gram.egg-info/
--rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      172 2024-04-04 14:54:07.000000 varbose_gram-0.1/varbose_gram.egg-info/PKG-INFO
--rw-------   0 u0_a251  (10251) u0_a251  (10251)      152 2024-04-04 14:54:07.000000 varbose_gram-0.1/varbose_gram.egg-info/SOURCES.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 14:54:07.000000 varbose_gram-0.1/varbose_gram.egg-info/dependency_links.txt
--rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 14:54:07.000000 varbose_gram-0.1/varbose_gram.egg-info/top_level.txt
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 15:11:38.232557 varbose_gram-0.2/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      201 2024-04-04 15:11:38.232557 varbose_gram-0.2/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)       38 2024-04-04 15:11:38.236557 varbose_gram-0.2/setup.cfg
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      297 2024-04-04 15:11:14.000000 varbose_gram-0.2/setup.py
+drwx------   0 u0_a251  (10251) u0_a251  (10251)        0 2024-04-04 15:11:38.228557 varbose_gram-0.2/varbose_gram.egg-info/
+-rw-r--r--   0 u0_a251  (10251) u0_a251  (10251)      201 2024-04-04 15:11:37.000000 varbose_gram-0.2/varbose_gram.egg-info/PKG-INFO
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)      152 2024-04-04 15:11:37.000000 varbose_gram-0.2/varbose_gram.egg-info/SOURCES.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 15:11:37.000000 varbose_gram-0.2/varbose_gram.egg-info/dependency_links.txt
+-rw-------   0 u0_a251  (10251) u0_a251  (10251)        1 2024-04-04 15:11:37.000000 varbose_gram-0.2/varbose_gram.egg-info/top_level.txt
```

