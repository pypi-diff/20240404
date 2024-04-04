# Comparing `tmp/torchao-0.0.3.tar.gz` & `tmp/torchao-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchao-0.0.3.tar", last modified: Thu Jan  4 00:22:39 2024, max compression
+gzip compressed data, was "dist/torchao-0.1.tar", last modified: Thu Apr  4 19:08:15 2024, max compression
```

## Comparing `torchao-0.0.3.tar` & `torchao-0.1.tar`

### file list

```diff
@@ -1,29 +1,38 @@
-drwxr-xr-x   0 cdhernandez (227438) users      (100)        0 2024-01-04 00:22:39.848549 torchao-0.0.3/
--rw-r--r--   0 cdhernandez (227438) users      (100)     1453 2023-11-03 22:22:16.000000 torchao-0.0.3/LICENSE
--rw-r--r--   0 cdhernandez (227438) users      (100)     6260 2024-01-04 00:22:39.848549 torchao-0.0.3/PKG-INFO
--rw-r--r--   0 cdhernandez (227438) users      (100)     6042 2024-01-03 23:13:07.000000 torchao-0.0.3/README.md
--rw-r--r--   0 cdhernandez (227438) users      (100)       38 2024-01-04 00:22:39.848549 torchao-0.0.3/setup.cfg
--rw-r--r--   0 cdhernandez (227438) users      (100)      582 2024-01-04 00:22:32.000000 torchao-0.0.3/setup.py
-drwxr-xr-x   0 cdhernandez (227438) users      (100)        0 2024-01-04 00:22:39.845548 torchao-0.0.3/test/
--rw-r--r--   0 cdhernandez (227438) users      (100)    43383 2024-01-03 22:38:45.000000 torchao-0.0.3/test/test.py
-drwxr-xr-x   0 cdhernandez (227438) users      (100)        0 2024-01-04 00:22:39.845548 torchao-0.0.3/torchao/
--rw-r--r--   0 cdhernandez (227438) users      (100)        0 2023-11-11 00:26:23.000000 torchao-0.0.3/torchao/__init__.py
-drwxr-xr-x   0 cdhernandez (227438) users      (100)        0 2024-01-04 00:22:39.847548 torchao-0.0.3/torchao/quantization/
--rw-r--r--   0 cdhernandez (227438) users      (100)     1485 2023-12-15 01:13:38.000000 torchao-0.0.3/torchao/quantization/__init__.py
--rw-r--r--   0 cdhernandez (227438) users      (100)     2760 2023-12-20 05:09:42.000000 torchao-0.0.3/torchao/quantization/dynamic_quant.py
--rw-r--r--   0 cdhernandez (227438) users      (100)     5771 2023-12-20 05:09:42.000000 torchao-0.0.3/torchao/quantization/quant_api.py
--rw-r--r--   0 cdhernandez (227438) users      (100)    16515 2023-12-11 23:35:08.000000 torchao-0.0.3/torchao/quantization/quant_primitives.py
--rw-r--r--   0 cdhernandez (227438) users      (100)     9153 2024-01-03 22:38:45.000000 torchao-0.0.3/torchao/quantization/smoothquant.py
--rw-r--r--   0 cdhernandez (227438) users      (100)    16953 2023-12-20 05:09:42.000000 torchao-0.0.3/torchao/quantization/subclass.py
--rw-r--r--   0 cdhernandez (227438) users      (100)     2513 2023-12-13 19:27:21.000000 torchao-0.0.3/torchao/quantization/utils.py
--rw-r--r--   0 cdhernandez (227438) users      (100)     2712 2023-12-20 05:09:42.000000 torchao-0.0.3/torchao/quantization/weight_only.py
-drwxr-xr-x   0 cdhernandez (227438) users      (100)        0 2024-01-04 00:22:39.848549 torchao-0.0.3/torchao/sparsity/
--rw-r--r--   0 cdhernandez (227438) users      (100)      370 2023-12-11 23:14:34.000000 torchao-0.0.3/torchao/sparsity/__init__.py
--rw-r--r--   0 cdhernandez (227438) users      (100)     1637 2023-12-11 23:14:34.000000 torchao-0.0.3/torchao/sparsity/utils.py
--rw-r--r--   0 cdhernandez (227438) users      (100)     4071 2023-12-11 23:14:34.000000 torchao-0.0.3/torchao/sparsity/wanda.py
-drwxr-xr-x   0 cdhernandez (227438) users      (100)        0 2024-01-04 00:22:39.846548 torchao-0.0.3/torchao.egg-info/
--rw-r--r--   0 cdhernandez (227438) users      (100)     6260 2024-01-04 00:22:39.000000 torchao-0.0.3/torchao.egg-info/PKG-INFO
--rw-r--r--   0 cdhernandez (227438) users      (100)      575 2024-01-04 00:22:39.000000 torchao-0.0.3/torchao.egg-info/SOURCES.txt
--rw-r--r--   0 cdhernandez (227438) users      (100)        1 2024-01-04 00:22:39.000000 torchao-0.0.3/torchao.egg-info/dependency_links.txt
--rw-r--r--   0 cdhernandez (227438) users      (100)        6 2024-01-04 00:22:39.000000 torchao-0.0.3/torchao.egg-info/requires.txt
--rw-r--r--   0 cdhernandez (227438) users      (100)        8 2024-01-04 00:22:39.000000 torchao-0.0.3/torchao.egg-info/top_level.txt
+drwxr-xr-x   0 jerryzh  (127034) users      (100)        0 2024-04-04 19:08:15.757860 torchao-0.1/
+-rw-r--r--   0 jerryzh  (127034) users      (100)     1453 2024-03-29 01:32:31.000000 torchao-0.1/LICENSE
+-rw-r--r--   0 jerryzh  (127034) users      (100)     5374 2024-04-04 19:08:15.756860 torchao-0.1/PKG-INFO
+-rw-r--r--   0 jerryzh  (127034) users      (100)     5062 2024-03-29 01:32:31.000000 torchao-0.1/README.md
+-rw-r--r--   0 jerryzh  (127034) users      (100)       38 2024-04-04 19:08:15.757860 torchao-0.1/setup.cfg
+-rw-r--r--   0 jerryzh  (127034) users      (100)     1193 2024-04-04 18:46:06.000000 torchao-0.1/setup.py
+drwxr-xr-x   0 jerryzh  (127034) users      (100)        0 2024-04-04 19:08:15.751860 torchao-0.1/torchao/
+-rw-r--r--   0 jerryzh  (127034) users      (100)      206 2024-03-29 01:32:31.000000 torchao-0.1/torchao/__init__.py
+drwxr-xr-x   0 jerryzh  (127034) users      (100)        0 2024-04-04 19:08:15.752860 torchao-0.1/torchao/dtypes/
+-rw-r--r--   0 jerryzh  (127034) users      (100)      136 2024-03-29 01:32:31.000000 torchao-0.1/torchao/dtypes/__init__.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)    20810 2024-03-29 05:15:24.000000 torchao-0.1/torchao/dtypes/nf4tensor.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)    12448 2024-03-29 01:32:31.000000 torchao-0.1/torchao/dtypes/uint4.py
+drwxr-xr-x   0 jerryzh  (127034) users      (100)        0 2024-04-04 19:08:15.753860 torchao-0.1/torchao/kernel/
+-rw-r--r--   0 jerryzh  (127034) users      (100)        0 2024-03-29 01:32:31.000000 torchao-0.1/torchao/kernel/__init__.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     7389 2024-03-29 01:32:31.000000 torchao-0.1/torchao/kernel/autotuner.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     3238 2024-03-30 19:02:42.000000 torchao-0.1/torchao/kernel/intmm.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)    11512 2024-03-29 01:32:31.000000 torchao-0.1/torchao/kernel/intmm_triton.py
+drwxr-xr-x   0 jerryzh  (127034) users      (100)        0 2024-04-04 19:08:15.755860 torchao-0.1/torchao/quantization/
+-rw-r--r--   0 jerryzh  (127034) users      (100)    52411 2024-04-04 06:37:03.000000 torchao-0.1/torchao/quantization/GPTQ.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     1574 2024-04-04 05:15:35.000000 torchao-0.1/torchao/quantization/__init__.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     2747 2024-03-29 01:32:31.000000 torchao-0.1/torchao/quantization/dynamic_quant.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     6290 2024-04-04 05:15:35.000000 torchao-0.1/torchao/quantization/quant_api.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)    18695 2024-04-04 05:15:35.000000 torchao-0.1/torchao/quantization/quant_primitives.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     9159 2024-03-29 01:32:31.000000 torchao-0.1/torchao/quantization/smoothquant.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)    17574 2024-04-03 22:11:55.000000 torchao-0.1/torchao/quantization/subclass.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)      754 2024-03-30 19:02:42.000000 torchao-0.1/torchao/quantization/unified.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     3169 2024-04-03 23:22:38.000000 torchao-0.1/torchao/quantization/utils.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     2742 2024-04-04 18:44:54.000000 torchao-0.1/torchao/quantization/weight_only.py
+drwxr-xr-x   0 jerryzh  (127034) users      (100)        0 2024-04-04 19:08:15.756860 torchao-0.1/torchao/sparsity/
+-rw-r--r--   0 jerryzh  (127034) users      (100)      370 2024-03-29 01:32:31.000000 torchao-0.1/torchao/sparsity/__init__.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     1708 2024-03-29 01:32:31.000000 torchao-0.1/torchao/sparsity/utils.py
+-rw-r--r--   0 jerryzh  (127034) users      (100)     4156 2024-03-29 01:32:31.000000 torchao-0.1/torchao/sparsity/wanda.py
+drwxr-xr-x   0 jerryzh  (127034) users      (100)        0 2024-04-04 19:08:15.756860 torchao-0.1/torchao.egg-info/
+-rw-r--r--   0 jerryzh  (127034) users      (100)     5374 2024-04-04 19:08:15.000000 torchao-0.1/torchao.egg-info/PKG-INFO
+-rw-r--r--   0 jerryzh  (127034) users      (100)      812 2024-04-04 19:08:15.000000 torchao-0.1/torchao.egg-info/SOURCES.txt
+-rw-r--r--   0 jerryzh  (127034) users      (100)        1 2024-04-04 19:08:15.000000 torchao-0.1/torchao.egg-info/dependency_links.txt
+-rw-r--r--   0 jerryzh  (127034) users      (100)       36 2024-04-04 19:08:15.000000 torchao-0.1/torchao.egg-info/requires.txt
+-rw-r--r--   0 jerryzh  (127034) users      (100)        8 2024-04-04 19:08:15.000000 torchao-0.1/torchao.egg-info/top_level.txt
```

### Comparing `torchao-0.0.3/LICENSE` & `torchao-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchao-0.0.3/torchao/quantization/__init__.py` & `torchao-0.1/torchao/quantization/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .smoothquant import *  # noqa: F403
 from .quant_api import *  # noqa: F403
 from .subclass import *  # noqa: F403
 from .quant_primitives import *  # noqa: F403
 from .utils import *  # noqa: F403
 from .weight_only import *  # noqa: F403
+from .unified import *
 
 __all__ = [
     "DynamicallyPerAxisQuantizedLinear",
     "apply_weight_only_int8_quant",
     "apply_dynamic_quant",
     "change_linear_weights_to_int8_dqtensors",
     "change_linear_weights_to_int8_woqtensors",
@@ -37,8 +38,10 @@
     "set_smooth_fq_attribute",
     "Int8DynamicallyQuantizedLinearWeight",
     "Int8WeightOnlyQuantizedLinearWeight",
     "Int4WeightOnlyQuantizedLinearWeight",
     "compute_error",
     "get_model_size_in_bytes",
     "WeightOnlyInt8QuantLinear",
+    "Int4WeightOnlyGPTQQuantizer",
+    "Int4WeightOnlyQuantizer",
 ]
```

### Comparing `torchao-0.0.3/torchao/quantization/dynamic_quant.py` & `torchao-0.1/torchao/quantization/dynamic_quant.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 import torch.nn as nn
+
 from .quant_primitives import (
     dynamically_quantize_per_channel,
     quant_int8_dynamic_per_token_linear,
 )
 
 __all__ = ["DynamicallyPerAxisQuantizedLinear"]
 
@@ -45,17 +46,15 @@
 
         Y = quant_int8_dynamic_per_token_linear(
             X, self.W_int_repr_t, self.W_scales, self.bias, X.dtype
         )
         return Y
 
     @classmethod
-    def from_float(
-        cls, mod: torch.nn.Linear
-    ) -> "DynamicallyPerAxisQuantizedLinear":
+    def from_float(cls, mod: torch.nn.Linear) -> "DynamicallyPerAxisQuantizedLinear":
         """
         Converts a `mod` of class `torch.nn.Linear` to the
         `DynamicallyPerAxisQuantizedLinear` class
 
         Args:
             mod (torch.nn.Linear): The original `torch.nn.Linear` module to convert.
```

### Comparing `torchao-0.0.3/torchao/quantization/quant_api.py` & `torchao-0.1/torchao/quantization/quant_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,39 +12,65 @@
 usage involves applying torch.compile to the model afterwards
 both because primitives were designed based on the fusions that
 come along with it and because that is how we access the intended quantized
 and mixed GEMM kernels
 """
 
 import torch
-from .dynamic_quant import (
-    DynamicallyPerAxisQuantizedLinear,
-)
+import torch.nn as nn
+import torch.nn.functional as F
+
+from .dynamic_quant import DynamicallyPerAxisQuantizedLinear
+from .utils import TORCH_VERSION_AFTER_2_3
+
 from .subclass import (
-    QuantizedLinearWeightBase,
+    Int4WeightOnlyQuantizedLinearWeight,
     Int8DynamicallyQuantizedLinearWeight,
     Int8WeightOnlyQuantizedLinearWeight,
-    Int4WeightOnlyQuantizedLinearWeight,
+    QuantizedLinearWeightBase,
 )
-from .weight_only import (
-    WeightOnlyInt8QuantLinear,
+from .weight_only import WeightOnlyInt8QuantLinear
+from .unified import Quantizer, TwoStepQuantizer
+from .GPTQ import (
+    Int4WeightOnlyGPTQQuantizer,
+    Int4WeightOnlyQuantizer,
 )
 
+
 __all__ = [
     "apply_weight_only_int8_quant",
     "apply_dynamic_quant",
     "change_linear_weights_to_int8_dqtensors",
     "change_linear_weights_to_int8_woqtensors",
     "change_linear_weights_to_int4_woqtensors",
-    "swap_conv2d_1x1_to_linear"
+    "swap_conv2d_1x1_to_linear",
+    "Quantizer",
+    "TwoStepQuantizer",
+    "Int4WeightOnlyGPTQQuantizer",
+    "Int4WeightOnlyQuantizer"
 ]
 
+if TORCH_VERSION_AFTER_2_3:
+    from .GPTQ import (
+        Int8DynActInt4WeightQuantizer,
+        Int8DynActInt4WeightGPTQQuantizer,
+
+    )
+    __all__ += [
+        "Int8DynActInt4WeightQuantizer",
+        "Int8DynActInt4WeightGPTQQuantizer",
+
+    ]
+
 
 def _replace_with_custom_fn_if_matches_filter(
-    model, replacement_fn, filter_fn, cur_fqn=""
+    model,
+    replacement_fn,
+    filter_fn,
+    cur_fqn="",
 ) -> None:
     """
     For each `child` in `model`, replaces it with `replacement_fn(child)`
     if `filter_fn(child)` is `True`
     """
     if filter_fn(model, cur_fqn[:-1]):
         model = replacement_fn(model)
@@ -57,22 +83,24 @@
             if new_child is not child:
                 setattr(model, name, new_child)
         return model
 
 
 def _is_linear(mod, *args):
     return (
-        isinstance(mod, torch.nn.Linear) and
-        hasattr(mod, "weight") and
-        not isinstance(mod.weight, QuantizedLinearWeightBase)
+        isinstance(mod, torch.nn.Linear)
+        and hasattr(mod, "weight")
+        and not isinstance(mod.weight, QuantizedLinearWeightBase)
     )
 
+
 def _in_features_greater_than_16(mod, *args):
     return hasattr(mod, "in_features") and mod.in_features > 16
 
+
 def apply_weight_only_int8_quant(model, filter_fn=None):
     """
     Applies weight-only symmetric per-channel int8 quantization to all linear layers
     in the given model using module swaps.
     """
     _replace_with_custom_fn_if_matches_filter(
         model,
@@ -80,25 +108,22 @@
         _is_linear if filter_fn is None else filter_fn,
     )
 
 
 def apply_dynamic_quant(model, filter_fn=None):
     """
     Applies dynamic symmetric per-token activation and per-channel weight
-    quantization to all linear layers in the given model using
-    module swaps.
+    quantization to all linear layers by converting all linear weight
+    tensors to the `Int8DynamicallyQuantizedLinearWeight` Tensor subclass.
     """
-    _replace_with_custom_fn_if_matches_filter(
-        model,
-        lambda mod: DynamicallyPerAxisQuantizedLinear.from_float(mod),
-        _is_linear if filter_fn is None else filter_fn,
-    )
+    change_linear_weights_to_int8_dqtensors(model, filter_fn)
 
 
 def _get_subclass_inserter(cls, **kwargs):
+
     def insert_subclass(lin):
         lin.weight = torch.nn.Parameter(
             cls.from_float(lin.weight, **kwargs), requires_grad=False
         )
         return lin
 
     return insert_subclass
@@ -107,24 +132,20 @@
 def change_linear_weights_to_int8_dqtensors(model, filter_fn=None):
     """
     Converts all linear weight tensors to the `Int8DynamicallyQuantizedLinearWeight`
     Tensor subclass, effectively applying the same form of quantization
     as apply_dynamic_quant while not modifying the linear modules.
     """
     if filter_fn is None:
-        filter_fn = (
-            lambda *args:
-            _is_linear(*args) and
-            _in_features_greater_than_16(*args)
+        filter_fn = lambda *args: _is_linear(*args) and _in_features_greater_than_16(
+            *args
         )
 
     _replace_with_custom_fn_if_matches_filter(
-        model,
-        _get_subclass_inserter(Int8DynamicallyQuantizedLinearWeight),
-        filter_fn
+        model, _get_subclass_inserter(Int8DynamicallyQuantizedLinearWeight), filter_fn
     )
 
 
 def change_linear_weights_to_int8_woqtensors(model, filter_fn=None):
     """
     Converts all linear weight tensors to the
     `Int8WeightOnlyQuantizedLinearWeight` tensor subclass,
@@ -149,35 +170,38 @@
 
     _replace_with_custom_fn_if_matches_filter(
         model,
         _get_subclass_inserter(Int4WeightOnlyQuantizedLinearWeight, **kwargs),
         filter_fn,
     )
 
+
 def swap_conv2d_1x1_to_linear(model, filter_fn=None):
     """
     Changes all conv2d 1x1 modules to equivalent linear modules so that they can then be quantized.
     """
+
     class PermuteSandwich(torch.nn.Module):
         def __init__(self, mod):
             super().__init__()
             self.mod = mod
 
         def forward(self, *args):
-            return self.mod(args[0].permute(0, 2, 3, 1)).permute(-0,3,1,2)
-
+            return self.mod(args[0].permute(0, 2, 3, 1)).permute(-0, 3, 1, 2)
 
     def replace_conv2d_1x1(conv):
         assert conv.kernel_size == (1, 1)
-        lin = torch.nn.Linear(conv.in_channels, conv.out_channels, bias=(conv.bias is None))
-        lin.weight=torch.nn.Parameter(conv.weight.squeeze(-1,-2))
+        lin = torch.nn.Linear(
+            conv.in_channels, conv.out_channels, bias=(conv.bias is None)
+        )
+        lin.weight = torch.nn.Parameter(conv.weight.squeeze(-1, -2))
         lin.bias = conv.bias
         return PermuteSandwich(lin)
 
     if filter_fn is None:
-        filter_fn=lambda mod, *args: isinstance(mod, torch.nn.Conv2d) and mod.kernel_size==(1,1)
+        filter_fn = lambda mod, *args: isinstance(
+            mod, torch.nn.Conv2d
+        ) and mod.kernel_size == (1, 1)
 
     _replace_with_custom_fn_if_matches_filter(
-        model,
-        replace_conv2d_1x1,
-        filter_fn=filter_fn
+        model, replace_conv2d_1x1, filter_fn=filter_fn
     )
```

### Comparing `torchao-0.0.3/torchao/quantization/quant_primitives.py` & `torchao-0.1/torchao/quantization/quant_primitives.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
 from torch._dynamo import is_compiling as dynamo_is_compiling
 from torch._higher_order_ops.out_dtype import out_dtype
+from torch.ao.quantization.fx._decomposed import quantized_decomposed_lib
+from torch.library import impl
+
+from torchao.kernel.intmm import int_scaled_matmul
+from torchao.kernel.intmm import safe_int_mm
+from .utils import TORCH_VERSION_AFTER_2_3
+
+
+_AFTER_TORCH_2_3_ONLY = [
+    "per_token_dynamic_quant",
+    "get_group_qparams_symmetric",
+]
 
 __all__ = [
     "safe_int_mm",
     "dynamically_quantize_per_tensor",
     "quantize_activation_per_token_absmax",
     "dynamically_quantize_per_channel",
     "dequantize_per_tensor",
@@ -22,73 +34,19 @@
     "get_groupwise_affine_qparams",
     "pack_tinygemm_scales_and_zeros",
     "unpack_tinygemm_scales_and_zeros",
     "groupwise_affine_quantize_tensor_from_qparams",
     "groupwise_affine_dequantize_tensor_from_qparams",
     "groupwise_affine_quantize_tensor",
     "groupwise_affine_dequantize_tensor",
-]
-
-
-def safe_int_mm(input: torch.Tensor, mat2: torch.Tensor) -> torch.Tensor:
-    r"""
-    This function wraps torch._int_mm and avoids several undesirable behaviors of the function for certain inputs while still
-    returning correct results and being torch.compiled in a performant way.
-
-    Assumes both tensors have dimension of 2.
-
-    Note: no error checking for torch.compiled path, if input.shape = [i, j] and j<=16 then the triton kernel
-    will error.
-
-    Args:
-        input (Tensor, int8): the first tensor to be multiplied
-        mat2 (Tensor, int8): the second tensor to be multiplied
-
-    Return:
-        out (Tensor, int32): the result of the matmul with device matching that of the inputs
-    """
-
-    # torch.compile path
-    if dynamo_is_compiling() or "FakeTensor" in input.__repr__():
-        return out_dtype(torch.ops.aten.mm.default, torch.int32, input, mat2)
-
-    # error checking for cublas path
-    assert (
-        mat2.device == input.device
-    ), f"need both tensors to be on the same device but got {mat2.device} and {input.device}"
-    device_cpu = "cpu" in [mat2.device.type, input.device.type]
-    # with input.shape = [i,j] and mat2.shape = [j,k]
-    i_is_strictly_greater_than_16 = input.shape[0] > 16
-    j_is_nonzero_multiple_of_8 = (input.shape[1] % 8 == 0) and (input.shape[1] > 0)
-    k_is_nonzero_multiple_of_8 = (mat2.shape[1] % 8 == 0) and (mat2.shape[1] > 0)
-    bad_dimensions_for_cublas = not (
-        i_is_strictly_greater_than_16
-        and j_is_nonzero_multiple_of_8
-        and k_is_nonzero_multiple_of_8
-    )
-
-    if device_cpu or bad_dimensions_for_cublas:
-        # fallback path
-        return torch.matmul(input.cpu().to(torch.int32), mat2.cpu().to(torch.int32)).to(
-            input.device.type
-        )
-
-    # cublas paths
-    if not mat2.is_contiguous():  # silently gives incorrect result without this
-        mat2 = mat2.contiguous()
-    if (not input.is_contiguous()) and (
-        input.shape[0] % 8 != 0
-    ):  # gives cryptic error without this
-        input = (
-            input.contiguous()
-        )  # (it seems the transpose makes cublas check the above j constraint on i)
-    return out_dtype(torch.ops.aten.mm.default, torch.int32, input, mat2)
-
+    # TODO: need to clean up above functions
+] + (_AFTER_TORCH_2_3_ONLY if TORCH_VERSION_AFTER_2_3 else [])
 
 # copy-pasta of https://www.internalfb.com/intern/anp/view/?id=3350736
+
 def dynamically_quantize_per_tensor(
     x,
     quant_min,
     quant_max,
     target_dtype,
     qscheme=torch.per_tensor_affine,  # for now, reuse existing qscheme enum
 ):
@@ -104,15 +62,14 @@
         min_val = torch.min(x)
         max_val = torch.max(x)
 
         # calculate scale and zero point based on min and max
         # reference: https://fburl.com/code/srbiybme
         min_val_neg = torch.min(min_val, torch.zeros_like(min_val))
         max_val_pos = torch.max(max_val, torch.zeros_like(max_val))
-        device = min_val_neg.device
 
         scale = (max_val_pos - min_val_neg) / float(quant_max - quant_min)
         # TODO(future): make torch.clamp with scalar work on cpu-half
         scale = torch.clamp(scale, min=eps).reshape(1)
         zero_point = quant_min - torch.round(min_val_neg / scale).to(torch.int)
         zero_point = torch.clamp(zero_point, quant_min, quant_max)
 
@@ -136,14 +93,16 @@
 
     return quant, scale, zero_point
 
 
 # taken from
 # https://github.com/mit-han-lab/smoothquant/blob/2f87951dacfb9238d8d657f52ae83a82a3c9ba0c/smoothquant/fake_quant.py#L26
 # and slightly modified
+
+
 def quantize_activation_per_token_absmax(t):
     n_bits = 8
     # if the shape of t is [B, N, K], the shape of scales will be [B, N, 1]
 
     scales = t.abs().amax(dim=-1, keepdim=True)
     if scales.dtype == torch.float16:
         scales = (
@@ -191,22 +150,26 @@
     x_zp = x_zp.transpose(0, 1)
     quant = torch.clamp(x_zp, quant_min, quant_max).to(target_dtype)
 
     return quant, scale, zero_point
 
 
 # reference: https://fburl.com/code/vfsygwd0
+
+
 def dequantize_per_tensor(int_repr, scale, zero_point, out_dtype=torch.float32):
     y = int_repr.to(out_dtype)
     if zero_point is not None:
         y -= zero_point
     return y * scale
 
 
 # reference: https://fburl.com/code/org0fmi3
+
+
 def dequantize_per_channel(int_repr, scales, zero_points, out_dtype=torch.float32):
     # assumes axis is 0
     y = int_repr.transpose(0, 1)
     y = y.to(out_dtype)
     y = y - zero_points
     y = y * scales
     y = y.transpose(0, 1)
@@ -348,36 +311,35 @@
     assert (
         x_vals_int8.dtype == torch.int8
     ), f"x dtype {x_vals_int8.dtype} not yet supported"
     assert (
         w_vals_int8_t.dtype == torch.int8
     ), f"w dtype {w_vals_int8_t.dtype} not yet supported"
 
+    assert x_scales.dtype in [
+        torch.float,
+        torch.bfloat16,
+    ], f"x_scales needs to be a torch.float32 or torch.bfloat16 but got {x_scales.dtype}"
+
     #
     # 1. do the matrix form of dot(X_i, W_j)
     #
-
-    tmp = x_vals_int8.reshape(-1, x_vals_int8.shape[-1])
-    y_dot_int32 = safe_int_mm(tmp, w_vals_int8_t)
-
     #
     # 2. rescale the output
     #
     # in cases with large matrices, y_dot_int32 can grow sufficiently
     # large that y_dot_int32 * a float16 scale is greater than the maximum
     # value of a float 16, (which results in a value of inf even if multiplying
     # by the other scale would bring it within the expected range)
 
-    assert x_scales.dtype in [
-        torch.float,
-        torch.bfloat16,
-    ], f"x_scales needs to be a torch.float32 or torch.bfloat16 but got {x_scales.dtype}"
+    tmp = x_vals_int8.reshape(-1, x_vals_int8.shape[-1])
+    y_dot_scaled = int_scaled_matmul(tmp, w_vals_int8_t, x_scales.reshape(-1, 1))
 
-    y = (y_dot_int32 * x_scales.reshape(-1, 1) * w_scales).reshape(
-        *x_vals_int8.shape[:-1], y_dot_int32.shape[-1]
+    y = (y_dot_scaled * w_scales).reshape(
+        *x_vals_int8.shape[:-1], y_dot_scaled.shape[-1]
     )
 
     # can downcast only at the very end
     y = y.to(output_dtype)
     return y
 
 
@@ -417,20 +379,23 @@
         .transpose(0, 1)
         .contiguous()
     )
 
 
 def unpack_tinygemm_scales_and_zeros(scales_and_zeros):
     assert len(scales_and_zeros.shape) == 3 and scales_and_zeros.shape[2] == 2
-    assert scales_and_zeros.dtype == torch.float
     return torch.split(scales_and_zeros.transpose(0, 1), 1, 2)
 
 
 def groupwise_affine_quantize_tensor_from_qparams(
-    w, scales, zeros, n_bit=4, groupsize=128
+    w,
+    scales,
+    zeros,
+    n_bit=4,
+    groupsize=128,
 ):
     assert groupsize > 1
     # needed for GPTQ single column quantize
     if groupsize > w.shape[-1] and scales.shape[-1] == 1:
         groupsize = w.shape[-1]
 
     assert w.shape[-1] % groupsize == 0
@@ -453,15 +418,19 @@
         .reshape_as(w)
     )
 
     return w_int4x8
 
 
 def groupwise_affine_dequantize_tensor_from_qparams(
-    w_int4x8, scales, zeros, n_bit=4, groupsize=128
+    w_int4x8,
+    scales,
+    zeros,
+    n_bit=4,
+    groupsize=128,
 ):
     assert groupsize > 1
     # needed for GPTQ single column dequantize
     if groupsize > w_int4x8.shape[-1] and scales.shape[-1] == 1:
         groupsize = w_int4x8.shape[-1]
     assert w_int4x8.shape[-1] % groupsize == 0
     assert w_int4x8.dim() == 2
@@ -485,13 +454,123 @@
         w, scales, zeros, n_bit, groupsize
     )
     scales_and_zeros = pack_tinygemm_scales_and_zeros(scales, zeros)
     return w_int4x8, scales_and_zeros
 
 
 def groupwise_affine_dequantize_tensor(
-    w_int4x8, scales_and_zeros, n_bit=4, groupsize=128
+    w_int4x8,
+    scales_and_zeros,
+    n_bit=4,
+    groupsize=128,
 ):
     scales, zeros = unpack_tinygemm_scales_and_zeros(scales_and_zeros)
     return groupwise_affine_dequantize_tensor_from_qparams(
         w_int4x8, scales, zeros, n_bit, groupsize
     )
+
+
+# TODO: replace this with torch.ao.quantization.PerChannelMinMaxObserver
+def get_group_qparams_symmetric(w, n_bit=4, groupsize=128, precision=torch.float32):
+    # needed for GPTQ with padding
+    if groupsize > w.shape[-1]:
+        groupsize = w.shape[-1]
+    assert groupsize > 1
+    assert w.shape[-1] % groupsize == 0
+    assert w.dim() == 2
+
+    to_quant = w.reshape(-1, groupsize)
+    assert torch.isnan(to_quant).sum() == 0
+
+    max_val = to_quant.amax(dim=1, keepdim=True)
+    min_val = to_quant.amin(dim=1, keepdim=True)
+    min_val_neg = torch.min(min_val, torch.zeros_like(min_val))
+    max_val_pos = torch.max(max_val, torch.zeros_like(max_val))
+
+    max_val_abs = torch.max(-min_val_neg, max_val_pos)
+    max_int = 2 ** (n_bit - 1) - 1
+    min_int = -(2 ** (n_bit - 1))
+
+    scales = max_val_abs / (float(max_int - min_int) / 2)
+    scales = torch.max(scales, torch.full_like(scales, torch.finfo(torch.float32).eps))
+    # TODO: make sure abs(scales) is not too small?
+    zeros = torch.full_like(scales, 0)
+    return scales.to(precision).reshape(w.shape[0], -1), zeros.to(precision).reshape(
+        w.shape[0], -1
+    )
+
+
+if TORCH_VERSION_AFTER_2_3:
+    def group_quantize_tensor_symmetric(
+        w,
+        n_bit=4,
+        group_size=128,
+        precision=torch.float32,
+    ):
+        scales, zeros = get_group_qparams_symmetric(w, n_bit, group_size, precision)
+        n_bit = 4
+        max_int = 2 ** (n_bit - 1) - 1
+        min_int = -(2 ** (n_bit - 1))
+        # TODO: currently we don't know how to express torch.int4, we'll
+        # add torch.int4 to core later
+        w_int8 = torch.ops.quantized_decomposed.quantize_per_channel_group(
+            w, scales, zeros, min_int, max_int, torch.int8, group_size
+        )
+
+        return w_int8, scales, zeros
+
+
+    def down_size(size):
+        assert size[-1] % 2 == 0, f"{size} last dim not divisible by two"
+        return (*size[:-1], size[-1] // 2)
+
+
+    def up_size(size):
+        return (*size[:-1], size[-1] * 2)
+
+
+    quantized_decomposed_lib.define("pack_int4_from_int8(Tensor int8_data) -> Tensor")
+
+
+    @impl(quantized_decomposed_lib, "pack_int4_from_int8", "CompositeExplicitAutograd")
+    def pack_int4_from_int8(int8_data: torch.Tensor) -> torch.Tensor:
+        # converting to uint8 for operations
+        shape = int8_data.shape
+        assert shape[-1] % 2 == 0
+        int8_data = int8_data.contiguous().view(-1)
+        return (int8_data[::2] << 4 | int8_data[1::2]).view(down_size(shape))
+
+
+    quantized_decomposed_lib.define("unpack_int4_to_int8(Tensor int8_data) -> Tensor")
+
+
+    @impl(quantized_decomposed_lib, "unpack_int4_to_int8", "CompositeExplicitAutograd")
+    def unpack_int4_to_int8(int8_data: torch.Tensor) -> torch.Tensor:
+        """Get the original weight from the normalized float weight format"""
+        # since we are using int8 we will decode 2 entries per byte
+        # Shift elements down 4 and select out the bottom 4 bits
+        shape = int8_data.shape
+        first_elements = (int8_data >> 4).to(torch.int8)
+        second_elements = (int8_data & 0b1111).to(torch.int8)
+        return torch.stack([first_elements, second_elements], dim=-1).view(up_size(shape))
+
+
+    def per_token_dynamic_quant(input: torch.Tensor) -> torch.Tensor:
+        orig_dtype = input.dtype
+        # TODO: we may need to make the choose_qparams op configurable
+        (
+            scales,
+            zero_points,
+        ) = torch.ops.quantized_decomposed.choose_qparams_per_token_asymmetric(
+            input, torch.int8
+        )
+
+        # TODO: get these from torch.int8
+        quant_min = -128
+        quant_max = 127
+        input = torch.ops.quantized_decomposed.quantize_per_token(
+            input, scales, zero_points, quant_min, quant_max, torch.int8
+        )
+        input = torch.ops.quantized_decomposed.dequantize_per_token(
+            input, scales, zero_points, quant_min, quant_max, torch.int8, orig_dtype
+        )
+        return input.to(orig_dtype)
```

### Comparing `torchao-0.0.3/torchao/quantization/smoothquant.py` & `torchao-0.1/torchao/quantization/smoothquant.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Note: this is an application of input-weight equalization, with the addition that the
 multiplication by scale is fused into the preceding layer, specifically for relevant
 parts of transformer blocks.
 """
 
 import torch
 import torch.nn.functional as F
+
 import torchao.quantization.quant_api as quant_api
 
 from .quant_primitives import (
     dynamically_quantize_per_channel,
     quant_int8_dynamic_per_token_linear,
 )
 
@@ -26,14 +27,15 @@
     "SmoothFakeDynQuantMixin",
     "SmoothFakeDynamicallyQuantizedLinear",
     "swap_linear_with_smooth_fq_linear",
     "smooth_fq_linear_to_inference",
     "set_smooth_fq_attribute",
 ]
 
+
 def get_scale(X_absmax, W_absmax, alpha=0.5):
     """
     Calculate the scale based on abs(max(X)), abs(max(W)) and alpha
     If X is of dimension `b*n*k` and W is dimension `k*m`, the returned
     scale is of dimension `k`.
     Note: X_absmax is calculated outside of this function because we
     need to keep a running version of it during calibration. W_absmax
@@ -42,14 +44,15 @@
     X_pow = torch.pow(X_absmax, alpha)
     W_pow = torch.pow(W_absmax, 1.0 - alpha)
     div = X_pow / W_pow
     return div.reshape(-1)
 
 
 class SmoothFakeDynQuantMixin(torch.nn.Module):
+
     def init_smoothquant_variables(self, alpha):
         self.calibrating = True
         self.x_running_abs_max = None
         self.register_buffer("smooth_scale", None)
         self.alpha = alpha
         # debug only
         self.debug_skip_scaling = False
@@ -189,14 +192,15 @@
         )
         self.fold_weight()
 
     def set_debug_x_absmax(self):
         w_absmax = torch.max(torch.abs(self.weight.transpose(0, 1)), dim=1).values
         self.x_running_abs_max = w_absmax
 
+
 #
 # utils to use the smooth linear on real models
 #
 
 source_cls_to_target_cls = {
     torch.nn.Linear: SmoothFakeDynamicallyQuantizedLinear,
     torch.nn.modules.linear.NonDynamicallyQuantizableLinear: SmoothFakeDynamicallyQuantizedLinear,
@@ -229,12 +233,14 @@
             if debug_skip_calibration:
                 mod.set_debug_x_absmax()
             mod.to_inference()
 
 
 # useful for quickly toggling smoothquant debug settings on all smoothquant
 # modules in a model
+
+
 def set_smooth_fq_attribute(model, attribute_name, new_attribute_val):
     for _, mod in model.named_modules():
         if isinstance(mod, tuple(source_cls_to_target_cls.values())):
             if hasattr(mod, attribute_name):
                 setattr(mod, attribute_name, new_attribute_val)
```

### Comparing `torchao-0.0.3/torchao/quantization/subclass.py` & `torchao-0.1/torchao/quantization/subclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
+import warnings
+
 import torch
 from torch.utils._python_dispatch import return_and_correct_aliasing
 
 from .quant_primitives import (
     dequantize_per_channel,
     dynamically_quantize_per_channel,
     groupwise_affine_quantize_tensor,
     quant_int8_dynamic_per_token_linear,
     unpack_tinygemm_scales_and_zeros,
 )
 from .utils import find_multiple
-import warnings
 
 
 __all__ = [
     "Int8DynamicallyQuantizedLinearWeight",
     "Int8WeightOnlyQuantizedLinearWeight",
     "Int4WeightOnlyQuantizedLinearWeight",
 ]
 
+
 aten = torch.ops.aten
 
+
 class QuantizedLinearWeightBase(torch.Tensor):
     """
     Base quantized tensor subclass for quantized linear weights. When the from_float method is used,
     to create an instance of any QuantizedLinearWeightBase, we assume the input
     weight is oriented the way it is in a normal linear op, i.e. out-channels x in-channels.
 
     The shape and dtype of the tensor subclass represent how the tensor subclass looks externally,
@@ -44,15 +47,17 @@
         )
         assert "dtype" in kwargs
         assert not kwargs.get("requires_grad", False)
         kwargs["requires_grad"] = False
         return torch.Tensor._make_wrapper_subclass(cls, shape, **kwargs)  # type: ignore[attr-defined]
 
     def __init__(self, int_data, transposed, *args, **kwargs):
+
         self.int_data = int_data
+
         self.transposed = transposed
 
     @staticmethod
     def _quantized_op(act_mat, w_qtensor, bias):
         pass
 
     def __repr__(self):
@@ -93,15 +98,17 @@
     def _change_shape(self):
         pass
 
     def __tensor_flatten__(self):
         pass
 
     @classmethod
-    def __tensor_unflatten__(cls, tensor_data_dict, tensor_attributes, outer_size, outer_stride):
+    def __tensor_unflatten__(
+        cls, tensor_data_dict, tensor_attributes, outer_size, outer_stride
+    ):
         pass
 
     @classmethod
     def from_float(cls, input_float):
         pass
 
     # __torch_function__ = torch._C._disabled_torch_function_impl
@@ -110,15 +117,15 @@
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         kwargs = {} if kwargs is None else kwargs
 
         if func is torch.nn.functional.linear:
             mat1, w_qtensor, bias = (
                 args[0],
                 args[1],
-                args[2] if len(args)>2 else None
+                args[2] if len(args) > 2 else None,
             )
             assert w_qtensor.transposed == False
             return cls._quantized_op(mat1, w_qtensor, bias)
 
         try:
             with torch._C.DisableTorchFunctionSubclass():
                 return func(*args, **kwargs)
@@ -150,33 +157,42 @@
                 assert args[0].shape[-1] == args[1].shape[0], (
                     f"need mat1 shape: {args[0].shape} final dim"
                     f"to match mat2 shape: {args[1].shape} first dim"
                 )
                 mat1, w_qtensor, bias = (
                     args[0],
                     args[1],
-                    None if len(args)==2 else args[2],
+                    None if len(args) == 2 else args[2],
                 )
             # call the quantized op for the specific type
             # of quantized tensor subclass
             return cls._quantized_op(mat1, w_qtensor, bias)
 
         if func is aten.detach.default:
-            return return_and_correct_aliasing(func, args, kwargs, args[0]._apply_fn_to_data(torch.detach))
+            return return_and_correct_aliasing(
+                func, args, kwargs, args[0]._apply_fn_to_data(torch.detach)
+            )
 
         if func is aten.clone.default:
-            return return_and_correct_aliasing(func, args, kwargs, args[0]._apply_fn_to_data(torch.clone))
+            return return_and_correct_aliasing(
+                func, args, kwargs, args[0]._apply_fn_to_data(torch.clone)
+            )
 
         if func is aten.t.default:
             args[0].transposed = not args[0].transposed
             new = args[0]._change_shape(args[0].shape[::-1])
             return return_and_correct_aliasing(func, args, kwargs, new)
 
         if func is aten._to_copy.default:
-            return return_and_correct_aliasing(func, args, kwargs, args[0].to(*args[1:], **kwargs)._apply_fn_to_data(torch.clone))
+            return return_and_correct_aliasing(
+                func,
+                args,
+                kwargs,
+                args[0].to(*args[1:], **kwargs)._apply_fn_to_data(torch.clone),
+            )
 
 
 class Int8DynamicallyQuantizedLinearWeight(QuantizedLinearWeightBase):
     """
     A Tensor subclass that when applied to a weight used in a linear op/module, changes the
     linear op to a dynamically quantized linear op with symmetric per-token and per-channel
     quantization on the activation and weight respectively.
@@ -184,14 +200,15 @@
 
     @staticmethod
     def __new__(cls, int_data, q_scales, transposed, shape, **kwargs):
         kwargs["dtype"] = kwargs.get("dtype", q_scales.dtype)
         return super().__new__(cls, int_data, transposed, shape, **kwargs)  # type: ignore[attr-defined]
 
     def __init__(self, int_data, q_scales, transposed, shape, **kwargs):
+
         self.q_scales = q_scales
         super().__init__(int_data, transposed)
 
     @staticmethod
     def _quantized_op(act_mat, w_qtensor, bias):
         return quant_int8_dynamic_per_token_linear(
             act_mat, w_qtensor.int_data, w_qtensor.q_scales, bias, act_mat.dtype
@@ -227,30 +244,45 @@
             self.transposed,
             self.shape,
             **kwargs,
         )
 
     def _apply_fn_to_data(self, fn):
         return self.__class__(
-            fn(self.int_data), fn(self.q_scales), self.transposed, self.shape, dtype=self.dtype
+            fn(self.int_data),
+            fn(self.q_scales),
+            self.transposed,
+            self.shape,
+            dtype=self.dtype,
         )
 
+    #  `QuantizedLinearWeightBase` inconsistently.
+
     def _change_shape(self, shape):
         return self.__class__(
             self.int_data, self.q_scales, self.transposed, shape, dtype=self.dtype
         )
 
     def __tensor_flatten__(self):
         return ["int_data", "q_scales"], [self.transposed, self.dtype, self.shape]
 
     @classmethod
-    def __tensor_unflatten__(cls, tensor_data_dict, tensor_attributes, outer_size=None, outer_stride=None):
+    def __tensor_unflatten__(
+        cls, tensor_data_dict, tensor_attributes, outer_size=None, outer_stride=None
+    ):
         int_data, q_scales = tensor_data_dict["int_data"], tensor_data_dict["q_scales"]
         transposed, dtype, shape = tensor_attributes
-        return cls(int_data, q_scales, transposed, shape if outer_size is None else outer_size, dtype=dtype, strides=outer_stride)
+        return cls(
+            int_data,
+            q_scales,
+            transposed,
+            shape if outer_size is None else outer_size,
+            dtype=dtype,
+            strides=outer_stride,
+        )
 
     @classmethod
     def from_float(cls, input_float, qmin=-128, qmax=127):
         """
         Method used to convert a linear weight tensor to an instance of the
         Int8DynamicallyQuantizedLinearWeight subclass.
 
@@ -282,15 +314,21 @@
     changes the linear op to a weight-only quantized linear op with symmetric
     per-channel quantization on the weight.
     """
 
     @staticmethod
     def _quantized_op(act_mat, w_qtensor, bias):
         orig_dtype = act_mat.dtype
-        y = torch.mm(act_mat.reshape(-1, act_mat.shape[-1]), w_qtensor.int_data.to(act_mat.dtype)) * w_qtensor.q_scales
+        y = (
+            torch.mm(
+                act_mat.reshape(-1, act_mat.shape[-1]),
+                w_qtensor.int_data.to(act_mat.dtype),
+            )
+            * w_qtensor.q_scales
+        )
         y = y.reshape(*act_mat.shape[:-1], y.shape[-1])
         if bias is not None:
             y += bias
         return y.to(orig_dtype)
 
 
 class Int4WeightOnlyQuantizedLinearWeight(QuantizedLinearWeightBase):
@@ -324,16 +362,19 @@
         inner_k_tiles,
         **kwargs,
     ):
         # the transposed flag tracks whether the tensor subclass has been transposed relative
         # to how a weight is normally stored in a linear i.e. [out_features, in_features].
         # tracking both transposed and shape is slightly redundant but corner cases like
         # square matrices can cause issues otherwise
+
         self.scales_and_zeros = scales_and_zeros
+
         self.groupsize = groupsize
+
         self.inner_k_tiles = inner_k_tiles
         super().__init__(int_data, transposed)
 
     @staticmethod
     def _quantized_op(act_mat, w_qtensor, bias):
         orig_act_size = act_mat.size()
         orig_dtype = act_mat.dtype
@@ -341,19 +382,24 @@
         # reshape and pad activation
         act_mat = act_mat.reshape(-1, act_mat.shape[-1]).to(torch.bfloat16)
         pad_size = find_multiple(act_mat.shape[-1], 1024)
         act_mat = torch.nn.functional.pad(act_mat, (0, pad_size - act_mat.shape[-1]))
 
         # matmul
         y = aten._weight_int4pack_mm(
-            act_mat.contiguous(), w_qtensor.int_data, w_qtensor.groupsize, w_qtensor.scales_and_zeros
+            act_mat.contiguous(),
+            w_qtensor.int_data,
+            w_qtensor.groupsize,
+            w_qtensor.scales_and_zeros,
         )
 
         # remove out_feature padding
-        orig_out_features = w_qtensor.shape[-1] if w_qtensor.transposed else w_qtensor.shape[-2]
+        orig_out_features = (
+            w_qtensor.shape[-1] if w_qtensor.transposed else w_qtensor.shape[-2]
+        )
         y = y[:, :orig_out_features]
 
         y = y.reshape(*orig_act_size[:-1], orig_out_features)
         if bias is not None:
             y += bias
         return y.to(orig_dtype)
 
@@ -395,36 +441,43 @@
             self.transposed,
             self.shape,
             self.groupsize,
             self.inner_k_tiles,
             dtype=self.dtype,
         )
 
+    #  `QuantizedLinearWeightBase` inconsistently.
+
     def _change_shape(self, shape):
         return self.__class__(
             self.int_data,
             self.scales_and_zeros,
             self.transposed,
             shape,
             self.groupsize,
             self.inner_k_tiles,
-            dtype=self.dtype
+            dtype=self.dtype,
         )
 
     def __tensor_flatten__(self):
         return ["int_data", "scales_and_zeros"], (
             self.transposed,
             self.groupsize,
             self.inner_k_tiles,
             self.dtype,
-            self.shape
+            self.shape,
         )
 
     @classmethod
-    def __tensor_unflatten__(cls, tensor_data_dict, attributes, outer_size=None, outer_stride=None):
+
+    #  `QuantizedLinearWeightBase` inconsistently.
+
+    def __tensor_unflatten__(
+        cls, tensor_data_dict, attributes, outer_size=None, outer_stride=None
+    ):
         int_data, scales_and_zeros = (
             tensor_data_dict["int_data"],
             tensor_data_dict["scales_and_zeros"],
         )
         transposed, groupsize, inner_k_tiles, dtype, shape = attributes
         return cls(
             int_data,
@@ -454,24 +507,23 @@
         orig_shape = input_float.shape
         orig_out_features, orig_in_features = input_float.shape
 
         # padding
         in_features = find_multiple(orig_in_features, 1024)
         out_features = find_multiple(orig_out_features, 8)
         input_float = torch.nn.functional.pad(
-            input_float, (0, in_features - orig_in_features, 0, out_features - orig_out_features)
+            input_float,
+            (0, in_features - orig_in_features, 0, out_features - orig_out_features),
         )
 
         # quantization and packing
         input_int4x8, scales_and_zeros = groupwise_affine_quantize_tensor(
             input_float, 4, groupsize
         )
-        int_data = aten._convert_weight_to_int4pack(
-            input_int4x8, inner_k_tiles
-        )
+        int_data = aten._convert_weight_to_int4pack(input_int4x8, inner_k_tiles)
 
         return cls(
             int_data,
             scales_and_zeros,
             False,
             orig_shape,
             groupsize,
```

### Comparing `torchao-0.0.3/torchao/quantization/utils.py` & `torchao-0.1/torchao/quantization/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,53 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
-from typing import Dict, Optional
+from typing import Dict, Optional, Tuple
 
 import torch
 from torch.utils._python_dispatch import TorchDispatchMode
+from packaging import version
+from functools import reduce
+from math import gcd
+
 
 __all__ = [
     "find_multiple",
     "compute_error",
     "_apply_logging_hook",
     "get_model_size_in_bytes",
+    "TORCH_VERSION_AFTER_2_3",
 ]
 
 
-def find_multiple(n: int, k: int) -> int:
+def find_multiple(n: int, *args: Tuple[int]) -> int:
+    k: int = reduce(lambda x, y: x * y // gcd(x, y), args + (1,))  # type: ignore[9]
     if n % k == 0:
         return n
     return n + k - (n % k)
 
 
 # basic SQNR
+
+
 def compute_error(x, y):
     Ps = torch.linalg.norm(x)
     Pn = torch.linalg.norm(x - y)
     return 20 * torch.log10(Ps / Pn)
 
 
 # logger for fqn + op + shape
 # note: not safe for any kind of multithreading
 _cur_fqn: Optional[str] = None
 
 
 def _get_logging_hook(fqn):
+
     def forward_hook(module, input):
         global _cur_fqn
         _cur_fqn = fqn
 
     return forward_hook
 
 
@@ -50,14 +59,15 @@
 # collections.defaultdict printing is weird with lambdas, so hand writing for now
 _fqn_to_op_to_shape_to_count: Dict[
     Optional[str], Dict[Optional[str], Dict[Optional[str], int]]
 ] = {}
 
 
 class LoggingTensorMode(TorchDispatchMode):
+
     def __torch_dispatch__(self, func, types, args=(), kwargs=None):
         if kwargs is None:
             kwargs = {}
         rs = func(*args, **kwargs)
         global _cur_fqn
         op_name: str = f"{func.__module__}.{func.__name__}"
         shape_str = ""
@@ -75,14 +85,31 @@
             _fqn_to_op_to_shape_to_count[_cur_fqn][op_name][shape_str] = 0
         _fqn_to_op_to_shape_to_count[_cur_fqn][op_name][shape_str] += 1
 
         return rs
 
 
 # https://discuss.pytorch.org/t/finding-model-size/130275
+
+
 def get_model_size_in_bytes(model):
     s = 0
     for p in model.parameters():
         s += p.nelement() * p.element_size()
     for b in model.buffers():
         s += b.nelement() * b.element_size()
     return s
+
+if version.parse(torch.__version__) >= version.parse("2.4.0.dev"):
+    TORCH_VERSION_AFTER_2_4 = True
+else:
+    TORCH_VERSION_AFTER_2_4 = False
+
+if version.parse(torch.__version__) >= version.parse("2.3.0.dev"):
+    TORCH_VERSION_AFTER_2_3 = True
+else:
+    TORCH_VERSION_AFTER_2_3 = False
+
+if version.parse(torch.__version__) >= version.parse("2.2.0.dev"):
+    TORCH_VERSION_AFTER_2_2 = True
+else:
+    TORCH_VERSION_AFTER_2_2 = False
```

### Comparing `torchao-0.0.3/torchao/quantization/weight_only.py` & `torchao-0.1/torchao/quantization/weight_only.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import torch
-from .quant_primitives import (
-    dynamically_quantize_per_channel,
-)
+
+from .quant_primitives import dynamically_quantize_per_channel
 
 __all__ = ["WeightOnlyInt8QuantLinear"]
 
 
 class WeightOnlyInt8QuantLinear(torch.nn.Linear):
     """
     This class is a replacement for `torch.nn.Linear`. It implements a
     mixed dtype matmul using int8 symmetric per-channel weight quantization
     """
+
     def __init__(self, *args, **kwargs):
         w_int8 = kwargs.pop("w_int8")
         scales = kwargs.pop("scales")
         super().__init__(*args, **kwargs)
-        self.w_int8 = w_int8
-        self.scales = scales
+
+        self.register_buffer("w_int8", w_int8)
+        self.register_buffer("scales", scales)
 
     def forward(self, x, *args, **kwargs):
         """
         Performs the forward pass of the quantized linear layer which consists
         ofmixed dtype matmul using int8 symmetric per-channel weight quantization
 
         Args:
```

### Comparing `torchao-0.0.3/torchao/sparsity/utils.py` & `torchao-0.1/torchao/sparsity/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch
 from torch.ao.quantization.observer import UniformQuantizationObserverBase
 
 __all__ = ["PerChannelNormObserver"]
 
+
 # Observers
 class PerChannelNormObserver(UniformQuantizationObserverBase):
     """
     A custom observer that computes the L2 norm of each channel and stores it in a buffer.
     """
 
     def __init__(self, **kwargs) -> None:
@@ -20,14 +21,16 @@
             eps=torch.finfo(torch.float32).eps,
             **kwargs
         )
         # set averaging constant so quantization flow knows observer is memoryless.
         self.averaging_constant = 1.0
         self.register_buffer("norm", torch.tensor([]))
 
+    #  inconsistently.
+
     def forward(self, x_orig):
         if x_orig.numel() == 0:
             return x_orig
         x = x_orig.detach()  # avoid keeping autograd tape
 
         # channel_ax is always the last dimension
         new_axis_list = [i for i in range(x.dim())]  # noqa: C416
@@ -40,9 +43,13 @@
             self.norm.resize_(norm.shape)
             self.norm.copy_(norm)
         else:
             self.norm += norm
 
         return x_orig
 
+    #  inconsistently.
+
     def calculate_qparams(self):
-        raise NotImplementedError("PerChannelNormObserver is designed to store activations only. ")
+        raise NotImplementedError(
+            "PerChannelNormObserver is designed to store activations only. "
+        )
```

### Comparing `torchao-0.0.3/torchao/sparsity/wanda.py` & `torchao-0.1/torchao/sparsity/wanda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-
 import warnings
 
 from typing import Dict, List, Optional, Tuple
 
 import torch
 from torch import nn
 from torch.ao.pruning import BaseSparsifier
 from torch.ao.quantization import default_placeholder_observer, QConfig
 from torch.ao.quantization.quantize import _remove_qconfig
+
 from .utils import PerChannelNormObserver
 
 __all__ = ["WandaSparsifier"]
 
 
 class WandaSparsifier(BaseSparsifier):
     r"""Wanda sparsifier
@@ -40,14 +40,15 @@
         if semi_structured_block_size is not None:
             m = semi_structured_block_size
             warnings.warn(
                 f"WandaSparsifier got semi_structured_bock_size={m}, sparsity_level fixed to 50% ({m // 2}:{m}) sparsity"
             )
         super().__init__(defaults=defaults)
 
+    #  `typing.Dict[<key type>, <value type>]` to avoid runtime subscripting errors.
     def prepare(self, model: nn.Module, config: List[Dict]) -> None:
         # activation: use PerChannelNormObserver
         # use no-op placeholder weight observer
         model.qconfig = QConfig(
             activation=PerChannelNormObserver, weight=default_placeholder_observer
         )  # type: ignore[assignment]
         torch.ao.quantization.prepare(model, inplace=True)
```

### Comparing `torchao-0.0.3/torchao.egg-info/SOURCES.txt` & `torchao-0.1/torchao.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 LICENSE
 README.md
 setup.py
-test/test.py
 torchao/__init__.py
 torchao.egg-info/PKG-INFO
 torchao.egg-info/SOURCES.txt
 torchao.egg-info/dependency_links.txt
 torchao.egg-info/requires.txt
 torchao.egg-info/top_level.txt
+torchao/dtypes/__init__.py
+torchao/dtypes/nf4tensor.py
+torchao/dtypes/uint4.py
+torchao/kernel/__init__.py
+torchao/kernel/autotuner.py
+torchao/kernel/intmm.py
+torchao/kernel/intmm_triton.py
+torchao/quantization/GPTQ.py
 torchao/quantization/__init__.py
 torchao/quantization/dynamic_quant.py
 torchao/quantization/quant_api.py
 torchao/quantization/quant_primitives.py
 torchao/quantization/smoothquant.py
 torchao/quantization/subclass.py
+torchao/quantization/unified.py
 torchao/quantization/utils.py
 torchao/quantization/weight_only.py
 torchao/sparsity/__init__.py
 torchao/sparsity/utils.py
 torchao/sparsity/wanda.py
```

