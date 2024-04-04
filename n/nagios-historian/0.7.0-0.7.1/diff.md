# Comparing `tmp/nagios_historian-0.7.0.tar.gz` & `tmp/nagios_historian-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagios_historian-0.7.0.tar", last modified: Thu Apr  4 18:42:27 2024, max compression
+gzip compressed data, was "nagios_historian-0.7.1.tar", last modified: Thu Apr  4 19:29:40 2024, max compression
```

## Comparing `nagios_historian-0.7.0.tar` & `nagios_historian-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 18:42:27.357814 nagios_historian-0.7.0/
--rw-rw-rw-   0        0        0     1089 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     3099 2024-04-04 18:42:27.357814 nagios_historian-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     2527 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-04 18:42:27.342193 nagios_historian-0.7.0/nagios_historian/
--rw-rw-rw-   0        0        0        5 2024-04-04 18:42:21.000000 nagios_historian-0.7.0/nagios_historian/VERSION
--rw-rw-rw-   0        0        0      163 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/nagios_historian/__init__.py
--rw-rw-rw-   0        0        0     6321 2024-04-04 17:54:02.000000 nagios_historian-0.7.0/nagios_historian/__main__.py
--rw-rw-rw-   0        0        0     5983 2024-04-04 17:54:02.000000 nagios_historian-0.7.0/nagios_historian/historian_check.py
--rw-rw-rw-   0        0        0     3288 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/nagios_historian/oauth2_token.py
--rw-rw-rw-   0        0        0     2055 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/nagios_historian/plugin_check.py
-drwxrwxrwx   0        0        0        0 2024-04-04 18:42:27.342193 nagios_historian-0.7.0/nagios_historian.egg-info/
--rw-rw-rw-   0        0        0     3099 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-04 17:58:08.000000 nagios_historian-0.7.0/nagios_historian.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 18:42:27.357814 nagios_historian-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     3646 2024-04-04 14:26:07.000000 nagios_historian-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:29:40.923386 nagios_historian-0.7.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-04 19:14:18.000000 nagios_historian-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     3099 2024-04-04 19:29:40.923386 nagios_historian-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2527 2024-04-04 19:14:18.000000 nagios_historian-0.7.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-04 19:29:40.913366 nagios_historian-0.7.1/nagios_historian/
+-rw-rw-rw-   0        0        0        5 2024-04-04 19:28:23.000000 nagios_historian-0.7.1/nagios_historian/VERSION
+-rw-rw-rw-   0        0        0      163 2024-04-04 19:14:18.000000 nagios_historian-0.7.1/nagios_historian/__init__.py
+-rw-rw-rw-   0        0        0     6321 2024-04-04 19:14:18.000000 nagios_historian-0.7.1/nagios_historian/__main__.py
+-rw-rw-rw-   0        0        0     6004 2024-04-04 19:14:18.000000 nagios_historian-0.7.1/nagios_historian/historian_check.py
+-rw-rw-rw-   0        0        0     3288 2024-04-04 19:14:18.000000 nagios_historian-0.7.1/nagios_historian/oauth2_token.py
+-rw-rw-rw-   0        0        0     2055 2024-04-04 19:14:18.000000 nagios_historian-0.7.1/nagios_historian/plugin_check.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:29:40.918381 nagios_historian-0.7.1/nagios_historian.egg-info/
+-rw-rw-rw-   0        0        0     3099 2024-04-04 19:29:40.000000 nagios_historian-0.7.1/nagios_historian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-04 19:29:40.000000 nagios_historian-0.7.1/nagios_historian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:29:40.000000 nagios_historian-0.7.1/nagios_historian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-04 19:29:40.000000 nagios_historian-0.7.1/nagios_historian.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-04 19:29:40.000000 nagios_historian-0.7.1/nagios_historian.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-04-04 19:29:40.000000 nagios_historian-0.7.1/nagios_historian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 19:29:40.000000 nagios_historian-0.7.1/nagios_historian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:29:40.923386 nagios_historian-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     3646 2024-04-04 19:16:50.000000 nagios_historian-0.7.1/setup.py
```

### Comparing `nagios_historian-0.7.0/LICENSE` & `nagios_historian-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.7.0/PKG-INFO` & `nagios_historian-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagios_historian
-Version: 0.7.0
+Version: 0.7.1
 Summary: nagios historian plugin
 Home-page: https://github.com/matiasgrana/nagios_historian
 Author: Matias Graña
 Author-email: maicolmatiasg@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
```

### Comparing `nagios_historian-0.7.0/README.rst` & `nagios_historian-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.7.0/nagios_historian/__main__.py` & `nagios_historian-0.7.1/nagios_historian/__main__.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.7.0/nagios_historian/historian_check.py` & `nagios_historian-0.7.1/nagios_historian/historian_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,16 @@
 
                 #Validate Quality (0 – Bad,  1 – Uncertain, 2 – NA , 3 – Good)
                 if Quality != 3:
                     retrcode = CRITICAL
                     retrcodetag = CRITICAL
 
                 #Validate Value (0 = Ok)
-                if not TagName in [self.STATUS_SAC_STATUS , self.STATUS_WS_SERVICE, self.STATUS_SAC_CYCLES_SEC, self.STATUS_SAC_OVERRUNS, self.STATUS_WS_ACTIVE_SESSIONS , self.STATUS_WS_CLIENT_CONNECTIONS , self.STATUS_WS_HOST_CONNECTIONS , self.STATUS_WS_MAXIMUM_SESSIONS, self.STATUS_LAST_UPDATE]:                       if Value != '0':
+                if not TagName in [self.STATUS_SAC_STATUS , self.STATUS_WS_SERVICE, self.STATUS_SAC_CYCLES_SEC, self.STATUS_SAC_OVERRUNS, self.STATUS_WS_ACTIVE_SESSIONS , self.STATUS_WS_CLIENT_CONNECTIONS , self.STATUS_WS_HOST_CONNECTIONS , self.STATUS_WS_MAXIMUM_SESSIONS, self.STATUS_LAST_UPDATE]:                      
+                    if Value != '0':
                         retrcode = CRITICAL
                         retrcodetag = CRITICAL
 
                 #STATUS_SAC_STATUS / STATUS_WS_SERVICE - ( 0=STOP | 1=RUN )
                 if TagName in [self.STATUS_SAC_STATUS , self.STATUS_WS_SERVICE] and Value != '1':
                     retrcode = CRITICAL
                     retrcodetag = CRITICAL
```

### Comparing `nagios_historian-0.7.0/nagios_historian/oauth2_token.py` & `nagios_historian-0.7.1/nagios_historian/oauth2_token.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.7.0/nagios_historian/plugin_check.py` & `nagios_historian-0.7.1/nagios_historian/plugin_check.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.7.0/nagios_historian.egg-info/PKG-INFO` & `nagios_historian-0.7.1/nagios_historian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagios-historian
-Version: 0.7.0
+Version: 0.7.1
 Summary: nagios historian plugin
 Home-page: https://github.com/matiasgrana/nagios_historian
 Author: Matias Graña
 Author-email: maicolmatiasg@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
```

### Comparing `nagios_historian-0.7.0/setup.py` & `nagios_historian-0.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 import os
 from os import path
 from setuptools import setup, find_packages
 #import rstcheck
 
 
-name_package = 'nagios_historian_plugin'
 mypackage_root_dir = 'nagios_historian'
+name_package = 'nagios_historian_plugin'
+
+
 
 # function to check a readme file
 def check_readme(file='README.rst'):
     """
     Checks readme rst file, to ensure it will upload to pypi and be formatted
     correctly.
     :param file:
@@ -38,15 +40,15 @@
     with open(os.path.join(here_path, 'requirements.txt')) as f:
         requires = [x.strip() for x in f if x.strip()]
 elif os.path.isfile('./' + name_package + '.egg-info/requires.txt'):
     with open('./' + name_package + '.egg-info/requires.txt') as f:
         requires = [x.strip() for x in f if x.strip()]
 else:
     requires=""
-    
+
 # Get the version from VERSION file
 with open(os.path.join(mypackage_root_dir, 'VERSION')) as version_file:
     version = version_file.read().strip()
 
 readme_path = path.join(here_path, 'README.rst')
 # Get the long description from the relevant file
 with open(readme_path, encoding='utf-8') as f:
```

