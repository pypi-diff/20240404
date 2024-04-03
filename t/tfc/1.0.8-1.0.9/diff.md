# Comparing `tmp/tfc-1.0.8.tar.gz` & `tmp/tfc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfc-1.0.8.tar", last modified: Tue Sep 19 15:18:39 2023, max compression
+gzip compressed data, was "tfc-1.0.9.tar", last modified: Thu Sep 28 20:28:11 2023, max compression
```

## Comparing `tfc-1.0.8.tar` & `tfc-1.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:18:39.467227 tfc-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-09-19 15:18:31.000000 tfc-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-19 15:18:31.000000 tfc-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2023-09-19 15:18:39.467227 tfc-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2023-09-19 15:18:31.000000 tfc-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-09-19 15:18:31.000000 tfc-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 15:18:39.467227 tfc-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2023-09-19 15:18:31.000000 tfc-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:18:39.463227 tfc-1.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:18:39.463227 tfc-1.0.8/src/tfc/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26104 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/mtfc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20865 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utfc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:18:39.463227 tfc-1.0.8/src/tfc/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:18:39.467227 tfc-1.0.8/src/tfc/utils/BF/
--rw-r--r--   0 runner    (1001) docker     (127)    44920 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/BF/BF.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    28381 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/BF/BF.h
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/BF/BF.i
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/BF/BF.py
--rw-r--r--   0 runner    (1001) docker     (127)    46499 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/BF/BF_Py.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/BF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109459 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/BF/numpy.i
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/CeSolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/Html.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/Latex.py
--rw-r--r--   0 runner    (1001) docker     (127)    12108 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/MakePlot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12573 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/MayaviMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (127)    25995 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/PlotlyMakePlot.py
--rw-r--r--   0 runner    (1001) docker     (127)    58239 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/TFCUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-19 15:18:31.000000 tfc-1.0.8/src/tfc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:18:39.463227 tfc-1.0.8/src/tfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2023-09-19 15:18:39.000000 tfc-1.0.8/src/tfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-09-19 15:18:39.000000 tfc-1.0.8/src/tfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 15:18:39.000000 tfc-1.0.8/src/tfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-19 15:18:39.000000 tfc-1.0.8/src/tfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-09-19 15:18:39.000000 tfc-1.0.8/src/tfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:28:11.721168 tfc-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-09-28 20:28:04.000000 tfc-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-28 20:28:04.000000 tfc-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2023-09-28 20:28:11.721168 tfc-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2023-09-28 20:28:04.000000 tfc-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-09-28 20:28:04.000000 tfc-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-28 20:28:11.721168 tfc-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2023-09-28 20:28:04.000000 tfc-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:28:11.717168 tfc-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:28:11.717168 tfc-1.0.9/src/tfc/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26321 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/mtfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20921 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utfc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:28:11.721168 tfc-1.0.9/src/tfc/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:28:11.721168 tfc-1.0.9/src/tfc/utils/BF/
+-rw-r--r--   0 runner    (1001) docker     (127)    44920 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/BF/BF.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    28381 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/BF/BF.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/BF/BF.i
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/BF/BF.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46499 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/BF/BF_Py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/BF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109459 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/BF/numpy.i
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/CeSolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/Html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/Latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12108 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/MakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12573 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/MayaviMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25995 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/PlotlyMakePlot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58239 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/TFCUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-09-28 20:28:04.000000 tfc-1.0.9/src/tfc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 20:28:11.717168 tfc-1.0.9/src/tfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2023-09-28 20:28:11.000000 tfc-1.0.9/src/tfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-09-28 20:28:11.000000 tfc-1.0.9/src/tfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 20:28:11.000000 tfc-1.0.9/src/tfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-28 20:28:11.000000 tfc-1.0.9/src/tfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-09-28 20:28:11.000000 tfc-1.0.9/src/tfc.egg-info/top_level.txt
```

### Comparing `tfc-1.0.8/LICENSE` & `tfc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/PKG-INFO` & `tfc-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -81,15 +81,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.8},
+    version = {1.0.9},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.8/README.md` & `tfc-1.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.8},
+    version = {1.0.9},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.8/pyproject.toml` & `tfc-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 requires-python = ">=3.9,<3.12"
 name = "tfc"
-version = "1.0.8"
+version = "1.0.9"
 
 [build-system]
 requires = ["setuptools>=42", 
             "wheel", 
             "numpy>=1.22",
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `tfc-1.0.8/setup.py` & `tfc-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/mtfc.py` & `tfc-1.0.9/src/tfc/mtfc.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     IntArrayLike,
     Array,
     Tuple,
 )
 from jax import core
 from jax.interpreters import ad, batching, mlir
 from jax.lib import xla_client
+from jaxlib import hlo_helpers
+import jaxlib.mlir.ir as ir
 
 from .utils.TFCUtils import TFCPrint
 
 
 class mtfc:
     """
     This is the multivariate TFC class. It acts as a container that holds:
@@ -520,35 +522,22 @@
         d = onp.zeros(self.dim, dtype=np.int32)
         d[2] = 1
         return self._Hjax(*x, d=d, full=full)
 
     def SetupJAX(self):
         """This function is used internally by TFC to setup autograd primatives and create desired behavior when taking derivatives of TFC constrained expressions."""
 
-        # Helper functions
-        def _constant_bool(c, a):
-            return xla_client.ops.Constant(c, bool(a))
-
-        def _constant_s32_scalar(c, a):
-            return xla_client.ops.Constant(c, int(a))
-
-        def _constant_array(c, a):
-            return xla_client.ops.Constant(c, a)
-
-        def _unpack_builder(c):
-            # If `c` is a ComputationBuilder object, extracts the underlying XlaBuilder.
-            return getattr(c, "_builder", c)
-
+        # Helper variables
         d0 = onp.zeros(self.dim, dtype=np.int32)
 
         # Regiser XLA function
         if self._backend == "C++":
             obj = self.basisClass.xlaCapsule
-            xlaName = "BasisFunc" + str(self.basisClass.identifier)
-            xlaName = xlaName.encode("utf-8")
+            xlaName_str = "BasisFunc" + str(self.basisClass.identifier)
+            xlaName = xlaName_str.encode("utf-8")
             xla_client.register_custom_call_target(xlaName, obj, platform="cpu")
 
         # Create Primitives
         H_p = core.Primitive("H")
 
         def Hjax(*x: JaxOrNumpyArray, d: npt.NDArray[onp.int32] = d0, full: bool = False):
             return cast(npt.NDArray, H_p.bind(*x, d=d, full=full))
@@ -573,38 +562,54 @@
                 dims = (x[0].shape[0], dim1)
             return core.ShapedArray(dims, x[0].dtype)
 
         H_p.def_abstract_eval(H_abstract_eval)
 
         if self._backend == "C++":
             # XLA compilation
-            def H_xla(c, *x, d: npt.NDArray[onp.int32] = d0, full: bool = False):
-                c = _unpack_builder(c)
-                x_shape = c.get_shape(x[0])
-                dims = x_shape.dimensions()
-                dtype = x_shape.element_type()
+            def default_layout(shape):
+                return tuple(range(len(shape) - 1, -1, -1))
+
+            def H_xla(ctx, *x, d: uint = 0, full: bool = False):
+                x_type = ir.RankedTensorType(x[0].type)
+                dims = x_type.shape
                 dim0 = dims[0]
                 if full:
                     dim1 = self.basisClass.numBasisFuncFull
                 else:
                     dim1 = self.basisClass.numBasisFunc
-                return xla_client.ops.CustomCall(
-                    c,
-                    xlaName,
-                    (
-                        _constant_s32_scalar(c, self.basisClass.identifier),
-                        xla_client.ops.ConcatInDim(c, x, 0),
-                        _constant_array(c, d),
-                        _constant_s32_scalar(c, self.dim),
-                        _constant_bool(c, full),
-                        _constant_s32_scalar(c, dim0),
-                        _constant_s32_scalar(c, dim1),
-                    ),
-                    xla_client.Shape.array_shape(dtype, (dim0, dim1)),
+                res_types, res_shapes = hlo_helpers.mk_result_types_and_shapes(
+                    [((dim0, dim1), x_type.element_type)]
                 )
+                return hlo_helpers.custom_call(
+                    xlaName_str,
+                    result_types=res_types,
+                    result_shapes=res_shapes,
+                    operands=[
+                        hlo_helpers.hlo_s32(self.basisClass.identifier),
+                        hlo_helpers.hlo.ConcatenateOp(x, 0).result,
+                        hlo_helpers.hlo_s32(d),
+                        hlo_helpers.hlo_s32(self.dim),
+                        mlir.ir_constant(full),
+                        hlo_helpers.hlo_s32(dim0),
+                        hlo_helpers.hlo_s32(dim1),
+                    ],
+                    operand_layouts=[
+                        (),
+                        default_layout((dim0 * len(x),)),
+                        default_layout((len(d),)),
+                        (),
+                        (),
+                        (),
+                        (),
+                    ],
+                    result_layouts=[
+                        default_layout((dim0, dim1)),
+                    ],
+                ).results
 
             mlir.register_lowering(H_p, H_xla, platform="cpu")
 
         # Batching translation
         def H_batch(vec, batch, d: npt.NDArray[onp.int32] = d0, full: bool = False):
             return Hjax(*vec, d=d, full=full), batch[0]
```

### Comparing `tfc-1.0.8/src/tfc/utfc.py` & `tfc-1.0.9/src/tfc/utfc.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import jax.numpy as np
 import numpy.typing as npt
 from typing import Optional, cast
 from .utils.types import Literal, uint, IntArrayLike, JaxOrNumpyArray
 from jax import core
 from jax.interpreters import ad, batching, mlir
 from jax.lib import xla_client
+from jaxlib import hlo_helpers
+import jaxlib.mlir.ir as ir
 
 from .utils.TFCUtils import TFCPrint
 
 
 class utfc:
     """
     This is the univariate TFC class. It acts as a container that creates and stores:
@@ -269,30 +271,19 @@
             Eighth derivative of the basis function matrix.
         """
         return self._Hjax(x, d=8, full=full)
 
     def _SetupJax(self):
         """This function is used internally by TFC to setup JAX primatives and create desired behavior when taking derivatives of TFC constrained expressions."""
 
-        # Helper functions
-        def _constant_bool(c, a):
-            return xla_client.ops.Constant(c, bool(a))
-
-        def _constant_s32_scalar(c, a):
-            return xla_client.ops.Constant(c, int(a))
-
-        def _unpack_builder(c):
-            # If `c` is a ComputationBuilder object, extracts the underlying XlaBuilder.
-            return getattr(c, "_builder", c)
-
         # Regiser XLA function
         if self._backend == "C++":
             obj = self.basisClass.xlaCapsule
-            xlaName = "BasisFunc" + str(self.basisClass.identifier)
-            xlaName = xlaName.encode("utf-8")
+            xlaName_str = "BasisFunc" + str(self.basisClass.identifier)
+            xlaName = xlaName_str.encode("utf-8")
             xla_client.register_custom_call_target(xlaName, obj, platform="cpu")
 
         # Create primitives
         H_p = core.Primitive("H")
 
         def Hjax(x: JaxOrNumpyArray, d: uint = 0, full: bool = False) -> npt.NDArray:
             return cast(npt.NDArray, H_p.bind(x, d=d, full=full))
@@ -315,37 +306,45 @@
                 dims = (x.shape[0], dim1)
             return core.ShapedArray(dims, x.dtype)
 
         H_p.def_abstract_eval(H_abstract_eval)
 
         if self._backend == "C++":
             # XLA compilation
-            def H_xla(c, x, d: uint = 0, full: bool = False):
-                c = _unpack_builder(c)
-                x_shape = c.get_shape(x)
-                dims = x_shape.dimensions()
-                dtype = x_shape.element_type()
+            def default_layout(shape):
+                return tuple(range(len(shape) - 1, -1, -1))
+
+            def H_xla(ctx, x, d: uint = 0, full: bool = False):
+                x_type = ir.RankedTensorType(x.type)
+                dims = x_type.shape
                 dim0 = dims[0]
                 if full:
                     dim1 = self.basisClass.m
                 else:
                     dim1 = self.basisClass.m - self.basisClass.numC
-                return xla_client.ops.CustomCall(
-                    c,
-                    xlaName,
-                    (
-                        _constant_s32_scalar(c, self.basisClass.identifier),
-                        x,
-                        _constant_s32_scalar(c, d),
-                        _constant_bool(c, full),
-                        _constant_s32_scalar(c, dim0),
-                        _constant_s32_scalar(c, dim1),
-                    ),
-                    xla_client.Shape.array_shape(dtype, (dim0, dim1)),
+                res_types, res_shapes = hlo_helpers.mk_result_types_and_shapes(
+                    [((dim0, dim1), x_type.element_type)]
                 )
+                return hlo_helpers.custom_call(
+                    xlaName_str,
+                    result_types=res_types,
+                    result_shapes=res_shapes,
+                    operands=[
+                        hlo_helpers.hlo_s32(self.basisClass.identifier),
+                        x,
+                        hlo_helpers.hlo_s32(d),
+                        mlir.ir_constant(full),
+                        hlo_helpers.hlo_s32(dim0),
+                        hlo_helpers.hlo_s32(dim1),
+                    ],
+                    operand_layouts=[(), default_layout(dims), (), (), (), ()],
+                    result_layouts=[
+                        default_layout((dim0, dim1)),
+                    ],
+                ).results
 
             mlir.register_lowering(H_p, H_xla, platform="cpu")
 
         # Define batching translation
         def H_batch(vec, batch, d: uint = 0, full: bool = False):
             return Hjax(*vec, d=d, full=full), batch[0]
```

### Comparing `tfc-1.0.8/src/tfc/utils/BF/BF.cxx` & `tfc-1.0.9/src/tfc/utils/BF/BF.cxx`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/BF/BF.h` & `tfc-1.0.9/src/tfc/utils/BF/BF.h`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/BF/BF.i` & `tfc-1.0.9/src/tfc/utils/BF/BF.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/BF/BF.py` & `tfc-1.0.9/src/tfc/utils/BF/BF.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/BF/BF_Py.py` & `tfc-1.0.9/src/tfc/utils/BF/BF_Py.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/BF/numpy.i` & `tfc-1.0.9/src/tfc/utils/BF/numpy.i`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/CeSolver.py` & `tfc-1.0.9/src/tfc/utils/CeSolver.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/Html.py` & `tfc-1.0.9/src/tfc/utils/Html.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/Latex.py` & `tfc-1.0.9/src/tfc/utils/Latex.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/MakePlot.py` & `tfc-1.0.9/src/tfc/utils/MakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/MayaviMakePlot.py` & `tfc-1.0.9/src/tfc/utils/MayaviMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/PlotlyMakePlot.py` & `tfc-1.0.9/src/tfc/utils/PlotlyMakePlot.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/TFCUtils.py` & `tfc-1.0.9/src/tfc/utils/TFCUtils.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc/utils/types.py` & `tfc-1.0.9/src/tfc/utils/types.py`

 * *Files identical despite different names*

### Comparing `tfc-1.0.8/src/tfc.egg-info/PKG-INFO` & `tfc-1.0.9/src/tfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tfc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Theory of Functional Connections (TFC): A functional interpolation framework with applications in differential equations.
 Home-page: https://github.com/leakec/tfc.git
 Author: Carl Leake and Hunter Johnston
 Author-email: leakec57@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -81,15 +81,15 @@
 ## Citing this repository:
 The authors of this repsitory and the associated theory have gone to lengths to ensure that both are publicy available at no cost to the user. All that we ask in return is that if you use them, please add a reference to this GitHub and following journal article. Thank you.
 ```
 @misc{tfc2023github,
     author = {Carl Leake and Hunter Johnston},
     title = {{TFC: A Functional Interpolation Framework}},
     url = {https://github.com/leakec/tfc},
-    version = {1.0.8},
+    version = {1.0.9},
     year = {2023},
 }
 @article{TFC, 
     title={The Multivariate Theory of Functional Connections: Theory, Proofs, and Application in Partial Differential Equations}, 
     volume={8}, 
     ISSN={2227-7390}, 
     url={http://dx.doi.org/10.3390/math8081303},
```

### Comparing `tfc-1.0.8/src/tfc.egg-info/SOURCES.txt` & `tfc-1.0.9/src/tfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

