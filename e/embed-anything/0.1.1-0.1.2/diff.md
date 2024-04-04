# Comparing `tmp/embed_anything-0.1.1.tar.gz` & `tmp/embed_anything-0.1.2.tar.gz`

## Comparing `embed_anything-0.1.1.tar` & `embed_anything-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 embed_anything-0.1.1/Cargo.toml
--rw-r--r--   0        0        0     3526 2024-03-31 23:05:19.000000 embed_anything-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2024-03-31 23:05:19.000000 embed_anything-0.1.1/.gitignore
--rw-r--r--   0        0        0     1411 2024-04-03 17:03:00.000000 embed_anything-0.1.1/README.md
--rw-r--r--   0        0        0      346 2024-03-31 23:05:19.000000 embed_anything-0.1.1/embed_anything.pyi
--rw-r--r--   0        0        0     2850 2024-03-31 23:05:19.000000 embed_anything-0.1.1/src/embed.rs
--rw-r--r--   0        0        0     1527 2024-03-31 23:05:19.000000 embed_anything-0.1.1/src/file_embed.rs
--rw-r--r--   0        0        0      924 2024-03-31 23:05:19.000000 embed_anything-0.1.1/src/lib.rs
--rw-r--r--   0        0        0      296 2024-03-31 23:05:19.000000 embed_anything-0.1.1/src/pdf_processor.rs
--rw-r--r--   0        0        0      129 2024-04-01 21:49:59.000000 embed_anything-0.1.1/test.py
--rw-r--r--   0        0        0    42778 2024-04-03 17:41:01.000000 embed_anything-0.1.1/Cargo.lock
--rw-r--r--   0        0        0      571 2024-04-03 17:31:33.000000 embed_anything-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 embed_anything-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 embed_anything-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0     3526 2024-03-31 23:05:19.000000 embed_anything-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1123 2024-04-04 15:11:59.000000 embed_anything-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      758 2024-03-31 23:05:19.000000 embed_anything-0.1.2/.gitignore
+-rw-r--r--   0        0        0    35823 2024-04-04 15:11:59.000000 embed_anything-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1431 2024-04-04 15:11:59.000000 embed_anything-0.1.2/README.md
+-rw-r--r--   0        0        0    17016 2024-04-04 13:30:00.000000 embed_anything-0.1.2/embed_anything-0.1.1.tar.gz
+-rw-r--r--   0        0        0      346 2024-03-31 23:05:19.000000 embed_anything-0.1.2/embed_anything.pyi
+-rw-r--r--   0        0        0     2850 2024-03-31 23:05:19.000000 embed_anything-0.1.2/src/embed.rs
+-rw-r--r--   0        0        0     1527 2024-03-31 23:05:19.000000 embed_anything-0.1.2/src/file_embed.rs
+-rw-r--r--   0        0        0      924 2024-03-31 23:05:19.000000 embed_anything-0.1.2/src/lib.rs
+-rw-r--r--   0        0        0      296 2024-03-31 23:05:19.000000 embed_anything-0.1.2/src/pdf_processor.rs
+-rw-r--r--   0        0        0      129 2024-04-01 21:49:59.000000 embed_anything-0.1.2/test.py
+-rw-r--r--   0        0        0    42778 2024-04-04 15:14:42.000000 embed_anything-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      571 2024-04-03 17:31:33.000000 embed_anything-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 embed_anything-0.1.2/PKG-INFO
```

### Comparing `embed_anything-0.1.1/Cargo.toml` & `embed_anything-0.1.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "embed_anything"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "embed_anything"
 crate-type = ["cdylib"]
```

### Comparing `embed_anything-0.1.1/.github/workflows/CI.yml` & `embed_anything-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.1/.gitignore` & `embed_anything-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.1/README.md` & `embed_anything-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# EmbedAnything
-# EmbedAnything
-
-EmbedAnything is a powerful library designed to streamline the creation and management of embedding pipelines. Whether you're working with text, images, audio, or any other type of data[Multimodality to be added], EmbedAnything makes it easy to generate embeddings from multiple sources and store them efficiently in a vector database.
-
-## Key Features
-
-- **Flexible:** Build custom embedding pipelines tailored to your needs.
-- **Efficient:** Optimized for speed and performance, with core functionality written in Rust.
-- **Scalable:** Store embeddings in a vector database for easy retrieval and scalability.
-- **Python Interface:** Packaged as a Python library for seamless integration into your existing projects.
-
-##ToDo
-- **Versatile:** Supports a wide range of data types, including text, images, audio, and more.
-- **Local embeddings** Release it for local embeddings as well
-- **Vector Database** Add functionalities to integrate with any Vector Database
-## Installation
-
-`
-pip install embed-anything`
-
-
-Requirements:
-
-Please check if you already have the OpenAI key in the Environment variable. We have only released the OpenAI embedder library so far. Please stay tuned for updates for the local embeddings as well.
-
-
-##Script:
-
-```python
-import embed_anything
-from embed_anything import EmbedData
-data = embed_anything.embed_file("filename.pdf")
-print(data[0])```
-
+# EmbedAnything
+
+
+EmbedAnything is a powerful library designed to streamline the creation and management of embedding pipelines. Whether you're working with text, images, audio, or any other type of data[Multimodality to be added], EmbedAnything makes it easy to generate embeddings from multiple sources and store them efficiently in a vector database.
+
+## Key Features
+
+- **Flexible:** Build custom embedding pipelines tailored to your needs.
+- **Efficient:** Optimized for speed and performance, with core functionality written in Rust.
+- **Scalable:** Store embeddings in a vector database for easy retrieval and scalability.
+- **Python Interface:** Packaged as a Python library for seamless integration into your existing projects.
+
+##ToDo
+- **Versatile:** Supports a wide range of data types, including text, images, audio, and more.
+- **Local embeddings** Release it for local embeddings as well
+- **Vector Database** Add functionalities to integrate with any Vector Database
+## Installation
+
+`
+pip install embed-anything`
+
+
+Requirements:
+
+Please check if you already have the OpenAI key in the Environment variable. We have only released the OpenAI embedder library so far. Please stay tuned for updates for the local embeddings as well.
+
+
+##Script:
+
+```python
+import embed_anything
+from embed_anything import EmbedData
+data = embed_anything.embed_file("filename.pdf")
+print(data[0])```
+
```

### Comparing `embed_anything-0.1.1/src/embed.rs` & `embed_anything-0.1.2/src/embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.1/src/file_embed.rs` & `embed_anything-0.1.2/src/file_embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.1/src/lib.rs` & `embed_anything-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.1/Cargo.lock` & `embed_anything-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "embed_anything"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "futures",
  "pdf-extract",
  "pyo3",
  "pyo3-asyncio",
  "reqwest",
  "serde",
```

### Comparing `embed_anything-0.1.1/pyproject.toml` & `embed_anything-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.1/PKG-INFO` & `embed_anything-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.3
 Name: embed_anything
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
 Summary: Embed anything at lightning speed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/StarlightSearch/EmbedAnything/tree/main
 
-# EmbedAnything
-# EmbedAnything
-
-EmbedAnything is a powerful library designed to streamline the creation and management of embedding pipelines. Whether you're working with text, images, audio, or any other type of data[Multimodality to be added], EmbedAnything makes it easy to generate embeddings from multiple sources and store them efficiently in a vector database.
-
-## Key Features
-
-- **Flexible:** Build custom embedding pipelines tailored to your needs.
-- **Efficient:** Optimized for speed and performance, with core functionality written in Rust.
-- **Scalable:** Store embeddings in a vector database for easy retrieval and scalability.
-- **Python Interface:** Packaged as a Python library for seamless integration into your existing projects.
-
-##ToDo
-- **Versatile:** Supports a wide range of data types, including text, images, audio, and more.
-- **Local embeddings** Release it for local embeddings as well
-- **Vector Database** Add functionalities to integrate with any Vector Database
-## Installation
-
-`
-pip install embed-anything`
-
-
-Requirements:
-
-Please check if you already have the OpenAI key in the Environment variable. We have only released the OpenAI embedder library so far. Please stay tuned for updates for the local embeddings as well.
-
-
-##Script:
-
-```python
-import embed_anything
-from embed_anything import EmbedData
-data = embed_anything.embed_file("filename.pdf")
-print(data[0])```
-
+# EmbedAnything
+
+
+EmbedAnything is a powerful library designed to streamline the creation and management of embedding pipelines. Whether you're working with text, images, audio, or any other type of data[Multimodality to be added], EmbedAnything makes it easy to generate embeddings from multiple sources and store them efficiently in a vector database.
+
+## Key Features
+
+- **Flexible:** Build custom embedding pipelines tailored to your needs.
+- **Efficient:** Optimized for speed and performance, with core functionality written in Rust.
+- **Scalable:** Store embeddings in a vector database for easy retrieval and scalability.
+- **Python Interface:** Packaged as a Python library for seamless integration into your existing projects.
+
+##ToDo
+- **Versatile:** Supports a wide range of data types, including text, images, audio, and more.
+- **Local embeddings** Release it for local embeddings as well
+- **Vector Database** Add functionalities to integrate with any Vector Database
+## Installation
+
+`
+pip install embed-anything`
+
+
+Requirements:
+
+Please check if you already have the OpenAI key in the Environment variable. We have only released the OpenAI embedder library so far. Please stay tuned for updates for the local embeddings as well.
+
+
+##Script:
+
+```python
+import embed_anything
+from embed_anything import EmbedData
+data = embed_anything.embed_file("filename.pdf")
+print(data[0])```
+
```

