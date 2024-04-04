# Comparing `tmp/pylogg-0.1.26.tar.gz` & `tmp/pylogg-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogg-0.1.26.tar", last modified: Fri Mar 15 16:02:14 2024, max compression
+gzip compressed data, was "pylogg-0.1.27.tar", last modified: Thu Apr  4 01:39:54 2024, max compression
```

## Comparing `pylogg-0.1.26.tar` & `pylogg-0.1.27.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:02:14.785570 pylogg-0.1.26/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-15 16:02:09.000000 pylogg-0.1.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-03-15 16:02:14.785570 pylogg-0.1.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-15 16:02:09.000000 pylogg-0.1.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:02:14.781570 pylogg-0.1.26/pylogg/
--rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-03-15 16:02:09.000000 pylogg-0.1.26/pylogg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-03-15 16:02:09.000000 pylogg-0.1.26/pylogg/jsonfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-03-15 16:02:09.000000 pylogg-0.1.26/pylogg/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-03-15 16:02:09.000000 pylogg-0.1.26/pylogg/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:02:14.785570 pylogg-0.1.26/pylogg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-03-15 16:02:14.000000 pylogg-0.1.26/pylogg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-15 16:02:14.000000 pylogg-0.1.26/pylogg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 16:02:14.000000 pylogg-0.1.26/pylogg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-15 16:02:14.000000 pylogg-0.1.26/pylogg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 16:02:14.000000 pylogg-0.1.26/pylogg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-15 16:02:09.000000 pylogg-0.1.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 16:02:14.785570 pylogg-0.1.26/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 16:02:14.785570 pylogg-0.1.26/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-15 16:02:09.000000 pylogg-0.1.26/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:39:54.004359 pylogg-0.1.27/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 01:39:49.000000 pylogg-0.1.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-04 01:39:54.004359 pylogg-0.1.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 01:39:49.000000 pylogg-0.1.27/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:39:54.004359 pylogg-0.1.27/pylogg/
+-rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-04 01:39:49.000000 pylogg-0.1.27/pylogg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 01:39:49.000000 pylogg-0.1.27/pylogg/jsonfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-04 01:39:49.000000 pylogg-0.1.27/pylogg/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8441 2024-04-04 01:39:49.000000 pylogg-0.1.27/pylogg/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:39:54.004359 pylogg-0.1.27/pylogg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-04 01:39:53.000000 pylogg-0.1.27/pylogg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 01:39:54.000000 pylogg-0.1.27/pylogg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:39:53.000000 pylogg-0.1.27/pylogg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 01:39:53.000000 pylogg-0.1.27/pylogg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 01:39:53.000000 pylogg-0.1.27/pylogg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-04 01:39:49.000000 pylogg-0.1.27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:39:54.004359 pylogg-0.1.27/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:39:54.004359 pylogg-0.1.27/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-04 01:39:49.000000 pylogg-0.1.27/tests/test_settings.py
```

### Comparing `pylogg-0.1.26/LICENSE` & `pylogg-0.1.27/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.26/PKG-INFO` & `pylogg-0.1.27/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.1.26
+Version: 0.1.27
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylogg-0.1.26/README.md` & `pylogg-0.1.27/README.md`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.26/pylogg/__init__.py` & `pylogg-0.1.27/pylogg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A personally opinionated logging package.
-LICENSE MIT Copyright 2023 Akhlak Mahmood
+LICENSE MIT Copyright 2024 Akhlak Mahmood
 
 """
 
-__version__ = "0.1.26"
+__version__ = "0.1.27"
 __author__ = "Akhlak Mahmood"
 
 import os
 import sys
 import textwrap
 import time
 from datetime import datetime, timezone
```

### Comparing `pylogg-0.1.26/pylogg/jsonfs.py` & `pylogg-0.1.27/pylogg/jsonfs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 
 import pylogg
 
 log = pylogg.get('jsonfs')
 
 def load_lines(jsonl_file : str) -> list[dict]:
     """ Load a JSONL file into list of dictionaries. """
-    log.info("Load JSONL:", jsonl_file)
+    log.trace("Load JSONL:", jsonl_file)
     with open(jsonl_file) as fp:
         jsonlines = list(fp)
 
     return [ json.loads(json_str) for json_str in jsonlines ]
 
 
 def save_lines(linelist : list[dict] , jsonl_file : str):
     """ Save a list of dictionaries as a JSONL file. """
 
     assert type(linelist) == list
-    log.info("Save JSONL:", jsonl_file)
+    log.trace("Save JSONL:", jsonl_file)
 
     # Make sure all dict items have the same keys.
     keys = set()
     for line in linelist:
         for k in line.keys():
             keys.add(k)
 
@@ -38,25 +38,25 @@
         fp.writelines(jsonlines)
 
 
 def save_dict(obj : dict, filename):
     """ Save a dictionary object as JSON. """
     obj = _recurse_type(obj)
 
-    log.info("Save JSON: ", filename)
+    log.trace("Save JSON: ", filename)
     try:
         json.dump(obj, open(filename, "w"), indent=4)
     except Exception as err:
         print(obj)
         print(err)
 
 
 def load_dict(filename) -> dict:
     """ Load a JSON file as dict. """
-    log.info("Load JSON: ", filename)
+    log.trace("Load JSON: ", filename)
     d = json.load(open(filename))
     return d
 
 
 def _recurse_type(obj):
     if type(obj) != dict:
         obj = dict(obj)
```

### Comparing `pylogg-0.1.26/pylogg/postgres.py` & `pylogg-0.1.27/pylogg/postgres.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.26/pylogg/settings.py` & `pylogg-0.1.27/pylogg/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # For access to the __annotations__ attribute.
 assert sys.version_info >= (3, 10), "Minimum Python 3.10 required"
 
 
 class YAMLSettings:
     """
-    Load settings from environment variables and/or a YAML file.
+    Load all settings from environment variables and/or a YAML file.
 
     name:
         Name of the settings. Used as the prefix for environment variables.
 
     yamlfile:
         YAML file to load the settings.
 
@@ -50,32 +50,32 @@
     """
 
     def __init__(self, name : str,
         yamlfile : str = 'settings.yaml', first_arg_as_file : bool = False,
         load_env : bool = True, prefer_env : bool = False):
 
         # Prefix of the env vars.
-        self.name = name
+        self._name = name
 
         # Environment variables.
-        self.env  = os.environ if load_env else {}
+        self._env  = os.environ if load_env else {}
 
         # Override file vars with env vars.
-        self.prefer_env = prefer_env
+        self._prefer_env = prefer_env
 
         # Commandline args.
-        self.args = self._get_cmdline_subs()
-        self.pos_args = self._get_positional_args()
+        self._args = self._get_cmdline_subs()
+        self._pos_args = self._get_positional_args()
 
-        self.file = yamlfile
+        self._file = yamlfile
 
         # Take the first argument as the settings file if any.
         if first_arg_as_file:
-            if len(self.pos_args):
-                self.file = self.pos_args[0]
+            if len(self._pos_args):
+                self._file = self._pos_args[0]
 
         # YAML file loaded variables.
         self.yamlvars : dict[str, dict[str, any]] = {}
 
         # Cache for the processed sections.
         self.cache = {}
 
@@ -104,24 +104,24 @@
             fieldname = f"{classname}.{field}"
             data_type = cls.__annotations__[field]
 
             # Default value.
             value = cls._field_defaults.get(field, None)
 
             env_var_name = \
-                f"{self.name.upper()}_{classname.upper()}_{field.upper()}"
+                f"{self._name.upper()}_{classname.upper()}_{field.upper()}"
 
-            if not self.prefer_env:
+            if not self._prefer_env:
                 value = self._get_env(env_var_name, value)
 
             # Override with YAML file vars.
             value = self._get_yaml(classname, field, value)
 
             # Override with env vars.
-            if self.prefer_env:
+            if self._prefer_env:
                 value = self._get_env(env_var_name, value)
 
             # Check if there is any arg template in env vars / yaml.
             value = self._get_arg(fieldname, value)
 
             # Convert to expected type.
             if value is not None:
@@ -175,25 +175,25 @@
         """ Perform string substitution using commandline arguments.
             Substitution placeholders are prefixed with a $.
             Raises ValueError if arguments do not contain a placeholder.
         """
         if type(value) == str and '$' in value:
             tmpl = string.Template(value)
             try:
-                value = tmpl.substitute(self.args)
+                value = tmpl.substitute(self._args)
             except KeyError as err:
                 err = str(err)[1:-1] # remove quotes
                 raise ValueError(
                     f"Argument required for {fieldname}='{value}', --{err} ?")
 
         return value
 
 
     def _get_env(self, var_name, default_value):
-        return self.env.get(var_name, default_value)
+        return self._env.get(var_name, default_value)
 
 
     def _get_yaml(self, classname, var_name, default_value):
         if classname in self.yamlvars:
             return self.yamlvars[classname].get(var_name, default_value)
         else:
             return default_value
@@ -207,17 +207,17 @@
         assert type(instance) == cls, "Class and instance do not match"
 
         classname = cls.__name__
         self.cache[classname] = instance
 
 
     def load_file(self):
-        """ Load the variables of the YAML file. """
-        if os.path.isfile(self.file):
-            yamlfile = yaml.safe_load(open(self.file))
+        """ Load all sections and variables of the YAML file. """
+        if os.path.isfile(self._file):
+            yamlfile = yaml.safe_load(open(self._file))
             for section, fields in yamlfile.items():
                 for fieldname, value in fields.items():
                     if section not in self.yamlvars:
                         self.yamlvars[section] = {}
                     self.yamlvars[section][fieldname] = value
 
 
@@ -232,15 +232,15 @@
             If no section is specified, all sections are written.
             If no yamlfile is given, the initial file is used.
 
             keep_existing:
                 Keep the already existing sections in the YAML file.
         """
         configs = self.yamlvars if keep_existing else {}
-        outfile = yamlfile if yamlfile is not None else self.file
+        outfile = yamlfile if yamlfile is not None else self._file
 
         # Use all sections
         if len(sections) == 0:
             sections = self.cache.values()
 
         # For each NamedTuple section
         for cls in sections:
@@ -265,9 +265,9 @@
         yaml.safe_dump(configs, open(outfile, 'w'), indent=4)
         print("Save OK:", outfile)
 
 
     def copy_sample(self, sample_file : str):
         """ Copy a sample YAML file to the current settings file. """
         import shutil
-        shutil.copyfile(sample_file, self.file)
-        print("Save OK:", self.file)
+        shutil.copyfile(sample_file, self._file)
+        print("Save OK:", self._file)
```

### Comparing `pylogg-0.1.26/pylogg.egg-info/PKG-INFO` & `pylogg-0.1.27/pylogg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.1.26
+Version: 0.1.27
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylogg-0.1.26/pyproject.toml` & `pylogg-0.1.27/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pylogg"
-version = "0.1.26"
+version = "0.1.27"
 authors = [
     { name="Akhlak Mahmood", email="akhlakm@gatech.edu" },
 ]
 description = "Logging and YAML-based configuration modules in Python."
 readme = "README.md"
 requires-python = ">=3.0"
```

### Comparing `pylogg-0.1.26/tests/test_settings.py` & `pylogg-0.1.27/tests/test_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,19 +50,19 @@
     print(test)
 
 
 def test_postitional_args():
     import sys
 
     yaml = YAMLSettings('pytest', first_arg_as_file=False)
-    assert yaml.file == 'settings.yaml'
-    print(yaml.pos_args)
+    assert yaml._file == 'settings.yaml'
+    print(yaml._pos_args)
 
     sys.argv += ['--name', 'world', 'settings2.yaml', '--debug', '--num', '22']
     yaml = YAMLSettings('pytest', first_arg_as_file=True)
-    assert yaml.file == 'settings2.yaml'
-    print(yaml.pos_args)
+    assert yaml._file == 'settings2.yaml'
+    print(yaml._pos_args)
 
     sys.argv += ['settings2.yaml']
     yaml = YAMLSettings('pytest', first_arg_as_file=True)
-    assert yaml.pos_args == ['settings2.yaml', 'settings2.yaml']
-    print(yaml.pos_args)
+    assert yaml._pos_args == ['settings2.yaml', 'settings2.yaml']
+    print(yaml._pos_args)
```

