# Comparing `tmp/nagios_historian-0.6.9.tar.gz` & `tmp/nagios_historian-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagios_historian-0.6.9.tar", last modified: Thu Apr  4 13:31:58 2024, max compression
+gzip compressed data, was "nagios_historian-0.7.0.tar", last modified: Thu Apr  4 18:42:27 2024, max compression
```

## Comparing `nagios_historian-0.6.9.tar` & `nagios_historian-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/
--rw-rw-rw-   0        0        0     1089 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/LICENSE
--rw-rw-rw-   0        0        0     3099 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     2527 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/nagios_historian/
--rw-rw-rw-   0        0        0        5 2024-04-04 13:30:48.000000 nagios_historian-0.6.9/nagios_historian/VERSION
--rw-rw-rw-   0        0        0      163 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/__init__.py
--rw-rw-rw-   0        0        0     6139 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/__main__.py
--rw-rw-rw-   0        0        0     4832 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/historian_check.py
--rw-rw-rw-   0        0        0     3288 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/oauth2_token.py
--rw-rw-rw-   0        0        0     2055 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/plugin_check.py
-drwxrwxrwx   0        0        0        0 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/nagios_historian.egg-info/
--rw-rw-rw-   0        0        0     3099 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/setup.cfg
--rw-rw-rw-   0        0        0     3329 2024-04-04 13:31:51.000000 nagios_historian-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:42:27.357814 nagios_historian-0.7.0/
+-rw-rw-rw-   0        0        0     1089 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0     3099 2024-04-04 18:42:27.357814 nagios_historian-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2527 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-04 18:42:27.342193 nagios_historian-0.7.0/nagios_historian/
+-rw-rw-rw-   0        0        0        5 2024-04-04 18:42:21.000000 nagios_historian-0.7.0/nagios_historian/VERSION
+-rw-rw-rw-   0        0        0      163 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/nagios_historian/__init__.py
+-rw-rw-rw-   0        0        0     6321 2024-04-04 17:54:02.000000 nagios_historian-0.7.0/nagios_historian/__main__.py
+-rw-rw-rw-   0        0        0     5983 2024-04-04 17:54:02.000000 nagios_historian-0.7.0/nagios_historian/historian_check.py
+-rw-rw-rw-   0        0        0     3288 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/nagios_historian/oauth2_token.py
+-rw-rw-rw-   0        0        0     2055 2024-04-04 13:29:07.000000 nagios_historian-0.7.0/nagios_historian/plugin_check.py
+drwxrwxrwx   0        0        0        0 2024-04-04 18:42:27.342193 nagios_historian-0.7.0/nagios_historian.egg-info/
+-rw-rw-rw-   0        0        0     3099 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-04 17:58:08.000000 nagios_historian-0.7.0/nagios_historian.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 18:42:27.000000 nagios_historian-0.7.0/nagios_historian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 18:42:27.357814 nagios_historian-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     3646 2024-04-04 14:26:07.000000 nagios_historian-0.7.0/setup.py
```

### Comparing `nagios_historian-0.6.9/LICENSE` & `nagios_historian-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.9/PKG-INFO` & `nagios_historian-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagios_historian
-Version: 0.6.9
+Version: 0.7.0
 Summary: nagios historian plugin
 Home-page: https://github.com/matiasgrana/nagios_historian
 Author: Matias Graña
 Author-email: maicolmatiasg@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
```

### Comparing `nagios_historian-0.6.9/README.rst` & `nagios_historian-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.9/nagios_historian/__main__.py` & `nagios_historian-0.7.0/nagios_historian/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,16 @@
                             help='oauth2 client_secret client password \n')
     parser.add_argument('--grant_type', dest='grant_type', nargs='?', default='client_credentials', const=None,
                             help='oauth2 grant_type \n')
     parser.add_argument('--auth_url', dest='auth_url', nargs='?', default=None, const=None,
                             help='oauth2 auth_url example: https://login.microsoftonline.com/company.onmicrosoft.com/oauth2/v2.0/token \n')
     parser.add_argument('--tags', dest='tags', nargs='?', default=None, const=None,
                         help='tags names of historian \n')
+    parser.add_argument('--instance', dest='instance', nargs='?', default=None, const=None,
+                        help='instance name of historian \n')
     parser.add_argument('--oauth2', action='store_true',
                             help='''Flag to use or not token for oauth2 before creating the request, used to check published services that uses azure oauth2 \n
                                     See https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token \n''')
 
     if not args:
         raise SystemExit(parser.print_help())
 
@@ -98,15 +100,15 @@
         header_token = {"Authorization": "Bearer {}".format(access_token)}
         # https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#use-the-access-token
         auth_args = "--header 'Authorization: {}'".format(header_token['Authorization'])
 
     #Create historian object    
     historianobj = HistorianChecks(url=options.url,
                               access_token=access_token,
-                              tags=options.tags)
+                              tags=options.tags,instance=options.instance)
 
     def collect_data():        
         retrcode, msgdata = historianobj.check_tags_data()
         return retrcode, msgdata
     
     def check(retrcode):
         if retrcode >= 2:
```

### Comparing `nagios_historian-0.6.9/nagios_historian/oauth2_token.py` & `nagios_historian-0.7.0/nagios_historian/oauth2_token.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.9/nagios_historian/plugin_check.py` & `nagios_historian-0.7.0/nagios_historian/plugin_check.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.9/nagios_historian.egg-info/PKG-INFO` & `nagios_historian-0.7.0/nagios_historian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagios-historian
-Version: 0.6.9
+Version: 0.7.0
 Summary: nagios historian plugin
 Home-page: https://github.com/matiasgrana/nagios_historian
 Author: Matias Graña
 Author-email: maicolmatiasg@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
```

### Comparing `nagios_historian-0.6.9/setup.py` & `nagios_historian-0.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 import os
 from os import path
 from setuptools import setup, find_packages
 #import rstcheck
 
 
+name_package = 'nagios_historian_plugin'
 mypackage_root_dir = 'nagios_historian'
 
 # function to check a readme file
 def check_readme(file='README.rst'):
     """
     Checks readme rst file, to ensure it will upload to pypi and be formatted
     correctly.
@@ -28,17 +29,24 @@
     #    raise SystemExit(msg)
     #else:
     #    msg = 'No errors in {}'.format(file)
     #    print(msg)
 
 # Get requirements for this package
 here_path = path.abspath(path.dirname(__file__))
-with open(os.path.join(here_path, 'requirements.txt')) as f:
-    requires = [x.strip() for x in f if x.strip()]
 
+if os.path.isfile('./requirements.txt'):
+    with open(os.path.join(here_path, 'requirements.txt')) as f:
+        requires = [x.strip() for x in f if x.strip()]
+elif os.path.isfile('./' + name_package + '.egg-info/requires.txt'):
+    with open('./' + name_package + '.egg-info/requires.txt') as f:
+        requires = [x.strip() for x in f if x.strip()]
+else:
+    requires=""
+    
 # Get the version from VERSION file
 with open(os.path.join(mypackage_root_dir, 'VERSION')) as version_file:
     version = version_file.read().strip()
 
 readme_path = path.join(here_path, 'README.rst')
 # Get the long description from the relevant file
 with open(readme_path, encoding='utf-8') as f:
```

