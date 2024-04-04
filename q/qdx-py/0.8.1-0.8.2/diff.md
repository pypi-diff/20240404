# Comparing `tmp/qdx_py-0.8.1.tar.gz` & `tmp/qdx_py-0.8.2.tar.gz`

## Comparing `qdx_py-0.8.1.tar` & `qdx_py-0.8.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 qdx_py-0.8.1/Cargo.toml
--rw-r--r--   0     1000      100     2809 2023-11-16 02:44:04.000000 qdx_py-0.8.1/.github/workflows/CI.yml
--rw-r--r--   0     1000      100      685 2023-11-16 02:44:04.000000 qdx_py-0.8.1/.gitignore
--rw-r--r--   0     1000      100     2028 2024-04-04 02:54:02.000000 qdx_py-0.8.1/README.md
--rw-r--r--   0     1000      100     7833 2024-04-04 02:54:02.000000 qdx_py-0.8.1/src/lib.rs
--rw-r--r--   0     1000      100    27252 2024-04-04 02:56:16.000000 qdx_py-0.8.1/Cargo.lock
--rw-r--r--   0     1000      100      366 2023-12-01 06:07:08.000000 qdx_py-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 qdx_py-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 qdx_py-0.8.2/Cargo.toml
+-rw-r--r--   0     1000      100     2809 2023-11-16 02:44:04.000000 qdx_py-0.8.2/.github/workflows/CI.yml
+-rw-r--r--   0     1000      100      685 2023-11-16 02:44:04.000000 qdx_py-0.8.2/.gitignore
+-rw-r--r--   0     1000      100     2028 2024-04-04 02:54:02.000000 qdx_py-0.8.2/README.md
+-rw-r--r--   0     1000      100     7839 2024-04-04 06:34:15.000000 qdx_py-0.8.2/src/lib.rs
+-rw-r--r--   0     1000      100    27252 2024-04-04 06:35:23.000000 qdx_py-0.8.2/Cargo.lock
+-rw-r--r--   0     1000      100      366 2023-12-01 06:07:08.000000 qdx_py-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 qdx_py-0.8.2/PKG-INFO
```

### Comparing `qdx_py-0.8.1/Cargo.toml` & `qdx_py-0.8.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qdx-py"
-version = "0.8.1"
+version = "0.8.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "qdx_py"
 crate-type = ["rlib", "cdylib"]
```

### Comparing `qdx_py-0.8.1/.github/workflows/CI.yml` & `qdx_py-0.8.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `qdx_py-0.8.1/.gitignore` & `qdx_py-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qdx_py-0.8.1/README.md` & `qdx_py-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `qdx_py-0.8.1/src/lib.rs` & `qdx_py-0.8.2/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -149,18 +149,15 @@
         .perceive_bonds(strictness)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
     conformer
         .perceive_formal_charges()
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
-    conformer.topology.fragments =
-        Some(conformer.fragment_by_label());
-
-
+    conformer.fragment_by_label().map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     conformer.topology.assign_fragment_charges();
     
     assert!(conformer.is_valid());   
     
     serde_json::to_string(&conformer).map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
```

### Comparing `qdx_py-0.8.1/Cargo.lock` & `qdx_py-0.8.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -459,16 +459,16 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "qdx-common"
-version = "0.7.2"
-source = "git+ssh://git@github.com/talo/qdx-common.git#18b5a4343f0299e1b3c545d69ceb20e0afb3ecb7"
+version = "0.8.1"
+source = "git+ssh://git@github.com/talo/qdx-common.git#c96f8a19e4d0bbb4e34740dd33e8b6970930f09c"
 dependencies = [
  "anyhow",
  "assertables",
  "base64",
  "euclid",
  "half",
  "itertools",
@@ -487,15 +487,15 @@
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "qdx-py"
-version = "0.8.1"
+version = "0.8.2"
 dependencies = [
  "pyo3",
  "qdx-common",
  "serde",
  "serde_json",
 ]
```

### Comparing `qdx_py-0.8.1/PKG-INFO` & `qdx_py-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdx-py
-Version: 0.8.1
+Version: 0.8.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # QDX-py
```

