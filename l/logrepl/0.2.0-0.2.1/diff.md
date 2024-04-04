# Comparing `tmp/logrepl-0.2.0.tar.gz` & `tmp/logrepl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrepl-0.2.0.tar", max compression
+gzip compressed data, was "logrepl-0.2.1.tar", max compression
```

## Comparing `logrepl-0.2.0.tar` & `logrepl-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.0/LICENSE
--rw-r--r--   0        0        0     2954 2024-04-04 15:16:31.672216 logrepl-0.2.0/README.md
--rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.0/logrepl/__init__.py
--rw-r--r--   0        0        0     7895 2024-04-04 15:01:45.293613 logrepl-0.2.0/logrepl/handler.py
--rw-r--r--   0        0        0      789 2024-04-04 14:20:57.326734 logrepl-0.2.0/logrepl/run.py
--rw-r--r--   0        0        0      507 2024-04-04 15:17:11.172226 logrepl-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 logrepl-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2956 2024-04-04 15:22:13.586885 logrepl-0.2.1/README.md
+-rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.1/logrepl/__init__.py
+-rw-r--r--   0        0        0     7895 2024-04-04 15:01:45.293613 logrepl-0.2.1/logrepl/handler.py
+-rw-r--r--   0        0        0      789 2024-04-04 14:20:57.326734 logrepl-0.2.1/logrepl/run.py
+-rw-r--r--   0        0        0      507 2024-04-04 15:23:00.367989 logrepl-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 logrepl-0.2.1/PKG-INFO
```

### Comparing `logrepl-0.2.0/LICENSE` & `logrepl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.0/README.md` & `logrepl-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,18 @@
 **logrepl.Handler.stop_log()**
 
 stop logging to the file.
 
 ## handle sys.stdin/stdout/stderr & builtins.input
 
 **logrepl.Handler.set_io()**
+
 To log **everything** of the repl, *logrepl* modifies sys.stdin/stdout/stderr & builtins.input by this method.
 
 **logrepl.Handler.reset_io()**
+
 Reset sys.stdin/stdout/stderr & builtins.input as-is. The repl will still log input into the file after executing `reset_io`.
 
 # Notes
 
 Exceptions ocurred when writing to the log file will not be logged since it'll lead to infinite loop.
```

### Comparing `logrepl-0.2.0/logrepl/handler.py` & `logrepl-0.2.1/logrepl/handler.py`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.0/logrepl/run.py` & `logrepl-0.2.1/logrepl/run.py`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.0/PKG-INFO` & `logrepl-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrepl
-Version: 0.2.0
+Version: 0.2.1
 Summary: By this command line tool, you can run a python repl which logs everying into a file.
 Home-page: https://github.com/baliuzeger/logrepl
 Keywords: repl,log,logging
 Author: bali
 Author-email: baluzeger@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -114,17 +114,19 @@
 **logrepl.Handler.stop_log()**
 
 stop logging to the file.
 
 ## handle sys.stdin/stdout/stderr & builtins.input
 
 **logrepl.Handler.set_io()**
+
 To log **everything** of the repl, *logrepl* modifies sys.stdin/stdout/stderr & builtins.input by this method.
 
 **logrepl.Handler.reset_io()**
+
 Reset sys.stdin/stdout/stderr & builtins.input as-is. The repl will still log input into the file after executing `reset_io`.
 
 # Notes
 
 Exceptions ocurred when writing to the log file will not be logged since it'll lead to infinite loop.
```

