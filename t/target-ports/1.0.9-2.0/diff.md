# Comparing `tmp/target-ports-1.0.9.tar.gz` & `tmp/target-ports-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-1.0.9.tar", last modified: Wed Apr  3 23:38:01 2024, max compression
+gzip compressed data, was "target-ports-2.0.tar", last modified: Wed Apr  3 23:40:05 2024, max compression
```

## Comparing `target-ports-1.0.9.tar` & `target-ports-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:38:01.076297 target-ports-1.0.9/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.9/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 23:38:01.075665 target-ports-1.0.9/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 22:52:42.000000 target-ports-1.0.9/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 23:37:24.000000 target-ports-1.0.9/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 23:38:01.076433 target-ports-1.0.9/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:38:01.061810 target-ports-1.0.9/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:38:01.065122 target-ports-1.0.9/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.9/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     6564 2024-04-03 23:37:31.000000 target-ports-1.0.9/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:38:01.074995 target-ports-1.0.9/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 23:38:01.000000 target-ports-1.0.9/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 23:38:01.000000 target-ports-1.0.9/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 23:38:01.000000 target-ports-1.0.9/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 23:38:01.000000 target-ports-1.0.9/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 23:38:01.000000 target-ports-1.0.9/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 23:38:01.000000 target-ports-1.0.9/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:40:05.359513 target-ports-2.0/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-2.0/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4419 2024-04-03 23:40:05.358899 target-ports-2.0/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 22:52:42.000000 target-ports-2.0/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1233 2024-04-03 23:39:44.000000 target-ports-2.0/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 23:40:05.359604 target-ports-2.0/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:40:05.345551 target-ports-2.0/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:40:05.348823 target-ports-2.0/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-2.0/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     6599 2024-04-03 23:39:39.000000 target-ports-2.0/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:40:05.358284 target-ports-2.0/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4419 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 23:40:05.000000 target-ports-2.0/src/target_ports.egg-info/top_level.txt
```

### Comparing `target-ports-1.0.9/LICENSE` & `target-ports-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.9/PKG-INFO` & `target-ports-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.9
+Version: 2.0
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

### Comparing `target-ports-1.0.9/README.md` & `target-ports-2.0/README.md`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.9/pyproject.toml` & `target-ports-2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "1.0.9"
+version = "2.0"
 description = "Scan ports of a target"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
```

### Comparing `target-ports-1.0.9/src/target_ports/target_ports.py` & `target-ports-2.0/src/target_ports/target_ports.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-__version__ = '1.0.9'
+__version__ = '2.0'
 
 from socket import socket, AF_INET, SOCK_STREAM, gaierror, error, setdefaulttimeout
 from optioner import options
 from sys import argv
 from re import match
 import termcolor
 
@@ -54,14 +54,15 @@
             if s==0:
                 print(termcolor.colored((f'[+] Port {port} is opened.'), 'green'))
                 self.container.append(port)
             else:
                 print(termcolor.colored(f'[-] port {port} is closed.', 'yellow'), end='\r')
             sock.close()
         except KeyboardInterrupt:
+            print('error', end='\r')
             print('|-- EXIT -', termcolor.colored('Keyboard Interrupt', 'red'))
             exit(1)
         except gaierror:
             print(termcolor.colored('SCANERROR', 'red'), f' : cannot resolve {target}.')
             exit(1)
         except error:
             print(termcolor.colored('SCANERROR', 'red'), f' : {target} did not respond.')
```

### Comparing `target-ports-1.0.9/src/target_ports.egg-info/PKG-INFO` & `target-ports-2.0/src/target_ports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.9
+Version: 2.0
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

