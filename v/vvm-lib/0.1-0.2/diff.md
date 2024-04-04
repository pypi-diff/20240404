# Comparing `tmp/vvm_lib-0.1.tar.gz` & `tmp/vvm_lib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvm_lib-0.1.tar", last modified: Thu Apr  4 09:46:15 2024, max compression
+gzip compressed data, was "vvm_lib-0.2.tar", last modified: Thu Apr  4 10:14:40 2024, max compression
```

## Comparing `vvm_lib-0.1.tar` & `vvm_lib-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 09:46:15.388902 vvm_lib-0.1/
--rw-rw-rw-   0        0        0      136 2024-04-04 09:46:15.388902 vvm_lib-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-04 09:46:15.395924 vvm_lib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      227 2024-04-04 09:46:10.000000 vvm_lib-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 09:46:15.365913 vvm_lib-0.1/vvm_lib/
--rw-rw-rw-   0        0        0       98 2024-04-04 09:35:03.000000 vvm_lib-0.1/vvm_lib/__init__.py
--rw-rw-rw-   0        0        0     1120 2024-04-03 11:26:36.000000 vvm_lib-0.1/vvm_lib/google_book.py
--rw-rw-rw-   0        0        0     1780 2024-04-03 11:27:48.000000 vvm_lib-0.1/vvm_lib/greenplum.py
--rw-rw-rw-   0        0        0      299 2024-04-03 11:24:43.000000 vvm_lib-0.1/vvm_lib/mssql.py
--rw-rw-rw-   0        0        0      397 2024-04-03 11:25:52.000000 vvm_lib-0.1/vvm_lib/vault.py
-drwxrwxrwx   0        0        0        0 2024-04-04 09:46:15.387931 vvm_lib-0.1/vvm_lib.egg-info/
--rw-rw-rw-   0        0        0      136 2024-04-04 09:46:15.000000 vvm_lib-0.1/vvm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2024-04-04 09:46:15.000000 vvm_lib-0.1/vvm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 09:46:15.000000 vvm_lib-0.1/vvm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-04 09:46:15.000000 vvm_lib-0.1/vvm_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-04-04 09:46:15.000000 vvm_lib-0.1/vvm_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 10:14:40.205942 vvm_lib-0.2/
+-rw-rw-rw-   0        0        0      129 2024-04-04 10:14:40.205942 vvm_lib-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-04 10:14:40.207941 vvm_lib-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      220 2024-04-04 10:14:28.000000 vvm_lib-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:14:40.194395 vvm_lib-0.2/vvm_lib/
+-rw-rw-rw-   0        0        0      229 2024-04-04 10:13:09.000000 vvm_lib-0.2/vvm_lib/__init__.py
+-rw-rw-rw-   0        0        0     1120 2024-04-03 11:26:36.000000 vvm_lib-0.2/vvm_lib/google_book.py
+-rw-rw-rw-   0        0        0     1780 2024-04-03 11:27:48.000000 vvm_lib-0.2/vvm_lib/greenplum.py
+-rw-rw-rw-   0        0        0      299 2024-04-03 11:24:43.000000 vvm_lib-0.2/vvm_lib/mssql.py
+-rw-rw-rw-   0        0        0      397 2024-04-03 11:25:52.000000 vvm_lib-0.2/vvm_lib/vault.py
+drwxrwxrwx   0        0        0        0 2024-04-04 10:14:40.204966 vvm_lib-0.2/vvm_lib.egg-info/
+-rw-rw-rw-   0        0        0      129 2024-04-04 10:14:40.000000 vvm_lib-0.2/vvm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2024-04-04 10:14:40.000000 vvm_lib-0.2/vvm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 10:14:40.000000 vvm_lib-0.2/vvm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-04 09:46:15.000000 vvm_lib-0.2/vvm_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-04-04 10:14:40.000000 vvm_lib-0.2/vvm_lib.egg-info/top_level.txt
```

### Comparing `vvm_lib-0.1/vvm_lib/google_book.py` & `vvm_lib-0.2/vvm_lib/google_book.py`

 * *Files identical despite different names*

### Comparing `vvm_lib-0.1/vvm_lib/greenplum.py` & `vvm_lib-0.2/vvm_lib/greenplum.py`

 * *Files identical despite different names*

