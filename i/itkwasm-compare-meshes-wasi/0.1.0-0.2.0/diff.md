# Comparing `tmp/itkwasm_compare_meshes_wasi-0.1.0.tar.gz` & `tmp/itkwasm_compare_meshes_wasi-0.2.0.tar.gz`

## Comparing `itkwasm_compare_meshes_wasi-0.1.0.tar` & `itkwasm_compare_meshes_wasi-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/itkwasm_compare_meshes_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/itkwasm_compare_meshes_wasi/_version.py
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/itkwasm_compare_meshes_wasi/compare_meshes.py
--rwxr-xr-x   0        0        0  2561276 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/itkwasm_compare_meshes_wasi/wasm_modules/compare-meshes.wasi.wasm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/tests/common.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/tests/test_compare_meshes.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/.gitignore
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/README.md
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/_version.py
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/compare_meshes.py
+-rwxr-xr-x   0        0        0  1183927 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/wasm_modules/compare-meshes.wasi.wasm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/tests/common.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/tests/test_compare_meshes.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/.gitignore
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/README.md
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/PKG-INFO
```

### Comparing `itkwasm_compare_meshes_wasi-0.1.0/itkwasm_compare_meshes_wasi/compare_meshes.py` & `itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/compare_meshes.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_meshes_wasi-0.1.0/README.md` & `itkwasm_compare_meshes_wasi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_meshes_wasi-0.1.0/pyproject.toml` & `itkwasm_compare_meshes_wasi-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_meshes_wasi-0.1.0/PKG-INFO` & `itkwasm_compare_meshes_wasi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkwasm-compare-meshes-wasi
-Version: 0.1.0
+Version: 0.2.0
 Summary: Compare meshes and polydata for regression testing.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

