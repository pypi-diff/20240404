# Comparing `tmp/campie-0.4.0.tar.gz` & `tmp/campie-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "campie-0.4.0.tar", max compression
+gzip compressed data, was "campie-0.4.1.tar", max compression
```

## Comparing `campie-0.4.0.tar` & `campie-0.4.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11356 2024-03-21 20:26:37.268156 campie-0.4.0/LICENSE
--rw-r--r--   0        0        0     3400 2024-03-21 20:26:37.268226 campie-0.4.0/README.md
--rw-r--r--   0        0        0     1222 2024-03-21 20:26:37.268350 campie-0.4.0/campie/__init__.py
--rw-r--r--   0        0        0    12270 2024-03-21 20:26:37.268409 campie-0.4.0/campie/cam.py
--rw-r--r--   0        0        0     5980 2024-03-21 20:26:37.268488 campie-0.4.0/campie/kernel.py
--rw-r--r--   0        0        0        0 2024-03-21 20:26:37.268512 campie-0.4.0/campie/py.typed
--rw-r--r--   0        0        0     9194 2024-03-21 20:26:37.268608 campie-0.4.0/campie/run.py
--rw-r--r--   0        0        0     4020 2024-03-21 20:26:37.268673 campie-0.4.0/campie/types.py
--rw-r--r--   0        0        0      801 2024-03-21 20:26:37.268756 campie-0.4.0/campie/util/__init__.py
--rw-r--r--   0        0        0     4011 2024-03-21 20:26:37.268825 campie-0.4.0/campie/util/flip_indices.py
--rw-r--r--   0        0        0     1288 2024-03-21 20:26:37.268883 campie-0.4.0/campie/util/helpers.py
--rw-r--r--   0        0        0     3075 2024-03-21 20:26:37.268947 campie-0.4.0/campie/validation.py
--rw-r--r--   0        0        0      845 2024-03-21 20:27:26.930524 campie-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 campie-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-04-04 00:23:23.721804 campie-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3400 2024-04-04 00:23:23.721935 campie-0.4.1/README.md
+-rw-r--r--   0        0        0     1222 2024-04-04 00:23:23.722168 campie-0.4.1/campie/__init__.py
+-rw-r--r--   0        0        0    12332 2024-04-04 00:24:41.350085 campie-0.4.1/campie/cam.py
+-rw-r--r--   0        0        0     5980 2024-04-04 00:23:23.722499 campie-0.4.1/campie/kernel.py
+-rw-r--r--   0        0        0        0 2024-04-04 00:23:23.722558 campie-0.4.1/campie/py.typed
+-rw-r--r--   0        0        0     9194 2024-04-04 00:23:23.722763 campie-0.4.1/campie/run.py
+-rw-r--r--   0        0        0     4020 2024-04-04 00:23:23.722894 campie-0.4.1/campie/types.py
+-rw-r--r--   0        0        0      801 2024-04-04 00:23:23.723083 campie-0.4.1/campie/util/__init__.py
+-rw-r--r--   0        0        0     4011 2024-04-04 00:23:23.723209 campie-0.4.1/campie/util/flip_indices.py
+-rw-r--r--   0        0        0     1288 2024-04-04 00:23:23.723329 campie-0.4.1/campie/util/helpers.py
+-rw-r--r--   0        0        0     3075 2024-04-04 00:23:23.723457 campie-0.4.1/campie/validation.py
+-rw-r--r--   0        0        0      845 2024-04-04 00:24:05.165839 campie-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4330 1970-01-01 00:00:00.000000 campie-0.4.1/PKG-INFO
```

### Comparing `campie-0.4.0/LICENSE` & `campie-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/README.md` & `campie-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/campie/__init__.py` & `campie-0.4.1/campie/__init__.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/campie/cam.py` & `campie-0.4.1/campie/cam.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,16 @@
 
     ### Notes:
     - The arguments for ACAM operations must contain floating point data types.
     """
     variant, op, result_dtype = CamVariant.ACAM, CamOp.MATCH, np.int8
     validate_args(variant, op, inputs, cam)
     kernel = generate_kernel(variant, op, inputs.dtype, cam.dtype, result_dtype)
+    if noise is not None:
+        cam = add_noise(cam, noise)
     return run_kernel(kernel, variant, op, inputs, cam, result_dtype)
 
 
 def acam_count_mismatches(
     inputs: NDArray[TN], cam: NDArray[TN], *, noise: Optional[float] = None
 ) -> NDArray[np.int64]:
     """
```

### Comparing `campie-0.4.0/campie/kernel.py` & `campie-0.4.1/campie/kernel.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/campie/run.py` & `campie-0.4.1/campie/run.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/campie/types.py` & `campie-0.4.1/campie/types.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/campie/util/__init__.py` & `campie-0.4.1/campie/util/__init__.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/campie/util/flip_indices.py` & `campie-0.4.1/campie/util/flip_indices.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/campie/util/helpers.py` & `campie-0.4.1/campie/util/helpers.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/campie/validation.py` & `campie-0.4.1/campie/validation.py`

 * *Files identical despite different names*

### Comparing `campie-0.4.0/pyproject.toml` & `campie-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "campie"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python APIs to simulate various CAMs on GPUs at scale"
 readme = "README.md"
 authors = []
 repository = "https://github.com/HewlettPackard/CAMPIE"
 homepage = "https://github.com/HewlettPackard/CAMPIE#readme"
 packages = [{ include = "campie" }]
```

### Comparing `campie-0.4.0/PKG-INFO` & `campie-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: campie
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python APIs to simulate various CAMs on GPUs at scale
 Home-page: https://github.com/HewlettPackard/CAMPIE#readme
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

