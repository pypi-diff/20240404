# Comparing `tmp/target-ports-1.0.3.tar.gz` & `tmp/target-ports-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "target-ports-1.0.3.tar", last modified: Wed Apr  3 21:42:07 2024, max compression
+gzip compressed data, was "target-ports-1.0.4.tar", last modified: Wed Apr  3 22:04:21 2024, max compression
```

## Comparing `target-ports-1.0.3.tar` & `target-ports-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:42:07.855377 target-ports-1.0.3/
--rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.3/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 21:42:07.854795 target-ports-1.0.3/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 21:12:11.000000 target-ports-1.0.3/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 21:41:55.000000 target-ports-1.0.3/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 21:42:07.855461 target-ports-1.0.3/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:42:07.840333 target-ports-1.0.3/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:42:07.843351 target-ports-1.0.3/src/target_ports/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.3/src/target_ports/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)     5709 2024-04-03 21:41:09.000000 target-ports-1.0.3/src/target_ports/target_ports.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:42:07.854166 target-ports-1.0.3/src/target_ports.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 21:42:07.000000 target-ports-1.0.3/src/target_ports.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 21:42:07.000000 target-ports-1.0.3/src/target_ports.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 21:42:07.000000 target-ports-1.0.3/src/target_ports.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 21:42:07.000000 target-ports-1.0.3/src/target_ports.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 21:42:07.000000 target-ports-1.0.3/src/target_ports.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 21:42:07.000000 target-ports-1.0.3/src/target_ports.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:04:21.882743 target-ports-1.0.4/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1384 2024-04-03 17:05:20.000000 target-ports-1.0.4/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 22:04:21.882391 target-ports-1.0.4/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     1811 2024-04-03 21:12:11.000000 target-ports-1.0.4/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1235 2024-04-03 21:59:22.000000 target-ports-1.0.4/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 22:04:21.882811 target-ports-1.0.4/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:04:21.874924 target-ports-1.0.4/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:04:21.876300 target-ports-1.0.4/src/target_ports/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:12:54.000000 target-ports-1.0.4/src/target_ports/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     6024 2024-04-03 22:04:02.000000 target-ports-1.0.4/src/target_ports/target_ports.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 22:04:21.882020 target-ports-1.0.4/src/target_ports.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     4421 2024-04-03 22:04:21.000000 target-ports-1.0.4/src/target_ports.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      336 2024-04-03 22:04:21.000000 target-ports-1.0.4/src/target_ports.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 22:04:21.000000 target-ports-1.0.4/src/target_ports.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       58 2024-04-03 22:04:21.000000 target-ports-1.0.4/src/target_ports.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       26 2024-04-03 22:04:21.000000 target-ports-1.0.4/src/target_ports.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       13 2024-04-03 22:04:21.000000 target-ports-1.0.4/src/target_ports.egg-info/top_level.txt
```

### Comparing `target-ports-1.0.3/LICENSE` & `target-ports-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.3/PKG-INFO` & `target-ports-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.3
+Version: 1.0.4
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

### Comparing `target-ports-1.0.3/README.md` & `target-ports-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `target-ports-1.0.3/pyproject.toml` & `target-ports-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "target-ports"
-version = "1.0.3"
+version = "1.0.4"
 description = "Scan ports of a target"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
```

### Comparing `target-ports-1.0.3/src/target_ports/target_ports.py` & `target-ports-1.0.4/src/target_ports/target_ports.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,34 +13,43 @@
         """_scan_ports_:
         Scan ports on a target.
 
         Args:
             targets (str | list[str]): target ip
             nports (int, optional): Number of ports to scan. Defaults to 65535.
         """
+        # print logo
         print(termcolor.colored('target-ports', 'blue'), termcolor.colored(f'v{__version__}', 'red'), 'Jumpstart')
+        
+        # define a container
+        self.container = []
+        
         # call scan according to targets
         if type(targets)==str:
             self.scan(targets, nports)
         elif type(targets)==list[str]:
             print(termcolor.colored((f'|-- Multiple Targets Detected.'), 'blue'))
             for target in targets:
                 self.scan(target, nports)
+                if len(self.container)==0:
+                    print('|-- No Ports Opened for', termcolor.colored(f'{target}', 'red'))
+                    self.container = []
     
     def scan(self, target:str, ports: int):
         print('|-- Starting scan for', termcolor.colored(f'{target}.', 'red'))
         for port in range(1, ports+1):
             self.scanport(target, port)
     
     def scanport(self, target:str, port: int):
         try:
             sock = socket(AF_INET, SOCK_STREAM)
             s = sock.connect_ex((target, port))
             if s==0:
                 print(termcolor.colored((f'[+] Port {port} is opened.'), 'green'))
+                self.container.append(port)
             else:
                 print(f'[-] port {port} is closed.', end='\r')
             sock.close()
         except KeyboardInterrupt:
             exit(1)
         except gaierror:
             print(termcolor.colored('SCANERROR', 'red'), f' : cannot resolve {target}.')
```

### Comparing `target-ports-1.0.3/src/target_ports.egg-info/PKG-INFO` & `target-ports-1.0.4/src/target_ports.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: target-ports
-Version: 1.0.3
+Version: 1.0.4
 Summary: Scan ports of a target
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

