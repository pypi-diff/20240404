# Comparing `tmp/py_rust_regex-0.1.0.tar.gz` & `tmp/py_rust_regex-0.1.1.tar.gz`

## Comparing `py_rust_regex-0.1.0.tar` & `py_rust_regex-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 py_rust_regex-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     3526 2024-04-04 02:16:58.000000 py_rust_regex-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-04-04 02:16:58.000000 py_rust_regex-0.1.0/.gitignore
--rw-r--r--   0      501       20      585 2024-04-04 02:17:32.000000 py_rust_regex-0.1.0/src/lib.rs
--rw-r--r--   0      501       20     9021 2024-04-04 02:25:13.000000 py_rust_regex-0.1.0/Cargo.lock
--rw-r--r--   0      501       20      393 2024-04-04 02:16:58.000000 py_rust_regex-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      262 1970-01-01 00:00:00.000000 py_rust_regex-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 py_rust_regex-0.1.1/Cargo.toml
+-rw-r--r--   0      501       20     3526 2024-04-04 02:16:58.000000 py_rust_regex-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      686 2024-04-04 02:16:58.000000 py_rust_regex-0.1.1/.gitignore
+-rw-r--r--   0      501       20      271 2024-04-04 04:10:13.000000 py_rust_regex-0.1.1/README.md
+-rw-r--r--   0      501       20     2387 2024-04-04 04:06:03.000000 py_rust_regex-0.1.1/src/lib.rs
+-rw-r--r--   0      501       20     9021 2024-04-04 04:11:51.000000 py_rust_regex-0.1.1/Cargo.lock
+-rw-r--r--   0      501       20      393 2024-04-04 02:16:58.000000 py_rust_regex-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 py_rust_regex-0.1.1/PKG-INFO
```

### Comparing `py_rust_regex-0.1.0/.github/workflows/CI.yml` & `py_rust_regex-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `py_rust_regex-0.1.0/.gitignore` & `py_rust_regex-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `py_rust_regex-0.1.0/Cargo.lock` & `py_rust_regex-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-rust-regex"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
  "regex",
 ]
 
 [[package]]
 name = "pyo3"
```

