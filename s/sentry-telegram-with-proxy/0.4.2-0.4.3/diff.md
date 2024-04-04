# Comparing `tmp/sentry_telegram_with_proxy-0.4.2.tar.gz` & `tmp/sentry_telegram_with_proxy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_telegram_with_proxy-0.4.2.tar", last modified: Thu Apr  4 13:40:35 2024, max compression
+gzip compressed data, was "sentry_telegram_with_proxy-0.4.3.tar", last modified: Thu Apr  4 14:30:01 2024, max compression
```

## Comparing `sentry_telegram_with_proxy-0.4.2.tar` & `sentry_telegram_with_proxy-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:40:35.804579 sentry_telegram_with_proxy-0.4.2/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1075 2024-04-04 12:24:47.000000 sentry_telegram_with_proxy-0.4.2/LICENSE
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 13:40:35.804372 sentry_telegram_with_proxy-0.4.2/PKG-INFO
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:40:35.802562 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      124 2024-04-04 13:40:33.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy/__init__.py
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     6681 2024-04-04 13:38:43.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy/plugin.py
-drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 13:40:35.804145 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/PKG-INFO
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      345 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)        1 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      108 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/entry_points.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       27 2024-04-04 13:40:35.000000 sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/top_level.txt
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       38 2024-04-04 13:40:35.804636 sentry_telegram_with_proxy-0.4.2/setup.cfg
--rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1504 2024-04-04 13:08:56.000000 sentry_telegram_with_proxy-0.4.2/setup.py
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:30:01.915338 sentry_telegram_with_proxy-0.4.3/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1075 2024-04-04 12:24:47.000000 sentry_telegram_with_proxy-0.4.3/LICENSE
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 14:30:01.915114 sentry_telegram_with_proxy-0.4.3/PKG-INFO
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:30:01.913374 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      124 2024-04-04 14:29:23.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy/__init__.py
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     8362 2024-04-04 14:28:45.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy/plugin.py
+drwxr-xr-x   0 andrey.rostovcev   (501) staff       (20)        0 2024-04-04 14:30:01.914900 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1105 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      345 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)        1 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)      108 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       27 2024-04-04 14:30:01.000000 sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/top_level.txt
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)       38 2024-04-04 14:30:01.915397 sentry_telegram_with_proxy-0.4.3/setup.cfg
+-rw-r--r--   0 andrey.rostovcev   (501) staff       (20)     1504 2024-04-04 13:08:56.000000 sentry_telegram_with_proxy-0.4.3/setup.py
```

### Comparing `sentry_telegram_with_proxy-0.4.2/LICENSE` & `sentry_telegram_with_proxy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_telegram_with_proxy-0.4.2/PKG-INFO` & `sentry_telegram_with_proxy-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_telegram_with_proxy
-Version: 0.4.2
+Version: 0.4.3
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/ivantzepner/sentry-telegram
 Author: Ivan Tzepner
 Author-email: ivan.tzepner@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy/plugin.py` & `sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # coding: utf-8
 import logging
+import warnings
 from collections import defaultdict
 
 from django import forms
 from django.utils.translation import gettext_lazy as _
 
+from sentry.net.http import SafeSession
 from sentry.plugins.bases import notify
-from sentry.http import safe_urlopen
 from sentry.utils.safe import safe_execute
 
 from . import __version__, __doc__ as package_doc
 
 
 class TelegramNotificationsOptionsForm(notify.NotificationConfigurationForm):
     api_origin = forms.CharField(
@@ -109,14 +110,71 @@
                 'validators': [],
                 'required': True,
                 'default': '*[Sentry]* {project_name} {tag[level]}: *{title}*\n```{message}```\n{url}'
             },
 
         ]
 
+    def safe_urlopen(
+            url,
+            method=None,
+            params=None,
+            data=None,
+            json=None,
+            headers=None,
+            allow_redirects=False,
+            timeout=30,
+            verify_ssl=True,
+            user_agent=None,
+            stream=False,
+            proxies=None,
+    ):
+        """
+        A slightly safer version of ``urlib2.urlopen`` which prevents redirection
+        and ensures the URL isn't attempting to hit a blacklisted IP range.
+        """
+        if user_agent is not None:
+            warnings.warn("user_agent is no longer used with safe_urlopen")
+
+        with SafeSession() as session:
+            kwargs = {}
+
+            if json:
+                kwargs["json"] = json
+                if not headers:
+                    headers = {}
+                headers.setdefault("Content-Type", "application/json")
+
+            if data:
+                kwargs["data"] = data
+
+            if params:
+                kwargs["params"] = params
+
+            if headers:
+                kwargs["headers"] = headers
+
+            if method is None:
+                method = "POST" if (data or json) else "GET"
+
+            if proxies:
+                kwargs["proxies"] = proxies
+
+            response = session.request(
+                method=method,
+                url=url,
+                allow_redirects=allow_redirects,
+                timeout=timeout,
+                verify=verify_ssl,
+                stream=stream,
+                **kwargs,
+            )
+
+            return response
+
     def build_message(self, group, event):
         the_tags = defaultdict(lambda: '[NA]')
         the_tags.update({k:v for k, v in event.tags})
         names = {
             'title': event.title,
             'tag': the_tags,
             'message': event.message,
@@ -147,15 +205,15 @@
         if not receivers:
             return []
         return list([line.strip() for line in receivers.strip().splitlines() if line.strip()])
 
     def send_message(self, url, payload, receiver, proxies):
         payload['chat_id'] = receiver
         self.logger.debug('Sending message to %s' % receiver)
-        response = safe_urlopen(
+        response = self.safe_urlopen(
             method='POST',
             url=url,
             json=payload,
             proxies=proxies,
         )
         self.logger.debug('Response code: %s, content: %s' % (response.status_code, response.content))
 
@@ -163,11 +221,14 @@
         self.logger.debug('Received notification for event: %s' % event)
         receivers = self.get_receivers(group.project)
         self.logger.debug('for receivers: %s' % ', '.join(receivers or ()))
         payload = self.build_message(group, event)
         self.logger.debug('Built payload: %s' % payload)
         url = self.build_url(group.project)
         self.logger.debug('Built url: %s' % url)
-        proxies = self.get_proxy(group.project)
+        proxies = {
+            'http': f'{self.get_proxy(group.project)}',
+            'https': f'{self.get_proxy(group.project)}',
+        }
         self.logger.debug('Proxy: %s' % proxies)
         for receiver in receivers:
             safe_execute(self.send_message, url, payload, receiver, proxies, _with_transaction=False)
```

### Comparing `sentry_telegram_with_proxy-0.4.2/sentry_telegram_with_proxy.egg-info/PKG-INFO` & `sentry_telegram_with_proxy-0.4.3/sentry_telegram_with_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-telegram-with-proxy
-Version: 0.4.2
+Version: 0.4.3
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/ivantzepner/sentry-telegram
 Author: Ivan Tzepner
 Author-email: ivan.tzepner@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `sentry_telegram_with_proxy-0.4.2/setup.py` & `sentry_telegram_with_proxy-0.4.3/setup.py`

 * *Files identical despite different names*

