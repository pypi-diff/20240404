# Comparing `tmp/subprocess_loop-1.0.8.tar.gz` & `tmp/subprocess_loop-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subprocess_loop-1.0.8.tar", last modified: Tue Feb 13 08:54:43 2024, max compression
+gzip compressed data, was "subprocess_loop-1.0.9.tar", last modified: Thu Apr  4 06:10:49 2024, max compression
```

## Comparing `subprocess_loop-1.0.8.tar` & `subprocess_loop-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-02-13 08:54:43.323433 subprocess_loop-1.0.8/
--rw-rw-rw-   0        0        0     1109 2024-02-13 05:19:50.000000 subprocess_loop-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      228 2024-02-13 08:54:43.322432 subprocess_loop-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-02-13 08:54:43.323433 subprocess_loop-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      288 2024-02-13 08:25:16.000000 subprocess_loop-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-13 08:54:43.296395 subprocess_loop-1.0.8/subprocess_loop/
--rw-rw-rw-   0        0        0       39 2024-02-13 05:19:50.000000 subprocess_loop-1.0.8/subprocess_loop/__init__.py
--rw-rw-rw-   0        0        0     1594 2024-02-13 08:23:51.000000 subprocess_loop-1.0.8/subprocess_loop/child.py
-drwxrwxrwx   0        0        0        0 2024-02-13 08:54:43.321483 subprocess_loop-1.0.8/subprocess_loop.egg-info/
--rw-rw-rw-   0        0        0      228 2024-02-13 08:54:42.000000 subprocess_loop-1.0.8/subprocess_loop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-02-13 08:54:42.000000 subprocess_loop-1.0.8/subprocess_loop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-13 08:54:42.000000 subprocess_loop-1.0.8/subprocess_loop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-13 08:54:42.000000 subprocess_loop-1.0.8/subprocess_loop.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 06:10:49.839288 subprocess_loop-1.0.9/
+-rw-rw-rw-   0        0        0     1109 2024-02-08 16:04:54.000000 subprocess_loop-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      228 2024-04-04 06:10:49.838286 subprocess_loop-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-04 06:10:49.839794 subprocess_loop-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      288 2024-04-04 06:07:34.000000 subprocess_loop-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:10:49.788211 subprocess_loop-1.0.9/subprocess_loop/
+-rw-rw-rw-   0        0        0       39 2024-02-09 16:58:43.000000 subprocess_loop-1.0.9/subprocess_loop/__init__.py
+-rw-rw-rw-   0        0        0     1582 2024-04-04 06:06:42.000000 subprocess_loop-1.0.9/subprocess_loop/child.py
+drwxrwxrwx   0        0        0        0 2024-04-04 06:10:49.801248 subprocess_loop-1.0.9/subprocess_loop.egg-info/
+-rw-rw-rw-   0        0        0      228 2024-04-04 06:10:49.000000 subprocess_loop-1.0.9/subprocess_loop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-04 06:10:49.000000 subprocess_loop-1.0.9/subprocess_loop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 06:10:49.000000 subprocess_loop-1.0.9/subprocess_loop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-04 06:10:49.000000 subprocess_loop-1.0.9/subprocess_loop.egg-info/top_level.txt
```

### Comparing `subprocess_loop-1.0.8/LICENSE` & `subprocess_loop-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `subprocess_loop-1.0.8/subprocess_loop/child.py` & `subprocess_loop-1.0.9/subprocess_loop/child.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,14 @@
     _orig_stdin = sys.stdin
     sys.stdout = _stdout
     sys.stdin = _stdin
 
     @staticmethod
     def run(on_request):
 
-        Child._stdout.on_write(Child._on_default_write)
-
         while(True):
             request_json = Child._orig_stdin.readline()
             if (len(request_json)==0):
                 break
             request = json.loads(request_json)
             response_data = on_request(request["data"])
             response = {"id": request["id"], "data": response_data}
@@ -55,7 +53,8 @@
 
     @staticmethod
     def _on_default_write(data):
         response = {"stdout": data}
         Child._orig_stdout.write(json.dumps(response))
         Child._orig_stdout.flush()
 
+Child._stdout.on_write(Child._on_default_write)
```

