# Comparing `tmp/trufflepig-py-0.1.1.tar.gz` & `tmp/trufflepig-py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trufflepig-py-0.1.1.tar", last modified: Wed Mar 20 20:23:32 2024, max compression
+gzip compressed data, was "trufflepig-py-0.1.3.tar", last modified: Thu Apr  4 00:12:11 2024, max compression
```

## Comparing `trufflepig-py-0.1.1.tar` & `trufflepig-py-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-03-20 20:23:32.592264 trufflepig-py-0.1.1/
--rw-r--r--   0 adamtazi   (501) staff       (20)     1079 2024-02-29 01:34:02.000000 trufflepig-py-0.1.1/LICENSE
--rw-r--r--   0 adamtazi   (501) staff       (20)       93 2024-02-29 00:40:22.000000 trufflepig-py-0.1.1/MANIFEST.in
--rw-r--r--   0 adamtazi   (501) staff       (20)      126 2024-03-20 20:23:32.592073 trufflepig-py-0.1.1/PKG-INFO
--rw-r--r--   0 adamtazi   (501) staff       (20)      762 2024-02-27 19:30:04.000000 trufflepig-py-0.1.1/README.md
--rw-r--r--   0 adamtazi   (501) staff       (20)       38 2024-03-20 20:23:32.592301 trufflepig-py-0.1.1/setup.cfg
--rw-r--r--   0 adamtazi   (501) staff       (20)      215 2024-03-20 20:23:16.000000 trufflepig-py-0.1.1/setup.py
-drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-03-20 20:23:32.590243 trufflepig-py-0.1.1/src/
-drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-03-20 20:23:32.591134 trufflepig-py-0.1.1/src/trufflepig/
--rw-r--r--   0 adamtazi   (501) staff       (20)       56 2024-02-29 01:23:39.000000 trufflepig-py-0.1.1/src/trufflepig/__init__.py
--rw-r--r--   0 adamtazi   (501) staff       (20)       37 2024-02-29 01:23:39.000000 trufflepig-py-0.1.1/src/trufflepig/_constants.py
--rw-r--r--   0 adamtazi   (501) staff       (20)     3451 2024-02-29 01:30:26.000000 trufflepig-py-0.1.1/src/trufflepig/client.py
--rw-r--r--   0 adamtazi   (501) staff       (20)    14478 2024-03-20 20:20:55.000000 trufflepig-py-0.1.1/src/trufflepig/index.py
-drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-03-20 20:23:32.591898 trufflepig-py-0.1.1/src/trufflepig_py.egg-info/
--rw-r--r--   0 adamtazi   (501) staff       (20)      126 2024-03-20 20:23:32.000000 trufflepig-py-0.1.1/src/trufflepig_py.egg-info/PKG-INFO
--rw-r--r--   0 adamtazi   (501) staff       (20)      347 2024-03-20 20:23:32.000000 trufflepig-py-0.1.1/src/trufflepig_py.egg-info/SOURCES.txt
--rw-r--r--   0 adamtazi   (501) staff       (20)        1 2024-03-20 20:23:32.000000 trufflepig-py-0.1.1/src/trufflepig_py.egg-info/dependency_links.txt
--rw-r--r--   0 adamtazi   (501) staff       (20)       17 2024-03-20 20:23:32.000000 trufflepig-py-0.1.1/src/trufflepig_py.egg-info/requires.txt
--rw-r--r--   0 adamtazi   (501) staff       (20)       11 2024-03-20 20:23:32.000000 trufflepig-py-0.1.1/src/trufflepig_py.egg-info/top_level.txt
+drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-04 00:12:11.381488 trufflepig-py-0.1.3/
+-rw-r--r--   0 adamtazi   (501) staff       (20)     1079 2024-02-29 01:34:02.000000 trufflepig-py-0.1.3/LICENSE
+-rw-r--r--   0 adamtazi   (501) staff       (20)       93 2024-02-29 00:40:22.000000 trufflepig-py-0.1.3/MANIFEST.in
+-rw-r--r--   0 adamtazi   (501) staff       (20)      126 2024-04-04 00:12:11.381322 trufflepig-py-0.1.3/PKG-INFO
+-rw-r--r--   0 adamtazi   (501) staff       (20)      762 2024-02-27 19:30:04.000000 trufflepig-py-0.1.3/README.md
+-rw-r--r--   0 adamtazi   (501) staff       (20)       38 2024-04-04 00:12:11.381523 trufflepig-py-0.1.3/setup.cfg
+-rw-r--r--   0 adamtazi   (501) staff       (20)      215 2024-04-04 00:12:06.000000 trufflepig-py-0.1.3/setup.py
+drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-04 00:12:11.379214 trufflepig-py-0.1.3/src/
+drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-04 00:12:11.380260 trufflepig-py-0.1.3/src/trufflepig/
+-rw-r--r--   0 adamtazi   (501) staff       (20)       56 2024-02-29 01:23:39.000000 trufflepig-py-0.1.3/src/trufflepig/__init__.py
+-rw-r--r--   0 adamtazi   (501) staff       (20)       37 2024-04-03 21:03:55.000000 trufflepig-py-0.1.3/src/trufflepig/_constants.py
+-rw-r--r--   0 adamtazi   (501) staff       (20)     3451 2024-02-29 01:30:26.000000 trufflepig-py-0.1.3/src/trufflepig/client.py
+-rw-r--r--   0 adamtazi   (501) staff       (20)    23287 2024-04-04 00:02:22.000000 trufflepig-py-0.1.3/src/trufflepig/index.py
+drwxr-xr-x   0 adamtazi   (501) staff       (20)        0 2024-04-04 00:12:11.381155 trufflepig-py-0.1.3/src/trufflepig_py.egg-info/
+-rw-r--r--   0 adamtazi   (501) staff       (20)      126 2024-04-04 00:12:11.000000 trufflepig-py-0.1.3/src/trufflepig_py.egg-info/PKG-INFO
+-rw-r--r--   0 adamtazi   (501) staff       (20)      347 2024-04-04 00:12:11.000000 trufflepig-py-0.1.3/src/trufflepig_py.egg-info/SOURCES.txt
+-rw-r--r--   0 adamtazi   (501) staff       (20)        1 2024-04-04 00:12:11.000000 trufflepig-py-0.1.3/src/trufflepig_py.egg-info/dependency_links.txt
+-rw-r--r--   0 adamtazi   (501) staff       (20)       17 2024-04-04 00:12:11.000000 trufflepig-py-0.1.3/src/trufflepig_py.egg-info/requires.txt
+-rw-r--r--   0 adamtazi   (501) staff       (20)       11 2024-04-04 00:12:11.000000 trufflepig-py-0.1.3/src/trufflepig_py.egg-info/top_level.txt
```

### Comparing `trufflepig-py-0.1.1/LICENSE` & `trufflepig-py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trufflepig-py-0.1.1/README.md` & `trufflepig-py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `trufflepig-py-0.1.1/src/trufflepig/client.py` & `trufflepig-py-0.1.3/src/trufflepig/client.py`

 * *Files identical despite different names*

