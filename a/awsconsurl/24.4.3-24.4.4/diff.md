# Comparing `tmp/awsconsurl-24.4.3.tar.gz` & `tmp/awsconsurl-24.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsconsurl-24.4.3.tar", last modified: Thu Apr  4 01:54:49 2024, max compression
+gzip compressed data, was "awsconsurl-24.4.4.tar", last modified: Thu Apr  4 02:26:13 2024, max compression
```

## Comparing `awsconsurl-24.4.3.tar` & `awsconsurl-24.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 01:54:49.878612 awsconsurl-24.4.3/
--rw-r--r--   0 rkras    (872432560) staff       (20)     1067 2021-08-19 00:37:30.000000 awsconsurl-24.4.3/LICENSE.txt
--rw-r--r--   0 rkras    (872432560) staff       (20)       94 2021-08-19 00:37:30.000000 awsconsurl-24.4.3/MANIFEST.in
--rw-r--r--   0 rkras    (872432560) staff       (20)     6121 2024-04-04 01:54:49.878298 awsconsurl-24.4.3/PKG-INFO
--rw-r--r--   0 rkras    (872432560) staff       (20)     5420 2021-08-19 00:37:30.000000 awsconsurl-24.4.3/README.md
--rw-r--r--   0 rkras    (872432560) staff       (20)      104 2021-08-19 00:37:30.000000 awsconsurl-24.4.3/pyproject.toml
--rw-r--r--   0 rkras    (872432560) staff       (20)       31 2021-08-19 00:37:30.000000 awsconsurl-24.4.3/requirements.txt
-drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 01:54:49.871592 awsconsurl-24.4.3/scripts/
--rwxr-xr-x   0 rkras    (872432560) staff       (20)      133 2021-08-19 00:37:30.000000 awsconsurl-24.4.3/scripts/consurl
--rw-r--r--   0 rkras    (872432560) staff       (20)      901 2024-04-04 01:54:49.880483 awsconsurl-24.4.3/setup.cfg
-drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 01:54:49.868457 awsconsurl-24.4.3/src/
-drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 01:54:49.872862 awsconsurl-24.4.3/src/awsconsurl/
--rw-r--r--   0 rkras    (872432560) staff       (20)       28 2021-08-19 00:37:30.000000 awsconsurl-24.4.3/src/awsconsurl/__init__.py
--rwxr-xr-x   0 rkras    (872432560) staff       (20)     7374 2024-04-04 01:45:45.000000 awsconsurl-24.4.3/src/awsconsurl/consurl.py
-drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 01:54:49.877335 awsconsurl-24.4.3/src/awsconsurl.egg-info/
--rw-r--r--   0 rkras    (872432560) staff       (20)     6121 2024-04-04 01:54:49.000000 awsconsurl-24.4.3/src/awsconsurl.egg-info/PKG-INFO
--rw-r--r--   0 rkras    (872432560) staff       (20)      333 2024-04-04 01:54:49.000000 awsconsurl-24.4.3/src/awsconsurl.egg-info/SOURCES.txt
--rw-r--r--   0 rkras    (872432560) staff       (20)        1 2024-04-04 01:54:49.000000 awsconsurl-24.4.3/src/awsconsurl.egg-info/dependency_links.txt
--rw-r--r--   0 rkras    (872432560) staff       (20)       31 2024-04-04 01:54:49.000000 awsconsurl-24.4.3/src/awsconsurl.egg-info/requires.txt
--rw-r--r--   0 rkras    (872432560) staff       (20)       11 2024-04-04 01:54:49.000000 awsconsurl-24.4.3/src/awsconsurl.egg-info/top_level.txt
+drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 02:26:13.688660 awsconsurl-24.4.4/
+-rw-r--r--   0 rkras    (872432560) staff       (20)     1067 2021-08-19 00:37:30.000000 awsconsurl-24.4.4/LICENSE.txt
+-rw-r--r--   0 rkras    (872432560) staff       (20)       94 2021-08-19 00:37:30.000000 awsconsurl-24.4.4/MANIFEST.in
+-rw-r--r--   0 rkras    (872432560) staff       (20)     6121 2024-04-04 02:26:13.688437 awsconsurl-24.4.4/PKG-INFO
+-rw-r--r--   0 rkras    (872432560) staff       (20)     5420 2021-08-19 00:37:30.000000 awsconsurl-24.4.4/README.md
+-rw-r--r--   0 rkras    (872432560) staff       (20)      104 2021-08-19 00:37:30.000000 awsconsurl-24.4.4/pyproject.toml
+-rw-r--r--   0 rkras    (872432560) staff       (20)       31 2021-08-19 00:37:30.000000 awsconsurl-24.4.4/requirements.txt
+drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 02:26:13.683363 awsconsurl-24.4.4/scripts/
+-rwxr-xr-x   0 rkras    (872432560) staff       (20)      133 2021-08-19 00:37:30.000000 awsconsurl-24.4.4/scripts/consurl
+-rw-r--r--   0 rkras    (872432560) staff       (20)      901 2024-04-04 02:26:13.689648 awsconsurl-24.4.4/setup.cfg
+drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 02:26:13.680439 awsconsurl-24.4.4/src/
+drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 02:26:13.684343 awsconsurl-24.4.4/src/awsconsurl/
+-rw-r--r--   0 rkras    (872432560) staff       (20)       28 2021-08-19 00:37:30.000000 awsconsurl-24.4.4/src/awsconsurl/__init__.py
+-rwxr-xr-x   0 rkras    (872432560) staff       (20)     7403 2024-04-04 02:21:50.000000 awsconsurl-24.4.4/src/awsconsurl/consurl.py
+drwxr-xr-x   0 rkras    (872432560) staff       (20)        0 2024-04-04 02:26:13.687696 awsconsurl-24.4.4/src/awsconsurl.egg-info/
+-rw-r--r--   0 rkras    (872432560) staff       (20)     6121 2024-04-04 02:26:13.000000 awsconsurl-24.4.4/src/awsconsurl.egg-info/PKG-INFO
+-rw-r--r--   0 rkras    (872432560) staff       (20)      333 2024-04-04 02:26:13.000000 awsconsurl-24.4.4/src/awsconsurl.egg-info/SOURCES.txt
+-rw-r--r--   0 rkras    (872432560) staff       (20)        1 2024-04-04 02:26:13.000000 awsconsurl-24.4.4/src/awsconsurl.egg-info/dependency_links.txt
+-rw-r--r--   0 rkras    (872432560) staff       (20)       31 2024-04-04 02:26:13.000000 awsconsurl-24.4.4/src/awsconsurl.egg-info/requires.txt
+-rw-r--r--   0 rkras    (872432560) staff       (20)       11 2024-04-04 02:26:13.000000 awsconsurl-24.4.4/src/awsconsurl.egg-info/top_level.txt
```

### Comparing `awsconsurl-24.4.3/LICENSE.txt` & `awsconsurl-24.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `awsconsurl-24.4.3/PKG-INFO` & `awsconsurl-24.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsconsurl
-Version: 24.4.3
+Version: 24.4.4
 Summary: Creates and Opens an AWS console login URL in a Browser
 Home-page: https://github.com/Glocktober/consurl
 Author: gunville
 Author-email: rk13088@yahoo.com
 Project-URL: repo, https://github.com/Glocktober/consurl
 Project-URL: overview, https://github.com/Glocktober/consurl/blob/main/README.md
 Keywords: 'aws'
```

### Comparing `awsconsurl-24.4.3/README.md` & `awsconsurl-24.4.4/README.md`

 * *Files identical despite different names*

### Comparing `awsconsurl-24.4.3/setup.cfg` & `awsconsurl-24.4.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = awsconsurl
-version = 24.04.03
+version = 24.04.04
 author = gunville
 author_email = rk13088@yahoo.com
 description = Creates and Opens an AWS console login URL in a Browser
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE.txt
 url = https://github.com/Glocktober/consurl
```

### Comparing `awsconsurl-24.4.3/src/awsconsurl/consurl.py` & `awsconsurl-24.4.4/src/awsconsurl/consurl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-copyright = 'copyright 2021 r.kras'
+copyright = 'copyright 2024 r.kras'
 import argparse
 import json
 import os
 import socket
 import sys
 from urllib.parse import urlencode
 import webbrowser
@@ -201,16 +201,15 @@
         return sin_url
     else:
         vprint(f'Opening webbrowser for {sin_url}')
         webbrowser.open(sin_url)
         return None
 
 
-if __name__ == '__main__':
-
+def consurl():
     args = arg_parse()
     if args.verbose:
         verbose = True
         vprint('verbose mode enabled')
     
     if args.version:
         print(version_info, file=sys.stdout)
@@ -221,7 +220,10 @@
                 print(url, file=sys.stdout)
 
         except Exception as e:
             if verbose:
                 raise e
             eprint(e)
 
+
+if __name__ == '__main__':
+    consurl()
```

### Comparing `awsconsurl-24.4.3/src/awsconsurl.egg-info/PKG-INFO` & `awsconsurl-24.4.4/src/awsconsurl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsconsurl
-Version: 24.4.3
+Version: 24.4.4
 Summary: Creates and Opens an AWS console login URL in a Browser
 Home-page: https://github.com/Glocktober/consurl
 Author: gunville
 Author-email: rk13088@yahoo.com
 Project-URL: repo, https://github.com/Glocktober/consurl
 Project-URL: overview, https://github.com/Glocktober/consurl/blob/main/README.md
 Keywords: 'aws'
```

