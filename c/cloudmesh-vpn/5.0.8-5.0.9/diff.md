# Comparing `tmp/cloudmesh-vpn-5.0.8.tar.gz` & `tmp/cloudmesh-vpn-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudmesh-vpn-5.0.8.tar", last modified: Wed Dec 27 04:41:36 2023, max compression
+gzip compressed data, was "cloudmesh-vpn-5.0.9.tar", last modified: Wed Dec 27 05:26:52 2023, max compression
```

## Comparing `cloudmesh-vpn-5.0.8.tar` & `cloudmesh-vpn-5.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-12-27 04:41:36.416832 cloudmesh-vpn-5.0.8/
--rw-rw-rw-   0        0        0      778 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.8/LICENSE
--rw-rw-rw-   0        0        0      166 2023-12-27 03:48:05.000000 cloudmesh-vpn-5.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8216 2023-12-27 04:41:36.416345 cloudmesh-vpn-5.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4736 2023-12-26 20:02:15.000000 cloudmesh-vpn-5.0.8/README.md
--rw-rw-rw-   0        0        0        5 2023-12-27 04:39:03.000000 cloudmesh-vpn-5.0.8/VERSION
--rw-rw-rw-   0        0        0     2477 2023-12-27 04:39:03.000000 cloudmesh-vpn-5.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       82 2023-12-27 04:23:33.000000 cloudmesh-vpn-5.0.8/requirements-dev.txt
--rw-rw-rw-   0        0        0       96 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.8/requirements.txt
--rw-rw-rw-   0        0        0       74 2023-12-27 04:41:36.416963 cloudmesh-vpn-5.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-12-27 04:41:36.386524 cloudmesh-vpn-5.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-12-27 04:41:36.384317 cloudmesh-vpn-5.0.8/src/cloudmesh/
-drwxrwxrwx   0        0        0        0 2023-12-27 04:41:36.399964 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/
--rw-rw-rw-   0        0        0       22 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-27 04:41:36.403329 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/bin/
--rw-rw-rw-   0        0        0    10519 2023-12-26 22:36:32.000000 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/bin/split-script-win.js
--rw-rw-rw-   0        0        0    10149 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/bin/split-script-win.python.py
-drwxrwxrwx   0        0        0        0 2023-12-27 04:41:36.406331 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/command/
--rw-rw-rw-   0        0        0        0 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/command/__init__.py
--rw-rw-rw-   0        0        0     3565 2023-12-27 04:36:03.000000 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/command/vpn.py
--rw-rw-rw-   0        0        0    30861 2023-12-27 04:35:56.000000 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/vpn.py
--rw-rw-rw-   0        0        0     3931 2023-12-26 02:19:06.000000 cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/windows.py
-drwxrwxrwx   0        0        0        0 2023-12-27 04:41:36.415329 cloudmesh-vpn-5.0.8/src/cloudmesh_vpn.egg-info/
--rw-rw-rw-   0        0        0     8216 2023-12-27 04:41:36.000000 cloudmesh-vpn-5.0.8/src/cloudmesh_vpn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-12-27 04:41:36.000000 cloudmesh-vpn-5.0.8/src/cloudmesh_vpn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-27 04:41:36.000000 cloudmesh-vpn-5.0.8/src/cloudmesh_vpn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-12-27 04:41:36.000000 cloudmesh-vpn-5.0.8/src/cloudmesh_vpn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-27 04:41:36.000000 cloudmesh-vpn-5.0.8/src/cloudmesh_vpn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-12-27 04:41:36.413329 cloudmesh-vpn-5.0.8/tests/
--rw-rw-rw-   0        0        0     1088 2023-11-28 03:13:34.000000 cloudmesh-vpn-5.0.8/tests/test_shell.py
+drwxrwxrwx   0        0        0        0 2023-12-27 05:26:52.601376 cloudmesh-vpn-5.0.9/
+-rw-rw-rw-   0        0        0      778 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.9/LICENSE
+-rw-rw-rw-   0        0        0      166 2023-12-27 03:48:05.000000 cloudmesh-vpn-5.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8216 2023-12-27 05:26:52.600898 cloudmesh-vpn-5.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4736 2023-12-26 20:02:15.000000 cloudmesh-vpn-5.0.9/README.md
+-rw-rw-rw-   0        0        0        5 2023-12-27 05:25:25.000000 cloudmesh-vpn-5.0.9/VERSION
+-rw-rw-rw-   0        0        0     2477 2023-12-27 05:25:25.000000 cloudmesh-vpn-5.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       82 2023-12-27 04:23:33.000000 cloudmesh-vpn-5.0.9/requirements-dev.txt
+-rw-rw-rw-   0        0        0       96 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       74 2023-12-27 05:26:52.604432 cloudmesh-vpn-5.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-12-27 05:26:52.548552 cloudmesh-vpn-5.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-12-27 05:26:52.546504 cloudmesh-vpn-5.0.9/src/cloudmesh/
+drwxrwxrwx   0        0        0        0 2023-12-27 05:26:52.573458 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/
+-rw-rw-rw-   0        0        0       22 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-27 05:26:52.577379 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/bin/
+-rw-rw-rw-   0        0        0    10519 2023-12-26 22:36:32.000000 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/bin/split-script-win.js
+-rw-rw-rw-   0        0        0    10149 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/bin/split-script-win.python.py
+drwxrwxrwx   0        0        0        0 2023-12-27 05:26:52.581368 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/command/
+-rw-rw-rw-   0        0        0        0 2023-12-25 03:23:59.000000 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/command/__init__.py
+-rw-rw-rw-   0        0        0     3565 2023-12-27 04:36:03.000000 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/command/vpn.py
+-rw-rw-rw-   0        0        0    30861 2023-12-27 04:35:56.000000 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/vpn.py
+-rw-rw-rw-   0        0        0     3934 2023-12-27 05:23:32.000000 cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/windows.py
+drwxrwxrwx   0        0        0        0 2023-12-27 05:26:52.598693 cloudmesh-vpn-5.0.9/src/cloudmesh_vpn.egg-info/
+-rw-rw-rw-   0        0        0     8216 2023-12-27 05:26:52.000000 cloudmesh-vpn-5.0.9/src/cloudmesh_vpn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      570 2023-12-27 05:26:52.000000 cloudmesh-vpn-5.0.9/src/cloudmesh_vpn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-27 05:26:52.000000 cloudmesh-vpn-5.0.9/src/cloudmesh_vpn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-12-27 05:26:52.000000 cloudmesh-vpn-5.0.9/src/cloudmesh_vpn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-12-27 05:26:52.000000 cloudmesh-vpn-5.0.9/src/cloudmesh_vpn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-27 05:26:52.595598 cloudmesh-vpn-5.0.9/tests/
+-rw-rw-rw-   0        0        0     1088 2023-11-28 03:13:34.000000 cloudmesh-vpn-5.0.9/tests/test_shell.py
```

### Comparing `cloudmesh-vpn-5.0.8/LICENSE` & `cloudmesh-vpn-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-5.0.8/PKG-INFO` & `cloudmesh-vpn-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-vpn
-Version: 5.0.8
+Version: 5.0.9
 Summary: Virtual Private Network connection in the cloudmesh suite
 Author-email: Gregor von Laszewski <laszewski@gmail.com>, "J.P. Fleischer" <jacquespfleischer@gmail.com>
 Maintainer-email: Gregor von Laszewski <laszewski@gmail.com>, "J.P. Fleischer" <jacquespfleischer@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `cloudmesh-vpn-5.0.8/README.md` & `cloudmesh-vpn-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-5.0.8/pyproject.toml` & `cloudmesh-vpn-5.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools >= 69",
     "wheel >= 0.42",
     "pip >= 23.2.1"
 ]
 
 [project]
 name = "cloudmesh-vpn"
-version = "5.0.8"
+version = "5.0.9"
 description = "Virtual Private Network connection in the cloudmesh suite"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Gregor von Laszewski", email = "laszewski@gmail.com"},
     {name = "J.P. Fleischer", email = "jacquespfleischer@gmail.com"}
```

### Comparing `cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/bin/split-script-win.js` & `cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/bin/split-script-win.js`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/bin/split-script-win.python.py` & `cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/bin/split-script-win.python.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/command/vpn.py` & `cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/command/vpn.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/vpn.py` & `cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/vpn.py`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-5.0.8/src/cloudmesh/vpn/windows.py` & `cloudmesh-vpn-5.0.9/src/cloudmesh/vpn/windows.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             os._exit(1)
         Console.msg('Installing OpenConnect...')
         # try:
         #     r =
         # except subprocess.CalledProcessError as e:
 
         # command = f'cd {current_script_directory}/bin && choco install chocolatey-core.extension -y && choco pack && choco install cisco-secure-client --debug --verbose --source . --force -y'
-        command = f'choco install openconnect --version=9.12.0.20231224'
+        command = f'choco install openconnect --version=9.12.0.20231224 -y'
         # try:
 
         #     r = Shell.run()
         # except subprocess.CalledProcessError as e:
         #     print(e.output)
 
         process = subprocess.Popen(
```

### Comparing `cloudmesh-vpn-5.0.8/src/cloudmesh_vpn.egg-info/PKG-INFO` & `cloudmesh-vpn-5.0.9/src/cloudmesh_vpn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudmesh-vpn
-Version: 5.0.8
+Version: 5.0.9
 Summary: Virtual Private Network connection in the cloudmesh suite
 Author-email: Gregor von Laszewski <laszewski@gmail.com>, "J.P. Fleischer" <jacquespfleischer@gmail.com>
 Maintainer-email: Gregor von Laszewski <laszewski@gmail.com>, "J.P. Fleischer" <jacquespfleischer@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `cloudmesh-vpn-5.0.8/src/cloudmesh_vpn.egg-info/SOURCES.txt` & `cloudmesh-vpn-5.0.9/src/cloudmesh_vpn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudmesh-vpn-5.0.8/tests/test_shell.py` & `cloudmesh-vpn-5.0.9/tests/test_shell.py`

 * *Files identical despite different names*

