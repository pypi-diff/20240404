# Comparing `tmp/loggerjava-0.7.5.dev1.tar.gz` & `tmp/loggerjava-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerjava-0.7.5.dev1.tar", last modified: Wed Apr  3 15:11:40 2024, max compression
+gzip compressed data, was "loggerjava-0.7.6.tar", last modified: Thu Apr  4 04:39:07 2024, max compression
```

## Comparing `loggerjava-0.7.5.dev1.tar` & `loggerjava-0.7.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/loggerjava/
--rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/loggerjava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/loggerjava/loggerjava.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/loggerjava/test_loggerjava.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/loggerjava.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-03 15:11:40.000000 loggerjava-0.7.5.dev1/loggerjava.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 15:11:40.000000 loggerjava-0.7.5.dev1/loggerjava.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:11:40.000000 loggerjava-0.7.5.dev1/loggerjava.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 15:11:40.000000 loggerjava-0.7.5.dev1/loggerjava.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:11:40.374334 loggerjava-0.7.5.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-03 15:11:34.000000 loggerjava-0.7.5.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:39:07.943115 loggerjava-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 04:39:00.000000 loggerjava-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-04 04:39:07.943115 loggerjava-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-04 04:39:00.000000 loggerjava-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:39:07.943115 loggerjava-0.7.6/loggerjava/
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-04-04 04:39:00.000000 loggerjava-0.7.6/loggerjava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-04 04:39:00.000000 loggerjava-0.7.6/loggerjava/loggerjava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-04 04:39:00.000000 loggerjava-0.7.6/loggerjava/test_loggerjava.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 04:39:07.943115 loggerjava-0.7.6/loggerjava.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-04-04 04:39:07.000000 loggerjava-0.7.6/loggerjava.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-04 04:39:07.000000 loggerjava-0.7.6/loggerjava.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 04:39:07.000000 loggerjava-0.7.6/loggerjava.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 04:39:07.000000 loggerjava-0.7.6/loggerjava.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-04 04:39:00.000000 loggerjava-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 04:39:07.943115 loggerjava-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-04 04:39:00.000000 loggerjava-0.7.6/setup.py
```

### Comparing `loggerjava-0.7.5.dev1/LICENSE` & `loggerjava-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerjava-0.7.5.dev1/PKG-INFO` & `loggerjava-0.7.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.7.5.dev1
+Version: 0.7.6
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,15 @@
 an easy logger outputs like java logs
 ### How to use
 ```python
 import loggerjava
 logger = loggerjava
 logger.info("test")
 logger.warn("test",pos="insidecommand")
+logger.log("test",type="w",pos="main_test",showinconsole=False)
 ```
 
 ### Outputs
 ```commandline
 [20:39:00] [main/debug]: test
 [20:39:00] [main/info]: test
 [20:39:00] [main/WARNING]: test
@@ -34,53 +35,56 @@
 [20:39:00] [main/FATAL]: test
 ```
 
 ### Developing features
 - [ ] mutiple variable with different configs
 - [x] new config format
 - [ ] catch and format errors
-- [ ] override config once
+- [X] override config once
 
 
 ### Config
 ```python
 import loggerjava
 loggerjava.config(**kwargs)
 """
 :param kwargs:input config names and config data
 format: config_name = config_data
 
 below are config_name and the description
 
 name : change the name of the log file, only actives when abolutepath config is off
 
-filetype : change the file type of the log file, only actives when abolutepath config is off
+fileextension : change the extension of the log file, only actives when abolutepath config is off
 
 absolutepath : change whether inputing the absolute path of the log file,
-True for using the name and filetype to create file in the program running location
+True for using the name and fileextension to create file in the program running location
 False for using the route to create file in the specific location(note:you need to enter the file format,like:test.log)
 
 route : change the file location, only activates when abolutepath config is on
+the route should contain the
 
 file_encoding : change the file encoding method
 
 showdetailedtime : whether to show detailed time in the log file
 
 showinconsole : whether to show the log in the python console
 
 fatalexit : whether to exit the program after a fatal log
 
-:return:
+:return: none
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
+
 `v0.7.5.dev1` follow SemVer, no actual updates
 
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
```

### Comparing `loggerjava-0.7.5.dev1/README.md` & `loggerjava-0.7.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 an easy logger outputs like java logs
 ### How to use
 ```python
 import loggerjava
 logger = loggerjava
 logger.info("test")
 logger.warn("test",pos="insidecommand")
+logger.log("test",type="w",pos="main_test",showinconsole=False)
 ```
 
 ### Outputs
 ```commandline
 [20:39:00] [main/debug]: test
 [20:39:00] [main/info]: test
 [20:39:00] [main/WARNING]: test
@@ -19,53 +20,56 @@
 [20:39:00] [main/FATAL]: test
 ```
 
 ### Developing features
 - [ ] mutiple variable with different configs
 - [x] new config format
 - [ ] catch and format errors
-- [ ] override config once
+- [X] override config once
 
 
 ### Config
 ```python
 import loggerjava
 loggerjava.config(**kwargs)
 """
 :param kwargs:input config names and config data
 format: config_name = config_data
 
 below are config_name and the description
 
 name : change the name of the log file, only actives when abolutepath config is off
 
-filetype : change the file type of the log file, only actives when abolutepath config is off
+fileextension : change the extension of the log file, only actives when abolutepath config is off
 
 absolutepath : change whether inputing the absolute path of the log file,
-True for using the name and filetype to create file in the program running location
+True for using the name and fileextension to create file in the program running location
 False for using the route to create file in the specific location(note:you need to enter the file format,like:test.log)
 
 route : change the file location, only activates when abolutepath config is on
+the route should contain the
 
 file_encoding : change the file encoding method
 
 showdetailedtime : whether to show detailed time in the log file
 
 showinconsole : whether to show the log in the python console
 
 fatalexit : whether to exit the program after a fatal log
 
-:return:
+:return: none
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
+
 `v0.7.5.dev1` follow SemVer, no actual updates
 
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
```

### Comparing `loggerjava-0.7.5.dev1/loggerjava/__init__.py` & `loggerjava-0.7.6/loggerjava/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,113 +1,134 @@
 import time
 import loggerjava
 
 if __name__ == '__main__':
     pass
 
-ver = "v0.7.5.dev1"
+ver = "v0.7.6"
 name = "log"
 absolutepath = False
 showdetailedtime = False
 showinconsole = True
-filetype = ".log"
+fileextension = ".log"
 file_encoding = "utf-8"
 route = r"log.log"
-debugin = False
+debugmode = False
 fatalclose = False
 
 
 # noinspection PyTypeChecker
 def log(txt, type="i", pos="main", **overrides):
     """
         :param txt: the detail description of this log
         :param type: the type of the log,using:debug,info,warn,error,fatal
         :param pos: show where the log's actual called positon in the code
+        :param overrides: the overrides of the current config,only actives once
+        available overrides: showinconsole , showdetailedtime
         :return: log
         """
-    for configname, configdata in overrides.items():
+    detailtime = showdetailedtime
+    inconsole = showinconsole
+    debugmodein = debugmode
+    for overridename, data in overrides.items():
         pass
+        if overridename == "showdetailedtime":
+            if _formats.testformat(data,1):
+                detailtime = data
+            else:
+                log("wrong detailed time override. Set as False", type="W",pos="main_loggerjava",showinconsole=True)
+                detailtime = False
+        elif overridename == "showinconsole":
+            if _formats.testformat(data,1):
+                inconsole = data
+            else:
+                log("wrong show in console override. Set as True", type="W", pos="main_loggerjava", showinconsole=True)
+                inconsole = True
+        elif overridename == "debugmode":
+            if _formats.testformat(data,1):
+                debugmodein = data
+            else:
+                log("wrong debug override. Set as False", type="W", pos="main_loggerjava", showinconsole=True)
+                debugmodein = False
+
+
     level = _formats.typeformat(type)
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
-        f = open(name + filetype, mode="at+", encoding=file_encoding)
-    if showdetailedtime and showinconsole:
-        # noinspection PyTypeChecker
-        f.write(_formats.format(time.asctime(), pos, level, txt))
-        print(_formats.format(time.asctime(), pos, level, txt))
-    elif not showdetailedtime and showinconsole:
-        f.write(_formats.format(_formats.time1(), pos, level, txt))
-        print(_formats.format(_formats.time1(), pos, level, txt))
-    elif showdetailedtime and not showinconsole:
-        f.write(_formats.format(time.asctime(), pos, level, txt))
+        f = open(name + fileextension, mode="at+", encoding=file_encoding)
+    if detailtime:
+        timelog = time.asctime()
     else:
-        f.write(_formats.format(_formats.time1(), pos, level, txt))
-    if debugin and not showdetailedtime:
-        return _formats.format(_formats.time1(), pos, level, txt)
-    elif debugin and showdetailedtime:
-        return _formats.format(time.asctime(), pos, level, txt)
-    f.close()
+        timelog = _formats.time1()
+    if inconsole:
+        print(_formats.format(timelog, pos, level, txt))
+    if not debugmodein:
+        f.write(_formats.format(timelog, pos, level, txt))
+        f.close()
+    if debugmodein:
+        return _formats.format(timelog, pos, level, txt)
+    del detailtime,inconsole,debugmodein
 
 
 def debug(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :return: debug log
         """
-    if debugin:
+    if debugmode:
         return log(txt, type='debug', pos=pos)
     else:
         log(txt, type='debug', pos=pos)
 
 
 def info(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :return: info log
         """
-    if debugin:
+    if debugmode:
         return log(txt, type='INFO', pos=pos)
     else:
-        return log(txt, type='INFO', pos=pos)
+        log(txt, type='INFO', pos=pos)
 
 
 def warn(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :return: warning log
         """
-    if debugin:
+    if debugmode:
         return log(txt, type='WARN', pos=pos)
     else:
         log(txt, type='WARN', pos=pos)
 
 
 def error(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :return: error log
         """
-    if debugin:
+    if debugmode:
         return log(txt, type='ERROR', pos=pos)
     else:
         log(txt, type='ERROR', pos=pos)
 
 
 def fatal(txt, pos="main"):
     """
     :param txt: the detail description of this log
     :param pos: show where the log's actual called positon in the code
     :return: fatal log
     """
-    if debugin:
+    if debugmode:
         return log(txt, type='FATAL', pos=pos)
     else:
         log(txt, type='FATAL', pos=pos)
     if fatalclose:
         exit(10)
 
 
@@ -116,63 +137,64 @@
     :param kwargs:input config names and config data
     format: config_name = config_data
 
     below are config_name and the description
 
     name : change the name of the log file, only actives when abolutepath config is off
 
-    filetype : change the file type of the log file, only actives when abolutepath config is off
+    fileextension : change the extension of the log file, only actives when abolutepath config is off
 
     absolutepath : change whether inputing the absolute path of the log file,
-    True for using the name and filetype to create file in the program running location
+    True for using the name and fileextension to create file in the program running location
     False for using the route to create file in the specific location(note:you need to enter the file format,like:test.log)
 
     route : change the file location, only activates when abolutepath config is on
+    the route should contain the
 
     file_encoding : change the file encoding method
 
     showdetailedtime : whether to show detailed time in the log file
 
     showinconsole : whether to show the log in the python console
 
     fatalexit : whether to exit the program after a fatal log
 
-    :return:
+    :return: none
     """
-    global showinconsole, showdetailedtime, absolutepath, name, filetype, file_encoding, route, debugin, fatalclose
+    global showinconsole, showdetailedtime, absolutepath, name, fileextension, file_encoding, route, debugmode, fatalclose
     for configname, configdata in kwargs.items():
 
         if configname == "name":
             name = configdata
-            f = open(name + filetype, mode="w", encoding=file_encoding)
+            f = open(name + fileextension, mode="w", encoding=file_encoding)
             f.close()
 
-        elif configname == "filetype":
-            filetype = configdata
-            f = open(name + filetype, mode="w", encoding=file_encoding)
+        elif configname == "fileextension":
+            fileextension = configdata
+            f = open(name + fileextension, mode="w", encoding=file_encoding)
             f.close()
 
         elif configname == "route":
             route = configdata
             f = open(route, mode="w", encoding=file_encoding)
             f.close()
 
         elif configname == "file_encoding":
             try:
                 if absolutepath:
                     tmpf = open(route, mode="w", encoding=configname)
                 else:
-                    tmpf = open(name + filetype, mode="w", encoding=configname)
+                    tmpf = open(name + fileextension, mode="w", encoding=configname)
                 tmpf.close()
                 file_encoding = configname
                 del tmpf
                 if absolutepath:
                     f = open(route, mode="w", encoding=file_encoding)
                 else:
-                    f = open(name + filetype, mode="w", encoding=file_encoding)
+                    f = open(name + fileextension, mode="w", encoding=file_encoding)
                 f.close()
             except LookupError:
                 warn("wrong file encoding config.this config is set to normal", pos="main_loggerjava")
                 file_encoding = "utf-8"
 
         elif configname == "showdetailedtime":
             if _formats.testformat(configdata, 1):
@@ -194,33 +216,34 @@
 
         elif configname == "absolutepath":
             if _formats.testformat(configdata, 1):
                 absolutepath = configdata
                 if absolutepath:
                     f = open(route, mode="w", encoding=file_encoding)
                 else:
-                    f = open(name + filetype, mode="w", encoding=file_encoding)
+                    f = open(name + fileextension, mode="w", encoding=file_encoding)
                 f.close()
             else:
                 tmpin = showinconsole
                 showinconsole = True
                 warn("wrong absolute path config.this config is set to normal", pos="main_loggerjava")
                 showinconsole = tmpin
                 absolutepath = False
-                f = open(name + filetype, mode="w", encoding=file_encoding)
+                f = open(name + fileextension, mode="w", encoding=file_encoding)
                 f.close()
                 del tmpin
-        elif configname == "debuging":
-            debugin = configdata
+        elif configname == "debugmode":
+            debugmode = configdata
         elif configname == "fatalexit":
             if _formats.testformat(configdata, 1):
                 fatalclose = configdata
             else:
                 warn("wrong fatal exit config.this config is set to normal", pos="main_loggerjava")
                 fatalclose = False
+        #log("all given configs modified",type="D",pos="main_loggerjava.config",showinconsole=False)
 
 
 def version():
     """
     show the current version of loggerjava
     :return:
     """
@@ -234,57 +257,57 @@
 def exportconfig():
     """
     export current config
     use loadconfig(config) to load this exported config
     returning as a lib
     :return:
     """
-    i = {"name": name, "filetype": filetype, "absolutepath": absolutepath,
+    i = {"name": name, "fileextension": fileextension, "absolutepath": absolutepath,
          "route": route, "showdetailedtime": showdetailedtime, "showinconsole": showinconsole,
          "file_encoding": file_encoding, "fatalexit": fatalclose}
     return i
 
 
 def loadconfig(inputconfig):
     """
     :param inputconfig: the config lib exported from exportconfig()
     :return:
     """
-    global name, showdetailedtime, showinconsole, absolutepath, filetype, file_encoding, route, fatalclose
+    global name, showdetailedtime, showinconsole, absolutepath, fileextension, file_encoding, route, fatalclose
 
     if _formats.testformat(inputconfig["absolutepath"], 1):
         absolutepath = inputconfig["absolutepath"]
     else:
         tmpin = showinconsole
         showinconsole = True
         warn("wrong absolute path config.this config is set to normal", pos="main_loggerjava")
         showinconsole = tmpin
         absolutepath = False
         del tmpin
 
     name = inputconfig["name"]
-    filetype = inputconfig["filetype"]
+    fileextension = inputconfig["fileextension"]
     route = inputconfig["route"]
 
     try:
         if absolutepath:
             tmpf = open(route, mode="w", encoding=inputconfig["file_encoding"])
         else:
-            tmpf = open(name + filetype, mode="w", encoding=inputconfig["file_encoding"])
+            tmpf = open(name + fileextension, mode="w", encoding=inputconfig["file_encoding"])
         tmpf.close()
         file_encoding = inputconfig["file_encoding"]
         del tmpf
     except LookupError:
         warn("wrong file encoding config.this config is set to normal", pos="main_loggerjava")
         file_encoding = "utf-8"
 
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
-        f = open(name + filetype, mode="at+", encoding=file_encoding)
+        f = open(name + fileextension, mode="at+", encoding=file_encoding)
     f.close()
 
     if _formats.testformat(inputconfig["showdetailedtime"], 1):
         showdetailedtime = inputconfig["showdetailedtime"]
     else:
         tmpin = showinconsole
         showinconsole = True
```

### Comparing `loggerjava-0.7.5.dev1/loggerjava/loggerjava.py` & `loggerjava-0.7.6/loggerjava/loggerjava.py`

 * *Files identical despite different names*

### Comparing `loggerjava-0.7.5.dev1/loggerjava/test_loggerjava.py` & `loggerjava-0.7.6/loggerjava/test_loggerjava.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 if __name__ == '__main__':
     unittest.main()
 """
 
 
 def testin():
     logger = lj
-    logger.config(debuging=True, showdetailedtime=False)
+    logger.config(debugmode=True, showdetailedtime=False)
     print("\n")
     assert logger.info("test1") == "[" + str(time.localtime().tm_hour).rjust(2, "0") + ":" + \
            str(time.localtime().tm_min).rjust(2, "0") + ":" + str(time.localtime().tm_sec).rjust(2,
                                                                                                  "0") + "] [main/INFO]: test1\n"
     assert logger.debug("test2") == "[" + str(time.localtime().tm_hour).rjust(2, "0") + ":" + \
            str(time.localtime().tm_min).rjust(2, "0") + ":" + str(time.localtime().tm_sec).rjust(2,
                                                                                                  "0") + "] [main/debug]: test2\n"
@@ -37,11 +37,13 @@
     assert logger.info("test6", pos="testing") == "[" + str(time.localtime().tm_hour).rjust(2, "0") + ":" + \
            str(time.localtime().tm_min).rjust(2, "0") + ":" + str(time.localtime().tm_sec).rjust(2,
                                                                                                  "0") + "] [testing/INFO]: test6\n"
     logger.config(name="test")
     assert logger.name == "test"
     logger.config(showdetailedtime=True)
     assert logger.info("test8") == "[" + time.asctime() + "] [main/INFO]: test8\n"
+    logger.config(showdetailedtime=False)
+    assert logger.log("testoverride",type="d",showdetailedtime=True) == "[" + time.asctime() + "] [main/debug]: testoverride\n"
 
 
 if __name__ == "__main__":
     testin()
```

### Comparing `loggerjava-0.7.5.dev1/loggerjava.egg-info/PKG-INFO` & `loggerjava-0.7.6/loggerjava.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.7.5.dev1
+Version: 0.7.6
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,14 +19,15 @@
 an easy logger outputs like java logs
 ### How to use
 ```python
 import loggerjava
 logger = loggerjava
 logger.info("test")
 logger.warn("test",pos="insidecommand")
+logger.log("test",type="w",pos="main_test",showinconsole=False)
 ```
 
 ### Outputs
 ```commandline
 [20:39:00] [main/debug]: test
 [20:39:00] [main/info]: test
 [20:39:00] [main/WARNING]: test
@@ -34,53 +35,56 @@
 [20:39:00] [main/FATAL]: test
 ```
 
 ### Developing features
 - [ ] mutiple variable with different configs
 - [x] new config format
 - [ ] catch and format errors
-- [ ] override config once
+- [X] override config once
 
 
 ### Config
 ```python
 import loggerjava
 loggerjava.config(**kwargs)
 """
 :param kwargs:input config names and config data
 format: config_name = config_data
 
 below are config_name and the description
 
 name : change the name of the log file, only actives when abolutepath config is off
 
-filetype : change the file type of the log file, only actives when abolutepath config is off
+fileextension : change the extension of the log file, only actives when abolutepath config is off
 
 absolutepath : change whether inputing the absolute path of the log file,
-True for using the name and filetype to create file in the program running location
+True for using the name and fileextension to create file in the program running location
 False for using the route to create file in the specific location(note:you need to enter the file format,like:test.log)
 
 route : change the file location, only activates when abolutepath config is on
+the route should contain the
 
 file_encoding : change the file encoding method
 
 showdetailedtime : whether to show detailed time in the log file
 
 showinconsole : whether to show the log in the python console
 
 fatalexit : whether to exit the program after a fatal log
 
-:return:
+:return: none
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
+
 `v0.7.5.dev1` follow SemVer, no actual updates
 
 `v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
 
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
```

### Comparing `loggerjava-0.7.5.dev1/setup.py` & `loggerjava-0.7.6/setup.py`

 * *Files identical despite different names*

