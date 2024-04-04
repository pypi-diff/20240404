# Comparing `tmp/macro_kit-0.4.8.tar.gz` & `tmp/macro_kit-0.4.9.tar.gz`

## Comparing `macro_kit-0.4.8.tar` & `macro_kit-0.4.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/__init__.py
--rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/_symbol.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/_validator.py
--rw-r--r--   0        0        0    20306 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/ast.py
--rw-r--r--   0        0        0    34512 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/expression.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/head.py
--rw-r--r--   0        0        0    33105 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/macro.py
--rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/mock.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/py.typed
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/type_map.py
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/utils.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/ipython/__init__.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/ipython/magic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/julia/__init__.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 macro_kit-0.4.8/macrokit/julia/translate.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 macro_kit-0.4.8/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 macro_kit-0.4.8/LICENSE
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 macro_kit-0.4.8/README.md
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 macro_kit-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 macro_kit-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/__init__.py
+-rw-r--r--   0        0        0     4604 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/_symbol.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/_validator.py
+-rw-r--r--   0        0        0    20306 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/ast.py
+-rw-r--r--   0        0        0    34625 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/expression.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/head.py
+-rw-r--r--   0        0        0    33105 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/macro.py
+-rw-r--r--   0        0        0    10628 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/mock.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/py.typed
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/type_map.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/utils.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/ipython/__init__.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/ipython/magic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/julia/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 macro_kit-0.4.9/macrokit/julia/translate.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 macro_kit-0.4.9/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 macro_kit-0.4.9/LICENSE
+-rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 macro_kit-0.4.9/README.md
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 macro_kit-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 macro_kit-0.4.9/PKG-INFO
```

### Comparing `macro_kit-0.4.8/macrokit/__init__.py` & `macro_kit-0.4.9/macrokit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """macro-kit is a package for macro recording and metaprogramming in Python."""
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 __author__ = "Hanjin Liu"
 __email__ = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp"
 
+from functools import wraps
+
 from macrokit._symbol import Symbol
+from macrokit.ast import parse
 from macrokit.expression import (
     Expr,
     Head,
-    symbol,
-    store_sequence,
-    store,
     object_stored_at,
+    store,
+    store_sequence,
+    symbol,
     symbol_stored_at,
 )
-from macrokit.macro import Macro, MacroFlags, BaseMacro
+from macrokit.macro import BaseMacro, Macro, MacroFlags
 from macrokit.mock import Mock
-from macrokit.ast import parse
-from macrokit.type_map import register_type, unregister_type, type_registered
-from functools import wraps
+from macrokit.type_map import register_type, type_registered, unregister_type
 
 __all__ = [
     "Symbol",
     "Head",
     "Expr",
     "Macro",
     "BaseMacro",
```

### Comparing `macro_kit-0.4.8/macrokit/_symbol.py` & `macro_kit-0.4.9/macrokit/_symbol.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/_validator.py` & `macro_kit-0.4.9/macrokit/_validator.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/ast.py` & `macro_kit-0.4.9/macrokit/ast.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/expression.py` & `macro_kit-0.4.9/macrokit/expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -746,16 +746,20 @@
             continue
         if arg.head is Head.block:
             yield from _iter_lines(arg)
         elif arg.head is Head.if_:  # = cond, if, else
             yield arg.args[0]
             assert isinstance(arg.args[1], Expr)
             yield from _iter_lines(arg.args[1])
-            assert isinstance(arg.args[2], Expr)
-            yield from _iter_lines(arg.args[2])
+            if len(arg.args) > 1:
+                a2 = arg.args[2]
+                if isinstance(a2, Expr):
+                    yield from _iter_lines(a2)
+                else:
+                    yield a2
         elif arg.head in (Head.for_, Head.while_):  # = binop, block
             yield arg.args[0]
             assert isinstance(arg.args[1], Expr)
             yield from _iter_lines(arg.args[1])
         elif arg.head in (Head.function, Head.class_, Head.with_):
             assert isinstance(arg.args[1], Expr)
             yield from _iter_lines(arg.args[1])
```

### Comparing `macro_kit-0.4.8/macrokit/head.py` & `macro_kit-0.4.9/macrokit/head.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/macro.py` & `macro_kit-0.4.9/macrokit/macro.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/mock.py` & `macro_kit-0.4.9/macrokit/mock.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/type_map.py` & `macro_kit-0.4.9/macrokit/type_map.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/utils.py` & `macro_kit-0.4.9/macrokit/utils.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/ipython/magic.py` & `macro_kit-0.4.9/macrokit/ipython/magic.py`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/macrokit/julia/translate.py` & `macro_kit-0.4.9/macrokit/julia/translate.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -41,8 +41,8 @@
     Head.annotate : lambda e, i: f"{as_str(e.args[0], i)}::{as_str(e.args[1])}"
 }
 
 def to_julia_expr(s: str|Expr):
     if isinstance(s, str):
         s = parse(s)
     julia_code = as_str(s)
-    return julia_code
+    return julia_code
```

### Comparing `macro_kit-0.4.8/.gitignore` & `macro_kit-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/LICENSE` & `macro_kit-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/README.md` & `macro_kit-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `macro_kit-0.4.8/PKG-INFO` & `macro_kit-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: macro-kit
-Version: 0.4.8
+Version: 0.4.9
 Summary: Macro recording and metaprogramming in Python
 Project-URL: Download, https://github.com/hanjinliu/macro-kit
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
@@ -36,14 +36,15 @@
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions
 Provides-Extra: testing
 Requires-Dist: numpy>=1.21.0; extra == 'testing'
 Requires-Dist: pandas>=1.3.0; extra == 'testing'
 Requires-Dist: pytest>=6.2.0; extra == 'testing'
 Description-Content-Type: text/markdown
```

