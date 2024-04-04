# Comparing `tmp/loggerjava-0.7.6.tar.gz` & `tmp/loggerjava-0.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerjava-0.7.6.tar", last modified: Thu Apr  4 04:39:07 2024, max compression
+gzip compressed data, was "loggerjava-0.8.0.dev1.tar", last modified: Thu Apr  4 15:13:03 2024, max compression
```

## Comparing `loggerjava-0.7.6.tar` & `loggerjava-0.8.0.dev1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:39:07.943115 loggerjava-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 04:39:00.000000 loggerjava-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-04 04:39:07.943115 loggerjava-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-04 04:39:00.000000 loggerjava-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:39:07.943115 loggerjava-0.7.6/loggerjava/
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-04 04:39:00.000000 loggerjava-0.7.6/loggerjava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-04 04:39:00.000000 loggerjava-0.7.6/loggerjava/loggerjava.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-04 04:39:00.000000 loggerjava-0.7.6/loggerjava/test_loggerjava.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:39:07.943115 loggerjava-0.7.6/loggerjava.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-04 04:39:07.000000 loggerjava-0.7.6/loggerjava.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-04 04:39:07.000000 loggerjava-0.7.6/loggerjava.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:39:07.000000 loggerjava-0.7.6/loggerjava.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 04:39:07.000000 loggerjava-0.7.6/loggerjava.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-04 04:39:00.000000 loggerjava-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:39:07.943115 loggerjava-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-04 04:39:00.000000 loggerjava-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:13:03.699328 loggerjava-0.8.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-04 15:13:03.695328 loggerjava-0.8.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:13:03.695328 loggerjava-0.8.0.dev1/loggerjava/
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/loggerjava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/loggerjava/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/loggerjava/loggerjava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/loggerjava/test_loggerjava.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:13:03.695328 loggerjava-0.8.0.dev1/loggerjava.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-04 15:13:03.000000 loggerjava-0.8.0.dev1/loggerjava.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 15:13:03.000000 loggerjava-0.8.0.dev1/loggerjava.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:13:03.000000 loggerjava-0.8.0.dev1/loggerjava.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 15:13:03.000000 loggerjava-0.8.0.dev1/loggerjava.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:13:03.699328 loggerjava-0.8.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/setup.py
```

### Comparing `loggerjava-0.7.6/LICENSE` & `loggerjava-0.8.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerjava-0.7.6/PKG-INFO` & `loggerjava-0.8.0.dev1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.7.6
+Version: 0.8.0.dev1
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
+Keywords: python,logger,java_like
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -73,16 +74,39 @@
 
 :return: none
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
+
+### Exception handler
+using the `loggerjava.exceptionhandler.exception(exc)` function to process an Exception
+
+```python
+import loggerjava
+import loggerjava.exceptionhandler
+def test1(a):
+    print(b)
+if __name__ == "__main__":
+    try:
+        test1(1)
+    except Exception as E:
+        loggerjava.error(loggerjava.exceptionhandler.handler(E))
+```
+#### Output：
+```commandline
+[20:39:00] [main/ERROR]: NameError: name 'b' is not defined
+    at <module> (<input>:7)
+    at test1 (<input>:4)
+```
 ### Versions
 
+`v0.8.0` added the exceptionhandler and clearcurrentlog function
+
 `v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
 
 `v0.7.5.dev1` follow SemVer, no actual updates
 
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `loggerjava-0.7.6/README.md` & `loggerjava-0.8.0.dev1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -58,16 +58,39 @@
 
 :return: none
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
+
+### Exception handler
+using the `loggerjava.exceptionhandler.exception(exc)` function to process an Exception
+
+```python
+import loggerjava
+import loggerjava.exceptionhandler
+def test1(a):
+    print(b)
+if __name__ == "__main__":
+    try:
+        test1(1)
+    except Exception as E:
+        loggerjava.error(loggerjava.exceptionhandler.handler(E))
+```
+#### Output：
+```commandline
+[20:39:00] [main/ERROR]: NameError: name 'b' is not defined
+    at <module> (<input>:7)
+    at test1 (<input>:4)
+```
 ### Versions
 
+`v0.8.0` added the exceptionhandler and clearcurrentlog function
+
 `v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
 
 `v0.7.5.dev1` follow SemVer, no actual updates
 
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `loggerjava-0.7.6/loggerjava/__init__.py` & `loggerjava-0.8.0.dev1/loggerjava/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import time
 import loggerjava
+import loggerjava.exceptionhandler
 
 if __name__ == '__main__':
+
     pass
 
-ver = "v0.7.6"
+ver = "v0.8.0.dev1"
 name = "log"
 absolutepath = False
 showdetailedtime = False
 showinconsole = True
 fileextension = ".log"
 file_encoding = "utf-8"
 route = r"log.log"
@@ -17,44 +19,50 @@
 
 
 # noinspection PyTypeChecker
 def log(txt, type="i", pos="main", **overrides):
     """
         :param txt: the detail description of this log
         :param type: the type of the log,using:debug,info,warn,error,fatal
+        accept types:
+        debug: "D", "d", "debug"
+        info: "I", "i", "INFO", "info"
+        warn:"W", "w", "WARN", "warn"
+        error:"E", "e", "ERROR", "error"
+        fatal:"F", "f", "FATAL", "fatal"
+
         :param pos: show where the log's actual called positon in the code
         :param overrides: the overrides of the current config,only actives once
         available overrides: showinconsole , showdetailedtime
+        format: override_name = override_value
         :return: log
         """
     detailtime = showdetailedtime
     inconsole = showinconsole
     debugmodein = debugmode
     for overridename, data in overrides.items():
-        pass
         if overridename == "showdetailedtime":
-            if _formats.testformat(data,1):
+            if _formats.testformat(data, 1):
                 detailtime = data
             else:
-                log("wrong detailed time override. Set as False", type="W",pos="main_loggerjava",showinconsole=True)
+                log("wrong detailed time override. Set as False", type="W", pos="main_loggerjava", showinconsole=True)
                 detailtime = False
         elif overridename == "showinconsole":
-            if _formats.testformat(data,1):
+            if _formats.testformat(data, 1):
                 inconsole = data
             else:
                 log("wrong show in console override. Set as True", type="W", pos="main_loggerjava", showinconsole=True)
                 inconsole = True
         elif overridename == "debugmode":
-            if _formats.testformat(data,1):
+            if _formats.testformat(data, 1):
                 debugmodein = data
             else:
                 log("wrong debug override. Set as False", type="W", pos="main_loggerjava", showinconsole=True)
                 debugmodein = False
 
-
     level = _formats.typeformat(type)
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + fileextension, mode="at+", encoding=file_encoding)
     if detailtime:
         timelog = time.asctime()
@@ -63,75 +71,83 @@
     if inconsole:
         print(_formats.format(timelog, pos, level, txt))
     if not debugmodein:
         f.write(_formats.format(timelog, pos, level, txt))
         f.close()
     if debugmodein:
         return _formats.format(timelog, pos, level, txt)
-    del detailtime,inconsole,debugmodein
+    del detailtime, inconsole, debugmodein
 
 
-def debug(txt, pos="main"):
+def debug(txt, pos="main", **overrides):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
+        :param overrides: the overrides of the current config,only actives once
+        available overrides: showinconsole , showdetailedtime
         :return: debug log
         """
     if debugmode:
-        return log(txt, type='debug', pos=pos)
+        return log(txt, type='debug', pos=pos, **overrides)
     else:
-        log(txt, type='debug', pos=pos)
+        log(txt, type='debug', pos=pos, **overrides)
 
 
-def info(txt, pos="main"):
+def info(txt, pos="main", **overrides):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :return: info log
         """
     if debugmode:
-        return log(txt, type='INFO', pos=pos)
+        return log(txt, type='INFO', pos=pos, **overrides)
     else:
-        log(txt, type='INFO', pos=pos)
+        log(txt, type='INFO', pos=pos, **overrides)
 
 
-def warn(txt, pos="main"):
+def warn(txt, pos="main", **overrides):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
+        :param overrides: the overrides of the current config,only actives once
+        available overrides: showinconsole , showdetailedtime
         :return: warning log
         """
     if debugmode:
-        return log(txt, type='WARN', pos=pos)
+        return log(txt, type='WARN', pos=pos, **overrides)
     else:
-        log(txt, type='WARN', pos=pos)
+        log(txt, type='WARN', pos=pos, **overrides)
 
 
-def error(txt, pos="main"):
+def error(txt, pos="main", **overrides):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
+        :param overrides: the overrides of the current config,only actives once
+        available overrides: showinconsole , showdetailedtime
         :return: error log
         """
     if debugmode:
-        return log(txt, type='ERROR', pos=pos)
+        return log(txt, type='ERROR', pos=pos, **overrides)
     else:
-        log(txt, type='ERROR', pos=pos)
+        log(txt, type='ERROR', pos=pos, **overrides)
 
 
-def fatal(txt, pos="main"):
+def fatal(txt, pos="main", **overrides):
     """
-    :param txt: the detail description of this log
-    :param pos: show where the log's actual called positon in the code
-    :return: fatal log
+        :param txt: the detail description of this log
+        :param pos: show where the log's actual called positon in the code
+        :param overrides: the overrides of the current config,only actives once
+        available overrides: showinconsole , showdetailedtime
+        :return: fatal log
     """
     if debugmode:
-        return log(txt, type='FATAL', pos=pos)
+        return log(txt, type='FATAL', pos=pos, **overrides)
     else:
-        log(txt, type='FATAL', pos=pos)
+        log(txt, type='FATAL', pos=pos, **overrides)
     if fatalclose:
         exit(10)
 
 
 def config(**kwargs):
     """
     :param kwargs:input config names and config data
@@ -141,18 +157,19 @@
 
     name : change the name of the log file, only actives when abolutepath config is off
 
     fileextension : change the extension of the log file, only actives when abolutepath config is off
 
     absolutepath : change whether inputing the absolute path of the log file,
     True for using the name and fileextension to create file in the program running location
-    False for using the route to create file in the specific location(note:you need to enter the file format,like:test.log)
+    False for using the route to create file in the specific location
+    (note:the route should contain the extension of the file,like:D:\test.log)
 
     route : change the file location, only activates when abolutepath config is on
-    the route should contain the
+    the route should contain the extension of the file
 
     file_encoding : change the file encoding method
 
     showdetailedtime : whether to show detailed time in the log file
 
     showinconsole : whether to show the log in the python console
 
@@ -189,61 +206,70 @@
                 del tmpf
                 if absolutepath:
                     f = open(route, mode="w", encoding=file_encoding)
                 else:
                     f = open(name + fileextension, mode="w", encoding=file_encoding)
                 f.close()
             except LookupError:
-                warn("wrong file encoding config.this config is set to normal", pos="main_loggerjava")
+                warn("wrong file encoding config.this config is set to default", pos="main_loggerjava",
+                     showinconsole=True)
                 file_encoding = "utf-8"
 
         elif configname == "showdetailedtime":
             if _formats.testformat(configdata, 1):
                 showdetailedtime = configdata
             else:
-                tmpin = showinconsole
-                showinconsole = True
-                warn("wrong detailed time config.this config is set to normal", pos="main_loggerjava")
-                showinconsole = tmpin
+                warn("wrong detailed time config.this config is set to default", pos="main_loggerjava",
+                     showinconsole=True)
                 showdetailedtime = False
-                del tmpin
 
         elif configname == "showinconsole":
             if _formats.testformat(configdata, 1):
                 showinconsole = configdata
             else:
                 showinconsole = True
-                warn("wrong show in console config.this config is set to normal", pos="main_loggerjava")
+                warn("wrong show in console config.this config is set to default", pos="main_loggerjava",
+                     showinconsole=True)
 
         elif configname == "absolutepath":
             if _formats.testformat(configdata, 1):
                 absolutepath = configdata
                 if absolutepath:
                     f = open(route, mode="w", encoding=file_encoding)
                 else:
                     f = open(name + fileextension, mode="w", encoding=file_encoding)
                 f.close()
             else:
-                tmpin = showinconsole
-                showinconsole = True
-                warn("wrong absolute path config.this config is set to normal", pos="main_loggerjava")
-                showinconsole = tmpin
+                warn("wrong absolute path config.this config is set to default", pos="main_loggerjava",
+                     showinconsole=True)
                 absolutepath = False
                 f = open(name + fileextension, mode="w", encoding=file_encoding)
                 f.close()
-                del tmpin
         elif configname == "debugmode":
             debugmode = configdata
         elif configname == "fatalexit":
             if _formats.testformat(configdata, 1):
                 fatalclose = configdata
             else:
-                warn("wrong fatal exit config.this config is set to normal", pos="main_loggerjava")
+                warn("wrong fatal exit config.this config is set to default", pos="main_loggerjava", showinconsole=True)
                 fatalclose = False
-        #log("all given configs modified",type="D",pos="main_loggerjava.config",showinconsole=False)
+        # log("all given configs modified",type="D",pos="main_loggerjava.config",showinconsole=False)
+
+
+def clearcurrentlog():
+    """
+    clean the current log file
+    :return: nothing
+    """
+    if absolutepath:
+        f = open(route, mode="w", encoding=file_encoding)
+    else:
+        f = open(name + fileextension, mode="w", encoding=file_encoding)
+    f.write("")
+    f.close()
 
 
 def version():
     """
     show the current version of loggerjava
     :return:
     """
@@ -273,76 +299,64 @@
     :return:
     """
     global name, showdetailedtime, showinconsole, absolutepath, fileextension, file_encoding, route, fatalclose
 
     if _formats.testformat(inputconfig["absolutepath"], 1):
         absolutepath = inputconfig["absolutepath"]
     else:
-        tmpin = showinconsole
-        showinconsole = True
-        warn("wrong absolute path config.this config is set to normal", pos="main_loggerjava")
-        showinconsole = tmpin
+        warn("wrong absolute path config.this config is set to default", pos="main_loggerjava", showinconsole=True)
         absolutepath = False
-        del tmpin
 
     name = inputconfig["name"]
     fileextension = inputconfig["fileextension"]
     route = inputconfig["route"]
 
     try:
         if absolutepath:
             tmpf = open(route, mode="w", encoding=inputconfig["file_encoding"])
         else:
             tmpf = open(name + fileextension, mode="w", encoding=inputconfig["file_encoding"])
         tmpf.close()
         file_encoding = inputconfig["file_encoding"]
         del tmpf
     except LookupError:
-        warn("wrong file encoding config.this config is set to normal", pos="main_loggerjava")
+        warn("wrong file encoding config.this config is set to default", pos="main_loggerjava", showinconsole=True)
         file_encoding = "utf-8"
 
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + fileextension, mode="at+", encoding=file_encoding)
     f.close()
 
     if _formats.testformat(inputconfig["showdetailedtime"], 1):
         showdetailedtime = inputconfig["showdetailedtime"]
     else:
-        tmpin = showinconsole
-        showinconsole = True
-        warn("wrong detailed time config.this config is set to normal", pos="main_loggerjava")
-        showinconsole = tmpin
+        warn("wrong detailed time config.this config is set to default", pos="main_loggerjava", showinconsole=True)
         showdetailedtime = False
-        del tmpin
 
     if _formats.testformat(inputconfig["showinconsole"], 1):
         showinconsole = inputconfig["showinconsole"]
     else:
         showinconsole = True
-        warn("wrong show in console config.this config is set to normal", pos="main_loggerjava")
+        warn("wrong show in console config.this config is set to default", pos="main_loggerjava", showinconsole=True)
 
     if _formats.testformat(inputconfig["fatalexit"], 1):
         fatalclose = inputconfig["fatalexit"]
     else:
         fatalclose = False
-        tmpin = showinconsole
-        showinconsole = True
-        warn("wrong fatal close config.this config is set to normal", pos="main_loggerjava")
-        showinconsole = tmpin
-        del tmpin
+        warn("wrong fatal close config.this config is set to default", pos="main_loggerjava", showinconsole=True)
 
 
 # noinspection PyMethodParameters
 
 
 class _formats:
     def typeformat(type):
-        debugformat = ["D", "d", "DEBUG", "debug"]
+        debugformat = ["D", "d", "debug"]
         infoformat = ["I", "i", "INFO", "info"]
         warnformat = ["W", "w", "WARN", "warn"]
         errorformat = ["E", "e", "ERROR", "error"]
         fatalformat = ["F", "f", "FATAL", "fatal"]
 
         if type in debugformat:
             return "debug"
@@ -351,15 +365,15 @@
         elif type in warnformat:
             return "WARN"
         elif type in errorformat:
             return "ERROR"
         elif type in fatalformat:
             return "FATAL"
         else:
-            warn("unknown given format", pos="main_loggerjava")
+            warn("unknown given format", pos="main_loggerjava", showinconsole=True)
             return "WARN"
 
     def testformat(name, type):
         if type == 1:
             if name or not name:
                 return True
             else:
```

### Comparing `loggerjava-0.7.6/loggerjava/loggerjava.py` & `loggerjava-0.8.0.dev1/loggerjava/loggerjava.py`

 * *Files identical despite different names*

### Comparing `loggerjava-0.7.6/loggerjava/test_loggerjava.py` & `loggerjava-0.8.0.dev1/loggerjava/test_loggerjava.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,12 +38,14 @@
            str(time.localtime().tm_min).rjust(2, "0") + ":" + str(time.localtime().tm_sec).rjust(2,
                                                                                                  "0") + "] [testing/INFO]: test6\n"
     logger.config(name="test")
     assert logger.name == "test"
     logger.config(showdetailedtime=True)
     assert logger.info("test8") == "[" + time.asctime() + "] [main/INFO]: test8\n"
     logger.config(showdetailedtime=False)
-    assert logger.log("testoverride",type="d",showdetailedtime=True) == "[" + time.asctime() + "] [main/debug]: testoverride\n"
+    assert logger.log("testoverride", type="d",
+                      showdetailedtime=True) == "[" + time.asctime() + "] [main/debug]: testoverride\n"
+    assert logger.warn("testoverride", showdetailedtime=True) == "[" + time.asctime() + "] [main/WARN]: testoverride\n"
 
 
 if __name__ == "__main__":
     testin()
```

### Comparing `loggerjava-0.7.6/loggerjava.egg-info/PKG-INFO` & `loggerjava-0.8.0.dev1/loggerjava.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.7.6
+Version: 0.8.0.dev1
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
+Keywords: python,logger,java_like
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -73,16 +74,39 @@
 
 :return: none
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
+
+### Exception handler
+using the `loggerjava.exceptionhandler.exception(exc)` function to process an Exception
+
+```python
+import loggerjava
+import loggerjava.exceptionhandler
+def test1(a):
+    print(b)
+if __name__ == "__main__":
+    try:
+        test1(1)
+    except Exception as E:
+        loggerjava.error(loggerjava.exceptionhandler.handler(E))
+```
+#### Output：
+```commandline
+[20:39:00] [main/ERROR]: NameError: name 'b' is not defined
+    at <module> (<input>:7)
+    at test1 (<input>:4)
+```
 ### Versions
 
+`v0.8.0` added the exceptionhandler and clearcurrentlog function
+
 `v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
 
 `v0.7.5.dev1` follow SemVer, no actual updates
 
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `loggerjava-0.7.6/setup.py` & `loggerjava-0.8.0.dev1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     author="HTony03",
     author_email="HTony03@foxmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[],
-    keywords=['python','logger'],
+    keywords=["python","logger","java_like"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

