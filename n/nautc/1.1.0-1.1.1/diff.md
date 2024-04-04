# Comparing `tmp/nautc-1.1.0.tar.gz` & `tmp/nautc-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautc-1.1.0.tar", last modified: Sat Mar  7 18:52:20 2020, max compression
+gzip compressed data, was "nautc-1.1.1.tar", last modified: Thu Apr  4 03:41:37 2024, max compression
```

## Comparing `nautc-1.1.0.tar` & `nautc-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     3245 2020-03-07 18:29:40.490838 nautc-1.1.0/nautc.py
--rw-r--r--   0        0        0      450 2020-03-07 18:51:46.807376 nautc-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     9884 2020-03-07 18:12:55.107358 nautc-1.1.0/txt.gz
--rw-r--r--   0        0        0      709 2020-03-07 18:52:20.963784 nautc-1.1.0/setup.py
--rw-r--r--   0        0        0      478 2020-03-07 18:52:20.964017 nautc-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    18353 2024-04-04 03:40:38.913356 nautc-1.1.1/README.md
+-rw-r--r--   0        0        0     3198 2024-04-04 03:41:37.074261 nautc-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9884 2020-03-07 18:12:55.000000 nautc-1.1.1/txt.gz
+-rw-r--r--   0        0        0    18669 1970-01-01 00:00:00.000000 nautc-1.1.1/PKG-INFO
```

### Comparing `nautc-1.1.0/txt.gz` & `nautc-1.1.1/txt.gz`

 * *Files identical despite different names*

