# Comparing `tmp/target-ports-1.0.7.tar.gz` & `tmp/target-ports-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-1.0.7.tar", last modified: Wed Apr  3 23:05:25 2024, max compression
+gzip compressed data, was "target-ports-1.0.8.tar", last modified: Wed Apr  3 23:35:22 2024, max compression
```

## Comparing `target-ports-1.0.7.tar` & `target-ports-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:05:25.478258 target-ports-1.0.7/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.7/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 23:05:25.477291 target-ports-1.0.7/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 22:52:42.000000 target-ports-1.0.7/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 23:04:10.000000 target-ports-1.0.7/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 23:05:25.478442 target-ports-1.0.7/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:05:25.463634 target-ports-1.0.7/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:05:25.466735 target-ports-1.0.7/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.7/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     6273 2024-04-03 23:04:06.000000 target-ports-1.0.7/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:05:25.476207 target-ports-1.0.7/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 23:05:25.000000 target-ports-1.0.7/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 23:05:25.000000 target-ports-1.0.7/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 23:05:25.000000 target-ports-1.0.7/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 23:05:25.000000 target-ports-1.0.7/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 23:05:25.000000 target-ports-1.0.7/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 23:05:25.000000 target-ports-1.0.7/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:35:22.082034 target-ports-1.0.8/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.8/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 23:35:22.081342 target-ports-1.0.8/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 22:52:42.000000 target-ports-1.0.8/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 23:30:26.000000 target-ports-1.0.8/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 23:35:22.082122 target-ports-1.0.8/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:35:22.067468 target-ports-1.0.8/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:35:22.070708 target-ports-1.0.8/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.8/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     6484 2024-04-03 23:35:13.000000 target-ports-1.0.8/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 23:35:22.080689 target-ports-1.0.8/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 23:35:22.000000 target-ports-1.0.8/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 23:35:22.000000 target-ports-1.0.8/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 23:35:22.000000 target-ports-1.0.8/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 23:35:22.000000 target-ports-1.0.8/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 23:35:22.000000 target-ports-1.0.8/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 23:35:22.000000 target-ports-1.0.8/src/target_ports.egg-info/top_level.txt
```

### Comparing `target-ports-1.0.7/LICENSE` & `target-ports-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.7/PKG-INFO` & `target-ports-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.7
+Version: 1.0.8
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

### Comparing `target-ports-1.0.7/README.md` & `target-ports-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.7/pyproject.toml` & `target-ports-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "1.0.7"
+version = "1.0.8"
 description = "Scan ports of a target"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
```

### Comparing `target-ports-1.0.7/src/target_ports/target_ports.py` & `target-ports-1.0.8/src/target_ports/target_ports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-__version__ = '1.0.7'
+__version__ = '1.0.8'
 
 from socket import socket, AF_INET, SOCK_STREAM, gaierror, error, setdefaulttimeout
 from optioner import options
 from sys import argv
 from re import match
 import termcolor
 
@@ -25,31 +25,35 @@
         
         # call scan according to targets
         if type(targets)==str:
             self.scan(targets, nports)
             if len(self.container)==0:
                 print('|-- No Ports Opened for', termcolor.colored(f'{targets}', 'red'))
                 self.container = []
+            else:
+                print('|-- Scan ended for', termcolor.colored(f'{targets}', 'red'))
         elif type(targets)==list[str]:
             print(termcolor.colored((f'|-- Multiple Targets Detected.'), 'blue'))
             for target in targets:
                 self.scan(target, nports)
                 if len(self.container)==0:
                     print('|-- No Ports Opened for', termcolor.colored(f'{target}', 'red'))
                     self.container = []
+                else:
+                    print('|-- Scan ended for', termcolor.colored(f'{target}', 'red'))
     
     def scan(self, target:str, ports: int):
         print('|-- Starting scan for', termcolor.colored(f'{target}.', 'red'))
         for port in range(1, ports+1):
             self.scanport(target, port)
     
     def scanport(self, target:str, port: int):
         try:
             sock = socket(AF_INET, SOCK_STREAM)
-            setdefaulttimeout(2.5)
+            setdefaulttimeout(1.1)
             s = sock.connect_ex((target, port))
             if s==0:
                 print(termcolor.colored((f'[+] Port {port} is opened.'), 'green'))
                 self.container.append(port)
             else:
                 print(termcolor.colored(f'[-] port {port} is closed.', 'yellow'), end='\r')
             sock.close()
```

### Comparing `target-ports-1.0.7/src/target_ports.egg-info/PKG-INFO` & `target-ports-1.0.8/src/target_ports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.7
+Version: 1.0.8
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

