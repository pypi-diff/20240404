# Comparing `tmp/Compteur-0.1.tar.gz` & `tmp/compteur-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Compteur-0.1.tar", last modified: Thu Apr  4 11:44:35 2024, max compression
+gzip compressed data, was "compteur-0.2.tar", last modified: Thu Apr  4 14:10:42 2024, max compression
```

## Comparing `Compteur-0.1.tar` & `compteur-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:35.535131 Compteur-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:35.535131 Compteur-0.1/Compteur/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-04 11:44:31.000000 Compteur-0.1/Compteur/Compteur.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 11:44:31.000000 Compteur-0.1/Compteur/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:44:35.535131 Compteur-0.1/Compteur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-04 11:44:35.000000 Compteur-0.1/Compteur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 11:44:35.000000 Compteur-0.1/Compteur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:44:35.000000 Compteur-0.1/Compteur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 11:44:35.000000 Compteur-0.1/Compteur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 11:44:31.000000 Compteur-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-04 11:44:35.535131 Compteur-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-04 11:44:31.000000 Compteur-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 11:44:35.535131 Compteur-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-04 11:44:31.000000 Compteur-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:10:42.299440 compteur-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-04 14:10:38.000000 compteur-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 14:10:42.299440 compteur-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-04 14:10:38.000000 compteur-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:10:42.299440 compteur-0.2/compteur/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 14:10:38.000000 compteur-0.2/compteur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-04 14:10:38.000000 compteur-0.2/compteur/compteur.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:10:42.299440 compteur-0.2/compteur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 14:10:42.000000 compteur-0.2/compteur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-04 14:10:42.000000 compteur-0.2/compteur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:10:42.000000 compteur-0.2/compteur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 14:10:42.000000 compteur-0.2/compteur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-04 14:10:42.299440 compteur-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-04 14:10:38.000000 compteur-0.2/setup.py
```

### Comparing `Compteur-0.1/Compteur/Compteur.py` & `compteur-0.2/compteur/compteur.py`

 * *Files identical despite different names*

### Comparing `Compteur-0.1/Compteur.egg-info/PKG-INFO` & `compteur-0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
-Name: Compteur
-Version: 0.1
+Name: compteur
+Version: 0.2
 Summary: Count how many time errors occur
-Home-page: https://github.com/OlivierProTips/Compteur
-Download-URL: https://github.com/OlivierProTips/Compteur/archive/refs/tags/v0.1.tar.gz
+Home-page: https://github.com/OlivierProTips/compteur
 Author: OlivireProTips
 Author-email: olivierprotips@gmail.com
 License: MIT
 Keywords: Compteur,error,count,track
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -26,17 +25,17 @@
 
 Goal of this package is to track how many times an error occurs. I can define a limit of # errors before warning me.
 
 ## Exemple
 
 ```python
 #!/usr/bin/env python3
-from Compteur import Compteur
+from compteur import Compteur
 
-cpt = Compteur('htb')
+cpt = Compteur('smartname')
 
 try:
     # My wonderful script
 except:
     cpt.inc()
     if cpt.isLimit():
         raise
```

### Comparing `Compteur-0.1/LICENSE` & `compteur-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Compteur-0.1/PKG-INFO` & `compteur-0.2/compteur.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
-Name: Compteur
-Version: 0.1
+Name: compteur
+Version: 0.2
 Summary: Count how many time errors occur
-Home-page: https://github.com/OlivierProTips/Compteur
-Download-URL: https://github.com/OlivierProTips/Compteur/archive/refs/tags/v0.1.tar.gz
+Home-page: https://github.com/OlivierProTips/compteur
 Author: OlivireProTips
 Author-email: olivierprotips@gmail.com
 License: MIT
 Keywords: Compteur,error,count,track
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -26,17 +25,17 @@
 
 Goal of this package is to track how many times an error occurs. I can define a limit of # errors before warning me.
 
 ## Exemple
 
 ```python
 #!/usr/bin/env python3
-from Compteur import Compteur
+from compteur import Compteur
 
-cpt = Compteur('htb')
+cpt = Compteur('smartname')
 
 try:
     # My wonderful script
 except:
     cpt.inc()
     if cpt.isLimit():
         raise
```

### Comparing `Compteur-0.1/README.md` & `compteur-0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 Goal of this package is to track how many times an error occurs. I can define a limit of # errors before warning me.
 
 ## Exemple
 
 ```python
 #!/usr/bin/env python3
-from Compteur import Compteur
+from compteur import Compteur
 
-cpt = Compteur('htb')
+cpt = Compteur('smartname')
 
 try:
     # My wonderful script
 except:
     cpt.inc()
     if cpt.isLimit():
         raise
```

### Comparing `Compteur-0.1/setup.py` & `compteur-0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from distutils.core import setup
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
-    
+
 setup(
-  name = 'Compteur',
-  packages = ['Compteur'],
-  version = '0.1',
+  name = 'compteur',
+  packages = ['compteur'],
+  version = '0.2',
   license='MIT',
   description = 'Count how many time errors occur',
-    long_description = long_description,
-    long_description_content_type = "text/markdown",
+  long_description = long_description,
+  long_description_content_type = "text/markdown",
   author = 'OlivireProTips',
   author_email = 'olivierprotips@gmail.com',
-  url = 'https://github.com/OlivierProTips/Compteur',
-  download_url = 'https://github.com/OlivierProTips/Compteur/archive/refs/tags/v0.1.tar.gz',
+  url = 'https://github.com/OlivierProTips/compteur',
   keywords = ['Compteur', 'error', 'count', 'track'],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```

