# Comparing `tmp/sentry_telegram_with_proxy-0.4.1.tar.gz` & `tmp/sentry_telegram_with_proxy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_telegram_with_proxy-0.4.1.tar", last modified: Thu Apr  4 13:15:54 2024, max compression
+gzip compressed data, was "sentry_telegram_with_proxy-0.4.2.tar", last modified: Thu Apr  4 13:40:35 2024, max compression
```

## Comparing `sentry_telegram_with_proxy-0.4.1.tar` & `sentry_telegram_with_proxy-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:15:54.436337 sentry_telegram_with_proxy-0.4.1/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1075 2024-04-04 12:24:47.000000 sentry_telegram_with_proxy-0.4.1/LICENSE
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 13:15:54.436140 sentry_telegram_with_proxy-0.4.1/PKG-INFO
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:15:54.434377 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      124 2024-04-04 12:24:47.000000 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy/__init__.py
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     6682 2024-04-04 13:08:56.000000 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy/plugin.py
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:15:54.435932 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy.egg-info/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 13:15:54.000000 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy.egg-info/PKG-INFO
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      345 2024-04-04 13:15:54.000000 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)        1 2024-04-04 13:15:54.000000 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      108 2024-04-04 13:15:54.000000 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy.egg-info/entry_points.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       27 2024-04-04 13:15:54.000000 sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy.egg-info/top_level.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       38 2024-04-04 13:15:54.436389 sentry_telegram_with_proxy-0.4.1/setup.cfg
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1504 2024-04-04 13:08:56.000000 sentry_telegram_with_proxy-0.4.1/setup.py
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:40:35.804579 sentry_telegram_with_proxy-0.4.2/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1075 2024-04-04 12:24:47.000000 sentry_telegram_with_proxy-0.4.2/LICENSE
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 13:40:35.804372 sentry_telegram_with_proxy-0.4.2/PKG-INFO
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:40:35.802562 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      124 2024-04-04 13:40:33.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy/__init__.py
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     6681 2024-04-04 13:38:43.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy/plugin.py
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:40:35.804145 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      345 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)        1 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      108 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       27 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/top_level.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       38 2024-04-04 13:40:35.804636 sentry_telegram_with_proxy-0.4.2/setup.cfg
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1504 2024-04-04 13:08:56.000000 sentry_telegram_with_proxy-0.4.2/setup.py
```

### Comparing `sentry_telegram_with_proxy-0.4.1/LICENSE` & `sentry_telegram_with_proxy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_telegram_with_proxy-0.4.1/PKG-INFO` & `sentry_telegram_with_proxy-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_telegram_with_proxy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/ivantzepner/sentry-telegram
 Author: Ivan Tzepner
 Author-email: ivan.tzepner@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy/plugin.py` & `sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 import logging
 from collections import defaultdict
 
 from django import forms
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from sentry.plugins.bases import notify
 from sentry.http import safe_urlopen
 from sentry.utils.safe import safe_execute
 
 from . import __version__, __doc__ as package_doc
```

### Comparing `sentry_telegram_with_proxy-0.4.1/sentry_telegram_with_proxy.egg-info/PKG-INFO` & `sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-telegram-with-proxy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/ivantzepner/sentry-telegram
 Author: Ivan Tzepner
 Author-email: ivan.tzepner@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `sentry_telegram_with_proxy-0.4.1/setup.py` & `sentry_telegram_with_proxy-0.4.2/setup.py`

 * *Files identical despite different names*

