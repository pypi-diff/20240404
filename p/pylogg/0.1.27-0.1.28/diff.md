# Comparing `tmp/pylogg-0.1.27.tar.gz` & `tmp/pylogg-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogg-0.1.27.tar", last modified: Thu Apr  4 01:39:54 2024, max compression
+gzip compressed data, was "pylogg-0.1.28.tar", last modified: Thu Apr  4 02:13:31 2024, max compression
```

## Comparing `pylogg-0.1.27.tar` & `pylogg-0.1.28.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:39:54.004359 pylogg-0.1.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 01:39:49.000000 pylogg-0.1.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-04 01:39:54.004359 pylogg-0.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 01:39:49.000000 pylogg-0.1.27/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:39:54.004359 pylogg-0.1.27/pylogg/
--rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-04 01:39:49.000000 pylogg-0.1.27/pylogg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 01:39:49.000000 pylogg-0.1.27/pylogg/jsonfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-04 01:39:49.000000 pylogg-0.1.27/pylogg/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8441 2024-04-04 01:39:49.000000 pylogg-0.1.27/pylogg/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:39:54.004359 pylogg-0.1.27/pylogg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-04 01:39:53.000000 pylogg-0.1.27/pylogg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 01:39:54.000000 pylogg-0.1.27/pylogg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 01:39:53.000000 pylogg-0.1.27/pylogg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 01:39:53.000000 pylogg-0.1.27/pylogg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 01:39:53.000000 pylogg-0.1.27/pylogg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-04 01:39:49.000000 pylogg-0.1.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 01:39:54.004359 pylogg-0.1.27/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 01:39:54.004359 pylogg-0.1.27/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-04 01:39:49.000000 pylogg-0.1.27/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:13:31.137462 pylogg-0.1.28/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 02:13:24.000000 pylogg-0.1.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-04 02:13:31.137462 pylogg-0.1.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 02:13:24.000000 pylogg-0.1.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:13:31.133462 pylogg-0.1.28/pylogg/
+-rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-04 02:13:24.000000 pylogg-0.1.28/pylogg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 02:13:24.000000 pylogg-0.1.28/pylogg/jsonfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-04 02:13:24.000000 pylogg-0.1.28/pylogg/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-04 02:13:24.000000 pylogg-0.1.28/pylogg/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:13:31.137462 pylogg-0.1.28/pylogg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-04 02:13:24.000000 pylogg-0.1.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 02:13:31.137462 pylogg-0.1.28/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:13:31.137462 pylogg-0.1.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-04 02:13:24.000000 pylogg-0.1.28/tests/test_settings.py
```

### Comparing `pylogg-0.1.27/LICENSE` & `pylogg-0.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.27/PKG-INFO` & `pylogg-0.1.28/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.1.27
+Version: 0.1.28
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylogg-0.1.27/README.md` & `pylogg-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.27/pylogg/__init__.py` & `pylogg-0.1.28/pylogg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A personally opinionated logging package.
 LICENSE MIT Copyright 2024 Akhlak Mahmood
 
 """
 
-__version__ = "0.1.27"
+__version__ = "0.1.28"
 __author__ = "Akhlak Mahmood"
 
 import os
 import sys
 import textwrap
 import time
 from datetime import datetime, timezone
```

### Comparing `pylogg-0.1.27/pylogg/jsonfs.py` & `pylogg-0.1.28/pylogg/jsonfs.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.27/pylogg/postgres.py` & `pylogg-0.1.28/pylogg/postgres.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.27/pylogg/settings.py` & `pylogg-0.1.28/pylogg/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,76 +32,62 @@
 class YAMLSettings:
     """
     Load all settings from environment variables and/or a YAML file.
 
     name:
         Name of the settings. Used as the prefix for environment variables.
 
-    yamlfile:
-        YAML file to load the settings.
-
-    first_arg_as_file:
-        Treat the first argument as the settings YAML file if any.
-
     load_env:
         Load settings from environment variables or not.
 
     prefer_env:
         Override YAML vars with environment variables or vice versa.
     """
 
-    def __init__(self, name : str,
-        yamlfile : str = 'settings.yaml', first_arg_as_file : bool = False,
-        load_env : bool = True, prefer_env : bool = False):
+    def __init__(self, name : str, load_env : bool = True,
+                prefer_env : bool = False):
 
         # Prefix of the env vars.
         self._name = name
 
         # Environment variables.
         self._env  = os.environ if load_env else {}
 
         # Override file vars with env vars.
         self._prefer_env = prefer_env
 
         # Commandline args.
         self._args = self._get_cmdline_subs()
         self._pos_args = self._get_positional_args()
 
-        self._file = yamlfile
-
-        # Take the first argument as the settings file if any.
-        if first_arg_as_file:
-            if len(self._pos_args):
-                self._file = self._pos_args[0]
+        # Loaded file path
+        self._file = 'settings.yaml'
 
         # YAML file loaded variables.
-        self.yamlvars : dict[str, dict[str, any]] = {}
+        self._yamlvars : dict[str, dict[str, any]] = {}
 
         # Cache for the processed sections.
-        self.cache = {}
-
-        self.load_file()
-
+        self._cache = {}
 
     def __repr__(self) -> str:
         s = self.__class__.__name__ + ": "
-        for k, v in self.cache.items():
+        for k, v in self._cache.items():
             s += f"{k} {v._asdict()}"
         return s
 
     def __call__(self, cls : NamedTuple):
         """ Populate settings to the current class/section. """
 
         assert hasattr(cls, '_fields'), "Settings must be a NamedTuple."
 
         fields = {}
         classname : str = cls.__name__
 
-        if classname in self.cache:
-            return self.cache[classname]
+        if classname in self._cache:
+            return self._cache[classname]
 
         # for each namedtuple fields ...
         for field in cls._fields:
             fieldname = f"{classname}.{field}"
             data_type = cls.__annotations__[field]
 
             # Default value.
@@ -131,18 +117,18 @@
                     raise ValueError(
                         f"Invalid type for {fieldname}: {value}")
 
             # Add to class fields
             fields[field] = value
 
         # Cache for future.
-        self.cache[classname] = cls(**fields)
+        self._cache[classname] = cls(**fields)
 
         # Return initialized class.
-        return self.cache[classname]
+        return self._cache[classname]
 
 
     def _get_positional_args(self) -> list[str]:
         positionals = []
         for i in range(1, len(sys.argv)):
             field = sys.argv[i]
             if not field.startswith("-"):
@@ -189,62 +175,79 @@
 
 
     def _get_env(self, var_name, default_value):
         return self._env.get(var_name, default_value)
 
 
     def _get_yaml(self, classname, var_name, default_value):
-        if classname in self.yamlvars:
-            return self.yamlvars[classname].get(var_name, default_value)
+        if classname in self._yamlvars:
+            return self._yamlvars[classname].get(var_name, default_value)
         else:
             return default_value
 
 
     def set(self, cls : type, instance : NamedTuple):
         """ Set the cached instance of a class with new version.
             Useful to update the global settings or writing new sections
             to YAML file.
         """
         assert type(instance) == cls, "Class and instance do not match"
 
         classname = cls.__name__
-        self.cache[classname] = instance
+        self._cache[classname] = instance
+
+
+    def load_file(
+        self, yaml_file : str = None, first_arg : bool = False):
+
+        """ Load all sections and variables of a YAML file.
+
+        yaml_file:
+            YAML file to load the settings.
+
+        first_arg:
+            Treat the first argument as the settings YAML file if any.
+
+        """
+
+        self._file = yaml_file if yaml_file else self._file
 
+        # Treat the first argument as the settings file if any.
+        if first_arg and len(self._pos_args):
+            self._file = self._pos_args[0]
 
-    def load_file(self):
-        """ Load all sections and variables of the YAML file. """
         if os.path.isfile(self._file):
-            yamlfile = yaml.safe_load(open(self._file))
-            for section, fields in yamlfile.items():
+            contents = yaml.safe_load(open(self._file))
+            for section, fields in contents.items():
                 for fieldname, value in fields.items():
-                    if section not in self.yamlvars:
-                        self.yamlvars[section] = {}
-                    self.yamlvars[section][fieldname] = value
+                    if section not in self._yamlvars:
+                        self._yamlvars[section] = {}
+                    self._yamlvars[section][fieldname] = value
 
 
     def is_loaded(self) -> bool:
         """ Returns True if at least one section from YAML file was loaded. """
-        return len(self.yamlvars) > 0
+        return len(self._yamlvars) > 0
 
 
     def save(self, *sections : NamedTuple, yamlfile : str = None,
                 keep_existing : bool = True):
         """ Save the given sections to YAML file.
             If no section is specified, all sections are written.
             If no yamlfile is given, the initial file is used.
 
             keep_existing:
                 Keep the already existing sections in the YAML file.
         """
-        configs = self.yamlvars if keep_existing else {}
+        configs = self._yamlvars if keep_existing else {}
         outfile = yamlfile if yamlfile is not None else self._file
 
         # Use all sections
         if len(sections) == 0:
-            sections = self.cache.values()
+            sections = self._cache.values()
 
         # For each NamedTuple section
         for cls in sections:
             assert hasattr(cls, '_fields'), "Section must be a NamedTuple"
 
             try:
                 # class
```

### Comparing `pylogg-0.1.27/pylogg.egg-info/PKG-INFO` & `pylogg-0.1.28/pylogg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.1.27
+Version: 0.1.28
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylogg-0.1.27/pyproject.toml` & `pylogg-0.1.28/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pylogg"
-version = "0.1.27"
+version = "0.1.28"
 authors = [
     { name="Akhlak Mahmood", email="akhlakm@gatech.edu" },
 ]
 description = "Logging and YAML-based configuration modules in Python."
 readme = "README.md"
 requires-python = ">=3.0"
```

### Comparing `pylogg-0.1.27/tests/test_settings.py` & `pylogg-0.1.28/tests/test_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pylogg.settings import NamedTuple, YAMLSettings
 
 
 def test_yaml_write(assets, tmp_path):
     asset_file = assets / "settings.yaml"
     test_output = tmp_path / "settings.yaml"
 
-    yaml = YAMLSettings('pytest', yamlfile=test_output, first_arg_as_file=False)
+    yaml = YAMLSettings('pytest')
+    yaml.load_file(yaml_file=test_output, first_arg=False)
 
     class Test(NamedTuple):
         row1: float = 23.6
         row2: str   = 'Hello'
         row3: str   = 'World'
 
         @classmethod
@@ -27,15 +28,16 @@
     yaml.save(Test)
     assert test_output.read_text() == asset_file.read_text()
 
 
 def test_args_subs():
     import sys
     sys.argv += ['--name', 'world', '--debug', '--num', '22']
-    yaml = YAMLSettings('pytest', first_arg_as_file=False)
+    yaml = YAMLSettings('pytest')
+    yaml.load_file(first_arg=False)
 
     class Test(NamedTuple):
         greeting: str   = 'Hello $name'
         number : int    = '$num'
         debug : bool    = '$debug'
 
         @classmethod
@@ -49,20 +51,18 @@
 
     print(test)
 
 
 def test_postitional_args():
     import sys
 
-    yaml = YAMLSettings('pytest', first_arg_as_file=False)
-    assert yaml._file == 'settings.yaml'
+    yaml = YAMLSettings('pytest')
     print(yaml._pos_args)
 
     sys.argv += ['--name', 'world', 'settings2.yaml', '--debug', '--num', '22']
-    yaml = YAMLSettings('pytest', first_arg_as_file=True)
-    assert yaml._file == 'settings2.yaml'
+    yaml = YAMLSettings('pytest')
     print(yaml._pos_args)
 
     sys.argv += ['settings2.yaml']
-    yaml = YAMLSettings('pytest', first_arg_as_file=True)
+    yaml = YAMLSettings('pytest')
     assert yaml._pos_args == ['settings2.yaml', 'settings2.yaml']
     print(yaml._pos_args)
```

