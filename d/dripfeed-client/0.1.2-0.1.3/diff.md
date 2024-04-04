# Comparing `tmp/dripfeed-client-0.1.2.tar.gz` & `tmp/dripfeed-client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dripfeed-client-0.1.2.tar", last modified: Wed Apr  3 18:51:18 2024, max compression
+gzip compressed data, was "dripfeed-client-0.1.3.tar", last modified: Thu Apr  4 06:38:49 2024, max compression
```

## Comparing `dripfeed-client-0.1.2.tar` & `dripfeed-client-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-03 18:51:18.042277 dripfeed-client-0.1.2/
--rw-r--r--   0 g          (501) staff       (20)     1071 2024-03-30 08:09:04.000000 dripfeed-client-0.1.2/LICENSE
--rw-r--r--   0 g          (501) staff       (20)      755 2024-04-03 18:51:18.042080 dripfeed-client-0.1.2/PKG-INFO
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-03 18:51:18.041177 dripfeed-client-0.1.2/dripfeed/
--rw-r--r--   0 g          (501) staff       (20)       46 2024-04-03 18:48:52.000000 dripfeed-client-0.1.2/dripfeed/__init__.py
--rw-r--r--   0 g          (501) staff       (20)     1923 2024-03-30 08:36:20.000000 dripfeed-client-0.1.2/dripfeed/api.py
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-03 18:51:18.041837 dripfeed-client-0.1.2/dripfeed_client.egg-info/
--rw-r--r--   0 g          (501) staff       (20)      755 2024-04-03 18:51:17.000000 dripfeed-client-0.1.2/dripfeed_client.egg-info/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)      247 2024-04-03 18:51:18.000000 dripfeed-client-0.1.2/dripfeed_client.egg-info/SOURCES.txt
--rw-r--r--   0 g          (501) staff       (20)        1 2024-04-03 18:51:17.000000 dripfeed-client-0.1.2/dripfeed_client.egg-info/dependency_links.txt
--rw-r--r--   0 g          (501) staff       (20)        9 2024-04-03 18:51:17.000000 dripfeed-client-0.1.2/dripfeed_client.egg-info/requires.txt
--rw-r--r--   0 g          (501) staff       (20)        9 2024-04-03 18:51:17.000000 dripfeed-client-0.1.2/dripfeed_client.egg-info/top_level.txt
--rw-r--r--   0 g          (501) staff       (20)       38 2024-04-03 18:51:18.042315 dripfeed-client-0.1.2/setup.cfg
--rw-r--r--   0 g          (501) staff       (20)      953 2024-04-03 18:50:22.000000 dripfeed-client-0.1.2/setup.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-04 06:38:49.378496 dripfeed-client-0.1.3/
+-rw-r--r--   0 g          (501) staff       (20)     1071 2024-03-30 08:09:04.000000 dripfeed-client-0.1.3/LICENSE
+-rw-r--r--   0 g          (501) staff       (20)      755 2024-04-04 06:38:49.378154 dripfeed-client-0.1.3/PKG-INFO
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-04 06:38:49.377215 dripfeed-client-0.1.3/dripfeed/
+-rw-r--r--   0 g          (501) staff       (20)       46 2024-04-04 06:25:16.000000 dripfeed-client-0.1.3/dripfeed/__init__.py
+-rw-r--r--   0 g          (501) staff       (20)     3492 2024-04-04 06:32:30.000000 dripfeed-client-0.1.3/dripfeed/api.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-04 06:38:49.377929 dripfeed-client-0.1.3/dripfeed_client.egg-info/
+-rw-r--r--   0 g          (501) staff       (20)      755 2024-04-04 06:38:49.000000 dripfeed-client-0.1.3/dripfeed_client.egg-info/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)      247 2024-04-04 06:38:49.000000 dripfeed-client-0.1.3/dripfeed_client.egg-info/SOURCES.txt
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-04-04 06:38:49.000000 dripfeed-client-0.1.3/dripfeed_client.egg-info/dependency_links.txt
+-rw-r--r--   0 g          (501) staff       (20)        9 2024-04-04 06:38:49.000000 dripfeed-client-0.1.3/dripfeed_client.egg-info/requires.txt
+-rw-r--r--   0 g          (501) staff       (20)        9 2024-04-04 06:38:49.000000 dripfeed-client-0.1.3/dripfeed_client.egg-info/top_level.txt
+-rw-r--r--   0 g          (501) staff       (20)       38 2024-04-04 06:38:49.378547 dripfeed-client-0.1.3/setup.cfg
+-rw-r--r--   0 g          (501) staff       (20)      953 2024-04-04 06:36:09.000000 dripfeed-client-0.1.3/setup.py
```

### Comparing `dripfeed-client-0.1.2/LICENSE` & `dripfeed-client-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dripfeed-client-0.1.2/PKG-INFO` & `dripfeed-client-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dripfeed-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A client for the dripfeed RSS proxy service.
 Home-page: https://github.com/xurble/python-dripfeed-client
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dripfeed-client-0.1.2/dripfeed_client.egg-info/PKG-INFO` & `dripfeed-client-0.1.3/dripfeed_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dripfeed-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A client for the dripfeed RSS proxy service.
 Home-page: https://github.com/xurble/python-dripfeed-client
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dripfeed-client-0.1.2/setup.py` & `dripfeed-client-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='dripfeed-client',
-    version='0.1.2',
+    version='0.1.3',
     description='A client for the dripfeed RSS proxy service.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Gareth Simpson',
     author_email='g@xurble.org',
     url='https://github.com/xurble/python-dripfeed-client',
     license='MIT',
```

