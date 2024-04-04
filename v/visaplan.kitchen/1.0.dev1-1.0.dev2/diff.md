# Comparing `tmp/visaplan.kitchen-1.0.dev1.tar.gz` & `tmp/visaplan.kitchen-1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visaplan.kitchen-1.0.dev1.tar", last modified: Mon Jul  9 15:46:20 2018, max compression
+gzip compressed data, was "dist/visaplan.kitchen-1.0.dev2.tar", last modified: Mon Sep 17 12:54:55 2018, max compression
```

## Comparing `visaplan.kitchen-1.0.dev1.tar` & `visaplan.kitchen-1.0.dev2.tar`

### file list

```diff
@@ -1,29 +1,33 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/docs/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2018-07-09 14:50:22.000000 visaplan.kitchen-1.0.dev1/docs/LICENSE.GPL
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      658 2018-07-09 15:18:54.000000 visaplan.kitchen-1.0.dev1/docs/LICENSE.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      151 2018-07-09 15:20:05.000000 visaplan.kitchen-1.0.dev1/docs/index.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan/kitchen/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan/kitchen/tests/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      354 2018-07-09 15:38:26.000000 visaplan.kitchen-1.0.dev1/src/visaplan/kitchen/tests/test_doctests.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       56 2018-07-09 15:07:51.000000 visaplan.kitchen-1.0.dev1/src/visaplan/kitchen/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    75774 2018-07-09 15:43:44.000000 visaplan.kitchen-1.0.dev1/src/visaplan/kitchen/spoons.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       56 2018-07-09 15:07:51.000000 visaplan.kitchen-1.0.dev1/src/visaplan/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3213 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      604 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       26 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2018-07-09 15:36:41.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      105 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       95 2018-07-09 14:50:22.000000 visaplan.kitchen-1.0.dev1/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2018-07-09 14:50:22.000000 visaplan.kitchen-1.0.dev1/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       65 2018-07-09 14:50:22.000000 visaplan.kitchen-1.0.dev1/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1614 2018-07-09 15:24:16.000000 visaplan.kitchen-1.0.dev1/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2399 2018-07-09 15:30:09.000000 visaplan.kitchen-1.0.dev1/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3213 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       38 2018-07-09 15:46:20.000000 visaplan.kitchen-1.0.dev1/setup.cfg
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/docs/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2018-07-09 14:50:22.000000 visaplan.kitchen-1.0.dev2/docs/LICENSE.GPL
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      669 2018-09-17 11:36:46.000000 visaplan.kitchen-1.0.dev2/docs/LICENSE.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      151 2018-07-09 15:20:05.000000 visaplan.kitchen-1.0.dev2/docs/index.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/tests/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      354 2018-07-09 15:38:26.000000 visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/tests/test_doctests.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2018-07-10 15:44:37.000000 visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      257 2018-09-17 11:22:28.000000 visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13124 2018-07-10 10:25:15.000000 visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/forks.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3472 2018-07-10 11:31:27.000000 visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/ids.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    75738 2018-09-17 11:35:17.000000 visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/spoons.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      245 2018-09-17 11:23:30.000000 visaplan.kitchen-1.0.dev2/src/visaplan/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3681 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      706 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2018-07-09 15:36:41.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      120 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      191 2018-09-17 12:53:27.000000 visaplan.kitchen-1.0.dev2/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2018-07-09 14:50:22.000000 visaplan.kitchen-1.0.dev2/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       81 2018-09-17 11:23:29.000000 visaplan.kitchen-1.0.dev2/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1852 2018-09-17 12:45:57.000000 visaplan.kitchen-1.0.dev2/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        4 2018-07-09 15:29:59.000000 visaplan.kitchen-1.0.dev2/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2571 2018-09-17 12:51:24.000000 visaplan.kitchen-1.0.dev2/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3681 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       38 2018-09-17 12:54:55.000000 visaplan.kitchen-1.0.dev2/setup.cfg
```

### Comparing `visaplan.kitchen-1.0.dev1/docs/LICENSE.GPL` & `visaplan.kitchen-1.0.dev2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `visaplan.kitchen-1.0.dev1/docs/LICENSE.rst` & `visaplan.kitchen-1.0.dev2/docs/LICENSE.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-visaplan.kitchen Copyright 2018, Tobias Herp
+visaplan.kitchen Copyright 2018, visaplan GmbH, Germany
 
 This program is free software; you can redistribute it and/or
 modify it under the terms of the GNU General Public License version 2
 as published by the Free Software Foundation.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `visaplan.kitchen-1.0.dev1/src/visaplan/kitchen/spoons.py` & `visaplan.kitchen-1.0.dev2/src/visaplan/kitchen/spoons.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 from bs4 import Tag, NavigableString, BeautifulSoup
 
 # Unitracc-Tools:
 from visaplan.tools.html import (entity,
         BLOCK_ELEMENT_NAMES, EMPTY_ELEMENT_NAMES, REPLACED_ELEMENT_NAMES,
         )
 from visaplan.tools.sequences import inject_indexes
-from visaplan.tools.debug import pp
 
 
 # -------------------------------------------- [ Daten ... [
 SOFT_HYPHEN = entity['shy']
 # -------------------------------------------- ] ... Daten ]
```

### Comparing `visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/PKG-INFO` & `visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.kitchen
-Version: 1.0.dev1
+Version: 1.0.dev2
 Summary: A kitchen for (beautiful) soup
 Home-page: https://pypi.org/project/visaplan.kitchen
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -13,42 +13,49 @@
         ================
         visaplan.kitchen
         ================
         
         This package tackles "soup", i.e. trees which are created by the well-known
         beautifulsoup4 package from parsed HTML or XML sources.
         It might be possible to accomplish the same by using lxml directly,
-        but it probably would have been more difficult, and thus it is left to another
+        but it might have been more difficult, and thus it is left to another
         product.
         
         Features
         --------
         
-        - Can be bullet points
+        - ``spoons`` module, for tackling "soup", e.g.
+        
+          - ``has_any_class`` (a filter function to check for one of the given classes)
+        
+        - ``forks`` module
+          (named mainly for historical reasons; for poking around in the soup), e.g.
+          ``extract_linktext``, ``convert_dimension_styles``
+        
+        - ``ids`` module, for creation of new ids for HTML elements
+        
+          - ``id_factory``::
+        
+            new_id = id_factory(...)
+            id = new_id(prefix)
         
         
         Examples
         --------
         
         This add-on can be seen in action at the following sites:
-        - Is there a page on the internet where everybody can see the features?
+        
+        - https://www.unitracc.de
+        - https://www.unitracc.com
         
         
         Documentation
         -------------
         
-        Full documentation for end users can be found in the "docs" folder.
-        
-        
-        Translations
-        ------------
-        
-        This product has been translated into
-        
-        - Klingon (thanks, K'Plai)
+        For now, the functions are documented by doctests.
         
         
         Installation
         ------------
         
         Install visaplan.kitchen by adding it to your buildout::
         
@@ -62,52 +69,60 @@
         
         and then running ``bin/buildout``
         
         
         Contribute
         ----------
         
-        - Issue Tracker: https://github.com/visaplan/visaplan.UnitraccShop/issues
-        - Source Code: https://github.com/visaplan/visaplan.PACKAGE
-        - Documentation: https://docs.plone.org/foo/bar
+        - Issue Tracker: https://github.com/visaplan/visaplan.kitchen/issues
+        - Source Code: https://github.com/visaplan/visaplan.kitchen
         
         
         Support
         -------
         
         If you are having issues, please let us know;
         please use the issue tracker mentioned above.
         
         
         License
         -------
         
         The project is licensed under the GPLv2.
         
+        .. vim: tw=79 cc=+1 sw=4 sts=4 si et
+        
         
         Contributors
         ============
         
         - Tobias Herp, tobias.herp@visaplan.com
         
         
         Changelog
         =========
         
         
-        1.0a1 (unreleased)
-        ------------------
+        1.0.dev2 (2018-09-17)
+        ---------------------
+        
+        - License changed to GPL v2
+          [tobiasherp]
+        
+        
+        1.0.dev1 (2018-07-09)
+        ---------------------
         
         - Initial release.
           [tobiasherp]
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: German
 Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Provides-Extra: test
```

### Comparing `visaplan.kitchen-1.0.dev1/src/visaplan.kitchen.egg-info/SOURCES.txt` & `visaplan.kitchen-1.0.dev2/src/visaplan.kitchen.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 CHANGES.rst
 CONTRIBUTORS.rst
 MANIFEST.in
 README.rst
+VERSION
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.rst
 docs/index.rst
 src/visaplan/__init__.py
 src/visaplan.kitchen.egg-info/PKG-INFO
 src/visaplan.kitchen.egg-info/SOURCES.txt
 src/visaplan.kitchen.egg-info/dependency_links.txt
 src/visaplan.kitchen.egg-info/entry_points.txt
 src/visaplan.kitchen.egg-info/namespace_packages.txt
 src/visaplan.kitchen.egg-info/not-zip-safe
 src/visaplan.kitchen.egg-info/requires.txt
 src/visaplan.kitchen.egg-info/top_level.txt
 src/visaplan/kitchen/__init__.py
+src/visaplan/kitchen/configure.zcml
+src/visaplan/kitchen/forks.py
+src/visaplan/kitchen/ids.py
 src/visaplan/kitchen/spoons.py
 src/visaplan/kitchen/tests/test_doctests.py
```

### Comparing `visaplan.kitchen-1.0.dev1/setup.py` & `visaplan.kitchen-1.0.dev2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 # -*- coding: utf-8 -*- vim: et ts=8 sw=4 sts=4 si tw=79 cc=+8
 """Installer for the visaplan.kitchen package."""
 
 from setuptools import find_packages
 from setuptools import setup
-# ---------------------------------------- [ destination locking ... [
-import sys, os
-try:  # Python 3:
-    from configparser import ConfigParser
-except ImportError:
-    # Python 2:
-    from ConfigParser import ConfigParser
-# ---------------------------------------- ] ... destination locking ]
 
+package_name = 'visaplan.kitchen'
 VERSION = (open('VERSION').read().strip()
-           + '.dev1'  # in branches only
+           + '.dev2'  # in branches only
            )
 
 
+# ------------------------------------------- [ for setup_kwargs ... [
 long_description = '\n\n'.join([
     open('README.rst').read(),
     open('CONTRIBUTORS.rst').read(),
     open('CHANGES.rst').read(),
 ])
 
+# see as well --> src/visaplan/kitchen/configure.zcml:
+exclude_subpackages = (
+        )
+exclude_packages = []
+for subp in exclude_subpackages:
+    exclude_packages.extend([package_name + '.' + subp,
+                             package_name + '.' + subp + '.*',
+                             ])
+packages = find_packages(
+            'src',
+            exclude=exclude_packages)
+# ------------------------------------------- ] ... for setup_kwargs ]
 
-setup(
-    name='visaplan.kitchen',
-    # see also --> ./visaplan.kitchen.egg-info/PKG-INFO: 
+setup_kwargs = dict(
+    name=package_name,
     version=VERSION,
     description="A kitchen for (beautiful) soup",
     long_description=long_description,
     # Get more from https://pypi.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.7",
         "Intended Audience :: Developers",
         "Natural Language :: German",
         "Operating System :: OS Independent",
-        "License :: OSI Approved :: Apache Software License",
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     ],
     # keywords='Python Plone',
     author='Tobias Herp',
     author_email='tobias.herp@visaplan.com',
     url='https://pypi.org/project/visaplan.kitchen',
     license='GPL version 2',
-    # packages=find_packages('src', exclude=['ez_setup']),
-    packages=find_packages('src'),
+    packages=packages,
     namespace_packages=[
         'visaplan',
-        'visaplan.kitchen',
         ],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'setuptools',
         # -*- Extra requirements: -*-
         'beautifulsoup4',
+        'visaplan.tools',
     ],
     extras_require={
         'test': [
             'plone.app.testing',
             # Plone KGS does not use this version, because it would break
             # Remove if your package shall be part of coredev.
             # plone_coredev tests as of 2016-04-01.
@@ -72,7 +76,8 @@
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
 )
+setup(**setup_kwargs)
```

### Comparing `visaplan.kitchen-1.0.dev1/PKG-INFO` & `visaplan.kitchen-1.0.dev2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.kitchen
-Version: 1.0.dev1
+Version: 1.0.dev2
 Summary: A kitchen for (beautiful) soup
 Home-page: https://pypi.org/project/visaplan.kitchen
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Description: .. This README is meant for consumption by humans and pypi. Pypi can render rst files so please do not use Sphinx features.
            If you want to learn more about writing documentation, please check out: http://docs.plone.org/about/documentation_styleguide.html
@@ -13,42 +13,49 @@
         ================
         visaplan.kitchen
         ================
         
         This package tackles "soup", i.e. trees which are created by the well-known
         beautifulsoup4 package from parsed HTML or XML sources.
         It might be possible to accomplish the same by using lxml directly,
-        but it probably would have been more difficult, and thus it is left to another
+        but it might have been more difficult, and thus it is left to another
         product.
         
         Features
         --------
         
-        - Can be bullet points
+        - ``spoons`` module, for tackling "soup", e.g.
+        
+          - ``has_any_class`` (a filter function to check for one of the given classes)
+        
+        - ``forks`` module
+          (named mainly for historical reasons; for poking around in the soup), e.g.
+          ``extract_linktext``, ``convert_dimension_styles``
+        
+        - ``ids`` module, for creation of new ids for HTML elements
+        
+          - ``id_factory``::
+        
+            new_id = id_factory(...)
+            id = new_id(prefix)
         
         
         Examples
         --------
         
         This add-on can be seen in action at the following sites:
-        - Is there a page on the internet where everybody can see the features?
+        
+        - https://www.unitracc.de
+        - https://www.unitracc.com
         
         
         Documentation
         -------------
         
-        Full documentation for end users can be found in the "docs" folder.
-        
-        
-        Translations
-        ------------
-        
-        This product has been translated into
-        
-        - Klingon (thanks, K'Plai)
+        For now, the functions are documented by doctests.
         
         
         Installation
         ------------
         
         Install visaplan.kitchen by adding it to your buildout::
         
@@ -62,52 +69,60 @@
         
         and then running ``bin/buildout``
         
         
         Contribute
         ----------
         
-        - Issue Tracker: https://github.com/visaplan/visaplan.UnitraccShop/issues
-        - Source Code: https://github.com/visaplan/visaplan.PACKAGE
-        - Documentation: https://docs.plone.org/foo/bar
+        - Issue Tracker: https://github.com/visaplan/visaplan.kitchen/issues
+        - Source Code: https://github.com/visaplan/visaplan.kitchen
         
         
         Support
         -------
         
         If you are having issues, please let us know;
         please use the issue tracker mentioned above.
         
         
         License
         -------
         
         The project is licensed under the GPLv2.
         
+        .. vim: tw=79 cc=+1 sw=4 sts=4 si et
+        
         
         Contributors
         ============
         
         - Tobias Herp, tobias.herp@visaplan.com
         
         
         Changelog
         =========
         
         
-        1.0a1 (unreleased)
-        ------------------
+        1.0.dev2 (2018-09-17)
+        ---------------------
+        
+        - License changed to GPL v2
+          [tobiasherp]
+        
+        
+        1.0.dev1 (2018-07-09)
+        ---------------------
         
         - Initial release.
           [tobiasherp]
         
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: 4.3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: German
 Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Provides-Extra: test
```

