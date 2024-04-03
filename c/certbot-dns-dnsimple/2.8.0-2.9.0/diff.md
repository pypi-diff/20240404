# Comparing `tmp/certbot-dns-dnsimple-2.8.0.tar.gz` & `tmp/certbot-dns-dnsimple-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-dnsimple-2.8.0.tar", last modified: Tue Dec  5 19:14:03 2023, max compression
+gzip compressed data, was "certbot-dns-dnsimple-2.9.0.tar", last modified: Thu Feb  8 19:45:30 2024, max compression
```

## Comparing `certbot-dns-dnsimple-2.8.0.tar` & `certbot-dns-dnsimple-2.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:03.039121 certbot-dns-dnsimple-2.8.0/
--rw-rw-r--   0 willg     (1000) willg     (1000)    10786 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/LICENSE.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      154 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/MANIFEST.in
--rw-r--r--   0 willg     (1000) willg     (1000)     1398 2023-12-05 19:14:03.039121 certbot-dns-dnsimple-2.8.0/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)       46 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/README.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:03.035121 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/
--rw-rw-r--   0 willg     (1000) willg     (1000)     3407 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/__init__.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:03.039121 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/_internal/
--rw-rw-r--   0 willg     (1000) willg     (1000)       78 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/_internal/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1852 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/_internal/dns_dnsimple.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:03.039121 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/_internal/tests/
--rw-rw-r--   0 willg     (1000) willg     (1000)       33 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/_internal/tests/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1169 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/_internal/tests/dns_dnsimple_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/py.typed
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:03.039121 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/
--rw-r--r--   0 willg     (1000) willg     (1000)     1398 2023-12-05 19:14:03.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)      654 2023-12-05 19:14:03.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/SOURCES.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        1 2023-12-05 19:14:03.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/dependency_links.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       91 2023-12-05 19:14:03.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/entry_points.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      118 2023-12-05 19:14:03.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/requires.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       21 2023-12-05 19:14:03.000000 certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/top_level.txt
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:03.039121 certbot-dns-dnsimple-2.8.0/docs/
--rw-rw-r--   0 willg     (1000) willg     (1000)        9 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/docs/.gitignore
--rw-rw-r--   0 willg     (1000) willg     (1000)      617 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/docs/Makefile
--rw-rw-r--   0 willg     (1000) willg     (1000)      149 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/docs/api.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     5399 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/docs/conf.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      565 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/docs/index.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      829 2023-12-05 19:13:52.000000 certbot-dns-dnsimple-2.8.0/docs/make.bat
--rw-rw-r--   0 willg     (1000) willg     (1000)       38 2023-12-05 19:14:03.039121 certbot-dns-dnsimple-2.8.0/setup.cfg
--rw-rw-r--   0 willg     (1000) willg     (1000)     2292 2023-12-05 19:13:53.000000 certbot-dns-dnsimple-2.8.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:30.603135 certbot-dns-dnsimple-2.9.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      154 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/MANIFEST.in
+-rw-r--r--   0 erica     (1001) erica     (1001)     1449 2024-02-08 19:45:30.603135 certbot-dns-dnsimple-2.9.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       46 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:30.599135 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3407 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:30.599135 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       78 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1852 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/_internal/dns_dnsimple.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:30.599135 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       33 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1169 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/_internal/tests/dns_dnsimple_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:30.603135 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/
+-rw-r--r--   0 erica     (1001) erica     (1001)     1449 2024-02-08 19:45:30.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      654 2024-02-08 19:45:30.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2024-02-08 19:45:30.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       91 2024-02-08 19:45:30.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      118 2024-02-08 19:45:30.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       21 2024-02-08 19:45:30.000000 certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:30.603135 certbot-dns-dnsimple-2.9.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      617 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5399 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      565 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      829 2024-02-08 19:45:17.000000 certbot-dns-dnsimple-2.9.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2024-02-08 19:45:30.603135 certbot-dns-dnsimple-2.9.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2342 2024-02-08 19:45:18.000000 certbot-dns-dnsimple-2.9.0/setup.py
```

### Comparing `certbot-dns-dnsimple-2.8.0/LICENSE.txt` & `certbot-dns-dnsimple-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/PKG-INFO` & `certbot-dns-dnsimple-2.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-dnsimple
-Version: 2.8.0
+Version: 2.9.0
 Summary: DNSimple DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,24 +13,25 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: dns-lexicon>=3.14.1
 Requires-Dist: setuptools>=41.6.0
-Requires-Dist: acme>=2.8.0
-Requires-Dist: certbot>=2.8.0
+Requires-Dist: acme>=2.9.0
+Requires-Dist: certbot>=2.9.0
 Provides-Extra: docs
 Requires-Dist: Sphinx>=1.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/__init__.py` & `certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/_internal/dns_dnsimple.py` & `certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/_internal/dns_dnsimple.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple/_internal/tests/dns_dnsimple_test.py` & `certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple/_internal/tests/dns_dnsimple_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/PKG-INFO` & `certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-dnsimple
-Version: 2.8.0
+Version: 2.9.0
 Summary: DNSimple DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,24 +13,25 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: dns-lexicon>=3.14.1
 Requires-Dist: setuptools>=41.6.0
-Requires-Dist: acme>=2.8.0
-Requires-Dist: certbot>=2.8.0
+Requires-Dist: acme>=2.9.0
+Requires-Dist: certbot>=2.9.0
 Provides-Extra: docs
 Requires-Dist: Sphinx>=1.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `certbot-dns-dnsimple-2.8.0/certbot_dns_dnsimple.egg-info/SOURCES.txt` & `certbot-dns-dnsimple-2.9.0/certbot_dns_dnsimple.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/docs/Makefile` & `certbot-dns-dnsimple-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/docs/conf.py` & `certbot-dns-dnsimple-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/docs/index.rst` & `certbot-dns-dnsimple-2.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/docs/make.bat` & `certbot-dns-dnsimple-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-dnsimple-2.8.0/setup.py` & `certbot-dns-dnsimple-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.8.0'
+version = '2.9.0'
 
 install_requires = [
     # This version of lexicon is required to address the problem described in
     # https://github.com/AnalogJ/lexicon/issues/387.
     'dns-lexicon>=3.14.1',
     'setuptools>=41.6.0',
 ]
@@ -50,14 +50,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Security',
         'Topic :: System :: Installation/Setup',
         'Topic :: System :: Networking',
         'Topic :: System :: Systems Administration',
         'Topic :: Utilities',
     ],
```

