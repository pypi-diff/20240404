# Comparing `tmp/certbot-dns-cloudflare-2.8.0.tar.gz` & `tmp/certbot-dns-cloudflare-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-cloudflare-2.8.0.tar", last modified: Tue Dec  5 19:14:00 2023, max compression
+gzip compressed data, was "certbot-dns-cloudflare-2.9.0.tar", last modified: Thu Feb  8 19:45:27 2024, max compression
```

## Comparing `certbot-dns-cloudflare-2.8.0.tar` & `certbot-dns-cloudflare-2.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:00.267160 certbot-dns-cloudflare-2.8.0/
--rw-rw-r--   0 willg     (1000) willg     (1000)    10786 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/LICENSE.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      156 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/MANIFEST.in
--rw-r--r--   0 willg     (1000) willg     (1000)     1400 2023-12-05 19:14:00.267160 certbot-dns-cloudflare-2.8.0/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)       48 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/README.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:00.267160 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/
--rw-rw-r--   0 willg     (1000) willg     (1000)     5309 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/__init__.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:00.267160 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/_internal/
--rw-rw-r--   0 willg     (1000) willg     (1000)       82 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/_internal/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    12911 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/_internal/dns_cloudflare.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:00.267160 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/_internal/tests/
--rw-rw-r--   0 willg     (1000) willg     (1000)       35 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/_internal/tests/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9767 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/_internal/tests/dns_cloudflare_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/py.typed
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:00.267160 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/
--rw-r--r--   0 willg     (1000) willg     (1000)     1400 2023-12-05 19:14:00.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)      682 2023-12-05 19:14:00.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/SOURCES.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        1 2023-12-05 19:14:00.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/dependency_links.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       97 2023-12-05 19:14:00.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/entry_points.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      116 2023-12-05 19:14:00.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/requires.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       23 2023-12-05 19:14:00.000000 certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/top_level.txt
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:14:00.267160 certbot-dns-cloudflare-2.8.0/docs/
--rw-rw-r--   0 willg     (1000) willg     (1000)        9 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/docs/.gitignore
--rw-rw-r--   0 willg     (1000) willg     (1000)      620 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/docs/Makefile
--rw-rw-r--   0 willg     (1000) willg     (1000)      149 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/docs/api.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     5419 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/docs/conf.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      572 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/docs/index.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      831 2023-12-05 19:13:52.000000 certbot-dns-cloudflare-2.8.0/docs/make.bat
--rw-rw-r--   0 willg     (1000) willg     (1000)       38 2023-12-05 19:14:00.267160 certbot-dns-cloudflare-2.8.0/setup.cfg
--rw-rw-r--   0 willg     (1000) willg     (1000)     2169 2023-12-05 19:13:53.000000 certbot-dns-cloudflare-2.8.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:27.811123 certbot-dns-cloudflare-2.9.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      156 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/MANIFEST.in
+-rw-r--r--   0 erica     (1001) erica     (1001)     1451 2024-02-08 19:45:27.811123 certbot-dns-cloudflare-2.9.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       48 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:27.811123 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5309 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:27.811123 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       82 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    12911 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/_internal/dns_cloudflare.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:27.811123 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       35 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9767 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/_internal/tests/dns_cloudflare_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:27.811123 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/
+-rw-r--r--   0 erica     (1001) erica     (1001)     1451 2024-02-08 19:45:27.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)      682 2024-02-08 19:45:27.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2024-02-08 19:45:27.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       97 2024-02-08 19:45:27.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      116 2024-02-08 19:45:27.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       23 2024-02-08 19:45:27.000000 certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:27.811123 certbot-dns-cloudflare-2.9.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)      620 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/docs/Makefile
+-rw-rw-r--   0 erica     (1001) erica     (1001)      149 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5419 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      572 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      831 2024-02-08 19:45:17.000000 certbot-dns-cloudflare-2.9.0/docs/make.bat
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2024-02-08 19:45:27.811123 certbot-dns-cloudflare-2.9.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2219 2024-02-08 19:45:18.000000 certbot-dns-cloudflare-2.9.0/setup.py
```

### Comparing `certbot-dns-cloudflare-2.8.0/LICENSE.txt` & `certbot-dns-cloudflare-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/PKG-INFO` & `certbot-dns-cloudflare-2.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-cloudflare
-Version: 2.8.0
+Version: 2.9.0
 Summary: Cloudflare DNS Authenticator plugin for Certbot
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
 Requires-Dist: cloudflare>=1.5.1
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

### Comparing `certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/__init__.py` & `certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/_internal/dns_cloudflare.py` & `certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/_internal/dns_cloudflare.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare/_internal/tests/dns_cloudflare_test.py` & `certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare/_internal/tests/dns_cloudflare_test.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/PKG-INFO` & `certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-cloudflare
-Version: 2.8.0
+Version: 2.9.0
 Summary: Cloudflare DNS Authenticator plugin for Certbot
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
 Requires-Dist: cloudflare>=1.5.1
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

### Comparing `certbot-dns-cloudflare-2.8.0/certbot_dns_cloudflare.egg-info/SOURCES.txt` & `certbot-dns-cloudflare-2.9.0/certbot_dns_cloudflare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/docs/Makefile` & `certbot-dns-cloudflare-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/docs/conf.py` & `certbot-dns-cloudflare-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/docs/index.rst` & `certbot-dns-cloudflare-2.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/docs/make.bat` & `certbot-dns-cloudflare-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-cloudflare-2.8.0/setup.py` & `certbot-dns-cloudflare-2.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.8.0'
+version = '2.9.0'
 
 install_requires = [
     'cloudflare>=1.5.1',
     'setuptools>=41.6.0',
 ]
 
 if os.environ.get('SNAP_BUILD'):
@@ -48,14 +48,15 @@
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

