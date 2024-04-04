# Comparing `tmp/SideJITServer-1.1.1.tar.gz` & `tmp/SideJITServer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SideJITServer-1.1.1.tar", last modified: Sun Mar 31 23:07:10 2024, max compression
+gzip compressed data, was "SideJITServer-1.2.0.tar", last modified: Thu Apr  4 18:05:42 2024, max compression
```

## Comparing `SideJITServer-1.1.1.tar` & `SideJITServer-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:07:10.590284 SideJITServer-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:07:10.586284 SideJITServer-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:07:10.586284 SideJITServer-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-31 23:07:10.590284 SideJITServer-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/README.Docker.md
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:07:10.586284 SideJITServer-1.1.1/SideJITServer/
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/SideJITServer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/SideJITServer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-31 23:07:10.000000 SideJITServer-1.1.1/SideJITServer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 23:07:10.586284 SideJITServer-1.1.1/SideJITServer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-31 23:07:10.000000 SideJITServer-1.1.1/SideJITServer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-31 23:07:10.000000 SideJITServer-1.1.1/SideJITServer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 23:07:10.000000 SideJITServer-1.1.1/SideJITServer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-31 23:07:10.000000 SideJITServer-1.1.1/SideJITServer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-31 23:07:10.000000 SideJITServer-1.1.1/SideJITServer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-31 23:07:10.000000 SideJITServer-1.1.1/SideJITServer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-31 23:06:59.000000 SideJITServer-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 23:07:10.590284 SideJITServer-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:42.243883 SideJITServer-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:42.239884 SideJITServer-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:42.239884 SideJITServer-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-04 18:05:42.243883 SideJITServer-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/README.Docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:42.239884 SideJITServer-1.2.0/SideJITServer/
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/SideJITServer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/SideJITServer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 18:05:42.000000 SideJITServer-1.2.0/SideJITServer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:05:42.243883 SideJITServer-1.2.0/SideJITServer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-04 18:05:42.000000 SideJITServer-1.2.0/SideJITServer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-04 18:05:42.000000 SideJITServer-1.2.0/SideJITServer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:05:42.000000 SideJITServer-1.2.0/SideJITServer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-04 18:05:42.000000 SideJITServer-1.2.0/SideJITServer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 18:05:42.000000 SideJITServer-1.2.0/SideJITServer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 18:05:42.000000 SideJITServer-1.2.0/SideJITServer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 18:05:31.000000 SideJITServer-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:05:42.243883 SideJITServer-1.2.0/setup.cfg
```

### Comparing `SideJITServer-1.1.1/.dockerignore` & `SideJITServer-1.2.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.1.1/.github/workflows/python-publish.yml` & `SideJITServer-1.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.1.1/.gitignore` & `SideJITServer-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.1.1/Dockerfile` & `SideJITServer-1.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.1.1/PKG-INFO` & `SideJITServer-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SideJITServer
-Version: 1.1.1
+Version: 1.2.0
 Summary: SideJITServer is an iOS 17 JIT enabler for Windows/macOS!
 Author: khanhduytran0
 Author-email: nythepegasus <me@nythepegas.us>, JoeMatt <git@joemattiello.com>
 Maintainer-email: nythepegasus <me@nythepegas.us>
 Project-URL: Homepage, https://github.com/nythepegasus/SideJITServer
 Project-URL: Bug Reports, https://github.com/nythepegasus/SideJITServer/issues
 Keywords: ios,automation,cli,jit
@@ -17,15 +17,15 @@
 Classifier: Operating System :: iOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: pymobiledevice3<3.1.0,>=3.0.1
+Requires-Dist: pymobiledevice3<3.2.0,>=3.1.0
 Requires-Dist: Flask==3.0.2
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # SideJITServer
 This project allows you to start a server that wirelessly gives you JIT for iOS 17+ on Windows/macOS. Linux support depends on a [kernel patch](https://github.com/doronz88/pymobiledevice3/issues/566#issuecomment-1850486679).
```

### Comparing `SideJITServer-1.1.1/README.md` & `SideJITServer-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.1.1/SideJITServer/__init__.py` & `SideJITServer-1.2.0/SideJITServer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,16 @@
 @click.command()
 @click.option('-p', '--port', default=8080, help='Set the server port')
 @click.option('-e', '--version', is_flag=True, default=False, help='Prints the versions of pymobiledevice3 and SideJITServer')
 @click.option('-d', '--debug', is_flag=True, default=False, help='Enables debug output of the flask server')
 @click.option('-t', '--timeout', default=10, help='The number of seconds to wait for the pymd3 admin tunnel')
 @click.option('-v', '--verbose', default=0, count=True, help='Increase verbosity (-v for INFO, -vv for DEBUG)')
 @click.option('-y', '--pair', is_flag=True, default=False, help='Alternate pairing mode, will wait to pair to 1 device')
-def start_server(verbose, timeout, port, debug, pair, version):
+@click.option('-n', '--tunnel', is_flag=True, default=False, help='This will not launch the tunnel task! You must manually start it')
+def start_server(verbose, timeout, port, debug, pair, version, tunnel):
     if version:
         click.echo(f"pymobiledevice3: {pymd_ver}" + "\n" + f"SideJITServer: {__version__}")
         return
 
     if pair:
         click.echo("Attempting to pair to a device! (Ctrl+C to stop)")
         devices = select_devices_by_connection_type(connection_type='USB')
@@ -206,17 +207,18 @@
         if "y" not in input("Continue? [y/N]: ").lower():
             return
 
     log_levels = [logging.WARNING, logging.INFO, logging.DEBUG]
     verbosity_level = min(len(log_levels) - 1, verbose)
     logging.getLogger().setLevel(log_levels[verbosity_level])
 
-    tunneld = multiprocessing.Process(target=start_tunneld_proc)
-    tunneld.start()
+    if not tunnel:
+        tunneld = multiprocessing.Process(target=start_tunneld_proc)
+        tunneld.start()
 
-    atexit.register(tunneld.terminate)
+        atexit.register(tunneld.terminate)
 
-    sleep(timeout)
+        sleep(timeout)
 
     refresh_devs()
 
     app.run(host='0.0.0.0', port=port, debug=debug)
```

### Comparing `SideJITServer-1.1.1/SideJITServer.egg-info/PKG-INFO` & `SideJITServer-1.2.0/SideJITServer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SideJITServer
-Version: 1.1.1
+Version: 1.2.0
 Summary: SideJITServer is an iOS 17 JIT enabler for Windows/macOS!
 Author: khanhduytran0
 Author-email: nythepegasus <me@nythepegas.us>, JoeMatt <git@joemattiello.com>
 Maintainer-email: nythepegasus <me@nythepegas.us>
 Project-URL: Homepage, https://github.com/nythepegasus/SideJITServer
 Project-URL: Bug Reports, https://github.com/nythepegasus/SideJITServer/issues
 Keywords: ios,automation,cli,jit
@@ -17,15 +17,15 @@
 Classifier: Operating System :: iOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: pymobiledevice3<3.1.0,>=3.0.1
+Requires-Dist: pymobiledevice3<3.2.0,>=3.1.0
 Requires-Dist: Flask==3.0.2
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # SideJITServer
 This project allows you to start a server that wirelessly gives you JIT for iOS 17+ on Windows/macOS. Linux support depends on a [kernel patch](https://github.com/doronz88/pymobiledevice3/issues/566#issuecomment-1850486679).
```

### Comparing `SideJITServer-1.1.1/compose.yaml` & `SideJITServer-1.2.0/compose.yaml`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.1.1/pyproject.toml` & `SideJITServer-1.2.0/pyproject.toml`

 * *Files identical despite different names*

