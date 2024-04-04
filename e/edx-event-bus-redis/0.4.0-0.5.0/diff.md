# Comparing `tmp/edx_event_bus_redis-0.4.0.tar.gz` & `tmp/edx_event_bus_redis-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx_event_bus_redis-0.4.0.tar", last modified: Mon Mar 11 14:43:46 2024, max compression
+gzip compressed data, was "edx_event_bus_redis-0.5.0.tar", last modified: Thu Apr  4 04:40:56 2024, max compression
```

## Comparing `edx_event_bus_redis-0.4.0.tar` & `edx_event_bus_redis-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.023072 edx_event_bus_redis-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-03-11 14:43:46.023072 edx_event_bus_redis-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.019072 edx_event_bus_redis-0.4.0/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.019072 edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    20605 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.019072 edx_event_bus_redis-0.4.0/edx_event_bus_redis/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.019072 edx_event_bus_redis-0.4.0/edx_event_bus_redis/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/management/commands/produce_event.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.015071 edx_event_bus_redis-0.4.0/edx_event_bus_redis/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.019072 edx_event_bus_redis-0.4.0/edx_event_bus_redis/templates/edx_event_bus_redis/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.023072 edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13559 2024-03-11 14:43:46.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-11 14:43:46.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 14:43:46.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 14:43:46.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-11 14:43:46.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-11 14:43:46.000000 edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.019072 edx_event_bus_redis-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-11 14:43:46.023072 edx_event_bus_redis-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:43:46.019072 edx_event_bus_redis-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-11 14:43:40.000000 edx_event_bus_redis-0.4.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:55.996103 edx_event_bus_redis-0.5.0/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20605 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/producer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/edx_event_bus_redis/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/edx_event_bus_redis/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/management/commands/produce_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:55.996103 edx_event_bus_redis-0.5.0/edx_event_bus_redis/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/edx_event_bus_redis/templates/edx_event_bus_redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13610 2024-04-04 04:40:55.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-04 04:40:55.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:40:55.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:40:55.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 04:40:55.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 04:40:55.000000 edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:40:56.000103 edx_event_bus_redis-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-04 04:40:52.000000 edx_event_bus_redis-0.5.0/tests/test_models.py
```

### Comparing `edx_event_bus_redis-0.4.0/CHANGELOG.rst` & `edx_event_bus_redis-0.5.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/LICENSE.txt` & `edx_event_bus_redis-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/PKG-INFO` & `edx_event_bus_redis-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_redis
-Version: 0.4.0
+Version: 0.5.0
 Summary: Redis Streams implementation for the Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-redis
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: Django
 Requires-Dist: edx_django_utils
 Requires-Dist: edx_toggles
 Requires-Dist: openedx-events>=9.5.0
```

### Comparing `edx_event_bus_redis-0.4.0/README.rst` & `edx_event_bus_redis-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/config.py` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/config.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/consumer.py` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/consumer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/message.py` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/message.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/producer.py` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/producer.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis/internal/utils.py` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis/management/commands/produce_event.py` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis/management/commands/produce_event.py`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis/templates/edx_event_bus_redis/base.html`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/PKG-INFO` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: edx_event_bus_redis
-Version: 0.4.0
+Version: 0.5.0
 Summary: Redis Streams implementation for the Open edX event bus.
 Home-page: https://github.com/openedx/event-bus-redis
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: Django
 Requires-Dist: edx_django_utils
 Requires-Dist: edx_toggles
 Requires-Dist: openedx-events>=9.5.0
```

### Comparing `edx_event_bus_redis-0.4.0/edx_event_bus_redis.egg-info/SOURCES.txt` & `edx_event_bus_redis-0.5.0/edx_event_bus_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx_event_bus_redis-0.4.0/requirements/constraints.txt` & `edx_event_bus_redis-0.5.0/requirements/constraints.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,7 +6,9 @@
 # When pinning something here, please provide an explanation of why.  Ideally,
 # link to other information that will help people in the future to remove the
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
 # Common constraints for edx repos
 -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+
+backports.zoneinfo;python_version<"3.9"
```

### Comparing `edx_event_bus_redis-0.4.0/setup.py` & `edx_event_bus_redis-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,10 +156,11 @@
         'Framework :: Django',
         'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
 )
```

