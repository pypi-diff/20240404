# Comparing `tmp/embed_anything-0.1.2.tar.gz` & `tmp/embed_anything-0.1.3.tar.gz`

## Comparing `embed_anything-0.1.2.tar` & `embed_anything-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 embed_anything-0.1.2/Cargo.toml
--rw-r--r--   0        0        0     3526 2024-03-31 23:05:19.000000 embed_anything-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1123 2024-04-04 15:11:59.000000 embed_anything-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      758 2024-03-31 23:05:19.000000 embed_anything-0.1.2/.gitignore
--rw-r--r--   0        0        0    35823 2024-04-04 15:11:59.000000 embed_anything-0.1.2/LICENSE
--rw-r--r--   0        0        0     1431 2024-04-04 15:11:59.000000 embed_anything-0.1.2/README.md
--rw-r--r--   0        0        0    17016 2024-04-04 13:30:00.000000 embed_anything-0.1.2/embed_anything-0.1.1.tar.gz
--rw-r--r--   0        0        0      346 2024-03-31 23:05:19.000000 embed_anything-0.1.2/embed_anything.pyi
--rw-r--r--   0        0        0     2850 2024-03-31 23:05:19.000000 embed_anything-0.1.2/src/embed.rs
--rw-r--r--   0        0        0     1527 2024-03-31 23:05:19.000000 embed_anything-0.1.2/src/file_embed.rs
--rw-r--r--   0        0        0      924 2024-03-31 23:05:19.000000 embed_anything-0.1.2/src/lib.rs
--rw-r--r--   0        0        0      296 2024-03-31 23:05:19.000000 embed_anything-0.1.2/src/pdf_processor.rs
--rw-r--r--   0        0        0      129 2024-04-01 21:49:59.000000 embed_anything-0.1.2/test.py
--rw-r--r--   0        0        0    42778 2024-04-04 15:14:42.000000 embed_anything-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      571 2024-04-03 17:31:33.000000 embed_anything-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 embed_anything-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 embed_anything-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0     3526 2024-03-31 23:05:19.000000 embed_anything-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1123 2024-04-04 15:11:59.000000 embed_anything-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      758 2024-03-31 23:05:19.000000 embed_anything-0.1.3/.gitignore
+-rw-r--r--   0        0        0    35823 2024-04-04 15:11:59.000000 embed_anything-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1431 2024-04-04 15:11:59.000000 embed_anything-0.1.3/README.md
+-rw-r--r--   0        0        0    17016 2024-04-04 13:30:00.000000 embed_anything-0.1.3/embed_anything-0.1.1.tar.gz
+-rw-r--r--   0        0        0      346 2024-03-31 23:05:19.000000 embed_anything-0.1.3/embed_anything.pyi
+-rw-r--r--   0        0        0     2850 2024-03-31 23:05:19.000000 embed_anything-0.1.3/src/embed.rs
+-rw-r--r--   0        0        0     1527 2024-03-31 23:05:19.000000 embed_anything-0.1.3/src/file_embed.rs
+-rw-r--r--   0        0        0      924 2024-03-31 23:05:19.000000 embed_anything-0.1.3/src/lib.rs
+-rw-r--r--   0        0        0      296 2024-03-31 23:05:19.000000 embed_anything-0.1.3/src/pdf_processor.rs
+-rw-r--r--   0        0        0      129 2024-04-01 21:49:59.000000 embed_anything-0.1.3/test.py
+-rw-r--r--   0        0        0    42778 2024-04-04 15:48:57.000000 embed_anything-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      601 2024-04-04 15:40:45.000000 embed_anything-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 embed_anything-0.1.3/PKG-INFO
```

### Comparing `embed_anything-0.1.2/Cargo.toml` & `embed_anything-0.1.3/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "embed_anything"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "embed_anything"
 crate-type = ["cdylib"]
```

### Comparing `embed_anything-0.1.2/.github/workflows/CI.yml` & `embed_anything-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/.github/workflows/python-publish.yml` & `embed_anything-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/.gitignore` & `embed_anything-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/LICENSE` & `embed_anything-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/README.md` & `embed_anything-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/embed_anything-0.1.1.tar.gz` & `embed_anything-0.1.3/embed_anything-0.1.1.tar.gz`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/src/embed.rs` & `embed_anything-0.1.3/src/embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/src/file_embed.rs` & `embed_anything-0.1.3/src/file_embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/src/lib.rs` & `embed_anything-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.2/Cargo.lock` & `embed_anything-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "embed_anything"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "futures",
  "pdf-extract",
  "pyo3",
  "pyo3-asyncio",
  "reqwest",
  "serde",
```

### Comparing `embed_anything-0.1.2/pyproject.toml` & `embed_anything-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -11,10 +11,11 @@
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = ["version"]
 [tool.maturin]
 features = ["pyo3/extension-module"]
+license = {file = "LICENSE"}
 
 [project.urls]
 Homepage = "https://github.com/StarlightSearch/EmbedAnything/tree/main"
```

### Comparing `embed_anything-0.1.2/PKG-INFO` & `embed_anything-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: embed_anything
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Embed anything at lightning speed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

