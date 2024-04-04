# Comparing `tmp/types-flake8-builtins-2.3.0.20240331.tar.gz` & `tmp/types-flake8-builtins-2.4.0.20240404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-builtins-2.3.0.20240331.tar", last modified: Sun Mar 31 02:18:00 2024, max compression
+gzip compressed data, was "types-flake8-builtins-2.4.0.20240404.tar", last modified: Thu Apr  4 02:16:32 2024, max compression
```

## Comparing `types-flake8-builtins-2.3.0.20240331.tar` & `types-flake8-builtins-2.4.0.20240404.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:00.279516 types-flake8-builtins-2.3.0.20240331/
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-03-31 02:17:59.000000 types-flake8-builtins-2.3.0.20240331/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-31 02:17:59.000000 types-flake8-builtins-2.3.0.20240331/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-03-31 02:18:00.279516 types-flake8-builtins-2.3.0.20240331/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:00.279516 types-flake8-builtins-2.3.0.20240331/flake8_builtins-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-31 02:17:59.000000 types-flake8-builtins-2.3.0.20240331/flake8_builtins-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-03-31 02:17:59.000000 types-flake8-builtins-2.3.0.20240331/flake8_builtins-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 02:17:59.000000 types-flake8-builtins-2.3.0.20240331/flake8_builtins-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 02:18:00.279516 types-flake8-builtins-2.3.0.20240331/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-31 02:17:59.000000 types-flake8-builtins-2.3.0.20240331/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 02:18:00.279516 types-flake8-builtins-2.3.0.20240331/types_flake8_builtins.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-03-31 02:18:00.000000 types-flake8-builtins-2.3.0.20240331/types_flake8_builtins.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 02:18:00.000000 types-flake8-builtins-2.3.0.20240331/types_flake8_builtins.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 02:18:00.000000 types-flake8-builtins-2.3.0.20240331/types_flake8_builtins.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-31 02:18:00.000000 types-flake8-builtins-2.3.0.20240331/types_flake8_builtins.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-04 02:16:30.000000 types-flake8-builtins-2.4.0.20240404/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:16:32.316810 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-04 02:16:32.000000 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 02:16:32.000000 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 02:16:32.000000 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 02:16:32.000000 types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/top_level.txt
```

### Comparing `types-flake8-builtins-2.3.0.20240331/CHANGELOG.md` & `types-flake8-builtins-2.4.0.20240404/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 2.4.0.20240404 (2024-04-04)
+
+[stubsabot] Bump flake8-builtins to 2.4.* (#11697)
+
+Co-authored-by: stubsabot <>
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 2.3.0.20240331 (2024-03-31)
 
 Update flake8-builtins to 2.3.* (#11669)
 
 ## 2.2.0.0 (2023-11-04)
 
 [stubsabot] Bump flake8-builtins to 2.2.* (#10975)
```

### Comparing `types-flake8-builtins-2.3.0.20240331/PKG-INFO` & `types-flake8-builtins-2.4.0.20240404/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-builtins
-Version: 2.3.0.20240331
+Version: 2.4.0.20240404
 Summary: Typing stubs for flake8-builtins
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-builtins.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,20 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-builtins`.
 
 This version of `types-flake8-builtins` aims to provide accurate annotations
-for `flake8-builtins==2.3.*`.
+for `flake8-builtins==2.4.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-builtins. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `0685754ab3b9c8c242d064c7b5d78d39d3ab0b57` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
```

### Comparing `types-flake8-builtins-2.3.0.20240331/flake8_builtins-stubs/__init__.pyi` & `types-flake8-builtins-2.4.0.20240404/flake8_builtins-stubs/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,27 +12,29 @@
     name: ClassVar[str]
     version: ClassVar[str]
     assign_msg: ClassVar[str]
     argument_msg: ClassVar[str]
     class_attribute_msg: ClassVar[str]
     import_msg: ClassVar[str]
     module_name_msg: ClassVar[str]
+    lambda_argument_msg: ClassVar[str]
 
     names: ClassVar[list[str]]
     ignore_list: ClassVar[set[str]]
     ignored_module_names: ClassVar[set[str]]
 
     def __init__(self, tree: ast.AST, filename: str) -> None: ...
     @classmethod
     def add_options(cls, option_manager: _OptionManager) -> None: ...
     @classmethod
     def parse_options(cls, options: Namespace) -> None: ...
     def run(self) -> Iterator[_Error]: ...
     def check_assignment(self, statement: ast.Assign | ast.AnnAssign | ast.NamedExpr) -> Iterator[_Error]: ...
     def check_function_definition(self, statement: ast.FunctionDef | ast.AsyncFunctionDef) -> Iterator[_Error]: ...
+    def check_lambda_definition(self, statement: ast.Lambda) -> Iterator[_Error]: ...
     def check_for_loop(self, statement: ast.For | ast.AsyncFor) -> Iterator[_Error]: ...
     def check_with(self, statement: ast.With | ast.AsyncWith) -> Iterator[_Error]: ...
     def check_exception(self, statement: ast.excepthandler) -> Iterator[_Error]: ...
     def check_comprehension(
         self, statement: ast.ListComp | ast.SetComp | ast.DictComp | ast.GeneratorExp
     ) -> Iterator[_Error]: ...
     def check_import(self, statement: ast.Import | ast.ImportFrom) -> Iterator[_Error]: ...
```

### Comparing `types-flake8-builtins-2.3.0.20240331/setup.py` & `types-flake8-builtins-2.4.0.20240404/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-builtins`.
 
 This version of `types-flake8-builtins` aims to provide accurate annotations
-for `flake8-builtins==2.3.*`.
+for `flake8-builtins==2.4.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-builtins. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `0685754ab3b9c8c242d064c7b5d78d39d3ab0b57` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="2.3.0.20240331",
+      version="2.4.0.20240404",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-builtins.md",
```

### Comparing `types-flake8-builtins-2.3.0.20240331/types_flake8_builtins.egg-info/PKG-INFO` & `types-flake8-builtins-2.4.0.20240404/types_flake8_builtins.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-builtins
-Version: 2.3.0.20240331
+Version: 2.4.0.20240404
 Summary: Typing stubs for flake8-builtins
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-builtins.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,20 +22,20 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-builtins`.
 
 This version of `types-flake8-builtins` aims to provide accurate annotations
-for `flake8-builtins==2.3.*`.
+for `flake8-builtins==2.4.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-builtins. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `027115e6249f17f9dee2c0372c4609335a1b9e7d` and was tested
+This package was generated from typeshed commit `0685754ab3b9c8c242d064c7b5d78d39d3ab0b57` and was tested
 with mypy 1.9.0, pyright 1.1.356, and
 pytype 2024.3.19.
```

