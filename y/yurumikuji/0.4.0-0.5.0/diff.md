# Comparing `tmp/yurumikuji-0.4.0.tar.gz` & `tmp/yurumikuji-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yurumikuji-0.4.0.tar", last modified: Thu Apr  4 12:21:06 2024, max compression
+gzip compressed data, was "yurumikuji-0.5.0.tar", last modified: Thu Apr  4 12:27:48 2024, max compression
```

## Comparing `yurumikuji-0.4.0.tar` & `yurumikuji-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/yurumikuji/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/yurumikuji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-04 12:20:56.000000 yurumikuji-0.4.0/yurumikuji/yurumikuji.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:21:06.003512 yurumikuji-0.4.0/yurumikuji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 12:21:05.000000 yurumikuji-0.4.0/yurumikuji.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/yurumikuji/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/yurumikuji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-04-04 12:27:40.000000 yurumikuji-0.5.0/yurumikuji/yurumikuji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:27:48.637964 yurumikuji-0.5.0/yurumikuji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 12:27:48.000000 yurumikuji-0.5.0/yurumikuji.egg-info/top_level.txt
```

### Comparing `yurumikuji-0.4.0/LICENSE` & `yurumikuji-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.4.0/PKG-INFO` & `yurumikuji-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yurumikuji
-Version: 0.4.0
+Version: 0.5.0
 Summary: kamidana(jinja2 cli) slack additonal.
 Home-page: https://github.com/srz-zumix/yurumikuji/
 Author: srz_zumix
 Author-email: zumix.cpp@gmail.com
 License: MIT
 Keywords: Slack,Jinja2
 Platform: any
```

### Comparing `yurumikuji-0.4.0/README.md` & `yurumikuji-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.4.0/setup.py` & `yurumikuji-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,14 @@
         , "Topic :: Utilities"
         , "License :: OSI Approved :: MIT License"
         , "Programming Language :: Python"
         , "Programming Language :: Python :: 3.7"
         , "Programming Language :: Python :: 3.8"
         , "Programming Language :: Python :: 3.9"
     ]
-    , install_requires=['jinja2<3.0', 'markupsafe==2.0.1', 'kamidana', 'slack_sdk', 'python-dotenv']
+    , install_requires=['jinja2>=3.1', 'markupsafe', 'kamidana>=0.10', 'slack_sdk', 'python-dotenv']
     , tests_require=test_deps
     , test_suite="tests.test_suite"
     , extras_require={
         'test': test_deps
     }
 )
```

### Comparing `yurumikuji-0.4.0/yurumikuji/__init__.py` & `yurumikuji-0.5.0/yurumikuji/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = 'srz_zumix'
-__version__ = '0.4.0'
+__version__ = '0.5.0'
 
 __copyright__ = '2021 %s ' % __author__
 __license__ = """
 The MIT License (MIT)
 
 Copyright (c) %s
```

### Comparing `yurumikuji-0.4.0/yurumikuji/yurumikuji.py` & `yurumikuji-0.5.0/yurumikuji/yurumikuji.py`

 * *Files identical despite different names*

### Comparing `yurumikuji-0.4.0/yurumikuji.egg-info/PKG-INFO` & `yurumikuji-0.5.0/yurumikuji.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yurumikuji
-Version: 0.4.0
+Version: 0.5.0
 Summary: kamidana(jinja2 cli) slack additonal.
 Home-page: https://github.com/srz-zumix/yurumikuji/
 Author: srz_zumix
 Author-email: zumix.cpp@gmail.com
 License: MIT
 Keywords: Slack,Jinja2
 Platform: any
```

