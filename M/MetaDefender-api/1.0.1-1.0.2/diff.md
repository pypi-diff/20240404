# Comparing `tmp/MetaDefender_api-1.0.1.tar.gz` & `tmp/MetaDefender_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MetaDefender_api-1.0.1.tar", last modified: Thu Apr  4 15:55:04 2024, max compression
+gzip compressed data, was "MetaDefender_api-1.0.2.tar", last modified: Thu Apr  4 16:00:02 2024, max compression
```

## Comparing `MetaDefender_api-1.0.1.tar` & `MetaDefender_api-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 15:55:04.692665 MetaDefender_api-1.0.1/
--rw-rw-rw-   0        0        0    35108 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       29 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      988 2024-04-04 15:55:04.692159 MetaDefender_api-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-04-04 13:44:21.000000 MetaDefender_api-1.0.1/README.md
--rw-rw-rw-   0        0        0       72 2024-04-04 15:37:02.000000 MetaDefender_api-1.0.1/__init__.py
--rw-rw-rw-   0        0        0      108 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      581 2024-04-04 15:55:04.693664 MetaDefender_api-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-04 15:55:04.677497 MetaDefender_api-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-04 15:55:04.691155 MetaDefender_api-1.0.1/src/MetaDefender_api.egg-info/
--rw-rw-rw-   0        0        0      988 2024-04-04 15:55:04.000000 MetaDefender_api-1.0.1/src/MetaDefender_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-04 15:55:04.000000 MetaDefender_api-1.0.1/src/MetaDefender_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:55:04.000000 MetaDefender_api-1.0.1/src/MetaDefender_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 15:55:04.000000 MetaDefender_api-1.0.1/src/MetaDefender_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 16:00:02.113134 MetaDefender_api-1.0.2/
+-rw-rw-rw-   0        0        0    35108 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0       29 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      988 2024-04-04 16:00:02.113134 MetaDefender_api-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-04-04 15:58:24.000000 MetaDefender_api-1.0.2/README.md
+-rw-rw-rw-   0        0        0       72 2024-04-04 15:37:02.000000 MetaDefender_api-1.0.2/__init__.py
+-rw-rw-rw-   0        0        0      108 2024-04-04 13:42:10.000000 MetaDefender_api-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      581 2024-04-04 16:00:02.114634 MetaDefender_api-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-04 16:00:02.101874 MetaDefender_api-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-04 16:00:02.112136 MetaDefender_api-1.0.2/src/MetaDefender_api.egg-info/
+-rw-rw-rw-   0        0        0      988 2024-04-04 16:00:02.000000 MetaDefender_api-1.0.2/src/MetaDefender_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-04 16:00:02.000000 MetaDefender_api-1.0.2/src/MetaDefender_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 16:00:02.000000 MetaDefender_api-1.0.2/src/MetaDefender_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 16:00:02.000000 MetaDefender_api-1.0.2/src/MetaDefender_api.egg-info/top_level.txt
```

### Comparing `MetaDefender_api-1.0.1/LICENSE` & `MetaDefender_api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MetaDefender_api-1.0.1/PKG-INFO` & `MetaDefender_api-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: MetaDefender_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple MetaDefender Api wrapper
 Home-page: https://github.com/cookie0o
 Author: cookie0_o
 Author-email: raphael.contact@zohomail.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align=center>
   
-  # MetaDefender_api v1.0.0
+  # MetaDefender_api v1.0.2
   
   **A simple MetaDefender Api wrapper**
 </div>
 
 ## +Info and usage:
-go to the wiki on the Github Page [here](https://github.com/sch-raphael/MetaDefender_api/wiki).  
+go to the wiki on the Github Page [here](https://github.com/sch-raphael/MetaDefender-api/wiki).  
 
 ## +Install:
 **manually**
-- Download the project [here](https://github.com/cookie0o/MetaDefender_api)
+- Download the project [here](https://github.com/cookie0o/MetaDefender-api)
 - cd in the project dir with the console
 - run: `pip install . --upgrade`
 - your done!
 
-**from [pip](https://pypi.org/project/MetaDefender_api/)**
-- run: `pip install MetaDefender_api`
+**from [pip](https://pypi.org/project/MetaDefender-api/)**
+- run: `pip install MetaDefender-api`
 - your done!
```

### Comparing `MetaDefender_api-1.0.1/setup.cfg` & `MetaDefender_api-1.0.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204d 6574 6144 6566 656e 6465 725f   = MetaDefender_
 00000020: 6170 690d 0a76 6572 7369 6f6e 203d 2031  api..version = 1
-00000030: 2e30 2e31 0d0a 6175 7468 6f72 203d 2063  .0.1..author = c
+00000030: 2e30 2e32 0d0a 6175 7468 6f72 203d 2063  .0.2..author = c
 00000040: 6f6f 6b69 6530 5f6f 0d0a 6175 7468 6f72  ookie0_o..author
 00000050: 5f65 6d61 696c 203d 2072 6170 6861 656c  _email = raphael
 00000060: 2e63 6f6e 7461 6374 407a 6f68 6f6d 6169  .contact@zohomai
 00000070: 6c2e 6575 0d0a 7572 6c20 3d20 6874 7470  l.eu..url = http
 00000080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
 00000090: 6f6f 6b69 6530 6f0d 0a64 6573 6372 6970  ookie0o..descrip
 000000a0: 7469 6f6e 203d 2041 2073 696d 706c 6520  tion = A simple
```

### Comparing `MetaDefender_api-1.0.1/src/MetaDefender_api.egg-info/PKG-INFO` & `MetaDefender_api-1.0.2/src/MetaDefender_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: MetaDefender_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple MetaDefender Api wrapper
 Home-page: https://github.com/cookie0o
 Author: cookie0_o
 Author-email: raphael.contact@zohomail.eu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align=center>
   
-  # MetaDefender_api v1.0.0
+  # MetaDefender_api v1.0.2
   
   **A simple MetaDefender Api wrapper**
 </div>
 
 ## +Info and usage:
-go to the wiki on the Github Page [here](https://github.com/sch-raphael/MetaDefender_api/wiki).  
+go to the wiki on the Github Page [here](https://github.com/sch-raphael/MetaDefender-api/wiki).  
 
 ## +Install:
 **manually**
-- Download the project [here](https://github.com/cookie0o/MetaDefender_api)
+- Download the project [here](https://github.com/cookie0o/MetaDefender-api)
 - cd in the project dir with the console
 - run: `pip install . --upgrade`
 - your done!
 
-**from [pip](https://pypi.org/project/MetaDefender_api/)**
-- run: `pip install MetaDefender_api`
+**from [pip](https://pypi.org/project/MetaDefender-api/)**
+- run: `pip install MetaDefender-api`
 - your done!
```

