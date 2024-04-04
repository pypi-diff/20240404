# Comparing `tmp/snowflakecli-0.2.0.tar.gz` & `tmp/snowflakecli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflakecli-0.2.0.tar", last modified: Fri Mar 29 16:09:14 2024, max compression
+gzip compressed data, was "snowflakecli-0.3.0.tar", last modified: Thu Apr  4 02:16:13 2024, max compression
```

## Comparing `snowflakecli-0.2.0.tar` & `snowflakecli-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,24 @@
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-03-29 16:09:14.574619 snowflakecli-0.2.0/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      347 2024-03-29 16:09:14.574444 snowflakecli-0.2.0/PKG-INFO
--rw-r--r--   0 jacobthomas   (501) staff       (20)       15 2024-03-29 15:52:39.000000 snowflakecli-0.2.0/README.md
--rw-r--r--   0 jacobthomas   (501) staff       (20)      384 2024-03-29 16:04:54.000000 snowflakecli-0.2.0/pyproject.toml
--rw-r--r--   0 jacobthomas   (501) staff       (20)       38 2024-03-29 16:09:14.574654 snowflakecli-0.2.0/setup.cfg
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-03-29 16:09:14.573294 snowflakecli-0.2.0/src/
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-03-29 16:09:14.573602 snowflakecli-0.2.0/src/snowflakecli/
--rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-03-29 15:52:39.000000 snowflakecli-0.2.0/src/snowflakecli/__init__.py
-drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-03-29 16:09:14.574279 snowflakecli-0.2.0/src/snowflakecli.egg-info/
--rw-r--r--   0 jacobthomas   (501) staff       (20)      347 2024-03-29 16:09:14.000000 snowflakecli-0.2.0/src/snowflakecli.egg-info/PKG-INFO
--rw-r--r--   0 jacobthomas   (501) staff       (20)      252 2024-03-29 16:09:14.000000 snowflakecli-0.2.0/src/snowflakecli.egg-info/SOURCES.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)        1 2024-03-29 16:09:14.000000 snowflakecli-0.2.0/src/snowflakecli.egg-info/dependency_links.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       49 2024-03-29 16:09:14.000000 snowflakecli-0.2.0/src/snowflakecli.egg-info/requires.txt
--rw-r--r--   0 jacobthomas   (501) staff       (20)       13 2024-03-29 16:09:14.000000 snowflakecli-0.2.0/src/snowflakecli.egg-info/top_level.txt
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-04 02:16:13.326636 snowflakecli-0.3.0/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-04 02:16:13.326450 snowflakecli-0.3.0/PKG-INFO
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       15 2024-03-29 15:52:39.000000 snowflakecli-0.3.0/README.md
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      475 2024-04-04 02:15:07.000000 snowflakecli-0.3.0/pyproject.toml
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       38 2024-04-04 02:16:13.326670 snowflakecli-0.3.0/setup.cfg
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-04 02:16:13.324074 snowflakecli-0.3.0/src/
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-04 02:16:13.325172 snowflakecli-0.3.0/src/app/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      250 2024-04-04 02:12:07.000000 snowflakecli-0.3.0/src/app/account.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      155 2024-04-04 01:55:51.000000 snowflakecli-0.3.0/src/app/ask.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      388 2024-04-04 02:03:43.000000 snowflakecli-0.3.0/src/app/database.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      702 2024-04-04 02:12:29.000000 snowflakecli-0.3.0/src/app/main.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:47.000000 snowflakecli-0.3.0/src/app/schema.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      418 2024-04-04 02:11:22.000000 snowflakecli-0.3.0/src/app/scrape.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-04-04 01:45:55.000000 snowflakecli-0.3.0/src/app/table.py
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      404 2024-04-04 01:52:20.000000 snowflakecli-0.3.0/src/app/warehouse.py
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-04 02:16:13.325303 snowflakecli-0.3.0/src/snowflakecli/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        0 2024-03-29 15:52:39.000000 snowflakecli-0.3.0/src/snowflakecli/__init__.py
+drwxr-xr-x   0 jacobthomas   (501) staff       (20)        0 2024-04-04 02:16:13.326254 snowflakecli-0.3.0/src/snowflakecli.egg-info/
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      408 2024-04-04 02:16:13.000000 snowflakecli-0.3.0/src/snowflakecli.egg-info/PKG-INFO
+-rw-r--r--   0 jacobthomas   (501) staff       (20)      439 2024-04-04 02:16:13.000000 snowflakecli-0.3.0/src/snowflakecli.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)        1 2024-04-04 02:16:13.000000 snowflakecli-0.3.0/src/snowflakecli.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       41 2024-04-04 02:16:13.000000 snowflakecli-0.3.0/src/snowflakecli.egg-info/entry_points.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       82 2024-04-04 02:16:13.000000 snowflakecli-0.3.0/src/snowflakecli.egg-info/requires.txt
+-rw-r--r--   0 jacobthomas   (501) staff       (20)       17 2024-04-04 02:16:13.000000 snowflakecli-0.3.0/src/snowflakecli.egg-info/top_level.txt
```
