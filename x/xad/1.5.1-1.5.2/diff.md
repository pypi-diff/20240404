# Comparing `tmp/xad-1.5.1-cp39-cp39-win_amd64.whl.zip` & `tmp/xad-1.5.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 359566 bytes, number of entries: 15
--rw-r--r--  2.0 fat     2156 b- defN 80-Jan-01 00:00 xad/__init__.py
--rw-r--r--  2.0 fat     2698 b- defN 80-Jan-01 00:00 xad/adj_1st/__init__.py
--rw-r--r--  2.0 fat     1357 b- defN 80-Jan-01 00:00 xad/exceptions/__init__.py
--rw-r--r--  2.0 fat     2360 b- defN 80-Jan-01 00:00 xad/fwd_1st/__init__.py
--rw-r--r--  2.0 fat     3536 b- defN 80-Jan-01 00:00 xad/math/__init__.py
--rw-r--r--  2.0 fat      212 b- defN 80-Jan-01 00:00 xad/_xad/__init__.pyi
--rw-r--r--  2.0 fat     8939 b- defN 80-Jan-01 00:00 xad/_xad/adj_1st.pyi
+Zip file size: 354292 bytes, number of entries: 15
+-rw-r--r--  2.0 fat     2114 b- defN 80-Jan-01 00:00 xad/__init__.py
+-rw-r--r--  2.0 fat      952 b- defN 80-Jan-01 00:00 xad/__init__.pyi
+-rw-r--r--  2.0 fat      184 b- defN 80-Jan-01 00:00 xad/_xad/__init__.pyi
+-rw-r--r--  2.0 fat     9609 b- defN 80-Jan-01 00:00 xad/_xad/adj_1st.pyi
 -rw-r--r--  2.0 fat      861 b- defN 80-Jan-01 00:00 xad/_xad/exceptions.pyi
--rw-r--r--  2.0 fat     5005 b- defN 80-Jan-01 00:00 xad/_xad/fwd_1st.pyi
--rw-r--r--  2.0 fat    23577 b- defN 80-Jan-01 00:00 xad/_xad/math.pyi
--rw-r--r--  2.0 fat   817664 b- defN 80-Jan-01 00:00 xad/_xad.cp39-win_amd64.pyd
--rw-r--r--  2.0 fat    34949 b- defN 80-Jan-01 00:00 xad-1.5.1.dist-info/LICENSE.md
--rw-r--r--  2.0 fat     5255 b- defN 80-Jan-01 00:00 xad-1.5.1.dist-info/METADATA
--rw-r--r--  2.0 fat       96 b- defN 80-Jan-01 00:00 xad-1.5.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1145 b- defN 16-Jan-01 00:00 xad-1.5.1.dist-info/RECORD
-15 files, 909810 bytes uncompressed, 357716 bytes compressed:  60.7%
+-rw-r--r--  2.0 fat     5675 b- defN 80-Jan-01 00:00 xad/_xad/fwd_1st.pyi
+-rw-r--r--  2.0 fat    27389 b- defN 80-Jan-01 00:00 xad/_xad/math.pyi
+-rw-r--r--  2.0 fat   853504 b- defN 80-Jan-01 00:00 xad/_xad.cp39-win_amd64.pyd
+-rw-r--r--  2.0 fat     2677 b- defN 80-Jan-01 00:00 xad/adj_1st/__init__.py
+-rw-r--r--  2.0 fat     1343 b- defN 80-Jan-01 00:00 xad/exceptions/__init__.py
+-rw-r--r--  2.0 fat     2344 b- defN 80-Jan-01 00:00 xad/fwd_1st/__init__.py
+-rw-r--r--  2.0 fat     3450 b- defN 80-Jan-01 00:00 xad/math/__init__.py
+-rw-r--r--  2.0 fat     5255 b- defN 80-Jan-01 00:00 xad-1.5.2.dist-info/METADATA
+-rw-r--r--  2.0 fat       96 b- defN 80-Jan-01 00:00 xad-1.5.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1129 b- defN 16-Jan-01 00:00 xad-1.5.2.dist-info/RECORD
+15 files, 916582 bytes uncompressed, 352470 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,20 +1,11 @@
 Filename: xad/__init__.py
 Comment: 
 
-Filename: xad/adj_1st/__init__.py
-Comment: 
-
-Filename: xad/exceptions/__init__.py
-Comment: 
-
-Filename: xad/fwd_1st/__init__.py
-Comment: 
-
-Filename: xad/math/__init__.py
+Filename: xad/__init__.pyi
 Comment: 
 
 Filename: xad/_xad/__init__.pyi
 Comment: 
 
 Filename: xad/_xad/adj_1st.pyi
 Comment: 
@@ -27,20 +18,29 @@
 
 Filename: xad/_xad/math.pyi
 Comment: 
 
 Filename: xad/_xad.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xad-1.5.1.dist-info/LICENSE.md
+Filename: xad/adj_1st/__init__.py
+Comment: 
+
+Filename: xad/exceptions/__init__.py
+Comment: 
+
+Filename: xad/fwd_1st/__init__.py
+Comment: 
+
+Filename: xad/math/__init__.py
 Comment: 
 
-Filename: xad-1.5.1.dist-info/METADATA
+Filename: xad-1.5.2.dist-info/METADATA
 Comment: 
 
-Filename: xad-1.5.1.dist-info/WHEEL
+Filename: xad-1.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: xad-1.5.1.dist-info/RECORD
+Filename: xad-1.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xad/__init__.py

```diff
@@ -1,12 +1,12 @@
 ##############################################################################
 #
 #  XAD Python bindings
 #
-#  This file is part of XAD's Python bindings, a comprehensive library for
+#  This file is part of XAD, a comprehensive C++ library for
 #  automatic differentiation.
 #
 #  Copyright (C) 2010-2024 Xcelerit Computing Ltd.
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Affero General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
@@ -21,17 +21,17 @@
 #  along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 ##############################################################################
 
 """Python bindings for the XAD comprehensive library for automatic differentiation"""
 
 from typing import Any, Union
-from ._xad import adj_1st, fwd_1st, __version__
+from ._xad import adj_1st, fwd_1st
 
-__all__ = ["value", "derivative", "__version__"]
+__all__ = ["value", "derivative"]
 
 
 def value(x: Union[adj_1st.Real, fwd_1st.Real, Any]) -> float:
     """Get the value of an XAD active type - or return the value itself otherwise
 
     Args:
         x (Real | any): Argument to get the value of
```

## xad/adj_1st/__init__.py

```diff
@@ -1,12 +1,12 @@
 ##############################################################################
 #
 #  First order adjoint mode module for the XAD Python bindings
 #
-#  This file is part of XAD's Python bindings, a comprehensive library for
+#  This file is part of XAD, a comprehensive C++ library for
 #  automatic differentiation.
 #
 #  Copyright (C) 2010-2024 Xcelerit Computing Ltd.
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Affero General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
@@ -94,12 +94,12 @@
 def _is_integer(x: Real) -> bool:
     return x.value.is_integer()
 
 
 Real.is_integer = _is_integer
 
 
-def _format(x: object, spec: str) -> str:
+def _format(x: Real, spec) -> str:
     return format(x.value, spec)
 
 
 Real.__format__ = _format
```

## xad/exceptions/__init__.py

```diff
@@ -1,12 +1,12 @@
 ##############################################################################
 #
 #  Exceptions module for the XAD Python bindings
 #
-#  This file is part of XAD's Python bindings, a comprehensive library for
+#  This file is part of XAD, a comprehensive C++ library for
 #  automatic differentiation.
 #
 #  Copyright (C) 2010-2024 Xcelerit Computing Ltd.
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Affero General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
```

## xad/fwd_1st/__init__.py

```diff
@@ -1,12 +1,12 @@
 ##############################################################################
 #
 #  First order forward mode module for the XAD Python bindings
 #
-#  This file is part of XAD's Python bindings, a comprehensive library for
+#  This file is part of XAD, a comprehensive C++ library for
 #  automatic differentiation.
 #
 #  Copyright (C) 2010-2024 Xcelerit Computing Ltd.
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Affero General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
@@ -69,8 +69,8 @@
     return x.value.is_integer()
 
 Real.is_integer = _is_integer
 
 def _format(x: Real, spec) -> str:
     return format(x.value, spec)
 
-Real.__format__ = _format
+Real.__format__ = _format
```

## xad/math/__init__.py

```diff
@@ -1,12 +1,12 @@
 ##############################################################################
 #
 #  Math module for the XAD Python bindings
 #
-#  This file is part of XAD's Python bindings, a comprehensive library for
+#  This file is part of XAD, a comprehensive C++ library for
 #  automatic differentiation.
 #
 #  Copyright (C) 2010-2024 Xcelerit Computing Ltd.
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU Affero General Public License as published
 #  by the Free Software Foundation, either version 3 of the License, or
@@ -135,26 +135,23 @@
     "nan",
     "isclose",
     "isfinite",
     "isinf",
     "isnan",
 ]
 
-import xad
+import xad as xad
 import math as _math
 
 
-def hypot(*inputs: Union["xad.adj_1st.Real", "xad.fwd_1st.Real", float, int]):
+def hypot(*inputs: List[Union["xad.adj_1st.Real", "xad.fwd_1st.Real", float, int]]):
     return sqrt(sum(pow(x, 2) for x in inputs))
 
 
-def dist(
-    p: List[Union["xad.adj_1st.Real", "xad.fwd_1st.Real", float, int]],
-    q: List[Union["xad.adj_1st.Real", "xad.fwd_1st.Real", float, int]],
-):
+def dist(p: Union["xad.adj_1st.Real", "xad.fwd_1st.Real", float, int], q):
     return sqrt(sum(pow(px - qx, 2) for px, qx in zip(p, q)))
 
 
 def isclose(a, b, *args, **kwargs):
     return _math.isclose(xad.value(a), xad.value(b), *args, **kwargs)
```

## xad/_xad/__init__.pyi

```diff
@@ -1,7 +1,6 @@
 from __future__ import annotations
 from . import adj_1st
 from . import exceptions
 from . import fwd_1st
 from . import math
 __all__ = ['adj_1st', 'exceptions', 'fwd_1st', 'math']
-__version__: str = '1.5.1'
```

## xad/_xad/adj_1st.pyi

```diff
@@ -21,28 +21,34 @@
     @typing.overload
     def __divmod__(self, arg0: Real) -> tuple[Real, Real]:
         ...
     @typing.overload
     def __divmod__(self, arg0: float) -> tuple[Real, Real]:
         ...
     @typing.overload
+    def __divmod__(self, arg0: int) -> tuple[Real, Real]:
+        ...
+    @typing.overload
     def __eq__(self, arg0: Real) -> bool:
         ...
     @typing.overload
     def __eq__(self, arg0: float) -> bool:
         ...
     def __floor__(self) -> int:
         ...
     @typing.overload
     def __floordiv__(self, arg0: Real) -> Real:
         ...
     @typing.overload
     def __floordiv__(self, arg0: float) -> Real:
         ...
     @typing.overload
+    def __floordiv__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __ge__(self, arg0: Real) -> bool:
         ...
     @typing.overload
     def __ge__(self, arg0: float) -> bool:
         ...
     @typing.overload
     def __gt__(self, arg0: Real) -> bool:
@@ -70,14 +76,17 @@
     @typing.overload
     def __lt__(self, arg0: float) -> bool:
         ...
     @typing.overload
     def __mod__(self, arg0: Real) -> Real:
         ...
     @typing.overload
+    def __mod__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __mod__(self, arg0: float) -> Real:
         ...
     @typing.overload
     def __mul__(self, arg0: float) -> Real:
         ...
     @typing.overload
     def __mul__(self, arg0: Real) -> Real:
@@ -92,46 +101,58 @@
         ...
     def __pos__(self) -> Real:
         ...
     @typing.overload
     def __pow__(self, arg0: Real) -> Real:
         ...
     @typing.overload
+    def __pow__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __pow__(self, arg0: float) -> Real:
         ...
     def __radd__(self, arg0: float) -> Real:
         ...
     @typing.overload
     def __rdivmod__(self, arg0: Real) -> tuple[Real, Real]:
         ...
     @typing.overload
     def __rdivmod__(self, arg0: float) -> tuple[Real, Real]:
         ...
+    @typing.overload
+    def __rdivmod__(self, arg0: int) -> tuple[Real, Real]:
+        ...
     def __repr__(self) -> str:
         ...
     def __req__(self, arg0: float) -> bool:
         ...
     @typing.overload
     def __rfloordiv__(self, arg0: Real) -> Real:
         ...
     @typing.overload
     def __rfloordiv__(self, arg0: float) -> Real:
         ...
+    @typing.overload
+    def __rfloordiv__(self, arg0: int) -> Real:
+        ...
     def __rge__(self, arg0: float) -> bool:
         ...
     def __rgt__(self, arg0: float) -> bool:
         ...
     def __rle__(self, arg0: float) -> bool:
         ...
     def __rlt__(self, arg0: float) -> bool:
         ...
     @typing.overload
     def __rmod__(self, arg0: Real) -> Real:
         ...
     @typing.overload
+    def __rmod__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __rmod__(self, arg0: float) -> Real:
         ...
     def __rmul__(self, arg0: float) -> Real:
         ...
     def __rne__(self, arg0: float) -> bool:
         ...
     @typing.overload
@@ -140,14 +161,17 @@
     @typing.overload
     def __round__(self) -> int:
         ...
     @typing.overload
     def __rpow__(self, arg0: Real) -> Real:
         ...
     @typing.overload
+    def __rpow__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __rpow__(self, arg0: float) -> Real:
         ...
     def __rsub__(self, arg0: float) -> Real:
         ...
     def __rtruediv__(self, arg0: float) -> Real:
         ...
     @typing.overload
```

## xad/_xad/fwd_1st.pyi

```diff
@@ -21,28 +21,34 @@
     @typing.overload
     def __divmod__(self, arg0: Real) -> tuple[Real, Real]:
         ...
     @typing.overload
     def __divmod__(self, arg0: float) -> tuple[Real, Real]:
         ...
     @typing.overload
+    def __divmod__(self, arg0: int) -> tuple[Real, Real]:
+        ...
+    @typing.overload
     def __eq__(self, arg0: Real) -> bool:
         ...
     @typing.overload
     def __eq__(self, arg0: float) -> bool:
         ...
     def __floor__(self) -> int:
         ...
     @typing.overload
     def __floordiv__(self, arg0: Real) -> Real:
         ...
     @typing.overload
     def __floordiv__(self, arg0: float) -> Real:
         ...
     @typing.overload
+    def __floordiv__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __ge__(self, arg0: Real) -> bool:
         ...
     @typing.overload
     def __ge__(self, arg0: float) -> bool:
         ...
     @typing.overload
     def __gt__(self, arg0: Real) -> bool:
@@ -70,14 +76,17 @@
     @typing.overload
     def __lt__(self, arg0: float) -> bool:
         ...
     @typing.overload
     def __mod__(self, arg0: Real) -> Real:
         ...
     @typing.overload
+    def __mod__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __mod__(self, arg0: float) -> Real:
         ...
     @typing.overload
     def __mul__(self, arg0: float) -> Real:
         ...
     @typing.overload
     def __mul__(self, arg0: Real) -> Real:
@@ -92,46 +101,58 @@
         ...
     def __pos__(self) -> Real:
         ...
     @typing.overload
     def __pow__(self, arg0: Real) -> Real:
         ...
     @typing.overload
+    def __pow__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __pow__(self, arg0: float) -> Real:
         ...
     def __radd__(self, arg0: float) -> Real:
         ...
     @typing.overload
     def __rdivmod__(self, arg0: Real) -> tuple[Real, Real]:
         ...
     @typing.overload
     def __rdivmod__(self, arg0: float) -> tuple[Real, Real]:
         ...
+    @typing.overload
+    def __rdivmod__(self, arg0: int) -> tuple[Real, Real]:
+        ...
     def __repr__(self) -> str:
         ...
     def __req__(self, arg0: float) -> bool:
         ...
     @typing.overload
     def __rfloordiv__(self, arg0: Real) -> Real:
         ...
     @typing.overload
     def __rfloordiv__(self, arg0: float) -> Real:
         ...
+    @typing.overload
+    def __rfloordiv__(self, arg0: int) -> Real:
+        ...
     def __rge__(self, arg0: float) -> bool:
         ...
     def __rgt__(self, arg0: float) -> bool:
         ...
     def __rle__(self, arg0: float) -> bool:
         ...
     def __rlt__(self, arg0: float) -> bool:
         ...
     @typing.overload
     def __rmod__(self, arg0: Real) -> Real:
         ...
     @typing.overload
+    def __rmod__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __rmod__(self, arg0: float) -> Real:
         ...
     def __rmul__(self, arg0: float) -> Real:
         ...
     def __rne__(self, arg0: float) -> bool:
         ...
     @typing.overload
@@ -140,14 +161,17 @@
     @typing.overload
     def __round__(self) -> int:
         ...
     @typing.overload
     def __rpow__(self, arg0: Real) -> Real:
         ...
     @typing.overload
+    def __rpow__(self, arg0: int) -> Real:
+        ...
+    @typing.overload
     def __rpow__(self, arg0: float) -> Real:
         ...
     def __rsub__(self, arg0: float) -> Real:
         ...
     def __rtruediv__(self, arg0: float) -> Real:
         ...
     @typing.overload
```

## xad/_xad/math.pyi

```diff
@@ -1,914 +1,1024 @@
 from __future__ import annotations
-import _xad.adj_1st
-import _xad.fwd_1st
 import typing
+import xad._xad.adj_1st
+import xad._xad.fwd_1st
 __all__ = ['abs', 'acos', 'acosh', 'asin', 'asinh', 'atan', 'atan2', 'atanh', 'cbrt', 'ceil', 'copysign', 'cos', 'cosh', 'degrees', 'erf', 'erfc', 'exp', 'exp2', 'expm1', 'fabs', 'floor', 'fmax', 'fmin', 'fmod', 'frexp', 'ldexp', 'log', 'log10', 'log1p', 'log2', 'max', 'min', 'modf', 'nextafter', 'pow', 'radians', 'remainder', 'sin', 'sinh', 'smooth_abs', 'smooth_max', 'smooth_min', 'sqrt', 'tan', 'tanh', 'trunc']
 @typing.overload
-def abs(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def abs(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     absolute value
     """
 @typing.overload
-def abs(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def abs(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     absolute value
     """
 @typing.overload
 def abs(arg0: float) -> float:
     """
     absolute value
     """
 @typing.overload
-def acos(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def acos(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     inverse cosine
     """
 @typing.overload
-def acos(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def acos(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     inverse cosine
     """
 @typing.overload
 def acos(arg0: float) -> float:
     """
     inverse cosine
     """
 @typing.overload
-def acosh(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def acosh(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     inverse cosine hyperbolicus
     """
 @typing.overload
-def acosh(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def acosh(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     inverse cosine hyperbolicus
     """
 @typing.overload
 def acosh(arg0: float) -> float:
     """
     inverse cosine hyperbolicus
     """
 @typing.overload
-def asin(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def asin(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     inverse sine
     """
 @typing.overload
-def asin(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def asin(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     inverse sine
     """
 @typing.overload
 def asin(arg0: float) -> float:
     """
     inverse sine
     """
 @typing.overload
-def asinh(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def asinh(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     inverse sine hyperbolicus
     """
 @typing.overload
-def asinh(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def asinh(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     inverse sine hyperbolicus
     """
 @typing.overload
 def asinh(arg0: float) -> float:
     """
     inverse sine hyperbolicus
     """
 @typing.overload
-def atan(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def atan(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     inverse tangent
     """
 @typing.overload
-def atan(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def atan(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     inverse tangent
     """
 @typing.overload
 def atan(arg0: float) -> float:
     """
     inverse tangent
     """
 @typing.overload
-def atan2(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def atan2(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     4-quadrant inverse tangent
     """
 @typing.overload
-def atan2(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def atan2(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
     """
     4 quadrant inverse tangent
     """
 @typing.overload
-def atan2(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def atan2(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     4 quadrant inverse tangent
     """
 @typing.overload
-def atan2(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def atan2(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     4-quadrant inverse tangent
     """
 @typing.overload
-def atan2(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def atan2(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     4 quadrant inverse tangent
     """
 @typing.overload
-def atan2(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def atan2(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     4 quadrant inverse tangent
     """
 @typing.overload
 def atan2(arg0: float, arg1: float) -> float:
     """
     4-quadrant inverse tangent
     """
 @typing.overload
-def atanh(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def atan2(arg0: float, arg1: float) -> float:
+    """
+    4 quadrant inverse tangent
+    """
+@typing.overload
+def atan2(arg0: float, arg1: float) -> float:
+    """
+    4 quadrant inverse tangent
+    """
+@typing.overload
+def atanh(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     inverse tangent hyperbolicus
     """
 @typing.overload
-def atanh(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def atanh(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     inverse tangent hyperbolicus
     """
 @typing.overload
 def atanh(arg0: float) -> float:
     """
     inverse tangent hyperbolicus
     """
 @typing.overload
-def cbrt(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def cbrt(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     cubic root
     """
 @typing.overload
-def cbrt(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def cbrt(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     cubic root
     """
 @typing.overload
 def cbrt(arg0: float) -> float:
     """
     cubic root
     """
 @typing.overload
-def ceil(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def ceil(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     rounding away from zero
     """
 @typing.overload
-def ceil(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def ceil(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     rounding away from zero
     """
 @typing.overload
 def ceil(arg0: float) -> float:
     """
     rounding away from zero
     """
 @typing.overload
-def copysign(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def copysign(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
+    """
+    copy sign of one value to another
+    """
+@typing.overload
+def copysign(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
     """
     copy sign of one value to another
     """
 @typing.overload
-def copysign(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def copysign(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     copy sign of one value to another
     """
 @typing.overload
-def copysign(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def copysign(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     copy sign of one value to another
     """
 @typing.overload
-def copysign(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def copysign(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     copy sign of one value to another
     """
 @typing.overload
-def copysign(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def copysign(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     copy sign of one value to another
     """
 @typing.overload
-def copysign(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def copysign(arg0: float, arg1: float) -> float:
     """
     copy sign of one value to another
     """
 @typing.overload
 def copysign(arg0: float, arg1: float) -> float:
     """
     copy sign of one value to another
     """
 @typing.overload
-def cos(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def copysign(arg0: float, arg1: float) -> float:
+    """
+    copy sign of one value to another
+    """
+@typing.overload
+def cos(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     cosine
     """
 @typing.overload
-def cos(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def cos(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     cosine
     """
 @typing.overload
 def cos(arg0: float) -> float:
     """
     cosine
     """
 @typing.overload
-def cosh(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def cosh(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     cosine hyperbolicus
     """
 @typing.overload
-def cosh(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def cosh(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     cosine hyperbolicus
     """
 @typing.overload
 def cosh(arg0: float) -> float:
     """
     cosine hyperbolicus
     """
 @typing.overload
-def degrees(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def degrees(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     convert radians to degrees
     """
 @typing.overload
-def degrees(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def degrees(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     convert radians to degrees
     """
 @typing.overload
 def degrees(arg0: float) -> float:
     """
     convert radians to degrees
     """
 @typing.overload
-def erf(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def erf(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     error function
     """
 @typing.overload
-def erf(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def erf(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     error function
     """
 @typing.overload
 def erf(arg0: float) -> float:
     """
     error function
     """
 @typing.overload
-def erfc(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def erfc(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     complementary error function
     """
 @typing.overload
-def erfc(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def erfc(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     complementary error function
     """
 @typing.overload
 def erfc(arg0: float) -> float:
     """
     complementary error function
     """
 @typing.overload
-def exp(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def exp(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     exponential function
     """
 @typing.overload
-def exp(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def exp(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     exponential function
     """
 @typing.overload
 def exp(arg0: float) -> float:
     """
     exponential function
     """
 @typing.overload
-def exp2(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def exp2(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     computes 2 to the power of the argument
     """
 @typing.overload
-def exp2(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def exp2(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     computes 2 to the power of the argument
     """
 @typing.overload
 def exp2(arg0: float) -> float:
     """
     computes 2 to the power of the argument
     """
 @typing.overload
-def expm1(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def expm1(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     computes exp(x)-1
     """
 @typing.overload
-def expm1(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def expm1(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     computes exp(x)-1
     """
 @typing.overload
 def expm1(arg0: float) -> float:
     """
     computes exp(x)-1
     """
 @typing.overload
-def fabs(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def fabs(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     absolute value
     """
 @typing.overload
-def fabs(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def fabs(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     absolute value
     """
 @typing.overload
 def fabs(arg0: float) -> float:
     """
     absolute value
     """
 @typing.overload
-def floor(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def floor(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     rounding towards zero
     """
 @typing.overload
-def floor(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def floor(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     rounding towards zero
     """
 @typing.overload
 def floor(arg0: float) -> float:
     """
     rounding towards zero
     """
 @typing.overload
-def fmax(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def fmax(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
+    """
+    maximum of 2 values
+    """
+@typing.overload
+def fmax(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def fmax(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def fmax(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def fmax(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def fmax(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def fmax(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def fmax(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def fmax(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def fmax(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def fmax(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def fmax(arg0: float, arg1: float) -> float:
     """
     maximum of 2 values
     """
 @typing.overload
 def fmax(arg0: float, arg1: float) -> float:
     """
     maximum of 2 values
     """
 @typing.overload
-def fmin(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def fmax(arg0: float, arg1: float) -> float:
+    """
+    maximum of 2 values
+    """
+@typing.overload
+def fmin(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
+    """
+    minimum of 2 values
+    """
+@typing.overload
+def fmin(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
+    """
+    minimum of 2 values
+    """
+@typing.overload
+def fmin(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     minimum of 2 values
     """
 @typing.overload
-def fmin(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def fmin(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     minimum of 2 values
     """
 @typing.overload
-def fmin(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def fmin(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     minimum of 2 values
     """
 @typing.overload
-def fmin(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def fmin(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     minimum of 2 values
     """
 @typing.overload
-def fmin(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def fmin(arg0: float, arg1: float) -> float:
     """
     minimum of 2 values
     """
 @typing.overload
-def fmin(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def fmin(arg0: float, arg1: float) -> float:
     """
     minimum of 2 values
     """
 @typing.overload
 def fmin(arg0: float, arg1: float) -> float:
     """
     minimum of 2 values
     """
 @typing.overload
-def fmod(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def fmod(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     floating point remainer after integer division
     """
 @typing.overload
-def fmod(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def fmod(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     floating point remainer after integer division
     """
 @typing.overload
 def fmod(arg0: float, arg1: float) -> float:
     """
     floating point remainer after integer division
     """
 @typing.overload
-def frexp(arg0: _xad.adj_1st.Real) -> tuple:
+def frexp(arg0: xad._xad.adj_1st.Real) -> tuple:
     """
     decomposes into normalised fraction and an integral power of 2
     """
 @typing.overload
-def frexp(arg0: _xad.fwd_1st.Real) -> tuple:
+def frexp(arg0: xad._xad.fwd_1st.Real) -> tuple:
     """
     decomposes into normalised fraction and an integral power of 2
     """
 @typing.overload
 def frexp(arg0: float) -> tuple:
     """
     decomposes into normalised fraction and an integral power of 2
     """
 @typing.overload
-def ldexp(arg0: _xad.adj_1st.Real, arg1: int) -> _xad.adj_1st.Real:
+def ldexp(arg0: xad._xad.adj_1st.Real, arg1: int) -> xad._xad.adj_1st.Real:
     """
     mutiplies x by 2 to the power of exp
     """
 @typing.overload
-def ldexp(arg0: _xad.fwd_1st.Real, arg1: int) -> _xad.fwd_1st.Real:
+def ldexp(arg0: xad._xad.fwd_1st.Real, arg1: int) -> xad._xad.fwd_1st.Real:
     """
     mutiplies x by 2 to the power of exp
     """
 @typing.overload
 def ldexp(arg0: float, arg1: int) -> float:
     """
     mutiplies x by 2 to the power of exp
     """
 @typing.overload
-def log(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def log(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     natural logarithm
     """
 @typing.overload
-def log(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def log(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     natural logarithm
     """
 @typing.overload
 def log(arg0: float) -> float:
     """
     natural logarithm
     """
 @typing.overload
-def log10(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def log10(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     base 10 logarithm
     """
 @typing.overload
-def log10(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def log10(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     base 10 logarithm
     """
 @typing.overload
 def log10(arg0: float) -> float:
     """
     base 10 logarithm
     """
 @typing.overload
-def log1p(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def log1p(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     computes log(1 + x)
     """
 @typing.overload
-def log1p(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def log1p(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     computes log(1 + x)
     """
 @typing.overload
 def log1p(arg0: float) -> float:
     """
     computes log(1 + x)
     """
 @typing.overload
-def log2(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def log2(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     base 2 logarithm
     """
 @typing.overload
-def log2(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def log2(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     base 2 logarithm
     """
 @typing.overload
 def log2(arg0: float) -> float:
     """
     base 2 logarithm
     """
 @typing.overload
-def max(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def max(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def max(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def max(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def max(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def max(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def max(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def max(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def max(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def max(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
-def max(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def max(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     maximum of 2 values
     """
 @typing.overload
 def max(arg0: float, arg1: float) -> float:
     """
     maximum of 2 values
     """
 @typing.overload
-def min(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def max(arg0: float, arg1: float) -> float:
+    """
+    maximum of 2 values
+    """
+@typing.overload
+def max(arg0: float, arg1: float) -> float:
+    """
+    maximum of 2 values
+    """
+@typing.overload
+def min(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
+    """
+    minimum of 2 values
+    """
+@typing.overload
+def min(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
+    """
+    minimum of 2 values
+    """
+@typing.overload
+def min(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     minimum of 2 values
     """
 @typing.overload
-def min(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def min(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     minimum of 2 values
     """
 @typing.overload
-def min(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def min(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     minimum of 2 values
     """
 @typing.overload
-def min(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def min(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     minimum of 2 values
     """
 @typing.overload
-def min(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def min(arg0: float, arg1: float) -> float:
     """
     minimum of 2 values
     """
 @typing.overload
-def min(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def min(arg0: float, arg1: float) -> float:
     """
     minimum of 2 values
     """
 @typing.overload
 def min(arg0: float, arg1: float) -> float:
     """
     minimum of 2 values
     """
 @typing.overload
-def modf(arg0: _xad.adj_1st.Real) -> tuple:
+def modf(arg0: xad._xad.adj_1st.Real) -> tuple:
     """
     decomposes into integral and fractional parts
     """
 @typing.overload
-def modf(arg0: _xad.fwd_1st.Real) -> tuple:
+def modf(arg0: xad._xad.fwd_1st.Real) -> tuple:
     """
     decomposes into integral and fractional parts
     """
 @typing.overload
 def modf(arg0: float) -> tuple:
     """
     decomposes into integral and fractional parts
     """
 @typing.overload
-def nextafter(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def nextafter(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
+    """
+    next representable value in the given direction
+    """
+@typing.overload
+def nextafter(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
     """
     next representable value in the given direction
     """
 @typing.overload
-def nextafter(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def nextafter(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     next representable value in the given direction
     """
 @typing.overload
-def nextafter(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def nextafter(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     next representable value in the given direction
     """
 @typing.overload
-def nextafter(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def nextafter(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     next representable value in the given direction
     """
 @typing.overload
-def nextafter(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def nextafter(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
+    """
+    next representable value in the given direction
+    """
+@typing.overload
+def nextafter(arg0: float, arg1: float) -> float:
     """
     next representable value in the given direction
     """
 @typing.overload
-def nextafter(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def nextafter(arg0: float, arg1: float) -> float:
     """
     next representable value in the given direction
     """
 @typing.overload
 def nextafter(arg0: float, arg1: float) -> float:
     """
     next representable value in the given direction
     """
 @typing.overload
-def pow(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def pow(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
+    """
+    power
+    """
+@typing.overload
+def pow(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
+    """
+    power
+    """
+@typing.overload
+def pow(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     power
     """
 @typing.overload
-def pow(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def pow(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     power
     """
 @typing.overload
-def pow(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def pow(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     power
     """
 @typing.overload
-def pow(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def pow(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     power
     """
 @typing.overload
-def pow(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def pow(arg0: float, arg1: float) -> float:
     """
     power
     """
 @typing.overload
-def pow(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def pow(arg0: float, arg1: float) -> float:
     """
     power
     """
 @typing.overload
 def pow(arg0: float, arg1: float) -> float:
     """
     power
     """
 @typing.overload
-def radians(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def radians(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     convert degrees to radians
     """
 @typing.overload
-def radians(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def radians(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     convert degrees to radians
     """
 @typing.overload
 def radians(arg0: float) -> float:
     """
     convert degrees to radians
     """
 @typing.overload
-def remainder(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def remainder(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     signed remainder after integer division
     """
 @typing.overload
-def remainder(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def remainder(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
     """
     signed remainder after integer division
     """
 @typing.overload
-def remainder(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def remainder(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     signed remainder after integer division
     """
 @typing.overload
-def remainder(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def remainder(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     signed remainder after integer division
     """
 @typing.overload
-def remainder(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def remainder(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     signed remainder after integer division
     """
 @typing.overload
-def remainder(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def remainder(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     signed remainder after integer division
     """
 @typing.overload
 def remainder(arg0: float, arg1: float) -> float:
     """
     signed remainder after integer division
     """
 @typing.overload
-def sin(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def remainder(arg0: float, arg1: float) -> float:
+    """
+    signed remainder after integer division
+    """
+@typing.overload
+def remainder(arg0: float, arg1: float) -> float:
+    """
+    signed remainder after integer division
+    """
+@typing.overload
+def sin(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     sine
     """
 @typing.overload
-def sin(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def sin(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     sine
     """
 @typing.overload
 def sin(arg0: float) -> float:
     """
     sine
     """
 @typing.overload
-def sinh(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def sinh(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     sine hyperbolicus
     """
 @typing.overload
-def sinh(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def sinh(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     sine hyperbolicus
     """
 @typing.overload
 def sinh(arg0: float) -> float:
     """
     sine hyperbolicus
     """
 @typing.overload
-def smooth_abs(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def smooth_abs(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     smoothed abs function for well-defined derivatives
     """
 @typing.overload
-def smooth_abs(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def smooth_abs(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     smoothed abs function for well-defined derivatives
     """
 @typing.overload
 def smooth_abs(arg0: float) -> float:
     """
     smoothed abs function for well-defined derivatives
     """
 @typing.overload
-def smooth_max(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def smooth_max(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     smoothed max function for well-defined derivatives
     """
 @typing.overload
-def smooth_max(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def smooth_max(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
     """
     smoothed max function for well-defined derivatives
     """
 @typing.overload
-def smooth_max(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def smooth_max(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     smoothed max function for well-defined derivatives
     """
 @typing.overload
-def smooth_max(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def smooth_max(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     smoothed max function for well-defined derivatives
     """
 @typing.overload
-def smooth_max(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def smooth_max(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     smoothed max function for well-defined derivatives
     """
 @typing.overload
-def smooth_max(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def smooth_max(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     smoothed max function for well-defined derivatives
     """
 @typing.overload
 def smooth_max(arg0: float, arg1: float) -> float:
     """
     smoothed max function for well-defined derivatives
     """
 @typing.overload
-def smooth_min(arg0: _xad.adj_1st.Real, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def smooth_max(arg0: float, arg1: float) -> float:
+    """
+    smoothed max function for well-defined derivatives
+    """
+@typing.overload
+def smooth_max(arg0: float, arg1: float) -> float:
+    """
+    smoothed max function for well-defined derivatives
+    """
+@typing.overload
+def smooth_min(arg0: xad._xad.adj_1st.Real, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
+    """
+    smoothed min function for well-defined derivatives
+    """
+@typing.overload
+def smooth_min(arg0: xad._xad.adj_1st.Real, arg1: float) -> xad._xad.adj_1st.Real:
     """
     smoothed min function for well-defined derivatives
     """
 @typing.overload
-def smooth_min(arg0: _xad.adj_1st.Real, arg1: float) -> _xad.adj_1st.Real:
+def smooth_min(arg0: float, arg1: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     smoothed min function for well-defined derivatives
     """
 @typing.overload
-def smooth_min(arg0: float, arg1: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def smooth_min(arg0: xad._xad.fwd_1st.Real, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     smoothed min function for well-defined derivatives
     """
 @typing.overload
-def smooth_min(arg0: _xad.fwd_1st.Real, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def smooth_min(arg0: xad._xad.fwd_1st.Real, arg1: float) -> xad._xad.fwd_1st.Real:
     """
     smoothed min function for well-defined derivatives
     """
 @typing.overload
-def smooth_min(arg0: _xad.fwd_1st.Real, arg1: float) -> _xad.fwd_1st.Real:
+def smooth_min(arg0: float, arg1: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     smoothed min function for well-defined derivatives
     """
 @typing.overload
-def smooth_min(arg0: float, arg1: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def smooth_min(arg0: float, arg1: float) -> float:
+    """
+    smoothed min function for well-defined derivatives
+    """
+@typing.overload
+def smooth_min(arg0: float, arg1: float) -> float:
     """
     smoothed min function for well-defined derivatives
     """
 @typing.overload
 def smooth_min(arg0: float, arg1: float) -> float:
     """
     smoothed min function for well-defined derivatives
     """
 @typing.overload
-def sqrt(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def sqrt(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     square root
     """
 @typing.overload
-def sqrt(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def sqrt(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     square root
     """
 @typing.overload
 def sqrt(arg0: float) -> float:
     """
     square root
     """
 @typing.overload
-def tan(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def tan(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     tangent
     """
 @typing.overload
-def tan(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def tan(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     tangent
     """
 @typing.overload
 def tan(arg0: float) -> float:
     """
     tangent
     """
 @typing.overload
-def tanh(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def tanh(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     tangent hyperbolicus
     """
 @typing.overload
-def tanh(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def tanh(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     tangent hyperbolicus
     """
 @typing.overload
 def tanh(arg0: float) -> float:
     """
     tangent hyperbolicus
     """
 @typing.overload
-def trunc(arg0: _xad.adj_1st.Real) -> _xad.adj_1st.Real:
+def trunc(arg0: xad._xad.adj_1st.Real) -> xad._xad.adj_1st.Real:
     """
     cut off decimals
     """
 @typing.overload
-def trunc(arg0: _xad.fwd_1st.Real) -> _xad.fwd_1st.Real:
+def trunc(arg0: xad._xad.fwd_1st.Real) -> xad._xad.fwd_1st.Real:
     """
     cut off decimals
     """
 @typing.overload
 def trunc(arg0: float) -> float:
     """
     cut off decimals
```

## Comparing `xad-1.5.1.dist-info/METADATA` & `xad-1.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xad
-Version: 1.5.1
+Version: 1.5.2
 Summary: High-Performance Automatic Differentiation for Python
 Home-page: https://auto-differentiation.github.io
 License: AGPL-3.0-or-later
 Keywords: automatic-differentiation,derivatives,machine-learning,optimisation,numerical-analysis,scientific-computing,risk-management,computer-graphics,robotics,biotechnology,meteorology,quant-finance
 Author: Auto Differentiation Dev Team
 Author-email: dev@auto-differentiation.com
 Requires-Python: >=3.8.1,<4.0
```

## Comparing `xad-1.5.1.dist-info/RECORD` & `xad-1.5.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-xad/__init__.py,sha256=sj8jeMibhrerkZrCY9SLB8w4Kr5w06VM-OhlEoh8kQk,2156
-xad/adj_1st/__init__.py,sha256=V-yzNQZ79Wdk4assGtQVCpoUfjmHr3HqUAdaT2o50Dk,2698
-xad/exceptions/__init__.py,sha256=0hN27f1s7L5c8x6FBsHy_h4VWLB6QAfNuR3Jldew7vw,1357
-xad/fwd_1st/__init__.py,sha256=V_8bW4wHYaqf3joio4ePt09Tm9GcwCWgYqJgcVCToRI,2360
-xad/math/__init__.py,sha256=G989-PB9kvUw3BaZvmYmCG-pJpv4ahXyQuXBDmPPpEU,3536
-xad/_xad/__init__.pyi,sha256=YRx83TPn3qQpA4vLxaeb32SxD90c9QLInQmlEsHGzd0,212
-xad/_xad/adj_1st.pyi,sha256=OMgZP1Eekd8uiMqw03jCLQmHMxtVeUVFJz5g-9aCgwk,8939
+xad/__init__.py,sha256=3i6Ov8sAPptSn7VL-Vy7rXEiNRWNdQV3aBh0UifSPtU,2114
+xad/__init__.pyi,sha256=GAj0P-NFtIm6o8A5es81YOXO4JGF0J8pX-eGWK3Nn-w,952
+xad/_xad/__init__.pyi,sha256=kYbHjfcu7ciQL5yjW-DPCj1wCzmsJxfcKNAv3enLJF0,184
+xad/_xad/adj_1st.pyi,sha256=usDDjwRIqRtb0F1uItLNrvlrr06N40kI1xQIHZjOqIw,9609
 xad/_xad/exceptions.pyi,sha256=ygitHAEq8AxQRdthxy5e_N9Acx3rSAoepa2xtODsj7Y,861
-xad/_xad/fwd_1st.pyi,sha256=jiKUAleJwNjfexywCvUmCnVq0KVBvBt_W1eaC6EVCYM,5005
-xad/_xad/math.pyi,sha256=nBwDD7vJ5AWJaeCfTr2QDw0IZ6M_QK9Hxgxlz-kI5Ws,23577
-xad/_xad.cp39-win_amd64.pyd,sha256=F0pfJZ_6jW0At2WaH_wdIO8lS9-lHlHSoGUzNZ1HQR8,817664
-xad-1.5.1.dist-info/LICENSE.md,sha256=EdxnuSBUdKUhR6j2BOysfsflJZtGxbWopO7u9xnrE0s,34949
-xad-1.5.1.dist-info/METADATA,sha256=IKdNsoICdpn8XM6D2ZH1XqTRbnsr5XupH-KkOcZ2Hqg,5255
-xad-1.5.1.dist-info/WHEEL,sha256=1IyMrlk0wO7UertYm7pyjf3m1sV0KDb8wW6mQlBtUog,96
-xad-1.5.1.dist-info/RECORD,,
+xad/_xad/fwd_1st.pyi,sha256=_X5xeF-1XSmhRIyazF87vOpgZjY1V7GMSi6_we1IU3k,5675
+xad/_xad/math.pyi,sha256=055kXne6ujXH17-R33CK13W3DJYTMPeO8x-OBGjTNfA,27389
+xad/_xad.cp39-win_amd64.pyd,sha256=aDwqtI6bOPUpI0ryf5joD-whiM-MUaB1pS-43sW3zqo,853504
+xad/adj_1st/__init__.py,sha256=06-d8GpLI7f4PZ4NK2qk9X7v5B1ZM_8guUxs53p8lQ8,2677
+xad/exceptions/__init__.py,sha256=MkaU7fC9GmaCfFHMP_pk6awipV2jkMDnx6XdcCz5BKc,1343
+xad/fwd_1st/__init__.py,sha256=DloUIkLEf86VYPwrH7PPQcIKaw84zlNX3lD-NJnTiWo,2344
+xad/math/__init__.py,sha256=Td_Uy1hpBlRfhZWkMhg8ySz8LpmJphvQiV1DQ1llykI,3450
+xad-1.5.2.dist-info/METADATA,sha256=hj5dHaHJ4M8--dvzAqce2CKczdvy-3mVMgaSFMFhSWI,5255
+xad-1.5.2.dist-info/WHEEL,sha256=1IyMrlk0wO7UertYm7pyjf3m1sV0KDb8wW6mQlBtUog,96
+xad-1.5.2.dist-info/RECORD,,
```

