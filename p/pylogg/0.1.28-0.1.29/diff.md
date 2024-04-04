# Comparing `tmp/pylogg-0.1.28.tar.gz` & `tmp/pylogg-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogg-0.1.28.tar", last modified: Thu Apr  4 02:13:31 2024, max compression
+gzip compressed data, was "pylogg-0.1.29.tar", last modified: Thu Apr  4 07:17:32 2024, max compression
```

## Comparing `pylogg-0.1.28.tar` & `pylogg-0.1.29.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:13:31.137462 pylogg-0.1.28/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 02:13:24.000000 pylogg-0.1.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-04 02:13:31.137462 pylogg-0.1.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 02:13:24.000000 pylogg-0.1.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:13:31.133462 pylogg-0.1.28/pylogg/
--rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-04 02:13:24.000000 pylogg-0.1.28/pylogg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 02:13:24.000000 pylogg-0.1.28/pylogg/jsonfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-04 02:13:24.000000 pylogg-0.1.28/pylogg/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-04 02:13:24.000000 pylogg-0.1.28/pylogg/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:13:31.137462 pylogg-0.1.28/pylogg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 02:13:31.000000 pylogg-0.1.28/pylogg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-04 02:13:24.000000 pylogg-0.1.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 02:13:31.137462 pylogg-0.1.28/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:13:31.137462 pylogg-0.1.28/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-04 02:13:24.000000 pylogg-0.1.28/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:17:32.307484 pylogg-0.1.29/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-04 07:17:27.000000 pylogg-0.1.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 07:17:32.307484 pylogg-0.1.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 07:17:27.000000 pylogg-0.1.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:17:32.307484 pylogg-0.1.29/pylogg/
+-rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-04 07:17:27.000000 pylogg-0.1.29/pylogg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-04 07:17:27.000000 pylogg-0.1.29/pylogg/jsonfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-04 07:17:27.000000 pylogg-0.1.29/pylogg/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-04-04 07:17:27.000000 pylogg-0.1.29/pylogg/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:17:32.307484 pylogg-0.1.29/pylogg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 07:17:32.000000 pylogg-0.1.29/pylogg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-04 07:17:27.000000 pylogg-0.1.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 07:17:32.307484 pylogg-0.1.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:17:32.307484 pylogg-0.1.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-04 07:17:27.000000 pylogg-0.1.29/tests/test_settings.py
```

### Comparing `pylogg-0.1.28/LICENSE` & `pylogg-0.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.28/PKG-INFO` & `pylogg-0.1.29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.1.28
+Version: 0.1.29
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Provides-Extra: postgres
 Requires-Dist: pandas; extra == "postgres"
 Requires-Dist: sshtunnel; extra == "postgres"
 Requires-Dist: psycopg[binary]; extra == "postgres"
```

### Comparing `pylogg-0.1.28/README.md` & `pylogg-0.1.29/README.md`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.28/pylogg/__init__.py` & `pylogg-0.1.29/pylogg/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A personally opinionated logging package.
 LICENSE MIT Copyright 2024 Akhlak Mahmood
 
 """
 
-__version__ = "0.1.28"
+__version__ = "0.1.29"
 __author__ = "Akhlak Mahmood"
 
 import os
 import sys
 import textwrap
 import time
 from datetime import datetime, timezone
```

### Comparing `pylogg-0.1.28/pylogg/jsonfs.py` & `pylogg-0.1.29/pylogg/jsonfs.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.28/pylogg/postgres.py` & `pylogg-0.1.29/pylogg/postgres.py`

 * *Files identical despite different names*

### Comparing `pylogg-0.1.28/pylogg/settings.py` & `pylogg-0.1.29/pylogg/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 """
     A simple module to load configurations from environment varibles or
     a YAML file.
 
-    Subclass the typing.NamedTuple, and define a classmethod to load the
-    settings.
-
-    yaml = YAMLSettings()
-
-    class Test(NamedTuple):
-        name: str   = 'hello'
-
-        @classmethod
-        def settings(cls) -> 'Test': return yaml(cls)
-
-    test = Test.settings()
-    print(test.name)
-
 """
 
 import os
 import string
 import sys
 from typing import NamedTuple
 
@@ -37,14 +23,38 @@
         Name of the settings. Used as the prefix for environment variables.
 
     load_env:
         Load settings from environment variables or not.
 
     prefer_env:
         Override YAML vars with environment variables or vice versa.
+
+
+    Example: Subclass the typing.NamedTuple, and define a classmethod to load the
+    settings.
+
+    class Test(NamedTuple):
+        name: str   = 'hello'
+
+    class Settings(NamedTuple):
+        YAML = None
+        TestSettings : Test
+
+        @classmethod
+        def load(c, yaml_file = None, first_arg = False) -> 'Settings':
+            c.YAML = YAMLSettings('pytest')
+            c.YAML.load_file(yaml_file=yaml_file, first_arg=first_arg)
+            return c.YAML.populate(c)
+
+        def save(self, newfile = None):
+            self.YAML.save(self, yamlfile=newfile)
+
+    settings = Settings.load(asset_file)
+    test = settings.TestSettings
+    print(test.name)
     """
 
     def __init__(self, name : str, load_env : bool = True,
                 prefer_env : bool = False):
 
         # Prefix of the env vars.
         self._name = name
@@ -61,50 +71,45 @@
 
         # Loaded file path
         self._file = 'settings.yaml'
 
         # YAML file loaded variables.
         self._yamlvars : dict[str, dict[str, any]] = {}
 
-        # Cache for the processed sections.
-        self._cache = {}
 
     def __repr__(self) -> str:
         s = self.__class__.__name__ + ": "
-        for k, v in self._cache.items():
+        for k, v in self._yamlvars.items():
             s += f"{k} {v._asdict()}"
         return s
 
-    def __call__(self, cls : NamedTuple):
+
+    def _populate_section(self, section_name : str, section_cls : NamedTuple):
         """ Populate settings to the current class/section. """
 
-        assert hasattr(cls, '_fields'), "Settings must be a NamedTuple."
+        assert hasattr(section_cls, '_fields'), "Section must be a NamedTuple."
 
         fields = {}
-        classname : str = cls.__name__
-
-        if classname in self._cache:
-            return self._cache[classname]
 
         # for each namedtuple fields ...
-        for field in cls._fields:
-            fieldname = f"{classname}.{field}"
-            data_type = cls.__annotations__[field]
+        for field in section_cls._fields:
+            fieldname = f"{section_name}.{field}"
+            data_type = section_cls.__annotations__[field]
 
             # Default value.
-            value = cls._field_defaults.get(field, None)
+            value = section_cls._field_defaults.get(field, None)
 
             env_var_name = \
-                f"{self._name.upper()}_{classname.upper()}_{field.upper()}"
+                f"{self._name.upper()}_{section_name.upper()}_{field.upper()}"
 
             if not self._prefer_env:
                 value = self._get_env(env_var_name, value)
 
             # Override with YAML file vars.
-            value = self._get_yaml(classname, field, value)
+            value = self._get_yaml(section_name, field, value)
 
             # Override with env vars.
             if self._prefer_env:
                 value = self._get_env(env_var_name, value)
 
             # Check if there is any arg template in env vars / yaml.
             value = self._get_arg(fieldname, value)
@@ -116,19 +121,37 @@
                 except:
                     raise ValueError(
                         f"Invalid type for {fieldname}: {value}")
 
             # Add to class fields
             fields[field] = value
 
-        # Cache for future.
-        self._cache[classname] = cls(**fields)
+        # Return initialized class.
+        return section_cls(**fields)
+
+
+    def populate(self, settings : NamedTuple):
+        """ Populate settings to all sections. """
+
+        assert hasattr(settings, '_fields'), "Settings must be a NamedTuple."
+
+        sections = {}
+
+        # for each settings sections ...
+        for section_name in settings._fields:
+            section_definition = settings.__annotations__[section_name]
+
+            # populate individual section
+            value = self._populate_section(section_name, section_definition)
+
+            # Add to class sections
+            sections[section_name] = value
 
         # Return initialized class.
-        return self._cache[classname]
+        return settings(**sections)
 
 
     def _get_positional_args(self) -> list[str]:
         positionals = []
         for i in range(1, len(sys.argv)):
             field = sys.argv[i]
             if not field.startswith("-"):
@@ -174,14 +197,18 @@
         return value
 
 
     def _get_env(self, var_name, default_value):
         return self._env.get(var_name, default_value)
 
 
+    def _get_yaml_section(self, classname, default_value):
+        return self._yamlvars.get(classname, default_value)
+
+
     def _get_yaml(self, classname, var_name, default_value):
         if classname in self._yamlvars:
             return self._yamlvars[classname].get(var_name, default_value)
         else:
             return default_value
 
 
@@ -225,49 +252,34 @@
 
 
     def is_loaded(self) -> bool:
         """ Returns True if at least one section from YAML file was loaded. """
         return len(self._yamlvars) > 0
 
 
-    def save(self, *sections : NamedTuple, yamlfile : str = None,
+    def save(self, settings : NamedTuple, yamlfile : str = None,
                 keep_existing : bool = True):
-        """ Save the given sections to YAML file.
-            If no section is specified, all sections are written.
+        """ Save the settings to a YAML file.
             If no yamlfile is given, the initial file is used.
 
             keep_existing:
                 Keep the already existing sections in the YAML file.
         """
+
         configs = self._yamlvars if keep_existing else {}
         outfile = yamlfile if yamlfile is not None else self._file
 
-        # Use all sections
-        if len(sections) == 0:
-            sections = self._cache.values()
-
-        # For each NamedTuple section
-        for cls in sections:
-            assert hasattr(cls, '_fields'), "Section must be a NamedTuple"
+        assert hasattr(settings, '_fields'), "Settings must be a NamedTuple."
 
-            try:
-                # class
-                section = cls.__name__
-                assert hasattr(cls, 'settings'), \
-                    f"No 'settings' method found in {section}, use an instance."
-                try:
-                    configs[section] = cls.settings()._asdict()
-                except:
-                    raise RuntimeError(
-                        f"{section}.settings() not found, use an instance.")
+        # for each settings sections ...
+        for section_name in settings._fields:
+            section = getattr(settings, section_name)
 
-            except AttributeError:
-                # instance
-                section = cls.__class__.__name__
-                configs[section] = cls._asdict()
+            if hasattr(section, '_asdict'):
+                configs[section_name] = section._asdict()
 
         yaml.safe_dump(configs, open(outfile, 'w'), indent=4)
         print("Save OK:", outfile)
 
 
     def copy_sample(self, sample_file : str):
         """ Copy a sample YAML file to the current settings file. """
```

### Comparing `pylogg-0.1.28/pylogg.egg-info/PKG-INFO` & `pylogg-0.1.29/pylogg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pylogg
-Version: 0.1.28
+Version: 0.1.29
 Summary: Logging and YAML-based configuration modules in Python.
 Author-email: Akhlak Mahmood <akhlakm@gatech.edu>
 Project-URL: Homepage, https://github.com/akhlakm/python-logg
 Project-URL: Bug Tracker, https://github.com/akhlakm/python-logg/issues
 Keywords: logging,development
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyyaml
 Provides-Extra: postgres
 Requires-Dist: pandas; extra == "postgres"
 Requires-Dist: sshtunnel; extra == "postgres"
 Requires-Dist: psycopg[binary]; extra == "postgres"
```

### Comparing `pylogg-0.1.28/pyproject.toml` & `pylogg-0.1.29/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "pylogg"
-version = "0.1.28"
+version = "0.1.29"
 authors = [
     { name="Akhlak Mahmood", email="akhlakm@gatech.edu" },
 ]
 description = "Logging and YAML-based configuration modules in Python."
 readme = "README.md"
-requires-python = ">=3.0"
+requires-python = ">=3.10"
 
 keywords = ["logging", "development"]
 
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

