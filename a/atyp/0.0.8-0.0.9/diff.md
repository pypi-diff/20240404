# Comparing `tmp/atyp-0.0.8.tar.gz` & `tmp/atyp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atyp-0.0.8.tar", last modified: Mon Oct  9 13:03:08 2023, max compression
+gzip compressed data, was "atyp-0.0.9.tar", last modified: Mon Oct  9 19:44:38 2023, max compression
```

## Comparing `atyp-0.0.8.tar` & `atyp-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-09 13:03:08.673788 atyp-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-08-28 14:10:36.000000 atyp-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-08-28 14:10:36.000000 atyp-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3446 2023-10-09 13:03:08.673657 atyp-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2806 2023-10-08 12:17:52.000000 atyp-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-09 13:03:08.672020 atyp-0.0.8/atyp/
--rw-r--r--   0 solst      (501) staff       (20)      203 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)      520 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2516 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)      597 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/btyp.py
--rw-r--r--   0 solst      (501) staff       (20)      721 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/ctyp.py
--rw-r--r--   0 solst      (501) staff       (20)     1548 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/dtyp.py
--rw-r--r--   0 solst      (501) staff       (20)      508 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/mtyp.py
--rw-r--r--   0 solst      (501) staff       (20)      646 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/ptyp.py
--rw-r--r--   0 solst      (501) staff       (20)     1665 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/qtyp.py
--rw-r--r--   0 solst      (501) staff       (20)      922 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/rtyp.py
--rw-r--r--   0 solst      (501) staff       (20)      415 2023-10-09 13:03:04.000000 atyp-0.0.8/atyp/ztyp.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-09 13:03:08.673462 atyp-0.0.8/atyp.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3446 2023-10-09 13:03:08.000000 atyp-0.0.8/atyp.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      398 2023-10-09 13:03:08.000000 atyp-0.0.8/atyp.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-10-09 13:03:08.000000 atyp-0.0.8/atyp.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-10-09 13:03:08.000000 atyp-0.0.8/atyp.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-08-28 15:00:29.000000 atyp-0.0.8/atyp.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-10-09 13:03:08.000000 atyp-0.0.8/atyp.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-10-09 13:03:08.000000 atyp-0.0.8/atyp.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      801 2023-10-09 13:03:03.000000 atyp-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-10-09 13:03:08.673833 atyp-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2023-08-28 14:10:36.000000 atyp-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-09 19:44:38.513389 atyp-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-08-28 14:10:36.000000 atyp-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-08-28 14:10:36.000000 atyp-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3597 2023-10-09 19:44:38.513269 atyp-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2957 2023-10-09 19:44:28.000000 atyp-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-09 19:44:38.512024 atyp-0.0.9/atyp/
+-rw-r--r--   0 solst      (501) staff       (20)      203 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)      520 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     2627 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)      597 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/btyp.py
+-rw-r--r--   0 solst      (501) staff       (20)      721 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/ctyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     1548 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/dtyp.py
+-rw-r--r--   0 solst      (501) staff       (20)      508 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/mtyp.py
+-rw-r--r--   0 solst      (501) staff       (20)      646 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/ptyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     1665 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/qtyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     1101 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/rtyp.py
+-rw-r--r--   0 solst      (501) staff       (20)      415 2023-10-09 19:44:22.000000 atyp-0.0.9/atyp/ztyp.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-10-09 19:44:38.513068 atyp-0.0.9/atyp.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3597 2023-10-09 19:44:38.000000 atyp-0.0.9/atyp.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      398 2023-10-09 19:44:38.000000 atyp-0.0.9/atyp.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-10-09 19:44:38.000000 atyp-0.0.9/atyp.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2023-10-09 19:44:38.000000 atyp-0.0.9/atyp.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-08-28 15:00:29.000000 atyp-0.0.9/atyp.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-10-09 19:44:38.000000 atyp-0.0.9/atyp.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2023-10-09 19:44:38.000000 atyp-0.0.9/atyp.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      801 2023-10-09 13:04:29.000000 atyp-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-10-09 19:44:38.513427 atyp-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2023-08-28 14:10:36.000000 atyp-0.0.9/setup.py
```

### Comparing `atyp-0.0.8/LICENSE` & `atyp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `atyp-0.0.8/PKG-INFO` & `atyp-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atyp
-Version: 0.0.8
+Version: 0.0.9
 Summary: atyp (type alias)
 Home-page: https://github.com/dsm-72/atyp
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python types type alias type atyp typ optional opt
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,27 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # atyp
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+## Packages that use `atyp`
+
+- `aprep`
+- `aspec`
+- `brvstr`
+- `dynattr`
+- `fuzstr`
+- `ispec`
+- `narr`
+- `nbkit`
+- `nymstr`
+- `synstr`
+
 ## Developer Guide
 
 ### Setup
 
 ``` sh
 # create conda environment
 $ mamba env create -f env.yml
@@ -157,15 +170,15 @@
 from atyp.ztyp import (FlagFunc, FlagFuncQ)
 ```
 
 ### R = Rich
 
 ``` python
 from atyp.rtyp import (
-    RTree, RText, RCons, RProg, TApp
+    RichTree, RichText, RichCons, RichProg, TyperApp
 )
 ```
 
 ### P = Plot
 
 ``` python
 from atyp.ptyp import (
```

### Comparing `atyp-0.0.8/README.md` & `atyp-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # atyp
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+## Packages that use `atyp`
+
+- `aprep`
+- `aspec`
+- `brvstr`
+- `dynattr`
+- `fuzstr`
+- `ispec`
+- `narr`
+- `nbkit`
+- `nymstr`
+- `synstr`
+
 ## Developer Guide
 
 ### Setup
 
 ``` sh
 # create conda environment
 $ mamba env create -f env.yml
@@ -138,15 +151,15 @@
 from atyp.ztyp import (FlagFunc, FlagFuncQ)
 ```
 
 ### R = Rich
 
 ``` python
 from atyp.rtyp import (
-    RTree, RText, RCons, RProg, TApp
+    RichTree, RichText, RichCons, RichProg, TyperApp
 )
 ```
 
 ### P = Plot
 
 ``` python
 from atyp.ptyp import (
```

### Comparing `atyp-0.0.8/atyp/_modidx.py` & `atyp-0.0.9/atyp/_modidx.py`

 * *Files identical despite different names*

### Comparing `atyp-0.0.8/atyp/atyp.py` & `atyp-0.0.9/atyp/atyp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_atyp.ipynb.
 
 # %% auto 0
-__all__ = ['Boolic', 'Boolish', 'Bools', 'Numeric', 'Numbers', 'StrLike', 'Strs', 'StrSet', 'PathType', 'PathLike', 'DirPath',
-           'DirNames', 'FileNames', 'WalkParts', 'Intum', 'Strum', 'ByteLike', 'Literals', 'TypingLike', 'GuardLike',
-           'Module', 'Loader', 'ModuleSpec', 'Sig', 'Param']
+__all__ = ['Boolic', 'Boolish', 'Bools', 'Numeric', 'Numbers', 'StrLike', 'Strs', 'StrSet', 'StrTmpl', 'PathType', 'PathLike',
+           'DirPath', 'DirNames', 'FileNames', 'WalkParts', 'Intum', 'Strum', 'ByteLike', 'Literals', 'TypingLike',
+           'GuardLike', 'Module', 'Loader', 'ModuleSpec', 'Sig', 'Param']
 
 # %% ../nbs/00_atyp.ipynb 4
 from typing import (
     TypeAlias, Literal, Union, List, Set,
     Iterable, Tuple
 )
 
@@ -24,63 +24,67 @@
 from numbers import Number
 
 # %% ../nbs/00_atyp.ipynb 11
 Numeric: TypeAlias = Union[int, float, complex, Number]
 Numbers: TypeAlias = List[Numeric]
 
 # %% ../nbs/00_atyp.ipynb 13
+from string import Template
+
+# %% ../nbs/00_atyp.ipynb 14
 StrLike: TypeAlias = Union[str, 'strfix', 'fuzstr', 'nymstr', 'synset']
 Strs: TypeAlias = List[StrLike]
 StrSet: TypeAlias = Set[StrLike]
+StrTmpl: TypeAlias = Union[str, Template]
 
-# %% ../nbs/00_atyp.ipynb 15
+# %% ../nbs/00_atyp.ipynb 16
 import os, pathlib
 
-# %% ../nbs/00_atyp.ipynb 16
+# %% ../nbs/00_atyp.ipynb 17
 PathType: TypeAlias = Union[pathlib.Path, pathlib.PosixPath]
 PathLike: TypeAlias = Union[str, PathType, os.PathLike]
 
-# %% ../nbs/00_atyp.ipynb 17
+# %% ../nbs/00_atyp.ipynb 18
 DirPath: TypeAlias = str
 DirNames: TypeAlias =  List[str]
 FileNames: TypeAlias =  List[str]
 WalkParts: TypeAlias = Iterable[Tuple[DirPath, DirNames, FileNames]]
 
-# %% ../nbs/00_atyp.ipynb 19
+# %% ../nbs/00_atyp.ipynb 20
 from enum import IntEnum, StrEnum
 
-# %% ../nbs/00_atyp.ipynb 20
+# %% ../nbs/00_atyp.ipynb 21
 Intum: TypeAlias = Union[IntEnum, 'LitIntEnum', 'Intum']
 Strum: TypeAlias = Union[StrEnum, 'LitStrEnum', 'Strum', 'LiteralEnum']
 
-# %% ../nbs/00_atyp.ipynb 22
+# %% ../nbs/00_atyp.ipynb 23
 ByteLike: TypeAlias = Union[bytes, 'BytesUnit', 'Bytes']
 
-# %% ../nbs/00_atyp.ipynb 24
+# %% ../nbs/00_atyp.ipynb 25
 from typing import TypeVar, TypeGuard
 
-# %% ../nbs/00_atyp.ipynb 25
+# %% ../nbs/00_atyp.ipynb 26
 Literals = TypeVar('Literals')
 TypingLike: TypeAlias = Union['TTyp', 'TType', 'TypingUnit', 'Typing']
 GuardLike: TypeAlias = Union['TTypGuard', 'TTypeGuard']
 
-# %% ../nbs/00_atyp.ipynb 27
+# %% ../nbs/00_atyp.ipynb 28
 import types
 
-# %% ../nbs/00_atyp.ipynb 28
+# %% ../nbs/00_atyp.ipynb 29
 Module: TypeAlias = types.ModuleType
 
-# %% ../nbs/00_atyp.ipynb 30
+# %% ../nbs/00_atyp.ipynb 31
 import importlib
 from importlib.abc import Loader
 
-# %% ../nbs/00_atyp.ipynb 31
+# %% ../nbs/00_atyp.ipynb 32
 Loader: TypeAlias = Loader
 
 ModuleSpec: TypeAlias = importlib.machinery.ModuleSpec
 
-# %% ../nbs/00_atyp.ipynb 33
+# %% ../nbs/00_atyp.ipynb 34
 import inspect
 
-# %% ../nbs/00_atyp.ipynb 34
+# %% ../nbs/00_atyp.ipynb 35
 Sig: TypeAlias = inspect.Signature
 Param: TypeAlias = inspect.Parameter
```

### Comparing `atyp-0.0.8/atyp/btyp.py` & `atyp-0.0.9/atyp/btyp.py`

 * *Files identical despite different names*

### Comparing `atyp-0.0.8/atyp/ctyp.py` & `atyp-0.0.9/atyp/ctyp.py`

 * *Files identical despite different names*

### Comparing `atyp-0.0.8/atyp/dtyp.py` & `atyp-0.0.9/atyp/dtyp.py`

 * *Files identical despite different names*

### Comparing `atyp-0.0.8/atyp/ptyp.py` & `atyp-0.0.9/atyp/ptyp.py`

 * *Files identical despite different names*

### Comparing `atyp-0.0.8/atyp/qtyp.py` & `atyp-0.0.9/atyp/qtyp.py`

 * *Files identical despite different names*

### Comparing `atyp-0.0.8/atyp.egg-info/PKG-INFO` & `atyp-0.0.9/atyp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atyp
-Version: 0.0.8
+Version: 0.0.9
 Summary: atyp (type alias)
 Home-page: https://github.com/dsm-72/atyp
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python types type alias type atyp typ optional opt
 Classifier: Development Status :: 4 - Beta
@@ -17,14 +17,27 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # atyp
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
+## Packages that use `atyp`
+
+- `aprep`
+- `aspec`
+- `brvstr`
+- `dynattr`
+- `fuzstr`
+- `ispec`
+- `narr`
+- `nbkit`
+- `nymstr`
+- `synstr`
+
 ## Developer Guide
 
 ### Setup
 
 ``` sh
 # create conda environment
 $ mamba env create -f env.yml
@@ -157,15 +170,15 @@
 from atyp.ztyp import (FlagFunc, FlagFuncQ)
 ```
 
 ### R = Rich
 
 ``` python
 from atyp.rtyp import (
-    RTree, RText, RCons, RProg, TApp
+    RichTree, RichText, RichCons, RichProg, TyperApp
 )
 ```
 
 ### P = Plot
 
 ``` python
 from atyp.ptyp import (
```

### Comparing `atyp-0.0.8/settings.ini` & `atyp-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = atyp
 lib_name = atyp
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = atyp
 nbs_path = nbs
 recursive = True
```

### Comparing `atyp-0.0.8/setup.py` & `atyp-0.0.9/setup.py`

 * *Files identical despite different names*

