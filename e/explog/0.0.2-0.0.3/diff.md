# Comparing `tmp/explog-0.0.2.tar.gz` & `tmp/explog-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "explog-0.0.2.tar", last modified: Sun Mar 24 13:41:47 2024, max compression
+gzip compressed data, was "explog-0.0.3.tar", last modified: Thu Apr  4 07:19:06 2024, max compression
```

## Comparing `explog-0.0.2.tar` & `explog-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gsprd      (501) staff       (20)        0 2024-03-24 13:41:47.821410 explog-0.0.2/
--rw-r--r--   0 gsprd      (501) staff       (20)     1062 2024-03-21 16:55:05.000000 explog-0.0.2/LICENSE
--rw-r--r--   0 gsprd      (501) staff       (20)     2999 2024-03-24 13:41:47.821211 explog-0.0.2/PKG-INFO
--rw-r--r--   0 gsprd      (501) staff       (20)     2485 2024-03-24 13:38:08.000000 explog-0.0.2/README.md
-drwxr-xr-x   0 gsprd      (501) staff       (20)        0 2024-03-24 13:41:47.820155 explog-0.0.2/explog/
--rw-r--r--   0 gsprd      (501) staff       (20)      126 2024-03-24 11:55:06.000000 explog-0.0.2/explog/__init__.py
--rw-r--r--   0 gsprd      (501) staff       (20)     4796 2024-03-24 11:55:26.000000 explog-0.0.2/explog/logger.py
-drwxr-xr-x   0 gsprd      (501) staff       (20)        0 2024-03-24 13:41:47.821030 explog-0.0.2/explog.egg-info/
--rw-r--r--   0 gsprd      (501) staff       (20)     2999 2024-03-24 13:41:47.000000 explog-0.0.2/explog.egg-info/PKG-INFO
--rw-r--r--   0 gsprd      (501) staff       (20)      217 2024-03-24 13:41:47.000000 explog-0.0.2/explog.egg-info/SOURCES.txt
--rw-r--r--   0 gsprd      (501) staff       (20)        1 2024-03-24 13:41:47.000000 explog-0.0.2/explog.egg-info/dependency_links.txt
--rw-r--r--   0 gsprd      (501) staff       (20)        7 2024-03-24 13:41:47.000000 explog-0.0.2/explog.egg-info/requires.txt
--rw-r--r--   0 gsprd      (501) staff       (20)        7 2024-03-24 13:41:47.000000 explog-0.0.2/explog.egg-info/top_level.txt
--rw-r--r--   0 gsprd      (501) staff       (20)      636 2024-03-24 13:40:54.000000 explog-0.0.2/pyproject.toml
--rw-r--r--   0 gsprd      (501) staff       (20)       38 2024-03-24 13:41:47.821453 explog-0.0.2/setup.cfg
+drwxr-xr-x   0 gsprd      (501) staff       (20)        0 2024-04-04 07:19:06.086815 explog-0.0.3/
+-rw-r--r--   0 gsprd      (501) staff       (20)     1062 2024-03-24 13:42:21.000000 explog-0.0.3/LICENSE
+-rw-r--r--   0 gsprd      (501) staff       (20)     3000 2024-04-04 07:19:06.086600 explog-0.0.3/PKG-INFO
+-rw-r--r--   0 gsprd      (501) staff       (20)     2486 2024-03-24 14:14:13.000000 explog-0.0.3/README.md
+drwxr-xr-x   0 gsprd      (501) staff       (20)        0 2024-04-04 07:19:06.085515 explog-0.0.3/explog/
+-rw-r--r--   0 gsprd      (501) staff       (20)      126 2024-03-24 13:42:33.000000 explog-0.0.3/explog/__init__.py
+-rw-r--r--   0 gsprd      (501) staff       (20)     5020 2024-04-04 07:14:44.000000 explog-0.0.3/explog/logger.py
+drwxr-xr-x   0 gsprd      (501) staff       (20)        0 2024-04-04 07:19:06.086400 explog-0.0.3/explog.egg-info/
+-rw-r--r--   0 gsprd      (501) staff       (20)     3000 2024-04-04 07:19:06.000000 explog-0.0.3/explog.egg-info/PKG-INFO
+-rw-r--r--   0 gsprd      (501) staff       (20)      217 2024-04-04 07:19:06.000000 explog-0.0.3/explog.egg-info/SOURCES.txt
+-rw-r--r--   0 gsprd      (501) staff       (20)        1 2024-04-04 07:19:06.000000 explog-0.0.3/explog.egg-info/dependency_links.txt
+-rw-r--r--   0 gsprd      (501) staff       (20)        7 2024-04-04 07:19:06.000000 explog-0.0.3/explog.egg-info/requires.txt
+-rw-r--r--   0 gsprd      (501) staff       (20)        7 2024-04-04 07:19:06.000000 explog-0.0.3/explog.egg-info/top_level.txt
+-rw-r--r--   0 gsprd      (501) staff       (20)      636 2024-04-04 07:18:24.000000 explog-0.0.3/pyproject.toml
+-rw-r--r--   0 gsprd      (501) staff       (20)       38 2024-04-04 07:19:06.086861 explog-0.0.3/setup.cfg
```

### Comparing `explog-0.0.2/LICENSE` & `explog-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `explog-0.0.2/PKG-INFO` & `explog-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: explog
-Version: 0.0.2
+Version: 0.0.3
 Summary: Experiment Logger
 Author-email: Gaspard Lambrechts <gsprd@protonmail.com>
 Project-URL: Homepage, https://github.com/glambrechts/explog
 Project-URL: Issues, https://github.com/glambrechts/explog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 
-# ExpLog - A Minimal Experiment Logger
+# Exp Log - A Minimal Experiment Logger
 
 ## Installation
 
 ```sh
 pip install explog
 ```
```

### Comparing `explog-0.0.2/README.md` & `explog-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ExpLog - A Minimal Experiment Logger
+# Exp Log - A Minimal Experiment Logger
 
 ## Installation
 
 ```sh
 pip install explog
 ```
```

### Comparing `explog-0.0.2/explog/logger.py` & `explog-0.0.3/explog/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import datetime as dt
 
 from pathlib import Path
 
 
 EXPS_DIRECTORY = Path("exps")
 FORMAT = "[a-zA-Z][a-zA-Z0-9_/]*"
-INFOS = ['_id', '_step', '_start']
+INFOS = ["_id", "_step", "_start"]
 
 
 def _identifier(n):
     """
     Sample a random identifier.
     """
-    return ''.join(random.choices(string.ascii_lowercase + string.digits, k=n))
+    return "".join(random.choices(string.ascii_lowercase + string.digits, k=n))
 
 
 def exp(*args, **kwargs):
     """
     Initialize an experiment.
     """
     return Experiment(*args, **kwargs)
@@ -48,47 +48,52 @@
 
 
 def exps():
     """
     Retrieve experiments.
     """
     exps = []
-    files = EXPS_DIRECTORY.glob('*/config.json')
+    files = EXPS_DIRECTORY.glob("*/config.json")
     for file in sorted(files, key=lambda x: os.path.getmtime(x)):
-        exp = pd.read_json(file, lines=True, convert_dates=['_start'])
+        try:
+            exp = pd.read_json(file, lines=True, convert_dates=["_start"])
+        except ValueError as e:
+            print(f"Error while reading config file '{file}' ({e}). Skipped.")
+            continue
         exps.append(exp)
     exps = pd.concat(exps, axis=0)
-    exps = exps.set_index('_id')
+    exps = exps.set_index("_id")
     return exps
 
 
 def runs():
     """
     Alias for `exps`.
     """
     return exps()
 
 
-def dict_from_kwargs(config=None, *args, **kwargs):
+def dict_from_kwargs(config=None, **kwargs):
     """
     Returns dictionary from either a single dictionary or kwargs arguments.
     """
     # Check that inputs are keyword arguments or a dictionary
-    if len(args) > 1 or (args and kwargs) or (
-            config is not None and (args or kwargs)):
+    if config and kwargs:
         raise ValueError("Usage: log(config) or log(**config).")
-    if config is not None:
-        args = [config]
-    if args and not isinstance(args[0], dict):
+
+    # Parse dictionary
+    if config is None:
+        dictionary = kwargs
+    elif isinstance(config, dict):
+        dictionary = config
+    else:
         try:
-            dictionary = vars(args[0])
+            dictionary = vars(config)
         except TypeError:
             raise ValueError("The provided argument should be a dictionary.")
-    else:
-        dictionary = kwargs
 
     return dictionary
 
 
 def logs(*columns, **filters):
     """
     """
@@ -96,36 +101,40 @@
     for column in columns:
         if not re.fullmatch(FORMAT, column):
             raise ValueError(f"Column '{column}' not in format '{FORMAT}'")
     columns = list(columns) + list(filters.keys())
 
     # Retrieve experiments logs
     logs = []
-    files = EXPS_DIRECTORY.glob('*/logs.json')
+    files = EXPS_DIRECTORY.glob("*/logs.json")
     for file in sorted(files, key=lambda x: os.path.getmtime(x)):
-        log = pd.read_json(file, lines=True)
-        log.index.name = '_step'
+        try:
+            log = pd.read_json(file, lines=True)
+        except ValueError as e:
+            print(f"Error while reading log file '{file}' ({e}). Skipped.")
+            continue
+        log.index.name = "_step"
         log = log.reset_index()
         for key, val in filters.items():
             if key in log:
                 log = log[log[key] == val]
         if columns:
             log = log.loc[:, log.columns.isin(columns + INFOS)]
         logs.append(log)
     logs = pd.concat(logs, axis=0)
 
     # Join configurations and logs
-    logs = logs.merge(exps(), on='_id')
+    logs = logs.merge(exps(), on="_id")
 
     # Filter rows
     for key, val in filters.items():
         logs = logs[logs[key] == val]
 
     # Set index
-    logs = logs.set_index(['_id', '_step'])
+    logs = logs.set_index(["_id", "_step"])
 
     return logs
 
 
 class Experiment:
     """
     """
@@ -138,15 +147,15 @@
         # Check configuration keys
         for key in config.keys():
             if not re.fullmatch(FORMAT, key):
                 raise ValueError(f"Column '{key}' not in format '{FORMAT}'")
 
         # Add information
         self.id = _identifier(8) if id is None else id
-        info = {'_id': self.id, '_start': dt.datetime.now().isoformat()}
+        info = {"_id": self.id, "_start": dt.datetime.now().isoformat()}
 
         # Check id does not exist
         path = EXPS_DIRECTORY / self.id
         if path.exists():
             raise ValueError(f"Experiment with id {self.id} already exist")
         else:
             path.mkdir()
@@ -166,15 +175,15 @@
 
         # Check logs keys
         for key in logs.keys():
             if not re.fullmatch(FORMAT, key):
                 raise ValueError(f"Column '{key}' not in format '{FORMAT}'")
 
         # Add information
-        info = {'_id': self.id, '_time': dt.datetime.now().isoformat()}
+        info = {"_id": self.id, "_time": dt.datetime.now().isoformat()}
 
         logs_file = EXPS_DIRECTORY / f"{self.id}/logs.json"
         logs_file.touch()
         with open(logs_file, "a") as f:
             f.write(json.dumps(logs | info) + "\n")
 
     def logs(self, *columns):
```

### Comparing `explog-0.0.2/explog.egg-info/PKG-INFO` & `explog-0.0.3/explog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: explog
-Version: 0.0.2
+Version: 0.0.3
 Summary: Experiment Logger
 Author-email: Gaspard Lambrechts <gsprd@protonmail.com>
 Project-URL: Homepage, https://github.com/glambrechts/explog
 Project-URL: Issues, https://github.com/glambrechts/explog/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 
-# ExpLog - A Minimal Experiment Logger
+# Exp Log - A Minimal Experiment Logger
 
 ## Installation
 
 ```sh
 pip install explog
 ```
```

### Comparing `explog-0.0.2/pyproject.toml` & `explog-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "explog"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Gaspard Lambrechts", email="gsprd@protonmail.com" },
 ]
 description = "Experiment Logger"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

