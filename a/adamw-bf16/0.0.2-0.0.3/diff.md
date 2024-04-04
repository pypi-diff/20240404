# Comparing `tmp/adamw_bf16-0.0.2.tar.gz` & `tmp/adamw_bf16-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adamw_bf16-0.0.2.tar", last modified: Thu Apr  4 03:48:56 2024, max compression
+gzip compressed data, was "adamw_bf16-0.0.3.tar", last modified: Thu Apr  4 16:07:36 2024, max compression
```

## Comparing `adamw_bf16-0.0.2.tar` & `adamw_bf16-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 03:48:56.686738 adamw_bf16-0.0.2/
--rw-r--r--   0 user      (1000) user      (1000)    34523 2024-04-04 02:06:36.000000 adamw_bf16-0.0.2/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)     1652 2024-04-04 03:48:56.686738 adamw_bf16-0.0.2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1068 2024-04-04 02:44:26.000000 adamw_bf16-0.0.2/README.md
--rw-r--r--   0 user      (1000) user      (1000)      659 2024-04-04 03:47:12.000000 adamw_bf16-0.0.2/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-04 03:48:56.686738 adamw_bf16-0.0.2/setup.cfg
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 03:48:56.682738 adamw_bf16-0.0.2/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 03:48:56.686738 adamw_bf16-0.0.2/src/adamw_bf16/
--rw-r--r--   0 user      (1000) user      (1000)     5480 2024-04-04 03:48:12.000000 adamw_bf16-0.0.2/src/adamw_bf16/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 03:48:56.686738 adamw_bf16-0.0.2/src/adamw_bf16/stochastic/
--rw-r--r--   0 user      (1000) user      (1000)     3561 2024-04-04 02:20:32.000000 adamw_bf16-0.0.2/src/adamw_bf16/stochastic/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 03:48:56.686738 adamw_bf16-0.0.2/src/adamw_bf16.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1652 2024-04-04 03:48:56.000000 adamw_bf16-0.0.2/src/adamw_bf16.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      290 2024-04-04 03:48:56.000000 adamw_bf16-0.0.2/src/adamw_bf16.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-04 03:48:56.000000 adamw_bf16-0.0.2/src/adamw_bf16.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2024-04-04 03:48:56.000000 adamw_bf16-0.0.2/src/adamw_bf16.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2024-04-04 03:48:56.000000 adamw_bf16-0.0.2/src/adamw_bf16.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 16:07:36.507442 adamw_bf16-0.0.3/
+-rw-r--r--   0 user      (1000) user      (1000)    34523 2024-04-04 02:06:36.000000 adamw_bf16-0.0.3/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1652 2024-04-04 16:07:36.507442 adamw_bf16-0.0.3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1068 2024-04-04 02:44:26.000000 adamw_bf16-0.0.3/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      659 2024-04-04 16:06:17.000000 adamw_bf16-0.0.3/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-04 16:07:36.507442 adamw_bf16-0.0.3/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 16:07:36.507442 adamw_bf16-0.0.3/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 16:07:36.507442 adamw_bf16-0.0.3/src/adamw_bf16/
+-rw-r--r--   0 user      (1000) user      (1000)     5481 2024-04-04 16:06:37.000000 adamw_bf16-0.0.3/src/adamw_bf16/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 16:07:36.507442 adamw_bf16-0.0.3/src/adamw_bf16/stochastic/
+-rw-r--r--   0 user      (1000) user      (1000)     3573 2024-04-04 16:05:56.000000 adamw_bf16-0.0.3/src/adamw_bf16/stochastic/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-04 16:07:36.507442 adamw_bf16-0.0.3/src/adamw_bf16.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1652 2024-04-04 16:07:36.000000 adamw_bf16-0.0.3/src/adamw_bf16.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      290 2024-04-04 16:07:36.000000 adamw_bf16-0.0.3/src/adamw_bf16.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-04 16:07:36.000000 adamw_bf16-0.0.3/src/adamw_bf16.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2024-04-04 16:07:36.000000 adamw_bf16-0.0.3/src/adamw_bf16.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       11 2024-04-04 16:07:36.000000 adamw_bf16-0.0.3/src/adamw_bf16.egg-info/top_level.txt
```

### Comparing `adamw_bf16-0.0.2/LICENSE.txt` & `adamw_bf16-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adamw_bf16-0.0.2/PKG-INFO` & `adamw_bf16-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adamw_bf16
-Version: 0.0.2
+Version: 0.0.3
 Summary: AdamW Optimizer for bfloat16
 Author-email: APJC <apjc@usa.com>
 Project-URL: Homepage, https://github.com/AmericanPresidentJimmyCarter/adamw-bf16
 Project-URL: Issues, https://github.com/AmericanPresidentJimmyCarter/adamw-bf16/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `adamw_bf16-0.0.2/README.md` & `adamw_bf16-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `adamw_bf16-0.0.2/pyproject.toml` & `adamw_bf16-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "adamw_bf16"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="APJC", email="apjc@usa.com" },
 ]
 description = "AdamW Optimizer for bfloat16"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `adamw_bf16-0.0.2/src/adamw_bf16/__init__.py` & `adamw_bf16-0.0.3/src/adamw_bf16/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 __all__ = ["AdamWBF16"]
 
 
 import torch
 from torch.optim.optimizer import Optimizer, _use_grad_for_differentiable
 
 from .stochastic import (
     add_stochastic_,
     addcdiv_stochastic_,
 )
 
+
 class AdamWBF16(Optimizer):
     decay_threshold = 5e-3
 
     def __init__(
         self,
         params,
         *,
```

### Comparing `adamw_bf16-0.0.2/src/adamw_bf16/stochastic/__init__.py` & `adamw_bf16-0.0.3/src/adamw_bf16/stochastic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from torch import Tensor
+from torch import Tensor, FloatTensor
 
 
 def swap_first_and_last_dims(tensor: torch.Tensor) -> torch.Tensor:
     """
     Swap the first dimension with the last dimension of a tensor.
     
     Args:
@@ -71,36 +71,41 @@
     del result
 
 
 def add_stochastic_(_input: Tensor, other: Tensor, alpha: float = 1.0):
     """
     Adds other to input using stochastic rounding.
 
-    There is a hack to fix a bug on MPS where uneven final dimensions cause
-    a crash.
+    There is a hack to fix a bug on MPS where the wrong dtype is used with
+    alpha.
 
     Args:
         _input: the input tensor with dtype=bfloat16
         other: the other tensor
         alpha: a multiplier for other
     """
+    _input_original = _input
+    if _input.device.type == 'mps':
+        _input = _input.to(dtype=torch.float32)
+
     if other.dtype == torch.float32:
         result = other.clone()
     else:
         result = other.to(dtype=torch.float32)
 
-    if _input.size(-1) % 2 != 0 and _input.device.type == 'mps':
-        _input = swap_first_and_last_dims(_input)
-        result = swap_first_and_last_dims(result)
-    result.add_(_input, alpha=alpha)
-    if _input.size(-1) % 2 != 0 and _input.device.type == 'mps':
-        _input = swap_back_first_and_last_dims(_input)
-        result = swap_back_first_and_last_dims(result)
+    if _input.device.type == 'mps':
+        result.add_(_input, alpha=torch.tensor(alpha, dtype=torch.float32))
+    else:
+        result.add_(_input, alpha=alpha)
+
     copy_stochastic_(_input, result)
 
+    if _input.device.type == 'mps':
+        _input_original.copy_(_input.view(dtype=torch.float32))
+
 
 def addcdiv_stochastic_(_input: Tensor, tensor1: Tensor, tensor2: Tensor, value: float = 1.0):
     """
     adds (tensor1 / tensor2 * value) to input using stochastic rounding
 
     Args:
         _input: the input tensor with dtype=bfloat16
```

### Comparing `adamw_bf16-0.0.2/src/adamw_bf16.egg-info/PKG-INFO` & `adamw_bf16-0.0.3/src/adamw_bf16.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adamw_bf16
-Version: 0.0.2
+Version: 0.0.3
 Summary: AdamW Optimizer for bfloat16
 Author-email: APJC <apjc@usa.com>
 Project-URL: Homepage, https://github.com/AmericanPresidentJimmyCarter/adamw-bf16
 Project-URL: Issues, https://github.com/AmericanPresidentJimmyCarter/adamw-bf16/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

