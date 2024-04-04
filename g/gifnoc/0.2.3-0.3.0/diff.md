# Comparing `tmp/gifnoc-0.2.3.tar.gz` & `tmp/gifnoc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gifnoc-0.2.3.tar", max compression
+gzip compressed data, was "gifnoc-0.3.0.tar", max compression
```

## Comparing `gifnoc-0.2.3.tar` & `gifnoc-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2268 2024-03-13 17:48:39.575307 gifnoc-0.2.3/README.md
--rw-r--r--   0        0        0      467 2024-03-20 01:16:51.384569 gifnoc-0.2.3/gifnoc/__init__.py
--rw-r--r--   0        0        0     3289 2024-03-22 19:29:13.603238 gifnoc-0.2.3/gifnoc/__main__.py
--rw-r--r--   0        0        0     2988 2024-03-20 22:11:14.339440 gifnoc-0.2.3/gifnoc/acquire.py
--rw-r--r--   0        0        0     6306 2024-04-02 18:13:35.610877 gifnoc-0.2.3/gifnoc/arg.py
--rw-r--r--   0        0        0     1390 2024-04-02 18:17:30.844733 gifnoc-0.2.3/gifnoc/config.py
--rw-r--r--   0        0        0     9878 2024-03-22 19:29:35.957640 gifnoc-0.2.3/gifnoc/core.py
--rw-r--r--   0        0        0      584 2024-03-11 19:31:05.660822 gifnoc-0.2.3/gifnoc/define.py
--rw-r--r--   0        0        0     4420 2024-03-14 18:27:32.891465 gifnoc-0.2.3/gifnoc/docstrings.py
--rw-r--r--   0        0        0     1348 2024-03-04 20:00:45.907307 gifnoc-0.2.3/gifnoc/merge.py
--rw-r--r--   0        0        0     3782 2024-04-02 18:12:58.922625 gifnoc-0.2.3/gifnoc/parse.py
--rw-r--r--   0        0        0     3138 2024-04-02 20:04:27.068678 gifnoc-0.2.3/gifnoc/registry.py
--rw-r--r--   0        0        0     1626 2024-04-02 19:45:27.258785 gifnoc-0.2.3/gifnoc/schema.py
--rw-r--r--   0        0        0      247 2024-03-08 22:39:08.607547 gifnoc-0.2.3/gifnoc/std/__init__.py
--rw-r--r--   0        0        0      819 2024-03-11 19:06:40.540661 gifnoc-0.2.3/gifnoc/std/_time.py
--rw-r--r--   0        0        0     3316 2024-04-02 20:12:00.338364 gifnoc-0.2.3/gifnoc/type_wrappers.py
--rw-r--r--   0        0        0     4273 2024-03-20 22:11:06.107781 gifnoc-0.2.3/gifnoc/utils.py
--rw-r--r--   0        0        0       18 2024-04-02 20:12:29.802856 gifnoc-0.2.3/gifnoc/version.py
--rw-r--r--   0        0        0      544 2024-04-02 20:12:29.780884 gifnoc-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 gifnoc-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2268 2024-03-13 17:48:39.575307 gifnoc-0.3.0/README.md
+-rw-r--r--   0        0        0      431 2024-04-04 05:32:30.662546 gifnoc-0.3.0/gifnoc/__init__.py
+-rw-r--r--   0        0        0     3289 2024-03-22 19:29:13.603238 gifnoc-0.3.0/gifnoc/__main__.py
+-rw-r--r--   0        0        0     3227 2024-04-04 03:48:00.163881 gifnoc-0.3.0/gifnoc/acquire.py
+-rw-r--r--   0        0        0     6539 2024-04-04 03:48:14.365182 gifnoc-0.3.0/gifnoc/arg.py
+-rw-r--r--   0        0        0      126 2024-04-04 03:48:14.345716 gifnoc-0.3.0/gifnoc/config.py
+-rw-r--r--   0        0        0     4420 2024-03-14 18:27:32.891465 gifnoc-0.3.0/gifnoc/docstrings.py
+-rw-r--r--   0        0        0     6588 2024-04-04 03:48:14.376041 gifnoc-0.3.0/gifnoc/interface.py
+-rw-r--r--   0        0        0     1348 2024-03-04 20:00:45.907307 gifnoc-0.3.0/gifnoc/merge.py
+-rw-r--r--   0        0        0     3782 2024-04-03 21:43:10.065094 gifnoc-0.3.0/gifnoc/parse.py
+-rw-r--r--   0        0        0     1392 2024-04-04 03:48:14.376295 gifnoc-0.3.0/gifnoc/proxy.py
+-rw-r--r--   0        0        0     6863 2024-04-04 03:48:14.395375 gifnoc-0.3.0/gifnoc/registry.py
+-rw-r--r--   0        0        0     1617 2024-04-04 03:48:14.390506 gifnoc-0.3.0/gifnoc/schema.py
+-rw-r--r--   0        0        0      247 2024-03-08 22:39:08.607547 gifnoc-0.3.0/gifnoc/std/__init__.py
+-rw-r--r--   0        0        0      822 2024-04-04 03:48:14.346765 gifnoc-0.3.0/gifnoc/std/_time.py
+-rw-r--r--   0        0        0     4006 2024-04-04 05:34:58.949225 gifnoc-0.3.0/gifnoc/type_wrappers.py
+-rw-r--r--   0        0        0     4273 2024-03-20 22:11:06.107781 gifnoc-0.3.0/gifnoc/utils.py
+-rw-r--r--   0        0        0       18 2024-04-04 15:42:38.322839 gifnoc-0.3.0/gifnoc/version.py
+-rw-r--r--   0        0        0      622 2024-04-04 15:42:38.300894 gifnoc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 gifnoc-0.3.0/PKG-INFO
```

### Comparing `gifnoc-0.2.3/README.md` & `gifnoc-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.3/gifnoc/__main__.py` & `gifnoc-0.3.0/gifnoc/__main__.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.3/gifnoc/acquire.py` & `gifnoc-0.3.0/gifnoc/acquire.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import fields, is_dataclass
 from pathlib import Path
 
 from ovld import meta, ovld
 
-from .parse import Context, EnvContext, FileContext, parse_file
+from .merge import merge
+from .parse import Context, EnvContext, FileContext, parse_file, parse_source
 from .utils import UnionTypes, convertible_from_string
 
 
 def is_structure(cls):
     return issubclass(cls, dict) or issubclass(cls, list) or is_dataclass(cls)
 
 
@@ -124,7 +125,15 @@
 
 
 def acquire(model, obj, context):
     if isinstance(model, UnionTypes):
         model, *_ = model.__args__
     method = _acquire[getattr(model, "__origin__", model), type(obj), type(context)]
     return method(model, obj, context)
+
+
+def parse_sources(model, *sources):
+    result = {}
+    for src in sources:
+        for ctx, dct in parse_source(src):
+            result = merge(result, acquire(model, dct, ctx))
+    return result
```

### Comparing `gifnoc-0.2.3/gifnoc/arg.py` & `gifnoc-0.3.0/gifnoc/arg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 from dataclasses import dataclass, field, fields, is_dataclass, replace
 from types import GenericAlias
 from typing import Union
 
 from ovld import ovld
 
-from gifnoc.registry import global_registry
-from gifnoc.utils import ConfigurationError, convertible_from_string, type_at_path
+from .registry import Registry
+from .utils import ConfigurationError, convertible_from_string, type_at_path
 
 
 @dataclass
 class Option:
     option: str = None
     aliases: list[str] = field(default_factory=list)
     action: object = None
@@ -43,17 +43,19 @@
         option.type = model
     return option
 
 
 @ovld
 def compile_option(model: object, path: str, option: Option):  # noqa: F811
     if isinstance(model, GenericAlias):
-        assert model.__origin__ is list
-        option = compile_option(model.__args__[0], path, option)
-        option.action = "append"
+        if model.__origin__ is list:
+            option = compile_option(model.__args__[0], path, option)
+            option.action = "append"
+        else:
+            return None
     elif option.type is None:
         option.type = str
     return option
 
 
 @ovld
 def compile_option(model: object, path: str, option: str):  # noqa: F811
@@ -90,14 +92,16 @@
         model = global_model
         doc = ""
 
     def _compile_option(p, v):
         ap = abspath(mount, p)
         typ, doc = type_at_path(global_model, ap.split("."), allow_union=False)
         opt = compile_option[typ, str, type(v)](typ, mount, v)
+        if not opt:
+            return None
         if opt.help is None:
             opt.help = doc
         return ap, opt
 
     def _merge(opts1, opts2):
         results = {abspath(mount, p): v for p, v in opts1.items()}
         opts2 = {abspath(mount, p): v for p, v in opts2.items()}
@@ -114,15 +118,17 @@
             results[k] = v
         return results
 
     options = {}
     if command.auto:
         options.update(auto(model, mount))
     options = _merge(options, command.options)
-    options = dict(_compile_option(p, v) for p, v in options.items())
+    options = dict(
+        compiled for p, v in options.items() if (compiled := _compile_option(p, v))
+    )
 
     commands = {
         cmd: compile_command(global_model, mount, v)
         for cmd, v in command.commands.items()
     }
     return replace(
         command,
@@ -131,20 +137,22 @@
         auto=False,
         commands=commands,
         options=options,
     )
 
 
 @ovld
-def add_arguments_to_parser(parser: argparse.ArgumentParser, command: Command):
+def add_arguments_to_parser(
+    parser: argparse.ArgumentParser, command: Command, registry: Registry
+):
     for dest, option in command.options.items():
         option.dest = f"&{dest}"
-        add_arguments_to_parser(parser, option)
+        add_arguments_to_parser(parser, option, registry)
     if command.commands:
-        global_model = global_registry.model()
+        global_model = registry.model()
         dest = f"&{command.mount}.{command.command_field}"
         path = dest[1:].split(".")
         try:
             holder_type, doc = type_at_path(model=global_model, path=path)
             if not issubclass(holder_type, str):
                 raise ConfigurationError(
                     errors=[
@@ -166,20 +174,20 @@
                 is_definition_problem=True,
             )
         subparsers = parser.add_subparsers(
             required=True, dest=dest, help=doc, metavar=command.command_field.upper()
         )
         for command_name, subcmd in command.commands.items():
             subparser = subparsers.add_parser(command_name, help=subcmd.help)
-            add_arguments_to_parser(subparser, subcmd)
+            add_arguments_to_parser(subparser, subcmd, registry)
 
 
 @ovld
 def add_arguments_to_parser(  # noqa: F811
-    parser: argparse.ArgumentParser, option: Option
+    parser: argparse.ArgumentParser, option: Option, registry: Registry
 ):
     if option.metavar is None and option.option is not None:
         option.metavar = option.option.strip("-").upper()
     parser.add_argument(
         *([option.option] if option.option else []),
         *option.aliases,
         action=option.action,
@@ -189,15 +197,17 @@
         type=option.type,
         dest=option.dest,
     )
 
 
 @ovld
 def add_arguments_to_parser(  # noqa: F811
-    parser: argparse.ArgumentParser, options: dict
+    parser: argparse.ArgumentParser, options: dict, registry: Registry
 ):
-    add_arguments_to_parser(parser, Command(mount="", options=options))
+    add_arguments_to_parser(parser, Command(mount="", options=options), registry)
 
 
 @ovld
-def add_arguments_to_parser(parser: argparse.ArgumentParser, mount: str):  # noqa: F811
-    add_arguments_to_parser(parser, Command(mount=mount, auto=True))
+def add_arguments_to_parser(  # noqa: F811
+    parser: argparse.ArgumentParser, mount: str, registry: Registry
+):
+    add_arguments_to_parser(parser, Command(mount=mount, auto=True), registry)
```

### Comparing `gifnoc-0.2.3/gifnoc/config.py` & `gifnoc-0.3.0/gifnoc/proxy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-from .core import current_configuration
+from .interface import current_configuration
 
 
-class _Proxy:
+class MissingConfigurationError(Exception):
+    pass
+
+
+class Proxy:
     def __init__(self, *pth):
         self._pth = pth
-        self._cached_built = None
+        self._cached_data = None
         self._cached = None
 
     def _obj(self):
         container = current_configuration()
-        if container is None:
-            raise Exception("No configuration was loaded.")
-        root = cfg = container.built
-        if cfg is self._cached_built:
+        if container is None:  # pragma: no cover
+            raise MissingConfigurationError("No configuration was loaded.")
+        root = cfg = container.data
+        if cfg is self._cached_data:
             return self._cached
         try:
             for k in self._pth:
                 if isinstance(cfg, dict):
                     cfg = cfg[k]
+                elif isinstance(cfg, list):
+                    cfg = cfg[int(k)]
                 else:
                     cfg = getattr(cfg, k)
-            if cfg is None:
-                key = ".".join(self._pth)
-                raise Exception(f"No configuration was loaded for key '{key}'.")
-            self._cached_built = root
+            self._cached_data = root
             self._cached = cfg
             return cfg
         except (KeyError, AttributeError):
             key = ".".join(self._pth)
-            raise Exception(f"No configuration was loaded for key '{key}'.")
+            raise MissingConfigurationError(
+                f"No configuration was loaded for key '{key}'."
+            )
 
     def __str__(self):
         return f"Proxy for {self._obj()}"
 
     def __repr__(self):
-        return f"_Proxy({self._obj()!r})"
+        return f"Proxy({self._obj()!r})"
 
     def __getattr__(self, attr):
         if attr.startswith("__") and attr.endswith("__"):
             raise AttributeError(attr)
         return getattr(self._obj(), attr)
-
-
-def __getattr__(key):
-    return _Proxy(key)
-
-
-__path__ = None
```

### Comparing `gifnoc-0.2.3/gifnoc/docstrings.py` & `gifnoc-0.3.0/gifnoc/docstrings.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.3/gifnoc/merge.py` & `gifnoc-0.3.0/gifnoc/merge.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.3/gifnoc/parse.py` & `gifnoc-0.3.0/gifnoc/parse.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.3/gifnoc/schema.py` & `gifnoc-0.3.0/gifnoc/schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import apischema
 from apischema import json_schema, settings
 from apischema.schemas import Schema
 from ovld import ovld
 
 from .docstrings import get_attribute_docstrings
-from .type_wrappers import TaggedSubclass
+from .type_wrappers import wrapper_cache
 
 logger = logging.getLogger(__name__)
 
 
 NoneType = type(None)
 
 
@@ -35,15 +35,15 @@
 
 @ovld
 def _pull_defs(obj: object):
     return {}
 
 
 def deserialization_schema(typ):
-    for cls in TaggedSubclass._cache.values():
+    for cls in wrapper_cache.values():
         cls.register_schemas()
     rval = json_schema.deserialization_schema(typ)
     defs = _pull_defs(rval)
     rval.setdefault("$defs", {}).update(defs)
     return rval
```

### Comparing `gifnoc-0.2.3/gifnoc/std/_time.py` & `gifnoc-0.3.0/gifnoc/std/_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time as stdtime
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 
-from ..define import define
+from ..interface import define
 from ..type_wrappers import TaggedSubclass
 
 
 @dataclass
 class NormalTime:
     def now(self):
         return datetime.now()
```

### Comparing `gifnoc-0.2.3/gifnoc/type_wrappers.py` & `gifnoc-0.3.0/gifnoc/type_wrappers.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,36 +8,41 @@
     deserializer,
     schema,
     serialize,
     serializer,
 )
 from apischema.conversions import Conversion
 from apischema.json_schema import deserialization_schema
+from apischema.objects import object_fields
 
 T = TypeVar("T")
 
 
-class _TaggedSubclass:
-    _cache = {}
+wrapper_cache = {}
 
+
+class _WrapperBase:
     def __class_getitem__(cls, item: Type[T]) -> Type[T]:
-        if item not in TaggedSubclass._cache:
+        name = cls.__name__.lstrip("_")
+        key = (cls, item)
+        if key not in wrapper_cache:
             typ = type(
-                f"TaggedSubclass[{item.__name__}]",
-                (TaggedSubclass,),
-                {"__passthrough__": item, "__wrapper__": _TaggedSubclass},
+                f"{name}[{item.__name__}]",
+                (cls,),
+                {"__passthrough__": item, "__wrapper__": cls},
             )
-            TaggedSubclass._cache[item] = typ
+            wrapper_cache[key] = typ
             deserializer(
                 Conversion(typ._deserialize, source=dict[str, Any], target=typ)
             )
-            typ.register_schemas()
 
-        return TaggedSubclass._cache[item]
+        return wrapper_cache[key]
+
 
+class _TaggedSubclass(_WrapperBase):
     @classmethod
     def register_schemas(cls):
         base = cls.__passthrough__
         possibilities = []
         base_mod = base.__module__
         queue = deque([base])
         while queue:
@@ -83,24 +88,46 @@
             except (ModuleNotFoundError, AttributeError) as exc:
                 raise ValidationError(str(exc))
         if not issubclass(actual_class, base):
             raise ValidationError(f"'{cls_name}' is not a '{base.__name__}' subclass")
         return deserialize(actual_class, data)
 
 
+class _Extensible(_WrapperBase):
+    @classmethod
+    def register_schemas(cls):
+        base = cls.__passthrough__
+        original = deserialization_schema(base)
+        schema(extra={**original, "additionalProperties": True})(cls)
+
+    @classmethod
+    def _deserialize(cls, data: dict):
+        base = cls.__passthrough__
+        fields = object_fields(base)
+        data = {k: v for k, v in data.items() if k in fields}
+        return deserialize(base, data)
+
+
 if TYPE_CHECKING:
     # Lets us pretend that TaggedSubclass[T] is T
     TaggedSubclass = Annotated[T, None]
+    Extensible = Annotated[T, None]
 
 else:
     TaggedSubclass = _TaggedSubclass
+    Extensible = _Extensible
 
 
 @serializer
-def _serialize(x: TaggedSubclass) -> dict:
+def _serialize_TaggedSubclass(x: TaggedSubclass) -> dict:
     qn = type(x).__qualname__
     assert "." not in qn, "Only top-level symbols can be serialized"
     mod = type(x).__module__
     return {
         "class": f"{mod}:{qn}",
         **serialize(x),
     }
+
+
+@serializer
+def _serialize_Extensible(x: Extensible) -> dict:
+    return serialize(x)
```

### Comparing `gifnoc-0.2.3/gifnoc/utils.py` & `gifnoc-0.3.0/gifnoc/utils.py`

 * *Files identical despite different names*

### Comparing `gifnoc-0.2.3/PKG-INFO` & `gifnoc-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gifnoc
-Version: 0.2.3
+Version: 0.3.0
 Summary: Handle configuration for multiple libraries
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

