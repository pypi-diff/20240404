# Comparing `tmp/dymmond_settings-1.0.4.tar.gz` & `tmp/dymmond_settings-1.0.5.tar.gz`

## Comparing `dymmond_settings-1.0.4.tar` & `dymmond_settings-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/dymmond_settings/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/dymmond_settings/base.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/dymmond_settings/conf.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/dymmond_settings/enums.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/dymmond_settings/exceptions.py
--rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/dymmond_settings/functional.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/dymmond_settings/module_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/dymmond_settings/py.typed
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/LICENSE
--rw-r--r--   0        0        0     8741 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/README.md
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dymmond_settings-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/dymmond_settings/__init__.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/dymmond_settings/base.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/dymmond_settings/conf.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/dymmond_settings/enums.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/dymmond_settings/exceptions.py
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/dymmond_settings/functional.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/dymmond_settings/module_loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/dymmond_settings/py.typed
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/LICENSE
+-rw-r--r--   0        0        0     8741 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/README.md
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dymmond_settings-1.0.5/PKG-INFO
```

### Comparing `dymmond_settings-1.0.4/dymmond_settings/base.py` & `dymmond_settings-1.0.5/dymmond_settings/base.py`

 * *Files identical despite different names*

### Comparing `dymmond_settings-1.0.4/dymmond_settings/conf.py` & `dymmond_settings-1.0.5/dymmond_settings/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,61 @@
 import os
+from functools import lru_cache
 from typing import TYPE_CHECKING, Any, Optional, Type
 
 from dymmond_settings.functional import LazyObject, empty
 from dymmond_settings.module_loading import import_string
 
 if TYPE_CHECKING:
     from dymmond_settings.base import Settings
 
 OVERRIDE_VARIABLE = "OVERRIDE_SETTINGS_MODULE_VARIABLE"
 ENVIRONMENT_VARIABLE = os.environ.get(OVERRIDE_VARIABLE) or "SETTINGS_MODULE"
 
 
+@lru_cache
+def reload_settings() -> Type["Settings"]:
+    """
+    Reloads the global settings.
+    """
+    settings_module: str = os.environ.get(ENVIRONMENT_VARIABLE, "dymmond_settings.base.Settings")
+    settings: Type["Settings"] = import_string(settings_module)
+
+    return settings
+
+
 class LazySettings(LazyObject):
     """
     A lazy proxy for either global application settings or a custom settings object.
     The user can manually configure settings prior to using them. Otherwise,
     The system uses the settings module pointed to by SETTINGS_MODULE.
     """
 
     def _setup(self, name: Optional[str] = None) -> None:
         """
         Load the settings module pointed to by the environment variable. This
         is used the first time settings are needed, if the user hasn't
         configured settings manually.
         """
-        settings_module: str = os.environ.get(
-            ENVIRONMENT_VARIABLE, "dymmond_settings.base.Settings"
-        )
 
-        settings: Type["Settings"] = import_string(settings_module)
+        settings: Type["Settings"] = reload_settings()
 
         for setting, _ in settings().dict().items():
             assert setting.islower(), "%s should be in lower case." % setting
 
         self._wrapped = settings()
 
+    def configure(self, override_settings: "LazySettings") -> None:
+        """
+        Making sure the settings are overriden by the settings
+        provided by a given application and therefore use it as the application
+        global.
+        """
+        self._wrapped = override_settings
+
     def __repr__(self: "LazySettings") -> str:
         # Hardcode the class name as otherwise it yields 'Settings'.
         if self._wrapped is empty:
             return "<LazySettings [Unevaluated]>"
         return '<LazySettings "{settings_module}">'.format(
             settings_module=self._wrapped.__class__.__name__
         )
```

### Comparing `dymmond_settings-1.0.4/dymmond_settings/functional.py` & `dymmond_settings-1.0.5/dymmond_settings/functional.py`

 * *Files identical despite different names*

### Comparing `dymmond_settings-1.0.4/dymmond_settings/module_loading.py` & `dymmond_settings-1.0.5/dymmond_settings/module_loading.py`

 * *Files identical despite different names*

### Comparing `dymmond_settings-1.0.4/LICENSE` & `dymmond_settings-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dymmond_settings-1.0.4/README.md` & `dymmond_settings-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dymmond_settings-1.0.4/pyproject.toml` & `dymmond_settings-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dymmond_settings-1.0.4/PKG-INFO` & `dymmond_settings-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dymmond_settings
-Version: 1.0.4
+Version: 1.0.5
 Summary: Generic settings system applied to any application
 Project-URL: Homepage, https://github.com/dymmond/dymmond-settings
 Project-URL: Documentation, https://settings.dymmond.com
 Project-URL: Changelog, https://settings.dymmond.com/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/dymmond/dymmond-settings
 Author-email: Tiago Silva <tiago.silva@dymmond.com>
```

