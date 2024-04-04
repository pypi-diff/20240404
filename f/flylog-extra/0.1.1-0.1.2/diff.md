# Comparing `tmp/flylog_extra-0.1.1.tar.gz` & `tmp/flylog_extra-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flylog_extra-0.1.1.tar", last modified: Thu Apr  4 04:01:49 2024, max compression
+gzip compressed data, was "dist/flylog_extra-0.1.2.tar", last modified: Thu Apr  4 04:50:49 2024, max compression
```

## Comparing `flylog_extra-0.1.1.tar` & `flylog_extra-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:01:49.000000 flylog_extra-0.1.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:01:48.000000 flylog_extra-0.1.1/flylog_extra/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:01:49.000000 flylog_extra-0.1.1/flylog_extra/api/
--rw-rw-r--   0 root         (0) root         (0)       23 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/api/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1140 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/api/client.py
--rw-rw-r--   0 root         (0) root         (0)     1637 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/api/log_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:01:49.000000 flylog_extra-0.1.1/flylog_extra/bin/
--rw-rw-r--   0 root         (0) root         (0)     1293 2024-04-04 03:49:04.000000 flylog_extra-0.1.1/flylog_extra/bin/run_flylog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:01:49.000000 flylog_extra-0.1.1/flylog_extra/server/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:01:49.000000 flylog_extra-0.1.1/flylog_extra/server/backends/
--rw-rw-r--   0 root         (0) root         (0)       23 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/backends/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3990 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/backends/ding.py
--rw-rw-r--   0 root         (0) root         (0)     2453 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/backends/mail.py
--rw-rw-r--   0 root         (0) root         (0)     2277 2024-04-02 09:02:43.000000 flylog_extra-0.1.1/flylog_extra/server/backends/send_slack.py
--rw-rw-r--   0 root         (0) root         (0)     1194 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/backends/sendcloud.py
--rw-rw-r--   0 root         (0) root         (0)       23 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      124 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/log.py
--rw-rw-r--   0 root         (0) root         (0)     3984 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/server.py
--rw-rw-r--   0 root         (0) root         (0)      527 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/six.py
--rw-rw-r--   0 root         (0) root         (0)     1760 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/server/utils.py
--rw-rw-r--   0 root         (0) root         (0)      206 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       87 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/flylog_extra/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:01:49.000000 flylog_extra-0.1.1/flylog_extra.egg-info/
--rw-r--r--   0 root         (0) root         (0)      248 2024-04-04 04:01:48.000000 flylog_extra-0.1.1/flylog_extra.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      712 2024-04-04 04:01:48.000000 flylog_extra-0.1.1/flylog_extra.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 04:01:48.000000 flylog_extra-0.1.1/flylog_extra.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 04:01:48.000000 flylog_extra-0.1.1/flylog_extra.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-04 04:01:48.000000 flylog_extra-0.1.1/flylog_extra.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      407 2024-04-03 07:30:40.000000 flylog_extra-0.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      671 2024-04-04 03:57:33.000000 flylog_extra-0.1.1/setup.py
--rw-r--r--   0 root         (0) root         (0)      248 2024-04-04 04:01:49.000000 flylog_extra-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 04:01:49.000000 flylog_extra-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra/api/
+-rw-rw-r--   0 root         (0) root         (0)       23 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/api/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1140 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/api/client.py
+-rw-rw-r--   0 root         (0) root         (0)     1637 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/api/log_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra/bin/
+-rw-rw-r--   0 root         (0) root         (0)     1299 2024-04-04 04:45:33.000000 flylog_extra-0.1.2/flylog_extra/bin/run_flylog_extra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra/server/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra/server/backends/
+-rw-rw-r--   0 root         (0) root         (0)       23 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/backends/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3990 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/backends/ding.py
+-rw-rw-r--   0 root         (0) root         (0)     2453 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/backends/mail.py
+-rw-rw-r--   0 root         (0) root         (0)     2277 2024-04-02 09:02:43.000000 flylog_extra-0.1.2/flylog_extra/server/backends/send_slack.py
+-rw-rw-r--   0 root         (0) root         (0)     1194 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/backends/sendcloud.py
+-rw-rw-r--   0 root         (0) root         (0)       23 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      124 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/log.py
+-rw-rw-r--   0 root         (0) root         (0)     3984 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/server.py
+-rw-rw-r--   0 root         (0) root         (0)      527 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/six.py
+-rw-rw-r--   0 root         (0) root         (0)     1760 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/server/utils.py
+-rw-rw-r--   0 root         (0) root         (0)      206 2024-04-04 04:38:44.000000 flylog_extra-0.1.2/flylog_extra/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       87 2024-04-03 07:30:40.000000 flylog_extra-0.1.2/flylog_extra/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 04:50:42.000000 flylog_extra-0.1.2/flylog_extra.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/flylog_extra.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      426 2024-04-04 04:45:13.000000 flylog_extra-0.1.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      677 2024-04-04 04:49:48.000000 flylog_extra-0.1.2/setup.py
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 04:50:49.000000 flylog_extra-0.1.2/setup.cfg
```

### Comparing `flylog_extra-0.1.1/flylog_extra/api/client.py` & `flylog_extra-0.1.2/flylog_extra/api/client.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra/api/log_handler.py` & `flylog_extra-0.1.2/flylog_extra/api/log_handler.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra/bin/run_flylog.py` & `flylog_extra-0.1.2/flylog_extra/bin/run_flylog_extra.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def build_parser():
     parser = argparse.ArgumentParser()
     parser.add_argument('-t', '--host', default=constants.HOST, help='bind host', action='store')
     parser.add_argument('-p', '--port', default=constants.PORT, type=int, help='bind port', action='store')
     parser.add_argument('-c', '--config', help='config file', action='store', required=True)
-    parser.add_argument('-v', '--version', action='version', version='%s' % flylog.__version__)
+    parser.add_argument('-v', '--version', action='version', version='%s' % flylog_extra.__version__)
     return parser
 
 
 def load_config(filename):
     d = types.ModuleType('config')
     d.__file__ = filename
     try:
```

### Comparing `flylog_extra-0.1.1/flylog_extra/server/backends/ding.py` & `flylog_extra-0.1.2/flylog_extra/server/backends/ding.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra/server/backends/mail.py` & `flylog_extra-0.1.2/flylog_extra/server/backends/mail.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra/server/backends/send_slack.py` & `flylog_extra-0.1.2/flylog_extra/server/backends/send_slack.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra/server/backends/sendcloud.py` & `flylog_extra-0.1.2/flylog_extra/server/backends/sendcloud.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra/server/server.py` & `flylog_extra-0.1.2/flylog_extra/server/server.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra/server/six.py` & `flylog_extra-0.1.2/flylog_extra/server/six.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra/server/utils.py` & `flylog_extra-0.1.2/flylog_extra/server/utils.py`

 * *Files identical despite different names*

### Comparing `flylog_extra-0.1.1/flylog_extra.egg-info/SOURCES.txt` & `flylog_extra-0.1.2/flylog_extra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 flylog_extra.egg-info/SOURCES.txt
 flylog_extra.egg-info/dependency_links.txt
 flylog_extra.egg-info/not-zip-safe
 flylog_extra.egg-info/top_level.txt
 flylog_extra/api/__init__.py
 flylog_extra/api/client.py
 flylog_extra/api/log_handler.py
-flylog_extra/bin/run_flylog.py
+flylog_extra/bin/run_flylog_extra.py
 flylog_extra/server/__init__.py
 flylog_extra/server/log.py
 flylog_extra/server/server.py
 flylog_extra/server/six.py
 flylog_extra/server/utils.py
 flylog_extra/server/backends/__init__.py
 flylog_extra/server/backends/ding.py
```

### Comparing `flylog_extra-0.1.1/setup.py` & `flylog_extra-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import sys
 
 PY2 = sys.version_info[0] == 2
 if PY2:
     REQUIRE_PACK = ['slackclient>=1.3.2']
-    __version__ = "0.1.1"
+    __version__ = "0.1.2"
 
 else:
     REQUIRE_PACK = ['slack_sdk>=3.19.5']
-    __version__ = "0.1.1"
+    __version__ = "0.1.2"
 
 
 
 setup(
     name="flylog_extra",
     version=__version__,
     zip_safe=False,
     platforms='any',
     packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
-    scripts=['flylog_extra/bin/run_flylog.py'],
+    scripts=['flylog_extra/bin/run_flylog_extra.py'],
     url="https://github.com/dkxx00/flylog-extra",
     license="BSD",
     author="dkxx00",
-    author_email="hymanxx6@gmail.com",
+    author_email="dkxx00@outlook.com",
     description="make log fly to mail or other(slack)",
 )
```

