# Comparing `tmp/compteur-0.2.tar.gz` & `tmp/compteur-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compteur-0.2.tar", last modified: Thu Apr  4 14:10:42 2024, max compression
+gzip compressed data, was "compteur-0.3.tar", last modified: Thu Apr  4 20:49:27 2024, max compression
```

## Comparing `compteur-0.2.tar` & `compteur-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:10:42.299440 compteur-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 14:10:38.000000 compteur-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 14:10:42.299440 compteur-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-04 14:10:38.000000 compteur-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:10:42.299440 compteur-0.2/compteur/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:10:38.000000 compteur-0.2/compteur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-04 14:10:38.000000 compteur-0.2/compteur/compteur.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:10:42.299440 compteur-0.2/compteur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 14:10:42.000000 compteur-0.2/compteur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 14:10:42.000000 compteur-0.2/compteur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:10:42.000000 compteur-0.2/compteur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 14:10:42.000000 compteur-0.2/compteur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 14:10:42.299440 compteur-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-04 14:10:38.000000 compteur-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:49:27.427424 compteur-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 20:49:23.000000 compteur-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 20:49:27.427424 compteur-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-04 20:49:23.000000 compteur-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:49:27.427424 compteur-0.3/compteur/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 20:49:23.000000 compteur-0.3/compteur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-04 20:49:23.000000 compteur-0.3/compteur/compteur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 20:49:27.427424 compteur-0.3/compteur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 20:49:27.000000 compteur-0.3/compteur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 20:49:27.000000 compteur-0.3/compteur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 20:49:27.000000 compteur-0.3/compteur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 20:49:27.000000 compteur-0.3/compteur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 20:49:27.427424 compteur-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-04 20:49:23.000000 compteur-0.3/setup.py
```

### Comparing `compteur-0.2/LICENSE` & `compteur-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `compteur-0.2/PKG-INFO` & `compteur-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: compteur
-Version: 0.2
+Version: 0.3
 Summary: Count how many time errors occur
 Home-page: https://github.com/OlivierProTips/compteur
-Author: OlivireProTips
+Author: OlivierProTips
 Author-email: olivierprotips@gmail.com
 License: MIT
 Keywords: Compteur,error,count,track
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `compteur-0.2/README.md` & `compteur-0.3/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     cpt.inc()
     if cpt.isLimit():
         raise
 else:
     cpt.reset()
 finally:
     # do something
-```
+```
```

### Comparing `compteur-0.2/compteur.egg-info/PKG-INFO` & `compteur-0.3/compteur.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: compteur
-Version: 0.2
+Version: 0.3
 Summary: Count how many time errors occur
 Home-page: https://github.com/OlivierProTips/compteur
-Author: OlivireProTips
+Author: OlivierProTips
 Author-email: olivierprotips@gmail.com
 License: MIT
 Keywords: Compteur,error,count,track
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `compteur-0.2/setup.py` & `compteur-0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setup(
   name = 'compteur',
   packages = ['compteur'],
-  version = '0.2',
+  version = '0.3',
   license='MIT',
   description = 'Count how many time errors occur',
   long_description = long_description,
   long_description_content_type = "text/markdown",
-  author = 'OlivireProTips',
+  author = 'OlivierProTips',
   author_email = 'olivierprotips@gmail.com',
   url = 'https://github.com/OlivierProTips/compteur',
   keywords = ['Compteur', 'error', 'count', 'track'],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

