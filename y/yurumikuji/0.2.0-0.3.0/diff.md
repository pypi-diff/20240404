# Comparing `tmp/yurumikuji-0.2.0.tar.gz` & `tmp/yurumikuji-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yurumikuji-0.2.0.tar", last modified: Sun Apr 25 11:59:47 2021, max compression
+gzip compressed data, was "yurumikuji-0.3.0.tar", last modified: Thu Apr  4 07:11:07 2024, max compression
```

## Comparing `yurumikuji-0.2.0.tar` & `yurumikuji-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)     3106 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2106 2021-04-25 11:59:37.000000 yurumikuji-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1529 2021-04-25 11:59:37.000000 yurumikuji-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/yurumikuji/
--rw-r--r--   0 runner    (1001) docker     (116)     1190 2021-04-25 11:59:37.000000 yurumikuji-0.2.0/yurumikuji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4064 2021-04-25 11:59:37.000000 yurumikuji-0.2.0/yurumikuji/yurumikuji.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/yurumikuji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3106 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/yurumikuji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      235 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/yurumikuji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/yurumikuji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       90 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/yurumikuji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2021-04-25 11:59:47.000000 yurumikuji-0.2.0/yurumikuji.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/yurumikuji/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/yurumikuji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-04 07:10:56.000000 yurumikuji-0.3.0/yurumikuji/yurumikuji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:11:07.322073 yurumikuji-0.3.0/yurumikuji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 07:11:07.000000 yurumikuji-0.3.0/yurumikuji.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `yurumikuji-0.2.0/README.md` & `yurumikuji-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [kamidana][] slack additonal
 
 ## Usage
 
 ```sh
 $ pip install yurumikuji
 $ echo "SLACK_TOKEN=<your token>" > .env
-$ amidana --additionals=yurumikuji.yurumikuji sample/profile.j2
+$ kamidana --additionals=yurumikuji.yurumikuji sample/profile.j2
 https://secure.gravatar.com/avatar/a7614593f3f6f46b73da348c89beba81.jpg?s=512&d=https%3A%2F%2Fa.slack-edge.com%2Fdf10d%2Fimg%2Favatars%2Fava_0023-512.png
 https://secure.gravatar.com/avatar/a7614593f3f6f46b73da348c89beba81.jpg?s=512&d=https%3A%2F%2Fa.slack-edge.com%2Fdf10d%2Fimg%2Favatars%2Fava_0023-512.png
 active
 ```
 
 sample/profile.j2
```

### Comparing `yurumikuji-0.2.0/setup.py` & `yurumikuji-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,14 @@
         , "Topic :: Utilities"
         , "License :: OSI Approved :: MIT License"
         , "Programming Language :: Python"
         , "Programming Language :: Python :: 3.7"
         , "Programming Language :: Python :: 3.8"
         , "Programming Language :: Python :: 3.9"
     ]
-    , install_requires=['kamidana', 'slack_sdk', 'python-dotenv']
+    , install_requires=['jinja2<3.0', 'markupsafe==2.0.1', 'kamidana', 'slack_sdk', 'python-dotenv']
     , tests_require=test_deps
     , test_suite="tests.test_suite"
     , extras_require={
         'test': test_deps
     }
 )
```

### Comparing `yurumikuji-0.2.0/yurumikuji/__init__.py` & `yurumikuji-0.3.0/yurumikuji/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = 'srz_zumix'
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 __copyright__ = '2021 %s ' % __author__
 __license__ = """
 The MIT License (MIT)
 
 Copyright (c) %s
```

