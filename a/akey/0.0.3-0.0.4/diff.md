# Comparing `tmp/akey-0.0.3.tar.gz` & `tmp/akey-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akey-0.0.3.tar", last modified: Wed Dec  6 14:05:04 2023, max compression
+gzip compressed data, was "akey-0.0.4.tar", last modified: Thu Apr  4 12:53:57 2024, max compression
```

## Comparing `akey-0.0.3.tar` & `akey-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-06 14:05:04.043770 akey-0.0.3/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-27 18:20:15.000000 akey-0.0.3/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-27 18:20:15.000000 akey-0.0.3/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     2044 2023-12-06 14:05:04.043650 akey-0.0.3/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1431 2023-11-30 20:00:19.000000 akey-0.0.3/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-06 14:05:04.042538 akey-0.0.3/akey/
--rw-r--r--   0 solst      (501) staff       (20)      384 2023-12-06 14:04:57.000000 akey-0.0.3/akey/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     1728 2023-12-06 14:04:57.000000 akey-0.0.3/akey/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     2264 2023-12-06 14:04:57.000000 akey-0.0.3/akey/dims.py
--rw-r--r--   0 solst      (501) staff       (20)    11071 2023-12-06 14:04:57.000000 akey-0.0.3/akey/keys.py
--rw-r--r--   0 solst      (501) staff       (20)     7802 2023-12-06 14:04:57.000000 akey-0.0.3/akey/mock.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-12-06 14:05:04.043480 akey-0.0.3/akey.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     2044 2023-12-06 14:05:04.000000 akey-0.0.3/akey.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      320 2023-12-06 14:05:04.000000 akey-0.0.3/akey.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-12-06 14:05:04.000000 akey-0.0.3/akey.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2023-12-06 14:05:04.000000 akey-0.0.3/akey.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-30 13:48:14.000000 akey-0.0.3/akey.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      176 2023-12-06 14:05:04.000000 akey-0.0.3/akey.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2023-12-06 14:05:04.000000 akey-0.0.3/akey.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      977 2023-12-05 15:14:18.000000 akey-0.0.3/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-12-06 14:05:04.043804 akey-0.0.3/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2023-11-27 18:20:15.000000 akey-0.0.3/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:53:57.191879 akey-0.0.4/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-27 18:20:15.000000 akey-0.0.4/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-27 18:20:15.000000 akey-0.0.4/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     2044 2024-04-04 12:53:57.191491 akey-0.0.4/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1431 2023-11-30 20:00:19.000000 akey-0.0.4/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:53:57.190448 akey-0.0.4/akey/
+-rw-r--r--   0 solst      (501) staff       (20)      384 2024-04-04 12:53:50.000000 akey-0.0.4/akey/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     2082 2024-04-04 12:53:50.000000 akey-0.0.4/akey/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     2477 2024-04-04 12:53:50.000000 akey-0.0.4/akey/dims.py
+-rw-r--r--   0 solst      (501) staff       (20)    11290 2024-04-04 12:53:50.000000 akey-0.0.4/akey/keys.py
+-rw-r--r--   0 solst      (501) staff       (20)     7658 2024-04-04 12:53:50.000000 akey-0.0.4/akey/mock.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-04 12:53:57.191316 akey-0.0.4/akey.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     2044 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      320 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-11-30 13:48:14.000000 akey-0.0.4/akey.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      186 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-04 12:53:57.000000 akey-0.0.4/akey.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      987 2023-12-08 21:07:08.000000 akey-0.0.4/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-04 12:53:57.191980 akey-0.0.4/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2023-11-27 18:20:15.000000 akey-0.0.4/setup.py
```

### Comparing `akey-0.0.3/LICENSE` & `akey-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `akey-0.0.3/PKG-INFO` & `akey-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akey
-Version: 0.0.3
+Version: 0.0.4
 Summary: akey
 Home-page: https://github.com/dsm-72/akey
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: akey extra extras single cell sc scanpy anndata RNA-seq seq
 Classifier: Development Status :: 4 - Beta
```

### Comparing `akey-0.0.3/README.md` & `akey-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `akey-0.0.3/akey/_modidx.py` & `akey-0.0.4/akey/_modidx.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/akey',
                 'doc_host': 'https://dsm-72.github.io',
                 'git_url': 'https://github.com/dsm-72/akey',
                 'lib_path': 'akey'},
-  'syms': { 'akey.dims': { 'akey.dims.keydims': ('dims.html#keydims', 'akey/dims.py'),
+  'syms': { 'akey.dims': { 'akey.dims.hascolumns': ('dims.html#hascolumns', 'akey/dims.py'),
+                           'akey.dims.hasshape': ('dims.html#hasshape', 'akey/dims.py'),
+                           'akey.dims.keydims': ('dims.html#keydims', 'akey/dims.py'),
                            'akey.dims.numcols': ('dims.html#numcols', 'akey/dims.py')},
             'akey.keys': { 'akey.keys.getattrkeys': ('keys.html#getattrkeys', 'akey/keys.py'),
                            'akey.keys.getattrskeys': ('keys.html#getattrskeys', 'akey/keys.py'),
                            'akey.keys.getkey': ('keys.html#getkey', 'akey/keys.py'),
                            'akey.keys.getkeyedattrs': ('keys.html#getkeyedattrs', 'akey/keys.py'),
                            'akey.keys.getpubattrs': ('keys.html#getpubattrs', 'akey/keys.py'),
+                           'akey.keys.hasget': ('keys.html#hasget', 'akey/keys.py'),
+                           'akey.keys.haskeys': ('keys.html#haskeys', 'akey/keys.py'),
                            'akey.keys.isattrkeys': ('keys.html#isattrkeys', 'akey/keys.py'),
                            'akey.keys.iskeyed': ('keys.html#iskeyed', 'akey/keys.py'),
                            'akey.keys.isobjattrkeys': ('keys.html#isobjattrkeys', 'akey/keys.py'),
                            'akey.keys.safeview': ('keys.html#safeview', 'akey/keys.py')},
             'akey.mock': { 'akey.mock.charjoin': ('mock.html#charjoin', 'akey/mock.py'),
                            'akey.mock.dropnils': ('mock.html#dropnils', 'akey/mock.py'),
                            'akey.mock.genlabels': ('mock.html#genlabels', 'akey/mock.py'),
```

### Comparing `akey-0.0.3/akey/dims.py` & `akey-0.0.4/akey/dims.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_dims.ipynb.
 
 # %% auto 0
-__all__ = ['numcols', 'keydims']
+__all__ = ['hasshape', 'hascolumns', 'numcols', 'keydims']
 
 # %% ../nbs/02_dims.ipynb 6
 import io, warnings, itertools
 from contextlib import redirect_stderr
 
 # %% ../nbs/02_dims.ipynb 8
 from typing import Callable
 
 # %% ../nbs/02_dims.ipynb 10
 try: import numpy as np, pandas as pd
-except ImportError: warnings.warn("Some packages are not installed")
+except ImportError: ...
 
 # %% ../nbs/02_dims.ipynb 12
-from hasr import (hasshape, hascolumns)
-from nlit import (__GETITEM__)
+from nlit import (__GETITEM__, SHAPE, COLUMNS)
+from chck import notnone
 
-# %% ../nbs/02_dims.ipynb 14
+# %% ../nbs/02_dims.ipynb 13
+def hasshape(obj) -> bool:
+    try: return notnone(getattr(obj, SHAPE, None))
+    except: False
+    
+def hascolumns(obj) -> bool:
+    try: return notnone(getattr(obj, COLUMNS, None))
+    except: False
+
+# %% ../nbs/02_dims.ipynb 15
 from .mock import mock_adata
 from .keys import getkey
 
-# %% ../nbs/02_dims.ipynb 17
+# %% ../nbs/02_dims.ipynb 18
 def numcols(obj, axis: int = 1) -> int:
     '''
     Calculate the number of columns (or specified axis dimension) of an object.
 
     Parameters
     ----------
     obj : Any
@@ -51,15 +60,15 @@
     4
     '''
     if hasshape(obj): return obj.shape[axis]
     if hascolumns(obj): return len(obj.columns)
     return len(obj)
 
 
-# %% ../nbs/02_dims.ipynb 18
+# %% ../nbs/02_dims.ipynb 19
 def keydims(obj, name: str, axis: int = 1) -> int:
     '''
     Retrieve the number of columns/dimensions for a specified key within an object.
 
     Parameters
     ----------
     obj : Any
```

### Comparing `akey-0.0.3/akey/keys.py` & `akey-0.0.4/akey/keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_keys.ipynb.
 
 # %% auto 0
-__all__ = ['getpubattrs', 'safeview', 'isattrkeys', 'isobjattrkeys', 'iskeyed', 'getkeyedattrs', 'getattrkeys', 'getattrskeys',
-           'getkey']
+__all__ = ['hasget', 'haskeys', 'getpubattrs', 'safeview', 'isattrkeys', 'isobjattrkeys', 'iskeyed', 'getkeyedattrs',
+           'getattrkeys', 'getattrskeys', 'getkey']
 
 # %% ../nbs/01_keys.ipynb 6
 import io, warnings, itertools
 from contextlib import redirect_stderr
 
 # %% ../nbs/01_keys.ipynb 8
 from typing import Callable
 
 # %% ../nbs/01_keys.ipynb 10
 try: import numpy as np, pandas as pd
 except ImportError: warnings.warn("Some packages are not installed")
 
 # %% ../nbs/01_keys.ipynb 12
+from nlit import (KEYS, __GETITEM__, GET, KEYS)
 from chck import (isstr, isbool, iscall, isnone, notnone, isinst, isad,  iscallattr, ispublic)
-from hasr import (hasget, haskeys)
 
-from nlit import (KEYS, __GETITEM__)
-
-from calr import callattr, callwith
-from excs import HushedErrors
 from asto import cast
+from sigr import callattr, callwith
+from excs import HushedErrors
 
-# %% ../nbs/01_keys.ipynb 14
+# %% ../nbs/01_keys.ipynb 13
+def hasget(obj) -> bool:
+    try: return callable(getattr(obj, GET, None))
+    except: False
+    
+def haskeys(obj) -> bool:
+    try: return callable(getattr(obj, KEYS, None))
+    except: False
+
+# %% ../nbs/01_keys.ipynb 15
 from .mock import mock_adata
 
-# %% ../nbs/01_keys.ipynb 17
+# %% ../nbs/01_keys.ipynb 18
 def getpubattrs(obj) -> list[str]:
     '''Retrieve the list of public attributes of an object.
 
     Parameters
     ----------
     obj : Any
         The object whose public attributes are to be retrieved.
@@ -56,15 +63,15 @@
 
     >>> pattrs = getpubattrs(adata)
     >>> pattrs[:8]
     ['T', 'X', 'chunk_X', 'chunked_X', 'concatenate', 'copy', 'file', 'filename']
     '''
     return list(filter(ispublic, dir(obj)))
 
-# %% ../nbs/01_keys.ipynb 19
+# %% ../nbs/01_keys.ipynb 20
 def safeview(obj, name: str) -> str:
     '''Adjust the attribute name for special cases, particularly for AnnData objects.
 
     Parameters
     ----------
     obj : Any
         The object to be checked for special cases.
@@ -80,15 +87,15 @@
     Notes
     -----
     This function is specifically designed to handle a warning issued when accessing
     `isview` on an AnnData object. In such cases, it changes `isview` to `is_view`.
     '''    
     return name if not (isad(obj) and name == 'isview') else 'is_view'
 
-# %% ../nbs/01_keys.ipynb 20
+# %% ../nbs/01_keys.ipynb 21
 def isattrkeys(obj, attr: str) -> bool:
     '''Check if an attribute of an object has a `keys` method.
 
     Parameters
     ----------
     obj : Any
         The object to be checked.
@@ -111,15 +118,15 @@
     ...     bar = dict()
     >>> isattrkeys(Foo, 'bar')    
     True
     '''
     attr = safeview(obj, attr)
     return haskeys(getattr(obj, attr, None))
 
-# %% ../nbs/01_keys.ipynb 21
+# %% ../nbs/01_keys.ipynb 22
 def isobjattrkeys(obj, attr: str) -> bool:
     '''Check if an object has a specific attribute that has a `keys` method.
 
     Parameters
     ----------
     obj : Any
         The object to be checked.
@@ -137,15 +144,15 @@
     >>> adata, params = mock_adata()
     >>> isobjattrkeys(adata, 'uns') # AnnData.uns_keys()
     True
     '''
     attr = safeview(obj, attr)
     return iscallattr(obj, f'{attr}_{KEYS}')
 
-# %% ../nbs/01_keys.ipynb 22
+# %% ../nbs/01_keys.ipynb 23
 def iskeyed(obj, attr: str) -> bool:
     '''Check if an attribute of an object is 'keyed', meaning it either directly has a `keys` 
     method or  the object has a corresponding method in the form of `<attr>_keys` e.g.
     `obj.<name>.keys(...)` or `obj.<name>_keys(...)`.
 
     Parameters
     ----------
@@ -167,15 +174,15 @@
     >>> pattr = pattrs[0]
     >>> pattr, isattrkeys(adata, 'obs'), isobjattrkeys(adata, pattr), iskeyed(adata, pattr)
     ('T', True, False, False)
     '''
     attr = safeview(obj, attr)
     return isattrkeys(obj, attr) or isobjattrkeys(obj, attr)
 
-# %% ../nbs/01_keys.ipynb 24
+# %% ../nbs/01_keys.ipynb 25
 def getkeyedattrs(obj) -> list[str]:
     '''Retrieve a list of attributes of an object that have a `keys` method.
 
     Parameters
     ----------
     obj : Any
         The object whose attributes are to be checked.
@@ -194,15 +201,15 @@
     >>> adata, params = mock_adata()
     >>> getkeyedattrs(adata)
     ['layers', 'obs', 'obsm', 'obsp', 'uns', 'var', 'varm', 'varp']
     '''
     with redirect_stderr(io.StringIO()): 
         return list((a for a in getpubattrs(obj) if iskeyed(obj, a)))
 
-# %% ../nbs/01_keys.ipynb 26
+# %% ../nbs/01_keys.ipynb 27
 def getattrkeys(obj, attr: str, zipattr: bool = False) -> list[str] | list[tuple[str, str]]:
     '''Retrieve keys from an attribute of an object, optionally zipping with the attribute name.
 
     Parameters
     ----------
     obj : Any
         The object whose attribute keys are to be retrieved.
@@ -228,15 +235,15 @@
     [('obs', 'barcodes'), ('obs', 'con'), ('obs', 'day')]    
     '''
     if isattrkeys(obj, attr): res = callattr(getattr(obj, attr), KEYS)
     elif isobjattrkeys(obj, attr): res = callattr(obj, f'{attr}_{KEYS}')
     else: res = list()
     return list(zip(itertools.repeat(attr), res)) if zipattr else list(res)
 
-# %% ../nbs/01_keys.ipynb 28
+# %% ../nbs/01_keys.ipynb 29
 def getattrskeys(obj, attrs = None) -> list[tuple[str, str]]:
     '''Retrieve keys from all or specified attributes of an object, combined with attribute names.
 
     Parameters
     ----------
     obj : Any
         The object whose attribute keys are to be retrieved.
@@ -255,15 +262,15 @@
     (('layers', 'squared'), ('obs', 'barcodes'), ('obs', 'con'))
     '''
     with redirect_stderr(io.StringIO()):
         attrs = attrs or getpubattrs(obj)
         return tuple(itertools.chain(*(getattrkeys(obj, a, True) for a in attrs)))
 
 
-# %% ../nbs/01_keys.ipynb 30
+# %% ../nbs/01_keys.ipynb 31
 def getkey(
     obj, key: str, locs: list = None, useobj: bool = True, dtype: type = None,
     hush: bool = True, eager: bool = False, default = None, fallback: Callable | bool = True
 ):
     '''Retrieve the value of a specified key from an object or its attributes.
 
     Parameters
```

### Comparing `akey-0.0.3/akey/mock.py` & `akey-0.0.4/akey/mock.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,53 +9,57 @@
 from contextlib import redirect_stderr
 
 # %% ../nbs/00_mock.ipynb 8
 from typing import Any, NamedTuple, Optional
 
 # %% ../nbs/00_mock.ipynb 11
 try: import pandas as pd, numpy as np, scipy
-except ImportError: warnings.warn("Some packages are not installed")
+except ImportError: ...
 
 # %% ../nbs/00_mock.ipynb 12
 try: from sklearn.datasets import make_blobs
-except ImportError: warnings.warn("Some packages are not installed")
+except ImportError: ...
 
 # %% ../nbs/00_mock.ipynb 14
 try: import anndata as ad, scanpy as sc, scprep
-except ImportError: warnings.warn("Some packages are not installed")
+except ImportError: ...
 
 # %% ../nbs/00_mock.ipynb 15
 try: import phate, magic, graphtools as gt
-except ImportError: warnings.warn("Some packages are not installed")
+except ImportError: ...
 
 # %% ../nbs/00_mock.ipynb 17
 from nlit import (
     X_PCA, X_MAGIC, LEIDEN, GENE_SYMBOL, 
     X_PCA_HVG, X_PHATE, X_PHATE_HVG
 )
 
-from asto import asarr
+from quac import notnilstr
 from chck import isiprod
-from fpos import arg1st
-from ltyp import notnilstr
+from atup import arg1st
+from asto import asarr
 
 # %% ../nbs/00_mock.ipynb 19
 #| export
 
 
 # %% ../nbs/00_mock.ipynb 21
 def dropnils(*args) -> list:
     return list(filter(notnilstr, args))
 
 def charjoin(sep: str = '', *args) -> str:
     return sep.join(dropnils(*tuple(map(str, args))))
 
 def genlabels(
-        n: int, base: str = 'label', prefix: str = '', 
-        suffix: str = '', sep = '_', oneidx: bool = False
+        n: int, 
+        base: str = 'label', 
+        prefix: str = '', 
+        suffix: str = '', 
+        sep = '_', 
+        oneidx: bool = False
 ) -> list[str]:
     label = lambda i: charjoin(sep, prefix, base, suffix, str(i))
     return list(map(label, range(bool(oneidx), n + bool(oneidx))))
 
 def nproducts(*args, retprod: bool = False) -> int | tuple[int, list]:
     prod = list(arg1st(*args, flag=isiprod, uselast=False, default=itertools.product(*args)))
     return len(prod) if not retprod else len(prod), prod
```

### Comparing `akey-0.0.3/akey.egg-info/PKG-INFO` & `akey-0.0.4/akey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akey
-Version: 0.0.3
+Version: 0.0.4
 Summary: akey
 Home-page: https://github.com/dsm-72/akey
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: akey extra extras single cell sc scanpy anndata RNA-seq seq
 Classifier: Development Status :: 4 - Beta
```

### Comparing `akey-0.0.3/settings.ini` & `akey-0.0.4/settings.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = akey
 lib_name = akey
-version = 0.0.3
+version = 0.0.4
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = akey
 nbs_path = nbs
 recursive = True
@@ -29,10 +29,10 @@
 conda_user = dsm-72
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
-requirements = atyp psrc nchr nlit chck hasr asto calr
+requirements = atyp psrc nchr nlit chck hasr asto calr fpos ltyp
 dev_requirements = pandas numpy>=1.22 scipy anndata scanpy scrublet scprep phate magic-impute graphtools matplotlib seaborn excs torch scikit-learn
```

### Comparing `akey-0.0.3/setup.py` & `akey-0.0.4/setup.py`

 * *Files identical despite different names*

