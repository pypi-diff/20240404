# Comparing `tmp/ortelius-cli-9.3.266.tar.gz` & `tmp/ortelius-cli-9.3.267.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortelius-cli-9.3.266.tar", last modified: Tue Apr  2 20:42:51 2024, max compression
+gzip compressed data, was "ortelius-cli-9.3.267.tar", last modified: Thu Apr  4 16:57:21 2024, max compression
```

## Comparing `ortelius-cli-9.3.266.tar` & `ortelius-cli-9.3.267.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.229957 ortelius-cli-9.3.266/
--rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/LICENSE
--rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/MANIFEST.in
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-02 20:42:51.228391 ortelius-cli-9.3.266/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/README.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.212846 ortelius-cli-9.3.266/bin/
--rwxr-xr-x   0 steve      (502) staff       (20)    70820 2024-04-02 20:42:32.000000 ortelius-cli-9.3.266/bin/dh
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.215039 ortelius-cli-9.3.266/deployhub/
--rw-r--r--   0 steve      (502) staff       (20)       65 2024-04-02 20:42:32.000000 ortelius-cli-9.3.266/deployhub/__init__.py
--rw-r--r--   0 steve      (502) staff       (20)    71098 2024-03-21 23:53:08.000000 ortelius-cli-9.3.266/deployhub/dhapi.py
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.217553 ortelius-cli-9.3.266/doc/
--rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/doc/deployhub.md
--rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.266/doc/dh.md
-drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-02 20:42:51.223299 ortelius-cli-9.3.266/ortelius_cli.egg-info/
--rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/PKG-INFO
--rw-r--r--   0 steve      (502) staff       (20)      292 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (502) staff       (20)        1 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (502) staff       (20)       68 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/requires.txt
--rw-r--r--   0 steve      (502) staff       (20)       10 2024-04-02 20:42:51.000000 ortelius-cli-9.3.266/ortelius_cli.egg-info/top_level.txt
--rw-r--r--   0 steve      (502) staff       (20)       38 2024-04-02 20:42:51.230714 ortelius-cli-9.3.266/setup.cfg
--rw-r--r--   0 steve      (502) staff       (20)     1069 2024-04-02 20:42:32.000000 ortelius-cli-9.3.266/setup.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 16:57:21.081674 ortelius-cli-9.3.267/
+-rw-r--r--   0 steve      (502) staff       (20)    10480 2023-12-11 19:25:24.000000 ortelius-cli-9.3.267/LICENSE
+-rw-r--r--   0 steve      (502) staff       (20)       17 2023-12-11 19:25:24.000000 ortelius-cli-9.3.267/MANIFEST.in
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-04 16:57:21.080842 ortelius-cli-9.3.267/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      818 2023-12-11 19:25:24.000000 ortelius-cli-9.3.267/README.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 16:57:21.062061 ortelius-cli-9.3.267/bin/
+-rwxr-xr-x   0 steve      (502) staff       (20)    70844 2024-04-04 16:57:00.000000 ortelius-cli-9.3.267/bin/dh
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 16:57:21.065236 ortelius-cli-9.3.267/deployhub/
+-rw-r--r--   0 steve      (502) staff       (20)       65 2024-04-04 16:57:00.000000 ortelius-cli-9.3.267/deployhub/__init__.py
+-rw-r--r--   0 steve      (502) staff       (20)    71098 2024-03-21 23:53:08.000000 ortelius-cli-9.3.267/deployhub/dhapi.py
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 16:57:21.071834 ortelius-cli-9.3.267/doc/
+-rw-r--r--   0 steve      (502) staff       (20)    23768 2023-12-11 19:25:24.000000 ortelius-cli-9.3.267/doc/deployhub.md
+-rw-r--r--   0 steve      (502) staff       (20)    11674 2023-12-11 19:25:24.000000 ortelius-cli-9.3.267/doc/dh.md
+drwxr-xr-x   0 steve      (502) staff       (20)        0 2024-04-04 16:57:21.079714 ortelius-cli-9.3.267/ortelius_cli.egg-info/
+-rw-r--r--   0 steve      (502) staff       (20)    12461 2024-04-04 16:57:21.000000 ortelius-cli-9.3.267/ortelius_cli.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (502) staff       (20)      292 2024-04-04 16:57:21.000000 ortelius-cli-9.3.267/ortelius_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (502) staff       (20)        1 2024-04-04 16:57:21.000000 ortelius-cli-9.3.267/ortelius_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (502) staff       (20)       68 2024-04-04 16:57:21.000000 ortelius-cli-9.3.267/ortelius_cli.egg-info/requires.txt
+-rw-r--r--   0 steve      (502) staff       (20)       10 2024-04-04 16:57:21.000000 ortelius-cli-9.3.267/ortelius_cli.egg-info/top_level.txt
+-rw-r--r--   0 steve      (502) staff       (20)       38 2024-04-04 16:57:21.081982 ortelius-cli-9.3.267/setup.cfg
+-rw-r--r--   0 steve      (502) staff       (20)     1069 2024-04-04 16:57:00.000000 ortelius-cli-9.3.267/setup.py
```

### Comparing `ortelius-cli-9.3.266/LICENSE` & `ortelius-cli-9.3.267/LICENSE`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.266/PKG-INFO` & `ortelius-cli-9.3.267/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.266
+Version: 9.3.267
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.266/README.md` & `ortelius-cli-9.3.267/README.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.266/bin/dh` & `ortelius-cli-9.3.267/bin/dh`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     `--todom` To Domain
 
 """
 
 # To generate markdown use:
 # pydoc-markdown -I bin | awk '/dh.main/ {p=1}; p==0 {print}'
 
-__version__ = "9.3.266"
+__version__ = "9.3.267"
 
 import json
 import os
 import re
 import stat
 import sys
 from datetime import datetime
@@ -419,14 +419,15 @@
 
         errors = []
 
         if dhapi.is_not_empty(cert):
             dhapi.sslcerts(dhurl, cert)
 
         cookies = dhapi.login(dhurl, dhuser, dhpass, errors)
+        pprint(cookies)
 
         if cookies is None:
             if errors:
                 print(errors[0])
             sys.exit(1)
 
     if action.lower() == "deploy":
```

### Comparing `ortelius-cli-9.3.266/deployhub/dhapi.py` & `ortelius-cli-9.3.267/deployhub/dhapi.py`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.266/doc/deployhub.md` & `ortelius-cli-9.3.267/doc/deployhub.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.266/doc/dh.md` & `ortelius-cli-9.3.267/doc/dh.md`

 * *Files identical despite different names*

### Comparing `ortelius-cli-9.3.266/ortelius_cli.egg-info/PKG-INFO` & `ortelius-cli-9.3.267/ortelius_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortelius-cli
-Version: 9.3.266
+Version: 9.3.267
 Home-page: https://ortelius.io
 Author: Steve Taylor
 Author-email: steve@deployhub.com
 License: Apache-2.0
 Project-URL: Project Repo, https://github.com/ortelius/ortelius-cli
 Project-URL: Issues, https://github.com/ortelius/ortelius/issues
 Project-URL: Ortelius CLI Documentation, https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md
```

### Comparing `ortelius-cli-9.3.266/setup.py` & `ortelius-cli-9.3.267/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "Issues": "https://github.com/ortelius/ortelius/issues",
         "Ortelius CLI Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/dh.md",
         "Python Python API Documentation": "https://github.com/ortelius/ortelius-cli/blob/main/doc/deployhub.md",
     },
     author="Steve Taylor",
     author_email="steve@deployhub.com",
     name="ortelius-cli",
-    version="9.3.266",
+    version="9.3.267",
     packages=[
         "deployhub",
     ],
     scripts=["bin/dh"],
     license="Apache-2.0",
     long_description=open("doc/dh.md").read(),
     long_description_content_type="text/markdown",
```

