# Comparing `tmp/pylogg-0.1.29.tar.gz` & `tmp/pylogg-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogg-0.1.29.tar", last modified: Thu Apr  4 07:17:32 2024, max compression
+gzip compressed data, was "pylogg-0.1.30.tar", last modified: Thu Apr  4 15:46:47 2024, max compression
```

## Comparing `pylogg-0.1.29.tar` & `pylogg-0.1.30.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:17:32.307484 pylogg-0.1.29/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 07:17:27.000000 pylogg-0.1.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 07:17:32.307484 pylogg-0.1.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 07:17:27.000000 pylogg-0.1.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:17:32.307484 pylogg-0.1.29/pylogg/
--rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-04 07:17:27.000000 pylogg-0.1.29/pylogg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 07:17:27.000000 pylogg-0.1.29/pylogg/jsonfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-04 07:17:27.000000 pylogg-0.1.29/pylogg/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-04-04 07:17:27.000000 pylogg-0.1.29/pylogg/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:17:32.307484 pylogg-0.1.29/pylogg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-04 07:17:27.000000 pylogg-0.1.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:17:32.307484 pylogg-0.1.29/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:17:32.307484 pylogg-0.1.29/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-04 07:17:27.000000 pylogg-0.1.29/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:47.950717 pylogg-0.1.30/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 15:46:43.000000 pylogg-0.1.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 15:46:47.950717 pylogg-0.1.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 15:46:43.000000 pylogg-0.1.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:47.950717 pylogg-0.1.30/pylogg/
+-rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-04 15:46:43.000000 pylogg-0.1.30/pylogg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 15:46:43.000000 pylogg-0.1.30/pylogg/jsonfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-04 15:46:43.000000 pylogg-0.1.30/pylogg/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-04 15:46:43.000000 pylogg-0.1.30/pylogg/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:47.950717 pylogg-0.1.30/pylogg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 15:46:47.000000 pylogg-0.1.30/pylogg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 15:46:47.000000 pylogg-0.1.30/pylogg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:46:47.000000 pylogg-0.1.30/pylogg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 15:46:47.000000 pylogg-0.1.30/pylogg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 15:46:47.000000 pylogg-0.1.30/pylogg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-04 15:46:43.000000 pylogg-0.1.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:46:47.950717 pylogg-0.1.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:46:47.950717 pylogg-0.1.30/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-04 15:46:43.000000 pylogg-0.1.30/tests/test_settings.py
```

### Comparing `pylogg-0.1.29/LICENSE` & `pylogg-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.29/PKG-INFO` & `pylogg-0.1.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.1.29
+Version: 0.1.30
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylogg-0.1.29/README.md` & `pylogg-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.29/pylogg/__init__.py` & `pylogg-0.1.30/pylogg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A personally opinionated logging package.
 LICENSE MIT Copyright 2024 Akhlak Mahmood
 
 """
 
-__version__ = "0.1.29"
+__version__ = "0.1.30"
 __author__ = "Akhlak Mahmood"
 
 import os
 import sys
 import textwrap
 import time
 from datetime import datetime, timezone
```

### Comparing `pylogg-0.1.29/pylogg/jsonfs.py` & `pylogg-0.1.30/pylogg/jsonfs.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.29/pylogg/postgres.py` & `pylogg-0.1.30/pylogg/postgres.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.29/pylogg/settings.py` & `pylogg-0.1.30/pylogg/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,140 +1,165 @@
 """
-    A simple module to load configurations from environment varibles or
-    a YAML file.
+    A module to load configurations from environment varibles or
+    YAML file(s).
 
 """
 
 import os
 import string
 import sys
 from typing import NamedTuple
 
 import yaml
 
 # For access to the __annotations__ attribute.
 assert sys.version_info >= (3, 10), "Minimum Python 3.10 required"
 
 
-class YAMLSettings:
+class PLSettings:
     """
     Load all settings from environment variables and/or a YAML file.
 
     name:
         Name of the settings. Used as the prefix for environment variables.
 
+    yaml_file:
+        YAML file to load the settings.
+
+    first_arg:
+        Treat the first argument as the settings YAML file if any.
+
     load_env:
         Load settings from environment variables or not.
 
     prefer_env:
         Override YAML vars with environment variables or vice versa.
+        Default order: cmdline > YAML > Env.
+        Prefer_env order: cmdline > Env. > YAML.
+
 
+    Example:
 
-    Example: Subclass the typing.NamedTuple, and define a classmethod to load the
+    Subclass the typing.NamedTuple, and define a classmethod to load the
     settings.
 
-    class Test(NamedTuple):
+    ```python
+    class _Test(NamedTuple):
         name: str   = 'hello'
 
     class Settings(NamedTuple):
         YAML = None
-        TestSettings : Test
+
+        # Define the sections ...
+        TestSettings : _Test
 
         @classmethod
         def load(c, yaml_file = None, first_arg = False) -> 'Settings':
-            c.YAML = YAMLSettings('pytest')
-            c.YAML.load_file(yaml_file=yaml_file, first_arg=first_arg)
+            c.YAML = PLSettings('pytest', yaml_file, first_arg=first_arg)
             return c.YAML.populate(c)
 
-        def save(self, newfile = None):
-            self.YAML.save(self, yamlfile=newfile)
+        def save(self, yaml_file = None):
+            self.YAML.save(self, yaml_file=yaml_file)
 
-    settings = Settings.load(asset_file)
+    settings = Settings.load('settings.yaml')
     test = settings.TestSettings
     print(test.name)
+    ```
     """
 
-    def __init__(self, name : str, load_env : bool = True,
-                prefer_env : bool = False):
+    def __init__(self, name : str, yaml_file : str = None,
+            first_arg : bool = True, load_env : bool = True,
+            prefer_env : bool = False):
 
         # Prefix of the env vars.
+        # So they can be specified as `NAME_SECTION_VAR=value`
         self._name = name
 
-        # Environment variables.
+        # Container for the environment variables.
         self._env  = os.environ if load_env else {}
 
         # Override file vars with env vars.
         self._prefer_env = prefer_env
 
         # Commandline args.
         self._args = self._get_cmdline_subs()
         self._pos_args = self._get_positional_args()
 
         # Loaded file path
-        self._file = 'settings.yaml'
+        self._file = yaml_file if yaml_file else 'settings.yaml'
 
         # YAML file loaded variables.
         self._yamlvars : dict[str, dict[str, any]] = {}
 
+        self.load_file(self._file, first_arg=first_arg)
+
 
     def __repr__(self) -> str:
         s = self.__class__.__name__ + ": "
         for k, v in self._yamlvars.items():
             s += f"{k} {v._asdict()}"
         return s
 
 
+    def _populate_field(self, section : str, field : str, data_type, def_value):
+        # Start with the default value.
+        value = def_value
+
+        # If _name is given, prefix it for the env var.
+        # Format: NAME_SECTION_FIELD=value
+        env_var_name = f"{section.upper()}_{field.upper()}"
+        if self._name:
+            env_var_name = f"{self._name.upper()}_{env_var_name}"
+
+        # Use the Env var first, if not preferred.
+        if not self._prefer_env:
+            value = self._get_env(env_var_name, value)
+
+        # Override with the YAML vars.
+        value = self._get_yaml(section, field, value)
+
+        # Override with env vars if its preferred.
+        if self._prefer_env:
+            value = self._get_env(env_var_name, value)
+
+        # Check if there is any $ arg template in env vars / yaml.
+        value = self._get_arg(field, value)
+
+        # Convert to expected type.
+        if value is not None:
+            try:
+                value = data_type(value)
+            except:
+                raise ValueError(f"Invalid type for {field}: {value}")
+        return value
+
+
     def _populate_section(self, section_name : str, section_cls : NamedTuple):
         """ Populate settings to the current class/section. """
 
         assert hasattr(section_cls, '_fields'), "Section must be a NamedTuple."
 
         fields = {}
 
         # for each namedtuple fields ...
         for field in section_cls._fields:
             fieldname = f"{section_name}.{field}"
             data_type = section_cls.__annotations__[field]
 
             # Default value.
             value = section_cls._field_defaults.get(field, None)
-
-            env_var_name = \
-                f"{self._name.upper()}_{section_name.upper()}_{field.upper()}"
-
-            if not self._prefer_env:
-                value = self._get_env(env_var_name, value)
-
-            # Override with YAML file vars.
-            value = self._get_yaml(section_name, field, value)
-
-            # Override with env vars.
-            if self._prefer_env:
-                value = self._get_env(env_var_name, value)
-
-            # Check if there is any arg template in env vars / yaml.
-            value = self._get_arg(fieldname, value)
-
-            # Convert to expected type.
-            if value is not None:
-                try:
-                    value = data_type(value)
-                except:
-                    raise ValueError(
-                        f"Invalid type for {fieldname}: {value}")
-
-            # Add to class fields
-            fields[field] = value
+            fields[field] = \
+                self._populate_field(section_name, fieldname, data_type, value)
 
         # Return initialized class.
         return section_cls(**fields)
 
 
     def populate(self, settings : NamedTuple):
-        """ Populate settings to all sections. """
+        """ Populate settings to all sections defined by NamedTuple fields. """
 
         assert hasattr(settings, '_fields'), "Settings must be a NamedTuple."
 
         sections = {}
 
         # for each settings sections ...
         for section_name in settings._fields:
@@ -189,15 +214,14 @@
             tmpl = string.Template(value)
             try:
                 value = tmpl.substitute(self._args)
             except KeyError as err:
                 err = str(err)[1:-1] # remove quotes
                 raise ValueError(
                     f"Argument required for {fieldname}='{value}', --{err} ?")
-
         return value
 
 
     def _get_env(self, var_name, default_value):
         return self._env.get(var_name, default_value)
 
 
@@ -208,39 +232,34 @@
     def _get_yaml(self, classname, var_name, default_value):
         if classname in self._yamlvars:
             return self._yamlvars[classname].get(var_name, default_value)
         else:
             return default_value
 
 
-    def set(self, cls : type, instance : NamedTuple):
-        """ Set the cached instance of a class with new version.
-            Useful to update the global settings or writing new sections
-            to YAML file.
-        """
-        assert type(instance) == cls, "Class and instance do not match"
-
-        classname = cls.__name__
-        self._cache[classname] = instance
-
-
     def load_file(
-        self, yaml_file : str = None, first_arg : bool = False):
+        self, yaml_file : str = None, first_arg : bool = False,
+        update : bool = True):
 
         """ Load all sections and variables of a YAML file.
+        Can be called multiple times to update/add over previous values.
 
         yaml_file:
             YAML file to load the settings.
 
         first_arg:
             Treat the first argument as the settings YAML file if any.
 
+        update:
+            Update the existing sections with the variables defined by the new
+            file. If `False`, all existing sections will be removed.
         """
 
         self._file = yaml_file if yaml_file else self._file
+        self._yamlvars = self._yamlvars if update else {}
 
         # Treat the first argument as the settings file if any.
         if first_arg and len(self._pos_args):
             self._file = self._pos_args[0]
 
         if os.path.isfile(self._file):
             contents = yaml.safe_load(open(self._file))
@@ -252,25 +271,31 @@
 
 
     def is_loaded(self) -> bool:
         """ Returns True if at least one section from YAML file was loaded. """
         return len(self._yamlvars) > 0
 
 
-    def save(self, settings : NamedTuple, yamlfile : str = None,
+    def save(self, settings : NamedTuple, yaml_file : str = None,
                 keep_existing : bool = True):
-        """ Save the settings to a YAML file.
-            If no yamlfile is given, the initial file is used.
+        """ Save all sections of the settings to a YAML file.
+            If no yaml_file is given, the initial file is used.
 
             keep_existing:
                 Keep the already existing sections in the YAML file.
         """
 
-        configs = self._yamlvars if keep_existing else {}
-        outfile = yamlfile if yamlfile is not None else self._file
+        outfile = yaml_file if yaml_file else self._file
+
+        existing = yaml.safe_load(open(outfile)) \
+            if os.path.isfile(outfile) else {}
+
+        configs = existing if keep_existing else {}
+
+        assert type(configs) == dict, f"Existing YAML is not a dict: {outfile}"
 
         assert hasattr(settings, '_fields'), "Settings must be a NamedTuple."
 
         # for each settings sections ...
         for section_name in settings._fields:
             section = getattr(settings, section_name)
```

### Comparing `pylogg-0.1.29/pylogg.egg-info/PKG-INFO` & `pylogg-0.1.30/pylogg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.1.29
+Version: 0.1.30
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pylogg-0.1.29/pyproject.toml` & `pylogg-0.1.30/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 [project]
 name = "pylogg"
-version = "0.1.29"
 authors = [
     { name="Akhlak Mahmood", email="akhlakm@gatech.edu" },
 ]
 description = "Logging and YAML-based configuration modules in Python."
 readme = "README.md"
 requires-python = ">=3.10"
 
+dynamic = [
+    "version",
+]
+
 keywords = ["logging", "development"]
 
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
@@ -40,7 +43,10 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["pylogg"]
+
+[tool.setuptools.dynamic]
+version = {attr = "pylogg.__version__"}
```

### Comparing `pylogg-0.1.29/tests/test_settings.py` & `pylogg-0.1.30/tests/test_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pylogg.settings import NamedTuple, YAMLSettings
+from pylogg.settings import NamedTuple, PLSettings
 
 
 def test_load_settings(assets, tmp_path):
     asset_file = assets / "settings.yaml"
     test_output = tmp_path / "settings.yaml"
 
     class Test(NamedTuple):
@@ -17,20 +17,19 @@
     class Settings(NamedTuple):
         YAML = None
         TestSettings : Test
         PersonSettings : Person
 
         @classmethod
         def load(c, yaml_file = None, first_arg = False) -> 'Settings':
-            c.YAML = YAMLSettings('pytest')
-            c.YAML.load_file(yaml_file=yaml_file, first_arg=first_arg)
+            c.YAML = PLSettings('pytest', yaml_file, first_arg=first_arg)
             return c.YAML.populate(c)
 
         def create(self, newfile = None):
-            self.YAML.save(self, yamlfile=newfile)
+            self.YAML.save(self, yaml_file=newfile)
 
 
     sett = Settings.load(asset_file)
     sett = sett._replace(TestSettings = sett.TestSettings._replace(row1 = 90.0))
     sett.create(test_output)
 
 
@@ -45,20 +44,19 @@
 
     class Settings(NamedTuple):
         YAML = None
         TestSettings : Test
 
         @classmethod
         def load(c, yaml_file = None, first_arg = False) -> 'Settings':
-            c.YAML = YAMLSettings('pytest')
-            c.YAML.load_file(yaml_file=yaml_file, first_arg=first_arg)
+            c.YAML = PLSettings('pytest', yaml_file, first_arg=first_arg)
             return c.YAML.populate(c)
 
         def save(self, newfile = None):
-            self.YAML.save(self, yamlfile=newfile)
+            self.YAML.save(self, yaml_file=newfile)
 
     settings = Settings.load(asset_file)
     test = settings.TestSettings
 
     assert test.row1 == 23.6
     assert type(test.row1) == float
     assert test.row2 == 'Hello'
@@ -80,16 +78,15 @@
 
     class Settings(NamedTuple):
         YAML = None
         TestSettings : Test
 
         @classmethod
         def load(c, yaml_file = None, first_arg = False) -> 'Settings':
-            c.YAML = YAMLSettings('pytest')
-            c.YAML.load_file(yaml_file=yaml_file, first_arg=first_arg)
+            c.YAML = PLSettings('pytest', yaml_file, first_arg=first_arg)
             return c.YAML.populate(c)
 
         def save(self, newfile = None):
             self.YAML.save(self, yamlfile=newfile)
 
     settings = Settings.load(None)
     test = settings.TestSettings
@@ -100,18 +97,18 @@
 
     print(test)
 
 
 def test_postitional_args():
     import sys
 
-    yaml = YAMLSettings('pytest')
+    yaml = PLSettings('pytest')
     print(yaml._pos_args)
 
     sys.argv += ['--name', 'world', 'settings2.yaml', '--debug', '--num', '22']
-    yaml = YAMLSettings('pytest')
+    yaml = PLSettings('pytest')
     print(yaml._pos_args)
 
     sys.argv += ['settings2.yaml']
-    yaml = YAMLSettings('pytest')
+    yaml = PLSettings('pytest')
     assert yaml._pos_args == ['settings2.yaml', 'settings2.yaml']
     print(yaml._pos_args)
```

