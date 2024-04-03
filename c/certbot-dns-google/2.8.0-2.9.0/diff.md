# Comparing `tmp/certbot-dns-google-2.8.0.tar.gz` & `tmp/certbot-dns-google-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-google-2.8.0.tar", last modified: Tue Dec  5 19:14:07 2023, max compression
+gzip compressed data, was "certbot-dns-google-2.9.0.tar", last modified: Thu Feb  8 19:45:34 2024, max compression
```

## Comparing `certbot-dns-google-2.8.0.tar` & `certbot-dns-google-2.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:07.159063 certbot-dns-google-2.8.0/
--rw-rw-r--   0 willg     (1000) willg     (1000)    10786 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/LICENSE.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      216 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/MANIFEST.in
--rw-r--r--   0 willg     (1000) willg     (1000)     1447 2023-12-05 19:14:07.155063 certbot-dns-google-2.8.0/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)       50 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/README.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:07.155063 certbot-dns-google-2.8.0/certbot_dns_google/
--rw-rw-r--   0 willg     (1000) willg     (1000)    10225 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/certbot_dns_google/__init__.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:07.155063 certbot-dns-google-2.8.0/certbot_dns_google/_internal/
--rw-rw-r--   0 willg     (1000) willg     (1000)       74 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/certbot_dns_google/_internal/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    13419 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/certbot_dns_google/_internal/dns_google.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:07.155063 certbot-dns-google-2.8.0/certbot_dns_google/_internal/tests/
--rw-rw-r--   0 willg     (1000) willg     (1000)       31 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/certbot_dns_google/_internal/tests/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    24511 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/certbot_dns_google/_internal/tests/dns_google_test.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:07.155063 certbot-dns-google-2.8.0/certbot_dns_google/_internal/tests/testdata/
--rw-rw-r--   0 willg     (1000) willg     (1000)    47820 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/certbot_dns_google/_internal/tests/testdata/discovery.json
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/certbot_dns_google/py.typed
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:07.155063 certbot-dns-google-2.8.0/certbot_dns_google.egg-info/
--rw-r--r--   0 willg     (1000) willg     (1000)     1447 2023-12-05 19:14:07.000000 certbot-dns-google-2.8.0/certbot_dns_google.egg-info/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)      685 2023-12-05 19:14:07.000000 certbot-dns-google-2.8.0/certbot_dns_google.egg-info/SOURCES.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        1 2023-12-05 19:14:07.000000 certbot-dns-google-2.8.0/certbot_dns_google.egg-info/dependency_links.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       85 2023-12-05 19:14:07.000000 certbot-dns-google-2.8.0/certbot_dns_google.egg-info/entry_points.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      150 2023-12-05 19:14:07.000000 certbot-dns-google-2.8.0/certbot_dns_google.egg-info/requires.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       19 2023-12-05 19:14:07.000000 certbot-dns-google-2.8.0/certbot_dns_google.egg-info/top_level.txt
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:07.155063 certbot-dns-google-2.8.0/docs/
--rw-rw-r--   0 willg     (1000) willg     (1000)        9 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/docs/.gitignore
--rw-rw-r--   0 willg     (1000) willg     (1000)      615 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/docs/Makefile
--rw-rw-r--   0 willg     (1000) willg     (1000)      149 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/docs/api.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     5376 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/docs/conf.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      557 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/docs/index.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      827 2023-12-05 19:13:52.000000 certbot-dns-google-2.8.0/docs/make.bat
--rw-rw-r--   0 willg     (1000) willg     (1000)       38 2023-12-05 19:14:07.159063 certbot-dns-google-2.8.0/setup.cfg
--rw-rw-r--   0 willg     (1000) willg     (1000)     2196 2023-12-05 19:13:53.000000 certbot-dns-google-2.8.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:34.975153 certbot-dns-google-2.9.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      216 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/MANIFEST.in
+-rw-r--r--   0 erica     (1001) erica     (1001)     1498 2024-02-08 19:45:34.975153 certbot-dns-google-2.9.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       50 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:34.971153 certbot-dns-google-2.9.0/certbot_dns_google/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10225 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/certbot_dns_google/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:34.975153 certbot-dns-google-2.9.0/certbot_dns_google/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       74 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/certbot_dns_google/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13419 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/certbot_dns_google/_internal/dns_google.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:34.975153 certbot-dns-google-2.9.0/certbot_dns_google/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       31 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/certbot_dns_google/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    24511 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/certbot_dns_google/_internal/tests/dns_google_test.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:34.975153 certbot-dns-google-2.9.0/certbot_dns_google/_internal/tests/testdata/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    47820 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/certbot_dns_google/_internal/tests/testdata/discovery.json
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/certbot_dns_google/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:34.975153 certbot-dns-google-2.9.0/certbot_dns_google.egg-info/
+-rw-r--r--   0 erica     (1001) erica     (1001)     1498 2024-02-08 19:45:34.000000 certbot-dns-google-2.9.0/certbot_dns_google.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      685 2024-02-08 19:45:34.000000 certbot-dns-google-2.9.0/certbot_dns_google.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2024-02-08 19:45:34.000000 certbot-dns-google-2.9.0/certbot_dns_google.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       85 2024-02-08 19:45:34.000000 certbot-dns-google-2.9.0/certbot_dns_google.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      150 2024-02-08 19:45:34.000000 certbot-dns-google-2.9.0/certbot_dns_google.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       19 2024-02-08 19:45:34.000000 certbot-dns-google-2.9.0/certbot_dns_google.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:34.975153 certbot-dns-google-2.9.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      615 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5376 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      557 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      827 2024-02-08 19:45:17.000000 certbot-dns-google-2.9.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2024-02-08 19:45:34.975153 certbot-dns-google-2.9.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2246 2024-02-08 19:45:18.000000 certbot-dns-google-2.9.0/setup.py
```

### Comparing `certbot-dns-google-2.8.0/LICENSE.txt` & `certbot-dns-google-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/PKG-INFO` & `certbot-dns-google-2.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-google
-Version: 2.8.0
+Version: 2.9.0
 Summary: Google Cloud DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,25 +13,26 @@
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
 Requires-Dist: google-api-python-client>=1.6.5
 Requires-Dist: google-auth>=2.16.0
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

### Comparing `certbot-dns-google-2.8.0/certbot_dns_google/__init__.py` & `certbot-dns-google-2.9.0/certbot_dns_google/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/certbot_dns_google/_internal/dns_google.py` & `certbot-dns-google-2.9.0/certbot_dns_google/_internal/dns_google.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/certbot_dns_google/_internal/tests/dns_google_test.py` & `certbot-dns-google-2.9.0/certbot_dns_google/_internal/tests/dns_google_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/certbot_dns_google/_internal/tests/testdata/discovery.json` & `certbot-dns-google-2.9.0/certbot_dns_google/_internal/tests/testdata/discovery.json`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/certbot_dns_google.egg-info/PKG-INFO` & `certbot-dns-google-2.9.0/certbot_dns_google.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-google
-Version: 2.8.0
+Version: 2.9.0
 Summary: Google Cloud DNS Authenticator plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,25 +13,26 @@
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
 Requires-Dist: google-api-python-client>=1.6.5
 Requires-Dist: google-auth>=2.16.0
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

### Comparing `certbot-dns-google-2.8.0/certbot_dns_google.egg-info/SOURCES.txt` & `certbot-dns-google-2.9.0/certbot_dns_google.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/docs/Makefile` & `certbot-dns-google-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/docs/conf.py` & `certbot-dns-google-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/docs/index.rst` & `certbot-dns-google-2.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/docs/make.bat` & `certbot-dns-google-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-google-2.8.0/setup.py` & `certbot-dns-google-2.9.0/setup.py`

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
     'google-api-python-client>=1.6.5',
     'google-auth>=2.16.0',
     'setuptools>=41.6.0',
 ]
 
@@ -49,14 +49,15 @@
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

