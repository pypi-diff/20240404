# Comparing `tmp/sentry_telegram_with_proxy-0.4.3.tar.gz` & `tmp/sentry_telegram_with_proxy-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_telegram_with_proxy-0.4.3.tar", last modified: Thu Apr  4 14:30:01 2024, max compression
+gzip compressed data, was "sentry_telegram_with_proxy-0.4.4.tar", last modified: Thu Apr  4 14:47:47 2024, max compression
```

## Comparing `sentry_telegram_with_proxy-0.4.3.tar` & `sentry_telegram_with_proxy-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:30:01.915338 sentry_telegram_with_proxy-0.4.3/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1075 2024-04-04 12:24:47.000000 sentry_telegram_with_proxy-0.4.3/LICENSE
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 14:30:01.915114 sentry_telegram_with_proxy-0.4.3/PKG-INFO
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:30:01.913374 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      124 2024-04-04 14:29:23.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy/__init__.py
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     8362 2024-04-04 14:28:45.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy/plugin.py
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:30:01.914900 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/PKG-INFO
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      345 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)        1 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      108 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/entry_points.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       27 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/top_level.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       38 2024-04-04 14:30:01.915397 sentry_telegram_with_proxy-0.4.3/setup.cfg
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1504 2024-04-04 13:08:56.000000 sentry_telegram_with_proxy-0.4.3/setup.py
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:47:47.731008 sentry_telegram_with_proxy-0.4.4/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1075 2024-04-04 12:24:47.000000 sentry_telegram_with_proxy-0.4.4/LICENSE
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 14:47:47.730816 sentry_telegram_with_proxy-0.4.4/PKG-INFO
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:47:47.729529 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      124 2024-04-04 14:47:38.000000 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy/__init__.py
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     8380 2024-04-04 14:47:10.000000 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy/plugin.py
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:47:47.730601 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy.egg-info/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 14:47:47.000000 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      345 2024-04-04 14:47:47.000000 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)        1 2024-04-04 14:47:47.000000 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      108 2024-04-04 14:47:47.000000 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       27 2024-04-04 14:47:47.000000 sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy.egg-info/top_level.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       38 2024-04-04 14:47:47.731057 sentry_telegram_with_proxy-0.4.4/setup.cfg
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1504 2024-04-04 13:08:56.000000 sentry_telegram_with_proxy-0.4.4/setup.py
```

### Comparing `sentry_telegram_with_proxy-0.4.3/LICENSE` & `sentry_telegram_with_proxy-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_telegram_with_proxy-0.4.3/PKG-INFO` & `sentry_telegram_with_proxy-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_telegram_with_proxy
-Version: 0.4.3
+Version: 0.4.4
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/ivantzepner/sentry-telegram
 Author: Ivan Tzepner
 Author-email: ivan.tzepner@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy/plugin.py` & `sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
                 'required': True,
                 'default': '*[Sentry]* {project_name} {tag[level]}: *{title}*\n```{message}```\n{url}'
             },
 
         ]
 
     def safe_urlopen(
+            self,
             url,
             method=None,
             params=None,
             data=None,
             json=None,
             headers=None,
             allow_redirects=False,
```

### Comparing `sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/PKG-INFO` & `sentry_telegram_with_proxy-0.4.4/sentry_telegram_with_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-telegram-with-proxy
-Version: 0.4.3
+Version: 0.4.4
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/ivantzepner/sentry-telegram
 Author: Ivan Tzepner
 Author-email: ivan.tzepner@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `sentry_telegram_with_proxy-0.4.3/setup.py` & `sentry_telegram_with_proxy-0.4.4/setup.py`

 * *Files identical despite different names*

