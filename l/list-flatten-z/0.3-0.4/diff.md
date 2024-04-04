# Comparing `tmp/list_flatten_z-0.3.tar.gz` & `tmp/list_flatten_z-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_flatten_z-0.3.tar", last modified: Thu Apr  4 06:53:55 2024, max compression
+gzip compressed data, was "list_flatten_z-0.4.tar", last modified: Thu Apr  4 07:12:42 2024, max compression
```

## Comparing `list_flatten_z-0.3.tar` & `list_flatten_z-0.4.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 06:53:55.692113 list_flatten_z-0.3/
--rw-rw-rw-   0        0        0      227 2024-04-04 06:53:55.691113 list_flatten_z-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 06:53:55.691113 list_flatten_z-0.3/list_flatten_z.egg-info/
--rw-rw-rw-   0        0        0      227 2024-04-04 06:53:55.000000 list_flatten_z-0.3/list_flatten_z.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2024-04-04 06:53:55.000000 list_flatten_z-0.3/list_flatten_z.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 06:53:55.000000 list_flatten_z-0.3/list_flatten_z.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 06:53:55.000000 list_flatten_z-0.3/list_flatten_z.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 06:53:55.692113 list_flatten_z-0.3/setup.cfg
--rw-rw-rw-   0        0        0      336 2024-04-04 06:50:38.000000 list_flatten_z-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:12:42.066517 list_flatten_z-0.4/
+-rw-rw-rw-   0        0        0      227 2024-04-04 07:12:42.066517 list_flatten_z-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 07:12:42.063517 list_flatten_z-0.4/list_flatten_z/
+-rw-rw-rw-   0        0        0        0 2024-04-04 05:08:17.000000 list_flatten_z-0.4/list_flatten_z/__init__.py
+-rw-rw-rw-   0        0        0      540 2024-04-04 04:42:03.000000 list_flatten_z-0.4/list_flatten_z/list_flatten_z.py
+drwxrwxrwx   0        0        0        0 2024-04-04 07:12:42.065517 list_flatten_z-0.4/list_flatten_z.egg-info/
+-rw-rw-rw-   0        0        0      227 2024-04-04 07:12:42.000000 list_flatten_z-0.4/list_flatten_z.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-04-04 07:12:42.000000 list_flatten_z-0.4/list_flatten_z.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 07:12:42.000000 list_flatten_z-0.4/list_flatten_z.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-04 07:12:42.000000 list_flatten_z-0.4/list_flatten_z.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 07:12:42.066517 list_flatten_z-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      336 2024-04-04 07:11:50.000000 list_flatten_z-0.4/setup.py
```

