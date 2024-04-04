# Comparing `tmp/logrepl-0.1.9.tar.gz` & `tmp/logrepl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrepl-0.1.9.tar", max compression
+gzip compressed data, was "logrepl-0.2.0.tar", max compression
```

## Comparing `logrepl-0.1.9.tar` & `logrepl-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.1.9/LICENSE
--rw-r--r--   0        0        0     1586 2024-03-12 08:53:56.800065 logrepl-0.1.9/README.md
--rw-r--r--   0        0        0      149 2024-03-12 07:11:03.648211 logrepl-0.1.9/logrepl/__init__.py
--rw-r--r--   0        0        0     2805 2024-03-12 08:12:07.064724 logrepl-0.1.9/logrepl/handler.py
--rw-r--r--   0        0        0     1025 2024-03-12 06:10:22.142025 logrepl-0.1.9/logrepl/run.py
--rw-r--r--   0        0        0      507 2024-03-12 09:43:55.001945 logrepl-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 logrepl-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2954 2024-04-04 15:16:31.672216 logrepl-0.2.0/README.md
+-rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.0/logrepl/__init__.py
+-rw-r--r--   0        0        0     7895 2024-04-04 15:01:45.293613 logrepl-0.2.0/logrepl/handler.py
+-rw-r--r--   0        0        0      789 2024-04-04 14:20:57.326734 logrepl-0.2.0/logrepl/run.py
+-rw-r--r--   0        0        0      507 2024-04-04 15:17:11.172226 logrepl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 logrepl-0.2.0/PKG-INFO
```

### Comparing `logrepl-0.1.9/LICENSE` & `logrepl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logrepl-0.1.9/README.md` & `logrepl-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,26 @@
 run the repl:
 ```
 pylogrepl
 ```
 
 then the whole repl will be logged to the file `yyyymmddhhmm.log`.
 
+You can also use *logrepl* to log the whole stream io of a program by:
+
+```
+with logrepl.log_handler(
+    log_dir,
+    prefix,
+    err_acc_time
+) as logrepl_handler:
+    # run your program here
+    # ...
+```
+
 # Config
 
 ## Prefix of the log file
 
 use the optional positional argument, for example:
 ```
 pylogrepl prefix
@@ -22,54 +34,75 @@
 
 then the log file will be `prefix_yyyymmddhhmm.log`.
 
 ## Dir to save the logs
 
 use the `-d` or `--dir` options:
 ```
-pylogrepl -d logs
-pylogrepl --dir logs
+pylogrepl -d "store/logs"
+pylogrepl --dir "store/logs"
 ```
 
-then the log file will be in the `logs` directory.
+then the log file will be in the `store/logs` directory.
+
+## Time interval to collect errors of logrepl
+
+We found that if something goes wrong in *logrepl*, it may produce many highly repeatitive exceptions is a short time. To avoid getting overwhelmed by those error messages, *logrepl* will collect them in a time interval and then print the non-duplicated ones. To set the time interval (although it should be non-necessary), use the '-t' or '--time' options:
+
+```
+pylogrepl -t 1.5
+pylogrepl --time 1.5
+```
+
+the unit is second.
 
 ## By .pylogrepl file
 
 You can also sepcify the prefix & the directory by making a `.pylogrepl` in the working directory:
 
 ```
 dir=logs
 prefix=my_prefix
+err_acc_time=1.5
 ```
 
 note that the command line arguments are prioritized over the settings in `.pylogrepl`. We suggest that specifying `dir` in `.pylogrepl` and `prefix` by command line argument is a handy approach.
 
 # APIs
 
-By executing `pylogrepl`, the module `logrepl` will be loaded to the current namespace.
+By executing `pylogrepl`, the `logrepl_handler` of class `logrepl.Handler` will be loaded to the current namespace. The `logrepl_handler` controls the logging behavior of the repl.
 
 ## update logging dir / file
 
-**logrepl.update(prefix=None, new_dir=None)**
+**logrepl.Handler.set_dir(log_dir)**
+
+Update new logging dir. `log_dir` must be `string` or `Path`. The suffix `_yyyymmddhhmm.log` will also be updated while the `prefix` will remain unchanged.
+
+**logrepl.Handler.set_prefix(prefix)**
+
+Update new prefix for the log file. `prefix` sholud be `str` or `None`. The suffix `_yyyymmddhhmm.log` will also be updated while the `log_dir` will remain unchanged. Drop the prefix of new log file by setting `prefix` as `None`.
 
-Update new logging dir & new prefix. When `new_dir` is not provided, the logging dir remain unchanged; when `prefix` is not provided, logs will be written to a new `yyyymmddhhmm.log`, i.e. the previous prefix will be dropped.
+**logrepl.Handler.update_suffix()**
+Update the timestamp suffix with `log_dir` & `prefix` unchanged.
 
 ## start / stop logging to file
 
-**logrepl.start_log()**
+**logrepl.Handler.start_log()**
 
 start logging to the file.
 
-**logrepl.stop_log()**
+**logrepl.Handler.stop_log()**
 
 stop logging to the file.
 
-## Handler
+## handle sys.stdin/stdout/stderr & builtins.input
 
-**logrepl.repl_handler**
+**logrepl.Handler.set_io()**
+To log **everything** of the repl, *logrepl* modifies sys.stdin/stdout/stderr & builtins.input by this method.
 
-the `Handler` object that controls the logging behavior of the repl.
+**logrepl.Handler.reset_io()**
+Reset sys.stdin/stdout/stderr & builtins.input as-is. The repl will still log input into the file after executing `reset_io`.
 
 # Notes
 
 Exceptions ocurred when writing to the log file will not be logged since it'll lead to infinite loop.
```

