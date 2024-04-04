# Comparing `tmp/nagios_historian-0.6.8.tar.gz` & `tmp/nagios_historian-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nagios_historian-0.6.8.tar", last modified: Wed Apr  3 19:18:32 2024, max compression
+gzip compressed data, was "nagios_historian-0.6.9.tar", last modified: Thu Apr  4 13:31:58 2024, max compression
```

## Comparing `nagios_historian-0.6.8.tar` & `nagios_historian-0.6.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/
--rw-rw-rw-   0        0        0     1089 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/LICENSE
--rw-rw-rw-   0        0        0     3099 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     2527 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/nagios_historian/
--rw-rw-rw-   0        0        0        7 2024-04-03 19:14:19.000000 nagios_historian-0.6.8/nagios_historian/VERSION
--rw-rw-rw-   0        0        0      163 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/__init__.py
--rw-rw-rw-   0        0        0     6139 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/__main__.py
--rw-rw-rw-   0        0        0     4832 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/historian_check.py
--rw-rw-rw-   0        0        0     3288 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/oauth2_token.py
--rw-rw-rw-   0        0        0     2055 2024-04-03 19:11:56.000000 nagios_historian-0.6.8/nagios_historian/plugin_check.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/nagios_historian.egg-info/
--rw-rw-rw-   0        0        0     3099 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-03 19:18:32.000000 nagios_historian-0.6.8/nagios_historian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 19:18:32.696434 nagios_historian-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     3328 2024-04-03 19:18:30.000000 nagios_historian-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/
+-rw-rw-rw-   0        0        0     1089 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/LICENSE
+-rw-rw-rw-   0        0        0     3099 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2527 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/nagios_historian/
+-rw-rw-rw-   0        0        0        5 2024-04-04 13:30:48.000000 nagios_historian-0.6.9/nagios_historian/VERSION
+-rw-rw-rw-   0        0        0      163 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/__init__.py
+-rw-rw-rw-   0        0        0     6139 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/__main__.py
+-rw-rw-rw-   0        0        0     4832 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/historian_check.py
+-rw-rw-rw-   0        0        0     3288 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/oauth2_token.py
+-rw-rw-rw-   0        0        0     2055 2024-04-04 13:29:07.000000 nagios_historian-0.6.9/nagios_historian/plugin_check.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/nagios_historian.egg-info/
+-rw-rw-rw-   0        0        0     3099 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-04 13:31:57.000000 nagios_historian-0.6.9/nagios_historian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 13:31:58.057799 nagios_historian-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     3329 2024-04-04 13:31:51.000000 nagios_historian-0.6.9/setup.py
```

### Comparing `nagios_historian-0.6.8/LICENSE` & `nagios_historian-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.8/PKG-INFO` & `nagios_historian-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagios_historian
-Version: 0.6.8
+Version: 0.6.9
 Summary: nagios historian plugin
 Home-page: https://github.com/matiasgrana/nagios_historian
 Author: Matias Graña
 Author-email: maicolmatiasg@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
```

### Comparing `nagios_historian-0.6.8/README.rst` & `nagios_historian-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.8/nagios_historian/__main__.py` & `nagios_historian-0.6.9/nagios_historian/__main__.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.8/nagios_historian/historian_check.py` & `nagios_historian-0.6.9/nagios_historian/historian_check.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.8/nagios_historian/oauth2_token.py` & `nagios_historian-0.6.9/nagios_historian/oauth2_token.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.8/nagios_historian/plugin_check.py` & `nagios_historian-0.6.9/nagios_historian/plugin_check.py`

 * *Files identical despite different names*

### Comparing `nagios_historian-0.6.8/nagios_historian.egg-info/PKG-INFO` & `nagios_historian-0.6.9/nagios_historian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nagios-historian
-Version: 0.6.8
+Version: 0.6.9
 Summary: nagios historian plugin
 Home-page: https://github.com/matiasgrana/nagios_historian
 Author: Matias Graña
 Author-email: maicolmatiasg@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
```

### Comparing `nagios_historian-0.6.8/setup.py` & `nagios_historian-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # http://python-packaging.readthedocs.io/en/latest/minimal.html
 # Help from: http://www.scotttorborg.com/python-packaging/minimal.html
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 import os
 from os import path
 from setuptools import setup, find_packages
-import rstcheck
+#import rstcheck
 
 
 mypackage_root_dir = 'nagios_historian'
 
 # function to check a readme file
 def check_readme(file='README.rst'):
     """
@@ -19,20 +19,20 @@
     """
     # Get the long description from the relevant file
     with open(file, encoding='utf-8') as f_object:
         readme_content = f_object.read()
 
     #errors = list(rstcheck.check(readme_content))
     #if errors:
-     #   msg = 'There_path are errors in {}, errors \n {}'.format(file,
-      #                                                      errors[0].message)
-       # raise SystemExit(msg)
+    #    msg = 'There_path are errors in {}, errors \n {}'.format(file,
+    #                                                        errors[0].message)
+    #    raise SystemExit(msg)
     #else:
-     #   msg = 'No errors in {}'.format(file)
-     #   print(msg)
+    #    msg = 'No errors in {}'.format(file)
+    #    print(msg)
 
 # Get requirements for this package
 here_path = path.abspath(path.dirname(__file__))
 with open(os.path.join(here_path, 'requirements.txt')) as f:
     requires = [x.strip() for x in f if x.strip()]
 
 # Get the version from VERSION file
```

