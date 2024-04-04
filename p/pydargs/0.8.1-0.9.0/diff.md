# Comparing `tmp/pydargs-0.8.1.tar.gz` & `tmp/pydargs-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydargs-0.8.1.tar", last modified: Fri Jan 19 11:02:51 2024, max compression
+gzip compressed data, was "pydargs-0.9.0.tar", last modified: Sat Feb 17 13:00:02 2024, max compression
```

## Comparing `pydargs-0.8.1.tar` & `pydargs-0.9.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:51.429449 pydargs-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:51.421449 pydargs-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:51.425449 pydargs-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-01-19 11:02:43.000000 pydargs-0.8.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-19 11:02:43.000000 pydargs-0.8.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-01-19 11:02:43.000000 pydargs-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-19 11:02:43.000000 pydargs-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-01-19 11:02:43.000000 pydargs-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-01-19 11:02:51.429449 pydargs-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-01-19 11:02:43.000000 pydargs-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-01-19 11:02:43.000000 pydargs-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 11:02:51.429449 pydargs-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:51.421449 pydargs-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:51.425449 pydargs-0.8.1/src/pydargs/
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2024-01-19 11:02:43.000000 pydargs-0.8.1/src/pydargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-19 11:02:51.000000 pydargs-0.8.1/src/pydargs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:43.000000 pydargs-0.8.1/src/pydargs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-19 11:02:43.000000 pydargs-0.8.1/src/pydargs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:51.429449 pydargs-0.8.1/src/pydargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-01-19 11:02:51.000000 pydargs-0.8.1/src/pydargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-01-19 11:02:51.000000 pydargs-0.8.1/src/pydargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 11:02:51.000000 pydargs-0.8.1/src/pydargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-19 11:02:51.000000 pydargs-0.8.1/src/pydargs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-19 11:02:51.000000 pydargs-0.8.1/src/pydargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:51.429449 pydargs-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 11:02:43.000000 pydargs-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-01-19 11:02:43.000000 pydargs-0.8.1/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-19 11:02:43.000000 pydargs-0.8.1/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-01-19 11:02:43.000000 pydargs-0.8.1/tests/test_recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-01-19 11:02:43.000000 pydargs-0.8.1/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:00:02.689183 pydargs-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:00:02.685183 pydargs-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:00:02.685183 pydargs-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-17 12:59:48.000000 pydargs-0.9.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-02-17 12:59:48.000000 pydargs-0.9.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-02-17 12:59:48.000000 pydargs-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-17 12:59:48.000000 pydargs-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-17 12:59:48.000000 pydargs-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-02-17 13:00:02.689183 pydargs-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-02-17 12:59:48.000000 pydargs-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-17 12:59:48.000000 pydargs-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 13:00:02.689183 pydargs-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:00:02.685183 pydargs-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:00:02.685183 pydargs-0.9.0/src/pydargs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-02-17 12:59:48.000000 pydargs-0.9.0/src/pydargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-17 13:00:02.000000 pydargs-0.9.0/src/pydargs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 12:59:48.000000 pydargs-0.9.0/src/pydargs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-17 12:59:48.000000 pydargs-0.9.0/src/pydargs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:00:02.689183 pydargs-0.9.0/src/pydargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-02-17 13:00:02.000000 pydargs-0.9.0/src/pydargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-17 13:00:02.000000 pydargs-0.9.0/src/pydargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 13:00:02.000000 pydargs-0.9.0/src/pydargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-17 13:00:02.000000 pydargs-0.9.0/src/pydargs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-17 13:00:02.000000 pydargs-0.9.0/src/pydargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:00:02.689183 pydargs-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 12:59:48.000000 pydargs-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-02-17 12:59:48.000000 pydargs-0.9.0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-17 12:59:48.000000 pydargs-0.9.0/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-02-17 12:59:48.000000 pydargs-0.9.0/tests/test_recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8909 2024-02-17 12:59:48.000000 pydargs-0.9.0/tests/test_subparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-02-17 12:59:48.000000 pydargs-0.9.0/tests/test_types.py
```

### Comparing `pydargs-0.8.1/.github/workflows/publish.yaml` & `pydargs-0.9.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/.github/workflows/test.yaml` & `pydargs-0.9.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/.gitignore` & `pydargs-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/.pre-commit-config.yaml` & `pydargs-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/LICENSE` & `pydargs-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/PKG-INFO` & `pydargs-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: pydargs
-Version: 0.8.1
-Summary: Pydargs allows configuring a dataclass through command line arguments.
-Author-email: Anton Steenvoorden <Anton.Steenvoorden@ah.nl>, Guus Verstegen <gjaverstegen@gmail.com>, Rogier van der Geer <rogier@vander-geer.nl>
-License: BSD
-Project-URL: Repository, https://github.com/rogiervandergeer/pydargs
-Keywords: cli,dataclass
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Typing :: Typed
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: mypy==1.6.1; extra == "dev"
-Requires-Dist: pre-commit==3.5.0; extra == "dev"
-Requires-Dist: ruff==0.1.5; extra == "dev"
-Requires-Dist: pytest==7.4.3; extra == "dev"
-Provides-Extra: pydantic
-Requires-Dist: pydantic>=2.0; extra == "pydantic"
-
 # pydargs
 
 Pydargs allows configuring a (Pydantic) dataclass through command line arguments.
 
 ## Installation
 
 Pydargs can be installed with your favourite package manager. For example:
@@ -93,14 +68,16 @@
 - **Optional types**, denoted as e.g. `typing.Optional[int]` or `int | None` (for Python 3.10 and above).
   Any argument passed is assumed to be of the provided type and can never be `None`.
 - **Unions of types**, denoted as e.g. `typing.Union[int, str]` or `int | str`. Each argument
   will be parsed into the first type that returns a valid result. Note that this means
   that `str | int` will _always_ result in a value of type `str`.
 - Any other type that can be instantiated from a string, such as `Path`.
 - Dataclasses that, in turn, contain fields of supported types. See [Nested Dataclasses](#nested-dataclasses).
+- A union of multiple dataclasses, that in turn contain fields of supported types,
+  which will be parsed in [Subparsers](#subparsers).
 
 ## Metadata
 
 Additional options can be provided to the dataclass field metadata.
 
 The following metadata fields are supported:
 
@@ -236,15 +213,15 @@
 @dataclass
 class Base:
   config: Config
   verbose: bool = False
 ```
 
 Argument names of fields of the nested dataclass are prefixed with the field name of the nested dataclass in the base
-dataclass. Calling `pydargs.parse(Base, ["-h"])` will result in somthing like:
+dataclass. Calling `pydargs.parse(Base, ["-h"])` will result in something like:
 
 ```text
 usage: your_program.py [-h] --config-field-a CONFIG_FIELD_A
                             [--config-field-b CONFIG_FIELD_B]
                             [--verbose VERBOSE]
 
 options:
@@ -261,7 +238,58 @@
 Please be aware of the following:
 - The default (factory) of fields with a dataclass type is ignored by pydargs, which may yield unexpected results.
   E.g., in the example above, `config: Config = field(default_factory=lambda: Config(field_b="def"))` will not result in a default of "def" for field_b when parsed by pydargs.
   Instead, set `field_b: str = "def"` in the definition of `Config`.
   If you must add a default, for example for instantiating your dataclass elsewhere, do `config: Config = field(default_factory=Config)`, assuming that all fields in `Config` have a default.
 - Nested dataclasses can not be positional (although _fields of_ the nested dataclass can be).
 - Argument names must not collide. In the example above, the `Base` class should not contain a field named `config_field_a`.
+
+## Subparsers
+
+Dataclasses can contain a field with a union-of-dataclasses type, e.g.:
+
+```python
+from dataclasses import dataclass, field
+from typing import Union
+
+
+@dataclass
+class Command1:
+  field_a: int
+  field_b: str = "abc"
+
+
+@dataclass
+class Command2:
+  field_c: str = field(metadata=dict(positional=True))
+
+
+@dataclass
+class Base:
+  command: Union[Command1, Command2]
+  verbose: bool = False
+```
+
+This will result in [sub commands](https://docs.python.org/3/library/argparse.html#sub-commands)
+which allow calling your entrypoint as `entrypoint --verbose Command1 --field-a 12`.
+
+Calling `pydargs.parse(Base, ["-h"])` will result in something like:
+
+```text
+usage: your_program.py [-h] [--verbose VERBOSE] {Command1,command1,Command2,command2} ...
+
+options:
+  -h, --help            show this help message and exit
+  --verbose VERBOSE     (default: False)
+
+action:
+  {Command1,command1,Command2,command2}
+```
+
+Note that:
+- Also lower-case command names are accepted.
+- Any dataclass can not contain more than one subcommand-field.
+- Sub-commands can be nested and mixed with nested dataclasses.
+- Any positional fields defined after a subcommand-field can not be parsed.
+- Subparsers handle all arguments that come after the command; so all global arguments must come before the command.
+  In the above example this means that  `entrypoint --verbose Command2 string`
+  is valid but `entrypoint Command2 string --verbose` is not.
```

### Comparing `pydargs-0.8.1/README.md` & `pydargs-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: pydargs
+Version: 0.9.0
+Summary: Pydargs allows configuring a dataclass through command line arguments.
+Author-email: Anton Steenvoorden <Anton.Steenvoorden@ah.nl>, Guus Verstegen <gjaverstegen@gmail.com>, Rogier van der Geer <rogier@vander-geer.nl>
+License: BSD
+Project-URL: Repository, https://github.com/rogiervandergeer/pydargs
+Keywords: cli,dataclass
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Typed
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: mypy==1.6.1; extra == "dev"
+Requires-Dist: pre-commit==3.5.0; extra == "dev"
+Requires-Dist: ruff==0.1.5; extra == "dev"
+Requires-Dist: pytest==7.4.3; extra == "dev"
+Provides-Extra: pydantic
+Requires-Dist: pydantic>=2.0; extra == "pydantic"
+
 # pydargs
 
 Pydargs allows configuring a (Pydantic) dataclass through command line arguments.
 
 ## Installation
 
 Pydargs can be installed with your favourite package manager. For example:
@@ -68,14 +93,16 @@
 - **Optional types**, denoted as e.g. `typing.Optional[int]` or `int | None` (for Python 3.10 and above).
   Any argument passed is assumed to be of the provided type and can never be `None`.
 - **Unions of types**, denoted as e.g. `typing.Union[int, str]` or `int | str`. Each argument
   will be parsed into the first type that returns a valid result. Note that this means
   that `str | int` will _always_ result in a value of type `str`.
 - Any other type that can be instantiated from a string, such as `Path`.
 - Dataclasses that, in turn, contain fields of supported types. See [Nested Dataclasses](#nested-dataclasses).
+- A union of multiple dataclasses, that in turn contain fields of supported types,
+  which will be parsed in [Subparsers](#subparsers).
 
 ## Metadata
 
 Additional options can be provided to the dataclass field metadata.
 
 The following metadata fields are supported:
 
@@ -211,15 +238,15 @@
 @dataclass
 class Base:
   config: Config
   verbose: bool = False
 ```
 
 Argument names of fields of the nested dataclass are prefixed with the field name of the nested dataclass in the base
-dataclass. Calling `pydargs.parse(Base, ["-h"])` will result in somthing like:
+dataclass. Calling `pydargs.parse(Base, ["-h"])` will result in something like:
 
 ```text
 usage: your_program.py [-h] --config-field-a CONFIG_FIELD_A
                             [--config-field-b CONFIG_FIELD_B]
                             [--verbose VERBOSE]
 
 options:
@@ -236,7 +263,58 @@
 Please be aware of the following:
 - The default (factory) of fields with a dataclass type is ignored by pydargs, which may yield unexpected results.
   E.g., in the example above, `config: Config = field(default_factory=lambda: Config(field_b="def"))` will not result in a default of "def" for field_b when parsed by pydargs.
   Instead, set `field_b: str = "def"` in the definition of `Config`.
   If you must add a default, for example for instantiating your dataclass elsewhere, do `config: Config = field(default_factory=Config)`, assuming that all fields in `Config` have a default.
 - Nested dataclasses can not be positional (although _fields of_ the nested dataclass can be).
 - Argument names must not collide. In the example above, the `Base` class should not contain a field named `config_field_a`.
+
+## Subparsers
+
+Dataclasses can contain a field with a union-of-dataclasses type, e.g.:
+
+```python
+from dataclasses import dataclass, field
+from typing import Union
+
+
+@dataclass
+class Command1:
+  field_a: int
+  field_b: str = "abc"
+
+
+@dataclass
+class Command2:
+  field_c: str = field(metadata=dict(positional=True))
+
+
+@dataclass
+class Base:
+  command: Union[Command1, Command2]
+  verbose: bool = False
+```
+
+This will result in [sub commands](https://docs.python.org/3/library/argparse.html#sub-commands)
+which allow calling your entrypoint as `entrypoint --verbose Command1 --field-a 12`.
+
+Calling `pydargs.parse(Base, ["-h"])` will result in something like:
+
+```text
+usage: your_program.py [-h] [--verbose VERBOSE] {Command1,command1,Command2,command2} ...
+
+options:
+  -h, --help            show this help message and exit
+  --verbose VERBOSE     (default: False)
+
+action:
+  {Command1,command1,Command2,command2}
+```
+
+Note that:
+- Also lower-case command names are accepted.
+- Any dataclass can not contain more than one subcommand-field.
+- Sub-commands can be nested and mixed with nested dataclasses.
+- Any positional fields defined after a subcommand-field can not be parsed.
+- Subparsers handle all arguments that come after the command; so all global arguments must come before the command.
+  In the above example this means that  `entrypoint --verbose Command2 string`
+  is valid but `entrypoint Command2 string --verbose` is not.
```

### Comparing `pydargs-0.8.1/pyproject.toml` & `pydargs-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/src/pydargs/__init__.py` & `pydargs-0.9.0/src/pydargs/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from argparse import ArgumentParser, BooleanOptionalAction, Namespace, SUPPRESS
 from collections.abc import Sequence
-from dataclasses import MISSING, fields
+from dataclasses import Field, MISSING, fields
 from datetime import date, datetime
 from enum import Enum
 from typing import (
     Any,
     ClassVar,
     Literal,
     Optional,
@@ -43,74 +43,102 @@
         args: Optional list of arguments. Defaults to sys.argv.
         **kwargs: Keyword arguments passed to the ArgumentParser object.
 
     Returns:
         An instance of tp.
     """
     namespace = _create_parser(tp, **kwargs).parse_args(args)
-    return _create_object(tp, namespace)
+    result = _create_object(tp, namespace)
+    if len(namespace.__dict__):
+        raise RuntimeError("Internal pydargs error: Some namespace arguments have not been consumed.")
+    return result
 
 
 def _create_object(tp: Type[Dataclass], namespace: Namespace, prefix: str = "") -> Dataclass:
     for field in fields(tp):
         if hasattr(field.type, "__dataclass_fields__"):
             # Create nested dataclass object
             setattr(
                 namespace,
                 prefix + field.name,
                 _create_object(field.type, namespace, prefix=f"{prefix}{field.name}_"),
             )
-    args = {key[len(prefix) :]: value for key, value in namespace.__dict__.items() if key.startswith(prefix)}
+        elif _is_command(field):
+            chosen_action = getattr(namespace, prefix + field.name)
+            # Remove chosen command name and optionally replace with instantiated object.
+            delattr(namespace, prefix + field.name)
+            if chosen_action is not None:
+                for arg in get_args(field.type):
+                    if arg.__name__ == chosen_action:
+                        setattr(namespace, prefix + field.name, _create_object(arg, namespace, prefix=f"{prefix}+"))
+                        break
+                if not hasattr(namespace, prefix + field.name):
+                    raise ValueError("Invalid command.", chosen_action)
+    # Select the relevant keys for the object and remove prefixes.
+    args = {
+        key[len(prefix) :]: value
+        for key, value in namespace.__dict__.items()
+        if key.startswith(prefix) and key[len(prefix) :] in {field.name for field in fields(tp)}
+    }
     # Remove the keys used so far from the namespace, to prevent clutter when creating a parent object.
     for key in args.keys():
         delattr(namespace, prefix + key)
     return tp(**args)
 
 
 def _create_parser(tp: Type[Dataclass], **kwargs: Any) -> ArgumentParser:
     parser = ArgumentParser(**kwargs, argument_default=SUPPRESS)
     _add_arguments(parser, tp)
     return parser
 
 
 def _add_arguments(parser: ArgumentParser, tp: Type[Dataclass], prefix: str = "") -> ArgumentParser:
-    parser_or_group = parser.add_argument_group(prefix.strip("_")) if prefix else parser
+    parser_or_group = (  # Only add a group if there is a prefix that isn't "" or "+".
+        parser.add_argument_group(prefix.strip("_")) if prefix.replace("+", "") else parser
+    )
+    has_subparser = False
     for field in fields(tp):
         if field.metadata.get("ignore_arg", False):
             continue
+        if _is_command(field):
+            _add_subparsers(parser, field, prefix)
+            has_subparser = True
+            continue
 
         argument_kwargs: dict[str, Any] = dict()
         field_has_default = field.default is not MISSING or field.default_factory is not MISSING
         argument_kwargs["help"] = field.metadata.get("help", "")
         if field.default is not MISSING:
             if len(argument_kwargs["help"]):
                 argument_kwargs["help"] += " "
             argument_kwargs["help"] += f"(default: {field.default})"
-        if "metavar" in field.metadata:
-            argument_kwargs["metavar"] = field.metadata["metavar"]
         positional = field.metadata.get("positional", False)
         short_option = field.metadata.get("short_option")
         if positional:
+            if has_subparser:
+                warn("Positional arguments defined after a subparser cannot be parsed.")
             if short_option:
                 raise ValueError("Short options are not supported for positional arguments.")
-            arguments = [prefix + field.name]
+            arguments = [prefix + field.name.replace("+", "")]
             if field_has_default:
                 # Positional arguments that are not required must have a valid default
                 argument_kwargs["default"] = (
                     field.default_factory()  # This is safe only because the parser is only used once.
                     if field.default_factory is not MISSING
                     else field.default
                 )
                 argument_kwargs["nargs"] = "?"
+            argument_kwargs["metavar"] = field.metadata.get("metavar", (prefix + field.name).replace("+", ""))
 
         else:
-            arguments = [f"--{(prefix+field.name).replace('_', '-')}"]
+            arguments = [f"--{(prefix+field.name).replace('_', '-').replace('+', '')}"]
             if short_option:
                 arguments = [short_option] + arguments
             argument_kwargs["dest"] = prefix + field.name
+            argument_kwargs["metavar"] = field.metadata.get("metavar", (prefix + field.name).replace("+", "").upper())
             argument_kwargs["required"] = not field_has_default
 
         if parser_fct := field.metadata.get("parser", None):
             parser_or_group.add_argument(
                 *arguments,
                 type=parser_fct,
                 **argument_kwargs,
@@ -122,14 +150,16 @@
                     *arguments,
                     type=get_args(field.type)[0],
                     **argument_kwargs,
                 )
             elif origin is Literal:
                 if len({type(arg) for arg in get_args(field.type)}) > 1:
                     raise NotImplementedError("Parsing Literals with mixed types is not supported.")
+                if "metavar" not in field.metadata:
+                    del argument_kwargs["metavar"]  # Remove default metavar in favour of argparse default
                 parser_or_group.add_argument(
                     *arguments,
                     choices=get_args(field.type),
                     type=type(get_args(field.type)[0]),
                     **argument_kwargs,
                 )
             elif origin in UNION_TYPES:
@@ -170,14 +200,16 @@
             else:
                 parser_or_group.add_argument(
                     *arguments,
                     type=_parse_bool,
                     **argument_kwargs,
                 )
         elif issubclass(field.type, Enum):
+            if "metavar" not in field.metadata:
+                del argument_kwargs["metavar"]  # Remove default metavar in favour of argparse default
             parser_or_group.add_argument(
                 *arguments,
                 choices=list(field.type),
                 type=named_partial(_parse_enum_key, _display_name=field.type.__name__, enum_type=field.type),
                 **argument_kwargs,
             )
         elif field.type is bytes:
@@ -192,14 +224,38 @@
                 *arguments,
                 type=field.type,
                 **argument_kwargs,
             )
     return parser
 
 
+def _add_subparsers(parser, field: Field, prefix: str = "") -> None:
+    subparsers = parser.add_subparsers(
+        dest=prefix + field.name,
+        title=field.name,
+        required=field.default is MISSING and field.default_factory is MISSING,
+        help=field.metadata.get("help"),
+    )
+
+    for command in get_args(field.type):
+        subparser = subparsers.add_parser(
+            str(command.__name__),
+            argument_default=SUPPRESS,
+            aliases=[str(command.__name__).lower()],
+        )
+        _add_arguments(subparser, command, prefix=f"{prefix}+")
+
+
+def _is_command(field: Field) -> bool:
+    # A command is a Union of dataclass fields.
+    return get_origin(field.type) in UNION_TYPES and all(
+        hasattr(arg, "__dataclass_fields__") for arg in get_args(field.type)
+    )
+
+
 @rename(name="bool")
 def _parse_bool(arg: str) -> bool:
     if arg.lower() == "true" or arg == "1":
         return True
     elif arg.lower() == "false" or arg == "0":
         return False
     raise TypeError(f"Unable to convert {arg} to boolean.")
```

### Comparing `pydargs-0.8.1/src/pydargs/utils.py` & `pydargs-0.9.0/src/pydargs/utils.py`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/src/pydargs.egg-info/PKG-INFO` & `pydargs-0.9.0/src/pydargs.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydargs
-Version: 0.8.1
+Version: 0.9.0
 Summary: Pydargs allows configuring a dataclass through command line arguments.
 Author-email: Anton Steenvoorden <Anton.Steenvoorden@ah.nl>, Guus Verstegen <gjaverstegen@gmail.com>, Rogier van der Geer <rogier@vander-geer.nl>
 License: BSD
 Project-URL: Repository, https://github.com/rogiervandergeer/pydargs
 Keywords: cli,dataclass
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -93,14 +93,16 @@
 - **Optional types**, denoted as e.g. `typing.Optional[int]` or `int | None` (for Python 3.10 and above).
   Any argument passed is assumed to be of the provided type and can never be `None`.
 - **Unions of types**, denoted as e.g. `typing.Union[int, str]` or `int | str`. Each argument
   will be parsed into the first type that returns a valid result. Note that this means
   that `str | int` will _always_ result in a value of type `str`.
 - Any other type that can be instantiated from a string, such as `Path`.
 - Dataclasses that, in turn, contain fields of supported types. See [Nested Dataclasses](#nested-dataclasses).
+- A union of multiple dataclasses, that in turn contain fields of supported types,
+  which will be parsed in [Subparsers](#subparsers).
 
 ## Metadata
 
 Additional options can be provided to the dataclass field metadata.
 
 The following metadata fields are supported:
 
@@ -236,15 +238,15 @@
 @dataclass
 class Base:
   config: Config
   verbose: bool = False
 ```
 
 Argument names of fields of the nested dataclass are prefixed with the field name of the nested dataclass in the base
-dataclass. Calling `pydargs.parse(Base, ["-h"])` will result in somthing like:
+dataclass. Calling `pydargs.parse(Base, ["-h"])` will result in something like:
 
 ```text
 usage: your_program.py [-h] --config-field-a CONFIG_FIELD_A
                             [--config-field-b CONFIG_FIELD_B]
                             [--verbose VERBOSE]
 
 options:
@@ -261,7 +263,58 @@
 Please be aware of the following:
 - The default (factory) of fields with a dataclass type is ignored by pydargs, which may yield unexpected results.
   E.g., in the example above, `config: Config = field(default_factory=lambda: Config(field_b="def"))` will not result in a default of "def" for field_b when parsed by pydargs.
   Instead, set `field_b: str = "def"` in the definition of `Config`.
   If you must add a default, for example for instantiating your dataclass elsewhere, do `config: Config = field(default_factory=Config)`, assuming that all fields in `Config` have a default.
 - Nested dataclasses can not be positional (although _fields of_ the nested dataclass can be).
 - Argument names must not collide. In the example above, the `Base` class should not contain a field named `config_field_a`.
+
+## Subparsers
+
+Dataclasses can contain a field with a union-of-dataclasses type, e.g.:
+
+```python
+from dataclasses import dataclass, field
+from typing import Union
+
+
+@dataclass
+class Command1:
+  field_a: int
+  field_b: str = "abc"
+
+
+@dataclass
+class Command2:
+  field_c: str = field(metadata=dict(positional=True))
+
+
+@dataclass
+class Base:
+  command: Union[Command1, Command2]
+  verbose: bool = False
+```
+
+This will result in [sub commands](https://docs.python.org/3/library/argparse.html#sub-commands)
+which allow calling your entrypoint as `entrypoint --verbose Command1 --field-a 12`.
+
+Calling `pydargs.parse(Base, ["-h"])` will result in something like:
+
+```text
+usage: your_program.py [-h] [--verbose VERBOSE] {Command1,command1,Command2,command2} ...
+
+options:
+  -h, --help            show this help message and exit
+  --verbose VERBOSE     (default: False)
+
+action:
+  {Command1,command1,Command2,command2}
+```
+
+Note that:
+- Also lower-case command names are accepted.
+- Any dataclass can not contain more than one subcommand-field.
+- Sub-commands can be nested and mixed with nested dataclasses.
+- Any positional fields defined after a subcommand-field can not be parsed.
+- Subparsers handle all arguments that come after the command; so all global arguments must come before the command.
+  In the above example this means that  `entrypoint --verbose Command2 string`
+  is valid but `entrypoint Command2 string --verbose` is not.
```

### Comparing `pydargs-0.8.1/tests/test_parse.py` & `pydargs-0.9.0/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/tests/test_pydantic.py` & `pydargs-0.9.0/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/tests/test_recursive.py` & `pydargs-0.9.0/tests/test_recursive.py`

 * *Files identical despite different names*

### Comparing `pydargs-0.8.1/tests/test_types.py` & `pydargs-0.9.0/tests/test_types.py`

 * *Files identical despite different names*

