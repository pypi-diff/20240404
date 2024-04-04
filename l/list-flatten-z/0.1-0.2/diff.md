# Comparing `tmp/list_flatten_z-0.1.tar.gz` & `tmp/list_flatten_z-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_flatten_z-0.1.tar", last modified: Thu Apr  4 05:22:30 2024, max compression
+gzip compressed data, was "list_flatten_z-0.2.tar", last modified: Thu Apr  4 06:07:17 2024, max compression
```

## Comparing `list_flatten_z-0.1.tar` & `list_flatten_z-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 05:22:30.921077 list_flatten_z-0.1/
--rw-rw-rw-   0        0        0      227 2024-04-04 05:22:30.921077 list_flatten_z-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 05:22:30.920077 list_flatten_z-0.1/list_flatten_z.egg-info/
--rw-rw-rw-   0        0        0      227 2024-04-04 05:22:30.000000 list_flatten_z-0.1/list_flatten_z.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2024-04-04 05:22:30.000000 list_flatten_z-0.1/list_flatten_z.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 05:22:30.000000 list_flatten_z-0.1/list_flatten_z.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 05:22:30.000000 list_flatten_z-0.1/list_flatten_z.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 05:22:30.921077 list_flatten_z-0.1/setup.cfg
--rw-rw-rw-   0        0        0      327 2024-04-04 05:11:14.000000 list_flatten_z-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:07:17.344018 list_flatten_z-0.2/
+-rw-rw-rw-   0        0        0      227 2024-04-04 06:07:17.344018 list_flatten_z-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 06:07:17.344018 list_flatten_z-0.2/list_flatten_z.egg-info/
+-rw-rw-rw-   0        0        0      227 2024-04-04 06:07:17.000000 list_flatten_z-0.2/list_flatten_z.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      160 2024-04-04 06:07:17.000000 list_flatten_z-0.2/list_flatten_z.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 06:07:17.000000 list_flatten_z-0.2/list_flatten_z.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 06:07:17.000000 list_flatten_z-0.2/list_flatten_z.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 06:07:17.345018 list_flatten_z-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      327 2024-04-04 06:05:51.000000 list_flatten_z-0.2/setup.py
```

