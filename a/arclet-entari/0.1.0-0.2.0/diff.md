# Comparing `tmp/arclet_entari-0.1.0.tar.gz` & `tmp/arclet_entari-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_entari-0.1.0.tar", last modified: Wed Dec  6 08:25:07 2023, max compression
+gzip compressed data, was "arclet_entari-0.2.0.tar", last modified: Thu Apr  4 15:32:15 2024, max compression
```

## Comparing `arclet_entari-0.1.0.tar` & `arclet_entari-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-12-06 08:24:37.271826 arclet_entari-0.1.0/LICENSE
--rw-r--r--   0        0        0      411 2023-12-06 08:24:37.271826 arclet_entari-0.1.0/README.md
--rw-r--r--   0        0        0     1918 2023-12-06 08:24:37.271826 arclet_entari-0.1.0/arclet/entari/__init__.py
--rw-r--r--   0        0        0    14581 2023-12-06 08:24:37.271826 arclet_entari-0.1.0/arclet/entari/command.py
--rw-r--r--   0        0        0     3241 2023-12-06 08:24:37.275826 arclet_entari-0.1.0/arclet/entari/core.py
--rw-r--r--   0        0        0     9705 2023-12-06 08:24:37.275826 arclet_entari-0.1.0/arclet/entari/event.py
--rw-r--r--   0        0        0     9833 2023-12-06 08:24:37.275826 arclet_entari-0.1.0/arclet/entari/message.py
--rw-r--r--   0        0        0     1335 2023-12-06 08:24:37.275826 arclet_entari-0.1.0/arclet/entari/plugin.py
--rw-r--r--   0        0        0    10059 2023-12-06 08:24:37.275826 arclet_entari-0.1.0/arclet/entari/session.py
--rw-r--r--   0        0        0     1796 2023-12-06 08:25:07.299780 arclet_entari-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1130 1970-01-01 00:00:00.000000 arclet_entari-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/LICENSE
+-rw-r--r--   0        0        0      880 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/README.md
+-rw-r--r--   0        0        0     1918 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/__init__.py
+-rw-r--r--   0        0        0    14779 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/command.py
+-rw-r--r--   0        0        0     3226 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/core.py
+-rw-r--r--   0        0        0     9705 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/event.py
+-rw-r--r--   0        0        0     9783 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/message.py
+-rw-r--r--   0        0        0     1335 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/plugin.py
+-rw-r--r--   0        0        0    10059 2024-04-04 15:31:50.612942 arclet_entari-0.2.0/arclet/entari/session.py
+-rw-r--r--   0        0        0     1820 2024-04-04 15:32:15.633198 arclet_entari-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 arclet_entari-0.2.0/PKG-INFO
```

### Comparing `arclet_entari-0.1.0/LICENSE` & `arclet_entari-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.1.0/arclet/entari/__init__.py` & `arclet_entari-0.2.0/arclet/entari/__init__.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.1.0/arclet/entari/command.py` & `arclet_entari-0.2.0/arclet/entari/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from copy import deepcopy
 from dataclasses import dataclass, field
 import inspect
-from typing import Any, Callable, Generic, Optional, TypeVar, Union, cast, get_args, overload
+from typing import Any, Callable, Generic, Literal, Optional, TypeVar, Union, cast, get_args, overload
 
 from arclet.alconna import (
     Alconna,
     Arg,
     Args,
     Arparma,
     CommandMeta,
@@ -30,15 +30,16 @@
     Publisher,
     Scope,
     Subscriber,
     SupplyAuxiliary,
 )
 from arclet.letoderea.handler import depend_handler
 from arclet.letoderea.provider import ProviderFactory
-from nepattern import DirectPattern, main
+from nepattern import DirectPattern
+from nepattern.util import CUnionType
 from pygtrie import CharTrie
 from satori.client import Account
 from satori.element import At, Text
 from tarina.generic import get_origin
 from tarina.string import split_once
 
 from .event import MessageEvent
@@ -170,26 +171,26 @@
             except Exception as e:
                 _res = Arparma(self.cmd.path, message, False, error_info=e)
             may_help_text: Optional[str] = cap.get("output", None)
         if _res.matched:
             context["alc_result"] = CommandResult(self.cmd, _res, may_help_text)
             return context
         elif may_help_text:
-            await account.send(context["$event"], may_help_text)
+            await account.send(context["$event"], MessageChain(may_help_text))
             return False
 
     @property
     def scopes(self) -> set[Scope]:
         return {Scope.prepare}
 
 
 class AlconnaProvider(Provider[Any]):
-    def __init__(self, type: str, extra: Optional[dict] = None):
+    def __init__(self, type_: str, extra: Optional[dict] = None):
         super().__init__()
-        self.type = type
+        self.type = type_
         self.extra = extra or {}
 
     async def __call__(self, context: Contexts):
         if "alc_result" not in context:
             return
         result: CommandResult = context["alc_result"]
         if self.type == "result":
@@ -217,15 +218,15 @@
         if self.extra["name"] in result.result.all_matched_args:
             return result.result.all_matched_args[self.extra["name"]]
 
 
 class AlconnaProviderFactory(ProviderFactory):
     def validate(self, param: Param):
         annotation = get_origin(param.annotation)
-        if annotation in main._Contents:
+        if annotation in (Union, CUnionType, Literal):
             annotation = get_origin(get_args(param.annotation)[0])
         if annotation is CommandResult:
             return AlconnaProvider("result")
         if annotation is Arparma:
             return AlconnaProvider("arparma")
         if annotation is Alconna:
             return AlconnaProvider("alconna")
@@ -250,15 +251,19 @@
     def __init__(self, need_tome: bool = False, remove_tome: bool = False):
         self.trie: CharTrie = CharTrie()
         self.publisher = Publisher("EntariCommands", MessageEvent)
         self.publisher.providers.append(AlconnaProviderFactory())
         plugins["~command.EntariCommands"] = self.publisher
         self.need_tome = need_tome
         self.remove_tome = remove_tome
-        config.namespaces["Entari"] = Namespace(self.__namespace__)
+        config.namespaces["Entari"] = Namespace(
+            self.__namespace__,
+            to_text=lambda x: x.text if x.__class__ is Text else None,
+            converter=lambda x: MessageChain(x),
+        )
 
         @self.publisher.register(auxiliaries=[MessageJudger()])
         async def listener(event: MessageEvent):
             msg = str(event.content.exclude(At)).lstrip()
             if not msg:
                 return
             if matches := list(self.trie.prefixes(msg)):
@@ -336,30 +341,28 @@
     def on(
         self,
         command: Alconna,
         need_tome: bool = False,
         remove_tome: bool = False,
         auxiliaries: Optional[list[BaseAuxiliary]] = None,
         providers: Optional[list[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]] = None,
-    ) -> Callable[[TCallable], TCallable]:
-        ...
+    ) -> Callable[[TCallable], TCallable]: ...
 
     @overload
     def on(
         self,
         command: str,
         need_tome: bool = False,
         remove_tome: bool = False,
         auxiliaries: Optional[list[BaseAuxiliary]] = None,
         providers: Optional[list[Provider, type[Provider], ProviderFactory, type[ProviderFactory]]] = None,
         *,
         args: Optional[dict[str, Union[TAValue, Args, Arg]]] = None,
         meta: Optional[CommandMeta] = None,
-    ) -> Callable[[TCallable], TCallable]:
-        ...
+    ) -> Callable[[TCallable], TCallable]: ...
 
     def on(
         self,
         command: Union[Alconna, str],
         need_tome: bool = False,
         remove_tome: bool = False,
         auxiliaries: Optional[list[BaseAuxiliary]] = None,
```

### Comparing `arclet_entari-0.1.0/arclet/entari/core.py` & `arclet_entari-0.2.0/arclet/entari/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 self.event_system.publish(ev)
                 for plugin in plugins.values():
                     loop.create_task(plugin.publish(ev))
                 return
 
             logger.warning(f"received unsupported event {raw.type}: {raw}")
 
-        asyncio.create_task(event_parse_task(account, event))
+        await event_parse_task(account, event)
 
     # async def handle_lifecycle(self, account: Account, state: LoginStatus):
     # if state == LoginStatus.ONLINE:
     #     route = Selector().land(account.platform).account(account.self_id)
     #     _account = SatoriAccount(route, self.protocol)
     #     self.protocol.avilla.accounts[route] = AccountInfo(
     #         route, _account, self.protocol, platform(account.platform)
```

### Comparing `arclet_entari-0.1.0/arclet/entari/event.py` & `arclet_entari-0.2.0/arclet/entari/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
     guild: Guild | None = None
     member: Member | None = None
     quote: Quote | None = None
 
     providers = [MessageContentProvider, QuoteProvider]
 
     def __post_init__(self):
-        self.content = MessageChain(self.message.content)
+        self.content = MessageChain(self.message.message)
         if self.content.has(Quote):
             self.quote = self.content.get(Quote, 1)[0]
             self.content = self.content.exclude(Quote)
 
     async def gather(self, context: Contexts):
         await super().gather(context)
         context["user"] = self.user
@@ -256,15 +256,15 @@
     quote: Quote | None = None
     guild: Guild | None = None
     member: Member | None = None
 
     providers = [MessageContentProvider, QuoteProvider]
 
     def __post_init__(self):
-        self.content = MessageChain(self.message.content)
+        self.content = MessageChain(self.message.message)
         if self.content.has(Quote):
             self.quote = self.content.get(Quote, 1)[0]
             self.content = self.content.exclude(Quote)
 
     async def gather(self, context: Contexts):
         await super().gather(context)
         context["user"] = self.user
@@ -334,15 +334,15 @@
     quote: Quote | None = None
     guild: Guild | None = None
     member: Member | None = None
 
     providers = [MessageContentProvider, QuoteProvider]
 
     def __post_init__(self):
-        self.content = MessageChain(self.message.content)
+        self.content = MessageChain(self.message.message)
         if self.content.has(Quote):
             self.quote = self.content.get(Quote, 1)[0]
             self.content = self.content.exclude(Quote)
 
     async def gather(self, context: Contexts):
         await super().gather(context)
         context["user"] = self.user
```

### Comparing `arclet_entari-0.1.0/arclet/entari/message.py` & `arclet_entari-0.2.0/arclet/entari/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,24 +35,21 @@
     def __str__(self) -> str:
         return "".join(str(seg) for seg in self)
 
     def __repr__(self) -> str:
         return "[" + ", ".join(repr(seg) for seg in self) + "]"
 
     @overload
-    def __add__(self, other: str) -> MessageChain[TE | Text]:
-        ...
+    def __add__(self, other: str) -> MessageChain[TE | Text]: ...
 
     @overload
-    def __add__(self, other: TE | Iterable[TE]) -> MessageChain[TE]:
-        ...
+    def __add__(self, other: TE | Iterable[TE]) -> MessageChain[TE]: ...
 
     @overload
-    def __add__(self, other: TE1 | Iterable[TE1]) -> MessageChain[TE | TE1]:
-        ...
+    def __add__(self, other: TE1 | Iterable[TE1]) -> MessageChain[TE | TE1]: ...
 
     def __add__(self, other: str | TE | TE1 | Iterable[TE | TE1]) -> MessageChain:
         result: MessageChain = self.copy()
         if isinstance(other, str):
             if result and isinstance(text := result[-1], Text):
                 text.text += other
             else:
@@ -66,24 +63,21 @@
             for seg in other:
                 result += seg
         else:
             raise TypeError(f"Unsupported type {type(other)!r}")
         return result
 
     @overload
-    def __radd__(self, other: str) -> MessageChain[Text | TE]:
-        ...
+    def __radd__(self, other: str) -> MessageChain[Text | TE]: ...
 
     @overload
-    def __radd__(self, other: TE | Iterable[TE]) -> MessageChain[TE]:
-        ...
+    def __radd__(self, other: TE | Iterable[TE]) -> MessageChain[TE]: ...
 
     @overload
-    def __radd__(self, other: TE1 | Iterable[TE1]) -> MessageChain[TE1 | TE]:
-        ...
+    def __radd__(self, other: TE1 | Iterable[TE1]) -> MessageChain[TE1 | TE]: ...
 
     def __radd__(self, other: str | TE1 | Iterable[TE1]) -> MessageChain:
         result = MessageChain(other)
         return result + self
 
     def __iadd__(self, other: str | TE | Iterable[TE]) -> Self:
         if isinstance(other, str):
@@ -156,15 +150,15 @@
 
         返回:
             消息切片 `args`
         """
 
     def __getitem__(
         self,
-        args: (type[TE1] | tuple[type[TE1], int] | tuple[type[TE1], slice] | int | slice),
+        args: type[TE1] | tuple[type[TE1], int] | tuple[type[TE1], slice] | int | slice,
     ) -> TE | TE1 | MessageChain[TE1] | Self:
         arg1, arg2 = args if isinstance(args, tuple) else (args, None)
         if isinstance(arg1, int) and arg2 is None:
             return super().__getitem__(arg1)
         if isinstance(arg1, slice) and arg2 is None:
             return MessageChain(super().__getitem__(arg1))
         if TYPE_CHECKING:
```

### Comparing `arclet_entari-0.1.0/arclet/entari/plugin.py` & `arclet_entari-0.2.0/arclet/entari/plugin.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.1.0/arclet/entari/session.py` & `arclet_entari-0.2.0/arclet/entari/session.py`

 * *Files identical despite different names*

### Comparing `arclet_entari-0.1.0/pyproject.toml` & `arclet_entari-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "arclet-entari"
-version = "0.1.0"
+version = "0.2.0"
 description = "Simple IM Framework based on satori-python"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "arclet-letoderea>=0.9.2",
-    "arclet-alconna>=1.7.38",
-    "satori-python-core>=0.9.2",
-    "satori-python-client>=0.9.2",
-    "arclet-alconna-tools>=0.6.8",
+    "arclet-alconna>=1.8.6",
+    "satori-python-core>=0.11.4",
+    "satori-python-client>=0.11.4",
+    "arclet-alconna-tools>=0.7.1",
     "pygtrie>=2.5.0",
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -35,28 +35,28 @@
 [tool.pdm.build]
 includes = [
     "arclet",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "isort>=5.12.0",
-    "black>=23.11.0",
-    "ruff>=0.1.7",
+    "isort>=5.13.2",
+    "black>=24.3.0",
+    "ruff>=0.3.5",
     "fix-future-annotations>=0.5.0",
 ]
 
 [tool.pdm.scripts]
 test = "pytest -v -n auto -W ignore ./tests/"
 
 [tool.pdm.scripts.format]
 composite = [
     "isort ./arclet/",
     "black ./arclet/",
-    "ruff ./arclet/",
+    "ruff check ./arclet/",
 ]
 
 [tool.black]
 line-length = 110
 target-version = [
     "py39",
     "py310",
@@ -72,14 +72,21 @@
 skip_gitignore = true
 force_sort_within_sections = true
 extra_standard_library = [
     "typing_extensions",
 ]
 
 [tool.ruff]
+line-length = 110
+target-version = "py39"
+include = [
+    "arclet/**.py",
+]
+
+[tool.ruff.lint]
 select = [
     "E",
     "W",
     "F",
     "UP",
     "C",
     "T",
@@ -89,17 +96,12 @@
 ]
 ignore = [
     "C901",
     "T201",
     "E731",
     "E402",
 ]
-line-length = 110
-target-version = "py39"
-include = [
-    "arclet/**.py",
-]
 
 [tool.pyright]
 pythonVersion = "3.9"
 pythonPlatform = "All"
 typeCheckingMode = "basic"
```

### Comparing `arclet_entari-0.1.0/PKG-INFO` & `arclet_entari-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 Metadata-Version: 2.1
 Name: arclet-entari
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple IM Framework based on satori-python
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Requires-Dist: arclet-letoderea>=0.9.2
-Requires-Dist: arclet-alconna>=1.7.38
-Requires-Dist: satori-python-core>=0.9.2
-Requires-Dist: satori-python-client>=0.9.2
-Requires-Dist: arclet-alconna-tools>=0.6.8
+Requires-Dist: arclet-alconna>=1.8.6
+Requires-Dist: satori-python-core>=0.11.4
+Requires-Dist: satori-python-client>=0.11.4
+Requires-Dist: arclet-alconna-tools>=0.7.1
 Requires-Dist: pygtrie>=2.5.0
 Description-Content-Type: text/markdown
 
-# arclet-entari
+<div align="center"> 
+  
+# Entari
+
+  > _lo su etheclim, ti zo entaem rish._
+  
+</div>
+
+[![Licence](https://img.shields.io/github/license/ArcletProject/Entari)](https://github.com/ArcletProject/Entari/blob/main/LICENSE)
+[![PyPI](https://img.shields.io/pypi/v/arclet-entari)](https://pypi.org/project/arclet-entari)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arclet-entari)](https://www.python.org/)
+![Entari](https://img.shields.io/badge/Arclet-Entari-2564c2.svg)
 
 一个基于 `Satori` 协议的简易 IM framework
 
 ## 示例
 
 ```python
 from arclet.entari import ContextSession, Entari, EntariCommands, WebsocketsInfo
```

