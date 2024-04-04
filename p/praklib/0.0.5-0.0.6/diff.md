# Comparing `tmp/praklib-0.0.5.tar.gz` & `tmp/praklib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.0.5.tar", last modified: Thu Apr  4 14:31:34 2024, max compression
+gzip compressed data, was "praklib-0.0.6.tar", last modified: Thu Apr  4 14:47:57 2024, max compression
```

## Comparing `praklib-0.0.5.tar` & `praklib-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:31:34.663973 praklib-0.0.5/
--rw-rw-rw-   0        0        0      313 2024-04-04 14:31:34.661778 praklib-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-04 14:31:34.622232 praklib-0.0.5/praklib/
--rw-rw-rw-   0        0        0     2727 2024-04-04 13:29:16.000000 praklib-0.0.5/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.5/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:31:34.659599 praklib-0.0.5/praklib.egg-info/
--rw-rw-rw-   0        0        0      313 2024-04-04 14:31:34.000000 praklib-0.0.5/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-04 14:31:34.000000 praklib-0.0.5/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 14:31:34.000000 praklib-0.0.5/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-04 14:31:34.000000 praklib-0.0.5/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 14:31:34.663973 praklib-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      431 2024-04-04 14:31:00.000000 praklib-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:47:57.602351 praklib-0.0.6/
+-rw-rw-rw-   0        0        0      313 2024-04-04 14:47:57.601345 praklib-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 14:47:57.590722 praklib-0.0.6/praklib/
+-rw-rw-rw-   0        0        0     4221 2024-04-04 14:42:09.000000 praklib-0.0.6/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.0.6/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:47:57.599244 praklib-0.0.6/praklib.egg-info/
+-rw-rw-rw-   0        0        0      313 2024-04-04 14:47:57.000000 praklib-0.0.6/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-04 14:47:57.000000 praklib-0.0.6/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 14:47:57.000000 praklib-0.0.6/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-04 14:47:57.000000 praklib-0.0.6/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 14:47:57.602351 praklib-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      431 2024-04-04 14:47:09.000000 praklib-0.0.6/setup.py
```

