# Comparing `tmp/pyshared-1.5.0-py3-none-any.whl.zip` & `tmp/pyshared-1.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11020 bytes, number of entries: 15
--rw-r--r--  2.0 unx      390 b- defN 24-Mar-31 21:28 pyshared/__init__.py
+Zip file size: 11304 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      755 b- defN 24-Apr-04 12:51 pyshared/__init__.py
 -rw-r--r--  2.0 unx      124 b- defN 24-Jan-11 01:53 pyshared/consts.py
 -rw-r--r--  2.0 unx     1293 b- defN 24-Jan-12 03:28 pyshared/crypto.py
--rw-r--r--  2.0 unx     1938 b- defN 24-Apr-02 21:41 pyshared/env.py
+-rw-r--r--  2.0 unx     2029 b- defN 24-Apr-03 16:31 pyshared/env.py
 -rw-r--r--  2.0 unx      943 b- defN 24-Mar-31 21:02 pyshared/exceptions.py
 -rw-r--r--  2.0 unx      914 b- defN 24-Mar-31 21:30 pyshared/pytest.py
--rw-r--r--  2.0 unx     4740 b- defN 24-Mar-31 21:11 pyshared/python.py
+-rw-r--r--  2.0 unx     4929 b- defN 24-Apr-03 16:29 pyshared/python.py
 -rw-r--r--  2.0 unx      790 b- defN 24-Jan-11 05:57 pyshared/shell.py
 -rw-r--r--  2.0 unx     2083 b- defN 24-Jan-12 03:45 pyshared/terminal.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-02 21:44 pyshared/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6307 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1138 b- defN 24-Apr-02 21:48 pyshared-1.5.0.dist-info/RECORD
-15 files, 21851 bytes uncompressed, 9160 bytes compressed:  58.1%
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-04 12:52 pyshared/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6666 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1138 b- defN 24-Apr-04 12:54 pyshared-1.5.2.dist-info/RECORD
+15 files, 22855 bytes uncompressed, 9444 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pyshared/terminal.py
 Comment: 
 
 Filename: pyshared/version.py
 Comment: 
 
-Filename: pyshared-1.5.0.dist-info/LICENSE
+Filename: pyshared-1.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyshared-1.5.0.dist-info/METADATA
+Filename: pyshared-1.5.2.dist-info/METADATA
 Comment: 
 
-Filename: pyshared-1.5.0.dist-info/WHEEL
+Filename: pyshared-1.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyshared-1.5.0.dist-info/top_level.txt
+Filename: pyshared-1.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyshared-1.5.0.dist-info/RECORD
+Filename: pyshared-1.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyshared/__init__.py

```diff
@@ -1,7 +1,30 @@
+# common imports
+import os
+import os.path as op
+import sys
+import random as ran
+import re
+from decimal import Decimal as D
+from typing import (
+    Generator as Gen,
+    List,
+    Tuple,
+    Union as U,
+    Any as A,
+    Callable as Call,
+    Dict,
+    Optional as Opt,
+    Type,
+    TypeVar as TypeV,
+    Sequence as Seq,
+    Iterable as Iter,
+)
+
+# custom imports
 from .version import __version__
 from .consts import ALPHANUMERIC_CHARS, ALPHANUMERIC_EXT_CHARS
 from .crypto import is_jwt
 from .env import typed_evar
 from .exceptions import NotPrintableError
 from .python import default_repr, ranstr, safe_repr, truncstr
 from .shell import runcmd
```

## pyshared/env.py

```diff
@@ -18,14 +18,17 @@
     (CURDAY, None) -> '25'
     (CURDAY, None, int) -> 25
     (CURDAY, None, float) -> 25.0
     (CURDAY, None, bool) -> True
     (CURDAY, None, Decimal) -> Decimal('25')
 
     """
+    if name is None:
+        raise ValueError('Environment variable name cannot be None')
+
     varval = os.environ.get(name)
     if varval is None:
         return default
 
     if vartype is not None:
         return vartype(varval)
```

## pyshared/python.py

```diff
@@ -100,17 +100,21 @@
     attributes = join_attrs_on.join(
         attrs_format.format(attr_name=attr, attr_repr=safe_repr(value))
         for attr, value in attributes.items()
         if not hasattr(value, '__call__')
         and not str(attr).startswith('_')
         and attr not in exclude_attrs
     )
-    return repr_format.format(
-        obj_name=obj.__class__.__name__, attributes=attributes
-    )
+    obj_name = ''
+    if hasattr(obj, '__class__'):
+        if hasattr(obj.__class__, '__name__'):
+            obj_name = obj.__class__.__name__
+    if hasattr(obj, '__name__'):
+        obj_name += ' ' + obj.__name__
+    return repr_format.format(obj_name=obj_name, attributes=attributes)
 
 
 def truncstr(
     text: str,
     start_chars: int = 3,
     ellipsis: str = '...',
     end_chars: Opt[int] = None,
```

## pyshared/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.5.0'
+__version__ = '1.5.2'
```

## Comparing `pyshared-1.5.0.dist-info/LICENSE` & `pyshared-1.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyshared-1.5.0.dist-info/METADATA` & `pyshared-1.5.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.5.0
+Version: 1.5.2
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -89,39 +89,39 @@
 ### `env.py`
 
 - `typed_evar`: Retrieves and type-casts environment variables.
 
 Examples: (input, default, type, expected_output)
 
 ```
-(None, 1, None, 1),
-(None, 1.0, None, 1.0),
-(None, '1', None, '1'),
-(None, None, int, None),
-(None, None, float, None),
-(None, '20.1', int, '20.1'),
-('0', None, None, 0),
-('0', True, None, False),
-('0', False, None, False),
-('0', 0, None, 0),
-('0', None, bool, True),
-('0', None, int, 0),
-('0', 1.0, float, 0.0),
-('0', None, float, 0.0),
-('0.0', None, None, 0.0),
-('0.', None, None, '0.'),
-('.0', None, None, 0.0),
-('True', None, None, True),
-('tRuE', None, None, True),
-('false', None, None, False),
-('fAlSe', None, None, False),
-('true', None, str, 'true'),
-('test', True, None, ValueError),
-('test', None, int, ValueError),
-('test', 1, None, ValueError),
+'evname, ev, default, vartype, expected',
+    # with default arg
+    ('evname', '0', 0, None, 0),
+    # this shouldnt ever happen but if it does, it should raise error
+    (None, None, '20.1', int, ValueError),
+    (None, None, None, float, ValueError),
+    # assumed typing
+    ('evname', '0.0', None, None, 0.0),
+    ('evname', '0.', None, None, '0.'),
+    ('evname', '.0', None, None, 0.0),
+    ('evname', 'True', None, None, True),
+    ('evname', 'tRuE', None, None, True),
+    ('evname', 'false', None, None, False),
+    ('evname', 'fAlSe', None, None, False),
+    ('evname', '0', None, None, 0),
+    ('evname', '0', True, None, False),
+    ('evname', '0', False, None, False),
+    ('evname', '0', None, bool, True),
+    ('evname', '0', None, int, 0),
+    ('evname', '0', 1.0, float, 0.0),
+    ('evname', '0', None, float, 0.0),
+    ('evname', 'true', None, str, 'true'),
+    ('evname', 'test', True, None, ValueError),
+    ('evname', 'test', None, int, ValueError),
+    ('evname', 'test', 1, None, ValueError),
 ```
 
 ### `exceptions.py`
 
 - `NotPrintableError`: Both str and repr methods raised exceptions.
 
 ### `python.py`
```

