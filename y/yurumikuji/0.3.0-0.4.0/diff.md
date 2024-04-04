# Comparing `tmp/yurumikuji-0.3.0.tar.gz` & `tmp/yurumikuji-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yurumikuji-0.3.0.tar", last modified: Thu Apr  4 07:11:07 2024, max compression
+gzip compressed data, was "yurumikuji-0.4.0.tar", last modified: Thu Apr  4 12:21:06 2024, max compression
```

## Comparing `yurumikuji-0.3.0.tar` & `yurumikuji-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/yurumikuji/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/yurumikuji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/yurumikuji/yurumikuji.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/yurumikuji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/yurumikuji/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/yurumikuji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/yurumikuji/yurumikuji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/yurumikuji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/top_level.txt
```

### Comparing `yurumikuji-0.3.0/LICENSE` & `yurumikuji-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.3.0/PKG-INFO` & `yurumikuji-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yurumikuji
-Version: 0.3.0
+Version: 0.4.0
 Summary: kamidana(jinja2 cli) slack additonal.
 Home-page: https://github.com/srz-zumix/yurumikuji/
 Author: srz_zumix
 Author-email: zumix.cpp@gmail.com
 License: MIT
 Keywords: Slack,Jinja2
 Platform: any
```

### Comparing `yurumikuji-0.3.0/README.md` & `yurumikuji-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.3.0/setup.py` & `yurumikuji-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.3.0/yurumikuji/__init__.py` & `yurumikuji-0.4.0/yurumikuji/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = 'srz_zumix'
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 __copyright__ = '2021 %s ' % __author__
 __license__ = """
 The MIT License (MIT)
 
 Copyright (c) %s
```

### Comparing `yurumikuji-0.3.0/yurumikuji/yurumikuji.py` & `yurumikuji-0.4.0/yurumikuji/yurumikuji.py`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.3.0/yurumikuji.egg-info/PKG-INFO` & `yurumikuji-0.4.0/yurumikuji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yurumikuji
-Version: 0.3.0
+Version: 0.4.0
 Summary: kamidana(jinja2 cli) slack additonal.
 Home-page: https://github.com/srz-zumix/yurumikuji/
 Author: srz_zumix
 Author-email: zumix.cpp@gmail.com
 License: MIT
 Keywords: Slack,Jinja2
 Platform: any
```

